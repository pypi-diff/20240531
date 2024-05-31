# Comparing `tmp/py-seal-0.0.7.tar.gz` & `tmp/py-seal-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-seal-0.0.7.tar", last modified: Wed May 29 10:34:21 2024, max compression
+gzip compressed data, was "py-seal-0.0.8.tar", last modified: Fri May 31 02:10:16 2024, max compression
```

## Comparing `py-seal-0.0.7.tar` & `py-seal-0.0.8.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-29 10:34:21.565684 py-seal-0.0.7/
--rw-r--r--   0 yehao      (501) staff       (20)    35148 2024-05-27 11:31:04.000000 py-seal-0.0.7/LICENSE
--rw-r--r--   0 yehao      (501) staff       (20)      130 2024-05-29 10:34:21.565578 py-seal-0.0.7/PKG-INFO
--rw-r--r--   0 yehao      (501) staff       (20)      772 2024-05-29 01:33:36.000000 py-seal-0.0.7/README.md
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-29 10:34:21.558841 py-seal-0.0.7/py_seal.egg-info/
--rw-r--r--   0 yehao      (501) staff       (20)      130 2024-05-29 10:34:21.000000 py-seal-0.0.7/py_seal.egg-info/PKG-INFO
--rw-r--r--   0 yehao      (501) staff       (20)      792 2024-05-29 10:34:21.000000 py-seal-0.0.7/py_seal.egg-info/SOURCES.txt
--rw-r--r--   0 yehao      (501) staff       (20)        1 2024-05-29 10:34:21.000000 py-seal-0.0.7/py_seal.egg-info/dependency_links.txt
--rw-r--r--   0 yehao      (501) staff       (20)        5 2024-05-29 10:34:21.000000 py-seal-0.0.7/py_seal.egg-info/top_level.txt
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-29 10:34:21.558944 py-seal-0.0.7/seal/
--rw-r--r--   0 yehao      (501) staff       (20)      516 2024-05-29 10:22:23.000000 py-seal-0.0.7/seal/__init__.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-29 10:34:21.559348 py-seal-0.0.7/seal/config/
--rw-r--r--   0 yehao      (501) staff       (20)       41 2024-05-29 02:01:44.000000 py-seal-0.0.7/seal/config/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)      376 2024-05-29 10:26:19.000000 py-seal-0.0.7/seal/config/configuration.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-29 10:34:21.559800 py-seal-0.0.7/seal/context/
--rw-r--r--   0 yehao      (501) staff       (20)       45 2024-05-29 02:01:44.000000 py-seal-0.0.7/seal/context/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)      623 2024-05-29 02:01:22.000000 py-seal-0.0.7/seal/context/context.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-29 10:34:21.560239 py-seal-0.0.7/seal/db/
--rw-r--r--   0 yehao      (501) staff       (20)       35 2024-05-29 02:17:30.000000 py-seal-0.0.7/seal/db/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)      122 2024-05-26 00:07:28.000000 py-seal-0.0.7/seal/db/connector.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-29 10:34:21.561260 py-seal-0.0.7/seal/db/mysql/
--rw-r--r--   0 yehao      (501) staff       (20)      120 2024-05-29 02:32:50.000000 py-seal-0.0.7/seal/db/mysql/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)     9966 2024-05-29 02:21:34.000000 py-seal-0.0.7/seal/db/mysql/base_mapper.py
--rw-r--r--   0 yehao      (501) staff       (20)     6570 2024-05-29 02:30:49.000000 py-seal-0.0.7/seal/db/mysql/chained_query.py
--rw-r--r--   0 yehao      (501) staff       (20)      728 2024-05-29 10:25:26.000000 py-seal-0.0.7/seal/db/mysql/mysql_connector.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-29 10:34:21.562254 py-seal-0.0.7/seal/db/sqlite/
--rw-r--r--   0 yehao      (501) staff       (20)      122 2024-05-29 02:34:53.000000 py-seal-0.0.7/seal/db/sqlite/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)     9399 2024-05-29 02:33:53.000000 py-seal-0.0.7/seal/db/sqlite/base_mapper.py
--rw-r--r--   0 yehao      (501) staff       (20)     6301 2024-05-29 02:34:35.000000 py-seal-0.0.7/seal/db/sqlite/chained_query.py
--rw-r--r--   0 yehao      (501) staff       (20)      320 2024-05-29 10:25:31.000000 py-seal-0.0.7/seal/db/sqlite/sqlite_connector.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-29 10:34:21.562889 py-seal-0.0.7/seal/model/
--rw-r--r--   0 yehao      (501) staff       (20)       67 2024-05-29 02:16:41.000000 py-seal-0.0.7/seal/model/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)      292 2024-05-25 14:35:24.000000 py-seal-0.0.7/seal/model/base_entity.py
--rw-r--r--   0 yehao      (501) staff       (20)      563 2024-04-03 02:38:36.000000 py-seal-0.0.7/seal/model/response.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-29 10:34:21.564389 py-seal-0.0.7/seal/router/
--rw-r--r--   0 yehao      (501) staff       (20)       67 2024-05-29 02:13:15.000000 py-seal-0.0.7/seal/router/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)     2269 2024-05-29 10:25:19.000000 py-seal-0.0.7/seal/router/router.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-29 10:34:21.564678 py-seal-0.0.7/seal/utils/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-28 10:25:13.000000 py-seal-0.0.7/seal/utils/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)      165 2024-05-29 01:31:15.000000 py-seal-0.0.7/seal/utils/str_utils.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-29 10:34:21.565315 py-seal-0.0.7/seal/wrapper/
--rw-r--r--   0 yehao      (501) staff       (20)       60 2024-05-29 02:13:15.000000 py-seal-0.0.7/seal/wrapper/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)      730 2024-05-29 01:32:54.000000 py-seal-0.0.7/seal/wrapper/entity.py
--rw-r--r--   0 yehao      (501) staff       (20)      767 2024-05-28 09:45:30.000000 py-seal-0.0.7/seal/wrapper/singleton.py
--rw-r--r--   0 yehao      (501) staff       (20)       38 2024-05-29 10:34:21.565722 py-seal-0.0.7/setup.cfg
--rw-r--r--   0 yehao      (501) staff       (20)      314 2024-05-29 10:34:07.000000 py-seal-0.0.7/setup.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-31 02:10:16.093517 py-seal-0.0.8/
+-rw-r--r--   0 yehao      (501) staff       (20)    35148 2024-05-27 11:31:04.000000 py-seal-0.0.8/LICENSE
+-rw-r--r--   0 yehao      (501) staff       (20)      130 2024-05-31 02:10:16.093396 py-seal-0.0.8/PKG-INFO
+-rw-r--r--   0 yehao      (501) staff       (20)      772 2024-05-29 10:36:57.000000 py-seal-0.0.8/README.md
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-31 02:10:16.086515 py-seal-0.0.8/py_seal.egg-info/
+-rw-r--r--   0 yehao      (501) staff       (20)      130 2024-05-31 02:10:16.000000 py-seal-0.0.8/py_seal.egg-info/PKG-INFO
+-rw-r--r--   0 yehao      (501) staff       (20)      856 2024-05-31 02:10:16.000000 py-seal-0.0.8/py_seal.egg-info/SOURCES.txt
+-rw-r--r--   0 yehao      (501) staff       (20)        1 2024-05-31 02:10:16.000000 py-seal-0.0.8/py_seal.egg-info/dependency_links.txt
+-rw-r--r--   0 yehao      (501) staff       (20)        5 2024-05-31 02:10:16.000000 py-seal-0.0.8/py_seal.egg-info/top_level.txt
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-31 02:10:16.086632 py-seal-0.0.8/seal/
+-rw-r--r--   0 yehao      (501) staff       (20)      590 2024-05-31 02:09:42.000000 py-seal-0.0.8/seal/__init__.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-31 02:10:16.087077 py-seal-0.0.8/seal/config/
+-rw-r--r--   0 yehao      (501) staff       (20)       41 2024-05-29 10:35:52.000000 py-seal-0.0.8/seal/config/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)      376 2024-05-29 10:35:52.000000 py-seal-0.0.8/seal/config/configuration.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-31 02:10:16.088530 py-seal-0.0.8/seal/context/
+-rw-r--r--   0 yehao      (501) staff       (20)       45 2024-05-29 10:35:52.000000 py-seal-0.0.8/seal/context/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)      623 2024-05-29 10:35:52.000000 py-seal-0.0.8/seal/context/context.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-31 02:10:16.088806 py-seal-0.0.8/seal/db/
+-rw-r--r--   0 yehao      (501) staff       (20)       35 2024-05-29 10:35:52.000000 py-seal-0.0.8/seal/db/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)      122 2024-05-26 00:07:28.000000 py-seal-0.0.8/seal/db/connector.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-31 02:10:16.089736 py-seal-0.0.8/seal/db/mysql/
+-rw-r--r--   0 yehao      (501) staff       (20)      120 2024-05-29 10:35:52.000000 py-seal-0.0.8/seal/db/mysql/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)     9966 2024-05-29 10:35:52.000000 py-seal-0.0.8/seal/db/mysql/base_mapper.py
+-rw-r--r--   0 yehao      (501) staff       (20)     6570 2024-05-29 10:35:52.000000 py-seal-0.0.8/seal/db/mysql/chained_query.py
+-rw-r--r--   0 yehao      (501) staff       (20)      728 2024-05-29 10:35:52.000000 py-seal-0.0.8/seal/db/mysql/mysql_connector.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-31 02:10:16.090528 py-seal-0.0.8/seal/db/sqlite/
+-rw-r--r--   0 yehao      (501) staff       (20)      122 2024-05-29 10:35:52.000000 py-seal-0.0.8/seal/db/sqlite/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)     9399 2024-05-29 10:35:52.000000 py-seal-0.0.8/seal/db/sqlite/base_mapper.py
+-rw-r--r--   0 yehao      (501) staff       (20)     6301 2024-05-29 10:35:52.000000 py-seal-0.0.8/seal/db/sqlite/chained_query.py
+-rw-r--r--   0 yehao      (501) staff       (20)      320 2024-05-29 10:35:52.000000 py-seal-0.0.8/seal/db/sqlite/sqlite_connector.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-31 02:10:16.090891 py-seal-0.0.8/seal/exception/
+-rw-r--r--   0 yehao      (501) staff       (20)       50 2024-05-30 06:42:43.000000 py-seal-0.0.8/seal/exception/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)      220 2024-05-31 01:18:19.000000 py-seal-0.0.8/seal/exception/business_exception.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-31 02:10:16.091477 py-seal-0.0.8/seal/model/
+-rw-r--r--   0 yehao      (501) staff       (20)       67 2024-05-29 10:35:52.000000 py-seal-0.0.8/seal/model/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)      292 2024-05-25 14:35:24.000000 py-seal-0.0.8/seal/model/base_entity.py
+-rw-r--r--   0 yehao      (501) staff       (20)      563 2024-04-03 02:38:36.000000 py-seal-0.0.8/seal/model/response.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-31 02:10:16.091857 py-seal-0.0.8/seal/router/
+-rw-r--r--   0 yehao      (501) staff       (20)       67 2024-05-29 10:35:52.000000 py-seal-0.0.8/seal/router/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)     2527 2024-05-30 07:19:06.000000 py-seal-0.0.8/seal/router/router.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-31 02:10:16.092697 py-seal-0.0.8/seal/utils/
+-rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-29 10:35:52.000000 py-seal-0.0.8/seal/utils/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)      165 2024-05-29 10:35:52.000000 py-seal-0.0.8/seal/utils/str_utils.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-31 02:10:16.093132 py-seal-0.0.8/seal/wrapper/
+-rw-r--r--   0 yehao      (501) staff       (20)       60 2024-05-29 10:35:52.000000 py-seal-0.0.8/seal/wrapper/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)      730 2024-05-29 10:35:52.000000 py-seal-0.0.8/seal/wrapper/entity.py
+-rw-r--r--   0 yehao      (501) staff       (20)      767 2024-05-28 09:45:30.000000 py-seal-0.0.8/seal/wrapper/singleton.py
+-rw-r--r--   0 yehao      (501) staff       (20)       38 2024-05-31 02:10:16.093558 py-seal-0.0.8/setup.cfg
+-rw-r--r--   0 yehao      (501) staff       (20)      314 2024-05-31 02:08:50.000000 py-seal-0.0.8/setup.py
```

### Comparing `py-seal-0.0.7/LICENSE` & `py-seal-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `py-seal-0.0.7/README.md` & `py-seal-0.0.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <p align="center"><h1 style="font-size: 50px" align="center">py-seal</h1></p>
 <p align="center">
     <em>基于 fastapi 的一个快速开发框架，更简约的注解、链式构建 sql 语句</em>
 </p>
 <p align="center">
-<a href="https://pypi.org/project/fastapi" target="_blank">
+<a href="https://pypi.org/project/py-seal" target="_blank">
     <img src="https://img.shields.io/pypi/v/py-seal?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
-<a href="https://pypi.org/project/fastapi" target="_blank">
+<a href="https://pypi.org/project/py-seal" target="_blank">
     <img src="https://img.shields.io/pypi/pyversions/fastapi.svg?color=%2334D058" alt="Supported Python versions">
 </a>
 </p>
 
 ---
 ## 安装
 ```shell
