# Comparing `tmp/changy-0.1.1.tar.gz` & `tmp/changy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "changy-0.1.1.tar", max compression
+gzip compressed data, was "changy-0.1.2.tar", max compression
```

## Comparing `changy-0.1.1.tar` & `changy-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1504 2024-05-31 10:46:04.512312 changy-0.1.1/LICENSE
--rw-r--r--   0        0        0      302 2024-05-31 10:46:04.512312 changy-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-31 10:46:04.512312 changy-0.1.1/changy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-31 10:46:04.512312 changy-0.1.1/changy/cli/__init__.py
--rw-r--r--   0        0        0      334 2024-05-31 10:46:04.512312 changy-0.1.1/changy/cli/__main__.py
--rw-r--r--   0        0        0       34 2024-05-31 10:46:04.512312 changy-0.1.1/changy/cli/application.py
--rw-r--r--   0        0        0      128 2024-05-31 10:46:04.512312 changy-0.1.1/changy/cli/changelog.py
--rw-r--r--   0        0        0      200 2024-05-31 10:46:04.512312 changy-0.1.1/changy/cli/unreleased.py
--rw-r--r--   0        0        0      145 2024-05-31 10:46:04.512312 changy-0.1.1/changy/cli/version.py
--rw-r--r--   0        0        0      477 2024-05-31 10:46:04.512312 changy-0.1.1/changy/constants.py
--rw-r--r--   0        0        0     2942 2024-05-31 10:46:04.512312 changy-0.1.1/changy/logic.py
--rw-r--r--   0        0        0      768 2024-05-31 10:46:04.512312 changy-0.1.1/changy/settings.py
--rw-r--r--   0        0        0        0 2024-05-31 10:46:04.512312 changy-0.1.1/changy/tests/__init__.py
--rw-r--r--   0        0        0       29 2024-05-31 10:46:04.516312 changy-0.1.1/changy/tests/test_logic.py
--rw-r--r--   0        0        0     1953 2024-05-31 10:46:12.072193 changy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1400 1970-01-01 00:00:00.000000 changy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-05-31 11:17:29.563136 changy-0.1.2/LICENSE
+-rw-r--r--   0        0        0      358 2024-05-31 11:17:29.563136 changy-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-31 11:17:29.567136 changy-0.1.2/changy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 11:17:29.567136 changy-0.1.2/changy/cli/__init__.py
+-rw-r--r--   0        0        0      334 2024-05-31 11:17:29.567136 changy-0.1.2/changy/cli/__main__.py
+-rw-r--r--   0        0        0       34 2024-05-31 11:17:29.567136 changy-0.1.2/changy/cli/application.py
+-rw-r--r--   0        0        0      128 2024-05-31 11:17:29.567136 changy-0.1.2/changy/cli/changelog.py
+-rw-r--r--   0        0        0      200 2024-05-31 11:17:29.567136 changy-0.1.2/changy/cli/unreleased.py
+-rw-r--r--   0        0        0      145 2024-05-31 11:17:29.567136 changy-0.1.2/changy/cli/version.py
+-rw-r--r--   0        0        0      477 2024-05-31 11:17:29.567136 changy-0.1.2/changy/constants.py
+-rw-r--r--   0        0        0     2942 2024-05-31 11:17:29.567136 changy-0.1.2/changy/logic.py
+-rw-r--r--   0        0        0      768 2024-05-31 11:17:29.567136 changy-0.1.2/changy/settings.py
+-rw-r--r--   0        0        0        0 2024-05-31 11:17:29.567136 changy-0.1.2/changy/tests/__init__.py
+-rw-r--r--   0        0        0       29 2024-05-31 11:17:29.567136 changy-0.1.2/changy/tests/test_logic.py
+-rw-r--r--   0        0        0     1953 2024-05-31 11:17:37.627241 changy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 changy-0.1.2/PKG-INFO
```

### Comparing `changy-0.1.1/LICENSE` & `changy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `changy-0.1.1/changy/logic.py` & `changy-0.1.2/changy/logic.py`

 * *Files identical despite different names*

### Comparing `changy-0.1.1/changy/settings.py` & `changy-0.1.2/changy/settings.py`

 * *Files identical despite different names*

### Comparing `changy-0.1.1/pyproject.toml` & `changy-0.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "changy"
-version = "0.1.1"
+version = "0.1.2"
 description = "Simplest changelog manager, oriented to human editing, not to special message formatting in commits and tags.."
 readme = "README.md"
 repository = "https://github.com/Tiendil/changy"
 authors = ["Aliaksei Yaletski (Tiendil) <a.eletsky@gmail.com>"]
 license = "BSD-3-Clause"
 keywords = ["changelog", "release-notes", "release-automation", "release-management", "changelog-generator", "changelog-formatter"]
 classifiers = [
```

### Comparing `changy-0.1.1/PKG-INFO` & `changy-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simplest changelog manager, oriented to human editing, not to special message formatting in commits and tags..
 Home-page: https://github.com/Tiendil/changy
 License: BSD-3-Clause
 Keywords: changelog,release-notes,release-automation,release-management,changelog-generator,changelog-formatter
 Author: Aliaksei Yaletski (Tiendil)
 Author-email: a.eletsky@gmail.com
 Requires-Python: >=3.12,<4.0
@@ -23,9 +23,14 @@
 Project-URL: Repository, https://github.com/Tiendil/changy
 Description-Content-Type: text/markdown
 
 # Changy
 
 Simplest changelog manager, oriented to human editing, not to special message formatting in commits.
 
-Inspired by [Changie](https://github.com/miniscruff/changie) but simpler, oriented to editing text files by hand: without cli commands to input changes, without strict messages format, etc.
+Inspired by
+
+- [Changie](https://github.com/miniscruff/changie)
+- [Towncrier](https://github.com/twisted/towncrier)
+
+But simpler, oriented to editing text files by hand: without cli commands to input changes, without strict messages format, etc.
```

