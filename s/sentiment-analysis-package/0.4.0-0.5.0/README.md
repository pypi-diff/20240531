# Comparing `tmp/sentiment_analysis_package-0.4.0.tar.gz` & `tmp/sentiment_analysis_package-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentiment_analysis_package-0.4.0.tar", last modified: Fri May 31 06:10:21 2024, max compression
+gzip compressed data, was "sentiment_analysis_package-0.5.0.tar", last modified: Fri May 31 07:38:44 2024, max compression
```

## Comparing `sentiment_analysis_package-0.4.0.tar` & `sentiment_analysis_package-0.5.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 06:10:21.494379 sentiment_analysis_package-0.4.0/
--rw-rw-rw-   0        0        0      305 2024-05-31 05:54:40.000000 sentiment_analysis_package-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0      243 2024-05-31 06:10:21.476118 sentiment_analysis_package-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0        2 2024-05-24 11:24:36.000000 sentiment_analysis_package-0.4.0/README.md
--rw-rw-rw-   0        0        0       93 2024-05-24 11:27:42.000000 sentiment_analysis_package-0.4.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-31 06:10:21.453118 sentiment_analysis_package-0.4.0/requirements/
--rw-rw-rw-   0        0        0      110 2024-05-24 14:45:58.000000 sentiment_analysis_package-0.4.0/requirements/requirements.txt
--rw-rw-rw-   0        0        0  8080721 2024-05-31 06:07:52.000000 sentiment_analysis_package-0.4.0/sentiment_analysis_model_0.4.0.pkl
-drwxrwxrwx   0        0        0        0 2024-05-31 06:10:21.476118 sentiment_analysis_package-0.4.0/sentiment_analysis_package.egg-info/
--rw-rw-rw-   0        0        0      243 2024-05-31 06:10:21.000000 sentiment_analysis_package-0.4.0/sentiment_analysis_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      758 2024-05-31 06:10:21.000000 sentiment_analysis_package-0.4.0/sentiment_analysis_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 06:10:21.000000 sentiment_analysis_package-0.4.0/sentiment_analysis_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-31 06:10:21.000000 sentiment_analysis_package-0.4.0/sentiment_analysis_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-31 06:10:21.000000 sentiment_analysis_package-0.4.0/sentiment_analysis_package.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-31 06:10:21.465118 sentiment_analysis_package-0.4.0/sentiment_model/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:26.000000 sentiment_analysis_package-0.4.0/sentiment_model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 06:10:21.467121 sentiment_analysis_package-0.4.0/sentiment_model/config/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:34.000000 sentiment_analysis_package-0.4.0/sentiment_model/config/__init__.py
--rw-rw-rw-   0        0        0      772 2024-05-24 14:24:34.000000 sentiment_analysis_package-0.4.0/sentiment_model/config/core.py
--rw-rw-rw-   0        0        0      225 2024-05-31 05:55:09.000000 sentiment_analysis_package-0.4.0/sentiment_model/config.yml
--rw-rw-rw-   0        0        0      419 2024-05-24 15:14:18.000000 sentiment_analysis_package-0.4.0/sentiment_model/pipeline.py
--rw-rw-rw-   0        0        0      503 2024-05-31 03:07:55.000000 sentiment_analysis_package-0.4.0/sentiment_model/predict.py
-drwxrwxrwx   0        0        0        0 2024-05-31 06:10:21.470118 sentiment_analysis_package-0.4.0/sentiment_model/processing/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:48.000000 sentiment_analysis_package-0.4.0/sentiment_model/processing/__init__.py
--rw-rw-rw-   0        0        0      582 2024-05-31 02:39:25.000000 sentiment_analysis_package-0.4.0/sentiment_model/processing/features.py
--rw-rw-rw-   0        0        0      355 2024-05-24 11:22:44.000000 sentiment_analysis_package-0.4.0/sentiment_model/processing/validation.py
--rw-rw-rw-   0        0        0     1555 2024-05-31 02:34:37.000000 sentiment_analysis_package-0.4.0/sentiment_model/train_pipeline.py
--rw-rw-rw-   0        0        0       42 2024-05-31 06:10:21.494379 sentiment_analysis_package-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      429 2024-05-31 05:54:54.000000 sentiment_analysis_package-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-31 06:10:21.474120 sentiment_analysis_package-0.4.0/tests/
--rw-rw-rw-   0        0        0      154 2024-05-24 11:23:44.000000 sentiment_analysis_package-0.4.0/tests/test_pipeline.py
--rw-rw-rw-   0        0        0      263 2024-05-31 03:05:48.000000 sentiment_analysis_package-0.4.0/tests/test_predict.py
--rw-rw-rw-   0        0        0      244 2024-05-31 02:07:23.000000 sentiment_analysis_package-0.4.0/tests/test_processing.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:38:44.203962 sentiment_analysis_package-0.5.0/
+-rw-rw-rw-   0        0        0      305 2024-05-31 05:54:40.000000 sentiment_analysis_package-0.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      243 2024-05-31 07:38:44.202965 sentiment_analysis_package-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0        2 2024-05-24 11:24:36.000000 sentiment_analysis_package-0.5.0/README.md
+-rw-rw-rw-   0        0        0       93 2024-05-24 11:27:42.000000 sentiment_analysis_package-0.5.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-31 07:38:44.154236 sentiment_analysis_package-0.5.0/requirements/
+-rw-rw-rw-   0        0        0      118 2024-05-31 07:09:14.000000 sentiment_analysis_package-0.5.0/requirements/requirements.txt
+-rw-rw-rw-   0        0        0  8080721 2024-05-31 07:34:07.000000 sentiment_analysis_package-0.5.0/sentiment_analysis_model_0.5.0.pkl
+drwxrwxrwx   0        0        0        0 2024-05-31 07:38:44.200963 sentiment_analysis_package-0.5.0/sentiment_analysis_package.egg-info/
+-rw-rw-rw-   0        0        0      243 2024-05-31 07:38:44.000000 sentiment_analysis_package-0.5.0/sentiment_analysis_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      758 2024-05-31 07:38:44.000000 sentiment_analysis_package-0.5.0/sentiment_analysis_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 07:38:44.000000 sentiment_analysis_package-0.5.0/sentiment_analysis_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-31 07:38:44.000000 sentiment_analysis_package-0.5.0/sentiment_analysis_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-31 07:38:44.000000 sentiment_analysis_package-0.5.0/sentiment_analysis_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 07:38:44.187964 sentiment_analysis_package-0.5.0/sentiment_model/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:26.000000 sentiment_analysis_package-0.5.0/sentiment_model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:38:44.189962 sentiment_analysis_package-0.5.0/sentiment_model/config/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:34.000000 sentiment_analysis_package-0.5.0/sentiment_model/config/__init__.py
+-rw-rw-rw-   0        0        0      743 2024-05-31 07:22:22.000000 sentiment_analysis_package-0.5.0/sentiment_model/config/core.py
+-rw-rw-rw-   0        0        0      225 2024-05-31 07:22:53.000000 sentiment_analysis_package-0.5.0/sentiment_model/config.yml
+-rw-rw-rw-   0        0        0      419 2024-05-24 15:14:18.000000 sentiment_analysis_package-0.5.0/sentiment_model/pipeline.py
+-rw-rw-rw-   0        0        0      499 2024-05-31 07:38:25.000000 sentiment_analysis_package-0.5.0/sentiment_model/predict.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:38:44.193964 sentiment_analysis_package-0.5.0/sentiment_model/processing/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:48.000000 sentiment_analysis_package-0.5.0/sentiment_model/processing/__init__.py
+-rw-rw-rw-   0        0        0      582 2024-05-31 02:39:25.000000 sentiment_analysis_package-0.5.0/sentiment_model/processing/features.py
+-rw-rw-rw-   0        0        0      355 2024-05-24 11:22:44.000000 sentiment_analysis_package-0.5.0/sentiment_model/processing/validation.py
+-rw-rw-rw-   0        0        0     1575 2024-05-31 07:22:26.000000 sentiment_analysis_package-0.5.0/sentiment_model/train_pipeline.py
+-rw-rw-rw-   0        0        0       42 2024-05-31 07:38:44.203962 sentiment_analysis_package-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      429 2024-05-31 07:22:49.000000 sentiment_analysis_package-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:38:44.198967 sentiment_analysis_package-0.5.0/tests/
+-rw-rw-rw-   0        0        0      154 2024-05-24 11:23:44.000000 sentiment_analysis_package-0.5.0/tests/test_pipeline.py
+-rw-rw-rw-   0        0        0      263 2024-05-31 03:05:48.000000 sentiment_analysis_package-0.5.0/tests/test_predict.py
+-rw-rw-rw-   0        0        0      244 2024-05-31 02:07:23.000000 sentiment_analysis_package-0.5.0/tests/test_processing.py
```

### Comparing `sentiment_analysis_package-0.4.0/sentiment_analysis_model_0.4.0.pkl` & `sentiment_analysis_package-0.5.0/sentiment_analysis_model_0.5.0.pkl`

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
-0003eda0: 5f69 6494 8a06 b074 e9ff e001 8c0b 766f  _id....t......vo
+0003eda0: 5f69 6494 8a06 707b d50d 0102 8c0b 766f  _id...p{......vo
 0003edb0: 6361 6275 6c61 7279 5f94 7d94 288c 0467  cabulary_.}.(..g
 0003edc0: 6f6f 6494 4dc3 2e8c 0b61 6d62 6172 6b6f  ood.M....ambarko
 0003edd0: 7274 697a 944d 3a0b 8c03 6d61 6494 4d52  rtiz.M:...mad.MR
 0003ede0: 428c 0474 7572 6e94 4d65 6e8c 0362 6167  B..turn.Men..bag
 0003edf0: 944d 770f 8c07 6261 7374 696f 6e94 4df0  .Mw...bastion.M.
 0003ee00: 0f8c 036c 6f6c 944d 1441 8c05 7377 6565  ...lol.M.A..swee
 0003ee10: 7494 4dd3 678c 0573 7072 6179 944d 1365  t.M.g..spray.M.e
```

