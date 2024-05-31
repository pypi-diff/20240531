# Comparing `tmp/satori_python_client-0.9.1.tar.gz` & `tmp/satori_python_client-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_python_client-0.9.1.tar", last modified: Wed Nov 29 15:18:03 2023, max compression
+gzip compressed data, was "satori_python_client-0.9.2.tar", last modified: Wed Dec  6 07:07:23 2023, max compression
```

## Comparing `satori_python_client-0.9.1.tar` & `satori_python_client-0.9.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      938 2023-11-29 15:17:49.932044 satori_python_client-0.9.1/.mina/client.toml
--rw-r--r--   0        0        0     1069 2023-11-29 15:17:49.932044 satori_python_client-0.9.1/LICENSE
--rw-r--r--   0        0        0     2662 2023-11-29 15:17:49.932044 satori_python_client-0.9.1/README.md
--rw-r--r--   0        0        0     1973 2023-11-29 15:18:03.567945 satori_python_client-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     3674 2023-11-29 15:17:49.932044 satori_python_client-0.9.1/src/satori/client/__init__.py
--rw-r--r--   0        0        0     1177 2023-11-29 15:17:49.932044 satori_python_client-0.9.1/src/satori/client/account.py
--rw-r--r--   0        0        0     5516 2023-11-29 15:17:49.932044 satori_python_client-0.9.1/src/satori/client/account.pyi
--rw-r--r--   0        0        0        0 2023-11-29 15:17:49.932044 satori_python_client-0.9.1/src/satori/client/network/__init__.py
--rw-r--r--   0        0        0     1248 2023-11-29 15:17:49.932044 satori_python_client-0.9.1/src/satori/client/network/base.py
--rw-r--r--   0        0        0     4292 2023-11-29 15:17:49.932044 satori_python_client-0.9.1/src/satori/client/network/webhook.py
--rw-r--r--   0        0        0     7211 2023-11-29 15:17:49.932044 satori_python_client-0.9.1/src/satori/client/network/websocket.py
--rw-r--r--   0        0        0    12785 2023-11-29 15:17:49.932044 satori_python_client-0.9.1/src/satori/client/session.py
--rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 satori_python_client-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      938 2023-12-06 07:07:08.724102 satori_python_client-0.9.2/.mina/client.toml
+-rw-r--r--   0        0        0     1069 2023-12-06 07:07:08.724102 satori_python_client-0.9.2/LICENSE
+-rw-r--r--   0        0        0     2662 2023-12-06 07:07:08.724102 satori_python_client-0.9.2/README.md
+-rw-r--r--   0        0        0     1973 2023-12-06 07:07:23.196170 satori_python_client-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     3674 2023-12-06 07:07:08.724102 satori_python_client-0.9.2/src/satori/client/__init__.py
+-rw-r--r--   0        0        0     1177 2023-12-06 07:07:08.724102 satori_python_client-0.9.2/src/satori/client/account.py
+-rw-r--r--   0        0        0     5558 2023-12-06 07:07:08.724102 satori_python_client-0.9.2/src/satori/client/account.pyi
+-rw-r--r--   0        0        0        0 2023-12-06 07:07:08.724102 satori_python_client-0.9.2/src/satori/client/network/__init__.py
+-rw-r--r--   0        0        0     1248 2023-12-06 07:07:08.728102 satori_python_client-0.9.2/src/satori/client/network/base.py
+-rw-r--r--   0        0        0     4292 2023-12-06 07:07:08.728102 satori_python_client-0.9.2/src/satori/client/network/webhook.py
+-rw-r--r--   0        0        0     7211 2023-12-06 07:07:08.728102 satori_python_client-0.9.2/src/satori/client/network/websocket.py
+-rw-r--r--   0        0        0    12845 2023-12-06 07:07:08.728102 satori_python_client-0.9.2/src/satori/client/session.py
+-rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 satori_python_client-0.9.2/PKG-INFO
```

### Comparing `satori_python_client-0.9.1/.mina/client.toml` & `satori_python_client-0.9.2/.mina/client.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 includes = ["src/satori/client"]
-raw-dependencies = ["satori-python-core >= 0.9.1"]
+raw-dependencies = ["satori-python-core >= 0.9.2"]
 
 [project]
 name = "satori-python-client"
 dynamic = ["version"]
 authors = [
   {name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com"}
 ]
```

### Comparing `satori_python_client-0.9.1/LICENSE` & `satori_python_client-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `satori_python_client-0.9.1/README.md` & `satori_python_client-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `satori_python_client-0.9.1/pyproject.toml` & `satori_python_client-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 dynamic = []
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "aiohttp>=3.8.6",
     "launart>=0.8.2",
-    "satori-python-core >= 0.9.1",
+    "satori-python-core >= 0.9.2",
 ]
 description = "Satori Protocol SDK for python, specify client part"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Typing :: Typed",
     "Development Status :: 4 - Beta",
