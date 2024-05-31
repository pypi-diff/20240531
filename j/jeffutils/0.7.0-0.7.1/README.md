# Comparing `tmp/jeffutils-0.7.0.tar.gz` & `tmp/jeffutils-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeffutils-0.7.0.tar", last modified: Fri May 31 17:01:18 2024, max compression
+gzip compressed data, was "jeffutils-0.7.1.tar", last modified: Fri May 31 17:11:00 2024, max compression
```

## Comparing `jeffutils-0.7.0.tar` & `jeffutils-0.7.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:01:18.506269 jeffutils-0.7.0/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.7.0/LICENSE.txt
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      576 2024-05-31 17:01:18.506269 jeffutils-0.7.0/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     2636 2024-05-31 16:55:11.000000 jeffutils-0.7.0/README.md
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.7.0/pyproject.toml
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-31 17:01:18.506269 jeffutils-0.7.0/setup.cfg
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      715 2024-05-31 17:01:15.000000 jeffutils-0.7.0/setup.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:01:18.506269 jeffutils-0.7.0/src/
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:01:18.506269 jeffutils-0.7.0/src/jeffutils/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.7.0/src/jeffutils/__init__.py
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    37444 2024-05-31 17:00:43.000000 jeffutils-0.7.0/src/jeffutils/utils.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:01:18.506269 jeffutils-0.7.0/src/jeffutils.egg-info/
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      576 2024-05-31 17:01:18.000000 jeffutils-0.7.0/src/jeffutils.egg-info/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-31 17:01:18.000000 jeffutils-0.7.0/src/jeffutils.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-31 17:01:18.000000 jeffutils-0.7.0/src/jeffutils.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-31 17:01:18.000000 jeffutils-0.7.0/src/jeffutils.egg-info/top_level.txt
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:11:00.333500 jeffutils-0.7.1/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.7.1/LICENSE.txt
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      576 2024-05-31 17:11:00.333500 jeffutils-0.7.1/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     2685 2024-05-31 17:04:40.000000 jeffutils-0.7.1/README.md
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.7.1/pyproject.toml
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-31 17:11:00.333500 jeffutils-0.7.1/setup.cfg
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      715 2024-05-31 17:10:59.000000 jeffutils-0.7.1/setup.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:11:00.333500 jeffutils-0.7.1/src/
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:11:00.333500 jeffutils-0.7.1/src/jeffutils/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.7.1/src/jeffutils/__init__.py
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    37827 2024-05-31 17:05:48.000000 jeffutils-0.7.1/src/jeffutils/utils.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:11:00.333500 jeffutils-0.7.1/src/jeffutils.egg-info/
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      576 2024-05-31 17:11:00.000000 jeffutils-0.7.1/src/jeffutils.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-31 17:11:00.000000 jeffutils-0.7.1/src/jeffutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-31 17:11:00.000000 jeffutils-0.7.1/src/jeffutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-31 17:11:00.000000 jeffutils-0.7.1/src/jeffutils.egg-info/top_level.txt
```

### Comparing `jeffutils-0.7.0/LICENSE.txt` & `jeffutils-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jeffutils-0.7.0/PKG-INFO` & `jeffutils-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeffutils
-Version: 0.7.0
+Version: 0.7.1
 Summary: Welcome to Jeff Hansen's suite of useful python functions! I use lots of these functions on most of my Data Analysis, Backend-Dev, and Machine Learning projects, and I hope you find some of them useful as well!
 Home-page: https://github.com/jeffxhansen/jeffutils
 Author: Jeff Hansen
 Author-email: jeffxhansen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jeffutils-0.7.0/README.md` & `jeffutils-0.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # jeffutils
 
-Welcome to Jeff Hansen's suite of useful python functions! I use lots of these functions on most of my projects, and I hope you find some of them useful as well!
+Welcome to Jeff Hansen's suite of useful python functions! I use lots of these functions on most of my Data Analysis, Backend-Dev, and Machine Learning projects, and I hope you find some of them useful as well!
 
 # Installation
 
 You can install this package from `PyPi` with
 ```
 pip install jeffutils
 ```
