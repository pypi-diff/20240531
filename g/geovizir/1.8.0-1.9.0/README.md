# Comparing `tmp/geovizir-1.8.0.tar.gz` & `tmp/geovizir-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geovizir-1.8.0.tar", max compression
+gzip compressed data, was "geovizir-1.9.0.tar", max compression
```

## Comparing `geovizir-1.8.0.tar` & `geovizir-1.9.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0     1074 2024-05-14 06:46:46.938838 geovizir-1.8.0/LICENSE
--rw-r--r--   0        0        0      946 2024-05-14 06:46:46.938838 geovizir-1.8.0/README.md
--rw-r--r--   0        0        0     1290 2024-05-14 06:47:26.810672 geovizir-1.8.0/pyproject.toml
--rw-r--r--   0        0        0      231 2024-05-14 06:46:46.938838 geovizir-1.8.0/src/geovizir/__init__.py
--rw-r--r--   0        0        0     1767 2024-05-14 06:46:46.938838 geovizir-1.8.0/src/geovizir/data.py
--rw-r--r--   0        0        0     1312 2024-05-14 06:46:46.938838 geovizir-1.8.0/src/geovizir/dplyr.py
--rw-r--r--   0        0        0     1996 2024-05-14 06:46:46.938838 geovizir-1.8.0/src/geovizir/features.py
--rw-r--r--   0        0        0     1086 2024-05-14 06:46:46.938838 geovizir-1.8.0/src/geovizir/scales.py
--rw-r--r--   0        0        0     1651 1970-01-01 00:00:00.000000 geovizir-1.8.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1074 2024-05-31 13:21:34.802317 geovizir-1.9.0/LICENSE
+-rw-r--r--   0        0        0      946 2024-05-31 13:21:34.802317 geovizir-1.9.0/README.md
+-rw-r--r--   0        0        0     1361 2024-05-31 13:22:12.485993 geovizir-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-05-31 13:21:34.802317 geovizir-1.9.0/src/geovizir/__init__.py
+-rw-r--r--   0        0        0     1767 2024-05-31 13:21:34.802317 geovizir-1.9.0/src/geovizir/data.py
+-rw-r--r--   0        0        0     1312 2024-05-31 13:21:34.802317 geovizir-1.9.0/src/geovizir/dplyr.py
+-rw-r--r--   0        0        0     1996 2024-05-31 13:21:34.802317 geovizir-1.9.0/src/geovizir/features.py
+-rw-r--r--   0        0        0     1086 2024-05-31 13:21:34.802317 geovizir-1.9.0/src/geovizir/scales.py
+-rw-r--r--   0        0        0     1651 1970-01-01 00:00:00.000000 geovizir-1.9.0/PKG-INFO
```

### Comparing `geovizir-1.8.0/LICENSE` & `geovizir-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geovizir-1.8.0/README.md` & `geovizir-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `geovizir-1.8.0/pyproject.toml` & `geovizir-1.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geovizir"
-version = "1.8.0"
+version = "1.9.0"
 description = "Support package for geo visuals."
 authors = ["Pascal Burkhard"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -21,14 +21,18 @@
 pytest-cov = "^4.1.0"
 pytest = "^7.4.3"
 myst-nb = {version = "^1.0.0", python = "^3.9"}
 sphinx-autoapi = "^3.0.0"
 sphinx-rtd-theme = "^2.0.0"
 pandas = "^2.1.4"
 
+
+[tool.poetry.group.doc.dependencies]
+pydata-sphinx-theme = "^0.15.3"
+
 [tool.semantic_release]
 branch = "main"                             # branch to make releases of
 changelog_file = "CHANGELOG.md"             # changelog file
 build_command = "poetry build"              # build command
 dist_path = "dist/"                         # where to put dists
 upload_to_release = true                    # auto-create GitHub release
 upload_to_pypi = false                      # don't auto-upload to PyPI
```

### Comparing `geovizir-1.8.0/src/geovizir/data.py` & `geovizir-1.9.0/src/geovizir/data.py`

 * *Files identical despite different names*

### Comparing `geovizir-1.8.0/src/geovizir/dplyr.py` & `geovizir-1.9.0/src/geovizir/dplyr.py`

 * *Files identical despite different names*

### Comparing `geovizir-1.8.0/src/geovizir/features.py` & `geovizir-1.9.0/src/geovizir/features.py`

 * *Files identical despite different names*

### Comparing `geovizir-1.8.0/src/geovizir/scales.py` & `geovizir-1.9.0/src/geovizir/scales.py`

 * *Files identical despite different names*

### Comparing `geovizir-1.8.0/PKG-INFO` & `geovizir-1.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geovizir
-Version: 1.8.0
+Version: 1.9.0
 Summary: Support package for geo visuals.
 License: MIT
 Author: Pascal Burkhard
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

