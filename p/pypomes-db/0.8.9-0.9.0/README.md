# Comparing `tmp/pypomes_db-0.8.9.tar.gz` & `tmp/pypomes_db-0.9.0.tar.gz`

## Comparing `pypomes_db-0.8.9.tar` & `pypomes_db-0.9.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    39427 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    18680 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/src/pypomes_db/migration_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    17852 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    16723 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    15635 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    12370 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    40499 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    18539 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/src/pypomes_db/migration_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    17654 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    16534 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.9.0/PKG-INFO
```

### Comparing `pypomes_db-0.8.9/src/pypomes_db/__init__.py` & `pypomes_db-0.9.0/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.9/src/pypomes_db/db_common.py` & `pypomes_db-0.9.0/src/pypomes_db/db_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,42 +19,45 @@
 # 2. alternatively, specify a comma-separated list of engines in
 #   {APP_PREFIX}_DB_ENGINES
 #   and for each engine, specify the set above, replacing 'DB' with
 #   'MSQL', 'ORCL', 'PG', and 'SQLS', respectively for the engines listed above
 
 _DB_CONN_DATA: dict = {}
 _DB_ENGINES: list[str] = []
-_prefix: str = env_get_str(f"{APP_PREFIX}_DB_ENGINE",  None)
+_prefix: str = env_get_str(key=f"{APP_PREFIX}_DB_ENGINE",
+                           def_value=None)
 if _prefix:
     _default_setup: bool = True
     _DB_ENGINES.append(_prefix)
 else:
     _default_setup: bool = False
-    _engines: str = env_get_str(f"{APP_PREFIX}_DB_ENGINES", None)
+    _engines: str = env_get_str(key=f"{APP_PREFIX}_DB_ENGINES",
+                                def_value=None)
     if _engines:
         _DB_ENGINES.extend(_engines.split(sep=","))
 for engine in _DB_ENGINES:
     if _default_setup:
         _tag = "DB"
         _default_setup = False
     else:
         _tag: str = str_get_positional(source=engine,
                                        list_origin=["mysql", "oracle", "postgres", "sqlserver"],
                                        list_dest=["MSQL", "ORCL", "PG", "SQLS"])
     _db_data = {
-        "name":  env_get_str(f"{APP_PREFIX}_{_tag}_NAME"),
-        "user": env_get_str(f"{APP_PREFIX}_{_tag}_USER"),
-        "pwd": env_get_str(f"{APP_PREFIX}_{_tag}_PWD"),
-        "host": env_get_str(f"{APP_PREFIX}_{_tag}_HOST"),
-        "port": env_get_int(f"{APP_PREFIX}_{_tag}_PORT")
+        "name":  env_get_str(key=f"{APP_PREFIX}_{_tag}_NAME"),
+        "user": env_get_str(key=f"{APP_PREFIX}_{_tag}_USER"),
+        "pwd": env_get_str(key=f"{APP_PREFIX}_{_tag}_PWD"),
+        "host": env_get_str(key=f"{APP_PREFIX}_{_tag}_HOST"),
+        "port": env_get_int(key=f"{APP_PREFIX}_{_tag}_PORT")
     }
     if engine == "oracle":
-        _db_data["client"] = env_get_str(f"{APP_PREFIX}_{_tag}_CLIENT", None)
+        _db_data["client"] = env_get_str(key=f"{APP_PREFIX}_{_tag}_CLIENT",
+                                         def_value=None)
     elif engine == "sqlserver":
-        _db_data["driver"] = env_get_str(f"{APP_PREFIX}_{_tag}_DRIVER")
+        _db_data["driver"] = env_get_str(key=f"{APP_PREFIX}_{_tag}_DRIVER")
     _DB_CONN_DATA[engine] = _db_data
 
 
 def _assert_engine(errors: list[str],
                    engine: str) -> str:
     """
     Verify if *engine* is in the list of supported engines.
@@ -76,21 +79,21 @@
     else:
         err_msg = f"Database engine '{engine}' unknown or not configured"
         errors.append(err_msg)
 
     return result
 
 
-def _db_assert_query_quota(errors: list[str],
-                           engine: str,
-                           query: str,
-                           where_vals: tuple,
-                           count: int,
-                           require_min: int,
-                           require_max: int) -> bool:
+def _assert_query_quota(errors: list[str],
+                        engine: str,
+                        query: str,
+                        where_vals: tuple,
+                        count: int,
+                        require_min: int,
+                        require_max: int) -> bool:
     """
     Verify whether the number of tuples returned is compliant with the constraints specified.
 
     :param errors: incidental error messages
     :param engine: the reference database engine
     :param query: the query statement used
     :param where_vals: the bind values used in the query
@@ -106,96 +109,97 @@
     if (isinstance(require_min, int) and
         isinstance(require_max, int) and
         require_min == require_max and
         require_min != count):
         # yes, report the error, if applicable
         result = False
         if isinstance(errors, list):
-            msg: str = _db_build_query_msg(query_stmt=query,
-                                            engine=engine,
-                                            bind_vals=where_vals)
+            msg: str = _build_query_msg(query_stmt=query,
+                                        engine=engine,
+                                        bind_vals=where_vals)
             errors.append(f"{count} tuples returned, {require_min} expected, for '{msg}'")
 
     # has a minimum number of tuples been defined but not returned ?
     elif (isinstance(require_min, int) and
           require_min > 0 and
           count < require_min):
         # yes, report the error, if applicable
         result = False
         if isinstance(errors, list):
-            msg: str = _db_build_query_msg(query_stmt=query,
-                                            engine=engine,
-                                            bind_vals=where_vals)
+            msg: str = _build_query_msg(query_stmt=query,
+                                        engine=engine,
+                                        bind_vals=where_vals)
             errors.append(f"{count} tuples returned, at least {require_min} expected, for '{msg}'")
 
     return result
 
 
