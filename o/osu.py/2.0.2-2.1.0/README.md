# Comparing `tmp/osu_py-2.0.2.tar.gz` & `tmp/osu_py-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osu_py-2.0.2.tar", last modified: Thu May  2 00:49:30 2024, max compression
+gzip compressed data, was "osu_py-2.1.0.tar", last modified: Fri May 31 15:29:09 2024, max compression
```

## Comparing `osu_py-2.0.2.tar` & `osu_py-2.1.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 00:49:30.929842 osu_py-2.0.2/
--rw-rw-rw-   0        0        0     1094 2022-06-04 07:49:48.000000 osu_py-2.0.2/LICENSE
--rw-rw-rw-   0        0        0       24 2023-10-21 06:55:23.000000 osu_py-2.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4035 2024-05-02 00:49:30.920843 osu_py-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2869 2024-04-29 06:28:38.000000 osu_py-2.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-02 00:49:30.101345 osu_py-2.0.2/osu/
--rw-rw-rw-   0        0        0      391 2024-05-02 00:47:43.000000 osu_py-2.0.2/osu/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 00:49:30.250841 osu_py-2.0.2/osu/asyncio/
--rw-rw-rw-   0        0        0       40 2022-02-10 01:20:57.000000 osu_py-2.0.2/osu/asyncio/__init__.py
--rw-rw-rw-   0        0        0    58757 2024-04-21 06:44:56.000000 osu_py-2.0.2/osu/asyncio/client.py
--rw-rw-rw-   0        0        0     5413 2024-04-21 06:44:55.000000 osu_py-2.0.2/osu/asyncio/http.py
--rw-rw-rw-   0        0        0    12078 2024-05-02 00:14:03.000000 osu_py-2.0.2/osu/auth.py
--rw-rw-rw-   0        0        0    58021 2024-04-21 06:44:56.000000 osu_py-2.0.2/osu/client.py
--rw-rw-rw-   0        0        0     1041 2024-04-12 20:15:58.000000 osu_py-2.0.2/osu/constants.py
--rw-rw-rw-   0        0        0    31492 2023-08-02 22:55:27.000000 osu_py-2.0.2/osu/enums.py
--rw-rw-rw-   0        0        0       97 2021-06-15 19:50:18.000000 osu_py-2.0.2/osu/exceptions.py
--rw-rw-rw-   0        0        0     4412 2024-04-21 06:44:55.000000 osu_py-2.0.2/osu/http.py
--rw-rw-rw-   0        0        0     7878 2024-04-21 06:44:55.000000 osu_py-2.0.2/osu/notification.py
-drwxrwxrwx   0        0        0        0 2024-05-02 00:49:30.894843 osu_py-2.0.2/osu/objects/
--rw-rw-rw-   0        0        0      554 2023-07-31 18:42:39.000000 osu_py-2.0.2/osu/objects/__init__.py
--rw-rw-rw-   0        0        0     1222 2023-07-09 07:14:02.000000 osu_py-2.0.2/osu/objects/achievement.py
--rw-rw-rw-   0        0        0    26137 2023-10-21 06:16:49.000000 osu_py-2.0.2/osu/objects/beatmap.py
--rw-rw-rw-   0        0        0     9870 2023-07-09 07:36:16.000000 osu_py-2.0.2/osu/objects/beatmapset_event.py
--rw-rw-rw-   0        0        0     6006 2023-07-09 07:36:16.000000 osu_py-2.0.2/osu/objects/build.py
--rw-rw-rw-   0        0        0     4966 2023-07-31 18:23:23.000000 osu_py-2.0.2/osu/objects/chat.py
--rw-rw-rw-   0        0        0     7460 2023-07-09 07:36:16.000000 osu_py-2.0.2/osu/objects/comment.py
--rw-rw-rw-   0        0        0     4860 2024-05-01 23:50:50.000000 osu_py-2.0.2/osu/objects/current_user_attributes.py
--rw-rw-rw-   0        0        0     8463 2023-07-31 18:23:24.000000 osu_py-2.0.2/osu/objects/discussion.py
--rw-rw-rw-   0        0        0     8203 2023-07-31 18:44:40.000000 osu_py-2.0.2/osu/objects/event.py
--rw-rw-rw-   0        0        0     5810 2023-07-31 23:59:49.000000 osu_py-2.0.2/osu/objects/forum.py
--rw-rw-rw-   0        0        0     2416 2023-07-09 07:40:37.000000 osu_py-2.0.2/osu/objects/group.py
--rw-rw-rw-   0        0        0     2138 2023-07-09 07:41:54.000000 osu_py-2.0.2/osu/objects/kudosu.py
--rw-rw-rw-   0        0        0     5432 2023-08-01 00:00:54.000000 osu_py-2.0.2/osu/objects/match.py
--rw-rw-rw-   0        0        0    12031 2023-07-31 18:23:24.000000 osu_py-2.0.2/osu/objects/multiplayer.py
--rw-rw-rw-   0        0        0     2427 2023-07-09 08:22:08.000000 osu_py-2.0.2/osu/objects/news.py
--rw-rw-rw-   0        0        0    17563 2023-07-09 08:22:51.000000 osu_py-2.0.2/osu/objects/notification.py
--rw-rw-rw-   0        0        0     3165 2023-07-09 08:23:43.000000 osu_py-2.0.2/osu/objects/ranking.py
--rw-rw-rw-   0        0        0     1691 2023-07-09 07:36:16.000000 osu_py-2.0.2/osu/objects/scope.py
--rw-rw-rw-   0        0        0    13178 2024-04-20 05:34:50.000000 osu_py-2.0.2/osu/objects/score.py
--rw-rw-rw-   0        0        0     1327 2023-07-09 07:36:16.000000 osu_py-2.0.2/osu/objects/seasonal_background.py
--rw-rw-rw-   0        0        0    29585 2024-04-20 05:16:20.000000 osu_py-2.0.2/osu/objects/user.py
--rw-rw-rw-   0        0        0     2001 2023-07-09 07:36:16.000000 osu_py-2.0.2/osu/objects/wiki.py
--rw-rw-rw-   0        0        0     6612 2024-04-20 05:44:23.000000 osu_py-2.0.2/osu/path.py
--rw-rw-rw-   0        0        0     9104 2024-04-21 08:54:44.000000 osu_py-2.0.2/osu/results.py
--rw-rw-rw-   0        0        0    12080 2023-10-21 06:16:48.000000 osu_py-2.0.2/osu/util.py
-drwxrwxrwx   0        0        0        0 2024-05-02 00:49:30.901342 osu_py-2.0.2/osu.py.egg-info/
--rw-rw-rw-   0        0        0     4035 2024-05-02 00:49:29.000000 osu_py-2.0.2/osu.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1003 2024-05-02 00:49:29.000000 osu_py-2.0.2/osu.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 00:49:29.000000 osu_py-2.0.2/osu.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      160 2024-05-02 00:49:29.000000 osu_py-2.0.2/osu.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-02 00:49:29.000000 osu_py-2.0.2/osu.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      204 2024-04-21 05:59:15.000000 osu_py-2.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       65 2024-04-21 05:30:36.000000 osu_py-2.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 00:49:30.930842 osu_py-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1630 2024-04-21 06:43:24.000000 osu_py-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 15:29:09.867043 osu_py-2.1.0/
+-rw-rw-rw-   0        0        0     1094 2022-06-04 07:49:48.000000 osu_py-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-10-21 06:55:23.000000 osu_py-2.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4035 2024-05-31 15:29:09.865947 osu_py-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2869 2024-04-29 06:28:38.000000 osu_py-2.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-31 15:29:09.787470 osu_py-2.1.0/osu/
+-rw-rw-rw-   0        0        0      391 2024-05-31 15:25:57.000000 osu_py-2.1.0/osu/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 15:29:09.826802 osu_py-2.1.0/osu/asyncio/
+-rw-rw-rw-   0        0        0       40 2022-02-10 01:20:57.000000 osu_py-2.1.0/osu/asyncio/__init__.py
+-rw-rw-rw-   0        0        0    60456 2024-05-03 23:20:24.000000 osu_py-2.1.0/osu/asyncio/client.py
+-rw-rw-rw-   0        0        0     5413 2024-04-21 06:44:55.000000 osu_py-2.1.0/osu/asyncio/http.py
+-rw-rw-rw-   0        0        0    12700 2024-05-03 22:51:01.000000 osu_py-2.1.0/osu/auth.py
+-rw-rw-rw-   0        0        0    59646 2024-05-03 23:20:24.000000 osu_py-2.1.0/osu/client.py
+-rw-rw-rw-   0        0        0     1041 2024-04-12 20:15:58.000000 osu_py-2.1.0/osu/constants.py
+-rw-rw-rw-   0        0        0    31492 2023-08-02 22:55:27.000000 osu_py-2.1.0/osu/enums.py
+-rw-rw-rw-   0        0        0       97 2021-06-15 19:50:18.000000 osu_py-2.1.0/osu/exceptions.py
+-rw-rw-rw-   0        0        0     4412 2024-04-21 06:44:55.000000 osu_py-2.1.0/osu/http.py
+-rw-rw-rw-   0        0        0     7878 2024-04-21 06:44:55.000000 osu_py-2.1.0/osu/notification.py
+drwxrwxrwx   0        0        0        0 2024-05-31 15:29:09.863389 osu_py-2.1.0/osu/objects/
+-rw-rw-rw-   0        0        0      554 2023-07-31 18:42:39.000000 osu_py-2.1.0/osu/objects/__init__.py
+-rw-rw-rw-   0        0        0     1222 2023-07-09 07:14:02.000000 osu_py-2.1.0/osu/objects/achievement.py
+-rw-rw-rw-   0        0        0    26137 2023-10-21 06:16:49.000000 osu_py-2.1.0/osu/objects/beatmap.py
+-rw-rw-rw-   0        0        0     9870 2023-07-09 07:36:16.000000 osu_py-2.1.0/osu/objects/beatmapset_event.py
+-rw-rw-rw-   0        0        0     6006 2023-07-09 07:36:16.000000 osu_py-2.1.0/osu/objects/build.py
+-rw-rw-rw-   0        0        0     4966 2023-07-31 18:23:23.000000 osu_py-2.1.0/osu/objects/chat.py
+-rw-rw-rw-   0        0        0     7460 2023-07-09 07:36:16.000000 osu_py-2.1.0/osu/objects/comment.py
+-rw-rw-rw-   0        0        0     4860 2024-05-01 23:50:50.000000 osu_py-2.1.0/osu/objects/current_user_attributes.py
+-rw-rw-rw-   0        0        0     8463 2023-07-31 18:23:24.000000 osu_py-2.1.0/osu/objects/discussion.py
+-rw-rw-rw-   0        0        0     8203 2023-07-31 18:44:40.000000 osu_py-2.1.0/osu/objects/event.py
+-rw-rw-rw-   0        0        0     5810 2023-07-31 23:59:49.000000 osu_py-2.1.0/osu/objects/forum.py
+-rw-rw-rw-   0        0        0     2416 2023-07-09 07:40:37.000000 osu_py-2.1.0/osu/objects/group.py
+-rw-rw-rw-   0        0        0     2138 2023-07-09 07:41:54.000000 osu_py-2.1.0/osu/objects/kudosu.py
+-rw-rw-rw-   0        0        0     5432 2023-08-01 00:00:54.000000 osu_py-2.1.0/osu/objects/match.py
+-rw-rw-rw-   0        0        0    12031 2023-07-31 18:23:24.000000 osu_py-2.1.0/osu/objects/multiplayer.py
+-rw-rw-rw-   0        0        0     2427 2023-07-09 08:22:08.000000 osu_py-2.1.0/osu/objects/news.py
+-rw-rw-rw-   0        0        0    17563 2023-07-09 08:22:51.000000 osu_py-2.1.0/osu/objects/notification.py
+-rw-rw-rw-   0        0        0     3165 2023-07-09 08:23:43.000000 osu_py-2.1.0/osu/objects/ranking.py
+-rw-rw-rw-   0        0        0     1691 2023-07-09 07:36:16.000000 osu_py-2.1.0/osu/objects/scope.py
+-rw-rw-rw-   0        0        0    13178 2024-04-20 05:34:50.000000 osu_py-2.1.0/osu/objects/score.py
+-rw-rw-rw-   0        0        0     1327 2023-07-09 07:36:16.000000 osu_py-2.1.0/osu/objects/seasonal_background.py
+-rw-rw-rw-   0        0        0    29815 2024-05-31 15:15:20.000000 osu_py-2.1.0/osu/objects/user.py
+-rw-rw-rw-   0        0        0     2001 2023-07-09 07:36:16.000000 osu_py-2.1.0/osu/objects/wiki.py
+-rw-rw-rw-   0        0        0     6752 2024-05-03 22:28:00.000000 osu_py-2.1.0/osu/path.py
+-rw-rw-rw-   0        0        0     9104 2024-04-21 08:54:44.000000 osu_py-2.1.0/osu/results.py
+-rw-rw-rw-   0        0        0    12080 2023-10-21 06:16:48.000000 osu_py-2.1.0/osu/util.py
+drwxrwxrwx   0        0        0        0 2024-05-31 15:29:09.864640 osu_py-2.1.0/osu.py.egg-info/
+-rw-rw-rw-   0        0        0     4035 2024-05-31 15:29:09.000000 osu_py-2.1.0/osu.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1003 2024-05-31 15:29:09.000000 osu_py-2.1.0/osu.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 15:29:09.000000 osu_py-2.1.0/osu.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      160 2024-05-31 15:29:09.000000 osu_py-2.1.0/osu.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-31 15:29:09.000000 osu_py-2.1.0/osu.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      204 2024-04-21 05:59:15.000000 osu_py-2.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       65 2024-04-21 05:30:36.000000 osu_py-2.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 15:29:09.868498 osu_py-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1630 2024-04-21 06:43:24.000000 osu_py-2.1.0/setup.py
```

### Comparing `osu_py-2.0.2/LICENSE` & `osu_py-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/PKG-INFO` & `osu_py-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osu.py
-Version: 2.0.2
+Version: 2.1.0
 Summary: API Wrapper for osu!api v2 written in Python.
 Home-page: https://github.com/Sheepposu/osu.py
 Author: Sheepposu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Sheepposu/osu.py/issues
 Project-URL: osu.py documentation, https://osupy.readthedocs.io/
 Project-URL: osu!api v2 documentation, https://osu.ppy.sh/docs/index.html
