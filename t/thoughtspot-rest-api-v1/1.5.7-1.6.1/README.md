# Comparing `tmp/thoughtspot_rest_api_v1-1.5.7.tar.gz` & `tmp/thoughtspot_rest_api_v1-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thoughtspot_rest_api_v1-1.5.7.tar", last modified: Thu Mar 21 20:19:42 2024, max compression
+gzip compressed data, was "thoughtspot_rest_api_v1-1.6.1.tar", last modified: Fri May 31 12:49:17 2024, max compression
```

## Comparing `thoughtspot_rest_api_v1-1.5.7.tar` & `thoughtspot_rest_api_v1-1.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2024-03-21 20:19:42.296886 thoughtspot_rest_api_v1-1.5.7/
--rw-r--r--   0 bryant.howell (535524999) 1339924365    14780 2022-04-06 21:26:49.000000 thoughtspot_rest_api_v1-1.5.7/LICENSE
--rw-r--r--   0 bryant.howell (535524999) 1339924365    29146 2024-03-21 20:19:42.296780 thoughtspot_rest_api_v1-1.5.7/PKG-INFO
--rw-r--r--   0 bryant.howell (535524999) 1339924365    28378 2023-09-19 19:22:42.000000 thoughtspot_rest_api_v1-1.5.7/README.md
--rw-r--r--   0 bryant.howell (535524999) 1339924365       85 2022-04-04 15:39:10.000000 thoughtspot_rest_api_v1-1.5.7/pyproject.toml
--rw-r--r--   0 bryant.howell (535524999) 1339924365      884 2024-03-21 20:19:42.297251 thoughtspot_rest_api_v1-1.5.7/setup.cfg
--rw-r--r--   0 bryant.howell (535524999) 1339924365      236 2022-04-04 15:39:10.000000 thoughtspot_rest_api_v1-1.5.7/setup.py
-drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2024-03-21 20:19:42.291483 thoughtspot_rest_api_v1-1.5.7/src/
-drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2024-03-21 20:19:42.294823 thoughtspot_rest_api_v1-1.5.7/src/thoughtspot_rest_api_v1/
--rw-r--r--   0 bryant.howell (535524999) 1339924365      318 2022-09-09 16:25:24.000000 thoughtspot_rest_api_v1-1.5.7/src/thoughtspot_rest_api_v1/__init__.py
--rw-r--r--   0 bryant.howell (535524999) 1339924365       22 2024-03-21 20:19:21.000000 thoughtspot_rest_api_v1-1.5.7/src/thoughtspot_rest_api_v1/_version.py
--rw-r--r--   0 bryant.howell (535524999) 1339924365     2328 2022-09-09 16:25:24.000000 thoughtspot_rest_api_v1-1.5.7/src/thoughtspot_rest_api_v1/details_objects.py
--rw-r--r--   0 bryant.howell (535524999) 1339924365    75805 2023-06-05 14:38:31.000000 thoughtspot_rest_api_v1-1.5.7/src/thoughtspot_rest_api_v1/tsrestapiv1.py
--rw-r--r--   0 bryant.howell (535524999) 1339924365    27517 2024-03-21 20:18:19.000000 thoughtspot_rest_api_v1-1.5.7/src/thoughtspot_rest_api_v1/tsrestapiv2.py
-drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2024-03-21 20:19:42.296463 thoughtspot_rest_api_v1-1.5.7/src/thoughtspot_rest_api_v1.egg-info/
--rw-r--r--   0 bryant.howell (535524999) 1339924365    29146 2024-03-21 20:19:42.000000 thoughtspot_rest_api_v1-1.5.7/src/thoughtspot_rest_api_v1.egg-info/PKG-INFO
--rw-r--r--   0 bryant.howell (535524999) 1339924365      518 2024-03-21 20:19:42.000000 thoughtspot_rest_api_v1-1.5.7/src/thoughtspot_rest_api_v1.egg-info/SOURCES.txt
--rw-r--r--   0 bryant.howell (535524999) 1339924365        1 2024-03-21 20:19:42.000000 thoughtspot_rest_api_v1-1.5.7/src/thoughtspot_rest_api_v1.egg-info/dependency_links.txt
--rw-r--r--   0 bryant.howell (535524999) 1339924365       22 2024-03-21 20:19:42.000000 thoughtspot_rest_api_v1-1.5.7/src/thoughtspot_rest_api_v1.egg-info/requires.txt
--rw-r--r--   0 bryant.howell (535524999) 1339924365       24 2024-03-21 20:19:42.000000 thoughtspot_rest_api_v1-1.5.7/src/thoughtspot_rest_api_v1.egg-info/top_level.txt
+drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2024-05-31 12:49:17.353702 thoughtspot_rest_api_v1-1.6.1/
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    14780 2022-04-06 21:26:49.000000 thoughtspot_rest_api_v1-1.6.1/LICENSE
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    29179 2024-05-31 12:49:17.353427 thoughtspot_rest_api_v1-1.6.1/PKG-INFO
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    28378 2023-09-19 19:22:42.000000 thoughtspot_rest_api_v1-1.6.1/README.md
+-rw-r--r--   0 bryant.howell (535524999) 1339924365       85 2022-04-04 15:39:10.000000 thoughtspot_rest_api_v1-1.6.1/pyproject.toml
+-rw-r--r--   0 bryant.howell (535524999) 1339924365      903 2024-05-31 12:49:17.354259 thoughtspot_rest_api_v1-1.6.1/setup.cfg
+-rw-r--r--   0 bryant.howell (535524999) 1339924365      236 2022-04-04 15:39:10.000000 thoughtspot_rest_api_v1-1.6.1/setup.py
+drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2024-05-31 12:49:17.333741 thoughtspot_rest_api_v1-1.6.1/src/
+drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2024-05-31 12:49:17.346281 thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1/
+-rw-r--r--   0 bryant.howell (535524999) 1339924365      318 2022-09-09 16:25:24.000000 thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1/__init__.py
+-rw-r--r--   0 bryant.howell (535524999) 1339924365       22 2024-05-31 12:48:22.000000 thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1/_version.py
+-rw-r--r--   0 bryant.howell (535524999) 1339924365     2328 2022-09-09 16:25:24.000000 thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1/details_objects.py
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    76379 2024-05-31 12:15:19.000000 thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1/tsrestapiv1.py
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    28187 2024-05-31 12:48:22.000000 thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1/tsrestapiv2.py
+drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2024-05-31 12:49:17.352909 thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1.egg-info/
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    29179 2024-05-31 12:49:17.000000 thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1.egg-info/PKG-INFO
+-rw-r--r--   0 bryant.howell (535524999) 1339924365      518 2024-05-31 12:49:17.000000 thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1.egg-info/SOURCES.txt
+-rw-r--r--   0 bryant.howell (535524999) 1339924365        1 2024-05-31 12:49:17.000000 thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1.egg-info/dependency_links.txt
+-rw-r--r--   0 bryant.howell (535524999) 1339924365       40 2024-05-31 12:49:17.000000 thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1.egg-info/requires.txt
+-rw-r--r--   0 bryant.howell (535524999) 1339924365       24 2024-05-31 12:49:17.000000 thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1.egg-info/top_level.txt
```

### Comparing `thoughtspot_rest_api_v1-1.5.7/LICENSE` & `thoughtspot_rest_api_v1-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thoughtspot_rest_api_v1-1.5.7/PKG-INFO` & `thoughtspot_rest_api_v1-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoughtspot_rest_api_v1
-Version: 1.5.7
+Version: 1.6.1
 Summary: Library implementing the ThoughtSpot V1 REST API
 Home-page: https://github.com/thoughtspot/thoughtspot_rest_api_v1_python
 Author: Bryant Howell
 Author-email: bryant.howell@thoughtspot.com
 License: MIT
 Project-URL: Documentation, https://github.com/thoughtspot/thoughtspot_rest_api_v1_python#readme
 Project-URL: Bug Tracker, https://github.com/thoughtspot/thoughtspot_rest_api_v1_python/issues
