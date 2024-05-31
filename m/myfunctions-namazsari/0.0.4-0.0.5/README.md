# Comparing `tmp/myfunctions_namazsari-0.0.4.tar.gz` & `tmp/myfunctions_namazsari-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/namazsari/python-class/evolvecyber/class5/dist/tmpdsyyrya4/myfunctions_namazsari-0.0.4.tar", last modified: Fri May 31 16:16:47 2024, max compression
+gzip compressed data, was "/mnt/namazsari/python-class/evolvecyber/class5/dist/tmpk2bu_z98/myfunctions_namazsari-0.0.5.tar", last modified: Fri May 31 16:24:20 2024, max compression
```

## Comparing `myfunctions_namazsari-0.0.4.tar` & `myfunctions_namazsari-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 namazsari  (1677) namazsari  (1678)        0 2024-05-31 16:16:47.000000 myfunctions_namazsari-0.0.4/
--rw-rw-r--   0 namazsari  (1677) namazsari  (1678)      635 2024-05-31 16:16:31.000000 myfunctions_namazsari-0.0.4/setup.py
-drwxrwxr-x   0 namazsari  (1677) namazsari  (1678)        0 2024-05-31 16:16:47.000000 myfunctions_namazsari-0.0.4/myfunctions_namazsari/
--rw-rw-r--   0 namazsari  (1677) namazsari  (1678)      258 2024-05-31 16:16:10.000000 myfunctions_namazsari-0.0.4/myfunctions_namazsari/math.py
--rw-rw-r--   0 namazsari  (1677) namazsari  (1678)        0 2024-05-31 14:59:26.000000 myfunctions_namazsari-0.0.4/myfunctions_namazsari/__init__.py
-drwxrwxr-x   0 namazsari  (1677) namazsari  (1678)        0 2024-05-31 16:16:47.000000 myfunctions_namazsari-0.0.4/myfunctions_namazsari.egg-info/
--rw-rw-r--   0 namazsari  (1677) namazsari  (1678)       22 2024-05-31 16:16:47.000000 myfunctions_namazsari-0.0.4/myfunctions_namazsari.egg-info/top_level.txt
--rw-rw-r--   0 namazsari  (1677) namazsari  (1678)      262 2024-05-31 16:16:47.000000 myfunctions_namazsari-0.0.4/myfunctions_namazsari.egg-info/SOURCES.txt
--rw-rw-r--   0 namazsari  (1677) namazsari  (1678)        1 2024-05-31 16:16:47.000000 myfunctions_namazsari-0.0.4/myfunctions_namazsari.egg-info/dependency_links.txt
--rw-rw-r--   0 namazsari  (1677) namazsari  (1678)     2843 2024-05-31 16:16:47.000000 myfunctions_namazsari-0.0.4/myfunctions_namazsari.egg-info/PKG-INFO
--rw-rw-r--   0 namazsari  (1677) namazsari  (1678)     2399 2024-05-31 16:03:23.000000 myfunctions_namazsari-0.0.4/README.md
--rw-rw-r--   0 namazsari  (1677) namazsari  (1678)     2843 2024-05-31 16:16:47.000000 myfunctions_namazsari-0.0.4/PKG-INFO
--rw-rw-r--   0 namazsari  (1677) namazsari  (1678)       38 2024-05-31 16:16:47.000000 myfunctions_namazsari-0.0.4/setup.cfg
+drwxrwxr-x   0 namazsari  (1677) namazsari  (1678)        0 2024-05-31 16:24:20.000000 myfunctions_namazsari-0.0.5/
+-rw-rw-r--   0 namazsari  (1677) namazsari  (1678)      635 2024-05-31 16:24:09.000000 myfunctions_namazsari-0.0.5/setup.py
+drwxrwxr-x   0 namazsari  (1677) namazsari  (1678)        0 2024-05-31 16:24:20.000000 myfunctions_namazsari-0.0.5/myfunctions_namazsari/
+-rw-rw-r--   0 namazsari  (1677) namazsari  (1678)      258 2024-05-31 16:16:10.000000 myfunctions_namazsari-0.0.5/myfunctions_namazsari/math.py
+-rw-rw-r--   0 namazsari  (1677) namazsari  (1678)        0 2024-05-31 14:59:26.000000 myfunctions_namazsari-0.0.5/myfunctions_namazsari/__init__.py
+drwxrwxr-x   0 namazsari  (1677) namazsari  (1678)        0 2024-05-31 16:24:20.000000 myfunctions_namazsari-0.0.5/myfunctions_namazsari.egg-info/
+-rw-rw-r--   0 namazsari  (1677) namazsari  (1678)       22 2024-05-31 16:24:20.000000 myfunctions_namazsari-0.0.5/myfunctions_namazsari.egg-info/top_level.txt
+-rw-rw-r--   0 namazsari  (1677) namazsari  (1678)      262 2024-05-31 16:24:20.000000 myfunctions_namazsari-0.0.5/myfunctions_namazsari.egg-info/SOURCES.txt
+-rw-rw-r--   0 namazsari  (1677) namazsari  (1678)        1 2024-05-31 16:24:20.000000 myfunctions_namazsari-0.0.5/myfunctions_namazsari.egg-info/dependency_links.txt
+-rw-rw-r--   0 namazsari  (1677) namazsari  (1678)     2843 2024-05-31 16:24:20.000000 myfunctions_namazsari-0.0.5/myfunctions_namazsari.egg-info/PKG-INFO
+-rw-rw-r--   0 namazsari  (1677) namazsari  (1678)     2399 2024-05-31 16:03:23.000000 myfunctions_namazsari-0.0.5/README.md
+-rw-rw-r--   0 namazsari  (1677) namazsari  (1678)     2843 2024-05-31 16:24:20.000000 myfunctions_namazsari-0.0.5/PKG-INFO
+-rw-rw-r--   0 namazsari  (1677) namazsari  (1678)       38 2024-05-31 16:24:20.000000 myfunctions_namazsari-0.0.5/setup.cfg
```

### Comparing `myfunctions_namazsari-0.0.4/setup.py` & `myfunctions_namazsari-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_namazsari',
-    version='0.0.4',
+    version='0.0.5',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/namazsari/',
     license='MIT',
     author='Namaz Sari',
     author_email='namazsariyev@gmail.com',
     description='A description of your package',
```

### Comparing `myfunctions_namazsari-0.0.4/myfunctions_namazsari.egg-info/PKG-INFO` & `myfunctions_namazsari-0.0.5/myfunctions_namazsari.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions-namazsari
-Version: 0.0.4
+Version: 0.0.5
 Summary: A description of your package
 Home-page: https://github.com/namazsari/
 Author: Namaz Sari
 Author-email: namazsariyev@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunctions_namazsari-0.0.4/README.md` & `myfunctions_namazsari-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `myfunctions_namazsari-0.0.4/PKG-INFO` & `myfunctions_namazsari-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions_namazsari
-Version: 0.0.4
+Version: 0.0.5
 Summary: A description of your package
 Home-page: https://github.com/namazsari/
 Author: Namaz Sari
 Author-email: namazsariyev@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

