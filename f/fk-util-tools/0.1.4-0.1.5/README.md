# Comparing `tmp/fk_util_tools-0.1.4.tar.gz` & `tmp/fk_util_tools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fk_util_tools-0.1.4.tar", last modified: Thu May 30 20:28:43 2024, max compression
+gzip compressed data, was "fk_util_tools-0.1.5.tar", last modified: Thu May 30 23:47:40 2024, max compression
```

## Comparing `fk_util_tools-0.1.4.tar` & `fk_util_tools-0.1.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/fk_util_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-30 20:28:43.000000 fk_util_tools-0.1.4/fk_util_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-30 20:28:43.000000 fk_util_tools-0.1.4/fk_util_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 20:28:43.000000 fk_util_tools-0.1.4/fk_util_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-30 20:28:43.000000 fk_util_tools-0.1.4/fk_util_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 20:28:43.000000 fk_util_tools-0.1.4/fk_util_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.480230 fk_util_tools-0.1.4/fk_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.480230 fk_util_tools-0.1.4/fk_utils/envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/envs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/fk_utils/envs/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/envs/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/envs/aws/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/envs/aws/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/fk_utils/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/middlewares/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/fk_utils/middlewares/django/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/middlewares/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/middlewares/django/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/fk_utils/middlewares/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/middlewares/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/middlewares/fastapi/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/fk_utils/middlewares/flask/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/middlewares/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/middlewares/flask/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/fk_utils/traces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/traces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/fk_utils/traces/datadog/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/traces/datadog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/django/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/django/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/fastapi/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/flask/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/flask/trace.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      556 2024-05-30 20:28:43.488230 fk_util_tools-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-30 20:28:41.000000 fk_util_tools-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.478041 fk_util_tools-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-30 23:47:40.478041 fk_util_tools-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.478041 fk_util_tools-0.1.5/fk_util_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-30 23:47:40.000000 fk_util_tools-0.1.5/fk_util_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-30 23:47:40.000000 fk_util_tools-0.1.5/fk_util_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 23:47:40.000000 fk_util_tools-0.1.5/fk_util_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-30 23:47:40.000000 fk_util_tools-0.1.5/fk_util_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 23:47:40.000000 fk_util_tools-0.1.5/fk_util_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.474040 fk_util_tools-0.1.5/fk_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.474040 fk_util_tools-0.1.5/fk_utils/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/envs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.474040 fk_util_tools-0.1.5/fk_utils/envs/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/envs/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/envs/aws/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/envs/aws/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.474040 fk_util_tools-0.1.5/fk_utils/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/middlewares/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.474040 fk_util_tools-0.1.5/fk_utils/middlewares/django/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/middlewares/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/middlewares/django/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.474040 fk_util_tools-0.1.5/fk_utils/middlewares/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/middlewares/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/middlewares/fastapi/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.474040 fk_util_tools-0.1.5/fk_utils/middlewares/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/middlewares/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/middlewares/flask/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.474040 fk_util_tools-0.1.5/fk_utils/traces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/traces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.478041 fk_util_tools-0.1.5/fk_utils/traces/datadog/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/traces/datadog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.478041 fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.478041 fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/django/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/django/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.478041 fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/fastapi/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.478041 fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/flask/trace.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      556 2024-05-30 23:47:40.478041 fk_util_tools-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-30 23:47:38.000000 fk_util_tools-0.1.5/setup.py
```

### Comparing `fk_util_tools-0.1.4/LICENSE` & `fk_util_tools-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fk_util_tools-0.1.4/PKG-INFO` & `fk_util_tools-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fk_util_tools
-Version: 0.1.4
+Version: 0.1.5
 Home-page: https://gitlab.com/f3315/team-back-end/cross/packages/package_utils
 Author: Steven Santacruz Garcia
 Author-email: stevengarcia1118@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3
@@ -13,9 +13,10 @@
 Requires-Dist: opentelemetry-instrumentation-fastapi
 Requires-Dist: opentelemetry-instrumentation-flask
 Requires-Dist: opentelemetry-instrumentation-django
 Requires-Dist: opentelemetry-exporter-otlp
 Requires-Dist: opentelemetry-instrumentation-sqlalchemy
 Requires-Dist: opentelemetry-instrumentation-requests
 Requires-Dist: opentelemetry-exporter-jaeger
+Requires-Dist: opentelemetry-instrumentation-psycopg2
 
 Herramientas de utilidad o funciones comunes para los proyectos de FK.
