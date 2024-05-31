# Comparing `tmp/rfc9457-0.0.8.tar.gz` & `tmp/rfc9457-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfc9457-0.0.8.tar", max compression
+gzip compressed data, was "rfc9457-0.0.9.tar", max compression
```

## Comparing `rfc9457-0.0.8.tar` & `rfc9457-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11307 2024-05-24 09:29:50.446730 rfc9457-0.0.8/LICENSE
--rw-r--r--   0        0        0     1789 2024-05-24 09:29:50.446730 rfc9457-0.0.8/README.md
--rw-r--r--   0        0        0     2021 2024-05-24 09:29:50.450730 rfc9457-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3308 2024-05-24 09:29:50.450730 rfc9457-0.0.8/src/rfc9457/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 09:29:50.450730 rfc9457-0.0.8/src/rfc9457/py.typed
--rw-r--r--   0        0        0     2451 1970-01-01 00:00:00.000000 rfc9457-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11307 2024-05-31 08:16:59.282453 rfc9457-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1789 2024-05-31 08:16:59.282453 rfc9457-0.0.9/README.md
+-rw-r--r--   0        0        0     2037 2024-05-31 08:16:59.282453 rfc9457-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3806 2024-05-31 08:16:59.282453 rfc9457-0.0.9/src/rfc9457/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 08:16:59.282453 rfc9457-0.0.9/src/rfc9457/py.typed
+-rw-r--r--   0        0        0     2476 1970-01-01 00:00:00.000000 rfc9457-0.0.9/PKG-INFO
```

### Comparing `rfc9457-0.0.8/LICENSE` & `rfc9457-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rfc9457-0.0.8/README.md` & `rfc9457-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `rfc9457-0.0.8/pyproject.toml` & `rfc9457-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [tool.poetry]
 name = "rfc9457"
-version = "0.0.8"
+version = "0.0.9"
 description = "Implementation of RFC9457 problems."
 authors = ["Daniel Edgecombe <daniel@nrwl.co>"]
 license = "Apache-2.0"
 repository="https://github.com/NRWLDev/rfc9457/"
 homepage="https://github.com/NRWLDev/rfc9457/"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
+multidict = "*"
 
 [tool.poetry.dev-dependencies]
 
 changelog-gen = { version="^0.9", extras=["bump-my-version"]}
 pytest = "~7.4.3"
 pytest-cov = "^4.1.0"
 pytest-random-order = "^1.0"
 
 # Style
 ruff = "^0.3"
 pre-commit = "^3.0.2"
 
 [tool.bumpversion]
-current_version = "0.0.8"
+current_version = "0.0.9"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `rfc9457-0.0.8/src/rfc9457/__init__.py` & `rfc9457-0.0.9/src/rfc9457/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 """
 
 from __future__ import annotations
 
 import re
 import typing as t
 
+from multidict import CIMultiDict
+
 CONVERT_RE = re.compile(r"(?<!^)(?=[A-Z])")
 
 
 def error_class_to_type(exc: Exception) -> str:
     """Convert an exception class name to a `problem-type` string."""
     type_ = "".join(exc.__class__.__name__.rsplit("Error", 1))
     return CONVERT_RE.sub("-", type_).lower()
@@ -28,15 +30,15 @@
 
     def __init__(  # noqa: PLR0913
         self: t.Self,
         title: str,
         type_: str | None = None,
         details: str | None = None,
         status: int = 500,
-        headers: dict[str, str] | None = None,
+        headers: CIMultiDict[str, str] | None = None,
         **kwargs,
     ) -> None:
         self._type = type_
         self.title = title
         self.details = details
         self.status = status
         self.status_code = status  # work around for sentry integrations that expect status_code attr
@@ -80,17 +82,22 @@
 
 
 class StatusProblem(Problem):
     code: str | None = None
     type_: str | None = None
     title: str = "Base http exception."
     status: int = 500
-    headers: dict[str, str] | None = None
+    headers: CIMultiDict[str, str] | None = None
 
-    def __init__(self: t.Self, details: str | None = None, headers: dict[str, str] | None = None, **kwargs) -> None:
+    def __init__(
+        self: t.Self,
+        details: str | None = None,
+        headers: CIMultiDict[str, str] | None = None,
+        **kwargs,
+    ) -> None:
         headers_ = (self.headers or {}).copy()
         if headers:
             headers_.update(headers)
 
         super().__init__(
             self.title,
             type_=self.type_ or self.code,
@@ -100,14 +107,29 @@
             **kwargs,
         )
 
 
 class ServerProblem(StatusProblem): ...
 
 
+class RedirectProblem(StatusProblem):
+    status = 301
+
+    def __init__(
+        self: t.Self,
+        location: str,
+        details: str | None = None,
+        headers: CIMultiDict[str, str] | None = None,
+        **kwargs,
+    ) -> None:
+        headers_ = CIMultiDict(Location=location)
+        headers_.update(headers or {})
+        super().__init__(details=details, headers=headers_, **kwargs)
+
+
 class BadRequestProblem(StatusProblem):
     status = 400
 
 
 class UnauthorisedProblem(StatusProblem):
     status = 401
```

### Comparing `rfc9457-0.0.8/PKG-INFO` & `rfc9457-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: rfc9457
-Version: 0.0.8
+Version: 0.0.9
 Summary: Implementation of RFC9457 problems.
 Home-page: https://github.com/NRWLDev/rfc9457/
 License: Apache-2.0
 Author: Daniel Edgecombe
 Author-email: daniel@nrwl.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: multidict
 Project-URL: Repository, https://github.com/NRWLDev/rfc9457/
 Description-Content-Type: text/markdown
 
 # RFC9457 implementation for Python
 [![image](https://img.shields.io/pypi/v/rfc9457.svg)](https://pypi.org/project/rfc9457/)
 [![image](https://img.shields.io/pypi/l/rfc9457.svg)](https://pypi.org/project/rfc9457/)
 [![image](https://img.shields.io/pypi/pyversions/rfc9457.svg)](https://pypi.org/project/rfc9457/)
```

