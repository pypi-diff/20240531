# Comparing `tmp/sentiment_analysis_package-0.8.0.tar.gz` & `tmp/sentiment_analysis_package-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentiment_analysis_package-0.8.0.tar", last modified: Fri May 31 08:02:50 2024, max compression
+gzip compressed data, was "sentiment_analysis_package-0.9.0.tar", last modified: Fri May 31 09:11:48 2024, max compression
```

## Comparing `sentiment_analysis_package-0.8.0.tar` & `sentiment_analysis_package-0.9.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 08:02:50.222191 sentiment_analysis_package-0.8.0/
--rw-rw-rw-   0        0        0      391 2024-05-31 07:59:51.000000 sentiment_analysis_package-0.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0      243 2024-05-31 08:02:50.221188 sentiment_analysis_package-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0        2 2024-05-24 11:24:36.000000 sentiment_analysis_package-0.8.0/README.md
--rw-rw-rw-   0        0        0       93 2024-05-24 11:27:42.000000 sentiment_analysis_package-0.8.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-31 08:02:50.183187 sentiment_analysis_package-0.8.0/requirements/
--rw-rw-rw-   0        0        0      118 2024-05-31 07:09:14.000000 sentiment_analysis_package-0.8.0/requirements/requirements.txt
--rw-rw-rw-   0        0        0  8080721 2024-05-31 07:34:07.000000 sentiment_analysis_package-0.8.0/sentiment_analysis_model_0.8.0.pkl
-drwxrwxrwx   0        0        0        0 2024-05-31 08:02:50.220193 sentiment_analysis_package-0.8.0/sentiment_analysis_package.egg-info/
--rw-rw-rw-   0        0        0      243 2024-05-31 08:02:50.000000 sentiment_analysis_package-0.8.0/sentiment_analysis_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      804 2024-05-31 08:02:50.000000 sentiment_analysis_package-0.8.0/sentiment_analysis_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 08:02:50.000000 sentiment_analysis_package-0.8.0/sentiment_analysis_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-31 08:02:50.000000 sentiment_analysis_package-0.8.0/sentiment_analysis_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-31 08:02:50.000000 sentiment_analysis_package-0.8.0/sentiment_analysis_package.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-31 08:02:50.196193 sentiment_analysis_package-0.8.0/sentiment_model/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:26.000000 sentiment_analysis_package-0.8.0/sentiment_model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:02:50.198188 sentiment_analysis_package-0.8.0/sentiment_model/config/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:34.000000 sentiment_analysis_package-0.8.0/sentiment_model/config/__init__.py
--rw-rw-rw-   0        0        0      743 2024-05-31 07:22:22.000000 sentiment_analysis_package-0.8.0/sentiment_model/config/core.py
--rw-rw-rw-   0        0        0      227 2024-05-31 07:57:54.000000 sentiment_analysis_package-0.8.0/sentiment_model/config.yml
-drwxrwxrwx   0        0        0        0 2024-05-31 08:02:50.200190 sentiment_analysis_package-0.8.0/sentiment_model/datasets/
--rw-rw-rw-   0        0        0 10325088 2021-08-08 23:52:12.000000 sentiment_analysis_package-0.8.0/sentiment_model/datasets/twitter_training.csv
--rw-rw-rw-   0        0        0      419 2024-05-24 15:14:18.000000 sentiment_analysis_package-0.8.0/sentiment_model/pipeline.py
--rw-rw-rw-   0        0        0      499 2024-05-31 07:38:25.000000 sentiment_analysis_package-0.8.0/sentiment_model/predict.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:02:50.214191 sentiment_analysis_package-0.8.0/sentiment_model/processing/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:48.000000 sentiment_analysis_package-0.8.0/sentiment_model/processing/__init__.py
--rw-rw-rw-   0        0        0      582 2024-05-31 02:39:25.000000 sentiment_analysis_package-0.8.0/sentiment_model/processing/features.py
--rw-rw-rw-   0        0        0      355 2024-05-24 11:22:44.000000 sentiment_analysis_package-0.8.0/sentiment_model/processing/validation.py
--rw-rw-rw-   0        0        0     1575 2024-05-31 07:22:26.000000 sentiment_analysis_package-0.8.0/sentiment_model/train_pipeline.py
--rw-rw-rw-   0        0        0       42 2024-05-31 08:02:50.222191 sentiment_analysis_package-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0      471 2024-05-31 08:01:50.000000 sentiment_analysis_package-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:02:50.218190 sentiment_analysis_package-0.8.0/tests/
--rw-rw-rw-   0        0        0      154 2024-05-24 11:23:44.000000 sentiment_analysis_package-0.8.0/tests/test_pipeline.py
--rw-rw-rw-   0        0        0      263 2024-05-31 03:05:48.000000 sentiment_analysis_package-0.8.0/tests/test_predict.py
--rw-rw-rw-   0        0        0      244 2024-05-31 02:07:23.000000 sentiment_analysis_package-0.8.0/tests/test_processing.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:11:48.439628 sentiment_analysis_package-0.9.0/
+-rw-rw-rw-   0        0        0      406 2024-05-31 08:17:06.000000 sentiment_analysis_package-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      243 2024-05-31 09:11:48.435644 sentiment_analysis_package-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0        2 2024-05-24 11:24:36.000000 sentiment_analysis_package-0.9.0/README.md
+-rw-rw-rw-   0        0        0       93 2024-05-24 11:27:42.000000 sentiment_analysis_package-0.9.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-31 09:11:48.266630 sentiment_analysis_package-0.9.0/requirements/
+-rw-rw-rw-   0        0        0      118 2024-05-31 07:09:14.000000 sentiment_analysis_package-0.9.0/requirements/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 09:11:48.431624 sentiment_analysis_package-0.9.0/sentiment_analysis_package.egg-info/
+-rw-rw-rw-   0        0        0      243 2024-05-31 09:11:48.000000 sentiment_analysis_package-0.9.0/sentiment_analysis_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      835 2024-05-31 09:11:48.000000 sentiment_analysis_package-0.9.0/sentiment_analysis_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 09:11:48.000000 sentiment_analysis_package-0.9.0/sentiment_analysis_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-31 09:11:48.000000 sentiment_analysis_package-0.9.0/sentiment_analysis_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-31 09:11:48.000000 sentiment_analysis_package-0.9.0/sentiment_analysis_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 09:11:48.319628 sentiment_analysis_package-0.9.0/sentiment_model/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:26.000000 sentiment_analysis_package-0.9.0/sentiment_model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:11:48.332629 sentiment_analysis_package-0.9.0/sentiment_model/config/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:34.000000 sentiment_analysis_package-0.9.0/sentiment_model/config/__init__.py
+-rw-rw-rw-   0        0        0      743 2024-05-31 07:22:22.000000 sentiment_analysis_package-0.9.0/sentiment_model/config/core.py
+-rw-rw-rw-   0        0        0      277 2024-05-31 08:57:31.000000 sentiment_analysis_package-0.9.0/sentiment_model/config.yml
+drwxrwxrwx   0        0        0        0 2024-05-31 09:11:48.334643 sentiment_analysis_package-0.9.0/sentiment_model/datasets/
+-rw-rw-rw-   0        0        0 10325088 2021-08-08 23:52:12.000000 sentiment_analysis_package-0.9.0/sentiment_model/datasets/twitter_training.csv
+-rw-rw-rw-   0        0        0      419 2024-05-24 15:14:18.000000 sentiment_analysis_package-0.9.0/sentiment_model/pipeline.py
+-rw-rw-rw-   0        0        0      499 2024-05-31 07:38:25.000000 sentiment_analysis_package-0.9.0/sentiment_model/predict.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:11:48.378631 sentiment_analysis_package-0.9.0/sentiment_model/processing/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:48.000000 sentiment_analysis_package-0.9.0/sentiment_model/processing/__init__.py
+-rw-rw-rw-   0        0        0      582 2024-05-31 02:39:25.000000 sentiment_analysis_package-0.9.0/sentiment_model/processing/features.py
+-rw-rw-rw-   0        0        0      355 2024-05-24 11:22:44.000000 sentiment_analysis_package-0.9.0/sentiment_model/processing/validation.py
+-rw-rw-rw-   0        0        0     1606 2024-05-31 08:44:25.000000 sentiment_analysis_package-0.9.0/sentiment_model/train_pipeline.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:11:48.382627 sentiment_analysis_package-0.9.0/sentiment_model/trained_models/
+-rw-rw-rw-   0        0        0  8080721 2024-05-31 09:10:39.000000 sentiment_analysis_package-0.9.0/sentiment_model/trained_models/sentiment_analysis_model_0.9.0.pkl
+-rw-rw-rw-   0        0        0       42 2024-05-31 09:11:48.439628 sentiment_analysis_package-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      486 2024-05-31 08:16:40.000000 sentiment_analysis_package-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:11:48.424640 sentiment_analysis_package-0.9.0/tests/
+-rw-rw-rw-   0        0        0      154 2024-05-24 11:23:44.000000 sentiment_analysis_package-0.9.0/tests/test_pipeline.py
+-rw-rw-rw-   0        0        0      263 2024-05-31 03:05:48.000000 sentiment_analysis_package-0.9.0/tests/test_predict.py
+-rw-rw-rw-   0        0        0      244 2024-05-31 02:07:23.000000 sentiment_analysis_package-0.9.0/tests/test_processing.py
```

### Comparing `sentiment_analysis_package-0.8.0/sentiment_analysis_model_0.8.0.pkl` & `sentiment_analysis_package-0.9.0/sentiment_model/trained_models/sentiment_analysis_model_0.9.0.pkl`

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
-0003eda0: 5f69 6494 8a06 707b d50d 0102 8c0b 766f  _id...p{......vo
+0003eda0: 5f69 6494 8a06 f077 8492 b501 8c0b 766f  _id....w......vo
 0003edb0: 6361 6275 6c61 7279 5f94 7d94 288c 0467  cabulary_.}.(..g
 0003edc0: 6f6f 6494 4dc3 2e8c 0b61 6d62 6172 6b6f  ood.M....ambarko
 0003edd0: 7274 697a 944d 3a0b 8c03 6d61 6494 4d52  rtiz.M:...mad.MR
 0003ede0: 428c 0474 7572 6e94 4d65 6e8c 0362 6167  B..turn.Men..bag
 0003edf0: 944d 770f 8c07 6261 7374 696f 6e94 4df0  .Mw...bastion.M.
 0003ee00: 0f8c 036c 6f6c 944d 1441 8c05 7377 6565  ...lol.M.A..swee
 0003ee10: 7494 4dd3 678c 0573 7072 6179 944d 1365  t.M.g..spray.M.e
```

