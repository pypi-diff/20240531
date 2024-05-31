# Comparing `tmp/stairlight-0.9.1.tar.gz` & `tmp/stairlight-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stairlight-0.9.1.tar", max compression
+gzip compressed data, was "stairlight-0.9.2.tar", max compression
```

## Comparing `stairlight-0.9.1.tar` & `stairlight-0.9.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1075 2021-10-23 11:41:32.044924 stairlight-0.9.1/LICENSE
--rw-r--r--   0        0        0    13890 2023-11-14 11:44:53.686907 stairlight-0.9.1/README.md
--rw-r--r--   0        0        0     2057 2023-11-14 12:36:45.749052 stairlight-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      364 2023-11-14 12:36:39.627478 stairlight-0.9.1/src/stairlight/__init__.py
--rw-r--r--   0        0        0      130 2023-02-22 17:10:30.825152 stairlight-0.9.1/src/stairlight/__main__.py
--rw-r--r--   0        0        0    10372 2023-07-24 11:54:58.182114 stairlight-0.9.1/src/stairlight/cli.py
--rw-r--r--   0        0        0     8513 2023-10-28 14:52:17.074664 stairlight-0.9.1/src/stairlight/configurator.py
--rw-r--r--   0        0        0    12225 2023-11-07 16:46:04.428004 stairlight-0.9.1/src/stairlight/map.py
--rw-r--r--   0        0        0        0 2022-06-14 11:44:47.716674 stairlight-0.9.1/src/stairlight/py.typed
--rw-r--r--   0        0        0     4724 2023-05-04 05:10:54.618092 stairlight-0.9.1/src/stairlight/query.py
--rw-r--r--   0        0        0        0 2023-10-14 12:40:15.575367 stairlight-0.9.1/src/stairlight/source/__init__.py
--rw-r--r--   0        0        0     6966 2023-09-26 14:09:32.555922 stairlight-0.9.1/src/stairlight/source/config.py
--rw-r--r--   0        0        0     2486 2023-02-22 17:10:30.826604 stairlight-0.9.1/src/stairlight/source/config_key.py
--rw-r--r--   0        0        0     7405 2023-04-30 09:26:10.348398 stairlight-0.9.1/src/stairlight/source/controller.py
--rw-r--r--   0        0        0        0 2022-06-18 04:24:48.115814 stairlight-0.9.1/src/stairlight/source/dbt/__init__.py
--rw-r--r--   0        0        0      880 2023-02-22 17:10:30.827070 stairlight-0.9.1/src/stairlight/source/dbt/config.py
--rw-r--r--   0        0        0     8166 2023-02-22 17:10:30.827317 stairlight-0.9.1/src/stairlight/source/dbt/template.py
--rw-r--r--   0        0        0        0 2023-10-14 12:39:57.398834 stairlight-0.9.1/src/stairlight/source/file/__init__.py
--rw-r--r--   0        0        0      737 2023-02-22 17:10:30.827555 stairlight-0.9.1/src/stairlight/source/file/config.py
--rw-r--r--   0        0        0     2866 2023-02-22 17:10:30.827814 stairlight-0.9.1/src/stairlight/source/file/template.py
--rw-r--r--   0        0        0        0 2022-06-18 04:24:48.117151 stairlight-0.9.1/src/stairlight/source/gcs/__init__.py
--rw-r--r--   0        0        0      755 2023-02-22 17:10:30.828091 stairlight-0.9.1/src/stairlight/source/gcs/config.py
--rw-r--r--   0        0        0      509 2023-02-22 17:10:30.828319 stairlight-0.9.1/src/stairlight/source/gcs/map.py
--rw-r--r--   0        0        0     3391 2023-02-22 17:10:30.828564 stairlight-0.9.1/src/stairlight/source/gcs/template.py
--rw-r--r--   0        0        0        0 2022-06-18 04:24:48.117695 stairlight-0.9.1/src/stairlight/source/redash/__init__.py
--rw-r--r--   0        0        0      827 2023-02-22 17:10:30.828829 stairlight-0.9.1/src/stairlight/source/redash/config.py
--rw-r--r--   0        0        0      179 2023-02-16 13:21:19.912956 stairlight-0.9.1/src/stairlight/source/redash/sql/redash_queries.sql
--rw-r--r--   0        0        0     5410 2023-02-22 17:10:30.829091 stairlight-0.9.1/src/stairlight/source/redash/template.py
--rw-r--r--   0        0        0        0 2022-06-25 05:53:09.840666 stairlight-0.9.1/src/stairlight/source/s3/__init__.py
--rw-r--r--   0        0        0      751 2023-02-22 17:10:30.829330 stairlight-0.9.1/src/stairlight/source/s3/config.py
--rw-r--r--   0        0        0      516 2023-02-22 17:10:30.829558 stairlight-0.9.1/src/stairlight/source/s3/map.py
--rw-r--r--   0        0        0     3840 2023-02-22 17:10:30.829767 stairlight-0.9.1/src/stairlight/source/s3/template.py
--rw-r--r--   0        0        0    10928 2023-11-14 12:34:43.544347 stairlight-0.9.1/src/stairlight/source/template.py
--rw-r--r--   0        0        0    23817 2023-09-26 14:23:00.035352 stairlight-0.9.1/src/stairlight/stairlight.py
--rw-r--r--   0        0        0     1751 2023-02-25 07:28:37.392887 stairlight-0.9.1/src/stairlight/util.py
--rw-r--r--   0        0        0    15245 1970-01-01 00:00:00.000000 stairlight-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2021-10-23 11:41:32.044924 stairlight-0.9.2/LICENSE
+-rw-r--r--   0        0        0    13890 2024-05-31 01:08:39.784613 stairlight-0.9.2/README.md
+-rw-r--r--   0        0        0     2209 2024-05-31 07:15:58.008392 stairlight-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      364 2024-05-31 06:53:55.166745 stairlight-0.9.2/src/stairlight/__init__.py
+-rw-r--r--   0        0        0      130 2023-02-22 17:10:30.825152 stairlight-0.9.2/src/stairlight/__main__.py
+-rw-r--r--   0        0        0    10372 2023-07-24 11:54:58.182114 stairlight-0.9.2/src/stairlight/cli.py
+-rw-r--r--   0        0        0     8513 2024-05-31 01:08:39.786819 stairlight-0.9.2/src/stairlight/configurator.py
+-rw-r--r--   0        0        0    12225 2024-05-31 01:08:39.787193 stairlight-0.9.2/src/stairlight/map.py
+-rw-r--r--   0        0        0        0 2022-06-14 11:44:47.716674 stairlight-0.9.2/src/stairlight/py.typed
+-rw-r--r--   0        0        0     4724 2023-05-04 05:10:54.618092 stairlight-0.9.2/src/stairlight/query.py
+-rw-r--r--   0        0        0        0 2023-10-14 12:40:15.575367 stairlight-0.9.2/src/stairlight/source/__init__.py
+-rw-r--r--   0        0        0     6966 2023-09-26 14:09:32.555922 stairlight-0.9.2/src/stairlight/source/config.py
+-rw-r--r--   0        0        0     2486 2023-02-22 17:10:30.826604 stairlight-0.9.2/src/stairlight/source/config_key.py
+-rw-r--r--   0        0        0     7405 2023-04-30 09:26:10.348398 stairlight-0.9.2/src/stairlight/source/controller.py
+-rw-r--r--   0        0        0        0 2022-06-18 04:24:48.115814 stairlight-0.9.2/src/stairlight/source/dbt/__init__.py
+-rw-r--r--   0        0        0      880 2023-02-22 17:10:30.827070 stairlight-0.9.2/src/stairlight/source/dbt/config.py
+-rw-r--r--   0        0        0     8166 2023-02-22 17:10:30.827317 stairlight-0.9.2/src/stairlight/source/dbt/template.py
+-rw-r--r--   0        0        0        0 2023-10-14 12:39:57.398834 stairlight-0.9.2/src/stairlight/source/file/__init__.py
+-rw-r--r--   0        0        0      737 2023-02-22 17:10:30.827555 stairlight-0.9.2/src/stairlight/source/file/config.py
+-rw-r--r--   0        0        0     2866 2023-02-22 17:10:30.827814 stairlight-0.9.2/src/stairlight/source/file/template.py
+-rw-r--r--   0        0        0        0 2022-06-18 04:24:48.117151 stairlight-0.9.2/src/stairlight/source/gcs/__init__.py
+-rw-r--r--   0        0        0      755 2023-02-22 17:10:30.828091 stairlight-0.9.2/src/stairlight/source/gcs/config.py
+-rw-r--r--   0        0        0      509 2023-02-22 17:10:30.828319 stairlight-0.9.2/src/stairlight/source/gcs/map.py
+-rw-r--r--   0        0        0     3391 2023-02-22 17:10:30.828564 stairlight-0.9.2/src/stairlight/source/gcs/template.py
+-rw-r--r--   0        0        0        0 2022-06-18 04:24:48.117695 stairlight-0.9.2/src/stairlight/source/redash/__init__.py
+-rw-r--r--   0        0        0      827 2023-02-22 17:10:30.828829 stairlight-0.9.2/src/stairlight/source/redash/config.py
+-rw-r--r--   0        0        0      179 2023-02-16 13:21:19.912956 stairlight-0.9.2/src/stairlight/source/redash/sql/redash_queries.sql
+-rw-r--r--   0        0        0     5401 2024-05-31 01:08:39.787483 stairlight-0.9.2/src/stairlight/source/redash/template.py
+-rw-r--r--   0        0        0        0 2022-06-25 05:53:09.840666 stairlight-0.9.2/src/stairlight/source/s3/__init__.py
+-rw-r--r--   0        0        0      751 2023-02-22 17:10:30.829330 stairlight-0.9.2/src/stairlight/source/s3/config.py
+-rw-r--r--   0        0        0      516 2023-02-22 17:10:30.829558 stairlight-0.9.2/src/stairlight/source/s3/map.py
+-rw-r--r--   0        0        0     3840 2023-02-22 17:10:30.829767 stairlight-0.9.2/src/stairlight/source/s3/template.py
+-rw-r--r--   0        0        0    10814 2024-05-31 06:51:58.158331 stairlight-0.9.2/src/stairlight/source/template.py
+-rw-r--r--   0        0        0    23819 2024-05-31 01:08:39.788288 stairlight-0.9.2/src/stairlight/stairlight.py
+-rw-r--r--   0        0        0     1751 2023-02-25 07:28:37.392887 stairlight-0.9.2/src/stairlight/util.py
+-rw-r--r--   0        0        0    15382 1970-01-01 00:00:00.000000 stairlight-0.9.2/PKG-INFO
```

### Comparing `stairlight-0.9.1/LICENSE` & `stairlight-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stairlight-0.9.1/README.md` & `stairlight-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `stairlight-0.9.1/pyproject.toml` & `stairlight-0.9.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 [tool.poetry]
 name = "stairlight"
-version = "0.9.1"
+version = "0.9.2"
 description = "Data lineage tool"
 authors = ["tosh2230 <rev.to12@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "src/stairlight" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
-PyYAML = ">=5.0"
+PyYAML = { version = "!=6.0.0,!=5.4.0,!=5.4.1" }
 Jinja2 = ">=2.10.3"
 
 # For unit tests
 boto3-stubs = {version = ">=1.24.17", extras = ["s3"]}
 
 # optional dependencies
-google-cloud-storage = { version = ">=2.0.0", optional = true }
-psycopg2 = { version = ">=2.9.3", optional = true }
-SQLAlchemy = { version = ">=1.4.31", optional = true }
-dbt-core = { version = ">=1.4", optional = true }
-dbt-bigquery = { version = ">=1.1", optional = true }
-google-cloud-bigquery = { version = ">=2.0", optional = true }
-protobuf = { version = ">=3.20.2", optional = true }
 boto3 = { version = ">=1.24.14", optional = true }
+cmake = { version = ">=3", optional = true }
+dbt-adapters = { version = "~1.1.1", optional = true }
+dbt-bigquery = { version = ">=1.8", optional = true }
+dbt-core = { version = ">=1.8", optional = true }
+google-cloud-bigquery = { version = ">=3.0", optional = true }
+google-cloud-storage = { version = ">=2.0", optional = true }
+protobuf = { version = ">=3.20.2", optional = true }
+psycopg2 = { version = ">=2.9.3", optional = true }
 rsa = { version = ">=4.7", optional = true }
+SQLAlchemy = { version = ">=2.0", optional = true }
 
 # To avoid not in poetry.lock metadata
 networkx = { version = ">=2.3,<2.8.1", optional = true }
 
 [tool.poetry.extras]
+dbt-bigquery = ["cmake", "dbt-adapters", "dbt-core", "dbt-bigquery", "google-cloud-bigquery", "protobuf", "networkx", "rsa"]
 gcs = ["google-cloud-storage", "protobuf", "rsa"]
 redash = ["psycopg2", "SQLAlchemy"]
-dbt-bigquery = ["dbt-core", "dbt-bigquery", "google-cloud-bigquery", "protobuf", "networkx", "rsa"]
 s3 = ["boto3", "boto3-stubs"]
 
 [tool.poetry.dev-dependencies]
 black = ">=22.3.0"
 flake8 = ">=4.0.1"
 isort = ">=5.9.3"
+moto = {extras = ["s3"], version = ">=3.1.16"}
 mypy = ">=0.961"
-types-PyYAML = ">=6.0.8"
 pytest = ">=7.2.0"
 pytest-cov = ">=4.0.0"
 pytest-mock = ">=3.8.1"
-moto = {extras = ["s3"], version = ">=3.1.16"}
+types-PyYAML = ">=6.0.8"
 
 [tool.poetry.scripts]
 stairlight = "src.stairlight.cli:main"
 
 [tool.black]
 line-length = 88
```

