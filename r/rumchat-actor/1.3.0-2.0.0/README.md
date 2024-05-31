# Comparing `tmp/rumchat_actor-1.3.0.tar.gz` & `tmp/rumchat_actor-2.0.0.tar.gz`

## Comparing `rumchat_actor-1.3.0.tar` & `rumchat_actor-2.0.0.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 rumchat_actor-1.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    22577 2020-02-02 00:00:00.000000 rumchat_actor-1.3.0/src/rumchat_actor/__init__.py
--rw-r--r--   0        0        0    26512 2020-02-02 00:00:00.000000 rumchat_actor-1.3.0/src/rumchat_actor/common_commands.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 rumchat_actor-1.3.0/LICENSE.txt
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 rumchat_actor-1.3.0/README.md
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 rumchat_actor-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 rumchat_actor-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 rumchat_actor-2.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    23031 2020-02-02 00:00:00.000000 rumchat_actor-2.0.0/src/rumchat_actor/__init__.py
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 rumchat_actor-2.0.0/src/rumchat_actor/actions.py
+-rw-r--r--   0        0        0    32541 2020-02-02 00:00:00.000000 rumchat_actor-2.0.0/src/rumchat_actor/commands.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 rumchat_actor-2.0.0/src/rumchat_actor/localvars.py
+-rw-r--r--   0        0        0     6592 2020-02-02 00:00:00.000000 rumchat_actor-2.0.0/src/rumchat_actor/misc.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 rumchat_actor-2.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 rumchat_actor-2.0.0/README.md
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 rumchat_actor-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 rumchat_actor-2.0.0/PKG-INFO
```

### Comparing `rumchat_actor-1.3.0/.github/workflows/python-publish.yml` & `rumchat_actor-2.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `rumchat_actor-1.3.0/src/rumchat_actor/__init__.py` & `rumchat_actor-2.0.0/src/rumchat_actor/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,41 @@
 #!/usr/bin/env python3
 """Rumble Chat Actor
 
 Automatically interact with your Rumble livestream chats.
+
+Example usage:
+
+import rumchat_actor
+
+def eat_some_cheese(message, actor):
+    '''If a message mentions cheese, eat some cheese'''
+    if "cheese" in message.text.lower():
+        actor.send_message(f"@{message.user.username} Eat some cheese 🧀.")
+
+    return True #Actions should return None or False if they had to delete a message
+
+#stream_id is either the base 10 or base 36 livestream ID you want the Actor to connect to, obtained from the popout chat or the Rumble Live Stream API.
+#If stream_id is None but you pass api_url, the latest livestream shown on the API is chosen automatically.
+#If you pass profile_dir to an existing Firefox profile directory, your sign-ins to Rumble chat for the actor will be saved.
+#Otherwise, you will have to log in manuaglly each time you use the bot, or pass credentials = (username, password).
+actor = rumchat_actor.RumbleChatActor(stream_id = STREAM_ID)
+
+#Register an action to be called on every message
+actor.register_message_action(eat_some_cheese)
+
+#Register a command via the ChatCommand class
+actor.register_command(rumchat_actor.commands.ChatCommand(name = "hi", actor = actor, target = lambda message, actor: actor.send_message(f"Hello, @{message.user.username}!")))
+
+#Register a command via a callable
+actor.register_command(name = "tester", command = lambda message, actor: print(f"Test command run by {message.user.username}"))
+
+#Run the bot continuously
+actor.mainloop()
+
 S.D.G."""
 
 import textwrap
 import time
 import threading
 from cocorum import RumbleAPI, utils
 from cocorum.ssechat import SSEChat
@@ -13,120 +43,16 @@
 from selenium import webdriver
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.alert import Alert
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
-
-#How long to wait maximum for a condition to be true in the browser
-BROWSER_WAIT_TIMEOUT = 30
-
-#How long to wait between sending messages
-SEND_MESSAGE_COOLDOWN = 3
-
-#Popout chat url. Format with stream_id_b10
-CHAT_URL = "https://rumble.com/chat/popup/{stream_id_b10}"
-
-#Rumble user URL. Format with username
-USER_URL = "https://rumble.com/user/{username}"
-
-#Rumble channel URL. Format with channel_name
-CHANNEL_URL = "https://rumble.com/c/{channel_name}"
-
-#Maximum chat message length
-MAX_MESSAGE_LEN = 200
-
-#Message split across multiple lines must not be longer than this
-MAX_MULTIMESSAGE_LEN = 1000
-
-#Prefix to all actor messages
-BOT_MESSAGE_PREFIX = "🤖: "
-
-#How commands always start
-COMMAND_PREFIX = "!"
-
-#Levels of mute to discipline a user with
-MUTE_LEVELS = {
-    "5" : "cmi js-btn-mute-current-5",
-    "stream" : "cmi js-btn-mute-current",
-    "forever" : "cmi js-btn-mute-for-account",
-    }
-
-class ChatCommand():
-    """A chat command, internal use only"""
-    def __init__(self, name, actor, cooldown = SEND_MESSAGE_COOLDOWN, amount_cents = 0, exclusive = False, allowed_badges = ["subscriber"], whitelist_badges = ["moderator"], target = None):
-        """name: The !name of the command
-    actor: The RumleChatActor host object
-    amount_cents: The minimum cost of the command. Defaults to free
-    exclusive: If this command can only be run by users with allowed badges. Defaults to False
-    allowed_badges: Badges that are allowed to run this command (if it is exclusive).
-        Defaults to subscribers, admin is added internally.
-    whitelist_badges: Badges which if borne give the user free-of-charge command access
-    target: The command function(message, actor) to call. Defaults to self.run"""
-        assert " " not in name, "Name cannot contain spaces"
-        self.name = name
-        self.actor = actor
-        assert cooldown >= SEND_MESSAGE_COOLDOWN, \
-            f"Cannot set a cooldown shorter than {SEND_MESSAGE_COOLDOWN}"
-
-        self.cooldown = cooldown
-        self.amount_cents = amount_cents #Cost of the command
-        self.exclusive = exclusive
-        self.allowed_badges = ["admin"] + allowed_badges #Admin can always run any command
-        self.whitelist_badges = ["admin"] + whitelist_badges #Admin always has free-of-charge usage
-        self.last_use_time = 0 #Last time the command was called
-        self.target = target
-
-    def call(self, message):
-        """The command was called"""
-        #this command is exclusive, and the user does not have the required badge
-        if self.exclusive and \
-            not (True in [badge.slug in self.allowed_badges for badge in message.user.badges]):
-
-            self.actor.send_message(f"@{message.user.username} That command is exclusive to: " +
-                                    ", ".join(self.allowed_badges)
-                                    )
-
-            return
-
-        #The command is still on cooldown
-        if (curtime := time.time()) - self.last_use_time < self.cooldown:
-            self.actor.send_message(
-                f"@{message.user.username} That command is still on cooldown. " +
-                f"Try again in {int(self.last_use_time + self.cooldown - curtime + 0.5)} seconds."
-                )
-
-            return
-
-        #the user did not pay enough for the command and they do not have a free pass
-        if message.rant_price_cents < self.amount_cents and \
-            not (True in [badge.slug in self.whitelist_badges for badge in message.user.badges]):
-
-            self.actor.send_message("@" + message.user.username +
-                                    f"That command costs ${self.amount_cents/100:.2f}."
-                                    )
-            return
-
-        #the command was called successfully
-        self.run(message)
-
-        #Mark the last use time for cooldown
-        self.last_use_time = time.time()
-
-    def run(self, message):
-        """Dummy run method"""
-        if self.target:
-            self.target(message, self.actor)
-            return
-
-        #Run method was never defined
-        self.actor.send_message("@" + message.user.username +
-                                "Hello, this command never had a target defined. :-)"
-                                )
+from . import actions, commands, misc
+from .localvars import *
 
 class RumbleChatActor():
     """Actor that interacts with Rumble chat"""
     def __init__(self, init_message = "Hello, Rumble!", ignore_users = ["TheRumbleBot"], **kwargs):
         """stream_id: The stream ID you want to connect to. Defaults to latest livestream
     init_message: What to say when the actor starts up.
     profile_dir: The Firefox profile directory to use. Defaults to temp (sign-in not saved)
@@ -134,14 +60,17 @@
     api_url: The Rumble Live Stream API URL with your key (or RumBot's passthrough).
         Defaults to no Live Stream API access
     streamer_username: The username of the person streaming.
         Defaults to Live Stream API username or manually requested if needed
     streamer_channel: The channel doing the livestream, if it is being streamed on a channel.
         Defaults to Live Stream API channel or manually requested if needed
     is_channel_stream: Bool, if the livestream is on a channel or not
+        Defaults to automatic determination if possible
+    streamer_main_page_url: The URL of the streamer's main page
+        Defaults to automatic determination if possible
     ignore_users: List of usernames, will ignore all their messages
     invalid_command_respond: Bool, sets if we should post an error message if a command was invalid.
         Defaults to False."""
 
         #The info of the person streaming
         self.__streamer_username = kwargs["streamer_username"] if "streamer_username" in kwargs else None
         assert isinstance(self.__streamer_username, str) or self.__streamer_username is None, \
@@ -151,14 +80,18 @@
         assert isinstance(self.__streamer_channel, str) or self.__streamer_channel is None, \
             f"Streamer channel name must be str or None, not {type(self.__streamer_channel)}"
 
         self.__is_channel_stream = kwargs["is_channel_stream"] if "is_channel_stream" in kwargs else None
         assert isinstance(self.__is_channel_stream, bool) or self.__is_channel_stream is None, \
             f"Argument is_channel_stream must be bool or None, not {type(self.__is_channel_stream)}"
 
+        self.__streamer_main_page_url = kwargs["streamer_main_page_url"] if "streamer_main_page_url" in kwargs else None
+        assert isinstance(self.__streamer_main_page_url, str) or self.__streamer_main_page_url is None, \
+            f"Argument streamer_main_page_url must be str or None, not {type(self.__is_channel_stream)}"
+
         #Get Live Stream API
         if "api_url" in kwargs:
             self.rum_api = RumbleAPI(kwargs["api_url"])
         else:
             self.rum_api = None
 
         #A stream ID was passed
@@ -241,14 +174,20 @@
 
         #History of the bot's messages so they do not get loop processed
         self.sent_messages = []
 
         #Messages waiting to be sent
         self.outbox = []
 
+        #Messages that we know are actually raid alerts
+        self.known_raid_alert_messages = []
+
+        #Action to be taken when raids occur
+        self.__raid_action = print
+
         #Time that the last message we sent was sent
         self.last_message_send_time = 0
 
         #Loop condition of the mainloop() and sender_loop() methods
         self.keep_running = True
 
         #thread to send messages at timed intervals
@@ -265,15 +204,15 @@
         assert "moderator" in m.user.badges or "admin" in m.user.badges, \
             "Actor cannot function without being a moderator"
 
         #Functions that are to be called on each message,
         #must return False if the message was deleted
         self.message_actions = []
 
-        #Instances of RumbleChatCommand, by name
+        #Instances of ChatCommand, by name
         self.chat_commands = {}
 
         #Wether or not to post an error message if an invalid command was called
         self.invalid_command_respond = kwargs["invalid_command_respond"] if "invalid_command_respond" in kwargs else False
         assert isinstance(self.invalid_command_respond, bool), \
             f"Argument invalid_command_respond must be bool, not {type(self.invalid_command_respond)}"
 
@@ -320,18 +259,38 @@
                 self.__is_channel_stream = "y" in input("Is this a channel stream? y/[N]:")
 
         return self.__is_channel_stream
 
     @property
     def streamer_main_page_url(self):
         """The URL of the main page of the streamer"""
-        if self.is_channel_stream:
-            return CHANNEL_URL.format(channel_name = self.streamer_channel.replace(" ", ""))
+        #We do not yet know the URL
+        if not self.__streamer_main_page_url:
+            if self.is_channel_stream:
+                #This stream is on the API
+                if self.api_stream:
+                    #We know our channel ID from the API
+                    if self.rum_api.channel_id:
+                        self.__streamer_main_page_url = CHANNEL_URL.format(channel_name = f"c-{self.rum_api.channel_id}")
+
+                    #Is a channel stream and on the API but API is not for channel, use the user page instead
+                    else:
+                        self.__streamer_main_page_url = USER_URL.format(username = self.streamer_username)
+
+                #Is not an API stream and we don't know the username
+                elif not self.__streamer_username:
+                    while not (specified := input("Enter streamer main page URL: ")).startswith(RUMBLE_BASE_URL):
+                        pass
+                    self.__streamer_main_page_url = specified
+
+            #Not a channel stream, go by username
+            else:
+                self.__streamer_main_page_url = USER_URL.format(username = self.streamer_username)
 
-        return USER_URL.format(username = self.streamer_username)
+        return self.__streamer_main_page_url
 
     def get_sign_in_button(self):
         """Look for the sign in button"""
         try:
             return self.browser.find_element(By.CLASS_NAME, "chat--sign-in")
         except selenium.common.exceptions.NoSuchElementException:
             print("Could not find sign-in button, already signed in.")
@@ -392,29 +351,42 @@
                 f"[@data-message-id='{message_id}']"
                 )
 
         #Not a valid message type
         else:
             raise TypeError("Message must be ID, li element, or have message_id attribute")
 
+        if message_id in self.known_raid_alert_messages:
+            print("Cannot open moderation menu: Is a raid message.")
+            return None
+
         #Hover over the message
         self.hover_element(message_li)
         #Find the moderation menu
-        menu_bttn = message_li.find_element(
-            By.XPATH,
-            ".//button[@class='js-moderate-btn chat-history--kebab-button']"
-            )
+        try:
+            menu_bttn = message_li.find_element(
+                By.XPATH,
+                ".//button[@class='js-moderate-btn chat-history--kebab-button']"
+                )
+        except selenium.common.exceptions.NoSuchElementException:
+            print("Cannot open moderation menu: Could not find moderation button.")
+            return None
+
         #Click the moderation menu button
         menu_bttn.click()
 
         return message_id
 
     def delete_message(self, message):
         """Delete a message in the chat"""
         m_id = self.open_moderation_menu(message)
+        if m_id is None:
+            print("Could not delete message.")
+            return
+
         del_bttn = self.browser.find_element(
             By.XPATH,
             f"//button[@class='cmi js-btn-delete-current'][@data-message-id='{m_id}']"
             )
 
         del_bttn.click()
 
@@ -425,15 +397,19 @@
             )
 
         #Confirm the confirmation dialog
         Alert(self.browser).accept()
 
     def mute_by_message(self, message, mute_level = "5"):
         """Mute a user by message"""
-        self.open_moderation_menu(message)
+        m_id = self.open_moderation_menu(message)
+        if m_id is None:
+            print("Could not mute by message.")
+            return
+
         timeout_bttn = self.browser.find_element(
             By.XPATH,
             f"//button[@class='{MUTE_LEVELS[mute_level]}']"
             )
 
         timeout_bttn.click()
 
@@ -445,15 +421,19 @@
             f"//li[@class='chat-history--row js-chat-history-item'][@data-username='{name}']"
             )
 
         self.mute_by_message(message = message_li, mute_level = mute_level)
 
     def pin_message(self, message):
         """Pin a message by ID or li element"""
-        self.open_moderation_menu(message)
+        m_id = self.open_moderation_menu(message)
+        if m_id is None:
+            print("Could not pin message.")
+            return
+
         pin_bttn = self.browser.find_element(By.XPATH, "//button[@class='cmi js-btn-pin-current']")
         pin_bttn.click()
 
     def unpin_message(self):
         """Unpin the currently pinned message"""
         try:
             unpin_bttn = self.browser.find_element(
@@ -487,45 +467,66 @@
         if name not in self.chat_commands:
             if self.invalid_command_respond:
                 self.send_message(f"@{message.user.username} That is not a registered command.")
             return
 
         self.chat_commands[name].call(message)
 
-    def register_command(self, command, name = None):
+    def register_command(self, command, name = None, help_message = None):
         """Register a command"""
         #Is a ChatCommand instance
-        if isinstance(command, ChatCommand):
+        if isinstance(command, commands.ChatCommand):
             assert not name or name == command.name, \
                 "ChatCommand instance has different name than one passed"
             self.chat_commands[command.name] = command
 
         #Is a callable
         elif callable(command):
             assert name, "Name cannot be None if command is a callable"
             assert " " not in name, "Name cannot contain spaces"
-            self.chat_commands[name] = ChatCommand(name = name, actor = self, target = command)
+            self.chat_commands[name] = commands.ChatCommand(name = name, actor = self, target = command)
 
         else:
             raise TypeError(f"Command must be of type ChatCommand or a callable, not {type(command)}.")
 
+        #A specific help message was provided
+        if help_message:
+            assert not self.chat_commands[name].help_message, "ChatCommand has internal help message already set, cannot override"
+            self.chat_commands[name].help_message = help_message
+
     def register_message_action(self, action):
         """Register an action callable to be run on every message
     - Action will be passed cocorum.ssechat.SSEChatMessage() and this actor
     - Action should return True if the message survived the action
     - Action should return False if the message was deleted by the action"""
         assert callable(action), "Action must be a callable"
         self.message_actions.append(action)
 
+    @property
+    def raid_action(self):
+        """The callable we are supposed to run on raids"""
+        return self.__raid_action
+
+    @raid_action.setter
+    def raid_action(self, new_action):
+        assert callable(new_action), "Raid action must be a callable"
+        self.__raid_action = new_action
+
     def __process_message(self, message):
         """Process a single SSE Chat message"""
         #Ignore messages that match ones we sent before
         if message.text in self.sent_messages:
             return
 
+        #the message is actually a raid alert, take raid action on it, nothing more
+        if message.raid_notification:
+            self.known_raid_alert_messages.append(message)
+            self.raid_action(message)
+            return
+
         #If the message is from the same account as us, consider it in message send cooldown
         if message.user.username == self.username:
             self.last_message_send_time = max((self.last_message_send_time, message.time))
 
         #Ignore messages that are in the ignore_users list
         if message.user.username in self.ignore_users:
             return
```

