# Comparing `tmp/ansys_tools_path-0.5.2.tar.gz` & `tmp/ansys_tools_path-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_tools_path-0.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_tools_path-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_tools_path-0.5.2.tar` & `ansys_tools_path-0.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1089 2024-04-15 19:06:49.783151 ansys_tools_path-0.5.2/LICENSE
--rw-r--r--   0        0        0     4692 2024-04-15 19:06:49.783151 ansys_tools_path-0.5.2/README.rst
--rw-r--r--   0        0        0     2027 2024-04-15 19:06:49.787151 ansys_tools_path-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1697 2024-04-15 19:06:49.787151 ansys_tools_path-0.5.2/src/ansys/tools/path/__init__.py
--rw-r--r--   0        0        0      297 2024-04-15 19:06:49.787151 ansys_tools_path-0.5.2/src/ansys/tools/path/applications/__init__.py
--rw-r--r--   0        0        0     1298 2024-04-15 19:06:49.787151 ansys_tools_path-0.5.2/src/ansys/tools/path/applications/dyna.py
--rw-r--r--   0        0        0     1417 2024-04-15 19:06:49.787151 ansys_tools_path-0.5.2/src/ansys/tools/path/applications/mapdl.py
--rw-r--r--   0        0        0     1726 2024-04-15 19:06:49.787151 ansys_tools_path-0.5.2/src/ansys/tools/path/applications/mechanical.py
--rw-r--r--   0        0        0      677 2024-04-15 19:06:49.787151 ansys_tools_path-0.5.2/src/ansys/tools/path/misc.py
--rw-r--r--   0        0        0    38410 2024-04-15 19:06:49.787151 ansys_tools_path-0.5.2/src/ansys/tools/path/path.py
--rw-r--r--   0        0        0        0 2024-04-15 19:06:49.787151 ansys_tools_path-0.5.2/src/ansys/tools/path/py.typed
--rw-r--r--   0        0        0     1971 2024-04-15 19:06:49.787151 ansys_tools_path-0.5.2/src/ansys/tools/path/save.py
--rw-r--r--   0        0        0     6227 1970-01-01 00:00:00.000000 ansys_tools_path-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-05-31 13:47:52.977856 ansys_tools_path-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4692 2024-05-31 13:47:52.977856 ansys_tools_path-0.6.0/README.rst
+-rw-r--r--   0        0        0     1996 2024-05-31 13:47:52.977856 ansys_tools_path-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1697 2024-05-31 13:47:52.977856 ansys_tools_path-0.6.0/src/ansys/tools/path/__init__.py
+-rw-r--r--   0        0        0      297 2024-05-31 13:47:52.977856 ansys_tools_path-0.6.0/src/ansys/tools/path/applications/__init__.py
+-rw-r--r--   0        0        0     1298 2024-05-31 13:47:52.977856 ansys_tools_path-0.6.0/src/ansys/tools/path/applications/dyna.py
+-rw-r--r--   0        0        0     1417 2024-05-31 13:47:52.977856 ansys_tools_path-0.6.0/src/ansys/tools/path/applications/mapdl.py
+-rw-r--r--   0        0        0     1726 2024-05-31 13:47:52.977856 ansys_tools_path-0.6.0/src/ansys/tools/path/applications/mechanical.py
+-rw-r--r--   0        0        0      677 2024-05-31 13:47:52.977856 ansys_tools_path-0.6.0/src/ansys/tools/path/misc.py
+-rw-r--r--   0        0        0    38429 2024-05-31 13:47:52.977856 ansys_tools_path-0.6.0/src/ansys/tools/path/path.py
+-rw-r--r--   0        0        0        0 2024-05-31 13:47:52.977856 ansys_tools_path-0.6.0/src/ansys/tools/path/py.typed
+-rw-r--r--   0        0        0     1971 2024-05-31 13:47:52.977856 ansys_tools_path-0.6.0/src/ansys/tools/path/save.py
+-rw-r--r--   0        0        0     6227 1970-01-01 00:00:00.000000 ansys_tools_path-0.6.0/PKG-INFO
```

### Comparing `ansys_tools_path-0.5.2/LICENSE` & `ansys_tools_path-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.5.2/README.rst` & `ansys_tools_path-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.5.2/pyproject.toml` & `ansys_tools_path-0.6.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-tools-path"
-version = "0.5.2"
+version = "0.6.0"
 description = "Library to locate Ansys products in a local machine."
 readme = "README.rst"
 requires-python = ">=3.8,<4"
 license = { file = "LICENSE" }
 authors = [{ name = "ANSYS, Inc.", email = "pyansys.core@ansys.com" }]
 maintainers = [{ name = "ANSYS, Inc.", email = "pyansys.core@ansys.com" }]
 
