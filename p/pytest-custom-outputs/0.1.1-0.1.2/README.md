# Comparing `tmp/pytest_custom_outputs-0.1.1.tar.gz` & `tmp/pytest_custom_outputs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_custom_outputs-0.1.1.tar", last modified: Thu May 30 00:54:14 2024, max compression
+gzip compressed data, was "pytest_custom_outputs-0.1.2.tar", last modified: Thu May 30 00:57:34 2024, max compression
```

## Comparing `pytest_custom_outputs-0.1.1.tar` & `pytest_custom_outputs-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-30 00:54:14.373583 pytest_custom_outputs-0.1.1/
--rw-r--r--   0 user      (1000) vboxusers   (136)     1501 2024-04-09 20:33:50.000000 pytest_custom_outputs-0.1.1/LICENSE
--rw-r--r--   0 user      (1000) vboxusers   (136)     9671 2024-05-30 00:54:14.373583 pytest_custom_outputs-0.1.1/PKG-INFO
--rw-r--r--   0 user      (1000) vboxusers   (136)     6675 2024-05-30 00:52:21.000000 pytest_custom_outputs-0.1.1/README.rst
--rw-r--r--   0 user      (1000) vboxusers   (136)     1490 2024-05-30 00:52:45.000000 pytest_custom_outputs-0.1.1/pyproject.toml
--rw-r--r--   0 user      (1000) vboxusers   (136)       38 2024-05-30 00:54:14.373583 pytest_custom_outputs-0.1.1/setup.cfg
-drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-30 00:54:14.373583 pytest_custom_outputs-0.1.1/src/
-drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-30 00:54:14.373583 pytest_custom_outputs-0.1.1/src/pytest_custom_outputs/
--rw-r--r--   0 user      (1000) vboxusers   (136)        0 2024-04-09 20:33:50.000000 pytest_custom_outputs-0.1.1/src/pytest_custom_outputs/__init__.py
--rw-r--r--   0 user      (1000) vboxusers   (136)     2390 2024-04-09 23:37:27.000000 pytest_custom_outputs-0.1.1/src/pytest_custom_outputs/custom_outputs.py
-drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-30 00:54:14.373583 pytest_custom_outputs-0.1.1/src/pytest_custom_outputs.egg-info/
--rw-r--r--   0 user      (1000) vboxusers   (136)     9671 2024-05-30 00:54:14.000000 pytest_custom_outputs-0.1.1/src/pytest_custom_outputs.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) vboxusers   (136)      411 2024-05-30 00:54:14.000000 pytest_custom_outputs-0.1.1/src/pytest_custom_outputs.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) vboxusers   (136)        1 2024-05-30 00:54:14.000000 pytest_custom_outputs-0.1.1/src/pytest_custom_outputs.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) vboxusers   (136)       65 2024-05-30 00:54:14.000000 pytest_custom_outputs-0.1.1/src/pytest_custom_outputs.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) vboxusers   (136)       14 2024-05-30 00:54:14.000000 pytest_custom_outputs-0.1.1/src/pytest_custom_outputs.egg-info/requires.txt
--rw-r--r--   0 user      (1000) vboxusers   (136)       22 2024-05-30 00:54:14.000000 pytest_custom_outputs-0.1.1/src/pytest_custom_outputs.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-30 00:57:34.619867 pytest_custom_outputs-0.1.2/
+-rw-r--r--   0 user      (1000) vboxusers   (136)     1501 2024-04-09 20:33:50.000000 pytest_custom_outputs-0.1.2/LICENSE
+-rw-r--r--   0 user      (1000) vboxusers   (136)     9608 2024-05-30 00:57:34.619867 pytest_custom_outputs-0.1.2/PKG-INFO
+-rw-r--r--   0 user      (1000) vboxusers   (136)     6612 2024-05-30 00:56:50.000000 pytest_custom_outputs-0.1.2/README.rst
+-rw-r--r--   0 user      (1000) vboxusers   (136)     1490 2024-05-30 00:57:28.000000 pytest_custom_outputs-0.1.2/pyproject.toml
+-rw-r--r--   0 user      (1000) vboxusers   (136)       38 2024-05-30 00:57:34.619867 pytest_custom_outputs-0.1.2/setup.cfg
+drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-30 00:57:34.619867 pytest_custom_outputs-0.1.2/src/
+drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-30 00:57:34.619867 pytest_custom_outputs-0.1.2/src/pytest_custom_outputs/
+-rw-r--r--   0 user      (1000) vboxusers   (136)        0 2024-04-09 20:33:50.000000 pytest_custom_outputs-0.1.2/src/pytest_custom_outputs/__init__.py
+-rw-r--r--   0 user      (1000) vboxusers   (136)     2390 2024-04-09 23:37:27.000000 pytest_custom_outputs-0.1.2/src/pytest_custom_outputs/custom_outputs.py
+drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-30 00:57:34.619867 pytest_custom_outputs-0.1.2/src/pytest_custom_outputs.egg-info/
+-rw-r--r--   0 user      (1000) vboxusers   (136)     9608 2024-05-30 00:57:34.000000 pytest_custom_outputs-0.1.2/src/pytest_custom_outputs.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) vboxusers   (136)      411 2024-05-30 00:57:34.000000 pytest_custom_outputs-0.1.2/src/pytest_custom_outputs.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) vboxusers   (136)        1 2024-05-30 00:57:34.000000 pytest_custom_outputs-0.1.2/src/pytest_custom_outputs.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) vboxusers   (136)       65 2024-05-30 00:57:34.000000 pytest_custom_outputs-0.1.2/src/pytest_custom_outputs.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) vboxusers   (136)       14 2024-05-30 00:57:34.000000 pytest_custom_outputs-0.1.2/src/pytest_custom_outputs.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) vboxusers   (136)       22 2024-05-30 00:57:34.000000 pytest_custom_outputs-0.1.2/src/pytest_custom_outputs.egg-info/top_level.txt
```

### Comparing `pytest_custom_outputs-0.1.1/LICENSE` & `pytest_custom_outputs-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_custom_outputs-0.1.1/PKG-INFO` & `pytest_custom_outputs-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-custom_outputs
-Version: 0.1.1
+Version: 0.1.2
 Summary: A plugin that allows users to create and use custom outputs instead of the standard Pass and Fail
 Author-email: Babak Michael Engheta <michaelengheta55@gmail.com>
 Maintainer-email: Babak Michael Engheta <michaelengheta55@gmail.com>
 License: 
         Copyright (c) 2024, Babak Michael Engheta
         All rights reserved.
         
