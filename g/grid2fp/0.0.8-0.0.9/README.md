# Comparing `tmp/grid2fp-0.0.8.tar.gz` & `tmp/grid2fp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grid2fp-0.0.8.tar", last modified: Mon Oct 30 01:59:21 2023, max compression
+gzip compressed data, was "grid2fp-0.0.9.tar", last modified: Fri May 31 06:50:24 2024, max compression
```

## Comparing `grid2fp-0.0.8.tar` & `grid2fp-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 01:59:21.042840 grid2fp-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-10-30 01:58:49.000000 grid2fp-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2023-10-30 01:59:21.042840 grid2fp-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2023-10-30 01:58:49.000000 grid2fp-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 01:59:21.038839 grid2fp-0.0.8/grid2fp/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-10-30 01:58:49.000000 grid2fp-0.0.8/grid2fp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6071 2023-10-30 01:58:49.000000 grid2fp-0.0.8/grid2fp/grid2fp.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2023-10-30 01:58:49.000000 grid2fp-0.0.8/grid2fp/grid_segment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 01:59:21.042840 grid2fp-0.0.8/grid2fp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2023-10-30 01:59:21.000000 grid2fp-0.0.8/grid2fp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-10-30 01:59:21.000000 grid2fp-0.0.8/grid2fp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-30 01:59:21.000000 grid2fp-0.0.8/grid2fp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-30 01:59:21.000000 grid2fp-0.0.8/grid2fp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-30 01:59:21.000000 grid2fp-0.0.8/grid2fp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-30 01:59:21.042840 grid2fp-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      994 2023-10-30 01:58:49.000000 grid2fp-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 01:59:21.042840 grid2fp-0.0.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-10-30 01:58:49.000000 grid2fp-0.0.8/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2023-10-30 01:58:49.000000 grid2fp-0.0.8/test/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:50:24.059421 grid2fp-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-31 06:50:09.000000 grid2fp-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-31 06:50:24.059421 grid2fp-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-31 06:50:09.000000 grid2fp-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:50:24.059421 grid2fp-0.0.9/grid2fp/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-31 06:50:09.000000 grid2fp-0.0.9/grid2fp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-05-31 06:50:09.000000 grid2fp-0.0.9/grid2fp/grid2fp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-31 06:50:09.000000 grid2fp-0.0.9/grid2fp/grid_segment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:50:24.059421 grid2fp-0.0.9/grid2fp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-31 06:50:24.000000 grid2fp-0.0.9/grid2fp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-31 06:50:24.000000 grid2fp-0.0.9/grid2fp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 06:50:24.000000 grid2fp-0.0.9/grid2fp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 06:50:24.000000 grid2fp-0.0.9/grid2fp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-31 06:50:24.000000 grid2fp-0.0.9/grid2fp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 06:50:24.059421 grid2fp-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-31 06:50:09.000000 grid2fp-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:50:24.059421 grid2fp-0.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-31 06:50:09.000000 grid2fp-0.0.9/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-31 06:50:09.000000 grid2fp-0.0.9/test/test_integration.py
```

### Comparing `grid2fp-0.0.8/LICENSE` & `grid2fp-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `grid2fp-0.0.8/PKG-INFO` & `grid2fp-0.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grid2fp
-Version: 0.0.8
+Version: 0.0.9
 Summary: A tool to eat grid diagrams and generate its front projection.
 Home-page: https://github.com/Joecstarr/grid2fp
 Author: Joe Starr
 Keywords: topology,Legendrian,Grid Diagram,knot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -67,54 +67,55 @@
 
 g = grid2fp(csv_file=csv_path,string_color = "pink", crossing_color="purple")
 d = g.draw()
 # make some changes to d with drawsvg
 d.save_svg(svg_path)
 
 ```
-# Sample images
+## Sample images
 
 x|o| | |
 -|-|-|-|
  |x|o| |
  | |x|o|
 o| | |x|
 
-<img  style="background:white;width:400px;height:auto" src="https://github.com/Joecstarr/grid2fp/blob/main/test/random.svg"/>
+<img  style="width:400px;height:auto" src="https://raw.githubusercontent.com/Joecstarr/grid2fp/main/test/random.svg"/>
 
 
 o| | |x| |
 -|-|-|-|-|
  | |x| |o|
  |x| |o| |
 x| |o| | |
  |o| | |x|
 
 
-<img  style="background:white;width:400px;height:auto" src="https://github.com/Joecstarr/grid2fp/blob/main/test/trefoil.svg"/>
+<img  style="width:400px;height:auto" src="https://raw.githubusercontent.com/Joecstarr/grid2fp/main/test/trefoil.svg"/>
 
 
 x| |o|
 -|-|-|
  | | |
 o| |x|
 
-<img  style="background:white;width:400px;height:auto" src="https://github.com/Joecstarr/grid2fp/blob/main/test/un.svg"/>
+<img  style="width:400px;height:auto" src="https://raw.githubusercontent.com/Joecstarr/grid2fp/main/test/un.svg"/>
 
 
 ‎| |o| | |x| |
 -|-|-|-|-|-|-|
  | | | |o| |x|
  |x| | | |o| |
 o| |x| | | | |
  | | |x| | |o|
  |o| | |x| | |
 x| | |o| | | |
 
-<img  style="background:white;width:400px;height:auto" src="https://github.com/Joecstarr/grid2fp/blob/main/test/fig1_from_paper.svg"/>
+<img  style="width:400px;height:auto" src="https://raw.githubusercontent.com/Joecstarr/grid2fp/main/test/fig1_from_paper.svg"/>
+
 
 
 ## ToDo
 - [ ] CLI interface
 - [x] fit canvas to drawing better.(still not perfect)
 - [x] set string color
 - [ ] ???
