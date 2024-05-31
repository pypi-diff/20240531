# Comparing `tmp/hugchat-0.4.6.tar.gz` & `tmp/hugchat-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugchat-0.4.6.tar", last modified: Wed May 22 03:08:33 2024, max compression
+gzip compressed data, was "hugchat-0.4.7.tar", last modified: Fri May 31 08:45:43 2024, max compression
```

## Comparing `hugchat-0.4.6.tar` & `hugchat-0.4.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:08:33.041164 hugchat-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-22 03:08:29.000000 hugchat-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-05-22 03:08:33.041164 hugchat-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-22 03:08:29.000000 hugchat-0.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 03:08:33.041164 hugchat-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-22 03:08:29.000000 hugchat-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:08:33.037163 hugchat-0.4.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:08:33.041164 hugchat-0.4.6/src/hugchat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 03:08:29.000000 hugchat-0.4.6/src/hugchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-05-22 03:08:29.000000 hugchat-0.4.6/src/hugchat/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-22 03:08:29.000000 hugchat-0.4.6/src/hugchat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    30347 2024-05-22 03:08:29.000000 hugchat-0.4.6/src/hugchat/hugchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-05-22 03:08:29.000000 hugchat-0.4.6/src/hugchat/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-05-22 03:08:29.000000 hugchat-0.4.6/src/hugchat/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:08:33.041164 hugchat-0.4.6/src/hugchat/types/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-22 03:08:29.000000 hugchat-0.4.6/src/hugchat/types/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-22 03:08:29.000000 hugchat-0.4.6/src/hugchat/types/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-22 03:08:29.000000 hugchat-0.4.6/src/hugchat/types/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:08:33.041164 hugchat-0.4.6/src/hugchat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-05-22 03:08:33.000000 hugchat-0.4.6/src/hugchat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-22 03:08:33.000000 hugchat-0.4.6/src/hugchat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 03:08:33.000000 hugchat-0.4.6/src/hugchat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 03:08:33.000000 hugchat-0.4.6/src/hugchat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 03:08:33.000000 hugchat-0.4.6/src/hugchat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:45:43.555865 hugchat-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-31 08:45:39.000000 hugchat-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-05-31 08:45:43.555865 hugchat-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-31 08:45:39.000000 hugchat-0.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 08:45:43.555865 hugchat-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-31 08:45:39.000000 hugchat-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:45:43.551865 hugchat-0.4.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:45:43.551865 hugchat-0.4.7/src/hugchat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:45:39.000000 hugchat-0.4.7/src/hugchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-05-31 08:45:39.000000 hugchat-0.4.7/src/hugchat/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-31 08:45:39.000000 hugchat-0.4.7/src/hugchat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30785 2024-05-31 08:45:39.000000 hugchat-0.4.7/src/hugchat/hugchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-05-31 08:45:39.000000 hugchat-0.4.7/src/hugchat/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-05-31 08:45:39.000000 hugchat-0.4.7/src/hugchat/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:45:43.555865 hugchat-0.4.7/src/hugchat/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-31 08:45:39.000000 hugchat-0.4.7/src/hugchat/types/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-31 08:45:39.000000 hugchat-0.4.7/src/hugchat/types/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-31 08:45:39.000000 hugchat-0.4.7/src/hugchat/types/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:45:43.555865 hugchat-0.4.7/src/hugchat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-05-31 08:45:43.000000 hugchat-0.4.7/src/hugchat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-31 08:45:43.000000 hugchat-0.4.7/src/hugchat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 08:45:43.000000 hugchat-0.4.7/src/hugchat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-31 08:45:43.000000 hugchat-0.4.7/src/hugchat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 08:45:43.000000 hugchat-0.4.7/src/hugchat.egg-info/top_level.txt
```

### Comparing `hugchat-0.4.6/LICENSE` & `hugchat-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.6/PKG-INFO` & `hugchat-0.4.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.4.6
+Version: 0.4.7
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -142,26 +142,27 @@
 - `-p` : Force request password to login, ignores saved cookies.
 - `-s` : Enable streaming mode output in CLI.
 - `-c` : Continue previous conversation in CLI ".
 
 Commands in cli mode:
 
 - `/new` : Create and switch to a new conversation.