### Comparing `rumchat_actor-1.3.0/src/rumchat_actor/common_commands.py` & `rumchat_actor-2.0.0/src/rumchat_actor/commands.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,140 @@
 #!/usr/bin/env python3
-"""Rumble chat actor common commands
+"""Chat commands
 
-Derivative classes for common chat commands.
+The base ChatCommand abstract class, and some commonly used derivatives
 S.D.G."""
 
+import glob
 import os
 import shutil
 import sys
 import tempfile
 import time
 import threading
 from tkinter import filedialog, Tk
 from cocorum.localvars import RUMBLE_BASE_URL, DEFAULT_TIMEOUT
 from browsermobproxy import Server
 from moviepy.editor import VideoFileClip, concatenate_videoclips
+from moviepy.video.io.ffmpeg_tools import ffmpeg_extract_subclip
 import requests
 # import selenium
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 import talkey
-from . import ChatCommand
+from .localvars import *
 
-OP_PATH = __file__[:__file__.rfind(os.sep)] #The path of the script
-BROWSERMOB_EXE = 'browsermob-proxy' #The Browsermob Proxy executable
-WAIT_FOR_LIVE_REFRESH_RATE = 10 #How often to refresh while waiting for a livestream to start
-CLIP_FILENAME_EXTENSION = "mp4" #The filename extension for saved clips
-CLIP_BITRATE = "4.5M" #The bitrate to use when saving clips. Deprecating
-STREAM_QUALITIES = {"360p" : "1.2M", "720p" : "2.8M", "1080p" : "4.5M"} #Valid resolutions of a livestream and the bitrates they use / should be saved with
-DEFAULT_CLIP_BITRATE = STREAM_QUALITIES["1080p"] #The default save quality for clips from a local recording
-VALID_CLIP_RECORDING_CONTAINERS = ["ts"] #Formats that the OBS recording can be in if recording-trimmed clips are to work
-TEMP_RECORDING_COPY_FILENAME = ".temp_recording_copy"
-NUM_TS_DOWNLOAD_TIME_CHECKS = 5 #How many times to test a TS chunk download to get its average download time
-TS_DOWNLOAD_SPEEDFACTOR_REQUIREMENT = 2 #TS chunks must be able to download this many times faster than their duration to be usable in a cache. Cannot be less than 1
+class ChatCommand():
+    """Chat command abstract class"""
+    def __init__(self, name, actor, cooldown = SEND_MESSAGE_COOLDOWN, amount_cents = 0, exclusive = False, allowed_badges = ["subscriber"], whitelist_badges = ["moderator"], target = None):
+        """name: The !name of the command
+    actor: The RumleChatActor host object
+    amount_cents: The minimum cost of the command. Defaults to free
+    exclusive: If this command can only be run by users with allowed badges. Defaults to False
+    allowed_badges: Badges that are allowed to run this command (if it is exclusive).
+       ChatCommand,  Defaults to subscribers, admin is added internally.
+    whitelist_badges: Badges which if borne give the user free-of-charge command access
+    target: The command function(message, actor) to call. Defaults to self.run"""
+        assert " " not in name, "Name cannot contain spaces"
+        self.name = name
+        self.actor = actor
+        assert cooldown >= SEND_MESSAGE_COOLDOWN, \
+            f"Cannot set a cooldown shorter than {SEND_MESSAGE_COOLDOWN}"
+
+        self.cooldown = cooldown
+        self.amount_cents = amount_cents #Cost of the command
+        self.exclusive = exclusive
+        self.allowed_badges = ["admin"] + allowed_badges #Admin can always run any command
+        self.whitelist_badges = ["admin"] + whitelist_badges #Admin always has free-of-charge usage
+        self.last_use_time = 0 #Last time the command was called
+        self.target = target
+        self.__set_help_message = None
+
+    @property
+    def help_message(self):
+        """The help message for this command"""
+        if self.__set_help_message:
+            return self.__set_help_message
+
+        return "No specific help for this command"
+
+    @help_message.setter
+    def help_message(self, new):
+        """Set the help message for this command externally"""
+        self.__set_help_message = str(new)
+
+    def call(self, message):
+        """The command was called"""
+        #this command is exclusive, and the user does not have the required badge
+        if self.exclusive and \
+            not (True in [badge.slug in self.allowed_badges for badge in message.user.badges]):
+
+            self.actor.send_message(f"@{message.user.username} That command is exclusive to: " +
+                                    ", ".join(self.allowed_badges)
+                                    )
+
+            return
+
+        #The command is still on cooldown
+        if (curtime := time.time()) - self.last_use_time < self.cooldown:
+            self.actor.send_message(
+                f"@{message.user.username} That command is still on cooldown. " +
+                f"Try again in {int(self.last_use_time + self.cooldown - curtime + 0.5)} seconds."
+                )
+
+            return
+
+        #the user did not pay enough for the command and they do not have a free pass
+        if message.rant_price_cents < self.amount_cents and \
+            not (True in [badge.slug in self.whitelist_badges for badge in message.user.badges]):
+
+            self.actor.send_message("@" + message.user.username +
+                                    f"That command costs ${self.amount_cents/100:.2f}."
+                                    )
+            return
+
+        #the command was called successfully
+        self.run(message)
+
+        #Mark the last use time for cooldown
+        self.last_use_time = time.time()
+
+    def run(self, message):
+        """Dummy run method"""
+        if self.target:
+            self.target(message, self.actor)
+            return
+
+        #Run method was never defined
+        self.actor.send_message("@" + message.user.username +
+                                "Hello, this command never had a target defined. :-)"
+                                )
 
 class TTSCommand(ChatCommand):
     """Text-to-speech command"""
-    def __init__(self, *args, name = "tts", voices = {"default" : talkey.Talkey().say}, **kwargs):
+    def __init__(self, *args, name = "tts", voices = {}, **kwargs):
         """Pass the same args and kwargs as ChatCommand, plus:
     voices: Dict of voice : say(text) callable"""
         super().__init__(*args, name = name, **kwargs)
         self.voices = voices
 
-        #Get the default voice
-        self.default_voice = voices["default"]
+        #Make sure we have a default voice
+        if "default" not in self.voices:
+            self.voices["default"] = talkey.Talkey().say
+
+    @property
+    def help_message(self):
+        """The help message for this command"""
+        return f"Speak your message{f" for ${self.amount_cents/100: .2%}" if self.amount_cents else ""}." + \
+            f"Use {COMMAND_PREFIX + self.name} [voice] Your message. Available voices are: " + ", ".join(self.voices)
+
+    @property
+    def default_voice(self):
+        """The default TTS voice as a say(text) callable"""
+        return self.voices["default"]
 
     def speak(self, text, voice = None):
         """Speak text with voice"""
         if not voice:
             self.default_voice(text)
 
         #Voice was not actually in our list of voices
@@ -82,35 +170,68 @@
     def __init__(self, actor, name = "lurk", text = "@{username} is now lurking. Enjoy!"):
         """actor: The Rumble chat actor host
     name = lurk: the command name
     text: A message to format with a username and post"""
         super().__init__(name = name, actor = actor)
         self.text = text
 
+    @property
+    def help_message(self):
+        """The help message for this command"""
+        return "Notify the chat that you are lurking."
+
     def run(self, message):
         """Run the lurk"""
         self.actor.send_message(self.text.format(username = message.user.username))
 
 class HelpCommand(ChatCommand):
     """List available commands"""
     def __init__(self, actor, name = "help"):
         """actor: The Rumble chat actor host
     name = help: the command name"""
         super().__init__(name = name, actor = actor)
 
+    @property
+    def help_message(self):
+        """The help message for this command"""
+        return f"Get help on a specific command with {COMMAND_PREFIX + self.name} [command_name] or run alone to list all available commands."
+
     def run(self, message):
         """Run the help command"""
-        self.actor.send_message("The following commands are registered: " + ", ".join(self.actor.chat_commands))
+        segs = message.split()
+
+        #Command was run without arguments
+        if len(segs) == 1:
+            self.actor.send_message("The following commands are registered: " + ", ".join(self.actor.chat_commands))
+
+        #Command had one argument
+        elif len(segs) == 2:
+            #Argument is a valid command
+            if segs[-1] in self.actor.chat_commands:
+                self.actor.send_message(segs[-1] + " command: " + self.actor.chat_commands[segs[-1]].help_message)
+
+            #Argument is something else
+            else:
+                self.actor.send_message(f"Cannot provide help for '{segs[-1]}' as it is not a registered command.")
+
+        #Command has more than one argument
+        else:
+            self.actor.send_message("Invalid number of arguments for help command.")
 
 class KillswitchCommand(ChatCommand):
     """A killswitch for Rumchat Actor if moderators or admin need to shut it down from the chat"""
     def __init__(self, actor, name = "killswitch", allowed_badges = ["moderator"]):
         """Pass the Rumchat Actor, the command name, and the badges allowed to use it"""
         super().__init__(name = name, actor = actor, exclusive = True, allowed_badges = allowed_badges)
 
+    @property
+    def help_message(self):
+        """The help message for this command"""
+        return "Shut down RumChat Actor."
+
     def run(self, message):
         """Shut down Rumchat Actor"""
         try:
             self.actor.send_message("Shutting down.")
             self.actor.quit()
         finally:
             print("Killswitch thrown.")
@@ -139,18 +260,25 @@
         self.ts_durations = {} #The duration of a TS chunk of a given stream quality
         self.is_dvr = False #Wether the stream is a DVR or not, detected later. No TS cache is needed if it is
         self.use_quality = None #The quality of stream to use, detected later, based on download speeds
         self.ts_url_start = "" #The start of the m3u8 and TS URLs, to be formatted with the selected quality, detected later
         self.m3u8_filename = "" #The filename of the m3u8 playlist, will be either chunklist.m3u8 or chunklist_DVR.m3u8, detected later
         self.saved_ts = {} #TS filenames : Tempfile objects containing TS chunks
         self.discarded_ts = [] #TS names that were saved then deleted
+        self.clip_uploader = None #An object to upload the clips when they are complete
         self.recorder_thread = threading.Thread(target = self.record_loop, daemon = True)
         self.run_recorder = True
         self.recorder_thread.start()
 
+    @property
+    def help_message(self):
+        """The help message for this command"""
+        return f"Save a clip from the livestream. Use {COMMAND_PREFIX + self.name} [duration] [custom clip name]." + \
+            f"Default duration is {self.default_duration}, max duration is {self.max_duration}."
+
     def get_ts_list(self, quality):
         """Download an m3u8 playlist and parse it for TS filenames"""
         assert self.ts_url_start and self.m3u8_filename, "Must have the TS URL start and the m3u8 filename before this runs"
         m3u8 = requests.get(self.ts_url_start.format(quality = quality) + self.m3u8_filename, timeout = DEFAULT_TIMEOUT).content.decode()
         return [line for line in m3u8.splitlines() if not line.startswith("#")]
 
     def record_loop(self):
@@ -202,15 +330,15 @@
             #Stream is not live or upcoming
             else:
                 print("Stream is not live or upcoming! Critical error.")
                 self.actor.quit()
                 return
 
             #Stream is still upcoming
-            time.sleep(WAIT_FOR_LIVE_REFRESH_RATE)
+            time.sleep(WAIT_FOR_PAGE_CONDITION_REFRESH_RATE)
             browser.refresh()
             stream_griditem = browser.find_element(By.XPATH,
                                                     "//div[@class='videostream thumbnail__grid--item']" +
                                                     f"[@data-video-id='{self.actor.stream_id_b10}']"
                                                         )
 
         #Watch the network traffic for the m3u8 URL
@@ -408,16 +536,23 @@
             use_ts = available_chunks[- int(duration / self.ts_durations[self.use_quality] + 0.5):]
 
         #No filename specified, construct from time values
         if not filename:
             t = time.time()
             filename = f"{round(t - self.ts_durations[self.use_quality] * len(use_ts))}-{round(t)}"
 
-        self.actor.send_message(f"Saving clip {filename}, duration of {round(self.ts_durations[self.use_quality] * len(use_ts))} seconds.")
-        saveclip_thread = threading.Thread(target = self.form_ts_into_clip, args = (filename, use_ts), daemon = True)
+        #Avoid overwriting other clips
+        increment = 0
+        safe_filename = filename
+        while safe_filename + "." + CLIP_FILENAME_EXTENSION in glob.glob("*", root_dir = self.clip_save_path):
+            increment += 1
+            safe_filename = filename + f"({increment})"
+
+        self.actor.send_message(f"Saving clip {safe_filename}, duration of {round(self.ts_durations[self.use_quality] * len(use_ts))} seconds.")
+        saveclip_thread = threading.Thread(target = self.form_ts_into_clip, args = (safe_filename, use_ts), daemon = True)
         saveclip_thread.start()
 
     def form_ts_into_clip(self, filename, use_ts):
         """Do the actual TS [down]loading and processing, and save the video clip"""
         #Download the TS chunks if this is a DVR stream
         if self.is_dvr:
             print("Downloading TS for clip")
@@ -454,14 +589,19 @@
             print("ERROR: Running clipsaves is now negative. Resetting it to zero, but this should not happen.")
             self.running_clipsaves = 0
 
         #We are responsible for DVR tempfile closing
         if self.is_dvr:
             for tf in tempfiles:
                 tf.close()
+
+        #Upload the clip
+        if self.clip_uploader:
+            self.clip_uploader.upload_clip(filename)
+
         print("Complete")
 
 class ClipRecordingCommand(ChatCommand):
     """Save clips of the livestream by duplicating then trimming an in-progress TS recording by OBS"""
     def __init__(self, actor, name = "clip", default_duration = 60, max_duration = 120, recording_load_path = ".", clip_save_path = "." + os.sep):
         """actor: The Rumchat Actor
     name: The name of the command
