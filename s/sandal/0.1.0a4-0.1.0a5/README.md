# Comparing `tmp/sandal-0.1.0a4.tar.gz` & `tmp/sandal-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sandal-0.1.0a4.tar", last modified: Fri Apr 26 20:58:53 2024, max compression
+gzip compressed data, was "sandal-0.1.0a5.tar", last modified: Fri May 31 21:27:22 2024, max compression
```

## Comparing `sandal-0.1.0a4.tar` & `sandal-0.1.0a5.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:58:53.209049 sandal-0.1.0a4/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-26 20:58:42.000000 sandal-0.1.0a4/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-26 20:58:42.000000 sandal-0.1.0a4/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-26 20:58:42.000000 sandal-0.1.0a4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-26 20:58:42.000000 sandal-0.1.0a4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-26 20:58:42.000000 sandal-0.1.0a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-26 20:58:53.209049 sandal-0.1.0a4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:58:53.205049 sandal-0.1.0a4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-26 20:58:42.000000 sandal-0.1.0a4/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-26 20:58:42.000000 sandal-0.1.0a4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-26 20:58:42.000000 sandal-0.1.0a4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-26 20:58:42.000000 sandal-0.1.0a4/docs/notebook.rst
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-26 20:58:42.000000 sandal-0.1.0a4/justfile
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-26 20:58:42.000000 sandal-0.1.0a4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:58:53.209049 sandal-0.1.0a4/sandal/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-26 20:58:42.000000 sandal-0.1.0a4/sandal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-26 20:58:42.000000 sandal-0.1.0a4/sandal/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-26 20:58:42.000000 sandal-0.1.0a4/sandal/loghelper.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-26 20:58:42.000000 sandal-0.1.0a4/sandal/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-26 20:58:42.000000 sandal-0.1.0a4/sandal/root.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:58:53.209049 sandal-0.1.0a4/sandal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-26 20:58:53.000000 sandal-0.1.0a4/sandal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-26 20:58:53.000000 sandal-0.1.0a4/sandal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:58:53.000000 sandal-0.1.0a4/sandal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-26 20:58:53.000000 sandal-0.1.0a4/sandal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-26 20:58:53.000000 sandal-0.1.0a4/sandal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 20:58:53.209049 sandal-0.1.0a4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:27:22.785819 sandal-0.1.0a5/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-31 21:27:18.000000 sandal-0.1.0a5/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-31 21:27:18.000000 sandal-0.1.0a5/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-31 21:27:18.000000 sandal-0.1.0a5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-31 21:27:18.000000 sandal-0.1.0a5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-31 21:27:18.000000 sandal-0.1.0a5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-31 21:27:22.785819 sandal-0.1.0a5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:27:22.777819 sandal-0.1.0a5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-31 21:27:18.000000 sandal-0.1.0a5/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-31 21:27:18.000000 sandal-0.1.0a5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-31 21:27:18.000000 sandal-0.1.0a5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-31 21:27:18.000000 sandal-0.1.0a5/docs/notebook.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-31 21:27:18.000000 sandal-0.1.0a5/justfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-31 21:27:18.000000 sandal-0.1.0a5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:27:22.781819 sandal-0.1.0a5/sandal/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-31 21:27:18.000000 sandal-0.1.0a5/sandal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-31 21:27:18.000000 sandal-0.1.0a5/sandal/autoroot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-31 21:27:18.000000 sandal-0.1.0a5/sandal/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-31 21:27:18.000000 sandal-0.1.0a5/sandal/loghelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-31 21:27:18.000000 sandal-0.1.0a5/sandal/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-31 21:27:18.000000 sandal-0.1.0a5/sandal/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-31 21:27:18.000000 sandal-0.1.0a5/sandal/root.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:27:22.781819 sandal-0.1.0a5/sandal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-31 21:27:22.000000 sandal-0.1.0a5/sandal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-31 21:27:22.000000 sandal-0.1.0a5/sandal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 21:27:22.000000 sandal-0.1.0a5/sandal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-31 21:27:22.000000 sandal-0.1.0a5/sandal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-31 21:27:22.000000 sandal-0.1.0a5/sandal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 21:27:22.785819 sandal-0.1.0a5/setup.cfg
```

### Comparing `sandal-0.1.0a4/.gitignore` & `sandal-0.1.0a5/.gitignore`

 * *Files identical despite different names*

### Comparing `sandal-0.1.0a4/LICENSE.md` & `sandal-0.1.0a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sandal-0.1.0a4/PKG-INFO` & `sandal-0.1.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sandal
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: Lightweight bootstrapping for project scripts
 Author-email: Michael Ekstrand <mdekstrand@drexel.edu>
 License: Copyright (c) 2023 Michael D. Ekstrand
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -33,15 +33,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: tomli~=2.0; python_version < "3.12"
 Requires-Dist: enlighten~=1.12
 Requires-Dist: colorlog==6.*