### Comparing `sentiment_analysis_package-0.4.0/sentiment_analysis_package.egg-info/SOURCES.txt` & `sentiment_analysis_package-0.5.0/sentiment_analysis_package.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 MANIFEST.in
 README.md
 pyproject.toml
-sentiment_analysis_model_0.4.0.pkl
+sentiment_analysis_model_0.5.0.pkl
 setup.py
 requirements/requirements.txt
 sentiment_analysis_package.egg-info/PKG-INFO
 sentiment_analysis_package.egg-info/SOURCES.txt
 sentiment_analysis_package.egg-info/dependency_links.txt
 sentiment_analysis_package.egg-info/requires.txt
 sentiment_analysis_package.egg-info/top_level.txt
```

### Comparing `sentiment_analysis_package-0.4.0/sentiment_model/config/core.py` & `sentiment_analysis_package-0.5.0/sentiment_model/config/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pydantic import BaseModel
-from strictyaml import load, YAML
+from strictyaml import load
 
 class TrainingConfig(BaseModel):
     batch_size: int
     epochs: int
     learning_rate: float
 
 class ModelConfig(BaseModel):
@@ -15,16 +15,18 @@
     test_size: float
 
 class AppConfig(BaseModel):
     model: ModelConfig
     training: TrainingConfig
     data: DataConfig
 
-def fetch_config_from_yaml(cfg_path: str) -> AppConfig:
-    with open(cfg_path, 'r') as conf_file:
-        config_data = conf_file.read()
-    cfg = load(config_data)
-    return AppConfig(
-        model=ModelConfig(**cfg['model'].data),
-        training=TrainingConfig(**cfg['training'].data),
-        data=DataConfig(**cfg['data'].data),
-    )
+
+import os
+import yaml
+
+
+def fetch_config_from_yaml(cfg_path):
+    sentiment_model_path = os.path.dirname(os.path.dirname(os.path.abspath(__file__))) 
+    config_path = os.path.join(sentiment_model_path, cfg_path)
+    with open(config_path, 'r') as conf_file:
+        config = yaml.safe_load(conf_file)
+    return config
```

### Comparing `sentiment_analysis_package-0.4.0/sentiment_model/processing/features.py` & `sentiment_analysis_package-0.5.0/sentiment_model/processing/features.py`

 * *Files identical despite different names*