@@ -473,14 +613,21 @@
         self.default_duration = default_duration
         self.max_duration = max_duration
         self.recording_load_path = recording_load_path
         self.clip_save_path = clip_save_path #Where to save the completed clips
         self.running_clipsaves = 0 #How many clip save operations are running
         self.__recording_filename = None #The filename of the running OBS recording, asked later
         print(self.recording_filename) #...now is later
+        self.clip_uploader = None #An object to upload the clips when they are complete
+
+    @property
+    def help_message(self):
+        """The help message for this command"""
+        return f"Save a clip from the livestream. Use {COMMAND_PREFIX + self.name} [duration] [custom clip name]." + \
+            f"Default duration is {self.default_duration}, max duration is {self.max_duration}."
 
     @property
     def recording_filename(self):
         """The filename of the running OBS recording"""
         #We do not know the filename yet
         while not self.__recording_filename:
             #Make and hide a background Tk window to allow filedialogs to appear
@@ -541,37 +688,45 @@
     def save_clip(self, duration, filename = None):
         """Save a clip with the given duration to the filename"""
         #No filename specified, construct from time values
         if not filename:
             t = time.time()
             filename = f"{round(t - duration)}-{round(t)}"
 
+        #Avoid overwriting other clips
+        increment = 0
+        safe_filename = filename
+        while safe_filename + "." + CLIP_FILENAME_EXTENSION in glob.glob("*", root_dir = self.clip_save_path):
+            increment += 1
+            safe_filename = filename + f"({increment})"
+
         #Report clip save