```

### Comparing `osu_py-2.0.2/README.rst` & `osu_py-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/asyncio/client.py` & `osu_py-2.1.0/osu/asyncio/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -721,15 +721,15 @@
 
     async def create_new_pm(
         self, target_id: int, message: str, is_action: bool, uuid: Optional[str] = None
     ) -> CreateNewPmResult:
         """
         This endpoint allows you to create a new PM channel.
 
-        Requires OAuth, scope chat.write, and a user (authorization code grant, delegate scope, or password auth)
+        Requires OAuth, scope chat.write, and a user (authorization code grant, delegate scope)
 
         **Parameters**
 
         target_id: :class:`int`
             user_id of user to start PM with
 
         message: :class:`str`
@@ -828,15 +828,15 @@
         """
         return CommentBundle(await self.http.make_request(Path.get_comment(comment)))
 
     async def reply_topic(self, topic: int, body: str) -> ForumPost:
         """
         Create a post replying to the specified topic.
 
-        Requires OAuth, scope forum.write, and a user (authorization code grant, delegate scope, or password auth)
+        Requires OAuth, scope forum.write, and a user (authorization code grant, delegate scope)
 
         **Parameters**
 
         topic: :class:`int`
             Id of the topic to be replied to.
 
         body: :class:`str`
@@ -862,15 +862,15 @@
         poll_options: Optional[str] = None,
         poll_title: Optional[str] = None,
         vote_change: Optional[bool] = None,
     ) -> CreateTopicResult:
         """
         Create a new topic.
 
