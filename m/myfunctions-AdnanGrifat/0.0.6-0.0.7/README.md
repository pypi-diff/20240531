# Comparing `tmp/myfunctions_AdnanGrifat-0.0.6.tar.gz` & `tmp/myfunctions_AdnanGrifat-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/AdnanGrifat/python-class/evolvecyber/class5/dist/tmp_rkz1rn4/myfunctions_AdnanGrifat-0.0.6.tar", last modified: Fri May 31 02:47:43 2024, max compression
+gzip compressed data, was "/mnt/AdnanGrifat/python-class/evolvecyber/class5/dist/tmpshn96mhj/myfunctions_AdnanGrifat-0.0.7.tar", last modified: Fri May 31 03:01:44 2024, max compression
```

## Comparing `myfunctions_AdnanGrifat-0.0.6.tar` & `myfunctions_AdnanGrifat-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxrwxr-x   0 AdnanGrifat  (1694) AdnanGrifat  (1695)        0 2024-05-31 02:47:43.000000 myfunctions_AdnanGrifat-0.0.6/
--rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)      639 2024-05-31 02:47:22.000000 myfunctions_AdnanGrifat-0.0.6/setup.py
--rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)     2028 2024-05-31 02:46:31.000000 myfunctions_AdnanGrifat-0.0.6/README.md
--rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)     2476 2024-05-31 02:47:43.000000 myfunctions_AdnanGrifat-0.0.6/PKG-INFO
-drwxrwxr-x   0 AdnanGrifat  (1694) AdnanGrifat  (1695)        0 2024-05-31 02:47:43.000000 myfunctions_AdnanGrifat-0.0.6/myfunctions_AdnanGrifat.egg-info/
--rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)        1 2024-05-31 02:47:43.000000 myfunctions_AdnanGrifat-0.0.6/myfunctions_AdnanGrifat.egg-info/top_level.txt
--rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)      206 2024-05-31 02:47:43.000000 myfunctions_AdnanGrifat-0.0.6/myfunctions_AdnanGrifat.egg-info/SOURCES.txt
--rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)        1 2024-05-31 02:47:43.000000 myfunctions_AdnanGrifat-0.0.6/myfunctions_AdnanGrifat.egg-info/dependency_links.txt
--rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)     2476 2024-05-31 02:47:43.000000 myfunctions_AdnanGrifat-0.0.6/myfunctions_AdnanGrifat.egg-info/PKG-INFO
--rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)       38 2024-05-31 02:47:43.000000 myfunctions_AdnanGrifat-0.0.6/setup.cfg
+drwxrwxr-x   0 AdnanGrifat  (1694) AdnanGrifat  (1695)        0 2024-05-31 03:01:44.000000 myfunctions_AdnanGrifat-0.0.7/
+-rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)      639 2024-05-31 03:01:23.000000 myfunctions_AdnanGrifat-0.0.7/setup.py
+-rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)     2028 2024-05-31 02:46:31.000000 myfunctions_AdnanGrifat-0.0.7/README.md
+-rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)     2476 2024-05-31 03:01:44.000000 myfunctions_AdnanGrifat-0.0.7/PKG-INFO
+drwxrwxr-x   0 AdnanGrifat  (1694) AdnanGrifat  (1695)        0 2024-05-31 03:01:44.000000 myfunctions_AdnanGrifat-0.0.7/myfunctions_AdnanGrifat.egg-info/
+-rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)        1 2024-05-31 03:01:44.000000 myfunctions_AdnanGrifat-0.0.7/myfunctions_AdnanGrifat.egg-info/top_level.txt
+-rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)      248 2024-05-31 03:01:44.000000 myfunctions_AdnanGrifat-0.0.7/myfunctions_AdnanGrifat.egg-info/SOURCES.txt
+-rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)       71 2024-05-31 02:57:42.000000 myfunctions_AdnanGrifat-0.0.7/myfunctions_AdnanGrifat.egg-info/Makefile
+-rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)        1 2024-05-31 03:01:44.000000 myfunctions_AdnanGrifat-0.0.7/myfunctions_AdnanGrifat.egg-info/dependency_links.txt
+-rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)     2476 2024-05-31 03:01:44.000000 myfunctions_AdnanGrifat-0.0.7/myfunctions_AdnanGrifat.egg-info/PKG-INFO
+-rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)       38 2024-05-31 03:01:44.000000 myfunctions_AdnanGrifat-0.0.7/setup.cfg
```

### Comparing `myfunctions_AdnanGrifat-0.0.6/setup.py` & `myfunctions_AdnanGrifat-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_AdnanGrifat',
-    version='0.0.6',
+    version='0.0.7',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/AdnanGrifat/',
     license='MIT',
     author='Adnan Grifat',
     author_email='grifat1978@gmail.com',
     description='A description of your package',
```

### Comparing `myfunctions_AdnanGrifat-0.0.6/README.md` & `myfunctions_AdnanGrifat-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `myfunctions_AdnanGrifat-0.0.6/PKG-INFO` & `myfunctions_AdnanGrifat-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions_AdnanGrifat
-Version: 0.0.6
+Version: 0.0.7
 Summary: A description of your package
 Home-page: https://github.com/AdnanGrifat/
 Author: Adnan Grifat
 Author-email: grifat1978@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunctions_AdnanGrifat-0.0.6/myfunctions_AdnanGrifat.egg-info/PKG-INFO` & `myfunctions_AdnanGrifat-0.0.7/myfunctions_AdnanGrifat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions-AdnanGrifat
-Version: 0.0.6
+Version: 0.0.7
 Summary: A description of your package
 Home-page: https://github.com/AdnanGrifat/
 Author: Adnan Grifat
 Author-email: grifat1978@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

