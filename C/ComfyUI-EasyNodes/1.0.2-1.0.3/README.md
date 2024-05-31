# Comparing `tmp/comfyui_easynodes-1.0.2.tar.gz` & `tmp/comfyui_easynodes-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comfyui_easynodes-1.0.2.tar", last modified: Fri May 31 00:44:08 2024, max compression
+gzip compressed data, was "comfyui_easynodes-1.0.3.tar", last modified: Fri May 31 03:01:04 2024, max compression
```

## Comparing `comfyui_easynodes-1.0.2.tar` & `comfyui_easynodes-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:44:08.575278 comfyui_easynodes-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:44:08.575278 comfyui_easynodes-1.0.2/ComfyUI_EasyNodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-05-31 00:44:08.000000 comfyui_easynodes-1.0.2/ComfyUI_EasyNodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-31 00:44:08.000000 comfyui_easynodes-1.0.2/ComfyUI_EasyNodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 00:44:08.000000 comfyui_easynodes-1.0.2/ComfyUI_EasyNodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-31 00:44:08.000000 comfyui_easynodes-1.0.2/ComfyUI_EasyNodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 00:44:08.000000 comfyui_easynodes-1.0.2/ComfyUI_EasyNodes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-31 00:43:55.000000 comfyui_easynodes-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-05-31 00:44:08.575278 comfyui_easynodes-1.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:44:08.575278 comfyui_easynodes-1.0.2/easy_nodes/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-31 00:43:55.000000 comfyui_easynodes-1.0.2/easy_nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-31 00:43:55.000000 comfyui_easynodes-1.0.2/easy_nodes/config_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    50014 2024-05-31 00:43:55.000000 comfyui_easynodes-1.0.2/easy_nodes/easy_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    22501 2024-05-31 00:43:55.000000 comfyui_easynodes-1.0.2/easy_nodes/llm_debugging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-31 00:43:55.000000 comfyui_easynodes-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     9452 2024-05-31 00:43:55.000000 comfyui_easynodes-1.0.2/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 00:44:08.575278 comfyui_easynodes-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:01:04.394346 comfyui_easynodes-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:01:04.394346 comfyui_easynodes-1.0.3/ComfyUI_EasyNodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12018 2024-05-31 03:01:04.000000 comfyui_easynodes-1.0.3/ComfyUI_EasyNodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-31 03:01:04.000000 comfyui_easynodes-1.0.3/ComfyUI_EasyNodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 03:01:04.000000 comfyui_easynodes-1.0.3/ComfyUI_EasyNodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-31 03:01:04.000000 comfyui_easynodes-1.0.3/ComfyUI_EasyNodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 03:01:04.000000 comfyui_easynodes-1.0.3/ComfyUI_EasyNodes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-31 03:00:55.000000 comfyui_easynodes-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-31 03:00:55.000000 comfyui_easynodes-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12018 2024-05-31 03:01:04.394346 comfyui_easynodes-1.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:01:04.394346 comfyui_easynodes-1.0.3/easy_nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-31 03:00:55.000000 comfyui_easynodes-1.0.3/easy_nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-31 03:00:55.000000 comfyui_easynodes-1.0.3/easy_nodes/config_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50014 2024-05-31 03:00:55.000000 comfyui_easynodes-1.0.3/easy_nodes/easy_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22501 2024-05-31 03:00:55.000000 comfyui_easynodes-1.0.3/easy_nodes/llm_debugging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:01:04.394346 comfyui_easynodes-1.0.3/easy_nodes/web/
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-31 03:00:55.000000 comfyui_easynodes-1.0.3/easy_nodes/web/config_service.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9407 2024-05-31 03:00:55.000000 comfyui_easynodes-1.0.3/easy_nodes/web/easy_nodes.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-31 03:00:55.000000 comfyui_easynodes-1.0.3/easy_nodes/web/llm_debugging.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-31 03:00:55.000000 comfyui_easynodes-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-05-31 03:00:55.000000 comfyui_easynodes-1.0.3/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 03:01:04.394346 comfyui_easynodes-1.0.3/setup.cfg
```

### Comparing `comfyui_easynodes-1.0.2/ComfyUI_EasyNodes.egg-info/PKG-INFO` & `comfyui_easynodes-1.0.3/ComfyUI_EasyNodes.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ComfyUI-EasyNodes
-Version: 1.0.2
+Version: 1.0.3
 Summary: Makes creating new nodes for ComfyUI a breeze.
 Author-email: Andrew Harp <andrew.harp@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Harp
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -53,28 +53,35 @@
     """Returns separate masks for values above and below the threshold value."""
     mask_below = torch.any(image < threshold_value, dim=-1)
     return mask_below.float(), (~mask_below).float()
 ```
 
 That's it! Now your node is ready for ComfyUI. More examples can be found [here](example/example_nodes.py).
 
+Sample node with tooltip and deep source link:
+
 <img src="assets/threshold_example.png" alt="The new node with tooltip" width="50%">
 
+New settings:
+
+<img src="assets/menu_options.png" alt="New menu options" width="50%">
+
 
 Note that ImageTensor/MaskTensor are just syntactic sugar for semantically differentiating the annotations (allowing ComfyUI to know what plugs into what); your function will still get passed genunine torch.Tensor objects.
 
 For more control, you can call easy_nodes.init(...) and change some settings that will apply to all nodes you create.
 
 ## New in 1.0.0:
 
 - Renamed to ComfyUI-EasyNodes (from ComfyUI-Annotations) to better reflect the package's goal (rather than the means)
 - Automatic module reloading: if you edit your node source, immediately see the changes
 - LLM-based debugging: optionally have ChatGPT take a crack at fixing your code
 - Set node colors via Python argument (no JavaScript required)
 - Add preview text and images to nodes via show_text and show_image Python functions, no JavaScript required.
+- Automatically create nodes with widgets to set the fields of existing Python objects.
 - Tooltips and deep links to node source code
 - Bug fixes
 
 ## Features
 
 - **@ComfyNode Decorator**: Simplifies the declaration of custom nodes with automagic node declaration based on Python type annotations. Existing Python functions can be converted to ComfyUI nodes with a simple "@ComfyNode()"
 - **Built-in text and image previews**: Just call `easy_nodes.add_preview_text()` and `easy_nodes.add_preview_image()` in the body of your function and EasyNodes will automatically display it, no JavaScript hacking required.
@@ -92,20 +99,27 @@
 To use this module in your ComfyUI project, follow these steps:
 
 1. **Install the Module**: Run the following command to install the ComfyUI-EasyNodes module:
 
     ```bash
     pip install ComfyUI-EasyNodes
     ```
-    or
-    ```
+    or, if you want to have an editable version:
+    ```bash
     pip install -e https://github.com/andrewharp/ComfyUI-EasyNodes
     ```
