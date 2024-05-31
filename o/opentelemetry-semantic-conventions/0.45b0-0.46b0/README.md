# Comparing `tmp/opentelemetry_semantic_conventions-0.45b0.tar.gz` & `tmp/opentelemetry_semantic_conventions-0.46b0.tar.gz`

## Comparing `opentelemetry_semantic_conventions-0.45b0.tar` & `opentelemetry_semantic_conventions-0.46b0.tar`

### file list

```diff
@@ -1,12 +1,83 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.45b0/src/opentelemetry/semconv/__init__.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.45b0/src/opentelemetry/semconv/version.py
--rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.45b0/src/opentelemetry/semconv/metrics/__init__.py
--rw-r--r--   0        0        0    31873 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.45b0/src/opentelemetry/semconv/resource/__init__.py
--rw-r--r--   0        0        0    68305 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.45b0/src/opentelemetry/semconv/trace/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.45b0/tests/__init__.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.45b0/tests/test_semconv.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.45b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.45b0/LICENSE
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.45b0/README.rst
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.45b0/pyproject.toml
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.45b0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/__init__.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/schemas.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/version.py
+-rw-r--r--   0        0        0    11256 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/aws_attributes.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/browser_attributes.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/client_attributes.py
+-rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/cloud_attributes.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/cloudevents_attributes.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/code_attributes.py
+-rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/container_attributes.py
+-rw-r--r--   0        0        0    10769 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/db_attributes.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/deployment_attributes.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/destination_attributes.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/device_attributes.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/disk_attributes.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/dns_attributes.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/enduser_attributes.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/error_attributes.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/event_attributes.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/exception_attributes.py
+-rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/faas_attributes.py
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/feature_flag_attributes.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/file_attributes.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/gcp_attributes.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/graphql_attributes.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/heroku_attributes.py
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/host_attributes.py
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/http_attributes.py
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/k8s_attributes.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/log_attributes.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/message_attributes.py
+-rw-r--r--   0        0        0    10761 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/messaging_attributes.py
+-rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/network_attributes.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/oci_attributes.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/opentracing_attributes.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/otel_attributes.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/other_attributes.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/peer_attributes.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/pool_attributes.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/process_attributes.py
+-rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/rpc_attributes.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/server_attributes.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/service_attributes.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/session_attributes.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/source_attributes.py
+-rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/system_attributes.py
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/telemetry_attributes.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/thread_attributes.py
+-rw-r--r--   0        0        0     6515 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/tls_attributes.py
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/url_attributes.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/user_agent_attributes.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/attributes/webengine_attributes.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/metrics/container_metrics.py
+-rw-r--r--   0        0        0     5522 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/metrics/db_metrics.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/metrics/dns_metrics.py
+-rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/metrics/faas_metrics.py
+-rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/metrics/http_metrics.py
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/metrics/messaging_metrics.py
+-rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/metrics/process_metrics.py
+-rw-r--r--   0        0        0     6194 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/metrics/rpc_metrics.py
+-rw-r--r--   0        0        0    13942 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/_incubating/metrics/system_metrics.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/attributes/client_attributes.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/attributes/error_attributes.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/attributes/exception_attributes.py
+-rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/attributes/http_attributes.py
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/attributes/network_attributes.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/attributes/otel_attributes.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/attributes/server_attributes.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/attributes/service_attributes.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/attributes/telemetry_attributes.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/attributes/url_attributes.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/attributes/user_agent_attributes.py
+-rw-r--r--   0        0        0     5790 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/metrics/__init__.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/metrics/http_metrics.py
+-rw-r--r--   0        0        0    32888 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/resource/__init__.py
+-rw-r--r--   0        0        0    69260 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/trace/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/tests/__init__.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/tests/test_semconv.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/LICENSE
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/README.rst
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/pyproject.toml
+-rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 opentelemetry_semantic_conventions-0.46b0/PKG-INFO
```

### Comparing `opentelemetry_semantic_conventions-0.45b0/src/opentelemetry/semconv/version.py` & `opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/version.py`

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

### Comparing `opentelemetry_semantic_conventions-0.45b0/src/opentelemetry/semconv/metrics/__init__.py` & `opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/metrics/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from deprecated import deprecated
 
+
+@deprecated(
+    "1.25.0",
+    reason="Use metrics defined in the :py:const:`opentelemetry.semconv.metrics` and :py:const:`opentelemetry.semconv._incubating.metrics` modules instead.",
+)
 class MetricInstruments:
     SCHEMA_URL = "https://opentelemetry.io/schemas/v1.21.0"
     """
     The URL of the OpenTelemetry schema for these keys and values.
     """
 
     HTTP_SERVER_DURATION = "http.server.duration"
```

### Comparing `opentelemetry_semantic_conventions-0.45b0/src/opentelemetry/semconv/resource/__init__.py` & `opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/resource/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,21 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # pylint: disable=too-many-lines
 
 from enum import Enum
 
