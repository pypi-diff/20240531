# Comparing `tmp/databind-4.5.1.tar.gz` & `tmp/databind-4.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databind-4.5.1.tar", max compression
+gzip compressed data, was "databind-4.5.2.tar", max compression
```

## Comparing `databind-4.5.1.tar` & `databind-4.5.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     3048 2024-04-02 09:25:49.053087 databind-4.5.1/README.md
--rw-r--r--   0        0        0     2118 2024-04-02 10:02:28.522788 databind-4.5.1/pyproject.toml
--rw-r--r--   0        0        0     1601 2024-04-02 10:02:28.522953 databind-4.5.1/src/databind/core/__init__.py
--rw-r--r--   0        0        0     5481 2024-04-02 09:22:26.323647 databind-4.5.1/src/databind/core/context.py
--rw-r--r--   0        0        0     6703 2024-04-02 09:22:26.323889 databind-4.5.1/src/databind/core/converter.py
--rw-r--r--   0        0        0     4099 2024-04-02 09:22:26.324326 databind-4.5.1/src/databind/core/dataclasses.py
--rw-r--r--   0        0        0     7120 2024-04-02 09:22:26.324930 databind-4.5.1/src/databind/core/dataclasses.pyi
--rw-r--r--   0        0        0     3943 2024-04-02 09:22:26.325111 databind-4.5.1/src/databind/core/mapper.py
--rw-r--r--   0        0        0        0 2024-04-02 09:22:26.325215 databind-4.5.1/src/databind/core/py.typed
--rw-r--r--   0        0        0    15523 2024-04-02 09:22:26.325612 databind-4.5.1/src/databind/core/schema.py
--rw-r--r--   0        0        0    27807 2024-04-02 09:22:26.325870 databind-4.5.1/src/databind/core/settings.py
--rw-r--r--   0        0        0     1044 2024-04-02 09:22:26.326210 databind-4.5.1/src/databind/core/tests/context_test.py
--rw-r--r--   0        0        0     1275 2024-04-02 09:22:26.331892 databind-4.5.1/src/databind/core/tests/schema_docspec_example_test.py
--rw-r--r--   0        0        0    11105 2024-04-02 09:22:26.333093 databind-4.5.1/src/databind/core/tests/schema_test.py
--rw-r--r--   0        0        0      733 2024-04-02 09:22:26.333360 databind-4.5.1/src/databind/core/tests/schema_with_nested_dataclasses_test.py
--rw-r--r--   0        0        0     8933 2024-04-02 09:22:26.334093 databind-4.5.1/src/databind/core/union.py
--rw-r--r--   0        0        0     2955 2024-04-02 09:22:26.334297 databind-4.5.1/src/databind/core/utils.py
--rw-r--r--   0        0        0     2410 2024-04-02 10:02:28.523077 databind-4.5.1/src/databind/json/__init__.py
--rw-r--r--   0        0        0    35450 2024-04-02 09:22:26.334878 databind-4.5.1/src/databind/json/converters.py
--rw-r--r--   0        0        0     2951 2024-04-02 09:22:26.335050 databind-4.5.1/src/databind/json/module.py
--rw-r--r--   0        0        0        0 2024-04-02 09:22:26.335120 databind-4.5.1/src/databind/json/py.typed
--rw-r--r--   0        0        0     1934 2024-04-02 09:22:26.335313 databind-4.5.1/src/databind/json/settings.py
--rw-r--r--   0        0        0    27496 2024-04-02 09:22:26.335657 databind-4.5.1/src/databind/json/tests/converters_test.py
--rw-r--r--   0        0        0     4328 1970-01-01 00:00:00.000000 databind-4.5.1/PKG-INFO
+-rw-r--r--   0        0        0     3048 2024-05-31 11:47:00.649650 databind-4.5.2/README.md
+-rw-r--r--   0        0        0     2118 2024-05-31 15:28:34.600847 databind-4.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1601 2024-05-31 15:28:34.601023 databind-4.5.2/src/databind/core/__init__.py
+-rw-r--r--   0        0        0     5481 2024-05-31 11:47:00.650816 databind-4.5.2/src/databind/core/context.py
+-rw-r--r--   0        0        0     6703 2024-05-31 11:47:00.651126 databind-4.5.2/src/databind/core/converter.py
+-rw-r--r--   0        0        0     4099 2024-05-31 11:47:00.651384 databind-4.5.2/src/databind/core/dataclasses.py
+-rw-r--r--   0        0        0     7120 2024-05-31 11:47:00.651650 databind-4.5.2/src/databind/core/dataclasses.pyi
+-rw-r--r--   0        0        0     3943 2024-05-31 11:47:00.651869 databind-4.5.2/src/databind/core/mapper.py
+-rw-r--r--   0        0        0        0 2024-05-31 11:47:00.652007 databind-4.5.2/src/databind/core/py.typed
+-rw-r--r--   0        0        0    15523 2024-05-31 14:59:46.084489 databind-4.5.2/src/databind/core/schema.py
+-rw-r--r--   0        0        0    27807 2024-05-31 11:47:00.659528 databind-4.5.2/src/databind/core/settings.py
+-rw-r--r--   0        0        0     1044 2024-05-31 11:47:00.660048 databind-4.5.2/src/databind/core/tests/context_test.py
+-rw-r--r--   0        0        0     1275 2024-05-31 11:47:00.660283 databind-4.5.2/src/databind/core/tests/schema_docspec_example_test.py
+-rw-r--r--   0        0        0    11105 2024-05-31 11:47:00.660589 databind-4.5.2/src/databind/core/tests/schema_test.py
+-rw-r--r--   0        0        0      733 2024-05-31 11:47:00.661668 databind-4.5.2/src/databind/core/tests/schema_with_nested_dataclasses_test.py
+-rw-r--r--   0        0        0     8933 2024-05-31 11:47:00.662245 databind-4.5.2/src/databind/core/union.py
+-rw-r--r--   0        0        0     2955 2024-05-31 11:47:00.662474 databind-4.5.2/src/databind/core/utils.py
+-rw-r--r--   0        0        0     2410 2024-05-31 15:28:34.601142 databind-4.5.2/src/databind/json/__init__.py
+-rw-r--r--   0        0        0    35554 2024-05-31 15:27:41.259232 databind-4.5.2/src/databind/json/converters.py
+-rw-r--r--   0        0        0     2951 2024-05-31 11:47:00.663658 databind-4.5.2/src/databind/json/module.py
+-rw-r--r--   0        0        0        0 2024-05-31 11:47:00.663812 databind-4.5.2/src/databind/json/py.typed
+-rw-r--r--   0        0        0     1934 2024-05-31 11:47:00.664036 databind-4.5.2/src/databind/json/settings.py
+-rw-r--r--   0        0        0    27665 2024-05-31 15:27:41.262023 databind-4.5.2/src/databind/json/tests/converters_test.py
+-rw-r--r--   0        0        0     4328 1970-01-01 00:00:00.000000 databind-4.5.2/PKG-INFO
```

### Comparing `databind-4.5.1/README.md` & `databind-4.5.2/README.md`

 * *Files identical despite different names*

### Comparing `databind-4.5.1/pyproject.toml` & `databind-4.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databind"
-version = "4.5.1"
+version = "4.5.2"
 description = "Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. The `databind` package will install the full suite of databind packages. Compatible with Python 3.8 and newer."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "databind/core", from = "src"}, {include = "databind/json", from = "src"}]
 
 [tool.poetry.urls]
