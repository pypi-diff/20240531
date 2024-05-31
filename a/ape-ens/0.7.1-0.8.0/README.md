# Comparing `tmp/ape-ens-0.7.1.tar.gz` & `tmp/ape-ens-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-ens-0.7.1.tar", last modified: Tue Apr 30 14:29:02 2024, max compression
+gzip compressed data, was "ape-ens-0.8.0.tar", last modified: Fri May 31 21:51:15 2024, max compression
```

## Comparing `ape-ens-0.7.1.tar` & `ape-ens-0.8.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:29:02.758334 ape-ens-0.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:29:02.758334 ape-ens-0.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:29:02.758334 ape-ens-0.7.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-30 14:28:09.000000 ape-ens-0.7.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-30 14:28:09.000000 ape-ens-0.7.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-30 14:28:09.000000 ape-ens-0.7.1/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-30 14:28:09.000000 ape-ens-0.7.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-30 14:28:09.000000 ape-ens-0.7.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:29:02.758334 ape-ens-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-30 14:28:09.000000 ape-ens-0.7.1/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-30 14:28:09.000000 ape-ens-0.7.1/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-30 14:28:09.000000 ape-ens-0.7.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-30 14:28:09.000000 ape-ens-0.7.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-30 14:28:09.000000 ape-ens-0.7.1/.github/workflows/title.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-30 14:28:09.000000 ape-ens-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-30 14:28:09.000000 ape-ens-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-30 14:28:09.000000 ape-ens-0.7.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-30 14:28:09.000000 ape-ens-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-30 14:29:02.758334 ape-ens-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-30 14:28:09.000000 ape-ens-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:29:02.758334 ape-ens-0.7.1/ape_ens/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-30 14:28:09.000000 ape-ens-0.7.1/ape_ens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-30 14:28:09.000000 ape-ens-0.7.1/ape_ens/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:28:09.000000 ape-ens-0.7.1/ape_ens/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:29:02.758334 ape-ens-0.7.1/ape_ens/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-30 14:28:09.000000 ape-ens-0.7.1/ape_ens/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-30 14:28:09.000000 ape-ens-0.7.1/ape_ens/utils/namehash.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 14:29:02.000000 ape-ens-0.7.1/ape_ens/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:29:02.758334 ape-ens-0.7.1/ape_ens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-30 14:29:02.000000 ape-ens-0.7.1/ape_ens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-30 14:29:02.000000 ape-ens-0.7.1/ape_ens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 14:29:02.000000 ape-ens-0.7.1/ape_ens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 14:29:02.000000 ape-ens-0.7.1/ape_ens.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-30 14:29:02.000000 ape-ens-0.7.1/ape_ens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 14:29:02.000000 ape-ens-0.7.1/ape_ens.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-30 14:28:09.000000 ape-ens-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-30 14:29:02.758334 ape-ens-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-30 14:28:09.000000 ape-ens-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:29:02.758334 ape-ens-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:28:09.000000 ape-ens-0.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-30 14:28:09.000000 ape-ens-0.7.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-30 14:28:09.000000 ape-ens-0.7.1/tests/test_ens.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-30 14:28:09.000000 ape-ens-0.7.1/tests/test_namehash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:51:15.882670 ape-ens-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:51:15.878670 ape-ens-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:51:15.878670 ape-ens-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-31 21:50:26.000000 ape-ens-0.8.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-31 21:50:26.000000 ape-ens-0.8.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-31 21:50:26.000000 ape-ens-0.8.0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-31 21:50:26.000000 ape-ens-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-31 21:50:26.000000 ape-ens-0.8.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:51:15.878670 ape-ens-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-31 21:50:26.000000 ape-ens-0.8.0/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-31 21:50:26.000000 ape-ens-0.8.0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-31 21:50:26.000000 ape-ens-0.8.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-31 21:50:26.000000 ape-ens-0.8.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-31 21:50:26.000000 ape-ens-0.8.0/.github/workflows/title.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-31 21:50:26.000000 ape-ens-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-31 21:50:26.000000 ape-ens-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-31 21:50:26.000000 ape-ens-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-31 21:50:26.000000 ape-ens-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-31 21:51:15.882670 ape-ens-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-31 21:50:26.000000 ape-ens-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:51:15.878670 ape-ens-0.8.0/ape_ens/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-31 21:50:26.000000 ape-ens-0.8.0/ape_ens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-31 21:50:26.000000 ape-ens-0.8.0/ape_ens/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 21:50:26.000000 ape-ens-0.8.0/ape_ens/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:51:15.882670 ape-ens-0.8.0/ape_ens/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-31 21:50:26.000000 ape-ens-0.8.0/ape_ens/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-31 21:50:26.000000 ape-ens-0.8.0/ape_ens/utils/namehash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 21:51:15.000000 ape-ens-0.8.0/ape_ens/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:51:15.882670 ape-ens-0.8.0/ape_ens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-31 21:51:15.000000 ape-ens-0.8.0/ape_ens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-31 21:51:15.000000 ape-ens-0.8.0/ape_ens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 21:51:15.000000 ape-ens-0.8.0/ape_ens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 21:51:15.000000 ape-ens-0.8.0/ape_ens.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-31 21:51:15.000000 ape-ens-0.8.0/ape_ens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 21:51:15.000000 ape-ens-0.8.0/ape_ens.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-31 21:50:26.000000 ape-ens-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-31 21:51:15.882670 ape-ens-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-05-31 21:50:26.000000 ape-ens-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:51:15.882670 ape-ens-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 21:50:26.000000 ape-ens-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-31 21:50:26.000000 ape-ens-0.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-31 21:50:26.000000 ape-ens-0.8.0/tests/test_ens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-31 21:50:26.000000 ape-ens-0.8.0/tests/test_namehash.py
```

### Comparing `ape-ens-0.7.1/.github/ISSUE_TEMPLATE/bug.md` & `ape-ens-0.8.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.1/.github/ISSUE_TEMPLATE/feature.md` & `ape-ens-0.8.0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.1/.github/ISSUE_TEMPLATE/work-item.md` & `ape-ens-0.8.0/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.1/.github/release-drafter.yml` & `ape-ens-0.8.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.1/.github/workflows/commit.yaml` & `ape-ens-0.8.0/.github/workflows/commit.yaml`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.1/.github/workflows/publish.yaml` & `ape-ens-0.8.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.1/.github/workflows/test.yaml` & `ape-ens-0.8.0/.github/workflows/test.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -58,16 +58,18 @@
           run: mypy .
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
-                os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, "3.10", "3.11"]
+                # TODO: Replace with macos-latest when works again.
+                #   https://github.com/actions/setup-python/issues/808
+                os: [ubuntu-latest, macos-12]   # eventually add `windows-latest`
+                python-version: [3.9, "3.10", "3.11", "3.12"]
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
```

