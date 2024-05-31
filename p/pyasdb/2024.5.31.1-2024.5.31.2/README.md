# Comparing `tmp/pyasdb-2024.5.31.1.tar.gz` & `tmp/pyasdb-2024.5.31.2.tar.gz`

## Comparing `pyasdb-2024.5.31.1.tar` & `pyasdb-2024.5.31.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.1/src/pyasdb/__init__.py
--rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.1/src/pyasdb/pyasdb.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.1/LICENSE
--rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.1/README.md
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.1/pyproject.toml
--rw-r--r--   0        0        0    48543 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.1/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.2/src/pyasdb/__init__.py
+-rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.2/src/pyasdb/pyasdb.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.2/LICENSE
+-rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.2/README.md
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.2/pyproject.toml
+-rw-r--r--   0        0        0    48543 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.2/PKG-INFO
```

### Comparing `pyasdb-2024.5.31.1/src/pyasdb/pyasdb.py` & `pyasdb-2024.5.31.2/src/pyasdb/pyasdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import shelve
-
+import atexit
 
 class Query:
     """
     Query Class For Making And Managing Results of Queries.
 
     """
     def __init__(self, table, results):
@@ -203,7 +203,12 @@
     def __next__(self):
         if self.index == len(self.__keycache):
             raise StopIteration
         else:
             x = self[self.__keycache[self.index]]
             self.index += 1
             return x
+
+    @atexit.register
+    def close(self):
+        self.sync()
+        self.shelf.close()
```

### Comparing `pyasdb-2024.5.31.1/LICENSE` & `pyasdb-2024.5.31.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyasdb-2024.5.31.1/README.md` & `pyasdb-2024.5.31.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 I kept using SQLite for local databases and too often it was overkill. Inflexible and too much work to maintain for it's
 benefit, even when using an abstraction.
 
 The goal with PYASDB (I pronounce it Py-As-DB) is to be a barebones simple no-sql, unstructured local database.
 
 While I try to optimize it's performance, it's probably less efficient than sqlite as the size of the data increases.
 
-As a side benefit of it's simplicity: the only import (at the time of writing) is the internal library shelve.
+Additionally this is built using only internal libraries, meaning no dependencies should need to be installed.
 
 Disclaimer: Due to it's use of shelve which is backed further by pickle, this is not advisable to load untrusted
 databases.
 
 ### Quickstart
 
 ```python
@@ -62,16 +62,16 @@
 - [ ] Convenience queries (ie. dedicated functions for =, <, >, != to cut down on repetitive lambdas)
 - [ ] SUM and similar
 - [x] Query Type Checking (to prevent TypeError if field has been assigned different types)
 - [ ] Subfield queries (your lambda can reference subfields, but the query function doesn't check to make sure they 
 exist)
 - [ ] Key type agnosticism (the key in the backend must be a string, but it can be handy to just str() all keys to allow
 different types)
-- [ ] Convert to package (and upload to pip)
-- [ ] Add help() data
+- [x] Available on PyPi (pip install pyasdb)
+- [x] Add help() data
 - [ ] Add thread safety
 
 ### PyDoc
 ```
 Python Library Documentation: module pyasdb
 
 NAME
```

### Comparing `pyasdb-2024.5.31.1/pyproject.toml` & `pyasdb-2024.5.31.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyasdb"
-version = "2024.05.31.1"
+version = "2024.05.31.2"
 authors = [
   { name="Shiri Bailem", email="shiri@bailem.me" },
 ]
 description = "A simplified NoSQL offline database built on top of shelve/pickle"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["database", "offline", "NoSQL"]
```

### Comparing `pyasdb-2024.5.31.1/PKG-INFO` & `pyasdb-2024.5.31.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyasdb
-Version: 2024.5.31.1
+Version: 2024.5.31.2
 Summary: A simplified NoSQL offline database built on top of shelve/pickle
 Project-URL: Homepage, https://github.com/shiribailem/pyasdb
 Project-URL: Issues, https://github.com/shiribailem/pyasdb/issues
 Author-email: Shiri Bailem <shiri@bailem.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -693,15 +693,15 @@
 I kept using SQLite for local databases and too often it was overkill. Inflexible and too much work to maintain for it's
 benefit, even when using an abstraction.
 
 The goal with PYASDB (I pronounce it Py-As-DB) is to be a barebones simple no-sql, unstructured local database.
 
 While I try to optimize it's performance, it's probably less efficient than sqlite as the size of the data increases.
 
-As a side benefit of it's simplicity: the only import (at the time of writing) is the internal library shelve.
+Additionally this is built using only internal libraries, meaning no dependencies should need to be installed.
 
 Disclaimer: Due to it's use of shelve which is backed further by pickle, this is not advisable to load untrusted
 databases.
 
 ### Quickstart
 
 ```python
@@ -752,16 +752,16 @@
 - [ ] Convenience queries (ie. dedicated functions for =, <, >, != to cut down on repetitive lambdas)
 - [ ] SUM and similar
 - [x] Query Type Checking (to prevent TypeError if field has been assigned different types)
 - [ ] Subfield queries (your lambda can reference subfields, but the query function doesn't check to make sure they 
 exist)
 - [ ] Key type agnosticism (the key in the backend must be a string, but it can be handy to just str() all keys to allow
 different types)
-- [ ] Convert to package (and upload to pip)
-- [ ] Add help() data
+- [x] Available on PyPi (pip install pyasdb)
+- [x] Add help() data
 - [ ] Add thread safety
 
 ### PyDoc
 ```
 Python Library Documentation: module pyasdb
 
 NAME
```

