# Comparing `tmp/general-superstaq-0.5.8.tar.gz` & `tmp/general-superstaq-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "general-superstaq-0.5.8.tar", last modified: Tue Jan 30 18:47:06 2024, max compression
+gzip compressed data, was "general-superstaq-0.5.9.tar", last modified: Fri Feb  9 16:13:08 2024, max compression
```

## Comparing `general-superstaq-0.5.8.tar` & `general-superstaq-0.5.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:47:06.014636 general-superstaq-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-01-30 18:47:06.014636 general-superstaq-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:47:06.014636 general-superstaq-0.5.8/general_superstaq/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/general_superstaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/general_superstaq/_init_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/general_superstaq/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/general_superstaq/_version_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:47:06.014636 general-superstaq-0.5.8/general_superstaq/check/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/general_superstaq/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/general_superstaq/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/general_superstaq/qubo.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/general_superstaq/qubo_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/general_superstaq/resource_estimate.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/general_superstaq/resource_estimate_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/general_superstaq/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/general_superstaq/serialization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    15908 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/general_superstaq/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/general_superstaq/service_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    29324 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/general_superstaq/superstaq_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    30145 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/general_superstaq/superstaq_client_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/general_superstaq/superstaq_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/general_superstaq/superstaq_exceptions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/general_superstaq/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/general_superstaq/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/general_superstaq/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/general_superstaq/validation_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:47:06.014636 general-superstaq-0.5.8/general_superstaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-01-30 18:47:06.000000 general-superstaq-0.5.8/general_superstaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-01-30 18:47:06.000000 general-superstaq-0.5.8/general_superstaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 18:47:06.000000 general-superstaq-0.5.8/general_superstaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-01-30 18:47:06.000000 general-superstaq-0.5.8/general_superstaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-30 18:47:06.000000 general-superstaq-0.5.8/general_superstaq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-30 18:46:39.000000 general-superstaq-0.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 18:47:06.014636 general-superstaq-0.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:13:08.801026 general-superstaq-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-02-09 16:13:08.801026 general-superstaq-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:13:08.797026 general-superstaq-0.5.9/general_superstaq/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/general_superstaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/general_superstaq/_init_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/general_superstaq/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/general_superstaq/_version_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:13:08.797026 general-superstaq-0.5.9/general_superstaq/check/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/general_superstaq/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/general_superstaq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/general_superstaq/qubo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/general_superstaq/qubo_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/general_superstaq/resource_estimate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/general_superstaq/resource_estimate_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/general_superstaq/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/general_superstaq/serialization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15908 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/general_superstaq/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/general_superstaq/service_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29324 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/general_superstaq/superstaq_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30145 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/general_superstaq/superstaq_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/general_superstaq/superstaq_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/general_superstaq/superstaq_exceptions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/general_superstaq/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/general_superstaq/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/general_superstaq/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/general_superstaq/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:13:08.801026 general-superstaq-0.5.9/general_superstaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-02-09 16:13:08.000000 general-superstaq-0.5.9/general_superstaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-02-09 16:13:08.000000 general-superstaq-0.5.9/general_superstaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 16:13:08.000000 general-superstaq-0.5.9/general_superstaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-09 16:13:08.000000 general-superstaq-0.5.9/general_superstaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-09 16:13:08.000000 general-superstaq-0.5.9/general_superstaq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-09 16:12:41.000000 general-superstaq-0.5.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 16:13:08.801026 general-superstaq-0.5.9/setup.cfg
```

### Comparing `general-superstaq-0.5.8/PKG-INFO` & `general-superstaq-0.5.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: general-superstaq
-Version: 0.5.8
+Version: 0.5.9
 Summary: The general module that provides tools and access to Superstaq.
 Author-email: Superstaq development team <superstaq@infleqtion.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/Infleqtion/client-superstaq
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: pydantic>=1.10.7
 Requires-Dist: qubovert>=1.2.3
 Requires-Dist: requests>=2.26.0
 Provides-Extra: dev
-Requires-Dist: checks-superstaq~=0.5.8; extra == "dev"
+Requires-Dist: checks-superstaq~=0.5.9; extra == "dev"
 Requires-Dist: pyyaml>=6.0; extra == "dev"
 
 # general-superstaq
 This package contains code that is common across our clients ([cirq-superstaq](https://github.com/Infleqtion/client-superstaq#-cirq-superstaq-) and [qiskit-superstaq](https://github.com/Infleqtion/client-superstaq#-qiskit-superstaq-)) and [Supermarq](https://github.com/Infleqtion/client-superstaq#-supermarq-).
```

### Comparing `general-superstaq-0.5.8/general_superstaq/__init__.py` & `general-superstaq-0.5.9/general_superstaq/__init__.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.5.8/general_superstaq/resource_estimate.py` & `general-superstaq-0.5.9/general_superstaq/resource_estimate.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.5.8/general_superstaq/serialization.py` & `general-superstaq-0.5.9/general_superstaq/serialization.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.5.8/general_superstaq/service.py` & `general-superstaq-0.5.9/general_superstaq/service.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.5.8/general_superstaq/service_test.py` & `general-superstaq-0.5.9/general_superstaq/service_test.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.5.8/general_superstaq/superstaq_client.py` & `general-superstaq-0.5.9/general_superstaq/superstaq_client.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.5.8/general_superstaq/superstaq_client_test.py` & `general-superstaq-0.5.9/general_superstaq/superstaq_client_test.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.5.8/general_superstaq/superstaq_exceptions.py` & `general-superstaq-0.5.9/general_superstaq/superstaq_exceptions.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.5.8/general_superstaq/superstaq_exceptions_test.py` & `general-superstaq-0.5.9/general_superstaq/superstaq_exceptions_test.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.5.8/general_superstaq/testing.py` & `general-superstaq-0.5.9/general_superstaq/testing.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.5.8/general_superstaq/typing.py` & `general-superstaq-0.5.9/general_superstaq/typing.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.5.8/general_superstaq/validation.py` & `general-superstaq-0.5.9/general_superstaq/validation.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.5.8/general_superstaq/validation_test.py` & `general-superstaq-0.5.9/general_superstaq/validation_test.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.5.8/general_superstaq.egg-info/PKG-INFO` & `general-superstaq-0.5.9/general_superstaq.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: general-superstaq
-Version: 0.5.8
+Version: 0.5.9
 Summary: The general module that provides tools and access to Superstaq.
 Author-email: Superstaq development team <superstaq@infleqtion.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/Infleqtion/client-superstaq
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: pydantic>=1.10.7
 Requires-Dist: qubovert>=1.2.3
 Requires-Dist: requests>=2.26.0
 Provides-Extra: dev
-Requires-Dist: checks-superstaq~=0.5.8; extra == "dev"
+Requires-Dist: checks-superstaq~=0.5.9; extra == "dev"
 Requires-Dist: pyyaml>=6.0; extra == "dev"
 
 # general-superstaq
 This package contains code that is common across our clients ([cirq-superstaq](https://github.com/Infleqtion/client-superstaq#-cirq-superstaq-) and [qiskit-superstaq](https://github.com/Infleqtion/client-superstaq#-qiskit-superstaq-)) and [Supermarq](https://github.com/Infleqtion/client-superstaq#-supermarq-).
```

### Comparing `general-superstaq-0.5.8/general_superstaq.egg-info/SOURCES.txt` & `general-superstaq-0.5.9/general_superstaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.5.8/pyproject.toml` & `general-superstaq-0.5.9/pyproject.toml`

 * *Files identical despite different names*

