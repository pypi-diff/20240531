# Comparing `tmp/prefect_bitbucket-0.2.5.tar.gz` & `tmp/prefect_bitbucket-0.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_bitbucket-0.2.5.tar", last modified: Thu May 16 20:58:30 2024, max compression
+gzip compressed data, was "prefect_bitbucket-0.3.0rc1.tar", last modified: Fri May 31 20:49:34 2024, max compression
```

## Comparing `prefect_bitbucket-0.2.5.tar` & `prefect_bitbucket-0.3.0rc1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:30.045588 prefect_bitbucket-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-16 20:58:18.000000 prefect_bitbucket-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 20:58:18.000000 prefect_bitbucket-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-05-16 20:58:30.045588 prefect_bitbucket-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-16 20:58:18.000000 prefect_bitbucket-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:30.041588 prefect_bitbucket-0.2.5/prefect_bitbucket/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-16 20:58:18.000000 prefect_bitbucket-0.2.5/prefect_bitbucket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 20:58:29.000000 prefect_bitbucket-0.2.5/prefect_bitbucket/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-16 20:58:18.000000 prefect_bitbucket-0.2.5/prefect_bitbucket/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-05-16 20:58:18.000000 prefect_bitbucket-0.2.5/prefect_bitbucket/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:30.045588 prefect_bitbucket-0.2.5/prefect_bitbucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-05-16 20:58:29.000000 prefect_bitbucket-0.2.5/prefect_bitbucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-16 20:58:30.000000 prefect_bitbucket-0.2.5/prefect_bitbucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:58:29.000000 prefect_bitbucket-0.2.5/prefect_bitbucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-16 20:58:29.000000 prefect_bitbucket-0.2.5/prefect_bitbucket.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-16 20:58:29.000000 prefect_bitbucket-0.2.5/prefect_bitbucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 20:58:29.000000 prefect_bitbucket-0.2.5/prefect_bitbucket.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-16 20:58:18.000000 prefect_bitbucket-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:58:30.045588 prefect_bitbucket-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:30.045588 prefect_bitbucket-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-16 20:58:18.000000 prefect_bitbucket-0.2.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-16 20:58:18.000000 prefect_bitbucket-0.2.5/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-05-16 20:58:18.000000 prefect_bitbucket-0.2.5/tests/test_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-16 20:58:18.000000 prefect_bitbucket-0.2.5/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:34.025392 prefect_bitbucket-0.3.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-31 20:49:22.000000 prefect_bitbucket-0.3.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-31 20:49:22.000000 prefect_bitbucket-0.3.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-05-31 20:49:34.025392 prefect_bitbucket-0.3.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-05-31 20:49:22.000000 prefect_bitbucket-0.3.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:34.021392 prefect_bitbucket-0.3.0rc1/prefect_bitbucket/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-31 20:49:22.000000 prefect_bitbucket-0.3.0rc1/prefect_bitbucket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-31 20:49:33.000000 prefect_bitbucket-0.3.0rc1/prefect_bitbucket/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-31 20:49:22.000000 prefect_bitbucket-0.3.0rc1/prefect_bitbucket/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-05-31 20:49:22.000000 prefect_bitbucket-0.3.0rc1/prefect_bitbucket/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:34.025392 prefect_bitbucket-0.3.0rc1/prefect_bitbucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-05-31 20:49:33.000000 prefect_bitbucket-0.3.0rc1/prefect_bitbucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-31 20:49:34.000000 prefect_bitbucket-0.3.0rc1/prefect_bitbucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:49:33.000000 prefect_bitbucket-0.3.0rc1/prefect_bitbucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-31 20:49:33.000000 prefect_bitbucket-0.3.0rc1/prefect_bitbucket.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-31 20:49:33.000000 prefect_bitbucket-0.3.0rc1/prefect_bitbucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-31 20:49:33.000000 prefect_bitbucket-0.3.0rc1/prefect_bitbucket.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-31 20:49:22.000000 prefect_bitbucket-0.3.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:49:34.025392 prefect_bitbucket-0.3.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:34.025392 prefect_bitbucket-0.3.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-31 20:49:22.000000 prefect_bitbucket-0.3.0rc1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-31 20:49:22.000000 prefect_bitbucket-0.3.0rc1/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-05-31 20:49:22.000000 prefect_bitbucket-0.3.0rc1/tests/test_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-31 20:49:22.000000 prefect_bitbucket-0.3.0rc1/tests/test_version.py
```

### Comparing `prefect_bitbucket-0.2.5/LICENSE` & `prefect_bitbucket-0.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_bitbucket-0.2.5/PKG-INFO` & `prefect_bitbucket-0.3.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: prefect-bitbucket
-Version: 0.2.5
+Version: 0.3.0rc1
 Summary: Prefect integrations for working with Bitbucket repositories.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-bitbucket
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
+Requires-Dist: pydantic>=2.4
 Requires-Dist: atlassian-python-api!=3.41.5,!=3.41.6,!=3.41.7,!=3.41.8,>=3.32.1
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
 