+from deprecated import deprecated
 
+
+@deprecated(
+    "1.25.0",
+    reason="Use attributes defined in the :py:const:`opentelemetry.semconv.attributes` and :py:const:`opentelemetry.semconv._incubating.attributes` modules instead.",
+)
 class ResourceAttributes:
     SCHEMA_URL = "https://opentelemetry.io/schemas/v1.21.0"
     """
     The URL of the OpenTelemetry schema for these keys and values.
     """
     BROWSER_BRANDS = "browser.brands"
     """
@@ -646,14 +652,18 @@
 
     FAAS_ID = "faas.id"
     """
     Deprecated, use the `cloud.resource.id` attribute.
     """
 
 
+@deprecated(
+    "1.25.0",
+    reason="Use :py:const:`opentelemetry.semconv._incubating.attributes.CloudProviderValues` instead.",
+)
 class CloudProviderValues(Enum):
     ALIBABA_CLOUD = "alibaba_cloud"
     """Alibaba Cloud."""
 
     AWS = "aws"
     """Amazon Web Services."""
 
@@ -669,14 +679,18 @@
     IBM_CLOUD = "ibm_cloud"
     """IBM Cloud."""
 
     TENCENT_CLOUD = "tencent_cloud"
     """Tencent Cloud."""
 
 
+@deprecated(
+    "1.25.0",
+    reason="Use :py:const:`opentelemetry.semconv._incubating.attributes.CloudPlatformValues` instead.",
+)
 class CloudPlatformValues(Enum):
     ALIBABA_CLOUD_ECS = "alibaba_cloud_ecs"
     """Alibaba Cloud Elastic Compute Service."""
 
     ALIBABA_CLOUD_FC = "alibaba_cloud_fc"
     """Alibaba Cloud Function Compute."""
 
@@ -752,22 +766,30 @@
     TENCENT_CLOUD_EKS = "tencent_cloud_eks"
     """Tencent Cloud Elastic Kubernetes Service (EKS)."""
 
     TENCENT_CLOUD_SCF = "tencent_cloud_scf"
     """Tencent Cloud Serverless Cloud Function (SCF)."""
 
 
+@deprecated(
+    "1.25.0",
+    reason="Use :py:const:`opentelemetry.semconv._incubating.attributes.AwsEcsLaunchtypeValues` instead.",
+)
 class AwsEcsLaunchtypeValues(Enum):
     EC2 = "ec2"
     """ec2."""
 
     FARGATE = "fargate"
     """fargate."""
 
 
+@deprecated(
+    "1.25.0",
+    reason="Use :py:const:`opentelemetry.semconv._incubating.attributes.HostArchValues` instead.",
+)
 class HostArchValues(Enum):
     AMD64 = "amd64"
     """AMD64."""
 
     ARM32 = "arm32"
     """ARM32."""
 
@@ -786,14 +808,18 @@
     S390X = "s390x"
     """IBM z/Architecture."""
 
     X86 = "x86"
     """32-bit x86."""
 
 
+@deprecated(
+    "1.25.0",
+    reason="Use :py:const:`opentelemetry.semconv._incubating.attributes.OsTypeValues` instead.",
+)
 class OsTypeValues(Enum):
     WINDOWS = "windows"
     """Microsoft Windows."""
 
     LINUX = "linux"
     """Linux."""
 
@@ -821,14 +847,18 @@
     SOLARIS = "solaris"
     """SunOS, Oracle Solaris."""
 
     Z_OS = "z_os"
     """IBM z/OS."""
 
 
+@deprecated(
+    "1.25.0",
+    reason="Use :py:const:`opentelemetry.semconv.attributes.TelemetrySdkLanguageValues` instead.",
+)
 class TelemetrySdkLanguageValues(Enum):
     CPP = "cpp"
     """cpp."""
 
     DOTNET = "dotnet"
     """dotnet."""
```

### Comparing `opentelemetry_semantic_conventions-0.45b0/src/opentelemetry/semconv/trace/__init__.py` & `opentelemetry_semantic_conventions-0.46b0/src/opentelemetry/semconv/trace/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 # pylint: disable=too-many-lines
 
 from enum import Enum
 
 from deprecated import deprecated
 
 
+@deprecated(
+    "1.25.0",
+    reason="Use attributes defined in the :py:const:`opentelemetry.semconv.attributes` and :py:const:`opentelemetry.semconv._incubating.attributes` modules instead.",
+)
 class SpanAttributes:
     SCHEMA_URL = "https://opentelemetry.io/schemas/v1.21.0"
     """
     The URL of the OpenTelemetry schema for these keys and values.
     """
     CLIENT_ADDRESS = "client.address"
     """
