# Comparing `tmp/contactsoftware_functions_client-0.5.1.tar.gz` & `tmp/contactsoftware_functions_client-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contactsoftware_functions_client-0.5.1.tar", max compression
+gzip compressed data, was "contactsoftware_functions_client-0.5.2.tar", max compression
```

## Comparing `contactsoftware_functions_client-0.5.1.tar` & `contactsoftware_functions_client-0.5.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1078 2024-04-09 13:16:14.496368 contactsoftware_functions_client-0.5.1/LICENSE
--rw-r--r--   0        0        0     1927 2024-04-09 13:16:14.500368 contactsoftware_functions_client-0.5.1/README.md
--rw-r--r--   0        0        0       85 2024-04-09 13:16:14.500368 contactsoftware_functions_client-0.5.1/cfc/__init__.py
--rw-r--r--   0        0        0     2443 2024-04-09 13:16:14.500368 contactsoftware_functions_client-0.5.1/cfc/app.py
--rw-r--r--   0        0        0     1264 2024-04-09 13:16:14.500368 contactsoftware_functions_client-0.5.1/cfc/auth.py
--rw-r--r--   0        0        0     3548 2024-04-09 13:47:16.015817 contactsoftware_functions_client-0.5.1/cfc/config.py
--rw-r--r--   0        0        0     6807 2024-04-09 13:16:14.500368 contactsoftware_functions_client-0.5.1/cfc/environment.py
--rw-r--r--   0        0        0      622 2024-04-09 13:47:27.664183 contactsoftware_functions_client-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2788 1970-01-01 00:00:00.000000 contactsoftware_functions_client-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-31 07:45:51.390947 contactsoftware_functions_client-0.5.2/LICENSE
+-rw-r--r--   0        0        0     1927 2024-05-31 07:45:51.390947 contactsoftware_functions_client-0.5.2/README.md
+-rw-r--r--   0        0        0       85 2024-05-31 07:45:51.390947 contactsoftware_functions_client-0.5.2/cfc/__init__.py
+-rw-r--r--   0        0        0     2443 2024-05-31 07:45:51.390947 contactsoftware_functions_client-0.5.2/cfc/app.py
+-rw-r--r--   0        0        0     1264 2024-05-31 07:45:51.390947 contactsoftware_functions_client-0.5.2/cfc/auth.py
+-rw-r--r--   0        0        0     3548 2024-05-31 07:45:51.390947 contactsoftware_functions_client-0.5.2/cfc/config.py
+-rw-r--r--   0        0        0     6926 2024-05-31 07:45:51.390947 contactsoftware_functions_client-0.5.2/cfc/environment.py
+-rw-r--r--   0        0        0      622 2024-05-31 07:45:51.390947 contactsoftware_functions_client-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2788 1970-01-01 00:00:00.000000 contactsoftware_functions_client-0.5.2/PKG-INFO
```

### Comparing `contactsoftware_functions_client-0.5.1/LICENSE` & `contactsoftware_functions_client-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions_client-0.5.1/README.md` & `contactsoftware_functions_client-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions_client-0.5.1/cfc/app.py` & `contactsoftware_functions_client-0.5.2/cfc/app.py`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions_client-0.5.1/cfc/auth.py` & `contactsoftware_functions_client-0.5.2/cfc/auth.py`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions_client-0.5.1/cfc/config.py` & `contactsoftware_functions_client-0.5.2/cfc/config.py`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions_client-0.5.1/cfc/environment.py` & `contactsoftware_functions_client-0.5.2/cfc/environment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import re
 import sys
 import tarfile
+from json import JSONDecodeError
 from time import sleep
 
 import requests
 import typer
 from rich.console import Console
 from rich.table import Table
 
@@ -63,17 +64,19 @@
         headers={"Authorization": f"Bearer {config.access_token}"},
     )
 
     if response.status_code == 201:
         console.print("Environment successfully created")
 
     elif response.status_code in (400, 500):
-        console.print(
-            "Error while creating environment: " + response.json()["detail"]["msg"]
-        )
+        try:
+            message = response.json().get("detail")
+        except JSONDecodeError:
+            message = response.text
+        console.print("Error while creating environment: " + message)
         raise typer.Exit(code=1)
 
     else:
         console.print("Unknown error while creating environment")
         raise typer.Exit(code=1)
```

### Comparing `contactsoftware_functions_client-0.5.1/pyproject.toml` & `contactsoftware_functions_client-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "contactsoftware-functions-client"
-version = "0.5.1"
+version = "0.5.2"
 readme = "README.md"
 license = "MIT"
 authors = [
     "Jens Kürten <jku@contact.de>",
     "Julian Alberts <jal@contact.de>"
 ]
 description = "Client for uploading and managing Functions in CIM Database Cloud."
```

### Comparing `contactsoftware_functions_client-0.5.1/PKG-INFO` & `contactsoftware_functions_client-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contactsoftware-functions-client
-Version: 0.5.1
+Version: 0.5.2
 Summary: Client for uploading and managing Functions in CIM Database Cloud.
 License: MIT
 Author: Jens Kürten
 Author-email: jku@contact.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: contactsoftware-functions-client Version: 0.5.1
+Metadata-Version: 2.1 Name: contactsoftware-functions-client Version: 0.5.2
 Summary: Client for uploading and managing Functions in CIM Database Cloud.
 License: MIT Author: Jens KÃ¼rten Author-email: jku@contact.de Requires-Python:
 >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: PyYAML (>=6.0,<7.0) Requires-Dist: appdirs
```

