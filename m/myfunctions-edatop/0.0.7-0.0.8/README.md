# Comparing `tmp/myfunctions_edatop-0.0.7.tar.gz` & `tmp/myfunctions_edatop-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/edatop/python-class/class5/dist/tmpxolp5vht/myfunctions_edatop-0.0.7.tar", last modified: Fri May 31 03:45:17 2024, max compression
+gzip compressed data, was "/mnt/edatop/python-class/class5/dist/tmpppfr12k9/myfunctions_edatop-0.0.8.tar", last modified: Fri May 31 03:47:53 2024, max compression
```

## Comparing `myfunctions_edatop-0.0.7.tar` & `myfunctions_edatop-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 edatop    (1697) edatop    (1698)        0 2024-05-31 03:45:17.000000 myfunctions_edatop-0.0.7/
--rw-rw-r--   0 edatop    (1697) edatop    (1698)      623 2024-05-31 03:45:07.000000 myfunctions_edatop-0.0.7/setup.py
-drwxrwxr-x   0 edatop    (1697) edatop    (1698)        0 2024-05-31 03:45:17.000000 myfunctions_edatop-0.0.7/myfunctions_edatop.egg-info/
--rw-rw-r--   0 edatop    (1697) edatop    (1698)       19 2024-05-31 03:45:17.000000 myfunctions_edatop-0.0.7/myfunctions_edatop.egg-info/top_level.txt
--rw-rw-r--   0 edatop    (1697) edatop    (1698)      244 2024-05-31 03:45:17.000000 myfunctions_edatop-0.0.7/myfunctions_edatop.egg-info/SOURCES.txt
--rw-rw-r--   0 edatop    (1697) edatop    (1698)        1 2024-05-31 03:45:17.000000 myfunctions_edatop-0.0.7/myfunctions_edatop.egg-info/dependency_links.txt
--rw-rw-r--   0 edatop    (1697) edatop    (1698)     2228 2024-05-31 03:45:17.000000 myfunctions_edatop-0.0.7/myfunctions_edatop.egg-info/PKG-INFO
--rw-rw-r--   0 edatop    (1697) edatop    (1698)     1796 2024-05-31 03:17:11.000000 myfunctions_edatop-0.0.7/README.md
--rw-rw-r--   0 edatop    (1697) edatop    (1698)     2228 2024-05-31 03:45:17.000000 myfunctions_edatop-0.0.7/PKG-INFO
-drwxrwxr-x   0 edatop    (1697) edatop    (1698)        0 2024-05-31 03:45:17.000000 myfunctions_edatop-0.0.7/myfunctions_edatop/
--rw-rw-r--   0 edatop    (1697) edatop    (1698)      445 2024-05-31 03:40:14.000000 myfunctions_edatop-0.0.7/myfunctions_edatop/math.py
--rw-rw-r--   0 edatop    (1697) edatop    (1698)        0 2024-05-30 19:49:44.000000 myfunctions_edatop-0.0.7/myfunctions_edatop/__init__.py
--rw-rw-r--   0 edatop    (1697) edatop    (1698)       38 2024-05-31 03:45:17.000000 myfunctions_edatop-0.0.7/setup.cfg
+drwxrwxr-x   0 edatop    (1697) edatop    (1698)        0 2024-05-31 03:47:53.000000 myfunctions_edatop-0.0.8/
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)      623 2024-05-31 03:47:44.000000 myfunctions_edatop-0.0.8/setup.py
+drwxrwxr-x   0 edatop    (1697) edatop    (1698)        0 2024-05-31 03:47:53.000000 myfunctions_edatop-0.0.8/myfunctions_edatop.egg-info/
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)       19 2024-05-31 03:47:53.000000 myfunctions_edatop-0.0.8/myfunctions_edatop.egg-info/top_level.txt
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)      244 2024-05-31 03:47:53.000000 myfunctions_edatop-0.0.8/myfunctions_edatop.egg-info/SOURCES.txt
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)        1 2024-05-31 03:47:53.000000 myfunctions_edatop-0.0.8/myfunctions_edatop.egg-info/dependency_links.txt
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)     2228 2024-05-31 03:47:53.000000 myfunctions_edatop-0.0.8/myfunctions_edatop.egg-info/PKG-INFO
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)     1796 2024-05-31 03:17:11.000000 myfunctions_edatop-0.0.8/README.md
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)     2228 2024-05-31 03:47:53.000000 myfunctions_edatop-0.0.8/PKG-INFO
+drwxrwxr-x   0 edatop    (1697) edatop    (1698)        0 2024-05-31 03:47:53.000000 myfunctions_edatop-0.0.8/myfunctions_edatop/
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)      547 2024-05-31 03:47:29.000000 myfunctions_edatop-0.0.8/myfunctions_edatop/math.py
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)        0 2024-05-30 19:49:44.000000 myfunctions_edatop-0.0.8/myfunctions_edatop/__init__.py
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)       38 2024-05-31 03:47:53.000000 myfunctions_edatop-0.0.8/setup.cfg
```

### Comparing `myfunctions_edatop-0.0.7/setup.py` & `myfunctions_edatop-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_edatop',
-    version='0.0.7',
+    version='0.0.8',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/edatop/',
     license='MIT',
     author='Eda Top',
     author_email='edatp.hir@gmail.com',
     description='A description of your package',
```

### Comparing `myfunctions_edatop-0.0.7/myfunctions_edatop.egg-info/PKG-INFO` & `myfunctions_edatop-0.0.8/myfunctions_edatop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions-edatop
-Version: 0.0.7
+Version: 0.0.8
 Summary: A description of your package
 Home-page: https://github.com/edatop/
 Author: Eda Top
 Author-email: edatp.hir@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunctions_edatop-0.0.7/README.md` & `myfunctions_edatop-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `myfunctions_edatop-0.0.7/PKG-INFO` & `myfunctions_edatop-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions_edatop
-Version: 0.0.7
+Version: 0.0.8
 Summary: A description of your package
 Home-page: https://github.com/edatop/
 Author: Eda Top
 Author-email: edatp.hir@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

