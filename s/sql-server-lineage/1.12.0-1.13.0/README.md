# Comparing `tmp/sql_server_lineage-1.12.0-cp39-cp39-win_amd64.whl.zip` & `tmp/sql_server_lineage-1.13.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,12 @@
-Zip file size: 1520452 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat     2146 b- defN 24-May-24 08:48 _sql_server_lineage.cp39-win_amd64.h
--rw-rw-rw-  2.0 fat  4504655 b- defN 24-May-24 08:48 _sql_server_lineage.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     3774 b- defN 24-May-24 08:43 sql_server_lineage.py
--rw-rw-rw-  2.0 fat     1090 b- defN 24-May-24 08:48 sql_server_lineage-1.12.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4979 b- defN 24-May-24 08:48 sql_server_lineage-1.12.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-May-24 08:48 sql_server_lineage-1.12.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       39 b- defN 24-May-24 08:48 sql_server_lineage-1.12.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      716 b- defN 24-May-24 08:48 sql_server_lineage-1.12.0.dist-info/RECORD
-8 files, 4517499 bytes uncompressed, 1519194 bytes compressed:  66.4%
+Zip file size: 1396086 bytes, number of entries: 10
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-31 07:17 sql_server_lineage.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-31 07:17 sql_server_lineage-1.13.0.dist-info/
+-rw-r--r--  2.0 unx     2080 b- defN 24-May-31 07:17 _sql_server_lineage.cpython-310-aarch64-linux-gnu.h
+-rw-r--r--  2.0 unx  2595400 b- defN 24-May-31 07:17 _sql_server_lineage.cpython-310-aarch64-linux-gnu.so
+-rw-r--r--  2.0 unx     3670 b- defN 24-May-31 07:17 sql_server_lineage.py
+-rw-r--r--  2.0 unx      154 b- defN 24-May-31 07:17 sql_server_lineage-1.13.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1070 b- defN 24-May-31 07:17 sql_server_lineage-1.13.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx       39 b- defN 24-May-31 07:17 sql_server_lineage-1.13.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      753 b- defN 24-May-31 07:17 sql_server_lineage-1.13.0.dist-info/RECORD
+-rw-r--r--  2.0 unx     4863 b- defN 24-May-31 07:17 sql_server_lineage-1.13.0.dist-info/METADATA
+10 files, 2608029 bytes uncompressed, 1394498 bytes compressed:  46.5%
```

## zipnote {}

```diff
@@ -1,25 +1,31 @@
-Filename: _sql_server_lineage.cp39-win_amd64.h
+Filename: sql_server_lineage.libs/
 Comment: 
 
-Filename: _sql_server_lineage.cp39-win_amd64.pyd
+Filename: sql_server_lineage-1.13.0.dist-info/
+Comment: 
+
+Filename: _sql_server_lineage.cpython-310-aarch64-linux-gnu.h
+Comment: 
+
+Filename: _sql_server_lineage.cpython-310-aarch64-linux-gnu.so
 Comment: 
 
 Filename: sql_server_lineage.py
 Comment: 
 
-Filename: sql_server_lineage-1.12.0.dist-info/LICENSE
+Filename: sql_server_lineage-1.13.0.dist-info/WHEEL
 Comment: 
 
-Filename: sql_server_lineage-1.12.0.dist-info/METADATA
+Filename: sql_server_lineage-1.13.0.dist-info/LICENSE
 Comment: 
 
-Filename: sql_server_lineage-1.12.0.dist-info/WHEEL
+Filename: sql_server_lineage-1.13.0.dist-info/top_level.txt
 Comment: 
 
-Filename: sql_server_lineage-1.12.0.dist-info/top_level.txt
+Filename: sql_server_lineage-1.13.0.dist-info/RECORD
 Comment: 
 
-Filename: sql_server_lineage-1.12.0.dist-info/RECORD
+Filename: sql_server_lineage-1.13.0.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## sql_server_lineage.py

 * *Ordering differences only*

