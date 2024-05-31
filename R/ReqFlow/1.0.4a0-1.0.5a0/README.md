# Comparing `tmp/ReqFlow-1.0.4a0.tar.gz` & `tmp/ReqFlow-1.0.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReqFlow-1.0.4a0.tar", last modified: Sat Mar 16 18:30:53 2024, max compression
+gzip compressed data, was "ReqFlow-1.0.5a0.tar", last modified: Fri May 31 14:33:50 2024, max compression
```

## Comparing `ReqFlow-1.0.4a0.tar` & `ReqFlow-1.0.5a0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 18:30:53.127524 ReqFlow-1.0.4a0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-16 18:30:44.000000 ReqFlow-1.0.4a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-16 18:30:44.000000 ReqFlow-1.0.4a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-03-16 18:30:53.127524 ReqFlow-1.0.4a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-03-16 18:30:44.000000 ReqFlow-1.0.4a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 18:30:53.123524 ReqFlow-1.0.4a0/ReqFlow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-03-16 18:30:53.000000 ReqFlow-1.0.4a0/ReqFlow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-16 18:30:53.000000 ReqFlow-1.0.4a0/ReqFlow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 18:30:53.000000 ReqFlow-1.0.4a0/ReqFlow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-16 18:30:53.000000 ReqFlow-1.0.4a0/ReqFlow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-16 18:30:53.000000 ReqFlow-1.0.4a0/ReqFlow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 18:30:53.123524 ReqFlow-1.0.4a0/reqflow/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-16 18:30:44.000000 ReqFlow-1.0.4a0/reqflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7835 2024-03-16 18:30:44.000000 ReqFlow-1.0.4a0/reqflow/assertions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-03-16 18:30:44.000000 ReqFlow-1.0.4a0/reqflow/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22684 2024-03-16 18:30:44.000000 ReqFlow-1.0.4a0/reqflow/fluent_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 18:30:53.123524 ReqFlow-1.0.4a0/reqflow/response/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 18:30:44.000000 ReqFlow-1.0.4a0/reqflow/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-03-16 18:30:44.000000 ReqFlow-1.0.4a0/reqflow/response/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 18:30:53.127524 ReqFlow-1.0.4a0/reqflow/validator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 18:30:44.000000 ReqFlow-1.0.4a0/reqflow/validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-16 18:30:44.000000 ReqFlow-1.0.4a0/reqflow/validator/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 18:30:53.127524 ReqFlow-1.0.4a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-16 18:30:44.000000 ReqFlow-1.0.4a0/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-31 14:33:50.411266 ReqFlow-1.0.5a0/
+-rw-r--r--   0 user       (501) staff       (20)     1066 2024-01-20 15:07:00.000000 ReqFlow-1.0.5a0/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)       85 2024-01-27 17:01:00.000000 ReqFlow-1.0.5a0/MANIFEST.in
+-rw-r--r--   0 user       (501) staff       (20)     1956 2024-05-31 14:33:50.410655 ReqFlow-1.0.5a0/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     1601 2024-03-16 18:38:18.000000 ReqFlow-1.0.5a0/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-31 14:33:50.409990 ReqFlow-1.0.5a0/ReqFlow.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     1956 2024-05-31 14:33:50.000000 ReqFlow-1.0.5a0/ReqFlow.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      393 2024-05-31 14:33:50.000000 ReqFlow-1.0.5a0/ReqFlow.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-05-31 14:33:50.000000 ReqFlow-1.0.5a0/ReqFlow.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       49 2024-05-31 14:33:50.000000 ReqFlow-1.0.5a0/ReqFlow.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)       14 2024-05-31 14:33:50.000000 ReqFlow-1.0.5a0/ReqFlow.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-31 14:33:50.407142 ReqFlow-1.0.5a0/reqflow/
+-rw-r--r--   0 user       (501) staff       (20)       56 2024-01-20 15:32:30.000000 ReqFlow-1.0.5a0/reqflow/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     7835 2024-01-27 16:22:39.000000 ReqFlow-1.0.5a0/reqflow/assertions.py
+-rw-r--r--   0 user       (501) staff       (20)     1517 2024-03-16 12:54:34.000000 ReqFlow-1.0.5a0/reqflow/client.py
+-rw-r--r--   0 user       (501) staff       (20)    23357 2024-05-31 14:25:46.000000 ReqFlow-1.0.5a0/reqflow/fluent_api.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-31 14:33:50.408310 ReqFlow-1.0.5a0/reqflow/response/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-12-29 19:50:15.000000 ReqFlow-1.0.5a0/reqflow/response/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     4376 2024-01-27 15:59:13.000000 ReqFlow-1.0.5a0/reqflow/response/response.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-31 14:33:50.409392 ReqFlow-1.0.5a0/reqflow/validator/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-12-29 14:12:44.000000 ReqFlow-1.0.5a0/reqflow/validator/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      482 2024-01-25 16:42:18.000000 ReqFlow-1.0.5a0/reqflow/validator/validator.py
+-rw-r--r--   0 user       (501) staff       (20)       38 2024-05-31 14:33:50.411420 ReqFlow-1.0.5a0/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      515 2024-05-31 14:33:36.000000 ReqFlow-1.0.5a0/setup.py
```

### Comparing `ReqFlow-1.0.4a0/LICENSE` & `ReqFlow-1.0.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `ReqFlow-1.0.4a0/PKG-INFO` & `ReqFlow-1.0.5a0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: ReqFlow
-Version: 1.0.4a0
+Version: 1.0.5a0
 Summary: A streamlined Python library for crafting HTTP requests and testing API
 Home-page: https://github.com/olxxi/ReqFlow
 Author: Oleksii P.
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: httpx>=0.26.0
+Requires-Dist: jsonpath-ng>=1.6.1
+Requires-Dist: pydantic>=2.5.3
 
 # ReqFlow
 
 ReqFlow is a Python library designed for efficient and intuitive API testing. 
 ReqFlow offers a fluent and flexible interface for crafting and validating HTTP requests, 
 making API testing both straightforward and adaptable. While it make sense to use standard approaches for a Python API
 testing, ReqFlow reduces the entry barrier for beginners and allows for more advanced use cases with RestAssured-like
@@ -49,21 +50,20 @@
 
 
 # Initialize the client
 client = Client(base_url="https://api.example.com")
 
 # Use ReqFlow's fluent API
 response = (given(client)
-            .header("Authorization", "Bearer your_token")
+            .header("Authorization", "Bearer TOKEN_VALUE")
             .query_param("param", "value")
             .when("GET", "/your_endpoint")
             .then()
             .validate_data(ExampleModel)
             .status_code(200)
             .get_content())
 
 print(response)
 ```
 
 ### Documentation
