# Comparing `tmp/pybare-1.0.1.tar.gz` & `tmp/pybare-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybare-1.0.1.tar", last modified: Thu May 30 17:03:13 2024, max compression
+gzip compressed data, was "pybare-1.1.0.tar", last modified: Fri May 31 17:31:38 2024, max compression
```

## Comparing `pybare-1.0.1.tar` & `pybare-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2024-05-30 17:03:13.129910 pybare-1.0.1/
--rw-rw-r--   0 noah      (1000) noah      (1000)     1053 2024-05-22 19:27:02.000000 pybare-1.0.1/LICENSE
--rw-r--r--   0 noah      (1000) noah      (1000)     2639 2024-05-30 17:03:13.129910 pybare-1.0.1/PKG-INFO
--rw-rw-r--   0 noah      (1000) noah      (1000)     2145 2024-05-30 16:48:15.000000 pybare-1.0.1/README.md
-drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2024-05-30 17:03:13.129910 pybare-1.0.1/bare/
--rw-rw-r--   0 noah      (1000) noah      (1000)      766 2024-05-30 16:48:36.000000 pybare-1.0.1/bare/__init__.py
--rw-rw-r--   0 noah      (1000) noah      (1000)     4654 2024-05-30 16:48:36.000000 pybare-1.0.1/bare/barearray.py
--rw-rw-r--   0 noah      (1000) noah      (1000)     3739 2024-05-30 16:56:39.000000 pybare-1.0.1/bare/barestruct.py
--rw-rw-r--   0 noah      (1000) noah      (1000)      662 2024-05-30 16:48:36.000000 pybare-1.0.1/bare/baretype.py
--rw-rw-r--   0 noah      (1000) noah      (1000)     2349 2024-05-30 16:48:36.000000 pybare-1.0.1/bare/data.py
--rw-rw-r--   0 noah      (1000) noah      (1000)     3567 2024-05-30 16:48:36.000000 pybare-1.0.1/bare/map.py
--rw-rw-r--   0 noah      (1000) noah      (1000)     3320 2024-05-30 16:48:36.000000 pybare-1.0.1/bare/misc.py
--rw-rw-r--   0 noah      (1000) noah      (1000)    10598 2024-05-30 16:58:41.000000 pybare-1.0.1/bare/number.py
--rw-rw-r--   0 noah      (1000) noah      (1000)     8310 2024-05-30 16:48:36.000000 pybare-1.0.1/bare/test_encoder.py
--rw-rw-r--   0 noah      (1000) noah      (1000)     6178 2024-05-30 16:48:36.000000 pybare-1.0.1/bare/union.py
--rw-rw-r--   0 noah      (1000) noah      (1000)     1282 2024-05-30 16:48:36.000000 pybare-1.0.1/bare/util.py
-drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2024-05-30 17:03:13.129910 pybare-1.0.1/pybare.egg-info/
--rw-r--r--   0 noah      (1000) noah      (1000)     2639 2024-05-30 17:03:13.000000 pybare-1.0.1/pybare.egg-info/PKG-INFO
--rw-rw-r--   0 noah      (1000) noah      (1000)      318 2024-05-30 17:03:13.000000 pybare-1.0.1/pybare.egg-info/SOURCES.txt
--rw-rw-r--   0 noah      (1000) noah      (1000)        1 2024-05-30 17:03:13.000000 pybare-1.0.1/pybare.egg-info/dependency_links.txt
--rw-rw-r--   0 noah      (1000) noah      (1000)        5 2024-05-30 17:03:13.000000 pybare-1.0.1/pybare.egg-info/top_level.txt
--rw-rw-r--   0 noah      (1000) noah      (1000)       38 2024-05-30 17:03:13.129910 pybare-1.0.1/setup.cfg
--rw-rw-r--   0 noah      (1000) noah      (1000)      743 2024-05-30 17:02:32.000000 pybare-1.0.1/setup.py
+drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2024-05-31 17:31:38.890370 pybare-1.1.0/
+-rw-rw-r--   0 noah      (1000) noah      (1000)     1053 2024-05-22 19:27:02.000000 pybare-1.1.0/LICENSE
+-rw-r--r--   0 noah      (1000) noah      (1000)     2639 2024-05-31 17:31:38.890370 pybare-1.1.0/PKG-INFO
+-rw-rw-r--   0 noah      (1000) noah      (1000)     2145 2024-05-30 16:48:15.000000 pybare-1.1.0/README.md
+drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2024-05-31 17:31:38.890370 pybare-1.1.0/bare/
+-rw-rw-r--   0 noah      (1000) noah      (1000)      813 2024-05-31 17:25:45.000000 pybare-1.1.0/bare/__init__.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     4799 2024-05-31 17:25:45.000000 pybare-1.1.0/bare/barearray.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     3744 2024-05-31 17:25:45.000000 pybare-1.1.0/bare/barestruct.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)      495 2024-05-31 17:25:45.000000 pybare-1.1.0/bare/baretype.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     2349 2024-05-30 16:48:36.000000 pybare-1.1.0/bare/data.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     3567 2024-05-30 16:48:36.000000 pybare-1.1.0/bare/map.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     3343 2024-05-31 17:25:45.000000 pybare-1.1.0/bare/misc.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)    10598 2024-05-30 16:58:41.000000 pybare-1.1.0/bare/number.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     8310 2024-05-30 16:48:36.000000 pybare-1.1.0/bare/test_encoder.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     6211 2024-05-31 17:25:45.000000 pybare-1.1.0/bare/union.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     1282 2024-05-30 16:48:36.000000 pybare-1.1.0/bare/util.py
+drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2024-05-31 17:31:38.890370 pybare-1.1.0/pybare.egg-info/
+-rw-r--r--   0 noah      (1000) noah      (1000)     2639 2024-05-31 17:31:38.000000 pybare-1.1.0/pybare.egg-info/PKG-INFO
+-rw-rw-r--   0 noah      (1000) noah      (1000)      318 2024-05-31 17:31:38.000000 pybare-1.1.0/pybare.egg-info/SOURCES.txt
+-rw-rw-r--   0 noah      (1000) noah      (1000)        1 2024-05-31 17:31:38.000000 pybare-1.1.0/pybare.egg-info/dependency_links.txt
+-rw-rw-r--   0 noah      (1000) noah      (1000)        5 2024-05-31 17:31:38.000000 pybare-1.1.0/pybare.egg-info/top_level.txt
+-rw-rw-r--   0 noah      (1000) noah      (1000)       38 2024-05-31 17:31:38.890370 pybare-1.1.0/setup.cfg
+-rw-rw-r--   0 noah      (1000) noah      (1000)      743 2024-05-31 17:28:31.000000 pybare-1.1.0/setup.py
```

### Comparing `pybare-1.0.1/LICENSE` & `pybare-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybare-1.0.1/PKG-INFO` & `pybare-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybare
-Version: 1.0.1
+Version: 1.1.0
 Summary: A declarative implementation of BARE for Python
 Home-page: https://sr.ht/~chiefnoah/PyBARE/
 Author: Noah Pederson
 Author-email: noah@packetlost.dev
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pybare-1.0.1/README.md` & `pybare-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pybare-1.0.1/bare/__init__.py` & `pybare-1.1.0/bare/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 pybare is a Python library for writing and reading binary data using the BARE
 serialization format.
 """
 
 from .barearray import Array, array
 from .barestruct import Field, Struct
+from .baretype import BAREType
 from .data import Data, data
 from .map import Map, map
 from .misc import Enum, Str, Void
 from .number import F32, F64, I8, I16, I32, I64, U8, U16, U32, U64, Bool, Int, UInt
 from .union import Union, UnionVariant, optional, union
 
 __all__ = [
+    "BAREType",
     "F32",
     "F64",
     "I8",
     "I16",
     "I32",
     "I64",
     "U8",
```

### Comparing `pybare-1.0.1/bare/barearray.py` & `pybare-1.1.0/bare/barearray.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import io
 from typing import Any, BinaryIO, Generic, Iterable, List, Optional, Self, Type, TypeVar
 
+from .baretype import BAREType
 from .number import UInt
 
 T = TypeVar("T")
 A = List[T]
 
 
 __all__ = ["Array", "array"]
@@ -13,15 +14,15 @@
 class ArrayMeta(type):
     def __new__(
         cls,
         name,
         bases,
         namespace,
         *,
-        inner: type | None = None,
+        inner: Type[BAREType[Any]] | None = None,
         size: Optional[int] = None,
     ):
         inner_type = inner or namespace.get("_type", None)
         if inner_type is None and name != "Array":
             raise TypeError("Array must have an inner type")
         namespace["_type"] = inner_type
         if size is None and name != "Array":
@@ -129,16 +130,19 @@
             if len(value) != cls._size:
                 return False
         for v in value:
             if not cls._type.validate(v):
                 return False
         return True
 
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}({repr(self.value)})"
 
-def array(inner: type, size: Optional[int] = None) -> Type[Array[A]]:
+
+def array(inner: Type[A], size: Optional[int] = None) -> Type[Array[A]]:
     """
     A function that defines and returns anonymous BARE `Array` subclass with
     the provided `inner` type and (optional) `size` arguments.
 
 
     Proper usage of this function is as follows:
