# Comparing `tmp/satori_python_server-0.9.1.tar.gz` & `tmp/satori_python_server-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_python_server-0.9.1.tar", last modified: Wed Nov 29 15:18:04 2023, max compression
+gzip compressed data, was "satori_python_server-0.9.2.tar", last modified: Wed Dec  6 07:07:30 2023, max compression
```

## Comparing `satori_python_server-0.9.1.tar` & `satori_python_server-0.9.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      986 2023-11-29 15:17:50.874842 satori_python_server-0.9.1/.mina/server.toml
--rw-r--r--   0        0        0     1069 2023-11-29 15:17:50.874842 satori_python_server-0.9.1/LICENSE
--rw-r--r--   0        0        0     2662 2023-11-29 15:17:50.874842 satori_python_server-0.9.1/README.md
--rw-r--r--   0        0        0     2049 2023-11-29 15:18:04.762926 satori_python_server-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     8183 2023-11-29 15:17:50.878841 satori_python_server-0.9.1/src/satori/server/__init__.py
--rw-r--r--   0        0        0      936 2023-11-29 15:17:50.878841 satori_python_server-0.9.1/src/satori/server/adapter.py
--rw-r--r--   0        0        0     1043 2023-11-29 15:17:50.878841 satori_python_server-0.9.1/src/satori/server/conection.py
--rw-r--r--   0        0        0      859 2023-11-29 15:17:50.878841 satori_python_server-0.9.1/src/satori/server/model.py
--rw-r--r--   0        0        0     3725 1970-01-01 00:00:00.000000 satori_python_server-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      986 2023-12-06 07:07:21.016116 satori_python_server-0.9.2/.mina/server.toml
+-rw-r--r--   0        0        0     1069 2023-12-06 07:07:21.020116 satori_python_server-0.9.2/LICENSE
+-rw-r--r--   0        0        0     2662 2023-12-06 07:07:21.020116 satori_python_server-0.9.2/README.md
+-rw-r--r--   0        0        0     2049 2023-12-06 07:07:30.508029 satori_python_server-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     8183 2023-12-06 07:07:21.020116 satori_python_server-0.9.2/src/satori/server/__init__.py
+-rw-r--r--   0        0        0      936 2023-12-06 07:07:21.020116 satori_python_server-0.9.2/src/satori/server/adapter.py
+-rw-r--r--   0        0        0     1043 2023-12-06 07:07:21.020116 satori_python_server-0.9.2/src/satori/server/conection.py
+-rw-r--r--   0        0        0      859 2023-12-06 07:07:21.020116 satori_python_server-0.9.2/src/satori/server/model.py
+-rw-r--r--   0        0        0     3725 1970-01-01 00:00:00.000000 satori_python_server-0.9.2/PKG-INFO
```

### Comparing `satori_python_server-0.9.1/.mina/server.toml` & `satori_python_server-0.9.2/.mina/server.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 includes = ["src/satori/server"]
-raw-dependencies = ["satori-python-core >= 0.9.1"]
+raw-dependencies = ["satori-python-core >= 0.9.2"]
 
 [project]
 name = "satori-python-server"
 dynamic = ["version"]
 authors = [
   {name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com"}
 ]
```

### Comparing `satori_python_server-0.9.1/LICENSE` & `satori_python_server-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `satori_python_server-0.9.1/README.md` & `satori_python_server-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `satori_python_server-0.9.1/pyproject.toml` & `satori_python_server-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "launart>=0.8.2",
     "graia-amnesia>=0.8.2",
     "starlette>=0.32.0.post1",
     "uvicorn[standard]>=0.24.0.post1",
-    "satori-python-core >= 0.9.1",
+    "satori-python-core >= 0.9.2",
 ]
 description = "Satori Protocol SDK for python, specify server part"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Typing :: Typed",
     "Development Status :: 4 - Beta",
@@ -21,15 +21,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
 ]
-version = "0.9.1"
+version = "0.9.2"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/RF-Tar-Railt/satori-python"
 repository = "https://github.com/RF-Tar-Railt/satori-python"
```

### Comparing `satori_python_server-0.9.1/src/satori/server/__init__.py` & `satori_python_server-0.9.2/src/satori/server/__init__.py`

 * *Files identical despite different names*

### Comparing `satori_python_server-0.9.1/src/satori/server/adapter.py` & `satori_python_server-0.9.2/src/satori/server/adapter.py`

 * *Files identical despite different names*

### Comparing `satori_python_server-0.9.1/src/satori/server/conection.py` & `satori_python_server-0.9.2/src/satori/server/conection.py`

 * *Files identical despite different names*

### Comparing `satori_python_server-0.9.1/src/satori/server/model.py` & `satori_python_server-0.9.2/src/satori/server/model.py`

 * *Files identical despite different names*

### Comparing `satori_python_server-0.9.1/PKG-INFO` & `satori_python_server-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satori-python-server
-Version: 0.9.1
+Version: 0.9.2
 Summary: Satori Protocol SDK for python, specify server part
 Home-page: https://github.com/RF-Tar-Railt/satori-python
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -17,15 +17,15 @@
 Project-URL: Homepage, https://github.com/RF-Tar-Railt/satori-python
 Project-URL: Repository, https://github.com/RF-Tar-Railt/satori-python
 Requires-Python: >=3.8
 Requires-Dist: launart>=0.8.2
 Requires-Dist: graia-amnesia>=0.8.2
 Requires-Dist: starlette>=0.32.0.post1
 Requires-Dist: uvicorn[standard]>=0.24.0.post1
-Requires-Dist: satori-python-core>=0.9.1
+Requires-Dist: satori-python-core>=0.9.2
 Description-Content-Type: text/markdown
 
 # satori-python
 
 ![latest release](https://img.shields.io/github/release/RF-Tar-Railt/satori-python)
 [![Licence](https://img.shields.io/github/license/RF-Tar-Railt/satori-python)](https://github.com/RF-Tar-Railt/satori-python/blob/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/satori-python)](https://pypi.org/project/satori-python)
```