-Detailed documentation can be found [here](https://reqflow.org/).
-
+Detailed documentation can be found at [reqflow.org](https://reqflow.org/)
```

### Comparing `ReqFlow-1.0.4a0/README.md` & `ReqFlow-1.0.5a0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -38,20 +38,20 @@
 
 
 # Initialize the client
 client = Client(base_url="https://api.example.com")
 
 # Use ReqFlow's fluent API
 response = (given(client)
-            .header("Authorization", "Bearer your_token")
+            .header("Authorization", "Bearer TOKEN_VALUE")
             .query_param("param", "value")
             .when("GET", "/your_endpoint")
             .then()
             .validate_data(ExampleModel)
             .status_code(200)
             .get_content())
 
 print(response)
 ```
 
 ### Documentation
-Detailed documentation can be found [here](https://reqflow.org/).
+Detailed documentation can be found at [reqflow.org](https://reqflow.org/)
```

### Comparing `ReqFlow-1.0.4a0/ReqFlow.egg-info/PKG-INFO` & `ReqFlow-1.0.5a0/ReqFlow.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: ReqFlow
-Version: 1.0.4a0
+Version: 1.0.5a0
 Summary: A streamlined Python library for crafting HTTP requests and testing API
 Home-page: https://github.com/olxxi/ReqFlow
 Author: Oleksii P.
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: httpx>=0.26.0
+Requires-Dist: jsonpath-ng>=1.6.1
+Requires-Dist: pydantic>=2.5.3
 
 # ReqFlow
 
 ReqFlow is a Python library designed for efficient and intuitive API testing. 
 ReqFlow offers a fluent and flexible interface for crafting and validating HTTP requests, 
 making API testing both straightforward and adaptable. While it make sense to use standard approaches for a Python API
 testing, ReqFlow reduces the entry barrier for beginners and allows for more advanced use cases with RestAssured-like
@@ -49,21 +50,20 @@
 
 
 # Initialize the client
 client = Client(base_url="https://api.example.com")
 
 # Use ReqFlow's fluent API
 response = (given(client)
-            .header("Authorization", "Bearer your_token")
+            .header("Authorization", "Bearer TOKEN_VALUE")
             .query_param("param", "value")
             .when("GET", "/your_endpoint")
             .then()
             .validate_data(ExampleModel)
             .status_code(200)
             .get_content())
 
 print(response)
 ```
 
 ### Documentation
-Detailed documentation can be found [here](https://reqflow.org/).
-
+Detailed documentation can be found at [reqflow.org](https://reqflow.org/)
```

### Comparing `ReqFlow-1.0.4a0/reqflow/assertions.py` & `ReqFlow-1.0.5a0/reqflow/assertions.py`

 * *Files identical despite different names*

### Comparing `ReqFlow-1.0.4a0/reqflow/client.py` & `ReqFlow-1.0.5a0/reqflow/client.py`

 * *Files identical despite different names*

### Comparing `ReqFlow-1.0.4a0/reqflow/fluent_api.py` & `ReqFlow-1.0.5a0/reqflow/fluent_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Optional, Union, Type
 
 from .client import Client
 from reqflow.response.response import UnifiedResponse
 from reqflow.validator.validator import Validator
 from pydantic import BaseModel
 from pydantic import ValidationError
 import base64
@@ -341,20 +341,20 @@
             >>> 200
 
         Returns:
             UnifiedResponse: The response from the request.
         """
         return self.response
 
-    def validate_data(self, expected_model: BaseModel) -> 'Then':
+    def validate_data(self, expected_model: Type[BaseModel]) -> 'Then':
         """
         Validates the response data against the expected Pydantic model.
 
         Args:
-            expected_model (BaseModel): The Pydantic model to validate the response data against.
+            expected_model (Type[BaseModel]): The Pydantic model to validate the response data against.
 
         Raises:
             AssertionError: If the response data does not match the expected model.
 
         Examples:
             >>> from reqflow import given, Client
             >>> from pydantic import BaseModel
@@ -539,14 +539,32 @@
 
         Returns:
             Then: The instance of the Then class.
         """
         self.response._assert_header(header_name, expected_value)
         return self
 
+    def assert_header_exists(self, header_name: str) -> 'Then':
+        """
+        Asserts that a specific header exists in the response.
+
+        Args:
+            header_name (str): The name of the header to assert.
+
+        Examples:
+            >>> from reqflow import given, Client
+            >>> client = Client(base_url="https://httpbin.org")
+            >>> given(client).when("GET", "/get").then().assert_header_exists("Content-Type")
+
+        Returns:
+            Then: The instance of the Then class.
+        """
+        assert header_name in self.response.headers, f"Header {header_name} does not exist in the response"
+        return self
+
     def assert_response_time(self, max_time: float) -> 'Then':
         """
         Asserts that the response time is less than or equal to the specified maximum time.
 
         Args:
             max_time (float): The maximum expected response time in seconds.
```

### Comparing `ReqFlow-1.0.4a0/reqflow/response/response.py` & `ReqFlow-1.0.5a0/reqflow/response/response.py`

 * *Files identical despite different names*

### Comparing `ReqFlow-1.0.4a0/setup.py` & `ReqFlow-1.0.5a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ReqFlow',
-    version='1.0.4-alpha',
+    version='1.0.5-alpha',
     packages=find_packages(),
     install_requires=[
         'httpx>=0.26.0',
         'jsonpath-ng>=1.6.1',
         'pydantic>=2.5.3'
     ],
     # Metadata
```

