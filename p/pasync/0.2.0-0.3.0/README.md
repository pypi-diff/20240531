# Comparing `tmp/pasync-0.2.0.tar.gz` & `tmp/pasync-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasync-0.2.0.tar", max compression
+gzip compressed data, was "pasync-0.3.0.tar", max compression
```

## Comparing `pasync-0.2.0.tar` & `pasync-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    11357 2024-05-29 02:09:04.511627 pasync-0.2.0/LICENSE
--rw-r--r--   0        0        0       49 2024-05-29 20:59:19.150246 pasync-0.2.0/README.md
--rw-r--r--   0        0        0      138 2024-05-29 20:25:23.140401 pasync-0.2.0/pasync/__init__.py
--rw-r--r--   0        0        0     3025 2024-05-30 15:21:56.014275 pasync-0.2.0/pasync/event_loop.py
--rw-r--r--   0        0        0     4290 2024-05-29 19:53:12.840550 pasync-0.2.0/pasync/promise/__init__.py
--rw-r--r--   0        0        0     1607 2024-05-30 17:32:37.083665 pasync-0.2.0/pasync/runner/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 03:42:13.701194 pasync-0.2.0/pasync/stream/__init__.py
--rw-r--r--   0        0        0      357 2024-05-30 17:28:54.323688 pasync-0.2.0/pasync/task.py
--rw-r--r--   0        0        0        0 2024-05-29 03:01:17.641390 pasync-0.2.0/pasync/utils/__init__.py
--rw-r--r--   0        0        0       35 2024-05-29 03:04:35.031383 pasync-0.2.0/pasync/utils/sleep.py
--rw-r--r--   0        0        0      370 2024-05-30 17:33:34.453663 pasync-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      462 1970-01-01 00:00:00.000000 pasync-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-29 02:09:04.511627 pasync-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1474 2024-05-30 17:50:50.193590 pasync-0.3.0/README.md
+-rw-r--r--   0        0        0      117 2024-05-30 17:58:31.783554 pasync-0.3.0/pasync/__init__.py
+-rw-r--r--   0        0        0     3025 2024-05-30 18:54:25.603284 pasync-0.3.0/pasync/event_loop.py
+-rw-r--r--   0        0        0     5457 2024-05-31 02:31:03.095588 pasync-0.3.0/pasync/promise/__init__.py
+-rw-r--r--   0        0        0     1608 2024-05-30 18:58:32.513258 pasync-0.3.0/pasync/runner/__init__.py
+-rw-r--r--   0        0        0      357 2024-05-31 01:40:14.751431 pasync-0.3.0/pasync/task.py
+-rw-r--r--   0        0        0        0 2024-05-29 03:01:17.641390 pasync-0.3.0/pasync/utils/__init__.py
+-rw-r--r--   0        0        0       35 2024-05-29 03:04:35.031383 pasync-0.3.0/pasync/utils/sleep.py
+-rw-r--r--   0        0        0      370 2024-05-31 02:34:00.915572 pasync-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1843 1970-01-01 00:00:00.000000 pasync-0.3.0/PKG-INFO
```

### Comparing `pasync-0.2.0/LICENSE` & `pasync-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pasync-0.2.0/pasync/event_loop.py` & `pasync-0.3.0/pasync/event_loop.py`

 * *Files identical despite different names*

### Comparing `pasync-0.2.0/pasync/promise/__init__.py` & `pasync-0.3.0/pasync/promise/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,110 +1,146 @@
 from __future__ import annotations
 
 from enum import Enum
 import inspect
 
 from typing import Any, Callable, Awaitable, Generic, Optional, TypeVar, Union
 
-from pasync.task import Task as _Task
-
 T1 = TypeVar("T1")
 E1 = TypeVar("E1")
 T2 = TypeVar("T2")
 E2 = TypeVar("E2")
 T3 = TypeVar("T3")
 E3 = TypeVar("E3")
 
 class PromiseState(Enum):
     Uninitiated = 0
     Pending = 1
     Fulfilled = 2
     Error = 3
 
-class Promise(Generic[T1, E1, T2, E2]):
+class Promise(Generic[T1, E1, T2, E2], Awaitable):
     def __init__(
         self,
         callback: Union[
             Callable[[Callable[[T1], None], Callable[[Union[E1, Exception]], None]], Any],
             Callable[[Callable[[T1], None], Callable[[Union[E1, Exception]], None]], Awaitable[T1]]]
     ):
         self.__state = PromiseState.Uninitiated
         self.__result: Optional[T1] = None
         self.__error: Optional[Union[E1, Exception]] = None
         disable_error = False
 
         def resolve(value: T1):
             if inspect.isawaitable(value):
