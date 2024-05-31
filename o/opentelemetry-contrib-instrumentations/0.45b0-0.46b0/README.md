# Comparing `tmp/opentelemetry_contrib_instrumentations-0.45b0.tar.gz` & `tmp/opentelemetry_contrib_instrumentations-0.46b0.tar.gz`

## Comparing `opentelemetry_contrib_instrumentations-0.45b0.tar` & `opentelemetry_contrib_instrumentations-0.46b0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_contrib_instrumentations-0.45b0/src/opentelemetry/contrib-instrumentations/version.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_contrib_instrumentations-0.45b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_contrib_instrumentations-0.45b0/LICENSE
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 opentelemetry_contrib_instrumentations-0.45b0/README.rst
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 opentelemetry_contrib_instrumentations-0.45b0/pyproject.toml
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 opentelemetry_contrib_instrumentations-0.45b0/PKG-INFO
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_contrib_instrumentations-0.46b0/src/opentelemetry/contrib-instrumentations/version.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_contrib_instrumentations-0.46b0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 opentelemetry_contrib_instrumentations-0.46b0/LICENSE
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 opentelemetry_contrib_instrumentations-0.46b0/README.rst
+-rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 opentelemetry_contrib_instrumentations-0.46b0/pyproject.toml
+-rw-r--r--   0        0        0     4522 2020-02-02 00:00:00.000000 opentelemetry_contrib_instrumentations-0.46b0/PKG-INFO
```

### Comparing `opentelemetry_contrib_instrumentations-0.45b0/src/opentelemetry/contrib-instrumentations/version.py` & `opentelemetry_contrib_instrumentations-0.46b0/src/opentelemetry/contrib-instrumentations/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.45b0"
+__version__ = "0.46b0"
```

### Comparing `opentelemetry_contrib_instrumentations-0.45b0/LICENSE` & `opentelemetry_contrib_instrumentations-0.46b0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright The OpenTelemetry Authors
+   Copyright [yyyy] [name of copyright owner]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `opentelemetry_contrib_instrumentations-0.45b0/README.rst` & `opentelemetry_contrib_instrumentations-0.46b0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,14 @@
 
 ::
 
     pip install opentelemetry-contrib-instrumentations
 
 
 This package installs all instrumentation packages hosted by the OpenTelemetry Python Contrib repository.
-The list of packages can be found (here)[https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation]
+The list of packages can be found `here <https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation>`_.
 
 
 References
 ----------
 
 * `OpenTelemetry Project <https://opentelemetry.io/>`_
