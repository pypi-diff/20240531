# Comparing `tmp/edaeasy-1.0.1.tar.gz` & `tmp/edaeasy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edaeasy-1.0.1.tar", max compression
+gzip compressed data, was "edaeasy-1.1.0.tar", max compression
```

## Comparing `edaeasy-1.0.1.tar` & `edaeasy-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1093 2023-08-30 17:58:18.245963 edaeasy-1.0.1/LICENSE
--rw-r--r--   0        0        0     1835 2023-07-28 01:32:55.456083 edaeasy-1.0.1/README.md
--rw-r--r--   0        0        0      538 2023-08-31 02:18:09.152286 edaeasy-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       71 2023-08-31 00:50:42.781565 edaeasy-1.0.1/src/edaeasy/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 19:33:18.234490 edaeasy-1.0.1/src/edaeasy/config.toml
--rw-r--r--   0        0        0     3022 2023-07-28 01:32:17.302672 edaeasy-1.0.1/src/edaeasy/functions.py
--rw-r--r--   0        0        0     2522 1970-01-01 00:00:00.000000 edaeasy-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-08-30 17:58:18.245963 edaeasy-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1835 2023-07-28 01:32:55.456083 edaeasy-1.1.0/README.md
+-rw-r--r--   0        0        0      588 2024-05-30 19:33:42.729950 edaeasy-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       71 2023-08-31 00:50:42.781565 edaeasy-1.1.0/src/edaeasy/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 19:33:18.234490 edaeasy-1.1.0/src/edaeasy/config.toml
+-rw-r--r--   0        0        0     4406 2024-05-30 19:27:52.911119 edaeasy-1.1.0/src/edaeasy/functions.py
+-rw-r--r--   0        0        0     2559 1970-01-01 00:00:00.000000 edaeasy-1.1.0/PKG-INFO
```

### Comparing `edaeasy-1.0.1/LICENSE` & `edaeasy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edaeasy-1.0.1/README.md` & `edaeasy-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `edaeasy-1.0.1/pyproject.toml` & `edaeasy-1.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 [tool.poetry]
 name = "EDAeasy"
-version = "1.0.1"
+version = "1.1.0"
 description = "Functions and tools for making Exploratory Data Analysis easy!"
 authors = ["Francisco Jesus Ocazionez Cardozo <pach812@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["Exploratory Analysis","EDA"]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.9,<4.0"
 numpy = "^1.24.0"
 pandas = ">=1.5.0"
+statsmodels = "^0.14.2"
+pingouin = "^0.5.4"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 black = "^23.7.0"
 pip-tools = "^7.3.0"
```

### Comparing `edaeasy-1.0.1/PKG-INFO` & `edaeasy-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: EDAeasy
-Version: 1.0.1
+Version: 1.1.0
 Summary: Functions and tools for making Exploratory Data Analysis easy!
 License: MIT
 Keywords: Exploratory Analysis,EDA
 Author: Francisco Jesus Ocazionez Cardozo
 Author-email: pach812@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.0,<2.0.0)
 Requires-Dist: pandas (>=1.5.0)
+Requires-Dist: pingouin (>=0.5.4,<0.6.0)
+Requires-Dist: statsmodels (>=0.14.2,<0.15.0)
 Description-Content-Type: text/markdown
 
 # EDAeasy 😀
 The package for quick exploratory data analysis
 
 
 ## Instalation
```