-                self.__task = _Task(value)
+                async def wrapper():
+                    try:
+                        resolve(await value)
+                    except Exception as e:
+                        reject(e)
+
+                self.__awaitable = wrapper()
+
                 return
+
+            self.__awaitable = None
+
             nonlocal disable_error
             self.__result = value
             disable_error = True
             self.__state = PromiseState.Fulfilled
 
         def reject(error: Union[E1, Exception]):
+            if inspect.isawaitable(error):
+                async def wrapper():
+                    try:
+                        reject(await error)
+                    except Exception as e:
+                        reject(e)
+
+                self.__awaitable = wrapper()
+
+                return
+            self.__awaitable = None
             nonlocal disable_error
             self.__error = error
             disable_error = True
             self.__state = PromiseState.Error
 
         async def asyncified():
             try:
                 self.__state = PromiseState.Pending
                 result = callback(resolve, reject)
                 if inspect.isawaitable(result):
                     await result
+                
+                if inspect.isawaitable(self.__result):
+                    self.__result = await self.__result
+
+                return self.__result
             except Exception as e:
                 if not disable_error:
                     reject(e)
+                else:
+                    raise e
         
         self.__awaitable = asyncified()
-        self.__task = _Task(self.__awaitable)
 
     @property
     def state(self):
         return self.__state
 
-    @property
-    def task(self):
-        return self.__task
+    def __await__(self):
+        result = None
+
+        if not self.__awaitable:
+            async def identity():
+                return self.__result
+            result = yield from identity().__await__()
+        while self.__awaitable:
+            result = yield from self.__awaitable.__await__()
+
+        self.__result = result
+
+        return result
 
     def then(
         self,
         next: Union[
             Callable[[T1], T2],
             Callable[[T1], Awaitable[T2]]],
         handle: Optional[Union[
             Callable[[E1], T2],
-            Callable[[E1], Awaitable[T2]]]],
+            Callable[[E1], Awaitable[T2]]]] = None,
     ) -> Promise[T2, E2, T3, E3]:
         async def thenify(
             resolve: Callable[[T2], None],
             reject: Callable[[Union[E2, Exception]], None],
         ) -> Any:
-            await self.__awaitable
+            await self
             try:
                 match self.__state:
                     case PromiseState.Fulfilled:
                         any_result: Any = self.__result
                         resolve_result = next(any_result)
                         while inspect.isawaitable(resolve_result):
                             resolve_result = await resolve_result
                         resolve_result: Any = resolve_result
                         resolve(resolve_result)
+                        return resolve_result
                     case PromiseState.Error:
                         any_error: Any = self.__error
                         if not handle:
                             reject(any_error)
                             return
-                        handle_result = handle(any_error)
+                        handle_result: Any = handle(any_error)
                         while inspect.isawaitable(handle_result):
                             handle_result = await handle_result 
-                        handle_result: Any = handle_result
                         resolve(handle_result)
+                        return handle_result
             except Exception as e:
                 reject(e)
 
         return Promise(thenify)
     
     def catch(
         self,
@@ -112,20 +148,23 @@
             Callable[[E1], T2],
             Callable[[E1], Awaitable[T2]]],
     ) -> Promise[T2, E2, T3, E3]:
         async def catchify(
             resolve: Callable[[T2], None],
             reject: Callable[[Union[E2, Exception]], None],
         ) -> Any:
-            await self.__awaitable
+            await self
             try:
                 if self.__state == PromiseState.Error:
                     any_error: Any = self.__error
                     handle_result = handle(any_error)
                     while inspect.isawaitable(handle_result):
                         handle_result = await handle_result 
                     handle_result: Any = handle_result
                     resolve(handle_result)
+                elif self.__state == PromiseState.Fulfilled:
+                    any_result: Any = self.__result
+                    resolve(any_result)
             except Exception as e:
                 reject(e)
 
         return Promise(catchify)
```

### Comparing `pasync-0.2.0/pasync/runner/__init__.py` & `pasync-0.3.0/pasync/runner/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         if self.__non_blocking:
             self.__run_non_blocking(*tasks)
         else:
             self.__run_blocking(*tasks)
             return [task.last_result for task in tasks]
 
     def run_task(self, awaitable: Awaitable):
+
         task = _Task(awaitable)
         if self.__non_blocking:
             self.__run_non_blocking(task)
         else:
             self.__run_blocking(task)
             return task.last_result
```

