# Comparing `tmp/parallel-pandas-0.6.1.tar.gz` & `tmp/parallel-pandas-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallel-pandas-0.6.1.tar", last modified: Sun Dec  3 13:05:28 2023, max compression
+gzip compressed data, was "parallel-pandas-0.6.2.tar", last modified: Sun Dec  3 13:10:40 2023, max compression
```

## Comparing `parallel-pandas-0.6.1.tar` & `parallel-pandas-0.6.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 admin     (1000) admin     (1000)        0 2023-12-03 13:05:28.881657 parallel-pandas-0.6.1/
--rw-rw-r--   0 admin     (1000) admin     (1000)     1070 2023-11-01 07:22:35.000000 parallel-pandas-0.6.1/LICENSE
--rw-r--r--   0 admin     (1000) admin     (1000)    17408 2023-12-03 13:05:28.881657 parallel-pandas-0.6.1/PKG-INFO
--rw-rw-r--   0 admin     (1000) admin     (1000)    16798 2023-12-03 12:36:17.000000 parallel-pandas-0.6.1/README.md
-drwxrwxr-x   0 admin     (1000) admin     (1000)        0 2023-12-03 13:05:28.877657 parallel-pandas-0.6.1/parallel_pandas/
--rw-rw-r--   0 admin     (1000) admin     (1000)       62 2023-11-01 07:22:35.000000 parallel-pandas-0.6.1/parallel_pandas/__init__.py
-drwxrwxr-x   0 admin     (1000) admin     (1000)        0 2023-12-03 13:05:28.881657 parallel-pandas-0.6.1/parallel_pandas/core/
--rw-rw-r--   0 admin     (1000) admin     (1000)     1589 2023-11-01 08:05:12.000000 parallel-pandas-0.6.1/parallel_pandas/core/__init__.py
--rw-rw-r--   0 admin     (1000) admin     (1000)     5686 2023-12-03 13:03:18.000000 parallel-pandas-0.6.1/parallel_pandas/core/_numba.py
--rw-rw-r--   0 admin     (1000) admin     (1000)    36645 2023-12-03 12:53:28.000000 parallel-pandas-0.6.1/parallel_pandas/core/parallel_dataframe.py
--rw-rw-r--   0 admin     (1000) admin     (1000)     2354 2023-11-01 07:22:35.000000 parallel-pandas-0.6.1/parallel_pandas/core/parallel_groupby.py
--rw-rw-r--   0 admin     (1000) admin     (1000)     2739 2023-12-03 12:26:15.000000 parallel-pandas-0.6.1/parallel_pandas/core/parallel_series.py
--rw-rw-r--   0 admin     (1000) admin     (1000)    13582 2023-11-15 14:00:45.000000 parallel-pandas-0.6.1/parallel_pandas/core/parallel_window.py
--rw-rw-r--   0 admin     (1000) admin     (1000)     4232 2023-12-01 16:35:51.000000 parallel-pandas-0.6.1/parallel_pandas/core/progress_imap.py
--rw-rw-r--   0 admin     (1000) admin     (1000)     2534 2023-12-03 09:36:09.000000 parallel-pandas-0.6.1/parallel_pandas/core/tools.py
--rw-rw-r--   0 admin     (1000) admin     (1000)    12196 2023-11-01 08:04:40.000000 parallel-pandas-0.6.1/parallel_pandas/main.py
-drwxrwxr-x   0 admin     (1000) admin     (1000)        0 2023-12-03 13:05:28.881657 parallel-pandas-0.6.1/parallel_pandas.egg-info/
--rw-r--r--   0 admin     (1000) admin     (1000)    17408 2023-12-03 13:05:28.000000 parallel-pandas-0.6.1/parallel_pandas.egg-info/PKG-INFO
--rw-rw-r--   0 admin     (1000) admin     (1000)      578 2023-12-03 13:05:28.000000 parallel-pandas-0.6.1/parallel_pandas.egg-info/SOURCES.txt
--rw-rw-r--   0 admin     (1000) admin     (1000)        1 2023-12-03 13:05:28.000000 parallel-pandas-0.6.1/parallel_pandas.egg-info/dependency_links.txt
--rw-rw-r--   0 admin     (1000) admin     (1000)       52 2023-12-03 13:05:28.000000 parallel-pandas-0.6.1/parallel_pandas.egg-info/requires.txt
--rw-rw-r--   0 admin     (1000) admin     (1000)       16 2023-12-03 13:05:28.000000 parallel-pandas-0.6.1/parallel_pandas.egg-info/top_level.txt
--rw-rw-r--   0 admin     (1000) admin     (1000)       79 2023-12-03 13:05:28.881657 parallel-pandas-0.6.1/setup.cfg
--rw-rw-r--   0 admin     (1000) admin     (1000)      929 2023-12-03 13:05:18.000000 parallel-pandas-0.6.1/setup.py
+drwxrwxr-x   0 admin     (1000) admin     (1000)        0 2023-12-03 13:10:40.457297 parallel-pandas-0.6.2/
+-rw-rw-r--   0 admin     (1000) admin     (1000)     1070 2023-11-01 07:22:35.000000 parallel-pandas-0.6.2/LICENSE
+-rw-r--r--   0 admin     (1000) admin     (1000)    17408 2023-12-03 13:10:40.457297 parallel-pandas-0.6.2/PKG-INFO
+-rw-rw-r--   0 admin     (1000) admin     (1000)    16798 2023-12-03 12:36:17.000000 parallel-pandas-0.6.2/README.md
+drwxrwxr-x   0 admin     (1000) admin     (1000)        0 2023-12-03 13:10:40.453297 parallel-pandas-0.6.2/parallel_pandas/
+-rw-rw-r--   0 admin     (1000) admin     (1000)       62 2023-11-01 07:22:35.000000 parallel-pandas-0.6.2/parallel_pandas/__init__.py
+drwxrwxr-x   0 admin     (1000) admin     (1000)        0 2023-12-03 13:10:40.453297 parallel-pandas-0.6.2/parallel_pandas/core/
+-rw-rw-r--   0 admin     (1000) admin     (1000)     1589 2023-11-01 08:05:12.000000 parallel-pandas-0.6.2/parallel_pandas/core/__init__.py
+-rw-rw-r--   0 admin     (1000) admin     (1000)     5688 2023-12-03 13:10:27.000000 parallel-pandas-0.6.2/parallel_pandas/core/_numba.py
+-rw-rw-r--   0 admin     (1000) admin     (1000)    36645 2023-12-03 12:53:28.000000 parallel-pandas-0.6.2/parallel_pandas/core/parallel_dataframe.py
+-rw-rw-r--   0 admin     (1000) admin     (1000)     2354 2023-11-01 07:22:35.000000 parallel-pandas-0.6.2/parallel_pandas/core/parallel_groupby.py
+-rw-rw-r--   0 admin     (1000) admin     (1000)     2739 2023-12-03 12:26:15.000000 parallel-pandas-0.6.2/parallel_pandas/core/parallel_series.py
+-rw-rw-r--   0 admin     (1000) admin     (1000)    13582 2023-11-15 14:00:45.000000 parallel-pandas-0.6.2/parallel_pandas/core/parallel_window.py
+-rw-rw-r--   0 admin     (1000) admin     (1000)     4232 2023-12-01 16:35:51.000000 parallel-pandas-0.6.2/parallel_pandas/core/progress_imap.py
+-rw-rw-r--   0 admin     (1000) admin     (1000)     2534 2023-12-03 09:36:09.000000 parallel-pandas-0.6.2/parallel_pandas/core/tools.py
+-rw-rw-r--   0 admin     (1000) admin     (1000)    12196 2023-11-01 08:04:40.000000 parallel-pandas-0.6.2/parallel_pandas/main.py
+drwxrwxr-x   0 admin     (1000) admin     (1000)        0 2023-12-03 13:10:40.453297 parallel-pandas-0.6.2/parallel_pandas.egg-info/
+-rw-r--r--   0 admin     (1000) admin     (1000)    17408 2023-12-03 13:10:40.000000 parallel-pandas-0.6.2/parallel_pandas.egg-info/PKG-INFO
+-rw-rw-r--   0 admin     (1000) admin     (1000)      578 2023-12-03 13:10:40.000000 parallel-pandas-0.6.2/parallel_pandas.egg-info/SOURCES.txt
+-rw-rw-r--   0 admin     (1000) admin     (1000)        1 2023-12-03 13:10:40.000000 parallel-pandas-0.6.2/parallel_pandas.egg-info/dependency_links.txt
+-rw-rw-r--   0 admin     (1000) admin     (1000)       52 2023-12-03 13:10:40.000000 parallel-pandas-0.6.2/parallel_pandas.egg-info/requires.txt
+-rw-rw-r--   0 admin     (1000) admin     (1000)       16 2023-12-03 13:10:40.000000 parallel-pandas-0.6.2/parallel_pandas.egg-info/top_level.txt
+-rw-rw-r--   0 admin     (1000) admin     (1000)       79 2023-12-03 13:10:40.457297 parallel-pandas-0.6.2/setup.cfg
+-rw-rw-r--   0 admin     (1000) admin     (1000)      929 2023-12-03 13:10:27.000000 parallel-pandas-0.6.2/setup.py
```

### Comparing `parallel-pandas-0.6.1/LICENSE` & `parallel-pandas-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `parallel-pandas-0.6.1/PKG-INFO` & `parallel-pandas-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parallel-pandas
-Version: 0.6.1
+Version: 0.6.2
 Summary: Parallel processing on pandas with progress bars
 Home-page: https://github.com/dubovikmaster/parallel-pandas
 Author: Dubovik Pavel
 Author-email: geometryk@gmail.com
 License: MIT
 Keywords: parallel pandas,progress bar,parallel apply,parallel groupby,multiprocessing bar
 Platform: any
```

