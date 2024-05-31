# Comparing `tmp/colabexts-0.12200000000000003.tar.gz` & `tmp/colabexts-0.12300000000000003.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colabexts-0.12200000000000003.tar", last modified: Sat May 18 09:39:23 2024, max compression
+gzip compressed data, was "colabexts-0.12300000000000003.tar", last modified: Fri May 31 04:33:29 2024, max compression
```

## Comparing `colabexts-0.12200000000000003.tar` & `colabexts-0.12300000000000003.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-05-18 09:39:23.583473 colabexts-0.12200000000000003/
--rw-r--r--   0 snarayan   (501) wheel        (0)      780 2024-05-18 09:39:23.583044 colabexts-0.12200000000000003/PKG-INFO
--rw-r--r--   0 snarayan   (501) wheel        (0)     1081 2022-11-26 05:52:19.000000 colabexts-0.12200000000000003/README.md
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-05-18 09:39:23.580352 colabexts-0.12200000000000003/colabexts/
--rw-r--r--   0 snarayan   (501) wheel        (0)        0 2022-11-26 05:52:19.000000 colabexts-0.12200000000000003/colabexts/__init__.py
--rw-r--r--   0 snarayan   (501) wheel        (0)    11567 2024-04-23 12:55:18.000000 colabexts-0.12200000000000003/colabexts/jcommon.ipynb
--rw-r--r--   0 snarayan   (501) wheel        (0)     4669 2024-04-23 12:57:14.000000 colabexts-0.12200000000000003/colabexts/jcommon.py
--rw-r--r--   0 snarayan   (501) wheel        (0)      454 2022-11-26 05:52:19.000000 colabexts-0.12200000000000003/colabexts/log.py
--rw-r--r--   0 snarayan   (501) wheel        (0)     3667 2024-05-18 09:38:08.000000 colabexts-0.12200000000000003/colabexts/utils.py
--rw-r--r--   0 snarayan   (501) wheel        (0)       27 2024-05-18 09:39:23.000000 colabexts-0.12200000000000003/colabexts/version.txt
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-05-18 09:39:23.582590 colabexts-0.12200000000000003/colabexts.egg-info/
--rw-r--r--   0 snarayan   (501) wheel        (0)      780 2024-05-18 09:39:23.000000 colabexts-0.12200000000000003/colabexts.egg-info/PKG-INFO
--rw-r--r--   0 snarayan   (501) wheel        (0)      339 2024-05-18 09:39:23.000000 colabexts-0.12200000000000003/colabexts.egg-info/SOURCES.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)        1 2024-05-18 09:39:23.000000 colabexts-0.12200000000000003/colabexts.egg-info/dependency_links.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)        1 2024-04-23 15:26:14.000000 colabexts-0.12200000000000003/colabexts.egg-info/not-zip-safe
--rw-r--r--   0 snarayan   (501) wheel        (0)       20 2024-05-18 09:39:23.000000 colabexts-0.12200000000000003/colabexts.egg-info/requires.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)       10 2024-05-18 09:39:23.000000 colabexts-0.12200000000000003/colabexts.egg-info/top_level.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)       38 2024-05-18 09:39:23.583552 colabexts-0.12200000000000003/setup.cfg
--rw-r--r--   0 snarayan   (501) wheel        (0)     1678 2024-05-18 09:39:23.000000 colabexts-0.12200000000000003/setup.py
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-05-31 04:33:29.801490 colabexts-0.12300000000000003/
+-rw-r--r--   0 snarayan   (501) wheel        (0)      780 2024-05-31 04:33:29.801076 colabexts-0.12300000000000003/PKG-INFO
+-rw-r--r--   0 snarayan   (501) wheel        (0)     1081 2022-11-26 05:52:19.000000 colabexts-0.12300000000000003/README.md
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-05-31 04:33:29.797913 colabexts-0.12300000000000003/colabexts/
+-rw-r--r--   0 snarayan   (501) wheel        (0)        0 2022-11-26 05:52:19.000000 colabexts-0.12300000000000003/colabexts/__init__.py
+-rw-r--r--   0 snarayan   (501) wheel        (0)    11567 2024-04-23 12:55:18.000000 colabexts-0.12300000000000003/colabexts/jcommon.ipynb
+-rw-r--r--   0 snarayan   (501) wheel        (0)     4669 2024-04-23 12:57:14.000000 colabexts-0.12300000000000003/colabexts/jcommon.py
+-rw-r--r--   0 snarayan   (501) wheel        (0)      454 2022-11-26 05:52:19.000000 colabexts-0.12300000000000003/colabexts/log.py
+-rw-r--r--   0 snarayan   (501) wheel        (0)     3659 2024-05-18 09:51:40.000000 colabexts-0.12300000000000003/colabexts/utils.py
+-rw-r--r--   0 snarayan   (501) wheel        (0)       27 2024-05-31 04:33:29.000000 colabexts-0.12300000000000003/colabexts/version.txt
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-05-31 04:33:29.800651 colabexts-0.12300000000000003/colabexts.egg-info/
+-rw-r--r--   0 snarayan   (501) wheel        (0)      780 2024-05-31 04:33:29.000000 colabexts-0.12300000000000003/colabexts.egg-info/PKG-INFO
+-rw-r--r--   0 snarayan   (501) wheel        (0)      339 2024-05-31 04:33:29.000000 colabexts-0.12300000000000003/colabexts.egg-info/SOURCES.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)        1 2024-05-31 04:33:29.000000 colabexts-0.12300000000000003/colabexts.egg-info/dependency_links.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)        1 2024-04-23 15:26:14.000000 colabexts-0.12300000000000003/colabexts.egg-info/not-zip-safe
+-rw-r--r--   0 snarayan   (501) wheel        (0)       20 2024-05-31 04:33:29.000000 colabexts-0.12300000000000003/colabexts.egg-info/requires.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)       10 2024-05-31 04:33:29.000000 colabexts-0.12300000000000003/colabexts.egg-info/top_level.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)       38 2024-05-31 04:33:29.801569 colabexts-0.12300000000000003/setup.cfg
+-rw-r--r--   0 snarayan   (501) wheel        (0)     1678 2024-05-31 04:33:29.000000 colabexts-0.12300000000000003/setup.py
```

### Comparing `colabexts-0.12200000000000003/PKG-INFO` & `colabexts-0.12300000000000003/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colabexts
-Version: 0.12200000000000003
+Version: 0.12300000000000003
 Summary: Some simple Utilities
 Home-page: https://github.com/meyers007/colabext.git
 Author: Code Red
 Author-email: meyers@geospaces.org
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `colabexts-0.12200000000000003/README.md` & `colabexts-0.12300000000000003/README.md`

 * *Files identical despite different names*

