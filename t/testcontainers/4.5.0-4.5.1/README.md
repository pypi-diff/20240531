# Comparing `tmp/testcontainers-4.5.0.tar.gz` & `tmp/testcontainers-4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testcontainers-4.5.0.tar", max compression
+gzip compressed data, was "testcontainers-4.5.1.tar", max compression
```

## Comparing `testcontainers-4.5.0.tar` & `testcontainers-4.5.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    11328 2024-05-25 19:37:09.791271 testcontainers-4.5.0/LICENSE.txt
--rw-r--r--   0        0        0     2042 2024-05-25 19:37:09.791271 testcontainers-4.5.0/README.md
--rw-r--r--   0        0        0      172 2024-05-25 19:37:09.791271 testcontainers-4.5.0/core/testcontainers/compose/__init__.py
--rw-r--r--   0        0        0    13448 2024-05-25 19:37:09.791271 testcontainers-4.5.0/core/testcontainers/compose/compose.py
--rw-r--r--   0        0        0        0 2024-05-25 19:37:09.791271 testcontainers-4.5.0/core/testcontainers/core/__init__.py
--rw-r--r--   0        0        0     3157 2024-05-25 19:37:09.791271 testcontainers-4.5.0/core/testcontainers/core/config.py
--rw-r--r--   0        0        0     8877 2024-05-25 19:37:09.791271 testcontainers-4.5.0/core/testcontainers/core/container.py
--rw-r--r--   0        0        0     7503 2024-05-25 19:37:09.791271 testcontainers-4.5.0/core/testcontainers/core/docker_client.py
--rw-r--r--   0        0        0      734 2024-05-25 19:37:09.791271 testcontainers-4.5.0/core/testcontainers/core/exceptions.py
--rw-r--r--   0        0        0     2591 2024-05-25 19:37:09.791271 testcontainers-4.5.0/core/testcontainers/core/generic.py
--rw-r--r--   0        0        0      979 2024-05-25 19:37:09.791271 testcontainers-4.5.0/core/testcontainers/core/labels.py
--rw-r--r--   0        0        0     1543 2024-05-25 19:37:09.791271 testcontainers-4.5.0/core/testcontainers/core/network.py
--rw-r--r--   0        0        0     3108 2024-05-25 19:37:09.791271 testcontainers-4.5.0/core/testcontainers/core/utils.py
--rw-r--r--   0        0        0     4069 2024-05-25 19:37:09.791271 testcontainers-4.5.0/core/testcontainers/core/waiting_utils.py
--rw-r--r--   0        0        0     3781 2024-05-25 19:37:09.791271 testcontainers-4.5.0/modules/arangodb/testcontainers/arangodb/__init__.py
--rw-r--r--   0        0        0     4385 2024-05-25 19:37:09.791271 testcontainers-4.5.0/modules/azurite/testcontainers/azurite/__init__.py
--rw-r--r--   0        0        0     2492 2024-05-25 19:37:09.791271 testcontainers-4.5.0/modules/cassandra/testcontainers/cassandra/__init__.py
--rw-r--r--   0        0        0     2736 2024-05-25 19:37:09.791271 testcontainers-4.5.0/modules/chroma/testcontainers/chroma/__init__.py
--rw-r--r--   0        0        0     3030 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/clickhouse/testcontainers/clickhouse/__init__.py
--rw-r--r--   0        0        0     3886 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/elasticsearch/testcontainers/elasticsearch/__init__.py
--rw-r--r--   0        0        0      106 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/google/testcontainers/google/__init__.py
--rw-r--r--   0        0        0     2709 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/google/testcontainers/google/datastore.py
--rw-r--r--   0        0        0     2952 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/google/testcontainers/google/pubsub.py
--rw-r--r--   0        0        0     3760 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/influxdb/testcontainers/influxdb.py
--rw-r--r--   0        0        0     2387 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/influxdb/testcontainers/influxdb1/__init__.py
--rw-r--r--   0        0        0     4464 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/influxdb/testcontainers/influxdb2/__init__.py
--rw-r--r--   0        0        0     2694 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/k3s/testcontainers/k3s/__init__.py
--rw-r--r--   0        0        0     3592 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/kafka/testcontainers/kafka/__init__.py
--rw-r--r--   0        0        0     2727 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/kafka/testcontainers/kafka/_redpanda.py
--rw-r--r--   0        0        0     4249 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/keycloak/testcontainers/keycloak/__init__.py
--rw-r--r--   0        0        0     3222 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/localstack/testcontainers/localstack/__init__.py
--rw-r--r--   0        0        0     2042 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/memcached/testcontainers/memcached/__init__.py
--rw-r--r--   0        0        0     4116 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/minio/testcontainers/minio/__init__.py
--rw-r--r--   0        0        0     3017 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/mongodb/testcontainers/mongodb/__init__.py
--rw-r--r--   0        0        0     2202 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/mssql/testcontainers/mssql/__init__.py
--rw-r--r--   0        0        0     4984 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/mysql/testcontainers/mysql/__init__.py
--rw-r--r--   0        0        0     2811 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/nats/testcontainers/nats/__init__.py
--rw-r--r--   0        0        0     2782 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/neo4j/testcontainers/neo4j/__init__.py
--rw-r--r--   0        0        0     1596 2024-05-25 19:37:09.799271 testcontainers-4.5.0/modules/nginx/testcontainers/nginx/__init__.py
--rw-r--r--   0        0        0     4109 2024-05-25 19:37:09.799271 testcontainers-4.5.0/modules/opensearch/testcontainers/opensearch/__init__.py
--rw-r--r--   0        0        0     2960 2024-05-25 19:37:09.799271 testcontainers-4.5.0/modules/oracle-free/testcontainers/oracle/__init__.py
--rw-r--r--   0        0        0     3984 2024-05-25 19:37:09.799271 testcontainers-4.5.0/modules/postgres/testcontainers/postgres/__init__.py
--rw-r--r--   0        0        0     5209 2024-05-25 19:37:09.799271 testcontainers-4.5.0/modules/qdrant/testcontainers/qdrant/__init__.py
--rw-r--r--   0        0        0     2967 2024-05-25 19:37:09.799271 testcontainers-4.5.0/modules/rabbitmq/testcontainers/rabbitmq/__init__.py
--rw-r--r--   0        0        0     3144 2024-05-25 19:37:09.799271 testcontainers-4.5.0/modules/redis/testcontainers/redis/__init__.py
--rw-r--r--   0        0        0     2761 2024-05-25 19:37:09.799271 testcontainers-4.5.0/modules/registry/testcontainers/registry/__init__.py
--rw-r--r--   0        0        0     4272 2024-05-25 19:37:09.799271 testcontainers-4.5.0/modules/selenium/testcontainers/selenium/__init__.py
--rw-r--r--   0        0        0     1432 2024-05-25 19:37:09.799271 testcontainers-4.5.0/modules/selenium/testcontainers/selenium/video.py
--rw-r--r--   0        0        0     2519 2024-05-25 19:37:09.799271 testcontainers-4.5.0/modules/vault/testcontainers/vault/__init__.py
--rw-r--r--   0        0        0     5589 2024-05-25 19:37:09.799271 testcontainers-4.5.0/modules/weaviate/testcontainers/weaviate/__init__.py
--rw-r--r--   0        0        0     8834 2024-05-25 19:37:09.803271 testcontainers-4.5.0/pyproject.toml
--rw-r--r--   0        0        0     5554 1970-01-01 00:00:00.000000 testcontainers-4.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11328 2024-05-31 09:20:48.616634 testcontainers-4.5.1/LICENSE.txt
+-rw-r--r--   0        0        0     2042 2024-05-31 09:20:48.616634 testcontainers-4.5.1/README.md
+-rw-r--r--   0        0        0      172 2024-05-31 09:20:48.616634 testcontainers-4.5.1/core/testcontainers/compose/__init__.py
+-rw-r--r--   0        0        0    13448 2024-05-31 09:20:48.616634 testcontainers-4.5.1/core/testcontainers/compose/compose.py
+-rw-r--r--   0        0        0        0 2024-05-31 09:20:48.616634 testcontainers-4.5.1/core/testcontainers/core/__init__.py
+-rw-r--r--   0        0        0     3157 2024-05-31 09:20:48.616634 testcontainers-4.5.1/core/testcontainers/core/config.py
+-rw-r--r--   0        0        0     8877 2024-05-31 09:20:48.616634 testcontainers-4.5.1/core/testcontainers/core/container.py
+-rw-r--r--   0        0        0     7503 2024-05-31 09:20:48.616634 testcontainers-4.5.1/core/testcontainers/core/docker_client.py
+-rw-r--r--   0        0        0      734 2024-05-31 09:20:48.616634 testcontainers-4.5.1/core/testcontainers/core/exceptions.py
+-rw-r--r--   0        0        0     2591 2024-05-31 09:20:48.616634 testcontainers-4.5.1/core/testcontainers/core/generic.py
+-rw-r--r--   0        0        0      979 2024-05-31 09:20:48.616634 testcontainers-4.5.1/core/testcontainers/core/labels.py
+-rw-r--r--   0        0        0     1543 2024-05-31 09:20:48.616634 testcontainers-4.5.1/core/testcontainers/core/network.py
+-rw-r--r--   0        0        0     3108 2024-05-31 09:20:48.616634 testcontainers-4.5.1/core/testcontainers/core/utils.py
+-rw-r--r--   0        0        0     4069 2024-05-31 09:20:48.616634 testcontainers-4.5.1/core/testcontainers/core/waiting_utils.py
+-rw-r--r--   0        0        0     3781 2024-05-31 09:20:48.616634 testcontainers-4.5.1/modules/arangodb/testcontainers/arangodb/__init__.py
+-rw-r--r--   0        0        0     4385 2024-05-31 09:20:48.620634 testcontainers-4.5.1/modules/azurite/testcontainers/azurite/__init__.py
+-rw-r--r--   0        0        0     2492 2024-05-31 09:20:48.620634 testcontainers-4.5.1/modules/cassandra/testcontainers/cassandra/__init__.py
+-rw-r--r--   0        0        0     2736 2024-05-31 09:20:48.620634 testcontainers-4.5.1/modules/chroma/testcontainers/chroma/__init__.py
+-rw-r--r--   0        0        0     3030 2024-05-31 09:20:48.620634 testcontainers-4.5.1/modules/clickhouse/testcontainers/clickhouse/__init__.py
+-rw-r--r--   0        0        0     3886 2024-05-31 09:20:48.620634 testcontainers-4.5.1/modules/elasticsearch/testcontainers/elasticsearch/__init__.py
+-rw-r--r--   0        0        0      106 2024-05-31 09:20:48.620634 testcontainers-4.5.1/modules/google/testcontainers/google/__init__.py
+-rw-r--r--   0        0        0     2709 2024-05-31 09:20:48.620634 testcontainers-4.5.1/modules/google/testcontainers/google/datastore.py
+-rw-r--r--   0        0        0     2952 2024-05-31 09:20:48.620634 testcontainers-4.5.1/modules/google/testcontainers/google/pubsub.py
+-rw-r--r--   0        0        0     3760 2024-05-31 09:20:48.620634 testcontainers-4.5.1/modules/influxdb/testcontainers/influxdb.py
+-rw-r--r--   0        0        0     2387 2024-05-31 09:20:48.620634 testcontainers-4.5.1/modules/influxdb/testcontainers/influxdb1/__init__.py
+-rw-r--r--   0        0        0     4464 2024-05-31 09:20:48.620634 testcontainers-4.5.1/modules/influxdb/testcontainers/influxdb2/__init__.py
+-rw-r--r--   0        0        0     2902 2024-05-31 09:20:48.620634 testcontainers-4.5.1/modules/k3s/testcontainers/k3s/__init__.py
+-rw-r--r--   0        0        0     3592 2024-05-31 09:20:48.620634 testcontainers-4.5.1/modules/kafka/testcontainers/kafka/__init__.py
+-rw-r--r--   0        0        0     2727 2024-05-31 09:20:48.620634 testcontainers-4.5.1/modules/kafka/testcontainers/kafka/_redpanda.py
+-rw-r--r--   0        0        0     4223 2024-05-31 09:20:48.620634 testcontainers-4.5.1/modules/keycloak/testcontainers/keycloak/__init__.py
+-rw-r--r--   0        0        0     3222 2024-05-31 09:20:48.620634 testcontainers-4.5.1/modules/localstack/testcontainers/localstack/__init__.py
+-rw-r--r--   0        0        0     2042 2024-05-31 09:20:48.620634 testcontainers-4.5.1/modules/memcached/testcontainers/memcached/__init__.py
+-rw-r--r--   0        0        0     4116 2024-05-31 09:20:48.624634 testcontainers-4.5.1/modules/minio/testcontainers/minio/__init__.py
+-rw-r--r--   0        0        0     3017 2024-05-31 09:20:48.624634 testcontainers-4.5.1/modules/mongodb/testcontainers/mongodb/__init__.py
+-rw-r--r--   0        0        0     2202 2024-05-31 09:20:48.624634 testcontainers-4.5.1/modules/mssql/testcontainers/mssql/__init__.py
+-rw-r--r--   0        0        0     4984 2024-05-31 09:20:48.624634 testcontainers-4.5.1/modules/mysql/testcontainers/mysql/__init__.py
+-rw-r--r--   0        0        0     2811 2024-05-31 09:20:48.624634 testcontainers-4.5.1/modules/nats/testcontainers/nats/__init__.py
+-rw-r--r--   0        0        0     2782 2024-05-31 09:20:48.624634 testcontainers-4.5.1/modules/neo4j/testcontainers/neo4j/__init__.py
+-rw-r--r--   0        0        0     1596 2024-05-31 09:20:48.624634 testcontainers-4.5.1/modules/nginx/testcontainers/nginx/__init__.py
+-rw-r--r--   0        0        0     4109 2024-05-31 09:20:48.624634 testcontainers-4.5.1/modules/opensearch/testcontainers/opensearch/__init__.py
+-rw-r--r--   0        0        0     2960 2024-05-31 09:20:48.624634 testcontainers-4.5.1/modules/oracle-free/testcontainers/oracle/__init__.py
+-rw-r--r--   0        0        0     3984 2024-05-31 09:20:48.624634 testcontainers-4.5.1/modules/postgres/testcontainers/postgres/__init__.py
+-rw-r--r--   0        0        0     5209 2024-05-31 09:20:48.624634 testcontainers-4.5.1/modules/qdrant/testcontainers/qdrant/__init__.py
+-rw-r--r--   0        0        0     2967 2024-05-31 09:20:48.624634 testcontainers-4.5.1/modules/rabbitmq/testcontainers/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     3144 2024-05-31 09:20:48.624634 testcontainers-4.5.1/modules/redis/testcontainers/redis/__init__.py
+-rw-r--r--   0        0        0     2761 2024-05-31 09:20:48.628634 testcontainers-4.5.1/modules/registry/testcontainers/registry/__init__.py
+-rw-r--r--   0        0        0     4272 2024-05-31 09:20:48.628634 testcontainers-4.5.1/modules/selenium/testcontainers/selenium/__init__.py
+-rw-r--r--   0        0        0     1432 2024-05-31 09:20:48.628634 testcontainers-4.5.1/modules/selenium/testcontainers/selenium/video.py
+-rw-r--r--   0        0        0     2519 2024-05-31 09:20:48.628634 testcontainers-4.5.1/modules/vault/testcontainers/vault/__init__.py
+-rw-r--r--   0        0        0     5589 2024-05-31 09:20:48.628634 testcontainers-4.5.1/modules/weaviate/testcontainers/weaviate/__init__.py
+-rw-r--r--   0        0        0     8834 2024-05-31 09:20:48.628634 testcontainers-4.5.1/pyproject.toml
+-rw-r--r--   0        0        0     5554 1970-01-01 00:00:00.000000 testcontainers-4.5.1/PKG-INFO
```

### Comparing `testcontainers-4.5.0/LICENSE.txt` & `testcontainers-4.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/README.md` & `testcontainers-4.5.1/README.md`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/core/testcontainers/compose/compose.py` & `testcontainers-4.5.1/core/testcontainers/compose/compose.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/core/testcontainers/core/config.py` & `testcontainers-4.5.1/core/testcontainers/core/config.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/core/testcontainers/core/container.py` & `testcontainers-4.5.1/core/testcontainers/core/container.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/core/testcontainers/core/docker_client.py` & `testcontainers-4.5.1/core/testcontainers/core/docker_client.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/core/testcontainers/core/exceptions.py` & `testcontainers-4.5.1/core/testcontainers/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/core/testcontainers/core/generic.py` & `testcontainers-4.5.1/core/testcontainers/core/generic.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/core/testcontainers/core/labels.py` & `testcontainers-4.5.1/core/testcontainers/core/labels.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/core/testcontainers/core/network.py` & `testcontainers-4.5.1/core/testcontainers/core/network.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/core/testcontainers/core/utils.py` & `testcontainers-4.5.1/core/testcontainers/core/utils.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/core/testcontainers/core/waiting_utils.py` & `testcontainers-4.5.1/core/testcontainers/core/waiting_utils.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/arangodb/testcontainers/arangodb/__init__.py` & `testcontainers-4.5.1/modules/arangodb/testcontainers/arangodb/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/azurite/testcontainers/azurite/__init__.py` & `testcontainers-4.5.1/modules/azurite/testcontainers/azurite/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/cassandra/testcontainers/cassandra/__init__.py` & `testcontainers-4.5.1/modules/cassandra/testcontainers/cassandra/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/chroma/testcontainers/chroma/__init__.py` & `testcontainers-4.5.1/modules/chroma/testcontainers/chroma/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/clickhouse/testcontainers/clickhouse/__init__.py` & `testcontainers-4.5.1/modules/clickhouse/testcontainers/clickhouse/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/elasticsearch/testcontainers/elasticsearch/__init__.py` & `testcontainers-4.5.1/modules/elasticsearch/testcontainers/elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/google/testcontainers/google/datastore.py` & `testcontainers-4.5.1/modules/google/testcontainers/google/datastore.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/google/testcontainers/google/pubsub.py` & `testcontainers-4.5.1/modules/google/testcontainers/google/pubsub.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/influxdb/testcontainers/influxdb.py` & `testcontainers-4.5.1/modules/influxdb/testcontainers/influxdb.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/influxdb/testcontainers/influxdb1/__init__.py` & `testcontainers-4.5.1/modules/influxdb/testcontainers/influxdb1/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/influxdb/testcontainers/influxdb2/__init__.py` & `testcontainers-4.5.1/modules/influxdb/testcontainers/influxdb2/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/k3s/testcontainers/k3s/__init__.py` & `testcontainers-4.5.1/modules/k3s/testcontainers/k3s/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
+import logging
+
 from testcontainers.core.config import testcontainers_config
 from testcontainers.core.container import DockerContainer
 from testcontainers.core.waiting_utils import wait_for_logs
 
 
 class K3SContainer(DockerContainer):
     """
@@ -33,21 +35,24 @@
             ...     pod = client.CoreV1Api().list_pod_for_all_namespaces(limit=1)
             ...     assert len(pod.items) > 0, "Unable to get running nodes from k3s cluster"
     """
 
     KUBE_SECURE_PORT = 6443
     RANCHER_WEBHOOK_PORT = 8443
 
-    def __init__(self, image="rancher/k3s:latest", **kwargs) -> None:
+    def __init__(self, image="rancher/k3s:latest", enable_cgroup_mount=True, **kwargs) -> None:
         super().__init__(image, **kwargs)
         self.with_exposed_ports(self.KUBE_SECURE_PORT, self.RANCHER_WEBHOOK_PORT)
         self.with_env("K3S_URL", f"https://{self.get_container_host_ip()}:{self.KUBE_SECURE_PORT}")
         self.with_command("server --disable traefik --tls-san=" + self.get_container_host_ip())
         self.with_kwargs(privileged=True, tmpfs={"/run": "", "/var/run": ""})
-        self.with_volume_mapping("/sys/fs/cgroup", "/sys/fs/cgroup", "rw")
+        if enable_cgroup_mount:
+            self.with_volume_mapping("/sys/fs/cgroup", "/sys/fs/cgroup", "rw")
+        else:
+            logging.warning("'enable_cgroup_mount' is experimental, see testcontainers/testcontainers-python#591)")
 
     def _connect(self) -> None:
         wait_for_logs(self, predicate="Node controller sync successful", timeout=testcontainers_config.timeout)
 
     def start(self) -> "K3SContainer":
         super().start()
         self._connect()
```

