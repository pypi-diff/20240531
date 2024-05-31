# Comparing `tmp/prefect_databricks-0.2.7.tar.gz` & `tmp/prefect_databricks-0.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_databricks-0.2.7.tar", last modified: Thu May 16 20:58:31 2024, max compression
+gzip compressed data, was "prefect_databricks-0.3.0rc1.tar", last modified: Fri May 31 20:49:36 2024, max compression
```

## Comparing `prefect_databricks-0.2.7.tar` & `prefect_databricks-0.3.0rc1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:31.271456 prefect_databricks-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-05-16 20:58:31.271456 prefect_databricks-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:31.267456 prefect_databricks-0.2.7/prefect_databricks/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/prefect_databricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 20:58:30.000000 prefect_databricks-0.2.7/prefect_databricks/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/prefect_databricks/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    19110 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/prefect_databricks/flows.py
--rw-r--r--   0 runner    (1001) docker     (127)    81198 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/prefect_databricks/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:31.267456 prefect_databricks-0.2.7/prefect_databricks/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/prefect_databricks/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   168341 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/prefect_databricks/models/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/prefect_databricks/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:31.267456 prefect_databricks-0.2.7/prefect_databricks/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)   178999 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/prefect_databricks/schemas/jobs-2.1-aws.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:31.267456 prefect_databricks-0.2.7/prefect_databricks/schemas/original/
--rw-r--r--   0 runner    (1001) docker     (127)   178843 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/prefect_databricks/schemas/original/jobs-2.1-aws.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:31.271456 prefect_databricks-0.2.7/prefect_databricks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-05-16 20:58:30.000000 prefect_databricks-0.2.7/prefect_databricks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-16 20:58:31.000000 prefect_databricks-0.2.7/prefect_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:58:30.000000 prefect_databricks-0.2.7/prefect_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-16 20:58:30.000000 prefect_databricks-0.2.7/prefect_databricks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-16 20:58:30.000000 prefect_databricks-0.2.7/prefect_databricks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 20:58:30.000000 prefect_databricks-0.2.7/prefect_databricks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:58:31.271456 prefect_databricks-0.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:31.271456 prefect_databricks-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/tests/mock_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    13610 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/tests/test_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/tests/test_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-16 20:58:19.000000 prefect_databricks-0.2.7/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:36.439279 prefect_databricks-0.3.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-31 20:49:25.000000 prefect_databricks-0.3.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-31 20:49:25.000000 prefect_databricks-0.3.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-05-31 20:49:36.439279 prefect_databricks-0.3.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-31 20:49:25.000000 prefect_databricks-0.3.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:36.431280 prefect_databricks-0.3.0rc1/prefect_databricks/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-31 20:49:25.000000 prefect_databricks-0.3.0rc1/prefect_databricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-31 20:49:36.000000 prefect_databricks-0.3.0rc1/prefect_databricks/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-31 20:49:25.000000 prefect_databricks-0.3.0rc1/prefect_databricks/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19074 2024-05-31 20:49:25.000000 prefect_databricks-0.3.0rc1/prefect_databricks/flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81182 2024-05-31 20:49:25.000000 prefect_databricks-0.3.0rc1/prefect_databricks/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:36.435279 prefect_databricks-0.3.0rc1/prefect_databricks/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:25.000000 prefect_databricks-0.3.0rc1/prefect_databricks/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   164508 2024-05-31 20:49:25.000000 prefect_databricks-0.3.0rc1/prefect_databricks/models/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-31 20:49:25.000000 prefect_databricks-0.3.0rc1/prefect_databricks/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:36.435279 prefect_databricks-0.3.0rc1/prefect_databricks/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)   178999 2024-05-31 20:49:25.000000 prefect_databricks-0.3.0rc1/prefect_databricks/schemas/jobs-2.1-aws.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:36.435279 prefect_databricks-0.3.0rc1/prefect_databricks/schemas/original/
+-rw-r--r--   0 runner    (1001) docker     (127)   178843 2024-05-31 20:49:25.000000 prefect_databricks-0.3.0rc1/prefect_databricks/schemas/original/jobs-2.1-aws.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:36.435279 prefect_databricks-0.3.0rc1/prefect_databricks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-05-31 20:49:36.000000 prefect_databricks-0.3.0rc1/prefect_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-31 20:49:36.000000 prefect_databricks-0.3.0rc1/prefect_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:49:36.000000 prefect_databricks-0.3.0rc1/prefect_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-31 20:49:36.000000 prefect_databricks-0.3.0rc1/prefect_databricks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-31 20:49:36.000000 prefect_databricks-0.3.0rc1/prefect_databricks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-31 20:49:36.000000 prefect_databricks-0.3.0rc1/prefect_databricks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-31 20:49:25.000000 prefect_databricks-0.3.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:49:36.439279 prefect_databricks-0.3.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:36.435279 prefect_databricks-0.3.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-31 20:49:25.000000 prefect_databricks-0.3.0rc1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-31 20:49:25.000000 prefect_databricks-0.3.0rc1/tests/mock_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-31 20:49:25.000000 prefect_databricks-0.3.0rc1/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-31 20:49:25.000000 prefect_databricks-0.3.0rc1/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13610 2024-05-31 20:49:25.000000 prefect_databricks-0.3.0rc1/tests/test_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-31 20:49:25.000000 prefect_databricks-0.3.0rc1/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-31 20:49:25.000000 prefect_databricks-0.3.0rc1/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-31 20:49:25.000000 prefect_databricks-0.3.0rc1/tests/test_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-31 20:49:25.000000 prefect_databricks-0.3.0rc1/tests/test_version.py
```

### Comparing `prefect_databricks-0.2.7/LICENSE` & `prefect_databricks-0.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.7/PKG-INFO` & `prefect_databricks-0.3.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 Metadata-Version: 2.1
 Name: prefect-databricks
-Version: 0.2.7
+Version: 0.3.0rc1
 Summary: Prefect integrations with Databricks
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-databricks
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
 Requires-Dist: respx; extra == "dev"
