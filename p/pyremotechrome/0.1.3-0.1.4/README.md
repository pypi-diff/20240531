# Comparing `tmp/pyremotechrome-0.1.3.tar.gz` & `tmp/pyremotechrome-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyremotechrome-0.1.3.tar", last modified: Tue May 28 14:33:31 2024, max compression
+gzip compressed data, was "pyremotechrome-0.1.4.tar", last modified: Fri May 31 11:15:39 2024, max compression
```

## Comparing `pyremotechrome-0.1.3.tar` & `pyremotechrome-0.1.4.tar`

### file list

```diff
@@ -1,42 +1,47 @@
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-28 14:33:31.422877 pyremotechrome-0.1.3/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1063 2024-05-22 13:27:37.000000 pyremotechrome-0.1.3/LICENSE
--rw-r--r--   0 wes       (1000) wes       (1000)      979 2024-05-28 14:33:31.422877 pyremotechrome-0.1.3/PKG-INFO
--rwxrwxr-x   0 wes       (1000) wes       (1000)      114 2024-05-22 14:14:51.000000 pyremotechrome-0.1.3/README.md
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1094 2024-05-28 14:33:28.000000 pyremotechrome-0.1.3/pyproject.toml
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-28 14:33:31.418877 pyremotechrome-0.1.3/pyremotechrome/
--rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-22 04:06:17.000000 pyremotechrome-0.1.3/pyremotechrome/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1846 2024-05-24 06:21:51.000000 pyremotechrome-0.1.3/pyremotechrome/__main__.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-28 14:33:31.418877 pyremotechrome-0.1.3/pyremotechrome/config/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1131 2024-05-24 04:08:11.000000 pyremotechrome-0.1.3/pyremotechrome/config/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     2099 2024-05-25 05:57:55.000000 pyremotechrome-0.1.3/pyremotechrome/config/config.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-28 14:33:31.422877 pyremotechrome-0.1.3/pyremotechrome/server/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-21 12:28:42.000000 pyremotechrome-0.1.3/pyremotechrome/server/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     4286 2024-05-21 12:36:41.000000 pyremotechrome-0.1.3/pyremotechrome/server/favicon.ico
--rw-rw-r--   0 wes       (1000) wes       (1000)     7462 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/server/manager.py
--rwxrwxr-x   0 wes       (1000) wes       (1000)     4635 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/server/server.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-28 14:33:31.422877 pyremotechrome-0.1.3/pyremotechrome/session/
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1179 2024-05-24 03:49:59.000000 pyremotechrome-0.1.3/pyremotechrome/session/__init__.py
--rwxrwxr-x   0 wes       (1000) wes       (1000)    16074 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/session/base.py
--rwxrwxr-x   0 wes       (1000) wes       (1000)     2893 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/session/mega.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-28 14:33:31.422877 pyremotechrome-0.1.3/pyremotechrome/session/monitor/
--rwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/session/monitor/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     7026 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/session/monitor/audio.py
--rwxrwxr-x   0 wes       (1000) wes       (1000)     5187 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/session/monitor/display.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-28 14:33:31.418877 pyremotechrome-0.1.3/pyremotechrome/session/support/
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-28 14:33:31.422877 pyremotechrome-0.1.3/pyremotechrome/session/support/common/
--rwxrwxr-x   0 wes       (1000) wes       (1000)     1344 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/session/support/common/__init__.py
--rwxrwxr-x   0 wes       (1000) wes       (1000)     2435 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/session/support/common/directory.py
--rwxrwxr-x   0 wes       (1000) wes       (1000)     1752 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/session/support/common/info.py
--rwxrwxr-x   0 wes       (1000) wes       (1000)     1451 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/session/support/common/result.py
--rwxrwxr-x   0 wes       (1000) wes       (1000)     1713 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/session/support/common/vector.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-28 14:33:31.422877 pyremotechrome-0.1.3/pyremotechrome/session/support/options/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1167 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/session/support/options/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1493 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/session/support/options/ffmpeg.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     3797 2024-05-26 04:51:07.000000 pyremotechrome-0.1.3/pyremotechrome/util.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-28 14:33:31.422877 pyremotechrome-0.1.3/pyremotechrome.egg-info/
--rw-r--r--   0 wes       (1000) wes       (1000)      979 2024-05-28 14:33:31.000000 pyremotechrome-0.1.3/pyremotechrome.egg-info/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)     1062 2024-05-28 14:33:31.000000 pyremotechrome-0.1.3/pyremotechrome.egg-info/SOURCES.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)        1 2024-05-28 14:33:31.000000 pyremotechrome-0.1.3/pyremotechrome.egg-info/dependency_links.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       83 2024-05-28 14:33:31.000000 pyremotechrome-0.1.3/pyremotechrome.egg-info/requires.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       20 2024-05-28 14:33:31.000000 pyremotechrome-0.1.3/pyremotechrome.egg-info/top_level.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       38 2024-05-28 14:33:31.422877 pyremotechrome-0.1.3/setup.cfg
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-31 11:15:39.525024 pyremotechrome-0.1.4/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1063 2024-05-22 13:27:37.000000 pyremotechrome-0.1.4/LICENSE
+-rw-r--r--   0 wes       (1000) wes       (1000)     4462 2024-05-31 11:15:39.525024 pyremotechrome-0.1.4/PKG-INFO
+-rwxrwxr-x   0 wes       (1000) wes       (1000)     3598 2024-05-31 11:15:28.000000 pyremotechrome-0.1.4/README.md
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-31 11:15:39.525024 pyremotechrome-0.1.4/dist/
+-rw-rw-r--   0 wes       (1000) wes       (1000)    33288 2024-05-28 14:33:35.000000 pyremotechrome-0.1.4/dist/pyremotechrome-0.1.3-py3-none-any.whl
+-rw-rw-r--   0 wes       (1000) wes       (1000)    18120 2024-05-28 14:33:31.000000 pyremotechrome-0.1.4/dist/pyremotechrome-0.1.3.tar.gz
+-rw-rw-r--   0 wes       (1000) wes       (1000)   535284 2024-05-31 11:12:05.000000 pyremotechrome-0.1.4/dist/pyremotechrome-0.1.4-py3-none-any.whl
+-rw-rw-r--   0 wes       (1000) wes       (1000)   522703 2024-05-31 11:12:02.000000 pyremotechrome-0.1.4/dist/pyremotechrome-0.1.4.tar.gz
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1094 2024-05-31 10:45:38.000000 pyremotechrome-0.1.4/pyproject.toml
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-31 11:15:39.525024 pyremotechrome-0.1.4/pyremotechrome/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-22 04:06:17.000000 pyremotechrome-0.1.4/pyremotechrome/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1846 2024-05-29 04:46:14.000000 pyremotechrome-0.1.4/pyremotechrome/__main__.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-31 11:15:39.525024 pyremotechrome-0.1.4/pyremotechrome/config/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1131 2024-05-24 04:08:11.000000 pyremotechrome-0.1.4/pyremotechrome/config/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2099 2024-05-25 05:57:55.000000 pyremotechrome-0.1.4/pyremotechrome/config/config.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-31 11:15:39.525024 pyremotechrome-0.1.4/pyremotechrome/server/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-21 12:28:42.000000 pyremotechrome-0.1.4/pyremotechrome/server/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     4286 2024-05-21 12:36:41.000000 pyremotechrome-0.1.4/pyremotechrome/server/favicon.ico
+-rw-rw-r--   0 wes       (1000) wes       (1000)     7462 2024-05-28 04:38:29.000000 pyremotechrome-0.1.4/pyremotechrome/server/manager.py
+-rwxrwxr-x   0 wes       (1000) wes       (1000)     4635 2024-05-28 04:38:29.000000 pyremotechrome-0.1.4/pyremotechrome/server/server.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-31 11:15:39.525024 pyremotechrome-0.1.4/pyremotechrome/session/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1179 2024-05-24 03:49:59.000000 pyremotechrome-0.1.4/pyremotechrome/session/__init__.py
+-rwxrwxr-x   0 wes       (1000) wes       (1000)    16178 2024-05-31 11:11:55.000000 pyremotechrome-0.1.4/pyremotechrome/session/base.py
+-rwxrwxr-x   0 wes       (1000) wes       (1000)     2893 2024-05-28 04:38:29.000000 pyremotechrome-0.1.4/pyremotechrome/session/mega.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-31 11:15:39.525024 pyremotechrome-0.1.4/pyremotechrome/session/monitor/
+-rwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-28 04:38:29.000000 pyremotechrome-0.1.4/pyremotechrome/session/monitor/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     7026 2024-05-28 04:38:29.000000 pyremotechrome-0.1.4/pyremotechrome/session/monitor/audio.py
+-rwxrwxr-x   0 wes       (1000) wes       (1000)     5242 2024-05-31 10:45:12.000000 pyremotechrome-0.1.4/pyremotechrome/session/monitor/display.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-31 11:15:39.517024 pyremotechrome-0.1.4/pyremotechrome/session/support/
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-31 11:15:39.525024 pyremotechrome-0.1.4/pyremotechrome/session/support/common/
+-rwxrwxr-x   0 wes       (1000) wes       (1000)     1344 2024-05-28 04:38:29.000000 pyremotechrome-0.1.4/pyremotechrome/session/support/common/__init__.py
+-rwxrwxr-x   0 wes       (1000) wes       (1000)     2435 2024-05-28 04:38:29.000000 pyremotechrome-0.1.4/pyremotechrome/session/support/common/directory.py
+-rwxrwxr-x   0 wes       (1000) wes       (1000)     1752 2024-05-28 04:38:29.000000 pyremotechrome-0.1.4/pyremotechrome/session/support/common/info.py
+-rwxrwxr-x   0 wes       (1000) wes       (1000)     1451 2024-05-28 04:38:29.000000 pyremotechrome-0.1.4/pyremotechrome/session/support/common/result.py
+-rwxrwxr-x   0 wes       (1000) wes       (1000)     1713 2024-05-28 04:38:29.000000 pyremotechrome-0.1.4/pyremotechrome/session/support/common/vector.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-31 11:15:39.525024 pyremotechrome-0.1.4/pyremotechrome/session/support/options/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1167 2024-05-28 04:38:29.000000 pyremotechrome-0.1.4/pyremotechrome/session/support/options/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1493 2024-05-28 04:38:29.000000 pyremotechrome-0.1.4/pyremotechrome/session/support/options/ffmpeg.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     3797 2024-05-26 04:51:07.000000 pyremotechrome-0.1.4/pyremotechrome/util.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-31 11:15:39.525024 pyremotechrome-0.1.4/pyremotechrome.egg-info/
+-rw-r--r--   0 wes       (1000) wes       (1000)     4462 2024-05-31 11:15:39.000000 pyremotechrome-0.1.4/pyremotechrome.egg-info/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1214 2024-05-31 11:15:39.000000 pyremotechrome-0.1.4/pyremotechrome.egg-info/SOURCES.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2024-05-31 11:15:39.000000 pyremotechrome-0.1.4/pyremotechrome.egg-info/dependency_links.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       83 2024-05-31 11:15:39.000000 pyremotechrome-0.1.4/pyremotechrome.egg-info/requires.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       26 2024-05-31 11:15:39.000000 pyremotechrome-0.1.4/pyremotechrome.egg-info/top_level.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       38 2024-05-31 11:15:39.525024 pyremotechrome-0.1.4/setup.cfg
```

### Comparing `pyremotechrome-0.1.3/LICENSE` & `pyremotechrome-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.3/pyproject.toml` & `pyremotechrome-0.1.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [metadata]
 name = "pyremotechrome"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.setuptools.packages]
 find = {}  # Scan the project directory with the default parameters
 
 [tool.setuptools.package-data]
 "*" = ["*.*"] # Include resources
 
 [project]
 name = "pyremotechrome"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Wes-KW", email="dotdotdashdash2024@hotmail.com" },
 ]
 dependencies = [
   "selenium>=4.19.0",
   "psutil>=5.9.8",
   "PyVirtualDisplay>=3.0",
```

### Comparing `pyremotechrome-0.1.3/pyremotechrome/__main__.py` & `pyremotechrome-0.1.4/pyremotechrome/__main__.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.3/pyremotechrome/config/__init__.py` & `pyremotechrome-0.1.4/pyremotechrome/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.3/pyremotechrome/config/config.py` & `pyremotechrome-0.1.4/pyremotechrome/config/config.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.3/pyremotechrome/server/favicon.ico` & `pyremotechrome-0.1.4/pyremotechrome/server/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.3/pyremotechrome/server/manager.py` & `pyremotechrome-0.1.4/pyremotechrome/server/manager.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.3/pyremotechrome/server/server.py` & `pyremotechrome-0.1.4/pyremotechrome/server/server.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.3/pyremotechrome/session/__init__.py` & `pyremotechrome-0.1.4/pyremotechrome/session/__init__.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.3/pyremotechrome/session/base.py` & `pyremotechrome-0.1.4/pyremotechrome/session/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 from pyremotechrome.session.support.common import Directory
 from pyremotechrome.session.support.common import Info
 from pyremotechrome.session.support.common import Vector
 from pyremotechrome.util import get_absolute_path
 from pyremotechrome.util import filter_rules
 from pyremotechrome.util import Numbers
 
-__CHROME_AUTOMATION_LABEL_HEIGHT__ = 6
 
 class Base(Chrome):
 
     _id: str
     _cursor: Vector
     _position: Vector
     _border_width: Vector
@@ -115,15 +114,14 @@
         bw, bh = self.execute_script("""
             var w=window;
             return [
                 w.outerWidth - w.innerWidth,
                 w.outerHeight - w.innerHeight
             ];
         """)
-        bh += __CHROME_AUTOMATION_LABEL_HEIGHT__
         self._border_width = Vector(bw, bh)
 
         width, height = size()
         self.set_window_size(width, height)
         self.set_window_position(0, 0)
         self.set_page_load_timeout(60)
         self.zoom()
@@ -167,15 +165,15 @@
         return width / self._scale, height / self._scale
 
     def set_window_size(self, width: Numbers, height: Numbers) -> None:
         """DOCSTRING"""
         x, y, bw, bh, _, _ = self.get_current_html_rect()()
         width = int(width * self._scale)
         height = int(height * self._scale)
-        super().set_window_size(width, height)
+        super().set_window_size(width + bw, height + bh)
         self.display.restart_capturing(x + bw, y + bh, width, height)
 
     # Window handle
     def get_current_window(self) -> str:
         """Return current window handle"""
         curr_handle = self.current_window_handle
         if curr_handle not in self.window_handles:
@@ -450,18 +448,23 @@
         except Exception:
             pass
 
     def hide_scrollbar(self) -> None:
         """DOCSTRING"""
         try:
             self.execute_script("""
-                if (document.styleSheets.length > 0){
-                    var sheet = document.styleSheets[0];
-                    var len = sheet.cssRules.length;
-                    sheet.insertRule('*{}', len);
-                    var rule = sheet.cssRules[len];
-                    rule.selectorText = 'body::-webkit-scrollbar';
-                    rule.style.display = 'none';
+                var slen = document.styleSheets.length;
+                for (var i=0;i<slen;i++){
+                    try {
+                        var sheet = document.styleSheets[i];
+                        var len = sheet.cssRules.length;
+                        sheet.insertRule('*{}', len);
+                        var rule = sheet.cssRules[len];
+                        rule.selectorText = 'body::-webkit-scrollbar';
+                        rule.style.display = 'none';
+                    } catch (error) {
+                           
+                    }
                 }
             """)
         except Exception:
             pass
```

### Comparing `pyremotechrome-0.1.3/pyremotechrome/session/mega.py` & `pyremotechrome-0.1.4/pyremotechrome/session/mega.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.3/pyremotechrome/session/monitor/audio.py` & `pyremotechrome-0.1.4/pyremotechrome/session/monitor/audio.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.3/pyremotechrome/session/monitor/display.py` & `pyremotechrome-0.1.4/pyremotechrome/session/monitor/display.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         self._log_file = None
         self.ffmpeg_options = None
         self._ffmpeg_process = None
 
         super().__init__(
             visible=False,
             size=(int(width * scale), int(height * scale)),
-            bgcolor="white",
+            bgcolor="black",
             extra_args=["-nocursor"]
         )
 
     def init_audio(self, browser_pid: int) -> None:
         """Set browser's sink input to the corresponding sink device"""
         self.audio_manager = Audio(browser_pid)
         self._sink_name = self.audio_manager.get_monitor()
@@ -95,19 +95,19 @@
             "-itsoffset", str(fg.audio_itsoffset), "-f", "pulse", "-i", f"{self._sink_name}"
         ])
 
         # combine audio and image and separate output
         proc_args.extend([
             "-f", "hls", "-hls_time", str(fg.segment_time), "-reset_timestamps",
             "1", "-g", str(frame_per_second * fg.segment_time), "-sc_threshold", "0",
-            "-force_key_frames",  f"expr:gte(t,n_forced*{fg.segment_time})", "-c:v",
-            "libx264", "-preset", "ultrafast", "-b:v", str(fg.maxrate), "-maxrate",
-            str(fg.maxrate), "-bufsize", str(fg.bufsize), "-pix_fmt", "yuv420p", "-crf",
-            str(fg.constant_rate_factor), "-c:a", "aac", "-preset", "ultrafast", "-tune",
-            "zerolatency", f"{self._video_dir}/.m3u8"
+            "-force_key_frames", f"expr:gte(t,n_forced*{fg.segment_time})", "-vf",
+            "drawbox=x=0:y=0:w=iw:h=6:color=white@1:t=fill", "-c:v", "libx264", "-preset",
+            "ultrafast", "-b:v", str(fg.maxrate), "-maxrate", str(fg.maxrate), "-bufsize",
+            str(fg.bufsize), "-pix_fmt", "yuv420p", "-crf", str(fg.constant_rate_factor), "-c:a",
+            "aac", "-preset", "ultrafast", "-tune", "zerolatency", f"{self._video_dir}/.m3u8"
         ])
 
         self._log_file = open(f"{self._log_dir}/{get_utc_timestr('%d.%b.%Y__%H_%M_%S')}.log", "w")
         self._ffmpeg_process = Popen(proc_args, stdout=self._log_file, stderr=STDOUT)
 
     def stop_capturing(self) -> None:
         """DOCSTRING"""
