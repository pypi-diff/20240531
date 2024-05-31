# Comparing `tmp/jeffutils-0.6.9.tar.gz` & `tmp/jeffutils-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeffutils-0.6.9.tar", last modified: Wed May 29 16:21:31 2024, max compression
+gzip compressed data, was "jeffutils-0.7.0.tar", last modified: Fri May 31 17:01:18 2024, max compression
```

## Comparing `jeffutils-0.6.9.tar` & `jeffutils-0.7.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-29 16:21:31.478493 jeffutils-0.6.9/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.6.9/LICENSE.txt
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      472 2024-05-29 16:21:31.478493 jeffutils-0.6.9/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     2614 2024-05-28 19:37:43.000000 jeffutils-0.6.9/README.md
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.6.9/pyproject.toml
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-29 16:21:31.478493 jeffutils-0.6.9/setup.cfg
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      611 2024-05-29 16:21:27.000000 jeffutils-0.6.9/setup.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-29 16:21:31.478493 jeffutils-0.6.9/src/
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-29 16:21:31.478493 jeffutils-0.6.9/src/jeffutils/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.6.9/src/jeffutils/__init__.py
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    36264 2024-05-29 16:21:14.000000 jeffutils-0.6.9/src/jeffutils/utils.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-29 16:21:31.478493 jeffutils-0.6.9/src/jeffutils.egg-info/
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      472 2024-05-29 16:21:31.000000 jeffutils-0.6.9/src/jeffutils.egg-info/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-29 16:21:31.000000 jeffutils-0.6.9/src/jeffutils.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-29 16:21:31.000000 jeffutils-0.6.9/src/jeffutils.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-29 16:21:31.000000 jeffutils-0.6.9/src/jeffutils.egg-info/top_level.txt
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:01:18.506269 jeffutils-0.7.0/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.7.0/LICENSE.txt
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      576 2024-05-31 17:01:18.506269 jeffutils-0.7.0/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     2636 2024-05-31 16:55:11.000000 jeffutils-0.7.0/README.md
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.7.0/pyproject.toml
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-31 17:01:18.506269 jeffutils-0.7.0/setup.cfg
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      715 2024-05-31 17:01:15.000000 jeffutils-0.7.0/setup.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:01:18.506269 jeffutils-0.7.0/src/
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:01:18.506269 jeffutils-0.7.0/src/jeffutils/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.7.0/src/jeffutils/__init__.py
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    37444 2024-05-31 17:00:43.000000 jeffutils-0.7.0/src/jeffutils/utils.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:01:18.506269 jeffutils-0.7.0/src/jeffutils.egg-info/
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      576 2024-05-31 17:01:18.000000 jeffutils-0.7.0/src/jeffutils.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-31 17:01:18.000000 jeffutils-0.7.0/src/jeffutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-31 17:01:18.000000 jeffutils-0.7.0/src/jeffutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-31 17:01:18.000000 jeffutils-0.7.0/src/jeffutils.egg-info/top_level.txt
```

### Comparing `jeffutils-0.6.9/LICENSE.txt` & `jeffutils-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jeffutils-0.6.9/README.md` & `jeffutils-0.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 ```
 >>> random_numbers(10)
 [3, 5, 5, 4, 5, 0, 0, 5, 5, 5]
 ```
 The python session is still using the old versions of the `start` and `end` variables. Without restarting your python session, you can run these lines of code:
 ```Python
 >>> from jeffutils.utils import reimport
->>> reimport(["import constants", "from file import random_numbers"])
+>>> reimport(["import constants", "from file import random_numbers"], globals())
 >>> random_numbers(10)
 [1, 1, 1, 0, 1, 1, 0, 0, 1, 1]
 ```
 and you will see that the changes have been updated, without you having to restart the session and lose all other variables.
 
 `reimport` also handles entire blocks of import statements like this:
 ```Python
@@ -73,15 +73,15 @@
 from jeffutils.utils import reimport
 reimport("""from time import sleep
 from constants import (
     long_var_name,
     another_long_var_name,
     EPOCHS
 )
-from file import func1, func2, func3""")
+from file import func1, func2, func3""", globals())
 ```
 
 ## stack_trace
 
 Are you tired of
 ```Python
 try:
```

### Comparing `jeffutils-0.6.9/setup.py` & `jeffutils-0.7.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 setup(
     name='jeffutils',
-    version='0.6.9',
+    version='0.7.0',
     author='Jeff Hansen',
     author_email='jeffxhansen@gmail.com',
-    description='A series of useful functions and decorators I use in most of my projects. Feel free to use them as well :)',
+    description="Welcome to Jeff Hansen's suite of useful python functions! I use lots of these functions on most of my Data Analysis, Backend-Dev, and Machine Learning projects, and I hope you find some of them useful as well!",
     package_dir={"": "src"},
     packages = find_packages(where="src"),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