```

### Comparing `fk_util_tools-0.1.4/fk_util_tools.egg-info/PKG-INFO` & `fk_util_tools-0.1.5/fk_util_tools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fk_util_tools
-Version: 0.1.4
+Version: 0.1.5
 Home-page: https://gitlab.com/f3315/team-back-end/cross/packages/package_utils
 Author: Steven Santacruz Garcia
 Author-email: stevengarcia1118@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3
@@ -13,9 +13,10 @@
 Requires-Dist: opentelemetry-instrumentation-fastapi
 Requires-Dist: opentelemetry-instrumentation-flask
 Requires-Dist: opentelemetry-instrumentation-django
 Requires-Dist: opentelemetry-exporter-otlp
 Requires-Dist: opentelemetry-instrumentation-sqlalchemy
 Requires-Dist: opentelemetry-instrumentation-requests
 Requires-Dist: opentelemetry-exporter-jaeger
+Requires-Dist: opentelemetry-instrumentation-psycopg2
 
 Herramientas de utilidad o funciones comunes para los proyectos de FK.
```

### Comparing `fk_util_tools-0.1.4/fk_util_tools.egg-info/SOURCES.txt` & `fk_util_tools-0.1.5/fk_util_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fk_util_tools-0.1.4/fk_utils/config.py` & `fk_util_tools-0.1.5/fk_utils/config.py`

 * *Files identical despite different names*

### Comparing `fk_util_tools-0.1.4/fk_utils/envs/aws/parameters.py` & `fk_util_tools-0.1.5/fk_utils/envs/aws/parameters.py`

 * *Files identical despite different names*

### Comparing `fk_util_tools-0.1.4/fk_utils/envs/aws/secrets.py` & `fk_util_tools-0.1.5/fk_utils/envs/aws/secrets.py`

 * *Files identical despite different names*

### Comparing `fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/django/trace.py` & `fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/flask/trace.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,29 @@
-# opentelemetry_config.py
 import logging
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from opentelemetry.exporter.otlp.proto.grpc.trace_exporter import OTLPSpanExporter
 from opentelemetry.sdk.resources import Resource
-from opentelemetry.instrumentation.django import DjangoInstrumentor
+from opentelemetry.instrumentation.flask import FlaskInstrumentor
+from opentelemetry.instrumentation.sqlalchemy import SQLAlchemyInstrumentor
 from opentelemetry.instrumentation.requests import RequestsInstrumentor
 
-from django.apps import AppConfig
-
 from fk_utils import SETTINGS
 
 # Configurar logging
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
-SERVICE_NAME = SETTINGS.OTLP_NAME
-
 
 def configure_tracer():
     try:
         # Configurar el proveedor de trazas
         trace.set_tracer_provider(TracerProvider(
-            resource=Resource.create({SERVICE_NAME: SERVICE_NAME})
+            resource=Resource.create({"service.name": SETTINGS.OTLP_NAME})
         ))
 
         # Configurar el exportador OTLP
         otlp_exporter = OTLPSpanExporter(
             endpoint=f"{SETTINGS.OTLP_HOST}:{SETTINGS.OTLP_PORT}",
             insecure=True
         )
@@ -39,28 +35,22 @@
 
         logger.info("OpenTelemetry tracer configurado correctamente.")
 
     except Exception as e:
         logger.error(f"Error al configurar el tracer de OpenTelemetry: {e}")
 
 
-def instrument_app():
+def instrument_app(app):
     try:
-        # Instrumentar Django
-        DjangoInstrumentor().instrument()
+        # Instrumentar Flask
+        FlaskInstrumentor().instrument_app(app)
+
+        # Instrumentar SQLAlchemy
+        SQLAlchemyInstrumentor().instrument()
 
         # Instrumentar Requests
         RequestsInstrumentor().instrument()
 
         logger.info("Aplicación instrumentada correctamente con OpenTelemetry.")
 
     except Exception as e:
         logger.error(f"Error al instrumentar la aplicación: {e}")
