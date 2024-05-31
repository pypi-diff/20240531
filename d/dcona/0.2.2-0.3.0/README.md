# Comparing `tmp/dcona-0.2.2.tar.gz` & `tmp/dcona-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcona-0.2.2.tar", last modified: Wed Nov 15 18:17:45 2023, max compression
+gzip compressed data, was "dcona-0.3.0.tar", last modified: Fri May 31 20:05:14 2024, max compression
```

## Comparing `dcona-0.2.2.tar` & `dcona-0.3.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 18:17:45.378758 dcona-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-11-15 18:17:39.000000 dcona-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6981 2023-11-15 18:17:45.374758 dcona-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6566 2023-11-15 18:17:39.000000 dcona-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 18:17:45.370758 dcona-0.2.2/dcona/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 18:17:45.370758 dcona-0.2.2/dcona/core/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 18:17:45.370758 dcona-0.2.2/dcona/core/correlations/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/core/correlations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/core/correlations/correlation_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    19564 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/core/correlations/correlation_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 18:17:45.374758 dcona-0.2.2/dcona/core/extern/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/core/extern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5945 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/core/extern/pcorrelations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6804 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/core/extern/ppipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/core/extern/pscores.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/core/extern/ptests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/core/extern/putils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 18:17:45.374758 dcona-0.2.2/dcona/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/core/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 18:17:45.374758 dcona-0.2.2/dcona/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/lib/dump.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/lib/hypergeom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/lib/zscore.py
--rw-r--r--   0 runner    (1001) docker     (127)     6612 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/lib/ztest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 18:17:45.370758 dcona-0.2.2/dcona/native/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 18:17:45.370758 dcona-0.2.2/dcona/native/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 18:17:45.374758 dcona-0.2.2/dcona/native/src/correlations/
--rw-r--r--   0 runner    (1001) docker     (127)     6312 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/native/src/correlations/correlations.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 18:17:45.374758 dcona-0.2.2/dcona/native/src/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/native/src/lib/correlations.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    29129 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/native/src/lib/pipelines.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/native/src/lib/scores.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/native/src/lib/tests.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/native/src/lib/utils.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 18:17:45.374758 dcona-0.2.2/dcona/native/src/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/native/src/pipelines/pipelines.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 18:17:45.374758 dcona-0.2.2/dcona/native/src/scores/
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/native/src/scores/scores.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 18:17:45.374758 dcona-0.2.2/dcona/native/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/native/src/tests/tests.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 18:17:45.374758 dcona-0.2.2/dcona/native/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2023-11-15 18:17:39.000000 dcona-0.2.2/dcona/native/src/utils/utils.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 18:17:45.370758 dcona-0.2.2/dcona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6981 2023-11-15 18:17:45.000000 dcona-0.2.2/dcona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2023-11-15 18:17:45.000000 dcona-0.2.2/dcona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 18:17:45.000000 dcona-0.2.2/dcona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-11-15 18:17:45.000000 dcona-0.2.2/dcona.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-11-15 18:17:45.000000 dcona-0.2.2/dcona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-15 18:17:45.000000 dcona-0.2.2/dcona.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-11-15 18:17:39.000000 dcona-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-15 18:17:45.378758 dcona-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2023-11-15 18:17:39.000000 dcona-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:14.624349 dcona-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-31 20:05:11.000000 dcona-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-05-31 20:05:14.624349 dcona-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-05-31 20:05:11.000000 dcona-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:14.616350 dcona-0.3.0/dcona/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:14.616350 dcona-0.3.0/dcona/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:14.616350 dcona-0.3.0/dcona/core/correlations/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/core/correlations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/core/correlations/correlation_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19564 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/core/correlations/correlation_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:14.620350 dcona-0.3.0/dcona/core/extern/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/core/extern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/core/extern/pcorrelations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/core/extern/ppipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/core/extern/pscores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/core/extern/ptests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/core/extern/putils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:14.620350 dcona-0.3.0/dcona/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/core/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:14.620350 dcona-0.3.0/dcona/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/lib/dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/lib/hypergeom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/lib/zscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/lib/ztest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:14.616350 dcona-0.3.0/dcona/native/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:14.616350 dcona-0.3.0/dcona/native/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:14.620350 dcona-0.3.0/dcona/native/src/correlations/
+-rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/native/src/correlations/correlations.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:14.620350 dcona-0.3.0/dcona/native/src/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/native/src/lib/correlations.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    29129 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/native/src/lib/pipelines.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/native/src/lib/scores.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/native/src/lib/tests.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/native/src/lib/utils.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:14.620350 dcona-0.3.0/dcona/native/src/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/native/src/pipelines/pipelines.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:14.620350 dcona-0.3.0/dcona/native/src/scores/
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/native/src/scores/scores.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:14.620350 dcona-0.3.0/dcona/native/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/native/src/tests/tests.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:14.620350 dcona-0.3.0/dcona/native/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-05-31 20:05:11.000000 dcona-0.3.0/dcona/native/src/utils/utils.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:14.620350 dcona-0.3.0/dcona.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-05-31 20:05:14.000000 dcona-0.3.0/dcona.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-31 20:05:14.000000 dcona-0.3.0/dcona.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:05:14.000000 dcona-0.3.0/dcona.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-31 20:05:14.000000 dcona-0.3.0/dcona.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-31 20:05:14.000000 dcona-0.3.0/dcona.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 20:05:14.000000 dcona-0.3.0/dcona.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-31 20:05:11.000000 dcona-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:05:14.624349 dcona-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-31 20:05:11.000000 dcona-0.3.0/setup.py
```

### Comparing `dcona-0.2.2/LICENSE` & `dcona-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/PKG-INFO` & `dcona-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcona
-Version: 0.2.2
+Version: 0.3.0
 Summary: Differential Correlation Network Analysis
 Home-page: https://github.com/zhiyanov/DCoNA
 Author: Anton Zhiyanov, Narek Engibaryan
 Author-email: zhiyanovap@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dcona-0.2.2/README.md` & `dcona-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/dcona/__main__.py` & `dcona-0.3.0/dcona/__main__.py`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/dcona/core/correlations/correlation_tests.py` & `dcona-0.3.0/dcona/core/correlations/correlation_tests.py`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/dcona/core/correlations/correlation_utils.py` & `dcona-0.3.0/dcona/core/correlations/correlation_utils.py`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/dcona/core/extern/pcorrelations.py` & `dcona-0.3.0/dcona/core/extern/pcorrelations.py`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/dcona/core/extern/ppipelines.py` & `dcona-0.3.0/dcona/core/extern/ppipelines.py`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/dcona/core/extern/pscores.py` & `dcona-0.3.0/dcona/core/extern/pscores.py`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/dcona/core/extern/ptests.py` & `dcona-0.3.0/dcona/core/extern/ptests.py`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/dcona/core/extern/putils.py` & `dcona-0.3.0/dcona/core/extern/putils.py`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/dcona/core/utils/utils.py` & `dcona-0.3.0/dcona/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/dcona/lib/dump.py` & `dcona-0.3.0/dcona/lib/dump.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import tqdm
 import sys
 import os