@@ -52,15 +51,15 @@
 
 Prefect integrations for working with Bitbucket repositories.
 
 ## Getting Started
 
 ### Python setup
 
-Requires an installation of Python 3.8+.
+Requires an installation of Python 3.9+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
 These tasks are designed to work with Prefect 2.0. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Installation
```

### Comparing `prefect_bitbucket-0.2.5/README.md` & `prefect_bitbucket-0.3.0rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 Prefect integrations for working with Bitbucket repositories.
 
 ## Getting Started
 
 ### Python setup
 
-Requires an installation of Python 3.8+.
+Requires an installation of Python 3.9+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
 These tasks are designed to work with Prefect 2.0. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Installation
 
@@ -141,8 +141,8 @@
 
 # Saves the BitBucketRepository block to your Prefect workspace (in the Blocks tab)
 private_bitbucket_block.save(name="my-private-bitbucket-block")
 ```
 
 !!! info "Differences between Bitbucket Server and Bitbucket Cloud"
 
-    For Bitbucket Cloud, only set the `token` to authenticate. For Bitbucket Server, set both the `token` and the `username`.
+    For Bitbucket Cloud, only set the `token` to authenticate. For Bitbucket Server, set both the `token` and the `username`.
```

### Comparing `prefect_bitbucket-0.2.5/prefect_bitbucket/credentials.py` & `prefect_bitbucket-0.3.0rc1/prefect_bitbucket/credentials.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 """Module to enable authenticate interactions with BitBucket."""
+
 import re
 from enum import Enum
 from typing import Optional, Union
 
-from pydantic import VERSION as PYDANTIC_VERSION
+from pydantic import Field, SecretStr, field_validator
 
 from prefect.blocks.abstract import CredentialsBlock
 
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field, SecretStr, validator
-else:
-    from pydantic import Field, SecretStr, validator
-
 try:
     from atlassian.bitbucket import Bitbucket, Cloud
 except ImportError:
     pass
 
 
 class ClientType(Enum):
@@ -44,36 +40,37 @@
         ```
 
 
     """
 
     _block_type_name = "BitBucket Credentials"
     _logo_url = "https://cdn.sanity.io/images/3ugk85nk/production/5d729f7355fb6828c4b605268ded9cfafab3ae4f-250x250.png"  # noqa
+
     token: Optional[SecretStr] = Field(
-        name="Personal Access Token",
+        title="Personal Access Token",
         default=None,
         description=(
             "A BitBucket Personal Access Token - required for private repositories."
         ),
-        example="x-token-auth:my-token",
+        examples=["x-token-auth:my-token"],
     )
     username: Optional[str] = Field(
         default=None,
         description="Identification name unique across entire BitBucket site.",
     )
     password: Optional[SecretStr] = Field(
         default=None, description="The password to authenticate to BitBucket."
     )
     url: str = Field(
         default="https://api.bitbucket.org/",
         description="The base URL of your BitBucket instance.",
         title="URL",
     )
 
-    @validator("username")
+    @field_validator("username")
     def _validate_username(cls, value: str) -> str:
         """When username provided, will validate it."""
         pattern = "^[A-Za-z0-9_-]*$"
 
         if not re.match(pattern, value):
             raise ValueError(
                 "Username must be alpha, num, dash and/or underscore only."
```

