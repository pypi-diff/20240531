# Comparing `tmp/prefect_azure-0.3.9.tar.gz` & `tmp/prefect_azure-0.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_azure-0.3.9.tar", last modified: Fri Apr 26 15:03:56 2024, max compression
+gzip compressed data, was "prefect_azure-0.4.0rc1.tar", last modified: Fri May 31 20:49:36 2024, max compression
```

## Comparing `prefect_azure-0.3.9.tar` & `prefect_azure-0.4.0rc1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.337059 prefect_azure-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-26 15:03:56.333059 prefect_azure-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.329059 prefect_azure-0.3.9/prefect_azure/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/prefect_azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 15:03:55.000000 prefect_azure-0.3.9/prefect_azure/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    25910 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/prefect_azure/blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    36429 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/prefect_azure/container_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/prefect_azure/cosmos_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    21828 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/prefect_azure/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.329059 prefect_azure-0.3.9/prefect_azure/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/prefect_azure/deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/prefect_azure/deployments/steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/prefect_azure/ml_datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/prefect_azure/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.329059 prefect_azure-0.3.9/prefect_azure/workers/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/prefect_azure/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39029 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/prefect_azure/workers/container_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.333059 prefect_azure-0.3.9/prefect_azure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-26 15:03:56.000000 prefect_azure-0.3.9/prefect_azure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-26 15:03:56.000000 prefect_azure-0.3.9/prefect_azure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:03:56.000000 prefect_azure-0.3.9/prefect_azure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 15:03:56.000000 prefect_azure-0.3.9/prefect_azure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-26 15:03:56.000000 prefect_azure-0.3.9/prefect_azure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 15:03:56.000000 prefect_azure-0.3.9/prefect_azure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:03:56.337059 prefect_azure-0.3.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.333059 prefect_azure-0.3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.333059 prefect_azure-0.3.9/tests/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)    14605 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/tests/deployments/test_steps.py
--rw-r--r--   0 runner    (1001) docker     (127)    37383 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/tests/test_aci_infrastructure.py
--rw-r--r--   0 runner    (1001) docker     (127)    39151 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/tests/test_aci_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/tests/test_blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/tests/test_cosmos_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/tests/test_ml_datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-26 15:03:41.000000 prefect_azure-0.3.9/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:36.876485 prefect_azure-0.4.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-05-31 20:49:36.876485 prefect_azure-0.4.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:36.872485 prefect_azure-0.4.0rc1/prefect_azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/prefect_azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-31 20:49:36.000000 prefect_azure-0.4.0rc1/prefect_azure/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25778 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/prefect_azure/blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/prefect_azure/container_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/prefect_azure/cosmos_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21736 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/prefect_azure/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:36.872485 prefect_azure-0.4.0rc1/prefect_azure/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/prefect_azure/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/prefect_azure/deployments/steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/prefect_azure/ml_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/prefect_azure/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:36.872485 prefect_azure-0.4.0rc1/prefect_azure/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/prefect_azure/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39311 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/prefect_azure/workers/container_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:36.876485 prefect_azure-0.4.0rc1/prefect_azure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-05-31 20:49:36.000000 prefect_azure-0.4.0rc1/prefect_azure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-31 20:49:36.000000 prefect_azure-0.4.0rc1/prefect_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:49:36.000000 prefect_azure-0.4.0rc1/prefect_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-31 20:49:36.000000 prefect_azure-0.4.0rc1/prefect_azure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-31 20:49:36.000000 prefect_azure-0.4.0rc1/prefect_azure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-31 20:49:36.000000 prefect_azure-0.4.0rc1/prefect_azure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:49:36.876485 prefect_azure-0.4.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:36.876485 prefect_azure-0.4.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:36.876485 prefect_azure-0.4.0rc1/tests/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)    14605 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/tests/deployments/test_steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/tests/test_aci_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38856 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/tests/test_aci_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/tests/test_blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/tests/test_cosmos_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/tests/test_ml_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-31 20:49:23.000000 prefect_azure-0.4.0rc1/tests/test_version.py
```

### Comparing `prefect_azure-0.3.9/LICENSE` & `prefect_azure-0.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.9/PKG-INFO` & `prefect_azure-0.4.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: prefect-azure
-Version: 0.3.9
+Version: 0.4.0rc1
 Summary: Prefect integrations with Microsoft Azure services
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-azure
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
 Requires-Dist: aiohttp
 Requires-Dist: azure_identity>=1.10
 Requires-Dist: azure_mgmt_containerinstance>=10.0
 Requires-Dist: azure-mgmt-resource>=21.2
-Requires-Dist: prefect>=2.14.10
+Requires-Dist: prefect>=3.0.0rc1
+Requires-Dist: setuptools
 Provides-Extra: blob-storage
 Requires-Dist: azure-storage-blob; extra == "blob-storage"
 Provides-Extra: cosmos-db
 Requires-Dist: azure-cosmos; extra == "cosmos-db"
 Provides-Extra: ml-datastore
 Requires-Dist: azureml-core; extra == "ml-datastore"
 Provides-Extra: all-extras
@@ -42,15 +42,14 @@
 Requires-Dist: azureml-core; extra == "dev"
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
```

### Comparing `prefect_azure-0.3.9/README.md` & `prefect_azure-0.4.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.9/prefect_azure/__init__.py` & `prefect_azure-0.4.0rc1/prefect_azure/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from .credentials import (  # noqa
     AzureBlobStorageCredentials,
     AzureCosmosDbCredentials,
     AzureMlCredentials,
     AzureContainerInstanceCredentials,
 )
 from .workers.container_instance import AzureContainerWorker  # noqa
-from .container_instance import AzureContainerInstanceJob  # noqa
 from .blob_storage import AzureBlobStorageContainer  # noqa
 
 __all__ = [
     "AzureBlobStorageCredentials",
     "AzureCosmosDbCredentials",
     "AzureMlCredentials",
     "AzureContainerInstanceCredentials",
-    "AzureContainerInstanceJob",
     "AzureContainerWorker",
     "AzureBlobStorageContainer",
 ]
 
 try:
     from ._version import version as __version__
 except ImportError:
```

### Comparing `prefect_azure-0.3.9/prefect_azure/blob_storage.py` & `prefect_azure-0.4.0rc1/prefect_azure/blob_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,28 +6,23 @@
 from typing import TYPE_CHECKING, Any, BinaryIO, Coroutine, Dict, List, Optional, Union
 
 from azure.core.exceptions import ResourceNotFoundError
 
 if TYPE_CHECKING:
     from azure.storage.blob import BlobProperties
 
