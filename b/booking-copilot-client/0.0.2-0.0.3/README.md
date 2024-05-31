# Comparing `tmp/booking_copilot_client-0.0.2.tar.gz` & `tmp/booking_copilot_client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "booking_copilot_client-0.0.2.tar", last modified: Fri May 31 12:04:30 2024, max compression
+gzip compressed data, was "booking_copilot_client-0.0.3.tar", last modified: Fri May 31 14:44:13 2024, max compression
```

## Comparing `booking_copilot_client-0.0.2.tar` & `booking_copilot_client-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 pmengers   (502) staff       (20)        0 2024-05-31 12:04:30.177354 booking_copilot_client-0.0.2/
--rw-r--r--   0 pmengers   (502) staff       (20)      111 2024-05-31 12:04:30.176643 booking_copilot_client-0.0.2/PKG-INFO
--rw-r--r--   0 pmengers   (502) staff       (20)        0 2024-05-31 07:42:43.000000 booking_copilot_client-0.0.2/README.md
--rw-r--r--   0 pmengers   (502) staff       (20)      282 2024-05-31 12:02:54.000000 booking_copilot_client-0.0.2/pyproject.toml
--rw-r--r--   0 pmengers   (502) staff       (20)       38 2024-05-31 12:04:30.177507 booking_copilot_client-0.0.2/setup.cfg
-drwxr-xr-x   0 pmengers   (502) staff       (20)        0 2024-05-31 12:04:30.163105 booking_copilot_client-0.0.2/src/
-drwxr-xr-x   0 pmengers   (502) staff       (20)        0 2024-05-31 12:04:30.165776 booking_copilot_client-0.0.2/src/booking_copilot_client/
--rw-r--r--   0 pmengers   (502) staff       (20)       97 2024-05-31 11:56:15.000000 booking_copilot_client-0.0.2/src/booking_copilot_client/__init__.py
--rw-r--r--   0 pmengers   (502) staff       (20)     5477 2024-05-31 11:59:32.000000 booking_copilot_client-0.0.2/src/booking_copilot_client/client.py
-drwxr-xr-x   0 pmengers   (502) staff       (20)        0 2024-05-31 12:04:30.176077 booking_copilot_client-0.0.2/src/booking_copilot_client.egg-info/
--rw-r--r--   0 pmengers   (502) staff       (20)      111 2024-05-31 12:04:30.000000 booking_copilot_client-0.0.2/src/booking_copilot_client.egg-info/PKG-INFO
--rw-r--r--   0 pmengers   (502) staff       (20)      349 2024-05-31 12:04:30.000000 booking_copilot_client-0.0.2/src/booking_copilot_client.egg-info/SOURCES.txt
--rw-r--r--   0 pmengers   (502) staff       (20)        1 2024-05-31 12:04:30.000000 booking_copilot_client-0.0.2/src/booking_copilot_client.egg-info/dependency_links.txt
--rw-r--r--   0 pmengers   (502) staff       (20)       15 2024-05-31 12:04:30.000000 booking_copilot_client-0.0.2/src/booking_copilot_client.egg-info/requires.txt
--rw-r--r--   0 pmengers   (502) staff       (20)       23 2024-05-31 12:04:30.000000 booking_copilot_client-0.0.2/src/booking_copilot_client.egg-info/top_level.txt
+drwxr-xr-x   0 pmengers   (502) staff       (20)        0 2024-05-31 14:44:13.963480 booking_copilot_client-0.0.3/
+-rw-r--r--   0 pmengers   (502) staff       (20)      111 2024-05-31 14:44:13.962818 booking_copilot_client-0.0.3/PKG-INFO
+-rw-r--r--   0 pmengers   (502) staff       (20)        0 2024-05-31 07:42:43.000000 booking_copilot_client-0.0.3/README.md
+-rw-r--r--   0 pmengers   (502) staff       (20)      282 2024-05-31 14:44:10.000000 booking_copilot_client-0.0.3/pyproject.toml
+-rw-r--r--   0 pmengers   (502) staff       (20)       38 2024-05-31 14:44:13.963643 booking_copilot_client-0.0.3/setup.cfg
+drwxr-xr-x   0 pmengers   (502) staff       (20)        0 2024-05-31 14:44:13.949346 booking_copilot_client-0.0.3/src/
+drwxr-xr-x   0 pmengers   (502) staff       (20)        0 2024-05-31 14:44:13.952485 booking_copilot_client-0.0.3/src/booking_copilot_client/
+-rw-r--r--   0 pmengers   (502) staff       (20)       97 2024-05-31 11:56:15.000000 booking_copilot_client-0.0.3/src/booking_copilot_client/__init__.py
+-rw-r--r--   0 pmengers   (502) staff       (20)     6686 2024-05-31 14:39:20.000000 booking_copilot_client-0.0.3/src/booking_copilot_client/client.py
+drwxr-xr-x   0 pmengers   (502) staff       (20)        0 2024-05-31 14:44:13.962237 booking_copilot_client-0.0.3/src/booking_copilot_client.egg-info/
+-rw-r--r--   0 pmengers   (502) staff       (20)      111 2024-05-31 14:44:13.000000 booking_copilot_client-0.0.3/src/booking_copilot_client.egg-info/PKG-INFO
+-rw-r--r--   0 pmengers   (502) staff       (20)      349 2024-05-31 14:44:13.000000 booking_copilot_client-0.0.3/src/booking_copilot_client.egg-info/SOURCES.txt
+-rw-r--r--   0 pmengers   (502) staff       (20)        1 2024-05-31 14:44:13.000000 booking_copilot_client-0.0.3/src/booking_copilot_client.egg-info/dependency_links.txt
+-rw-r--r--   0 pmengers   (502) staff       (20)       15 2024-05-31 14:44:13.000000 booking_copilot_client-0.0.3/src/booking_copilot_client.egg-info/requires.txt
+-rw-r--r--   0 pmengers   (502) staff       (20)       23 2024-05-31 14:44:13.000000 booking_copilot_client-0.0.3/src/booking_copilot_client.egg-info/top_level.txt
```

### Comparing `booking_copilot_client-0.0.2/src/booking_copilot_client/client.py` & `booking_copilot_client-0.0.3/src/booking_copilot_client/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         if not path.exists():
             raise ValueError(f"File {order_path} does not exist")
         
         if not path.is_file():
             raise ValueError(f"Path {order_path} is not a file")
         
         content = path.read_bytes()