### Comparing `prefect_bitbucket-0.2.5/prefect_bitbucket/repository.py` & `prefect_bitbucket-0.3.0rc1/prefect_bitbucket/repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,32 +32,27 @@
 )
 
 private_bitbucket_block.save(name="my-private-bitbucket-block")
 
 """
 
 import io
-from distutils.dir_util import copy_tree
 from pathlib import Path
+from shutil import copytree
 from tempfile import TemporaryDirectory
 from typing import Optional, Tuple, Union
 from urllib.parse import urlparse, urlunparse
 
-from pydantic import VERSION as PYDANTIC_VERSION
+from pydantic import Field, model_validator
+from typing_extensions import Self
 
 from prefect.exceptions import InvalidRepositoryURLError
 from prefect.filesystems import ReadableDeploymentStorage
 from prefect.utilities.asyncutils import sync_compatible
 from prefect.utilities.processutils import run_process
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field, validator
-else:
-    from pydantic import Field, validator
-
 from prefect_bitbucket.credentials import BitBucketCredentials
 
 
 class BitBucketRepository(ReadableDeploymentStorage):
     """Interact with files stored in BitBucket repositories.
 
     An accessible installation of git is required for this block to function
@@ -80,36 +75,36 @@
         default=None,
         description=(
             "An optional BitBucketCredentials block for authenticating with "
             "private BitBucket repos."
         ),
     )
 
-    @validator("bitbucket_credentials")
-    def _ensure_credentials_go_with_https(cls, v: str, values: dict) -> str:
+    @model_validator(mode="after")
+    def _ensure_credentials_go_with_https(self) -> Self:
         """Ensure that credentials are not provided with 'SSH' formatted BitBucket URLs.
 
         Validators are by default only called on provided arguments.
 
         Note: validates `credentials` specifically so that it only fires when private
         repositories are used.
         """
-        if v is not None:
-            if urlparse(values["repository"]).scheme != "https":
+        if self.bitbucket_credentials is not None:
+            if urlparse(self.repository).scheme != "https":
                 raise InvalidRepositoryURLError(
                     (
                         "Credentials can only be used with BitBucket repositories "
                         "using the 'HTTPS' format. You must either remove the "
                         "credential if you wish to use the 'SSH' format and are not "
                         "using a private repository, or you must change the repository "
                         "URL to the 'HTTPS' format."
                     )
                 )
 
