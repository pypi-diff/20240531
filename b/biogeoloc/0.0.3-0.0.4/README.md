# Comparing `tmp/biogeoloc-0.0.3.tar.gz` & `tmp/biogeoloc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biogeoloc-0.0.3.tar", last modified: Sat May 25 21:59:58 2024, max compression
+gzip compressed data, was "biogeoloc-0.0.4.tar", last modified: Fri May 31 20:27:41 2024, max compression
```

## Comparing `biogeoloc-0.0.3.tar` & `biogeoloc-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-25 21:59:58.000000 biogeoloc-0.0.3/
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     1066 2024-05-09 23:42:35.000000 biogeoloc-0.0.3/LICENSE
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     2914 2024-05-25 21:59:58.000000 biogeoloc-0.0.3/PKG-INFO
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     2476 2024-05-11 19:39:17.000000 biogeoloc-0.0.3/README.md
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-25 21:59:58.000000 biogeoloc-0.0.3/biogeoloc/
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)      108 2024-05-23 19:38:34.000000 biogeoloc-0.0.3/biogeoloc/__init__.py
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)    30009 2024-05-25 20:09:02.000000 biogeoloc-0.0.3/biogeoloc/cls.py
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)    12965 2024-05-25 18:14:38.000000 biogeoloc-0.0.3/biogeoloc/genesys.py
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)      536 2024-05-25 18:16:26.000000 biogeoloc-0.0.3/biogeoloc/versions.py
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-25 21:59:58.000000 biogeoloc-0.0.3/biogeoloc.egg-info/
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     2914 2024-05-25 21:59:58.000000 biogeoloc-0.0.3/biogeoloc.egg-info/PKG-INFO
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      272 2024-05-25 21:59:58.000000 biogeoloc-0.0.3/biogeoloc.egg-info/SOURCES.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        1 2024-05-25 21:59:58.000000 biogeoloc-0.0.3/biogeoloc.egg-info/dependency_links.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       49 2024-05-25 21:59:58.000000 biogeoloc-0.0.3/biogeoloc.egg-info/requires.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       10 2024-05-25 21:59:58.000000 biogeoloc-0.0.3/biogeoloc.egg-info/top_level.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       38 2024-05-25 21:59:58.000000 biogeoloc-0.0.3/setup.cfg
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)      837 2024-05-11 03:29:08.000000 biogeoloc-0.0.3/setup.py
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-31 20:27:41.000000 biogeoloc-0.0.4/
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     1066 2024-05-09 23:42:35.000000 biogeoloc-0.0.4/LICENSE
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     2937 2024-05-31 20:27:41.000000 biogeoloc-0.0.4/PKG-INFO
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     2476 2024-05-11 19:39:17.000000 biogeoloc-0.0.4/README.md
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-31 20:27:41.000000 biogeoloc-0.0.4/biogeoloc/
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)      108 2024-05-23 19:38:34.000000 biogeoloc-0.0.4/biogeoloc/__init__.py
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)    30009 2024-05-25 20:09:02.000000 biogeoloc-0.0.4/biogeoloc/cls.py
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)    12906 2024-05-31 20:18:58.000000 biogeoloc-0.0.4/biogeoloc/genesys.py
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)      657 2024-05-31 20:19:33.000000 biogeoloc-0.0.4/biogeoloc/versions.py
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-31 20:27:41.000000 biogeoloc-0.0.4/biogeoloc.egg-info/
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     2937 2024-05-31 20:27:41.000000 biogeoloc-0.0.4/biogeoloc.egg-info/PKG-INFO
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      272 2024-05-31 20:27:41.000000 biogeoloc-0.0.4/biogeoloc.egg-info/SOURCES.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        1 2024-05-31 20:27:41.000000 biogeoloc-0.0.4/biogeoloc.egg-info/dependency_links.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       33 2024-05-31 20:27:41.000000 biogeoloc-0.0.4/biogeoloc.egg-info/requires.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       10 2024-05-31 20:27:41.000000 biogeoloc-0.0.4/biogeoloc.egg-info/top_level.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       38 2024-05-31 20:27:41.000000 biogeoloc-0.0.4/setup.cfg
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)      853 2024-05-31 20:22:48.000000 biogeoloc-0.0.4/setup.py
```

### Comparing `biogeoloc-0.0.3/LICENSE` & `biogeoloc-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `biogeoloc-0.0.3/PKG-INFO` & `biogeoloc-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: biogeoloc
-Version: 0.0.3
-Summary: A python package for plotting correlations between variants and environmental factors.
-Home-page: https://github.com/SouthernCD/GeoGenoPlot
+Version: 0.0.4
+Summary: A python object package for storing and managing geographic information about biological samples.
+Home-page: https://github.com/SouthernCD/biogeoloc
 Author: Yuxing Xu
 Author-email: xuyuxing@mail.kib.ac.cn
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: toolbiox>=0.0.46
-Requires-Dist: plotbiox>=0.0.2
-Requires-Dist: cyvcf2>=0.30.28
+Requires-Dist: yxmath
+Requires-Dist: yxmap
+Requires-Dist: yxutil
+Requires-Dist: pandas
+Requires-Dist: numpy
 
 # biogeoloc
 A python object package for storing and managing geographic information about biological samples
 
 ## Installation
 ```
 pip install biogeoloc
