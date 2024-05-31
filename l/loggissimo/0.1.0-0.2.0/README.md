# Comparing `tmp/loggissimo-0.1.0.tar.gz` & `tmp/loggissimo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggissimo-0.1.0.tar", last modified: Mon May 27 09:02:30 2024, max compression
+gzip compressed data, was "loggissimo-0.2.0.tar", last modified: Fri May 31 10:03:09 2024, max compression
```

## Comparing `loggissimo-0.1.0.tar` & `loggissimo-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 09:02:30.798428 loggissimo-0.1.0/
--rw-r--r--   0 root         (0) root         (0)      186 2024-05-27 09:02:30.798428 loggissimo-0.1.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)       12 2024-03-05 09:15:45.000000 loggissimo-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 09:02:30.798428 loggissimo-0.1.0/loggissimo/
--rw-rw-r--   0 root         (0) root         (0)       77 2024-05-27 09:02:28.000000 loggissimo-0.1.0/loggissimo/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    12483 2024-05-27 09:01:57.000000 loggissimo-0.1.0/loggissimo/_logger.py
--rwxrwxr-x   0 root         (0) root         (0)     2639 2024-05-27 07:44:47.000000 loggissimo-0.1.0/loggissimo/_style.py
--rw-rw-r--   0 root         (0) root         (0)     1496 2024-05-27 06:31:36.000000 loggissimo-0.1.0/loggissimo/_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 09:02:30.798428 loggissimo-0.1.0/loggissimo/colorizer/
--rw-rw-r--   0 root         (0) root         (0)      561 2024-05-27 06:34:49.000000 loggissimo-0.1.0/loggissimo/colorizer/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1006 2024-05-27 06:34:49.000000 loggissimo-0.1.0/loggissimo/colorizer/colorizer.py
--rw-rw-r--   0 root         (0) root         (0)      394 2024-05-27 06:31:45.000000 loggissimo-0.1.0/loggissimo/constants.py
--rw-rw-r--   0 root         (0) root         (0)      385 2024-05-27 06:31:48.000000 loggissimo-0.1.0/loggissimo/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 10:35:22.000000 loggissimo-0.1.0/loggissimo/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 09:02:30.798428 loggissimo-0.1.0/loggissimo.egg-info/
--rw-r--r--   0 root         (0) root         (0)      186 2024-05-27 09:02:30.000000 loggissimo-0.1.0/loggissimo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      387 2024-05-27 09:02:30.000000 loggissimo-0.1.0/loggissimo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 09:02:30.000000 loggissimo-0.1.0/loggissimo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-27 09:02:30.000000 loggissimo-0.1.0/loggissimo.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       63 2024-05-27 09:02:30.798428 loggissimo-0.1.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      373 2024-05-27 06:43:49.000000 loggissimo-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 10:03:09.324045 loggissimo-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1853 2024-05-31 10:03:09.324045 loggissimo-0.2.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)       12 2024-03-05 09:15:45.000000 loggissimo-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 10:03:09.324045 loggissimo-0.2.0/loggissimo/
+-rw-rw-r--   0 root         (0) root         (0)       77 2024-05-31 10:03:06.000000 loggissimo-0.2.0/loggissimo/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10122 2024-05-31 07:59:51.000000 loggissimo-0.2.0/loggissimo/_logger.py
+-rwxrwxr-x   0 root         (0) root         (0)     2946 2024-05-31 09:18:50.000000 loggissimo-0.2.0/loggissimo/_style.py
+-rw-rw-r--   0 root         (0) root         (0)     1496 2024-05-27 06:31:36.000000 loggissimo-0.2.0/loggissimo/_utils.py
+-rw-rw-r--   0 root         (0) root         (0)      394 2024-05-31 03:53:19.000000 loggissimo-0.2.0/loggissimo/constants.py
+-rw-rw-r--   0 root         (0) root         (0)      385 2024-05-27 06:31:48.000000 loggissimo-0.2.0/loggissimo/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 10:35:22.000000 loggissimo-0.2.0/loggissimo/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 10:03:09.324045 loggissimo-0.2.0/loggissimo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1853 2024-05-31 10:03:09.000000 loggissimo-0.2.0/loggissimo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      353 2024-05-31 10:03:09.000000 loggissimo-0.2.0/loggissimo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 10:03:09.000000 loggissimo-0.2.0/loggissimo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-31 10:03:09.000000 loggissimo-0.2.0/loggissimo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-31 10:03:09.000000 loggissimo-0.2.0/loggissimo.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       63 2024-05-31 10:03:09.324045 loggissimo-0.2.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      730 2024-05-31 10:02:27.000000 loggissimo-0.2.0/setup.py
```

### Comparing `loggissimo-0.1.0/loggissimo/_logger.py` & `loggissimo-0.2.0/loggissimo/_logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,41 +9,14 @@
 from typing import IO, Callable, Dict, List, Optional, Self, Tuple
 
 from ._style import style
 from .exceptions import LoggissimoError
 from .constants import DEFAULT_LOGGER_NAME, Level
 from ._utils import print_trace, get_module_combinations
 
