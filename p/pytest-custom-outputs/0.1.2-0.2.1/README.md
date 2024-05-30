# Comparing `tmp/pytest_custom_outputs-0.1.2.tar.gz` & `tmp/pytest_custom_outputs-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_custom_outputs-0.1.2.tar", last modified: Thu May 30 00:57:34 2024, max compression
+gzip compressed data, was "pytest_custom_outputs-0.2.1.tar", last modified: Thu May 30 22:27:16 2024, max compression
```

## Comparing `pytest_custom_outputs-0.1.2.tar` & `pytest_custom_outputs-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-30 00:57:34.619867 pytest_custom_outputs-0.1.2/
--rw-r--r--   0 user      (1000) vboxusers   (136)     1501 2024-04-09 20:33:50.000000 pytest_custom_outputs-0.1.2/LICENSE
--rw-r--r--   0 user      (1000) vboxusers   (136)     9608 2024-05-30 00:57:34.619867 pytest_custom_outputs-0.1.2/PKG-INFO
--rw-r--r--   0 user      (1000) vboxusers   (136)     6612 2024-05-30 00:56:50.000000 pytest_custom_outputs-0.1.2/README.rst
--rw-r--r--   0 user      (1000) vboxusers   (136)     1490 2024-05-30 00:57:28.000000 pytest_custom_outputs-0.1.2/pyproject.toml
--rw-r--r--   0 user      (1000) vboxusers   (136)       38 2024-05-30 00:57:34.619867 pytest_custom_outputs-0.1.2/setup.cfg
-drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-30 00:57:34.619867 pytest_custom_outputs-0.1.2/src/
-drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-30 00:57:34.619867 pytest_custom_outputs-0.1.2/src/pytest_custom_outputs/
--rw-r--r--   0 user      (1000) vboxusers   (136)        0 2024-04-09 20:33:50.000000 pytest_custom_outputs-0.1.2/src/pytest_custom_outputs/__init__.py
--rw-r--r--   0 user      (1000) vboxusers   (136)     2390 2024-04-09 23:37:27.000000 pytest_custom_outputs-0.1.2/src/pytest_custom_outputs/custom_outputs.py
-drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-30 00:57:34.619867 pytest_custom_outputs-0.1.2/src/pytest_custom_outputs.egg-info/
--rw-r--r--   0 user      (1000) vboxusers   (136)     9608 2024-05-30 00:57:34.000000 pytest_custom_outputs-0.1.2/src/pytest_custom_outputs.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) vboxusers   (136)      411 2024-05-30 00:57:34.000000 pytest_custom_outputs-0.1.2/src/pytest_custom_outputs.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) vboxusers   (136)        1 2024-05-30 00:57:34.000000 pytest_custom_outputs-0.1.2/src/pytest_custom_outputs.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) vboxusers   (136)       65 2024-05-30 00:57:34.000000 pytest_custom_outputs-0.1.2/src/pytest_custom_outputs.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) vboxusers   (136)       14 2024-05-30 00:57:34.000000 pytest_custom_outputs-0.1.2/src/pytest_custom_outputs.egg-info/requires.txt
--rw-r--r--   0 user      (1000) vboxusers   (136)       22 2024-05-30 00:57:34.000000 pytest_custom_outputs-0.1.2/src/pytest_custom_outputs.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-30 22:27:16.678738 pytest_custom_outputs-0.2.1/
+-rw-r--r--   0 user      (1000) vboxusers   (136)     1501 2024-04-09 20:33:50.000000 pytest_custom_outputs-0.2.1/LICENSE
+-rw-r--r--   0 user      (1000) vboxusers   (136)     7580 2024-05-30 22:27:16.678738 pytest_custom_outputs-0.2.1/PKG-INFO
+-rw-r--r--   0 user      (1000) vboxusers   (136)     4584 2024-05-30 22:26:44.000000 pytest_custom_outputs-0.2.1/README.rst
+-rw-r--r--   0 user      (1000) vboxusers   (136)     1490 2024-05-30 22:27:06.000000 pytest_custom_outputs-0.2.1/pyproject.toml
+-rw-r--r--   0 user      (1000) vboxusers   (136)       38 2024-05-30 22:27:16.678738 pytest_custom_outputs-0.2.1/setup.cfg
+drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-30 22:27:16.678738 pytest_custom_outputs-0.2.1/src/
+drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-30 22:27:16.678738 pytest_custom_outputs-0.2.1/src/pytest_custom_outputs/
+-rw-r--r--   0 user      (1000) vboxusers   (136)       58 2024-05-30 22:17:46.000000 pytest_custom_outputs-0.2.1/src/pytest_custom_outputs/__init__.py
+-rw-r--r--   0 user      (1000) vboxusers   (136)     2100 2024-05-30 22:17:51.000000 pytest_custom_outputs-0.2.1/src/pytest_custom_outputs/custom_outputs.py
+drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-30 22:27:16.678738 pytest_custom_outputs-0.2.1/src/pytest_custom_outputs.egg-info/
+-rw-r--r--   0 user      (1000) vboxusers   (136)     7580 2024-05-30 22:27:16.000000 pytest_custom_outputs-0.2.1/src/pytest_custom_outputs.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) vboxusers   (136)      411 2024-05-30 22:27:16.000000 pytest_custom_outputs-0.2.1/src/pytest_custom_outputs.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) vboxusers   (136)        1 2024-05-30 22:27:16.000000 pytest_custom_outputs-0.2.1/src/pytest_custom_outputs.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) vboxusers   (136)       65 2024-05-30 22:27:16.000000 pytest_custom_outputs-0.2.1/src/pytest_custom_outputs.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) vboxusers   (136)       14 2024-05-30 22:27:16.000000 pytest_custom_outputs-0.2.1/src/pytest_custom_outputs.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) vboxusers   (136)       22 2024-05-30 22:27:16.000000 pytest_custom_outputs-0.2.1/src/pytest_custom_outputs.egg-info/top_level.txt
```

### Comparing `pytest_custom_outputs-0.1.2/LICENSE` & `pytest_custom_outputs-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_custom_outputs-0.1.2/PKG-INFO` & `pytest_custom_outputs-0.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-custom_outputs
-Version: 0.1.2
+Version: 0.2.1
 Summary: A plugin that allows users to create and use custom outputs instead of the standard Pass and Fail
 Author-email: Babak Michael Engheta <michaelengheta55@gmail.com>
 Maintainer-email: Babak Michael Engheta <michaelengheta55@gmail.com>
 License: 
         Copyright (c) 2024, Babak Michael Engheta
         All rights reserved.
         
