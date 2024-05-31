# Comparing `tmp/pypomes_db-0.9.3.tar.gz` & `tmp/pypomes_db-0.9.4.tar.gz`

## Comparing `pypomes_db-0.9.3.tar` & `pypomes_db-0.9.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    12370 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    39398 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    18539 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/src/pypomes_db/migration_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    17604 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    16484 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    15408 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    12342 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    39398 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    18539 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/src/pypomes_db/migration_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    17600 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    16480 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    15394 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.9.4/PKG-INFO
```

### Comparing `pypomes_db-0.9.3/src/pypomes_db/__init__.py` & `pypomes_db-0.9.4/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.9.3/src/pypomes_db/db_common.py` & `pypomes_db-0.9.4/src/pypomes_db/db_common.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,55 +84,55 @@
 
 
 def _assert_query_quota(errors: list[str],
                         engine: str,
                         query: str,
                         where_vals: tuple,
                         count: int,
-                        require_min: int,
-                        require_max: int) -> bool:
+                        min_count: int,
+                        max_count: int) -> bool:
     """
     Verify whether the number of tuples returned is compliant with the constraints specified.
 
     :param errors: incidental error messages
     :param engine: the reference database engine
     :param query: the query statement used
     :param where_vals: the bind values used in the query
     :param count: the number of tuples returned
-    :param require_min: optionally defines the minimum number of tuples to be returned
-    :param require_max: optionally defines the maximum number of tuples to be returned
+    :param min_count: optionally defines the minimum number of tuples to be returned
+    :param max_count: optionally defines the maximum number of tuples to be returned
     :return: whether or not the number of tuples returned is compliant
     """
     # initialize the return variable
     result: bool = True
 
     # has an exact number of tuples been defined but not returned ?
-    if (isinstance(require_min, int) and
-        isinstance(require_max, int) and
-        require_min == require_max and
-        require_min != count):
+    if (isinstance(min_count, int) and
+        isinstance(max_count, int) and
+        min_count == max_count and
+        min_count != count):
         # yes, report the error, if applicable
         result = False
         if isinstance(errors, list):
             msg: str = _build_query_msg(query_stmt=query,
                                         engine=engine,
                                         bind_vals=where_vals)
-            errors.append(f"{count} tuples returned, {require_min} expected, for '{msg}'")
+            errors.append(f"{count} tuples returned, {min_count} expected, for '{msg}'")
 
     # has a minimum number of tuples been defined but not returned ?
-    elif (isinstance(require_min, int) and
-          require_min > 0 and
-          count < require_min):
+    elif (isinstance(min_count, int) and
+          min_count > 0 and
+          count < min_count):
         # yes, report the error, if applicable
         result = False
         if isinstance(errors, list):
             msg: str = _build_query_msg(query_stmt=query,
                                         engine=engine,
                                         bind_vals=where_vals)
-            errors.append(f"{count} tuples returned, at least {require_min} expected, for '{msg}'")
+            errors.append(f"{count} tuples returned, at least {min_count} expected, for '{msg}'")
 
     return result
 
 
 def _get_param(engine: str,
                param: str) -> Any:
     """
```

### Comparing `pypomes_db-0.9.3/src/pypomes_db/db_pomes.py` & `pypomes_db-0.9.4/src/pypomes_db/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.9.3/src/pypomes_db/migration_pomes.py` & `pypomes_db-0.9.4/src/pypomes_db/migration_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.9.3/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.9.4/src/pypomes_db/oracle_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,16 +100,16 @@
 
             # has the query quota been satisfied ?
             if _assert_query_quota(errors=errors,
                                    engine="oracle",
                                    query=sel_stmt,
                                    where_vals=where_vals,
                                    count=count,
-                                   require_min=min_count,
-                                   require_max=max_count):
+                                   min_count=min_count,
+                                   max_count=max_count):
                 # yes, retrieve the returned tuples
                 rows: list = cursor.fetchall()
                 result = [tuple(row) for row in rows]
         # commit the transaction, if appropriate
         if committable or not conn:
             curr_conn.commit()
     except Exception as e:
```

### Comparing `pypomes_db-0.9.3/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.9.4/src/pypomes_db/postgres_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,16 +102,16 @@
 
             # has the query quota been satisfied ?
             if _assert_query_quota(errors=errors,
                                    engine="postgres",
                                    query=sel_stmt,
                                    where_vals=where_vals,
                                    count=count,
-                                   require_min=min_count,
-                                   require_max=max_count):
+                                   min_count=min_count,
+                                   max_count=max_count):
                 # yes, retrieve the returned tuples
                 result = list(cursor)
 
         # commit the transaction, if appropriate
         if committable or not conn:
             curr_conn.commit()
     except Exception as e:
```

### Comparing `pypomes_db-0.9.3/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.9.4/src/pypomes_db/sqlserver_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,27 +88,27 @@
     if isinstance(max_count, int) and max_count > 0:
         sel_stmt: str = sel_stmt.replace("SELECT", f"SELECT TOP {max_count}", 1)
 
     try:
         # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
             cursor.execute(sel_stmt, where_vals)
+            rows: list[Row] = cursor.fetchall()
             # obtain the number of tuples returned
-            count: int = cursor.rowcount
+            count: int = len(rows)
 
             # has the query quota been satisfied ?
             if _assert_query_quota(errors=errors,
                                    engine="sqlserver",
                                    query=sel_stmt,
                                    where_vals=where_vals,
                                    count=count,
-                                   require_min=min_count,
-                                   require_max=max_count):
+                                   min_count=min_count,
+                                   max_count=max_count):
                 # yes, retrieve the returned tuples
-                rows: list[Row] = cursor.fetchall()
                 result = [tuple(row) for row in rows]
 
         # commit the transaction, if appropriate
         if committable or not conn:
             curr_conn.commit()
     except Exception as e:
         if curr_conn:
```

### Comparing `pypomes_db-0.9.3/LICENSE` & `pypomes_db-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.9.3/pyproject.toml` & `pypomes_db-0.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.9.3"
+version = "0.9.4"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.9.3/PKG-INFO` & `pypomes_db-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.9.3
+Version: 0.9.4
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

