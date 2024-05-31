# Comparing `tmp/consensusgen-1.6.tar.gz` & `tmp/consensusgen-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consensusgen-1.6.tar", last modified: Fri May 31 13:24:34 2024, max compression
+gzip compressed data, was "consensusgen-1.7.tar", last modified: Fri May 31 13:39:54 2024, max compression
```

## Comparing `consensusgen-1.6.tar` & `consensusgen-1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:24:34.849056 consensusgen-1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-31 13:24:26.000000 consensusgen-1.6/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:24:26.000000 consensusgen-1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-31 13:24:34.849056 consensusgen-1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-31 13:24:26.000000 consensusgen-1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:24:34.845056 consensusgen-1.6/consensusGen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-31 13:24:34.000000 consensusgen-1.6/consensusGen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-31 13:24:34.000000 consensusgen-1.6/consensusGen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:24:34.000000 consensusgen-1.6/consensusGen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 13:24:34.000000 consensusgen-1.6/consensusGen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-31 13:24:34.000000 consensusgen-1.6/consensusGen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:24:34.845056 consensusgen-1.6/consensusgen/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 13:24:26.000000 consensusgen-1.6/consensusgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-05-31 13:24:26.000000 consensusgen-1.6/consensusgen/consensusGen.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 13:24:34.849056 consensusgen-1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-31 13:24:26.000000 consensusgen-1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:39:54.165601 consensusgen-1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-31 13:39:46.000000 consensusgen-1.7/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:39:46.000000 consensusgen-1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-31 13:39:54.165601 consensusgen-1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-31 13:39:46.000000 consensusgen-1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:39:54.165601 consensusgen-1.7/consensusGen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-31 13:39:54.000000 consensusgen-1.7/consensusGen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-31 13:39:54.000000 consensusgen-1.7/consensusGen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:39:54.000000 consensusgen-1.7/consensusGen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 13:39:54.000000 consensusgen-1.7/consensusGen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-31 13:39:54.000000 consensusgen-1.7/consensusGen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:39:54.165601 consensusgen-1.7/consensusgen/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 13:39:46.000000 consensusgen-1.7/consensusgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-05-31 13:39:46.000000 consensusgen-1.7/consensusgen/consensusGen.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 13:39:54.165601 consensusgen-1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-31 13:39:46.000000 consensusgen-1.7/setup.py
```

### Comparing `consensusgen-1.6/LICENCE.md` & `consensusgen-1.7/LICENCE.md`

 * *Files identical despite different names*

### Comparing `consensusgen-1.6/PKG-INFO` & `consensusgen-1.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consensusGen
-Version: 1.6
+Version: 1.7
 Summary: Genetic algorithm for consensus building
 Home-page: https://pypi.org/project/consensusGen/
 Author: RomainCoulon (Romain Coulon)
 Author-email: <romain.coulon@bipm.org>
 Project-URL: Documentation, https://github.com/RomainCoulon/consensusGen/
 Keywords: genetic algorithm,inter-laboratory comparison,consenus building
 Classifier: Development Status :: 4 - Beta
@@ -21,10 +21,12 @@
 License-File: LICENCE.md
 Requires-Dist: numpy
 Requires-Dist: tqdm
 Requires-Dist: matplotlib
 
 # consensusGen
 
-`consensusGen` is a Python code implementing an genetic algorithm allowing to build a consensus value from measurement results of an inter-laboratory comparison. 
+`consensusGen.py` is a Python code implementing an genetic algorithm allowing to build a consensus value from measurement results of an inter-laboratory comparison. 
+
+Details are provided in [Romain Coulon and Steven Judge 2021 Metrologia 58 065007](https://doi.org/10.1088/1681-7575/ac31c0)
 
 The code is developped and maintained by the BIPM (MIT license).
```

### Comparing `consensusgen-1.6/consensusGen.egg-info/PKG-INFO` & `consensusgen-1.7/consensusGen.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consensusGen
-Version: 1.6
+Version: 1.7
 Summary: Genetic algorithm for consensus building
 Home-page: https://pypi.org/project/consensusGen/
 Author: RomainCoulon (Romain Coulon)
 Author-email: <romain.coulon@bipm.org>
 Project-URL: Documentation, https://github.com/RomainCoulon/consensusGen/
 Keywords: genetic algorithm,inter-laboratory comparison,consenus building
 Classifier: Development Status :: 4 - Beta
@@ -21,10 +21,12 @@
 License-File: LICENCE.md
 Requires-Dist: numpy
 Requires-Dist: tqdm
 Requires-Dist: matplotlib
 
 # consensusGen
 
-`consensusGen` is a Python code implementing an genetic algorithm allowing to build a consensus value from measurement results of an inter-laboratory comparison. 
+`consensusGen.py` is a Python code implementing an genetic algorithm allowing to build a consensus value from measurement results of an inter-laboratory comparison. 
+
+Details are provided in [Romain Coulon and Steven Judge 2021 Metrologia 58 065007](https://doi.org/10.1088/1681-7575/ac31c0)
 
 The code is developped and maintained by the BIPM (MIT license).
```

### Comparing `consensusgen-1.6/consensusgen/consensusGen.py` & `consensusgen-1.7/consensusgen/consensusGen.py`

 * *Files identical despite different names*

### Comparing `consensusgen-1.6/setup.py` & `consensusgen-1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = "1.6"
+VERSION = "1.7"
 
 
 DESCRIPTION = "Genetic algorithm for consensus building"
 
 with open("README.md", "r") as f:
     long_description = f.read()
```