@@ -85,131 +85,86 @@
 In the directory where you will be running your pytest, create a file called "pytest_custom_outputs.json".
 You will use this file to create your own custom outputs.
 Feel free to copy and paste the below json file into yours and edit from there.
 
 EXAMPLE FILE:
 ```python
 {
-        "use_unknown_if_no_match": true,
         "unknown": {
-                "attribute":"_unknown",
-                "status": {
-                        "desc":"unknown",
-                        "code":"?",
-                        "output": {
-                                "tag":"UNKNOWN",
-                                "color":"purple"
-                        }
-                }
+                "desc":"unknown",
+                "code":"?",
+                "tag":"UNKNOWN",
+                "color":"purple"
         },
         "custom_outputs": {
                 "Pass_with_exception": {
-                        "attribute":"_expected_pass",
-                        "status": {
-                                "desc":"passed_with_exception",
-                                "code":"P",
-                                "output": {
-                                        "tag":"XPASSED",
-                                        "color":"green"
-                                }
-                        }
+                        "desc":"passed_with_exception",
+                        "code":"P",
+                        "tag":"XPASSED",
+                        "color":"green"
                 },
                 "Fatal_failed": {
-                        "attribute":"_fatal_fail",
-                        "status": {
-                                "desc":"fatal_failed",
-                                "code":"!",
-                                "output": {
-                                        "tag":"FAILED",
-                                        "color":"red"
-                                }
-                        }
+                        "desc":"fatal_failed",
+                        "code":"!",
+                        "tag":"FAILED",
+                        "color":"red"
                 },
                 "Not_available": {
-                        "attribute":"_not_available",
-                        "status": {
-                                "desc":"not_available",
-                                "code":"N",
-                                "output": {
-                                        "tag":"NOT_AVAILABLE",
-                                        "color":"blue"
-                                }
-                        }
+                        "desc":"not_available",
+                        "code":"N",
+                        "tag":"NOT_AVAILABLE",
+                        "color":"blue"
                 },
                 "Failed_but_proceed": {
-                        "attribute":"_fail_but_proceed",
-                        "status": {
-                                "desc":"failed_but_proceed",
-                                "code":"X",
-                                "output": {
-                                        "tag":"FAILED_BUT_PROCEED",
-                                        "color":"red"
-                                }
-                        }
+                        "desc":"failed_but_proceed",
+                        "code":"X",
+                        "tag":"FAILED_BUT_PROCEED",
+                        "color":"red"
                 },
                 "Unimplemented": {
-                        "attribute":"_unimplemented",
-                        "status": {
-                                "desc":"unimplemented",
-                                "code":"U",
-                                "output": {
-                                        "tag":"UNIMPLEMENTED",
-                                        "color":"yellow"
-                                }
-                        }
+                        "desc":"unimplemented",
+                        "code":"U",
+                        "tag":"UNIMPLEMENTED",
+                        "color":"yellow"
                 },
                 "Skipped": {
-                        "attribute":"_skipped",
-                        "status": {
-                                "desc":"skipped",
-                                "code":"S",
-                                "output": {
-                                        "tag":"SKIPPED",
-                                        "color":"yellow"
-                                }
-                        }
+                        "desc":"skipped",
+                        "code":"S",
+                        "tag":"SKIPPED",
+                        "color":"yellow"
                 }
         }
 }
-```
 
