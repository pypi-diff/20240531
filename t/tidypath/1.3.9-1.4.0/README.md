# Comparing `tmp/tidypath-1.3.9.tar.gz` & `tmp/tidypath-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidypath-1.3.9.tar", last modified: Thu May 30 13:41:36 2024, max compression
+gzip compressed data, was "tidypath-1.4.0.tar", last modified: Thu May 30 14:04:46 2024, max compression
```

## Comparing `tidypath-1.3.9.tar` & `tidypath-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-30 13:41:36.139047 tidypath-1.3.9/
--rwxr-xr-x   0 jorgemedina  (1236) users      (100)    35149 2023-09-08 10:22:16.000000 tidypath-1.3.9/LICENSE.md
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3682 2024-05-30 13:41:36.139047 tidypath-1.3.9/PKG-INFO
--rwxr-xr-x   0 jorgemedina  (1236) users      (100)     2804 2023-09-08 10:22:16.000000 tidypath-1.3.9/README.md
--rwxr-xr-x   0 jorgemedina  (1236) users      (100)      106 2024-05-30 13:41:36.143047 tidypath-1.3.9/setup.cfg
--rwxr-xr-x   0 jorgemedina  (1236) users      (100)     1161 2024-05-30 13:41:15.000000 tidypath-1.3.9/setup.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-30 13:41:36.131047 tidypath-1.3.9/tidypath/
--rwxr-xr-x   0 jorgemedina  (1236) users      (100)      371 2023-09-08 10:22:16.000000 tidypath-1.3.9/tidypath/__init__.py
--rwxr-xr-x   0 jorgemedina  (1236) users      (100)     1629 2023-09-08 10:22:16.000000 tidypath-1.3.9/tidypath/_helper.py
--rwxr-xr-x   0 jorgemedina  (1236) users      (100)     4998 2024-04-05 11:52:19.000000 tidypath-1.3.9/tidypath/config.py
--rwxr-xr-x   0 jorgemedina  (1236) users      (100)    14770 2024-05-30 13:41:07.000000 tidypath-1.3.9/tidypath/decorators.py
--rwxr-xr-x   0 jorgemedina  (1236) users      (100)     6165 2023-09-08 10:22:17.000000 tidypath-1.3.9/tidypath/fmt.py
--rwxr-xr-x   0 jorgemedina  (1236) users      (100)     5197 2023-09-08 10:22:17.000000 tidypath-1.3.9/tidypath/inspection.py
--rwxr-xr-x   0 jorgemedina  (1236) users      (100)    14158 2024-04-05 11:52:19.000000 tidypath-1.3.9/tidypath/paths.py
--rwxr-xr-x   0 jorgemedina  (1236) users      (100)     9844 2023-09-08 10:22:17.000000 tidypath-1.3.9/tidypath/storage.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-30 13:41:36.139047 tidypath-1.3.9/tidypath.egg-info/
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3682 2024-05-30 13:41:35.000000 tidypath-1.3.9/tidypath.egg-info/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)      358 2024-05-30 13:41:36.000000 tidypath-1.3.9/tidypath.egg-info/SOURCES.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2024-05-30 13:41:35.000000 tidypath-1.3.9/tidypath.egg-info/dependency_links.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)       63 2024-05-30 13:41:35.000000 tidypath-1.3.9/tidypath.egg-info/requires.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        9 2024-05-30 13:41:35.000000 tidypath-1.3.9/tidypath.egg-info/top_level.txt
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-30 14:04:46.870695 tidypath-1.4.0/
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)    35149 2023-09-08 10:22:16.000000 tidypath-1.4.0/LICENSE.md
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3682 2024-05-30 14:04:46.870695 tidypath-1.4.0/PKG-INFO
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)     2804 2023-09-08 10:22:16.000000 tidypath-1.4.0/README.md
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)      106 2024-05-30 14:04:46.874695 tidypath-1.4.0/setup.cfg
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)     1161 2024-05-30 14:04:17.000000 tidypath-1.4.0/setup.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-30 14:04:46.858695 tidypath-1.4.0/tidypath/
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)      371 2023-09-08 10:22:16.000000 tidypath-1.4.0/tidypath/__init__.py
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)     1629 2023-09-08 10:22:16.000000 tidypath-1.4.0/tidypath/_helper.py
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)     4998 2024-04-05 11:52:19.000000 tidypath-1.4.0/tidypath/config.py
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)    14770 2024-05-30 13:41:07.000000 tidypath-1.4.0/tidypath/decorators.py
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)     6165 2023-09-08 10:22:17.000000 tidypath-1.4.0/tidypath/fmt.py
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)     5197 2023-09-08 10:22:17.000000 tidypath-1.4.0/tidypath/inspection.py
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)    14563 2024-05-30 14:03:40.000000 tidypath-1.4.0/tidypath/paths.py
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)     9844 2023-09-08 10:22:17.000000 tidypath-1.4.0/tidypath/storage.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-30 14:04:46.870695 tidypath-1.4.0/tidypath.egg-info/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3682 2024-05-30 14:04:46.000000 tidypath-1.4.0/tidypath.egg-info/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      358 2024-05-30 14:04:46.000000 tidypath-1.4.0/tidypath.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2024-05-30 14:04:46.000000 tidypath-1.4.0/tidypath.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       63 2024-05-30 14:04:46.000000 tidypath-1.4.0/tidypath.egg-info/requires.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        9 2024-05-30 14:04:46.000000 tidypath-1.4.0/tidypath.egg-info/top_level.txt
```

### Comparing `tidypath-1.3.9/LICENSE.md` & `tidypath-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.9/PKG-INFO` & `tidypath-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypath
-Version: 1.3.9
+Version: 1.4.0
 Summary: Automatically store/load data in a tidy, efficient way.
 Home-page: https://github.com/medinajorge/tidypath
 Download-URL: https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tidypath-1.3.9/README.md` & `tidypath-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.9/setup.py` & `tidypath-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tidypath',
