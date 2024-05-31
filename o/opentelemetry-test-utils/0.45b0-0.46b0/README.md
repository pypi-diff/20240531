# Comparing `tmp/opentelemetry_test_utils-0.45b0.tar.gz` & `tmp/opentelemetry_test_utils-0.46b0.tar.gz`

## Comparing `opentelemetry_test_utils-0.45b0.tar` & `opentelemetry_test_utils-0.46b0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.45b0/src/opentelemetry/test/__init__.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.45b0/src/opentelemetry/test/asgitestutil.py
--rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.45b0/src/opentelemetry/test/concurrency_test.py
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.45b0/src/opentelemetry/test/globals_test.py
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.45b0/src/opentelemetry/test/httptest.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.45b0/src/opentelemetry/test/metrictestutil.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.45b0/src/opentelemetry/test/mock_textmap.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.45b0/src/opentelemetry/test/spantestutil.py
--rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.45b0/src/opentelemetry/test/test_base.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.45b0/src/opentelemetry/test/version.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.45b0/src/opentelemetry/test/wsgitestutil.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.45b0/.gitignore
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.45b0/README.rst
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.45b0/pyproject.toml
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.45b0/PKG-INFO
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.46b0/src/opentelemetry/test/__init__.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.46b0/src/opentelemetry/test/asgitestutil.py
+-rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.46b0/src/opentelemetry/test/concurrency_test.py
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.46b0/src/opentelemetry/test/globals_test.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.46b0/src/opentelemetry/test/httptest.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.46b0/src/opentelemetry/test/metrictestutil.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.46b0/src/opentelemetry/test/mock_textmap.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.46b0/src/opentelemetry/test/spantestutil.py
+-rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.46b0/src/opentelemetry/test/test_base.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.46b0/src/opentelemetry/test/version.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.46b0/src/opentelemetry/test/wsgitestutil.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.46b0/.gitignore
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.46b0/README.rst
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.46b0/pyproject.toml
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 opentelemetry_test_utils-0.46b0/PKG-INFO
```

### Comparing `opentelemetry_test_utils-0.45b0/src/opentelemetry/test/__init__.py` & `opentelemetry_test_utils-0.46b0/src/opentelemetry/test/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_test_utils-0.45b0/src/opentelemetry/test/asgitestutil.py` & `opentelemetry_test_utils-0.46b0/src/opentelemetry/test/asgitestutil.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_test_utils-0.45b0/src/opentelemetry/test/concurrency_test.py` & `opentelemetry_test_utils-0.46b0/src/opentelemetry/test/concurrency_test.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_test_utils-0.45b0/src/opentelemetry/test/globals_test.py` & `opentelemetry_test_utils-0.46b0/src/opentelemetry/test/globals_test.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_test_utils-0.45b0/src/opentelemetry/test/httptest.py` & `opentelemetry_test_utils-0.46b0/src/opentelemetry/test/httptest.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_test_utils-0.45b0/src/opentelemetry/test/metrictestutil.py` & `opentelemetry_test_utils-0.46b0/src/opentelemetry/test/metrictestutil.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,22 +9,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+from typing import Optional
+
 from opentelemetry.attributes import BoundedAttributes
 from opentelemetry.sdk.metrics.export import (
     AggregationTemporality,
     Gauge,
+    Histogram,
+    HistogramDataPoint,
     Metric,
     NumberDataPoint,
     Sum,
 )
+from opentelemetry.util.types import Attributes
 
 
 def _generate_metric(
     name, data, attributes=None, description=None, unit=None
 ) -> Metric:
     if description is None:
         description = "foo"
@@ -94,7 +99,38 @@
 ) -> Metric:
     return _generate_metric(
         name,
         None,
         description=description,
         unit=unit,
     )
+
+
+def _generate_histogram(
+    name: str,
+    attributes: Attributes = None,
+    description: Optional[str] = None,
+    unit: Optional[str] = None,
+) -> Metric:
+    if attributes is None:
+        attributes = BoundedAttributes(attributes={"a": 1, "b": True})
+    return _generate_metric(
+        name,
+        Histogram(
+            data_points=[
+                HistogramDataPoint(
+                    attributes=attributes,
+                    start_time_unix_nano=1641946016139533244,
+                    time_unix_nano=1641946016139533244,
+                    count=6,
+                    sum=579.0,
+                    bucket_counts=[1, 3, 2],
+                    explicit_bounds=[123.0, 456.0],
+                    min=1,
+                    max=457,
+                )
+            ],
+            aggregation_temporality=AggregationTemporality.CUMULATIVE,
+        ),
+        description=description,
+        unit=unit,
+    )
```

### Comparing `opentelemetry_test_utils-0.45b0/src/opentelemetry/test/mock_textmap.py` & `opentelemetry_test_utils-0.46b0/src/opentelemetry/test/mock_textmap.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_test_utils-0.45b0/src/opentelemetry/test/spantestutil.py` & `opentelemetry_test_utils-0.46b0/src/opentelemetry/test/spantestutil.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_test_utils-0.45b0/src/opentelemetry/test/test_base.py` & `opentelemetry_test_utils-0.46b0/src/opentelemetry/test/test_base.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_test_utils-0.45b0/src/opentelemetry/test/wsgitestutil.py` & `opentelemetry_test_utils-0.46b0/src/opentelemetry/test/wsgitestutil.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_test_utils-0.45b0/.gitignore` & `opentelemetry_test_utils-0.46b0/.gitignore`

 * *Files identical despite different names*

### Comparing `opentelemetry_test_utils-0.45b0/pyproject.toml` & `opentelemetry_test_utils-0.46b0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -10,26 +10,27 @@
 license = {text = "Apache-2.0"}
 requires-python = ">=3.8"
 authors = [
   { name = "OpenTelemetry Authors", email = "cncf-opentelemetry-contributors@lists.cncf.io" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
+  "Framework :: OpenTelemetry",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
   "asgiref ~= 3.0",
-  "opentelemetry-api == 1.24.0",
-  "opentelemetry-sdk == 1.24.0",
+  "opentelemetry-api == 1.25.0",
+  "opentelemetry-sdk == 1.25.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python/tests/opentelemetry-test-utils"
 
 [tool.hatch.version]
 path = "src/opentelemetry/test/version.py"
```

### Comparing `opentelemetry_test_utils-0.45b0/PKG-INFO` & `opentelemetry_test_utils-0.46b0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.3
 Name: opentelemetry-test-utils
-Version: 0.45b0
+Version: 0.46b0
 Summary: Test utilities for OpenTelemetry unit tests
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python/tests/opentelemetry-test-utils
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: OpenTelemetry
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Requires-Dist: asgiref~=3.0
-Requires-Dist: opentelemetry-api==1.24.0
-Requires-Dist: opentelemetry-sdk==1.24.0
+Requires-Dist: opentelemetry-api==1.25.0
+Requires-Dist: opentelemetry-sdk==1.25.0
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Test Utilities
 ============================
 
 This package provides internal testing utilities for the OpenTelemetry Python project and provides no stability or quality guarantees.
 Please do not use it for anything other than writing or running tests for the OpenTelemetry Python project (github.com/open-telemetry/opentelemetry-python).
```

