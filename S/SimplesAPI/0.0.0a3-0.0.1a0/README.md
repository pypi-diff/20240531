# Comparing `tmp/simplesapi-0.0.0a3.tar.gz` & `tmp/simplesapi-0.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplesapi-0.0.0a3.tar", max compression
+gzip compressed data, was "simplesapi-0.0.1a0.tar", max compression
```

## Comparing `simplesapi-0.0.0a3.tar` & `simplesapi-0.0.1a0.tar`

### file list

```diff
@@ -1,8 +1,6 @@
--rw-r--r--   0        0        0      471 2024-05-31 00:51:43.140035 simplesapi-0.0.0a3/pyproject.toml
--rw-r--r--   0        0        0       12 2024-05-30 15:30:50.326578 simplesapi-0.0.0a3/README.md
--rw-r--r--   0        0        0      173 2024-05-31 00:45:34.171209 simplesapi-0.0.0a3/simplesapi/__init__.py
--rw-r--r--   0        0        0      918 2024-05-31 00:43:10.780386 simplesapi-0.0.0a3/simplesapi/app.py
--rw-r--r--   0        0        0     1340 2024-05-30 15:29:16.921041 simplesapi-0.0.0a3/simplesapi/auto_routing.py
--rw-r--r--   0        0        0      194 2024-05-31 00:46:06.435574 simplesapi-0.0.0a3/simplesapi/lifespan.py
--rw-r--r--   0        0        0     1091 2024-05-31 00:46:33.986007 simplesapi-0.0.0a3/simplesapi/settings.py
--rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 simplesapi-0.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0        9 2024-05-30 15:17:38.677459 simplesapi-0.0.1a0/README.md
+-rw-r--r--   0        0        0      382 2024-05-30 15:17:50.665460 simplesapi-0.0.1a0/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-05-30 15:17:38.677459 simplesapi-0.0.1a0/simplesapi/__init__.py
+-rw-r--r--   0        0        0      813 2024-05-30 15:17:38.677459 simplesapi-0.0.1a0/simplesapi/app.py
+-rw-r--r--   0        0        0     1300 2024-05-30 15:17:38.677459 simplesapi-0.0.1a0/simplesapi/auto_routing.py
+-rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 simplesapi-0.0.1a0/PKG-INFO
```

### Comparing `simplesapi-0.0.0a3/simplesapi/auto_routing.py` & `simplesapi-0.0.1a0/simplesapi/auto_routing.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-
-import importlib
-import os
-
-
-def _import_handler(module_path, handler_name="handler"):
-    spec = importlib.util.spec_from_file_location("routes", module_path)
-    module = importlib.util.module_from_spec(spec)
-    spec.loader.exec_module(module)
-    return getattr(module, handler_name)
-
-def _create_route_from_file(app, file_path):
-    parts = file_path.split(os.sep)
-    method_file = parts[-1]
-    method = method_file.split('.')[0].split('__')[1].lower() if '__' in method_file else method_file.split('.')[0].lower()
-    
-    route = os.sep.join(parts[:-1])
-    route = route.replace('routes', '')
-    route = route.replace('[', '{').replace(']', '}')
-    route = '/' + route.strip(os.sep)
-
-    handler = _import_handler(file_path)
-    
-    if method == "get":
-        app.get(route)(handler)
-    elif method == "post":
-        app.post(route)(handler)
-    elif method == "put":
-        app.put(route)(handler)
-    elif method == "delete":
-        app.delete(route)(handler)
-    elif method == "patch":
-        app.patch(route)(handler)
-
-def register_routes(app, base_path):
-    for root, _, files in os.walk(base_path):
-        for file in files:
-            if file.endswith('.py'):
-                file_path = os.path.join(root, file)
-                _create_route_from_file(app, file_path)
+
+import importlib
+import os
+
+
+def _import_handler(module_path, handler_name="handler"):
+    spec = importlib.util.spec_from_file_location("routes", module_path)
+    module = importlib.util.module_from_spec(spec)
+    spec.loader.exec_module(module)
+    return getattr(module, handler_name)
+
+def _create_route_from_file(app, file_path):
+    parts = file_path.split(os.sep)
+    method_file = parts[-1]
+    method = method_file.split('.')[0].split('__')[1].lower() if '__' in method_file else method_file.split('.')[0].lower()
+    
+    route = os.sep.join(parts[:-1])
+    route = route.replace('routes', '')
+    route = route.replace('[', '{').replace(']', '}')
+    route = '/' + route.strip(os.sep)
+
+    handler = _import_handler(file_path)
+    
+    if method == "get":
+        app.get(route)(handler)
+    elif method == "post":
+        app.post(route)(handler)
+    elif method == "put":
+        app.put(route)(handler)
+    elif method == "delete":
+        app.delete(route)(handler)
+    elif method == "patch":
+        app.patch(route)(handler)
+
+def register_routes(app, base_path):
+    for root, _, files in os.walk(base_path):
+        for file in files:
+            if file.endswith('.py'):
+                file_path = os.path.join(root, file)
+                _create_route_from_file(app, file_path)
```

