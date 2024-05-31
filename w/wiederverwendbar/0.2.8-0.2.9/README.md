# Comparing `tmp/wiederverwendbar-0.2.8.tar.gz` & `tmp/wiederverwendbar-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiederverwendbar-0.2.8.tar", last modified: Thu May 30 11:23:36 2024, max compression
+gzip compressed data, was "wiederverwendbar-0.2.9.tar", last modified: Thu May 30 12:03:51 2024, max compression
```

## Comparing `wiederverwendbar-0.2.8.tar` & `wiederverwendbar-0.2.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       19 2024-05-30 11:22:35.039636 wiederverwendbar-0.2.8/README.md
--rw-r--r--   0        0        0      763 2024-05-30 11:23:36.474497 wiederverwendbar-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      156 2024-05-30 11:22:35.039636 wiederverwendbar-0.2.8/src/wiederverwendbar/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 11:22:35.039636 wiederverwendbar-0.2.8/src/wiederverwendbar/functions/__init__.py
--rw-r--r--   0        0        0     1113 2024-05-30 11:22:35.039636 wiederverwendbar-0.2.8/src/wiederverwendbar/functions/admin.py
--rw-r--r--   0        0        0     1734 2024-05-30 11:22:35.039636 wiederverwendbar-0.2.8/src/wiederverwendbar/functions/eval_file.py
--rw-r--r--   0        0        0     3174 2024-05-30 11:22:35.039636 wiederverwendbar-0.2.8/src/wiederverwendbar/functions/eval_value.py
--rw-r--r--   0        0        0      407 2024-05-30 11:22:35.039636 wiederverwendbar-0.2.8/src/wiederverwendbar/functions/find_class_method.py
--rw-r--r--   0        0        0     1162 2024-05-30 11:22:35.039636 wiederverwendbar-0.2.8/src/wiederverwendbar/functions/wait_ping.py
--rw-r--r--   0        0        0      186 2024-05-30 11:22:35.039636 wiederverwendbar-0.2.8/src/wiederverwendbar/logger/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 11:22:35.039636 wiederverwendbar-0.2.8/src/wiederverwendbar/logger/handlers/__init__.py
--rw-r--r--   0        0        0      600 2024-05-30 11:22:35.039636 wiederverwendbar-0.2.8/src/wiederverwendbar/logger/handlers/rich_console_handler.py
--rw-r--r--   0        0        0      624 2024-05-30 11:22:35.039636 wiederverwendbar-0.2.8/src/wiederverwendbar/logger/handlers/stream_console_handler.py
--rw-r--r--   0        0        0     2378 2024-05-30 11:22:35.039636 wiederverwendbar-0.2.8/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py
--rw-r--r--   0        0        0     3036 2024-05-30 11:22:35.039636 wiederverwendbar-0.2.8/src/wiederverwendbar/logger/logger.py
--rw-r--r--   0        0        0     5665 2024-05-30 11:22:35.043637 wiederverwendbar-0.2.8/src/wiederverwendbar/logger/logger_settings.py
--rw-r--r--   0        0        0     2375 2024-05-30 11:22:35.043637 wiederverwendbar-0.2.8/src/wiederverwendbar/logger/logger_singleton.py
--rw-r--r--   0        0        0        0 2024-05-30 11:22:35.043637 wiederverwendbar-0.2.8/src/wiederverwendbar/mongoengine/__init__.py
--rw-r--r--   0        0        0     3982 2024-05-30 11:22:35.043637 wiederverwendbar-0.2.8/src/wiederverwendbar/mongoengine/backup.py
--rw-r--r--   0        0        0        0 2024-05-30 11:22:35.043637 wiederverwendbar-0.2.8/src/wiederverwendbar/mongoengine/fields/__init__.py
--rw-r--r--   0        0        0      453 2024-05-30 11:22:35.043637 wiederverwendbar-0.2.8/src/wiederverwendbar/mongoengine/fields/ipv4_address_field.py
--rw-r--r--   0        0        0      548 2024-05-30 11:22:35.043637 wiederverwendbar-0.2.8/src/wiederverwendbar/mongoengine/property_document.py
--rw-r--r--   0        0        0        0 2024-05-30 11:22:35.043637 wiederverwendbar-0.2.8/src/wiederverwendbar/pydantic/__init__.py
--rw-r--r--   0        0        0     2145 2024-05-30 11:22:35.043637 wiederverwendbar-0.2.8/src/wiederverwendbar/pydantic/file_config.py
--rw-r--r--   0        0        0      762 2024-05-30 11:22:35.043637 wiederverwendbar-0.2.8/src/wiederverwendbar/pydantic/indexable_model.py
--rw-r--r--   0        0        0     7453 2024-05-30 11:22:35.043637 wiederverwendbar-0.2.8/src/wiederverwendbar/singleton.py
--rw-r--r--   0        0        0        0 2024-05-30 11:22:35.043637 wiederverwendbar-0.2.8/tests/__init__.py
--rw-r--r--   0        0        0      890 2024-05-30 11:22:35.043637 wiederverwendbar-0.2.8/tests/logger.py
--rw-r--r--   0        0        0      920 2024-05-30 11:22:35.043637 wiederverwendbar-0.2.8/tests/singletons.py
--rw-r--r--   0        0        0      466 2024-05-30 11:22:35.043637 wiederverwendbar-0.2.8/tests/test.py
--rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 wiederverwendbar-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0       19 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/README.md
+-rw-r--r--   0        0        0      763 2024-05-30 12:03:51.711650 wiederverwendbar-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      156 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/src/wiederverwendbar/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/src/wiederverwendbar/functions/__init__.py
+-rw-r--r--   0        0        0     1113 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/src/wiederverwendbar/functions/admin.py
+-rw-r--r--   0        0        0     1734 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/src/wiederverwendbar/functions/eval_file.py
+-rw-r--r--   0        0        0     3174 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/src/wiederverwendbar/functions/eval_value.py
+-rw-r--r--   0        0        0      407 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/src/wiederverwendbar/functions/find_class_method.py
+-rw-r--r--   0        0        0     1162 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/src/wiederverwendbar/functions/wait_ping.py
+-rw-r--r--   0        0        0      186 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/src/wiederverwendbar/logger/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/src/wiederverwendbar/logger/handlers/__init__.py
+-rw-r--r--   0        0        0      600 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/src/wiederverwendbar/logger/handlers/rich_console_handler.py
+-rw-r--r--   0        0        0      624 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/src/wiederverwendbar/logger/handlers/stream_console_handler.py
+-rw-r--r--   0        0        0     2378 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py
+-rw-r--r--   0        0        0     3036 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/src/wiederverwendbar/logger/logger.py
+-rw-r--r--   0        0        0     5665 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/src/wiederverwendbar/logger/logger_settings.py
+-rw-r--r--   0        0        0     2375 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/src/wiederverwendbar/logger/logger_singleton.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/src/wiederverwendbar/mongoengine/__init__.py
+-rw-r--r--   0        0        0     4598 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/src/wiederverwendbar/mongoengine/backup.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/src/wiederverwendbar/mongoengine/fields/__init__.py
+-rw-r--r--   0        0        0      453 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/src/wiederverwendbar/mongoengine/fields/ipv4_address_field.py
+-rw-r--r--   0        0        0      548 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/src/wiederverwendbar/mongoengine/property_document.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/src/wiederverwendbar/pydantic/__init__.py
+-rw-r--r--   0        0        0     2145 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/src/wiederverwendbar/pydantic/file_config.py
+-rw-r--r--   0        0        0      762 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/src/wiederverwendbar/pydantic/indexable_model.py
+-rw-r--r--   0        0        0     7453 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/src/wiederverwendbar/singleton.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/tests/__init__.py
+-rw-r--r--   0        0        0      890 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/tests/logger.py
+-rw-r--r--   0        0        0      920 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/tests/singletons.py
+-rw-r--r--   0        0        0      466 2024-05-30 12:03:01.103530 wiederverwendbar-0.2.9/tests/test.py
+-rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 wiederverwendbar-0.2.9/PKG-INFO
```

### Comparing `wiederverwendbar-0.2.8/pyproject.toml` & `wiederverwendbar-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 dependencies = [
     "pydantic>=2.7.1",
     "pydantic-settings>=2.2.1",
 ]
 requires-python = ">=3.12"
 readme = "README.md"
