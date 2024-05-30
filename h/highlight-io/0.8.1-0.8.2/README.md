# Comparing `tmp/highlight_io-0.8.1.tar.gz` & `tmp/highlight_io-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highlight_io-0.8.1.tar", max compression
+gzip compressed data, was "highlight_io-0.8.2.tar", max compression
```

## Comparing `highlight_io-0.8.1.tar` & `highlight_io-0.8.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1340 2024-05-08 02:00:56.630477 highlight_io-0.8.1/README.md
--rw-r--r--   0        0        0       80 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/__init__.py
--rw-r--r--   0        0        0     1402 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/__init__.py
--rw-r--r--   0        0        0     1950 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/all.py
--rw-r--r--   0        0        0      278 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/anthropic.py
--rw-r--r--   0        0        0      717 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/aws.py
--rw-r--r--   0        0        0      740 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/azure.py
--rw-r--r--   0        0        0      268 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/bedrock.py
--rw-r--r--   0        0        0      253 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/boto.py
--rw-r--r--   0        0        0      273 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/boto3sqs.py
--rw-r--r--   0        0        0      263 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/celery.py
--rw-r--r--   0        0        0      269 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/chromadb.py
--rw-r--r--   0        0        0      263 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/cohere.py
--rw-r--r--   0        0        0     1871 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/django.py
--rw-r--r--   0        0        0     2192 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/fastapi.py
--rw-r--r--   0        0        0     1648 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/flask.py
--rw-r--r--   0        0        0      747 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/gcp.py
--rw-r--r--   0        0        0      273 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/haystack.py
--rw-r--r--   0        0        0      278 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/langchain.py
--rw-r--r--   0        0        0      283 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/llamaindex.py
--rw-r--r--   0        0        0      263 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/openai.py
--rw-r--r--   0        0        0      273 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/pinecone.py
--rw-r--r--   0        0        0      267 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/qdrant.py
--rw-r--r--   0        0        0      258 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/redis.py
--rw-r--r--   0        0        0      278 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/replicate.py
--rw-r--r--   0        0        0      273 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/requests.py
--rw-r--r--   0        0        0     1094 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/serverless.py
--rw-r--r--   0        0        0      283 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/sqlalchemy.py
--rw-r--r--   0        0        0      293 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/transformers.py
--rw-r--r--   0        0        0      273 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/vertexai.py
--rw-r--r--   0        0        0      268 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/watsonx.py
--rw-r--r--   0        0        0      273 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/integrations/weaviate.py
--rw-r--r--   0        0        0    19461 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/sdk.py
--rw-r--r--   0        0        0        0 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/utils/__init__.py
--rw-r--r--   0        0        0     1150 2024-05-08 02:00:56.630477 highlight_io-0.8.1/highlight_io/utils/lru_cache.py
--rw-r--r--   0        0        0     2532 2024-05-08 02:00:56.630477 highlight_io-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     4106 1970-01-01 00:00:00.000000 highlight_io-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1340 2024-04-30 00:51:35.479597 highlight_io-0.8.2/README.md
+-rw-r--r--   0        0        0       80 2024-05-30 20:33:32.029862 highlight_io-0.8.2/highlight_io/__init__.py
+-rw-r--r--   0        0        0     1402 2024-05-30 20:33:32.029862 highlight_io-0.8.2/highlight_io/integrations/__init__.py
+-rw-r--r--   0        0        0     1950 2024-05-30 20:33:32.029862 highlight_io-0.8.2/highlight_io/integrations/all.py
+-rw-r--r--   0        0        0      278 2024-05-30 20:33:32.029862 highlight_io-0.8.2/highlight_io/integrations/anthropic.py
+-rw-r--r--   0        0        0      717 2024-04-15 23:43:48.116115 highlight_io-0.8.2/highlight_io/integrations/aws.py
+-rw-r--r--   0        0        0      740 2023-04-19 05:15:30.945106 highlight_io-0.8.2/highlight_io/integrations/azure.py
+-rw-r--r--   0        0        0      268 2024-05-30 20:33:32.029862 highlight_io-0.8.2/highlight_io/integrations/bedrock.py
+-rw-r--r--   0        0        0      253 2024-05-30 20:33:32.029862 highlight_io-0.8.2/highlight_io/integrations/boto.py
+-rw-r--r--   0        0        0      273 2024-05-30 20:33:32.029862 highlight_io-0.8.2/highlight_io/integrations/boto3sqs.py
+-rw-r--r--   0        0        0      263 2024-05-30 20:33:32.029862 highlight_io-0.8.2/highlight_io/integrations/celery.py
+-rw-r--r--   0        0        0      269 2024-05-30 20:33:32.029862 highlight_io-0.8.2/highlight_io/integrations/chromadb.py
+-rw-r--r--   0        0        0      263 2024-05-30 20:33:32.029862 highlight_io-0.8.2/highlight_io/integrations/cohere.py
+-rw-r--r--   0        0        0     1871 2024-05-30 20:33:32.029862 highlight_io-0.8.2/highlight_io/integrations/django.py
+-rw-r--r--   0        0        0     2192 2024-05-30 20:33:32.029862 highlight_io-0.8.2/highlight_io/integrations/fastapi.py
+-rw-r--r--   0        0        0     1648 2024-05-30 20:33:32.029862 highlight_io-0.8.2/highlight_io/integrations/flask.py
+-rw-r--r--   0        0        0      747 2023-04-19 05:15:30.949106 highlight_io-0.8.2/highlight_io/integrations/gcp.py
+-rw-r--r--   0        0        0      273 2024-05-30 20:33:32.029862 highlight_io-0.8.2/highlight_io/integrations/haystack.py
+-rw-r--r--   0        0        0      278 2024-05-30 20:33:32.029862 highlight_io-0.8.2/highlight_io/integrations/langchain.py
+-rw-r--r--   0        0        0      283 2024-05-30 20:33:32.029862 highlight_io-0.8.2/highlight_io/integrations/llamaindex.py
+-rw-r--r--   0        0        0      263 2024-05-30 20:33:32.029862 highlight_io-0.8.2/highlight_io/integrations/openai.py
+-rw-r--r--   0        0        0      273 2024-05-30 20:33:32.029862 highlight_io-0.8.2/highlight_io/integrations/pinecone.py
+-rw-r--r--   0        0        0      267 2024-05-30 20:33:32.029862 highlight_io-0.8.2/highlight_io/integrations/qdrant.py
+-rw-r--r--   0        0        0      258 2024-05-30 20:33:32.029862 highlight_io-0.8.2/highlight_io/integrations/redis.py
+-rw-r--r--   0        0        0      278 2024-05-30 20:33:32.029862 highlight_io-0.8.2/highlight_io/integrations/replicate.py
+-rw-r--r--   0        0        0      273 2024-05-30 20:33:32.029862 highlight_io-0.8.2/highlight_io/integrations/requests.py
+-rw-r--r--   0        0        0     1094 2024-05-30 20:33:32.030862 highlight_io-0.8.2/highlight_io/integrations/serverless.py
+-rw-r--r--   0        0        0      283 2024-05-30 20:33:32.030862 highlight_io-0.8.2/highlight_io/integrations/sqlalchemy.py
+-rw-r--r--   0        0        0      293 2024-05-30 20:33:32.030862 highlight_io-0.8.2/highlight_io/integrations/transformers.py
+-rw-r--r--   0        0        0      273 2024-05-30 20:33:32.030862 highlight_io-0.8.2/highlight_io/integrations/vertexai.py
+-rw-r--r--   0        0        0      268 2024-05-30 20:33:32.030862 highlight_io-0.8.2/highlight_io/integrations/watsonx.py
+-rw-r--r--   0        0        0      273 2024-05-30 20:33:32.030862 highlight_io-0.8.2/highlight_io/integrations/weaviate.py
+-rw-r--r--   0        0        0    19929 2024-05-30 21:59:18.922274 highlight_io-0.8.2/highlight_io/sdk.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:51:35.480597 highlight_io-0.8.2/highlight_io/utils/__init__.py
+-rw-r--r--   0        0        0     1150 2024-04-30 00:51:35.480597 highlight_io-0.8.2/highlight_io/utils/lru_cache.py
+-rw-r--r--   0        0        0     2373 2024-05-30 21:50:03.441667 highlight_io-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     4064 1970-01-01 00:00:00.000000 highlight_io-0.8.2/PKG-INFO
```

### Comparing `highlight_io-0.8.1/README.md` & `highlight_io-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `highlight_io-0.8.1/highlight_io/integrations/__init__.py` & `highlight_io-0.8.2/highlight_io/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.8.1/highlight_io/integrations/all.py` & `highlight_io-0.8.2/highlight_io/integrations/all.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.8.1/highlight_io/integrations/aws.py` & `highlight_io-0.8.2/highlight_io/integrations/aws.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.8.1/highlight_io/integrations/azure.py` & `highlight_io-0.8.2/highlight_io/integrations/azure.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.8.1/highlight_io/integrations/django.py` & `highlight_io-0.8.2/highlight_io/integrations/django.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.8.1/highlight_io/integrations/fastapi.py` & `highlight_io-0.8.2/highlight_io/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.8.1/highlight_io/integrations/flask.py` & `highlight_io-0.8.2/highlight_io/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.8.1/highlight_io/integrations/gcp.py` & `highlight_io-0.8.2/highlight_io/integrations/gcp.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.8.1/highlight_io/integrations/serverless.py` & `highlight_io-0.8.2/highlight_io/integrations/serverless.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.8.1/highlight_io/sdk.py` & `highlight_io-0.8.2/highlight_io/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
         disabled_integrations: typing.List[str] = None,
         otlp_endpoint: str = "",
         instrument_logging: bool = True,
         log_level=logging.DEBUG,
         service_name: str = "",
         service_version: str = "",
         environment: str = "",
+        disable_export_error_logging: bool = False,
         debug: bool = False,
         **kwargs,
     ):
         """
         Setup Highlight backend instrumentation.
 
         Example:
@@ -132,14 +133,23 @@
             handler.setLevel(logging.DEBUG)
             formatter = logging.Formatter(
                 "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
             )
             handler.setFormatter(formatter)
             root.addHandler(handler)
 
+        if disable_export_error_logging:
+            for logger_name in (
+                "opentelemetry.exporter.otlp.proto.http._log_exporter",
+                "opentelemetry.exporter.otlp.proto.http.trace_exporter",
+                "opentelemetry.sdk._logs._internal.export",
+                "opentelemetry.sdk.trace.export",
+            ):
+                logging.getLogger(logger_name).setLevel(logging.FATAL)
+
         logger = logging.getLogger("highlight_io")
 
         H._instance = self
         self._project_id = project_id
         self._integrations = integrations or []
         self._disabled_integrations = disabled_integrations or []
         self._otlp_endpoint = otlp_endpoint or H.OTLP_HTTP
```

