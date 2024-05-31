# Comparing `tmp/fero-2.2.1.tar.gz` & `tmp/fero-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fero-2.2.1.tar", last modified: Tue May 14 19:32:48 2024, max compression
+gzip compressed data, was "fero-2.2.2.tar", last modified: Fri May 31 18:27:35 2024, max compression
```

## Comparing `fero-2.2.1.tar` & `fero-2.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 19:32:48.001696 fero-2.2.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1070 2024-05-14 19:32:22.000000 fero-2.2.1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20013 2024-05-14 19:32:48.001696 fero-2.2.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19117 2024-05-14 19:32:22.000000 fero-2.2.1/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 19:32:48.001696 fero-2.2.1/fero/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-05-14 19:32:22.000000 fero-2.2.1/fero/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    39852 2024-05-14 19:32:22.000000 fero-2.2.1/fero/analysis.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7005 2024-05-14 19:32:22.000000 fero-2.2.1/fero/asset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19497 2024-05-14 19:32:22.000000 fero-2.2.1/fero/client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2475 2024-05-14 19:32:22.000000 fero-2.2.1/fero/common.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9394 2024-05-14 19:32:22.000000 fero-2.2.1/fero/datasource.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2024-05-14 19:32:22.000000 fero-2.2.1/fero/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16444 2024-05-14 19:32:22.000000 fero-2.2.1/fero/process.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1140 2024-05-14 19:32:22.000000 fero-2.2.1/fero/workspace.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 19:32:48.001696 fero-2.2.1/fero.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20013 2024-05-14 19:32:47.000000 fero-2.2.1/fero.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      464 2024-05-14 19:32:47.000000 fero-2.2.1/fero.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-14 19:32:47.000000 fero-2.2.1/fero.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2024-05-14 19:32:47.000000 fero-2.2.1/fero.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2024-05-14 19:32:47.000000 fero-2.2.1/fero.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      280 2024-05-14 19:32:48.005696 fero-2.2.1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1909 2024-05-14 19:32:22.000000 fero-2.2.1/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 19:32:48.001696 fero-2.2.1/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43655 2024-05-14 19:32:22.000000 fero-2.2.1/tests/test_analysis.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10345 2024-05-14 19:32:22.000000 fero-2.2.1/tests/test_asset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12383 2024-05-14 19:32:22.000000 fero-2.2.1/tests/test_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2097 2024-05-14 19:32:22.000000 fero-2.2.1/tests/test_datasource.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8032 2024-05-14 19:32:22.000000 fero-2.2.1/tests/test_process.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6348 2024-05-14 19:32:22.000000 fero-2.2.1/tests/test_unsafe_client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 18:27:35.029709 fero-2.2.2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1070 2024-05-31 18:27:15.000000 fero-2.2.2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20013 2024-05-31 18:27:35.029709 fero-2.2.2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19117 2024-05-31 18:27:15.000000 fero-2.2.2/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 18:27:35.029709 fero-2.2.2/fero/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-05-31 18:27:15.000000 fero-2.2.2/fero/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    39852 2024-05-31 18:27:15.000000 fero-2.2.2/fero/analysis.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7005 2024-05-31 18:27:15.000000 fero-2.2.2/fero/asset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19948 2024-05-31 18:27:15.000000 fero-2.2.2/fero/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2475 2024-05-31 18:27:15.000000 fero-2.2.2/fero/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9394 2024-05-31 18:27:15.000000 fero-2.2.2/fero/datasource.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2024-05-31 18:27:15.000000 fero-2.2.2/fero/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16444 2024-05-31 18:27:15.000000 fero-2.2.2/fero/process.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1140 2024-05-31 18:27:15.000000 fero-2.2.2/fero/workspace.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 18:27:35.029709 fero-2.2.2/fero.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20013 2024-05-31 18:27:34.000000 fero-2.2.2/fero.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      464 2024-05-31 18:27:34.000000 fero-2.2.2/fero.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-31 18:27:34.000000 fero-2.2.2/fero.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2024-05-31 18:27:34.000000 fero-2.2.2/fero.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2024-05-31 18:27:34.000000 fero-2.2.2/fero.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      280 2024-05-31 18:27:35.029709 fero-2.2.2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1909 2024-05-31 18:27:15.000000 fero-2.2.2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 18:27:35.029709 fero-2.2.2/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43655 2024-05-31 18:27:15.000000 fero-2.2.2/tests/test_analysis.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10345 2024-05-31 18:27:15.000000 fero-2.2.2/tests/test_asset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12383 2024-05-31 18:27:15.000000 fero-2.2.2/tests/test_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2097 2024-05-31 18:27:15.000000 fero-2.2.2/tests/test_datasource.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8032 2024-05-31 18:27:15.000000 fero-2.2.2/tests/test_process.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6348 2024-05-31 18:27:15.000000 fero-2.2.2/tests/test_unsafe_client.py
```

### Comparing `fero-2.2.1/LICENSE` & `fero-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fero-2.2.1/PKG-INFO` & `fero-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fero
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python client for accessing Fero API
 Home-page: https://github.com/FeroLabs/fero_client
 Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
 Project-URL: Source, https://github.com/pypa/sampleproject/
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fero-2.2.1/README.md` & `fero-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `fero-2.2.1/fero/analysis.py` & `fero-2.2.2/fero/analysis.py`

 * *Files identical despite different names*

