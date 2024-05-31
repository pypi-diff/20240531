# Comparing `tmp/aioselectel_api-0.1.2.tar.gz` & `tmp/aioselectel_api-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioselectel_api-0.1.2.tar", max compression
+gzip compressed data, was "aioselectel_api-0.1.4.tar", max compression
```

## Comparing `aioselectel_api-0.1.2.tar` & `aioselectel_api-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1066 2024-05-29 17:12:48.985417 aioselectel_api-0.1.2/LICENSE
--rw-r--r--   0        0        0      394 2024-05-29 17:12:48.985417 aioselectel_api-0.1.2/README.md
--rw-r--r--   0        0        0      105 2024-05-29 17:12:48.985417 aioselectel_api-0.1.2/aioselectel_api/__init__.py
--rw-r--r--   0        0        0      246 2024-05-29 17:12:48.985417 aioselectel_api-0.1.2/aioselectel_api/base_client.py
--rw-r--r--   0        0        0     5221 2024-05-29 17:12:48.985417 aioselectel_api-0.1.2/aioselectel_api/client.py
--rw-r--r--   0        0        0       67 2024-05-29 17:12:48.985417 aioselectel_api-0.1.2/aioselectel_api/config.py
--rw-r--r--   0        0        0      365 2024-05-29 17:12:48.985417 aioselectel_api-0.1.2/aioselectel_api/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-29 17:12:48.985417 aioselectel_api-0.1.2/aioselectel_api/services/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 17:12:48.985417 aioselectel_api-0.1.2/aioselectel_api/services/object_storage.py
--rw-r--r--   0        0        0     1251 2024-05-29 17:12:48.985417 aioselectel_api-0.1.2/aioselectel_api/session.py
--rw-r--r--   0        0        0      417 2024-05-29 17:12:48.985417 aioselectel_api-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1027 1970-01-01 00:00:00.000000 aioselectel_api-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      108 2024-05-29 13:38:37.189072 aioselectel_api-0.1.4/aioselectel_api/__init__.py
+-rw-r--r--   0        0        0     1522 2024-05-31 08:05:35.819344 aioselectel_api-0.1.4/aioselectel_api/base_client.py
+-rw-r--r--   0        0        0     7915 2024-05-31 08:05:35.819344 aioselectel_api-0.1.4/aioselectel_api/client.py
+-rw-r--r--   0        0        0       68 2024-05-29 12:17:08.937064 aioselectel_api-0.1.4/aioselectel_api/config.py
+-rw-r--r--   0        0        0      385 2024-05-29 16:52:23.996144 aioselectel_api-0.1.4/aioselectel_api/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:00:51.477077 aioselectel_api-0.1.4/aioselectel_api/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 12:23:31.469560 aioselectel_api-0.1.4/aioselectel_api/services/object_storage.py
+-rw-r--r--   0        0        0     1294 2024-05-29 12:12:59.656500 aioselectel_api-0.1.4/aioselectel_api/session.py
+-rw-r--r--   0        0        0     1087 2024-05-29 13:39:24.195503 aioselectel_api-0.1.4/LICENSE
+-rw-r--r--   0        0        0      438 2024-05-31 08:05:35.819344 aioselectel_api-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2298 2024-05-31 08:05:35.819344 aioselectel_api-0.1.4/README.md
+-rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 aioselectel_api-0.1.4/PKG-INFO
```

### Comparing `aioselectel_api-0.1.2/aioselectel_api/session.py` & `aioselectel_api-0.1.4/aioselectel_api/session.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-import aiohttp
-
-
-class ClientCreatorContext:
-    def __init__(self, coro):
-        self._coro = coro
-        self._client = None
-
-    async def __aenter__(self):
-        self._client = await self._coro
-        return await self._client.__aenter__()
-
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
-        await self._client.__aexit__(exc_type, exc_val, exc_tb)
-
-
-class SelectelSession:
-    def __init__(self, base_url):
-        self.base_url = base_url
-        self.session = aiohttp.ClientSession()
-
-    async def __aenter__(self):
-        return self
-
-    async def __aexit__(self, exc_type, exc, tb):
-        await self.session.close()
-
-    async def request(self, method, path, **kwargs):
-        url = f"{self.base_url}{path}"
-        async with self.session.request(method, url, **kwargs) as response:
-            return response
-
-    async def get(self, path, **kwargs):
-        return await self.request("GET", path, **kwargs)
-
-    async def post(self, path, **kwargs):
-        return await self.request("POST", path, **kwargs)
-
-    async def put(self, path, **kwargs):
-        return await self.request("PUT", path, **kwargs)
-
-    async def delete(self, path, **kwargs):
-        return await self.request("DELETE", path, **kwargs)
+import aiohttp
+
+
+class ClientCreatorContext:
+    def __init__(self, coro):
+        self._coro = coro
+        self._client = None
+
+    async def __aenter__(self):
+        self._client = await self._coro
+        return await self._client.__aenter__()
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        await self._client.__aexit__(exc_type, exc_val, exc_tb)
+
+
+class SelectelSession:
+    def __init__(self, base_url):
+        self.base_url = base_url
+        self.session = aiohttp.ClientSession()
+
+    async def __aenter__(self):
+        return self
+
+    async def __aexit__(self, exc_type, exc, tb):
+        await self.session.close()
+
+    async def request(self, method, path, **kwargs):
+        url = f"{self.base_url}{path}"
+        async with self.session.request(method, url, **kwargs) as response:
+            return response
+
+    async def get(self, path, **kwargs):
+        return await self.request("GET", path, **kwargs)
+
+    async def post(self, path, **kwargs):
+        return await self.request("POST", path, **kwargs)
+
+    async def put(self, path, **kwargs):
+        return await self.request("PUT", path, **kwargs)
+
+    async def delete(self, path, **kwargs):
+        return await self.request("DELETE", path, **kwargs)
```

