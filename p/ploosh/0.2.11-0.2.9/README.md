# Comparing `tmp/ploosh-0.2.11.tar.gz` & `tmp/ploosh-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ploosh-0.2.11.tar", last modified: Mon Apr 29 16:33:53 2024, max compression
+gzip compressed data, was "ploosh-0.2.9.tar", last modified: Wed Apr 17 21:25:11 2024, max compression
```

## Comparing `ploosh-0.2.11.tar` & `ploosh-0.2.9.tar`

### file list

```diff
@@ -1,43 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:33:53.175996 ploosh-0.2.11/
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-29 16:33:53.175996 ploosh-0.2.11/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:33:53.171996 ploosh-0.2.11/ploosh/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:33:53.171996 ploosh-0.2.11/ploosh/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/connectors/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/connectors/connector_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/connectors/connector_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/connectors/connector_csv_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/connectors/connector_databricks.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/connectors/connector_delta_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/connectors/connector_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/connectors/connector_empty_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/connectors/connector_mssql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/connectors/connector_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/connectors/connector_odbc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/connectors/connector_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/connectors/connector_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/connectors/connector_sql_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/execute.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:33:53.175996 ploosh-0.2.11/ploosh/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/exporters/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/exporters/exporter_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/exporters/exporter_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/exporters/exporter_trx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-29 16:33:05.000000 ploosh-0.2.11/ploosh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:33:53.171996 ploosh-0.2.11/ploosh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-29 16:33:53.000000 ploosh-0.2.11/ploosh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-29 16:33:53.000000 ploosh-0.2.11/ploosh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:33:53.000000 ploosh-0.2.11/ploosh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-29 16:33:53.000000 ploosh-0.2.11/ploosh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-29 16:33:53.000000 ploosh-0.2.11/ploosh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 16:33:53.000000 ploosh-0.2.11/ploosh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-29 16:33:05.000000 ploosh-0.2.11/setup-full.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 16:33:53.175996 ploosh-0.2.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-29 16:33:05.000000 ploosh-0.2.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:25:11.837555 ploosh-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-17 21:25:11.837555 ploosh-0.2.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:25:11.833555 ploosh-0.2.9/ploosh/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:25:11.833555 ploosh-0.2.9/ploosh/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector_csv_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector_databricks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector_delta_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector_empty_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector_mssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector_sql_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/execute.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:25:11.837555 ploosh-0.2.9/ploosh/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/exporters/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/exporters/exporter_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/exporters/exporter_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/exporters/exporter_trx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:25:11.833555 ploosh-0.2.9/ploosh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-17 21:25:11.000000 ploosh-0.2.9/ploosh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-17 21:25:11.000000 ploosh-0.2.9/ploosh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 21:25:11.000000 ploosh-0.2.9/ploosh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 21:25:11.000000 ploosh-0.2.9/ploosh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-17 21:25:11.000000 ploosh-0.2.9/ploosh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 21:25:11.000000 ploosh-0.2.9/ploosh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-17 21:24:21.000000 ploosh-0.2.9/setup-full.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 21:25:11.837555 ploosh-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-17 21:24:21.000000 ploosh-0.2.9/setup.py
```

### Comparing `ploosh-0.2.11/PKG-INFO` & `ploosh-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ploosh
-Version: 0.2.11
+Version: 0.2.9
 Summary: A framework to automatize your tests for data projects
 Home-page: https://github.com/CSharplie/ploosh/
 Download-URL: https://pypi.org/project/ploosh/
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/CSharplie/ploosh/issues
 Project-URL: CI, https://github.com/CSharplie/ploosh/actions
 Project-URL: Documentation, https://github.com/CSharplie/ploosh
