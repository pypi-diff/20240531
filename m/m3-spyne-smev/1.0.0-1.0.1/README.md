# Comparing `tmp/m3-spyne-smev-1.0.0.tar.gz` & `tmp/m3-spyne-smev-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m3-spyne-smev-1.0.0.tar", last modified: Wed Jul 26 08:51:55 2023, max compression
+gzip compressed data, was "m3-spyne-smev-1.0.1.tar", last modified: Fri May 31 09:33:56 2024, max compression
```

## Comparing `m3-spyne-smev-1.0.0.tar` & `m3-spyne-smev-1.0.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:51:55.463104 m3-spyne-smev-1.0.0/
--rw-r--r--   0 root         (0) root         (0)       93 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.0/DESCRIPTION
--rw-r--r--   0 root         (0) root         (0)     3461 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      154 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1044 2023-07-26 08:51:55.463104 m3-spyne-smev-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13033 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/README
--rw-r--r--   0 root         (0) root         (0)    13033 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 08:51:55.463104 m3-spyne-smev-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2595 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:51:55.451104 m3-spyne-smev-1.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:51:55.456104 m3-spyne-smev-1.0.0/src/m3_spyne_smev.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1044 2023-07-26 08:51:55.000000 m3-spyne-smev-1.0.0/src/m3_spyne_smev.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1057 2023-07-26 08:51:55.000000 m3-spyne-smev-1.0.0/src/m3_spyne_smev.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-07-26 08:51:55.000000 m3-spyne-smev-1.0.0/src/m3_spyne_smev.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-07-26 08:51:55.000000 m3-spyne-smev-1.0.0/src/m3_spyne_smev.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-26 08:51:55.000000 m3-spyne-smev-1.0.0/src/m3_spyne_smev.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:51:55.458104 m3-spyne-smev-1.0.0/src/spyne_smev/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11558 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/_base.py
--rw-r--r--   0 root         (0) root         (0)     2939 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/_utils.py
--rw-r--r--   0 root         (0) root         (0)     2433 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/_xmlns.py
--rw-r--r--   0 root         (0) root         (0)      980 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/application.py
--rw-r--r--   0 root         (0) root         (0)     5431 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/client.py
--rw-r--r--   0 root         (0) root         (0)     6454 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/crypto.py
--rw-r--r--   0 root         (0) root         (0)     1742 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/fault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:51:55.459104 m3-spyne-smev-1.0.0/src/spyne_smev/server/
--rw-r--r--   0 root         (0) root         (0)      327 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)      516 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/server/django.py
--rw-r--r--   0 root         (0) root         (0)      537 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/server/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:51:55.460104 m3-spyne-smev-1.0.0/src/spyne_smev/smev255/
--rw-r--r--   0 root         (0) root         (0)     7648 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/smev255/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3249 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/smev255/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:51:55.460104 m3-spyne-smev-1.0.0/src/spyne_smev/smev256/
--rw-r--r--   0 root         (0) root         (0)     8360 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/smev256/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3329 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/smev256/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:51:55.461104 m3-spyne-smev-1.0.0/src/spyne_smev/wsse/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/wsse/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5119 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/wsse/protocols.py
--rw-r--r--   0 root         (0) root         (0)    12346 2023-07-26 08:51:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/wsse/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:51:55.463104 m3-spyne-smev-1.0.0/src/spyne_smev/xsd/
--rw-r--r--   0 root         (0) root         (0)     3162 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/xsd/smev248-atachments.xsd
--rw-r--r--   0 root         (0) root         (0)    14970 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/xsd/smev248.xsd
--rw-r--r--   0 root         (0) root         (0)     3148 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/xsd/smev255-atachments.xsd
--rw-r--r--   0 root         (0) root         (0)    18041 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/xsd/smev255.xsd
--rw-r--r--   0 root         (0) root         (0)     3164 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/xsd/smev256-atachments.xsd
--rw-r--r--   0 root         (0) root         (0)    20659 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/xsd/smev256.xsd
--rw-r--r--   0 root         (0) root         (0)      518 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.0/src/spyne_smev/xsd/xop-include.xsd
--rw-r--r--   0 root         (0) root         (0)      448 2023-07-26 08:51:55.000000 m3-spyne-smev-1.0.0/version.conf
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-31 09:33:56.716713 m3-spyne-smev-1.0.1/
+-rw-r--r--   0 toor      (1000) toor      (1000)       93 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.1/DESCRIPTION
+-rw-r--r--   0 toor      (1000) toor      (1000)     3461 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.1/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      154 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.1/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)     1222 2024-05-31 09:33:56.716713 m3-spyne-smev-1.0.1/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)    13033 2024-05-31 09:33:52.000000 m3-spyne-smev-1.0.1/README
+-rw-r--r--   0 toor      (1000) toor      (1000)    13033 2024-05-31 09:33:52.000000 m3-spyne-smev-1.0.1/README.md
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2024-05-31 09:33:56.716713 m3-spyne-smev-1.0.1/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2595 2024-05-31 09:33:52.000000 m3-spyne-smev-1.0.1/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-31 09:33:56.696713 m3-spyne-smev-1.0.1/src/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-31 09:33:56.714713 m3-spyne-smev-1.0.1/src/m3_spyne_smev.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1222 2024-05-31 09:33:56.000000 m3-spyne-smev-1.0.1/src/m3_spyne_smev.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     1057 2024-05-31 09:33:56.000000 m3-spyne-smev-1.0.1/src/m3_spyne_smev.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       43 2024-05-31 09:33:56.000000 m3-spyne-smev-1.0.1/src/m3_spyne_smev.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      106 2024-05-31 09:33:56.000000 m3-spyne-smev-1.0.1/src/m3_spyne_smev.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       26 2024-05-31 09:33:56.000000 m3-spyne-smev-1.0.1/src/m3_spyne_smev.egg-info/top_level.txt
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-31 09:33:56.706713 m3-spyne-smev-1.0.1/src/spyne_smev/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-05-31 09:33:52.000000 m3-spyne-smev-1.0.1/src/spyne_smev/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    11558 2024-05-31 09:33:52.000000 m3-spyne-smev-1.0.1/src/spyne_smev/_base.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2939 2024-05-31 09:33:52.000000 m3-spyne-smev-1.0.1/src/spyne_smev/_utils.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2433 2024-05-31 09:33:52.000000 m3-spyne-smev-1.0.1/src/spyne_smev/_xmlns.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      980 2024-05-31 09:33:52.000000 m3-spyne-smev-1.0.1/src/spyne_smev/application.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5431 2024-05-31 09:33:52.000000 m3-spyne-smev-1.0.1/src/spyne_smev/client.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6454 2024-05-31 09:33:52.000000 m3-spyne-smev-1.0.1/src/spyne_smev/crypto.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1742 2024-05-31 09:33:52.000000 m3-spyne-smev-1.0.1/src/spyne_smev/fault.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-31 09:33:56.707713 m3-spyne-smev-1.0.1/src/spyne_smev/server/
+-rw-r--r--   0 toor      (1000) toor      (1000)      327 2024-05-31 09:33:52.000000 m3-spyne-smev-1.0.1/src/spyne_smev/server/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      532 2024-05-31 09:33:52.000000 m3-spyne-smev-1.0.1/src/spyne_smev/server/django.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      553 2024-05-31 09:33:52.000000 m3-spyne-smev-1.0.1/src/spyne_smev/server/wsgi.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-31 09:33:56.708713 m3-spyne-smev-1.0.1/src/spyne_smev/smev255/
+-rw-r--r--   0 toor      (1000) toor      (1000)     7648 2024-05-31 09:33:52.000000 m3-spyne-smev-1.0.1/src/spyne_smev/smev255/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3249 2024-05-31 09:33:52.000000 m3-spyne-smev-1.0.1/src/spyne_smev/smev255/model.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-31 09:33:56.709713 m3-spyne-smev-1.0.1/src/spyne_smev/smev256/
+-rw-r--r--   0 toor      (1000) toor      (1000)     8360 2024-05-31 09:33:52.000000 m3-spyne-smev-1.0.1/src/spyne_smev/smev256/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3329 2024-05-31 09:33:52.000000 m3-spyne-smev-1.0.1/src/spyne_smev/smev256/model.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-31 09:33:56.710713 m3-spyne-smev-1.0.1/src/spyne_smev/wsse/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-05-31 09:33:52.000000 m3-spyne-smev-1.0.1/src/spyne_smev/wsse/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5119 2024-05-31 09:33:52.000000 m3-spyne-smev-1.0.1/src/spyne_smev/wsse/protocols.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    12346 2024-05-31 09:33:52.000000 m3-spyne-smev-1.0.1/src/spyne_smev/wsse/utils.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-31 09:33:56.713713 m3-spyne-smev-1.0.1/src/spyne_smev/xsd/
+-rw-r--r--   0 toor      (1000) toor      (1000)     3162 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.1/src/spyne_smev/xsd/smev248-atachments.xsd
+-rw-r--r--   0 toor      (1000) toor      (1000)    14970 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.1/src/spyne_smev/xsd/smev248.xsd
+-rw-r--r--   0 toor      (1000) toor      (1000)     3148 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.1/src/spyne_smev/xsd/smev255-atachments.xsd
+-rw-r--r--   0 toor      (1000) toor      (1000)    18041 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.1/src/spyne_smev/xsd/smev255.xsd
+-rw-r--r--   0 toor      (1000) toor      (1000)     3164 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.1/src/spyne_smev/xsd/smev256-atachments.xsd
+-rw-r--r--   0 toor      (1000) toor      (1000)    20659 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.1/src/spyne_smev/xsd/smev256.xsd
+-rw-r--r--   0 toor      (1000) toor      (1000)      518 2023-07-25 12:36:42.000000 m3-spyne-smev-1.0.1/src/spyne_smev/xsd/xop-include.xsd
+-rw-r--r--   0 toor      (1000) toor      (1000)      450 2024-05-31 09:33:56.000000 m3-spyne-smev-1.0.1/version.conf
```

### Comparing `m3-spyne-smev-1.0.0/LICENSE` & `m3-spyne-smev-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-1.0.0/README` & `m3-spyne-smev-1.0.1/README`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-1.0.0/README.md` & `m3-spyne-smev-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-1.0.0/setup.py` & `m3-spyne-smev-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-1.0.0/src/m3_spyne_smev.egg-info/SOURCES.txt` & `m3-spyne-smev-1.0.1/src/m3_spyne_smev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-1.0.0/src/spyne_smev/_base.py` & `m3-spyne-smev-1.0.1/src/spyne_smev/_base.py`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-1.0.0/src/spyne_smev/_utils.py` & `m3-spyne-smev-1.0.1/src/spyne_smev/_utils.py`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-1.0.0/src/spyne_smev/_xmlns.py` & `m3-spyne-smev-1.0.1/src/spyne_smev/_xmlns.py`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-1.0.0/src/spyne_smev/application.py` & `m3-spyne-smev-1.0.1/src/spyne_smev/application.py`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-1.0.0/src/spyne_smev/client.py` & `m3-spyne-smev-1.0.1/src/spyne_smev/client.py`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-1.0.0/src/spyne_smev/crypto.py` & `m3-spyne-smev-1.0.1/src/spyne_smev/crypto.py`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-1.0.0/src/spyne_smev/fault.py` & `m3-spyne-smev-1.0.1/src/spyne_smev/fault.py`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-1.0.0/src/spyne_smev/server/django.py` & `m3-spyne-smev-1.0.1/src/spyne_smev/server/wsgi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from spyne.server.django import DjangoApplication as _SpyneDjangoApplication
+from spyne.server.wsgi import WsgiApplication as _SpyneWsgiApplication
 
 from spyne_smev.server import _AllYourInterfaceDocuments
 
 
