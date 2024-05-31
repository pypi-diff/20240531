# Comparing `tmp/xeus-python-shell-0.6.1.tar.gz` & `tmp/xeus_python_shell-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xeus-python-shell-0.6.1.tar", last modified: Thu Aug  3 14:28:38 2023, max compression
+gzip compressed data, was "xeus_python_shell-0.6.2.tar", last modified: Fri May 31 13:32:23 2024, max compression
```

## Comparing `xeus-python-shell-0.6.1.tar` & `xeus_python_shell-0.6.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-08-03 14:28:38.054923 xeus-python-shell-0.6.1/
--rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)     1518 2021-08-13 10:02:56.000000 xeus-python-shell-0.6.1/LICENSE
--rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)       16 2021-08-19 09:11:29.000000 xeus-python-shell-0.6.1/MANIFEST.in
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      852 2023-08-03 14:28:38.053923 xeus-python-shell-0.6.1/PKG-INFO
--rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)      101 2021-08-19 08:49:07.000000 xeus-python-shell-0.6.1/README.md
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)       38 2023-08-03 14:28:38.054923 xeus-python-shell-0.6.1/setup.cfg
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1144 2023-08-03 14:27:22.000000 xeus-python-shell-0.6.1/setup.py
-drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-08-03 14:28:38.050923 xeus-python-shell-0.6.1/xeus_python_shell/
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)        0 2022-08-05 13:17:28.000000 xeus-python-shell-0.6.1/xeus_python_shell/__init__.py
--rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)      587 2022-06-29 10:04:57.000000 xeus-python-shell-0.6.1/xeus_python_shell/compiler.py
--rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)     3805 2022-08-09 09:38:41.000000 xeus-python-shell-0.6.1/xeus_python_shell/debugger.py
--rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)     1383 2022-06-29 10:04:57.000000 xeus-python-shell-0.6.1/xeus_python_shell/display.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     3521 2023-08-03 14:27:05.000000 xeus-python-shell-0.6.1/xeus_python_shell/shell.py
-drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-08-03 14:28:38.053923 xeus-python-shell-0.6.1/xeus_python_shell.egg-info/
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      852 2023-08-03 14:28:38.000000 xeus-python-shell-0.6.1/xeus_python_shell.egg-info/PKG-INFO
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      388 2023-08-03 14:28:38.000000 xeus-python-shell-0.6.1/xeus_python_shell.egg-info/SOURCES.txt
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)        1 2023-08-03 14:28:38.000000 xeus-python-shell-0.6.1/xeus_python_shell.egg-info/dependency_links.txt
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)       73 2023-08-03 14:28:38.000000 xeus-python-shell-0.6.1/xeus_python_shell.egg-info/requires.txt
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)       18 2023-08-03 14:28:38.000000 xeus-python-shell-0.6.1/xeus_python_shell.egg-info/top_level.txt
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2024-05-31 13:32:23.579568 xeus_python_shell-0.6.2/
+-rw-r--r--   0 martin    (1000) martin    (1000)     1518 2024-05-31 13:31:00.000000 xeus_python_shell-0.6.2/LICENSE
+-rw-r--r--   0 martin    (1000) martin    (1000)       16 2024-05-31 13:31:00.000000 xeus_python_shell-0.6.2/MANIFEST.in
+-rw-r--r--   0 martin    (1000) martin    (1000)      988 2024-05-31 13:32:23.579568 xeus_python_shell-0.6.2/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)      101 2024-05-31 13:31:00.000000 xeus_python_shell-0.6.2/README.md
+-rw-r--r--   0 martin    (1000) martin    (1000)       38 2024-05-31 13:32:23.579568 xeus_python_shell-0.6.2/setup.cfg
+-rw-r--r--   0 martin    (1000) martin    (1000)     1144 2024-05-31 13:31:52.000000 xeus_python_shell-0.6.2/setup.py
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2024-05-31 13:32:23.578568 xeus_python_shell-0.6.2/xeus_python_shell/
+-rw-r--r--   0 martin    (1000) martin    (1000)        0 2024-05-31 13:31:00.000000 xeus_python_shell-0.6.2/xeus_python_shell/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      587 2024-05-31 13:31:00.000000 xeus_python_shell-0.6.2/xeus_python_shell/compiler.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     3805 2024-05-31 13:31:00.000000 xeus_python_shell-0.6.2/xeus_python_shell/debugger.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     1383 2024-05-31 13:31:00.000000 xeus_python_shell-0.6.2/xeus_python_shell/display.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     3584 2024-05-31 13:31:01.000000 xeus_python_shell-0.6.2/xeus_python_shell/shell.py
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2024-05-31 13:32:23.578568 xeus_python_shell-0.6.2/xeus_python_shell.egg-info/
+-rw-r--r--   0 martin    (1000) martin    (1000)      988 2024-05-31 13:32:23.000000 xeus_python_shell-0.6.2/xeus_python_shell.egg-info/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)      388 2024-05-31 13:32:23.000000 xeus_python_shell-0.6.2/xeus_python_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)        1 2024-05-31 13:32:23.000000 xeus_python_shell-0.6.2/xeus_python_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)       73 2024-05-31 13:32:23.000000 xeus_python_shell-0.6.2/xeus_python_shell.egg-info/requires.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)       18 2024-05-31 13:32:23.000000 xeus_python_shell-0.6.2/xeus_python_shell.egg-info/top_level.txt
```

### Comparing `xeus-python-shell-0.6.1/LICENSE` & `xeus_python_shell-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xeus-python-shell-0.6.1/PKG-INFO` & `xeus_python_shell-0.6.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeus-python-shell
-Version: 0.6.1
+Version: 0.6.2
 Summary: The xeus-python core python logic.
 Home-page: https://github.com/jupyter-xeus/xeus-python-shell
 Author: QuantStack dev team
 Maintainer: QuantStack dev team
 License: BSD 3-Clause
 Keywords: python ipython xeus-python
 Platform: any
