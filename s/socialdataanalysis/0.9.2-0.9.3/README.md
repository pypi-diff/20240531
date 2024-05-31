# Comparing `tmp/socialdataanalysis-0.9.2.tar.gz` & `tmp/socialdataanalysis-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socialdataanalysis-0.9.2.tar", last modified: Fri May 31 14:27:09 2024, max compression
+gzip compressed data, was "socialdataanalysis-0.9.3.tar", last modified: Fri May 31 14:38:46 2024, max compression
```

## Comparing `socialdataanalysis-0.9.2.tar` & `socialdataanalysis-0.9.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:27:09.529188 socialdataanalysis-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-31 14:27:00.000000 socialdataanalysis-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 14:27:00.000000 socialdataanalysis-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-31 14:27:09.529188 socialdataanalysis-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-31 14:27:00.000000 socialdataanalysis-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 14:27:09.529188 socialdataanalysis-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-31 14:27:00.000000 socialdataanalysis-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:27:09.529188 socialdataanalysis-0.9.2/socialdataanalysis/
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-31 14:27:00.000000 socialdataanalysis-0.9.2/socialdataanalysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63870 2024-05-31 14:27:00.000000 socialdataanalysis-0.9.2/socialdataanalysis/association.py
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-31 14:27:00.000000 socialdataanalysis-0.9.2/socialdataanalysis/exploratoryfactoranalysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:27:09.529188 socialdataanalysis-0.9.2/socialdataanalysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-31 14:27:09.000000 socialdataanalysis-0.9.2/socialdataanalysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-31 14:27:09.000000 socialdataanalysis-0.9.2/socialdataanalysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 14:27:09.000000 socialdataanalysis-0.9.2/socialdataanalysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 14:27:09.000000 socialdataanalysis-0.9.2/socialdataanalysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-31 14:27:09.000000 socialdataanalysis-0.9.2/socialdataanalysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:38:46.015607 socialdataanalysis-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-31 14:38:36.000000 socialdataanalysis-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-31 14:38:36.000000 socialdataanalysis-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-31 14:38:46.015607 socialdataanalysis-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-31 14:38:36.000000 socialdataanalysis-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 14:38:46.015607 socialdataanalysis-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-31 14:38:36.000000 socialdataanalysis-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:38:46.015607 socialdataanalysis-0.9.3/socialdataanalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-31 14:38:36.000000 socialdataanalysis-0.9.3/socialdataanalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63870 2024-05-31 14:38:36.000000 socialdataanalysis-0.9.3/socialdataanalysis/association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-31 14:38:36.000000 socialdataanalysis-0.9.3/socialdataanalysis/exploratoryfactoranalysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:38:46.015607 socialdataanalysis-0.9.3/socialdataanalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-31 14:38:45.000000 socialdataanalysis-0.9.3/socialdataanalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-31 14:38:45.000000 socialdataanalysis-0.9.3/socialdataanalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 14:38:45.000000 socialdataanalysis-0.9.3/socialdataanalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 14:38:45.000000 socialdataanalysis-0.9.3/socialdataanalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-31 14:38:45.000000 socialdataanalysis-0.9.3/socialdataanalysis.egg-info/top_level.txt
```

### Comparing `socialdataanalysis-0.9.2/LICENSE` & `socialdataanalysis-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.2/PKG-INFO` & `socialdataanalysis-0.9.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socialdataanalysis
-Version: 0.9.2
+Version: 0.9.3
 Summary: Funções personalizadas para análise de dados nas ciências sociais, complementando o uso do SPSS.
 Home-page: https://github.com/rcmergulhao/socialdataanalysis
 Author: Ricardo Mergulhao
 Author-email: ricardomergulhao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `socialdataanalysis-0.9.2/README.md` & `socialdataanalysis-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.2/setup.py` & `socialdataanalysis-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='socialdataanalysis',
-    version='0.9.2',
+    version='0.9.3',
     packages=find_packages(),
     include_package_data=True,
     package_data={
         'socialdataanalysis': ['notebooks/*.ipynb'],
     },
     install_requires=[
         'pandas',
```

### Comparing `socialdataanalysis-0.9.2/socialdataanalysis/__init__.py` & `socialdataanalysis-0.9.3/socialdataanalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.2/socialdataanalysis/association.py` & `socialdataanalysis-0.9.3/socialdataanalysis/association.py`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.2/socialdataanalysis/exploratoryfactoranalysis.py` & `socialdataanalysis-0.9.3/socialdataanalysis/exploratoryfactoranalysis.py`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.2/socialdataanalysis.egg-info/PKG-INFO` & `socialdataanalysis-0.9.3/socialdataanalysis.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socialdataanalysis
-Version: 0.9.2
+Version: 0.9.3
 Summary: Funções personalizadas para análise de dados nas ciências sociais, complementando o uso do SPSS.
 Home-page: https://github.com/rcmergulhao/socialdataanalysis
 Author: Ricardo Mergulhao
 Author-email: ricardomergulhao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