### Comparing `ape-ens-0.7.1/.github/workflows/title.yaml` & `ape-ens-0.8.0/.github/workflows/title.yaml`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.1/.gitignore` & `ape-ens-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.1/.pre-commit-config.yaml` & `ape-ens-0.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.1/CONTRIBUTING.md` & `ape-ens-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.1/LICENSE` & `ape-ens-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.1/PKG-INFO` & `ape-ens-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: ape-ens
-Version: 0.7.1
+Version: 0.8.0
 Summary: ape-ens: Ape plugin for ENS argument conversion and contracts
 Home-page: https://github.com/ApeWorX/ape-ens
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8,<4
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
 
 # Quick Start
 
 Ape plugin for ENS argument conversion and contracts
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-ens-0.7.1/README.md` & `ape-ens-0.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 Ape plugin for ENS argument conversion and contracts
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-ens-0.7.1/ape_ens/converter.py` & `ape-ens-0.8.0/ape_ens/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Any, Dict, Optional
+from typing import Any, Optional
 
 from ape.api import ConverterAPI
 from ape.exceptions import NetworkError, ProviderError
 from ape.logging import logger
 from ape.types import AddressType
 from ape.utils import cached_property
 from ape_ethereum.provider import Web3Provider
 from web3.exceptions import CannotHandleRequest
 from web3.main import ENS
 
 
 class ENSConversions(ConverterAPI):
     """Converts ENS names like `my-name.eth` to `0xAbCd...1234`"""
 
-    address_cache: Dict[str, AddressType] = {}
+    address_cache: dict[str, AddressType] = {}
 
     @cached_property
     def mainnet_provider(self) -> Optional[Web3Provider]:
         provider = self.network_manager.active_provider
         if (
             provider
             and isinstance(provider, Web3Provider)
```

### Comparing `ape-ens-0.7.1/ape_ens/utils/namehash.py` & `ape-ens-0.8.0/ape_ens/utils/namehash.py`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.1/ape_ens.egg-info/PKG-INFO` & `ape-ens-0.8.0/ape_ens.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: ape-ens
-Version: 0.7.1
+Version: 0.8.0
 Summary: ape-ens: Ape plugin for ENS argument conversion and contracts
 Home-page: https://github.com/ApeWorX/ape-ens
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8,<4
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
 
 # Quick Start
 
 Ape plugin for ENS argument conversion and contracts
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-ens-0.7.1/ape_ens.egg-info/SOURCES.txt` & `ape-ens-0.8.0/ape_ens.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.1/ape_ens.egg-info/requires.txt` & `ape-ens-0.8.0/ape_ens.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-eth-ape<0.8,>=0.7.0
+eth-ape<0.9,>=0.8.1
 web3
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 pytest-mock
```

### Comparing `ape-ens-0.7.1/pyproject.toml` & `ape-ens-0.8.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py38', 'py39', 'py310', 'py311']
+target-version = ['py39', 'py310', 'py311', 'py312']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
     -p no:ape_test
     --cov-branch
     --cov-report term
```

### Comparing `ape-ens-0.7.1/setup.py` & `ape-ens-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,18 +64,18 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-ens",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.7.0,<0.8",
+        "eth-ape>=0.8.1,<0.9",
         "web3",  # Use same version as eth-ape
     ],
-    python_requires=">=3.8,<4",
+    python_requires=">=3.9,<4",
     extras_require=extras_require,
     py_modules=["ape_ens"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ape_ens": ["py.typed"]},
@@ -83,13 +83,13 @@
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `ape-ens-0.7.1/tests/conftest.py` & `ape-ens-0.8.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from functools import partial
 from pathlib import Path
-from typing import Dict, cast
+from typing import cast
 
 import pytest
 from ape.api import UpstreamProvider
 from ape.types import AddressType
 from ape_ethereum.provider import Web3Provider
 
 from ape_ens.converter import ENSConversions
@@ -36,17 +36,16 @@
         yield
     finally:
         os.chdir(curr_dir)
 
 
 class MockMainnetProvider(Web3Provider, UpstreamProvider):
     name: str = "mock"
-    provider_settings: Dict = {}
-    data_folder: Path = Path(".")
-    request_header: Dict = {}
+    provider_settings: dict = {}
+    request_header: dict = {}
 
     @property
     def connection_str(self) -> str:
         return "<MOCK>"
 
     @property
     def is_connected(self) -> bool:
```

### Comparing `ape-ens-0.7.1/tests/test_ens.py` & `ape-ens-0.8.0/tests/test_ens.py`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.1/tests/test_namehash.py` & `ape-ens-0.8.0/tests/test_namehash.py`

 * *Files identical despite different names*

