# Comparing `tmp/sentry-auth-gitlab-v2-0.3.1.tar.gz` & `tmp/sentry-auth-gitlab-v2-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry-auth-gitlab-v2-0.3.1.tar", last modified: Tue Sep 19 09:28:39 2023, max compression
+gzip compressed data, was "sentry-auth-gitlab-v2-0.4.0.tar", last modified: Fri May 31 14:12:15 2024, max compression
```

## Comparing `sentry-auth-gitlab-v2-0.3.1.tar` & `sentry-auth-gitlab-v2-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,28 @@
-drwxr-xr-x   0 zekker    (1000) zekker    (1000)        0 2023-09-19 09:28:39.915498 sentry-auth-gitlab-v2-0.3.1/
--rw-r--r--   0 zekker    (1000) zekker    (1000)    10848 2023-09-08 11:18:00.000000 sentry-auth-gitlab-v2-0.3.1/LICENSE
--rw-r--r--   0 zekker    (1000) zekker    (1000)       66 2023-09-08 11:18:00.000000 sentry-auth-gitlab-v2-0.3.1/MANIFEST.in
--rw-r--r--   0 zekker    (1000) zekker    (1000)     3516 2023-09-19 09:28:39.915498 sentry-auth-gitlab-v2-0.3.1/PKG-INFO
--rw-r--r--   0 zekker    (1000) zekker    (1000)     3014 2023-09-08 11:18:00.000000 sentry-auth-gitlab-v2-0.3.1/README.rst
-drwxr-xr-x   0 zekker    (1000) zekker    (1000)        0 2023-09-19 09:28:39.915498 sentry-auth-gitlab-v2-0.3.1/auth_gitlab/
--rw-r--r--   0 zekker    (1000) zekker    (1000)      165 2023-09-08 11:18:00.000000 sentry-auth-gitlab-v2-0.3.1/auth_gitlab/__init__.py
--rw-r--r--   0 zekker    (1000) zekker    (1000)      288 2023-09-08 11:18:00.000000 sentry-auth-gitlab-v2-0.3.1/auth_gitlab/apps.py
--rw-r--r--   0 zekker    (1000) zekker    (1000)      890 2023-09-08 11:18:00.000000 sentry-auth-gitlab-v2-0.3.1/auth_gitlab/client.py
--rw-r--r--   0 zekker    (1000) zekker    (1000)      655 2023-09-08 11:18:00.000000 sentry-auth-gitlab-v2-0.3.1/auth_gitlab/constants.py
--rw-r--r--   0 zekker    (1000) zekker    (1000)     1168 2023-09-19 09:25:25.000000 sentry-auth-gitlab-v2-0.3.1/auth_gitlab/provider.py
--rw-r--r--   0 zekker    (1000) zekker    (1000)      373 2023-09-08 11:18:00.000000 sentry-auth-gitlab-v2-0.3.1/auth_gitlab/views.py
-drwxr-xr-x   0 zekker    (1000) zekker    (1000)        0 2023-09-19 09:28:39.915498 sentry-auth-gitlab-v2-0.3.1/sentry_auth_gitlab_v2.egg-info/
--rw-r--r--   0 zekker    (1000) zekker    (1000)     3516 2023-09-19 09:28:39.000000 sentry-auth-gitlab-v2-0.3.1/sentry_auth_gitlab_v2.egg-info/PKG-INFO
--rw-r--r--   0 zekker    (1000) zekker    (1000)      501 2023-09-19 09:28:39.000000 sentry-auth-gitlab-v2-0.3.1/sentry_auth_gitlab_v2.egg-info/SOURCES.txt
--rw-r--r--   0 zekker    (1000) zekker    (1000)        1 2023-09-19 09:28:39.000000 sentry-auth-gitlab-v2-0.3.1/sentry_auth_gitlab_v2.egg-info/dependency_links.txt
--rw-r--r--   0 zekker    (1000) zekker    (1000)       52 2023-09-19 09:28:39.000000 sentry-auth-gitlab-v2-0.3.1/sentry_auth_gitlab_v2.egg-info/entry_points.txt
--rw-r--r--   0 zekker    (1000) zekker    (1000)        1 2023-09-19 09:28:39.000000 sentry-auth-gitlab-v2-0.3.1/sentry_auth_gitlab_v2.egg-info/not-zip-safe
--rw-r--r--   0 zekker    (1000) zekker    (1000)       28 2023-09-19 09:28:39.000000 sentry-auth-gitlab-v2-0.3.1/sentry_auth_gitlab_v2.egg-info/requires.txt
--rw-r--r--   0 zekker    (1000) zekker    (1000)       12 2023-09-19 09:28:39.000000 sentry-auth-gitlab-v2-0.3.1/sentry_auth_gitlab_v2.egg-info/top_level.txt
--rw-r--r--   0 zekker    (1000) zekker    (1000)      320 2023-09-19 09:28:39.915498 sentry-auth-gitlab-v2-0.3.1/setup.cfg
--rw-r--r--   0 zekker    (1000) zekker    (1000)     1368 2023-09-19 09:28:12.000000 sentry-auth-gitlab-v2-0.3.1/setup.py
+drwxr-xr-x   0 zekker    (1000) zekker    (1000)        0 2024-05-31 14:12:15.679017 sentry-auth-gitlab-v2-0.4.0/
+-rw-r--r--   0 zekker    (1000) zekker    (1000)       76 2023-09-19 09:26:38.000000 sentry-auth-gitlab-v2-0.4.0/.gitignore
+-rw-r--r--   0 zekker    (1000) zekker    (1000)       22 2023-09-08 11:18:00.000000 sentry-auth-gitlab-v2-0.4.0/.python-version
+-rw-r--r--   0 zekker    (1000) zekker    (1000)      387 2023-09-08 11:18:00.000000 sentry-auth-gitlab-v2-0.4.0/.travis.yml
+-rw-r--r--   0 zekker    (1000) zekker    (1000)    10848 2023-09-08 11:18:00.000000 sentry-auth-gitlab-v2-0.4.0/LICENSE
+-rw-r--r--   0 zekker    (1000) zekker    (1000)       66 2023-09-08 11:18:00.000000 sentry-auth-gitlab-v2-0.4.0/MANIFEST.in
+-rw-r--r--   0 zekker    (1000) zekker    (1000)      204 2023-09-19 09:26:04.000000 sentry-auth-gitlab-v2-0.4.0/Makefile
+-rw-r--r--   0 zekker    (1000) zekker    (1000)     3616 2024-05-31 14:12:15.679017 sentry-auth-gitlab-v2-0.4.0/PKG-INFO
+-rw-r--r--   0 zekker    (1000) zekker    (1000)     3014 2023-09-08 11:18:00.000000 sentry-auth-gitlab-v2-0.4.0/README.rst
+drwxr-xr-x   0 zekker    (1000) zekker    (1000)        0 2024-05-31 14:12:15.678017 sentry-auth-gitlab-v2-0.4.0/auth_gitlab/
+-rw-r--r--   0 zekker    (1000) zekker    (1000)        0 2024-05-31 14:06:55.000000 sentry-auth-gitlab-v2-0.4.0/auth_gitlab/__init__.py
+-rw-r--r--   0 zekker    (1000) zekker    (1000)      255 2024-05-31 14:08:42.000000 sentry-auth-gitlab-v2-0.4.0/auth_gitlab/apps.py
+-rw-r--r--   0 zekker    (1000) zekker    (1000)     1150 2024-05-31 14:07:41.000000 sentry-auth-gitlab-v2-0.4.0/auth_gitlab/client.py
+-rw-r--r--   0 zekker    (1000) zekker    (1000)      371 2024-05-31 14:07:55.000000 sentry-auth-gitlab-v2-0.4.0/auth_gitlab/constants.py
+-rw-r--r--   0 zekker    (1000) zekker    (1000)     1453 2024-05-31 14:08:01.000000 sentry-auth-gitlab-v2-0.4.0/auth_gitlab/provider.py
+-rw-r--r--   0 zekker    (1000) zekker    (1000)      339 2024-05-31 14:08:08.000000 sentry-auth-gitlab-v2-0.4.0/auth_gitlab/views.py
+-rw-r--r--   0 zekker    (1000) zekker    (1000)      175 2023-09-08 11:18:00.000000 sentry-auth-gitlab-v2-0.4.0/conftest.py
+-rw-r--r--   0 zekker    (1000) zekker    (1000)      123 2023-09-08 11:18:00.000000 sentry-auth-gitlab-v2-0.4.0/renovate.json
+drwxr-xr-x   0 zekker    (1000) zekker    (1000)        0 2024-05-31 14:12:15.679017 sentry-auth-gitlab-v2-0.4.0/sentry_auth_gitlab_v2.egg-info/
+-rw-r--r--   0 zekker    (1000) zekker    (1000)     3616 2024-05-31 14:12:15.000000 sentry-auth-gitlab-v2-0.4.0/sentry_auth_gitlab_v2.egg-info/PKG-INFO
+-rw-r--r--   0 zekker    (1000) zekker    (1000)      584 2024-05-31 14:12:15.000000 sentry-auth-gitlab-v2-0.4.0/sentry_auth_gitlab_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 zekker    (1000) zekker    (1000)        1 2024-05-31 14:12:15.000000 sentry-auth-gitlab-v2-0.4.0/sentry_auth_gitlab_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 zekker    (1000) zekker    (1000)       52 2024-05-31 14:12:15.000000 sentry-auth-gitlab-v2-0.4.0/sentry_auth_gitlab_v2.egg-info/entry_points.txt
+-rw-r--r--   0 zekker    (1000) zekker    (1000)        1 2023-09-19 09:28:39.000000 sentry-auth-gitlab-v2-0.4.0/sentry_auth_gitlab_v2.egg-info/not-zip-safe
+-rw-r--r--   0 zekker    (1000) zekker    (1000)       28 2024-05-31 14:12:15.000000 sentry-auth-gitlab-v2-0.4.0/sentry_auth_gitlab_v2.egg-info/requires.txt
+-rw-r--r--   0 zekker    (1000) zekker    (1000)       12 2024-05-31 14:12:15.000000 sentry-auth-gitlab-v2-0.4.0/sentry_auth_gitlab_v2.egg-info/top_level.txt
+-rw-r--r--   0 zekker    (1000) zekker    (1000)      320 2024-05-31 14:12:15.679017 sentry-auth-gitlab-v2-0.4.0/setup.cfg
+-rw-r--r--   0 zekker    (1000) zekker    (1000)     1368 2024-05-31 14:10:22.000000 sentry-auth-gitlab-v2-0.4.0/setup.py
```

### Comparing `sentry-auth-gitlab-v2-0.3.1/LICENSE` & `sentry-auth-gitlab-v2-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry-auth-gitlab-v2-0.3.1/PKG-INFO` & `sentry-auth-gitlab-v2-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: sentry-auth-gitlab-v2
-Version: 0.3.1
+Version: 0.4.0
 Summary: Gitlab authentication provider for Sentry
 Home-page: https://github.com/zekker6/sentry-auth-gitlab
 Author: Zakhar Bessarab
 Author-email: zekker6@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
