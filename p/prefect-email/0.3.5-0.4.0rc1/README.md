# Comparing `tmp/prefect_email-0.3.5.tar.gz` & `tmp/prefect_email-0.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_email-0.3.5.tar", last modified: Thu May 16 20:58:36 2024, max compression
+gzip compressed data, was "prefect_email-0.4.0rc1.tar", last modified: Fri May 31 20:49:41 2024, max compression
```

## Comparing `prefect_email-0.3.5.tar` & `prefect_email-0.4.0rc1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:36.100809 prefect_email-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-16 20:58:24.000000 prefect_email-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 20:58:24.000000 prefect_email-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7099 2024-05-16 20:58:36.100809 prefect_email-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-05-16 20:58:24.000000 prefect_email-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:36.096809 prefect_email-0.3.5/prefect_email/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-16 20:58:24.000000 prefect_email-0.3.5/prefect_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 20:58:35.000000 prefect_email-0.3.5/prefect_email/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6479 2024-05-16 20:58:24.000000 prefect_email-0.3.5/prefect_email/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-16 20:58:24.000000 prefect_email-0.3.5/prefect_email/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:36.096809 prefect_email-0.3.5/prefect_email.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7099 2024-05-16 20:58:35.000000 prefect_email-0.3.5/prefect_email.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-16 20:58:36.000000 prefect_email-0.3.5/prefect_email.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:58:35.000000 prefect_email-0.3.5/prefect_email.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-16 20:58:35.000000 prefect_email-0.3.5/prefect_email.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-16 20:58:35.000000 prefect_email-0.3.5/prefect_email.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 20:58:35.000000 prefect_email-0.3.5/prefect_email.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-16 20:58:24.000000 prefect_email-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:58:36.100809 prefect_email-0.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:36.096809 prefect_email-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 20:58:24.000000 prefect_email-0.3.5/tests/attachment.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-16 20:58:24.000000 prefect_email-0.3.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-16 20:58:24.000000 prefect_email-0.3.5/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-16 20:58:24.000000 prefect_email-0.3.5/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-16 20:58:24.000000 prefect_email-0.3.5/tests/test_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-16 20:58:24.000000 prefect_email-0.3.5/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:41.213826 prefect_email-0.4.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-31 20:49:28.000000 prefect_email-0.4.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-31 20:49:28.000000 prefect_email-0.4.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-05-31 20:49:41.213826 prefect_email-0.4.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-05-31 20:49:28.000000 prefect_email-0.4.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:41.209826 prefect_email-0.4.0rc1/prefect_email/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-31 20:49:28.000000 prefect_email-0.4.0rc1/prefect_email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-31 20:49:40.000000 prefect_email-0.4.0rc1/prefect_email/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-31 20:49:28.000000 prefect_email-0.4.0rc1/prefect_email/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-31 20:49:28.000000 prefect_email-0.4.0rc1/prefect_email/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:41.209826 prefect_email-0.4.0rc1/prefect_email.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-05-31 20:49:40.000000 prefect_email-0.4.0rc1/prefect_email.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-31 20:49:41.000000 prefect_email-0.4.0rc1/prefect_email.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:49:40.000000 prefect_email-0.4.0rc1/prefect_email.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-31 20:49:40.000000 prefect_email-0.4.0rc1/prefect_email.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-31 20:49:40.000000 prefect_email-0.4.0rc1/prefect_email.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-31 20:49:40.000000 prefect_email-0.4.0rc1/prefect_email.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-31 20:49:28.000000 prefect_email-0.4.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:49:41.213826 prefect_email-0.4.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:41.209826 prefect_email-0.4.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-31 20:49:28.000000 prefect_email-0.4.0rc1/tests/attachment.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-31 20:49:28.000000 prefect_email-0.4.0rc1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-31 20:49:28.000000 prefect_email-0.4.0rc1/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-31 20:49:28.000000 prefect_email-0.4.0rc1/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-31 20:49:28.000000 prefect_email-0.4.0rc1/tests/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-31 20:49:28.000000 prefect_email-0.4.0rc1/tests/test_version.py
```

### Comparing `prefect_email-0.3.5/LICENSE` & `prefect_email-0.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_email-0.3.5/PKG-INFO` & `prefect_email-0.4.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 Metadata-Version: 2.1
 Name: prefect-email
-Version: 0.3.5
+Version: 0.4.0rc1
 Summary: Prefect integrations for interacting with email.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-email
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: prefect<3.0.0,>=2.14.10
+Requires-Dist: prefect>=3.0.0rc1
 Provides-Extra: dev
 Requires-Dist: aiohttp; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: mock; python_version < "3.8" and extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pillow; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 
@@ -137,15 +135,15 @@
 
 ```bash
 prefect block register -m prefect_email
 ```
 
 Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://docs.prefect.io/ui/blocks/).
 
-Requires an installation of Python 3.8+.
+Requires an installation of Python 3.9+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
 These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Saving credentials to block
```

### Comparing `prefect_email-0.3.5/README.md` & `prefect_email-0.4.0rc1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
 ```bash
 prefect block register -m prefect_email
 ```
 
 Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://docs.prefect.io/ui/blocks/).
 
-Requires an installation of Python 3.8+.
+Requires an installation of Python 3.9+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
 These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Saving credentials to block
```

### Comparing `prefect_email-0.3.5/prefect_email/credentials.py` & `prefect_email-0.4.0rc1/prefect_email/credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,18 @@
 
 import ssl
 from enum import Enum
 from functools import partial
 from smtplib import SMTP, SMTP_SSL
 from typing import Optional, Union
 
