# Comparing `tmp/ultralytics_thop-0.0.2.tar.gz` & `tmp/ultralytics_thop-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultralytics_thop-0.0.2.tar", last modified: Fri May 31 19:00:18 2024, max compression
+gzip compressed data, was "ultralytics_thop-0.0.3.tar", last modified: Fri May 31 19:10:24 2024, max compression
```

## Comparing `ultralytics_thop-0.0.2.tar` & `ultralytics_thop-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:00:18.703634 ultralytics_thop-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    47843 2024-05-31 19:00:18.703634 ultralytics_thop-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 19:00:18.703634 ultralytics_thop-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:00:18.699634 ultralytics_thop-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/tests/test_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/tests/test_matmul.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/tests/test_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:00:18.699634 ultralytics_thop-0.0.2/thop/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/thop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/thop/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/thop/fx_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/thop/onnx_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/thop/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/thop/rnn_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/thop/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:00:18.699634 ultralytics_thop-0.0.2/thop/vision/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/thop/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/thop/vision/basic_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/thop/vision/calc_func.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/thop/vision/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    13298 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/thop/vision/onnx_counter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:00:18.703634 ultralytics_thop-0.0.2/ultralytics_thop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    47843 2024-05-31 19:00:18.000000 ultralytics_thop-0.0.2/ultralytics_thop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-31 19:00:18.000000 ultralytics_thop-0.0.2/ultralytics_thop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 19:00:18.000000 ultralytics_thop-0.0.2/ultralytics_thop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 19:00:18.000000 ultralytics_thop-0.0.2/ultralytics_thop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-31 19:00:18.000000 ultralytics_thop-0.0.2/ultralytics_thop.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:10:24.217950 ultralytics_thop-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    47915 2024-05-31 19:10:24.217950 ultralytics_thop-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 19:10:24.217950 ultralytics_thop-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:10:24.213950 ultralytics_thop-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/tests/test_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/tests/test_matmul.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/tests/test_relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:10:24.213950 ultralytics_thop-0.0.3/thop/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/thop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/thop/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/thop/fx_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/thop/onnx_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/thop/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/thop/rnn_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/thop/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:10:24.213950 ultralytics_thop-0.0.3/thop/vision/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/thop/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/thop/vision/basic_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/thop/vision/calc_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/thop/vision/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13298 2024-05-31 19:09:19.000000 ultralytics_thop-0.0.3/thop/vision/onnx_counter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:10:24.217950 ultralytics_thop-0.0.3/ultralytics_thop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    47915 2024-05-31 19:10:24.000000 ultralytics_thop-0.0.3/ultralytics_thop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-31 19:10:24.000000 ultralytics_thop-0.0.3/ultralytics_thop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 19:10:24.000000 ultralytics_thop-0.0.3/ultralytics_thop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 19:10:24.000000 ultralytics_thop-0.0.3/ultralytics_thop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-31 19:10:24.000000 ultralytics_thop-0.0.3/ultralytics_thop.egg-info/top_level.txt
```

### Comparing `ultralytics_thop-0.0.2/LICENSE` & `ultralytics_thop-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.2/PKG-INFO` & `ultralytics_thop-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics-thop
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool to count the FLOPs of PyTorch model.
 Author-email: Ligeng Zhu <ligeng.zhu+github@gmail.com>
 Maintainer-email: Ligeng Zhu <ligeng.zhu+github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -684,24 +684,25 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: packaging
 Requires-Dist: torch
 
 <br>
 <img src="https://raw.githubusercontent.com/ultralytics/assets/main/logo/Ultralytics_Logotype_Original.svg" width="320">
 
 # 🚀 THOP: PyTorch-OpCounter
 
 Welcome to the [THOP](https://github.com/ultralytics/thop) repository, your comprehensive solution for profiling PyTorch models by computing the number of Multiply-Accumulate Operations (MACs) and parameters. This tool is essential for deep learning practitioners to evaluate model efficiency and performance.
 
-[![GitHub Actions](https://github.com/ultralytics/thop/actions/workflows/format.yml/badge.svg)](https://github.com/ultralytics/thop/actions/workflows/main.yml) [![PyPI version](https://badge.fury.io/py/ultralytics-.svg)](https://badge.fury.io/py/ultralytics-thop) <a href="https://ultralytics.com/discord"><img alt="Discord" src="https://img.shields.io/discord/1089800235347353640?logo=discord&logoColor=white&label=Discord&color=blue"></a>
+[![GitHub Actions](https://github.com/ultralytics/thop/actions/workflows/format.yml/badge.svg)](https://github.com/ultralytics/thop/actions/workflows/main.yml) [![PyPI version](https://badge.fury.io/py/ultralytics-thop.svg)](https://badge.fury.io/py/ultralytics-thop) <a href="https://ultralytics.com/discord"><img alt="Discord" src="https://img.shields.io/discord/1089800235347353640?logo=discord&logoColor=white&label=Discord&color=blue"></a>
 
 ## 📄 Description
 
 THOP offers an intuitive API to profile PyTorch models by calculating the number of MACs and parameters. This functionality is crucial for assessing the computational efficiency and memory footprint of deep learning models.
 
 ## 📦 Installation
 
@@ -826,21 +827,21 @@
 
 ## 📮 Contact
 
 For bugs or feature requests, please open an issue on [GitHub Issues](https://github.com/ultralytics/thop/issues). Join our community on [Discord](https://ultralytics.com/discord) for discussions and support.
 
 <br>
 <div align="center">
-  <a href="https://github.com/ultralytics/thop"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-github.png" width="3%" alt="THOP GitHub"></a>
+  <a href="https://github.com/ultralytics"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-github.png" width="3%" alt="Ultralytics GitHub"></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="space">
-  <a href="https://www.linkedin.com/company/pytorch/"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-linkedin.png" width="3%" alt="PyTorch LinkedIn"></a>
+  <a href="https://www.linkedin.com/company/ultralytics/"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-linkedin.png" width="3%" alt="Ultralytics LinkedIn"></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="space">
-  <a href="https://twitter.com/pytorch"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-twitter.png" width="3%" alt="PyTorch Twitter"></a>
+  <a href="https://twitter.com/ultralytics"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-twitter.png" width="3%" alt="Ultralytics Twitter"></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="space">
-  <a href="https://youtube.com/pytorch?sub_confirmation=1"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-youtube.png" width="3%" alt="PyTorch YouTube"></a>
+  <a href="https://youtube.com/ultralytics?sub_confirmation=1"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-youtube.png" width="3%" alt="Ultralytics YouTube"></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="space">
-  <a href="https://www.tiktok.com/@pytorch"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-tiktok.png" width="3%" alt="PyTorch TikTok"></a>
+  <a href="https://www.tiktok.com/@ultralytics"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-tiktok.png" width="3%" alt="Ultralytics TikTok"></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="space">
-  <a href="https://www.instagram.com/pytorch/"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-instagram.png" width="3%" alt="PyTorch Instagram"></a>
+  <a href="https://www.instagram.com/ultralytics/"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-instagram.png" width="3%" alt="Ultralytics Instagram"></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="space">
-  <a href="https://discord.com/invite/pytorch"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-discord.png" width="3%" alt="PyTorch Discord"></a>
+  <a href="https://ultralytics.com/discord"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-discord.png" width="3%" alt="Ultralytics Discord"></a>
 </div>
```

### Comparing `ultralytics_thop-0.0.2/README.md` & `ultralytics_thop-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <br>
 <img src="https://raw.githubusercontent.com/ultralytics/assets/main/logo/Ultralytics_Logotype_Original.svg" width="320">
 
 # 🚀 THOP: PyTorch-OpCounter
 
 Welcome to the [THOP](https://github.com/ultralytics/thop) repository, your comprehensive solution for profiling PyTorch models by computing the number of Multiply-Accumulate Operations (MACs) and parameters. This tool is essential for deep learning practitioners to evaluate model efficiency and performance.
 
-[![GitHub Actions](https://github.com/ultralytics/thop/actions/workflows/format.yml/badge.svg)](https://github.com/ultralytics/thop/actions/workflows/main.yml) [![PyPI version](https://badge.fury.io/py/ultralytics-.svg)](https://badge.fury.io/py/ultralytics-thop) <a href="https://ultralytics.com/discord"><img alt="Discord" src="https://img.shields.io/discord/1089800235347353640?logo=discord&logoColor=white&label=Discord&color=blue"></a>
+[![GitHub Actions](https://github.com/ultralytics/thop/actions/workflows/format.yml/badge.svg)](https://github.com/ultralytics/thop/actions/workflows/main.yml) [![PyPI version](https://badge.fury.io/py/ultralytics-thop.svg)](https://badge.fury.io/py/ultralytics-thop) <a href="https://ultralytics.com/discord"><img alt="Discord" src="https://img.shields.io/discord/1089800235347353640?logo=discord&logoColor=white&label=Discord&color=blue"></a>
 
 ## 📄 Description
 
 THOP offers an intuitive API to profile PyTorch models by calculating the number of MACs and parameters. This functionality is crucial for assessing the computational efficiency and memory footprint of deep learning models.
 
 ## 📦 Installation
 
@@ -134,21 +134,21 @@
 
 ## 📮 Contact
 
 For bugs or feature requests, please open an issue on [GitHub Issues](https://github.com/ultralytics/thop/issues). Join our community on [Discord](https://ultralytics.com/discord) for discussions and support.
 
 <br>
 <div align="center">
-  <a href="https://github.com/ultralytics/thop"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-github.png" width="3%" alt="THOP GitHub"></a>
+  <a href="https://github.com/ultralytics"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-github.png" width="3%" alt="Ultralytics GitHub"></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="space">
-  <a href="https://www.linkedin.com/company/pytorch/"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-linkedin.png" width="3%" alt="PyTorch LinkedIn"></a>
+  <a href="https://www.linkedin.com/company/ultralytics/"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-linkedin.png" width="3%" alt="Ultralytics LinkedIn"></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="space">
-  <a href="https://twitter.com/pytorch"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-twitter.png" width="3%" alt="PyTorch Twitter"></a>
+  <a href="https://twitter.com/ultralytics"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-twitter.png" width="3%" alt="Ultralytics Twitter"></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="space">
-  <a href="https://youtube.com/pytorch?sub_confirmation=1"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-youtube.png" width="3%" alt="PyTorch YouTube"></a>
+  <a href="https://youtube.com/ultralytics?sub_confirmation=1"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-youtube.png" width="3%" alt="Ultralytics YouTube"></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="space">
-  <a href="https://www.tiktok.com/@pytorch"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-tiktok.png" width="3%" alt="PyTorch TikTok"></a>
+  <a href="https://www.tiktok.com/@ultralytics"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-tiktok.png" width="3%" alt="Ultralytics TikTok"></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="space">
-  <a href="https://www.instagram.com/pytorch/"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-instagram.png" width="3%" alt="PyTorch Instagram"></a>
+  <a href="https://www.instagram.com/ultralytics/"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-instagram.png" width="3%" alt="Ultralytics Instagram"></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="space">
-  <a href="https://discord.com/invite/pytorch"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-discord.png" width="3%" alt="PyTorch Discord"></a>
+  <a href="https://ultralytics.com/discord"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-discord.png" width="3%" alt="Ultralytics Discord"></a>
 </div>
```

### Comparing `ultralytics_thop-0.0.2/pyproject.toml` & `ultralytics_thop-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 [build-system]
 requires = ["setuptools>=57.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ultralytics-thop"
-version = "0.0.2"  # Placeholder version, needs to be dynamically set
+version = "0.0.3"  # Placeholder version, needs to be dynamically set
 description = "A tool to count the FLOPs of PyTorch model."
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = ["FLOPs", "PyTorch", "Model Analysis"]  # Optional
 authors = [
     { name = "Ligeng Zhu", email = "ligeng.zhu+github@gmail.com" }
@@ -53,14 +53,15 @@
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
 ]
 dependencies = [
+    "packaging",
     "torch",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ultralytics/thop"
 
 [tool.setuptools]
```

### Comparing `ultralytics_thop-0.0.2/tests/test_conv2d.py` & `ultralytics_thop-0.0.3/tests/test_conv2d.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.2/tests/test_matmul.py` & `ultralytics_thop-0.0.3/tests/test_matmul.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.2/tests/test_utils.py` & `ultralytics_thop-0.0.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.2/thop/fx_profile.py` & `ultralytics_thop-0.0.3/thop/fx_profile.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.2/thop/onnx_profile.py` & `ultralytics_thop-0.0.3/thop/onnx_profile.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.2/thop/profile.py` & `ultralytics_thop-0.0.3/thop/profile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from distutils.version import LooseVersion
+from packaging.version import Version
 
 from thop.rnn_hooks import *
 from thop.vision.basic_hooks import *
 
 # logger = logging.getLogger(__name__)
 # logger.setLevel(logging.INFO)
 from .utils import prGreen, prRed, prYellow
 
-if LooseVersion(torch.__version__) < LooseVersion("1.0.0"):
+if Version(torch.__version__) < Version("1.0.0"):
     logging.warning(
         "You are using an old version PyTorch {version}, which THOP does NOT support.".format(version=torch.__version__)
     )
 
 default_dtype = torch.float64
 
 register_hooks = {
@@ -57,15 +57,15 @@
     nn.RNN: count_rnn,
     nn.GRU: count_gru,
     nn.LSTM: count_lstm,
     nn.Sequential: zero_ops,
     nn.PixelShuffle: zero_ops,
 }
 
-if LooseVersion(torch.__version__) >= LooseVersion("1.1.0"):
+if Version(torch.__version__) >= Version("1.1.0"):
     register_hooks.update({nn.SyncBatchNorm: count_normalization})
 
 
 def profile_origin(model, inputs, custom_ops=None, verbose=True, report_missing=False):
     """Profiles a PyTorch model's operations and parameters by applying custom or default hooks and returns total
     operations and parameters.
     """
```

### Comparing `ultralytics_thop-0.0.2/thop/rnn_hooks.py` & `ultralytics_thop-0.0.3/thop/rnn_hooks.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.2/thop/utils.py` & `ultralytics_thop-0.0.3/thop/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.2/thop/vision/basic_hooks.py` & `ultralytics_thop-0.0.3/thop/vision/basic_hooks.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.2/thop/vision/calc_func.py` & `ultralytics_thop-0.0.3/thop/vision/calc_func.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.2/thop/vision/onnx_counter.py` & `ultralytics_thop-0.0.3/thop/vision/onnx_counter.py`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.2/ultralytics_thop.egg-info/PKG-INFO` & `ultralytics_thop-0.0.3/ultralytics_thop.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics-thop
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool to count the FLOPs of PyTorch model.
 Author-email: Ligeng Zhu <ligeng.zhu+github@gmail.com>
 Maintainer-email: Ligeng Zhu <ligeng.zhu+github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -684,24 +684,25 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: packaging
 Requires-Dist: torch
 
 <br>
 <img src="https://raw.githubusercontent.com/ultralytics/assets/main/logo/Ultralytics_Logotype_Original.svg" width="320">
 
 # 🚀 THOP: PyTorch-OpCounter
 
 Welcome to the [THOP](https://github.com/ultralytics/thop) repository, your comprehensive solution for profiling PyTorch models by computing the number of Multiply-Accumulate Operations (MACs) and parameters. This tool is essential for deep learning practitioners to evaluate model efficiency and performance.
 
-[![GitHub Actions](https://github.com/ultralytics/thop/actions/workflows/format.yml/badge.svg)](https://github.com/ultralytics/thop/actions/workflows/main.yml) [![PyPI version](https://badge.fury.io/py/ultralytics-.svg)](https://badge.fury.io/py/ultralytics-thop) <a href="https://ultralytics.com/discord"><img alt="Discord" src="https://img.shields.io/discord/1089800235347353640?logo=discord&logoColor=white&label=Discord&color=blue"></a>
+[![GitHub Actions](https://github.com/ultralytics/thop/actions/workflows/format.yml/badge.svg)](https://github.com/ultralytics/thop/actions/workflows/main.yml) [![PyPI version](https://badge.fury.io/py/ultralytics-thop.svg)](https://badge.fury.io/py/ultralytics-thop) <a href="https://ultralytics.com/discord"><img alt="Discord" src="https://img.shields.io/discord/1089800235347353640?logo=discord&logoColor=white&label=Discord&color=blue"></a>
 
 ## 📄 Description
 
 THOP offers an intuitive API to profile PyTorch models by calculating the number of MACs and parameters. This functionality is crucial for assessing the computational efficiency and memory footprint of deep learning models.
 
 ## 📦 Installation
 
@@ -826,21 +827,21 @@
 
 ## 📮 Contact
 
 For bugs or feature requests, please open an issue on [GitHub Issues](https://github.com/ultralytics/thop/issues). Join our community on [Discord](https://ultralytics.com/discord) for discussions and support.
 
 <br>
 <div align="center">
-  <a href="https://github.com/ultralytics/thop"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-github.png" width="3%" alt="THOP GitHub"></a>
+  <a href="https://github.com/ultralytics"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-github.png" width="3%" alt="Ultralytics GitHub"></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="space">
-  <a href="https://www.linkedin.com/company/pytorch/"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-linkedin.png" width="3%" alt="PyTorch LinkedIn"></a>
+  <a href="https://www.linkedin.com/company/ultralytics/"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-linkedin.png" width="3%" alt="Ultralytics LinkedIn"></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="space">
-  <a href="https://twitter.com/pytorch"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-twitter.png" width="3%" alt="PyTorch Twitter"></a>
+  <a href="https://twitter.com/ultralytics"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-twitter.png" width="3%" alt="Ultralytics Twitter"></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="space">
-  <a href="https://youtube.com/pytorch?sub_confirmation=1"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-youtube.png" width="3%" alt="PyTorch YouTube"></a>
+  <a href="https://youtube.com/ultralytics?sub_confirmation=1"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-youtube.png" width="3%" alt="Ultralytics YouTube"></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="space">
-  <a href="https://www.tiktok.com/@pytorch"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-tiktok.png" width="3%" alt="PyTorch TikTok"></a>
+  <a href="https://www.tiktok.com/@ultralytics"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-tiktok.png" width="3%" alt="Ultralytics TikTok"></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="space">
-  <a href="https://www.instagram.com/pytorch/"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-instagram.png" width="3%" alt="PyTorch Instagram"></a>
+  <a href="https://www.instagram.com/ultralytics/"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-instagram.png" width="3%" alt="Ultralytics Instagram"></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="space">
-  <a href="https://discord.com/invite/pytorch"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-discord.png" width="3%" alt="PyTorch Discord"></a>
+  <a href="https://ultralytics.com/discord"><img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-discord.png" width="3%" alt="Ultralytics Discord"></a>
 </div>
```

### Comparing `ultralytics_thop-0.0.2/ultralytics_thop.egg-info/SOURCES.txt` & `ultralytics_thop-0.0.3/ultralytics_thop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