```diff
@@ -1,104 +1,104 @@
-from ctypes import cdll, POINTER, c_char_p, c_int, Array, CDLL, Structure
-from typing import Dict, List
-from distutils.sysconfig import get_config_var
-from pathlib import Path
-import json
-
-class Error(Structure):
-    _fields_ = [('err', c_char_p)]
-
-    def __del__(self):
-        # Free the memory allocated to error.
-        if self.err is not None:
-            del_error(self)
-
-    def raise_if_err(self):
-        if self.err is not None:
-            raise IOError(self.err.decode())
-
-
-class Lineage(Structure):
-    # Multiple return values can be grabbed in a struct.
-    _fields_ = [
-        ('lineage', c_char_p),
-        ('err', Error),
-    ]
-
-# Location of shared library
-here = Path(__file__).absolute().parent
-ext_suffix = get_config_var('EXT_SUFFIX')
-so_file = str(here / ('_sql_server_lineage' + ext_suffix))
-print(so_file)
-
-# Load functions from shared library set their signatures
-lib: CDLL = cdll.LoadLibrary(so_file)
-extract_lineage_f = lib.extractLineage
-extract_lineage_f.argtypes = [POINTER(c_char_p), c_int]
-extract_lineage_f.restype = Lineage
-
-del_error = lib.delError
-del_error.argtypes = [Error]
-
-generate_html = lib.generateHtmlLineage
-generate_html.argtypes = [POINTER(c_char_p), c_int, c_char_p]
-generate_html.restype = Error
-
-
-def get_lineage(stored_procedures: List[str]) -> Dict:
-    """Generate the lineage for the stored procedures provided.
-
-    The format of the lineage data structure is the following:
-        {'lineage': {'dbo.sink_table': {'dbo.stored_procedure': ['dbo.source', 'another_schema.another_source']}}}
-    If multiple stored procedures write data to the same table then we will have:
-        {'lineage': {'dbo.sink_table': {'dbo.stored_procedure_1': ['dbo.source'], 'dbo.stored_procedure_2': ['another_schema.another_source']}}}
-
-    Args:
-        - stored_procedures: The list of stored procedures to generate the lineage for.
-
-    Returns:
-        dict: Lineage dictionary.
-
-    Raises:
-        Error: if something went wrong during the lineage generation.
-    """
-    len_array: int = len(stored_procedures)
-    ptr: Array[c_char_p] = (c_char_p * len_array)()
-    ptr[:] = [s.encode() for s in stored_procedures]
-    resultLineage: Lineage = extract_lineage_f(ptr, len_array)
-    resultLineage.err.raise_if_err()
-    lineage_nested: Dict = json.loads(resultLineage.lineage)
-
-    return lineage_nested['lineage']
-
-def generate_html_lineage(stored_procedures: List[str], filename: str = None) -> None:
-    """Generate the lineage html file for the stored procedures provided.
-
-    The html file should be read from left to right:
-        sources -> stored_procedures -> sink_table
-
-    Args:
-        - stored_procedures: The list of stored procedures to generate the lineage for.
-        - filename: Name of the html file, it must include the .html extension.
-
-    Returns:
-        None.
-
-    Raises:
-        ValueError: if .html extension has not been provided or if the extension is not .html
-        Error: if something went wrong during the html generation.
-    """
-    if not filename:
-        filename = "lineage_generated.html"
-    else:
-        splitted: str = filename.split(".")
-        if len(splitted) == 1:
-            raise ValueError("The filename provided should contain .html extension")
-        elif splitted[1] != "html":
-            raise ValueError("The filename provided should contain .html extension")
-        
-    len_array: int = len(stored_procedures)
-    ptr: Array[c_char_p] = (c_char_p * len_array)()
-    ptr[:] = [s.encode() for s in stored_procedures]
-    filename_encoded: bytes = filename.encode()
-    err: Error = generate_html(ptr, len_array, filename_encoded)
-    err.raise_if_err()
+from ctypes import cdll, POINTER, c_char_p, c_int, Array, CDLL, Structure
+from typing import Dict, List
+from distutils.sysconfig import get_config_var
+from pathlib import Path
+import json
+
+class Error(Structure):
+    _fields_ = [('err', c_char_p)]
+
+    def __del__(self):
+        # Free the memory allocated to error.
+        if self.err is not None:
+            del_error(self)
+
+    def raise_if_err(self):
+        if self.err is not None:
+            raise IOError(self.err.decode())
+
+
+class Lineage(Structure):
+    # Multiple return values can be grabbed in a struct.
+    _fields_ = [
+        ('lineage', c_char_p),
+        ('err', Error),
+    ]
+
+# Location of shared library
+here = Path(__file__).absolute().parent
+ext_suffix = get_config_var('EXT_SUFFIX')
+so_file = str(here / ('_sql_server_lineage' + ext_suffix))
+print(so_file)
+
+# Load functions from shared library set their signatures
+lib: CDLL = cdll.LoadLibrary(so_file)
+extract_lineage_f = lib.extractLineage
+extract_lineage_f.argtypes = [POINTER(c_char_p), c_int]
+extract_lineage_f.restype = Lineage
+
+del_error = lib.delError
+del_error.argtypes = [Error]
+
+generate_html = lib.generateHtmlLineage
+generate_html.argtypes = [POINTER(c_char_p), c_int, c_char_p]
+generate_html.restype = Error
+
+
+def get_lineage(stored_procedures: List[str]) -> Dict:
+    """Generate the lineage for the stored procedures provided.
+
+    The format of the lineage data structure is the following:
+        {'lineage': {'dbo.sink_table': {'dbo.stored_procedure': ['dbo.source', 'another_schema.another_source']}}}
+    If multiple stored procedures write data to the same table then we will have:
+        {'lineage': {'dbo.sink_table': {'dbo.stored_procedure_1': ['dbo.source'], 'dbo.stored_procedure_2': ['another_schema.another_source']}}}
+
+    Args:
+        - stored_procedures: The list of stored procedures to generate the lineage for.
+
+    Returns:
+        dict: Lineage dictionary.
+
+    Raises:
+        Error: if something went wrong during the lineage generation.
+    """
+    len_array: int = len(stored_procedures)
+    ptr: Array[c_char_p] = (c_char_p * len_array)()
+    ptr[:] = [s.encode() for s in stored_procedures]
+    resultLineage: Lineage = extract_lineage_f(ptr, len_array)
+    resultLineage.err.raise_if_err()
+    lineage_nested: Dict = json.loads(resultLineage.lineage)
+
+    return lineage_nested['lineage']
+
+def generate_html_lineage(stored_procedures: List[str], filename: str = None) -> None:
+    """Generate the lineage html file for the stored procedures provided.
+
+    The html file should be read from left to right:
+        sources -> stored_procedures -> sink_table
+
+    Args:
+        - stored_procedures: The list of stored procedures to generate the lineage for.
+        - filename: Name of the html file, it must include the .html extension.
+
+    Returns:
+        None.
+
+    Raises:
+        ValueError: if .html extension has not been provided or if the extension is not .html
+        Error: if something went wrong during the html generation.
+    """
+    if not filename:
+        filename = "lineage_generated.html"
+    else:
+        splitted: str = filename.split(".")
+        if len(splitted) == 1:
+            raise ValueError("The filename provided should contain .html extension")
+        elif splitted[1] != "html":
+            raise ValueError("The filename provided should contain .html extension")
+        
+    len_array: int = len(stored_procedures)
+    ptr: Array[c_char_p] = (c_char_p * len_array)()
+    ptr[:] = [s.encode() for s in stored_procedures]
+    filename_encoded: bytes = filename.encode()
+    err: Error = generate_html(ptr, len_array, filename_encoded)
+    err.raise_if_err()
```

