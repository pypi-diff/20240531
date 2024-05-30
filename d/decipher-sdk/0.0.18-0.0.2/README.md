# Comparing `tmp/decipher-sdk-0.0.18.tar.gz` & `tmp/decipher-sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decipher-sdk-0.0.18.tar", last modified: Thu May 30 23:00:10 2024, max compression
+gzip compressed data, was "decipher-sdk-0.0.2.tar", last modified: Tue Apr 30 22:15:10 2024, max compression
```

## Comparing `decipher-sdk-0.0.18.tar` & `decipher-sdk-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-05-30 23:00:10.117313 decipher-sdk-0.0.18/
--rw-r--r--   0 mrosenfield   (501) staff       (20)      323 2024-05-30 23:00:10.117132 decipher-sdk-0.0.18/PKG-INFO
--rw-r--r--   0 mrosenfield   (501) staff       (20)      126 2024-04-12 14:51:10.000000 decipher-sdk-0.0.18/README.md
--rw-r--r--   0 mrosenfield   (501) staff       (20)       38 2024-05-30 23:00:10.117470 decipher-sdk-0.0.18/setup.cfg
--rw-r--r--   0 mrosenfield   (501) staff       (20)      455 2024-05-30 22:19:20.000000 decipher-sdk-0.0.18/setup.py
-drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-05-30 23:00:10.114874 decipher-sdk-0.0.18/src/
-drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-05-30 23:00:10.115557 decipher-sdk-0.0.18/src/decipher_sdk/
--rw-r--r--   0 mrosenfield   (501) staff       (20)       55 2024-04-30 21:56:25.000000 decipher-sdk-0.0.18/src/decipher_sdk/__init__.py
--rw-r--r--   0 mrosenfield   (501) staff       (20)     9690 2024-05-30 22:31:53.000000 decipher-sdk-0.0.18/src/decipher_sdk/decipher_sdk.py
-drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-05-30 23:00:10.116854 decipher-sdk-0.0.18/src/decipher_sdk.egg-info/
--rw-r--r--   0 mrosenfield   (501) staff       (20)      323 2024-05-30 23:00:10.000000 decipher-sdk-0.0.18/src/decipher_sdk.egg-info/PKG-INFO
--rw-r--r--   0 mrosenfield   (501) staff       (20)      279 2024-05-30 23:00:10.000000 decipher-sdk-0.0.18/src/decipher_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 mrosenfield   (501) staff       (20)        1 2024-05-30 23:00:10.000000 decipher-sdk-0.0.18/src/decipher_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 mrosenfield   (501) staff       (20)       15 2024-05-30 23:00:10.000000 decipher-sdk-0.0.18/src/decipher_sdk.egg-info/requires.txt
--rw-r--r--   0 mrosenfield   (501) staff       (20)       13 2024-05-30 23:00:10.000000 decipher-sdk-0.0.18/src/decipher_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-04-30 22:15:10.675422 decipher-sdk-0.0.2/
+-rw-r--r--   0 mrosenfield   (501) staff       (20)      322 2024-04-30 22:15:10.675294 decipher-sdk-0.0.2/PKG-INFO
+-rw-r--r--   0 mrosenfield   (501) staff       (20)      126 2024-04-12 14:51:10.000000 decipher-sdk-0.0.2/README.md
+-rw-r--r--   0 mrosenfield   (501) staff       (20)       38 2024-04-30 22:15:10.675508 decipher-sdk-0.0.2/setup.cfg
+-rw-r--r--   0 mrosenfield   (501) staff       (20)      454 2024-04-30 22:15:06.000000 decipher-sdk-0.0.2/setup.py
+drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-04-30 22:15:10.672561 decipher-sdk-0.0.2/src/
+drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-04-30 22:15:10.673637 decipher-sdk-0.0.2/src/decipher_sdk/
+-rw-r--r--   0 mrosenfield   (501) staff       (20)       55 2024-04-30 21:56:25.000000 decipher-sdk-0.0.2/src/decipher_sdk/__init__.py
+-rw-r--r--   0 mrosenfield   (501) staff       (20)     9020 2024-04-30 22:13:01.000000 decipher-sdk-0.0.2/src/decipher_sdk/decipher_sdk.py
+drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-04-30 22:15:10.675046 decipher-sdk-0.0.2/src/decipher_sdk.egg-info/
+-rw-r--r--   0 mrosenfield   (501) staff       (20)      322 2024-04-30 22:15:10.000000 decipher-sdk-0.0.2/src/decipher_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 mrosenfield   (501) staff       (20)      279 2024-04-30 22:15:10.000000 decipher-sdk-0.0.2/src/decipher_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 mrosenfield   (501) staff       (20)        1 2024-04-30 22:15:10.000000 decipher-sdk-0.0.2/src/decipher_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 mrosenfield   (501) staff       (20)       15 2024-04-30 22:15:10.000000 decipher-sdk-0.0.2/src/decipher_sdk.egg-info/requires.txt
+-rw-r--r--   0 mrosenfield   (501) staff       (20)       13 2024-04-30 22:15:10.000000 decipher-sdk-0.0.2/src/decipher_sdk.egg-info/top_level.txt
```

### Comparing `decipher-sdk-0.0.18/src/decipher_sdk/decipher_sdk.py` & `decipher-sdk-0.0.2/src/decipher_sdk/decipher_sdk.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,17 +23,15 @@
     def __init__(self, codebase_id, customer_id):
         self.codebase_id = codebase_id
         self.customer_id = customer_id
         self.endpoint = "https://prod.getdecipher.com/api/exception_upload"
         #self.endpoint = "http://localhost:3000/api/exception_upload"
         self.messages = []  # Initialize the messages list
         self.user = None
