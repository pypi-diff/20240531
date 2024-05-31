# Comparing `tmp/colorcall-0.1.1.tar.gz` & `tmp/colorcall-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorcall-0.1.1.tar", last modified: Fri May 31 07:27:10 2024, max compression
+gzip compressed data, was "colorcall-0.2.0.tar", last modified: Fri May 31 08:48:17 2024, max compression
```

## Comparing `colorcall-0.1.1.tar` & `colorcall-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 07:27:10.933271 colorcall-0.1.1/
--rw-r--r--   0 root         (0) root         (0)      977 2024-05-31 07:27:10.933271 colorcall-0.1.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 07:27:10.933271 colorcall-0.1.1/colorcall/
--rw-rw-r--   0 root         (0) root         (0)      584 2024-05-31 07:27:10.000000 colorcall-0.1.1/colorcall/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1027 2024-05-31 06:46:29.000000 colorcall-0.1.1/colorcall/colorizer.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-31 06:18:56.000000 colorcall-0.1.1/colorcall/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 07:27:10.933271 colorcall-0.1.1/colorcall.egg-info/
--rw-r--r--   0 root         (0) root         (0)      977 2024-05-31 07:27:10.000000 colorcall-0.1.1/colorcall.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      204 2024-05-31 07:27:10.000000 colorcall-0.1.1/colorcall.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 07:27:10.000000 colorcall-0.1.1/colorcall.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-31 07:27:10.000000 colorcall-0.1.1/colorcall.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 07:27:10.933271 colorcall-0.1.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      595 2024-05-31 07:25:13.000000 colorcall-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 08:48:17.697541 colorcall-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)      977 2024-05-31 08:48:17.697541 colorcall-0.2.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 08:48:17.697541 colorcall-0.2.0/colorcall/
+-rw-rw-r--   0 root         (0) root         (0)      584 2024-05-31 08:48:06.000000 colorcall-0.2.0/colorcall/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1172 2024-05-31 08:47:21.000000 colorcall-0.2.0/colorcall/colorizer.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-31 06:18:56.000000 colorcall-0.2.0/colorcall/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 08:48:17.697541 colorcall-0.2.0/colorcall.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      977 2024-05-31 08:48:17.000000 colorcall-0.2.0/colorcall.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      204 2024-05-31 08:48:17.000000 colorcall-0.2.0/colorcall.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 08:48:17.000000 colorcall-0.2.0/colorcall.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-31 08:48:17.000000 colorcall-0.2.0/colorcall.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 08:48:17.697541 colorcall-0.2.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      595 2024-05-31 07:47:09.000000 colorcall-0.2.0/setup.py
```

### Comparing `colorcall-0.1.1/PKG-INFO` & `colorcall-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colorcall
-Version: 0.1.1
+Version: 0.2.0
 Summary: Color call your caracal
 Home-page: https://github.com/Sw1mmeR/colorcall/tree/main
 Author: Mikle Sedrakyan
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `colorcall-0.1.1/colorcall/__init__.py` & `colorcall-0.2.0/colorcall/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .colorizer import Color, FontStyle, _cprint, basic, rgb
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 
 
 def black(text: str) -> None:
     _cprint(text, Color.black)
 
 
 def red(text: str) -> None:
```

### Comparing `colorcall-0.1.1/colorcall.egg-info/PKG-INFO` & `colorcall-0.2.0/colorcall.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colorcall
-Version: 0.1.1
+Version: 0.2.0
 Summary: Color call your caracal
 Home-page: https://github.com/Sw1mmeR/colorcall/tree/main
 Author: Mikle Sedrakyan
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `colorcall-0.1.1/setup.py` & `colorcall-0.2.0/setup.py`

 * *Files identical despite different names*

