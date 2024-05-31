# Comparing `tmp/prefect_gitlab-0.2.5.tar.gz` & `tmp/prefect_gitlab-0.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_gitlab-0.2.5.tar", last modified: Thu May 16 20:58:39 2024, max compression
+gzip compressed data, was "prefect_gitlab-0.3.0rc1.tar", last modified: Fri May 31 20:50:02 2024, max compression
```

## Comparing `prefect_gitlab-0.2.5.tar` & `prefect_gitlab-0.3.0rc1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:39.688641 prefect_gitlab-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-16 20:58:28.000000 prefect_gitlab-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 20:58:28.000000 prefect_gitlab-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-16 20:58:39.688641 prefect_gitlab-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-16 20:58:28.000000 prefect_gitlab-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:39.684641 prefect_gitlab-0.2.5/prefect_gitlab/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-16 20:58:28.000000 prefect_gitlab-0.2.5/prefect_gitlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 20:58:39.000000 prefect_gitlab-0.2.5/prefect_gitlab/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-16 20:58:28.000000 prefect_gitlab-0.2.5/prefect_gitlab/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-05-16 20:58:28.000000 prefect_gitlab-0.2.5/prefect_gitlab/repositories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:39.684641 prefect_gitlab-0.2.5/prefect_gitlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-16 20:58:39.000000 prefect_gitlab-0.2.5/prefect_gitlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-16 20:58:39.000000 prefect_gitlab-0.2.5/prefect_gitlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:58:39.000000 prefect_gitlab-0.2.5/prefect_gitlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 20:58:39.000000 prefect_gitlab-0.2.5/prefect_gitlab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-16 20:58:39.000000 prefect_gitlab-0.2.5/prefect_gitlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-16 20:58:39.000000 prefect_gitlab-0.2.5/prefect_gitlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-16 20:58:28.000000 prefect_gitlab-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:58:39.688641 prefect_gitlab-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:39.684641 prefect_gitlab-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-16 20:58:28.000000 prefect_gitlab-0.2.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-16 20:58:28.000000 prefect_gitlab-0.2.5/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-05-16 20:58:28.000000 prefect_gitlab-0.2.5/tests/test_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-16 20:58:28.000000 prefect_gitlab-0.2.5/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:02.282854 prefect_gitlab-0.3.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-31 20:49:48.000000 prefect_gitlab-0.3.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-31 20:49:48.000000 prefect_gitlab-0.3.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-05-31 20:50:02.282854 prefect_gitlab-0.3.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-31 20:49:48.000000 prefect_gitlab-0.3.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:02.278854 prefect_gitlab-0.3.0rc1/prefect_gitlab/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-31 20:49:48.000000 prefect_gitlab-0.3.0rc1/prefect_gitlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-31 20:50:01.000000 prefect_gitlab-0.3.0rc1/prefect_gitlab/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-31 20:49:48.000000 prefect_gitlab-0.3.0rc1/prefect_gitlab/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6479 2024-05-31 20:49:48.000000 prefect_gitlab-0.3.0rc1/prefect_gitlab/repositories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:02.278854 prefect_gitlab-0.3.0rc1/prefect_gitlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-05-31 20:50:01.000000 prefect_gitlab-0.3.0rc1/prefect_gitlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-31 20:50:02.000000 prefect_gitlab-0.3.0rc1/prefect_gitlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:50:01.000000 prefect_gitlab-0.3.0rc1/prefect_gitlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-31 20:50:01.000000 prefect_gitlab-0.3.0rc1/prefect_gitlab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-31 20:50:01.000000 prefect_gitlab-0.3.0rc1/prefect_gitlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-31 20:50:01.000000 prefect_gitlab-0.3.0rc1/prefect_gitlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-31 20:49:48.000000 prefect_gitlab-0.3.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:50:02.282854 prefect_gitlab-0.3.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:02.278854 prefect_gitlab-0.3.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-31 20:49:48.000000 prefect_gitlab-0.3.0rc1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-31 20:49:48.000000 prefect_gitlab-0.3.0rc1/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-05-31 20:49:48.000000 prefect_gitlab-0.3.0rc1/tests/test_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-31 20:49:48.000000 prefect_gitlab-0.3.0rc1/tests/test_version.py
```

### Comparing `prefect_gitlab-0.2.5/LICENSE` & `prefect_gitlab-0.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_gitlab-0.2.5/PKG-INFO` & `prefect_gitlab-0.3.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 Metadata-Version: 2.1
 Name: prefect-gitlab