-from pydantic import VERSION as PYDANTIC_VERSION
+
+from pydantic import Field
 
 from prefect import task
 from prefect.blocks.abstract import ObjectStorageBlock
 from prefect.filesystems import WritableDeploymentStorage, WritableFileSystem
 from prefect.logging import get_run_logger
 from prefect.utilities.asyncutils import sync_compatible
 from prefect.utilities.filesystem import filter_files
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field
-else:
-    from pydantic import Field
-
 from prefect_azure.credentials import AzureBlobStorageCredentials
 
 
 @task
 async def blob_storage_download(
     container: str,
     blob: str,
```

### Comparing `prefect_azure-0.3.9/prefect_azure/container_instance.py` & `prefect_azure-0.4.0rc1/prefect_azure/workers/container_instance.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,137 +1,188 @@
 """
-Integrations with the Azure Container Instances service.
-Note this module is experimental. The interfaces within may change without notice.
+Module containing the Azure Container Instances worker used for executing flow
+runs in ACI containers.
 
-The `AzureContainerInstanceJob` infrastructure block in this module is ideally
-configured via the Prefect UI and run via a Prefect agent, but it can be called directly
-as demonstrated in the following examples.
-
-Examples:
-    Run a command using an Azure Container Instances container.
-    ```python
-    AzureContainerInstanceJob(command=["echo", "hello world"]).run()
-    ```
-
-    Run a command and stream the container's output to the local terminal.
-    ```python
-    AzureContainerInstanceJob(
-        command=["echo", "hello world"],
-        stream_output=True,
-    )
-    ```
-
-    Run a command with a specific image
-    ```python
-    AzureContainerInstanceJob(command=["echo", "hello world"], image="alpine:latest")
-    ```
-
-    Run a task with custom memory and CPU requirements
-    ```python
-    AzureContainerInstanceJob(command=["echo", "hello world"], memory=1.0, cpu=1.0)
-    ```
-
-    Run a task with custom memory and CPU requirements
-    ```python
-    AzureContainerInstanceJob(command=["echo", "hello world"], memory=1.0, cpu=1.0)
-    ```
+To start an ACI worker, run the following command:
 
-    Run a task with custom memory, CPU, and GPU requirements
-    ```python
-    AzureContainerInstanceJob(command=["echo", "hello world"], memory=1.0, cpu=1.0,
-    gpu_count=1, gpu_sku="V100")
+```bash
+prefect worker start --pool 'my-work-pool' --type azure-container-instance
+```
+
+Replace `my-work-pool` with the name of the work pool you want the worker
+to poll for flow runs.
+
+!!! example "Using a custom ARM template"
+    To facilitate easy customization, the Azure Container worker provisions a
+    containing group using an ARM template. The default ARM template is represented
+    in YAML as follows:
+    ```yaml
+    ---
+    arm_template:
+      "$schema": https://schema.management.azure.com/schemas/2019-08-01/deploymentTemplate.json#
+      contentVersion: 1.0.0.0
+      parameters:
+        location:
+          type: string
+          defaultValue: "[resourceGroup().location]"
+          metadata:
+            description: Location for all resources.
+        container_group_name:
+          type: string
+          defaultValue: "[uniqueString(resourceGroup().id)]"
+          metadata:
+            description: The name of the container group to create.
+        container_name:
+          type: string
+          defaultValue: "[uniqueString(resourceGroup().id)]"
+          metadata:
+            description: The name of the container to create.
+      resources:
+      - type: Microsoft.ContainerInstance/containerGroups
+        apiVersion: '2022-09-01'
+        name: "[parameters('container_group_name')]"
+        location: "[parameters('location')]"
+        properties:
+          containers:
+          - name: "[parameters('container_name')]"
+            properties:
+              image: rpeden/my-aci-flow:latest
+              command: "{{ command }}"
+              resources:
+                requests:
+                  cpu: "{{ cpu }}"
+                  memoryInGB: "{{ memory }}"
+              environmentVariables: []
+          osType: Linux
+          restartPolicy: Never
     ```
 
-    Run a task with custom environment variables
-    ```python
-    AzureContainerInstanceJob(
-        command=["echo", "hello $PLANET"],
-        env={"PLANET": "earth"}
-    )
-    ```
-
-    Run a task that uses a private ACR registry with a managed identity
-    ```python
-    AzureContainerInstanceJob(
-        command=["echo", "hello $PLANET"],
-        image="my-registry.azurecr.io/my-image",
-        image_registry=ACRManagedIdentity(
-            registry_url="my-registry.azurecr.io",
-            identity="/my/managed/identity/123abc"
-        )
-    )
-    ```
-"""
+    Each values enclosed in `{{ }}` is a placeholder that will be replaced with
+    a value at runtime. The values that can be used a placeholders are defined
+    by the `variables` schema defined in the base job template.
+
+    The default job manifest and available variables can be customized on a work pool
+    by work pool basis. These customizations can be made via the Prefect UI when
+    creating or editing a work pool.
+
+    Using an ARM template makes the worker flexible; you're not limited to using the
+    features the worker provides out of the box. Instead, you can modify the ARM
+    template to use any features available in Azure Container Instances.
+"""  # noqa
 
 import datetime
-import json
-import random
-import shlex
-import string
 import sys
 import time
-import uuid
-from copy import deepcopy
 from enum import Enum
-from typing import Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 import anyio
 import dateutil.parser
-from anyio.abc import TaskStatus
 from azure.core.exceptions import HttpResponseError, ResourceNotFoundError
 from azure.core.polling import LROPoller
 from azure.mgmt.containerinstance import ContainerInstanceManagementClient
-from azure.mgmt.containerinstance.models import (
-    Container,
-    ContainerGroup,
-    ContainerGroupIdentity,
-    ContainerGroupRestartPolicy,
-    ContainerGroupSubnetId,
-    DnsConfiguration,
-    EnvironmentVariable,
-    GpuResource,
-    ImageRegistryCredential,
-    Logs,
-    OperatingSystemTypes,
-    ResourceRequests,
-    ResourceRequirements,
-    UserAssignedIdentities,
+from azure.mgmt.containerinstance.models import Container, ContainerGroup, Logs
+from azure.mgmt.resource import ResourceManagementClient
+from azure.mgmt.resource.resources.models import (
+    Deployment,
+    DeploymentExtended,
+    DeploymentMode,
+    DeploymentProperties,
 )
-from pydantic import VERSION as PYDANTIC_VERSION
+from pydantic import Field, SecretStr
+from slugify import slugify
 
-import prefect.infrastructure.container
-from prefect.blocks.core import BlockNotSavedError
+from prefect import get_client
+from prefect.client.schemas import FlowRun
 from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
-from prefect.infrastructure.base import Infrastructure, InfrastructureResult
-from prefect.utilities.asyncutils import run_sync_in_worker_thread, sync_compatible
+from prefect.server.schemas.core import Flow
+from prefect.server.schemas.responses import DeploymentResponse
+from prefect.utilities.asyncutils import run_sync_in_worker_thread
 from prefect.utilities.dockerutils import get_prefect_image_name
+from prefect.workers.base import (
+    BaseJobConfiguration,
+    BaseVariables,
+    BaseWorker,
+    BaseWorkerResult,
+)
+from prefect_azure.container_instance import ACRManagedIdentity
+from prefect_azure.credentials import AzureContainerInstanceCredentials
 
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import BaseModel, Field, SecretStr
-else:
-    from pydantic import BaseModel, Field, SecretStr
+# import aio Azure container instance client
 
-from slugify import slugify
-from typing_extensions import Literal
-
-from prefect_azure.credentials import AzureContainerInstanceCredentials
 
 ACI_DEFAULT_CPU = 1.0
 ACI_DEFAULT_MEMORY = 1.0
 ACI_DEFAULT_GPU = 0.0
 DEFAULT_CONTAINER_ENTRYPOINT = "/opt/prefect/entrypoint.sh"
 # environment variables that ACI should treat as secure variables so they
 # won't appear in logs
 ENV_SECRETS = ["PREFECT_API_KEY"]
 
 # The maximum time to wait for container group deletion before giving up and
 # moving on. Deletion is usually quick, so exceeding this timeout means something
 # has gone wrong and we should raise an exception to inform the user they should
 # check their Azure account for orphaned container groups.
 CONTAINER_GROUP_DELETION_TIMEOUT_SECONDS = 30
+DockerRegistry = Union[ACRManagedIdentity, Any, None]
+
+
+def _get_default_arm_template():
+    """Get the default ARM template for creating a container group."""
+    return {
+        "$schema": "https://schema.management.azure.com/schemas/2019-08-01/deploymentTemplate.json#",  # noqa
+        "contentVersion": "1.0.0.0",
+        "parameters": {
+            "location": {
+                "type": "string",
+                "defaultValue": "[resourceGroup().location]",
+                "metadata": {"description": "Location for all resources."},
+            },
+            "container_group_name": {
+                "type": "string",
+                "defaultValue": "[uniqueString(resourceGroup().id)]",
+                "metadata": {
+                    "description": "The name of the container group to create."
+                },
+            },
+            "container_name": {
+                "type": "string",
+                "defaultValue": "[uniqueString(resourceGroup().id)]",
+                "metadata": {"description": "The name of the container to create."},
+            },
+        },
+        "resources": [
+            {
+                "type": "Microsoft.ContainerInstance/containerGroups",
+                "apiVersion": "2022-09-01",
+                "name": "[parameters('container_group_name')]",
+                "location": "[parameters('location')]",
+                "properties": {
+                    "containers": [
+                        {
+                            "name": "[parameters('container_name')]",
+                            "properties": {
+                                "image": "{{ image }}",
+                                "command": "{{ command }}",
+                                "resources": {
+                                    "requests": {
+                                        "cpu": "{{ cpu }}",
+                                        "memoryInGB": "{{ memory }}",
+                                    }
+                                },
+                                "environmentVariables": [],
+                            },
+                        }
+                    ],
+                    "osType": "Linux",
+                    "restartPolicy": "Never",
+                },
+            }
+        ],
+    }
 
 
 class ContainerGroupProvisioningState(str, Enum):
     """
     Terminal provisioning states for ACI container groups. Per the Azure docs,
     the states in this Enum are the only ones that can be relied on as dependencies.
     """
@@ -145,61 +196,203 @@
     Terminal run states for ACI containers.
     """
 
     RUNNING = "Running"
     TERMINATED = "Terminated"
 
 
-class ACRManagedIdentity(BaseModel):
+class AzureContainerJobConfiguration(BaseJobConfiguration):
     """
-    Use a Managed Identity to access Azure Container registry. Requires the
-    user-assigned managed identity be available to the ACI container group.
+    Configuration for an Azure Container Instance flow run.
     """
 
-    registry_url: str = Field(
-        default=...,
-        title="Registry URL",
-        description=(
-            "The URL to the registry, such as myregistry.azurecr.io. Generally, 'http' "
-            "or 'https' can be omitted."
-        ),
+    image: str = Field(default_factory=get_prefect_image_name)
+    resource_group_name: str = Field(default=...)
+    subscription_id: SecretStr = Field(default=...)
+    identities: Optional[List[str]] = Field(default=None)
+    entrypoint: Optional[str] = Field(default=DEFAULT_CONTAINER_ENTRYPOINT)
+    image_registry: DockerRegistry = Field(default=None)
+    cpu: float = Field(default=ACI_DEFAULT_CPU)
+    gpu_count: Optional[int] = Field(default=None)
+    gpu_sku: Optional[str] = Field(default=None)
+    memory: float = Field(default=ACI_DEFAULT_MEMORY)
+    subnet_ids: Optional[List[str]] = Field(default=None)
+    dns_servers: Optional[List[str]] = Field(default=None)
+    stream_output: bool = Field(default=False)
+    aci_credentials: AzureContainerInstanceCredentials = Field(
+        # default to an empty credentials object that will use
+        # `DefaultAzureCredential` to authenticate.
+        default_factory=AzureContainerInstanceCredentials
     )
-    identity: str = Field(
-        default=...,
-        description=(
-            "The user-assigned Azure managed identity for the private registry."
-        ),
+    # Execution settings
+    task_start_timeout_seconds: int = Field(default=240)
+    task_watch_poll_interval: float = Field(default=5.0)
+    arm_template: Dict[str, Any] = Field(
+        json_schema_extra=dict(template=_get_default_arm_template())
     )
+    keep_container_group: bool = Field(default=False)
 
+    def prepare_for_flow_run(
+        self,
+        flow_run: "FlowRun",
+        deployment: Optional["DeploymentResponse"] = None,
+        flow: Optional["Flow"] = None,
+    ):
+        """
+        Prepares the job configuration for a flow run.
+        """
+        super().prepare_for_flow_run(flow_run, deployment, flow)
 
-class AzureContainerInstanceJobResult(InfrastructureResult):
-    """
-    The result of an `AzureContainerInstanceJob` run.
-    """
+        # expectations:
+        # - the first resource in the template is the container group
+        # - the container group has a single container
+        container_group = self.arm_template["resources"][0]
+        container = container_group["properties"]["containers"][0]
+
+        # set the container's environment variables
+        container["properties"]["environmentVariables"] = self._get_arm_environment()
+
+        # convert the command from a string to a list, because that's what ACI expects
+        if self.command:
+            container["properties"]["command"] = self.command.split(" ")
+
+        self._add_image()
+
+        # Add the entrypoint if provided. Creating an ACI container with a
+        # command overrides the container's built-in entrypoint. Prefect base images
+        # use entrypoint.sh as the entrypoint, so we need to add to the beginning of
+        # the command list to avoid breaking EXTRA_PIP_PACKAGES installation on
+        # container startup.
+        if self.entrypoint:
+            container["properties"]["command"].insert(0, self.entrypoint)
+
+        if self.image_registry:
+            self._add_image_registry_credentials(self.image_registry)
 
+        if self.identities:
+            self._add_identities(self.identities)
+
+        if self.subnet_ids:
+            self._add_subnets(self.subnet_ids)
+
+        if self.dns_servers:
+            self._add_dns_servers(self.dns_servers)
+
+    def _add_image(self):
+        """
+        Add the image to the arm template.
+        """
+        try:
+            self.arm_template["resources"][0]["properties"]["containers"][0][
+                "properties"
+            ]["image"] = self.image
+        except KeyError:
+            raise ValueError("Unable to add image due to invalid job ARM template.")
+
+    def _add_image_registry_credentials(self, image_registry: DockerRegistry):
+        """
+        Create image registry credentials based on the type of image_registry provided.
+
+        Args:
+            image_registry: An instance of a DockerRegistry or
+            ACRManagedIdentity object.
+        """
+        if not image_registry:
+            return
+
+        if isinstance(image_registry, ACRManagedIdentity):
+            self.arm_template["resources"][0]["properties"][
+                "imageRegistryCredentials"
+            ] = [
+                {
+                    "server": image_registry.registry_url,
+                    "identity": image_registry.identity,
+                }
+            ]
+        elif (
+            hasattr(image_registry, "username")
+            and hasattr(image_registry, "password")
+            and hasattr(image_registry, "registry_url")
+        ):
+            self.arm_template["resources"][0]["properties"][
+                "imageRegistryCredentials"
+            ] = [
+                {
+                    "server": image_registry.registry_url,
+                    "username": image_registry.username,
+                    "password": image_registry.password.get_secret_value(),
+                }
+            ]
+
+    def _add_identities(self, identities: List[str]):
+        """
+        Add identities to the container group.
+
+        Args:
+            identities: A list of user-assigned identities to add to
+            the container group.
+        """
+        self.arm_template["resources"][0]["identity"] = {
+            "type": "UserAssigned",
+            "userAssignedIdentities": {
+                # note: For user-assigned identities, the key is the resource ID
+                # of the identity and the value is an empty object. See:
+                # https://docs.microsoft.com/en-us/azure/templates/microsoft.containerinstance/containergroups?tabs=bicep#identity-object # noqa
+                identity: {}
+                for identity in identities
+            },
+        }
 
-class AzureContainerInstanceJob(Infrastructure):
+    def _add_subnets(self, subnet_ids: List[str]):
+        """
+        Add subnets to the container group.
+
+        Args:
+            subnet_ids: A list of subnet ids to add to the container group.
+        """
+        self.arm_template["resources"][0]["properties"]["subnetIds"] = [
+            {"id": subnet_id} for subnet_id in subnet_ids
+        ]
+
+    def _add_dns_servers(self, dns_servers: List[str]):
+        """
+        Add dns servers to the container group.
+
+        Args:
+            dns_servers: A list of dns servers to add to the container group.
+        """
+        self.arm_template["resources"][0]["properties"]["dnsConfig"] = {
+            "nameServers": dns_servers
+        }
+
+    def _get_arm_environment(self):
+        """
+        Returns the environment variables to pass to the ARM template.
+        """
+        env = {**self._base_environment(), **self.env}
+
+        azure_env = [
+            {"name": key, "secureValue": value}
+            if key in ENV_SECRETS
+            else {"name": key, "value": value}
+            for key, value in env.items()
+        ]
+        return azure_env
+
+
+class AzureContainerVariables(BaseVariables):
     """
-    Run a command using a container on Azure Container Instances.
-    Note this block is experimental. The interface may change without notice.
+    Variables for an Azure Container Instance flow run.
     """
 
-    _block_type_name = "Azure Container Instance Job"
-    _logo_url = "https://cdn.sanity.io/images/3ugk85nk/production/54e3fa7e00197a4fbd1d82ed62494cb58d08c96a-250x250.png"  # noqa
-    _description = "Run tasks using Azure Container Instances. Note this block is experimental. The interface may change without notice."  # noqa
-    _documentation_url = "https://prefecthq.github.io/prefect-azure/container_instance/#prefect_azure.container_instance.AzureContainerInstanceJob"  # noqa
-
-    type: Literal["container-instance-job"] = Field(
-        default="container-instance-job", description="The slug for this task type."
-    )
-    aci_credentials: AzureContainerInstanceCredentials = Field(
-        default_factory=AzureContainerInstanceCredentials,
+    image: str = Field(
+        default_factory=get_prefect_image_name,
         description=(
-            "Credentials for Azure Container Instances; "
-            "if not provided will attempt to use DefaultAzureCredentials."
+            "The image to use for the Prefect container in the task. This value "
+            "defaults to a Prefect base image matching your local versions."
         ),
     )
     resource_group_name: str = Field(
         default=...,
         title="Azure Resource Group Name",
         description=(
             "The name of the Azure Resource Group in which to run Prefect ACI tasks."
@@ -215,37 +408,25 @@
         default=None,
         description=(
             "A list of user-assigned identities to associate with the container group. "
             "The identities should be an ARM resource IDs in the form: "
             "'/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ManagedIdentity/userAssignedIdentities/{identityName}'."  # noqa
         ),
     )
-    image: Optional[str] = Field(
-        default_factory=get_prefect_image_name,
-        description=(
-            "The image to use for the Prefect container in the task. This value "
-            "defaults to a Prefect base image matching your local versions."
-        ),
-    )
     entrypoint: Optional[str] = Field(
         default=DEFAULT_CONTAINER_ENTRYPOINT,
         description=(
             "The entrypoint of the container you wish you run. This value "
             "defaults to the entrypoint used by Prefect images and should only be "
             "changed when using a custom image that is not based on an official "
             "Prefect image. Any commands set on deployments will be passed "
             "to the entrypoint as parameters."
         ),
     )
-    image_registry: Optional[
-        Union[
-            prefect.infrastructure.container.DockerRegistry,
-            ACRManagedIdentity,
-        ]
-    ] = Field(
+    image_registry: DockerRegistry = Field(
         default=None,
         title="Image Registry (Optional)",
         description=(
             "To use any private container registry with a username and password, "
             "choose DockerRegistry. To use a private Azure Container Registry "
             "with a managed identity, choose ACRManagedIdentity."
         ),
@@ -280,39 +461,34 @@
             "The amount of memory in gigabytes to provide to the ACI task. Valid "
             "amounts are specified in the Azure documentation. If not provided, a "
             f"default value of  {ACI_DEFAULT_MEMORY} will be used unless present "
             "on the task definition."
         ),
     )
     subnet_ids: Optional[List[str]] = Field(
-        default=None,
         title="Subnet IDs",
-        description="A list of Azure subnet IDs the container should be connected to.",
+        default=None,
+        description=("A list of subnet IDs to associate with the container group. "),
     )
     dns_servers: Optional[List[str]] = Field(
-        default=None,
         title="DNS Servers",
-        description="A list of custom DNS Servers the container should use.",
-    )
-    stream_output: Optional[bool] = Field(
         default=None,
+        description=("A list of DNS servers to associate with the container group."),
+    )
+    aci_credentials: AzureContainerInstanceCredentials = Field(
+        default_factory=AzureContainerInstanceCredentials,
+        description=("The credentials to use to authenticate with Azure."),
+    )
+    stream_output: bool = Field(
+        default=False,
         description=(
             "If `True`, logs will be streamed from the Prefect container to the local "
             "console."
         ),
     )
-    env: Dict[str, Optional[str]] = Field(
-        title="Environment Variables",
-        default_factory=dict,
-        description=(
-            "Environment variables to provide to the task run. These variables are set "
-            "on the Prefect container at task runtime. These will not be set on the "
-            "task definition."
-        ),
-    )
     # Execution settings
     task_start_timeout_seconds: int = Field(
         default=240,
         description=(
             "The amount of time to watch for the start of the ACI container. "
             "before marking it as failed."
         ),
@@ -320,474 +496,324 @@
     task_watch_poll_interval: float = Field(
         default=5.0,
         description=(
             "The number of seconds to wait between Azure API calls while monitoring "
             "the state of an Azure Container Instances task."
         ),
     )
+    keep_container_group: bool = Field(
+        default=False,
+        title="Keep Container Group After Completion",
+        description="Keep the completed container group on Azure.",
+    )
+
+
+class AzureContainerWorkerResult(BaseWorkerResult):
+    """Contains information about the final state of a completed process"""
+
+
+class AzureContainerWorker(BaseWorker):
+    """
+    A Prefect worker that runs flows in an Azure Container Instance.
+    """
+
+    type: str = "azure-container-instance"
+    job_configuration = AzureContainerJobConfiguration
+    job_configuration_variables = AzureContainerVariables
+    _logo_url = "https://cdn.sanity.io/images/3ugk85nk/production/54e3fa7e00197a4fbd1d82ed62494cb58d08c96a-250x250.png"  # noqa
+    _display_name = "Azure Container Instances"
+    _description = (
+        "Execute flow runs within containers on Azure's Container Instances "
+        "service. Requires an Azure account."
+    )
+    _documentation_url = (
+        "https://prefecthq.github.io/prefect-azure/container_instance_worker/"
+    )
 
-    @sync_compatible
     async def run(
-        self, task_status: Optional[TaskStatus] = None
-    ) -> AzureContainerInstanceJobResult:
+        self,
+        flow_run: FlowRun,
+        configuration: AzureContainerJobConfiguration,
+        task_status: Optional[anyio.abc.TaskStatus] = None,
+    ):
         """
-        Runs the configured task using an ACI container.
-
+        Run a flow in an Azure Container Instance.
         Args:
-            task_status: An optional `TaskStatus` to update when the container starts.
+            flow_run: The flow run to run.
+            configuration: The configuration for the flow run.
+            task_status: The task status object for the current task. Used
+            to provide an identifier that can be used to cancel the task.
 
         Returns:
-            An `AzureContainerInstanceJobResult` with the container's exit code.
+            The result of the flow run.
         """
-
         run_start_time = datetime.datetime.now(datetime.timezone.utc)
+        prefect_client = get_client()
 
-        container = self._configure_container()
-        container_group = self._configure_container_group(container)
-        created_container_group = None
+        # Get the flow, so we can use its name in the container group name
+        # to make it easier to identify and debug.
+        flow = await prefect_client.read_flow(flow_run.flow_id)
+        container_group_name = f"{flow.name}-{flow_run.id}"
+
+        # Slugify flow.name if the generated name will be too long for the
+        # max deployment name length (64) including "prefect-"
+        if len(container_group_name) > 55:
+            slugified_flow_name = slugify(
+                flow.name,
+                max_length=55 - len(str(flow_run.id)),
+                regex_pattern=r"[^a-zA-Z0-9-]+",
+            )
+            container_group_name = f"{slugified_flow_name}-{flow_run.id}"
 
-        aci_client = self.aci_credentials.get_container_client(
-            self.subscription_id.get_secret_value()
+        self._logger.info(
+            f"{self._log_prefix}: Preparing to run command {configuration.command} "
+            f"in container  {configuration.image})..."
         )
 
-        self.logger.info(
-            f"{self._log_prefix}: Preparing to run command {' '.join(self.command)!r} "
-            f"in container {container.name!r} ({self.image})..."
+        aci_client = configuration.aci_credentials.get_container_client(
+            configuration.subscription_id.get_secret_value()
+        )
+        resource_client = configuration.aci_credentials.get_resource_client(
+            configuration.subscription_id.get_secret_value()
         )
+
+        created_container_group: Union[ContainerGroup, None] = None
         try:
-            self.logger.info(f"{self._log_prefix}: Waiting for container creation...")
-            # Create the container group and wait for it to start
-            creation_status_poller = await run_sync_in_worker_thread(
-                aci_client.container_groups.begin_create_or_update,
-                self.resource_group_name,
-                container.name,
-                container_group,
-            )
-            created_container_group = await run_sync_in_worker_thread(
-                self._wait_for_task_container_start, creation_status_poller
+            self._logger.info(f"{self._log_prefix}: Creating container group...")
+
+            created_container_group = await self._provision_container_group(
+                aci_client,
+                resource_client,
+                configuration,
+                container_group_name,
             )
+            # Both the flow ID and container group name will be needed to
+            # cancel the flow run if needed.
+            identifier = f"{flow_run.id}:{container_group_name}"
 
-            # If creation succeeded, group provisioning state should be 'Succeeded'
-            # and the group should have a single container
             if self._provisioning_succeeded(created_container_group):
-                self.logger.info(f"{self._log_prefix}: Running command...")
-                if task_status:
-                    task_status.started(value=created_container_group.name)
+                self._logger.info(f"{self._log_prefix}: Running command...")
+                if task_status is not None:
+                    task_status.started(value=identifier)
+
                 status_code = await run_sync_in_worker_thread(
                     self._watch_task_and_get_exit_code,
                     aci_client,
+                    configuration,
                     created_container_group,
                     run_start_time,
                 )
-                self.logger.info(f"{self._log_prefix}: Completed command run.")
+
+                self._logger.info(f"{self._log_prefix}: Completed command run.")
+
             else:
                 raise RuntimeError(f"{self._log_prefix}: Container creation failed.")
 
         finally:
-            if created_container_group:
+            if configuration.keep_container_group:
+                self._logger.info(f"{self._log_prefix}: Stopping container group...")
+                aci_client.container_groups.stop(
+                    resource_group_name=configuration.resource_group_name,
+                    container_group_name=container_group_name,
+                )
+            else:
                 await self._wait_for_container_group_deletion(
-                    aci_client, created_container_group
+                    aci_client, configuration, container_group_name
                 )
 
-        return AzureContainerInstanceJobResult(
+        return AzureContainerWorkerResult(
             identifier=created_container_group.name, status_code=status_code
         )
 
-    async def kill(
+    async def kill_infrastructure(
         self,
-        container_group_name: str,
-        grace_seconds: int = CONTAINER_GROUP_DELETION_TIMEOUT_SECONDS,
+        infrastructure_pid: str,
+        configuration: AzureContainerJobConfiguration,
     ):
         """
         Kill a flow running in an ACI container group.
 
         Args:
-            container_group_name: The container group name yielded by
+            infrastructure_pid: The container group identification data yielded by
                 `AzureContainerInstanceJob.run`.
+            configuration: The job configuration.
         """
-        # ACI does not provide a way to specify grace period, but it gives
-        # applications ~30 seconds to gracefully terminate before killing
-        # a container group.
-        if grace_seconds != CONTAINER_GROUP_DELETION_TIMEOUT_SECONDS:
-            self.logger.warning(
-                f"{self._log_prefix}: Kill grace period of {grace_seconds}s requested, "
-                f"but ACI does not support grace period configuration."
-            )
+        (flow_run_id, container_group_name) = infrastructure_pid.split(":")
 
-        aci_client = self.aci_credentials.get_container_client(
-            self.subscription_id.get_secret_value()
+        aci_client = configuration.aci_credentials.get_container_client(
+            configuration.subscription_id.get_secret_value()
         )
 
         # get the container group to check that it still exists
         try:
             container_group = aci_client.container_groups.get(
-                resource_group_name=self.resource_group_name,
+                resource_group_name=configuration.resource_group_name,
                 container_group_name=container_group_name,
             )
         except ResourceNotFoundError as exc:
             # the container group no longer exists, so there's nothing to cancel
             raise InfrastructureNotFound(
-                f"Cannot stop ACI job: container group {container_group_name} "
-                "no longer exists."
+                f"Cannot stop ACI job: container group "
+                f"{container_group_name} no longer exists."
             ) from exc
 
         # get the container state to check if the container has terminated
         container = self._get_container(container_group)
         container_state = container.instance_view.current_state.state
 
         # the container group needs to be deleted regardless of whether the container
         # already terminated
-        await self._wait_for_container_group_deletion(aci_client, container_group)
+        await self._wait_for_container_group_deletion(
+            aci_client, configuration, container_group_name
+        )
 
-        # if the container had already terminated, raise an exception to let the agent
+        # if the container has already terminated, raise an exception to let the agent
         # know the flow was not cancelled
         if container_state == ContainerRunState.TERMINATED:
             raise InfrastructureNotAvailable(
                 f"Cannot stop ACI job: container group {container_group.name} exists, "
                 f"but container {container.name} has already terminated."
             )
 
-    def preview(self) -> str:
-        """
-        Provides a summary of how the container will be created when `run` is called.
-
-        Returns:
-           A string containing the summary.
-        """
-        preview = {
-            "container_name": "<generated when run>",
-            "resource_group_name": self.resource_group_name,
-            "memory": self.memory,
-            "cpu": self.cpu,
-            "gpu_count": self.gpu_count,
-            "gpu_sku": self.gpu_sku,
-            "env": self._get_environment(),
-        }
-
-        return json.dumps(preview)
-
-    def get_corresponding_worker_type(self) -> str:
-        """Return the corresponding worker type for this infrastructure block."""
-        from prefect_azure.workers.container_instance import AzureContainerWorker
-
-        return AzureContainerWorker.type
-
-    async def generate_work_pool_base_job_template(self) -> dict:
-        """
-        Generate a base job template for an `Azure Container Instance` work pool
-        with the same configuration as this block.
-
-        Returns:
-            - dict: a base job template for an `Azure Container Instance` work pool
-        """
-        from prefect_azure.workers.container_instance import AzureContainerWorker
-
-        base_job_template = deepcopy(
-            AzureContainerWorker.get_default_base_job_template()
-        )
-        for key, value in self.dict(exclude_unset=True, exclude_defaults=True).items():
-            if key == "command":
-                base_job_template["variables"]["properties"]["command"][
-                    "default"
-                ] = shlex.join(value)
-            elif key in [
-                "type",
-                "block_type_slug",
-                "_block_document_id",
-                "_block_document_name",
-                "_is_anonymous",
-            ]:
-                continue
-            elif key == "subscription_id":
-                base_job_template["variables"]["properties"]["subscription_id"][
-                    "default"
-                ] = value.get_secret_value()
-            elif key == "aci_credentials":
-                if not self.aci_credentials._block_document_id:
-                    raise BlockNotSavedError(
-                        "It looks like you are trying to use a block that"
-                        " has not been saved. Please call `.save` on your block"
-                        " before publishing it as a work pool."
-                    )
-                base_job_template["variables"]["properties"]["aci_credentials"][
-                    "default"
-                ] = {
-                    "$ref": {
-                        "block_document_id": str(
-                            self.aci_credentials._block_document_id
-                        )
-                    }
-                }
-            elif key == "image_registry":
-                if not self.image_registry._block_document_id:
-                    raise BlockNotSavedError(
-                        "It looks like you are trying to use a block that"
-                        " has not been saved. Please call `.save` on your block"
-                        " before publishing it as a work pool."
-                    )
-                base_job_template["variables"]["properties"]["image_registry"][
-                    "default"
-                ] = {
-                    "$ref": {
-                        "block_document_id": str(self.image_registry._block_document_id)
-                    }
-                }
-            elif key in base_job_template["variables"]["properties"]:
-                base_job_template["variables"]["properties"][key]["default"] = value
-            else:
-                self.logger.warning(
-                    f"Variable {key!r} is not supported by `Azure Container Instance`"
-                    " work pools. Skipping."
-                )
-
-        return base_job_template
-
-    def _configure_container(self) -> Container:
-        """
-        Configures an Azure `Container` using data from the block's fields.
-
-        Returns:
-            An instance of `Container` ready to submit to Azure.
-        """
-
-        # setup container environment variables
-        environment = [
-            EnvironmentVariable(name=k, secure_value=v)
-            if k in ENV_SECRETS
-            else EnvironmentVariable(name=k, value=v)
-            for (k, v) in self._get_environment().items()
-        ]
-
-        # all container names in a resource group must be unique
-        if self.name:
-            slugified_name = slugify(
-                self.name,
-                max_length=52,
-                regex_pattern=r"[^a-zA-Z0-9-]+",
-            )
-            random_suffix = "".join(
-                random.choices(string.ascii_lowercase + string.digits, k=10)
-            )
-            container_name = slugified_name + "-" + random_suffix
-        else:
-            container_name = str(uuid.uuid4())
-
-        container_resource_requirements = self._configure_container_resources()
-
-        # add the entrypoint if provided, because creating an ACI container with a
-        # command overrides the container's built-in entrypoint.
-        if self.entrypoint:
-            self.command.insert(0, self.entrypoint)
-
-        return Container(
-            name=container_name,
-            image=self.image,
-            command=self.command,
-            resources=container_resource_requirements,
-            environment_variables=environment,
-        )
-
-    def _configure_container_resources(self) -> ResourceRequirements:
-        """
-        Configures the container's memory, CPU, and GPU resources.
-
-        Returns:
-            A `ResourceRequirements` instance initialized with data from this
-            `AzureContainerInstanceJob` block.
-        """
-
-        gpu_resource = (
-            GpuResource(count=self.gpu_count, sku=self.gpu_sku)
-            if self.gpu_count and self.gpu_sku
-            else None
-        )
-        container_resource_requests = ResourceRequests(
-            memory_in_gb=self.memory, cpu=self.cpu, gpu=gpu_resource
-        )
-
-        return ResourceRequirements(requests=container_resource_requests)
-
-    def _configure_container_group(self, container: Container) -> ContainerGroup:
-        """
-        Configures the container group needed to start a container on ACI.
-
-        Args:
-            container: An initialized instance of `Container`.
-
-        Returns:
-            An initialized `ContainerGroup` ready to submit to Azure.
-        """
-
-        # Load the resource group, so we can set the container group location
-        # correctly.
-
-        resource_group_client = self.aci_credentials.get_resource_client(
-            self.subscription_id.get_secret_value()
-        )
-
-        resource_group = resource_group_client.resource_groups.get(
-            self.resource_group_name
-        )
-
-        image_registry_credentials = self._create_image_registry_credentials(
-            self.image_registry
-        )
-
-        identity = (
-            ContainerGroupIdentity(
-                type="UserAssigned",
-                # The Azure API only uses the dict keys and ignores values when
-                # creating a container group. Using empty `UserAssignedIdentities`
-                # instances as dict values satisfies Python type checkers.
-                user_assigned_identities={
-                    identity: UserAssignedIdentities() for identity in self.identities
-                },
-            )
-            if self.identities
-            else None
-        )
-
-        subnet_ids = (
-            [ContainerGroupSubnetId(id=subnet_id) for subnet_id in self.subnet_ids]
-            if self.subnet_ids
-            else None
-        )
-
-        dns_config = (
-            DnsConfiguration(name_servers=self.dns_servers)
-            if self.dns_servers
-            else None
-        )
-
-        return ContainerGroup(
-            location=resource_group.location,
-            identity=identity,
-            containers=[container],
-            os_type=OperatingSystemTypes.linux,
-            restart_policy=ContainerGroupRestartPolicy.never,
-            image_registry_credentials=image_registry_credentials,
-            subnet_ids=subnet_ids,
-            dns_config=dns_config,
-        )
-
-    @staticmethod
-    def _create_image_registry_credentials(
-        image_registry: Union[
-            prefect.infrastructure.container.DockerRegistry,
-            ACRManagedIdentity,
-            None,
-        ],
-    ):
-        """
-        Create image registry credentials based on the type of image_registry provided.
-
-        Args:
-            image_registry: An instance of a DockerRegistry or
-            ACRManagedIdentity object.
-
-        Returns:
-            A list containing an ImageRegistryCredential object if the input is a
-            `DockerRegistry` or `ACRManagedIdentity`, or None if the
-            input doesn't match any of the expected types.
-        """
-        if image_registry and isinstance(
-            image_registry, prefect.infrastructure.container.DockerRegistry
-        ):
-            return [
-                ImageRegistryCredential(
-                    server=image_registry.registry_url,
-                    username=image_registry.username,
-                    password=image_registry.password.get_secret_value(),
-                )
-            ]
-        elif image_registry and isinstance(image_registry, ACRManagedIdentity):
-            return [
-                ImageRegistryCredential(
-                    server=image_registry.registry_url,
-                    identity=image_registry.identity,
-                )
-            ]
-        else:
-            return None
-
     def _wait_for_task_container_start(
-        self, creation_status_poller: LROPoller[ContainerGroup]
-    ) -> ContainerGroup:
+        self,
+        client: ContainerInstanceManagementClient,
+        configuration: AzureContainerJobConfiguration,
+        container_group_name: str,
+        creation_status_poller: LROPoller[DeploymentExtended],
+    ) -> Optional[ContainerGroup]:
         """
         Wait for the result of group and container creation.
 
         Args:
             creation_status_poller: Poller returned by the Azure SDK.
 
         Raises:
             RuntimeError: Raised if the timeout limit is exceeded before the
             container starts.
 
         Returns:
             A `ContainerGroup` representing the current status of the group being
-            watched.
+            watched, or None if creation failed.
         """
-
         t0 = time.time()
-        timeout = self.task_start_timeout_seconds
+        timeout = configuration.task_start_timeout_seconds
 
         while not creation_status_poller.done():
             elapsed_time = time.time() - t0
 
             if timeout and elapsed_time > timeout:
                 raise RuntimeError(
                     (
                         f"Timed out after {elapsed_time}s while watching waiting for "
                         "container start."
                     )
                 )
-            time.sleep(self.task_watch_poll_interval)
+            time.sleep(configuration.task_watch_poll_interval)
+
+        deployment = creation_status_poller.result()
+
+        provisioning_succeeded = (
+            deployment.properties.provisioning_state
+            == ContainerGroupProvisioningState.SUCCEEDED
+        )
 
-        return creation_status_poller.result()
+        if provisioning_succeeded:
+            return self._get_container_group(
+                client, configuration.resource_group_name, container_group_name
+            )
+        else:
+            return None
+
+    async def _provision_container_group(
+        self,
+        aci_client: ContainerInstanceManagementClient,
+        resource_client: ResourceManagementClient,
+        configuration: AzureContainerJobConfiguration,
+        container_group_name: str,
+    ):
+        """
+        Create a container group and wait for it to start.
+        Args:
+            aci_client: An authenticated ACI client.
+            resource_client: An authenticated resource client.
+            configuration: The job configuration.
+            container_group_name: The name of the container group to create.
+
+        Returns:
+            A `ContainerGroup` representing the container group that was created.
+        """
+        properties = DeploymentProperties(
+            mode=DeploymentMode.INCREMENTAL,
+            template=configuration.arm_template,
+            parameters={"container_group_name": {"value": container_group_name}},
+        )
+        deployment = Deployment(properties=properties)
+
+        creation_status_poller = await run_sync_in_worker_thread(
+            resource_client.deployments.begin_create_or_update,
+            resource_group_name=configuration.resource_group_name,
+            deployment_name=f"prefect-{container_group_name}",
+            parameters=deployment,
+        )
+
+        created_container_group = await run_sync_in_worker_thread(
+            self._wait_for_task_container_start,
+            aci_client,
+            configuration,
+            container_group_name,
+            creation_status_poller,
+        )
+
+        return created_container_group
 
     def _watch_task_and_get_exit_code(
         self,
         client: ContainerInstanceManagementClient,
+        configuration: AzureContainerJobConfiguration,
         container_group: ContainerGroup,
         run_start_time: datetime.datetime,
     ) -> int:
         """
         Waits until the container finishes running and obtains its exit code.
 
         Args:
             client: An initialized Azure `ContainerInstanceManagementClient`
             container_group: The `ContainerGroup` in which the container resides.
 
         Returns:
             An `int` representing the container's exit code.
         """
-
         status_code = -1
         running_container = self._get_container(container_group)
         current_state = running_container.instance_view.current_state.state
 
         # get any logs the container has already generated
         last_log_time = run_start_time
-        if self.stream_output:
+        if configuration.stream_output:
             last_log_time = self._get_and_stream_output(
-                client, container_group, last_log_time
+                client=client,
+                configuration=configuration,
+                container_group=container_group,
+                last_log_time=last_log_time,
             )
 
         # set exit code if flow run already finished:
         if current_state == ContainerRunState.TERMINATED:
             status_code = running_container.instance_view.current_state.exit_code
 
         while current_state != ContainerRunState.TERMINATED:
             try:
-                container_group = client.container_groups.get(
-                    resource_group_name=self.resource_group_name,
-                    container_group_name=container_group.name,
+                container_group = self._get_container_group(
+                    client,
+                    configuration.resource_group_name,
+                    container_group.name,
                 )
             except ResourceNotFoundError:
-                self.logger.exception(
+                self._logger.exception(
                     f"{self._log_prefix}: Container group was deleted before flow run "
                     "completed, likely due to flow cancellation."
                 )
 
                 # since the flow was cancelled, exit early instead of raising an
                 # exception
                 return status_code
@@ -797,64 +823,90 @@
 
             if current_state == ContainerRunState.TERMINATED:
                 status_code = container.instance_view.current_state.exit_code
                 # break instead of waiting for next loop iteration because
                 # trying to read logs from a terminated container raises an exception
                 break
 
-            if self.stream_output:
+            if configuration.stream_output:
                 last_log_time = self._get_and_stream_output(
-                    client, container_group, last_log_time
+                    client=client,
+                    configuration=configuration,
+                    container_group=container_group,
+                    last_log_time=last_log_time,
                 )
 
-            time.sleep(self.task_watch_poll_interval)
+            time.sleep(configuration.task_watch_poll_interval)
 
         return status_code
 
     async def _wait_for_container_group_deletion(
         self,
         aci_client: ContainerInstanceManagementClient,
-        container_group: ContainerGroup,
+        configuration: AzureContainerJobConfiguration,
+        container_group_name: str,
     ):
-        self.logger.info(f"{self._log_prefix}: Deleting container...")
+        """
+        Wait for the container group to be deleted.
+        Args:
+            aci_client: An authenticated ACI client.
+            configuration: The job configuration.
+            container_group_name: The name of the container group to delete.
+        """
+        self._logger.info(f"{self._log_prefix}: Deleting container...")
 
         deletion_status_poller = await run_sync_in_worker_thread(
             aci_client.container_groups.begin_delete,
-            resource_group_name=self.resource_group_name,
-            container_group_name=container_group.name,
+            resource_group_name=configuration.resource_group_name,
+            container_group_name=container_group_name,
         )
 
         t0 = time.time()
         timeout = CONTAINER_GROUP_DELETION_TIMEOUT_SECONDS
 
         while not deletion_status_poller.done():
             elapsed_time = time.time() - t0
 
             if timeout and elapsed_time > timeout:
                 raise RuntimeError(
                     (
                         f"Timed out after {elapsed_time}s while waiting for deletion of"
-                        f" container group {container_group.name}. To verify the group "
+                        f" container group {container_group_name}. To verify the group "
                         "has been deleted, check the Azure Portal or run "
-                        f"az container show --name {container_group.name} --resource-group {self.resource_group_name}"  # noqa
+                        f"az container show --name {container_group_name} --resource-group {configuration.resource_group_name}"  # noqa
                     )
                 )
-            await anyio.sleep(self.task_watch_poll_interval)
+            await anyio.sleep(configuration.task_watch_poll_interval)
 
-        self.logger.info(f"{self._log_prefix}: Container deleted.")
+        self._logger.info(f"{self._log_prefix}: Container deleted.")
 
     def _get_container(self, container_group: ContainerGroup) -> Container:
         """
         Extracts the job container from a container group.
         """
         return container_group.containers[0]
 
+    @staticmethod
+    def _get_container_group(
+        client: ContainerInstanceManagementClient,
+        resource_group_name: str,
+        container_group_name: str,
+    ) -> ContainerGroup:
+        """
+        Gets the container group from Azure.
+        """
+        return client.container_groups.get(
+            resource_group_name=resource_group_name,
+            container_group_name=container_group_name,
+        )
+
     def _get_and_stream_output(
         self,
         client: ContainerInstanceManagementClient,
+        configuration: AzureContainerJobConfiguration,
         container_group: ContainerGroup,
         last_log_time: datetime.datetime,
     ) -> datetime.datetime:
         """
         Fetches logs output from the job container and writes all entries after
         a given time to stderr.
 
@@ -862,20 +914,23 @@
             client: An initialized `ContainerInstanceManagementClient`
             container_group: The container group that holds the job container.
             last_log_time: The timestamp of the last output line already streamed.
 
         Returns:
             The time of the most recent output line written by this call.
         """
-        logs = self._get_logs(client, container_group)
+        logs = self._get_logs(
+            client=client, configuration=configuration, container_group=container_group
+        )
         return self._stream_output(logs, last_log_time)
 
     def _get_logs(
         self,
         client: ContainerInstanceManagementClient,
+        configuration: AzureContainerJobConfiguration,
         container_group: ContainerGroup,
         max_lines: int = 100,
     ) -> str:
         """
         Gets the most container logs up to a given maximum.
 
         Args:
@@ -887,28 +942,29 @@
             A string containing the requested log entries, one per line.
         """
         container = self._get_container(container_group)
 
         logs: Union[Logs, None] = None
         try:
             logs = client.containers.list_logs(
-                resource_group_name=self.resource_group_name,
+                resource_group_name=configuration.resource_group_name,
                 container_group_name=container_group.name,
                 container_name=container.name,
                 tail=max_lines,
                 timestamps=True,
             )
         except HttpResponseError:
             # Trying to get logs when the container is under heavy CPU load sometimes
             # results in an error, but we won't want to raise an exception and stop
             # monitoring the flow. Instead, log the error and carry on so we can try to
             # get all missed logs on the next check.
-            self.logger.warning(
+            self._logger.warning(
                 f"{self._log_prefix}: Unable to retrieve logs from container "
-                f"{container.name}. Trying again in {self.task_watch_poll_interval}s"
+                f"{container.name}. Trying again in "
+                f"{configuration.task_watch_poll_interval}s"
             )
 
         return logs.content if logs else ""
 
     def _stream_output(
         self, log_content: Union[str, None], last_log_time: datetime.datetime
     ) -> datetime.datetime:
@@ -942,44 +998,37 @@
 
             try:
                 line_time = dateutil.parser.parse(line_timestamp)
                 if line_time > last_written_time:
                     self._write_output_line(line)
                     last_written_time = line_time
             except dateutil.parser.ParserError as e:
-                self.logger.debug(
+                self._logger.debug(
                     (
                         f"{self._log_prefix}: Unable to parse timestamp from Azure "
                         "log line: %s"
                     ),
                     log_line,
                     exc_info=e,
                 )
 
         return last_written_time
 
-    def _get_environment(self):
-        """
-        Generates a dictionary of all environment variables to send to the
-        ACI container.
-        """
-        return {**self._base_environment(), **self.env}
-
     @property
     def _log_prefix(self) -> str:
         """
         Internal property for generating a prefix for logs where `name` may be null
         """
         if self.name is not None:
             return f"AzureContainerInstanceJob {self.name!r}"
         else:
             return "AzureContainerInstanceJob"
 
     @staticmethod
-    def _provisioning_succeeded(container_group: ContainerGroup) -> bool:
+    def _provisioning_succeeded(container_group: Union[ContainerGroup, None]) -> bool:
         """
         Determines whether ACI container group provisioning was successful.
 
         Args:
             container_group: a container group returned by the Azure SDK.
 
         Returns:
```

### Comparing `prefect_azure-0.3.9/prefect_azure/cosmos_db.py` & `prefect_azure-0.4.0rc1/prefect_azure/cosmos_db.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.9/prefect_azure/credentials.py` & `prefect_azure-0.4.0rc1/prefect_azure/credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,15 @@
 import functools
 from typing import TYPE_CHECKING, Any, Dict, Optional
 
 from azure.identity import ClientSecretCredential, DefaultAzureCredential
 from azure.identity.aio import DefaultAzureCredential as ADefaultAzureCredential
 from azure.mgmt.containerinstance import ContainerInstanceManagementClient
 from azure.mgmt.resource import ResourceManagementClient
-from pydantic import VERSION as PYDANTIC_VERSION
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field, SecretStr, root_validator
-else:
-    from pydantic import Field, SecretStr, root_validator
+from pydantic import Field, SecretStr, model_validator
 
 try:
     from azure.cosmos import CosmosClient
 
     if TYPE_CHECKING:
         from azure.cosmos import ContainerProxy, DatabaseProxy
 except ModuleNotFoundError:
@@ -115,15 +110,16 @@
         description=(
             "The URL for your Azure storage account. If provided, the account "
             "URL will be used to authenticate with the discovered default "
             "Azure credentials."
         ),
     )
 
-    @root_validator
+    @model_validator(mode="before")
+    @classmethod
     def check_connection_string_or_account_url(
         cls, values: Dict[str, Any]
     ) -> Dict[str, Any]:
         """
         Checks that either a connection string or account URL is provided, not both.
         """
         has_account_url = values.get("account_url") is not None
@@ -514,15 +510,16 @@
         title="Additional Credential Keyword Arguments",
         description=(
             "Additional keyword arguments to pass to "
             "`ClientSecretCredential` or `DefaultAzureCredential`."
         ),
     )
 
-    @root_validator
+    @model_validator(mode="before")
+    @classmethod
     def validate_credential_kwargs(cls, values):
         """
         Validates that if any of `client_id`, `tenant_id`, or `client_secret` are
         provided, all must be provided.
         """
         auth_args = ("client_id", "tenant_id", "client_secret")
         has_any = any(values.get(key) is not None for key in auth_args)
```

### Comparing `prefect_azure-0.3.9/prefect_azure/deployments/steps.py` & `prefect_azure-0.4.0rc1/prefect_azure/deployments/steps.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.9/prefect_azure/ml_datastore.py` & `prefect_azure-0.4.0rc1/prefect_azure/ml_datastore.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.9/prefect_azure.egg-info/PKG-INFO` & `prefect_azure-0.4.0rc1/prefect_azure.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: prefect-azure
-Version: 0.3.9
+Version: 0.4.0rc1
 Summary: Prefect integrations with Microsoft Azure services
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-azure
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
 Requires-Dist: aiohttp
 Requires-Dist: azure_identity>=1.10
 Requires-Dist: azure_mgmt_containerinstance>=10.0
 Requires-Dist: azure-mgmt-resource>=21.2
-Requires-Dist: prefect>=2.14.10
+Requires-Dist: prefect>=3.0.0rc1
+Requires-Dist: setuptools
 Provides-Extra: blob-storage
 Requires-Dist: azure-storage-blob; extra == "blob-storage"
 Provides-Extra: cosmos-db
 Requires-Dist: azure-cosmos; extra == "cosmos-db"
 Provides-Extra: ml-datastore
 Requires-Dist: azureml-core; extra == "ml-datastore"
 Provides-Extra: all-extras
@@ -42,15 +42,14 @@
 Requires-Dist: azureml-core; extra == "dev"
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
```

### Comparing `prefect_azure-0.3.9/prefect_azure.egg-info/SOURCES.txt` & `prefect_azure-0.4.0rc1/prefect_azure.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 prefect_azure.egg-info/requires.txt
 prefect_azure.egg-info/top_level.txt
 prefect_azure/deployments/__init__.py
 prefect_azure/deployments/steps.py
 prefect_azure/workers/__init__.py
 prefect_azure/workers/container_instance.py
 tests/conftest.py
-tests/test_aci_infrastructure.py
+tests/test_aci_credentials.py
 tests/test_aci_worker.py
 tests/test_blob_storage.py
 tests/test_block_standards.py
 tests/test_cosmos_db.py
 tests/test_credentials.py
 tests/test_ml_datastore.py
 tests/test_version.py
```

### Comparing `prefect_azure-0.3.9/pyproject.toml` & `prefect_azure-0.4.0rc1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,63 +2,56 @@
 requires = ["setuptools>=45", "wheel", "setuptools_scm>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prefect-azure"
 description = "Prefect integrations with Microsoft Azure services"
 readme = "README.md"
-requires-python = ">=3.8"
-license = {text = "Apache License 2.0"}
+requires-python = ">=3.9"
+license = { text = "Apache License 2.0" }
 keywords = ["prefect"]
-authors = [
-  {name = "Prefect Technologies, Inc.", email = "help@prefect.io"}
-]
+authors = [{ name = "Prefect Technologies, Inc.", email = "help@prefect.io" }]
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
   "aiohttp",
   "azure_identity>=1.10",
   "azure_mgmt_containerinstance>=10.0",
   "azure-mgmt-resource>=21.2",
-  "prefect>=2.14.10",
+  "prefect>=3.0.0rc1",
+  "setuptools",                                           #required in 3.12 to get pkg_resources (used by azureml.core)
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 blob_storage = ["azure-storage-blob"]
 cosmos_db = ["azure-cosmos"]
 ml_datastore = ["azureml-core"]
-all_extras = [
-  "azure-cosmos",
-  "azure-storage-blob",
-  "azureml-core",
-]
+all_extras = ["azure-cosmos", "azure-storage-blob", "azureml-core"]
 dev = [
   "aiohttp",
   "azure-cosmos",
   "azure-storage-blob",
   "azureml-core",
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
@@ -68,15 +61,15 @@
 
 [project.entry-points."prefect.collections"]
 prefect_azure = "prefect_azure"
 
 [tool.setuptools_scm]
 version_file = "prefect_azure/_version.py"
 root = "../../.."
-tag_regex = "^prefect-azure-(?P<version>\\d+\\.\\d+\\.\\d+)$"
+tag_regex = "^prefect-azure-(?P<version>\\d+\\.\\d+\\.\\d+(?:[a-zA-Z0-9]+(?:\\.[a-zA-Z0-9]+)*)?)$"
 fallback_version = "0.0.0"
 git_describe_command = 'git describe --dirty --tags --long --match "prefect-azure-*[0-9]*"'
 
 [tool.interrogate]
 ignore-init-module = true
 ignore_init_method = true
 exclude = ["prefect_azure/_version.py", "tests"]
@@ -87,8 +80,8 @@
 omit = ["tests/*", "prefect_azure/_version.py"]
 
 [tool.coverage.report]
 fail_under = 80
 show_missing = true
 
 [tool.pytest.ini_options]
-asyncio_mode = "auto"
+asyncio_mode = "auto"
```

### Comparing `prefect_azure-0.3.9/tests/conftest.py` & `prefect_azure-0.4.0rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.9/tests/deployments/test_steps.py` & `prefect_azure-0.4.0rc1/tests/deployments/test_steps.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.9/tests/test_aci_worker.py` & `prefect_azure-0.4.0rc1/tests/test_aci_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,37 @@
 import asyncio
 import uuid
 from typing import Dict, List, Tuple, Union
 from unittest.mock import MagicMock, Mock
 
 import dateutil.parser
+import prefect_azure.container_instance
 import pytest
 from anyio.abc import TaskStatus
 from azure.core.exceptions import HttpResponseError, ResourceNotFoundError
 from azure.identity import ClientSecretCredential
 from azure.mgmt.resource import ResourceManagementClient
-from pydantic import VERSION as PYDANTIC_VERSION
-
-from prefect.client.schemas import FlowRun
-from prefect.exceptions import InfrastructureNotFound
-from prefect.infrastructure.container import DockerRegistry
-from prefect.server.schemas.core import Flow
-from prefect.settings import get_current_settings
-from prefect.testing.utilities import AsyncMock
-from prefect.utilities.dockerutils import get_prefect_image_name
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import SecretStr
-else:
-    from pydantic import SecretStr
-
-import prefect_azure.container_instance
 from prefect_azure import AzureContainerInstanceCredentials
 from prefect_azure.container_instance import ACRManagedIdentity
 from prefect_azure.workers.container_instance import (
     AzureContainerJobConfiguration,
     AzureContainerVariables,  # noqa
     AzureContainerWorker,
     AzureContainerWorkerResult,
     ContainerGroupProvisioningState,
     ContainerRunState,
 )
+from pydantic import SecretStr
+
+from prefect.client.schemas import FlowRun
+from prefect.exceptions import InfrastructureNotFound
+from prefect.server.schemas.core import Flow
+from prefect.settings import get_current_settings
+from prefect.testing.utilities import AsyncMock
+from prefect.utilities.dockerutils import get_prefect_image_name
 
 
 # Helper functions
 def credential_values(
     credentials: AzureContainerInstanceCredentials,
 ) -> Tuple[str, str, str]:
     """
@@ -104,15 +97,15 @@
     for k, v in overrides.items():
         values = {**values, k: v}
 
     container_instance_variables = AzureContainerVariables(**values)
 
     json_config = {
         "job_configuration": AzureContainerJobConfiguration.json_template(),
-        "variables": container_instance_variables.dict(),
+        "variables": container_instance_variables.model_dump(),
     }
 
     container_instance_configuration = (
         await AzureContainerJobConfiguration.from_template_and_values(
             json_config, values
         )
     )
@@ -341,15 +334,15 @@
     monkeypatch.setattr(
         prefect_azure.credentials,
         "ResourceManagementClient",
         mock_resource_client_constructor,
     )
 
     subscription_id = "test_subscription"
-    job_configuration.subscription_id = SecretStr(value=subscription_id)
+    job_configuration.subscription_id = SecretStr(subscription_id)
 
     async with AzureContainerWorker(work_pool_name="test_pool") as aci_worker:
         # Using mock Azure clients to avoid making real calls to Azure
         # during testing means that the client will raise an exception
         # unless we mock multiple client responses. Since we're only
         # mocking what's needed for this test, we expect the worker to
         # raise an exception when it tries to proceed further.
@@ -538,14 +531,38 @@
         )
 
         await aci_worker.run(worker_flow_run, job_configuration)
 
     mock_aci_client.container_groups.begin_delete.assert_called_once()
 
 
+async def test_stop_after_group_creation_success(
+    mock_prefect_client,
+    worker_flow_run,
+    job_configuration,
+    mock_aci_client,
+    monkeypatch,
+    running_worker_container_group,
+):
+    async with AzureContainerWorker(work_pool_name="test_pool") as aci_worker:
+        # if provisioning was successful, and keep_container_group is enabled,
+        # the container group should be stopped instead of deleted
+        monkeypatch.setattr(
+            aci_worker,
+            "_wait_for_task_container_start",
+            Mock(return_value=running_worker_container_group),
+        )
+
+        job_configuration.keep_container_group = True
+
+        await aci_worker.run(worker_flow_run, job_configuration)
+
+    mock_aci_client.container_groups.stop.assert_called_once()
+
+
 async def test_delete_after_after_exception(
     mock_prefect_client,
     worker_flow_run,
     job_configuration,
     mock_aci_client,
     mock_resource_client,
     monkeypatch,
@@ -851,40 +868,14 @@
         "name": "PREFECT_API_KEY",
         "secureValue": "my-api-key",
     }
 
     assert api_key_entry == expected
 
 
-def test_add_docker_registry_credentials(
-    raw_job_configuration, worker_flow_run, mock_aci_client, monkeypatch
-):
-    registry = DockerRegistry(
-        username="username",
-        password="password",
-        registry_url="https://myregistry.dockerhub.com",
-    )
-
-    raw_job_configuration.image_registry = registry
-    raw_job_configuration.prepare_for_flow_run(worker_flow_run)
-
-    container_group = raw_job_configuration.arm_template["resources"][0]
-    image_registry_credentials = container_group["properties"][
-        "imageRegistryCredentials"
-    ]
-
-    assert len(image_registry_credentials) == 1
-    assert image_registry_credentials[0]["server"] == registry.registry_url
-    assert image_registry_credentials[0]["username"] == registry.username
-    assert (
-        image_registry_credentials[0]["password"]
-        == registry.password.get_secret_value()
-    )
-
-
 def test_add_acr_registry_identity(
     raw_job_configuration, worker_flow_run, mock_aci_client, monkeypatch
 ):
     registry = ACRManagedIdentity(
         registry_url="https://myregistry.azurecr.io",
         identity="my-identity",
     )
@@ -961,15 +952,15 @@
 
 async def test_image_populated_in_template_when_not_provided(worker_flow_run):
     config = await AzureContainerJobConfiguration.from_template_and_values(
         base_job_template=AzureContainerWorker.get_default_base_job_template(),
         values=AzureContainerVariables(
             subscription_id="my-subscription-id",
             resource_group_name="my-resource-group",
-        ).dict(exclude_unset=True),
+        ).model_dump(exclude_unset=True),
     )
     config.prepare_for_flow_run(worker_flow_run)
 
     assert config.image == get_prefect_image_name()
     assert (
         config.arm_template["resources"][0]["properties"]["containers"][0][
             "properties"
```

### Comparing `prefect_azure-0.3.9/tests/test_blob_storage.py` & `prefect_azure-0.4.0rc1/tests/test_blob_storage.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.9/tests/test_block_standards.py` & `prefect_azure-0.4.0rc1/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.9/tests/test_cosmos_db.py` & `prefect_azure-0.4.0rc1/tests/test_cosmos_db.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.9/tests/test_credentials.py` & `prefect_azure-0.4.0rc1/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_azure-0.3.9/tests/test_ml_datastore.py` & `prefect_azure-0.4.0rc1/tests/test_ml_datastore.py`

 * *Files identical despite different names*