### Comparing `stairlight-0.9.1/src/stairlight/cli.py` & `stairlight-0.9.2/src/stairlight/cli.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.9.1/src/stairlight/configurator.py` & `stairlight-0.9.2/src/stairlight/configurator.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.9.1/src/stairlight/map.py` & `stairlight-0.9.2/src/stairlight/map.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.9.1/src/stairlight/query.py` & `stairlight-0.9.2/src/stairlight/query.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.9.1/src/stairlight/source/config.py` & `stairlight-0.9.2/src/stairlight/source/config.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.9.1/src/stairlight/source/config_key.py` & `stairlight-0.9.2/src/stairlight/source/config_key.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.9.1/src/stairlight/source/controller.py` & `stairlight-0.9.2/src/stairlight/source/controller.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.9.1/src/stairlight/source/dbt/config.py` & `stairlight-0.9.2/src/stairlight/source/dbt/config.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.9.1/src/stairlight/source/dbt/template.py` & `stairlight-0.9.2/src/stairlight/source/dbt/template.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.9.1/src/stairlight/source/file/config.py` & `stairlight-0.9.2/src/stairlight/source/file/config.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.9.1/src/stairlight/source/file/template.py` & `stairlight-0.9.2/src/stairlight/source/file/template.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.9.1/src/stairlight/source/gcs/config.py` & `stairlight-0.9.2/src/stairlight/source/gcs/config.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.9.1/src/stairlight/source/gcs/template.py` & `stairlight-0.9.2/src/stairlight/source/gcs/template.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.9.1/src/stairlight/source/redash/config.py` & `stairlight-0.9.2/src/stairlight/source/redash/config.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.9.1/src/stairlight/source/redash/template.py` & `stairlight-0.9.2/src/stairlight/source/redash/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         Returns:
             str: Template string
         """
         return self.query_str
 
     def get_uri(self) -> str:
         """Get uri"""
-        return super().get_uri()
+        return self.uri
 
 
 class RedashTemplateSource(TemplateSource):
     REDASH_QUERIES = "sql/redash_queries.sql"
     WHERE_CLAUSE_TEMPLATES = {
         StairlightConfigKey.Redash.DATA_SOURCE_NAME: "data_sources.name = :data_source",
         StairlightConfigKey.Redash.QUERY_IDS: "queries.id IN :query_ids",
```

### Comparing `stairlight-0.9.1/src/stairlight/source/s3/config.py` & `stairlight-0.9.2/src/stairlight/source/s3/config.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.9.1/src/stairlight/source/s3/map.py` & `stairlight-0.9.2/src/stairlight/source/s3/map.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.9.1/src/stairlight/source/s3/template.py` & `stairlight-0.9.2/src/stairlight/source/s3/template.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.9.1/src/stairlight/source/template.py` & `stairlight-0.9.2/src/stairlight/source/template.py`

 * *Files 5% similar despite different names*

```diff
@@ -192,32 +192,30 @@
         Returns:
             str: rendered query string
         """
         s = StringTemplate(template=template_str)
 
         try:
             rendered_str = s.substitute(params)
