# Comparing `tmp/adaptive-1.2.0.tar.gz` & `tmp/adaptive-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptive-1.2.0.tar", last modified: Wed Apr 10 07:51:04 2024, max compression
+gzip compressed data, was "adaptive-1.3.0.tar", last modified: Fri May 31 01:44:06 2024, max compression
```

## Comparing `adaptive-1.2.0.tar` & `adaptive-1.3.0.tar`

### file list

```diff
@@ -1,57 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:51:04.332553 adaptive-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-10 07:50:51.000000 adaptive-1.2.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-10 07:50:51.000000 adaptive-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 07:50:51.000000 adaptive-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12946 2024-04-10 07:51:04.332553 adaptive-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10733 2024-04-10 07:50:51.000000 adaptive-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:51:04.336553 adaptive-1.2.0/adaptive/
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-10 07:51:04.336553 adaptive-1.2.0/adaptive/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:51:04.328553 adaptive-1.2.0/adaptive/learner/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/average_learner.py
--rw-r--r--   0 runner    (1001) docker     (127)    26126 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/average_learner1D.py
--rw-r--r--   0 runner    (1001) docker     (127)    21987 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/balancing_learner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/base_learner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/data_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/integrator_coeffs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23366 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/integrator_learner.py
--rw-r--r--   0 runner    (1001) docker     (127)    33353 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/learner1D.py
--rw-r--r--   0 runner    (1001) docker     (127)    31038 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/learner2D.py
--rw-r--r--   0 runner    (1001) docker     (127)    45362 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/learnerND.py
--rw-r--r--   0 runner    (1001) docker     (127)     9773 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/sequence_learner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/skopt_learner.py
--rw-r--r--   0 runner    (1001) docker     (127)    24593 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/triangulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/notebook_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    47162 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:51:04.328553 adaptive-1.2.0/adaptive/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19316 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/algorithm_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_average_learner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_average_learner1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_balancing_learner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8704 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_cquad.py
--rw-r--r--   0 runner    (1001) docker     (127)    12699 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_learner1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_learnernd.py
--rw-r--r--   0 runner    (1001) docker     (127)    24883 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_learners.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_notebook_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_pickling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_sequence_learner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_skopt_learner.py
--rw-r--r--   0 runner    (1001) docker     (127)    10004 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_triangulation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:51:04.332553 adaptive-1.2.0/adaptive/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/unit/test_learnernd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/unit/test_learnernd_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/unit/test_triangulation.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:51:04.332553 adaptive-1.2.0/adaptive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12946 2024-04-10 07:51:04.000000 adaptive-1.2.0/adaptive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-10 07:51:04.000000 adaptive-1.2.0/adaptive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 07:51:04.000000 adaptive-1.2.0/adaptive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-10 07:51:04.000000 adaptive-1.2.0/adaptive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 07:51:04.000000 adaptive-1.2.0/adaptive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-10 07:50:51.000000 adaptive-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-10 07:51:04.332553 adaptive-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:44:06.025996 adaptive-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-31 01:43:55.000000 adaptive-1.3.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-31 01:43:55.000000 adaptive-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 01:43:55.000000 adaptive-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12844 2024-05-31 01:44:06.025996 adaptive-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10733 2024-05-31 01:43:55.000000 adaptive-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:44:06.029996 adaptive-1.3.0/adaptive/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-31 01:44:06.029996 adaptive-1.3.0/adaptive/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:44:06.021996 adaptive-1.3.0/adaptive/learner/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/learner/average_learner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26126 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/learner/average_learner1D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21987 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/learner/balancing_learner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/learner/base_learner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/learner/data_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/learner/integrator_coeffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23366 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/learner/integrator_learner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33353 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/learner/learner1D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31046 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/learner/learner2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45371 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/learner/learnerND.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9773 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/learner/sequence_learner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24593 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/learner/triangulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/notebook_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47162 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:44:06.025996 adaptive-1.3.0/adaptive/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19316 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/tests/algorithm_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/tests/test_average_learner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/tests/test_average_learner1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/tests/test_balancing_learner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8704 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/tests/test_cquad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12699 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/tests/test_learner1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/tests/test_learnernd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24520 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/tests/test_learners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/tests/test_notebook_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/tests/test_pickling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/tests/test_sequence_learner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10004 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/tests/test_triangulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:44:06.025996 adaptive-1.3.0/adaptive/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/tests/unit/test_learnernd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/tests/unit/test_learnernd_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/tests/unit/test_triangulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-31 01:43:55.000000 adaptive-1.3.0/adaptive/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:44:06.025996 adaptive-1.3.0/adaptive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12844 2024-05-31 01:44:06.000000 adaptive-1.3.0/adaptive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-31 01:44:06.000000 adaptive-1.3.0/adaptive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 01:44:06.000000 adaptive-1.3.0/adaptive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-31 01:44:06.000000 adaptive-1.3.0/adaptive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 01:44:06.000000 adaptive-1.3.0/adaptive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-31 01:43:55.000000 adaptive-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-31 01:44:06.025996 adaptive-1.3.0/setup.cfg
```

### Comparing `adaptive-1.2.0/AUTHORS.md` & `adaptive-1.3.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/LICENSE` & `adaptive-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/PKG-INFO` & `adaptive-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptive
-Version: 1.2.0
+Version: 1.3.0
 Summary: Parallel active learning of mathematical functions
 Maintainer: Adaptive authors
 License: BSD
 Project-URL: homepage, https://adaptive.readthedocs.io/
 Project-URL: documentation, https://adaptive.readthedocs.io/
 Project-URL: repository, https://github.com/python-adaptive/adaptive
 Classifier: Development Status :: 4 - Beta
