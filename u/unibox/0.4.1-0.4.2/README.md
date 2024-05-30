# Comparing `tmp/unibox-0.4.1.tar.gz` & `tmp/unibox-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unibox-0.4.1.tar", max compression
+gzip compressed data, was "unibox-0.4.2.tar", max compression
```

## Comparing `unibox-0.4.1.tar` & `unibox-0.4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1061 2024-05-20 01:53:31.357326 unibox-0.4.1/LICENSE
--rw-r--r--   0        0        0     4329 2024-05-20 01:53:31.361326 unibox-0.4.1/README.md
--rw-r--r--   0        0        0      629 2024-05-20 01:53:31.361326 unibox-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     4353 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/__init__.py
--rw-r--r--   0        0        0     5428 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/cli.py
--rw-r--r--   0        0        0        0 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/processing/__init__.py
--rw-r--r--   0        0        0     3051 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/processing/file_mover.py
--rw-r--r--   0        0        0     2149 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/processing/file_renamer.py
--rw-r--r--   0        0        0     7196 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/processing/image_resizer.py
--rw-r--r--   0        0        0        0 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/utils/__init__.py
--rw-r--r--   0        0        0      244 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/utils/constants.py
--rw-r--r--   0        0        0     6415 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/utils/s3_client.py
--rw-r--r--   0        0        0     6788 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/utils/uni_loader.py
--rw-r--r--   0        0        0     4279 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/utils/uni_logger.py
--rw-r--r--   0        0        0     3139 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/utils/uni_merger.py
--rw-r--r--   0        0        0     4377 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/utils/uni_peeker.py
--rw-r--r--   0        0        0     8327 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/utils/uni_resizer.py
--rw-r--r--   0        0        0     5387 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/utils/uni_saver.py
--rw-r--r--   0        0        0     5885 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/utils/uni_traverser.py
--rw-r--r--   0        0        0      580 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/utils/utils.py
--rw-r--r--   0        0        0     5442 1970-01-01 00:00:00.000000 unibox-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-30 22:44:01.279500 unibox-0.4.2/LICENSE
+-rw-r--r--   0        0        0     4329 2024-05-30 22:44:01.279500 unibox-0.4.2/README.md
+-rw-r--r--   0        0        0      629 2024-05-30 22:44:01.283500 unibox-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     4394 2024-05-30 22:44:01.283500 unibox-0.4.2/unibox/__init__.py
+-rw-r--r--   0        0        0     5428 2024-05-30 22:44:01.283500 unibox-0.4.2/unibox/cli.py
+-rw-r--r--   0        0        0        0 2024-05-30 22:44:01.283500 unibox-0.4.2/unibox/processing/__init__.py
+-rw-r--r--   0        0        0     3051 2024-05-30 22:44:01.283500 unibox-0.4.2/unibox/processing/file_mover.py
+-rw-r--r--   0        0        0     2149 2024-05-30 22:44:01.283500 unibox-0.4.2/unibox/processing/file_renamer.py
+-rw-r--r--   0        0        0     7196 2024-05-30 22:44:01.283500 unibox-0.4.2/unibox/processing/image_resizer.py
+-rw-r--r--   0        0        0        0 2024-05-30 22:44:01.283500 unibox-0.4.2/unibox/utils/__init__.py
+-rw-r--r--   0        0        0      244 2024-05-30 22:44:01.283500 unibox-0.4.2/unibox/utils/constants.py
+-rw-r--r--   0        0        0     6417 2024-05-30 22:44:01.283500 unibox-0.4.2/unibox/utils/s3_client.py
+-rw-r--r--   0        0        0     6788 2024-05-30 22:44:01.283500 unibox-0.4.2/unibox/utils/uni_loader.py
+-rw-r--r--   0        0        0     4279 2024-05-30 22:44:01.283500 unibox-0.4.2/unibox/utils/uni_logger.py
+-rw-r--r--   0        0        0     3139 2024-05-30 22:44:01.283500 unibox-0.4.2/unibox/utils/uni_merger.py
+-rw-r--r--   0        0        0     4377 2024-05-30 22:44:01.283500 unibox-0.4.2/unibox/utils/uni_peeker.py
+-rw-r--r--   0        0        0     8327 2024-05-30 22:44:01.283500 unibox-0.4.2/unibox/utils/uni_resizer.py
+-rw-r--r--   0        0        0     5387 2024-05-30 22:44:01.283500 unibox-0.4.2/unibox/utils/uni_saver.py
+-rw-r--r--   0        0        0     5867 2024-05-30 22:44:01.283500 unibox-0.4.2/unibox/utils/uni_traverser.py
+-rw-r--r--   0        0        0      580 2024-05-30 22:44:01.283500 unibox-0.4.2/unibox/utils/utils.py
+-rw-r--r--   0        0        0     5442 1970-01-01 00:00:00.000000 unibox-0.4.2/PKG-INFO
```

### Comparing `unibox-0.4.1/LICENSE` & `unibox-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unibox-0.4.1/README.md` & `unibox-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `unibox-0.4.1/pyproject.toml` & `unibox-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unibox"
-version = "0.4.1"
+version = "0.4.2"
 description = "Unibox provides unified interface for common file operations."
 authors = ["yada <trojblue@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/trojblue/unibox"
 
 [tool.poetry.dependencies]
```

