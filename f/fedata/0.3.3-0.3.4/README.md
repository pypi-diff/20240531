# Comparing `tmp/fedata-0.3.3.tar.gz` & `tmp/fedata-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedata-0.3.3.tar", max compression
+gzip compressed data, was "fedata-0.3.4.tar", max compression
```

## Comparing `fedata-0.3.3.tar` & `fedata-0.3.4.tar`

### file list

```diff
@@ -1,33 +1,19 @@
--rw-r--r--   0        0        0        0 2023-09-02 11:04:50.002671 fedata-0.3.3/fedata/__init__.py
--rw-r--r--   0        0        0      628 2023-09-02 11:12:30.225684 fedata-0.3.3/fedata/exceptions/__pycache__/fetchdataexceptions.cpython-310.pyc
--rw-r--r--   0        0        0      817 2023-09-02 11:12:20.628754 fedata-0.3.3/fedata/exceptions/__pycache__/generateexceptions.cpython-310.pyc
--rw-r--r--   0        0        0      293 2023-09-02 11:04:50.004812 fedata-0.3.3/fedata/exceptions/fetchdataexceptions.py
--rw-r--r--   0        0        0      410 2023-09-02 11:04:50.004812 fedata-0.3.3/fedata/exceptions/generateexceptions.py
--rw-r--r--   0        0        0     2588 2023-10-12 07:47:43.099177 fedata-0.3.3/fedata/hub/__pycache__/fetch_data.cpython-310.pyc
--rw-r--r--   0        0        0     1404 2023-09-02 11:12:50.554493 fedata-0.3.3/fedata/hub/__pycache__/generate_dataset.cpython-310.pyc
--rw-r--r--   0        0        0     3689 2023-09-28 09:39:42.322192 fedata-0.3.3/fedata/hub/fetch_data.py
--rw-r--r--   0        0        0     1290 2023-09-02 11:04:50.007073 fedata-0.3.3/fedata/hub/generate_dataset.py
--rw-r--r--   0        0        0     2015 2024-03-12 16:04:23.029576 fedata-0.3.3/fedata/load/__pycache__/load_cifar.cpython-310.pyc
--rw-r--r--   0        0        0     1969 2024-03-12 16:04:32.768402 fedata-0.3.3/fedata/load/__pycache__/load_fmnist.cpython-310.pyc
--rw-r--r--   0        0        0     1958 2024-03-12 16:04:32.777756 fedata-0.3.3/fedata/load/__pycache__/load_mnist.cpython-310.pyc
--rw-r--r--   0        0        0     3379 2024-03-12 16:02:43.822143 fedata-0.3.3/fedata/load/load_cifar.py
--rw-r--r--   0        0        0     3267 2024-03-12 16:02:25.235292 fedata-0.3.3/fedata/load/load_fmnist.py
--rw-r--r--   0        0        0     3278 2024-03-12 16:02:34.744819 fedata-0.3.3/fedata/load/load_mnist.py
--rw-r--r--   0        0        0     8160 2024-03-12 16:05:24.178715 fedata-0.3.3/fedata/split/__pycache__/shard_splits.cpython-310.pyc
--rw-r--r--   0        0        0    15482 2024-03-12 16:05:17.290521 fedata-0.3.3/fedata/split/shard_splits.py
--rw-r--r--   0        0        0     5504 2023-09-02 12:26:40.846089 fedata-0.3.3/fedata/transform/__pycache__/shard_transformation.cpython-310.pyc
--rw-r--r--   0        0        0     6086 2023-09-02 12:20:47.478633 fedata-0.3.3/fedata/transform/shard_transformation.py
--rw-r--r--   0        0        0     1147 2023-09-02 11:10:31.237511 fedata-0.3.3/fedata/utils/__pycache__/custom_transformation.cpython-310.pyc
--rw-r--r--   0        0        0     1332 2023-09-02 11:12:54.268988 fedata-0.3.3/fedata/utils/__pycache__/load_from_json.cpython-310.pyc
--rw-r--r--   0        0        0     2241 2023-09-02 12:34:56.060988 fedata-0.3.3/fedata/utils/__pycache__/save_blueprint.cpython-310.pyc
--rw-r--r--   0        0        0      774 2023-09-28 08:55:34.176330 fedata-0.3.3/fedata/utils/__pycache__/save_dataset.cpython-310.pyc
--rw-r--r--   0        0        0     1349 2023-09-02 12:45:11.438631 fedata-0.3.3/fedata/utils/__pycache__/showcase.cpython-310.pyc
--rw-r--r--   0        0        0      633 2023-09-02 11:04:50.013008 fedata-0.3.3/fedata/utils/custom_transformation.py
--rw-r--r--   0        0        0     1059 2023-09-02 11:04:50.013008 fedata-0.3.3/fedata/utils/load_from_json.py
--rw-r--r--   0        0        0     2119 2023-09-02 12:34:36.730854 fedata-0.3.3/fedata/utils/save_blueprint.py
--rw-r--r--   0        0        0      612 2023-09-28 08:55:13.025705 fedata-0.3.3/fedata/utils/save_dataset.py
--rw-r--r--   0        0        0     1203 2023-09-02 12:45:02.783406 fedata-0.3.3/fedata/utils/showcase.py
--rw-r--r--   0        0        0      424 2024-03-12 16:23:36.370239 fedata-0.3.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-09-02 11:04:49.989065 fedata-0.3.3/README.md
--rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 fedata-0.3.3/setup.py
--rw-r--r--   0        0        0      503 1970-01-01 00:00:00.000000 fedata-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-09-02 11:04:50.002671 fedata-0.3.4/fedata/__init__.py
+-rw-r--r--   0        0        0      293 2023-09-02 11:04:50.004812 fedata-0.3.4/fedata/exceptions/fetchdataexceptions.py
+-rw-r--r--   0        0        0      410 2023-09-02 11:04:50.004812 fedata-0.3.4/fedata/exceptions/generateexceptions.py
+-rw-r--r--   0        0        0     3689 2024-05-31 18:12:00.052623 fedata-0.3.4/fedata/hub/fetch_data.py
+-rw-r--r--   0        0        0     1290 2024-05-31 18:12:00.056627 fedata-0.3.4/fedata/hub/generate_dataset.py
+-rw-r--r--   0        0        0     3379 2024-05-31 18:12:00.060927 fedata-0.3.4/fedata/load/load_cifar.py
+-rw-r--r--   0        0        0     3267 2024-05-31 18:12:00.064062 fedata-0.3.4/fedata/load/load_fmnist.py
+-rw-r--r--   0        0        0     3278 2024-05-31 18:12:00.075394 fedata-0.3.4/fedata/load/load_mnist.py
+-rw-r--r--   0        0        0    15517 2024-05-31 18:13:14.821602 fedata-0.3.4/fedata/split/shard_splits.py
+-rw-r--r--   0        0        0     6086 2023-09-02 12:20:47.478633 fedata-0.3.4/fedata/transform/shard_transformation.py
+-rw-r--r--   0        0        0      633 2023-09-02 11:04:50.013008 fedata-0.3.4/fedata/utils/custom_transformation.py
+-rw-r--r--   0        0        0     1059 2023-09-02 11:04:50.013008 fedata-0.3.4/fedata/utils/load_from_json.py
+-rw-r--r--   0        0        0     2119 2023-09-02 12:34:36.730854 fedata-0.3.4/fedata/utils/save_blueprint.py
+-rw-r--r--   0        0        0      612 2023-09-28 08:55:13.025705 fedata-0.3.4/fedata/utils/save_dataset.py
+-rw-r--r--   0        0        0     1203 2023-09-02 12:45:02.783406 fedata-0.3.4/fedata/utils/showcase.py
+-rw-r--r--   0        0        0      424 2024-05-31 18:14:44.760381 fedata-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-09-02 11:04:49.989065 fedata-0.3.4/README.md
+-rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 fedata-0.3.4/setup.py
+-rw-r--r--   0        0        0      503 1970-01-01 00:00:00.000000 fedata-0.3.4/PKG-INFO
```

### Comparing `fedata-0.3.3/fedata/hub/fetch_data.py` & `fedata-0.3.4/fedata/hub/fetch_data.py`

 * *Files identical despite different names*

### Comparing `fedata-0.3.3/fedata/hub/generate_dataset.py` & `fedata-0.3.4/fedata/hub/generate_dataset.py`

 * *Files identical despite different names*

### Comparing `fedata-0.3.3/fedata/load/load_cifar.py` & `fedata-0.3.4/fedata/load/load_cifar.py`

 * *Files identical despite different names*

### Comparing `fedata-0.3.3/fedata/load/load_fmnist.py` & `fedata-0.3.4/fedata/load/load_fmnist.py`

 * *Files identical despite different names*

### Comparing `fedata-0.3.3/fedata/load/load_mnist.py` & `fedata-0.3.4/fedata/load/load_mnist.py`

 * *Files identical despite different names*

### Comparing `fedata-0.3.3/fedata/split/shard_splits.py` & `fedata-0.3.4/fedata/split/shard_splits.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
         for agent in agents:
             if agent in mising_classes:
                 # 1. Sampling indexes
                 sampling_weights = {key: (1 / ( len(labels) - len(mising_classes[agent] )))
                                     if key not in mising_classes[agent] else 0 for key in labels}                
                 # 2. Applying weights
                 pandas_df["weights"] = pandas_df['label'].apply(lambda x: sampling_weights[x])
