# Comparing `tmp/cirq-superstaq-0.5.8.tar.gz` & `tmp/cirq-superstaq-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cirq-superstaq-0.5.8.tar", last modified: Tue Jan 30 18:47:35 2024, max compression
+gzip compressed data, was "cirq-superstaq-0.5.9.tar", last modified: Fri Feb  9 16:13:39 2024, max compression
```

## Comparing `cirq-superstaq-0.5.8.tar` & `cirq-superstaq-0.5.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:47:35.322321 cirq-superstaq-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-01-30 18:47:35.322321 cirq-superstaq-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:47:35.318321 cirq-superstaq-0.5.8/cirq_superstaq/
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/cirq_superstaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/cirq_superstaq/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/cirq_superstaq/_version_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    16243 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/cirq_superstaq/compiler_output.py
--rw-r--r--   0 runner    (1001) docker     (127)    19187 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/cirq_superstaq/compiler_output_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11614 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/cirq_superstaq/daily_integration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17989 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/cirq_superstaq/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    15405 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/cirq_superstaq/job_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:47:35.318321 cirq-superstaq-0.5.8/cirq_superstaq/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/cirq_superstaq/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35183 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/cirq_superstaq/ops/qubit_gates.py
--rw-r--r--   0 runner    (1001) docker     (127)    38616 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/cirq_superstaq/ops/qubit_gates_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24838 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/cirq_superstaq/ops/qudit_gates.py
--rw-r--r--   0 runner    (1001) docker     (127)    21520 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/cirq_superstaq/ops/qudit_gates_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/cirq_superstaq/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/cirq_superstaq/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/cirq_superstaq/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/cirq_superstaq/serialization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    42079 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/cirq_superstaq/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    30388 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/cirq_superstaq/service_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/cirq_superstaq/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/cirq_superstaq/validation_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:47:35.322321 cirq-superstaq-0.5.8/cirq_superstaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-01-30 18:47:35.000000 cirq-superstaq-0.5.8/cirq_superstaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-01-30 18:47:35.000000 cirq-superstaq-0.5.8/cirq_superstaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 18:47:35.000000 cirq-superstaq-0.5.8/cirq_superstaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-30 18:47:35.000000 cirq-superstaq-0.5.8/cirq_superstaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-30 18:47:35.000000 cirq-superstaq-0.5.8/cirq_superstaq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/example-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-30 18:46:39.000000 cirq-superstaq-0.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 18:47:35.322321 cirq-superstaq-0.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:13:39.873274 cirq-superstaq-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-02-09 16:13:39.873274 cirq-superstaq-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:13:39.869274 cirq-superstaq-0.5.9/cirq_superstaq/
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/cirq_superstaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/cirq_superstaq/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/cirq_superstaq/_version_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16243 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/cirq_superstaq/compiler_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19187 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/cirq_superstaq/compiler_output_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11614 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/cirq_superstaq/daily_integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17989 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/cirq_superstaq/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15405 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/cirq_superstaq/job_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:13:39.873274 cirq-superstaq-0.5.9/cirq_superstaq/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/cirq_superstaq/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35183 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/cirq_superstaq/ops/qubit_gates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38616 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/cirq_superstaq/ops/qubit_gates_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24838 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/cirq_superstaq/ops/qudit_gates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21520 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/cirq_superstaq/ops/qudit_gates_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/cirq_superstaq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/cirq_superstaq/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/cirq_superstaq/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/cirq_superstaq/serialization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42079 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/cirq_superstaq/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30388 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/cirq_superstaq/service_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/cirq_superstaq/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/cirq_superstaq/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:13:39.873274 cirq-superstaq-0.5.9/cirq_superstaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-02-09 16:13:39.000000 cirq-superstaq-0.5.9/cirq_superstaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-02-09 16:13:39.000000 cirq-superstaq-0.5.9/cirq_superstaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 16:13:39.000000 cirq-superstaq-0.5.9/cirq_superstaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-09 16:13:39.000000 cirq-superstaq-0.5.9/cirq_superstaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-09 16:13:39.000000 cirq-superstaq-0.5.9/cirq_superstaq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/example-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-09 16:12:41.000000 cirq-superstaq-0.5.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 16:13:39.873274 cirq-superstaq-0.5.9/setup.cfg
```

### Comparing `cirq-superstaq-0.5.8/PKG-INFO` & `cirq-superstaq-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cirq-superstaq
-Version: 0.5.8
+Version: 0.5.9
 Summary: The Cirq module that provides tools and access to Superstaq.
 Author-email: Superstaq development team <superstaq@infleqtion.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/Infleqtion/client-superstaq
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Requires-Dist: cirq-core>=1.0.0
-Requires-Dist: general-superstaq~=0.5.8
+Requires-Dist: general-superstaq~=0.5.9
 Provides-Extra: dev
-Requires-Dist: checks-superstaq~=0.5.8; extra == "dev"
+Requires-Dist: checks-superstaq~=0.5.9; extra == "dev"
 Requires-Dist: notebook>=6.5.5; extra == "dev"
-Requires-Dist: qiskit-superstaq~=0.5.8; extra == "dev"
+Requires-Dist: qiskit-superstaq~=0.5.9; extra == "dev"
 Provides-Extra: examples
 Requires-Dist: notebook>=6.5.5; extra == "examples"
