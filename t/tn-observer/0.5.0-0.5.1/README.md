# Comparing `tmp/tn_observer-0.5.0.tar.gz` & `tmp/tn_observer-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tn_observer-0.5.0.tar", last modified: Fri May 31 08:27:00 2024, max compression
+gzip compressed data, was "tn_observer-0.5.1.tar", last modified: Fri May 31 09:58:43 2024, max compression
```

## Comparing `tn_observer-0.5.0.tar` & `tn_observer-0.5.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 sorapol    (502) staff       (20)        0 2024-05-31 08:27:00.882711 tn_observer-0.5.0/
--rw-r--r--   0 sorapol    (502) staff       (20)     1064 2024-05-31 04:22:54.000000 tn_observer-0.5.0/LICENSE.txt
--rw-r--r--   0 sorapol    (502) staff       (20)     7341 2024-05-31 08:27:00.882457 tn_observer-0.5.0/PKG-INFO
--rw-r--r--   0 sorapol    (502) staff       (20)     6437 2024-05-31 08:26:54.000000 tn_observer-0.5.0/README.md
--rw-r--r--   0 sorapol    (502) staff       (20)      918 2024-05-31 08:25:22.000000 tn_observer-0.5.0/pyproject.toml
--rw-r--r--   0 sorapol    (502) staff       (20)       38 2024-05-31 08:27:00.882761 tn_observer-0.5.0/setup.cfg
-drwxr-xr-x   0 sorapol    (502) staff       (20)        0 2024-05-31 08:27:00.874778 tn_observer-0.5.0/src/
-drwxr-xr-x   0 sorapol    (502) staff       (20)        0 2024-05-31 08:27:00.876197 tn_observer-0.5.0/src/thinknet_observer/
--rw-r--r--   0 sorapol    (502) staff       (20)      580 2024-05-31 07:02:07.000000 tn_observer-0.5.0/src/thinknet_observer/__init__.py
--rw-r--r--   0 sorapol    (502) staff       (20)     1927 2024-04-05 09:52:59.000000 tn_observer-0.5.0/src/thinknet_observer/calulator.py
-drwxr-xr-x   0 sorapol    (502) staff       (20)        0 2024-05-31 08:27:00.877221 tn_observer-0.5.0/src/thinknet_observer/loggers/
--rw-r--r--   0 sorapol    (502) staff       (20)        0 2024-04-19 08:30:57.000000 tn_observer-0.5.0/src/thinknet_observer/loggers/__init__.py
--rw-r--r--   0 sorapol    (502) staff       (20)     2383 2024-05-30 06:15:33.000000 tn_observer-0.5.0/src/thinknet_observer/loggers/fast_logger.py
--rw-r--r--   0 sorapol    (502) staff       (20)     2665 2024-05-30 06:15:26.000000 tn_observer-0.5.0/src/thinknet_observer/loggers/flask_logger.py
--rw-r--r--   0 sorapol    (502) staff       (20)     7460 2024-05-30 03:04:57.000000 tn_observer-0.5.0/src/thinknet_observer/loggers/loggers.py
-drwxr-xr-x   0 sorapol    (502) staff       (20)        0 2024-05-31 08:27:00.879031 tn_observer-0.5.0/src/thinknet_observer/metrics/
--rw-r--r--   0 sorapol    (502) staff       (20)        1 2024-04-05 09:52:59.000000 tn_observer-0.5.0/src/thinknet_observer/metrics/__init__.py
--rw-r--r--   0 sorapol    (502) staff       (20)     4671 2024-05-30 09:45:23.000000 tn_observer-0.5.0/src/thinknet_observer/metrics/collector.py
--rw-r--r--   0 sorapol    (502) staff       (20)      495 2024-05-23 04:51:23.000000 tn_observer-0.5.0/src/thinknet_observer/metrics/config.py
--rw-r--r--   0 sorapol    (502) staff       (20)     3800 2024-04-05 09:52:59.000000 tn_observer-0.5.0/src/thinknet_observer/metrics/custom_metrics_wrapper.py
--rw-r--r--   0 sorapol    (502) staff       (20)      486 2024-04-05 09:52:59.000000 tn_observer-0.5.0/src/thinknet_observer/metrics/fastapi_metrics_redirect.py
--rw-r--r--   0 sorapol    (502) staff       (20)    16059 2024-05-30 06:05:00.000000 tn_observer-0.5.0/src/thinknet_observer/metrics/metrics.py
--rw-r--r--   0 sorapol    (502) staff       (20)     7407 2024-05-30 08:48:29.000000 tn_observer-0.5.0/src/thinknet_observer/otel.py
-drwxr-xr-x   0 sorapol    (502) staff       (20)        0 2024-05-31 08:27:00.880416 tn_observer-0.5.0/src/thinknet_observer/utils/
--rw-r--r--   0 sorapol    (502) staff       (20)        0 2024-04-05 09:52:59.000000 tn_observer-0.5.0/src/thinknet_observer/utils/__init__.py
--rw-r--r--   0 sorapol    (502) staff       (20)      227 2024-04-05 09:52:59.000000 tn_observer-0.5.0/src/thinknet_observer/utils/bcolor.py
--rw-r--r--   0 sorapol    (502) staff       (20)      587 2024-04-05 09:52:59.000000 tn_observer-0.5.0/src/thinknet_observer/utils/gunicorn_multiprocess.py
--rw-r--r--   0 sorapol    (502) staff       (20)      599 2024-04-19 09:58:03.000000 tn_observer-0.5.0/src/thinknet_observer/utils/health.py
--rw-r--r--   0 sorapol    (502) staff       (20)      627 2024-04-05 09:52:59.000000 tn_observer-0.5.0/src/thinknet_observer/utils/singleton.py
-drwxr-xr-x   0 sorapol    (502) staff       (20)        0 2024-05-31 08:27:00.882098 tn_observer-0.5.0/src/tn_observer.egg-info/
--rw-r--r--   0 sorapol    (502) staff       (20)     7341 2024-05-31 08:27:00.000000 tn_observer-0.5.0/src/tn_observer.egg-info/PKG-INFO
--rw-r--r--   0 sorapol    (502) staff       (20)     1074 2024-05-31 08:27:00.000000 tn_observer-0.5.0/src/tn_observer.egg-info/SOURCES.txt
--rw-r--r--   0 sorapol    (502) staff       (20)        1 2024-05-31 08:27:00.000000 tn_observer-0.5.0/src/tn_observer.egg-info/dependency_links.txt
--rw-r--r--   0 sorapol    (502) staff       (20)      359 2024-05-31 08:27:00.000000 tn_observer-0.5.0/src/tn_observer.egg-info/requires.txt
--rw-r--r--   0 sorapol    (502) staff       (20)       18 2024-05-31 08:27:00.000000 tn_observer-0.5.0/src/tn_observer.egg-info/top_level.txt
-drwxr-xr-x   0 sorapol    (502) staff       (20)        0 2024-05-31 08:27:00.881836 tn_observer-0.5.0/tests/
--rw-r--r--   0 sorapol    (502) staff       (20)     1523 2024-04-05 09:52:59.000000 tn_observer-0.5.0/tests/test_calculator.py
--rw-r--r--   0 sorapol    (502) staff       (20)    30470 2024-05-31 07:03:54.000000 tn_observer-0.5.0/tests/test_metric_fastapi.py
--rw-r--r--   0 sorapol    (502) staff       (20)    31043 2024-05-31 07:00:14.000000 tn_observer-0.5.0/tests/test_metric_flask.py
+drwxr-xr-x   0 sorapol    (502) staff       (20)        0 2024-05-31 09:58:43.370094 tn_observer-0.5.1/
+-rw-r--r--   0 sorapol    (502) staff       (20)     1064 2024-05-31 04:22:54.000000 tn_observer-0.5.1/LICENSE.txt
+-rw-r--r--   0 sorapol    (502) staff       (20)     7615 2024-05-31 09:58:43.369867 tn_observer-0.5.1/PKG-INFO
+-rw-r--r--   0 sorapol    (502) staff       (20)     6711 2024-05-31 09:20:54.000000 tn_observer-0.5.1/README.md
+-rw-r--r--   0 sorapol    (502) staff       (20)      918 2024-05-31 09:58:38.000000 tn_observer-0.5.1/pyproject.toml
+-rw-r--r--   0 sorapol    (502) staff       (20)       38 2024-05-31 09:58:43.370146 tn_observer-0.5.1/setup.cfg
+drwxr-xr-x   0 sorapol    (502) staff       (20)        0 2024-05-31 09:58:43.362639 tn_observer-0.5.1/src/
+drwxr-xr-x   0 sorapol    (502) staff       (20)        0 2024-05-31 09:58:43.364169 tn_observer-0.5.1/src/thinknet_observer/
+-rw-r--r--   0 sorapol    (502) staff       (20)      578 2024-05-31 09:56:06.000000 tn_observer-0.5.1/src/thinknet_observer/__init__.py
+-rw-r--r--   0 sorapol    (502) staff       (20)     1927 2024-04-05 09:52:59.000000 tn_observer-0.5.1/src/thinknet_observer/calulator.py
+drwxr-xr-x   0 sorapol    (502) staff       (20)        0 2024-05-31 09:58:43.364812 tn_observer-0.5.1/src/thinknet_observer/loggers/
+-rw-r--r--   0 sorapol    (502) staff       (20)        0 2024-04-19 08:30:57.000000 tn_observer-0.5.1/src/thinknet_observer/loggers/__init__.py
+-rw-r--r--   0 sorapol    (502) staff       (20)     2383 2024-05-30 06:15:33.000000 tn_observer-0.5.1/src/thinknet_observer/loggers/fast_logger.py
+-rw-r--r--   0 sorapol    (502) staff       (20)     2665 2024-05-30 06:15:26.000000 tn_observer-0.5.1/src/thinknet_observer/loggers/flask_logger.py
+-rw-r--r--   0 sorapol    (502) staff       (20)     7460 2024-05-30 03:04:57.000000 tn_observer-0.5.1/src/thinknet_observer/loggers/loggers.py
+drwxr-xr-x   0 sorapol    (502) staff       (20)        0 2024-05-31 09:58:43.366159 tn_observer-0.5.1/src/thinknet_observer/metrics/
+-rw-r--r--   0 sorapol    (502) staff       (20)        1 2024-04-05 09:52:59.000000 tn_observer-0.5.1/src/thinknet_observer/metrics/__init__.py
+-rw-r--r--   0 sorapol    (502) staff       (20)     4671 2024-05-30 09:45:23.000000 tn_observer-0.5.1/src/thinknet_observer/metrics/collector.py
+-rw-r--r--   0 sorapol    (502) staff       (20)      495 2024-05-23 04:51:23.000000 tn_observer-0.5.1/src/thinknet_observer/metrics/config.py
+-rw-r--r--   0 sorapol    (502) staff       (20)     3800 2024-04-05 09:52:59.000000 tn_observer-0.5.1/src/thinknet_observer/metrics/custom_metrics_wrapper.py
+-rw-r--r--   0 sorapol    (502) staff       (20)      486 2024-04-05 09:52:59.000000 tn_observer-0.5.1/src/thinknet_observer/metrics/fastapi_metrics_redirect.py
+-rw-r--r--   0 sorapol    (502) staff       (20)    16059 2024-05-30 06:05:00.000000 tn_observer-0.5.1/src/thinknet_observer/metrics/metrics.py
+-rw-r--r--   0 sorapol    (502) staff       (20)     7407 2024-05-30 08:48:29.000000 tn_observer-0.5.1/src/thinknet_observer/otel.py
+drwxr-xr-x   0 sorapol    (502) staff       (20)        0 2024-05-31 09:58:43.367332 tn_observer-0.5.1/src/thinknet_observer/utils/
+-rw-r--r--   0 sorapol    (502) staff       (20)        0 2024-04-05 09:52:59.000000 tn_observer-0.5.1/src/thinknet_observer/utils/__init__.py
+-rw-r--r--   0 sorapol    (502) staff       (20)      227 2024-04-05 09:52:59.000000 tn_observer-0.5.1/src/thinknet_observer/utils/bcolor.py
+-rw-r--r--   0 sorapol    (502) staff       (20)      587 2024-04-05 09:52:59.000000 tn_observer-0.5.1/src/thinknet_observer/utils/gunicorn_multiprocess.py
+-rw-r--r--   0 sorapol    (502) staff       (20)      599 2024-04-19 09:58:03.000000 tn_observer-0.5.1/src/thinknet_observer/utils/health.py
+-rw-r--r--   0 sorapol    (502) staff       (20)      627 2024-04-05 09:52:59.000000 tn_observer-0.5.1/src/thinknet_observer/utils/singleton.py
+drwxr-xr-x   0 sorapol    (502) staff       (20)        0 2024-05-31 09:58:43.369469 tn_observer-0.5.1/src/tn_observer.egg-info/
+-rw-r--r--   0 sorapol    (502) staff       (20)     7615 2024-05-31 09:58:43.000000 tn_observer-0.5.1/src/tn_observer.egg-info/PKG-INFO
+-rw-r--r--   0 sorapol    (502) staff       (20)     1074 2024-05-31 09:58:43.000000 tn_observer-0.5.1/src/tn_observer.egg-info/SOURCES.txt
+-rw-r--r--   0 sorapol    (502) staff       (20)        1 2024-05-31 09:58:43.000000 tn_observer-0.5.1/src/tn_observer.egg-info/dependency_links.txt
+-rw-r--r--   0 sorapol    (502) staff       (20)      359 2024-05-31 09:58:43.000000 tn_observer-0.5.1/src/tn_observer.egg-info/requires.txt
+-rw-r--r--   0 sorapol    (502) staff       (20)       18 2024-05-31 09:58:43.000000 tn_observer-0.5.1/src/tn_observer.egg-info/top_level.txt
+drwxr-xr-x   0 sorapol    (502) staff       (20)        0 2024-05-31 09:58:43.368715 tn_observer-0.5.1/tests/
+-rw-r--r--   0 sorapol    (502) staff       (20)     1523 2024-04-05 09:52:59.000000 tn_observer-0.5.1/tests/test_calculator.py
+-rw-r--r--   0 sorapol    (502) staff       (20)    30448 2024-05-31 09:47:45.000000 tn_observer-0.5.1/tests/test_metric_fastapi.py
+-rw-r--r--   0 sorapol    (502) staff       (20)    31043 2024-05-31 09:47:43.000000 tn_observer-0.5.1/tests/test_metric_flask.py
```

### Comparing `tn_observer-0.5.0/LICENSE.txt` & `tn_observer-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tn_observer-0.5.0/PKG-INFO` & `tn_observer-0.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tn-observer
-Version: 0.5.0
+Version: 0.5.1
 Summary: library for data observerability in our company THiNKNET via opentelemetry
 Author-email: capukampan <capukampan22@gmail.com>, THiNKNET <sorapol@thinknet.co.th>
 Keywords: thinknet,observerability
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: prometheus-client
@@ -29,18 +29,33 @@
 
 ## Installation
 ```
 pip install tn-observer
 ```
 
 
