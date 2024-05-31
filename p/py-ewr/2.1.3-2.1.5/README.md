# Comparing `tmp/py_ewr-2.1.3.tar.gz` & `tmp/py_ewr-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ewr-2.1.3.tar", last modified: Fri May 31 04:34:48 2024, max compression
+gzip compressed data, was "py_ewr-2.1.5.tar", last modified: Fri May 31 04:35:28 2024, max compression
```

## Comparing `py_ewr-2.1.3.tar` & `py_ewr-2.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 04:34:48.432059 py_ewr-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-31 04:34:43.000000 py_ewr-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-05-31 04:34:48.432059 py_ewr-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-05-31 04:34:43.000000 py_ewr-2.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 04:34:48.428059 py_ewr-2.1.3/py_ewr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 04:34:43.000000 py_ewr-2.1.3/py_ewr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18046 2024-05-31 04:34:43.000000 py_ewr-2.1.3/py_ewr/data_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)   229279 2024-05-31 04:34:43.000000 py_ewr-2.1.3/py_ewr/evaluate_EWRs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 04:34:48.428059 py_ewr-2.1.3/py_ewr/model_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)   164412 2024-05-31 04:34:43.000000 py_ewr-2.1.3/py_ewr/model_metadata/SiteID_MDBA.csv
--rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-05-31 04:34:43.000000 py_ewr-2.1.3/py_ewr/model_metadata/SiteID_NSW.csv
--rw-r--r--   0 runner    (1001) docker     (127)    18173 2024-05-31 04:34:43.000000 py_ewr-2.1.3/py_ewr/observed_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 04:34:48.428059 py_ewr-2.1.3/py_ewr/parameter_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)    17556 2024-05-31 04:34:43.000000 py_ewr-2.1.3/py_ewr/parameter_metadata/ewr_calc_config.json
--rw-r--r--   0 runner    (1001) docker     (127)   594257 2024-05-31 04:34:43.000000 py_ewr-2.1.3/py_ewr/parameter_metadata/parameter_sheet.csv
--rw-r--r--   0 runner    (1001) docker     (127)    28184 2024-05-31 04:34:43.000000 py_ewr-2.1.3/py_ewr/scenario_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)    29747 2024-05-31 04:34:43.000000 py_ewr-2.1.3/py_ewr/summarise_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 04:34:48.432059 py_ewr-2.1.3/py_ewr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-05-31 04:34:48.000000 py_ewr-2.1.3/py_ewr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-31 04:34:48.000000 py_ewr-2.1.3/py_ewr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 04:34:48.000000 py_ewr-2.1.3/py_ewr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-31 04:34:48.000000 py_ewr-2.1.3/py_ewr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-31 04:34:48.000000 py_ewr-2.1.3/py_ewr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-31 04:34:43.000000 py_ewr-2.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 04:34:48.432059 py_ewr-2.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-31 04:34:43.000000 py_ewr-2.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 04:34:48.432059 py_ewr-2.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-05-31 04:34:43.000000 py_ewr-2.1.3/tests/test_data_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)   184847 2024-05-31 04:34:43.000000 py_ewr-2.1.3/tests/test_evaluate_ewr_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)    90413 2024-05-31 04:34:43.000000 py_ewr-2.1.3/tests/test_evaluate_ewrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-05-31 04:34:43.000000 py_ewr-2.1.3/tests/test_observed_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)    17159 2024-05-31 04:34:43.000000 py_ewr-2.1.3/tests/test_scenario_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-05-31 04:34:43.000000 py_ewr-2.1.3/tests/test_summarise_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 04:35:28.063656 py_ewr-2.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-31 04:35:24.000000 py_ewr-2.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-05-31 04:35:28.063656 py_ewr-2.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-05-31 04:35:24.000000 py_ewr-2.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 04:35:28.059656 py_ewr-2.1.5/py_ewr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 04:35:24.000000 py_ewr-2.1.5/py_ewr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18046 2024-05-31 04:35:24.000000 py_ewr-2.1.5/py_ewr/data_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   229279 2024-05-31 04:35:24.000000 py_ewr-2.1.5/py_ewr/evaluate_EWRs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 04:35:28.063656 py_ewr-2.1.5/py_ewr/model_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)   164412 2024-05-31 04:35:24.000000 py_ewr-2.1.5/py_ewr/model_metadata/SiteID_MDBA.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-05-31 04:35:24.000000 py_ewr-2.1.5/py_ewr/model_metadata/SiteID_NSW.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    18173 2024-05-31 04:35:24.000000 py_ewr-2.1.5/py_ewr/observed_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 04:35:28.063656 py_ewr-2.1.5/py_ewr/parameter_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    17556 2024-05-31 04:35:24.000000 py_ewr-2.1.5/py_ewr/parameter_metadata/ewr_calc_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)   594257 2024-05-31 04:35:24.000000 py_ewr-2.1.5/py_ewr/parameter_metadata/parameter_sheet.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    28184 2024-05-31 04:35:24.000000 py_ewr-2.1.5/py_ewr/scenario_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29747 2024-05-31 04:35:24.000000 py_ewr-2.1.5/py_ewr/summarise_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 04:35:28.063656 py_ewr-2.1.5/py_ewr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-05-31 04:35:28.000000 py_ewr-2.1.5/py_ewr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-31 04:35:28.000000 py_ewr-2.1.5/py_ewr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 04:35:28.000000 py_ewr-2.1.5/py_ewr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-31 04:35:28.000000 py_ewr-2.1.5/py_ewr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-31 04:35:28.000000 py_ewr-2.1.5/py_ewr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-31 04:35:24.000000 py_ewr-2.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 04:35:28.063656 py_ewr-2.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-31 04:35:24.000000 py_ewr-2.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 04:35:28.063656 py_ewr-2.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-05-31 04:35:24.000000 py_ewr-2.1.5/tests/test_data_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   184847 2024-05-31 04:35:24.000000 py_ewr-2.1.5/tests/test_evaluate_ewr_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90413 2024-05-31 04:35:24.000000 py_ewr-2.1.5/tests/test_evaluate_ewrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-05-31 04:35:24.000000 py_ewr-2.1.5/tests/test_observed_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17159 2024-05-31 04:35:24.000000 py_ewr-2.1.5/tests/test_scenario_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-05-31 04:35:24.000000 py_ewr-2.1.5/tests/test_summarise_results.py
```

### Comparing `py_ewr-2.1.3/LICENSE` & `py_ewr-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ewr-2.1.3/PKG-INFO` & `py_ewr-2.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ewr
-Version: 2.1.3
+Version: 2.1.5
 Summary: Environmental Water Requirement calculator
 Home-page: https://github.com/MDBAuth/EWR_tool
 Author: Martin Job
 Author-email: Martin.Job@mdba.gov.au
 Project-URL: Bug Tracker, https://github.com/MDBAuth/EWR_tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -28,15 +28,15 @@
 Requires-Dist: cachetools==5.2.0
 
 [![CI](https://github.com/MDBAuth/EWR_tool/actions/workflows/test-release.yml/badge.svg)]()
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/py-ewr)](https://pypi.org/project/py-ewr/)
 [![PyPI](https://img.shields.io/pypi/v/py-ewr)](https://pypi.org/project/py-ewr/)
 [![DOI](https://zenodo.org/badge/342122359.svg)](https://zenodo.org/badge/latestdoi/342122359)
 
-### **EWR tool version 2.1.3 README**
+### **EWR tool version 2.1.5 README**
 
 ### **Notes on recent version update**
 - Standard time-series handling added - each column needs a gauge, followed by and underscore, followed by either flow or level (e.g. 409025_flow). This handling also has missing date filling - so any missing dates will be filled with NaN values in all columns.
 - ten thousand year handling - the same formatting as above is required (gauge_flow OR gauge_level)
 - bug fixes: spells of length equal to the minimum required spell length were getting filtered out of the successful events table and successful interevents table.
 
 ### **Installation**
```

### Comparing `py_ewr-2.1.3/README.md` & `py_ewr-2.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![CI](https://github.com/MDBAuth/EWR_tool/actions/workflows/test-release.yml/badge.svg)]()
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/py-ewr)](https://pypi.org/project/py-ewr/)
 [![PyPI](https://img.shields.io/pypi/v/py-ewr)](https://pypi.org/project/py-ewr/)
 [![DOI](https://zenodo.org/badge/342122359.svg)](https://zenodo.org/badge/latestdoi/342122359)
 
-### **EWR tool version 2.1.3 README**
+### **EWR tool version 2.1.5 README**
 
 ### **Notes on recent version update**
 - Standard time-series handling added - each column needs a gauge, followed by and underscore, followed by either flow or level (e.g. 409025_flow). This handling also has missing date filling - so any missing dates will be filled with NaN values in all columns.
 - ten thousand year handling - the same formatting as above is required (gauge_flow OR gauge_level)
 - bug fixes: spells of length equal to the minimum required spell length were getting filtered out of the successful events table and successful interevents table.
 
 ### **Installation**
```

### Comparing `py_ewr-2.1.3/py_ewr/data_inputs.py` & `py_ewr-2.1.5/py_ewr/data_inputs.py`

 * *Files identical despite different names*

### Comparing `py_ewr-2.1.3/py_ewr/evaluate_EWRs.py` & `py_ewr-2.1.5/py_ewr/evaluate_EWRs.py`

 * *Files identical despite different names*

### Comparing `py_ewr-2.1.3/py_ewr/model_metadata/SiteID_MDBA.csv` & `py_ewr-2.1.5/py_ewr/model_metadata/SiteID_MDBA.csv`

 * *Files identical despite different names*

### Comparing `py_ewr-2.1.3/py_ewr/model_metadata/SiteID_NSW.csv` & `py_ewr-2.1.5/py_ewr/model_metadata/SiteID_NSW.csv`

 * *Files identical despite different names*

### Comparing `py_ewr-2.1.3/py_ewr/observed_handling.py` & `py_ewr-2.1.5/py_ewr/observed_handling.py`

 * *Files identical despite different names*

### Comparing `py_ewr-2.1.3/py_ewr/parameter_metadata/ewr_calc_config.json` & `py_ewr-2.1.5/py_ewr/parameter_metadata/ewr_calc_config.json`

 * *Files identical despite different names*

### Comparing `py_ewr-2.1.3/py_ewr/parameter_metadata/parameter_sheet.csv` & `py_ewr-2.1.5/py_ewr/parameter_metadata/parameter_sheet.csv`

 * *Files identical despite different names*

### Comparing `py_ewr-2.1.3/py_ewr/scenario_handling.py` & `py_ewr-2.1.5/py_ewr/scenario_handling.py`

 * *Files identical despite different names*

### Comparing `py_ewr-2.1.3/py_ewr/summarise_results.py` & `py_ewr-2.1.5/py_ewr/summarise_results.py`

 * *Files identical despite different names*

### Comparing `py_ewr-2.1.3/py_ewr.egg-info/PKG-INFO` & `py_ewr-2.1.5/py_ewr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ewr
-Version: 2.1.3
+Version: 2.1.5
 Summary: Environmental Water Requirement calculator
 Home-page: https://github.com/MDBAuth/EWR_tool
 Author: Martin Job
 Author-email: Martin.Job@mdba.gov.au
 Project-URL: Bug Tracker, https://github.com/MDBAuth/EWR_tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -28,15 +28,15 @@
 Requires-Dist: cachetools==5.2.0
 
 [![CI](https://github.com/MDBAuth/EWR_tool/actions/workflows/test-release.yml/badge.svg)]()
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/py-ewr)](https://pypi.org/project/py-ewr/)
 [![PyPI](https://img.shields.io/pypi/v/py-ewr)](https://pypi.org/project/py-ewr/)
 [![DOI](https://zenodo.org/badge/342122359.svg)](https://zenodo.org/badge/latestdoi/342122359)
 
-### **EWR tool version 2.1.3 README**
+### **EWR tool version 2.1.5 README**
 
 ### **Notes on recent version update**
 - Standard time-series handling added - each column needs a gauge, followed by and underscore, followed by either flow or level (e.g. 409025_flow). This handling also has missing date filling - so any missing dates will be filled with NaN values in all columns.
 - ten thousand year handling - the same formatting as above is required (gauge_flow OR gauge_level)
 - bug fixes: spells of length equal to the minimum required spell length were getting filtered out of the successful events table and successful interevents table.
 
 ### **Installation**
```

### Comparing `py_ewr-2.1.3/py_ewr.egg-info/SOURCES.txt` & `py_ewr-2.1.5/py_ewr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_ewr-2.1.3/setup.py` & `py_ewr-2.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="py_ewr",
-    version="2.1.3",
+    version="2.1.5",
     author="Martin Job",
     author_email="Martin.Job@mdba.gov.au",
     description="Environmental Water Requirement calculator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MDBAuth/EWR_tool",
     project_urls={
```

### Comparing `py_ewr-2.1.3/tests/test_data_inputs.py` & `py_ewr-2.1.5/tests/test_data_inputs.py`

 * *Files identical despite different names*

### Comparing `py_ewr-2.1.3/tests/test_evaluate_ewr_rest.py` & `py_ewr-2.1.5/tests/test_evaluate_ewr_rest.py`

 * *Files identical despite different names*

### Comparing `py_ewr-2.1.3/tests/test_evaluate_ewrs.py` & `py_ewr-2.1.5/tests/test_evaluate_ewrs.py`

 * *Files identical despite different names*

### Comparing `py_ewr-2.1.3/tests/test_observed_handling.py` & `py_ewr-2.1.5/tests/test_observed_handling.py`

 * *Files identical despite different names*

### Comparing `py_ewr-2.1.3/tests/test_scenario_handling.py` & `py_ewr-2.1.5/tests/test_scenario_handling.py`

 * *Files identical despite different names*

### Comparing `py_ewr-2.1.3/tests/test_summarise_results.py` & `py_ewr-2.1.5/tests/test_summarise_results.py`

 * *Files identical despite different names*

