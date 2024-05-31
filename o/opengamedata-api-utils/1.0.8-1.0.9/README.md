# Comparing `tmp/opengamedata_api_utils-1.0.8.tar.gz` & `tmp/opengamedata_api_utils-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengamedata_api_utils-1.0.8.tar", last modified: Thu May 16 04:33:54 2024, max compression
+gzip compressed data, was "opengamedata_api_utils-1.0.9.tar", last modified: Fri May 31 17:26:48 2024, max compression
```

## Comparing `opengamedata_api_utils-1.0.8.tar` & `opengamedata_api_utils-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:33:54.396318 opengamedata_api_utils-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-16 04:33:42.000000 opengamedata_api_utils-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-16 04:33:54.396318 opengamedata_api_utils-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-16 04:33:42.000000 opengamedata_api_utils-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-16 04:33:42.000000 opengamedata_api_utils-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 04:33:54.396318 opengamedata_api_utils-1.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:33:54.392318 opengamedata_api_utils-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:33:54.392318 opengamedata_api_utils-1.0.8/src/ogd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:33:54.392318 opengamedata_api_utils-1.0.8/src/ogd/apis/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-16 04:33:42.000000 opengamedata_api_utils-1.0.8/src/ogd/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:33:54.392318 opengamedata_api_utils-1.0.8/src/ogd/apis/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-16 04:33:42.000000 opengamedata_api_utils-1.0.8/src/ogd/apis/schemas/ServerConfigSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 04:33:42.000000 opengamedata_api_utils-1.0.8/src/ogd/apis/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:33:54.392318 opengamedata_api_utils-1.0.8/src/ogd/apis/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-16 04:33:42.000000 opengamedata_api_utils-1.0.8/src/ogd/apis/utils/APIResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-16 04:33:42.000000 opengamedata_api_utils-1.0.8/src/ogd/apis/utils/APIUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-16 04:33:42.000000 opengamedata_api_utils-1.0.8/src/ogd/apis/utils/HelloAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 04:33:42.000000 opengamedata_api_utils-1.0.8/src/ogd/apis/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:33:54.396318 opengamedata_api_utils-1.0.8/src/opengamedata_api_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-16 04:33:54.000000 opengamedata_api_utils-1.0.8/src/opengamedata_api_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-16 04:33:54.000000 opengamedata_api_utils-1.0.8/src/opengamedata_api_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 04:33:54.000000 opengamedata_api_utils-1.0.8/src/opengamedata_api_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-16 04:33:54.000000 opengamedata_api_utils-1.0.8/src/opengamedata_api_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:48.098001 opengamedata_api_utils-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-31 17:26:35.000000 opengamedata_api_utils-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-31 17:26:48.098001 opengamedata_api_utils-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-31 17:26:35.000000 opengamedata_api_utils-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-31 17:26:35.000000 opengamedata_api_utils-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 17:26:48.098001 opengamedata_api_utils-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:48.098001 opengamedata_api_utils-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:48.094001 opengamedata_api_utils-1.0.9/src/ogd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:48.098001 opengamedata_api_utils-1.0.9/src/ogd/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-31 17:26:35.000000 opengamedata_api_utils-1.0.9/src/ogd/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:48.098001 opengamedata_api_utils-1.0.9/src/ogd/apis/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-31 17:26:35.000000 opengamedata_api_utils-1.0.9/src/ogd/apis/schemas/ServerConfigSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:35.000000 opengamedata_api_utils-1.0.9/src/ogd/apis/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:48.098001 opengamedata_api_utils-1.0.9/src/ogd/apis/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-31 17:26:35.000000 opengamedata_api_utils-1.0.9/src/ogd/apis/utils/APIResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-31 17:26:35.000000 opengamedata_api_utils-1.0.9/src/ogd/apis/utils/APIUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-31 17:26:35.000000 opengamedata_api_utils-1.0.9/src/ogd/apis/utils/HelloAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:35.000000 opengamedata_api_utils-1.0.9/src/ogd/apis/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:48.098001 opengamedata_api_utils-1.0.9/src/opengamedata_api_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-31 17:26:48.000000 opengamedata_api_utils-1.0.9/src/opengamedata_api_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-31 17:26:48.000000 opengamedata_api_utils-1.0.9/src/opengamedata_api_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 17:26:48.000000 opengamedata_api_utils-1.0.9/src/opengamedata_api_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-31 17:26:48.000000 opengamedata_api_utils-1.0.9/src/opengamedata_api_utils.egg-info/top_level.txt
```

### Comparing `opengamedata_api_utils-1.0.8/LICENSE` & `opengamedata_api_utils-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.8/PKG-INFO` & `opengamedata_api_utils-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengamedata-api-utils
-Version: 1.0.8
+Version: 1.0.9
 Summary: Package of utilities for server-side scripts in OpenGameData.
 Author: Ryan Wilkinson, Glenn Palmer, Daus Husaini
 Author-email: Luke Swanson <superscription58@gmail.com>
 Project-URL: Homepage, https://github.com/opengamedata/opengamedata-api-utils
 Project-URL: Bug Tracker, https://github.com/opengamedata/opengamedata-api-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `opengamedata_api_utils-1.0.8/README.md` & `opengamedata_api_utils-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.8/pyproject.toml` & `opengamedata_api_utils-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.8/src/ogd/apis/schemas/ServerConfigSchema.py` & `opengamedata_api_utils-1.0.9/src/ogd/apis/schemas/ServerConfigSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.8/src/ogd/apis/utils/APIResponse.py` & `opengamedata_api_utils-1.0.9/src/ogd/apis/utils/APIResponse.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Contains class for representing a response from an OGD API,
 as well as utility enums used by the APIResponse class.
 """
 
 # import standard libraries
 import json
 from enum import IntEnum
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 
 # import 3rd-party libraries
 
 # import OGD libraries
 import ogd.core.requests.RequestResult as RequestResult
 
 # Import local files
@@ -67,15 +67,15 @@
                 return "INVALID STATUS TYPE"
 
 class APIResponse:
     def __init__(self, req_type:RESTType, val:Any, msg:str, status:ResponseStatus):
         self._type   : RESTType       = req_type
         self._val    : Dict[str, Any] = val
         self._msg    : str            = msg
-        self._status : ResponseStatus   = status
+        self._status : ResponseStatus = status
 
     def __str__(self):
         return f"{self.Type.name} request: {self.Status}\n{self.Message}\nValues: {self.Value}"
 
     @staticmethod
     def Default(req_type:RESTType):
         return APIResponse(
@@ -92,14 +92,32 @@
             _status = ResponseStatus.SUCCESS 
         elif result.Status == RequestResult.ResultStatus.FAILURE:
             _status = ResponseStatus.ERR_REQ
         else:
             _status = ResponseStatus.ERR_SRV
         ret_val = APIResponse(req_type=req_type, val=None, msg=result.Message, status=_status)
         return ret_val
+    
+    @staticmethod
+    def FromDict(all_elements:Dict[str, Any]) -> Optional["APIResponse"]:
+        ret_val : Optional["APIResponse"] = None
+
+        _type_str   = all_elements.get("type", "NOT FOUND").upper()
+        _val        = all_elements.get("val", {})
+        _msg        = all_elements.get("msg", "NOT FOUND")
+        _status_str = all_elements.get("status", "NOT FOUND").upper()
+        try:
+            _type   = RESTType[_type_str]
+            _status = ResponseStatus[_status_str]
+        except KeyError as err:
+            pass
+        else:
+            ret_val = APIResponse(req_type=_type, val=_val, msg=_msg, status=_status)
+        finally:
+            return ret_val
 
     @property
     def Type(self) -> RESTType:
         """Property for the type of REST request
 
         :return: A RESTType representing the type of REST request
         :rtype: _type_
```

### Comparing `opengamedata_api_utils-1.0.8/src/ogd/apis/utils/APIUtils.py` & `opengamedata_api_utils-1.0.9/src/ogd/apis/utils/APIUtils.py`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.8/src/ogd/apis/utils/HelloAPI.py` & `opengamedata_api_utils-1.0.9/src/ogd/apis/utils/HelloAPI.py`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.8/src/opengamedata_api_utils.egg-info/PKG-INFO` & `opengamedata_api_utils-1.0.9/src/opengamedata_api_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengamedata-api-utils
-Version: 1.0.8
+Version: 1.0.9
 Summary: Package of utilities for server-side scripts in OpenGameData.
 Author: Ryan Wilkinson, Glenn Palmer, Daus Husaini
 Author-email: Luke Swanson <superscription58@gmail.com>
 Project-URL: Homepage, https://github.com/opengamedata/opengamedata-api-utils
 Project-URL: Bug Tracker, https://github.com/opengamedata/opengamedata-api-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

