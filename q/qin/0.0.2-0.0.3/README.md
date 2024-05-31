# Comparing `tmp/qin-0.0.2.tar.gz` & `tmp/qin-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qin-0.0.2.tar", last modified: Sun Oct  8 13:35:22 2023, max compression
+gzip compressed data, was "qin-0.0.3.tar", last modified: Fri May 31 11:36:10 2024, max compression
```

## Comparing `qin-0.0.2.tar` & `qin-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 13:35:22.867274 qin-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-10-08 13:35:12.000000 qin-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      391 2023-10-08 13:35:22.867274 qin-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      818 2023-10-08 13:35:12.000000 qin-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 13:35:22.863274 qin-0.0.2/qin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-08 13:35:12.000000 qin-0.0.2/qin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 13:35:22.867274 qin-0.0.2/qin/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-08 13:35:12.000000 qin-0.0.2/qin/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-10-08 13:35:12.000000 qin-0.0.2/qin/common/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2023-10-08 13:35:12.000000 qin-0.0.2/qin/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2023-10-08 13:35:12.000000 qin-0.0.2/qin/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2023-10-08 13:35:12.000000 qin-0.0.2/qin/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2023-10-08 13:35:12.000000 qin-0.0.2/qin/media.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 13:35:22.867274 qin-0.0.2/qin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2023-10-08 13:35:22.000000 qin-0.0.2/qin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-10-08 13:35:22.000000 qin-0.0.2/qin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-08 13:35:22.000000 qin-0.0.2/qin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-10-08 13:35:22.000000 qin-0.0.2/qin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-08 13:35:22.000000 qin-0.0.2/qin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-08 13:35:22.000000 qin-0.0.2/qin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-08 13:35:22.867274 qin-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      702 2023-10-08 13:35:12.000000 qin-0.0.2/setup.py
+drwxr-xr-x   0 kinda      (501) staff       (20)        0 2024-05-31 11:36:10.801419 qin-0.0.3/
+-rw-r--r--   0 kinda      (501) staff       (20)     1067 2024-05-27 15:51:03.000000 qin-0.0.3/LICENSE
+-rw-r--r--   0 kinda      (501) staff       (20)      455 2024-05-31 11:36:10.801185 qin-0.0.3/PKG-INFO
+-rw-r--r--   0 kinda      (501) staff       (20)      722 2024-05-30 16:09:13.000000 qin-0.0.3/README.md
+drwxr-xr-x   0 kinda      (501) staff       (20)        0 2024-05-31 11:36:10.798431 qin-0.0.3/qin/
+-rw-r--r--   0 kinda      (501) staff       (20)        0 2024-05-27 15:51:03.000000 qin-0.0.3/qin/__init__.py
+drwxr-xr-x   0 kinda      (501) staff       (20)        0 2024-05-31 11:36:10.799774 qin-0.0.3/qin/common/
+-rw-r--r--   0 kinda      (501) staff       (20)        0 2024-05-27 15:51:03.000000 qin-0.0.3/qin/common/__init__.py
+-rw-r--r--   0 kinda      (501) staff       (20)      286 2024-05-27 15:51:03.000000 qin-0.0.3/qin/common/file.py
+-rw-r--r--   0 kinda      (501) staff       (20)     1383 2024-05-27 15:51:03.000000 qin-0.0.3/qin/common/logger.py
+drwxr-xr-x   0 kinda      (501) staff       (20)        0 2024-05-31 11:36:10.800434 qin-0.0.3/qin/config/
+-rw-r--r--   0 kinda      (501) staff       (20)        0 2024-05-27 15:51:03.000000 qin-0.0.3/qin/config/__init__.py
+-rw-r--r--   0 kinda      (501) staff       (20)      189 2024-05-27 15:51:03.000000 qin-0.0.3/qin/config/base.py
+-rw-r--r--   0 kinda      (501) staff       (20)      625 2024-05-31 08:10:34.000000 qin-0.0.3/qin/config/config.py
+-rw-r--r--   0 kinda      (501) staff       (20)     3476 2024-05-31 08:55:27.000000 qin-0.0.3/qin/file.py
+-rw-r--r--   0 kinda      (501) staff       (20)      806 2024-05-27 15:51:03.000000 qin-0.0.3/qin/main.py
+-rw-r--r--   0 kinda      (501) staff       (20)     1643 2024-05-31 07:34:09.000000 qin-0.0.3/qin/media.py
+drwxr-xr-x   0 kinda      (501) staff       (20)        0 2024-05-31 11:36:10.800887 qin-0.0.3/qin.egg-info/
+-rw-r--r--   0 kinda      (501) staff       (20)      455 2024-05-31 11:36:10.000000 qin-0.0.3/qin.egg-info/PKG-INFO
+-rw-r--r--   0 kinda      (501) staff       (20)      369 2024-05-31 11:36:10.000000 qin-0.0.3/qin.egg-info/SOURCES.txt
+-rw-r--r--   0 kinda      (501) staff       (20)        1 2024-05-31 11:36:10.000000 qin-0.0.3/qin.egg-info/dependency_links.txt
+-rw-r--r--   0 kinda      (501) staff       (20)       37 2024-05-31 11:36:10.000000 qin-0.0.3/qin.egg-info/entry_points.txt
+-rw-r--r--   0 kinda      (501) staff       (20)       39 2024-05-31 11:36:10.000000 qin-0.0.3/qin.egg-info/requires.txt
+-rw-r--r--   0 kinda      (501) staff       (20)        4 2024-05-31 11:36:10.000000 qin-0.0.3/qin.egg-info/top_level.txt
+-rw-r--r--   0 kinda      (501) staff       (20)       38 2024-05-31 11:36:10.801463 qin-0.0.3/setup.cfg
+-rw-r--r--   0 kinda      (501) staff       (20)      730 2024-05-31 11:36:05.000000 qin-0.0.3/setup.py
```

### Comparing `qin-0.0.2/LICENSE` & `qin-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qin-0.0.2/qin/common/logger.py` & `qin-0.0.3/qin/common/logger.py`

 * *Files identical despite different names*

### Comparing `qin-0.0.2/setup.py` & `qin-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 from setuptools import setup, find_packages
 
 setup(
     name="qin",
-    version="0.0.2",
+    version="0.0.3",
     keywords=("pip", "tools"),
     description="cli tool",
     entry_points={
         'console_scripts': [
             'qin = qin.main:app'
         ]
     },
@@ -19,9 +19,9 @@
     author="Kinda Hall",
     maintainer="Kinda Hall",
     maintainer_email="1142704468@qq.com",
     author_email="1142704468@qq.com",
     packages=find_packages(),
     include_package_data=True,
     platforms="any",
-    install_requires=['typer', 'ffmpeg-python']
+    install_requires=['typer', 'ffmpeg-python', 'oss2', 'gradio', 'yt-dlp']
 )
```

