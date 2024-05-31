# Comparing `tmp/lazy_mongo-0.3.1.tar.gz` & `tmp/lazy_mongo-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_mongo-0.3.1.tar", max compression
+gzip compressed data, was "lazy_mongo-0.3.2.tar", max compression
```

## Comparing `lazy_mongo-0.3.1.tar` & `lazy_mongo-0.3.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       40 2024-03-08 03:29:01.600206 lazy_mongo-0.3.1/README.md
--rw-r--r--   0        0        0      207 2024-03-22 03:18:21.246648 lazy_mongo-0.3.1/lazy_mongo/__init__.py
--rw-r--r--   0        0        0      217 2024-05-28 06:19:06.611731 lazy_mongo-0.3.1/lazy_mongo/insert_response.py
--rw-r--r--   0        0        0     3089 2024-05-29 03:08:52.126191 lazy_mongo-0.3.1/lazy_mongo/lazy_collection.py
--rw-r--r--   0        0        0     2293 2024-05-29 03:08:54.930297 lazy_mongo-0.3.1/lazy_mongo/lazy_database.py
--rw-r--r--   0        0        0     2812 2024-05-28 06:19:18.974919 lazy_mongo-0.3.1/lazy_mongo/lazy_mongo.py
--rw-r--r--   0        0        0      211 2024-04-16 01:49:06.275740 lazy_mongo-0.3.1/lazy_mongo/update_response.py
--rw-r--r--   0        0        0      296 2024-05-29 03:09:06.082721 lazy_mongo-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 lazy_mongo-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       40 2024-03-08 03:29:01.600206 lazy_mongo-0.3.2/README.md
+-rw-r--r--   0        0        0      207 2024-03-22 03:18:21.246648 lazy_mongo-0.3.2/lazy_mongo/__init__.py
+-rw-r--r--   0        0        0      217 2024-05-28 06:19:06.611731 lazy_mongo-0.3.2/lazy_mongo/insert_response.py
+-rw-r--r--   0        0        0     3094 2024-05-31 01:35:52.316023 lazy_mongo-0.3.2/lazy_mongo/lazy_collection.py
+-rw-r--r--   0        0        0     2293 2024-05-29 03:08:54.930297 lazy_mongo-0.3.2/lazy_mongo/lazy_database.py
+-rw-r--r--   0        0        0     2812 2024-05-28 06:19:18.974919 lazy_mongo-0.3.2/lazy_mongo/lazy_mongo.py
+-rw-r--r--   0        0        0      211 2024-04-16 01:49:06.275740 lazy_mongo-0.3.2/lazy_mongo/update_response.py
+-rw-r--r--   0        0        0      296 2024-05-31 01:36:06.027924 lazy_mongo-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 lazy_mongo-0.3.2/PKG-INFO
```

### Comparing `lazy_mongo-0.3.1/lazy_mongo/lazy_collection.py` & `lazy_mongo-0.3.2/lazy_mongo/lazy_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             return InsertResponse(
                 ok=True,
                 result=result,
             )
 
         except DuplicateKeyError as e:
             if self.mongo.log:
-                print("[Mongo.Duplicate]", e)
+                print("[Mongo.Duplicate]", e.code)
 
             return InsertResponse(
                 ok=False,
                 is_duplicate=True,
                 error=e,
             )
```

### Comparing `lazy_mongo-0.3.1/lazy_mongo/lazy_database.py` & `lazy_mongo-0.3.2/lazy_mongo/lazy_database.py`

 * *Files identical despite different names*

### Comparing `lazy_mongo-0.3.1/lazy_mongo/lazy_mongo.py` & `lazy_mongo-0.3.2/lazy_mongo/lazy_mongo.py`

 * *Files identical despite different names*

### Comparing `lazy_mongo-0.3.1/PKG-INFO` & `lazy_mongo-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-mongo
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Author: MisterNyan
 Author-email: michael.edmund.wong@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

