# Comparing `tmp/harlequin_databend-0.1.17.tar.gz` & `tmp/harlequin_databend-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harlequin_databend-0.1.17.tar", max compression
+gzip compressed data, was "harlequin_databend-0.1.2.tar", max compression
```

## Comparing `harlequin_databend-0.1.17.tar` & `harlequin_databend-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0     1463 2024-05-30 06:52:19.611002 harlequin_databend-0.1.17/README.md
--rwxr-xr-x   0        0        0     1514 2024-05-31 09:45:43.430335 harlequin_databend-0.1.17/pyproject.toml
--rwxr-xr-x   0        0        0      104 2024-05-30 06:52:19.620915 harlequin_databend-0.1.17/src/harlequin_databend/__init__.py
--rwxr-xr-x   0        0        0     8247 2024-05-31 09:45:27.260309 harlequin_databend-0.1.17/src/harlequin_databend/adapter.py
--rwxr-xr-x   0        0        0     1210 2024-05-31 08:46:59.222723 harlequin_databend-0.1.17/src/harlequin_databend/cli_options.py
--rwxr-xr-x   0        0        0     1397 2024-05-30 06:52:19.631028 harlequin_databend-0.1.17/src/harlequin_databend/completions.py
--rwxr-xr-x   0        0        0        0 2024-05-30 06:52:19.640940 harlequin_databend-0.1.17/src/harlequin_databend/py.typed
--rw-r--r--   0        0        0     2208 1970-01-01 00:00:00.000000 harlequin_databend-0.1.17/PKG-INFO
+-rw-r--r--   0        0        0     1463 2024-05-27 16:58:44.635010 harlequin_databend-0.1.2/README.md
+-rw-r--r--   0        0        0     1472 2024-05-30 17:14:10.779529 harlequin_databend-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      104 2024-05-27 13:37:37.195474 harlequin_databend-0.1.2/src/harlequin_databend/__init__.py
+-rw-r--r--   0        0        0     7197 2024-05-27 16:20:29.051820 harlequin_databend-0.1.2/src/harlequin_databend/adapter.py
+-rw-r--r--   0        0        0     1172 2024-05-26 09:35:57.962231 harlequin_databend-0.1.2/src/harlequin_databend/cli_options.py
+-rw-r--r--   0        0        0     1397 2024-05-27 16:20:39.840201 harlequin_databend-0.1.2/src/harlequin_databend/completions.py
+-rw-r--r--   0        0        0        0 2024-05-26 09:00:04.820057 harlequin_databend-0.1.2/src/harlequin_databend/py.typed
+-rw-r--r--   0        0        0     2121 1970-01-01 00:00:00.000000 harlequin_databend-0.1.2/PKG-INFO
```

### Comparing `harlequin_databend-0.1.17/README.md` & `harlequin_databend-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `harlequin_databend-0.1.17/pyproject.toml` & `harlequin_databend-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 [tool.poetry]
 name = "harlequin-databend"
-version = "0.1.17"
+version = "0.1.2"
 description = "A Harlequin adapter for Databend."
 authors = ["hanxuanliang <hxuanliang@163.com>"]
 license = "MIT"
 keywords = ["databend", "harlequin"]
 homepage = "https://github.com/datafuselabs/databend"
 readme = "README.md"
 packages = [{ include = "harlequin_databend", from = "src" }]
 
 [tool.poetry.plugins."harlequin.adapter"]
 databend = "harlequin_databend:HarlequinDatabendAdapter"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
+harlequin = "^1.7"
 databend-py = "^0.6.0"
-harlequin = "^1.20.0"
-pandas = "^2.2.2"
-pyarrow = "^16.1.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.1.6"
 pytest = "^7.4.3"
 mypy = "^1.7.0"
 pre-commit = "^3.5.0"
 importlib_metadata = { version = ">=4.6.0", python = "<3.10.0" }
```

### Comparing `harlequin_databend-0.1.17/src/harlequin_databend/adapter.py` & `harlequin_databend-0.1.2/src/harlequin_databend/adapter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,51 @@
 from __future__ import annotations
 
-from typing import Any, List, Sequence, Tuple
+import os
+from typing import Any, Dict, List, Sequence, Tuple
 
-import pandas as pd
-import pyarrow
 from databend_py import Client
 from harlequin import (
     HarlequinAdapter,
     HarlequinCompletion,
     HarlequinConnection,
     HarlequinCursor,
 )
 from harlequin.catalog import Catalog, CatalogItem
 from harlequin.exception import HarlequinConnectionError
-from textual_fastdatatable.backend import AutoBackendType
 
 from harlequin_databend.cli_options import DATABEND_OPTIONS
 from harlequin_databend.completions import _get_completions
 
 
-class HarlequinDatabendCursor(HarlequinCursor):
-    def __init__(self, conn: HarlequinDatabendConnection, query: str) -> None:
-        self.results = conn.execute(query, with_column_types=True)
-        self._limit: int | None = None
-
-    def columns(self) -> list[tuple[str, str]]:
-        return self.results[0]
-
-    def set_limit(self, limit: int) -> HarlequinDatabendCursor:
-        self._limit = limit
-        return self
-
-    def fetchall(self) -> AutoBackendType | None:
-        return pyarrow.Table.from_pandas(
-            pd.DataFrame(
-                data=[list(row) for row in self.results[1]],
-                columns=[col[0] for col in self.results[0]],
-            )
-        )
-
-
 class HarlequinDatabendConnection(HarlequinConnection):
