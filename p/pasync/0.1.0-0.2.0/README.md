# Comparing `tmp/pasync-0.1.0.tar.gz` & `tmp/pasync-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasync-0.1.0.tar", max compression
+gzip compressed data, was "pasync-0.2.0.tar", max compression
```

## Comparing `pasync-0.1.0.tar` & `pasync-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2024-05-29 02:09:04.511627 pasync-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2024-05-29 02:32:59.521523 pasync-0.1.0/README.md
--rw-r--r--   0        0        0      138 2024-05-29 20:25:23.140401 pasync-0.1.0/pasync/__init__.py
--rw-r--r--   0        0        0     2718 2024-05-29 20:53:55.730276 pasync-0.1.0/pasync/event_loop.py
--rw-r--r--   0        0        0     4290 2024-05-29 19:53:12.840550 pasync-0.1.0/pasync/promise/__init__.py
--rw-r--r--   0        0        0     1332 2024-05-29 20:40:44.990327 pasync-0.1.0/pasync/runner/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 03:42:13.701194 pasync-0.1.0/pasync/stream/__init__.py
--rw-r--r--   0        0        0      246 2024-05-29 18:09:03.221030 pasync-0.1.0/pasync/task.py
--rw-r--r--   0        0        0        0 2024-05-29 03:01:17.641390 pasync-0.1.0/pasync/utils/__init__.py
--rw-r--r--   0        0        0       35 2024-05-29 03:04:35.031383 pasync-0.1.0/pasync/utils/sleep.py
--rw-r--r--   0        0        0      370 2024-05-29 02:46:15.661462 pasync-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      414 1970-01-01 00:00:00.000000 pasync-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-29 02:09:04.511627 pasync-0.2.0/LICENSE
+-rw-r--r--   0        0        0       49 2024-05-29 20:59:19.150246 pasync-0.2.0/README.md
+-rw-r--r--   0        0        0      138 2024-05-29 20:25:23.140401 pasync-0.2.0/pasync/__init__.py
+-rw-r--r--   0        0        0     3025 2024-05-30 15:21:56.014275 pasync-0.2.0/pasync/event_loop.py
+-rw-r--r--   0        0        0     4290 2024-05-29 19:53:12.840550 pasync-0.2.0/pasync/promise/__init__.py
+-rw-r--r--   0        0        0     1607 2024-05-30 17:32:37.083665 pasync-0.2.0/pasync/runner/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 03:42:13.701194 pasync-0.2.0/pasync/stream/__init__.py
+-rw-r--r--   0        0        0      357 2024-05-30 17:28:54.323688 pasync-0.2.0/pasync/task.py
+-rw-r--r--   0        0        0        0 2024-05-29 03:01:17.641390 pasync-0.2.0/pasync/utils/__init__.py
+-rw-r--r--   0        0        0       35 2024-05-29 03:04:35.031383 pasync-0.2.0/pasync/utils/sleep.py
+-rw-r--r--   0        0        0      370 2024-05-30 17:33:34.453663 pasync-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      462 1970-01-01 00:00:00.000000 pasync-0.2.0/PKG-INFO
```

### Comparing `pasync-0.1.0/LICENSE` & `pasync-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pasync-0.1.0/pasync/event_loop.py` & `pasync-0.2.0/pasync/event_loop.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 from enum import Enum
 import threading
-from typing import Awaitable, List, Optional
+from typing import Awaitable, Optional, Union
 from collections import deque
 from threading import Thread
 
 from pasync.task import Task as _Task
 
 class _RunMode(Enum):
     IDLE = 0
     BLOCKING = 1
     NON_BLOCKING = 2
     STOP_SIGNALLED = 3
 
 class EventLoop():
-    def __init__(self, *tasks: List[_Task]):
-        self.__task_queue = deque(tasks) 
+    def __init__(self, *tasks: Union[Awaitable, _Task]):
+        self.__task_queue = deque([_Task(task) if not isinstance(task, _Task) else task for task in tasks])
         self.__run_mode = _RunMode.IDLE
         self.__push_cv = threading.Condition()
         self.__thread = None
 
-    def queue(self, awaitable: Awaitable):
+    def queue(self, task: Union[Awaitable, _Task]):
         if self.__run_mode == _RunMode.STOP_SIGNALLED:
-            raise Exception("Warning: Queuing a task on an event queue that was signalled to stop has no effect") 
+            raise Exception("Queuing a task on an event queue that was signalled to stop has no effect") 
 
-        self.__queue(_Task(awaitable))
+        if self.__run_mode == _RunMode.BLOCKING:
+            raise Exception("Can not queue a task on an already running blocking event loop")
+
+        if not isinstance(task, _Task):
+            self.__queue(_Task(task))
+        else:
+            self.__queue(task)
         
         if self.__run_mode == _RunMode.NON_BLOCKING:
             with self.__push_cv:
                 self.__push_cv.notify()
 
     def signal_stop(self):
         self.__run_mode = _RunMode.STOP_SIGNALLED
```

### Comparing `pasync-0.1.0/pasync/promise/__init__.py` & `pasync-0.2.0/pasync/promise/__init__.py`

 * *Files identical despite different names*

### Comparing `pasync-0.1.0/pasync/runner/__init__.py` & `pasync-0.2.0/pasync/runner/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,48 @@
 from typing import Awaitable
 from pasync.event_loop import EventLoop
+from pasync.task import Task as _Task
 
 
 class Runner():
     def __init__(self, *, event_loop = None, non_blocking = False):
         self.__event_loop = event_loop or EventLoop()
         self.__non_blocking = non_blocking
         self.__is_non_blocking_running = False
 
-    def __enter__(self, *, event_loop = None, non_blocking = False):
+    def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, exc_msg):
         self.close()
         return False
 
     def close(self):
         if self.__is_non_blocking_running and self.__event_loop.thread:
             self.__event_loop.signal_stop()
             self.__event_loop.thread.join()
 
-    def run(self, awaitable: Awaitable, *awaitables: Awaitable):
+    def gather(self, *awaitables: Awaitable):
+        tasks = [_Task(awaitable) for awaitable in awaitables]
         if self.__non_blocking:
-            self.__run_non_blocking(awaitable, *awaitables)
+            self.__run_non_blocking(*tasks)
         else:
-            self.__run_blocking(awaitable, *awaitables)
+            self.__run_blocking(*tasks)
+            return [task.last_result for task in tasks]
+
+    def run_task(self, awaitable: Awaitable):
+        task = _Task(awaitable)
+        if self.__non_blocking:
+            self.__run_non_blocking(task)
+        else:
+            self.__run_blocking(task)
+            return task.last_result
         
-    def __run_blocking(self, *awaitables: Awaitable):
-        [self.__event_loop.queue(task) for task in awaitables]
+    def __run_blocking(self, *tasks: _Task):
+        [self.__event_loop.queue(task) for task in tasks]
         self.__event_loop.run_blocking()
 
-    def __run_non_blocking(self, *awaitables: Awaitable):
-        [self.__event_loop.queue(task) for task in awaitables]
+    def __run_non_blocking(self, *tasks: _Task):
+        [self.__event_loop.queue(task) for task in tasks]
         if not self.__is_non_blocking_running:
             self.__event_loop.run_non_blocking()
             self.__is_non_blocking_running = True
```

