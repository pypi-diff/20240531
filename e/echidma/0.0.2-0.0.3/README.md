# Comparing `tmp/echidma-0.0.2.tar.gz` & `tmp/echidma-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echidma-0.0.2.tar", last modified: Thu May 30 22:31:50 2024, max compression
+gzip compressed data, was "echidma-0.0.3.tar", last modified: Fri May 31 06:01:02 2024, max compression
```

## Comparing `echidma-0.0.2.tar` & `echidma-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        0 2024-05-30 22:31:50.863682 echidma-0.0.2/
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)     1071 2024-05-28 22:21:10.000000 echidma-0.0.2/LICENSE
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      576 2024-05-30 22:31:50.863384 echidma-0.0.2/PKG-INFO
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      197 2024-05-30 05:14:43.000000 echidma-0.0.2/README.md
-drwxr-xr-x   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        0 2024-05-30 22:31:50.860170 echidma-0.0.2/echidma/
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)       75 2024-05-30 05:03:37.000000 echidma-0.0.2/echidma/__init__.py
-drwxr-xr-x   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        0 2024-05-30 22:31:50.861722 echidma-0.0.2/echidma/caching/
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)       35 2024-05-28 22:55:50.000000 echidma-0.0.2/echidma/caching/__init__.py
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      461 2024-05-29 04:37:47.000000 echidma-0.0.2/echidma/caching/chunk_cache.py
-drwxr-xr-x   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        0 2024-05-30 22:31:50.862322 echidma-0.0.2/echidma/config_management/
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)       41 2024-05-28 22:54:08.000000 echidma-0.0.2/echidma/config_management/__init__.py
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)     1787 2024-05-30 01:08:08.000000 echidma-0.0.2/echidma/config_management/config_manager.py
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)     2313 2024-05-30 05:36:56.000000 echidma-0.0.2/echidma/indexer_base.py
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      529 2024-05-30 05:23:56.000000 echidma-0.0.2/echidma/indexer_h5.py
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)     1173 2024-05-30 06:55:35.000000 echidma-0.0.2/echidma/indexer_memmap.py
-drwxr-xr-x   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        0 2024-05-30 22:31:50.862993 echidma-0.0.2/echidma.egg-info/
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      576 2024-05-30 22:31:50.000000 echidma-0.0.2/echidma.egg-info/PKG-INFO
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      428 2024-05-30 22:31:50.000000 echidma-0.0.2/echidma.egg-info/SOURCES.txt
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        1 2024-05-30 22:31:50.000000 echidma-0.0.2/echidma.egg-info/dependency_links.txt
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)       86 2024-05-30 22:31:50.000000 echidma-0.0.2/echidma.egg-info/requires.txt
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        8 2024-05-30 22:31:50.000000 echidma-0.0.2/echidma.egg-info/top_level.txt
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)       86 2024-05-30 22:22:28.000000 echidma-0.0.2/pyproject.toml
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)       38 2024-05-30 22:31:50.863739 echidma-0.0.2/setup.cfg
--rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      835 2024-05-30 22:28:26.000000 echidma-0.0.2/setup.py
+drwxr-xr-x   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        0 2024-05-31 06:01:02.467719 echidma-0.0.3/
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)     1071 2024-05-28 22:21:10.000000 echidma-0.0.3/LICENSE
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      576 2024-05-31 06:01:02.467423 echidma-0.0.3/PKG-INFO
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      197 2024-05-30 05:14:43.000000 echidma-0.0.3/README.md
+drwxr-xr-x   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        0 2024-05-31 06:01:02.464209 echidma-0.0.3/echidma/
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      121 2024-05-30 23:29:41.000000 echidma-0.0.3/echidma/__init__.py
+drwxr-xr-x   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        0 2024-05-31 06:01:02.465584 echidma-0.0.3/echidma/caching/
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)       35 2024-05-28 22:55:50.000000 echidma-0.0.3/echidma/caching/__init__.py
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      461 2024-05-29 04:37:47.000000 echidma-0.0.3/echidma/caching/chunk_cache.py
+drwxr-xr-x   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        0 2024-05-31 06:01:02.466268 echidma-0.0.3/echidma/config_management/
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)       41 2024-05-28 22:54:08.000000 echidma-0.0.3/echidma/config_management/__init__.py
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)     4341 2024-05-31 02:53:16.000000 echidma-0.0.3/echidma/config_management/config_manager.py
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)     2314 2024-05-30 23:44:05.000000 echidma-0.0.3/echidma/indexer_base.py
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      735 2024-05-30 23:03:19.000000 echidma-0.0.3/echidma/indexer_h5.py
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)     1663 2024-05-31 02:56:56.000000 echidma-0.0.3/echidma/indexer_memmap.py
+drwxr-xr-x   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        0 2024-05-31 06:01:02.467068 echidma-0.0.3/echidma.egg-info/
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      576 2024-05-31 06:01:02.000000 echidma-0.0.3/echidma.egg-info/PKG-INFO
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      428 2024-05-31 06:01:02.000000 echidma-0.0.3/echidma.egg-info/SOURCES.txt
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        1 2024-05-31 06:01:02.000000 echidma-0.0.3/echidma.egg-info/dependency_links.txt
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)       86 2024-05-31 06:01:02.000000 echidma-0.0.3/echidma.egg-info/requires.txt
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)        8 2024-05-31 06:01:02.000000 echidma-0.0.3/echidma.egg-info/top_level.txt
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)       86 2024-05-30 22:22:28.000000 echidma-0.0.3/pyproject.toml
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)       38 2024-05-31 06:01:02.467781 echidma-0.0.3/setup.cfg
+-rw-r--r--   0 lpin0002 (1846448621) MONASH\Domain Users (907548567)      938 2024-05-31 05:14:47.000000 echidma-0.0.3/setup.py
```

### Comparing `echidma-0.0.2/LICENSE` & `echidma-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `echidma-0.0.2/PKG-INFO` & `echidma-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echidma
-Version: 0.0.2
+Version: 0.0.3
 Summary: Embarrassingly Chunky Hard Indexed Data Memory Access
 Home-page: https://github.com/lpin0002/ECHIDMA
 Author: Liam Pinchbeck
 Author-email: Liam.Pinchbeck@monash.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
```

