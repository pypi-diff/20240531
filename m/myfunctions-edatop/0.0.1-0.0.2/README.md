# Comparing `tmp/myfunctions_edatop-0.0.1.tar.gz` & `tmp/myfunctions_edatop-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/edatop/python-class/class5/dist/tmpkelq8_yk/myfunctions_edatop-0.0.1.tar", last modified: Thu May 30 20:00:43 2024, max compression
+gzip compressed data, was "/mnt/edatop/python-class/class5/dist/tmpl4xb81y1/myfunctions_edatop-0.0.2.tar", last modified: Thu May 30 20:16:27 2024, max compression
```

## Comparing `myfunctions_edatop-0.0.1.tar` & `myfunctions_edatop-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 edatop    (1697) edatop    (1698)        0 2024-05-30 20:00:43.000000 myfunctions_edatop-0.0.1/
--rw-rw-r--   0 edatop    (1697) edatop    (1698)      623 2024-05-30 19:58:53.000000 myfunctions_edatop-0.0.1/setup.py
-drwxrwxr-x   0 edatop    (1697) edatop    (1698)        0 2024-05-30 20:00:43.000000 myfunctions_edatop-0.0.1/myfunctions_edatop.egg-info/
--rw-rw-r--   0 edatop    (1697) edatop    (1698)       19 2024-05-30 20:00:43.000000 myfunctions_edatop-0.0.1/myfunctions_edatop.egg-info/top_level.txt
--rw-rw-r--   0 edatop    (1697) edatop    (1698)      244 2024-05-30 20:00:43.000000 myfunctions_edatop-0.0.1/myfunctions_edatop.egg-info/SOURCES.txt
--rw-rw-r--   0 edatop    (1697) edatop    (1698)        1 2024-05-30 20:00:42.000000 myfunctions_edatop-0.0.1/myfunctions_edatop.egg-info/dependency_links.txt
--rw-rw-r--   0 edatop    (1697) edatop    (1698)      439 2024-05-30 20:00:42.000000 myfunctions_edatop-0.0.1/myfunctions_edatop.egg-info/PKG-INFO
--rw-rw-r--   0 edatop    (1697) edatop    (1698)        0 2024-05-30 19:48:59.000000 myfunctions_edatop-0.0.1/README.md
--rw-rw-r--   0 edatop    (1697) edatop    (1698)      439 2024-05-30 20:00:43.000000 myfunctions_edatop-0.0.1/PKG-INFO
-drwxrwxr-x   0 edatop    (1697) edatop    (1698)        0 2024-05-30 20:00:43.000000 myfunctions_edatop-0.0.1/myfunctions_edatop/
--rw-rw-r--   0 edatop    (1697) edatop    (1698)      105 2024-05-30 19:56:07.000000 myfunctions_edatop-0.0.1/myfunctions_edatop/math.py
--rw-rw-r--   0 edatop    (1697) edatop    (1698)        0 2024-05-30 19:49:44.000000 myfunctions_edatop-0.0.1/myfunctions_edatop/__init__.py
--rw-rw-r--   0 edatop    (1697) edatop    (1698)       38 2024-05-30 20:00:43.000000 myfunctions_edatop-0.0.1/setup.cfg
+drwxrwxr-x   0 edatop    (1697) edatop    (1698)        0 2024-05-30 20:16:27.000000 myfunctions_edatop-0.0.2/
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)      623 2024-05-30 20:15:33.000000 myfunctions_edatop-0.0.2/setup.py
+drwxrwxr-x   0 edatop    (1697) edatop    (1698)        0 2024-05-30 20:16:27.000000 myfunctions_edatop-0.0.2/myfunctions_edatop.egg-info/
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)       19 2024-05-30 20:16:26.000000 myfunctions_edatop-0.0.2/myfunctions_edatop.egg-info/top_level.txt
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)      244 2024-05-30 20:16:26.000000 myfunctions_edatop-0.0.2/myfunctions_edatop.egg-info/SOURCES.txt
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)        1 2024-05-30 20:16:26.000000 myfunctions_edatop-0.0.2/myfunctions_edatop.egg-info/dependency_links.txt
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)      439 2024-05-30 20:16:26.000000 myfunctions_edatop-0.0.2/myfunctions_edatop.egg-info/PKG-INFO
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)        0 2024-05-30 19:48:59.000000 myfunctions_edatop-0.0.2/README.md
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)      439 2024-05-30 20:16:27.000000 myfunctions_edatop-0.0.2/PKG-INFO
+drwxrwxr-x   0 edatop    (1697) edatop    (1698)        0 2024-05-30 20:16:27.000000 myfunctions_edatop-0.0.2/myfunctions_edatop/
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)      172 2024-05-30 20:15:25.000000 myfunctions_edatop-0.0.2/myfunctions_edatop/math.py
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)        0 2024-05-30 19:49:44.000000 myfunctions_edatop-0.0.2/myfunctions_edatop/__init__.py
+-rw-rw-r--   0 edatop    (1697) edatop    (1698)       38 2024-05-30 20:16:27.000000 myfunctions_edatop-0.0.2/setup.cfg
```

### Comparing `myfunctions_edatop-0.0.1/setup.py` & `myfunctions_edatop-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_edatop',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/edatop/',
     license='MIT',
     author='Eda Top',
     author_email='edatp.hir@gmail.com',
     description='A description of your package',
```

