# Comparing `tmp/dagster-msteams-0.23.7.tar.gz` & `tmp/dagster-msteams-0.23.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-msteams-0.23.7.tar", last modified: Thu May 23 20:57:17 2024, max compression
+gzip compressed data, was "dagster-msteams-0.23.8.tar", last modified: Thu May 30 22:12:46 2024, max compression
```

## Comparing `dagster-msteams-0.23.7.tar` & `dagster-msteams-0.23.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:57:17.900118 dagster-msteams-0.23.7/
--rw-r--r--   0 root         (0) root         (0)    11348 2024-05-23 20:50:32.000000 dagster-msteams-0.23.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       66 2024-05-23 20:50:32.000000 dagster-msteams-0.23.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      727 2024-05-23 20:57:17.900118 dagster-msteams-0.23.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2024-05-23 20:50:32.000000 dagster-msteams-0.23.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:57:17.900118 dagster-msteams-0.23.7/dagster_msteams/
--rw-r--r--   0 root         (0) root         (0)      510 2024-05-23 20:50:32.000000 dagster-msteams-0.23.7/dagster_msteams/__init__.py
--rw-r--r--   0 root         (0) root         (0)      849 2024-05-23 20:50:32.000000 dagster-msteams-0.23.7/dagster_msteams/card.py
--rw-r--r--   0 root         (0) root         (0)     1389 2024-05-23 20:50:32.000000 dagster-msteams-0.23.7/dagster_msteams/client.py
--rw-r--r--   0 root         (0) root         (0)     5109 2024-05-23 20:50:32.000000 dagster-msteams-0.23.7/dagster_msteams/hooks.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-23 20:50:32.000000 dagster-msteams-0.23.7/dagster_msteams/py.typed
--rw-r--r--   0 root         (0) root         (0)     3778 2024-05-23 20:50:32.000000 dagster-msteams-0.23.7/dagster_msteams/resources.py
--rw-r--r--   0 root         (0) root         (0)     6264 2024-05-23 20:50:32.000000 dagster-msteams-0.23.7/dagster_msteams/sensors.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-23 20:50:32.000000 dagster-msteams-0.23.7/dagster_msteams/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:57:17.900118 dagster-msteams-0.23.7/dagster_msteams.egg-info/
--rw-r--r--   0 root         (0) root         (0)      727 2024-05-23 20:57:17.000000 dagster-msteams-0.23.7/dagster_msteams.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      491 2024-05-23 20:57:17.000000 dagster-msteams-0.23.7/dagster_msteams.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:57:17.000000 dagster-msteams-0.23.7/dagster_msteams.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:57:17.000000 dagster-msteams-0.23.7/dagster_msteams.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       30 2024-05-23 20:57:17.000000 dagster-msteams-0.23.7/dagster_msteams.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-23 20:57:17.000000 dagster-msteams-0.23.7/dagster_msteams.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2024-05-23 20:57:17.900118 dagster-msteams-0.23.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1335 2024-05-23 20:50:32.000000 dagster-msteams-0.23.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:12:46.542666 dagster-msteams-0.23.8/
+-rw-r--r--   0 root         (0) root         (0)    11348 2024-05-30 22:04:22.000000 dagster-msteams-0.23.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-30 22:04:22.000000 dagster-msteams-0.23.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      727 2024-05-30 22:12:46.542666 dagster-msteams-0.23.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2024-05-30 22:04:22.000000 dagster-msteams-0.23.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:12:46.542666 dagster-msteams-0.23.8/dagster_msteams/
+-rw-r--r--   0 root         (0) root         (0)      510 2024-05-30 22:04:22.000000 dagster-msteams-0.23.8/dagster_msteams/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      849 2024-05-30 22:04:22.000000 dagster-msteams-0.23.8/dagster_msteams/card.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2024-05-30 22:04:22.000000 dagster-msteams-0.23.8/dagster_msteams/client.py
+-rw-r--r--   0 root         (0) root         (0)     5109 2024-05-30 22:04:22.000000 dagster-msteams-0.23.8/dagster_msteams/hooks.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-30 22:04:22.000000 dagster-msteams-0.23.8/dagster_msteams/py.typed
+-rw-r--r--   0 root         (0) root         (0)     3778 2024-05-30 22:04:22.000000 dagster-msteams-0.23.8/dagster_msteams/resources.py
+-rw-r--r--   0 root         (0) root         (0)     6264 2024-05-30 22:04:22.000000 dagster-msteams-0.23.8/dagster_msteams/sensors.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-30 22:04:22.000000 dagster-msteams-0.23.8/dagster_msteams/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:12:46.542666 dagster-msteams-0.23.8/dagster_msteams.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      727 2024-05-30 22:12:46.000000 dagster-msteams-0.23.8/dagster_msteams.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      491 2024-05-30 22:12:46.000000 dagster-msteams-0.23.8/dagster_msteams.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 22:12:46.000000 dagster-msteams-0.23.8/dagster_msteams.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 22:12:46.000000 dagster-msteams-0.23.8/dagster_msteams.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-30 22:12:46.000000 dagster-msteams-0.23.8/dagster_msteams.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-30 22:12:46.000000 dagster-msteams-0.23.8/dagster_msteams.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2024-05-30 22:12:46.546666 dagster-msteams-0.23.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1335 2024-05-30 22:04:22.000000 dagster-msteams-0.23.8/setup.py
```

### Comparing `dagster-msteams-0.23.7/LICENSE` & `dagster-msteams-0.23.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.23.7/PKG-INFO` & `dagster-msteams-0.23.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-msteams
-Version: 0.23.7
+Version: 0.23.8
 Summary: A Microsoft Teams client resource for posting to Microsoft Teams
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-msteams
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-msteams-0.23.7/dagster_msteams/card.py` & `dagster-msteams-0.23.8/dagster_msteams/card.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.23.7/dagster_msteams/client.py` & `dagster-msteams-0.23.8/dagster_msteams/client.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.23.7/dagster_msteams/hooks.py` & `dagster-msteams-0.23.8/dagster_msteams/hooks.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.23.7/dagster_msteams/resources.py` & `dagster-msteams-0.23.8/dagster_msteams/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.23.7/dagster_msteams/sensors.py` & `dagster-msteams-0.23.8/dagster_msteams/sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.23.7/dagster_msteams.egg-info/PKG-INFO` & `dagster-msteams-0.23.8/dagster_msteams.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-msteams
-Version: 0.23.7
+Version: 0.23.8
 Summary: A Microsoft Teams client resource for posting to Microsoft Teams
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-msteams
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-msteams-0.23.7/setup.py` & `dagster-msteams-0.23.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,12 +32,12 @@
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_msteams_tests*"]),
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.7",
+        "dagster==1.7.8",
         "requests>=2,<3",
     ],
     zip_safe=False,
 )
```

