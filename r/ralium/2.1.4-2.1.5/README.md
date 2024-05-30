# Comparing `tmp/ralium-2.1.4.tar.gz` & `tmp/ralium-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralium-2.1.4.tar", last modified: Wed May 29 20:36:17 2024, max compression
+gzip compressed data, was "ralium-2.1.5.tar", last modified: Thu May 30 22:17:43 2024, max compression
```

## Comparing `ralium-2.1.4.tar` & `ralium-2.1.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 20:36:17.806156 ralium-2.1.4/
--rw-rw-rw-   0        0        0    35823 2024-05-21 00:22:26.000000 ralium-2.1.4/LICENSE
--rw-rw-rw-   0        0        0    41897 2024-05-29 20:36:17.806156 ralium-2.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       52 2024-05-21 00:22:26.000000 ralium-2.1.4/README.md
--rw-rw-rw-   0        0        0      970 2024-05-29 20:35:32.000000 ralium-2.1.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-29 20:36:17.781469 ralium-2.1.4/ralium/
--rw-rw-rw-   0        0        0      357 2024-05-21 05:00:06.000000 ralium-2.1.4/ralium/__init__.py
--rw-rw-rw-   0        0        0     2381 2024-05-29 20:35:37.000000 ralium-2.1.4/ralium/_util.py
--rw-rw-rw-   0        0        0     1321 2024-05-29 20:31:01.000000 ralium-2.1.4/ralium/_util.pyi
--rw-rw-rw-   0        0        0     7555 2024-05-29 00:26:49.000000 ralium-2.1.4/ralium/api.py
--rw-rw-rw-   0        0        0     1066 2024-05-21 00:25:27.000000 ralium-2.1.4/ralium/api.pyi
--rw-rw-rw-   0        0        0      680 2024-05-21 00:25:27.000000 ralium-2.1.4/ralium/builtins.py
--rw-rw-rw-   0        0        0      541 2024-05-21 00:25:27.000000 ralium-2.1.4/ralium/builtins.pyi
--rw-rw-rw-   0        0        0     9598 2024-05-29 20:32:14.000000 ralium-2.1.4/ralium/bundle.py
--rw-rw-rw-   0        0        0     1958 2024-05-29 00:37:29.000000 ralium-2.1.4/ralium/bundle.pyi
--rw-rw-rw-   0        0        0     3332 2024-05-21 00:25:27.000000 ralium-2.1.4/ralium/config.py
--rw-rw-rw-   0        0        0      467 2024-05-21 00:25:27.000000 ralium-2.1.4/ralium/config.pyi
--rw-rw-rw-   0        0        0     6425 2024-05-21 00:25:27.000000 ralium-2.1.4/ralium/element.py
--rw-rw-rw-   0        0        0     1376 2024-05-21 00:26:03.000000 ralium-2.1.4/ralium/element.pyi
--rw-rw-rw-   0        0        0     4402 2024-05-21 00:26:03.000000 ralium-2.1.4/ralium/engine.py
--rw-rw-rw-   0        0        0     1389 2024-05-21 00:25:27.000000 ralium-2.1.4/ralium/engine.pyi
--rw-rw-rw-   0        0        0     1147 2024-05-27 18:22:26.000000 ralium-2.1.4/ralium/errors.py
--rw-rw-rw-   0        0        0     2387 2024-05-21 00:25:27.000000 ralium-2.1.4/ralium/listener.py
--rw-rw-rw-   0        0        0      890 2024-05-21 00:25:27.000000 ralium-2.1.4/ralium/listener.pyi
--rw-rw-rw-   0        0        0      804 2024-05-21 00:25:27.000000 ralium-2.1.4/ralium/navigation.py
--rw-rw-rw-   0        0        0      376 2024-05-21 00:25:27.000000 ralium-2.1.4/ralium/navigation.pyi
--rw-rw-rw-   0        0        0     4847 2024-05-28 23:54:13.000000 ralium-2.1.4/ralium/pyhtml.py
--rw-rw-rw-   0        0        0      531 2024-05-21 07:20:26.000000 ralium-2.1.4/ralium/pyhtml.pyi
--rw-rw-rw-   0        0        0     7678 2024-05-28 23:49:25.000000 ralium-2.1.4/ralium/setuptools.py
--rw-rw-rw-   0        0        0      959 2024-05-28 23:49:19.000000 ralium-2.1.4/ralium/setuptools.pyi
--rw-rw-rw-   0        0        0     6471 2024-05-29 00:21:58.000000 ralium-2.1.4/ralium/webpage.py
--rw-rw-rw-   0        0        0     1870 2024-05-21 00:26:03.000000 ralium-2.1.4/ralium/webpage.pyi
--rw-rw-rw-   0        0        0     6078 2024-05-29 00:22:41.000000 ralium-2.1.4/ralium/window.py
--rw-rw-rw-   0        0        0      693 2024-05-21 00:25:27.000000 ralium-2.1.4/ralium/window.pyi
-drwxrwxrwx   0        0        0        0 2024-05-29 20:36:17.803844 ralium-2.1.4/ralium.egg-info/
--rw-rw-rw-   0        0        0    41897 2024-05-29 20:36:17.000000 ralium-2.1.4/ralium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      692 2024-05-29 20:36:17.000000 ralium-2.1.4/ralium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 20:36:17.000000 ralium-2.1.4/ralium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 20:36:17.000000 ralium-2.1.4/ralium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-29 20:36:17.000000 ralium-2.1.4/ralium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 20:36:17.806156 ralium-2.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-30 22:17:43.562978 ralium-2.1.5/
+-rw-rw-rw-   0        0        0    35823 2024-05-21 00:22:26.000000 ralium-2.1.5/LICENSE
+-rw-rw-rw-   0        0        0    41897 2024-05-30 22:17:43.562978 ralium-2.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2024-05-21 00:22:26.000000 ralium-2.1.5/README.md
+-rw-rw-rw-   0        0        0      970 2024-05-30 22:15:49.000000 ralium-2.1.5/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-30 22:17:43.542141 ralium-2.1.5/ralium/
+-rw-rw-rw-   0        0        0      357 2024-05-21 05:00:06.000000 ralium-2.1.5/ralium/__init__.py
+-rw-rw-rw-   0        0        0     2911 2024-05-30 22:15:54.000000 ralium-2.1.5/ralium/_util.py
+-rw-rw-rw-   0        0        0     1410 2024-05-30 22:16:28.000000 ralium-2.1.5/ralium/_util.pyi
+-rw-rw-rw-   0        0        0     7555 2024-05-29 00:26:49.000000 ralium-2.1.5/ralium/api.py
+-rw-rw-rw-   0        0        0     1066 2024-05-21 00:25:27.000000 ralium-2.1.5/ralium/api.pyi
+-rw-rw-rw-   0        0        0      680 2024-05-21 00:25:27.000000 ralium-2.1.5/ralium/builtins.py
+-rw-rw-rw-   0        0        0      541 2024-05-21 00:25:27.000000 ralium-2.1.5/ralium/builtins.pyi
+-rw-rw-rw-   0        0        0     9678 2024-05-30 21:55:41.000000 ralium-2.1.5/ralium/bundle.py
+-rw-rw-rw-   0        0        0     1958 2024-05-29 00:37:29.000000 ralium-2.1.5/ralium/bundle.pyi
+-rw-rw-rw-   0        0        0     3332 2024-05-21 00:25:27.000000 ralium-2.1.5/ralium/config.py
+-rw-rw-rw-   0        0        0      467 2024-05-21 00:25:27.000000 ralium-2.1.5/ralium/config.pyi
+-rw-rw-rw-   0        0        0     6425 2024-05-21 00:25:27.000000 ralium-2.1.5/ralium/element.py
+-rw-rw-rw-   0        0        0     1376 2024-05-21 00:26:03.000000 ralium-2.1.5/ralium/element.pyi
+-rw-rw-rw-   0        0        0     4402 2024-05-21 00:26:03.000000 ralium-2.1.5/ralium/engine.py
+-rw-rw-rw-   0        0        0     1389 2024-05-21 00:25:27.000000 ralium-2.1.5/ralium/engine.pyi
+-rw-rw-rw-   0        0        0     1147 2024-05-27 18:22:26.000000 ralium-2.1.5/ralium/errors.py
+-rw-rw-rw-   0        0        0     2387 2024-05-21 00:25:27.000000 ralium-2.1.5/ralium/listener.py
+-rw-rw-rw-   0        0        0      890 2024-05-21 00:25:27.000000 ralium-2.1.5/ralium/listener.pyi
+-rw-rw-rw-   0        0        0      804 2024-05-21 00:25:27.000000 ralium-2.1.5/ralium/navigation.py
+-rw-rw-rw-   0        0        0      376 2024-05-21 00:25:27.000000 ralium-2.1.5/ralium/navigation.pyi
+-rw-rw-rw-   0        0        0     5543 2024-05-30 22:09:24.000000 ralium-2.1.5/ralium/pyhtml.py
+-rw-rw-rw-   0        0        0      531 2024-05-21 07:20:26.000000 ralium-2.1.5/ralium/pyhtml.pyi
+-rw-rw-rw-   0        0        0     7678 2024-05-30 21:56:28.000000 ralium-2.1.5/ralium/setuptools.py
+-rw-rw-rw-   0        0        0      959 2024-05-28 23:49:19.000000 ralium-2.1.5/ralium/setuptools.pyi
+-rw-rw-rw-   0        0        0     6471 2024-05-29 00:21:58.000000 ralium-2.1.5/ralium/webpage.py
+-rw-rw-rw-   0        0        0     1870 2024-05-21 00:26:03.000000 ralium-2.1.5/ralium/webpage.pyi
+-rw-rw-rw-   0        0        0     6078 2024-05-29 00:22:41.000000 ralium-2.1.5/ralium/window.py
+-rw-rw-rw-   0        0        0      693 2024-05-21 00:25:27.000000 ralium-2.1.5/ralium/window.pyi
+drwxrwxrwx   0        0        0        0 2024-05-30 22:17:43.561643 ralium-2.1.5/ralium.egg-info/
+-rw-rw-rw-   0        0        0    41897 2024-05-30 22:17:43.000000 ralium-2.1.5/ralium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      692 2024-05-30 22:17:43.000000 ralium-2.1.5/ralium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 22:17:43.000000 ralium-2.1.5/ralium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 22:17:43.000000 ralium-2.1.5/ralium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-30 22:17:43.000000 ralium-2.1.5/ralium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 22:17:43.562978 ralium-2.1.5/setup.cfg
```

### Comparing `ralium-2.1.4/LICENSE` & `ralium-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ralium-2.1.4/PKG-INFO` & `ralium-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 2.1.4
+Version: 2.1.5
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-2.1.4/pyproject.toml` & `ralium-2.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools >= 69.5.0", "wheel >= 0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ralium"
-version = "2.1.4"
+version = "2.1.5"
 description = "An easy to use wrapper for pywebview."
 readme = "README.md"
 authors = [{ name = "Isaiah Coroama", email = "coroamaisaiah@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

### Comparing `ralium-2.1.4/ralium/_util.py` & `ralium-2.1.5/ralium/_util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 import http.server
 import string
 import sys
 import os
 
 __all__ = [
-    "__version__", "SYS_PATH_SEPERATOR", "SYS_PATH_SEPERATOR", "BasicHTTPServer", "NamedDict", 
-    "_get_http_server_handler", "_get_bundle", "_norm_url", "_norm_path", "_check_exists",  
-    "_check_is_dir", "_read_file", "_get_path"
+    "__version__", "SYS_PATH_SEPERATOR", "SYS_PATH_SEPERATOR", "BACKSLASH", "BasicHTTPServer", 
+    "NamedDict", "_get_http_server_handler", "_get_bundle", "_norm_url", "_norm_path", 
+    "_check_exists", "_check_is_dir", "_read_file", "_get_path"
 ]
 
-__version__ = "2.1.4"
+__version__ = "2.1.5"
+
+# Used for backwards compatibility with Python versions below 3.12.
+# Older versions raise a SyntaxError when you try to include a plain
+# backslash ('\') in an f-string, like: f"{'\\'.join(...)}". 
+# Using f"{BACKSLASH.join(...)}" instead circumvents this problem.
+BACKSLASH = "\\"
 
 SYS_BUNDLE_ATTRIBUTE = "bundled"
 SYS_PATH_SEPERATOR = "\\" if sys.platform.startswith("win") else "/"
 
 class BasicHTTPServer(http.server.SimpleHTTPRequestHandler):
     pass
 
@@ -21,14 +27,19 @@
     def __init__(self, iterable):
         for key, value in iterable.items():
             if isinstance(value, dict):
                 self[key] = NamedDict(value)
                 continue
 
             self[key] = value
+    
+    def __getattr__(self, name):
+        if not super().__contains__(name):
+            raise AttributeError(f"Object does not contain value '{name}'")
+        return super().__getitem__(name)
 
 def _is_abs_win(path):
     if not sys.platform.startswith("win"):
         return False
 
     for letter in string.ascii_uppercase:
         if path.startswith(f"{letter}:"):
@@ -59,20 +70,20 @@
 
     if bundle is not None:
         return path in bundle.dirs
     
     return os.path.isdir(path)
 
 def _norm_url(path):
-    return os.path.normpath(f"/{path.lstrip('/\\')}").replace("\\", "/")
+    return os.path.normpath(f"/{path.lstrip(f'/{BACKSLASH}')}").replace(BACKSLASH, "/")
 
 def _norm_path(path):
     if _is_abs_win(path):
         return path
-    return os.path.normpath(f"{SYS_PATH_SEPERATOR}{path.lstrip('/\\')}").replace("/", SYS_PATH_SEPERATOR)
+    return os.path.normpath(f"{SYS_PATH_SEPERATOR}{path.lstrip(f'/{BACKSLASH}')}").replace("/", SYS_PATH_SEPERATOR)
 
 def _read_file(path, encoding = "UTF-8"):
     bundle = _get_bundle()
 
     if bundle is not None:
         return bundle.open(path).decode(encoding)
```

### Comparing `ralium-2.1.4/ralium/_util.pyi` & `ralium-2.1.5/ralium/_util.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -13,33 +13,35 @@
     FunctionType, 
     ModuleType
 )
 
 import http.server
 
 __all__ = [
-    "__version__", "SYS_PATH_SEPERATOR", "SYS_PATH_SEPERATOR", "BasicHTTPServer", "NamedDict", 
+    "__version__", "SYS_PATH_SEPERATOR", "SYS_PATH_SEPERATOR", "BACKSLASH", "BasicHTTPServer", "NamedDict", 
     "_get_http_server_handler", "_get_bundle", "_norm_url", "_norm_path", "_check_exists",  
     "_check_is_dir", "_read_file", "_get_path"
 ]
 
 __version__: str
 
+BACKSLASH: Literal["\\"]
 SYS_BUNDLE_ATTRIBUTE: str
 SYS_PATH_SEPERATOR: Literal["\\"] | Literal["/"]
 
 _RT = TypeVar("_RT") # Return Type
 ClassType: TypeAlias = object
 DirPathStr: TypeAlias = str
 FilePathStr: TypeAlias = str
 
 class BasicHTTPServer(http.server.SimpleHTTPRequestHandler): ...
 
 class NamedDict(dict):
     def __init__(self, iterable: dict[str, Any]) -> None: ...
+    def __getattr__(self, name: str) -> Any: ...
 
 def _is_abs_win(path: str) -> bool: ...
 def _get_bundle() -> FileSystem | None: ...
 def _get_http_server_handler() -> BasicHTTPServer | BundledHTTPServer: ...
 def _check_exists(path: str) -> bool: ...
 def _check_is_dir(path: str) -> bool: ...
 def _norm_url(path: str) -> str: ...
```

### Comparing `ralium-2.1.4/ralium/api.py` & `ralium-2.1.5/ralium/api.py`

 * *Files identical despite different names*

### Comparing `ralium-2.1.4/ralium/api.pyi` & `ralium-2.1.5/ralium/api.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.1.4/ralium/builtins.py` & `ralium-2.1.5/ralium/builtins.py`

 * *Files identical despite different names*

### Comparing `ralium-2.1.4/ralium/builtins.pyi` & `ralium-2.1.5/ralium/builtins.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.1.4/ralium/bundle.py` & `ralium-2.1.5/ralium/bundle.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
     _check_web_folder,
     _check_web_routes
 )
 
 from ralium._util import (
     SYS_BUNDLE_ATTRIBUTE,
     SYS_PATH_SEPERATOR,
+    BACKSLASH,
     _get_bundle,
     _get_path,
     _norm_url
 )
 
 from shutil import COPY_BUFSIZE
 from http import HTTPStatus