-Version: 0.2.5
+Version: 0.3.0rc1
 Summary: A Prefect collection for working with GitLab repositories.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-gitlab
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
-Requires-Dist: prefect<3.0.0,>=2.13.5
+Requires-Dist: prefect>=3.0.0rc1
 Requires-Dist: python-gitlab>=3.12.0
 Requires-Dist: tenacity>=8.2.3
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
 
@@ -52,15 +50,15 @@
 
 `prefect-gitlab` is a Prefect collection for working with GitLab repositories.
 
 ## Getting Started
 
 ### Python setup
 
-Requires an installation of Python 3.8 or higher.
+Requires an installation of Python 3.9 or higher.
 
 We recommend using a Python virtual environment manager such as pipenv, conda, or virtualenv.
 
 This integration is designed to work with Prefect 2.3.0 or higher. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Installation
```

#### html2text {}

```diff
@@ -1,36 +1,34 @@
-Metadata-Version: 2.1 Name: prefect-gitlab Version: 0.2.5 Summary: A Prefect
+Metadata-Version: 2.1 Name: prefect-gitlab Version: 0.3.0rc1 Summary: A Prefect
 collection for working with GitLab repositories. Author-email: "Prefect
 Technologies, Inc."
 prefect.io> License: Apache License 2.0 Project-URL: Homepage, https://
 github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-gitlab
 Keywords: prefect Classifier: Natural Language :: English Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
-Topic :: Software Development :: Libraries Requires-Python: >=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-prefect<3.0.0,>=2.13.5 Requires-Dist: python-gitlab>=3.12.0 Requires-Dist:
-tenacity>=8.2.3 Provides-Extra: dev Requires-Dist: aiohttp; extra == "dev"
-Requires-Dist: coverage; extra == "dev" Requires-Dist: interrogate; extra ==
-"dev" Requires-Dist: mkdocs-gen-files; extra == "dev" Requires-Dist: mkdocs-
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Topic :: Software Development :: Libraries Requires-
+Python: >=3.9 Description-Content-Type: text/markdown License-File: LICENSE
+Requires-Dist: prefect>=3.0.0rc1 Requires-Dist: python-gitlab>=3.12.0 Requires-
+Dist: tenacity>=8.2.3 Provides-Extra: dev Requires-Dist: aiohttp; extra ==
+"dev" Requires-Dist: coverage; extra == "dev" Requires-Dist: interrogate; extra
+== "dev" Requires-Dist: mkdocs-gen-files; extra == "dev" Requires-Dist: mkdocs-
 material; extra == "dev" Requires-Dist: mkdocs; extra == "dev" Requires-Dist:
-mkdocstrings[python]; extra == "dev" Requires-Dist: mock; python_version <
-"3.8" and extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-Dist:
-pillow; extra == "dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist:
-pytest-asyncio; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-
-Dist: pytest-xdist; extra == "dev" # prefect-gitlab
+mkdocstrings[python]; extra == "dev" Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pillow; extra == "dev" Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev" Requires-Dist: pytest; extra ==
+"dev" Requires-Dist: pytest-xdist; extra == "dev" # prefect-gitlab
                 _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_p_r_e_f_e_c_t_-
                     _g_i_t_l_a_b_?_c_o_l_o_r_=_2_6_2_7_2_B_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]
 ## Welcome! `prefect-gitlab` is a Prefect collection for working with GitLab
 repositories. ## Getting Started ### Python setup Requires an installation of