-Requires-Dist: progress-api>=0.1.0a6
+Requires-Dist: progress-api>=0.1.0a9
 Provides-Extra: dev
 Requires-Dist: setuptools>=64; extra == "dev"
 Requires-Dist: setuptools_scm>=8; extra == "dev"
 Requires-Dist: build==1.*; extra == "dev"
 Requires-Dist: ruff>=0.2; extra == "dev"
 Requires-Dist: pyright; extra == "dev"
 Requires-Dist: copier==9.*; extra == "dev"
```

### Comparing `sandal-0.1.0a4/docs/conf.py` & `sandal-0.1.0a5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sandal-0.1.0a4/justfile` & `sandal-0.1.0a5/justfile`

 * *Files identical despite different names*

### Comparing `sandal-0.1.0a4/pyproject.toml` & `sandal-0.1.0a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 readme = "README.md"
 license = { file = "LICENSE.md" }
 dynamic = ["version"]
 dependencies = [
   "tomli~=2.0;python_version<'3.12'",
   "enlighten~=1.12",
   "colorlog==6.*",
-  "progress-api>=0.1.0a6",
+  "progress-api>=0.1.0a9",
 ]
 
 [project.optional-dependencies]
 dev = [
   "setuptools>=64",
   "setuptools_scm>=8",
   "build ==1.*",       # p2c: -s python-build==1
```

### Comparing `sandal-0.1.0a4/sandal/cli.py` & `sandal-0.1.0a5/sandal/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from colorlog import ColoredFormatter
 from enlighten import Manager
 from progress_api.backends.enlighten import EnlightenProgressBackend
 
 from .loghelper import BunyanFormatter, Verbosity, vrb_to_level
 
 term_fmt = ColoredFormatter(
-    "[%(blue)s%(asctime)s%(reset)s] %(log_color)s%(levelname)-8s%(reset)s %(cyan)s%(name)s %(reset)s%(message)s",  # noqa: E501
+    "[%(blue)s%(asctime)s%(reset)s] %(log_color)s%(levelname)8s%(reset)s %(cyan)s%(name)s %(reset)s%(message)s",  # noqa: E501
     datefmt="%H:%M:%S",
     reset=True,
     log_colors={
         "DEBUG": "cyan",
         "INFO": "green",
         "WARNING": "yellow",
         "ERROR": "red",
@@ -61,8 +61,17 @@
         fh.setLevel(file_level)
         fh.setFormatter(BunyanFormatter())
         root.addHandler(fh)
     else:
         root.setLevel(term_level)
 
     emgr = Manager(stream=sys.stderr)
-    progress_api.set_backend(EnlightenProgressBackend, emgr)
+    progress_api.set_backend(
+        EnlightenProgressBackend,
+        emgr,
+        state_colors={
+            "finished": "green",
+            "failed": "red",
+            "in-progress": "yellow",
+            "dispatched": "grey",
+        },
+    )
```

### Comparing `sandal-0.1.0a4/sandal/loghelper.py` & `sandal-0.1.0a5/sandal/loghelper.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,17 @@
     elif verbose > 0:
         level = logging.DEBUG
     return level
 
 
 class BunyanFormatter(Formatter):
     def format(self, record: LogRecord) -> str:
+        if not hasattr(record, "message"):
+            record.message = record.getMessage()
+
         obj = {
             "v": 0,
             "time": self.formatTime(record),
             "level": record.levelno + 10,
             "name": record.name,
             "pid": record.process,
             "msg": record.message,
```

### Comparing `sandal-0.1.0a4/sandal/notebook.py` & `sandal-0.1.0a5/sandal/notebook.py`

 * *Files identical despite different names*

### Comparing `sandal-0.1.0a4/sandal.egg-info/PKG-INFO` & `sandal-0.1.0a5/sandal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sandal
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: Lightweight bootstrapping for project scripts
 Author-email: Michael Ekstrand <mdekstrand@drexel.edu>
 License: Copyright (c) 2023 Michael D. Ekstrand
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -33,15 +33,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: tomli~=2.0; python_version < "3.12"
 Requires-Dist: enlighten~=1.12
 Requires-Dist: colorlog==6.*
-Requires-Dist: progress-api>=0.1.0a6
+Requires-Dist: progress-api>=0.1.0a9
 Provides-Extra: dev
 Requires-Dist: setuptools>=64; extra == "dev"
 Requires-Dist: setuptools_scm>=8; extra == "dev"
 Requires-Dist: build==1.*; extra == "dev"
 Requires-Dist: ruff>=0.2; extra == "dev"
 Requires-Dist: pyright; extra == "dev"
 Requires-Dist: copier==9.*; extra == "dev"
```