-def _db_get_param(engine: str,
-                  param: str) -> Any:
+def _get_param(engine: str,
+               param: str) -> Any:
     """
     Return the current value of *param* being used by *engine*.
 
     :param engine: the reference database engine
     :param param: the reference parameter
     :return: the parameter's current value
     """
-    return _DB_CONN_DATA[engine].get(param)
+    return _DB_CONN_DATA.get(engine or {}).get(param)
 
 
-def _db_get_params(engine: str) -> tuple:
+def _get_params(engine: str) -> tuple:
     """
     Return the current connection parameters being used for *engine*.
 
     The connection parameters are returned as a *tuple*, with the elements
     *name*, *user*, *pwd*, *host*, *port*.
     For *oracle* engines, the extra element *client* is returned.
     For *sqlserver* engines, the extra element *driver* is returned.
     The meaning of some parameters may vary between different database engines.
 
     :param engine: the reference database engine
     :return: the current connection parameters for the engine
     """
-    name: str = _DB_CONN_DATA[engine].get("name")
-    user: str = _DB_CONN_DATA[engine].get("user")
-    pwd: str = _DB_CONN_DATA[engine].get("pwd")
-    host: str = _DB_CONN_DATA[engine].get("host")
-    port: int = _DB_CONN_DATA[engine].get("port")
+    conn_data: dict = _DB_CONN_DATA[engine] or {}
+    name: str = conn_data.get("name")
+    user: str = conn_data.get("user")
+    pwd: str = conn_data.get("pwd")
+    host: str = conn_data.get("host")
+    port: int = conn_data.get("port")
 
     result: tuple
     if engine == "sqlserver":
-        driver: str = _DB_CONN_DATA[engine].get("driver")
+        driver: str = conn_data.get("driver")
         result = (name, user, pwd, host, port, driver)
     else:
         result = (name, user, pwd, host, port)
 
     return result
 
 
-def _db_except_msg(exception: Exception,
-                   engine: str) -> str:
+def _except_msg(exception: Exception,
+                engine: str) -> str:
     """
     Format and return the error message corresponding to the exception raised while accessing the database.
 
     :param exception: the exception raised
     :param engine: the reference database engine
     :return: the formatted error message
     """
     name: str = _DB_CONN_DATA[engine].get("name")
     host: str = _DB_CONN_DATA[engine].get("host")
     return f"Error accessing '{name}' at '{host}': {str_sanitize(f'{exception}')}"
 
 
-def _db_log(logger: Logger,
-            engine: str,
-            err_msg: str = None,
-            level: int = DEBUG,
-            errors: list[str] = None,
-            stmt: str = None,
-            bind_vals: tuple = None) -> None:
+def _log(logger: Logger,
+         engine: str,
+         err_msg: str = None,
+         level: int = DEBUG,
+         errors: list[str] = None,
+         stmt: str = None,
+         bind_vals: tuple = None) -> None:
     """
     Log *err_msg* and add it to *errors*, or else log the executed query, whichever is applicable.
 
     :param logger: the logger object
     :param engine: the reference database engine
     :param err_msg: the error message to log
     :param level: log level (defaults to DEBUG)
@@ -205,23 +209,23 @@
     """
     if err_msg:
         if logger:
             logger.log(level, err_msg)
         if isinstance(errors, list):
             errors.append(err_msg)
     if logger and stmt:
-        log_msg: str = _db_build_query_msg(query_stmt=stmt,
-                                           engine=engine,
-                                           bind_vals=bind_vals)
+        log_msg: str = _build_query_msg(query_stmt=stmt,
+                                        engine=engine,
+                                        bind_vals=bind_vals)
         logger.log(level, log_msg)
 
 
-def _db_build_query_msg(query_stmt: str,
-                        engine: str,
-                        bind_vals: tuple) -> str:
+def _build_query_msg(query_stmt: str,
+                     engine: str,
+                     bind_vals: tuple) -> str:
     """
     Format and return the message indicative of a query problem.
 
     :param query_stmt: the query command
     :param engine: the reference database engine
     :param bind_vals: values associated with the query command
     :return: message indicative of empty search
@@ -240,18 +244,18 @@
                 result = result.replace("%s", sval, 1)
             case "sqlserver":
                 result = result.replace("?", sval, 1)
 
     return result
 
 
-def _db_bind_columns(engine: str,
-                     columns: list[str],
-                     concat: str,
-                     start_index: int) -> str:
+def _bind_columns(engine: str,
+                  columns: list[str],
+                  concat: str,
+                  start_index: int) -> str:
     """
     Concatenate a list of column names bindings, appropriate for the engine sepcified.
 
     The concatenation term *concat* is typically *" AND "*, if the bindings are aimed at a
     *WHERE* clause, or *", "* otherwise.
 
     :param engine: the reference database engine
@@ -275,17 +279,17 @@
             result =  concat.join([f"{column} = %s" for column in columns])
         case "sqlserver":
             result = concat.join([f"{column} = ?" for column in columns])
 
     return result
 
 
-def _db_bind_marks(engine: str,
-                   start: int,
-                   finish: int) -> str:
+def _bind_marks(engine: str,
+                start: int,
+                finish: int) -> str:
     """
     Concatenate a list of binding marks, appropriate for the engine sepcified.
 
     :param engine: the reference database engine
     :param start: the number to start from, inclusive
     :param finish: the number to finish at, exclusive
     :return: the concatenated string
@@ -303,15 +307,15 @@
             result = ",".join(["%s" for _inx in range(start, finish)])
         case "sqlserver":
             result = ",".join(["?" for _inx in range(start, finish)])
 
     return result
 
 
-def _db_remove_nulls(row: Iterable) -> list[Any]:
+def _remove_nulls(row: Iterable) -> list[Any]:
     """
     Remove all occurrences of *NULL* (char(0)) values from the elements in *row*.
 
     :param row: the row to be cleaned
     :return: a row with cleaned data, or None if no cleaning was necessary
     """
     # initialize the return variable
```

### Comparing `pypomes_db-0.8.9/src/pypomes_db/db_pomes.py` & `pypomes_db-0.9.0/src/pypomes_db/db_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # noinspection DuplicatedCode
+from copy import copy
 from logging import Logger
 from pathlib import Path
-from typing import Any
+from typing import Any, Literal
 
 from .db_common import (
-    _DB_ENGINES, _DB_CONN_DATA, _assert_engine
+    _DB_ENGINES, _DB_CONN_DATA, _assert_engine, _get_param
 )
 
 
-def db_setup(engine: str,
+def db_setup(engine: Literal["mysql", "oracle", "postgres", "sqlserver"],
              db_name: str,
              db_user: str,
              db_pwd: str,
              db_host: str,
              db_port: int,
              db_client: str = None,
              db_driver: str = None) -> bool:
@@ -70,28 +71,49 @@
     *mysql*, *oracle*, *postgres*, *sqlserver*.
 
     :return: the list of configured engines
     """
     return _DB_ENGINES
 
 
