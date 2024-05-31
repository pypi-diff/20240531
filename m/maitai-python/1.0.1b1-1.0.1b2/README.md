# Comparing `tmp/maitai_python-1.0.1b1.tar.gz` & `tmp/maitai_python-1.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maitai_python-1.0.1b1.tar", last modified: Thu May 30 21:32:37 2024, max compression
+gzip compressed data, was "maitai_python-1.0.1b2.tar", last modified: Fri May 31 19:24:41 2024, max compression
```

## Comparing `maitai_python-1.0.1b1.tar` & `maitai_python-1.0.1b2.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.672278 maitai_python-1.0.1b1/
--rw-r--r--   0 runner    (1001) runner    (1001)     1721 2024-05-30 21:32:37.672278 maitai_python-1.0.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)     1215 2024-05-30 21:32:04.000000 maitai_python-1.0.1b1/README.md
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.664278 maitai_python-1.0.1b1/maitai/
--rw-r--r--   0 runner    (1001) runner    (1001)      459 2024-05-30 21:32:04.000000 maitai_python-1.0.1b1/maitai/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2249 2024-05-30 21:32:04.000000 maitai_python-1.0.1b1/maitai/_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)      495 2024-05-30 21:32:04.000000 maitai_python-1.0.1b1/maitai/_config_listener_thread.py
--rw-r--r--   0 runner    (1001) runner    (1001)    12978 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai/_evaluator.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4659 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai/_inference.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1135 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai/_maitai_client.py
--rw-r--r--   0 runner    (1001) runner    (1001)    16039 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai/_openai.py
--rw-r--r--   0 runner    (1001) runner    (1001)      236 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai/_openai_types.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1307 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai/_types.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4243 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai/_utils.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.664278 maitai_python-1.0.1b1/maitai_common/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_common/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.664278 maitai_python-1.0.1b1/maitai_common/processes/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_common/processes/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1977 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_common/processes/io_thread.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3392 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_common/processes/websocket_listener_thread.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.668278 maitai_python-1.0.1b1/maitai_common/utils/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_common/utils/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      407 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_common/utils/proto_utils.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.668278 maitai_python-1.0.1b1/maitai_gen/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_gen/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.668278 maitai_python-1.0.1b1/maitai_gen/application/
--rw-r--r--   0 runner    (1001) runner    (1001)     1364 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_gen/application/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.668278 maitai_python-1.0.1b1/maitai_gen/chat/
--rw-r--r--   0 runner    (1001) runner    (1001)     9847 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_gen/chat/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.668278 maitai_python-1.0.1b1/maitai_gen/company/
--rw-r--r--   0 runner    (1001) runner    (1001)      641 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_gen/company/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.668278 maitai_python-1.0.1b1/maitai_gen/inference/
--rw-r--r--   0 runner    (1001) runner    (1001)      600 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_gen/inference/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.668278 maitai_python-1.0.1b1/maitai_gen/notification/
--rw-r--r--   0 runner    (1001) runner    (1001)     1198 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_gen/notification/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.668278 maitai_python-1.0.1b1/maitai_gen/sandbox/
--rw-r--r--   0 runner    (1001) runner    (1001)     1460 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_gen/sandbox/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.668278 maitai_python-1.0.1b1/maitai_gen/sentinel/
--rw-r--r--   0 runner    (1001) runner    (1001)     1518 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_gen/sentinel/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.668278 maitai_python-1.0.1b1/maitai_gen/session/
--rw-r--r--   0 runner    (1001) runner    (1001)      886 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_gen/session/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.672278 maitai_python-1.0.1b1/maitai_python.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)     1721 2024-05-30 21:32:37.000000 maitai_python-1.0.1b1/maitai_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      915 2024-05-30 21:32:37.000000 maitai_python-1.0.1b1/maitai_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-05-30 21:32:37.000000 maitai_python-1.0.1b1/maitai_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       70 2024-05-30 21:32:37.000000 maitai_python-1.0.1b1/maitai_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       32 2024-05-30 21:32:37.000000 maitai_python-1.0.1b1/maitai_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-05-30 21:32:37.672278 maitai_python-1.0.1b1/setup.cfg
--rw-r--r--   0 runner    (1001) runner    (1001)      764 2024-05-30 21:32:24.000000 maitai_python-1.0.1b1/setup.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-31 19:24:41.892221 maitai_python-1.0.1b2/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1721 2024-05-31 19:24:41.892221 maitai_python-1.0.1b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)     1215 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/README.md
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-31 19:24:41.884221 maitai_python-1.0.1b2/maitai/
+-rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2249 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai/_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      495 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai/_config_listener_thread.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13120 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai/_evaluator.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5946 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai/_inference.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1135 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai/_maitai_client.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10429 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai/_openai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10729 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai/_openai_async.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      236 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai/_openai_types.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2324 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai/_types.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10243 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai/_utils.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-31 19:24:41.884221 maitai_python-1.0.1b2/maitai_common/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai_common/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-31 19:24:41.884221 maitai_python-1.0.1b2/maitai_common/processes/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai_common/processes/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1977 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai_common/processes/io_thread.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3392 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai_common/processes/websocket_listener_thread.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-31 19:24:41.884221 maitai_python-1.0.1b2/maitai_common/utils/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai_common/utils/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      407 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai_common/utils/proto_utils.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-31 19:24:41.884221 maitai_python-1.0.1b2/maitai_gen/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai_gen/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-31 19:24:41.888221 maitai_python-1.0.1b2/maitai_gen/application/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1364 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai_gen/application/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-31 19:24:41.888221 maitai_python-1.0.1b2/maitai_gen/chat/
+-rw-r--r--   0 runner    (1001) runner    (1001)     9847 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai_gen/chat/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-31 19:24:41.888221 maitai_python-1.0.1b2/maitai_gen/company/
+-rw-r--r--   0 runner    (1001) runner    (1001)      641 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai_gen/company/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-31 19:24:41.888221 maitai_python-1.0.1b2/maitai_gen/inference/
+-rw-r--r--   0 runner    (1001) runner    (1001)      600 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai_gen/inference/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-31 19:24:41.888221 maitai_python-1.0.1b2/maitai_gen/notification/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1198 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai_gen/notification/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-31 19:24:41.888221 maitai_python-1.0.1b2/maitai_gen/sandbox/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1460 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai_gen/sandbox/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-31 19:24:41.888221 maitai_python-1.0.1b2/maitai_gen/sentinel/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1518 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai_gen/sentinel/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-31 19:24:41.888221 maitai_python-1.0.1b2/maitai_gen/session/
+-rw-r--r--   0 runner    (1001) runner    (1001)      886 2024-05-31 19:24:10.000000 maitai_python-1.0.1b2/maitai_gen/session/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-31 19:24:41.892221 maitai_python-1.0.1b2/maitai_python.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1721 2024-05-31 19:24:41.000000 maitai_python-1.0.1b2/maitai_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      939 2024-05-31 19:24:41.000000 maitai_python-1.0.1b2/maitai_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-05-31 19:24:41.000000 maitai_python-1.0.1b2/maitai_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       70 2024-05-31 19:24:41.000000 maitai_python-1.0.1b2/maitai_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       32 2024-05-31 19:24:41.000000 maitai_python-1.0.1b2/maitai_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-05-31 19:24:41.892221 maitai_python-1.0.1b2/setup.cfg
+-rw-r--r--   0 runner    (1001) runner    (1001)      764 2024-05-31 19:24:29.000000 maitai_python-1.0.1b2/setup.py
```

### Comparing `maitai_python-1.0.1b1/PKG-INFO` & `maitai_python-1.0.1b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maitai-python
-Version: 1.0.1b1
+Version: 1.0.1b2
 Summary: MaiTai SDK for Python
 Home-page: https://docs.trymaitai.ai
 Author: Maitai
 Author-email: support@trymaitai.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `maitai_python-1.0.1b1/README.md` & `maitai_python-1.0.1b2/README.md`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b1/maitai/_config.py` & `maitai_python-1.0.1b2/maitai/_config.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b1/maitai/_evaluator.py` & `maitai_python-1.0.1b2/maitai/_evaluator.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,45 +7,55 @@
 
 from maitai._config import config
 from maitai._maitai_client import MaiTaiClient
 from maitai._types import EvaluateCallback
 from maitai_gen.chat import EvaluateRequest, EvaluateResponse, EvaluationContentType
 
 
