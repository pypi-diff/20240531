# Comparing `tmp/brianmechanisms-0.1.6.tar.gz` & `tmp/brianmechanisms-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brianmechanisms-0.1.6.tar", last modified: Sun May 26 19:24:27 2024, max compression
+gzip compressed data, was "brianmechanisms-0.1.7.tar", last modified: Fri May 31 10:21:03 2024, max compression
```

## Comparing `brianmechanisms-0.1.6.tar` & `brianmechanisms-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:24:27.419389 brianmechanisms-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-05-26 19:24:12.000000 brianmechanisms-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-05-26 19:24:27.419389 brianmechanisms-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-05-26 19:24:12.000000 brianmechanisms-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-26 19:24:12.000000 brianmechanisms-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 19:24:27.419389 brianmechanisms-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:24:27.415389 brianmechanisms-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:24:27.419389 brianmechanisms-0.1.6/src/brianmechanisms/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-26 19:24:12.000000 brianmechanisms-0.1.6/src/brianmechanisms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23980 2024-05-26 19:24:12.000000 brianmechanisms-0.1.6/src/brianmechanisms/appproximateStraightLineMechanisms.py
--rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-05-26 19:24:12.000000 brianmechanisms-0.1.6/src/brianmechanisms/locii.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-26 19:24:12.000000 brianmechanisms-0.1.6/src/brianmechanisms/mirror.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-26 19:24:12.000000 brianmechanisms-0.1.6/src/brianmechanisms/straightLineMechanisms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:24:27.419389 brianmechanisms-0.1.6/src/brianmechanisms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-05-26 19:24:27.000000 brianmechanisms-0.1.6/src/brianmechanisms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-26 19:24:27.000000 brianmechanisms-0.1.6/src/brianmechanisms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 19:24:27.000000 brianmechanisms-0.1.6/src/brianmechanisms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-26 19:24:27.000000 brianmechanisms-0.1.6/src/brianmechanisms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-26 19:24:27.000000 brianmechanisms-0.1.6/src/brianmechanisms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:21:03.759320 brianmechanisms-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-05-31 10:20:53.000000 brianmechanisms-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-05-31 10:21:03.759320 brianmechanisms-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-05-31 10:20:53.000000 brianmechanisms-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-31 10:20:53.000000 brianmechanisms-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 10:21:03.759320 brianmechanisms-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:21:03.755320 brianmechanisms-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:21:03.755320 brianmechanisms-0.1.7/src/brianmechanisms/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-31 10:20:53.000000 brianmechanisms-0.1.7/src/brianmechanisms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23980 2024-05-31 10:20:53.000000 brianmechanisms-0.1.7/src/brianmechanisms/appproximateStraightLineMechanisms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14454 2024-05-31 10:20:53.000000 brianmechanisms-0.1.7/src/brianmechanisms/locii.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-31 10:20:53.000000 brianmechanisms-0.1.7/src/brianmechanisms/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-31 10:20:53.000000 brianmechanisms-0.1.7/src/brianmechanisms/straightLineMechanisms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:21:03.759320 brianmechanisms-0.1.7/src/brianmechanisms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-05-31 10:21:03.000000 brianmechanisms-0.1.7/src/brianmechanisms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-31 10:21:03.000000 brianmechanisms-0.1.7/src/brianmechanisms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 10:21:03.000000 brianmechanisms-0.1.7/src/brianmechanisms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-31 10:21:03.000000 brianmechanisms-0.1.7/src/brianmechanisms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 10:21:03.000000 brianmechanisms-0.1.7/src/brianmechanisms.egg-info/top_level.txt
```

### Comparing `brianmechanisms-0.1.6/LICENSE` & `brianmechanisms-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `brianmechanisms-0.1.6/PKG-INFO` & `brianmechanisms-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brianmechanisms
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python module for designing mechanisms and robots
 Home-page: https://brianmechanisms.github.io
 Author: Brian Onang'o
 Author-email: surgbc@gmail.com
 Project-URL: Homepage, https://github.com/brianmechanisms/brianmechanisms-designer
 Project-URL: Issues, https://github.com/brianmechanisms/brianmechanisms-designer/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `brianmechanisms-0.1.6/README.md` & `brianmechanisms-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `brianmechanisms-0.1.6/src/brianmechanisms/appproximateStraightLineMechanisms.py` & `brianmechanisms-0.1.7/src/brianmechanisms/appproximateStraightLineMechanisms.py`

 * *Files identical despite different names*

### Comparing `brianmechanisms-0.1.6/src/brianmechanisms.egg-info/PKG-INFO` & `brianmechanisms-0.1.7/src/brianmechanisms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brianmechanisms
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python module for designing mechanisms and robots
 Home-page: https://brianmechanisms.github.io
 Author: Brian Onang'o
 Author-email: surgbc@gmail.com
 Project-URL: Homepage, https://github.com/brianmechanisms/brianmechanisms-designer
 Project-URL: Issues, https://github.com/brianmechanisms/brianmechanisms-designer/issues
 Classifier: Programming Language :: Python :: 3
```