@@ -13,14 +13,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: PyYAML
 Requires-Dist: oyaml
+Requires-Dist: requests_toolbelt
 
 *A simple and pythonic Python implementation of ThoughtSpot's REST APIs (both V1 and V2).*
 
 `thoughtspot_rest_api_v1` library implements the ThoughtSpot public REST APIs as directly as possible. It is not a "full SDK" with representation of each request and response type, but rather uses Python's Lists and Dicts for input and output.
 
 Each API endpoint is represented by a single method within the `TSRestApiV1` or `TSRestApiV2` class.
```

### Comparing `thoughtspot_rest_api_v1-1.5.7/README.md` & `thoughtspot_rest_api_v1-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `thoughtspot_rest_api_v1-1.5.7/setup.cfg` & `thoughtspot_rest_api_v1-1.6.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = thoughtspot_rest_api_v1
-version = 1.5.7
+version = 1.6.1
 description = Library implementing the ThoughtSpot V1 REST API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/thoughtspot/thoughtspot_rest_api_v1_python
 author = Bryant Howell
 author_email = bryant.howell@thoughtspot.com
 license = MIT
@@ -22,14 +22,15 @@
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	requests
 	PyYAML
 	oyaml
+	requests_toolbelt
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `thoughtspot_rest_api_v1-1.5.7/src/thoughtspot_rest_api_v1/details_objects.py` & `thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1/details_objects.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_rest_api_v1-1.5.7/src/thoughtspot_rest_api_v1/tsrestapiv1.py` & `thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1/tsrestapiv1.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 #   and notes written throughout to help the reader understand more.
 #
 from collections import OrderedDict
 from typing import Optional, Dict, List, Union
 import json
 
 import requests