-        self.actor.send_message(f"Saving clip {filename}, duration of {duration} seconds.")
+        self.actor.send_message(f"Saving clip {safe_filename}, duration of {duration} seconds.")
 
         #Run the clip save in a thread
-        saveclip_thread = threading.Thread(target = self.form_recording_into_clip, args = (duration, filename), daemon = True)
+        saveclip_thread = threading.Thread(target = self.form_recording_into_clip, args = (duration, safe_filename), daemon = True)
         saveclip_thread.start()
 
     def form_recording_into_clip(self, duration, filename):
         """Do the actual file operations to save a clip"""
         #Keep a counter of running clipsaves, may not be needed
         self.running_clipsaves += 1
 
         print("Making frozen copy of recording")
         shutil.copy(self.recording_filename, self.recording_copy_fn)
         print("Loading copy")
         recording = VideoFileClip(self.recording_copy_fn)
-        print("Trimming")
-        clip = recording.subclip(max((recording.duration - duration, 0)), recording.duration)
-        print("Saving clip")
-        clip.write_videofile(self.clip_save_path + os.sep + filename + "." + CLIP_FILENAME_EXTENSION, logger = None)
+        print("Saving trimmed clip")
+        ffmpeg_extract_subclip(self.recording_copy_fn, max((recording.duration - duration, 0)), recording.duration, targetname = self.clip_save_path + os.sep + filename + "." + CLIP_FILENAME_EXTENSION)
         print("Closing and deleting frozen copy")
         recording.close()
         os.system("rm " + self.recording_copy_fn)
         print("Done.")
 
         #Make note that the clipsave has finished
         self.running_clipsaves -= 1
         if self.running_clipsaves < 0:
             print("ERROR: Running clipsaves is now negative. Resetting it to zero, but this should not happen.")
             self.running_clipsaves = 0
