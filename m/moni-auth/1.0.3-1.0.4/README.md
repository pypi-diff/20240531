# Comparing `tmp/moni-auth-1.0.3.tar.gz` & `tmp/moni-auth-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moni-auth-1.0.3.tar", last modified: Tue Mar 12 13:35:43 2024, max compression
+gzip compressed data, was "moni-auth-1.0.4.tar", last modified: Fri May 31 17:48:08 2024, max compression
```

## Comparing `moni-auth-1.0.3.tar` & `moni-auth-1.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 imanol     (501) staff       (20)        0 2024-03-12 13:35:43.200041 moni-auth-1.0.3/
--rw-r--r--   0 imanol     (501) staff       (20)       18 2024-03-12 13:30:58.000000 moni-auth-1.0.3/MANIFEST.in
--rw-r--r--   0 imanol     (501) staff       (20)     2273 2024-03-12 13:35:43.200126 moni-auth-1.0.3/PKG-INFO
--rw-r--r--   0 imanol     (501) staff       (20)     1413 2024-03-12 13:30:58.000000 moni-auth-1.0.3/README.rst
-drwxr-xr-x   0 imanol     (501) staff       (20)        0 2024-03-12 13:35:43.199248 moni-auth-1.0.3/moni_auth/
--rw-r--r--   0 imanol     (501) staff       (20)        0 2024-03-12 13:30:58.000000 moni-auth-1.0.3/moni_auth/__init__.py
--rw-r--r--   0 imanol     (501) staff       (20)      217 2024-03-12 13:30:58.000000 moni-auth-1.0.3/moni_auth/apps.py
--rw-r--r--   0 imanol     (501) staff       (20)      799 2024-03-12 13:30:58.000000 moni-auth-1.0.3/moni_auth/authenticators.py
--rw-r--r--   0 imanol     (501) staff       (20)     1032 2024-03-12 13:30:58.000000 moni-auth-1.0.3/moni_auth/exceptions.py
--rw-r--r--   0 imanol     (501) staff       (20)     4147 2024-03-12 13:35:10.000000 moni-auth-1.0.3/moni_auth/mixins.py
--rw-r--r--   0 imanol     (501) staff       (20)      387 2024-03-12 13:30:58.000000 moni-auth-1.0.3/moni_auth/models.py
--rw-r--r--   0 imanol     (501) staff       (20)     1762 2024-03-12 13:30:58.000000 moni-auth-1.0.3/moni_auth/permissions.py
--rw-r--r--   0 imanol     (501) staff       (20)     1177 2024-03-12 13:30:58.000000 moni-auth-1.0.3/moni_auth/service.py
--rw-r--r--   0 imanol     (501) staff       (20)     2229 2024-03-12 13:30:58.000000 moni-auth-1.0.3/moni_auth/signals.py
--rw-r--r--   0 imanol     (501) staff       (20)     1474 2024-03-12 13:30:58.000000 moni-auth-1.0.3/moni_auth/tests.py
--rw-r--r--   0 imanol     (501) staff       (20)      443 2024-03-12 13:30:58.000000 moni-auth-1.0.3/moni_auth/urls.py
--rw-r--r--   0 imanol     (501) staff       (20)     2473 2024-03-12 13:30:58.000000 moni-auth-1.0.3/moni_auth/utils.py
--rw-r--r--   0 imanol     (501) staff       (20)     5086 2024-03-12 13:30:58.000000 moni-auth-1.0.3/moni_auth/views.py
-drwxr-xr-x   0 imanol     (501) staff       (20)        0 2024-03-12 13:35:43.199918 moni-auth-1.0.3/moni_auth.egg-info/
--rw-r--r--   0 imanol     (501) staff       (20)     2273 2024-03-12 13:35:43.000000 moni-auth-1.0.3/moni_auth.egg-info/PKG-INFO
--rw-r--r--   0 imanol     (501) staff       (20)      494 2024-03-12 13:35:43.000000 moni-auth-1.0.3/moni_auth.egg-info/SOURCES.txt
--rw-r--r--   0 imanol     (501) staff       (20)        1 2024-03-12 13:35:43.000000 moni-auth-1.0.3/moni_auth.egg-info/dependency_links.txt
--rw-r--r--   0 imanol     (501) staff       (20)       70 2024-03-12 13:35:43.000000 moni-auth-1.0.3/moni_auth.egg-info/requires.txt
--rw-r--r--   0 imanol     (501) staff       (20)       10 2024-03-12 13:35:43.000000 moni-auth-1.0.3/moni_auth.egg-info/top_level.txt
--rw-r--r--   0 imanol     (501) staff       (20)       88 2024-03-12 13:30:58.000000 moni-auth-1.0.3/pyproject.toml
--rw-r--r--   0 imanol     (501) staff       (20)      932 2024-03-12 13:35:43.200677 moni-auth-1.0.3/setup.cfg
--rw-r--r--   0 imanol     (501) staff       (20)       38 2024-03-12 13:30:58.000000 moni-auth-1.0.3/setup.py
+drwxr-xr-x   0 c.e.niebylski   (501) staff       (20)        0 2024-05-31 17:48:08.060983 moni-auth-1.0.4/
+-rw-r--r--   0 c.e.niebylski   (501) staff       (20)       18 2024-03-06 20:06:08.000000 moni-auth-1.0.4/MANIFEST.in
+-rw-r--r--   0 c.e.niebylski   (501) staff       (20)     2273 2024-05-31 17:48:08.061198 moni-auth-1.0.4/PKG-INFO
+-rw-r--r--   0 c.e.niebylski   (501) staff       (20)     1413 2024-03-06 20:06:08.000000 moni-auth-1.0.4/README.rst
+drwxr-xr-x   0 c.e.niebylski   (501) staff       (20)        0 2024-05-31 17:48:08.057602 moni-auth-1.0.4/moni_auth/
+-rw-r--r--   0 c.e.niebylski   (501) staff       (20)        0 2024-03-06 20:06:08.000000 moni-auth-1.0.4/moni_auth/__init__.py
+-rw-r--r--   0 c.e.niebylski   (501) staff       (20)      217 2024-03-06 20:06:08.000000 moni-auth-1.0.4/moni_auth/apps.py
+-rw-r--r--   0 c.e.niebylski   (501) staff       (20)      799 2024-03-06 20:06:08.000000 moni-auth-1.0.4/moni_auth/authenticators.py
+-rw-r--r--   0 c.e.niebylski   (501) staff       (20)     1032 2024-03-06 20:06:08.000000 moni-auth-1.0.4/moni_auth/exceptions.py
+-rw-r--r--   0 c.e.niebylski   (501) staff       (20)     4147 2024-05-30 17:38:35.000000 moni-auth-1.0.4/moni_auth/mixins.py
+-rw-r--r--   0 c.e.niebylski   (501) staff       (20)      387 2024-03-06 20:06:08.000000 moni-auth-1.0.4/moni_auth/models.py
+-rw-r--r--   0 c.e.niebylski   (501) staff       (20)     1762 2024-03-06 20:06:08.000000 moni-auth-1.0.4/moni_auth/permissions.py
+-rw-r--r--   0 c.e.niebylski   (501) staff       (20)     1177 2024-03-06 20:06:08.000000 moni-auth-1.0.4/moni_auth/service.py
+-rw-r--r--   0 c.e.niebylski   (501) staff       (20)     2229 2024-03-06 20:06:08.000000 moni-auth-1.0.4/moni_auth/signals.py
+-rw-r--r--   0 c.e.niebylski   (501) staff       (20)     1474 2024-03-06 20:06:08.000000 moni-auth-1.0.4/moni_auth/tests.py
+-rw-r--r--   0 c.e.niebylski   (501) staff       (20)      443 2024-03-06 20:06:08.000000 moni-auth-1.0.4/moni_auth/urls.py
+-rw-r--r--   0 c.e.niebylski   (501) staff       (20)     2470 2024-05-30 17:39:59.000000 moni-auth-1.0.4/moni_auth/utils.py
+-rw-r--r--   0 c.e.niebylski   (501) staff       (20)     5086 2024-03-06 20:06:08.000000 moni-auth-1.0.4/moni_auth/views.py
+drwxr-xr-x   0 c.e.niebylski   (501) staff       (20)        0 2024-05-31 17:48:08.060394 moni-auth-1.0.4/moni_auth.egg-info/
+-rw-r--r--   0 c.e.niebylski   (501) staff       (20)     2273 2024-05-31 17:48:07.000000 moni-auth-1.0.4/moni_auth.egg-info/PKG-INFO
+-rw-r--r--   0 c.e.niebylski   (501) staff       (20)      494 2024-05-31 17:48:08.000000 moni-auth-1.0.4/moni_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 c.e.niebylski   (501) staff       (20)        1 2024-05-31 17:48:07.000000 moni-auth-1.0.4/moni_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 c.e.niebylski   (501) staff       (20)       70 2024-05-31 17:48:07.000000 moni-auth-1.0.4/moni_auth.egg-info/requires.txt
+-rw-r--r--   0 c.e.niebylski   (501) staff       (20)       10 2024-05-31 17:48:07.000000 moni-auth-1.0.4/moni_auth.egg-info/top_level.txt
+-rw-r--r--   0 c.e.niebylski   (501) staff       (20)       88 2024-03-06 20:06:08.000000 moni-auth-1.0.4/pyproject.toml
+-rw-r--r--   0 c.e.niebylski   (501) staff       (20)      932 2024-05-31 17:48:08.062334 moni-auth-1.0.4/setup.cfg
+-rw-r--r--   0 c.e.niebylski   (501) staff       (20)       38 2024-03-06 20:06:08.000000 moni-auth-1.0.4/setup.py
```

### Comparing `moni-auth-1.0.3/PKG-INFO` & `moni-auth-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moni-auth
-Version: 1.0.3
+Version: 1.0.4
 Summary: Django app to integrate with the centralized Moni authentication system
 Home-page: https://www.example.com/
 Author: Lorenzo Fabro
 Author-email: lorenzo.fabro@moni.com.ar
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `moni-auth-1.0.3/README.rst` & `moni-auth-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `moni-auth-1.0.3/moni_auth/authenticators.py` & `moni-auth-1.0.4/moni_auth/authenticators.py`

 * *Files identical despite different names*

### Comparing `moni-auth-1.0.3/moni_auth/exceptions.py` & `moni-auth-1.0.4/moni_auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `moni-auth-1.0.3/moni_auth/mixins.py` & `moni-auth-1.0.4/moni_auth/mixins.py`

 * *Files identical despite different names*

