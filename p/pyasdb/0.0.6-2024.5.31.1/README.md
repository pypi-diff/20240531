# Comparing `tmp/pyasdb-0.0.6.tar.gz` & `tmp/pyasdb-2024.5.31.1.tar.gz`

## Comparing `pyasdb-0.0.6.tar` & `pyasdb-2024.5.31.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pyasdb-0.0.6/src/pyasdb/__init__.py
--rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 pyasdb-0.0.6/src/pyasdb/pyasdb.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyasdb-0.0.6/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pyasdb-0.0.6/LICENSE
--rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 pyasdb-0.0.6/README.md
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 pyasdb-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    48537 2020-02-02 00:00:00.000000 pyasdb-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.1/src/pyasdb/__init__.py
+-rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.1/src/pyasdb/pyasdb.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.1/LICENSE
+-rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.1/README.md
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.1/pyproject.toml
+-rw-r--r--   0        0        0    48543 2020-02-02 00:00:00.000000 pyasdb-2024.5.31.1/PKG-INFO
```

### Comparing `pyasdb-0.0.6/src/pyasdb/pyasdb.py` & `pyasdb-2024.5.31.1/src/pyasdb/pyasdb.py`

 * *Files identical despite different names*

### Comparing `pyasdb-0.0.6/LICENSE` & `pyasdb-2024.5.31.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyasdb-0.0.6/README.md` & `pyasdb-2024.5.31.1/README.md`

 * *Files identical despite different names*

### Comparing `pyasdb-0.0.6/pyproject.toml` & `pyasdb-2024.5.31.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyasdb"
-version = "0.0.6"
+version = "2024.05.31.1"
 authors = [
   { name="Shiri Bailem", email="shiri@bailem.me" },
 ]
 description = "A simplified NoSQL offline database built on top of shelve/pickle"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["database", "offline", "NoSQL"]
```

### Comparing `pyasdb-0.0.6/PKG-INFO` & `pyasdb-2024.5.31.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyasdb
-Version: 0.0.6
+Version: 2024.5.31.1
 Summary: A simplified NoSQL offline database built on top of shelve/pickle
 Project-URL: Homepage, https://github.com/shiribailem/pyasdb
 Project-URL: Issues, https://github.com/shiribailem/pyasdb/issues
 Author-email: Shiri Bailem <shiri@bailem.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

