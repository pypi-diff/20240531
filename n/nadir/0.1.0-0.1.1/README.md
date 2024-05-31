# Comparing `tmp/nadir-0.1.0.tar.gz` & `tmp/nadir-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadir-0.1.0.tar", last modified: Sat Apr 29 19:59:51 2023, max compression
+gzip compressed data, was "nadir-0.1.1.tar", last modified: Fri May 31 16:08:06 2024, max compression
```

## Comparing `nadir-0.1.0.tar` & `nadir-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxr-x   0 ec3dev    (1001) ec3dev    (1001)        0 2023-04-29 19:59:51.316702 nadir-0.1.0/
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)    11344 2023-03-04 17:09:02.000000 nadir-0.1.0/LICENCE
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     4464 2023-04-29 19:59:51.316702 nadir-0.1.0/PKG-INFO
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     3665 2023-04-29 19:54:16.000000 nadir-0.1.0/README.md
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1006 2023-04-29 19:59:04.000000 nadir-0.1.0/pyproject.toml
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)      791 2023-04-29 19:59:51.320702 nadir-0.1.0/setup.cfg
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)       37 2023-03-04 17:09:02.000000 nadir-0.1.0/setup.py
-drwxrwxr-x   0 ec3dev    (1001) ec3dev    (1001)        0 2023-04-29 19:59:51.300703 nadir-0.1.0/src/
-drwxrwxr-x   0 ec3dev    (1001) ec3dev    (1001)        0 2023-04-29 19:59:51.312703 nadir-0.1.0/src/nadir/
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1065 2023-04-29 19:51:57.000000 nadir-0.1.0/src/nadir/NAG.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1592 2023-04-29 19:59:18.000000 nadir-0.1.0/src/nadir/__init__.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1803 2023-04-29 18:32:39.000000 nadir-0.1.0/src/nadir/adadelta.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1410 2023-03-04 17:17:09.000000 nadir-0.1.0/src/nadir/adagrad.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     3825 2023-04-25 15:23:45.000000 nadir-0.1.0/src/nadir/adam.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1617 2023-04-29 16:39:23.000000 nadir-0.1.0/src/nadir/adamax.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1193 2023-04-29 18:34:17.000000 nadir-0.1.0/src/nadir/adamw.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1201 2023-04-29 18:37:27.000000 nadir-0.1.0/src/nadir/amsgrad.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     2569 2023-04-25 15:16:08.000000 nadir-0.1.0/src/nadir/base.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     2327 2023-04-29 18:47:36.000000 nadir-0.1.0/src/nadir/lion.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1364 2023-04-29 18:56:03.000000 nadir-0.1.0/src/nadir/momentum.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1802 2023-04-29 18:50:06.000000 nadir-0.1.0/src/nadir/radam.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1232 2023-03-04 17:16:03.000000 nadir-0.1.0/src/nadir/rmsprop.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     2454 2023-04-29 19:50:57.000000 nadir-0.1.0/src/nadir/sgd.py
-drwxrwxr-x   0 ec3dev    (1001) ec3dev    (1001)        0 2023-04-29 19:59:51.316702 nadir-0.1.0/src/nadir.egg-info/
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     4464 2023-04-29 19:59:51.000000 nadir-0.1.0/src/nadir.egg-info/PKG-INFO
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)      490 2023-04-29 19:59:51.000000 nadir-0.1.0/src/nadir.egg-info/SOURCES.txt
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)        1 2023-04-29 19:59:51.000000 nadir-0.1.0/src/nadir.egg-info/dependency_links.txt
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)       45 2023-04-29 19:59:51.000000 nadir-0.1.0/src/nadir.egg-info/requires.txt
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)        6 2023-04-29 19:59:51.000000 nadir-0.1.0/src/nadir.egg-info/top_level.txt
+drwxrwxr-x   0 ec3dev    (1001) ec3dev    (1001)        0 2024-05-31 16:08:06.852694 nadir-0.1.1/
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)    11344 2024-05-31 12:32:51.000000 nadir-0.1.1/LICENCE
+-rw-r--r--   0 ec3dev    (1001) ec3dev    (1001)     5943 2024-05-31 16:08:06.852694 nadir-0.1.1/PKG-INFO
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     5037 2024-05-31 12:33:28.000000 nadir-0.1.1/README.md
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1108 2024-05-31 16:02:46.000000 nadir-0.1.1/pyproject.toml
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)       38 2024-05-31 16:08:06.852694 nadir-0.1.1/setup.cfg
+drwxrwxr-x   0 ec3dev    (1001) ec3dev    (1001)        0 2024-05-31 16:08:06.852694 nadir-0.1.1/src/
+drwxrwxr-x   0 ec3dev    (1001) ec3dev    (1001)        0 2024-05-31 16:08:06.852694 nadir-0.1.1/src/nadir/
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1065 2024-05-31 12:32:51.000000 nadir-0.1.1/src/nadir/NAG.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1680 2024-05-31 12:32:51.000000 nadir-0.1.1/src/nadir/__init__.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1501 2024-05-31 12:32:51.000000 nadir-0.1.1/src/nadir/adabelief.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1803 2024-05-31 12:32:51.000000 nadir-0.1.1/src/nadir/adadelta.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1410 2024-05-31 12:32:51.000000 nadir-0.1.1/src/nadir/adagrad.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     4382 2024-05-31 12:32:51.000000 nadir-0.1.1/src/nadir/adam.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1617 2024-05-31 12:32:51.000000 nadir-0.1.1/src/nadir/adamax.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1193 2024-05-31 12:32:51.000000 nadir-0.1.1/src/nadir/adamw.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1201 2024-05-31 12:32:51.000000 nadir-0.1.1/src/nadir/amsgrad.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     2569 2024-05-31 12:32:51.000000 nadir-0.1.1/src/nadir/base.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     2327 2024-05-31 12:32:51.000000 nadir-0.1.1/src/nadir/lion.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1364 2024-05-31 12:32:51.000000 nadir-0.1.1/src/nadir/momentum.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)      976 2024-05-31 12:32:51.000000 nadir-0.1.1/src/nadir/nadam.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1775 2024-05-31 15:07:20.000000 nadir-0.1.1/src/nadir/radam.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1232 2024-05-31 12:32:51.000000 nadir-0.1.1/src/nadir/rmsprop.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     2454 2024-05-31 12:32:51.000000 nadir-0.1.1/src/nadir/sgd.py
+drwxrwxr-x   0 ec3dev    (1001) ec3dev    (1001)        0 2024-05-31 16:08:06.852694 nadir-0.1.1/src/nadir.egg-info/
+-rw-r--r--   0 ec3dev    (1001) ec3dev    (1001)     5943 2024-05-31 16:08:06.000000 nadir-0.1.1/src/nadir.egg-info/PKG-INFO
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)      513 2024-05-31 16:08:06.000000 nadir-0.1.1/src/nadir.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)        1 2024-05-31 16:08:06.000000 nadir-0.1.1/src/nadir.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)       53 2024-05-31 16:08:06.000000 nadir-0.1.1/src/nadir.egg-info/requires.txt
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)        6 2024-05-31 16:08:06.000000 nadir-0.1.1/src/nadir.egg-info/top_level.txt
```

### Comparing `nadir-0.1.0/LICENCE` & `nadir-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `nadir-0.1.0/PKG-INFO` & `nadir-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,47 @@
-Metadata-Version: 2.1
-Name: nadir
-Version: 0.1.0
-Summary: Nadir is a library of bleeding-edge DL optimisers built for speed and functionality in PyTorch for researchers
-Author-email: Bhavnick Minhas <bhavnicksm@gmail.com>
-Maintainer-email: Bhavnick Minhas <bhavnicksm@gmail.com>
-License: Apache 2.0
-Project-URL: Homepage, https://github.com/Dawn-Of-Eve/nadir
-Project-URL: Bug Tracker, https://github.com/Dawn-Of-Eve/nadir/issues
-Keywords: machine learning,optimization,adam-optimizer
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
 ![NADIRbanner2](https://user-images.githubusercontent.com/11348086/221370644-fcc05274-eb99-4237-a270-60dafd5ab69d.png)
 
 # Nadir
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/nadir)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/Dawn-Of-Eve/nadir)
 ![GitHub Repo stars](https://img.shields.io/github/stars/Dawn-Of-Eve/nadir?style=social)
-![Twitter Follow](https://img.shields.io/twitter/follow/dawnofevehq?style=social)
 
 **Nadir** (pronounced _nay-di-ah_) is derived from the arabic word _nazir_, and means "the lowest point of a space". In optimisation problems, it is equivalent to the point of minimum. If you are a machine learning enthusiast, a data scientist or an AI practitioner, you know how important it is to use the best optimization algorithms to train your models. The purpose of this library is to help optimize machine learning models and enable them to reach the point of nadir in the appropriate context.
 
-PyTorch is a popular machine learning framework that provides a flexible and efficient way of building and training deep neural networks. This library, Nadir, is built on top of PyTorch to provide high-performing general-purpose optimisation algorithms.  
+**Nadir** follows the principles of Simplicity, Modularity and Composabilty. Read more in the [Core Philosophy](#core-philosophy) section. 
 
-# Table of Contents
+## Table of Contents
 
 - [Nadir](#nadir)
 - [Table of Contents](#table-of-contents)
 - [Installation](#installation)
 - [Simple Usage](#simple-usage)
+- [Core Philosphy](#core-philosophy)
 - [Supported Optimisers](#supported-optimisers)
 - [Acknowledgements](#acknowledgements)
 - [Citation](#citation)
 
 
 
-# Installation
+## Installation
 
 You can either choose to install from the PyPI index, in the following manner:
 
 ```bash
 $ pip install nadir
 ```
 or install from source, in the following manner:
 
 ```bash
 $ pip install git+https://github.com/Dawn-Of-Eve/nadir.git
 ```
 **Note:** Installing from source might lead to a breaking package. It is recommended that you install from PyPI itself.
 
-# Simple Usage
+## Simple Usage
 
 ```python
 import nadir as nd
 
 # some model setup here...
 model = ...
 