@@ -120,15 +121,16 @@
         self.relpath = relpath
         self.content = content
     
     def __str__(self):
         return self.content.decode()
 
     def __repr__(self):
-        return f"ralium.bundle.File(relpath='{self.relpath.replace('\\', '\\\\')}', content={repr(self.content)})"
+        DOUBLE_BACKSLASH = "\\\\"
+        return f"ralium.bundle.File(relpath='{self.relpath.replace(BACKSLASH, DOUBLE_BACKSLASH)}', content={repr(self.content)})"
     
 class Bundle:
     __slots__ = ("url", "page", "server", "styles",)
 
     def __init__(self, *, url, page, server, styles):
         self.url = url
         self.page = page
@@ -142,15 +144,15 @@
     __slots__ = ("images", "styles", "bundles", "dirs", "files",)
 
     def __init__(self, *, images, styles, bundles):
         self.images = images
         self.styles = styles
         self.bundles = bundles
 
-        self.dirs = ["\\"]
+        self.dirs = [SYS_PATH_SEPERATOR]
         self.files = {}
 
         for image in images:
             self.__add_file(image)
 
         for style in styles:
             self.__add_file(style)
```

### Comparing `ralium-2.1.4/ralium/bundle.pyi` & `ralium-2.1.5/ralium/bundle.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.1.4/ralium/config.py` & `ralium-2.1.5/ralium/config.py`

 * *Files identical despite different names*

### Comparing `ralium-2.1.4/ralium/element.py` & `ralium-2.1.5/ralium/element.py`

 * *Files identical despite different names*

### Comparing `ralium-2.1.4/ralium/element.pyi` & `ralium-2.1.5/ralium/element.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.1.4/ralium/engine.py` & `ralium-2.1.5/ralium/engine.py`

 * *Files identical despite different names*

### Comparing `ralium-2.1.4/ralium/engine.pyi` & `ralium-2.1.5/ralium/engine.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.1.4/ralium/errors.py` & `ralium-2.1.5/ralium/errors.py`

 * *Files identical despite different names*

### Comparing `ralium-2.1.4/ralium/listener.py` & `ralium-2.1.5/ralium/listener.py`

 * *Files identical despite different names*

### Comparing `ralium-2.1.4/ralium/listener.pyi` & `ralium-2.1.5/ralium/listener.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.1.4/ralium/navigation.py` & `ralium-2.1.5/ralium/navigation.py`

 * *Files identical despite different names*

### Comparing `ralium-2.1.4/ralium/pyhtml.py` & `ralium-2.1.5/ralium/pyhtml.py`

 * *Files 21% similar despite different names*

```diff
@@ -43,35 +43,39 @@
 
         :returns: A list of processed code blocks as strings.
         """
 
         data = []
 
         for block in blocks:
-            lines = []
-            
-            for line in block.split("\n")[1:-1]:
-                tags = re.findall(RE_HTML_PATTERN, line)
-                
-                if not tags: 
-                    lines.append(line)
-                    continue
-
-                for tag in tags:
-                    tag = tag[0]
-                    rep = tag
-
-                    if rep.startswith('<">') and rep.endswith('</">'):
-                        rep = rep.removeprefix('<">')
-                        rep = rep.removesuffix('</">')
+            block = PyHTML.removeaffix(block, "{%ralium", "%}")
+            html = PyHTML.get_enclosed(block, "{$html", "$}")
 
-                    rep = rep.replace('"', '\\"')
-                    lines.append(line.replace(tag, f'__ralium_html__.append("{rep}")'))
+            if not html:
+                lines = []
+                
+                for line in block.split("\n"):
+                    tags = re.findall(RE_HTML_PATTERN, line)
+                    
+                    if not tags: 
+                        lines.append(line)
+                        continue
+
+                    for tag in tags:
+                        rep = PyHTML.removeaffix(tag[0], '<">', '</">').replace('"', '\\"')
+                        lines.append(line.replace(tag[0], f'__ralium_html__.append("{rep}")'))
+                
+                data.append("\n".join(lines))
+                continue
+            
+            for tag in html:
+                rep = PyHTML.removeaffix(tag, "{$html", "$}").replace('"', '\\"')
+                block = block.replace(tag, f'__ralium_html__.append("""{rep}""")')
             
-            data.append("\n".join(lines))
+            data.append(block)
         
         return data
     
     @staticmethod
     def locals(webhook):
         """
         Creates a locals dictionary from a `WebHook` object.