-Provides-Extra: tests
 License-File: LICENSE
+Requires-Dist: sentry
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: mock; extra == "tests"
 
 
 .. image:: https://badge.fury.io/py/sentry-auth-gitlab-v2.svg
     :target: https://badge.fury.io/py/sentry-auth-gitlab-v2
 
 
 Disclaimer 1
```

### Comparing `sentry-auth-gitlab-v2-0.3.1/README.rst` & `sentry-auth-gitlab-v2-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `sentry-auth-gitlab-v2-0.3.1/auth_gitlab/provider.py` & `sentry-auth-gitlab-v2-0.4.0/auth_gitlab/provider.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,50 @@
-from __future__ import absolute_import
+from sentry.auth.exceptions import IdentityNotValid
+from sentry.auth.providers.oauth2 import OAuth2Callback, OAuth2Provider, OAuth2Login
 
-from sentry.auth.providers.oauth2 import (
-    OAuth2Callback, OAuth2Provider, OAuth2Login
-)
-
-from .constants import (
-    AUTHORIZE_URL, ACCESS_TOKEN_URL, CLIENT_ID, CLIENT_SECRET, SCOPE
-)
+from .constants import AUTHORIZE_URL, ACCESS_TOKEN_URL, CLIENT_ID, CLIENT_SECRET, SCOPE
 from .views import FetchUser
 
 
 class GitLabOAuth2Provider(OAuth2Provider):
+    access_token_url = ACCESS_TOKEN_URL
+    authorize_url = AUTHORIZE_URL
     name = 'Gitlab'
 
+    def get_client_id(self):
+        return CLIENT_ID
+
+    def get_client_secret(self):
+        return CLIENT_SECRET
+
     def get_auth_pipeline(self):
         return [
-            OAuth2Login(AUTHORIZE_URL, client_id=CLIENT_ID, scope=SCOPE),
+            OAuth2Login(
+                authorize_url=self.authorize_url, client_id=self.get_client_id(), scope=SCOPE
+            ),
             OAuth2Callback(
-                access_token_url=ACCESS_TOKEN_URL,
-                client_id=CLIENT_ID, client_secret=CLIENT_SECRET,
+                access_token_url=self.access_token_url,
+                client_id=self.get_client_id(),
+                client_secret=self.get_client_secret(),
             ),
             FetchUser()
         ]
 
+    def get_setup_pipeline(self):
+        pipeline = self.get_auth_pipeline()
+        return pipeline
+
     def get_refresh_token_url(self):
         return ACCESS_TOKEN_URL
 
-    def build_config(self, state):
+    def build_config(self, config):
         return {}
 
     def build_identity(self, state):
         data = state['data']
         user_data = state['user']
         return {
             'id': user_data['id'],
             'email': user_data['email'],
             'name': user_data['name'],
             'data': self.get_oauth_data(data),
         }
-
-    def get_client_id():
-        return CLIENT_ID
-
-    def get_client_secret():
-        return CLIENT_SECRET
```