+def db_get_param(key: Literal["name", "user", "host", "port", "client", "driver"],
+                 engine: str = None) -> dict:
+    """
+    Return the connection parameter value for *key*.
+
+    The connection key should be one of *name*, *user*, *host*, and *port*.
+    For *oracle* and *sqlserver* engines, the extra keys *client* and *driver*
+    might be used, respectively.
+
+    :param key: the reference parameter
+    :param engine: the database engine to use (uses the default engine, if not provided)
+    :return: the current connection parameters for the engine
+    """
+    curr_engine: str = _DB_ENGINES[0] if not engine and _DB_ENGINES else engine
+    return None if key == "pwd" else _get_param(curr_engine, key)
+
+
 def db_get_params(engine: str = None) -> dict:
     """
     Return the connection parameters as a *dict*.
 
-    The returned *dict* contains the keys *name*, *user*, *pwd*, *host*, *port*.
+    The returned *dict* contains the keys *name*, *user*, *host*, *port*.
     For *oracle* engines, the returned *dict* contains the extra key *client*.
     For *sqlserver* engines, the  returned *dict* contains the extra key *driver*.
     The meaning of these parameters may vary between different database engines.
+    Note that the value of the *pwd* parameter is not returned.
 
-    :param engine: the database engine
+    :param engine: the database engine to use (uses the default engine, if not provided)
     :return: the current connection parameters for the engine
     """
     curr_engine: str = _DB_ENGINES[0] if not engine and _DB_ENGINES else engine
-    return _DB_CONN_DATA.get(engine or curr_engine)
+    result: dict = copy(x=_DB_CONN_DATA.get(curr_engine))
+    result.pop("pwd", None)
+
+    return result
 
 
 def db_assert_connection(errors: list[str] | None,
                          engine: str = None,
                          logger: Logger = None) -> bool:
     """
     Determine whether the *engine*'s current configuration allows for a safe connection.
@@ -194,15 +216,15 @@
 
     :param errors: incidental error messages
     :param table: the table to be searched
     :param where_attrs: the search attributes
     :param where_vals: the values for the search attributes
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'connection' to be provided)
     :param logger: optional logger
     :return: True if at least one tuple was found
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
     # noinspection PyDataSource
@@ -243,15 +265,15 @@
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: values to be associated with the search criteria
     :param require_nonempty: defines whether an empty search should be considered an error
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'connection' to be provided)
     :param logger: optional logger
     :return: tuple containing the search result, [] if the search was empty, or None if there was an error
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
     require_min: int = 1 if require_nonempty else None
@@ -292,15 +314,15 @@
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'connection' to be provided)
     :param logger: optional logger
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] | None = None
 
     # initialize the local errors list
@@ -361,15 +383,15 @@
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the values to be inserted
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'connection' to be provided)
     :param logger: optional logger
     :return: the number of inserted tuples (0 ou 1), or None if an error occurred
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
     result: int = db_execute(errors=op_errors,
@@ -403,15 +425,15 @@
 
     :param errors: incidental error messages
     :param update_stmt: the UPDATE command
     :param update_vals: the values for the update operation
     :param where_vals: the values to be associated with the search criteria
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'connection' to be provided)
     :param logger: optional logger
     :return: the number of updated tuples, or None if an error occurred
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
     bind_vals: tuple | None = None
@@ -449,15 +471,15 @@
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param delete_stmt: the DELETE command
     :param where_vals: the values to be associated with the search criteria
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'connection' to be provided)
     :param logger: optional logger
     :return: the number of deleted tuples, or None if an error occurred
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
     result: int = db_execute(errors=op_errors,
@@ -493,15 +515,15 @@
     data in the tuple. In the specific case of *postgres*, the *VALUES* clause must be simply *VALUES %s*.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'connection' to be provided)
     :param logger: optional logger
     :return: the number of inserted tuples (1 for postgres), or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
     # initialize the local errors list
@@ -566,15 +588,15 @@
     there is also a *FROM* clause to go along with it.
 
     :param errors: incidental error messages
     :param update_stmt: the UPDATE command
     :param update_vals: the list of values to update the database with, and to locate the tuple
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'connection' to be provided)
     :param logger: optional logger
     :return: the number of updated tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
     # initialize the local errors list
@@ -635,15 +657,15 @@
     :param lob_column: the column to be updated with the new LOB
     :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
     :param pk_vals: values with which to locate the tuple to be updated
     :param lob_file: file holding the LOB (a file object or a valid path)
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'connection' to be provided)
     :param logger: optional logger
     :return: number of LOBs effectively copied
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
     # determine the database engine
@@ -711,15 +733,15 @@
     ou None if an error occurred.
 
     :param errors: incidental error messages
     :param exc_stmt: the command to execute
     :param bind_vals: optional bind values
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'connection' to be provided)
     :param logger: optional logger
     :return: the return value from the command execution
     """
     # initialize the return variable
     result: int | None = None
 
     # initialize the local errors list
