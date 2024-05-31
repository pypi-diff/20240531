# Comparing `tmp/pypomes_db-0.9.4.tar.gz` & `tmp/pypomes_db-0.9.5.tar.gz`

## Comparing `pypomes_db-0.9.4.tar` & `pypomes_db-0.9.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    12342 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    39398 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    18539 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/src/pypomes_db/migration_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    17600 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    16480 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    15394 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 pypomes_db-0.9.5/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    12342 2020-02-02 00:00:00.000000 pypomes_db-0.9.5/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    39398 2020-02-02 00:00:00.000000 pypomes_db-0.9.5/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    18539 2020-02-02 00:00:00.000000 pypomes_db-0.9.5/src/pypomes_db/migration_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.9.5/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    17590 2020-02-02 00:00:00.000000 pypomes_db-0.9.5/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    16480 2020-02-02 00:00:00.000000 pypomes_db-0.9.5/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    15394 2020-02-02 00:00:00.000000 pypomes_db-0.9.5/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.9.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.9.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.9.5/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.9.5/PKG-INFO
```

### Comparing `pypomes_db-0.9.4/src/pypomes_db/__init__.py` & `pypomes_db-0.9.5/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.9.4/src/pypomes_db/db_common.py` & `pypomes_db-0.9.5/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.9.4/src/pypomes_db/db_pomes.py` & `pypomes_db-0.9.5/src/pypomes_db/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.9.4/src/pypomes_db/migration_pomes.py` & `pypomes_db-0.9.5/src/pypomes_db/migration_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.9.4/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.9.5/src/pypomes_db/oracle_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,27 +91,27 @@
     err_msg: str | None = None
     try:
         # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
             # execute the query
             cursor.execute(statement=sel_stmt,
                            parameters=where_vals)
+            rows: list = cursor.fetchall()
             # obtain the number of tuples returned
-            count: int = cursor.rowcount
+            count: int = len(rows)
 
             # has the query quota been satisfied ?
             if _assert_query_quota(errors=errors,
                                    engine="oracle",
                                    query=sel_stmt,
                                    where_vals=where_vals,
                                    count=count,
                                    min_count=min_count,
                                    max_count=max_count):
                 # yes, retrieve the returned tuples
-                rows: list = cursor.fetchall()
                 result = [tuple(row) for row in rows]
         # commit the transaction, if appropriate
         if committable or not conn:
             curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
```

### Comparing `pypomes_db-0.9.4/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.9.5/src/pypomes_db/postgres_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.9.4/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.9.5/src/pypomes_db/sqlserver_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.9.4/LICENSE` & `pypomes_db-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.9.4/pyproject.toml` & `pypomes_db-0.9.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.9.4"
+version = "0.9.5"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -20,15 +20,15 @@
 ]
 dependencies = [
     "pip>=24.0",
 #   "mysql-connector-python>=8.4.0",
 #   "oracledb>=2.2.1",
 #   "psycopg2-binary>=2.9.9",
 #   "pyodbc>=5.1.0",
-    "pypomes_core>=1.1.4",
+    "pypomes_core>=1.1.6",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-DB"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes-DB/issues"
```

### Comparing `pypomes_db-0.9.4/PKG-INFO` & `pypomes_db-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.9.4
+Version: 0.9.5
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=1.1.4
+Requires-Dist: pypomes-core>=1.1.6
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
```