@@ -26,24 +26,24 @@
 dependencies = [
     "platformdirs>=3.6.0",
     "click>=8.1.3",        # for CLI interface
 ]
 
 
 [project.optional-dependencies]
-tests = ["pytest==8.1.1", "pytest-cov==5.0.0", "pyfakefs==5.4.1"]
+tests = ["pytest==8.2.1", "pytest-cov==5.0.0", "pyfakefs==5.5.0"]
 
 doc = [
-    "Sphinx==7.2.6",
+    "Sphinx==7.3.7",
     "numpydoc==1.7.0",
-    "ansys-sphinx-theme==0.15.2",
+    "ansys-sphinx-theme==0.16.2",
     "sphinx-copybutton==0.5.2",
 ]
 
-build = ["build==1.2.1", "twine==5.0.0"]
+build = ["build==1.2.1", "twine==5.1.0"]
 
 [tool.flit.module]
 name = "ansys.tools.path"
 
 [project.scripts]
 save-ansys-path = "ansys.tools.path.save:cli"
 
@@ -57,15 +57,14 @@
 [tool.black]
 line-length = 100
 
 [tool.isort]
 profile = "black"
 force_sort_within_sections = true
 line_length = 100
-default_section = "THIRDPARTY"
 src_paths = ["doc", "src", "tests"]
 
 [tool.flake8]
 max-line-length = 100
 
 [tool.coverage.run]
 source = ["ansys.tools"]
```

### Comparing `ansys_tools_path-0.5.2/src/ansys/tools/path/__init__.py` & `ansys_tools_path-0.6.0/src/ansys/tools/path/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.5.2/src/ansys/tools/path/applications/dyna.py` & `ansys_tools_path-0.6.0/src/ansys/tools/path/applications/dyna.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.5.2/src/ansys/tools/path/applications/mapdl.py` & `ansys_tools_path-0.6.0/src/ansys/tools/path/applications/mapdl.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.5.2/src/ansys/tools/path/applications/mechanical.py` & `ansys_tools_path-0.6.0/src/ansys/tools/path/applications/mechanical.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.5.2/src/ansys/tools/path/misc.py` & `ansys_tools_path-0.6.0/src/ansys/tools/path/misc.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.5.2/src/ansys/tools/path/path.py` & `ansys_tools_path-0.6.0/src/ansys/tools/path/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 LINUX_DEFAULT_DIRS = [["/", "usr", "ansys_inc"], ["/", "ansys_inc"], ["/", "install", "ansys_inc"]]
 LINUX_DEFAULT_DIRS = [os.path.join(*each) for each in LINUX_DEFAULT_DIRS]
 
 CONFIG_FILE_NAME = "config.txt"
 
 SUPPORTED_ANSYS_VERSIONS: SUPPORTED_VERSIONS_TYPE = {
+    251: "2025R1",
     242: "2024R2",
     241: "2024R1",
     232: "2023R2",
     231: "2023R1",
     222: "2022R2",
     221: "2022R1",
     212: "2021R2",
```

### Comparing `ansys_tools_path-0.5.2/src/ansys/tools/path/save.py` & `ansys_tools_path-0.6.0/src/ansys/tools/path/save.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.5.2/PKG-INFO` & `ansys_tools_path-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-tools-path
-Version: 0.5.2
+Version: 0.6.0
 Summary: Library to locate Ansys products in a local machine.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
@@ -13,22 +13,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: platformdirs>=3.6.0
 Requires-Dist: click>=8.1.3
 Requires-Dist: build==1.2.1 ; extra == "build"
-Requires-Dist: twine==5.0.0 ; extra == "build"
-Requires-Dist: Sphinx==7.2.6 ; extra == "doc"
+Requires-Dist: twine==5.1.0 ; extra == "build"
+Requires-Dist: Sphinx==7.3.7 ; extra == "doc"
 Requires-Dist: numpydoc==1.7.0 ; extra == "doc"
-Requires-Dist: ansys-sphinx-theme==0.15.2 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.16.2 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
-Requires-Dist: pytest==8.1.1 ; extra == "tests"
+Requires-Dist: pytest==8.2.1 ; extra == "tests"
 Requires-Dist: pytest-cov==5.0.0 ; extra == "tests"
-Requires-Dist: pyfakefs==5.4.1 ; extra == "tests"
+Requires-Dist: pyfakefs==5.5.0 ; extra == "tests"
 Project-URL: Documentation, https://path.tools.docs.pyansys.com
 Project-URL: Homepage, https://github.com/ansys/ansys-tools-path
 Project-URL: Source, https://github.com/ansys/ansys-tools-path
 Project-URL: Tracker, https://github.com/ansys/ansys-tools-path/issues
 Provides-Extra: build
 Provides-Extra: doc
 Provides-Extra: tests
```

