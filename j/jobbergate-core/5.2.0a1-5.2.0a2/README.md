# Comparing `tmp/jobbergate_core-5.2.0a1.tar.gz` & `tmp/jobbergate_core-5.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate_core-5.2.0a1.tar", max compression
+gzip compressed data, was "jobbergate_core-5.2.0a2.tar", max compression
```

## Comparing `jobbergate_core-5.2.0a1.tar` & `jobbergate_core-5.2.0a2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1082 2024-05-24 13:00:30.180921 jobbergate_core-5.2.0a1/LICENSE
--rw-r--r--   0        0        0      371 2024-05-24 13:00:30.180921 jobbergate_core-5.2.0a1/README.md
--rw-r--r--   0        0        0      330 2024-05-24 13:00:30.180921 jobbergate_core-5.2.0a1/jobbergate_core/__init__.py
--rw-r--r--   0        0        0      367 2024-05-24 13:00:30.180921 jobbergate_core-5.2.0a1/jobbergate_core/auth/__init__.py
--rw-r--r--   0        0        0      279 2024-05-24 13:00:30.180921 jobbergate_core-5.2.0a1/jobbergate_core/auth/exceptions.py
--rw-r--r--   0        0        0    11832 2024-05-24 13:00:30.180921 jobbergate_core-5.2.0a1/jobbergate_core/auth/handler.py
--rw-r--r--   0        0        0     5529 2024-05-24 13:00:30.180921 jobbergate_core-5.2.0a1/jobbergate_core/auth/token.py
--rw-r--r--   0        0        0        0 2024-05-24 13:00:30.180921 jobbergate_core-5.2.0a1/jobbergate_core/py.typed
--rw-r--r--   0        0        0        0 2024-05-24 13:00:30.180921 jobbergate_core-5.2.0a1/jobbergate_core/tools/__init__.py
--rw-r--r--   0        0        0     6411 2024-05-24 13:00:30.180921 jobbergate_core-5.2.0a1/jobbergate_core/tools/sbatch.py
--rw-r--r--   0        0        0      209 2024-05-24 13:00:30.180921 jobbergate_core-5.2.0a1/jobbergate_core/version.py
--rw-r--r--   0        0        0     1838 2024-05-24 13:00:30.180921 jobbergate_core-5.2.0a1/pyproject.toml
--rw-r--r--   0        0        0     1537 1970-01-01 00:00:00.000000 jobbergate_core-5.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-05-31 17:18:20.624356 jobbergate_core-5.2.0a2/LICENSE
+-rw-r--r--   0        0        0      371 2024-05-31 17:18:20.624356 jobbergate_core-5.2.0a2/README.md
+-rw-r--r--   0        0        0      330 2024-05-31 17:18:20.624356 jobbergate_core-5.2.0a2/jobbergate_core/__init__.py
+-rw-r--r--   0        0        0      367 2024-05-31 17:18:20.624356 jobbergate_core-5.2.0a2/jobbergate_core/auth/__init__.py
+-rw-r--r--   0        0        0      279 2024-05-31 17:18:20.624356 jobbergate_core-5.2.0a2/jobbergate_core/auth/exceptions.py
+-rw-r--r--   0        0        0    11832 2024-05-31 17:18:20.624356 jobbergate_core-5.2.0a2/jobbergate_core/auth/handler.py
+-rw-r--r--   0        0        0     5529 2024-05-31 17:18:20.624356 jobbergate_core-5.2.0a2/jobbergate_core/auth/token.py
+-rw-r--r--   0        0        0        0 2024-05-31 17:18:20.624356 jobbergate_core-5.2.0a2/jobbergate_core/py.typed
+-rw-r--r--   0        0        0        0 2024-05-31 17:18:20.624356 jobbergate_core-5.2.0a2/jobbergate_core/tools/__init__.py
+-rw-r--r--   0        0        0     6411 2024-05-31 17:18:20.624356 jobbergate_core-5.2.0a2/jobbergate_core/tools/sbatch.py
+-rw-r--r--   0        0        0      209 2024-05-31 17:18:20.624356 jobbergate_core-5.2.0a2/jobbergate_core/version.py
+-rw-r--r--   0        0        0     1838 2024-05-31 17:18:20.624356 jobbergate_core-5.2.0a2/pyproject.toml
+-rw-r--r--   0        0        0     1537 1970-01-01 00:00:00.000000 jobbergate_core-5.2.0a2/PKG-INFO
```

### Comparing `jobbergate_core-5.2.0a1/LICENSE` & `jobbergate_core-5.2.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate_core-5.2.0a1/jobbergate_core/auth/handler.py` & `jobbergate_core-5.2.0a2/jobbergate_core/auth/handler.py`

 * *Files identical despite different names*

### Comparing `jobbergate_core-5.2.0a1/jobbergate_core/auth/token.py` & `jobbergate_core-5.2.0a2/jobbergate_core/auth/token.py`

 * *Files identical despite different names*

### Comparing `jobbergate_core-5.2.0a1/jobbergate_core/tools/sbatch.py` & `jobbergate_core-5.2.0a2/jobbergate_core/tools/sbatch.py`

 * *Files identical despite different names*

### Comparing `jobbergate_core-5.2.0a1/pyproject.toml` & `jobbergate_core-5.2.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-core"
-version = "5.2.0a1"
+version = "5.2.0a2"
 description = "Jobbergate Core"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `jobbergate_core-5.2.0a1/PKG-INFO` & `jobbergate_core-5.2.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobbergate-core
-Version: 5.2.0a1
+Version: 5.2.0a2
 Summary: Jobbergate Core
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

