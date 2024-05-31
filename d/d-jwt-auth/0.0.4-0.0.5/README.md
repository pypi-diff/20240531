# Comparing `tmp/d_jwt_auth-0.0.4.tar.gz` & `tmp/d_jwt_auth-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d_jwt_auth-0.0.4.tar", last modified: Sun May  5 20:27:11 2024, max compression
+gzip compressed data, was "d_jwt_auth-0.0.5.tar", last modified: Fri May 31 20:56:39 2024, max compression
```

## Comparing `d_jwt_auth-0.0.4.tar` & `d_jwt_auth-0.0.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-05 20:27:11.558348 d_jwt_auth-0.0.4/
--rw-rw-r--   0 ali       (1000) ali       (1000)     1069 2024-04-19 07:51:05.000000 d_jwt_auth-0.0.4/LICENSE
--rw-rw-r--   0 ali       (1000) ali       (1000)    11696 2024-05-05 20:27:11.558348 d_jwt_auth-0.0.4/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)    10360 2024-05-01 04:36:53.000000 d_jwt_auth-0.0.4/README.md
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-05 20:27:11.554347 d_jwt_auth-0.0.4/config/
--rw-rw-r--   0 ali       (1000) ali       (1000)        0 2024-04-19 18:54:17.000000 d_jwt_auth-0.0.4/config/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      389 2024-04-19 18:54:17.000000 d_jwt_auth-0.0.4/config/asgi.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3970 2024-05-05 20:16:02.000000 d_jwt_auth-0.0.4/config/settings.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      762 2024-04-19 18:54:17.000000 d_jwt_auth-0.0.4/config/urls.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      389 2024-04-19 18:54:17.000000 d_jwt_auth-0.0.4/config/wsgi.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-05 20:27:11.558348 d_jwt_auth-0.0.4/d_jwt_auth/
--rw-rw-r--   0 ali       (1000) ali       (1000)        0 2024-04-19 18:34:36.000000 d_jwt_auth-0.0.4/d_jwt_auth/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      144 2024-04-19 03:20:09.000000 d_jwt_auth-0.0.4/d_jwt_auth/admin.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     2024 2024-05-01 02:17:28.000000 d_jwt_auth-0.0.4/d_jwt_auth/app_settings.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      150 2024-04-19 18:21:44.000000 d_jwt_auth-0.0.4/d_jwt_auth/apps.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1594 2024-04-19 05:10:17.000000 d_jwt_auth-0.0.4/d_jwt_auth/authenticate.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      560 2024-04-18 01:51:55.000000 d_jwt_auth-0.0.4/d_jwt_auth/cache.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      803 2024-04-18 03:51:03.000000 d_jwt_auth-0.0.4/d_jwt_auth/client.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      183 2024-05-01 04:29:12.000000 d_jwt_auth-0.0.4/d_jwt_auth/constants.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1225 2024-04-18 15:23:34.000000 d_jwt_auth-0.0.4/d_jwt_auth/encryption.py
--rw-rw-r--   0 ali       (1000) ali       (1000)       84 2024-04-18 03:06:06.000000 d_jwt_auth-0.0.4/d_jwt_auth/exceptions.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-05 20:27:11.558348 d_jwt_auth-0.0.4/d_jwt_auth/migrations/
--rw-rw-r--   0 ali       (1000) ali       (1000)     1048 2024-05-05 20:19:29.000000 d_jwt_auth-0.0.4/d_jwt_auth/migrations/0001_initial.py
--rw-rw-r--   0 ali       (1000) ali       (1000)        0 2023-11-27 10:37:30.000000 d_jwt_auth-0.0.4/d_jwt_auth/migrations/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      970 2024-05-01 02:29:31.000000 d_jwt_auth-0.0.4/d_jwt_auth/models.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     2919 2024-05-01 04:11:40.000000 d_jwt_auth-0.0.4/d_jwt_auth/services.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     6441 2024-05-05 20:03:09.000000 d_jwt_auth-0.0.4/d_jwt_auth/token.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-05 20:27:11.558348 d_jwt_auth-0.0.4/d_jwt_auth.egg-info/
--rw-rw-r--   0 ali       (1000) ali       (1000)    11696 2024-05-05 20:27:11.000000 d_jwt_auth-0.0.4/d_jwt_auth.egg-info/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)      835 2024-05-05 20:27:11.000000 d_jwt_auth-0.0.4/d_jwt_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)        1 2024-05-05 20:27:11.000000 d_jwt_auth-0.0.4/d_jwt_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)        1 2024-05-05 20:27:11.000000 d_jwt_auth-0.0.4/d_jwt_auth.egg-info/not-zip-safe
--rw-rw-r--   0 ali       (1000) ali       (1000)       92 2024-05-05 20:27:11.000000 d_jwt_auth-0.0.4/d_jwt_auth.egg-info/requires.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       18 2024-05-05 20:27:11.000000 d_jwt_auth-0.0.4/d_jwt_auth.egg-info/top_level.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       38 2024-05-05 20:27:11.558348 d_jwt_auth-0.0.4/setup.cfg
--rw-rw-r--   0 ali       (1000) ali       (1000)     1835 2024-05-05 20:24:25.000000 d_jwt_auth-0.0.4/setup.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-05 20:27:11.558348 d_jwt_auth-0.0.4/tests/
--rw-rw-r--   0 ali       (1000) ali       (1000)     2650 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.4/tests/test_app_settings.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1239 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.4/tests/test_cache.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     6909 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.4/tests/test_client.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1439 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.4/tests/test_encryption.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      811 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.4/tests/test_models.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     6823 2024-05-01 02:59:28.000000 d_jwt_auth-0.0.4/tests/test_services.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    12791 2024-05-01 04:30:31.000000 d_jwt_auth-0.0.4/tests/test_token.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-31 20:56:39.340093 d_jwt_auth-0.0.5/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1069 2024-04-19 07:51:05.000000 d_jwt_auth-0.0.5/LICENSE
+-rw-rw-r--   0 ali       (1000) ali       (1000)    11696 2024-05-31 20:56:39.340093 d_jwt_auth-0.0.5/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)    10360 2024-05-01 04:36:53.000000 d_jwt_auth-0.0.5/README.md
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-31 20:56:39.163969 d_jwt_auth-0.0.5/config/
+-rw-rw-r--   0 ali       (1000) ali       (1000)        0 2024-04-19 18:54:17.000000 d_jwt_auth-0.0.5/config/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      389 2024-04-19 18:54:17.000000 d_jwt_auth-0.0.5/config/asgi.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3970 2024-05-05 20:16:02.000000 d_jwt_auth-0.0.5/config/settings.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      762 2024-04-19 18:54:17.000000 d_jwt_auth-0.0.5/config/urls.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      389 2024-04-19 18:54:17.000000 d_jwt_auth-0.0.5/config/wsgi.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-31 20:56:39.292059 d_jwt_auth-0.0.5/d_jwt_auth/
+-rw-rw-r--   0 ali       (1000) ali       (1000)        0 2024-04-19 18:34:36.000000 d_jwt_auth-0.0.5/d_jwt_auth/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      144 2024-04-19 03:20:09.000000 d_jwt_auth-0.0.5/d_jwt_auth/admin.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     2024 2024-05-01 02:17:28.000000 d_jwt_auth-0.0.5/d_jwt_auth/app_settings.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      150 2024-04-19 18:21:44.000000 d_jwt_auth-0.0.5/d_jwt_auth/apps.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1594 2024-04-19 05:10:17.000000 d_jwt_auth-0.0.5/d_jwt_auth/authenticate.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      560 2024-04-18 01:51:55.000000 d_jwt_auth-0.0.5/d_jwt_auth/cache.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      803 2024-04-18 03:51:03.000000 d_jwt_auth-0.0.5/d_jwt_auth/client.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      183 2024-05-01 04:29:12.000000 d_jwt_auth-0.0.5/d_jwt_auth/constants.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1225 2024-04-18 15:23:34.000000 d_jwt_auth-0.0.5/d_jwt_auth/encryption.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)       84 2024-04-18 03:06:06.000000 d_jwt_auth-0.0.5/d_jwt_auth/exceptions.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-31 20:56:39.304068 d_jwt_auth-0.0.5/d_jwt_auth/migrations/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1048 2024-05-05 20:19:29.000000 d_jwt_auth-0.0.5/d_jwt_auth/migrations/0001_initial.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)        0 2023-11-27 10:37:30.000000 d_jwt_auth-0.0.5/d_jwt_auth/migrations/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      970 2024-05-01 02:29:31.000000 d_jwt_auth-0.0.5/d_jwt_auth/models.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     2919 2024-05-01 04:11:40.000000 d_jwt_auth-0.0.5/d_jwt_auth/services.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     6446 2024-05-31 20:47:55.000000 d_jwt_auth-0.0.5/d_jwt_auth/token.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-31 20:56:39.296062 d_jwt_auth-0.0.5/d_jwt_auth.egg-info/
+-rw-rw-r--   0 ali       (1000) ali       (1000)    11696 2024-05-31 20:56:38.000000 d_jwt_auth-0.0.5/d_jwt_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)      835 2024-05-31 20:56:38.000000 d_jwt_auth-0.0.5/d_jwt_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)        1 2024-05-31 20:56:38.000000 d_jwt_auth-0.0.5/d_jwt_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)        1 2024-05-31 20:56:38.000000 d_jwt_auth-0.0.5/d_jwt_auth.egg-info/not-zip-safe
+-rw-rw-r--   0 ali       (1000) ali       (1000)       92 2024-05-31 20:56:38.000000 d_jwt_auth-0.0.5/d_jwt_auth.egg-info/requires.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       18 2024-05-31 20:56:38.000000 d_jwt_auth-0.0.5/d_jwt_auth.egg-info/top_level.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       38 2024-05-31 20:56:39.344096 d_jwt_auth-0.0.5/setup.cfg
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1835 2024-05-31 20:49:34.000000 d_jwt_auth-0.0.5/setup.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-31 20:56:39.336090 d_jwt_auth-0.0.5/tests/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     2650 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.5/tests/test_app_settings.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1239 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.5/tests/test_cache.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     6909 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.5/tests/test_client.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1439 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.5/tests/test_encryption.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      811 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.5/tests/test_models.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     6823 2024-05-01 02:59:28.000000 d_jwt_auth-0.0.5/tests/test_services.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    12791 2024-05-01 04:30:31.000000 d_jwt_auth-0.0.5/tests/test_token.py
```

### Comparing `d_jwt_auth-0.0.4/LICENSE` & `d_jwt_auth-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.4/PKG-INFO` & `d_jwt_auth-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d_jwt_auth
-Version: 0.0.4
+Version: 0.0.5
 Summary: django-jwt-auth is an application for authenticating users with jwt in Django.
 Home-page: https://github.com/alireza-fa/django-jwt-auth
 Author: Alireza Feizi
 Author-email: alirezafeyze44@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/alireza-fa/django-jwt-auth
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `d_jwt_auth-0.0.4/README.md` & `d_jwt_auth-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.4/config/settings.py` & `d_jwt_auth-0.0.5/config/settings.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.4/config/urls.py` & `d_jwt_auth-0.0.5/config/urls.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.4/d_jwt_auth/app_settings.py` & `d_jwt_auth-0.0.5/d_jwt_auth/app_settings.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.4/d_jwt_auth/authenticate.py` & `d_jwt_auth-0.0.5/d_jwt_auth/authenticate.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.4/d_jwt_auth/cache.py` & `d_jwt_auth-0.0.5/d_jwt_auth/cache.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.4/d_jwt_auth/client.py` & `d_jwt_auth-0.0.5/d_jwt_auth/client.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.4/d_jwt_auth/encryption.py` & `d_jwt_auth-0.0.5/d_jwt_auth/encryption.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.4/d_jwt_auth/migrations/0001_initial.py` & `d_jwt_auth-0.0.5/d_jwt_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.4/d_jwt_auth/models.py` & `d_jwt_auth-0.0.5/d_jwt_auth/models.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.4/d_jwt_auth/services.py` & `d_jwt_auth-0.0.5/d_jwt_auth/services.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.4/d_jwt_auth/token.py` & `d_jwt_auth-0.0.5/d_jwt_auth/token.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,18 @@
 
 def set_token_claims(*, token: Token, claims: Dict, **kwargs):
     for key in claims:
         claims[key] = kwargs[key]
 
     for key, value in claims.items():
         if isinstance(value, File):
-            token[key] = value.url
-        elif isinstance(value, File):
-            token[key] = value.url
+            if value:
+                token[key] = value.url
+            else:
+                token[key] = None
         elif isinstance(value, datetime):
             token[key] = str(value)
         else:
             token[key] = value
 
 
 def get_token_claims(*, token: Token, claims: Dict):
```

