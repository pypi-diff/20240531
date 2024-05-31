# Comparing `tmp/napari_moltrack-0.0.2.tar.gz` & `tmp/napari_moltrack-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_moltrack-0.0.2.tar", last modified: Thu May 30 17:31:07 2024, max compression
+gzip compressed data, was "napari_moltrack-0.0.3.tar", last modified: Thu May 30 17:38:09 2024, max compression
```

## Comparing `napari_moltrack-0.0.2.tar` & `napari_moltrack-0.0.3.tar`

### file list

```diff
@@ -1,36 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 17:31:07.231171 napari_moltrack-0.0.2/
--rw-rw-rw-   0        0        0     1515 2024-05-29 16:12:09.000000 napari_moltrack-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      101 2024-05-29 16:12:09.000000 napari_moltrack-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6468 2024-05-30 17:31:07.231171 napari_moltrack-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2705 2024-05-29 16:12:09.000000 napari_moltrack-0.0.2/README.md
--rw-rw-rw-   0        0        0     3406 2024-05-30 17:30:23.000000 napari_moltrack-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-30 17:31:07.231171 napari_moltrack-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-30 17:31:07.162120 napari_moltrack-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-30 17:31:07.177741 napari_moltrack-0.0.2/src/moltrack/
-drwxrwxrwx   0        0        0        0 2024-05-30 17:31:07.193362 napari_moltrack-0.0.2/src/moltrack/GUI/
--rw-rw-rw-   0        0        0        0 2024-05-29 16:42:16.000000 napari_moltrack-0.0.2/src/moltrack/GUI/__init__.py
--rw-rw-rw-   0        0        0    61681 2024-05-30 13:51:32.000000 napari_moltrack-0.0.2/src/moltrack/GUI/widget_ui.py
--rw-rw-rw-   0        0        0       98 2024-05-30 17:30:58.000000 napari_moltrack-0.0.2/src/moltrack/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 17:31:07.199895 napari_moltrack-0.0.2/src/moltrack/_tests/
--rw-rw-rw-   0        0        0        0 2024-05-29 16:12:09.000000 napari_moltrack-0.0.2/src/moltrack/_tests/__init__.py
--rw-rw-rw-   0        0        0     2172 2024-05-29 16:15:26.000000 napari_moltrack-0.0.2/src/moltrack/_tests/test_widget.py
--rw-rw-rw-   0        0        0     6552 2024-05-30 16:54:29.000000 napari_moltrack-0.0.2/src/moltrack/_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-30 17:31:07.215547 napari_moltrack-0.0.2/src/moltrack/funcs/
--rw-rw-rw-   0        0        0        0 2024-05-30 07:19:51.000000 napari_moltrack-0.0.2/src/moltrack/funcs/__init__.py
--rw-rw-rw-   0        0        0     8053 2024-05-30 10:37:04.000000 napari_moltrack-0.0.2/src/moltrack/funcs/compute_utils.py
--rw-rw-rw-   0        0        0    13311 2024-05-30 12:41:31.000000 napari_moltrack-0.0.2/src/moltrack/funcs/events_utils.py
--rw-rw-rw-   0        0        0     8893 2024-05-30 11:25:33.000000 napari_moltrack-0.0.2/src/moltrack/funcs/export_utils.py
--rw-rw-rw-   0        0        0    13425 2024-05-30 17:25:19.000000 napari_moltrack-0.0.2/src/moltrack/funcs/import_utils.py
--rw-rw-rw-   0        0        0     5422 2024-05-30 10:39:02.000000 napari_moltrack-0.0.2/src/moltrack/funcs/loc_filter_utils.py
--rw-rw-rw-   0        0        0    34039 2024-05-30 16:52:33.000000 napari_moltrack-0.0.2/src/moltrack/funcs/picasso_detect_utils.py
--rw-rw-rw-   0        0        0     3282 2024-05-30 10:49:15.000000 napari_moltrack-0.0.2/src/moltrack/funcs/picasso_render_utils.py
--rw-rw-rw-   0        0        0    18504 2024-05-30 09:31:37.000000 napari_moltrack-0.0.2/src/moltrack/funcs/segmentation_utils.py
--rw-rw-rw-   0        0        0     4161 2024-05-30 10:54:17.000000 napari_moltrack-0.0.2/src/moltrack/funcs/tracking_utils.py
--rw-rw-rw-   0        0        0      495 2024-05-29 16:15:26.000000 napari_moltrack-0.0.2/src/moltrack/napari.yaml
-drwxrwxrwx   0        0        0        0 2024-05-30 17:31:07.231171 napari_moltrack-0.0.2/src/napari_moltrack.egg-info/
--rw-rw-rw-   0        0        0     6468 2024-05-30 17:31:07.000000 napari_moltrack-0.0.2/src/napari_moltrack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      879 2024-05-30 17:31:07.000000 napari_moltrack-0.0.2/src/napari_moltrack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 17:31:07.000000 napari_moltrack-0.0.2/src/napari_moltrack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-05-30 17:31:07.000000 napari_moltrack-0.0.2/src/napari_moltrack.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      234 2024-05-30 17:31:07.000000 napari_moltrack-0.0.2/src/napari_moltrack.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-30 17:31:07.000000 napari_moltrack-0.0.2/src/napari_moltrack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 17:38:09.599934 napari_moltrack-0.0.3/
+-rw-rw-rw-   0        0        0     1515 2024-05-29 16:12:09.000000 napari_moltrack-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-05-29 16:12:09.000000 napari_moltrack-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6468 2024-05-30 17:38:09.599934 napari_moltrack-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2705 2024-05-29 16:12:09.000000 napari_moltrack-0.0.3/README.md
+-rw-rw-rw-   0        0        0     3406 2024-05-30 17:30:23.000000 napari_moltrack-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 17:38:09.599934 napari_moltrack-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-30 17:38:09.530942 napari_moltrack-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 17:38:09.546564 napari_moltrack-0.0.3/src/moltrack/
+drwxrwxrwx   0        0        0        0 2024-05-30 17:38:09.546564 napari_moltrack-0.0.3/src/moltrack/GUI/
+-rw-rw-rw-   0        0        0        0 2024-05-29 16:42:16.000000 napari_moltrack-0.0.3/src/moltrack/GUI/__init__.py
+-rw-rw-rw-   0        0        0    61681 2024-05-30 13:51:32.000000 napari_moltrack-0.0.3/src/moltrack/GUI/widget_ui.py
+-rw-rw-rw-   0        0        0       98 2024-05-30 17:37:59.000000 napari_moltrack-0.0.3/src/moltrack/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:38:09.562213 napari_moltrack-0.0.3/src/moltrack/_tests/
+-rw-rw-rw-   0        0        0        0 2024-05-29 16:12:09.000000 napari_moltrack-0.0.3/src/moltrack/_tests/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-05-29 16:15:26.000000 napari_moltrack-0.0.3/src/moltrack/_tests/test_widget.py
+-rw-rw-rw-   0        0        0     6368 2024-05-30 17:35:51.000000 napari_moltrack-0.0.3/src/moltrack/_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:38:09.577834 napari_moltrack-0.0.3/src/moltrack/funcs/
+-rw-rw-rw-   0        0        0        0 2024-05-30 07:19:51.000000 napari_moltrack-0.0.3/src/moltrack/funcs/__init__.py
+-rw-rw-rw-   0        0        0     8053 2024-05-30 10:37:04.000000 napari_moltrack-0.0.3/src/moltrack/funcs/compute_utils.py
+-rw-rw-rw-   0        0        0    13311 2024-05-30 12:41:31.000000 napari_moltrack-0.0.3/src/moltrack/funcs/events_utils.py
+-rw-rw-rw-   0        0        0     8893 2024-05-30 11:25:33.000000 napari_moltrack-0.0.3/src/moltrack/funcs/export_utils.py
+-rw-rw-rw-   0        0        0    13425 2024-05-30 17:25:19.000000 napari_moltrack-0.0.3/src/moltrack/funcs/import_utils.py
+-rw-rw-rw-   0        0        0     5422 2024-05-30 10:39:02.000000 napari_moltrack-0.0.3/src/moltrack/funcs/loc_filter_utils.py
+-rw-rw-rw-   0        0        0    33767 2024-05-30 17:35:51.000000 napari_moltrack-0.0.3/src/moltrack/funcs/picasso_detect_utils.py
+-rw-rw-rw-   0        0        0     3282 2024-05-30 10:49:15.000000 napari_moltrack-0.0.3/src/moltrack/funcs/picasso_render_utils.py
+-rw-rw-rw-   0        0        0    18504 2024-05-30 09:31:37.000000 napari_moltrack-0.0.3/src/moltrack/funcs/segmentation_utils.py
+-rw-rw-rw-   0        0        0     4161 2024-05-30 10:54:17.000000 napari_moltrack-0.0.3/src/moltrack/funcs/tracking_utils.py
+-rw-rw-rw-   0        0        0      495 2024-05-29 16:15:26.000000 napari_moltrack-0.0.3/src/moltrack/napari.yaml
+drwxrwxrwx   0        0        0        0 2024-05-30 17:38:09.599934 napari_moltrack-0.0.3/src/napari_moltrack.egg-info/
+-rw-rw-rw-   0        0        0     6468 2024-05-30 17:38:09.000000 napari_moltrack-0.0.3/src/napari_moltrack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      975 2024-05-30 17:38:09.000000 napari_moltrack-0.0.3/src/napari_moltrack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 17:38:09.000000 napari_moltrack-0.0.3/src/napari_moltrack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-30 17:38:09.000000 napari_moltrack-0.0.3/src/napari_moltrack.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      234 2024-05-30 17:38:09.000000 napari_moltrack-0.0.3/src/napari_moltrack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-30 17:38:09.000000 napari_moltrack-0.0.3/src/napari_moltrack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 17:38:09.599934 napari_moltrack-0.0.3/src/pygpufit/
+-rw-rw-rw-   0        0        0  1982976 2024-05-21 11:03:35.000000 napari_moltrack-0.0.3/src/pygpufit/Gpufit.dll
+-rw-rw-rw-   0        0        0        0 2024-05-21 11:03:35.000000 napari_moltrack-0.0.3/src/pygpufit/__init__.py
+-rw-rw-rw-   0        0        0    14512 2024-05-21 11:03:35.000000 napari_moltrack-0.0.3/src/pygpufit/gpufit.py
+-rw-rw-rw-   0        0        0      140 2024-05-21 11:03:35.000000 napari_moltrack-0.0.3/src/pygpufit/version.py
```

### Comparing `napari_moltrack-0.0.2/LICENSE` & `napari_moltrack-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.2/PKG-INFO` & `napari_moltrack-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-moltrack
-Version: 0.0.2
+Version: 0.0.3
 Summary: Single molecule tracking package for Napari
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: 
         Copyright (c) 2024, Piers Turner
         All rights reserved.