-version = "0.2.8"
+version = "0.2.9"
 
 [project.license]
 text = "GPL-3.0"
 
 [project.optional-dependencies]
 rich = [
     "rich>=13.7.1",
```

### Comparing `wiederverwendbar-0.2.8/src/wiederverwendbar/functions/admin.py` & `wiederverwendbar-0.2.9/src/wiederverwendbar/functions/admin.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.8/src/wiederverwendbar/functions/eval_file.py` & `wiederverwendbar-0.2.9/src/wiederverwendbar/functions/eval_file.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.8/src/wiederverwendbar/functions/eval_value.py` & `wiederverwendbar-0.2.9/src/wiederverwendbar/functions/eval_value.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.8/src/wiederverwendbar/functions/wait_ping.py` & `wiederverwendbar-0.2.9/src/wiederverwendbar/functions/wait_ping.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.8/src/wiederverwendbar/logger/handlers/rich_console_handler.py` & `wiederverwendbar-0.2.9/src/wiederverwendbar/logger/handlers/rich_console_handler.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.8/src/wiederverwendbar/logger/handlers/stream_console_handler.py` & `wiederverwendbar-0.2.9/src/wiederverwendbar/logger/handlers/stream_console_handler.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.8/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py` & `wiederverwendbar-0.2.9/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.8/src/wiederverwendbar/logger/logger.py` & `wiederverwendbar-0.2.9/src/wiederverwendbar/logger/logger.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.8/src/wiederverwendbar/logger/logger_settings.py` & `wiederverwendbar-0.2.9/src/wiederverwendbar/logger/logger_settings.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.8/src/wiederverwendbar/logger/logger_singleton.py` & `wiederverwendbar-0.2.9/src/wiederverwendbar/logger/logger_singleton.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.8/src/wiederverwendbar/mongoengine/backup.py` & `wiederverwendbar-0.2.9/src/wiederverwendbar/mongoengine/backup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,69 +5,72 @@
 
 import bson
 from pymongo.database import Database
 
 logger = logging.getLogger(__name__)
 
 
-def dump(db: Database, path: str | Path, overwrite: bool = False, zip: bool = True) -> None:
+def dump(db: Database, path: str | Path, overwrite: bool = False) -> None:
     """
     MongoDB Dump
     :param db: MongoDB database
     :param path: Database dump path
     :param overwrite: Overwrite existing files
-    :param zip: Zip dump
     :return: None
     """
 
     # convert path to Path object
     if type(path) is str:
         path = Path(path)
 
     logger.debug(f"Dumping database to '{path}'")
 
-    if path.is_dir():
+    if path.exists():
         if not overwrite:
             raise FileExistsError(f"Path '{path}' already exists")
-        # remove existing files
-        logger.debug(f"Removing existing files in '{path}'")
-        shutil.rmtree(path)
+        if path.is_file():
+            # remove existing file
+            logger.debug(f"Removing existing file '{path}'")
+            os.remove(path)
+        else:
+            # remove existing files
+            logger.debug(f"Removing existing files in '{path}'")
+            shutil.rmtree(path)
 
     # ensure path dir exists
-    path.mkdir(parents=True, exist_ok=True)
+    path.with_suffix("").mkdir(parents=True, exist_ok=True)
 
     for collection_name in db.list_collection_names():
         logger.debug(f"Dumping collection '{collection_name}'")
 
         # get all documents from collection
         documents_encoded = []
         for document in db[collection_name].find():
             # encode document to bson
             document_encode = bson.BSON.encode(document)
             documents_encoded.append(document_encode)
 
         logger.debug(f"Dumping {len(documents_encoded)} documents")
 
         # create bson file
-        bson_file = path / f'{collection_name}.bson'
+        bson_file = path.with_suffix("") / f'{collection_name}.bson'
         with open(bson_file, 'wb+') as f:
             # write all documents to bson file
             for document_encode in documents_encoded:
                 f.write(document_encode)
 
-    if zip:
+    if path.suffix == ".zip":
         # zip dump
-        zip_file = path.with_suffix(".zip")
-        logger.debug(f"Zipping dump to '{zip_file}'")
-        shutil.make_archive(str(zip_file), 'zip', path)
+        logger.debug(f"Zipping dump '{path.with_suffix("")}' as '{path}'")
+        shutil.make_archive(str(path.with_suffix("")), path.suffix.replace(".", ""), path.with_suffix(""))
         logger.debug("Zipped dump successfully")
 
         # remove bson files
-        logger.debug(f"Removing bson files in '{path}'")
-        shutil.rmtree(path)
+        logger.debug(f"Removing bson files in '{path.with_suffix("")}'")
+        shutil.rmtree(path.with_suffix(""))
 
     logger.debug("Database dumped successfully")
 
 
 def restore(db: Database, path: str | Path, overwrite: bool = False) -> None:
     """
     MongoDB Restore
@@ -81,25 +84,27 @@
     if type(path) is str:
         path = Path(path)
 
     logger.debug(f"Restoring database from '{path}'")
 
     # unzip dump
     if path.suffix == ".zip":
+        if path.with_suffix("").is_dir():
+            logger.debug(f"Removing existing directory '{path.with_suffix("")}'")
+            shutil.rmtree(path.with_suffix(""))
         logger.debug(f"Unzipping dump '{path}'")
         shutil.unpack_archive(path, path.with_suffix(""))
-        path = path.with_suffix("")
         logger.debug("Unzipped dump successfully")
 
     # check if path is a directory
-    if not os.path.isdir(path):
-        raise FileNotFoundError(f"Path '{path}' does not exist")
+    if not os.path.isdir(path.with_suffix("")):
+        raise FileNotFoundError(f"Path '{path.with_suffix("")}' does not exist")
 
-    for bson_file in os.listdir(path):
-        bson_file = path / bson_file
+    for bson_file in os.listdir(path.with_suffix("")):
+        bson_file = path.with_suffix("") / bson_file
 
         # check bson file is a file
         if not os.path.isfile(bson_file):
             continue
 
         # check bson file is a bson file
         if not bson_file.suffix == ".bson":
@@ -125,8 +130,13 @@
             else:
                 raise FileExistsError(f"Collection '{collection_name}' already exists")
 
         # insert documents into collection
         logger.debug(f"Restoring {len(documents)} documents")
         db[collection_name].insert_many(documents)
 
+    # remove bson files
+    if path.suffix == ".zip":
+        logger.debug(f"Removing bson files in '{path.with_suffix("")}'")
+        shutil.rmtree(path.with_suffix(""))
+
     logger.debug("Database restored successfully")
```

### Comparing `wiederverwendbar-0.2.8/src/wiederverwendbar/mongoengine/property_document.py` & `wiederverwendbar-0.2.9/src/wiederverwendbar/mongoengine/property_document.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.8/src/wiederverwendbar/pydantic/file_config.py` & `wiederverwendbar-0.2.9/src/wiederverwendbar/pydantic/file_config.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.8/src/wiederverwendbar/pydantic/indexable_model.py` & `wiederverwendbar-0.2.9/src/wiederverwendbar/pydantic/indexable_model.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.8/src/wiederverwendbar/singleton.py` & `wiederverwendbar-0.2.9/src/wiederverwendbar/singleton.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.8/tests/logger.py` & `wiederverwendbar-0.2.9/tests/logger.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.8/tests/singletons.py` & `wiederverwendbar-0.2.9/tests/singletons.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.8/PKG-INFO` & `wiederverwendbar-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiederverwendbar
-Version: 0.2.8
+Version: 0.2.9
 Summary: A collection of scripts, classes and tools they are "wiederverwendbar".
 Author-Email: Julius Koenig <info@bastelquartier.de>
 License: GPL-3.0
 Requires-Python: >=3.12
 Requires-Dist: pydantic>=2.7.1
 Requires-Dist: pydantic-settings>=2.2.1
 Requires-Dist: rich>=13.7.1; extra == "rich"
```