-        Requires OAuth, scope forum.write, and a user (authorization code grant, delegate scope, or password auth)
+        Requires OAuth, scope forum.write, and a user (authorization code grant, delegate scope)
 
         **Parameters**
 
         body: :class:`str`
             Content of the topic.
 
         forum_id: :class:`int`
@@ -1060,15 +1060,15 @@
         room: int,
         playlist: int,
         limit: Optional[int] = None,
         sort: Optional[Union[str, MultiplayerScoresSort]] = None,
         cursor: Optional[str] = None,
     ) -> MultiplayerScores:
         """
-        Requires OAuth, scope public, and a user (authorization code grant, delegate scope, or password auth)
+        Requires OAuth, scope public, and a user (authorization code grant, delegate scope)
 
         **Parameters**
 
         room: :class:`int`
             Id of the room.
 
         playlist: :class:`int`
@@ -1222,15 +1222,15 @@
         """
         return Spotlights(await self.http.make_request(Path.get_spotlights()))
 
     async def get_own_data(self, mode: Union[str, GameModeStr] = "") -> User:
         """
         Similar to get_user but with authenticated user (token owner) as user id.
 
-        Requires OAuth, scope identify, and a user (authorization code grant, delegate scope, or password auth)
+        Requires OAuth, scope identify, and a user (authorization code grant, delegate scope)
 
         **Parameters**
 
         mode: Optional[:class:`str`, :class:`GameModeStr`]
             GameMode. User default mode will be used if not specified.
 
         **Returns**
@@ -1579,15 +1579,15 @@
         room_type: Optional[Union[RoomType, str]] = None,
         category: Optional[Union[RoomCategory, str]] = None,
         filter_mode: Optional[Union[RoomFilterMode, str]] = None,
     ) -> List[Room]:
         """
         Returns a list of rooms.
 