+    Note that this is not a typical ComfyUI nodepack, so does not itself live under custom_nodes.
+    
+    However, after installing you can copy the example node directory into custom_nodes to test them out:
+    ```bash
+    git clone --depth=1 https://github.com/andrewharp/ComfyUI-EasyNodes.git /tmp/easynodes
+    mv /tmp/easynodes/example $COMFYUI_DIR/custom_nodes/easynodes
+    ```
 
-2. **Integrate into Your Project**:
+3. **Integrate into Your Project**:
     - Open your ComfyUI project's `__init__.py` (e.g. `ComfyUI/custom_nodes/my_project/__init__.py`).
     - Make sure you're importing the module where you define your nodes:
 
     ```python
     import your_node_module
     ```
 
@@ -117,15 +131,15 @@
 
     @ComfyNode()
     def create_random_image(width: int=NumberInput(128, 128, 1024), 
                             height: int=NumberInput(128, 128, 1024)) -> ImageTensor:
         return torch.rand((1, height, width, 3))
     ```
 
-    If you run into problems with the auto-registration, you can try turning it off give ComfyUI your node mappings the regular way:
+    If you run into problems with the auto-registration, you can try turning it off and give ComfyUI your node mappings the regular way:
     <details>
 
     In `__init__.py`:
 
     ```python
     import easy_nodes
     import your_node_module
