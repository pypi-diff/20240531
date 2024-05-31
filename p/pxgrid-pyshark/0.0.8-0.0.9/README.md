# Comparing `tmp/pxgrid_pyshark-0.0.8.tar.gz` & `tmp/pxgrid_pyshark-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pxgrid_pyshark-0.0.8.tar", last modified: Wed Mar 13 19:20:45 2024, max compression
+gzip compressed data, was "pxgrid_pyshark-0.0.9.tar", last modified: Fri May 31 21:45:02 2024, max compression
```

## Comparing `pxgrid_pyshark-0.0.8.tar` & `pxgrid_pyshark-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 aacook     (501) staff       (20)        0 2024-03-13 19:20:45.804512 pxgrid_pyshark-0.0.8/
--rw-r--r--   0 aacook     (501) staff       (20)    11356 2024-01-21 14:34:20.000000 pxgrid_pyshark-0.0.8/LICENSE
--rw-r--r--   0 aacook     (501) staff       (20)       84 2024-01-24 01:20:48.000000 pxgrid_pyshark-0.0.8/MANIFEST.in
--rw-r--r--   0 aacook     (501) staff       (20)      157 2024-01-21 14:34:20.000000 pxgrid_pyshark-0.0.8/NOTICE
--rw-r--r--   0 aacook     (501) staff       (20)     1215 2024-03-13 19:20:45.804373 pxgrid_pyshark-0.0.8/PKG-INFO
--rw-r--r--   0 aacook     (501) staff       (20)     9557 2024-03-05 15:01:18.000000 pxgrid_pyshark-0.0.8/README.md
-drwxr-xr-x   0 aacook     (501) staff       (20)        0 2024-03-13 19:20:45.738916 pxgrid_pyshark-0.0.8/bin/
--rw-r--r--   0 aacook     (501) staff       (20)    15930 2024-03-13 19:18:51.000000 pxgrid_pyshark-0.0.8/bin/pxgrid-pyshark
--rw-r--r--   0 aacook     (501) staff       (20)     4928 2024-03-12 19:44:51.000000 pxgrid_pyshark-0.0.8/bin/pxgrid-pyshark-file
--rw-r--r--   0 aacook     (501) staff       (20)      504 2024-03-05 13:44:52.000000 pxgrid_pyshark-0.0.8/bin/pxgrid-pyshark-view
-drwxr-xr-x   0 aacook     (501) staff       (20)        0 2024-03-13 19:20:45.740913 pxgrid_pyshark-0.0.8/pxgrid_pyshark/
--rw-r--r--   0 aacook     (501) staff       (20)      288 2024-01-21 15:03:33.000000 pxgrid_pyshark-0.0.8/pxgrid_pyshark/__init__.py
--rw-r--r--   0 aacook     (501) staff       (20)      497 2024-03-13 19:20:45.805031 pxgrid_pyshark-0.0.8/pxgrid_pyshark/_version.py
--rw-r--r--   0 aacook     (501) staff       (20)     3517 2024-01-28 15:21:12.000000 pxgrid_pyshark-0.0.8/pxgrid_pyshark/capture.py
-drwxr-xr-x   0 aacook     (501) staff       (20)        0 2024-03-13 19:20:45.797376 pxgrid_pyshark-0.0.8/pxgrid_pyshark/db/
--rw-r--r--   0 aacook     (501) staff       (20)    24720 2024-03-13 12:51:46.000000 pxgrid_pyshark-0.0.8/pxgrid_pyshark/db/androids.json
--rw-r--r--   0 aacook     (501) staff       (20)      661 2024-03-03 14:54:23.000000 pxgrid_pyshark-0.0.8/pxgrid_pyshark/db/apple-os.json
--rw-r--r--   0 aacook     (501) staff       (20)  2899968 2024-02-26 14:35:41.000000 pxgrid_pyshark-0.0.8/pxgrid_pyshark/db/macoui.db
--rw-r--r--   0 aacook     (501) staff       (20)  1067347 2024-02-26 14:35:41.000000 pxgrid_pyshark-0.0.8/pxgrid_pyshark/db/macoui.pipe
--rw-r--r--   0 aacook     (501) staff       (20)  5707876 2024-02-26 14:35:41.000000 pxgrid_pyshark-0.0.8/pxgrid_pyshark/db/macoui.txt
--rw-r--r--   0 aacook     (501) staff       (20)    50581 2024-03-13 02:21:22.000000 pxgrid_pyshark-0.0.8/pxgrid_pyshark/db/models.json
--rw-r--r--   0 aacook     (501) staff       (20)     8504 2024-03-05 14:02:45.000000 pxgrid_pyshark-0.0.8/pxgrid_pyshark/endpointsdb.py
--rw-r--r--   0 aacook     (501) staff       (20)     3154 2024-03-05 13:48:44.000000 pxgrid_pyshark-0.0.8/pxgrid_pyshark/ouidb.py
--rw-r--r--   0 aacook     (501) staff       (20)    33881 2024-03-13 13:12:11.000000 pxgrid_pyshark-0.0.8/pxgrid_pyshark/parser.py
-drwxr-xr-x   0 aacook     (501) staff       (20)        0 2024-03-13 19:20:45.803748 pxgrid_pyshark-0.0.8/pxgrid_pyshark.egg-info/
--rw-r--r--   0 aacook     (501) staff       (20)     1215 2024-03-13 19:20:45.000000 pxgrid_pyshark-0.0.8/pxgrid_pyshark.egg-info/PKG-INFO
--rw-r--r--   0 aacook     (501) staff       (20)      665 2024-03-13 19:20:45.000000 pxgrid_pyshark-0.0.8/pxgrid_pyshark.egg-info/SOURCES.txt
--rw-r--r--   0 aacook     (501) staff       (20)        1 2024-03-13 19:20:45.000000 pxgrid_pyshark-0.0.8/pxgrid_pyshark.egg-info/dependency_links.txt
--rw-r--r--   0 aacook     (501) staff       (20)      117 2024-03-13 19:20:45.000000 pxgrid_pyshark-0.0.8/pxgrid_pyshark.egg-info/requires.txt
--rwx------   0 aacook     (501) staff       (20)       15 2024-03-13 19:20:45.000000 pxgrid_pyshark-0.0.8/pxgrid_pyshark.egg-info/top_level.txt
--rw-r--r--   0 aacook     (501) staff       (20)      210 2024-03-13 19:20:45.804859 pxgrid_pyshark-0.0.8/setup.cfg
--rw-r--r--   0 aacook     (501) staff       (20)     2188 2024-03-05 13:51:29.000000 pxgrid_pyshark-0.0.8/setup.py
--rw-r--r--   0 aacook     (501) staff       (20)    86677 2024-01-24 01:32:49.000000 pxgrid_pyshark-0.0.8/versioneer.py
+drwxr-xr-x   0 aacook     (501) staff       (20)        0 2024-05-31 21:45:02.882034 pxgrid_pyshark-0.0.9/
+-rw-r--r--   0 aacook     (501) staff       (20)    11356 2024-01-21 14:34:20.000000 pxgrid_pyshark-0.0.9/LICENSE
+-rw-r--r--   0 aacook     (501) staff       (20)       84 2024-01-24 01:20:48.000000 pxgrid_pyshark-0.0.9/MANIFEST.in
+-rw-r--r--   0 aacook     (501) staff       (20)      157 2024-01-21 14:34:20.000000 pxgrid_pyshark-0.0.9/NOTICE
+-rw-r--r--   0 aacook     (501) staff       (20)     1215 2024-05-31 21:45:02.881946 pxgrid_pyshark-0.0.9/PKG-INFO
+-rw-r--r--   0 aacook     (501) staff       (20)     9557 2024-03-05 15:01:18.000000 pxgrid_pyshark-0.0.9/README.md
+drwxr-xr-x   0 aacook     (501) staff       (20)        0 2024-05-31 21:45:02.869542 pxgrid_pyshark-0.0.9/bin/
+-rw-r--r--   0 aacook     (501) staff       (20)    15930 2024-05-31 14:32:36.000000 pxgrid_pyshark-0.0.9/bin/pxgrid-pyshark
+-rw-r--r--   0 aacook     (501) staff       (20)     4928 2024-03-23 22:15:34.000000 pxgrid_pyshark-0.0.9/bin/pxgrid-pyshark-file
+-rw-r--r--   0 aacook     (501) staff       (20)      504 2024-03-05 13:44:52.000000 pxgrid_pyshark-0.0.9/bin/pxgrid-pyshark-view
+drwxr-xr-x   0 aacook     (501) staff       (20)        0 2024-05-31 21:45:02.870526 pxgrid_pyshark-0.0.9/pxgrid_pyshark/
+-rw-r--r--   0 aacook     (501) staff       (20)      288 2024-01-21 15:03:33.000000 pxgrid_pyshark-0.0.9/pxgrid_pyshark/__init__.py
+-rw-r--r--   0 aacook     (501) staff       (20)      497 2024-05-31 21:45:02.882446 pxgrid_pyshark-0.0.9/pxgrid_pyshark/_version.py
+-rw-r--r--   0 aacook     (501) staff       (20)     3517 2024-01-28 15:21:12.000000 pxgrid_pyshark-0.0.9/pxgrid_pyshark/capture.py
+drwxr-xr-x   0 aacook     (501) staff       (20)        0 2024-05-31 21:45:02.881295 pxgrid_pyshark-0.0.9/pxgrid_pyshark/db/
+-rw-r--r--   0 aacook     (501) staff       (20)    38191 2024-05-30 16:05:10.000000 pxgrid_pyshark-0.0.9/pxgrid_pyshark/db/androids.json
+-rw-r--r--   0 aacook     (501) staff       (20)      557 2024-05-07 19:28:34.000000 pxgrid_pyshark-0.0.9/pxgrid_pyshark/db/apple-os.json
+-rw-r--r--   0 aacook     (501) staff       (20)  2899968 2024-02-26 14:35:41.000000 pxgrid_pyshark-0.0.9/pxgrid_pyshark/db/macoui.db
+-rw-r--r--   0 aacook     (501) staff       (20)  1067347 2024-02-26 14:35:41.000000 pxgrid_pyshark-0.0.9/pxgrid_pyshark/db/macoui.pipe
+-rw-r--r--   0 aacook     (501) staff       (20)  5707876 2024-02-26 14:35:41.000000 pxgrid_pyshark-0.0.9/pxgrid_pyshark/db/macoui.txt
+-rw-r--r--   0 aacook     (501) staff       (20)    55135 2024-05-31 21:38:45.000000 pxgrid_pyshark-0.0.9/pxgrid_pyshark/db/models.json
+-rw-r--r--   0 aacook     (501) staff       (20)     8504 2024-03-05 14:02:45.000000 pxgrid_pyshark-0.0.9/pxgrid_pyshark/endpointsdb.py
+-rw-r--r--   0 aacook     (501) staff       (20)     3154 2024-03-05 13:48:44.000000 pxgrid_pyshark-0.0.9/pxgrid_pyshark/ouidb.py
+-rw-r--r--   0 aacook     (501) staff       (20)    24334 2024-05-31 14:25:53.000000 pxgrid_pyshark-0.0.9/pxgrid_pyshark/parser.py
+drwxr-xr-x   0 aacook     (501) staff       (20)        0 2024-05-31 21:45:02.881596 pxgrid_pyshark-0.0.9/pxgrid_pyshark.egg-info/
+-rw-r--r--   0 aacook     (501) staff       (20)     1215 2024-05-31 21:45:02.000000 pxgrid_pyshark-0.0.9/pxgrid_pyshark.egg-info/PKG-INFO
+-rw-r--r--   0 aacook     (501) staff       (20)      665 2024-05-31 21:45:02.000000 pxgrid_pyshark-0.0.9/pxgrid_pyshark.egg-info/SOURCES.txt
+-rw-r--r--   0 aacook     (501) staff       (20)        1 2024-05-31 21:45:02.000000 pxgrid_pyshark-0.0.9/pxgrid_pyshark.egg-info/dependency_links.txt
+-rw-r--r--   0 aacook     (501) staff       (20)      117 2024-05-31 21:45:02.000000 pxgrid_pyshark-0.0.9/pxgrid_pyshark.egg-info/requires.txt
+-rwx------   0 aacook     (501) staff       (20)       15 2024-05-31 21:45:02.000000 pxgrid_pyshark-0.0.9/pxgrid_pyshark.egg-info/top_level.txt
+-rw-r--r--   0 aacook     (501) staff       (20)      210 2024-05-31 21:45:02.882328 pxgrid_pyshark-0.0.9/setup.cfg
+-rw-r--r--   0 aacook     (501) staff       (20)     2188 2024-03-05 13:51:29.000000 pxgrid_pyshark-0.0.9/setup.py
+-rw-r--r--   0 aacook     (501) staff       (20)    86677 2024-01-24 01:32:49.000000 pxgrid_pyshark-0.0.9/versioneer.py
```

### Comparing `pxgrid_pyshark-0.0.8/LICENSE` & `pxgrid_pyshark-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pxgrid_pyshark-0.0.8/PKG-INFO` & `pxgrid_pyshark-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pxgrid_pyshark
-Version: 0.0.8
+Version: 0.0.9
 Summary: Custom DPI tool used to passively analyze endpoint data and transmit results via Cisco ISE pxGrid messaging for improved endpoint profiling
 Home-page: https://github.com/taylor-cook/pxgrid-pyshark
 Download-URL: https://github.com/taylor-cook/pxgrid-pyshark
 Author: Taylor Cook
 Author-email: aacook@cisco.com
 License: Apache 2.0; Copyright (c) 2024 Cisco and/or its affiliates.
 Keywords: ISE,pxGrid