```

### Comparing `databind-4.5.1/src/databind/core/__init__.py` & `databind-4.5.2/src/databind/core/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "4.5.1"
+__version__ = "4.5.2"
 
 from .context import Context, Direction, Location, format_context_trace
 from .converter import ConversionError, Converter, DelegateToClassmethodConverter, Module, NoMatchingConverter
 from .mapper import ObjectMapper
 from .schema import (
     Field,
     Schema,
```

### Comparing `databind-4.5.1/src/databind/core/context.py` & `databind-4.5.2/src/databind/core/context.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.1/src/databind/core/converter.py` & `databind-4.5.2/src/databind/core/converter.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.1/src/databind/core/dataclasses.py` & `databind-4.5.2/src/databind/core/dataclasses.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.1/src/databind/core/dataclasses.pyi` & `databind-4.5.2/src/databind/core/dataclasses.pyi`

 * *Files identical despite different names*

### Comparing `databind-4.5.1/src/databind/core/mapper.py` & `databind-4.5.2/src/databind/core/mapper.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.1/src/databind/core/schema.py` & `databind-4.5.2/src/databind/core/schema.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.1/src/databind/core/settings.py` & `databind-4.5.2/src/databind/core/settings.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.1/src/databind/core/tests/context_test.py` & `databind-4.5.2/src/databind/core/tests/context_test.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.1/src/databind/core/tests/schema_docspec_example_test.py` & `databind-4.5.2/src/databind/core/tests/schema_docspec_example_test.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.1/src/databind/core/tests/schema_test.py` & `databind-4.5.2/src/databind/core/tests/schema_test.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.1/src/databind/core/tests/schema_with_nested_dataclasses_test.py` & `databind-4.5.2/src/databind/core/tests/schema_with_nested_dataclasses_test.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.1/src/databind/core/union.py` & `databind-4.5.2/src/databind/core/union.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.1/src/databind/core/utils.py` & `databind-4.5.2/src/databind/core/utils.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.1/src/databind/json/__init__.py` & `databind-4.5.2/src/databind/json/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 import typing as t
 
 from databind.core import ObjectMapper, Setting, Settings
 from databind.json.module import JsonModule
 from databind.json.settings import JsonConverter
 
-__version__ = "4.5.1"
+__version__ = "4.5.2"
 __all__ = [
     "dump",
     "dumps",
     "get_object_mapper",
     "JsonConverter",
     "JsonModule",
     "JsonType",
```

### Comparing `databind-4.5.1/src/databind/json/converters.py` & `databind-4.5.2/src/databind/json/converters.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
             raise NotImplementedError
         if ctx.value is None:
             return None
         return ctx.spawn(ctx.value, datatype.without_none_type(), None).convert()
 
 
 class PlainDatatypeConverter(Converter):
-    """A converter for the plain datatypes #bool, #bytes, #int, #str and #float.
+    """A converter for the plain datatypes #bool, #bytes, #int, #str, #float and #null.
 
     Arguments:
       direction (Direction): The direction in which to convert (serialize or deserialize).
       strict_by_default (bool): Whether to use strict type conversion on values by default if no other
         information on strictness is given. This defaults to `True`. With strict conversion enabled,
         loss-less type conversions are disabled (such as casting a string to an integer). Note that
         serialization is _always_ strict, only the deserialization is controlled with this option or
@@ -390,26 +390,28 @@
         (str, bytes): base64.b64decode,
         (str, str): str,
         (int, int): int,
         (float, float): float,
         (int, float): float,
         (float, int): _int_lossless,
         (bool, bool): bool,
+        (type(None), type(None)): lambda x: x,
     }
 
     # Used only during deserialization if the #fieldinfo.strict is disabled.
     _nonstrict_adapters = _strict_adapters.copy()
     _nonstrict_adapters.update(
         {
             (str, int): int,
             (str, float): float,
             (str, bool): _bool_from_str,
             (int, str): str,
             (float, str): str,
             (bool, str): str,
+            (type(None), type(None)): lambda x: x,
         }
     )
 
     def __init__(self, strict_by_default: bool = True) -> None:
         self.strict_by_default = strict_by_default
 
     def convert(self, ctx: Context) -> t.Any:
@@ -424,15 +426,14 @@
         strict = (
             (ctx.get_setting(Strict) or Strict(self.strict_by_default))
             if ctx.direction == Direction.DESERIALIZE
             else Strict(True)
         )
         adapters = self._strict_adapters if strict.enabled else self._nonstrict_adapters
         adapter = adapters.get((source_type, target_type))
-
         if adapter is None:
             raise ConversionError.expected(self, ctx, target_type, source_type)
 
         try:
             return adapter(ctx.value)
         except ValueError as exc:
             raise ConversionError(self, ctx, str(exc)) from exc
```

### Comparing `databind-4.5.1/src/databind/json/module.py` & `databind-4.5.2/src/databind/json/module.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.1/src/databind/json/settings.py` & `databind-4.5.2/src/databind/json/settings.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.1/src/databind/json/tests/converters_test.py` & `databind-4.5.2/src/databind/json/tests/converters_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,18 @@
             assert mapper.convert(direction, "42", int)
 
     else:
         assert mapper.convert(direction, "42", int) == 42
         with pytest.raises(ConversionError):
             mapper.convert(direction, "foobar", int)
 
+    # None should behave the same in both cases
+    assert mapper.convert(direction, None, type(None)) is None
+    assert mapper.convert(direction, None, None) is None
+
 
 @pytest.mark.parametrize("direction", (Direction.SERIALIZE, Direction.DESERIALIZE))
 def test_decimal_converter(direction: Direction) -> None:
     mapper = make_mapper([DecimalConverter()])
 
     pi = decimal.Decimal("3.141592653589793")
     if direction == Direction.SERIALIZE:
```

### Comparing `databind-4.5.1/PKG-INFO` & `databind-4.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databind
-Version: 4.5.1
+Version: 4.5.2
 Summary: Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. The `databind` package will install the full suite of databind packages. Compatible with Python 3.8 and newer.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

