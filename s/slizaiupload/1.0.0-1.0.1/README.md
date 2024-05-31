# Comparing `tmp/slizaiupload-1.0.0.tar.gz` & `tmp/slizaiupload-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slizaiupload-1.0.0.tar", max compression
+gzip compressed data, was "slizaiupload-1.0.1.tar", max compression
```

## Comparing `slizaiupload-1.0.0.tar` & `slizaiupload-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1092 2024-05-31 02:54:16.415304 slizaiupload-1.0.0/LICENSE
--rw-r--r--   0        0        0     1006 2024-05-31 03:15:09.971020 slizaiupload-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      371 2024-05-31 02:54:04.108862 slizaiupload-1.0.0/README.md
--rw-r--r--   0        0        0       21 2024-05-31 02:47:02.151584 slizaiupload-1.0.0/slizaiupload/__init__.py
--rw-r--r--   0        0        0     9387 2024-05-31 06:06:58.736384 slizaiupload-1.0.0/slizaiupload/main.py
--rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 slizaiupload-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-05-31 02:54:16.415304 slizaiupload-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1006 2024-05-31 06:26:08.955112 slizaiupload-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      371 2024-05-31 02:54:04.108862 slizaiupload-1.0.1/README.md
+-rw-r--r--   0        0        0       21 2024-05-31 02:47:02.151584 slizaiupload-1.0.1/slizaiupload/__init__.py
+-rw-r--r--   0        0        0     9417 2024-05-31 06:22:33.854134 slizaiupload-1.0.1/slizaiupload/main.py
+-rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 slizaiupload-1.0.1/PKG-INFO
```

### Comparing `slizaiupload-1.0.0/LICENSE` & `slizaiupload-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `slizaiupload-1.0.0/pyproject.toml` & `slizaiupload-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "slizaiupload"
-version = "1.0.0"
+version = "1.0.1"
 description = "A tool to upload folders with multipart upload."
 authors = ["Victor Duong <victor.duong@lizai.co>"]
 homepage = "https://lizai.co"
 readme = ["README.md", "LICENSE"]
 
 [project]
 name = "slizaiupload"
-version = "1.0.0"
+version = "1.0.1"
 description = "A tool to upload folders with multipart upload."
 authors = [{ name = "Victor Duong", email = "victor.duong@lizai.co" }]
 homepage = "https://lizai.co"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `slizaiupload-1.0.0/slizaiupload/main.py` & `slizaiupload-1.0.1/slizaiupload/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,9 +214,10 @@
         asyncio.run(upload_folder(api_url, version, folder_path, include_folder, parent_folder_name))
     except Exception as e:
         print("An error occurred during the upload process:", str(e))
 
 if __name__ == "__main__":
     try:
         main()
+        print("Upload Done")
     except Exception as e:
         print("Error occurred:", str(e))
```

### Comparing `slizaiupload-1.0.0/PKG-INFO` & `slizaiupload-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slizaiupload
-Version: 1.0.0
+Version: 1.0.1
 Summary: A tool to upload folders with multipart upload.
 Home-page: https://lizai.co
 Author: Victor Duong
 Author-email: victor.duong@lizai.co
 Requires-Python: >=3.6
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