## Comparing `_sql_server_lineage.cp39-win_amd64.h` & `_sql_server_lineage.cpython-310-aarch64-linux-gnu.h`

 * *Files 5% similar despite different names*

```diff
@@ -78,20 +78,20 @@
 
 /* End of boilerplate cgo prologue.  */
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
-extern __declspec(dllexport) void delError(error err);
+extern void delError(error err);
 
 /* Return type for extractLineage */
 struct extractLineage_return {
 	char* r0;
 	error r1;
 };
-extern __declspec(dllexport) struct extractLineage_return extractLineage(char** storedProcedures, int length);
-extern __declspec(dllexport) error generateHtmlLineage(char** storedProcedures, int length, char* fileName);
+extern struct extractLineage_return extractLineage(char** storedProcedures, int length);
+extern error generateHtmlLineage(char** storedProcedures, int length, char* fileName);
 
 #ifdef __cplusplus
 }
 #endif
```

## Comparing `sql_server_lineage-1.12.0.dist-info/LICENSE` & `sql_server_lineage-1.13.0.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Ivan Ostymchuk
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2024 Ivan Ostymchuk
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

## Comparing `sql_server_lineage-1.12.0.dist-info/METADATA` & `sql_server_lineage-1.13.0.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-Metadata-Version: 2.1
-Name: sql-server-lineage
-Version: 1.12.0
-Summary: Python library to extract lineage from Sql Server stored procedures
-Author: Ivan Ostymchuk
-License: MIT
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# sql-server-lineage
-
-I worked many times on sql server data warehouses or or sql server application databases with almost   
-no documentation and lots of stored procedures transforming data. At some point I wanted a tool that would   
-analyse all the stored procedures and generate a lineage that I would be able to send to a Data Catalog or   
-visualise immediately to get an idea of the structure and debug much more easily. So I decided to develop it.
-
-This is a library available in Golang and Python that would enable you to do 2 things:
-- Get the lineage of all the stored procedures in a database as python dictionary.
-- Generate an html file with the lineage visualised (That you can share on Google Pages or Github Pages or wherever you like).
-
-CTEs (deeply nested as well), Temp Tables, Table Variables are all handled gracefully. You'll always see the original source tables.
-
-The resulting lineage structure is the following:
-    sink_table -> stored_procedure (1 or more) -> list_of_sources
-
-Dictionary Example:
-```
-{
-    'db_name.schema.table_sink': {
-        'schema.stored_procedure_1': [
-            'schema.table_source_1',
-            'schema.table_source_2',
-            'schema.table_source_3',
-        ],
-        'schema.stored_procedure_2': [
-            'schema.table_source_a',
-            'schema.table_source_b',
-            'schema.table_source_c',
-        ],
-    },
-    'db_name.schema.table_sink_2': {
-        'schema.stored_procedure_3': [
-            'schema.table_source',
-        ],
-    },
-}
-```
-
-Html Example:
-
-![Sample Image](https://github.com/ivan-ostymchuk/sql-server-lineage/blob/main/lineage_example.png)
-
-Therefore, everything is centered around the sink_table. Because most likely you want to see for each table where does the data come from. If you need it different (for a Data Catalog) you can transform the objects and adapt them to your requirement.
-In the html you will see the sink table as reference in a different color (green) and you will see it again in the lineage.
-
-I decided to generate html files instead of starting a local server (like DBT does) because I wanted to keep it simple and make it easy to host somewhere as a static website and therefore sharing it with other Data Engineers, Data Analysts, etc.
-
-This project is named sql-server-lineage because I want to keep it specialised only on Sql Server. To generate the lineage you need to develop a custom implementation of a Sql parser. I did it for Sql Server as I've been using it recently but I do not intend to develop parsers for other sql dialects.
-
-# DISCLAIMER
-Since this library analyses stored procedures, if you transform data externally and then write it to the database there is nothing you can do for the lineage. Also if the stored procedures rely heavily on dynamic sql especially with table names passed as parameters then the library would not be able to determine the table names for the lineage.
-
-# Implementation
-
-All the core logic is developed in Go, then using CGO, C bindings and some adapter functions I made it available also as a Python library.
-The main reason to do that was because Data Engineers work mainly in Python.
-
-# Get Started
-
-### Installation
-```
-pip install sql-server-lineage
-```
-
-### Example to generate the lineage directly from sql server
-In this example we get the stored procedures definitions from sql server
-but you can also read the definitions from files.
-
-```
-from sql_server_lineage import get_lineage, generate_html_lineage
-from typing import Dict, List
-import pyodbc
-
-host: str = "host"
-port: str = "port"
-driver: str = "driver"
-user: str = "user"
-password: str = "password"
-database: str = "database"
-otherparams: str = "otherparams"
-
-db_conn_string: str = f"DRIVER={{{driver}}};SERVER={host};PORT={port};DATABASE={database};UID={user};PWD={password};{otherparams}"
-conn: pyodbc.Connection = pyodbc.connect(db_conn_string)
-
-sql_query: str = """
-    SELECT OBJECT_DEFINITION(object_id) as sp_definition
-    FROM sys.procedures
-    WHERE object_id not in (select major_id from sys.extended_properties);
-"""
-
-cursor = conn.cursor()
-cursor.execute(sql_query)
-records: List = cursor.fetchall()
-stored_procedures: List[str] = [r.sp_definition for r in records]
-
-# get lineage and then send it to a Data Catalog, or transform and then send.
-result_lineage: Dict = get_lineage(stored_procedures)
-
-# generate the html representation of the lineage
-# providing the filename is optional
-lineage_file: str = "lineage_generated.html"
-generate_html_lineage(stored_procedures, lineage_file)
-```
-
-This project operates under the MIT License.
+Metadata-Version: 2.1
+Name: sql-server-lineage
+Version: 1.13.0
+Summary: Python library to extract lineage from Sql Server stored procedures
+Author: Ivan Ostymchuk
+License: MIT
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# sql-server-lineage
+
+I worked many times on sql server data warehouses or or sql server application databases with almost   
+no documentation and lots of stored procedures transforming data. At some point I wanted a tool that would   
+analyse all the stored procedures and generate a lineage that I would be able to send to a Data Catalog or   
+visualise immediately to get an idea of the structure and debug much more easily. So I decided to develop it.
+
+This is a library available in Golang and Python that would enable you to do 2 things:
+- Get the lineage of all the stored procedures in a database as python dictionary.
+- Generate an html file with the lineage visualised (That you can share on Google Pages or Github Pages or wherever you like).
+
+CTEs (deeply nested as well), Temp Tables, Table Variables are all handled gracefully. You'll always see the original source tables.
+
+The resulting lineage structure is the following:
+    sink_table -> stored_procedure (1 or more) -> list_of_sources
+
+Dictionary Example:
+```
+{
+    'db_name.schema.table_sink': {
+        'schema.stored_procedure_1': [
+            'schema.table_source_1',
+            'schema.table_source_2',
+            'schema.table_source_3',
+        ],
+        'schema.stored_procedure_2': [
+            'schema.table_source_a',
+            'schema.table_source_b',
+            'schema.table_source_c',
+        ],
+    },
+    'db_name.schema.table_sink_2': {
+        'schema.stored_procedure_3': [
+            'schema.table_source',
+        ],
+    },
+}
+```
+
+Html Example:
+
+![Sample Image](https://github.com/ivan-ostymchuk/sql-server-lineage/blob/main/lineage_example.png)
+
+Therefore, everything is centered around the sink_table. Because most likely you want to see for each table where does the data come from. If you need it different (for a Data Catalog) you can transform the objects and adapt them to your requirement.
+In the html you will see the sink table as reference in a different color (green) and you will see it again in the lineage.
+
+I decided to generate html files instead of starting a local server (like DBT does) because I wanted to keep it simple and make it easy to host somewhere as a static website and therefore sharing it with other Data Engineers, Data Analysts, etc.
+
+This project is named sql-server-lineage because I want to keep it specialised only on Sql Server. To generate the lineage you need to develop a custom implementation of a Sql parser. I did it for Sql Server as I've been using it recently but I do not intend to develop parsers for other sql dialects.
+
+# DISCLAIMER
+Since this library analyses stored procedures, if you transform data externally and then write it to the database there is nothing you can do for the lineage. Also if the stored procedures rely heavily on dynamic sql especially with table names passed as parameters then the library would not be able to determine the table names for the lineage.
+
+# Implementation
+
+All the core logic is developed in Go, then using CGO, C bindings and some adapter functions I made it available also as a Python library.
+The main reason to do that was because Data Engineers work mainly in Python.
+
+# Get Started
+
+### Installation
+```
+pip install sql-server-lineage
+```
+
+### Example to generate the lineage directly from sql server
+In this example we get the stored procedures definitions from sql server
+but you can also read the definitions from files.
+
+```
+from sql_server_lineage import get_lineage, generate_html_lineage
+from typing import Dict, List
+import pyodbc
+
+host: str = "host"
+port: str = "port"
+driver: str = "driver"
+user: str = "user"
+password: str = "password"
+database: str = "database"
+otherparams: str = "otherparams"
+
+db_conn_string: str = f"DRIVER={{{driver}}};SERVER={host};PORT={port};DATABASE={database};UID={user};PWD={password};{otherparams}"
+conn: pyodbc.Connection = pyodbc.connect(db_conn_string)
+
+sql_query: str = """
+    SELECT OBJECT_DEFINITION(object_id) as sp_definition
+    FROM sys.procedures
+    WHERE object_id not in (select major_id from sys.extended_properties);
+"""
+
+cursor = conn.cursor()
+cursor.execute(sql_query)
+records: List = cursor.fetchall()
+stored_procedures: List[str] = [r.sp_definition for r in records]
+
+# get lineage and then send it to a Data Catalog, or transform and then send.
+result_lineage: Dict = get_lineage(stored_procedures)
+
+# generate the html representation of the lineage
+# providing the filename is optional
+lineage_file: str = "lineage_generated.html"
+generate_html_lineage(stored_procedures, lineage_file)
+```
+
+This project operates under the MIT License.
```

## Comparing `sql_server_lineage-1.12.0.dist-info/RECORD` & `sql_server_lineage-1.13.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-_sql_server_lineage.cp39-win_amd64.h,sha256=XFbD59UuMzQZLb0MCkKFpuWHflnMSEFx3lnddbsF_9g,2146
-_sql_server_lineage.cp39-win_amd64.pyd,sha256=x_yefKRR_ifg9WnKliM5voxfIDZWofVLIOMWt3IY1cg,4504655
-sql_server_lineage.py,sha256=LcuP4DQ4jTpngHEr1UG2oqUj-3RmqsBDZheRd8kRUhM,3774
-sql_server_lineage-1.12.0.dist-info/LICENSE,sha256=1t1J3-Xosw6RA66aI3kVJNCTdskdFDJLy52SquEppio,1090
-sql_server_lineage-1.12.0.dist-info/METADATA,sha256=_G31WWMOwgqGmZIQoZ4nNYQeOGfOCKexCAOHh399TiE,4979
-sql_server_lineage-1.12.0.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-sql_server_lineage-1.12.0.dist-info/top_level.txt,sha256=VnPX7sid6BFlcg6FXWZ2izIWcWHM_fQtFKk5vUQjncQ,39
-sql_server_lineage-1.12.0.dist-info/RECORD,,
+_sql_server_lineage.cpython-310-aarch64-linux-gnu.h,sha256=6kljXVJxdRkfg37egkRI-_34VoUL9rmbW5hlcJkdpUs,2080
+_sql_server_lineage.cpython-310-aarch64-linux-gnu.so,sha256=okA0UyWP_tgpuBZYgttvaN8hFX9r9T4w3mSDIIiSItM,2595400
+sql_server_lineage.py,sha256=Lsq8x3tklDyypVvWXEEqJNXWZRhjWbHI6IhyRL-4PwU,3670
+sql_server_lineage-1.13.0.dist-info/WHEEL,sha256=7-IJbjbL0nWUFP_cSrTULDrfI4l8JN0GBqGHPqza7ao,154
+sql_server_lineage-1.13.0.dist-info/LICENSE,sha256=MP07Z1xzkk0lR0zBSUkDlO7g2lpkvzpLmYYasaO3bTU,1070
+sql_server_lineage-1.13.0.dist-info/top_level.txt,sha256=VnPX7sid6BFlcg6FXWZ2izIWcWHM_fQtFKk5vUQjncQ,39
+sql_server_lineage-1.13.0.dist-info/RECORD,,
+sql_server_lineage-1.13.0.dist-info/METADATA,sha256=eA4lbf4KzYYnCfkSFu6IWOMrGItnGBs9bPso3CJx1JA,4863
```

