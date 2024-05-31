# Comparing `tmp/prefect_docker-0.5.2.tar.gz` & `tmp/prefect_docker-0.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_docker-0.5.2.tar", last modified: Thu May 16 20:58:36 2024, max compression
+gzip compressed data, was "prefect_docker-0.6.0rc1.tar", last modified: Fri May 31 20:49:37 2024, max compression
```

## Comparing `prefect_docker-0.5.2.tar` & `prefect_docker-0.6.0rc1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:36.134754 prefect_docker-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-16 20:58:36.130754 prefect_docker-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:36.126754 prefect_docker-0.5.2/prefect_docker/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/prefect_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 20:58:35.000000 prefect_docker-0.5.2/prefect_docker/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/prefect_docker/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/prefect_docker/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:36.130754 prefect_docker-0.5.2/prefect_docker/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/prefect_docker/deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/prefect_docker/deployments/steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/prefect_docker/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/prefect_docker/images.py
--rw-r--r--   0 runner    (1001) docker     (127)    30166 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/prefect_docker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:36.130754 prefect_docker-0.5.2/prefect_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-16 20:58:35.000000 prefect_docker-0.5.2/prefect_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-16 20:58:36.000000 prefect_docker-0.5.2/prefect_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:58:35.000000 prefect_docker-0.5.2/prefect_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 20:58:35.000000 prefect_docker-0.5.2/prefect_docker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-16 20:58:35.000000 prefect_docker-0.5.2/prefect_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-16 20:58:35.000000 prefect_docker-0.5.2/prefect_docker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:58:36.134754 prefect_docker-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:36.130754 prefect_docker-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:36.130754 prefect_docker-0.5.2/tests/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)    11532 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/tests/deployments/test_steps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:36.130754 prefect_docker-0.5.2/tests/test-project/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/tests/test-project/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/tests/test-project/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/tests/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/tests/test_host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    46168 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/tests/test_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:37.449532 prefect_docker-0.6.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-31 20:49:25.000000 prefect_docker-0.6.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-31 20:49:25.000000 prefect_docker-0.6.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-31 20:49:37.449532 prefect_docker-0.6.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-31 20:49:25.000000 prefect_docker-0.6.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:37.445532 prefect_docker-0.6.0rc1/prefect_docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-31 20:49:25.000000 prefect_docker-0.6.0rc1/prefect_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-31 20:49:37.000000 prefect_docker-0.6.0rc1/prefect_docker/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-05-31 20:49:25.000000 prefect_docker-0.6.0rc1/prefect_docker/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-31 20:49:25.000000 prefect_docker-0.6.0rc1/prefect_docker/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:37.445532 prefect_docker-0.6.0rc1/prefect_docker/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:25.000000 prefect_docker-0.6.0rc1/prefect_docker/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-05-31 20:49:25.000000 prefect_docker-0.6.0rc1/prefect_docker/deployments/steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-31 20:49:25.000000 prefect_docker-0.6.0rc1/prefect_docker/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-31 20:49:25.000000 prefect_docker-0.6.0rc1/prefect_docker/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-05-31 20:49:25.000000 prefect_docker-0.6.0rc1/prefect_docker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:37.449532 prefect_docker-0.6.0rc1/prefect_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-31 20:49:37.000000 prefect_docker-0.6.0rc1/prefect_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-31 20:49:37.000000 prefect_docker-0.6.0rc1/prefect_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:49:37.000000 prefect_docker-0.6.0rc1/prefect_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-31 20:49:37.000000 prefect_docker-0.6.0rc1/prefect_docker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-31 20:49:37.000000 prefect_docker-0.6.0rc1/prefect_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-31 20:49:37.000000 prefect_docker-0.6.0rc1/prefect_docker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-31 20:49:25.000000 prefect_docker-0.6.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:49:37.449532 prefect_docker-0.6.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:37.449532 prefect_docker-0.6.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-05-31 20:49:25.000000 prefect_docker-0.6.0rc1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:37.449532 prefect_docker-0.6.0rc1/tests/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-05-31 20:49:25.000000 prefect_docker-0.6.0rc1/tests/deployments/test_steps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:37.449532 prefect_docker-0.6.0rc1/tests/test-project/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-31 20:49:25.000000 prefect_docker-0.6.0rc1/tests/test-project/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-31 20:49:25.000000 prefect_docker-0.6.0rc1/tests/test-project/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-31 20:49:25.000000 prefect_docker-0.6.0rc1/tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-31 20:49:25.000000 prefect_docker-0.6.0rc1/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-31 20:49:25.000000 prefect_docker-0.6.0rc1/tests/test_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-31 20:49:25.000000 prefect_docker-0.6.0rc1/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-31 20:49:25.000000 prefect_docker-0.6.0rc1/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46471 2024-05-31 20:49:25.000000 prefect_docker-0.6.0rc1/tests/test_worker.py
```

### Comparing `prefect_docker-0.5.2/LICENSE` & `prefect_docker-0.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.2/PKG-INFO` & `prefect_docker-0.6.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: prefect-docker
-Version: 0.5.2
+Version: 0.6.0rc1
 Summary: Prefect integrations for interacting with Docker.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-docker
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
 Requires-Dist: docker>=6.1.1