+def _get_content_type(content):
+    if isinstance(content, str):
+        return EvaluationContentType.TEXT
+    elif isinstance(content, list):
+        return EvaluationContentType.MESSAGE
+
+
 class Evaluator(MaiTaiClient):
 
     def __init__(self):
         super().__init__()
 
     @classmethod
-    def evaluate_with_callback(cls, session_id, reference_id, action_type, content_type, content, application_id=None,
-                               application_ref_name=None, callback=None):
-        if application_id is None and application_ref_name is None:
-            raise Exception('application_id or application_ref_name must be provided')
-        eval_request: EvaluateRequest = cls.create_eval_request(application_id, application_ref_name, session_id,
-                                                                reference_id, action_type, content_type, content)
-        cls.run_async(cls.send_evaluation_request_async(eval_request, callback))
-
-    @classmethod
-    async def evaluate_async(cls, session_id, reference_id, action_type, content_type, content, application_id=None,
-                             application_ref_name=None):
-        if application_id is None and application_ref_name is None:
-            raise Exception('application_id or application_ref_name must be provided')
-        eval_request: EvaluateRequest = cls.create_eval_request(application_id, application_ref_name, session_id,
-                                                                reference_id, action_type, content_type, content)
-        return await cls.send_evaluation_request_async(eval_request)
-
-    @classmethod
-    def evaluate(cls, session_id, reference_id, action_type, content_type, content, application_id=None,
-                 application_ref_name=None):
-        if application_id is None and application_ref_name is None:
-            raise Exception('application_id or application_ref_name must be provided')
-        eval_request: EvaluateRequest = cls.create_eval_request(application_id, application_ref_name, session_id,
-                                                                reference_id, action_type, content_type, content)
-        return cls.send_evaluation_request(eval_request)
+    async def evaluate_async(cls, session_id, reference_id, action_type, content, content_type=None, application_id=None, application_ref_name=None, callback=None):
+        if content_type is None:
+            content_type = _get_content_type(content)
+        if content_type is None:
+            raise Exception('Unable to automatically determine content_type')
+        if application_id is None and application_ref_name is None:
+            raise Exception('application_id or application_ref_name must be provided')
+        eval_request: EvaluateRequest = cls.create_eval_request(application_id, application_ref_name, session_id, reference_id, action_type, content_type, content)
+        if callback is None:
+            return await cls.send_evaluation_request_async(eval_request)
+        else:
+            cls.run_async(cls.send_evaluation_request_async(eval_request, callback))
+            return None
+
+    @classmethod
+    def evaluate(cls, session_id, reference_id, action_type, content, content_type=None, application_id=None, application_ref_name=None, callback=None):
+        if content_type is None:
+            content_type = _get_content_type(content)
+        if content_type is None:
+            raise Exception('Unable to automatically determine content_type')
+        if application_id is None and application_ref_name is None:
+            raise Exception('application_id or application_ref_name must be provided')
+        eval_request: EvaluateRequest = cls.create_eval_request(application_id, application_ref_name, session_id, reference_id, action_type, content_type, content)
+        if callback is None:
+            return cls.send_evaluation_request(eval_request)
+        else:
+            cls.run_async(cls.send_evaluation_request_async(eval_request, callback))
+            return None
 
     @classmethod
     def create_eval_request(cls, application_id, application_ref_name, session_id, reference_id, action_type,
                             content_type, content):
         eval_request: EvaluateRequest = EvaluateRequest()
         eval_request.evaluation_content_type = content_type
         if content_type == EvaluationContentType.TEXT:
