# Comparing `tmp/comfyui_easynodes-1.0.0.tar.gz` & `tmp/comfyui_easynodes-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comfyui_easynodes-1.0.0.tar", last modified: Fri May 31 00:04:10 2024, max compression
+gzip compressed data, was "comfyui_easynodes-1.0.1.tar", last modified: Fri May 31 00:17:59 2024, max compression
```

## Comparing `comfyui_easynodes-1.0.0.tar` & `comfyui_easynodes-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:04:10.964366 comfyui_easynodes-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:04:10.964366 comfyui_easynodes-1.0.0/ComfyUI_EasyNodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-05-31 00:04:10.000000 comfyui_easynodes-1.0.0/ComfyUI_EasyNodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-31 00:04:10.000000 comfyui_easynodes-1.0.0/ComfyUI_EasyNodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 00:04:10.000000 comfyui_easynodes-1.0.0/ComfyUI_EasyNodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-31 00:04:10.000000 comfyui_easynodes-1.0.0/ComfyUI_EasyNodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 00:04:10.000000 comfyui_easynodes-1.0.0/ComfyUI_EasyNodes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-31 00:03:54.000000 comfyui_easynodes-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-05-31 00:04:10.964366 comfyui_easynodes-1.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:04:10.964366 comfyui_easynodes-1.0.0/easy_nodes/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-31 00:03:54.000000 comfyui_easynodes-1.0.0/easy_nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-31 00:03:54.000000 comfyui_easynodes-1.0.0/easy_nodes/config_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    50046 2024-05-31 00:03:54.000000 comfyui_easynodes-1.0.0/easy_nodes/easy_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    22501 2024-05-31 00:03:54.000000 comfyui_easynodes-1.0.0/easy_nodes/llm_debugging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-31 00:03:54.000000 comfyui_easynodes-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     9452 2024-05-31 00:03:54.000000 comfyui_easynodes-1.0.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 00:04:10.964366 comfyui_easynodes-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:17:59.814185 comfyui_easynodes-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:17:59.814185 comfyui_easynodes-1.0.1/ComfyUI_EasyNodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-05-31 00:17:59.000000 comfyui_easynodes-1.0.1/ComfyUI_EasyNodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-31 00:17:59.000000 comfyui_easynodes-1.0.1/ComfyUI_EasyNodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 00:17:59.000000 comfyui_easynodes-1.0.1/ComfyUI_EasyNodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-31 00:17:59.000000 comfyui_easynodes-1.0.1/ComfyUI_EasyNodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 00:17:59.000000 comfyui_easynodes-1.0.1/ComfyUI_EasyNodes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-31 00:17:42.000000 comfyui_easynodes-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-05-31 00:17:59.814185 comfyui_easynodes-1.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:17:59.814185 comfyui_easynodes-1.0.1/easy_nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-31 00:17:42.000000 comfyui_easynodes-1.0.1/easy_nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-31 00:17:42.000000 comfyui_easynodes-1.0.1/easy_nodes/config_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50046 2024-05-31 00:17:42.000000 comfyui_easynodes-1.0.1/easy_nodes/easy_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22501 2024-05-31 00:17:42.000000 comfyui_easynodes-1.0.1/easy_nodes/llm_debugging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-31 00:17:42.000000 comfyui_easynodes-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     9452 2024-05-31 00:17:42.000000 comfyui_easynodes-1.0.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 00:17:59.814185 comfyui_easynodes-1.0.1/setup.cfg
```

### Comparing `comfyui_easynodes-1.0.0/ComfyUI_EasyNodes.egg-info/PKG-INFO` & `comfyui_easynodes-1.0.1/ComfyUI_EasyNodes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ComfyUI-EasyNodes
-Version: 1.0.0
+Version: 1.0.1
 Summary: Makes creating new nodes for ComfyUI a breeze.
 Author-email: Andrew Harp <andrew.harp@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Harp
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `comfyui_easynodes-1.0.0/LICENSE` & `comfyui_easynodes-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `comfyui_easynodes-1.0.0/PKG-INFO` & `comfyui_easynodes-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ComfyUI-EasyNodes
-Version: 1.0.0
+Version: 1.0.1
 Summary: Makes creating new nodes for ComfyUI a breeze.
 Author-email: Andrew Harp <andrew.harp@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Harp
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `comfyui_easynodes-1.0.0/easy_nodes/config_service.py` & `comfyui_easynodes-1.0.1/easy_nodes/config_service.py`

 * *Files identical despite different names*

### Comparing `comfyui_easynodes-1.0.0/easy_nodes/easy_nodes.py` & `comfyui_easynodes-1.0.1/easy_nodes/easy_nodes.py`

 * *Files identical despite different names*

### Comparing `comfyui_easynodes-1.0.0/easy_nodes/llm_debugging.py` & `comfyui_easynodes-1.0.1/easy_nodes/llm_debugging.py`

 * *Files identical despite different names*

### Comparing `comfyui_easynodes-1.0.0/pyproject.toml` & `comfyui_easynodes-1.0.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ComfyUI-EasyNodes"
-version = "1.0.0"
+version = "1.0.1"
 description = "Makes creating new nodes for ComfyUI a breeze."
 readme = "readme.md"
 authors = [{ name = "Andrew Harp", email = "andrew.harp@gmail.com" }]
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
 dependencies = [
     "torch",
@@ -24,22 +24,23 @@
 "Source" = "https://github.com/andrewharp/ComfyUI-EasyNodes/"
 
 [tool.setuptools]
 packages = ["easy_nodes"]
 
 [tool.poetry]
 name = "ComfyUI-EasyNodes"
-version = "1.0.0"
+version = "1.0.1"
 description = "Makes creating new nodes for ComfyUI a breeze."
 authors = ["Andrew Harp <andrew.harp@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/andrewharp/ComfyUI-EasyNodes"
 repository = "https://github.com/andrewharp/ComfyUI-EasyNodes"
 documentation = "https://github.com/andrewharp/ComfyUI-EasyNodes"
 readme = "readme.md"
+include = ["web/**/*"]
 
 [tool.poetry.dependencies]
 python = ">=3.10"
 torch = "*"
 pillow = "*"
 colorama = "*"
 numpy = "*"
```

### Comparing `comfyui_easynodes-1.0.0/readme.md` & `comfyui_easynodes-1.0.1/readme.md`

 * *Files identical despite different names*

