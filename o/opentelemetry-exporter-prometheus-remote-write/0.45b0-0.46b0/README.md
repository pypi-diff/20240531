# Comparing `tmp/opentelemetry_exporter_prometheus_remote_write-0.45b0.tar.gz` & `tmp/opentelemetry_exporter_prometheus_remote_write-0.46b0.tar.gz`

## Comparing `opentelemetry_exporter_prometheus_remote_write-0.45b0.tar` & `opentelemetry_exporter_prometheus_remote_write-0.46b0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    14850 2020-02-02 00:00:00.000000 opentelemetry_exporter_prometheus_remote_write-0.45b0/src/opentelemetry/exporter/prometheus_remote_write/__init__.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_exporter_prometheus_remote_write-0.45b0/src/opentelemetry/exporter/prometheus_remote_write/version.py
--rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 opentelemetry_exporter_prometheus_remote_write-0.45b0/src/opentelemetry/exporter/prometheus_remote_write/gen/remote_pb2.py
--rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 opentelemetry_exporter_prometheus_remote_write-0.45b0/src/opentelemetry/exporter/prometheus_remote_write/gen/types_pb2.py
--rw-r--r--   0        0        0    15743 2020-02-02 00:00:00.000000 opentelemetry_exporter_prometheus_remote_write-0.45b0/src/opentelemetry/exporter/prometheus_remote_write/gen/gogoproto/gogo_pb2.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 opentelemetry_exporter_prometheus_remote_write-0.45b0/tests/__init__.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 opentelemetry_exporter_prometheus_remote_write-0.45b0/tests/conftest.py
--rw-r--r--   0        0        0    10764 2020-02-02 00:00:00.000000 opentelemetry_exporter_prometheus_remote_write-0.45b0/tests/test_prometheus_remote_write_exporter.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_exporter_prometheus_remote_write-0.45b0/.gitignore
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 opentelemetry_exporter_prometheus_remote_write-0.45b0/README.rst
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 opentelemetry_exporter_prometheus_remote_write-0.45b0/pyproject.toml
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 opentelemetry_exporter_prometheus_remote_write-0.45b0/PKG-INFO
+-rw-r--r--   0        0        0    14850 2020-02-02 00:00:00.000000 opentelemetry_exporter_prometheus_remote_write-0.46b0/src/opentelemetry/exporter/prometheus_remote_write/__init__.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_exporter_prometheus_remote_write-0.46b0/src/opentelemetry/exporter/prometheus_remote_write/version.py
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 opentelemetry_exporter_prometheus_remote_write-0.46b0/src/opentelemetry/exporter/prometheus_remote_write/gen/remote_pb2.py
+-rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 opentelemetry_exporter_prometheus_remote_write-0.46b0/src/opentelemetry/exporter/prometheus_remote_write/gen/types_pb2.py
+-rw-r--r--   0        0        0    15743 2020-02-02 00:00:00.000000 opentelemetry_exporter_prometheus_remote_write-0.46b0/src/opentelemetry/exporter/prometheus_remote_write/gen/gogoproto/gogo_pb2.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 opentelemetry_exporter_prometheus_remote_write-0.46b0/tests/__init__.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 opentelemetry_exporter_prometheus_remote_write-0.46b0/tests/conftest.py
+-rw-r--r--   0        0        0    10764 2020-02-02 00:00:00.000000 opentelemetry_exporter_prometheus_remote_write-0.46b0/tests/test_prometheus_remote_write_exporter.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_exporter_prometheus_remote_write-0.46b0/.gitignore
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 opentelemetry_exporter_prometheus_remote_write-0.46b0/README.rst
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 opentelemetry_exporter_prometheus_remote_write-0.46b0/pyproject.toml
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 opentelemetry_exporter_prometheus_remote_write-0.46b0/PKG-INFO
```

### Comparing `opentelemetry_exporter_prometheus_remote_write-0.45b0/src/opentelemetry/exporter/prometheus_remote_write/__init__.py` & `opentelemetry_exporter_prometheus_remote_write-0.46b0/src/opentelemetry/exporter/prometheus_remote_write/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_prometheus_remote_write-0.45b0/src/opentelemetry/exporter/prometheus_remote_write/version.py` & `opentelemetry_exporter_prometheus_remote_write-0.46b0/src/opentelemetry/exporter/prometheus_remote_write/version.py`

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

### Comparing `opentelemetry_exporter_prometheus_remote_write-0.45b0/src/opentelemetry/exporter/prometheus_remote_write/gen/remote_pb2.py` & `opentelemetry_exporter_prometheus_remote_write-0.46b0/src/opentelemetry/exporter/prometheus_remote_write/gen/remote_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,21 +30,21 @@
     "opentelemetry.exporter.prometheus_remote_write.gen.remote_pb2",
     globals(),
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z\006prompb"
     _WRITEREQUEST.fields_by_name["timeseries"]._options = None
-    _WRITEREQUEST.fields_by_name[
-        "timeseries"
-    ]._serialized_options = b"\310\336\037\000"
+    _WRITEREQUEST.fields_by_name["timeseries"]._serialized_options = (
+        b"\310\336\037\000"
+    )
     _WRITEREQUEST.fields_by_name["metadata"]._options = None
