# Comparing `tmp/matterdelta-1.5.0.tar.gz` & `tmp/matterdelta-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matterdelta-1.5.0.tar", last modified: Fri May 24 19:41:37 2024, max compression
+gzip compressed data, was "matterdelta-1.6.1.tar", last modified: Fri May 31 17:39:02 2024, max compression
```

## Comparing `matterdelta-1.5.0.tar` & `matterdelta-1.6.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:41:37.359733 matterdelta-1.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:41:37.355733 matterdelta-1.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:41:37.355733 matterdelta-1.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-24 19:41:27.000000 matterdelta-1.5.0/.github/workflows/python-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-24 19:41:27.000000 matterdelta-1.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-24 19:41:27.000000 matterdelta-1.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-24 19:41:37.359733 matterdelta-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-24 19:41:27.000000 matterdelta-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:41:37.355733 matterdelta-1.5.0/matterdelta/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-24 19:41:27.000000 matterdelta-1.5.0/matterdelta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-24 19:41:27.000000 matterdelta-1.5.0/matterdelta/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-24 19:41:37.000000 matterdelta-1.5.0/matterdelta/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-05-24 19:41:27.000000 matterdelta-1.5.0/matterdelta/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-24 19:41:27.000000 matterdelta-1.5.0/matterdelta/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:41:37.359733 matterdelta-1.5.0/matterdelta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-24 19:41:37.000000 matterdelta-1.5.0/matterdelta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-24 19:41:37.000000 matterdelta-1.5.0/matterdelta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 19:41:37.000000 matterdelta-1.5.0/matterdelta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-24 19:41:37.000000 matterdelta-1.5.0/matterdelta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-24 19:41:37.000000 matterdelta-1.5.0/matterdelta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 19:41:37.000000 matterdelta-1.5.0/matterdelta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-24 19:41:27.000000 matterdelta-1.5.0/pylama.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-24 19:41:27.000000 matterdelta-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 19:41:37.359733 matterdelta-1.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:39:02.915506 matterdelta-1.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:39:02.911507 matterdelta-1.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:39:02.911507 matterdelta-1.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-31 17:38:51.000000 matterdelta-1.6.1/.github/workflows/python-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-31 17:38:51.000000 matterdelta-1.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-31 17:38:51.000000 matterdelta-1.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-31 17:39:02.915506 matterdelta-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-31 17:38:51.000000 matterdelta-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:39:02.911507 matterdelta-1.6.1/matterdelta/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-31 17:38:51.000000 matterdelta-1.6.1/matterdelta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-31 17:38:51.000000 matterdelta-1.6.1/matterdelta/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 17:39:02.000000 matterdelta-1.6.1/matterdelta/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-05-31 17:38:51.000000 matterdelta-1.6.1/matterdelta/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-31 17:38:51.000000 matterdelta-1.6.1/matterdelta/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:39:02.915506 matterdelta-1.6.1/matterdelta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-31 17:39:02.000000 matterdelta-1.6.1/matterdelta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-31 17:39:02.000000 matterdelta-1.6.1/matterdelta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 17:39:02.000000 matterdelta-1.6.1/matterdelta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 17:39:02.000000 matterdelta-1.6.1/matterdelta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-31 17:39:02.000000 matterdelta-1.6.1/matterdelta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-31 17:39:02.000000 matterdelta-1.6.1/matterdelta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-31 17:38:51.000000 matterdelta-1.6.1/pylama.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-31 17:38:51.000000 matterdelta-1.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 17:39:02.915506 matterdelta-1.6.1/setup.cfg
```

### Comparing `matterdelta-1.5.0/.github/workflows/python-ci.yml` & `matterdelta-1.6.1/.github/workflows/python-ci.yml`

 * *Files identical despite different names*

### Comparing `matterdelta-1.5.0/LICENSE.txt` & `matterdelta-1.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `matterdelta-1.5.0/PKG-INFO` & `matterdelta-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matterdelta
-Version: 1.5.0
+Version: 1.6.1
 Summary: Matterbridge API plugin for Delta Chat
 Author-email: adbenitez <adb@merlinux.eu>
 Project-URL: Homepage, https://github.com/deltachat-bot/matterdelta
 Keywords: deltachat,bot,matterbridge,bridge
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `matterdelta-1.5.0/README.md` & `matterdelta-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `matterdelta-1.5.0/matterdelta/api.py` & `matterdelta-1.6.1/matterdelta/api.py`

 * *Files identical despite different names*