@@ -137,14 +151,17 @@
     ```
 
     and in `your_node_module.py`:
     ```python
     import easy_nodes
     easy_nodes.initialize_easy_nodes(default_category=my_category, auto_register=False)
 
+    @ComfyNode()
+    def my_node(foo: int) -> int:
+        return foo + 42
     ...
     ```
 
     </details>
 
 ## Usage
```

### Comparing `comfyui_easynodes-1.0.2/LICENSE` & `comfyui_easynodes-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `comfyui_easynodes-1.0.2/PKG-INFO` & `comfyui_easynodes-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ComfyUI-EasyNodes
-Version: 1.0.2
+Version: 1.0.3
 Summary: Makes creating new nodes for ComfyUI a breeze.
 Author-email: Andrew Harp <andrew.harp@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Harp
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -53,28 +53,35 @@
     """Returns separate masks for values above and below the threshold value."""
     mask_below = torch.any(image < threshold_value, dim=-1)
     return mask_below.float(), (~mask_below).float()
 ```
 
 That's it! Now your node is ready for ComfyUI. More examples can be found [here](example/example_nodes.py).
 
+Sample node with tooltip and deep source link:
+
 <img src="assets/threshold_example.png" alt="The new node with tooltip" width="50%">
 
+New settings:
+
+<img src="assets/menu_options.png" alt="New menu options" width="50%">
+
 
 Note that ImageTensor/MaskTensor are just syntactic sugar for semantically differentiating the annotations (allowing ComfyUI to know what plugs into what); your function will still get passed genunine torch.Tensor objects.
 
 For more control, you can call easy_nodes.init(...) and change some settings that will apply to all nodes you create.
 
 ## New in 1.0.0:
 
 - Renamed to ComfyUI-EasyNodes (from ComfyUI-Annotations) to better reflect the package's goal (rather than the means)
 - Automatic module reloading: if you edit your node source, immediately see the changes
 - LLM-based debugging: optionally have ChatGPT take a crack at fixing your code
 - Set node colors via Python argument (no JavaScript required)
 - Add preview text and images to nodes via show_text and show_image Python functions, no JavaScript required.
+- Automatically create nodes with widgets to set the fields of existing Python objects.
 - Tooltips and deep links to node source code
 - Bug fixes
 
 ## Features
 
 - **@ComfyNode Decorator**: Simplifies the declaration of custom nodes with automagic node declaration based on Python type annotations. Existing Python functions can be converted to ComfyUI nodes with a simple "@ComfyNode()"
 - **Built-in text and image previews**: Just call `easy_nodes.add_preview_text()` and `easy_nodes.add_preview_image()` in the body of your function and EasyNodes will automatically display it, no JavaScript hacking required.
@@ -92,20 +99,27 @@
 To use this module in your ComfyUI project, follow these steps:
 
 1. **Install the Module**: Run the following command to install the ComfyUI-EasyNodes module:
 
     ```bash
     pip install ComfyUI-EasyNodes
     ```
-    or
-    ```
+    or, if you want to have an editable version:
+    ```bash
     pip install -e https://github.com/andrewharp/ComfyUI-EasyNodes
     ```
+    Note that this is not a typical ComfyUI nodepack, so does not itself live under custom_nodes.
+    
+    However, after installing you can copy the example node directory into custom_nodes to test them out:
+    ```bash
+    git clone --depth=1 https://github.com/andrewharp/ComfyUI-EasyNodes.git /tmp/easynodes
+    mv /tmp/easynodes/example $COMFYUI_DIR/custom_nodes/easynodes
+    ```
 
