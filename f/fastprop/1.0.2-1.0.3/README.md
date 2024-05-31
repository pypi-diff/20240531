# Comparing `tmp/fastprop-1.0.2.tar.gz` & `tmp/fastprop-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastprop-1.0.2.tar", last modified: Wed May 29 17:02:30 2024, max compression
+gzip compressed data, was "fastprop-1.0.3.tar", last modified: Fri May 31 17:21:02 2024, max compression
```

## Comparing `fastprop-1.0.2.tar` & `fastprop-1.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:02:30.194127 fastprop-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-29 17:02:26.000000 fastprop-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-05-29 17:02:30.194127 fastprop-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-05-29 17:02:26.000000 fastprop-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:02:30.190127 fastprop-1.0.2/fastprop/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-29 17:02:26.000000 fastprop-1.0.2/fastprop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:02:30.194127 fastprop-1.0.2/fastprop/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:02:26.000000 fastprop-1.0.2/fastprop/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-05-29 17:02:26.000000 fastprop-1.0.2/fastprop/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-29 17:02:26.000000 fastprop-1.0.2/fastprop/cli/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-29 17:02:26.000000 fastprop-1.0.2/fastprop/cli/shap.py
--rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-29 17:02:26.000000 fastprop-1.0.2/fastprop/cli/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-05-29 17:02:26.000000 fastprop-1.0.2/fastprop/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    39676 2024-05-29 17:02:26.000000 fastprop-1.0.2/fastprop/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-29 17:02:26.000000 fastprop-1.0.2/fastprop/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-29 17:02:26.000000 fastprop-1.0.2/fastprop/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-29 17:02:26.000000 fastprop-1.0.2/fastprop/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12208 2024-05-29 17:02:26.000000 fastprop-1.0.2/fastprop/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:02:30.194127 fastprop-1.0.2/fastprop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-05-29 17:02:30.000000 fastprop-1.0.2/fastprop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-29 17:02:30.000000 fastprop-1.0.2/fastprop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:02:30.000000 fastprop-1.0.2/fastprop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-29 17:02:30.000000 fastprop-1.0.2/fastprop.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-29 17:02:30.000000 fastprop-1.0.2/fastprop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 17:02:30.000000 fastprop-1.0.2/fastprop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-29 17:02:26.000000 fastprop-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 17:02:30.194127 fastprop-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:02:30.194127 fastprop-1.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-29 17:02:26.000000 fastprop-1.0.2/test/test_fastprop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:21:02.752336 fastprop-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-31 17:20:59.000000 fastprop-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-05-31 17:21:02.752336 fastprop-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-05-31 17:20:59.000000 fastprop-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:21:02.748336 fastprop-1.0.3/fastprop/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-31 17:20:59.000000 fastprop-1.0.3/fastprop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:21:02.748336 fastprop-1.0.3/fastprop/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 17:20:59.000000 fastprop-1.0.3/fastprop/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-05-31 17:20:59.000000 fastprop-1.0.3/fastprop/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-31 17:20:59.000000 fastprop-1.0.3/fastprop/cli/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-31 17:20:59.000000 fastprop-1.0.3/fastprop/cli/shap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-31 17:20:59.000000 fastprop-1.0.3/fastprop/cli/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-05-31 17:20:59.000000 fastprop-1.0.3/fastprop/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39676 2024-05-31 17:20:59.000000 fastprop-1.0.3/fastprop/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-31 17:20:59.000000 fastprop-1.0.3/fastprop/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-31 17:20:59.000000 fastprop-1.0.3/fastprop/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-31 17:20:59.000000 fastprop-1.0.3/fastprop/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-05-31 17:20:59.000000 fastprop-1.0.3/fastprop/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:21:02.748336 fastprop-1.0.3/fastprop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-05-31 17:21:02.000000 fastprop-1.0.3/fastprop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-31 17:21:02.000000 fastprop-1.0.3/fastprop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 17:21:02.000000 fastprop-1.0.3/fastprop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-31 17:21:02.000000 fastprop-1.0.3/fastprop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-31 17:21:02.000000 fastprop-1.0.3/fastprop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 17:21:02.000000 fastprop-1.0.3/fastprop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-31 17:20:59.000000 fastprop-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 17:21:02.752336 fastprop-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:21:02.748336 fastprop-1.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-31 17:20:59.000000 fastprop-1.0.3/test/test_fastprop.py
```

### Comparing `fastprop-1.0.2/LICENSE` & `fastprop-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.2/PKG-INFO` & `fastprop-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastprop
-Version: 1.0.2
+Version: 1.0.3
 Summary: Fast Molecular Property Prediction with mordredcommunity
 Author: Jackson Burns
 License: MIT
 Project-URL: Homepage, https://github.com/JacksonBurns/fastprop
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastprop Version: 1.0.2 Summary: Fast Molecular
+Metadata-Version: 2.1 Name: fastprop Version: 1.0.3 Summary: Fast Molecular
 Property Prediction with mordredcommunity Author: Jackson Burns License: MIT
 Project-URL: Homepage, https://github.com/JacksonBurns/fastprop Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: pyyaml Requires-Dist:
 lightning Requires-Dist: torch>=1.13 Requires-Dist: mordredcommunity Requires-
 Dist: astartes[molecules] Requires-Dist: tensorboard Requires-Dist: psutil
 Requires-Dist: polars Requires-Dist: pandas Requires-Dist: pyarrow Provides-