+## Prerequisites
+you should these enviroment in your `.env` file, 
+
+```env
+OTEL_EXPORTER_OTLP_ENDPOINT="[OTEL_ENDPOINT]"
+APP_VERSION="[APP_VERSION]"
+SERVICE_NAME_PREFIX="[SERVICE_NAME_PREFIX]"
+SERVICE_NAME="[SERVICE_NAME]"
+LOG_LEVEL="info"
+OTEL_DISABLE_TRACE="False" or "True"
+OTEL_PYTHON_EXCLUDED_URLS="hello,testy"
+
+```
+
+
 ## Get started
 1. in `main.py` or `server.py` import thinknet observer library
 ```python
-from src.thinknet_observer import TNObserver
+from thinknet_observer import TNObserver
 ``` 
 
 2. call setup otel 
 ```python
 tn_observer = TNObserver.with_default_service_info()
 
 tracer = TNObserver.setup_trace(__name__, tn_observer.resources)
@@ -52,16 +67,16 @@
 
 ### Flask Instrumentation
 
 ```python
 # import library
 from flask import Flask, request
 
-from src.thinknet_observer import TNObserver
-from src.thinknet_observer import FlaskLoggerMiddleware
+from thinknet_observer import TNObserver
+from thinknet_observer import FlaskLoggerMiddleware
 
 tn_observer = TNObserver.with_default_service_info()
 
 # create web server
 app = Flask(__name__)
 
 # trace setup
