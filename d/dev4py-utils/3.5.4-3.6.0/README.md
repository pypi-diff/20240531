# Comparing `tmp/dev4py_utils-3.5.4.tar.gz` & `tmp/dev4py_utils-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dev4py_utils-3.5.4.tar", max compression
+gzip compressed data, was "dev4py_utils-3.6.0.tar", max compression
```

## Comparing `dev4py_utils-3.5.4.tar` & `dev4py_utils-3.6.0.tar`

### file list

```diff
@@ -1,38 +1,37 @@
--rw-r--r--   0        0        0    11357 2023-01-24 11:35:53.713914 dev4py_utils-3.5.4/LICENSE
--rw-r--r--   0        0        0    19600 2023-01-24 11:35:53.713914 dev4py_utils-3.5.4/README.md
--rwxr-xr-x   0        0        0    15675 2023-01-24 11:35:53.725915 dev4py_utils-3.5.4/project.py
--rw-r--r--   0        0        0     6008 2023-01-24 11:35:53.725915 dev4py_utils-3.5.4/pyproject.toml
--rw-r--r--   0        0        0      845 2023-01-24 11:35:53.725915 dev4py_utils-3.5.4/src/main/python/dev4py/utils/__init__.py
--rw-r--r--   0        0        0    14914 2023-01-24 11:35:53.725915 dev4py_utils-3.5.4/src/main/python/dev4py/utils/async_joptional.py
--rw-r--r--   0        0        0     3651 2023-01-24 11:35:53.725915 dev4py_utils-3.5.4/src/main/python/dev4py/utils/awaitables.py
--rw-r--r--   0        0        0     8141 2023-01-24 11:35:53.725915 dev4py_utils-3.5.4/src/main/python/dev4py/utils/collectors.py
--rw-r--r--   0        0        0     5500 2023-01-24 11:35:53.725915 dev4py_utils-3.5.4/src/main/python/dev4py/utils/dicts.py
--rw-r--r--   0        0        0     1404 2023-01-24 11:35:53.725915 dev4py_utils-3.5.4/src/main/python/dev4py/utils/iterables.py
--rw-r--r--   0        0        0    13554 2023-01-24 11:35:53.725915 dev4py_utils-3.5.4/src/main/python/dev4py/utils/joptional.py
--rw-r--r--   0        0        0     1693 2023-01-24 11:35:53.725915 dev4py_utils-3.5.4/src/main/python/dev4py/utils/lists.py
--rw-r--r--   0        0        0     6270 2023-01-24 11:35:53.725915 dev4py_utils-3.5.4/src/main/python/dev4py/utils/objects.py
--rw-r--r--   0        0        0      821 2023-01-24 11:35:53.725915 dev4py_utils-3.5.4/src/main/python/dev4py/utils/pipeline/__init__.py
--rw-r--r--   0        0        0     3039 2023-01-24 11:35:53.725915 dev4py_utils-3.5.4/src/main/python/dev4py/utils/pipeline/simple_pipeline.py
--rw-r--r--   0        0        0     5955 2023-01-24 11:35:53.725915 dev4py_utils-3.5.4/src/main/python/dev4py/utils/pipeline/step_pipeline.py
--rw-r--r--   0        0        0    12673 2023-01-24 11:35:53.725915 dev4py_utils-3.5.4/src/main/python/dev4py/utils/retry.py
--rw-r--r--   0        0        0    39972 2023-01-24 11:35:53.725915 dev4py_utils-3.5.4/src/main/python/dev4py/utils/stream.py
--rw-r--r--   0        0        0     1801 2023-01-24 11:35:53.725915 dev4py_utils-3.5.4/src/main/python/dev4py/utils/tuples.py
--rw-r--r--   0        0        0     3558 2023-01-24 11:35:53.725915 dev4py_utils-3.5.4/src/main/python/dev4py/utils/types.py
--rw-r--r--   0        0        0      626 2023-01-24 11:35:53.725915 dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/__init__.py
--rw-r--r--   0        0        0      626 2023-01-24 11:35:53.725915 dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/pipeline/__init__.py
--rw-r--r--   0        0        0     6150 2023-01-24 11:35:53.725915 dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/pipeline/test_simple_pipeline.py
--rw-r--r--   0        0        0     8302 2023-01-24 11:35:53.725915 dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/pipeline/test_step_pipeline.py
--rw-r--r--   0        0        0    75107 2023-01-24 11:35:53.729915 dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/test_async_joptional.py
--rw-r--r--   0        0        0     9882 2023-01-24 11:35:53.729915 dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/test_awaitables.py
--rw-r--r--   0        0        0    14854 2023-01-24 11:35:53.729915 dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/test_collectors.py
--rw-r--r--   0        0        0    17968 2023-01-24 11:35:53.729915 dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/test_dicts.py
--rw-r--r--   0        0        0     2711 2023-01-24 11:35:53.729915 dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/test_iterables.py
--rw-r--r--   0        0        0    39554 2023-01-24 11:35:53.729915 dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/test_joptional.py
--rw-r--r--   0        0        0     4013 2023-01-24 11:35:53.729915 dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/test_lists.py
--rw-r--r--   0        0        0    24161 2023-01-24 11:35:53.729915 dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/test_objects.py
--rw-r--r--   0        0        0    47843 2023-01-24 11:35:53.729915 dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/test_retry.py
--rw-r--r--   0        0        0    71928 2023-01-24 11:35:53.729915 dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/test_stream.py
--rw-r--r--   0        0        0     3907 2023-01-24 11:35:53.729915 dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/test_tuples.py
--rw-r--r--   0        0        0     9758 2023-01-24 11:35:53.729915 dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/test_types.py
--rw-r--r--   0        0        0    21337 1970-01-01 00:00:00.000000 dev4py_utils-3.5.4/setup.py
--rw-r--r--   0        0        0    20447 1970-01-01 00:00:00.000000 dev4py_utils-3.5.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-31 14:23:24.778183 dev4py_utils-3.6.0/LICENSE
+-rw-r--r--   0        0        0    19600 2024-05-31 14:23:24.778183 dev4py_utils-3.6.0/README.md
+-rwxr-xr-x   0        0        0    15675 2024-05-31 14:23:24.786183 dev4py_utils-3.6.0/project.py
+-rw-r--r--   0        0        0     6010 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0      845 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/main/python/dev4py/utils/__init__.py
+-rw-r--r--   0        0        0    14998 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/main/python/dev4py/utils/async_joptional.py
+-rw-r--r--   0        0        0     3651 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/main/python/dev4py/utils/awaitables.py
+-rw-r--r--   0        0        0    10338 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/main/python/dev4py/utils/collectors.py
+-rw-r--r--   0        0        0     5500 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/main/python/dev4py/utils/dicts.py
+-rw-r--r--   0        0        0     1404 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/main/python/dev4py/utils/iterables.py
+-rw-r--r--   0        0        0    13554 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/main/python/dev4py/utils/joptional.py
+-rw-r--r--   0        0        0     1693 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/main/python/dev4py/utils/lists.py
+-rw-r--r--   0        0        0     6270 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/main/python/dev4py/utils/objects.py
+-rw-r--r--   0        0        0      821 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/main/python/dev4py/utils/pipeline/__init__.py
+-rw-r--r--   0        0        0     3039 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/main/python/dev4py/utils/pipeline/simple_pipeline.py
+-rw-r--r--   0        0        0     5955 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/main/python/dev4py/utils/pipeline/step_pipeline.py
+-rw-r--r--   0        0        0    12673 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/main/python/dev4py/utils/retry.py
+-rw-r--r--   0        0        0    39942 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/main/python/dev4py/utils/stream.py
+-rw-r--r--   0        0        0     1801 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/main/python/dev4py/utils/tuples.py
+-rw-r--r--   0        0        0     3558 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/main/python/dev4py/utils/types.py
+-rw-r--r--   0        0        0      626 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/__init__.py
+-rw-r--r--   0        0        0      626 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/pipeline/__init__.py
+-rw-r--r--   0        0        0     6150 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/pipeline/test_simple_pipeline.py
+-rw-r--r--   0        0        0     8302 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/pipeline/test_step_pipeline.py
+-rw-r--r--   0        0        0    75107 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/test_async_joptional.py
+-rw-r--r--   0        0        0     9882 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/test_awaitables.py
+-rw-r--r--   0        0        0    16561 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/test_collectors.py
+-rw-r--r--   0        0        0    17968 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/test_dicts.py
+-rw-r--r--   0        0        0     2711 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/test_iterables.py
+-rw-r--r--   0        0        0    39554 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/test_joptional.py
+-rw-r--r--   0        0        0     4013 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/test_lists.py
+-rw-r--r--   0        0        0    24161 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/test_objects.py
+-rw-r--r--   0        0        0    47843 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/test_retry.py
+-rw-r--r--   0        0        0    71928 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/test_stream.py
+-rw-r--r--   0        0        0     3907 2024-05-31 14:23:24.790183 dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/test_tuples.py
+-rw-r--r--   0        0        0     9758 2024-05-31 14:23:24.794183 dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/test_types.py
+-rw-r--r--   0        0        0    20498 1970-01-01 00:00:00.000000 dev4py_utils-3.6.0/PKG-INFO
```

### Comparing `dev4py_utils-3.5.4/LICENSE` & `dev4py_utils-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/README.md` & `dev4py_utils-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/project.py` & `dev4py_utils-3.6.0/project.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/pyproject.toml` & `dev4py_utils-3.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ##################
 ##### POETRY #####
 ##################
 [tool.poetry]
 name = 'dev4py-utils'
