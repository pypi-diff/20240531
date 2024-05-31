# Comparing `tmp/jabutiutils-0.0.5.tar.gz` & `tmp/jabutiutils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jabutiutils-0.0.5.tar", last modified: Wed May 29 21:07:56 2024, max compression
+gzip compressed data, was "jabutiutils-0.0.6.tar", last modified: Fri May 31 14:16:56 2024, max compression
```

## Comparing `jabutiutils-0.0.5.tar` & `jabutiutils-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 21:07:56.116047 jabutiutils-0.0.5/
--rw-rw-rw-   0        0        0     1072 2024-05-29 20:23:25.000000 jabutiutils-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      219 2024-05-29 21:07:56.113592 jabutiutils-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-29 20:14:42.000000 jabutiutils-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 21:07:56.086941 jabutiutils-0.0.5/jabutiutils/
--rw-rw-rw-   0        0        0        0 2024-05-29 20:24:06.000000 jabutiutils-0.0.5/jabutiutils/JbtUtils.py
--rw-rw-rw-   0        0        0        0 2024-05-29 20:40:15.000000 jabutiutils-0.0.5/jabutiutils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 21:07:56.104699 jabutiutils-0.0.5/jabutiutils/ms_identity_web/
--rw-rw-rw-   0        0        0    15688 2024-05-29 20:30:56.000000 jabutiutils-0.0.5/jabutiutils/ms_identity_web/__init__.py
--rw-rw-rw-   0        0        0     9507 2024-05-29 20:30:10.000000 jabutiutils-0.0.5/jabutiutils/ms_identity_web/adapters.py
--rw-rw-rw-   0        0        0     3642 2024-05-29 20:27:25.000000 jabutiutils-0.0.5/jabutiutils/ms_identity_web/configuration.py
--rw-rw-rw-   0        0        0     3173 2024-05-29 20:27:48.000000 jabutiutils-0.0.5/jabutiutils/ms_identity_web/constants.py
--rw-rw-rw-   0        0        0     2779 2024-05-29 20:29:54.000000 jabutiutils-0.0.5/jabutiutils/ms_identity_web/context.py
-drwxrwxrwx   0        0        0        0 2024-05-29 21:07:56.110227 jabutiutils-0.0.5/jabutiutils/ms_identity_web/django/
--rw-rw-rw-   0        0        0        0 2024-05-29 21:03:33.000000 jabutiutils-0.0.5/jabutiutils/ms_identity_web/django/__init__.py
--rw-rw-rw-   0        0        0     4911 2024-05-29 21:05:19.000000 jabutiutils-0.0.5/jabutiutils/ms_identity_web/django/adapter.py
--rw-rw-rw-   0        0        0     1324 2024-05-29 21:04:05.000000 jabutiutils-0.0.5/jabutiutils/ms_identity_web/django/middleware.py
--rw-rw-rw-   0        0        0     2828 2024-05-29 21:04:53.000000 jabutiutils-0.0.5/jabutiutils/ms_identity_web/django/msal_views_and_urls.py
--rw-rw-rw-   0        0        0     1277 2024-05-29 20:30:31.000000 jabutiutils-0.0.5/jabutiutils/ms_identity_web/errors.py
-drwxrwxrwx   0        0        0        0 2024-05-29 21:07:56.112516 jabutiutils-0.0.5/jabutiutils.egg-info/
--rw-rw-rw-   0        0        0      219 2024-05-29 21:07:56.000000 jabutiutils-0.0.5/jabutiutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      691 2024-05-29 21:07:56.000000 jabutiutils-0.0.5/jabutiutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 21:07:56.000000 jabutiutils-0.0.5/jabutiutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-05-29 21:07:56.000000 jabutiutils-0.0.5/jabutiutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-29 21:07:56.000000 jabutiutils-0.0.5/jabutiutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 21:07:56.116047 jabutiutils-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      247 2024-05-29 21:07:52.000000 jabutiutils-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:16:56.680032 jabutiutils-0.0.6/
+-rw-rw-rw-   0        0        0     1072 2024-05-29 20:23:25.000000 jabutiutils-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      219 2024-05-31 14:16:56.677270 jabutiutils-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-29 20:14:42.000000 jabutiutils-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 14:16:56.642494 jabutiutils-0.0.6/jabutiutils/
+-rw-rw-rw-   0        0        0        0 2024-05-29 20:24:06.000000 jabutiutils-0.0.6/jabutiutils/JbtUtils.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 20:40:15.000000 jabutiutils-0.0.6/jabutiutils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:16:56.665002 jabutiutils-0.0.6/jabutiutils/ms_identity_web/
+-rw-rw-rw-   0        0        0    15688 2024-05-29 20:30:56.000000 jabutiutils-0.0.6/jabutiutils/ms_identity_web/__init__.py
+-rw-rw-rw-   0        0        0     9507 2024-05-29 20:30:10.000000 jabutiutils-0.0.6/jabutiutils/ms_identity_web/adapters.py
+-rw-rw-rw-   0        0        0     3642 2024-05-29 20:27:25.000000 jabutiutils-0.0.6/jabutiutils/ms_identity_web/configuration.py
+-rw-rw-rw-   0        0        0     3173 2024-05-29 20:27:48.000000 jabutiutils-0.0.6/jabutiutils/ms_identity_web/constants.py
+-rw-rw-rw-   0        0        0     2779 2024-05-29 20:29:54.000000 jabutiutils-0.0.6/jabutiutils/ms_identity_web/context.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:16:56.673512 jabutiutils-0.0.6/jabutiutils/ms_identity_web/django/
+-rw-rw-rw-   0        0        0        0 2024-05-29 21:03:33.000000 jabutiutils-0.0.6/jabutiutils/ms_identity_web/django/__init__.py
+-rw-rw-rw-   0        0        0     4911 2024-05-29 21:05:19.000000 jabutiutils-0.0.6/jabutiutils/ms_identity_web/django/adapter.py
+-rw-rw-rw-   0        0        0     1324 2024-05-29 21:04:05.000000 jabutiutils-0.0.6/jabutiutils/ms_identity_web/django/middleware.py
+-rw-rw-rw-   0        0        0     2828 2024-05-29 21:04:53.000000 jabutiutils-0.0.6/jabutiutils/ms_identity_web/django/msal_views_and_urls.py
+-rw-rw-rw-   0        0        0     1277 2024-05-29 20:30:31.000000 jabutiutils-0.0.6/jabutiutils/ms_identity_web/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:16:56.675674 jabutiutils-0.0.6/jabutiutils.egg-info/
+-rw-rw-rw-   0        0        0      219 2024-05-31 14:16:56.000000 jabutiutils-0.0.6/jabutiutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      691 2024-05-31 14:16:56.000000 jabutiutils-0.0.6/jabutiutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 14:16:56.000000 jabutiutils-0.0.6/jabutiutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-31 14:16:56.000000 jabutiutils-0.0.6/jabutiutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-31 14:16:56.000000 jabutiutils-0.0.6/jabutiutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 14:16:56.680032 jabutiutils-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      247 2024-05-31 14:16:33.000000 jabutiutils-0.0.6/setup.py
```

### Comparing `jabutiutils-0.0.5/LICENSE` & `jabutiutils-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jabutiutils-0.0.5/jabutiutils/ms_identity_web/__init__.py` & `jabutiutils-0.0.6/jabutiutils/ms_identity_web/__init__.py`

 * *Files identical despite different names*

### Comparing `jabutiutils-0.0.5/jabutiutils/ms_identity_web/adapters.py` & `jabutiutils-0.0.6/jabutiutils/ms_identity_web/adapters.py`

 * *Files identical despite different names*

### Comparing `jabutiutils-0.0.5/jabutiutils/ms_identity_web/configuration.py` & `jabutiutils-0.0.6/jabutiutils/ms_identity_web/configuration.py`

 * *Files identical despite different names*

### Comparing `jabutiutils-0.0.5/jabutiutils/ms_identity_web/constants.py` & `jabutiutils-0.0.6/jabutiutils/ms_identity_web/constants.py`

 * *Files identical despite different names*

### Comparing `jabutiutils-0.0.5/jabutiutils/ms_identity_web/context.py` & `jabutiutils-0.0.6/jabutiutils/ms_identity_web/context.py`

 * *Files identical despite different names*

### Comparing `jabutiutils-0.0.5/jabutiutils/ms_identity_web/django/adapter.py` & `jabutiutils-0.0.6/jabutiutils/ms_identity_web/django/adapter.py`

 * *Files identical despite different names*

### Comparing `jabutiutils-0.0.5/jabutiutils/ms_identity_web/django/middleware.py` & `jabutiutils-0.0.6/jabutiutils/ms_identity_web/django/middleware.py`

 * *Files identical despite different names*

### Comparing `jabutiutils-0.0.5/jabutiutils/ms_identity_web/django/msal_views_and_urls.py` & `jabutiutils-0.0.6/jabutiutils/ms_identity_web/django/msal_views_and_urls.py`

 * *Files identical despite different names*

### Comparing `jabutiutils-0.0.5/jabutiutils/ms_identity_web/errors.py` & `jabutiutils-0.0.6/jabutiutils/ms_identity_web/errors.py`

 * *Files identical despite different names*

### Comparing `jabutiutils-0.0.5/jabutiutils.egg-info/SOURCES.txt` & `jabutiutils-0.0.6/jabutiutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