-2. **Integrate into Your Project**:
+3. **Integrate into Your Project**:
     - Open your ComfyUI project's `__init__.py` (e.g. `ComfyUI/custom_nodes/my_project/__init__.py`).
     - Make sure you're importing the module where you define your nodes:
 
     ```python
     import your_node_module
     ```
 
@@ -117,15 +131,15 @@
 
     @ComfyNode()
     def create_random_image(width: int=NumberInput(128, 128, 1024), 
                             height: int=NumberInput(128, 128, 1024)) -> ImageTensor:
         return torch.rand((1, height, width, 3))
     ```
 
-    If you run into problems with the auto-registration, you can try turning it off give ComfyUI your node mappings the regular way:
+    If you run into problems with the auto-registration, you can try turning it off and give ComfyUI your node mappings the regular way:
     <details>
 
     In `__init__.py`:
 
     ```python
     import easy_nodes
     import your_node_module
@@ -137,14 +151,17 @@
     ```
 
     and in `your_node_module.py`:
     ```python
     import easy_nodes
     easy_nodes.initialize_easy_nodes(default_category=my_category, auto_register=False)
 
+    @ComfyNode()
+    def my_node(foo: int) -> int:
+        return foo + 42
     ...
     ```
 
     </details>
 
 ## Usage
```

### Comparing `comfyui_easynodes-1.0.2/easy_nodes/config_service.py` & `comfyui_easynodes-1.0.3/easy_nodes/config_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 import os
 import json
 import re
 from server import PromptServer
 from aiohttp import web
 
 # Receives config values from config_service.js
