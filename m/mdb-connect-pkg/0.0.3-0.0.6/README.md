# Comparing `tmp/mdb_connect_pkg-0.0.3.tar.gz` & `tmp/mdb_connect_pkg-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdb_connect_pkg-0.0.3.tar", last modified: Wed May 29 17:54:38 2024, max compression
+gzip compressed data, was "mdb_connect_pkg-0.0.6.tar", last modified: Fri May 31 02:47:02 2024, max compression
```

## Comparing `mdb_connect_pkg-0.0.3.tar` & `mdb_connect_pkg-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:54:38.330097 mdb_connect_pkg-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-29 17:54:11.000000 mdb_connect_pkg-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-29 17:54:38.330097 mdb_connect_pkg-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-29 17:54:11.000000 mdb_connect_pkg-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-29 17:54:11.000000 mdb_connect_pkg-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-29 17:54:38.330097 mdb_connect_pkg-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-29 17:54:11.000000 mdb_connect_pkg-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:54:38.326097 mdb_connect_pkg-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:54:38.326097 mdb_connect_pkg-0.0.3/src/mdb_connect_pkg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:54:11.000000 mdb_connect_pkg-0.0.3/src/mdb_connect_pkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-29 17:54:11.000000 mdb_connect_pkg-0.0.3/src/mdb_connect_pkg/mongo_crud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:54:38.330097 mdb_connect_pkg-0.0.3/src/mdb_connect_pkg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-29 17:54:38.000000 mdb_connect_pkg-0.0.3/src/mdb_connect_pkg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-29 17:54:38.000000 mdb_connect_pkg-0.0.3/src/mdb_connect_pkg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:54:38.000000 mdb_connect_pkg-0.0.3/src/mdb_connect_pkg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-29 17:54:38.000000 mdb_connect_pkg-0.0.3/src/mdb_connect_pkg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 17:54:38.000000 mdb_connect_pkg-0.0.3/src/mdb_connect_pkg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 02:47:02.645506 mdb_connect_pkg-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-31 02:46:41.000000 mdb_connect_pkg-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-31 02:47:02.645506 mdb_connect_pkg-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-31 02:46:41.000000 mdb_connect_pkg-0.0.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-31 02:46:41.000000 mdb_connect_pkg-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-31 02:47:02.645506 mdb_connect_pkg-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-31 02:46:41.000000 mdb_connect_pkg-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 02:47:02.641506 mdb_connect_pkg-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 02:47:02.641506 mdb_connect_pkg-0.0.6/src/mdb_connect_pkg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 02:46:41.000000 mdb_connect_pkg-0.0.6/src/mdb_connect_pkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-31 02:46:41.000000 mdb_connect_pkg-0.0.6/src/mdb_connect_pkg/mongo_crud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 02:47:02.645506 mdb_connect_pkg-0.0.6/src/mdb_connect_pkg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-31 02:47:02.000000 mdb_connect_pkg-0.0.6/src/mdb_connect_pkg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-31 02:47:02.000000 mdb_connect_pkg-0.0.6/src/mdb_connect_pkg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 02:47:02.000000 mdb_connect_pkg-0.0.6/src/mdb_connect_pkg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-31 02:47:02.000000 mdb_connect_pkg-0.0.6/src/mdb_connect_pkg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 02:47:02.000000 mdb_connect_pkg-0.0.6/src/mdb_connect_pkg.egg-info/top_level.txt
```

### Comparing `mdb_connect_pkg-0.0.3/LICENSE` & `mdb_connect_pkg-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mdb_connect_pkg-0.0.3/setup.cfg` & `mdb_connect_pkg-0.0.6/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 [metadata]
 license = MIT
 license_file = LICENSE
 classifiers = 
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Operating System :: OS Independent
 
 [options]
+python_requires = >=3.8
 install_requires = 
-	ensure==1.0.2
-	py-youtube==1.1.7
-python_requires = >=3.7
+	pymongo
+	pymongo[srv]
+	dnspython
+	pandas
+	numpy
+	ensure
 
 [options.extras_require]
 testing = 
 	pytest>=7.1.3
 	mypy>=0.971
 	flake8>=5.0.4
-	tox>=3.25.1
+	tox>=3.24.4
 	black>=22.8.0
 
 [options.package_data]
 MongoDB-Connect = py.typed
 
 [flake8]
 max-line-length = 160
```

### Comparing `mdb_connect_pkg-0.0.3/src/mdb_connect_pkg/mongo_crud.py` & `mdb_connect_pkg-0.0.6/src/mdb_connect_pkg/mongo_crud.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # importing necessary libraries:
 from pathlib import Path
 import pandas as pd
 from pymongo.mongo_client import MongoClient
 import json
+import warnings
+warnings.filterwarnings('ignore')
 
 
 # creatring a class for mongodb connection:
 class MongoDBConnection:
 
     # constructor:
     def __init__(self, client_url: str, database_name: str, collection_name: str):
@@ -50,8 +52,28 @@
             coll.insert_many(csv_file_data)
 
     # load the collection as a dataframe:
     def load_data(self):
         collection = self.collection_()
         data = collection.find()
         df = pd.DataFrame(list(data))
+        df.drop('_id', axis=1, inplace=True)
         return df
+
+    # updating the data:
+    def update_data(self, *query):
+        collection = self.collection_()
+        collection.update_many(*query)
+
+    # delete the data:
+    def delete_record(self, *query):
+        collection = self.collection_()
+        collection.delete_many(*query)
+
+    # drop the entire collection:
+    def drop_collection(self):
+        collection = self.collection_()
+        collection.drop()
+
+    # drop the entire database:
+    def drop_database(self):
+        self.client.drop_database(self.database_name)
```