### Comparing `matterdelta-1.5.0/matterdelta/hooks.py` & `matterdelta-1.6.1/matterdelta/hooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     CoreEvent,
     EventType,
     JsonRpcError,
     MsgData,
     NewMsgEvent,
     events,
 )
-from deltachat2.types import SpecialContactId
 from rich.logging import RichHandler
 
 from ._version import __version__
 from .api import dc2mb, init_api
 
 cli = BotCli("matterdelta")
 cli.add_generic_option("-v", "--version", action="version", version=__version__)
@@ -55,30 +54,27 @@
     elif event.kind == EventType.ERROR:
         bot.logger.error(event.msg)
     elif event.kind == EventType.SECUREJOIN_INVITER_PROGRESS:
         if event.progress == 1000:
             if not bot.rpc.get_contact(accid, event.contact_id).is_bot:
                 bot.logger.debug("QR scanned by contact id=%s", event.contact_id)
                 chatid = bot.rpc.create_chat_by_contact_id(accid, event.contact_id)
-                _send_help(bot, accid, chatid)
+                if not is_community(bot, accid):
+                    _send_help(bot, accid, chatid)
 
 
 @cli.on(events.NewMessage(is_info=False, is_bot=None))
 def _bridge(bot: Bot, accid: int, event: NewMsgEvent) -> None:
     if bot.has_command(event.command):
         return
     msg = event.msg
     chat = bot.rpc.get_basic_chat_info(accid, msg.chat_id)
     if chat.chat_type == ChatType.SINGLE and not msg.is_bot:
         bot.rpc.markseen_msgs(accid, [msg.id])
-        try:
-            community = bot.rpc.get_config(accid, "is_community") == "1"
-        except JsonRpcError:
-            community = False
-        if not community or msg.from_id > SpecialContactId.LAST_SPECIAL:
+        if not is_community(bot, accid):
             _send_help(bot, accid, msg.chat_id)
     else:
         dc2mb(bot, accid, msg)
 
 
 @cli.on(events.NewMessage(command="/id"))
 def _id(bot: Bot, accid: int, event: NewMsgEvent) -> None:
@@ -97,7 +93,15 @@
     text = (
         "I'm a bot, I allow to bridge Delta Chat groups with groups in other platforms."
         " Only the bot administrator can bridge groups.\n\n"
         "**Available commands**\n\n"
         "/id - send me this command in a group to get its ID."
     )
     bot.rpc.send_msg(accid, chatid, MsgData(text=text))
+
+
+def is_community(bot: Bot, accid: int) -> bool:
+    """Return True if this is a community account."""
+    try:
+        return bot.rpc.get_config(accid, "is_community") == "1"
+    except JsonRpcError:
+        return False
```

### Comparing `matterdelta-1.5.0/matterdelta.egg-info/PKG-INFO` & `matterdelta-1.6.1/matterdelta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matterdelta
-Version: 1.5.0
+Version: 1.6.1
 Summary: Matterbridge API plugin for Delta Chat
 Author-email: adbenitez <adb@merlinux.eu>
 Project-URL: Homepage, https://github.com/deltachat-bot/matterdelta
 Keywords: deltachat,bot,matterbridge,bridge
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `matterdelta-1.5.0/pyproject.toml` & `matterdelta-1.6.1/pyproject.toml`

 * *Files identical despite different names*

