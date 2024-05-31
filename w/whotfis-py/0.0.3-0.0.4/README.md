# Comparing `tmp/whotfis_py-0.0.3.tar.gz` & `tmp/whotfis_py-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whotfis_py-0.0.3.tar", last modified: Thu May 30 19:22:43 2024, max compression
+gzip compressed data, was "whotfis_py-0.0.4.tar", last modified: Thu May 30 19:38:02 2024, max compression
```

## Comparing `whotfis_py-0.0.3.tar` & `whotfis_py-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-30 19:22:43.316008 whotfis_py-0.0.3/
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)    11357 2024-05-30 18:44:34.000000 whotfis_py-0.0.3/LICENSE
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       68 2024-05-30 19:22:27.000000 whotfis_py-0.0.3/MANIFEST.in
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      639 2024-05-30 19:22:43.315797 whotfis_py-0.0.3/PKG-INFO
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       67 2024-05-30 18:44:34.000000 whotfis_py-0.0.3/README.md
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       38 2024-05-30 19:22:43.316047 whotfis_py-0.0.3/setup.cfg
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      766 2024-05-30 19:22:41.000000 whotfis_py-0.0.3/setup.py
-drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-30 19:22:43.314892 whotfis_py-0.0.3/whotfis-py/
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      631 2024-05-30 18:52:25.000000 whotfis_py-0.0.3/whotfis-py/__init__.py
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     2412 2024-05-30 18:33:09.000000 whotfis_py-0.0.3/whotfis-py/parser.py
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     1639 2024-05-30 18:19:52.000000 whotfis_py-0.0.3/whotfis-py/registries.py
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     4108 2024-05-30 18:14:07.000000 whotfis_py-0.0.3/whotfis-py/result.py
-drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-30 19:22:43.315596 whotfis_py-0.0.3/whotfis_py.egg-info/
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      639 2024-05-30 19:22:43.000000 whotfis_py-0.0.3/whotfis_py.egg-info/PKG-INFO
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      264 2024-05-30 19:22:43.000000 whotfis_py-0.0.3/whotfis_py.egg-info/SOURCES.txt
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)        1 2024-05-30 19:22:43.000000 whotfis_py-0.0.3/whotfis_py.egg-info/dependency_links.txt
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       11 2024-05-30 19:22:43.000000 whotfis_py-0.0.3/whotfis_py.egg-info/top_level.txt
+drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-30 19:38:02.045009 whotfis_py-0.0.4/
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)    11357 2024-05-30 18:44:34.000000 whotfis_py-0.0.4/LICENSE
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       68 2024-05-30 19:22:27.000000 whotfis_py-0.0.4/MANIFEST.in
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      639 2024-05-30 19:38:02.044824 whotfis_py-0.0.4/PKG-INFO
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       67 2024-05-30 18:44:34.000000 whotfis_py-0.0.4/README.md
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       38 2024-05-30 19:38:02.045044 whotfis_py-0.0.4/setup.cfg
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      766 2024-05-30 19:37:34.000000 whotfis_py-0.0.4/setup.py
+drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-30 19:38:02.044067 whotfis_py-0.0.4/whotfis-py/
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      639 2024-05-30 19:36:49.000000 whotfis_py-0.0.4/whotfis-py/__init__.py
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     2412 2024-05-30 18:33:09.000000 whotfis_py-0.0.4/whotfis-py/parser.py
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     1639 2024-05-30 18:19:52.000000 whotfis_py-0.0.4/whotfis-py/registries.py
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     4108 2024-05-30 18:14:07.000000 whotfis_py-0.0.4/whotfis-py/result.py
+drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-30 19:38:02.044642 whotfis_py-0.0.4/whotfis_py.egg-info/
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      639 2024-05-30 19:38:02.000000 whotfis_py-0.0.4/whotfis_py.egg-info/PKG-INFO
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      264 2024-05-30 19:38:02.000000 whotfis_py-0.0.4/whotfis_py.egg-info/SOURCES.txt
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)        1 2024-05-30 19:38:02.000000 whotfis_py-0.0.4/whotfis_py.egg-info/dependency_links.txt
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       11 2024-05-30 19:38:02.000000 whotfis_py-0.0.4/whotfis_py.egg-info/top_level.txt
```

### Comparing `whotfis_py-0.0.3/LICENSE` & `whotfis_py-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `whotfis_py-0.0.3/PKG-INFO` & `whotfis_py-0.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whotfis-py
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple package to interact with the whois command line tool
 Author: Valerio Pio De Nicola
 Author-email: valeriopio02@gmail.com
 Keywords: python,whois,whois command line,whois python,whois python package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `whotfis_py-0.0.3/setup.py` & `whotfis_py-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = "Simple package to interact with the whois command line tool"
 
 setup(
     name="whotfis-py",
     version=VERSION,
     author="Valerio Pio De Nicola",
     author_email="valeriopio02@gmail.com",
```

### Comparing `whotfis_py-0.0.3/whotfis-py/__init__.py` & `whotfis_py-0.0.4/whotfis-py/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
-import registries
-from parser import parse
+from . import registries
+from .parser import parse
 
 
 def lookup(query, registry=registries.RADB, custom_server=""):
     if registry == registries.CUSTOM:
         if custom_server == "" or custom_server is None:
             raise ValueError("Custom server must be specified when using the CUSTOM registry")
```

### Comparing `whotfis_py-0.0.3/whotfis-py/parser.py` & `whotfis_py-0.0.4/whotfis-py/parser.py`

 * *Files identical despite different names*

### Comparing `whotfis_py-0.0.3/whotfis-py/registries.py` & `whotfis_py-0.0.4/whotfis-py/registries.py`

 * *Files identical despite different names*

### Comparing `whotfis_py-0.0.3/whotfis-py/result.py` & `whotfis_py-0.0.4/whotfis-py/result.py`

 * *Files identical despite different names*

### Comparing `whotfis_py-0.0.3/whotfis_py.egg-info/PKG-INFO` & `whotfis_py-0.0.4/whotfis_py.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whotfis-py
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple package to interact with the whois command line tool
 Author: Valerio Pio De Nicola
 Author-email: valeriopio02@gmail.com
 Keywords: python,whois,whois command line,whois python,whois python package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

