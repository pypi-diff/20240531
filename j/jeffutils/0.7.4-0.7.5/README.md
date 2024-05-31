# Comparing `tmp/jeffutils-0.7.4.tar.gz` & `tmp/jeffutils-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeffutils-0.7.4.tar", last modified: Fri May 31 17:18:03 2024, max compression
+gzip compressed data, was "jeffutils-0.7.5.tar", last modified: Fri May 31 17:18:31 2024, max compression
```

## Comparing `jeffutils-0.7.4.tar` & `jeffutils-0.7.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:18:03.275903 jeffutils-0.7.4/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.7.4/LICENSE.txt
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      576 2024-05-31 17:18:03.275903 jeffutils-0.7.4/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     2685 2024-05-31 17:04:40.000000 jeffutils-0.7.4/README.md
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.7.4/pyproject.toml
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-31 17:18:03.275903 jeffutils-0.7.4/setup.cfg
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      715 2024-05-31 17:18:02.000000 jeffutils-0.7.4/setup.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:18:03.275903 jeffutils-0.7.4/src/
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:18:03.275903 jeffutils-0.7.4/src/jeffutils/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.7.4/src/jeffutils/__init__.py
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    37827 2024-05-31 17:05:48.000000 jeffutils-0.7.4/src/jeffutils/utils.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:18:03.275903 jeffutils-0.7.4/src/jeffutils.egg-info/
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      576 2024-05-31 17:18:03.000000 jeffutils-0.7.4/src/jeffutils.egg-info/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-31 17:18:03.000000 jeffutils-0.7.4/src/jeffutils.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-31 17:18:03.000000 jeffutils-0.7.4/src/jeffutils.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-31 17:18:03.000000 jeffutils-0.7.4/src/jeffutils.egg-info/top_level.txt
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:18:31.212224 jeffutils-0.7.5/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.7.5/LICENSE.txt
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      576 2024-05-31 17:18:31.212224 jeffutils-0.7.5/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     2685 2024-05-31 17:04:40.000000 jeffutils-0.7.5/README.md
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.7.5/pyproject.toml
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-31 17:18:31.212224 jeffutils-0.7.5/setup.cfg
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      715 2024-05-31 17:18:29.000000 jeffutils-0.7.5/setup.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:18:31.212224 jeffutils-0.7.5/src/
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:18:31.212224 jeffutils-0.7.5/src/jeffutils/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.7.5/src/jeffutils/__init__.py
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    37827 2024-05-31 17:05:48.000000 jeffutils-0.7.5/src/jeffutils/utils.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:18:31.212224 jeffutils-0.7.5/src/jeffutils.egg-info/
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      576 2024-05-31 17:18:31.000000 jeffutils-0.7.5/src/jeffutils.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-31 17:18:31.000000 jeffutils-0.7.5/src/jeffutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-31 17:18:31.000000 jeffutils-0.7.5/src/jeffutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-31 17:18:31.000000 jeffutils-0.7.5/src/jeffutils.egg-info/top_level.txt
```

### Comparing `jeffutils-0.7.4/LICENSE.txt` & `jeffutils-0.7.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jeffutils-0.7.4/PKG-INFO` & `jeffutils-0.7.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeffutils
-Version: 0.7.4
+Version: 0.7.5
 Summary: Welcome to Jeff Hansen's suite of useful python functions! I use lots of these functions on most of my Data Analysis, Backend-Dev, and Machine Learning projects, and I hope you find some of them useful as well!
 Home-page: https://github.com/jeffxhansen/jeffutils
 Author: Jeff Hansen
 Author-email: jeffxhansen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jeffutils-0.7.4/README.md` & `jeffutils-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `jeffutils-0.7.4/setup.py` & `jeffutils-0.7.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='jeffutils',
-    version='0.7.4',
+    version='0.7.5',
     author='Jeff Hansen',
     author_email='jeffxhansen@gmail.com',
     description="Welcome to Jeff Hansen's suite of useful python functions! I use lots of these functions on most of my Data Analysis, Backend-Dev, and Machine Learning projects, and I hope you find some of them useful as well!",
     package_dir={"": "src"},
     packages = find_packages(where="src"),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `jeffutils-0.7.4/src/jeffutils/utils.py` & `jeffutils-0.7.5/src/jeffutils/utils.py`

 * *Files identical despite different names*

### Comparing `jeffutils-0.7.4/src/jeffutils.egg-info/PKG-INFO` & `jeffutils-0.7.5/src/jeffutils.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeffutils
-Version: 0.7.4
+Version: 0.7.5
 Summary: Welcome to Jeff Hansen's suite of useful python functions! I use lots of these functions on most of my Data Analysis, Backend-Dev, and Machine Learning projects, and I hope you find some of them useful as well!
 Home-page: https://github.com/jeffxhansen/jeffutils
 Author: Jeff Hansen
 Author-email: jeffxhansen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

