# Comparing `tmp/anne-1.0.4.tar.gz` & `tmp/anne-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anne-1.0.4.tar", last modified: Fri May 31 00:50:17 2024, max compression
+gzip compressed data, was "anne-1.0.5.tar", last modified: Fri May 31 00:52:30 2024, max compression
```

## Comparing `anne-1.0.4.tar` & `anne-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 00:50:17.836950 anne-1.0.4/
--rw-rw-rw-   0        0        0     1090 2024-05-28 14:49:46.000000 anne-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     1731 2024-05-31 00:50:17.836950 anne-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       45 2024-05-28 15:27:28.000000 anne-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 00:50:17.830970 anne-1.0.4/app/
-drwxrwxrwx   0        0        0        0 2024-05-31 00:50:17.832964 anne-1.0.4/app/anne/
--rw-rw-rw-   0        0        0       64 2024-05-31 00:19:07.000000 anne-1.0.4/app/anne/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 00:50:17.835954 anne-1.0.4/app/anne/browser/
--rw-rw-rw-   0        0        0    18824 2024-05-28 16:14:25.000000 anne-1.0.4/app/anne/browser/AnneBrowser.py
--rw-rw-rw-   0        0        0       38 2024-05-31 00:17:53.000000 anne-1.0.4/app/anne/browser/__init__.py
--rw-rw-rw-   0        0        0      692 2024-05-28 16:07:51.000000 anne-1.0.4/app/anne/browser/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-31 00:50:17.836950 anne-1.0.4/app/anne/proxy/
--rw-rw-rw-   0        0        0      882 2024-05-31 00:03:51.000000 anne-1.0.4/app/anne/proxy/AnneProxy.py
--rw-rw-rw-   0        0        0       32 2024-05-31 00:19:01.000000 anne-1.0.4/app/anne/proxy/__init__.py
--rw-rw-rw-   0        0        0       16 2024-05-31 00:09:11.000000 anne-1.0.4/app/anne/proxy/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-31 00:50:17.834957 anne-1.0.4/app/anne.egg-info/
--rw-rw-rw-   0        0        0     1731 2024-05-31 00:50:17.000000 anne-1.0.4/app/anne.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2024-05-31 00:50:17.000000 anne-1.0.4/app/anne.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 00:50:17.000000 anne-1.0.4/app/anne.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-31 00:50:17.000000 anne-1.0.4/app/anne.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-31 00:50:17.000000 anne-1.0.4/app/anne.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 00:50:17.836950 anne-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      859 2024-05-31 00:50:17.000000 anne-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 00:52:30.606892 anne-1.0.5/
+-rw-rw-rw-   0        0        0     1090 2024-05-28 14:49:46.000000 anne-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1731 2024-05-31 00:52:30.606892 anne-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2024-05-28 15:27:28.000000 anne-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 00:52:30.586908 anne-1.0.5/app/
+drwxrwxrwx   0        0        0        0 2024-05-31 00:52:30.587904 anne-1.0.5/app/anne/
+-rw-rw-rw-   0        0        0       64 2024-05-31 00:19:07.000000 anne-1.0.5/app/anne/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 00:52:30.591325 anne-1.0.5/app/anne/browser/
+-rw-rw-rw-   0        0        0    18824 2024-05-28 16:14:25.000000 anne-1.0.5/app/anne/browser/AnneBrowser.py
+-rw-rw-rw-   0        0        0       38 2024-05-31 00:17:53.000000 anne-1.0.5/app/anne/browser/__init__.py
+-rw-rw-rw-   0        0        0      692 2024-05-28 16:07:51.000000 anne-1.0.5/app/anne/browser/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 00:52:30.605895 anne-1.0.5/app/anne/proxy/
+-rw-rw-rw-   0        0        0      882 2024-05-31 00:03:51.000000 anne-1.0.5/app/anne/proxy/AnneProxy.py
+-rw-rw-rw-   0        0        0       32 2024-05-31 00:19:01.000000 anne-1.0.5/app/anne/proxy/__init__.py
+-rw-rw-rw-   0        0        0       16 2024-05-31 00:09:11.000000 anne-1.0.5/app/anne/proxy/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 00:52:30.589898 anne-1.0.5/app/anne.egg-info/
+-rw-rw-rw-   0        0        0     1731 2024-05-31 00:52:30.000000 anne-1.0.5/app/anne.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2024-05-31 00:52:30.000000 anne-1.0.5/app/anne.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 00:52:30.000000 anne-1.0.5/app/anne.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-31 00:52:30.000000 anne-1.0.5/app/anne.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-31 00:52:30.000000 anne-1.0.5/app/anne.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 00:52:30.606892 anne-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      859 2024-05-31 00:52:30.000000 anne-1.0.5/setup.py
```

### Comparing `anne-1.0.4/LICENSE` & `anne-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `anne-1.0.4/PKG-INFO` & `anne-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anne
-Version: 1.0.4
+Version: 1.0.5
 Summary: Lib for lazy dev
 Home-page: https://github.com/mrship666/anne-lib
 Author: AnneHouman
 Author-email: annehouman01@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `anne-1.0.4/app/anne/browser/AnneBrowser.py` & `anne-1.0.5/app/anne/browser/AnneBrowser.py`

 * *Files identical despite different names*

### Comparing `anne-1.0.4/app/anne/browser/utils.py` & `anne-1.0.5/app/anne/browser/utils.py`

 * *Files identical despite different names*

### Comparing `anne-1.0.4/app/anne/proxy/AnneProxy.py` & `anne-1.0.5/app/anne/proxy/AnneProxy.py`

 * *Files identical despite different names*

### Comparing `anne-1.0.4/app/anne.egg-info/PKG-INFO` & `anne-1.0.5/app/anne.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anne
-Version: 1.0.4
+Version: 1.0.5
 Summary: Lib for lazy dev
 Home-page: https://github.com/mrship666/anne-lib
 Author: AnneHouman
 Author-email: annehouman01@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `anne-1.0.4/setup.py` & `anne-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("app/README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="anne",
-    version="1.0.4",
+    version="1.0.5",
     description="Lib for lazy dev",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mrship666/anne-lib",
     author="AnneHouman",
```