@@ -774,15 +796,15 @@
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param func_name: name of the stored function
     :param func_vals: parameters for the stored function
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'connection' to be provided)
     :param logger: optional logger
     :return: the data returned by the function
     """
     # initialize the return variable
     result: Any = None
 
     # initialize the local errors list
@@ -837,15 +859,15 @@
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'connection' to be provided)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
     result: Any = None
 
     # initialize the local errors list
```

### Comparing `pypomes_db-0.8.9/src/pypomes_db/migration_pomes.py` & `pypomes_db-0.9.0/src/pypomes_db/migration_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # noinspection DuplicatedCode
 from logging import WARNING, Logger
 from typing import Any
 
 from .db_common import (
-    _db_bind_columns, _db_bind_marks, _db_log, _db_except_msg, _db_remove_nulls
+    _bind_columns, _bind_marks, _log, _except_msg, _remove_nulls
 )
 from .db_pomes import db_connect
 
 
 def db_migrate_data(errors: list[str],
                     source_engine: str,
                     source_table: str,
@@ -69,26 +69,26 @@
     if where_clause:
         sel_stmt += f" WHERE {where_clause}"
 
     # build the INSERT query
     if target_engine == "postgres":
         values: str = "VALUES %s"
     else:
-        raw_row: str = _db_bind_marks(engine=target_engine,
-                                      start=1,
-                                      finish=len(target_columns)+1)
+        raw_row: str = _bind_marks(engine=target_engine,
+                                   start=1,
+                                   finish=len(target_columns)+1)
         values: str = f"VALUES({raw_row})"
     cols: str = ", ".join(target_columns)
     insert_stmt = (f"INSERT INTO {target_table} "
                    f"({cols}) {values}")
 
     # log the migration start
-    _db_log(logger=logger,
-            engine=source_engine,
-            stmt=(f"Started migrating data, "
+    _log(logger=logger,
+         engine=source_engine,
+         stmt=(f"Started migrating data, "
                   f"from {source_engine}.{source_table} "
                   f"to {target_engine}.{target_table}"))
 
     # migrate the data
     err_msg: str | None = None
     try:
         source_cursor: Any = curr_source_conn.cursor()
@@ -121,22 +121,22 @@
                                        sql=insert_stmt,
                                        argslist=rows)
                     except ValueError as e:
                         # is it a 'ValueError' exception on NULLs in strings ?
                         # ("A string literal cannot contain NUL (0x00) characters.")
                         if "contain NUL" in e.args[0]:
                             # yes, log the occurrence, remove the NULLs, and try again
-                            _db_log(logger=logger,
-                                    engine="postgres",
-                                    level=WARNING,
-                                    stmt=f"Found NULLs in values for {insert_stmt}")
+                            _log(logger=logger,
+                                 engine="postgres",
+                                 level=WARNING,
+                                 stmt=f"Found NULLs in values for {insert_stmt}")
                             # search for NULLs in input data
                             cleaned_rows: [tuple] = []
                             for row in rows:
-                                cleaned_row: list[Any] = _db_remove_nulls(row)
+                                cleaned_row: list[Any] = _remove_nulls(row)
                                 # has the row been cleaned ?
                                 if cleaned_row:
                                     # yes, use it
                                     cleaned_rows.append(tuple(cleaned_row))
                                 else:
                                     # no, use original row
                                     cleaned_rows.append(row)
@@ -146,17 +146,17 @@
                                            argslist=cleaned_rows)
                 case "sqlserver":
                     target_cursor.executemany(insert_stmt, rows)
 
             # log partial result
             row_count += 1
             if row_count % 100000 == 0:
-                _db_log(logger=logger,
-                        engine=source_engine,
-                        stmt=(f"Migrated {row_count} tuples, "
+                _log(logger=logger,
+                     engine=source_engine,
+                     stmt=(f"Migrated {row_count} tuples, "
                               f"from {source_engine}.{source_table} "
                               f"to {target_engine}.{target_table}"))
 
             # increment the tuple migration counter
             result += len(rows)
             # read the next batch
             if batch_size:
@@ -171,29 +171,29 @@
         curr_target_conn.commit()
     except Exception as e:
         # rollback the transactions
         if curr_source_conn:
             curr_source_conn.rollback()
         if curr_target_conn:
             curr_target_conn.rollback()
-        err_msg = _db_except_msg(exception=e,
-                                 engine=source_engine)
+        err_msg = _except_msg(exception=e,
+                              engine=source_engine)
     finally:
         # close the connections, if locally acquired
         if curr_source_conn and not source_conn:
             curr_source_conn.close()
         if curr_target_conn and not target_conn:
             curr_target_conn.close()
 
     # log the migration finish
-    _db_log(logger=logger,
-            engine=source_engine,
-            err_msg=err_msg,
-            errors=op_errors,
-            stmt=(f"Migrated {result} tuples, "
+    _log(logger=logger,
+         engine=source_engine,
+         err_msg=err_msg,
+         errors=op_errors,
+         stmt=(f"Migrated {result} tuples, "
                   f"from {source_engine}.{source_table} "
                   f"to {target_engine}.{target_table}"))
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
@@ -270,36 +270,36 @@
     source_pks: str = ", ".join(source_pk_columns)
     sel_stmt: str = f"SELECT {source_pks}, {source_lob_column} FROM {source_table}"
     if where_clause:
         sel_stmt += f" WHERE {where_clause}"
     blob_index: int = len(source_pk_columns)
 
     # build the UPDATE query
-    target_where_columns: str = _db_bind_columns(engine=target_engine,
-                                                 columns=target_pk_columns,
-                                                 concat=" AND ",
-                                                 start_index=2)
+    target_where_columns: str = _bind_columns(engine=target_engine,
+                                              columns=target_pk_columns,
+                                              concat=" AND ",
+                                              start_index=2)
     if target_engine == "oracle":
         update_stmt: str = (f"UPDATE {target_table} "
                             f"SET {target_lob_column} = empty_blob() "
                             f"WHERE {target_where_columns} "
                             f"RETURNING {target_lob_column} INTO :{len(target_where_columns) + 2}")
     else:
-        lob_bind: str = _db_bind_columns(engine=target_engine,
-                                         columns=[target_lob_column],
-                                         concat=", ",
-                                         start_index=1)
+        lob_bind: str = _bind_columns(engine=target_engine,
+                                      columns=[target_lob_column],
+                                      concat=", ",
+                                      start_index=1)
         update_stmt: str = (f"UPDATE {target_table} "
                             f"SET {target_lob_column} = {target_lob_column} || {lob_bind[len(target_lob_column) + 3:]} "
                             f"WHERE {target_where_columns}")
 
     # log the migration start
-    _db_log(logger=logger,
-            engine=source_engine,
-            stmt=(f"Started migrating LOBs, "
+    _log(logger=logger,
+         engine=source_engine,
+         stmt=(f"Started migrating LOBs, "
                   f"from {source_engine}.{source_table}.{source_lob_column} "
                   f"to {target_engine}.{target_table}.{target_lob_column}"))
 
     # migrate the LOBs
     err_msg: str | None = None
     try:
         source_cursor: Any = curr_source_conn.cursor()
@@ -368,46 +368,46 @@
 
             # increment the LOB migration counter, if applicable
             if has_data:
                 result += 1
 
             # log partial result at each 100000 LOBs migrated
             if result % 10000 == 0:
-                _db_log(logger=logger,
-                        engine=source_engine,
-                        stmt=(f"Migrated {result} LOBs, "
+                _log(logger=logger,
+                     engine=source_engine,
+                     stmt=(f"Migrated {result} LOBs, "
                               f"from {source_engine}.{source_table}.{source_lob_column} "
                               f"to {target_engine}.{target_table}.{target_lob_column}"))
 
         # close the cursors and commit the transactions
         source_cursor.close()
         curr_source_conn.commit()
         target_cursor.close()
         curr_target_conn.commit()
     except Exception as e:
         # rollback the transactions
         if curr_source_conn:
             curr_source_conn.rollback()
         if curr_target_conn:
             curr_target_conn.rollback()
-        err_msg = _db_except_msg(exception=e,
-                                 engine=source_engine)
+        err_msg = _except_msg(exception=e,
+                              engine=source_engine)
     finally:
         # close the connections, if locally acquired
         if curr_source_conn and not source_conn:
             curr_source_conn.close()
         if curr_target_conn and not target_conn:
             curr_target_conn.close()
 
     # log the migration finish
-    _db_log(logger=logger,
-            engine=source_engine,
-            err_msg=err_msg,
-            errors=op_errors,
-            stmt=(f"Migrated {result} LOBs, "
+    _log(logger=logger,
+         engine=source_engine,
+         err_msg=err_msg,
+         errors=op_errors,
+         stmt=(f"Migrated {result} LOBs, "
                   f"from {source_engine}.{source_table}.{source_lob_column} "
                   f"to {target_engine}.{target_table}.{target_lob_column}"))
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
```

### Comparing `pypomes_db-0.8.9/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.9.0/src/pypomes_db/oracle_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import oracledb
 from logging import Logger
 from oracledb import Connection, init_oracle_client
 from pathlib import Path
 
 from .db_common import (
     _DB_CONN_DATA,
-    _db_assert_query_quota, _db_get_params, _db_log, _db_except_msg
+    _assert_query_quota, _get_params, _log, _except_msg
 )
 
 
 def connect(errors: list[str],
             autocommit: bool,
             logger: Logger) -> Connection:
     """