@@ -67,37 +49,51 @@
 config = nd.SGDConfig(lr=learning_rate)
 optimizer = nd.SGD(model.parameters(), config)
 
 # Call the optimizer step
 optimizer.step()
 ```
 
-# Supported Optimisers
+## Core Philosophy
+
+`Nadir` was built to provide a sense of uniformity and integration that might be lacking in the optimisation community, based on the simple idea that optimisers are not islands. They are usually inheriting characteristics from other optimisers and they provide inspiration to other optimisers. So why not make optimisers inheritable, composible and modular objects? 
+
+The core concepts that each optimiser in `Nadir` follows are:
+
+1. **Simplicity** is of key importance. We prefer readability and simplicity over performance. Experiment, test and verify what works and what does not with Nadir. Optimise and write custom fused kernels for your favorite optimisers after, for performance. 
+
+2. **Modularity** means that the each new optimiser should minimise on the extra new logic added by adding or editing only the parts that need editing. If you want to have a different momentum in Adam, you only change the function of Momentum after inheriting Adam. No need to write the entire code from scratch.
+
+3. **Composibility** implies that we can take things from one optimiser and add them to another without much effort. You can build a optimiser that is the mix of RAdam and NAdam with the properties of AdaBelief, if you so desire! That's what makes this library really powerful. 
+
+## Supported Optimisers
 
-| Optimiser 	| Paper 	                                            |
-|:---------:	|:-----:	                                            |
-|  **SGD**  	| https://paperswithcode.com/method/sgd                 |
-|  **Momentum** | https://paperswithcode.com/method/sgd-with-momentum   |
-|  **NAG**      | https://jlmelville.github.io/mize/nesterov.html       |
+| Optimiser 	| Paper 	                                                 |
+|:---------:	|:-----:	                                                 |
+|  **SGD**  	| https://paperswithcode.com/method/sgd                      |
+|  **Momentum** | https://paperswithcode.com/method/sgd-with-momentum        |
+|  **NAG**      | https://jlmelville.github.io/mize/nesterov.html            |
 |  **Adagrad** 	| https://www.jmlr.org/papers/volume12/duchi11a/duchi11a.pdf |
-|  **RMSProp** 	| https://paperswithcode.com/method/rmsprop             |
-|  **Adam**     | https://arxiv.org/abs/1412.6980v9                     |
-|  **Adamax**   | https://arxiv.org/abs/1412.6980v9                     |
-|  **AdamW**    | https://arxiv.org/abs/1711.05101v3                    |
-|  **Adadelta** | https://arxiv.org/abs/1212.5701v1                     |
-|  **AMSGrad**    | https://arxiv.org/abs/1904.09237v1                  |
-|  **RAdam**    | https://arxiv.org/abs/1908.03265v4                    |
-|  **Lion**     | https://arxiv.org/abs/2302.06675                      |
+|  **RMSProp** 	| https://paperswithcode.com/method/rmsprop                  |
+|  **Adam**     | https://arxiv.org/abs/1412.6980v9                          |
+|  **Adamax**   | https://arxiv.org/abs/1412.6980v9                          |
+|  **AdamW**    | https://arxiv.org/abs/1711.05101v3                         |
+|  **Adadelta** | https://arxiv.org/abs/1212.5701v1                          |
+|  **AMSGrad**  | https://arxiv.org/abs/1904.09237v1                         |
+|  **RAdam**    | https://arxiv.org/abs/1908.03265v4                         |
+|  **Lion**     | https://arxiv.org/abs/2302.06675                           |
+|  **AdaBelief**| https://arxiv.org/pdf/2010.07468v5.pdf                     |
+|  **NAdam**    | http://cs229.stanford.edu/proj2015/054_report.pdf          |
 
-# Acknowledgements
+## Acknowledgements
 
 We would like to thank all the amazing contributors of this project who spent so much effort making this repositary awesome! :heart:
 
 
-# Citation
+## Citation
 
 You can use the _Cite this repository_ button provided by Github or use the following bibtex:
 
 ```bibtex
 @software{MinhasNadir,
     title        = {{Nadir: A Library for Bleeding-Edge Optimizers in PyTorch}},
     author       = {Minhas, Bhavnick and Kalathukunnel, Apsal},
```

### Comparing `nadir-0.1.0/pyproject.toml` & `nadir-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nadir"
-version = "0.1.0"
 authors = [
   { name="Bhavnick Minhas", email="bhavnicksm@gmail.com" },
 ]
 maintainers = [
   { name = "Bhavnick Minhas", email="bhavnicksm@gmail.com"},
 ]
-description = "Nadir is a library of bleeding-edge DL optimisers built for speed and functionality in PyTorch for researchers"
+description = "Nadir: Cutting-edge PyTorch optimizers for simplicity & composability! 🔥🚀💻"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Artificial Intelligence"
 ]
 license = { text = "Apache 2.0"}
 dependencies = [
     "torch>=1.13.1",
+]
+dynamic = ["version"]
+
+[project.optional-dependencies]
+test = [
     "torchvision>=0.14.1",
     "tqdm",
     "wandb"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/Dawn-Of-Eve/nadir"
-"Bug Tracker" = "https://github.com/Dawn-Of-Eve/nadir/issues"
-
+"Homepage" = "https://github.com/OptimalFoundation/nadir"
+"Bug Tracker" = "https://github.com/OptimalFoundation/nadir/issues"
 
 [tools.setuptools]
 packages = ["nadir"]
-package-dir = {"" = "src"}
+package-dir = {"" = "src"}
+
+[tool.setuptools.dynamic]
+version = {  attr = "nadir.__version__" }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nadir-0.1.0/src/nadir/NAG.py` & `nadir-0.1.1/src/nadir/NAG.py`

 * *Files identical despite different names*

### Comparing `nadir-0.1.0/src/nadir/__init__.py` & `nadir-0.1.1/src/nadir/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from .lion import Lion, LionConfig
 from .momentum import Momentum, MomentumConfig
 from .rmsprop import RMSProp, RMSPropConfig
 from .radam import Radam, RadamConfig
 from .sgd import SGD, SGDConfig
 
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 __all__ = ('Adadelta',
            'AdadeltaConfig',
            'Adagrad',
            'AdagradConfig',
            'Adam',
            'AdamConfig',
@@ -41,13 +41,17 @@
            'Adam' 
            'BaseOptimizer',
            'BaseConfig',
            'Lion',
            'LionConfig',
            'Momentum',
            'MomentumConfig',
+           'Nadam',
+           'NadamConfig',
+           'NAG',
+           'NAGConfig',
            'RMSProp',
            'RMSPropConfig',
            'Radam',
            'RadamConfig',
            'SGD',
            'SGDConfig')
```

### Comparing `nadir-0.1.0/src/nadir/adadelta.py` & `nadir-0.1.1/src/nadir/adadelta.py`

 * *Files identical despite different names*

### Comparing `nadir-0.1.0/src/nadir/adagrad.py` & `nadir-0.1.1/src/nadir/adagrad.py`

 * *Files identical despite different names*

### Comparing `nadir-0.1.0/src/nadir/adam.py` & `nadir-0.1.1/src/nadir/adam.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 class AdamConfig(BaseConfig):
   lr : float = 3E-4
   beta_1 : float = 0.9
   beta_2 : float = 0.999
   eps : float = 1E-8
   weight_decay : float = 0.0
   amsgrad : bool = False
+  nesterov : bool = False
   bias_correction: bool = True
 
 class Adam(BaseOptimizer):
 
   def __init__(self, params, config : AdamConfig = AdamConfig()):
     if not 1 >= config.beta_1 >= 0:
       raise ValueError(f"Invalid value for beta_1 in config: {config.beta_1} ", 
@@ -57,14 +58,39 @@
     
     if 1 >= self.config.beta_2 > 0:
       state['adaptivity'] = torch.zeros_like(param, memory_format=torch.preserve_format)
       
       if self.config.amsgrad:
         state['amsgrad'] = torch.zeros_like(param, memory_format=torch.preserve_format)
 
+  def nesterov(momentum):
+
+    def __momentum__(self, state, grad):
+      m = momentum(self, state, grad)
+      
+      if self.config.nesterov:
+        beta = self.config.beta_1
+        step = state['step']
+
+        if step > 0:
+          if self.config.bias_correction:
+            grad_hat = grad.mul(1-beta).div(1 - beta ** (step))
+          else:
+            grad_hat = grad
+          n = m.mul(beta).add_(grad_hat)
+        else:
+          n = grad
+    
+        return n
+
+      return m
+
+    return __momentum__
+  
+  @nesterov
   def momentum(self,
                state, 
                grad):
     step = state['step']
     m = state['momentum']
     beta_1 = self.config.beta_1
     bias_correction = self.config.bias_correction
```

### Comparing `nadir-0.1.0/src/nadir/adamax.py` & `nadir-0.1.1/src/nadir/adamax.py`

 * *Files identical despite different names*

### Comparing `nadir-0.1.0/src/nadir/adamw.py` & `nadir-0.1.1/src/nadir/adamw.py`

 * *Files identical despite different names*

### Comparing `nadir-0.1.0/src/nadir/amsgrad.py` & `nadir-0.1.1/src/nadir/amsgrad.py`

 * *Files identical despite different names*

### Comparing `nadir-0.1.0/src/nadir/base.py` & `nadir-0.1.1/src/nadir/base.py`

 * *Files identical despite different names*

### Comparing `nadir-0.1.0/src/nadir/lion.py` & `nadir-0.1.1/src/nadir/lion.py`

 * *Files identical despite different names*

### Comparing `nadir-0.1.0/src/nadir/momentum.py` & `nadir-0.1.1/src/nadir/momentum.py`

 * *Files identical despite different names*

### Comparing `nadir-0.1.0/src/nadir/radam.py` & `nadir-0.1.1/src/nadir/radam.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,30 +13,28 @@
 # limitations under the License.
 from typing import Dict, Any, Optional
 from dataclasses import dataclass
 
 import torch
 import math
 
-from .base import BaseOptimizer
-from .base import BaseConfig
-
+from .adam import Adam, AdamConfig
 
 __all__ = ['RadamConfig', 'Radam']
 
 @dataclass
 class RadamConfig(AdamConfig):
   lr : float = 3E-4
   beta_1 : float = 0.9
   beta_2 : float = 0.99
   eps : float = 1E-8
   weight_decay : float = 0.
 
 class Radam(Adam):
-  def __init__ (self, params, config : LionConfig = LionConfig()):
+  def __init__ (self, params, config : AdamConfig = AdamConfig()):
     super().__init__(params, config)
     self.config = config
 
   def update(self, state, group, grad, param):
     lr = group['lr']
     beta_2 = self.config.beta_2
     step = state['step']
```

### Comparing `nadir-0.1.0/src/nadir/rmsprop.py` & `nadir-0.1.1/src/nadir/rmsprop.py`

 * *Files identical despite different names*

### Comparing `nadir-0.1.0/src/nadir/sgd.py` & `nadir-0.1.1/src/nadir/sgd.py`

 * *Files identical despite different names*

### Comparing `nadir-0.1.0/src/nadir.egg-info/PKG-INFO` & `nadir-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,69 @@
 Metadata-Version: 2.1
 Name: nadir
-Version: 0.1.0
-Summary: Nadir is a library of bleeding-edge DL optimisers built for speed and functionality in PyTorch for researchers
+Version: 0.1.1
+Summary: Nadir: Cutting-edge PyTorch optimizers for simplicity & composability! 🔥🚀💻
 Author-email: Bhavnick Minhas <bhavnicksm@gmail.com>
 Maintainer-email: Bhavnick Minhas <bhavnicksm@gmail.com>
 License: Apache 2.0
-Project-URL: Homepage, https://github.com/Dawn-Of-Eve/nadir
-Project-URL: Bug Tracker, https://github.com/Dawn-Of-Eve/nadir/issues
-Keywords: machine learning,optimization,adam-optimizer
+Project-URL: Homepage, https://github.com/OptimalFoundation/nadir
+Project-URL: Bug Tracker, https://github.com/OptimalFoundation/nadir/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
+Requires-Dist: torch>=1.13.1
+Provides-Extra: test
+Requires-Dist: torchvision>=0.14.1; extra == "test"
+Requires-Dist: tqdm; extra == "test"
+Requires-Dist: wandb; extra == "test"
 
 ![NADIRbanner2](https://user-images.githubusercontent.com/11348086/221370644-fcc05274-eb99-4237-a270-60dafd5ab69d.png)
 
 # Nadir
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/nadir)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/Dawn-Of-Eve/nadir)
 ![GitHub Repo stars](https://img.shields.io/github/stars/Dawn-Of-Eve/nadir?style=social)
-![Twitter Follow](https://img.shields.io/twitter/follow/dawnofevehq?style=social)
 
 **Nadir** (pronounced _nay-di-ah_) is derived from the arabic word _nazir_, and means "the lowest point of a space". In optimisation problems, it is equivalent to the point of minimum. If you are a machine learning enthusiast, a data scientist or an AI practitioner, you know how important it is to use the best optimization algorithms to train your models. The purpose of this library is to help optimize machine learning models and enable them to reach the point of nadir in the appropriate context.
 
-PyTorch is a popular machine learning framework that provides a flexible and efficient way of building and training deep neural networks. This library, Nadir, is built on top of PyTorch to provide high-performing general-purpose optimisation algorithms.  
+**Nadir** follows the principles of Simplicity, Modularity and Composabilty. Read more in the [Core Philosophy](#core-philosophy) section. 
 
-# Table of Contents
+## Table of Contents
 
 - [Nadir](#nadir)
 - [Table of Contents](#table-of-contents)
 - [Installation](#installation)
 - [Simple Usage](#simple-usage)
+- [Core Philosphy](#core-philosophy)
 - [Supported Optimisers](#supported-optimisers)
 - [Acknowledgements](#acknowledgements)
 - [Citation](#citation)
 
 
 
-# Installation
+## Installation
 
 You can either choose to install from the PyPI index, in the following manner:
 
 ```bash
 $ pip install nadir
 ```
 or install from source, in the following manner:
 
 ```bash
 $ pip install git+https://github.com/Dawn-Of-Eve/nadir.git
 ```
 **Note:** Installing from source might lead to a breaking package. It is recommended that you install from PyPI itself.
 
-# Simple Usage
+## Simple Usage
 
 ```python
 import nadir as nd
 
 # some model setup here...
 model = ...
 
@@ -67,37 +71,51 @@
 config = nd.SGDConfig(lr=learning_rate)
 optimizer = nd.SGD(model.parameters(), config)
 
 # Call the optimizer step
 optimizer.step()
 ```
 
-# Supported Optimisers
+## Core Philosophy
 
-| Optimiser 	| Paper 	                                            |
-|:---------:	|:-----:	                                            |
-|  **SGD**  	| https://paperswithcode.com/method/sgd                 |
-|  **Momentum** | https://paperswithcode.com/method/sgd-with-momentum   |
-|  **NAG**      | https://jlmelville.github.io/mize/nesterov.html       |
+`Nadir` was built to provide a sense of uniformity and integration that might be lacking in the optimisation community, based on the simple idea that optimisers are not islands. They are usually inheriting characteristics from other optimisers and they provide inspiration to other optimisers. So why not make optimisers inheritable, composible and modular objects? 
+
+The core concepts that each optimiser in `Nadir` follows are:
+
+1. **Simplicity** is of key importance. We prefer readability and simplicity over performance. Experiment, test and verify what works and what does not with Nadir. Optimise and write custom fused kernels for your favorite optimisers after, for performance. 
+
+2. **Modularity** means that the each new optimiser should minimise on the extra new logic added by adding or editing only the parts that need editing. If you want to have a different momentum in Adam, you only change the function of Momentum after inheriting Adam. No need to write the entire code from scratch.
+
+3. **Composibility** implies that we can take things from one optimiser and add them to another without much effort. You can build a optimiser that is the mix of RAdam and NAdam with the properties of AdaBelief, if you so desire! That's what makes this library really powerful. 
+
+## Supported Optimisers
+
+| Optimiser 	| Paper 	                                                 |
+|:---------:	|:-----:	                                                 |
+|  **SGD**  	| https://paperswithcode.com/method/sgd                      |
+|  **Momentum** | https://paperswithcode.com/method/sgd-with-momentum        |
+|  **NAG**      | https://jlmelville.github.io/mize/nesterov.html            |
 |  **Adagrad** 	| https://www.jmlr.org/papers/volume12/duchi11a/duchi11a.pdf |
-|  **RMSProp** 	| https://paperswithcode.com/method/rmsprop             |
-|  **Adam**     | https://arxiv.org/abs/1412.6980v9                     |
-|  **Adamax**   | https://arxiv.org/abs/1412.6980v9                     |
-|  **AdamW**    | https://arxiv.org/abs/1711.05101v3                    |
-|  **Adadelta** | https://arxiv.org/abs/1212.5701v1                     |
-|  **AMSGrad**    | https://arxiv.org/abs/1904.09237v1                  |
-|  **RAdam**    | https://arxiv.org/abs/1908.03265v4                    |
-|  **Lion**     | https://arxiv.org/abs/2302.06675                      |
+|  **RMSProp** 	| https://paperswithcode.com/method/rmsprop                  |
+|  **Adam**     | https://arxiv.org/abs/1412.6980v9                          |
+|  **Adamax**   | https://arxiv.org/abs/1412.6980v9                          |
+|  **AdamW**    | https://arxiv.org/abs/1711.05101v3                         |
+|  **Adadelta** | https://arxiv.org/abs/1212.5701v1                          |
+|  **AMSGrad**  | https://arxiv.org/abs/1904.09237v1                         |
+|  **RAdam**    | https://arxiv.org/abs/1908.03265v4                         |
+|  **Lion**     | https://arxiv.org/abs/2302.06675                           |
+|  **AdaBelief**| https://arxiv.org/pdf/2010.07468v5.pdf                     |
+|  **NAdam**    | http://cs229.stanford.edu/proj2015/054_report.pdf          |
 
-# Acknowledgements
+## Acknowledgements
 
 We would like to thank all the amazing contributors of this project who spent so much effort making this repositary awesome! :heart:
 
 
-# Citation
+## Citation
 
 You can use the _Cite this repository_ button provided by Github or use the following bibtex:
 
 ```bibtex
 @software{MinhasNadir,
     title        = {{Nadir: A Library for Bleeding-Edge Optimizers in PyTorch}},
     author       = {Minhas, Bhavnick and Kalathukunnel, Apsal},
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

