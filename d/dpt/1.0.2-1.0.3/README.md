# Comparing `tmp/dpt-1.0.2.tar.gz` & `tmp/dpt-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpt-1.0.2.tar", last modified: Wed May 22 18:29:47 2024, max compression
+gzip compressed data, was "dpt-1.0.3.tar", last modified: Fri May 31 07:23:11 2024, max compression
```

## Comparing `dpt-1.0.2.tar` & `dpt-1.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 18:29:47.428633 dpt-1.0.2/
--rw-rw-rw-   0        0        0      188 2024-05-22 18:29:47.427630 dpt-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-22 18:29:47.382063 dpt-1.0.2/dpt/
--rw-rw-rw-   0        0        0      123 2024-03-05 23:00:59.000000 dpt-1.0.2/dpt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 18:29:47.416065 dpt-1.0.2/dpt/deployment/
--rw-rw-rw-   0        0        0        4 2024-02-01 03:57:26.000000 dpt-1.0.2/dpt/deployment/__init__.py
--rw-rw-rw-   0        0        0      110 2024-02-01 20:25:45.000000 dpt-1.0.2/dpt/deployment/common.py
--rw-rw-rw-   0        0        0     9539 2024-04-14 15:36:27.000000 dpt-1.0.2/dpt/deployment/deploy.py
--rw-rw-rw-   0        0        0     1054 2024-02-01 20:24:35.000000 dpt-1.0.2/dpt/deployment/extract.py
--rw-rw-rw-   0        0        0     1981 2024-02-01 20:24:46.000000 dpt-1.0.2/dpt/management.py
-drwxrwxrwx   0        0        0        0 2024-05-22 18:29:47.425623 dpt-1.0.2/dpt/mongo/
--rw-rw-rw-   0        0        0        4 2024-02-01 03:59:35.000000 dpt-1.0.2/dpt/mongo/__init__.py
--rw-rw-rw-   0        0        0      266 2024-01-27 22:13:49.000000 dpt-1.0.2/dpt/mongo/commands.py
--rw-rw-rw-   0        0        0     1032 2024-01-28 00:52:12.000000 dpt-1.0.2/dpt/mongo/files.py
--rw-rw-rw-   0        0        0    13269 2024-04-14 20:36:18.000000 dpt-1.0.2/dpt/processor.py
--rw-rw-rw-   0        0        0     6689 2024-05-22 18:29:30.000000 dpt-1.0.2/dpt/storage.py
-drwxrwxrwx   0        0        0        0 2024-05-22 18:29:47.408064 dpt-1.0.2/dpt.egg-info/
--rw-rw-rw-   0        0        0      188 2024-05-22 18:29:47.000000 dpt-1.0.2/dpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2024-05-22 18:29:47.000000 dpt-1.0.2/dpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 18:29:47.000000 dpt-1.0.2/dpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-22 18:29:47.000000 dpt-1.0.2/dpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-22 18:29:47.000000 dpt-1.0.2/dpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 18:29:47.429633 dpt-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      338 2024-05-22 18:29:44.000000 dpt-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:23:11.564511 dpt-1.0.3/
+-rw-rw-rw-   0        0        0      188 2024-05-31 07:23:11.563178 dpt-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-31 07:23:11.538176 dpt-1.0.3/dpt/
+-rw-rw-rw-   0        0        0      123 2024-03-05 23:00:59.000000 dpt-1.0.3/dpt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:23:11.557178 dpt-1.0.3/dpt/deployment/
+-rw-rw-rw-   0        0        0        4 2024-02-01 03:57:26.000000 dpt-1.0.3/dpt/deployment/__init__.py
+-rw-rw-rw-   0        0        0      110 2024-02-01 20:25:45.000000 dpt-1.0.3/dpt/deployment/common.py
+-rw-rw-rw-   0        0        0     9539 2024-04-14 15:36:27.000000 dpt-1.0.3/dpt/deployment/deploy.py
+-rw-rw-rw-   0        0        0     1054 2024-02-01 20:24:35.000000 dpt-1.0.3/dpt/deployment/extract.py
+-rw-rw-rw-   0        0        0     1981 2024-02-01 20:24:46.000000 dpt-1.0.3/dpt/management.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:23:11.561177 dpt-1.0.3/dpt/mongo/
+-rw-rw-rw-   0        0        0        4 2024-02-01 03:59:35.000000 dpt-1.0.3/dpt/mongo/__init__.py
+-rw-rw-rw-   0        0        0      266 2024-01-27 22:13:49.000000 dpt-1.0.3/dpt/mongo/commands.py
+-rw-rw-rw-   0        0        0     1032 2024-01-28 00:52:12.000000 dpt-1.0.3/dpt/mongo/files.py
+-rw-rw-rw-   0        0        0    13269 2024-04-14 20:36:18.000000 dpt-1.0.3/dpt/processor.py
+-rw-rw-rw-   0        0        0     6899 2024-05-31 07:19:33.000000 dpt-1.0.3/dpt/storage.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:23:11.551176 dpt-1.0.3/dpt.egg-info/
+-rw-rw-rw-   0        0        0      188 2024-05-31 07:23:11.000000 dpt-1.0.3/dpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2024-05-31 07:23:11.000000 dpt-1.0.3/dpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 07:23:11.000000 dpt-1.0.3/dpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-31 07:23:11.000000 dpt-1.0.3/dpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-31 07:23:11.000000 dpt-1.0.3/dpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 07:23:11.564511 dpt-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      338 2024-05-31 07:23:06.000000 dpt-1.0.3/setup.py
```

### Comparing `dpt-1.0.2/dpt/deployment/deploy.py` & `dpt-1.0.3/dpt/deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `dpt-1.0.2/dpt/deployment/extract.py` & `dpt-1.0.3/dpt/deployment/extract.py`

 * *Files identical despite different names*

### Comparing `dpt-1.0.2/dpt/management.py` & `dpt-1.0.3/dpt/management.py`

 * *Files identical despite different names*

### Comparing `dpt-1.0.2/dpt/mongo/files.py` & `dpt-1.0.3/dpt/mongo/files.py`

 * *Files identical despite different names*

### Comparing `dpt-1.0.2/dpt/processor.py` & `dpt-1.0.3/dpt/processor.py`

 * *Files identical despite different names*

### Comparing `dpt-1.0.2/dpt/storage.py` & `dpt-1.0.3/dpt/storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+import json
 from pymongo import MongoClient
 from pymongo.database import Database as MongoDatabase
 from pymongo.collection import Collection
 from typing import Any, Optional
 import jsonschema
 import copy
 
@@ -123,15 +124,20 @@
 
     def aggregate(self, out: DbWriter, pipeline: list[dict[str, Any]]):
         self._update_count_from_collection()
         self._prepare_pipeline(pipeline)
         self._create_lookup_indexes(pipeline)
         pipeline.append({"$out": out._collection_name})
         print(f"read {self._count} documents from {self.get_info()}")
-        print("run aggregation:\n", pipeline)
+        print("")
+        pipeline_json = json.dumps(pipeline,ensure_ascii=False)
+        print("run aggregation:")
+        print("")
+        print(f'db.getCollection("{self.instance().name}").aggregate(\n{pipeline_json}\n)')
+        print("")
         self.instance().aggregate(pipeline)
         out._update_count_from_collection()
         out.close()
 
     def create_index(
         self,
         keys,
```