-
-
-class OpenTelemetryConfig(AppConfig):
-    name = 'fk_utils.traces.opentelemetry.django.trace'
-    verbose_name = "OpenTelemetry Integration"
-
-    def ready(self):
-        configure_tracer()
-        instrument_app()
```

### Comparing `fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/fastapi/trace.py` & `fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/fastapi/trace.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,22 +10,20 @@
 
 from fk_utils import SETTINGS
 
 # Configurar logging
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
-SERVICE_NAME = SETTINGS.OTLP_NAME
-
 
 def configure_tracer():
     try:
         # Configurar el proveedor de trazas
         trace.set_tracer_provider(TracerProvider(
-            resource=Resource.create({SERVICE_NAME: SERVICE_NAME})
+            resource=Resource.create({"service.name": SETTINGS.OTLP_NAME})
         ))
 
         # Configurar el exportador OTLP
         otlp_exporter = OTLPSpanExporter(
             endpoint=f"{SETTINGS.OTLP_HOST}:{SETTINGS.OTLP_PORT}",
             insecure=True
         )
```

### Comparing `fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/flask/trace.py` & `fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/django/trace.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,33 @@
+# opentelemetry_config.py
 import logging
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from opentelemetry.exporter.otlp.proto.grpc.trace_exporter import OTLPSpanExporter
 from opentelemetry.sdk.resources import Resource
-from opentelemetry.instrumentation.flask import FlaskInstrumentor
-from opentelemetry.instrumentation.sqlalchemy import SQLAlchemyInstrumentor
+from opentelemetry.instrumentation.django import DjangoInstrumentor
 from opentelemetry.instrumentation.requests import RequestsInstrumentor
+from opentelemetry.instrumentation.psycopg2 import Psycopg2Instrumentor
+
+import logging
+from django.apps import AppConfig
 
 from fk_utils import SETTINGS
 
 # Configurar logging
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
-SERVICE_NAME = SETTINGS.OTLP_NAME
-
 
 def configure_tracer():
     try:
         # Configurar el proveedor de trazas
         trace.set_tracer_provider(TracerProvider(
-            resource=Resource.create({SERVICE_NAME: SERVICE_NAME})
+            resource=Resource.create({"service.name": SETTINGS.OTLP_NAME})
         ))
 
         # Configurar el exportador OTLP
         otlp_exporter = OTLPSpanExporter(
             endpoint=f"{SETTINGS.OTLP_HOST}:{SETTINGS.OTLP_PORT}",
             insecure=True
         )
@@ -37,22 +39,31 @@
 
         logger.info("OpenTelemetry tracer configurado correctamente.")
 
     except Exception as e:
         logger.error(f"Error al configurar el tracer de OpenTelemetry: {e}")
 
 
-def instrument_app(app):
+def instrument_app():
     try:
-        # Instrumentar Flask
-        FlaskInstrumentor().instrument_app(app)
-
-        # Instrumentar SQLAlchemy
-        SQLAlchemyInstrumentor().instrument()
+        # Instrumentar Django
+        DjangoInstrumentor().instrument()
 
         # Instrumentar Requests
         RequestsInstrumentor().instrument()
 
+        # Instrumentar PostgreSQL
+        Psycopg2Instrumentor().instrument()
+
         logger.info("Aplicación instrumentada correctamente con OpenTelemetry.")
 
     except Exception as e:
         logger.error(f"Error al instrumentar la aplicación: {e}")
+
+
+class OpenTelemetryConfig(AppConfig):
+    name = 'fk_utils.traces.opentelemetry.django.trace'
+    verbose_name = "OpenTelemetry Integration"
+
+    def ready(self):
+        configure_tracer()
+        instrument_app()
```

### Comparing `fk_util_tools-0.1.4/setup.cfg` & `fk_util_tools-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `fk_util_tools-0.1.4/setup.py` & `fk_util_tools-0.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 PACKAGE_NAME = 'fk_util_tools'
 AUTHOR = 'Steven Santacruz Garcia'
 AUTHOR_EMAIL = 'stevengarcia1118@gmail.com'
 URL = 'https://gitlab.com/f3315/team-back-end/cross/packages/package_utils'
 
 LICENSE = 'MIT'
 DESCRIPTION = """Herramientas de utilidad o funciones comunes para los proyectos de FK."""
@@ -18,15 +18,16 @@
     'opentelemetry-sdk',
     'opentelemetry-instrumentation-fastapi',
     'opentelemetry-instrumentation-flask',
     'opentelemetry-instrumentation-django',
     'opentelemetry-exporter-otlp',
     'opentelemetry-instrumentation-sqlalchemy',
     'opentelemetry-instrumentation-requests',
-    'opentelemetry-exporter-jaeger'
+    'opentelemetry-exporter-jaeger',
+    'opentelemetry-instrumentation-psycopg2'
 
 ]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     long_description=LONG_DESCRIPTION,
```