```

### Comparing `opentelemetry_contrib_instrumentations-0.45b0/pyproject.toml` & `opentelemetry_contrib_instrumentations-0.46b0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -24,61 +24,62 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "opentelemetry-instrumentation-aio-pika==0.45b0",
-    "opentelemetry-instrumentation-aiohttp-client==0.45b0",
-    "opentelemetry-instrumentation-aiohttp-server==0.45b0",
-    "opentelemetry-instrumentation-aiopg==0.45b0",
-    "opentelemetry-instrumentation-asgi==0.45b0",
-    "opentelemetry-instrumentation-asyncio==0.45b0",
-    "opentelemetry-instrumentation-asyncpg==0.45b0",
-    "opentelemetry-instrumentation-aws-lambda==0.45b0",
-    "opentelemetry-instrumentation-boto==0.45b0",
-    "opentelemetry-instrumentation-boto3sqs==0.45b0",
-    "opentelemetry-instrumentation-botocore==0.45b0",
-    "opentelemetry-instrumentation-cassandra==0.45b0",
-    "opentelemetry-instrumentation-celery==0.45b0",
-    "opentelemetry-instrumentation-confluent-kafka==0.45b0",
-    "opentelemetry-instrumentation-dbapi==0.45b0",
-    "opentelemetry-instrumentation-django==0.45b0",
-    "opentelemetry-instrumentation-elasticsearch==0.45b0",
-    "opentelemetry-instrumentation-falcon==0.45b0",
-    "opentelemetry-instrumentation-fastapi==0.45b0",
-    "opentelemetry-instrumentation-flask==0.45b0",
-    "opentelemetry-instrumentation-grpc==0.45b0",
-    "opentelemetry-instrumentation-httpx==0.45b0",
-    "opentelemetry-instrumentation-jinja2==0.45b0",
-    "opentelemetry-instrumentation-kafka-python==0.45b0",
-    "opentelemetry-instrumentation-logging==0.45b0",
-    "opentelemetry-instrumentation-mysql==0.45b0",
-    "opentelemetry-instrumentation-mysqlclient==0.45b0",
-    "opentelemetry-instrumentation-pika==0.45b0",
-    "opentelemetry-instrumentation-psycopg==0.45b0",
-    "opentelemetry-instrumentation-psycopg2==0.45b0",
-    "opentelemetry-instrumentation-pymemcache==0.45b0",
-    "opentelemetry-instrumentation-pymongo==0.45b0",
-    "opentelemetry-instrumentation-pymysql==0.45b0",
-    "opentelemetry-instrumentation-pyramid==0.45b0",
-    "opentelemetry-instrumentation-redis==0.45b0",
-    "opentelemetry-instrumentation-remoulade==0.45b0",
-    "opentelemetry-instrumentation-requests==0.45b0",
-    "opentelemetry-instrumentation-sklearn==0.45b0",
-    "opentelemetry-instrumentation-sqlalchemy==0.45b0",
-    "opentelemetry-instrumentation-sqlite3==0.45b0",
-    "opentelemetry-instrumentation-starlette==0.45b0",
-    "opentelemetry-instrumentation-system-metrics==0.45b0",
-    "opentelemetry-instrumentation-tornado==0.45b0",
-    "opentelemetry-instrumentation-tortoiseorm==0.45b0",
-    "opentelemetry-instrumentation-urllib==0.45b0",
-    "opentelemetry-instrumentation-urllib3==0.45b0",
-    "opentelemetry-instrumentation-wsgi==0.45b0",
+    "opentelemetry-instrumentation-aio-pika==0.46b0",
+    "opentelemetry-instrumentation-aiohttp-client==0.46b0",
+    "opentelemetry-instrumentation-aiohttp-server==0.46b0",
+    "opentelemetry-instrumentation-aiopg==0.46b0",
+    "opentelemetry-instrumentation-asgi==0.46b0",
+    "opentelemetry-instrumentation-asyncio==0.46b0",
+    "opentelemetry-instrumentation-asyncpg==0.46b0",
+    "opentelemetry-instrumentation-aws-lambda==0.46b0",
+    "opentelemetry-instrumentation-boto==0.46b0",
+    "opentelemetry-instrumentation-boto3sqs==0.46b0",
+    "opentelemetry-instrumentation-botocore==0.46b0",
+    "opentelemetry-instrumentation-cassandra==0.46b0",
+    "opentelemetry-instrumentation-celery==0.46b0",
+    "opentelemetry-instrumentation-confluent-kafka==0.46b0",
+    "opentelemetry-instrumentation-dbapi==0.46b0",
+    "opentelemetry-instrumentation-django==0.46b0",
+    "opentelemetry-instrumentation-elasticsearch==0.46b0",
+    "opentelemetry-instrumentation-falcon==0.46b0",
+    "opentelemetry-instrumentation-fastapi==0.46b0",
+    "opentelemetry-instrumentation-flask==0.46b0",
+    "opentelemetry-instrumentation-grpc==0.46b0",
+    "opentelemetry-instrumentation-httpx==0.46b0",
+    "opentelemetry-instrumentation-jinja2==0.46b0",
+    "opentelemetry-instrumentation-kafka-python==0.46b0",
+    "opentelemetry-instrumentation-logging==0.46b0",
+    "opentelemetry-instrumentation-mysql==0.46b0",
+    "opentelemetry-instrumentation-mysqlclient==0.46b0",
+    "opentelemetry-instrumentation-pika==0.46b0",
+    "opentelemetry-instrumentation-psycopg==0.46b0",
+    "opentelemetry-instrumentation-psycopg2==0.46b0",
+    "opentelemetry-instrumentation-pymemcache==0.46b0",
+    "opentelemetry-instrumentation-pymongo==0.46b0",
+    "opentelemetry-instrumentation-pymysql==0.46b0",
+    "opentelemetry-instrumentation-pyramid==0.46b0",
+    "opentelemetry-instrumentation-redis==0.46b0",
+    "opentelemetry-instrumentation-remoulade==0.46b0",
+    "opentelemetry-instrumentation-requests==0.46b0",
+    "opentelemetry-instrumentation-sklearn==0.46b0",
+    "opentelemetry-instrumentation-sqlalchemy==0.46b0",
+    "opentelemetry-instrumentation-sqlite3==0.46b0",
+    "opentelemetry-instrumentation-starlette==0.46b0",
+    "opentelemetry-instrumentation-system-metrics==0.46b0",
+    "opentelemetry-instrumentation-threading==0.46b0",
+    "opentelemetry-instrumentation-tornado==0.46b0",
+    "opentelemetry-instrumentation-tortoiseorm==0.46b0",
+    "opentelemetry-instrumentation-urllib==0.46b0",
+    "opentelemetry-instrumentation-urllib3==0.46b0",
+    "opentelemetry-instrumentation-wsgi==0.46b0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/opentelemetry-contrib-instrumentations"
 
 [tool.hatch.version]
 path = "src/opentelemetry/contrib-instrumentations/version.py"
