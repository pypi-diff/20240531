# Comparing `tmp/resmda-0.1.1.tar.gz` & `tmp/resmda-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resmda-0.1.1.tar", last modified: Thu May 30 12:19:52 2024, max compression
+gzip compressed data, was "resmda-0.1.2.tar", last modified: Fri May 31 12:57:56 2024, max compression
```

## Comparing `resmda-0.1.1.tar` & `resmda-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:19:52.411924 resmda-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 12:19:43.000000 resmda-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-30 12:19:52.411924 resmda-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-30 12:19:43.000000 resmda-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:19:52.411924 resmda-0.1.1/resmda/
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-30 12:19:43.000000 resmda-0.1.1/resmda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-05-30 12:19:43.000000 resmda-0.1.1/resmda/data_assimilation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13810 2024-05-30 12:19:43.000000 resmda-0.1.1/resmda/reservoir_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-30 12:19:43.000000 resmda-0.1.1/resmda/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 12:19:52.000000 resmda-0.1.1/resmda/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:19:52.411924 resmda-0.1.1/resmda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-30 12:19:52.000000 resmda-0.1.1/resmda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-30 12:19:52.000000 resmda-0.1.1/resmda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 12:19:52.000000 resmda-0.1.1/resmda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 12:19:52.000000 resmda-0.1.1/resmda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 12:19:52.000000 resmda-0.1.1/resmda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 12:19:52.411924 resmda-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-30 12:19:43.000000 resmda-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:57:56.293482 resmda-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-31 12:57:47.000000 resmda-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-31 12:57:56.289482 resmda-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-31 12:57:47.000000 resmda-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:57:56.289482 resmda-0.1.2/resmda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-31 12:57:47.000000 resmda-0.1.2/resmda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-05-31 12:57:47.000000 resmda-0.1.2/resmda/data_assimilation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13810 2024-05-31 12:57:47.000000 resmda-0.1.2/resmda/reservoir_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-31 12:57:47.000000 resmda-0.1.2/resmda/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 12:57:56.000000 resmda-0.1.2/resmda/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:57:56.289482 resmda-0.1.2/resmda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-31 12:57:56.000000 resmda-0.1.2/resmda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-31 12:57:56.000000 resmda-0.1.2/resmda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 12:57:56.000000 resmda-0.1.2/resmda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-31 12:57:56.000000 resmda-0.1.2/resmda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-31 12:57:56.000000 resmda-0.1.2/resmda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 12:57:56.293482 resmda-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-31 12:57:47.000000 resmda-0.1.2/setup.py
```

### Comparing `resmda-0.1.1/LICENSE` & `resmda-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `resmda-0.1.1/PKG-INFO` & `resmda-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resmda
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple 2D reservoir modeller plus ESMDA.
 Home-page: https://github.com/tuda-geo/resmda
 Author: Dieter Werthmüller, Gabriel Serrao Seabra
 Author-email: info@emsig.xyz
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `resmda-0.1.1/README.rst` & `resmda-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `resmda-0.1.1/resmda/__init__.py` & `resmda-0.1.2/resmda/__init__.py`

 * *Files identical despite different names*

### Comparing `resmda-0.1.1/resmda/data_assimilation.py` & `resmda-0.1.2/resmda/data_assimilation.py`

 * *Files identical despite different names*

### Comparing `resmda-0.1.1/resmda/reservoir_simulator.py` & `resmda-0.1.2/resmda/reservoir_simulator.py`

 * *Files identical despite different names*

### Comparing `resmda-0.1.1/resmda/utils.py` & `resmda-0.1.2/resmda/utils.py`

 * *Files identical despite different names*

### Comparing `resmda-0.1.1/resmda.egg-info/PKG-INFO` & `resmda-0.1.2/resmda.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resmda
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple 2D reservoir modeller plus ESMDA.
 Home-page: https://github.com/tuda-geo/resmda
 Author: Dieter Werthmüller, Gabriel Serrao Seabra
 Author-email: info@emsig.xyz
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `resmda-0.1.1/setup.py` & `resmda-0.1.2/setup.py`

 * *Files identical despite different names*