-                sample = pandas_df.sample(n = sample_size, weights='weights', random_state=42)
+                sample = pandas_df.sample(n = sample_size, weights='weights', random_state=42, replace=settings['allow_replace'])
                 
                 # 3. Selecting indexes and performing test - train split.
                 sampled_data = dataset.filter(lambda _, idx: idx in list(sample.index), with_indices=True)
                 
                 # Shard transformation
                 if agent in settings['transformations'].keys():
                     sampled_data = transform_shard(shard=sampled_data,
```

### Comparing `fedata-0.3.3/fedata/transform/shard_transformation.py` & `fedata-0.3.4/fedata/transform/shard_transformation.py`

 * *Files identical despite different names*

### Comparing `fedata-0.3.3/fedata/utils/custom_transformation.py` & `fedata-0.3.4/fedata/utils/custom_transformation.py`

 * *Files identical despite different names*

### Comparing `fedata-0.3.3/fedata/utils/load_from_json.py` & `fedata-0.3.4/fedata/utils/load_from_json.py`

 * *Files identical despite different names*

### Comparing `fedata-0.3.3/fedata/utils/save_blueprint.py` & `fedata-0.3.4/fedata/utils/save_blueprint.py`

 * *Files identical despite different names*

### Comparing `fedata-0.3.3/fedata/utils/save_dataset.py` & `fedata-0.3.4/fedata/utils/save_dataset.py`

 * *Files identical despite different names*

### Comparing `fedata-0.3.3/fedata/utils/showcase.py` & `fedata-0.3.4/fedata/utils/showcase.py`

 * *Files identical despite different names*

### Comparing `fedata-0.3.3/setup.py` & `fedata-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'numpy>=1.24.1',
  'scikit-learn>=1.2.0',
  'torchaudio>=2.0.2',
  'torchvision>=0.15.1']
 
 setup_kwargs = {
     'name': 'fedata',
-    'version': '0.3.3',
+    'version': '0.3.4',
     'description': '',
     'long_description': '',
     'author': 'Scolpe',
     'author_email': 'maciejzuziak101@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

