# Comparing `tmp/dt_extension_migrator-0.1.4.tar.gz` & `tmp/dt_extension_migrator-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dt_extension_migrator-0.1.4.tar", max compression
+gzip compressed data, was "dt_extension_migrator-0.1.5.tar", max compression
```

## Comparing `dt_extension_migrator-0.1.4.tar` & `dt_extension_migrator-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2024-05-24 16:54:43.631910 dt_extension_migrator-0.1.4/dt_extension_migrator/__init__.py
--rw-r--r--   0        0        0    12520 2024-05-31 14:21:37.719564 dt_extension_migrator-0.1.4/dt_extension_migrator/extension_apps/__pycache__/generic_commands.cpython-312.pyc
--rw-r--r--   0        0        0    12388 2024-05-31 14:21:38.917591 dt_extension_migrator-0.1.4/dt_extension_migrator/extension_apps/__pycache__/remote_logs.cpython-312.pyc
--rw-r--r--   0        0        0    10963 2024-05-31 14:12:54.335124 dt_extension_migrator-0.1.4/dt_extension_migrator/extension_apps/__pycache__/remote_unix.cpython-312.pyc
--rw-r--r--   0        0        0    12750 2024-05-31 14:24:05.451600 dt_extension_migrator-0.1.4/dt_extension_migrator/extension_apps/generic_commands.py
--rw-r--r--   0        0        0    11234 2024-05-31 14:24:06.310591 dt_extension_migrator-0.1.4/dt_extension_migrator/extension_apps/remote_logs.py
--rw-r--r--   0        0        0    10539 2024-05-31 14:24:07.148063 dt_extension_migrator-0.1.4/dt_extension_migrator/extension_apps/remote_unix.py
--rw-r--r--   0        0        0     2324 2024-05-31 14:24:08.331493 dt_extension_migrator-0.1.4/dt_extension_migrator/main.py
--rw-r--r--   0        0        0     2496 2024-05-31 13:01:13.126905 dt_extension_migrator-0.1.4/dt_extension_migrator/remote_unix_utils.py
--rw-r--r--   0        0        0      483 2024-05-31 15:12:50.168545 dt_extension_migrator-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2600 2024-05-30 19:05:07.587694 dt_extension_migrator-0.1.4/README.md
--rw-r--r--   0        0        0     3238 1970-01-01 00:00:00.000000 dt_extension_migrator-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-24 16:54:43.631910 dt_extension_migrator-0.1.5/dt_extension_migrator/__init__.py
+-rw-r--r--   0        0        0    12520 2024-05-31 14:21:37.719564 dt_extension_migrator-0.1.5/dt_extension_migrator/extension_apps/__pycache__/generic_commands.cpython-312.pyc
+-rw-r--r--   0        0        0    12388 2024-05-31 14:21:38.917591 dt_extension_migrator-0.1.5/dt_extension_migrator/extension_apps/__pycache__/remote_logs.cpython-312.pyc
+-rw-r--r--   0        0        0    10963 2024-05-31 14:12:54.335124 dt_extension_migrator-0.1.5/dt_extension_migrator/extension_apps/__pycache__/remote_unix.cpython-312.pyc
+-rw-r--r--   0        0        0    12750 2024-05-31 14:24:05.451600 dt_extension_migrator-0.1.5/dt_extension_migrator/extension_apps/generic_commands.py
+-rw-r--r--   0        0        0    11234 2024-05-31 14:24:06.310591 dt_extension_migrator-0.1.5/dt_extension_migrator/extension_apps/remote_logs.py
+-rw-r--r--   0        0        0    10539 2024-05-31 14:24:07.148063 dt_extension_migrator-0.1.5/dt_extension_migrator/extension_apps/remote_unix.py
+-rw-r--r--   0        0        0     2324 2024-05-31 14:24:08.331493 dt_extension_migrator-0.1.5/dt_extension_migrator/main.py
+-rw-r--r--   0        0        0     2496 2024-05-31 13:01:13.126905 dt_extension_migrator-0.1.5/dt_extension_migrator/remote_unix_utils.py
+-rw-r--r--   0        0        0      507 2024-05-31 15:27:15.603032 dt_extension_migrator-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2600 2024-05-30 19:05:07.587694 dt_extension_migrator-0.1.5/README.md
+-rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 dt_extension_migrator-0.1.5/PKG-INFO
```

### Comparing `dt_extension_migrator-0.1.4/dt_extension_migrator/extension_apps/__pycache__/generic_commands.cpython-312.pyc` & `dt_extension_migrator-0.1.5/dt_extension_migrator/extension_apps/__pycache__/generic_commands.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `dt_extension_migrator-0.1.4/dt_extension_migrator/extension_apps/__pycache__/remote_logs.cpython-312.pyc` & `dt_extension_migrator-0.1.5/dt_extension_migrator/extension_apps/__pycache__/remote_logs.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `dt_extension_migrator-0.1.4/dt_extension_migrator/extension_apps/__pycache__/remote_unix.cpython-312.pyc` & `dt_extension_migrator-0.1.5/dt_extension_migrator/extension_apps/__pycache__/remote_unix.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `dt_extension_migrator-0.1.4/dt_extension_migrator/extension_apps/generic_commands.py` & `dt_extension_migrator-0.1.5/dt_extension_migrator/extension_apps/generic_commands.py`

 * *Files identical despite different names*

### Comparing `dt_extension_migrator-0.1.4/dt_extension_migrator/extension_apps/remote_logs.py` & `dt_extension_migrator-0.1.5/dt_extension_migrator/extension_apps/remote_logs.py`

 * *Files identical despite different names*

### Comparing `dt_extension_migrator-0.1.4/dt_extension_migrator/extension_apps/remote_unix.py` & `dt_extension_migrator-0.1.5/dt_extension_migrator/extension_apps/remote_unix.py`

 * *Files identical despite different names*

### Comparing `dt_extension_migrator-0.1.4/dt_extension_migrator/main.py` & `dt_extension_migrator-0.1.5/dt_extension_migrator/main.py`

 * *Files identical despite different names*

### Comparing `dt_extension_migrator-0.1.4/dt_extension_migrator/remote_unix_utils.py` & `dt_extension_migrator-0.1.5/dt_extension_migrator/remote_unix_utils.py`

 * *Files identical despite different names*

### Comparing `dt_extension_migrator-0.1.4/README.md` & `dt_extension_migrator-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `dt_extension_migrator-0.1.4/PKG-INFO` & `dt_extension_migrator-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: dt-extension-migrator
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Your Name
 Author-email: you@example.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: dt (>=1.1.63,<2.0.0)
 Requires-Dist: mmh3 (>=4.1.0,<5.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: typer[all] (>=0.12.3,<0.13.0)
+Requires-Dist: xlsxwriter (>=3.2.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # Dynatrace Extension Migrator
 
 Helps with moving the configurations of select Extensions 1.0 extensions to their 2.0 equivalents.
 
 ## Requirements
```

