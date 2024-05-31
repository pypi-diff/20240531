# Comparing `tmp/svn2git-0.8.5rc2.tar.gz` & `tmp/svn2git-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svn2git-0.8.5rc2.tar", max compression
+gzip compressed data, was "svn2git-0.9.0.tar", max compression
```

## Comparing `svn2git-0.8.5rc2.tar` & `svn2git-0.9.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11912 2024-05-31 11:19:21.472481 svn2git-0.8.5rc2/README.md
--rw-r--r--   0        0        0     2432 2024-05-31 11:19:48.700613 svn2git-0.8.5rc2/pyproject.toml
--rw-r--r--   0        0        0      446 2024-05-31 11:19:48.700613 svn2git-0.8.5rc2/svn2git/__init__.py
--rw-r--r--   0        0        0     9888 2024-05-31 11:19:21.472481 svn2git-0.8.5rc2/svn2git/__main__.py
--rw-r--r--   0        0        0      714 2024-05-31 11:19:21.472481 svn2git-0.8.5rc2/svn2git/env_default_action.py
--rw-r--r--   0        0        0    21934 2024-05-31 11:19:21.472481 svn2git-0.8.5rc2/svn2git/git.py
--rw-r--r--   0        0        0     2972 2024-05-31 11:19:21.472481 svn2git-0.8.5rc2/svn2git/options.py
--rw-r--r--   0        0        0     1730 2024-05-31 11:19:21.472481 svn2git-0.8.5rc2/svn2git/svn.py
--rw-r--r--   0        0        0     5934 2024-05-31 11:19:21.472481 svn2git-0.8.5rc2/svn2git/svn_store_plaintext_password.py
--rw-r--r--   0        0        0     1389 2024-05-31 11:19:21.472481 svn2git-0.8.5rc2/svn2git/utils.py
--rw-r--r--   0        0        0    12472 1970-01-01 00:00:00.000000 svn2git-0.8.5rc2/PKG-INFO
+-rw-r--r--   0        0        0    11912 2024-05-31 12:28:17.833392 svn2git-0.9.0/README.md
+-rw-r--r--   0        0        0     2427 2024-05-31 12:28:35.669385 svn2git-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      441 2024-05-31 12:28:35.669385 svn2git-0.9.0/svn2git/__init__.py
+-rw-r--r--   0        0        0     9888 2024-05-31 12:28:17.837391 svn2git-0.9.0/svn2git/__main__.py
+-rw-r--r--   0        0        0      714 2024-05-31 12:28:17.837391 svn2git-0.9.0/svn2git/env_default_action.py
+-rw-r--r--   0        0        0    21934 2024-05-31 12:28:17.837391 svn2git-0.9.0/svn2git/git.py
+-rw-r--r--   0        0        0     2972 2024-05-31 12:28:17.837391 svn2git-0.9.0/svn2git/options.py
+-rw-r--r--   0        0        0     1730 2024-05-31 12:28:17.837391 svn2git-0.9.0/svn2git/svn.py
+-rw-r--r--   0        0        0     5934 2024-05-31 12:28:17.837391 svn2git-0.9.0/svn2git/svn_store_plaintext_password.py
+-rw-r--r--   0        0        0     1389 2024-05-31 12:28:17.837391 svn2git-0.9.0/svn2git/utils.py
+-rw-r--r--   0        0        0    12469 1970-01-01 00:00:00.000000 svn2git-0.9.0/PKG-INFO
```

### Comparing `svn2git-0.8.5rc2/README.md` & `svn2git-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `svn2git-0.8.5rc2/pyproject.toml` & `svn2git-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "svn2git"
-version = "0.8.5-rc.2"
+version = "0.9.0"
 description = "A tool for migrating svn projects to git"
 license = "MIT"
 authors = ["Pascal Helmer <pascal@pascalhelmer.de>"]
 readme = "README.md"
 homepage = "https://helmergmbh.github.io/svn2git/"
 repository = "https://github.com/helmergmbh/svn2git"
 packages = [{ include = "svn2git" }]
```

### Comparing `svn2git-0.8.5rc2/svn2git/__main__.py` & `svn2git-0.9.0/svn2git/__main__.py`

 * *Files identical despite different names*

### Comparing `svn2git-0.8.5rc2/svn2git/env_default_action.py` & `svn2git-0.9.0/svn2git/env_default_action.py`

 * *Files identical despite different names*

### Comparing `svn2git-0.8.5rc2/svn2git/git.py` & `svn2git-0.9.0/svn2git/git.py`

 * *Files identical despite different names*

### Comparing `svn2git-0.8.5rc2/svn2git/options.py` & `svn2git-0.9.0/svn2git/options.py`

 * *Files identical despite different names*

### Comparing `svn2git-0.8.5rc2/svn2git/svn.py` & `svn2git-0.9.0/svn2git/svn.py`

 * *Files identical despite different names*

### Comparing `svn2git-0.8.5rc2/svn2git/svn_store_plaintext_password.py` & `svn2git-0.9.0/svn2git/svn_store_plaintext_password.py`

 * *Files identical despite different names*

### Comparing `svn2git-0.8.5rc2/svn2git/utils.py` & `svn2git-0.9.0/svn2git/utils.py`

 * *Files identical despite different names*

### Comparing `svn2git-0.8.5rc2/PKG-INFO` & `svn2git-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svn2git
-Version: 0.8.5rc2
+Version: 0.9.0
 Summary: A tool for migrating svn projects to git
 Home-page: https://helmergmbh.github.io/svn2git/
 License: MIT
 Author: Pascal Helmer
 Author-email: pascal@pascalhelmer.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

