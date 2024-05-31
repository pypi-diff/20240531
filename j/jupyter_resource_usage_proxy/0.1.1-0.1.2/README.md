# Comparing `tmp/jupyter_resource_usage_proxy-0.1.1.tar.gz` & `tmp/jupyter_resource_usage_proxy-0.1.2.tar.gz`

## Comparing `jupyter_resource_usage_proxy-0.1.1.tar` & `jupyter_resource_usage_proxy-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyter_resource_usage_proxy-0.1.1/jupyter-config/jupyter_resource_usage_proxy.json
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyter_resource_usage_proxy-0.1.1/jupyter_resource_usage_proxy/__init__.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 jupyter_resource_usage_proxy-0.1.1/jupyter_resource_usage_proxy/app.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 jupyter_resource_usage_proxy-0.1.1/jupyter_resource_usage_proxy/handlers.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 jupyter_resource_usage_proxy-0.1.1/LICENSE
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 jupyter_resource_usage_proxy-0.1.1/README.md
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 jupyter_resource_usage_proxy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 jupyter_resource_usage_proxy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyter_resource_usage_proxy-0.1.2/jupyter-config/jupyter_resource_usage_proxy.json
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyter_resource_usage_proxy-0.1.2/jupyter_resource_usage_proxy/__init__.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 jupyter_resource_usage_proxy-0.1.2/jupyter_resource_usage_proxy/app.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 jupyter_resource_usage_proxy-0.1.2/jupyter_resource_usage_proxy/handlers.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 jupyter_resource_usage_proxy-0.1.2/LICENSE
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 jupyter_resource_usage_proxy-0.1.2/README.md
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 jupyter_resource_usage_proxy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 jupyter_resource_usage_proxy-0.1.2/PKG-INFO
```

### Comparing `jupyter_resource_usage_proxy-0.1.1/jupyter_resource_usage_proxy/app.py` & `jupyter_resource_usage_proxy-0.1.2/jupyter_resource_usage_proxy/app.py`

 * *Files identical despite different names*

### Comparing `jupyter_resource_usage_proxy-0.1.1/jupyter_resource_usage_proxy/handlers.py` & `jupyter_resource_usage_proxy-0.1.2/jupyter_resource_usage_proxy/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter_resource_usage_proxy-0.1.1/LICENSE` & `jupyter_resource_usage_proxy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_resource_usage_proxy-0.1.1/README.md` & `jupyter_resource_usage_proxy-0.1.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Jupyter Resource Usage Proxy
 
 In one terminal/environment:
 
 ```console
-pip install fps_uvicorn
-pip install fps_resource_usage
+pip install jupyverse-api
+pip install fps-resource-usage
 pip install fps-noauth
 
 # launch a terminal server at http://127.0.0.1:8000
-fps-uvicorn --port=8000 --no-open-browser
+jupyverse --port=8000
 ```
 
 In another terminal/environment:
 
 ```console
 pip install jupyter_resource_usage
 pip install jupyter_resource_usage_proxy
```

### Comparing `jupyter_resource_usage_proxy-0.1.1/pyproject.toml` & `jupyter_resource_usage_proxy-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -11,31 +11,33 @@
 keywords = ["ipython", "jupyter"]
 classifiers = [
   "Intended Audience :: Developers",
   "Intended Audience :: System Administrators",
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
-  "jupyter_server>=1.0.0",
-  "httpx>=0.23.1",
+  "jupyter_server >=1.0.0,<3.0.0",
+  "httpx >=0.27.0,<0.28",
 ]
 
 [[project.authors]]
 name = "David Brochart"
 email = "david.brochart@gmail.com"
 
 [project.urls]
 Homepage = "https://github.com/davidbrochart/jupyter_resource_usage_proxy"
 
 [tool.hatch.version]
 path = "jupyter_resource_usage_proxy/__init__.py"
 
-[tool.hatch.build.targets.wheel.shared-data]
-"jupyter-config" = "etc/jupyter/jupyter_server_config.d"
+[tool.hatch.build.targets.wheel]
+ignore-vcs = true
+packages = ["jupyter_resource_usage_proxy"]
+shared-data = {"jupyter-config" = "etc/jupyter/jupyter_server_config.d"}
```

### Comparing `jupyter_resource_usage_proxy-0.1.1/PKG-INFO` & `jupyter_resource_usage_proxy-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jupyter_resource_usage_proxy
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Jupyter Server Extension Proxying Resource Usage.
 Project-URL: Homepage, https://github.com/davidbrochart/jupyter_resource_usage_proxy
 Author-email: David Brochart <david.brochart@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 David Brochart
         
@@ -28,35 +28,35 @@
 License-File: LICENSE
 Keywords: ipython,jupyter
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Requires-Dist: httpx>=0.23.1
-Requires-Dist: jupyter-server>=1.0.0
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Requires-Dist: httpx<0.28,>=0.27.0
+Requires-Dist: jupyter-server<3.0.0,>=1.0.0
 Description-Content-Type: text/markdown
 
 # Jupyter Resource Usage Proxy
 
 In one terminal/environment:
 
 ```console
-pip install fps_uvicorn
-pip install fps_resource_usage
+pip install jupyverse-api
+pip install fps-resource-usage
 pip install fps-noauth
 
 # launch a terminal server at http://127.0.0.1:8000
-fps-uvicorn --port=8000 --no-open-browser
+jupyverse --port=8000
 ```
 
 In another terminal/environment:
 
 ```console
 pip install jupyter_resource_usage
 pip install jupyter_resource_usage_proxy
```