-        return v
+        return self
 
     def _create_repo_url(self) -> str:
         """Format the URL provided to the `git clone` command.
 
         For private repos in the cloud:
         https://x-token-auth:<access-token>@bitbucket.org/<user>/<repo>.git
         For private repos with a local bitbucket server:
@@ -193,8 +188,8 @@
                 err_stream.seek(0)
                 raise OSError(f"Failed to pull from remote:\n {err_stream.read()}")
 
             content_source, content_destination = self._get_paths(
                 dst_dir=local_path, src_dir=tmp_dir, sub_directory=from_path
             )
 
-            copy_tree(src=content_source, dst=content_destination)
+            copytree(src=content_source, dst=content_destination, dirs_exist_ok=True)
```

### Comparing `prefect_bitbucket-0.2.5/prefect_bitbucket.egg-info/PKG-INFO` & `prefect_bitbucket-0.3.0rc1/prefect_bitbucket.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: prefect-bitbucket
-Version: 0.2.5
+Version: 0.3.0rc1
 Summary: Prefect integrations for working with Bitbucket repositories.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-bitbucket
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
+Requires-Dist: pydantic>=2.4
 Requires-Dist: atlassian-python-api!=3.41.5,!=3.41.6,!=3.41.7,!=3.41.8,>=3.32.1
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
 
@@ -52,15 +51,15 @@
 
 Prefect integrations for working with Bitbucket repositories.
 
 ## Getting Started
 
 ### Python setup
 
-Requires an installation of Python 3.8+.
+Requires an installation of Python 3.9+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
 These tasks are designed to work with Prefect 2.0. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Installation
```

### Comparing `prefect_bitbucket-0.2.5/pyproject.toml` & `prefect_bitbucket-0.3.0rc1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,47 +2,46 @@
 requires = ["setuptools>=45", "wheel", "setuptools_scm>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prefect-bitbucket"
 description = "Prefect integrations for working with Bitbucket repositories."
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
 dependencies = [
-  "prefect>=2.14.10, < 3.0.0",
+  "prefect>=3.0.0rc1",
+  "pydantic>=2.4",
   "atlassian-python-api>=3.32.1,!=3.41.5,!=3.41.6,!=3.41.7,!=3.41.8",
 ]
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
@@ -52,15 +51,15 @@
 
 [project.entry-points."prefect.collections"]
 prefect_bitbucket = "prefect_bitbucket"
 
 [tool.setuptools_scm]
 version_file = "prefect_bitbucket/_version.py"
 root = "../../.."
-tag_regex = "^prefect-bitbucket-(?P<version>\\d+\\.\\d+\\.\\d+)$"
+tag_regex = "^prefect-bitbucket-(?P<version>\\d+\\.\\d+\\.\\d+(?:[a-zA-Z0-9]+(?:\\.[a-zA-Z0-9]+)*)?)$"
 fallback_version = "0.0.0"
 git_describe_command = 'git describe --dirty --tags --long --match "prefect-bitbucket-*[0-9]*"'
 
 [tool.interrogate]
 ignore-init-module = true
 ignore_init_method = true
 exclude = ["prefect_bitbucket/_version.py", "tests"]
```

### Comparing `prefect_bitbucket-0.2.5/tests/test_credentials.py` & `prefect_bitbucket-0.3.0rc1/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_bitbucket-0.2.5/tests/test_repository.py` & `prefect_bitbucket-0.3.0rc1/tests/test_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import pytest
 from pydantic import VERSION as PYDANTIC_VERSION
 
 from prefect.exceptions import InvalidRepositoryURLError
 from prefect.testing.utilities import AsyncMock
 
 if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import SecretStr
+    pass
 else:
-    from pydantic import SecretStr
+    pass
 
 import prefect_bitbucket
 from prefect_bitbucket.credentials import BitBucketCredentials
 from prefect_bitbucket.repository import BitBucketRepository
 
 
 class TestBitBucketRepository:
@@ -133,15 +133,15 @@
 
         mock = AsyncMock(return_value=p())
         monkeypatch.setattr(prefect_bitbucket.repository, "run_process", mock)
         credential = "XYZ"
         repo = "https://bitbucket.org/PrefectHQ/prefect.git"
         b = BitBucketRepository(
             repository=repo,
-            bitbucket_credentials=BitBucketCredentials(token=SecretStr(credential)),
+            bitbucket_credentials=BitBucketCredentials(token=credential),
         )
         await b.get_directory()
         assert mock.await_count == 1
         expected_cmd = [
             "git",
             "clone",
             f"https://x-token-auth:{credential}@bitbucket.org/PrefectHQ/prefect.git",
@@ -162,15 +162,15 @@
         monkeypatch.setattr(prefect_bitbucket.repository, "run_process", mock)
         credential = "XYZ"
         username = "ABC"
         repo = "https://bitbucket.org/PrefectHQ/prefect.git"
         b = BitBucketRepository(
             repository=repo,
             bitbucket_credentials=BitBucketCredentials(
-                token=SecretStr(credential), username=username
+                token=credential, username=username
             ),
         )
         await b.get_directory()
         assert mock.await_count == 1
         expected_cmd = [
             "git",
             "clone",
@@ -197,15 +197,15 @@
             "credential if you wish to use the 'SSH' format and are not "
             "using a private repository, or you must change the repository "
             "URL to the 'HTTPS' format."
         )
         with pytest.raises(InvalidRepositoryURLError, match=error_msg):
             BitBucketRepository(
                 repository="git@bitbucket.org:PrefectHQ/prefect.git",
-                bitbucket_credentials=BitBucketCredentials(token=SecretStr(credential)),
+                bitbucket_credentials=BitBucketCredentials(token=credential),
             )
 
     async def test_dir_contents_copied_correctly_with_get_directory(self, monkeypatch):  # noqa
         """Check that `get_directory` is able to correctly copy contents from src->dst"""  # noqa
 
         class p:
             returncode = 0
```