@@ -139,14 +149,16 @@
                     return await response.read()
 
         result = await send_request()
         if result is not None:
             eval_result = EvaluateResponse().from_json(result)
             if callback is not None:
                 callback(eval_result)
+            else:
+                return eval_result
 
     @classmethod
     def send_evaluation_request(cls, eval_request: EvaluateRequest) -> EvaluateResponse:
         start = time.time()
 
         def send_request():
             host = config.maitai_host
```

### Comparing `maitai_python-1.0.1b1/maitai/_maitai_client.py` & `maitai_python-1.0.1b2/maitai/_maitai_client.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b1/maitai/_openai.py` & `maitai_python-1.0.1b2/maitai/_openai_async.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,72 +1,75 @@
-from typing import Dict, Iterable, List, Mapping, Optional, Union
+from typing import AsyncIterable, Dict, Iterable, List, Mapping, Optional, Union
 
 import httpx
 import openai
 import openai.types as openai_types
 import openai.types.chat as openai_chat_types
 
 import maitai
 from maitai._config import config
 from maitai._openai_types import Body, Headers, Query
 from maitai._types import EvaluateCallback
-from maitai._utils import convert_open_ai_chat_completion_chunk, convert_openai_chat_completion, required_args, set_chunk_evaluation_response, set_completion_evaluation_response
+from maitai._utils import convert_open_ai_chat_completion_chunk, convert_openai_chat_completion, get_chat_completion_params, process_chunk, process_stream_response, required_args, \
+    set_completion_evaluation_response
 from maitai_common.utils.proto_utils import openai_messages_to_proto