```

### Comparing `py-seal-0.0.7/py_seal.egg-info/SOURCES.txt` & `py-seal-0.0.8/py_seal.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 seal/db/mysql/base_mapper.py
 seal/db/mysql/chained_query.py
 seal/db/mysql/mysql_connector.py
 seal/db/sqlite/__init__.py
 seal/db/sqlite/base_mapper.py
 seal/db/sqlite/chained_query.py
 seal/db/sqlite/sqlite_connector.py
+seal/exception/__init__.py
+seal/exception/business_exception.py
 seal/model/__init__.py
 seal/model/base_entity.py
 seal/model/response.py
 seal/router/__init__.py
 seal/router/router.py
 seal/utils/__init__.py
 seal/utils/str_utils.py
```

### Comparing `py-seal-0.0.7/seal/__init__.py` & `py-seal-0.0.8/seal/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from .config import Configuration
 from .wrapper import singleton
 
+__author__ = 'melon'
+__email__ = '77729052@qq.com'
+__version__ = '0.0.8'
+
 
 @singleton
 class Seal:
 
     def __init__(self):
         self.config = Configuration()
```

### Comparing `py-seal-0.0.7/seal/context/context.py` & `py-seal-0.0.8/seal/context/context.py`

 * *Files identical despite different names*

### Comparing `py-seal-0.0.7/seal/db/mysql/base_mapper.py` & `py-seal-0.0.8/seal/db/mysql/base_mapper.py`

 * *Files identical despite different names*

### Comparing `py-seal-0.0.7/seal/db/mysql/chained_query.py` & `py-seal-0.0.8/seal/db/mysql/chained_query.py`

 * *Files identical despite different names*

### Comparing `py-seal-0.0.7/seal/db/mysql/mysql_connector.py` & `py-seal-0.0.8/seal/db/mysql/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `py-seal-0.0.7/seal/db/sqlite/base_mapper.py` & `py-seal-0.0.8/seal/db/sqlite/base_mapper.py`

 * *Files identical despite different names*

