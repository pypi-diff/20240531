# Comparing `tmp/pypomes_db-0.9.1.tar.gz` & `tmp/pypomes_db-0.9.3.tar.gz`

## Comparing `pypomes_db-0.9.1.tar` & `pypomes_db-0.9.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    12370 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    40499 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    18539 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/src/pypomes_db/migration_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    17654 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    16534 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    12370 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    39398 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    18539 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/src/pypomes_db/migration_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    17604 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    16484 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    15408 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.9.3/PKG-INFO
```

### Comparing `pypomes_db-0.9.1/src/pypomes_db/__init__.py` & `pypomes_db-0.9.3/src/pypomes_db/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from .db_pomes import (
-    db_setup, db_get_engines,  db_get_param, db_get_params,
+    db_setup, db_get_engines, db_get_param, db_get_params,
     db_assert_connection, db_connect,
-    db_exists, db_select_one, db_select_all,
-    db_insert, db_update, db_delete,
+    db_exists, db_select, db_insert, db_update, db_delete,
     db_bulk_insert, db_bulk_update, db_update_lob,
     db_execute, db_call_function, db_call_procedure,
 )
 from .migration_pomes import (
     db_migrate_data, db_migrate_lobs,
 )
 
 __all__ = [
     # db_pomes
     "db_setup", "db_get_engines", "db_get_param", "db_get_params",
     "db_assert_connection", "db_connect",
-    "db_exists", "db_select_one", "db_select_all",
-    "db_insert", "db_update", "db_delete",
+    "db_exists", "db_select", "db_insert", "db_update", "db_delete",
     "db_bulk_insert", "db_bulk_update", "db_update_lob",
     "db_execute", "db_call_function", "db_call_procedure",
     # migration_pomes
     "db_migrate_data", "db_migrate_lobs",
 ]
 
 from importlib.metadata import version