+Requires-Dist: exceptiongroup
+Requires-Dist: requests<2.30.0
 Provides-Extra: dev
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
 
@@ -54,15 +54,15 @@
 
 Do not use `DockerRegistry` with this collection. Instead, use `DockerHost` and `DockerRegistryCredentials`.
 
 ## Getting Started
 
 ### Python setup
 
-Requires an installation of Python 3.8+.
+Requires an installation of Python 3.9+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda, or virtualenv.
 
 These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Installation
```

### Comparing `prefect_docker-0.5.2/README.md` & `prefect_docker-0.6.0rc1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 Do not use `DockerRegistry` with this collection. Instead, use `DockerHost` and `DockerRegistryCredentials`.
 
 ## Getting Started
 
 ### Python setup
 
-Requires an installation of Python 3.8+.
+Requires an installation of Python 3.9+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda, or virtualenv.
 
 These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Installation
```

### Comparing `prefect_docker-0.5.2/prefect_docker/containers.py` & `prefect_docker-0.6.0rc1/prefect_docker/containers.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.2/prefect_docker/credentials.py` & `prefect_docker-0.6.0rc1/prefect_docker/credentials.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 """Module containing docker credentials."""
+
 import docker
-from pydantic import VERSION as PYDANTIC_VERSION
+from pydantic import Field, SecretStr
 
 from prefect import get_run_logger
 from prefect.blocks.core import Block
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
 
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field, SecretStr
-else:
-    from pydantic import Field, SecretStr
-
 
 class DockerRegistryCredentials(Block):
     """
     Block used to manage credentials for interacting with a Docker Registry.
 
     Examples:
         Log into Docker Registry.
@@ -43,15 +39,15 @@
         default=..., description="The password to log into the registry with."
     )
     registry_url: str = Field(
         default=...,
         description=(
             'The URL to the registry. Generally, "http" or "https" can be omitted.'
         ),
-        example="index.docker.io",
+        examples=["index.docker.io"],
     )
     reauth: bool = Field(
         default=True,
         description="Whether or not to reauthenticate on each interaction.",
     )
 
     async def login(self, client: docker.DockerClient):
```

### Comparing `prefect_docker-0.5.2/prefect_docker/deployments/steps.py` & `prefect_docker-0.6.0rc1/prefect_docker/deployments/steps.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.2/prefect_docker/host.py` & `prefect_docker-0.6.0rc1/prefect_docker/host.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 """Module containing Docker host settings."""
+
 from typing import Any, Dict, Optional
 
 import docker
-from pydantic import VERSION as PYDANTIC_VERSION
+from pydantic import Field
 
 from prefect import get_run_logger
 from prefect.blocks.core import Block
 
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field
-else:
-    from pydantic import Field
-
 
 class _ContextManageableDockerClient(docker.DockerClient):
     """
     Allow context managing Docker Client, but also allow it to be instantiated without.
     """
 
     def __enter__(self):
@@ -64,15 +60,15 @@
     _logo_url = "https://cdn.sanity.io/images/3ugk85nk/production/14a315b79990200db7341e42553e23650b34bb96-250x250.png"  # noqa
     _description = "Store settings for interacting with a Docker host."
 
     base_url: Optional[str] = Field(
         default=None,
         description="URL to the Docker host.",
         title="Base URL",
-        example="unix:///var/run/docker.sock",
+        examples=["unix:///var/run/docker.sock"],
     )
     version: str = Field(default="auto", description="The version of the API to use")
     timeout: Optional[int] = Field(
         default=None, description="Default timeout for API calls, in seconds."
     )
     max_pool_size: Optional[int] = Field(
         default=None,
```

### Comparing `prefect_docker-0.5.2/prefect_docker/images.py` & `prefect_docker-0.6.0rc1/prefect_docker/images.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.2/prefect_docker/worker.py` & `prefect_docker-0.6.0rc1/prefect_docker/worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 
 import anyio.abc
 import docker
 import docker.errors
 import packaging.version
 from docker import DockerClient
 from docker.models.containers import Container
-from pydantic import VERSION as PYDANTIC_VERSION
+from pydantic import AfterValidator, Field
+from slugify import slugify
+from typing_extensions import Annotated, Literal
 
 import prefect
 from prefect.client.orchestration import ServerType, get_client
 from prefect.client.schemas import FlowRun
 from prefect.events import Event, RelatedResource, emit_event
 from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
 from prefect.server.schemas.core import Flow
@@ -43,35 +45,30 @@
     format_outlier_version_name,
     get_prefect_image_name,
     parse_image_tag,
 )
 from prefect.workers.base import BaseJobConfiguration, BaseWorker, BaseWorkerResult
 from prefect_docker.credentials import DockerRegistryCredentials
 
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field, validator
-else:
-    from pydantic import Field, validator
-
-from slugify import slugify
-from typing_extensions import Literal
-
 CONTAINER_LABELS = {
     "io.prefect.version": prefect.__version__,
 }
 
 
 class ImagePullPolicy(enum.Enum):
     """Enum representing the image pull policy options for a Docker container."""
 
     IF_NOT_PRESENT = "IfNotPresent"
     ALWAYS = "Always"
     NEVER = "Never"
 
 
+VolumeStr = Annotated[str, AfterValidator(lambda v: ":" in v)]
+
+
 class DockerWorkerJobConfiguration(BaseJobConfiguration):
     """
     Configuration class used by the Docker worker.
 
     An instance of this class is passed to the Docker worker's `run` method
     for each flow run. It contains all the information necessary to execute the
     flow run as a Docker container.
