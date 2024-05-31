# Comparing `tmp/jeffutils-0.8.0.tar.gz` & `tmp/jeffutils-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeffutils-0.8.0.tar", last modified: Fri May 31 17:35:33 2024, max compression
+gzip compressed data, was "jeffutils-0.8.1.tar", last modified: Fri May 31 20:45:45 2024, max compression
```

## Comparing `jeffutils-0.8.0.tar` & `jeffutils-0.8.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:35:33.461742 jeffutils-0.8.0/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.8.0/LICENSE.txt
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      576 2024-05-31 17:35:33.461742 jeffutils-0.8.0/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     2685 2024-05-31 17:04:40.000000 jeffutils-0.8.0/README.md
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.8.0/pyproject.toml
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-31 17:35:33.461742 jeffutils-0.8.0/setup.cfg
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      715 2024-05-31 17:35:32.000000 jeffutils-0.8.0/setup.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:35:33.461742 jeffutils-0.8.0/src/
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:35:33.461742 jeffutils-0.8.0/src/jeffutils/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.8.0/src/jeffutils/__init__.py
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    37827 2024-05-31 17:05:48.000000 jeffutils-0.8.0/src/jeffutils/utils.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 17:35:33.461742 jeffutils-0.8.0/src/jeffutils.egg-info/
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      576 2024-05-31 17:35:33.000000 jeffutils-0.8.0/src/jeffutils.egg-info/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-31 17:35:33.000000 jeffutils-0.8.0/src/jeffutils.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-31 17:35:33.000000 jeffutils-0.8.0/src/jeffutils.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-31 17:35:33.000000 jeffutils-0.8.0/src/jeffutils.egg-info/top_level.txt
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 20:45:45.724649 jeffutils-0.8.1/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.8.1/LICENSE.txt
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      576 2024-05-31 20:45:45.724649 jeffutils-0.8.1/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     2685 2024-05-31 17:04:40.000000 jeffutils-0.8.1/README.md
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.8.1/pyproject.toml
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-31 20:45:45.724649 jeffutils-0.8.1/setup.cfg
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      715 2024-05-31 20:45:43.000000 jeffutils-0.8.1/setup.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 20:45:45.724649 jeffutils-0.8.1/src/
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 20:45:45.724649 jeffutils-0.8.1/src/jeffutils/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.8.1/src/jeffutils/__init__.py
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    38677 2024-05-31 20:45:13.000000 jeffutils-0.8.1/src/jeffutils/utils.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-31 20:45:45.724649 jeffutils-0.8.1/src/jeffutils.egg-info/
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      576 2024-05-31 20:45:45.000000 jeffutils-0.8.1/src/jeffutils.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-31 20:45:45.000000 jeffutils-0.8.1/src/jeffutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-31 20:45:45.000000 jeffutils-0.8.1/src/jeffutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-31 20:45:45.000000 jeffutils-0.8.1/src/jeffutils.egg-info/top_level.txt
```

### Comparing `jeffutils-0.8.0/LICENSE.txt` & `jeffutils-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jeffutils-0.8.0/PKG-INFO` & `jeffutils-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeffutils
-Version: 0.8.0
+Version: 0.8.1
 Summary: Welcome to Jeff Hansen's suite of useful python functions! I use lots of these functions on most of my Data Analysis, Backend-Dev, and Machine Learning projects, and I hope you find some of them useful as well!
 Home-page: https://github.com/jeffxhansen/jeffutils
 Author: Jeff Hansen
 Author-email: jeffxhansen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jeffutils-0.8.0/README.md` & `jeffutils-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `jeffutils-0.8.0/setup.py` & `jeffutils-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='jeffutils',
-    version='0.8.0',
+    version='0.8.1',
     author='Jeff Hansen',
     author_email='jeffxhansen@gmail.com',
     description="Welcome to Jeff Hansen's suite of useful python functions! I use lots of these functions on most of my Data Analysis, Backend-Dev, and Machine Learning projects, and I hope you find some of them useful as well!",
     package_dir={"": "src"},
     packages = find_packages(where="src"),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `jeffutils-0.8.0/src/jeffutils/utils.py` & `jeffutils-0.8.1/src/jeffutils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -174,15 +174,15 @@
     return string
 
 def initialize_log_func_vars_func(LOG_TOGGLE):
     """ returns a function that will log the variables of a function
     with the LOG_TOGGLE dictionary set to LOG_TOGGLE
     """
     def log_func_vars_func(func_name, vars, globals, locals, header=True):
