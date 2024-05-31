# Comparing `tmp/synctodoist-0.3.2.tar.gz` & `tmp/synctodoist-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synctodoist-0.3.2.tar", max compression
+gzip compressed data, was "synctodoist-0.3.3.tar", max compression
```

## Comparing `synctodoist-0.3.2.tar` & `synctodoist-0.3.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rwxr-xr-x   0        0        0     1068 2022-12-11 09:21:02.000000 synctodoist-0.3.2/LICENSE.md
--rwxr-xr-x   0        0        0     1309 2022-12-22 13:33:09.000000 synctodoist-0.3.2/README.md
--rwxr-xr-x   0        0        0     2188 2024-01-14 11:02:57.691143 synctodoist-0.3.2/pyproject.toml
--rwxr-xr-x   0        0        0       36 2022-12-11 09:40:38.000000 synctodoist-0.3.2/synctodoist/__init__.py
--rwxr-xr-x   0        0        0       90 2022-12-13 06:24:20.000000 synctodoist-0.3.2/synctodoist/exceptions.py
--rwxr-xr-x   0        0        0      510 2022-12-20 04:59:43.000000 synctodoist-0.3.2/synctodoist/managers/__init__.py
--rwxr-xr-x   0        0        0     7078 2024-01-14 08:50:01.089055 synctodoist-0.3.2/synctodoist/managers/base_manager.py
--rwxr-xr-x   0        0        0     4933 2023-12-12 09:35:04.007512 synctodoist-0.3.2/synctodoist/managers/command_manager.py
--rwxr-xr-x   0        0        0      584 2022-12-25 05:04:46.000000 synctodoist-0.3.2/synctodoist/managers/label_manager.py
--rwxr-xr-x   0        0        0     1273 2024-01-14 08:50:01.089694 synctodoist-0.3.2/synctodoist/managers/project_manager.py
--rwxr-xr-x   0        0        0      303 2022-12-25 05:04:56.000000 synctodoist-0.3.2/synctodoist/managers/reminder_manager.py
--rwxr-xr-x   0        0        0      297 2022-12-25 05:05:05.000000 synctodoist-0.3.2/synctodoist/managers/section_manager.py
--rwxr-xr-x   0        0        0     4240 2024-01-14 08:50:01.090006 synctodoist-0.3.2/synctodoist/managers/task_manager.py
--rwxr-xr-x   0        0        0      330 2022-12-19 06:18:00.000000 synctodoist-0.3.2/synctodoist/models/__init__.py
--rwxr-xr-x   0        0        0      456 2024-01-14 08:50:01.090278 synctodoist-0.3.2/synctodoist/models/command.py
--rwxr-xr-x   0        0        0      334 2024-01-14 08:50:01.090874 synctodoist-0.3.2/synctodoist/models/due.py
--rwxr-xr-x   0        0        0     1445 2022-12-26 16:50:57.000000 synctodoist-0.3.2/synctodoist/models/enums.py
--rwxr-xr-x   0        0        0      621 2024-01-14 08:50:01.091204 synctodoist-0.3.2/synctodoist/models/label.py
--rwxr-xr-x   0        0        0     2720 2024-01-14 08:50:01.091648 synctodoist-0.3.2/synctodoist/models/project.py
--rwxr-xr-x   0        0        0     1014 2024-01-14 08:50:01.093114 synctodoist-0.3.2/synctodoist/models/reminder.py
--rwxr-xr-x   0        0        0      814 2024-01-14 08:50:01.093690 synctodoist-0.3.2/synctodoist/models/section.py
--rwxr-xr-x   0        0        0      535 2024-01-14 10:59:11.939227 synctodoist-0.3.2/synctodoist/models/settings.py
--rwxr-xr-x   0        0        0     1472 2024-01-14 08:50:01.094426 synctodoist-0.3.2/synctodoist/models/task.py
--rwxr-xr-x   0        0        0     1338 2024-01-14 08:50:01.095177 synctodoist-0.3.2/synctodoist/models/todoist_base_model.py
--rwxr-xr-x   0        0        0      131 2022-12-12 15:54:10.000000 synctodoist-0.3.2/synctodoist/models/utils.py
--rwxr-xr-x   0        0        0    21564 2024-01-14 08:50:01.095752 synctodoist-0.3.2/synctodoist/todoist_api.py
--rw-r--r--   0        0        0     2325 1970-01-01 00:00:00.000000 synctodoist-0.3.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1068 2022-12-11 09:21:02.000000 synctodoist-0.3.3/LICENSE.md
+-rwxr-xr-x   0        0        0     1309 2022-12-22 13:33:09.000000 synctodoist-0.3.3/README.md
+-rwxr-xr-x   0        0        0     2206 2024-05-31 14:51:39.126175 synctodoist-0.3.3/pyproject.toml
+-rwxr-xr-x   0        0        0       36 2022-12-11 09:40:38.000000 synctodoist-0.3.3/synctodoist/__init__.py
+-rwxr-xr-x   0        0        0       90 2022-12-13 06:24:20.000000 synctodoist-0.3.3/synctodoist/exceptions.py
+-rwxr-xr-x   0        0        0      510 2022-12-20 04:59:43.000000 synctodoist-0.3.3/synctodoist/managers/__init__.py
+-rwxr-xr-x   0        0        0     7078 2024-01-14 08:50:01.000000 synctodoist-0.3.3/synctodoist/managers/base_manager.py
+-rwxr-xr-x   0        0        0     4933 2023-12-12 09:35:04.000000 synctodoist-0.3.3/synctodoist/managers/command_manager.py
+-rwxr-xr-x   0        0        0      584 2022-12-25 05:04:46.000000 synctodoist-0.3.3/synctodoist/managers/label_manager.py
+-rwxr-xr-x   0        0        0     1273 2024-01-14 08:50:01.000000 synctodoist-0.3.3/synctodoist/managers/project_manager.py
+-rwxr-xr-x   0        0        0      303 2022-12-25 05:04:56.000000 synctodoist-0.3.3/synctodoist/managers/reminder_manager.py
+-rwxr-xr-x   0        0        0      297 2022-12-25 05:05:05.000000 synctodoist-0.3.3/synctodoist/managers/section_manager.py
+-rwxr-xr-x   0        0        0     4240 2024-01-14 08:50:01.000000 synctodoist-0.3.3/synctodoist/managers/task_manager.py
+-rwxr-xr-x   0        0        0      330 2022-12-19 06:18:00.000000 synctodoist-0.3.3/synctodoist/models/__init__.py
+-rwxr-xr-x   0        0        0      456 2024-01-14 08:50:01.000000 synctodoist-0.3.3/synctodoist/models/command.py
+-rwxr-xr-x   0        0        0      334 2024-01-14 08:50:01.000000 synctodoist-0.3.3/synctodoist/models/due.py
+-rwxr-xr-x   0        0        0     1445 2022-12-26 16:50:57.000000 synctodoist-0.3.3/synctodoist/models/enums.py
+-rwxr-xr-x   0        0        0      621 2024-01-14 08:50:01.000000 synctodoist-0.3.3/synctodoist/models/label.py
+-rwxr-xr-x   0        0        0     2720 2024-01-14 08:50:01.000000 synctodoist-0.3.3/synctodoist/models/project.py
+-rwxr-xr-x   0        0        0     1014 2024-01-14 08:50:01.000000 synctodoist-0.3.3/synctodoist/models/reminder.py
+-rwxr-xr-x   0        0        0      814 2024-01-14 08:50:01.000000 synctodoist-0.3.3/synctodoist/models/section.py
+-rwxr-xr-x   0        0        0      535 2024-01-14 10:59:11.000000 synctodoist-0.3.3/synctodoist/models/settings.py
+-rwxr-xr-x   0        0        0     1472 2024-01-14 08:50:01.000000 synctodoist-0.3.3/synctodoist/models/task.py
+-rwxr-xr-x   0        0        0     1338 2024-01-14 08:50:01.000000 synctodoist-0.3.3/synctodoist/models/todoist_base_model.py
+-rwxr-xr-x   0        0        0      131 2022-12-12 15:54:10.000000 synctodoist-0.3.3/synctodoist/models/utils.py
+-rwxr-xr-x   0        0        0    21564 2024-01-14 08:50:01.000000 synctodoist-0.3.3/synctodoist/todoist_api.py
+-rw-r--r--   0        0        0     2364 1970-01-01 00:00:00.000000 synctodoist-0.3.3/PKG-INFO
```

### Comparing `synctodoist-0.3.2/LICENSE.md` & `synctodoist-0.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `synctodoist-0.3.2/README.md` & `synctodoist-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `synctodoist-0.3.2/pyproject.toml` & `synctodoist-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "synctodoist"
-version = "0.3.2"
+version = "0.3.3"
 description = "A Python wrapper for the Todoist Sync API v9"
 license = "MIT"
 authors = ["Gabor Schulz"]
 readme = "README.md"
 homepage = "https://github.com/gaborschulz/synctodoist"
 repository = "https://github.com/gaborschulz/synctodoist"
 documentation = "https://github.com/gaborschulz/synctodoist"
