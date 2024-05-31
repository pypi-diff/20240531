# Comparing `tmp/myfunctions_namazsari-0.0.1.tar.gz` & `tmp/myfunctions_namazsari-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/namazsari/python-class/evolvecyber/class5/dist/tmpx39rmrgn/myfunctions_namazsari-0.0.1.tar", last modified: Fri May 31 15:16:27 2024, max compression
+gzip compressed data, was "/mnt/namazsari/python-class/evolvecyber/class5/dist/tmp74poldud/myfunctions_namazsari-0.0.2.tar", last modified: Fri May 31 15:52:58 2024, max compression
```

## Comparing `myfunctions_namazsari-0.0.1.tar` & `myfunctions_namazsari-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 namazsari  (1677) namazsari  (1678)        0 2024-05-31 15:16:27.000000 myfunctions_namazsari-0.0.1/
--rw-rw-r--   0 namazsari  (1677) namazsari  (1678)      635 2024-05-31 15:15:13.000000 myfunctions_namazsari-0.0.1/setup.py
-drwxrwxr-x   0 namazsari  (1677) namazsari  (1678)        0 2024-05-31 15:16:27.000000 myfunctions_namazsari-0.0.1/myfunctions_namazsari/
--rw-rw-r--   0 namazsari  (1677) namazsari  (1678)      108 2024-05-31 15:10:29.000000 myfunctions_namazsari-0.0.1/myfunctions_namazsari/math.py
--rw-rw-r--   0 namazsari  (1677) namazsari  (1678)        0 2024-05-31 14:59:26.000000 myfunctions_namazsari-0.0.1/myfunctions_namazsari/__init__.py
-drwxrwxr-x   0 namazsari  (1677) namazsari  (1678)        0 2024-05-31 15:16:27.000000 myfunctions_namazsari-0.0.1/myfunctions_namazsari.egg-info/
--rw-rw-r--   0 namazsari  (1677) namazsari  (1678)       22 2024-05-31 15:16:27.000000 myfunctions_namazsari-0.0.1/myfunctions_namazsari.egg-info/top_level.txt
--rw-rw-r--   0 namazsari  (1677) namazsari  (1678)      262 2024-05-31 15:16:27.000000 myfunctions_namazsari-0.0.1/myfunctions_namazsari.egg-info/SOURCES.txt
--rw-rw-r--   0 namazsari  (1677) namazsari  (1678)        1 2024-05-31 15:16:27.000000 myfunctions_namazsari-0.0.1/myfunctions_namazsari.egg-info/dependency_links.txt
--rw-rw-r--   0 namazsari  (1677) namazsari  (1678)      451 2024-05-31 15:16:27.000000 myfunctions_namazsari-0.0.1/myfunctions_namazsari.egg-info/PKG-INFO
--rw-rw-r--   0 namazsari  (1677) namazsari  (1678)        0 2024-05-31 14:58:45.000000 myfunctions_namazsari-0.0.1/README.md
--rw-rw-r--   0 namazsari  (1677) namazsari  (1678)      451 2024-05-31 15:16:27.000000 myfunctions_namazsari-0.0.1/PKG-INFO
--rw-rw-r--   0 namazsari  (1677) namazsari  (1678)       38 2024-05-31 15:16:27.000000 myfunctions_namazsari-0.0.1/setup.cfg
+drwxrwxr-x   0 namazsari  (1677) namazsari  (1678)        0 2024-05-31 15:52:58.000000 myfunctions_namazsari-0.0.2/
+-rw-rw-r--   0 namazsari  (1677) namazsari  (1678)      635 2024-05-31 15:52:27.000000 myfunctions_namazsari-0.0.2/setup.py
+drwxrwxr-x   0 namazsari  (1677) namazsari  (1678)        0 2024-05-31 15:52:57.000000 myfunctions_namazsari-0.0.2/myfunctions_namazsari/
+-rw-rw-r--   0 namazsari  (1677) namazsari  (1678)      176 2024-05-31 15:51:40.000000 myfunctions_namazsari-0.0.2/myfunctions_namazsari/math.py
+-rw-rw-r--   0 namazsari  (1677) namazsari  (1678)        0 2024-05-31 14:59:26.000000 myfunctions_namazsari-0.0.2/myfunctions_namazsari/__init__.py
+drwxrwxr-x   0 namazsari  (1677) namazsari  (1678)        0 2024-05-31 15:52:58.000000 myfunctions_namazsari-0.0.2/myfunctions_namazsari.egg-info/
+-rw-rw-r--   0 namazsari  (1677) namazsari  (1678)       22 2024-05-31 15:52:57.000000 myfunctions_namazsari-0.0.2/myfunctions_namazsari.egg-info/top_level.txt
+-rw-rw-r--   0 namazsari  (1677) namazsari  (1678)      262 2024-05-31 15:52:57.000000 myfunctions_namazsari-0.0.2/myfunctions_namazsari.egg-info/SOURCES.txt
+-rw-rw-r--   0 namazsari  (1677) namazsari  (1678)        1 2024-05-31 15:52:57.000000 myfunctions_namazsari-0.0.2/myfunctions_namazsari.egg-info/dependency_links.txt
+-rw-rw-r--   0 namazsari  (1677) namazsari  (1678)      451 2024-05-31 15:52:57.000000 myfunctions_namazsari-0.0.2/myfunctions_namazsari.egg-info/PKG-INFO
+-rw-rw-r--   0 namazsari  (1677) namazsari  (1678)        0 2024-05-31 14:58:45.000000 myfunctions_namazsari-0.0.2/README.md
+-rw-rw-r--   0 namazsari  (1677) namazsari  (1678)      451 2024-05-31 15:52:58.000000 myfunctions_namazsari-0.0.2/PKG-INFO
+-rw-rw-r--   0 namazsari  (1677) namazsari  (1678)       38 2024-05-31 15:52:58.000000 myfunctions_namazsari-0.0.2/setup.cfg
```

### Comparing `myfunctions_namazsari-0.0.1/setup.py` & `myfunctions_namazsari-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_namazsari',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/namazsari/',
     license='MIT',
     author='Namaz Sari',
     author_email='namazsariyev@gmail.com',
     description='A description of your package',
```

