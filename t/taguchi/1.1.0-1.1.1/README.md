# Comparing `tmp/taguchi-1.1.0.tar.gz` & `tmp/taguchi-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taguchi-1.1.0.tar", last modified: Fri May 31 02:03:45 2024, max compression
+gzip compressed data, was "taguchi-1.1.1.tar", last modified: Fri May 31 02:08:49 2024, max compression
```

## Comparing `taguchi-1.1.0.tar` & `taguchi-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-31 02:03:45.225072 taguchi-1.1.0/
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)       29 2024-05-09 03:46:44.000000 taguchi-1.1.0/MANIFEST.in
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     4596 2024-05-31 02:03:45.225072 taguchi-1.1.0/PKG-INFO
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     4166 2024-05-31 02:03:14.000000 taguchi-1.1.0/README.md
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      103 2024-05-04 04:45:54.000000 taguchi-1.1.0/pyproject.toml
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      757 2024-05-31 02:03:45.226072 taguchi-1.1.0/setup.cfg
-drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-31 02:03:45.220072 taguchi-1.1.0/taguchi/
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)       17 2024-05-31 01:58:54.000000 taguchi-1.1.0/taguchi/__init__.py
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     3572 2024-05-31 01:57:39.000000 taguchi-1.1.0/taguchi/__main__.py
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)   127056 2024-05-31 01:37:34.000000 taguchi-1.1.0/taguchi/database.json
-drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-31 02:03:45.224072 taguchi-1.1.0/taguchi.egg-info/
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     4596 2024-05-31 02:03:45.000000 taguchi-1.1.0/taguchi.egg-info/PKG-INFO
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      296 2024-05-31 02:03:45.000000 taguchi-1.1.0/taguchi.egg-info/SOURCES.txt
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-31 02:03:45.000000 taguchi-1.1.0/taguchi.egg-info/dependency_links.txt
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)       54 2024-05-31 02:03:45.000000 taguchi-1.1.0/taguchi.egg-info/entry_points.txt
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-04 04:46:44.000000 taguchi-1.1.0/taguchi.egg-info/not-zip-safe
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)        8 2024-05-31 02:03:45.000000 taguchi-1.1.0/taguchi.egg-info/top_level.txt
+drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-31 02:08:49.943220 taguchi-1.1.1/
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)       29 2024-05-09 03:46:44.000000 taguchi-1.1.1/MANIFEST.in
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     4596 2024-05-31 02:08:49.942220 taguchi-1.1.1/PKG-INFO
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     4166 2024-05-31 02:03:14.000000 taguchi-1.1.1/README.md
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      103 2024-05-04 04:45:54.000000 taguchi-1.1.1/pyproject.toml
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      757 2024-05-31 02:08:49.943220 taguchi-1.1.1/setup.cfg
+drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-31 02:08:49.941220 taguchi-1.1.1/taguchi/
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)       17 2024-05-31 02:08:10.000000 taguchi-1.1.1/taguchi/__init__.py
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     3582 2024-05-31 02:07:58.000000 taguchi-1.1.1/taguchi/__main__.py
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)   127056 2024-05-31 01:37:34.000000 taguchi-1.1.1/taguchi/database.json
+drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-31 02:08:49.942220 taguchi-1.1.1/taguchi.egg-info/
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     4596 2024-05-31 02:08:49.000000 taguchi-1.1.1/taguchi.egg-info/PKG-INFO
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      296 2024-05-31 02:08:49.000000 taguchi-1.1.1/taguchi.egg-info/SOURCES.txt
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-31 02:08:49.000000 taguchi-1.1.1/taguchi.egg-info/dependency_links.txt
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)       54 2024-05-31 02:08:49.000000 taguchi-1.1.1/taguchi.egg-info/entry_points.txt
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-04 04:46:44.000000 taguchi-1.1.1/taguchi.egg-info/not-zip-safe
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)        8 2024-05-31 02:08:49.000000 taguchi-1.1.1/taguchi.egg-info/top_level.txt
```

### Comparing `taguchi-1.1.0/PKG-INFO` & `taguchi-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taguchi
-Version: 1.1.0
+Version: 1.1.1
 Summary: A tool for optimising systems parameterised by environment variables, based on Taguchi/orthogonal array systems of experiments.
 Home-page: https://github.com/jcranney/taguchi
 Author: Jesse Cranney
 Author-email: jesse.cranney@anu.edu.au
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `taguchi-1.1.0/README.md` & `taguchi-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `taguchi-1.1.0/setup.cfg` & `taguchi-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `taguchi-1.1.0/taguchi/__main__.py` & `taguchi-1.1.1/taguchi/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 
 results = []
 for experiment in array:
     for param,state in zip(params,experiment):
         os.environ[param] = str(a[param][state])
         if verbose:
-            print(param,state)
+            print(param,a[param][state])
     proc = subprocess.Popen(command, stdout=subprocess.PIPE, shell=True)
     (out, err) = proc.communicate()
     if err is not None:
         print(err.decode())
         exit(1)
     if verbose > 1:
         print(out.decode())
```

### Comparing `taguchi-1.1.0/taguchi/database.json` & `taguchi-1.1.1/taguchi/database.json`

 * *Files identical despite different names*

### Comparing `taguchi-1.1.0/taguchi.egg-info/PKG-INFO` & `taguchi-1.1.1/taguchi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taguchi
-Version: 1.1.0
+Version: 1.1.1
 Summary: A tool for optimising systems parameterised by environment variables, based on Taguchi/orthogonal array systems of experiments.
 Home-page: https://github.com/jcranney/taguchi
 Author: Jesse Cranney
 Author-email: jesse.cranney@anu.edu.au
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