@@ -27,14 +27,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.10"
 httpx = "^0.23.1"
 python-dotenv = "^0.21.0"
 pydantic = "^2.5.3"
 pydantic-settings = "^2.1.0"
+isort = "^5.13.2"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `synctodoist-0.3.2/synctodoist/managers/base_manager.py` & `synctodoist-0.3.3/synctodoist/managers/base_manager.py`

 * *Files identical despite different names*

### Comparing `synctodoist-0.3.2/synctodoist/managers/command_manager.py` & `synctodoist-0.3.3/synctodoist/managers/command_manager.py`

 * *Files identical despite different names*

### Comparing `synctodoist-0.3.2/synctodoist/managers/label_manager.py` & `synctodoist-0.3.3/synctodoist/managers/label_manager.py`

 * *Files identical despite different names*

### Comparing `synctodoist-0.3.2/synctodoist/managers/project_manager.py` & `synctodoist-0.3.3/synctodoist/managers/project_manager.py`

 * *Files identical despite different names*

### Comparing `synctodoist-0.3.2/synctodoist/managers/task_manager.py` & `synctodoist-0.3.3/synctodoist/managers/task_manager.py`

 * *Files identical despite different names*

### Comparing `synctodoist-0.3.2/synctodoist/models/enums.py` & `synctodoist-0.3.3/synctodoist/models/enums.py`

 * *Files identical despite different names*