+
+        if self.clip_uploader:
+            self.clip_uploader.upload_clip(filename)
```

### Comparing `rumchat_actor-1.3.0/LICENSE.txt` & `rumchat_actor-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rumchat_actor-1.3.0/README.md` & `rumchat_actor-2.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 #Otherwise, you will have to log in manuaglly each time you use the bot, or pass credentials = (username, password).
 actor = rumchat_actor.RumbleChatActor(stream_id = STREAM_ID)
 
 #Register an action to be called on every message
 actor.register_message_action(eat_some_cheese)
 
 #Register a command via the ChatCommand class
-actor.register_command(rumchat_actor.ChatCommand(name = "hi", actor = actor, target = lambda message, actor: actor.send_message(f"Hello, @{message.user.username}!")))
+actor.register_command(rumchat_actor.commands.ChatCommand(name = "hi", actor = actor, target = lambda message, actor: actor.send_message(f"Hello, @{message.user.username}!")))
 
 #Register a command via a callable
 actor.register_command(name = "tester", command = lambda message, actor: print(f"Test command run by {message.user.username}"))
 
 #Run the bot continuously
 actor.mainloop()
 ```
```

### Comparing `rumchat_actor-1.3.0/pyproject.toml` & `rumchat_actor-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rumchat_actor"
-version = "1.3.0"
+version = "2.0.0"
 keywords = ["rumble", "chat", "livestream", "bot"]
 authors = [
   { name="Wilbur Jaywright", email="zargulthewizard@outlook.com" },
 ]
 description = "Automatically interact with your Rumble livestream chats."
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
   "browsermobproxy",
