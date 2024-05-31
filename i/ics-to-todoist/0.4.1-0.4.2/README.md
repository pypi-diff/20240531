# Comparing `tmp/ics_to_todoist-0.4.1.tar.gz` & `tmp/ics_to_todoist-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ics_to_todoist-0.4.1.tar", max compression
+gzip compressed data, was "ics_to_todoist-0.4.2.tar", max compression
```

## Comparing `ics_to_todoist-0.4.1.tar` & `ics_to_todoist-0.4.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0     1088 2022-11-14 14:48:23.000000 ics_to_todoist-0.4.1/LICENSE.md
--rwxr-xr-x   0        0        0     1382 2022-12-21 10:42:15.000000 ics_to_todoist-0.4.1/README.md
--rwxr-xr-x   0        0        0        0 2022-11-22 14:00:13.000000 ics_to_todoist-0.4.1/ics_to_todoist/__init__.py
--rwxr-xr-x   0        0        0     4743 2022-12-23 04:34:46.000000 ics_to_todoist-0.4.1/ics_to_todoist/__main__.py
--rwxr-xr-x   0        0        0      106 2022-12-23 03:36:49.000000 ics_to_todoist-0.4.1/ics_to_todoist/models/__init__.py
--rwxr-xr-x   0        0        0     1260 2022-12-04 05:31:00.000000 ics_to_todoist-0.4.1/ics_to_todoist/models/configuration.py
--rwxr-xr-x   0        0        0      235 2022-11-22 14:00:13.000000 ics_to_todoist-0.4.1/ics_to_todoist/models/event.py
--rw-r--r--   0        0        0     1234 2024-01-14 13:32:36.168479 ics_to_todoist-0.4.1/ics_to_todoist/models/reminder_time.py
--rwxr-xr-x   0        0        0     1785 2022-12-23 04:29:42.000000 ics_to_todoist-0.4.1/ics_to_todoist/todoist_helper.py
--rw-r--r--   0        0        0     2307 2024-01-14 13:38:32.538519 ics_to_todoist-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2556 1970-01-01 00:00:00.000000 ics_to_todoist-0.4.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1088 2022-11-14 14:48:23.000000 ics_to_todoist-0.4.2/LICENSE.md
+-rwxr-xr-x   0        0        0     1382 2022-12-21 10:42:15.000000 ics_to_todoist-0.4.2/README.md
+-rwxr-xr-x   0        0        0        0 2022-11-22 14:00:13.000000 ics_to_todoist-0.4.2/ics_to_todoist/__init__.py
+-rwxr-xr-x   0        0        0     4743 2022-12-23 04:34:46.000000 ics_to_todoist-0.4.2/ics_to_todoist/__main__.py
+-rwxr-xr-x   0        0        0      106 2022-12-23 03:36:49.000000 ics_to_todoist-0.4.2/ics_to_todoist/models/__init__.py
+-rwxr-xr-x   0        0        0     1260 2022-12-04 05:31:00.000000 ics_to_todoist-0.4.2/ics_to_todoist/models/configuration.py
+-rwxr-xr-x   0        0        0      235 2022-11-22 14:00:13.000000 ics_to_todoist-0.4.2/ics_to_todoist/models/event.py
+-rwxr-xr-x   0        0        0     1234 2024-01-14 13:32:36.000000 ics_to_todoist-0.4.2/ics_to_todoist/models/reminder_time.py
+-rwxr-xr-x   0        0        0     1785 2022-12-23 04:29:42.000000 ics_to_todoist-0.4.2/ics_to_todoist/todoist_helper.py
+-rwxr-xr-x   0        0        0     2307 2024-05-31 14:54:33.758014 ics_to_todoist-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2556 1970-01-01 00:00:00.000000 ics_to_todoist-0.4.2/PKG-INFO
```

### Comparing `ics_to_todoist-0.4.1/LICENSE.md` & `ics_to_todoist-0.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ics_to_todoist-0.4.1/README.md` & `ics_to_todoist-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ics_to_todoist-0.4.1/ics_to_todoist/__main__.py` & `ics_to_todoist-0.4.2/ics_to_todoist/__main__.py`

 * *Files identical despite different names*

### Comparing `ics_to_todoist-0.4.1/ics_to_todoist/models/configuration.py` & `ics_to_todoist-0.4.2/ics_to_todoist/models/configuration.py`

 * *Files identical despite different names*

### Comparing `ics_to_todoist-0.4.1/ics_to_todoist/models/reminder_time.py` & `ics_to_todoist-0.4.2/ics_to_todoist/models/reminder_time.py`

 * *Files identical despite different names*

### Comparing `ics_to_todoist-0.4.1/ics_to_todoist/todoist_helper.py` & `ics_to_todoist-0.4.2/ics_to_todoist/todoist_helper.py`

 * *Files identical despite different names*

### Comparing `ics_to_todoist-0.4.1/pyproject.toml` & `ics_to_todoist-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ics-to-todoist"
-version = "0.4.1"
+version = "0.4.2"
 description = "A command line tool to convert entries from an .ics file to tasks in Todoist."
 authors = ["Gabor Schulz"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://gaborschulz.github.io/ics-to-todoist/"
 repository = "https://github.com/gaborschulz/ics-to-todoist"
 # documentation = "https://gaborschulz.github.io/ics-to-todoist/"
```

### Comparing `ics_to_todoist-0.4.1/PKG-INFO` & `ics_to_todoist-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ics-to-todoist
-Version: 0.4.1
+Version: 0.4.2
 Summary: A command line tool to convert entries from an .ics file to tasks in Todoist.
 Home-page: https://gaborschulz.github.io/ics-to-todoist/
 License: MIT
 Keywords: ics,todoist
 Author: Gabor Schulz
 Requires-Python: >=3.10,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

