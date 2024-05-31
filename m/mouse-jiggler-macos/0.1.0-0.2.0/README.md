# Comparing `tmp/mouse_jiggler_macos-0.1.0.tar.gz` & `tmp/mouse_jiggler_macos-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mouse_jiggler_macos-0.1.0.tar", last modified: Thu May 30 05:10:08 2024, max compression
+gzip compressed data, was "mouse_jiggler_macos-0.2.0.tar", last modified: Thu May 30 05:19:34 2024, max compression
```

## Comparing `mouse_jiggler_macos-0.1.0.tar` & `mouse_jiggler_macos-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 umair      (501) staff       (20)        0 2024-05-30 05:10:08.712537 mouse_jiggler_macos-0.1.0/
--rw-r--r--   0 umair      (501) staff       (20)     2133 2024-05-30 05:10:08.712406 mouse_jiggler_macos-0.1.0/PKG-INFO
--rw-r--r--   0 umair      (501) staff       (20)     1719 2024-05-30 03:57:54.000000 mouse_jiggler_macos-0.1.0/README.md
-drwxr-xr-x   0 umair      (501) staff       (20)        0 2024-05-30 05:10:08.711340 mouse_jiggler_macos-0.1.0/mouse_jiggler/
--rw-r--r--   0 umair      (501) staff       (20)       44 2024-05-30 04:58:44.000000 mouse_jiggler_macos-0.1.0/mouse_jiggler/__init__.py
--rw-r--r--   0 umair      (501) staff       (20)     3713 2024-05-30 04:57:44.000000 mouse_jiggler_macos-0.1.0/mouse_jiggler/jiggler.py
-drwxr-xr-x   0 umair      (501) staff       (20)        0 2024-05-30 05:10:08.712235 mouse_jiggler_macos-0.1.0/mouse_jiggler_macos.egg-info/
--rw-r--r--   0 umair      (501) staff       (20)     2133 2024-05-30 05:10:08.000000 mouse_jiggler_macos-0.1.0/mouse_jiggler_macos.egg-info/PKG-INFO
--rw-r--r--   0 umair      (501) staff       (20)      329 2024-05-30 05:10:08.000000 mouse_jiggler_macos-0.1.0/mouse_jiggler_macos.egg-info/SOURCES.txt
--rw-r--r--   0 umair      (501) staff       (20)        1 2024-05-30 05:10:08.000000 mouse_jiggler_macos-0.1.0/mouse_jiggler_macos.egg-info/dependency_links.txt
--rw-r--r--   0 umair      (501) staff       (20)       61 2024-05-30 05:10:08.000000 mouse_jiggler_macos-0.1.0/mouse_jiggler_macos.egg-info/entry_points.txt
--rw-r--r--   0 umair      (501) staff       (20)       22 2024-05-30 05:10:08.000000 mouse_jiggler_macos-0.1.0/mouse_jiggler_macos.egg-info/requires.txt
--rw-r--r--   0 umair      (501) staff       (20)       14 2024-05-30 05:10:08.000000 mouse_jiggler_macos-0.1.0/mouse_jiggler_macos.egg-info/top_level.txt
--rw-r--r--   0 umair      (501) staff       (20)       38 2024-05-30 05:10:08.712577 mouse_jiggler_macos-0.1.0/setup.cfg
--rw-r--r--   0 umair      (501) staff       (20)      863 2024-05-30 05:09:51.000000 mouse_jiggler_macos-0.1.0/setup.py
+drwxr-xr-x   0 umair      (501) staff       (20)        0 2024-05-30 05:19:34.821276 mouse_jiggler_macos-0.2.0/
+-rw-r--r--   0 umair      (501) staff       (20)     2133 2024-05-30 05:19:34.821149 mouse_jiggler_macos-0.2.0/PKG-INFO
+-rw-r--r--   0 umair      (501) staff       (20)     1719 2024-05-30 03:57:54.000000 mouse_jiggler_macos-0.2.0/README.md
+drwxr-xr-x   0 umair      (501) staff       (20)        0 2024-05-30 05:19:34.819658 mouse_jiggler_macos-0.2.0/mouse_jiggler/
+-rw-r--r--   0 umair      (501) staff       (20)       44 2024-05-30 04:58:44.000000 mouse_jiggler_macos-0.2.0/mouse_jiggler/__init__.py
+-rw-r--r--   0 umair      (501) staff       (20)     3709 2024-05-30 05:17:59.000000 mouse_jiggler_macos-0.2.0/mouse_jiggler/jiggler.py
+drwxr-xr-x   0 umair      (501) staff       (20)        0 2024-05-30 05:19:34.820978 mouse_jiggler_macos-0.2.0/mouse_jiggler_macos.egg-info/
+-rw-r--r--   0 umair      (501) staff       (20)     2133 2024-05-30 05:19:34.000000 mouse_jiggler_macos-0.2.0/mouse_jiggler_macos.egg-info/PKG-INFO
+-rw-r--r--   0 umair      (501) staff       (20)      329 2024-05-30 05:19:34.000000 mouse_jiggler_macos-0.2.0/mouse_jiggler_macos.egg-info/SOURCES.txt
+-rw-r--r--   0 umair      (501) staff       (20)        1 2024-05-30 05:19:34.000000 mouse_jiggler_macos-0.2.0/mouse_jiggler_macos.egg-info/dependency_links.txt
+-rw-r--r--   0 umair      (501) staff       (20)       61 2024-05-30 05:19:34.000000 mouse_jiggler_macos-0.2.0/mouse_jiggler_macos.egg-info/entry_points.txt
+-rw-r--r--   0 umair      (501) staff       (20)       22 2024-05-30 05:19:34.000000 mouse_jiggler_macos-0.2.0/mouse_jiggler_macos.egg-info/requires.txt
+-rw-r--r--   0 umair      (501) staff       (20)       14 2024-05-30 05:19:34.000000 mouse_jiggler_macos-0.2.0/mouse_jiggler_macos.egg-info/top_level.txt
+-rw-r--r--   0 umair      (501) staff       (20)       38 2024-05-30 05:19:34.821317 mouse_jiggler_macos-0.2.0/setup.cfg
+-rw-r--r--   0 umair      (501) staff       (20)      863 2024-05-30 05:19:04.000000 mouse_jiggler_macos-0.2.0/setup.py
```

### Comparing `mouse_jiggler_macos-0.1.0/PKG-INFO` & `mouse_jiggler_macos-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mouse_jiggler_macos
-Version: 0.1.0
+Version: 0.2.0
 Summary: A simple mouse jiggler for MacOS
 Home-page: https://github.com/UmairK5669/mouse-jiggler
 Author: Umair Khan
 Author-email: u7khan@uwaterloo.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mouse_jiggler_macos-0.1.0/README.md` & `mouse_jiggler_macos-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mouse_jiggler_macos-0.1.0/mouse_jiggler/jiggler.py` & `mouse_jiggler_macos-0.2.0/mouse_jiggler/jiggler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import threading
 import time
 from pynput import keyboard
 import pyautogui
 import pync
 from pync import Notifier
 
-def executable():
+jiggler_running = False
 
-    jiggler_running = False
+def executable():
 
     def mouse_jiggler_function(movement_distance=5, interval=0.5):
         global jiggler_running
         screen_width, screen_height = pyautogui.size()
 
         # Initial delay with periodic checks to allow immediate stopping
         for _ in range(20):
```

### Comparing `mouse_jiggler_macos-0.1.0/mouse_jiggler_macos.egg-info/PKG-INFO` & `mouse_jiggler_macos-0.2.0/mouse_jiggler_macos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mouse-jiggler-macos
-Version: 0.1.0
+Version: 0.2.0
 Summary: A simple mouse jiggler for MacOS
 Home-page: https://github.com/UmairK5669/mouse-jiggler
 Author: Umair Khan
 Author-email: u7khan@uwaterloo.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mouse_jiggler_macos-0.1.0/setup.py` & `mouse_jiggler_macos-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mouse_jiggler_macos",
-    version="0.1.0",
+    version="0.2.0",
     author="Umair Khan",
     author_email="u7khan@uwaterloo.ca",
     description="A simple mouse jiggler for MacOS",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/UmairK5669/mouse-jiggler",
     packages=find_packages(),
```

