# Comparing `tmp/comfyui_easynodes-1.0.1.tar.gz` & `tmp/comfyui_easynodes-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comfyui_easynodes-1.0.1.tar", last modified: Fri May 31 00:17:59 2024, max compression
+gzip compressed data, was "comfyui_easynodes-1.0.2.tar", last modified: Fri May 31 00:44:08 2024, max compression
```

## Comparing `comfyui_easynodes-1.0.1.tar` & `comfyui_easynodes-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:17:59.814185 comfyui_easynodes-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:17:59.814185 comfyui_easynodes-1.0.1/ComfyUI_EasyNodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-05-31 00:17:59.000000 comfyui_easynodes-1.0.1/ComfyUI_EasyNodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-31 00:17:59.000000 comfyui_easynodes-1.0.1/ComfyUI_EasyNodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 00:17:59.000000 comfyui_easynodes-1.0.1/ComfyUI_EasyNodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-31 00:17:59.000000 comfyui_easynodes-1.0.1/ComfyUI_EasyNodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 00:17:59.000000 comfyui_easynodes-1.0.1/ComfyUI_EasyNodes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-31 00:17:42.000000 comfyui_easynodes-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-05-31 00:17:59.814185 comfyui_easynodes-1.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:17:59.814185 comfyui_easynodes-1.0.1/easy_nodes/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-31 00:17:42.000000 comfyui_easynodes-1.0.1/easy_nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-31 00:17:42.000000 comfyui_easynodes-1.0.1/easy_nodes/config_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    50046 2024-05-31 00:17:42.000000 comfyui_easynodes-1.0.1/easy_nodes/easy_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    22501 2024-05-31 00:17:42.000000 comfyui_easynodes-1.0.1/easy_nodes/llm_debugging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-31 00:17:42.000000 comfyui_easynodes-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     9452 2024-05-31 00:17:42.000000 comfyui_easynodes-1.0.1/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 00:17:59.814185 comfyui_easynodes-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:44:08.575278 comfyui_easynodes-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:44:08.575278 comfyui_easynodes-1.0.2/ComfyUI_EasyNodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-05-31 00:44:08.000000 comfyui_easynodes-1.0.2/ComfyUI_EasyNodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-31 00:44:08.000000 comfyui_easynodes-1.0.2/ComfyUI_EasyNodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 00:44:08.000000 comfyui_easynodes-1.0.2/ComfyUI_EasyNodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-31 00:44:08.000000 comfyui_easynodes-1.0.2/ComfyUI_EasyNodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 00:44:08.000000 comfyui_easynodes-1.0.2/ComfyUI_EasyNodes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-31 00:43:55.000000 comfyui_easynodes-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-05-31 00:44:08.575278 comfyui_easynodes-1.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:44:08.575278 comfyui_easynodes-1.0.2/easy_nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-31 00:43:55.000000 comfyui_easynodes-1.0.2/easy_nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-31 00:43:55.000000 comfyui_easynodes-1.0.2/easy_nodes/config_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50014 2024-05-31 00:43:55.000000 comfyui_easynodes-1.0.2/easy_nodes/easy_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22501 2024-05-31 00:43:55.000000 comfyui_easynodes-1.0.2/easy_nodes/llm_debugging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-31 00:43:55.000000 comfyui_easynodes-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     9452 2024-05-31 00:43:55.000000 comfyui_easynodes-1.0.2/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 00:44:08.575278 comfyui_easynodes-1.0.2/setup.cfg
```

### Comparing `comfyui_easynodes-1.0.1/ComfyUI_EasyNodes.egg-info/PKG-INFO` & `comfyui_easynodes-1.0.2/ComfyUI_EasyNodes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ComfyUI-EasyNodes
-Version: 1.0.1
+Version: 1.0.2
 Summary: Makes creating new nodes for ComfyUI a breeze.
 Author-email: Andrew Harp <andrew.harp@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Harp
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `comfyui_easynodes-1.0.1/LICENSE` & `comfyui_easynodes-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `comfyui_easynodes-1.0.1/PKG-INFO` & `comfyui_easynodes-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ComfyUI-EasyNodes
-Version: 1.0.1
+Version: 1.0.2
 Summary: Makes creating new nodes for ComfyUI a breeze.
 Author-email: Andrew Harp <andrew.harp@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Harp
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `comfyui_easynodes-1.0.1/easy_nodes/config_service.py` & `comfyui_easynodes-1.0.2/easy_nodes/config_service.py`

 * *Files identical despite different names*

