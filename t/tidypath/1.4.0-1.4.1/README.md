# Comparing `tmp/tidypath-1.4.0.tar.gz` & `tmp/tidypath-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidypath-1.4.0.tar", last modified: Thu May 30 14:04:46 2024, max compression
+gzip compressed data, was "tidypath-1.4.1.tar", last modified: Fri May 31 11:04:12 2024, max compression
```

## Comparing `tidypath-1.4.0.tar` & `tidypath-1.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-30 14:04:46.870695 tidypath-1.4.0/
--rwxr-xr-x   0 jorgemedina  (1236) users      (100)    35149 2023-09-08 10:22:16.000000 tidypath-1.4.0/LICENSE.md
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3682 2024-05-30 14:04:46.870695 tidypath-1.4.0/PKG-INFO
--rwxr-xr-x   0 jorgemedina  (1236) users      (100)     2804 2023-09-08 10:22:16.000000 tidypath-1.4.0/README.md
--rwxr-xr-x   0 jorgemedina  (1236) users      (100)      106 2024-05-30 14:04:46.874695 tidypath-1.4.0/setup.cfg
--rwxr-xr-x   0 jorgemedina  (1236) users      (100)     1161 2024-05-30 14:04:17.000000 tidypath-1.4.0/setup.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-30 14:04:46.858695 tidypath-1.4.0/tidypath/
--rwxr-xr-x   0 jorgemedina  (1236) users      (100)      371 2023-09-08 10:22:16.000000 tidypath-1.4.0/tidypath/__init__.py
--rwxr-xr-x   0 jorgemedina  (1236) users      (100)     1629 2023-09-08 10:22:16.000000 tidypath-1.4.0/tidypath/_helper.py
--rwxr-xr-x   0 jorgemedina  (1236) users      (100)     4998 2024-04-05 11:52:19.000000 tidypath-1.4.0/tidypath/config.py
--rwxr-xr-x   0 jorgemedina  (1236) users      (100)    14770 2024-05-30 13:41:07.000000 tidypath-1.4.0/tidypath/decorators.py
--rwxr-xr-x   0 jorgemedina  (1236) users      (100)     6165 2023-09-08 10:22:17.000000 tidypath-1.4.0/tidypath/fmt.py
--rwxr-xr-x   0 jorgemedina  (1236) users      (100)     5197 2023-09-08 10:22:17.000000 tidypath-1.4.0/tidypath/inspection.py
--rwxr-xr-x   0 jorgemedina  (1236) users      (100)    14563 2024-05-30 14:03:40.000000 tidypath-1.4.0/tidypath/paths.py
--rwxr-xr-x   0 jorgemedina  (1236) users      (100)     9844 2023-09-08 10:22:17.000000 tidypath-1.4.0/tidypath/storage.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-30 14:04:46.870695 tidypath-1.4.0/tidypath.egg-info/
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3682 2024-05-30 14:04:46.000000 tidypath-1.4.0/tidypath.egg-info/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)      358 2024-05-30 14:04:46.000000 tidypath-1.4.0/tidypath.egg-info/SOURCES.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2024-05-30 14:04:46.000000 tidypath-1.4.0/tidypath.egg-info/dependency_links.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)       63 2024-05-30 14:04:46.000000 tidypath-1.4.0/tidypath.egg-info/requires.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        9 2024-05-30 14:04:46.000000 tidypath-1.4.0/tidypath.egg-info/top_level.txt
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-31 11:04:12.823873 tidypath-1.4.1/
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)    35149 2023-09-08 10:22:16.000000 tidypath-1.4.1/LICENSE.md
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3682 2024-05-31 11:04:12.823873 tidypath-1.4.1/PKG-INFO
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)     2804 2023-09-08 10:22:16.000000 tidypath-1.4.1/README.md
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)      106 2024-05-31 11:04:12.827873 tidypath-1.4.1/setup.cfg
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)     1161 2024-05-31 11:04:02.000000 tidypath-1.4.1/setup.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-31 11:04:12.811873 tidypath-1.4.1/tidypath/
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)      371 2023-09-08 10:22:16.000000 tidypath-1.4.1/tidypath/__init__.py
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)     1629 2023-09-08 10:22:16.000000 tidypath-1.4.1/tidypath/_helper.py
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)     4998 2024-04-05 11:52:19.000000 tidypath-1.4.1/tidypath/config.py
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)    14770 2024-05-30 13:41:07.000000 tidypath-1.4.1/tidypath/decorators.py
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)     6165 2023-09-08 10:22:17.000000 tidypath-1.4.1/tidypath/fmt.py
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)     5197 2023-09-08 10:22:17.000000 tidypath-1.4.1/tidypath/inspection.py
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)    14563 2024-05-30 14:03:40.000000 tidypath-1.4.1/tidypath/paths.py
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)     9664 2024-05-31 11:03:48.000000 tidypath-1.4.1/tidypath/storage.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-31 11:04:12.823873 tidypath-1.4.1/tidypath.egg-info/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3682 2024-05-31 11:04:12.000000 tidypath-1.4.1/tidypath.egg-info/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      358 2024-05-31 11:04:12.000000 tidypath-1.4.1/tidypath.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2024-05-31 11:04:12.000000 tidypath-1.4.1/tidypath.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       63 2024-05-31 11:04:12.000000 tidypath-1.4.1/tidypath.egg-info/requires.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        9 2024-05-31 11:04:12.000000 tidypath-1.4.1/tidypath.egg-info/top_level.txt
```

### Comparing `tidypath-1.4.0/LICENSE.md` & `tidypath-1.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tidypath-1.4.0/PKG-INFO` & `tidypath-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypath
-Version: 1.4.0
+Version: 1.4.1
 Summary: Automatically store/load data in a tidy, efficient way.
 Home-page: https://github.com/medinajorge/tidypath
 Download-URL: https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tidypath-1.4.0/README.md` & `tidypath-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `tidypath-1.4.0/setup.py` & `tidypath-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tidypath',
-    version='1.4.0',
+    version='1.4.1',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=['tidypath'],
     url='https://github.com/medinajorge/tidypath',
     download_url='https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz',
     description="Automatically store/load data in a tidy, efficient way.",
     long_description=open('README.md').read(),
```

