# Comparing `tmp/iaparc_inference-0.0.9.tar.gz` & `tmp/iaparc_inference-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iaparc_inference-0.0.9.tar", last modified: Fri Dec 22 17:59:22 2023, max compression
+gzip compressed data, was "iaparc_inference-0.1.0.tar", last modified: Fri May 31 10:09:28 2024, max compression
```

## Comparing `iaparc_inference-0.0.9.tar` & `iaparc_inference-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-22 17:59:22.558469 iaparc_inference-0.0.9/
--rw-rw-rw-   0 root         (0) root         (0)    11348 2023-12-18 15:12:27.000000 iaparc_inference-0.0.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2924 2023-12-22 17:59:22.558469 iaparc_inference-0.0.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2224 2023-12-21 10:52:01.000000 iaparc_inference-0.0.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)      789 2023-12-18 15:12:27.000000 iaparc_inference-0.0.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-12-22 17:59:22.558469 iaparc_inference-0.0.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-12-18 15:12:27.000000 iaparc_inference-0.0.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-22 17:59:22.554469 iaparc_inference-0.0.9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-22 17:59:22.558469 iaparc_inference-0.0.9/src/iaparc_inference/
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-12-18 15:12:27.000000 iaparc_inference-0.0.9/src/iaparc_inference/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9077 2023-12-18 15:12:27.000000 iaparc_inference-0.0.9/src/iaparc_inference/config.py
--rw-rw-rw-   0 root         (0) root         (0)     9561 2023-12-22 17:58:05.000000 iaparc_inference-0.0.9/src/iaparc_inference/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-22 17:59:22.558469 iaparc_inference-0.0.9/src/iaparc_inference.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2924 2023-12-22 17:59:22.000000 iaparc_inference-0.0.9/src/iaparc_inference.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      356 2023-12-22 17:59:22.000000 iaparc_inference-0.0.9/src/iaparc_inference.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-22 17:59:22.000000 iaparc_inference-0.0.9/src/iaparc_inference.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-12-22 17:59:22.000000 iaparc_inference-0.0.9/src/iaparc_inference.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-12-22 17:59:22.000000 iaparc_inference-0.0.9/src/iaparc_inference.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 10:09:28.878289 iaparc_inference-0.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11348 2024-05-31 10:09:15.000000 iaparc_inference-0.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3416 2024-05-31 10:09:28.878289 iaparc_inference-0.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2024-05-31 10:09:15.000000 iaparc_inference-0.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      789 2024-05-31 10:09:15.000000 iaparc_inference-0.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 10:09:28.878289 iaparc_inference-0.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      147 2024-05-31 10:09:15.000000 iaparc_inference-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 10:09:28.874289 iaparc_inference-0.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 10:09:28.874289 iaparc_inference-0.1.0/src/iaparc_inference/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-31 10:09:15.000000 iaparc_inference-0.1.0/src/iaparc_inference/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6795 2024-05-31 10:09:15.000000 iaparc_inference-0.1.0/src/iaparc_inference/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    10660 2024-05-31 10:09:15.000000 iaparc_inference-0.1.0/src/iaparc_inference/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 10:09:28.878289 iaparc_inference-0.1.0/src/iaparc_inference.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3416 2024-05-31 10:09:28.000000 iaparc_inference-0.1.0/src/iaparc_inference.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      356 2024-05-31 10:09:28.000000 iaparc_inference-0.1.0/src/iaparc_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 10:09:28.000000 iaparc_inference-0.1.0/src/iaparc_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-31 10:09:28.000000 iaparc_inference-0.1.0/src/iaparc_inference.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-31 10:09:28.000000 iaparc_inference-0.1.0/src/iaparc_inference.egg-info/top_level.txt
```

### Comparing `iaparc_inference-0.0.9/LICENSE` & `iaparc_inference-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iaparc_inference-0.0.9/PKG-INFO` & `iaparc_inference-0.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: iaparc_inference
-Version: 0.0.9
-Summary: Inference service package for IAPARC
-Author-email: Bertrand Louargant <blouargant@chapsvision.com>
-Project-URL: Homepage, https://gitlab.com/ia-parc/public/pypi/iaparc_inference
-Project-URL: Issues, https://gitlab.com/ia-parc/public/pypi/iaparc_inference/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: nats-py~=2.6.0
-Requires-Dist: pyyaml~=6.0.1
-Requires-Dist: asyncio~=3.4.3
-Requires-Dist: json-tricks~=3.17.3
-
 # iaparc_inference
 
 
 [![PyPI version](https://badge.fury.io/py/iaparc-inference.svg)](https://badge.fury.io/py/iaparc-inference)
 ![PyPI - License](https://img.shields.io/pypi/l/iaparc-inference)
 
 
@@ -41,16 +23,20 @@
 
     # Define a callback to query your inference pipeline
     # To load your model only once it is recommended to use a class:
     class MyModel:
         def __init__(self, model_path: str):
             ## Load your model in pytorch, tensorflow or any other backend
         
-        def batch_query(batch: list) -> list:
-            ## execute your pipeline on a batch input
+        def batch_query(batch: list, parameters: Optional) -> list:
+            ''' execute your pipeline on a batch input
+                Note:   "parameters" is an optional argument.
+                        It can be used to handle URL's query parameters
+                        It's a list of key(string)/value(string) dictionaries
+            '''
 
     if __name__ == '__main__':
         # Initiate your model class
         my_model = MyModel("path/to/my/model")
 
         # Initiate IAParc listener
         listener = IAPListener(my_model.batch_query)
@@ -65,16 +51,20 @@
 
     # Define a callback to query your inference pipeline
     # To load your model only once it is recommended to use a class:
     class MyModel:
         def __init__(self, model_path: str):
             ## Load your model in pytorch, tensorflow or any other backend
         
-        def single_query(one_input):
-            ## execute your pipeline on a single input
+        def single_query(one_input, parameters: Optional):
+            ''' execute your pipeline on a single input
+                Note:   "parameters" is an optional argument.
+                        It can be used to handle URL's query parameters
+                        It's a key(string)/value(string) dictionary
+            '''
 
     if __name__ == '__main__':
         # Initiate your model class
         my_model = MyModel("path/to/my/model")
 
         # Initiate IAParc listener
         listener = IAPListener(my_model.single_query, batch=1)  # Note that batch size is forced to 1 here
@@ -85,8 +75,8 @@
 * Dynamic batching
 * Autoscalling 
 * Support both synchronous and asynchronous queries
 * Data agnostic
 
 
 ## License
-This project is licensed under the Apache License Version 2.0  - see the Apache [LICENSE](https://www.apache.org/licenses/LICENSE-2.0) file for details.
+This project is licensed under the Apache License Version 2.0  - see the Apache [LICENSE](https://www.apache.org/licenses/LICENSE-2.0) file for details.
```

### Comparing `iaparc_inference-0.0.9/pyproject.toml` & `iaparc_inference-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iaparc_inference-0.0.9/src/iaparc_inference/service.py` & `iaparc_inference-0.1.0/src/iaparc_inference/service.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 IA Parc Inference service
 Support for inference of IA Parc models
 """
 import os
 import io
 import asyncio
 import uuid
+from inspect import signature
 import logging
 import logging.config
 from typing import Tuple
 import nats
 from nats.errors import TimeoutError as NATSTimeoutError
 from json_tricks import dumps, loads
 from iaparc_inference.config import Config
@@ -53,14 +54,21 @@
                         By default determined by the NATS_URL environment variable,
                         however you can orverride it here
         - self.queue:        name of self.queue (default: None)
                         By default determined by the NATS_self.queue environment variable,
                         however you can orverride it here
         """
         self.callback = callback
+        sig = signature(callback)
+        self.callback_args = sig.parameters
+        if len(self.callback_args) != 2:
+            self.callback_has_parameters = False
+        else:
+            self.callback_has_parameters = True
+        
         self.batch = batch
         self.config_path = config_path
         self.url = url
         self.queue = queue
         # Init internal variables
         self._dag = None
         self._input = None
@@ -126,28 +134,33 @@
                                     queue=self.queue+"-"+self.inputs,
                                     stream=self.queue)
         data_store = await js.object_store(bucket=self.queue+"-data")
 
         async def get_data(msg):
             uid = msg.subject[l:]
             source = msg.headers.get("DataSource", "")
+            params_lst = msg.headers.get("Parameters", "")
+            params = {}
+            for p in params_lst.split(","):
+                k, v = p.split("=")
+                params[k] = v
             data = None
             if source == "json":
                 data = loads(msg.data.decode())
             elif source == "object_store":
                 obj_res = await data_store.get(msg.data.decode())
                 data = obj_res.data
             elif source == "file":
                 file = io.BytesIO()
                 obj_res = await data_store.get(msg.data.decode(), file)
                 file.read()
             else:
                 data = msg.data
 
-            return (uid, source, data)
+            return (uid, source, data, params)
 
         async def send_reply(uid, source, data, error=""):
             _out = queue_out + "." + uid
             breply = b''
             if data is not None:
                 match source:
                     case "json":
@@ -163,29 +176,28 @@
                             breply = data
                         else:
                             breply = (str(data)).encode()
             await js.publish(_out, breply, headers={"ProcessError": error, "DataSource": source})
 
         async def handle_msg(msgs, is_batch: bool):
             if is_batch:
-                batch, uids, sources = zip(*[await get_data(msg) for msg in msgs])
+                batch, uids, sources, params_lst = zip(*[await get_data(msg) for msg in msgs])
                 batch = list(batch)
-                reply, err = self._process_data(batch, is_batch)
+                reply, err = self._process_data(batch, is_batch, params_lst)
                 if not err:
                     for data, uid, source in zip(reply, uids, sources):
                         await send_reply(uid, source, data)
                     return
                 for uid, source in zip(uids, sources):
                     await send_reply(uid, source, None, err)
                 return
 
             for msg in msgs:
-                print("handle msg", msg.subject)
-                uid, source, data = await get_data(msg)
-                reply, err = self._process_data([data], is_batch)
+                uid, source, data, params = await get_data(msg)
+                reply, err = self._process_data([data], is_batch, [params])
                 if err:
                     await send_reply(uid, source, reply, err)
                 else:
                     await send_reply(uid, source, reply[0])
                 return
 
         async def term_msg(msgs):
@@ -195,15 +207,14 @@
         # Mark as running
         os.system("touch /tmp/running")
         # Fetch and ack messagess from consumer.
         while True:
             try:
                 pending_msgs = sub_in.pending_msgs
                 if self.batch == 1 or pending_msgs == 0:
-                    print("waiting for messages")
                     msg = await sub_in.next_msg(timeout=600)
                     await asyncio.gather(
                         handle_msg([msg], False),
                         term_msg([msg])
                     )
                 else:
                     if pending_msgs >= self.batch:
@@ -238,31 +249,48 @@
                 continue
             except Exception as e: # pylint: disable=W0703
                 LOGGER.error("Fatal error message handler: %s",
                              str(e), exc_info=True)
                 break
         await nc.close()
 
-    def _process_data(self, requests: list, is_batch: bool = False) -> Tuple[list, str | None]:
+    def _process_data(self, requests: list, reqs_parameters: list, is_batch: bool = False) -> Tuple[list, str | None]:
         """
         Process data
         Arguments:
         - requests:   list of data to process
         - is_batch:   is batched data
         Returns:
         - Tuple[List[bytes], str]:  list of processed data and error message
         """
         try:
             LOGGER.debug("handle request")
-            result = self.callback(requests)
+            
             if is_batch:
-                if not isinstance(result, list):
+                if self.callback_has_parameters:
+                    result = self.callback(requests, reqs_parameters)
+                else:
+                    result = self.callback(requests)
+                if not isinstance(result, list):    
                     return [], "batch reply is not a list"
                 if len(requests) != len(result):
                     return [], "batch reply has wrong size"
+            else:
+                if len(requests) == 0:
+                    request = []
+                else:
+                    request = requests[0]
+                if len(reqs_parameters) == 0:
+                    parameters = {}
+                else:
+                    parameters = reqs_parameters[0]
+                if self.callback_has_parameters:
+                    result = self.callback(request, parameters)
+                else:
+                    result = self.callback(request)
             return result, None
         except ValueError:
             LOGGER.error("Fatal error message handler", exc_info=True)
             return [], "Wrong input"
         except Exception as e: # pylint: disable=W0703
             LOGGER.error("Fatal error message handler", exc_info=True)
             return [], str(e)
```

### Comparing `iaparc_inference-0.0.9/src/iaparc_inference.egg-info/PKG-INFO` & `iaparc_inference-0.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: iaparc-inference
-Version: 0.0.9
+Name: iaparc_inference
+Version: 0.1.0
 Summary: Inference service package for IAPARC
 Author-email: Bertrand Louargant <blouargant@chapsvision.com>
 Project-URL: Homepage, https://gitlab.com/ia-parc/public/pypi/iaparc_inference
 Project-URL: Issues, https://gitlab.com/ia-parc/public/pypi/iaparc_inference/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -41,16 +41,20 @@
 
     # Define a callback to query your inference pipeline
     # To load your model only once it is recommended to use a class:
     class MyModel:
         def __init__(self, model_path: str):
             ## Load your model in pytorch, tensorflow or any other backend
         
-        def batch_query(batch: list) -> list:
-            ## execute your pipeline on a batch input
+        def batch_query(batch: list, parameters: Optional) -> list:
+            ''' execute your pipeline on a batch input
+                Note:   "parameters" is an optional argument.
+                        It can be used to handle URL's query parameters
+                        It's a list of key(string)/value(string) dictionaries
+            '''
 
     if __name__ == '__main__':
         # Initiate your model class
         my_model = MyModel("path/to/my/model")
 
         # Initiate IAParc listener
         listener = IAPListener(my_model.batch_query)
@@ -65,16 +69,20 @@
 
     # Define a callback to query your inference pipeline
     # To load your model only once it is recommended to use a class:
     class MyModel:
         def __init__(self, model_path: str):
             ## Load your model in pytorch, tensorflow or any other backend
         
-        def single_query(one_input):
-            ## execute your pipeline on a single input
+        def single_query(one_input, parameters: Optional):
+            ''' execute your pipeline on a single input
+                Note:   "parameters" is an optional argument.
+                        It can be used to handle URL's query parameters
+                        It's a key(string)/value(string) dictionary
+            '''
 
     if __name__ == '__main__':
         # Initiate your model class
         my_model = MyModel("path/to/my/model")
 
         # Initiate IAParc listener
         listener = IAPListener(my_model.single_query, batch=1)  # Note that batch size is forced to 1 here
```

