# Comparing `tmp/tdimport_client-0.2.2-py3-none-any.whl.zip` & `tmp/tdimport_client-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4613 bytes, number of entries: 9
--rw-r--r--  2.0 unx      589 b- defN 24-May-28 12:12 tdimport_client/__init__.py
+Zip file size: 4488 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      357 b- defN 24-May-31 11:16 tdimport_client/__init__.py
 -rw-r--r--  2.0 unx     2079 b- defN 22-Nov-23 10:47 tdimport_client/models.py
 -rw-r--r--  2.0 unx     1051 b- defN 22-Nov-23 10:47 tdimport_client/sftp_client.py
 -rw-r--r--  2.0 unx      900 b- defN 22-Nov-23 10:47 tdimport_client/tdimport_client.py
--rw-rw-rw-  2.0 unx      575 b- defN 24-May-28 12:21 tdimport_client-0.2.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      893 b- defN 24-May-28 12:21 tdimport_client-0.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-28 12:21 tdimport_client-0.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 24-May-28 12:21 tdimport_client-0.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      770 b- defN 24-May-28 12:21 tdimport_client-0.2.2.dist-info/RECORD
-9 files, 6965 bytes uncompressed, 3269 bytes compressed:  53.1%
+-rw-rw-rw-  2.0 unx      575 b- defN 24-May-31 11:33 tdimport_client-0.2.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      844 b- defN 24-May-31 11:33 tdimport_client-0.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-31 11:33 tdimport_client-0.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 24-May-31 11:33 tdimport_client-0.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      770 b- defN 24-May-31 11:33 tdimport_client-0.2.3.dist-info/RECORD
+9 files, 6684 bytes uncompressed, 3144 bytes compressed:  53.0%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: tdimport_client/sftp_client.py
 Comment: 
 
 Filename: tdimport_client/tdimport_client.py
 Comment: 
 
-Filename: tdimport_client-0.2.2.dist-info/LICENSE.txt
+Filename: tdimport_client-0.2.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: tdimport_client-0.2.2.dist-info/METADATA
+Filename: tdimport_client-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: tdimport_client-0.2.2.dist-info/WHEEL
+Filename: tdimport_client-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: tdimport_client-0.2.2.dist-info/top_level.txt
+Filename: tdimport_client-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: tdimport_client-0.2.2.dist-info/RECORD
+Filename: tdimport_client-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tdimport_client/__init__.py

```diff
@@ -1,17 +1,12 @@
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 
 __all__ = [
     "TDImportServiceClient",
     "TDBundleUploadSFTPClient",
     "TDBundleImportModel",
     "TDBundleUploadModel",
 ]
 
-try:
-    # Attempts to import the client class
-    # Allowed to fail importing so the package metadata can be read for building
-    from .tdimport_client import TDImportServiceClient  # noqa: F401
-    from .sftp_client import TDBundleUploadSFTPClient  # noqa: F401
-    from .models import TDBundleImportModel, TDBundleUploadModel  # noqa: F401
-except (ImportError, ModuleNotFoundError):  # pragma: no cover
-    pass  # pragma: no cover
+from .tdimport_client import TDImportServiceClient  # noqa: F401
+from .sftp_client import TDBundleUploadSFTPClient  # noqa: F401
+from .models import TDBundleImportModel, TDBundleUploadModel  # noqa: F401
```

## Comparing `tdimport_client-0.2.2.dist-info/LICENSE.txt` & `tdimport_client-0.2.3.dist-info/LICENSE.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2022 IQVIA Ltd
+Copyright 2024 IQVIA Ltd
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
      http://www.apache.org/licenses/LICENSE-2.0
```

## Comparing `tdimport_client-0.2.2.dist-info/METADATA` & `tdimport_client-0.2.3.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
-Name: tdimport-client
-Version: 0.2.2
+Name: tdimport_client
+Version: 0.2.3
 Summary: E360 TDImport Service Client for Python
 Author: IQVIA
 Author-email: e360pypi@iqvia.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.7
 License-File: LICENSE.txt
-Requires-Dist: clients-core (<3,>=2.1.1)
-Requires-Dist: pydantic
+Requires-Dist: clients-core <3,>=2.1.1
+Requires-Dist: pydantic <2
```

