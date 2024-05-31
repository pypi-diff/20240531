# Comparing `tmp/prefect_ray-0.3.6.tar.gz` & `tmp/prefect_ray-0.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_ray-0.3.6.tar", last modified: Thu May 16 20:58:40 2024, max compression
+gzip compressed data, was "prefect_ray-0.4.0rc1.tar", last modified: Fri May 31 20:49:42 2024, max compression
```

## Comparing `prefect_ray-0.3.6.tar` & `prefect_ray-0.4.0rc1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:40.762359 prefect_ray-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-05-16 20:58:40.758359 prefect_ray-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:40.754359 prefect_ray-0.3.6/prefect_ray/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/prefect_ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 20:58:40.000000 prefect_ray-0.3.6/prefect_ray/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/prefect_ray/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     8840 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/prefect_ray/task_runners.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:40.758359 prefect_ray-0.3.6/prefect_ray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-05-16 20:58:40.000000 prefect_ray-0.3.6/prefect_ray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-16 20:58:40.000000 prefect_ray-0.3.6/prefect_ray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:58:40.000000 prefect_ray-0.3.6/prefect_ray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-16 20:58:40.000000 prefect_ray-0.3.6/prefect_ray.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-16 20:58:40.000000 prefect_ray-0.3.6/prefect_ray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 20:58:40.000000 prefect_ray-0.3.6/prefect_ray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:58:40.762359 prefect_ray-0.3.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:40.758359 prefect_ray-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    10949 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/tests/test_task_runners.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:42.523760 prefect_ray-0.4.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-31 20:49:31.000000 prefect_ray-0.4.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-31 20:49:31.000000 prefect_ray-0.4.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-05-31 20:49:42.523760 prefect_ray-0.4.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-05-31 20:49:31.000000 prefect_ray-0.4.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:42.519760 prefect_ray-0.4.0rc1/prefect_ray/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-31 20:49:31.000000 prefect_ray-0.4.0rc1/prefect_ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-31 20:49:42.000000 prefect_ray-0.4.0rc1/prefect_ray/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-31 20:49:31.000000 prefect_ray-0.4.0rc1/prefect_ray/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10346 2024-05-31 20:49:31.000000 prefect_ray-0.4.0rc1/prefect_ray/task_runners.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:42.519760 prefect_ray-0.4.0rc1/prefect_ray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-05-31 20:49:42.000000 prefect_ray-0.4.0rc1/prefect_ray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-31 20:49:42.000000 prefect_ray-0.4.0rc1/prefect_ray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:49:42.000000 prefect_ray-0.4.0rc1/prefect_ray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-31 20:49:42.000000 prefect_ray-0.4.0rc1/prefect_ray.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-31 20:49:42.000000 prefect_ray-0.4.0rc1/prefect_ray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-31 20:49:42.000000 prefect_ray-0.4.0rc1/prefect_ray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-31 20:49:31.000000 prefect_ray-0.4.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:49:42.523760 prefect_ray-0.4.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:42.519760 prefect_ray-0.4.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:31.000000 prefect_ray-0.4.0rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-31 20:49:31.000000 prefect_ray-0.4.0rc1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-31 20:49:31.000000 prefect_ray-0.4.0rc1/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-31 20:49:31.000000 prefect_ray-0.4.0rc1/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12809 2024-05-31 20:49:31.000000 prefect_ray-0.4.0rc1/tests/test_task_runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-31 20:49:31.000000 prefect_ray-0.4.0rc1/tests/test_version.py
```

### Comparing `prefect_ray-0.3.6/LICENSE` & `prefect_ray-0.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_ray-0.3.6/PKG-INFO` & `prefect_ray-0.4.0rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 Metadata-Version: 2.1
 Name: prefect-ray
-Version: 0.3.6
+Version: 0.4.0rc1
 Summary: Prefect integrations with the Ray execution framework.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-ray
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
 Requires-Dist: ray[default]>=2.0.0
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
 Requires-Dist: pytest-asyncio!=0.22.0,<0.23.0,>=0.18.2; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
@@ -57,15 +55,15 @@
 
 Provides a `RayTaskRunner` that enables Prefect flows to run tasks execute tasks in parallel using Ray.
 
 ## Getting Started
 
 ### Python setup
 
-Requires an installation of Python 3.8 or newer.
+Requires an installation of Python 3.9 or newer.
 
 We recommend using a Python virtual environment manager such as pipenv, conda, or virtualenv.
 
 These tasks are designed to work with Prefect 2.0+. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Installation
 
@@ -75,15 +73,15 @@
 pip install prefect-ray
 ```
 
 Users running Apple Silicon (such as M1 macs) should check out the Ray docs [here](https://docs.ray.io/en/master/ray-overview/installation.html#m1-mac-apple-silicon-support) for more details.
 
 ## Running tasks on Ray
 
-The `RayTaskRunner` is a [Prefect task runner](https://docs.prefect.io/concepts/task-runners/) that submits tasks to [Ray](https://www.ray.io/) for parallel execution. 
+The `RayTaskRunner` is a [Prefect task runner](https://docs.prefect.io/concepts/task-runners/) that submits tasks to [Ray](https://www.ray.io/) for parallel execution.
 
 By default, a temporary Ray instance is created for the duration of the flow run.
 
 For example, this flow counts to 3 in parallel.
 
 ```python
 import time
@@ -129,47 +127,47 @@
 
 ```python
 from prefect import flow
 from prefect_ray.task_runners import RayTaskRunner
 
 @flow(task_runner=RayTaskRunner())
 def my_flow():
-    ... 
+    ...
 ```
 
 This flow uses the `RayTaskRunner` configured to access an existing Ray instance at `ray://192.0.2.255:8786`.
 
 ```python
 from prefect import flow
 from prefect_ray.task_runners import RayTaskRunner
 
 @flow(task_runner=RayTaskRunner(address="ray://192.0.2.255:8786"))
 def my_flow():
-    ... 
+    ...
 ```
 
 `RayTaskRunner` accepts the following optional parameters:
 
