# Comparing `tmp/apiamocrm-0.1.4.tar.gz` & `tmp/apiamocrm-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apiamocrm-0.1.4.tar", last modified: Fri May 31 03:12:07 2024, max compression
+gzip compressed data, was "apiamocrm-0.1.5.tar", last modified: Fri May 31 05:19:56 2024, max compression
```

## Comparing `apiamocrm-0.1.4.tar` & `apiamocrm-0.1.5.tar`

### file list

```diff
@@ -1,29 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 03:12:07.207208 apiamocrm-0.1.4/
--rw-rw-rw-   0        0        0      438 2024-05-31 03:12:07.205213 apiamocrm-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-30 09:48:06.000000 apiamocrm-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 03:12:07.182353 apiamocrm-0.1.4/amoApi/
--rw-rw-rw-   0        0        0     6353 2024-05-29 09:02:42.000000 apiamocrm-0.1.4/amoApi/API.py
--rw-rw-rw-   0        0        0        0 2024-05-30 10:16:29.000000 apiamocrm-0.1.4/amoApi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 03:12:07.185344 apiamocrm-0.1.4/amoApi/amoEntities/
--rw-rw-rw-   0        0        0     1612 2024-05-28 06:33:36.000000 apiamocrm-0.1.4/amoApi/amoEntities/Contact.py
--rw-rw-rw-   0        0        0     3338 2024-05-29 08:28:40.000000 apiamocrm-0.1.4/amoApi/amoEntities/Lead.py
--rw-rw-rw-   0        0        0        0 2024-05-30 10:19:41.000000 apiamocrm-0.1.4/amoApi/amoEntities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 03:12:07.191558 apiamocrm-0.1.4/amoChatApi/
--rw-rw-rw-   0        0        0     5038 2024-05-30 03:55:43.000000 apiamocrm-0.1.4/amoChatApi/API.py
--rw-rw-rw-   0        0        0      138 2024-05-28 08:25:22.000000 apiamocrm-0.1.4/amoChatApi/Message.py
--rw-rw-rw-   0        0        0     1876 2024-05-29 07:38:48.000000 apiamocrm-0.1.4/amoChatApi/Payload.py
--rw-rw-rw-   0        0        0      384 2024-05-28 08:33:26.000000 apiamocrm-0.1.4/amoChatApi/TextMessage.py
--rw-rw-rw-   0        0        0        0 2024-05-30 10:16:39.000000 apiamocrm-0.1.4/amoChatApi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 03:12:07.204216 apiamocrm-0.1.4/apiAmoCRM.egg-info/
--rw-rw-rw-   0        0        0      438 2024-05-31 03:12:07.000000 apiamocrm-0.1.4/apiAmoCRM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      521 2024-05-31 03:12:07.000000 apiamocrm-0.1.4/apiAmoCRM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 03:12:07.000000 apiamocrm-0.1.4/apiAmoCRM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-31 03:12:07.000000 apiamocrm-0.1.4/apiAmoCRM.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-31 03:12:07.000000 apiamocrm-0.1.4/apiAmoCRM.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-31 03:12:07.203218 apiamocrm-0.1.4/services/
--rw-rw-rw-   0        0        0      243 2024-05-30 03:55:43.000000 apiamocrm-0.1.4/services/AbstractService.py
--rw-rw-rw-   0        0        0     4710 2024-05-30 09:08:16.000000 apiamocrm-0.1.4/services/BibinetService.py
--rw-rw-rw-   0        0        0     5765 2024-05-30 09:08:23.000000 apiamocrm-0.1.4/services/DromService.py
--rw-rw-rw-   0        0        0     5749 2024-05-30 09:08:57.000000 apiamocrm-0.1.4/services/JapancarService.py
--rw-rw-rw-   0        0        0       42 2024-05-31 03:12:07.207208 apiamocrm-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      633 2024-05-31 03:11:56.000000 apiamocrm-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:19:56.868632 apiamocrm-0.1.5/
+-rw-rw-rw-   0        0        0      438 2024-05-31 05:19:56.867632 apiamocrm-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-30 09:48:06.000000 apiamocrm-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 05:19:56.852944 apiamocrm-0.1.5/amoApi/
+-rw-rw-rw-   0        0        0     6353 2024-05-29 09:02:42.000000 apiamocrm-0.1.5/amoApi/API.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 10:16:29.000000 apiamocrm-0.1.5/amoApi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:19:56.855935 apiamocrm-0.1.5/amoApi/amoEntities/
+-rw-rw-rw-   0        0        0     1612 2024-05-28 06:33:36.000000 apiamocrm-0.1.5/amoApi/amoEntities/Contact.py
+-rw-rw-rw-   0        0        0     3338 2024-05-29 08:28:40.000000 apiamocrm-0.1.5/amoApi/amoEntities/Lead.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 10:19:41.000000 apiamocrm-0.1.5/amoApi/amoEntities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:19:56.861116 apiamocrm-0.1.5/amoChatApi/
+-rw-rw-rw-   0        0        0     5038 2024-05-30 03:55:43.000000 apiamocrm-0.1.5/amoChatApi/API.py
+-rw-rw-rw-   0        0        0      138 2024-05-28 08:25:22.000000 apiamocrm-0.1.5/amoChatApi/Message.py
+-rw-rw-rw-   0        0        0     1876 2024-05-29 07:38:48.000000 apiamocrm-0.1.5/amoChatApi/Payload.py
+-rw-rw-rw-   0        0        0      384 2024-05-28 08:33:26.000000 apiamocrm-0.1.5/amoChatApi/TextMessage.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 10:16:39.000000 apiamocrm-0.1.5/amoChatApi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:19:56.866631 apiamocrm-0.1.5/apiAmoCRM.egg-info/
+-rw-rw-rw-   0        0        0      438 2024-05-31 05:19:56.000000 apiamocrm-0.1.5/apiAmoCRM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2024-05-31 05:19:56.000000 apiamocrm-0.1.5/apiAmoCRM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 05:19:56.000000 apiamocrm-0.1.5/apiAmoCRM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-31 05:19:56.000000 apiamocrm-0.1.5/apiAmoCRM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-31 05:19:56.000000 apiamocrm-0.1.5/apiAmoCRM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 05:19:56.868632 apiamocrm-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      633 2024-05-31 05:19:49.000000 apiamocrm-0.1.5/setup.py
```

### Comparing `apiamocrm-0.1.4/amoApi/API.py` & `apiamocrm-0.1.5/amoApi/API.py`

 * *Files identical despite different names*

### Comparing `apiamocrm-0.1.4/amoApi/amoEntities/Contact.py` & `apiamocrm-0.1.5/amoApi/amoEntities/Contact.py`

 * *Files identical despite different names*

### Comparing `apiamocrm-0.1.4/amoApi/amoEntities/Lead.py` & `apiamocrm-0.1.5/amoApi/amoEntities/Lead.py`

 * *Files identical despite different names*

### Comparing `apiamocrm-0.1.4/amoChatApi/API.py` & `apiamocrm-0.1.5/amoChatApi/API.py`

 * *Files identical despite different names*

### Comparing `apiamocrm-0.1.4/amoChatApi/Payload.py` & `apiamocrm-0.1.5/amoChatApi/Payload.py`

 * *Files identical despite different names*

### Comparing `apiamocrm-0.1.4/setup.py` & `apiamocrm-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='apiAmoCRM',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
     install_requires=[
         "requests",
     ],
     author='wlovem',
     author_email='wlovemrock@gmail.com',
     description='Api for amoCRM',
```

