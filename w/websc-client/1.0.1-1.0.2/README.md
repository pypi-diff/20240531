# Comparing `tmp/websc_client-1.0.1.tar.gz` & `tmp/websc_client-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "websc_client-1.0.1.tar", last modified: Wed May 29 21:41:22 2024, max compression
+gzip compressed data, was "websc_client-1.0.2.tar", last modified: Fri May 31 06:33:39 2024, max compression
```

## Comparing `websc_client-1.0.1.tar` & `websc_client-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-05-29 21:41:22.777395 websc_client-1.0.1/
--rw-r--r--   0 hell      (1000) hell      (1000)     2080 2024-05-29 21:41:22.777395 websc_client-1.0.1/PKG-INFO
--rw-rw-r--   0 hell      (1000) hell      (1000)     1581 2024-05-29 20:54:27.000000 websc_client-1.0.1/README.md
--rw-rw-r--   0 hell      (1000) hell      (1000)      512 2024-05-29 21:40:33.000000 websc_client-1.0.1/pyproject.toml
--rw-rw-r--   0 hell      (1000) hell      (1000)       38 2024-05-29 21:41:22.777395 websc_client-1.0.1/setup.cfg
-drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-05-29 21:41:22.777395 websc_client-1.0.1/websc_client/
--rw-rw-r--   0 hell      (1000) hell      (1000)       84 2024-05-29 21:40:33.000000 websc_client-1.0.1/websc_client/__init__.py
--rw-rw-r--   0 hell      (1000) hell      (1000)     4144 2024-05-29 20:54:27.000000 websc_client-1.0.1/websc_client/client.py
--rw-rw-r--   0 hell      (1000) hell      (1000)     4068 2024-05-29 21:22:12.000000 websc_client-1.0.1/websc_client/websc.py
-drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-05-29 21:41:22.777395 websc_client-1.0.1/websc_client.egg-info/
--rw-r--r--   0 hell      (1000) hell      (1000)     2080 2024-05-29 21:41:22.000000 websc_client-1.0.1/websc_client.egg-info/PKG-INFO
--rw-rw-r--   0 hell      (1000) hell      (1000)      273 2024-05-29 21:41:22.000000 websc_client-1.0.1/websc_client.egg-info/SOURCES.txt
--rw-rw-r--   0 hell      (1000) hell      (1000)        1 2024-05-29 21:41:22.000000 websc_client-1.0.1/websc_client.egg-info/dependency_links.txt
--rw-rw-r--   0 hell      (1000) hell      (1000)       17 2024-05-29 21:41:22.000000 websc_client-1.0.1/websc_client.egg-info/requires.txt
--rw-rw-r--   0 hell      (1000) hell      (1000)       13 2024-05-29 21:41:22.000000 websc_client-1.0.1/websc_client.egg-info/top_level.txt
+drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-05-31 06:33:39.804592 websc_client-1.0.2/
+-rw-r--r--   0 hell      (1000) hell      (1000)     2080 2024-05-31 06:33:39.804592 websc_client-1.0.2/PKG-INFO
+-rw-rw-r--   0 hell      (1000) hell      (1000)     1581 2024-05-29 20:54:27.000000 websc_client-1.0.2/README.md
+-rw-rw-r--   0 hell      (1000) hell      (1000)      512 2024-05-31 06:29:55.000000 websc_client-1.0.2/pyproject.toml
+-rw-rw-r--   0 hell      (1000) hell      (1000)       38 2024-05-31 06:33:39.804592 websc_client-1.0.2/setup.cfg
+drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-05-31 06:33:39.804592 websc_client-1.0.2/websc_client/
+-rw-rw-r--   0 hell      (1000) hell      (1000)       84 2024-05-31 06:29:55.000000 websc_client-1.0.2/websc_client/__init__.py
+-rw-rw-r--   0 hell      (1000) hell      (1000)     4267 2024-05-31 06:29:55.000000 websc_client-1.0.2/websc_client/client.py
+-rw-rw-r--   0 hell      (1000) hell      (1000)      162 2024-05-31 06:29:55.000000 websc_client-1.0.2/websc_client/exceptions.py
+-rw-rw-r--   0 hell      (1000) hell      (1000)     4276 2024-05-31 06:29:55.000000 websc_client-1.0.2/websc_client/websc.py
+drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-05-31 06:33:39.804592 websc_client-1.0.2/websc_client.egg-info/
+-rw-r--r--   0 hell      (1000) hell      (1000)     2080 2024-05-31 06:33:39.000000 websc_client-1.0.2/websc_client.egg-info/PKG-INFO
+-rw-rw-r--   0 hell      (1000) hell      (1000)      300 2024-05-31 06:33:39.000000 websc_client-1.0.2/websc_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 hell      (1000) hell      (1000)        1 2024-05-31 06:33:39.000000 websc_client-1.0.2/websc_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 hell      (1000) hell      (1000)       17 2024-05-31 06:33:39.000000 websc_client-1.0.2/websc_client.egg-info/requires.txt
+-rw-rw-r--   0 hell      (1000) hell      (1000)       13 2024-05-31 06:33:39.000000 websc_client-1.0.2/websc_client.egg-info/top_level.txt
```

### Comparing `websc_client-1.0.1/PKG-INFO` & `websc_client-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: websc-client
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for communicate with websc
 Author-email: Patrik Kratochvil <info@ledsc.eu>
 Project-URL: homepage, https://ledsc.eu/websc/
 Project-URL: repository, https://gitlab.com/ledsc/websclient
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `websc_client-1.0.1/README.md` & `websc_client-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `websc_client-1.0.1/pyproject.toml` & `websc_client-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "websc-client"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Patrik Kratochvil", email="info@ledsc.eu" },
 ]
 description = "Library for communicate with websc"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `websc_client-1.0.1/websc_client/client.py` & `websc_client-1.0.2/websc_client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 """
 import asyncio
 import logging
 import json
 
 import websockets as websocket
 from websockets import WebSocketClientProtocol
-from websockets.exceptions import ConnectionClosedOK
+from websockets.exceptions import ConnectionClosedOK, WebSocketException
+
+from .exceptions import WebSClientConnectionError
 from .websc import WebSCAsync, WebSClientAsyncTemplate
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class WebSClientAsync(WebSClientAsyncTemplate):
     def __init__(self, host: str, port: int):
@@ -26,21 +28,21 @@
         """
         Connect to WebSC.
 
         Read configuration from initial message and create LedSC devices.
         Create background task for websocket listening.
         """
         if self._client is not None and not self._client.closed:
-            raise ConnectionError(f"LedSClient: Already connected to {self.host}:{self.port}")
+            raise WebSClientConnectionError(f"LedSClient: Already connected to {self.host}:{self.port}")
         _LOGGER.debug(f"LedSClient: Connecting to %s:%s", self.host, self.port)
 
         try:
             self._client = await websocket.connect(f"ws://{self.host}:{self.port}", open_timeout=2)
-        except OSError as E:
-            raise ConnectionError(
+        except (OSError, WebSocketException) as E:
+            raise WebSClientConnectionError(
                 f"LedSClient: Could not connect to websocket at {self.host}:{self.port}"
             ) from E
         _LOGGER.info(f"LedSClient: Connected to %s:%s", self.host, self.port)
         initial_message = json.loads(await self._client.recv())
 
         if "dev" in initial_message:
             for name, data in initial_message["dev"].items():
@@ -82,15 +84,15 @@
                     _LOGGER.warning("LedSClient: Connection closed. Reconnecting...")
                     for device in self.devices.values():
                         await device.data({"is_lost": 1})
                     while self._client.closed:
                         try:
                             await self.connect()
                             await asyncio.sleep(1)
-                        except ConnectionError:
+                        except WebSClientConnectionError:
                             await asyncio.sleep(5)
         finally:
             self._observer_running = False
             await self.disconnect()
 
     async def disconnect(self) -> None:
         """ Disconnect from WebSC """
```

