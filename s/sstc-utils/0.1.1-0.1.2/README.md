# Comparing `tmp/sstc_utils-0.1.1.tar.gz` & `tmp/sstc_utils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sstc_utils-0.1.1.tar", max compression
+gzip compressed data, was "sstc_utils-0.1.2.tar", max compression
```

## Comparing `sstc_utils-0.1.1.tar` & `sstc_utils-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      846 2023-11-28 15:37:30.239310 sstc_utils-0.1.1/README.md
--rw-r--r--   0        0        0      598 2024-05-23 10:18:15.177754 sstc_utils-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       46 2024-05-23 08:34:23.958374 sstc_utils-0.1.1/src/sstc_utils/__init__.py
--rw-r--r--   0        0        0     2929 2023-12-05 15:57:45.920017 sstc_utils-0.1.1/src/sstc_utils/decorators.py
--rw-r--r--   0        0        0     1862 2024-05-23 10:12:48.247786 sstc_utils-0.1.1/src/sstc_utils/requirements.txt
--rw-r--r--   0        0        0     1713 2024-05-23 09:38:41.737988 sstc_utils-0.1.1/src/sstc_utils/utils.py
--rw-r--r--   0        0        0       21 2024-05-23 09:21:10.998097 sstc_utils-0.1.1/src/sstc_utils/version.py
--rw-r--r--   0        0        0     1450 1970-01-01 00:00:00.000000 sstc_utils-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      846 2023-11-28 15:37:30.239310 sstc_utils-0.1.2/README.md
+-rw-r--r--   0        0        0      640 2024-05-31 12:02:42.844280 sstc_utils-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       46 2024-05-23 08:34:23.958374 sstc_utils-0.1.2/src/sstc_utils/__init__.py
+-rw-r--r--   0        0        0     2929 2023-12-05 15:57:45.920017 sstc_utils-0.1.2/src/sstc_utils/decorators.py
+-rw-r--r--   0        0        0     1862 2024-05-23 10:12:48.247786 sstc_utils-0.1.2/src/sstc_utils/requirements.txt
+-rw-r--r--   0        0        0     1713 2024-05-23 09:38:41.737988 sstc_utils-0.1.2/src/sstc_utils/utils.py
+-rw-r--r--   0        0        0       21 2024-05-31 11:56:41.434296 sstc_utils-0.1.2/src/sstc_utils/version.py
+-rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 sstc_utils-0.1.2/PKG-INFO
```

### Comparing `sstc_utils-0.1.1/README.md` & `sstc_utils-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sstc_utils-0.1.1/src/sstc_utils/decorators.py` & `sstc_utils-0.1.2/src/sstc_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `sstc_utils-0.1.1/src/sstc_utils/requirements.txt` & `sstc_utils-0.1.2/src/sstc_utils/requirements.txt`

 * *Files identical despite different names*

### Comparing `sstc_utils-0.1.1/src/sstc_utils/utils.py` & `sstc_utils-0.1.2/src/sstc_utils/utils.py`

 * *Files identical despite different names*

### Comparing `sstc_utils-0.1.1/PKG-INFO` & `sstc_utils-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: sstc-utils
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Jobelund
 Author-email: 124563223+jobelund@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: mkdocs (>=1.5.3,<2.0.0)
-Requires-Dist: mkdocs-rtd-dropdown (>=1.0.2,<2.0.0)
+Requires-Dist: mkdocs
+Requires-Dist: mkdocs-rtd-dropdown
 Requires-Dist: mkdocstrings-python
-Requires-Dist: pyexiv2 (>=2.9.0,<3.0.0)
-Requires-Dist: pytest (>=7.4.3,<8.0.0)
-Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Requires-Dist: pyexiv2
+Requires-Dist: pytest
+Requires-Dist: pyyaml
 Description-Content-Type: text/markdown
 
 ![alt text](https://h24-original.s3.amazonaws.com/231546/28893673-EQhe9.png "SITES Spectral Thematic Center")
 # Swedish Infrastructure for Ecosystem Science (SITES) - Spectral | Thematic Center (SSTC)
 ["SITES spectral"](https://www.fieldsites.se/en-GB/sites-thematic-programs/sites-spectral-32634403)
```