### Comparing `parallel-pandas-0.6.1/README.md` & `parallel-pandas-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `parallel-pandas-0.6.1/parallel_pandas/core/__init__.py` & `parallel-pandas-0.6.2/parallel_pandas/core/__init__.py`

 * *Files identical despite different names*

### Comparing `parallel-pandas-0.6.1/parallel_pandas/core/_numba.py` & `parallel-pandas-0.6.2/parallel_pandas/core/_numba.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import numpy as np
 
 try:
     from numba import njit, prange
+
+
     @njit
     def _pearson_corr(x, y):
         return np.corrcoef(x, y)[0, 1]
 
 
     @njit
     def calculate_rank(arr):
```

### Comparing `parallel-pandas-0.6.1/parallel_pandas/core/parallel_dataframe.py` & `parallel-pandas-0.6.2/parallel_pandas/core/parallel_dataframe.py`

 * *Files identical despite different names*

### Comparing `parallel-pandas-0.6.1/parallel_pandas/core/parallel_groupby.py` & `parallel-pandas-0.6.2/parallel_pandas/core/parallel_groupby.py`

 * *Files identical despite different names*

### Comparing `parallel-pandas-0.6.1/parallel_pandas/core/parallel_series.py` & `parallel-pandas-0.6.2/parallel_pandas/core/parallel_series.py`

 * *Files identical despite different names*

### Comparing `parallel-pandas-0.6.1/parallel_pandas/core/parallel_window.py` & `parallel-pandas-0.6.2/parallel_pandas/core/parallel_window.py`

 * *Files identical despite different names*

### Comparing `parallel-pandas-0.6.1/parallel_pandas/core/progress_imap.py` & `parallel-pandas-0.6.2/parallel_pandas/core/progress_imap.py`

 * *Files identical despite different names*

### Comparing `parallel-pandas-0.6.1/parallel_pandas/core/tools.py` & `parallel-pandas-0.6.2/parallel_pandas/core/tools.py`

 * *Files identical despite different names*

### Comparing `parallel-pandas-0.6.1/parallel_pandas/main.py` & `parallel-pandas-0.6.2/parallel_pandas/main.py`

 * *Files identical despite different names*

### Comparing `parallel-pandas-0.6.1/parallel_pandas.egg-info/PKG-INFO` & `parallel-pandas-0.6.2/parallel_pandas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parallel-pandas
-Version: 0.6.1
+Version: 0.6.2
 Summary: Parallel processing on pandas with progress bars
 Home-page: https://github.com/dubovikmaster/parallel-pandas
 Author: Dubovik Pavel
 Author-email: geometryk@gmail.com
 License: MIT
 Keywords: parallel pandas,progress bar,parallel apply,parallel groupby,multiprocessing bar
 Platform: any
```

### Comparing `parallel-pandas-0.6.1/parallel_pandas.egg-info/SOURCES.txt` & `parallel-pandas-0.6.2/parallel_pandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parallel-pandas-0.6.1/setup.py` & `parallel-pandas-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='parallel-pandas',
     python_requires='>=3.7',
-    version='0.6.1',
+    version='0.6.2',
     packages=find_packages(),
     author='Dubovik Pavel',
     author_email='geometryk@gmail.com',
     description='Parallel processing on pandas with progress bars',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=[
```