@@ -1515,14 +1519,18 @@
     NRNSA = "nrnsa"
     """5G NRNSA (New Radio Non-Standalone)."""
 
     LTE_CA = "lte_ca"
     """LTE CA."""
 
 
+@deprecated(
+    "1.25.0",
+    reason="Use :py:const:`opentelemetry.semconv.attributes.NetworkTransportValues` instead.",
+)
 class NetTransportValues(Enum):
     IP_TCP = "ip_tcp"
     """ip_tcp."""
 
     IP_UDP = "ip_udp"
     """ip_udp."""
 
@@ -1532,25 +1540,33 @@
     INPROC = "inproc"
     """In-process communication."""
 
     OTHER = "other"
     """Something else (non IP-based)."""
 
 
+@deprecated(
+    "1.25.0",
+    reason="Use :py:const:`opentelemetry.semconv.attributes.NetworkType` instead.",
+)
 class NetSockFamilyValues(Enum):
     INET = "inet"
     """IPv4 address."""
 
     INET6 = "inet6"
     """IPv6 address."""
 
     UNIX = "unix"
     """Unix domain socket path."""
 
 
+@deprecated(
+    "1.25.0",
+    reason="Use :py:const:`opentelemetry.semconv.attributes.HttpRequestMethodValues` instead.",
+)
 class HttpRequestMethodValues(Enum):
     CONNECT = "CONNECT"
     """CONNECT method."""
 
     DELETE = "DELETE"
     """DELETE method."""
 
@@ -1575,41 +1591,51 @@
     TRACE = "TRACE"
     """TRACE method."""
 
     OTHER = "_OTHER"
     """Any HTTP method that the instrumentation has no prior knowledge of."""
 
 
+@deprecated("1.25.0", reason="Removed from the specification.")
 class EventDomainValues(Enum):
     BROWSER = "browser"
     """Events from browser apps."""
 
     DEVICE = "device"
     """Events from mobile apps."""
 
     K8S = "k8s"
     """Events from Kubernetes."""
 
 
+@deprecated(
+    "1.25.0",
+    reason="Use :py:const:`opentelemetry.semconv._incubating.attributes.LogIostreamValues` instead.",
+)
 class LogIostreamValues(Enum):
     STDOUT = "stdout"
     """Logs from stdout stream."""
 
     STDERR = "stderr"
     """Events from stderr stream."""
 
 
+@deprecated("1.25.0", reason="Removed from the specification.")
 class TypeValues(Enum):
     HEAP = "heap"
     """Heap memory."""
 
     NON_HEAP = "non_heap"
     """Non-heap memory."""
 
 
+@deprecated(
+    "1.25.0",
+    reason="Use :py:const:`opentelemetry.semconv._incubating.attributes.OpentracingRefTypeValues` instead.",
+)
 class OpentracingRefTypeValues(Enum):
     CHILD_OF = "child_of"
     """The parent Span depends on the child Span in some capacity."""
 
     FOLLOWS_FROM = "follows_from"
     """The parent Span does not depend in any way on the result of the child Span."""
```

### Comparing `opentelemetry_semantic_conventions-0.45b0/tests/test_semconv.py` & `opentelemetry_semantic_conventions-0.46b0/tests/test_semconv.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_semantic_conventions-0.45b0/.gitignore` & `opentelemetry_semantic_conventions-0.46b0/.gitignore`

 * *Files identical despite different names*

### Comparing `opentelemetry_semantic_conventions-0.45b0/LICENSE` & `opentelemetry_semantic_conventions-0.46b0/LICENSE`

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

### Comparing `opentelemetry_semantic_conventions-0.45b0/README.rst` & `opentelemetry_semantic_conventions-0.46b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_semantic_conventions-0.45b0/pyproject.toml` & `opentelemetry_semantic_conventions-0.46b0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -10,24 +10,29 @@
 license = {text = "Apache-2.0"}
 requires-python = ">=3.8"
 authors = [
   { name = "OpenTelemetry Authors", email = "cncf-opentelemetry-contributors@lists.cncf.io" },
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
+  "Framework :: OpenTelemetry",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 
+dependencies = [
+  "opentelemetry-api == 1.25.0",
+]
+
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python/tree/main/opentelemetry-semantic-conventions"
 
 [tool.hatch.version]
 path = "src/opentelemetry/semconv/version.py"
 
 [tool.hatch.build.targets.sdist]
```

### Comparing `opentelemetry_semantic_conventions-0.45b0/PKG-INFO` & `opentelemetry_semantic_conventions-0.46b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.3
 Name: opentelemetry-semantic-conventions
-Version: 0.45b0
+Version: 0.46b0
 Summary: OpenTelemetry Semantic Conventions
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python/tree/main/opentelemetry-semantic-conventions
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: OpenTelemetry
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Requires-Dist: opentelemetry-api==1.25.0
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Semantic Conventions
 ==================================
 
 |pypi|
```