### Comparing `tidypath-1.4.0/tidypath/_helper.py` & `tidypath-1.4.1/tidypath/_helper.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.4.0/tidypath/config.py` & `tidypath-1.4.1/tidypath/config.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.4.0/tidypath/decorators.py` & `tidypath-1.4.1/tidypath/decorators.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.4.0/tidypath/fmt.py` & `tidypath-1.4.1/tidypath/fmt.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.4.0/tidypath/inspection.py` & `tidypath-1.4.1/tidypath/inspection.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.4.0/tidypath/paths.py` & `tidypath-1.4.1/tidypath/paths.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.4.0/tidypath/storage.py` & `tidypath-1.4.1/tidypath/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     _parent_dir, _filename = os.path.split(filename)
     if _parent_dir:  # directory specified in filename
         parent_dir = _parent_dir
         filename = _filename
     Path(parent_dir).mkdir(parents=True, exist_ok=True)
     filename = filename if filename.endswith('.{}'.format(saving_type)) else '{}.{}'.format(filename, saving_type)
     return parent_dir, filename
-        
+
 def create_saving_func(file_opener, file_writer, saving_type, **kwargs):
     def saving_func(data, filename, parent_dir=parent_dir):
         """Can specify directory in filename or in parent_dir."""
         parent_dir, filename = save_preprocess(filename, saving_type, parent_dir)
         with file_opener(os.path.join(parent_dir, filename), 'w') as f:
             file_writer(data, f, **kwargs)
         return
@@ -54,15 +54,15 @@
 save_bz2 = create_saving_func(bz2.BZ2File, pickle.dump, 'pbz2')
 save_lzma = create_saving_func(lzma.LZMAFile, pickle.dump, 'lzma')
 
 def save_npz(arr, filename, parent_dir=parent_dir, key="arr"):
     np.savez_compressed(os.path.join(parent_dir, filename), **{key:arr})
     return
 
-def save_csv(data, filename, parent_dir=parent_dir, **df_kwargs):
+def save_csv(data, filename, parent_dir=parent_dir, **kwargs):
     """
     If data is a numpy array => if 2D => data
                                    1D => [data]
     (required by np.savetxt)
     """
     parent_dir, filename = save_preprocess(filename, "csv", parent_dir)
     if isinstance(data, (pd.core.frame.DataFrame, pd.core.series.Series)):
@@ -81,31 +81,31 @@
     - extra_processing = List of process that could be applied to the file.
     - apply_defaults = dict:{str: bool}. The key is set as a function variable, the value indicates whether to apply the process named by the key.
     """
     if extra_processing is None:
         def loading_func(path):
             with file_opener(path, 'rb') as f:
                 return file_loader(f)
-    else:        
+    else:
         def loading_func(path):
             args = {key:val for key,val in locals().items() if key not in  ('path', *create_loading_func.__code__.co_varnames)}
             with file_opener(path, 'rb') as f:
                 data = file_loader(f)
-            
+
             for condition, process in zip(args.values(), extra_processing):
                 if condition:
                     data = process(data)
             return data
-        
+
         # I know this sould not be done this way, but I wanted to check it can
         code_data = loading_func.__code__
         num_vars = code_data.co_argcount
         num_vars_new = len(apply_defaults)
         new_code = code_data.replace(co_varnames=(*code_data.co_varnames[:num_vars], *apply_defaults.keys(), *code_data.co_varnames[num_vars:]),
-                                     co_argcount=num_vars + num_vars_new, 
+                                     co_argcount=num_vars + num_vars_new,
                                      co_nlocals=code_data.co_nlocals + num_vars_new)
         loading_func.__code__ = new_code
         loading_func.__defaults__ = tuple(apply_defaults.values())
     return loading_func
 
 def int_keys(dictionary):
      return {int(key):val for key,val in dictionary.items()}
@@ -122,106 +122,105 @@
 def load_csv(path, mode="pandas", **kwargs):
     if mode == "pandas":
         return pd.read_csv(path, **kwargs)
     elif mode == "numpy":
         return np.loadtxt(path, delimiter=",", **kwargs)
     else:
         raise ValueError(f"mode {mode} not valid. Available: 'panda', 'numpy'.")
-        
+
 
 ##############################################################################################################################
 """                                                   III. Compression                                                     """
 ##############################################################################################################################
 
 def compress_files(rootDir=parent_dir, extension='.json', compress_to='lzma', min_size=0, loading_key=None):
     """
     Searches in a directory and all its subdirectories files with a certain extension and compresses them.