-| Parameter | Description |
-| --- | --- |
-| address | Address of a currently running Ray instance, starting with the [ray://](https://docs.ray.io/en/master/cluster/ray-client.html) URI. |
-| init_kwargs | Additional kwargs to use when calling `ray.init`. |
+| Parameter   | Description                                                                                                                         |
+| ----------- | ----------------------------------------------------------------------------------------------------------------------------------- |
+| address     | Address of a currently running Ray instance, starting with the [ray://](https://docs.ray.io/en/master/cluster/ray-client.html) URI. |
+| init_kwargs | Additional kwargs to use when calling `ray.init`.                                                                                   |
 
 Note that Ray Client uses the [ray://](https://docs.ray.io/en/master/cluster/ray-client.html) URI to indicate the address of a Ray instance. If you don't provide the `address` of a Ray instance, Prefect creates a temporary instance automatically.
 
 !!! warning "Ray environment limitations"
     Ray support for non-x86/64 architectures such as ARM/M1 processors with installation from `pip` alone and will be skipped during installation of Prefect. It is possible to manually install the blocking component with `conda`. See the [Ray documentation](https://docs.ray.io/en/latest/ray-overview/installation.html#m1-mac-apple-silicon-support) for instructions.
 
     See the [Ray installation documentation](https://docs.ray.io/en/latest/ray-overview/installation.html) for further compatibility information.
 
 ## Running tasks on a Ray remote cluster
 
 When using the `RayTaskRunner` with a remote Ray cluster, you may run into issues that are not seen when using a local Ray instance. To resolve these issues, we recommend taking the following steps when working with a remote Ray cluster:
 
-1. By default, Prefect will not persist any data to the filesystem of the remote ray worker. However, if you want to take advantage of Prefect's caching ability, you will need to configure a remote result storage to persist results across task runs. 
+1. By default, Prefect will not persist any data to the filesystem of the remote ray worker. However, if you want to take advantage of Prefect's caching ability, you will need to configure a remote result storage to persist results across task runs.
 
 We recommend using the [Prefect UI to configure a storage block](https://docs.prefect.io/concepts/blocks/) to use for remote results storage.
 
 Here's an example of a flow that uses caching and remote result storage:
 ```python
 from typing import List
 
@@ -205,15 +203,15 @@
 ```
 
 2. If you get an error stating that the module 'prefect' cannot be found, ensure `prefect` is installed on the remote cluster, with:
 ```bash
 pip install prefect
 ```
 
-3. If you get an error with a message similar to "File system created with scheme 's3' could not be created", ensure the required Python modules are installed on **both local and remote machines**. The required prerequisite modules can be found in the [Prefect documentation](https://docs.prefect.io/guides/deployment/storage-guide). For example, if using S3 for the remote storage:
+3. If you get an error with a message similar to "File system created with scheme 's3' could not be created", ensure the required Python modules are installed on **both local and remote machines**. For example, if using S3 for the remote storage:
 ```bash
 pip install s3fs
 ```
 
 4. If you are seeing timeout or other connection errors, double check the address provided to the `RayTaskRunner`. The address should look similar to: `address='ray://<head_node_ip_address>:10001'`:
 ```bash
 RayTaskRunner(address="ray://1.23.199.255:10001")
```

### Comparing `prefect_ray-0.3.6/README.md` & `prefect_ray-0.4.0rc1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 Provides a `RayTaskRunner` that enables Prefect flows to run tasks execute tasks in parallel using Ray.
 
 ## Getting Started
 
 ### Python setup
 
-Requires an installation of Python 3.8 or newer.
+Requires an installation of Python 3.9 or newer.
 
 We recommend using a Python virtual environment manager such as pipenv, conda, or virtualenv.
 
 These tasks are designed to work with Prefect 2.0+. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Installation
 
@@ -34,15 +34,15 @@
 pip install prefect-ray
 ```
 
 Users running Apple Silicon (such as M1 macs) should check out the Ray docs [here](https://docs.ray.io/en/master/ray-overview/installation.html#m1-mac-apple-silicon-support) for more details.
 
 ## Running tasks on Ray
 
-The `RayTaskRunner` is a [Prefect task runner](https://docs.prefect.io/concepts/task-runners/) that submits tasks to [Ray](https://www.ray.io/) for parallel execution. 
+The `RayTaskRunner` is a [Prefect task runner](https://docs.prefect.io/concepts/task-runners/) that submits tasks to [Ray](https://www.ray.io/) for parallel execution.
 
 By default, a temporary Ray instance is created for the duration of the flow run.
 
 For example, this flow counts to 3 in parallel.
 
 ```python
 import time
@@ -88,47 +88,47 @@
 
 ```python
 from prefect import flow
 from prefect_ray.task_runners import RayTaskRunner
 
 @flow(task_runner=RayTaskRunner())
 def my_flow():
-    ... 
+    ...
 ```
 
 This flow uses the `RayTaskRunner` configured to access an existing Ray instance at `ray://192.0.2.255:8786`.
 
 ```python
 from prefect import flow
 from prefect_ray.task_runners import RayTaskRunner
 
 @flow(task_runner=RayTaskRunner(address="ray://192.0.2.255:8786"))
 def my_flow():
-    ... 
+    ...
 ```
 
 `RayTaskRunner` accepts the following optional parameters:
 
-| Parameter | Description |
-| --- | --- |
-| address | Address of a currently running Ray instance, starting with the [ray://](https://docs.ray.io/en/master/cluster/ray-client.html) URI. |
-| init_kwargs | Additional kwargs to use when calling `ray.init`. |
+| Parameter   | Description                                                                                                                         |
+| ----------- | ----------------------------------------------------------------------------------------------------------------------------------- |
+| address     | Address of a currently running Ray instance, starting with the [ray://](https://docs.ray.io/en/master/cluster/ray-client.html) URI. |
+| init_kwargs | Additional kwargs to use when calling `ray.init`.                                                                                   |
 
 Note that Ray Client uses the [ray://](https://docs.ray.io/en/master/cluster/ray-client.html) URI to indicate the address of a Ray instance. If you don't provide the `address` of a Ray instance, Prefect creates a temporary instance automatically.
 
 !!! warning "Ray environment limitations"
     Ray support for non-x86/64 architectures such as ARM/M1 processors with installation from `pip` alone and will be skipped during installation of Prefect. It is possible to manually install the blocking component with `conda`. See the [Ray documentation](https://docs.ray.io/en/latest/ray-overview/installation.html#m1-mac-apple-silicon-support) for instructions.
 
     See the [Ray installation documentation](https://docs.ray.io/en/latest/ray-overview/installation.html) for further compatibility information.
 
 ## Running tasks on a Ray remote cluster
 
 When using the `RayTaskRunner` with a remote Ray cluster, you may run into issues that are not seen when using a local Ray instance. To resolve these issues, we recommend taking the following steps when working with a remote Ray cluster:
 
-1. By default, Prefect will not persist any data to the filesystem of the remote ray worker. However, if you want to take advantage of Prefect's caching ability, you will need to configure a remote result storage to persist results across task runs. 
+1. By default, Prefect will not persist any data to the filesystem of the remote ray worker. However, if you want to take advantage of Prefect's caching ability, you will need to configure a remote result storage to persist results across task runs.
 
 We recommend using the [Prefect UI to configure a storage block](https://docs.prefect.io/concepts/blocks/) to use for remote results storage.
 
 Here's an example of a flow that uses caching and remote result storage:
 ```python
 from typing import List
 
@@ -164,15 +164,15 @@
 ```
 
 2. If you get an error stating that the module 'prefect' cannot be found, ensure `prefect` is installed on the remote cluster, with:
 ```bash
 pip install prefect
 ```
 
-3. If you get an error with a message similar to "File system created with scheme 's3' could not be created", ensure the required Python modules are installed on **both local and remote machines**. The required prerequisite modules can be found in the [Prefect documentation](https://docs.prefect.io/guides/deployment/storage-guide). For example, if using S3 for the remote storage:
+3. If you get an error with a message similar to "File system created with scheme 's3' could not be created", ensure the required Python modules are installed on **both local and remote machines**. For example, if using S3 for the remote storage:
 ```bash
 pip install s3fs
 ```
 
 4. If you are seeing timeout or other connection errors, double check the address provided to the `RayTaskRunner`. The address should look similar to: `address='ray://<head_node_ip_address>:10001'`:
 ```bash
 RayTaskRunner(address="ray://1.23.199.255:10001")
@@ -195,8 +195,8 @@
 
 
 @flow(task_runner=RayTaskRunner())
 def my_flow():
     # equivalent to setting @ray.remote(num_cpus=4, num_gpus=2)
     with remote_options(num_cpus=4, num_gpus=2):
         process.submit(42)
-```
+```
```

### Comparing `prefect_ray-0.3.6/prefect_ray/context.py` & `prefect_ray-0.4.0rc1/prefect_ray/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 """
 Contexts to manage Ray clusters and tasks.
 """
 
 from contextlib import contextmanager
-from typing import Any, Dict
+from typing import Any, Dict, Generator
 
-from pydantic import VERSION as PYDANTIC_VERSION
+from pydantic import Field
 
 from prefect.context import ContextModel, ContextVar
 
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field
-else:
-    from pydantic import Field
-
 
 class RemoteOptionsContext(ContextModel):
     """
     The context for Ray remote_options management.
 
     Attributes:
         current_remote_options: A set of current remote_options in the context.
     """
 
+    __var__: ContextVar = ContextVar("remote_options")
     current_remote_options: Dict[str, Any] = Field(default_factory=dict)
 
     @classmethod
     def get(cls) -> "RemoteOptionsContext":
         """
         Return an empty `RemoteOptionsContext`
         instead of `None` if no context exists.
         """
         return cls.__var__.get(RemoteOptionsContext())
 
     __var__ = ContextVar("remote_options")
 
 
 @contextmanager
-def remote_options(**new_remote_options: Dict[str, Any]) -> Dict[str, Any]:
+def remote_options(
+    **new_remote_options: Dict[str, Any],
+) -> Generator[None, Dict[str, Any], None]:
     """
     Context manager to add keyword arguments to Ray `@remote` calls
     for task runs. If contexts are nested, new options are merged with options
     in the outer context. If a key is present in both, the new option will be used.
 
     Yields:
         The current set of remote options.
```

### Comparing `prefect_ray-0.3.6/prefect_ray/task_runners.py` & `prefect_ray-0.4.0rc1/prefect_ray/task_runners.py`

 * *Files 23% similar despite different names*

```diff
@@ -67,31 +67,74 @@
     #1
     #5
     #8
     #9
     ```
 """
 
-from contextlib import AsyncExitStack
-from typing import Awaitable, Callable, Dict, Optional
-from uuid import UUID
+import asyncio
+import inspect
+from typing import Any, Dict, Iterable, Optional, Set
+from uuid import UUID, uuid4
 
-import anyio
 import ray
-from ray.exceptions import RayTaskError
+from ray.exceptions import GetTimeoutError
 
-from prefect.futures import PrefectFuture
+from prefect.client.schemas.objects import TaskRunInput
+from prefect.context import serialize_context
+from prefect.futures import PrefectFuture, PrefectWrappedFuture
 from prefect.states import State, exception_to_crashed_state
-from prefect.task_runners import BaseTaskRunner, R, TaskConcurrencyType
-from prefect.utilities.asyncutils import sync_compatible
+from prefect.task_engine import run_task_async, run_task_sync
+from prefect.task_runners import TaskRunner
+from prefect.tasks import Task
+from prefect.utilities.asyncutils import run_coro_as_sync
 from prefect.utilities.collections import visit_collection
 from prefect_ray.context import RemoteOptionsContext
 
 
-class RayTaskRunner(BaseTaskRunner):
+class PrefectRayFuture(PrefectWrappedFuture[ray.ObjectRef]):
+    def wait(self, timeout: Optional[float] = None) -> None:
+        try:
+            result = ray.get(self.wrapped_future, timeout=timeout)
+        except GetTimeoutError:
+            return
+        except Exception as exc:
+            result = run_coro_as_sync(exception_to_crashed_state(exc))
+        if isinstance(result, State):
+            self._final_state = result
+
+    def result(
+        self,
+        timeout: Optional[float] = None,
+        raise_on_failure: bool = True,
+    ) -> Any:
+        if not self._final_state:
+            try:
+                object_ref_result = ray.get(self.wrapped_future, timeout=timeout)
+            except GetTimeoutError as exc:
+                raise TimeoutError(
+                    f"Task run {self.task_run_id} did not complete within {timeout} seconds"
+                ) from exc
+
+            if isinstance(object_ref_result, State):
+                self._final_state = object_ref_result
+            else:
+                return object_ref_result
+
+        _result = self._final_state.result(
+            raise_on_failure=raise_on_failure, fetch=True
+        )
+        # state.result is a `sync_compatible` function that may or may not return an awaitable
+        # depending on whether the parent frame is sync or not
+        if inspect.isawaitable(_result):
+            _result = run_coro_as_sync(_result)
+        return _result
+
+
+class RayTaskRunner(TaskRunner[PrefectRayFuture]):
     """
     A parallel task_runner that submits tasks to `ray`.
     By default, a temporary Ray cluster is created for the duration of the flow run.
     Alternatively, if you already have a `ray` instance running, you can provide
     the connection URL via the `address` kwarg.
     Args:
         address (string, optional): Address of a currently running `ray` instance; if
@@ -111,180 +154,184 @@
         ```python
         RayTaskRunner(address="ray://192.0.2.255:8786")
         ```
     """
 
     def __init__(
         self,
-        address: str = None,
-        init_kwargs: dict = None,
+        address: Optional[str] = None,
+        init_kwargs: Optional[Dict] = None,
     ):
         # Store settings
         self.address = address
         self.init_kwargs = init_kwargs.copy() if init_kwargs else {}
 
         self.init_kwargs.setdefault("namespace", "prefect")
 
         # Runtime attributes
-        self._ray_refs: Dict[str, "ray.ObjectRef"] = {}
+        self._ray_context = None
 
         super().__init__()
 
     def duplicate(self):
         """
         Return a new instance of with the same settings as this one.
         """
         return type(self)(address=self.address, init_kwargs=self.init_kwargs)
 
     def __eq__(self, other: object) -> bool:
         """
         Check if an instance has the same settings as this task runner.
         """
-        if type(self) == type(other):
+        if isinstance(other, RayTaskRunner):
             return (
                 self.address == other.address and self.init_kwargs == other.init_kwargs
             )
         else:
-            return NotImplemented
-
-    @property
-    def concurrency_type(self) -> TaskConcurrencyType:
-        return TaskConcurrencyType.PARALLEL
+            return False
 
-    async def submit(
+    def submit(
         self,
-        key: UUID,
-        call: Callable[..., Awaitable[State[R]]],
-    ) -> None:
+        task: Task,
+        parameters: Dict[str, Any],
+        wait_for: Optional[Iterable[PrefectFuture]] = None,
+        dependencies: Optional[Dict[str, Set[TaskRunInput]]] = None,
+    ) -> PrefectRayFuture:
         if not self._started:
             raise RuntimeError(
                 "The task runner must be started before submitting work."
             )
 
-        call_kwargs, upstream_ray_obj_refs = self._exchange_prefect_for_ray_futures(
-            call.keywords
+        parameters, upstream_ray_obj_refs = self._exchange_prefect_for_ray_futures(
+            parameters
         )
+        task_run_id = uuid4()
+        context = serialize_context()
 
         remote_options = RemoteOptionsContext.get().current_remote_options
-        # Ray does not support the submission of async functions and we must create a
-        # sync entrypoint
         if remote_options:
             ray_decorator = ray.remote(**remote_options)
         else:
             ray_decorator = ray.remote
 
-        self._ray_refs[key] = (
+        object_ref = (
             ray_decorator(self._run_prefect_task)
-            .options(name=call.keywords["task_run"].name)
-            .remote(sync_compatible(call.func), *upstream_ray_obj_refs, **call_kwargs)
+            .options(name=task.name)
+            .remote(
+                *upstream_ray_obj_refs,
+                task=task,
+                task_run_id=task_run_id,
+                parameters=parameters,
+                wait_for=wait_for,
+                dependencies=dependencies,
+                context=context,
+            )
         )
+        return PrefectRayFuture(task_run_id=task_run_id, wrapped_future=object_ref)
 
     def _exchange_prefect_for_ray_futures(self, kwargs_prefect_futures):
         """Exchanges Prefect futures for Ray futures."""
 
         upstream_ray_obj_refs = []
 
         def exchange_prefect_for_ray_future(expr):
             """Exchanges Prefect future for Ray future."""
-            if isinstance(expr, PrefectFuture):
-                ray_future = self._ray_refs.get(expr.key)
-                if ray_future is not None:
-                    upstream_ray_obj_refs.append(ray_future)
-                    return ray_future
+            if isinstance(expr, PrefectRayFuture):
+                ray_future = expr.wrapped_future
+                upstream_ray_obj_refs.append(ray_future)
+                return ray_future
             return expr
 
         kwargs_ray_futures = visit_collection(
             kwargs_prefect_futures,
             visit_fn=exchange_prefect_for_ray_future,
             return_data=True,
         )
 
         return kwargs_ray_futures, upstream_ray_obj_refs
 
     @staticmethod
-    def _run_prefect_task(func, *upstream_ray_obj_refs, **kwargs):
+    def _run_prefect_task(
+        *upstream_ray_obj_refs,
+        task: Task,
+        task_run_id: UUID,
+        context: Dict[str, Any],
+        parameters: Dict[str, Any],
+        wait_for: Optional[Iterable[PrefectFuture]] = None,
+        dependencies: Optional[Dict[str, Set[TaskRunInput]]] = None,
+    ):
         """Resolves Ray futures before calling the actual Prefect task function.
 
         Passing upstream_ray_obj_refs directly as args enables Ray to wait for
         upstream tasks before running this remote function.
         This variable is otherwise unused as the ray object refs are also
-        contained in kwargs.
+        contained in parameters.
         """
 
+        # Resolve Ray futures to ensure that the task function receives the actual values
         def resolve_ray_future(expr):
             """Resolves Ray future."""
             if isinstance(expr, ray.ObjectRef):
                 return ray.get(expr)
             return expr
 
-        kwargs = visit_collection(kwargs, visit_fn=resolve_ray_future, return_data=True)
+        parameters = visit_collection(
+            parameters, visit_fn=resolve_ray_future, return_data=True
+        )
 
-        return func(**kwargs)
+        run_task_kwargs = {
+            "task": task,
+            "task_run_id": task_run_id,
+            "parameters": parameters,
+            "wait_for": wait_for,
+            "dependencies": dependencies,
+            "context": context,
+            "return_type": "state",
+        }
 
-    async def wait(self, key: UUID, timeout: float = None) -> Optional[State]:
-        ref = self._get_ray_ref(key)
+        # Ray does not support the submission of async functions and we must create a
+        # sync entrypoint
+        if task.isasync:
+            return asyncio.run(run_task_async(**run_task_kwargs))
+        else:
+            return run_task_sync(**run_task_kwargs)
 
-        result = None
+    def __enter__(self):
+        super().__enter__()
 
-        with anyio.move_on_after(timeout):
-            # We await the reference directly instead of using `ray.get` so we can
-            # avoid blocking the event loop
-            try:
-                result = await ref
-            except RayTaskError as exc:
-                # unwrap the original exception that caused task failure, except for
-                # KeyboardInterrupt, which unwraps as TaskCancelledError
-                result = await exception_to_crashed_state(exc.cause)
-            except BaseException as exc:
-                result = await exception_to_crashed_state(exc)
-
-        return result
-
-    async def _start(self, exit_stack: AsyncExitStack):
-        """
-        Start the task runner and prep for context exit.
-
-        - Creates a cluster if an external address is not set.
-        - Creates a client to connect to the cluster.
-        - Pushes a call to wait for all running futures to complete on exit.
-        """
         if self.address and self.address != "auto":
             self.logger.info(
                 f"Connecting to an existing Ray instance at {self.address}"
             )
             init_args = (self.address,)
         elif ray.is_initialized():
             self.logger.info(
                 "Local Ray instance is already initialized. "
                 "Using existing local instance."
             )
-            return
+            return self
         else:
             self.logger.info("Creating a local Ray instance")
             init_args = ()
 
-        context = ray.init(*init_args, **self.init_kwargs)
-        dashboard_url = getattr(context, "dashboard_url", None)
-        exit_stack.push(context)
+        self._ray_context = ray.init(*init_args, **self.init_kwargs)
+        dashboard_url = getattr(self._ray_context, "dashboard_url", None)
 
         # Display some information about the cluster
         nodes = ray.nodes()
         living_nodes = [node for node in nodes if node.get("alive")]
         self.logger.info(f"Using Ray cluster with {len(living_nodes)} nodes.")
 
         if dashboard_url:
             self.logger.info(
                 f"The Ray UI is available at {dashboard_url}",
             )
 
-    async def _shutdown_ray(self):
+        return self
+
+    def __exit__(self, *exc_info):
         """
         Shuts down the cluster.
         """
         self.logger.debug("Shutting down Ray cluster...")
         ray.shutdown()
-
-    def _get_ray_ref(self, key: UUID) -> "ray.ObjectRef":
-        """
-        Retrieve the ray object reference corresponding to a prefect future.
-        """
-        return self._ray_refs[key]
+        super().__exit__(*exc_info)
```

### Comparing `prefect_ray-0.3.6/prefect_ray.egg-info/PKG-INFO` & `prefect_ray-0.4.0rc1/prefect_ray.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 Metadata-Version: 2.1
 Name: prefect-ray
-Version: 0.3.6
+Version: 0.4.0rc1
 Summary: Prefect integrations with the Ray execution framework.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-ray
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
 Requires-Dist: ray[default]>=2.0.0
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
 Requires-Dist: pytest-asyncio!=0.22.0,<0.23.0,>=0.18.2; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
@@ -57,15 +55,15 @@
 
 Provides a `RayTaskRunner` that enables Prefect flows to run tasks execute tasks in parallel using Ray.
 
 ## Getting Started
 
 ### Python setup
 
-Requires an installation of Python 3.8 or newer.
+Requires an installation of Python 3.9 or newer.
 
 We recommend using a Python virtual environment manager such as pipenv, conda, or virtualenv.
 
 These tasks are designed to work with Prefect 2.0+. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Installation
 
@@ -75,15 +73,15 @@
 pip install prefect-ray
 ```
 
 Users running Apple Silicon (such as M1 macs) should check out the Ray docs [here](https://docs.ray.io/en/master/ray-overview/installation.html#m1-mac-apple-silicon-support) for more details.
 
 ## Running tasks on Ray
 
-The `RayTaskRunner` is a [Prefect task runner](https://docs.prefect.io/concepts/task-runners/) that submits tasks to [Ray](https://www.ray.io/) for parallel execution. 
+The `RayTaskRunner` is a [Prefect task runner](https://docs.prefect.io/concepts/task-runners/) that submits tasks to [Ray](https://www.ray.io/) for parallel execution.
 
 By default, a temporary Ray instance is created for the duration of the flow run.
 
 For example, this flow counts to 3 in parallel.
 
 ```python
 import time
@@ -129,47 +127,47 @@
 
 ```python
 from prefect import flow
 from prefect_ray.task_runners import RayTaskRunner
 
 @flow(task_runner=RayTaskRunner())
 def my_flow():
-    ... 
+    ...
 ```
 
 This flow uses the `RayTaskRunner` configured to access an existing Ray instance at `ray://192.0.2.255:8786`.
 
 ```python
 from prefect import flow
 from prefect_ray.task_runners import RayTaskRunner
 
 @flow(task_runner=RayTaskRunner(address="ray://192.0.2.255:8786"))
 def my_flow():
-    ... 
+    ...
 ```
 
 `RayTaskRunner` accepts the following optional parameters:
 
-| Parameter | Description |
-| --- | --- |
-| address | Address of a currently running Ray instance, starting with the [ray://](https://docs.ray.io/en/master/cluster/ray-client.html) URI. |
-| init_kwargs | Additional kwargs to use when calling `ray.init`. |
+| Parameter   | Description                                                                                                                         |
+| ----------- | ----------------------------------------------------------------------------------------------------------------------------------- |
+| address     | Address of a currently running Ray instance, starting with the [ray://](https://docs.ray.io/en/master/cluster/ray-client.html) URI. |
+| init_kwargs | Additional kwargs to use when calling `ray.init`.                                                                                   |
 
 Note that Ray Client uses the [ray://](https://docs.ray.io/en/master/cluster/ray-client.html) URI to indicate the address of a Ray instance. If you don't provide the `address` of a Ray instance, Prefect creates a temporary instance automatically.
 
 !!! warning "Ray environment limitations"
     Ray support for non-x86/64 architectures such as ARM/M1 processors with installation from `pip` alone and will be skipped during installation of Prefect. It is possible to manually install the blocking component with `conda`. See the [Ray documentation](https://docs.ray.io/en/latest/ray-overview/installation.html#m1-mac-apple-silicon-support) for instructions.
 
     See the [Ray installation documentation](https://docs.ray.io/en/latest/ray-overview/installation.html) for further compatibility information.
 
 ## Running tasks on a Ray remote cluster
 
 When using the `RayTaskRunner` with a remote Ray cluster, you may run into issues that are not seen when using a local Ray instance. To resolve these issues, we recommend taking the following steps when working with a remote Ray cluster:
 
-1. By default, Prefect will not persist any data to the filesystem of the remote ray worker. However, if you want to take advantage of Prefect's caching ability, you will need to configure a remote result storage to persist results across task runs. 
+1. By default, Prefect will not persist any data to the filesystem of the remote ray worker. However, if you want to take advantage of Prefect's caching ability, you will need to configure a remote result storage to persist results across task runs.
 
 We recommend using the [Prefect UI to configure a storage block](https://docs.prefect.io/concepts/blocks/) to use for remote results storage.
 
 Here's an example of a flow that uses caching and remote result storage:
 ```python
 from typing import List
 
@@ -205,15 +203,15 @@
 ```
 
 2. If you get an error stating that the module 'prefect' cannot be found, ensure `prefect` is installed on the remote cluster, with:
 ```bash
 pip install prefect
 ```
 
-3. If you get an error with a message similar to "File system created with scheme 's3' could not be created", ensure the required Python modules are installed on **both local and remote machines**. The required prerequisite modules can be found in the [Prefect documentation](https://docs.prefect.io/guides/deployment/storage-guide). For example, if using S3 for the remote storage:
+3. If you get an error with a message similar to "File system created with scheme 's3' could not be created", ensure the required Python modules are installed on **both local and remote machines**. For example, if using S3 for the remote storage:
 ```bash
 pip install s3fs
 ```
 
 4. If you are seeing timeout or other connection errors, double check the address provided to the `RayTaskRunner`. The address should look similar to: `address='ray://<head_node_ip_address>:10001'`:
 ```bash
 RayTaskRunner(address="ray://1.23.199.255:10001")
```

### Comparing `prefect_ray-0.3.6/pyproject.toml` & `prefect_ray-0.4.0rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,44 +2,45 @@
 requires = ["setuptools>=45", "wheel", "setuptools_scm>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prefect-ray"
 description = "Prefect integrations with the Ray execution framework."
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
-dependencies = ["prefect>=2.14.10, < 3.0.0", "ray[default]>=2.0.0"]
+dependencies = [
+  "prefect>=3.0.0rc1",
+  "ray[default]>=2.0.0",
+]
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
   "pytest-asyncio>=0.18.2,!=0.22.0,<0.23.0",
   "pytest-xdist",
@@ -50,15 +51,15 @@
 
 [project.entry-points."prefect.collections"]
 prefect_ray = "prefect_ray"
 
 [tool.setuptools_scm]
 version_file = "prefect_ray/_version.py"
 root = "../../.."
-tag_regex = "^prefect-ray-(?P<version>\\d+\\.\\d+\\.\\d+)$"
+tag_regex = "^prefect-ray-(?P<version>\\d+\\.\\d+\\.\\d+(?:[a-zA-Z0-9]+(?:\\.[a-zA-Z0-9]+)*)?)$"
 fallback_version = "0.0.0"
 git_describe_command = 'git describe --dirty --tags --long --match "prefect-ray-*[0-9]*"'
 
 [tool.interrogate]
 ignore-init-module = true
 ignore_init_method = true
 exclude = ["prefect_ray/_version.py", "tests"]
```

### Comparing `prefect_ray-0.3.6/tests/test_block_standards.py` & `prefect_ray-0.4.0rc1/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect_ray-0.3.6/tests/test_context.py` & `prefect_ray-0.4.0rc1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `prefect_ray-0.3.6/tests/test_task_runners.py` & `prefect_ray-0.4.0rc1/tests/test_task_runners.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 import asyncio
 import logging
 import subprocess
 import sys
 import time
 import warnings
-from functools import partial
-from uuid import uuid4
 
 import pytest
 import ray
 import ray.cluster_utils
 from prefect_ray import RayTaskRunner
 from prefect_ray.context import remote_options
-from ray.exceptions import TaskCancelledError
 
 import prefect
-import prefect.engine
+import prefect.task_engine
 import tests
-from prefect import flow, get_run_logger, task
+from prefect import flow, task
 from prefect.states import State, StateType
-from prefect.tasks import TaskRun
 from prefect.testing.fixtures import (  # noqa: F401
     hosted_api_server,
     use_hosted_api_server,
 )
-from prefect.testing.standard_test_suites import TaskRunnerStandardTestSuite
-from prefect.testing.utilities import exceptions_equal
 
 
 @pytest.fixture(scope="session")
 def event_loop(request):
     """
     Redefine the event loop to support session/module-scoped fixtures;
     see https://github.com/pytest-dev/pytest-asyncio/issues/68
@@ -51,32 +45,34 @@
 
     try:
         yield loop
     finally:
         loop.close()
 
 
-@pytest.fixture(scope="module")
+@pytest.fixture
 def machine_ray_instance():
     """
     Starts a ray instance for the current machine
     """
-    subprocess.check_call(
-        [
-            "ray",
-            "start",
-            "--head",
-            "--include-dashboard",
-            "False",
-            "--disable-usage-stats",
-        ],
-        cwd=str(prefect.__development_base_path__),
-    )
     try:
+        subprocess.check_output(
+            [
+                "ray",
+                "start",
+                "--head",
+                "--include-dashboard",
+                "False",
+                "--disable-usage-stats",
+            ],
+            cwd=str(prefect.__development_base_path__),
+        )
         yield "ray://127.0.0.1:10001"
+    except subprocess.CalledProcessError as exc:
+        pytest.fail(f"Failed to start ray: {exc.stderr}")
     finally:
         subprocess.run(["ray", "stop"])
 
 
 @pytest.fixture
 def default_ray_task_runner():
     with warnings.catch_warnings():
@@ -108,15 +104,15 @@
                 # deserialize test tasks / flows
                 "py_modules": [tests]
             }
         },
     )
 
 
-@pytest.fixture(scope="module")
+@pytest.fixture
 def inprocess_ray_cluster():
     """
     Starts a ray cluster in-process
     """
     cluster = ray.cluster_utils.Cluster(initialize_head=True)
     try:
         cluster.add_node()  # We need to add a second node for parallelism
@@ -177,117 +173,258 @@
     ray_task_runner_with_temporary_cluster,
 ]
 
 if sys.version_info >= (3, 10):
     task_runner_setups.append(ray_task_runner_with_existing_cluster)
 
 
-class TestRayTaskRunner(TaskRunnerStandardTestSuite):
+class TestRayTaskRunner:
     @pytest.fixture(params=task_runner_setups)
     def task_runner(self, request):
         yield request.getfixturevalue(
             request.param._pytestfixturefunction.name or request.param.__name__
         )
 
+    @pytest.fixture
+    def tmp_file(self, tmp_path):
+        file_path = tmp_path / "canary.txt"
+        file_path.touch()
+        return file_path
+
+    async def test_duplicate(self, task_runner):
+        new = task_runner.duplicate()
+        assert new == task_runner
+        assert new is not task_runner
+
+    async def test_successful_flow_run(self, task_runner):
+        @task
+        def task_a():
+            return "a"
+
+        @task
+        def task_b():
+            return "b"
+
+        @task
+        def task_c(b):
+            return b + "c"
+
+        @flow(version="test", task_runner=task_runner)
+        def test_flow():
+            a = task_a.submit()
+            b = task_b.submit()
+            c = task_c.submit(b)
+            return a, b, c
+
+        a, b, c = test_flow()
+        assert await a.result() == "a"
+        assert await b.result() == "b"
+        assert await c.result() == "bc"
+
+    async def test_failing_flow_run(self, task_runner):
+        @task
+        def task_a():
+            raise RuntimeError("This task fails!")
+
+        @task
+        def task_b():
+            raise ValueError("This task fails and passes data downstream!")
+
+        @task
+        def task_c(b):
+            # This task attempts to use the upstream data and should fail too
+            return b + "c"
+
+        @flow(version="test", task_runner=task_runner)
+        def test_flow():
+            a = task_a.submit()
+            b = task_b.submit()
+            c = task_c.submit(b)
+            d = task_c.submit(c)
+
+            return a, b, c, d
+
+        state = test_flow(return_state=True)
+
+        assert state.is_failed()
+        result = await state.result(raise_on_failure=False)
+        a, b, c, d = result
+        with pytest.raises(RuntimeError, match="This task fails!"):
+            await a.result()
+        with pytest.raises(
+            ValueError, match="This task fails and passes data downstream"
+        ):
+            await b.result()
+
+        assert c.is_pending()
+        assert c.name == "NotReady"
+        assert (
+            f"Upstream task run '{b.state_details.task_run_id}' did not reach a"
+            " 'COMPLETED' state" in c.message
+        )
+
+        assert d.is_pending()
+        assert d.name == "NotReady"
+        assert (
+            f"Upstream task run '{c.state_details.task_run_id}' did not reach a"
+            " 'COMPLETED' state" in d.message
+        )
+
+    async def test_async_tasks(self, task_runner):
+        @task
+        async def task_a():
+            return "a"
+
+        @task
+        async def task_b():
+            return "b"
+
+        @task
+        async def task_c(b):
+            return b + "c"
+
+        @flow(version="test", task_runner=task_runner)
+        async def test_flow():
+            a = task_a.submit()
+            b = task_b.submit()
+            c = task_c.submit(b)
+            return a, b, c
+
+        a, b, c = await test_flow()
+        assert await a.result() == "a"
+        assert await b.result() == "b"
+        assert await c.result() == "bc"
+
+    async def test_submit_and_wait(self, task_runner):
+        @task
+        async def task_a():
+            return "a"
+
+        async def fake_orchestrate_task_run(example_kwarg):
+            return State(
+                type=StateType.COMPLETED,
+                data=example_kwarg,
+            )
+
+        with task_runner:
+            future = task_runner.submit(task_a, parameters={}, wait_for=[])
+            future.wait()
+            state = future.state
+            assert await state.result() == "a"
+
+    async def test_async_task_timeout(self, task_runner):
+        @task(timeout_seconds=0.1)
+        async def my_timeout_task():
+            await asyncio.sleep(2)
+            return 42
+
+        @task
+        async def my_dependent_task(task_res):
+            return 1764
+
+        @task
+        async def my_independent_task():
+            return 74088
+
+        @flow(version="test", task_runner=task_runner)
+        async def test_flow():
+            a = my_timeout_task.submit()
+            b = my_dependent_task.submit(a)
+            c = my_independent_task.submit()
+
+            return a, b, c
+
+        state = await test_flow(return_state=True)
+
+        assert state.is_failed()
+        ax, bx, cx = await state.result(raise_on_failure=False)
+        assert ax.type == StateType.FAILED
+        assert bx.type == StateType.PENDING
+        assert cx.type == StateType.COMPLETED
+
+    async def test_sync_task_timeout(self, task_runner):
+        @task(timeout_seconds=1)
+        def my_timeout_task():
+            time.sleep(2)
+            return 42
+
+        @task
+        def my_dependent_task(task_res):
+            return 1764
+
+        @task
+        def my_independent_task():
+            return 74088
+
+        @flow(version="test", task_runner=task_runner)
+        def test_flow():
+            a = my_timeout_task.submit()
+            b = my_dependent_task.submit(a)
+            c = my_independent_task.submit()
+
+            return a, b, c
+
+        state = test_flow(return_state=True)
+
+        assert state.is_failed()
+        ax, bx, cx = await state.result(raise_on_failure=False)
+        assert ax.type == StateType.FAILED
+        assert bx.type == StateType.PENDING
+        assert cx.type == StateType.COMPLETED
+
     def get_sleep_time(self) -> float:
         """
         Return an amount of time to sleep for concurrency tests.
         The RayTaskRunner is prone to flaking on concurrency tests.
         """
         return 5.0
 
-    @pytest.mark.parametrize("exception", [KeyboardInterrupt(), ValueError("test")])
-    async def test_wait_captures_exceptions_as_crashed_state(
-        self, task_runner, exception
-    ):
+    async def test_wait_captures_exceptions_as_crashed_state(self, task_runner):
         """
         Ray wraps the exception, interrupts will result in "Cancelled" tasks
         or "Killed" workers while normal errors will result in a "RayTaskError".
         We care more about the crash detection and
         lack of re-raise here than the equality of the exception.
         """
 
-        async def fake_orchestrate_task_run(task_run):
-            raise exception
-
-        task_run = TaskRun(
-            flow_run_id=uuid4(), task_key=str(uuid4()), dynamic_key="bar"
-        )
+        @task
+        async def task_a():
+            raise KeyboardInterrupt()
 
-        async with task_runner.start():
-            await task_runner.submit(
-                call=partial(fake_orchestrate_task_run, task_run=task_run),
-                key=task_run.id,
+        with task_runner:
+            future = task_runner.submit(
+                task=task_a,
+                parameters={},
+                wait_for=[],
             )
 
-            state = await task_runner.wait(task_run.id, 5)
+            future.wait()
+            state = future.state
             assert state is not None, "wait timed out"
             assert isinstance(state, State), "wait should return a state"
             assert state.name == "Crashed"
 
-    @pytest.mark.parametrize(
-        "exceptions",
-        [
-            (KeyboardInterrupt(), TaskCancelledError),
-            (ValueError("test"), ValueError),
-        ],
-    )
-    async def test_exception_to_crashed_state_in_flow_run(
-        self, exceptions, task_runner, monkeypatch
-    ):
-        (raised_exception, state_exception_type) = exceptions
-
-        async def throws_exception_before_task_begins(
-            task, task_run, parameters, wait_for, result_factory, settings, **kwds
-        ):
-            """
-            Simulates an exception occurring while a remote task runner is attempting
-            to unpickle and run a Prefect task.
-            """
-            raise raised_exception
-
-        monkeypatch.setattr(
-            prefect.engine, "begin_task_run", throws_exception_before_task_begins
-        )
-
-        @task()
-        def test_task():
-            logger = get_run_logger()
-            logger.info("Ray should raise an exception before this task runs.")
-
-        @flow(task_runner=task_runner)
-        def test_flow():
-            future = test_task.submit()
-            future.wait(10)
-
-        # ensure that the type of exception raised by the flow matches the type of
-        # exception we expected the task runner to receive.
-        with pytest.raises(state_exception_type) as exc:
-            test_flow()
-            # If Ray passes the same exception type back, it should pass
-            # the equality check
-            if type(raised_exception) == state_exception_type:
-                assert exceptions_equal(raised_exception, exc)
-
     def test_flow_and_subflow_both_with_task_runner(self, task_runner, tmp_file):
         @task
         def some_task(text):
             tmp_file.write_text(text)
 
         @flow(task_runner=RayTaskRunner())
         def subflow():
-            some_task.submit("a")
-            some_task.submit("b")
-            some_task.submit("c")
+            a = some_task.submit("a")
+            b = some_task.submit("b")
+            c = some_task.submit("c")
+            return a, b, c
 
         @flow(task_runner=task_runner)
         def base_flow():
             subflow()
             time.sleep(self.get_sleep_time())
-            some_task.submit("d")
+            d = some_task.submit("d")
+            return d
 
         base_flow()
         assert tmp_file.read_text() == "d"
 
     def test_ray_options(self):
         @task
         def process(x):
@@ -315,43 +452,7 @@
                 b_future = b.submit(wait_for=[a_future])
 
                 c.submit(wait_for=[b_future])
                 d.submit(wait_for=[b_future])
                 e.submit(wait_for=[b_future])
 
         flow_with_dependent_tasks()
-
-    def test_sync_task_timeout(self, task_runner):
-        """
-        This test is inherited from the prefect testing module and it may not
-        appropriately skip on Windows. Here we skip it explicitly.
-        """
-        if sys.platform.startswith("win"):
-            pytest.skip("cancellation due to timeouts is not supported on Windows")
-        super().test_async_task_timeout(task_runner)
-
-    async def test_submit_and_wait(self, task_runner):
-        """
-        This test is inherited from the prefect testing module. The key difference
-        here is that task_runner is waiting longer than 5 seconds.
-        """
-        MAX_WAIT_TIME = 60
-
-        task_run = TaskRun(flow_run_id=uuid4(), task_key="foo", dynamic_key="bar")
-
-        async def fake_orchestrate_task_run(example_kwarg, task_run):
-            return State(
-                type=StateType.COMPLETED,
-                data=example_kwarg,
-            )
-
-        async with task_runner.start():
-            await task_runner.submit(
-                key=task_run.id,
-                call=partial(
-                    fake_orchestrate_task_run, task_run=task_run, example_kwarg=1
-                ),
-            )
-            state = await task_runner.wait(task_run.id, MAX_WAIT_TIME)
-            assert state is not None, "wait timed out"
-            assert isinstance(state, State), "wait should return a state"
-            assert await state.result() == 1
```

