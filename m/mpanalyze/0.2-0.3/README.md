# Comparing `tmp/mpanalyze-0.2.tar.gz` & `tmp/mpanalyze-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpanalyze-0.2.tar", last modified: Sat May 25 13:34:30 2024, max compression
+gzip compressed data, was "mpanalyze-0.3.tar", last modified: Fri May 31 11:20:34 2024, max compression
```

## Comparing `mpanalyze-0.2.tar` & `mpanalyze-0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 13:34:30.762240 mpanalyze-0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-25 13:34:24.000000 mpanalyze-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-25 13:34:30.762240 mpanalyze-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-25 13:34:24.000000 mpanalyze-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 13:34:30.762240 mpanalyze-0.2/mpanalyze/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-25 13:34:24.000000 mpanalyze-0.2/mpanalyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-25 13:34:24.000000 mpanalyze-0.2/mpanalyze/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-25 13:34:24.000000 mpanalyze-0.2/mpanalyze/generate_cahrts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-25 13:34:24.000000 mpanalyze-0.2/mpanalyze/get_params_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-25 13:34:24.000000 mpanalyze-0.2/mpanalyze/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 13:34:30.762240 mpanalyze-0.2/mpanalyze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-25 13:34:30.000000 mpanalyze-0.2/mpanalyze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-25 13:34:30.000000 mpanalyze-0.2/mpanalyze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 13:34:30.000000 mpanalyze-0.2/mpanalyze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-25 13:34:30.000000 mpanalyze-0.2/mpanalyze.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 13:34:30.000000 mpanalyze-0.2/mpanalyze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 13:34:30.000000 mpanalyze-0.2/mpanalyze.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 13:34:30.762240 mpanalyze-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-25 13:34:24.000000 mpanalyze-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:20:34.454029 mpanalyze-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-31 11:20:31.000000 mpanalyze-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-31 11:20:34.454029 mpanalyze-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-31 11:20:31.000000 mpanalyze-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:20:34.454029 mpanalyze-0.3/mpanalyze/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-31 11:20:31.000000 mpanalyze-0.3/mpanalyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-31 11:20:31.000000 mpanalyze-0.3/mpanalyze/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-31 11:20:31.000000 mpanalyze-0.3/mpanalyze/generate_cahrts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-31 11:20:31.000000 mpanalyze-0.3/mpanalyze/get_params_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-31 11:20:31.000000 mpanalyze-0.3/mpanalyze/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:20:34.454029 mpanalyze-0.3/mpanalyze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-31 11:20:34.000000 mpanalyze-0.3/mpanalyze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-31 11:20:34.000000 mpanalyze-0.3/mpanalyze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 11:20:34.000000 mpanalyze-0.3/mpanalyze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-31 11:20:34.000000 mpanalyze-0.3/mpanalyze.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-31 11:20:34.000000 mpanalyze-0.3/mpanalyze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-31 11:20:34.000000 mpanalyze-0.3/mpanalyze.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 11:20:34.454029 mpanalyze-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-31 11:20:31.000000 mpanalyze-0.3/setup.py
```

### Comparing `mpanalyze-0.2/LICENSE` & `mpanalyze-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mpanalyze-0.2/PKG-INFO` & `mpanalyze-0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,54 @@
-Metadata-Version: 2.1
-Name: mpanalyze
-Version: 0.2
-Summary: A package for analyzing model parameters
-Home-page: https://github.com/JJLi0427/Model_Params_Analyze
-Author: Jiajun Li
-Author-email: 2366876022@qq.com
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pyecharts
-
 # Model Parameters Analyzer
 
 This is a Python package that helps you analyze the parameters of your models. It calculates the number of parameters in the model and their percentages than generate analyze JSON file and charts for you.
 
