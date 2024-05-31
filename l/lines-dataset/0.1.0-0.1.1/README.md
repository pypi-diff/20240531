# Comparing `tmp/lines_dataset-0.1.0.tar.gz` & `tmp/lines_dataset-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lines_dataset-0.1.0.tar", last modified: Thu May 30 21:31:13 2024, max compression
+gzip compressed data, was "lines_dataset-0.1.1.tar", last modified: Thu May 30 21:32:39 2024, max compression
```

## Comparing `lines_dataset-0.1.0.tar` & `lines_dataset-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 21:31:13.626657 lines_dataset-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      429 2024-05-30 21:31:13.616657 lines_dataset-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       91 2024-05-30 21:28:08.000000 lines_dataset-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      574 2024-05-30 21:29:11.000000 lines_dataset-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-30 21:31:13.626657 lines_dataset-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 21:31:13.616657 lines_dataset-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 21:31:13.616657 lines_dataset-0.1.0/src/lines_dataset/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      196 2024-05-30 21:28:45.000000 lines_dataset-0.1.0/src/lines_dataset/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      118 2024-05-30 21:30:44.000000 lines_dataset-0.1.0/src/lines_dataset/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      960 2024-05-30 21:30:17.000000 lines_dataset-0.1.0/src/lines_dataset/dataset.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      191 2024-05-30 21:29:24.000000 lines_dataset-0.1.0/src/lines_dataset/meta.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 21:31:13.616657 lines_dataset-0.1.0/src/lines_dataset.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      429 2024-05-30 21:31:13.000000 lines_dataset-0.1.0/src/lines_dataset.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      344 2024-05-30 21:31:13.000000 lines_dataset-0.1.0/src/lines_dataset.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-30 21:31:13.000000 lines_dataset-0.1.0/src/lines_dataset.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-30 21:31:13.000000 lines_dataset-0.1.0/src/lines_dataset.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       14 2024-05-30 21:31:13.000000 lines_dataset-0.1.0/src/lines_dataset.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 21:32:39.896659 lines_dataset-0.1.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      429 2024-05-30 21:32:39.896659 lines_dataset-0.1.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       91 2024-05-30 21:28:08.000000 lines_dataset-0.1.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      574 2024-05-30 21:32:37.000000 lines_dataset-0.1.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-30 21:32:39.896659 lines_dataset-0.1.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 21:32:39.886659 lines_dataset-0.1.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 21:32:39.896659 lines_dataset-0.1.1/src/lines_dataset/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      196 2024-05-30 21:28:45.000000 lines_dataset-0.1.1/src/lines_dataset/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      118 2024-05-30 21:30:44.000000 lines_dataset-0.1.1/src/lines_dataset/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1267 2024-05-30 21:32:28.000000 lines_dataset-0.1.1/src/lines_dataset/dataset.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      191 2024-05-30 21:29:24.000000 lines_dataset-0.1.1/src/lines_dataset/meta.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 21:32:39.896659 lines_dataset-0.1.1/src/lines_dataset.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      429 2024-05-30 21:32:39.000000 lines_dataset-0.1.1/src/lines_dataset.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      344 2024-05-30 21:32:39.000000 lines_dataset-0.1.1/src/lines_dataset.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-30 21:32:39.000000 lines_dataset-0.1.1/src/lines_dataset.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-30 21:32:39.000000 lines_dataset-0.1.1/src/lines_dataset.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       14 2024-05-30 21:32:39.000000 lines_dataset-0.1.1/src/lines_dataset.egg-info/top_level.txt
```

### Comparing `lines_dataset-0.1.0/pyproject.toml` & `lines_dataset-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lines-dataset"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Simple tools for storing inputs + labels datasets as one sample per line"
 dependencies = [
   "pydantic"
 ]
```

### Comparing `lines_dataset-0.1.0/src/lines_dataset/dataset.py` & `lines_dataset-0.1.1/src/lines_dataset/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,22 @@
 
   @classmethod
   def read(cls, base: str) -> 'Dataset':
     with open(os.path.join(base, 'meta.json')) as f:
       meta = Meta.model_validate_json(f.read())
     return Dataset(base, meta)
   
+  @classmethod
+  def create(cls, base: str, meta: Meta, *, overwrite: bool = False) -> 'Dataset':
+    os.makedirs(base, exist_ok=True)
+    mode = 'x' if not overwrite else 'w'
+    with open(os.path.join(base, 'meta.json'), mode) as f:
+      f.write(meta.model_dump_json())
+    return Dataset(base, meta)
+  
   def input_files(self) -> Sequence[str]:
     return glob(os.path.join(self.base_path, self.meta.files.inputs))
   
   def label_files(self) -> Sequence[str]:
     return glob(os.path.join(self.base_path, self.meta.files.labels))
 
   def samples(self) -> Iterable[tuple[str, str]]:
```

