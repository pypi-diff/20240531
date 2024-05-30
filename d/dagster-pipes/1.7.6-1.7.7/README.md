# Comparing `tmp/dagster-pipes-1.7.6.tar.gz` & `tmp/dagster-pipes-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-pipes-1.7.6.tar", last modified: Thu May 16 19:28:05 2024, max compression
+gzip compressed data, was "dagster-pipes-1.7.7.tar", last modified: Thu May 23 20:23:13 2024, max compression
```

## Comparing `dagster-pipes-1.7.6.tar` & `dagster-pipes-1.7.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:05.272140 dagster-pipes-1.7.6/
--rw-r--r--   0 root         (0) root         (0)    11348 2024-05-16 19:27:09.000000 dagster-pipes-1.7.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-16 19:27:09.000000 dagster-pipes-1.7.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      794 2024-05-16 19:28:05.272140 dagster-pipes-1.7.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      125 2024-05-16 19:27:09.000000 dagster-pipes-1.7.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:05.272140 dagster-pipes-1.7.6/dagster_pipes/
--rw-r--r--   0 root         (0) root         (0)    48159 2024-05-16 19:27:09.000000 dagster-pipes-1.7.6/dagster_pipes/__init__.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-16 19:27:09.000000 dagster-pipes-1.7.6/dagster_pipes/py.typed
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-16 19:27:09.000000 dagster-pipes-1.7.6/dagster_pipes/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:05.272140 dagster-pipes-1.7.6/dagster_pipes.egg-info/
--rw-r--r--   0 root         (0) root         (0)      794 2024-05-16 19:28:04.000000 dagster-pipes-1.7.6/dagster_pipes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      306 2024-05-16 19:28:05.000000 dagster-pipes-1.7.6/dagster_pipes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 19:28:04.000000 dagster-pipes-1.7.6/dagster_pipes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 19:28:04.000000 dagster-pipes-1.7.6/dagster_pipes.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       14 2024-05-16 19:28:04.000000 dagster-pipes-1.7.6/dagster_pipes.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      160 2024-05-16 19:28:05.276140 dagster-pipes-1.7.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1313 2024-05-16 19:27:09.000000 dagster-pipes-1.7.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:23:13.228924 dagster-pipes-1.7.7/
+-rw-r--r--   0 root         (0) root         (0)    11348 2024-05-23 20:22:18.000000 dagster-pipes-1.7.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-23 20:22:18.000000 dagster-pipes-1.7.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      794 2024-05-23 20:23:13.228924 dagster-pipes-1.7.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      125 2024-05-23 20:22:18.000000 dagster-pipes-1.7.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:23:13.224924 dagster-pipes-1.7.7/dagster_pipes/
+-rw-r--r--   0 root         (0) root         (0)    48159 2024-05-23 20:22:18.000000 dagster-pipes-1.7.7/dagster_pipes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-23 20:22:18.000000 dagster-pipes-1.7.7/dagster_pipes/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 20:22:18.000000 dagster-pipes-1.7.7/dagster_pipes/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:23:13.224924 dagster-pipes-1.7.7/dagster_pipes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      794 2024-05-23 20:23:13.000000 dagster-pipes-1.7.7/dagster_pipes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      306 2024-05-23 20:23:13.000000 dagster-pipes-1.7.7/dagster_pipes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:23:13.000000 dagster-pipes-1.7.7/dagster_pipes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:23:13.000000 dagster-pipes-1.7.7/dagster_pipes.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-23 20:23:13.000000 dagster-pipes-1.7.7/dagster_pipes.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      160 2024-05-23 20:23:13.228924 dagster-pipes-1.7.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1313 2024-05-23 20:22:18.000000 dagster-pipes-1.7.7/setup.py
```

### Comparing `dagster-pipes-1.7.6/LICENSE` & `dagster-pipes-1.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-pipes-1.7.6/PKG-INFO` & `dagster-pipes-1.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-pipes
-Version: 1.7.6
+Version: 1.7.7
 Summary: Toolkit for Dagster integrations with transform logic outside of Dagster
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-pipes
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-pipes-1.7.6/dagster_pipes/__init__.py` & `dagster-pipes-1.7.7/dagster_pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-pipes-1.7.6/dagster_pipes.egg-info/PKG-INFO` & `dagster-pipes-1.7.7/dagster_pipes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-pipes
-Version: 1.7.6
+Version: 1.7.7
 Summary: Toolkit for Dagster integrations with transform logic outside of Dagster
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-pipes
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-pipes-1.7.6/setup.py` & `dagster-pipes-1.7.7/setup.py`

 * *Files identical despite different names*

