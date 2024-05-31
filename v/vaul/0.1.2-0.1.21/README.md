# Comparing `tmp/vaul-0.1.2.tar.gz` & `tmp/vaul-0.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vaul-0.1.2.tar", last modified: Wed May 29 15:36:35 2024, max compression
+gzip compressed data, was "vaul-0.1.21.tar", last modified: Fri May 31 00:14:25 2024, max compression
```

## Comparing `vaul-0.1.2.tar` & `vaul-0.1.21.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 sporter    (501) staff       (20)        0 2024-05-29 15:36:35.685207 vaul-0.1.2/
--rw-r--r--   0 sporter    (501) staff       (20)    34599 2024-05-29 00:30:50.000000 vaul-0.1.2/LICENSE.txt
--rw-r--r--   0 sporter    (501) staff       (20)       33 2024-05-29 00:36:56.000000 vaul-0.1.2/MANIFEST.in
--rw-r--r--   0 sporter    (501) staff       (20)     3859 2024-05-29 15:36:35.685138 vaul-0.1.2/PKG-INFO
--rw-r--r--   0 sporter    (501) staff       (20)     3567 2024-05-29 13:35:57.000000 vaul-0.1.2/README.md
--rw-r--r--   0 sporter    (501) staff       (20)       79 2024-05-29 15:36:35.685411 vaul-0.1.2/setup.cfg
--rw-r--r--   0 sporter    (501) staff       (20)      524 2024-05-29 15:36:33.000000 vaul-0.1.2/setup.py
-drwxr-xr-x   0 sporter    (501) staff       (20)        0 2024-05-29 15:36:35.684218 vaul-0.1.2/vaul/
--rw-r--r--   0 sporter    (501) staff       (20)     5018 2024-05-29 13:30:39.000000 vaul-0.1.2/vaul/__init__.py
--rw-r--r--   0 sporter    (501) staff       (20)     1312 2024-05-28 23:32:45.000000 vaul-0.1.2/vaul/ctx.py
--rw-r--r--   0 sporter    (501) staff       (20)      228 2024-05-28 17:31:12.000000 vaul-0.1.2/vaul/enums.py
--rw-r--r--   0 sporter    (501) staff       (20)     1235 2024-05-28 18:02:10.000000 vaul-0.1.2/vaul/helpers.py
--rw-r--r--   0 sporter    (501) staff       (20)      987 2024-05-28 15:31:29.000000 vaul-0.1.2/vaul/logging.py
--rw-r--r--   0 sporter    (501) staff       (20)     5891 2024-05-29 15:34:29.000000 vaul-0.1.2/vaul/models.py
--rw-r--r--   0 sporter    (501) staff       (20)     1119 2024-05-28 14:55:24.000000 vaul-0.1.2/vaul/request.py
-drwxr-xr-x   0 sporter    (501) staff       (20)        0 2024-05-29 15:36:35.684918 vaul-0.1.2/vaul.egg-info/
--rw-r--r--   0 sporter    (501) staff       (20)     3859 2024-05-29 15:36:35.000000 vaul-0.1.2/vaul.egg-info/PKG-INFO
--rw-r--r--   0 sporter    (501) staff       (20)      297 2024-05-29 15:36:35.000000 vaul-0.1.2/vaul.egg-info/SOURCES.txt
--rw-r--r--   0 sporter    (501) staff       (20)        1 2024-05-29 15:36:35.000000 vaul-0.1.2/vaul.egg-info/dependency_links.txt
--rw-r--r--   0 sporter    (501) staff       (20)       16 2024-05-29 15:36:35.000000 vaul-0.1.2/vaul.egg-info/requires.txt
--rw-r--r--   0 sporter    (501) staff       (20)        5 2024-05-29 15:36:35.000000 vaul-0.1.2/vaul.egg-info/top_level.txt
+drwxr-xr-x   0 sporter    (501) staff       (20)        0 2024-05-31 00:14:25.098056 vaul-0.1.21/
+-rw-r--r--   0 sporter    (501) staff       (20)    34599 2024-05-29 00:30:50.000000 vaul-0.1.21/LICENSE.txt
+-rw-r--r--   0 sporter    (501) staff       (20)       33 2024-05-29 00:36:56.000000 vaul-0.1.21/MANIFEST.in
+-rw-r--r--   0 sporter    (501) staff       (20)     3860 2024-05-31 00:14:25.097996 vaul-0.1.21/PKG-INFO
+-rw-r--r--   0 sporter    (501) staff       (20)     3567 2024-05-29 13:35:57.000000 vaul-0.1.21/README.md
+-rw-r--r--   0 sporter    (501) staff       (20)       79 2024-05-31 00:14:25.098263 vaul-0.1.21/setup.cfg
+-rw-r--r--   0 sporter    (501) staff       (20)      525 2024-05-31 00:13:47.000000 vaul-0.1.21/setup.py
+drwxr-xr-x   0 sporter    (501) staff       (20)        0 2024-05-31 00:14:25.097106 vaul-0.1.21/vaul/
+-rw-r--r--   0 sporter    (501) staff       (20)     5040 2024-05-30 23:50:39.000000 vaul-0.1.21/vaul/__init__.py
+-rw-r--r--   0 sporter    (501) staff       (20)     1301 2024-05-30 23:29:53.000000 vaul-0.1.21/vaul/ctx.py
+-rw-r--r--   0 sporter    (501) staff       (20)      228 2024-05-28 17:31:12.000000 vaul-0.1.21/vaul/enums.py
+-rw-r--r--   0 sporter    (501) staff       (20)     1052 2024-05-30 23:30:22.000000 vaul-0.1.21/vaul/helpers.py
+-rw-r--r--   0 sporter    (501) staff       (20)      899 2024-05-30 23:30:46.000000 vaul-0.1.21/vaul/logging.py
+-rw-r--r--   0 sporter    (501) staff       (20)     5875 2024-05-31 00:09:42.000000 vaul-0.1.21/vaul/models.py
+-rw-r--r--   0 sporter    (501) staff       (20)     1135 2024-05-30 23:33:15.000000 vaul-0.1.21/vaul/request.py
+drwxr-xr-x   0 sporter    (501) staff       (20)        0 2024-05-31 00:14:25.097786 vaul-0.1.21/vaul.egg-info/
+-rw-r--r--   0 sporter    (501) staff       (20)     3860 2024-05-31 00:14:25.000000 vaul-0.1.21/vaul.egg-info/PKG-INFO
+-rw-r--r--   0 sporter    (501) staff       (20)      297 2024-05-31 00:14:25.000000 vaul-0.1.21/vaul.egg-info/SOURCES.txt
+-rw-r--r--   0 sporter    (501) staff       (20)        1 2024-05-31 00:14:25.000000 vaul-0.1.21/vaul.egg-info/dependency_links.txt
+-rw-r--r--   0 sporter    (501) staff       (20)       16 2024-05-31 00:14:25.000000 vaul-0.1.21/vaul.egg-info/requires.txt
+-rw-r--r--   0 sporter    (501) staff       (20)        5 2024-05-31 00:14:25.000000 vaul-0.1.21/vaul.egg-info/top_level.txt
```

### Comparing `vaul-0.1.2/LICENSE.txt` & `vaul-0.1.21/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vaul-0.1.2/PKG-INFO` & `vaul-0.1.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vaul
-Version: 0.1.2
+Version: 0.1.21
 Summary: A nano-framework for deploying Python functions as APIs on AWS Lambda using Function URLs.
 Author: Spencer Porter
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pydantic==2.6.4
```

### Comparing `vaul-0.1.2/README.md` & `vaul-0.1.21/README.md`

 * *Files identical despite different names*

### Comparing `vaul-0.1.2/setup.py` & `vaul-0.1.21/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="vaul",
-    version="0.1.2",
+    version="0.1.21",
     description="A nano-framework for deploying Python functions as APIs on AWS Lambda using Function URLs.",
     author="Spencer Porter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         'pydantic==2.6.4',
     ],