```

### Comparing `grid2fp-0.0.8/README.md` & `grid2fp-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -51,54 +51,55 @@
 
 g = grid2fp(csv_file=csv_path,string_color = "pink", crossing_color="purple")
 d = g.draw()
 # make some changes to d with drawsvg
 d.save_svg(svg_path)
 
 ```
-# Sample images
+## Sample images
 
 x|o| | |
 -|-|-|-|
  |x|o| |
  | |x|o|
 o| | |x|
 
-<img  style="background:white;width:400px;height:auto" src="https://github.com/Joecstarr/grid2fp/blob/main/test/random.svg"/>
+<img  style="width:400px;height:auto" src="https://raw.githubusercontent.com/Joecstarr/grid2fp/main/test/random.svg"/>
 
 
 o| | |x| |
 -|-|-|-|-|
  | |x| |o|
  |x| |o| |
 x| |o| | |
  |o| | |x|
 
 
-<img  style="background:white;width:400px;height:auto" src="https://github.com/Joecstarr/grid2fp/blob/main/test/trefoil.svg"/>
+<img  style="width:400px;height:auto" src="https://raw.githubusercontent.com/Joecstarr/grid2fp/main/test/trefoil.svg"/>
 
 
 x| |o|
 -|-|-|
  | | |
 o| |x|
 
-<img  style="background:white;width:400px;height:auto" src="https://github.com/Joecstarr/grid2fp/blob/main/test/un.svg"/>
+<img  style="width:400px;height:auto" src="https://raw.githubusercontent.com/Joecstarr/grid2fp/main/test/un.svg"/>
 
 
 ‎| |o| | |x| |
 -|-|-|-|-|-|-|
  | | | |o| |x|
  |x| | | |o| |
 o| |x| | | | |
  | | |x| | |o|
  |o| | |x| | |
 x| | |o| | | |
 
-<img  style="background:white;width:400px;height:auto" src="https://github.com/Joecstarr/grid2fp/blob/main/test/fig1_from_paper.svg"/>
+<img  style="width:400px;height:auto" src="https://raw.githubusercontent.com/Joecstarr/grid2fp/main/test/fig1_from_paper.svg"/>
+
 
 
 ## ToDo
 - [ ] CLI interface
 - [x] fit canvas to drawing better.(still not perfect)
 - [x] set string color
 - [ ] ???
```

### Comparing `grid2fp-0.0.8/grid2fp/grid2fp.py` & `grid2fp-0.0.9/grid2fp/grid2fp.py`

 * *Files identical despite different names*

### Comparing `grid2fp-0.0.8/grid2fp.egg-info/PKG-INFO` & `grid2fp-0.0.9/grid2fp.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grid2fp
-Version: 0.0.8
+Version: 0.0.9
 Summary: A tool to eat grid diagrams and generate its front projection.
 Home-page: https://github.com/Joecstarr/grid2fp
 Author: Joe Starr
 Keywords: topology,Legendrian,Grid Diagram,knot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -67,54 +67,55 @@
 
 g = grid2fp(csv_file=csv_path,string_color = "pink", crossing_color="purple")
 d = g.draw()
 # make some changes to d with drawsvg
 d.save_svg(svg_path)
 
 ```
-# Sample images
+## Sample images
 
 x|o| | |
 -|-|-|-|
  |x|o| |
  | |x|o|
 o| | |x|
 
-<img  style="background:white;width:400px;height:auto" src="https://github.com/Joecstarr/grid2fp/blob/main/test/random.svg"/>
+<img  style="width:400px;height:auto" src="https://raw.githubusercontent.com/Joecstarr/grid2fp/main/test/random.svg"/>
 
 
 o| | |x| |
 -|-|-|-|-|
  | |x| |o|
  |x| |o| |
 x| |o| | |
  |o| | |x|
 
 
-<img  style="background:white;width:400px;height:auto" src="https://github.com/Joecstarr/grid2fp/blob/main/test/trefoil.svg"/>
+<img  style="width:400px;height:auto" src="https://raw.githubusercontent.com/Joecstarr/grid2fp/main/test/trefoil.svg"/>
 
 
 x| |o|
 -|-|-|
  | | |
 o| |x|
 
-<img  style="background:white;width:400px;height:auto" src="https://github.com/Joecstarr/grid2fp/blob/main/test/un.svg"/>
+<img  style="width:400px;height:auto" src="https://raw.githubusercontent.com/Joecstarr/grid2fp/main/test/un.svg"/>
 
 
 ‎| |o| | |x| |
 -|-|-|-|-|-|-|
  | | | |o| |x|
  |x| | | |o| |
 o| |x| | | | |
  | | |x| | |o|
  |o| | |x| | |
 x| | |o| | | |
 
-<img  style="background:white;width:400px;height:auto" src="https://github.com/Joecstarr/grid2fp/blob/main/test/fig1_from_paper.svg"/>
+<img  style="width:400px;height:auto" src="https://raw.githubusercontent.com/Joecstarr/grid2fp/main/test/fig1_from_paper.svg"/>
+
 
 
 ## ToDo
 - [ ] CLI interface
 - [x] fit canvas to drawing better.(still not perfect)
 - [x] set string color
 - [ ] ???
```

### Comparing `grid2fp-0.0.8/setup.py` & `grid2fp-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import logging
 
 logger = logging.getLogger(__name__)
 
-version = "0.0.8"
+version = "0.0.9"
 
 try:
     with open("README.md", "r") as f:
         long_desc = f.read()
 except:
     logger.warning("Could not open README.md.  long_description will be set to None.")
     long_desc = None
```

### Comparing `grid2fp-0.0.8/test/test_integration.py` & `grid2fp-0.0.9/test/test_integration.py`

 * *Files identical despite different names*