+from requests_toolbelt.adapters.socket_options import TCPKeepAliveAdapter
 
 
 class MetadataTypes:
     """
     Value provided as the 'type' parameter in the
     /metadata/ endpoint calls.
 
@@ -175,14 +176,23 @@
         self.non_public_base_url = '{server}/callosum/v1/'.format(server=self.server)
         # V2 REST API for basic implementation
         self.v2_base_url = '{server}/tspublic/rest/v2/'.format(server=self.server)
 
         # Flag for whether the version implements the export_fqn option of metadata/tml/export
         self.can_export_fqn = True
 
+    # The following two methods allow for modifying the session for long-lived purposes, particularly TML import
+    @staticmethod
+    def get_default_tcp_keep_alive_adaptor() -> TCPKeepAliveAdapter:
+        return TCPKeepAliveAdapter(idle=120, count=20, interval=30)
+
+    def set_tcp_keep_alive_adaptor(self, tcp_keep_alive_adaptor: TCPKeepAliveAdapter):
+        self.requests_session.mount('http://', tcp_keep_alive_adaptor)
+        self.requests_session.mount('https://', tcp_keep_alive_adaptor)
+
     #
     # Session management calls
     # - up here vs. in the SESSION section below (because these two are required)
     #
     def session_login(self, username: str, password: str, remember_me: bool = True) -> bool:
         endpoint = 'session/login'
         post_data = {'username': username, 'password': password, 'rememberme': str(remember_me).lower()}
```

### Comparing `thoughtspot_rest_api_v1-1.5.7/src/thoughtspot_rest_api_v1/tsrestapiv2.py` & `thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1/tsrestapiv2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import OrderedDict
 from typing import Optional, Dict, List, Union
 import json
 
 import requests
-
+from requests_toolbelt.adapters.socket_options import TCPKeepAliveAdapter
 
 class ReportTypes:
     PDF = 'PDF'
     XLSX = 'XLSX'
     CSV = 'CSV'
     PNG = 'PNG'
 
@@ -53,14 +53,23 @@
         # Will be set after initial request
         self.__bearer_token = None
 
         # TS documentation shows the /tspublic/v2/ portion but it is always preceded by {server}/callosum/v2/
         self.base_url = '{server}/api/rest/{version}/'.format(server=self.server, version=self.api_version)
         # self.non_public_base_url = '{server}/callosum/v1/'.format(server=self.server)
 
+    # The following two methods allow for modifying the session for long-lived purposes, particularly TML import
+    @staticmethod
+    def get_default_tcp_keep_alive_adaptor() -> TCPKeepAliveAdapter:
+        return TCPKeepAliveAdapter(idle=120, count=20, interval=30)
+
+    def set_tcp_keep_alive_adaptor(self, tcp_keep_alive_adaptor: TCPKeepAliveAdapter):
+        self.requests_session.mount('http://', tcp_keep_alive_adaptor)
+        self.requests_session.mount('https://', tcp_keep_alive_adaptor)
+
     @property
     def bearer_token(self):
         return self.__bearer_token
 
     @bearer_token.setter
     def bearer_token(self, bearer_token):
         self.__bearer_token = bearer_token
@@ -69,29 +78,32 @@
 
     #
     # Session management calls
     # - up here vs. in the SESSION section below (because these two are required)
     #
     def auth_session_login(self,  username: Optional[str] = None, password: Optional[str] = None,
                            remember_me: bool = True,
-                           bearer_token: Optional[str] = None) -> requests.Session:
+                           bearer_token: Optional[str] = None,
+                           org_identifier: Optional[int] = None) -> requests.Session:
         endpoint = 'auth/session/login'
 
         url = self.base_url + endpoint
 
         if bearer_token is not None:
             response = self.requests_session.post(url=url,
                                                   headers={"Authorization": "Bearer {}".format(bearer_token)},
                                                   json={'remember_me': str(remember_me).lower()})
         elif username is not None and password is not None:
             json_post_data = {
                 'username': username,
                 'password': password,
                 'remember_me': str(remember_me).lower()
             }
+            if org_identifier is not None:
+                json_post_data["org_identifier"] = org_identifier
             response = self.requests_session.post(url=url, json=json_post_data)
         else:
             raise Exception("If using username/password, must include both")
 
         # HTTP 204 - success, no content
         response.raise_for_status()
         return self.requests_session
@@ -354,16 +366,14 @@
         return self.post_request(endpoint=endpoint)
 
     #
     # /metadata/tag endpoints
     #
     def tags_search(self, tag_identifier: Optional[str] = None, color: Optional[str] = None):
         endpoint = 'tags/search'
-        if tag_identifier is None and color is None:
-            raise Exception("Must provide tag_identifier or color")
         request = {}
         if tag_identifier is not None:
             request['tag_identifier'] = tag_identifier
         if color is not None:
             request['color'] = color
         return self.post_request(endpoint=endpoint, request=request)
 
@@ -458,16 +468,17 @@
         endpoint = 'metadata/tml/export'
 
         request = {
             'export_associated': export_associated,
             'export_fqn': export_fqn
         }
         # These are left as optionals / defaults because they may have been added after 9.5
-        if edoc_format.upper() == 'YAML':
-            request['edoc_format'] = 'YAML'
+        if edoc_format is not None:
+            if edoc_format.upper() == 'YAML':
+                request['edoc_format'] = 'YAML'
         if export_schema_version is not None:
             request['export_schema_version'] = export_schema_version
         if metadata_request is not None:
             request['metadata'] = metadata_request
         else:
             metadata_list = []
             for i in metadata_ids:
```

### Comparing `thoughtspot_rest_api_v1-1.5.7/src/thoughtspot_rest_api_v1.egg-info/PKG-INFO` & `thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoughtspot_rest_api_v1
-Version: 1.5.7
+Version: 1.6.1
 Summary: Library implementing the ThoughtSpot V1 REST API
 Home-page: https://github.com/thoughtspot/thoughtspot_rest_api_v1_python
 Author: Bryant Howell
 Author-email: bryant.howell@thoughtspot.com
 License: MIT
 Project-URL: Documentation, https://github.com/thoughtspot/thoughtspot_rest_api_v1_python#readme
 Project-URL: Bug Tracker, https://github.com/thoughtspot/thoughtspot_rest_api_v1_python/issues
@@ -13,14 +13,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: PyYAML
 Requires-Dist: oyaml
+Requires-Dist: requests_toolbelt
 
 *A simple and pythonic Python implementation of ThoughtSpot's REST APIs (both V1 and V2).*
 
 `thoughtspot_rest_api_v1` library implements the ThoughtSpot public REST APIs as directly as possible. It is not a "full SDK" with representation of each request and response type, but rather uses Python's Lists and Dicts for input and output.
 
 Each API endpoint is represented by a single method within the `TSRestApiV1` or `TSRestApiV2` class.
```

### Comparing `thoughtspot_rest_api_v1-1.5.7/src/thoughtspot_rest_api_v1.egg-info/SOURCES.txt` & `thoughtspot_rest_api_v1-1.6.1/src/thoughtspot_rest_api_v1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