```

### Comparing `opentelemetry_contrib_instrumentations-0.45b0/PKG-INFO` & `opentelemetry_contrib_instrumentations-0.46b0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: opentelemetry-contrib-instrumentations
-Version: 0.45b0
+Version: 0.46b0
 Summary: OpenTelemetry Contrib Instrumentation Packages
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/opentelemetry-contrib-instrumentations
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -12,61 +12,62 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
-Requires-Dist: opentelemetry-instrumentation-aio-pika==0.45b0
-Requires-Dist: opentelemetry-instrumentation-aiohttp-client==0.45b0
-Requires-Dist: opentelemetry-instrumentation-aiohttp-server==0.45b0
-Requires-Dist: opentelemetry-instrumentation-aiopg==0.45b0
-Requires-Dist: opentelemetry-instrumentation-asgi==0.45b0
-Requires-Dist: opentelemetry-instrumentation-asyncio==0.45b0
-Requires-Dist: opentelemetry-instrumentation-asyncpg==0.45b0
-Requires-Dist: opentelemetry-instrumentation-aws-lambda==0.45b0
-Requires-Dist: opentelemetry-instrumentation-boto3sqs==0.45b0
-Requires-Dist: opentelemetry-instrumentation-boto==0.45b0
-Requires-Dist: opentelemetry-instrumentation-botocore==0.45b0
-Requires-Dist: opentelemetry-instrumentation-cassandra==0.45b0
-Requires-Dist: opentelemetry-instrumentation-celery==0.45b0
-Requires-Dist: opentelemetry-instrumentation-confluent-kafka==0.45b0
-Requires-Dist: opentelemetry-instrumentation-dbapi==0.45b0
-Requires-Dist: opentelemetry-instrumentation-django==0.45b0
-Requires-Dist: opentelemetry-instrumentation-elasticsearch==0.45b0
-Requires-Dist: opentelemetry-instrumentation-falcon==0.45b0
-Requires-Dist: opentelemetry-instrumentation-fastapi==0.45b0
-Requires-Dist: opentelemetry-instrumentation-flask==0.45b0
-Requires-Dist: opentelemetry-instrumentation-grpc==0.45b0
-Requires-Dist: opentelemetry-instrumentation-httpx==0.45b0
-Requires-Dist: opentelemetry-instrumentation-jinja2==0.45b0
-Requires-Dist: opentelemetry-instrumentation-kafka-python==0.45b0
-Requires-Dist: opentelemetry-instrumentation-logging==0.45b0
-Requires-Dist: opentelemetry-instrumentation-mysql==0.45b0
-Requires-Dist: opentelemetry-instrumentation-mysqlclient==0.45b0
-Requires-Dist: opentelemetry-instrumentation-pika==0.45b0
-Requires-Dist: opentelemetry-instrumentation-psycopg2==0.45b0
-Requires-Dist: opentelemetry-instrumentation-psycopg==0.45b0
-Requires-Dist: opentelemetry-instrumentation-pymemcache==0.45b0
-Requires-Dist: opentelemetry-instrumentation-pymongo==0.45b0
-Requires-Dist: opentelemetry-instrumentation-pymysql==0.45b0
-Requires-Dist: opentelemetry-instrumentation-pyramid==0.45b0
-Requires-Dist: opentelemetry-instrumentation-redis==0.45b0
-Requires-Dist: opentelemetry-instrumentation-remoulade==0.45b0
-Requires-Dist: opentelemetry-instrumentation-requests==0.45b0
-Requires-Dist: opentelemetry-instrumentation-sklearn==0.45b0
-Requires-Dist: opentelemetry-instrumentation-sqlalchemy==0.45b0
-Requires-Dist: opentelemetry-instrumentation-sqlite3==0.45b0
-Requires-Dist: opentelemetry-instrumentation-starlette==0.45b0
-Requires-Dist: opentelemetry-instrumentation-system-metrics==0.45b0
-Requires-Dist: opentelemetry-instrumentation-tornado==0.45b0
-Requires-Dist: opentelemetry-instrumentation-tortoiseorm==0.45b0
-Requires-Dist: opentelemetry-instrumentation-urllib3==0.45b0
-Requires-Dist: opentelemetry-instrumentation-urllib==0.45b0
-Requires-Dist: opentelemetry-instrumentation-wsgi==0.45b0
+Requires-Dist: opentelemetry-instrumentation-aio-pika==0.46b0
+Requires-Dist: opentelemetry-instrumentation-aiohttp-client==0.46b0
+Requires-Dist: opentelemetry-instrumentation-aiohttp-server==0.46b0
+Requires-Dist: opentelemetry-instrumentation-aiopg==0.46b0
+Requires-Dist: opentelemetry-instrumentation-asgi==0.46b0
+Requires-Dist: opentelemetry-instrumentation-asyncio==0.46b0
+Requires-Dist: opentelemetry-instrumentation-asyncpg==0.46b0
+Requires-Dist: opentelemetry-instrumentation-aws-lambda==0.46b0
+Requires-Dist: opentelemetry-instrumentation-boto3sqs==0.46b0
+Requires-Dist: opentelemetry-instrumentation-boto==0.46b0
+Requires-Dist: opentelemetry-instrumentation-botocore==0.46b0
+Requires-Dist: opentelemetry-instrumentation-cassandra==0.46b0
+Requires-Dist: opentelemetry-instrumentation-celery==0.46b0
+Requires-Dist: opentelemetry-instrumentation-confluent-kafka==0.46b0
+Requires-Dist: opentelemetry-instrumentation-dbapi==0.46b0
+Requires-Dist: opentelemetry-instrumentation-django==0.46b0
+Requires-Dist: opentelemetry-instrumentation-elasticsearch==0.46b0
+Requires-Dist: opentelemetry-instrumentation-falcon==0.46b0
+Requires-Dist: opentelemetry-instrumentation-fastapi==0.46b0
+Requires-Dist: opentelemetry-instrumentation-flask==0.46b0
+Requires-Dist: opentelemetry-instrumentation-grpc==0.46b0
+Requires-Dist: opentelemetry-instrumentation-httpx==0.46b0
+Requires-Dist: opentelemetry-instrumentation-jinja2==0.46b0
+Requires-Dist: opentelemetry-instrumentation-kafka-python==0.46b0
+Requires-Dist: opentelemetry-instrumentation-logging==0.46b0
+Requires-Dist: opentelemetry-instrumentation-mysql==0.46b0
+Requires-Dist: opentelemetry-instrumentation-mysqlclient==0.46b0
+Requires-Dist: opentelemetry-instrumentation-pika==0.46b0
+Requires-Dist: opentelemetry-instrumentation-psycopg2==0.46b0
+Requires-Dist: opentelemetry-instrumentation-psycopg==0.46b0
+Requires-Dist: opentelemetry-instrumentation-pymemcache==0.46b0
+Requires-Dist: opentelemetry-instrumentation-pymongo==0.46b0
+Requires-Dist: opentelemetry-instrumentation-pymysql==0.46b0
+Requires-Dist: opentelemetry-instrumentation-pyramid==0.46b0
+Requires-Dist: opentelemetry-instrumentation-redis==0.46b0
+Requires-Dist: opentelemetry-instrumentation-remoulade==0.46b0
+Requires-Dist: opentelemetry-instrumentation-requests==0.46b0
+Requires-Dist: opentelemetry-instrumentation-sklearn==0.46b0
+Requires-Dist: opentelemetry-instrumentation-sqlalchemy==0.46b0
+Requires-Dist: opentelemetry-instrumentation-sqlite3==0.46b0
+Requires-Dist: opentelemetry-instrumentation-starlette==0.46b0
+Requires-Dist: opentelemetry-instrumentation-system-metrics==0.46b0
+Requires-Dist: opentelemetry-instrumentation-threading==0.46b0
+Requires-Dist: opentelemetry-instrumentation-tornado==0.46b0
+Requires-Dist: opentelemetry-instrumentation-tortoiseorm==0.46b0
+Requires-Dist: opentelemetry-instrumentation-urllib3==0.46b0
+Requires-Dist: opentelemetry-instrumentation-urllib==0.46b0
+Requires-Dist: opentelemetry-instrumentation-wsgi==0.46b0
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Instrumentation
 =============================
 
 |pypi|
 
@@ -78,14 +79,14 @@
 
 ::
 
     pip install opentelemetry-contrib-instrumentations
 
 
 This package installs all instrumentation packages hosted by the OpenTelemetry Python Contrib repository.
-The list of packages can be found (here)[https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation]
+The list of packages can be found `here <https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation>`_.
 
 
 References
 ----------
 
 * `OpenTelemetry Project <https://opentelemetry.io/>`_
```