@@ -25,16 +25,14 @@
 Requires-Dist: loky>=2.9
 Requires-Dist: typing_extensions; python_version < "3.10"
 Requires-Dist: versioningit
 Provides-Extra: other
 Requires-Dist: dill; extra == "other"
 Requires-Dist: distributed; extra == "other"
 Requires-Dist: ipyparallel>=6.2.5; extra == "other"
-Requires-Dist: scikit-optimize>=0.8.1; extra == "other"
-Requires-Dist: scikit-learn; extra == "other"
 Requires-Dist: wexpect; os_name == "nt" and extra == "other"
 Requires-Dist: pexpect; os_name != "nt" and extra == "other"
 Provides-Extra: notebook
 Requires-Dist: ipython; extra == "notebook"
 Requires-Dist: ipykernel>=4.8.0; extra == "notebook"
 Requires-Dist: jupyter_client>=5.2.2; extra == "notebook"
 Requires-Dist: holoviews>=1.9.1; extra == "notebook"
```

### Comparing `adaptive-1.2.0/README.md` & `adaptive-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/__init__.py` & `adaptive-1.3.0/adaptive/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from contextlib import suppress
-
 from adaptive._version import __version__
 from adaptive.learner import (
     AverageLearner,
     AverageLearner1D,
     BalancingLearner,
     BaseLearner,
     DataSaver,
@@ -43,15 +41,9 @@
     "live_plot",
     "notebook_extension",
     "AsyncRunner",
     "BlockingRunner",
     "Runner",
 ]
 
-with suppress(ImportError):
-    # Only available if 'scikit-optimize' is installed
-    from adaptive.learner import SKOptLearner  # noqa: F401
-
-    __all__.append("SKOptLearner")
-
 # to avoid confusion with `notebook_extension`
 del notebook_integration  # type: ignore[name-defined] # noqa: F821
