# Comparing `tmp/mypy-boto3-codeguru-security-1.34.0.tar.gz` & `tmp/mypy_boto3_codeguru_security-1.34.117.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codeguru-security-1.34.0.tar", last modified: Wed Dec 13 21:22:15 2023, max compression
+gzip compressed data, was "mypy_boto3_codeguru_security-1.34.117.tar", last modified: Fri May 31 19:47:09 2024, max compression
```

## Comparing `mypy-boto3-codeguru-security-1.34.0.tar` & `mypy_boto3_codeguru_security-1.34.117.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:15.671164 mypy-boto3-codeguru-security-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:07:21.000000 mypy-boto3-codeguru-security-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13512 2023-12-13 21:22:15.671164 mypy-boto3-codeguru-security-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11940 2023-12-13 21:07:21.000000 mypy-boto3-codeguru-security-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:15.671164 mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2023-12-13 21:07:21.000000 mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2023-12-13 21:07:21.000000 mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      943 2023-12-13 21:07:21.000000 mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12832 2023-12-13 21:07:21.000000 mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12828 2023-12-13 21:07:21.000000 mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9033 2023-12-13 21:07:21.000000 mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2023-12-13 21:07:21.000000 mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2023-12-13 21:07:21.000000 mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2023-12-13 21:07:21.000000 mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:07:21.000000 mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13313 2023-12-13 21:07:21.000000 mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13312 2023-12-13 21:07:21.000000 mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:07:21.000000 mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:15.671164 mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13512 2023-12-13 21:22:15.000000 mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-13 21:22:15.000000 mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:15.000000 mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:15.000000 mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:22:15.000000 mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 21:22:15.000000 mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:22:15.671164 mypy-boto3-codeguru-security-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2023-12-13 21:07:21.000000 mypy-boto3-codeguru-security-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:47:09.169631 mypy_boto3_codeguru_security-1.34.117/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-31 19:46:52.000000 mypy_boto3_codeguru_security-1.34.117/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13538 2024-05-31 19:47:09.169631 mypy_boto3_codeguru_security-1.34.117/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-05-31 19:46:52.000000 mypy_boto3_codeguru_security-1.34.117/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:47:09.169631 mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-31 19:46:52.000000 mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-31 19:46:52.000000 mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-31 19:46:52.000000 mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12923 2024-05-31 19:46:52.000000 mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-05-31 19:46:52.000000 mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-05-31 19:46:53.000000 mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-05-31 19:46:53.000000 mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-05-31 19:46:53.000000 mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-31 19:46:53.000000 mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 19:46:52.000000 mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13354 2024-05-31 19:46:53.000000 mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13354 2024-05-31 19:46:53.000000 mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-31 19:46:52.000000 mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:47:09.169631 mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13538 2024-05-31 19:47:09.000000 mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-31 19:47:09.000000 mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 19:47:09.000000 mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 19:47:09.000000 mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-31 19:47:09.000000 mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-31 19:47:09.000000 mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 19:47:09.169631 mypy_boto3_codeguru_security-1.34.117/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-31 19:46:52.000000 mypy_boto3_codeguru_security-1.34.117/setup.py
```

### Comparing `mypy-boto3-codeguru-security-1.34.0/LICENSE` & `mypy_boto3_codeguru_security-1.34.117/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-codeguru-security-1.34.0/PKG-INFO` & `mypy_boto3_codeguru_security-1.34.117/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguru-security
-Version: 1.34.0
-Summary: Type annotations for boto3.CodeGuruSecurity 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.117
+Summary: Type annotations for boto3.CodeGuruSecurity 1.34.117 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-codeguru-security"></a>
 
 # mypy-boto3-codeguru-security
 
 [![PyPI - mypy-boto3-codeguru-security](https://img.shields.io/pypi/v/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguru-security)](https://pepy.tech/project/mypy-boto3-codeguru-security)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruSecurity 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
+[boto3.CodeGuruSecurity 1.34.117](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeguru-security docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-codeguru-security-1.34.0/README.md` & `mypy_boto3_codeguru_security-1.34.117/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguru-security)](https://pepy.tech/project/mypy-boto3-codeguru-security)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruSecurity 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
+[boto3.CodeGuruSecurity 1.34.117](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeguru-security docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/__init__.py` & `mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 """
 
 from .client import CodeGuruSecurityClient
 from .paginator import GetFindingsPaginator, ListFindingsMetricsPaginator, ListScansPaginator
 
 Client = CodeGuruSecurityClient
 
-
 __all__ = (
     "Client",
     "CodeGuruSecurityClient",
     "GetFindingsPaginator",
     "ListFindingsMetricsPaginator",
     "ListScansPaginator",
 )
```

### Comparing `mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/__init__.pyi` & `mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/__main__.py` & `mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeGuruSecurity 1.34.0\nVersion:         1.34.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security//\nBoto3 docs:   "
-        "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.CodeGuruSecurity 1.34.117\n"
+        "Version:         1.34.117\n"
+        "Builder version: 7.24.0\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.0")
+    print("1.34.117")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/client.py` & `mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CodeGuruSecurityClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -83,15 +82,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#exceptions)
         """
 
     def batch_get_findings(
         self, *, findingIdentifiers: Sequence[FindingIdentifierTypeDef]
     ) -> BatchGetFindingsResponseTypeDef:
         """
-        Returns a list of all requested findings.
+        Returns a list of requested findings from standard scans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.batch_get_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#batch_get_findings)
         """
 
     def can_paginate(self, operation_name: str) -> bool:
         """
@@ -113,26 +112,28 @@
         self,
         *,
         resourceId: ResourceIdTypeDef,
         scanName: str,
         analysisType: AnalysisTypeType = ...,
         clientToken: str = ...,
         scanType: ScanTypeType = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateScanResponseTypeDef:
         """
-        Use to create a scan using code uploaded to an S3 bucket.
+        Use to create a scan using code uploaded to an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.create_scan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#create_scan)
         """
 
     def create_upload_url(self, *, scanName: str) -> CreateUploadUrlResponseTypeDef:
         """
-        Generates a pre-signed URL and request headers used to upload a code resource.
+        Generates a pre-signed URL, request headers used to upload a code resource, and
+        code artifact identifier for the uploaded
+        resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.create_upload_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#create_upload_url)
         """
 
     def generate_presigned_url(
         self,
@@ -146,38 +147,38 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#generate_presigned_url)
         """
 
     def get_account_configuration(self) -> GetAccountConfigurationResponseTypeDef:
         """
-        Use to get account level configuration.
+        Use to get the encryption configuration for an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.get_account_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#get_account_configuration)
         """
 
     def get_findings(
         self,
         *,
         scanName: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        status: StatusType = ...
+        status: StatusType = ...,
     ) -> GetFindingsResponseTypeDef:
         """
         Returns a list of all findings generated by a particular scan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.get_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#get_findings)
         """
 
     def get_metrics_summary(self, *, date: TimestampTypeDef) -> GetMetricsSummaryResponseTypeDef:
         """
-        Returns top level metrics about an account from a specified date, including
+        Returns a summary of metrics for an account from a specified date, including
         number of open findings, the categories with most findings, the scans with most
         open findings, and scans with most open critical
         findings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.get_metrics_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#get_metrics_summary)
         """
@@ -192,28 +193,28 @@
 
     def list_findings_metrics(
         self,
         *,
         endDate: TimestampTypeDef,
         startDate: TimestampTypeDef,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListFindingsMetricsResponseTypeDef:
         """
         Returns metrics about all findings in an account within a specified time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.list_findings_metrics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#list_findings_metrics)
         """
 
     def list_scans(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListScansResponseTypeDef:
         """
-        Returns a list of all the standard scans in an account.
+        Returns a list of all scans in an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.list_scans)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#list_scans)
         """
 
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
@@ -239,15 +240,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#untag_resource)
         """
 
     def update_account_configuration(
         self, *, encryptionConfig: EncryptionConfigTypeDef
     ) -> UpdateAccountConfigurationResponseTypeDef:
         """
-        Use to update account-level configuration with an encryption key.
+        Use to update the encryption configuration for an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.update_account_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#update_account_configuration)
         """
 
     @overload
     def get_paginator(self, operation_name: Literal["get_findings"]) -> GetFindingsPaginator:
```

### Comparing `mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/client.pyi` & `mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#exceptions)
         """
 
     def batch_get_findings(
         self, *, findingIdentifiers: Sequence[FindingIdentifierTypeDef]
     ) -> BatchGetFindingsResponseTypeDef:
         """
-        Returns a list of all requested findings.
+        Returns a list of requested findings from standard scans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.batch_get_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#batch_get_findings)
         """
 
     def can_paginate(self, operation_name: str) -> bool:
         """
@@ -109,26 +109,28 @@
         self,
         *,
         resourceId: ResourceIdTypeDef,
         scanName: str,
         analysisType: AnalysisTypeType = ...,
         clientToken: str = ...,
         scanType: ScanTypeType = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateScanResponseTypeDef:
         """
-        Use to create a scan using code uploaded to an S3 bucket.
+        Use to create a scan using code uploaded to an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.create_scan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#create_scan)
         """
 
     def create_upload_url(self, *, scanName: str) -> CreateUploadUrlResponseTypeDef:
         """
-        Generates a pre-signed URL and request headers used to upload a code resource.
+        Generates a pre-signed URL, request headers used to upload a code resource, and
+        code artifact identifier for the uploaded
+        resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.create_upload_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#create_upload_url)
         """
 
     def generate_presigned_url(
         self,
@@ -142,38 +144,38 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#generate_presigned_url)
         """
 
     def get_account_configuration(self) -> GetAccountConfigurationResponseTypeDef:
         """
-        Use to get account level configuration.
+        Use to get the encryption configuration for an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.get_account_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#get_account_configuration)
         """
 
     def get_findings(
         self,
         *,
         scanName: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        status: StatusType = ...
+        status: StatusType = ...,
     ) -> GetFindingsResponseTypeDef:
         """
         Returns a list of all findings generated by a particular scan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.get_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#get_findings)
         """
 
     def get_metrics_summary(self, *, date: TimestampTypeDef) -> GetMetricsSummaryResponseTypeDef:
         """
-        Returns top level metrics about an account from a specified date, including
+        Returns a summary of metrics for an account from a specified date, including
         number of open findings, the categories with most findings, the scans with most
         open findings, and scans with most open critical
         findings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.get_metrics_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#get_metrics_summary)
         """
@@ -188,28 +190,28 @@
 
     def list_findings_metrics(
         self,
         *,
         endDate: TimestampTypeDef,
         startDate: TimestampTypeDef,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListFindingsMetricsResponseTypeDef:
         """
         Returns metrics about all findings in an account within a specified time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.list_findings_metrics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#list_findings_metrics)
         """
 
     def list_scans(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListScansResponseTypeDef:
         """
-        Returns a list of all the standard scans in an account.
+        Returns a list of all scans in an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.list_scans)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#list_scans)
         """
 
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
@@ -235,15 +237,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#untag_resource)
         """
 
     def update_account_configuration(
         self, *, encryptionConfig: EncryptionConfigTypeDef
     ) -> UpdateAccountConfigurationResponseTypeDef:
         """
-        Use to update account-level configuration with an encryption key.
+        Use to update the encryption configuration for an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.update_account_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/client/#update_account_configuration)
         """
 
     @overload
     def get_paginator(self, operation_name: Literal["get_findings"]) -> GetFindingsPaginator:
```

### Comparing `mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/literals.py` & `mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AnalysisTypeType",
     "ErrorCodeType",
     "GetFindingsPaginatorName",
     "ListFindingsMetricsPaginatorName",
     "ListScansPaginatorName",
     "ScanStateType",
@@ -32,15 +31,14 @@
     "StatusType",
     "CodeGuruSecurityServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 AnalysisTypeType = Literal["All", "Security"]
 ErrorCodeType = Literal[
     "DUPLICATE_IDENTIFIER",
     "INTERNAL_ERROR",
     "INVALID_FINDING_ID",
     "INVALID_SCAN_NAME",
     "ITEM_DOES_NOT_EXIST",
@@ -75,14 +73,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -93,14 +92,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -118,14 +118,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -138,24 +139,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -216,15 +219,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -266,14 +268,15 @@
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie2",
+    "mailmanager",
     "managedblockchain",
     "managedblockchain-query",
     "marketplace-agreement",
     "marketplace-catalog",
     "marketplace-deployment",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
@@ -296,17 +299,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -351,14 +356,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -396,19 +402,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/literals.pyi` & `mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -91,14 +92,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -116,14 +118,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -136,24 +139,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -214,15 +219,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -264,14 +268,15 @@
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie2",
+    "mailmanager",
     "managedblockchain",
     "managedblockchain-query",
     "marketplace-agreement",
     "marketplace-catalog",
     "marketplace-deployment",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
@@ -294,17 +299,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -349,14 +356,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -394,19 +402,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/paginator.py` & `mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     ListScansResponseTypeDef,
     PaginatorConfigTypeDef,
     TimestampTypeDef,
 )
 
 __all__ = ("GetFindingsPaginator", "ListFindingsMetricsPaginator", "ListScansPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -57,15 +56,15 @@
     """
 
     def paginate(
         self,
         *,
         scanName: str,
         status: StatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[GetFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.GetFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/paginators/#getfindingspaginator)
         """
 
 
@@ -76,15 +75,15 @@
     """
 
     def paginate(
         self,
         *,
         endDate: TimestampTypeDef,
         startDate: TimestampTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListFindingsMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListFindingsMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/paginators/#listfindingsmetricspaginator)
         """
```

### Comparing `mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/paginator.pyi` & `mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     """
 
     def paginate(
         self,
         *,
         scanName: str,
         status: StatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[GetFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.GetFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/paginators/#getfindingspaginator)
         """
 
 class ListFindingsMetricsPaginator(Paginator):
@@ -72,15 +72,15 @@
     """
 
     def paginate(
         self,
         *,
         endDate: TimestampTypeDef,
         startDate: TimestampTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListFindingsMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListFindingsMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/paginators/#listfindingsmetricspaginator)
         """
 
 class ListScansPaginator(Paginator):
```

### Comparing `mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/type_defs.py` & `mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "FindingMetricsValuePerSeverityTypeDef",
     "BatchGetFindingsErrorTypeDef",
     "FindingIdentifierTypeDef",
     "ResponseMetadataTypeDef",
     "CategoryWithFindingNumTypeDef",
     "CodeLineTypeDef",
@@ -111,18 +110,18 @@
         "scanName": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 CategoryWithFindingNumTypeDef = TypedDict(
     "CategoryWithFindingNumTypeDef",
     {
         "categoryName": NotRequired[str],
         "findingNumber": NotRequired[int],
@@ -270,14 +269,15 @@
     },
 )
 GetScanResponseTypeDef = TypedDict(
     "GetScanResponseTypeDef",
     {
         "analysisType": AnalysisTypeType,
         "createdAt": datetime,
+        "errorMessage": str,
         "numberOfRevisions": int,
         "runId": str,
         "scanName": str,
         "scanNameArn": str,
         "scanState": ScanStateType,
         "updatedAt": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security/type_defs.pyi` & `mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -110,18 +110,18 @@
         "scanName": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 CategoryWithFindingNumTypeDef = TypedDict(
     "CategoryWithFindingNumTypeDef",
     {
         "categoryName": NotRequired[str],
         "findingNumber": NotRequired[int],
@@ -269,14 +269,15 @@
     },
 )
 GetScanResponseTypeDef = TypedDict(
     "GetScanResponseTypeDef",
     {
         "analysisType": AnalysisTypeType,
         "createdAt": datetime,
+        "errorMessage": str,
         "numberOfRevisions": int,
         "runId": str,
         "scanName": str,
         "scanNameArn": str,
         "scanState": ScanStateType,
         "updatedAt": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security.egg-info/PKG-INFO` & `mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguru-security
-Version: 1.34.0
-Summary: Type annotations for boto3.CodeGuruSecurity 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.117
+Summary: Type annotations for boto3.CodeGuruSecurity 1.34.117 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-codeguru-security"></a>
 
 # mypy-boto3-codeguru-security
 
 [![PyPI - mypy-boto3-codeguru-security](https://img.shields.io/pypi/v/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguru-security)](https://pepy.tech/project/mypy-boto3-codeguru-security)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruSecurity 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
+[boto3.CodeGuruSecurity 1.34.117](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeguru-security docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-codeguru-security-1.34.0/mypy_boto3_codeguru_security.egg-info/SOURCES.txt` & `mypy_boto3_codeguru_security-1.34.117/mypy_boto3_codeguru_security.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.34.0/setup.py` & `mypy_boto3_codeguru_security-1.34.117/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codeguru-security",
-    version="1.34.0",
+    version="1.34.117",
     packages=["mypy_boto3_codeguru_security"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.CodeGuruSecurity 1.34.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
-    ),
+    description="Type annotations for boto3.CodeGuruSecurity 1.34.117 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="boto3 codeguru-security type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_codeguru_security": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