### Comparing `py-seal-0.0.7/seal/db/sqlite/chained_query.py` & `py-seal-0.0.8/seal/db/sqlite/chained_query.py`

 * *Files identical despite different names*

### Comparing `py-seal-0.0.7/seal/model/response.py` & `py-seal-0.0.8/seal/model/response.py`

 * *Files identical despite different names*

### Comparing `py-seal-0.0.7/seal/router/router.py` & `py-seal-0.0.8/seal/router/router.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 from functools import wraps
 
 import jwt
 from fastapi import FastAPI, Request, Response, HTTPException, Depends
 from starlette.middleware.cors import CORSMiddleware
 from ..context import WebContext
 from ..model import Response as ResponseModel
+from ..exception import BusinessException
 from .. import get_seal
 
 
 async def verify_token(request: Request = Request):
     if request.method == 'OPTIONS' or request.url.path in ['/login/submit']:
         return None
     try:
         payload = jwt.decode(request.headers['Authorization'],
                              get_seal().get_config('jwt_key'),
                              algorithms=["HS256"])
         WebContext().set({'uid': payload['uid']})
     except Exception as e:
-        print(e)
         raise HTTPException(status_code=401, detail=f"Token is invalid: {e}")
 
 
 app = FastAPI(dependencies=[Depends(verify_token)])
 
 
 @app.middleware("http")
@@ -48,16 +48,21 @@
 async def http_exception_handler(request: Request, exc: HTTPException):
     return Response(status_code=exc.status_code, content=exc.detail)
 
 
 def response_body(func):
     @wraps(func)
     async def wrapper(*args, **kwargs):
-        result = await func(*args, **kwargs)
-        return ResponseModel.build(result).success()
+        try:
+            result = await func(*args, **kwargs)
+            return ResponseModel.build(result).success()
+        except BusinessException as e:
+            return ResponseModel.build().error(message=e.message, code=e.code)
+        except Exception as e:
+            return ResponseModel.build().error(message=str(e))
 
     return wrapper
 
 
 def get(path: str):
     def decorator(func):
         return app.get(path, response_model=ResponseModel)(response_body(func))
```

### Comparing `py-seal-0.0.7/seal/wrapper/entity.py` & `py-seal-0.0.8/seal/wrapper/entity.py`

 * *Files identical despite different names*

### Comparing `py-seal-0.0.7/seal/wrapper/singleton.py` & `py-seal-0.0.8/seal/wrapper/singleton.py`

 * *Files identical despite different names*

