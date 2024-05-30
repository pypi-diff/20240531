# Comparing `tmp/fk_util_tools-0.1.3.tar.gz` & `tmp/fk_util_tools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fk_util_tools-0.1.3.tar", last modified: Thu May 30 19:48:44 2024, max compression
+gzip compressed data, was "fk_util_tools-0.1.4.tar", last modified: Thu May 30 20:28:43 2024, max compression
```

## Comparing `fk_util_tools-0.1.3.tar` & `fk_util_tools-0.1.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.216690 fk_util_tools-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-30 19:48:44.216690 fk_util_tools-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.216690 fk_util_tools-0.1.3/fk_util_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-30 19:48:44.000000 fk_util_tools-0.1.3/fk_util_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-30 19:48:44.000000 fk_util_tools-0.1.3/fk_util_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:48:44.000000 fk_util_tools-0.1.3/fk_util_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-30 19:48:44.000000 fk_util_tools-0.1.3/fk_util_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 19:48:44.000000 fk_util_tools-0.1.3/fk_util_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.212690 fk_util_tools-0.1.3/fk_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.212690 fk_util_tools-0.1.3/fk_utils/envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/envs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.212690 fk_util_tools-0.1.3/fk_utils/envs/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/envs/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/envs/aws/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/envs/aws/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.212690 fk_util_tools-0.1.3/fk_utils/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/middlewares/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.212690 fk_util_tools-0.1.3/fk_utils/middlewares/django/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/middlewares/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/middlewares/django/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.216690 fk_util_tools-0.1.3/fk_utils/middlewares/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/middlewares/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/middlewares/fastapi/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.216690 fk_util_tools-0.1.3/fk_utils/middlewares/flask/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/middlewares/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/middlewares/flask/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.216690 fk_util_tools-0.1.3/fk_utils/traces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/traces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.216690 fk_util_tools-0.1.3/fk_utils/traces/datadog/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/traces/datadog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.216690 fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.216690 fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/django/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/django/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.216690 fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/fastapi/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.216690 fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/flask/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/flask/trace.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      556 2024-05-30 19:48:44.216690 fk_util_tools-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-30 19:48:42.000000 fk_util_tools-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/fk_util_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-30 20:28:43.000000 fk_util_tools-0.1.4/fk_util_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-30 20:28:43.000000 fk_util_tools-0.1.4/fk_util_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 20:28:43.000000 fk_util_tools-0.1.4/fk_util_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-30 20:28:43.000000 fk_util_tools-0.1.4/fk_util_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 20:28:43.000000 fk_util_tools-0.1.4/fk_util_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.480230 fk_util_tools-0.1.4/fk_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.480230 fk_util_tools-0.1.4/fk_utils/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/envs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/fk_utils/envs/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/envs/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/envs/aws/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/envs/aws/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/fk_utils/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/middlewares/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/fk_utils/middlewares/django/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/middlewares/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/middlewares/django/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/fk_utils/middlewares/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/middlewares/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/middlewares/fastapi/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/fk_utils/middlewares/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/middlewares/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/middlewares/flask/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/fk_utils/traces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/traces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/fk_utils/traces/datadog/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/traces/datadog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/django/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/django/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/fastapi/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:43.484230 fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-30 20:28:37.000000 fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/flask/trace.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      556 2024-05-30 20:28:43.488230 fk_util_tools-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-30 20:28:41.000000 fk_util_tools-0.1.4/setup.py
```

### Comparing `fk_util_tools-0.1.3/LICENSE` & `fk_util_tools-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fk_util_tools-0.1.3/PKG-INFO` & `fk_util_tools-0.1.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: fk_util_tools
-Version: 0.1.3
+Version: 0.1.4
 Home-page: https://gitlab.com/f3315/team-back-end/cross/packages/package_utils
 Author: Steven Santacruz Garcia
 Author-email: stevengarcia1118@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3
 Requires-Dist: opentelemetry-api
 Requires-Dist: opentelemetry-sdk
 Requires-Dist: opentelemetry-instrumentation-fastapi
 Requires-Dist: opentelemetry-instrumentation-flask
 Requires-Dist: opentelemetry-instrumentation-django
+Requires-Dist: opentelemetry-exporter-otlp
+Requires-Dist: opentelemetry-instrumentation-sqlalchemy
+Requires-Dist: opentelemetry-instrumentation-requests
+Requires-Dist: opentelemetry-exporter-jaeger
 
 Herramientas de utilidad o funciones comunes para los proyectos de FK.