-        Requires OAuth, scope public, and a user (authorization code grant, delegate scope, or password auth).
+        Requires OAuth, scope public, and a user (authorization code grant, delegate scope).
 
         **Parameters**
 
         mode: Optional[Union[:class:`str`, :class:`GameModeStr`]]
             Game mode to filter rooms by.
 
         sort: Optional[Union[:class:`str`, :class:`RoomSort`]]
@@ -1681,15 +1681,17 @@
         **Returns**
 
         Union[:class:`SoloScore`, :class:`LegacyScore`]
             Should be a SoloScore, unless for some strange reason it's not
         """
         return get_score_object(await self.http.make_request(Path.get_score_by_id_only(score_id)))
 
-    async def search_beatmapsets(self, filters=None, page=None) -> BeatmapsetSearchResult:
+    async def search_beatmapsets(
+        self, filters: Optional[BeatmapsetSearchFilter] = None, page: Optional[int] = None
+    ) -> BeatmapsetSearchResult:
         """
         Search for beatmapsets.
 
         Requires OAuth and scope public.
 
         **Attributes**
 
@@ -1717,62 +1719,104 @@
 
     async def get_room_leaderboard(self, room_id: int) -> GetRoomLeaderboardResult:
         """
         Return a room's leaderboard. The :class:`UserScoreAggregate` objects returned under the "leaderboard"
         key contain the "user" attribute. The :class:`UserScoreAggregate` object under the "user_score" key
         contains the "user" and "position" attributes.
 
-        Requires OAuth, scope public, and a user (authorization code grant, delegate scope, or password auth).
+        Requires OAuth, scope public, and a user (authorization code grant, delegate scope).
 
         **Parameters**
 
         room_id: :class:`int`
 
         **Returns**
 
         :class:`GetRoomLeaderboard`
         """
         resp = await self.http.make_request(Path.get_room_leaderboard(room_id))
         return GetRoomLeaderboardResult(
             list(map(UserScoreAggregate, resp["leaderboard"])), get_optional(resp, "user_score", UserScoreAggregate)
         )
 
-    async def get_replay_data(self, mode, score_id) -> "osrparse.Replay":
+    async def get_replay_data(
+        self, mode: Optional[Union[GameModeStr, str]], score_id: int, use_osrparse: bool = True
+    ) -> Union["osrparse.Replay", bytes]:
         """
         Returns replay data for a score.
 
-        Requires OAuth, scope public, and a user (authorization code grant, delegate scope, or password auth).
+        Requires OAuth, scope public, and a user (authorization code grant, delegate scope).
 
         Requires osu.py is installed with the 'replay' feature
 
         **Parameters**
 
-        mode: Union[:class:`str`, :class:`GameModeStr`]
+        mode: Optional[Union[:class:`str`, :class:`GameModeStr`]]
 
         score_id: :class:`int`
 
+        use_osrparse: :class:`bool`
+            If true, returns an :class:`osrparse.Replay` object. Defaults to true.
+
         **Returns**
 
-        :class:`osrparse.Replay`
+        Union[:class:`osrparse.Replay`, :class:`bytes`]
         """