+```
 
-use_unknown_if_no_match
- - If True, use the unknown output below if there is no match. Otherwise, use standard skip
 
 unknown
- - The output to use if a test's result is not in default or custom outputs 
+ - The output to use if a test's result is not in custom outputs when calling c_assert
 
 custom_outputs
  - A dictionary with all the custom outputs you write inside of it. You can edit, delete, and add new outputs here.
 
-
 Each custom output is denoted by a name. The name is also the key for that output
 For example, in the above example file, "Pass_with_exception" and "Fatal_failed" are the names for their respective output.
 Names are also how we determine the result of a test case. 
-This is done by using skip followed by the name in the parameter.
+We use the c_assert function and enter the name as an argument to assert that specific output.
 
 For example:
 ```python
 import pytest
-from pytest import skip
+from pytest_custom_outputs import c_assert
 
 def test_1():
-    skip("Pass_with_exception")
+    c_assert("Pass_with_exception")
 ```
 
 In the example above, test_1 will result in "passed_with_exception".
-Because the name overrides the outcome, it will not result in a skip.
-We use the keyword skip as a means to obtaining our desired outcome.
-
-If we put a name that is not in our custom output in the skip parameter,
-then the following occurs:
- - if we set unknown to True in the json, we will use the unknown outcome
- - else we will use the default skip and pass the name as a message (Standard skip behavior)
 
+If we put a name that is not in our custom output in the c_assert parameter, then it will assert the unknown outcome
 
 The rest of the information in the json file can be edited and customized to your liking.
 
 
 Why pytest-custom_outputs?
 --------------------------
```

### Comparing `pytest_custom_outputs-0.1.2/pyproject.toml` & `pytest_custom_outputs-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=61.0.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytest-custom_outputs"
 description = "A plugin that allows users to create and use custom outputs instead of the standard Pass and Fail"
