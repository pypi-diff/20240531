# Comparing `tmp/fvupgrader-1.0.8.tar.gz` & `tmp/fvupgrader-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fvupgrader-1.0.8.tar", max compression
+gzip compressed data, was "fvupgrader-1.0.9.tar", max compression
```

## Comparing `fvupgrader-1.0.8.tar` & `fvupgrader-1.0.9.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2176 2024-03-20 09:55:58.427013 fvupgrader-1.0.8/README.md
--rwxr-xr-x   0        0        0     8424 2024-03-20 09:55:58.427013 fvupgrader-1.0.8/fvupgrader.py
--rw-r--r--   0        0        0      589 2024-03-20 09:55:58.427013 fvupgrader-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     2922 1970-01-01 00:00:00.000000 fvupgrader-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     2176 2024-05-31 15:57:39.860696 fvupgrader-1.0.9/README.md
+-rwxr-xr-x   0        0        0     8482 2024-05-31 15:57:39.860696 fvupgrader-1.0.9/fvupgrader.py
+-rw-r--r--   0        0        0      589 2024-05-31 15:57:39.860696 fvupgrader-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2922 1970-01-01 00:00:00.000000 fvupgrader-1.0.9/PKG-INFO
```

### Comparing `fvupgrader-1.0.8/README.md` & `fvupgrader-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fvupgrader-1.0.8/fvupgrader.py` & `fvupgrader-1.0.9/fvupgrader.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import os.path
 import re
 from argparse import ArgumentParser
 
 version_regex: str = r"version: (\d+\.\d+\.\d+\+\d+)"
 version_file: str = "pubspec.yaml"
-version_number: str = "1.0.8"
+version_number: str = "1.0.9"
 
 
 class GitOperationException(Exception):
     """Exception raised for Git operation errors.
 
     Attributes:
         message -- explanation of the error
@@ -115,14 +115,15 @@
     if not parsed_args.no_tag:
         os.system(f"git -C {directory_path} tag {new_version}")
         print(f"Tagged release {new_version}")
 
     # Push the changes
     if not parsed_args.no_push:
         os.system(f"git -C {directory_path} push")
+        os.system(f"git -C {directory_path} push --tags")
 
 
 def is_dir_git_repo(directory_path: str) -> bool:
     """
     Check if a directory is a Git repository.
 
     Args:
```

### Comparing `fvupgrader-1.0.8/pyproject.toml` & `fvupgrader-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fvupgrader"
-version = "1.0.8"
+version = "1.0.9"
 description = "fvupgrader streamlines version upgrades in Flutter projects by automatically updating the pubspec.yaml file and tagging changes in Git. Simplify version control for your Flutter apps, packages, and plugins with this versatile tool."
 authors = ["Emilio Dalla Torre <info@emiliodallatorre.it>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `fvupgrader-1.0.8/PKG-INFO` & `fvupgrader-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fvupgrader
-Version: 1.0.8
+Version: 1.0.9
 Summary: fvupgrader streamlines version upgrades in Flutter projects by automatically updating the pubspec.yaml file and tagging changes in Git. Simplify version control for your Flutter apps, packages, and plugins with this versatile tool.
 License: MIT
 Author: Emilio Dalla Torre
 Author-email: info@emiliodallatorre.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