@@ -103,15 +100,15 @@
         privileged: Give extended privileges to created containers.
     """
 
     image: str = Field(
         default_factory=get_prefect_image_name,
         description="The image reference of a container image to use for created jobs. "
         "If not set, the latest Prefect image will be used.",
-        example="docker.io/prefecthq/prefect:2-latest",
+        example="docker.io/prefecthq/prefect:3-latest",
     )
     registry_credentials: Optional[DockerRegistryCredentials] = Field(
         default=None,
         description="Credentials for logging into a Docker registry to pull"
         " images from.",
     )
     image_pull_policy: Optional[Literal["IfNotPresent", "Always", "Never"]] = Field(
@@ -129,18 +126,18 @@
             " 'networks' is set, this cannot be set."
         ),
     )
     auto_remove: bool = Field(
         default=False,
         description="If set, containers will be deleted on completion.",
     )
-    volumes: List[str] = Field(
+    volumes: List[VolumeStr] = Field(
         default_factory=list,
         description="A list of volume to mount into created containers.",
-        example=["/my/local/path:/path/in/container"],
+        examples=["/my/local/path:/path/in/container"],
     )
     stream_output: bool = Field(
         default=True,
         description=(
             "If set, the output from created containers will be streamed to local "
             "standard output."
         ),
@@ -167,26 +164,14 @@
     )
 
     privileged: bool = Field(
         default=False,
         description="Give extended privileges to created container.",
     )
 
-    @validator("volumes")
-    def _validate_volume_format(cls, volumes):
-        """Validates that provided volume strings are in the correct format."""
-        for volume in volumes:
-            if ":" not in volume:
-                raise ValueError(
-                    "Invalid volume specification. "
-                    f"Expected format 'path:container_path', but got {volume!r}"
-                )
-
-        return volumes
-
     def _convert_labels_to_docker_format(self, labels: Dict[str, str]):
         """Converts labels to the format expected by Docker."""
         labels = labels or {}
         new_labels = {}
         for name, value in labels.items():
             if "/" in name:
                 namespace, key = name.split("/", maxsplit=1)
@@ -763,15 +748,15 @@
         last_event: Optional[Event] = None,
     ) -> Event:
         """Emit a Prefect event for a Docker container event."""
         related = self._event_related_resources(configuration=configuration)
 
         worker_resource = self._event_resource()
         worker_resource["prefect.resource.role"] = "worker"
-        worker_related_resource = RelatedResource(__root__=worker_resource)
+        worker_related_resource = RelatedResource(worker_resource)
 
         return emit_event(
             event=f"prefect.docker.container.{container.status.lower()}",
             resource=self._container_as_resource(container),
             related=related + [worker_related_resource],
             follows=last_event,
         )
```

### Comparing `prefect_docker-0.5.2/prefect_docker.egg-info/PKG-INFO` & `prefect_docker-0.6.0rc1/prefect_docker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: prefect-docker
-Version: 0.5.2
+Version: 0.6.0rc1
 Summary: Prefect integrations for interacting with Docker.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-docker
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
 Requires-Dist: docker>=6.1.1
+Requires-Dist: exceptiongroup
+Requires-Dist: requests<2.30.0
 Provides-Extra: dev
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
 
@@ -54,15 +54,15 @@
 
 Do not use `DockerRegistry` with this collection. Instead, use `DockerHost` and `DockerRegistryCredentials`.
 
 ## Getting Started
 
 ### Python setup
 
-Requires an installation of Python 3.8+.
+Requires an installation of Python 3.9+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda, or virtualenv.
 
 These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Installation
```

### Comparing `prefect_docker-0.5.2/prefect_docker.egg-info/SOURCES.txt` & `prefect_docker-0.6.0rc1/prefect_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.2/pyproject.toml` & `prefect_docker-0.6.0rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,43 +2,46 @@
 requires = ["setuptools>=45", "wheel", "setuptools_scm>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prefect-docker"
 description = "Prefect integrations for interacting with Docker."
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
-dependencies = ["prefect>=2.13.5, < 3.0.0", "docker>=6.1.1"]
+dependencies = [
+  "prefect>=3.0.0rc1",
+  "docker>=6.1.1",
+  "exceptiongroup",
+  "requests<2.30.0",
+]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
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
@@ -48,15 +51,15 @@
 
 [project.entry-points."prefect.collections"]
 prefect_docker = "prefect_docker"
 
 [tool.setuptools_scm]
 version_file = "prefect_docker/_version.py"
 root = "../../.."
-tag_regex = "^prefect-docker-(?P<version>\\d+\\.\\d+\\.\\d+)$"
+tag_regex = "^prefect-docker-(?P<version>\\d+\\.\\d+\\.\\d+(?:[a-zA-Z0-9]+(?:\\.[a-zA-Z0-9]+)*)?)$"
 fallback_version = "0.0.0"
 git_describe_command = 'git describe --dirty --tags --long --match "prefect-docker-*[0-9]*"'
 
 [tool.interrogate]
 ignore-init-module = true
 ignore_init_method = true
 exclude = ["prefect_docker/_version.py", "tests"]
```

### Comparing `prefect_docker-0.5.2/tests/conftest.py` & `prefect_docker-0.6.0rc1/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
 import logging
 import sys
 from contextlib import contextmanager
 from typing import Generator
 from unittest.mock import MagicMock, patch
 
+from anyio import to_thread
 from prefect_docker.worker import CONTAINER_LABELS
 
 from prefect.server.database.alembic_commands import alembic_upgrade
 from prefect.testing.fixtures import *  # noqa
 from prefect.testing.utilities import prefect_test_harness
 from prefect.utilities.dockerutils import IMAGE_LABELS, silence_docker_warnings
 
@@ -23,15 +24,15 @@
 
 @pytest.fixture(scope="session", autouse=True)
 def prefect_db():
     """
     Sets up test harness for temporary DB during test runs.
     """
     with prefect_test_harness():
-        alembic_upgrade()
+        asyncio.run(to_thread.run_sync(alembic_upgrade))
         yield
 
 
 @pytest.fixture(autouse=True)
 def reset_object_registry():
     """
     Ensures each test has a clean object registry.