```

### Comparing `vaul-0.1.2/vaul/__init__.py` & `vaul-0.1.21/vaul/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
+# vaul/__init__.py
 from __future__ import annotations
-from .ctx import RequestContextMiddleware, get_request
-from .enums import RequestMethod
-from .models import Action
-from .request import Request
-from .helpers import remove_keys_recursively
 import json
 from pydantic import ValidationError
 from typing import Callable
 
+from .ctx import RequestContextMiddleware, get_request
+from .enums import RequestMethod
+from .models import Action
+from .helpers import remove_keys_recursively
 
 class Vaul:
     instance = None
 
     @staticmethod
     def get_instance():
         if Vaul.instance is None:
@@ -68,15 +68,16 @@
             body = self.routes[path][method].run(request.json())
             return self._response(200, body, method)
         except ValidationError as e:
             return self._response(400, {'error': 'Invalid request body', 'details': str(e)}, method)
         except ValueError as e:
             return self._response(400, {'error': str(e), 'details': 'Check the path and method or JSON body format.'}, method)
         except Exception as e:
-            print(e)
+            if self.debug:
+                print(e)
             return self._response(500, {'error': str(e), 'details': 'Internal server error'}, method)
 
     def _response(self, status_code, body, method, content_type='application/json', is_base64_encoded=False):
         headers = {
             'Content-Type': content_type,
         }
 
@@ -125,7 +126,8 @@
 
     def handle_openapi_request(self, domain_name):
         return self._generate_openapi_schema(url=f'https://{domain_name}/')
 
     @staticmethod
     def handle_base_path():
         return {'message': 'Vaul Cloud API Base Path'}
+
```

### Comparing `vaul-0.1.2/vaul/ctx.py` & `vaul-0.1.21/vaul/ctx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from .request import Request
-
-from typing import Any, Dict, Optional, Callable
-
+from typing import Any, Dict, Callable
 import contextvars
 