@@ -21,36 +21,36 @@
     :param logger: optional logger
     :return: the connection to the database
     """
     # initialize the return variable
     result: Connection | None = None
 
     # retrieve the connection parameters
-    name, user, pwd, host, port = _db_get_params("oracle")
+    name, user, pwd, host, port = _get_params("oracle")
 
     # obtain a connection to the database
     err_msg: str | None = None
     try:
         result = oracledb.connect(service_name=name,
                                   host=host,
                                   port=port,
                                   user=user,
                                   password=pwd)
         # establish the connection's autocommit mode
         result.autocommit = autocommit
     except Exception as e:
-        err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+        err_msg = _except_msg(exception=e,
+                              engine="oracle")
 
     # log the results
-    _db_log(logger=logger,
-            engine="oracle",
-            err_msg=err_msg,
-            errors=errors,
-            stmt=f"Connecting to '{name}' at '{host}'")
+    _log(logger=logger,
+         engine="oracle",
+         err_msg=err_msg,
+         errors=errors,
+         stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
 def select_all(errors: list[str],
                sel_stmt: str,
                where_vals: tuple,
@@ -95,45 +95,45 @@
             # execute the query
             cursor.execute(statement=sel_stmt,
                            parameters=where_vals)
             # obtain the number of tuples returned
             count: int = cursor.rowcount
 
             # has the query quota been satisfied ?
-            if _db_assert_query_quota(errors=errors,
-                                      engine="oracle",
-                                      query=sel_stmt,
-                                      where_vals=where_vals,
-                                      count=count,
-                                      require_min=require_min,
-                                      require_max=require_max):
+            if _assert_query_quota(errors=errors,
+                                   engine="oracle",
+                                   query=sel_stmt,
+                                   where_vals=where_vals,
+                                   count=count,
+                                   require_min=require_min,
+                                   require_max=require_max):
                 # yes, retrieve the returned tuples
                 rows: list = cursor.fetchall()
                 result = [tuple(row) for row in rows]
         # commit the transaction, if appropriate
         if committable or not conn:
             curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
-        err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+        err_msg = _except_msg(exception=e,
+                              engine="oracle")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
-        _db_log(logger=logger,
-                engine="oracle",
-                err_msg=err_msg,
-                errors=errors,
-                stmt=sel_stmt,
-                bind_vals=where_vals)
+        _log(logger=logger,
+             engine="oracle",
+             err_msg=err_msg,
+             errors=errors,
+             stmt=sel_stmt,
+             bind_vals=where_vals)
 
     return result
 
 
 def execute(errors: list[str],
             exc_stmt: str,
             bind_vals: tuple,
@@ -177,29 +177,29 @@
 
         # commit the transaction, if appropriate
         if committable or not conn:
             curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
-        err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+        err_msg = _except_msg(exception=e,
+                              engine="oracle")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
-        _db_log(logger=logger,
-                engine="oracle",
-                err_msg=err_msg,
-                errors=errors,
-                stmt=exc_stmt,
-                bind_vals=bind_vals)
+        _log(logger=logger,
+             engine="oracle",
+             err_msg=err_msg,
+             errors=errors,
+             stmt=exc_stmt,
+             bind_vals=bind_vals)
 
     return result
 
 
 def bulk_execute(errors: list[str],
                  exc_stmt: str,
                  exc_vals: list[tuple],
@@ -241,29 +241,29 @@
 
         # commit the transaction, if appropriate
         if committable or not conn:
             curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
-        err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+        err_msg = _except_msg(exception=e,
+                              engine="oracle")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
-        _db_log(logger=logger,
-                engine="oracle",
-                err_msg=err_msg,
-                errors=errors,
-                stmt=exc_stmt,
-                bind_vals=exc_vals[0])
+        _log(logger=logger,
+             engine="oracle",
+             err_msg=err_msg,
+             errors=errors,
+             stmt=exc_stmt,
+             bind_vals=exc_vals[0])
 
     return result
 
 
 def update_lob(errors: list[str],
                lob_table: str,
                lob_column: str,
@@ -324,29 +324,29 @@
 
         # commit the transaction, if appropriate
         if committable or not conn:
             curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
-        err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+        err_msg = _except_msg(exception=e,
+                              engine="oracle")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
-        _db_log(logger=logger,
-                err_msg=err_msg,
-                engine="oracle",
-                errors=errors,
-                stmt=update_stmt,
-                bind_vals=pk_vals)
+        _log(logger=logger,
+             err_msg=err_msg,
+             engine="oracle",
+             errors=errors,
+             stmt=update_stmt,
+             bind_vals=pk_vals)
 
 
 # TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
 # noinspection PyUnusedLocal
 def call_function(errors: list[str],
                   func_name: str,
                   func_vals: tuple,
@@ -409,29 +409,29 @@
 
         # commit the transaction, if appropriate
         if committable or not conn:
             curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
-        err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+        err_msg = _except_msg(exception=e,
+                              engine="oracle")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
-        _db_log(logger=logger,
-                engine="oracle",
-                err_msg=err_msg,
-                errors=errors,
-                stmt=proc_name,
-                bind_vals=proc_vals)
+        _log(logger=logger,
+             engine="oracle",
+             err_msg=err_msg,
+             errors=errors,
+             stmt=proc_name,
+             bind_vals=proc_vals)
 
     return result
 
 __is_initialized: str | None = None
 
 def initialize(errors: list[str],
                logger: Logger) -> bool:
@@ -450,17 +450,17 @@
         err_msg: str | None = None
         client: str = _DB_CONN_DATA["oracle"]["client"]
         try:
             init_oracle_client(client)
             __is_initialized = True
         except Exception as e:
             result = False
-            err_msg = _db_except_msg(exception=e,
-                                     engine="oracle")
+            err_msg = _except_msg(exception=e,
+                                  engine="oracle")
         # log the results
-        _db_log(logger=logger,
-                engine="oracle",
-                err_msg=err_msg,
-                errors=errors,
-                stmt="Initializing the client")
+        _log(logger=logger,
+             engine="oracle",
+             err_msg=err_msg,
+             errors=errors,
+             stmt="Initializing the client")
 
     return result
```

### Comparing `pypomes_db-0.8.9/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.9.0/src/pypomes_db/postgres_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from psycopg2 import Binary
 from psycopg2.extras import execute_values
 # noinspection PyProtectedMember
 from psycopg2._psycopg import connection
 from typing import Any
 
 from .db_common import (
-    _db_assert_query_quota, _db_get_params,
-    _db_log, _db_except_msg, _db_remove_nulls
+    _assert_query_quota, _get_params,
+    _log, _except_msg, _remove_nulls
 )
 
 
 def connect(errors: list[str],
             autocommit: bool,
             logger: Logger = None) -> connection:
     """