@@ -76,16 +91,16 @@
 
 ### FastAPI Instrumentation
 
 ```python
 # import libraries
 from fastapi import FastAPI, APIRouter
 
-from src.thinknet_observer import TNObserver
-from src.thinknet_observer import FastAPILogger
+from thinknet_observer import TNObserver
+from thinknet_observer import FastAPILogger
 
 tn_observer = TNObserver.with_default_service_info()
 
 app = FastAPI()
 router = APIRouter(route_class=FastAPILogger)
 
 TNObserver.register_metrics(app)
@@ -97,52 +112,52 @@
 
 
 ### pymongo instrumentation
 insert the commands to `mongo.py` or file with use pymongo 
 ex.
 
 ```python
-from src.thinknet_observer import TNObserver
+from thinknet_observer import TNObserver
 
 TNObserver.pymongo_instrumentation()
 client = pymongo.MongoClient(MONGO_URI)
 
 ```
 
 ### requests instrumentation
 when use lib requests to connect other services or graphQL
 example
 
 ```python
 import requests
-from src.thinknet_observer import TNObserver
+from thinknet_observer import TNObserver
 
 TNObserver.requests_instrumentation()
 res = request.get(url)
 
 ```
 
 ### kafka instrumentation
 
 ```python
-from src.thinknet_observer import TNObserver
+from thinknet_observer import TNObserver
 from kafka import KafkaProducer, KafkaConsumer
 
 TNObserver.kafka_instrumentation()
 
 producer = KafkaProducer(bootstrap_servers=["KAFKA_HOST"])
 ...
 ```
 
 
 
 ### LOGGING
 
 ```python
