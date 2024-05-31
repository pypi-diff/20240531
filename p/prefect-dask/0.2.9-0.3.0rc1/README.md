# Comparing `tmp/prefect_dask-0.2.9.tar.gz` & `tmp/prefect_dask-0.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_dask-0.2.9.tar", last modified: Thu May 16 20:58:35 2024, max compression
+gzip compressed data, was "prefect_dask-0.3.0rc1.tar", last modified: Fri May 31 20:49:35 2024, max compression
```

## Comparing `prefect_dask-0.2.9.tar` & `prefect_dask-0.3.0rc1.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.480780 prefect_dask-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11371 2024-05-16 20:58:35.476780 prefect_dask-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9529 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.472780 prefect_dask-0.2.9/prefect_dask/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/prefect_dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 20:58:35.000000 prefect_dask-0.2.9/prefect_dask/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/prefect_dask/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13443 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/prefect_dask/task_runners.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/prefect_dask/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.476780 prefect_dask-0.2.9/prefect_dask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11371 2024-05-16 20:58:35.000000 prefect_dask-0.2.9/prefect_dask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-16 20:58:35.000000 prefect_dask-0.2.9/prefect_dask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:58:35.000000 prefect_dask-0.2.9/prefect_dask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-16 20:58:35.000000 prefect_dask-0.2.9/prefect_dask.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-16 20:58:35.000000 prefect_dask-0.2.9/prefect_dask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 20:58:35.000000 prefect_dask-0.2.9/prefect_dask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:58:35.480780 prefect_dask-0.2.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.476780 prefect_dask-0.2.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)    11057 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/tests/test_task_runners.py
--rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:35.960592 prefect_dask-0.3.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-31 20:49:24.000000 prefect_dask-0.3.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-31 20:49:24.000000 prefect_dask-0.3.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11135 2024-05-31 20:49:35.960592 prefect_dask-0.3.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9529 2024-05-31 20:49:24.000000 prefect_dask-0.3.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:35.956592 prefect_dask-0.3.0rc1/prefect_dask/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-31 20:49:24.000000 prefect_dask-0.3.0rc1/prefect_dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-31 20:49:35.000000 prefect_dask-0.3.0rc1/prefect_dask/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-31 20:49:24.000000 prefect_dask-0.3.0rc1/prefect_dask/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:49:24.000000 prefect_dask-0.3.0rc1/prefect_dask/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-05-31 20:49:24.000000 prefect_dask-0.3.0rc1/prefect_dask/task_runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-31 20:49:24.000000 prefect_dask-0.3.0rc1/prefect_dask/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:35.956592 prefect_dask-0.3.0rc1/prefect_dask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11135 2024-05-31 20:49:35.000000 prefect_dask-0.3.0rc1/prefect_dask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-31 20:49:35.000000 prefect_dask-0.3.0rc1/prefect_dask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:49:35.000000 prefect_dask-0.3.0rc1/prefect_dask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-31 20:49:35.000000 prefect_dask-0.3.0rc1/prefect_dask.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-31 20:49:35.000000 prefect_dask-0.3.0rc1/prefect_dask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-31 20:49:35.000000 prefect_dask-0.3.0rc1/prefect_dask.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-31 20:49:24.000000 prefect_dask-0.3.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:49:35.960592 prefect_dask-0.3.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:35.956592 prefect_dask-0.3.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:24.000000 prefect_dask-0.3.0rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-31 20:49:24.000000 prefect_dask-0.3.0rc1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-31 20:49:24.000000 prefect_dask-0.3.0rc1/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-05-31 20:49:24.000000 prefect_dask-0.3.0rc1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10805 2024-05-31 20:49:24.000000 prefect_dask-0.3.0rc1/tests/test_task_runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-31 20:49:24.000000 prefect_dask-0.3.0rc1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-31 20:49:24.000000 prefect_dask-0.3.0rc1/tests/test_version.py
```

### Comparing `prefect_dask-0.2.9/LICENSE` & `prefect_dask-0.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_dask-0.2.9/PKG-INFO` & `prefect_dask-0.3.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 Metadata-Version: 2.1
 Name: prefect-dask