### Comparing `unibox-0.4.1/unibox/__init__.py` & `unibox-0.4.2/unibox/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     >>> json_dict_list = unibox.loads("data.jsonl")
     >>> pil_iimage = unibox.loads("image.png")
     """
     loader = UniLoader(debug_print=debug_print)
     return loader.loads(file_path)
 
 
-def saves(data: Any, file_path: Path | str) -> None:
+def saves(data: Any, file_path: Path | str, debug_print=True) -> None:
     """
     Saves arbitrary data to the given file path, using the UniSaver.saves() method.
     :param data: The data to saves.
     :param file_path: Path to the file to saves.
 
     example:
     >>> json_dict = {"name": "John", "age": 30}
@@ -45,15 +45,15 @@
     >>> json_dict_list = [{"name": "John", "age": 30}, {"name": "Doe", "age": 40}]
     >>> unibox.saves(json_dict_list, "data.jsonl")
     >>> df = pd.DataFrame({'A': [1, 2], 'B': [3, 4]})
     >>> unibox.saves(df, "data.parquet")
     >>> pil_image = Image.new('RGB', (60, 30), color='red')
     >>> unibox.saves(pil_image, "image.png")
     """
-    saver = UniSaver()
+    saver = UniSaver(debug_print=debug_print)
     saver.saves(data, file_path)
 
 
 def traverses(root_dir: str, include_extensions: List[str] = None,
               exclude_extensions: List[str] = None, relative_unix=False, debug_print=True) -> List[str]:
     """
```

### Comparing `unibox-0.4.1/unibox/cli.py` & `unibox-0.4.2/unibox/cli.py`

 * *Files identical despite different names*

### Comparing `unibox-0.4.1/unibox/processing/file_mover.py` & `unibox-0.4.2/unibox/processing/file_mover.py`

 * *Files identical despite different names*

### Comparing `unibox-0.4.1/unibox/processing/file_renamer.py` & `unibox-0.4.2/unibox/processing/file_renamer.py`

 * *Files identical despite different names*

### Comparing `unibox-0.4.1/unibox/processing/image_resizer.py` & `unibox-0.4.2/unibox/processing/image_resizer.py`

 * *Files identical despite different names*

### Comparing `unibox-0.4.1/unibox/utils/s3_client.py` & `unibox-0.4.2/unibox/utils/s3_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,20 +112,20 @@
                     "etag": obj["ETag"],
                     "storage_class": obj["StorageClass"],
                 }
 
     def traverse(self, s3_uri, include_extensions=None, exclude_extensions=None, 
                  relative_unix=False, debug_print=True):
         """
-        traverse through a s3 directory and returns direct entries (folder or file) under the directory
+        Traverse through a s3 directory and return direct entries (folder or file) under the directory.
 
         :param include_extensions: list of extensions to include (e.g. ['.jpg', '.png']), defaults to everything
         :param exclude_extensions: list of extensions to exclude (e.g. ['.txt', '.json']), defaults to nothing
         :param relative_unix: whether to give a relative path (relative to bucket) or not 
-        :param debug_print: whether to print debug statuses (eg. tqdm bar) or not
+        :param debug_print: whether to print debug statuses (e.g., tqdm bar) or not
         """
         bucket, prefix = parse_s3_url(s3_uri)
 
         if not prefix.endswith('/'):
             prefix += '/'
 
         paginator = self.s3.get_paginator("list_objects_v2")