@@ -50,18 +50,14 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytest>=6.2.0
 
-pytest-custom_outputs
-
-Overview
---------
 
 Enhance Your Pytest Reporting with Customizable Test Outputs
 
 Tired of the standard pass/fail binary in pytest? With pytest-custom_outputs, you can create expressive and informative custom test results that go beyond the ordinary.  Tailor your reports to provide deeper insights into your test scenarios.
 
 Useful for if you want more than just the default Pass, Fail, and Skip outcomes.
 
@@ -71,24 +67,20 @@
 
 - Flexible Output Types: Define new outcome types like "unimplemented", "soft_fail"," "inconclusive," or any custom label that suits your testing needs.
 - Fully Customizeable: Custom outputs are customizable in their name, description, result code, tag, and color.
 - Seamless Integration: Easily incorporate custom outputs into your existing pytest test suites.
 - Terminal and File Reporting: View your custom outputs in both your terminal output and pytest file reports.
 
 
-Requirements
-------------
-
-None
-
-
 Installation
 ------------
 
+```bash
 pip install pytest-custom_outputs
+```
 
 
 Usage
 -----
 
 In the directory where you will be running your pytest, create a file called "pytest_custom_outputs.json".
 You will use this file to create your own custom outputs.
```

### Comparing `pytest_custom_outputs-0.1.1/README.rst` & `pytest_custom_outputs-0.1.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-pytest-custom_outputs
-
-Overview
---------
 
 Enhance Your Pytest Reporting with Customizable Test Outputs
 
 Tired of the standard pass/fail binary in pytest? With pytest-custom_outputs, you can create expressive and informative custom test results that go beyond the ordinary.  Tailor your reports to provide deeper insights into your test scenarios.
 
 Useful for if you want more than just the default Pass, Fail, and Skip outcomes.
 