@@ -19,15 +19,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
 ]
-version = "0.9.1"
+version = "0.9.2"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/RF-Tar-Railt/satori-python"
 repository = "https://github.com/RF-Tar-Railt/satori-python"
```

### Comparing `satori_python_client-0.9.1/src/satori/client/__init__.py` & `satori_python_client-0.9.2/src/satori/client/__init__.py`

 * *Files identical despite different names*

### Comparing `satori_python_client-0.9.1/src/satori/client/account.py` & `satori_python_client-0.9.2/src/satori/client/account.py`

 * *Files identical despite different names*

### Comparing `satori_python_client-0.9.1/src/satori/client/account.pyi` & `satori_python_client-0.9.2/src/satori/client/account.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 from typing import Any, Iterable, Protocol, overload
 
 from yarl import URL
 
 from satori.element import Element
-from satori.model import Channel, Event, Guild, Login, Member, Message, PageResult, Role, User
+from satori.model import Channel, Event, Guild, Login, Member, MessageObject, PageResult, Role, User
 
 from .session import Session
 
 class Api(Protocol):
     token: str | None = None
 
     @property
@@ -34,32 +34,32 @@
     @overload
     def custom(self, *, host: str, port: int, token: str | None = None) -> Session: ...
     async def send(
         self,
         event: Event,
         message: str | Iterable[str | Element],
         **kwargs,
-    ) -> list[Message]: ...
+    ) -> list[MessageObject]: ...
     async def send_message(
         self,
         channel_id: str,
         message: str | Iterable[str | Element],
-    ) -> list[Message]:
+    ) -> list[MessageObject]:
         """发送消息
 
         参数:
             channel_id: 要发送的频道 ID
             message: 要发送的消息
         """
         ...
     async def send_private_message(
         self,
         user_id: str,
         message: str | Iterable[str | Element],
-    ) -> list[Message]:
+    ) -> list[MessageObject]:
         """发送私聊消息
 
         参数:
             user_id: 要发送的用户 ID
             message: 要发送的消息
         """
         ...