```

### Comparing `fastprop-1.0.2/README.md` & `fastprop-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.2/fastprop/cli/base.py` & `fastprop-1.0.3/fastprop/cli/base.py`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.2/fastprop/cli/predict.py` & `fastprop-1.0.3/fastprop/cli/predict.py`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.2/fastprop/cli/shap.py` & `fastprop-1.0.3/fastprop/cli/shap.py`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.2/fastprop/cli/train.py` & `fastprop-1.0.3/fastprop/cli/train.py`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.2/fastprop/data.py` & `fastprop-1.0.3/fastprop/data.py`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.2/fastprop/defaults.py` & `fastprop-1.0.3/fastprop/defaults.py`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.2/fastprop/descriptors.py` & `fastprop-1.0.3/fastprop/descriptors.py`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.2/fastprop/io.py` & `fastprop-1.0.3/fastprop/io.py`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.2/fastprop/metrics.py` & `fastprop-1.0.3/fastprop/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,23 +32,29 @@
         prediction.numpy(force=True),
         multioutput="raw_values" if multitask else "uniform_average",
         sample_weight=truth.numpy(force=True),
     )
 
 
 def mean_absolute_error_score(truth: torch.Tensor, prediction: torch.Tensor, ignored: None, multitask: bool = False):
-    return torch.nn.functional.l1_loss(prediction, truth, reduction="none" if multitask else "mean")
+    res = torch.nn.functional.l1_loss(prediction, truth, reduction="none" if multitask else "mean")
+    if multitask:
+        res = res.mean(dim=0)
+    return res
 
 
 def mean_squared_error_loss(truth: torch.Tensor, prediction: torch.Tensor, ignored: None, multitask: bool = False):
-    return torch.nn.functional.mse_loss(prediction, truth, reduction="none" if multitask else "mean")
+    res = torch.nn.functional.mse_loss(prediction, truth, reduction="none" if multitask else "mean")
+    if multitask:
+        res = res.mean(dim=0)
+    return res
 
 
 def root_mean_squared_error_loss(truth: torch.Tensor, prediction: torch.Tensor, ignored: None, multitask: bool = False):
-    return torch.sqrt(mean_squared_error_loss(truth, prediction, multitask))
+    return torch.sqrt(mean_squared_error_loss(truth, prediction, ignored, multitask))
 
 
 def binary_accuracy_score(truth: torch.Tensor, prediction: torch.Tensor, ignored: None, multitask: bool = False):
     return accuracy(prediction, truth, task="binary")
 
 
 def binary_f1_score(truth: torch.Tensor, prediction: torch.Tensor, ignored: None, multitask: bool = False):
```

### Comparing `fastprop-1.0.2/fastprop/model.py` & `fastprop-1.0.3/fastprop/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
             pred = torch.sigmoid(pred)
         else:
             pred = torch.nn.functional.softmax(pred, dim=1)
 
         for metric in SCORE_LOOKUP[self.problem_type]:
             self.log(f"{name}_{metric.__name__}", metric(truth, pred, self.readout.out_features))
             if "multi" not in self.problem_type and self.n_tasks > 1:
-                per_task_metric = metric(truth, pred, True)
+                per_task_metric = metric(truth, pred, None, True)
                 for target, value in zip(self.target_names, per_task_metric):
                     self.log(f"{name}_{target}_{metric.__name__}", value)
 
 
 def train_and_test(
     output_directory: str,
     fastprop_model: fastprop,
```

### Comparing `fastprop-1.0.2/fastprop.egg-info/PKG-INFO` & `fastprop-1.0.3/fastprop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastprop
-Version: 1.0.2
+Version: 1.0.3
 Summary: Fast Molecular Property Prediction with mordredcommunity
 Author: Jackson Burns
 License: MIT
 Project-URL: Homepage, https://github.com/JacksonBurns/fastprop
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastprop Version: 1.0.2 Summary: Fast Molecular
+Metadata-Version: 2.1 Name: fastprop Version: 1.0.3 Summary: Fast Molecular
 Property Prediction with mordredcommunity Author: Jackson Burns License: MIT
 Project-URL: Homepage, https://github.com/JacksonBurns/fastprop Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: pyyaml Requires-Dist:
 lightning Requires-Dist: torch>=1.13 Requires-Dist: mordredcommunity Requires-
 Dist: astartes[molecules] Requires-Dist: tensorboard Requires-Dist: psutil
 Requires-Dist: polars Requires-Dist: pandas Requires-Dist: pyarrow Provides-
```

### Comparing `fastprop-1.0.2/pyproject.toml` & `fastprop-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastprop"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
     { name = "Jackson Burns" },
 ]
 license = { text = "MIT" }
 description = "Fast Molecular Property Prediction with mordredcommunity"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `fastprop-1.0.2/test/test_fastprop.py` & `fastprop-1.0.3/test/test_fastprop.py`

 * *Files identical despite different names*