```

### Comparing `prefect_databricks-0.2.7/README.md` & `prefect_databricks-0.3.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.7/prefect_databricks/credentials.py` & `prefect_databricks-0.3.0rc1/prefect_databricks/credentials.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 """Credential classes used to perform authenticated interactions with Databricks"""
 
 from typing import Any, Dict, Optional
 
 from httpx import AsyncClient
-
-from prefect._internal.pydantic import HAS_PYDANTIC_V2
-
-if HAS_PYDANTIC_V2:
-    from pydantic.v1 import Field, SecretStr
-else:
-    from pydantic import Field, SecretStr
+from pydantic import Field, SecretStr
 
 from prefect.blocks.core import Block
 
 
 class DatabricksCredentials(Block):
     """
     Block used to manage Databricks authentication.
```

### Comparing `prefect_databricks-0.2.7/prefect_databricks/flows.py` & `prefect_databricks-0.3.0rc1/prefect_databricks/flows.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,25 +249,25 @@
 
             return multi_task_runs
         ```
     """  # noqa
     logger = get_run_logger()
 
     # submit the jobs runs
-    multi_task_jobs_runs_future = await jobs_runs_submit.submit(
+    multi_task_jobs_runs_future = jobs_runs_submit.submit(
         databricks_credentials=databricks_credentials,
         tasks=tasks,
         run_name=run_name,
         git_source=git_source,
         timeout_seconds=timeout_seconds,
         idempotency_token=idempotency_token,
         access_control_list=access_control_list,
         **jobs_runs_submit_kwargs,
     )
-    multi_task_jobs_runs = await multi_task_jobs_runs_future.result()
+    multi_task_jobs_runs = multi_task_jobs_runs_future.result()
     multi_task_jobs_runs_id = multi_task_jobs_runs["run_id"]
 
     # wait for all the jobs runs to complete in a separate flow
     # for a cleaner radar interface
     jobs_runs_state, jobs_runs_metadata = await jobs_runs_wait_for_completion(
         multi_task_jobs_runs_id=multi_task_jobs_runs_id,
         databricks_credentials=databricks_credentials,
@@ -284,19 +284,19 @@
     if jobs_runs_life_cycle_state == RunLifeCycleState.terminated.value:
         jobs_runs_result_state = jobs_runs_state.get("result_state", None)
         if jobs_runs_result_state == RunResultState.success.value:
             task_notebook_outputs = {}
             for task in jobs_runs_metadata["tasks"]:
                 task_key = task["task_key"]
                 task_run_id = task["run_id"]
-                task_run_output_future = await jobs_runs_get_output.submit(
+                task_run_output_future = jobs_runs_get_output.submit(
                     run_id=task_run_id,
                     databricks_credentials=databricks_credentials,
                 )
-                task_run_output = await task_run_output_future.result()
+                task_run_output = task_run_output_future.result()
                 task_run_notebook_output = task_run_output.get("notebook_output", {})
                 task_notebook_outputs[task_key] = task_run_notebook_output
             logger.info(
                 "Databricks Jobs Runs Submit (%s ID %s) completed successfully!",
                 run_name,
                 multi_task_jobs_runs_id,
             )
@@ -445,22 +445,22 @@
 
     seconds_waited_for_run_completion = 0
     wait_for = []
 
     jobs_status = {}
     tasks_status = {}
     while seconds_waited_for_run_completion <= max_wait_seconds:
-        jobs_runs_metadata_future = await jobs_runs_get.submit(
+        jobs_runs_metadata_future = jobs_runs_get.submit(
             run_id=multi_task_jobs_runs_id,
             databricks_credentials=databricks_credentials,
             wait_for=wait_for,
         )
         wait_for = [jobs_runs_metadata_future]
 
-        jobs_runs_metadata = await jobs_runs_metadata_future.result()
+        jobs_runs_metadata = jobs_runs_metadata_future.result()
         jobs_status = _update_and_log_state_changes(
             jobs_status, jobs_runs_metadata, logger, "Job"
         )
         jobs_runs_metadata_tasks = jobs_runs_metadata.get("tasks", [])
         for task_metadata in jobs_runs_metadata_tasks:
             tasks_status = _update_and_log_state_changes(
                 tasks_status, task_metadata, logger, "Task"
```

### Comparing `prefect_databricks-0.2.7/prefect_databricks/jobs.py` & `prefect_databricks-0.3.0rc1/prefect_databricks/jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,18 +6,17 @@
 # This module was auto-generated using prefect-collection-generator so
 # manually editing this file is not recommended. If this module
 # is outdated, rerun scripts/generate.py.
 
 # OpenAPI spec: jobs-2.1-aws.yaml
 # Updated at: 2022-12-10T01:04:37.047265
 
-from typing import Any, Dict, List, Optional, Union  # noqa
+from typing import Any, Dict, List, Optional
 
 from prefect import task
-
 from prefect_databricks import DatabricksCredentials
 from prefect_databricks.models import jobs as models  # noqa
 from prefect_databricks.rest import HTTPMethod, _unpack_contents, execute_endpoint
 
 
 @task
 async def jobs_runs_export(
```

### Comparing `prefect_databricks-0.2.7/prefect_databricks/models/jobs.py` & `prefect_databricks-0.3.0rc1/prefect_databricks/models/jobs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # generated by datamodel-codegen:
 #   filename:  jobs-2.1-aws.yaml
 #   timestamp: 2022-12-10T01:04:37+00:00
 
 from __future__ import annotations
 
 from enum import Enum
-from typing import Any, Dict, List, Optional, Union
-
-from prefect._internal.pydantic import HAS_PYDANTIC_V2
-
-if HAS_PYDANTIC_V2:
-    from pydantic.v1 import BaseModel, Extra, Field
-else:
-    from pydantic import BaseModel, Extra, Field
+from typing import Annotated, Any, Dict, List, Optional, Union
 
+from pydantic import BaseModel, ConfigDict, Field, RootModel
 from typing_extensions import Literal
 
 
 class AutoScale(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     max_workers: Optional[int] = Field(
         None,
         description=(
             "The maximum number of workers to which the cluster can scale up when"
             " overloaded. max_workers must be strictly greater than min_workers."
         ),
@@ -44,17 +36,15 @@
 
 
 class AwsAttributes(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     availability: Optional[Literal["SPOT", "ON_DEMAND", "SPOT_WITH_FALLBACK"]] = Field(
         None,
         description=(
             "Availability type used for all subsequent nodes past the `first_on_demand`"
             " ones. **Note:** If `first_on_demand` is zero, this availability type is"
             " used for the entire cluster.\n\n`SPOT`: use spot instances.\n`ON_DEMAND`:"
@@ -264,17 +254,15 @@
 
 
 class ClusterInstance(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     cluster_id: Optional[str] = Field(
         None,
         description=(
             "The canonical identifier for the cluster used by a run. This field is"
             " always available for runs on existing clusters. For runs on new clusters,"
             " it becomes available once the cluster is created. This value can be used"
@@ -298,17 +286,15 @@
 
 
 class ClusterSize(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     autoscale: Optional[AutoScale] = Field(
         None,
         description=(
             "If autoscale, parameters needed in order to automatically scale clusters"
             " up and down based on load."
         ),
@@ -367,28 +353,23 @@
 class ClusterTag(BaseModel):
     """
     See source code for the fields' description.
 
     An object with key value pairs. The key length must be between 1 and 127 UTF-8 characters, inclusive. The value length must be less than or equal to 255 UTF-8 characters. For a list of all restrictions, see AWS Tag Restrictions: <https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Using_Tags.html#tag-restrictions>
     """
 
-    class Config:
-        extra = Extra.allow
-
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
 
 class CronSchedule(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     pause_status: Optional[Literal["PAUSED", "UNPAUSED"]] = Field(
         None,
         description="Indicate whether this schedule is paused or not.",
         example="PAUSED",
     )
     quartz_cron_expression: str = Field(
@@ -414,31 +395,27 @@
 
 
 class DbfsStorageInfo(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     destination: Optional[str] = Field(
         None, description="DBFS destination. Example: `dbfs:/my/path`"
     )
 
 
 class DbtOutput(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     artifacts_headers: Optional[Dict[str, Any]] = Field(
         None,
         description=(
             "An optional map of headers to send when retrieving the artifact from the"
             " `artifacts_link`."
         ),
@@ -454,17 +431,15 @@
 
 
 class DbtTask(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     catalog: Optional[str] = Field(
         None,
         description=(
             "Optional name of the catalog to use. The value is the top level in the"
             " 3-level namespace of Unity Catalog (catalog / schema / relation). The"
             " catalog value can only be specified if a warehouse_id is specified."
@@ -518,49 +493,43 @@
 
 
 class DockerBasicAuth(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     password: Optional[str] = Field(
         None, description="Password for the Docker repository."
     )
     username: Optional[str] = Field(
         None, description="User name for the Docker repository."
     )
 
 
 class DockerImage(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     basic_auth: Optional[DockerBasicAuth] = Field(
         None, description="Basic authentication information for Docker repository."
     )
     url: Optional[str] = Field(None, description="URL for the Docker image.")
 
 
 class Error(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     error_code: Optional[str] = Field(
         None, description="Error code", example="INTERNAL_ERROR"
     )
     message: Optional[str] = Field(
         None,
         description=(
@@ -571,33 +540,29 @@
 
 
 class FileStorageInfo(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     destination: Optional[str] = Field(
         None, description="File destination. Example: `file:/my/file.sh`"
     )
 
 
 class GitSnapshot(BaseModel):
     """
     See source code for the fields' description.
 
     Read-only state of the remote repository at the time the job was run. This field is only included on job runs.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     used_commit: Optional[str] = Field(
         None,
         description=(
             "Commit that was used to execute the run. If git_branch was specified, this"
             " points to the HEAD of the branch at the time of the run; if git_tag was"
             " specified, this points to the commit the tag points to."
@@ -611,17 +576,15 @@
     See source code for the fields' description.
 
         This functionality is in Public Preview.
 
     An optional specification for a remote repository containing the notebooks used by this job's notebook tasks.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     git_branch: Optional[str] = Field(
         None,
         description=(
             "Name of the branch to be checked out and used by this job. This field"
             " cannot be specified in conjunction with git_tag or git_commit.\nThe"
             " maximum length is 255 characters."
@@ -672,55 +635,28 @@
             "URL of the repository to be cloned by this job.\nThe maximum length is 300"
             " characters."
         ),
         example="https://github.com/databricks/databricks-cli",
     )
 
 
-class GitSource1(BaseModel):
+class GitSource1(RootModel[Union[GitSource, Any, Any, Any]]):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
-
-    __root__: Union[GitSource, Any, Any, Any] = Field(
-        ...,
-        description=(
-            "This functionality is in Public Preview.\n\nAn optional specification for"
-            " a remote repository containing the notebooks used by this job's notebook"
-            " tasks."
-        ),
-        example={
-            "git_branch": "main",
-            "git_provider": "gitHub",
-            "git_url": "https://github.com/databricks/databricks-cli",
-        },
-    )
+    model_config = ConfigDict(frozen=True)
 
 
-class GroupName(BaseModel):
+class GroupName(RootModel[str]):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
-
-    __root__: str = Field(
-        ...,
-        description=(
-            "Group name. There are two built-in groups: `users` for all users, and"
-            " `admins` for administrators."
-        ),
-        example="users",
-    )
+    model_config = ConfigDict(frozen=True)
 
 
 class IsOwner(str, Enum):
     """
     Perimssion that represents ownership of the job.
     """
 
@@ -728,17 +664,15 @@
 
 
 class JobEmailNotifications(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     no_alert_for_skipped_runs: Optional[bool] = Field(
         None,
         description=(
             "If true, do not send email to recipients specified in `on_failure` if the"
             " run is skipped."
         ),
@@ -813,17 +747,15 @@
 
 
 class LogSyncStatus(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     last_attempted: Optional[int] = Field(
         None,
         description=(
             "The timestamp of last attempt. If the last attempt fails, last_exception"
             " contains the exception in the last attempt."
         ),
@@ -838,17 +770,15 @@
 
 
 class MavenLibrary(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     coordinates: str = Field(
         ...,
         description=(
             "Gradle-style Maven coordinates. For example: `org.jsoup:jsoup:1.7.2`. This"
             " field is required."
         ),
@@ -874,17 +804,15 @@
 
 
 class NotebookOutput(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     result: Optional[str] = Field(
         None,
         description=(
             "The value passed to"
             " [dbutils.notebook.exit()](https://docs.databricks.com/notebooks/notebook-workflows.html#notebook-workflows-exit)."
             " Databricks restricts this API to return the first 5 MB of the value. For"
@@ -900,17 +828,15 @@
 
 
 class NotebookTask(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     base_parameters: Optional[Dict[str, Any]] = Field(
         None,
         description=(
             "Base parameters to be used for each run of this job. If the run is"
             " initiated by a call to"
             " [`run-now`](https://docs.databricks.com/dev-tools/api/latest/jobs.html#operation/JobsRunNow)"
@@ -952,56 +878,39 @@
 class ParameterPair(BaseModel):
     """
     See source code for the fields' description.
 
     An object with additional information about why a cluster was terminated. The object keys are one of `TerminationParameter` and the value is the termination information.
     """
 
-    class Config:
-        extra = Extra.allow
+    model_config = ConfigDict(extra="allow", frozen=True)
 
-        allow_mutation = False
 
-
-class PermissionLevel(BaseModel):
+class PermissionLevel(RootModel[Union[CanManage, CanManageRun, CanView, IsOwner]]):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(frozen=True)
 
-    __root__: Union[CanManage, CanManageRun, CanView, IsOwner] = Field(
-        ..., description="Permission level to grant."
-    )
 
-
-class PermissionLevelForGroup(BaseModel):
+class PermissionLevelForGroup(RootModel[Union[CanManage, CanManageRun, CanView]]):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
-
-    __root__: Union[CanManage, CanManageRun, CanView] = Field(
-        ..., description="Permission level to grant."
-    )
+    model_config = ConfigDict(frozen=True)
 
 
 class PipelineTask(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     full_refresh: Optional[bool] = Field(
         False,
         description=(
             "If true, a full refresh will be triggered on the delta live table."
         ),
     )
@@ -1023,17 +932,15 @@
 
 
 class PythonPyPiLibrary(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     package: str = Field(
         ...,
         description=(
             "The name of the PyPI package to install. An optional exact version"
             " specification is also supported. Examples: `simplejson` and"
             " `simplejson==3.8.0`. This field is required."
@@ -1051,17 +958,15 @@
 
 
 class PythonWheelTask(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     entry_point: Optional[str] = Field(
         None,
         description=(
             "Named entry point to use, if it does not exist in the metadata of the"
             " package it executes the function from the package directly using"
             " `$packageName.$entryPoint()`"
@@ -1090,17 +995,15 @@
 
 
 class RCranLibrary(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     package: str = Field(
         ...,
         description="The name of the CRAN package to install. This field is required.",
         example="geojson",
     )
     repo: Optional[str] = Field(
@@ -1114,17 +1017,15 @@
 
 
 class RepairRunInput(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     latest_repair_id: Optional[int] = Field(
         None,
         description=(
             "The ID of the latest repair. This parameter is not required when repairing"
             " a run for the first time, but must be provided on subsequent requests to"
             " repair the same run."
@@ -1187,17 +1088,15 @@
 
 
 class RunNowInput(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     idempotency_token: Optional[str] = Field(
         None,
         description=(
             "An optional token to guarantee the idempotency of job run requests. If a"
             " run with the provided token already exists, the request does not create a"
             " new run but returns the ID of the existing run instead. If a run with the"
@@ -1216,31 +1115,27 @@
 
 
 class PipelineParams(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     full_refresh: Optional[bool] = Field(
         None, description="If true, triggers a full refresh on the delta live table."
     )
 
 
 class RunParameters(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     dbt_commands: Optional[List] = Field(
         None,
         description=(
             "An array of commands to execute for jobs with the dbt task, for example"
             ' `"dbt_commands": ["dbt deps", "dbt seed", "dbt run"]`'
         ),
@@ -1355,17 +1250,15 @@
 class RunState(BaseModel):
     """
     See source code for the fields' description.
 
     The result and lifecycle state of the run.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     life_cycle_state: Optional[RunLifeCycleState] = Field(
         None,
         description=(
             "A description of a run’s current location in the run lifecycle. This field"
             " is always available in the response."
         ),
@@ -1403,17 +1296,15 @@
 
 
 class S3StorageInfo(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     canned_acl: Optional[str] = Field(
         None,
         description=(
             "(Optional) Set canned access control list. For example:"
             " `bucket-owner-full-control`. If canned_acl is set, the cluster instance"
             " profile must have `s3:PutObjectAcl` permission on the destination bucket"
@@ -1461,64 +1352,48 @@
         description=(
             "S3 region. For example: `us-west-2`. Either region or endpoint must be"
             " set. If both are set, endpoint is used."
         ),
     )
 
 
-class ServicePrincipalName(BaseModel):
+class ServicePrincipalName(RootModel[str]):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
-
-    __root__: str = Field(
-        ...,
-        description="Name of an Azure service principal.",
-        example="9f0621ee-b52b-11ea-b3de-0242ac130004",
-    )
+    model_config = ConfigDict(frozen=True)
 
 
 class SparkConfPair(BaseModel):
     """
     See source code for the fields' description.
 
     An arbitrary object where the object key is a configuration property name and the value is a configuration property value.
     """
 
-    class Config:
-        extra = Extra.allow
-
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
 
 class SparkEnvPair(BaseModel):
     """
     See source code for the fields' description.
 
     An arbitrary object where the object key is an environment variable name and the value is an environment variable value.
     """
 
-    class Config:
-        extra = Extra.allow
-
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
 
 class SparkJarTask(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     jar_uri: Optional[str] = Field(
         None,
         deprecated=True,
         description=(
             "Deprecated since 04/2016\\. Provide a `jar` through the `libraries` field"
             " instead. For an example, see"
@@ -1547,31 +1422,27 @@
 
 
 class SparkNodeAwsAttributes(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     is_spot: Optional[bool] = Field(
         None, description="Whether this node is on an Amazon spot instance."
     )
 
 
 class SparkPythonTask(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     parameters: Optional[List[str]] = Field(
         None,
         description=(
             "Command line parameters passed to the Python file.\n\nUse [Task parameter"
             " variables](https://docs.databricks.com/jobs.html#parameter-variables) to"
             " set parameters containing information about job runs."
@@ -1591,17 +1462,15 @@
 
 
 class SparkSubmitTask(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     parameters: Optional[List[str]] = Field(
         None,
         description=(
             "Command-line parameters passed to spark submit.\n\nUse [Task parameter"
             " variables](https://docs.databricks.com/jobs.html#parameter-variables) to"
             " set parameters containing information about job runs."
@@ -1616,17 +1485,15 @@
 
 
 class SparkVersion(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     key: Optional[str] = Field(
         None,
         description=(
             "[Databricks Runtime"
             " version](https://docs.databricks.com/dev-tools/api/latest/index.html#programmatic-version)"
             " key, for example `7.3.x-scala2.12`. The value that must be provided as"
@@ -1645,154 +1512,119 @@
 
 
 class SqlOutputError(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     message: Optional[str] = Field(
         None, description="The error message when execution fails."
     )
 
 
 class SqlStatementOutput(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     lookup_key: Optional[str] = Field(
         None, description="A key that can be used to look up query details."
     )
 
 
 class SqlTaskAlert(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     alert_id: str = Field(..., description="The canonical identifier of the SQL alert.")
 
 
 class SqlTaskDashboard(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     dashboard_id: str = Field(
         ..., description="The canonical identifier of the SQL dashboard."
     )
 
 
 class SqlTaskQuery(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     query_id: str = Field(..., description="The canonical identifier of the SQL query.")
 
 
 class TaskDependency(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     task_key: Optional[str] = None
 
 
-class TaskDependencies(BaseModel):
+class TaskDependencies(List[TaskDependency]):
     """
     See source code for the fields' description.
 
         An optional array of objects specifying the dependency graph of the task. All tasks specified in this field must complete successfully before executing this task.
     The key is `task_key`, and the value is the name assigned to the dependent task.
     This field is required when a job consists of more than one task.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
-
-    __root__: List[TaskDependency] = Field(
-        ...,
-        description=(
-            "An optional array of objects specifying the dependency graph of the task."
-            " All tasks specified in this field must complete successfully before"
-            " executing this task.\nThe key is `task_key`, and the value is the name"
-            " assigned to the dependent task.\nThis field is required when a job"
-            " consists of more than one task."
-        ),
-        example=[{"task_key": "Previous_Task_Key"}, {"task_key": "Other_Task_Key"}],
-    )
+    model_config = ConfigDict(extra="allow", frozen=True)
 
 
-class TaskDescription(BaseModel):
+class TaskDescription(RootModel[str]):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
-
-    __root__: str = Field(
-        ...,
-        description=(
-            "An optional description for this task.\nThe maximum length is 4096 bytes."
-        ),
-        example="This is the description for this task.",
-        max_length=4096,
-    )
-
-
-class TaskKey(BaseModel):
-    """
-    See source code for the fields' description.
-    """
+    model_config = ConfigDict(frozen=True)
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
 
-    __root__: str = Field(
+TaskKeyStr = Annotated[
+    str,
+    Field(
         ...,
         description=(
             "A unique name for the task. This field is used to refer to this task from"
             " other tasks.\nThis field is required and must be unique within its parent"
             " job.\nOn Update or Reset, this field is used to reference the tasks to be"
             " updated or reset.\nThe maximum length is 100 characters."
         ),
-        example="Task_Key",
+        examples=["Task_Key"],
         max_length=100,
         min_length=1,
-        regex="^[\\w\\-]+$",
-    )
+        pattern="^[\\w\\-]+$",
+    ),
+]
+
+
+class TaskKey(RootModel[TaskKeyStr]):
+    """
+    See source code for the fields' description.
+    """
+
+    model_config = ConfigDict(frozen=True)
 
 
 class TerminationCode(str, Enum):
     """
         * USER_REQUEST: A user terminated the cluster directly. Parameters should include a `username` field that indicates the specific user who terminated the cluster.
     * JOB_FINISHED: The cluster was launched by a job, and terminated when the job completed.
     * INACTIVITY: The cluster was terminated since it was idle.
@@ -1840,17 +1672,15 @@
 
 
 class TerminationParameter(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     aws_api_error_code: Optional[str] = Field(
         None,
         description=(
             "The AWS provided error code describing why cluster nodes could not be"
             " provisioned. For example, `InstanceLimitExceeded` indicates that the"
             " limit of EC2 instances for a specific instance type has been exceeded."
@@ -1965,26 +1795,20 @@
     """
 
     periodic = "PERIODIC"
     onetime = "ONE_TIME"
     retry = "RETRY"
 
 
-class UserName(BaseModel):
+class UserName(RootModel[str]):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
-
-    __root__: str = Field(
-        ..., description="Email address for the user.", example="jsmith@example.com"
-    )
+    model_config = ConfigDict(frozen=True)
 
 
 class ViewType(str, Enum):
     """
         * `NOTEBOOK`: Notebook view item.
     * `DASHBOARD`: Dashboard view item.
     """
@@ -2006,53 +1830,45 @@
 
 
 class OnFailureItem(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     id: Optional[str] = None
 
 
 class OnStartItem(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     id: Optional[str] = None
 
 
 class OnSucces(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     id: Optional[str] = None
 
 
 class WebhookNotifications(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     on_failure: Optional[List[OnFailureItem]] = Field(
         None,
         description=(
             "An optional list of notification IDs to call when the run fails. A maximum"
             " of 3 destinations can be specified for the `on_failure` property."
         ),
@@ -2081,56 +1897,48 @@
 
 
 class AccessControlRequestForGroup(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     group_name: Optional[GroupName] = None
     permission_level: Optional[PermissionLevelForGroup] = None
 
 
 class AccessControlRequestForServicePrincipal(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     permission_level: Optional[PermissionLevel] = None
     service_principal_name: Optional[ServicePrincipalName] = None
 
 
 class AccessControlRequestForUser(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     permission_level: Optional[PermissionLevel] = None
     user_name: Optional[UserName] = None
 
 
 class ClusterCloudProviderNodeInfo(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     available_core_quota: Optional[int] = Field(
         None, description="Available CPU core quota."
     )
     status: Optional[ClusterCloudProviderNodeStatus] = Field(
         None, description="Status as reported by the cloud provider."
     )
@@ -2138,17 +1946,15 @@
 
 
 class ClusterLogConf(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     dbfs: Optional[DbfsStorageInfo] = Field(
         None,
         description=(
             "DBFS location of cluster log. Destination must be provided. For example,"
             ' `{ "dbfs" : { "destination" : "dbfs:/home/cluster_log" } }`'
         ),
@@ -2164,17 +1970,15 @@
 
 
 class InitScriptInfo(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     s3: Optional[S3StorageInfo] = Field(
         None,
         alias="S3",
         description=(
             "S3 location of init script. Destination and either region or endpoint must"
             ' be provided. For example, `{ "s3": { "destination" :'
@@ -2198,17 +2002,15 @@
 
 
 class Library(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     cran: Optional[RCranLibrary] = Field(
         None, description="If cran, specification of a CRAN library to be installed."
     )
     egg: Optional[str] = Field(
         None,
         description=(
@@ -2265,17 +2067,15 @@
 
 
 class LibraryFullStatus(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     is_library_for_all_clusters: Optional[bool] = Field(
         None,
         description=(
             "Whether the library was set to be installed on all clusters via the"
             " libraries UI."
         ),
@@ -2296,17 +2096,15 @@
 
 
 class NewCluster(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     autoscale: Optional[AutoScale] = Field(
         None,
         description=(
             "If autoscale, the required parameters to automatically scale clusters up"
             " and down based on load."
         ),
@@ -2473,17 +2271,15 @@
 
 
 class NodeType(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     description: str = Field(
         ...,
         description=(
             "A string description associated with this node type. This field is"
             " required."
         ),
@@ -2525,17 +2321,15 @@
 
 
 class RepairHistoryItem(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     end_time: Optional[int] = Field(
         None, description="The end time of the (repaired) run.", example=1625060863413
     )
     id: Optional[int] = Field(
         None,
         description=(
@@ -2565,17 +2359,15 @@
 
 
 class SparkNode(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     host_private_ip: Optional[str] = Field(
         None, description="The private IP address of the host instance."
     )
     instance_id: Optional[str] = Field(
         None,
         description=(
@@ -2611,17 +2403,15 @@
 
 
 class SqlAlertOutput(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     output_link: Optional[str] = Field(
         None, description="The link to find the output results."
     )
     query_text: Optional[str] = Field(
         None,
         description=(
@@ -2638,17 +2428,15 @@
 
 
 class SqlDashboardWidgetOutput(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     end_time: Optional[int] = Field(
         None,
         description=(
             "Time (in epoch milliseconds) when execution of the SQL widget ends."
         ),
     )
@@ -2676,17 +2464,15 @@
 
 
 class SqlQueryOutput(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     output_link: Optional[str] = Field(
         None, description="The link to find the output results."
     )
     query_text: Optional[str] = Field(
         None,
         description=(
@@ -2703,17 +2489,15 @@
 
 
 class SqlTask(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     alert: Optional[SqlTaskAlert] = Field(
         None, description="If alert, indicates that this job must refresh a SQL alert."
     )
     dashboard: Optional[SqlTaskDashboard] = Field(
         None,
         description=(
@@ -2741,17 +2525,15 @@
 
 
 class TerminationReason(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     code: Optional[TerminationCode] = Field(
         None, description="Status code indicating why a cluster was terminated."
     )
     parameters: Optional[ParameterPair] = Field(
         None,
         description=(
@@ -2765,17 +2547,15 @@
 
 
 class ViewItem(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     content: Optional[str] = Field(None, description="Content of the view.")
     name: Optional[str] = Field(
         None,
         description=(
             "Name of the view item. In the case of code view, it would be the"
             " notebook’s name. In the case of dashboard view, it would be the"
@@ -2786,27 +2566,23 @@
 
 
 class AccessControlRequest(AccessControlRequestForUser, AccessControlRequestForGroup):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
 
 class ClusterAttributes(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     autotermination_minutes: Optional[int] = Field(
         None,
         description=(
             "Automatically terminates the cluster after it is inactive for this time in"
             " minutes. If not set, this cluster is not be automatically terminated. If"
             " specified, the threshold must be between 10 and 10000 minutes. You can"
@@ -2970,17 +2746,15 @@
 
 
 class ClusterInfo(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     autoscale: Optional[AutoScale] = Field(
         None,
         description=(
             "If autoscale, parameters needed in order to automatically scale clusters"
             " up and down based on load."
         ),
@@ -3264,34 +3038,30 @@
 
 
 class ClusterLibraryStatuses(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     cluster_id: Optional[str] = Field(
         None, description="Unique identifier for the cluster."
     )
     library_statuses: Optional[List[LibraryFullStatus]] = Field(
         None, description="Status of all libraries on the cluster."
     )
 
 
 class ClusterSpec(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     existing_cluster_id: Optional[str] = Field(
         None,
         description=(
             "If existing_cluster_id, the ID of an existing cluster that is used for all"
             " runs of this job. When running jobs on an existing cluster, you may need"
             " to manually restart the cluster if it stops responding. We suggest"
@@ -3315,17 +3085,15 @@
 
 
 class EventDetails(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     attributes: Optional[AwsAttributes] = Field(
         None,
         description=(
             "* For created clusters, the attributes of the cluster.\n* For edited"
             " clusters, the new attributes of the cluster."
         ),
@@ -3367,41 +3135,37 @@
 
 
 class JobCluster(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     job_cluster_key: str = Field(
         ...,
         description=(
             "A unique name for the job cluster. This field is required and must be"
             " unique within the job.\n`JobTaskSettings` may refer to this field to"
             " determine which cluster to launch for the task execution."
         ),
-        example="auto_scaling_cluster",
+        examples=["auto_scaling_cluster"],
         max_length=100,
         min_length=1,
-        regex="^[\\w\\-]+$",
+        pattern="^[\\w\\-]+$",
     )
     new_cluster: Optional[NewCluster] = None
 
 
 class JobTask(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     dbt_task: Optional[DbtTask] = Field(
         None,
         description=(
             "If dbt_task, indicates that this must execute a dbt task. It requires both"
             " Databricks SQL and the ability to use a serverless or a pro SQL"
             " warehouse."
@@ -3454,17 +3218,15 @@
 
 
 class JobTaskSettings(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True, arbitrary_types_allowed=True)
 
     dbt_task: Optional[DbtTask] = Field(
         None,
         description=(
             "If dbt_task, indicates that this must execute a dbt task. It requires both"
             " Databricks SQL and the ability to use a serverless or a pro SQL"
             " warehouse."
@@ -3494,15 +3256,15 @@
         None,
         description=(
             "If job_cluster_key, this task is executed reusing the cluster specified in"
             " `job.settings.job_clusters`."
         ),
         max_length=100,
         min_length=1,
-        regex="^[\\w\\-]+$",
+        pattern="^[\\w\\-]+$",
     )
     libraries: Optional[List[Library]] = Field(
         None,
         description=(
             "An optional list of libraries to be installed on the cluster that executes"
             " the task. The default value is an empty list."
         ),
@@ -3602,31 +3364,27 @@
 
 
 class RepairHistory(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     repair_history: Optional[List[RepairHistoryItem]] = Field(
         None, description="The repair history of the run."
     )
 
 
 class RunSubmitTaskSettings(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True, arbitrary_types_allowed=True)
 
     dbt_task: Optional[DbtTask] = Field(
         None,
         description=(
             "If dbt_task, indicates that this must execute a dbt task. It requires both"
             " Databricks SQL and the ability to use a serverless or a pro SQL"
             " warehouse."
@@ -3710,17 +3468,15 @@
 
 
 class RunTask(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True, arbitrary_types_allowed=True)
 
     attempt_number: Optional[int] = Field(
         None,
         description=(
             "The sequence number of this run attempt for a triggered job run. The"
             " initial attempt of a run has an attempt_number of 0\\. If the initial run"
             " attempt fails, and the job has a retry policy (`max_retries` \\> 0),"
@@ -3881,34 +3637,30 @@
 
 
 class SqlDashboardOutput(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     widgets: Optional[SqlDashboardWidgetOutput] = Field(
         None,
         description=(
             "Widgets executed in the run. Only SQL query based widgets are listed."
         ),
     )
 
 
 class SqlOutput(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     alert_output: Optional[SqlAlertOutput] = Field(
         None, description="The output of a SQL alert task, if available."
     )
     dashboard_output: Optional[SqlDashboardOutput] = Field(
         None, description="The output of a SQL dashboard task, if available."
     )
@@ -3918,31 +3670,27 @@
 
 
 class AccessControlList(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     access_control_list: Optional[List[AccessControlRequest]] = Field(
         None, description="List of permissions to set on the job."
     )
 
 
 class ClusterEvent(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     cluster_id: str = Field(
         ..., description="Canonical identifier for the cluster. This field is required."
     )
     details: EventDetails = Field(
         ..., description="The event details. This field is required."
     )
@@ -3959,17 +3707,15 @@
 
 
 class JobSettings(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     email_notifications: Optional[JobEmailNotifications] = Field(
         None,
         description=(
             "An optional set of email addresses that is notified when runs of this job"
             " begin or complete as well as when this job is deleted. The default"
             " behavior is to not send any emails."
@@ -4012,15 +3758,15 @@
                     "aws_attributes": {"availability": "SPOT", "zone_id": "us-west-2a"},
                     "node_type_id": "i3.xlarge",
                     "spark_conf": {"spark.speculation": True},
                     "spark_version": "7.3.x-scala2.12",
                 },
             }
         ],
-        max_items=100,
+        max_length=100,
     )
     max_concurrent_runs: Optional[int] = Field(
         None,
         description=(
             "An optional maximum allowed number of concurrent runs of the job.\n\nSet"
             " this value if you want to be able to execute multiple runs of the same"
             " job concurrently. This is useful for example if you trigger your job on a"
@@ -4114,15 +3860,15 @@
                     "source": "WORKSPACE",
                 },
                 "retry_on_timeout": False,
                 "task_key": "Match",
                 "timeout_seconds": 86400,
             },
         ],
-        max_items=100,
+        max_length=100,
     )
     timeout_seconds: Optional[int] = Field(
         None,
         description=(
             "An optional timeout applied to each run of this job. The default behavior"
             " is to have no timeout."
         ),
@@ -4139,17 +3885,15 @@
 
 
 class Run(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     attempt_number: Optional[int] = Field(
         None,
         description=(
             "The sequence number of this run attempt for a triggered job run. The"
             " initial attempt of a run has an attempt_number of 0\\. If the initial run"
             " attempt fails, and the job has a retry policy (`max_retries` \\> 0),"
@@ -4236,15 +3980,15 @@
                     "aws_attributes": {"availability": "SPOT", "zone_id": "us-west-2a"},
                     "node_type_id": "i3.xlarge",
                     "spark_conf": {"spark.speculation": True},
                     "spark_version": "7.3.x-scala2.12",
                 },
             }
         ],
-        max_items=100,
+        max_length=100,
     )
     job_id: Optional[int] = Field(
         None,
         description="The canonical identifier of the job that contains this run.",
         example=11223344,
     )
     number_in_job: Optional[int] = Field(
@@ -4419,29 +4163,27 @@
                         " libraries on a cluster"
                     ),
                     "user_cancelled_or_timedout": False,
                 },
                 "task_key": "Sessionize",
             },
         ],
-        max_items=100,
+        max_length=100,
     )
     trigger: Optional[TriggerType] = Field(
         None, description="The type of trigger that fired this run."
     )
 
 
 class RunSubmitSettings(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     git_source: Optional[GitSource1] = Field(
         None,
         description=(
             "This functionality is in Public Preview.\n\nAn optional specification for"
             " a remote repository containing the notebooks used by this job's notebook"
             " tasks."
@@ -4517,15 +4259,15 @@
                     "notebook_path": "/Users/user.name@databricks.com/Match",
                     "source": "WORKSPACE",
                 },
                 "task_key": "Match",
                 "timeout_seconds": 86400,
             },
         ],
-        max_items=100,
+        max_length=100,
     )
     timeout_seconds: Optional[int] = Field(
         None,
         description=(
             "An optional timeout applied to each run of this job. The default behavior"
             " is to have no timeout."
         ),
@@ -4542,17 +4284,15 @@
 
 
 class Job(BaseModel):
     """
     See source code for the fields' description.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     created_time: Optional[int] = Field(
         None,
         description=(
             "The time at which this job was created in epoch milliseconds (milliseconds"
             " since 1/1/1970 UTC)."
         ),
```

### Comparing `prefect_databricks-0.2.7/prefect_databricks/rest.py` & `prefect_databricks-0.3.0rc1/prefect_databricks/rest.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,27 +6,15 @@
 # manually editing this file is not recommended.
 
 import json
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 import httpx
-
-from prefect._internal.pydantic import HAS_PYDANTIC_V2
-from prefect._internal.pydantic._compat import model_dump
-
-if HAS_PYDANTIC_V2:
-    from pydantic import BaseModel as V2BaseModel
-    from pydantic.v1 import BaseModel
-
-    MODELS = (BaseModel, V2BaseModel)
-else:
-    from pydantic import BaseModel
-
-    MODELS = BaseModel
+from pydantic import BaseModel
 
 from prefect import task
 
 if TYPE_CHECKING:
     from prefect_databricks import DatabricksCredentials
 
 
@@ -54,16 +42,16 @@
         Serialized version of object.
     """
     if isinstance(obj, list):
         return [serialize_model(o) for o in obj]
     elif isinstance(obj, Dict):
         return {k: serialize_model(v) for k, v in obj.items()}
 
-    if isinstance(obj, MODELS):
-        return model_dump(obj, mode="json")
+    if isinstance(obj, BaseModel):
+        return obj.model_dump(mode="json")
     elif isinstance(obj, Enum):
         return obj.value
     return obj
 
 
 def strip_kwargs(**kwargs: Dict) -> Dict:
     """
```

### Comparing `prefect_databricks-0.2.7/prefect_databricks/schemas/jobs-2.1-aws.yaml` & `prefect_databricks-0.3.0rc1/prefect_databricks/schemas/jobs-2.1-aws.yaml`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.7/prefect_databricks/schemas/original/jobs-2.1-aws.yaml` & `prefect_databricks-0.3.0rc1/prefect_databricks/schemas/original/jobs-2.1-aws.yaml`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.7/prefect_databricks.egg-info/PKG-INFO` & `prefect_databricks-0.3.0rc1/prefect_databricks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 Metadata-Version: 2.1
 Name: prefect-databricks
-Version: 0.2.7
+Version: 0.3.0rc1
 Summary: Prefect integrations with Databricks
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-databricks
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
 Requires-Dist: respx; extra == "dev"
```

### Comparing `prefect_databricks-0.2.7/prefect_databricks.egg-info/SOURCES.txt` & `prefect_databricks-0.3.0rc1/prefect_databricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.7/pyproject.toml` & `prefect_databricks-0.3.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,43 +2,41 @@
 requires = ["setuptools>=45", "wheel", "setuptools_scm>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prefect-databricks"
 description = "Prefect integrations with Databricks"
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
   "respx",
@@ -49,15 +47,15 @@
 
 [project.entry-points."prefect.collections"]
 prefect_databricks = "prefect_databricks"
 
 [tool.setuptools_scm]
 version_file = "prefect_databricks/_version.py"
 root = "../../.."
-tag_regex = "^prefect-databricks-(?P<version>\\d+\\.\\d+\\.\\d+)$"
+tag_regex = "^prefect-databricks-(?P<version>\\d+\\.\\d+\\.\\d+(?:[a-zA-Z0-9]+(?:\\.[a-zA-Z0-9]+)*)?)$"
 fallback_version = "0.0.0"
 git_describe_command = 'git describe --dirty --tags --long --match "prefect-databricks-*[0-9]*"'
 
 [tool.interrogate]
 ignore-init-module = true
 ignore_init_method = true
 exclude = ["prefect_databricks/_version.py", "tests"]
```

### Comparing `prefect_databricks-0.2.7/tests/mock_schema.yaml` & `prefect_databricks-0.3.0rc1/tests/mock_schema.yaml`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.7/tests/test_block_standards.py` & `prefect_databricks-0.3.0rc1/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.7/tests/test_flows.py` & `prefect_databricks-0.3.0rc1/tests/test_flows.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.7/tests/test_generate.py` & `prefect_databricks-0.3.0rc1/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.7/tests/test_jobs.py` & `prefect_databricks-0.3.0rc1/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.7/tests/test_rest.py` & `prefect_databricks-0.3.0rc1/tests/test_rest.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from prefect_databricks import DatabricksCredentials
 from prefect_databricks.rest import (
     HTTPMethod,
     execute_endpoint,
     serialize_model,
     strip_kwargs,
 )
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel, ConfigDict
 
 
 @pytest.mark.parametrize("params", [dict(a="A", b="B"), None])
 @pytest.mark.parametrize("http_method", ["get", HTTPMethod.GET, "post"])
 async def test_execute_endpoint(params, http_method, respx_mock):
     url = "https://prefect.io/"
 
@@ -44,17 +44,15 @@
 
 class TestAnotherBaseModel(BaseModel):
     some_float: float
     some_bool: bool
 
 
 class TestBaseModel(BaseModel):
-    class Config:
-        extra = Extra.allow
-        allow_mutation = False
+    model_config = ConfigDict(extra="allow", frozen=True)
 
     some_string: str
     some_int: int
     another_base_model: TestAnotherBaseModel
     other_base_models: List[TestAnotherBaseModel]
```