### Comparing `fero-2.2.1/fero/asset.py` & `fero-2.2.2/fero/asset.py`

 * *Files identical despite different names*

### Comparing `fero-2.2.1/fero/client.py` & `fero-2.2.2/fero/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -378,75 +378,98 @@
         backoff.fibo, predicate=lambda ds: ds.status != "R", max_time=600
     )
     def _wait_until_datasource_is_ready(self, ds: DataSource) -> DataSource:
         if ds.status == "R":
             return ds
         return DataSource(self, self.get(f"/api/v2/data_source/{str(ds.uuid)}/"))
 
-    def create_live_datasource(self, ds_name, ds_schema):
+    def _upload_config(
+        self,
+        format_type=None,
+        file_type=None,
+        primary_datetime=None,
+        primary_keys=None,
+    ):
+        # TODO: Get from an endpoint
+        data = {
+            "upload_format_configuration": {
+                "format_type": format_type or "tabular",
+                "file_options": {"kind": file_type or "CsvFileOptions"},
+            }
+        }
+
+        if primary_datetime is not None:
+            data["primary_datetime_col"] = primary_datetime
+        if primary_keys is not None:
+            data["primary_key_col"] = primary_keys
+
+        return data
+
+    def create_live_datasource(
+        self,
+        ds_name,
+        ds_schema,
+        format_type=None,
+        file_type=None,
+        primary_datetime=None,
+        primary_keys=None,
+    ):
         """SCRIPT USE ONLY: Create a live data source."""
         me = self.get("/api/me/")
         upload_ac = me["profile"]["default_upload_ac"]["name"]
