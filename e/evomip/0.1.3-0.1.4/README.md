# Comparing `tmp/evomip-0.1.3.tar.gz` & `tmp/evomip-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evomip-0.1.3.tar", max compression
+gzip compressed data, was "evomip-0.1.4.tar", max compression
```

## Comparing `evomip-0.1.3.tar` & `evomip-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1063 2024-05-31 08:41:03.560634 evomip-0.1.3/LICENSE
--rw-r--r--   0        0        0        0 2024-05-31 08:26:16.289146 evomip-0.1.3/README.md
--rw-r--r--   0        0        0     2747 2024-05-31 08:55:31.962143 evomip-0.1.3/evomip/Algorithm.py
--rw-r--r--   0        0        0     3234 2024-05-31 08:27:54.171024 evomip-0.1.3/evomip/Config.py
--rw-r--r--   0        0        0      310 2024-05-31 08:27:54.171723 evomip-0.1.3/evomip/Constraint.py
--rw-r--r--   0        0        0     1204 2024-05-31 08:55:13.635100 evomip-0.1.3/evomip/Individual.py
--rw-r--r--   0        0        0     1628 2024-05-31 08:28:01.173012 evomip-0.1.3/evomip/Parameter.py
--rw-r--r--   0        0        0     9529 2024-05-31 08:53:39.528963 evomip-0.1.3/evomip/Population.py
--rw-r--r--   0        0        0     2285 2024-05-31 08:54:49.869990 evomip-0.1.3/evomip/SearchSpace.py
--rw-r--r--   0        0        0     5181 2024-05-31 08:54:57.172388 evomip-0.1.3/evomip/WOA.py
--rw-r--r--   0        0        0        0 2024-05-31 08:26:16.289106 evomip-0.1.3/evomip/__init__.py
--rw-r--r--   0        0        0      270 2024-05-31 08:55:35.240445 evomip-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      289 1970-01-01 00:00:00.000000 evomip-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-31 08:41:03.560634 evomip-0.1.4/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-31 08:26:16.289146 evomip-0.1.4/README.md
+-rw-r--r--   0        0        0     2788 2024-05-31 08:57:14.293405 evomip-0.1.4/evomip/Algorithm.py
+-rw-r--r--   0        0        0     3234 2024-05-31 08:27:54.171024 evomip-0.1.4/evomip/Config.py
+-rw-r--r--   0        0        0      310 2024-05-31 08:27:54.171723 evomip-0.1.4/evomip/Constraint.py
+-rw-r--r--   0        0        0     1204 2024-05-31 08:55:13.635100 evomip-0.1.4/evomip/Individual.py
+-rw-r--r--   0        0        0     1628 2024-05-31 08:28:01.173012 evomip-0.1.4/evomip/Parameter.py
+-rw-r--r--   0        0        0     9529 2024-05-31 08:53:39.528963 evomip-0.1.4/evomip/Population.py
+-rw-r--r--   0        0        0     2285 2024-05-31 08:54:49.869990 evomip-0.1.4/evomip/SearchSpace.py
+-rw-r--r--   0        0        0     5181 2024-05-31 08:54:57.172388 evomip-0.1.4/evomip/WOA.py
+-rw-r--r--   0        0        0        0 2024-05-31 08:26:16.289106 evomip-0.1.4/evomip/__init__.py
+-rw-r--r--   0        0        0      270 2024-05-31 08:57:20.847634 evomip-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      289 1970-01-01 00:00:00.000000 evomip-0.1.4/PKG-INFO
```

### Comparing `evomip-0.1.3/LICENSE` & `evomip-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `evomip-0.1.3/evomip/Algorithm.py` & `evomip-0.1.4/evomip/Algorithm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import math
 from tqdm import tqdm
 from matplotlib import pyplot as plt
 from dataclasses import dataclass
 
 from evomip.Population import Population
 from evomip.Config import Config
+from evomip.Individual import Individual
 
 @dataclass
 class OptResult:
     algo: str
     nIter: int
     popSize: int
     config:  Config
```

### Comparing `evomip-0.1.3/evomip/Config.py` & `evomip-0.1.4/evomip/Config.py`

 * *Files identical despite different names*

### Comparing `evomip-0.1.3/evomip/Individual.py` & `evomip-0.1.4/evomip/Individual.py`

 * *Files identical despite different names*

### Comparing `evomip-0.1.3/evomip/Parameter.py` & `evomip-0.1.4/evomip/Parameter.py`

 * *Files identical despite different names*

### Comparing `evomip-0.1.3/evomip/Population.py` & `evomip-0.1.4/evomip/Population.py`

 * *Files identical despite different names*

### Comparing `evomip-0.1.3/evomip/SearchSpace.py` & `evomip-0.1.4/evomip/SearchSpace.py`

 * *Files identical despite different names*

### Comparing `evomip-0.1.3/evomip/WOA.py` & `evomip-0.1.4/evomip/WOA.py`

 * *Files identical despite different names*

