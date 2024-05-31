# Comparing `tmp/vtacML-0.1.0.tar.gz` & `tmp/vtacML-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtacML-0.1.0.tar", last modified: Fri May 31 19:11:33 2024, max compression
+gzip compressed data, was "vtacML-0.1.1.tar", last modified: Fri May 31 19:28:03 2024, max compression
```

## Comparing `vtacML-0.1.0.tar` & `vtacML-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jeremypalmerio   (501) staff       (20)        0 2024-05-31 19:11:33.401625 vtacML-0.1.0/
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)     1496 2024-02-23 14:25:44.000000 vtacML-0.1.0/LICENSE
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)      706 2024-05-31 19:11:33.401420 vtacML-0.1.0/PKG-INFO
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)       20 2024-05-31 17:50:09.000000 vtacML-0.1.0/README.md
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)       94 2024-05-31 18:21:42.000000 vtacML-0.1.0/pyproject.toml
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)       38 2024-05-31 19:11:33.401674 vtacML-0.1.0/setup.cfg
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)     1187 2024-05-31 19:09:48.000000 vtacML-0.1.0/setup.py
-drwxr-xr-x   0 jeremypalmerio   (501) staff       (20)        0 2024-05-31 19:11:33.400438 vtacML-0.1.0/testing/
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)        0 2024-05-31 17:36:29.000000 vtacML-0.1.0/testing/__init__.py
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)      365 2024-04-10 18:56:40.000000 vtacML-0.1.0/testing/config.py
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)      853 2024-05-31 19:09:48.000000 vtacML-0.1.0/testing/resampler.py
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)     1115 2024-03-28 12:06:52.000000 vtacML-0.1.0/testing/training.py
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)      240 2024-03-28 12:06:52.000000 vtacML-0.1.0/testing/validation.py
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)      411 2024-05-31 19:09:48.000000 vtacML-0.1.0/testing/wrapper.py
-drwxr-xr-x   0 jeremypalmerio   (501) staff       (20)        0 2024-05-31 19:11:33.401092 vtacML-0.1.0/vtacML.egg-info/
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)      706 2024-05-31 19:11:33.000000 vtacML-0.1.0/vtacML.egg-info/PKG-INFO
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)      310 2024-05-31 19:11:33.000000 vtacML-0.1.0/vtacML.egg-info/SOURCES.txt
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)        1 2024-05-31 19:11:33.000000 vtacML-0.1.0/vtacML.egg-info/dependency_links.txt
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)       99 2024-05-31 19:11:33.000000 vtacML-0.1.0/vtacML.egg-info/requires.txt
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)        8 2024-05-31 19:11:33.000000 vtacML-0.1.0/vtacML.egg-info/top_level.txt
+drwxr-xr-x   0 jeremypalmerio   (501) staff       (20)        0 2024-05-31 19:28:03.527204 vtacML-0.1.1/
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)     1496 2024-02-23 14:25:44.000000 vtacML-0.1.1/LICENSE
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      706 2024-05-31 19:28:03.526973 vtacML-0.1.1/PKG-INFO
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)       20 2024-05-31 17:50:09.000000 vtacML-0.1.1/README.md
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)       94 2024-05-31 18:21:42.000000 vtacML-0.1.1/pyproject.toml
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)       38 2024-05-31 19:28:03.527246 vtacML-0.1.1/setup.cfg
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)     1187 2024-05-31 19:27:54.000000 vtacML-0.1.1/setup.py
+drwxr-xr-x   0 jeremypalmerio   (501) staff       (20)        0 2024-05-31 19:28:03.525925 vtacML-0.1.1/testing/
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)        0 2024-05-31 17:36:29.000000 vtacML-0.1.1/testing/__init__.py
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      365 2024-04-10 18:56:40.000000 vtacML-0.1.1/testing/config.py
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      853 2024-05-31 19:09:48.000000 vtacML-0.1.1/testing/resampler.py
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)     1115 2024-03-28 12:06:52.000000 vtacML-0.1.1/testing/training.py
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      240 2024-03-28 12:06:52.000000 vtacML-0.1.1/testing/validation.py
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      411 2024-05-31 19:09:48.000000 vtacML-0.1.1/testing/wrapper.py
+drwxr-xr-x   0 jeremypalmerio   (501) staff       (20)        0 2024-05-31 19:28:03.526638 vtacML-0.1.1/vtacML.egg-info/
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      706 2024-05-31 19:28:03.000000 vtacML-0.1.1/vtacML.egg-info/PKG-INFO
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      310 2024-05-31 19:28:03.000000 vtacML-0.1.1/vtacML.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)        1 2024-05-31 19:28:03.000000 vtacML-0.1.1/vtacML.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)       99 2024-05-31 19:28:03.000000 vtacML-0.1.1/vtacML.egg-info/requires.txt
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)        8 2024-05-31 19:28:03.000000 vtacML-0.1.1/vtacML.egg-info/top_level.txt
```

### Comparing `vtacML-0.1.0/LICENSE` & `vtacML-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vtacML-0.1.0/PKG-INFO` & `vtacML-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtacML
-Version: 0.1.0
+Version: 0.1.1
 Summary: A machine learning pipeline to classify objects in VTAC dataset as GRB or not.
 Home-page: https://github.com/jerbeario/VTAC_ML
 Author: Jeremy Palmerio
 Author-email: jeremypalmerio05@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vtacML-0.1.0/setup.py` & `vtacML-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vtacML',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(include=['testing', 'testing.*']),
     install_requires=[
         'numpy>=1.26.3',
         'matplotlib>=3.8.0',
         'pandas>=2.1.4',
         'scikit-learn>=1.3.0',
         'seaborn>=0.12.2',
```

### Comparing `vtacML-0.1.0/testing/resampler.py` & `vtacML-0.1.1/testing/resampler.py`

 * *Files identical despite different names*

### Comparing `vtacML-0.1.0/testing/training.py` & `vtacML-0.1.1/testing/training.py`

 * *Files identical despite different names*

### Comparing `vtacML-0.1.0/vtacML.egg-info/PKG-INFO` & `vtacML-0.1.1/vtacML.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtacML
-Version: 0.1.0
+Version: 0.1.1
 Summary: A machine learning pipeline to classify objects in VTAC dataset as GRB or not.
 Home-page: https://github.com/jerbeario/VTAC_ML
 Author: Jeremy Palmerio
 Author-email: jeremypalmerio05@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

