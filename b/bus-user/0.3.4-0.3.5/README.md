# Comparing `tmp/bus_user-0.3.4.tar.gz` & `tmp/bus_user-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bus_user-0.3.4.tar", last modified: Wed May 29 14:44:28 2024, max compression
+gzip compressed data, was "bus_user-0.3.5.tar", last modified: Fri May 31 12:02:11 2024, max compression
```

## Comparing `bus_user-0.3.4.tar` & `bus_user-0.3.5.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 14:44:28.283771 bus_user-0.3.4/
--rw-rw-rw-   0        0        0     1082 2023-12-11 08:31:15.000000 bus_user-0.3.4/LICENSE
--rw-rw-rw-   0        0        0     4169 2024-05-29 14:44:28.282772 bus_user-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     3204 2024-05-29 14:44:03.000000 bus_user-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 14:44:28.274251 bus_user-0.3.4/bus_user/
--rw-rw-rw-   0        0        0     2286 2024-05-24 09:30:08.000000 bus_user-0.3.4/bus_user/__init__.py
--rw-rw-rw-   0        0        0     3366 2023-12-14 12:44:59.000000 bus_user-0.3.4/bus_user/history.py
--rw-rw-rw-   0        0        0     3761 2024-05-24 09:30:08.000000 bus_user-0.3.4/bus_user/i2c_client.py
--rw-rw-rw-   0        0        0     2158 2024-05-24 09:19:18.000000 bus_user-0.3.4/bus_user/line_parser.py
--rw-rw-rw-   0        0        0    40675 2024-05-29 14:13:02.000000 bus_user-0.3.4/bus_user/serial_client.py
--rw-rw-rw-   0        0        0      711 2024-05-24 15:12:34.000000 bus_user-0.3.4/bus_user/serial_derivatives.py
--rw-rw-rw-   0        0        0    18620 2024-05-29 14:36:15.000000 bus_user-0.3.4/bus_user/serial_server.py
--rw-rw-rw-   0        0        0     6032 2024-05-24 09:11:17.000000 bus_user-0.3.4/bus_user/values.py
-drwxrwxrwx   0        0        0        0 2024-05-29 14:44:28.281694 bus_user-0.3.4/bus_user.egg-info/
--rw-rw-rw-   0        0        0     4169 2024-05-29 14:44:28.000000 bus_user-0.3.4/bus_user.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-05-29 14:44:28.000000 bus_user-0.3.4/bus_user.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 14:44:28.000000 bus_user-0.3.4/bus_user.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-29 14:44:28.000000 bus_user-0.3.4/bus_user.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 14:44:28.284271 bus_user-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 bus_user-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:02:11.550973 bus_user-0.3.5/
+-rw-rw-rw-   0        0        0     1082 2023-12-11 08:31:15.000000 bus_user-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0     4169 2024-05-31 12:02:11.550973 bus_user-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3204 2024-05-31 11:59:33.000000 bus_user-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 12:02:11.545672 bus_user-0.3.5/bus_user/
+-rw-rw-rw-   0        0        0     2077 2024-05-31 07:59:53.000000 bus_user-0.3.5/bus_user/__init__.py
+-rw-rw-rw-   0        0        0     3366 2023-12-14 12:44:59.000000 bus_user-0.3.5/bus_user/history.py
+-rw-rw-rw-   0        0        0     3761 2024-05-24 09:30:08.000000 bus_user-0.3.5/bus_user/i2c_client.py
+-rw-rw-rw-   0        0        0     2158 2024-05-24 09:19:18.000000 bus_user-0.3.5/bus_user/line_parser.py
+-rw-rw-rw-   0        0        0    41851 2024-05-31 10:37:16.000000 bus_user-0.3.5/bus_user/serial_client.py
+-rw-rw-rw-   0        0        0      711 2024-05-24 15:12:34.000000 bus_user-0.3.5/bus_user/serial_derivatives.py
+-rw-rw-rw-   0        0        0    18547 2024-05-31 07:59:53.000000 bus_user-0.3.5/bus_user/serial_server.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:02:11.550973 bus_user-0.3.5/bus_user.egg-info/
+-rw-rw-rw-   0        0        0     4169 2024-05-31 12:02:11.000000 bus_user-0.3.5/bus_user.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2024-05-31 12:02:11.000000 bus_user-0.3.5/bus_user.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 12:02:11.000000 bus_user-0.3.5/bus_user.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-31 12:02:11.000000 bus_user-0.3.5/bus_user.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 12:02:11.551975 bus_user-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 bus_user-0.3.5/setup.py
```

### Comparing `bus_user-0.3.4/LICENSE` & `bus_user-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.4/PKG-INFO` & `bus_user-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bus_user
-Version: 0.3.4
+Version: 0.3.5
 Summary: work with equipment over buses like Serial/i2c/... as client and server
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/bus_user
 Keywords: serial,serial bus,pyserial,serial port,com port,comport,rs232,UART,TTL,serial client,serial server,serial emulator,i2c
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# bus_user (v0.3.4)
+# bus_user (v0.3.5)
 
 ## DESCRIPTION_SHORT
 work with equipment over buses like Serial/i2c/... as client and server
 
 ## DESCRIPTION_LONG
 ###
 NOTE: IT SEEMS THIS IS OLD DATA! see tests for actual usage!