-from src.thinknet_observer import TNLogger, TNObserver
+from thinknet_observer import TNLogger, TNObserver
 
 # use if service name and service version in env #
 tn_observer = TNObserver.with_default_service_info()
 
 # use if not service name and service version in env #
 tn_observer = TNObserver(service_name, service_version)
 
@@ -154,15 +169,15 @@
 ```
 
 #### error logging
 
 1. in file such as `error.py`
 
 ```
-from src.thinknet_observer import TNAPIError
+from thinknet_observer import TNAPIError
 
 class DatabaseError(TNAPIError):
     http_status = 404
     message = "service can't connect database."
 
 ```
 2. in controller
@@ -174,15 +189,15 @@
     raise DatabaseError(service_code="service can't connect database.")
 ```
 
 
 ### custom tracing
 
 ```python
-from src.thinknet_observer import TNObserver
+from thinknet_observer import TNObserver
 
 tracer = TNObserver.setup_trace(__name__, tn_observer.resources)
 
 #sample function
 def do_roll():
     with tracer.start_as_current_span("do_roll") as rollspan:
         res =  randint(1, 6)
@@ -213,15 +228,15 @@
 
 ```
 
 
 #### gauge
 
 ```python
-from  thinknet_observer  import  MetricCollector
+from thinknet_observer  import  MetricCollector
 
 # NOTE: metrics name(1st param) must be unique for each metrics
 
 # Custom gauge 
 # (for gauge metrics if using multiprocess add param 'multiprocess_mode="livesum"')
 CUSTOM_GAUGE = MetricCollector.gauge(
     "CUSTOM_GAUGE", "desc of CUSTOM_GAUGE", ["something"]
@@ -244,15 +259,15 @@
     return {"msg": f"dec {number}"}
 
 ```
 
 #### histogram
 
 ```python
-from  thinknet_observer  import  MetricCollector
+from thinknet_observer import MetricCollector
 
 # Custom histogram
 CUSTOM_HISTOGRAM = MetricCollector.histogram(
     "CUSTOM_HISTOGRAM", "desc of CUSTOM_HISTOGRAM", ["something"]
 )
 CUSTOM_HISTOGRAM_NOLABEL = MetricCollector.histogram(
     "CUSTOM_HISTOGRAM_NOLABEL", "desc of CUSTOM_HISTOGRAM_NOLABEL"
@@ -276,15 +291,15 @@
     return {"msg": f"histogram_observe {number}"}
 
 ```
 
 #### summary
 
 ```python
-from  thinknet_observer  import  MetricCollector
+from thinknet_observer import  MetricCollector
 
 
 # Custom summary
 CUSTOM_SUMMARY = MetricCollector.summary(
     "CUSTOM_SUMMARY", "desc of CUSTOM_SUMMARY", ["something"]
 )
 CUSTOM_SUMMARY_NOLABEL = MetricCollector.summary(
```