+from .request import Request
+
 
 class RequestContext:
     def __init__(self):
         self._storage: Dict[str, Any] = {}
 
     def __getattr__(self, name: str) -> Any:
         return self._storage.get(name)
@@ -18,15 +17,14 @@
         else:
             self._storage[name] = value
 
     def __delattr__(self, name: str):
         if name in self._storage:
             del self._storage[name]
 
-
 # Create a context variable for the request context
 request_context_var = contextvars.ContextVar('request_context', default=RequestContext())
 
 
 def get_request_context() -> RequestContext:
     return request_context_var.get()
 
@@ -43,8 +41,8 @@
         token = request_context_var.set(RequestContext())
         try:
             req_ctx = get_request_context()
             req_ctx.request = Request(event)
             response = self.app(event)
         finally:
             request_context_var.reset(token)
-        return response
+        return response
```

### Comparing `vaul-0.1.2/vaul/logging.py` & `vaul-0.1.21/vaul/logging.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-from __future__ import annotations
-
 import logging
 import sys
 
 
 def has_level_handler(logger: logging.Logger) -> bool:
-    """Check if there is a handler in the logging chain that will handler
-    the given loggers :meth:`effective level <logging.Logger.getEffectiveLevel>`.
-    """
+    """Check if there is a handler in the logging chain that will handle the given logger's effective level."""
     level = logger.getEffectiveLevel()
     current = logger
 
     while current:
         if any(handler.level <= level for handler in current.handlers):
             return True
```

### Comparing `vaul-0.1.2/vaul/models.py` & `vaul-0.1.21/vaul/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,34 +71,34 @@
     def _get_model_fields_with_defaults(self) -> Tuple[Dict[str, Any], list]:
         type_hints = get_type_hints(self.func)
         signature = inspect.signature(self.func)
         model_fields = {}
         required_fields = []
 
         for param in signature.parameters.values():
-            param_type = type_hints.get(param.name, Any)
+            param_type = type_hints.get(param.name, str)  # Default to str if type hint is not provided
+            if param_type is Any and param.default is not param.empty:
+                param_type = type(param.default)
+
             if param.default is param.empty:
                 model_fields[param.name] = (param_type, ...)
                 required_fields.append(param.name)
             else:
-                if param.default is None:
-                    param_type = Optional[param_type] if param_type is not Any else Optional[str]
-                else:
-                    param_type = param_type if param_type is not Any else type(param.default)
-                model_fields[param.name] = (param_type, param.default)
+                model_fields[param.name] = (Optional[param_type], param.default)
 
         return model_fields, required_fields
 
     def _clean_schema(self, schema: Dict[str, Any], required_fields: list) -> Dict[str, Any]:
         relevant_properties = {
             k: v for k, v in schema["properties"].items() if k not in {"v__duplicate_kwargs", "args", "kwargs"}
         }
         for key, value in relevant_properties.items():
             if key not in required_fields:
                 value["nullable"] = True
+                # Adjust the type definition to avoid "anyOf"
                 if "anyOf" in value:
                     value["type"] = value["anyOf"][0].get("type", "string")
                     del value["anyOf"]
 
         schema["properties"] = relevant_properties
         schema["required"] = required_fields
         schema = remove_keys_recursively(schema, "additionalProperties")
```

### Comparing `vaul-0.1.2/vaul/request.py` & `vaul-0.1.21/vaul/request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,31 @@
+# vaul/request.py
 from urllib.parse import urlparse, parse_qs
-
 import json
 
-
 class Request:
     def __init__(self, event):
         self.method = event['requestContext']['http']['method'].upper()
         self.path = event['requestContext']['http']['path']
         self.headers = {k.lower(): v for k, v in event.get('headers', {}).items() if v is not None}
         self.body = self._parse_body(event.get('body', ''), self.headers.get('content-type', ''))
         self.query_params = self._parse_query_params(self.path)
 
     @staticmethod
     def _parse_query_params(path):
         if '?' in path:
             parsed = urlparse(path)
             parsed_params = parse_qs(parsed.query)
             return {k: v[0] for k, v in parsed_params.items()}
-
         return {}
 
     @staticmethod
     def _parse_body(body, content_type):
         if content_type == 'application/json':
             try:
                 return json.loads(body)
             except json.JSONDecodeError as e:
                 raise ValueError('Invalid JSON body') from e
         return {}
 
     def json(self):
-        return self.body if isinstance(self.body, dict) else {}
+        return self.body if isinstance(self.body, dict) else {}
```

### Comparing `vaul-0.1.2/vaul.egg-info/PKG-INFO` & `vaul-0.1.21/vaul.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vaul
-Version: 0.1.2
+Version: 0.1.21
 Summary: A nano-framework for deploying Python functions as APIs on AWS Lambda using Function URLs.
 Author: Spencer Porter
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pydantic==2.6.4
```

