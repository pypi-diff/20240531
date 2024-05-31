# Comparing `tmp/xchainpy2_utils-0.0.4.tar.gz` & `tmp/xchainpy2_utils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xchainpy2_utils-0.0.4.tar", last modified: Tue Dec  5 14:36:16 2023, max compression
+gzip compressed data, was "xchainpy2_utils-0.0.6.tar", last modified: Tue Dec  5 14:48:28 2023, max compression
```

## Comparing `xchainpy2_utils-0.0.4.tar` & `xchainpy2_utils-0.0.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2023-12-05 14:36:16.948966 xchainpy2_utils-0.0.4/
--rw-r--r--   0 tirinox    (501) staff       (20)     1086 2023-04-22 16:09:04.000000 xchainpy2_utils-0.0.4/LICENSE
--rw-r--r--   0 tirinox    (501) staff       (20)     1168 2023-12-05 14:36:16.948717 xchainpy2_utils-0.0.4/PKG-INFO
--rw-r--r--   0 tirinox    (501) staff       (20)      231 2023-04-22 16:09:04.000000 xchainpy2_utils-0.0.4/README.md
--rw-r--r--   0 tirinox    (501) staff       (20)     1225 2023-10-09 09:24:07.000000 xchainpy2_utils-0.0.4/pyproject.toml
--rw-r--r--   0 tirinox    (501) staff       (20)       38 2023-12-05 14:36:16.949012 xchainpy2_utils-0.0.4/setup.cfg
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2023-12-05 14:36:16.945753 xchainpy2_utils-0.0.4/xchainpy2_utils/
--rw-r--r--   0 tirinox    (501) staff       (20)      168 2023-10-27 11:08:10.000000 xchainpy2_utils-0.0.4/xchainpy2_utils/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)     8844 2023-11-25 07:56:04.000000 xchainpy2_utils-0.0.4/xchainpy2_utils/amount.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2806 2023-11-25 07:57:35.000000 xchainpy2_utils-0.0.4/xchainpy2_utils/asset.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3041 2023-11-24 19:11:50.000000 xchainpy2_utils-0.0.4/xchainpy2_utils/consts.py
--rw-r--r--   0 tirinox    (501) staff       (20)      455 2023-10-27 11:08:10.000000 xchainpy2_utils-0.0.4/xchainpy2_utils/dates.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3074 2023-04-23 14:23:49.000000 xchainpy2_utils-0.0.4/xchainpy2_utils/format.py
--rw-r--r--   0 tirinox    (501) staff       (20)       66 2023-04-23 08:08:00.000000 xchainpy2_utils-0.0.4/xchainpy2_utils/math.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1255 2023-11-09 17:37:25.000000 xchainpy2_utils-0.0.4/xchainpy2_utils/seqs.py
--rw-r--r--   0 tirinox    (501) staff       (20)    11671 2023-06-04 14:28:14.000000 xchainpy2_utils-0.0.4/xchainpy2_utils/swap.py
--rw-r--r--   0 tirinox    (501) staff       (20)      223 2023-07-20 11:54:44.000000 xchainpy2_utils-0.0.4/xchainpy2_utils/testing_utils.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2023-12-05 14:36:16.947888 xchainpy2_utils-0.0.4/xchainpy2_utils/tests/
--rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-04-22 16:09:04.000000 xchainpy2_utils-0.0.4/xchainpy2_utils/tests/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4176 2023-11-19 09:49:41.000000 xchainpy2_utils-0.0.4/xchainpy2_utils/tests/test_amount.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2755 2023-07-10 15:41:13.000000 xchainpy2_utils-0.0.4/xchainpy2_utils/tests/test_asset.py
--rw-r--r--   0 tirinox    (501) staff       (20)      974 2023-11-19 09:49:41.000000 xchainpy2_utils-0.0.4/xchainpy2_utils/tests/test_crypto_amount.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2182 2023-04-23 14:25:24.000000 xchainpy2_utils-0.0.4/xchainpy2_utils/tests/test_money_format.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1424 2023-07-10 15:29:37.000000 xchainpy2_utils-0.0.4/xchainpy2_utils/tests/test_utils.py
--rw-r--r--   0 tirinox    (501) staff       (20)      299 2023-10-06 16:54:52.000000 xchainpy2_utils-0.0.4/xchainpy2_utils/util.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2023-12-05 14:36:16.948245 xchainpy2_utils-0.0.4/xchainpy2_utils.egg-info/
--rw-r--r--   0 tirinox    (501) staff       (20)     1168 2023-12-05 14:36:16.000000 xchainpy2_utils-0.0.4/xchainpy2_utils.egg-info/PKG-INFO
--rw-r--r--   0 tirinox    (501) staff       (20)      741 2023-12-05 14:36:16.000000 xchainpy2_utils-0.0.4/xchainpy2_utils.egg-info/SOURCES.txt
--rw-r--r--   0 tirinox    (501) staff       (20)        1 2023-12-05 14:36:16.000000 xchainpy2_utils-0.0.4/xchainpy2_utils.egg-info/dependency_links.txt
--rw-r--r--   0 tirinox    (501) staff       (20)       15 2023-12-05 14:36:16.000000 xchainpy2_utils-0.0.4/xchainpy2_utils.egg-info/requires.txt
--rw-r--r--   0 tirinox    (501) staff       (20)       16 2023-12-05 14:36:16.000000 xchainpy2_utils-0.0.4/xchainpy2_utils.egg-info/top_level.txt
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2023-12-05 14:48:28.733783 xchainpy2_utils-0.0.6/
+-rw-r--r--   0 tirinox    (501) staff       (20)     1086 2023-04-22 16:09:04.000000 xchainpy2_utils-0.0.6/LICENSE
+-rw-r--r--   0 tirinox    (501) staff       (20)     1168 2023-12-05 14:48:28.733554 xchainpy2_utils-0.0.6/PKG-INFO
+-rw-r--r--   0 tirinox    (501) staff       (20)      231 2023-12-05 14:47:30.000000 xchainpy2_utils-0.0.6/README.md
+-rw-r--r--   0 tirinox    (501) staff       (20)     1225 2023-12-05 14:47:30.000000 xchainpy2_utils-0.0.6/pyproject.toml
+-rw-r--r--   0 tirinox    (501) staff       (20)       38 2023-12-05 14:48:28.733825 xchainpy2_utils-0.0.6/setup.cfg
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2023-12-05 14:48:28.730863 xchainpy2_utils-0.0.6/xchainpy2_utils/
+-rw-r--r--   0 tirinox    (501) staff       (20)      168 2023-10-27 11:08:10.000000 xchainpy2_utils-0.0.6/xchainpy2_utils/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     8844 2023-11-25 07:56:04.000000 xchainpy2_utils-0.0.6/xchainpy2_utils/amount.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2806 2023-11-25 07:57:35.000000 xchainpy2_utils-0.0.6/xchainpy2_utils/asset.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3041 2023-11-24 19:11:50.000000 xchainpy2_utils-0.0.6/xchainpy2_utils/consts.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      455 2023-10-27 11:08:10.000000 xchainpy2_utils-0.0.6/xchainpy2_utils/dates.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3074 2023-04-23 14:23:49.000000 xchainpy2_utils-0.0.6/xchainpy2_utils/format.py
+-rw-r--r--   0 tirinox    (501) staff       (20)       66 2023-04-23 08:08:00.000000 xchainpy2_utils-0.0.6/xchainpy2_utils/math.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1255 2023-11-09 17:37:25.000000 xchainpy2_utils-0.0.6/xchainpy2_utils/seqs.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    11671 2023-06-04 14:28:14.000000 xchainpy2_utils-0.0.6/xchainpy2_utils/swap.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      223 2023-07-20 11:54:44.000000 xchainpy2_utils-0.0.6/xchainpy2_utils/testing_utils.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2023-12-05 14:48:28.732843 xchainpy2_utils-0.0.6/xchainpy2_utils/tests/
+-rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-04-22 16:09:04.000000 xchainpy2_utils-0.0.6/xchainpy2_utils/tests/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4176 2023-11-19 09:49:41.000000 xchainpy2_utils-0.0.6/xchainpy2_utils/tests/test_amount.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2755 2023-07-10 15:41:13.000000 xchainpy2_utils-0.0.6/xchainpy2_utils/tests/test_asset.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      974 2023-11-19 09:49:41.000000 xchainpy2_utils-0.0.6/xchainpy2_utils/tests/test_crypto_amount.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2182 2023-04-23 14:25:24.000000 xchainpy2_utils-0.0.6/xchainpy2_utils/tests/test_money_format.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1424 2023-07-10 15:29:37.000000 xchainpy2_utils-0.0.6/xchainpy2_utils/tests/test_utils.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      299 2023-10-06 16:54:52.000000 xchainpy2_utils-0.0.6/xchainpy2_utils/util.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2023-12-05 14:48:28.733122 xchainpy2_utils-0.0.6/xchainpy2_utils.egg-info/
+-rw-r--r--   0 tirinox    (501) staff       (20)     1168 2023-12-05 14:48:28.000000 xchainpy2_utils-0.0.6/xchainpy2_utils.egg-info/PKG-INFO
+-rw-r--r--   0 tirinox    (501) staff       (20)      741 2023-12-05 14:48:28.000000 xchainpy2_utils-0.0.6/xchainpy2_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)        1 2023-12-05 14:48:28.000000 xchainpy2_utils-0.0.6/xchainpy2_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)       15 2023-12-05 14:48:28.000000 xchainpy2_utils-0.0.6/xchainpy2_utils.egg-info/requires.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)       16 2023-12-05 14:48:28.000000 xchainpy2_utils-0.0.6/xchainpy2_utils.egg-info/top_level.txt
```

### Comparing `xchainpy2_utils-0.0.4/LICENSE` & `xchainpy2_utils-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xchainpy2_utils-0.0.4/PKG-INFO` & `xchainpy2_utils-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchainpy2_utils
-Version: 0.0.4
+Version: 0.0.6
 Summary: XChainPy 2 Utils
 Author-email: Tirinox <developer@tirinox.ru>
 License: MIT
 Project-URL: source, https://github.com/tirinox/xchainpy
 Keywords: Crypto,THORChain,Blockchain,XChain
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -30,8 +30,8 @@
 ## Modules (in alphabetical order)
 
 - `asset` - Utilities for handling assets
 - `amount` - Utilities for handling amounts
 
 ## Installation
 