```

### Comparing `pyremotechrome-0.1.3/pyremotechrome/session/support/common/__init__.py` & `pyremotechrome-0.1.4/pyremotechrome/session/support/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.3/pyremotechrome/session/support/common/directory.py` & `pyremotechrome-0.1.4/pyremotechrome/session/support/common/directory.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.3/pyremotechrome/session/support/common/info.py` & `pyremotechrome-0.1.4/pyremotechrome/session/support/common/info.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.3/pyremotechrome/session/support/common/result.py` & `pyremotechrome-0.1.4/pyremotechrome/session/support/common/result.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.3/pyremotechrome/session/support/common/vector.py` & `pyremotechrome-0.1.4/pyremotechrome/session/support/common/vector.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.3/pyremotechrome/session/support/options/__init__.py` & `pyremotechrome-0.1.4/pyremotechrome/session/support/options/__init__.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.3/pyremotechrome/session/support/options/ffmpeg.py` & `pyremotechrome-0.1.4/pyremotechrome/session/support/options/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.3/pyremotechrome/util.py` & `pyremotechrome-0.1.4/pyremotechrome/util.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.3/pyremotechrome.egg-info/SOURCES.txt` & `pyremotechrome-0.1.4/pyremotechrome.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
+dist/pyremotechrome-0.1.3-py3-none-any.whl
+dist/pyremotechrome-0.1.3.tar.gz
+dist/pyremotechrome-0.1.4-py3-none-any.whl
+dist/pyremotechrome-0.1.4.tar.gz
 pyremotechrome/__init__.py
 pyremotechrome/__main__.py
 pyremotechrome/util.py
 pyremotechrome.egg-info/PKG-INFO
 pyremotechrome.egg-info/SOURCES.txt
 pyremotechrome.egg-info/dependency_links.txt
 pyremotechrome.egg-info/requires.txt
```

