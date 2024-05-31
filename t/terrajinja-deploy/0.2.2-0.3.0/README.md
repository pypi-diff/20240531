# Comparing `tmp/terrajinja-deploy-0.2.2.tar.gz` & `tmp/terrajinja-deploy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terrajinja-deploy-0.2.2.tar", last modified: Mon Mar 25 12:22:39 2024, max compression
+gzip compressed data, was "terrajinja-deploy-0.3.0.tar", last modified: Fri May 31 09:00:57 2024, max compression
```

## Comparing `terrajinja-deploy-0.2.2.tar` & `terrajinja-deploy-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 12:22:39.928233 terrajinja-deploy-0.2.2/
--rw-rw-rw-   0 root         (0) root         (0)       80 2024-03-25 12:22:37.000000 terrajinja-deploy-0.2.2/HISTORY.md
--rw-r--r--   0 root         (0) root         (0)     1061 2024-03-25 12:22:38.000000 terrajinja-deploy-0.2.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      320 2024-03-25 12:22:37.000000 terrajinja-deploy-0.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      779 2024-03-25 12:22:39.928233 terrajinja-deploy-0.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      263 2024-03-25 12:22:37.000000 terrajinja-deploy-0.2.2/Pipfile
--rw-rw-rw-   0 root         (0) root         (0)      135 2024-03-25 12:22:37.000000 terrajinja-deploy-0.2.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)       45 2024-03-25 12:22:37.000000 terrajinja-deploy-0.2.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-25 12:22:39.928233 terrajinja-deploy-0.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1352 2024-03-25 12:22:38.000000 terrajinja-deploy-0.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 12:22:39.924232 terrajinja-deploy-0.2.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 12:22:39.924232 terrajinja-deploy-0.2.2/src/terrajinja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 12:22:39.926232 terrajinja-deploy-0.2.2/src/terrajinja/deploy/
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-03-25 12:22:37.000000 terrajinja-deploy-0.2.2/src/terrajinja/deploy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9471 2024-03-25 12:22:37.000000 terrajinja-deploy-0.2.2/src/terrajinja/deploy/terraform_deployment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 12:22:39.927232 terrajinja-deploy-0.2.2/src/terrajinja_deploy.egg-info/
--rw-r--r--   0 root         (0) root         (0)      779 2024-03-25 12:22:39.000000 terrajinja-deploy-0.2.2/src/terrajinja_deploy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      413 2024-03-25 12:22:39.000000 terrajinja-deploy-0.2.2/src/terrajinja_deploy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 12:22:39.000000 terrajinja-deploy-0.2.2/src/terrajinja_deploy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-03-25 12:22:39.000000 terrajinja-deploy-0.2.2/src/terrajinja_deploy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-03-25 12:22:39.000000 terrajinja-deploy-0.2.2/src/terrajinja_deploy.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 12:22:39.927232 terrajinja-deploy-0.2.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3476 2024-03-25 12:22:37.000000 terrajinja-deploy-0.2.2/tests/test_terraform_deployment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:00:57.197350 terrajinja-deploy-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2024-05-31 09:00:56.000000 terrajinja-deploy-0.3.0/HISTORY.md
+-rw-r--r--   0 root         (0) root         (0)     1061 2024-05-31 09:00:56.000000 terrajinja-deploy-0.3.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      320 2024-05-31 09:00:56.000000 terrajinja-deploy-0.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      779 2024-05-31 09:00:57.197350 terrajinja-deploy-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      263 2024-05-31 09:00:56.000000 terrajinja-deploy-0.3.0/Pipfile
+-rw-rw-rw-   0 root         (0) root         (0)      135 2024-05-31 09:00:56.000000 terrajinja-deploy-0.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       45 2024-05-31 09:00:56.000000 terrajinja-deploy-0.3.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 09:00:57.197350 terrajinja-deploy-0.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1352 2024-05-31 09:00:56.000000 terrajinja-deploy-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:00:57.194350 terrajinja-deploy-0.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:00:57.194350 terrajinja-deploy-0.3.0/src/terrajinja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:00:57.196350 terrajinja-deploy-0.3.0/src/terrajinja/deploy/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-31 09:00:56.000000 terrajinja-deploy-0.3.0/src/terrajinja/deploy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9572 2024-05-31 09:00:56.000000 terrajinja-deploy-0.3.0/src/terrajinja/deploy/terraform_deployment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:00:57.197350 terrajinja-deploy-0.3.0/src/terrajinja_deploy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      779 2024-05-31 09:00:57.000000 terrajinja-deploy-0.3.0/src/terrajinja_deploy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      413 2024-05-31 09:00:57.000000 terrajinja-deploy-0.3.0/src/terrajinja_deploy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 09:00:57.000000 terrajinja-deploy-0.3.0/src/terrajinja_deploy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-31 09:00:57.000000 terrajinja-deploy-0.3.0/src/terrajinja_deploy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-31 09:00:57.000000 terrajinja-deploy-0.3.0/src/terrajinja_deploy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:00:57.197350 terrajinja-deploy-0.3.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     5869 2024-05-31 09:00:56.000000 terrajinja-deploy-0.3.0/tests/test_terraform_deployment.py
```

### Comparing `terrajinja-deploy-0.2.2/LICENSE` & `terrajinja-deploy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `terrajinja-deploy-0.2.2/PKG-INFO` & `terrajinja-deploy-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrajinja-deploy
-Version: 0.2.2
+Version: 0.3.0
 Summary: Terrajinja extension for automation using cdktf
 Home-page: https://gitlab/terrajinja
 Author: Terrajinja Team
 Author-email: int-terrajinja@schubergphilis.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `terrajinja-deploy-0.2.2/setup.py` & `terrajinja-deploy-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 requirements = [line.strip()
           for line in open('requirements.txt').readlines()
           if line.strip() and not line.startswith('#')]
 
 readme = open('README.md').read()
 history = open('HISTORY.md').read()