-version = '3.5.4'
+version = '3.6.0'
 description = 'A set of Python regularly used classes/functions'
 authors = ['St4rG00se <st4rg00se@protonmail.com>']
 license = 'Apache-2.0'
 readme = 'README.md'
 homepage = 'https://github.com/dev4py/dev4py-utils'
 repository = 'https://github.com/dev4py/dev4py-utils'
 documentation = 'https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils.html'
@@ -26,19 +26,19 @@
     { include = 'project.py', format = 'sdist' }
 ]
 
 [tool.poetry.dependencies]
 python = '^3.10'
 
 [tool.poetry.dev-dependencies]
-tomli = '2.0.1'  # for project.py if pytest is removed
-tox = "^3.24.5"
-pytest = "^7.0.1"
-pytest-asyncio = "^0.19"
-pdoc = "^12.0.0"
+tomli = '^2'  # for project.py if pytest is removed
+tox = "^3"
+pytest = "^7"
+pytest-asyncio = "^0"
+pdoc = "^12"
 
 
 [tool.pytest.ini_options]
 addopts = "-rA"
 testpaths = ['src/test/python']
 asyncio_mode = "auto"
 
@@ -174,15 +174,16 @@
 
 [tool.pylint.messages_control]
 disable = [
     'invalid-name',
     'too-few-public-methods',
     'missing-class-docstring',
     'missing-function-docstring',
-    'missing-module-docstring'
+    'missing-module-docstring',
+    'cyclic-import'
 ]
 
 [tool.pylint.format]
 max-line-length = 120
 indent-string = "    "
 
 [tool.pylint.reports]
```

### Comparing `dev4py_utils-3.5.4/src/main/python/dev4py/utils/__init__.py` & `dev4py_utils-3.6.0/src/main/python/dev4py/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/main/python/dev4py/utils/async_joptional.py` & `dev4py_utils-3.6.0/src/main/python/dev4py/utils/async_joptional.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     """A JOptional class for async value mapping"""
 
     __CREATE_KEY: Final[object] = object()
     __NO_VALUE_ERROR_MSG: Final[str] = "No value present"
     __EMPTY: AsyncJOptional[Any]
 
     @classmethod
+    # pylint: disable=E1136
     def of(cls, value: _VType[T]) -> AsyncJOptional[T]:
         """
         Returns a JOptional describing the given non-None value or Awaitable value
 
         Args:
             value: The value (or Awaitable value) to describe, which must be non-None and not an Awaitable of None
 
@@ -47,14 +48,15 @@
 
         Raises:
             TypeError: Raises a TypeError on terminal operation if value is None or is an Awaitable of None
         """
         return AsyncJOptional(async_require_non_none(value, cls.__NO_VALUE_ERROR_MSG), cls.__CREATE_KEY)
 
     @classmethod
+    # pylint: disable=E1136
     def of_noneable(cls, value: _VType[T]) -> AsyncJOptional[T]:
         """
         Returns a JOptional describing the given value or Awaitable value, if non-None, otherwise returns an empty
         AsyncJOptional
 
         Args:
             value: The possibly-None or Awaitable of None value to describe
@@ -66,14 +68,15 @@
         return AsyncJOptional(value, cls.__CREATE_KEY)
 
     @classmethod
     def empty(cls) -> AsyncJOptional[T]:
         """Return an empty instance of AsyncJOptional"""
         return cls.__EMPTY
 
+    # pylint: disable=E1136
     def __init__(self, value: _VType[T], create_key: object):
         """AsyncJOptional private constructor: Constructs an instance with the described value"""
         assert create_key == self.__CREATE_KEY, \
             "AsyncJOptional private constructor! Please use AsyncJOptional.of or AsyncJOptional.of_noneable"
         self._value: _VType[T] = value
 
     async def _get_value(self) -> Optional[T]:
```

### Comparing `dev4py_utils-3.5.4/src/main/python/dev4py/utils/awaitables.py` & `dev4py_utils-3.6.0/src/main/python/dev4py/utils/awaitables.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/main/python/dev4py/utils/dicts.py` & `dev4py_utils-3.6.0/src/main/python/dev4py/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/main/python/dev4py/utils/iterables.py` & `dev4py_utils-3.6.0/src/main/python/dev4py/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/main/python/dev4py/utils/joptional.py` & `dev4py_utils-3.6.0/src/main/python/dev4py/utils/joptional.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/main/python/dev4py/utils/lists.py` & `dev4py_utils-3.6.0/src/main/python/dev4py/utils/lists.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/main/python/dev4py/utils/objects.py` & `dev4py_utils-3.6.0/src/main/python/dev4py/utils/objects.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/main/python/dev4py/utils/pipeline/__init__.py` & `dev4py_utils-3.6.0/src/main/python/dev4py/utils/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/main/python/dev4py/utils/pipeline/simple_pipeline.py` & `dev4py_utils-3.6.0/src/main/python/dev4py/utils/pipeline/simple_pipeline.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/main/python/dev4py/utils/pipeline/step_pipeline.py` & `dev4py_utils-3.6.0/src/main/python/dev4py/utils/pipeline/step_pipeline.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/main/python/dev4py/utils/retry.py` & `dev4py_utils-3.6.0/src/main/python/dev4py/utils/retry.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/main/python/dev4py/utils/stream.py` & `dev4py_utils-3.6.0/src/main/python/dev4py/utils/stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 
 from concurrent.futures import Executor, wait, FIRST_COMPLETED, Future, as_completed
 from dataclasses import dataclass
 from functools import partial, cmp_to_key
 from typing import Generic, Final, Optional, cast, Any, Collection, Iterable, Iterator
 
 from dev4py.utils import collectors
-from dev4py.utils.joptional import JOptional
 from dev4py.utils.collectors import Collector
 from dev4py.utils.iterables import get_chunks
+from dev4py.utils.joptional import JOptional
 from dev4py.utils.objects import require_non_none, require_non_none_else_get, to_self
 from dev4py.utils.pipeline import StepPipeline, StepResult
 from dev4py.utils.types import T, Function, R, V, Predicate, Supplier, BiConsumer, K, Consumer, BiFunction
 
 
 ##############################
 #  PRIVATE MODULE FUNCTIONS  #
@@ -260,16 +260,15 @@
         partial(_process_values, pipeline=pipeline, stop_on_first_completed=False, collector=collectors.to_list())
     futures: Final[list[Future[tuple[list[T], bool]]]] = \
         [executor.submit(process_values, chunk) for chunk in get_chunks(values, chunksize)]
     try:
         futures_iterable: Final[Iterable[Future[tuple[list[T], bool]]]] = \
             (futures if ordered_execution else as_completed(futures))
         for future in futures_iterable:
-            for value in future.result()[0]:
-                yield value
+            yield from future.result()[0]
 
     except BaseException as e:
         for future in futures:
             future.cancel()
         raise e
 
 
@@ -947,22 +946,23 @@
             ordered_execution: bool,
             mapper: Function[T, Stream[R]]
     ) -> Iterable[R]:
         """
         private method used by `flat_map` public method in replacement of lambda
         Note: lambda are not used in order to be compatible with multiprocessing (lambda are not serializable)
         """
-        list_generator: Final[Iterable[list[R]]] = self \
-            ._init_to_values_function(parallel_config, ordered_execution) \
-            .map(mapper) \
-            .map(_stream_to_list_lambda) \
+        list_generator: Final[Iterable[list[R]]] = (
+            self
+            ._init_to_values_function(parallel_config, ordered_execution)
+            .map(mapper)
+            .map(_stream_to_list_lambda)  # type: ignore
             .to_generator()
+        )
         for values in list_generator:
-            for value in values:
-                yield value
+            yield from values
 
     def _distinct_values_function(
             self, parallel_config: Optional[ParallelConfiguration], ordered_execution: bool
     ) -> Iterable[T]:
         """
         private method used by `distinct` public method in replacement of lambda
         Note: lambda are not used in order to be compatible with multiprocessing (lambda are not serializable)