+
+        data = {
+            "name": ds_name,
+            "description": "",
+            "access_control": upload_ac,
+            "live_configuration": ds_schema,
+            "default_upload_config": self._upload_config(
+                file_type=file_type,
+                format_type=format_type,
+                primary_datetime=primary_datetime,
+                primary_keys=primary_keys,
+            ),
+        }
+
+        if primary_datetime is not None:
+            data["primary_datetime_column"] = primary_datetime
+
+        if primary_keys is not None:
+            data["primary_keys"] = primary_keys
+
         ds = DataSource(
             self,
-            self.post(
-                "/api/v2/data_source/",
-                {
-                    "name": ds_name,
-                    "description": "",
-                    "access_control": upload_ac,
-                    "live_configuration": ds_schema,
-                    "default_upload_config": {
-                        "upload_format_configuration": {
-                            "format_type": "tabular",
-                            "file_options": {"kind": "CsvFileOptions"},
-                        }
-                    },
-                },
-            ),
+            self.post("/api/v2/data_source/", data),
         )
         return self._wait_until_datasource_is_ready(ds)
 
     def create_datasource_from_file(
         self,
         ds_name: str,
         file_name: str,
         file_schema: Dict[str, Any],
         file: TextIO,
+        file_type: Optional[str] = "CsvFileOptions",
+        format_type: Optional[str] = "tabular",
         overwrites: Optional[Dict[str, Any]] = None,
         primary_datetime: Optional[str] = None,
         primary_keys: Optional[Sequence[str]] = None,
     ) -> DataSource:
         """SCRIPT USE ONLY: Create a data source from a CSV file."""
-
-        def _guess_file_type(file_name):
-            if file_name.lower().endswith(".csv"):
-                return "CsvFileOptions"
-            return "ExcelFileOptions"
-
         data = {
             "name": file_name,
-            "uploaded_data_configuration": {
-                # TODO: Get from an endpoint
-                "upload_format_configuration": {
-                    "format_type": "tabular",
-                    "file_options": {"kind": _guess_file_type(file_name)},
-                }
-            },
+            "uploaded_data_configuration": self._upload_config(
+                file_type=file_type,
+                format_type=format_type,
+                primary_datetime=primary_datetime,
+                primary_keys=primary_keys,
+            ),
             "parsed_schema": file_schema,
         }
 
-        if primary_datetime is not None:
-            data["uploaded_data_configuration"][
-                "primary_datetime_col"
-            ] = primary_datetime
-
-        elif primary_keys is not None:
-            data["uploaded_data_configuration"]["primary_key_col"] = primary_keys
-
         uf_res = self.post(
             "/api/v2/uploaded_files/",
             data,
         )
 
         files_uuid = uf_res["uuid"]
         inbox_response = self.get(
```

### Comparing `fero-2.2.1/fero/common.py` & `fero-2.2.2/fero/common.py`

 * *Files identical despite different names*

### Comparing `fero-2.2.1/fero/datasource.py` & `fero-2.2.2/fero/datasource.py`

 * *Files identical despite different names*

### Comparing `fero-2.2.1/fero/process.py` & `fero-2.2.2/fero/process.py`

 * *Files identical despite different names*

### Comparing `fero-2.2.1/fero/workspace.py` & `fero-2.2.2/fero/workspace.py`

 * *Files identical despite different names*

### Comparing `fero-2.2.1/fero.egg-info/PKG-INFO` & `fero-2.2.2/fero.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fero
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python client for accessing Fero API
 Home-page: https://github.com/FeroLabs/fero_client
 Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
 Project-URL: Source, https://github.com/pypa/sampleproject/
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fero-2.2.1/setup.py` & `fero-2.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup
 from setuptools.command.install import install
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
-VERSION = "2.2.1"
+VERSION = "2.2.2"
 
 
 class VerifyVersionCommand(install):
     """Custom command to verify that the git tag matches our version."""
 
     description = "verify that the git tag matches our version"
```

### Comparing `fero-2.2.1/tests/test_analysis.py` & `fero-2.2.2/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `fero-2.2.1/tests/test_asset.py` & `fero-2.2.2/tests/test_asset.py`

 * *Files identical despite different names*

### Comparing `fero-2.2.1/tests/test_client.py` & `fero-2.2.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `fero-2.2.1/tests/test_datasource.py` & `fero-2.2.2/tests/test_datasource.py`

 * *Files identical despite different names*

### Comparing `fero-2.2.1/tests/test_process.py` & `fero-2.2.2/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `fero-2.2.1/tests/test_unsafe_client.py` & `fero-2.2.2/tests/test_unsafe_client.py`

 * *Files identical despite different names*

