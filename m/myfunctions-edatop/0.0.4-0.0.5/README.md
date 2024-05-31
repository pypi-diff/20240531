# Comparing `tmp/myfunctions_edatop-0.0.4.tar.gz` & `tmp/myfunctions_edatop-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/edatop/python-class/class5/dist/tmpevxfm4xr/myfunctions_edatop-0.0.4.tar", last modified: Fri May 31 03:35:45 2024, max compression
+gzip compressed data, was "/mnt/edatop/python-class/class5/dist/tmpij6gn65z/myfunctions_edatop-0.0.5.tar", last modified: Fri May 31 03:40:53 2024, max compression
```

## Comparing `myfunctions_edatop-0.0.4.tar` & `myfunctions_edatop-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 edatop    (1697) edatop    (1698)        0 2024-05-31 03:35:45.000000 myfunctions_edatop-0.0.4/
--rw-rw-r--   0 edatop    (1697) edatop    (1698)      623 2024-05-31 03:32:52.000000 myfunctions_edatop-0.0.4/setup.py
-drwxrwxr-x   0 edatop    (1697) edatop    (1698)        0 2024-05-31 03:35:45.000000 myfunctions_edatop-0.0.4/myfunctions_edatop.egg-info/
--rw-rw-r--   0 edatop    (1697) edatop    (1698)       19 2024-05-31 03:35:45.000000 myfunctions_edatop-0.0.4/myfunctions_edatop.egg-info/top_level.txt
--rw-rw-r--   0 edatop    (1697) edatop    (1698)      244 2024-05-31 03:35:45.000000 myfunctions_edatop-0.0.4/myfunctions_edatop.egg-info/SOURCES.txt
--rw-rw-r--   0 edatop    (1697) edatop    (1698)        1 2024-05-31 03:35:45.000000 myfunctions_edatop-0.0.4/myfunctions_edatop.egg-info/dependency_links.txt
--rw-rw-r--   0 edatop    (1697) edatop    (1698)     2228 2024-05-31 03:35:45.000000 myfunctions_edatop-0.0.4/myfunctions_edatop.egg-info/PKG-INFO
--rw-rw-r--   0 edatop    (1697) edatop    (1698)     1796 2024-05-31 03:17:11.000000 myfunctions_edatop-0.0.4/README.md
--rw-rw-r--   0 edatop    (1697) edatop    (1698)     2228 2024-05-31 03:35:45.000000 myfunctions_edatop-0.0.4/PKG-INFO
-drwxrwxr-x   0 edatop    (1697) edatop    (1698)        0 2024-05-31 03:35:45.000000 myfunctions_edatop-0.0.4/myfunctions_edatop/
--rw-rw-r--   0 edatop    (1697) edatop    (1698)      331 2024-05-31 03:32:43.000000 myfunctions_edatop-0.0.4/myfunctions_edatop/math.py
--rw-rw-r--   0 edatop    (1697) edatop    (1698)        0 2024-05-30 19:49:44.000000 myfunctions_edatop-0.0.4/myfunctions_edatop/__init__.py
--rw-rw-r--   0 edatop    (1697) edatop    (1698)       38 2024-05-31 03:35:45.000000 myfunctions_edatop-0.0.4/setup.cfg
+drwxrwxr-x   0 edatop    (1697) edatop    (1698)        0 2024-05-31 03:40:53.000000 myfunctions_edatop-0.0.5/
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)      623 2024-05-31 03:40:40.000000 myfunctions_edatop-0.0.5/setup.py
+drwxrwxr-x   0 edatop    (1697) edatop    (1698)        0 2024-05-31 03:40:52.000000 myfunctions_edatop-0.0.5/myfunctions_edatop.egg-info/
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)       19 2024-05-31 03:40:52.000000 myfunctions_edatop-0.0.5/myfunctions_edatop.egg-info/top_level.txt
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)      244 2024-05-31 03:40:52.000000 myfunctions_edatop-0.0.5/myfunctions_edatop.egg-info/SOURCES.txt
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)        1 2024-05-31 03:40:52.000000 myfunctions_edatop-0.0.5/myfunctions_edatop.egg-info/dependency_links.txt
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)     2228 2024-05-31 03:40:52.000000 myfunctions_edatop-0.0.5/myfunctions_edatop.egg-info/PKG-INFO
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)     1796 2024-05-31 03:17:11.000000 myfunctions_edatop-0.0.5/README.md
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)     2228 2024-05-31 03:40:53.000000 myfunctions_edatop-0.0.5/PKG-INFO
+drwxrwxr-x   0 edatop    (1697) edatop    (1698)        0 2024-05-31 03:40:52.000000 myfunctions_edatop-0.0.5/myfunctions_edatop/
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)      445 2024-05-31 03:40:14.000000 myfunctions_edatop-0.0.5/myfunctions_edatop/math.py
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)        0 2024-05-30 19:49:44.000000 myfunctions_edatop-0.0.5/myfunctions_edatop/__init__.py
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)       38 2024-05-31 03:40:53.000000 myfunctions_edatop-0.0.5/setup.cfg
```

### Comparing `myfunctions_edatop-0.0.4/setup.py` & `myfunctions_edatop-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_edatop',
-    version='0.0.4',
+    version='0.0.5',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/edatop/',
     license='MIT',
     author='Eda Top',
     author_email='edatp.hir@gmail.com',
     description='A description of your package',
```

### Comparing `myfunctions_edatop-0.0.4/myfunctions_edatop.egg-info/PKG-INFO` & `myfunctions_edatop-0.0.5/myfunctions_edatop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions-edatop
-Version: 0.0.4
+Version: 0.0.5
 Summary: A description of your package
 Home-page: https://github.com/edatop/
 Author: Eda Top
 Author-email: edatp.hir@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunctions_edatop-0.0.4/README.md` & `myfunctions_edatop-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `myfunctions_edatop-0.0.4/PKG-INFO` & `myfunctions_edatop-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions_edatop
-Version: 0.0.4
+Version: 0.0.5
 Summary: A description of your package
 Home-page: https://github.com/edatop/
 Author: Eda Top
 Author-email: edatp.hir@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