```

### Comparing `jeffutils-0.7.0/setup.py` & `jeffutils-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='jeffutils',
-    version='0.7.0',
+    version='0.7.1',
     author='Jeff Hansen',
     author_email='jeffxhansen@gmail.com',
     description="Welcome to Jeff Hansen's suite of useful python functions! I use lots of these functions on most of my Data Analysis, Backend-Dev, and Machine Learning projects, and I hope you find some of them useful as well!",
     package_dir={"": "src"},
     packages = find_packages(where="src"),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `jeffutils-0.7.0/src/jeffutils/utils.py` & `jeffutils-0.7.1/src/jeffutils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -589,20 +589,22 @@
             else:
                 pass
             
         # sleep for 1 minute, so that it only checks all of the threads
         # every minute
         time.sleep(60)
         
-def reimport(statements:str|list):
+def reimport(statements:str|list, globals):
     """ takes in python import code represented as a string or a list of strings, and
     it reimports all of the modules and functions in the import statements. This allows
     you to reimport modules that have been changed in the background without having to
     restart the kernel.
     
+    Example Call: reimport("import numpy as np", globals())
+    
     The input can either be:
     - a string with a single import statement
       ex: 'import numpy as np' or 'from random import choice, randint'
     - a multiline string with multiple import statements
       ex: '''import numpy as np
       import pandas as pd
       from random import choice, randint'''
@@ -621,14 +623,20 @@
         thing2, \\
         thing3
     
     
     raises:
     AttributeError: if the module or function is not found in sys.modules
     
+    GLOBALS NOTE:
+    Note that the function call requires that you pass in globals() as the second argument
+    so that the function can update the global variables with the new imports. If you don't
+    pass in globals(), then the function will not be able to update the global variables with
+    the new imports.
+    
     DEPENDENCY NOTE: 
     If you make changes to two files file_1.py and file_2.py, and file_2 imports file_1, if you
     reimport file_2, then the changes in file_1 will not be reflected in file_2. You must reimport
     both file_1 and file_2 to see the changes in file_1 reflected in file_2.
        
     """
     ##########################
@@ -650,18 +658,18 @@
             importlib.reload(sys.modules[module_name])
             module_obj = sys.modules[module_name]
         else:
             if "." in module_name:
                 module_obj = _import_module_hierarchy(module_name)[module_name]
             else:
                 module_obj = importlib.import_module(module_name)
-        globals()[module_name] = module_obj
+        globals[module_name] = module_obj
         
         if alias:
-            globals()[alias] = module_obj
+            globals[alias] = module_obj
             
         return module_obj
             
     def _import_sub_func(module, func):
         """ handles something like "from random import randint" where 'random'
         is the module and 'randint' is the function
         """
@@ -674,17 +682,17 @@
             func_name = func_name.strip()
             alias = alias.strip()
         else:
             func_name, alias = func.strip(), None
         
         if func_name in dir(module_obj):
             if alias:
-                globals()[alias] = getattr(module_obj, func_name)
+                globals[alias] = getattr(module_obj, func_name)
             else:
-                globals()[func_name] = getattr(module_obj, func_name)
+                globals[func_name] = getattr(module_obj, func_name)
         else:
             raise AttributeError(f"Function {func_name} not found in module {module}")
         
     def _get_sub_modules(package_path:str):
         """ takes in a package_path like directory.sub_directory and returns a 
         string of all of the modules in that directory like ['directory.sub_directory.module1',
         'directory.sub_directory.module2', ...]
@@ -728,15 +736,15 @@
         all of the functions inside the module_name.py file """
         if module not in sys.modules:
             raise AttributeError(f"Module {module} not found in sys.modules")
         module_obj = sys.modules[module]
         
         for func_name in dir(module_obj):
             if not func_name.startswith("_"):
-                globals()[func_name] = getattr(module_obj, func_name)
+                globals[func_name] = getattr(module_obj, func_name)
 
     def _import_sub_module_component(parent_module, sub_component):
         """ handles a situation like 'from parent_module import sub_component' whether
         that sub_component is another package/module, function or the '*' wildcard
         """
         sub_component_type = _get_type_as_str(parent_module, sub_component)
         if sub_component_type == 'module':
@@ -769,15 +777,15 @@
             if curr_module in sys.modules:
                 importlib.reload(sys.modules[curr_module])
                 module_obj = sys.modules[curr_module]
             else:
                 module_obj = importlib.import_module(curr_module)
             # add the current_module path to the module_objs dictionary
             module_objs[curr_module] = module_obj
-            globals()[curr_module] = module_obj
+            globals[curr_module] = module_obj
             
         return module_objs
             
     def _process_single_import_statement(import_statement:str):
         """ takes in a single import statement like 'import numpy as np' or 'from random import choice'
         and imports the module or function
         """
```

### Comparing `jeffutils-0.7.0/src/jeffutils.egg-info/PKG-INFO` & `jeffutils-0.7.1/src/jeffutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeffutils
-Version: 0.7.0
+Version: 0.7.1
 Summary: Welcome to Jeff Hansen's suite of useful python functions! I use lots of these functions on most of my Data Analysis, Backend-Dev, and Machine Learning projects, and I hope you find some of them useful as well!
 Home-page: https://github.com/jeffxhansen/jeffutils
 Author: Jeff Hansen
 Author-email: jeffxhansen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

