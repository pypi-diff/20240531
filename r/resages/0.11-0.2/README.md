# Comparing `tmp/resages-0.11.tar.gz` & `tmp/resages-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resages-0.11.tar", last modified: Fri May 31 09:52:13 2024, max compression
+gzip compressed data, was "resages-0.2.tar", last modified: Fri May 31 10:16:34 2024, max compression
```

## Comparing `resages-0.11.tar` & `resages-0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 09:52:13.290733 resages-0.11/
--rw-rw-rw-   0        0        0      262 2024-05-31 09:52:13.290733 resages-0.11/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-31 09:52:13.244050 resages-0.11/resage/
--rw-rw-rw-   0        0        0        0 2024-05-31 08:12:38.000000 resages-0.11/resage/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 09:52:13.244050 resages-0.11/resage/colyear/
--rw-rw-rw-   0        0        0        0 2024-05-31 08:12:38.000000 resages-0.11/resage/colyear/__init__.py
--rw-rw-rw-   0        0        0     1932 2024-05-31 08:12:38.000000 resages-0.11/resage/colyear/abs.py
--rw-rw-rw-   0        0        0     5483 2024-05-31 08:12:38.000000 resages-0.11/resage/colyear/colyear.py
-drwxrwxrwx   0        0        0        0 2024-05-31 09:52:13.244050 resages-0.11/resage/rad2/
--rw-rw-rw-   0        0        0    11599 2024-05-31 08:12:38.000000 resages-0.11/resage/rad2/Rad2.py
--rw-rw-rw-   0        0        0        0 2024-05-31 08:12:38.000000 resages-0.11/resage/rad2/__init__.py
--rw-rw-rw-   0        0        0     1932 2024-05-31 08:12:38.000000 resages-0.11/resage/rad2/abs.py
-drwxrwxrwx   0        0        0        0 2024-05-31 09:52:13.244050 resages-0.11/resage/radical/
--rw-rw-rw-   0        0        0        0 2024-05-26 13:53:18.000000 resages-0.11/resage/radical/__init__.py
--rw-rw-rw-   0        0        0     1932 2024-05-28 05:16:31.000000 resages-0.11/resage/radical/abs.py
--rw-rw-rw-   0        0        0    36636 2024-05-31 08:12:38.000000 resages-0.11/resage/radical/radical.py
-drwxrwxrwx   0        0        0        0 2024-05-31 09:52:13.290733 resages-0.11/resages.egg-info/
--rw-rw-rw-   0        0        0      262 2024-05-31 09:52:13.000000 resages-0.11/resages.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2024-05-31 09:52:13.000000 resages-0.11/resages.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 09:52:13.000000 resages-0.11/resages.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-31 09:52:13.000000 resages-0.11/resages.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-31 09:52:13.000000 resages-0.11/resages.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 09:52:13.290733 resages-0.11/setup.cfg
--rw-rw-rw-   0        0        0      651 2024-05-31 09:51:57.000000 resages-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 10:16:34.720601 resages-0.2/
+-rw-rw-rw-   0        0        0      261 2024-05-31 10:16:34.714578 resages-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-31 10:16:34.535993 resages-0.2/resages/
+-rw-rw-rw-   0        0        0        0 2024-05-31 08:12:38.000000 resages-0.2/resages/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 10:16:34.651615 resages-0.2/resages/colyear/
+-rw-rw-rw-   0        0        0        0 2024-05-31 08:12:38.000000 resages-0.2/resages/colyear/__init__.py
+-rw-rw-rw-   0        0        0     1932 2024-05-31 08:12:38.000000 resages-0.2/resages/colyear/abs.py
+-rw-rw-rw-   0        0        0     5483 2024-05-31 08:12:38.000000 resages-0.2/resages/colyear/colyear.py
+drwxrwxrwx   0        0        0        0 2024-05-31 10:16:34.680619 resages-0.2/resages/rad2/
+-rw-rw-rw-   0        0        0    11599 2024-05-31 08:12:38.000000 resages-0.2/resages/rad2/Rad2.py
+-rw-rw-rw-   0        0        0        0 2024-05-31 08:12:38.000000 resages-0.2/resages/rad2/__init__.py
+-rw-rw-rw-   0        0        0     1932 2024-05-31 08:12:38.000000 resages-0.2/resages/rad2/abs.py
+drwxrwxrwx   0        0        0        0 2024-05-31 10:16:34.713605 resages-0.2/resages/radical/
+-rw-rw-rw-   0        0        0        0 2024-05-26 13:53:18.000000 resages-0.2/resages/radical/__init__.py
+-rw-rw-rw-   0        0        0     1932 2024-05-28 05:16:31.000000 resages-0.2/resages/radical/abs.py
+-rw-rw-rw-   0        0        0    36636 2024-05-31 08:12:38.000000 resages-0.2/resages/radical/radical.py
+drwxrwxrwx   0        0        0        0 2024-05-31 10:16:34.607995 resages-0.2/resages.egg-info/
+-rw-rw-rw-   0        0        0      261 2024-05-31 10:16:34.000000 resages-0.2/resages.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      404 2024-05-31 10:16:34.000000 resages-0.2/resages.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 10:16:34.000000 resages-0.2/resages.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-31 10:16:34.000000 resages-0.2/resages.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-31 10:16:34.000000 resages-0.2/resages.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 10:16:34.720601 resages-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      652 2024-05-31 10:09:10.000000 resages-0.2/setup.py
```

### Comparing `resages-0.11/resage/colyear/abs.py` & `resages-0.2/resages/colyear/abs.py`

 * *Files identical despite different names*

### Comparing `resages-0.11/resage/colyear/colyear.py` & `resages-0.2/resages/colyear/colyear.py`

 * *Files identical despite different names*

### Comparing `resages-0.11/resage/rad2/Rad2.py` & `resages-0.2/resages/rad2/Rad2.py`

 * *Files identical despite different names*

### Comparing `resages-0.11/resage/rad2/abs.py` & `resages-0.2/resages/rad2/abs.py`

 * *Files identical despite different names*

### Comparing `resages-0.11/resage/radical/abs.py` & `resages-0.2/resages/radical/abs.py`

 * *Files identical despite different names*

### Comparing `resages-0.11/resage/radical/radical.py` & `resages-0.2/resages/radical/radical.py`

 * *Files identical despite different names*

### Comparing `resages-0.11/setup.py` & `resages-0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='resages',
-    version='0.11',
+    version='0.2',
     py_modules=['resages'],
-    packages=find_packages(include=['resage', 'resage.*']),
+    packages=find_packages(include=['resages', 'resages.*']),
     
     install_requires=[
         
          'numpy',
          'pandas',
          'scipy',
          'tqdm',
```