```

### Comparing `pybare-1.0.1/bare/barestruct.py` & `pybare-1.1.0/bare/barestruct.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 from typing import Any, BinaryIO
 
 from .util import Field
 
-
 __all__ = ["Struct"]
 
 
 class StructMeta(type):
     def __new__(cls, clsname, bases, clsdict):
         fields = {}
         has_fields = False
@@ -97,19 +96,19 @@
             return False
         for name, ty in cls._fields.items():
             if not ty.validate(getattr(value, name)):
                 return False
         return True
 
     def __repr__(self) -> str:
-        name = self.__class__.__name__
+        clsname = self.__class__.__name__
         fields = []
         for name, field in self._fields.items():
             fields.append(f"{name}={getattr(self, name)}")
-        return f"{name}({', '.join(fields)})"
+        return f"{clsname}({', '.join(fields)})"
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, self.__class__):
             for name in self._fields.keys():
                 if getattr(self, name) != getattr(other, name):
                     return False
             return True
```

### Comparing `pybare-1.0.1/bare/data.py` & `pybare-1.1.0/bare/data.py`

 * *Files identical despite different names*

### Comparing `pybare-1.0.1/bare/map.py` & `pybare-1.1.0/bare/map.py`

 * *Files identical despite different names*

### Comparing `pybare-1.0.1/bare/misc.py` & `pybare-1.1.0/bare/misc.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,16 +99,17 @@
     def __init__(self, value: str):
         if not self.validate(value):
             raise TypeError(f"Str must wrap a python str. Got {type(value)}")
         self.value = value
 
     def pack(self) -> bytes:
         fp = io.BytesIO()