@@ -144,23 +144,19 @@
                 all_entries.append(dir_entry)
 
             # Add files to the list, applying filters if specified
             for obj in page.get('Contents', []):
                 file_key = obj["Key"]
                 if file_key == prefix:  # Skip the input directory itself
                     continue
-                _, ext = os.path.splitext(file_key)
-                if include_extensions and ext not in include_extensions:
-                    continue
-                if exclude_extensions and ext in exclude_extensions:
-                    continue
-
-                file_entry = file_key[len(prefix):] if relative_unix else f"s3://{bucket}/{file_key}"
-                all_entries.append(file_entry)
-
+                
+                if (include_extensions is None or any(file_key.endswith(ext) for ext in include_extensions)) and \
+                   (exclude_extensions is None or not any(file_key.endswith(ext) for ext in exclude_extensions)):
+                    file_entry = file_key[len(prefix):] if relative_unix else f"s3://{bucket}/{file_key}"
+                    all_entries.append(file_entry)
 
         return all_entries
 
 
 if __name__ == '__main__':
     client = S3Client()
     # s3_uri = "s3://dataset-artstation-uw2/artists/_angelaramos_/"
```

### Comparing `unibox-0.4.1/unibox/utils/uni_loader.py` & `unibox-0.4.2/unibox/utils/uni_loader.py`

 * *Files identical despite different names*

### Comparing `unibox-0.4.1/unibox/utils/uni_logger.py` & `unibox-0.4.2/unibox/utils/uni_logger.py`

 * *Files identical despite different names*

### Comparing `unibox-0.4.1/unibox/utils/uni_merger.py` & `unibox-0.4.2/unibox/utils/uni_merger.py`

 * *Files identical despite different names*

### Comparing `unibox-0.4.1/unibox/utils/uni_peeker.py` & `unibox-0.4.2/unibox/utils/uni_peeker.py`

 * *Files identical despite different names*

### Comparing `unibox-0.4.1/unibox/utils/uni_resizer.py` & `unibox-0.4.2/unibox/utils/uni_resizer.py`

 * *Files identical despite different names*

### Comparing `unibox-0.4.1/unibox/utils/uni_saver.py` & `unibox-0.4.2/unibox/utils/uni_saver.py`

 * *Files identical despite different names*

### Comparing `unibox-0.4.1/unibox/utils/uni_traverser.py` & `unibox-0.4.2/unibox/utils/uni_traverser.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,16 @@
         self.post_process = post_process
         self.error_handler = error_handler
         self.traversed_files = []
 
     def _files_to_traverse(self):
         for root, _, files in os.walk(self.root_dir):
             for file_name in files:
-                extension = os.path.splitext(file_name)[1].lower()
-                if (self.include_extensions is None or extension in self.include_extensions) and \
-                        (self.exclude_extensions is None or extension not in self.exclude_extensions):
+                if (self.include_extensions is None or any(file_name.endswith(ext) for ext in self.include_extensions)) and \
+                   (self.exclude_extensions is None or not any(file_name.endswith(ext) for ext in self.exclude_extensions)):
                     yield os.path.join(root, file_name)
 
     def traverse(self, file_handler: Callable[[str], None] = None, debug_print: bool = True) -> None:
         """
         Traverses the directory tree and applies the given file handler to each file.
 
         Args:
```

### Comparing `unibox-0.4.1/unibox/utils/utils.py` & `unibox-0.4.2/unibox/utils/utils.py`

 * *Files identical despite different names*

### Comparing `unibox-0.4.1/PKG-INFO` & `unibox-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unibox
-Version: 0.4.1
+Version: 0.4.2
 Summary: Unibox provides unified interface for common file operations.
 Home-page: https://github.com/trojblue/unibox
 License: MIT
 Author: yada
 Author-email: trojblue@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

