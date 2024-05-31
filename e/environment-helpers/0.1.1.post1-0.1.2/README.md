# Comparing `tmp/environment_helpers-0.1.1.post1.tar.gz` & `tmp/environment_helpers-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "environment_helpers-0.1.1.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "environment_helpers-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `environment_helpers-0.1.1.post1.tar` & `environment_helpers-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1078 2024-05-29 12:42:27.075752 environment_helpers-0.1.1.post1/LICENSE
--rw-r--r--   0        0        0      195 2024-05-29 12:42:27.075752 environment_helpers-0.1.1.post1/README.md
--rw-r--r--   0        0        0     4026 2024-05-29 12:42:40.652855 environment_helpers-0.1.1.post1/environment_helpers/__init__.py
--rw-r--r--   0        0        0      422 2024-05-29 12:42:27.075752 environment_helpers-0.1.1.post1/environment_helpers/_scripts/call.py
--rw-r--r--   0        0        0      348 2024-05-29 12:42:27.075752 environment_helpers-0.1.1.post1/environment_helpers/_scripts/launcher-kind.py
--rw-r--r--   0        0        0      188 2024-05-29 12:42:27.075752 environment_helpers-0.1.1.post1/environment_helpers/_scripts/scheme.py
--rw-r--r--   0        0        0     2033 2024-05-29 12:42:27.075752 environment_helpers-0.1.1.post1/environment_helpers/_scripts/system-scheme.py
--rw-r--r--   0        0        0      197 2024-05-29 12:42:27.075752 environment_helpers-0.1.1.post1/environment_helpers/_scripts/version.py
--rw-r--r--   0        0        0     2112 2024-05-29 12:42:27.075752 environment_helpers-0.1.1.post1/environment_helpers/build.py
--rw-r--r--   0        0        0     1013 2024-05-29 12:42:27.075752 environment_helpers-0.1.1.post1/environment_helpers/install.py
--rw-r--r--   0        0        0     4799 2024-05-29 12:42:27.075752 environment_helpers-0.1.1.post1/environment_helpers/introspect.py
--rw-r--r--   0        0        0     1894 2024-05-29 12:42:40.652855 environment_helpers-0.1.1.post1/pyproject.toml
--rw-r--r--   0        0        0     1443 1970-01-01 00:00:00.000000 environment_helpers-0.1.1.post1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-29 12:42:27.075752 environment_helpers-0.1.2/LICENSE
+-rw-r--r--   0        0        0      195 2024-05-29 12:42:27.075752 environment_helpers-0.1.2/README.md
+-rw-r--r--   0        0        0     4056 2024-05-31 18:15:50.263386 environment_helpers-0.1.2/environment_helpers/__init__.py
+-rw-r--r--   0        0        0      422 2024-05-29 12:42:27.075752 environment_helpers-0.1.2/environment_helpers/_scripts/call.py
+-rw-r--r--   0        0        0      348 2024-05-29 12:42:27.075752 environment_helpers-0.1.2/environment_helpers/_scripts/launcher-kind.py
+-rw-r--r--   0        0        0      188 2024-05-29 12:42:27.075752 environment_helpers-0.1.2/environment_helpers/_scripts/scheme.py
+-rw-r--r--   0        0        0     2033 2024-05-29 12:42:27.075752 environment_helpers-0.1.2/environment_helpers/_scripts/system-scheme.py
+-rw-r--r--   0        0        0      197 2024-05-29 12:42:27.075752 environment_helpers-0.1.2/environment_helpers/_scripts/version.py
+-rw-r--r--   0        0        0     2148 2024-05-31 18:15:50.263386 environment_helpers-0.1.2/environment_helpers/build.py
+-rw-r--r--   0        0        0     1049 2024-05-31 18:15:50.263386 environment_helpers-0.1.2/environment_helpers/install.py
+-rw-r--r--   0        0        0     4835 2024-05-31 18:15:50.263386 environment_helpers-0.1.2/environment_helpers/introspect.py
+-rw-r--r--   0        0        0     1888 2024-05-31 18:15:50.263386 environment_helpers-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1437 1970-01-01 00:00:00.000000 environment_helpers-0.1.2/PKG-INFO
```

### Comparing `environment_helpers-0.1.1.post1/LICENSE` & `environment_helpers-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `environment_helpers-0.1.1.post1/environment_helpers/__init__.py` & `environment_helpers-0.1.2/environment_helpers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Collection of helpers for managing Python environments."""
 
+from __future__ import annotations
+
 import os
 import pathlib
 import shutil
 import subprocess
 import tempfile
 import venv
 
@@ -11,15 +13,15 @@
 from typing import Any, Collection, Literal, Optional, Protocol
 
 import environment_helpers.build
 import environment_helpers.install
 import environment_helpers.introspect
 
 
-__version__ = '0.1.1.post1'
+__version__ = '0.1.2'
 
 
 class Environment(Protocol):
     """Object representing a Python environment."""
 
     @property
     def base(self) -> pathlib.Path: ...
```

### Comparing `environment_helpers-0.1.1.post1/environment_helpers/_scripts/system-scheme.py` & `environment_helpers-0.1.2/environment_helpers/_scripts/system-scheme.py`

 * *Files identical despite different names*

### Comparing `environment_helpers-0.1.1.post1/environment_helpers/build.py` & `environment_helpers-0.1.2/environment_helpers/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 import pathlib
 import tarfile
 import tempfile
 
 from typing import Optional
```

### Comparing `environment_helpers-0.1.1.post1/environment_helpers/install.py` & `environment_helpers-0.1.2/environment_helpers/install.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 import pathlib
 
 from typing import Optional
 
 import installer
 import installer.destinations
```

### Comparing `environment_helpers-0.1.1.post1/environment_helpers/introspect.py` & `environment_helpers-0.1.2/environment_helpers/introspect.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import functools
 import json
 import os
 import pickle
 import subprocess
 import sys
 import sysconfig
```

### Comparing `environment_helpers-0.1.1.post1/pyproject.toml` & `environment_helpers-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['flit-core >= 3.4']
 build-backend = 'flit_core.buildapi'
 
 [project]
 name = 'environment-helpers'
-version = '0.1.1.post1'
+version = '0.1.2'
 description = 'Collection of helpers for managing Python environments'
 readme = 'README.md'
 requires-python = '>= 3.8'
 license.file = 'LICENSE'
 authors = [
   { name = 'Filipe Laíns', email = 'lains@riseup.net' },
 ]
```

### Comparing `environment_helpers-0.1.1.post1/PKG-INFO` & `environment_helpers-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: environment-helpers
-Version: 0.1.1.post1
+Version: 0.1.2
 Summary: Collection of helpers for managing Python environments
 Author-email: Filipe Laíns <lains@riseup.net>
 Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

