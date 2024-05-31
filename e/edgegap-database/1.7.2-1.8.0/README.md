# Comparing `tmp/edgegap_database-1.7.2.tar.gz` & `tmp/edgegap_database-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_database-1.7.2.tar", max compression
+gzip compressed data, was "edgegap_database-1.8.0.tar", max compression
```

## Comparing `edgegap_database-1.7.2.tar` & `edgegap_database-1.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1993 2024-05-08 18:23:12.697847 edgegap_database-1.7.2/LICENSE
--rw-r--r--   0        0        0     2180 2024-05-08 18:23:12.697847 edgegap_database-1.7.2/README.md
--rw-r--r--   0        0        0      467 2024-05-08 18:23:12.697847 edgegap_database-1.7.2/edgegap_database/__init__.py
--rw-r--r--   0        0        0      754 2024-05-08 18:23:12.697847 edgegap_database-1.7.2/edgegap_database/_base.py
--rw-r--r--   0        0        0      580 2024-05-08 18:23:12.697847 edgegap_database-1.7.2/edgegap_database/_configuration.py
--rw-r--r--   0        0        0     1072 2024-05-08 18:23:12.697847 edgegap_database-1.7.2/edgegap_database/_engine.py
--rw-r--r--   0        0        0      796 2024-05-08 18:23:12.697847 edgegap_database-1.7.2/edgegap_database/_factory.py
--rw-r--r--   0        0        0     2252 2024-05-08 18:23:12.697847 edgegap_database-1.7.2/edgegap_database/_operator.py
--rw-r--r--   0        0        0      509 2024-05-08 18:23:12.697847 edgegap_database-1.7.2/edgegap_database/_session.py
--rw-r--r--   0        0        0      327 2024-05-08 18:23:12.697847 edgegap_database-1.7.2/edgegap_database/errors/__init__.py
--rw-r--r--   0        0        0      698 2024-05-08 18:23:12.697847 edgegap_database-1.7.2/edgegap_database/errors/_exceptions.py
--rw-r--r--   0        0        0      484 2024-05-08 18:23:12.697847 edgegap_database-1.7.2/edgegap_database/errors/_factory.py
--rw-r--r--   0        0        0       63 2024-05-08 18:23:12.697847 edgegap_database-1.7.2/edgegap_database/models/__init__.py
--rw-r--r--   0        0        0      271 2024-05-08 18:23:12.697847 edgegap_database-1.7.2/edgegap_database/models/_sqlite.py
--rw-r--r--   0        0        0      766 2024-05-08 18:23:37.732643 edgegap_database-1.7.2/pyproject.toml
--rw-r--r--   0        0        0     2943 1970-01-01 00:00:00.000000 edgegap_database-1.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-31 11:59:59.015154 edgegap_database-1.8.0/LICENSE
+-rw-r--r--   0        0        0     2180 2024-05-31 11:59:59.015154 edgegap_database-1.8.0/README.md
+-rw-r--r--   0        0        0      533 2024-05-31 11:59:59.015154 edgegap_database-1.8.0/edgegap_database/__init__.py
+-rw-r--r--   0        0        0      754 2024-05-31 11:59:59.015154 edgegap_database-1.8.0/edgegap_database/_base.py
+-rw-r--r--   0        0        0      580 2024-05-31 11:59:59.015154 edgegap_database-1.8.0/edgegap_database/_configuration.py
+-rw-r--r--   0        0        0     2206 2024-05-31 11:59:59.015154 edgegap_database-1.8.0/edgegap_database/_engine.py
+-rw-r--r--   0        0        0      796 2024-05-31 11:59:59.015154 edgegap_database-1.8.0/edgegap_database/_factory.py
+-rw-r--r--   0        0        0     2252 2024-05-31 11:59:59.015154 edgegap_database-1.8.0/edgegap_database/_operator.py
+-rw-r--r--   0        0        0     1029 2024-05-31 11:59:59.015154 edgegap_database-1.8.0/edgegap_database/_session.py
+-rw-r--r--   0        0        0      327 2024-05-31 11:59:59.015154 edgegap_database-1.8.0/edgegap_database/errors/__init__.py
+-rw-r--r--   0        0        0      698 2024-05-31 11:59:59.015154 edgegap_database-1.8.0/edgegap_database/errors/_exceptions.py
+-rw-r--r--   0        0        0      484 2024-05-31 11:59:59.015154 edgegap_database-1.8.0/edgegap_database/errors/_factory.py
+-rw-r--r--   0        0        0       63 2024-05-31 11:59:59.015154 edgegap_database-1.8.0/edgegap_database/models/__init__.py
+-rw-r--r--   0        0        0      271 2024-05-31 11:59:59.015154 edgegap_database-1.8.0/edgegap_database/models/_sqlite.py
+-rw-r--r--   0        0        0      766 2024-05-31 12:00:11.995035 edgegap_database-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2994 1970-01-01 00:00:00.000000 edgegap_database-1.8.0/PKG-INFO
```

### Comparing `edgegap_database-1.7.2/LICENSE` & `edgegap_database-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.7.2/README.md` & `edgegap_database-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.7.2/edgegap_database/_base.py` & `edgegap_database-1.8.0/edgegap_database/_base.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.7.2/edgegap_database/_configuration.py` & `edgegap_database-1.8.0/edgegap_database/_configuration.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.7.2/edgegap_database/_factory.py` & `edgegap_database-1.8.0/edgegap_database/_factory.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.7.2/edgegap_database/_operator.py` & `edgegap_database-1.8.0/edgegap_database/_operator.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.7.2/edgegap_database/errors/_exceptions.py` & `edgegap_database-1.8.0/edgegap_database/errors/_exceptions.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.7.2/pyproject.toml` & `edgegap_database-1.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-database"
-version = "1.7.2"
+version = "1.8.0"
 description = "The Edgegap Database library includes various tools and helpers for interacting with Database and Migrations. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 psycopg-c = "^3.1.18"
```

### Comparing `edgegap_database-1.7.2/PKG-INFO` & `edgegap_database-1.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: edgegap-database
-Version: 1.7.2
+Version: 1.8.0
 Summary: The Edgegap Database library includes various tools and helpers for interacting with Database and Migrations. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: alembic (>=1.13.1,<2.0.0)
 Requires-Dist: psycopg-c (>=3.1.18,<4.0.0)
 Requires-Dist: psycopg2 (>=2.9.9,<3.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.29,<3.0.0)
 Requires-Dist: sqlmodel (>=0.0.18,<0.0.19)
 Description-Content-Type: text/markdown
```

