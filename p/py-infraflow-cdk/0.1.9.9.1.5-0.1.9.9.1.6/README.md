# Comparing `tmp/py_infraflow_cdk-0.1.9.9.1.5.tar.gz` & `tmp/py_infraflow_cdk-0.1.9.9.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_infraflow_cdk-0.1.9.9.1.5.tar", max compression
+gzip compressed data, was "py_infraflow_cdk-0.1.9.9.1.6.tar", max compression
```

## Comparing `py_infraflow_cdk-0.1.9.9.1.5.tar` & `py_infraflow_cdk-0.1.9.9.1.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      337 2024-01-24 18:03:42.816211 py_infraflow_cdk-0.1.9.9.1.5/README.md
--rw-r--r--   0        0        0        0 2024-01-22 17:24:55.856613 py_infraflow_cdk-0.1.9.9.1.5/infraflow/__init__.py
--rw-r--r--   0        0        0      240 2024-01-22 17:24:55.856719 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/__init__.py
--rw-r--r--   0        0        0        0 2024-01-22 17:24:55.856794 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/_step_functions/__init__.py
--rw-r--r--   0        0        0     1329 2024-01-22 17:24:55.856883 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/_step_functions/core.py
--rw-r--r--   0        0        0     1261 2024-01-22 17:24:55.856942 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/_step_functions/patterns.py
--rw-r--r--   0        0        0      280 2024-01-22 17:24:55.857004 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/api_gateway.py
--rw-r--r--   0        0        0     7399 2024-05-22 22:22:01.944518 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/app_patterns/express_default_dlq_processor.py
--rw-r--r--   0        0        0    12829 2024-05-22 22:26:07.349206 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/app_patterns/standard.py
--rw-r--r--   0        0        0      156 2024-01-22 17:24:55.857163 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/arns.py
--rw-r--r--   0        0        0        0 2024-01-22 17:24:55.857224 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/core/__init__.py
--rw-r--r--   0        0        0      364 2024-01-22 17:24:55.857292 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/core/component_service.py
--rw-r--r--   0        0        0      316 2024-01-22 17:24:55.857349 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/core/construct.py
--rw-r--r--   0        0        0     5168 2024-03-20 16:31:56.831033 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/core/environment.py
--rw-r--r--   0        0        0     1020 2024-01-24 18:03:42.816662 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/core/service_stage.py
--rw-r--r--   0        0        0      367 2024-02-19 16:57:57.498391 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/core/utils.py
--rw-r--r--   0        0        0    10397 2024-05-08 20:06:25.481166 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/docker.py
--rw-r--r--   0        0        0     9235 2024-05-10 16:52:15.747978 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/events.py
--rw-r--r--   0        0        0      139 2024-01-22 17:24:55.857712 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/iam/__init__.py
--rw-r--r--   0        0        0   533095 2024-01-24 18:03:42.817968 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/iam/_actions.py
--rw-r--r--   0        0        0   249582 2024-01-22 17:24:55.859417 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/iam/action_groups.py
--rw-r--r--   0        0        0   108710 2024-01-22 17:24:55.859750 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/iam/actions
--rw-r--r--   0        0        0     4943 2024-01-22 17:24:55.859832 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/iam/base.py
--rw-r--r--   0        0        0        0 2024-03-20 16:31:56.831151 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/instrumentation/__init__.py
--rw-r--r--   0        0        0     1376 2024-04-11 23:31:09.973506 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/instrumentation/alarms.py
--rw-r--r--   0        0        0     5976 2024-04-24 21:59:03.929389 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/instrumentation/docker.py
--rw-r--r--   0        0        0     7347 2024-04-25 19:01:22.356096 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/instrumentation/lambdas.py
--rw-r--r--   0        0        0     1704 2024-04-11 23:31:09.974803 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/instrumentation/metrics.py
--rw-r--r--   0        0        0     4435 2024-04-11 23:31:09.975272 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/instrumentation/queues.py
--rw-r--r--   0        0        0     6529 2024-05-22 23:00:52.247334 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/lambdas.py
--rw-r--r--   0        0        0      349 2024-02-28 20:32:26.259456 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/queue.py
--rw-r--r--   0        0        0        0 2024-01-22 17:24:55.859986 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/sg/__init__.py
--rw-r--r--   0        0        0     3481 2024-01-24 18:03:42.818220 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/sg/patterns.py
--rw-r--r--   0        0        0      715 2024-01-24 18:03:42.818283 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/sg/ports.py
--rw-r--r--   0        0        0      629 2024-01-22 17:24:55.860118 py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/sg/tier_maps.py
--rw-r--r--   0        0        0      141 2024-01-24 18:03:42.818392 py_infraflow_cdk-0.1.9.9.1.5/infraflow/priv_utils/__init__.py
--rw-r--r--   0        0        0      154 2024-01-22 17:24:55.860264 py_infraflow_cdk-0.1.9.9.1.5/infraflow/util.py
--rw-r--r--   0        0        0      687 2024-05-22 23:01:15.530052 py_infraflow_cdk-0.1.9.9.1.5/pyproject.toml
--rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 py_infraflow_cdk-0.1.9.9.1.5/PKG-INFO
+-rw-r--r--   0        0        0      337 2024-01-24 18:03:42.816211 py_infraflow_cdk-0.1.9.9.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-01-22 17:24:55.856613 py_infraflow_cdk-0.1.9.9.1.6/infraflow/__init__.py
+-rw-r--r--   0        0        0      240 2024-01-22 17:24:55.856719 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-22 17:24:55.856794 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/_step_functions/__init__.py
+-rw-r--r--   0        0        0     1329 2024-01-22 17:24:55.856883 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/_step_functions/core.py
+-rw-r--r--   0        0        0     1261 2024-01-22 17:24:55.856942 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/_step_functions/patterns.py
+-rw-r--r--   0        0        0      280 2024-01-22 17:24:55.857004 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/api_gateway.py
+-rw-r--r--   0        0        0     7399 2024-05-22 22:22:01.944518 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/app_patterns/express_default_dlq_processor.py
+-rw-r--r--   0        0        0    12981 2024-05-29 20:26:00.919576 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/app_patterns/standard.py
+-rw-r--r--   0        0        0      156 2024-01-22 17:24:55.857163 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/arns.py
+-rw-r--r--   0        0        0        0 2024-01-22 17:24:55.857224 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/core/__init__.py
+-rw-r--r--   0        0        0      364 2024-01-22 17:24:55.857292 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/core/component_service.py
+-rw-r--r--   0        0        0      316 2024-01-22 17:24:55.857349 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/core/construct.py
+-rw-r--r--   0        0        0     5168 2024-03-20 16:31:56.831033 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/core/environment.py
+-rw-r--r--   0        0        0     1020 2024-01-24 18:03:42.816662 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/core/service_stage.py
+-rw-r--r--   0        0        0      367 2024-02-19 16:57:57.498391 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/core/utils.py
+-rw-r--r--   0        0        0    10486 2024-05-31 20:48:36.978901 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/docker.py
+-rw-r--r--   0        0        0     9235 2024-05-10 16:52:15.747978 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/events.py
+-rw-r--r--   0        0        0      139 2024-01-22 17:24:55.857712 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/iam/__init__.py
+-rw-r--r--   0        0        0   533095 2024-01-24 18:03:42.817968 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/iam/_actions.py
+-rw-r--r--   0        0        0   249582 2024-01-22 17:24:55.859417 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/iam/action_groups.py
+-rw-r--r--   0        0        0   108710 2024-01-22 17:24:55.859750 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/iam/actions
+-rw-r--r--   0        0        0     4943 2024-01-22 17:24:55.859832 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/iam/base.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:31:56.831151 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/instrumentation/__init__.py
+-rw-r--r--   0        0        0     1376 2024-04-11 23:31:09.973506 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/instrumentation/alarms.py
+-rw-r--r--   0        0        0     5976 2024-04-24 21:59:03.929389 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/instrumentation/docker.py
+-rw-r--r--   0        0        0     7347 2024-04-25 19:01:22.356096 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/instrumentation/lambdas.py
+-rw-r--r--   0        0        0     1704 2024-04-11 23:31:09.974803 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/instrumentation/metrics.py
+-rw-r--r--   0        0        0     4435 2024-04-11 23:31:09.975272 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/instrumentation/queues.py
+-rw-r--r--   0        0        0     6482 2024-05-22 23:33:23.263873 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/lambdas.py
+-rw-r--r--   0        0        0      349 2024-02-28 20:32:26.259456 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/queue.py
+-rw-r--r--   0        0        0        0 2024-01-22 17:24:55.859986 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/sg/__init__.py
+-rw-r--r--   0        0        0     3481 2024-01-24 18:03:42.818220 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/sg/patterns.py
+-rw-r--r--   0        0        0      715 2024-01-24 18:03:42.818283 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/sg/ports.py
+-rw-r--r--   0        0        0      629 2024-01-22 17:24:55.860118 py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/sg/tier_maps.py
+-rw-r--r--   0        0        0      141 2024-01-24 18:03:42.818392 py_infraflow_cdk-0.1.9.9.1.6/infraflow/priv_utils/__init__.py
+-rw-r--r--   0        0        0      154 2024-01-22 17:24:55.860264 py_infraflow_cdk-0.1.9.9.1.6/infraflow/util.py
+-rw-r--r--   0        0        0      687 2024-05-31 20:49:19.576092 py_infraflow_cdk-0.1.9.9.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 py_infraflow_cdk-0.1.9.9.1.6/PKG-INFO
```

### Comparing `py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/_step_functions/core.py` & `py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/_step_functions/core.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/_step_functions/patterns.py` & `py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/_step_functions/patterns.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/app_patterns/express_default_dlq_processor.py` & `py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/app_patterns/express_default_dlq_processor.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/app_patterns/standard.py` & `py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/app_patterns/standard.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,18 @@
 
     def use_lambda(self):
         ## allow lambda access to build EC2 network interface
         self.app_role.add_managed_policy(
             self.managed_policy("LambdaAllowENIManagement", name="AWSLambdaENIManagementAccess")
         )
 