-        self.response = None
-        self.captured_exceptions = []
-        self.uncaught_exception = None
+        self.exception_occurred = False  # Flag to indicate an exception has occurred
         self.connect_to_signals()
 
     @safe_method
     def connect_to_signals(self):
         # Connect to Flask signals
         request_started.connect(self.before_request_handler)
         request_finished.connect(self.teardown_request_handler)
@@ -45,42 +43,29 @@
         if has_request_context():
             self.override_print()
 
     @safe_method
     def teardown_request_handler(self, sender, response, **extra):
         if has_request_context():
             self.restore_print()
-            self.response = response;
-            self.handleExceptions();
-
-            #Reset state
+            if not self.exception_occurred and response.status_code != 200:
+                self.capture_error_with_response(response)
+            self.user = None
             self.clear_messages()
 
     @safe_method
-    def handleExceptions(self):
-        if self.uncaught_exception:
-            self.capture_error_with_response(self.response, self.uncaught_exception, True)
-        if self.captured_exceptions:
-            for exception in self.captured_exceptions:
-                self.capture_error_with_response(self.response, exception)
-        self.response = None
-        self.user = None
-        self.uncaught_exception = None
-        self.captured_exceptions = []
-
-    @safe_method
-    def capture_error_with_response(self, response, exception, is_uncaught_exception=False):
-        data = self.prepare_data(response, exception, is_uncaught_exception)
+    def capture_error_with_response(self, response):
+        data = self.prepare_data(response)
         self.send_to_decipher(data)
 
     @safe_method
     def capture_error_handler(self, sender, exception, **extra):
-        self.uncaught_exception = exception
+        self.exception_occurred = True  # Set the flag when an exception is caught
         if has_request_context():
-            self.handleExceptions()
+            self.capture_error_with_exception(sender, exception, **extra)
 
     @safe_method
     def get_request_body(self):
         request_body = None
         max_content_length = 10 * 1024 * 1024  # 10 MB
         if request.content_length and request.content_length < max_content_length:
             request_body = request.get_data(as_text=True)
@@ -120,17 +105,17 @@
             "level": "log",
             "timestamp": self.get_timestamp()
         })
         # Call the original print function
         self.original_print(*args, **kwargs)
 
     @safe_method
-    def capture_error_with_exception(self, sender, **extra):
+    def capture_error_with_exception(self, sender, exception, **extra):
         if has_request_context():
-            data = self.prepare_data()
+            data = self.prepare_data(exception=exception)
             self.send_to_decipher(data)
         #stack_trace = "\n".join(traceback.format_stack()) if response else traceback.format_exc()
 
     @safe_method
     def get_code_context(self, filename, line_number, context=5):
         start_line = max(1, line_number - context)
         end_line = line_number + context
@@ -149,30 +134,27 @@
     @safe_method
     def get_stack_trace_with_code(self, exception):
         if exception is None:
             return []
         
         tb = traceback.extract_tb(exception.__traceback__)
         formatted_trace = []
-        context = 40
+        context = 5 
         for frame, line_number in [(tb_frame, tb_lineno) for tb_frame, tb_lineno in traceback.walk_tb(exception.__traceback__)]:
             filename = frame.f_code.co_filename
             function_name = frame.f_code.co_name
             start_line = max(1, line_number - context)
             code_context = self.get_code_context(filename, line_number, context)
             locals = self.get_local_variables(frame)
-            highlight_index = line_number - start_line
-            if highlight_index >= len(code_context):
-                highlight_index = len(code_context) - 1 
             formatted_trace.append({
                 "file": filename,
                 "line": line_number,
                 "function": function_name,
                 "code": code_context,
-                "highlight_index": highlight_index,
+                "highlight_index": context,
                 "start_line": start_line,
                 "locals": locals,  # Add local variables to the trace
             })
         
         # Add the exception type and message to the last trace
         exception_type = type(exception).__name__
         exception_message = str(exception)
@@ -181,23 +163,18 @@
             last_trace.update({
                 "exception_type": exception_type,
                 "exception_message": exception_message
             })
 
         return formatted_trace
 
-
-    @safe_method
-    def append_error(self, error):
-        self.captured_exceptions.append(error)
-
     @safe_method
-    def prepare_data(self, response, exception, is_uncaught_exception=False):
+    def prepare_data(self, response=None, exception=None):
         request_body = self.get_request_body()
-        stack_trace = self.get_stack_trace_with_code(exception)
+        stack_trace = self.get_stack_trace_with_code(exception) if exception else ""
         #stack_trace = "\n".join(traceback.format_stack()) if response else traceback.format_exc()
 
         response_body = {}
         status_code = 500
         if response:
             status_code = response.status_code
             try:
@@ -212,15 +189,15 @@
             "error_stack": stack_trace,
             "request_url": request.url,
             "request_endpoint": request.endpoint,
             "request_headers": self.get_headers(request.headers),
             "request_body": request_body,
             "response_body": response_body,
             "status_code": status_code,
-            "is_uncaught_exception": is_uncaught_exception,
+            "is_uncaught_exception": exception is not None,
             'messages': self.messages,
             'affected_user': self.user
         }
         return data
 
     @safe_method
     def get_timestamp(self):
@@ -265,15 +242,15 @@
 
 def init(codebase_id, customer_id):
     global _decipher_monitor_instance
     _decipher_monitor_instance = DecipherMonitor(codebase_id, customer_id)
 
 def capture_error(error):
     if _decipher_monitor_instance:
-        _decipher_monitor_instance.append_error(error)
+        _decipher_monitor_instance.capture_error(error)
     else:
         # Handle the case where DecipherMonitor is not initialized
         pass
 
 def set_user(user):
     if _decipher_monitor_instance:
         _decipher_monitor_instance.set_user(user)
```