-Python 3.8 or higher. We recommend using a Python virtual environment manager
+Python 3.9 or higher. We recommend using a Python virtual environment manager
 such as pipenv, conda, or virtualenv. This integration is designed to work with
 Prefect 2.3.0 or higher. For more information about how to use Prefect, please
 refer to the [Prefect documentation](https://docs.prefect.io/). ###
 Installation Install `prefect-gitlab` with `pip`: ```bash pip install prefect-
 gitlab ``` Then, register the [block types](https://docs.prefect.io/concepts/
 blocks/)) in this integration to view the storage block type on Prefect Cloud:
 ```bash prefect block register -m prefect_gitlab ``` Note, to use the `load`
```

### Comparing `prefect_gitlab-0.2.5/README.md` & `prefect_gitlab-0.3.0rc1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 `prefect-gitlab` is a Prefect collection for working with GitLab repositories.
 
 ## Getting Started
 
 ### Python setup
 
-Requires an installation of Python 3.8 or higher.
+Requires an installation of Python 3.9 or higher.
 
 We recommend using a Python virtual environment manager such as pipenv, conda, or virtualenv.
 
 This integration is designed to work with Prefect 2.3.0 or higher. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Installation
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # prefect-gitlab
                 _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_p_r_e_f_e_c_t_-
                     _g_i_t_l_a_b_?_c_o_l_o_r_=_2_6_2_7_2_B_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]
 ## Welcome! `prefect-gitlab` is a Prefect collection for working with GitLab
 repositories. ## Getting Started ### Python setup Requires an installation of
-Python 3.8 or higher. We recommend using a Python virtual environment manager
+Python 3.9 or higher. We recommend using a Python virtual environment manager
 such as pipenv, conda, or virtualenv. This integration is designed to work with
 Prefect 2.3.0 or higher. For more information about how to use Prefect, please
 refer to the [Prefect documentation](https://docs.prefect.io/). ###
 Installation Install `prefect-gitlab` with `pip`: ```bash pip install prefect-
 gitlab ``` Then, register the [block types](https://docs.prefect.io/concepts/
 blocks/)) in this integration to view the storage block type on Prefect Cloud:
 ```bash prefect block register -m prefect_gitlab ``` Note, to use the `load`
```

### Comparing `prefect_gitlab-0.2.5/prefect_gitlab/credentials.py` & `prefect_gitlab-0.3.0rc1/prefect_gitlab/credentials.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 """Module used to enable authenticated interactions with GitLab"""
 
+from typing import Optional
+
 from gitlab import Gitlab
-from pydantic import VERSION as PYDANTIC_VERSION
+from pydantic import Field, SecretStr
 
 from prefect.blocks.core import Block
 
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field, HttpUrl, SecretStr
-else:
-    from pydantic import Field, HttpUrl, SecretStr
-
 
 class GitLabCredentials(Block):
     """
     Store a GitLab personal access token to interact with private GitLab
     repositories.
 
     Attributes:
@@ -25,25 +22,22 @@
         ```python
         from prefect_gitlab import GitLabCredentials
         gitlab_credentials_block = GitLabCredentials.load("BLOCK_NAME")
         ```
     """
 
     _block_type_name = "GitLab Credentials"
-    _logo_url = HttpUrl(
-        url="https://images.ctfassets.net/gm98wzqotmnx/55edIimT4g9gbjhkh5a3Sp/dfdb9391d8f45c2e93e72e3a4d350771/gitlab-logo-500.png?h=250",  # noqa
-        scheme="https",
-    )
+    _logo_url = "https://images.ctfassets.net/gm98wzqotmnx/55edIimT4g9gbjhkh5a3Sp/dfdb9391d8f45c2e93e72e3a4d350771/gitlab-logo-500.png?h=250"
 
