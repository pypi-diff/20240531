# Comparing `tmp/processing_pypelines-0.0.60.tar.gz` & `tmp/processing_pypelines-0.0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processing_pypelines-0.0.60.tar", last modified: Wed May 29 21:12:05 2024, max compression
+gzip compressed data, was "processing_pypelines-0.0.61.tar", last modified: Thu May 30 16:56:12 2024, max compression
```

## Comparing `processing_pypelines-0.0.60.tar` & `processing_pypelines-0.0.61.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1073 2024-05-29 21:11:56.073603 processing_pypelines-0.0.60/LICENSE
--rw-r--r--   0        0        0      118 2024-05-29 21:11:56.073603 processing_pypelines-0.0.60/README.md
--rw-r--r--   0        0        0     1152 2024-05-29 21:12:05.097519 processing_pypelines-0.0.60/pyproject.toml
--rw-r--r--   0        0        0      367 2024-05-29 21:11:56.077603 processing_pypelines-0.0.60/src/pypelines/__init__.py
--rw-r--r--   0        0        0     4483 2024-05-29 21:11:56.077603 processing_pypelines-0.0.60/src/pypelines/accessors.py
--rw-r--r--   0        0        0     4671 2024-05-29 21:11:56.077603 processing_pypelines-0.0.60/src/pypelines/arguments.py
--rw-r--r--   0        0        0    34226 2024-05-29 21:11:56.077603 processing_pypelines-0.0.60/src/pypelines/celery_tasks.py
--rw-r--r--   0        0        0    11851 2024-05-29 21:11:56.077603 processing_pypelines-0.0.60/src/pypelines/disk.py
--rw-r--r--   0        0        0     6647 2024-05-29 21:11:56.077603 processing_pypelines-0.0.60/src/pypelines/examples.py
--rw-r--r--   0        0        0   352259 2024-05-29 21:11:56.081603 processing_pypelines-0.0.60/src/pypelines/feature_test.ipynb
--rw-r--r--   0        0        0     7880 2024-05-29 21:11:56.081603 processing_pypelines-0.0.60/src/pypelines/graphs.py
--rw-r--r--   0        0        0    17073 2024-05-29 21:11:56.081603 processing_pypelines-0.0.60/src/pypelines/loggs.py
--rw-r--r--   0        0        0     5985 2024-05-29 21:11:56.081603 processing_pypelines-0.0.60/src/pypelines/multisession.py
--rw-r--r--   0        0        0    18914 2024-05-29 21:11:56.081603 processing_pypelines-0.0.60/src/pypelines/pickle_backend.py
--rw-r--r--   0        0        0     6662 2024-05-29 21:11:56.081603 processing_pypelines-0.0.60/src/pypelines/pipelines.py
--rw-r--r--   0        0        0     9547 2024-05-29 21:11:56.081603 processing_pypelines-0.0.60/src/pypelines/pipes.py
--rw-r--r--   0        0        0     3084 2024-05-29 21:11:56.081603 processing_pypelines-0.0.60/src/pypelines/sessions.py
--rw-r--r--   0        0        0    37044 2024-05-29 21:11:56.081603 processing_pypelines-0.0.60/src/pypelines/steps.py
--rw-r--r--   0        0        0     3915 2024-05-29 21:11:56.081603 processing_pypelines-0.0.60/src/pypelines/tasks.py
--rw-r--r--   0        0        0     7360 2024-05-29 21:11:56.081603 processing_pypelines-0.0.60/src/pypelines/versions.py
--rw-r--r--   0        0        0        0 2024-05-29 21:11:56.133603 processing_pypelines-0.0.60/tests/__init__.py
--rw-r--r--   0        0        0      962 2024-05-29 21:11:56.085603 processing_pypelines-0.0.60/tests/tests.py
--rw-r--r--   0        0        0     1230 2024-05-29 21:11:56.085603 processing_pypelines-0.0.60/tests/versions_example.json
--rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 processing_pypelines-0.0.60/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-30 16:56:02.600375 processing_pypelines-0.0.61/LICENSE
+-rw-r--r--   0        0        0      118 2024-05-30 16:56:02.600375 processing_pypelines-0.0.61/README.md
+-rw-r--r--   0        0        0     1152 2024-05-30 16:56:12.156258 processing_pypelines-0.0.61/pyproject.toml
+-rw-r--r--   0        0        0      367 2024-05-30 16:56:02.600375 processing_pypelines-0.0.61/src/pypelines/__init__.py
+-rw-r--r--   0        0        0     4483 2024-05-30 16:56:02.604375 processing_pypelines-0.0.61/src/pypelines/accessors.py
+-rw-r--r--   0        0        0     4671 2024-05-30 16:56:02.604375 processing_pypelines-0.0.61/src/pypelines/arguments.py
+-rw-r--r--   0        0        0    34304 2024-05-30 16:56:02.604375 processing_pypelines-0.0.61/src/pypelines/celery_tasks.py
+-rw-r--r--   0        0        0    11851 2024-05-30 16:56:02.604375 processing_pypelines-0.0.61/src/pypelines/disk.py
+-rw-r--r--   0        0        0     6647 2024-05-30 16:56:02.604375 processing_pypelines-0.0.61/src/pypelines/examples.py
+-rw-r--r--   0        0        0   352259 2024-05-30 16:56:02.604375 processing_pypelines-0.0.61/src/pypelines/feature_test.ipynb
+-rw-r--r--   0        0        0     7880 2024-05-30 16:56:02.604375 processing_pypelines-0.0.61/src/pypelines/graphs.py
+-rw-r--r--   0        0        0    17073 2024-05-30 16:56:02.604375 processing_pypelines-0.0.61/src/pypelines/loggs.py
+-rw-r--r--   0        0        0     5985 2024-05-30 16:56:02.604375 processing_pypelines-0.0.61/src/pypelines/multisession.py
+-rw-r--r--   0        0        0    18914 2024-05-30 16:56:02.608375 processing_pypelines-0.0.61/src/pypelines/pickle_backend.py
+-rw-r--r--   0        0        0     6662 2024-05-30 16:56:02.608375 processing_pypelines-0.0.61/src/pypelines/pipelines.py
+-rw-r--r--   0        0        0     9547 2024-05-30 16:56:02.608375 processing_pypelines-0.0.61/src/pypelines/pipes.py
+-rw-r--r--   0        0        0     3084 2024-05-30 16:56:02.608375 processing_pypelines-0.0.61/src/pypelines/sessions.py
+-rw-r--r--   0        0        0    36861 2024-05-30 16:56:02.608375 processing_pypelines-0.0.61/src/pypelines/steps.py
+-rw-r--r--   0        0        0     3915 2024-05-30 16:56:02.608375 processing_pypelines-0.0.61/src/pypelines/tasks.py
+-rw-r--r--   0        0        0     7360 2024-05-30 16:56:02.608375 processing_pypelines-0.0.61/src/pypelines/versions.py
+-rw-r--r--   0        0        0        0 2024-05-30 16:56:02.676374 processing_pypelines-0.0.61/tests/__init__.py
+-rw-r--r--   0        0        0      962 2024-05-30 16:56:02.608375 processing_pypelines-0.0.61/tests/tests.py
+-rw-r--r--   0        0        0     1230 2024-05-30 16:56:02.608375 processing_pypelines-0.0.61/tests/versions_example.json
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 processing_pypelines-0.0.61/PKG-INFO
```

### Comparing `processing_pypelines-0.0.60/LICENSE` & `processing_pypelines-0.0.61/LICENSE`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.60/pyproject.toml` & `processing_pypelines-0.0.61/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 maintainers = [
     { name = "Timothé Jost-Mousseau", email = "timothe.jost-mousseau@pasteur.fr" },
 ]
 description = "Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api"
 readme = "README.md"
 requires-python = ">=3.10"
 dynamic = []
-version = "0.0.60"
+version = "0.0.61"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 celery = [
     "celery>=5.3.5",
```