```

### Comparing `pypomes_db-0.9.1/src/pypomes_db/db_common.py` & `pypomes_db-0.9.3/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.9.1/src/pypomes_db/db_pomes.py` & `pypomes_db-0.9.3/src/pypomes_db/db_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # noinspection DuplicatedCode
 from copy import copy
 from logging import Logger
 from pathlib import Path
 from typing import Any, Literal
 
 from .db_common import (
-    _DB_ENGINES, _DB_CONN_DATA, _assert_engine, _get_param
+    _DB_ENGINES, _DB_CONN_DATA, _assert_engine, _build_query_msg, _get_param
 )
 
 
 def db_setup(engine: Literal["mysql", "oracle", "postgres", "sqlserver"],
              db_name: str,
              db_user: str,
              db_pwd: str,
@@ -141,16 +141,17 @@
         conn: Any = db_connect(errors=op_errors,
                                engine=curr_engine,
                                logger=logger)
         if conn:
             conn.close()
             result = True
 
-    # acknowledge eventual local errors
-    errors.extend(op_errors)
+    # acknowledge eventual local errors, if appropriate
+    if isinstance(errors, list):
+        errors.extend(op_errors)
 
     return result
 
 
 def db_connect(errors: list[str] | None,
                autocommit: bool = False,
                engine: str = None,
@@ -189,16 +190,18 @@
                                         logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
         result = sqlserver_pomes.connect(errors=op_errors,
                                          autocommit=autocommit,
                                          logger=logger)
 
-    # acknowledge eventual local errors
-    errors.extend(op_errors)
+
+    # acknowledge eventual local errors, if appropriate
+    if isinstance(errors, list):
+        errors.extend(op_errors)
 
     return result
 
 
 def db_exists(errors: list[str],
               table: str,
               where_attrs: list[str] = None,
@@ -220,106 +223,66 @@
     :param where_vals: the values for the search attributes
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
     :param committable: whether to commit upon errorless completion ('False' requires 'connection' to be provided)
     :param logger: optional logger
     :return: True if at least one tuple was found
     """
+    # initialize the return variable
+    result: bool | None = None
+
     # initialize the local errors list
     op_errors: list[str] = []
 
     # noinspection PyDataSource
     sel_stmt: str = "SELECT * FROM " + table
     if where_attrs:
         sel_stmt += " WHERE " + "".join(f"{attr} = %s AND " for attr in where_attrs)[0:-5]
-    rec: tuple = db_select_one(errors=op_errors,
-                               sel_stmt=sel_stmt,
-                               where_vals=where_vals,
-                               require_nonempty=False,
-                               engine = engine,
-                               connection=connection,
-                               committable=committable,
-                               logger=logger)
-    result: bool = None if op_errors else rec is not None
-
-    # acknowledge eventual local errors
-    errors.extend(op_errors)
+    rec: list[tuple] = db_select(errors=op_errors,
+                                 sel_stmt=sel_stmt,
+                                 where_vals=where_vals,
+                                 max_count=1,
+                                 engine = engine,
+                                 connection=connection,
+                                 committable=committable,
+                                 logger=logger)
+    if not op_errors:
+        result = rec is not None and len(rec) > 0
+    elif isinstance(errors, list):
+        errors.extend(op_errors)
 
     return result
 
 
-def db_select_one(errors: list[str] | None,
-                  sel_stmt: str,
-                  where_vals: tuple = None,
-                  require_nonempty: bool = False,
-                  engine: str = None,
-                  connection: Any = None,
-                  committable: bool = True,
-                  logger: Logger = None) -> tuple:
-    """
-    Search the database and return the first tuple that satisfies the *sel_stmt* search command.
-
-    The command can optionally contain search criteria, with respective values given
-    in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
-    in a specific tuple. In case of error, or if the search is empty, *None* is returned.
-    The target database engine, default or specified, must have been previously configured.
-
-    :param errors: incidental error messages
-    :param sel_stmt: SELECT command for the search
-    :param where_vals: values to be associated with the search criteria
-    :param require_nonempty: defines whether an empty search should be considered an error
-    :param engine: the database engine to use (uses the default engine, if not provided)
-    :param connection: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires 'connection' to be provided)
-    :param logger: optional logger
-    :return: tuple containing the search result, [] if the search was empty, or None if there was an error
-    """
-    # initialize the local errors list
-    op_errors: list[str] = []
-
-    require_min: int = 1 if require_nonempty else None
-    reply: list[tuple] = db_select_all(errors=op_errors,
-                                       sel_stmt=sel_stmt,
-                                       where_vals=where_vals,
-                                       require_min=require_min,
-                                       require_max=1,
-                                       engine=engine,
-                                       connection=connection,
-                                       committable=committable,
-                                       logger=logger)
-
-    # acknowledge eventual local errors
-    errors.extend(op_errors)
-
-    return reply[0] if reply else None
-
-
-def db_select_all(errors: list[str] | None,
-                  sel_stmt: str,
-                  where_vals: tuple = None,
-                  require_min: int = None,
-                  require_max: int = None,
-                  engine: str = None,
-                  connection: Any = None,
-                  committable: bool = True,
-                  logger: Logger = None) -> list[tuple]:
+def db_select(errors: list[str] | None,
+              sel_stmt: str,
+              where_vals: tuple = None,
+              min_count: int = None,
+              max_count: int = None,
+              require_single: bool = False,
+              engine: str = None,
+              connection: Any = None,
+              committable: bool = True,
+              logger: Logger = None) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
-    in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
+    in a specific tuple. If not positive integers, *min_count* and *max_count* are ignored.
+    If *require_single* is specified, then exactly one touple must be returned by the query.
     If the search is empty, an empty list is returned.
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
-    :param require_min: optionally defines the minimum number of tuples to be returned
-    :param require_max: optionally defines the maximum number of tuples to be returned
+    :param min_count: optionally defines the minimum number of tuples to be returned
+    :param max_count: optionally defines the maximum number of tuples to be returned
+    :param require_single: query must be satisfied by exactly one touple (overrides 'min_count' and 'max_count')
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
     :param committable: whether to commit upon errorless completion ('False' requires 'connection' to be provided)
     :param logger: optional logger
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
@@ -327,49 +290,63 @@
 
     # initialize the local errors list
     op_errors: list[str] = []
 
     # determine the database engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
+
+    if require_single:
+        min_count = 1
+        max_count = 2
+
+    reply: list[tuple] | None = None
     if curr_engine == "mysql":
-        pass
+        reply = []
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        result = oracle_pomes.select_all(errors=op_errors,
-                                         sel_stmt=sel_stmt,
-                                         where_vals=where_vals,
-                                         require_min=require_min,
-                                         require_max=require_max,
-                                         conn=connection,
-                                         committable=committable,
-                                         logger=logger)
+        reply = oracle_pomes.select(errors=op_errors,
+                                    sel_stmt=sel_stmt,
+                                    where_vals=where_vals,
+                                    min_count=min_count,
+                                    max_count=max_count,
+                                    conn=connection,
+                                    committable=committable,
+                                    logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        result = postgres_pomes.select_all(errors=op_errors,
-                                           sel_stmt=sel_stmt,
-                                           where_vals=where_vals,
-                                           require_min=require_min,
-                                           require_max=require_max,
-                                           conn=connection,
-                                           committable=committable,
-                                           logger=logger)
+        reply = postgres_pomes.select(errors=op_errors,
+                                      sel_stmt=sel_stmt,
+                                      where_vals=where_vals,
+                                      min_count=min_count,
+                                      max_count=max_count,
+                                      conn=connection,
+                                      committable=committable,
+                                      logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
-        result = sqlserver_pomes.select_all(errors=op_errors,
-                                            sel_stmt=sel_stmt,
-                                            where_vals=where_vals,
-                                            require_min=require_min,
-                                            require_max=require_max,
-                                            conn=connection,
-                                            committable=committable,
-                                            logger=logger)
+        reply = sqlserver_pomes.select(errors=op_errors,
+                                       sel_stmt=sel_stmt,
+                                       where_vals=where_vals,
+                                       min_count=min_count,
+                                       max_count=max_count,
+                                       conn=connection,
+                                       committable=committable,
+                                       logger=logger)
 
-    # acknowledge eventual local errors
-    errors.extend(op_errors)
+    if not op_errors and require_single and len(reply) > 1:
+        msg: str = _build_query_msg(query_stmt=sel_stmt,
+                                    engine=engine,
+                                    bind_vals=where_vals)
+        op_errors.append(f"More than one touple satisfies {msg}")
+
+    if not op_errors:
+        result = reply
+    elif isinstance(errors, list):
+        errors.extend(op_errors)
 
     return result
 
 
 def db_insert(errors: list[str] | None,
               insert_stmt: str,
               insert_vals: tuple,
@@ -398,16 +375,17 @@
                              exc_stmt=insert_stmt,
                              bind_vals=insert_vals,
                              engine=engine,
                              connection=connection,
                              committable=committable,
                              logger=logger)
 
-    # acknowledge eventual local errors
-    errors.extend(op_errors)
+    # acknowledge eventual local errors, if appropriate
+    if isinstance(errors, list):
+        errors.extend(op_errors)
 
     return result
 
 
 def db_update(errors: list[str] | None,
               update_stmt: str,
               update_vals: tuple = None,
@@ -447,16 +425,17 @@
                              exc_stmt=update_stmt,
                              bind_vals=bind_vals,
                              engine=engine,
                              connection=connection,
                              committable=committable,
                              logger=logger)
 
-    # acknowledge eventual local errors
-    errors.extend(op_errors)
+    # acknowledge eventual local errors, if appropriate
+    if isinstance(errors, list):
+        errors.extend(op_errors)
 
     return result
 
 
 def db_delete(errors: list[str] | None,
               delete_stmt: str,
               where_vals: tuple = None,
@@ -486,16 +465,17 @@
                              exc_stmt=delete_stmt,
                              bind_vals=where_vals,
                              engine=engine,
                              connection=connection,
                              committable=committable,
                              logger=logger)
 
-    # acknowledge eventual local errors
-    errors.extend(op_errors)
+    # acknowledge eventual local errors, if appropriate
+    if isinstance(errors, list):
+        errors.extend(op_errors)
 
     return result
 
 
 def db_bulk_insert(errors: list[str] | None,
                    insert_stmt: str,
                    insert_vals: list[tuple],
@@ -555,16 +535,17 @@
         result = sqlserver_pomes.bulk_execute(errors=op_errors,
                                               exc_stmt=insert_stmt,
                                               exc_vals=insert_vals,
                                               conn=connection,
                                               committable=committable,
                                               logger=logger)
 
-    # acknowledge eventual local errors
-    errors.extend(op_errors)
+    # acknowledge eventual local errors, if appropriate
+    if isinstance(errors, list):
+        errors.extend(op_errors)
 
     return result
 
 
 def db_bulk_update(errors: list[str] | None,
                    update_stmt: str,
                    update_vals: list[tuple],
@@ -628,16 +609,17 @@
         result = sqlserver_pomes.bulk_execute(errors=op_errors,
                                               exc_stmt=update_stmt,
                                               exc_vals=update_vals,
                                               conn=connection,
                                               committable=committable,
                                               logger=logger)
 
-    # acknowledge eventual local errors
-    errors.extend(op_errors)
+    # acknowledge eventual local errors, if appropriate
+    if isinstance(errors, list):
+        errors.extend(op_errors)
 
     return result
 
 
 def db_update_lob(errors: list[str],
                   lob_table: str,
                   lob_column: str,
@@ -706,16 +688,17 @@
                                    pk_vals=pk_vals,
                                    lob_file=lob_file,
                                    chunk_size=chunk_size,
                                    conn=connection,
                                    committable=committable,
                                    logger=logger)
 
-    # acknowledge eventual local errors
-    errors.extend(op_errors)
+    # acknowledge eventual local errors, if appropriate
+    if isinstance(errors, list):
+        errors.extend(op_errors)
 
 
 def db_execute(errors: list[str] | None,
                exc_stmt: str,
                bind_vals: tuple = None,
                engine: str = None,
                connection: Any = None,
@@ -773,16 +756,17 @@
         result = sqlserver_pomes.execute(errors=op_errors,
                                          exc_stmt=exc_stmt,
                                          bind_vals=bind_vals,
                                          conn=connection,
                                          committable=committable,
                                          logger=logger)
 
-    # acknowledge eventual local errors
-    errors.extend(op_errors)
+    # acknowledge eventual local errors, if appropriate
+    if isinstance(errors, list):
+        errors.extend(op_errors)
 
     return result
 
 
 def db_call_function(errors: list[str] | None,
                      func_name: str,
                      func_vals: tuple = None,
@@ -836,16 +820,17 @@
         result = sqlserver_pomes.call_procedure(errors=op_errors,
                                                 proc_name=func_name,
                                                 proc_vals=func_vals,
                                                 conn=connection,
                                                 committable=committable,
                                                 logger=logger)
 
-    # acknowledge eventual local errors
-    errors.extend(op_errors)
+    # acknowledge eventual local errors, if appropriate
+    if isinstance(errors, list):
+        errors.extend(op_errors)
 
     return result
 
 
 def db_call_procedure(errors: list[str] | None,
                       proc_name: str,
                       proc_vals: tuple = None,
@@ -899,11 +884,12 @@
         result = sqlserver_pomes.call_procedure(errors=op_errors,
                                                 proc_name=proc_name,
                                                 proc_vals=proc_vals,
                                                 conn=connection,
                                                 committable=committable,
                                                 logger=logger)
 
-    # acknowledge eventual local errors
-    errors.extend(op_errors)
+    # acknowledge eventual local errors, if appropriate
+    if isinstance(errors, list):
+        errors.extend(op_errors)
 
     return result
```

### Comparing `pypomes_db-0.9.1/src/pypomes_db/migration_pomes.py` & `pypomes_db-0.9.3/src/pypomes_db/migration_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.9.1/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.9.3/src/pypomes_db/oracle_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,50 +47,50 @@
          err_msg=err_msg,
          errors=errors,
          stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
-def select_all(errors: list[str],
-               sel_stmt: str,
-               where_vals: tuple,
-               require_min: int,
-               require_max: int,
-               conn: Connection,
-               committable: bool,
-               logger: Logger) -> list[tuple]:
+def select(errors: list[str],
+           sel_stmt: str,
+           where_vals: tuple,
+           min_count: int,
+           max_count: int,
+           conn: Connection,
+           committable: bool,
+           logger: Logger) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
     If the search is empty, an empty list is returned.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
-    :param require_min: optionally defines the minimum number of tuples to be returned
-    :param require_max: optionally defines the maximum number of tuples to be returned
+    :param min_count: optionally defines the minimum number of tuples to be returned
+    :param max_count: optionally defines the maximum number of tuples to be returned
     :param conn: optional connection to use (obtains a new one, if not provided)
     :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
     :return: tuple containing the search result, [] if the search was empty, or None if there was an error
     """
     # initialize the return variable
     result: list[tuple] = []
 
     # make sure to have a connection
     curr_conn: Connection = conn or connect(errors=errors,
                                             autocommit=False,
                                             logger=logger)
 
-    if isinstance(require_max, int) and require_max > 0:
-        sel_stmt: str = f"{sel_stmt} FETCH NEXT {require_max} ROWS ONLY"
+    if isinstance(max_count, int) and max_count > 0:
+        sel_stmt: str = f"{sel_stmt} FETCH NEXT {max_count} ROWS ONLY"
 
     err_msg: str | None = None
     try:
         # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
             # execute the query
             cursor.execute(statement=sel_stmt,
@@ -100,16 +100,16 @@
 
             # has the query quota been satisfied ?
             if _assert_query_quota(errors=errors,
                                    engine="oracle",
                                    query=sel_stmt,
                                    where_vals=where_vals,
                                    count=count,
-                                   require_min=require_min,
-                                   require_max=require_max):
+                                   require_min=min_count,
+                                   require_max=max_count):
                 # yes, retrieve the returned tuples
                 rows: list = cursor.fetchall()
                 result = [tuple(row) for row in rows]
         # commit the transaction, if appropriate
         if committable or not conn:
             curr_conn.commit()
     except Exception as e:
```

### Comparing `pypomes_db-0.9.1/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.9.3/src/pypomes_db/postgres_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,50 +50,50 @@
          err_msg=err_msg,
          errors=errors,
          stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
-def select_all(errors: list[str],
-               sel_stmt: str,
-               where_vals: tuple,
-               require_min: int,
-               require_max: int,
-               conn: connection,
-               committable: bool,
-               logger: Logger) -> list[tuple]:
+def select(errors: list[str],
+           sel_stmt: str,
+           where_vals: tuple,
+           min_count: int,
+           max_count: int,
+           conn: connection,
+           committable: bool,
+           logger: Logger) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
     If the search is empty, an empty list is returned.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
-    :param require_min: optionally defines the minimum number of tuples to be returned
-    :param require_max: optionally defines the maximum number of tuples to be returned
+    :param min_count: optionally defines the minimum number of tuples to be returned
+    :param max_count: optionally defines the maximum number of tuples to be returned
     :param conn: optional connection to use (obtains a new one, if not provided)
     :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] = []
 
     # make sure to have a connection
     curr_conn: connection = conn or connect(errors=errors,
                                             autocommit=False,
                                             logger=logger)
 
-    if isinstance(require_max, int) and require_max >= 0:
-        sel_stmt += f" LIMIT {require_max}"
+    if isinstance(max_count, int) and max_count >= 0:
+        sel_stmt += f" LIMIT {max_count}"
 
     err_msg: str | None = None
     try:
         # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
             cursor.execute(query=f"{sel_stmt};",
                            vars=where_vals)
@@ -102,16 +102,16 @@
 
             # has the query quota been satisfied ?
             if _assert_query_quota(errors=errors,
                                    engine="postgres",
                                    query=sel_stmt,
                                    where_vals=where_vals,
                                    count=count,
-                                   require_min=require_min,
-                                   require_max=require_max):
+                                   require_min=min_count,
+                                   require_max=max_count):
                 # yes, retrieve the returned tuples
                 result = list(cursor)
 
         # commit the transaction, if appropriate
         if committable or not conn:
             curr_conn.commit()
     except Exception as e:
```

### Comparing `pypomes_db-0.9.1/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.9.3/src/pypomes_db/sqlserver_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,67 +46,67 @@
          err_msg=err_msg,
          errors=errors,
          stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
-def select_all(errors: list[str],
-               sel_stmt: str,
-               where_vals: tuple,
-               require_min: int,
-               require_max: int,
-               conn: Connection,
-               committable: bool,
-               logger: Logger) -> list[tuple]:
+def select(errors: list[str],
+           sel_stmt: str,
+           where_vals: tuple,
+           min_count: int,
+           max_count: int,
+           conn: Connection,
+           committable: bool,
+           logger: Logger) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
     If the search is empty, an empty list is returned.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
-    :param require_min: optionally defines the minimum number of tuples to be returned
-    :param require_max: optionally defines the maximum number of tuples to be returned
+    :param min_count: optionally defines the minimum number of tuples to be returned
+    :param max_count: optionally defines the maximum number of tuples to be returned
     :param conn: optional connection to use (obtains a new one, if not provided)
     :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
     :return: tuple containing the search result, [] if the search was empty, or None if there was an error
     """
     # initialize the return variable
     result: list[tuple] = []
 
     # make sure to have a connection
     curr_conn: Connection = conn or connect(errors=errors,
                                             autocommit=False,
                                             logger=logger)
 
     err_msg: str | None = None
-    if isinstance(require_max, int) and require_max > 0:
-        sel_stmt: str = sel_stmt.replace("SELECT", f"SELECT TOP {require_max}", 1)
+    if isinstance(max_count, int) and max_count > 0:
+        sel_stmt: str = sel_stmt.replace("SELECT", f"SELECT TOP {max_count}", 1)
 
     try:
         # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
             cursor.execute(sel_stmt, where_vals)
             # obtain the number of tuples returned
             count: int = cursor.rowcount
 
             # has the query quota been satisfied ?
             if _assert_query_quota(errors=errors,
                                    engine="sqlserver",
                                    query=sel_stmt,
                                    where_vals=where_vals,
                                    count=count,
-                                   require_min=require_min,
-                                   require_max=require_max):
+                                   require_min=min_count,
+                                   require_max=max_count):
                 # yes, retrieve the returned tuples
                 rows: list[Row] = cursor.fetchall()
                 result = [tuple(row) for row in rows]
 
         # commit the transaction, if appropriate
         if committable or not conn:
             curr_conn.commit()
```

### Comparing `pypomes_db-0.9.1/LICENSE` & `pypomes_db-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.9.1/pyproject.toml` & `pypomes_db-0.9.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.9.1"
+version = "0.9.3"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "pip>=24.0",
 #   "mysql-connector-python>=8.4.0",
-#   "oracledb>=2.2.0",
+#   "oracledb>=2.2.1",
 #   "psycopg2-binary>=2.9.9",
 #   "pyodbc>=5.1.0",
-    "pypomes_core>=1.1.3",
+    "pypomes_core>=1.1.4",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-DB"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes-DB/issues"
```

### Comparing `pypomes_db-0.9.1/PKG-INFO` & `pypomes_db-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.9.1
+Version: 0.9.3
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
-Requires-Dist: pypomes-core>=1.1.3
+Requires-Dist: pypomes-core>=1.1.4
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
```

