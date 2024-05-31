# Comparing `tmp/chzzkpy-0.0.4a1.tar.gz` & `tmp/chzzkpy-0.0.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chzzkpy-0.0.4a1.tar", last modified: Tue Mar  5 13:47:26 2024, max compression
+gzip compressed data, was "chzzkpy-0.0.5a1.tar", last modified: Fri May 31 11:35:42 2024, max compression
```

## Comparing `chzzkpy-0.0.4a1.tar` & `chzzkpy-0.0.5a1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 13:47:26.282506 chzzkpy-0.0.4a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-05 13:47:16.000000 chzzkpy-0.0.4a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-03-05 13:47:26.282506 chzzkpy-0.0.4a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-03-05 13:47:16.000000 chzzkpy-0.0.4a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 13:47:26.278506 chzzkpy-0.0.4a1/chzzkpy/
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-03-05 13:47:16.000000 chzzkpy-0.0.4a1/chzzkpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-03-05 13:47:16.000000 chzzkpy-0.0.4a1/chzzkpy/base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 13:47:26.278506 chzzkpy-0.0.4a1/chzzkpy/chat/
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-03-05 13:47:16.000000 chzzkpy-0.0.4a1/chzzkpy/chat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-03-05 13:47:16.000000 chzzkpy-0.0.4a1/chzzkpy/chat/access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-05 13:47:16.000000 chzzkpy-0.0.4a1/chzzkpy/chat/blind.py
--rw-r--r--   0 runner    (1001) docker     (127)     9661 2024-03-05 13:47:16.000000 chzzkpy-0.0.4a1/chzzkpy/chat/chat_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-05 13:47:16.000000 chzzkpy-0.0.4a1/chzzkpy/chat/connected.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-03-05 13:47:16.000000 chzzkpy-0.0.4a1/chzzkpy/chat/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-03-05 13:47:16.000000 chzzkpy-0.0.4a1/chzzkpy/chat/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     7448 2024-03-05 13:47:16.000000 chzzkpy-0.0.4a1/chzzkpy/chat/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-05 13:47:16.000000 chzzkpy-0.0.4a1/chzzkpy/chat/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-03-05 13:47:16.000000 chzzkpy-0.0.4a1/chzzkpy/chat/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-03-05 13:47:16.000000 chzzkpy-0.0.4a1/chzzkpy/chat/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-03-05 13:47:16.000000 chzzkpy-0.0.4a1/chzzkpy/chat/recent_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-03-05 13:47:16.000000 chzzkpy-0.0.4a1/chzzkpy/chat/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-03-05 13:47:16.000000 chzzkpy-0.0.4a1/chzzkpy/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-03-05 13:47:16.000000 chzzkpy-0.0.4a1/chzzkpy/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-03-05 13:47:16.000000 chzzkpy-0.0.4a1/chzzkpy/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-03-05 13:47:16.000000 chzzkpy-0.0.4a1/chzzkpy/live.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-03-05 13:47:16.000000 chzzkpy-0.0.4a1/chzzkpy/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 13:47:26.278506 chzzkpy-0.0.4a1/chzzkpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-03-05 13:47:26.000000 chzzkpy-0.0.4a1/chzzkpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-05 13:47:26.000000 chzzkpy-0.0.4a1/chzzkpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 13:47:26.000000 chzzkpy-0.0.4a1/chzzkpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-05 13:47:26.000000 chzzkpy-0.0.4a1/chzzkpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-05 13:47:26.000000 chzzkpy-0.0.4a1/chzzkpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 13:47:26.282506 chzzkpy-0.0.4a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-03-05 13:47:16.000000 chzzkpy-0.0.4a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:35:42.441451 chzzkpy-0.0.5a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-31 11:35:32.000000 chzzkpy-0.0.5a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-31 11:35:42.441451 chzzkpy-0.0.5a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-31 11:35:32.000000 chzzkpy-0.0.5a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:35:42.437451 chzzkpy-0.0.5a1/chzzkpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-31 11:35:32.000000 chzzkpy-0.0.5a1/chzzkpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-31 11:35:32.000000 chzzkpy-0.0.5a1/chzzkpy/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:35:42.437451 chzzkpy-0.0.5a1/chzzkpy/chat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-31 11:35:32.000000 chzzkpy-0.0.5a1/chzzkpy/chat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-31 11:35:32.000000 chzzkpy-0.0.5a1/chzzkpy/chat/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-31 11:35:32.000000 chzzkpy-0.0.5a1/chzzkpy/chat/blind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9661 2024-05-31 11:35:32.000000 chzzkpy-0.0.5a1/chzzkpy/chat/chat_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-31 11:35:32.000000 chzzkpy-0.0.5a1/chzzkpy/chat/connected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-31 11:35:32.000000 chzzkpy-0.0.5a1/chzzkpy/chat/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-31 11:35:32.000000 chzzkpy-0.0.5a1/chzzkpy/chat/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7448 2024-05-31 11:35:32.000000 chzzkpy-0.0.5a1/chzzkpy/chat/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-31 11:35:32.000000 chzzkpy-0.0.5a1/chzzkpy/chat/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-31 11:35:32.000000 chzzkpy-0.0.5a1/chzzkpy/chat/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-31 11:35:32.000000 chzzkpy-0.0.5a1/chzzkpy/chat/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-31 11:35:32.000000 chzzkpy-0.0.5a1/chzzkpy/chat/recent_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-05-31 11:35:32.000000 chzzkpy-0.0.5a1/chzzkpy/chat/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-31 11:35:32.000000 chzzkpy-0.0.5a1/chzzkpy/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-31 11:35:32.000000 chzzkpy-0.0.5a1/chzzkpy/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-31 11:35:32.000000 chzzkpy-0.0.5a1/chzzkpy/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-31 11:35:32.000000 chzzkpy-0.0.5a1/chzzkpy/live.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-31 11:35:32.000000 chzzkpy-0.0.5a1/chzzkpy/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:35:42.441451 chzzkpy-0.0.5a1/chzzkpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-31 11:35:42.000000 chzzkpy-0.0.5a1/chzzkpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-31 11:35:42.000000 chzzkpy-0.0.5a1/chzzkpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 11:35:42.000000 chzzkpy-0.0.5a1/chzzkpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-31 11:35:42.000000 chzzkpy-0.0.5a1/chzzkpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 11:35:42.000000 chzzkpy-0.0.5a1/chzzkpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 11:35:42.441451 chzzkpy-0.0.5a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-31 11:35:32.000000 chzzkpy-0.0.5a1/setup.py
```

### Comparing `chzzkpy-0.0.4a1/LICENSE` & `chzzkpy-0.0.5a1/LICENSE`

 * *Files identical despite different names*

### Comparing `chzzkpy-0.0.4a1/PKG-INFO` & `chzzkpy-0.0.5a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chzzkpy
-Version: 0.0.4a1
+Version: 0.0.5a1
 Summary: An unofficial Python library of Chzzk(Naver live-streaming service)
 Home-page: https://github.com/gunyu1019/chzzk_py
 Author: gunyu1019
 Author-email: gunyu1019@yhs.kr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chzzkpy-0.0.4a1/README.md` & `chzzkpy-0.0.5a1/README.md`

 * *Files identical despite different names*

### Comparing `chzzkpy-0.0.4a1/chzzkpy/__init__.py` & `chzzkpy-0.0.5a1/chzzkpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     pass
 
 
 __title__ = "chzzkpy"
 __author__ = "gunyu1019"
 __license__ = "MIT"
 __copyright__ = "Copyright 2024-present gunyu1019"
