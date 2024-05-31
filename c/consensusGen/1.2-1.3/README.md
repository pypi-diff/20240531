# Comparing `tmp/consensusgen-1.2.tar.gz` & `tmp/consensusgen-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consensusgen-1.2.tar", last modified: Fri May 31 11:48:25 2024, max compression
+gzip compressed data, was "consensusgen-1.3.tar", last modified: Fri May 31 11:57:33 2024, max compression
```

## Comparing `consensusgen-1.2.tar` & `consensusgen-1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:48:25.461360 consensusgen-1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-31 11:48:15.000000 consensusgen-1.2/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:48:15.000000 consensusgen-1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-31 11:48:25.461360 consensusgen-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-31 11:48:15.000000 consensusgen-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:48:25.461360 consensusgen-1.2/consensusGen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-31 11:48:25.000000 consensusgen-1.2/consensusGen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-31 11:48:25.000000 consensusgen-1.2/consensusGen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 11:48:25.000000 consensusgen-1.2/consensusGen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 11:48:25.000000 consensusgen-1.2/consensusGen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-31 11:48:25.000000 consensusgen-1.2/consensusGen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:48:25.461360 consensusgen-1.2/consensusgen/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-31 11:48:15.000000 consensusgen-1.2/consensusgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-05-31 11:48:15.000000 consensusgen-1.2/consensusgen/consensusGen.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 11:48:25.461360 consensusgen-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-31 11:48:15.000000 consensusgen-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:57:33.581230 consensusgen-1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-31 11:57:24.000000 consensusgen-1.3/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:57:24.000000 consensusgen-1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-31 11:57:33.581230 consensusgen-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-31 11:57:24.000000 consensusgen-1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:57:33.581230 consensusgen-1.3/consensusGen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-31 11:57:33.000000 consensusgen-1.3/consensusGen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-31 11:57:33.000000 consensusgen-1.3/consensusGen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 11:57:33.000000 consensusgen-1.3/consensusGen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 11:57:33.000000 consensusgen-1.3/consensusGen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-31 11:57:33.000000 consensusgen-1.3/consensusGen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:57:33.581230 consensusgen-1.3/consensusgen/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 11:57:24.000000 consensusgen-1.3/consensusgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-05-31 11:57:24.000000 consensusgen-1.3/consensusgen/consensusGen.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 11:57:33.581230 consensusgen-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-31 11:57:24.000000 consensusgen-1.3/setup.py
```

### Comparing `consensusgen-1.2/LICENCE.md` & `consensusgen-1.3/LICENCE.md`

 * *Files identical despite different names*

### Comparing `consensusgen-1.2/PKG-INFO` & `consensusgen-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consensusGen
-Version: 1.2
+Version: 1.3
 Summary: Genetic algorithm for consensus building
 Home-page: https://pypi.org/project/consensusGen/
 Author: RomainCoulon (Romain Coulon)
 Author-email: <romain.coulon@bipm.org>
 Project-URL: Documentation, https://github.com/RomainCoulon/consensusGen/
 Keywords: genetic algorithm,inter-laboratory comparison,consenus building
 Classifier: Development Status :: 4 - Beta
```

### Comparing `consensusgen-1.2/consensusGen.egg-info/PKG-INFO` & `consensusgen-1.3/consensusGen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consensusGen
-Version: 1.2
+Version: 1.3
 Summary: Genetic algorithm for consensus building
 Home-page: https://pypi.org/project/consensusGen/
 Author: RomainCoulon (Romain Coulon)
 Author-email: <romain.coulon@bipm.org>
 Project-URL: Documentation, https://github.com/RomainCoulon/consensusGen/
 Keywords: genetic algorithm,inter-laboratory comparison,consenus building
 Classifier: Development Status :: 4 - Beta
```

### Comparing `consensusgen-1.2/consensusgen/consensusGen.py` & `consensusgen-1.3/consensusgen/consensusGen.py`

 * *Files identical despite different names*

### Comparing `consensusgen-1.2/setup.py` & `consensusgen-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = "1.2"
+VERSION = "1.3"
 
 DESCRIPTION = "Genetic algorithm for consensus building"
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
```