```

### Comparing `bus_user-0.3.4/README.md` & `bus_user-0.3.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# bus_user (v0.3.4)
+# bus_user (v0.3.5)
 
 ## DESCRIPTION_SHORT
 work with equipment over buses like Serial/i2c/... as client and server
 
 ## DESCRIPTION_LONG
 ###
 NOTE: IT SEEMS THIS IS OLD DATA! see tests for actual usage!
```

### Comparing `bus_user-0.3.4/bus_user/__init__.py` & `bus_user-0.3.5/bus_user/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,28 +15,14 @@
 #     # TYPES
 #
 #     # EXX
 # )
 # ---------------------------------------------------------------------------------------------------------------------
 from .history import HistoryIO
 from .line_parser import LineParsed
-from .values import (
-    # BASE
-    Value_NotPassed,
-    Value_WithUnit,
-    Value_FromVariants,
-
-    # AUX
-
-    # TYPES
-
-    # EXX
-    Exx__ValueNotInVariants,
-    Exx__VariantsIncompatible,
-)
 from .serial_client import (
     # BASE
     SerialClient,
 
     # AUX
 
     # TYPES
```

### Comparing `bus_user-0.3.4/bus_user/history.py` & `bus_user-0.3.5/bus_user/history.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.4/bus_user/i2c_client.py` & `bus_user-0.3.5/bus_user/i2c_client.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.4/bus_user/line_parser.py` & `bus_user-0.3.5/bus_user/line_parser.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.4/bus_user/serial_client.py` & `bus_user-0.3.5/bus_user/serial_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -217,20 +217,38 @@
     def cmd_prefix__set(self) -> None:
         """
         OVERWRITE IF NEED/USED!
         """
         # self.PREFIX = ""
         return
 
-    def _clear_buffer_read(self) -> None:
+    def _clear_buffer__read(self) -> None:
         try:
             self.read_lines(_timeout=0.3)
         except:
             pass
 
+    def _clear_buffer__write(self) -> None:
+        """useful to drop old previous incorrect send msg! in other words it is clear/reinit write buffer!
+
+        here we need just finish line by correct/exact EOL if it was previously send without it or with incorrect.
+        """
+        try:
+            self.write_eol()
+        except:
+            pass
+
+    def clear_buffers(self) -> None:
+        """useful to drop old previous incorrect send msg! in other words it is clear/reinit write buffer!
+
+        here we need just finish line by correct/exact EOL if it was previously send without it or with incorrect.
+        """
+        self._clear_buffer__write()
+        self._clear_buffer__read()
+
     # CONNECT =========================================================================================================
     def disconnect(self) -> None:
         try:
             self._SERIAL.close()
         except:
             pass
 
@@ -356,15 +374,15 @@
 
         if self._EMULATOR__CLS:
             self._EMULATOR__INST = self._EMULATOR__CLS(self.address_paired__get())
 
         if self._EMULATOR__INST.connect():
             self._EMULATOR__INST.start()
             self._EMULATOR__INST.wait__cycle_active()
-            self._clear_buffer_read()
+            self._clear_buffer__read()
 
     # ADDRESS =========================================================================================================
     """
     THIS IS USED for applying by SIMPLE WAY just exact address! 
     """
     pass
     pass
@@ -730,34 +748,35 @@
     pass
     pass
     pass
     pass
     pass
 
     # CMD -------------------------------------------------------------------------------------------------------------
-    def _create_cmd_line(self, cmd: Any, prefix: Optional[str] = None, args: List[Any] = None, kwargs: Dict[str, Any] = None) -> str:
+    def _create_cmd_line(self, cmd: str, prefix: Optional[str] = None, args: List[Any] = None, kwargs: Dict[Any, Any] = None) -> str:
         result = ""
 
-        cmd = str(cmd)
+        cmd = self._data_ensure__string(cmd)
+        cmd = self._data_eol__clear(cmd)
 
         if prefix is None:
-            prefix = self.PREFIX
+            prefix = self.PREFIX or ""
 
         if prefix and not cmd.startswith(prefix):
             result += f"{prefix}"
 
         result += f"{cmd}"
 
         if args:
             for arg in args:
                 result += f" {arg}"
 
         if kwargs:
-            for name, value in kwargs.items():
-                result += f" {name}={value}"
+            for key, value in kwargs.items():
+                result += f" {key}={value}"
         return result
 
     # SUCCESS ---------------------------------------------------------------------------------------------------------
     def answer_is_success(self, data: AnyStr) -> bool:
         data = self._data_ensure__string(data)
         return self.ANSWER_SUCCESS.upper() == data.upper()
 
@@ -780,28 +799,32 @@
                 else:
                     return True
 
         return False
 
     # BYTES -----------------------------------------------------------------------------------------------------------
     @classmethod
-    def _bytes_eol__ensure(cls, data: bytes) -> bytes:
-        if not data.endswith(cls.EOL__SEND):
-            data = data + cls.EOL__SEND
+    def _bytes_eol__ensure(cls, data: bytes) -> Union[bytes, NoReturn]:
+        data = cls._data_eol__clear(data) + cls.EOL__SEND
         return data
 
     @classmethod
-    def _bytes_eol__clear(cls, data: bytes) -> bytes:
+    def _data_eol__clear(cls, data: AnyStr) -> Union[AnyStr, NoReturn]:
+        result: bytes = cls._data_ensure__bytes(data)
         while True:
-            data_new = data.strip()
+            data_new = result.strip()
             data_new = data_new.strip(cls.EOL__UNI_SET)
-            if not data or data == data_new:
+            if not result or result == data_new:
                 break
-            data = data_new
-        return data
+            result = data_new
+
+        if isinstance(data, str):
+            return cls._data_ensure__string(result)
+
+        return result
 
     @classmethod
     def _bytes_edition__apply(cls, data: bytes) -> bytes:
         """not used so far!!!
         need to handle editions used by hand in manual typing from terminal!
         """
         # TODO: finish or leave blank! its not so necessary!!! and seems a little bit hard to apply
@@ -896,15 +919,15 @@
 
         else:
             msg = f"[WARN]BLANK read_line={data}"
 
         self.LOGGER.info(f"[{self._SERIAL.port}]{msg}")
 
         data = self._bytes_edition__apply(data)
-        data = self._bytes_eol__clear(data)
+        data = self._data_eol__clear(data)
         data = self._data_ensure__string(data)
         self.history.add_output(data)
         self.answer_is_fail(data)
         return data
 
     # W ---------------------------------------------------------------------------------------------------------------
     def _write(
@@ -951,14 +974,17 @@
         if data_length > 0:
             return True
         else:
             msg = f"[ERROR] write {data}"
             self.LOGGER.error(f"[{self._SERIAL.port}]{msg}")
             return False
 
+    def write_eol(self) -> bool:
+        return self._write(data=self.EOL__SEND, prefix="")
+
     def write_read(
             self,
             data: Union[AnyStr, List[AnyStr]],
             prefix: Optional[str] = None,
             args: Optional[List] = None,
             kwargs: Optional[Dict] = None,
     ) -> Union[HistoryIO, NoReturn]:
@@ -999,22 +1025,27 @@
             self,
             input: Union[AnyStr, list[AnyStr]] | None,
             expect: Union[str, list[str]],
             prefix: Optional[str] = None,
             args: Optional[List] = None,
             kwargs: Optional[Dict] = None,
     ) -> bool:
+        """
+        created specially for address__answer_validation
+        """
+        self.clear_buffers()
+        time.sleep(1)
         if input:
-            return self.write_read__last(data=input, prefix=prefix, args=args, kwargs=kwargs) == expect
+            output_last = self.write_read__last(data=input, prefix=prefix, args=args, kwargs=kwargs)
         else:
             outputs = self.read_lines()
             output_last = None
             if outputs:
                 output_last = outputs[-1]
-            return output_last == expect
+        return output_last == expect
 
     def dump_cmds(self, cmds: List[str] = None) -> Union[HistoryIO, NoReturn]:
         """
         useful to get results for standard cmds list
         if you need to read all params from device!
         """
         cmds = cmds or self.CMDS_DUMP
```

### Comparing `bus_user-0.3.4/bus_user/serial_derivatives.py` & `bus_user-0.3.5/bus_user/serial_derivatives.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.4/bus_user/serial_server.py` & `bus_user-0.3.5/bus_user/serial_server.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import re
 import logging
 import datetime
 
 from object_info import ObjectInfo
 from PyQt5.QtCore import QThread
 
-import funcs_aux
+from funcs_aux import *
 from logger_aux import Logger
 
 
 # =====================================================================================================================
 TYPE__CMD_RESULT = Union[str, List[str]]
 
 
@@ -233,15 +233,15 @@
         return write_result
 
     # CMD - ENTRY POINT -----------------------------------------------------------------------------------------------
     def _cmd__(self, line_parsed: LineParsed) -> TYPE__CMD_RESULT:
         self.LOGGER.debug("")
 
         meth_name__expected = f"{self._STARTSWITH__CMD}{line_parsed.CMD}"
-        meth_name__original = funcs_aux.Iterables().item__get_original__case_insensitive(meth_name__expected, dir(self))
+        meth_name__original = Iterables().item__get_original__case_insensitive(meth_name__expected, dir(self))
         # GET METHOD --------------------
         if meth_name__original:
             meth = getattr(self, meth_name__original.VALUE)
         else:
             meth = self._cmd__param_as_cmd
 
         # EXEC METHOD --------------------
@@ -287,15 +287,15 @@
 
         # PREPARE --------------------------------
         ARGS = []
         for arg in line_parsed.ARGS:
             ARGS.extend(arg.split("/"))
 
         # WORK --------------------------------
-        param_value = funcs_aux.Iterables().value_by_path__get(ARGS, self.PARAMS)
+        param_value = Iterables().value_by_path__get(ARGS, self.PARAMS)
         if not param_value:
             return self.ANSWER.ERR__NAME_CMD_OR_PARAM
 
         param_value = param_value.VALUE
 
         # VARIANTS ------------------------------------------------------------------
         # Value_WithUnit -------------------------------
@@ -328,41 +328,41 @@
         # PREPARE --------------------------------
         KWARGS = {**line_parsed.KWARGS}
         if line_parsed.ARGS:
             KWARGS = {line_parsed.ARGS[0]: line_parsed.ARGS[1]}
 
         # VALIDATE = check AVAILABLE TO CHANGE = exists all and not callable --------------
         for path, value_new in KWARGS.items():
-            path_name__original = funcs_aux.Iterables().path__get_original(path, self.PARAMS)
+            path_name__original = Iterables().path__get_original(path, self.PARAMS)
             if not path_name__original:
                 return self.ANSWER.ERR__NAME_CMD_OR_PARAM
 
-            value_old = funcs_aux.Iterables().value_by_path__get(path, self.PARAMS).VALUE
+            value_old = Iterables().value_by_path__get(path, self.PARAMS).VALUE
             if isinstance(value_old, Value_WithUnit):
                 # NOTE: ALL CLASSES/INSTANCES ARE CALLABLE!!!
                 pass
             elif isinstance(value_old, Value_FromVariants):
                 if value_new not in value_old:
                     return self.ANSWER.ERR__VALUE_INCOMPATIBLE
             elif callable(value_old):
                 return self.ANSWER.ERR__NAME_CMD_OR_PARAM
 
         # SET --------------
         for path, value_new in KWARGS.items():
-            value_new = funcs_aux.Strings().try_convert_to__elementary(value_new)
-            value_old = funcs_aux.Iterables().value_by_path__get(path, self.PARAMS).VALUE
+            value_new = Strings().try_convert_to__elementary(value_new)
+            value_old = Iterables().value_by_path__get(path, self.PARAMS).VALUE
             # SET ----------
             if isinstance(value_old, (Value_WithUnit, Value_FromVariants)):
                 try:
                     value_old.value = value_new
                     result = True
                 except:
                     return self.ANSWER.ERR__VALUE_INCOMPATIBLE
             else:
-                result = funcs_aux.Iterables().value_by_path__set(path, value_new, self.PARAMS)
+                result = Iterables().value_by_path__set(path, value_new, self.PARAMS)
 
             if not result:
                 return self.ANSWER.FAIL
 
         return self.ANSWER.SUCCESS
 
     # CMDS - STD ------------------------------------------------------------------------------------------------------
@@ -397,15 +397,15 @@
     def _script__(self, line_parsed: LineParsed) -> TYPE__CMD_RESULT:
         # ERR__ARGS_VALIDATION --------------------------------
         if line_parsed.ARGS_count() == 0:
             return self.ANSWER.ERR__ARGS_VALIDATION
 
         # WORK --------------------------------
         meth_name__expected = f"{self._STARTSWITH__SCRIPT}{line_parsed.ARGS[0]}"
-        meth_name__original = funcs_aux.Iterables().item__get_original__case_insensitive(meth_name__expected, dir(self))
+        meth_name__original = Iterables().item__get_original__case_insensitive(meth_name__expected, dir(self))
         if not meth_name__original:
             return self.ANSWER.ERR__NAME_SCRIPT
 
         meth = getattr(self, meth_name__original.VALUE)
 
         # EXEC METHOD --------------------
         try:
```

### Comparing `bus_user-0.3.4/bus_user.egg-info/PKG-INFO` & `bus_user-0.3.5/bus_user.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bus_user
-Version: 0.3.4
+Version: 0.3.5
 Summary: work with equipment over buses like Serial/i2c/... as client and server
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/bus_user
 Keywords: serial,serial bus,pyserial,serial port,com port,comport,rs232,UART,TTL,serial client,serial server,serial emulator,i2c
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# bus_user (v0.3.4)
+# bus_user (v0.3.5)
 
 ## DESCRIPTION_SHORT
 work with equipment over buses like Serial/i2c/... as client and server
 
 ## DESCRIPTION_LONG
 ###
 NOTE: IT SEEMS THIS IS OLD DATA! see tests for actual usage!
```

### Comparing `bus_user-0.3.4/setup.py` & `bus_user-0.3.5/setup.py`

 * *Files identical despite different names*

