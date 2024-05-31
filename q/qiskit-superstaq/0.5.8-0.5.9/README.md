# Comparing `tmp/qiskit-superstaq-0.5.8.tar.gz` & `tmp/qiskit-superstaq-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-superstaq-0.5.8.tar", last modified: Tue Jan 30 18:47:20 2024, max compression
+gzip compressed data, was "qiskit-superstaq-0.5.9.tar", last modified: Fri Feb  9 16:13:23 2024, max compression
```

## Comparing `qiskit-superstaq-0.5.8.tar` & `qiskit-superstaq-0.5.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:47:20.870479 qiskit-superstaq-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-01-30 18:47:20.870479 qiskit-superstaq-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/example-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:47:20.866479 qiskit-superstaq-0.5.8/qiskit_superstaq/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/qiskit_superstaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/qiskit_superstaq/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/qiskit_superstaq/_version_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/qiskit_superstaq/compiler_output.py
--rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/qiskit_superstaq/compiler_output_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/qiskit_superstaq/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    17522 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/qiskit_superstaq/custom_gates.py
--rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/qiskit_superstaq/custom_gates_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/qiskit_superstaq/daily_integration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/qiskit_superstaq/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14453 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/qiskit_superstaq/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13765 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/qiskit_superstaq/serialization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    23215 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/qiskit_superstaq/superstaq_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    12594 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/qiskit_superstaq/superstaq_backend_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14404 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/qiskit_superstaq/superstaq_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    20906 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/qiskit_superstaq/superstaq_job_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24325 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/qiskit_superstaq/superstaq_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    18350 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/qiskit_superstaq/superstaq_provider_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/qiskit_superstaq/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/qiskit_superstaq/validation_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:47:20.870479 qiskit-superstaq-0.5.8/qiskit_superstaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-01-30 18:47:20.000000 qiskit-superstaq-0.5.8/qiskit_superstaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-01-30 18:47:20.000000 qiskit-superstaq-0.5.8/qiskit_superstaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 18:47:20.000000 qiskit-superstaq-0.5.8/qiskit_superstaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-01-30 18:47:20.000000 qiskit-superstaq-0.5.8/qiskit_superstaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-30 18:47:20.000000 qiskit-superstaq-0.5.8/qiskit_superstaq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-30 18:46:39.000000 qiskit-superstaq-0.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 18:47:20.870479 qiskit-superstaq-0.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:13:23.989145 qiskit-superstaq-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-02-09 16:13:23.989145 qiskit-superstaq-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/example-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:13:23.985145 qiskit-superstaq-0.5.9/qiskit_superstaq/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/qiskit_superstaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/qiskit_superstaq/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/qiskit_superstaq/_version_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/qiskit_superstaq/compiler_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/qiskit_superstaq/compiler_output_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/qiskit_superstaq/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17522 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/qiskit_superstaq/custom_gates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/qiskit_superstaq/custom_gates_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10117 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/qiskit_superstaq/daily_integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/qiskit_superstaq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14457 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/qiskit_superstaq/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13765 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/qiskit_superstaq/serialization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23215 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/qiskit_superstaq/superstaq_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12594 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/qiskit_superstaq/superstaq_backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14404 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/qiskit_superstaq/superstaq_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20906 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/qiskit_superstaq/superstaq_job_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24325 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/qiskit_superstaq/superstaq_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18350 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/qiskit_superstaq/superstaq_provider_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/qiskit_superstaq/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/qiskit_superstaq/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:13:23.989145 qiskit-superstaq-0.5.9/qiskit_superstaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-02-09 16:13:23.000000 qiskit-superstaq-0.5.9/qiskit_superstaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-02-09 16:13:23.000000 qiskit-superstaq-0.5.9/qiskit_superstaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 16:13:23.000000 qiskit-superstaq-0.5.9/qiskit_superstaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-09 16:13:23.000000 qiskit-superstaq-0.5.9/qiskit_superstaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-09 16:13:23.000000 qiskit-superstaq-0.5.9/qiskit_superstaq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-09 16:12:41.000000 qiskit-superstaq-0.5.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 16:13:23.989145 qiskit-superstaq-0.5.9/setup.cfg
```

### Comparing `qiskit-superstaq-0.5.8/PKG-INFO` & `qiskit-superstaq-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: qiskit-superstaq
-Version: 0.5.8
+Version: 0.5.9
 Summary: The Qiskit module that provides tools and access to Superstaq.
 Author-email: Superstaq development team <superstaq@infleqtion.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/Infleqtion/client-superstaq
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
-Requires-Dist: general-superstaq~=0.5.8
+Requires-Dist: general-superstaq~=0.5.9
 Requires-Dist: qiskit>=0.44.1
 Requires-Dist: qiskit-ibm-provider>=0.7.2
 Requires-Dist: symengine~=0.11.0
 Provides-Extra: dev
-Requires-Dist: checks-superstaq~=0.5.8; extra == "dev"
+Requires-Dist: checks-superstaq~=0.5.9; extra == "dev"
 Requires-Dist: matplotlib>=3.0.0; extra == "dev"
 Requires-Dist: notebook>=6.5.5; extra == "dev"
 Requires-Dist: pylatexenc>=2.0; extra == "dev"
 Provides-Extra: examples
 Requires-Dist: matplotlib>=3.0.0; extra == "examples"
 Requires-Dist: notebook>=6.5.5; extra == "examples"
 Requires-Dist: pylatexenc>=2.0; extra == "examples"
