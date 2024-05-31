# Comparing `tmp/flameai-1.0.6.tar.gz` & `tmp/flameai-1.0.7.tar.gz`

## Comparing `flameai-1.0.6.tar` & `flameai-1.0.7.tar`

### file list

```diff
@@ -1,29 +1,39 @@
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 flameai-1.0.6/.flake8
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 flameai-1.0.6/noxfile.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 flameai-1.0.6/.github/workflows/nox.yml
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 flameai-1.0.6/examples/eval_binary.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 flameai-1.0.6/examples/eval_regression.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 flameai-1.0.6/examples/hive_cli.sh
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 flameai-1.0.6/examples/simple.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 flameai-1.0.6/src/flameai/__init__.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 flameai-1.0.6/src/flameai/__main__.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 flameai-1.0.6/src/flameai/_env.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 flameai-1.0.6/src/flameai/cmd.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 flameai-1.0.6/src/flameai/hive.py
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 flameai-1.0.6/src/flameai/metrics.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 flameai-1.0.6/src/flameai/mining.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 flameai-1.0.6/src/flameai/plot.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 flameai-1.0.6/src/flameai/preprocessing.py
--rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 flameai-1.0.6/src/flameai/train.py
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 flameai-1.0.6/src/flameai/util.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 flameai-1.0.6/tests/test_cmd.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 flameai-1.0.6/tests/test_metrics.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 flameai-1.0.6/tests/test_mining.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 flameai-1.0.6/tests/test_plot.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 flameai-1.0.6/tests/test_preprocessing.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 flameai-1.0.6/tests/test_train.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 flameai-1.0.6/.gitignore
--rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 flameai-1.0.6/LICENSE
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 flameai-1.0.6/README.md
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 flameai-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 flameai-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 flameai-1.0.7/.flake8
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 flameai-1.0.7/CHANGELOG.rst
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 flameai-1.0.7/noxfile.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 flameai-1.0.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 flameai-1.0.7/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 flameai-1.0.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 flameai-1.0.7/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    25316 2020-02-02 00:00:00.000000 flameai-1.0.7/docs/_static/flame.jpeg
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 flameai-1.0.7/examples/confusion_matrix.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 flameai-1.0.7/examples/dataloader.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 flameai-1.0.7/examples/eval_binary.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 flameai-1.0.7/examples/eval_regression.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 flameai-1.0.7/examples/gen_abspath.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 flameai-1.0.7/examples/hive_cli.sh
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 flameai-1.0.7/examples/roc_curve.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 flameai-1.0.7/examples/set_logger.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 flameai-1.0.7/examples/simple.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 flameai-1.0.7/src/flameai/__init__.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 flameai-1.0.7/src/flameai/__main__.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 flameai-1.0.7/src/flameai/_env.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 flameai-1.0.7/src/flameai/cmd.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 flameai-1.0.7/src/flameai/hive.py
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 flameai-1.0.7/src/flameai/metrics.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 flameai-1.0.7/src/flameai/mining.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 flameai-1.0.7/src/flameai/plot.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 flameai-1.0.7/src/flameai/preprocessing.py
+-rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 flameai-1.0.7/src/flameai/train.py
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 flameai-1.0.7/src/flameai/util.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 flameai-1.0.7/tests/test_cmd.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 flameai-1.0.7/tests/test_metrics.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 flameai-1.0.7/tests/test_mining.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 flameai-1.0.7/tests/test_plot.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 flameai-1.0.7/tests/test_preprocessing.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 flameai-1.0.7/tests/test_train.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 flameai-1.0.7/.gitignore
+-rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 flameai-1.0.7/LICENSE
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 flameai-1.0.7/README.md
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 flameai-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 flameai-1.0.7/PKG-INFO
```

### Comparing `flameai-1.0.6/.github/workflows/nox.yml` & `flameai-1.0.7/.github/workflows/ci.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Run nox tests
+name: CI
 
 on:
   push:
     branches:
       - main
   pull_request:
     branches:
```

### Comparing `flameai-1.0.6/examples/eval_binary.py` & `flameai-1.0.7/examples/eval_binary.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.6/src/flameai/_env.py` & `flameai-1.0.7/src/flameai/_env.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.6/src/flameai/metrics.py` & `flameai-1.0.7/src/flameai/metrics.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.6/src/flameai/plot.py` & `flameai-1.0.7/src/flameai/plot.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.6/src/flameai/preprocessing.py` & `flameai-1.0.7/src/flameai/preprocessing.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.6/src/flameai/train.py` & `flameai-1.0.7/src/flameai/train.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.6/src/flameai/util.py` & `flameai-1.0.7/src/flameai/util.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.6/tests/test_metrics.py` & `flameai-1.0.7/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.6/tests/test_plot.py` & `flameai-1.0.7/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.6/tests/test_preprocessing.py` & `flameai-1.0.7/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.6/tests/test_train.py` & `flameai-1.0.7/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.6/LICENSE` & `flameai-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `flameai-1.0.6/pyproject.toml` & `flameai-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "flameai"
-version = "1.0.6"
+version = "1.0.7"
 description = "Python Deep Learning Toolkit."
 readme = "README.md"
 keywords = [
   "deep learning",
   "flameai",
 ]
 license = { text = "Apache-2.0" }
```

### Comparing `flameai-1.0.6/PKG-INFO` & `flameai-1.0.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: flameai
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python Deep Learning Toolkit.
 Project-URL: repository, https://github.com/luochang212/flameai
 Project-URL: bug-tracker, https://github.com/luochang212/flameai/issues
 Project-URL: documentation, https://luochang212.github.io/posts/flameai
 Author: luochang
 Author-email: luochang212@gmail.com
 License: Apache-2.0
@@ -30,16 +30,27 @@
 Requires-Dist: optuna>=3.6.1
 Requires-Dist: pandas>=2.0.3
 Requires-Dist: scikit-learn>=1.3.2
 Requires-Dist: scipy>=1.10.1
 Requires-Dist: seaborn>=0.13.2
 Description-Content-Type: text/markdown
 
+<!-- <p align="center">
+<img src="https://github.com/luochang212/flameai/raw/main/docs/_static/flame.jpeg" alt="logo" width=88%>
+</p> -->
+
+
 # 🔥 FlameAI
 
+[![License](https://img.shields.io/github/license/luochang212/flameai)](https://github.com/luochang212/flameai)
+[![PyPI](https://img.shields.io/pypi/v/flameai.svg?logo=python)](https://pypi.python.org/pypi/flameai)
+[![GitHub](https://img.shields.io/github/v/release/luochang212/flameai?logo=github&sort=semver)](https://github.com/luochang212/flameai)
+[![CI](https://github.com/luochang212/flameai/workflows/CI/badge.svg)](https://github.com/luochang212/flameai/actions?query=workflow:CI)
+[![Downloads](https://static.pepy.tech/personalized-badge/flameai?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads)](https://pepy.tech/project/flameai)
+
 Python Deep Learning Toolkit.
 
 ## Installation
 
 Install the package: 
 
 ```bash
@@ -81,14 +92,16 @@
 False Positive (FP): 2
 False Negative (FN): 1
 confusion matrix:
 [[4 2]
  [1 3]]
 ```
 
+Other examples: [examples](/examples/)
+
 ## Test Locally
 
 Create a conda environment:
 
 ```bash
 # Create env
 mamba create -n python_3_10 python=3.10
```