-- `/ids` : Shows a list of all ID numbers and ID strings in current session.
-- `/switch <id>` : Switches to the ID number or ID string passed.
-- `/del <id>` : Deletes the ID number or ID string passed. Will not delete active session.
+- `/ids` : Shows a list of all ID numbers and ID strings in *current session*.
+- `/switch` : Shows a list of all conversations' info in *current session*. Then you can choose one to switch to.
+- `/switch all` : Shows a list of all conversations' info in *your account*. Then you can choose one to switch to. (not recommended if your account has a lot of conversations)
+- `/del <index>` : Deletes the conversation linked with the index passed. Will not delete active session.
 - `/delete-all` : Deletes all the conversations for the logged in user.
 - `/clear` : Clear the terminal.
 - `/llm` : Get available models you can switch to.
 - `/llm <index>` : Switches model to given model index based on `/llm`.
-- `/sharewithauthor <on|off>` : Changes settings for sharing data with model author. On by default.
+- `/share` : Toggles settings for sharing data with model author. On by default.
 - `/exit` : Closes CLI environment.
-- `/stream <on|off>`: streaming the response.
-- `/web <on|off>`: web search.
-- `/web-hint <on|off>`: display web search hint.
+- `/stream` : Toggles streaming the response.
+- `/web` : Toggles web search.
+- `/web-hint` : Toggles display web search hint.
 
 - AI is an area of active research with known problems such as biased generation and misinformation. Do not use this application for high-stakes decisions or advice.
 - Server resources are precious, it is not recommended to request this API in a high frequency.
 (`Hugging Face's CTO🤗` just liked the suggestion)
 <div align="center"><img width=500 src="https://github.com/Soulter/hugging-chat-api/assets/37870767/06e64501-02fb-4d4a-ab6f-cf18d8638ace"></img></div>
```

### Comparing `hugchat-0.4.6/README.md` & `hugchat-0.4.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -116,26 +116,27 @@
 - `-p` : Force request password to login, ignores saved cookies.
 - `-s` : Enable streaming mode output in CLI.
 - `-c` : Continue previous conversation in CLI ".
 
 Commands in cli mode:
 
 - `/new` : Create and switch to a new conversation.
-- `/ids` : Shows a list of all ID numbers and ID strings in current session.
-- `/switch <id>` : Switches to the ID number or ID string passed.
-- `/del <id>` : Deletes the ID number or ID string passed. Will not delete active session.
+- `/ids` : Shows a list of all ID numbers and ID strings in *current session*.
+- `/switch` : Shows a list of all conversations' info in *current session*. Then you can choose one to switch to.
+- `/switch all` : Shows a list of all conversations' info in *your account*. Then you can choose one to switch to. (not recommended if your account has a lot of conversations)
+- `/del <index>` : Deletes the conversation linked with the index passed. Will not delete active session.
 - `/delete-all` : Deletes all the conversations for the logged in user.
 - `/clear` : Clear the terminal.
 - `/llm` : Get available models you can switch to.
 - `/llm <index>` : Switches model to given model index based on `/llm`.
-- `/sharewithauthor <on|off>` : Changes settings for sharing data with model author. On by default.
+- `/share` : Toggles settings for sharing data with model author. On by default.
 - `/exit` : Closes CLI environment.
-- `/stream <on|off>`: streaming the response.
-- `/web <on|off>`: web search.
-- `/web-hint <on|off>`: display web search hint.
+- `/stream` : Toggles streaming the response.
+- `/web` : Toggles web search.
+- `/web-hint` : Toggles display web search hint.
 
 - AI is an area of active research with known problems such as biased generation and misinformation. Do not use this application for high-stakes decisions or advice.
 - Server resources are precious, it is not recommended to request this API in a high frequency.
 (`Hugging Face's CTO🤗` just liked the suggestion)
 <div align="center"><img width=500 src="https://github.com/Soulter/hugging-chat-api/assets/37870767/06e64501-02fb-4d4a-ab6f-cf18d8638ace"></img></div>