### Comparing `sentry-auth-gitlab-v2-0.3.1/sentry_auth_gitlab_v2.egg-info/PKG-INFO` & `sentry-auth-gitlab-v2-0.4.0/sentry_auth_gitlab_v2.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: sentry-auth-gitlab-v2
-Version: 0.3.1
+Version: 0.4.0
 Summary: Gitlab authentication provider for Sentry
 Home-page: https://github.com/zekker6/sentry-auth-gitlab
 Author: Zakhar Bessarab
 Author-email: zekker6@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
-Provides-Extra: tests
 License-File: LICENSE
+Requires-Dist: sentry
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: mock; extra == "tests"
 
 
 .. image:: https://badge.fury.io/py/sentry-auth-gitlab-v2.svg
     :target: https://badge.fury.io/py/sentry-auth-gitlab-v2
 
 
 Disclaimer 1
```

### Comparing `sentry-auth-gitlab-v2-0.3.1/setup.py` & `sentry-auth-gitlab-v2-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 # The text of the README file
 with open(HERE + "/README.rst", 'r') as f:
     README = f.read()
 
 setup(
     name='sentry-auth-gitlab-v2',
-    version='0.3.1',
+    version='0.4.0',
     author='Zakhar Bessarab',
     author_email='zekker6@gmail.com',
     url='https://github.com/zekker6/sentry-auth-gitlab',
     description='Gitlab authentication provider for Sentry',
     long_description=README,
     long_description_content_type="text/markdown",
     license='',
```

