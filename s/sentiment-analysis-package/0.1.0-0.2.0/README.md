# Comparing `tmp/sentiment_analysis_package-0.1.0.tar.gz` & `tmp/sentiment_analysis_package-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentiment_analysis_package-0.1.0.tar", last modified: Fri May 31 03:26:22 2024, max compression
+gzip compressed data, was "sentiment_analysis_package-0.2.0.tar", last modified: Fri May 31 05:09:14 2024, max compression
```

## Comparing `sentiment_analysis_package-0.1.0.tar` & `sentiment_analysis_package-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 03:26:22.957329 sentiment_analysis_package-0.1.0/
--rw-rw-rw-   0        0        0       81 2024-05-24 11:27:30.000000 sentiment_analysis_package-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      243 2024-05-31 03:26:22.957329 sentiment_analysis_package-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        2 2024-05-24 11:24:36.000000 sentiment_analysis_package-0.1.0/README.md
--rw-rw-rw-   0        0        0       93 2024-05-24 11:27:42.000000 sentiment_analysis_package-0.1.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-31 03:26:22.956303 sentiment_analysis_package-0.1.0/sentiment_analysis_package.egg-info/
--rw-rw-rw-   0        0        0      243 2024-05-31 03:26:22.000000 sentiment_analysis_package-0.1.0/sentiment_analysis_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      703 2024-05-31 03:26:22.000000 sentiment_analysis_package-0.1.0/sentiment_analysis_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 03:26:22.000000 sentiment_analysis_package-0.1.0/sentiment_analysis_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-31 03:26:22.000000 sentiment_analysis_package-0.1.0/sentiment_analysis_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-31 03:26:22.000000 sentiment_analysis_package-0.1.0/sentiment_analysis_package.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-31 03:26:22.946307 sentiment_analysis_package-0.1.0/sentiment_model/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:26.000000 sentiment_analysis_package-0.1.0/sentiment_model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 03:26:22.949302 sentiment_analysis_package-0.1.0/sentiment_model/config/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:34.000000 sentiment_analysis_package-0.1.0/sentiment_model/config/__init__.py
--rw-rw-rw-   0        0        0      772 2024-05-24 14:24:34.000000 sentiment_analysis_package-0.1.0/sentiment_model/config/core.py
--rw-rw-rw-   0        0        0      225 2024-05-31 02:23:22.000000 sentiment_analysis_package-0.1.0/sentiment_model/config.yml
--rw-rw-rw-   0        0        0      419 2024-05-24 15:14:18.000000 sentiment_analysis_package-0.1.0/sentiment_model/pipeline.py
--rw-rw-rw-   0        0        0      503 2024-05-31 03:07:55.000000 sentiment_analysis_package-0.1.0/sentiment_model/predict.py
-drwxrwxrwx   0        0        0        0 2024-05-31 03:26:22.951343 sentiment_analysis_package-0.1.0/sentiment_model/processing/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:48.000000 sentiment_analysis_package-0.1.0/sentiment_model/processing/__init__.py
--rw-rw-rw-   0        0        0      582 2024-05-31 02:39:25.000000 sentiment_analysis_package-0.1.0/sentiment_model/processing/features.py
--rw-rw-rw-   0        0        0      355 2024-05-24 11:22:44.000000 sentiment_analysis_package-0.1.0/sentiment_model/processing/validation.py
--rw-rw-rw-   0        0        0     1555 2024-05-31 02:34:37.000000 sentiment_analysis_package-0.1.0/sentiment_model/train_pipeline.py
--rw-rw-rw-   0        0        0       86 2024-05-31 03:26:22.958304 sentiment_analysis_package-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      414 2024-05-31 03:23:43.000000 sentiment_analysis_package-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-31 03:26:22.955306 sentiment_analysis_package-0.1.0/tests/
--rw-rw-rw-   0        0        0      154 2024-05-24 11:23:44.000000 sentiment_analysis_package-0.1.0/tests/test_pipeline.py
--rw-rw-rw-   0        0        0      263 2024-05-31 03:05:48.000000 sentiment_analysis_package-0.1.0/tests/test_predict.py
--rw-rw-rw-   0        0        0      244 2024-05-31 02:07:23.000000 sentiment_analysis_package-0.1.0/tests/test_processing.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:09:14.752108 sentiment_analysis_package-0.2.0/
+-rw-rw-rw-   0        0        0      323 2024-05-31 04:50:04.000000 sentiment_analysis_package-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      243 2024-05-31 05:09:14.751108 sentiment_analysis_package-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        2 2024-05-24 11:24:36.000000 sentiment_analysis_package-0.2.0/README.md
+-rw-rw-rw-   0        0        0       93 2024-05-24 11:27:42.000000 sentiment_analysis_package-0.2.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-31 05:09:14.729109 sentiment_analysis_package-0.2.0/requirements/
+-rw-rw-rw-   0        0        0      110 2024-05-24 14:45:58.000000 sentiment_analysis_package-0.2.0/requirements/requirements.txt
+-rw-rw-rw-   0        0        0  8080721 2024-05-31 05:07:25.000000 sentiment_analysis_package-0.2.0/sentiment_analysis_model_0.2.0.pkl
+drwxrwxrwx   0        0        0        0 2024-05-31 05:09:14.750108 sentiment_analysis_package-0.2.0/sentiment_analysis_package.egg-info/
+-rw-rw-rw-   0        0        0      243 2024-05-31 05:09:14.000000 sentiment_analysis_package-0.2.0/sentiment_analysis_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      758 2024-05-31 05:09:14.000000 sentiment_analysis_package-0.2.0/sentiment_analysis_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 05:09:14.000000 sentiment_analysis_package-0.2.0/sentiment_analysis_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-31 05:09:14.000000 sentiment_analysis_package-0.2.0/sentiment_analysis_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-31 05:09:14.000000 sentiment_analysis_package-0.2.0/sentiment_analysis_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 05:09:14.740108 sentiment_analysis_package-0.2.0/sentiment_model/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:26.000000 sentiment_analysis_package-0.2.0/sentiment_model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:09:14.743108 sentiment_analysis_package-0.2.0/sentiment_model/config/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:34.000000 sentiment_analysis_package-0.2.0/sentiment_model/config/__init__.py
+-rw-rw-rw-   0        0        0      772 2024-05-24 14:24:34.000000 sentiment_analysis_package-0.2.0/sentiment_model/config/core.py
+-rw-rw-rw-   0        0        0      225 2024-05-31 04:50:52.000000 sentiment_analysis_package-0.2.0/sentiment_model/config.yml
+-rw-rw-rw-   0        0        0      419 2024-05-24 15:14:18.000000 sentiment_analysis_package-0.2.0/sentiment_model/pipeline.py
+-rw-rw-rw-   0        0        0      503 2024-05-31 03:07:55.000000 sentiment_analysis_package-0.2.0/sentiment_model/predict.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:09:14.746107 sentiment_analysis_package-0.2.0/sentiment_model/processing/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:48.000000 sentiment_analysis_package-0.2.0/sentiment_model/processing/__init__.py
+-rw-rw-rw-   0        0        0      582 2024-05-31 02:39:25.000000 sentiment_analysis_package-0.2.0/sentiment_model/processing/features.py
+-rw-rw-rw-   0        0        0      355 2024-05-24 11:22:44.000000 sentiment_analysis_package-0.2.0/sentiment_model/processing/validation.py
+-rw-rw-rw-   0        0        0     1555 2024-05-31 02:34:37.000000 sentiment_analysis_package-0.2.0/sentiment_model/train_pipeline.py
+-rw-rw-rw-   0        0        0       42 2024-05-31 05:09:14.752108 sentiment_analysis_package-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      414 2024-05-31 04:50:58.000000 sentiment_analysis_package-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:09:14.749108 sentiment_analysis_package-0.2.0/tests/
+-rw-rw-rw-   0        0        0      154 2024-05-24 11:23:44.000000 sentiment_analysis_package-0.2.0/tests/test_pipeline.py
+-rw-rw-rw-   0        0        0      263 2024-05-31 03:05:48.000000 sentiment_analysis_package-0.2.0/tests/test_predict.py
+-rw-rw-rw-   0        0        0      244 2024-05-31 02:07:23.000000 sentiment_analysis_package-0.2.0/tests/test_processing.py
```

### Comparing `sentiment_analysis_package-0.1.0/sentiment_analysis_package.egg-info/SOURCES.txt` & `sentiment_analysis_package-0.2.0/sentiment_analysis_package.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
+sentiment_analysis_model_0.2.0.pkl
 setup.py
+requirements/requirements.txt
 sentiment_analysis_package.egg-info/PKG-INFO
 sentiment_analysis_package.egg-info/SOURCES.txt
 sentiment_analysis_package.egg-info/dependency_links.txt
 sentiment_analysis_package.egg-info/requires.txt
 sentiment_analysis_package.egg-info/top_level.txt
 sentiment_model/__init__.py
 sentiment_model/config.yml
```

### Comparing `sentiment_analysis_package-0.1.0/sentiment_model/config/core.py` & `sentiment_analysis_package-0.2.0/sentiment_model/config/core.py`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_package-0.1.0/sentiment_model/processing/features.py` & `sentiment_analysis_package-0.2.0/sentiment_model/processing/features.py`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_package-0.1.0/sentiment_model/train_pipeline.py` & `sentiment_analysis_package-0.2.0/sentiment_model/train_pipeline.py`

 * *Files identical despite different names*