```

### Comparing `pxgrid_pyshark-0.0.8/README.md` & `pxgrid_pyshark-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pxgrid_pyshark-0.0.8/bin/pxgrid-pyshark` & `pxgrid_pyshark-0.0.9/bin/pxgrid-pyshark`

 * *Files identical despite different names*

### Comparing `pxgrid_pyshark-0.0.8/bin/pxgrid-pyshark-file` & `pxgrid_pyshark-0.0.9/bin/pxgrid-pyshark-file`

 * *Files identical despite different names*

### Comparing `pxgrid_pyshark-0.0.8/pxgrid_pyshark/capture.py` & `pxgrid_pyshark-0.0.9/pxgrid_pyshark/capture.py`

 * *Files identical despite different names*

### Comparing `pxgrid_pyshark-0.0.8/pxgrid_pyshark/db/androids.json` & `pxgrid_pyshark-0.0.9/pxgrid_pyshark/db/androids.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6357012750455373%*

 * *Differences: {"'CPH2145'": "OrderedDict([('name', 'Oppo Find X3 Lite'), ('type', 'Mobile Device')])",*

 * * "'CPH2173'": "OrderedDict([('name', 'Oppo Find X3 Pro'), ('type', 'Mobile Device')])",*

 * * "'CPH2195'": "OrderedDict([('name', 'Oppo A54 5G'), ('type', 'Mobile Device')])",*

 * * "'CPH2197'": "OrderedDict([('name', 'Oppo A74 5G'), ('type', 'Mobile Device')])",*

 * * "'CPH2207'": "OrderedDict([('name', 'Oppo Find X3 Neo'), ('type', 'Mobile Device')])",*

 * * "'CPH2249'": "OrderedDict([('name', 'Oppo Reno6 Pro 5G'), ('type', 'Mobile Devic […]*

```diff
@@ -7,34 +7,254 @@
         "name": "OnePlus 3",
         "type": "Mobile Device"
     },
     "CPH1937": {
         "name": "Oppo A9 (2020)",
         "type": "Mobile Device"
     },
+    "CPH2145": {
+        "name": "Oppo Find X3 Lite",
+        "type": "Mobile Device"
+    },
+    "CPH2173": {
+        "name": "Oppo Find X3 Pro",
+        "type": "Mobile Device"
+    },
     "CPH2185": {
         "name": "Oppo A15",
         "type": "Mobile Device"
     },
+    "CPH2195": {
+        "name": "Oppo A54 5G",
+        "type": "Mobile Device"
+    },
+    "CPH2197": {
+        "name": "Oppo A74 5G",
+        "type": "Mobile Device"
+    },
+    "CPH2207": {
+        "name": "Oppo Find X3 Neo",
+        "type": "Mobile Device"
+    },
+    "CPH2249": {
+        "name": "Oppo Reno6 Pro 5G",
+        "type": "Mobile Device"
+    },
+    "CPH2251": {
+        "name": "Oppo Reno6 5G",
+        "type": "Mobile Device"
+    },
+    "CPH2263": {
+        "name": "Oppo A74 5G",
+        "type": "Mobile Device"
+    },
+    "CPH2269": {
+        "name": "Oppo A16",
+        "type": "Mobile Device"
+    },
+    "CPH2293": {
+        "name": "Oppo Reno7 Pro 5G",
+        "type": "Mobile Device"
+    },
+    "CPH2305": {
+        "name": "Oppo Find X5 Pro",
+        "type": "Mobile Device"
+    },
+    "CPH2307": {
+        "name": "Oppo Find X5",
+        "type": "Mobile Device"
+    },
+    "CPH2325": {
+        "name": "Oppo A55",
+        "type": "Mobile Device"
+    },
+    "CPH2333": {
+        "name": "Oppo A96",
+        "type": "Mobile Device"
+    },
+    "CPH2357": {
+        "name": "Oppo Reno8 Pro 5G",
+        "type": "Mobile Device"
+    },
+    "CPH2360": {
+        "name": "Oppo Reno7",
+        "type": "Mobile Device"
+    },
+    "CPH2363": {
+        "name": "Oppo Reno7 5G",
+        "type": "Mobile Device"
+    },
+    "CPH2365": {
+        "name": "Oppo A95",
+        "type": "Mobile Device"
+    },
+    "CPH2371": {
+        "name": "Oppo Find X5 Lite",
+        "type": "Mobile Device"
+    },
+    "CPH2375": {
+        "name": "Oppo A76",
+        "type": "Mobile Device"
+    },
+    "CPH2385": {
+        "name": "Oppo A77",
+        "type": "Mobile Device"
+    },
+    "CPH2387": {
+        "name": "Oppo A57",
+        "type": "Mobile Device"
+    },
+    "CPH2447": {
+        "name": "OnePlus 11",
+        "type": "Mobile Device"
+    },
+    "CPH2449": {
+        "name": "OnePlus 11",
+        "type": "Mobile Device"
+    },
+    "CPH2451": {
+        "name": "OnePlus 11",
+        "type": "Mobile Device"
+    },
+    "CPH2457": {
+        "name": "Oppo Reno8 5G",
+        "type": "Mobile Device"
+    },
+    "CPH2459": {
+        "name": "Oppo Reno8 Z 5G",
+        "type": "Mobile Device"
+    },
+    "CPH2487": {
+        "name": "OnePlus 11r",
+        "type": "Mobile Device"
+    },
+    "CPH2573": {
+        "name": "OnePlus 12",
+        "type": "Mobile Device"
+    },
+    "CPH2581": {
+        "name": "OnePlus 12",
+        "type": "Mobile Device"
+    },
+    "CPH2585": {
+        "name": "OnePlus 12r",
+        "type": "Mobile Device"
+    },
+    "CPH2609": {
+        "name": "OnePlus 12r",
+        "type": "Mobile Device"
+    },
+    "CPH2631": {
+        "name": "Oppo A60",
+        "type": "Mobile Device"
+    },
+    "G1MNW": {
+        "name": "Google Pixel 8 Pro",
+        "type": "Mobile Device"
+    },
+    "G8VOU": {
+        "name": "Google Pixel 6 Pro",
+        "type": "Mobile Device"
+    },
+    "G9BQD": {
+        "name": "Google Pixel 8",
+        "type": "Mobile Device"
+    },
+    "G9S9B": {
+        "name": "Google Pixel 6",
+        "type": "Mobile Device"
+    },
+    "G9S9B16": {
+        "name": "Google Pixel 6",
+        "type": "Mobile Device"
+    },
+    "GA04851-US": {
+        "name": "Google Pixel 8",
+        "type": "Mobile Device"
+    },
+    "GB7N6": {
+        "name": "Google Pixel 6",
+        "type": "Mobile Device"
+    },
+    "GC3VE": {
+        "name": "Google Pixel 8 Pro",
+        "type": "Mobile Device"
+    },
     "GE2AE": {
         "name": "Google Pixel 7 Pro",
         "type": "Mobile Device"
     },
+    "GF5KQ": {
+        "name": "Google Pixel 6 Pro",
+        "type": "Mobile Device"
+    },
     "GFE4J": {
         "name": "Google Pixel 7 Pro",
         "type": "Mobile Device"
     },
+    "GKWS6": {
+        "name": "Google Pixel 8",
+        "type": "Mobile Device"
+    },
+    "GLUOG": {
+        "name": "Google Pixel 6 Pro",
+        "type": "Mobile Device"
+    },
+    "GO3Z5": {
+        "name": "Google Pixel 7",
+        "type": "Mobile Device"
+    },
     "GP4BC": {
         "name": "Google Pixel 7 Pro",
         "type": "Mobile Device"
     },
+    "GPJ41": {
+        "name": "Google Pixel 8",
+        "type": "Mobile Device"
+    },
+    "GQML3": {
+        "name": "Google Pixel 7",
+        "type": "Mobile Device"
+    },
+    "GR1YH": {
+        "name": "Google Pixel 6",
+        "type": "Mobile Device"
+    },
+    "GVU6C": {
+        "name": "Google Pixel 7",
+        "type": "Mobile Device"
+    },
+    "GZPFO": {
+        "name": "Google Pixel 8",
+        "type": "Mobile Device"
+    },
     "M-F7000": {
         "name": "Samsung Galaxy Z Flip",
         "type": "Mobile Device"
     },
+    "NE2210": {
+        "name": "OnePlus 10 Pro",
+        "type": "Mobile Device"
+    },
+    "NE2211": {
+        "name": "OnePlus 10 Pro",
+        "type": "Mobile Device"
+    },
+    "NE2213": {
+        "name": "OnePlus 10 Pro",
+        "type": "Mobile Device"
+    },
+    "NE2215": {
+        "name": "OnePlus 10 Pro",
+        "type": "Mobile Device"
+    },
+    "NE2217": {
+        "name": "OnePlus 10 Pro",
+        "type": "Mobile Device"
+    },
     "OnePlus KB2000": {
         "name": "OnePlus 8T",
         "type": "Mobile Device"
     },
     "OnePlus KB2001": {
         "name": "OnePlus 8T",
         "type": "Mobile Device"
@@ -63,14 +283,22 @@
         "name": "OnePlus 9",
         "type": "Mobile Device"
     },
     "OnePlus LE2115": {
         "name": "OnePlus 9",
         "type": "Mobile Device"
     },
+    "OnePlus LE2117": {
+        "name": "OnePlus 9",
+        "type": "Mobile Device"
+    },
+    "PHB110": {
+        "name": "OnePlus 11",
+        "type": "Mobile Device"
+    },
     "SC-41A": {
         "name": "Samsung Galaxy A41",
         "type": "Mobile Device"
     },
     "SCV48": {
         "name": "Samsung Galaxy A41",
         "type": "Mobile Device"
@@ -727,14 +955,30 @@
         "name": "Samsung Galaxy A34",
         "type": "Mobile Device"
     },
     "SM-A346M": {
         "name": "Samsung Galaxy A34",
         "type": "Mobile Device"
     },
+    "SM-A356B": {
+        "name": "Samsung Galaxy A35",
+        "type": "Mobile Device"
+    },
+    "SM-A356E": {
+        "name": "Samsung Galaxy A35",
+        "type": "Mobile Device"
+    },
+    "SM-A356U": {
+        "name": "Samsung Galaxy A35",
+        "type": "Mobile Device"
+    },
+    "SM-A356U1": {
+        "name": "Samsung Galaxy A35",
+        "type": "Mobile Device"
+    },
     "SM-A405FM": {
         "name": "Samsung Galaxy A40",
         "type": "Mobile Device"
     },
     "SM-A405FN": {
         "name": "Samsung Galaxy A40",
         "type": "Mobile Device"
@@ -911,26 +1155,38 @@
         "name": "Samsung Galaxy A8 (2018)",
         "type": "Mobile Device"
     },
     "SM-A530W": {
         "name": "Samsung Galaxy A8 (2018)",
         "type": "Mobile Device"
     },
+    "SM-A5360": {
+        "name": "Samsung Galaxy A53 5G",
+        "type": "Mobile Device"
+    },
     "SM-A536B": {
         "name": "Samsung Galaxy A53",
         "type": "Mobile Device"
     },
     "SM-A536E": {
         "name": "Samsung Galaxy A53",
         "type": "Mobile Device"
     },
     "SM-A536U": {
         "name": "Samsung Galaxy A53",
         "type": "Mobile Device"
     },
+    "SM-A536V": {
+        "name": "Samsung Galaxy A53 5G",
+        "type": "Mobile Device"
+    },
+    "SM-A536W": {
+        "name": "Samsung Galaxy A53 5G",
+        "type": "Mobile Device"
+    },
     "SM-A5460": {
         "name": "Samsung Galaxy A54",
         "type": "Mobile Device"
     },
     "SM-A546B": {
         "name": "Samsung Galaxy A54",
         "type": "Mobile Device"
@@ -975,18 +1231,158 @@
         "name": "Samsung Galaxy A55",
         "type": "Mobile Device"
     },
     "SM-A556V": {
         "name": "Samsung Galaxy A55",
         "type": "Mobile Device"
     },
+    "SM-A600A": {
+        "name": "Samsung Galaxy A6",
+        "type": "Mobile Device"
+    },
+    "SM-A600FN": {
+        "name": "Samsung Galaxy A6",
+        "type": "Mobile Device"
+    },
+    "SM-A600GN": {
+        "name": "Samsung Galaxy A6",
+        "type": "Mobile Device"
+    },
+    "SM-A605FN": {
+        "name": "Samsung Galaxy A6+",
+        "type": "Mobile Device"
+    },
+    "SM-A605G": {
+        "name": "Samsung Galaxy A6+",
+        "type": "Mobile Device"
+    },
+    "SM-A605K": {
+        "name": "Samsung Galaxy A6+",
+        "type": "Mobile Device"
+    },
+    "SM-A6060": {
+        "name": "Samsung Galaxy A60",
+        "type": "Mobile Device"
+    },
+    "SM-A606Y": {
+        "name": "Samsung Galaxy A60",
+        "type": "Mobile Device"
+    },
+    "SM-A700F": {
+        "name": "Samsung Galaxy A7",
+        "type": "Mobile Device"
+    },
+    "SM-A700FD": {
+        "name": "Samsung Galaxy A7",
+        "type": "Mobile Device"
+    },
+    "SM-A700H": {
+        "name": "Samsung Galaxy A7 Duos",
+        "type": "Mobile Device"
+    },
+    "SM-A700L": {
+        "name": "Samsung Galaxy A7",
+        "type": "Mobile Device"
+    },
+    "SM-A700S": {
+        "name": "Samsung Galaxy A7",
+        "type": "Mobile Device"
+    },
+    "SM-A700YD": {
+        "name": "Samsung Galaxy A7 Duos",
+        "type": "Mobile Device"
+    },
+    "SM-A7050": {
+        "name": "Samsung Galaxy A70",
+        "type": "Mobile Device"
+    },
+    "SM-A705F": {
+        "name": "Samsung Galaxy A70",
+        "type": "Mobile Device"
+    },
+    "SM-A705FN": {
+        "name": "Samsung Galaxy A70",
+        "type": "Mobile Device"
+    },
     "SM-A705MN": {
         "name": "Samsung Galaxy A70",
         "type": "Mobile Device"
     },
+    "SM-A707F": {
+        "name": "Samsung Galaxy A70s",
+        "type": "Mobile Device"
+    },
+    "SM-A710FD": {
+        "name": "Samsung Galaxy A7",
+        "type": "Mobile Device"
+    },
+    "SM-A715F": {
+        "name": "Samsung Galaxy A71",
+        "type": "Mobile Device"
+    },
+    "SM-A7160": {
+        "name": "Samsung Galaxy A71 5G",
+        "type": "Mobile Device"
+    },
+    "SM-A716S": {
+        "name": "Samsung Galaxy A71 5G",
+        "type": "Mobile Device"
+    },
+    "SM-A716U": {
+        "name": "Samsung Galaxy A71 5G",
+        "type": "Mobile Device"
+    },
+    "SM-A716V": {
+        "name": "Samsung Galaxy A71 5G",
+        "type": "Mobile Device"
+    },
+    "SM-A720F": {
+        "name": "Samsung Galaxy A7",
+        "type": "Mobile Device"
+    },
+    "SM-A725F": {
+        "name": "Samsung Galaxy A72",
+        "type": "Mobile Device"
+    },
+    "SM-A730F": {
+        "name": "Samsung Galaxy A8+",
+        "type": "Mobile Device"
+    },
+    "SM-A736B": {
+        "name": "Samsung Galaxy A73 5G",
+        "type": "Mobile Device"
+    },
+    "SM-A750F": {
+        "name": "Samsung Galaxy A7",
+        "type": "Mobile Device"
+    },
+    "SM-A750FN": {
+        "name": "Samsung Galaxy A7",
+        "type": "Mobile Device"
+    },
+    "SM-A750G": {
+        "name": "Samsung Galaxy A7",
+        "type": "Mobile Device"
+    },
+    "SM-A800F": {
+        "name": "Samsung Galaxy A8",
+        "type": "Mobile Device"
+    },
+    "SM-A805F": {
+        "name": "Samsung Galaxy A80",
+        "type": "Mobile Device"
+    },
+    "SM-A805N": {
+        "name": "Samsung Galaxy A80",
+        "type": "Mobile Device"
+    },
+    "SM-A805X": {
+        "name": "Samsung Galaxy A80",
+        "type": "Mobile Device"
+    },
     "SM-A8100": {
         "name": "Samsung Galaxy A8 (2016)",
         "type": "Mobile Device"
     },
     "SM-A810F": {
         "name": "Samsung Galaxy A8 (2016)",
         "type": "Mobile Device"
@@ -1115,14 +1511,22 @@
         "name": "Samsung Galaxy F42 5G",
         "type": "Mobile Device"
     },
     "SM-E5260": {
         "name": "Samsung Galaxy F52 5G",
         "type": "Mobile Device"
     },
+    "SM-E546B": {
+        "name": "Samsung Galaxy F54",
+        "type": "Mobile Device"
+    },
+    "SM-E556B": {
+        "name": "Samsung Galaxy F55",
+        "type": "Mobile Device"
+    },
     "SM-E625F": {
         "name": "Samsung Galaxy F62",
         "type": "Mobile Device"
     },
     "SM-F127F": {
         "name": "Samsung Galaxy F12",
         "type": "Mobile Device"
@@ -1287,14 +1691,270 @@
         "name": "Samsung Galaxy Z Fold2 5G",
         "type": "Mobile Device"
     },
     "SM-F916W": {
         "name": "Samsung Galaxy Z Fold2 5G",
         "type": "Mobile Device"
     },
+    "SM-F926B": {
+        "name": "Samsung Galaxy Z Fold3 5G",
+        "type": "Mobile Device"
+    },
+    "SM-F926N": {
+        "name": "Samsung Galaxy Z Fold3 5G",
+        "type": "Mobile Device"
+    },
+    "SM-F926U": {
+        "name": "Samsung Galaxy Z Fold3 5G",
+        "type": "Mobile Device"
+    },
+    "SM-F926U1": {
+        "name": "Samsung Galaxy Z Fold3 5G",
+        "type": "Mobile Device"
+    },
+    "SM-F936B": {
+        "name": "Samsung Galaxy Z Fold4",
+        "type": "Mobile Device"
+    },
+    "SM-F936U": {
+        "name": "Samsung Galaxy Z Fold4",
+        "type": "Mobile Device"
+    },
+    "SM-F936U1": {
+        "name": "Samsung Galaxy Z Fold4",
+        "type": "Mobile Device"
+    },
+    "SM-F936W": {
+        "name": "Samsung Galaxy Z Fold4",
+        "type": "Mobile Device"
+    },
+    "SM-F9460": {
+        "name": "Samsung Galaxy Z Fold5",
+        "type": "Mobile Device"
+    },
+    "SM-F946B": {
+        "name": "Samsung Galaxy Z Fold5",
+        "type": "Mobile Device"
+    },
+    "SM-F946U": {
+        "name": "Samsung Galaxy Z Fold5",
+        "type": "Mobile Device"
+    },
+    "SM-F946U1": {
+        "name": "Samsung Galaxy Z Fold5",
+        "type": "Mobile Device"
+    },
+    "SM-F946W": {
+        "name": "Samsung Galaxy Z Fold5",
+        "type": "Mobile Device"
+    },
+    "SM-G130HN": {
+        "name": "Samsung Galaxy Young 2",
+        "type": "Mobile Device"
+    },
+    "SM-J810Y": {
+        "name": "Samsung Galaxy J8",
+        "type": ""
+    },
+    "SM-M013F": {
+        "name": "Samsung Galaxy M01 Core",
+        "type": ""
+    },
+    "SM-M236B": {
+        "name": "Samsung Galaxy M23",
+        "type": ""
+    },
+    "SM-M236L": {
+        "name": "Samsung Galaxy M23",
+        "type": ""
+    },
+    "SM-M305F": {
+        "name": "Samsung Galaxy M30",
+        "type": ""
+    },
+    "SM-M305M": {
+        "name": "Samsung Galaxy M30",
+        "type": ""
+    },
+    "SM-M315F": {
+        "name": "Samsung Galaxy M31'",
+        "type": ""
+    },
+    "SM-M317F": {
+        "name": "Samsung Galaxy M31f",
+        "type": ""
+    },
+    "SM-M325F": {
+        "name": "Samsung Galaxy M32",
+        "type": ""
+    },
+    "SM-M325FV": {
+        "name": "Samsung Galaxy M32",
+        "type": ""
+    },
+    "SM-M326B": {
+        "name": "Samsung Galaxy M32 5G",
+        "type": ""
+    },
+    "SM-M336B": {
+        "name": "Samsung Galaxy M33",
+        "type": ""
+    },
+    "SM-M336BU": {
+        "name": "Samsung Galaxy M33",
+        "type": ""
+    },
+    "SM-M336K": {
+        "name": "Samsung Galaxy M33",
+        "type": ""
+    },
+    "SM-M346B": {
+        "name": "Samsung Galaxy M34 5G",
+        "type": ""
+    },
+    "SM-M356B": {
+        "name": "Samsung Galaxy M35",
+        "type": ""
+    },
+    "SM-M405F": {
+        "name": "Samsung Galaxy M40",
+        "type": ""
+    },
+    "SM-M426B": {
+        "name": "Samsung Galaxy M42 5G",
+        "type": ""
+    },
+    "SM-M515F": {
+        "name": "Samsung Galaxy M51",
+        "type": ""
+    },
+    "SM-M526B": {
+        "name": "Samsung Galaxy M52 5G",
+        "type": ""
+    },
+    "SM-M526BR": {
+        "name": "Samsung Galaxy M52 5G",
+        "type": ""
+    },
+    "SM-M536B": {
+        "name": "Samsung Galaxy M53",
+        "type": ""
+    },
+    "SM-M536S": {
+        "name": "Samsung Galaxy M53",
+        "type": ""
+    },
+    "SM-M546B": {
+        "name": "Samsung Galaxy M54",
+        "type": ""
+    },
+    "SM-M625F": {
+        "name": "Samsung Galaxy M62",
+        "type": ""
+    },
+    "SM-N7505": {
+        "name": "Samsung Galaxy Note 3 Neo",
+        "type": ""
+    },
+    "SM-N930F": {
+        "name": "Samsung Galaxy Note7",
+        "type": "Mobile Device"
+    },
+    "SM-N935L": {
+        "name": "Samsung Galaxy Note FE",
+        "type": "Mobile Device"
+    },
+    "SM-N950F": {
+        "name": "Samsung Galaxy Note8",
+        "type": "Mobile Device"
+    },
+    "SM-N950N": {
+        "name": "Samsung Galaxy Note8",
+        "type": "Mobile Device"
+    },
+    "SM-N950U": {
+        "name": "Samsung Galaxy Note8",
+        "type": "Mobile Device"
+    },
+    "SM-N960F": {
+        "name": "Samsung Galaxy Note9",
+        "type": "Mobile Device"
+    },
+    "SM-N960U": {
+        "name": "Samsung Galaxy Note9",
+        "type": "Mobile Device"
+    },
+    "SM-N960W": {
+        "name": "Samsung Galaxy Note9",
+        "type": "Mobile Device"
+    },
+    "SM-N9700": {
+        "name": "Samsung Galaxy Note10",
+        "type": "Mobile Device"
+    },
+    "SM-N970F": {
+        "name": "Samsung Galaxy Note10",
+        "type": "Mobile Device"
+    },
+    "SM-N975F": {
+        "name": "Samsung Galaxy Note10+",
+        "type": "Mobile Device"
+    },
+    "SM-N975U": {
+        "name": "Samsung Galaxy Note10+",
+        "type": "Mobile Device"
+    },
+    "SM-N975W": {
+        "name": "Samsung Galaxy Note10+",
+        "type": "Mobile Device"
+    },
+    "SM-N976B": {
+        "name": "Samsung Galaxy Note10+ 5G",
+        "type": "Mobile Device"
+    },
+    "SM-N976N": {
+        "name": "Samsung Galaxy Note10+ 5G",
+        "type": "Mobile Device"
+    },
+    "SM-N976U": {
+        "name": "Samsung Galaxy Note10+ 5G",
+        "type": "Mobile Device"
+    },
+    "SM-N976V": {
+        "name": "Samsung Galaxy Note10+ 5G",
+        "type": "Mobile Device"
+    },
+    "SM-N980F": {
+        "name": "Samsung Galaxy Note20",
+        "type": "Mobile Device"
+    },
+    "SM-N981B": {
+        "name": "Samsung Galaxy Note20 5G",
+        "type": "Mobile Device"
+    },
+    "SM-N981U": {
+        "name": "Samsung Galaxy Note20 5G",
+        "type": "Mobile Device"
+    },
+    "SM-N985F": {
+        "name": "SamSung Galaxy Note 20 Ultra",
+        "type": "Mobile Device"
+    },
+    "SM-N986B": {
+        "name": "Samsung Galaxy Note20 Ultra 5G",
+        "type": "Mobile Device"
+    },
+    "SM-N986N": {
+        "name": "Samsung Galaxy Note20 Ultra 5G",
+        "type": "Mobile Device"
+    },
+    "SM-N986W": {
+        "name": "Samsung Galaxy Note20 Ultra 5G",
+        "type": "Mobile Device"
+    },
     "SM-S102DL": {
         "name": "Samsung Galaxy A10e",
         "type": "Mobile Device"
     },
     "SM-S111DL": {
         "name": "Samsung Galaxy A01",
         "type": "Mobile Device"
@@ -1327,14 +1987,154 @@
         "name": "Samsung Galaxy A21",
         "type": "Mobile Device"
     },
     "SM-S326DL": {
         "name": "Samsung Galaxy A32 5G",
         "type": "Mobile Device"
     },
+    "SM-S337TL": {
+        "name": "Samsung Galaxy J3",
+        "type": "Mobile Device"
+    },
+    "SM-S7110": {
+        "name": "Samsung Galaxy S23 FE",
+        "type": "Mobile Device"
+    },
+    "SM-S711U": {
+        "name": "Samsung Galaxy S23 FE",
+        "type": "Mobile Device"
+    },
+    "SM-S711W": {
+        "name": "Samsung Galaxy S23 FE",
+        "type": "Mobile Device"
+    },
+    "SM-S727VL": {
+        "name": "Samsung Galaxy J7",
+        "type": "Mobile Device"
+    },
+    "SM-S901B": {
+        "name": "Samsung Galaxy S22 5G",
+        "type": "Mobile Device"
+    },
+    "SM-S901E": {
+        "name": "Samsung Galaxy S22 5G",
+        "type": "Mobile Device"
+    },
+    "SM-S901U": {
+        "name": "Samsung Galaxy S22 5G",
+        "type": "Mobile Device"
+    },
+    "SM-S901U1": {
+        "name": "Samsung Galaxy S22 5G",
+        "type": "Mobile Device"
+    },
+    "SM-S901W": {
+        "name": "Samsung Galaxy S22 5G",
+        "type": "Mobile Device"
+    },
+    "SM-S9060": {
+        "name": "Samsung Galaxy S22+ 5G",
+        "type": "Mobile Device"
+    },
+    "SM-S906B": {
+        "name": "Samsung Galaxy S22+ 5G",
+        "type": "Mobile Device"
+    },
+    "SM-S906E": {
+        "name": "Samsung Galaxy S22+ 5G",
+        "type": "Mobile Device"
+    },
+    "SM-S906N": {
+        "name": "Samsung Galaxy S22+ 5G",
+        "type": "Mobile Device"
+    },
+    "SM-S906U": {
+        "name": "Samsung Galaxy S22+ 5G",
+        "type": "Mobile Device"
+    },
+    "SM-S906W": {
+        "name": "Samsung Galaxy S22+ 5G",
+        "type": "Mobile Device"
+    },
+    "SM-S907VL": {
+        "name": "Samsung Galaxy S6",
+        "type": "Mobile Device"
+    },
+    "SM-S908B": {
+        "name": "Samsung Galaxy S22 Ultra 5G",
+        "type": "Mobile Device"
+    },
+    "SM-S908N": {
+        "name": "Samsung Galaxy S22 Ultra 5G",
+        "type": "Mobile Device"
+    },
+    "SM-S908U": {
+        "name": "Samsung Galaxy S22 Ultra 5G",
+        "type": "Mobile Device"
+    },
+    "SM-S911B": {
+        "name": "Samsung Galaxy S23",
+        "type": "Mobile Device"
+    },
+    "SM-S911U": {
+        "name": "Samsung Galaxy S23",
+        "type": "Mobile Device"
+    },
+    "SM-S911U1": {
+        "name": "Samsung Galaxy S23",
+        "type": "Mobile Device"
+    },
+    "SM-S911W": {
+        "name": "Samsung Galaxy S23",
+        "type": "Mobile Device"
+    },
+    "SM-S916B": {
+        "name": "Samsung Galaxy S23+",
+        "type": "Mobile Device"
+    },
+    "SM-S916U": {
+        "name": "Samsung Galaxy S23+",
+        "type": "Mobile Device"
+    },
+    "SM-S916U1": {
+        "name": "Samsung Galaxy S23+",
+        "type": "Mobile Device"
+    },
+    "SM-S916W": {
+        "name": "Samsung Galaxy S23+",
+        "type": "Mobile Device"
+    },
+    "SM-S9180": {
+        "name": "Samsung Galaxy S23 Ultra",
+        "type": "Mobile Device"
+    },
+    "SM-S918B": {
+        "name": "Samsung Galaxy S23 Ultra",
+        "type": "Mobile Device"
+    },
+    "SM-S918E": {
+        "name": "Samsung Galaxy S23 Ultra",
+        "type": "Mobile Device"
+    },
+    "SM-S918N": {
+        "name": "Samsung Galaxy S23 Ultra",
+        "type": "Mobile Device"
+    },
+    "SM-S918U": {
+        "name": "Samsung Galaxy S23 Ultra",
+        "type": "Mobile Device"
+    },
+    "SM-S918U1": {
+        "name": "Samsung Galaxy S23 Ultra",
+        "type": "Mobile Device"
+    },
+    "SM-S918W": {
+        "name": "Samsung Galaxy S23 Ultra",
+        "type": "Mobile Device"
+    },
     "SM-S9210": {
         "name": "Samsung Galaxy S24",
         "type": "Mobile Device"
     },
     "SM-S921B": {
         "name": "Samsung Galaxy S24",
         "type": "Mobile Device"
```

### Comparing `pxgrid_pyshark-0.0.8/pxgrid_pyshark/db/macoui.db` & `pxgrid_pyshark-0.0.9/pxgrid_pyshark/db/macoui.db`

 * *Files identical despite different names*

### Comparing `pxgrid_pyshark-0.0.8/pxgrid_pyshark/db/macoui.pipe` & `pxgrid_pyshark-0.0.9/pxgrid_pyshark/db/macoui.pipe`

 * *Files identical despite different names*

### Comparing `pxgrid_pyshark-0.0.8/pxgrid_pyshark/db/macoui.txt` & `pxgrid_pyshark-0.0.9/pxgrid_pyshark/db/macoui.txt`

 * *Files identical despite different names*

### Comparing `pxgrid_pyshark-0.0.8/pxgrid_pyshark/db/models.json` & `pxgrid_pyshark-0.0.9/pxgrid_pyshark/db/models.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9215605826575707%*

 * *Differences: {"'Apple'": "{'model=Mac14,2': {'name': 'MacBookAir (M2, 2022)'}}",*

 * * "'Microsoft'": "{'md=XboxOneS': OrderedDict([('name', 'Xbox One S'), ('type', 'Gaming Device')]), "*

 * *                "'md=XboxOneX': OrderedDict([('name', 'Xbox One X'), ('type', 'Gaming Device')])}",*

 * * "'Samsung Electronics'": "OrderedDict([('UN40JU6400', OrderedDict([('name', 'Samsung UHD TV "*

 * *                          "40in'), ('type', 'Smart TV')])), ('UN43JU6400', OrderedDict([('name', "*

 * *                          "'Samsung UHD TV 43in') […]*

```diff
@@ -709,15 +709,15 @@
             "type": "Workstation"
         },
         "model=Mac14,15": {
             "name": "Macbook Air (15-inch, M2 2023)",
             "type": "Workstation"
         },
         "model=Mac14,2": {
-            "name": "MacBookAir M2, 2022)",
+            "name": "MacBookAir (M2, 2022)",
             "type": "Workstation"
         },
         "model=Mac14,3": {
             "name": "Mac Mini (M2, 2023)",
             "type": "Workstation"
         },
         "model=Mac14,5": {
@@ -1933,14 +1933,22 @@
             "type": "Smart TV"
         }
     },
     "Microsoft": {
         "md=XboxOne": {
             "name": "Xbox One",
             "type": "Gaming Device"
+        },
+        "md=XboxOneS": {
+            "name": "Xbox One S",
+            "type": "Gaming Device"
+        },
+        "md=XboxOneX": {
+            "name": "Xbox One X",
+            "type": "Gaming Device"
         }
     },
     "Murata Manufacturing": {
         "SM-G975U": {
             "name": "Galaxy S10 Plus",
             "type": "Mobile Device"
         },
@@ -2333,14 +2341,148 @@
             "type": "IOT Device"
         },
         "model=N1101": {
             "name": "Roku HD-XR",
             "type": "IOT Device"
         }
     },
+    "Samsung Electronics": {
+        "QN50Q60T": {
+            "name": "Samsung QLED UHD TV 50in",
+            "type": "Smart TV"
+        },
+        "QN55Q60T": {
+            "name": "Samsung QLED UHD TV 55in",
+            "type": "Smart TV"
+        },
+        "QN55QN85": {
+            "name": "Samsung QLED UHD TV 55in",
+            "type": "Smart TV"
+        },
+        "QN58Q60T": {
+            "name": "Samsung QLED UHD TV 58in",
+            "type": "Smart TV"
+        },
+        "QN65Q60T": {
+            "name": "Samsung QLED UHD TV 65in",
+            "type": "Smart TV"
+        },
+        "QN65QN85": {
+            "name": "Samsung QLED UHD TV 65in",
+            "type": "Smart TV"
+        },
+        "QN70Q6DT": {
+            "name": "Samsung QLED UHD TV 70in",
+            "type": "Smart TV"
+        },
+        "QN75Q60T": {
+            "name": "Samsung QLED UHD TV 75in",
+            "type": "Smart TV"
+        },
+        "QN75QN85": {
+            "name": "Samsung QLED UHD TV 75in",
+            "type": "Smart TV"
+        },
+        "QN82Q60T": {
+            "name": "Samsung QLED UHD TV 82in",
+            "type": "Smart TV"
+        },
+        "QN85Q60T": {
+            "name": "Samsung QLED UHD TV 85in",
+            "type": "Smart TV"
+        },
+        "QN85QN85": {
+            "name": "Samsung QLED UHD TV 85in",
+            "type": "Smart TV"
+        },
+        "UN40JU6400": {
+            "name": "Samsung UHD TV 40in",
+            "type": "Smart TV"
+        },
+        "UN43JU6400": {
+            "name": "Samsung UHD TV 43in",
+            "type": "Smart TV"
+        },
+        "UN43TU7000": {
+            "name": "Samsung UHD HDR TV 43in",
+            "type": "Smart TV"
+        },
+        "UN48JU6400": {
+            "name": "Samsung UHD TV 48in",
+            "type": "Smart TV"
+        },
+        "UN50CU8000": {
+            "name": "Samsung Crystal UHD TV 50in",
+            "type": "Smart TV"
+        },
+        "UN50TU7000": {
+            "name": "Samsung UHD HDR TV 50in",
+            "type": "Smart TV"
+        },
+        "UN55CU8000": {
+            "name": "Samsung Crystal UHD TV 55in",
+            "type": "Smart TV"
+        },
+        "UN55JU6400": {
+            "name": "Samsung UHD TV 55in",
+            "type": "Smart TV"
+        },
+        "UN55TU7000": {
+            "name": "Samsung UHD HDR TV 55in",
+            "type": "Smart TV"
+        },
+        "UN58TU7000": {
+            "name": "Samsung UHD HDR TV 68in",
+            "type": "Smart TV"
+        },
+        "UN60JU6400": {
+            "name": "Samsung UHD TV 60in",
+            "type": "Smart TV"
+        },
+        "UN60TU7000": {
+            "name": "Samsung UHD HDR TV 60in",
+            "type": "Smart TV"
+        },
+        "UN65CU8000": {
+            "name": "Samsung Crystal UHD TV 65in",
+            "type": "Smart TV"
+        },
+        "UN65JU6400": {
+            "name": "Samsung UHD TV 65in",
+            "type": "Smart TV"
+        },
+        "UN65TU7000": {
+            "name": "Samsung UHD HDR TV 65in",
+            "type": "Smart TV"
+        },
+        "UN70TU7000": {
+            "name": "Samsung UHD HDR TV 70in",
+            "type": "Smart TV"
+        },
+        "UN75CU8000": {
+            "name": "Samsung Crystal UHD TV 75in",
+            "type": "Smart TV"
+        },
+        "UN75TU7000": {
+            "name": "Samsung UHD HDR TV 75in",
+            "type": "Smart TV"
+        },
+        "UN82TU7000": {
+            "name": "Samsung UHD HDR TV 82in",
+            "type": "Smart TV"
+        },
+        "UN85CU8000": {
+            "name": "Samsung Crystal UHD TV 85in",
+            "type": "Smart TV"
+        },
+        "UN85TU7000": {
+            "name": "Samsung UHD HDR TV 85in",
+            "type": "Smart TV"
+        }
+    },
     "Smart Innovation LLC": {
         "md=T7400": {
             "name": "Smart Safe S10",
             "type": "IOT Device"
         },
         "md=T7401": {
             "name": "Smart Safe S12",
```

### Comparing `pxgrid_pyshark-0.0.8/pxgrid_pyshark/endpointsdb.py` & `pxgrid_pyshark-0.0.9/pxgrid_pyshark/endpointsdb.py`

 * *Files identical despite different names*

### Comparing `pxgrid_pyshark-0.0.8/pxgrid_pyshark/ouidb.py` & `pxgrid_pyshark-0.0.9/pxgrid_pyshark/ouidb.py`

 * *Files identical despite different names*

### Comparing `pxgrid_pyshark-0.0.8/pxgrid_pyshark/parser.py` & `pxgrid_pyshark-0.0.9/pxgrid_pyshark/parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -271,24 +271,47 @@
             layer = packet['XML']
             binary_xml = binascii.unhexlify(packet.xml_raw.value)  ## Convert the XML data raw into a string, which is in binary format
             root = ET.fromstring(binary_xml)
 
             ## TO DO: IMPROVE XML PARSING METHOD ##
             try:
                 # Extract data from the XML
-                asset_values[4] = root.find(".//{urn:schemas-upnp-org:device-1-0}friendlyName").text
-                asset_values[12] = 80
-                asset_values[5] = root.find(".//{urn:schemas-upnp-org:device-1-0}manufacturer").text
-                asset_values[13] = 80
-                asset_values[6] = root.find(".//{urn:schemas-upnp-org:device-1-0}modelName").text
-                asset_values[14] = 80
-                asset_values[8] = root.find(".//{urn:schemas-upnp-org:device-1-0}modelNumber").text
-                asset_values[16] = 80
-                asset_values[9] = root.find(".//{urn:schemas-upnp-org:device-1-0}serialNumber").text
-                asset_values[17] = 80
+                friendlyName = root.find(".//{urn:schemas-upnp-org:device-1-0}friendlyName")
+                if friendlyName is not None:
+                    asset_values[4] = friendlyName.text
+                    asset_values[12] = 80
+                manufacturer = root.find(".//{urn:schemas-upnp-org:device-1-0}manufacturer")
+                if manufacturer is not None:
+                    asset_values[5] = manufacturer.text
+                    asset_values[13] = 80
+                modelNumber = root.find(".//{urn:schemas-upnp-org:device-1-0}modelNumber")
+                if modelNumber is not None:
+                    asset_values[8] = modelNumber.text
+                    asset_values[16] = 70
+                modelName = root.find(".//{urn:schemas-upnp-org:device-1-0}modelName")
+                if modelName is not None:
+                    asset_values[6] = modelName.text
+                    asset_values[14] = 70
+                    asset_values = self.parse_model_and_os(asset_values,modelName.text)
+                serialNumber = root.find(".//{urn:schemas-upnp-org:device-1-0}serialNumber")
+                if serialNumber is not None:
+                    asset_values[9] = serialNumber.text
+                    asset_values[17] = 80
+                # print(asset_values)
+
+                # asset_values[4] = root.find(".//{urn:schemas-upnp-org:device-1-0}friendlyName").text
+                # asset_values[12] = 80
+                # asset_values[5] = root.find(".//{urn:schemas-upnp-org:device-1-0}manufacturer").text
+                # asset_values[13] = 80
+                # asset_values[6] = root.find(".//{urn:schemas-upnp-org:device-1-0}modelName").text
+                # asset_values[14] = 80
+                # asset_values[8] = root.find(".//{urn:schemas-upnp-org:device-1-0}modelNumber").text
+                # asset_values[16] = 80
+                # asset_values[9] = root.find(".//{urn:schemas-upnp-org:device-1-0}serialNumber").text
+                # asset_values[17] = 80
             except Exception as e:
                 logger.debug(f'Error processing {asset_values[1]} packet: {e}')
                 pass
             return asset_values
         except AttributeError:
             return None
         
@@ -330,176 +353,14 @@
                 asset_values[4] = layer.server      #record the hostname field and weighting
                 asset_values[12] = 80
             return asset_values
         except Exception as e:
             logger.debug(f'Error for {asset_values[1]} packet from {asset_values[0]}: {e}')
             return None
 
-    def parse_mdns_v5(self, packet):
-        mac, ip, vendor = self.parse_mac_ip(packet)
-        asset_values = ['']*11 + ['0']*8      # Create an empty list for potential values
-        
-        if mac is None:
-            return None
-        asset_values[0] = mac
-        asset_values[5] = vendor
-        if ip is not None:
-            asset_values[2] = ip
-        asset_values[1] = 'mDNS'
-        try:
-            layer = packet['mdns']
-            if int(layer.answers) >0:
-                for key in layer._all_fields['Answers']:
-                    ## If an Apple device and an mDNS "device-info" advertisement, parse known attributes of endpoint
-                    if layer._all_fields['Answers'][key]['dns.resp.type'] == '16' and 'device-info' in key:
-                        asset_values[4] = layer._all_fields['Answers'][key]['dns.resp.name'].partition('.')[0]  #Return the name up to the first '.'
-                        asset_values[12] = 80
-                        dns_txt = str(layer._all_fields['Answers'][key]['dns.txt'])
-                        asset_values = self.parse_model_and_os(asset_values, dns_txt)
-                        return asset_values
-                    
-                    elif layer._all_fields['Answers'][key]['dns.resp.type'] == '16':
-                        for item in layer._all_fields['Answers'][key]['dns.txt']:
-                            if 'model=' in item or 'MDL=' in item or 'md=' in item or 'modelid=' in item or 'usb_MDL=' in item:
-                                asset_values = self.parse_model_and_os(asset_values, item)
-                            elif 'MFG=' in item or 'manufacturer=' in item:
-                                asset_values[5] = item.partition('=')[2]   ## Return only the value after the '='
-                                asset_values[13] = 50
-                            elif 'UUID=' in item or 'serialNumber=' in item:
-                                asset_values[9] = item.partition('=')[2]
-                                asset_values[17] = 50
-                            elif 'deviceid=' in item and asset_values[0] in item:
-                                #Only store the "deviceid=" value if it is not the MAC address
-                                if str(item.partition('=')[2]).lower() is not (asset_values[0]).lower():
-                                    asset_values[3] = item.partition('=')[2]
-                        return asset_values
-            if int(layer.add_rr) > 0:
-                for key in layer._all_fields['Additional records']:
-                    if 'device-info' in key:
-                        asset_values[4] = layer._all_fields['Additional records'][key]['dns.resp.name'].partition('.')[0]  #Return the name up to the first '.'
-                        asset_values[12] = 80
-                        dns_txt = str(layer._all_fields['Additional records'][key]['dns.txt'])
-                        asset_values = self.parse_model_and_os(asset_values, dns_txt)
-                        
-                        return asset_values
-                    elif 'local: type TXT' in key:
-                        asset_values[4] = layer._all_fields['Additional records'][key]['dns.resp.name'].partition('.')[0]  #Return the name up to the first '.'
-                        asset_values[12] = 80
-                        dns_txt = layer._all_fields['Additional records'][key]['dns.txt']
-                        if type(dns_txt) == list:
-                            for entry in dns_txt:
-                                if 'md=' in entry:
-                                    asset_values = self.parse_model_and_os(asset_values, entry)
-                        else:
-                            if 'md=' in dns_txt:
-                                asset_values = self.parse_model_and_os(asset_values, entry)
-            return asset_values
-        except AttributeError:
-            logger.debug(f'AttributeError for {asset_values[1]} packet from {asset_values[0]}: {e}')
-            return asset_values
-        except TypeError as e:
-            logger.debug(f'TypeError for {asset_values[1]} packet from {asset_values[0]}: {e}')
-            return asset_values
-
-    def parse_mdns_v6(self, packet):
-        mac, ip, vendor = self.parse_mac_ip(packet)
-        asset_values = ['']*11 + ['0']*8      # Create an empty list for potential values
-        
-        if mac is None:
-            return None
-        asset_values[0] = mac
-        asset_values[5] = vendor
-        if ip is not None:
-            asset_values[2] = ip
-        asset_values[1] = 'mDNS'
-        try:
-            layer = packet['mdns']
-            if int(layer.answers) >0:
-                for key in layer._all_fields['Answers']:
-                    ## If an Apple device and an mDNS "device-info" advertisement, parse known attributes of endpoint
-                    # print(key)
-                    if layer._all_fields['Answers'][key]['dns.resp.type'] == '16' and 'device-info' in key:
-                        result = layer._all_fields['Answers'][key]['dns.resp.name'].partition('.')[0]  #Return the name up to the first '.'
-                        if '@' in result:
-                            asset_values[4] = result.partition('@')[2]              #Some TXT records include <mac>@<hostname> format, return only the hostname
-                        else:
-                            asset_values[4] = result
-                        ## TO DO: Evaluate customer choice of hostname record vs device-info record
-                        asset_values[12] = 60                   ## Apple Device-Info fields more readable ('Amy's iPad') but not actual hostname record, 'Amys-iPad'
-                        dns_txt = str(layer._all_fields['Answers'][key]['dns.txt'])
-                        asset_values = self.parse_model_and_os(asset_values, dns_txt)
-                        return asset_values
-                    elif layer._all_fields['Answers'][key]['dns.resp.type'] == '16' and '_raop._tcp' not in layer._all_fields['Answers'][key]['dns.resp.name'] and 'kerberos' not in layer._all_fields['Answers'][key]['dns.resp.name']:
-                        result = layer._all_fields['Answers'][key]['dns.resp.name'].partition('.')[0]
-                        if '@' in result:
-                            asset_values[4] = result.partition('@')[2]              #Some TXT records include <mac>@<hostname> format, return only the hostname
-                        else:
-                            asset_values[4] = result
-                        asset_values[12] = 60
-                        for item in layer._all_fields['Answers'][key]['dns.txt']:
-                            if len(str(item)) == 1:     ## Avoid parsing mDNS record letter by letter
-                                break       
-                            if 'model=' in item or 'modelname=' in item or 'mdl=' in item.lower() or 'md=' in item or 'modelid=' in item or 'usb_MDL=' in item:
-                                asset_values = self.parse_model_and_os(asset_values, item)
-                            elif "name=" in item:
-                                asset_values[4] = item.partition('=')[2]
-                                asset_values[12] = 80
-                            elif 'MFG=' in item or 'manufacturer=' in item:
-                                asset_values[5] = item.partition('=')[2]   ## Return only the value after the '='
-                                asset_values[13] = 50
-                            elif 'UUID=' in item or 'serialNumber=' in item:
-                                asset_values[9] = item.partition('=')[2]
-                                asset_values[17] = 50
-                            elif 'deviceid=' in item and asset_values[0] in item:
-                                #Only store the "deviceid=" value if it is not the MAC address
-                                if str(item.partition('=')[2]).lower() is not (asset_values[0]).lower():
-                                    asset_values[3] = item.partition('=')[2]
-                        # return asset_values
-                    ## If mDNS answer record is a 'A' record
-                    elif layer._all_fields['Answers'][key]['dns.resp.type'] == '1':
-                        asset_values[4] = layer._all_fields['Answers'][key]['dns.resp.name'].partition('.')[0]
-                        asset_values[12] = 80
-                return asset_values
-
-            if int(layer.add_rr) > 0:
-                for key in layer._all_fields['Additional records']:
-                    # print(f"{key} - {str(layer._all_fields['Additional records'][key]['dns.txt'])}")
-                    if 'device-info' in key or 'airplay' in key:
-                        result = layer._all_fields['Additional records'][key]['dns.resp.name'].partition('.')[0]  #Return the name up to the first '.'
-                        if '@' in result:
-                            asset_values[4] = result.partition('@')[2]              #Some TXT records include <mac>@<hostname> format, return only the hostname
-                        else:
-                            asset_values[4] = result
-                        asset_values[12] = 80                                       ## Device info records consistently have hostname accurately represented
-                        dns_txt = str(layer._all_fields['Additional records'][key]['dns.txt'])
-                        asset_values = self.parse_model_and_os(asset_values, dns_txt)
-                        return asset_values
-                    elif 'local: type TXT' in key:
-                        result = layer._all_fields['Additional records'][key]['dns.resp.name'].partition('.')[0]  #Return the name up to the first '.'
-                        asset_values[12] = 60
-                        if '@' in result:
-                            asset_values[4] = result.partition('@')[2]              #Some TXT records include <mac>@<hostname> format, return only the hostname
-                        else:
-                            asset_values[4] = result
-                        dns_txt = layer._all_fields['Additional records'][key]['dns.txt']
-                        if type(dns_txt) == list:
-                            for entry in dns_txt:
-                                if 'md=' in entry:
-                                    asset_values = self.parse_model_and_os(asset_values, entry)
-                        else:
-                            if 'md=' in dns_txt:
-                                asset_values = self.parse_model_and_os(asset_values, entry)
-            return asset_values
-        except AttributeError:
-            logger.debug(f'AttributeError for {asset_values[1]} packet from {asset_values[0]}: {e}')
-            return asset_values
-        except TypeError as e:
-            logger.debug(f'TypeError for {asset_values[1]} packet from {asset_values[0]}: {e}')
-            return asset_values
-
     def parse_mdns_v7(self,packet):
         mac, ip, vendor = self.parse_mac_ip(packet)
         asset_values = ['']*11 + ['0']*8      # Create an empty list for potential values
         
         if mac is None:
             return None
         asset_values[0] = mac
```

### Comparing `pxgrid_pyshark-0.0.8/pxgrid_pyshark.egg-info/PKG-INFO` & `pxgrid_pyshark-0.0.9/pxgrid_pyshark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pxgrid_pyshark
-Version: 0.0.8
+Version: 0.0.9
 Summary: Custom DPI tool used to passively analyze endpoint data and transmit results via Cisco ISE pxGrid messaging for improved endpoint profiling
 Home-page: https://github.com/taylor-cook/pxgrid-pyshark
 Download-URL: https://github.com/taylor-cook/pxgrid-pyshark
 Author: Taylor Cook
 Author-email: aacook@cisco.com
 License: Apache 2.0; Copyright (c) 2024 Cisco and/or its affiliates.
 Keywords: ISE,pxGrid
```

### Comparing `pxgrid_pyshark-0.0.8/pxgrid_pyshark.egg-info/SOURCES.txt` & `pxgrid_pyshark-0.0.9/pxgrid_pyshark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pxgrid_pyshark-0.0.8/setup.py` & `pxgrid_pyshark-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `pxgrid_pyshark-0.0.8/versioneer.py` & `pxgrid_pyshark-0.0.9/versioneer.py`

 * *Files identical despite different names*

