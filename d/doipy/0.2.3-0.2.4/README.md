# Comparing `tmp/doipy-0.2.3.tar.gz` & `tmp/doipy-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doipy-0.2.3.tar", max compression
+gzip compressed data, was "doipy-0.2.4.tar", max compression
```

## Comparing `doipy-0.2.3.tar` & `doipy-0.2.4.tar`

### file list

```diff
@@ -1,11 +1,21 @@
--rw-r--r--   0        0        0     2306 2024-03-16 06:28:14.439402 doipy-0.2.3/README.md
--rw-r--r--   0        0        0      227 2024-03-15 20:23:37.354806 doipy-0.2.3/doipy/__init__.py
--rw-r--r--   0        0        0       34 2024-02-26 18:50:55.433868 doipy-0.2.3/doipy/__main__.py
--rw-r--r--   0        0        0     7095 2024-03-17 19:15:47.831946 doipy-0.2.3/doipy/actions.py
--rw-r--r--   0        0        0      327 2024-03-18 09:30:05.899471 doipy-0.2.3/doipy/config.py
--rw-r--r--   0        0        0       86 2024-03-11 14:42:17.492230 doipy-0.2.3/doipy/fdo_config.py
--rw-r--r--   0        0        0     3836 2024-03-17 19:15:47.835409 doipy-0.2.3/doipy/main.py
--rw-r--r--   0        0        0     2437 2024-03-17 19:09:11.542479 doipy-0.2.3/doipy/server.py
--rw-r--r--   0        0        0     1608 2024-03-17 19:05:27.799235 doipy-0.2.3/doipy/socket_utils.py
--rw-r--r--   0        0        0      754 2024-03-18 09:30:57.074571 doipy-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3143 1970-01-01 00:00:00.000000 doipy-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     3523 2024-05-30 14:40:10.577307 doipy-0.2.4/README.md
+-rw-r--r--   0        0        0      327 2024-05-30 14:45:32.253535 doipy-0.2.4/doipy/__init__.py
+-rw-r--r--   0        0        0       34 2024-02-26 13:59:23.359455 doipy-0.2.4/doipy/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-30 14:40:10.577537 doipy-0.2.4/doipy/actions/__init__.py
+-rw-r--r--   0        0        0      164 2024-05-30 14:47:47.115322 doipy-0.2.4/doipy/actions/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     1516 2024-05-30 14:47:47.119089 doipy-0.2.4/doipy/actions/__pycache__/cordra.cpython-312.pyc
+-rw-r--r--   0        0        0     5465 2024-05-30 14:47:47.772589 doipy-0.2.4/doipy/actions/__pycache__/doip.cpython-312.pyc
+-rw-r--r--   0        0        0     2915 2024-05-30 14:50:55.953016 doipy-0.2.4/doipy/actions/__pycache__/fdo.cpython-312.pyc
+-rw-r--r--   0        0        0      907 2024-05-30 14:40:10.578604 doipy-0.2.4/doipy/actions/cordra.py
+-rw-r--r--   0        0        0     5489 2024-05-30 14:40:10.579232 doipy-0.2.4/doipy/actions/doip.py
+-rw-r--r--   0        0        0     2518 2024-05-30 14:50:28.688405 doipy-0.2.4/doipy/actions/fdo.py
+-rw-r--r--   0        0        0      331 2024-04-24 15:51:39.654431 doipy-0.2.4/doipy/config.py
+-rw-r--r--   0        0        0     1179 2024-05-14 12:29:25.337054 doipy-0.2.4/doipy/constants.py
+-rw-r--r--   0        0        0      104 2024-05-30 14:40:10.584039 doipy-0.2.4/doipy/exceptions.py
+-rw-r--r--   0        0        0     2443 2024-05-30 14:40:10.585134 doipy-0.2.4/doipy/input_schema.py
+-rw-r--r--   0        0        0     5818 2024-05-30 14:44:11.049171 doipy-0.2.4/doipy/main.py
+-rw-r--r--   0        0        0     1544 2024-05-30 14:40:10.586690 doipy-0.2.4/doipy/models.py
+-rw-r--r--   0        0        0     2399 2024-05-08 09:19:51.610399 doipy-0.2.4/doipy/server.py
+-rw-r--r--   0        0        0     2292 2024-05-08 09:19:51.611712 doipy-0.2.4/doipy/socket_utils.py
+-rw-r--r--   0        0        0      860 2024-05-31 09:48:15.210555 doipy-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 doipy-0.2.4/PKG-INFO
```

### Comparing `doipy-0.2.3/doipy/server.py` & `doipy-0.2.4/doipy/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,46 +23,45 @@
         with context.wrap_socket(sock, server_side=True) as ssock:
             print('Wait for connection')
             while True:
                 conn, addr = ssock.accept()
                 print('Connected by', addr)
                 request = json.loads(conn.recv(8192))
                 print(request)
-                data2 = conn.recv(8192)
-                data2 = conn.recv(8192)
+                # data2 = conn.recv(8192)
                 if request['operationId'] == '0.DOIP/Op.Hello':
                     doip_hello(conn, port)
                 elif request['operationId'] == '0.DOIP/Op.ListOperations':
                     doip_list_operations(conn)
                 else:
                     not_implemented(conn, request['operationId'])
                 conn.close()
 
 
 def doip_list_operations(conn: object):
     message = {
-        "status": "0.DOIP/Status.001",
-        "output": [
-            "0.DOIP/Op.Hello",
-            "0.DOIP/Op.ListOperations",
+        'status': '0.DOIP/Status.001',
+        'output': [
+            '0.DOIP/Op.Hello',
+            '0.DOIP/Op.ListOperations',
         ]
     }
     send_server_message(message, conn)
 
 
 def doip_hello(conn: object, port: int):
-    message = {"status": "0.DOIP/Status.001",
-               "output": {
-                   "id": "doip-server-1",
-                   "type": "0.TYPE/DOIPServiceInfo",
-                   "attributes": {
-                       "ipAddress": "0.0.0.0",
-                       "port": port,
-                       "protocol": "TCP",
-                       "protocolVersion": "2.0"
+    message = {'status': '0.DOIP/Status.001',
+               'output': {
+                   'id': 'doip-server-1',
+                   'type': '0.TYPE/DOIPServiceInfo',
+                   'attributes': {
+                       'ipAddress': '0.0.0.0',
+                       'port': port,
+                       'protocol': 'TCP',
+                       'protocolVersion': '2.0'
                    }
                }
                }
     print('send reply')
     send_server_message(message, conn)
```

### Comparing `doipy-0.2.3/pyproject.toml` & `doipy-0.2.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "doipy"
-version = "0.2.3"
+version = "0.2.4"
 description = "A Python wrapper for DOIP."
 authors = [
     "Triet Doan <triet.doan@gwdg.de>",
     "Sven Bingert <sven.bingert@gwdg.de>"
 ]
 readme = "README.md"
 
@@ -15,20 +15,25 @@
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [tool.poetry.scripts]
 doipy = "doipy.main:app"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.11"
 typer = {extras = ["all"], version = "^0.9.0"}
 rich = "^13.7.0"
 pydantic = "^2.6.3"
 pydantic-settings = "^2.2.1"
+jsonschema = "^4.22.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.2"
+pytest-mock = "^3.14.0"
+pytest-cov = "^5.0.0"
+flake8 = "^7.0.0"
+pylint = "^3.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

