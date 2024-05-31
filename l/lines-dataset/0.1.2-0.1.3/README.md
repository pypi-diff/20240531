# Comparing `tmp/lines_dataset-0.1.2.tar.gz` & `tmp/lines_dataset-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lines_dataset-0.1.2.tar", last modified: Fri May 31 09:46:46 2024, max compression
+gzip compressed data, was "lines_dataset-0.1.3.tar", last modified: Fri May 31 09:48:19 2024, max compression
```

## Comparing `lines_dataset-0.1.2.tar` & `lines_dataset-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 09:46:46.145699 lines_dataset-0.1.2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      429 2024-05-31 09:46:46.145699 lines_dataset-0.1.2/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       91 2024-05-30 21:28:08.000000 lines_dataset-0.1.2/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      574 2024-05-31 09:46:39.000000 lines_dataset-0.1.2/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-31 09:46:46.145699 lines_dataset-0.1.2/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 09:46:46.135699 lines_dataset-0.1.2/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 09:46:46.145699 lines_dataset-0.1.2/src/lines_dataset/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      196 2024-05-30 21:28:45.000000 lines_dataset-0.1.2/src/lines_dataset/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      118 2024-05-30 21:30:44.000000 lines_dataset-0.1.2/src/lines_dataset/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1776 2024-05-31 08:48:12.000000 lines_dataset-0.1.2/src/lines_dataset/dataset.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      154 2024-05-31 08:34:26.000000 lines_dataset-0.1.2/src/lines_dataset/meta.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 09:46:46.145699 lines_dataset-0.1.2/src/lines_dataset.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      429 2024-05-31 09:46:46.000000 lines_dataset-0.1.2/src/lines_dataset.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      344 2024-05-31 09:46:46.000000 lines_dataset-0.1.2/src/lines_dataset.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-31 09:46:46.000000 lines_dataset-0.1.2/src/lines_dataset.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-31 09:46:46.000000 lines_dataset-0.1.2/src/lines_dataset.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       14 2024-05-31 09:46:46.000000 lines_dataset-0.1.2/src/lines_dataset.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 09:48:19.925698 lines_dataset-0.1.3/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      429 2024-05-31 09:48:19.925698 lines_dataset-0.1.3/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       91 2024-05-30 21:28:08.000000 lines_dataset-0.1.3/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      574 2024-05-31 09:48:17.000000 lines_dataset-0.1.3/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-31 09:48:19.925698 lines_dataset-0.1.3/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 09:48:19.925698 lines_dataset-0.1.3/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 09:48:19.925698 lines_dataset-0.1.3/src/lines_dataset/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      196 2024-05-30 21:28:45.000000 lines_dataset-0.1.3/src/lines_dataset/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      118 2024-05-30 21:30:44.000000 lines_dataset-0.1.3/src/lines_dataset/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1762 2024-05-31 09:48:15.000000 lines_dataset-0.1.3/src/lines_dataset/dataset.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      154 2024-05-31 08:34:26.000000 lines_dataset-0.1.3/src/lines_dataset/meta.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 09:48:19.925698 lines_dataset-0.1.3/src/lines_dataset.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      429 2024-05-31 09:48:19.000000 lines_dataset-0.1.3/src/lines_dataset.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      344 2024-05-31 09:48:19.000000 lines_dataset-0.1.3/src/lines_dataset.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-31 09:48:19.000000 lines_dataset-0.1.3/src/lines_dataset.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-31 09:48:19.000000 lines_dataset-0.1.3/src/lines_dataset.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       14 2024-05-31 09:48:19.000000 lines_dataset-0.1.3/src/lines_dataset.egg-info/top_level.txt
```

### Comparing `lines_dataset-0.1.2/pyproject.toml` & `lines_dataset-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lines-dataset"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Simple tools for storing inputs + labels datasets as one sample per line"
 dependencies = [
   "pydantic"
 ]
```

### Comparing `lines_dataset-0.1.2/src/lines_dataset/dataset.py` & `lines_dataset-0.1.3/src/lines_dataset/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 from glob import glob
 import fs
 from .meta import Meta
 
 K = TypeVar('K', bound=LiteralString)
 
-def zip_files(files: Mapping[str, Sequence[str]]) -> Iterable[Mapping[str, str]]:
+def zip_files(files: Mapping[K, Sequence[str]]) -> Iterable[Mapping[K, str]]:
   iters = {
     key: iter(fs.concat_lines(file))
     for key, file in files.items()
   }
   while True:
     try:
       yield {
@@ -49,19 +49,19 @@
       return glob(os.path.join(self.base_path, self.meta.files[key]))
     return []
   
   def iterate(self, key: str) -> Iterable[str]:
     yield from fs.concat_lines(self.files(key))
 
   def samples(self, *keys: K) -> Iterable[Mapping[K, str]]:
-    keys = keys or list(self.meta.files.keys())
+    keys = keys or list(self.meta.files.keys()) # type: ignore
     files = {
       key: self.files(key)
       for key in keys
     }
     yield from zip_files(files)
 
-  def __iter__(self) -> Iterable[Mapping[str, str]]:
-    return self.samples()
+  def __iter__(self):
+    return iter(self.samples())
 
   def __len__(self) -> int:
     return self.meta.samples
```

