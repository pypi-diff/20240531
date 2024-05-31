# Comparing `tmp/pandas-ods-reader-0.1.2.tar.gz` & `tmp/pandas-ods-reader-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-ods-reader-0.1.2.tar", last modified: Sun Aug 22 17:58:25 2021, max compression
+gzip compressed data, was "pandas-ods-reader-0.1.4.tar", max compression
```

## Comparing `pandas-ods-reader-0.1.2.tar` & `pandas-ods-reader-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,11 @@
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2021-08-22 17:58:25.634420 pandas-ods-reader-0.1.2/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     1063 2021-08-18 15:35:36.000000 pandas-ods-reader-0.1.2/LICENSE.txt
--rw-rw-r--   0 lukas     (1000) lukas     (1000)       72 2021-08-18 22:36:55.000000 pandas-ods-reader-0.1.2/MANIFEST.in
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3651 2021-08-22 17:58:25.634420 pandas-ods-reader-0.1.2/PKG-INFO
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     1451 2021-08-22 16:57:26.000000 pandas-ods-reader-0.1.2/README.md
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2021-08-22 17:58:25.630421 pandas-ods-reader-0.1.2/pandas_ods_reader/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)        6 2021-08-22 17:54:49.000000 pandas-ods-reader-0.1.2/pandas_ods_reader/VERSION
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      301 2021-08-22 17:44:29.000000 pandas-ods-reader-0.1.2/pandas_ods_reader/__init__.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2637 2021-08-22 16:06:36.000000 pandas-ods-reader-0.1.2/pandas_ods_reader/algo.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     1104 2021-08-22 16:06:36.000000 pandas-ods-reader-0.1.2/pandas_ods_reader/main.py
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2021-08-22 17:58:25.634420 pandas-ods-reader-0.1.2/pandas_ods_reader/parsers/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     1977 2021-08-22 16:06:36.000000 pandas-ods-reader-0.1.2/pandas_ods_reader/parsers/fods.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      592 2021-08-22 16:06:36.000000 pandas-ods-reader-0.1.2/pandas_ods_reader/parsers/ods.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      912 2021-08-22 16:06:36.000000 pandas-ods-reader-0.1.2/pandas_ods_reader/utils.py
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2021-08-22 17:58:25.634420 pandas-ods-reader-0.1.2/pandas_ods_reader.egg-info/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3651 2021-08-22 17:58:25.000000 pandas-ods-reader-0.1.2/pandas_ods_reader.egg-info/PKG-INFO
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      498 2021-08-22 17:58:25.000000 pandas-ods-reader-0.1.2/pandas_ods_reader.egg-info/SOURCES.txt
--rw-rw-r--   0 lukas     (1000) lukas     (1000)        1 2021-08-22 17:58:25.000000 pandas-ods-reader-0.1.2/pandas_ods_reader.egg-info/dependency_links.txt
--rw-rw-r--   0 lukas     (1000) lukas     (1000)        1 2021-08-18 15:43:45.000000 pandas-ods-reader-0.1.2/pandas_ods_reader.egg-info/not-zip-safe
--rw-rw-r--   0 lukas     (1000) lukas     (1000)       33 2021-08-22 17:58:25.000000 pandas-ods-reader-0.1.2/pandas_ods_reader.egg-info/requires.txt
--rw-rw-r--   0 lukas     (1000) lukas     (1000)       18 2021-08-22 17:58:25.000000 pandas-ods-reader-0.1.2/pandas_ods_reader.egg-info/top_level.txt
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      774 2021-08-22 17:58:25.634420 pandas-ods-reader-0.1.2/setup.cfg
--rw-rw-r--   0 lukas     (1000) lukas     (1000)       99 2021-08-22 16:46:27.000000 pandas-ods-reader-0.1.2/setup.py
+-rw-r--r--   0        0        0     1063 2021-10-03 15:05:38.294888 pandas-ods-reader-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0     1451 2021-10-03 15:05:38.294888 pandas-ods-reader-0.1.4/README.md
+-rw-r--r--   0        0        0      208 2021-10-04 15:04:12.773256 pandas-ods-reader-0.1.4/pandas_ods_reader/__init__.py
+-rw-r--r--   0        0        0     2637 2021-10-03 15:05:38.310933 pandas-ods-reader-0.1.4/pandas_ods_reader/algo.py
+-rw-r--r--   0        0        0     1157 2021-10-04 14:47:18.979161 pandas-ods-reader-0.1.4/pandas_ods_reader/main.py
+-rw-r--r--   0        0        0     1977 2021-10-03 15:05:38.310933 pandas-ods-reader-0.1.4/pandas_ods_reader/parsers/fods.py
+-rw-r--r--   0        0        0      592 2021-10-03 15:05:38.310933 pandas-ods-reader-0.1.4/pandas_ods_reader/parsers/ods.py
+-rw-r--r--   0        0        0      912 2021-10-03 15:05:38.310933 pandas-ods-reader-0.1.4/pandas_ods_reader/utils.py
+-rw-r--r--   0        0        0      835 2021-10-04 15:50:55.175387 pandas-ods-reader-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2439 1970-01-01 00:00:00.000000 pandas-ods-reader-0.1.4/setup.py
+-rw-r--r--   0        0        0     2530 1970-01-01 00:00:00.000000 pandas-ods-reader-0.1.4/PKG-INFO
```

### Comparing `pandas-ods-reader-0.1.2/LICENSE.txt` & `pandas-ods-reader-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pandas-ods-reader-0.1.2/README.md` & `pandas-ods-reader-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pandas-ods-reader-0.1.2/pandas_ods_reader/algo.py` & `pandas-ods-reader-0.1.4/pandas_ods_reader/algo.py`

 * *Files identical despite different names*

### Comparing `pandas-ods-reader-0.1.2/pandas_ods_reader/main.py` & `pandas-ods-reader-0.1.4/pandas_ods_reader/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 
 
 EXT_MAP = {".ods": ods, ".fods": fods}
 
 
 def read_ods(file_or_path, sheet=1, headers=True, columns=None):
     """
-    Read in the provided ods file and convert it to `pandas.DataFrame`.
+    Read in the provided ods or .ods file and convert it to `pandas.DataFrame`.
+    Will detect the filetype based on the file's extension or fall back to
+    ods.
 
     Parameters
     ----------
-    file_or_path : str
+    file_or_path : str or pathlib.Path
         The path to the .ods or .fods file.
     sheet : int or str, default 1
         If `int`, the 1 based index of the sheet to be read. If `str`, the
         name of the sheet to be read.
     header : bool, default True
         If `True`, then the first row is treated as the list of column names.
-    columns : list or None, optional
+    columns : list, default None, optional
         A list of column names to be used as headers.
 
     Returns
     -------
     pandas.DataFrame
         The content of the specified sheet as a DataFrame.
     """
-    backend = EXT_MAP.get(Path(file_or_path).suffix)
-    if not backend:
-        raise ValueError("Unknown filetype.")
+    backend = EXT_MAP.get(Path(file_or_path).suffix, ods)
     return algo.read_data(
         backend, file_or_path, sheet, headers=headers, columns=columns
     )
```

### Comparing `pandas-ods-reader-0.1.2/pandas_ods_reader/parsers/fods.py` & `pandas-ods-reader-0.1.4/pandas_ods_reader/parsers/fods.py`

 * *Files identical despite different names*

### Comparing `pandas-ods-reader-0.1.2/pandas_ods_reader/parsers/ods.py` & `pandas-ods-reader-0.1.4/pandas_ods_reader/parsers/ods.py`

 * *Files identical despite different names*

### Comparing `pandas-ods-reader-0.1.2/pandas_ods_reader/utils.py` & `pandas-ods-reader-0.1.4/pandas_ods_reader/utils.py`

 * *Files identical despite different names*

