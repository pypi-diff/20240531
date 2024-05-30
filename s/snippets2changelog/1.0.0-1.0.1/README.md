# Comparing `tmp/snippets2changelog-1.0.0.tar.gz` & `tmp/snippets2changelog-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snippets2changelog-1.0.0.tar", max compression
+gzip compressed data, was "snippets2changelog-1.0.1.tar", max compression
```

## Comparing `snippets2changelog-1.0.0.tar` & `snippets2changelog-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1198 2024-05-30 22:18:21.490965 snippets2changelog-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     3205 2024-05-30 22:18:21.490965 snippets2changelog-1.0.0/README.md
--rw-r--r--   0        0        0     3386 2024-05-30 22:18:38.539173 snippets2changelog-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-30 22:18:21.490965 snippets2changelog-1.0.0/snippets2changelog/__init__.py
--rwxr-xr-x   0        0        0     4333 2024-05-30 22:18:21.490965 snippets2changelog-1.0.0/snippets2changelog/cli.py
--rw-r--r--   0        0        0     4262 2024-05-30 22:18:21.490965 snippets2changelog-1.0.0/snippets2changelog/collector.py
--rw-r--r--   0        0        0     1991 2024-05-30 22:18:21.490965 snippets2changelog-1.0.0/snippets2changelog/common.py
--rw-r--r--   0        0        0     5172 2024-05-30 22:18:21.490965 snippets2changelog-1.0.0/snippets2changelog/creator.py
--rw-r--r--   0        0        0     2817 2024-05-30 22:18:21.490965 snippets2changelog-1.0.0/snippets2changelog/parser.py
--rw-r--r--   0        0        0      112 2024-05-30 22:18:21.490965 snippets2changelog-1.0.0/snippets2changelog/templates/snippet.md.template
--rw-r--r--   0        0        0      124 2024-05-30 22:18:38.015166 snippets2changelog-1.0.0/snippets2changelog/version.py
--rw-r--r--   0        0        0     4407 1970-01-01 00:00:00.000000 snippets2changelog-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1198 2024-05-30 22:38:13.227014 snippets2changelog-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     3205 2024-05-30 22:38:13.227014 snippets2changelog-1.0.1/README.md
+-rw-r--r--   0        0        0     3386 2024-05-30 22:38:29.518896 snippets2changelog-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 22:38:13.227014 snippets2changelog-1.0.1/snippets2changelog/__init__.py
+-rwxr-xr-x   0        0        0     4333 2024-05-30 22:38:13.231014 snippets2changelog-1.0.1/snippets2changelog/cli.py
+-rw-r--r--   0        0        0     4262 2024-05-30 22:38:13.231014 snippets2changelog-1.0.1/snippets2changelog/collector.py
+-rw-r--r--   0        0        0     1991 2024-05-30 22:38:13.231014 snippets2changelog-1.0.1/snippets2changelog/common.py
+-rw-r--r--   0        0        0     5172 2024-05-30 22:38:13.231014 snippets2changelog-1.0.1/snippets2changelog/creator.py
+-rw-r--r--   0        0        0     2817 2024-05-30 22:38:13.231014 snippets2changelog-1.0.1/snippets2changelog/parser.py
+-rw-r--r--   0        0        0      112 2024-05-30 22:38:13.231014 snippets2changelog-1.0.1/snippets2changelog/templates/snippet.md.template
+-rw-r--r--   0        0        0      124 2024-05-30 22:38:28.998900 snippets2changelog-1.0.1/snippets2changelog/version.py
+-rw-r--r--   0        0        0     4407 1970-01-01 00:00:00.000000 snippets2changelog-1.0.1/PKG-INFO
```

### Comparing `snippets2changelog-1.0.0/LICENSE.txt` & `snippets2changelog-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snippets2changelog-1.0.0/README.md` & `snippets2changelog-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `snippets2changelog-1.0.0/pyproject.toml` & `snippets2changelog-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snippets2changelog"
-version = "1.0.0" # will-be-updated-automatically
+version = "1.0.1" # will-be-updated-automatically
 description =  "Generate a changelog from individual snippets"
 authors = ["brainelectronics <info@brainelectronics.de>"]
 repository = "https://github.com/brainelectronics/snippets2changelog"
 readme = "README.md"
 license = "MIT"
 packages = [
   { include = "snippets2changelog/**/*.py" }
```

### Comparing `snippets2changelog-1.0.0/snippets2changelog/cli.py` & `snippets2changelog-1.0.1/snippets2changelog/cli.py`

 * *Files identical despite different names*

### Comparing `snippets2changelog-1.0.0/snippets2changelog/collector.py` & `snippets2changelog-1.0.1/snippets2changelog/collector.py`

 * *Files identical despite different names*

### Comparing `snippets2changelog-1.0.0/snippets2changelog/common.py` & `snippets2changelog-1.0.1/snippets2changelog/common.py`

 * *Files identical despite different names*

### Comparing `snippets2changelog-1.0.0/snippets2changelog/creator.py` & `snippets2changelog-1.0.1/snippets2changelog/creator.py`

 * *Files identical despite different names*

### Comparing `snippets2changelog-1.0.0/snippets2changelog/parser.py` & `snippets2changelog-1.0.1/snippets2changelog/parser.py`

 * *Files identical despite different names*

### Comparing `snippets2changelog-1.0.0/PKG-INFO` & `snippets2changelog-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snippets2changelog
-Version: 1.0.0
+Version: 1.0.1
 Summary: Generate a changelog from individual snippets
 Home-page: https://github.com/brainelectronics/snippets2changelog
 License: MIT
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