+import numpy as np
 
 from ..core import extern as cextern
 
 CHUNK_LENGTH = 10**5
 
 
 def check_directory_existence(
@@ -37,14 +38,16 @@
         if i >= chunk_number - 1:
             end = len(indexes)
         
         dump_indexes = indexes[start : end]
         
         if (isinstance(df_indexes, tuple)) and (len(df_indexes) == 2):
             source_indexes, target_indexes = df_indexes
+            source_indexes = np.array(source_indexes)[dump_indexes]
+            target_indexes = np.array(target_indexes)[dump_indexes]
         else:
             source_indexes = []
             target_indexes = []
             for ind in dump_indexes:
                 if not (index_transform is None):
                     ind = index_transform[ind]
```

### Comparing `dcona-0.2.2/dcona/lib/hypergeom.py` & `dcona-0.3.0/dcona/lib/hypergeom.py`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/dcona/lib/utils.py` & `dcona-0.3.0/dcona/lib/utils.py`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/dcona/lib/zscore.py` & `dcona-0.3.0/dcona/lib/zscore.py`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/dcona/lib/ztest.py` & `dcona-0.3.0/dcona/lib/ztest.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         if repeats_number is None:
             repeats_number = int(len(interaction_df) / 0.05)
     else:
         interaction_df = None
 
         if repeats_number is None:
             repeats_number = 0
-    
+
     sorted_indexes, df_indexes, \
     ref_corrs, ref_pvalues, exp_corrs, exp_pvalues, \
     stat, pvalue, adjusted_pvalue, \
     boot_pvalue = _ztest(
         data_df, description_df, interaction_df, \
         reference_group, experimental_group, \
         correlation, alternative, \
@@ -74,53 +74,55 @@
 
             df_columns = [
                 ref_corrs, ref_pvalues,
                 exp_corrs, exp_pvalues, stat,
                 pvalue, adjusted_pvalue
             ]
 
-
         path_to_file = output_dir.rstrip("/") + f"/{correlation}_{alternative}_ztest.csv"
         dump.save_by_chunks(
             sorted_indexes,
             df_indexes, df_template, df_columns,
             path_to_file
         )
         
         print(f"File saved at: {path_to_file}")
         return None
     
-    source_indexes = []
-    target_indexes = []
-
     if (isinstance(df_indexes, tuple)) and (len(df_indexes) == 2):
+        # This "if" is true when user passed interaction_df
         source_indexes, target_indexes = df_indexes
+        source_indexes = np.array(source_indexes)[sorted_indexes]
+        target_indexes = np.array(target_indexes)[sorted_indexes]
     else:
+        # This "else" is true when user passed no interaction_df
+        source_indexes = []
+        target_indexes = []
         for ind in sorted_indexes:
             s, t = extern.paired_index(ind, len(df_indexes))
             source_indexes.append(df_indexes[s])
             target_indexes.append(df_indexes[t])
-    
+
     if repeats_number > 0:
         output_df = pd.DataFrame(data={
-            "Source": source_indexes.to_numpy()[sorted_indexes],
-            "Target": target_indexes.to_numpy()[sorted_indexes],
+            "Source": source_indexes,
+            "Target": target_indexes,
             "RefCorr": ref_corrs[sorted_indexes], 
             "RefPvalue": ref_pvalues[sorted_indexes], 
             "ExpCorr": exp_corrs[sorted_indexes], 
             "ExpPvalue": exp_pvalues[sorted_indexes], 
             "Statistic": stat[sorted_indexes],
             "Pvalue": pvalue[sorted_indexes], 
             "AdjPvalue": adjusted_pvalue[sorted_indexes],
             "PermutePvalue": boot_pvalue[sorted_indexes] 
         })
     else:
         output_df = pd.DataFrame(data={
-            "Source": source_indexes.to_numpy()[sorted_indexes],
-            "Target": target_indexes.to_numpy()[sorted_indexes],
+            "Source": source_indexes,
+            "Target": target_indexes,
             "RefCorr": ref_corrs[sorted_indexes], 
             "RefPvalue": ref_pvalues[sorted_indexes], 
             "ExpCorr": exp_corrs[sorted_indexes], 
             "ExpPvalue": exp_pvalues[sorted_indexes], 
             "Statistic": stat[sorted_indexes],
             "Pvalue": pvalue[sorted_indexes], 
             "AdjPvalue": adjusted_pvalue[sorted_indexes]
```

### Comparing `dcona-0.2.2/dcona/native/src/correlations/correlations.cpp` & `dcona-0.3.0/dcona/native/src/correlations/correlations.cpp`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/dcona/native/src/lib/correlations.cpp` & `dcona-0.3.0/dcona/native/src/lib/correlations.cpp`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/dcona/native/src/lib/pipelines.cpp` & `dcona-0.3.0/dcona/native/src/lib/pipelines.cpp`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/dcona/native/src/lib/scores.cpp` & `dcona-0.3.0/dcona/native/src/lib/scores.cpp`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/dcona/native/src/lib/tests.cpp` & `dcona-0.3.0/dcona/native/src/lib/tests.cpp`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/dcona/native/src/lib/utils.cpp` & `dcona-0.3.0/dcona/native/src/lib/utils.cpp`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/dcona/native/src/pipelines/pipelines.cpp` & `dcona-0.3.0/dcona/native/src/pipelines/pipelines.cpp`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/dcona/native/src/scores/scores.cpp` & `dcona-0.3.0/dcona/native/src/scores/scores.cpp`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/dcona/native/src/tests/tests.cpp` & `dcona-0.3.0/dcona/native/src/tests/tests.cpp`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/dcona/native/src/utils/utils.cpp` & `dcona-0.3.0/dcona/native/src/utils/utils.cpp`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/dcona.egg-info/PKG-INFO` & `dcona-0.3.0/dcona.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcona
-Version: 0.2.2
+Version: 0.3.0
 Summary: Differential Correlation Network Analysis
 Home-page: https://github.com/zhiyanov/DCoNA
 Author: Anton Zhiyanov, Narek Engibaryan
 Author-email: zhiyanovap@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dcona-0.2.2/dcona.egg-info/SOURCES.txt` & `dcona-0.3.0/dcona.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcona-0.2.2/setup.py` & `dcona-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import setup, Extension, find_packages
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = ['pybind11', 'pandas', 'numpy', 'scipy', 'tqdm']
 
-__version__ = "0.2.2"
+__version__ = "0.3.0"
 
 
 ext_modules = [
     Extension("dcona.core.extern.utils",
         ["dcona/native/src/utils/utils.cpp",
          "dcona/native/src/lib/utils.cpp"],
          include_dirs=[pybind11.get_include()],
```

