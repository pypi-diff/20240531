# Comparing `tmp/tersel-0.0.2.tar.gz` & `tmp/tersel-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tersel-0.0.2.tar", last modified: Wed May 29 15:10:56 2024, max compression
+gzip compressed data, was "tersel-0.0.3.tar", last modified: Fri May 31 12:13:53 2024, max compression
```

## Comparing `tersel-0.0.2.tar` & `tersel-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:10:56.504281 tersel-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    20848 2024-05-29 15:10:42.000000 tersel-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-29 15:10:56.504281 tersel-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-29 15:10:42.000000 tersel-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-29 15:10:42.000000 tersel-0.0.2/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 15:10:56.504281 tersel-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 15:10:42.000000 tersel-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:10:56.504281 tersel-0.0.2/tersel/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-29 15:10:42.000000 tersel-0.0.2/tersel/Option.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-29 15:10:42.000000 tersel-0.0.2/tersel/OptionList.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-29 15:10:42.000000 tersel-0.0.2/tersel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:10:56.504281 tersel-0.0.2/tersel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-29 15:10:56.000000 tersel-0.0.2/tersel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-29 15:10:56.000000 tersel-0.0.2/tersel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:10:56.000000 tersel-0.0.2/tersel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-29 15:10:56.000000 tersel-0.0.2/tersel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 15:10:56.000000 tersel-0.0.2/tersel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:13:53.863292 tersel-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    20848 2024-05-31 12:13:39.000000 tersel-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-31 12:13:53.863292 tersel-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-31 12:13:39.000000 tersel-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-31 12:13:39.000000 tersel-0.0.3/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 12:13:53.863292 tersel-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 12:13:39.000000 tersel-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:13:53.859292 tersel-0.0.3/tersel/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-31 12:13:39.000000 tersel-0.0.3/tersel/Option.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-31 12:13:39.000000 tersel-0.0.3/tersel/OptionList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-31 12:13:39.000000 tersel-0.0.3/tersel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:13:53.863292 tersel-0.0.3/tersel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-31 12:13:53.000000 tersel-0.0.3/tersel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-31 12:13:53.000000 tersel-0.0.3/tersel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 12:13:53.000000 tersel-0.0.3/tersel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-31 12:13:53.000000 tersel-0.0.3/tersel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-31 12:13:53.000000 tersel-0.0.3/tersel.egg-info/top_level.txt
```

### Comparing `tersel-0.0.2/LICENSE` & `tersel-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tersel-0.0.2/PKG-INFO` & `tersel-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: tersel
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library for easily implementing selection prompts in the terminal
 Author-email: Thijn Smulders <thijnsmulders04@gmail.com>
 License: CC BY-NC-SA 4.0
 Project-URL: github, https://github.com/thijnmens/tersel
 Keywords: terminal,cli,selection
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.12
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: colorama~=0.4.6
 Requires-Dist: keyboard~=0.13.5
 
 # Tersel
```

### Comparing `tersel-0.0.2/pyproject.toml` & `tersel-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = 'tersel'
 authors = [
     { name = 'Thijn Smulders', email = 'thijnsmulders04@gmail.com' }
 ]
 description = 'A library for easily implementing selection prompts in the terminal'
 readme = 'readme.md'
-requires-python = '>=3.12'
+requires-python = '>=3.10'
 keywords = ['terminal', 'cli', 'selection']
 license = { text = 'CC BY-NC-SA 4.0' }
 classifiers = [
     'Environment :: Console',
     'Programming Language :: Python :: 3.12',
     'Operating System :: Microsoft :: Windows',
     'Operating System :: Unix',
@@ -23,8 +23,8 @@
     'colorama~=0.4.6',
     'keyboard~=0.13.5'
 ]
 dynamic = ["version"]
 urls = { github = 'https://github.com/thijnmens/tersel' }
 
 [tool.setuptools.dynamic]
-version = { attr = "tersel.VERSION" }
+version = { attr = "tersel.VERSION" }
```

### Comparing `tersel-0.0.2/tersel/OptionList.py` & `tersel-0.0.3/tersel/OptionList.py`

 * *Files identical despite different names*

### Comparing `tersel-0.0.2/tersel/__init__.py` & `tersel-0.0.3/tersel/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import keyboard
 from colorama import Fore, Style
 from colorama import init as colorama_init
 
 from tersel.Option import Option
 from tersel.OptionList import OptionList
 
-VERSION: str = "0.0.2"
+VERSION: str = "0.0.3"
 Option = Option
 OptionList = OptionList
 
 
 class Tersel:
     def __init__(self, title: str, options: [any], max_options_shown: int = 5, line_start: str = "[{index}] ",
                  title_color: str = Fore.GREEN, option_color: str = Fore.LIGHTBLACK_EX,
```

### Comparing `tersel-0.0.2/tersel.egg-info/PKG-INFO` & `tersel-0.0.3/tersel.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: tersel
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library for easily implementing selection prompts in the terminal
 Author-email: Thijn Smulders <thijnsmulders04@gmail.com>
 License: CC BY-NC-SA 4.0
 Project-URL: github, https://github.com/thijnmens/tersel
 Keywords: terminal,cli,selection
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.12
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: colorama~=0.4.6
 Requires-Dist: keyboard~=0.13.5
 
 # Tersel
```

