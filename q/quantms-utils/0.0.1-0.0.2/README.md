# Comparing `tmp/quantms_utils-0.0.1.tar.gz` & `tmp/quantms_utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantms_utils-0.0.1.tar", last modified: Wed May 29 10:51:56 2024, max compression
+gzip compressed data, was "quantms_utils-0.0.2.tar", last modified: Fri May 31 17:05:31 2024, max compression
```

## Comparing `quantms_utils-0.0.1.tar` & `quantms_utils-0.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:51:56.530560 quantms_utils-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-29 10:51:52.000000 quantms_utils-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-29 10:51:56.530560 quantms_utils-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-29 10:51:52.000000 quantms_utils-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-29 10:51:52.000000 quantms_utils-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:51:56.530560 quantms_utils-0.0.1/quantms_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-29 10:51:56.000000 quantms_utils-0.0.1/quantms_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-29 10:51:56.000000 quantms_utils-0.0.1/quantms_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:51:56.000000 quantms_utils-0.0.1/quantms_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-29 10:51:56.000000 quantms_utils-0.0.1/quantms_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-29 10:51:56.000000 quantms_utils-0.0.1/quantms_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-29 10:51:56.000000 quantms_utils-0.0.1/quantms_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:51:56.526560 quantms_utils-0.0.1/quantmsutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:51:52.000000 quantms_utils-0.0.1/quantmsutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:51:56.530560 quantms_utils-0.0.1/quantmsutils/diann/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:51:52.000000 quantms_utils-0.0.1/quantmsutils/diann/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59274 2024-05-29 10:51:52.000000 quantms_utils-0.0.1/quantmsutils/diann/diann2mztab.py
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-05-29 10:51:52.000000 quantms_utils-0.0.1/quantmsutils/diann/dianncfg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:51:56.530560 quantms_utils-0.0.1/quantmsutils/features/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:51:52.000000 quantms_utils-0.0.1/quantmsutils/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-29 10:51:52.000000 quantms_utils-0.0.1/quantmsutils/features/sage_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:51:56.530560 quantms_utils-0.0.1/quantmsutils/mzml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:51:52.000000 quantms_utils-0.0.1/quantmsutils/mzml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-05-29 10:51:52.000000 quantms_utils-0.0.1/quantmsutils/mzml/mzml_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:51:56.530560 quantms_utils-0.0.1/quantmsutils/psm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:51:52.000000 quantms_utils-0.0.1/quantmsutils/psm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-05-29 10:51:52.000000 quantms_utils-0.0.1/quantmsutils/psm/psm_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-29 10:51:52.000000 quantms_utils-0.0.1/quantmsutils/quantmsutilsc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:51:56.530560 quantms_utils-0.0.1/quantmsutils/rescoring/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:51:52.000000 quantms_utils-0.0.1/quantmsutils/rescoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-05-29 10:51:52.000000 quantms_utils-0.0.1/quantmsutils/rescoring/ms2rescore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:51:56.530560 quantms_utils-0.0.1/quantmsutils/sdrf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:51:52.000000 quantms_utils-0.0.1/quantmsutils/sdrf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-29 10:51:52.000000 quantms_utils-0.0.1/quantmsutils/sdrf/check_samplesheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-29 10:51:52.000000 quantms_utils-0.0.1/quantmsutils/sdrf/extract_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-29 10:51:56.530560 quantms_utils-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-29 10:51:52.000000 quantms_utils-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:51:56.530560 quantms_utils-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-29 10:51:52.000000 quantms_utils-0.0.1/tests/test_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:05:31.134614 quantms_utils-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-31 17:05:24.000000 quantms_utils-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-31 17:05:31.134614 quantms_utils-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-31 17:05:24.000000 quantms_utils-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-31 17:05:24.000000 quantms_utils-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:05:31.134614 quantms_utils-0.0.2/quantms_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-31 17:05:31.000000 quantms_utils-0.0.2/quantms_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-31 17:05:31.000000 quantms_utils-0.0.2/quantms_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 17:05:31.000000 quantms_utils-0.0.2/quantms_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-31 17:05:31.000000 quantms_utils-0.0.2/quantms_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-31 17:05:31.000000 quantms_utils-0.0.2/quantms_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-31 17:05:31.000000 quantms_utils-0.0.2/quantms_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:05:31.134614 quantms_utils-0.0.2/quantmsutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 17:05:24.000000 quantms_utils-0.0.2/quantmsutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:05:31.134614 quantms_utils-0.0.2/quantmsutils/diann/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 17:05:24.000000 quantms_utils-0.0.2/quantmsutils/diann/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59274 2024-05-31 17:05:24.000000 quantms_utils-0.0.2/quantmsutils/diann/diann2mztab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-05-31 17:05:24.000000 quantms_utils-0.0.2/quantmsutils/diann/dianncfg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:05:31.134614 quantms_utils-0.0.2/quantmsutils/features/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 17:05:24.000000 quantms_utils-0.0.2/quantmsutils/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-31 17:05:24.000000 quantms_utils-0.0.2/quantmsutils/features/sage_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:05:31.134614 quantms_utils-0.0.2/quantmsutils/mzml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 17:05:24.000000 quantms_utils-0.0.2/quantmsutils/mzml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-05-31 17:05:24.000000 quantms_utils-0.0.2/quantmsutils/mzml/mzml_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:05:31.134614 quantms_utils-0.0.2/quantmsutils/psm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 17:05:24.000000 quantms_utils-0.0.2/quantmsutils/psm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-05-31 17:05:24.000000 quantms_utils-0.0.2/quantmsutils/psm/psm_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-31 17:05:24.000000 quantms_utils-0.0.2/quantmsutils/quantmsutilsc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:05:31.134614 quantms_utils-0.0.2/quantmsutils/rescoring/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 17:05:24.000000 quantms_utils-0.0.2/quantmsutils/rescoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-05-31 17:05:24.000000 quantms_utils-0.0.2/quantmsutils/rescoring/ms2rescore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:05:31.134614 quantms_utils-0.0.2/quantmsutils/sdrf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 17:05:24.000000 quantms_utils-0.0.2/quantmsutils/sdrf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-31 17:05:24.000000 quantms_utils-0.0.2/quantmsutils/sdrf/check_samplesheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-31 17:05:24.000000 quantms_utils-0.0.2/quantmsutils/sdrf/extract_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 17:05:31.134614 quantms_utils-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-31 17:05:24.000000 quantms_utils-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:05:31.134614 quantms_utils-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-31 17:05:24.000000 quantms_utils-0.0.2/tests/test_commands.py
```

### Comparing `quantms_utils-0.0.1/LICENSE` & `quantms_utils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quantms_utils-0.0.1/PKG-INFO` & `quantms_utils-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantms-utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package with scripts and helpers for the QuantMS workflow
 Home-page: https://www.github.com/bigbio/pyquantms
 Author: Yasset Perez-Riverol, Dai Chengxin
 Author-email: ypriverol@gmail.com
 License: MIT License
 Project-URL: Documentation, https://docs.quantms.org/en/latest/
 Project-URL: quantms Workflow, https://github.com/bigbio/quantms