```

### Comparing `jeffutils-0.6.9/src/jeffutils/utils.py` & `jeffutils-0.7.0/src/jeffutils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -630,15 +630,15 @@
     reimport file_2, then the changes in file_1 will not be reflected in file_2. You must reimport
     both file_1 and file_2 to see the changes in file_1 reflected in file_2.
        
     """
     ##########################
     # inner helper functions #
     ##########################
-    
+
     def _import_one(module:str):
         """ takes in a string like 'random' or 'numpy as np' and imports that
         module with its alias if given
         """
         if ' as ' in module:
             module_name, alias = module.split(' as ')
             module_name = module_name.strip()
@@ -680,29 +680,35 @@
             if alias:
                 globals()[alias] = getattr(module_obj, func_name)
             else:
                 globals()[func_name] = getattr(module_obj, func_name)
         else:
             raise AttributeError(f"Function {func_name} not found in module {module}")
         
-    def _get_sub_modules(module_path:str):
-        """ takes in a module_path like directory.sub_directory and returns a 
+    def _get_sub_modules(package_path:str):
+        """ takes in a package_path like directory.sub_directory and returns a 
         string of all of the modules in that directory like ['directory.sub_directory.module1',
         'directory.sub_directory.module2', ...]
         """
-        module_obj = _import_one(module_path)
+        module_obj = _import_one(package_path)
         if not hasattr(module_obj, "__path__"):
             return []
         
         return [
             module_info.name
             for module_info in pkgutil.walk_packages(module_obj.__path__, module_obj.__name__ + ".")
         ]
-    
+
     def _get_type_as_str(parent_module, name):
+        """ returns 'module' if the name is a module/package, 'function' if the name
+        is a function inside the parent_module.py file, and '*' if the name is a wildcard
+        import like 'from module import *'
+        """
+        if name.strip() == "*":
+            return "*"
         
         if isinstance(parent_module, str):
             parent_module_obj = sys.modules[parent_module]
         else:
             parent_module_obj = parent_module
         
         # if there is an alias in the name, remove it
@@ -712,22 +718,38 @@
         # modules inside of them. Modules with functions, do have string attributes
         # for each of their functions
         full_path = f"{parent_module_obj.__name__}.{main_portion}"
         if full_path in _get_sub_modules(parent_module):
             return "module"
         else:
             return "function"
+        
+    def _import_all_sub_funcs(module):
+        """ handles a situation like from module_name import * where it imports
+        all of the functions inside the module_name.py file """
+        if module not in sys.modules:
+            raise AttributeError(f"Module {module} not found in sys.modules")
+        module_obj = sys.modules[module]
+        
+        for func_name in dir(module_obj):
+            if not func_name.startswith("_"):
+                globals()[func_name] = getattr(module_obj, func_name)
 
     def _import_sub_module_component(parent_module, sub_component):
+        """ handles a situation like 'from parent_module import sub_component' whether
+        that sub_component is another package/module, function or the '*' wildcard
+        """
         sub_component_type = _get_type_as_str(parent_module, sub_component)
         if sub_component_type == 'module':
             full_module_name = f"{parent_module}.{sub_component}"
             _import_one(full_module_name)
         elif sub_component_type == 'function':
             _import_sub_func(parent_module, sub_component)
+        elif sub_component_type == '*':
+            _import_all_sub_funcs(parent_module)
         else:
             print(f"Unknown type: {sub_component_type}")
             
     def _import_module_hierarchy(module_path:str):
         """ This takes in a module_path like 'directory.sub_directory.module_name'
         and imports all the modules in the hierarchy like directory, 
         director.sub_directory, director.sub_directory.module_name
@@ -759,15 +781,20 @@
         """ takes in a single import statement like 'import numpy as np' or 'from random import choice'
         and imports the module or function
         """
         # remove whitespace at the start and end of the import statement
         import_statement = import_statement.strip()
         
         # extract all of the modules names ('os', 'numpy as np', 'jeffutils.utils', 'stack_trace')
-        module_re = re.compile(r"(\b(?!(?:import|from|as))[a-zA-Z0-9._]+\b\sas\s\b(?!(?:import|from|as))[a-zA-Z0-9._]+\b|\b(?!(?:import|from|as))[a-zA-Z0-9._]+\b)")
+        module_re = re.compile(
+            r"("
+                r"\b(?!(?:import|from|as))[a-zA-Z0-9._]+\b\sas\s\b(?!(?:import|from|as))[a-zA-Z0-9._]+\b|"
+                r"\b(?!(?:import|from|as))[a-zA-Z0-9._]+\b|"
+                r"(?!(?:import))[*]"
+            r")")
         module_names = module_re.findall(import_statement)
         
         # if a vanilla import statement, import each module
         if import_statement.startswith("import"):
             for module_name in module_names:
                 _import_one(module_name)
             
@@ -925,15 +952,15 @@
     finally:
         conn.close()
         
     if verbose:
         for table_name, col_names in table_info.items():
             print(f'{table_name}:', ", ".join(map(str, col_names)))
             
-    return table_info
+    return dict(table_info)
 
 def get_unique_counts(path_db, table_name, ref_col, cols):
     """
     Retrieve the count of unique values for specified columns grouped by a reference column from a SQLite table.
 
     Args:
         path_db (str): Path to the SQLite database file.
```

