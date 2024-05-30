# Comparing `tmp/dagster-snowflake-pandas-0.23.7.tar.gz` & `tmp/dagster-snowflake-pandas-0.23.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-snowflake-pandas-0.23.7.tar", last modified: Thu May 23 21:00:58 2024, max compression
+gzip compressed data, was "dagster-snowflake-pandas-0.23.8.tar", last modified: Thu May 30 23:19:30 2024, max compression
```

## Comparing `dagster-snowflake-pandas-0.23.7.tar` & `dagster-snowflake-pandas-0.23.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:00:58.618247 dagster-snowflake-pandas-0.23.7/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-23 20:50:32.000000 dagster-snowflake-pandas-0.23.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       76 2024-05-23 20:50:32.000000 dagster-snowflake-pandas-0.23.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      739 2024-05-23 21:00:58.618247 dagster-snowflake-pandas-0.23.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      158 2024-05-23 20:50:32.000000 dagster-snowflake-pandas-0.23.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:00:58.614247 dagster-snowflake-pandas-0.23.7/dagster_snowflake_pandas/
--rw-r--r--   0 root         (0) root         (0)      413 2024-05-23 20:50:32.000000 dagster-snowflake-pandas-0.23.7/dagster_snowflake_pandas/__init__.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-23 20:50:32.000000 dagster-snowflake-pandas-0.23.7/dagster_snowflake_pandas/py.typed
--rw-r--r--   0 root         (0) root         (0)    13246 2024-05-23 20:50:32.000000 dagster-snowflake-pandas-0.23.7/dagster_snowflake_pandas/snowflake_pandas_type_handler.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-23 20:50:32.000000 dagster-snowflake-pandas-0.23.7/dagster_snowflake_pandas/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:00:58.618247 dagster-snowflake-pandas-0.23.7/dagster_snowflake_pandas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      739 2024-05-23 21:00:58.000000 dagster-snowflake-pandas-0.23.7/dagster_snowflake_pandas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2024-05-23 21:00:58.000000 dagster-snowflake-pandas-0.23.7/dagster_snowflake_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 21:00:58.000000 dagster-snowflake-pandas-0.23.7/dagster_snowflake_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 21:00:58.000000 dagster-snowflake-pandas-0.23.7/dagster_snowflake_pandas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      144 2024-05-23 21:00:58.000000 dagster-snowflake-pandas-0.23.7/dagster_snowflake_pandas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-23 21:00:58.000000 dagster-snowflake-pandas-0.23.7/dagster_snowflake_pandas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      171 2024-05-23 21:00:58.618247 dagster-snowflake-pandas-0.23.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1637 2024-05-23 20:50:32.000000 dagster-snowflake-pandas-0.23.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:19:30.611968 dagster-snowflake-pandas-0.23.8/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-30 23:14:10.000000 dagster-snowflake-pandas-0.23.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       76 2024-05-30 23:14:10.000000 dagster-snowflake-pandas-0.23.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      739 2024-05-30 23:19:30.611968 dagster-snowflake-pandas-0.23.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      158 2024-05-30 23:14:10.000000 dagster-snowflake-pandas-0.23.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:19:30.611968 dagster-snowflake-pandas-0.23.8/dagster_snowflake_pandas/
+-rw-r--r--   0 root         (0) root         (0)      413 2024-05-30 23:14:10.000000 dagster-snowflake-pandas-0.23.8/dagster_snowflake_pandas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-30 23:14:10.000000 dagster-snowflake-pandas-0.23.8/dagster_snowflake_pandas/py.typed
+-rw-r--r--   0 root         (0) root         (0)    13246 2024-05-30 23:14:10.000000 dagster-snowflake-pandas-0.23.8/dagster_snowflake_pandas/snowflake_pandas_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-30 23:14:10.000000 dagster-snowflake-pandas-0.23.8/dagster_snowflake_pandas/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:19:30.611968 dagster-snowflake-pandas-0.23.8/dagster_snowflake_pandas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      739 2024-05-30 23:19:30.000000 dagster-snowflake-pandas-0.23.8/dagster_snowflake_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2024-05-30 23:19:30.000000 dagster-snowflake-pandas-0.23.8/dagster_snowflake_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 23:19:30.000000 dagster-snowflake-pandas-0.23.8/dagster_snowflake_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 23:19:30.000000 dagster-snowflake-pandas-0.23.8/dagster_snowflake_pandas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      144 2024-05-30 23:19:30.000000 dagster-snowflake-pandas-0.23.8/dagster_snowflake_pandas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-30 23:19:30.000000 dagster-snowflake-pandas-0.23.8/dagster_snowflake_pandas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      171 2024-05-30 23:19:30.615968 dagster-snowflake-pandas-0.23.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1637 2024-05-30 23:14:10.000000 dagster-snowflake-pandas-0.23.8/setup.py
```

### Comparing `dagster-snowflake-pandas-0.23.7/LICENSE` & `dagster-snowflake-pandas-0.23.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-snowflake-pandas-0.23.7/PKG-INFO` & `dagster-snowflake-pandas-0.23.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-snowflake-pandas
-Version: 0.23.7
+Version: 0.23.8
 Summary: Package for integrating Snowflake and Pandas with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pandas
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-snowflake-pandas-0.23.7/dagster_snowflake_pandas/snowflake_pandas_type_handler.py` & `dagster-snowflake-pandas-0.23.8/dagster_snowflake_pandas/snowflake_pandas_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-snowflake-pandas-0.23.7/dagster_snowflake_pandas.egg-info/PKG-INFO` & `dagster-snowflake-pandas-0.23.8/dagster_snowflake_pandas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-snowflake-pandas
-Version: 0.23.7
+Version: 0.23.8
 Summary: Package for integrating Snowflake and Pandas with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pandas
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-snowflake-pandas-0.23.7/setup.py` & `dagster-snowflake-pandas-0.23.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,16 +32,16 @@
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_snowflake_pandas_tests*"]),
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.7",
-        "dagster-snowflake==0.23.7",
+        "dagster==1.7.8",
+        "dagster-snowflake==0.23.8",
         "pandas",
         "requests",
         "snowflake-connector-python[pandas]>=3.4.0",
         "sqlalchemy!=1.4.42",  # workaround for https://github.com/snowflakedb/snowflake-sqlalchemy/issues/350
         "snowflake-sqlalchemy>=1.2",
     ],
     zip_safe=False,
```

