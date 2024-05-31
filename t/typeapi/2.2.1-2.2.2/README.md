# Comparing `tmp/typeapi-2.2.1.tar.gz` & `tmp/typeapi-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typeapi-2.2.1.tar", max compression
+gzip compressed data, was "typeapi-2.2.2.tar", max compression
```

## Comparing `typeapi-2.2.1.tar` & `typeapi-2.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      991 2023-06-11 20:15:18.012081 typeapi-2.2.1/LICENSE
--rw-r--r--   0        0        0     1049 2024-03-18 14:43:32.286566 typeapi-2.2.1/README.md
--rw-r--r--   0        0        0     1991 2024-03-18 14:51:35.053031 typeapi-2.2.1/pyproject.toml
--rw-r--r--   0        0        0      644 2024-03-18 14:51:35.053176 typeapi-2.2.1/src/typeapi/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 14:04:49.591433 typeapi-2.2.1/src/typeapi/backport/__init__.py
--rw-r--r--   0        0        0     4883 2023-06-11 20:15:18.015669 typeapi-2.2.1/src/typeapi/backport/inspect.py
--rw-r--r--   0        0        0        0 2024-03-18 14:04:49.592505 typeapi-2.2.1/src/typeapi/future/__init__.py
--rw-r--r--   0        0        0     5210 2024-03-18 14:04:49.593289 typeapi-2.2.1/src/typeapi/future/astrewrite.py
--rw-r--r--   0        0        0      765 2024-03-18 14:04:49.593633 typeapi-2.2.1/src/typeapi/future/astrewrite_test.py
--rw-r--r--   0        0        0     3723 2024-03-18 14:04:49.594150 typeapi-2.2.1/src/typeapi/future/fake.py
--rw-r--r--   0        0        0     1965 2024-03-18 14:04:49.595220 typeapi-2.2.1/src/typeapi/future/fake_test.py
--rw-r--r--   0        0        0        0 2023-06-11 20:15:18.016850 typeapi-2.2.1/src/typeapi/py.typed
--rw-r--r--   0        0        0    21609 2024-03-18 14:50:29.899989 typeapi-2.2.1/src/typeapi/typehint.py
--rw-r--r--   0        0        0    18002 2023-07-10 15:21:16.380134 typeapi-2.2.1/src/typeapi/typehint_test.py
--rw-r--r--   0        0        0    13464 2024-03-18 14:50:29.867283 typeapi-2.2.1/src/typeapi/utils.py
--rw-r--r--   0        0        0    16290 2024-03-18 10:51:38.262922 typeapi-2.2.1/src/typeapi/utils_test.py
--rw-r--r--   0        0        0     1892 1970-01-01 00:00:00.000000 typeapi-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0      991 2024-05-31 11:19:30.842857 typeapi-2.2.2/LICENSE
+-rw-r--r--   0        0        0     1049 2024-05-31 11:19:30.843192 typeapi-2.2.2/README.md
+-rw-r--r--   0        0        0     1991 2024-05-31 12:08:15.541630 typeapi-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0      644 2024-05-31 12:08:15.541834 typeapi-2.2.2/src/typeapi/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 11:19:30.851552 typeapi-2.2.2/src/typeapi/backport/__init__.py
+-rw-r--r--   0        0        0     4883 2024-05-31 11:19:30.851882 typeapi-2.2.2/src/typeapi/backport/inspect.py
+-rw-r--r--   0        0        0        0 2024-05-31 11:19:30.852135 typeapi-2.2.2/src/typeapi/future/__init__.py
+-rw-r--r--   0        0        0     5210 2024-05-31 11:19:30.852349 typeapi-2.2.2/src/typeapi/future/astrewrite.py
+-rw-r--r--   0        0        0      765 2024-05-31 11:19:30.852527 typeapi-2.2.2/src/typeapi/future/astrewrite_test.py
+-rw-r--r--   0        0        0     3723 2024-05-31 11:19:30.852714 typeapi-2.2.2/src/typeapi/future/fake.py
+-rw-r--r--   0        0        0     1965 2024-05-31 11:19:30.852899 typeapi-2.2.2/src/typeapi/future/fake_test.py
+-rw-r--r--   0        0        0        0 2024-05-31 11:19:30.853043 typeapi-2.2.2/src/typeapi/py.typed
+-rw-r--r--   0        0        0    21758 2024-05-31 12:07:53.624891 typeapi-2.2.2/src/typeapi/typehint.py
+-rw-r--r--   0        0        0    18312 2024-05-31 12:07:51.422032 typeapi-2.2.2/src/typeapi/typehint_test.py
+-rw-r--r--   0        0        0    13898 2024-05-31 12:07:51.423515 typeapi-2.2.2/src/typeapi/utils.py
+-rw-r--r--   0        0        0    16290 2024-05-31 11:19:30.855810 typeapi-2.2.2/src/typeapi/utils_test.py
+-rw-r--r--   0        0        0     1892 1970-01-01 00:00:00.000000 typeapi-2.2.2/PKG-INFO
```

### Comparing `typeapi-2.2.1/LICENSE` & `typeapi-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `typeapi-2.2.1/README.md` & `typeapi-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `typeapi-2.2.1/pyproject.toml` & `typeapi-2.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # NOTE(NiklasRosenstein): We pin this version so we can keep using the old way that Slap supports installing
 #                         the "docs" extra without Poetry complaining about invalid format of the requirements.
 requires = ["poetry-core>=1.1.0a6"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "typeapi"
-version = "2.2.1"
+version = "2.2.2"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "typeapi", from = "src" }]
 classifiers = []
 keywords = []