### Comparing `d_jwt_auth-0.0.4/d_jwt_auth.egg-info/PKG-INFO` & `d_jwt_auth-0.0.5/d_jwt_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d-jwt-auth
-Version: 0.0.4
+Version: 0.0.5
 Summary: django-jwt-auth is an application for authenticating users with jwt in Django.
 Home-page: https://github.com/alireza-fa/django-jwt-auth
 Author: Alireza Feizi
 Author-email: alirezafeyze44@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/alireza-fa/django-jwt-auth
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `d_jwt_auth-0.0.4/d_jwt_auth.egg-info/SOURCES.txt` & `d_jwt_auth-0.0.5/d_jwt_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.4/setup.py` & `d_jwt_auth-0.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read(f):
     with open(f, 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name='d_jwt_auth',
-    version="0.0.4",
+    version="0.0.5",
     url='https://github.com/alireza-fa/django-jwt-auth',
     license='MIT',
     description='django-jwt-auth is an application for authenticating users with jwt in Django.',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     author='Alireza Feizi',
     author_email='alirezafeyze44@gmail.com',
```

### Comparing `d_jwt_auth-0.0.4/tests/test_app_settings.py` & `d_jwt_auth-0.0.5/tests/test_app_settings.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.4/tests/test_cache.py` & `d_jwt_auth-0.0.5/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.4/tests/test_client.py` & `d_jwt_auth-0.0.5/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.4/tests/test_encryption.py` & `d_jwt_auth-0.0.5/tests/test_encryption.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.4/tests/test_models.py` & `d_jwt_auth-0.0.5/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.4/tests/test_services.py` & `d_jwt_auth-0.0.5/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.4/tests/test_token.py` & `d_jwt_auth-0.0.5/tests/test_token.py`

 * *Files identical despite different names*

