# Comparing `tmp/evomip-0.1.1.tar.gz` & `tmp/evomip-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evomip-0.1.1.tar", max compression
+gzip compressed data, was "evomip-0.1.2.tar", max compression
```

## Comparing `evomip-0.1.1.tar` & `evomip-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1063 2024-05-31 08:41:03.560634 evomip-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2024-05-31 08:26:16.289146 evomip-0.1.1/README.md
--rw-r--r--   0        0        0     2718 2024-05-31 08:27:45.937293 evomip-0.1.1/evomip/Algorithm.py
--rw-r--r--   0        0        0     3234 2024-05-31 08:27:54.171024 evomip-0.1.1/evomip/Config.py
--rw-r--r--   0        0        0      310 2024-05-31 08:27:54.171723 evomip-0.1.1/evomip/Constraint.py
--rw-r--r--   0        0        0      988 2024-05-31 08:28:13.804246 evomip-0.1.1/evomip/Individual.py
--rw-r--r--   0        0        0     1628 2024-05-31 08:28:01.173012 evomip-0.1.1/evomip/Parameter.py
--rw-r--r--   0        0        0     9484 2024-05-31 08:28:01.174802 evomip-0.1.1/evomip/Population.py
--rw-r--r--   0        0        0     2252 2024-05-31 08:28:05.625620 evomip-0.1.1/evomip/SearchSpace.py
--rw-r--r--   0        0        0     5166 2024-05-31 08:28:22.623824 evomip-0.1.1/evomip/WOA.py
--rw-r--r--   0        0        0        0 2024-05-31 08:26:16.289106 evomip-0.1.1/evomip/__init__.py
--rw-r--r--   0        0        0      270 2024-05-31 08:44:05.354067 evomip-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      289 1970-01-01 00:00:00.000000 evomip-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-31 08:41:03.560634 evomip-0.1.2/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-31 08:26:16.289146 evomip-0.1.2/README.md
+-rw-r--r--   0        0        0     2718 2024-05-31 08:27:45.937293 evomip-0.1.2/evomip/Algorithm.py
+-rw-r--r--   0        0        0     3234 2024-05-31 08:27:54.171024 evomip-0.1.2/evomip/Config.py
+-rw-r--r--   0        0        0      310 2024-05-31 08:27:54.171723 evomip-0.1.2/evomip/Constraint.py
+-rw-r--r--   0        0        0      988 2024-05-31 08:28:13.804246 evomip-0.1.2/evomip/Individual.py
+-rw-r--r--   0        0        0     1628 2024-05-31 08:28:01.173012 evomip-0.1.2/evomip/Parameter.py
+-rw-r--r--   0        0        0     9484 2024-05-31 08:28:01.174802 evomip-0.1.2/evomip/Population.py
+-rw-r--r--   0        0        0     2266 2024-05-31 08:48:46.786358 evomip-0.1.2/evomip/SearchSpace.py
+-rw-r--r--   0        0        0     5166 2024-05-31 08:28:22.623824 evomip-0.1.2/evomip/WOA.py
+-rw-r--r--   0        0        0        0 2024-05-31 08:26:16.289106 evomip-0.1.2/evomip/__init__.py
+-rw-r--r--   0        0        0      270 2024-05-31 08:50:23.684236 evomip-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      289 1970-01-01 00:00:00.000000 evomip-0.1.2/PKG-INFO
```

### Comparing `evomip-0.1.1/LICENSE` & `evomip-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `evomip-0.1.1/evomip/Algorithm.py` & `evomip-0.1.2/evomip/Algorithm.py`

 * *Files identical despite different names*

### Comparing `evomip-0.1.1/evomip/Config.py` & `evomip-0.1.2/evomip/Config.py`

 * *Files identical despite different names*

### Comparing `evomip-0.1.1/evomip/Individual.py` & `evomip-0.1.2/evomip/Individual.py`

 * *Files identical despite different names*

### Comparing `evomip-0.1.1/evomip/Parameter.py` & `evomip-0.1.2/evomip/Parameter.py`

 * *Files identical despite different names*

### Comparing `evomip-0.1.1/evomip/Population.py` & `evomip-0.1.2/evomip/Population.py`

 * *Files identical despite different names*

### Comparing `evomip-0.1.1/evomip/SearchSpace.py` & `evomip-0.1.2/evomip/SearchSpace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from Parameter import *
-from Constraint import *
+from evomip.Parameter import *
+from evomip.Constraint import *
 import random
 import numpy
 
 class SearchSpace: 
 
     #_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/
     def __init__(self, parameters: list[Parameter], constraints: list[Constraint] = []) -> None:
```

### Comparing `evomip-0.1.1/evomip/WOA.py` & `evomip-0.1.2/evomip/WOA.py`

 * *Files identical despite different names*

