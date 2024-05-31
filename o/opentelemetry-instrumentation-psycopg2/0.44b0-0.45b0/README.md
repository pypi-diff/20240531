# Comparing `tmp/opentelemetry_instrumentation_psycopg2-0.44b0.tar.gz` & `tmp/opentelemetry_instrumentation_psycopg2-0.45b0.tar.gz`

## Comparing `opentelemetry_instrumentation_psycopg2-0.44b0.tar` & `opentelemetry_instrumentation_psycopg2-0.45b0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     8374 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_psycopg2-0.44b0/src/opentelemetry/instrumentation/psycopg2/__init__.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_psycopg2-0.44b0/src/opentelemetry/instrumentation/psycopg2/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_psycopg2-0.44b0/src/opentelemetry/instrumentation/psycopg2/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_psycopg2-0.44b0/tests/__init__.py
--rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_psycopg2-0.44b0/tests/test_psycopg2_integration.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_psycopg2-0.44b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_psycopg2-0.44b0/LICENSE
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_psycopg2-0.44b0/README.rst
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_psycopg2-0.44b0/pyproject.toml
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_psycopg2-0.44b0/PKG-INFO
+-rw-r--r--   0        0        0     8374 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_psycopg2-0.45b0/src/opentelemetry/instrumentation/psycopg2/__init__.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_psycopg2-0.45b0/src/opentelemetry/instrumentation/psycopg2/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_psycopg2-0.45b0/src/opentelemetry/instrumentation/psycopg2/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_psycopg2-0.45b0/tests/__init__.py
+-rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_psycopg2-0.45b0/tests/test_psycopg2_integration.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_psycopg2-0.45b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_psycopg2-0.45b0/LICENSE
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_psycopg2-0.45b0/README.rst
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_psycopg2-0.45b0/pyproject.toml
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_psycopg2-0.45b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_psycopg2-0.44b0/src/opentelemetry/instrumentation/psycopg2/__init__.py` & `opentelemetry_instrumentation_psycopg2-0.45b0/src/opentelemetry/instrumentation/psycopg2/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_psycopg2-0.44b0/src/opentelemetry/instrumentation/psycopg2/package.py` & `opentelemetry_instrumentation_psycopg2-0.45b0/src/opentelemetry/instrumentation/psycopg2/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_psycopg2-0.44b0/src/opentelemetry/instrumentation/psycopg2/version.py` & `opentelemetry_instrumentation_psycopg2-0.45b0/src/opentelemetry/instrumentation/psycopg2/version.py`

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

### Comparing `opentelemetry_instrumentation_psycopg2-0.44b0/tests/test_psycopg2_integration.py` & `opentelemetry_instrumentation_psycopg2-0.45b0/tests/test_psycopg2_integration.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_psycopg2-0.44b0/LICENSE` & `opentelemetry_instrumentation_psycopg2-0.45b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_psycopg2-0.44b0/README.rst` & `opentelemetry_instrumentation_psycopg2-0.45b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_psycopg2-0.44b0/pyproject.toml` & `opentelemetry_instrumentation_psycopg2-0.45b0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,46 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "opentelemetry-instrumentation-psycopg2"
-dynamic = ["version"]
-description = "OpenTelemetry psycopg2 instrumentation"
-readme = "README.rst"
-license = "Apache-2.0"
-requires-python = ">=3.8"
-authors = [
-  { name = "OpenTelemetry Authors", email = "cncf-opentelemetry-contributors@lists.cncf.io" },
-]
-classifiers = [
-  "Development Status :: 4 - Beta",
-  "Intended Audience :: Developers",
-  "License :: OSI Approved :: Apache Software License",
-  "Programming Language :: Python",
-  "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
-  "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
-]
-dependencies = [
-  "opentelemetry-api ~= 1.12",
-  "opentelemetry-instrumentation == 0.44b0",
-  "opentelemetry-instrumentation-dbapi == 0.44b0",
-]
-
-[project.optional-dependencies]
-instruments = [
-  "psycopg2 >= 2.7.3.1",
-]
-test = [
-  "opentelemetry-instrumentation-psycopg2[instruments]",
-  "opentelemetry-test-utils == 0.44b0",
-]
-
-[project.entry-points.opentelemetry_instrumentor]
-psycopg2 = "opentelemetry.instrumentation.psycopg2:Psycopg2Instrumentor"
-
-[project.urls]
-Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-psycopg2"
-
-[tool.hatch.version]
-path = "src/opentelemetry/instrumentation/psycopg2/version.py"
-
-[tool.hatch.build.targets.sdist]
-include = [
-  "/src",
-  "/tests",
-]
-
-[tool.hatch.build.targets.wheel]
-packages = ["src/opentelemetry"]
+Metadata-Version: 2.3
+Name: opentelemetry-instrumentation-psycopg2
+Version: 0.45b0
+Summary: OpenTelemetry psycopg2 instrumentation
+Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-psycopg2
+Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
+License-Expression: Apache-2.0
+License-File: LICENSE
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Requires-Dist: opentelemetry-api~=1.12
+Requires-Dist: opentelemetry-instrumentation-dbapi==0.45b0
+Requires-Dist: opentelemetry-instrumentation==0.45b0
+Provides-Extra: instruments
+Requires-Dist: psycopg2>=2.7.3.1; extra == 'instruments'
+Description-Content-Type: text/x-rst
+
+OpenTelemetry Psycopg Instrumentation
+=====================================
+
+|pypi|
+
+.. |pypi| image:: https://badge.fury.io/py/opentelemetry-instrumentation-psycopg2.svg
+   :target: https://pypi.org/project/opentelemetry-instrumentation-psycopg2/
+
+Installation
+------------
+
+::
+
+    pip install opentelemetry-instrumentation-psycopg2
+
+
+References
+----------
+* `OpenTelemetry Psycopg Instrumentation <https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/psycopg2/psycopg2.html>`_
+* `OpenTelemetry Project <https://opentelemetry.io/>`_
+* `OpenTelemetry Python Examples <https://github.com/open-telemetry/opentelemetry-python/tree/main/docs/examples>`_
```

