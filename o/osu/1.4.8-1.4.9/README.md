# Comparing `tmp/osu-1.4.8.tar.gz` & `tmp/osu-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osu-1.4.8.tar", last modified: Tue May 21 23:26:44 2024, max compression
+gzip compressed data, was "osu-1.4.9.tar", last modified: Fri May 31 15:37:47 2024, max compression
```

## Comparing `osu-1.4.8.tar` & `osu-1.4.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:26:44.733149 osu-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-21 23:26:37.000000 osu-1.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-21 23:26:44.733149 osu-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-21 23:26:37.000000 osu-1.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:26:44.729149 osu-1.4.8/osu/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-21 23:26:37.000000 osu-1.4.8/osu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:26:44.729149 osu-1.4.8/osu/api/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-21 23:26:37.000000 osu-1.4.8/osu/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16326 2024-05-21 23:26:37.000000 osu-1.4.8/osu/api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-21 23:26:37.000000 osu-1.4.8/osu/api/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:26:44.729149 osu-1.4.8/osu/bancho/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-21 23:26:37.000000 osu-1.4.8/osu/bancho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-05-21 23:26:37.000000 osu-1.4.8/osu/bancho/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15611 2024-05-21 23:26:37.000000 osu-1.4.8/osu/bancho/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    16165 2024-05-21 23:26:37.000000 osu-1.4.8/osu/bancho/packets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-05-21 23:26:37.000000 osu-1.4.8/osu/bancho/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-21 23:26:37.000000 osu-1.4.8/osu/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-05-21 23:26:37.000000 osu-1.4.8/osu/game.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:26:44.733149 osu-1.4.8/osu/objects/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-21 23:26:37.000000 osu-1.4.8/osu/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-21 23:26:37.000000 osu-1.4.8/osu/objects/beatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-21 23:26:37.000000 osu-1.4.8/osu/objects/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-05-21 23:26:37.000000 osu-1.4.8/osu/objects/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-21 23:26:37.000000 osu-1.4.8/osu/objects/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-21 23:26:37.000000 osu-1.4.8/osu/objects/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-21 23:26:37.000000 osu-1.4.8/osu/objects/lists.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-21 23:26:37.000000 osu-1.4.8/osu/objects/player.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-21 23:26:37.000000 osu-1.4.8/osu/objects/replays.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-21 23:26:37.000000 osu-1.4.8/osu/objects/score.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-21 23:26:37.000000 osu-1.4.8/osu/objects/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-21 23:26:37.000000 osu-1.4.8/osu/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:26:44.733149 osu-1.4.8/osu/tcp/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-21 23:26:37.000000 osu-1.4.8/osu/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-21 23:26:37.000000 osu-1.4.8/osu/tcp/bancho.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-21 23:26:37.000000 osu-1.4.8/osu/tcp/game.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:26:44.733149 osu-1.4.8/osu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-21 23:26:44.000000 osu-1.4.8/osu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-21 23:26:44.000000 osu-1.4.8/osu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 23:26:44.000000 osu-1.4.8/osu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-21 23:26:44.000000 osu-1.4.8/osu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 23:26:44.000000 osu-1.4.8/osu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 23:26:44.733149 osu-1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-21 23:26:37.000000 osu-1.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:37:47.572342 osu-1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-31 15:37:42.000000 osu-1.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-31 15:37:47.572342 osu-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-31 15:37:42.000000 osu-1.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:37:47.568342 osu-1.4.9/osu/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-31 15:37:42.000000 osu-1.4.9/osu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:37:47.568342 osu-1.4.9/osu/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-31 15:37:42.000000 osu-1.4.9/osu/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16326 2024-05-31 15:37:42.000000 osu-1.4.9/osu/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-31 15:37:42.000000 osu-1.4.9/osu/api/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:37:47.568342 osu-1.4.9/osu/bancho/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-31 15:37:42.000000 osu-1.4.9/osu/bancho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-05-31 15:37:42.000000 osu-1.4.9/osu/bancho/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15611 2024-05-31 15:37:42.000000 osu-1.4.9/osu/bancho/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16165 2024-05-31 15:37:42.000000 osu-1.4.9/osu/bancho/packets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-05-31 15:37:42.000000 osu-1.4.9/osu/bancho/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-31 15:37:42.000000 osu-1.4.9/osu/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-05-31 15:37:42.000000 osu-1.4.9/osu/game.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:37:47.572342 osu-1.4.9/osu/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-31 15:37:42.000000 osu-1.4.9/osu/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-31 15:37:42.000000 osu-1.4.9/osu/objects/beatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-31 15:37:42.000000 osu-1.4.9/osu/objects/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-05-31 15:37:42.000000 osu-1.4.9/osu/objects/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-31 15:37:42.000000 osu-1.4.9/osu/objects/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-31 15:37:42.000000 osu-1.4.9/osu/objects/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-31 15:37:42.000000 osu-1.4.9/osu/objects/lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-31 15:37:42.000000 osu-1.4.9/osu/objects/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-31 15:37:42.000000 osu-1.4.9/osu/objects/replays.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-31 15:37:42.000000 osu-1.4.9/osu/objects/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-31 15:37:42.000000 osu-1.4.9/osu/objects/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-31 15:37:42.000000 osu-1.4.9/osu/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:37:47.572342 osu-1.4.9/osu/tcp/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-31 15:37:42.000000 osu-1.4.9/osu/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-31 15:37:42.000000 osu-1.4.9/osu/tcp/bancho.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-31 15:37:42.000000 osu-1.4.9/osu/tcp/game.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:37:47.572342 osu-1.4.9/osu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-31 15:37:47.000000 osu-1.4.9/osu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-31 15:37:47.000000 osu-1.4.9/osu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:37:47.000000 osu-1.4.9/osu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-31 15:37:47.000000 osu-1.4.9/osu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-31 15:37:47.000000 osu-1.4.9/osu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:37:47.572342 osu-1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-31 15:37:42.000000 osu-1.4.9/setup.py
```

### Comparing `osu-1.4.8/LICENSE` & `osu-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `osu-1.4.8/PKG-INFO` & `osu-1.4.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: osu
-Version: 1.4.8
+Version: 1.4.9
 Summary: A python library that emulates the osu! stable client
 Author: Lekuru
 Author-email: contact@lekuru.xyz
 Keywords: osu,osugame,python,bancho
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-dateutil==2.9.0.post0
-Requires-Dist: requests==2.32.0
+Requires-Dist: requests==2.32.2
 Requires-Dist: psutil==5.9.8
 Requires-Dist: wmi; platform_system == "Windows"
 
 # osu.py
 
 [![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
 [![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/Lekuruu/osu.py/blob/main/LICENSE)
 
 osu.py is a python library that emulates part of the online functionality of the osu! stable client.
 
 **IMPORTANT:**
-Use this library at your own risk! I am not responsible for anything that can happen to your account. If you want to test it out on a private server, you can set the `server` attribute when initializing the client.
+Use this library at your own risk! I am not responsible for any unexpected behavior of the client or anything that can happen to your account. If you want to test it out on a custom server, you can set the `server` attribute when initializing the client.
 
 You can install this package with pip:
 
 ```shell
 pip install osu
 ```
 
@@ -43,17 +43,18 @@
 - [x] Sending/Receiving chat messages
 - [x] Spectating
 - [x] Avatars
 - [x] Comments
 - [x] Replays
 - [x] Scores/Leaderboards
 - [x] Tournament client behaviour
-- [x] osu!direct
-- [ ] Documentation
+- [x] Direct Search
+- [x] Direct Download
 - [ ] Multiplayer
+- [ ] Documentation
 
 ## Example
 
 Here is a small example of how to use this package:
 
 ```python
 from osu.bancho.constants import ServerPackets
