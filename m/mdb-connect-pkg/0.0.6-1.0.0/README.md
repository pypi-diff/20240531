# Comparing `tmp/mdb_connect_pkg-0.0.6.tar.gz` & `tmp/mdb_connect_pkg-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdb_connect_pkg-0.0.6.tar", last modified: Fri May 31 02:47:02 2024, max compression
+gzip compressed data, was "mdb_connect_pkg-1.0.0.tar", last modified: Fri May 31 03:19:20 2024, max compression
```

## Comparing `mdb_connect_pkg-0.0.6.tar` & `mdb_connect_pkg-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 02:47:02.645506 mdb_connect_pkg-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-31 02:46:41.000000 mdb_connect_pkg-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-31 02:47:02.645506 mdb_connect_pkg-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-31 02:46:41.000000 mdb_connect_pkg-0.0.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-31 02:46:41.000000 mdb_connect_pkg-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-31 02:47:02.645506 mdb_connect_pkg-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-31 02:46:41.000000 mdb_connect_pkg-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 02:47:02.641506 mdb_connect_pkg-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 02:47:02.641506 mdb_connect_pkg-0.0.6/src/mdb_connect_pkg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 02:46:41.000000 mdb_connect_pkg-0.0.6/src/mdb_connect_pkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-31 02:46:41.000000 mdb_connect_pkg-0.0.6/src/mdb_connect_pkg/mongo_crud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 02:47:02.645506 mdb_connect_pkg-0.0.6/src/mdb_connect_pkg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-31 02:47:02.000000 mdb_connect_pkg-0.0.6/src/mdb_connect_pkg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-31 02:47:02.000000 mdb_connect_pkg-0.0.6/src/mdb_connect_pkg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 02:47:02.000000 mdb_connect_pkg-0.0.6/src/mdb_connect_pkg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-31 02:47:02.000000 mdb_connect_pkg-0.0.6/src/mdb_connect_pkg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 02:47:02.000000 mdb_connect_pkg-0.0.6/src/mdb_connect_pkg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:19:20.124486 mdb_connect_pkg-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-31 03:19:00.000000 mdb_connect_pkg-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-05-31 03:19:20.124486 mdb_connect_pkg-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-31 03:19:00.000000 mdb_connect_pkg-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-31 03:19:00.000000 mdb_connect_pkg-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-31 03:19:20.124486 mdb_connect_pkg-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-31 03:19:00.000000 mdb_connect_pkg-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:19:20.120486 mdb_connect_pkg-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:19:20.120486 mdb_connect_pkg-1.0.0/src/mdb_connect_pkg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:19:00.000000 mdb_connect_pkg-1.0.0/src/mdb_connect_pkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-31 03:19:00.000000 mdb_connect_pkg-1.0.0/src/mdb_connect_pkg/mongo_crud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:19:20.124486 mdb_connect_pkg-1.0.0/src/mdb_connect_pkg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-05-31 03:19:20.000000 mdb_connect_pkg-1.0.0/src/mdb_connect_pkg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-31 03:19:20.000000 mdb_connect_pkg-1.0.0/src/mdb_connect_pkg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 03:19:20.000000 mdb_connect_pkg-1.0.0/src/mdb_connect_pkg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-31 03:19:20.000000 mdb_connect_pkg-1.0.0/src/mdb_connect_pkg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 03:19:20.000000 mdb_connect_pkg-1.0.0/src/mdb_connect_pkg.egg-info/top_level.txt
```

### Comparing `mdb_connect_pkg-0.0.6/LICENSE` & `mdb_connect_pkg-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mdb_connect_pkg-0.0.6/PKG-INFO` & `mdb_connect_pkg-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdb_connect_pkg
-Version: 0.0.6
+Version: 1.0.0
 Summary: A python package for connecting with database.
 Home-page: https://github.com/yuvaneshkm/mongodb-connector-pkg
 Author: yuvaneshkm
 Author-email: yuvaneshkm27@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yuvaneshkm/mongodb-connector-pkg/issues
 Classifier: Programming Language :: Python :: 3.8
