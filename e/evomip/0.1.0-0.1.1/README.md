# Comparing `tmp/evomip-0.1.0.tar.gz` & `tmp/evomip-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evomip-0.1.0.tar", max compression
+gzip compressed data, was "evomip-0.1.1.tar", max compression
```

## Comparing `evomip-0.1.0.tar` & `evomip-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0        0 2024-05-31 08:26:16.289146 evomip-0.1.0/README.md
--rw-r--r--   0        0        0     2718 2024-05-31 08:27:45.937293 evomip-0.1.0/evomip/Algorithm.py
--rw-r--r--   0        0        0     3234 2024-05-31 08:27:54.171024 evomip-0.1.0/evomip/Config.py
--rw-r--r--   0        0        0      310 2024-05-31 08:27:54.171723 evomip-0.1.0/evomip/Constraint.py
--rw-r--r--   0        0        0      988 2024-05-31 08:28:13.804246 evomip-0.1.0/evomip/Individual.py
--rw-r--r--   0        0        0     1628 2024-05-31 08:28:01.173011 evomip-0.1.0/evomip/Parameter.py
--rw-r--r--   0        0        0     9484 2024-05-31 08:28:01.174801 evomip-0.1.0/evomip/Population.py
--rw-r--r--   0        0        0     2252 2024-05-31 08:28:05.625620 evomip-0.1.0/evomip/SearchSpace.py
--rw-r--r--   0        0        0     5166 2024-05-31 08:28:22.623824 evomip-0.1.0/evomip/WOA.py
--rw-r--r--   0        0        0        0 2024-05-31 08:26:16.289107 evomip-0.1.0/evomip/__init__.py
--rw-r--r--   0        0        0      270 2024-05-31 08:35:57.572512 evomip-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      289 1970-01-01 00:00:00.000000 evomip-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-31 08:41:03.560634 evomip-0.1.1/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-31 08:26:16.289146 evomip-0.1.1/README.md
+-rw-r--r--   0        0        0     2718 2024-05-31 08:27:45.937293 evomip-0.1.1/evomip/Algorithm.py
+-rw-r--r--   0        0        0     3234 2024-05-31 08:27:54.171024 evomip-0.1.1/evomip/Config.py
+-rw-r--r--   0        0        0      310 2024-05-31 08:27:54.171723 evomip-0.1.1/evomip/Constraint.py
+-rw-r--r--   0        0        0      988 2024-05-31 08:28:13.804246 evomip-0.1.1/evomip/Individual.py
+-rw-r--r--   0        0        0     1628 2024-05-31 08:28:01.173012 evomip-0.1.1/evomip/Parameter.py
+-rw-r--r--   0        0        0     9484 2024-05-31 08:28:01.174802 evomip-0.1.1/evomip/Population.py
+-rw-r--r--   0        0        0     2252 2024-05-31 08:28:05.625620 evomip-0.1.1/evomip/SearchSpace.py
+-rw-r--r--   0        0        0     5166 2024-05-31 08:28:22.623824 evomip-0.1.1/evomip/WOA.py
+-rw-r--r--   0        0        0        0 2024-05-31 08:26:16.289106 evomip-0.1.1/evomip/__init__.py
+-rw-r--r--   0        0        0      270 2024-05-31 08:44:05.354067 evomip-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      289 1970-01-01 00:00:00.000000 evomip-0.1.1/PKG-INFO
```

### Comparing `evomip-0.1.0/evomip/Algorithm.py` & `evomip-0.1.1/evomip/Algorithm.py`

 * *Files identical despite different names*

### Comparing `evomip-0.1.0/evomip/Config.py` & `evomip-0.1.1/evomip/Config.py`

 * *Files identical despite different names*

### Comparing `evomip-0.1.0/evomip/Individual.py` & `evomip-0.1.1/evomip/Individual.py`

 * *Files identical despite different names*

### Comparing `evomip-0.1.0/evomip/Parameter.py` & `evomip-0.1.1/evomip/Parameter.py`

 * *Files identical despite different names*

### Comparing `evomip-0.1.0/evomip/Population.py` & `evomip-0.1.1/evomip/Population.py`

 * *Files identical despite different names*

### Comparing `evomip-0.1.0/evomip/SearchSpace.py` & `evomip-0.1.1/evomip/SearchSpace.py`

 * *Files identical despite different names*

### Comparing `evomip-0.1.0/evomip/WOA.py` & `evomip-0.1.1/evomip/WOA.py`

 * *Files identical despite different names*