```

### Comparing `dev4py_utils-3.5.4/src/main/python/dev4py/utils/tuples.py` & `dev4py_utils-3.6.0/src/main/python/dev4py/utils/tuples.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/main/python/dev4py/utils/types.py` & `dev4py_utils-3.6.0/src/main/python/dev4py/utils/types.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/__init__.py` & `dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/__init__.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/pipeline/__init__.py` & `dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/pipeline/test_simple_pipeline.py` & `dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/pipeline/test_simple_pipeline.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/pipeline/test_step_pipeline.py` & `dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/pipeline/test_step_pipeline.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/test_async_joptional.py` & `dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/test_async_joptional.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/test_awaitables.py` & `dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/test_awaitables.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/test_collectors.py` & `dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/test_collectors.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from dataclasses import FrozenInstanceError, dataclass
-from typing import Final
+from typing import Final, List
 
 from pytest import raises
 
-from dev4py.utils import Collector, collectors
+from dev4py.utils import collectors, Collector
 from dev4py.utils.objects import non_none, to_self
 from dev4py.utils.types import Supplier, BiFunction, BiConsumer, Function
 
 
 class TestCollector:
     """Collector class tests"""
 
@@ -339,7 +339,48 @@
             # GIVEN / WHEN
             collector: Collector[int, int] = collectors.to_counter()
 
             # THEN
             assert collector.supplier() == 0
             assert collector.accumulator(1, 10) == 2
             assert collector.combiner(3, 7) == 10