-        except KeyError as e:
+        except KeyError:
             logger.warning(
                 (
-                    f"{e.with_traceback}, "
+                    f"Params not found. "
                     f"source_type: {self.source_type}, "
                     f"key: {self.key}",
-                    f"template_str: {template_str}",
                     f"params: {params}",
                 )
             )
             rendered_str = s.safe_substitute(params)
-        except ValueError as e:
+        except ValueError:
             logger.warning(
                 (
-                    f"{e.with_traceback}, "
+                    f"Query rendering failed. "
                     f"source_type: {self.source_type}, "
                     f"key: {self.key}",
-                    f"template_str: {template_str}",
                     f"params: {params}",
                 )
             )
             rendered_str = template_str
         return rendered_str
 
     @staticmethod
```

### Comparing `stairlight-0.9.1/src/stairlight/stairlight.py` & `stairlight-0.9.2/src/stairlight/stairlight.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,17 +501,17 @@
                     if not next_response.get(next_table_name):
                         continue
 
                     search_results[next_table_name]["Templates"] = relative_map[
                         next_table_name
                     ]
                     if next_response[next_table_name][direction.value]:
-                        search_results[next_table_name][
-                            direction.value
-                        ] = next_response[next_table_name][direction.value]
+                        search_results[next_table_name][direction.value] = (
+                            next_response[next_table_name][direction.value]
+                        )
                 else:
                     search_results[table_name]["Templates"].append(template)
 
         response[table_name][direction.value] = search_results
         return response
 
     def search_plain(
```

### Comparing `stairlight-0.9.1/src/stairlight/util.py` & `stairlight-0.9.2/src/stairlight/util.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.9.1/PKG-INFO` & `stairlight-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stairlight
-Version: 0.9.1
+Version: 0.9.2
 Summary: Data lineage tool
 License: MIT
 Author: tosh2230
 Author-email: rev.to12@gmail.com
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,26 +13,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: dbt-bigquery
 Provides-Extra: gcs
 Provides-Extra: redash
 Provides-Extra: s3
 Requires-Dist: Jinja2 (>=2.10.3)
-Requires-Dist: PyYAML (>=5.0)
-Requires-Dist: SQLAlchemy (>=1.4.31) ; extra == "redash"
+Requires-Dist: PyYAML (!=6.0.0,!=5.4.0,!=5.4.1)
+Requires-Dist: SQLAlchemy (>=2.0) ; extra == "redash"
 Requires-Dist: boto3 (>=1.24.14) ; extra == "s3"
 Requires-Dist: boto3-stubs[s3] (>=1.24.17) ; extra == "s3"
-Requires-Dist: dbt-bigquery (>=1.1) ; extra == "dbt-bigquery"
-Requires-Dist: dbt-core (>=1.4) ; extra == "dbt-bigquery"
-Requires-Dist: google-cloud-bigquery (>=2.0) ; extra == "dbt-bigquery"
-Requires-Dist: google-cloud-storage (>=2.0.0) ; extra == "gcs"
+Requires-Dist: cmake (>=3) ; extra == "dbt-bigquery"
+Requires-Dist: dbt-adapters (>=1.1.1,<1.2.0) ; extra == "dbt-bigquery"
+Requires-Dist: dbt-bigquery (>=1.8) ; extra == "dbt-bigquery"
+Requires-Dist: dbt-core (>=1.8) ; extra == "dbt-bigquery"
+Requires-Dist: google-cloud-bigquery (>=3.0) ; extra == "dbt-bigquery"
+Requires-Dist: google-cloud-storage (>=2.0) ; extra == "gcs"
 Requires-Dist: networkx (>=2.3,<2.8.1) ; extra == "dbt-bigquery"
-Requires-Dist: protobuf (>=3.20.2) ; extra == "gcs" or extra == "dbt-bigquery"
+Requires-Dist: protobuf (>=3.20.2) ; extra == "dbt-bigquery" or extra == "gcs"
 Requires-Dist: psycopg2 (>=2.9.3) ; extra == "redash"
-Requires-Dist: rsa (>=4.7) ; extra == "gcs" or extra == "dbt-bigquery"
+Requires-Dist: rsa (>=4.7) ; extra == "dbt-bigquery" or extra == "gcs"
 Description-Content-Type: text/markdown
 
 <div align="center">
   <img src="https://raw.githubusercontent.com/tosh2230/stairlight/main/img/stairlight_white.png" width="400" alt="Stairlight">
 </div>
 
 -----------------
```