### Comparing `comfyui_easynodes-1.0.1/easy_nodes/easy_nodes.py` & `comfyui_easynodes-1.0.2/easy_nodes/easy_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,20 +26,19 @@
 from PIL import Image
 
 import easy_nodes.config_service as config_service
 import easy_nodes.llm_debugging as llm_debugging
 
 
 # Export the web directory so ComfyUI can pick up the JavaScript.
-_web_path = os.path.join(os.path.dirname(__file__), "..", "web")
-
+_web_path = os.path.join(os.path.dirname(__file__), "web")
 
 if os.path.exists(_web_path):
     comfyui_nodes.EXTENSION_WEB_DIRS["ComfyUI-EasyNodes"] = _web_path
-    logging.info(f"Registered ComfyUI-EasyNodes web directory: '{_web_path}'")
+    logging.debug(f"Registered ComfyUI-EasyNodes web directory: '{_web_path}'")
 else:
     logging.warning(f"ComfyUI-EasyNodes: Web directory not found at {_web_path}. Some features may not be available.")
 
 
 class AutoDescriptionMode(Enum):
     NONE = "none"
     BRIEF = "brief"
@@ -81,28 +80,27 @@
         verify_tensors (bool, optional): Whether to verify tensors for shape and data type according to ComfyUI type (MASK, IMAGE, etc). Runs on inputs and outputs. Defaults to False.
         auto_move_tensors (bool, optional): Whether to automatically move torch Tensors to the GPU before your function gets called, and then to the CPU on output. Defaults to False.
     """
     global _current_config
     if _current_config and _current_config.num_registered == 0:
         logging.warning("Re-initializing EasyNodes, but no Nodes have been registered since last initialization. This may indicate an issue.")
 
-    logging.info("Initializing EasyNodes.")
+    logging.info(f"Initializing EasyNodes. Auto-registration: {auto_register}")
         
     _current_config = dataclasses.replace(_easy_nodes_config)
     _current_config.default_category = default_category
     _current_config.auto_register = auto_register
     _current_config.docstring_mode = docstring_mode
     _current_config.verify_tensors = verify_tensors
     _current_config.auto_move_tensors = auto_move_tensors
 
     if auto_register:
         _current_config.NODE_CLASS_MAPPINGS = comfyui_nodes.NODE_CLASS_MAPPINGS
         _current_config.NODE_DISPLAY_NAME_MAPPINGS = comfyui_nodes.NODE_DISPLAY_NAME_MAPPINGS
         frame = sys._getframe(1).f_globals['__name__']
-        logging.info(f"Auto-registering nodes for {frame}")
         _ensure_package_dicts_exist(frame)
     else:
         _current_config.NODE_CLASS_MAPPINGS = {}
         _current_config.NODE_DISPLAY_NAME_MAPPINGS = {}
 
 
 def get_node_mappings():
```

### Comparing `comfyui_easynodes-1.0.1/easy_nodes/llm_debugging.py` & `comfyui_easynodes-1.0.2/easy_nodes/llm_debugging.py`

 * *Files identical despite different names*

### Comparing `comfyui_easynodes-1.0.1/pyproject.toml` & `comfyui_easynodes-1.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ComfyUI-EasyNodes"
-version = "1.0.1"
+version = "1.0.2"
 description = "Makes creating new nodes for ComfyUI a breeze."
 readme = "readme.md"
 authors = [{ name = "Andrew Harp", email = "andrew.harp@gmail.com" }]
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
 dependencies = [
     "torch",
@@ -24,15 +24,15 @@
 "Source" = "https://github.com/andrewharp/ComfyUI-EasyNodes/"
 
 [tool.setuptools]
 packages = ["easy_nodes"]
 
 [tool.poetry]
 name = "ComfyUI-EasyNodes"
-version = "1.0.1"
+version = "1.0.2"
 description = "Makes creating new nodes for ComfyUI a breeze."
 authors = ["Andrew Harp <andrew.harp@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/andrewharp/ComfyUI-EasyNodes"
 repository = "https://github.com/andrewharp/ComfyUI-EasyNodes"
 documentation = "https://github.com/andrewharp/ComfyUI-EasyNodes"
 readme = "readme.md"
```

### Comparing `comfyui_easynodes-1.0.1/readme.md` & `comfyui_easynodes-1.0.2/readme.md`

 * *Files identical despite different names*