+        self.app_role.add_managed_policy(
+            self.managed_policy("AWSLambdaBasicExecutionRole", name="AWSLambdaBasicExecutionRole")
+        )
+
         self._lambda_context = self._lambda_context or LambdaContext(
             self,
             path=self.src_path,
             role=self.app_role,
             runtime=self.python_version,
             excluded_code=self.excluded_code
         )
```

### Comparing `py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/core/environment.py` & `py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/core/environment.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/core/service_stage.py` & `py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/core/service_stage.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/docker.py` & `py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,18 @@
         self.cpu = cpu
 
 
 class ContainerImage:
     def __init__(
             self,
             path=None,
+            dockerfile=None,
             ecr_image=None,
     ):
+        self.dockerfile = dockerfile
         self.ecr_image = ecr_image
         self.path = path
 
 
 class ContainerInstanceInfo:
     def __init__(
             self,
@@ -78,15 +80,15 @@
 
         self.cluster = ecs.Cluster(self.scope, cluster_name, vpc=vpc)
         self.queue_instrumentation: dict[sqs.IQueue, QueueInstrumentation] = {}
         self.service_instrumentation: dict[ecs.FargateService, EcsServiceInstrumentation] = {}
 
     def get_image(self, image: ContainerImage, name):
         if image.path:
-            image_asset = assets.DockerImageAsset(self.scope, f"{name}_image", directory=image.path)
+            image_asset = assets.DockerImageAsset(self.scope, f"{name}_image", directory=image.path, file=image.dockerfile)
             local_image = ecs.ContainerImage.from_docker_image_asset(image_asset)
         else:
             local_image = None
         cdk_image = ecs.ContainerImage.from_registry(
             image.ecr_image) if image.ecr_image else local_image if image.path else None
         return cdk_image
```

### Comparing `py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/events.py` & `py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/events.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/iam/_actions.py` & `py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/iam/_actions.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/iam/action_groups.py` & `py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/iam/action_groups.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/iam/actions` & `py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/iam/actions`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/iam/base.py` & `py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/iam/base.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/instrumentation/alarms.py` & `py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/instrumentation/alarms.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/instrumentation/docker.py` & `py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/instrumentation/docker.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/instrumentation/lambdas.py` & `py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/instrumentation/lambdas.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/instrumentation/metrics.py` & `py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/instrumentation/metrics.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/instrumentation/queues.py` & `py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/instrumentation/queues.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/lambdas.py` & `py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/lambdas.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             timeout: Union[datetime.timedelta, Duration, int]=datetime.timedelta(minutes=5)
     ):
         constructed_name = self.construct_name(handler, name, suffix)
         func = aws_lambda.Function(
                 id=constructed_name,
                 handler=handler,
                 scope=scope_override or self.stage,
-                code=aws_lambda.Code.from_asset(path=self.path, exclude=self.excluded_code), ## TODO SH here we can have an exclude pattern
+                code=aws_lambda.Code.from_asset(path=self.path, exclude=self.excluded_code),
                 runtime=self.runtime,
                 reserved_concurrent_executions=max_concurrency,
                 timeout=to_duration(timeout),
                 security_groups=[
                     self.stage.security_groups.get_group(target=SecurityGroupTarget(
                         scope_override or self.stage,
                         id=constructed_name,
```

### Comparing `py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/sg/patterns.py` & `py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/sg/patterns.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/sg/ports.py` & `py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/sg/ports.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.5/infraflow/cdk/sg/tier_maps.py` & `py_infraflow_cdk-0.1.9.9.1.6/infraflow/cdk/sg/tier_maps.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.9.1.5/pyproject.toml` & `py_infraflow_cdk-0.1.9.9.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-infraflow-cdk"
-version = "0.1.9.9.1.5"
+version = "0.1.9.9.1.6"
 description = "Build Event Based and Microservice infrastructure and connections using these reusable AWS CDK patterns"
 authors = ["Matthew Beatty <infraflow@upcontent.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "infraflow"}]
 
 [tool.poetry.dependencies]
```

### Comparing `py_infraflow_cdk-0.1.9.9.1.5/PKG-INFO` & `py_infraflow_cdk-0.1.9.9.1.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-infraflow-cdk
-Version: 0.1.9.9.1.5
+Version: 0.1.9.9.1.6
 Summary: Build Event Based and Microservice infrastructure and connections using these reusable AWS CDK patterns
 License: MIT
 Author: Matthew Beatty
 Author-email: infraflow@upcontent.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