```

### Comparing `prefect_docker-0.5.2/tests/deployments/test_steps.py` & `prefect_docker-0.6.0rc1/tests/deployments/test_steps.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import pytest
 from prefect_docker.deployments.steps import build_docker_image, push_docker_image
 
 import prefect
 import prefect.utilities.dockerutils
 
 FAKE_CONTAINER_ID = "fake-id"
-FAKE_BASE_URL = "http+docker://my-url"
+FAKE_BASE_URL = "my-url"
 FAKE_DEFAULT_TAG = "2022-08-31t18-01-32-00-00"
 FAKE_IMAGE_NAME = "registry/repo"
 FAKE_TAG = "mytag"
 FAKE_ADDITIONAL_TAGS = ["addtag1", "addtag2"]
 FAKE_EVENT = [{"status": "status", "progress": "progress"}, {"status": "status"}]
 FAKE_CREDENTIALS = {
     "username": "user",
```

### Comparing `prefect_docker-0.5.2/tests/test-project/flow.py` & `prefect_docker-0.6.0rc1/tests/test-project/flow.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.2/tests/test_containers.py` & `prefect_docker-0.6.0rc1/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.2/tests/test_host.py` & `prefect_docker-0.6.0rc1/tests/test_host.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.2/tests/test_images.py` & `prefect_docker-0.6.0rc1/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.2/tests/test_worker.py` & `prefect_docker-0.6.0rc1/tests/test_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 import copy
-import re
 import uuid
 from unittest.mock import MagicMock, call, patch
 
 import anyio.abc
 import docker
 import docker.errors
 import docker.models.containers
 import pytest
 from docker import DockerClient
 from docker.models.containers import Container
-from packaging import version
+from exceptiongroup import ExceptionGroup
 from prefect_docker.credentials import DockerRegistryCredentials
 from prefect_docker.worker import (
     CONTAINER_LABELS,
     DockerWorker,
     DockerWorkerJobConfiguration,
 )
 
-import prefect
 from prefect.client.schemas import FlowRun
 from prefect.events import RelatedResource
 from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
 from prefect.settings import (
     PREFECT_EXPERIMENTAL_ENABLE_WORKERS,
     PREFECT_EXPERIMENTAL_WARN_WORKERS,
     get_current_settings,
     temporary_settings,
 )
 from prefect.testing.utilities import assert_does_not_warn
 from prefect.utilities.dockerutils import get_prefect_image_name
 
 FAKE_CONTAINER_ID = "fake-id"
-FAKE_BASE_URL = "http+docker://my-url"
+FAKE_BASE_URL = "my-url"
 
 
 @pytest.fixture(autouse=True)
 def enable_workers():
     with temporary_settings(
         {PREFECT_EXPERIMENTAL_ENABLE_WORKERS: 1, PREFECT_EXPERIMENTAL_WARN_WORKERS: 0}
     ):
@@ -215,19 +213,22 @@
 ):
     import docker.errors
 
     mock_docker_client.containers.create.side_effect = docker.errors.APIError(
         "test error"
     )
 