+
+
+class TestGroupingBy:
+    """grouping_by function tests"""
+
+    class TestNominalCase:
+        def test_existing_mappers__should__return_grouping_by_collector(self) -> None:
+            """When key mapper is provided, should return a dict collector"""
+            # GIVEN
+            key_mapper = lambda x: x % 2
+            value_mapper = lambda x: x * 2
+
+            # WHEN
+            collector: Collector[int, dict[int, List[int]]] = collectors.grouping_by(key_mapper, value_mapper)
+
+            # THEN
+            assert collector.supplier() == {}
+            assert collector.accumulator({1: [3]}, 4) == {0: [8], 1: [3]}
+            assert collector.accumulator({0: [2], 1: [3]}, 4) == {0: [2, 8], 1: [3]}
+            assert collector.accumulator({0: [2], 1: [3]}, 5) == {0: [2], 1: [3, 10]}
+            assert collector.combiner({0: [2, 8]}, {1: [3, 10]}) == {0: [2, 8], 1: [3, 10]}
+            assert collector.combiner({0: [2, 8]}, {0: [4, 6] , 1: [3, 10]}) == {0: [2, 8, 4, 6], 1: [3, 10]}
+
+    class TestErrorCase:
+        def test_none_key_mapper__should__raise_type_error(self) -> None:
+            """When key mapper is None should raise a TypeError exception"""
+            # GIVEN
+            value_mapper = lambda x: x * 2
+
+            # WHEN / THEN
+            with raises(TypeError):
+                collectors.grouping_by(None, value_mapper)
+
+        def test_none_value_mapper__should__raise_type_error(self) -> None:
+            """When value mapper is None should raise a TypeError exception"""
+            # GIVEN
+            key_mapper = lambda x: x % 2
+
+            # WHEN / THEN
+            with raises(TypeError):
+                collectors.grouping_by(key_mapper, None)
```

### Comparing `dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/test_dicts.py` & `dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/test_dicts.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/test_iterables.py` & `dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/test_iterables.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/test_joptional.py` & `dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/test_joptional.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/test_lists.py` & `dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/test_lists.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/test_objects.py` & `dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/test_objects.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/test_retry.py` & `dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/test_retry.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/test_stream.py` & `dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/test_stream.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/test_tuples.py` & `dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/test_tuples.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/src/test/python/dev4py/utils_test/test_types.py` & `dev4py_utils-3.6.0/src/test/python/dev4py/utils_test/test_types.py`

 * *Files identical despite different names*

### Comparing `dev4py_utils-3.5.4/setup.py` & `dev4py_utils-3.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,565 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dev4py-utils
+Version: 3.6.0
+Summary: A set of Python regularly used classes/functions
+Home-page: https://github.com/dev4py/dev4py-utils
+License: Apache-2.0
+Keywords: python,utils,function,classes
+Author: St4rG00se
+Author-email: st4rg00se@protonmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Project-URL: Documentation, https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils.html
+Project-URL: Repository, https://github.com/dev4py/dev4py-utils
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src/main/python',
- 'python': 'src/test/python/python',
- 'python.dev4py.utils_test': 'src/test/python/python/dev4py/utils_test',
- 'python.dev4py.utils_test.pipeline': 'src/test/python/python/dev4py/utils_test/pipeline'}
-
-packages = \
-['python',
- 'python.dev4py.utils',
- 'python.dev4py.utils.pipeline',
- 'python.dev4py.utils_test',
- 'python.dev4py.utils_test.pipeline']
-
-package_data = \
-{'': ['*']}
-
-modules = \
-['project']
-setup_kwargs = {
-    'name': 'dev4py-utils',
-    'version': '3.5.4',
-    'description': 'A set of Python regularly used classes/functions',
-    'long_description': '# Dev4py-utils\n\nA set of Python regularly used classes/functions\n\n[![ci](https://github.com/dev4py/dev4py-utils/actions/workflows/ci.yml/badge.svg?event=push&branch=main)](https://github.com/dev4py/dev4py-utils/actions/workflows/ci.yml) \\\n[![Last release](https://github.com/dev4py/dev4py-utils/actions/workflows/on_release.yml/badge.svg)](https://github.com/dev4py/dev4py-utils/actions/workflows/on_release.yml) \\\n[![Weekly checks](https://github.com/dev4py/dev4py-utils/actions/workflows/weekly_checks.yml/badge.svg?branch=main)](https://github.com/dev4py/dev4py-utils/actions/workflows/weekly_checks.yml) \\\n[![Python >= 3.10.1](https://img.shields.io/badge/Python->=3.10.1-informational.svg?style=plastic&logo=python&logoColor=yellow)](https://www.python.org/) \\\n[![Maintainer](https://img.shields.io/badge/maintainer-St4rG00se-informational?style=plastic&logo=superuser)](https://github.com/St4rG00se) \\\n![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg?style=plastic&logo=github) \\\n[![License: Apache-2.0](https://img.shields.io/badge/License-Apache_2.0-yellow.svg?style=plastic&logo=github)](https://opensource.org/licenses/Apache-2.0)\n\n## Table of contents\n\n- [Quickstart](#quickstart)\n- [Project template](#project-template)\n- [Project links](#project-links)\n- [Dev4py-utils modules](#dev4py-utils-modules)\n  - [dev4py.utils.AsyncJOptional](#dev4pyutilsasyncjoptional)\n  - [dev4py.utils.awaitables](#dev4pyutilsawaitables)\n  - [dev4py.utils.collectors](#dev4pyutilscollectors)\n  - [dev4py.utils.dicts](#dev4pyutilsdicts)\n  - [dev4py.utils.iterables](#dev4pyutilsiterables)\n  - [dev4py.utils.JOptional](#dev4pyutilsjoptional)\n  - [dev4py.utils.lists](#dev4pyutilslists)\n  - [dev4py.utils.objects](#dev4pyutilsobjects)\n  - [dev4py.utils.pipeline](#dev4pyutilspipeline)\n  - [dev4py.utils.retry](#dev4pyutilsretry)\n  - [dev4py.utils.Stream](#dev4pyutilsstream)\n  - [dev4py.utils.tuples](#dev4pyutilstuples)\n  - [dev4py.utils.types](#dev4pyutilstypes)\n\n## Quickstart\n\n```shell\npip install dev4py-utils\n```\n\n## Project template\n\nThis project is based on [pymsdl_template](https://github.com/dev4py/pymsdl_template)\n\n## Project links\n\n- [Documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils.html)\n- [PyPi project](https://pypi.org/project/dev4py-utils/)\n\n## Dev4py-utils modules\n\n### dev4py.utils.AsyncJOptional\n\n[AsyncJOptional documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/async_joptional.html)\n\n> ***Note:** [AsyncJOptional](src/main/python/dev4py/utils/async_joptional.py) class is designed in order to simplify\n> JOptional with async mapper.*\n\n> ***Note:** AsyncJOptional support T or Awaitable[T] values. That\'s why some checks are done when terminal operation is\n> called with `await`.*\n\nExamples:\n\n```python\nimport asyncio\nfrom dev4py.utils import AsyncJOptional\n\ndef sync_mapper(i: int) -> int:\n  return i * 2\n\nasync def async_mapper(i: int) -> str:\n  return f"The value is {i}"\n\nasync def async_sample() -> None:\n  value: int = 1\n  await AsyncJOptional.of_noneable(value) \\\n    .map(sync_mapper) \\\n    .map(async_mapper) \\\n    .if_present(print)  # The value is 2\n\nasyncio.run(async_sample())\n```\n\n### dev4py.utils.awaitables\n\n[Awaitables documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/awaitables.html)\n\n> ***Note:** [awaitables](src/main/python/dev4py/utils/awaitables.py) module provides a set of utility functions to\n> simplify Awaitable operations.*\n\nExamples:\n\n```python\nimport asyncio\nfrom dev4py.utils import awaitables, JOptional\n\n# is_awaitable sample\nawaitables.is_awaitable(asyncio.sleep(2))  # True\nawaitables.is_awaitable(print(\'Hello\'))  # False\n\n\n# to_sync_or_async_param_function sample\ndef mapper(s: str) -> str:\n    return s + \'_suffix\'\n\nasync def async_mapper(s: str) -> str:\n    await asyncio.sleep(1)\n    return s + \'_async_suffix\'\n\nasync def async_test():\n    # Note: mapper parameter is str and async_mapper returns an Awaitable[str] so we have to manage it\n    # Note: !WARNING! Since 3.0.0 see AsyncJOptional / JOptional to_async_joptional method\n    result: str = await JOptional.of("A value") \\\n      .map(async_mapper) \\\n      .map(awaitables.to_sync_or_async_param_function(mapper)) \\\n      .get()\n    print(result)  # A value_async_suffix_suffix\n\nasyncio.run(async_test())\n````\n\n### dev4py.utils.collectors\n\n[Collectors documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/collectors.html)\n\n> ***Note:** The [collectors](src/main/python/dev4py/utils/collectors.py) class is inspired by\n> [java.util.stream.Collectors](https://docs.oracle.com/en/java/javase/17/docs/api//java.base/java/util/stream/Collectors.html)*\n\nExamples:\n\n```python\nfrom dev4py.utils import Stream, collectors\n\nStream.of(\'a\', \'b\', \'c\').collect(collectors.to_list())  # [\'a\', \'b\', \'c\']\n```\n\n### dev4py.utils.dicts\n\n[Dicts documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/dicts.html)\n\n> ***Note:** [dicts](src/main/python/dev4py/utils/dicts.py) module provides a set of utility functions to\n> simplify dict operations.*\n\nExamples:\n\n```python\nfrom dev4py.utils import dicts\nfrom dev4py.utils.types import Supplier\n\n# is_dict sample\ndicts.is_dict("A str")  # False\ndicts.is_dict({\'key\': \'A dict value\'})  # True\n\n\n# get_value sample\nint_supplier: Supplier[int] = lambda: 3\ndictionary: dict[str, int] = {\'key_1\': 1, \'key_2\': 2}\n\ndicts.get_value(dictionary, \'key_1\')  # 1\ndicts.get_value(dictionary, \'key_3\')  # None\ndicts.get_value(dictionary, \'key_3\', int_supplier)  # 3\n\n\n# get_value_from_path sample\nstr_supplier: Supplier[str] = lambda: "a3"\ndeep_dictionary: dict[str, dict[int, str]] = { \\\n  \'a\': {1: \'a1\', 2: \'a2\'}, \\\n  \'b\': {1: \'b1\', 2: \'b2\'} \\\n}\n\ndicts.get_value_from_path(deep_dictionary, ["a", 1])  # \'a1\'\ndicts.get_value_from_path(deep_dictionary, ["c", 1])  # None\ndicts.get_value_from_path(deep_dictionary, ["a", 3])  # None\ndicts.get_value_from_path(deep_dictionary, ["a", 3], str_supplier)  # \'a3\'\n````\n\n### dev4py.utils.iterables\n\n[Iterables documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/iterables.html)\n\n> ***Note:** The [iterables](src/main/python/dev4py/utils/iterables.py) module provides a set of utility functions to simplify\n> iterables operations.*\n\nExample:\n\n```python\nfrom typing import Iterator\n\nfrom dev4py.utils import iterables\n\nvalues: range = range(0, 10)\nchunks: Iterator[list[int]] = iterables.get_chunks(values, 3)\n[chunk for chunk in chunks]  # [[0, 1, 2], [3, 4, 5], [6, 7, 8], [9]]\n```\n\n### dev4py.utils.JOptional\n\n[JOptional documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/joptional.html)\n\n> ***Note:** [JOptional](src/main/python/dev4py/utils/joptional.py) class is inspired by\n> [java.util.Optional](https://docs.oracle.com/en/java/javase/17/docs/api//java.base/java/util/Optional.html)\n> class with some adds (like `peek` method).*\n\nExamples:\n\n```python\nfrom dev4py.utils import JOptional\n\nvalue: int = 1\nJOptional.of_noneable(value) \\\n  .map(lambda v: f"The value is {v}") \\\n  .if_present(print)  # The value is 1\n```\n\n### dev4py.utils.lists\n\n[Lists documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/lists.html)\n\n> ***Note:** [lists](src/main/python/dev4py/utils/lists.py) module provides a set of utility functions to simplify lists\n> operations.*\n\nExamples:\n\n```python\nfrom dev4py.utils import lists\n\n# empty sample\nlst: list[int] = lists.empty_list()  # []\n\n# append sample\nlst: list[int] = [1, 2, 3, 4]\napp_lst: list[int] = lists.append(lst, 5)  # [1, 2, 3, 4, 5]\n# - Note: lst == app_lst\n\n# extend sample\nlst: list[int] = [1, 2, 3, 4]\nlst2: list[int] = [5, 6, 7, 8]\next_lst: list[int] = lists.extend(lst, lst2)  # [1, 2, 3, 4, 5, 6, 7, 8]\n# - Note: lst == ext_lst\n```\n\n### dev4py.utils.objects\n\n[Objects documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/objects.html)\n\n> ***Note:** The [objects](src/main/python/dev4py/utils/objects.py) module is inspired by\n> [java.util.Objects](https://docs.oracle.com/en/java/javase/17/docs/api//java.base/java/util/Objects.html)\n> class.*\n\nExamples:\n\n```python\nfrom dev4py.utils import objects\n\n# non_none sample\nvalue = None\nobjects.non_none(value)  # False\n\n# require_non_none sample\nvalue = "A value"\nobjects.require_non_none(value)  # \'A value\'\n\n# to_string sample\nvalue = None\ndefault_value: str = "A default value"\nobjects.to_string(value, default_value)  # \'A default value\'\n```\n\n### dev4py.utils.pipeline\n\n[Pipeline documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/pipeline.html)\n\n> ***Note:** The [pipeline](src/main/python/dev4py/utils/pipeline) package provides a set of Pipeline class describing\n> different kind of pipelines.*\n\nExamples:\n\n```python\nfrom dev4py.utils.pipeline import SimplePipeline, StepPipeline, StepResult\n\n# SimplePipeline sample\npipeline: SimplePipeline[int, str] = SimplePipeline.of(lambda i: i * i) \\\n    .add_handler(str) \\\n    .add_handler(lambda s: f"Result: {s} | Type: {type(s)}")\n\npipeline.execute(10)  # "Result: 100 | Type: <class \'str\'>"\n\n\n# StepPipeline sample\n# Note: StepPipeline can be stopped at each step by setting `go_next` value to False\npipeline: StepPipeline[int, str] = StepPipeline.of(lambda i: StepResult(i * i)) \\\n    .add_handler(lambda i: StepResult(value=str(i), go_next=i < 150)) \\\n    .add_handler(lambda s: StepResult(f"Result: {s} | Type: {type(s)}"))\n\npipeline.execute(10)  # StepResult(value="Result: 100 | Type: <class \'str\'>", go_next=True)\n# - Note: When the pipeline is fully completed, `go_next` is True\npipeline.execute(15)  # StepResult(value=\'225\', go_next=False)\n# - Note: Even if the pipeline is not fully completed, the last StepResult is returned with `go_next=False`\n```\n\n### dev4py.utils.retry\n\n[Retry documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/retry.html)\n\n> ***Note:** The [retry](src/main/python/dev4py/utils/retry.py) module provides provides function to create retryable\n> callable from simple sync or async callables using exponential backoff*\n>\n> *Usage idea: network requests (HTTP, AMQP, MQTT, etc.) with retry on error*\n\nExamples:\n\n```python\nimport asyncio\nfrom time import time\nfrom typing import Awaitable\n\nfrom dev4py.utils.retry import RetryConfiguration, to_retryable, to_async_retryable, retryable, async_retryable\nfrom dev4py.utils.types import BiFunction\n\n# RetryConfiguration:\n# Note: exponential backoff used formula is \'delay * (exponent^retry_number)\'\n#\n#   => Example: For the following RetryConfiguration, waiting times in case of error are:\n#       * first try:                    0 sec (always 0 for the first try)\n#       * second try (/first retry):    1 sec (\'0.5 * (2^1)\')\n#       * third try (/second retry):    2 sec (\'0.5 * (2^2)\')\n#       * max_tries=3 => no fourth try (/third retry)\nretry_config: RetryConfiguration = RetryConfiguration(\n    delay=0.5,  # the exponential backoff delay in second (default: 0.1)\n    exponent=2,  # the exponential backoff exponent to determine delay between each try (default: 2)\n    max_tries=3  # max try number (first try included) (default: 3, i.e.: first try and 2 retry)\n)\n\n\n# to_retryable sample:\n# -> SUCCESSFUL CALL SAMPLE\ndef callable_sample(j: int, start_time: float) -> int:\n    print("callable_sample - call time: \'%.2f\'" % (time() - start_time))\n    return j ** 2\n\nretryable_sample: BiFunction[int, float, int] = to_retryable(sync_callable=callable_sample, retry_config=retry_config)\n# Note: Since 3.5.0 you can also use `retryable(sync_callable=callable_sample, retry_config=retry_config)`\n\nresult: int = retryable_sample(3, time())  # result = 9\n# outputs:\n#  callable_sample - call time: \'0.00\'\n\n\n# -> IN ERROR CALL SAMPLE\ndef in_error_callable_sample(j: int, start_time: float) -> int:\n    print("in_error_callable_sample - call time: \'%.2f\'" % (time() - start_time))\n    raise ValueError(j)\n\nin_error_retryable_sample: BiFunction[int, float, int] = \\\n    to_retryable(sync_callable=in_error_callable_sample, retry_config=retry_config)\n# Note: Since 3.5.0 you can also use `retryable(sync_callable=in_error_callable_sample, retry_config=retry_config)`\n# Note: By default the last raised exception is raised if max_tries is reach. You can change this behavior by setting\n#       the `on_failure` parameter\nresult: int = in_error_retryable_sample(3, time())\n# outputs:\n#  in_error_callable_sample - call time: \'0.00\'\n#  in_error_callable_sample - call time: \'1.00\'\n#  in_error_callable_sample - call time: \'3.00\'\n#  ValueError: 3\n#\n# Note: By default the last raised exception is raised if max_tries is reached. You can change this behavior by setting\n#       the `on_failure` parameter\n\n# -> DECORATOR SAMPLE\n@retryable(retry_config=retry_config)\ndef decorated_in_error_callable_sample(j: int, start_time: float) -> int:\n    print("decorated_in_error_callable_sample - call time: \'%.2f\'" % (time() - start_time))\n    raise ValueError(j)\n\nresult: int = decorated_in_error_callable_sample(3, time())\n# outputs:\n#  decorated_in_error_callable_sample - call time: \'0.00\'\n#  decorated_in_error_callable_sample - call time: \'1.00\'\n#  decorated_in_error_callable_sample - call time: \'3.00\'\n#  ValueError: 3\n#\n# Note: By default the last raised exception is raised if max_tries is reached. You can change this behavior by setting\n#       the `on_failure` parameter\n\n\n# to_async_retryable sample:\n# -> IN ERROR CALL ASYNC SAMPLE\nasync def in_error_async_callable_sample(j: int, start_time: float) -> int:\n    print("in_error_async_callable_sample - call time: \'%.2f\'" % (time() - start_time))\n    raise ValueError(j)\n\nasync def async_retryable_sample() -> None:\n    in_error_async_retryable_sample: BiFunction[int, float, Awaitable[int]] = \\\n        to_async_retryable(async_callable=in_error_async_callable_sample, retry_config=retry_config)\n    # Note: Since 3.5.0 you can also use \n    # `async_retryable(async_callable=in_error_async_callable_sample, retry_config=retry_config)`\n    result: int = await in_error_async_retryable_sample(2, time())\n\nasyncio.run(async_retryable_sample())\n# outputs:\n#  in_error_async_callable_sample - call time: \'0.00\'\n#  in_error_async_callable_sample - call time: \'1.00\'\n#  in_error_async_callable_sample - call time: \'3.00\'\n#  ValueError: 2\n#\n# Note: By default the last raised exception is raised if max_tries is reached. You can change this behavior by setting\n#       the `on_failure` parameter\n\n# -> DECORATOR ASYNC SAMPLE\n@async_retryable(retry_config=retry_config)\nasync def decorated_in_error_async_callable_sample(j: int, start_time: float) -> int:\n    print("decorated_in_error_async_callable_sample - call time: \'%.2f\'" % (time() - start_time))\n    raise ValueError(j)\n\nasync def async_decorated_retryable_sample() -> None:\n    result: int = await decorated_in_error_async_callable_sample(2, time())\n\nasyncio.run(async_decorated_retryable_sample())\n# outputs:\n#  in_error_async_callable_sample - call time: \'0.00\'\n#  in_error_async_callable_sample - call time: \'1.00\'\n#  in_error_async_callable_sample - call time: \'3.00\'\n#  ValueError: 2\n#\n# Note: By default the last raised exception is raised if max_tries is reached. You can change this behavior by setting\n#       the `on_failure` parameter\n```\n\n### dev4py.utils.Stream\n\n[Stream documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/stream.html)\n\n> ***Note:** [Stream](src/main/python/dev4py/utils/stream.py) class is inspired by\n> [java.util.stream.Stream](https://docs.oracle.com/en/java/javase/17/docs/api//java.base/java/util/stream/Stream.html).*\n\nExamples:\n\n```python\nfrom concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor\nfrom time import sleep\n\nfrom dev4py.utils import Stream, ParallelConfiguration\n\n# Sequential sample\nStream.of(1, 2, 3, 4) \\\n    .map(str) \\\n    .peek(lambda s: sleep(0.5)) \\\n    .map(lambda s: f"Mapped value: {s}") \\\n    .to_list()  # [\'Mapped value: 1\', \'Mapped value: 2\', \'Mapped value: 3\', \'Mapped value: 4\']\n# - Note: Execution time around 2 sec due to the sleep call\n\n\n# Multithreading sample\nwith ThreadPoolExecutor(max_workers=2) as executor:\n    Stream.of(1, 2, 3, 4) \\\n        .parallel(parallel_config=ParallelConfiguration(executor=executor, chunksize=2)) \\\n        .map(str) \\\n        .peek(lambda s: sleep(0.5)) \\\n        .map(lambda s: f"Mapped value: {s}") \\\n        .to_list()  # [\'Mapped value: 3\', \'Mapped value: 4\', \'Mapped value: 1\', \'Mapped value: 2\']\n# - Note: Execution time around 1 sec due to the given ParallelConfiguration\n# - Note: Since this stream is (by default) unordered, results order is random\n\n\n# Multiprocessing sample\n# - Note: Due to use of Multiprocessing:\n#       * lambdas cannot be used since they cannot be pickled\n#       * This sample should be put in a python file in order to work\ndef _sleep(s: str) -> None:\n    # eq lambda s: sleep(0.5)\n    sleep(0.5)\n\ndef _mapper(s: str) -> str:\n    # eq lambda s: f"Mapped value: {s}"\n    return f"Mapped value: {s}"\n\nif __name__ == \'__main__\':\n    with ProcessPoolExecutor(max_workers=2) as executor:\n        Stream.of(1, 2, 3, 4) \\\n            .parallel(parallel_config=ParallelConfiguration(executor=executor, chunksize=2)) \\\n            .map(str) \\\n            .peek(_sleep) \\\n            .map(_mapper) \\\n            .to_list()\n\n# - Note: Execution time around 1 sec due to the given ParallelConfiguration\n#         (Reminder: Use Multiprocessing for CPU-bound tasks. In this case Multithreading is more appropriate)\n# - Note: Since this stream is (by default) unordered, results order is random\n```\n\n### dev4py.utils.tuples\n\n[Tuples documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/tuples.html)\n\n> ***Note:** [tuples](src/main/python/dev4py/utils/tuples.py) module provides a set of utility functions to simplify\n> tuples operations.*\n\nExamples:\n\n```python\nfrom dev4py.utils import tuples\n\n# empty sample\ntpl: tuple[int, ...] = tuples.empty_tuple()  # ()\n\n# append sample\ntpl: tuple[int, ...] = (1, 2, 3, 4)\napp_tpl: tuple[int, ...] = tuples.append(tpl, 5)  # (1, 2, 3, 4, 5)\n\n# extend sample\ntpl: tuple[int, ...] = (1, 2, 3, 4)\ntpl2: tuple[int, ...] = (5, 6, 7, 8)\next_tpl: tuple[int, ...] = tuples.extend(tpl, tpl2)  # (1, 2, 3, 4, 5, 6, 7, 8)\n```\n\n### dev4py.utils.types\n\n[Types documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/types.html)\n\n> ***Note:** The [types](src/main/python/dev4py/utils/types.py) module is inspired by\n> [java.util.function](https://docs.oracle.com/en/java/javase/17/docs/api//java.base/java/util/function/package-summary.html)\n> package.*\n\nExamples:\n\n```python\nfrom dev4py.utils.types import Function, Predicate, Consumer\n\n# Function sample\nint_to_str: Function[int, str] = lambda i: str(i)\nstr_result: str = int_to_str(1)  # \'1\'\n\n# Predicate sample\nstr_predicate: Predicate[str] = lambda s: s == "A value"\npred_result: bool = str_predicate("Value to test")  # False\n\n# Consumer sample\ndef sample(consumer: Consumer[str], value: str) -> None:\n    consumer(value)\n\ndef my_consumer(arg: str) -> None:\n    print(arg)\n\nsample(my_consumer, "My value")  # My value\n```\n',
-    'author': 'St4rG00se',
-    'author_email': 'st4rg00se@protonmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/dev4py/dev4py-utils',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'py_modules': modules,
-    'python_requires': '>=3.10,<4.0',
+# Dev4py-utils
+
+A set of Python regularly used classes/functions
+
+[![ci](https://github.com/dev4py/dev4py-utils/actions/workflows/ci.yml/badge.svg?event=push&branch=main)](https://github.com/dev4py/dev4py-utils/actions/workflows/ci.yml) \
+[![Last release](https://github.com/dev4py/dev4py-utils/actions/workflows/on_release.yml/badge.svg)](https://github.com/dev4py/dev4py-utils/actions/workflows/on_release.yml) \
+[![Weekly checks](https://github.com/dev4py/dev4py-utils/actions/workflows/weekly_checks.yml/badge.svg?branch=main)](https://github.com/dev4py/dev4py-utils/actions/workflows/weekly_checks.yml) \
+[![Python >= 3.10.1](https://img.shields.io/badge/Python->=3.10.1-informational.svg?style=plastic&logo=python&logoColor=yellow)](https://www.python.org/) \
+[![Maintainer](https://img.shields.io/badge/maintainer-St4rG00se-informational?style=plastic&logo=superuser)](https://github.com/St4rG00se) \
+![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg?style=plastic&logo=github) \
+[![License: Apache-2.0](https://img.shields.io/badge/License-Apache_2.0-yellow.svg?style=plastic&logo=github)](https://opensource.org/licenses/Apache-2.0)
+
+## Table of contents
+
+- [Quickstart](#quickstart)
+- [Project template](#project-template)
+- [Project links](#project-links)
+- [Dev4py-utils modules](#dev4py-utils-modules)
+  - [dev4py.utils.AsyncJOptional](#dev4pyutilsasyncjoptional)
+  - [dev4py.utils.awaitables](#dev4pyutilsawaitables)
+  - [dev4py.utils.collectors](#dev4pyutilscollectors)
+  - [dev4py.utils.dicts](#dev4pyutilsdicts)
+  - [dev4py.utils.iterables](#dev4pyutilsiterables)
+  - [dev4py.utils.JOptional](#dev4pyutilsjoptional)
+  - [dev4py.utils.lists](#dev4pyutilslists)
+  - [dev4py.utils.objects](#dev4pyutilsobjects)
+  - [dev4py.utils.pipeline](#dev4pyutilspipeline)
+  - [dev4py.utils.retry](#dev4pyutilsretry)
+  - [dev4py.utils.Stream](#dev4pyutilsstream)
+  - [dev4py.utils.tuples](#dev4pyutilstuples)
+  - [dev4py.utils.types](#dev4pyutilstypes)
+
+## Quickstart
+
+```shell
+pip install dev4py-utils
+```
+
+## Project template
+
+This project is based on [pymsdl_template](https://github.com/dev4py/pymsdl_template)
+
+## Project links
+
+- [Documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils.html)
+- [PyPi project](https://pypi.org/project/dev4py-utils/)
+
+## Dev4py-utils modules
+
+### dev4py.utils.AsyncJOptional
+
+[AsyncJOptional documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/async_joptional.html)
+
+> ***Note:** [AsyncJOptional](src/main/python/dev4py/utils/async_joptional.py) class is designed in order to simplify
+> JOptional with async mapper.*
+
+> ***Note:** AsyncJOptional support T or Awaitable[T] values. That's why some checks are done when terminal operation is
+> called with `await`.*
+
+Examples:
+
+```python
+import asyncio
+from dev4py.utils import AsyncJOptional
+
+def sync_mapper(i: int) -> int:
+  return i * 2
+
+async def async_mapper(i: int) -> str:
+  return f"The value is {i}"
+
+async def async_sample() -> None:
+  value: int = 1
+  await AsyncJOptional.of_noneable(value) \
+    .map(sync_mapper) \
+    .map(async_mapper) \
+    .if_present(print)  # The value is 2
+
+asyncio.run(async_sample())
+```
+
+### dev4py.utils.awaitables
+
+[Awaitables documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/awaitables.html)
+
+> ***Note:** [awaitables](src/main/python/dev4py/utils/awaitables.py) module provides a set of utility functions to
+> simplify Awaitable operations.*
+
+Examples:
+
+```python
+import asyncio
+from dev4py.utils import awaitables, JOptional
+
+# is_awaitable sample
+awaitables.is_awaitable(asyncio.sleep(2))  # True
+awaitables.is_awaitable(print('Hello'))  # False
+
+
+# to_sync_or_async_param_function sample
+def mapper(s: str) -> str:
+    return s + '_suffix'
+
+async def async_mapper(s: str) -> str:
+    await asyncio.sleep(1)
+    return s + '_async_suffix'
+
+async def async_test():
+    # Note: mapper parameter is str and async_mapper returns an Awaitable[str] so we have to manage it
+    # Note: !WARNING! Since 3.0.0 see AsyncJOptional / JOptional to_async_joptional method
+    result: str = await JOptional.of("A value") \
+      .map(async_mapper) \
+      .map(awaitables.to_sync_or_async_param_function(mapper)) \
+      .get()
+    print(result)  # A value_async_suffix_suffix
+
+asyncio.run(async_test())
+````
+
+### dev4py.utils.collectors
+
+[Collectors documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/collectors.html)
+
+> ***Note:** The [collectors](src/main/python/dev4py/utils/collectors.py) class is inspired by
+> [java.util.stream.Collectors](https://docs.oracle.com/en/java/javase/17/docs/api//java.base/java/util/stream/Collectors.html)*
+
+Examples:
+
+```python
+from dev4py.utils import Stream, collectors
+
+Stream.of('a', 'b', 'c').collect(collectors.to_list())  # ['a', 'b', 'c']
+```
+
+### dev4py.utils.dicts
+
+[Dicts documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/dicts.html)
+
+> ***Note:** [dicts](src/main/python/dev4py/utils/dicts.py) module provides a set of utility functions to
+> simplify dict operations.*
+
+Examples:
+
+```python
+from dev4py.utils import dicts
+from dev4py.utils.types import Supplier
+
+# is_dict sample
+dicts.is_dict("A str")  # False
+dicts.is_dict({'key': 'A dict value'})  # True
+
+
+# get_value sample
+int_supplier: Supplier[int] = lambda: 3
+dictionary: dict[str, int] = {'key_1': 1, 'key_2': 2}
+
+dicts.get_value(dictionary, 'key_1')  # 1
+dicts.get_value(dictionary, 'key_3')  # None
+dicts.get_value(dictionary, 'key_3', int_supplier)  # 3
+
+
+# get_value_from_path sample
+str_supplier: Supplier[str] = lambda: "a3"
+deep_dictionary: dict[str, dict[int, str]] = { \
+  'a': {1: 'a1', 2: 'a2'}, \
+  'b': {1: 'b1', 2: 'b2'} \
 }
 
+dicts.get_value_from_path(deep_dictionary, ["a", 1])  # 'a1'
+dicts.get_value_from_path(deep_dictionary, ["c", 1])  # None
+dicts.get_value_from_path(deep_dictionary, ["a", 3])  # None
+dicts.get_value_from_path(deep_dictionary, ["a", 3], str_supplier)  # 'a3'
+````
+
+### dev4py.utils.iterables
+
+[Iterables documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/iterables.html)
+
+> ***Note:** The [iterables](src/main/python/dev4py/utils/iterables.py) module provides a set of utility functions to simplify
+> iterables operations.*
+
+Example:
+
+```python
+from typing import Iterator
+
+from dev4py.utils import iterables
+
+values: range = range(0, 10)
+chunks: Iterator[list[int]] = iterables.get_chunks(values, 3)
+[chunk for chunk in chunks]  # [[0, 1, 2], [3, 4, 5], [6, 7, 8], [9]]
+```
+
+### dev4py.utils.JOptional
+
+[JOptional documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/joptional.html)
+
+> ***Note:** [JOptional](src/main/python/dev4py/utils/joptional.py) class is inspired by
+> [java.util.Optional](https://docs.oracle.com/en/java/javase/17/docs/api//java.base/java/util/Optional.html)
+> class with some adds (like `peek` method).*
+
+Examples:
+
+```python
+from dev4py.utils import JOptional
+
+value: int = 1
+JOptional.of_noneable(value) \
+  .map(lambda v: f"The value is {v}") \
+  .if_present(print)  # The value is 1
+```
+
+### dev4py.utils.lists
+
+[Lists documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/lists.html)
+
+> ***Note:** [lists](src/main/python/dev4py/utils/lists.py) module provides a set of utility functions to simplify lists
+> operations.*
+
+Examples:
+
+```python
+from dev4py.utils import lists
+
+# empty sample
+lst: list[int] = lists.empty_list()  # []
+
+# append sample
+lst: list[int] = [1, 2, 3, 4]
+app_lst: list[int] = lists.append(lst, 5)  # [1, 2, 3, 4, 5]
+# - Note: lst == app_lst
+
+# extend sample
+lst: list[int] = [1, 2, 3, 4]
+lst2: list[int] = [5, 6, 7, 8]
+ext_lst: list[int] = lists.extend(lst, lst2)  # [1, 2, 3, 4, 5, 6, 7, 8]
+# - Note: lst == ext_lst
+```
+
+### dev4py.utils.objects
+
+[Objects documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/objects.html)
+
+> ***Note:** The [objects](src/main/python/dev4py/utils/objects.py) module is inspired by
+> [java.util.Objects](https://docs.oracle.com/en/java/javase/17/docs/api//java.base/java/util/Objects.html)
+> class.*
+
+Examples:
+
+```python
+from dev4py.utils import objects
+
+# non_none sample
+value = None
+objects.non_none(value)  # False
+
+# require_non_none sample
+value = "A value"
+objects.require_non_none(value)  # 'A value'
+
+# to_string sample
+value = None
+default_value: str = "A default value"
+objects.to_string(value, default_value)  # 'A default value'
+```
+
+### dev4py.utils.pipeline
+
+[Pipeline documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/pipeline.html)
+
+> ***Note:** The [pipeline](src/main/python/dev4py/utils/pipeline) package provides a set of Pipeline class describing
+> different kind of pipelines.*
+
+Examples:
+
+```python
+from dev4py.utils.pipeline import SimplePipeline, StepPipeline, StepResult
+
+# SimplePipeline sample
+pipeline: SimplePipeline[int, str] = SimplePipeline.of(lambda i: i * i) \
+    .add_handler(str) \
+    .add_handler(lambda s: f"Result: {s} | Type: {type(s)}")
+
+pipeline.execute(10)  # "Result: 100 | Type: <class 'str'>"
+
+
+# StepPipeline sample
+# Note: StepPipeline can be stopped at each step by setting `go_next` value to False
+pipeline: StepPipeline[int, str] = StepPipeline.of(lambda i: StepResult(i * i)) \
+    .add_handler(lambda i: StepResult(value=str(i), go_next=i < 150)) \
+    .add_handler(lambda s: StepResult(f"Result: {s} | Type: {type(s)}"))
+
+pipeline.execute(10)  # StepResult(value="Result: 100 | Type: <class 'str'>", go_next=True)
+# - Note: When the pipeline is fully completed, `go_next` is True
+pipeline.execute(15)  # StepResult(value='225', go_next=False)
+# - Note: Even if the pipeline is not fully completed, the last StepResult is returned with `go_next=False`
+```
+
+### dev4py.utils.retry
+
+[Retry documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/retry.html)
+
+> ***Note:** The [retry](src/main/python/dev4py/utils/retry.py) module provides provides function to create retryable
+> callable from simple sync or async callables using exponential backoff*
+>
+> *Usage idea: network requests (HTTP, AMQP, MQTT, etc.) with retry on error*
+
+Examples:
+
+```python
+import asyncio
+from time import time
+from typing import Awaitable
+
+from dev4py.utils.retry import RetryConfiguration, to_retryable, to_async_retryable, retryable, async_retryable
+from dev4py.utils.types import BiFunction
+
+# RetryConfiguration:
+# Note: exponential backoff used formula is 'delay * (exponent^retry_number)'
+#
+#   => Example: For the following RetryConfiguration, waiting times in case of error are:
+#       * first try:                    0 sec (always 0 for the first try)
+#       * second try (/first retry):    1 sec ('0.5 * (2^1)')
+#       * third try (/second retry):    2 sec ('0.5 * (2^2)')
+#       * max_tries=3 => no fourth try (/third retry)
+retry_config: RetryConfiguration = RetryConfiguration(
+    delay=0.5,  # the exponential backoff delay in second (default: 0.1)
+    exponent=2,  # the exponential backoff exponent to determine delay between each try (default: 2)
+    max_tries=3  # max try number (first try included) (default: 3, i.e.: first try and 2 retry)
+)
+
+
+# to_retryable sample:
+# -> SUCCESSFUL CALL SAMPLE
+def callable_sample(j: int, start_time: float) -> int:
+    print("callable_sample - call time: '%.2f'" % (time() - start_time))
+    return j ** 2
+
+retryable_sample: BiFunction[int, float, int] = to_retryable(sync_callable=callable_sample, retry_config=retry_config)
+# Note: Since 3.5.0 you can also use `retryable(sync_callable=callable_sample, retry_config=retry_config)`
+
+result: int = retryable_sample(3, time())  # result = 9
+# outputs:
+#  callable_sample - call time: '0.00'
+
+
+# -> IN ERROR CALL SAMPLE
+def in_error_callable_sample(j: int, start_time: float) -> int:
+    print("in_error_callable_sample - call time: '%.2f'" % (time() - start_time))
+    raise ValueError(j)
+
+in_error_retryable_sample: BiFunction[int, float, int] = \
+    to_retryable(sync_callable=in_error_callable_sample, retry_config=retry_config)
+# Note: Since 3.5.0 you can also use `retryable(sync_callable=in_error_callable_sample, retry_config=retry_config)`
+# Note: By default the last raised exception is raised if max_tries is reach. You can change this behavior by setting
+#       the `on_failure` parameter
+result: int = in_error_retryable_sample(3, time())
+# outputs:
+#  in_error_callable_sample - call time: '0.00'
+#  in_error_callable_sample - call time: '1.00'
+#  in_error_callable_sample - call time: '3.00'
+#  ValueError: 3
+#
+# Note: By default the last raised exception is raised if max_tries is reached. You can change this behavior by setting
+#       the `on_failure` parameter
+
+# -> DECORATOR SAMPLE
+@retryable(retry_config=retry_config)
+def decorated_in_error_callable_sample(j: int, start_time: float) -> int:
+    print("decorated_in_error_callable_sample - call time: '%.2f'" % (time() - start_time))
+    raise ValueError(j)
+
+result: int = decorated_in_error_callable_sample(3, time())
+# outputs:
+#  decorated_in_error_callable_sample - call time: '0.00'
+#  decorated_in_error_callable_sample - call time: '1.00'
+#  decorated_in_error_callable_sample - call time: '3.00'
+#  ValueError: 3
+#
+# Note: By default the last raised exception is raised if max_tries is reached. You can change this behavior by setting
+#       the `on_failure` parameter
+
+
+# to_async_retryable sample:
+# -> IN ERROR CALL ASYNC SAMPLE
+async def in_error_async_callable_sample(j: int, start_time: float) -> int:
+    print("in_error_async_callable_sample - call time: '%.2f'" % (time() - start_time))
+    raise ValueError(j)
+
+async def async_retryable_sample() -> None:
+    in_error_async_retryable_sample: BiFunction[int, float, Awaitable[int]] = \
+        to_async_retryable(async_callable=in_error_async_callable_sample, retry_config=retry_config)
+    # Note: Since 3.5.0 you can also use 
+    # `async_retryable(async_callable=in_error_async_callable_sample, retry_config=retry_config)`
+    result: int = await in_error_async_retryable_sample(2, time())
+
+asyncio.run(async_retryable_sample())
+# outputs:
+#  in_error_async_callable_sample - call time: '0.00'
+#  in_error_async_callable_sample - call time: '1.00'
+#  in_error_async_callable_sample - call time: '3.00'
+#  ValueError: 2
+#
+# Note: By default the last raised exception is raised if max_tries is reached. You can change this behavior by setting
+#       the `on_failure` parameter
+
+# -> DECORATOR ASYNC SAMPLE
+@async_retryable(retry_config=retry_config)
+async def decorated_in_error_async_callable_sample(j: int, start_time: float) -> int:
+    print("decorated_in_error_async_callable_sample - call time: '%.2f'" % (time() - start_time))
+    raise ValueError(j)
+
+async def async_decorated_retryable_sample() -> None:
+    result: int = await decorated_in_error_async_callable_sample(2, time())
+
+asyncio.run(async_decorated_retryable_sample())
+# outputs:
+#  in_error_async_callable_sample - call time: '0.00'
+#  in_error_async_callable_sample - call time: '1.00'
+#  in_error_async_callable_sample - call time: '3.00'
+#  ValueError: 2
+#
+# Note: By default the last raised exception is raised if max_tries is reached. You can change this behavior by setting
+#       the `on_failure` parameter
+```
+
+### dev4py.utils.Stream
+
+[Stream documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/stream.html)
+
+> ***Note:** [Stream](src/main/python/dev4py/utils/stream.py) class is inspired by
+> [java.util.stream.Stream](https://docs.oracle.com/en/java/javase/17/docs/api//java.base/java/util/stream/Stream.html).*
+
+Examples:
+
+```python
+from concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor
+from time import sleep
+
+from dev4py.utils import Stream, ParallelConfiguration
+
+# Sequential sample
+Stream.of(1, 2, 3, 4) \
+    .map(str) \
+    .peek(lambda s: sleep(0.5)) \
+    .map(lambda s: f"Mapped value: {s}") \
+    .to_list()  # ['Mapped value: 1', 'Mapped value: 2', 'Mapped value: 3', 'Mapped value: 4']
+# - Note: Execution time around 2 sec due to the sleep call
+
+
+# Multithreading sample
+with ThreadPoolExecutor(max_workers=2) as executor:
+    Stream.of(1, 2, 3, 4) \
+        .parallel(parallel_config=ParallelConfiguration(executor=executor, chunksize=2)) \
+        .map(str) \
+        .peek(lambda s: sleep(0.5)) \
+        .map(lambda s: f"Mapped value: {s}") \
+        .to_list()  # ['Mapped value: 3', 'Mapped value: 4', 'Mapped value: 1', 'Mapped value: 2']
+# - Note: Execution time around 1 sec due to the given ParallelConfiguration
+# - Note: Since this stream is (by default) unordered, results order is random
+
+
+# Multiprocessing sample
+# - Note: Due to use of Multiprocessing:
+#       * lambdas cannot be used since they cannot be pickled
+#       * This sample should be put in a python file in order to work
+def _sleep(s: str) -> None:
+    # eq lambda s: sleep(0.5)
+    sleep(0.5)
+
+def _mapper(s: str) -> str:
+    # eq lambda s: f"Mapped value: {s}"
+    return f"Mapped value: {s}"
+
+if __name__ == '__main__':
+    with ProcessPoolExecutor(max_workers=2) as executor:
+        Stream.of(1, 2, 3, 4) \
+            .parallel(parallel_config=ParallelConfiguration(executor=executor, chunksize=2)) \
+            .map(str) \
+            .peek(_sleep) \
+            .map(_mapper) \
+            .to_list()
+
+# - Note: Execution time around 1 sec due to the given ParallelConfiguration
+#         (Reminder: Use Multiprocessing for CPU-bound tasks. In this case Multithreading is more appropriate)
+# - Note: Since this stream is (by default) unordered, results order is random
+```
+
+### dev4py.utils.tuples
+
+[Tuples documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/tuples.html)
+
+> ***Note:** [tuples](src/main/python/dev4py/utils/tuples.py) module provides a set of utility functions to simplify
+> tuples operations.*
+
+Examples:
+
+```python
+from dev4py.utils import tuples
+
+# empty sample
+tpl: tuple[int, ...] = tuples.empty_tuple()  # ()
+
+# append sample
+tpl: tuple[int, ...] = (1, 2, 3, 4)
+app_tpl: tuple[int, ...] = tuples.append(tpl, 5)  # (1, 2, 3, 4, 5)
+
+# extend sample
+tpl: tuple[int, ...] = (1, 2, 3, 4)
+tpl2: tuple[int, ...] = (5, 6, 7, 8)
+ext_tpl: tuple[int, ...] = tuples.extend(tpl, tpl2)  # (1, 2, 3, 4, 5, 6, 7, 8)
+```
+
+### dev4py.utils.types
+
+[Types documentation](https://htmlpreview.github.io/?https://github.com/dev4py/dev4py-utils/blob/main/docs/dev4py/utils/types.html)
+
+> ***Note:** The [types](src/main/python/dev4py/utils/types.py) module is inspired by
+> [java.util.function](https://docs.oracle.com/en/java/javase/17/docs/api//java.base/java/util/function/package-summary.html)
+> package.*
+
+Examples:
+
+```python
+from dev4py.utils.types import Function, Predicate, Consumer
+
+# Function sample
+int_to_str: Function[int, str] = lambda i: str(i)
+str_result: str = int_to_str(1)  # '1'
+
+# Predicate sample
+str_predicate: Predicate[str] = lambda s: s == "A value"
+pred_result: bool = str_predicate("Value to test")  # False
+
+# Consumer sample
+def sample(consumer: Consumer[str], value: str) -> None:
+    consumer(value)
+
+def my_consumer(arg: str) -> None:
+    print(arg)
+
+sample(my_consumer, "My value")  # My value
+```
 
-setup(**setup_kwargs)
```