### Comparing `synctodoist-0.3.2/synctodoist/models/label.py` & `synctodoist-0.3.3/synctodoist/models/label.py`

 * *Files identical despite different names*

### Comparing `synctodoist-0.3.2/synctodoist/models/project.py` & `synctodoist-0.3.3/synctodoist/models/project.py`

 * *Files identical despite different names*

### Comparing `synctodoist-0.3.2/synctodoist/models/reminder.py` & `synctodoist-0.3.3/synctodoist/models/reminder.py`

 * *Files identical despite different names*

### Comparing `synctodoist-0.3.2/synctodoist/models/section.py` & `synctodoist-0.3.3/synctodoist/models/section.py`

 * *Files identical despite different names*

### Comparing `synctodoist-0.3.2/synctodoist/models/settings.py` & `synctodoist-0.3.3/synctodoist/models/settings.py`

 * *Files identical despite different names*

### Comparing `synctodoist-0.3.2/synctodoist/models/task.py` & `synctodoist-0.3.3/synctodoist/models/task.py`

 * *Files identical despite different names*

### Comparing `synctodoist-0.3.2/synctodoist/models/todoist_base_model.py` & `synctodoist-0.3.3/synctodoist/models/todoist_base_model.py`

 * *Files identical despite different names*

### Comparing `synctodoist-0.3.2/synctodoist/todoist_api.py` & `synctodoist-0.3.3/synctodoist/todoist_api.py`

 * *Files identical despite different names*

### Comparing `synctodoist-0.3.2/PKG-INFO` & `synctodoist-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synctodoist
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Python wrapper for the Todoist Sync API v9
 Home-page: https://github.com/gaborschulz/synctodoist
 License: MIT
 Author: Gabor Schulz
 Requires-Python: >=3.10
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: httpx (>=0.23.1,<0.24.0)
+Requires-Dist: isort (>=5.13.2,<6.0.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.1.0,<3.0.0)
 Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
 Project-URL: Documentation, https://github.com/gaborschulz/synctodoist
 Project-URL: Repository, https://github.com/gaborschulz/synctodoist
 Description-Content-Type: text/markdown
```

