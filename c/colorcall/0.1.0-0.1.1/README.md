# Comparing `tmp/colorcall-0.1.0.tar.gz` & `tmp/colorcall-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorcall-0.1.0.tar", last modified: Fri May 31 06:28:09 2024, max compression
+gzip compressed data, was "colorcall-0.1.1.tar", last modified: Fri May 31 07:27:10 2024, max compression
```

## Comparing `colorcall-0.1.0.tar` & `colorcall-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 06:28:09.044509 colorcall-0.1.0/
--rw-r--r--   0 root         (0) root         (0)      174 2024-05-31 06:28:09.044509 colorcall-0.1.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 06:28:09.044509 colorcall-0.1.0/colorcall/
--rw-rw-r--   0 root         (0) root         (0)      584 2024-05-31 06:28:08.000000 colorcall-0.1.0/colorcall/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1013 2024-05-31 06:19:42.000000 colorcall-0.1.0/colorcall/colorizer.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-31 06:18:56.000000 colorcall-0.1.0/colorcall/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 06:28:09.044509 colorcall-0.1.0/colorcall.egg-info/
--rw-r--r--   0 root         (0) root         (0)      174 2024-05-31 06:28:09.000000 colorcall-0.1.0/colorcall.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      204 2024-05-31 06:28:09.000000 colorcall-0.1.0/colorcall.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 06:28:09.000000 colorcall-0.1.0/colorcall.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-31 06:28:09.000000 colorcall-0.1.0/colorcall.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 06:28:09.044509 colorcall-0.1.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      306 2024-05-31 06:25:34.000000 colorcall-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 07:27:10.933271 colorcall-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)      977 2024-05-31 07:27:10.933271 colorcall-0.1.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 07:27:10.933271 colorcall-0.1.1/colorcall/
+-rw-rw-r--   0 root         (0) root         (0)      584 2024-05-31 07:27:10.000000 colorcall-0.1.1/colorcall/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1027 2024-05-31 06:46:29.000000 colorcall-0.1.1/colorcall/colorizer.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-31 06:18:56.000000 colorcall-0.1.1/colorcall/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 07:27:10.933271 colorcall-0.1.1/colorcall.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      977 2024-05-31 07:27:10.000000 colorcall-0.1.1/colorcall.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      204 2024-05-31 07:27:10.000000 colorcall-0.1.1/colorcall.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 07:27:10.000000 colorcall-0.1.1/colorcall.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-31 07:27:10.000000 colorcall-0.1.1/colorcall.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 07:27:10.933271 colorcall-0.1.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      595 2024-05-31 07:25:13.000000 colorcall-0.1.1/setup.py
```

### Comparing `colorcall-0.1.0/colorcall/__init__.py` & `colorcall-0.1.1/colorcall/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .colorizer import Color, FontStyle, _cprint, basic, rgb
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 
 def black(text: str) -> None:
     _cprint(text, Color.black)
 
 
 def red(text: str) -> None:
```

### Comparing `colorcall-0.1.0/colorcall/colorizer.py` & `colorcall-0.1.1/colorcall/colorizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 def _cprint(text: str, color: Color) -> None:
     sys.stdout.write(basic(text, color, end="\n"))
 
 
 def basic(
     text: str,
-    color: Color,
+    color: Color = Color.white,
     style: FontStyle = FontStyle.default,
     target: Literal["font", "background"] = "font",
     end="",
 ) -> str:
     return f"\x1b[{style};{3 if target == 'font' else 4}{color.value}m{text}{end}\x1b[{style.default}m"
```

