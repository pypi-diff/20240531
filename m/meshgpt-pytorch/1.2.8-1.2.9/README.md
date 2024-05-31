# Comparing `tmp/meshgpt_pytorch-1.2.8.tar.gz` & `tmp/meshgpt_pytorch-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshgpt_pytorch-1.2.8.tar", last modified: Fri May 17 19:34:38 2024, max compression
+gzip compressed data, was "meshgpt_pytorch-1.2.9.tar", last modified: Fri May 31 18:32:03 2024, max compression
```

## Comparing `meshgpt_pytorch-1.2.8.tar` & `meshgpt_pytorch-1.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:34:38.583101 meshgpt_pytorch-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-17 19:34:34.000000 meshgpt_pytorch-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-17 19:34:38.583101 meshgpt_pytorch-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-05-17 19:34:34.000000 meshgpt_pytorch-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:34:38.583101 meshgpt_pytorch-1.2.8/meshgpt_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-17 19:34:34.000000 meshgpt_pytorch-1.2.8/meshgpt_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-05-17 19:34:34.000000 meshgpt_pytorch-1.2.8/meshgpt_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    50687 2024-05-17 19:34:34.000000 meshgpt_pytorch-1.2.8/meshgpt_pytorch/meshgpt_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-17 19:34:34.000000 meshgpt_pytorch-1.2.8/meshgpt_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 19:34:34.000000 meshgpt_pytorch-1.2.8/meshgpt_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:34:38.583101 meshgpt_pytorch-1.2.8/meshgpt_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-17 19:34:38.000000 meshgpt_pytorch-1.2.8/meshgpt_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-17 19:34:38.000000 meshgpt_pytorch-1.2.8/meshgpt_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 19:34:38.000000 meshgpt_pytorch-1.2.8/meshgpt_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-17 19:34:38.000000 meshgpt_pytorch-1.2.8/meshgpt_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-17 19:34:38.000000 meshgpt_pytorch-1.2.8/meshgpt_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 19:34:38.583101 meshgpt_pytorch-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-17 19:34:34.000000 meshgpt_pytorch-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:32:03.189141 meshgpt_pytorch-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-31 18:31:58.000000 meshgpt_pytorch-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-31 18:32:03.189141 meshgpt_pytorch-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-05-31 18:31:58.000000 meshgpt_pytorch-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:32:03.189141 meshgpt_pytorch-1.2.9/meshgpt_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-31 18:31:58.000000 meshgpt_pytorch-1.2.9/meshgpt_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-05-31 18:31:58.000000 meshgpt_pytorch-1.2.9/meshgpt_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50687 2024-05-31 18:31:58.000000 meshgpt_pytorch-1.2.9/meshgpt_pytorch/meshgpt_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-31 18:31:58.000000 meshgpt_pytorch-1.2.9/meshgpt_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 18:31:58.000000 meshgpt_pytorch-1.2.9/meshgpt_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:32:03.189141 meshgpt_pytorch-1.2.9/meshgpt_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-31 18:32:03.000000 meshgpt_pytorch-1.2.9/meshgpt_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-31 18:32:03.000000 meshgpt_pytorch-1.2.9/meshgpt_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 18:32:03.000000 meshgpt_pytorch-1.2.9/meshgpt_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-31 18:32:03.000000 meshgpt_pytorch-1.2.9/meshgpt_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 18:32:03.000000 meshgpt_pytorch-1.2.9/meshgpt_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 18:32:03.189141 meshgpt_pytorch-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-31 18:31:58.000000 meshgpt_pytorch-1.2.9/setup.py
```

### Comparing `meshgpt_pytorch-1.2.8/LICENSE` & `meshgpt_pytorch-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.8/PKG-INFO` & `meshgpt_pytorch-1.2.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshgpt-pytorch
-Version: 1.2.8
+Version: 1.2.9
 Summary: MeshGPT Pytorch
 Home-page: https://github.com/lucidrains/meshgpt-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanisms,transformers,mesh generation
 Classifier: Development Status :: 4 - Beta
@@ -26,8 +26,8 @@
 Requires-Dist: pytorch-custom-utils>=0.0.9
 Requires-Dist: taylor-series-linear-attention>=0.1.6
 Requires-Dist: torch>=2.1
 Requires-Dist: torch_geometric
 Requires-Dist: torchtyping
 Requires-Dist: tqdm
 Requires-Dist: vector-quantize-pytorch>=1.14.22
-Requires-Dist: x-transformers>=1.29.2
+Requires-Dist: x-transformers>=1.30.4
```

### Comparing `meshgpt_pytorch-1.2.8/README.md` & `meshgpt_pytorch-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.8/meshgpt_pytorch/data.py` & `meshgpt_pytorch-1.2.9/meshgpt_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.8/meshgpt_pytorch/meshgpt_pytorch.py` & `meshgpt_pytorch-1.2.9/meshgpt_pytorch/meshgpt_pytorch.py`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.8/meshgpt_pytorch/trainer.py` & `meshgpt_pytorch-1.2.9/meshgpt_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.8/meshgpt_pytorch.egg-info/PKG-INFO` & `meshgpt_pytorch-1.2.9/meshgpt_pytorch.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshgpt-pytorch
-Version: 1.2.8
+Version: 1.2.9
 Summary: MeshGPT Pytorch
 Home-page: https://github.com/lucidrains/meshgpt-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanisms,transformers,mesh generation
 Classifier: Development Status :: 4 - Beta
@@ -26,8 +26,8 @@
 Requires-Dist: pytorch-custom-utils>=0.0.9
 Requires-Dist: taylor-series-linear-attention>=0.1.6
 Requires-Dist: torch>=2.1
 Requires-Dist: torch_geometric
 Requires-Dist: torchtyping
 Requires-Dist: tqdm
 Requires-Dist: vector-quantize-pytorch>=1.14.22
-Requires-Dist: x-transformers>=1.29.2
+Requires-Dist: x-transformers>=1.30.4
```

### Comparing `meshgpt_pytorch-1.2.8/setup.py` & `meshgpt_pytorch-1.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     'pytorch-custom-utils>=0.0.9',
     'taylor-series-linear-attention>=0.1.6',
     'torch>=2.1',
     'torch_geometric',
     'torchtyping',
     'tqdm',
     'vector-quantize-pytorch>=1.14.22',
-    'x-transformers>=1.29.2',
+    'x-transformers>=1.30.4',
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
```

