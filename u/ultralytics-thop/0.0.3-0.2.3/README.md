# Comparing `tmp/ultralytics_thop-0.0.3.tar.gz` & `tmp/ultralytics_thop-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultralytics_thop-0.0.3.tar", last modified: Fri May 31 19:10:24 2024, max compression
+gzip compressed data, was "ultralytics_thop-0.2.3.tar", last modified: Fri May 31 20:00:40 2024, max compression
```

## Comparing `ultralytics_thop-0.0.3.tar` & `ultralytics_thop-0.2.3.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:10:24.217950 ultralytics_thop-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    47915 2024-05-31 19:10:24.217950 ultralytics_thop-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 19:10:24.217950 ultralytics_thop-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:10:24.213950 ultralytics_thop-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/tests/test_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/tests/test_matmul.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/tests/test_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:10:24.213950 ultralytics_thop-0.0.3/thop/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/thop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/thop/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/thop/fx_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/thop/onnx_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/thop/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/thop/rnn_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/thop/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:10:24.213950 ultralytics_thop-0.0.3/thop/vision/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/thop/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/thop/vision/basic_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/thop/vision/calc_func.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/thop/vision/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    13298 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/thop/vision/onnx_counter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:10:24.217950 ultralytics_thop-0.0.3/ultralytics_thop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    47915 2024-05-31 19:10:24.000000 ultralytics_thop-0.0.3/ultralytics_thop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-31 19:10:24.000000 ultralytics_thop-0.0.3/ultralytics_thop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 19:10:24.000000 ultralytics_thop-0.0.3/ultralytics_thop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 19:10:24.000000 ultralytics_thop-0.0.3/ultralytics_thop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-31 19:10:24.000000 ultralytics_thop-0.0.3/ultralytics_thop.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:00:40.938287 ultralytics_thop-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-31 19:59:41.000000 ultralytics_thop-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-05-31 20:00:40.938287 ultralytics_thop-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-05-31 19:59:41.000000 ultralytics_thop-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-31 19:59:41.000000 ultralytics_thop-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:00:40.938287 ultralytics_thop-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:00:40.934287 ultralytics_thop-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-31 19:59:41.000000 ultralytics_thop-0.2.3/tests/test_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-31 19:59:41.000000 ultralytics_thop-0.2.3/tests/test_matmul.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-31 19:59:41.000000 ultralytics_thop-0.2.3/tests/test_relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-31 19:59:41.000000 ultralytics_thop-0.2.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:00:40.934287 ultralytics_thop-0.2.3/thop/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-31 19:59:41.000000 ultralytics_thop-0.2.3/thop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-05-31 19:59:41.000000 ultralytics_thop-0.2.3/thop/fx_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-31 19:59:41.000000 ultralytics_thop-0.2.3/thop/onnx_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-05-31 19:59:41.000000 ultralytics_thop-0.2.3/thop/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-05-31 19:59:41.000000 ultralytics_thop-0.2.3/thop/rnn_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-31 19:59:41.000000 ultralytics_thop-0.2.3/thop/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:00:40.938287 ultralytics_thop-0.2.3/thop/vision/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 19:59:41.000000 ultralytics_thop-0.2.3/thop/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-31 19:59:41.000000 ultralytics_thop-0.2.3/thop/vision/basic_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-31 19:59:41.000000 ultralytics_thop-0.2.3/thop/vision/calc_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-31 19:59:41.000000 ultralytics_thop-0.2.3/thop/vision/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13298 2024-05-31 19:59:41.000000 ultralytics_thop-0.2.3/thop/vision/onnx_counter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:00:40.938287 ultralytics_thop-0.2.3/ultralytics_thop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-05-31 20:00:40.000000 ultralytics_thop-0.2.3/ultralytics_thop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-31 20:00:40.000000 ultralytics_thop-0.2.3/ultralytics_thop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:00:40.000000 ultralytics_thop-0.2.3/ultralytics_thop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-31 20:00:40.000000 ultralytics_thop-0.2.3/ultralytics_thop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-31 20:00:40.000000 ultralytics_thop-0.2.3/ultralytics_thop.egg-info/top_level.txt
```

### Comparing `ultralytics_thop-0.0.3/LICENSE` & `ultralytics_thop-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.3/README.md` & `ultralytics_thop-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.3/pyproject.toml` & `ultralytics_thop-0.2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -21,25 +21,25 @@
 
 [build-system]
 requires = ["setuptools>=57.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ultralytics-thop"
-version = "0.0.3"  # Placeholder version, needs to be dynamically set
-description = "A tool to count the FLOPs of PyTorch model."
+dynamic = ["version"]
+description = "Ultralytics THOP package for fast computation of PyTorch model FLOPs and parameters."
 readme = "README.md"
 requires-python = ">=3.8"
-license = { file = "LICENSE" }
+license = { "text" = "AGPL-3.0" }
 keywords = ["FLOPs", "PyTorch", "Model Analysis"]  # Optional
 authors = [
     { name = "Ligeng Zhu", email = "ligeng.zhu+github@gmail.com" }
 ]
 maintainers = [
-    { name = "Ligeng Zhu", email = "ligeng.zhu+github@gmail.com" }
+    { name = "Glenn Jocher" },
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
@@ -53,19 +53,18 @@
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
 ]
 dependencies = [
-    "packaging",
+    "numpy",
     "torch",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/ultralytics/thop"
-
-[tool.setuptools]
-package-data = { "thop" = ["__version__.py"] }
+"Bug Reports" = "https://github.com/ultralytics/thop/issues"
+"Funding" = "https://ultralytics.com"
+"Source" = "https://github.com/ultralytics/thop/"
 
 [tool.setuptools.dynamic]
-version = { attr = "thop.__version__.VERSION" }
+version = { attr = "thop.__version__" }
```

### Comparing `ultralytics_thop-0.0.3/tests/test_conv2d.py` & `ultralytics_thop-0.2.3/tests/test_conv2d.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.3/tests/test_matmul.py` & `ultralytics_thop-0.2.3/tests/test_matmul.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.3/tests/test_utils.py` & `ultralytics_thop-0.2.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.3/thop/fx_profile.py` & `ultralytics_thop-0.2.3/thop/fx_profile.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.3/thop/onnx_profile.py` & `ultralytics_thop-0.2.3/thop/onnx_profile.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.3/thop/profile.py` & `ultralytics_thop-0.2.3/thop/profile.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,14 @@
-from packaging.version import Version
-
 from thop.rnn_hooks import *
 from thop.vision.basic_hooks import *
 
 # logger = logging.getLogger(__name__)
 # logger.setLevel(logging.INFO)
 from .utils import prGreen, prRed, prYellow
 
-if Version(torch.__version__) < Version("1.0.0"):
-    logging.warning(
-        "You are using an old version PyTorch {version}, which THOP does NOT support.".format(version=torch.__version__)
-    )
-
 default_dtype = torch.float64
 
 register_hooks = {
     nn.ZeroPad2d: zero_ops,  # padding does not involve any multiplication.
     nn.Conv1d: count_convNd,
     nn.Conv2d: count_convNd,
     nn.Conv3d: count_convNd,
@@ -55,19 +48,17 @@
     nn.GRUCell: count_gru_cell,
     nn.LSTMCell: count_lstm_cell,
     nn.RNN: count_rnn,
     nn.GRU: count_gru,
     nn.LSTM: count_lstm,
     nn.Sequential: zero_ops,
     nn.PixelShuffle: zero_ops,
+    nn.SyncBatchNorm: count_normalization,
 }
 
-if Version(torch.__version__) >= Version("1.1.0"):
-    register_hooks.update({nn.SyncBatchNorm: count_normalization})
-
 
 def profile_origin(model, inputs, custom_ops=None, verbose=True, report_missing=False):
     """Profiles a PyTorch model's operations and parameters by applying custom or default hooks and returns total
     operations and parameters.
     """
     handler_collection = []
     types_collection = set()
@@ -94,22 +85,22 @@
 
         m_type = type(m)
 
         fn = None
         if m_type in custom_ops:  # if defined both op maps, use custom_ops to overwrite.
             fn = custom_ops[m_type]
             if m_type not in types_collection and verbose:
-                print("[INFO] Customize rule %s() %s." % (fn.__qualname__, m_type))
+                print(f"[INFO] Customize rule {fn.__qualname__}() {m_type}.")
         elif m_type in register_hooks:
             fn = register_hooks[m_type]
             if m_type not in types_collection and verbose:
-                print("[INFO] Register %s() for %s." % (fn.__qualname__, m_type))
+                print(f"[INFO] Register {fn.__qualname__}() for {m_type}.")
         else:
             if m_type not in types_collection and report_missing:
-                prRed("[WARN] Cannot find rule for %s. Treat it as zero Macs and zero Params." % m_type)
+                prRed(f"[WARN] Cannot find rule for {m_type}. Treat it as zero Macs and zero Params.")
 
         if fn is not None:
             handler = m.register_forward_hook(fn)
             handler_collection.append(handler)
         types_collection.add(m_type)
 
     training = model.training
@@ -175,22 +166,22 @@
         m_type = type(m)
 
         fn = None
         if m_type in custom_ops:
             # if defined both op maps, use custom_ops to overwrite.
             fn = custom_ops[m_type]
             if m_type not in types_collection and verbose:
-                print("[INFO] Customize rule %s() %s." % (fn.__qualname__, m_type))
+                print(f"[INFO] Customize rule {fn.__qualname__}() {m_type}.")
         elif m_type in register_hooks:
             fn = register_hooks[m_type]
             if m_type not in types_collection and verbose:
-                print("[INFO] Register %s() for %s." % (fn.__qualname__, m_type))
+                print(f"[INFO] Register {fn.__qualname__}() for {m_type}.")
         else:
             if m_type not in types_collection and report_missing:
-                prRed("[WARN] Cannot find rule for %s. Treat it as zero Macs and zero Params." % m_type)
+                prRed(f"[WARN] Cannot find rule for {m_type}. Treat it as zero Macs and zero Params.")
 
         if fn is not None:
             handler_collection[m] = (
                 m.register_forward_hook(fn),
                 m.register_forward_hook(count_parameters),
             )
         types_collection.add(m_type)
```

### Comparing `ultralytics_thop-0.0.3/thop/rnn_hooks.py` & `ultralytics_thop-0.2.3/thop/rnn_hooks.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.3/thop/utils.py` & `ultralytics_thop-0.2.3/thop/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.3/thop/vision/basic_hooks.py` & `ultralytics_thop-0.2.3/thop/vision/basic_hooks.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.3/thop/vision/calc_func.py` & `ultralytics_thop-0.2.3/thop/vision/calc_func.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.3/thop/vision/onnx_counter.py` & `ultralytics_thop-0.2.3/thop/vision/onnx_counter.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.3/ultralytics_thop.egg-info/SOURCES.txt` & `ultralytics_thop-0.2.3/ultralytics_thop.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 README.md
 pyproject.toml
 tests/test_conv2d.py
 tests/test_matmul.py
 tests/test_relu.py
 tests/test_utils.py
 thop/__init__.py
-thop/__version__.py
 thop/fx_profile.py
 thop/onnx_profile.py
 thop/profile.py
 thop/rnn_hooks.py
 thop/utils.py
 thop/vision/__init__.py
 thop/vision/basic_hooks.py
```