### Comparing `tn_observer-0.5.0/README.md` & `tn_observer-0.5.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,18 +6,33 @@
 
 ## Installation
 ```
 pip install tn-observer
 ```
 
 
+## Prerequisites
+you should these enviroment in your `.env` file, 
+
+```env
+OTEL_EXPORTER_OTLP_ENDPOINT="[OTEL_ENDPOINT]"
+APP_VERSION="[APP_VERSION]"
+SERVICE_NAME_PREFIX="[SERVICE_NAME_PREFIX]"
+SERVICE_NAME="[SERVICE_NAME]"
+LOG_LEVEL="info"
+OTEL_DISABLE_TRACE="False" or "True"
+OTEL_PYTHON_EXCLUDED_URLS="hello,testy"
+
+```
+
+
 ## Get started
 1. in `main.py` or `server.py` import thinknet observer library
 ```python
-from src.thinknet_observer import TNObserver
+from thinknet_observer import TNObserver
 ``` 
 
 2. call setup otel 
 ```python
 tn_observer = TNObserver.with_default_service_info()
 
 tracer = TNObserver.setup_trace(__name__, tn_observer.resources)
@@ -29,16 +44,16 @@
 
 ### Flask Instrumentation
 
 ```python
 # import library
 from flask import Flask, request
 
-from src.thinknet_observer import TNObserver
-from src.thinknet_observer import FlaskLoggerMiddleware
+from thinknet_observer import TNObserver
+from thinknet_observer import FlaskLoggerMiddleware
 
 tn_observer = TNObserver.with_default_service_info()
 
 # create web server
 app = Flask(__name__)
 
 # trace setup
@@ -53,16 +68,16 @@
 
 ### FastAPI Instrumentation
 
 ```python
 # import libraries
 from fastapi import FastAPI, APIRouter
 
-from src.thinknet_observer import TNObserver
-from src.thinknet_observer import FastAPILogger
+from thinknet_observer import TNObserver
+from thinknet_observer import FastAPILogger
 
 tn_observer = TNObserver.with_default_service_info()
 
 app = FastAPI()
 router = APIRouter(route_class=FastAPILogger)
 
 TNObserver.register_metrics(app)
@@ -74,52 +89,52 @@
 
 
 ### pymongo instrumentation
 insert the commands to `mongo.py` or file with use pymongo 
 ex.
 
 ```python
-from src.thinknet_observer import TNObserver
+from thinknet_observer import TNObserver
 
 TNObserver.pymongo_instrumentation()
 client = pymongo.MongoClient(MONGO_URI)
 
 ```
 
 ### requests instrumentation
 when use lib requests to connect other services or graphQL
 example
 
 ```python
 import requests