-version = '0.2.2'
+version = '0.3.0'
 name= 'terrajinja-deploy'
 package_path= name.replace('-', '.')
 
 # only the cli has an entry point
 entry_points=None
 if name=='terrajinja-cli':
     entry_points={
```

### Comparing `terrajinja-deploy-0.2.2/src/terrajinja/deploy/terraform_deployment.py` & `terrajinja-deploy-0.3.0/src/terrajinja/deploy/terraform_deployment.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import os
 from importlib import import_module
 from inspect import isclass
 from pathlib import Path
 from sys import path
+import re
 
 from cdktf import App, TerraformStack
 from subprocess import Popen, PIPE
 
 # adjust path for library loading:
 # prefer cdktf get over prebuild imports
 path.append(f"{Path(__file__).parent.parent.parent}/imports")
@@ -160,27 +161,26 @@
             parameters: the parameters items of the module
 
         Returns:
             dict with search values resolved
 
         """
         if isinstance(parameters, dict):
-            for k in parameters.keys():
-                parameters[k] = self.replace_lookup_variables_recursive(parameters[k])
+            return {key: self.replace_lookup_variables_recursive(value) for key, value in parameters.items()}
+        elif isinstance(parameters, list):
+            return [self.replace_lookup_variables_recursive(item) for item in parameters]
+        elif isinstance(parameters, str):
+            matches = re.findall(r'\$[a-zA-Z0-9_.]+', parameters)
+            for match in matches:
+                lookup_key = match[1:]  # remove the dollar sign
+                replacement_value = self.get_variable_by_path(self.results, lookup_key)
+                parameters = parameters.replace(match, str(replacement_value))
             return parameters
-
-        if isinstance(parameters, list):
-            return [self.replace_lookup_variables_recursive(t) for t in parameters]
-
-        if isinstance(parameters, str):
-            # terraform uses ${} for some syntax
-            if len(parameters) > 2 and parameters[0] == "$" and parameters[1] != "{":
-                parameters = self.get_variable_by_path(self.results, parameters[1:])
+        else:
             return parameters
-        return parameters
 
     def create_resource(self, name: str, module: str, resource: dict) -> object:
         """Create a terraform resource and add it to App
 
         Args:
             name (str): name of the resource to create
             module (str): name of the module to load
```

### Comparing `terrajinja-deploy-0.2.2/src/terrajinja_deploy.egg-info/PKG-INFO` & `terrajinja-deploy-0.3.0/src/terrajinja_deploy.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrajinja-deploy
-Version: 0.2.2
+Version: 0.3.0
 Summary: Terrajinja extension for automation using cdktf
 Home-page: https://gitlab/terrajinja
 Author: Terrajinja Team
 Author-email: int-terrajinja@schubergphilis.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

