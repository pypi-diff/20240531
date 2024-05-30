# Comparing `tmp/schemafunc-0.3.6.tar.gz` & `tmp/schemafunc-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schemafunc-0.3.6.tar", max compression
+gzip compressed data, was "schemafunc-0.3.7.tar", max compression
```

## Comparing `schemafunc-0.3.6.tar` & `schemafunc-0.3.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2024-04-11 16:31:26.401239 schemafunc-0.3.6/LICENSE
--rw-r--r--   0        0        0     1140 2024-05-30 22:29:36.085958 schemafunc-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     6614 2024-04-14 16:41:56.673792 schemafunc-0.3.6/README.md
--rw-r--r--   0        0        0    21509 2024-05-30 22:25:14.052065 schemafunc-0.3.6/src/schemafunc.py
--rw-r--r--   0        0        0     7626 1970-01-01 00:00:00.000000 schemafunc-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-11 16:31:26.401239 schemafunc-0.3.7/LICENSE
+-rw-r--r--   0        0        0     1140 2024-05-30 22:46:14.259054 schemafunc-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     6614 2024-04-14 16:41:56.673792 schemafunc-0.3.7/README.md
+-rw-r--r--   0        0        0    21542 2024-05-30 22:44:02.104024 schemafunc-0.3.7/src/schemafunc.py
+-rw-r--r--   0        0        0     7626 1970-01-01 00:00:00.000000 schemafunc-0.3.7/PKG-INFO
```

### Comparing `schemafunc-0.3.6/LICENSE` & `schemafunc-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `schemafunc-0.3.6/pyproject.toml` & `schemafunc-0.3.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "schemafunc"
-version = "0.3.6"
+version = "0.3.7"
 description = "Python function-to-LLM tool maker."
 authors = ["Dustin Wyatt <dustin.wyatt@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dmwyatt/schemafunc"
 
 keywords = ["python", "openai", "llm", "language-model", "schema", "function", "tool"]
```

### Comparing `schemafunc-0.3.6/README.md` & `schemafunc-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `schemafunc-0.3.6/src/schemafunc.py` & `schemafunc-0.3.7/src/schemafunc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import inspect
+import types
 import typing
 from collections.abc import Sequence, Set
 from functools import wraps
 from types import MappingProxyType
 
 from docstring_parser import Docstring, parse
 
@@ -388,15 +389,15 @@
 
 
 def resolve_basic_type(param_type: typing.Type) -> dict:
     return {"type": JSON_SCHEMA_TYPES[param_type]}
 
 
 def is_union_type(param_type: typing.Type) -> bool:
-    return typing.get_origin(param_type) == typing.Union
+    return typing.get_origin(param_type) in [typing.Union, types.UnionType]
 
 
 def resolve_union_type(param_type: typing.Type) -> dict:
     """
     Resolves a union type into a JSON schema.
 
     Given a Python type that represents a union (i.e., a type that can be one of
@@ -588,14 +589,15 @@
         return False
     return False
 
 
 def is_dict_type(param_type: typing.Type) -> bool:
     return typing.get_origin(param_type) == dict
 
+
 def resolve_dict_type(param_type: typing.Type) -> dict:
     """
     Resolves a dictionary type into a JSON schema.
 
     This function expects the key type of the dictionary to be a string, as required
     by the JSON specification. If the key type is not a string, a UnsupportedTypeError is raised.
     The value type is resolved using the `resolve_type` function and included in the schema.
```

### Comparing `schemafunc-0.3.6/PKG-INFO` & `schemafunc-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemafunc
-Version: 0.3.6
+Version: 0.3.7
 Summary: Python function-to-LLM tool maker.
 Home-page: https://github.com/dmwyatt/schemafunc
 License: MIT
 Keywords: python,openai,llm,language-model,schema,function,tool
 Author: Dustin Wyatt
 Author-email: dustin.wyatt@gmail.com
 Requires-Python: >=3.10.11,<4.0.0
```

