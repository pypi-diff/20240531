# Comparing `tmp/copious-0.1.14.tar.gz` & `tmp/copious-0.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copious-0.1.14.tar", last modified: Mon May 27 11:22:21 2024, max compression
+gzip compressed data, was "copious-0.1.15.tar", last modified: Fri May 31 10:53:08 2024, max compression
```

## Comparing `copious-0.1.14.tar` & `copious-0.1.15.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-27 11:22:21.110617 copious-0.1.14/
--rw-r--r--   0 rlan       (501) staff       (20)      386 2024-05-27 11:22:21.110455 copious-0.1.14/PKG-INFO
--rw-r--r--   0 rlan       (501) staff       (20)      124 2024-05-07 10:00:56.000000 copious-0.1.14/README.md
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-27 11:22:21.105904 copious-0.1.14/copious/
--rw-r--r--   0 rlan       (501) staff       (20)        0 2024-05-07 09:54:59.000000 copious-0.1.14/copious/__init__.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-27 11:22:21.107047 copious-0.1.14/copious/cv/
--rw-r--r--   0 rlan       (501) staff       (20)        0 2024-05-07 09:54:59.000000 copious-0.1.14/copious/cv/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)     4859 2024-05-27 11:22:15.000000 copious-0.1.14/copious/cv/geometry.py
--rw-r--r--   0 rlan       (501) staff       (20)     2900 2024-05-07 09:54:59.000000 copious-0.1.14/copious/cv/graphics.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-27 11:22:21.107506 copious-0.1.14/copious/data_structure/
--rw-r--r--   0 rlan       (501) staff       (20)        0 2024-05-07 09:54:59.000000 copious-0.1.14/copious/data_structure/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)      646 2024-05-07 09:54:59.000000 copious-0.1.14/copious/data_structure/set.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-27 11:22:21.109429 copious-0.1.14/copious/io/
--rw-r--r--   0 rlan       (501) staff       (20)        0 2024-05-07 09:54:59.000000 copious-0.1.14/copious/io/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)      671 2024-05-07 09:54:59.000000 copious-0.1.14/copious/io/args.py
--rw-r--r--   0 rlan       (501) staff       (20)     1763 2024-05-07 09:54:59.000000 copious-0.1.14/copious/io/fs.py
--rw-r--r--   0 rlan       (501) staff       (20)     2686 2024-05-07 09:54:59.000000 copious-0.1.14/copious/io/indices.py
--rw-r--r--   0 rlan       (501) staff       (20)      682 2024-05-07 09:54:59.000000 copious-0.1.14/copious/io/network.py
--rw-r--r--   0 rlan       (501) staff       (20)     1441 2024-05-07 09:54:59.000000 copious-0.1.14/copious/io/parallelism.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-27 11:22:21.110143 copious-0.1.14/copious/plot/
--rw-r--r--   0 rlan       (501) staff       (20)      118 2024-05-07 09:54:59.000000 copious-0.1.14/copious/plot/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)     1256 2024-05-07 09:54:59.000000 copious-0.1.14/copious/plot/color.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-27 11:22:21.106629 copious-0.1.14/copious.egg-info/
--rw-r--r--   0 rlan       (501) staff       (20)      386 2024-05-27 11:22:21.000000 copious-0.1.14/copious.egg-info/PKG-INFO
--rw-r--r--   0 rlan       (501) staff       (20)      502 2024-05-27 11:22:21.000000 copious-0.1.14/copious.egg-info/SOURCES.txt
--rw-r--r--   0 rlan       (501) staff       (20)        1 2024-05-27 11:22:21.000000 copious-0.1.14/copious.egg-info/dependency_links.txt
--rw-r--r--   0 rlan       (501) staff       (20)       42 2024-05-27 11:22:21.000000 copious-0.1.14/copious.egg-info/requires.txt
--rw-r--r--   0 rlan       (501) staff       (20)        8 2024-05-27 11:22:21.000000 copious-0.1.14/copious.egg-info/top_level.txt
--rw-r--r--   0 rlan       (501) staff       (20)       38 2024-05-27 11:22:21.110685 copious-0.1.14/setup.cfg
--rw-r--r--   0 rlan       (501) staff       (20)      553 2024-05-27 11:22:15.000000 copious-0.1.14/setup.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-31 10:53:08.624105 copious-0.1.15/
+-rw-r--r--   0 rlan       (501) staff       (20)      386 2024-05-31 10:53:08.623964 copious-0.1.15/PKG-INFO
+-rw-r--r--   0 rlan       (501) staff       (20)      124 2024-05-07 10:00:56.000000 copious-0.1.15/README.md
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-31 10:53:08.620705 copious-0.1.15/copious/
+-rw-r--r--   0 rlan       (501) staff       (20)        0 2024-05-07 09:54:59.000000 copious-0.1.15/copious/__init__.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-31 10:53:08.621860 copious-0.1.15/copious/cv/
+-rw-r--r--   0 rlan       (501) staff       (20)        0 2024-05-07 09:54:59.000000 copious-0.1.15/copious/cv/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)     4859 2024-05-27 11:22:15.000000 copious-0.1.15/copious/cv/geometry.py
+-rw-r--r--   0 rlan       (501) staff       (20)     2900 2024-05-07 09:54:59.000000 copious-0.1.15/copious/cv/graphics.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-31 10:53:08.622271 copious-0.1.15/copious/data_structure/
+-rw-r--r--   0 rlan       (501) staff       (20)        0 2024-05-07 09:54:59.000000 copious-0.1.15/copious/data_structure/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)      646 2024-05-07 09:54:59.000000 copious-0.1.15/copious/data_structure/set.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-31 10:53:08.623386 copious-0.1.15/copious/io/
+-rw-r--r--   0 rlan       (501) staff       (20)        0 2024-05-07 09:54:59.000000 copious-0.1.15/copious/io/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1159 2024-05-31 10:43:48.000000 copious-0.1.15/copious/io/args.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1763 2024-05-07 09:54:59.000000 copious-0.1.15/copious/io/fs.py
+-rw-r--r--   0 rlan       (501) staff       (20)     2686 2024-05-07 09:54:59.000000 copious-0.1.15/copious/io/indices.py
+-rw-r--r--   0 rlan       (501) staff       (20)      682 2024-05-07 09:54:59.000000 copious-0.1.15/copious/io/network.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1441 2024-05-07 09:54:59.000000 copious-0.1.15/copious/io/parallelism.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-31 10:53:08.623753 copious-0.1.15/copious/plot/
+-rw-r--r--   0 rlan       (501) staff       (20)      118 2024-05-07 09:54:59.000000 copious-0.1.15/copious/plot/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1256 2024-05-07 09:54:59.000000 copious-0.1.15/copious/plot/color.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-31 10:53:08.621275 copious-0.1.15/copious.egg-info/
+-rw-r--r--   0 rlan       (501) staff       (20)      386 2024-05-31 10:53:08.000000 copious-0.1.15/copious.egg-info/PKG-INFO
+-rw-r--r--   0 rlan       (501) staff       (20)      502 2024-05-31 10:53:08.000000 copious-0.1.15/copious.egg-info/SOURCES.txt
+-rw-r--r--   0 rlan       (501) staff       (20)        1 2024-05-31 10:53:08.000000 copious-0.1.15/copious.egg-info/dependency_links.txt
+-rw-r--r--   0 rlan       (501) staff       (20)       42 2024-05-31 10:53:08.000000 copious-0.1.15/copious.egg-info/requires.txt
+-rw-r--r--   0 rlan       (501) staff       (20)        8 2024-05-31 10:53:08.000000 copious-0.1.15/copious.egg-info/top_level.txt
+-rw-r--r--   0 rlan       (501) staff       (20)       38 2024-05-31 10:53:08.624146 copious-0.1.15/setup.cfg
+-rw-r--r--   0 rlan       (501) staff       (20)      553 2024-05-31 10:37:42.000000 copious-0.1.15/setup.py
```

### Comparing `copious-0.1.14/copious/cv/geometry.py` & `copious-0.1.15/copious/cv/geometry.py`

 * *Files identical despite different names*

### Comparing `copious-0.1.14/copious/cv/graphics.py` & `copious-0.1.15/copious/cv/graphics.py`

 * *Files identical despite different names*

### Comparing `copious-0.1.14/copious/data_structure/set.py` & `copious-0.1.15/copious/data_structure/set.py`

 * *Files identical despite different names*

### Comparing `copious-0.1.14/copious/io/fs.py` & `copious-0.1.15/copious/io/fs.py`

 * *Files identical despite different names*

### Comparing `copious-0.1.14/copious/io/indices.py` & `copious-0.1.15/copious/io/indices.py`

 * *Files identical despite different names*

### Comparing `copious-0.1.14/copious/io/network.py` & `copious-0.1.15/copious/io/network.py`

 * *Files identical despite different names*

### Comparing `copious-0.1.14/copious/io/parallelism.py` & `copious-0.1.15/copious/io/parallelism.py`

 * *Files identical despite different names*

### Comparing `copious-0.1.14/copious/plot/color.py` & `copious-0.1.15/copious/plot/color.py`

 * *Files identical despite different names*

### Comparing `copious-0.1.14/setup.py` & `copious-0.1.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='copious',
-    version='0.1.14',
+    version='0.1.15',
     packages=find_packages(),
     description='A handy tool that make your day to day programming much easier. ',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='brianlan',
     author_email='brianlanbo@gmail.com',
     url='https://gitlab.com/rlan/copious',
```

