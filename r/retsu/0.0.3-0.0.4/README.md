# Comparing `tmp/retsu-0.0.3.tar.gz` & `tmp/retsu-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retsu-0.0.3.tar", max compression
+gzip compressed data, was "retsu-0.0.4.tar", max compression
```

## Comparing `retsu-0.0.3.tar` & `retsu-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1514 2024-05-29 04:16:24.816518 retsu-0.0.3/LICENSE
--rw-r--r--   0        0        0      319 2024-05-29 04:16:24.820518 retsu-0.0.3/README.md
--rw-r--r--   0        0        0     2224 2024-05-29 04:17:28.440662 retsu-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      666 2024-05-29 04:17:28.436662 retsu-0.0.3/src/retsu/__init__.py
--rw-r--r--   0        0        0     1956 2024-05-29 04:16:24.820518 retsu-0.0.3/src/retsu/celery.py
--rw-r--r--   0        0        0     5513 2024-05-29 04:16:24.820518 retsu-0.0.3/src/retsu/core.py
--rw-r--r--   0        0        0       31 2024-05-29 04:16:24.820518 retsu-0.0.3/src/retsu/plugins/__init__.py
--rw-r--r--   0        0        0      827 2024-05-29 04:16:24.824518 retsu-0.0.3/src/retsu/plugins/django.py
--rw-r--r--   0        0        0        0 2024-05-29 04:16:24.824518 retsu-0.0.3/src/retsu/py.typed
--rw-r--r--   0        0        0     1075 1970-01-01 00:00:00.000000 retsu-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1514 2024-05-31 03:55:05.924349 retsu-0.0.4/LICENSE
+-rw-r--r--   0        0        0      319 2024-05-31 03:55:05.924349 retsu-0.0.4/README.md
+-rw-r--r--   0        0        0     2255 2024-05-31 03:56:08.321178 retsu-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      733 2024-05-31 03:56:08.317178 retsu-0.0.4/src/retsu/__init__.py
+-rw-r--r--   0        0        0     2097 2024-05-31 03:55:05.928349 retsu-0.0.4/src/retsu/celery.py
+-rw-r--r--   0        0        0     4331 2024-05-31 03:55:05.928349 retsu-0.0.4/src/retsu/core.py
+-rw-r--r--   0        0        0       31 2024-05-31 03:55:05.928349 retsu-0.0.4/src/retsu/plugins/__init__.py
+-rw-r--r--   0        0        0      827 2024-05-31 03:55:05.928349 retsu-0.0.4/src/retsu/plugins/django.py
+-rw-r--r--   0        0        0        0 2024-05-31 03:55:05.928349 retsu-0.0.4/src/retsu/py.typed
+-rw-r--r--   0        0        0     6366 2024-05-31 03:55:05.928349 retsu-0.0.4/src/retsu/tracking.py
+-rw-r--r--   0        0        0     1119 1970-01-01 00:00:00.000000 retsu-0.0.4/PKG-INFO
```

### Comparing `retsu-0.0.3/LICENSE` & `retsu-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `retsu-0.0.3/pyproject.toml` & `retsu-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "retsu"
-version = "0.0.3"  # semantic-release
+version = "0.0.4"  # semantic-release
 description = "Retsu aims to wrap-up Celery in way to facilitate to create parallel and serial tasks"
 readme = "README.md"
 authors = ["Ivan Ogasawara <ivan.ogasawara@gmail.com>"]
 packages = [
   {include = "retsu", from="src"},
 ]
 license = "BSD 3 Clause"
@@ -17,14 +17,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4"
 atpublic = ">=4.0"
 celery = ">=5"
 redis = ">=5"
 django = { version = ">=3", optional = true }
+typing-extensions = ">=4.12.0"
 
 [tool.poetry.extras]
 django = [
   "django",
 ]
```

### Comparing `retsu-0.0.3/src/retsu/__init__.py` & `retsu-0.0.4/src/retsu/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 """Retsu."""
 
 from importlib import metadata as importlib_metadata
 
 from retsu.core import (
     ParallelTask,
-    ResultTask,
     SerialTask,
+    Task,
     TaskManager,
 )