-from src.thinknet_observer import TNObserver
+from thinknet_observer import TNObserver
 
 TNObserver.requests_instrumentation()
 res = request.get(url)
 
 ```
 
 ### kafka instrumentation
 
 ```python
-from src.thinknet_observer import TNObserver
+from thinknet_observer import TNObserver
 from kafka import KafkaProducer, KafkaConsumer
 
 TNObserver.kafka_instrumentation()
 
 producer = KafkaProducer(bootstrap_servers=["KAFKA_HOST"])
 ...
 ```
 
 
 
 ### LOGGING
 
 ```python
-from src.thinknet_observer import TNLogger, TNObserver
+from thinknet_observer import TNLogger, TNObserver
 
 # use if service name and service version in env #
 tn_observer = TNObserver.with_default_service_info()
 
 # use if not service name and service version in env #
 tn_observer = TNObserver(service_name, service_version)
 
@@ -131,15 +146,15 @@
 ```
 
 #### error logging
 
 1. in file such as `error.py`
 
 ```
-from src.thinknet_observer import TNAPIError
+from thinknet_observer import TNAPIError
 
 class DatabaseError(TNAPIError):
     http_status = 404
     message = "service can't connect database."
 
 ```
 2. in controller
@@ -151,15 +166,15 @@
     raise DatabaseError(service_code="service can't connect database.")
 ```
 
 
 ### custom tracing
 
 ```python
-from src.thinknet_observer import TNObserver
+from thinknet_observer import TNObserver
 
 tracer = TNObserver.setup_trace(__name__, tn_observer.resources)
 
 #sample function
 def do_roll():
     with tracer.start_as_current_span("do_roll") as rollspan:
         res =  randint(1, 6)
@@ -190,15 +205,15 @@
 
 ```
 
 
 #### gauge
 
 ```python
-from  thinknet_observer  import  MetricCollector
+from thinknet_observer  import  MetricCollector
 
 # NOTE: metrics name(1st param) must be unique for each metrics
 
 # Custom gauge 
 # (for gauge metrics if using multiprocess add param 'multiprocess_mode="livesum"')
 CUSTOM_GAUGE = MetricCollector.gauge(
     "CUSTOM_GAUGE", "desc of CUSTOM_GAUGE", ["something"]
@@ -221,15 +236,15 @@
     return {"msg": f"dec {number}"}
 
 ```
 
 #### histogram
 
 ```python
-from  thinknet_observer  import  MetricCollector
+from thinknet_observer import MetricCollector
 
 # Custom histogram
 CUSTOM_HISTOGRAM = MetricCollector.histogram(
     "CUSTOM_HISTOGRAM", "desc of CUSTOM_HISTOGRAM", ["something"]
 )
 CUSTOM_HISTOGRAM_NOLABEL = MetricCollector.histogram(
     "CUSTOM_HISTOGRAM_NOLABEL", "desc of CUSTOM_HISTOGRAM_NOLABEL"
@@ -253,15 +268,15 @@
     return {"msg": f"histogram_observe {number}"}
 
 ```
 
 #### summary
 
 ```python
-from  thinknet_observer  import  MetricCollector
+from thinknet_observer import  MetricCollector
 
 
 # Custom summary
 CUSTOM_SUMMARY = MetricCollector.summary(
     "CUSTOM_SUMMARY", "desc of CUSTOM_SUMMARY", ["something"]
 )
 CUSTOM_SUMMARY_NOLABEL = MetricCollector.summary(
```

### Comparing `tn_observer-0.5.0/pyproject.toml` & `tn_observer-0.5.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "tn-observer"
 authors = [
     {name = "capukampan", email = "capukampan22@gmail.com"},
     {name = "THiNKNET", email = "sorapol@thinknet.co.th"}
 ]
 description = "library for data observerability in our company THiNKNET via opentelemetry"