-__version__ = "0.0.4-alpha1"  # version_info.to_string()
+__version__ = "0.0.5-alpha1"  # version_info.to_string()
 
 
 class VersionInfo(NamedTuple):
     major: int
     minor: int
     micro: int
     release_level: Optional[Literal["alpha", "beta", "candidate", "final"]]
@@ -53,9 +53,9 @@
         _version_info = f"{self.major}.{self.minor}.{self.micro}"
         if self.release_level is not None:
             _version_info += "-{}".format(self.release_level) + str(self.serial)
         return _version_info
 
 
 version_info: VersionInfo = VersionInfo(
-    major=0, minor=0, micro=4, release_level="alpha", serial=1
+    major=0, minor=0, micro=5, release_level="alpha", serial=1
 )
```

### Comparing `chzzkpy-0.0.4a1/chzzkpy/base_model.py` & `chzzkpy-0.0.5a1/chzzkpy/base_model.py`

 * *Files identical despite different names*

### Comparing `chzzkpy-0.0.4a1/chzzkpy/chat/__init__.py` & `chzzkpy-0.0.5a1/chzzkpy/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `chzzkpy-0.0.4a1/chzzkpy/chat/access_token.py` & `chzzkpy-0.0.5a1/chzzkpy/chat/access_token.py`

 * *Files identical despite different names*

### Comparing `chzzkpy-0.0.4a1/chzzkpy/chat/blind.py` & `chzzkpy-0.0.5a1/chzzkpy/chat/blind.py`

 * *Files identical despite different names*

### Comparing `chzzkpy-0.0.4a1/chzzkpy/chat/chat_client.py` & `chzzkpy-0.0.5a1/chzzkpy/chat/chat_client.py`

 * *Files identical despite different names*

### Comparing `chzzkpy-0.0.4a1/chzzkpy/chat/connected.py` & `chzzkpy-0.0.5a1/chzzkpy/chat/connected.py`

 * *Files identical despite different names*