@@ -25,35 +25,35 @@
     :param logger: optional logger
     :return: the connection to the database
     """
     # initialize the return variable
     result: connection | None = None
 
     # retrieve the connection parameters
-    name, user, pwd, host, port = _db_get_params("postgres")
+    name, user, pwd, host, port = _get_params("postgres")
 
     # obtain a connection to the database
     err_msg: str | None = None
     try:
         result = psycopg2.connect(host=host,
                                   port=port,
                                   database=name,
                                   user=user,
                                   password=pwd)
         # establish the connection's autocommit mode
         result.autocommit = autocommit
     except Exception as e:
-        err_msg = _db_except_msg(e, "postgres")
+        err_msg = _except_msg(e, "postgres")
 
     # log the results
-    _db_log(logger=logger,
-            engine="postgres",
-            err_msg=err_msg,
-            errors=errors,
-            stmt=f"Connecting to '{name}' at '{host}'")
+    _log(logger=logger,
+         engine="postgres",
+         err_msg=err_msg,
+         errors=errors,
+         stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
 def select_all(errors: list[str],
                sel_stmt: str,
                where_vals: tuple,
@@ -97,45 +97,45 @@
         with curr_conn.cursor() as cursor:
             cursor.execute(query=f"{sel_stmt};",
                            vars=where_vals)
             # obtain the number of tuples returned
             count: int = cursor.rowcount
 
             # has the query quota been satisfied ?
-            if _db_assert_query_quota(errors=errors,
-                                      engine="postgres",
-                                      query=sel_stmt,
-                                      where_vals=where_vals,
-                                      count=count,
-                                      require_min=require_min,
-                                      require_max=require_max):
+            if _assert_query_quota(errors=errors,
+                                   engine="postgres",
+                                   query=sel_stmt,
+                                   where_vals=where_vals,
+                                   count=count,
+                                   require_min=require_min,
+                                   require_max=require_max):
                 # yes, retrieve the returned tuples
                 result = list(cursor)
 
         # commit the transaction, if appropriate
         if committable or not conn:
             curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
-        err_msg = _db_except_msg(exception=e,
-                                 engine="postgres")
+        err_msg = _except_msg(exception=e,
+                              engine="postgres")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
-        _db_log(logger=logger,
-                engine="postgres",
-                err_msg=err_msg,
-                errors=errors,
-                stmt=sel_stmt,
-                bind_vals=where_vals)
+        _log(logger=logger,
+             engine="postgres",
+             err_msg=err_msg,
+             errors=errors,
+             stmt=sel_stmt,
+             bind_vals=where_vals)
 
     return result
 
 
 def execute(errors: list[str],
             exc_stmt: str,
             bind_vals: tuple,
@@ -179,29 +179,29 @@
 
         # commit the transaction, if appropriate
         if committable or not conn:
             curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
-        err_msg = _db_except_msg(exception=e,
-                                 engine="postgres")
+        err_msg = _except_msg(exception=e,
+                              engine="postgres")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
-        _db_log(logger=logger,
-                engine="postgres",
-                err_msg=err_msg,
-                errors=errors,
-                stmt=exc_stmt,
-                bind_vals=bind_vals)
+        _log(logger=logger,
+             engine="postgres",
+             err_msg=err_msg,
+             errors=errors,
+             stmt=exc_stmt,
+             bind_vals=bind_vals)
 
     return result
 
 
 def bulk_execute(errors: list[str],
                  exc_stmt: str,
                  exc_vals: list[tuple],
@@ -245,22 +245,22 @@
         if committable or not conn:
             curr_conn.commit()
     except ValueError as e:
         curr_conn.rollback()
         # is the exception ValueError("A string literal cannot contain NUL (0x00) characters.") ?
         if "contain NUL" in e.args[0]:
             # yes, log the occurrence, remove the NULLs, and try again
-            _db_log(logger=logger,
-                    engine="postgres",
-                    level=WARNING,
-                    stmt=f"Found NULLs in values for {exc_stmt}")
+            _log(logger=logger,
+                 engine="postgres",
+                 level=WARNING,
+                 stmt=f"Found NULLs in values for {exc_stmt}")
             # search for NULLs in input data
             cleaned_rows: list[tuple[int, list]] = []
             for inx, vals in enumerate(exc_vals):
-                cleaned_row: list[Any] = _db_remove_nulls(vals)
+                cleaned_row: list[Any] = _remove_nulls(vals)
                 # has the row been cleaned ?
                 if cleaned_row:
                     # yes, register it
                     cleaned_rows.append((inx, cleaned_row))
             # replace the cleaned rows
             for cleaned_row in cleaned_rows:
                 exc_vals[cleaned_row[0]] = tuple(cleaned_row[1])
@@ -270,28 +270,28 @@
                          exc_vals=exc_vals,
                          conn=conn,
                          committable=committable,
                          logger=logger)
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
-        err_msg = _db_except_msg(exception=e,
-                                 engine="postgres")
+        err_msg = _except_msg(exception=e,
+                              engine="postgres")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
-        _db_log(logger=logger,
-                engine="postgres",
-                err_msg=err_msg,
-                errors=errors,
-                stmt=exc_stmt)
+        _log(logger=logger,
+             engine="postgres",
+             err_msg=err_msg,
+             errors=errors,
+             stmt=exc_stmt)
 
     return result
 
 
 def update_lob(errors: list[str],
                lob_table: str,
                lob_column: str,
@@ -349,29 +349,29 @@
 
         # commit the transaction, if appropriate
         if committable or not conn:
             curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
-        err_msg = _db_except_msg(exception=e,
-                                 engine="postgres")
+        err_msg = _except_msg(exception=e,
+                              engine="postgres")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
-        _db_log(logger=logger,
-                engine="postgres",
-                err_msg=err_msg,
-                errors=errors,
-                stmt=update_stmt,
-                bind_vals=pk_vals)
+        _log(logger=logger,
+             engine="postgres",
+             err_msg=err_msg,
+             errors=errors,
+             stmt=update_stmt,
+             bind_vals=pk_vals)
 
 
 def call_procedure(errors: list[str],
                    proc_name: str,
                    proc_vals: tuple,
                    conn: connection,
                    committable: bool,
@@ -410,24 +410,24 @@
 
         # commit the transaction, if appropriate
         if committable or not conn:
             curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
-        err_msg = _db_except_msg(exception=e,
-                                 engine="postgres")
+        err_msg = _except_msg(exception=e,
+                              engine="postgres")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
-        _db_log(logger=logger,
-                engine="postgres",
-                err_msg=err_msg,
-                errors=errors,
-                stmt=proc_stmt,
-                bind_vals=proc_vals)
+        _log(logger=logger,
+             engine="postgres",
+             err_msg=err_msg,
+             errors=errors,
+             stmt=proc_stmt,
+             bind_vals=proc_vals)
 
     return result
```

### Comparing `pypomes_db-0.8.9/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.9.0/src/pypomes_db/sqlserver_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # noinspection DuplicatedCode
 import pyodbc
 from logging import Logger
 from pyodbc import Binary, Connection, Row
 from pathlib import Path
 
 from .db_common import (
-    _db_assert_query_quota, _db_get_params, _db_log, _db_except_msg
+    _assert_query_quota, _get_params, _log, _except_msg
 )
 
 
 def connect(errors: list[str],
             autocommit: bool,
             logger: Logger = None) -> Connection:
     """
