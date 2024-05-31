# Comparing `tmp/rpmlint_codeclimate-0.1.0.tar.gz` & `tmp/rpmlint_codeclimate-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpmlint_codeclimate-0.1.0.tar", last modified: Wed May 29 16:25:03 2024, max compression
+gzip compressed data, was "rpmlint_codeclimate-0.1.1.tar", last modified: Fri May 31 16:35:54 2024, max compression
```

## Comparing `rpmlint_codeclimate-0.1.0.tar` & `rpmlint_codeclimate-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 16:25:03.339887 rpmlint_codeclimate-0.1.0/
--rw-rw-rw-   0 root         (0) root         (0)      551 2024-05-29 16:24:57.000000 rpmlint_codeclimate-0.1.0/.flake8
--rw-rw-rw-   0 root         (0) root         (0)      236 2024-05-29 16:24:57.000000 rpmlint_codeclimate-0.1.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     2786 2024-05-29 16:24:57.000000 rpmlint_codeclimate-0.1.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1083 2024-05-29 16:24:57.000000 rpmlint_codeclimate-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1470 2024-05-29 16:25:03.339887 rpmlint_codeclimate-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      398 2024-05-29 16:24:57.000000 rpmlint_codeclimate-0.1.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1483 2024-05-29 16:24:57.000000 rpmlint_codeclimate-0.1.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 16:25:03.336887 rpmlint_codeclimate-0.1.0/rpmlint_codeclimate/
--rw-rw-rw-   0 root         (0) root         (0)      337 2024-05-29 16:24:57.000000 rpmlint_codeclimate-0.1.0/rpmlint_codeclimate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      273 2024-05-29 16:24:57.000000 rpmlint_codeclimate-0.1.0/rpmlint_codeclimate/__main__.py
--rw-r--r--   0 root         (0) root         (0)      411 2024-05-29 16:25:03.000000 rpmlint_codeclimate-0.1.0/rpmlint_codeclimate/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     4729 2024-05-29 16:24:57.000000 rpmlint_codeclimate-0.1.0/rpmlint_codeclimate/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 16:25:03.338887 rpmlint_codeclimate-0.1.0/rpmlint_codeclimate/tests/
--rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-29 16:24:57.000000 rpmlint_codeclimate-0.1.0/rpmlint_codeclimate/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1751 2024-05-29 16:24:57.000000 rpmlint_codeclimate-0.1.0/rpmlint_codeclimate/tests/example.spec
--rw-rw-rw-   0 root         (0) root         (0)     4002 2024-05-29 16:24:57.000000 rpmlint_codeclimate-0.1.0/rpmlint_codeclimate/tests/test_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 16:25:03.338887 rpmlint_codeclimate-0.1.0/rpmlint_codeclimate.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1470 2024-05-29 16:25:03.000000 rpmlint_codeclimate-0.1.0/rpmlint_codeclimate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      524 2024-05-29 16:25:03.000000 rpmlint_codeclimate-0.1.0/rpmlint_codeclimate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 16:25:03.000000 rpmlint_codeclimate-0.1.0/rpmlint_codeclimate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      126 2024-05-29 16:25:03.000000 rpmlint_codeclimate-0.1.0/rpmlint_codeclimate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-29 16:25:03.000000 rpmlint_codeclimate-0.1.0/rpmlint_codeclimate.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 16:25:03.339887 rpmlint_codeclimate-0.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 16:35:54.969138 rpmlint_codeclimate-0.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)      551 2024-05-31 16:35:49.000000 rpmlint_codeclimate-0.1.1/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)      236 2024-05-31 16:35:49.000000 rpmlint_codeclimate-0.1.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     2786 2024-05-31 16:35:49.000000 rpmlint_codeclimate-0.1.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2024-05-31 16:35:49.000000 rpmlint_codeclimate-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1470 2024-05-31 16:35:54.969138 rpmlint_codeclimate-0.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      398 2024-05-31 16:35:49.000000 rpmlint_codeclimate-0.1.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1483 2024-05-31 16:35:49.000000 rpmlint_codeclimate-0.1.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 16:35:54.966138 rpmlint_codeclimate-0.1.1/rpmlint_codeclimate/
+-rw-rw-rw-   0 root         (0) root         (0)      337 2024-05-31 16:35:49.000000 rpmlint_codeclimate-0.1.1/rpmlint_codeclimate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      273 2024-05-31 16:35:49.000000 rpmlint_codeclimate-0.1.1/rpmlint_codeclimate/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2024-05-31 16:35:54.000000 rpmlint_codeclimate-0.1.1/rpmlint_codeclimate/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     4739 2024-05-31 16:35:49.000000 rpmlint_codeclimate-0.1.1/rpmlint_codeclimate/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 16:35:54.968138 rpmlint_codeclimate-0.1.1/rpmlint_codeclimate/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-31 16:35:49.000000 rpmlint_codeclimate-0.1.1/rpmlint_codeclimate/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1751 2024-05-31 16:35:49.000000 rpmlint_codeclimate-0.1.1/rpmlint_codeclimate/tests/example.spec
+-rw-rw-rw-   0 root         (0) root         (0)     3994 2024-05-31 16:35:49.000000 rpmlint_codeclimate-0.1.1/rpmlint_codeclimate/tests/test_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 16:35:54.968138 rpmlint_codeclimate-0.1.1/rpmlint_codeclimate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1470 2024-05-31 16:35:54.000000 rpmlint_codeclimate-0.1.1/rpmlint_codeclimate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      524 2024-05-31 16:35:54.000000 rpmlint_codeclimate-0.1.1/rpmlint_codeclimate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 16:35:54.000000 rpmlint_codeclimate-0.1.1/rpmlint_codeclimate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      126 2024-05-31 16:35:54.000000 rpmlint_codeclimate-0.1.1/rpmlint_codeclimate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-31 16:35:54.000000 rpmlint_codeclimate-0.1.1/rpmlint_codeclimate.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 16:35:54.970138 rpmlint_codeclimate-0.1.1/setup.cfg
```

### Comparing `rpmlint_codeclimate-0.1.0/.flake8` & `rpmlint_codeclimate-0.1.1/.flake8`

 * *Files identical despite different names*

### Comparing `rpmlint_codeclimate-0.1.0/.gitlab-ci.yml` & `rpmlint_codeclimate-0.1.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `rpmlint_codeclimate-0.1.0/LICENSE` & `rpmlint_codeclimate-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rpmlint_codeclimate-0.1.0/PKG-INFO` & `rpmlint_codeclimate-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpmlint-codeclimate
-Version: 0.1.0
+Version: 0.1.1
 Summary: Codeclimate parser for rpmlint
 Author-email: Duncan Macleod <macleoddm@cardiff.ac.uk>
 License: MIT
 Project-URL: Homepage, https://gitlab.com/duncanmmacleod/rpmlint-codeclimate/
 Project-URL: Bug Tracker, https://gitlab.com/duncanmmacleod/rpmlint-codeclimate/-/issues/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rpmlint_codeclimate-0.1.0/pyproject.toml` & `rpmlint_codeclimate-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rpmlint_codeclimate-0.1.0/rpmlint_codeclimate/parser.py` & `rpmlint_codeclimate-0.1.1/rpmlint_codeclimate/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,16 +56,16 @@
 def get_location(path, lineno=None, tag=None, **kwargs):
     """Attempt to identify a codeclimate 'location' for a lint entry.
     """
     def _loc(begin, end):
         return {
             "path": str(path),
             "lines": {
-                "begin": begin,
-                "end": end,
+                "begin": int(begin),
+                "end": int(end),
             }
         }
 
     if lineno:
         return _loc(lineno, lineno)
 
     pattern = Template(LOCATION_PATTERN.get(tag, "")).safe_substitute(
```

