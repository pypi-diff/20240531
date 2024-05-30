# Comparing `tmp/cropimg-0.1.2.tar.gz` & `tmp/cropimg-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cropimg-0.1.2.tar", last modified: Wed May 29 12:10:05 2024, max compression
+gzip compressed data, was "cropimg-0.2.0.tar", last modified: Thu May 30 23:36:36 2024, max compression
```

## Comparing `cropimg-0.1.2.tar` & `cropimg-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-29 12:10:05.049324 cropimg-0.1.2/
--rw-r--r--   0 iuchi      (501) staff       (20)     1068 2024-05-28 13:09:12.000000 cropimg-0.1.2/LICENSE
--rw-r--r--   0 iuchi      (501) staff       (20)      361 2024-05-29 12:10:05.049189 cropimg-0.1.2/PKG-INFO
--rw-r--r--   0 iuchi      (501) staff       (20)     1817 2024-05-28 23:25:40.000000 cropimg-0.1.2/README.md
-drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-29 12:10:05.048168 cropimg-0.1.2/crop_image/
--rw-r--r--   0 iuchi      (501) staff       (20)        0 2024-05-28 12:52:37.000000 cropimg-0.1.2/crop_image/__init__.py
--rwxr-xr-x   0 iuchi      (501) staff       (20)     3426 2024-05-29 12:06:32.000000 cropimg-0.1.2/crop_image/cropimg.py
--rw-r--r--   0 iuchi      (501) staff       (20)      647 2024-05-28 07:17:22.000000 cropimg-0.1.2/crop_image/update_image.py
--rw-r--r--   0 iuchi      (501) staff       (20)      660 2024-05-29 11:56:14.000000 cropimg-0.1.2/crop_image/update_image_adb.py
--rw-r--r--   0 iuchi      (501) staff       (20)     1153 2024-05-29 12:07:43.000000 cropimg-0.1.2/crop_image/update_image_desktop.py
-drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-29 12:10:05.048994 cropimg-0.1.2/cropimg.egg-info/
--rw-r--r--   0 iuchi      (501) staff       (20)      361 2024-05-29 12:10:05.000000 cropimg-0.1.2/cropimg.egg-info/PKG-INFO
--rw-r--r--   0 iuchi      (501) staff       (20)      352 2024-05-29 12:10:05.000000 cropimg-0.1.2/cropimg.egg-info/SOURCES.txt
--rw-r--r--   0 iuchi      (501) staff       (20)        1 2024-05-29 12:10:05.000000 cropimg-0.1.2/cropimg.egg-info/dependency_links.txt
--rw-r--r--   0 iuchi      (501) staff       (20)       52 2024-05-29 12:10:05.000000 cropimg-0.1.2/cropimg.egg-info/entry_points.txt
--rw-r--r--   0 iuchi      (501) staff       (20)       32 2024-05-29 12:10:05.000000 cropimg-0.1.2/cropimg.egg-info/requires.txt
--rw-r--r--   0 iuchi      (501) staff       (20)       11 2024-05-29 12:10:05.000000 cropimg-0.1.2/cropimg.egg-info/top_level.txt
--rw-r--r--   0 iuchi      (501) staff       (20)       38 2024-05-29 12:10:05.049364 cropimg-0.1.2/setup.cfg
--rw-r--r--   0 iuchi      (501) staff       (20)      680 2024-05-29 12:09:01.000000 cropimg-0.1.2/setup.py
+drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-30 23:36:36.051283 cropimg-0.2.0/
+-rw-r--r--   0 iuchi      (501) staff       (20)     1068 2024-05-28 13:09:12.000000 cropimg-0.2.0/LICENSE
+-rw-r--r--   0 iuchi      (501) staff       (20)      361 2024-05-30 23:36:36.051146 cropimg-0.2.0/PKG-INFO
+-rw-r--r--   0 iuchi      (501) staff       (20)     1817 2024-05-28 23:25:40.000000 cropimg-0.2.0/README.md
+drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-30 23:36:36.049978 cropimg-0.2.0/crop_image/
+-rw-r--r--   0 iuchi      (501) staff       (20)        0 2024-05-28 12:52:37.000000 cropimg-0.2.0/crop_image/__init__.py
+-rwxr-xr-x   0 iuchi      (501) staff       (20)     3426 2024-05-29 12:06:32.000000 cropimg-0.2.0/crop_image/cropimg.py
+-rw-r--r--   0 iuchi      (501) staff       (20)      647 2024-05-28 07:17:22.000000 cropimg-0.2.0/crop_image/update_image.py
+-rw-r--r--   0 iuchi      (501) staff       (20)      660 2024-05-29 11:56:14.000000 cropimg-0.2.0/crop_image/update_image_adb.py
+-rw-r--r--   0 iuchi      (501) staff       (20)     1153 2024-05-29 12:07:43.000000 cropimg-0.2.0/crop_image/update_image_desktop.py
+drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-30 23:36:36.050970 cropimg-0.2.0/cropimg.egg-info/
+-rw-r--r--   0 iuchi      (501) staff       (20)      361 2024-05-30 23:36:36.000000 cropimg-0.2.0/cropimg.egg-info/PKG-INFO
+-rw-r--r--   0 iuchi      (501) staff       (20)      352 2024-05-30 23:36:36.000000 cropimg-0.2.0/cropimg.egg-info/SOURCES.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)        1 2024-05-30 23:36:36.000000 cropimg-0.2.0/cropimg.egg-info/dependency_links.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)       52 2024-05-30 23:36:36.000000 cropimg-0.2.0/cropimg.egg-info/entry_points.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)       32 2024-05-30 23:36:36.000000 cropimg-0.2.0/cropimg.egg-info/requires.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)       11 2024-05-30 23:36:36.000000 cropimg-0.2.0/cropimg.egg-info/top_level.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)       38 2024-05-30 23:36:36.051339 cropimg-0.2.0/setup.cfg
+-rw-r--r--   0 iuchi      (501) staff       (20)      681 2024-05-30 23:36:05.000000 cropimg-0.2.0/setup.py
```

### Comparing `cropimg-0.1.2/LICENSE` & `cropimg-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cropimg-0.1.2/README.md` & `cropimg-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cropimg-0.1.2/crop_image/cropimg.py` & `cropimg-0.2.0/crop_image/cropimg.py`

 * *Files identical despite different names*

### Comparing `cropimg-0.1.2/crop_image/update_image.py` & `cropimg-0.2.0/crop_image/update_image.py`

 * *Files identical despite different names*

### Comparing `cropimg-0.1.2/crop_image/update_image_adb.py` & `cropimg-0.2.0/crop_image/update_image_adb.py`

 * *Files identical despite different names*

### Comparing `cropimg-0.1.2/crop_image/update_image_desktop.py` & `cropimg-0.2.0/crop_image/update_image_desktop.py`

 * *Files identical despite different names*

### Comparing `cropimg-0.1.2/setup.py` & `cropimg-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cropimg',
-    version='0.1.2',
+    version='0.2.0',
     packages=find_packages(),
     install_requires=[
         'Flask',
         'pillow',
         'adb-tool-py>=0.1.2',
     ],
     entry_points={
@@ -20,8 +20,8 @@
     license='MIT',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
     keywords='crop, image, adb, screenshot',
     url='https://github.com/ShotaIuchi/crop-image',
-)
+)
```

