# Comparing `tmp/lama2923-1.0.8.tar.gz` & `tmp/lama2923-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lama2923-1.0.8.tar", last modified: Wed May 22 00:56:19 2024, max compression
+gzip compressed data, was "lama2923-1.1.2.tar", last modified: Fri May 31 11:19:59 2024, max compression
```

## Comparing `lama2923-1.0.8.tar` & `lama2923-1.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 00:56:19.079795 lama2923-1.0.8/
--rw-rw-rw-   0        0        0      962 2024-05-22 00:56:19.078781 lama2923-1.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-22 00:56:19.064927 lama2923-1.0.8/lama2923/
--rw-rw-rw-   0        0        0    22715 2024-05-22 00:55:26.000000 lama2923-1.0.8/lama2923/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 00:56:19.075757 lama2923-1.0.8/lama2923.egg-info/
--rw-rw-rw-   0        0        0      962 2024-05-22 00:56:18.000000 lama2923-1.0.8/lama2923.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-05-22 00:56:18.000000 lama2923-1.0.8/lama2923.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 00:56:18.000000 lama2923-1.0.8/lama2923.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-22 00:56:18.000000 lama2923-1.0.8/lama2923.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-22 00:56:18.000000 lama2923-1.0.8/lama2923.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 00:56:19.079795 lama2923-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1300 2024-05-22 00:56:02.000000 lama2923-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:19:59.229035 lama2923-1.1.2/
+-rw-rw-rw-   0        0        0      962 2024-05-31 11:19:59.227960 lama2923-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-31 11:19:59.203961 lama2923-1.1.2/lama2923/
+-rw-rw-rw-   0        0        0    24301 2024-05-31 11:19:09.000000 lama2923-1.1.2/lama2923/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:19:59.224969 lama2923-1.1.2/lama2923.egg-info/
+-rw-rw-rw-   0        0        0      962 2024-05-31 11:19:58.000000 lama2923-1.1.2/lama2923.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-05-31 11:19:59.000000 lama2923-1.1.2/lama2923.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 11:19:58.000000 lama2923-1.1.2/lama2923.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-31 11:19:58.000000 lama2923-1.1.2/lama2923.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-31 11:19:58.000000 lama2923-1.1.2/lama2923.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 11:19:59.229035 lama2923-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1300 2024-05-31 11:19:49.000000 lama2923-1.1.2/setup.py
```

### Comparing `lama2923-1.0.8/PKG-INFO` & `lama2923-1.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lama2923
-Version: 1.0.8
+Version: 1.1.2
 Summary: Sikimsonik bir kütüphane
 Author: lama2923
 Author-email: lama2923.v2@gmail.com
 Keywords: example project setuptools development discord lama2923
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lama2923-1.0.8/lama2923/__init__.py` & `lama2923-1.1.2/lama2923/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import time
 import socket
 from colorama import Fore, Style, init
 import requests
 
 if os.name == 'nt':
     import msvcrt
+import requests
 
 def ekran_temizle():
     if os.name == 'posix':
         os.system('clear')
     elif os.name == 'nt':
         os.system('cls')
     else:
@@ -182,35 +183,53 @@
     if not isinstance(Numbers, str):
         raise TypeError("Value must be a string.")
     return Numbers.replace(".", "").replace(",", ".")
 
 class TokenIsNotWork(Exception):
     pass
 
+
+
+
+
+
 class Discord:
     class User:
         def __init__(self, token):
             self.token = str(token)
             response = requests.get('https://discord.com/api/v9/users/@me', headers={'Authorization': self.token})
             if response.status_code != 200:
                 raise TokenIsNotWork('Token is not working!')
-
+            
         def send_message(self, Channel_id, Message, files=None):
             payload = {'content': str(Message)}
             headers = {'Authorization': self.token}
             if files is not None and isinstance(files, list):
                 files_data = {
                     os.path.basename(file_name): open(file_name, "rb").read()
                     for file_name in files if os.path.getsize(file_name) > 0
                 }
                 response = requests.post(f'https://discord.com/api/v9/channels/{Channel_id}/messages', data=payload, files=files_data, headers=headers)
             else:
                 response = requests.post(f'https://discord.com/api/v9/channels/{Channel_id}/messages', data=payload, headers=headers)
             return response.status_code
-        
+
+        def send_reply_message(self, Channel_id, Message, ReplyMessage_id, files=None):
+            payload = {'content': str(Message), 'message_reference': {'message_id': ReplyMessage_id}}
+            headers = {'Authorization': self.token}
+            if files is not None and isinstance(files, list):
+                files_data = {
+                    os.path.basename(file_name): open(file_name, "rb").read()
+                    for file_name in files if os.path.getsize(file_name) > 0
+                }
+                response = requests.post(f'https://discord.com/api/v9/channels/{Channel_id}/messages', data=payload, files=files_data, headers=headers)
+            else:
+                response = requests.post(f'https://discord.com/api/v9/channels/{Channel_id}/messages', data=payload, headers=headers)
+            return response.status_code
+ 
         def delete_message(self, Channel_id, Message_id):
             headers = {'Authorization': self.token}
             response = requests.delete(f'https://discord.com/api/v9/channels/{Channel_id}/messages/{Message_id}', headers=headers)
             return response.status_code
         
         def edit_message(self, Channel_id, Message_id, Message_Content):
             headers = {'Authorization': self.token}
@@ -246,19 +265,14 @@
             return response.status_code, response.json() if response.status_code == 200 else response.status_code
     
         def get_guild_dms(self, Guild_id):
             headers = {'Authorization': self.token}
             response = requests.get(f'https://discord.com/api/v9/guilds/{Guild_id}/channels', headers=headers)
             return response.status_code, response.json() if response.status_code == 200 else response.status_code   
 
