# Comparing `tmp/simple_space-0.6.0.tar.gz` & `tmp/simple_space-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_space-0.6.0.tar", last modified: Thu May 30 21:32:05 2024, max compression
+gzip compressed data, was "simple_space-0.7.0.tar", last modified: Thu May 30 22:02:32 2024, max compression
```

## Comparing `simple_space-0.6.0.tar` & `simple_space-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 21:32:05.172782 simple_space-0.6.0/
--rw-rw-r--   0 user      (1000) user      (1000)     1062 2024-05-30 00:58:34.000000 simple_space-0.6.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)    11079 2024-05-30 21:32:05.172782 simple_space-0.6.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    10006 2024-05-30 19:17:31.000000 simple_space-0.6.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 21:32:05.168779 simple_space-0.6.0/SimpleS/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 21:32:05.172782 simple_space-0.6.0/SimpleS/ImageRelated/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:36.000000 simple_space-0.6.0/SimpleS/ImageRelated/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     9526 2024-05-30 15:59:18.000000 simple_space-0.6.0/SimpleS/ImageRelated/basics.py
--rw-r--r--   0 user      (1000) user      (1000)     4603 2024-05-30 18:12:49.000000 simple_space-0.6.0/SimpleS/ImageRelated/enhancements.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 21:32:05.172782 simple_space-0.6.0/SimpleS/Points/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:29.000000 simple_space-0.6.0/SimpleS/Points/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     4748 2024-05-30 21:22:31.000000 simple_space-0.6.0/SimpleS/Points/dim2.py
--rw-rw-r--   0 user      (1000) user      (1000)     8666 2024-05-30 21:27:05.000000 simple_space-0.6.0/SimpleS/Points/dim3.py
--rw-rw-r--   0 user      (1000) user      (1000)       47 2024-05-30 21:29:30.000000 simple_space-0.6.0/SimpleS/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1223 2024-05-30 07:41:04.000000 simple_space-0.6.0/SimpleS/utils.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 21:32:05.172782 simple_space-0.6.0/Simple_Space.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)    11079 2024-05-30 21:32:05.000000 simple_space-0.6.0/Simple_Space.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      422 2024-05-30 21:32:05.000000 simple_space-0.6.0/Simple_Space.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-30 21:32:05.000000 simple_space-0.6.0/Simple_Space.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       57 2024-05-30 21:32:05.000000 simple_space-0.6.0/Simple_Space.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        8 2024-05-30 21:32:05.000000 simple_space-0.6.0/Simple_Space.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1082 2024-05-30 21:29:43.000000 simple_space-0.6.0/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-30 21:32:05.172782 simple_space-0.6.0/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 22:02:32.285267 simple_space-0.7.0/
+-rw-rw-r--   0 user      (1000) user      (1000)     1062 2024-05-30 00:58:34.000000 simple_space-0.7.0/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)    11079 2024-05-30 22:02:32.285267 simple_space-0.7.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    10006 2024-05-30 19:17:31.000000 simple_space-0.7.0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 22:02:32.281267 simple_space-0.7.0/SimpleS/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 22:02:32.281267 simple_space-0.7.0/SimpleS/ImageRelated/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:36.000000 simple_space-0.7.0/SimpleS/ImageRelated/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9526 2024-05-30 15:59:18.000000 simple_space-0.7.0/SimpleS/ImageRelated/basics.py
+-rw-r--r--   0 user      (1000) user      (1000)     4603 2024-05-30 18:12:49.000000 simple_space-0.7.0/SimpleS/ImageRelated/enhancements.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 22:02:32.281267 simple_space-0.7.0/SimpleS/Points/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:29.000000 simple_space-0.7.0/SimpleS/Points/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4748 2024-05-30 21:22:31.000000 simple_space-0.7.0/SimpleS/Points/dim2.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8666 2024-05-30 21:27:05.000000 simple_space-0.7.0/SimpleS/Points/dim3.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 22:02:16.000000 simple_space-0.7.0/SimpleS/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1394 2024-05-30 22:02:09.000000 simple_space-0.7.0/SimpleS/utils.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 22:02:32.285267 simple_space-0.7.0/Simple_Space.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)    11079 2024-05-30 22:02:32.000000 simple_space-0.7.0/Simple_Space.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      422 2024-05-30 22:02:32.000000 simple_space-0.7.0/Simple_Space.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-30 22:02:32.000000 simple_space-0.7.0/Simple_Space.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       57 2024-05-30 22:02:32.000000 simple_space-0.7.0/Simple_Space.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        8 2024-05-30 22:02:32.000000 simple_space-0.7.0/Simple_Space.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1082 2024-05-30 22:02:23.000000 simple_space-0.7.0/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-30 22:02:32.285267 simple_space-0.7.0/setup.cfg
```

### Comparing `simple_space-0.6.0/LICENSE` & `simple_space-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_space-0.6.0/PKG-INFO` & `simple_space-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simple-Space
-Version: 0.6.0
+Version: 0.7.0
 Summary: A Try at Better Understanding Space.
 Author-email: Hamed Hajipour <cloner174.org@gmail.com>
 Project-URL: Homepage, https://github.com/cloner174/Simple-Space
 Project-URL: Documentation, https://github.com/cloner174/Simple-Space#readme
 Project-URL: Repository, https://github.com/cloner174/Simple-Space.git
 Project-URL: Issues, https://github.com/cloner174/Simple-Space/issues
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `simple_space-0.6.0/README.md` & `simple_space-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `simple_space-0.6.0/SimpleS/ImageRelated/basics.py` & `simple_space-0.7.0/SimpleS/ImageRelated/basics.py`

 * *Files identical despite different names*

### Comparing `simple_space-0.6.0/SimpleS/ImageRelated/enhancements.py` & `simple_space-0.7.0/SimpleS/ImageRelated/enhancements.py`

 * *Files identical despite different names*

### Comparing `simple_space-0.6.0/SimpleS/Points/dim2.py` & `simple_space-0.7.0/SimpleS/Points/dim2.py`

 * *Files identical despite different names*

### Comparing `simple_space-0.6.0/SimpleS/Points/dim3.py` & `simple_space-0.7.0/SimpleS/Points/dim3.py`

 * *Files identical despite different names*

### Comparing `simple_space-0.6.0/SimpleS/utils.py` & `simple_space-0.7.0/SimpleS/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import datetime
 import os
 
 def save_path_generator(filename = None, path = None, flag = None):
         
         try:
                 if path is not None:
-                        path = path
+                        if not path.endswith('.png') or not path.endswith('.jpg'):
+                                path = path
+                        else:
+                                path = 'results'
                 else:
                         path = 'results'
                 os.makedirs(path,exist_ok=True)
                 if filename is not None:
                         if not filename.endswith('.png') or not filename.endswith('.jpg'):
                                 filename = filename + '.png'
                 else:
@@ -35,8 +38,8 @@
 
 def arr_to_list(arr):
         
         temp = []
         for i, j in arr :
                 temp.append((int(i),int(j)))
         
-        return temp
+        return temp
```

### Comparing `simple_space-0.6.0/Simple_Space.egg-info/PKG-INFO` & `simple_space-0.7.0/Simple_Space.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simple-Space
-Version: 0.6.0
+Version: 0.7.0
 Summary: A Try at Better Understanding Space.
 Author-email: Hamed Hajipour <cloner174.org@gmail.com>
 Project-URL: Homepage, https://github.com/cloner174/Simple-Space
 Project-URL: Documentation, https://github.com/cloner174/Simple-Space#readme
 Project-URL: Repository, https://github.com/cloner174/Simple-Space.git
 Project-URL: Issues, https://github.com/cloner174/Simple-Space/issues
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `simple_space-0.6.0/pyproject.toml` & `simple_space-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Simple-Space"
-version = "0.6.0"
+version = "0.7.0"
 description = "A Try at Better Understanding Space."
 readme = "README.md"
 requires-python = ">=3.6"
 authors = [
     { name = "Hamed Hajipour", email = "cloner174.org@gmail.com" },
 ]
 classifiers = [
```