### Comparing `echidma-0.0.2/echidma/indexer_base.py` & `echidma-0.0.3/echidma/indexer_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import h5py as hp
 from echidma.config_management import ConfigManager
 from echidma.caching import ChunkCache
 
 
 class EchidmaBase:
     def __init__(self, config=None, config_file=None, cache_size=5):
+
         self.config_manager = ConfigManager(config, config_file)
 
         self.cache = ChunkCache(cache_size)
 
 
     
     def get_chunk_by_slice(self, filename, data_slice):
```

### Comparing `echidma-0.0.2/echidma/indexer_h5.py` & `echidma-0.0.3/echidma/indexer_h5.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import h5py as hp
 from echidma.indexer_base import EchidmaBase
+from echidma.config_management import ConfigManager
 
 
 class EchidmaH5(EchidmaBase):
     def __init__(self, config=None, config_file=None, cache_size=5):
         super().__init__(config=config, config_file=config_file, cache_size=cache_size)
             
 
@@ -16,7 +17,10 @@
             chunk = dset[data_slice]
 
         return chunk
 
 
 
 
+    def create_filename(file_id=None, filestem=None, ext='h5'):
+
+        return ConfigManager.create_filename(file_id=file_id, filestem=filestem, ext=ext)
```

### Comparing `echidma-0.0.2/echidma.egg-info/PKG-INFO` & `echidma-0.0.3/echidma.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echidma
-Version: 0.0.2
+Version: 0.0.3
 Summary: Embarrassingly Chunky Hard Indexed Data Memory Access
 Home-page: https://github.com/lpin0002/ECHIDMA
 Author: Liam Pinchbeck
 Author-email: Liam.Pinchbeck@monash.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
```

### Comparing `echidma-0.0.2/setup.py` & `echidma-0.0.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,26 +6,25 @@
 
 setup(name='echidma',
       description='Embarrassingly Chunky Hard Indexed Data Memory Access',
       url='https://github.com/lpin0002/ECHIDMA',
       author='Liam Pinchbeck',
       author_email='Liam.Pinchbeck@monash.edu',
       license="MIT",
-      version='0.0.2',
+      version='0.0.3',
       packages=find_packages(),
 
       # For a lot of the DM spectral classes we require that dict types are ordered
       python_requires='>=3.6',
-      install_requires=[
-        "scipy==1.11.3",
-        "tqdm>=4.65.0",
-        "numpy>=1.23",
-        "pandas>=1.5.3",
-        "pytest",
-        "h5py",
-        "hdf5plugin",
-        "numcodecs",],
+      install_requires=["scipy==1.11.3",
+                        "tqdm>=4.65.0",
+                        "numpy>=1.23",
+                        "pandas>=1.5.3",
+                        "pytest",
+                        "h5py",
+                        "hdf5plugin",
+                        "numcodecs",],
 
       classifiers=[
           "License :: OSI Approved :: MIT License",
           "Operating System :: Unix",],
       )
```