-    def __init__(
-        self,
-        conn_str: Sequence[str],
-        *_: Any,
-        init_message: str = "",
-        options: dict[str, Any],
-    ) -> None:
-        self.init_message = "Hello from Databend!" if not init_message else init_message
+    def __init__(self, conn_str: Sequence[str], options: Dict[str, Any]) -> None:
+        self.init_message = "Hello from Databend!"
         try:
             if conn_str and conn_str[0]:
                 self.conn = Client(conn_str[0])
             else:
-                hostname = options.get("host", "127.0.0.1")
+                hostname = options.get("host", "localhost")
                 database = options.get("dbname", "default")
-                port = options.get("port", "8000")
-                username = options.get("user", None)
+                username = options.get("user", "")
                 password = options.get("password", None)
                 self.conn = Client(
                     host=hostname,
-                    port=int(port) if port is not None else 8000,
                     database=database,
-                    user=username if username else "",
-                    password=password if password else "",
+                    user=username,
+                    password=password if password else os.environ["DATABEND_PASSWORD"],
                 )
 
         except Exception as e:
             raise HarlequinConnectionError(
-                msg=str(e),
-                title="Harlequin could not connect to databend.",
+                msg=str(e), title="Harlequin could not connect to databend."
             ) from e
 
     def execute(self, query: str) -> HarlequinCursor:
-        return HarlequinDatabendCursor(self.conn, query)
+        return self.conn.execute(query)
 
     def get_catalog(self) -> Catalog:
         databases = self._get_databases()
         db_items: List[CatalogItem] = []
 
         for (db,) in databases:
             schemas = self._get_schemas(db)
@@ -114,17 +82,17 @@
 
     def _get_schemas(self, dbname: str) -> List[Tuple[str]]:
         _, res = self.conn.execute(
             f"""
             select schema_name
             from information_schema.schemata
             where
-                catalog_name = '{dbname}'
-                and schema_name != 'information_schema'
-            order by schema_name asc
+                table_catalog = '{dbname}'
+                and table_schema != 'information_schema'
+            order by table_schema asc
             ;"""
         )
         return res
 
     def _get_table(
         self,
         dbname: str,
@@ -227,19 +195,19 @@
 
 class HarlequinDatabendAdapter(HarlequinAdapter):
     ADAPTER_OPTIONS = DATABEND_OPTIONS
 
     def __init__(
         self,
         conn_str: Sequence[str],
-        host: str | None = None,
-        port: str | None = None,
-        dbname: str | None = None,
-        user: str | None = None,
-        password: str | None = None,
+        host: str = "localhost",
+        port: str = "8000",
+        dbname: str = "default",
+        user: str = None,
+        password: str = None,
         **_: Any,
     ) -> None:
         self.conn_str = conn_str
         self.options = {
             "host": host,
             "port": port,
             "dbname": dbname,
```

### Comparing `harlequin_databend-0.1.17/src/harlequin_databend/cli_options.py` & `harlequin_databend-0.1.2/src/harlequin_databend/cli_options.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,37 +6,36 @@
     name="host",
     description=(
         "Specifies the host name of the machine on which the server is running. "
         "If the value begins with a slash, it is used as the directory for the "
         "Unix-domain socket."
     ),
     short_decls=["-h"],
-    default="127.0.0.1",
+    default="localhost",
 )
 
 
 port = TextOption(
     name="port",
     description=(
         "Port number to connect to at the server host, or socket file name extension "
         "for Unix-domain connections."
     ),
-    short_decls=["-P", "--port"],
+    short_decls=["-p"],
     default="8000",
 )
 
 user = TextOption(
     name="user",
     description=("databend user name to connect as."),
-    short_decls=["-U", "--user"],
+    short_decls=["-u", "--username", "-U"],
 )
 
 password = TextOption(
     name="password",
-    short_decls=["-p", "--password"],
     description=("Password to be used if the server demands password authentication."),
 )
 
 
 dbname = TextOption(
     name="dbname",
     description=(
```

### Comparing `harlequin_databend-0.1.17/src/harlequin_databend/completions.py` & `harlequin_databend-0.1.2/src/harlequin_databend/completions.py`

 * *Files identical despite different names*

### Comparing `harlequin_databend-0.1.17/PKG-INFO` & `harlequin_databend-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: harlequin-databend
-Version: 0.1.17
+Version: 0.1.2
 Summary: A Harlequin adapter for Databend.
 Home-page: https://github.com/datafuselabs/databend
 License: MIT
 Keywords: databend,harlequin
 Author: hanxuanliang
 Author-email: hxuanliang@163.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: databend-py (>=0.6.0,<0.7.0)
-Requires-Dist: harlequin (>=1.20.0,<2.0.0)
-Requires-Dist: pandas (>=2.2.2,<3.0.0)
-Requires-Dist: pyarrow (>=16.1.0,<17.0.0)
+Requires-Dist: harlequin (>=1.7,<2.0)
 Description-Content-Type: text/markdown
 
 # harlequin-databend
 
 This repo provides the Harlequin adapter for [Databend](https://github.com/datafuselabs/databend).
 
 ## Installation
```