-version = "0.5.0"
+version = "0.5.1"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["thinknet", "observerability"]
 dependencies = [
     "prometheus-client",
     "Flask",
     "fastapi",
```

### Comparing `tn_observer-0.5.0/src/thinknet_observer/__init__.py` & `tn_observer-0.5.1/src/thinknet_observer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 from .loggers.fast_logger import FastAPILogger
 from .loggers.loggers import TNAPIError, TNLogger
 
 from .utils import health
 from .otel import TNObserver
 
 from .utils.singleton import SingletonMeta
-# from .utils.gunicorn_multiprocess import clear_multiproc_dir
+from .utils.gunicorn_multiprocess import clear_multiproc_dir
```

### Comparing `tn_observer-0.5.0/src/thinknet_observer/calulator.py` & `tn_observer-0.5.1/src/thinknet_observer/calulator.py`

 * *Files identical despite different names*

### Comparing `tn_observer-0.5.0/src/thinknet_observer/loggers/fast_logger.py` & `tn_observer-0.5.1/src/thinknet_observer/loggers/fast_logger.py`

 * *Files identical despite different names*

### Comparing `tn_observer-0.5.0/src/thinknet_observer/loggers/flask_logger.py` & `tn_observer-0.5.1/src/thinknet_observer/loggers/flask_logger.py`

 * *Files identical despite different names*

### Comparing `tn_observer-0.5.0/src/thinknet_observer/loggers/loggers.py` & `tn_observer-0.5.1/src/thinknet_observer/loggers/loggers.py`

 * *Files identical despite different names*

### Comparing `tn_observer-0.5.0/src/thinknet_observer/metrics/collector.py` & `tn_observer-0.5.1/src/thinknet_observer/metrics/collector.py`

 * *Files identical despite different names*

### Comparing `tn_observer-0.5.0/src/thinknet_observer/metrics/custom_metrics_wrapper.py` & `tn_observer-0.5.1/src/thinknet_observer/metrics/custom_metrics_wrapper.py`

 * *Files identical despite different names*

### Comparing `tn_observer-0.5.0/src/thinknet_observer/metrics/metrics.py` & `tn_observer-0.5.1/src/thinknet_observer/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `tn_observer-0.5.0/src/thinknet_observer/otel.py` & `tn_observer-0.5.1/src/thinknet_observer/otel.py`

 * *Files identical despite different names*

### Comparing `tn_observer-0.5.0/src/thinknet_observer/utils/gunicorn_multiprocess.py` & `tn_observer-0.5.1/src/thinknet_observer/utils/gunicorn_multiprocess.py`

 * *Files identical despite different names*

### Comparing `tn_observer-0.5.0/src/thinknet_observer/utils/health.py` & `tn_observer-0.5.1/src/thinknet_observer/utils/health.py`

 * *Files identical despite different names*

### Comparing `tn_observer-0.5.0/src/thinknet_observer/utils/singleton.py` & `tn_observer-0.5.1/src/thinknet_observer/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `tn_observer-0.5.0/src/tn_observer.egg-info/PKG-INFO` & `tn_observer-0.5.1/src/tn_observer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tn-observer
-Version: 0.5.0
+Version: 0.5.1
 Summary: library for data observerability in our company THiNKNET via opentelemetry
 Author-email: capukampan <capukampan22@gmail.com>, THiNKNET <sorapol@thinknet.co.th>
 Keywords: thinknet,observerability
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: prometheus-client
@@ -29,18 +29,33 @@
 
 ## Installation
 ```
 pip install tn-observer
 ```
 
 
+## Prerequisites
+you should these enviroment in your `.env` file, 
+
+```env
+OTEL_EXPORTER_OTLP_ENDPOINT="[OTEL_ENDPOINT]"
+APP_VERSION="[APP_VERSION]"
+SERVICE_NAME_PREFIX="[SERVICE_NAME_PREFIX]"
+SERVICE_NAME="[SERVICE_NAME]"
+LOG_LEVEL="info"
+OTEL_DISABLE_TRACE="False" or "True"
+OTEL_PYTHON_EXCLUDED_URLS="hello,testy"
+
+```
+
+
 ## Get started
 1. in `main.py` or `server.py` import thinknet observer library
 ```python
-from src.thinknet_observer import TNObserver
+from thinknet_observer import TNObserver
 ``` 
 
 2. call setup otel 
 ```python
 tn_observer = TNObserver.with_default_service_info()
 
 tracer = TNObserver.setup_trace(__name__, tn_observer.resources)
@@ -52,16 +67,16 @@
 
 ### Flask Instrumentation
 
 ```python
 # import library
 from flask import Flask, request
 
-from src.thinknet_observer import TNObserver
-from src.thinknet_observer import FlaskLoggerMiddleware
+from thinknet_observer import TNObserver
+from thinknet_observer import FlaskLoggerMiddleware
 
 tn_observer = TNObserver.with_default_service_info()
 
 # create web server
 app = Flask(__name__)
 
 # trace setup
@@ -76,16 +91,16 @@
 
 ### FastAPI Instrumentation
 
 ```python
 # import libraries
 from fastapi import FastAPI, APIRouter
 
-from src.thinknet_observer import TNObserver
-from src.thinknet_observer import FastAPILogger
+from thinknet_observer import TNObserver
+from thinknet_observer import FastAPILogger
 
 tn_observer = TNObserver.with_default_service_info()
 
 app = FastAPI()
 router = APIRouter(route_class=FastAPILogger)
 
 TNObserver.register_metrics(app)
@@ -97,52 +112,52 @@
 
 
 ### pymongo instrumentation
 insert the commands to `mongo.py` or file with use pymongo 
 ex.
 
 ```python
-from src.thinknet_observer import TNObserver
+from thinknet_observer import TNObserver
 
 TNObserver.pymongo_instrumentation()
 client = pymongo.MongoClient(MONGO_URI)
 
 ```
 
 ### requests instrumentation
 when use lib requests to connect other services or graphQL
 example
 
 ```python
 import requests
-from src.thinknet_observer import TNObserver
+from thinknet_observer import TNObserver
 
 TNObserver.requests_instrumentation()
 res = request.get(url)
 
 ```
 
 ### kafka instrumentation
 
 ```python
-from src.thinknet_observer import TNObserver
+from thinknet_observer import TNObserver
 from kafka import KafkaProducer, KafkaConsumer
 
 TNObserver.kafka_instrumentation()
 
 producer = KafkaProducer(bootstrap_servers=["KAFKA_HOST"])
 ...
 ```
 
 
 
 ### LOGGING
 
 ```python
-from src.thinknet_observer import TNLogger, TNObserver
+from thinknet_observer import TNLogger, TNObserver
 
 # use if service name and service version in env #
 tn_observer = TNObserver.with_default_service_info()
 
 # use if not service name and service version in env #
 tn_observer = TNObserver(service_name, service_version)
 
@@ -154,15 +169,15 @@
 ```
 
 #### error logging
 
 1. in file such as `error.py`
 
 ```
-from src.thinknet_observer import TNAPIError
+from thinknet_observer import TNAPIError
 
 class DatabaseError(TNAPIError):
     http_status = 404
     message = "service can't connect database."
 
 ```
 2. in controller
@@ -174,15 +189,15 @@
     raise DatabaseError(service_code="service can't connect database.")
 ```
 
 
 ### custom tracing
 
 ```python
-from src.thinknet_observer import TNObserver
+from thinknet_observer import TNObserver
 
 tracer = TNObserver.setup_trace(__name__, tn_observer.resources)
 
 #sample function
 def do_roll():
     with tracer.start_as_current_span("do_roll") as rollspan:
         res =  randint(1, 6)
@@ -213,15 +228,15 @@
 
 ```
 
 
 #### gauge
 
 ```python
-from  thinknet_observer  import  MetricCollector
+from thinknet_observer  import  MetricCollector
 
 # NOTE: metrics name(1st param) must be unique for each metrics
 
 # Custom gauge 
 # (for gauge metrics if using multiprocess add param 'multiprocess_mode="livesum"')
 CUSTOM_GAUGE = MetricCollector.gauge(
     "CUSTOM_GAUGE", "desc of CUSTOM_GAUGE", ["something"]
@@ -244,15 +259,15 @@
     return {"msg": f"dec {number}"}
 
 ```
 
 #### histogram
 
 ```python
-from  thinknet_observer  import  MetricCollector
+from thinknet_observer import MetricCollector
 
 # Custom histogram
 CUSTOM_HISTOGRAM = MetricCollector.histogram(
     "CUSTOM_HISTOGRAM", "desc of CUSTOM_HISTOGRAM", ["something"]
 )
 CUSTOM_HISTOGRAM_NOLABEL = MetricCollector.histogram(
     "CUSTOM_HISTOGRAM_NOLABEL", "desc of CUSTOM_HISTOGRAM_NOLABEL"
@@ -276,15 +291,15 @@
     return {"msg": f"histogram_observe {number}"}
 
 ```
 
 #### summary
 
 ```python
-from  thinknet_observer  import  MetricCollector
+from thinknet_observer import  MetricCollector
 
 
 # Custom summary
 CUSTOM_SUMMARY = MetricCollector.summary(
     "CUSTOM_SUMMARY", "desc of CUSTOM_SUMMARY", ["something"]
 )
 CUSTOM_SUMMARY_NOLABEL = MetricCollector.summary(
```

### Comparing `tn_observer-0.5.0/src/tn_observer.egg-info/SOURCES.txt` & `tn_observer-0.5.1/src/tn_observer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tn_observer-0.5.0/tests/test_calculator.py` & `tn_observer-0.5.1/tests/test_calculator.py`

 * *Files identical despite different names*

### Comparing `tn_observer-0.5.0/tests/test_metric_fastapi.py` & `tn_observer-0.5.1/tests/test_metric_fastapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import time
 from flask import Flask
 from flask_cors import CORS
 from fastapi import FastAPI
 from fastapi.testclient import TestClient
 
 
-from src.thinknet_observer import TNObserver, PrometheusMiddleware
+from src.thinknet_observer import TNObserver
 from src.thinknet_observer import SingletonMeta
 from src.thinknet_observer import MetricCollector
 
 from src.thinknet_observer.metrics.config import NAMESPACE, SERVICENAME
 
 
 CUSTOM_GAUGE = MetricCollector.gauge(
```

### Comparing `tn_observer-0.5.0/tests/test_metric_flask.py` & `tn_observer-0.5.1/tests/test_metric_flask.py`

 * *Files identical despite different names*