### Comparing `highlight_io-0.8.1/highlight_io/utils/lru_cache.py` & `highlight_io-0.8.2/highlight_io/utils/lru_cache.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.8.1/pyproject.toml` & `highlight_io-0.8.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "highlight-io"
-version = "0.8.1"
+version = "0.8.2"
 description = "Session replay and error monitoring: stop guessing why bugs happen!"
 license = "Apache-2.0"
 authors = [
     "Vadim Korolik <vadim@highlight.io>",
     "Jay Khatri <jay@highlight.io>",
     "Spencer Amarantides <spencer@highlight.io>",
 ]
@@ -23,56 +23,56 @@
     "Topic :: Software Development",
     "Topic :: System :: Monitoring"
 ]
 packages = [{ include = "highlight_io" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
-opentelemetry-api = "1.24.0"
-opentelemetry-distro = "0.45b0"
-opentelemetry-exporter-otlp-proto-http = "1.24.0"
-opentelemetry-instrumentation = "0.45b0"
-opentelemetry-proto = "1.24.0"
-opentelemetry-sdk = "1.24.0"
-opentelemetry-instrumentation-anthropic = "0.17.2"
-opentelemetry-instrumentation-bedrock = "0.17.2"
-opentelemetry-instrumentation-boto = "0.45b0"
-opentelemetry-instrumentation-boto3sqs = "0.45b0"
-opentelemetry-instrumentation-celery = "0.45b0"
-opentelemetry-instrumentation-chromadb = "0.17.2"
-opentelemetry-instrumentation-cohere = "0.17.2"
-opentelemetry-instrumentation-haystack = "0.17.2"
-opentelemetry-instrumentation-langchain = "0.17.2"
-opentelemetry-instrumentation-llamaindex = "0.17.2"
-opentelemetry-instrumentation-logging = "0.45b0"
-opentelemetry-instrumentation-openai = "0.17.2"
-opentelemetry-instrumentation-pinecone = "0.17.2"
-opentelemetry-instrumentation-qdrant = "0.17.2"
-opentelemetry-instrumentation-redis = "0.45b0"
-opentelemetry-instrumentation-replicate = "0.17.2"
-opentelemetry-instrumentation-requests = "0.45b0"
-opentelemetry-instrumentation-sqlalchemy = "0.45b0"
-opentelemetry-instrumentation-transformers = "0.17.2"
-opentelemetry-instrumentation-vertexai = "0.17.2"
-opentelemetry-instrumentation-watsonx = "0.17.2"
-opentelemetry-instrumentation-weaviate = "0.17.2"
-urllib3 = "2.2.1"
-requests = "2.31.0"
+opentelemetry-api = "^1"
+opentelemetry-distro = "^0"
+opentelemetry-exporter-otlp-proto-http = "^1"
+opentelemetry-instrumentation = "^0"
+opentelemetry-proto = "^1"
+opentelemetry-sdk = "^1"
+opentelemetry-instrumentation-anthropic = "^0"
+opentelemetry-instrumentation-bedrock = "^0"
+opentelemetry-instrumentation-boto = "^0"
+opentelemetry-instrumentation-boto3sqs = "^0"
+opentelemetry-instrumentation-celery = "^0"
+opentelemetry-instrumentation-chromadb = "^0"
+opentelemetry-instrumentation-cohere = "^0"
+opentelemetry-instrumentation-haystack = "^0"
+opentelemetry-instrumentation-langchain = "^0"
+opentelemetry-instrumentation-llamaindex = "^0"
+opentelemetry-instrumentation-logging = "^0"
+opentelemetry-instrumentation-openai = "^0"
+opentelemetry-instrumentation-pinecone = "^0"
+opentelemetry-instrumentation-qdrant = "^0"
+opentelemetry-instrumentation-redis = "^0"
+opentelemetry-instrumentation-replicate = "^0"
+opentelemetry-instrumentation-requests = "^0"
+opentelemetry-instrumentation-sqlalchemy = "^0"
+opentelemetry-instrumentation-transformers = "^0"
+opentelemetry-instrumentation-vertexai = "^0"
+opentelemetry-instrumentation-watsonx = "^0"
+opentelemetry-instrumentation-weaviate = "^0"
+urllib3 = "^2.2.1"
+requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
-azure-functions = "^1.19.0"
-black = "^24.4.2"
-blinker = "^1.8.1"
+azure-functions = "^1"
+black = "^24"
+blinker = "^1"
 django = "^4"
-fastapi = "^0.111.0"
-flask = "^3.0.3"
-functions-framework = "^3.5.0"
-loguru = "^0.7.2"
+fastapi = "^0"
+flask = "^3"
+functions-framework = "^3"
+loguru = "^0"
 orjson = "3.9.15"
-pytest = "^8.2.0"
-pytest-asyncio = "^0.23.6"
-pytest-cov = "^5.0.0"
-pytest-mock = "^3.14.0"
+pytest = "^8"
+pytest-asyncio = "^0"
+pytest-cov = "^5"
+pytest-mock = "^3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `highlight_io-0.8.1/PKG-INFO` & `highlight_io-0.8.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highlight-io
-Version: 0.8.1
+Version: 0.8.2
 Summary: Session replay and error monitoring: stop guessing why bugs happen!
 Home-page: https://www.highlight.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Vadim Korolik
 Author-email: vadim@highlight.io
 Requires-Python: >=3.9,<4
@@ -15,44 +15,44 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: opentelemetry-api (==1.24.0)
-Requires-Dist: opentelemetry-distro (==0.45b0)
-Requires-Dist: opentelemetry-exporter-otlp-proto-http (==1.24.0)
-Requires-Dist: opentelemetry-instrumentation (==0.45b0)
-Requires-Dist: opentelemetry-instrumentation-anthropic (==0.17.2)
-Requires-Dist: opentelemetry-instrumentation-bedrock (==0.17.2)
-Requires-Dist: opentelemetry-instrumentation-boto (==0.45b0)
-Requires-Dist: opentelemetry-instrumentation-boto3sqs (==0.45b0)
-Requires-Dist: opentelemetry-instrumentation-celery (==0.45b0)
-Requires-Dist: opentelemetry-instrumentation-chromadb (==0.17.2)
-Requires-Dist: opentelemetry-instrumentation-cohere (==0.17.2)
-Requires-Dist: opentelemetry-instrumentation-haystack (==0.17.2)
-Requires-Dist: opentelemetry-instrumentation-langchain (==0.17.2)
-Requires-Dist: opentelemetry-instrumentation-llamaindex (==0.17.2)
-Requires-Dist: opentelemetry-instrumentation-logging (==0.45b0)
-Requires-Dist: opentelemetry-instrumentation-openai (==0.17.2)
-Requires-Dist: opentelemetry-instrumentation-pinecone (==0.17.2)
-Requires-Dist: opentelemetry-instrumentation-qdrant (==0.17.2)
-Requires-Dist: opentelemetry-instrumentation-redis (==0.45b0)
-Requires-Dist: opentelemetry-instrumentation-replicate (==0.17.2)
-Requires-Dist: opentelemetry-instrumentation-requests (==0.45b0)
-Requires-Dist: opentelemetry-instrumentation-sqlalchemy (==0.45b0)
-Requires-Dist: opentelemetry-instrumentation-transformers (==0.17.2)
-Requires-Dist: opentelemetry-instrumentation-vertexai (==0.17.2)
-Requires-Dist: opentelemetry-instrumentation-watsonx (==0.17.2)
-Requires-Dist: opentelemetry-instrumentation-weaviate (==0.17.2)
-Requires-Dist: opentelemetry-proto (==1.24.0)
-Requires-Dist: opentelemetry-sdk (==1.24.0)
-Requires-Dist: requests (==2.31.0)
-Requires-Dist: urllib3 (==2.2.1)
+Requires-Dist: opentelemetry-api (>=1,<2)
+Requires-Dist: opentelemetry-distro (>=0,<1)
+Requires-Dist: opentelemetry-exporter-otlp-proto-http (>=1,<2)
+Requires-Dist: opentelemetry-instrumentation (>=0,<1)
+Requires-Dist: opentelemetry-instrumentation-anthropic (>=0,<1)
+Requires-Dist: opentelemetry-instrumentation-bedrock (>=0,<1)
+Requires-Dist: opentelemetry-instrumentation-boto (>=0,<1)
+Requires-Dist: opentelemetry-instrumentation-boto3sqs (>=0,<1)
+Requires-Dist: opentelemetry-instrumentation-celery (>=0,<1)
+Requires-Dist: opentelemetry-instrumentation-chromadb (>=0,<1)
+Requires-Dist: opentelemetry-instrumentation-cohere (>=0,<1)
+Requires-Dist: opentelemetry-instrumentation-haystack (>=0,<1)
+Requires-Dist: opentelemetry-instrumentation-langchain (>=0,<1)
+Requires-Dist: opentelemetry-instrumentation-llamaindex (>=0,<1)
+Requires-Dist: opentelemetry-instrumentation-logging (>=0,<1)
+Requires-Dist: opentelemetry-instrumentation-openai (>=0,<1)
+Requires-Dist: opentelemetry-instrumentation-pinecone (>=0,<1)
+Requires-Dist: opentelemetry-instrumentation-qdrant (>=0,<1)
+Requires-Dist: opentelemetry-instrumentation-redis (>=0,<1)
+Requires-Dist: opentelemetry-instrumentation-replicate (>=0,<1)
+Requires-Dist: opentelemetry-instrumentation-requests (>=0,<1)
+Requires-Dist: opentelemetry-instrumentation-sqlalchemy (>=0,<1)
+Requires-Dist: opentelemetry-instrumentation-transformers (>=0,<1)
+Requires-Dist: opentelemetry-instrumentation-vertexai (>=0,<1)
+Requires-Dist: opentelemetry-instrumentation-watsonx (>=0,<1)
+Requires-Dist: opentelemetry-instrumentation-weaviate (>=0,<1)
+Requires-Dist: opentelemetry-proto (>=1,<2)
+Requires-Dist: opentelemetry-sdk (>=1,<2)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: urllib3 (>=2.2.1,<3.0.0)
 Project-URL: Documentation, https://www.highlight.io/docs
 Project-URL: Repository, https://github.com/highlight/highlight
 Description-Content-Type: text/markdown
 
 # highlight-io Python SDK
 
 This directory contains the source code for the Highlight Python SDK.
```

