# Comparing `tmp/myfunctions_edatop-0.0.6.tar.gz` & `tmp/myfunctions_edatop-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/edatop/python-class/class5/dist/tmp7ilf9mz5/myfunctions_edatop-0.0.6.tar", last modified: Fri May 31 03:41:45 2024, max compression
+gzip compressed data, was "/mnt/edatop/python-class/class5/dist/tmpxolp5vht/myfunctions_edatop-0.0.7.tar", last modified: Fri May 31 03:45:17 2024, max compression
```

## Comparing `myfunctions_edatop-0.0.6.tar` & `myfunctions_edatop-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxr-x   0 edatop    (1697) edatop    (1698)        0 2024-05-31 03:41:45.000000 myfunctions_edatop-0.0.6/
--rw-rw-r--   0 edatop    (1697) edatop    (1698)      627 2024-05-31 03:41:28.000000 myfunctions_edatop-0.0.6/setup.py
-drwxrwxr-x   0 edatop    (1697) edatop    (1698)        0 2024-05-31 03:41:45.000000 myfunctions_edatop-0.0.6/myfunctions_edatop.egg-info/
--rw-rw-r--   0 edatop    (1697) edatop    (1698)       19 2024-05-31 03:41:45.000000 myfunctions_edatop-0.0.6/myfunctions_edatop.egg-info/top_level.txt
--rw-rw-r--   0 edatop    (1697) edatop    (1698)      285 2024-05-31 03:41:45.000000 myfunctions_edatop-0.0.6/myfunctions_edatop.egg-info/SOURCES.txt
--rw-rw-r--   0 edatop    (1697) edatop    (1698)        3 2024-05-31 03:41:45.000000 myfunctions_edatop-0.0.6/myfunctions_edatop.egg-info/requires.txt
--rw-rw-r--   0 edatop    (1697) edatop    (1698)        1 2024-05-31 03:41:45.000000 myfunctions_edatop-0.0.6/myfunctions_edatop.egg-info/dependency_links.txt
--rw-rw-r--   0 edatop    (1697) edatop    (1698)     2228 2024-05-31 03:41:45.000000 myfunctions_edatop-0.0.6/myfunctions_edatop.egg-info/PKG-INFO
--rw-rw-r--   0 edatop    (1697) edatop    (1698)     1796 2024-05-31 03:17:11.000000 myfunctions_edatop-0.0.6/README.md
--rw-rw-r--   0 edatop    (1697) edatop    (1698)     2228 2024-05-31 03:41:45.000000 myfunctions_edatop-0.0.6/PKG-INFO
-drwxrwxr-x   0 edatop    (1697) edatop    (1698)        0 2024-05-31 03:41:45.000000 myfunctions_edatop-0.0.6/myfunctions_edatop/
--rw-rw-r--   0 edatop    (1697) edatop    (1698)      445 2024-05-31 03:40:14.000000 myfunctions_edatop-0.0.6/myfunctions_edatop/math.py
--rw-rw-r--   0 edatop    (1697) edatop    (1698)        0 2024-05-30 19:49:44.000000 myfunctions_edatop-0.0.6/myfunctions_edatop/__init__.py
--rw-rw-r--   0 edatop    (1697) edatop    (1698)       38 2024-05-31 03:41:45.000000 myfunctions_edatop-0.0.6/setup.cfg
+drwxrwxr-x   0 edatop    (1697) edatop    (1698)        0 2024-05-31 03:45:17.000000 myfunctions_edatop-0.0.7/
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)      623 2024-05-31 03:45:07.000000 myfunctions_edatop-0.0.7/setup.py
+drwxrwxr-x   0 edatop    (1697) edatop    (1698)        0 2024-05-31 03:45:17.000000 myfunctions_edatop-0.0.7/myfunctions_edatop.egg-info/
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)       19 2024-05-31 03:45:17.000000 myfunctions_edatop-0.0.7/myfunctions_edatop.egg-info/top_level.txt
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)      244 2024-05-31 03:45:17.000000 myfunctions_edatop-0.0.7/myfunctions_edatop.egg-info/SOURCES.txt
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)        1 2024-05-31 03:45:17.000000 myfunctions_edatop-0.0.7/myfunctions_edatop.egg-info/dependency_links.txt
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)     2228 2024-05-31 03:45:17.000000 myfunctions_edatop-0.0.7/myfunctions_edatop.egg-info/PKG-INFO
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)     1796 2024-05-31 03:17:11.000000 myfunctions_edatop-0.0.7/README.md
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)     2228 2024-05-31 03:45:17.000000 myfunctions_edatop-0.0.7/PKG-INFO
+drwxrwxr-x   0 edatop    (1697) edatop    (1698)        0 2024-05-31 03:45:17.000000 myfunctions_edatop-0.0.7/myfunctions_edatop/
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)      445 2024-05-31 03:40:14.000000 myfunctions_edatop-0.0.7/myfunctions_edatop/math.py
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)        0 2024-05-30 19:49:44.000000 myfunctions_edatop-0.0.7/myfunctions_edatop/__init__.py
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)       38 2024-05-31 03:45:17.000000 myfunctions_edatop-0.0.7/setup.cfg
```

### Comparing `myfunctions_edatop-0.0.6/setup.py` & `myfunctions_edatop-0.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_edatop',
-    version='0.0.6',
+    version='0.0.7',
     packages=find_packages(),
-    install_requires=["os"],
+    install_requires=[],
     url='https://github.com/edatop/',
     license='MIT',
     author='Eda Top',
     author_email='edatp.hir@gmail.com',
     description='A description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `myfunctions_edatop-0.0.6/myfunctions_edatop.egg-info/PKG-INFO` & `myfunctions_edatop-0.0.7/myfunctions_edatop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions-edatop
-Version: 0.0.6
+Version: 0.0.7
 Summary: A description of your package
 Home-page: https://github.com/edatop/
 Author: Eda Top
 Author-email: edatp.hir@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunctions_edatop-0.0.6/README.md` & `myfunctions_edatop-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `myfunctions_edatop-0.0.6/PKG-INFO` & `myfunctions_edatop-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions_edatop
-Version: 0.0.6
+Version: 0.0.7
 Summary: A description of your package
 Home-page: https://github.com/edatop/
 Author: Eda Top
 Author-email: edatp.hir@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

