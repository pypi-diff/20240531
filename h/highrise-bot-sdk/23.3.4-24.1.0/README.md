# Comparing `tmp/highrise_bot_sdk-23.3.4.tar.gz` & `tmp/highrise_bot_sdk-24.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highrise_bot_sdk-23.3.4.tar", max compression
+gzip compressed data, was "highrise_bot_sdk-24.1.0.tar", max compression
```

## Comparing `highrise_bot_sdk-23.3.4.tar` & `highrise_bot_sdk-24.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     9818 2023-09-01 10:43:23.445202 highrise_bot_sdk-23.3.4/README.md
--rw-r--r--   0        0        0     1037 2023-09-01 10:42:25.949366 highrise_bot_sdk-23.3.4/pyproject.toml
--rw-r--r--   0        0        0    15519 2023-09-01 10:44:03.306208 highrise_bot_sdk-23.3.4/src/highrise/__init__.py
--rw-r--r--   0        0        0    16806 2023-09-01 10:44:03.337218 highrise_bot_sdk-23.3.4/src/highrise/__main__.py
--rw-r--r--   0        0        0     3064 2023-03-31 11:07:05.693250 highrise_bot_sdk-23.3.4/src/highrise/_unions.py
--rw-r--r--   0        0        0    17356 2023-09-01 10:43:23.450205 highrise_bot_sdk-23.3.4/src/highrise/models.py
--rw-r--r--   0        0        0      621 2023-06-30 16:42:03.849460 highrise_bot_sdk-23.3.4/src/highrise/models_control.py
--rw-r--r--   0        0        0     9591 2023-08-11 12:25:48.234209 highrise_bot_sdk-23.3.4/src/highrise/models_webapi.py
--rw-r--r--   0        0        0        0 2023-03-30 13:16:17.585454 highrise_bot_sdk-23.3.4/src/highrise/py.typed
--rw-r--r--   0        0        0     8842 2023-07-17 10:55:23.462681 highrise_bot_sdk-23.3.4/src/highrise/webapi.py
--rw-r--r--   0        0        0    10523 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.3.4/PKG-INFO
+-rw-r--r--   0        0        0     9978 2024-05-29 15:31:11.535391 highrise_bot_sdk-24.1.0/README.md
+-rw-r--r--   0        0        0     1037 2024-05-29 15:31:11.539547 highrise_bot_sdk-24.1.0/pyproject.toml
+-rw-r--r--   0        0        0    16280 2024-05-29 14:56:41.303754 highrise_bot_sdk-24.1.0/src/highrise/__init__.py
+-rw-r--r--   0        0        0    16806 2023-10-16 20:59:07.393072 highrise_bot_sdk-24.1.0/src/highrise/__main__.py
+-rw-r--r--   0        0        0     3064 2023-10-16 20:59:07.393171 highrise_bot_sdk-24.1.0/src/highrise/_unions.py
+-rw-r--r--   0        0        0    18010 2024-05-29 12:47:34.128839 highrise_bot_sdk-24.1.0/src/highrise/models.py
+-rw-r--r--   0        0        0      621 2023-10-16 20:59:07.393353 highrise_bot_sdk-24.1.0/src/highrise/models_control.py
+-rw-r--r--   0        0        0     9591 2023-10-16 20:59:07.393426 highrise_bot_sdk-24.1.0/src/highrise/models_webapi.py
+-rw-r--r--   0        0        0        0 2023-10-16 20:59:07.393450 highrise_bot_sdk-24.1.0/src/highrise/py.typed
+-rw-r--r--   0        0        0     8842 2023-10-16 20:59:07.393521 highrise_bot_sdk-24.1.0/src/highrise/webapi.py
+-rw-r--r--   0        0        0    10683 1970-01-01 00:00:00.000000 highrise_bot_sdk-24.1.0/PKG-INFO
```

### Comparing `highrise_bot_sdk-23.3.4/README.md` & `highrise_bot_sdk-24.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ---
 
 The Highrise Python Bot SDK is a python library for writing and running Highrise bots.
 
 First, install the library (preferably in a virtual environment):
 
 ```shell
-$ pip install highrise-bot-sdk==23.3.2
+$ pip install highrise-bot-sdk==24.1.0
 ```
 
 In the [`Settings` section of the Highrise website](https://highrise.game/account/settings), create a bot and generate the API token. You'll need the token to start your bot later.
 You will also need a room ID for your bot to connect to; the room needs to be owned by you or your bot user needs to have designer rights to enter it.
 
 Open a new file, and paste the following to get started (into `mybot.py` for example):
 
@@ -28,14 +28,20 @@
 
 ```
 $ highrise mybot:Bot <room ID> <API token>
 ```
 
 ## Changelog
 
+### 24.1.0 (2024-05-29)
+
+- Add support for world invites in invite messages
+- Add support for sending bulk messages to users (up to 100 users in one request)
+
+
 ### 23.3.4 (2023-08-11)
 
 - Support for multiple rooms.
 - Removed deprecated options in buy_room_boost and buy_voice_time.
 
 ### 23.3.3 (2023-08-11)
```

### Comparing `highrise_bot_sdk-23.3.4/pyproject.toml` & `highrise_bot_sdk-24.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "highrise-bot-sdk"
-version = "23.3.4"
+version = "24.1.0"
 description = "The Highrise Bot SDK, for running Highrise bots written in Python."
 authors = ["Pocket Worlds Inc <server@high.rs>"]
 license = "proprietary"
 readme = "README.md"
 packages = [{include = "highrise", from = "src"}]
```

### Comparing `highrise_bot_sdk-23.3.4/src/highrise/__init__.py` & `highrise_bot_sdk-24.1.0/src/highrise/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     Position,
     Reaction,
     ReactionEvent,
     ReactionRequest,
     RemoveSpeakerRequest,
     RoomModeratedEvent,
     RoomPermissions,
+    SendBulkMessageRequest,
     SendMessageRequest,
     SessionMetadata,
     SetOutfitRequest,
     TeleportRequest,
     TipReactionEvent,
     TipUserRequest,
     User,
@@ -312,19 +313,43 @@
 
     async def send_message(
         self,
         conversation_id: str,
         content: str,
         message_type: Literal["text", "invite"] = "text",
         room_id: str | None = None,
-    ) -> None:
+        world_id: str | None = None,
+    ) -> None | Error:
         """Send a message to conversation."""
