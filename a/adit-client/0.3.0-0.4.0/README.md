# Comparing `tmp/adit_client-0.3.0.tar.gz` & `tmp/adit_client-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adit_client-0.3.0.tar", max compression
+gzip compressed data, was "adit_client-0.4.0.tar", max compression
```

## Comparing `adit_client-0.3.0.tar` & `adit_client-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35122 2024-05-27 22:34:48.182611 adit_client-0.3.0/LICENSE
--rw-r--r--   0        0        0      859 2024-05-27 22:34:48.182611 adit_client-0.3.0/README.md
--rw-r--r--   0        0        0       57 2024-05-27 22:34:48.182611 adit_client-0.3.0/adit_client/__init__.py
--rw-r--r--   0        0        0     2488 2024-05-27 23:24:15.289869 adit_client-0.3.0/adit_client/client.py
--rw-r--r--   0        0        0     1701 2024-05-27 23:47:42.803608 adit_client-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1453 1970-01-01 00:00:00.000000 adit_client-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35122 2024-05-27 22:34:48.000000 adit_client-0.4.0/LICENSE
+-rw-r--r--   0        0        0      859 2024-05-27 22:34:48.000000 adit_client-0.4.0/README.md
+-rw-r--r--   0        0        0       57 2024-05-27 22:34:48.000000 adit_client-0.4.0/adit_client/__init__.py
+-rw-r--r--   0        0        0     2833 2024-05-31 14:48:02.000000 adit_client-0.4.0/adit_client/client.py
+-rw-r--r--   0        0        0     1701 2024-05-31 14:48:02.000000 adit_client-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1453 1970-01-01 00:00:00.000000 adit_client-0.4.0/PKG-INFO
```

### Comparing `adit_client-0.3.0/LICENSE` & `adit_client-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adit_client-0.3.0/README.md` & `adit_client-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `adit_client-0.3.0/adit_client/client.py` & `adit_client-0.4.0/adit_client/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from dicomweb_client import DICOMwebClient
+from dicomweb_client import DICOMwebClient, session_utils
 from pydicom import Dataset
 
 
 class AditClient:
-    def __init__(self, server_url: str, auth_token: str) -> None:
+    def __init__(self, server_url: str, auth_token: str, verify: str | bool = True) -> None:
         self.server_url = server_url
         self.auth_token = auth_token
+        self.verify = verify
 
     def search_for_studies(
         self, ae_title: str, query: dict[str, str] | None = None
     ) -> list[Dataset]:
         """Query an ADIT server for studies."""
         results = self._create_dicom_web_client(ae_title).search_for_studies(search_filters=query)
         return [Dataset.from_json(result) for result in results]
@@ -48,14 +49,22 @@
         )
 
     def store_instances(self, ae_title: str, instances: list[Dataset]) -> None:
         """Store some instances on an ADIT server."""
         self._create_dicom_web_client(ae_title).store_instances(instances)
 
     def _create_dicom_web_client(self, ae_title: str) -> DICOMwebClient:
+        session = session_utils.create_session()
+
+        if isinstance(self.verify, bool):
+            session.verify = self.verify
+        else:
+            session = session_utils.add_certs_to_session(session=session, ca_bundle=self.verify)
+
         return DICOMwebClient(
+            session=session,
             url=f"{self.server_url}/api/dicom-web/{ae_title}",
             qido_url_prefix="qidors",
             wado_url_prefix="wadors",
             stow_url_prefix="stowrs",
             headers={"Authorization": f"Token {self.auth_token}"},
         )
```

### Comparing `adit_client-0.3.0/pyproject.toml` & `adit_client-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "adit-client"
-version = "0.3.0"
+version = "0.4.0"
 description = "ADIT Client library to connect to an ADIT server."
 authors = ["Kai Schlamp <kai.schlamp@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{ include = "adit_client" }]
 
 [tool.poetry.dependencies]
```

### Comparing `adit_client-0.3.0/PKG-INFO` & `adit_client-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adit-client
-Version: 0.3.0
+Version: 0.4.0
 Summary: ADIT Client library to connect to an ADIT server.
 License: GPL-3.0-or-later
 Author: Kai Schlamp
 Author-email: kai.schlamp@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