-from pydantic import VERSION as PYDANTIC_VERSION
+from pydantic import Field, SecretStr, field_validator
 
 from prefect.blocks.core import Block
 
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field, SecretStr, validator
-else:
-    from pydantic import Field, SecretStr, validator
-
 
 class SMTPType(Enum):
     """
     Protocols used to secure email transmissions.
     """
 
     SSL = 465
@@ -129,23 +124,24 @@
     )
     smtp_port: Optional[int] = Field(
         default=None,
         description=("If provided, overrides the smtp_type's default port number."),
         title="SMTP Port",
     )
 
-    @validator("smtp_server", pre=True)
-    def _cast_smtp_server(cls, value):
+    @field_validator("smtp_server", mode="before")
+    def _cast_smtp_server(cls, value: str):
         """
         Cast the smtp_server to an SMTPServer Enum member, if valid.
         """
         return _cast_to_enum(value, SMTPServer)
 
-    @validator("smtp_type", pre=True)
-    def _cast_smtp_type(cls, value):
+    @field_validator("smtp_type", mode="before")
+    @classmethod
+    def _cast_smtp_type(cls, value: str):
         """
         Cast the smtp_type to an SMTPType Enum member, if valid.
         """
         if isinstance(value, int):
             return SMTPType(value)
         return _cast_to_enum(value, SMTPType, restrict=True)
```

### Comparing `prefect_email-0.3.5/prefect_email/message.py` & `prefect_email-0.4.0rc1/prefect_email/message.py`

 * *Files identical despite different names*

### Comparing `prefect_email-0.3.5/prefect_email.egg-info/PKG-INFO` & `prefect_email-0.4.0rc1/prefect_email.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 Metadata-Version: 2.1
 Name: prefect-email
-Version: 0.3.5
+Version: 0.4.0rc1
 Summary: Prefect integrations for interacting with email.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-email
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: prefect<3.0.0,>=2.14.10
+Requires-Dist: prefect>=3.0.0rc1
 Provides-Extra: dev
 Requires-Dist: aiohttp; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: mock; python_version < "3.8" and extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pillow; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 
@@ -137,15 +135,15 @@
 
 ```bash
 prefect block register -m prefect_email
 ```
 
 Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://docs.prefect.io/ui/blocks/).
 
-Requires an installation of Python 3.8+.
+Requires an installation of Python 3.9+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
 These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Saving credentials to block
```

### Comparing `prefect_email-0.3.5/prefect_email.egg-info/SOURCES.txt` & `prefect_email-0.4.0rc1/prefect_email.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect_email-0.3.5/pyproject.toml` & `prefect_email-0.4.0rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,44 +2,42 @@
 requires = ["setuptools>=45", "wheel", "setuptools_scm>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prefect-email"
 description = "Prefect integrations for interacting with email."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = { text = "Apache License 2.0" }
 keywords = ["prefect"]
 authors = [{ name = "Prefect Technologies, Inc.", email = "help@prefect.io" }]
 classifiers = [
   "Natural Language :: English",
   "Intended Audience :: Developers",
   "Intended Audience :: System Administrators",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries",
 ]
-dependencies = ["prefect>=2.14.10, < 3.0.0"]
+dependencies = ["prefect>=3.0.0rc1"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
   "aiohttp",
   "coverage",
   "interrogate",
   "mkdocs-gen-files",
   "mkdocs-material",
   "mkdocs",
   "mkdocstrings[python]",
-  "mock; python_version < '3.8'",
   "mypy",
   "pillow",
   "pre-commit",
   "pytest-asyncio",
   "pytest",
   "pytest-xdist",
 ]
@@ -49,15 +47,15 @@
 
 [project.entry-points."prefect.collections"]
 prefect_email = "prefect_email"
 
 [tool.setuptools_scm]
 version_file = "prefect_email/_version.py"
 root = "../../.."
-tag_regex = "^prefect-email-(?P<version>\\d+\\.\\d+\\.\\d+)$"
+tag_regex = "^prefect-email-(?P<version>\\d+\\.\\d+\\.\\d+(?:[a-zA-Z0-9]+(?:\\.[a-zA-Z0-9]+)*)?)$"
 fallback_version = "0.0.0"
 git_describe_command = 'git describe --dirty --tags --long --match "prefect-email-*[0-9]*"'
 
 [tool.interrogate]
 ignore-init-module = true
 ignore_init_method = true
 exclude = ["prefect_email/_version.py", "tests"]
```

### Comparing `prefect_email-0.3.5/tests/conftest.py` & `prefect_email-0.4.0rc1/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from unittest.mock import MagicMock
 
 import pytest
 
 from prefect.testing.utilities import prefect_test_harness
 
 
-@pytest.fixture(autouse=True)
+@pytest.fixture(autouse=True, scope="session")
 def prefect_db():
     with prefect_test_harness():
         yield
 
 
 class EmailServerMethodsMock:
     def __enter__(self):
```

### Comparing `prefect_email-0.3.5/tests/test_block_standards.py` & `prefect_email-0.4.0rc1/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect_email-0.3.5/tests/test_credentials.py` & `prefect_email-0.4.0rc1/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_email-0.3.5/tests/test_message.py` & `prefect_email-0.4.0rc1/tests/test_message.py`

 * *Files identical despite different names*

