# Comparing `tmp/mtgcdb-0.1.5.tar.gz` & `tmp/mtgcdb-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtgcdb-0.1.5.tar", max compression
+gzip compressed data, was "mtgcdb-0.1.6.tar", max compression
```

## Comparing `mtgcdb-0.1.5.tar` & `mtgcdb-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2024-05-30 23:50:57.330439 mtgcdb-0.1.5/LICENSE
--rw-r--r--   0        0        0      203 2024-05-30 23:50:57.330439 mtgcdb-0.1.5/README.md
--rw-r--r--   0        0        0      612 2024-05-30 23:51:04.714466 mtgcdb-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       71 2024-05-30 23:50:57.334439 mtgcdb-0.1.5/src/mtgcdb/__init__.py
--rw-r--r--   0        0        0     1201 2024-05-30 23:50:57.334439 mtgcdb-0.1.5/src/mtgcdb/card.py
--rw-r--r--   0        0        0     3483 2024-05-30 23:50:57.334439 mtgcdb-0.1.5/src/mtgcdb/db.py
--rw-r--r--   0        0        0     4848 2024-05-30 23:50:57.334439 mtgcdb-0.1.5/src/mtgcdb/mtgcdb.py
--rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 mtgcdb-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-31 17:12:53.635470 mtgcdb-0.1.6/LICENSE
+-rw-r--r--   0        0        0      203 2024-05-31 17:12:53.635470 mtgcdb-0.1.6/README.md
+-rw-r--r--   0        0        0      612 2024-05-31 17:13:02.707452 mtgcdb-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       71 2024-05-31 17:13:02.703452 mtgcdb-0.1.6/src/mtgcdb/__init__.py
+-rw-r--r--   0        0        0     1201 2024-05-31 17:12:53.635470 mtgcdb-0.1.6/src/mtgcdb/card.py
+-rw-r--r--   0        0        0     3483 2024-05-31 17:12:53.635470 mtgcdb-0.1.6/src/mtgcdb/db.py
+-rw-r--r--   0        0        0     4848 2024-05-31 17:12:53.635470 mtgcdb-0.1.6/src/mtgcdb/mtgcdb.py
+-rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 mtgcdb-0.1.6/PKG-INFO
```

### Comparing `mtgcdb-0.1.5/LICENSE` & `mtgcdb-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mtgcdb-0.1.5/src/mtgcdb/card.py` & `mtgcdb-0.1.6/src/mtgcdb/card.py`

 * *Files identical despite different names*

### Comparing `mtgcdb-0.1.5/src/mtgcdb/db.py` & `mtgcdb-0.1.6/src/mtgcdb/db.py`

 * *Files identical despite different names*

### Comparing `mtgcdb-0.1.5/src/mtgcdb/mtgcdb.py` & `mtgcdb-0.1.6/src/mtgcdb/mtgcdb.py`

 * *Files identical despite different names*

### Comparing `mtgcdb-0.1.5/PKG-INFO` & `mtgcdb-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtgcdb
-Version: 0.1.5
+Version: 0.1.6
 Summary: MTG Card Database
 License: Apache 2.0
 Author: j6e
 Author-email: jongares@hotmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

