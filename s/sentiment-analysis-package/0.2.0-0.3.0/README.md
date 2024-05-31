# Comparing `tmp/sentiment_analysis_package-0.2.0.tar.gz` & `tmp/sentiment_analysis_package-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentiment_analysis_package-0.2.0.tar", last modified: Fri May 31 05:09:14 2024, max compression
+gzip compressed data, was "sentiment_analysis_package-0.3.0.tar", last modified: Fri May 31 05:39:26 2024, max compression
```

## Comparing `sentiment_analysis_package-0.2.0.tar` & `sentiment_analysis_package-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 05:09:14.752108 sentiment_analysis_package-0.2.0/
--rw-rw-rw-   0        0        0      323 2024-05-31 04:50:04.000000 sentiment_analysis_package-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      243 2024-05-31 05:09:14.751108 sentiment_analysis_package-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0        2 2024-05-24 11:24:36.000000 sentiment_analysis_package-0.2.0/README.md
--rw-rw-rw-   0        0        0       93 2024-05-24 11:27:42.000000 sentiment_analysis_package-0.2.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-31 05:09:14.729109 sentiment_analysis_package-0.2.0/requirements/
--rw-rw-rw-   0        0        0      110 2024-05-24 14:45:58.000000 sentiment_analysis_package-0.2.0/requirements/requirements.txt
--rw-rw-rw-   0        0        0  8080721 2024-05-31 05:07:25.000000 sentiment_analysis_package-0.2.0/sentiment_analysis_model_0.2.0.pkl
-drwxrwxrwx   0        0        0        0 2024-05-31 05:09:14.750108 sentiment_analysis_package-0.2.0/sentiment_analysis_package.egg-info/
--rw-rw-rw-   0        0        0      243 2024-05-31 05:09:14.000000 sentiment_analysis_package-0.2.0/sentiment_analysis_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      758 2024-05-31 05:09:14.000000 sentiment_analysis_package-0.2.0/sentiment_analysis_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 05:09:14.000000 sentiment_analysis_package-0.2.0/sentiment_analysis_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-31 05:09:14.000000 sentiment_analysis_package-0.2.0/sentiment_analysis_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-31 05:09:14.000000 sentiment_analysis_package-0.2.0/sentiment_analysis_package.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-31 05:09:14.740108 sentiment_analysis_package-0.2.0/sentiment_model/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:26.000000 sentiment_analysis_package-0.2.0/sentiment_model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 05:09:14.743108 sentiment_analysis_package-0.2.0/sentiment_model/config/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:34.000000 sentiment_analysis_package-0.2.0/sentiment_model/config/__init__.py
--rw-rw-rw-   0        0        0      772 2024-05-24 14:24:34.000000 sentiment_analysis_package-0.2.0/sentiment_model/config/core.py
--rw-rw-rw-   0        0        0      225 2024-05-31 04:50:52.000000 sentiment_analysis_package-0.2.0/sentiment_model/config.yml
--rw-rw-rw-   0        0        0      419 2024-05-24 15:14:18.000000 sentiment_analysis_package-0.2.0/sentiment_model/pipeline.py
--rw-rw-rw-   0        0        0      503 2024-05-31 03:07:55.000000 sentiment_analysis_package-0.2.0/sentiment_model/predict.py
-drwxrwxrwx   0        0        0        0 2024-05-31 05:09:14.746107 sentiment_analysis_package-0.2.0/sentiment_model/processing/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:48.000000 sentiment_analysis_package-0.2.0/sentiment_model/processing/__init__.py
--rw-rw-rw-   0        0        0      582 2024-05-31 02:39:25.000000 sentiment_analysis_package-0.2.0/sentiment_model/processing/features.py
--rw-rw-rw-   0        0        0      355 2024-05-24 11:22:44.000000 sentiment_analysis_package-0.2.0/sentiment_model/processing/validation.py
--rw-rw-rw-   0        0        0     1555 2024-05-31 02:34:37.000000 sentiment_analysis_package-0.2.0/sentiment_model/train_pipeline.py
--rw-rw-rw-   0        0        0       42 2024-05-31 05:09:14.752108 sentiment_analysis_package-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      414 2024-05-31 04:50:58.000000 sentiment_analysis_package-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-31 05:09:14.749108 sentiment_analysis_package-0.2.0/tests/
--rw-rw-rw-   0        0        0      154 2024-05-24 11:23:44.000000 sentiment_analysis_package-0.2.0/tests/test_pipeline.py
--rw-rw-rw-   0        0        0      263 2024-05-31 03:05:48.000000 sentiment_analysis_package-0.2.0/tests/test_predict.py
--rw-rw-rw-   0        0        0      244 2024-05-31 02:07:23.000000 sentiment_analysis_package-0.2.0/tests/test_processing.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:39:26.125480 sentiment_analysis_package-0.3.0/
+-rw-rw-rw-   0        0        0      323 2024-05-31 04:50:04.000000 sentiment_analysis_package-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      243 2024-05-31 05:39:26.123481 sentiment_analysis_package-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0        2 2024-05-24 11:24:36.000000 sentiment_analysis_package-0.3.0/README.md
+-rw-rw-rw-   0        0        0       93 2024-05-24 11:27:42.000000 sentiment_analysis_package-0.3.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-31 05:39:26.077483 sentiment_analysis_package-0.3.0/requirements/
+-rw-rw-rw-   0        0        0      110 2024-05-24 14:45:58.000000 sentiment_analysis_package-0.3.0/requirements/requirements.txt
+-rw-rw-rw-   0        0        0  8080721 2024-05-31 05:38:05.000000 sentiment_analysis_package-0.3.0/sentiment_analysis_model_0.3.0.pkl
+drwxrwxrwx   0        0        0        0 2024-05-31 05:39:26.121487 sentiment_analysis_package-0.3.0/sentiment_analysis_package.egg-info/
+-rw-rw-rw-   0        0        0      243 2024-05-31 05:39:26.000000 sentiment_analysis_package-0.3.0/sentiment_analysis_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      758 2024-05-31 05:39:26.000000 sentiment_analysis_package-0.3.0/sentiment_analysis_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 05:39:26.000000 sentiment_analysis_package-0.3.0/sentiment_analysis_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-31 05:39:26.000000 sentiment_analysis_package-0.3.0/sentiment_analysis_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-31 05:39:26.000000 sentiment_analysis_package-0.3.0/sentiment_analysis_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 05:39:26.093480 sentiment_analysis_package-0.3.0/sentiment_model/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:26.000000 sentiment_analysis_package-0.3.0/sentiment_model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:39:26.108482 sentiment_analysis_package-0.3.0/sentiment_model/config/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:34.000000 sentiment_analysis_package-0.3.0/sentiment_model/config/__init__.py
+-rw-rw-rw-   0        0        0      772 2024-05-24 14:24:34.000000 sentiment_analysis_package-0.3.0/sentiment_model/config/core.py
+-rw-rw-rw-   0        0        0      225 2024-05-31 05:39:11.000000 sentiment_analysis_package-0.3.0/sentiment_model/config.yml
+-rw-rw-rw-   0        0        0      419 2024-05-24 15:14:18.000000 sentiment_analysis_package-0.3.0/sentiment_model/pipeline.py
+-rw-rw-rw-   0        0        0      503 2024-05-31 03:07:55.000000 sentiment_analysis_package-0.3.0/sentiment_model/predict.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:39:26.114488 sentiment_analysis_package-0.3.0/sentiment_model/processing/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:48.000000 sentiment_analysis_package-0.3.0/sentiment_model/processing/__init__.py
+-rw-rw-rw-   0        0        0      582 2024-05-31 02:39:25.000000 sentiment_analysis_package-0.3.0/sentiment_model/processing/features.py
+-rw-rw-rw-   0        0        0      355 2024-05-24 11:22:44.000000 sentiment_analysis_package-0.3.0/sentiment_model/processing/validation.py
+-rw-rw-rw-   0        0        0     1555 2024-05-31 02:34:37.000000 sentiment_analysis_package-0.3.0/sentiment_model/train_pipeline.py
+-rw-rw-rw-   0        0        0       42 2024-05-31 05:39:26.125480 sentiment_analysis_package-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      414 2024-05-31 05:38:57.000000 sentiment_analysis_package-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:39:26.118481 sentiment_analysis_package-0.3.0/tests/
+-rw-rw-rw-   0        0        0      154 2024-05-24 11:23:44.000000 sentiment_analysis_package-0.3.0/tests/test_pipeline.py
+-rw-rw-rw-   0        0        0      263 2024-05-31 03:05:48.000000 sentiment_analysis_package-0.3.0/tests/test_predict.py
+-rw-rw-rw-   0        0        0      244 2024-05-31 02:07:23.000000 sentiment_analysis_package-0.3.0/tests/test_processing.py
```

### Comparing `sentiment_analysis_package-0.2.0/sentiment_analysis_model_0.2.0.pkl` & `sentiment_analysis_package-0.3.0/sentiment_analysis_model_0.3.0.pkl`

 * *Files 0% similar despite different names*

```diff
@@ -16084,15 +16084,15 @@
 0003ed30: af5b 97d8 981a 2440 9806 08df 69cc 2540  .[....$@....i.%@
 0003ed40: 9806 08df 69cc 2540 5b03 6efe 029c 2640  ....i.%@[.n...&@
 0003ed50: af5b 97d8 981a 2440 9500 0001 0000 0000  .[....$@........
 0003ed60: 008c 105f 736b 6c65 6172 6e5f 7665 7273  ..._sklearn_vers
 0003ed70: 696f 6e94 8c05 312e 352e 3094 7562 8c11  ion...1.5.0.ub..
 0003ed80: 6669 7865 645f 766f 6361 6275 6c61 7279  fixed_vocabulary
 0003ed90: 5f94 898c 0e5f 7374 6f70 5f77 6f72 6473  _...._stop_words
-0003eda0: 5f69 6494 8a06 70f8 0867 4a01 8c0b 766f  _id...p..gJ...vo
+0003eda0: 5f69 6494 8a06 3072 d498 6c02 8c0b 766f  _id...0r..l...vo
 0003edb0: 6361 6275 6c61 7279 5f94 7d94 288c 0467  cabulary_.}.(..g
 0003edc0: 6f6f 6494 4dc3 2e8c 0b61 6d62 6172 6b6f  ood.M....ambarko
 0003edd0: 7274 697a 944d 3a0b 8c03 6d61 6494 4d52  rtiz.M:...mad.MR
 0003ede0: 428c 0474 7572 6e94 4d65 6e8c 0362 6167  B..turn.Men..bag
 0003edf0: 944d 770f 8c07 6261 7374 696f 6e94 4df0  .Mw...bastion.M.
 0003ee00: 0f8c 036c 6f6c 944d 1441 8c05 7377 6565  ...lol.M.A..swee
 0003ee10: 7494 4dd3 678c 0573 7072 6179 944d 1365  t.M.g..spray.M.e
```

### Comparing `sentiment_analysis_package-0.2.0/sentiment_analysis_package.egg-info/SOURCES.txt` & `sentiment_analysis_package-0.3.0/sentiment_analysis_package.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 MANIFEST.in
 README.md
 pyproject.toml
-sentiment_analysis_model_0.2.0.pkl
+sentiment_analysis_model_0.3.0.pkl
 setup.py
 requirements/requirements.txt
 sentiment_analysis_package.egg-info/PKG-INFO
 sentiment_analysis_package.egg-info/SOURCES.txt
 sentiment_analysis_package.egg-info/dependency_links.txt
 sentiment_analysis_package.egg-info/requires.txt
 sentiment_analysis_package.egg-info/top_level.txt
```

### Comparing `sentiment_analysis_package-0.2.0/sentiment_model/config/core.py` & `sentiment_analysis_package-0.3.0/sentiment_model/config/core.py`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_package-0.2.0/sentiment_model/processing/features.py` & `sentiment_analysis_package-0.3.0/sentiment_model/processing/features.py`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_package-0.2.0/sentiment_model/train_pipeline.py` & `sentiment_analysis_package-0.3.0/sentiment_model/train_pipeline.py`

 * *Files identical despite different names*

