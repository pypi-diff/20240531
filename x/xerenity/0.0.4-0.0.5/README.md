# Comparing `tmp/xerenity-0.0.4.tar.gz` & `tmp/xerenity-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xerenity-0.0.4.tar", last modified: Fri May 31 15:52:32 2024, max compression
+gzip compressed data, was "xerenity-0.0.5.tar", last modified: Fri May 31 15:59:03 2024, max compression
```

## Comparing `xerenity-0.0.4.tar` & `xerenity-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:32.335926 xerenity-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:23.000000 xerenity-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-31 15:52:32.335926 xerenity-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:52:32.335926 xerenity-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-31 15:52:23.000000 xerenity-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:32.331926 xerenity-0.0.4/xerenity/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-31 15:52:23.000000 xerenity-0.0.4/xerenity/Xerenity.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-31 15:52:23.000000 xerenity-0.0.4/xerenity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:32.335926 xerenity-0.0.4/xerenity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-31 15:52:32.000000 xerenity-0.0.4/xerenity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-31 15:52:32.000000 xerenity-0.0.4/xerenity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:52:32.000000 xerenity-0.0.4/xerenity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-31 15:52:32.000000 xerenity-0.0.4/xerenity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 15:52:32.000000 xerenity-0.0.4/xerenity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:59:03.834955 xerenity-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:58:54.000000 xerenity-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-31 15:59:03.834955 xerenity-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:59:03.834955 xerenity-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-31 15:58:54.000000 xerenity-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:59:03.830955 xerenity-0.0.5/xerenity/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-31 15:58:54.000000 xerenity-0.0.5/xerenity/Xerenity.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-31 15:58:54.000000 xerenity-0.0.5/xerenity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:59:03.834955 xerenity-0.0.5/xerenity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-31 15:59:03.000000 xerenity-0.0.5/xerenity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-31 15:59:03.000000 xerenity-0.0.5/xerenity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:59:03.000000 xerenity-0.0.5/xerenity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-31 15:59:03.000000 xerenity-0.0.5/xerenity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 15:59:03.000000 xerenity-0.0.5/xerenity.egg-info/top_level.txt
```

### Comparing `xerenity-0.0.4/PKG-INFO` & `xerenity-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xerenity
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package for xerenity
 Home-page: https://xerenity.vercel.app/login
 Author: Andres Velez
 Author-email: svelez@xerenity.co
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `xerenity-0.0.4/setup.py` & `xerenity-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='xerenity',
-    version='0.0.4',
+    version='0.0.5',
     description='Python package for xerenity',
     url='https://xerenity.vercel.app/login',
     author='Andres Velez',
     author_email='svelez@xerenity.co',
     license='BSD 2-clause',
     packages=['xerenity'],
     install_requires=['supabase>=2.4.4','pandas'],
```

### Comparing `xerenity-0.0.4/xerenity.egg-info/PKG-INFO` & `xerenity-0.0.5/xerenity.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xerenity
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package for xerenity
 Home-page: https://xerenity.vercel.app/login
 Author: Andres Velez
 Author-email: svelez@xerenity.co
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

