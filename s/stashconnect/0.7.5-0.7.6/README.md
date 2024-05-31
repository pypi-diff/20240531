# Comparing `tmp/stashconnect-0.7.5.tar.gz` & `tmp/stashconnect-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stashconnect-0.7.5.tar", last modified: Fri May 31 07:06:51 2024, max compression
+gzip compressed data, was "stashconnect-0.7.6.tar", last modified: Fri May 31 20:43:26 2024, max compression
```

## Comparing `stashconnect-0.7.5.tar` & `stashconnect-0.7.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 07:06:51.973674 stashconnect-0.7.5/
--rw-rw-rw-   0        0        0     1087 2024-04-21 06:28:56.000000 stashconnect-0.7.5/LICENSE
--rw-rw-rw-   0        0        0     1586 2024-05-31 07:06:51.969653 stashconnect-0.7.5/PKG-INFO
--rw-rw-rw-   0        0        0      551 2024-05-31 07:04:06.000000 stashconnect-0.7.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-31 07:06:51.974180 stashconnect-0.7.5/setup.cfg
--rw-rw-rw-   0        0        0     1380 2024-05-31 06:38:24.000000 stashconnect-0.7.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:06:51.945594 stashconnect-0.7.5/stashconnect/
--rw-rw-rw-   0        0        0      216 2024-05-31 07:03:45.000000 stashconnect-0.7.5/stashconnect/__init__.py
--rw-rw-rw-   0        0        0    17257 2024-05-10 18:47:16.000000 stashconnect-0.7.5/stashconnect/channels.py
--rw-rw-rw-   0        0        0     9234 2024-05-31 07:01:44.000000 stashconnect-0.7.5/stashconnect/client.py
--rw-rw-rw-   0        0        0     3618 2024-05-10 20:37:19.000000 stashconnect-0.7.5/stashconnect/companies.py
--rw-rw-rw-   0        0        0     4704 2024-05-31 06:25:48.000000 stashconnect-0.7.5/stashconnect/conversations.py
--rw-rw-rw-   0        0        0     2584 2024-04-25 17:41:41.000000 stashconnect-0.7.5/stashconnect/crypto_utils.py
--rw-rw-rw-   0        0        0     9567 2024-05-30 21:29:23.000000 stashconnect-0.7.5/stashconnect/files.py
--rw-rw-rw-   0        0        0     6298 2024-05-30 19:29:31.000000 stashconnect-0.7.5/stashconnect/messages.py
--rw-rw-rw-   0        0        0    17343 2024-05-11 08:24:59.000000 stashconnect-0.7.5/stashconnect/models.py
--rw-rw-rw-   0        0        0     1458 2024-05-07 15:16:08.000000 stashconnect-0.7.5/stashconnect/settings.py
--rw-rw-rw-   0        0        0      926 2024-04-29 18:11:09.000000 stashconnect-0.7.5/stashconnect/tools.py
--rw-rw-rw-   0        0        0     2101 2024-05-10 15:03:08.000000 stashconnect-0.7.5/stashconnect/users.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:06:51.966153 stashconnect-0.7.5/stashconnect.egg-info/
--rw-rw-rw-   0        0        0     1586 2024-05-31 07:06:51.000000 stashconnect-0.7.5/stashconnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2024-05-31 07:06:51.000000 stashconnect-0.7.5/stashconnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 07:06:51.000000 stashconnect-0.7.5/stashconnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-05-31 07:06:51.000000 stashconnect-0.7.5/stashconnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-31 07:06:51.000000 stashconnect-0.7.5/stashconnect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 20:43:26.636630 stashconnect-0.7.6/
+-rw-rw-rw-   0        0        0     1087 2024-04-21 06:28:56.000000 stashconnect-0.7.6/LICENSE
+-rw-rw-rw-   0        0        0     1728 2024-05-31 20:43:26.633619 stashconnect-0.7.6/PKG-INFO
+-rw-rw-rw-   0        0        0      693 2024-05-31 07:27:08.000000 stashconnect-0.7.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-31 20:43:26.637129 stashconnect-0.7.6/setup.cfg
+-rw-rw-rw-   0        0        0     1380 2024-05-31 20:41:53.000000 stashconnect-0.7.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 20:43:26.612070 stashconnect-0.7.6/stashconnect/
+-rw-rw-rw-   0        0        0      216 2024-05-31 20:41:35.000000 stashconnect-0.7.6/stashconnect/__init__.py
+-rw-rw-rw-   0        0        0    17257 2024-05-10 18:47:16.000000 stashconnect-0.7.6/stashconnect/channels.py
+-rw-rw-rw-   0        0        0     9246 2024-05-31 20:41:47.000000 stashconnect-0.7.6/stashconnect/client.py
+-rw-rw-rw-   0        0        0     3618 2024-05-10 20:37:19.000000 stashconnect-0.7.6/stashconnect/companies.py
+-rw-rw-rw-   0        0        0     4704 2024-05-31 06:25:48.000000 stashconnect-0.7.6/stashconnect/conversations.py
+-rw-rw-rw-   0        0        0     2584 2024-04-25 17:41:41.000000 stashconnect-0.7.6/stashconnect/crypto_utils.py
+-rw-rw-rw-   0        0        0    12358 2024-05-31 20:31:12.000000 stashconnect-0.7.6/stashconnect/files.py
+-rw-rw-rw-   0        0        0     6298 2024-05-30 19:29:31.000000 stashconnect-0.7.6/stashconnect/messages.py
+-rw-rw-rw-   0        0        0    17343 2024-05-11 08:24:59.000000 stashconnect-0.7.6/stashconnect/models.py
+-rw-rw-rw-   0        0        0     1458 2024-05-07 15:16:08.000000 stashconnect-0.7.6/stashconnect/settings.py
+-rw-rw-rw-   0        0        0     1001 2024-05-31 18:50:21.000000 stashconnect-0.7.6/stashconnect/tools.py
+-rw-rw-rw-   0        0        0     2101 2024-05-10 15:03:08.000000 stashconnect-0.7.6/stashconnect/users.py
+drwxrwxrwx   0        0        0        0 2024-05-31 20:43:26.630619 stashconnect-0.7.6/stashconnect.egg-info/
+-rw-rw-rw-   0        0        0     1728 2024-05-31 20:43:26.000000 stashconnect-0.7.6/stashconnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2024-05-31 20:43:26.000000 stashconnect-0.7.6/stashconnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 20:43:26.000000 stashconnect-0.7.6/stashconnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-05-31 20:43:26.000000 stashconnect-0.7.6/stashconnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 20:43:26.000000 stashconnect-0.7.6/stashconnect.egg-info/top_level.txt
```

### Comparing `stashconnect-0.7.5/LICENSE` & `stashconnect-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.5/PKG-INFO` & `stashconnect-0.7.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashconnect
-Version: 0.7.5
+Version: 0.7.6
 Summary: An API wrapper for stashcat and schul.cloud.
 Home-page: https://github.com/BuStudios/StashConnect
 Author: BuStudios
 Author-email: support@bustudios.org
 Project-URL: Bug Tracker, https://github.com/BuStudios/StashConnect/issues
 Project-URL: Documentation, https://github.com/BuStudios/StashConnect/wiki
 Project-URL: Source Code, https://github.com/BuStudios/StashConnect
