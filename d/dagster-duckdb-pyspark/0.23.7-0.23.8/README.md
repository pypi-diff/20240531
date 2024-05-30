# Comparing `tmp/dagster-duckdb-pyspark-0.23.7.tar.gz` & `tmp/dagster-duckdb-pyspark-0.23.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-pyspark-0.23.7.tar", last modified: Thu May 23 20:56:57 2024, max compression
+gzip compressed data, was "dagster-duckdb-pyspark-0.23.8.tar", last modified: Thu May 30 23:21:04 2024, max compression
```

## Comparing `dagster-duckdb-pyspark-0.23.7.tar` & `dagster-duckdb-pyspark-0.23.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:56:57.176293 dagster-duckdb-pyspark-0.23.7/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-23 20:50:32.000000 dagster-duckdb-pyspark-0.23.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       56 2024-05-23 20:50:32.000000 dagster-duckdb-pyspark-0.23.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      623 2024-05-23 20:56:57.176293 dagster-duckdb-pyspark-0.23.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      152 2024-05-23 20:50:32.000000 dagster-duckdb-pyspark-0.23.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:56:57.176293 dagster-duckdb-pyspark-0.23.7/dagster_duckdb_pyspark/
--rw-r--r--   0 root         (0) root         (0)      382 2024-05-23 20:50:32.000000 dagster-duckdb-pyspark-0.23.7/dagster_duckdb_pyspark/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9588 2024-05-23 20:50:32.000000 dagster-duckdb-pyspark-0.23.7/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-23 20:50:32.000000 dagster-duckdb-pyspark-0.23.7/dagster_duckdb_pyspark/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-23 20:50:32.000000 dagster-duckdb-pyspark-0.23.7/dagster_duckdb_pyspark/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:56:57.176293 dagster-duckdb-pyspark-0.23.7/dagster_duckdb_pyspark.egg-info/
--rw-r--r--   0 root         (0) root         (0)      623 2024-05-23 20:56:57.000000 dagster-duckdb-pyspark-0.23.7/dagster_duckdb_pyspark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      477 2024-05-23 20:56:57.000000 dagster-duckdb-pyspark-0.23.7/dagster_duckdb_pyspark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:56:57.000000 dagster-duckdb-pyspark-0.23.7/dagster_duckdb_pyspark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:56:57.000000 dagster-duckdb-pyspark-0.23.7/dagster_duckdb_pyspark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       64 2024-05-23 20:56:57.000000 dagster-duckdb-pyspark-0.23.7/dagster_duckdb_pyspark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-23 20:56:57.000000 dagster-duckdb-pyspark-0.23.7/dagster_duckdb_pyspark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      133 2024-05-23 20:56:57.176293 dagster-duckdb-pyspark-0.23.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1366 2024-05-23 20:50:32.000000 dagster-duckdb-pyspark-0.23.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:21:04.107190 dagster-duckdb-pyspark-0.23.8/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-30 23:14:09.000000 dagster-duckdb-pyspark-0.23.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       56 2024-05-30 23:14:09.000000 dagster-duckdb-pyspark-0.23.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      623 2024-05-30 23:21:04.107190 dagster-duckdb-pyspark-0.23.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      152 2024-05-30 23:14:09.000000 dagster-duckdb-pyspark-0.23.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:21:04.107190 dagster-duckdb-pyspark-0.23.8/dagster_duckdb_pyspark/
+-rw-r--r--   0 root         (0) root         (0)      382 2024-05-30 23:14:09.000000 dagster-duckdb-pyspark-0.23.8/dagster_duckdb_pyspark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9588 2024-05-30 23:14:09.000000 dagster-duckdb-pyspark-0.23.8/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-30 23:14:09.000000 dagster-duckdb-pyspark-0.23.8/dagster_duckdb_pyspark/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-30 23:14:09.000000 dagster-duckdb-pyspark-0.23.8/dagster_duckdb_pyspark/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:21:04.107190 dagster-duckdb-pyspark-0.23.8/dagster_duckdb_pyspark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      623 2024-05-30 23:21:03.000000 dagster-duckdb-pyspark-0.23.8/dagster_duckdb_pyspark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      477 2024-05-30 23:21:03.000000 dagster-duckdb-pyspark-0.23.8/dagster_duckdb_pyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 23:21:03.000000 dagster-duckdb-pyspark-0.23.8/dagster_duckdb_pyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 23:21:03.000000 dagster-duckdb-pyspark-0.23.8/dagster_duckdb_pyspark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-30 23:21:03.000000 dagster-duckdb-pyspark-0.23.8/dagster_duckdb_pyspark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-30 23:21:03.000000 dagster-duckdb-pyspark-0.23.8/dagster_duckdb_pyspark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      133 2024-05-30 23:21:04.107190 dagster-duckdb-pyspark-0.23.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1366 2024-05-30 23:14:09.000000 dagster-duckdb-pyspark-0.23.8/setup.py
```

### Comparing `dagster-duckdb-pyspark-0.23.7/LICENSE` & `dagster-duckdb-pyspark-0.23.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-pyspark-0.23.7/PKG-INFO` & `dagster-duckdb-pyspark-0.23.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pyspark
-Version: 0.23.7
+Version: 0.23.8
 Summary: Package for storing PySpark DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pyspark
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-pyspark-0.23.7/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py` & `dagster-duckdb-pyspark-0.23.8/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-pyspark-0.23.7/dagster_duckdb_pyspark.egg-info/PKG-INFO` & `dagster-duckdb-pyspark-0.23.8/dagster_duckdb_pyspark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pyspark
-Version: 0.23.7
+Version: 0.23.8
 Summary: Package for storing PySpark DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pyspark
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-pyspark-0.23.7/setup.py` & `dagster-duckdb-pyspark-0.23.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_pyspark_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.7",
-        "dagster-duckdb==0.23.7",
+        "dagster==1.7.8",
+        "dagster-duckdb==0.23.8",
         "pyspark>=3",
         "pandas",
         "pyarrow",
     ],
     zip_safe=False,
 )
```