-    _WRITEREQUEST.fields_by_name[
-        "metadata"
-    ]._serialized_options = b"\310\336\037\000"
+    _WRITEREQUEST.fields_by_name["metadata"]._serialized_options = (
+        b"\310\336\037\000"
+    )
     _WRITEREQUEST._serialized_start = 216
     _WRITEREQUEST._serialized_end = 338
     _READREQUEST._serialized_start = 341
     _READREQUEST._serialized_end = 515
     _READREQUEST_RESPONSETYPE._serialized_start = 463
     _READREQUEST_RESPONSETYPE._serialized_end = 515
     _READRESPONSE._serialized_start = 517
```

### Comparing `opentelemetry_exporter_prometheus_remote_write-0.45b0/src/opentelemetry/exporter/prometheus_remote_write/gen/types_pb2.py` & `opentelemetry_exporter_prometheus_remote_write-0.46b0/src/opentelemetry/exporter/prometheus_remote_write/gen/types_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,39 +27,39 @@
     "opentelemetry.exporter.prometheus_remote_write.gen.types_pb2",
     globals(),
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z\006prompb"
     _EXEMPLAR.fields_by_name["labels"]._options = None
-    _EXEMPLAR.fields_by_name[
-        "labels"
-    ]._serialized_options = b"\310\336\037\000"
+    _EXEMPLAR.fields_by_name["labels"]._serialized_options = (
+        b"\310\336\037\000"
+    )
     _TIMESERIES.fields_by_name["labels"]._options = None
-    _TIMESERIES.fields_by_name[
-        "labels"
-    ]._serialized_options = b"\310\336\037\000"
+    _TIMESERIES.fields_by_name["labels"]._serialized_options = (
+        b"\310\336\037\000"
+    )
     _TIMESERIES.fields_by_name["samples"]._options = None
-    _TIMESERIES.fields_by_name[
-        "samples"
-    ]._serialized_options = b"\310\336\037\000"
+    _TIMESERIES.fields_by_name["samples"]._serialized_options = (
+        b"\310\336\037\000"
+    )
     _TIMESERIES.fields_by_name["exemplars"]._options = None
-    _TIMESERIES.fields_by_name[
-        "exemplars"
-    ]._serialized_options = b"\310\336\037\000"
+    _TIMESERIES.fields_by_name["exemplars"]._serialized_options = (
+        b"\310\336\037\000"
+    )
     _LABELS.fields_by_name["labels"]._options = None
     _LABELS.fields_by_name["labels"]._serialized_options = b"\310\336\037\000"
     _CHUNKEDSERIES.fields_by_name["labels"]._options = None
-    _CHUNKEDSERIES.fields_by_name[
-        "labels"
-    ]._serialized_options = b"\310\336\037\000"
+    _CHUNKEDSERIES.fields_by_name["labels"]._serialized_options = (
+        b"\310\336\037\000"
+    )
     _CHUNKEDSERIES.fields_by_name["chunks"]._options = None
-    _CHUNKEDSERIES.fields_by_name[
-        "chunks"
-    ]._serialized_options = b"\310\336\037\000"
+    _CHUNKEDSERIES.fields_by_name["chunks"]._serialized_options = (
+        b"\310\336\037\000"
+    )
     _METRICMETADATA._serialized_start = 152
     _METRICMETADATA._serialized_end = 400
     _METRICMETADATA_METRICTYPE._serialized_start = 279
     _METRICMETADATA_METRICTYPE._serialized_end = 400
     _SAMPLE._serialized_start = 402
     _SAMPLE._serialized_end = 444
     _EXEMPLAR._serialized_start = 446
```

### Comparing `opentelemetry_exporter_prometheus_remote_write-0.45b0/src/opentelemetry/exporter/prometheus_remote_write/gen/gogoproto/gogo_pb2.py` & `opentelemetry_exporter_prometheus_remote_write-0.46b0/src/opentelemetry/exporter/prometheus_remote_write/gen/gogoproto/gogo_pb2.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_prometheus_remote_write-0.45b0/tests/__init__.py` & `opentelemetry_exporter_prometheus_remote_write-0.46b0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_prometheus_remote_write-0.45b0/tests/conftest.py` & `opentelemetry_exporter_prometheus_remote_write-0.46b0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_prometheus_remote_write-0.45b0/tests/test_prometheus_remote_write_exporter.py` & `opentelemetry_exporter_prometheus_remote_write-0.46b0/tests/test_prometheus_remote_write_exporter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_prometheus_remote_write-0.45b0/README.rst` & `opentelemetry_exporter_prometheus_remote_write-0.46b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_prometheus_remote_write-0.45b0/pyproject.toml` & `opentelemetry_exporter_prometheus_remote_write-0.46b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_prometheus_remote_write-0.45b0/PKG-INFO` & `opentelemetry_exporter_prometheus_remote_write-0.46b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: opentelemetry-exporter-prometheus-remote-write
-Version: 0.45b0
+Version: 0.46b0
 Summary: Prometheus Remote Write Metrics Exporter for OpenTelemetry
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/exporter/opentelemetry-exporter-prometheus-remote-write
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