-        fp.write(UInt(len(self.value)).pack())
-        fp.write(self.value.encode("utf-8"))
+        encoded = self.value.encode("utf-8")
+        fp.write(UInt(len(encoded)).pack())
+        fp.write(encoded)
         return fp.getbuffer()
 
     @classmethod
     def validate(cls, value: str) -> bool:
         return isinstance(value, (str, cls))
 
     @classmethod
```

### Comparing `pybare-1.0.1/bare/number.py` & `pybare-1.1.0/bare/number.py`

 * *Files identical despite different names*

### Comparing `pybare-1.0.1/bare/test_encoder.py` & `pybare-1.1.0/bare/test_encoder.py`

 * *Files identical despite different names*

### Comparing `pybare-1.0.1/bare/union.py` & `pybare-1.1.0/bare/union.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,17 @@
     # TODO: type annotations based on this
     value: Any
     _variants: dict[int, type]
     _discriminants: dict[type, int]
 
     def __init__(self, value: Any, *_args, **_kwargs):
         self.value = UnionValidator(self._variants)
+        if value is None:
+            # coerce None to Void for sanity
+            value = Void()
         if not self.validate(value):
             union_member_error(value, self._variants.values())
         self.value = value
 
     def pack(self: Union) -> bytes:
         buf = io.BytesIO()
         ty = type(self.value)
@@ -116,22 +119,22 @@
             return other.value == self.value
         for ty in self._variants.values():
             if ty.validate(other):
                 return other == ty(other)
         return NotImplemented
 
     def __repr__(self) -> str:
-        variants = " | ".join([repr(x) for x in self._variants.values()])
-        return f"{self.__class__.__name__}({variants}) = {self.value}"
+        return f"{self.__class__.__name__}({self.value})"
 
     def _type_to_discriminant(self, ty: type) -> int:
         try:
             return self._discriminants[ty]
         except KeyError:
             union_member_error(ty, self._variants.values())
+            raise
 
 
 class UnionVariant(Generic[T]):
     """
     Represents a variant of a union with an explici discriminator.
     Use in any place you would otherwise use a BARE type when defining variants
     of a `Union`
@@ -143,15 +146,15 @@
 
     def __init__(self, variant, discriminant: int):
         self.variant = variant
         self.discriminant = discriminant
 
 
 def union_member_error(t: type, variants: Iterable[type]):
-    variants = " | ".join([str(x) for x in variants])
+    variants = " | ".join([x.__name__ for x in variants])
     raise TypeError(
         f"Type {t} is not a valid variant for this union. "
         f"Valid options include {variants}"
     )
 
 
 def union(*variants: tuple[type, ...]) -> Type[Union]:
```

### Comparing `pybare-1.0.1/bare/util.py` & `pybare-1.1.0/bare/util.py`

 * *Files identical despite different names*

### Comparing `pybare-1.0.1/pybare.egg-info/PKG-INFO` & `pybare-1.1.0/pybare.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybare
-Version: 1.0.1
+Version: 1.1.0
 Summary: A declarative implementation of BARE for Python
 Home-page: https://sr.ht/~chiefnoah/PyBARE/
 Author: Noah Pederson
 Author-email: noah@packetlost.dev
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pybare-1.0.1/setup.py` & `pybare-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pybare",  # Replace with your own username
-    version="1.0.1",
+    version="1.1.0",
     author="Noah Pederson",
     author_email="noah@packetlost.dev",
     description="A declarative implementation of BARE for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://sr.ht/~chiefnoah/PyBARE/",
     packages=setuptools.find_packages(),
```