### Comparing `moni-auth-1.0.3/moni_auth/permissions.py` & `moni-auth-1.0.4/moni_auth/permissions.py`

 * *Files identical despite different names*

### Comparing `moni-auth-1.0.3/moni_auth/service.py` & `moni-auth-1.0.4/moni_auth/service.py`

 * *Files identical despite different names*

### Comparing `moni-auth-1.0.3/moni_auth/signals.py` & `moni-auth-1.0.4/moni_auth/signals.py`

 * *Files identical despite different names*

### Comparing `moni-auth-1.0.3/moni_auth/tests.py` & `moni-auth-1.0.4/moni_auth/tests.py`

 * *Files identical despite different names*

### Comparing `moni-auth-1.0.3/moni_auth/utils.py` & `moni-auth-1.0.4/moni_auth/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         email (str): user email
 
     Returns:
         user: User object
     """
     User = get_user_model()
     try:
-        user = User.objects.get(username=email)
+        user = User.objects.get(email=email)
     except User.DoesNotExist:
         user = User.objects.create_user(email, email, generate_random_password())
         user.is_superuser = True
         user.is_staff = True
         user.save()
     return user
```

### Comparing `moni-auth-1.0.3/moni_auth/views.py` & `moni-auth-1.0.4/moni_auth/views.py`

 * *Files identical despite different names*

### Comparing `moni-auth-1.0.3/moni_auth.egg-info/PKG-INFO` & `moni-auth-1.0.4/moni_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moni-auth
-Version: 1.0.3
+Version: 1.0.4
 Summary: Django app to integrate with the centralized Moni authentication system
 Home-page: https://www.example.com/
 Author: Lorenzo Fabro
 Author-email: lorenzo.fabro@moni.com.ar
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `moni-auth-1.0.3/setup.cfg` & `moni-auth-1.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = moni-auth
-version = 1.0.3
+version = 1.0.4
 description = Django app to integrate with the centralized Moni authentication system
 long_description = file: README.rst
 url = https://www.example.com/
 author = Lorenzo Fabro
 author_email = lorenzo.fabro@moni.com.ar
 classifiers = 
 	Environment :: Web Environment
```

