# Comparing `tmp/jeffutils-0.7.1.tar.gz` & `tmp/jeffutils-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeffutils-0.7.1.tar", last modified: Fri May 31 17:11:00 2024, max compression
+gzip compressed data, was "jeffutils-0.7.2.tar", last modified: Fri May 31 17:14:14 2024, max compression
```

## Comparing `jeffutils-0.7.1.tar` & `jeffutils-0.7.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:11:00.333500 jeffutils-0.7.1/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.7.1/LICENSE.txt
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      576 2024-05-31 17:11:00.333500 jeffutils-0.7.1/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     2685 2024-05-31 17:04:40.000000 jeffutils-0.7.1/README.md
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.7.1/pyproject.toml
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-31 17:11:00.333500 jeffutils-0.7.1/setup.cfg
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      715 2024-05-31 17:10:59.000000 jeffutils-0.7.1/setup.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:11:00.333500 jeffutils-0.7.1/src/
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:11:00.333500 jeffutils-0.7.1/src/jeffutils/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.7.1/src/jeffutils/__init__.py
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    37827 2024-05-31 17:05:48.000000 jeffutils-0.7.1/src/jeffutils/utils.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:11:00.333500 jeffutils-0.7.1/src/jeffutils.egg-info/
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      576 2024-05-31 17:11:00.000000 jeffutils-0.7.1/src/jeffutils.egg-info/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-31 17:11:00.000000 jeffutils-0.7.1/src/jeffutils.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-31 17:11:00.000000 jeffutils-0.7.1/src/jeffutils.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-31 17:11:00.000000 jeffutils-0.7.1/src/jeffutils.egg-info/top_level.txt
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:14:14.889932 jeffutils-0.7.2/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.7.2/LICENSE.txt
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      576 2024-05-31 17:14:14.889932 jeffutils-0.7.2/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     2685 2024-05-31 17:04:40.000000 jeffutils-0.7.2/README.md
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.7.2/pyproject.toml
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-31 17:14:14.889932 jeffutils-0.7.2/setup.cfg
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      715 2024-05-31 17:14:13.000000 jeffutils-0.7.2/setup.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:14:14.889932 jeffutils-0.7.2/src/
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:14:14.889932 jeffutils-0.7.2/src/jeffutils/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.7.2/src/jeffutils/__init__.py
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    37827 2024-05-31 17:05:48.000000 jeffutils-0.7.2/src/jeffutils/utils.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:14:14.889932 jeffutils-0.7.2/src/jeffutils.egg-info/
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      576 2024-05-31 17:14:14.000000 jeffutils-0.7.2/src/jeffutils.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-31 17:14:14.000000 jeffutils-0.7.2/src/jeffutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-31 17:14:14.000000 jeffutils-0.7.2/src/jeffutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-31 17:14:14.000000 jeffutils-0.7.2/src/jeffutils.egg-info/top_level.txt
```

### Comparing `jeffutils-0.7.1/LICENSE.txt` & `jeffutils-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jeffutils-0.7.1/PKG-INFO` & `jeffutils-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeffutils
-Version: 0.7.1
+Version: 0.7.2
 Summary: Welcome to Jeff Hansen's suite of useful python functions! I use lots of these functions on most of my Data Analysis, Backend-Dev, and Machine Learning projects, and I hope you find some of them useful as well!
 Home-page: https://github.com/jeffxhansen/jeffutils
 Author: Jeff Hansen
 Author-email: jeffxhansen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jeffutils-0.7.1/README.md` & `jeffutils-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `jeffutils-0.7.1/setup.py` & `jeffutils-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='jeffutils',
-    version='0.7.1',
+    version='0.7.2',
     author='Jeff Hansen',
     author_email='jeffxhansen@gmail.com',
     description="Welcome to Jeff Hansen's suite of useful python functions! I use lots of these functions on most of my Data Analysis, Backend-Dev, and Machine Learning projects, and I hope you find some of them useful as well!",
     package_dir={"": "src"},
     packages = find_packages(where="src"),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `jeffutils-0.7.1/src/jeffutils/utils.py` & `jeffutils-0.7.2/src/jeffutils/utils.py`

 * *Files identical despite different names*

### Comparing `jeffutils-0.7.1/src/jeffutils.egg-info/PKG-INFO` & `jeffutils-0.7.2/src/jeffutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeffutils
-Version: 0.7.1
+Version: 0.7.2
 Summary: Welcome to Jeff Hansen's suite of useful python functions! I use lots of these functions on most of my Data Analysis, Backend-Dev, and Machine Learning projects, and I hope you find some of them useful as well!
 Home-page: https://github.com/jeffxhansen/jeffutils
 Author: Jeff Hansen
 Author-email: jeffxhansen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

