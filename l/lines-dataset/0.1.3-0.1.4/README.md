# Comparing `tmp/lines_dataset-0.1.3.tar.gz` & `tmp/lines_dataset-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lines_dataset-0.1.3.tar", last modified: Fri May 31 09:48:19 2024, max compression
+gzip compressed data, was "lines_dataset-0.1.4.tar", last modified: Fri May 31 09:48:52 2024, max compression
```

## Comparing `lines_dataset-0.1.3.tar` & `lines_dataset-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 09:48:19.925698 lines_dataset-0.1.3/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      429 2024-05-31 09:48:19.925698 lines_dataset-0.1.3/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       91 2024-05-30 21:28:08.000000 lines_dataset-0.1.3/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      574 2024-05-31 09:48:17.000000 lines_dataset-0.1.3/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-31 09:48:19.925698 lines_dataset-0.1.3/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 09:48:19.925698 lines_dataset-0.1.3/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 09:48:19.925698 lines_dataset-0.1.3/src/lines_dataset/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      196 2024-05-30 21:28:45.000000 lines_dataset-0.1.3/src/lines_dataset/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      118 2024-05-30 21:30:44.000000 lines_dataset-0.1.3/src/lines_dataset/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1762 2024-05-31 09:48:15.000000 lines_dataset-0.1.3/src/lines_dataset/dataset.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      154 2024-05-31 08:34:26.000000 lines_dataset-0.1.3/src/lines_dataset/meta.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 09:48:19.925698 lines_dataset-0.1.3/src/lines_dataset.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      429 2024-05-31 09:48:19.000000 lines_dataset-0.1.3/src/lines_dataset.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      344 2024-05-31 09:48:19.000000 lines_dataset-0.1.3/src/lines_dataset.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-31 09:48:19.000000 lines_dataset-0.1.3/src/lines_dataset.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-31 09:48:19.000000 lines_dataset-0.1.3/src/lines_dataset.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       14 2024-05-31 09:48:19.000000 lines_dataset-0.1.3/src/lines_dataset.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 09:48:52.895698 lines_dataset-0.1.4/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      453 2024-05-31 09:48:52.895698 lines_dataset-0.1.4/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       91 2024-05-30 21:28:08.000000 lines_dataset-0.1.4/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      586 2024-05-31 09:48:48.000000 lines_dataset-0.1.4/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-31 09:48:52.895698 lines_dataset-0.1.4/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 09:48:52.895698 lines_dataset-0.1.4/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 09:48:52.895698 lines_dataset-0.1.4/src/lines_dataset/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      196 2024-05-30 21:28:45.000000 lines_dataset-0.1.4/src/lines_dataset/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      118 2024-05-30 21:30:44.000000 lines_dataset-0.1.4/src/lines_dataset/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1762 2024-05-31 09:48:15.000000 lines_dataset-0.1.4/src/lines_dataset/dataset.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      154 2024-05-31 08:34:26.000000 lines_dataset-0.1.4/src/lines_dataset/meta.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 09:48:52.895698 lines_dataset-0.1.4/src/lines_dataset.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      453 2024-05-31 09:48:52.000000 lines_dataset-0.1.4/src/lines_dataset.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      344 2024-05-31 09:48:52.000000 lines_dataset-0.1.4/src/lines_dataset.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-31 09:48:52.000000 lines_dataset-0.1.4/src/lines_dataset.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-05-31 09:48:52.000000 lines_dataset-0.1.4/src/lines_dataset.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       14 2024-05-31 09:48:52.000000 lines_dataset-0.1.4/src/lines_dataset.egg-info/top_level.txt
```

### Comparing `lines_dataset-0.1.3/pyproject.toml` & `lines_dataset-0.1.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lines-dataset"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Simple tools for storing inputs + labels datasets as one sample per line"
 dependencies = [
-  "pydantic"
+  "pydantic", "fs-tools"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 repo = "https://github.com/moveread/REPO.git"
```

### Comparing `lines_dataset-0.1.3/src/lines_dataset/dataset.py` & `lines_dataset-0.1.4/src/lines_dataset/dataset.py`

 * *Files identical despite different names*