-        if not has_osrparse:
+        if mode is None:
+            return await self.get_replay_data_by_id_only(score_id, use_osrparse=use_osrparse)
+
+        if not has_osrparse and use_osrparse:
             raise RuntimeError(
                 "osrparse is required to call get_replay_data. "
                 "Install osu.py with the 'replay' feature to use this function."
             )
 
         mode = parse_enum_args(mode)
         gen = self.http.get_req_gen(Path.get_replay_data(mode, score_id))
-        async for resp in gen:
-            return osrparse.Replay.from_string(await resp.read())
+        async for resp in gen:  # at most one resp, but shouldn't be zero here
+            data = await resp.read()
+            return osrparse.Replay.from_string(data) if use_osrparse else data
+
+    async def get_replay_data_by_id_only(
+        self, score_id: int, use_osrparse: bool = True
+    ) -> Union["osrparse.Replay", bytes]:
+        """
+        Returns replay data for a score. Use :func:`AsynchronousClient.get_replay_data` for score ids that require
+        specifying the game mode too.
+
+        Requires OAuth, scope public, and a user (authorization code grant, delegate scope).
+
+        Requires osu.py is installed with the 'replay' feature if use_osrparse is true.
+
+        **Parameters**
+
+        score_id: :class:`int`
+
+        use_osrparse: :class:`bool`
+            If true, returns an :class:`osrparse.Replay` object. Defaults to true.
+
+        **Returns**
+
+        Union[:class:`osrparse.Replay`, :class:`bytes`]
+        """
+        if not has_osrparse and use_osrparse:
+            raise RuntimeError(
+                "osrparse is required to call get_replay_data. "
+                "Install osu.py with the 'replay' feature to use this function."
+            )
+
+        gen = self.http.get_req_gen(Path.get_replay_data_by_id_only(score_id))
+        async for resp in gen:  # at most one resp, but shouldn't be zero here
+            data = await resp.read()
+            return osrparse.Replay.from_string(data) if use_osrparse else data
 
     async def get_friends(self) -> List[UserCompact]:
         """
         Returns a list of friends.
 
-        Requires OAuth, scope friends.read, and a user (authorization code grant, delegate scope, or password auth).
+        Requires OAuth, scope friends.read, and a user (authorization code grant, delegate scope).
 
         **Returns**
 
         List[:class:`UserCompact`]
         """
         return list(map(UserCompact, await self.http.make_request(Path.get_friends())))
```

### Comparing `osu_py-2.0.2/osu/asyncio/http.py` & `osu_py-2.1.0/osu/asyncio/http.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/auth.py` & `osu_py-2.1.0/osu/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,31 +220,42 @@
         refresh_token: Optional[:class:`str`]
             A refresh token used to get a new access token.
         """
         raise NotImplementedError()
 
 
 class AuthHandler(FunctionalAuthHandler):
+    @staticmethod
+    def _raise_for_status(resp):
+        try:
+            resp.raise_for_status()
+        except Exception as exc:
+            try:
+                msg = resp.json()["error"]
+            except:
+                msg = None
+            raise type(exc)(str(exc) + ": " + msg) if msg is not None else exc from None
+
     def get_auth_token(self, code: Optional[str] = None) -> None:
         data = self._get_data("client_credentials" if code is None else "authorization_code", code)
 
         response = requests.post(token_url, data=data)
-        response.raise_for_status()
+        self._raise_for_status(response)
         response = response.json()
 
         self._handle_response(response)
 
     def refresh_access_token(self, refresh_token: Optional[str] = None) -> None:
         if refresh_token:
             self.refresh_token = refresh_token
 
         data = self._get_data("client_credentials" if self.refresh_token is None else "refresh_token")
 
         response = requests.post(token_url, data=data)
-        response.raise_for_status()
+        self._raise_for_status(response)
         response = response.json()
 
         self._handle_response(response)
 
         if self._refresh_callback:
             self._refresh_callback(self)
 
@@ -276,21 +287,29 @@
         auth._token = self._token
         self.expire_time = self.expire_time
         self._refresh_callback = self._refresh_callback
         return auth
 
 
 class AsynchronousAuthHandler(FunctionalAuthHandler):
+    @staticmethod
+    async def _raise_for_status(resp):
+        try:
+            resp.raise_for_status()
+        except Exception as exc:
+            try:
+                msg = (await resp.json())["error"]
+            except:
+                msg = None
+            raise type(exc)(str(exc) + ": " + msg) if msg is not None else exc from None
+
     async def _request(self, data, is_refresh=False):
         async with aiohttp.ClientSession() as session:
             async with session.request("POST", token_url, json=data) as resp:
-                try:
-                    resp.raise_for_status()
-                except Exception as e:
-                    raise e
+                await self._raise_for_status(resp)
                 json = await resp.json()
                 self._handle_response(json)
 
                 if is_refresh and self._refresh_callback:
                     self._refresh_callback(self)
 
     async def get_auth_token(self, code: Optional[str] = None):
```

### Comparing `osu_py-2.0.2/osu/client.py` & `osu_py-2.1.0/osu/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -714,15 +714,15 @@
 
     def create_new_pm(
         self, target_id: int, message: str, is_action: bool, uuid: Optional[str] = None
     ) -> CreateNewPmResult:
         """
         This endpoint allows you to create a new PM channel.
 