-    with pytest.raises(docker.errors.APIError, match="test error"):
+    with pytest.raises(ExceptionGroup) as exc:
         async with DockerWorker(work_pool_name="test") as worker:
             await worker.run(
                 flow_run=flow_run, configuration=default_docker_worker_job_configuration
             )
+    assert len(exc.value.exceptions) == 1
+    assert isinstance(exc.value.exceptions[0], docker.errors.APIError)
+    assert "test error" in str(exc.value.exceptions[0])
 
 
 async def test_uses_image_setting(
     mock_docker_client, flow_run, default_docker_worker_job_configuration
 ):
     default_docker_worker_job_configuration.image = "foo"
     async with DockerWorker(work_pool_name="test") as worker:
@@ -384,22 +385,17 @@
     async with DockerWorker(work_pool_name="test") as worker:
         await worker.run(
             flow_run=flow_run, configuration=default_docker_worker_job_configuration
         )
     mock_docker_client.containers.create.assert_called_once()
     call_env = mock_docker_client.containers.create.call_args[1].get("environment")
 
-    flow_run_id = (
-        str(flow_run.id)
-        if version.parse(prefect.__version__) >= version.parse("2.13.5")
-        else flow_run.id.hex
-    )
     assert call_env == {
         **get_current_settings().to_environment_variables(exclude_unset=True),
-        "PREFECT__FLOW_RUN_ID": flow_run_id,
+        "PREFECT__FLOW_RUN_ID": str(flow_run.id),
         "foo": "FOO",
         "bar": "BAR",
     }
 
 
 async def test_allows_unsetting_environment_variables(
     mock_docker_client, flow_run, default_docker_worker_job_configuration
@@ -1109,42 +1105,44 @@
     expected_string = "".join(
         [
             f"Unable to stop container {FAKE_CONTAINER_ID!r}: the current Docker API ",
             f"URL {mock_docker_client.api.base_url!r} does not match the expected ",
             f"API base URL {BAD_BASE_URL}.",
         ]
     )
-    with pytest.raises(InfrastructureNotAvailable, match=re.escape(expected_string)):
+    with pytest.raises(ExceptionGroup) as exc:
         async with DockerWorker(work_pool_name="test") as worker:
             await worker.kill_infrastructure(
                 infrastructure_pid=f"{BAD_BASE_URL}:{FAKE_CONTAINER_ID}",
                 configuration=default_docker_worker_job_configuration,
                 grace_seconds=0,
             )
+    assert len(exc.value.exceptions) == 1
+    assert isinstance(exc.value.exceptions[0], InfrastructureNotAvailable)
+    assert str(exc.value.exceptions[0]) == expected_string
 
 
 async def test_kill_infrastructure_raises_infra_not_found_with_bad_container_id(
     mock_docker_client, default_docker_worker_job_configuration
 ):
     mock_docker_client.containers.get.side_effect = [docker.errors.NotFound("msg")]
 
     BAD_CONTAINER_ID = "bad-container-id"
-    with pytest.raises(
-        InfrastructureNotFound,
-        match=(
-            f"Unable to stop container {BAD_CONTAINER_ID!r}: The container was not"
-            " found."
-        ),
-    ):
+    with pytest.raises(ExceptionGroup) as exc:
         async with DockerWorker(work_pool_name="test") as worker:
             await worker.kill_infrastructure(
                 infrastructure_pid=f"{FAKE_BASE_URL}:{BAD_CONTAINER_ID}",
                 configuration=default_docker_worker_job_configuration,
                 grace_seconds=0,
             )
+    assert len(exc.value.exceptions) == 1
+    assert isinstance(exc.value.exceptions[0], InfrastructureNotFound)
+    assert str(exc.value.exceptions[0]) == (
+        f"Unable to stop container {BAD_CONTAINER_ID!r}: The container was not found."
+    )
 
 
 async def test_emits_events(
     mock_docker_client, flow_run, default_docker_worker_job_configuration
 ):
     event_count = 0
 
@@ -1157,15 +1155,15 @@
         async with DockerWorker(work_pool_name="test") as worker:
             await worker.run(
                 flow_run=flow_run, configuration=default_docker_worker_job_configuration
             )
 
     worker_resource = worker._event_resource()
     worker_resource["prefect.resource.role"] = "worker"
-    worker_related_resource = RelatedResource(__root__=worker_resource)
+    worker_related_resource = RelatedResource(worker_resource)
 
     mock_emit.assert_has_calls(
         [
             call(
                 event="prefect.docker.container.created",
                 resource={
                     "prefect.resource.id": "prefect.docker.container.fake-id",
@@ -1203,20 +1201,22 @@
 
     mock_docker_client.containers.create.side_effect = docker.errors.APIError(
         "test error"
     )
 
     worker_resource = None
     with patch("prefect_docker.worker.emit_event") as mock_emit:
-        with pytest.raises(docker.errors.APIError, match="test error"):
+        with pytest.raises(ExceptionGroup) as exc:
             async with DockerWorker(work_pool_name="test") as worker:
                 worker_resource = worker._event_resource()
                 await worker.run(
                     flow_run=flow_run,
                     configuration=default_docker_worker_job_configuration,
                 )
+        assert len(exc.value.exceptions) == 1
+        assert isinstance(exc.value.exceptions[0], docker.errors.APIError)
 
         mock_emit.assert_called_once_with(
             event="prefect.docker.container.creation-failed",
             resource=worker_resource,
             related=[],
         )
```

