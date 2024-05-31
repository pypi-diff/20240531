# Comparing `tmp/analytic_workbench_clients-0.6.1-py3-none-any.whl.zip` & `tmp/analytic_workbench_clients-0.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7387 bytes, number of entries: 11
--rw-r--r--  2.0 unx      428 b- defN 24-May-24 11:15 analytic_workbench_clients/__init__.py
+Zip file size: 7401 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      428 b- defN 24-May-29 09:06 analytic_workbench_clients/__init__.py
 -rw-r--r--  2.0 unx     1417 b- defN 24-Mar-11 11:09 analytic_workbench_clients/cache_store_client.py
--rw-r--r--  2.0 unx     5516 b- defN 24-Mar-11 11:09 analytic_workbench_clients/job_client.py
+-rw-r--r--  2.0 unx     5567 b- defN 24-May-29 09:06 analytic_workbench_clients/job_client.py
 -rw-r--r--  2.0 unx     1302 b- defN 23-Oct-23 08:40 analytic_workbench_clients/methods_client.py
 -rw-r--r--  2.0 unx     1968 b- defN 24-Mar-11 11:09 analytic_workbench_clients/models.py
 -rw-r--r--  2.0 unx     1231 b- defN 23-Oct-23 08:40 analytic_workbench_clients/resource_client.py
--rw-rw-rw-  2.0 unx      575 b- defN 24-May-24 15:31 analytic_workbench_clients-0.6.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      892 b- defN 24-May-24 15:31 analytic_workbench_clients-0.6.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-24 15:31 analytic_workbench_clients-0.6.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       27 b- defN 24-May-24 15:31 analytic_workbench_clients-0.6.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1075 b- defN 24-May-24 15:31 analytic_workbench_clients-0.6.1.dist-info/RECORD
-11 files, 14523 bytes uncompressed, 5511 bytes compressed:  62.1%
+-rw-rw-rw-  2.0 unx      575 b- defN 24-May-31 09:03 analytic_workbench_clients-0.7.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      892 b- defN 24-May-31 09:03 analytic_workbench_clients-0.7.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-31 09:03 analytic_workbench_clients-0.7.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       27 b- defN 24-May-31 09:03 analytic_workbench_clients-0.7.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1075 b- defN 24-May-31 09:03 analytic_workbench_clients-0.7.0.dist-info/RECORD
+11 files, 14574 bytes uncompressed, 5525 bytes compressed:  62.1%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: analytic_workbench_clients/models.py
 Comment: 
 
 Filename: analytic_workbench_clients/resource_client.py
 Comment: 
 
-Filename: analytic_workbench_clients-0.6.1.dist-info/LICENSE.txt
+Filename: analytic_workbench_clients-0.7.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: analytic_workbench_clients-0.6.1.dist-info/METADATA
+Filename: analytic_workbench_clients-0.7.0.dist-info/METADATA
 Comment: 
 
-Filename: analytic_workbench_clients-0.6.1.dist-info/WHEEL
+Filename: analytic_workbench_clients-0.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: analytic_workbench_clients-0.6.1.dist-info/top_level.txt
+Filename: analytic_workbench_clients-0.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: analytic_workbench_clients-0.6.1.dist-info/RECORD
+Filename: analytic_workbench_clients-0.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## analytic_workbench_clients/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.1"
+__version__ = "0.7.0"
 
 __all__ = [
     "AWResourcesClient",
     "AWJobsClient",
     "AWCacheStoreClient",
     "MethodsClient",
     "JobModel",
```

## analytic_workbench_clients/job_client.py

```diff
@@ -1,11 +1,12 @@
 import time
 from typing import Any, Callable, Generator, List, Union
 from uuid import UUID
 
+from clients_core import JsonPatchModel
 from clients_core.exceptions import ClientValueError  # noqa: F401
 from clients_core.service_clients import E360ServiceClient
 from pydantic import parse_obj_as
 
 from .models import (
     JobCreateModel,
     JobModel,
@@ -51,20 +52,20 @@
     def get_by_id(self, job_id: UUID, **kwargs: Any) -> JobModel:
         url = f"{job_id}/"
         response = self.client.get(
             url, headers=self.service_headers, raises=True, **kwargs
         )
         return JobModel.parse_obj(response.json())
 
-    def modify(self, job_id: UUID, patches: List[dict], **kwargs: Any) -> JobModel:
+    def modify(self, job_id: UUID, patches: JsonPatchModel, **kwargs: Any) -> JobModel:
         """Performs a patch method on an existing job id with a patch document"""
         url = f"{self.service_endpoint}/{job_id}/"
         response = self.client.patch(
             url,
-            json=patches,
+            json=patches.dump(),
             headers=self.service_headers,
             raises=True,
             **kwargs,
         )
         return JobModel.parse_obj(response.json())
 
     def update(self, job_id: UUID, model: JobCreateModel, **kwargs: Any) -> JobModel:
```

## Comparing `analytic_workbench_clients-0.6.1.dist-info/LICENSE.txt` & `analytic_workbench_clients-0.7.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `analytic_workbench_clients-0.6.1.dist-info/METADATA` & `analytic_workbench_clients-0.7.0.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: analytic_workbench_clients
-Version: 0.6.1
+Version: 0.7.0
 Summary: E360 Analytic Workbench Clients for Python
 Author: IQVIA
 Author-email: e360pypi@iqvia.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