-        Requires OAuth, scope chat.write, and a user (authorization code grant, delegate scope, or password auth)
+        Requires OAuth, scope chat.write, and a user (authorization code grant, delegate scope)
 
         **Parameters**
 
         target_id: :class:`int`
             user_id of user to start PM with
 
         message: :class:`str`
@@ -821,15 +821,15 @@
         """
         return CommentBundle(self.http.make_request(Path.get_comment(comment)))
 
     def reply_topic(self, topic: int, body: str) -> ForumPost:
         """
         Create a post replying to the specified topic.
 
-        Requires OAuth, scope forum.write, and a user (authorization code grant, delegate scope, or password auth)
+        Requires OAuth, scope forum.write, and a user (authorization code grant, delegate scope)
 
         **Parameters**
 
         topic: :class:`int`
             Id of the topic to be replied to.
 
         body: :class:`str`
@@ -855,15 +855,15 @@
         poll_options: Optional[str] = None,
         poll_title: Optional[str] = None,
         vote_change: Optional[bool] = None,
     ) -> CreateTopicResult:
         """
         Create a new topic.
 
-        Requires OAuth, scope forum.write, and a user (authorization code grant, delegate scope, or password auth)
+        Requires OAuth, scope forum.write, and a user (authorization code grant, delegate scope)
 
         **Parameters**
 
         body: :class:`str`
             Content of the topic.
 
         forum_id: :class:`int`
@@ -1053,15 +1053,15 @@
         room: int,
         playlist: int,
         limit: Optional[int] = None,
         sort: Optional[Union[str, MultiplayerScoresSort]] = None,
         cursor: Optional[str] = None,
     ) -> MultiplayerScores:
         """
-        Requires OAuth, scope public, and a user (authorization code grant, delegate scope, or password auth)
+        Requires OAuth, scope public, and a user (authorization code grant, delegate scope)
 
         **Parameters**
 
         room: :class:`int`
             Id of the room.
 
         playlist: :class:`int`
@@ -1215,15 +1215,15 @@
         """
         return Spotlights(self.http.make_request(Path.get_spotlights()))
 
     def get_own_data(self, mode: Union[str, GameModeStr] = "") -> User:
         """
         Similar to get_user but with authenticated user (token owner) as user id.
 
-        Requires OAuth, scope identify, and a user (authorization code grant, delegate scope, or password auth)
+        Requires OAuth, scope identify, and a user (authorization code grant, delegate scope)
 
         **Parameters**
 
         mode: Optional[:class:`str`, :class:`GameModeStr`]
             GameMode. User default mode will be used if not specified.
 
         **Returns**
@@ -1570,15 +1570,15 @@
         room_type: Optional[Union[RoomType, str]] = None,
         category: Optional[Union[RoomCategory, str]] = None,
         filter_mode: Optional[Union[RoomFilterMode, str]] = None,
     ) -> List[Room]:
         """
         Returns a list of rooms.
 
-        Requires OAuth, scope public, and a user (authorization code grant, delegate scope, or password auth).
+        Requires OAuth, scope public, and a user (authorization code grant, delegate scope).
 
         **Parameters**
 
         mode: Optional[Union[:class:`str`, :class:`GameModeStr`]]
             Game mode to filter rooms by.
 
         sort: Optional[Union[:class:`str`, :class:`RoomSort`]]
@@ -1672,15 +1672,17 @@
         **Returns**
 
         Union[:class:`SoloScore`, :class:`LegacyScore`]
             Should be a SoloScore, unless for some strange reason it's not
         """
         return get_score_object(self.http.make_request(Path.get_score_by_id_only(score_id)))
 
-    def search_beatmapsets(self, filters=None, page=None) -> BeatmapsetSearchResult:
+    def search_beatmapsets(
+        self, filters: Optional[BeatmapsetSearchFilter] = None, page: Optional[int] = None
+    ) -> BeatmapsetSearchResult:
         """
         Search for beatmapsets.
 
         Requires OAuth and scope public.
 
         **Attributes**
 
@@ -1708,62 +1710,99 @@
 
     def get_room_leaderboard(self, room_id: int) -> GetRoomLeaderboardResult:
         """
         Return a room's leaderboard. The :class:`UserScoreAggregate` objects returned under the "leaderboard"
         key contain the "user" attribute. The :class:`UserScoreAggregate` object under the "user_score" key
         contains the "user" and "position" attributes.
 
-        Requires OAuth, scope public, and a user (authorization code grant, delegate scope, or password auth).
+        Requires OAuth, scope public, and a user (authorization code grant, delegate scope).
 
         **Parameters**
 
         room_id: :class:`int`
 
         **Returns**
 
         :class:`GetRoomLeaderboard`
         """
         resp = self.http.make_request(Path.get_room_leaderboard(room_id))
         return GetRoomLeaderboardResult(
             list(map(UserScoreAggregate, resp["leaderboard"])), get_optional(resp, "user_score", UserScoreAggregate)
         )
 
-    def get_replay_data(self, mode, score_id) -> "osrparse.Replay":
+    def get_replay_data(
+        self, mode: Optional[Union[GameModeStr, str]], score_id: int, use_osrparse: bool = True
+    ) -> Union["osrparse.Replay", bytes]:
         """
