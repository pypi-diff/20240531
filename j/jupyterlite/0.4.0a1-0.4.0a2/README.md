# Comparing `tmp/jupyterlite-0.4.0a1.tar.gz` & `tmp/jupyterlite-0.4.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue May 28 19:52:14 2024, max compression
+gzip compressed data, last modified: Fri May 31 13:26:32 2024, max compression
```

## Comparing `jupyterlite-0.4.0a1.tar` & `jupyterlite-0.4.0a2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       56 2024-05-28 19:52:14.000000 jupyterlite-0.4.0a1/jupyterlite/__init__.py
--rw-r--r--   0        0        0       81 2024-05-28 19:52:14.000000 jupyterlite-0.4.0a1/jupyterlite/__main__.py
--rw-r--r--   0        0        0      354 2024-05-28 19:52:14.000000 jupyterlite-0.4.0a1/jupyterlite/constants.py
--rw-r--r--   0        0        0      331 2024-05-28 19:52:14.000000 jupyterlite-0.4.0a1/jupyterlite/addons/base.py
--rw-r--r--   0        0        0     2189 2024-05-28 19:52:14.000000 jupyterlite-0.4.0a1/.gitignore
--rw-r--r--   0        0        0     1524 2024-05-28 19:52:14.000000 jupyterlite-0.4.0a1/LICENSE
--rw-r--r--   0        0        0     5688 2024-05-28 19:52:14.000000 jupyterlite-0.4.0a1/README.md
--rw-r--r--   0        0        0     1995 2024-05-28 19:52:14.000000 jupyterlite-0.4.0a1/pyproject.toml
--rw-r--r--   0        0        0     9542 2024-05-28 19:52:14.000000 jupyterlite-0.4.0a1/PKG-INFO
+-rw-r--r--   0        0        0       56 2024-05-31 13:26:32.000000 jupyterlite-0.4.0a2/jupyterlite/__init__.py
+-rw-r--r--   0        0        0       81 2024-05-31 13:26:32.000000 jupyterlite-0.4.0a2/jupyterlite/__main__.py
+-rw-r--r--   0        0        0      354 2024-05-31 13:26:32.000000 jupyterlite-0.4.0a2/jupyterlite/constants.py
+-rw-r--r--   0        0        0      331 2024-05-31 13:26:32.000000 jupyterlite-0.4.0a2/jupyterlite/addons/base.py
+-rw-r--r--   0        0        0     2189 2024-05-31 13:26:32.000000 jupyterlite-0.4.0a2/.gitignore
+-rw-r--r--   0        0        0     1524 2024-05-31 13:26:32.000000 jupyterlite-0.4.0a2/LICENSE
+-rw-r--r--   0        0        0     5688 2024-05-31 13:26:32.000000 jupyterlite-0.4.0a2/README.md
+-rw-r--r--   0        0        0     1995 2024-05-31 13:26:32.000000 jupyterlite-0.4.0a2/pyproject.toml
+-rw-r--r--   0        0        0     9542 2024-05-31 13:26:32.000000 jupyterlite-0.4.0a2/PKG-INFO
```

### Comparing `jupyterlite-0.4.0a1/.gitignore` & `jupyterlite-0.4.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlite-0.4.0a1/LICENSE` & `jupyterlite-0.4.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlite-0.4.0a1/README.md` & `jupyterlite-0.4.0a2/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlite-0.4.0a1/pyproject.toml` & `jupyterlite-0.4.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "jupyterlite"
 authors = [
     {name = "JupyterLite Contributors"},
 ]
 dependencies = [
-    "jupyterlite-core >=0.4.0a1",
+    "jupyterlite-core >=0.4.0a2",
 ]
 keywords = [
     "browser",
     "js",
     "jupyter",
     "jupyterlab",
     "notebook",
@@ -64,15 +64,15 @@
 ]
 check = [
     "jsonschema[format_nongpl] >=3",
 ]
 all = [
     "jsonschema >=3",
     "jupyter_server",
-    "jupyterlab >=4.2.0,<4.3",
+    "jupyterlab >=4.2.1,<4.3",
     "jupyterlab_server >=2.8.1,<3",
     "libarchive-c >=4.0",
     "notebook >=7.2.0,<7.3",
     "pkginfo",
     "tornado >=6.1",
 ]
```

### Comparing `jupyterlite-0.4.0a1/PKG-INFO` & `jupyterlite-0.4.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlite
-Version: 0.4.0a1
+Version: 0.4.0a2
 Dynamic: Summary
 Project-URL: Source, https://github.com/jupyterlite/jupyterlite
 Author: JupyterLite Contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2022, JupyterLite Contributors
         All rights reserved.
@@ -48,20 +48,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Pre-processors
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Requires-Python: >=3.8
-Requires-Dist: jupyterlite-core>=0.4.0a1
+Requires-Dist: jupyterlite-core>=0.4.0a2
 Provides-Extra: all
 Requires-Dist: jsonschema>=3; extra == 'all'
 Requires-Dist: jupyter-server; extra == 'all'
 Requires-Dist: jupyterlab-server<3,>=2.8.1; extra == 'all'
-Requires-Dist: jupyterlab<4.3,>=4.2.0; extra == 'all'
+Requires-Dist: jupyterlab<4.3,>=4.2.1; extra == 'all'
 Requires-Dist: libarchive-c>=4.0; extra == 'all'
 Requires-Dist: notebook<7.3,>=7.2.0; extra == 'all'
 Requires-Dist: pkginfo; extra == 'all'
 Requires-Dist: tornado>=6.1; extra == 'all'
 Provides-Extra: check
 Requires-Dist: jsonschema[format-nongpl]>=3; extra == 'check'
 Provides-Extra: contents
```