```

### Comparing `adaptive-1.2.0/adaptive/learner/average_learner.py` & `adaptive-1.3.0/adaptive/learner/average_learner.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/learner/average_learner1D.py` & `adaptive-1.3.0/adaptive/learner/average_learner1D.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/learner/balancing_learner.py` & `adaptive-1.3.0/adaptive/learner/balancing_learner.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/learner/base_learner.py` & `adaptive-1.3.0/adaptive/learner/base_learner.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/learner/data_saver.py` & `adaptive-1.3.0/adaptive/learner/data_saver.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/learner/integrator_coeffs.py` & `adaptive-1.3.0/adaptive/learner/integrator_coeffs.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/learner/integrator_learner.py` & `adaptive-1.3.0/adaptive/learner/integrator_learner.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/learner/learner1D.py` & `adaptive-1.3.0/adaptive/learner/learner1D.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/learner/learner2D.py` & `adaptive-1.3.0/adaptive/learner/learner2D.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     ip : `scipy.interpolate.LinearNDInterpolator` instance
 
     Returns
     -------
     deviations : list
         The deviation per triangle.
     """
-    values = ip.values / (ip.values.ptp(axis=0).max() or 1)
+    values = ip.values / (np.ptp(ip.values, axis=0).max() or 1)
     gradients = interpolate.interpnd.estimate_gradients_2d_global(
         ip.tri, values, tol=1e-6
     )
 
     simplices = ip.tri.simplices
     p = ip.tri.points[simplices]
     vs = values[simplices]
@@ -191,15 +191,15 @@
     >>> learner = adaptive.Learner2D(f, bounds=[(-1, -1), (1, 1)],
     ...     loss_per_triangle=minimize_triangle_surface_loss)
     >>>
     """
     tri = ip.tri
     points = tri.points[tri.simplices]
     values = ip.values[tri.simplices]
-    values = values / (ip.values.ptp(axis=0).max() or 1)
+    values = values / (np.ptp(ip.values, axis=0).max() or 1)
 
     def _get_vectors(points):
         delta = points - points[:, -1, :][:, None, :]
         vectors = delta[:, :2, :]
         return vectors[:, 0, :], vectors[:, 1, :]
 
     a_xy, b_xy = _get_vectors(points)
```

### Comparing `adaptive-1.2.0/adaptive/learner/learnerND.py` & `adaptive-1.3.0/adaptive/learner/learnerND.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import functools
 import itertools
+import math
 import random
 from collections import OrderedDict
 from collections.abc import Iterable
 from copy import deepcopy
 
 import numpy as np
 import scipy.spatial
@@ -46,15 +47,15 @@
 def volume(simplex, ys=None):
     # Notice the parameter ys is there so you can use this volume method as
     # as loss function
     matrix = np.subtract(simplex[:-1], simplex[-1], dtype=float)
 
     # See https://www.jstor.org/stable/2315353
     dim = len(simplex) - 1
-    vol = np.abs(fast_det(matrix)) / np.math.factorial(dim)
+    vol = np.abs(fast_det(matrix)) / math.factorial(dim)
     return vol
 
 
 def orientation(simplex):
     matrix = np.subtract(simplex[:-1], simplex[-1])
     # See https://www.jstor.org/stable/2315353
     sign, _logdet = np.linalg.slogdet(matrix)
```

### Comparing `adaptive-1.2.0/adaptive/learner/sequence_learner.py` & `adaptive-1.3.0/adaptive/learner/sequence_learner.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/learner/triangulation.py` & `adaptive-1.3.0/adaptive/learner/triangulation.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/notebook_integration.py` & `adaptive-1.3.0/adaptive/notebook_integration.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/runner.py` & `adaptive-1.3.0/adaptive/runner.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/tests/algorithm_4.py` & `adaptive-1.3.0/adaptive/tests/algorithm_4.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/tests/test_average_learner.py` & `adaptive-1.3.0/adaptive/tests/test_average_learner.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/tests/test_average_learner1d.py` & `adaptive-1.3.0/adaptive/tests/test_average_learner1d.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/tests/test_balancing_learner.py` & `adaptive-1.3.0/adaptive/tests/test_balancing_learner.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/tests/test_cquad.py` & `adaptive-1.3.0/adaptive/tests/test_cquad.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/tests/test_learner1d.py` & `adaptive-1.3.0/adaptive/tests/test_learner1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,15 +395,15 @@
 
 
 def test_NaN_loss():
     # see https://github.com/python-adaptive/adaptive/issues/145
     def f(x):
         a = 0.01
         if random.random() < 0.2:
-            return np.NaN
+            return np.nan
         return x + a**2 / (a**2 + x**2)
 
     learner = Learner1D(f, bounds=(-1, 1))
     simple(learner, npoints_goal=100)
 
 
 def test_inf_loss_with_missing_bounds():
```

### Comparing `adaptive-1.2.0/adaptive/tests/test_learnernd.py` & `adaptive-1.3.0/adaptive/tests/test_learnernd.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/tests/test_learners.py` & `adaptive-1.3.0/adaptive/tests/test_learners.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,21 +26,14 @@
     Learner2D,
     LearnerND,
     SequenceLearner,
 )
 from adaptive.learner.learner1D import with_pandas
 from adaptive.runner import simple
 
-try:
-    from adaptive.learner.skopt_learner import SKOptLearner
-except (ModuleNotFoundError, ImportError):
-    # XXX: catch the ImportError because of https://github.com/scikit-optimize/scikit-optimize/issues/902
-    SKOptLearner = None  # type: ignore[assignment,misc]
-
-
 LOSS_FUNCTIONS = {
     Learner1D: (
         "loss_per_interval",
         (
             adaptive.learner.learner1D.default_loss,
             adaptive.learner.learner1D.uniform_loss,
             adaptive.learner.learner1D.curvature_loss_function(),
@@ -570,15 +563,14 @@
 
 @run_with(
     Learner1D,
     Learner2D,
     LearnerND,
     AverageLearner,
     AverageLearner1D,
-    maybe_skip(SKOptLearner),
     IntegratorLearner,
     SequenceLearner,
     with_all_loss_functions=False,
 )
 def test_saving(learner_type, f, learner_kwargs):
     f = generate_random_parametrization(f)
     learner = learner_type(f, **learner_kwargs)
@@ -603,15 +595,14 @@
 
 @run_with(
     Learner1D,
     Learner2D,
     LearnerND,
     AverageLearner,
     AverageLearner1D,
-    maybe_skip(SKOptLearner),
     IntegratorLearner,
     SequenceLearner,
     with_all_loss_functions=False,
 )
 def test_saving_of_balancing_learner(learner_type, f, learner_kwargs):
     f = generate_random_parametrization(f)
     learner = BalancingLearner([learner_type(f, **learner_kwargs)])
@@ -642,15 +633,14 @@
 
 @run_with(
     Learner1D,
     Learner2D,
     LearnerND,
     AverageLearner,
     AverageLearner1D,
-    maybe_skip(SKOptLearner),
     IntegratorLearner,
     with_all_loss_functions=False,
 )
 def test_saving_with_datasaver(learner_type, f, learner_kwargs):
     f = generate_random_parametrization(f)
     g = lambda x: {"y": f(x), "t": random.random()}  # noqa: E731
     arg_picker = operator.itemgetter("y")
```

### Comparing `adaptive-1.2.0/adaptive/tests/test_notebook_integration.py` & `adaptive-1.3.0/adaptive/tests/test_notebook_integration.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/tests/test_pickling.py` & `adaptive-1.3.0/adaptive/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/tests/test_runner.py` & `adaptive-1.3.0/adaptive/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/tests/test_sequence_learner.py` & `adaptive-1.3.0/adaptive/tests/test_sequence_learner.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/tests/test_triangulation.py` & `adaptive-1.3.0/adaptive/tests/test_triangulation.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/tests/unit/test_learnernd.py` & `adaptive-1.3.0/adaptive/tests/unit/test_learnernd.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/tests/unit/test_learnernd_integration.py` & `adaptive-1.3.0/adaptive/tests/unit/test_learnernd_integration.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/tests/unit/test_triangulation.py` & `adaptive-1.3.0/adaptive/tests/unit/test_triangulation.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive/utils.py` & `adaptive-1.3.0/adaptive/utils.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.2.0/adaptive.egg-info/PKG-INFO` & `adaptive-1.3.0/adaptive.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptive
-Version: 1.2.0
+Version: 1.3.0
 Summary: Parallel active learning of mathematical functions
 Maintainer: Adaptive authors
 License: BSD
 Project-URL: homepage, https://adaptive.readthedocs.io/
 Project-URL: documentation, https://adaptive.readthedocs.io/
 Project-URL: repository, https://github.com/python-adaptive/adaptive
 Classifier: Development Status :: 4 - Beta
@@ -25,16 +25,14 @@
 Requires-Dist: loky>=2.9
 Requires-Dist: typing_extensions; python_version < "3.10"
 Requires-Dist: versioningit
 Provides-Extra: other
 Requires-Dist: dill; extra == "other"
 Requires-Dist: distributed; extra == "other"
 Requires-Dist: ipyparallel>=6.2.5; extra == "other"
-Requires-Dist: scikit-optimize>=0.8.1; extra == "other"
-Requires-Dist: scikit-learn; extra == "other"
 Requires-Dist: wexpect; os_name == "nt" and extra == "other"
 Requires-Dist: pexpect; os_name != "nt" and extra == "other"
 Provides-Extra: notebook
 Requires-Dist: ipython; extra == "notebook"
 Requires-Dist: ipykernel>=4.8.0; extra == "notebook"
 Requires-Dist: jupyter_client>=5.2.2; extra == "notebook"
 Requires-Dist: holoviews>=1.9.1; extra == "notebook"
```

### Comparing `adaptive-1.2.0/adaptive.egg-info/SOURCES.txt` & `adaptive-1.3.0/adaptive.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,28 +23,26 @@
 adaptive/learner/data_saver.py
 adaptive/learner/integrator_coeffs.py
 adaptive/learner/integrator_learner.py
 adaptive/learner/learner1D.py
 adaptive/learner/learner2D.py
 adaptive/learner/learnerND.py
 adaptive/learner/sequence_learner.py
-adaptive/learner/skopt_learner.py
 adaptive/learner/triangulation.py
 adaptive/tests/__init__.py
 adaptive/tests/algorithm_4.py
 adaptive/tests/test_average_learner.py
 adaptive/tests/test_average_learner1d.py
 adaptive/tests/test_balancing_learner.py
 adaptive/tests/test_cquad.py
 adaptive/tests/test_learner1d.py
 adaptive/tests/test_learnernd.py
 adaptive/tests/test_learners.py
 adaptive/tests/test_notebook_integration.py
 adaptive/tests/test_pickling.py
 adaptive/tests/test_runner.py
 adaptive/tests/test_sequence_learner.py
-adaptive/tests/test_skopt_learner.py
 adaptive/tests/test_triangulation.py
 adaptive/tests/unit/__init__.py
 adaptive/tests/unit/test_learnernd.py
 adaptive/tests/unit/test_learnernd_integration.py
 adaptive/tests/unit/test_triangulation.py
```

### Comparing `adaptive-1.2.0/pyproject.toml` & `adaptive-1.3.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -28,24 +28,22 @@
     "versioningit",
 ]
 
 [project.optional-dependencies]
 other = [
     "dill",
     "distributed",
-    "ipyparallel>=6.2.5",                    # because of https://github.com/ipython/ipyparallel/issues/404
-    "scikit-optimize>=0.8.1",                # because of https://github.com/scikit-optimize/scikit-optimize/issues/931
-    "scikit-learn",
+    "ipyparallel>=6.2.5",       # because of https://github.com/ipython/ipyparallel/issues/404
     "wexpect; os_name == 'nt'",
     "pexpect; os_name != 'nt'",
 ]
 notebook = [
     "ipython",
-    "ipykernel>=4.8.0",                      # because https://github.com/ipython/ipykernel/issues/274 and https://github.com/ipython/ipykernel/issues/263
-    "jupyter_client>=5.2.2",                 # because https://github.com/jupyter/jupyter_client/pull/314
+    "ipykernel>=4.8.0",      # because https://github.com/ipython/ipykernel/issues/274 and https://github.com/ipython/ipykernel/issues/263
+    "jupyter_client>=5.2.2", # because https://github.com/jupyter/jupyter_client/pull/314
     "holoviews>=1.9.1",
     "ipywidgets",
     "bokeh",
     "pandas",
     "matplotlib",
     "plotly",
 ]
```

