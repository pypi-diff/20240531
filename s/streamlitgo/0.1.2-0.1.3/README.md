# Comparing `tmp/streamlitgo-0.1.2.tar.gz` & `tmp/streamlitgo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitgo-0.1.2.tar", max compression
+gzip compressed data, was "streamlitgo-0.1.3.tar", max compression
```

## Comparing `streamlitgo-0.1.2.tar` & `streamlitgo-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2597 2024-05-15 10:15:22.290746 streamlitgo-0.1.2/README.md
--rw-r--r--   0        0        0      733 2024-05-15 10:15:26.590699 streamlitgo-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-15 10:15:22.290746 streamlitgo-0.1.2/streamlitgo/__init__.py
--rw-r--r--   0        0        0       61 2024-05-15 10:15:22.290746 streamlitgo-0.1.2/streamlitgo/__main__.py
--rw-r--r--   0        0        0      930 2024-05-15 10:15:22.290746 streamlitgo-0.1.2/streamlitgo/cli.py
--rw-r--r--   0        0        0     1835 2024-05-15 10:15:22.290746 streamlitgo-0.1.2/streamlitgo/config/stgo.py
--rw-r--r--   0        0        0     3035 1970-01-01 00:00:00.000000 streamlitgo-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2597 2024-05-31 02:03:22.446894 streamlitgo-0.1.3/README.md
+-rw-r--r--   0        0        0      741 2024-05-31 02:03:30.702896 streamlitgo-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-31 02:03:22.446894 streamlitgo-0.1.3/streamlitgo/__init__.py
+-rw-r--r--   0        0        0       61 2024-05-31 02:03:22.446894 streamlitgo-0.1.3/streamlitgo/__main__.py
+-rw-r--r--   0        0        0      930 2024-05-31 02:03:22.446894 streamlitgo-0.1.3/streamlitgo/cli.py
+-rw-r--r--   0        0        0     2417 2024-05-31 02:03:22.446894 streamlitgo-0.1.3/streamlitgo/config/stgo.py
+-rw-r--r--   0        0        0     3156 1970-01-01 00:00:00.000000 streamlitgo-0.1.3/PKG-INFO
```

### Comparing `streamlitgo-0.1.2/README.md` & `streamlitgo-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `streamlitgo-0.1.2/streamlitgo/cli.py` & `streamlitgo-0.1.3/streamlitgo/cli.py`

 * *Files identical despite different names*

### Comparing `streamlitgo-0.1.2/streamlitgo/config/stgo.py` & `streamlitgo-0.1.3/streamlitgo/config/stgo.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,38 +12,52 @@
 logger = get_logger(__name__)
 
 
 class MyScriptCache(ScriptCache):
     def get_bytecode(self, script_path: str) -> T.Any:
         user = _get_user_info()
         email = user.get("email", "")
-        remote_ip = user.get("remote_ip", "")
+        remote_ip = user.get("ip", "")
         logger.info(f"{email} [{remote_ip}] access script {script_path}")
         return super().get_bytecode(script_path)
 
 
 streamlit.runtime.runtime.ScriptCache = MyScriptCache
 
 
 class MyBrowserWebSocketHandler(BrowserWebSocketHandler):
     def open(self, *args, **kwargs) -> T.Awaitable[None] | None:
         ret = super().open(*args, **kwargs)
         session = self._runtime._session_mgr.get_session_info(self._session_id).session
-        email = self.request.headers.get("x-auth-request-user", "bob@Alice.com")
-        remote_ip = self.request.headers.get("X-Real-IP", "192.168.1.1")
+        email = self.request.headers.get("x-auth-request-email", "bob@Alice.com")
+        remote_ip = self.request.headers.get("X-Forwarded-For", "192.168.1.1")
+        # X-Auth-Request-Preferred-Username
+        preferred_username = (
+            self.request.headers.get("x-auth-request-preferred-username", "Bob")
+            .encode("ISO-8859-1")
+            .decode()
+        )
+        name = (
+            self.request.headers.get("x-auth-request-user", "Bob")
+            .encode("ISO-8859-1")
+            .decode()
+        )
         # script_path = "streamlitgo/__main__.py"
         # logger.error(f"{email} [{ip}] access script {script_path}")
         user = session._user_info
+        user["name"] = name
+        user["preferred_username"] = preferred_username
         user["email"] = email
-        user["ip"] = remote_ip
+        user["ip"] = remote_ip.split(",")[0].strip()
+        # all_headers = list(self.request.headers.get_all())
+        # user["all_headers"] = all_headers
         return ret
 
 
 class StreamlitServer(Server):
-
     def _create_app(self):
         app = super()._create_app()
         rules = app.wildcard_router.rules
         for rule in rules:
             if issubclass(rule.target, BrowserWebSocketHandler):
                 rule.target = MyBrowserWebSocketHandler
                 break
```

### Comparing `streamlitgo-0.1.2/PKG-INFO` & `streamlitgo-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: streamlitgo
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: paleneutron
 Author-email: paleneutron@outlook.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: streamlit (>=1.32.2,<2.0.0)
+Requires-Dist: streamlit (>=1.23,<2.0)
 Description-Content-Type: text/markdown
 
 # Streamlit GO
 
 Package for loading a script before streamlit server start
 
 This package will load `stgo.py` in current working directory before the streamlit server starts. You can use this to patch the streamlit server or to load some data before the server starts!
```

