# Comparing `tmp/crudfastapi-0.0.8.tar.gz` & `tmp/crudfastapi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crudfastapi-0.0.8.tar", max compression
+gzip compressed data, was "crudfastapi-0.0.9.tar", max compression
```

## Comparing `crudfastapi-0.0.8.tar` & `crudfastapi-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      403 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/crud/__init__.py
--rw-r--r--   0        0        0    73026 2024-05-28 08:04:14.443842 crudfastapi-0.0.8/CRUDFastAPI/crud/fast_crud.py
--rw-r--r--   0        0        0     6121 2024-05-15 05:35:59.523525 crudfastapi-0.0.8/CRUDFastAPI/crud/helper.py
--rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/endpoint/__init__.py
--rw-r--r--   0        0        0    10362 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/endpoint/crud_router.py
--rw-r--r--   0        0        0    24496 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/endpoint/endpoint_creator.py
--rw-r--r--   0        0        0     3993 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/endpoint/helper.py
--rw-r--r--   0        0        0       64 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/exceptions/__init__.py
--rw-r--r--   0        0        0     2105 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/exceptions/http_exceptions.py
--rw-r--r--   0        0        0      255 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/paginated/__init__.py
--rw-r--r--   0        0        0      821 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/paginated/helper.py
--rw-r--r--   0        0        0     1034 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/paginated/response.py
--rw-r--r--   0        0        0      397 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/paginated/schemas.py
--rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/py.typed
--rw-r--r--   0        0        0     1088 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/LICENSE
--rw-r--r--   0        0        0     1498 2024-05-28 08:03:28.031007 crudfastapi-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     8347 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/README.md
--rw-r--r--   0        0        0     9370 1970-01-01 00:00:00.000000 crudfastapi-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      403 2024-05-14 02:36:21.061981 crudfastapi-0.0.9/CRUDFastAPI/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.9/CRUDFastAPI/crud/__init__.py
+-rw-r--r--   0        0        0    73026 2024-05-28 08:04:14.443842 crudfastapi-0.0.9/CRUDFastAPI/crud/fast_crud.py
+-rw-r--r--   0        0        0     6121 2024-05-15 05:35:59.523525 crudfastapi-0.0.9/CRUDFastAPI/crud/helper.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.9/CRUDFastAPI/endpoint/__init__.py
+-rw-r--r--   0        0        0    10362 2024-05-14 02:36:21.061981 crudfastapi-0.0.9/CRUDFastAPI/endpoint/crud_router.py
+-rw-r--r--   0        0        0    24496 2024-05-14 02:36:21.061981 crudfastapi-0.0.9/CRUDFastAPI/endpoint/endpoint_creator.py
+-rw-r--r--   0        0        0     3993 2024-05-14 02:36:21.061981 crudfastapi-0.0.9/CRUDFastAPI/endpoint/helper.py
+-rw-r--r--   0        0        0       64 2024-05-14 02:36:21.061981 crudfastapi-0.0.9/CRUDFastAPI/exceptions/__init__.py
+-rw-r--r--   0        0        0     2668 2024-05-31 04:30:31.997828 crudfastapi-0.0.9/CRUDFastAPI/exceptions/http_exceptions.py
+-rw-r--r--   0        0        0      255 2024-05-14 02:36:21.061981 crudfastapi-0.0.9/CRUDFastAPI/paginated/__init__.py
+-rw-r--r--   0        0        0      821 2024-05-14 02:36:21.061981 crudfastapi-0.0.9/CRUDFastAPI/paginated/helper.py
+-rw-r--r--   0        0        0     1034 2024-05-14 02:36:21.061981 crudfastapi-0.0.9/CRUDFastAPI/paginated/response.py
+-rw-r--r--   0        0        0      397 2024-05-14 02:36:21.061981 crudfastapi-0.0.9/CRUDFastAPI/paginated/schemas.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.9/CRUDFastAPI/py.typed
+-rw-r--r--   0        0        0     1088 2024-05-14 02:36:21.061981 crudfastapi-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2614 2024-05-31 04:30:52.215868 crudfastapi-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     8347 2024-05-14 02:36:21.061981 crudfastapi-0.0.9/README.md
+-rw-r--r--   0        0        0     9370 1970-01-01 00:00:00.000000 crudfastapi-0.0.9/PKG-INFO
```

### Comparing `crudfastapi-0.0.8/CRUDFastAPI/crud/fast_crud.py` & `crudfastapi-0.0.9/CRUDFastAPI/crud/fast_crud.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.8/CRUDFastAPI/crud/helper.py` & `crudfastapi-0.0.9/CRUDFastAPI/crud/helper.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.8/CRUDFastAPI/endpoint/crud_router.py` & `crudfastapi-0.0.9/CRUDFastAPI/endpoint/crud_router.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.8/CRUDFastAPI/endpoint/endpoint_creator.py` & `crudfastapi-0.0.9/CRUDFastAPI/endpoint/endpoint_creator.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.8/CRUDFastAPI/endpoint/helper.py` & `crudfastapi-0.0.9/CRUDFastAPI/endpoint/helper.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.8/CRUDFastAPI/exceptions/http_exceptions.py` & `crudfastapi-0.0.9/CRUDFastAPI/exceptions/http_exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,87 @@
+from http import HTTPStatus
 from typing import Union
 
