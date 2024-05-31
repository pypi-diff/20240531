# Comparing `tmp/wxhandler-0.1.1.tar.gz` & `tmp/wxhandler-0.1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxhandler-0.1.1.tar", last modified: Fri May 31 00:01:53 2024, max compression
+gzip compressed data, was "wxhandler-0.1.1.1.tar", last modified: Fri May 31 00:05:47 2024, max compression
```

## Comparing `wxhandler-0.1.1.tar` & `wxhandler-0.1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 00:01:53.685370 wxhandler-0.1.1/
--rw-rw-rw-   0        0        0     1055 2024-05-30 23:10:26.000000 wxhandler-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      612 2024-05-31 00:01:53.683371 wxhandler-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      126 2024-05-30 23:08:56.000000 wxhandler-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-31 00:01:53.685370 wxhandler-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      678 2024-05-31 00:00:25.000000 wxhandler-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-31 00:01:53.667381 wxhandler-0.1.1/wxhandler/
--rw-rw-rw-   0        0        0        0 2024-05-30 23:05:42.000000 wxhandler-0.1.1/wxhandler/__init__.py
--rw-rw-rw-   0        0        0    23197 2024-05-30 15:38:25.000000 wxhandler-0.1.1/wxhandler/wxhandler.py
-drwxrwxrwx   0        0        0        0 2024-05-31 00:01:53.681372 wxhandler-0.1.1/wxhandler.egg-info/
--rw-rw-rw-   0        0        0      612 2024-05-31 00:01:53.000000 wxhandler-0.1.1/wxhandler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-05-31 00:01:53.000000 wxhandler-0.1.1/wxhandler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 00:01:53.000000 wxhandler-0.1.1/wxhandler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-31 00:01:53.000000 wxhandler-0.1.1/wxhandler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-31 00:01:53.000000 wxhandler-0.1.1/wxhandler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 00:05:47.809847 wxhandler-0.1.1.1/
+-rw-rw-rw-   0        0        0     1055 2024-05-30 23:10:26.000000 wxhandler-0.1.1.1/LICENSE
+-rw-rw-rw-   0        0        0      888 2024-05-31 00:05:47.808872 wxhandler-0.1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2024-05-31 00:04:24.000000 wxhandler-0.1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-31 00:05:47.810848 wxhandler-0.1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      680 2024-05-31 00:05:36.000000 wxhandler-0.1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 00:05:47.792476 wxhandler-0.1.1.1/wxhandler/
+-rw-rw-rw-   0        0        0        0 2024-05-30 23:05:42.000000 wxhandler-0.1.1.1/wxhandler/__init__.py
+-rw-rw-rw-   0        0        0    23197 2024-05-30 15:38:25.000000 wxhandler-0.1.1.1/wxhandler/wxhandler.py
+drwxrwxrwx   0        0        0        0 2024-05-31 00:05:47.805848 wxhandler-0.1.1.1/wxhandler.egg-info/
+-rw-rw-rw-   0        0        0      888 2024-05-31 00:05:47.000000 wxhandler-0.1.1.1/wxhandler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-05-31 00:05:47.000000 wxhandler-0.1.1.1/wxhandler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 00:05:47.000000 wxhandler-0.1.1.1/wxhandler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-31 00:05:47.000000 wxhandler-0.1.1.1/wxhandler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-31 00:05:47.000000 wxhandler-0.1.1.1/wxhandler.egg-info/top_level.txt
```

### Comparing `wxhandler-0.1.1/LICENSE` & `wxhandler-0.1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wxhandler-0.1.1/setup.py` & `wxhandler-0.1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="wxhandler",
-    version="0.1.1",
+    version="0.1.1.1",
     packages=find_packages(),
     install_requires=[
         "requests",
     ],
     author="chenbifu",
     author_email="pythonaaa@gmail.com",
     description="A Python package for handling wxHandler operations.",
```

### Comparing `wxhandler-0.1.1/wxhandler/wxhandler.py` & `wxhandler-0.1.1.1/wxhandler/wxhandler.py`

 * *Files identical despite different names*