```

### Comparing `fk_util_tools-0.1.3/fk_util_tools.egg-info/PKG-INFO` & `fk_util_tools-0.1.4/fk_util_tools.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: fk_util_tools
-Version: 0.1.3
+Version: 0.1.4
 Home-page: https://gitlab.com/f3315/team-back-end/cross/packages/package_utils
 Author: Steven Santacruz Garcia
 Author-email: stevengarcia1118@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3
 Requires-Dist: opentelemetry-api
 Requires-Dist: opentelemetry-sdk
 Requires-Dist: opentelemetry-instrumentation-fastapi
 Requires-Dist: opentelemetry-instrumentation-flask
 Requires-Dist: opentelemetry-instrumentation-django
+Requires-Dist: opentelemetry-exporter-otlp
+Requires-Dist: opentelemetry-instrumentation-sqlalchemy
+Requires-Dist: opentelemetry-instrumentation-requests
+Requires-Dist: opentelemetry-exporter-jaeger
 
 Herramientas de utilidad o funciones comunes para los proyectos de FK.
```

### Comparing `fk_util_tools-0.1.3/fk_util_tools.egg-info/SOURCES.txt` & `fk_util_tools-0.1.4/fk_util_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fk_util_tools-0.1.3/fk_utils/config.py` & `fk_util_tools-0.1.4/fk_utils/config.py`

 * *Files identical despite different names*

### Comparing `fk_util_tools-0.1.3/fk_utils/envs/aws/parameters.py` & `fk_util_tools-0.1.4/fk_utils/envs/aws/parameters.py`

 * *Files identical despite different names*

### Comparing `fk_util_tools-0.1.3/fk_utils/envs/aws/secrets.py` & `fk_util_tools-0.1.4/fk_utils/envs/aws/secrets.py`

 * *Files identical despite different names*

### Comparing `fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/django/trace.py` & `fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/django/trace.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # opentelemetry_config.py
 import logging
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
-from opentelemetry.sdk.trace.export import BatchSpanProcessor, OTLPSpanExporter
+from opentelemetry.sdk.trace.export import BatchSpanProcessor
+from opentelemetry.exporter.otlp.proto.grpc.trace_exporter import OTLPSpanExporter
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.instrumentation.django import DjangoInstrumentor
 from opentelemetry.instrumentation.requests import RequestsInstrumentor
 
 from django.apps import AppConfig
 
 from fk_utils import SETTINGS
```

### Comparing `fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/fastapi/trace.py` & `fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/fastapi/trace.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
-from opentelemetry.sdk.trace.export import BatchSpanProcessor, OTLPSpanExporter
+from opentelemetry.sdk.trace.export import BatchSpanProcessor
+from opentelemetry.exporter.otlp.proto.grpc.trace_exporter import OTLPSpanExporter
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.instrumentation.fastapi import FastAPIInstrumentor
 from opentelemetry.instrumentation.sqlalchemy import SQLAlchemyInstrumentor
 from opentelemetry.instrumentation.requests import RequestsInstrumentor
 
 from fk_utils import SETTINGS
```

### Comparing `fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/flask/trace.py` & `fk_util_tools-0.1.4/fk_utils/traces/opentelemetry/flask/trace.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
-from opentelemetry.sdk.trace.export import BatchSpanProcessor, OTLPSpanExporter
+from opentelemetry.sdk.trace.export import BatchSpanProcessor
+from opentelemetry.exporter.otlp.proto.grpc.trace_exporter import OTLPSpanExporter
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.instrumentation.flask import FlaskInstrumentor
 from opentelemetry.instrumentation.sqlalchemy import SQLAlchemyInstrumentor
 from opentelemetry.instrumentation.requests import RequestsInstrumentor
 
 from fk_utils import SETTINGS
```

### Comparing `fk_util_tools-0.1.3/setup.cfg` & `fk_util_tools-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `fk_util_tools-0.1.3/setup.py` & `fk_util_tools-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 PACKAGE_NAME = 'fk_util_tools'
 AUTHOR = 'Steven Santacruz Garcia'
 AUTHOR_EMAIL = 'stevengarcia1118@gmail.com'
 URL = 'https://gitlab.com/f3315/team-back-end/cross/packages/package_utils'
 
 LICENSE = 'MIT'
 DESCRIPTION = """Herramientas de utilidad o funciones comunes para los proyectos de FK."""
@@ -14,15 +14,20 @@
 
 INSTALL_REQUIRES = [
     'boto3',
     'opentelemetry-api',
     'opentelemetry-sdk',
     'opentelemetry-instrumentation-fastapi',
     'opentelemetry-instrumentation-flask',
-    'opentelemetry-instrumentation-django'
+    'opentelemetry-instrumentation-django',
+    'opentelemetry-exporter-otlp',
+    'opentelemetry-instrumentation-sqlalchemy',
+    'opentelemetry-instrumentation-requests',
+    'opentelemetry-exporter-jaeger'
+
 ]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type=LONG_DESC_TYPE,
```