@@ -15,24 +11,20 @@
 
 - Flexible Output Types: Define new outcome types like "unimplemented", "soft_fail"," "inconclusive," or any custom label that suits your testing needs.
 - Fully Customizeable: Custom outputs are customizable in their name, description, result code, tag, and color.
 - Seamless Integration: Easily incorporate custom outputs into your existing pytest test suites.
 - Terminal and File Reporting: View your custom outputs in both your terminal output and pytest file reports.
 
 
-Requirements
-------------
-
-None
-
-
 Installation
 ------------
 
+```bash
 pip install pytest-custom_outputs
+```
 
 
 Usage
 -----
 
 In the directory where you will be running your pytest, create a file called "pytest_custom_outputs.json".
 You will use this file to create your own custom outputs.
```

### Comparing `pytest_custom_outputs-0.1.1/pyproject.toml` & `pytest_custom_outputs-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=61.0.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytest-custom_outputs"
 description = "A plugin that allows users to create and use custom outputs instead of the standard Pass and Fail"
-version = "0.1.1"
+version = "0.1.2"
 readme = {file = "README.rst", content-type = "text/markdown"}
 requires-python = ">=3.8"
 authors = [
     { name = "Babak Michael Engheta", email = "michaelengheta55@gmail.com" },
 ]
 maintainers = [
     { name = "Babak Michael Engheta", email = "michaelengheta55@gmail.com" },
```

### Comparing `pytest_custom_outputs-0.1.1/src/pytest_custom_outputs/custom_outputs.py` & `pytest_custom_outputs-0.1.2/src/pytest_custom_outputs/custom_outputs.py`

 * *Files identical despite different names*

### Comparing `pytest_custom_outputs-0.1.1/src/pytest_custom_outputs.egg-info/PKG-INFO` & `pytest_custom_outputs-0.1.2/src/pytest_custom_outputs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-custom_outputs
-Version: 0.1.1
+Version: 0.1.2
 Summary: A plugin that allows users to create and use custom outputs instead of the standard Pass and Fail
 Author-email: Babak Michael Engheta <michaelengheta55@gmail.com>
 Maintainer-email: Babak Michael Engheta <michaelengheta55@gmail.com>
 License: 
         Copyright (c) 2024, Babak Michael Engheta
         All rights reserved.
         
@@ -50,18 +50,14 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytest>=6.2.0
 
-pytest-custom_outputs
-
-Overview
---------
 
 Enhance Your Pytest Reporting with Customizable Test Outputs
 
 Tired of the standard pass/fail binary in pytest? With pytest-custom_outputs, you can create expressive and informative custom test results that go beyond the ordinary.  Tailor your reports to provide deeper insights into your test scenarios.
 
 Useful for if you want more than just the default Pass, Fail, and Skip outcomes.
 
@@ -71,24 +67,20 @@
 
 - Flexible Output Types: Define new outcome types like "unimplemented", "soft_fail"," "inconclusive," or any custom label that suits your testing needs.
 - Fully Customizeable: Custom outputs are customizable in their name, description, result code, tag, and color.
 - Seamless Integration: Easily incorporate custom outputs into your existing pytest test suites.
 - Terminal and File Reporting: View your custom outputs in both your terminal output and pytest file reports.
 
 
-Requirements
-------------
-
-None
-
-
 Installation
 ------------
 
+```bash
 pip install pytest-custom_outputs
+```
 
 
 Usage
 -----
 
 In the directory where you will be running your pytest, create a file called "pytest_custom_outputs.json".
 You will use this file to create your own custom outputs.
```