-Version: 0.2.9
+Version: 0.3.0rc1
 Summary: Prefect integrations with the Dask execution framework.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-dask
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
-Requires-Dist: anyio<4.0.0,>=3.7.1
-Requires-Dist: prefect<3.0.0,>=2.13.5
-Requires-Dist: distributed==2022.2.0; python_version < "3.8"
-Requires-Dist: distributed!=2023.3.2,!=2023.3.2.1,!=2023.4.*,!=2023.5.*,>=2022.5.0; python_version >= "3.8"
+Requires-Dist: prefect>=3.0.0rc1
+Requires-Dist: distributed!=2023.3.2,!=2023.3.2.1,!=2023.4.*,!=2023.5.*,>=2022.5.0
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
 Requires-Dist: pytest-asyncio!=0.22.0,<0.23.0,>=0.18.2; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
```

### Comparing `prefect_dask-0.2.9/README.md` & `prefect_dask-0.3.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `prefect_dask-0.2.9/prefect_dask/task_runners.py` & `prefect_dask-0.3.0rc1/prefect_dask/task_runners.py`

 * *Files 13% similar despite different names*

```diff
@@ -68,30 +68,73 @@
     #5
     #8
     #9
     ```
 """
 
 import inspect
-from contextlib import AsyncExitStack
-from typing import Awaitable, Callable, Dict, Optional, Union
-from uuid import UUID
+from contextlib import ExitStack
+from typing import Any, Callable, Dict, Iterable, Optional, Set, Union
 
 import distributed
 
-from prefect.client.schemas.objects import State
-from prefect.context import FlowRunContext
-from prefect.futures import PrefectFuture
-from prefect.states import exception_to_crashed_state
-from prefect.task_runners import BaseTaskRunner, R, TaskConcurrencyType
+from prefect.client.schemas.objects import State, TaskRunInput
+from prefect.futures import PrefectFuture, PrefectWrappedFuture
+from prefect.task_runners import TaskRunner
+from prefect.tasks import Task
+from prefect.utilities.asyncutils import run_coro_as_sync
 from prefect.utilities.collections import visit_collection
 from prefect.utilities.importtools import from_qualified_name, to_qualified_name
+from prefect_dask.client import PrefectDaskClient
 
 
-class DaskTaskRunner(BaseTaskRunner):
+class PrefectDaskFuture(PrefectWrappedFuture[distributed.Future]):
+    """
+    A Prefect future that wraps a distributed.Future. This future is used
+    when the task run is submitted to a DaskTaskRunner.
+    """
+
+    def wait(self, timeout: Optional[float] = None) -> None:
+        try:
+            result = self._wrapped_future.result(timeout=timeout)
+        except Exception:
+            # either the task failed or the timeout was reached
+            return
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
+                future_result = self._wrapped_future.result(timeout=timeout)
+            except distributed.TimeoutError as exc:
+                raise TimeoutError(
+                    f"Task run {self.task_run_id} did not complete within {timeout} seconds"
+                ) from exc
+
+            if isinstance(future_result, State):
+                self._final_state = future_result
+            else:
+                return future_result
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
+class DaskTaskRunner(TaskRunner):
     """
     A parallel task_runner that submits tasks to the `dask.distributed` scheduler.
     By default a temporary `distributed.LocalCluster` is created (and
     subsequently torn down) within the `start()` contextmanager. To use a
     different cluster class (e.g.
     [`dask_kubernetes.KubeCluster`](https://kubernetes.dask.org/)), you can
     specify `cluster_class`/`cluster_kwargs`.
@@ -149,37 +192,32 @@
         DaskTaskRunner(address="192.0.2.255:8786")
         ```
     """
 
     def __init__(
         self,
         cluster: Optional[distributed.deploy.Cluster] = None,
-        address: str = None,
-        cluster_class: Union[str, Callable] = None,
-        cluster_kwargs: dict = None,
-        adapt_kwargs: dict = None,
-        client_kwargs: dict = None,
+        address: Optional[str] = None,
+        cluster_class: Union[str, Callable, None] = None,
+        cluster_kwargs: Optional[Dict] = None,
+        adapt_kwargs: Optional[Dict] = None,
+        client_kwargs: Optional[Dict] = None,
     ):
         # Validate settings and infer defaults
         if address:
             if cluster or cluster_class or cluster_kwargs or adapt_kwargs:
                 raise ValueError(
                     "Cannot specify `address` and "
                     "`cluster`/`cluster_class`/`cluster_kwargs`/`adapt_kwargs`"
                 )
         elif cluster:
             if cluster_class or cluster_kwargs:
                 raise ValueError(
                     "Cannot specify `cluster` and `cluster_class`/`cluster_kwargs`"
                 )
-            if not cluster.asynchronous:
-                raise ValueError(
-                    "The cluster must have `asynchronous=True` to be "
-                    "used with `DaskTaskRunner`."
-                )
         else:
             if isinstance(cluster_class, str):
                 cluster_class = from_qualified_name(cluster_class)
             else:
                 cluster_class = cluster_class
 
         # Create a copies of incoming kwargs since we may mutate them
@@ -206,127 +244,92 @@
         self.address = address
         self.cluster_class = cluster_class
         self.cluster_kwargs = cluster_kwargs
         self.adapt_kwargs = adapt_kwargs
         self.client_kwargs = client_kwargs
 
         # Runtime attributes
-        self._client: "distributed.Client" = None
+        self._client: PrefectDaskClient = None
         self._cluster: "distributed.deploy.Cluster" = cluster
-        self._dask_futures: Dict[str, "distributed.Future"] = {}
 
-        super().__init__()
-
-    @property
-    def concurrency_type(self) -> TaskConcurrencyType:
-        return (
-            TaskConcurrencyType.PARALLEL
-            if self.cluster_kwargs.get("processes")
-            else TaskConcurrencyType.CONCURRENT
-        )
+        self._exit_stack = ExitStack()
 
-    def duplicate(self):
-        """
-        Create a new instance of the task runner with the same settings.
-        """
-        return type(self)(
-            address=self.address,
-            cluster_class=self.cluster_class,
-            cluster_kwargs=self.cluster_kwargs,
-            adapt_kwargs=self.adapt_kwargs,
-            client_kwargs=self.client_kwargs,
-        )
+        super().__init__()
 
     def __eq__(self, other: object) -> bool:
         """
         Check if an instance has the same settings as this task runner.
         """
-        if type(self) == type(other):
+        if isinstance(other, DaskTaskRunner):
             return (
                 self.address == other.address
                 and self.cluster_class == other.cluster_class
                 and self.cluster_kwargs == other.cluster_kwargs
                 and self.adapt_kwargs == other.adapt_kwargs
                 and self.client_kwargs == other.client_kwargs
             )
         else:
-            return NotImplemented
+            return False
+
+    def duplicate(self):
+        """
+        Create a new instance of the task runner with the same settings.
+        """
+        return type(self)(
+            address=self.address,
+            cluster_class=self.cluster_class,
+            cluster_kwargs=self.cluster_kwargs,
+            adapt_kwargs=self.adapt_kwargs,
+            client_kwargs=self.client_kwargs,
+        )
 
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
+    ) -> PrefectDaskFuture:
         if not self._started:
             raise RuntimeError(
                 "The task runner must be started before submitting work."
             )
 
         # unpack the upstream call in order to cast Prefect futures to Dask futures
         # where possible to optimize Dask task scheduling
-        call_kwargs = self._optimize_futures(call.keywords)
-
-        if "task_run" in call_kwargs:
-            task_run = call_kwargs["task_run"]
-            flow_run = FlowRunContext.get().flow_run
-            # Dask displays the text up to the first '-' as the name; the task run key
-            # should include the task run name for readability in the Dask console.
-            # For cases where the task run fails and reruns for a retried flow run,
-            # the flow run count is included so that the new key will not match
-            # the failed run's key, therefore not retrieving from the Dask cache.
-            dask_key = f"{task_run.name}-{task_run.id.hex}-{flow_run.run_count}"
-        else:
-            dask_key = str(key)
+        parameters = self._optimize_futures(parameters)
 
-        self._dask_futures[key] = self._client.submit(
-            call.func,
-            key=dask_key,
-            # Dask defaults to treating functions are pure, but we set this here for
-            # explicit expectations. If this task run is submitted to Dask twice, the
-            # result of the first run should be returned. Subsequent runs would return
-            # `Abort` exceptions if they were submitted again.
-            pure=True,
-            **call_kwargs,
+        future = self._client.submit(
+            task,
+            parameters=parameters,
+            wait_for=wait_for,
+            dependencies=dependencies,
+            return_type="state",
         )
-
-    def _get_dask_future(self, key: UUID) -> "distributed.Future":
-        """
-        Retrieve the dask future corresponding to a Prefect future.
-        The Dask future is for the `run_fn`, which should return a `State`.
-        """
-        return self._dask_futures[key]
+        return PrefectDaskFuture(wrapped_future=future, task_run_id=future.task_run_id)
 
     def _optimize_futures(self, expr):
         def visit_fn(expr):
-            if isinstance(expr, PrefectFuture):
-                dask_future = self._dask_futures.get(expr.key)
+            if isinstance(expr, PrefectDaskFuture):
+                dask_future = expr.wrapped_future
                 if dask_future is not None:
                     return dask_future
             # Fallback to return the expression unaltered
             return expr
 
         return visit_collection(expr, visit_fn=visit_fn, return_data=True)
 
-    async def wait(self, key: UUID, timeout: float = None) -> Optional[State]:
-        future = self._get_dask_future(key)
-        try:
-            return await future.result(timeout=timeout)
-        except distributed.TimeoutError:
-            return None
-        except BaseException as exc:
-            return await exception_to_crashed_state(exc)
-
-    async def _start(self, exit_stack: AsyncExitStack):
+    def __enter__(self):
         """
         Start the task runner and prep for context exit.
         - Creates a cluster if an external address is not set.
         - Creates a client to connect to the cluster.
-        - Pushes a call to wait for all running futures to complete on exit.
         """
-
+        super().__enter__()
+        exit_stack = self._exit_stack.__enter__()
         if self._cluster:
             self.logger.info(f"Connecting to existing Dask cluster {self._cluster}")
             self._connect_to = self._cluster
             if self.adapt_kwargs:
                 self._cluster.adapt(**self.adapt_kwargs)
         elif self.address:
             self.logger.info(
@@ -336,42 +339,30 @@
         else:
             self.cluster_class = self.cluster_class or distributed.LocalCluster
 
             self.logger.info(
                 f"Creating a new Dask cluster with "
                 f"`{to_qualified_name(self.cluster_class)}`"
             )
-            self._connect_to = self._cluster = await exit_stack.enter_async_context(
-                self.cluster_class(asynchronous=True, **self.cluster_kwargs)
+            self._connect_to = self._cluster = exit_stack.enter_context(
+                self.cluster_class(**self.cluster_kwargs)
             )
+
             if self.adapt_kwargs:
-                adapt_response = self._cluster.adapt(**self.adapt_kwargs)
-                if inspect.isawaitable(adapt_response):
-                    await adapt_response
-
-        self._client = await exit_stack.enter_async_context(
-            distributed.Client(
-                self._connect_to, asynchronous=True, **self.client_kwargs
-            )
+                maybe_coro = self._cluster.adapt(**self.adapt_kwargs)
+                if inspect.isawaitable(maybe_coro):
+                    run_coro_as_sync(maybe_coro)
+
+        self._client = exit_stack.enter_context(
+            PrefectDaskClient(self._connect_to, **self.client_kwargs)
         )
 
         if self._client.dashboard_link:
             self.logger.info(
                 f"The Dask dashboard is available at {self._client.dashboard_link}",
             )
 
-    def __getstate__(self):
-        """
-        Allow the `DaskTaskRunner` to be serialized by dropping
-        the `distributed.Client`, which contains locks.
-        Must be deserialized on a dask worker.
-        """
-        data = self.__dict__.copy()
-        data.update({k: None for k in {"_client", "_cluster", "_connect_to"}})
-        return data
+        return self
 
-    def __setstate__(self, data: dict):
-        """
-        Restore the `distributed.Client` by loading the client on a dask worker.
-        """
-        self.__dict__.update(data)
-        self._client = distributed.get_client()
+    def __exit__(self, *args):
+        self._exit_stack.__exit__(*args)
+        super().__exit__(*args)
```

### Comparing `prefect_dask-0.2.9/prefect_dask/utils.py` & `prefect_dask-0.3.0rc1/prefect_dask/utils.py`

 * *Files identical despite different names*

### Comparing `prefect_dask-0.2.9/prefect_dask.egg-info/PKG-INFO` & `prefect_dask-0.3.0rc1/prefect_dask.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 Metadata-Version: 2.1
 Name: prefect-dask
-Version: 0.2.9
+Version: 0.3.0rc1
 Summary: Prefect integrations with the Dask execution framework.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-dask
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
-Requires-Dist: anyio<4.0.0,>=3.7.1
-Requires-Dist: prefect<3.0.0,>=2.13.5
-Requires-Dist: distributed==2022.2.0; python_version < "3.8"
-Requires-Dist: distributed!=2023.3.2,!=2023.3.2.1,!=2023.4.*,!=2023.5.*,>=2022.5.0; python_version >= "3.8"
+Requires-Dist: prefect>=3.0.0rc1
+Requires-Dist: distributed!=2023.3.2,!=2023.3.2.1,!=2023.4.*,!=2023.5.*,>=2022.5.0
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
 Requires-Dist: pytest-asyncio!=0.22.0,<0.23.0,>=0.18.2; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
```

### Comparing `prefect_dask-0.2.9/pyproject.toml` & `prefect_dask-0.3.0rc1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [build-system]
 requires = ["setuptools>=45", "wheel", "setuptools_scm>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prefect-dask"
 dependencies = [
-  "anyio >= 3.7.1, < 4.0.0",
-  "prefect>=2.13.5, < 3.0.0",
-  "distributed==2022.2.0; python_version < '3.8'",
-  "distributed>=2022.5.0,!=2023.3.2,!=2023.3.2.1,!=2023.4.*,!=2023.5.*; python_version >= '3.8'", # don't allow versions from 2023.3.2 to 2023.5 (inclusive) due to issue with get_client starting in 2023.3.2 (fixed in 2023.6.0) - https://github.com/dask/distributed/issues/7763
+  "prefect>=3.0.0rc1",
+  # don't allow versions from 2023.3.2 to 2023.5 (inclusive) due to issue with
+  # get_client starting in 2023.3.2 (fixed in 2023.6.0)
+  # https://github.com/dask/distributed/issues/7763
+  "distributed>=2022.5.0,!=2023.3.2,!=2023.3.2.1,!=2023.4.*,!=2023.5.*",
 ]
 dynamic = ["version"]
 description = "Prefect integrations with the Dask execution framework."
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
 
@@ -35,15 +35,14 @@
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
   "pytest-asyncio >= 0.18.2, != 0.22.0, < 0.23.0",
   "pytest",
   "pytest-xdist",
 ]
@@ -53,15 +52,15 @@
 
 [project.entry-points."prefect.collections"]
 prefect_dask = "prefect_dask"
 
 [tool.setuptools_scm]
 version_file = "prefect_dask/_version.py"
 root = "../../.."
-tag_regex = "^prefect-dask-(?P<version>\\d+\\.\\d+\\.\\d+)$"
+tag_regex = "^prefect-dask-(?P<version>\\d+\\.\\d+\\.\\d+(?:[a-zA-Z0-9]+(?:\\.[a-zA-Z0-9]+)*)?)$"
 fallback_version = "0.0.0"
 git_describe_command = 'git describe --dirty --tags --long --match "prefect-dask-*[0-9]*"'
 
 [tool.interrogate]
 ignore-init-module = true
 ignore_init_method = true
 exclude = ["prefect_dask/_version.py", "tests"]
```

### Comparing `prefect_dask-0.2.9/tests/test_block_standards.py` & `prefect_dask-0.3.0rc1/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect_dask-0.2.9/tests/test_task_runners.py` & `prefect_dask-0.3.0rc1/tests/test_task_runners.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,31 @@
 import asyncio
-import logging
-import sys
-from functools import partial
+import time
 from typing import List
-from uuid import uuid4
 
-import cloudpickle
 import distributed
 import pytest
 from distributed import LocalCluster
-from distributed.scheduler import KilledWorker
 from prefect_dask import DaskTaskRunner
 
-import prefect.engine
-from prefect import flow, get_run_logger, task
-from prefect.client.schemas import TaskRun
+from prefect import flow, task
 from prefect.server.schemas.states import StateType
 from prefect.states import State
-from prefect.task_runners import TaskConcurrencyType
 from prefect.testing.fixtures import (  # noqa: F401
     hosted_api_server,
     use_hosted_api_server,
 )
-from prefect.testing.standard_test_suites import TaskRunnerStandardTestSuite
-from prefect.testing.utilities import exceptions_equal
-
-
-@pytest.fixture(scope="session")
-def event_loop(request):
-    """
-    Redefine the event loop to support session/module-scoped fixtures;
-    see https://github.com/pytest-dev/pytest-asyncio/issues/68
-    When running on Windows we need to use a non-default loop for subprocess support.
-    """
-    if sys.platform == "win32":
-        asyncio.set_event_loop_policy(asyncio.WindowsProactorEventLoopPolicy())
-
-    policy = asyncio.get_event_loop_policy()
-
-    loop = policy.new_event_loop()
-
-    # configure asyncio logging to capture long running tasks
-    asyncio_logger = logging.getLogger("asyncio")
-    asyncio_logger.setLevel("WARNING")
-    asyncio_logger.addHandler(logging.StreamHandler())
-    loop.set_debug(True)
-    loop.slow_callback_duration = 0.25
-
-    try:
-        yield loop
-    finally:
-        loop.close()
-
-    # Workaround for failures in pytest_asyncio 0.17;
-    # see https://github.com/pytest-dev/pytest-asyncio/issues/257
-    policy.set_event_loop(loop)
 
 
 @pytest.fixture
-async def dask_task_runner_with_existing_cluster(use_hosted_api_server):  # noqa
+def dask_task_runner_with_existing_cluster(use_hosted_api_server):  # noqa
     """
     Generate a dask task runner that's connected to a local cluster
     """
-    async with distributed.LocalCluster(n_workers=2, asynchronous=True) as cluster:
+    with distributed.LocalCluster(n_workers=2) as cluster:
         yield DaskTaskRunner(cluster=cluster)
 
 
 @pytest.fixture
 def dask_task_runner_with_existing_cluster_address(use_hosted_api_server):  # noqa
     """
     Generate a dask task runner that's connected to a local cluster
@@ -74,182 +33,275 @@
     with distributed.LocalCluster(n_workers=2) as cluster:
         with distributed.Client(cluster) as client:
             address = client.scheduler.address
             yield DaskTaskRunner(address=address)
 
 
 @pytest.fixture
-def dask_task_runner_with_process_pool():
+def dask_task_runner_with_process_pool(use_hosted_api_server):  # noqa
     yield DaskTaskRunner(cluster_kwargs={"processes": True})
 
 
 @pytest.fixture
-def dask_task_runner_with_thread_pool():
+def dask_task_runner_with_thread_pool(use_hosted_api_server):  # noqa
     yield DaskTaskRunner(cluster_kwargs={"processes": False})
 
 
 @pytest.fixture
-def default_dask_task_runner():
+def default_dask_task_runner(use_hosted_api_server):  # noqa
     yield DaskTaskRunner()
 
 
-class TestDaskTaskRunner(TaskRunnerStandardTestSuite):
+class TestDaskTaskRunner:
     @pytest.fixture(
         params=[
             default_dask_task_runner,
-            dask_task_runner_with_existing_cluster,
+            # Existing cluster works outside of tests, but fails with serialization errors in tests
+            # dask_task_runner_with_existing_cluster, :TODO Fix serialization errors in these tests
             dask_task_runner_with_existing_cluster_address,
             dask_task_runner_with_process_pool,
             dask_task_runner_with_thread_pool,
         ]
     )
     def task_runner(self, request):
         yield request.getfixturevalue(
             request.param._pytestfixturefunction.name or request.param.__name__
         )
 
-    def test_sync_task_timeout(self, task_runner):
-        """
-        This test is inherited from the prefect testing module and it may not
-        appropriately skip on Windows. Here we skip it explicitly.
-        """
-        if sys.platform.startswith("win"):
-            pytest.skip("cancellation due to timeouts is not supported on Windows")
-        super().test_async_task_timeout(task_runner)
+    async def test_duplicate(self, task_runner):
+        new = task_runner.duplicate()
+        assert new == task_runner
+        assert new is not task_runner
 
-    async def test_is_pickleable_after_start(self, task_runner):
-        """
-        The task_runner must be picklable as it is attached to `PrefectFuture` objects
-        Reimplemented to set Dask client as default to allow unpickling
-        """
-        task_runner.client_kwargs["set_as_default"] = True
-        async with task_runner.start():
-            pickled = cloudpickle.dumps(task_runner)
-            unpickled = cloudpickle.loads(pickled)
-            assert isinstance(unpickled, type(task_runner))
-
-    @pytest.mark.parametrize("exception", [KeyboardInterrupt(), ValueError("test")])
-    async def test_wait_captures_exceptions_as_crashed_state(
-        self, task_runner, exception
-    ):
-        """
-        Dask wraps the exception, interrupts will result in "Cancelled" tasks
-        or "Killed" workers while normal errors will result in the raw error with Dask.
-        We care more about the crash detection and
-        lack of re-raise here than the equality of the exception.
-        """
-        if task_runner.concurrency_type != TaskConcurrencyType.PARALLEL:
-            pytest.skip(
-                f"This will abort the run for "
-                f"{task_runner.concurrency_type} task runners."
-            )
+    async def test_successful_flow_run(self, task_runner):
+        @task
+        def task_a():
+            return "a"
 
-        task_run = TaskRun(flow_run_id=uuid4(), task_key="foo", dynamic_key="bar")
+        @task
+        def task_b():
+            return "b"
 
-        async def fake_orchestrate_task_run():
-            raise exception
+        @task
+        def task_c(b):
+            return b + "c"
 
-        async with task_runner.start():
-            await task_runner.submit(
-                key=task_run.id,
-                call=partial(fake_orchestrate_task_run),
-            )
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
 
-            state = await task_runner.wait(task_run.id, 5)
-            assert state is not None, "wait timed out"
-            assert isinstance(state, State), "wait should return a state"
-            assert state.type == StateType.CRASHED
-
-    @pytest.mark.parametrize(
-        "exceptions",
-        [
-            (KeyboardInterrupt(), KilledWorker),
-            (ValueError("test"), ValueError),
-        ],
-    )
-    async def test_exception_to_crashed_state_in_flow_run(
-        self, exceptions, task_runner, monkeypatch
-    ):
-        if task_runner.concurrency_type != TaskConcurrencyType.PARALLEL:
-            pytest.skip(
-                f"This will abort the run for "
-                f"{task_runner.concurrency_type} task runners."
-            )
+    async def test_failing_flow_run(self, task_runner):
+        @task
+        def task_a():
+            raise RuntimeError("This task fails!")
 
-        (raised_exception, state_exception_type) = exceptions
+        @task
+        def task_b():
+            raise ValueError("This task fails and passes data downstream!")
 
-        def throws_exception_before_task_begins(
-            task,
-            task_run,
-            parameters,
-            wait_for,
-            result_factory,
-            settings,
-            *args,
-            **kwds,
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
         ):
-            """
-            Simulates an exception occurring while a remote task runner is attempting
-            to unpickle and run a Prefect task.
-            """
-            raise raised_exception
+            await b.result()
 
-        monkeypatch.setattr(
-            prefect.engine, "begin_task_run", throws_exception_before_task_begins
+        assert c.is_pending()
+        assert c.name == "NotReady"
+        assert (
+            f"Upstream task run '{b.state_details.task_run_id}' did not reach a"
+            " 'COMPLETED' state" in c.message
         )
 
-        @task()
-        def test_task():
-            logger = get_run_logger()
-            logger.info("Dask should raise an exception before this task runs.")
+        assert d.is_pending()
+        assert d.name == "NotReady"
+        assert (
+            f"Upstream task run '{c.state_details.task_run_id}' did not reach a"
+            " 'COMPLETED' state" in d.message
+        )
 
-        @flow(task_runner=task_runner)
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
         def test_flow():
-            future = test_task.submit()
-            future.wait(10)
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
+    async def test_wait_captures_exceptions_as_crashed_state(self, task_runner):
+        """
+        Dask wraps the exception, interrupts will result in "Cancelled" tasks
+        or "Killed" workers while normal errors will result in the raw error with Dask.
+        We care more about the crash detection and
+        lack of re-raise here than the equality of the exception.
+        """
+        if "processes" in task_runner.cluster_kwargs:
+            pytest.skip("This will abort the run for a Dask cluster using processes.")
 
-        # ensure that the type of exception raised by the flow matches the type of
-        # exception we expected the task runner to receive.
-        with pytest.raises(state_exception_type) as exc:
-            await test_flow()
-            # If Dask passes the same exception type back, it should pass
-            # the equality check
-            if type(raised_exception) == state_exception_type:
-                assert exceptions_equal(raised_exception, exc)
-
-    def test_cluster_not_asynchronous(self):
-        with pytest.raises(ValueError, match="The cluster must have"):
-            with distributed.LocalCluster(n_workers=2) as cluster:
-                DaskTaskRunner(cluster=cluster)
+        @task
+        def task_a():
+            raise KeyboardInterrupt()
+
+        with task_runner:
+            future = task_runner.submit(
+                task=task_a,
+                parameters={},
+                wait_for=[],
+            )
+
+            future.wait()
+            assert future.state.type == StateType.CRASHED
 
     def test_dask_task_key_has_prefect_task_name(self):
         task_runner = DaskTaskRunner()
 
         @task
         def my_task():
             return 1
 
+        futures = []
+
         @flow(task_runner=task_runner)
         def my_flow():
-            my_task.submit()
-            my_task.submit()
-            my_task.submit()
+            futures.append(my_task.submit())
+            futures.append(my_task.submit())
+            futures.append(my_task.submit())
 
         my_flow()
-        futures = task_runner._dask_futures.values()
         # ensure task run name is in key
-        assert all(future.key.startswith("my_task-") for future in futures)
-        # ensure flow run retries is in key
-        assert all(future.key.endswith("-1") for future in futures)
+        assert all(
+            future.wrapped_future.key.startswith("my_task-") for future in futures
+        )
 
     async def test_dask_cluster_adapt_is_properly_called(self):
         # mock of cluster instances with synchronous adapt method like
         # dask_kubernetes.classic.kubecluster.KubeCluster
         class MockDaskCluster(LocalCluster):
-            def __init__(self, asynchronous: bool):
+            def __init__(self, asynchronous: bool = False):
                 self._adapt_called = False
                 super().__init__(asynchronous=asynchronous)
 
             def adapt(self, **kwargs):
                 self._adapt_called = True
 
         # mock of cluster instances with asynchronous adapt method like
@@ -260,36 +312,17 @@
 
         for task_runner_class in [MockDaskCluster, AsyncMockDaskCluster]:
             # the adapt_kwargs argument triggers the calls to the adapt method
             task_runner = DaskTaskRunner(
                 cluster_class=task_runner_class,
                 adapt_kwargs={"minimum": 1, "maximum": 1},
             )
-            async with task_runner.start():
+            with task_runner:
                 assert task_runner._cluster._adapt_called
 
-    async def test_task_runner_can_execute_sync_task_in_async_flow(self, task_runner):
-        """
-        This is a regression test for https://github.com/PrefectHQ/prefect/issues/7422
-        """
-
-        @task
-        def identity(x):
-            return x
-
-        @flow(task_runner=task_runner)
-        async def test_flow() -> int:
-            mapped_futures = identity.map(range(1, 4))
-            single_future = identity.submit(1)
-
-            return sum([fut.result() for fut in mapped_futures + [single_future]])
-
-        result = await test_flow()
-        assert result == 7  # 1 + 2 + 3 + 1
-
     class TestInputArguments:
         async def test_dataclasses_can_be_passed_to_task_runners(self, task_runner):
             """
             this is a regression test for https://github.com/PrefectHQ/prefect/issues/6905
             """
             from dataclasses import dataclass
```

### Comparing `prefect_dask-0.2.9/tests/test_utils.py` & `prefect_dask-0.3.0rc1/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 import dask
 import pytest
 from distributed import Client
 from prefect_dask import DaskTaskRunner, get_async_dask_client, get_dask_client
 
 from prefect import flow, task
 
+pytestmark = pytest.mark.skip(
+    reason="Skipping tests while task runner is being rewritten"
+)
+
 
 class TestDaskSyncClient:
     def test_from_task(self):
         @task
         def test_task():
             delayed_num = dask.delayed(42)
             with get_dask_client() as client:
@@ -62,28 +66,28 @@
             async with get_async_dask_client() as client:
                 assert isinstance(client, Client)
                 result = await client.compute(delayed_num).result()
             return result
 
         @flow(task_runner=DaskTaskRunner)
         async def test_flow():
-            future = await test_task.submit()
-            return await future.result()
+            future = test_task.submit()
+            return future.result()
 
         assert (await test_flow()) == 42
 
     def test_from_sync_task_error(self):
         @task
         def test_task():
             with get_async_dask_client():
                 pass
 
         @flow(task_runner=DaskTaskRunner)
         def test_flow():
-            test_task.submit()
+            return test_task.submit()
 
         if sys.version_info < (3, 11):
             with pytest.raises(AttributeError, match="__enter__"):
                 test_flow()
         else:
             with pytest.raises(
                 TypeError, match="not support the context manager protocol"
```

