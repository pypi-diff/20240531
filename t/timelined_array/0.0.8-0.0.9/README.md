# Comparing `tmp/timelined_array-0.0.8.tar.gz` & `tmp/timelined_array-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timelined_array-0.0.8.tar", last modified: Wed May 29 22:15:57 2024, max compression
+gzip compressed data, was "timelined_array-0.0.9.tar", last modified: Thu May 30 18:46:59 2024, max compression
```

## Comparing `timelined_array-0.0.8.tar` & `timelined_array-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2024-05-29 22:15:35.716439 timelined_array-0.0.8/LICENSE
--rw-r--r--   0        0        0    10618 2024-05-29 22:15:35.716439 timelined_array-0.0.8/README.md
--rw-r--r--   0        0        0      613 2024-05-29 22:15:57.720723 timelined_array-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       97 2024-05-29 22:15:35.716439 timelined_array-0.0.8/src/timelined_array/__init__.py
--rw-r--r--   0        0        0    52912 2024-05-29 22:15:35.716439 timelined_array-0.0.8/src/timelined_array/time.py
--rw-r--r--   0        0        0        0 2024-05-29 22:15:35.716439 timelined_array-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0    10988 1970-01-01 00:00:00.000000 timelined_array-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-30 18:46:47.436293 timelined_array-0.0.9/LICENSE
+-rw-r--r--   0        0        0    10618 2024-05-30 18:46:47.436293 timelined_array-0.0.9/README.md
+-rw-r--r--   0        0        0      613 2024-05-30 18:46:59.096357 timelined_array-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       97 2024-05-30 18:46:47.436293 timelined_array-0.0.9/src/timelined_array/__init__.py
+-rw-r--r--   0        0        0    52278 2024-05-30 18:46:47.436293 timelined_array-0.0.9/src/timelined_array/time.py
+-rw-r--r--   0        0        0        0 2024-05-30 18:46:47.436293 timelined_array-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0    10988 1970-01-01 00:00:00.000000 timelined_array-0.0.9/PKG-INFO
```

### Comparing `timelined_array-0.0.8/LICENSE` & `timelined_array-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `timelined_array-0.0.8/README.md` & `timelined_array-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `timelined_array-0.0.8/pyproject.toml` & `timelined_array-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ]
 dependencies = [
     "numpy",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 dynamic = []
-version = "0.0.8"
+version = "0.0.9"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `timelined_array-0.0.8/src/timelined_array/time.py` & `timelined_array-0.0.9/src/timelined_array/time.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # -*- coding: utf-8 -*-
 
 import numpy as np
 from logging import getLogger
-from typing import Tuple, List, Protocol, Type
 from enum import Enum
 import operator
 
+from typing import Tuple, List, Protocol, Type, Callable, Any
+
+OperatorType = Callable[[Any, Any], bool]
+
 # class syntax
 
 logger = getLogger("timelined_array")
 
 
 class TimeCompatibleProtocol(Protocol):
 
@@ -145,64 +148,47 @@
         """Largest time between two timeline points, multiplied by max_step_mult"""
         if self._max_step is None:
             diff = np.diff(self)
             self._max_step = diff[np.argmax(np.absolute(diff))]
         return self._max_step * self.max_step_mult
 
 
-class Boundary(Enum):
-    inclusive = 0
-    exclusive = 1
-    inc = 0
-    exc = 1
-
-    @staticmethod
-    def get_operation(boundary, setting):
-        """Return the appropriate comparison operator based on the boundary and setting.
-
-        Args:
-            boundary (str): The boundary type, either "start" or "stop".
-            setting (Boundary): The setting for the boundary, either inclusive or exclusive.
-
-        Returns:
-            function: The comparison operator based on the boundary and setting.
-
-        Raises:
-            ValueError: If the boundary or setting is invalid.
-        """
-
-        if boundary == "start":
-            if setting == Boundary.inclusive:
-                return operator.ge
-            elif setting == Boundary.exclusive:
-                return operator.gt
-            else:
-                raise ValueError
-        elif boundary == "stop":
-            if setting == Boundary.inclusive:
-                return operator.le
-            elif setting == Boundary.exclusive:
-                return operator.lt
-            else:
-                raise ValueError
-        else:
-            raise ValueError
+class StartBoundary(Enum):
+    inclusive = operator.ge
+    exclusive = operator.gt
+    inc = operator.ge
+    exc = operator.gt
+
+
+class StoptBoundary(Enum):
+    inclusive = operator.le
+    exclusive = operator.lt
+    inc = operator.le
+    exc = operator.lt
+
+
+class EdgePolicy(Enum):
+    start = StartBoundary
+    stop = StoptBoundary
 
 
 class TimeIndexer:
     """The time indexer indexes by default from >= to the time start, and strictly < to time stop"""
 
-    start_mode = Boundary.inclusive
-    stop_mode = Boundary.exclusive
+    _start_operation: OperatorType
+    _stop_operation: OperatorType
 
-    _start_operation = Boundary.get_operation("start", start_mode)
-    _stop_operation = Boundary.get_operation("stop", stop_mode)
-
-    def __init__(self, array: TimeCompatibleProtocol):
+    def __init__(self, array: TimeCompatibleProtocol, start="inclusive", stop="exclusive"):
         self.array = array
+        self.set_edge_policy(start, stop)
+
+    def set_edge_policy(self, start="inclusive", stop="exclusive"):
+        self._start_operation = EdgePolicy["start"].value[start]
+        self._stop_operation = EdgePolicy["stop"].value[stop]
+        return self
 
     def time_to_index(
         self, time: float | int | slice | Tuple[int | float] | List[float | int | slice | Tuple[int | float]]
     ):
         """Converts time to index based on different input types.
 
         Args:
@@ -225,15 +211,15 @@
         elif isinstance(time, list):
             return np.array([self.time_to_index(t) for t in time])
         elif isinstance(time, tuple):
             return self.get_iindex(*[time[i] if len(time) > i else None for i in range(3)])
         elif isinstance(time, (int, float)):
             return self.get_iindex(sec_start=time).start
         else:
-            raise ValueError("Cannot process time to index ")
+            raise ValueError("Cannot process time to index")
 
     seconds_to_index = time_to_index
 
     def _insert_time_index(self, time_index):
         """Inserts a time index into the full index.
 
         Args:
@@ -329,25 +315,24 @@
             step = 1
         else:
             step = int(np.round(sec_step / self.array.timeline.step))
             if step < 1:
                 step = 1
         return slice(start, stop, step)
 
-    def __call__(self, start=None, stop=None):
-        if start is not None:
-            self._start_operation = Boundary.get_operation("start", start)
-        if stop is not None:
-            self._stop_operation = Boundary.get_operation("stop", stop)
+    def __call__(self, start="inclusive", stop="exclusive"):
+        return self.set_edge_policy(start, stop)
 
 
 class TimeMixin:
 
     time_dimension: int
     timeline: Timeline
+    start_policy = "inclusive"
+    stop_policy = "exclusive"
 
     def _time_dimension_in_axis(self, axis: int | Tuple[int, ...] | None) -> bool:
         """Check if the time dimension is present in the specified axis.
 
         Args:
             axis (int | Tuple[int, ...] | None): The axis to check for the time dimension.
 
@@ -618,15 +603,15 @@
             f"and timeline shape {self.timeline.shape}"
         )
 
     @property
     def itime(self: TimeCompatibleProtocol):
         """Return a TimeIndexer object based on the given TimeCompatibleProtocol object."""
 
-        return TimeIndexer(self)
+        return TimeIndexer(self, self.start_policy, self.stop_policy)
 
     isec = itime
 
     def align_trace(self, start: float, element_nb: int):
         """Aligns the timelined array by making it start from a timepoint in time-units (synchronizing)
         and cutting the array N elements after the start point.
 
@@ -1180,15 +1165,15 @@
         Returns:
             TimelinedArray | np.ndarray: Indexed result based on the provided index.
         """
 
         index, final_timeline, final_time_dimension = self._get_indexed_times(index)
 
         if final_timeline is None or final_time_dimension is None:
-            return np.array(self).__getitem__(index)
+            return np.asarray(self).__getitem__(index)
 
         indexed_result = super().__getitem__(index)
 
         logger.debug(
             f"Current object : {self.array_info}.\n"
             f"Newly indexed object : {type(indexed_result).__name__} of shape {indexed_result.shape}, "
             f"time_dimension {final_time_dimension} and timeline shape {final_timeline.shape}"
```

### Comparing `timelined_array-0.0.8/PKG-INFO` & `timelined_array-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timelined_array
-Version: 0.0.8
+Version: 0.0.9
 Summary: Manage easily 1 or multidimensionnal samples numpy arrays that are time related. Extends numpy without removing any of it's abilities on such arrays.
 Author-Email: Timothe Jost <timothe.jost@wanadoo.fr>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: numpy
 Description-Content-Type: text/markdown
```