```

### Comparing `qiskit-superstaq-0.5.8/README.md` & `qiskit-superstaq-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.5.8/pyproject.toml` & `qiskit-superstaq-0.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.5.8/qiskit_superstaq/__init__.py` & `qiskit-superstaq-0.5.9/qiskit_superstaq/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.5.8/qiskit_superstaq/compiler_output.py` & `qiskit-superstaq-0.5.9/qiskit_superstaq/compiler_output.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.5.8/qiskit_superstaq/compiler_output_test.py` & `qiskit-superstaq-0.5.9/qiskit_superstaq/compiler_output_test.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.5.8/qiskit_superstaq/conftest.py` & `qiskit-superstaq-0.5.9/qiskit_superstaq/conftest.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.5.8/qiskit_superstaq/custom_gates.py` & `qiskit-superstaq-0.5.9/qiskit_superstaq/custom_gates.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.5.8/qiskit_superstaq/custom_gates_test.py` & `qiskit-superstaq-0.5.9/qiskit_superstaq/custom_gates_test.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.5.8/qiskit_superstaq/daily_integration_test.py` & `qiskit-superstaq-0.5.9/qiskit_superstaq/daily_integration_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,25 @@
 
 @pytest.fixture
 def provider() -> qss.SuperstaqProvider:
     return qss.SuperstaqProvider()
 
 
 def test_backends(provider: qss.SuperstaqProvider) -> None:
-    result = provider.backends()
-    assert provider.get_backend("ibmq_qasm_simulator") in result
+    result = provider.get_targets()
+    ibmq_backend_info = gss.typing.Target(
+        target="ibmq_qasm_simulator",
+        supports_submit=True,
+        supports_submit_qubo=False,
+        supports_compile=True,
+        available=True,
+        retired=False,
+    )
+    assert ibmq_backend_info in result
+    assert provider.get_backend("ibmq_qasm_simulator").name == "ibmq_qasm_simulator"
 
 
 def test_ibmq_compile(provider: qss.SuperstaqProvider) -> None:
     qc = qiskit.QuantumCircuit(4)
     qc.append(qss.AceCR("-+"), [0, 1])
     qc.append(qss.AceCR("-+"), [1, 2])
     qc.append(qss.AceCR("-+"), [2, 3])
```

### Comparing `qiskit-superstaq-0.5.8/qiskit_superstaq/serialization.py` & `qiskit-superstaq-0.5.9/qiskit_superstaq/serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from collections.abc import Callable, Sequence
 from typing import TypeVar
 
 import general_superstaq as gss
 import numpy as np
 import numpy.typing as npt
 import qiskit.qpy
-import qiskit_ibm_provider
+import qiskit_ibm_provider.qpy
 
 import qiskit_superstaq as qss
 
 T = TypeVar("T")
 
 # Custom gate types to resolve when deserializing circuits
 # MSGate included as a workaround for https://github.com/Qiskit/qiskit/issues/11378
```

### Comparing `qiskit-superstaq-0.5.8/qiskit_superstaq/serialization_test.py` & `qiskit-superstaq-0.5.9/qiskit_superstaq/serialization_test.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.5.8/qiskit_superstaq/superstaq_backend.py` & `qiskit-superstaq-0.5.9/qiskit_superstaq/superstaq_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.5.8/qiskit_superstaq/superstaq_backend_test.py` & `qiskit-superstaq-0.5.9/qiskit_superstaq/superstaq_backend_test.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.5.8/qiskit_superstaq/superstaq_job.py` & `qiskit-superstaq-0.5.9/qiskit_superstaq/superstaq_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.5.8/qiskit_superstaq/superstaq_job_test.py` & `qiskit-superstaq-0.5.9/qiskit_superstaq/superstaq_job_test.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.5.8/qiskit_superstaq/superstaq_provider.py` & `qiskit-superstaq-0.5.9/qiskit_superstaq/superstaq_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.5.8/qiskit_superstaq/superstaq_provider_test.py` & `qiskit-superstaq-0.5.9/qiskit_superstaq/superstaq_provider_test.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.5.8/qiskit_superstaq/validation.py` & `qiskit-superstaq-0.5.9/qiskit_superstaq/validation.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.5.8/qiskit_superstaq/validation_test.py` & `qiskit-superstaq-0.5.9/qiskit_superstaq/validation_test.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.5.8/qiskit_superstaq.egg-info/PKG-INFO` & `qiskit-superstaq-0.5.9/qiskit_superstaq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: qiskit-superstaq
-Version: 0.5.8
+Version: 0.5.9
 Summary: The Qiskit module that provides tools and access to Superstaq.
 Author-email: Superstaq development team <superstaq@infleqtion.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/Infleqtion/client-superstaq
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
-Requires-Dist: general-superstaq~=0.5.8
+Requires-Dist: general-superstaq~=0.5.9
 Requires-Dist: qiskit>=0.44.1
 Requires-Dist: qiskit-ibm-provider>=0.7.2
 Requires-Dist: symengine~=0.11.0
 Provides-Extra: dev
-Requires-Dist: checks-superstaq~=0.5.8; extra == "dev"
+Requires-Dist: checks-superstaq~=0.5.9; extra == "dev"
 Requires-Dist: matplotlib>=3.0.0; extra == "dev"
 Requires-Dist: notebook>=6.5.5; extra == "dev"
 Requires-Dist: pylatexenc>=2.0; extra == "dev"
 Provides-Extra: examples
 Requires-Dist: matplotlib>=3.0.0; extra == "examples"
 Requires-Dist: notebook>=6.5.5; extra == "examples"
 Requires-Dist: pylatexenc>=2.0; extra == "examples"
```

### Comparing `qiskit-superstaq-0.5.8/qiskit_superstaq.egg-info/SOURCES.txt` & `qiskit-superstaq-0.5.9/qiskit_superstaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

