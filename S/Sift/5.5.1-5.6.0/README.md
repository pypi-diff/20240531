# Comparing `tmp/Sift-5.5.1.tar.gz` & `tmp/Sift-5.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sift-5.5.1.tar", last modified: Fri Feb 23 12:42:53 2024, max compression
+gzip compressed data, was "Sift-5.6.0.tar", last modified: Fri May 31 13:48:33 2024, max compression
```

## Comparing `Sift-5.5.1.tar` & `Sift-5.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:42:53.257240 Sift-5.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-02-23 12:42:52.000000 Sift-5.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-23 12:42:52.000000 Sift-5.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12336 2024-02-23 12:42:53.257240 Sift-5.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-02-23 12:42:52.000000 Sift-5.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:42:53.257240 Sift-5.5.1/Sift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12336 2024-02-23 12:42:53.000000 Sift-5.5.1/Sift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-23 12:42:53.000000 Sift-5.5.1/Sift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 12:42:53.000000 Sift-5.5.1/Sift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-23 12:42:53.000000 Sift-5.5.1/Sift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-23 12:42:53.000000 Sift-5.5.1/Sift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 12:42:53.257240 Sift-5.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-02-23 12:42:52.000000 Sift-5.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:42:53.257240 Sift-5.5.1/sift/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-23 12:42:52.000000 Sift-5.5.1/sift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46525 2024-02-23 12:42:52.000000 Sift-5.5.1/sift/client.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 12:42:52.000000 Sift-5.5.1/sift/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:48:33.902280 Sift-5.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-31 13:48:33.000000 Sift-5.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 13:48:33.000000 Sift-5.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12706 2024-05-31 13:48:33.902280 Sift-5.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-05-31 13:48:33.000000 Sift-5.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:48:33.902280 Sift-5.6.0/Sift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12706 2024-05-31 13:48:33.000000 Sift-5.6.0/Sift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-31 13:48:33.000000 Sift-5.6.0/Sift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:48:33.000000 Sift-5.6.0/Sift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-31 13:48:33.000000 Sift-5.6.0/Sift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-31 13:48:33.000000 Sift-5.6.0/Sift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 13:48:33.902280 Sift-5.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-31 13:48:33.000000 Sift-5.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:48:33.902280 Sift-5.6.0/sift/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-31 13:48:33.000000 Sift-5.6.0/sift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47355 2024-05-31 13:48:33.000000 Sift-5.6.0/sift/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 13:48:33.000000 Sift-5.6.0/sift/version.py
```

### Comparing `Sift-5.5.1/LICENSE` & `Sift-5.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Sift-5.5.1/PKG-INFO` & `Sift-5.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sift
-Version: 5.5.1
+Version: 5.6.0
 Summary: Python bindings for Sift Science's API
 Home-page: https://siftscience.com
 Author: Sift Science
 Author-email: support@siftscience.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -136,14 +136,22 @@
     if response.is_ok():
         score_response = response.body["score_response"]
         print(score_response)
 except sift.client.ApiException:
     # request failed
     pass
 
+# To include `warnings` field to Events API response via calling `track()` method, set it by the `include_warnings` param:
+try:
+    response = client.track("$transaction", properties, include_warnings=True)
+    # ...
+except sift.client.ApiException:
+    # request failed
+    pass
+
 # Request a score for the user with user_id 23056
 try:
     response = client.score(user_id)
     s = json.dumps(response.body)
     print s
 
 except sift.client.ApiException:
@@ -284,14 +292,17 @@
 pip install ../sift-python
 
 # run the app
 python test_integration_app/main.py
 ```
 
 
+5.6.0 2024-05-31
+- Added support for a `warnings` value in the `fields` query parameter
+
 5.5.1 2024-02-22
 - Support for Python 3.12
 
 5.5.0 2023-10-03
 - Score percentiles for Score API
 
 5.4.0 2023-07-26
```

### Comparing `Sift-5.5.1/README.md` & `Sift-5.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -115,14 +115,22 @@
     if response.is_ok():
         score_response = response.body["score_response"]
         print(score_response)
 except sift.client.ApiException:
     # request failed
     pass
 
+# To include `warnings` field to Events API response via calling `track()` method, set it by the `include_warnings` param:
+try:
+    response = client.track("$transaction", properties, include_warnings=True)
+    # ...
+except sift.client.ApiException:
+    # request failed
+    pass
+
 # Request a score for the user with user_id 23056
 try:
     response = client.score(user_id)
     s = json.dumps(response.body)
     print s
 
 except sift.client.ApiException:
```

### Comparing `Sift-5.5.1/Sift.egg-info/PKG-INFO` & `Sift-5.6.0/Sift.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sift
-Version: 5.5.1
+Version: 5.6.0
 Summary: Python bindings for Sift Science's API
 Home-page: https://siftscience.com
 Author: Sift Science
 Author-email: support@siftscience.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -136,14 +136,22 @@
     if response.is_ok():
         score_response = response.body["score_response"]
         print(score_response)
 except sift.client.ApiException:
     # request failed
     pass
 
+# To include `warnings` field to Events API response via calling `track()` method, set it by the `include_warnings` param:
+try:
+    response = client.track("$transaction", properties, include_warnings=True)
+    # ...
+except sift.client.ApiException:
+    # request failed
+    pass
+
 # Request a score for the user with user_id 23056
 try:
     response = client.score(user_id)
     s = json.dumps(response.body)
     print s
 
 except sift.client.ApiException:
@@ -284,14 +292,17 @@
 pip install ../sift-python
 
 # run the app
 python test_integration_app/main.py
 ```
 
 
+5.6.0 2024-05-31
+- Added support for a `warnings` value in the `fields` query parameter
+
 5.5.1 2024-02-22
 - Support for Python 3.12
 
 5.5.0 2023-10-03
 - Score percentiles for Score API
 
 5.4.0 2023-07-26
```

### Comparing `Sift-5.5.1/setup.py` & `Sift-5.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `Sift-5.5.1/sift/client.py` & `Sift-5.6.0/sift/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,16 @@
             return_action=False,
             return_workflow_status=False,
             return_route_info=False,
             force_workflow_run=False,
             abuse_types=None,
             timeout=None,
             version=None,
-            include_score_percentiles=False):
+            include_score_percentiles=False,
+            include_warnings=False):
         """Track an event and associated properties to the Sift Science client.
         This call is blocking.  Check out https://siftscience.com/resources/references/events-api
         for more information on what types of events you can send and fields you can add to the
         properties parameter.
 
         Args:
             event: The name of the event to send. This can either be a reserved
@@ -133,14 +134,18 @@
             timeout(optional): Use a custom timeout (in seconds) for this call.
 
             version(optional): Use a different version of the Sift Science API for this call.
 
             include_score_percentiles(optional) : Whether to add new parameter in the query parameter.
                 if include_score_percentiles is true then add a new parameter called fields in the query parameter
 
+            include_warnings(optional) : Whether the API response should include `warnings` field.
+                if include_warnings is True `warnings` field returns the amount of validation warnings
+                along with their descriptions. They are not critical enough to reject the whole request,
+                but important enough to be fixed.
         Returns:
             A sift.client.Response object if the track call succeeded, otherwise
             raises an ApiException.
 
         """
         _assert_non_empty_unicode(event, 'event')
         _assert_non_empty_dict(properties, 'properties')
@@ -175,16 +180,20 @@
 
         if return_route_info:
             params['return_route_info'] = 'true'
 
         if force_workflow_run:
             params['force_workflow_run'] = 'true'
 
-        if include_score_percentiles:
-            params['fields'] = 'SCORE_PERCENTILES'
+        include_fields = Client._get_fields_param(include_score_percentiles,
+                                               include_warnings)
+        if include_fields:
+            params['fields'] = ",".join(include_fields)
+
+
         try:
             response = self.session.post(
                 path,
                 data=json.dumps(properties, cls=DecimalEncoder),
                 headers=headers,
                 timeout=timeout,
                 params=params)
@@ -1116,14 +1125,24 @@
     
     def _verification_resend_url(self):
         return (API_URL_VERIFICATION + 'resend')
     
     def _verification_check_url(self):
         return (API_URL_VERIFICATION + 'check')
 
+    @staticmethod
+    def _get_fields_param(include_score_percentiles, include_warnings):
+        return [
+            field for include, field in [
+                (include_score_percentiles, 'SCORE_PERCENTILES'),
+                (include_warnings, 'WARNINGS')
+            ] if include
+        ]
+
+
 class Response(object):
     HTTP_CODES_WITHOUT_BODY = [204, 304]
 
     def __init__(self, http_response):
         """
         Raises ApiException on invalid JSON in Response body or non-2XX HTTP
         status code.
```