-        Returns replay data for a score.
+        Returns replay data for a score. Use :func:`Client.get_replay_data_by_id_only` for only the id, or specify
+        None to the mode attribute.
 
-        Requires OAuth, scope public, and a user (authorization code grant, delegate scope, or password auth).
+        Requires OAuth, scope public, and a user (authorization code grant, delegate scope).
 
-        Requires osu.py is installed with the 'replay' feature
+        Requires osu.py is installed with the 'replay' feature if use_osrparse is true.
 
         **Parameters**
 
-        mode: Union[:class:`str`, :class:`GameModeStr`]
+        mode: Optional[Union[:class:`str`, :class:`GameModeStr`]]
 
         score_id: :class:`int`
 
+        use_osrparse: :class:`bool`
+            If true, returns an :class:`osrparse.Replay` object. Defaults to true.
+
         **Returns**
 
-        :class:`osrparse.Replay`
+        Union[:class:`osrparse.Replay`, :class:`bytes`]
         """
-        if not has_osrparse:
+        if mode is None:
+            return self.get_replay_data_by_id_only(score_id, use_osrparse=use_osrparse)
+
+        if not has_osrparse and use_osrparse:
             raise RuntimeError(
                 "osrparse is required to call get_replay_data. "
                 "Install osu.py with the 'replay' feature to use this function."
             )
 
         mode = parse_enum_args(mode)
-        return osrparse.Replay.from_string(
-            self.http.make_request(Path.get_replay_data(mode, score_id), is_download=True).content
-        )
+        data = self.http.make_request(Path.get_replay_data(mode, score_id), is_download=True).content
+        return osrparse.Replay.from_string(data) if use_osrparse else data
+
+    def get_replay_data_by_id_only(self, score_id: int, use_osrparse: bool = True) -> Union["osrparse.Replay", bytes]:
+        """
+        Returns replay data for a score. Use :func:`Client.get_replay_data` for score ids that require
+        specifying the game mode too.
+
+        Requires OAuth, scope public, and a user (authorization code grant, delegate scope).
+
+        Requires osu.py is installed with the 'replay' feature if use_osrparse is true.
+
+        **Parameters**
+
+        score_id: :class:`int`
+
+        use_osrparse: :class:`bool`
+            If true, returns an :class:`osrparse.Replay` object. Defaults to true.
+
+        **Returns**
+
+        Union[:class:`osrparse.Replay`, :class:`bytes`]
+        """
+        if not has_osrparse and use_osrparse:
+            raise RuntimeError(
+                "osrparse is required to call get_replay_data. "
+                "Install osu.py with the 'replay' feature to use this function."
+            )
+
+        data = self.http.make_request(Path.get_replay_data_by_id_only(score_id), is_download=True).content
+        return osrparse.Replay.from_string(data) if use_osrparse else data
 
     def get_friends(self) -> List[UserCompact]:
         """
         Returns a list of friends.
 