-    
+
     Attributes:
     - rootDir: The root directory.
     - extension: Extension setting which files should be compressed. Available options: '.json', '.npz'.
     - compress_to: File type after compression. Available options: 'lzma', 'bz2' (or pbz2).
     - min_size: Minimum size for applying compression (in MB).
     - loading_key: Key for retrieving the data in a npz file. If None, retrieves the data corresponding to the first key.
-    
+
     Returns: Dict containing the name of the files that could not be processed ('bad compression') or those that were corrupted and had to be deleted('deleted files').
     """
     try:
         shell = get_ipython().__class__.__name__
         if shell == 'ZMQInteractiveShell': # script being run in Jupyter notebook
             from tqdm.notebook import tqdm
         elif shell == 'TerminalInteractiveShell': #script being run in iPython terminal
             from tqdm import tqdm
     except NameError:
             from tqdm import tqdm # Probably runing on standard python terminal.
-            
+
     # Get all the paths with the desired extension and minimum size.
     files = []
 
     for dirpath, subdirList, fileList in os.walk(rootDir):
         files += [os.path.join(dirpath, file) for file in fileList if os.path.splitext(file)[1] == extension]
-    
+
     if min_size > 0:
         files = [file for file in files if os.path.getsize(file) > min_size*1e6]
-    
+
     # Load files, compress, save and delete if compressed_file == pre_compressed_file
     if extension == '.json':
         loader = load_json
     elif extension == '.npz':
         loader = load_npz
     else:
         raise ValueError("extension = '{}' not valid. Available options: '.json', '.npz'".format(extension))
-        
+
     if compress_to == 'lzma':
         compressor = save_lzma
         load_compressor = load_lzma
     elif compress_to == 'bz2':
         compressor = save_bz2
         load_compressor = load_bz2
     else:
         raise ValueError("compress_to = '{}' not valid. Available options: 'lzma', 'bz2'".format(extension))
-    
+
     not_correctly_processed = {'bad_compression': []}
     pbar = tqdm(range(len(files)))
-    
+
     if extension == '.json':
         for file in files:
             try:
                 pre_compressed = loader(file, int_keys=True)
             except ValueError:
                 pre_compressed = loader(file, int_keys=False)
-            
+
             new_filename = '{}.{}'.format(os.path.splitext(file)[0], compress_to)
             compressor(pre_compressed, new_filename, parent_dir="")
             compressed_file = load_compressor(new_filename)
-            
+
             if compressed_file == pre_compressed:
                 os.remove(file)
             else:
                 not_correctly_processed['bad_compression'].append(file)
-            
+
             pbar.refresh()
             print(pbar.update())
-            
+
     if extension == '.npz':
         not_correctly_processed['deleted_files'] = []
         for file in files:
             try:
                 pre_compressed = loader(file, key=loading_key)
             except zipfile.BadZipFile: # corrupted file
                 os.remove(file)
                 not_correctly_processed['deleted_files'].append(file)
                 continue
-                
+
             new_filename = '{}.{}'.format(os.path.splitext(file)[0], compress_to)
             compressor(pre_compressed, new_filename, parent_dir="")
             compressed_file = load_compressor(new_filename)
-            
+
             if np.all(compressed_file == pre_compressed):
                 os.remove(file)
             else:
                 not_correctly_processed['bad_compression'].append(file)
             pbar.refresh()
             print(pbar.update())
-    
+
     return not_correctly_processed
-
```

### Comparing `tidypath-1.4.0/tidypath.egg-info/PKG-INFO` & `tidypath-1.4.1/tidypath.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypath
-Version: 1.4.0
+Version: 1.4.1
 Summary: Automatically store/load data in a tidy, efficient way.
 Home-page: https://github.com/medinajorge/tidypath
 Download-URL: https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