### Comparing `sentiment_analysis_package-0.8.0/sentiment_analysis_package.egg-info/SOURCES.txt` & `sentiment_analysis_package-0.9.0/sentiment_analysis_package.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 MANIFEST.in
 README.md
 pyproject.toml
-sentiment_analysis_model_0.8.0.pkl
 setup.py
 requirements/requirements.txt
 sentiment_analysis_package.egg-info/PKG-INFO
 sentiment_analysis_package.egg-info/SOURCES.txt
 sentiment_analysis_package.egg-info/dependency_links.txt
 sentiment_analysis_package.egg-info/requires.txt
 sentiment_analysis_package.egg-info/top_level.txt
@@ -16,10 +15,11 @@
 sentiment_model/train_pipeline.py
 sentiment_model/config/__init__.py
 sentiment_model/config/core.py
 sentiment_model/datasets/twitter_training.csv
 sentiment_model/processing/__init__.py
 sentiment_model/processing/features.py
 sentiment_model/processing/validation.py
+sentiment_model/trained_models/sentiment_analysis_model_0.9.0.pkl
 tests/test_pipeline.py
 tests/test_predict.py
 tests/test_processing.py
```

### Comparing `sentiment_analysis_package-0.8.0/sentiment_model/config/core.py` & `sentiment_analysis_package-0.9.0/sentiment_model/config/core.py`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_package-0.8.0/sentiment_model/datasets/twitter_training.csv` & `sentiment_analysis_package-0.9.0/sentiment_model/datasets/twitter_training.csv`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_package-0.8.0/sentiment_model/processing/features.py` & `sentiment_analysis_package-0.9.0/sentiment_model/processing/features.py`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_package-0.8.0/sentiment_model/train_pipeline.py` & `sentiment_analysis_package-0.9.0/sentiment_model/train_pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,12 +28,12 @@
     X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=config["data"]["test_size"], random_state=42)
 
     logger.info("Creating and training the pipeline.")
     pipeline = create_pipeline()
     pipeline.fit(X_train, y_train)
 
     logger.info("Saving the trained model.")
-    dump(pipeline, f"{config['model']['name']}_{config['model']['version']}.pkl")
+    dump(pipeline, f"{config['data']['saving_path']}{config['model']['name']}_{config['model']['version']}.pkl")
     logger.info(f"Model trained and saved as {config['model']['name']}_{config['model']['version']}.pkl")
 
 if __name__ == "__main__":
     train()
```