@@ -72,15 +73,15 @@
   USERNAME,
   PASSWORD
 )
 
 # Simple message handler
 @game.events.register(ServerPackets.SEND_MESSAGE)
 def on_message(sender: Player, message: str, target: Player):
-  if message.startswith('!ping'):
+  if message.startswith('?ping'):
     sender.send_message('pong!')
 
 # Run the game
 game.run()
 ```
 
 You can also run tasks, independent of server actions:
```

### Comparing `osu-1.4.8/README.md` & `osu-1.4.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
 [![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/Lekuruu/osu.py/blob/main/LICENSE)
 
 osu.py is a python library that emulates part of the online functionality of the osu! stable client.
 
 **IMPORTANT:**
-Use this library at your own risk! I am not responsible for anything that can happen to your account. If you want to test it out on a private server, you can set the `server` attribute when initializing the client.
+Use this library at your own risk! I am not responsible for any unexpected behavior of the client or anything that can happen to your account. If you want to test it out on a custom server, you can set the `server` attribute when initializing the client.
 
 You can install this package with pip:
 
 ```shell
 pip install osu
 ```
 
@@ -29,17 +29,18 @@
 - [x] Sending/Receiving chat messages
 - [x] Spectating
 - [x] Avatars
 - [x] Comments
 - [x] Replays
 - [x] Scores/Leaderboards
 - [x] Tournament client behaviour
-- [x] osu!direct
-- [ ] Documentation
+- [x] Direct Search
+- [x] Direct Download
 - [ ] Multiplayer
+- [ ] Documentation
 
 ## Example
 
 Here is a small example of how to use this package:
 
 ```python
 from osu.bancho.constants import ServerPackets
@@ -58,15 +59,15 @@
   USERNAME,
   PASSWORD
 )
 
 # Simple message handler
 @game.events.register(ServerPackets.SEND_MESSAGE)
 def on_message(sender: Player, message: str, target: Player):
-  if message.startswith('!ping'):
+  if message.startswith('?ping'):
     sender.send_message('pong!')
 
 # Run the game
 game.run()
 ```
 
 You can also run tasks, independent of server actions:
```

### Comparing `osu-1.4.8/osu/api/client.py` & `osu-1.4.9/osu/api/client.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.8/osu/api/constants.py` & `osu-1.4.9/osu/api/constants.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.8/osu/bancho/client.py` & `osu-1.4.9/osu/bancho/client.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.8/osu/bancho/constants.py` & `osu-1.4.9/osu/bancho/constants.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.8/osu/bancho/packets.py` & `osu-1.4.9/osu/bancho/packets.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.8/osu/bancho/streams.py` & `osu-1.4.9/osu/bancho/streams.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.8/osu/events.py` & `osu-1.4.9/osu/events.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.8/osu/game.py` & `osu-1.4.9/osu/game.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.8/osu/objects/beatmap.py` & `osu-1.4.9/osu/objects/beatmap.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.8/osu/objects/channel.py` & `osu-1.4.9/osu/objects/channel.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.8/osu/objects/client.py` & `osu-1.4.9/osu/objects/client.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.8/osu/objects/collections.py` & `osu-1.4.9/osu/objects/collections.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.8/osu/objects/lists.py` & `osu-1.4.9/osu/objects/lists.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.8/osu/objects/player.py` & `osu-1.4.9/osu/objects/player.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.8/osu/objects/replays.py` & `osu-1.4.9/osu/objects/replays.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.8/osu/objects/score.py` & `osu-1.4.9/osu/objects/score.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.8/osu/objects/status.py` & `osu-1.4.9/osu/objects/status.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.8/osu/tasks.py` & `osu-1.4.9/osu/tasks.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.8/osu/tcp/bancho.py` & `osu-1.4.9/osu/tcp/bancho.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,78 +76,67 @@
         try:
             self.socket.connect((self.ip, self.port))
             self.socket.send(login_data.encode())
             self.connected = True
         except ConnectionRefusedError:
             self.logger.error("Connection refused by the server.")
 
-    def get_packet(self) -> Tuple[int, StreamIn]:
-        """Get a packet from the server"""
-        packet_header = StreamIn(self.socket.recv(7))
-
-        packet_id = packet_header.u16()
-        compression = packet_header.bool()
-        packet_size = packet_header.u32()
-        packet_data = self.socket.recv(packet_size)
+    def process_packets(self) -> None:
+        """Process incoming packets from the server"""
+        while True:
+            packet_header = StreamIn(self.socket.recv(7))
+
+            if packet_header.eof():
+                return
+
+            packet_id = packet_header.u16()
+            compression = packet_header.bool()
+            packet_size = packet_header.u32()
+            packet_data = self.socket.recv(packet_size)
 
-        if compression:
-            packet_data = gzip.decompress(packet_data)
+            if compression:
+                packet_data = gzip.decompress(packet_data)
 
-        return ServerPackets(packet_id), StreamIn(packet_data)
+            packet, stream = ServerPackets(packet_id), StreamIn(packet_data)
+
+            self.logger.debug(f'Received packet {packet.name} -> "{stream.get()}"')
+            self.game.packets.packet_received(packet, stream, self.game)
 
     def enqueue(
-        self, packet: ClientPackets, data: bytes = b"", dequeue: bool = True
+        self, packet: ClientPackets, data: bytes = b"", dequeue: bool = False
     ) -> bytes:
-        """Send a packet to the queue and dequeue"""
+        """Send a packet to the server and dequeue"""
         stream = StreamOut()
 
         # Construct header
         stream.u16(packet.value)
         stream.bool(False)
         stream.u32(len(data))
         stream.write(data)
 
         self.logger.debug(f'Sending {packet.name} -> "{data}"')
-
-        # Append to queue
-        self.queue.put(stream.get())
+        self.socket.send(stream.get())
+        self.last_action = datetime.now().timestamp()
 
         if dequeue:
             self.dequeue()
 
         return stream.get()
 
     def dequeue(self) -> None:
-        """Send a request to bancho, empty the queue and handle incoming packets"""
-        if not self.connected and self.queue.empty():
-            return
-
-        data = b""
-
-        while not self.queue.empty():
-            data += self.queue.get()
-
-        if data:
-            self.socket.send(data)
-            self.last_action = datetime.now().timestamp()
-
+        """Process all incoming packets from the server"""
         if not self.connected:
             return
 
         try:
-            packet, stream = self.get_packet()
+            self.process_packets()
         except OverflowError as e:
-            self.logger.error(f'Failed to receive packet: "{e}"')
+            self.logger.error(f'Failed to process packets: "{e}"')
             self.connected = False
             self.retry = True
-            return
-
-        self.logger.debug(f'Received packet {packet.name} -> "{stream.get()}"')
-
-        self.game.packets.packet_received(packet, stream, self.game)
 
     def exit(self):
         """Send logout packet to bancho, and disconnect."""
         try:
             self.retry = False
             self.connected = False
             self.enqueue(ClientPackets.LOGOUT, int(0).to_bytes(4, "little"))
```

### Comparing `osu-1.4.8/osu/tcp/game.py` & `osu-1.4.9/osu/tcp/game.py`

 * *Files identical despite different names*

### Comparing `osu-1.4.8/osu.egg-info/PKG-INFO` & `osu-1.4.9/osu.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: osu
-Version: 1.4.8
+Version: 1.4.9
 Summary: A python library that emulates the osu! stable client
 Author: Lekuru
 Author-email: contact@lekuru.xyz
 Keywords: osu,osugame,python,bancho
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-dateutil==2.9.0.post0
-Requires-Dist: requests==2.32.0
+Requires-Dist: requests==2.32.2
 Requires-Dist: psutil==5.9.8
 Requires-Dist: wmi; platform_system == "Windows"
 
 # osu.py
 
 [![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
 [![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/Lekuruu/osu.py/blob/main/LICENSE)
 
 osu.py is a python library that emulates part of the online functionality of the osu! stable client.
 
 **IMPORTANT:**
-Use this library at your own risk! I am not responsible for anything that can happen to your account. If you want to test it out on a private server, you can set the `server` attribute when initializing the client.
+Use this library at your own risk! I am not responsible for any unexpected behavior of the client or anything that can happen to your account. If you want to test it out on a custom server, you can set the `server` attribute when initializing the client.
 
 You can install this package with pip:
 
 ```shell
 pip install osu
 ```
 
@@ -43,17 +43,18 @@
 - [x] Sending/Receiving chat messages
 - [x] Spectating
 - [x] Avatars
 - [x] Comments
 - [x] Replays
 - [x] Scores/Leaderboards
 - [x] Tournament client behaviour
-- [x] osu!direct
-- [ ] Documentation
+- [x] Direct Search
+- [x] Direct Download
 - [ ] Multiplayer
+- [ ] Documentation
 
 ## Example
 
 Here is a small example of how to use this package:
 
 ```python
 from osu.bancho.constants import ServerPackets
@@ -72,15 +73,15 @@
   USERNAME,
   PASSWORD
 )
 
 # Simple message handler
 @game.events.register(ServerPackets.SEND_MESSAGE)
 def on_message(sender: Player, message: str, target: Player):
-  if message.startswith('!ping'):
+  if message.startswith('?ping'):
     sender.send_message('pong!')
 
 # Run the game
 game.run()
 ```
 
 You can also run tasks, independent of server actions:
```

### Comparing `osu-1.4.8/osu.egg-info/SOURCES.txt` & `osu-1.4.9/osu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osu-1.4.8/setup.py` & `osu-1.4.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     long_description = f.read()
 
 with open(os.path.join(current_directory, "requirements.txt"), "r") as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="osu",
-    version="1.4.8",
+    version="1.4.9",
     author="Lekuru",
     author_email="contact@lekuru.xyz",
     description="A python library that emulates the osu! stable client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=requirements,
```