-from http import HTTPStatus
 from fastapi import HTTPException, status
 
 
 class CustomException(HTTPException):
     def __init__(
         self,
         status_code: int = status.HTTP_500_INTERNAL_SERVER_ERROR,
         detail: Union[str, None] = None,
+        headers: dict[str, str] = None,
     ):
         if not detail:  # pragma: no cover
             detail = HTTPStatus(status_code).description
-        super().__init__(status_code=status_code, detail=detail)
+        super().__init__(status_code=status_code, detail=detail, headers=headers)
 
 
 class BadRequestException(CustomException):
-    def __init__(self, detail: Union[str, None] = None):
-        super().__init__(
-            status_code=status.HTTP_400_BAD_REQUEST, detail=detail
-        )  # pragma: no cover
+    def __init__(
+        self,
+        detail: Union[str, None] = None,
+        headers: dict[str, str] = None,
+    ):
+        super().__init__(status_code=status.HTTP_400_BAD_REQUEST, detail=detail, headers=headers)  # pragma: no cover
 
 
 class NotFoundException(CustomException):
-    def __init__(self, detail: Union[str, None] = None):
-        super().__init__(
-            status_code=status.HTTP_404_NOT_FOUND, detail=detail
-        )  # pragma: no cover
+    def __init__(
+        self,
+        detail: Union[str, None] = None,
+        headers: dict[str, str] = None,
+    ):
+        super().__init__(status_code=status.HTTP_404_NOT_FOUND, detail=detail, headers=headers)  # pragma: no cover
 
 
 class ForbiddenException(CustomException):
-    def __init__(self, detail: Union[str, None] = None):
-        super().__init__(
-            status_code=status.HTTP_403_FORBIDDEN, detail=detail
-        )  # pragma: no cover
+    def __init__(
+        self,
+        detail: Union[str, None] = None,
+        headers: dict[str, str] = None,
+    ):
+        super().__init__(status_code=status.HTTP_403_FORBIDDEN, detail=detail, headers=headers)  # pragma: no cover
 
 
 class UnauthorizedException(CustomException):
-    def __init__(self, detail: Union[str, None] = None):
-        super().__init__(
-            status_code=status.HTTP_401_UNAUTHORIZED, detail=detail
-        )  # pragma: no cover
+    def __init__(
+        self,
+        detail: Union[str, None] = None,
+        headers: dict[str, str] = None,
+    ):
+        super().__init__(status_code=status.HTTP_401_UNAUTHORIZED, detail=detail, headers=headers)  # pragma: no cover
 
 
 class UnprocessableEntityException(CustomException):
-    def __init__(self, detail: Union[str, None] = None):
+    def __init__(
+        self,
+        detail: Union[str, None] = None,
+        headers: dict[str, str] = None,
+    ):
         super().__init__(
-            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY, detail=detail
+            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+            detail=detail,
+            headers=headers,
         )  # pragma: no cover
 
 
 class DuplicateValueException(CustomException):
-    def __init__(self, detail: Union[str, None] = None):
-        super().__init__(
-            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY, detail=detail
-        )
+    def __init__(
+        self,
+        detail: Union[str, None] = None,
+        headers: dict[str, str] = None,
+    ):
+        super().__init__(status_code=status.HTTP_422_UNPROCESSABLE_ENTITY, detail=detail)
 
 
 class RateLimitException(CustomException):
-    def __init__(self, detail: Union[str, None] = None):
+    def __init__(
+        self,
+        detail: Union[str, None] = None,
+        headers: dict[str, str] = None,
+    ):
         super().__init__(
-            status_code=status.HTTP_429_TOO_MANY_REQUESTS, detail=detail
+            status_code=status.HTTP_429_TOO_MANY_REQUESTS,
+            detail=detail,
+            headers=headers,
         )  # pragma: no cover
```

### Comparing `crudfastapi-0.0.8/CRUDFastAPI/paginated/helper.py` & `crudfastapi-0.0.9/CRUDFastAPI/paginated/helper.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.8/CRUDFastAPI/paginated/response.py` & `crudfastapi-0.0.9/CRUDFastAPI/paginated/response.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.8/LICENSE` & `crudfastapi-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.8/README.md` & `crudfastapi-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.8/PKG-INFO` & `crudfastapi-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CRUDFastAPI
-Version: 0.0.8
+Version: 0.0.9
 Summary: CRUDFastAPI is a Python package for FastAPI, offering robust async CRUD operations and flexible endpoint creation utilities.
 Home-page: https://github.com/mithun2003/CRUDFastAPI
 License: MIT
 Keywords: fastapi,crud,async,sqlalchemy,pydantic,fastcrud,crudfastapi
 Author: Mithun Thomas
 Author-email: mithunthomas003@gmail.com
 Requires-Python: >=3.9,<4.0
```