@@ -20,36 +20,36 @@
     :param logger: optional logger
     :return: the connection to the database
     """
     # initialize the return valiable
     result: Connection | None = None
 
     # retrieve the connection parameters and build the connection string
-    name, user, pwd, host, port, driver = _db_get_params("sqlserver")
+    name, user, pwd, host, port, driver = _get_params("sqlserver")
     connection_kwargs: str = (
         f"DRIVER={{{driver}}};SERVER={host},{port};"
         f"DATABASE={name};UID={user};PWD={pwd};TrustServerCertificate=yes;"
     )
 
     # obtain a connection to the database
     err_msg: str | None = None
     try:
         result = pyodbc.connect(connection_kwargs)
         # establish the connection's autocommit mode
         result.autocommit = autocommit
     except Exception as e:
-        err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
+        err_msg = _except_msg(exception=e,
+                              engine="sqlserver")
 
     # log the results
-    _db_log(logger=logger,
-            engine="sqlserver",
-            err_msg=err_msg,
-            errors=errors,
-            stmt=f"Connecting to '{name}' at '{host}'")
+    _log(logger=logger,
+         engine="sqlserver",
+         err_msg=err_msg,
+         errors=errors,
+         stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
 def select_all(errors: list[str],
                sel_stmt: str,
                where_vals: tuple,
@@ -92,46 +92,46 @@
         # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
             cursor.execute(sel_stmt, where_vals)
             # obtain the number of tuples returned
             count: int = cursor.rowcount
 
             # has the query quota been satisfied ?
-            if _db_assert_query_quota(errors=errors,
-                                      engine="sqlserver",
-                                      query=sel_stmt,
-                                      where_vals=where_vals,
-                                      count=count,
-                                      require_min=require_min,
-                                      require_max=require_max):
+            if _assert_query_quota(errors=errors,
+                                   engine="sqlserver",
+                                   query=sel_stmt,
+                                   where_vals=where_vals,
+                                   count=count,
+                                   require_min=require_min,
+                                   require_max=require_max):
                 # yes, retrieve the returned tuples
                 rows: list[Row] = cursor.fetchall()
                 result = [tuple(row) for row in rows]
 
         # commit the transaction, if appropriate
         if committable or not conn:
             curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
-        err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
+        err_msg = _except_msg(exception=e,
+                              engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
-        _db_log(logger=logger,
-                engine="sqlserver",
-                err_msg=err_msg,
-                errors=errors,
-                stmt=sel_stmt,
-                bind_vals=where_vals)
+        _log(logger=logger,
+             engine="sqlserver",
+             err_msg=err_msg,
+             errors=errors,
+             stmt=sel_stmt,
+             bind_vals=where_vals)
 
     return result
 
 
 def execute(errors: list[str],
             exc_stmt: str,
             bind_vals: tuple,
@@ -174,29 +174,29 @@
 
         # commit the transaction, if appropriate
         if committable or not conn:
             curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
-        err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
+        err_msg = _except_msg(exception=e,
+                              engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
-        _db_log(logger=logger,
-                engine="sqlserver",
-                err_msg=err_msg,
-                errors=errors,
-                stmt=exc_stmt,
-                bind_vals=bind_vals)
+        _log(logger=logger,
+             engine="sqlserver",
+             err_msg=err_msg,
+             errors=errors,
+             stmt=exc_stmt,
+             bind_vals=bind_vals)
 
     return result
 
 
 def bulk_execute(errors: list[str],
                  exc_stmt: str,
                  exc_vals: list[tuple],
@@ -241,29 +241,29 @@
 
         # commit the transaction, if appropriate
         if committable or not conn:
             curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
-        err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
+        err_msg = _except_msg(exception=e,
+                              engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
-        _db_log(logger=logger,
-                engine="sqlserver",
-                err_msg=err_msg,
-                errors=errors,
-                stmt=exc_stmt,
-                bind_vals=exc_vals[0])
+        _log(logger=logger,
+             engine="sqlserver",
+             err_msg=err_msg,
+             errors=errors,
+             stmt=exc_stmt,
+             bind_vals=exc_vals[0])
 
     return result
 
 
 def update_lob(errors: list[str],
                lob_table: str,
                lob_column: str,
@@ -321,29 +321,29 @@
 
         # commit the transaction, if appropriate
         if committable or not conn:
             curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
-        err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
+        err_msg = _except_msg(exception=e,
+                              engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
-        _db_log(logger=logger,
-                engine="sqlserver",
-                err_msg=err_msg,
-                errors=errors,
-                stmt=update_stmt,
-                bind_vals=pk_vals)
+        _log(logger=logger,
+             engine="sqlserver",
+             err_msg=err_msg,
+             errors=errors,
+             stmt=update_stmt,
+             bind_vals=pk_vals)
 
 
 def call_procedure(errors: list[str],
                    proc_name: str,
                    proc_vals: tuple,
                    conn: Connection,
                    committable: bool,
@@ -383,24 +383,24 @@
 
         # commit the transaction, if appropriate
         if committable or not conn:
             curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
-        err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
+        err_msg = _except_msg(exception=e,
+                              engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
-        _db_log(logger=logger,
-                engine="sqlserver",
-                err_msg=err_msg,
-                errors=errors,
-                stmt=proc_stmt,
-                bind_vals=proc_vals)
+        _log(logger=logger,
+             engine="sqlserver",
+             err_msg=err_msg,
+             errors=errors,
+             stmt=proc_stmt,
+             bind_vals=proc_vals)
 
     return result
```

### Comparing `pypomes_db-0.8.9/LICENSE` & `pypomes_db-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.9/pyproject.toml` & `pypomes_db-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.8.9"
+version = "0.9.0"
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
 #   "oracledb>=2.2.0",
 #   "psycopg2-binary>=2.9.9",
 #   "pyodbc>=5.1.0",
-    "pypomes_core>=1.0.7",
+    "pypomes_core>=1.1.3",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-DB"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes-DB/issues"
```

### Comparing `pypomes_db-0.8.9/PKG-INFO` & `pypomes_db-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.8.9
+Version: 0.9.0
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
-Requires-Dist: pypomes-core>=1.0.7
+Requires-Dist: pypomes-core>=1.1.3
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
```

