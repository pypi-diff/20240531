# Comparing `tmp/pyson_data-0.1.3.tar.gz` & `tmp/pyson_data-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyson_data-0.1.3.tar", last modified: Thu May 16 16:51:44 2024, max compression
+gzip compressed data, was "pyson_data-0.2.0.tar", last modified: Fri May 31 13:37:51 2024, max compression
```

## Comparing `pyson_data-0.1.3.tar` & `pyson_data-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:51:44.565463 pyson_data-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-16 16:51:40.000000 pyson_data-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-16 16:51:44.565463 pyson_data-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-16 16:51:40.000000 pyson_data-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-16 16:51:40.000000 pyson_data-0.1.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:51:44.565463 pyson_data-0.1.3/pyson_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-16 16:51:44.000000 pyson_data-0.1.3/pyson_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-16 16:51:44.000000 pyson_data-0.1.3/pyson_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 16:51:44.000000 pyson_data-0.1.3/pyson_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 16:51:44.000000 pyson_data-0.1.3/pyson_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 16:51:44.565463 pyson_data-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-16 16:51:40.000000 pyson_data-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:37:51.186326 pyson_data-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-31 13:37:46.000000 pyson_data-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-31 13:37:51.186326 pyson_data-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-31 13:37:46.000000 pyson_data-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-31 13:37:46.000000 pyson_data-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:37:51.186326 pyson_data-0.2.0/pyson_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-31 13:37:51.000000 pyson_data-0.2.0/pyson_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-31 13:37:51.000000 pyson_data-0.2.0/pyson_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:37:51.000000 pyson_data-0.2.0/pyson_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:37:51.000000 pyson_data-0.2.0/pyson_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 13:37:51.186326 pyson_data-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-31 13:37:46.000000 pyson_data-0.2.0/setup.py
```

### Comparing `pyson_data-0.1.3/LICENSE` & `pyson_data-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyson_data-0.1.3/PKG-INFO` & `pyson_data-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 Metadata-Version: 2.1
 Name: pyson_data
-Version: 0.1.3
-Summary: Pyson package for .pyson data format support
+Version: 0.2.0
+Summary: Package for .pyson data format support
 Home-page: https://github.com/OmegaGodzilla66/PYSON
 Author: josh-co-dev
 Author-email: josh-co <omegaraspberrypi@gmail.com>
-Project-URL: Homepage, https://github.com/ProbablyComputingSquid/PYSON/
-Project-URL: Issues, https://github.com/ProbablyComputingSquid/PYSON/issues
+Project-URL: Homepage, https://github.com/OmegaGodzilla66/PYSON/
+Project-URL: Issues, https://github.com/OmegaGodzilla66/PYSON/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PYSON #
 ##### Maintained by: [OmegaGodzilla66](https://github.com/OmegaGodzilla66), [ComputingSquid](https://github.com/ProbablyComputingSquid), [CoolSchnoodle](https://github.com/CoolSchnoodle), and [nmd102](https://github.com/nmd102) #####
 