### Comparing `processing_pypelines-0.0.60/src/pypelines/accessors.py` & `processing_pypelines-0.0.61/src/pypelines/accessors.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.60/src/pypelines/arguments.py` & `processing_pypelines-0.0.61/src/pypelines/arguments.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.60/src/pypelines/celery_tasks.py` & `processing_pypelines-0.0.61/src/pypelines/celery_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -711,15 +711,18 @@
 
     def get_remote_tasks(self):
         """Retrieve information about remote tasks.
 
         Returns:
             dict: A dictionary containing information about remote tasks, including workers and task names.
         """
-        registered_tasks = self.control.inspect().registered_tasks()
+        try:
+            registered_tasks = self.control.inspect().registered_tasks()
+        except ConnectionResetError:
+            return None
         workers = []
         task_names = []
         if registered_tasks:
             for worker, tasks in registered_tasks.items():
                 workers.append(worker)
                 for task in tasks:
                     task_names.append(task)
```

### Comparing `processing_pypelines-0.0.60/src/pypelines/disk.py` & `processing_pypelines-0.0.61/src/pypelines/disk.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.60/src/pypelines/examples.py` & `processing_pypelines-0.0.61/src/pypelines/examples.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.60/src/pypelines/feature_test.ipynb` & `processing_pypelines-0.0.61/src/pypelines/feature_test.ipynb`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.60/src/pypelines/graphs.py` & `processing_pypelines-0.0.61/src/pypelines/graphs.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.60/src/pypelines/loggs.py` & `processing_pypelines-0.0.61/src/pypelines/loggs.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.60/src/pypelines/multisession.py` & `processing_pypelines-0.0.61/src/pypelines/multisession.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.60/src/pypelines/pickle_backend.py` & `processing_pypelines-0.0.61/src/pypelines/pickle_backend.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.60/src/pypelines/pipelines.py` & `processing_pypelines-0.0.61/src/pypelines/pipelines.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.60/src/pypelines/pipes.py` & `processing_pypelines-0.0.61/src/pypelines/pipes.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.60/src/pypelines/sessions.py` & `processing_pypelines-0.0.61/src/pypelines/sessions.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.60/src/pypelines/steps.py` & `processing_pypelines-0.0.61/src/pypelines/steps.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,14 +296,18 @@
 
         Returns:
             int: The level of the step.
         """
         self.pipeline.resolve()
         return StepLevel(self).resolve_level(selfish=selfish)
 
+    def is_required(self):
+        # TODO implement this (False if the step is not present in any other step' requirement stack, else True)
+        raise NotImplementedError
+
     def get_disk_object(self, session, extra=None):
         """Return a disk object based on the provided session and optional extra parameters.
 
         Args:
             session: The session to use for creating the disk object.
             extra (optional): Additional parameters to be passed to the disk object. Defaults to None.
 
@@ -513,37 +517,15 @@
             if self.is_refresh_in_kwargs():
                 kwargs.update({"refresh": refresh})
             result = self.pipe.pre_run_wrapper(self.worker(session, *args, **kwargs))
 
             if save_output:
                 logger.save(f"Saving the generated {self.relative_name}{'.' + extra if extra else ''} output.")
                 disk_object.save(result)
-
-                # AFTER the saving has been done, if there is some callback function that should be run, we execute them
-                # If an exception is thrown in a callback, the whole pipeline will stop, intentionnaly.
-                # TODO an option could be added to catch, display and store exceptions tracebacks,
-                # while allowing the pipeline to continue,
-                # in case the callbacks are not absolutely necessary for the pipeline process. (ex, generate plots)
-                for callback_data in self.callbacks:
-                    arguments = {"session": session, "extra": extra, "pipeline": self.pipeline}
-                    if isinstance(callback_data, tuple):
-                        callback = callback_data[0]
-                        overriding_arguments = callback_data[1]
-                    else:
-                        callback = callback_data
-                        overriding_arguments = {}
-                    arguments.update(overriding_arguments)
-                    try:
-                        callback(**arguments)
-                    except Exception as e:
-                        import traceback
-
-                        traceback_msg = traceback.format_exc()
-                        logger.error(f"The callback {callback} failed with error : {e}")
-                        logger.error("Full traceback below :\n" + traceback_msg)
+                self.run_callbacks(session, extra, show_plots=False)
 
             return result
 
         original_signature = inspect.signature(self.worker)
         original_params = list(original_signature.parameters.values())
 
         kwarg_position = len(original_params)
@@ -569,14 +551,35 @@
 
         # Replace the wrapper function's signature with the new one
         wrapper.__signature__ = original_signature.replace(parameters=original_params)
         wrapper.__doc__ = self.generate_doc()
 
         return wrapper
 
+    def run_callbacks(self, session, extra="", show_plots=True) -> None:
+        logger = logging.getLogger("callback_runner")
+        for callback_data in self.callbacks:
+            arguments = {"session": session, "extra": extra, "pipeline": self.pipeline}
+            if isinstance(callback_data, tuple):
+                callback = callback_data[0]
+                overriding_arguments = callback_data[1]
+            else:
+                callback = callback_data
+                overriding_arguments = {}
+            arguments.update(overriding_arguments)
+            try:
+                logger.info(f"Running the callback {callback.__name__}")
+                callback(**arguments)
+            except Exception as e:
+                import traceback
+
+                traceback_msg = traceback.format_exc()
+                logger.error(f"The callback {callback} failed with error : {e}")
+                logger.error("Full traceback below :\n" + traceback_msg)
+
     def generate_doc(self) -> str:
         """Generate a new docstring by inserting a chapter about Pipeline Args before the existing
         docstring of the function.
         If the existing docstring contains 'Raises' or 'Returns', the new chapter will be inserted before that.
         If not, it will be inserted at the end of the existing docstring.
         """
```

### Comparing `processing_pypelines-0.0.60/src/pypelines/tasks.py` & `processing_pypelines-0.0.61/src/pypelines/tasks.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.60/src/pypelines/versions.py` & `processing_pypelines-0.0.61/src/pypelines/versions.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.60/tests/tests.py` & `processing_pypelines-0.0.61/tests/tests.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.60/tests/versions_example.json` & `processing_pypelines-0.0.61/tests/versions_example.json`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.60/PKG-INFO` & `processing_pypelines-0.0.61/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processing-pypelines
-Version: 0.0.60
+Version: 0.0.61
 Summary: Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api
 Home-page: https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Author-Email: =?utf-8?q?Timoth=C3=A9_Jost-Mousseau?= <timothe.jost-mousseau@pasteur.fr>
 Maintainer-Email: =?utf-8?q?Timoth=C3=A9_Jost-Mousseau?= <timothe.jost-mousseau@pasteur.fr>
 License: MIT
 Project-URL: Homepage, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: Repository, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
```