@@ -26,15 +26,15 @@
 typing-extensions = ">=3.0.0"
 
 [tool.poetry.dev-dependencies]
 mypy = "*"
 pytest = "*"
 types-dataclasses = "^0.6.5"
 isort = "^5.10.1"
-flake8 = "^5.0.4"
+flake8 = "^7.0.0"
 black = "^24.0.0"
 astor = "^0.8.1"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
```

### Comparing `typeapi-2.2.1/src/typeapi/__init__.py` & `typeapi-2.2.2/src/typeapi/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.2.1"
+__version__ = "2.2.2"
 
 from .typehint import (
     AnnotatedTypeHint,
     ClassTypeHint,
     ForwardRefTypeHint,
     LiteralTypeHint,
     TupleTypeHint,
```

### Comparing `typeapi-2.2.1/src/typeapi/backport/inspect.py` & `typeapi-2.2.2/src/typeapi/backport/inspect.py`

 * *Files identical despite different names*

### Comparing `typeapi-2.2.1/src/typeapi/future/astrewrite.py` & `typeapi-2.2.2/src/typeapi/future/astrewrite.py`

 * *Files identical despite different names*

### Comparing `typeapi-2.2.1/src/typeapi/future/astrewrite_test.py` & `typeapi-2.2.2/src/typeapi/future/astrewrite_test.py`

 * *Files identical despite different names*

### Comparing `typeapi-2.2.1/src/typeapi/future/fake.py` & `typeapi-2.2.2/src/typeapi/future/fake.py`

 * *Files identical despite different names*

### Comparing `typeapi-2.2.1/src/typeapi/future/fake_test.py` & `typeapi-2.2.2/src/typeapi/future/fake_test.py`

 * *Files identical despite different names*

### Comparing `typeapi-2.2.1/src/typeapi/typehint.py` & `typeapi-2.2.2/src/typeapi/typehint.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     ForwardRef,
     HasGetitem,
     get_subscriptable_type_hint_from_origin,
     get_type_hint_args,
     get_type_hint_origin_or_none,
     get_type_hint_original_bases,
     get_type_hint_parameters,
+    is_new_type,
     type_repr,
 )
 
 NoneType = type(None)
 
 
 class _TypeHintMeta(abc.ABCMeta):
@@ -168,15 +169,15 @@
         """
         The object from which on which the type hint was found, for example a class or a function.
         """
 
         return self._source
 
     def __eq__(self, other: object) -> bool:
-        if type(self) != type(other):
+        if type(self) is not type(other):
             return False
         assert isinstance(other, TypeHint)
         return (self.hint, self.origin, self.args, self.parameters) == (
             other.hint,
             other.origin,
             other.args,
             other.parameters,
@@ -281,32 +282,35 @@
 
 
 class ClassTypeHint(TypeHint):
     """Represents a real, possibly parameterized, type. For example `int`, `list`, `list[int]` or `list[T]`."""
 
     def __init__(self, hint: object, source: "Any | None" = None) -> None:
         super().__init__(hint, source)
-        assert isinstance(self.hint, type) or isinstance(self.origin, type), (
-            "ClassTypeHint must be initialized from a real type or a generic that points to a real type. "
-            f'Got "{self.hint!r}" with origin "{self.origin}"'
-        )
+        if not is_new_type(hint):
+            assert isinstance(self.hint, type) or isinstance(self.origin, type), (
+                "ClassTypeHint must be initialized from a real type or a generic that points to a real type. "
+                f'Got "{self.hint!r}" with origin "{self.origin}"'
+            )
 
     def parameterize(self, parameter_map: Mapping[object, Any]) -> "TypeHint":
         if self.type is Generic:  # type: ignore[comparison-overlap]
             return self
         return super().parameterize(parameter_map)
 
     @property
     def type(self) -> type:
         """Returns the concrepte type."""
 
         if isinstance(self.origin, type):
             return self.origin
         if isinstance(self.hint, type):
             return self.hint
+        if is_new_type(self.hint):
+            return self.hint.__supertype__
         assert False, "ClassTypeHint not initialized from a real type or a generic that points to a real type."
 
     @property
     def bases(self) -> "Tuple[Any, ...]":
         """
         Return the bases of the classes' types. If the type is a generic, the bases of the generic's origin are
         returned in their parameterized form (e.g. `Generic[T]` instead of `Generic` is returned).
```

### Comparing `typeapi-2.2.1/src/typeapi/typehint_test.py` & `typeapi-2.2.2/src/typeapi/typehint_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, ClassVar, Dict, Generic, List, Optional, Sequence, Tuple, TypeVar, Union
+from typing import Any, ClassVar, Dict, Generic, List, NewType, Optional, Sequence, Tuple, TypeVar, Union
 
 from pytest import mark
 from typing_extensions import Annotated, Literal, TypeAlias
 
 from typeapi.typehint import (
     AnnotatedTypeHint,
     ClassTypeHint,
@@ -259,14 +259,25 @@
     assert isinstance(hint, UnionTypeHint)
     assert hint.hint == Optional[int]
     assert hint.origin is Union
     assert hint.args == (int, type(None))
     assert hint.parameters == ()
 
 
+def test__TypeHint__from_newtype() -> None:
+    MyInt = NewType("MyInt", int)
+    hint = TypeHint(MyInt)
+    assert isinstance(hint, ClassTypeHint)
+    assert hint.args == ()
+    assert hint.bases == (object,)
+    assert hint.origin is None
+    assert hint.type is int
+    assert hint.hint is MyInt
+
+
 def test__ClassTypeHint__parametrize() -> None:
     """This method tests the infusion of type parameters into other types.
 
     This is relevant when you want to carry over a type parameter into the
     fields of a type, such as in dataclasses."""
 
     from dataclasses import dataclass, fields
```

### Comparing `typeapi-2.2.1/src/typeapi/utils.py` & `typeapi-2.2.2/src/typeapi/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -380,7 +380,22 @@
         if hasattr(m, "_TypedDictMeta") and isinstance(hint, m._TypedDictMeta):  # type: ignore[attr-defined]
             return True
     return False
 
 
 class HasGetitem(Protocol, Generic[T_contra, U_co]):
     def __getitem__(self, __key: T_contra) -> U_co: ...
+
+
+class NewTypeP(Protocol):
+    """
+    Protocol for objects returned by `typing.NewType`.
+    """
+
+    __name__: str
+    __supertype__: type
+
+
+def is_new_type(hint: Any) -> TypeGuard[NewTypeP]:
+    # NOTE: Starting with Python 3.10, `typing.NewType` is actually a class instead of a function, but it is
+    #       still typed as a function in Mypy until 3.12.
+    return hasattr(hint, "__name__") and hasattr(hint, "__supertype__")
```

### Comparing `typeapi-2.2.1/src/typeapi/utils_test.py` & `typeapi-2.2.2/src/typeapi/utils_test.py`

 * *Files identical despite different names*

### Comparing `typeapi-2.2.1/PKG-INFO` & `typeapi-2.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeapi
-Version: 2.2.1
+Version: 2.2.2
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