-class DjangoApplication(_SpyneDjangoApplication):
+class WsgiApplication(_SpyneWsgiApplication):
 
     # pylint: disable=abstract-method
 
     def __init__(self, app, chunked=True, max_content_length=2 * 1024 * 1024,
                  block_length=8 * 1024):
-        super(DjangoApplication, self).__init__(
-            app, chunked, max_content_length, block_length)
-        self.doc = _AllYourInterfaceDocuments(app.interface)
+        super(WsgiApplication, self).__init__(app, chunked, max_content_length,
+                                              block_length)
+
+        self.app.interface.docs = _AllYourInterfaceDocuments(app.interface)
```

### Comparing `m3-spyne-smev-1.0.0/src/spyne_smev/smev255/__init__.py` & `m3-spyne-smev-1.0.1/src/spyne_smev/smev255/__init__.py`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-1.0.0/src/spyne_smev/smev255/model.py` & `m3-spyne-smev-1.0.1/src/spyne_smev/smev255/model.py`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-1.0.0/src/spyne_smev/smev256/__init__.py` & `m3-spyne-smev-1.0.1/src/spyne_smev/smev256/__init__.py`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-1.0.0/src/spyne_smev/smev256/model.py` & `m3-spyne-smev-1.0.1/src/spyne_smev/smev256/model.py`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-1.0.0/src/spyne_smev/wsse/protocols.py` & `m3-spyne-smev-1.0.1/src/spyne_smev/wsse/protocols.py`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-1.0.0/src/spyne_smev/wsse/utils.py` & `m3-spyne-smev-1.0.1/src/spyne_smev/wsse/utils.py`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-1.0.0/src/spyne_smev/xsd/smev248-atachments.xsd` & `m3-spyne-smev-1.0.1/src/spyne_smev/xsd/smev248-atachments.xsd`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-1.0.0/src/spyne_smev/xsd/smev248.xsd` & `m3-spyne-smev-1.0.1/src/spyne_smev/xsd/smev248.xsd`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-1.0.0/src/spyne_smev/xsd/smev255-atachments.xsd` & `m3-spyne-smev-1.0.1/src/spyne_smev/xsd/smev255-atachments.xsd`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-1.0.0/src/spyne_smev/xsd/smev255.xsd` & `m3-spyne-smev-1.0.1/src/spyne_smev/xsd/smev255.xsd`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-1.0.0/src/spyne_smev/xsd/smev256-atachments.xsd` & `m3-spyne-smev-1.0.1/src/spyne_smev/xsd/smev256-atachments.xsd`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-1.0.0/src/spyne_smev/xsd/smev256.xsd` & `m3-spyne-smev-1.0.1/src/spyne_smev/xsd/smev256.xsd`

 * *Files identical despite different names*

### Comparing `m3-spyne-smev-1.0.0/src/spyne_smev/xsd/xop-include.xsd` & `m3-spyne-smev-1.0.1/src/spyne_smev/xsd/xop-include.xsd`

 * *Files identical despite different names*