### Comparing `colabexts-0.12200000000000003/colabexts/jcommon.ipynb` & `colabexts-0.12300000000000003/colabexts/jcommon.ipynb`

 * *Files identical despite different names*

### Comparing `colabexts-0.12200000000000003/colabexts/jcommon.py` & `colabexts-0.12300000000000003/colabexts/jcommon.py`

 * *Files identical despite different names*

### Comparing `colabexts-0.12200000000000003/colabexts/utils.py` & `colabexts-0.12300000000000003/colabexts/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,9 +108,9 @@
          return key
 
     def parsej(self, s):
         eval(s, **self)
 
         
 def parsej(s, *args, **kwargs):
-    return mydict(eval(s.strip() or "{}", mydict(*args, **kwargs)))
+    return eval(s.strip() or "{}", mydict(*args, **kwargs))
```

### Comparing `colabexts-0.12200000000000003/colabexts.egg-info/PKG-INFO` & `colabexts-0.12300000000000003/colabexts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colabexts
-Version: 0.12200000000000003
+Version: 0.12300000000000003
 Summary: Some simple Utilities
 Home-page: https://github.com/meyers007/colabext.git
 Author: Code Red
 Author-email: meyers@geospaces.org
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `colabexts-0.12200000000000003/setup.py` & `colabexts-0.12300000000000003/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version=0.12200000000000003
+version=0.12300000000000003
 
 setup(name='colabexts', 
       version=str(version), 
       description='Some simple Utilities',
       url='https://github.com/meyers007/colabext.git',
       author='Code Red',
       author_email='meyers@geospaces.org',
```