-        def send_reply_message(self, Channel_id, Message, ReplyMessage_id):
-            payload = {'content': str(Message), 'message_reference': {'message_id': ReplyMessage_id}}
-            headers = {'Authorization': self.token}
-            response = requests.post(f'https://discord.com/api/v9/channels/{Channel_id}/messages', data=payload, headers=headers)
-            return response.status_code
         
         def change_user_nickname(self, Guild_id, Nickname):
             headers = {'Authorization': self.token}
             payload = {'nick': str(Nickname)}
             response = requests.patch(f'https://discord.com/api/v9/guilds/{Guild_id}/members/@me/nick', json=payload, headers=headers)
             return response.status_code
 
@@ -363,14 +377,37 @@
             response = requests.get(f'https://discord.com/api/v9/guilds/{Guild_id}/roles', headers=headers)
             return response.status_code, response.json() if response.status_code == 200 else response.status_code
             
         def get_user_connections(self, id):
             headers = {'Authorization': self.token}
             response = requests.get(f'https://discord.com/api/v9/users/{id}/connections', headers=headers)
             return response.status_code, response.json() if response.status_code == 200 else response.status_code
+        
+        def join_channel(self, Channel_id):
+            headers = {'Authorization': self.token}
+            response = requests.put(f'https://discord.com/api/v9/channels/{Channel_id}/call/join', headers=headers)
+            return response.status_code
+
+        def leave_channel(self, Channel_id):
+            headers = {'Authorization': self.token}
+            response = requests.delete(f'https://discord.com/api/v9/channels/{Channel_id}/call', headers=headers)
+            return response.status_code
+
+        
+        
+        def get_channel_call(self, Channel_id):
+            headers = {'Authorization': self.token}
+            response = requests.get(f'https://discord.com/api/v9/channels/{Channel_id}/call', headers=headers)
+            return response.status_code, response.json() if response.status_code == 200 else response.status_code
+        
+        def play_sound(self, Channel_id, Sound):
+            headers = {'Authorization': self.token}
+            payload = {'audio': str(Sound)}
+            response = requests.post(f'https://discord.com/api/v9/channels/{Channel_id}/call/ring', json=payload, headers=headers)
+            return response.status_code
 
         def create_guild(self, Guild_name, Region='europe', Verification_level=0, Default_message_notifications=0, Explicit_content_filter=0, Roles=None, Channels=None):
             headers = {'Authorization': self.token}
             payload = {
                 'name': str(Guild_name),
                 'region': str(Region),
                 'verification_level': int(Verification_level),
@@ -388,28 +425,28 @@
             headers = {'Authorization': self.token}
             response = requests.delete(f'https://discord.com/api/v9/guilds/{Guild_id}', headers=headers)
             return response.status_code
 
        
 
         def edit_guild(self, Guild_id, Guild_name, Region='europe', Verification_level=0, Default_message_notifications=0, Explicit_content_filter=0, Roles=None, Channels=None):
-                    headers = {'Authorization': self.token}
-                    payload = {
-                        'name': str(Guild_name),
-                        'region': str(Region),
-                        'verification_level': int(Verification_level),
-                        'default_message_notifications': int(Default_message_notifications),
-                        'explicit_content_filter': int(Explicit_content_filter)
-                    }
-                    if Roles is not None and isinstance(Roles, list):
-                        payload['roles'] = Roles
-                    if Channels is not None and isinstance(Channels, list):
-                        payload['channels'] = Channels
-                    response = requests.patch(f'https://discord.com/api/v9/guilds/{Guild_id}', json=payload, headers=headers)
-                    return response.status_code
+            headers = {'Authorization': self.token}
+            payload = {
+                'name': str(Guild_name),
+                'region': str(Region),
+                'verification_level': int(Verification_level),
+                'default_message_notifications': int(Default_message_notifications),
+                'explicit_content_filter': int(Explicit_content_filter)
+            }
+            if Roles is not None and isinstance(Roles, list):
+                payload['roles'] = Roles
+            if Channels is not None and isinstance(Channels, list):
+                payload['channels'] = Channels
+            response = requests.patch(f'https://discord.com/api/v9/guilds/{Guild_id}', json=payload, headers=headers)
+            return response.status_code
         
         def create_guild_role(self, Guild_id, Role_name):
             headers = {'Authorization': self.token}
             payload = {'name': str(Role_name)}
             response = requests.post(f'https://discord.com/api/v9/guilds/{Guild_id}/roles', json=payload, headers=headers)
             return response.status_code
```

### Comparing `lama2923-1.0.8/lama2923.egg-info/PKG-INFO` & `lama2923-1.1.2/lama2923.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lama2923
-Version: 1.0.8
+Version: 1.1.2
 Summary: Sikimsonik bir kütüphane
 Author: lama2923
 Author-email: lama2923.v2@gmail.com
 Keywords: example project setuptools development discord lama2923
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lama2923-1.0.8/setup.py` & `lama2923-1.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Komutlar.txt dosyasından komutlar ile terminalde setup dosyasını çalıştırım upload edebilirsin.
 
 setup(
     name='lama2923',
-    version='1.0.8',
+    version='1.1.2',
     description='Sikimsonik bir kütüphane',
     long_description="Discord Api ile işlemler, Webhook ile işlemler, lprint, linput gibi güzel görünümlü yazılar... kısacası projenizde kullanabilceğiniz tasarım olarak ve Api işlemleri için kullanabilceğiniz bir kütüphane, ayrıca bu kütüphanenin ana dili Türkçe.",
     author='lama2923',
     author_email='lama2923.v2@gmail.com',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
```

