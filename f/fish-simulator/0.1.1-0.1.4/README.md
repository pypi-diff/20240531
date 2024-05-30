# Comparing `tmp/fish_simulator-0.1.1.tar.gz` & `tmp/fish_simulator-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fish_simulator-0.1.1.tar", last modified: Thu May 30 21:19:16 2024, max compression
+gzip compressed data, was "fish_simulator-0.1.4.tar", last modified: Thu May 30 22:36:41 2024, max compression
```

## Comparing `fish_simulator-0.1.1.tar` & `fish_simulator-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:19:16.118037 fish_simulator-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-30 21:19:09.000000 fish_simulator-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-05-30 21:19:16.118037 fish_simulator-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-30 21:19:09.000000 fish_simulator-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:19:16.114037 fish_simulator-0.1.1/fish_simulator/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 21:19:09.000000 fish_simulator-0.1.1/fish_simulator/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-30 21:19:09.000000 fish_simulator-0.1.1/fish_simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-30 21:19:09.000000 fish_simulator-0.1.1/fish_simulator/image_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    17595 2024-05-30 21:19:09.000000 fish_simulator-0.1.1/fish_simulator/simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-30 21:19:09.000000 fish_simulator-0.1.1/fish_simulator/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-30 21:19:09.000000 fish_simulator-0.1.1/fish_simulator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:19:16.118037 fish_simulator-0.1.1/fish_simulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-05-30 21:19:16.000000 fish_simulator-0.1.1/fish_simulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-30 21:19:16.000000 fish_simulator-0.1.1/fish_simulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 21:19:16.000000 fish_simulator-0.1.1/fish_simulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-30 21:19:16.000000 fish_simulator-0.1.1/fish_simulator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-30 21:19:16.000000 fish_simulator-0.1.1/fish_simulator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-30 21:19:09.000000 fish_simulator-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-30 21:19:09.000000 fish_simulator-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 21:19:16.118037 fish_simulator-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:19:16.114037 fish_simulator-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-30 21:19:09.000000 fish_simulator-0.1.1/test/test_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:36:41.094200 fish_simulator-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-30 22:36:34.000000 fish_simulator-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-05-30 22:36:41.094200 fish_simulator-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-30 22:36:34.000000 fish_simulator-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:36:41.090200 fish_simulator-0.1.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:36:34.000000 fish_simulator-0.1.4/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:36:41.090200 fish_simulator-0.1.4/fish_simulator/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 22:36:34.000000 fish_simulator-0.1.4/fish_simulator/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-30 22:36:34.000000 fish_simulator-0.1.4/fish_simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-30 22:36:34.000000 fish_simulator-0.1.4/fish_simulator/image_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17595 2024-05-30 22:36:34.000000 fish_simulator-0.1.4/fish_simulator/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:36:41.094200 fish_simulator-0.1.4/fish_simulator/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:36:34.000000 fish_simulator-0.1.4/fish_simulator/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:36:41.094200 fish_simulator-0.1.4/fish_simulator/templates/template_img/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:36:34.000000 fish_simulator-0.1.4/fish_simulator/templates/template_img/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:36:41.094200 fish_simulator-0.1.4/fish_simulator/templates/template_img/segs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:36:34.000000 fish_simulator-0.1.4/fish_simulator/templates/template_img/segs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-30 22:36:34.000000 fish_simulator-0.1.4/fish_simulator/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-30 22:36:34.000000 fish_simulator-0.1.4/fish_simulator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:36:41.094200 fish_simulator-0.1.4/fish_simulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-05-30 22:36:41.000000 fish_simulator-0.1.4/fish_simulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-30 22:36:41.000000 fish_simulator-0.1.4/fish_simulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 22:36:41.000000 fish_simulator-0.1.4/fish_simulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-30 22:36:41.000000 fish_simulator-0.1.4/fish_simulator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-30 22:36:41.000000 fish_simulator-0.1.4/fish_simulator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-30 22:36:34.000000 fish_simulator-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-30 22:36:34.000000 fish_simulator-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 22:36:41.094200 fish_simulator-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:36:41.094200 fish_simulator-0.1.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:36:34.000000 fish_simulator-0.1.4/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:36:41.094200 fish_simulator-0.1.4/test/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:36:34.000000 fish_simulator-0.1.4/test/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-30 22:36:34.000000 fish_simulator-0.1.4/test/test_methods.py
```

### Comparing `fish_simulator-0.1.1/LICENSE` & `fish_simulator-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.1/PKG-INFO` & `fish_simulator-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fish_simulator
-Version: 0.1.1
+Version: 0.1.4
 Summary: Simulate zebrafish swim from tail angle tracking data
 Author-email: Thomas Soares Mullen <thomasmullen96@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Thomas Soares Mullen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fish_simulator-0.1.1/README.md` & `fish_simulator-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.1/fish_simulator/image_loader.py` & `fish_simulator-0.1.4/fish_simulator/image_loader.py`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.1/fish_simulator/simulator.py` & `fish_simulator-0.1.4/fish_simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.1/fish_simulator/transforms.py` & `fish_simulator-0.1.4/fish_simulator/transforms.py`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.1/fish_simulator/utils.py` & `fish_simulator-0.1.4/fish_simulator/utils.py`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.1/fish_simulator.egg-info/PKG-INFO` & `fish_simulator-0.1.4/fish_simulator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fish_simulator
-Version: 0.1.1
+Version: 0.1.4
 Summary: Simulate zebrafish swim from tail angle tracking data
 Author-email: Thomas Soares Mullen <thomasmullen96@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Thomas Soares Mullen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fish_simulator-0.1.1/pyproject.toml` & `fish_simulator-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3 :: Only",
 ]
 
 [tool.setuptools]
-#packages = ["fish_simulator", "test"]
+#packages = ["fish_simulator", "fish_simulator.templates", "test"]
 #package-dir = {"" = "fish_simulator"}
 
 [tool.setuptools.packages]
 find = {}
 
 [tool.setuptools.dynamic]
 version = {file = "fish_simulator/VERSION"}
```

### Comparing `fish_simulator-0.1.1/test/test_methods.py` & `fish_simulator-0.1.4/test/test_methods.py`

 * *Files identical despite different names*

