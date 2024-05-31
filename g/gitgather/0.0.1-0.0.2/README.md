# Comparing `tmp/gitgather-0.0.1.tar.gz` & `tmp/gitgather-0.0.2.tar.gz`

## Comparing `gitgather-0.0.1.tar` & `gitgather-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 gitgather-0.0.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gitgather-0.0.1/src/gitgather/__init__.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 gitgather-0.0.1/src/gitgather/__main__.py
--rw-r--r--   0        0        0    10655 2020-02-02 00:00:00.000000 gitgather-0.0.1/src/gitgather/gather.py
--rw-r--r--   0        0        0    14197 2020-02-02 00:00:00.000000 gitgather-0.0.1/tests/test_gitgather.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 gitgather-0.0.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gitgather-0.0.1/LICENSE
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 gitgather-0.0.1/README.md
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 gitgather-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 gitgather-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 gitgather-0.0.2/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gitgather-0.0.2/src/gitgather/__init__.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 gitgather-0.0.2/src/gitgather/__main__.py
+-rw-r--r--   0        0        0    10739 2020-02-02 00:00:00.000000 gitgather-0.0.2/src/gitgather/gather.py
+-rw-r--r--   0        0        0    14197 2020-02-02 00:00:00.000000 gitgather-0.0.2/tests/test_gitgather.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 gitgather-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gitgather-0.0.2/LICENSE
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 gitgather-0.0.2/README.md
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 gitgather-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 gitgather-0.0.2/PKG-INFO
```

### Comparing `gitgather-0.0.1/src/gitgather/__main__.py` & `gitgather-0.0.2/src/gitgather/__main__.py`

 * *Files identical despite different names*

### Comparing `gitgather-0.0.1/src/gitgather/gather.py` & `gitgather-0.0.2/src/gitgather/gather.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import subprocess
 import os
 import logging
 import fnmatch
 from typing import LiteralString
 
-logging.basicConfig(level=logging.DEBUG)
+# Initialize the logger
 logger = logging.getLogger(__name__)
 
 
 def capture_tree_output(repo_path, filtered_file_paths):
     """Capture the directory tree structure using the filtered file paths."""
     tree_lines = ["."]
     path_tree = {}
@@ -219,14 +219,17 @@
         no_dotfiles (bool, optional): Exclude dotfiles. Defaults to False.
         verbose (bool, optional): Enable verbose output. Defaults to False.
         tree_output (bool, optional): Include directory tree structure in the output. Defaults to True.
 
     Returns:
         None
     """
+    log_level = logging.DEBUG if verbose else logging.INFO
+    logging.basicConfig(level=log_level)
+
     # Get all file paths in the repository
     all_file_paths = [
         os.path.join(dp, f)
         for dp, _, filenames in os.walk(repo_path)
         for f in filenames
     ]
     logger.debug("All file paths: %s", all_file_paths)
```

### Comparing `gitgather-0.0.1/tests/test_gitgather.py` & `gitgather-0.0.2/tests/test_gitgather.py`

 * *Files identical despite different names*

### Comparing `gitgather-0.0.1/.gitignore` & `gitgather-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gitgather-0.0.1/LICENSE` & `gitgather-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gitgather-0.0.1/pyproject.toml` & `gitgather-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gitgather"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name = "claysauruswrecks", email = "44852834+claysauruswrecks@users.noreply.github.com" },
 ]
 description = "A simple tool to gather source code from a local repo or folder into a single file for LLM context windows."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