-  "cocorum>=1.0.0",
+  "cocorum",
   "moviepy",
   "requests",
   "selenium",
   "talkey",
   ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `rumchat_actor-1.3.0/PKG-INFO` & `rumchat_actor-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.3
 Name: rumchat_actor
-Version: 1.3.0
+Version: 2.0.0
 Summary: Automatically interact with your Rumble livestream chats.
 Project-URL: Homepage, https://github.com/thelabcat/rum-chat-actor
 Project-URL: Issues, https://github.com/thelabcat/rumble-api-wrapper-py/issues
 Author-email: Wilbur Jaywright <zargulthewizard@outlook.com>
 License-File: LICENSE.txt
 Keywords: bot,chat,livestream,rumble
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: browsermobproxy
-Requires-Dist: cocorum>=1.0.0
+Requires-Dist: cocorum
 Requires-Dist: moviepy
 Requires-Dist: requests
 Requires-Dist: selenium
 Requires-Dist: talkey
 Description-Content-Type: text/markdown
 
 # Rumble Chat Actor
@@ -49,15 +49,15 @@
 #Otherwise, you will have to log in manuaglly each time you use the bot, or pass credentials = (username, password).
 actor = rumchat_actor.RumbleChatActor(stream_id = STREAM_ID)
 
 #Register an action to be called on every message
 actor.register_message_action(eat_some_cheese)
 
 #Register a command via the ChatCommand class
-actor.register_command(rumchat_actor.ChatCommand(name = "hi", actor = actor, target = lambda message, actor: actor.send_message(f"Hello, @{message.user.username}!")))
+actor.register_command(rumchat_actor.commands.ChatCommand(name = "hi", actor = actor, target = lambda message, actor: actor.send_message(f"Hello, @{message.user.username}!")))
 
 #Register a command via a callable
 actor.register_command(name = "tester", command = lambda message, actor: print(f"Test command run by {message.user.username}"))
 
 #Run the bot continuously
 actor.mainloop()
 ```
```

