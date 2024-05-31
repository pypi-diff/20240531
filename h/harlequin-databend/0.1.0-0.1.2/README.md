# Comparing `tmp/harlequin_databend-0.1.0.tar.gz` & `tmp/harlequin_databend-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harlequin_databend-0.1.0.tar", max compression
+gzip compressed data, was "harlequin_databend-0.1.2.tar", max compression
```

## Comparing `harlequin_databend-0.1.0.tar` & `harlequin_databend-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0     1463 2024-05-30 06:52:19.611002 harlequin_databend-0.1.0/README.md
--rwxr-xr-x   0        0        0     1472 2024-05-30 07:03:48.820741 harlequin_databend-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0      104 2024-05-30 06:52:19.620915 harlequin_databend-0.1.0/src/harlequin_databend/__init__.py
--rwxr-xr-x   0        0        0     7197 2024-05-30 06:52:19.631028 harlequin_databend-0.1.0/src/harlequin_databend/adapter.py
--rwxr-xr-x   0        0        0     1172 2024-05-30 06:52:19.631028 harlequin_databend-0.1.0/src/harlequin_databend/cli_options.py
--rwxr-xr-x   0        0        0     1397 2024-05-30 06:52:19.631028 harlequin_databend-0.1.0/src/harlequin_databend/completions.py
--rwxr-xr-x   0        0        0        0 2024-05-30 06:52:19.640940 harlequin_databend-0.1.0/src/harlequin_databend/py.typed
--rw-r--r--   0        0        0     2121 1970-01-01 00:00:00.000000 harlequin_databend-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1463 2024-05-27 16:58:44.635010 harlequin_databend-0.1.2/README.md
+-rw-r--r--   0        0        0     1472 2024-05-30 17:14:10.779529 harlequin_databend-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      104 2024-05-27 13:37:37.195474 harlequin_databend-0.1.2/src/harlequin_databend/__init__.py
+-rw-r--r--   0        0        0     7197 2024-05-27 16:20:29.051820 harlequin_databend-0.1.2/src/harlequin_databend/adapter.py
+-rw-r--r--   0        0        0     1172 2024-05-26 09:35:57.962231 harlequin_databend-0.1.2/src/harlequin_databend/cli_options.py
+-rw-r--r--   0        0        0     1397 2024-05-27 16:20:39.840201 harlequin_databend-0.1.2/src/harlequin_databend/completions.py
+-rw-r--r--   0        0        0        0 2024-05-26 09:00:04.820057 harlequin_databend-0.1.2/src/harlequin_databend/py.typed
+-rw-r--r--   0        0        0     2121 1970-01-01 00:00:00.000000 harlequin_databend-0.1.2/PKG-INFO
```

### Comparing `harlequin_databend-0.1.0/README.md` & `harlequin_databend-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `harlequin_databend-0.1.0/pyproject.toml` & `harlequin_databend-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "harlequin-databend"
-version = "0.1.0"
+version = "0.1.2"
 description = "A Harlequin adapter for Databend."
 authors = ["hanxuanliang <hxuanliang@163.com>"]
 license = "MIT"
 keywords = ["databend", "harlequin"]
 homepage = "https://github.com/datafuselabs/databend"
 readme = "README.md"
 packages = [{ include = "harlequin_databend", from = "src" }]
```

### Comparing `harlequin_databend-0.1.0/src/harlequin_databend/adapter.py` & `harlequin_databend-0.1.2/src/harlequin_databend/adapter.py`

 * *Files identical despite different names*

### Comparing `harlequin_databend-0.1.0/src/harlequin_databend/cli_options.py` & `harlequin_databend-0.1.2/src/harlequin_databend/cli_options.py`

 * *Files identical despite different names*

### Comparing `harlequin_databend-0.1.0/src/harlequin_databend/completions.py` & `harlequin_databend-0.1.2/src/harlequin_databend/completions.py`

 * *Files identical despite different names*

### Comparing `harlequin_databend-0.1.0/PKG-INFO` & `harlequin_databend-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harlequin-databend
-Version: 0.1.0
+Version: 0.1.2
 Summary: A Harlequin adapter for Databend.
 Home-page: https://github.com/datafuselabs/databend
 License: MIT
 Keywords: databend,harlequin
 Author: hanxuanliang
 Author-email: hxuanliang@163.com
 Requires-Python: >=3.10,<4.0
```

