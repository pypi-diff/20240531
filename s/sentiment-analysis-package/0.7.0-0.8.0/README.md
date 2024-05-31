# Comparing `tmp/sentiment_analysis_package-0.7.0.tar.gz` & `tmp/sentiment_analysis_package-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentiment_analysis_package-0.7.0.tar", last modified: Fri May 31 07:51:10 2024, max compression
+gzip compressed data, was "sentiment_analysis_package-0.8.0.tar", last modified: Fri May 31 08:02:50 2024, max compression
```

## Comparing `sentiment_analysis_package-0.7.0.tar` & `sentiment_analysis_package-0.8.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 07:51:10.990557 sentiment_analysis_package-0.7.0/
--rw-rw-rw-   0        0        0      336 2024-05-31 07:49:51.000000 sentiment_analysis_package-0.7.0/MANIFEST.in
--rw-rw-rw-   0        0        0      243 2024-05-31 07:51:10.989559 sentiment_analysis_package-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0        2 2024-05-24 11:24:36.000000 sentiment_analysis_package-0.7.0/README.md
--rw-rw-rw-   0        0        0       93 2024-05-24 11:27:42.000000 sentiment_analysis_package-0.7.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-31 07:51:10.958559 sentiment_analysis_package-0.7.0/requirements/
--rw-rw-rw-   0        0        0      118 2024-05-31 07:09:14.000000 sentiment_analysis_package-0.7.0/requirements/requirements.txt
--rw-rw-rw-   0        0        0  8080721 2024-05-31 07:34:07.000000 sentiment_analysis_package-0.7.0/sentiment_analysis_model_0.7.0.pkl
-drwxrwxrwx   0        0        0        0 2024-05-31 07:51:10.987559 sentiment_analysis_package-0.7.0/sentiment_analysis_package.egg-info/
--rw-rw-rw-   0        0        0      243 2024-05-31 07:51:10.000000 sentiment_analysis_package-0.7.0/sentiment_analysis_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      758 2024-05-31 07:51:10.000000 sentiment_analysis_package-0.7.0/sentiment_analysis_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 07:51:10.000000 sentiment_analysis_package-0.7.0/sentiment_analysis_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-31 07:51:10.000000 sentiment_analysis_package-0.7.0/sentiment_analysis_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-31 07:51:10.000000 sentiment_analysis_package-0.7.0/sentiment_analysis_package.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-31 07:51:10.971557 sentiment_analysis_package-0.7.0/sentiment_model/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:26.000000 sentiment_analysis_package-0.7.0/sentiment_model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:51:10.973585 sentiment_analysis_package-0.7.0/sentiment_model/config/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:34.000000 sentiment_analysis_package-0.7.0/sentiment_model/config/__init__.py
--rw-rw-rw-   0        0        0      743 2024-05-31 07:22:22.000000 sentiment_analysis_package-0.7.0/sentiment_model/config/core.py
--rw-rw-rw-   0        0        0      225 2024-05-31 07:50:57.000000 sentiment_analysis_package-0.7.0/sentiment_model/config.yml
--rw-rw-rw-   0        0        0      419 2024-05-24 15:14:18.000000 sentiment_analysis_package-0.7.0/sentiment_model/pipeline.py
--rw-rw-rw-   0        0        0      499 2024-05-31 07:38:25.000000 sentiment_analysis_package-0.7.0/sentiment_model/predict.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:51:10.977557 sentiment_analysis_package-0.7.0/sentiment_model/processing/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:48.000000 sentiment_analysis_package-0.7.0/sentiment_model/processing/__init__.py
--rw-rw-rw-   0        0        0      582 2024-05-31 02:39:25.000000 sentiment_analysis_package-0.7.0/sentiment_model/processing/features.py
--rw-rw-rw-   0        0        0      355 2024-05-24 11:22:44.000000 sentiment_analysis_package-0.7.0/sentiment_model/processing/validation.py
--rw-rw-rw-   0        0        0     1575 2024-05-31 07:22:26.000000 sentiment_analysis_package-0.7.0/sentiment_model/train_pipeline.py
--rw-rw-rw-   0        0        0       42 2024-05-31 07:51:10.991558 sentiment_analysis_package-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0      429 2024-05-31 07:50:38.000000 sentiment_analysis_package-0.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:51:10.982560 sentiment_analysis_package-0.7.0/tests/
--rw-rw-rw-   0        0        0      154 2024-05-24 11:23:44.000000 sentiment_analysis_package-0.7.0/tests/test_pipeline.py
--rw-rw-rw-   0        0        0      263 2024-05-31 03:05:48.000000 sentiment_analysis_package-0.7.0/tests/test_predict.py
--rw-rw-rw-   0        0        0      244 2024-05-31 02:07:23.000000 sentiment_analysis_package-0.7.0/tests/test_processing.py
+drwxrwxrwx   0        0        0        0 2024-05-31 08:02:50.222191 sentiment_analysis_package-0.8.0/
+-rw-rw-rw-   0        0        0      391 2024-05-31 07:59:51.000000 sentiment_analysis_package-0.8.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      243 2024-05-31 08:02:50.221188 sentiment_analysis_package-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0        2 2024-05-24 11:24:36.000000 sentiment_analysis_package-0.8.0/README.md
+-rw-rw-rw-   0        0        0       93 2024-05-24 11:27:42.000000 sentiment_analysis_package-0.8.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-31 08:02:50.183187 sentiment_analysis_package-0.8.0/requirements/
+-rw-rw-rw-   0        0        0      118 2024-05-31 07:09:14.000000 sentiment_analysis_package-0.8.0/requirements/requirements.txt
+-rw-rw-rw-   0        0        0  8080721 2024-05-31 07:34:07.000000 sentiment_analysis_package-0.8.0/sentiment_analysis_model_0.8.0.pkl
+drwxrwxrwx   0        0        0        0 2024-05-31 08:02:50.220193 sentiment_analysis_package-0.8.0/sentiment_analysis_package.egg-info/
+-rw-rw-rw-   0        0        0      243 2024-05-31 08:02:50.000000 sentiment_analysis_package-0.8.0/sentiment_analysis_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      804 2024-05-31 08:02:50.000000 sentiment_analysis_package-0.8.0/sentiment_analysis_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 08:02:50.000000 sentiment_analysis_package-0.8.0/sentiment_analysis_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-31 08:02:50.000000 sentiment_analysis_package-0.8.0/sentiment_analysis_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-31 08:02:50.000000 sentiment_analysis_package-0.8.0/sentiment_analysis_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 08:02:50.196193 sentiment_analysis_package-0.8.0/sentiment_model/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:26.000000 sentiment_analysis_package-0.8.0/sentiment_model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 08:02:50.198188 sentiment_analysis_package-0.8.0/sentiment_model/config/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:34.000000 sentiment_analysis_package-0.8.0/sentiment_model/config/__init__.py
+-rw-rw-rw-   0        0        0      743 2024-05-31 07:22:22.000000 sentiment_analysis_package-0.8.0/sentiment_model/config/core.py
+-rw-rw-rw-   0        0        0      227 2024-05-31 07:57:54.000000 sentiment_analysis_package-0.8.0/sentiment_model/config.yml
+drwxrwxrwx   0        0        0        0 2024-05-31 08:02:50.200190 sentiment_analysis_package-0.8.0/sentiment_model/datasets/
+-rw-rw-rw-   0        0        0 10325088 2021-08-08 23:52:12.000000 sentiment_analysis_package-0.8.0/sentiment_model/datasets/twitter_training.csv
+-rw-rw-rw-   0        0        0      419 2024-05-24 15:14:18.000000 sentiment_analysis_package-0.8.0/sentiment_model/pipeline.py
+-rw-rw-rw-   0        0        0      499 2024-05-31 07:38:25.000000 sentiment_analysis_package-0.8.0/sentiment_model/predict.py
+drwxrwxrwx   0        0        0        0 2024-05-31 08:02:50.214191 sentiment_analysis_package-0.8.0/sentiment_model/processing/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:48.000000 sentiment_analysis_package-0.8.0/sentiment_model/processing/__init__.py
+-rw-rw-rw-   0        0        0      582 2024-05-31 02:39:25.000000 sentiment_analysis_package-0.8.0/sentiment_model/processing/features.py
+-rw-rw-rw-   0        0        0      355 2024-05-24 11:22:44.000000 sentiment_analysis_package-0.8.0/sentiment_model/processing/validation.py
+-rw-rw-rw-   0        0        0     1575 2024-05-31 07:22:26.000000 sentiment_analysis_package-0.8.0/sentiment_model/train_pipeline.py
+-rw-rw-rw-   0        0        0       42 2024-05-31 08:02:50.222191 sentiment_analysis_package-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0      471 2024-05-31 08:01:50.000000 sentiment_analysis_package-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 08:02:50.218190 sentiment_analysis_package-0.8.0/tests/
+-rw-rw-rw-   0        0        0      154 2024-05-24 11:23:44.000000 sentiment_analysis_package-0.8.0/tests/test_pipeline.py
+-rw-rw-rw-   0        0        0      263 2024-05-31 03:05:48.000000 sentiment_analysis_package-0.8.0/tests/test_predict.py
+-rw-rw-rw-   0        0        0      244 2024-05-31 02:07:23.000000 sentiment_analysis_package-0.8.0/tests/test_processing.py
```

### Comparing `sentiment_analysis_package-0.7.0/sentiment_analysis_model_0.7.0.pkl` & `sentiment_analysis_package-0.8.0/sentiment_analysis_model_0.8.0.pkl`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_package-0.7.0/sentiment_analysis_package.egg-info/SOURCES.txt` & `sentiment_analysis_package-0.8.0/sentiment_analysis_package.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 MANIFEST.in
 README.md
 pyproject.toml
-sentiment_analysis_model_0.7.0.pkl
+sentiment_analysis_model_0.8.0.pkl
 setup.py
 requirements/requirements.txt
 sentiment_analysis_package.egg-info/PKG-INFO
 sentiment_analysis_package.egg-info/SOURCES.txt
 sentiment_analysis_package.egg-info/dependency_links.txt
 sentiment_analysis_package.egg-info/requires.txt
 sentiment_analysis_package.egg-info/top_level.txt
 sentiment_model/__init__.py
 sentiment_model/config.yml
 sentiment_model/pipeline.py
 sentiment_model/predict.py
 sentiment_model/train_pipeline.py
 sentiment_model/config/__init__.py
 sentiment_model/config/core.py
+sentiment_model/datasets/twitter_training.csv
 sentiment_model/processing/__init__.py
 sentiment_model/processing/features.py
 sentiment_model/processing/validation.py
 tests/test_pipeline.py
 tests/test_predict.py
 tests/test_processing.py
```

### Comparing `sentiment_analysis_package-0.7.0/sentiment_model/config/core.py` & `sentiment_analysis_package-0.8.0/sentiment_model/config/core.py`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_package-0.7.0/sentiment_model/processing/features.py` & `sentiment_analysis_package-0.8.0/sentiment_model/processing/features.py`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_package-0.7.0/sentiment_model/train_pipeline.py` & `sentiment_analysis_package-0.8.0/sentiment_model/train_pipeline.py`

 * *Files identical despite different names*

