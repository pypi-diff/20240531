# Comparing `tmp/neo4j_uploader-0.5.3.tar.gz` & `tmp/neo4j_uploader-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo4j_uploader-0.5.3.tar", max compression
+gzip compressed data, was "neo4j_uploader-0.5.4.tar", max compression
```

## Comparing `neo4j_uploader-0.5.3.tar` & `neo4j_uploader-0.5.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2024-01-09 01:53:44.393152 neo4j_uploader-0.5.3/LICENSE.txt
--rw-r--r--   0        0        0     2115 2024-01-09 01:53:44.393436 neo4j_uploader-0.5.3/README.md
--rw-r--r--   0        0        0     9199 2024-02-15 02:03:18.871243 neo4j_uploader-0.5.3/neo4j_uploader/__init__.py
--rw-r--r--   0        0        0     1873 2024-01-09 01:53:44.401080 neo4j_uploader-0.5.3/neo4j_uploader/_conversions.py
--rw-r--r--   0        0        0     2017 2024-01-09 01:53:44.401361 neo4j_uploader-0.5.3/neo4j_uploader/_logger.py
--rw-r--r--   0        0        0     2507 2024-02-15 02:03:15.182832 neo4j_uploader-0.5.3/neo4j_uploader/_n4j.py
--rw-r--r--   0        0        0    12364 2024-01-09 01:53:44.401971 neo4j_uploader-0.5.3/neo4j_uploader/_queries.py
--rw-r--r--   0        0        0    17709 2024-01-09 01:53:44.402249 neo4j_uploader-0.5.3/neo4j_uploader/_upload_utils.py
--rw-r--r--   0        0        0      202 2024-01-09 01:53:44.402593 neo4j_uploader-0.5.3/neo4j_uploader/errors.py
--rw-r--r--   0        0        0     4240 2024-01-09 01:53:44.402991 neo4j_uploader-0.5.3/neo4j_uploader/models.py
--rw-r--r--   0        0        0      431 2024-02-15 02:04:40.845839 neo4j_uploader-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     2583 1970-01-01 00:00:00.000000 neo4j_uploader-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-01-09 01:53:44.393152 neo4j_uploader-0.5.4/LICENSE.txt
+-rw-r--r--   0        0        0     2115 2024-01-09 01:53:44.393436 neo4j_uploader-0.5.4/README.md
+-rw-r--r--   0        0        0     9199 2024-05-31 20:45:56.693846 neo4j_uploader-0.5.4/neo4j_uploader/__init__.py
+-rw-r--r--   0        0        0     1873 2024-01-09 01:53:44.401080 neo4j_uploader-0.5.4/neo4j_uploader/_conversions.py
+-rw-r--r--   0        0        0     2017 2024-03-07 22:50:49.059425 neo4j_uploader-0.5.4/neo4j_uploader/_logger.py
+-rw-r--r--   0        0        0     2507 2024-02-15 02:03:15.182832 neo4j_uploader-0.5.4/neo4j_uploader/_n4j.py
+-rw-r--r--   0        0        0    12364 2024-05-31 20:45:56.695162 neo4j_uploader-0.5.4/neo4j_uploader/_queries.py
+-rw-r--r--   0        0        0    17709 2024-01-09 01:53:44.402249 neo4j_uploader-0.5.4/neo4j_uploader/_upload_utils.py
+-rw-r--r--   0        0        0      202 2024-01-09 01:53:44.402593 neo4j_uploader-0.5.4/neo4j_uploader/errors.py
+-rw-r--r--   0        0        0     4240 2024-05-31 20:45:56.695780 neo4j_uploader-0.5.4/neo4j_uploader/models.py
+-rw-r--r--   0        0        0      442 2024-05-31 20:51:52.882167 neo4j_uploader-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2647 1970-01-01 00:00:00.000000 neo4j_uploader-0.5.4/PKG-INFO
```

### Comparing `neo4j_uploader-0.5.3/LICENSE.txt` & `neo4j_uploader-0.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neo4j_uploader-0.5.3/README.md` & `neo4j_uploader-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `neo4j_uploader-0.5.3/neo4j_uploader/__init__.py` & `neo4j_uploader-0.5.4/neo4j_uploader/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j_uploader-0.5.3/neo4j_uploader/_conversions.py` & `neo4j_uploader-0.5.4/neo4j_uploader/_conversions.py`

 * *Files identical despite different names*

### Comparing `neo4j_uploader-0.5.3/neo4j_uploader/_logger.py` & `neo4j_uploader-0.5.4/neo4j_uploader/_logger.py`

 * *Files identical despite different names*

### Comparing `neo4j_uploader-0.5.3/neo4j_uploader/_n4j.py` & `neo4j_uploader-0.5.4/neo4j_uploader/_n4j.py`

 * *Files identical despite different names*

### Comparing `neo4j_uploader-0.5.3/neo4j_uploader/_queries.py` & `neo4j_uploader-0.5.4/neo4j_uploader/_queries.py`

 * *Files identical despite different names*

### Comparing `neo4j_uploader-0.5.3/neo4j_uploader/_upload_utils.py` & `neo4j_uploader-0.5.4/neo4j_uploader/_upload_utils.py`

 * *Files identical despite different names*

### Comparing `neo4j_uploader-0.5.3/neo4j_uploader/models.py` & `neo4j_uploader-0.5.4/neo4j_uploader/models.py`

 * *Files identical despite different names*

### Comparing `neo4j_uploader-0.5.3/PKG-INFO` & `neo4j_uploader-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: neo4j-uploader
-Version: 0.5.3
+Version: 0.5.4
 Summary: 
 Author: Jason Koo
 Author-email: jalakoo@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: neo4j (>=5.14.1,<6.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: neo4j-rust-ext (>=5.20.0.0,<6.0.0.0)
 Requires-Dist: pydantic (>=2.5.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Neo4j-uploader
 For uploading specially formatted dictionary data to a Neo4j database instance.
 
 ## Installation
```