-`pip install xchainpy_util`
+`pip install xchainpy-util`
```

### Comparing `xchainpy2_utils-0.0.4/pyproject.toml` & `xchainpy2_utils-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xchainpy2_utils"
-version = "0.0.4"
+version = "0.0.6"
 authors = [
     { name = "Tirinox", email = "developer@tirinox.ru" },
 ]
 description = "XChainPy 2 Utils"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["Crypto", "THORChain", "Blockchain", "XChain"]
```

### Comparing `xchainpy2_utils-0.0.4/xchainpy2_utils/amount.py` & `xchainpy2_utils-0.0.6/xchainpy2_utils/amount.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_utils-0.0.4/xchainpy2_utils/asset.py` & `xchainpy2_utils-0.0.6/xchainpy2_utils/asset.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_utils-0.0.4/xchainpy2_utils/consts.py` & `xchainpy2_utils-0.0.6/xchainpy2_utils/consts.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_utils-0.0.4/xchainpy2_utils/format.py` & `xchainpy2_utils-0.0.6/xchainpy2_utils/format.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_utils-0.0.4/xchainpy2_utils/seqs.py` & `xchainpy2_utils-0.0.6/xchainpy2_utils/seqs.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_utils-0.0.4/xchainpy2_utils/swap.py` & `xchainpy2_utils-0.0.6/xchainpy2_utils/swap.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_utils-0.0.4/xchainpy2_utils/tests/test_amount.py` & `xchainpy2_utils-0.0.6/xchainpy2_utils/tests/test_amount.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_utils-0.0.4/xchainpy2_utils/tests/test_asset.py` & `xchainpy2_utils-0.0.6/xchainpy2_utils/tests/test_asset.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_utils-0.0.4/xchainpy2_utils/tests/test_crypto_amount.py` & `xchainpy2_utils-0.0.6/xchainpy2_utils/tests/test_crypto_amount.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_utils-0.0.4/xchainpy2_utils/tests/test_money_format.py` & `xchainpy2_utils-0.0.6/xchainpy2_utils/tests/test_money_format.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_utils-0.0.4/xchainpy2_utils/tests/test_utils.py` & `xchainpy2_utils-0.0.6/xchainpy2_utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_utils-0.0.4/xchainpy2_utils.egg-info/PKG-INFO` & `xchainpy2_utils-0.0.6/xchainpy2_utils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchainpy2-utils
-Version: 0.0.4
+Version: 0.0.6
 Summary: XChainPy 2 Utils
 Author-email: Tirinox <developer@tirinox.ru>
 License: MIT
 Project-URL: source, https://github.com/tirinox/xchainpy
 Keywords: Crypto,THORChain,Blockchain,XChain
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -30,8 +30,8 @@
 ## Modules (in alphabetical order)
 
 - `asset` - Utilities for handling assets
 - `amount` - Utilities for handling amounts
 
 ## Installation
 
-`pip install xchainpy_util`
+`pip install xchainpy-util`
```

### Comparing `xchainpy2_utils-0.0.4/xchainpy2_utils.egg-info/SOURCES.txt` & `xchainpy2_utils-0.0.6/xchainpy2_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

