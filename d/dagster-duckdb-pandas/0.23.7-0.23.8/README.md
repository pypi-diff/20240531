# Comparing `tmp/dagster-duckdb-pandas-0.23.7.tar.gz` & `tmp/dagster-duckdb-pandas-0.23.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-pandas-0.23.7.tar", last modified: Thu May 23 20:55:47 2024, max compression
+gzip compressed data, was "dagster-duckdb-pandas-0.23.8.tar", last modified: Thu May 30 22:13:19 2024, max compression
```

## Comparing `dagster-duckdb-pandas-0.23.7.tar` & `dagster-duckdb-pandas-0.23.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:55:47.164910 dagster-duckdb-pandas-0.23.7/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-23 20:50:32.000000 dagster-duckdb-pandas-0.23.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       55 2024-05-23 20:50:32.000000 dagster-duckdb-pandas-0.23.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      671 2024-05-23 20:55:47.164910 dagster-duckdb-pandas-0.23.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      142 2024-05-23 20:50:32.000000 dagster-duckdb-pandas-0.23.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:55:47.160910 dagster-duckdb-pandas-0.23.7/dagster_duckdb_pandas/
--rw-r--r--   0 root         (0) root         (0)      374 2024-05-23 20:50:32.000000 dagster-duckdb-pandas-0.23.7/dagster_duckdb_pandas/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9099 2024-05-23 20:50:32.000000 dagster-duckdb-pandas-0.23.7/dagster_duckdb_pandas/duckdb_pandas_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-23 20:50:32.000000 dagster-duckdb-pandas-0.23.7/dagster_duckdb_pandas/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-23 20:50:32.000000 dagster-duckdb-pandas-0.23.7/dagster_duckdb_pandas/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:55:47.164910 dagster-duckdb-pandas-0.23.7/dagster_duckdb_pandas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      671 2024-05-23 20:55:47.000000 dagster-duckdb-pandas-0.23.7/dagster_duckdb_pandas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      466 2024-05-23 20:55:47.000000 dagster-duckdb-pandas-0.23.7/dagster_duckdb_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:55:47.000000 dagster-duckdb-pandas-0.23.7/dagster_duckdb_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:55:47.000000 dagster-duckdb-pandas-0.23.7/dagster_duckdb_pandas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       45 2024-05-23 20:55:47.000000 dagster-duckdb-pandas-0.23.7/dagster_duckdb_pandas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 20:55:47.000000 dagster-duckdb-pandas-0.23.7/dagster_duckdb_pandas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      132 2024-05-23 20:55:47.164910 dagster-duckdb-pandas-0.23.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1370 2024-05-23 20:50:32.000000 dagster-duckdb-pandas-0.23.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:13:19.462380 dagster-duckdb-pandas-0.23.8/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-30 22:04:22.000000 dagster-duckdb-pandas-0.23.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       55 2024-05-30 22:04:22.000000 dagster-duckdb-pandas-0.23.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      671 2024-05-30 22:13:19.462380 dagster-duckdb-pandas-0.23.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      142 2024-05-30 22:04:22.000000 dagster-duckdb-pandas-0.23.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:13:19.462380 dagster-duckdb-pandas-0.23.8/dagster_duckdb_pandas/
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-30 22:04:22.000000 dagster-duckdb-pandas-0.23.8/dagster_duckdb_pandas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9099 2024-05-30 22:04:22.000000 dagster-duckdb-pandas-0.23.8/dagster_duckdb_pandas/duckdb_pandas_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-30 22:04:22.000000 dagster-duckdb-pandas-0.23.8/dagster_duckdb_pandas/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-30 22:04:22.000000 dagster-duckdb-pandas-0.23.8/dagster_duckdb_pandas/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:13:19.462380 dagster-duckdb-pandas-0.23.8/dagster_duckdb_pandas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      671 2024-05-30 22:13:19.000000 dagster-duckdb-pandas-0.23.8/dagster_duckdb_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      466 2024-05-30 22:13:19.000000 dagster-duckdb-pandas-0.23.8/dagster_duckdb_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 22:13:19.000000 dagster-duckdb-pandas-0.23.8/dagster_duckdb_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 22:13:19.000000 dagster-duckdb-pandas-0.23.8/dagster_duckdb_pandas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       45 2024-05-30 22:13:19.000000 dagster-duckdb-pandas-0.23.8/dagster_duckdb_pandas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-30 22:13:19.000000 dagster-duckdb-pandas-0.23.8/dagster_duckdb_pandas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2024-05-30 22:13:19.462380 dagster-duckdb-pandas-0.23.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1370 2024-05-30 22:04:22.000000 dagster-duckdb-pandas-0.23.8/setup.py
```

### Comparing `dagster-duckdb-pandas-0.23.7/LICENSE` & `dagster-duckdb-pandas-0.23.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-pandas-0.23.7/PKG-INFO` & `dagster-duckdb-pandas-0.23.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pandas
-Version: 0.23.7
+Version: 0.23.8
 Summary: Package for storing Pandas DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pandas
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-pandas-0.23.7/dagster_duckdb_pandas/duckdb_pandas_type_handler.py` & `dagster-duckdb-pandas-0.23.8/dagster_duckdb_pandas/duckdb_pandas_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-pandas-0.23.7/dagster_duckdb_pandas.egg-info/PKG-INFO` & `dagster-duckdb-pandas-0.23.8/dagster_duckdb_pandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pandas
-Version: 0.23.7
+Version: 0.23.8
 Summary: Package for storing Pandas DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pandas
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-pandas-0.23.7/setup.py` & `dagster-duckdb-pandas-0.23.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,13 +31,13 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_pandas_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.7",
-        "dagster-duckdb==0.23.7",
+        "dagster==1.7.8",
+        "dagster-duckdb==0.23.8",
         "pandas",
     ],
     zip_safe=False,
 )
```