-Requires-Dist: qiskit-superstaq~=0.5.8; extra == "examples"
+Requires-Dist: qiskit-superstaq~=0.5.9; extra == "examples"
 
 # `cirq-superstaq`
 
 ![cirq-superstaq's default workflow](https://github.com/Infleqtion/client-superstaq/actions/workflows/ci.yml/badge.svg)
 
 This package is used to access Superstaq via a Web API through [Cirq](https://github.com/quantumlib/Cirq).
 Cirq programmers can take advantage of the applications, pulse level optimizations, and write-once-target-all
```

### Comparing `cirq-superstaq-0.5.8/README.md` & `cirq-superstaq-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.5.8/cirq_superstaq/__init__.py` & `cirq-superstaq-0.5.9/cirq_superstaq/__init__.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.5.8/cirq_superstaq/compiler_output.py` & `cirq-superstaq-0.5.9/cirq_superstaq/compiler_output.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.5.8/cirq_superstaq/compiler_output_test.py` & `cirq-superstaq-0.5.9/cirq_superstaq/compiler_output_test.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.5.8/cirq_superstaq/daily_integration_test.py` & `cirq-superstaq-0.5.9/cirq_superstaq/daily_integration_test.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.5.8/cirq_superstaq/job.py` & `cirq-superstaq-0.5.9/cirq_superstaq/job.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.5.8/cirq_superstaq/job_test.py` & `cirq-superstaq-0.5.9/cirq_superstaq/job_test.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.5.8/cirq_superstaq/ops/__init__.py` & `cirq-superstaq-0.5.9/cirq_superstaq/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.5.8/cirq_superstaq/ops/qubit_gates.py` & `cirq-superstaq-0.5.9/cirq_superstaq/ops/qubit_gates.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.5.8/cirq_superstaq/ops/qubit_gates_test.py` & `cirq-superstaq-0.5.9/cirq_superstaq/ops/qubit_gates_test.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.5.8/cirq_superstaq/ops/qudit_gates.py` & `cirq-superstaq-0.5.9/cirq_superstaq/ops/qudit_gates.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.5.8/cirq_superstaq/ops/qudit_gates_test.py` & `cirq-superstaq-0.5.9/cirq_superstaq/ops/qudit_gates_test.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.5.8/cirq_superstaq/sampler.py` & `cirq-superstaq-0.5.9/cirq_superstaq/sampler.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.5.8/cirq_superstaq/serialization.py` & `cirq-superstaq-0.5.9/cirq_superstaq/serialization.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.5.8/cirq_superstaq/serialization_test.py` & `cirq-superstaq-0.5.9/cirq_superstaq/serialization_test.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.5.8/cirq_superstaq/service.py` & `cirq-superstaq-0.5.9/cirq_superstaq/service.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.5.8/cirq_superstaq/service_test.py` & `cirq-superstaq-0.5.9/cirq_superstaq/service_test.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.5.8/cirq_superstaq/validation.py` & `cirq-superstaq-0.5.9/cirq_superstaq/validation.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.5.8/cirq_superstaq/validation_test.py` & `cirq-superstaq-0.5.9/cirq_superstaq/validation_test.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.5.8/cirq_superstaq.egg-info/PKG-INFO` & `cirq-superstaq-0.5.9/cirq_superstaq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cirq-superstaq
-Version: 0.5.8
+Version: 0.5.9
 Summary: The Cirq module that provides tools and access to Superstaq.
 Author-email: Superstaq development team <superstaq@infleqtion.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/Infleqtion/client-superstaq
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Requires-Dist: cirq-core>=1.0.0
-Requires-Dist: general-superstaq~=0.5.8
+Requires-Dist: general-superstaq~=0.5.9
 Provides-Extra: dev
-Requires-Dist: checks-superstaq~=0.5.8; extra == "dev"
+Requires-Dist: checks-superstaq~=0.5.9; extra == "dev"
 Requires-Dist: notebook>=6.5.5; extra == "dev"
-Requires-Dist: qiskit-superstaq~=0.5.8; extra == "dev"
+Requires-Dist: qiskit-superstaq~=0.5.9; extra == "dev"
 Provides-Extra: examples
 Requires-Dist: notebook>=6.5.5; extra == "examples"
-Requires-Dist: qiskit-superstaq~=0.5.8; extra == "examples"
+Requires-Dist: qiskit-superstaq~=0.5.9; extra == "examples"
 
 # `cirq-superstaq`
 
 ![cirq-superstaq's default workflow](https://github.com/Infleqtion/client-superstaq/actions/workflows/ci.yml/badge.svg)
 
 This package is used to access Superstaq via a Web API through [Cirq](https://github.com/quantumlib/Cirq).
 Cirq programmers can take advantage of the applications, pulse level optimizations, and write-once-target-all
```

### Comparing `cirq-superstaq-0.5.8/cirq_superstaq.egg-info/SOURCES.txt` & `cirq-superstaq-0.5.9/cirq_superstaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.5.8/pyproject.toml` & `cirq-superstaq-0.5.9/pyproject.toml`

 * *Files identical despite different names*