### Comparing `websc_client-1.0.1/websc_client/websc.py` & `websc_client-1.0.2/websc_client/websc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import inspect
 from typing import Callable, Coroutine
 
+from websc_client.exceptions import WebSClientCallbackError
+
 
 class WebSClientAsyncTemplate:
     def __init__(self, host: str, port: int):
         self.devices: dict[str, WebSCAsync] = {}
         self.host = host
         self.port = port
 
@@ -51,15 +53,18 @@
         """
         self.callback_data_change = callback
 
     async def data(self, value: dict):
         """ For update data. This data must be received from WebSC """
         self._data.update(value)
         if self.callback_data_change:
-            await self.callback_data_change(value)
+            try:
+                await self.callback_data_change(value)
+            except Exception as E:
+                raise WebSClientCallbackError(f"Error in registered callback: {E}") from E
 
     async def send(self, data: dict):
         """ Marks the message with identifying characters and sends. """
         await self.client.send({'dev': {self.name: data}})
 
     async def set_red(self, value: int):
         await self.send({"R": value})
```

### Comparing `websc_client-1.0.1/websc_client.egg-info/PKG-INFO` & `websc_client-1.0.2/websc_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: websc-client
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for communicate with websc
 Author-email: Patrik Kratochvil <info@ledsc.eu>
 Project-URL: homepage, https://ledsc.eu/websc/
 Project-URL: repository, https://gitlab.com/ledsc/websclient
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

