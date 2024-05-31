# Comparing `tmp/taguchi-1.0.3.tar.gz` & `tmp/taguchi-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taguchi-1.0.3.tar", last modified: Fri May 17 20:50:28 2024, max compression
+gzip compressed data, was "taguchi-1.0.4.tar", last modified: Fri May 31 01:38:34 2024, max compression
```

## Comparing `taguchi-1.0.3.tar` & `taguchi-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-17 20:50:28.461237 taguchi-1.0.3/
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)       29 2024-05-09 03:46:44.000000 taguchi-1.0.3/MANIFEST.in
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     4216 2024-05-17 20:50:28.461237 taguchi-1.0.3/PKG-INFO
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     3786 2024-05-09 03:35:22.000000 taguchi-1.0.3/README.md
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      103 2024-05-04 04:45:54.000000 taguchi-1.0.3/pyproject.toml
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      757 2024-05-17 20:50:28.462237 taguchi-1.0.3/setup.cfg
-drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-17 20:50:28.458237 taguchi-1.0.3/taguchi/
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)       17 2024-05-17 20:34:26.000000 taguchi-1.0.3/taguchi/__init__.py
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     3329 2024-05-17 20:49:51.000000 taguchi-1.0.3/taguchi/__main__.py
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)   126984 2024-05-17 20:49:28.000000 taguchi-1.0.3/taguchi/database.json
-drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-17 20:50:28.460237 taguchi-1.0.3/taguchi.egg-info/
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     4216 2024-05-17 20:50:28.000000 taguchi-1.0.3/taguchi.egg-info/PKG-INFO
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      296 2024-05-17 20:50:28.000000 taguchi-1.0.3/taguchi.egg-info/SOURCES.txt
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-17 20:50:28.000000 taguchi-1.0.3/taguchi.egg-info/dependency_links.txt
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)       54 2024-05-17 20:50:28.000000 taguchi-1.0.3/taguchi.egg-info/entry_points.txt
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-04 04:46:44.000000 taguchi-1.0.3/taguchi.egg-info/not-zip-safe
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)        8 2024-05-17 20:50:28.000000 taguchi-1.0.3/taguchi.egg-info/top_level.txt
+drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-31 01:38:34.458768 taguchi-1.0.4/
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)       29 2024-05-09 03:46:44.000000 taguchi-1.0.4/MANIFEST.in
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     4216 2024-05-31 01:38:34.457768 taguchi-1.0.4/PKG-INFO
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     3786 2024-05-09 03:35:22.000000 taguchi-1.0.4/README.md
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      103 2024-05-04 04:45:54.000000 taguchi-1.0.4/pyproject.toml
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      757 2024-05-31 01:38:34.458768 taguchi-1.0.4/setup.cfg
+drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-31 01:38:34.457768 taguchi-1.0.4/taguchi/
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)       17 2024-05-31 01:37:40.000000 taguchi-1.0.4/taguchi/__init__.py
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     3329 2024-05-17 20:49:51.000000 taguchi-1.0.4/taguchi/__main__.py
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)   127056 2024-05-31 01:37:34.000000 taguchi-1.0.4/taguchi/database.json
+drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-31 01:38:34.457768 taguchi-1.0.4/taguchi.egg-info/
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     4216 2024-05-31 01:38:34.000000 taguchi-1.0.4/taguchi.egg-info/PKG-INFO
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      296 2024-05-31 01:38:34.000000 taguchi-1.0.4/taguchi.egg-info/SOURCES.txt
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-31 01:38:34.000000 taguchi-1.0.4/taguchi.egg-info/dependency_links.txt
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)       54 2024-05-31 01:38:34.000000 taguchi-1.0.4/taguchi.egg-info/entry_points.txt
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-04 04:46:44.000000 taguchi-1.0.4/taguchi.egg-info/not-zip-safe
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)        8 2024-05-31 01:38:34.000000 taguchi-1.0.4/taguchi.egg-info/top_level.txt
```

### Comparing `taguchi-1.0.3/PKG-INFO` & `taguchi-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taguchi
-Version: 1.0.3
+Version: 1.0.4
 Summary: A tool for optimising systems parameterised by environment variables, based on Taguchi/orthogonal array systems of experiments.
 Home-page: https://github.com/jcranney/taguchi
 Author: Jesse Cranney
 Author-email: jesse.cranney@anu.edu.au
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `taguchi-1.0.3/README.md` & `taguchi-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `taguchi-1.0.3/setup.cfg` & `taguchi-1.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `taguchi-1.0.3/taguchi/__main__.py` & `taguchi-1.0.4/taguchi/__main__.py`

 * *Files identical despite different names*

### Comparing `taguchi-1.0.3/taguchi/database.json` & `taguchi-1.0.4/taguchi/database.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9629629629629629%*

 * *Differences: {"'1,3'": '[[0], [1], [2]]', "'1,4'": '[[0], [1], [2], [3]]', "'1,5'": '[[0], [1], [2], [3], [4]]'}*

```diff
@@ -6,14 +6,56 @@
         [
             0
         ],
         [
             1
         ]
     ],
+    "1,3": [
+        [
+            0
+        ],
+        [
+            1
+        ],
+        [
+            2
+        ]
+    ],
+    "1,4": [
+        [
+            0
+        ],
+        [
+            1
+        ],
+        [
+            2
+        ],
+        [
+            3
+        ]
+    ],
+    "1,5": [
+        [
+            0
+        ],
+        [
+            1
+        ],
+        [
+            2
+        ],
+        [
+            3
+        ],
+        [
+            4
+        ]
+    ],
     "10,2": [
         [
             1,
             0,
             0,
             0,
             1,
```

### Comparing `taguchi-1.0.3/taguchi.egg-info/PKG-INFO` & `taguchi-1.0.4/taguchi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taguchi
-Version: 1.0.3
+Version: 1.0.4
 Summary: A tool for optimising systems parameterised by environment variables, based on Taguchi/orthogonal array systems of experiments.
 Home-page: https://github.com/jcranney/taguchi
 Author: Jesse Cranney
 Author-email: jesse.cranney@anu.edu.au
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

