# Comparing `tmp/dagster-gcp-pyspark-0.23.7.tar.gz` & `tmp/dagster-gcp-pyspark-0.23.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-gcp-pyspark-0.23.7.tar", last modified: Thu May 23 20:58:47 2024, max compression
+gzip compressed data, was "dagster-gcp-pyspark-0.23.8.tar", last modified: Thu May 30 22:12:42 2024, max compression
```

## Comparing `dagster-gcp-pyspark-0.23.7.tar` & `dagster-gcp-pyspark-0.23.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:58:47.807360 dagster-gcp-pyspark-0.23.7/
--rw-r--r--   0 root         (0) root         (0)    11348 2024-05-23 20:50:32.000000 dagster-gcp-pyspark-0.23.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       52 2024-05-23 20:50:32.000000 dagster-gcp-pyspark-0.23.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      635 2024-05-23 20:58:47.807360 dagster-gcp-pyspark-0.23.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      144 2024-05-23 20:50:32.000000 dagster-gcp-pyspark-0.23.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:58:47.807360 dagster-gcp-pyspark-0.23.7/dagster_gcp_pyspark/
--rw-r--r--   0 root         (0) root         (0)      402 2024-05-23 20:50:32.000000 dagster-gcp-pyspark-0.23.7/dagster_gcp_pyspark/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:58:47.807360 dagster-gcp-pyspark-0.23.7/dagster_gcp_pyspark/bigquery/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:50:32.000000 dagster-gcp-pyspark-0.23.7/dagster_gcp_pyspark/bigquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11188 2024-05-23 20:50:32.000000 dagster-gcp-pyspark-0.23.7/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-23 20:50:32.000000 dagster-gcp-pyspark-0.23.7/dagster_gcp_pyspark/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-23 20:50:32.000000 dagster-gcp-pyspark-0.23.7/dagster_gcp_pyspark/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:58:47.807360 dagster-gcp-pyspark-0.23.7/dagster_gcp_pyspark.egg-info/
--rw-r--r--   0 root         (0) root         (0)      635 2024-05-23 20:58:47.000000 dagster-gcp-pyspark-0.23.7/dagster_gcp_pyspark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2024-05-23 20:58:47.000000 dagster-gcp-pyspark-0.23.7/dagster_gcp_pyspark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:58:47.000000 dagster-gcp-pyspark-0.23.7/dagster_gcp_pyspark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:58:47.000000 dagster-gcp-pyspark-0.23.7/dagster_gcp_pyspark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       62 2024-05-23 20:58:47.000000 dagster-gcp-pyspark-0.23.7/dagster_gcp_pyspark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-23 20:58:47.000000 dagster-gcp-pyspark-0.23.7/dagster_gcp_pyspark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      166 2024-05-23 20:58:47.811360 dagster-gcp-pyspark-0.23.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1359 2024-05-23 20:50:32.000000 dagster-gcp-pyspark-0.23.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:12:42.594701 dagster-gcp-pyspark-0.23.8/
+-rw-r--r--   0 root         (0) root         (0)    11348 2024-05-30 22:04:22.000000 dagster-gcp-pyspark-0.23.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-30 22:04:22.000000 dagster-gcp-pyspark-0.23.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      635 2024-05-30 22:12:42.594701 dagster-gcp-pyspark-0.23.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      144 2024-05-30 22:04:22.000000 dagster-gcp-pyspark-0.23.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:12:42.594701 dagster-gcp-pyspark-0.23.8/dagster_gcp_pyspark/
+-rw-r--r--   0 root         (0) root         (0)      402 2024-05-30 22:04:22.000000 dagster-gcp-pyspark-0.23.8/dagster_gcp_pyspark/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:12:42.594701 dagster-gcp-pyspark-0.23.8/dagster_gcp_pyspark/bigquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 22:04:22.000000 dagster-gcp-pyspark-0.23.8/dagster_gcp_pyspark/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11188 2024-05-30 22:04:22.000000 dagster-gcp-pyspark-0.23.8/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-30 22:04:22.000000 dagster-gcp-pyspark-0.23.8/dagster_gcp_pyspark/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-30 22:04:22.000000 dagster-gcp-pyspark-0.23.8/dagster_gcp_pyspark/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:12:42.594701 dagster-gcp-pyspark-0.23.8/dagster_gcp_pyspark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      635 2024-05-30 22:12:42.000000 dagster-gcp-pyspark-0.23.8/dagster_gcp_pyspark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2024-05-30 22:12:42.000000 dagster-gcp-pyspark-0.23.8/dagster_gcp_pyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 22:12:42.000000 dagster-gcp-pyspark-0.23.8/dagster_gcp_pyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 22:12:42.000000 dagster-gcp-pyspark-0.23.8/dagster_gcp_pyspark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       62 2024-05-30 22:12:42.000000 dagster-gcp-pyspark-0.23.8/dagster_gcp_pyspark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-30 22:12:42.000000 dagster-gcp-pyspark-0.23.8/dagster_gcp_pyspark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      166 2024-05-30 22:12:42.598701 dagster-gcp-pyspark-0.23.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1359 2024-05-30 22:04:22.000000 dagster-gcp-pyspark-0.23.8/setup.py
```

### Comparing `dagster-gcp-pyspark-0.23.7/LICENSE` & `dagster-gcp-pyspark-0.23.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-gcp-pyspark-0.23.7/PKG-INFO` & `dagster-gcp-pyspark-0.23.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-gcp-pyspark
-Version: 0.23.7
+Version: 0.23.8
 Summary: Package for storing PySpark DataFrames in GCP
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pyspark
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-gcp-pyspark-0.23.7/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py` & `dagster-gcp-pyspark-0.23.8/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-pyspark-0.23.7/dagster_gcp_pyspark.egg-info/PKG-INFO` & `dagster-gcp-pyspark-0.23.8/dagster_gcp_pyspark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-gcp-pyspark
-Version: 0.23.7
+Version: 0.23.8
 Summary: Package for storing PySpark DataFrames in GCP
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pyspark
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-gcp-pyspark-0.23.7/setup.py` & `dagster-gcp-pyspark-0.23.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,14 @@
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_gcp_pyspark_tests*"]),
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.7",
-        "dagster-gcp==0.23.7",
+        "dagster==1.7.8",
+        "dagster-gcp==0.23.8",
         "pyspark",
     ],
     extras_require={"test": ["pandas-gbq"]},
     zip_safe=False,
 )
```