```

### Comparing `biogeoloc-0.0.3/README.md` & `biogeoloc-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `biogeoloc-0.0.3/biogeoloc/cls.py` & `biogeoloc-0.0.4/biogeoloc/cls.py`

 * *Files identical despite different names*

### Comparing `biogeoloc-0.0.3/biogeoloc/genesys.py` & `biogeoloc-0.0.4/biogeoloc/genesys.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
 import numpy as np
 import re
-from toolbiox.lib.common.math.set import merge_same_element_set
-from toolbiox.lib.xuyuxing.map.base import haversine
-from toolbiox.lib.common.os import cmd_run
+from yxmath.set import merge_same_element_set
+from yxmap import haversine
+from yxutil import cmd_run
 from biogeoloc.cls import Accession, AccessionSet
 import time
 
 
 class GeneSysAccSet(AccessionSet):
     def __init__(self, name=None, date=None):
         date = date if date else time.strftime(
```

### Comparing `biogeoloc-0.0.3/biogeoloc/versions.py` & `biogeoloc-0.0.4/biogeoloc/versions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 def get_versions():
     return versions[0]["number"]
 
 versions = [
     {
+        "number": "0.0.4",
+        "features": [
+            "1. move from toolbiox to yxtools",
+        ],
+    },
+    {
         "number": "0.0.3",
         "features": [
             "1. There seems to be a lot of errors in GeneSys with the label of whether Accession is Landraces or not, removed that part of the information from genesys.py.",
         ],
     },
     {
         "number": "0.0.2",
```

### Comparing `biogeoloc-0.0.3/biogeoloc.egg-info/PKG-INFO` & `biogeoloc-0.0.4/biogeoloc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: biogeoloc
-Version: 0.0.3
-Summary: A python package for plotting correlations between variants and environmental factors.
-Home-page: https://github.com/SouthernCD/GeoGenoPlot
+Version: 0.0.4
+Summary: A python object package for storing and managing geographic information about biological samples.
+Home-page: https://github.com/SouthernCD/biogeoloc
 Author: Yuxing Xu
 Author-email: xuyuxing@mail.kib.ac.cn
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: toolbiox>=0.0.46
-Requires-Dist: plotbiox>=0.0.2
-Requires-Dist: cyvcf2>=0.30.28
+Requires-Dist: yxmath
+Requires-Dist: yxmap
+Requires-Dist: yxutil
+Requires-Dist: pandas
+Requires-Dist: numpy
 
 # biogeoloc
 A python object package for storing and managing geographic information about biological samples
 
 ## Installation
 ```
 pip install biogeoloc
```

### Comparing `biogeoloc-0.0.3/setup.py` & `biogeoloc-0.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,27 +6,29 @@
     LONG_DESCRIPTION = f.read()
 
 setuptools.setup(
     name="biogeoloc",
     version=get_versions(),
     author="Yuxing Xu",
     author_email="xuyuxing@mail.kib.ac.cn",
-    description="A python package for plotting correlations between variants and environmental factors.",
+    description="A python object package for storing and managing geographic information about biological samples.",
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
-    url="https://github.com/SouthernCD/GeoGenoPlot",
+    url="https://github.com/SouthernCD/biogeoloc",
     include_package_data = True,
 
     # entry_points={
     #     "console_scripts": ["HugeP2G = hugep2g.cli:main"]
     # },    
 
     packages=setuptools.find_packages(),
 
     install_requires=[
-        "toolbiox>=0.0.46",
-        "plotbiox>=0.0.2",
-        "cyvcf2>=0.30.28"
+        "yxmath",
+        "yxmap",
+        "yxutil",
+        "pandas",
+        "numpy",
     ],
 
     python_requires='>=3.5',
 )
```

