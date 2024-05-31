# Comparing `tmp/myfunction_ViktoriyaXIII-0.0.6.tar.gz` & `tmp/myfunction_ViktoriyaXIII-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/ViktoriyaXIII/Python/evolve_cyber/class5/dist/tmp7zjb7x8v/myfunction_ViktoriyaXIII-0.0.6.tar", last modified: Thu May 30 01:33:57 2024, max compression
+gzip compressed data, was "/mnt/ViktoriyaXIII/Python/evolve_cyber/class5/dist/tmpu7afxyfa/myfunction_ViktoriyaXIII-0.0.7.tar", last modified: Fri May 31 19:03:47 2024, max compression
```

## Comparing `myfunction_ViktoriyaXIII-0.0.6.tar` & `myfunction_ViktoriyaXIII-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-30 01:33:57.000000 myfunction_ViktoriyaXIII-0.0.6/
-drwxrwxr-x   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-30 01:33:57.000000 myfunction_ViktoriyaXIII-0.0.6/myfunction_ViktoriyaXIII/
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)      406 2024-05-30 01:31:46.000000 myfunction_ViktoriyaXIII-0.0.6/myfunction_ViktoriyaXIII/math.py
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-30 00:48:58.000000 myfunction_ViktoriyaXIII-0.0.6/myfunction_ViktoriyaXIII/__init__.py
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)      649 2024-05-30 01:33:46.000000 myfunction_ViktoriyaXIII-0.0.6/setup.py
-drwxrwxr-x   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-30 01:33:57.000000 myfunction_ViktoriyaXIII-0.0.6/myfunction_ViktoriyaXIII.egg-info/
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)       25 2024-05-30 01:33:57.000000 myfunction_ViktoriyaXIII-0.0.6/myfunction_ViktoriyaXIII.egg-info/top_level.txt
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)      327 2024-05-30 01:33:57.000000 myfunction_ViktoriyaXIII-0.0.6/myfunction_ViktoriyaXIII.egg-info/SOURCES.txt
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        3 2024-05-30 01:33:57.000000 myfunction_ViktoriyaXIII-0.0.6/myfunction_ViktoriyaXIII.egg-info/requires.txt
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        1 2024-05-30 01:33:57.000000 myfunction_ViktoriyaXIII-0.0.6/myfunction_ViktoriyaXIII.egg-info/dependency_links.txt
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)     2251 2024-05-30 01:33:57.000000 myfunction_ViktoriyaXIII-0.0.6/myfunction_ViktoriyaXIII.egg-info/PKG-INFO
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)     1797 2024-05-30 01:18:49.000000 myfunction_ViktoriyaXIII-0.0.6/README.md
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)     2251 2024-05-30 01:33:57.000000 myfunction_ViktoriyaXIII-0.0.6/PKG-INFO
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)       38 2024-05-30 01:33:57.000000 myfunction_ViktoriyaXIII-0.0.6/setup.cfg
+drwxrwxr-x   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-31 19:03:47.000000 myfunction_ViktoriyaXIII-0.0.7/
+drwxrwxr-x   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-31 19:03:47.000000 myfunction_ViktoriyaXIII-0.0.7/myfunction_ViktoriyaXIII/
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)      659 2024-05-31 18:56:03.000000 myfunction_ViktoriyaXIII-0.0.7/myfunction_ViktoriyaXIII/math.py
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-30 00:48:58.000000 myfunction_ViktoriyaXIII-0.0.7/myfunction_ViktoriyaXIII/__init__.py
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)      649 2024-05-31 19:03:35.000000 myfunction_ViktoriyaXIII-0.0.7/setup.py
+drwxrwxr-x   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-31 19:03:47.000000 myfunction_ViktoriyaXIII-0.0.7/myfunction_ViktoriyaXIII.egg-info/
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)       25 2024-05-31 19:03:46.000000 myfunction_ViktoriyaXIII-0.0.7/myfunction_ViktoriyaXIII.egg-info/top_level.txt
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)      327 2024-05-31 19:03:47.000000 myfunction_ViktoriyaXIII-0.0.7/myfunction_ViktoriyaXIII.egg-info/SOURCES.txt
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        3 2024-05-31 19:03:46.000000 myfunction_ViktoriyaXIII-0.0.7/myfunction_ViktoriyaXIII.egg-info/requires.txt
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        1 2024-05-31 19:03:46.000000 myfunction_ViktoriyaXIII-0.0.7/myfunction_ViktoriyaXIII.egg-info/dependency_links.txt
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)     2251 2024-05-31 19:03:46.000000 myfunction_ViktoriyaXIII-0.0.7/myfunction_ViktoriyaXIII.egg-info/PKG-INFO
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)     1797 2024-05-30 01:18:49.000000 myfunction_ViktoriyaXIII-0.0.7/README.md
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)     2251 2024-05-31 19:03:47.000000 myfunction_ViktoriyaXIII-0.0.7/PKG-INFO
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)       38 2024-05-31 19:03:47.000000 myfunction_ViktoriyaXIII-0.0.7/setup.cfg
```

### Comparing `myfunction_ViktoriyaXIII-0.0.6/setup.py` & `myfunction_ViktoriyaXIII-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunction_ViktoriyaXIII',
-    version='0.0.6',
+    version='0.0.7',
     packages=find_packages(),
     install_requires=["os"],
     url='https://github.com/ViktoriyaXIII',
     license='MIT',
     author='Viktoriia',
     author_email='viktoriya.bielova@gmail.com',
     description='A description of your package',
```

### Comparing `myfunction_ViktoriyaXIII-0.0.6/myfunction_ViktoriyaXIII.egg-info/PKG-INFO` & `myfunction_ViktoriyaXIII-0.0.7/myfunction_ViktoriyaXIII.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunction-ViktoriyaXIII
-Version: 0.0.6
+Version: 0.0.7
 Summary: A description of your package
 Home-page: https://github.com/ViktoriyaXIII
 Author: Viktoriia
 Author-email: viktoriya.bielova@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunction_ViktoriyaXIII-0.0.6/README.md` & `myfunction_ViktoriyaXIII-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `myfunction_ViktoriyaXIII-0.0.6/PKG-INFO` & `myfunction_ViktoriyaXIII-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunction_ViktoriyaXIII
-Version: 0.0.6
+Version: 0.0.7
 Summary: A description of your package
 Home-page: https://github.com/ViktoriyaXIII
 Author: Viktoriia
 Author-email: viktoriya.bielova@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

