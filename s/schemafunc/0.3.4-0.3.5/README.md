# Comparing `tmp/schemafunc-0.3.4.tar.gz` & `tmp/schemafunc-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schemafunc-0.3.4.tar", max compression
+gzip compressed data, was "schemafunc-0.3.5.tar", max compression
```

## Comparing `schemafunc-0.3.4.tar` & `schemafunc-0.3.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2024-04-11 16:31:26.401239 schemafunc-0.3.4/LICENSE
--rw-r--r--   0        0        0     1140 2024-05-29 17:21:14.574566 schemafunc-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     6614 2024-04-14 16:41:56.673792 schemafunc-0.3.4/README.md
--rw-r--r--   0        0        0    20027 2024-05-29 17:09:14.473876 schemafunc-0.3.4/src/schemafunc.py
--rw-r--r--   0        0        0     7626 1970-01-01 00:00:00.000000 schemafunc-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-11 16:31:26.401239 schemafunc-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1140 2024-05-30 22:12:48.922020 schemafunc-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     6614 2024-04-14 16:41:56.673792 schemafunc-0.3.5/README.md
+-rw-r--r--   0        0        0    20756 2024-05-30 22:10:20.788241 schemafunc-0.3.5/src/schemafunc.py
+-rw-r--r--   0        0        0     7626 1970-01-01 00:00:00.000000 schemafunc-0.3.5/PKG-INFO
```

### Comparing `schemafunc-0.3.4/LICENSE` & `schemafunc-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `schemafunc-0.3.4/pyproject.toml` & `schemafunc-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "schemafunc"
-version = "0.3.4"
+version = "0.3.5"
 description = "Python function-to-LLM tool maker."
 authors = ["Dustin Wyatt <dustin.wyatt@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dmwyatt/schemafunc"
 
 keywords = ["python", "openai", "llm", "language-model", "schema", "function", "tool"]
```

### Comparing `schemafunc-0.3.4/README.md` & `schemafunc-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `schemafunc-0.3.4/src/schemafunc.py` & `schemafunc-0.3.5/src/schemafunc.py`

 * *Files 3% similar despite different names*

```diff
@@ -318,16 +318,16 @@
 
 
 def resolve_type(param_type: typing.Type) -> dict:
     """
     Resolves a Python type into a JSON Schema dictionary.
 
     This function takes a Python type (such as `int`, `str`, `typing.Union`,
-    `typing.List`, etc.) and returns a dictionary representing the equivalent
-    JSON Schema type.
+    `typing.List`, `typing.Dict`, etc.) and returns a dictionary representing the
+    equivalent JSON Schema type.
 
     Args:
         param_type (typing.Type): The Python type to resolve.
 
     Returns:
         dict: A dictionary representing the JSON Schema equivalent of the input type.
 
@@ -340,14 +340,17 @@
 
         >>> resolve_type(typing.List[str])
         {'type': 'array', 'items': {'type': 'string'}}
 
         >>> resolve_type(typing.Union[int, str])
         {'type': ['integer', 'string']}
 
+        >>> resolve_type(typing.Dict[str, int])
+        {'type': 'object', 'additionalProperties': {'type': 'integer'}}
+
     The function supports the following types:
 
     - Basic types (`int`, `float`, `str`, `bool`, `None`): These are converted to the
       corresponding JSON Schema types (`'integer'`, `'number'`, `'string'`,
       `'boolean'`, `'null'`).
 
     - Union types (`typing.Union`): These are converted to a JSON Schema type array,
@@ -355,23 +358,29 @@
 
     - Array types (`typing.List`, `typing.Tuple`, `typing.Set`, etc.): These are
       converted to a JSON Schema `'array'` type, with the `items` property
       representing the type of the array elements.
 
     - Literal types (`typing.Literal`): These are converted to a JSON Schema
       `'string'` type, with an `enum` property listing the permitted literal values.
+
+    - Dictionary types (`typing.Dict`): These are converted to a JSON Schema
+      `'object'` type, with the `additionalProperties` property representing the
+      type of the dictionary values.
     """
     if is_basic_type(param_type):
         return resolve_basic_type(param_type)
     elif is_union_type(param_type):
         return resolve_union_type(param_type)
     elif is_array_type(param_type):
         return resolve_array_type(param_type)
     elif is_literal_type(param_type):
         return resolve_literal_type(param_type)
+    elif is_dict_type(param_type):
+        return resolve_dict_type(param_type)
     else:
         raise UnsupportedTypeError(f"Unsupported type: {param_type}")
 
 
 def is_basic_type(param_type: typing.Type) -> bool:
     return param_type in JSON_SCHEMA_TYPES
 
@@ -572,7 +581,18 @@
             typ, (str, bytes, bytearray, dict)
         ):
             return True
     except TypeError:
         # If the type is not a class, then nothing to check.
         return False
     return False
+
+
+def is_dict_type(param_type: typing.Type) -> bool:
+    return typing.get_origin(param_type) == dict
+
+def resolve_dict_type(param_type: typing.Type) -> dict:
+    key_type, value_type = typing.get_args(param_type)
+    return {
+        "type": "object",
+        "additionalProperties": resolve_type(value_type),
+    }
```

### Comparing `schemafunc-0.3.4/PKG-INFO` & `schemafunc-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemafunc
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python function-to-LLM tool maker.
 Home-page: https://github.com/dmwyatt/schemafunc
 License: MIT
 Keywords: python,openai,llm,language-model,schema,function,tool
 Author: Dustin Wyatt
 Author-email: dustin.wyatt@gmail.com
 Requires-Python: >=3.10.11,<4.0.0
```

