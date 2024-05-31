# Comparing `tmp/evomip-0.1.5.tar.gz` & `tmp/evomip-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evomip-0.1.5.tar", max compression
+gzip compressed data, was "evomip-0.1.6.tar", max compression
```

## Comparing `evomip-0.1.5.tar` & `evomip-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1063 2024-05-31 08:41:03.560634 evomip-0.1.5/LICENSE
--rw-r--r--   0        0        0        0 2024-05-31 08:26:16.289146 evomip-0.1.5/README.md
--rw-r--r--   0        0        0     2827 2024-05-31 08:58:01.782974 evomip-0.1.5/evomip/Algorithm.py
--rw-r--r--   0        0        0     3234 2024-05-31 08:27:54.171024 evomip-0.1.5/evomip/Config.py
--rw-r--r--   0        0        0      310 2024-05-31 08:27:54.171723 evomip-0.1.5/evomip/Constraint.py
--rw-r--r--   0        0        0     1204 2024-05-31 08:55:13.635100 evomip-0.1.5/evomip/Individual.py
--rw-r--r--   0        0        0     1628 2024-05-31 08:28:01.173012 evomip-0.1.5/evomip/Parameter.py
--rw-r--r--   0        0        0     9529 2024-05-31 08:53:39.528963 evomip-0.1.5/evomip/Population.py
--rw-r--r--   0        0        0     2285 2024-05-31 08:54:49.869990 evomip-0.1.5/evomip/SearchSpace.py
--rw-r--r--   0        0        0     5181 2024-05-31 08:54:57.172388 evomip-0.1.5/evomip/WOA.py
--rw-r--r--   0        0        0        0 2024-05-31 08:26:16.289106 evomip-0.1.5/evomip/__init__.py
--rw-r--r--   0        0        0      270 2024-05-31 08:58:07.376227 evomip-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      289 1970-01-01 00:00:00.000000 evomip-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-31 08:41:03.560634 evomip-0.1.6/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-31 08:26:16.289146 evomip-0.1.6/README.md
+-rw-r--r--   0        0        0     2827 2024-05-31 08:58:01.782974 evomip-0.1.6/evomip/Algorithm.py
+-rw-r--r--   0        0        0     3234 2024-05-31 08:27:54.171024 evomip-0.1.6/evomip/Config.py
+-rw-r--r--   0        0        0      310 2024-05-31 08:27:54.171723 evomip-0.1.6/evomip/Constraint.py
+-rw-r--r--   0        0        0     1204 2024-05-31 08:55:13.635100 evomip-0.1.6/evomip/Individual.py
+-rw-r--r--   0        0        0     1628 2024-05-31 08:28:01.173012 evomip-0.1.6/evomip/Parameter.py
+-rw-r--r--   0        0        0     9529 2024-05-31 08:53:39.528963 evomip-0.1.6/evomip/Population.py
+-rw-r--r--   0        0        0     2285 2024-05-31 08:54:49.869990 evomip-0.1.6/evomip/SearchSpace.py
+-rw-r--r--   0        0        0     5222 2024-05-31 08:58:47.947283 evomip-0.1.6/evomip/WOA.py
+-rw-r--r--   0        0        0        0 2024-05-31 08:26:16.289106 evomip-0.1.6/evomip/__init__.py
+-rw-r--r--   0        0        0      270 2024-05-31 08:58:53.192738 evomip-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      289 1970-01-01 00:00:00.000000 evomip-0.1.6/PKG-INFO
```

### Comparing `evomip-0.1.5/LICENSE` & `evomip-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `evomip-0.1.5/evomip/Algorithm.py` & `evomip-0.1.6/evomip/Algorithm.py`

 * *Files identical despite different names*

### Comparing `evomip-0.1.5/evomip/Config.py` & `evomip-0.1.6/evomip/Config.py`

 * *Files identical despite different names*

### Comparing `evomip-0.1.5/evomip/Individual.py` & `evomip-0.1.6/evomip/Individual.py`

 * *Files identical despite different names*

### Comparing `evomip-0.1.5/evomip/Parameter.py` & `evomip-0.1.6/evomip/Parameter.py`

 * *Files identical despite different names*

### Comparing `evomip-0.1.5/evomip/Population.py` & `evomip-0.1.6/evomip/Population.py`

 * *Files identical despite different names*

### Comparing `evomip-0.1.5/evomip/SearchSpace.py` & `evomip-0.1.6/evomip/SearchSpace.py`

 * *Files identical despite different names*

### Comparing `evomip-0.1.5/evomip/WOA.py` & `evomip-0.1.6/evomip/WOA.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from evomip.Algorithm import Algorithm
+from evomip.Population import Population
 
 #_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/
 #_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/
 #_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/
 class WOAPopulation(Population):
     #_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/
     def __init__(self, population: Population) -> None:
```

