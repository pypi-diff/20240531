# Comparing `tmp/python_sdk_rafay_workflow-0.0.8.tar.gz` & `tmp/python_sdk_rafay_workflow-0.0.9.tar.gz`

## Comparing `python_sdk_rafay_workflow-0.0.8.tar` & `python_sdk_rafay_workflow-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       60 1980-01-01 00:00:00.000000 python_sdk_rafay_workflow-0.0.8/src/python_sdk_rafay_workflow/__init__.py
--rw-r--r--   0        0        0      823 1980-01-01 00:00:00.000000 python_sdk_rafay_workflow-0.0.8/src/python_sdk_rafay_workflow/activity_logger.py
--rw-r--r--   0        0        0      283 1980-01-01 00:00:00.000000 python_sdk_rafay_workflow-0.0.8/src/python_sdk_rafay_workflow/const.py
--rw-r--r--   0        0        0     2581 1980-01-01 00:00:00.000000 python_sdk_rafay_workflow-0.0.8/src/python_sdk_rafay_workflow/sdk.py
--rw-r--r--   0        0        0      505 1980-01-01 00:00:00.000000 python_sdk_rafay_workflow-0.0.8/.gitignore
--rw-r--r--   0        0        0     1080 1980-01-01 00:00:00.000000 python_sdk_rafay_workflow-0.0.8/LICENSE
--rw-r--r--   0        0        0      192 1980-01-01 00:00:00.000000 python_sdk_rafay_workflow-0.0.8/README.md
--rw-r--r--   0        0        0      781 1980-01-01 00:00:00.000000 python_sdk_rafay_workflow-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      847 1980-01-01 00:00:00.000000 python_sdk_rafay_workflow-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       60 1980-01-01 00:00:00.000000 python_sdk_rafay_workflow-0.0.9/src/python_sdk_rafay_workflow/__init__.py
+-rw-r--r--   0        0        0      987 1980-01-01 00:00:00.000000 python_sdk_rafay_workflow-0.0.9/src/python_sdk_rafay_workflow/activity_logger.py
+-rw-r--r--   0        0        0      283 1980-01-01 00:00:00.000000 python_sdk_rafay_workflow-0.0.9/src/python_sdk_rafay_workflow/const.py
+-rw-r--r--   0        0        0     2540 1980-01-01 00:00:00.000000 python_sdk_rafay_workflow-0.0.9/src/python_sdk_rafay_workflow/sdk.py
+-rw-r--r--   0        0        0      505 1980-01-01 00:00:00.000000 python_sdk_rafay_workflow-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1080 1980-01-01 00:00:00.000000 python_sdk_rafay_workflow-0.0.9/LICENSE
+-rw-r--r--   0        0        0      192 1980-01-01 00:00:00.000000 python_sdk_rafay_workflow-0.0.9/README.md
+-rw-r--r--   0        0        0      781 1980-01-01 00:00:00.000000 python_sdk_rafay_workflow-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      847 1980-01-01 00:00:00.000000 python_sdk_rafay_workflow-0.0.9/PKG-INFO
```

### Comparing `python_sdk_rafay_workflow-0.0.8/src/python_sdk_rafay_workflow/activity_logger.py` & `python_sdk_rafay_workflow-0.0.9/src/python_sdk_rafay_workflow/activity_logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,16 @@
             resp = requests.post(self.endpoint, headers={
                 WorkflowTokenHeader: self.token,
             }, data='\n'.join(buf))
 
             if resp.status_code != 200:
                 print(f"Failed to send logs to {self.endpoint}, status code: {resp.status_code}, response: {resp.text}")
             self.buffer.clear()
+        except Exception as e:
+            print(f"Failed to send logs to {self.endpoint}, status code: {resp.status_code}, response: {resp.text}, exception: {e}")
         finally:
             self.release()
```

### Comparing `python_sdk_rafay_workflow-0.0.8/src/python_sdk_rafay_workflow/sdk.py` & `python_sdk_rafay_workflow-0.0.9/src/python_sdk_rafay_workflow/sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 def _log(f):
     def wrap(*args, **kwargs):
         logger = logging.Logger(__name__)
 
         engineEndpoint= request.headers.get(EngineAPIEndpointHeader),
         fileUploadPath= request.headers.get(ActivityFileUploadHeader),
+
         token = request.headers.get(WorkflowTokenHeader)
 
         endpoint = engineEndpoint + fileUploadPath
         handler = ActivityLogHandler(endpoint=endpoint, token=token, capacity=LOG_BUFFER_CAPACITY, flushLevel=LOG_BUFFER_FLUSH_LEVEL)
         logger.setLevel(LOG_LEVEL)
         logger.info(f"calling function: {FUNCTION_NAME}")
         logger.addHandler(handler)
@@ -43,15 +44,14 @@
     return jsonify({ "status": "ready" }), 200
 
 def call(handler):
     return lambda: handle(handler)
 
 @_log
 def handle(handler, logger=None) -> Tuple[Dict[str, Any], int]:
-    print(f"calling function handle: {handler.__name__}")
     resp, status_code = None, 0
     try:
         req = json.loads(request.data)
         if req is None:
             req = {}
         req["metadata"] = {
             "activityID": request.headers.get(ActivityIDHeader),
@@ -62,15 +62,15 @@
         resp, status_code = jsonify(resp), 200        
     except Exception as e:
         resp, status_code = jsonify({ "error": str(e) }), 500
     return resp, status_code
 
 
 def serve_function(handler, host='0.0.0.0', port=5000):
-    _logger.info(f'Starting Python Function ...')
+    _logger.info(f'Starting Python Function {FUNCTION_NAME} ...')
 
     app = Flask(FUNCTION_NAME)
 
     app.add_url_rule('/_/ready', methods=['GET'], view_func=call_ready)
     app.add_url_rule('/', methods=['POST'], view_func=call(handler))
 
     serve(app, host=host, port=port)
```

### Comparing `python_sdk_rafay_workflow-0.0.8/LICENSE` & `python_sdk_rafay_workflow-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python_sdk_rafay_workflow-0.0.8/pyproject.toml` & `python_sdk_rafay_workflow-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/python_sdk_rafay_workflow"]
 
 [project]
 name = "python_sdk_rafay_workflow"
-version = "0.0.8"
+version = "0.0.9"
 authors = [{ name = "Bheema Sarat Chandra Kaki", email = "sarat@rafay.co" }]
 
 description = "Rafay workflow handler Python function SDK"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `python_sdk_rafay_workflow-0.0.8/PKG-INFO` & `python_sdk_rafay_workflow-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_sdk_rafay_workflow
-Version: 0.0.8
+Version: 0.0.9
 Summary: Rafay workflow handler Python function SDK
 Project-URL: Homepage, https://github.com/RafaySystems/function-templates
 Project-URL: Issues, https://github.com/RafaySystems/function-templates/issues
 Author-email: Bheema Sarat Chandra Kaki <sarat@rafay.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

