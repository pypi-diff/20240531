# Comparing `tmp/whotfis_py-0.0.4.tar.gz` & `tmp/whotfis_py-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whotfis_py-0.0.4.tar", last modified: Thu May 30 19:38:02 2024, max compression
+gzip compressed data, was "whotfis_py-0.0.5.tar", last modified: Fri May 31 05:19:14 2024, max compression
```

## Comparing `whotfis_py-0.0.4.tar` & `whotfis_py-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-30 19:38:02.045009 whotfis_py-0.0.4/
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)    11357 2024-05-30 18:44:34.000000 whotfis_py-0.0.4/LICENSE
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       68 2024-05-30 19:22:27.000000 whotfis_py-0.0.4/MANIFEST.in
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      639 2024-05-30 19:38:02.044824 whotfis_py-0.0.4/PKG-INFO
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       67 2024-05-30 18:44:34.000000 whotfis_py-0.0.4/README.md
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       38 2024-05-30 19:38:02.045044 whotfis_py-0.0.4/setup.cfg
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      766 2024-05-30 19:37:34.000000 whotfis_py-0.0.4/setup.py
-drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-30 19:38:02.044067 whotfis_py-0.0.4/whotfis-py/
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      639 2024-05-30 19:36:49.000000 whotfis_py-0.0.4/whotfis-py/__init__.py
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     2412 2024-05-30 18:33:09.000000 whotfis_py-0.0.4/whotfis-py/parser.py
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     1639 2024-05-30 18:19:52.000000 whotfis_py-0.0.4/whotfis-py/registries.py
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     4108 2024-05-30 18:14:07.000000 whotfis_py-0.0.4/whotfis-py/result.py
-drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-30 19:38:02.044642 whotfis_py-0.0.4/whotfis_py.egg-info/
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      639 2024-05-30 19:38:02.000000 whotfis_py-0.0.4/whotfis_py.egg-info/PKG-INFO
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      264 2024-05-30 19:38:02.000000 whotfis_py-0.0.4/whotfis_py.egg-info/SOURCES.txt
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)        1 2024-05-30 19:38:02.000000 whotfis_py-0.0.4/whotfis_py.egg-info/dependency_links.txt
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       11 2024-05-30 19:38:02.000000 whotfis_py-0.0.4/whotfis_py.egg-info/top_level.txt
+drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-31 05:19:14.655583 whotfis_py-0.0.5/
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)    11357 2024-05-30 18:44:34.000000 whotfis_py-0.0.5/LICENSE
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       68 2024-05-30 19:22:27.000000 whotfis_py-0.0.5/MANIFEST.in
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      705 2024-05-31 05:19:14.655429 whotfis_py-0.0.5/PKG-INFO
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       67 2024-05-30 18:44:34.000000 whotfis_py-0.0.5/README.md
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       38 2024-05-31 05:19:14.655615 whotfis_py-0.0.5/setup.cfg
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      837 2024-05-31 05:19:12.000000 whotfis_py-0.0.5/setup.py
+drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-31 05:19:14.654646 whotfis_py-0.0.5/whotfis_py/
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      699 2024-05-31 05:19:12.000000 whotfis_py-0.0.5/whotfis_py/__init__.py
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     2419 2024-05-31 05:16:32.000000 whotfis_py-0.0.5/whotfis_py/parser.py
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     1646 2024-05-31 05:16:32.000000 whotfis_py-0.0.5/whotfis_py/registries.py
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     4108 2024-05-30 18:14:07.000000 whotfis_py-0.0.5/whotfis_py/result.py
+drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-31 05:19:14.655279 whotfis_py-0.0.5/whotfis_py.egg-info/
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      705 2024-05-31 05:19:14.000000 whotfis_py-0.0.5/whotfis_py.egg-info/PKG-INFO
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      264 2024-05-31 05:19:14.000000 whotfis_py-0.0.5/whotfis_py.egg-info/SOURCES.txt
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)        1 2024-05-31 05:19:14.000000 whotfis_py-0.0.5/whotfis_py.egg-info/dependency_links.txt
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       11 2024-05-31 05:19:14.000000 whotfis_py-0.0.5/whotfis_py.egg-info/top_level.txt
```

### Comparing `whotfis_py-0.0.4/LICENSE` & `whotfis_py-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `whotfis_py-0.0.4/PKG-INFO` & `whotfis_py-0.0.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: whotfis-py
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple package to interact with the whois command line tool
+Home-page: https://github.com/xV4L3x/whotfis-py
 Author: Valerio Pio De Nicola
 Author-email: valeriopio02@gmail.com
+License: Apache 2
 Keywords: python,whois,whois command line,whois python,whois python package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `whotfis_py-0.0.4/setup.py` & `whotfis_py-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = "Simple package to interact with the whois command line tool"
 
 setup(
     name="whotfis-py",
     version=VERSION,
     author="Valerio Pio De Nicola",
     author_email="valeriopio02@gmail.com",
     description=DESCRIPTION,
-    long_description=open('whotfis-py/README.md').read(),
+    long_description=open('whotfis_py/README.md').read(),
     long_description_content_type='text/markdown',
-    packages=find_packages(),
+    url="https://github.com/xV4L3x/whotfis-py",
+    license="Apache 2",
+    packages=['whotfis_py'],
     install_requires=[],
     keywords=['python', 'whois', 'whois command line', 'whois python', 'whois python package'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `whotfis_py-0.0.4/whotfis-py/__init__.py` & `whotfis_py-0.0.5/whotfis_py/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import os
 from . import registries
 from .parser import parse
 
+__version__ = "0.0.5"
+__author__ = "Valerio Pio De Nicola"
+
 
 def lookup(query, registry=registries.RADB, custom_server=""):
     if registry == registries.CUSTOM:
         if custom_server == "" or custom_server is None:
             raise ValueError("Custom server must be specified when using the CUSTOM registry")
 
     command = "whois {} {} {}".format(registry, custom_server, query)
```

### Comparing `whotfis_py-0.0.4/whotfis-py/parser.py` & `whotfis_py-0.0.5/whotfis_py/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import registries
+from . import registries
 
 
 def print_error(error, registry):
     print(error + "\n")
     print(registries.infos[registry])
```

### Comparing `whotfis_py-0.0.4/whotfis-py/registries.py` & `whotfis_py-0.0.5/whotfis_py/registries.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import result
+from . import result
 
 ARIN = "-a"
 APNIC = "-A"
 ABUSE = "-b"
 AFRINIC = "-f"
 USMILITRY = "-g"
 INTERNIC = "-i"
```

### Comparing `whotfis_py-0.0.4/whotfis-py/result.py` & `whotfis_py-0.0.5/whotfis_py/result.py`

 * *Files identical despite different names*

### Comparing `whotfis_py-0.0.4/whotfis_py.egg-info/PKG-INFO` & `whotfis_py-0.0.5/whotfis_py.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: whotfis-py
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple package to interact with the whois command line tool
+Home-page: https://github.com/xV4L3x/whotfis-py
 Author: Valerio Pio De Nicola
 Author-email: valeriopio02@gmail.com
+License: Apache 2
 Keywords: python,whois,whois command line,whois python,whois python package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