+## 中文介绍
+
+这是一个可帮助您分析模型参数的Python包。它计算模型中的参数数量及其百分比，然后为您生成分析 JSON 文件和图表。  
+快速安装: `pip install mpanalyze`  
+简单使用: `import mpanalyze` `mpanalyze.params_analyze(${model})`  
+详细参数参考 [Usage](#Usage)
+
 ## Porject Displays
 
+![tree](./display/tree.jpg)
+![treemap](./display/treemap.jpg)
+
 ## Installation
 
 To install this package, you can use pip:
 
 ```sh
 pip install mpanalyze
 ```
 
 ## Usage
 
 You can use this package from the command line with the follow command:
 
 ```python
-from mpanalyze import params_analyze
-params_analyze(${model})
+import mpanalyze
+mpanalyze.params_analyze(${model})
 ```
 
-* More parameters  
+* More parameters for params_analyze   
 `model`: object | The model to analyze.  
 `name`: str(Optional) | The name of the model. It will add to the analyze dir begin. If not specified, the directory name will be 'params_analyze'.  
 `port`: int(Opetional) | The port to use for the HTTP server. If not specified, the browser will not be opened. Recommended only use in Debug mode. If you want to use in training, it will block the training process.  
+`save_dict`: bool(Optional) | Whether to save the parameters to a JSON file. Default is True.
 `tree`: bool(Optional) | Whether to draw a tree chart. Default is True.  
 `treemap`: bool(Optional) | Whether to draw a TreeMap chart. Default is True.  
 
+Only get analyze aict:  
+
+```python
+param_dict = calculate_dict(model)
+```
+
 This will calculate the parameters and their percentages for your model.  
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
 
 ## License
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mpanalyze-0.2/mpanalyze/analyze.py` & `mpanalyze-0.3/mpanalyze/analyze.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 # Usage:
-# calculate_parameters(model)
+# mpanalyze.params_analyze(${model})
 
 from typing import Optional
 from .utils import save_parameters_to_json, start_http_server, make_analyze_dir
 from .generate_cahrts import create_charts
 from .get_params_dict import calculate_dict
 
 def params_analyze(
     model: object, 
     name: Optional[str]=None,
     port: Optional[int]=None,
+    save_dict: Optional[bool]=True,
     tree: Optional[bool]=True,
     treemap: Optional[bool]=True
 ):
     """
     Calculate the number of parameters in the model and their percentages.
     Draw a tree chart and a TreeMap chart to visualize the parameters.
     :param model: The model to analyze.
     :param name: The name of the model. If not specified, the directory name will be 'params_analyze'.
     :param port: The port to use for the HTTP server. If not specified, the browser will not be opened. Recommended only use in Debug mode. If you want to use in training, it will block the training process.
+    :param save_dict: Whether to save the parameters to a JSON file. Default is True.
     :param tree: Whether to draw a tree chart. Default is True.
     :param treemap: Whether to draw a TreeMap chart. Default is True.
     """
     try:
-        dir = make_analyze_dir(name)
-        param_dict = calculate_dict(model)
-        save_parameters_to_json(param_dict, dir)
-        if tree and treemap:
-            create_charts(
-                param_dict, 
-                tree, 
-                treemap, 
-                dir
-            )
-            start_http_server(port)
+        if save_dict == False and tree == False and treemap == False:
+            print("Not saving any analyze file. Printing the parameters calculate dict instead.")
+            param_dict = calculate_dict(model)
+            print(param_dict)
+            return
+        else:
+            dir = make_analyze_dir(name)
+            param_dict = calculate_dict(model)
+            if save_dict:
+                save_parameters_to_json(param_dict, dir)
+            if tree and treemap:
+                create_charts(
+                    param_dict, 
+                    tree, 
+                    treemap, 
+                    dir
+                )
+                start_http_server(port)
     except Exception as e:
         print("Failed to calculate parameters: {}".format(e))
```

### Comparing `mpanalyze-0.2/mpanalyze/generate_cahrts.py` & `mpanalyze-0.3/mpanalyze/generate_cahrts.py`

 * *Files identical despite different names*

### Comparing `mpanalyze-0.2/mpanalyze/get_params_dict.py` & `mpanalyze-0.3/mpanalyze/get_params_dict.py`

 * *Files identical despite different names*

### Comparing `mpanalyze-0.2/setup.py` & `mpanalyze-0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mpanalyze",
-    version="0.2",
+    version="0.3",
     packages=find_packages(),
     install_requires=[
         'pyecharts',
     ],
     entry_points={
         'console_scripts': [
             'params_analyze=params_analyze.analyze:calculate_parameters',
```