-    version='1.3.9',
+    version='1.4.0',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=['tidypath'],
     url='https://github.com/medinajorge/tidypath',
     download_url='https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz',
     description="Automatically store/load data in a tidy, efficient way.",
     long_description=open('README.md').read(),
```

### Comparing `tidypath-1.3.9/tidypath/_helper.py` & `tidypath-1.4.0/tidypath/_helper.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.9/tidypath/config.py` & `tidypath-1.4.0/tidypath/config.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.9/tidypath/decorators.py` & `tidypath-1.4.0/tidypath/decorators.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.9/tidypath/fmt.py` & `tidypath-1.4.0/tidypath/fmt.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.9/tidypath/inspection.py` & `tidypath-1.4.0/tidypath/inspection.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.9/tidypath/paths.py` & `tidypath-1.4.0/tidypath/paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,22 +74,30 @@
     path = os.path.join(class_tree, func_name)
     return path
 
 def saving_path(Dir, ext, func, keys={}, subfolder="", return_dir=False, funcname_in_filename=False, iterable_maxsize=3, **kwargs):
     """Tree path: Dir -> subfolder -> module -> (classes) -> func_name."""
     func_path = inspect.getabsfile(func).replace('.py', '')
     module_head = func.__module__.split('.')[0]
-    path_split = func_path.split(module_head + '/')
-    parentDir = os.path.join(path_split[0],
-                             Dir,
-                             subfolder,
-                             module_head,
-                             *path_split[1:],
-                             class_path(func=func, **kwargs)
-                             )
+    if module_head == '__main__':
+        parentDir = os.path.join(Dir,
+                                 subfolder,
+                                 module_head,
+                                 class_path(func=func, **kwargs)
+                                 )
+        warnings.warn(f"Module {module_head} is '__main__'. Saving in {parentDir}.", RuntimeWarning)
+    else:
+        path_split = func_path.split(module_head + '/')
+        parentDir = os.path.join(path_split[0],
+                                 Dir,
+                                 subfolder,
+                                 module_head,
+                                 *path_split[1:],
+                                 class_path(func=func, **kwargs)
+                                 )
     Path(parentDir).mkdir(exist_ok=True, parents=True)
     if return_dir:
         return parentDir
     else:
         if funcname_in_filename:
             filename = parentDir.split("/")[-1] + f"_{dict_to_id(keys, iterable_maxsize=iterable_maxsize)}_.{ext}"
         else:
```

### Comparing `tidypath-1.3.9/tidypath/storage.py` & `tidypath-1.4.0/tidypath/storage.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.9/tidypath.egg-info/PKG-INFO` & `tidypath-1.4.0/tidypath.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypath
-Version: 1.3.9
+Version: 1.4.0
 Summary: Automatically store/load data in a tidy, efficient way.
 Home-page: https://github.com/medinajorge/tidypath
 Download-URL: https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