-styles = {
-    Level.INFO: Template(
-        "<font=yellow>$name<font=green>$time<font=white style=bold>$level<font=cyan>$stack<font=white style=bold>$text"
-    ),
-    Level.SUCCESS: Template(
-        "<font=yellow>$name<font=green>$time<font=green style=bold>$level<font=cyan>$stack<font=green style=bold>$text"
-    ),
-    Level.DEBUG: Template(
-        "<font=yellow>$name<font=green>$time<font=blue style=bold>$level<font=cyan>$stack<font=blue style=bold>$text"
-    ),
-    Level.TRACE: Template(
-        "<font=yellow>$name<font=green>$time<font=cyan style=bold>$level<font=cyan>$stack<font=cyan style=bold>$text"
-    ),
-    Level.WARNING: Template(
-        "<font=yellow>$name<font=green>$time<font=yellow style=bold>$level<font=cyan>$stack<font=yellow style=bold>$text"
-    ),
-    Level.ERROR: Template(
-        "<font=yellow>$name<font=green>$time<font=red style=bold>$level<font=cyan>$stack<font=red style=bold>$text"
-    ),
-    Level.CRITICAL: Template(
-        "<font=yellow>$name<font=green>$time<font=white bg=red style=bold>$level<font=cyan>$stack<font=white style=bold>$text"
-    ),
-    Level.DELETE: Template(
-        "<font=yellow>$name<font=green>$time<font=purple style=bold>$level<font=cyan>$stack<font=purple style=bold>$text"
-    ),
-}
-
 
 class __LoggerMeta(type):
     _instances: WeakValueDictionary = WeakValueDictionary()
     lock = multiprocessing.Lock()
 
     def __call__(cls, name: str = DEFAULT_LOGGER_NAME, *args, **kwargs):
 
@@ -69,16 +42,18 @@
 
     def __new__(cls, *args, **kwargs) -> Self:
         return super().__new__(cls)
 
     def __init__(self, stream: IO = sys.stdout, *args, **kwargs) -> None:
         self._name_: str = kwargs.get("name", DEFAULT_LOGGER_NAME)
         self._force_colorize: bool = kwargs.get("force_colorize", False)
-        self._format: str = kwargs.get("format", "$name @ $time| $level | $stack:$text")
-        self._message_template = Template(f"{self._format}\n")
+        self._format: str = kwargs.get(
+            "format", "$name@ $time | $level | $stack: $text"
+        )
+        self._time_format = kwargs.get("time", "%Y-%m-%d %H:%M:%S")
         self._streams = {stream.name: stream}
         self._proc_name = ""
 
     def _check_threading(self) -> bool:
         """
         Determine whether the logger is in a thread
         """
@@ -124,76 +99,60 @@
                 return func(*args, **kwargs)
             except Exception as ex:
                 print_trace(ex)
 
         return _decorator
 
     def _log(self, level: Level, message: str):
-        def colorize(msg: str, do: bool = True):
-            msg_l = style(msg, not do)
-            iterator = iter(msg_l)
-            msg_values = {
-                "name": next(iterator, ""),
-                "time": next(iterator, ""),
-                "level": next(iterator, ""),
-                "stack": next(iterator, ""),
-                "text": next(iterator, ""),
-            }
-            return self._message_template.safe_substitute(**msg_values)
+        def colorize(do_not_colorize: bool):
+            msg_t = style(self._format, level, do_not_colorize)
+            return Template(msg_t).safe_substitute(
+                name=f"{name:30}",
+                time=f"{time}",
+                level=f"{level.name:<8}",
+                stack=f"{stack}",
+                text=f"{message}\n",
+            )
 
         self.in_thread = self._check_threading()
         time_now = datetime.now()
         frame = sys._getframe(3)
 
         try:
             module = frame.f_globals["__name__"]
         except KeyError:
             module = None
 
         if not self._is_enabled(level, module):
             return
 