### Comparing `chzzkpy-0.0.4a1/chzzkpy/chat/enums.py` & `chzzkpy-0.0.5a1/chzzkpy/chat/enums.py`

 * *Files identical despite different names*

### Comparing `chzzkpy-0.0.4a1/chzzkpy/chat/error.py` & `chzzkpy-0.0.5a1/chzzkpy/chat/error.py`

 * *Files identical despite different names*

### Comparing `chzzkpy-0.0.4a1/chzzkpy/chat/gateway.py` & `chzzkpy-0.0.5a1/chzzkpy/chat/gateway.py`

 * *Files identical despite different names*

### Comparing `chzzkpy-0.0.4a1/chzzkpy/chat/http.py` & `chzzkpy-0.0.5a1/chzzkpy/chat/http.py`

 * *Files identical despite different names*

### Comparing `chzzkpy-0.0.4a1/chzzkpy/chat/message.py` & `chzzkpy-0.0.5a1/chzzkpy/chat/message.py`

 * *Files identical despite different names*

### Comparing `chzzkpy-0.0.4a1/chzzkpy/chat/profile.py` & `chzzkpy-0.0.5a1/chzzkpy/chat/profile.py`

 * *Files identical despite different names*

### Comparing `chzzkpy-0.0.4a1/chzzkpy/chat/recent_chat.py` & `chzzkpy-0.0.5a1/chzzkpy/chat/recent_chat.py`

 * *Files identical despite different names*

### Comparing `chzzkpy-0.0.4a1/chzzkpy/chat/state.py` & `chzzkpy-0.0.5a1/chzzkpy/chat/state.py`

 * *Files identical despite different names*

### Comparing `chzzkpy-0.0.4a1/chzzkpy/client.py` & `chzzkpy-0.0.5a1/chzzkpy/client.py`

 * *Files identical despite different names*

### Comparing `chzzkpy-0.0.4a1/chzzkpy/error.py` & `chzzkpy-0.0.5a1/chzzkpy/error.py`

 * *Files identical despite different names*

### Comparing `chzzkpy-0.0.4a1/chzzkpy/http.py` & `chzzkpy-0.0.5a1/chzzkpy/http.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,26 +20,32 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 import asyncio
 import functools
 import logging
-from typing import Annotated, Optional
+from typing import Annotated, Final, Optional
 
-from ahttp_client import Session, get, Path
+from ahttp_client import Session, get, Path, Query
 from ahttp_client.extension import get_pydantic_response_model
 from ahttp_client.request import RequestCore
 
 from .base_model import ChzzkModel, Content
+from .channel import Channel
 from .error import LoginRequired
 from .live import LiveStatus, LiveDetail
+from .search import TopSearchResult
 from .user import User
 
 _log = logging.getLogger(__name__)
+_user_agent: Final[str] = (
+    "Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36"
+    "(KHTML, like Gecko) Chrome/37.0.2049.0 Safari/537.36"
+)
 
 
 class ChzzkSession(Session):
     def __init__(self, base_url: str, loop: Optional[asyncio.AbstractEventLoop] = None):
         super().__init__(base_url=base_url, loop=loop)
 
         self._authorization_key = None
@@ -71,14 +77,19 @@
         if getattr(request.func, "__login_able__", False):
             if self.has_login:
                 if "Cookie" not in request.headers.keys():
                     request.headers["Cookie"] = ""
                 request.headers["Cookie"] += self._token
             elif getattr(request.func, "__login_required__", False):
                 raise LoginRequired()
+
+        # Add User-Agent to avoid blocking
+        if "User-Agent" not in request.headers:
+            request.headers["User-Agent"] = _user_agent
+
         return request, path
 
     @property
     def _token(self) -> str:
         return f"NID_SES={self._session_key}; NID_AUT={self._authorization_key}"
```

### Comparing `chzzkpy-0.0.4a1/chzzkpy/live.py` & `chzzkpy-0.0.5a1/chzzkpy/live.py`

 * *Files identical despite different names*

### Comparing `chzzkpy-0.0.4a1/chzzkpy/user.py` & `chzzkpy-0.0.5a1/chzzkpy/user.py`

 * *Files identical despite different names*

### Comparing `chzzkpy-0.0.4a1/chzzkpy.egg-info/PKG-INFO` & `chzzkpy-0.0.5a1/chzzkpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chzzkpy
-Version: 0.0.4a1
+Version: 0.0.5a1
 Summary: An unofficial Python library of Chzzk(Naver live-streaming service)
 Home-page: https://github.com/gunyu1019/chzzk_py
 Author: gunyu1019
 Author-email: gunyu1019@yhs.kr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chzzkpy-0.0.4a1/chzzkpy.egg-info/SOURCES.txt` & `chzzkpy-0.0.5a1/chzzkpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chzzkpy-0.0.4a1/setup.py` & `chzzkpy-0.0.5a1/setup.py`

 * *Files identical despite different names*

