# Comparing `tmp/apiamocrm-0.1.3.tar.gz` & `tmp/apiamocrm-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apiamocrm-0.1.3.tar", last modified: Thu May 30 10:20:33 2024, max compression
+gzip compressed data, was "apiamocrm-0.1.4.tar", last modified: Fri May 31 03:12:07 2024, max compression
```

## Comparing `apiamocrm-0.1.3.tar` & `apiamocrm-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 10:20:33.081108 apiamocrm-0.1.3/
--rw-rw-rw-   0        0        0      438 2024-05-30 10:20:33.080353 apiamocrm-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-30 09:48:06.000000 apiamocrm-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 10:20:33.052734 apiamocrm-0.1.3/amoApi/
--rw-rw-rw-   0        0        0     6353 2024-05-29 09:02:42.000000 apiamocrm-0.1.3/amoApi/API.py
--rw-rw-rw-   0        0        0        0 2024-05-30 10:16:29.000000 apiamocrm-0.1.3/amoApi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 10:20:33.062941 apiamocrm-0.1.3/amoApi/amoEntities/
--rw-rw-rw-   0        0        0     1612 2024-05-28 06:33:36.000000 apiamocrm-0.1.3/amoApi/amoEntities/Contact.py
--rw-rw-rw-   0        0        0     3338 2024-05-29 08:28:40.000000 apiamocrm-0.1.3/amoApi/amoEntities/Lead.py
--rw-rw-rw-   0        0        0        0 2024-05-30 10:19:41.000000 apiamocrm-0.1.3/amoApi/amoEntities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 10:20:33.067184 apiamocrm-0.1.3/amoChatApi/
--rw-rw-rw-   0        0        0     5038 2024-05-30 03:55:43.000000 apiamocrm-0.1.3/amoChatApi/API.py
--rw-rw-rw-   0        0        0      138 2024-05-28 08:25:22.000000 apiamocrm-0.1.3/amoChatApi/Message.py
--rw-rw-rw-   0        0        0     1876 2024-05-29 07:38:48.000000 apiamocrm-0.1.3/amoChatApi/Payload.py
--rw-rw-rw-   0        0        0      384 2024-05-28 08:33:26.000000 apiamocrm-0.1.3/amoChatApi/TextMessage.py
--rw-rw-rw-   0        0        0        0 2024-05-30 10:16:39.000000 apiamocrm-0.1.3/amoChatApi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 10:20:33.079353 apiamocrm-0.1.3/apiAmoCRM.egg-info/
--rw-rw-rw-   0        0        0      438 2024-05-30 10:20:32.000000 apiamocrm-0.1.3/apiAmoCRM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      542 2024-05-30 10:20:33.000000 apiamocrm-0.1.3/apiAmoCRM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 10:20:32.000000 apiamocrm-0.1.3/apiAmoCRM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-30 10:20:32.000000 apiamocrm-0.1.3/apiAmoCRM.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-05-30 10:20:32.000000 apiamocrm-0.1.3/apiAmoCRM.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-30 10:20:33.078597 apiamocrm-0.1.3/services/
--rw-rw-rw-   0        0        0      243 2024-05-30 03:55:43.000000 apiamocrm-0.1.3/services/AbstractService.py
--rw-rw-rw-   0        0        0     4710 2024-05-30 09:08:16.000000 apiamocrm-0.1.3/services/BibinetService.py
--rw-rw-rw-   0        0        0     5765 2024-05-30 09:08:23.000000 apiamocrm-0.1.3/services/DromService.py
--rw-rw-rw-   0        0        0     5749 2024-05-30 09:08:57.000000 apiamocrm-0.1.3/services/JapancarService.py
--rw-rw-rw-   0        0        0        0 2024-05-30 10:17:02.000000 apiamocrm-0.1.3/services/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-30 10:20:33.081108 apiamocrm-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      633 2024-05-30 10:20:12.000000 apiamocrm-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:12:07.207208 apiamocrm-0.1.4/
+-rw-rw-rw-   0        0        0      438 2024-05-31 03:12:07.205213 apiamocrm-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-30 09:48:06.000000 apiamocrm-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 03:12:07.182353 apiamocrm-0.1.4/amoApi/
+-rw-rw-rw-   0        0        0     6353 2024-05-29 09:02:42.000000 apiamocrm-0.1.4/amoApi/API.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 10:16:29.000000 apiamocrm-0.1.4/amoApi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:12:07.185344 apiamocrm-0.1.4/amoApi/amoEntities/
+-rw-rw-rw-   0        0        0     1612 2024-05-28 06:33:36.000000 apiamocrm-0.1.4/amoApi/amoEntities/Contact.py
+-rw-rw-rw-   0        0        0     3338 2024-05-29 08:28:40.000000 apiamocrm-0.1.4/amoApi/amoEntities/Lead.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 10:19:41.000000 apiamocrm-0.1.4/amoApi/amoEntities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:12:07.191558 apiamocrm-0.1.4/amoChatApi/
+-rw-rw-rw-   0        0        0     5038 2024-05-30 03:55:43.000000 apiamocrm-0.1.4/amoChatApi/API.py
+-rw-rw-rw-   0        0        0      138 2024-05-28 08:25:22.000000 apiamocrm-0.1.4/amoChatApi/Message.py
+-rw-rw-rw-   0        0        0     1876 2024-05-29 07:38:48.000000 apiamocrm-0.1.4/amoChatApi/Payload.py
+-rw-rw-rw-   0        0        0      384 2024-05-28 08:33:26.000000 apiamocrm-0.1.4/amoChatApi/TextMessage.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 10:16:39.000000 apiamocrm-0.1.4/amoChatApi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:12:07.204216 apiamocrm-0.1.4/apiAmoCRM.egg-info/
+-rw-rw-rw-   0        0        0      438 2024-05-31 03:12:07.000000 apiamocrm-0.1.4/apiAmoCRM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      521 2024-05-31 03:12:07.000000 apiamocrm-0.1.4/apiAmoCRM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 03:12:07.000000 apiamocrm-0.1.4/apiAmoCRM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-31 03:12:07.000000 apiamocrm-0.1.4/apiAmoCRM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-31 03:12:07.000000 apiamocrm-0.1.4/apiAmoCRM.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 03:12:07.203218 apiamocrm-0.1.4/services/
+-rw-rw-rw-   0        0        0      243 2024-05-30 03:55:43.000000 apiamocrm-0.1.4/services/AbstractService.py
+-rw-rw-rw-   0        0        0     4710 2024-05-30 09:08:16.000000 apiamocrm-0.1.4/services/BibinetService.py
+-rw-rw-rw-   0        0        0     5765 2024-05-30 09:08:23.000000 apiamocrm-0.1.4/services/DromService.py
+-rw-rw-rw-   0        0        0     5749 2024-05-30 09:08:57.000000 apiamocrm-0.1.4/services/JapancarService.py
+-rw-rw-rw-   0        0        0       42 2024-05-31 03:12:07.207208 apiamocrm-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      633 2024-05-31 03:11:56.000000 apiamocrm-0.1.4/setup.py
```

### Comparing `apiamocrm-0.1.3/amoApi/API.py` & `apiamocrm-0.1.4/amoApi/API.py`

 * *Files identical despite different names*

### Comparing `apiamocrm-0.1.3/amoApi/amoEntities/Contact.py` & `apiamocrm-0.1.4/amoApi/amoEntities/Contact.py`

 * *Files identical despite different names*

### Comparing `apiamocrm-0.1.3/amoApi/amoEntities/Lead.py` & `apiamocrm-0.1.4/amoApi/amoEntities/Lead.py`

 * *Files identical despite different names*

### Comparing `apiamocrm-0.1.3/amoChatApi/API.py` & `apiamocrm-0.1.4/amoChatApi/API.py`

 * *Files identical despite different names*

### Comparing `apiamocrm-0.1.3/amoChatApi/Payload.py` & `apiamocrm-0.1.4/amoChatApi/Payload.py`

 * *Files identical despite different names*

### Comparing `apiamocrm-0.1.3/apiAmoCRM.egg-info/SOURCES.txt` & `apiamocrm-0.1.4/apiAmoCRM.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -14,9 +14,8 @@
 apiAmoCRM.egg-info/SOURCES.txt
 apiAmoCRM.egg-info/dependency_links.txt
 apiAmoCRM.egg-info/requires.txt
 apiAmoCRM.egg-info/top_level.txt
 services/AbstractService.py
 services/BibinetService.py
 services/DromService.py
-services/JapancarService.py
-services/__init__.py
+services/JapancarService.py
```

### Comparing `apiamocrm-0.1.3/services/BibinetService.py` & `apiamocrm-0.1.4/services/BibinetService.py`

 * *Files identical despite different names*

### Comparing `apiamocrm-0.1.3/services/DromService.py` & `apiamocrm-0.1.4/services/DromService.py`

 * *Files identical despite different names*

### Comparing `apiamocrm-0.1.3/services/JapancarService.py` & `apiamocrm-0.1.4/services/JapancarService.py`

 * *Files identical despite different names*

### Comparing `apiamocrm-0.1.3/setup.py` & `apiamocrm-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='apiAmoCRM',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     install_requires=[
         "requests",
     ],
     author='wlovem',
     author_email='wlovemrock@gmail.com',
     description='Api for amoCRM',
```