-version = "0.1.2"
+version = "0.2.1"
 readme = {file = "README.rst", content-type = "text/markdown"}
 requires-python = ">=3.8"
 authors = [
     { name = "Babak Michael Engheta", email = "michaelengheta55@gmail.com" },
 ]
 maintainers = [
     { name = "Babak Michael Engheta", email = "michaelengheta55@gmail.com" },
```

### Comparing `pytest_custom_outputs-0.1.2/src/pytest_custom_outputs.egg-info/PKG-INFO` & `pytest_custom_outputs-0.2.1/src/pytest_custom_outputs.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-custom_outputs
-Version: 0.1.2
+Version: 0.2.1
 Summary: A plugin that allows users to create and use custom outputs instead of the standard Pass and Fail
 Author-email: Babak Michael Engheta <michaelengheta55@gmail.com>
 Maintainer-email: Babak Michael Engheta <michaelengheta55@gmail.com>
 License: 
         Copyright (c) 2024, Babak Michael Engheta
         All rights reserved.
         
@@ -85,131 +85,86 @@
 In the directory where you will be running your pytest, create a file called "pytest_custom_outputs.json".
 You will use this file to create your own custom outputs.
 Feel free to copy and paste the below json file into yours and edit from there.
 
 EXAMPLE FILE:
 ```python
 {
-        "use_unknown_if_no_match": true,
         "unknown": {
-                "attribute":"_unknown",
-                "status": {
-                        "desc":"unknown",
-                        "code":"?",
-                        "output": {
-                                "tag":"UNKNOWN",
-                                "color":"purple"
-                        }
-                }
+                "desc":"unknown",
+                "code":"?",
+                "tag":"UNKNOWN",
+                "color":"purple"
         },
         "custom_outputs": {
                 "Pass_with_exception": {
-                        "attribute":"_expected_pass",
-                        "status": {
-                                "desc":"passed_with_exception",
-                                "code":"P",
-                                "output": {
-                                        "tag":"XPASSED",
-                                        "color":"green"
-                                }
-                        }
+                        "desc":"passed_with_exception",
+                        "code":"P",
+                        "tag":"XPASSED",
+                        "color":"green"
                 },
                 "Fatal_failed": {
-                        "attribute":"_fatal_fail",
-                        "status": {
-                                "desc":"fatal_failed",
-                                "code":"!",
-                                "output": {
-                                        "tag":"FAILED",
-                                        "color":"red"
-                                }
-                        }
+                        "desc":"fatal_failed",
+                        "code":"!",
+                        "tag":"FAILED",
+                        "color":"red"
                 },
                 "Not_available": {
-                        "attribute":"_not_available",
-                        "status": {
-                                "desc":"not_available",
-                                "code":"N",
-                                "output": {
-                                        "tag":"NOT_AVAILABLE",
-                                        "color":"blue"
-                                }
-                        }
+                        "desc":"not_available",
+                        "code":"N",
+                        "tag":"NOT_AVAILABLE",
+                        "color":"blue"
                 },
                 "Failed_but_proceed": {
-                        "attribute":"_fail_but_proceed",
-                        "status": {
-                                "desc":"failed_but_proceed",
-                                "code":"X",
-                                "output": {
-                                        "tag":"FAILED_BUT_PROCEED",
-                                        "color":"red"
-                                }
-                        }
+                        "desc":"failed_but_proceed",
+                        "code":"X",
+                        "tag":"FAILED_BUT_PROCEED",
+                        "color":"red"
                 },
                 "Unimplemented": {
-                        "attribute":"_unimplemented",
-                        "status": {
-                                "desc":"unimplemented",
-                                "code":"U",
-                                "output": {
-                                        "tag":"UNIMPLEMENTED",
-                                        "color":"yellow"
-                                }
-                        }
+                        "desc":"unimplemented",
+                        "code":"U",
+                        "tag":"UNIMPLEMENTED",
+                        "color":"yellow"
                 },
                 "Skipped": {
-                        "attribute":"_skipped",
-                        "status": {
-                                "desc":"skipped",
-                                "code":"S",
-                                "output": {
-                                        "tag":"SKIPPED",
-                                        "color":"yellow"
-                                }
-                        }
+                        "desc":"skipped",
+                        "code":"S",
+                        "tag":"SKIPPED",
+                        "color":"yellow"
                 }
         }
 }
-```
 
+```
 
-use_unknown_if_no_match
- - If True, use the unknown output below if there is no match. Otherwise, use standard skip
 
 unknown
- - The output to use if a test's result is not in default or custom outputs 
+ - The output to use if a test's result is not in custom outputs when calling c_assert
 
 custom_outputs
  - A dictionary with all the custom outputs you write inside of it. You can edit, delete, and add new outputs here.
 
-
 Each custom output is denoted by a name. The name is also the key for that output
 For example, in the above example file, "Pass_with_exception" and "Fatal_failed" are the names for their respective output.
 Names are also how we determine the result of a test case. 
-This is done by using skip followed by the name in the parameter.
+We use the c_assert function and enter the name as an argument to assert that specific output.
 
 For example:
 ```python
 import pytest
-from pytest import skip
+from pytest_custom_outputs import c_assert
 
 def test_1():
-    skip("Pass_with_exception")
+    c_assert("Pass_with_exception")
 ```
 
 In the example above, test_1 will result in "passed_with_exception".
-Because the name overrides the outcome, it will not result in a skip.
-We use the keyword skip as a means to obtaining our desired outcome.
-
-If we put a name that is not in our custom output in the skip parameter,
-then the following occurs:
- - if we set unknown to True in the json, we will use the unknown outcome
- - else we will use the default skip and pass the name as a message (Standard skip behavior)
 
+If we put a name that is not in our custom output in the c_assert parameter, then it will assert the unknown outcome
 
 The rest of the information in the json file can be edited and customized to your liking.
 
 
 Why pytest-custom_outputs?
 --------------------------
```

