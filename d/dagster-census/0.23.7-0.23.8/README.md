# Comparing `tmp/dagster-census-0.23.7.tar.gz` & `tmp/dagster-census-0.23.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-census-0.23.7.tar", last modified: Thu May 23 20:55:58 2024, max compression
+gzip compressed data, was "dagster-census-0.23.8.tar", last modified: Thu May 30 22:11:07 2024, max compression
```

## Comparing `dagster-census-0.23.7.tar` & `dagster-census-0.23.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:55:58.928811 dagster-census-0.23.7/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-23 20:50:32.000000 dagster-census-0.23.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       34 2024-05-23 20:50:32.000000 dagster-census-0.23.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      705 2024-05-23 20:55:58.928811 dagster-census-0.23.7/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:55:58.924811 dagster-census-0.23.7/dagster_census/
--rw-r--r--   0 root         (0) root         (0)      394 2024-05-23 20:50:32.000000 dagster-census-0.23.7/dagster_census/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3551 2024-05-23 20:50:32.000000 dagster-census-0.23.7/dagster_census/ops.py
--rw-r--r--   0 root         (0) root         (0)    10798 2024-05-23 20:50:32.000000 dagster-census-0.23.7/dagster_census/resources.py
--rw-r--r--   0 root         (0) root         (0)      677 2024-05-23 20:50:32.000000 dagster-census-0.23.7/dagster_census/types.py
--rw-r--r--   0 root         (0) root         (0)     1325 2024-05-23 20:50:32.000000 dagster-census-0.23.7/dagster_census/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-23 20:50:32.000000 dagster-census-0.23.7/dagster_census/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:55:58.928811 dagster-census-0.23.7/dagster_census.egg-info/
--rw-r--r--   0 root         (0) root         (0)      705 2024-05-23 20:55:58.000000 dagster-census-0.23.7/dagster_census.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      415 2024-05-23 20:55:58.000000 dagster-census-0.23.7/dagster_census.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:55:58.000000 dagster-census-0.23.7/dagster_census.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:55:58.000000 dagster-census-0.23.7/dagster_census.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-23 20:55:58.000000 dagster-census-0.23.7/dagster_census.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-23 20:55:58.000000 dagster-census-0.23.7/dagster_census.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      161 2024-05-23 20:55:58.928811 dagster-census-0.23.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1291 2024-05-23 20:50:32.000000 dagster-census-0.23.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:11:07.459520 dagster-census-0.23.8/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-30 22:04:22.000000 dagster-census-0.23.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       34 2024-05-30 22:04:22.000000 dagster-census-0.23.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      705 2024-05-30 22:11:07.459520 dagster-census-0.23.8/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:11:07.455520 dagster-census-0.23.8/dagster_census/
+-rw-r--r--   0 root         (0) root         (0)      394 2024-05-30 22:04:22.000000 dagster-census-0.23.8/dagster_census/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3551 2024-05-30 22:04:22.000000 dagster-census-0.23.8/dagster_census/ops.py
+-rw-r--r--   0 root         (0) root         (0)    10798 2024-05-30 22:04:22.000000 dagster-census-0.23.8/dagster_census/resources.py
+-rw-r--r--   0 root         (0) root         (0)      677 2024-05-30 22:04:22.000000 dagster-census-0.23.8/dagster_census/types.py
+-rw-r--r--   0 root         (0) root         (0)     1325 2024-05-30 22:04:22.000000 dagster-census-0.23.8/dagster_census/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-30 22:04:22.000000 dagster-census-0.23.8/dagster_census/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:11:07.459520 dagster-census-0.23.8/dagster_census.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      705 2024-05-30 22:11:07.000000 dagster-census-0.23.8/dagster_census.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      415 2024-05-30 22:11:07.000000 dagster-census-0.23.8/dagster_census.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 22:11:07.000000 dagster-census-0.23.8/dagster_census.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 22:11:07.000000 dagster-census-0.23.8/dagster_census.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-30 22:11:07.000000 dagster-census-0.23.8/dagster_census.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-30 22:11:07.000000 dagster-census-0.23.8/dagster_census.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2024-05-30 22:11:07.459520 dagster-census-0.23.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1291 2024-05-30 22:04:22.000000 dagster-census-0.23.8/setup.py
```

### Comparing `dagster-census-0.23.7/LICENSE` & `dagster-census-0.23.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-census-0.23.7/PKG-INFO` & `dagster-census-0.23.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-census
-Version: 0.23.7
+Version: 0.23.8
 Summary: Package for integrating Census with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-census
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-census-0.23.7/dagster_census/ops.py` & `dagster-census-0.23.8/dagster_census/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-census-0.23.7/dagster_census/resources.py` & `dagster-census-0.23.8/dagster_census/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-census-0.23.7/dagster_census/types.py` & `dagster-census-0.23.8/dagster_census/types.py`

 * *Files identical despite different names*

### Comparing `dagster-census-0.23.7/dagster_census/utils.py` & `dagster-census-0.23.8/dagster_census/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-census-0.23.7/dagster_census.egg-info/PKG-INFO` & `dagster-census-0.23.8/dagster_census.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-census
-Version: 0.23.7
+Version: 0.23.8
 Summary: Package for integrating Census with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-census
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-census-0.23.7/setup.py` & `dagster-census-0.23.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,10 +30,10 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_census_tests*"]),
     python_requires=">=3.8,<3.13",
-    install_requires=["dagster==1.7.7"],
+    install_requires=["dagster==1.7.8"],
     zip_safe=False,
 )
```