@@ -169,9 +169,29 @@
 .. code-block:: python
 
     mongo.drop_collection()
 
 To delete the entire database:
 
 .. code-block:: python
-    
+
     mongo.drop_database()
+
+Contributing
+------------
+
+Contributions are welcome! Please open an issue or submit a pull request on GitHub.
+
+License
+-------
+
+This project is licensed under the MIT License.
+
+Contact
+-------
+
+For any questions or suggestions, please contact `yuvaneshkm05@gmail.com <mailto:yuvaneshkm05@gmail.com>`_
+
+Connect
+-------
+
+Connect with me on `LinkedIn <https://www.linkedin.com/in/yuvaneshkm>`_
```

### Comparing `mdb_connect_pkg-0.0.6/README.rst` & `mdb_connect_pkg-1.0.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -139,9 +139,29 @@
 .. code-block:: python
 
     mongo.drop_collection()
 
 To delete the entire database:
 
 .. code-block:: python
-    
-    mongo.drop_database()
+
+    mongo.drop_database()
+
+Contributing
+------------
+
+Contributions are welcome! Please open an issue or submit a pull request on GitHub.
+
+License
+-------
+
+This project is licensed under the MIT License.
+
+Contact
+-------
+
+For any questions or suggestions, please contact `yuvaneshkm05@gmail.com <mailto:yuvaneshkm05@gmail.com>`_
+
+Connect
+-------
+
+Connect with me on `LinkedIn <https://www.linkedin.com/in/yuvaneshkm>`_
```

### Comparing `mdb_connect_pkg-0.0.6/setup.cfg` & `mdb_connect_pkg-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mdb_connect_pkg-0.0.6/setup.py` & `mdb_connect_pkg-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import warnings
 warnings.filterwarnings('ignore')
 
 # ==================================== Setup ===============================================
 
 # basic info:
 PKG_NAME= "mdb_connect_pkg"
-__version__ = "0.0.6"
+__version__ = "1.0.0"
 AUTHOR_USER_NAME = "yuvaneshkm"
 REPO_NAME = "mongodb-connector-pkg"
 AUTHOR_EMAIL = "yuvaneshkm27@gmail.com"
 
 # long description:
 def read_file(filename):
     with open(filename, 'r', encoding='utf-8') as f:
```

### Comparing `mdb_connect_pkg-0.0.6/src/mdb_connect_pkg/mongo_crud.py` & `mdb_connect_pkg-1.0.0/src/mdb_connect_pkg/mongo_crud.py`

 * *Files identical despite different names*

### Comparing `mdb_connect_pkg-0.0.6/src/mdb_connect_pkg.egg-info/PKG-INFO` & `mdb_connect_pkg-1.0.0/src/mdb_connect_pkg.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdb_connect_pkg
-Version: 0.0.6
+Version: 1.0.0
 Summary: A python package for connecting with database.
 Home-page: https://github.com/yuvaneshkm/mongodb-connector-pkg
 Author: yuvaneshkm
 Author-email: yuvaneshkm27@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yuvaneshkm/mongodb-connector-pkg/issues
 Classifier: Programming Language :: Python :: 3.8
@@ -169,9 +169,29 @@
 .. code-block:: python
 
     mongo.drop_collection()
 
 To delete the entire database:
 
 .. code-block:: python
-    
+
     mongo.drop_database()
+
+Contributing
+------------
+
+Contributions are welcome! Please open an issue or submit a pull request on GitHub.
+
+License
+-------
+
+This project is licensed under the MIT License.
+
+Contact
+-------
+
+For any questions or suggestions, please contact `yuvaneshkm05@gmail.com <mailto:yuvaneshkm05@gmail.com>`_
+
+Connect
+-------
+
+Connect with me on `LinkedIn <https://www.linkedin.com/in/yuvaneshkm>`_
```