```

### Comparing `quantms_utils-0.0.1/README.md` & `quantms_utils-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `quantms_utils-0.0.1/pyproject.toml` & `quantms_utils-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 [tool.poetry]
 name = "quantms-utils"
-version = "0.0.1"
+version = "0.0.2"
 description = "Python scripts and helpers for the quantMS workflow"
 authors = ["Yasset Perez-Riverol", "Dai Chengxin"]
+packages = [
+    { include = "quantmsutils" }
+]
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry.dependencies]
 click = ">=7.0"
@@ -20,12 +23,15 @@
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-ra -q"
-testpaths = ["tests", ]
+testpaths = ["tests"]
 
 [tool.black]
 line-length = 88
-target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
+target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
+
+[tool.poetry.scripts]
+quantmsutilsc = "quantmsutils.quantmsutilsc:main"
```

### Comparing `quantms_utils-0.0.1/quantms_utils.egg-info/PKG-INFO` & `quantms_utils-0.0.2/quantms_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantms-utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package with scripts and helpers for the QuantMS workflow
 Home-page: https://www.github.com/bigbio/pyquantms
 Author: Yasset Perez-Riverol, Dai Chengxin
 Author-email: ypriverol@gmail.com
 License: MIT License
 Project-URL: Documentation, https://docs.quantms.org/en/latest/
 Project-URL: quantms Workflow, https://github.com/bigbio/quantms
```

### Comparing `quantms_utils-0.0.1/quantms_utils.egg-info/SOURCES.txt` & `quantms_utils-0.0.2/quantms_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quantms_utils-0.0.1/quantmsutils/diann/diann2mztab.py` & `quantms_utils-0.0.2/quantmsutils/diann/diann2mztab.py`

 * *Files identical despite different names*

### Comparing `quantms_utils-0.0.1/quantmsutils/diann/dianncfg.py` & `quantms_utils-0.0.2/quantmsutils/diann/dianncfg.py`

 * *Files identical despite different names*

### Comparing `quantms_utils-0.0.1/quantmsutils/features/sage_feature.py` & `quantms_utils-0.0.2/quantmsutils/features/sage_feature.py`

 * *Files identical despite different names*

### Comparing `quantms_utils-0.0.1/quantmsutils/mzml/mzml_statistics.py` & `quantms_utils-0.0.2/quantmsutils/mzml/mzml_statistics.py`

 * *Files identical despite different names*

### Comparing `quantms_utils-0.0.1/quantmsutils/psm/psm_conversion.py` & `quantms_utils-0.0.2/quantmsutils/psm/psm_conversion.py`

 * *Files identical despite different names*

### Comparing `quantms_utils-0.0.1/quantmsutils/quantmsutilsc.py` & `quantms_utils-0.0.2/quantmsutils/quantmsutilsc.py`

 * *Files identical despite different names*

### Comparing `quantms_utils-0.0.1/quantmsutils/rescoring/ms2rescore.py` & `quantms_utils-0.0.2/quantmsutils/rescoring/ms2rescore.py`

 * *Files identical despite different names*

### Comparing `quantms_utils-0.0.1/quantmsutils/sdrf/check_samplesheet.py` & `quantms_utils-0.0.2/quantmsutils/sdrf/check_samplesheet.py`

 * *Files identical despite different names*

### Comparing `quantms_utils-0.0.1/quantmsutils/sdrf/extract_sample.py` & `quantms_utils-0.0.2/quantmsutils/sdrf/extract_sample.py`

 * *Files identical despite different names*

### Comparing `quantms_utils-0.0.1/setup.py` & `quantms_utils-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 NAME = "quantms-utils"
 LICENSE = "MIT License"
 DESCRIPTION = "Python package with scripts and helpers for the QuantMS workflow"
 AUTHOR = "Yasset Perez-Riverol, Dai Chengxin"
 AUTHOR_EMAIL = "ypriverol@gmail.com"
 URL = "https://www.github.com/bigbio/pyquantms"
```

### Comparing `quantms_utils-0.0.1/tests/test_commands.py` & `quantms_utils-0.0.2/tests/test_commands.py`

 * *Files identical despite different names*