@@ -19,19 +19,19 @@
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: pycryptodome
 Requires-Dist: python-socketio
 Requires-Dist: Pillow
 Requires-Dist: websocket-client
 
-# <img src="assets/icon.png" height="22"> StashConnect
+# <img src="https://raw.githubusercontent.com/BuStudios/StashConnect/main/assets/icon.png" height="22"> StashConnect
 
 An API wrapper for [stashcat](https://stashcat.com/) and [schul.cloud](https://schul.cloud).<br>
-```
-unfinished
+```bash
+pip install stashconnect
 ```
 
 ## Contributors
 - All code made by [BuStudios](https://github.com/bustudios)
 - Create a pull request to contribute code yourself
 
 ## Version 0.7.5
@@ -39,8 +39,8 @@
 - [x] fix links
 - [ ] returnable file object
 - [ ] bot file for easy bot setup
 
 ---
 StashConnect is not affiliated with Stashcat GmbH or any of its affiliates.
 
-<img src="assets/icon-full.png">
+<img src="https://raw.githubusercontent.com/BuStudios/StashConnect/main/assets/icon-full.png">
```

### Comparing `stashconnect-0.7.5/setup.py` & `stashconnect-0.7.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.7.5"
+VERSION = "0.7.6"
 DESCRIPTION = "An API wrapper for stashcat and schul.cloud."
 
 setup(
     name="stashconnect",
     version=VERSION,
     author="BuStudios",
     author_email="support@bustudios.org",
```

### Comparing `stashconnect-0.7.5/stashconnect/channels.py` & `stashconnect-0.7.6/stashconnect/channels.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.5/stashconnect/client.py` & `stashconnect-0.7.6/stashconnect/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from .messages import MessageManager
 from .settings import Settings
 from .users import UserManager
 from .crypto_utils import CryptoUtils
 from .conversations import ConversationManager
 from .companies import CompanyManager
 from .channels import ChannelManager
+from .files import FileManager
 
-from .files import Files
 from .tools import Tools
 
 from .models import Message
 
 headers = {
     "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36",
     "Accept": "application/json, text/plain, */*",
@@ -45,25 +45,25 @@
 
     def __init__(self, *, email, password, encryption_password=None, device_id=None, app_name=None):
 
         self.messages = MessageManager(self)
         self.tools = Tools(self)
         self.settings = Settings(self)
         self.users = UserManager(self)
-        self.files = Files(self)
+        self.files = FileManager(self)
         self.conversations = ConversationManager(self)
         self.companies = CompanyManager(self)
         self.channels = ChannelManager(self)
 
         self.email = email
         self.password = password
         self.encryption_password = encryption_password
 
         self.device_id = "stashconnect" if device_id is None else device_id
-        self.app_name = "stashconnect v.0.7.5" if app_name is None else app_name
+        self.app_name = "stashconnect v.0.7.6" if app_name is None else app_name
 
         self._main_url = "https://api.stashcat.com/"
         self._push_url = "https://push.stashcat.com/"
 
         self._headers = headers
         self._session = requests.Session()
         self._session.headers.update(self._headers)
```

### Comparing `stashconnect-0.7.5/stashconnect/companies.py` & `stashconnect-0.7.6/stashconnect/companies.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.5/stashconnect/conversations.py` & `stashconnect-0.7.6/stashconnect/conversations.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.5/stashconnect/crypto_utils.py` & `stashconnect-0.7.6/stashconnect/crypto_utils.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.5/stashconnect/files.py` & `stashconnect-0.7.6/stashconnect/files.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,25 +10,40 @@
 import io
 import json
 
 from .crypto_utils import CryptoUtils
 from .models import Channel, Conversation
 
 
-class Files:
+class FileManager:
     def __init__(self, client):
         self.client = client
 
-    def quota(self):
+    def quota(self) -> dict:
+        """Gets the users quota
+
+        Returns:
+            dict: The users quota.
+        """
         response = self.client._post(
             "file/quota", data={"type": "personal", "type_id": self.client.user_id}
         )
         return response["quota"]
 
-    def upload(self, target, filepath, encrypted=True):
+    def upload(self, target: str | int, filepath: str, encrypted: bool = True) -> dict:
+        """Uploads a file to a target location
+
+        Args:
+            target (str | int): The upolads target id.
+            filepath (str): The files location path.
+            encrypted (bool, optional): Sets wether a file should be encrypted. Defaults to True.
+
+        Returns:
+            File: A file object.
+        """
         filename = os.path.basename(filepath)
 
         if encrypted:
             if self.client._private_key is None:
                 print(
                     "Could not upload encrypted file as no encryption password was provided"
                 )
@@ -151,15 +166,24 @@
             self.client._post("file/storePreviewImage", data=data)
 
         except Exception:
             pass
 
         return file
 
-    def download(self, id, directory=""):
+    def download(self, id: str | int, directory: str = "") -> str:
+        """Downloads a file to a local location
+
+        Args:
+            id (str | int): The files id.
+            directory (str, optional): The download dir. Defaults to main.
+
+        Returns:
+            str: The path of the saved file.
+        """
         response = self.client._post(f"file/download?id={id}", data={}, return_all=True)
 
         file_info = self.client.files.file_info(id)
         file_path = os.path.join(directory, file_info["name"])
 
         with open(file_path, "wb") as file:
 
@@ -186,19 +210,35 @@
                 )
                 file.write(decrypted)
             else:
                 file.write(response.content)
 
         return file_path
 
-    def info(self, id):
+    def info(self, id: str | int) -> dict:
+        """Fetches the info of a file
+
+        Args:
+            id (str | int): The files id.
+
+        Returns:
+            File: A file object.
+        """
         response = self.client._post("file/info", data={"file_id": id})
         return response["file"]
 
-    def delete(self, ids):
+    def delete(self, ids: str | int | list) -> dict:
+        """Deletes specified files
+
+        Args:
+            ids (str | int | list): The file or files ids
+
+        Returns:
+            dict: The success status.
+        """
 
         ids_sent = []
 
         if isinstance(ids, str | int):
             ids_sent = [ids]
         else:
             ids_sent = ids
@@ -236,15 +276,14 @@
         response = self.client._post("file/rename", data=data)
         return response
 
     def copy(
         self,
         id: str | int,
         folder_id: str | int = 0,
-        type: str = "personal",
         type_id: str | int = None,
     ):
         """Copies a file to a folder.
 
         Args:
             id (str | int): The files id.
             folder_id (str | int, optional): The new folders id. Defaults to main.
@@ -252,18 +291,21 @@
             type_id (str | int, optional): The destinations type id. Defaults to client.user_id.
 
         Returns:
             File: A file object.
         """
         if type_id is None:
             type_id = self.client.user_id
+
+        target_type = self.client.tools.get_type(type_id)
+
         data = {
             "file_id": id,
             "folder_id": folder_id,
-            "type": type,
+            "type": target_type,
             "type_id": type_id,
         }
         response = self.client._post("file/copy", data=data)
         return response["file"]
 
     def shares(self, id: str | int) -> dict:
         """Get a files shares
@@ -285,7 +327,49 @@
         for conversation in response["conversations"]:
             conversations.append(Conversation(self.client, conversation))
 
         response["channels"] = channels
         response["conversations"] = conversations
 
         return response
+
+    def get(
+        self,
+        folder_id: str | int = 0,
+        type_id: str | int = None,
+        folder_only: str = "no",
+        offset: int | str = 0,
+        limit: int | str = 75,
+        search: str = None,
+        sorting: str = "created_asc",
+    ) -> dict:
+        """Gets the files and folders in a dir. Defaults to personal
+
+        Args:
+            folder_id (str | int, optional): The folders id. Defaults to 0 (personal).
+            type_id (str | int, optional): The type id. Defaults to None.
+            folder_only (str, optional): Set that only folder should be shown. Defaults to "no".
+            offset (int | str, optional): The response offset. Defaults to 0.
+            limit (int | str, optional): The response limit. Defaults to 75.
+            search (str, optional): The search prompt. Defaults to None.
+            sorting (str, optional): The sorting setting. Defaults to "created_asc".
+
+        Returns:
+            dict: A dictonary containing folder and file objects.
+        """
+        if type_id is None:
+            type_id = self.client.user_id
+
+        target_type = self.client.tools.get_type(type_id)
+        data = {
+            "folder_id": folder_id,
+            "type": target_type,
+            "type_id": type_id,
+            "folder_only": folder_only,
+            "offset": offset,
+            "limit": limit,
+            "search": search,
+            "sorting": sorting,
+        }
+
+        response = self.client._post("folder/get", data=data)
+        return response["content"]
```

### Comparing `stashconnect-0.7.5/stashconnect/messages.py` & `stashconnect-0.7.6/stashconnect/messages.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.5/stashconnect/models.py` & `stashconnect-0.7.6/stashconnect/models.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.5/stashconnect/settings.py` & `stashconnect-0.7.6/stashconnect/settings.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.5/stashconnect/tools.py` & `stashconnect-0.7.6/stashconnect/tools.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,16 @@
         self.client = client
 
     def get_type(self, type_id):
         """Returns type (conversation or channel)
         Args:
             type_id (int | str): The conversation or channel id
         """
+        if type_id == self.client.user_id:
+            return "personal"
 
         conversation_data = {
             "conversation_id": type_id,
             "source": "conversation",
             "limit": 0,
             "offset": 0,
         }
```

### Comparing `stashconnect-0.7.5/stashconnect/users.py` & `stashconnect-0.7.6/stashconnect/users.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.5/stashconnect.egg-info/PKG-INFO` & `stashconnect-0.7.6/stashconnect.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashconnect
-Version: 0.7.5
+Version: 0.7.6
 Summary: An API wrapper for stashcat and schul.cloud.
 Home-page: https://github.com/BuStudios/StashConnect
 Author: BuStudios
 Author-email: support@bustudios.org
 Project-URL: Bug Tracker, https://github.com/BuStudios/StashConnect/issues
 Project-URL: Documentation, https://github.com/BuStudios/StashConnect/wiki
 Project-URL: Source Code, https://github.com/BuStudios/StashConnect
@@ -19,19 +19,19 @@
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: pycryptodome
 Requires-Dist: python-socketio
 Requires-Dist: Pillow
 Requires-Dist: websocket-client
 
-# <img src="assets/icon.png" height="22"> StashConnect
+# <img src="https://raw.githubusercontent.com/BuStudios/StashConnect/main/assets/icon.png" height="22"> StashConnect
 
 An API wrapper for [stashcat](https://stashcat.com/) and [schul.cloud](https://schul.cloud).<br>
-```
-unfinished
+```bash
+pip install stashconnect
 ```
 
 ## Contributors
 - All code made by [BuStudios](https://github.com/bustudios)
 - Create a pull request to contribute code yourself
 
 ## Version 0.7.5
@@ -39,8 +39,8 @@
 - [x] fix links
 - [ ] returnable file object
 - [ ] bot file for easy bot setup
 
 ---
 StashConnect is not affiliated with Stashcat GmbH or any of its affiliates.
 
-<img src="assets/icon-full.png">
+<img src="https://raw.githubusercontent.com/BuStudios/StashConnect/main/assets/icon-full.png">
```