@@ -17,15 +17,15 @@
 
 Ploosh is yaml based framework used to automatized the testing process in data projects. 
 
 # Get started
 Go to the [ploosh wiki](https://github.com/CSharplie/ploosh/wiki) to find the get started tutorial.
 
 ## Steps
-1. Install ploosh package
+1. Install PyJeb package
 2. Run tests
 3. Analyse results
 
 ## Install Ploosh
 
 Install from [PyPi](https://pypi.org/project/ploosh/) package manager:
 ``` shell
```

### Comparing `ploosh-0.2.11/ploosh/__init__.py` & `ploosh-0.2.9/ploosh/__init__.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.2.11/ploosh/case.py` & `ploosh-0.2.9/ploosh/case.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.2.11/ploosh/configuration.py` & `ploosh-0.2.9/ploosh/configuration.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.2.11/ploosh/connectors/__init__.py` & `ploosh-0.2.9/ploosh/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.2.11/ploosh/connectors/connector_bigquery.py` & `ploosh-0.2.9/ploosh/connectors/connector_bigquery.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.2.11/ploosh/connectors/connector_csv.py` & `ploosh-0.2.9/ploosh/connectors/connector_csv.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.2.11/ploosh/connectors/connector_csv_spark.py` & `ploosh-0.2.9/ploosh/connectors/connector_csv_spark.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.2.11/ploosh/connectors/connector_databricks.py` & `ploosh-0.2.9/ploosh/connectors/connector_databricks.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.2.11/ploosh/connectors/connector_delta_spark.py` & `ploosh-0.2.9/ploosh/connectors/connector_delta_spark.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.2.11/ploosh/connectors/connector_empty_spark.py` & `ploosh-0.2.9/ploosh/connectors/connector_empty_spark.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.2.11/ploosh/connectors/connector_mssql.py` & `ploosh-0.2.9/ploosh/connectors/connector_mssql.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.2.11/ploosh/connectors/connector_mysql.py` & `ploosh-0.2.9/ploosh/connectors/connector_mysql.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.2.11/ploosh/connectors/connector_postgresql.py` & `ploosh-0.2.9/ploosh/connectors/connector_postgresql.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.2.11/ploosh/connectors/connector_snowflake.py` & `ploosh-0.2.9/ploosh/connectors/connector_snowflake.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.2.11/ploosh/connectors/connector_sql_spark.py` & `ploosh-0.2.9/ploosh/connectors/connector_sql_spark.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.2.11/ploosh/execute.py` & `ploosh-0.2.9/ploosh/execute.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.2.11/ploosh/exporters/__init__.py` & `ploosh-0.2.9/ploosh/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.2.11/ploosh/exporters/exporter_csv.py` & `ploosh-0.2.9/ploosh/exporters/exporter_csv.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.2.11/ploosh/exporters/exporter_json.py` & `ploosh-0.2.9/ploosh/exporters/exporter_json.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.2.11/ploosh/exporters/exporter_trx.py` & `ploosh-0.2.9/ploosh/exporters/exporter_trx.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.2.11/ploosh/logs.py` & `ploosh-0.2.9/ploosh/logs.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.2.11/ploosh/parameters.py` & `ploosh-0.2.9/ploosh/parameters.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.2.11/ploosh.egg-info/PKG-INFO` & `ploosh-0.2.9/ploosh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ploosh
-Version: 0.2.11
+Version: 0.2.9
 Summary: A framework to automatize your tests for data projects
 Home-page: https://github.com/CSharplie/ploosh/
 Download-URL: https://pypi.org/project/ploosh/
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/CSharplie/ploosh/issues
 Project-URL: CI, https://github.com/CSharplie/ploosh/actions
 Project-URL: Documentation, https://github.com/CSharplie/ploosh
@@ -17,15 +17,15 @@
 
 Ploosh is yaml based framework used to automatized the testing process in data projects. 
 
 # Get started
 Go to the [ploosh wiki](https://github.com/CSharplie/ploosh/wiki) to find the get started tutorial.
 
 ## Steps
-1. Install ploosh package
+1. Install PyJeb package
 2. Run tests
 3. Analyse results
 
 ## Install Ploosh
 
 Install from [PyPi](https://pypi.org/project/ploosh/) package manager:
 ``` shell
```

### Comparing `ploosh-0.2.11/ploosh.egg-info/SOURCES.txt` & `ploosh-0.2.9/ploosh.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 ploosh/connectors/connector_csv_spark.py
 ploosh/connectors/connector_databricks.py
 ploosh/connectors/connector_delta_spark.py
 ploosh/connectors/connector_empty.py
 ploosh/connectors/connector_empty_spark.py
 ploosh/connectors/connector_mssql.py
 ploosh/connectors/connector_mysql.py
-ploosh/connectors/connector_odbc.py
 ploosh/connectors/connector_postgresql.py
 ploosh/connectors/connector_snowflake.py
 ploosh/connectors/connector_sql_spark.py
 ploosh/exporters/__init__.py
 ploosh/exporters/exporter.py
 ploosh/exporters/exporter_csv.py
 ploosh/exporters/exporter_json.py
```

### Comparing `ploosh-0.2.11/setup.py` & `ploosh-0.2.9/setup.py`

 * *Files identical despite different names*