-    token: SecretStr = Field(
-        name="Personal Access Token",
+    token: Optional[SecretStr] = Field(
+        title="Personal Access Token",
         default=None,
         description="A GitLab Personal Access Token with read_repository scope.",
     )
-    url: str = Field(
+    url: Optional[str] = Field(
         default=None, title="URL", description="URL to self-hosted GitLab instances."
     )
 
     def get_client(self) -> Gitlab:
         """
         Gets an authenticated GitLab client.
```

### Comparing `prefect_gitlab-0.2.5/prefect_gitlab/repositories.py` & `prefect_gitlab-0.3.0rc1/prefect_gitlab/repositories.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,34 +36,28 @@
         repository="https://gitlab.com/testing/my-repository.git",
         access_token="YOUR_GITLAB_PERSONAL_ACCESS_TOKEN"
     )
 
     private_gitlab_block.save()
 ```
 """
+
 import io
+import shutil
 import urllib.parse
-from distutils.dir_util import copy_tree
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Optional, Tuple, Union
 
-from pydantic import VERSION as PYDANTIC_VERSION
+from pydantic import Field
 from tenacity import retry, stop_after_attempt, wait_fixed, wait_random
 
-from prefect.exceptions import InvalidRepositoryURLError
 from prefect.filesystems import ReadableDeploymentStorage
 from prefect.utilities.asyncutils import sync_compatible
 from prefect.utilities.processutils import run_process
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field, HttpUrl, validator
-else:
-    from pydantic import Field, HttpUrl, validator
-
 from prefect_gitlab.credentials import GitLabCredentials
 
 # Create get_directory retry settings
 
 MAX_CLONE_ATTEMPTS = 3
 CLONE_RETRY_MIN_DELAY_SECONDS = 1
 CLONE_RETRY_MIN_DELAY_JITTER_SECONDS = 0
@@ -75,18 +69,15 @@
     Interact with files stored in GitLab repositories.
 
     An accessible installation of git is required for this block to function
     properly.
     """
 
     _block_type_name = "GitLab Repository"
-    _logo_url = HttpUrl(
-        url="https://images.ctfassets.net/gm98wzqotmnx/55edIimT4g9gbjhkh5a3Sp/dfdb9391d8f45c2e93e72e3a4d350771/gitlab-logo-500.png?h=250",  # noqa
-        scheme="https",
-    )
+    _logo_url = "https://images.ctfassets.net/gm98wzqotmnx/55edIimT4g9gbjhkh5a3Sp/dfdb9391d8f45c2e93e72e3a4d350771/gitlab-logo-500.png?h=250"
     _description = "Interact with files stored in GitLab repositories."
 
     repository: str = Field(
         default=...,
         description=(
             "The URL of a GitLab repository to read from, in either HTTP/HTTPS or SSH format."  # noqa
         ),
@@ -103,37 +94,14 @@
     )
     credentials: Optional[GitLabCredentials] = Field(
         default=None,
         description="An optional GitLab Credentials block for authenticating with "
         "private GitLab repos.",
     )
 
-    @validator("credentials")
-    def _ensure_credentials_go_with_http(cls, v: str, values: dict) -> str:
-        """Ensure that credentials are not provided with 'SSH' formatted GitLub URLs.
-        Note: validates `access_token` specifically so that it only fires when
-        private repositories are used.
-        """
-        if v is not None:
-            if urllib.parse.urlparse(values["repository"]).scheme not in [
-                "https",
-                "http",
-            ]:
-                raise InvalidRepositoryURLError(
-                    (
-                        "Credentials can only be used with GitLab repositories "
-                        "using the 'HTTPS'/'HTTP' format. You must either remove the "
-                        "credential if you wish to use the 'SSH' format and are not "
-                        "using a private repository, or you must change the repository "
-                        "URL to the 'HTTPS'/'HTTP' format."
-                    )
-                )
-
-        return v
-
     def _create_repo_url(self) -> str:
         """Format the URL provided to the `git clone` command.
         For private repos: https://<oauth-key>@gitlab.com/<username>/<repo>.git
         All other repos should be the same as `self.repository`.
         """
         url_components = urllib.parse.urlparse(self.repository)
         if url_components.scheme in ["https", "http"] and self.credentials is not None:
@@ -209,8 +177,10 @@
                 err_stream.seek(0)
                 raise OSError(f"Failed to pull from remote:\n {err_stream.read()}")
 
             content_source, content_destination = self._get_paths(
                 dst_dir=local_path, src_dir=tmp_dir, sub_directory=from_path
             )
 
-            copy_tree(src=content_source, dst=content_destination)
+            shutil.copytree(
+                src=content_source, dst=content_destination, dirs_exist_ok=True
+            )
```

### Comparing `prefect_gitlab-0.2.5/prefect_gitlab.egg-info/PKG-INFO` & `prefect_gitlab-0.3.0rc1/prefect_gitlab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 Metadata-Version: 2.1
 Name: prefect-gitlab
-Version: 0.2.5
+Version: 0.3.0rc1
 Summary: A Prefect collection for working with GitLab repositories.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-gitlab
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
-Requires-Dist: prefect<3.0.0,>=2.13.5
+Requires-Dist: prefect>=3.0.0rc1
 Requires-Dist: python-gitlab>=3.12.0
 Requires-Dist: tenacity>=8.2.3
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
 
@@ -52,15 +50,15 @@
 
 `prefect-gitlab` is a Prefect collection for working with GitLab repositories.
 
 ## Getting Started
 
 ### Python setup
 
-Requires an installation of Python 3.8 or higher.
+Requires an installation of Python 3.9 or higher.
 
 We recommend using a Python virtual environment manager such as pipenv, conda, or virtualenv.
 
 This integration is designed to work with Prefect 2.3.0 or higher. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Installation
```

#### html2text {}

```diff
@@ -1,36 +1,34 @@
-Metadata-Version: 2.1 Name: prefect-gitlab Version: 0.2.5 Summary: A Prefect
+Metadata-Version: 2.1 Name: prefect-gitlab Version: 0.3.0rc1 Summary: A Prefect
 collection for working with GitLab repositories. Author-email: "Prefect
 Technologies, Inc."
 prefect.io> License: Apache License 2.0 Project-URL: Homepage, https://
 github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-gitlab
 Keywords: prefect Classifier: Natural Language :: English Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
-Topic :: Software Development :: Libraries Requires-Python: >=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-prefect<3.0.0,>=2.13.5 Requires-Dist: python-gitlab>=3.12.0 Requires-Dist:
-tenacity>=8.2.3 Provides-Extra: dev Requires-Dist: aiohttp; extra == "dev"
-Requires-Dist: coverage; extra == "dev" Requires-Dist: interrogate; extra ==
-"dev" Requires-Dist: mkdocs-gen-files; extra == "dev" Requires-Dist: mkdocs-
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Topic :: Software Development :: Libraries Requires-
+Python: >=3.9 Description-Content-Type: text/markdown License-File: LICENSE
+Requires-Dist: prefect>=3.0.0rc1 Requires-Dist: python-gitlab>=3.12.0 Requires-
+Dist: tenacity>=8.2.3 Provides-Extra: dev Requires-Dist: aiohttp; extra ==
+"dev" Requires-Dist: coverage; extra == "dev" Requires-Dist: interrogate; extra
+== "dev" Requires-Dist: mkdocs-gen-files; extra == "dev" Requires-Dist: mkdocs-
 material; extra == "dev" Requires-Dist: mkdocs; extra == "dev" Requires-Dist:
-mkdocstrings[python]; extra == "dev" Requires-Dist: mock; python_version <
-"3.8" and extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-Dist:
-pillow; extra == "dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist:
-pytest-asyncio; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-
-Dist: pytest-xdist; extra == "dev" # prefect-gitlab
+mkdocstrings[python]; extra == "dev" Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pillow; extra == "dev" Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev" Requires-Dist: pytest; extra ==
+"dev" Requires-Dist: pytest-xdist; extra == "dev" # prefect-gitlab
                 _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_p_r_e_f_e_c_t_-
                     _g_i_t_l_a_b_?_c_o_l_o_r_=_2_6_2_7_2_B_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]
 ## Welcome! `prefect-gitlab` is a Prefect collection for working with GitLab
 repositories. ## Getting Started ### Python setup Requires an installation of
-Python 3.8 or higher. We recommend using a Python virtual environment manager
+Python 3.9 or higher. We recommend using a Python virtual environment manager
 such as pipenv, conda, or virtualenv. This integration is designed to work with
 Prefect 2.3.0 or higher. For more information about how to use Prefect, please
 refer to the [Prefect documentation](https://docs.prefect.io/). ###
 Installation Install `prefect-gitlab` with `pip`: ```bash pip install prefect-
 gitlab ``` Then, register the [block types](https://docs.prefect.io/concepts/
 blocks/)) in this integration to view the storage block type on Prefect Cloud:
 ```bash prefect block register -m prefect_gitlab ``` Note, to use the `load`
```

### Comparing `prefect_gitlab-0.2.5/pyproject.toml` & `prefect_gitlab-0.3.0rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,48 +2,46 @@
 requires = ["setuptools>=45", "wheel", "setuptools_scm>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prefect-gitlab"
 description = "A Prefect collection for working with GitLab repositories."
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
-  "prefect>=2.13.5, < 3.0.0",
+  "prefect>=3.0.0rc1",
   "python-gitlab>=3.12.0",
   "tenacity>=8.2.3",
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
@@ -53,15 +51,15 @@
 
 [project.entry-points."prefect.collections"]
 prefect_gitlab = "prefect_gitlab"
 
 [tool.setuptools_scm]
 version_file = "prefect_gitlab/_version.py"
 root = "../../.."
-tag_regex = "^prefect-gitlab-(?P<version>\\d+\\.\\d+\\.\\d+)$"
+tag_regex = "^prefect-gitlab-(?P<version>\\d+\\.\\d+\\.\\d+(?:[a-zA-Z0-9]+(?:\\.[a-zA-Z0-9]+)*)?)$"
 fallback_version = "0.0.0"
 git_describe_command = 'git describe --dirty --tags --long --match "prefect-gitlab-*[0-9]*"'
 
 [tool.interrogate]
 ignore-init-module = true
 ignore_init_method = true
 exclude = ["prefect_gitlab/_version.py", "tests"]
```

### Comparing `prefect_gitlab-0.2.5/tests/test_credentials.py` & `prefect_gitlab-0.3.0rc1/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_gitlab-0.2.5/tests/test_repositories.py` & `prefect_gitlab-0.3.0rc1/tests/test_repositories.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 import os
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Set, Tuple
 
-import pytest
-from pydantic import VERSION as PYDANTIC_VERSION
-
-from prefect.exceptions import InvalidRepositoryURLError
-from prefect.testing.utilities import AsyncMock
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import SecretStr
-else:
-    from pydantic import SecretStr
-
 import prefect_gitlab
+import pytest
 from prefect_gitlab.credentials import GitLabCredentials
 from prefect_gitlab.repositories import GitLabRepository  # noqa: E402
+from pydantic import SecretStr
+
+from prefect.testing.utilities import AsyncMock
 
 
 class TestGitLab:
     def setup_test_directory(
         self, tmp_src: str, sub_dir: str = "puppy"
     ) -> Tuple[Set[str], Set[str]]:
         """Add files and directories to a temporary directory. Returns a tuple with the
@@ -166,38 +159,14 @@
         expected_cmd = [
             "git",
             "clone",
             repo,
         ]
         assert mock.await_args[0][0][: len(expected_cmd)] == expected_cmd
 
-    async def test_ssh_fails_with_credential(self, monkeypatch):
-        """Ensure that credentials cannot be passed in if the URL is not in the HTTPS/HTTP
-        format.
-        """
-
-        class p:
-            returncode = 0
-
-        mock = AsyncMock(return_value=p())
-        monkeypatch.setattr(prefect_gitlab.repositories, "run_process", mock)
-        credential = "XYZ"
-        error_msg = (
-            "Credentials can only be used with GitLab repositories "
-            "using the 'HTTPS'/'HTTP' format. You must either remove the "
-            "credential if you wish to use the 'SSH' format and are not "
-            "using a private repository, or you must change the repository "
-            "URL to the 'HTTPS'/'HTTP' format."
-        )
-        with pytest.raises(InvalidRepositoryURLError, match=error_msg):
-            GitLabRepository(
-                repository="git@gitlab.com:PrefectHQ/prefect.git",
-                credentials=GitLabCredentials(token=SecretStr(credential)),
-            )
-
     async def test_dir_contents_copied_correctly_with_get_directory(self, monkeypatch):  # noqa
         """Check that `get_directory` is able to correctly copy contents from src->dst"""  # noqa
 
         class p:
             returncode = 0
 
         mock = AsyncMock(return_value=p())
```