```

### Comparing `hugchat-0.4.6/setup.py` & `hugchat-0.4.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_namespace_packages
 from setuptools import setup
 
 setup(
     name="hugchat",
-    version="0.4.6",
+    version="0.4.7",
     description="A huggingchat python api.",
     long_description=open("README.md", "rt", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Soulter/hugging-chat-api",
     project_urls={
         "Bug Report": "https://github.com/Soulter/hugging-chat-api/issues"
     },
```

### Comparing `hugchat-0.4.6/src/hugchat/cli.py` & `hugchat-0.4.7/src/hugchat/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,115 +36,160 @@
 
     arguments = userInput.lower().split(" ")
     command = arguments[0][1:] # Remove the '/' at the start of the input
     arguments = arguments[1:]
 
     if command == "help" or command == "commands":
         print("""
-/new: Create and switch to a new conversation.
-/ids: Shows a list of all ID numbers and ID strings in *current session*.
-/switch <id>: Switches to the ID number or ID string passed.
-/switch: Shows a list of all conversations' info in *current session*. Then you can choose one to switch to.
-/switch all: Shows a list of all conversations' info in *your account*. Then you can choose one to switch to. (not recommended if your account has a lot of conversations)
-/del <id>: Deletes the ID number or ID string passed. Will not delete active session.
-/delete-all: Deletes all the conversations for the logged in user.
-/clear: Clear the terminal.
-/llm: Get available models you can switch to.
-/llm <index>: Switches model to given model index based on /llm.
-/sharewithauthor <on|off>: Changes settings for sharing data with model author. On by default.
+/new : Create and switch to a new conversation.
+/ids : Shows a list of all ID numbers and ID strings in *current session*.
+/switch : Shows a list of all conversations' info in *current session*. Then you can choose one to switch to.
+/switch all : Shows a list of all conversations' info in *your account*. Then you can choose one to switch to. (not recommended if your account has a lot of conversations)
+/del <index> : Deletes the conversation linked with the index passed. Will not delete active session.
+/delete-all : Deletes all the conversations for the logged in user.
+/clear : Clear the terminal.
+/llm : Get available models you can switch to.
+/llm <index> : Switches model to given model index based on /llm.
+/share : Toggles settings for sharing data with model author. On by default.
 /exit : Closes CLI environment.
-/stream <on|off>: streaming the response.
-/web <on|off>: web search.
-/web-hint <on|off>: display web search hint.
+/stream : Toggles streaming the response.
+/web : Toggles web search.
+/web-hint : Toggles display web search hint.
         """)
 
     elif command == "new":
         new_conversation = chatbot.new_conversation(switch_to=True)
-        print(f"# Created and switched to a new conversation\n# New conversation ID: {new_conversation.id}")
+        conversation_index = len(chatbot.get_conversation_list())
+        print(f"# Created and switched to a new conversation\n# New conversation ID: {new_conversation.id}\n# New conversation index: {conversation_index}")
 
     elif command == "ids":
-        print(f"# Conversations: {[conversation.id for conversation in chatbot.get_conversation_list()]}")
+        print(f"# Conversations: ")
+        for i, conversation in enumerate(chatbot.get_conversation_list()):
+            print(f"# {i+1}.) {conversation.id}{' (acitve)' if chatbot.get_conversation_info().id == conversation.id else ''}")
 
     elif command == "switch":
         try:
-            if arguments[0] == "all":
+            if arguments and arguments[0] == "all":
                 id = chatbot.get_remote_conversations(replace_conversation_list=True)
-            else:
+            elif not arguments:
                 id = chatbot.get_conversation_list()
-
+            else:
+                print("# Invalid argument(s).")
+                return
             conversation_dict = {i+1: id_string for i, id_string in enumerate(id)}
 
             for i, id_string in conversation_dict.items():
                 info = chatbot.get_conversation_info(id_string)
-                print(f"{i}: ID: {info.id}\nTitle: {info.title[:43]}...\nModel: {info.model}.\nSystem Prompt: {info.system_prompt}\n--------------------------------------------------------")
+                print(f"# {i}: ID: {info.id}\n# Title: {info.title[:43]}...\n# Model: {info.model}.\n# System Prompt: {info.system_prompt}\n# --------------------------------------------------------")
 
-            index_value = int(input("Choose conversation ID(input the index): "))
+            index_value = int(input("# Choose conversation ID(input the index): "))
             target_id = conversation_dict.get(index_value)
 
             if target_id:
                 chatbot.change_conversation(target_id)
-                print(f"Switched to conversation with ID: {target_id}\n")
+                print(f"# Switched to conversation with ID: {target_id}\n")
             else:
-                print("Invalid conversation ID")
+                print("# Invalid conversation ID")
         except Exception as e:
-            print(f"Error: {e}")
+            if isinstance(e, ValueError):
+                print(f"# Invlid argument.")
+            else:
+                print(f"# Error: {e}")
 
     elif command == "del" or command == "delete":
         try:
-            to_delete_conversation = chatbot.get_conversation_from_id(arguments[0])
-        except Exception:
-            print("# Unable to delete conversation with ID. Conversation ID not found.")
+            if not arguments:
+                print("# No argument for index provided.")
+                return
+
+            conversation_index = int(arguments[0])
+            if conversation_index < 1:
+                raise IndexError()
+            selected_conversation = chatbot.get_conversation_list()[conversation_index-1].id
+            current_conversation_id = chatbot.get_conversation_info().id
+
+            if selected_conversation == current_conversation_id:
+                print("# Cannot delete active chat.")
+                return
+            
+            to_delete_conversation = chatbot.get_conversation_from_id(selected_conversation)
+        except Exception as e:
+            if isinstance(e, ValueError):
+                print("# Invalid argument for index.")
+            else:
+                print("# Invalid index.")
             return
-
-        chatbot.delete_conversation(to_delete_conversation)
-
-        print("# Deleted conversation successfully")
+        
+        if not to_delete_conversation is None:
+            chatbot.delete_conversation(to_delete_conversation)
+            print("# Deleted conversation successfully.")
+            return
+        print("# Error")
 
     elif command == "delete-all" or command == "deleteall":
-        chatbot.delete_all_conversations()
-        print("# Deleted all conversations successfully")
+        if input("# WARNING: This will delete all conversations linked with this account. Continue? (y/n) : ").lower() == 'y':
+            chatbot.delete_all_conversations()
+            print("# Deleted all conversations successfully")
 
-        new_conversation = chatbot.new_conversation(switch_to=True)
-        print(f"# Created and switched to a new conversation\n# New conversation ID: {new_conversation.id}")
+            new_conversation = chatbot.new_conversation(switch_to=True)
+            print(f"# Created and switched to a new conversation\n# New conversation ID: {new_conversation.id}")
 
     elif command == "clear" or command == "cls":
         os.system('cls' if os.name == 'nt' else 'clear')
 
     elif command == "llm":
         if len(arguments) == 0:
-            print(f"# Available Models: {[model.id for model in chatbot.get_available_llm_models()]}")
+            print(f"# Available Models: ")
+            for i, model in enumerate(chatbot.get_available_llm_models()):
+                print(f"# {i+1}.) {model.id}")
             return
 
         try:
-            chatbot.switch_llm(int(arguments[0]))
-        except ValueError:
-            print("# Invalid LLM index")
+            chatbot.switch_llm(int(arguments[0])-1)
+        except Exception as e:
+            if isinstance(e, ValueError):
+                print("# Not a valid argument")
+            elif isinstance(e, IndexError):
+                print("# Invalid LLM index")
+            else:
+                print(e)
             return
 
         print(f"# Switched to LLM {chatbot.active_model.id}\n# Please note that you have to create a new conversation for this to take effect")
 
-    elif command == "sharewithauthor":
-        sharing = arguments[0] == "on"
-        chatbot.set_share_conversations(sharing)
-
-        print(f"# {'Now sharing conversations with model author' if sharing else 'No longer sharing conversations with model author'}")
+    elif command == "share":
+        if arguments:
+            chatbot.sharing = arguments[0] == "on"
+        else:
+            chatbot.sharing = not chatbot.sharing
+        try:
+            chatbot.set_share_conversations(chatbot.sharing)
+            print(f"# {'Now sharing conversations with model author' if chatbot.sharing else 'No longer sharing conversations with model author'}")
+        except Exception as e:
+            print(f"# Error: {e}\n")
 
     elif command == "stream" or command == "streamoutput":
-        stream_output = arguments[0] == "on"
-
+        if arguments:
+            stream_output = arguments[0] == "on"
+        else:
+            stream_output = not stream_output
         print(f"# {'Now streaming responses' if stream_output else 'No longer streaming responses'}")
 
     elif command == "web" or command == "websearch":
-        is_web_search = arguments[0] == "on"
-
+        if arguments:
+            is_web_search = arguments[0] == "on"
+        else:
+            is_web_search = not is_web_search
         print(f"# {'Web searching activated' if is_web_search else 'We searching deactivated'}")
 
     elif command == "web-hint" or command == "webhint":
-        web_search_hint = arguments[0] == "on"
-
+        if arguments:
+            web_search_hint = arguments[0] == "on"
+        else:
+            web_search_hint = not web_search_hint
         print(f"# {'Enabled web hint' if web_search_hint else 'Disabled web hint'}")
 
     else:
         print("# Unrecognized command")
 
 
 def stream_response(generator) -> None:
```

### Comparing `hugchat-0.4.6/src/hugchat/exceptions.py` & `hugchat-0.4.7/src/hugchat/exceptions.py`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.6/src/hugchat/hugchat.py` & `hugchat-0.4.7/src/hugchat/hugchat.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 
         self.cookies = cookies
 
         self.hf_base_url = "https://huggingface.co"
         self.json_header = {"Content-Type": "application/json"}
         self.session = self.get_hc_session()
         self.conversation_list = []
+        self.sharing = True
         self.accepted_welcome_modal = (
             False  # It is no longer required to accept the welcome modal
         )
 
         self.llms = self.get_remote_llms()
 
         if isinstance(default_llm, str):
@@ -499,22 +500,26 @@
             conversations.append(c)
 
         if replace_conversation_list:
             self.conversation_list = conversations
 
         return conversations
 
-    def get_conversation_info(self, conversation: Conversation = None) -> Conversation:
+    def get_conversation_info(self, conversation: Union[Conversation, str] = None) -> Conversation:
         """
         Fetches information related to the specified conversation. Returns the conversation object.
+        conversation: Conversation object that has the conversation id Or None to use the current conversation.
         """
 
         if conversation is None:
             conversation = self.current_conversation
 
+        if isinstance(conversation, str):
+            conversation = Conversation(id=conversation)
+
         r = self.session.get(
             self.hf_base_url +
             f"/chat/conversation/{conversation.id}/__data.json?x-sveltekit-invalidated=01",
             headers=self.get_headers(ref=False),
             cookies=self.get_cookies(),
         )
 
@@ -603,14 +608,15 @@
         if res['nodes'][1]['type'] == 'error':
             return None
         # here we parse the result
         return self._parse_assistants(res['nodes'][1]['data'])
 
     def search_assistant(self, assistant_name: str = None, assistant_id: str = None) -> Assistant:
         '''
+        - If you created an assistant by your own, you should pass the assistant_id here but not the assistant_name. You can pass your assistant_id into the new_conversation() directly.
         - Search an available assistant by assistant name or assistant id.
         - Will search on api.soulter.top/hugchat because offifial api doesn't support search.
         - Return the `Assistant` object if found, return None if not found.
         '''
         if not assistant_name and not assistant_id:
             raise ValueError(
                 "assistant_name and assistant_id can not be both None.")
```

### Comparing `hugchat-0.4.6/src/hugchat/login.py` & `hugchat-0.4.7/src/hugchat/login.py`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.6/src/hugchat/message.py` & `hugchat-0.4.7/src/hugchat/message.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,32 +54,39 @@
         # or simply use:
         final = msg.wait_until_done()
     """
 
     g: Generator
     _stream_yield_all: bool = False
     web_search: bool = False
-
     web_search_sources: list = []
-    # For backward compatibility, we have to reserve the `text` field.
-    text: str = ""
+    _result_text: str = ""
     web_search_done: bool = not web_search
     msg_status: int = MSGSTATUS_PENDING
     error: Union[Exception, None] = None
 
     def __init__(
         self,
         g: Generator,
         _stream_yield_all: bool = False,
         web_search: bool = False,
     ) -> None:
         self.g = g
         self._stream_yield_all = _stream_yield_all
         self.web_search = web_search
 
+    @property
+    def text(self) -> str:
+        self._result_text = self.wait_until_done()
+        return self._result_text
+    
+    @text.setter
+    def text(self, v: str) -> None:
+        self._result_text = v
+
     def _filterResponse(self, obj: dict):
         if not obj.__contains__("type"):
             if obj.__contains__("message"):
                 raise ChatError(f"Server returns an error: {obj['message']}")
             else:
                 raise ChatError(f"No `type` and `message` returned: {obj}")
 
@@ -95,15 +102,15 @@
 
         try:
             a: dict = next(self.g)
             self._filterResponse(a)
             t: str = a["type"]
             message_type: str = ""
             if t == RESPONSE_TYPE_FINAL:
-                self.text = a["text"]
+                self._result_text = a["text"]
                 self.msg_status = MSGSTATUS_RESOLVED
             elif t == RESPONSE_TYPE_WEB:
                 # gracefully pass unparseable webpages
                 if message_type != MSGTYPE_ERROR and a.__contains__("sources"):
                     self.web_search_sources.clear()
                     sources = a["sources"]
                     for source in sources:
@@ -191,15 +198,15 @@
             - self.text if resolved else raise error
 
         wait until every response is resolved
         """
         while not self.is_done():
             self.__next__()
         if self.is_done() == MSGSTATUS_RESOLVED:
-            return self.text
+            return self._result_text
         elif self.error is not None:
             raise self.error
         else:
             raise Exception("Rejected but no error captured!")
 
     def is_done(self):
         """
```

### Comparing `hugchat-0.4.6/src/hugchat/types/message.py` & `hugchat-0.4.7/src/hugchat/types/message.py`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.6/src/hugchat/types/model.py` & `hugchat-0.4.7/src/hugchat/types/model.py`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.6/src/hugchat.egg-info/PKG-INFO` & `hugchat-0.4.7/src/hugchat.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.4.6
+Version: 0.4.7
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -142,26 +142,27 @@
 - `-p` : Force request password to login, ignores saved cookies.
 - `-s` : Enable streaming mode output in CLI.
 - `-c` : Continue previous conversation in CLI ".
 
 Commands in cli mode:
 
 - `/new` : Create and switch to a new conversation.
-- `/ids` : Shows a list of all ID numbers and ID strings in current session.
-- `/switch <id>` : Switches to the ID number or ID string passed.
-- `/del <id>` : Deletes the ID number or ID string passed. Will not delete active session.
+- `/ids` : Shows a list of all ID numbers and ID strings in *current session*.
+- `/switch` : Shows a list of all conversations' info in *current session*. Then you can choose one to switch to.
+- `/switch all` : Shows a list of all conversations' info in *your account*. Then you can choose one to switch to. (not recommended if your account has a lot of conversations)
+- `/del <index>` : Deletes the conversation linked with the index passed. Will not delete active session.
 - `/delete-all` : Deletes all the conversations for the logged in user.
 - `/clear` : Clear the terminal.
 - `/llm` : Get available models you can switch to.
 - `/llm <index>` : Switches model to given model index based on `/llm`.
-- `/sharewithauthor <on|off>` : Changes settings for sharing data with model author. On by default.
+- `/share` : Toggles settings for sharing data with model author. On by default.
 - `/exit` : Closes CLI environment.
-- `/stream <on|off>`: streaming the response.
-- `/web <on|off>`: web search.
-- `/web-hint <on|off>`: display web search hint.
+- `/stream` : Toggles streaming the response.
+- `/web` : Toggles web search.
+- `/web-hint` : Toggles display web search hint.
 
 - AI is an area of active research with known problems such as biased generation and misinformation. Do not use this application for high-stakes decisions or advice.
 - Server resources are precious, it is not recommended to request this API in a high frequency.
 (`Hugging Face's CTO🤗` just liked the suggestion)
 <div align="center"><img width=500 src="https://github.com/Soulter/hugging-chat-api/assets/37870767/06e64501-02fb-4d4a-ab6f-cf18d8638ace"></img></div>
```

