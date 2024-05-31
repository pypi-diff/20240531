# Comparing `tmp/apiamocrm-0.1.2.tar.gz` & `tmp/apiamocrm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apiamocrm-0.1.2.tar", last modified: Thu May 30 10:18:30 2024, max compression
+gzip compressed data, was "apiamocrm-0.1.3.tar", last modified: Thu May 30 10:20:33 2024, max compression
```

## Comparing `apiamocrm-0.1.2.tar` & `apiamocrm-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 10:18:30.298593 apiamocrm-0.1.2/
--rw-rw-rw-   0        0        0      438 2024-05-30 10:18:30.297596 apiamocrm-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-30 09:48:06.000000 apiamocrm-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 10:18:30.279558 apiamocrm-0.1.2/amoApi/
--rw-rw-rw-   0        0        0     6353 2024-05-29 09:02:42.000000 apiamocrm-0.1.2/amoApi/API.py
--rw-rw-rw-   0        0        0        0 2024-05-30 10:16:29.000000 apiamocrm-0.1.2/amoApi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 10:18:30.285690 apiamocrm-0.1.2/amoChatApi/
--rw-rw-rw-   0        0        0     5038 2024-05-30 03:55:43.000000 apiamocrm-0.1.2/amoChatApi/API.py
--rw-rw-rw-   0        0        0      138 2024-05-28 08:25:22.000000 apiamocrm-0.1.2/amoChatApi/Message.py
--rw-rw-rw-   0        0        0     1876 2024-05-29 07:38:48.000000 apiamocrm-0.1.2/amoChatApi/Payload.py
--rw-rw-rw-   0        0        0      384 2024-05-28 08:33:26.000000 apiamocrm-0.1.2/amoChatApi/TextMessage.py
--rw-rw-rw-   0        0        0        0 2024-05-30 10:16:39.000000 apiamocrm-0.1.2/amoChatApi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 10:18:30.297596 apiamocrm-0.1.2/apiAmoCRM.egg-info/
--rw-rw-rw-   0        0        0      438 2024-05-30 10:18:30.000000 apiamocrm-0.1.2/apiAmoCRM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2024-05-30 10:18:30.000000 apiamocrm-0.1.2/apiAmoCRM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 10:18:30.000000 apiamocrm-0.1.2/apiAmoCRM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-30 10:18:30.000000 apiamocrm-0.1.2/apiAmoCRM.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-05-30 10:18:30.000000 apiamocrm-0.1.2/apiAmoCRM.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-30 10:18:30.296594 apiamocrm-0.1.2/services/
--rw-rw-rw-   0        0        0      243 2024-05-30 03:55:43.000000 apiamocrm-0.1.2/services/AbstractService.py
--rw-rw-rw-   0        0        0     4710 2024-05-30 09:08:16.000000 apiamocrm-0.1.2/services/BibinetService.py
--rw-rw-rw-   0        0        0     5765 2024-05-30 09:08:23.000000 apiamocrm-0.1.2/services/DromService.py
--rw-rw-rw-   0        0        0     5749 2024-05-30 09:08:57.000000 apiamocrm-0.1.2/services/JapancarService.py
--rw-rw-rw-   0        0        0        0 2024-05-30 10:17:02.000000 apiamocrm-0.1.2/services/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-30 10:18:30.298593 apiamocrm-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      633 2024-05-30 10:17:23.000000 apiamocrm-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 10:20:33.081108 apiamocrm-0.1.3/
+-rw-rw-rw-   0        0        0      438 2024-05-30 10:20:33.080353 apiamocrm-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-30 09:48:06.000000 apiamocrm-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 10:20:33.052734 apiamocrm-0.1.3/amoApi/
+-rw-rw-rw-   0        0        0     6353 2024-05-29 09:02:42.000000 apiamocrm-0.1.3/amoApi/API.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 10:16:29.000000 apiamocrm-0.1.3/amoApi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 10:20:33.062941 apiamocrm-0.1.3/amoApi/amoEntities/
+-rw-rw-rw-   0        0        0     1612 2024-05-28 06:33:36.000000 apiamocrm-0.1.3/amoApi/amoEntities/Contact.py
+-rw-rw-rw-   0        0        0     3338 2024-05-29 08:28:40.000000 apiamocrm-0.1.3/amoApi/amoEntities/Lead.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 10:19:41.000000 apiamocrm-0.1.3/amoApi/amoEntities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 10:20:33.067184 apiamocrm-0.1.3/amoChatApi/
+-rw-rw-rw-   0        0        0     5038 2024-05-30 03:55:43.000000 apiamocrm-0.1.3/amoChatApi/API.py
+-rw-rw-rw-   0        0        0      138 2024-05-28 08:25:22.000000 apiamocrm-0.1.3/amoChatApi/Message.py
+-rw-rw-rw-   0        0        0     1876 2024-05-29 07:38:48.000000 apiamocrm-0.1.3/amoChatApi/Payload.py
+-rw-rw-rw-   0        0        0      384 2024-05-28 08:33:26.000000 apiamocrm-0.1.3/amoChatApi/TextMessage.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 10:16:39.000000 apiamocrm-0.1.3/amoChatApi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 10:20:33.079353 apiamocrm-0.1.3/apiAmoCRM.egg-info/
+-rw-rw-rw-   0        0        0      438 2024-05-30 10:20:32.000000 apiamocrm-0.1.3/apiAmoCRM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      542 2024-05-30 10:20:33.000000 apiamocrm-0.1.3/apiAmoCRM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 10:20:32.000000 apiamocrm-0.1.3/apiAmoCRM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-30 10:20:32.000000 apiamocrm-0.1.3/apiAmoCRM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-30 10:20:32.000000 apiamocrm-0.1.3/apiAmoCRM.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 10:20:33.078597 apiamocrm-0.1.3/services/
+-rw-rw-rw-   0        0        0      243 2024-05-30 03:55:43.000000 apiamocrm-0.1.3/services/AbstractService.py
+-rw-rw-rw-   0        0        0     4710 2024-05-30 09:08:16.000000 apiamocrm-0.1.3/services/BibinetService.py
+-rw-rw-rw-   0        0        0     5765 2024-05-30 09:08:23.000000 apiamocrm-0.1.3/services/DromService.py
+-rw-rw-rw-   0        0        0     5749 2024-05-30 09:08:57.000000 apiamocrm-0.1.3/services/JapancarService.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 10:17:02.000000 apiamocrm-0.1.3/services/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 10:20:33.081108 apiamocrm-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      633 2024-05-30 10:20:12.000000 apiamocrm-0.1.3/setup.py
```

### Comparing `apiamocrm-0.1.2/amoApi/API.py` & `apiamocrm-0.1.3/amoApi/API.py`

 * *Files identical despite different names*

### Comparing `apiamocrm-0.1.2/amoChatApi/API.py` & `apiamocrm-0.1.3/amoChatApi/API.py`

 * *Files identical despite different names*

### Comparing `apiamocrm-0.1.2/amoChatApi/Payload.py` & `apiamocrm-0.1.3/amoChatApi/Payload.py`

 * *Files identical despite different names*

### Comparing `apiamocrm-0.1.2/services/BibinetService.py` & `apiamocrm-0.1.3/services/BibinetService.py`

 * *Files identical despite different names*

### Comparing `apiamocrm-0.1.2/services/DromService.py` & `apiamocrm-0.1.3/services/DromService.py`

 * *Files identical despite different names*

### Comparing `apiamocrm-0.1.2/services/JapancarService.py` & `apiamocrm-0.1.3/services/JapancarService.py`

 * *Files identical despite different names*

### Comparing `apiamocrm-0.1.2/setup.py` & `apiamocrm-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='apiAmoCRM',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=[
         "requests",
     ],
     author='wlovem',
     author_email='wlovemrock@gmail.com',
     description='Api for amoCRM',
```

