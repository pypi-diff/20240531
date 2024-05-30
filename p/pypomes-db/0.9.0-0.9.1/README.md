# Comparing `tmp/pypomes_db-0.9.0.tar.gz` & `tmp/pypomes_db-0.9.1.tar.gz`

## Comparing `pypomes_db-0.9.0.tar` & `pypomes_db-0.9.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    12370 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    40499 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    18539 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/src/pypomes_db/migration_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    17654 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    16534 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    12370 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    40499 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    18539 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/src/pypomes_db/migration_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    17654 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    16534 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/PKG-INFO
```

### Comparing `pypomes_db-0.9.0/src/pypomes_db/__init__.py` & `pypomes_db-0.9.1/src/pypomes_db/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from .db_pomes import (
-    db_setup, db_get_engines, db_get_params,
+    db_setup, db_get_engines,  db_get_param, db_get_params,
     db_assert_connection, db_connect,
     db_exists, db_select_one, db_select_all,
     db_insert, db_update, db_delete,
     db_bulk_insert, db_bulk_update, db_update_lob,
     db_execute, db_call_function, db_call_procedure,
 )
 from .migration_pomes import (
     db_migrate_data, db_migrate_lobs,
 )
 
 __all__ = [
     # db_pomes
-    "db_setup", "db_get_engines", "db_get_params",
+    "db_setup", "db_get_engines", "db_get_param", "db_get_params",
     "db_assert_connection", "db_connect",
     "db_exists", "db_select_one", "db_select_all",
     "db_insert", "db_update", "db_delete",
     "db_bulk_insert", "db_bulk_update", "db_update_lob",
     "db_execute", "db_call_function", "db_call_procedure",
     # migration_pomes
     "db_migrate_data", "db_migrate_lobs",
```

### Comparing `pypomes_db-0.9.0/src/pypomes_db/db_common.py` & `pypomes_db-0.9.1/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.9.0/src/pypomes_db/db_pomes.py` & `pypomes_db-0.9.1/src/pypomes_db/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.9.0/src/pypomes_db/migration_pomes.py` & `pypomes_db-0.9.1/src/pypomes_db/migration_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.9.0/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.9.1/src/pypomes_db/oracle_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.9.0/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.9.1/src/pypomes_db/postgres_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.9.0/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.9.1/src/pypomes_db/sqlserver_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.9.0/LICENSE` & `pypomes_db-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.9.0/pyproject.toml` & `pypomes_db-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.9.0"
+version = "0.9.1"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.9.0/PKG-INFO` & `pypomes_db-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.9.0
+Version: 0.9.1
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

