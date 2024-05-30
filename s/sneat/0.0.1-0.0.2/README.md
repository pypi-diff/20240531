# Comparing `tmp/sneat-0.0.1.tar.gz` & `tmp/sneat-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sneat-0.0.1.tar", last modified: Thu May 30 23:08:03 2024, max compression
+gzip compressed data, was "sneat-0.0.2.tar", last modified: Thu May 30 23:19:14 2024, max compression
```

## Comparing `sneat-0.0.1.tar` & `sneat-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 bhark     (1000) bhark     (1000)        0 2024-05-30 23:08:03.745775 sneat-0.0.1/
--rw-r--r--   0 bhark     (1000) bhark     (1000)    35149 2024-05-30 22:22:33.000000 sneat-0.0.1/LICENSE
--rw-r--r--   0 bhark     (1000) bhark     (1000)      382 2024-05-30 23:08:03.745775 sneat-0.0.1/PKG-INFO
--rw-r--r--   0 bhark     (1000) bhark     (1000)     3791 2024-05-30 22:51:56.000000 sneat-0.0.1/README.md
--rw-r--r--   0 bhark     (1000) bhark     (1000)       38 2024-05-30 23:08:03.745775 sneat-0.0.1/setup.cfg
--rw-r--r--   0 bhark     (1000) bhark     (1000)      469 2024-05-30 22:58:32.000000 sneat-0.0.1/setup.py
-drwxr-xr-x   0 bhark     (1000) bhark     (1000)        0 2024-05-30 23:08:03.745775 sneat-0.0.1/sneat/
--rw-r--r--   0 bhark     (1000) bhark     (1000)       61 2024-05-30 22:13:55.000000 sneat-0.0.1/sneat/__init__.py
--rw-r--r--   0 bhark     (1000) bhark     (1000)     1376 2024-05-30 22:27:44.000000 sneat-0.0.1/sneat/config.py
--rw-r--r--   0 bhark     (1000) bhark     (1000)     2737 2024-05-30 14:15:17.000000 sneat-0.0.1/sneat/evolve.py
--rw-r--r--   0 bhark     (1000) bhark     (1000)     3084 2024-05-29 17:13:59.000000 sneat-0.0.1/sneat/genome.py
--rw-r--r--   0 bhark     (1000) bhark     (1000)    10559 2024-05-30 13:52:42.000000 sneat-0.0.1/sneat/neuralnetwork.py
--rw-r--r--   0 bhark     (1000) bhark     (1000)      591 2024-05-29 09:31:05.000000 sneat-0.0.1/sneat/normalizer.py
--rw-r--r--   0 bhark     (1000) bhark     (1000)     7327 2024-05-29 20:23:27.000000 sneat-0.0.1/sneat/population.py
--rw-r--r--   0 bhark     (1000) bhark     (1000)      302 2024-05-29 10:55:19.000000 sneat-0.0.1/sneat/species.py
-drwxr-xr-x   0 bhark     (1000) bhark     (1000)        0 2024-05-30 23:08:03.745775 sneat-0.0.1/sneat.egg-info/
--rw-r--r--   0 bhark     (1000) bhark     (1000)      382 2024-05-30 23:08:03.000000 sneat-0.0.1/sneat.egg-info/PKG-INFO
--rw-r--r--   0 bhark     (1000) bhark     (1000)      316 2024-05-30 23:08:03.000000 sneat-0.0.1/sneat.egg-info/SOURCES.txt
--rw-r--r--   0 bhark     (1000) bhark     (1000)        1 2024-05-30 23:08:03.000000 sneat-0.0.1/sneat.egg-info/dependency_links.txt
--rw-r--r--   0 bhark     (1000) bhark     (1000)       75 2024-05-30 23:08:03.000000 sneat-0.0.1/sneat.egg-info/requires.txt
--rw-r--r--   0 bhark     (1000) bhark     (1000)        6 2024-05-30 23:08:03.000000 sneat-0.0.1/sneat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:19:14.311392 sneat-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 23:19:05.000000 sneat-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-30 23:19:14.311392 sneat-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-05-30 23:19:05.000000 sneat-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 23:19:14.311392 sneat-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-30 23:19:05.000000 sneat-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:19:14.311392 sneat-0.0.2/sneat/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-30 23:19:05.000000 sneat-0.0.2/sneat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-30 23:19:05.000000 sneat-0.0.2/sneat/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-30 23:19:05.000000 sneat-0.0.2/sneat/evolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-30 23:19:05.000000 sneat-0.0.2/sneat/genome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10559 2024-05-30 23:19:05.000000 sneat-0.0.2/sneat/neuralnetwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-30 23:19:05.000000 sneat-0.0.2/sneat/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-05-30 23:19:05.000000 sneat-0.0.2/sneat/population.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-30 23:19:05.000000 sneat-0.0.2/sneat/species.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:19:14.311392 sneat-0.0.2/sneat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-30 23:19:14.000000 sneat-0.0.2/sneat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-30 23:19:14.000000 sneat-0.0.2/sneat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 23:19:14.000000 sneat-0.0.2/sneat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-30 23:19:14.000000 sneat-0.0.2/sneat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 23:19:14.000000 sneat-0.0.2/sneat.egg-info/top_level.txt
```

### Comparing `sneat-0.0.1/LICENSE` & `sneat-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sneat-0.0.1/README.md` & `sneat-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sneat-0.0.1/sneat/config.py` & `sneat-0.0.2/sneat/config.py`

 * *Files identical despite different names*

### Comparing `sneat-0.0.1/sneat/evolve.py` & `sneat-0.0.2/sneat/evolve.py`

 * *Files identical despite different names*

### Comparing `sneat-0.0.1/sneat/genome.py` & `sneat-0.0.2/sneat/genome.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from .neuralnetwork import NeuralNetwork
 from .config import get_config
 import numpy as np
 from copy import deepcopy
 import time
-import dill
 import pickle
 
 class Genome:
     def __init__(self, callbacks):
         self.callbacks = callbacks
         self.fitness = 0
         self.normalized_fitness = 0
```

### Comparing `sneat-0.0.1/sneat/neuralnetwork.py` & `sneat-0.0.2/sneat/neuralnetwork.py`

 * *Files identical despite different names*

### Comparing `sneat-0.0.1/sneat/normalizer.py` & `sneat-0.0.2/sneat/normalizer.py`

 * *Files identical despite different names*

### Comparing `sneat-0.0.1/sneat/population.py` & `sneat-0.0.2/sneat/population.py`

 * *Files identical despite different names*