+![GitHub Repo stars](https://img.shields.io/github/stars/OmegaGodzilla66/PYSON)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/OmegaGodzilla66/PYSON/python-publish.yml)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/t/OmegaGodzilla66/PYSON)
+![GitHub last commit](https://img.shields.io/github/last-commit/OmegaGodzilla66/PYSON)
+![GitHub Release](https://img.shields.io/github/v/release/OmegaGodzilla66/PYSON)
+![GitHub commits since latest release](https://img.shields.io/github/commits-since/OmegaGodzilla66/PYSON/latest)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pyson-data)
+
+
 
 ## Overview ##
 The purpose of this project is to provide a python-based alternative to JSON. This is a (almost) fully functional JSON-inspired data management system!
 
 ## How to Use ##
 This is a pip package, so to use this in python you can just `pip install pyson-data`.
 From there, you can just `import pyson_data as pyson`.
@@ -31,28 +40,35 @@
 
 ## Documentation ##
 Documentation has also been moved to the project wiki [here](https://github.com/OmegaGodzilla66/PYSON/wiki) to decrease clutter in the README.
 
 ## Supported Types ##
 There are 4 supported types: int, float, str, and list
 <br><br>
-- An int is a whole number that can be any valu
-- A str is a list of text (quotes not required)
-- A list is a list of values, which currently have to all be strings. List items are seperated by the (*) seperator.
-Currently there is no escaping support. I don't really know why you would use that value normally in a list.
+- An int is a whole number
+- A str is some text
+- A list is a list of values, which currently have to all be strings.
+  List items are seperated by the (*) seperator.
+  Currently there is no escaping support.
+  I don't really know why you would use (\*) normally in a list.
 - A float is a decimal number, that can be any value representable by a 64-bit floating point number.
 <br>More supported types may be added  at some point in the future. 
 
 ## Changelog ##
+- v0.2.0: Full rewrite, code is now much more organized.
+  Not all convenience features are back yet but it is overall much more usable
 - v0.1.3: Added getDict function
 - v0.1.2: Refactored pyson.py
 - v0.1.1: Added writeMultiple function, various bug fixes
-- v0.1.0-alpha: package & release deployed to pypi, merged code to main, and resolved all merge conflicts! truly a cause for celebration 🎉
+- v0.1.0-alpha: package & release deployed to pypi, merged code to main, and resolved all merge conflicts!
+  truly a cause for celebration 🎉
 - v0.0.9: coolSchnoodle and nmd102 made code fixes and README fixes
 - v0.0.8: Added updateData function
 - v0.0.7: Fixed errors, refactored bad code
 - v0.0.6: Added floats
 - v0.0.5: Updated naming system, ported to github!
-- v0.0.4: Added a function that checks if a file is compatible with .pyson file format. Fixed a bug in the write. Other general bug fixes.
+- v0.0.4: Added a function that checks if a file is compatible with .pyson file format.
+  Fixed a bug in the write. Other general bug fixes.
 - v0.0.3: Added a write function! This is now (technically) fully functional!
 - v0.0.2: Added a read function for the whole file. Returns a list of all contents.
-- v0.0.1: Initial launch! Basic reading features for a .cnf (renamed almost immediately to pyson) file. Current compatible types are string, int, and list.
+- v0.0.1: Initial launch! Basic reading features for a .cnf (renamed almost immediately to pyson) file.
+  Current compatible types are string, int, and list.
```

### Comparing `pyson_data-0.1.3/README.md` & `pyson_data-0.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 # PYSON #
 ##### Maintained by: [OmegaGodzilla66](https://github.com/OmegaGodzilla66), [ComputingSquid](https://github.com/ProbablyComputingSquid), [CoolSchnoodle](https://github.com/CoolSchnoodle), and [nmd102](https://github.com/nmd102) #####
 
+![GitHub Repo stars](https://img.shields.io/github/stars/OmegaGodzilla66/PYSON)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/OmegaGodzilla66/PYSON/python-publish.yml)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/t/OmegaGodzilla66/PYSON)
+![GitHub last commit](https://img.shields.io/github/last-commit/OmegaGodzilla66/PYSON)
+![GitHub Release](https://img.shields.io/github/v/release/OmegaGodzilla66/PYSON)
+![GitHub commits since latest release](https://img.shields.io/github/commits-since/OmegaGodzilla66/PYSON/latest)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pyson-data)
+
+
 
 ## Overview ##
 The purpose of this project is to provide a python-based alternative to JSON. This is a (almost) fully functional JSON-inspired data management system!
 
 ## How to Use ##
 This is a pip package, so to use this in python you can just `pip install pyson-data`.
 From there, you can just `import pyson_data as pyson`.
@@ -15,28 +24,35 @@
 
 ## Documentation ##
 Documentation has also been moved to the project wiki [here](https://github.com/OmegaGodzilla66/PYSON/wiki) to decrease clutter in the README.
 
 ## Supported Types ##
 There are 4 supported types: int, float, str, and list
 <br><br>
-- An int is a whole number that can be any valu
-- A str is a list of text (quotes not required)
-- A list is a list of values, which currently have to all be strings. List items are seperated by the (*) seperator.
-Currently there is no escaping support. I don't really know why you would use that value normally in a list.
+- An int is a whole number
+- A str is some text
+- A list is a list of values, which currently have to all be strings.
+  List items are seperated by the (*) seperator.
+  Currently there is no escaping support.
+  I don't really know why you would use (\*) normally in a list.
 - A float is a decimal number, that can be any value representable by a 64-bit floating point number.
 <br>More supported types may be added  at some point in the future. 
 
 ## Changelog ##
+- v0.2.0: Full rewrite, code is now much more organized.
+  Not all convenience features are back yet but it is overall much more usable
 - v0.1.3: Added getDict function
 - v0.1.2: Refactored pyson.py
 - v0.1.1: Added writeMultiple function, various bug fixes
-- v0.1.0-alpha: package & release deployed to pypi, merged code to main, and resolved all merge conflicts! truly a cause for celebration 🎉
+- v0.1.0-alpha: package & release deployed to pypi, merged code to main, and resolved all merge conflicts!
+  truly a cause for celebration 🎉
 - v0.0.9: coolSchnoodle and nmd102 made code fixes and README fixes
 - v0.0.8: Added updateData function
 - v0.0.7: Fixed errors, refactored bad code
 - v0.0.6: Added floats
 - v0.0.5: Updated naming system, ported to github!
-- v0.0.4: Added a function that checks if a file is compatible with .pyson file format. Fixed a bug in the write. Other general bug fixes.
+- v0.0.4: Added a function that checks if a file is compatible with .pyson file format.
+  Fixed a bug in the write. Other general bug fixes.
 - v0.0.3: Added a write function! This is now (technically) fully functional!
 - v0.0.2: Added a read function for the whole file. Returns a list of all contents.
-- v0.0.1: Initial launch! Basic reading features for a .cnf (renamed almost immediately to pyson) file. Current compatible types are string, int, and list.
+- v0.0.1: Initial launch! Basic reading features for a .cnf (renamed almost immediately to pyson) file.
+  Current compatible types are string, int, and list.
```

### Comparing `pyson_data-0.1.3/pyson_data.egg-info/PKG-INFO` & `pyson_data-0.2.0/pyson_data.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 Metadata-Version: 2.1
 Name: pyson_data
-Version: 0.1.3
-Summary: Pyson package for .pyson data format support
+Version: 0.2.0
+Summary: Package for .pyson data format support
 Home-page: https://github.com/OmegaGodzilla66/PYSON
 Author: josh-co-dev
 Author-email: josh-co <omegaraspberrypi@gmail.com>
-Project-URL: Homepage, https://github.com/ProbablyComputingSquid/PYSON/
-Project-URL: Issues, https://github.com/ProbablyComputingSquid/PYSON/issues
+Project-URL: Homepage, https://github.com/OmegaGodzilla66/PYSON/
+Project-URL: Issues, https://github.com/OmegaGodzilla66/PYSON/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PYSON #
 ##### Maintained by: [OmegaGodzilla66](https://github.com/OmegaGodzilla66), [ComputingSquid](https://github.com/ProbablyComputingSquid), [CoolSchnoodle](https://github.com/CoolSchnoodle), and [nmd102](https://github.com/nmd102) #####
 
+![GitHub Repo stars](https://img.shields.io/github/stars/OmegaGodzilla66/PYSON)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/OmegaGodzilla66/PYSON/python-publish.yml)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/t/OmegaGodzilla66/PYSON)
+![GitHub last commit](https://img.shields.io/github/last-commit/OmegaGodzilla66/PYSON)
+![GitHub Release](https://img.shields.io/github/v/release/OmegaGodzilla66/PYSON)
+![GitHub commits since latest release](https://img.shields.io/github/commits-since/OmegaGodzilla66/PYSON/latest)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pyson-data)
+
+
 
 ## Overview ##
 The purpose of this project is to provide a python-based alternative to JSON. This is a (almost) fully functional JSON-inspired data management system!
 
 ## How to Use ##
 This is a pip package, so to use this in python you can just `pip install pyson-data`.
 From there, you can just `import pyson_data as pyson`.
@@ -31,28 +40,35 @@
 
 ## Documentation ##
 Documentation has also been moved to the project wiki [here](https://github.com/OmegaGodzilla66/PYSON/wiki) to decrease clutter in the README.
 
 ## Supported Types ##
 There are 4 supported types: int, float, str, and list
 <br><br>
-- An int is a whole number that can be any valu
-- A str is a list of text (quotes not required)
-- A list is a list of values, which currently have to all be strings. List items are seperated by the (*) seperator.
-Currently there is no escaping support. I don't really know why you would use that value normally in a list.
+- An int is a whole number
+- A str is some text
+- A list is a list of values, which currently have to all be strings.
+  List items are seperated by the (*) seperator.
+  Currently there is no escaping support.
+  I don't really know why you would use (\*) normally in a list.
 - A float is a decimal number, that can be any value representable by a 64-bit floating point number.
 <br>More supported types may be added  at some point in the future. 
 
 ## Changelog ##
+- v0.2.0: Full rewrite, code is now much more organized.
+  Not all convenience features are back yet but it is overall much more usable
 - v0.1.3: Added getDict function
 - v0.1.2: Refactored pyson.py
 - v0.1.1: Added writeMultiple function, various bug fixes
-- v0.1.0-alpha: package & release deployed to pypi, merged code to main, and resolved all merge conflicts! truly a cause for celebration 🎉
+- v0.1.0-alpha: package & release deployed to pypi, merged code to main, and resolved all merge conflicts!
+  truly a cause for celebration 🎉
 - v0.0.9: coolSchnoodle and nmd102 made code fixes and README fixes
 - v0.0.8: Added updateData function
 - v0.0.7: Fixed errors, refactored bad code
 - v0.0.6: Added floats
 - v0.0.5: Updated naming system, ported to github!
-- v0.0.4: Added a function that checks if a file is compatible with .pyson file format. Fixed a bug in the write. Other general bug fixes.
+- v0.0.4: Added a function that checks if a file is compatible with .pyson file format.
+  Fixed a bug in the write. Other general bug fixes.
 - v0.0.3: Added a write function! This is now (technically) fully functional!
 - v0.0.2: Added a read function for the whole file. Returns a list of all contents.
-- v0.0.1: Initial launch! Basic reading features for a .cnf (renamed almost immediately to pyson) file. Current compatible types are string, int, and list.
+- v0.0.1: Initial launch! Basic reading features for a .cnf (renamed almost immediately to pyson) file.
+  Current compatible types are string, int, and list.
```

### Comparing `pyson_data-0.1.3/setup.py` & `pyson_data-0.2.0/setup.py`

 * *Files identical despite different names*