@@ -78,27 +78,27 @@
         """
         ...
     async def message_create(
         self,
         *,
         channel_id: str,
         content: str,
-    ) -> list[Message]: ...
-    async def message_get(self, *, channel_id: str, message_id: str) -> Message: ...
+    ) -> list[MessageObject]: ...
+    async def message_get(self, *, channel_id: str, message_id: str) -> MessageObject: ...
     async def message_delete(self, *, channel_id: str, message_id: str) -> None: ...
     async def message_update(
         self,
         *,
         channel_id: str,
         message_id: str,
         content: str,
     ) -> None: ...
     async def message_list(
         self, *, channel_id: str, next_token: str | None = None
-    ) -> PageResult[Message]: ...
+    ) -> PageResult[MessageObject]: ...
     async def channel_get(self, *, channel_id: str) -> Channel: ...
     async def channel_list(self, *, guild_id: str, next_token: str | None = None) -> PageResult[Channel]: ...
     async def channel_create(self, *, guild_id: str, data: Channel) -> Channel: ...
     async def channel_update(
         self,
         *,
         channel_id: str,
```

### Comparing `satori_python_client-0.9.1/src/satori/client/network/base.py` & `satori_python_client-0.9.2/src/satori/client/network/base.py`

 * *Files identical despite different names*

### Comparing `satori_python_client-0.9.1/src/satori/client/network/webhook.py` & `satori_python_client-0.9.2/src/satori/client/network/webhook.py`

 * *Files identical despite different names*

### Comparing `satori_python_client-0.9.1/src/satori/client/network/websocket.py` & `satori_python_client-0.9.2/src/satori/client/network/websocket.py`

 * *Files identical despite different names*

### Comparing `satori_python_client-0.9.1/src/satori/client/session.py` & `satori_python_client-0.9.2/src/satori/client/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     ApiNotImplementedException,
     BadRequestException,
     ForbiddenException,
     MethodNotAllowedException,
     NotFoundException,
     UnauthorizedException,
 )
-from satori.model import Channel, Event, Guild, Login, Member, Message, PageResult, Role, User
+from satori.model import Channel, Event, Guild, Login, Member, MessageObject, PageResult, Role, User
 
 if TYPE_CHECKING:
     from .account import Account
 
 
 class Session:
     def __init__(self, account: Account):
@@ -57,39 +57,39 @@
                     resp.raise_for_status()
                     return json.loads(content) if (content := await resp.text()) else {}
 
     async def send(
         self,
         event: Event,
         message: str | Iterable[str | Element],
-    ) -> list[Message]:
+    ) -> list[MessageObject]:
         if not event.channel:
             raise RuntimeError("Event cannot be replied to!")
         return await self.send_message(event.channel.id, message)
 
     async def send_message(
         self,
         channel: str | Channel,
         message: str | Iterable[str | Element],
-    ) -> list[Message]:
+    ) -> list[MessageObject]:
         """发送消息
 
         参数:
             channel_id: 要发送的频道 ID
             message: 要发送的消息
         """
         channel_id = channel.id if isinstance(channel, Channel) else channel
         msg = message if isinstance(message, str) else "".join(str(i) for i in message)
         return await self.message_create(channel_id=channel_id, content=msg)
 
     async def send_private_message(
         self,
         user: str | User,
         message: str | Iterable[str | Element],
-    ) -> list[Message]:
+    ) -> list[MessageObject]:
         """发送私聊消息
 
         参数:
             user_id: 要发送的用户 ID
             message: 要发送的消息
         """
         user_id = user.id if isinstance(user, User) else user
@@ -117,28 +117,28 @@
             content=msg,
         )
 
     async def message_create(
         self,
         channel_id: str,
         content: str,
-    ) -> list[Message]:
+    ) -> list[MessageObject]:
         res = await self.call_api(
             Api.MESSAGE_CREATE,
             {"channel_id": channel_id, "content": content},
         )
         res = cast(List[dict], res)
-        return [Message.parse(i) for i in res]
+        return [MessageObject.parse(i) for i in res]
 
-    async def message_get(self, channel_id: str, message_id: str) -> Message:
+    async def message_get(self, channel_id: str, message_id: str) -> MessageObject:
         res = await self.call_api(
             Api.MESSAGE_GET,
             {"channel_id": channel_id, "message_id": message_id},
         )
-        return Message.parse(res)
+        return MessageObject.parse(res)
 
     async def message_delete(self, channel_id: str, message_id: str) -> None:
         await self.call_api(
             Api.MESSAGE_DELETE,
             {"channel_id": channel_id, "message_id": message_id},
         )
 
@@ -149,20 +149,20 @@
         content: str,
     ) -> None:
         await self.call_api(
             Api.MESSAGE_UPDATE,
             {"channel_id": channel_id, "message_id": message_id, "content": content},
         )
 
-    async def message_list(self, channel_id: str, next_token: str | None = None) -> PageResult[Message]:
+    async def message_list(self, channel_id: str, next_token: str | None = None) -> PageResult[MessageObject]:
         res = await self.call_api(
             Api.MESSAGE_LIST,
             {"channel_id": channel_id, "next": next_token},
         )
-        return PageResult.parse(res, Message.parse)
+        return PageResult.parse(res, MessageObject.parse)
 
     async def channel_get(self, channel_id: str) -> Channel:
         res = await self.call_api(
             Api.CHANNEL_GET,
             {"channel_id": channel_id},
         )
         return Channel.parse(res)
```

### Comparing `satori_python_client-0.9.1/PKG-INFO` & `satori_python_client-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satori-python-client
-Version: 0.9.1
+Version: 0.9.2
 Summary: Satori Protocol SDK for python, specify client part
 Home-page: https://github.com/RF-Tar-Railt/satori-python
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/RF-Tar-Railt/satori-python
 Project-URL: Repository, https://github.com/RF-Tar-Railt/satori-python
 Requires-Python: >=3.8
 Requires-Dist: aiohttp>=3.8.6
 Requires-Dist: launart>=0.8.2
-Requires-Dist: satori-python-core>=0.9.1
+Requires-Dist: satori-python-core>=0.9.2
 Description-Content-Type: text/markdown
 
 # satori-python
 
 ![latest release](https://img.shields.io/github/release/RF-Tar-Railt/satori-python)
 [![Licence](https://img.shields.io/github/license/RF-Tar-Railt/satori-python)](https://github.com/RF-Tar-Railt/satori-python/blob/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/satori-python)](https://pypi.org/project/satori-python)
```

