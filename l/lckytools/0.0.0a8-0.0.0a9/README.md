# Comparing `tmp/lckytools-0.0.0a8.tar.gz` & `tmp/lckytools-0.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lckytools-0.0.0a8.tar", max compression
+gzip compressed data, was "lckytools-0.0.0a9.tar", max compression
```

## Comparing `lckytools-0.0.0a8.tar` & `lckytools-0.0.0a9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1096 2024-05-27 03:04:13.567796 lckytools-0.0.0a8/LICENSE
--rw-r--r--   0        0        0      516 2024-05-27 04:17:58.845240 lckytools-0.0.0a8/pyproject.toml
--rw-r--r--   0        0        0     1423 2024-05-27 01:01:39.126939 lckytools-0.0.0a8/README.md
--rw-r--r--   0        0        0        0 2024-05-27 02:47:26.411528 lckytools-0.0.0a8/src/lckytools/__init__.py
--rw-r--r--   0        0        0       42 2024-05-27 03:49:27.940843 lckytools-0.0.0a8/src/lckytools/hello.py
--rw-r--r--   0        0        0        0 2024-05-27 02:47:26.411528 lckytools-0.0.0a8/src/lckytools.ai/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 02:49:12.032838 lckytools-0.0.0a8/src/lckytools.ai/metrics/__init__.py
--rw-r--r--   0        0        0      911 2024-05-27 03:07:44.681865 lckytools-0.0.0a8/src/lckytools.ai/metrics/confusion_matrix.py
--rw-r--r--   0        0        0     2016 1970-01-01 00:00:00.000000 lckytools-0.0.0a8/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-05-27 03:04:13.567796 lckytools-0.0.0a9/LICENSE
+-rw-r--r--   0        0        0      516 2024-05-27 04:19:59.368124 lckytools-0.0.0a9/pyproject.toml
+-rw-r--r--   0        0        0     1423 2024-05-27 01:01:39.126939 lckytools-0.0.0a9/README.md
+-rw-r--r--   0        0        0       26 2024-05-27 04:19:54.197217 lckytools-0.0.0a9/src/lckytools/__init__.py
+-rw-r--r--   0        0        0       42 2024-05-27 03:49:27.940843 lckytools-0.0.0a9/src/lckytools/hello.py
+-rw-r--r--   0        0        0        0 2024-05-27 02:47:26.411528 lckytools-0.0.0a9/src/lckytools.ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 02:49:12.032838 lckytools-0.0.0a9/src/lckytools.ai/metrics/__init__.py
+-rw-r--r--   0        0        0      911 2024-05-27 03:07:44.681865 lckytools-0.0.0a9/src/lckytools.ai/metrics/confusion_matrix.py
+-rw-r--r--   0        0        0     2016 1970-01-01 00:00:00.000000 lckytools-0.0.0a9/PKG-INFO
```

### Comparing `lckytools-0.0.0a8/LICENSE` & `lckytools-0.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `lckytools-0.0.0a8/pyproject.toml` & `lckytools-0.0.0a9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lckytools"
-version = "0.0.0a8"
+version = "0.0.0a9"
 description = ""
 authors = ["LCKYN <T.Pawarit@lckyn.com>"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     { include = "lckytools", from = "src" },
```

### Comparing `lckytools-0.0.0a8/README.md` & `lckytools-0.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `lckytools-0.0.0a8/src/lckytools.ai/metrics/confusion_matrix.py` & `lckytools-0.0.0a9/src/lckytools.ai/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `lckytools-0.0.0a8/PKG-INFO` & `lckytools-0.0.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lckytools
-Version: 0.0.0a8
+Version: 0.0.0a9
 Summary: 
 License: MIT
 Author: LCKYN
 Author-email: T.Pawarit@lckyn.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

