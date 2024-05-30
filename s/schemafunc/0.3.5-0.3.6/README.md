# Comparing `tmp/schemafunc-0.3.5.tar.gz` & `tmp/schemafunc-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schemafunc-0.3.5.tar", max compression
+gzip compressed data, was "schemafunc-0.3.6.tar", max compression
```

## Comparing `schemafunc-0.3.5.tar` & `schemafunc-0.3.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2024-04-11 16:31:26.401239 schemafunc-0.3.5/LICENSE
--rw-r--r--   0        0        0     1140 2024-05-30 22:12:48.922020 schemafunc-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     6614 2024-04-14 16:41:56.673792 schemafunc-0.3.5/README.md
--rw-r--r--   0        0        0    20756 2024-05-30 22:10:20.788241 schemafunc-0.3.5/src/schemafunc.py
--rw-r--r--   0        0        0     7626 1970-01-01 00:00:00.000000 schemafunc-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-11 16:31:26.401239 schemafunc-0.3.6/LICENSE
+-rw-r--r--   0        0        0     1140 2024-05-30 22:29:36.085958 schemafunc-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     6614 2024-04-14 16:41:56.673792 schemafunc-0.3.6/README.md
+-rw-r--r--   0        0        0    21509 2024-05-30 22:25:14.052065 schemafunc-0.3.6/src/schemafunc.py
+-rw-r--r--   0        0        0     7626 1970-01-01 00:00:00.000000 schemafunc-0.3.6/PKG-INFO
```

### Comparing `schemafunc-0.3.5/LICENSE` & `schemafunc-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `schemafunc-0.3.5/pyproject.toml` & `schemafunc-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "schemafunc"
-version = "0.3.5"
+version = "0.3.6"
 description = "Python function-to-LLM tool maker."
 authors = ["Dustin Wyatt <dustin.wyatt@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dmwyatt/schemafunc"
 
 keywords = ["python", "openai", "llm", "language-model", "schema", "function", "tool"]
```

### Comparing `schemafunc-0.3.5/README.md` & `schemafunc-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `schemafunc-0.3.5/src/schemafunc.py` & `schemafunc-0.3.6/src/schemafunc.py`

 * *Files 4% similar despite different names*

```diff
@@ -363,14 +363,16 @@
     - Literal types (`typing.Literal`): These are converted to a JSON Schema
       `'string'` type, with an `enum` property listing the permitted literal values.
 
     - Dictionary types (`typing.Dict`): These are converted to a JSON Schema
       `'object'` type, with the `additionalProperties` property representing the
       type of the dictionary values.
     """
+    if param_type is typing.Any:
+        return {}
     if is_basic_type(param_type):
         return resolve_basic_type(param_type)
     elif is_union_type(param_type):
         return resolve_union_type(param_type)
     elif is_array_type(param_type):
         return resolve_array_type(param_type)
     elif is_literal_type(param_type):
@@ -587,12 +589,30 @@
     return False
 
 
 def is_dict_type(param_type: typing.Type) -> bool:
     return typing.get_origin(param_type) == dict
 
 def resolve_dict_type(param_type: typing.Type) -> dict:
+    """
+    Resolves a dictionary type into a JSON schema.
+
+    This function expects the key type of the dictionary to be a string, as required
+    by the JSON specification. If the key type is not a string, a UnsupportedTypeError is raised.
+    The value type is resolved using the `resolve_type` function and included in the schema.
+
+    Args:
+        param_type (typing.Type): The dictionary type to resolve.
+
+    Returns:
+        dict: A JSON schema representing the dictionary type.
+
+    Raises:
+        UnsupportedTypeError: If the key type of the dictionary is not a string.
+    """
     key_type, value_type = typing.get_args(param_type)
+    if key_type != str:
+        raise UnsupportedTypeError(f"Dictionary keys must be strings, not {key_type}")
     return {
         "type": "object",
         "additionalProperties": resolve_type(value_type),
     }
```

### Comparing `schemafunc-0.3.5/PKG-INFO` & `schemafunc-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemafunc
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python function-to-LLM tool maker.
 Home-page: https://github.com/dmwyatt/schemafunc
 License: MIT
 Keywords: python,openai,llm,language-model,schema,function,tool
 Author: Dustin Wyatt
 Author-email: dustin.wyatt@gmail.com
 Requires-Python: >=3.10.11,<4.0.0
```