@@ -132,8 +136,22 @@
 
             if _end == -1:
                 raise PyHTMLSyntaxError(f"Missing ending symbol '{end}'")
             
             _end += len(end)
             found.append(text[_start:_end])
         
-        return found
+        return found
+
+    @staticmethod
+    def removeaffix(text, prefix, suffix):
+        """
+        Removes a prefix and a suffix from a string.
+
+        :param text: The string to process.
+        :param prefix: The prefix to remove.
+        :param suffix: The suffix to remove.
+
+        :returns: The string without the specified prefix and suffix.
+        """
+
+        return text.removeprefix(prefix).removesuffix(suffix)
```

### Comparing `ralium-2.1.4/ralium/pyhtml.pyi` & `ralium-2.1.5/ralium/pyhtml.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.1.4/ralium/setuptools.py` & `ralium-2.1.5/ralium/setuptools.py`

 * *Files identical despite different names*

### Comparing `ralium-2.1.4/ralium/setuptools.pyi` & `ralium-2.1.5/ralium/setuptools.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.1.4/ralium/webpage.py` & `ralium-2.1.5/ralium/webpage.py`

 * *Files identical despite different names*

### Comparing `ralium-2.1.4/ralium/webpage.pyi` & `ralium-2.1.5/ralium/webpage.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.1.4/ralium/window.py` & `ralium-2.1.5/ralium/window.py`

 * *Files identical despite different names*

### Comparing `ralium-2.1.4/ralium/window.pyi` & `ralium-2.1.5/ralium/window.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.1.4/ralium.egg-info/PKG-INFO` & `ralium-2.1.5/ralium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 2.1.4
+Version: 2.1.5
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-2.1.4/ralium.egg-info/SOURCES.txt` & `ralium-2.1.5/ralium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