```

### Comparing `comfyui_easynodes-1.0.2/easy_nodes/easy_nodes.py` & `comfyui_easynodes-1.0.3/easy_nodes/easy_nodes.py`

 * *Files identical despite different names*

### Comparing `comfyui_easynodes-1.0.2/easy_nodes/llm_debugging.py` & `comfyui_easynodes-1.0.3/easy_nodes/llm_debugging.py`

 * *Files identical despite different names*

### Comparing `comfyui_easynodes-1.0.2/pyproject.toml` & `comfyui_easynodes-1.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ComfyUI-EasyNodes"
-version = "1.0.2"
+version = "1.0.3"
 description = "Makes creating new nodes for ComfyUI a breeze."
 readme = "readme.md"
 authors = [{ name = "Andrew Harp", email = "andrew.harp@gmail.com" }]
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
 dependencies = [
     "torch",
@@ -19,29 +19,36 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/andrewharp/ComfyUI-EasyNodes"
 "Bug Reports" = "https://github.com/andrewharp/ComfyUI-EasyNodes/issues"
 "Source" = "https://github.com/andrewharp/ComfyUI-EasyNodes/"
 
-[tool.setuptools]
-packages = ["easy_nodes"]
+[tool.setuptools.packages.find]
+where = ["."]
+include = ["easy_nodes"]
+exclude = ["web"]
+
+[tool.setuptools.package-data]
+"*" = ["web/**/*"]
 
 [tool.poetry]
-name = "ComfyUI-EasyNodes"
-version = "1.0.2"
+name = "comfyui-easynodes"
+version = "1.0.3"
 description = "Makes creating new nodes for ComfyUI a breeze."
 authors = ["Andrew Harp <andrew.harp@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/andrewharp/ComfyUI-EasyNodes"
 repository = "https://github.com/andrewharp/ComfyUI-EasyNodes"
 documentation = "https://github.com/andrewharp/ComfyUI-EasyNodes"
 readme = "readme.md"
-include = ["web/**/*"]
+packages = [{ include = "easy_nodes" }]
+include = ["easy_nodes/web/**/*"]
+
 
 [tool.poetry.dependencies]
 python = ">=3.10"
 torch = "*"
 pillow = "*"
 colorama = "*"
 numpy = "*"
-openai = "*"
+openai = "*"
```

### Comparing `comfyui_easynodes-1.0.2/readme.md` & `comfyui_easynodes-1.0.3/readme.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,28 +14,35 @@
     """Returns separate masks for values above and below the threshold value."""
     mask_below = torch.any(image < threshold_value, dim=-1)
     return mask_below.float(), (~mask_below).float()
 ```
 
 That's it! Now your node is ready for ComfyUI. More examples can be found [here](example/example_nodes.py).
 
+Sample node with tooltip and deep source link:
+
 <img src="assets/threshold_example.png" alt="The new node with tooltip" width="50%">
 
+New settings:
+
+<img src="assets/menu_options.png" alt="New menu options" width="50%">
+
 
 Note that ImageTensor/MaskTensor are just syntactic sugar for semantically differentiating the annotations (allowing ComfyUI to know what plugs into what); your function will still get passed genunine torch.Tensor objects.
 
 For more control, you can call easy_nodes.init(...) and change some settings that will apply to all nodes you create.
 
 ## New in 1.0.0:
 
 - Renamed to ComfyUI-EasyNodes (from ComfyUI-Annotations) to better reflect the package's goal (rather than the means)
 - Automatic module reloading: if you edit your node source, immediately see the changes
 - LLM-based debugging: optionally have ChatGPT take a crack at fixing your code
 - Set node colors via Python argument (no JavaScript required)
 - Add preview text and images to nodes via show_text and show_image Python functions, no JavaScript required.
+- Automatically create nodes with widgets to set the fields of existing Python objects.
 - Tooltips and deep links to node source code
 - Bug fixes
 
 ## Features
 
 - **@ComfyNode Decorator**: Simplifies the declaration of custom nodes with automagic node declaration based on Python type annotations. Existing Python functions can be converted to ComfyUI nodes with a simple "@ComfyNode()"
 - **Built-in text and image previews**: Just call `easy_nodes.add_preview_text()` and `easy_nodes.add_preview_image()` in the body of your function and EasyNodes will automatically display it, no JavaScript hacking required.
@@ -53,20 +60,27 @@
 To use this module in your ComfyUI project, follow these steps:
 
 1. **Install the Module**: Run the following command to install the ComfyUI-EasyNodes module:
 
     ```bash
     pip install ComfyUI-EasyNodes
     ```
-    or
-    ```
+    or, if you want to have an editable version:
+    ```bash
     pip install -e https://github.com/andrewharp/ComfyUI-EasyNodes
     ```
+    Note that this is not a typical ComfyUI nodepack, so does not itself live under custom_nodes.
+    
+    However, after installing you can copy the example node directory into custom_nodes to test them out:
+    ```bash
+    git clone --depth=1 https://github.com/andrewharp/ComfyUI-EasyNodes.git /tmp/easynodes
+    mv /tmp/easynodes/example $COMFYUI_DIR/custom_nodes/easynodes
+    ```
 
-2. **Integrate into Your Project**:
+3. **Integrate into Your Project**:
     - Open your ComfyUI project's `__init__.py` (e.g. `ComfyUI/custom_nodes/my_project/__init__.py`).
     - Make sure you're importing the module where you define your nodes:
 
     ```python
     import your_node_module
     ```
 
@@ -78,15 +92,15 @@
 
     @ComfyNode()
     def create_random_image(width: int=NumberInput(128, 128, 1024), 
                             height: int=NumberInput(128, 128, 1024)) -> ImageTensor:
         return torch.rand((1, height, width, 3))
     ```
 
-    If you run into problems with the auto-registration, you can try turning it off give ComfyUI your node mappings the regular way:
+    If you run into problems with the auto-registration, you can try turning it off and give ComfyUI your node mappings the regular way:
     <details>
 
     In `__init__.py`:
 
     ```python
     import easy_nodes
     import your_node_module
@@ -98,14 +112,17 @@
     ```
 
     and in `your_node_module.py`:
     ```python
     import easy_nodes
     easy_nodes.initialize_easy_nodes(default_category=my_category, auto_register=False)
 
+    @ComfyNode()
+    def my_node(foo: int) -> int:
+        return foo + 42
     ...
     ```
 
     </details>
 
 ## Usage
```