-        Requires OAuth, scope friends.read, and a user (authorization code grant, delegate scope, or password auth).
+        Requires OAuth, scope friends.read, and a user (authorization code grant, delegate scope).
 
         **Returns**
 
         List[:class:`UserCompact`]
         """
         return list(map(UserCompact, self.http.make_request(Path.get_friends())))
```

### Comparing `osu_py-2.0.2/osu/constants.py` & `osu_py-2.1.0/osu/constants.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/enums.py` & `osu_py-2.1.0/osu/enums.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/http.py` & `osu_py-2.1.0/osu/http.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/notification.py` & `osu_py-2.1.0/osu/notification.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/objects/__init__.py` & `osu_py-2.1.0/osu/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/objects/achievement.py` & `osu_py-2.1.0/osu/objects/achievement.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/objects/beatmap.py` & `osu_py-2.1.0/osu/objects/beatmap.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/objects/beatmapset_event.py` & `osu_py-2.1.0/osu/objects/beatmapset_event.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/objects/build.py` & `osu_py-2.1.0/osu/objects/build.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/objects/chat.py` & `osu_py-2.1.0/osu/objects/chat.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/objects/comment.py` & `osu_py-2.1.0/osu/objects/comment.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/objects/current_user_attributes.py` & `osu_py-2.1.0/osu/objects/current_user_attributes.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/objects/discussion.py` & `osu_py-2.1.0/osu/objects/discussion.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/objects/event.py` & `osu_py-2.1.0/osu/objects/event.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/objects/forum.py` & `osu_py-2.1.0/osu/objects/forum.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/objects/group.py` & `osu_py-2.1.0/osu/objects/group.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/objects/kudosu.py` & `osu_py-2.1.0/osu/objects/kudosu.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/objects/match.py` & `osu_py-2.1.0/osu/objects/match.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/objects/multiplayer.py` & `osu_py-2.1.0/osu/objects/multiplayer.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/objects/news.py` & `osu_py-2.1.0/osu/objects/news.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/objects/notification.py` & `osu_py-2.1.0/osu/objects/notification.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/objects/ranking.py` & `osu_py-2.1.0/osu/objects/ranking.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/objects/scope.py` & `osu_py-2.1.0/osu/objects/scope.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/objects/score.py` & `osu_py-2.1.0/osu/objects/score.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/objects/seasonal_background.py` & `osu_py-2.1.0/osu/objects/seasonal_background.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/objects/user.py` & `osu_py-2.1.0/osu/objects/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -636,15 +636,15 @@
     country_rank: Optional[:class:`int`]
         Current country rank according to pp.
 
      global_rank: Optional[:class:`int`]
         Current global rank according to pp.
 
     global_rank_exp: Optional[:class:`int`]
-        Current global rank according to experimental pp.
+        Current global rank according to experimental pp (not used anymore).
 
     grade_counts: :class:`NamedTuple`
         Below are the attributes and their meanings.
 
         a: :class:`int`
             Number of A ranked scores.
 
@@ -677,16 +677,18 @@
 
     play_time: :class:`int`
         Cumulative time played.
 
     pp: :class:`int`
         Performance points
 
-    pp_exp: :class:`int`
-        Experimental performance points (on lazer.ppy.sh)
+    pp_exp: Optional[:class:`int`]
+        Experimental performance points (not used anymore)
+
+    rank_change_since_30_days: Optional[:class:`int`]
 
     recommended_difficulty: :class:`float`
         Recommended difficulty for a player. This value is not received from the api, but locally calculated.
         The formula is pp^0.4 * 0.195
 
     recommended_difficulty_exp: :class:`float`
         Recommended difficulty based on the pp_exp value.
@@ -730,14 +732,15 @@
         "count_100",
         "count_300",
         "count_50",
         "count_miss",
         "recommended_difficulty",
         "recommended_difficulty_exp",
         "variants",
+        "rank_change_since_30_days",
     )
 
     def __init__(self, data):
         self.count_100: int = data["count_100"]
         self.count_300: int = data["count_300"]
         self.count_50: int = data["count_50"]
         self.count_miss: int = data["count_miss"]
@@ -748,23 +751,24 @@
         self.level: NamedTuple = namedtuple("Level", ("current", "progress"))(**data["level"])
         self.hit_accuracy: float = data["hit_accuracy"]
         self.is_ranked: bool = data["is_ranked"]
         self.maximum_combo: int = data["maximum_combo"]
         self.play_count: int = data["play_count"]
         self.play_time: int = data["play_time"]
         self.pp: int = data["pp"]
-        self.pp_exp: int = data.get("pp_exp")
+        self.pp_exp: Optional[int] = data.get("pp_exp")
         self.recommended_difficulty: float = math.pow(self.pp, 0.4) * 0.195
         self.recommended_difficulty_exp: float = math.pow(self.pp_exp, 0.4) * 0.195 if self.pp_exp is not None else None
         self.ranked_score: int = data["ranked_score"]
         self.replays_watched_by_others: int = data["replays_watched_by_others"]
         self.total_hits: int = data["total_hits"]
         self.total_score: int = data["total_score"]
         self.user: Optional[UserCompact] = get_optional(data, "user", UserCompact)
         self.variants: Optional[List[UserStatisticVariant]] = get_optional_list(data, "variants", UserStatisticVariant)
+        self.rank_change_since_30_days: Optional[int] = data.get("rank_change_since_30_days")
 
     def __repr__(self):
         return prettify(self, "pp", "global_rank", "user")
 
 
 class UserStatisticVariant:
     """
```

### Comparing `osu_py-2.0.2/osu/objects/wiki.py` & `osu_py-2.1.0/osu/objects/wiki.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/path.py` & `osu_py-2.1.0/osu/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,13 +213,17 @@
         return cls("get", "seasonal-backgrounds", None)
 
     @classmethod
     def get_replay_data(cls, mode, score):
         return cls("get", f"scores/{mode}/{score}/download", "public", True)
 
     @classmethod
+    def get_replay_data_by_id_only(cls, score):
+        return cls("get", f"scores/{score}/download", "public", True)
+
+    @classmethod
     def get_friends(cls):
         return cls("get", "friends", "friends.read", True)
 
     @classmethod
     def beatmapset_search(cls):
         return cls("get", "beatmapsets/search", "public")
```

### Comparing `osu_py-2.0.2/osu/results.py` & `osu_py-2.1.0/osu/results.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu/util.py` & `osu_py-2.1.0/osu/util.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/osu.py.egg-info/PKG-INFO` & `osu_py-2.1.0/osu.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osu.py
-Version: 2.0.2
+Version: 2.1.0
 Summary: API Wrapper for osu!api v2 written in Python.
 Home-page: https://github.com/Sheepposu/osu.py
 Author: Sheepposu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Sheepposu/osu.py/issues
 Project-URL: osu.py documentation, https://osupy.readthedocs.io/
 Project-URL: osu!api v2 documentation, https://osu.ppy.sh/docs/index.html
```

### Comparing `osu_py-2.0.2/osu.py.egg-info/SOURCES.txt` & `osu_py-2.1.0/osu.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.2/setup.py` & `osu_py-2.1.0/setup.py`

 * *Files identical despite different names*