-        
+
     return content
 
 class Client():
 
     def __init__(self, bucket_name, lambda_name):
         self.bucket_name = bucket_name
         self.lambda_name = lambda_name
@@ -131,34 +131,58 @@
             if part not in ("positions", "header"):
                 raise ValueError(f"Invalid part: {part}")
             
         for format_value in formats:
             if format_value not in ("html", "json"):
                 raise ValueError(f"Invalid format: {format_value}")
         
+        ########################################
         try:
             content = _get_content(order_path)
-        except GetContentException as e:
+        except Exception as e:
+            if isinstance(e, GetContentException):
+                message = f"couldn't get the content from the provided url. The return statuscode was {e.status_code}"
+            else:
+                message = f"couldn't get the content from the provided url. The error was {e}"
             return {
-                "message": f"couldn't get the content from the provided url. The return statuscode was {e.status_code}",
+                "message": message,
                 "status_code": 401
             }
         
-        order_key = _upload_document(content, self.bucket_name)
-        result = _get_extraction_result(order_key, self.lambda_name)
-        output = _load_result_from_s3(result, self.bucket_name, parts=parts, formats=formats)
+        ########################################
+        try:
+            order_key = _upload_document(content, self.bucket_name)
+            logging.info("Document uploaded to s3. Key: %s", order_key)
+        except Exception as e:
+            return {
+                "message": f"couldn't upload the document to s3. The error was {e}",
+                "status_code": 401
+            }
 
-        object_key = "positions_html"
-        if object_key in output:
+        ########################################
+        try:
+            result = _get_extraction_result(order_key, self.lambda_name)
+            if not ('statusCode' in result and result['statusCode'] == 200):
+                raise ValueError(f"Error in lambda function: {result}")
+            logging.info("Extraction result: %s", result)
+        except  Exception as e:
+            return {
+                "message": f"couldn't get the extraction result from the lambda function. The error was {e}",
+                "status_code": 401
+            }
+        
+        ########################################
+        try:
+            output = _load_result_from_s3(result, self.bucket_name, parts=parts, formats=formats)
+            logging.info("Output: %s", output)
+            object_key = "positions_html"
+            content = output[object_key]
             return {
                 "message": "Extraction successful",
                 "status_code": 200,
-                "content": output[object_key]
+                "content": content
             }
-        else:
+        except Exception as e:
             return {
-                "message": "Extraction failed",
-                "status_code": 400
-            }
-
-
-
+                "message": f"couldn't load the result from s3. The error was {e}",
+                "status_code": 401
+            }
```