@@ -14,10 +14,13 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
+License-File: LICENSE
+Requires-Dist: debugpy<2,>=1.1.0
 Provides-Extra: ipython
+Requires-Dist: ipython<9,>=7.21; extra == "ipython"
 Provides-Extra: wasm
-License-File: LICENSE
+Requires-Dist: pyjs<2.0.0,>=1.1.0; extra == "wasm"
```

### Comparing `xeus-python-shell-0.6.1/setup.py` & `xeus_python_shell-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 __AUTHOR__ = 'QuantStack dev team'
 
 setup(
     name='xeus-python-shell',
-    version='0.6.1',
+    version='0.6.2',
     description='The xeus-python core python logic.',
     author=__AUTHOR__,
     maintainer=__AUTHOR__,
     url='https://github.com/jupyter-xeus/xeus-python-shell',
     license='BSD 3-Clause',
     keywords='python ipython xeus-python',
     packages=find_packages(exclude=['test']),
```

### Comparing `xeus-python-shell-0.6.1/xeus_python_shell/compiler.py` & `xeus_python_shell-0.6.2/xeus_python_shell/compiler.py`

 * *Files identical despite different names*

### Comparing `xeus-python-shell-0.6.1/xeus_python_shell/debugger.py` & `xeus_python_shell-0.6.2/xeus_python_shell/debugger.py`

 * *Files identical despite different names*

### Comparing `xeus-python-shell-0.6.1/xeus_python_shell/display.py` & `xeus_python_shell-0.6.2/xeus_python_shell/display.py`

 * *Files identical despite different names*

### Comparing `xeus-python-shell-0.6.1/xeus_python_shell/shell.py` & `xeus_python_shell-0.6.2/xeus_python_shell/shell.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 
     def __init__(self, shell=None, config=None, **traits):
         self.enabled = False
         super(LiteHistoryManager, self).__init__(shell=shell, config=config, **traits)
 
 
 class XPythonShell(InteractiveShell):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, use_jedi, *args, **kwargs):
         super(XPythonShell, self).__init__(*args, **kwargs)
 
         self.kernel = None
-        self.Completer.use_jedi = False
+        self.Completer.use_jedi = use_jedi
 
     def enable_gui(self, gui=None):
         """Not implemented yet."""
         pass
 
     def init_hooks(self):
         super(XPythonShell, self).init_hooks()
@@ -72,36 +72,37 @@
             cursor_end = cursor_pos
             matches = []
 
         return matches, cursor_start, cursor_end
 
 
 class XPythonShellApp(BaseIPythonApplication, InteractiveShellApp):
-    def initialize(self, argv=None):
+    def initialize(self, use_jedi, argv=None):
         super(XPythonShellApp, self).initialize(argv)
 
         self.user_ns = {}
 
         # self.init_io() ?
 
         self.init_path()
-        self.init_shell()
+        self.init_shell(use_jedi)
 
         if not os.environ.get("MPLBACKEND"):
             os.environ["MPLBACKEND"] = "module://matplotlib_inline.backend_inline"
         self.init_gui_pylab()
 
         self.init_extensions()
         self.init_code()
 
         sys.stdout.flush()
         sys.stderr.flush()
 
-    def init_shell(self):
+    def init_shell(self, use_jedi):
         self.shell = XPythonShell.instance(
+            use_jedi,
             display_pub_class=XDisplayPublisher,
             displayhook_class=XDisplayHook,
             compiler_class=XCachingCompiler,
             user_ns=self.user_ns,
         )
 
     # Overwrite exit logic, this is not part of the kernel protocol
```

### Comparing `xeus-python-shell-0.6.1/xeus_python_shell.egg-info/PKG-INFO` & `xeus_python_shell-0.6.2/xeus_python_shell.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeus-python-shell
-Version: 0.6.1
+Version: 0.6.2
 Summary: The xeus-python core python logic.
 Home-page: https://github.com/jupyter-xeus/xeus-python-shell
 Author: QuantStack dev team
 Maintainer: QuantStack dev team
 License: BSD 3-Clause
 Keywords: python ipython xeus-python
 Platform: any
@@ -14,10 +14,13 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
+License-File: LICENSE
+Requires-Dist: debugpy<2,>=1.1.0
 Provides-Extra: ipython
+Requires-Dist: ipython<9,>=7.21; extra == "ipython"
 Provides-Extra: wasm
-License-File: LICENSE
+Requires-Dist: pyjs<2.0.0,>=1.1.0; extra == "wasm"
```

