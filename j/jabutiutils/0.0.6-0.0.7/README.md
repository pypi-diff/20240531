# Comparing `tmp/jabutiutils-0.0.6.tar.gz` & `tmp/jabutiutils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jabutiutils-0.0.6.tar", last modified: Fri May 31 14:16:56 2024, max compression
+gzip compressed data, was "jabutiutils-0.0.7.tar", last modified: Fri May 31 14:33:57 2024, max compression
```

## Comparing `jabutiutils-0.0.6.tar` & `jabutiutils-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 14:16:56.680032 jabutiutils-0.0.6/
--rw-rw-rw-   0        0        0     1072 2024-05-29 20:23:25.000000 jabutiutils-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      219 2024-05-31 14:16:56.677270 jabutiutils-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-29 20:14:42.000000 jabutiutils-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 14:16:56.642494 jabutiutils-0.0.6/jabutiutils/
--rw-rw-rw-   0        0        0        0 2024-05-29 20:24:06.000000 jabutiutils-0.0.6/jabutiutils/JbtUtils.py
--rw-rw-rw-   0        0        0        0 2024-05-29 20:40:15.000000 jabutiutils-0.0.6/jabutiutils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 14:16:56.665002 jabutiutils-0.0.6/jabutiutils/ms_identity_web/
--rw-rw-rw-   0        0        0    15688 2024-05-29 20:30:56.000000 jabutiutils-0.0.6/jabutiutils/ms_identity_web/__init__.py
--rw-rw-rw-   0        0        0     9507 2024-05-29 20:30:10.000000 jabutiutils-0.0.6/jabutiutils/ms_identity_web/adapters.py
--rw-rw-rw-   0        0        0     3642 2024-05-29 20:27:25.000000 jabutiutils-0.0.6/jabutiutils/ms_identity_web/configuration.py
--rw-rw-rw-   0        0        0     3173 2024-05-29 20:27:48.000000 jabutiutils-0.0.6/jabutiutils/ms_identity_web/constants.py
--rw-rw-rw-   0        0        0     2779 2024-05-29 20:29:54.000000 jabutiutils-0.0.6/jabutiutils/ms_identity_web/context.py
-drwxrwxrwx   0        0        0        0 2024-05-31 14:16:56.673512 jabutiutils-0.0.6/jabutiutils/ms_identity_web/django/
--rw-rw-rw-   0        0        0        0 2024-05-29 21:03:33.000000 jabutiutils-0.0.6/jabutiutils/ms_identity_web/django/__init__.py
--rw-rw-rw-   0        0        0     4911 2024-05-29 21:05:19.000000 jabutiutils-0.0.6/jabutiutils/ms_identity_web/django/adapter.py
--rw-rw-rw-   0        0        0     1324 2024-05-29 21:04:05.000000 jabutiutils-0.0.6/jabutiutils/ms_identity_web/django/middleware.py
--rw-rw-rw-   0        0        0     2828 2024-05-29 21:04:53.000000 jabutiutils-0.0.6/jabutiutils/ms_identity_web/django/msal_views_and_urls.py
--rw-rw-rw-   0        0        0     1277 2024-05-29 20:30:31.000000 jabutiutils-0.0.6/jabutiutils/ms_identity_web/errors.py
-drwxrwxrwx   0        0        0        0 2024-05-31 14:16:56.675674 jabutiutils-0.0.6/jabutiutils.egg-info/
--rw-rw-rw-   0        0        0      219 2024-05-31 14:16:56.000000 jabutiutils-0.0.6/jabutiutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      691 2024-05-31 14:16:56.000000 jabutiutils-0.0.6/jabutiutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 14:16:56.000000 jabutiutils-0.0.6/jabutiutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-05-31 14:16:56.000000 jabutiutils-0.0.6/jabutiutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-31 14:16:56.000000 jabutiutils-0.0.6/jabutiutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 14:16:56.680032 jabutiutils-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      247 2024-05-31 14:16:33.000000 jabutiutils-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:33:57.590429 jabutiutils-0.0.7/
+-rw-rw-rw-   0        0        0     1072 2024-05-29 20:23:25.000000 jabutiutils-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      219 2024-05-31 14:33:57.588425 jabutiutils-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-29 20:14:42.000000 jabutiutils-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 14:33:57.556944 jabutiutils-0.0.7/jabutiutils/
+-rw-rw-rw-   0        0        0        0 2024-05-29 20:24:06.000000 jabutiutils-0.0.7/jabutiutils/JbtUtils.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 20:40:15.000000 jabutiutils-0.0.7/jabutiutils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:33:57.576272 jabutiutils-0.0.7/jabutiutils/ms_identity_web/
+-rw-rw-rw-   0        0        0    15688 2024-05-29 20:30:56.000000 jabutiutils-0.0.7/jabutiutils/ms_identity_web/__init__.py
+-rw-rw-rw-   0        0        0     9507 2024-05-29 20:30:10.000000 jabutiutils-0.0.7/jabutiutils/ms_identity_web/adapters.py
+-rw-rw-rw-   0        0        0     3642 2024-05-29 20:27:25.000000 jabutiutils-0.0.7/jabutiutils/ms_identity_web/configuration.py
+-rw-rw-rw-   0        0        0     3173 2024-05-29 20:27:48.000000 jabutiutils-0.0.7/jabutiutils/ms_identity_web/constants.py
+-rw-rw-rw-   0        0        0     2779 2024-05-29 20:29:54.000000 jabutiutils-0.0.7/jabutiutils/ms_identity_web/context.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:33:57.585426 jabutiutils-0.0.7/jabutiutils/ms_identity_web/django/
+-rw-rw-rw-   0        0        0        0 2024-05-29 21:03:33.000000 jabutiutils-0.0.7/jabutiutils/ms_identity_web/django/__init__.py
+-rw-rw-rw-   0        0        0     4897 2024-05-31 14:33:42.000000 jabutiutils-0.0.7/jabutiutils/ms_identity_web/django/adapter.py
+-rw-rw-rw-   0        0        0     1324 2024-05-29 21:04:05.000000 jabutiutils-0.0.7/jabutiutils/ms_identity_web/django/middleware.py
+-rw-rw-rw-   0        0        0     2828 2024-05-29 21:04:53.000000 jabutiutils-0.0.7/jabutiutils/ms_identity_web/django/msal_views_and_urls.py
+-rw-rw-rw-   0        0        0     1277 2024-05-29 20:30:31.000000 jabutiutils-0.0.7/jabutiutils/ms_identity_web/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:33:57.587426 jabutiutils-0.0.7/jabutiutils.egg-info/
+-rw-rw-rw-   0        0        0      219 2024-05-31 14:33:57.000000 jabutiutils-0.0.7/jabutiutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      691 2024-05-31 14:33:57.000000 jabutiutils-0.0.7/jabutiutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 14:33:57.000000 jabutiutils-0.0.7/jabutiutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-31 14:33:57.000000 jabutiutils-0.0.7/jabutiutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-31 14:33:57.000000 jabutiutils-0.0.7/jabutiutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 14:33:57.590429 jabutiutils-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      247 2024-05-31 14:33:47.000000 jabutiutils-0.0.7/setup.py
```

### Comparing `jabutiutils-0.0.6/LICENSE` & `jabutiutils-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jabutiutils-0.0.6/jabutiutils/ms_identity_web/__init__.py` & `jabutiutils-0.0.7/jabutiutils/ms_identity_web/__init__.py`

 * *Files identical despite different names*

### Comparing `jabutiutils-0.0.6/jabutiutils/ms_identity_web/adapters.py` & `jabutiutils-0.0.7/jabutiutils/ms_identity_web/adapters.py`

 * *Files identical despite different names*

### Comparing `jabutiutils-0.0.6/jabutiutils/ms_identity_web/configuration.py` & `jabutiutils-0.0.7/jabutiutils/ms_identity_web/configuration.py`

 * *Files identical despite different names*

### Comparing `jabutiutils-0.0.6/jabutiutils/ms_identity_web/constants.py` & `jabutiutils-0.0.7/jabutiutils/ms_identity_web/constants.py`

 * *Files identical despite different names*

### Comparing `jabutiutils-0.0.6/jabutiutils/ms_identity_web/context.py` & `jabutiutils-0.0.7/jabutiutils/ms_identity_web/context.py`

 * *Files identical despite different names*

### Comparing `jabutiutils-0.0.6/jabutiutils/ms_identity_web/django/adapter.py` & `jabutiutils-0.0.7/jabutiutils/ms_identity_web/django/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 try:
     from ms_identity_web import IdentityWebPython
     from ms_identity_web.context import IdentityContextData
-    from ms_identity_web.adapters import IdentityWebContextAdapter
+    from ..adapters import IdentityWebContextAdapter
     from django.http.request import HttpRequest as DjangoHttpRequest
     from django.shortcuts import redirect as django_redirect
     import logging
 except:
     pass
 
 class DjangoContextAdapter(IdentityWebContextAdapter):
```

### Comparing `jabutiutils-0.0.6/jabutiutils/ms_identity_web/django/middleware.py` & `jabutiutils-0.0.7/jabutiutils/ms_identity_web/django/middleware.py`

 * *Files identical despite different names*

### Comparing `jabutiutils-0.0.6/jabutiutils/ms_identity_web/django/msal_views_and_urls.py` & `jabutiutils-0.0.7/jabutiutils/ms_identity_web/django/msal_views_and_urls.py`

 * *Files identical despite different names*

### Comparing `jabutiutils-0.0.6/jabutiutils/ms_identity_web/errors.py` & `jabutiutils-0.0.7/jabutiutils/ms_identity_web/errors.py`

 * *Files identical despite different names*

### Comparing `jabutiutils-0.0.6/jabutiutils.egg-info/SOURCES.txt` & `jabutiutils-0.0.7/jabutiutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

