# Comparing `tmp/dagster_looker-0.23.7.tar.gz` & `tmp/dagster_looker-0.23.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_looker-0.23.7.tar", last modified: Thu May 23 20:59:08 2024, max compression
+gzip compressed data, was "dagster_looker-0.23.8.tar", last modified: Thu May 30 22:46:30 2024, max compression
```

## Comparing `dagster_looker-0.23.7.tar` & `dagster_looker-0.23.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:59:08.939180 dagster_looker-0.23.7/
--rw-r--r--   0 root         (0) root         (0)    11347 2024-05-23 20:50:32.000000 dagster_looker-0.23.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       66 2024-05-23 20:50:32.000000 dagster_looker-0.23.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      622 2024-05-23 20:59:08.939180 dagster_looker-0.23.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      129 2024-05-23 20:50:32.000000 dagster_looker-0.23.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:59:08.939180 dagster_looker-0.23.7/dagster_looker/
--rw-r--r--   0 root         (0) root         (0)      379 2024-05-23 20:50:32.000000 dagster_looker-0.23.7/dagster_looker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1366 2024-05-23 20:50:32.000000 dagster_looker-0.23.7/dagster_looker/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     3805 2024-05-23 20:50:32.000000 dagster_looker-0.23.7/dagster_looker/asset_utils.py
--rw-r--r--   0 root         (0) root         (0)    17128 2024-05-23 20:50:32.000000 dagster_looker-0.23.7/dagster_looker/dagster_looker_translator.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-23 20:50:32.000000 dagster_looker-0.23.7/dagster_looker/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-23 20:50:32.000000 dagster_looker-0.23.7/dagster_looker/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:59:08.939180 dagster_looker-0.23.7/dagster_looker.egg-info/
--rw-r--r--   0 root         (0) root         (0)      622 2024-05-23 20:59:08.000000 dagster_looker-0.23.7/dagster_looker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      459 2024-05-23 20:59:08.000000 dagster_looker-0.23.7/dagster_looker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:59:08.000000 dagster_looker-0.23.7/dagster_looker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:59:08.000000 dagster_looker-0.23.7/dagster_looker.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       28 2024-05-23 20:59:08.000000 dagster_looker-0.23.7/dagster_looker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-23 20:59:08.000000 dagster_looker-0.23.7/dagster_looker.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      161 2024-05-23 20:59:08.943180 dagster_looker-0.23.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1299 2024-05-23 20:50:32.000000 dagster_looker-0.23.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:46:30.100729 dagster_looker-0.23.8/
+-rw-r--r--   0 root         (0) root         (0)    11347 2024-05-30 22:41:26.000000 dagster_looker-0.23.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-30 22:41:26.000000 dagster_looker-0.23.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      622 2024-05-30 22:46:30.100729 dagster_looker-0.23.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      129 2024-05-30 22:41:26.000000 dagster_looker-0.23.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:46:30.100729 dagster_looker-0.23.8/dagster_looker/
+-rw-r--r--   0 root         (0) root         (0)      379 2024-05-30 22:41:26.000000 dagster_looker-0.23.8/dagster_looker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1366 2024-05-30 22:41:26.000000 dagster_looker-0.23.8/dagster_looker/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     3805 2024-05-30 22:41:26.000000 dagster_looker-0.23.8/dagster_looker/asset_utils.py
+-rw-r--r--   0 root         (0) root         (0)    17128 2024-05-30 22:41:26.000000 dagster_looker-0.23.8/dagster_looker/dagster_looker_translator.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-30 22:41:26.000000 dagster_looker-0.23.8/dagster_looker/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-30 22:41:26.000000 dagster_looker-0.23.8/dagster_looker/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:46:30.100729 dagster_looker-0.23.8/dagster_looker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      622 2024-05-30 22:46:29.000000 dagster_looker-0.23.8/dagster_looker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      459 2024-05-30 22:46:29.000000 dagster_looker-0.23.8/dagster_looker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 22:46:29.000000 dagster_looker-0.23.8/dagster_looker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 22:46:29.000000 dagster_looker-0.23.8/dagster_looker.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-30 22:46:29.000000 dagster_looker-0.23.8/dagster_looker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-30 22:46:29.000000 dagster_looker-0.23.8/dagster_looker.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2024-05-30 22:46:30.104729 dagster_looker-0.23.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1299 2024-05-30 22:41:26.000000 dagster_looker-0.23.8/setup.py
```

### Comparing `dagster_looker-0.23.7/LICENSE` & `dagster_looker-0.23.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster_looker-0.23.7/PKG-INFO` & `dagster_looker-0.23.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster_looker
-Version: 0.23.7
+Version: 0.23.8
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-looker
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dagster_looker-0.23.7/dagster_looker/asset_decorator.py` & `dagster_looker-0.23.8/dagster_looker/asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster_looker-0.23.7/dagster_looker/asset_utils.py` & `dagster_looker-0.23.8/dagster_looker/asset_utils.py`

 * *Files identical despite different names*

### Comparing `dagster_looker-0.23.7/dagster_looker/dagster_looker_translator.py` & `dagster_looker-0.23.8/dagster_looker/dagster_looker_translator.py`

 * *Files identical despite different names*

### Comparing `dagster_looker-0.23.7/dagster_looker.egg-info/PKG-INFO` & `dagster_looker-0.23.8/dagster_looker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-looker
-Version: 0.23.7
+Version: 0.23.8
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-looker
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dagster_looker-0.23.7/setup.py` & `dagster_looker-0.23.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,13 +33,13 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_looker_tests*"]),
     install_requires=[
-        "dagster==1.7.7",
+        "dagster==1.7.8",
         "lkml",
         "sqlglot",
     ],
     zip_safe=False,
 )
```