-from maitai_gen.chat import ChatCompletionChunk, ChatCompletionParams, ChatCompletionResponse, ChatMessage, EvaluationContentType, Function, ResponseFormat, StreamOptions, Tool
+from maitai_gen.chat import ChatCompletionChunk, ChatCompletionResponse, ChatMessage, EvaluationContentType
 from maitai_gen.inference import InferenceStreamResponse
 
 DEFAULT_MAX_RETRIES = 2
 
 
-class MaiTaiOpenAIClient:
+class MaiTaiAsyncOpenAIClient:
     def __init__(
         self,
         *,
         maitai_api_key: Optional[str] = None,
         api_key: Optional[str] = None,
         organization: Optional[str] = None,
         project: Optional[str] = None,
         base_url: Union[str, httpx.URL, None] = None,
         timeout: Union[float, httpx.Timeout, None, openai.NotGiven] = openai.NOT_GIVEN,
         max_retries: int = DEFAULT_MAX_RETRIES,
         default_headers: Optional[Mapping[str, str]] = None,
         default_query: Optional[Mapping[str, object]] = None,
         http_client: Optional[httpx.Client] = None,
         _strict_response_validation: bool = False,
+
     ):
         if maitai_api_key:
             config.initialize(maitai_api_key)
-        self.client = openai.OpenAI(
+        self.client = openai.AsyncClient(
             api_key=api_key,
             organization=organization,
             project=project,
             base_url=base_url,
             timeout=timeout,
             max_retries=max_retries,
             default_headers=default_headers,
             default_query=default_query,
             http_client=http_client,
         )
-        self.chat = Chat(self.client)
+
+        self.chat = AsyncChat(self.client)
 
 
-class Chat:
+class AsyncChat:
     def __init__(self, client=None):
-        self.completions = Completions(client)
+        self.completions = AsyncCompletions(client)
 
 
-class Completions:
-    def __init__(self, client: Optional[openai.Client] = None):
+class AsyncCompletions:
+    def __init__(self, client: Optional[openai.AsyncClient] = None):
         if client is None:
-            client = openai.OpenAI()
+            client = openai.AsyncClient()
         self.client = client
 
     @required_args(["session_id", "action_type", "application_ref_name", "messages", "model"],
                    ["session_id", "action_type", "application_ref_name", "messages", "model", "stream"])
-    def create(
+    async def create(
         self,
         *,
         # Maitai Arguments
         session_id: Union[str, int] = None,
         reference_id: Union[str, int, None] = None,
         action_type: str = None,
         application_ref_name: str = None,
@@ -94,15 +97,15 @@
         top_logprobs: Union[Optional[int], openai.NotGiven] = openai.NOT_GIVEN,
         top_p: Union[Optional[float], openai.NotGiven] = openai.NOT_GIVEN,
         user: Union[str, openai.NotGiven] = openai.NOT_GIVEN,
         extra_headers: Optional[Headers] = None,
         extra_query: Optional[Query] = None,
         extra_body: Optional[Body] = None,
         timeout: Union[float, httpx.Timeout, None, openai.NotGiven] = openai.NOT_GIVEN,
-    ) -> Union[ChatCompletionResponse, Iterable[ChatCompletionChunk]]:
+    ) -> Union[ChatCompletionResponse, AsyncIterable[ChatCompletionChunk]]:
         if not config.api_key:
             raise ValueError("Maitai API Key has not been set")
         if server_side_inference:
             completion_params = get_chat_completion_params(
                 messages=messages,
                 model=model,
                 frequency_penalty=frequency_penalty,
@@ -122,31 +125,31 @@
                 top_logprobs=top_logprobs,
                 top_p=top_p,
                 user=user,
             )
             response_timeout = None
             if isinstance(timeout, float) or isinstance(timeout, int):
                 response_timeout = timeout
-            response = maitai.Inference.infer(session_id, reference_id, action_type, application_ref_name, completion_params, callback, timeout=response_timeout)
+            response = await maitai.Inference.infer_async(session_id, reference_id, action_type, application_ref_name, completion_params, callback, timeout=response_timeout)
             if stream:
-                return _process_inference_stream(response, callback)
+                return _process_inference_stream_async(response, callback)
             # ChatCompletion only
             chat_completion: Optional[ChatCompletionResponse] = None
-            for resp in response:
+            async for resp in response:
                 if callback:
                     return resp.chat_completion_response
                 else:
                     if resp.chat_completion_response:
                         chat_completion = resp.chat_completion_response
                     if resp.evaluate_response and chat_completion:
                         set_completion_evaluation_response(chat_completion, resp.evaluate_response)
                         return chat_completion
             return chat_completion
         else:
-            response = self.client.chat.completions.create(
+            response = await self.client.chat.completions.create(
                 messages=messages,
                 model=model,
                 frequency_penalty=frequency_penalty,
                 function_call=function_call,
                 functions=functions,
                 logit_bias=logit_bias,
                 logprobs=logprobs,
@@ -167,168 +170,57 @@
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
 
             )
             if stream:
-                return _process_stream(session_id, reference_id, action_type, application_ref_name, messages, response, callback)
+                return _process_async_openai_stream(session_id, reference_id, action_type, application_ref_name, messages, response, callback)
             else:
                 maitai_completion = convert_openai_chat_completion(response)
                 proto_messages = openai_messages_to_proto(messages)
                 proto_messages.append(
                     ChatMessage(role="assistant", content=maitai_completion.choices[0].message.content))
-                if callback:
-                    maitai.Evaluator.evaluate_with_callback(
-                        session_id=session_id,
-                        reference_id=reference_id,
-                        action_type=action_type,
-                        content_type=EvaluationContentType.MESSAGE,
-                        content=proto_messages,
-                        application_ref_name=application_ref_name,
-                        callback=callback
-                    )
-                    return maitai_completion
-                else:
-                    maitai_eval = maitai.Evaluator.evaluate(
-                        session_id=session_id,
-                        reference_id=reference_id,
-                        action_type=action_type,
-                        content_type=EvaluationContentType.MESSAGE,
-                        content=proto_messages,
-                        application_ref_name=application_ref_name,
-                    )
-                    set_completion_evaluation_response(maitai_completion, maitai_eval)
-                    return maitai_completion
-
-
-def _process_stream(session_id: Union[str, int],
-                    reference_id: Union[str, int, None],
-                    action_type: str,
-                    application_ref_name: str,
-                    messages: Iterable[openai_chat_types.ChatCompletionMessageParam],
-                    stream: Union[openai.Stream[openai_chat_types.ChatCompletionChunk], openai_chat_types.ChatCompletion],
-                    callback: Optional[EvaluateCallback] = None) -> Iterable[ChatCompletionChunk]:
-    full_body = ""
-    proto_messages = openai_messages_to_proto(messages)
-    for chunk in stream:
-        maitai_chunk = convert_open_ai_chat_completion_chunk(chunk)
-        content = maitai_chunk.choices[0].delta.content
-        if content is not None:
-            full_body += content
-        if maitai_chunk.choices[0].finish_reason:
-            proto_messages.append(ChatMessage(role="assistant", content=full_body))
-            if callback:
-                yield maitai_chunk
-                maitai.Evaluator.evaluate_with_callback(
+                maitai_eval = await maitai.Evaluator.evaluate_async(
                     session_id=session_id,
                     reference_id=reference_id,
                     action_type=action_type,
                     content_type=EvaluationContentType.MESSAGE,
                     content=proto_messages,
                     application_ref_name=application_ref_name,
-                    callback=callback
+                    callback=callback,
                 )
-            else:
-                maitai_eval = maitai.Evaluator.evaluate(
-                    session_id=session_id,
-                    reference_id=reference_id,
-                    action_type=action_type,
-                    content_type=EvaluationContentType.MESSAGE,
-                    content=proto_messages,
-                    application_ref_name=application_ref_name,
-                )
-                maitai_chunk.evaluate_response = maitai_eval
-                yield maitai_chunk
+                if not callback:
+                    set_completion_evaluation_response(maitai_completion, maitai_eval)
+                return maitai_completion
+
+
+async def _process_async_openai_stream(session_id: Union[str, int],
+                                       reference_id: Union[str, int, None],
+                                       action_type: str,
+                                       application_ref_name: str,
+                                       messages: Iterable[openai_chat_types.ChatCompletionMessageParam],
+                                       stream: openai.AsyncStream[openai_chat_types.ChatCompletionChunk],
+                                       callback: Optional[EvaluateCallback] = None) -> AsyncIterable[ChatCompletionChunk]:
+    full_body = ""
+    proto_messages = openai_messages_to_proto(messages)
+    async for chunk in stream:
+        maitai_chunk = convert_open_ai_chat_completion_chunk(chunk)
+        full_body, result_chunk = process_chunk(session_id, reference_id, action_type, application_ref_name, proto_messages, full_body, maitai_chunk, callback)
+        if result_chunk is not None:
+            yield result_chunk
             break
         yield maitai_chunk
 
 
-def _process_inference_stream(stream: Iterable[InferenceStreamResponse], callback: EvaluateCallback) -> Iterable[ChatCompletionChunk]:
+async def _process_inference_stream_async(stream: AsyncIterable[InferenceStreamResponse], callback: EvaluateCallback) -> AsyncIterable[ChatCompletionChunk]:
     last_chat_completion_chunk: Optional[ChatCompletionChunk] = None
-    for infer_resp in stream:
-        if infer_resp.evaluate_response:
-            if not callback:
-                maitai_chunk = last_chat_completion_chunk
-                set_chunk_evaluation_response(maitai_chunk, infer_resp.evaluate_response)
-                yield maitai_chunk
-                return
-        if infer_resp.chat_completion_chunk:
-            chunk = infer_resp.chat_completion_chunk
+    async for infer_resp in stream:
+        chunk = process_stream_response(infer_resp, callback, last_chat_completion_chunk)
+        if chunk is not None:
             if chunk.choices[0].finish_reason:
                 if callback:
                     yield chunk
                     return
                 else:
                     last_chat_completion_chunk = chunk
-            else:
-                yield chunk
-
-
-def get_chat_completion_params(*,
-                               messages: Iterable[openai_chat_types.ChatCompletionMessageParam],
-                               model: Union[str, openai_types.ChatModel],
-                               frequency_penalty: Union[Optional[float], openai.NotGiven] = openai.NOT_GIVEN,
-                               logit_bias: Union[Optional[Dict[str, int]], openai.NotGiven] = openai.NOT_GIVEN,
-                               logprobs: Union[Optional[bool], openai.NotGiven] = openai.NOT_GIVEN,
-                               max_tokens: Union[Optional[int], openai.NotGiven] = openai.NOT_GIVEN,
-                               n: Union[Optional[int], openai.NotGiven] = openai.NOT_GIVEN,
-                               presence_penalty: Union[Optional[float], openai.NotGiven] = openai.NOT_GIVEN,
-                               response_format: Union[openai_chat_types.completion_create_params.ResponseFormat, openai.NotGiven] = openai.NOT_GIVEN,
-                               seed: Union[Optional[int], openai.NotGiven] = openai.NOT_GIVEN,
-                               stop: Union[Union[Optional[str], List[str]], openai.NotGiven] = openai.NOT_GIVEN,
-                               stream: Optional[bool] = False,
-                               stream_options: Union[Optional[openai_chat_types.ChatCompletionStreamOptionsParam], openai.NotGiven] = openai.NOT_GIVEN,
-                               temperature: Union[Optional[float], openai.NotGiven] = openai.NOT_GIVEN,
-                               tool_choice: Union[openai_chat_types.ChatCompletionToolChoiceOptionParam, openai.NotGiven] = openai.NOT_GIVEN,
-                               tools: Union[Iterable[openai_chat_types.ChatCompletionToolParam], openai.NotGiven] = openai.NOT_GIVEN,
-                               top_logprobs: Union[Optional[int], openai.NotGiven] = openai.NOT_GIVEN,
-                               top_p: Union[Optional[float], openai.NotGiven] = openai.NOT_GIVEN,
-                               user: Union[str, openai.NotGiven] = openai.NOT_GIVEN,
-                               ) -> ChatCompletionParams:
-    params = ChatCompletionParams(
-        messages=openai_messages_to_proto(messages),
-        model=model,
-        stream=stream,
-    )
-    # Define all optional parameters in a dictionary
-    optional_params = {
-        'max_tokens': max_tokens,
-        'temperature': temperature,
-        'top_p': top_p,
-        'stop': stop,
-        'logprobs': logprobs,
-        'top_logprobs': top_logprobs,
-        'n': n,
-        'seed': seed,
-        'logit_bias': logit_bias,
-        'presence_penalty': presence_penalty,
-        'frequency_penalty': frequency_penalty,
-        'user': user,
-        'tool_choice': tool_choice,
-    }
-    # Set each parameter that is not marked as NOT_GIVEN
-    for param_name, value in optional_params.items():
-        if value != openai.NOT_GIVEN:
-            setattr(params, param_name, value)
-
-    if stream_options != openai.NOT_GIVEN and stream_options:
-        params.stream_options = StreamOptions(include_usage=stream_options.get("include_usage"))
-
-    if response_format != openai.NOT_GIVEN:
-        params.response_format = ResponseFormat(type=response_format["type"])
-
-    if tools != openai.NOT_GIVEN:
-        params.tools = []
-        for tool in tools:
-            function = tool.get("function")
-            params.tools.append(
-                Tool(
-                    type=tool["type"],
-                    function=Function(
-                        name=function.get("name"),
-                        description=function.get("description"),
-                        parameters=function.get("parameters")
-                    )
-                )
-            )
-    return params
+            yield chunk
```

### Comparing `maitai_python-1.0.1b1/maitai/_types.py` & `maitai_python-1.0.1b2/maitai/_types.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,28 @@
+import asyncio
 import queue
 from typing import Callable, Union
 
 import maitai_gen.chat as chat_types
-from maitai_gen.chat import EvaluateResponse
+from maitai_gen.chat import *
 
 ChunkQueue = queue.Queue[Union[chat_types.ChatCompletionChunk, "done"]]
+AsyncChunkQueue = asyncio.Queue[Union[chat_types.ChatCompletionChunk, "done"]]
 
 
 class QueueIterable:
-    def __init__(self, chunk_queue: ChunkQueue, timeout=None) -> None:
+    def __init__(self, chunk_queue: Union[ChunkQueue, AsyncChunkQueue], timeout=None) -> None:
         self.queue = chunk_queue
         self.done = False  # Indicates if "done" token has been received
         self.timeout = timeout
 
+    def __aiter__(self):
+        """Returns the asynchronous iterator object itself."""
+        return self
+
     def __iter__(self):
         """Returns the iterator object itself."""
         return self
 
     def __next__(self) -> chat_types.ChatCompletionChunk:
         """Waits for the next item from the queue or raises StopIteration if "done"."""
         while not self.done:
@@ -29,9 +35,32 @@
                 return item
             except queue.Empty:
                 print("Queue timed out")
                 self.done = True
                 raise TimeoutError
         raise StopIteration
 
+    async def __anext__(self) -> chat_types.ChatCompletionChunk:
+        """Waits for the next item from the queue or raises StopAsyncIteration if "done"."""
+        if self.done:
+            raise StopAsyncIteration
+
+        try:
+            # Wait for an item from the queue with a timeout if specified
+            if self.timeout:
+                item = await asyncio.wait_for(self.queue.get(), timeout=self.timeout)
+            else:
+                item = await self.queue.get()
+
+            if item == "done":
+                self.done = True  # Set done to True to prevent further blocking
+                raise StopAsyncIteration
+
+            return item
+
+        except asyncio.TimeoutError:
+            print("Queue timed out")
+            self.done = True
+            raise StopAsyncIteration
+
 
 EvaluateCallback = Callable[[EvaluateResponse], None]
```

### Comparing `maitai_python-1.0.1b1/maitai_common/processes/io_thread.py` & `maitai_python-1.0.1b2/maitai_common/processes/io_thread.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b1/maitai_common/processes/websocket_listener_thread.py` & `maitai_python-1.0.1b2/maitai_common/processes/websocket_listener_thread.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b1/maitai_gen/application/__init__.py` & `maitai_python-1.0.1b2/maitai_gen/application/__init__.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b1/maitai_gen/chat/__init__.py` & `maitai_python-1.0.1b2/maitai_gen/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b1/maitai_gen/company/__init__.py` & `maitai_python-1.0.1b2/maitai_gen/company/__init__.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b1/maitai_gen/inference/__init__.py` & `maitai_python-1.0.1b2/maitai_gen/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b1/maitai_gen/notification/__init__.py` & `maitai_python-1.0.1b2/maitai_gen/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b1/maitai_gen/sandbox/__init__.py` & `maitai_python-1.0.1b2/maitai_gen/sandbox/__init__.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b1/maitai_gen/sentinel/__init__.py` & `maitai_python-1.0.1b2/maitai_gen/sentinel/__init__.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b1/maitai_gen/session/__init__.py` & `maitai_python-1.0.1b2/maitai_gen/session/__init__.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b1/maitai_python.egg-info/PKG-INFO` & `maitai_python-1.0.1b2/maitai_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maitai-python
-Version: 1.0.1b1
+Version: 1.0.1b2
 Summary: MaiTai SDK for Python
 Home-page: https://docs.trymaitai.ai
 Author: Maitai
 Author-email: support@trymaitai.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `maitai_python-1.0.1b1/maitai_python.egg-info/SOURCES.txt` & `maitai_python-1.0.1b2/maitai_python.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 maitai/__init__.py
 maitai/_config.py
 maitai/_config_listener_thread.py
 maitai/_evaluator.py
 maitai/_inference.py
 maitai/_maitai_client.py
 maitai/_openai.py
+maitai/_openai_async.py
 maitai/_openai_types.py
 maitai/_types.py
 maitai/_utils.py
 maitai_common/__init__.py
 maitai_common/processes/__init__.py
 maitai_common/processes/io_thread.py
 maitai_common/processes/websocket_listener_thread.py
```

### Comparing `maitai_python-1.0.1b1/setup.py` & `maitai_python-1.0.1b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 
 from setuptools import setup, find_packages
 setup(
     name='maitai-python',
-    version='1.0.1b1',
+    version='1.0.1b2',
     packages=find_packages(exclude=("maitai_back", "maitai_back.*")),
     install_requires=[
         'requests',
         'openai',
         'betterproto',
         'httpx',
         'aiohttp',
```