-        return log_func_vars(func_name, vars, globals, locals, header=header, LOG_TOGGLE=LOG_TOGGLE)
+        return log_func_vars(func_name, vars, globals, locals, header=header, only_log=LOG_TOGGLE)
     
     return log_func_vars_func
             
 def format_perc(perc):
     """takes in a percentage as a decimal and formats it
     in the form of +x.xx% or -x.xx%
     """
@@ -473,55 +473,74 @@
         d2 = deepcopy(d)
         d2.update(d_)
         return d2
     else:
         d.update(d_)
 
 
-def time_function(func, *args, **kwargs):
+def time_function(func, args=None, kwargs=None, output_directory=None):
     """takes in a function, its argument, and its keyword arguments. It runs this function
-    and outputs the cProfile timing analysis in the kwargs['output_path'] file. If no 'output_path'
-    in the keyword arguments, then it will just save it to a file called time_output_<func_name> in
+    and outputs the cProfile timing analysis in the 'output_directory' file. If no 'output_directory'
+    is provided, then it will just save it to a file called time_<func_name> in
     the current directory.
     
     example: 
-      time_function(your_function, arg1, arg2, kwarg1=kwarg1, kwarg2=kwarg2, output_path="path/to/file/"))
+      time_function(your_function, args=(arg1, arg2,), kwargs={'kwarg1':kwarg1, 'kwarg2':kwarg2}, output_directory="path/to/file/"))
     """
+    # setup where the output will be saved
     output_name = f"time_{func.__name__}"
-    if 'output_path' in kwargs:
-        output_path = kwargs['output_path'] + output_name
-        del kwargs['output_path']
+    if output_directory is not None:
+        output_path_dir = os.path.dirname(output_directory)
+        output_path = os.path.join(output_path_dir, output_name)
     else:
         output_path = output_name
+    # make sure the directory for the output_path exists
+    output_dir = os.path.dirname(output_path)
+    if not os.path.exists(output_dir):
+        os.makedirs(output_dir)
         
+    # run the function and save the cProfile timing analysis
     try:
         pr = cProfile.Profile()
         pr.enable()
-        func(*args, **kwargs)
+        if args is not None and kwargs is not None:
+            func(*args, **kwargs)
+        elif args is not None:
+            func(*args)
+        elif kwargs is not None:
+            func(**kwargs)
+        else:
+            func()
+    
+    # make sure that it still outputs the cProfile timing analysis even if the function
+    # is interrupted by a KeyboardInterrupt
     except KeyboardInterrupt as ke:
         pass
     finally:
+        # the cProfile has to go to a .prof file
         pr.disable()
         prof_path = output_path + '.prof'
         text_path = output_path + '.txt'
         with open(prof_path, 'w+') as file:
             file.write("")
         pr.dump_stats(prof_path)
 
+        # load the .prof file into a text file
         s = io.StringIO()
         ps = pstats.Stats(pr, stream=s)
         ps.strip_dirs()
         ps.sort_stats('cumulative')
         ps.print_stats()
         
         print(f"Saving a record of how long {func.__name__} took to run in {output_path}.txt")
 
         with open(text_path, 'w+') as file:
             file.write(s.getvalue())
             
+        # remove the .prof path since it is no longer needed
         if os.path.exists(prof_path):
             os.remove(prof_path)
 
             
 def print_skip_exceptions(full_stack_trace=True, log_error=True):
     """ a decorator that will just print an exception thrown
     by the function without raising it up the call stack
```

### Comparing `jeffutils-0.8.0/src/jeffutils.egg-info/PKG-INFO` & `jeffutils-0.8.1/src/jeffutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeffutils
-Version: 0.8.0
+Version: 0.8.1
 Summary: Welcome to Jeff Hansen's suite of useful python functions! I use lots of these functions on most of my Data Analysis, Backend-Dev, and Machine Learning projects, and I hope you find some of them useful as well!
 Home-page: https://github.com/jeffxhansen/jeffutils
 Author: Jeff Hansen
 Author-email: jeffxhansen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

