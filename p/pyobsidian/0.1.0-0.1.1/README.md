# Comparing `tmp/pyobsidian-0.1.0.tar.gz` & `tmp/pyobsidian-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobsidian-0.1.0.tar", max compression
+gzip compressed data, was "pyobsidian-0.1.1.tar", max compression
```

## Comparing `pyobsidian-0.1.0.tar` & `pyobsidian-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1098 2024-05-30 20:18:59.408210 pyobsidian-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2024-05-30 20:08:41.859655 pyobsidian-0.1.0/pyobsidian/__init__.py
--rw-r--r--   0        0        0     4044 2024-05-30 20:08:41.859655 pyobsidian-0.1.0/pyobsidian/filter.py
--rw-r--r--   0        0        0    14456 2024-05-30 20:08:41.859655 pyobsidian-0.1.0/pyobsidian/note.py
--rw-r--r--   0        0        0    10829 2024-05-30 20:23:57.264147 pyobsidian-0.1.0/pyobsidian/searchby.py
--rw-r--r--   0        0        0     7317 2024-05-30 20:24:02.076702 pyobsidian-0.1.0/pyobsidian/vault.py
--rw-r--r--   0        0        0      763 2024-05-30 20:28:49.338659 pyobsidian-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1539 2024-05-30 20:21:51.172239 pyobsidian-0.1.0/README.md
--rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 pyobsidian-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-05-30 20:18:59.408210 pyobsidian-0.1.1/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-30 20:08:41.859655 pyobsidian-0.1.1/pyobsidian/__init__.py
+-rw-r--r--   0        0        0     4044 2024-05-30 20:08:41.859655 pyobsidian-0.1.1/pyobsidian/filter.py
+-rw-r--r--   0        0        0    14456 2024-05-30 20:08:41.859655 pyobsidian-0.1.1/pyobsidian/note.py
+-rw-r--r--   0        0        0    10829 2024-05-30 20:23:57.264147 pyobsidian-0.1.1/pyobsidian/searchby.py
+-rw-r--r--   0        0        0     7317 2024-05-30 20:24:02.076702 pyobsidian-0.1.1/pyobsidian/vault.py
+-rw-r--r--   0        0        0      801 2024-05-31 00:00:11.872907 pyobsidian-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1539 2024-05-30 20:21:51.172239 pyobsidian-0.1.1/README.md
+-rw-r--r--   0        0        0     2113 1970-01-01 00:00:00.000000 pyobsidian-0.1.1/PKG-INFO
```

### Comparing `pyobsidian-0.1.0/LICENSE` & `pyobsidian-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobsidian-0.1.0/pyobsidian/filter.py` & `pyobsidian-0.1.1/pyobsidian/filter.py`

 * *Files identical despite different names*

### Comparing `pyobsidian-0.1.0/pyobsidian/note.py` & `pyobsidian-0.1.1/pyobsidian/note.py`

 * *Files identical despite different names*

### Comparing `pyobsidian-0.1.0/pyobsidian/searchby.py` & `pyobsidian-0.1.1/pyobsidian/searchby.py`

 * *Files identical despite different names*

### Comparing `pyobsidian-0.1.0/pyobsidian/vault.py` & `pyobsidian-0.1.1/pyobsidian/vault.py`

 * *Files identical despite different names*

### Comparing `pyobsidian-0.1.0/pyproject.toml` & `pyobsidian-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [tool.poetry]
 name = "pyobsidian"
-version = "0.1.0"
+version = "0.1.1"
 description = "Find and manipulate any note in your Obsidian vault"
 authors = [
     "Matheus S. Rodrigues <matheus.srodr@gmail.com>"
 ]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/matheussrod/pyobsidian"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-pytest = "^8.2.1"
-mkdocs = "^1.6.0"
 pyyaml = "^6.0.1"
+
+[tool.poetry.group.dev.dependencies]
+mkdocs = "^1.6.0"
+pytest = "^8.2.1"
+pytest-cov = "^5.0.0"
 mypy = "^1.10.0"
 types-pyyaml = "^6.0.12.20240311"
-pytest-cov = "^5.0.0"
 mkdocs-material = "^9.5.25"
 mkdocs-include-dir-to-nav = "^1.2.0"
 mkdocstrings = {extras = ["python"], version = "^0.25.1"}
 
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = "--cov --cov-report term-missing"
```

### Comparing `pyobsidian-0.1.0/README.md` & `pyobsidian-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyobsidian-0.1.0/PKG-INFO` & `pyobsidian-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,21 @@
 Metadata-Version: 2.1
 Name: pyobsidian
-Version: 0.1.0
+Version: 0.1.1
 Summary: Find and manipulate any note in your Obsidian vault
 Home-page: https://github.com/matheussrod/pyobsidian
 License: MIT
 Author: Matheus S. Rodrigues
 Author-email: matheus.srodr@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: mkdocs (>=1.6.0,<2.0.0)
-Requires-Dist: mkdocs-include-dir-to-nav (>=1.2.0,<2.0.0)
-Requires-Dist: mkdocs-material (>=9.5.25,<10.0.0)
-Requires-Dist: mkdocstrings[python] (>=0.25.1,<0.26.0)
-Requires-Dist: mypy (>=1.10.0,<2.0.0)
-Requires-Dist: pytest (>=8.2.1,<9.0.0)
-Requires-Dist: pytest-cov (>=5.0.0,<6.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Requires-Dist: types-pyyaml (>=6.0.12.20240311,<7.0.0.0)
 Project-URL: Repository, https://github.com/matheussrod/pyobsidian
 Description-Content-Type: text/markdown
 
 # pyobsidian
 
 ## Overview
```