```

### Comparing `napari_moltrack-0.0.2/README.md` & `napari_moltrack-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.2/pyproject.toml` & `napari_moltrack-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.2/src/moltrack/GUI/widget_ui.py` & `napari_moltrack-0.0.3/src/moltrack/GUI/widget_ui.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.2/src/moltrack/_tests/test_widget.py` & `napari_moltrack-0.0.3/src/moltrack/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.2/src/moltrack/_widget.py` & `napari_moltrack-0.0.3/src/moltrack/_widget.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 from typing import TYPE_CHECKING
 
-from magicgui import magic_factory
-from magicgui.widgets import CheckBox, Container, create_widget
-from qtpy.QtWidgets import QHBoxLayout, QPushButton, QWidget
-from skimage.util import img_as_float
-import traceback
+from qtpy.QtWidgets import QWidget
 from multiprocessing import Manager
 from functools import partial
 from qtpy.QtCore import QThreadPool
 from qtpy.QtWidgets import QVBoxLayout
 import pyqtgraph as pg
 
 if TYPE_CHECKING:
```

### Comparing `napari_moltrack-0.0.2/src/moltrack/funcs/compute_utils.py` & `napari_moltrack-0.0.3/src/moltrack/funcs/compute_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.2/src/moltrack/funcs/events_utils.py` & `napari_moltrack-0.0.3/src/moltrack/funcs/events_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.2/src/moltrack/funcs/export_utils.py` & `napari_moltrack-0.0.3/src/moltrack/funcs/export_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.2/src/moltrack/funcs/import_utils.py` & `napari_moltrack-0.0.3/src/moltrack/funcs/import_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.2/src/moltrack/funcs/loc_filter_utils.py` & `napari_moltrack-0.0.3/src/moltrack/funcs/loc_filter_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.2/src/moltrack/funcs/picasso_detect_utils.py` & `napari_moltrack-0.0.3/src/moltrack/funcs/picasso_detect_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,27 @@
-import numpy as np
 import traceback
 
