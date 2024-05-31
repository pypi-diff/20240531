# Comparing `tmp/sentiment_analysis_package-0.5.0.tar.gz` & `tmp/sentiment_analysis_package-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentiment_analysis_package-0.5.0.tar", last modified: Fri May 31 07:38:44 2024, max compression
+gzip compressed data, was "sentiment_analysis_package-0.6.0.tar", last modified: Fri May 31 07:47:37 2024, max compression
```

## Comparing `sentiment_analysis_package-0.5.0.tar` & `sentiment_analysis_package-0.6.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 07:38:44.203962 sentiment_analysis_package-0.5.0/
--rw-rw-rw-   0        0        0      305 2024-05-31 05:54:40.000000 sentiment_analysis_package-0.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0      243 2024-05-31 07:38:44.202965 sentiment_analysis_package-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0        2 2024-05-24 11:24:36.000000 sentiment_analysis_package-0.5.0/README.md
--rw-rw-rw-   0        0        0       93 2024-05-24 11:27:42.000000 sentiment_analysis_package-0.5.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-31 07:38:44.154236 sentiment_analysis_package-0.5.0/requirements/
--rw-rw-rw-   0        0        0      118 2024-05-31 07:09:14.000000 sentiment_analysis_package-0.5.0/requirements/requirements.txt
--rw-rw-rw-   0        0        0  8080721 2024-05-31 07:34:07.000000 sentiment_analysis_package-0.5.0/sentiment_analysis_model_0.5.0.pkl
-drwxrwxrwx   0        0        0        0 2024-05-31 07:38:44.200963 sentiment_analysis_package-0.5.0/sentiment_analysis_package.egg-info/
--rw-rw-rw-   0        0        0      243 2024-05-31 07:38:44.000000 sentiment_analysis_package-0.5.0/sentiment_analysis_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      758 2024-05-31 07:38:44.000000 sentiment_analysis_package-0.5.0/sentiment_analysis_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 07:38:44.000000 sentiment_analysis_package-0.5.0/sentiment_analysis_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-31 07:38:44.000000 sentiment_analysis_package-0.5.0/sentiment_analysis_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-31 07:38:44.000000 sentiment_analysis_package-0.5.0/sentiment_analysis_package.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-31 07:38:44.187964 sentiment_analysis_package-0.5.0/sentiment_model/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:26.000000 sentiment_analysis_package-0.5.0/sentiment_model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:38:44.189962 sentiment_analysis_package-0.5.0/sentiment_model/config/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:34.000000 sentiment_analysis_package-0.5.0/sentiment_model/config/__init__.py
--rw-rw-rw-   0        0        0      743 2024-05-31 07:22:22.000000 sentiment_analysis_package-0.5.0/sentiment_model/config/core.py
--rw-rw-rw-   0        0        0      225 2024-05-31 07:22:53.000000 sentiment_analysis_package-0.5.0/sentiment_model/config.yml
--rw-rw-rw-   0        0        0      419 2024-05-24 15:14:18.000000 sentiment_analysis_package-0.5.0/sentiment_model/pipeline.py
--rw-rw-rw-   0        0        0      499 2024-05-31 07:38:25.000000 sentiment_analysis_package-0.5.0/sentiment_model/predict.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:38:44.193964 sentiment_analysis_package-0.5.0/sentiment_model/processing/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:48.000000 sentiment_analysis_package-0.5.0/sentiment_model/processing/__init__.py
--rw-rw-rw-   0        0        0      582 2024-05-31 02:39:25.000000 sentiment_analysis_package-0.5.0/sentiment_model/processing/features.py
--rw-rw-rw-   0        0        0      355 2024-05-24 11:22:44.000000 sentiment_analysis_package-0.5.0/sentiment_model/processing/validation.py
--rw-rw-rw-   0        0        0     1575 2024-05-31 07:22:26.000000 sentiment_analysis_package-0.5.0/sentiment_model/train_pipeline.py
--rw-rw-rw-   0        0        0       42 2024-05-31 07:38:44.203962 sentiment_analysis_package-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0      429 2024-05-31 07:22:49.000000 sentiment_analysis_package-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:38:44.198967 sentiment_analysis_package-0.5.0/tests/
--rw-rw-rw-   0        0        0      154 2024-05-24 11:23:44.000000 sentiment_analysis_package-0.5.0/tests/test_pipeline.py
--rw-rw-rw-   0        0        0      263 2024-05-31 03:05:48.000000 sentiment_analysis_package-0.5.0/tests/test_predict.py
--rw-rw-rw-   0        0        0      244 2024-05-31 02:07:23.000000 sentiment_analysis_package-0.5.0/tests/test_processing.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:47:37.235235 sentiment_analysis_package-0.6.0/
+-rw-rw-rw-   0        0        0      349 2024-05-31 07:46:57.000000 sentiment_analysis_package-0.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      243 2024-05-31 07:47:37.233327 sentiment_analysis_package-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0        2 2024-05-24 11:24:36.000000 sentiment_analysis_package-0.6.0/README.md
+-rw-rw-rw-   0        0        0       93 2024-05-24 11:27:42.000000 sentiment_analysis_package-0.6.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-31 07:47:37.198235 sentiment_analysis_package-0.6.0/requirements/
+-rw-rw-rw-   0        0        0      118 2024-05-31 07:09:14.000000 sentiment_analysis_package-0.6.0/requirements/requirements.txt
+-rw-rw-rw-   0        0        0  8080721 2024-05-31 07:34:07.000000 sentiment_analysis_package-0.6.0/sentiment_analysis_model_0.6.0.pkl
+drwxrwxrwx   0        0        0        0 2024-05-31 07:47:37.219262 sentiment_analysis_package-0.6.0/sentiment_analysis_package.egg-info/
+-rw-rw-rw-   0        0        0      243 2024-05-31 07:47:37.000000 sentiment_analysis_package-0.6.0/sentiment_analysis_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      758 2024-05-31 07:47:37.000000 sentiment_analysis_package-0.6.0/sentiment_analysis_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 07:47:37.000000 sentiment_analysis_package-0.6.0/sentiment_analysis_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-31 07:47:37.000000 sentiment_analysis_package-0.6.0/sentiment_analysis_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-31 07:47:37.000000 sentiment_analysis_package-0.6.0/sentiment_analysis_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 07:47:37.210235 sentiment_analysis_package-0.6.0/sentiment_model/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:26.000000 sentiment_analysis_package-0.6.0/sentiment_model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:47:37.211235 sentiment_analysis_package-0.6.0/sentiment_model/config/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:34.000000 sentiment_analysis_package-0.6.0/sentiment_model/config/__init__.py
+-rw-rw-rw-   0        0        0      743 2024-05-31 07:22:22.000000 sentiment_analysis_package-0.6.0/sentiment_model/config/core.py
+-rw-rw-rw-   0        0        0      225 2024-05-31 07:22:53.000000 sentiment_analysis_package-0.6.0/sentiment_model/config.yml
+-rw-rw-rw-   0        0        0      419 2024-05-24 15:14:18.000000 sentiment_analysis_package-0.6.0/sentiment_model/pipeline.py
+-rw-rw-rw-   0        0        0      499 2024-05-31 07:38:25.000000 sentiment_analysis_package-0.6.0/sentiment_model/predict.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:47:37.215263 sentiment_analysis_package-0.6.0/sentiment_model/processing/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:48.000000 sentiment_analysis_package-0.6.0/sentiment_model/processing/__init__.py
+-rw-rw-rw-   0        0        0      582 2024-05-31 02:39:25.000000 sentiment_analysis_package-0.6.0/sentiment_model/processing/features.py
+-rw-rw-rw-   0        0        0      355 2024-05-24 11:22:44.000000 sentiment_analysis_package-0.6.0/sentiment_model/processing/validation.py
+-rw-rw-rw-   0        0        0     1575 2024-05-31 07:22:26.000000 sentiment_analysis_package-0.6.0/sentiment_model/train_pipeline.py
+-rw-rw-rw-   0        0        0       42 2024-05-31 07:47:37.235235 sentiment_analysis_package-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      429 2024-05-31 07:47:10.000000 sentiment_analysis_package-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:47:37.218272 sentiment_analysis_package-0.6.0/tests/
+-rw-rw-rw-   0        0        0      154 2024-05-24 11:23:44.000000 sentiment_analysis_package-0.6.0/tests/test_pipeline.py
+-rw-rw-rw-   0        0        0      263 2024-05-31 03:05:48.000000 sentiment_analysis_package-0.6.0/tests/test_predict.py
+-rw-rw-rw-   0        0        0      244 2024-05-31 02:07:23.000000 sentiment_analysis_package-0.6.0/tests/test_processing.py
```

### Comparing `sentiment_analysis_package-0.5.0/sentiment_analysis_model_0.5.0.pkl` & `sentiment_analysis_package-0.6.0/sentiment_analysis_model_0.6.0.pkl`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_package-0.5.0/sentiment_analysis_package.egg-info/SOURCES.txt` & `sentiment_analysis_package-0.6.0/sentiment_analysis_package.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 MANIFEST.in
 README.md
 pyproject.toml
-sentiment_analysis_model_0.5.0.pkl
+sentiment_analysis_model_0.6.0.pkl
 setup.py
 requirements/requirements.txt
 sentiment_analysis_package.egg-info/PKG-INFO
 sentiment_analysis_package.egg-info/SOURCES.txt
 sentiment_analysis_package.egg-info/dependency_links.txt
 sentiment_analysis_package.egg-info/requires.txt
 sentiment_analysis_package.egg-info/top_level.txt
```

### Comparing `sentiment_analysis_package-0.5.0/sentiment_model/config/core.py` & `sentiment_analysis_package-0.6.0/sentiment_model/config/core.py`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_package-0.5.0/sentiment_model/processing/features.py` & `sentiment_analysis_package-0.6.0/sentiment_model/processing/features.py`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_package-0.5.0/sentiment_model/train_pipeline.py` & `sentiment_analysis_package-0.6.0/sentiment_model/train_pipeline.py`

 * *Files identical despite different names*