### Comparing `rpmlint_codeclimate-0.1.0/rpmlint_codeclimate/tests/example.spec` & `rpmlint_codeclimate-0.1.1/rpmlint_codeclimate/tests/example.spec`

 * *Files identical despite different names*

### Comparing `rpmlint_codeclimate-0.1.0/rpmlint_codeclimate/tests/test_parser.py` & `rpmlint_codeclimate-0.1.1/rpmlint_codeclimate/tests/test_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,16 @@
         'content': {
             'body': 'The specfile contains an unversioned Obsoletes: token, which will match all\nolder, equal and newer versions of the obsoleted thing.  This may cause update\nproblems, restrict future package/provides naming, and may match something it\nwas originally not inteded to match -- make the Obsoletes versioned if\npossible.'
         },
         'description': 'Unversioned explicit obsoletes other-example-package',
         'fingerprint': 'f20db46605ba2cc06c7bffd5f91d7a09f49c0c59',
         'location': {
             'lines': {
-                'begin': '36',
-                'end': '36',
+                'begin': 36,
+                'end': 36,
             },
             'path': str(EXAMPLE_SPEC),
         },
         'severity': 'minor',
         'type': 'issue',
     },
     {
@@ -86,16 +86,16 @@
         'content': {
             'body': "The Packager tag is hardcoded in your spec file. It should be removed, so as\nto use rebuilder's own defaults."
         },
         'description': 'Hardcoded packager tag Duncan Macleod <macleoddm@cardiff.ac.uk>',
         'fingerprint': '9bf0a84c9f1e0f84adad31639dd36de4048564f2',
         'location': {
             'lines': {
-                'begin': '15',
-                'end': '15',
+                'begin': 15,
+                'end': 15,
             },
             'path': str(EXAMPLE_SPEC),
         },
         'severity': 'minor',
         'type': 'issue',
     },
 ]
```

### Comparing `rpmlint_codeclimate-0.1.0/rpmlint_codeclimate.egg-info/PKG-INFO` & `rpmlint_codeclimate-0.1.1/rpmlint_codeclimate.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpmlint-codeclimate
-Version: 0.1.0
+Version: 0.1.1
 Summary: Codeclimate parser for rpmlint
 Author-email: Duncan Macleod <macleoddm@cardiff.ac.uk>
 License: MIT
 Project-URL: Homepage, https://gitlab.com/duncanmmacleod/rpmlint-codeclimate/
 Project-URL: Bug Tracker, https://gitlab.com/duncanmmacleod/rpmlint-codeclimate/-/issues/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rpmlint_codeclimate-0.1.0/rpmlint_codeclimate.egg-info/SOURCES.txt` & `rpmlint_codeclimate-0.1.1/rpmlint_codeclimate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

