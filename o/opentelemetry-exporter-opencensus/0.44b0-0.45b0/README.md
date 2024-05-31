# Comparing `tmp/opentelemetry_exporter_opencensus-0.44b0.tar.gz` & `tmp/opentelemetry_exporter_opencensus-0.45b0.tar.gz`

## Comparing `opentelemetry_exporter_opencensus-0.44b0.tar` & `opentelemetry_exporter_opencensus-0.45b0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 opentelemetry_exporter_opencensus-0.44b0/src/opentelemetry/exporter/opencensus/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_exporter_opencensus-0.44b0/src/opentelemetry/exporter/opencensus/py.typed
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 opentelemetry_exporter_opencensus-0.44b0/src/opentelemetry/exporter/opencensus/util.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_exporter_opencensus-0.44b0/src/opentelemetry/exporter/opencensus/version.py
--rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 opentelemetry_exporter_opencensus-0.44b0/src/opentelemetry/exporter/opencensus/trace_exporter/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_exporter_opencensus-0.44b0/tests/__init__.py
--rw-r--r--   0        0        0    13238 2020-02-02 00:00:00.000000 opentelemetry_exporter_opencensus-0.44b0/tests/test_otcollector_trace_exporter.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 opentelemetry_exporter_opencensus-0.44b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_exporter_opencensus-0.44b0/LICENSE
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 opentelemetry_exporter_opencensus-0.44b0/README.rst
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 opentelemetry_exporter_opencensus-0.44b0/pyproject.toml
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 opentelemetry_exporter_opencensus-0.44b0/PKG-INFO
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 opentelemetry_exporter_opencensus-0.45b0/src/opentelemetry/exporter/opencensus/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_exporter_opencensus-0.45b0/src/opentelemetry/exporter/opencensus/py.typed
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 opentelemetry_exporter_opencensus-0.45b0/src/opentelemetry/exporter/opencensus/util.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_exporter_opencensus-0.45b0/src/opentelemetry/exporter/opencensus/version.py
+-rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 opentelemetry_exporter_opencensus-0.45b0/src/opentelemetry/exporter/opencensus/trace_exporter/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_exporter_opencensus-0.45b0/tests/__init__.py
+-rw-r--r--   0        0        0    13238 2020-02-02 00:00:00.000000 opentelemetry_exporter_opencensus-0.45b0/tests/test_otcollector_trace_exporter.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 opentelemetry_exporter_opencensus-0.45b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_exporter_opencensus-0.45b0/LICENSE
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 opentelemetry_exporter_opencensus-0.45b0/README.rst
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 opentelemetry_exporter_opencensus-0.45b0/pyproject.toml
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 opentelemetry_exporter_opencensus-0.45b0/PKG-INFO
```

### Comparing `opentelemetry_exporter_opencensus-0.44b0/src/opentelemetry/exporter/opencensus/__init__.py` & `opentelemetry_exporter_opencensus-0.45b0/src/opentelemetry/exporter/opencensus/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_opencensus-0.44b0/src/opentelemetry/exporter/opencensus/util.py` & `opentelemetry_exporter_opencensus-0.45b0/src/opentelemetry/exporter/opencensus/util.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_opencensus-0.44b0/src/opentelemetry/exporter/opencensus/version.py` & `opentelemetry_exporter_opencensus-0.45b0/src/opentelemetry/exporter/opencensus/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.44b0"
+__version__ = "0.45b0"
```

### Comparing `opentelemetry_exporter_opencensus-0.44b0/src/opentelemetry/exporter/opencensus/trace_exporter/__init__.py` & `opentelemetry_exporter_opencensus-0.45b0/src/opentelemetry/exporter/opencensus/trace_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_opencensus-0.44b0/tests/test_otcollector_trace_exporter.py` & `opentelemetry_exporter_opencensus-0.45b0/tests/test_otcollector_trace_exporter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_opencensus-0.44b0/.gitignore` & `opentelemetry_exporter_opencensus-0.45b0/.gitignore`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_opencensus-0.44b0/LICENSE` & `opentelemetry_exporter_opencensus-0.45b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_opencensus-0.44b0/README.rst` & `opentelemetry_exporter_opencensus-0.45b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_exporter_opencensus-0.44b0/pyproject.toml` & `opentelemetry_exporter_opencensus-0.45b0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "opentelemetry-exporter-opencensus"
 dynamic = ["version"]
 description = "OpenCensus Exporter"
 readme = "README.rst"
-license = "Apache-2.0"
+license = {text = "Apache-2.0"}
 requires-python = ">=3.8"
 authors = [
   { name = "OpenTelemetry Authors", email = "cncf-opentelemetry-contributors@lists.cncf.io" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
@@ -23,23 +23,20 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Typing :: Typed",
 ]
 dependencies = [
   "grpcio >= 1.0.0, < 2.0.0",
   "opencensus-proto >= 0.1.0, < 1.0.0",
-  "opentelemetry-api >= 1.23.0",
+  "opentelemetry-api >= 1.24.0",
   "opentelemetry-sdk >= 1.15",
   "protobuf ~= 3.13",
   "setuptools >= 16.0",
 ]
 
-[project.optional-dependencies]
-test = []
-
 [project.entry-points.opentelemetry_traces_exporter]
 opencensus = "opentelemetry.exporter.opencensus.trace_exporter:OpenCensusSpanExporter"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python/tree/main/exporter/opentelemetry-exporter-opencensus"
 
 [tool.hatch.version]
```

### Comparing `opentelemetry_exporter_opencensus-0.44b0/PKG-INFO` & `opentelemetry_exporter_opencensus-0.45b0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: opentelemetry-exporter-opencensus
-Version: 0.44b0
+Version: 0.45b0
 Summary: OpenCensus Exporter
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python/tree/main/exporter/opentelemetry-exporter-opencensus
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
-License-Expression: Apache-2.0
+License: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: grpcio<2.0.0,>=1.0.0
 Requires-Dist: opencensus-proto<1.0.0,>=0.1.0
-Requires-Dist: opentelemetry-api>=1.23.0
+Requires-Dist: opentelemetry-api>=1.24.0
 Requires-Dist: opentelemetry-sdk>=1.15
 Requires-Dist: protobuf~=3.13
 Requires-Dist: setuptools>=16.0
-Provides-Extra: test
 Description-Content-Type: text/x-rst
 
 OpenCensus Exporter
 ===================
 
 |pypi|
```