-        raw_frame_line = f"{module}:{frame.f_code.co_name}:{frame.f_lineno}"
+        time = (
+            f"{'.' * len(self._time_format)}"
+            if level == Level.DELETE
+            else f"{time_now.strftime(self._time_format)}"
+        )
+
+        stack = f"{module}:{frame.f_code.co_name}:{frame.f_lineno}"
         name = (
             f"{self._name_:8} {f'({self._proc_name})':8}"
             if self._proc_name
             else f"{self._name_:12}"
         )
         name = name if self._name_ != DEFAULT_LOGGER_NAME else ""
-        levelname = str(level)
-        _message = message
-        msg = (
-            styles[level]
-            .safe_substitute(
-                name=f"{name:30}",
-                time=(
-                    f"{'.' * 19}"
-                    if level == Level.DELETE
-                    else f"{time_now.strftime('%Y-%m-%d %H:%M:%S'):19}"
-                ),
-                level=f"{levelname:<8}",
-                stack=f"{raw_frame_line:52}",
-                text=_message,
-            )
-            .lstrip()
-        )
-
-        msg_not_colored = colorize(msg, False)
-        msg_colored = colorize(msg)
 
         if not self._streams:
             raise LoggissimoError(
                 "No streams found. It could have happened that you cleared the list of streams and then did not add a stream."
             )
 
         for stream in self._streams.values():
             if self._force_colorize or stream.name == "<stdout>":
-                stream.write(msg_colored)
+                stream.write(colorize(False))
                 continue
-            stream.write(msg_not_colored)
+            stream.write(colorize(True))
 
     def _change_module_status(
         self, module: Optional[str], action: bool, path: str = ""
     ):
         if module in _Logger._modules.keys():
             _Logger._modules[module] = (_Logger._modules[module][0], action)
             return
@@ -250,33 +209,14 @@
     def level(self, level: Level | str) -> None:
         if hasattr(self, "_cached_level"):
             _Logger._cached_level.clear()
         if isinstance(level, str):
             level = Level[level]
         _Logger._level = level
 
-    @property
-    def format(self) -> str:
-        """
-        Set logger format. String of the form:
-        '$instance_name $time | $level | $program_line - $message'
-        Where optional parameters:
-            $instance_name - name of logger instance;
-            $time - message time;
-            $level - log level;
-            $program_line - the line in which the message is called;
-            $message - log message;
-        """
-        return self._format
-
-    @format.setter
-    def format(self, format: str) -> None:
-        self._format = format
-        self._message_template = Template(f"{self._format}")
-
     def enable(self, module: Optional[str] = None) -> None:
         self._change_module_status(module, True)
 
     def disable(self) -> None:
         frame = inspect.stack()[1]
         module = inspect.getmodule(frame[0])
 
@@ -320,15 +260,15 @@
 
     @_Logger._catch
     def destructor(self, message: str = "") -> None:
         self._log(Level.DELETE, message)
 
     @classmethod
     @_Logger._catch
-    def addall(cls, stream: IO | str) -> None:
+    def addall(cls, stream: IO | str, format: str = "") -> None:
         """
         Add stream to ALL logger instances.
 
         Args
         ----
             stream (IO | str): IO object or filename.
         """
@@ -341,15 +281,15 @@
 
         cls._aggregated_streams[stream.name] = stream
 
         for instance in cls._instances.values():
             instance._streams[stream.name] = stream
 
     @_Logger._catch
-    def add(self, stream: IO | str) -> None:
+    def add(self, stream: IO | str, format: str = "") -> None:
         """
         Add stream to logger instance output.
 
         Args
         ----
             stream (IO | str): IO object or filename.
         """
```

### Comparing `loggissimo-0.1.0/loggissimo/_utils.py` & `loggissimo-0.2.0/loggissimo/_utils.py`

 * *Files identical despite different names*

