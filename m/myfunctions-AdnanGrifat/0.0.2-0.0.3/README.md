# Comparing `tmp/myfunctions_AdnanGrifat-0.0.2.tar.gz` & `tmp/myfunctions_AdnanGrifat-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/AdnanGrifat/python-class/evolvecyber/class5/dist/tmpigtmfaah/myfunctions_AdnanGrifat-0.0.2.tar", last modified: Fri May 31 02:37:53 2024, max compression
+gzip compressed data, was "/mnt/AdnanGrifat/python-class/evolvecyber/class5/dist/tmphltudvs6/myfunctions_AdnanGrifat-0.0.3.tar", last modified: Fri May 31 02:40:06 2024, max compression
```

## Comparing `myfunctions_AdnanGrifat-0.0.2.tar` & `myfunctions_AdnanGrifat-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 AdnanGrifat  (1694) AdnanGrifat  (1695)        0 2024-05-31 02:37:53.000000 myfunctions_AdnanGrifat-0.0.2/
--rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)      639 2024-05-31 02:36:48.000000 myfunctions_AdnanGrifat-0.0.2/setup.py
--rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)        0 2024-05-31 01:27:35.000000 myfunctions_AdnanGrifat-0.0.2/README.md
--rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)      455 2024-05-31 02:37:53.000000 myfunctions_AdnanGrifat-0.0.2/PKG-INFO
-drwxrwxr-x   0 AdnanGrifat  (1694) AdnanGrifat  (1695)        0 2024-05-31 02:37:53.000000 myfunctions_AdnanGrifat-0.0.2/myfunctions_AdnanGrifat.egg-info/
--rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)        1 2024-05-31 02:37:53.000000 myfunctions_AdnanGrifat-0.0.2/myfunctions_AdnanGrifat.egg-info/top_level.txt
--rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)      206 2024-05-31 02:37:53.000000 myfunctions_AdnanGrifat-0.0.2/myfunctions_AdnanGrifat.egg-info/SOURCES.txt
--rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)        1 2024-05-31 02:37:53.000000 myfunctions_AdnanGrifat-0.0.2/myfunctions_AdnanGrifat.egg-info/dependency_links.txt
--rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)      455 2024-05-31 02:37:53.000000 myfunctions_AdnanGrifat-0.0.2/myfunctions_AdnanGrifat.egg-info/PKG-INFO
--rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)       38 2024-05-31 02:37:53.000000 myfunctions_AdnanGrifat-0.0.2/setup.cfg
+drwxrwxr-x   0 AdnanGrifat  (1694) AdnanGrifat  (1695)        0 2024-05-31 02:40:06.000000 myfunctions_AdnanGrifat-0.0.3/
+-rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)      639 2024-05-31 02:39:47.000000 myfunctions_AdnanGrifat-0.0.3/setup.py
+-rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)        0 2024-05-31 01:27:35.000000 myfunctions_AdnanGrifat-0.0.3/README.md
+-rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)      455 2024-05-31 02:40:06.000000 myfunctions_AdnanGrifat-0.0.3/PKG-INFO
+drwxrwxr-x   0 AdnanGrifat  (1694) AdnanGrifat  (1695)        0 2024-05-31 02:40:06.000000 myfunctions_AdnanGrifat-0.0.3/myfunctions_AdnanGrifat.egg-info/
+-rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)        1 2024-05-31 02:40:06.000000 myfunctions_AdnanGrifat-0.0.3/myfunctions_AdnanGrifat.egg-info/top_level.txt
+-rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)      206 2024-05-31 02:40:06.000000 myfunctions_AdnanGrifat-0.0.3/myfunctions_AdnanGrifat.egg-info/SOURCES.txt
+-rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)        1 2024-05-31 02:40:06.000000 myfunctions_AdnanGrifat-0.0.3/myfunctions_AdnanGrifat.egg-info/dependency_links.txt
+-rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)      455 2024-05-31 02:40:06.000000 myfunctions_AdnanGrifat-0.0.3/myfunctions_AdnanGrifat.egg-info/PKG-INFO
+-rw-rw-r--   0 AdnanGrifat  (1694) AdnanGrifat  (1695)       38 2024-05-31 02:40:06.000000 myfunctions_AdnanGrifat-0.0.3/setup.cfg
```

### Comparing `myfunctions_AdnanGrifat-0.0.2/setup.py` & `myfunctions_AdnanGrifat-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_AdnanGrifat',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/AdnanGrifat/',
     license='MIT',
     author='Adnan Grifat',
     author_email='grifat1978@gmail.com',
     description='A description of your package',
```