-import pandas as pd
-
 from moltrack.funcs.compute_utils import Worker
 import time
 import os
 from multiprocessing import shared_memory
-from picasso import localize
 from picasso.localize import get_spots, identify_frame
-from picasso.gaussmle import gaussmle
 from picasso import gausslq
 from picasso import postprocess
 from functools import partial
 import concurrent.futures
 import multiprocessing
-from picasso.render import render
-from shapely.geometry import Point, Polygon
-from multiprocessing import Manager, Event
-import numba
-from numba import jit, types,typed
-from numba.typed import Dict
+from shapely.geometry import Point
+from multiprocessing import Manager
 import numpy as np
 import pandas as pd
 import math
 import cv2
 from skimage.feature import peak_local_max
-from numba import jit, prange
+
 
 def precompute_kernels(lnoise=0, lobject=1):
 
     if lnoise == 0:
         gaussian_kernel = 1
     else:
         gaussian_kernel = cv2.getGaussianKernel(2 * math.ceil(5 * lnoise) + 1, math.sqrt(2) * lnoise)
```

### Comparing `napari_moltrack-0.0.2/src/moltrack/funcs/picasso_render_utils.py` & `napari_moltrack-0.0.3/src/moltrack/funcs/picasso_render_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.2/src/moltrack/funcs/segmentation_utils.py` & `napari_moltrack-0.0.3/src/moltrack/funcs/segmentation_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.2/src/moltrack/funcs/tracking_utils.py` & `napari_moltrack-0.0.3/src/moltrack/funcs/tracking_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.2/src/napari_moltrack.egg-info/PKG-INFO` & `napari_moltrack-0.0.3/src/napari_moltrack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-moltrack
-Version: 0.0.2
+Version: 0.0.3
 Summary: Single molecule tracking package for Napari
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: 
         Copyright (c) 2024, Piers Turner
         All rights reserved.
```

### Comparing `napari_moltrack-0.0.2/src/napari_moltrack.egg-info/SOURCES.txt` & `napari_moltrack-0.0.3/src/napari_moltrack.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -20,8 +20,12 @@
 src/moltrack/funcs/segmentation_utils.py
 src/moltrack/funcs/tracking_utils.py
 src/napari_moltrack.egg-info/PKG-INFO
 src/napari_moltrack.egg-info/SOURCES.txt
 src/napari_moltrack.egg-info/dependency_links.txt
 src/napari_moltrack.egg-info/entry_points.txt
 src/napari_moltrack.egg-info/requires.txt
-src/napari_moltrack.egg-info/top_level.txt
+src/napari_moltrack.egg-info/top_level.txt
+src/pygpufit/Gpufit.dll
+src/pygpufit/__init__.py
+src/pygpufit/gpufit.py
+src/pygpufit/version.py
```

