# Comparing `tmp/svn2git-0.8.5.tar.gz` & `tmp/svn2git-0.8.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svn2git-0.8.5.tar", max compression
+gzip compressed data, was "svn2git-0.8.5rc1.tar", max compression
```

## Comparing `svn2git-0.8.5.tar` & `svn2git-0.8.5rc1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11912 2023-12-11 15:40:48.530207 svn2git-0.8.5/README.md
--rw-r--r--   0        0        0     2427 2023-12-11 15:41:06.458185 svn2git-0.8.5/pyproject.toml
--rw-r--r--   0        0        0      441 2023-12-11 15:41:06.458185 svn2git-0.8.5/svn2git/__init__.py
--rw-r--r--   0        0        0     9888 2023-12-11 15:40:48.534206 svn2git-0.8.5/svn2git/__main__.py
--rw-r--r--   0        0        0      714 2023-12-11 15:40:48.534206 svn2git-0.8.5/svn2git/env_default_action.py
--rw-r--r--   0        0        0    21963 2023-12-11 15:40:48.534206 svn2git-0.8.5/svn2git/git.py
--rw-r--r--   0        0        0     2972 2023-12-11 15:40:48.534206 svn2git-0.8.5/svn2git/options.py
--rw-r--r--   0        0        0     1730 2023-12-11 15:40:48.534206 svn2git-0.8.5/svn2git/svn.py
--rw-r--r--   0        0        0     5934 2023-12-11 15:40:48.534206 svn2git-0.8.5/svn2git/svn_store_plaintext_password.py
--rw-r--r--   0        0        0     1389 2023-12-11 15:40:48.534206 svn2git-0.8.5/svn2git/utils.py
--rw-r--r--   0        0        0    12469 1970-01-01 00:00:00.000000 svn2git-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0    11912 2023-12-05 08:52:27.832461 svn2git-0.8.5rc1/README.md
+-rw-r--r--   0        0        0     2432 2023-12-05 08:53:01.008400 svn2git-0.8.5rc1/pyproject.toml
+-rw-r--r--   0        0        0      446 2023-12-05 08:53:01.008400 svn2git-0.8.5rc1/svn2git/__init__.py
+-rw-r--r--   0        0        0     9888 2023-12-05 08:52:27.832461 svn2git-0.8.5rc1/svn2git/__main__.py
+-rw-r--r--   0        0        0      714 2023-12-05 08:52:27.836461 svn2git-0.8.5rc1/svn2git/env_default_action.py
+-rw-r--r--   0        0        0    21963 2023-12-05 08:52:27.836461 svn2git-0.8.5rc1/svn2git/git.py
+-rw-r--r--   0        0        0     2972 2023-12-05 08:52:27.836461 svn2git-0.8.5rc1/svn2git/options.py
+-rw-r--r--   0        0        0     1730 2023-12-05 08:52:27.836461 svn2git-0.8.5rc1/svn2git/svn.py
+-rw-r--r--   0        0        0     5934 2023-12-05 08:52:27.836461 svn2git-0.8.5rc1/svn2git/svn_store_plaintext_password.py
+-rw-r--r--   0        0        0     1389 2023-12-05 08:52:27.836461 svn2git-0.8.5rc1/svn2git/utils.py
+-rw-r--r--   0        0        0    12472 1970-01-01 00:00:00.000000 svn2git-0.8.5rc1/PKG-INFO
```

### Comparing `svn2git-0.8.5/README.md` & `svn2git-0.8.5rc1/README.md`

 * *Files identical despite different names*

### Comparing `svn2git-0.8.5/pyproject.toml` & `svn2git-0.8.5rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "svn2git"
-version = "0.8.5"
+version = "0.8.5-rc.1"
 description = "A tool for migrating svn projects to git"
 license = "MIT"
 authors = ["Pascal Helmer <pascal@pascalhelmer.de>"]
 readme = "README.md"
 homepage = "https://helmergmbh.github.io/svn2git/"
 repository = "https://github.com/helmergmbh/svn2git"
 packages = [{ include = "svn2git" }]
@@ -12,31 +12,31 @@
 [tool.poetry.scripts]
 svn2git = "svn2git.__main__:main"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "3.6.0"
+pre-commit = "3.5.0"
 flake8 = "6.1.0"
 black = "23.11.0"
-isort = "5.13.0"
+isort = "5.12.0"
 mypy = "1.7.1"
 pytest = "7.4.3"
 pytest-asyncio = "0.23.2"
 pytest-cov = "4.1.0"
-python-semantic-release = "8.5.0"
+python-semantic-release = "8.3.0"
 sphinx = "7.2.6"
 sphinx-rtd-theme = "2.0.0"
 sphinx-autodoc-typehints = "1.25.2"
 livereload = "2.6.3"
 pytest-watch = "4.2.0"
 pytest-sugar = "0.9.7"
-pytest-icdiff = "0.9"
-bandit = { extras = ["toml"], version = "1.7.6" }
+pytest-icdiff = "0.8"
+bandit = { extras = ["toml"], version = "1.7.5" }
 enum-tools = { extras = ["sphinx"], version = "0.11.0" }
 sphinx-material = { git = "https://github.com/bashtage/sphinx-material.git" }
 twine = "4.0.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `svn2git-0.8.5/svn2git/__main__.py` & `svn2git-0.8.5rc1/svn2git/__main__.py`

 * *Files identical despite different names*

### Comparing `svn2git-0.8.5/svn2git/env_default_action.py` & `svn2git-0.8.5rc1/svn2git/env_default_action.py`

 * *Files identical despite different names*

### Comparing `svn2git-0.8.5/svn2git/git.py` & `svn2git-0.8.5rc1/svn2git/git.py`

 * *Files identical despite different names*

### Comparing `svn2git-0.8.5/svn2git/options.py` & `svn2git-0.8.5rc1/svn2git/options.py`

 * *Files identical despite different names*

### Comparing `svn2git-0.8.5/svn2git/svn.py` & `svn2git-0.8.5rc1/svn2git/svn.py`

 * *Files identical despite different names*

### Comparing `svn2git-0.8.5/svn2git/svn_store_plaintext_password.py` & `svn2git-0.8.5rc1/svn2git/svn_store_plaintext_password.py`

 * *Files identical despite different names*

### Comparing `svn2git-0.8.5/svn2git/utils.py` & `svn2git-0.8.5rc1/svn2git/utils.py`

 * *Files identical despite different names*

### Comparing `svn2git-0.8.5/PKG-INFO` & `svn2git-0.8.5rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svn2git
-Version: 0.8.5
+Version: 0.8.5rc1
 Summary: A tool for migrating svn projects to git
 Home-page: https://helmergmbh.github.io/svn2git/
 License: MIT
 Author: Pascal Helmer
 Author-email: pascal@pascalhelmer.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