### Comparing `testcontainers-4.5.0/modules/kafka/testcontainers/kafka/__init__.py` & `testcontainers-4.5.1/modules/kafka/testcontainers/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/kafka/testcontainers/kafka/_redpanda.py` & `testcontainers-4.5.1/modules/kafka/testcontainers/kafka/_redpanda.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/keycloak/testcontainers/keycloak/__init__.py` & `testcontainers-4.5.1/modules/keycloak/testcontainers/keycloak/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,14 @@
         # Keycloak provides REST API endpoints for health checks: https://www.keycloak.org/server/health
         response = requests.get(f"{self.get_url()}/health/ready", timeout=1)
         response.raise_for_status()
         if _DEFAULT_DEV_COMMAND in self._command:
             wait_for_logs(self, "Added user .* to realm .*")
 
     def start(self) -> "KeycloakContainer":
-        self._configure()
         super().start()
         self._readiness_probe()
         return self
 
     def with_realm_import_file(self, realm_import_file: str) -> "KeycloakContainer":
         file = os.path.abspath(realm_import_file)
         if not os.path.exists(file):
```

### Comparing `testcontainers-4.5.0/modules/localstack/testcontainers/localstack/__init__.py` & `testcontainers-4.5.1/modules/localstack/testcontainers/localstack/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/memcached/testcontainers/memcached/__init__.py` & `testcontainers-4.5.1/modules/memcached/testcontainers/memcached/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/minio/testcontainers/minio/__init__.py` & `testcontainers-4.5.1/modules/minio/testcontainers/minio/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/mongodb/testcontainers/mongodb/__init__.py` & `testcontainers-4.5.1/modules/mongodb/testcontainers/mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/mssql/testcontainers/mssql/__init__.py` & `testcontainers-4.5.1/modules/mssql/testcontainers/mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/mysql/testcontainers/mysql/__init__.py` & `testcontainers-4.5.1/modules/mysql/testcontainers/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/nats/testcontainers/nats/__init__.py` & `testcontainers-4.5.1/modules/nats/testcontainers/nats/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/neo4j/testcontainers/neo4j/__init__.py` & `testcontainers-4.5.1/modules/neo4j/testcontainers/neo4j/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/nginx/testcontainers/nginx/__init__.py` & `testcontainers-4.5.1/modules/nginx/testcontainers/nginx/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/opensearch/testcontainers/opensearch/__init__.py` & `testcontainers-4.5.1/modules/opensearch/testcontainers/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/oracle-free/testcontainers/oracle/__init__.py` & `testcontainers-4.5.1/modules/oracle-free/testcontainers/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/postgres/testcontainers/postgres/__init__.py` & `testcontainers-4.5.1/modules/postgres/testcontainers/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/qdrant/testcontainers/qdrant/__init__.py` & `testcontainers-4.5.1/modules/qdrant/testcontainers/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/rabbitmq/testcontainers/rabbitmq/__init__.py` & `testcontainers-4.5.1/modules/rabbitmq/testcontainers/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/redis/testcontainers/redis/__init__.py` & `testcontainers-4.5.1/modules/redis/testcontainers/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/registry/testcontainers/registry/__init__.py` & `testcontainers-4.5.1/modules/registry/testcontainers/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/selenium/testcontainers/selenium/__init__.py` & `testcontainers-4.5.1/modules/selenium/testcontainers/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/selenium/testcontainers/selenium/video.py` & `testcontainers-4.5.1/modules/selenium/testcontainers/selenium/video.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/vault/testcontainers/vault/__init__.py` & `testcontainers-4.5.1/modules/vault/testcontainers/vault/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/modules/weaviate/testcontainers/weaviate/__init__.py` & `testcontainers-4.5.1/modules/weaviate/testcontainers/weaviate/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.5.0/pyproject.toml` & `testcontainers-4.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "testcontainers"
-version = "4.5.0"  # auto-incremented by release-please
+version = "4.5.1"  # auto-incremented by release-please
 description = "Python library for throwaway instances of anything that can run in a Docker container"
 authors = ["Sergey Pirogov <automationremarks@gmail.com>"]
 maintainers = [
     "Balint Bartha <totallyzen@users.noreply.github.com>",
     "David Ankin <daveankin@gmail.com>",
     "Vemund Santi <vemund@santi.no>"
 ]
```

### Comparing `testcontainers-4.5.0/PKG-INFO` & `testcontainers-4.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testcontainers
-Version: 4.5.0
+Version: 4.5.1
 Summary: Python library for throwaway instances of anything that can run in a Docker container
 Keywords: testing,logging,docker,test automation
 Author: Sergey Pirogov
 Author-email: automationremarks@gmail.com
 Maintainer: Balint Bartha
 Maintainer-email: totallyzen@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
```

