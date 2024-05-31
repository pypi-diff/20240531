# Comparing `tmp/myfunction_vikmin2022-0.1.tar.gz` & `tmp/myfunction_vikmin2022-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/Vikmin2022/Python_class/Class5/dist/tmpusb0gmdv/myfunction_vikmin2022-0.1.tar", last modified: Thu May 30 22:11:40 2024, max compression
+gzip compressed data, was "/mnt/Vikmin2022/Python_class/Class5/dist/tmphoypg274/myfunction_vikmin2022-0.2.tar", last modified: Fri May 31 01:22:09 2024, max compression
```

## Comparing `myfunction_vikmin2022-0.1.tar` & `myfunction_vikmin2022-0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 Vikmin2022  (1652) Vikmin2022  (1653)        0 2024-05-30 22:11:40.000000 myfunction_vikmin2022-0.1/
--rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)      648 2024-05-30 01:03:18.000000 myfunction_vikmin2022-0.1/setup.py
-drwxrwxr-x   0 Vikmin2022  (1652) Vikmin2022  (1653)        0 2024-05-30 22:11:40.000000 myfunction_vikmin2022-0.1/myfunction_vikmin2022.egg-info/
--rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)        1 2024-05-30 22:11:40.000000 myfunction_vikmin2022-0.1/myfunction_vikmin2022.egg-info/top_level.txt
--rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)      198 2024-05-30 22:11:40.000000 myfunction_vikmin2022-0.1/myfunction_vikmin2022.egg-info/SOURCES.txt
--rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)        1 2024-05-30 22:11:40.000000 myfunction_vikmin2022-0.1/myfunction_vikmin2022.egg-info/dependency_links.txt
--rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)      473 2024-05-30 22:11:40.000000 myfunction_vikmin2022-0.1/myfunction_vikmin2022.egg-info/PKG-INFO
--rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)       17 2024-05-30 01:19:10.000000 myfunction_vikmin2022-0.1/README.md
--rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)      473 2024-05-30 22:11:40.000000 myfunction_vikmin2022-0.1/PKG-INFO
--rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)       38 2024-05-30 22:11:40.000000 myfunction_vikmin2022-0.1/setup.cfg
+drwxrwxr-x   0 Vikmin2022  (1652) Vikmin2022  (1653)        0 2024-05-31 01:22:09.000000 myfunction_vikmin2022-0.2/
+-rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)      648 2024-05-31 01:21:53.000000 myfunction_vikmin2022-0.2/setup.py
+drwxrwxr-x   0 Vikmin2022  (1652) Vikmin2022  (1653)        0 2024-05-31 01:22:09.000000 myfunction_vikmin2022-0.2/myfunction_vikmin2022.egg-info/
+-rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)        1 2024-05-31 01:22:09.000000 myfunction_vikmin2022-0.2/myfunction_vikmin2022.egg-info/top_level.txt
+-rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)      198 2024-05-31 01:22:09.000000 myfunction_vikmin2022-0.2/myfunction_vikmin2022.egg-info/SOURCES.txt
+-rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)        1 2024-05-31 01:22:09.000000 myfunction_vikmin2022-0.2/myfunction_vikmin2022.egg-info/dependency_links.txt
+-rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)      662 2024-05-31 01:22:09.000000 myfunction_vikmin2022-0.2/myfunction_vikmin2022.egg-info/PKG-INFO
+-rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)      206 2024-05-31 01:17:47.000000 myfunction_vikmin2022-0.2/README.md
+-rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)      662 2024-05-31 01:22:09.000000 myfunction_vikmin2022-0.2/PKG-INFO
+-rw-rw-r--   0 Vikmin2022  (1652) Vikmin2022  (1653)       38 2024-05-31 01:22:09.000000 myfunction_vikmin2022-0.2/setup.cfg
```

### Comparing `myfunction_vikmin2022-0.1/setup.py` & `myfunction_vikmin2022-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunction_vikmin2022',
-    version='0.01',
+    version='0.02',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/vikmin2022',
     license='MIT',
     author='Viktoriia Minosian',
     author_email='viktoriia.minosian@gmail.com',
     description='A description of your package',
```