+from retsu.tracking import (
+    ResultTaskManager,
+)
 
 
 def get_version() -> str:
     """Return the program version."""
     try:
         return importlib_metadata.version(__name__)
     except importlib_metadata.PackageNotFoundError:  # pragma: no cover
-        return "0.0.3"  # semantic-release
+        return "0.0.4"  # semantic-release
 
 
 version = get_version()
 
 __version__ = version
 __author__ = "Ivan Ogasawara"
 __email__ = "ivan.ogasawara@gmail.com"
 
 __all__ = [
     "__version__",
     "__author__",
     "__email__",
     "ParallelTask",
-    "ResultTask",
+    "ResultTaskManager",
     "SerialTask",
+    "Task",
     "TaskManager",
 ]
```

### Comparing `retsu-0.0.3/src/retsu/celery.py` & `retsu-0.0.4/src/retsu/celery.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,52 @@
 """Retsu tasks with celery."""
 
 from __future__ import annotations
 
-from typing import Optional
+from typing import Any, Optional
 
 import celery
 
-from celery import chain, chord
+from celery import chain, chord, group
+from public import public
 
 from retsu.core import ParallelTask, SerialTask
 
 
 class CeleryTask:
     """Celery Task class."""
 
-    def task(self, *args, task_id: str, **kwargs) -> None:  # type: ignore
+    def task(self, *args, task_id: str, **kwargs) -> Any:  # type: ignore
         """Define the task to be executed."""
         chord_tasks, chord_callback = self.get_chord_tasks(
             *args, task_id=task_id, **kwargs
         )
         chain_tasks = self.get_chain_tasks(*args, task_id=task_id, **kwargs)
 
         # start the tasks
         if chord_tasks:
             if chord_callback:
                 workflow_chord = chord(chord_tasks, chord_callback)
             else:
-                workflow_chord = chord(chord_tasks)
+                workflow_chord = group(chord_tasks)
             promise_chord = workflow_chord.apply_async()
 
         if chain_tasks:
             workflow_chain = chain(chord_tasks)
             promise_chain = workflow_chain.apply_async()
 
         # wait for the tasks
+        results: list[Any] = []
         if chord_tasks:
-            promise_chord.get()
+            results.extend(promise_chord.get())
 
         if chain_tasks:
-            promise_chain.get()
+            results.append(promise_chain.get())
+
+        return results
 
     def get_chord_tasks(  # type: ignore
         self, *args, **kwargs
     ) -> tuple[list[celery.Signature], Optional[celery.Signature]]:
         """
         Run tasks with chord.
 
@@ -59,17 +63,19 @@
         self, *args, **kwargs
     ) -> list[celery.Signature]:
         """Run tasks with chain."""
         chain_tasks: list[celery.Signature] = []
         return chain_tasks
 
 
+@public
 class ParallelCeleryTask(CeleryTask, ParallelTask):
     """Parallel Task for Celery."""
 
     ...
 
 
+@public
 class SerialCeleryTask(CeleryTask, SerialTask):
     """Serial Task for Celery."""
 
     ...
```

### Comparing `retsu-0.0.3/src/retsu/core.py` & `retsu-0.0.4/src/retsu/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,86 +1,37 @@
 """Retsu core classes."""
 
 from __future__ import annotations
 
-import json
 import multiprocessing as mp
-import os
 import warnings
 
 from abc import abstractmethod
-from pathlib import Path
-from typing import Any, Optional, cast
+from datetime import datetime
+from typing import Any, Optional
 from uuid import uuid4
 
 from public import public
 
-
-class ResultTask:
-    """Result from a task."""
-
-    def __init__(self) -> None:
-        """Initialize ResultTask."""
-        self.result_path = Path(
-            os.getenv("RETSU_RESULT_PATH", "/tmp/retsu/results")
-        )
-        os.makedirs(self.result_path, exist_ok=True)
-
-    @public
-    def save(self, task_id: str, result: Any) -> None:
-        """Save the result in a file."""
-        with open(self.result_path / f"{task_id}.json", "w") as f:
-            json.dump(
-                {"task_id": task_id, "result": result},
-                f,
-                indent=2,
-            )
-
-    @public
-    def load(self, task_id: str) -> dict[str, Any]:
-        """Load the result from a file."""
-        result_file = self.result_path / f"{task_id}.json"
-        if not result_file.exists():
-            raise Exception(f"File {result_file} doesn't exist.")
-        with open(result_file, "r") as f:
-            return cast(dict[str, Any], json.load(f))
-
-    @public
-    def status(self, task_id: str) -> bool:
-        """Return if the result for a given task was already stored."""
-        result_file = self.result_path / f"{task_id}.json"
-        return result_file.exists()
-
-    @public
-    def get(self, task_id: str) -> Any:
-        """Return the result for given task."""
-        if not self.status(task_id):
-            return {"status": False, "message": "Result not ready."}
-
-        return self.load(task_id)
+from retsu.tracking import ResultTaskManager, create_result_task_manager
 
 
 @public
 class Task:
     """Main class for handling a task."""
 
     def __init__(self, workers: int = 1) -> None:
         """Initialize a task object."""
         self.active = True
         self.workers = workers
-        self.result = ResultTask()
+        self.result: ResultTaskManager = create_result_task_manager()
         self.queue_in: mp.Queue[Any] = mp.Queue()
         self.processes: list[mp.Process] = []
 
     @public
-    def get_result(self, task_id: str) -> Any:
-        """Get the result for given task id."""
-        return self.result.get(task_id)
-
-    @public
     def start(self) -> None:
         """Start processes."""
         for _ in range(self.workers):
             p = mp.Process(target=self.run)
             p.start()
             self.processes.append(p)
 
@@ -101,44 +52,47 @@
 
         self.queue_in.close()
         self.queue_in.join_thread()
 
     @public
     def request(self, *args, **kwargs) -> str:  # type: ignore
         """Feed the queue with data from the request for the task."""
-        key = uuid4().hex
-        print(
-            {
-                "task_id": key,
-                "args": args,
-                "kwargs": kwargs,
-            }
-        )
+        task_id = uuid4().hex
+        metadata = {
+            "status": "starting",
+            "created_at": datetime.now().isoformat(),
+            "updated_at": datetime.now().isoformat(),
+        }
+        self.result.create(task_id, metadata)
         self.queue_in.put(
             {
-                "task_id": key,
+                "task_id": task_id,
                 "args": args,
                 "kwargs": kwargs,
             },
             block=False,
         )
-        return key
+        return task_id
 
     @abstractmethod
-    def task(self, *args, task_id: str, **kwargs) -> None:  # type: ignore
+    def task(self, *args, task_id: str, **kwargs) -> Any:  # type: ignore
         """Define the task to be executed."""
         raise Exception("`task` not implemented yet.")
 
-    def prepare_task(self, data: Any) -> None:
+    def prepare_task(self, data: dict[str, Any]) -> None:
         """Call the task with the necessary arguments."""
-        self.task(
+        task_id = data.pop("task_id")
+        self.result.metadata.update(task_id, "status", "running")
+        result = self.task(
             *data["args"],
-            task_id=data["task_id"],
+            task_id=task_id,
             **data["kwargs"],
         )
+        self.result.save(task_id, result)
+        self.result.metadata.update(task_id, "status", "completed")
 
     @public
     def run(self) -> None:
         """Run the task with data from the queue."""
         while self.active:
             data = self.queue_in.get()
             if data is None:
```

### Comparing `retsu-0.0.3/src/retsu/plugins/django.py` & `retsu-0.0.4/src/retsu/plugins/django.py`

 * *Files identical despite different names*

### Comparing `retsu-0.0.3/PKG-INFO` & `retsu-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retsu
-Version: 0.0.3
+Version: 0.0.4
 Summary: Retsu aims to wrap-up Celery in way to facilitate to create parallel and serial tasks
 License: BSD 3 Clause
 Author: Ivan Ogasawara
 Author-email: ivan.ogasawara@gmail.com
 Requires-Python: >=3.8.1,<4
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: django
 Requires-Dist: atpublic (>=4.0)
 Requires-Dist: celery (>=5)
 Requires-Dist: django (>=3) ; extra == "django"
 Requires-Dist: redis (>=5)
+Requires-Dist: typing-extensions (>=4.12.0)
 Description-Content-Type: text/markdown
 
 # Retsu
 
 Retsu aims to wrap-up Celery in way to facilitate to create parallel and serial
 tasks
```