-        await _do_req_no_resp(
-            self, SendMessageRequest(conversation_id, content, message_type, room_id)
+        res = await do_req_resp(
+            self,
+            SendMessageRequest(
+                conversation_id, content, message_type, room_id, world_id
+            ),
         )
+        if isinstance(res, Error):
+            return res
+        return None
+
+    async def send_message_bulk(
+        self,
+        user_ids: list[str],
+        content: str,
+        message_type: Literal["text", "invite"] = "text",
+        room_id: str | None = None,
+        world_id: str | None = None,
+    ) -> None | Error:
+        """Send a message to conversation."""
+        res = await do_req_resp(
+            self,
+            SendBulkMessageRequest(user_ids, content, message_type, room_id, world_id),
+        )
+        if isinstance(res, Error):
+            return res
+        return None
 
     async def get_messages(
         self, conversation_id: str, last_id: str | None = None
     ) -> GetMessagesRequest.GetMessagesResponse | Error:
         """Fetch messages from a conversation."""
         return await do_req_resp(self, GetMessagesRequest(conversation_id, last_id))
 
@@ -480,14 +505,15 @@
     | LeaveConversationRequest
     | BuyVoiceTimeRequest
     | BuyRoomBoostRequest
     | TipUserRequest
     | SetOutfitRequest
     | GetInventoryRequest
     | BuyItemRequest
+    | SendBulkMessageRequest
 )
 IncomingEvents = (
     Error
     | ChatEvent
     | EmoteEvent
     | ReactionEvent
     | UserJoinedEvent
```

### Comparing `highrise_bot_sdk-23.3.4/src/highrise/__main__.py` & `highrise_bot_sdk-24.1.0/src/highrise/__main__.py`

 * *Files identical despite different names*

### Comparing `highrise_bot_sdk-23.3.4/src/highrise/_unions.py` & `highrise_bot_sdk-24.1.0/src/highrise/_unions.py`

 * *Files identical despite different names*

### Comparing `highrise_bot_sdk-23.3.4/src/highrise/models.py` & `highrise_bot_sdk-24.1.0/src/highrise/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -706,31 +706,54 @@
 
     Response: ClassVar = GetConversationsResponse
 
 
 @define
 class SendMessageRequest:
     """
-    Send a message to a conversation. If bot wishes to send room invite, the room_id must be provided.
+    Send a message to a conversation. If bot wishes to send room invite, the room_id must be provided. If bot wishes to
+    send world invite, the world_id must be provided.
     """
 
     conversation_id: str
     content: str
     type: Literal["text", "invite"]
     room_id: str | None = None
+    world_id: str | None = None
     rid: str | None = None
 
     @define
     class SendMessageResponse:
         rid: str | None = None
 
     Response: ClassVar = SendMessageResponse
 
 
 @define
+class SendBulkMessageRequest:
+    """
+    Send a message to a multiple users, with limit being 100. If bot wishes to send room invite, the room_id must
+    be provided. If bot wishes to send world invite, the world_id must be provided.
+    """
+
+    user_ids: list[str]
+    content: str
+    type: Literal["text", "invite"]
+    room_id: str | None = None
+    world_id: str | None = None
+    rid: str | None = None
+
+    @define
+    class SendBulkMessageResponse:
+        rid: str | None = None
+
+    Response: ClassVar = SendBulkMessageResponse
+
+
+@define
 class GetMessagesRequest:
     """
     Get the messages of a conversation.
     20 messages will be returned at most, if all 20 messages are returned, the
      last_message_id can be used to retrieve the next 20 messages.
     """
```

### Comparing `highrise_bot_sdk-23.3.4/src/highrise/models_control.py` & `highrise_bot_sdk-24.1.0/src/highrise/models_control.py`

 * *Files identical despite different names*

### Comparing `highrise_bot_sdk-23.3.4/src/highrise/models_webapi.py` & `highrise_bot_sdk-24.1.0/src/highrise/models_webapi.py`

 * *Files identical despite different names*

### Comparing `highrise_bot_sdk-23.3.4/src/highrise/webapi.py` & `highrise_bot_sdk-24.1.0/src/highrise/webapi.py`

 * *Files identical despite different names*

### Comparing `highrise_bot_sdk-23.3.4/PKG-INFO` & `highrise_bot_sdk-24.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highrise-bot-sdk
-Version: 23.3.4
+Version: 24.1.0
 Summary: The Highrise Bot SDK, for running Highrise bots written in Python.
 License: Proprietary
 Author: Pocket Worlds Inc
 Author-email: server@high.rs
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -23,15 +23,15 @@
 ---
 
 The Highrise Python Bot SDK is a python library for writing and running Highrise bots.
 
 First, install the library (preferably in a virtual environment):
 
 ```shell
-$ pip install highrise-bot-sdk==23.3.2
+$ pip install highrise-bot-sdk==24.1.0
 ```
 
 In the [`Settings` section of the Highrise website](https://highrise.game/account/settings), create a bot and generate the API token. You'll need the token to start your bot later.
 You will also need a room ID for your bot to connect to; the room needs to be owned by you or your bot user needs to have designer rights to enter it.
 
 Open a new file, and paste the following to get started (into `mybot.py` for example):
 
@@ -48,14 +48,20 @@
 
 ```
 $ highrise mybot:Bot <room ID> <API token>
 ```
 
 ## Changelog
 
+### 24.1.0 (2024-05-29)
+
+- Add support for world invites in invite messages
+- Add support for sending bulk messages to users (up to 100 users in one request)
+
+
 ### 23.3.4 (2023-08-11)
 
 - Support for multiple rooms.
 - Removed deprecated options in buy_room_boost and buy_voice_time.
 
 ### 23.3.3 (2023-08-11)
```

