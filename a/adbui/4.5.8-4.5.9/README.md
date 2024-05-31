# Comparing `tmp/adbui-4.5.8.tar.gz` & `tmp/adbui-4.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/adbui-4.5.8.tar", last modified: Thu May 13 03:47:27 2021, max compression
+gzip compressed data, was "dist/adbui-4.5.9.tar", last modified: Thu May 13 12:23:12 2021, max compression
```

## Comparing `adbui-4.5.8.tar` & `adbui-4.5.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 tango     (1000) tango     (1000)        0 2021-05-13 03:47:27.000000 adbui-4.5.8/
-drwxrwxrwx   0 tango     (1000) tango     (1000)        0 2021-05-13 03:47:27.000000 adbui-4.5.8/adbui/
--rwxrwxrwx   0 tango     (1000) tango     (1000)     7745 2021-05-13 01:50:52.000000 adbui-4.5.8/adbui/adb_ext.py
--rwxrwxrwx   0 tango     (1000) tango     (1000)     6687 2021-05-11 08:53:36.000000 adbui-4.5.8/adbui/get_ui.py
--rwxrwxrwx   0 tango     (1000) tango     (1000)     4983 2021-05-11 09:07:35.000000 adbui-4.5.8/adbui/ocr.py
-drwxrwxrwx   0 tango     (1000) tango     (1000)        0 2021-05-13 03:47:27.000000 adbui-4.5.8/adbui/static/
--rwxrwxrwx   0 tango     (1000) tango     (1000)    17384 2021-05-10 16:33:48.000000 adbui-4.5.8/adbui/static/adbui
--rwxrwxrwx   0 tango     (1000) tango     (1000)     1149 2020-04-07 06:50:18.000000 adbui-4.5.8/adbui/tango.py
--rwxrwxrwx   0 tango     (1000) tango     (1000)     4169 2021-05-13 03:45:36.000000 adbui-4.5.8/adbui/util.py
--rwxrwxrwx   0 tango     (1000) tango     (1000)      298 2020-04-07 06:50:18.000000 adbui-4.5.8/adbui/__init__.py
-drwxrwxrwx   0 tango     (1000) tango     (1000)        0 2021-05-13 03:47:27.000000 adbui-4.5.8/adbui.egg-info/
--rwxrwxrwx   0 tango     (1000) tango     (1000)        1 2021-05-13 03:47:26.000000 adbui-4.5.8/adbui.egg-info/dependency_links.txt
--rwxrwxrwx   0 tango     (1000) tango     (1000)     6845 2021-05-13 03:47:26.000000 adbui-4.5.8/adbui.egg-info/PKG-INFO
--rwxrwxrwx   0 tango     (1000) tango     (1000)       58 2021-05-13 03:47:26.000000 adbui-4.5.8/adbui.egg-info/requires.txt
--rwxrwxrwx   0 tango     (1000) tango     (1000)      286 2021-05-13 03:47:26.000000 adbui-4.5.8/adbui.egg-info/SOURCES.txt
--rwxrwxrwx   0 tango     (1000) tango     (1000)        6 2021-05-13 03:47:26.000000 adbui-4.5.8/adbui.egg-info/top_level.txt
--rwxrwxrwx   0 tango     (1000) tango     (1000)       32 2021-05-11 09:11:18.000000 adbui-4.5.8/MANIFEST.in
--rwxrwxrwx   0 tango     (1000) tango     (1000)     6845 2021-05-13 03:47:27.000000 adbui-4.5.8/PKG-INFO
--rwxrwxrwx   0 tango     (1000) tango     (1000)     5234 2021-05-11 09:07:35.000000 adbui-4.5.8/README.md
--rwxrwxrwx   0 tango     (1000) tango     (1000)       38 2021-05-13 03:47:27.000000 adbui-4.5.8/setup.cfg
--rwxrwxrwx   0 tango     (1000) tango     (1000)     1215 2021-05-13 03:47:24.000000 adbui-4.5.8/setup.py
+drwxrwxrwx   0 tango     (1000) tango     (1000)        0 2021-05-13 12:23:12.000000 adbui-4.5.9/
+drwxrwxrwx   0 tango     (1000) tango     (1000)        0 2021-05-13 12:23:11.000000 adbui-4.5.9/adbui/
+-rwxrwxrwx   0 tango     (1000) tango     (1000)     7745 2021-05-13 01:50:52.000000 adbui-4.5.9/adbui/adb_ext.py
+-rwxrwxrwx   0 tango     (1000) tango     (1000)     6687 2021-05-11 08:53:36.000000 adbui-4.5.9/adbui/get_ui.py
+-rwxrwxrwx   0 tango     (1000) tango     (1000)     4983 2021-05-11 09:07:35.000000 adbui-4.5.9/adbui/ocr.py
+drwxrwxrwx   0 tango     (1000) tango     (1000)        0 2021-05-13 12:23:11.000000 adbui-4.5.9/adbui/static/
+-rwxrwxrwx   0 tango     (1000) tango     (1000)    17384 2021-05-10 16:33:48.000000 adbui-4.5.9/adbui/static/adbui
+-rwxrwxrwx   0 tango     (1000) tango     (1000)     1149 2020-04-07 06:50:18.000000 adbui-4.5.9/adbui/tango.py
+-rwxrwxrwx   0 tango     (1000) tango     (1000)     4054 2021-05-13 12:22:45.000000 adbui-4.5.9/adbui/util.py
+-rwxrwxrwx   0 tango     (1000) tango     (1000)      298 2020-04-07 06:50:18.000000 adbui-4.5.9/adbui/__init__.py
+drwxrwxrwx   0 tango     (1000) tango     (1000)        0 2021-05-13 12:23:11.000000 adbui-4.5.9/adbui.egg-info/
+-rwxrwxrwx   0 tango     (1000) tango     (1000)        1 2021-05-13 12:23:11.000000 adbui-4.5.9/adbui.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tango     (1000) tango     (1000)     6845 2021-05-13 12:23:11.000000 adbui-4.5.9/adbui.egg-info/PKG-INFO
+-rwxrwxrwx   0 tango     (1000) tango     (1000)       58 2021-05-13 12:23:11.000000 adbui-4.5.9/adbui.egg-info/requires.txt
+-rwxrwxrwx   0 tango     (1000) tango     (1000)      286 2021-05-13 12:23:11.000000 adbui-4.5.9/adbui.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tango     (1000) tango     (1000)        6 2021-05-13 12:23:11.000000 adbui-4.5.9/adbui.egg-info/top_level.txt
+-rwxrwxrwx   0 tango     (1000) tango     (1000)       32 2021-05-11 09:11:18.000000 adbui-4.5.9/MANIFEST.in
+-rwxrwxrwx   0 tango     (1000) tango     (1000)     6845 2021-05-13 12:23:12.000000 adbui-4.5.9/PKG-INFO
+-rwxrwxrwx   0 tango     (1000) tango     (1000)     5234 2021-05-11 09:07:35.000000 adbui-4.5.9/README.md
+-rwxrwxrwx   0 tango     (1000) tango     (1000)       38 2021-05-13 12:23:12.000000 adbui-4.5.9/setup.cfg
+-rwxrwxrwx   0 tango     (1000) tango     (1000)     1215 2021-05-13 12:22:45.000000 adbui-4.5.9/setup.py
```

### Comparing `adbui-4.5.8/adbui/adb_ext.py` & `adbui-4.5.9/adbui/adb_ext.py`

 * *Files identical despite different names*

### Comparing `adbui-4.5.8/adbui/get_ui.py` & `adbui-4.5.9/adbui/get_ui.py`

 * *Files identical despite different names*

### Comparing `adbui-4.5.8/adbui/ocr.py` & `adbui-4.5.9/adbui/ocr.py`

 * *Files identical despite different names*

### Comparing `adbui-4.5.8/adbui/static/adbui` & `adbui-4.5.9/adbui/static/adbui`

 * *Files identical despite different names*

### Comparing `adbui-4.5.8/adbui/tango.py` & `adbui-4.5.9/adbui/tango.py`

 * *Files identical despite different names*

### Comparing `adbui-4.5.8/adbui/util.py` & `adbui-4.5.9/adbui/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,17 +92,15 @@
         arg = 'shell {}'.format(arg)
         return self.adb(arg, timeout, encoding=encoding)
 
     def connect_sn(self):
         if self.sn.count('.') != 3:
             return  # 非网络设备不处理
         self.cmd('adb disconnect {}'.format(self.sn))  # 首先断开连接，排除该 sn 当前是 offline 状态
-        out, err = self.cmd('adb connect {}'.format(self.sn))
-        if 'connected to' not in out:
-            raise NameError('无法连接: {}'.format(self.sn))
+        self.cmd('adb connect {}'.format(self.sn))
 
     def get_first_sn(self):
         sn_info = self.get_sn_info()
         for sn in sn_info:
             if sn_info[sn] == 'device':
                 return sn
         raise NameError('没有可以使用的设备: {}'.format(sn_info))
```

### Comparing `adbui-4.5.8/adbui.egg-info/PKG-INFO` & `adbui-4.5.9/adbui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adbui
-Version: 4.5.8
+Version: 4.5.9
 Summary: adbui 所有的功能都是通过 adb 命令，adbui 的特色是可以通过 xpath，ocr 获取 ui 元素。
 Home-page: https://github.com/hao1032/adbui
 Author: Tango Nian
 Author-email: hao1032@gmail.com
 License: MIT
 Description: # 常见问题
         - adbui 交流微信群，加 hao1032，备注 adbui，会拉入微信群
```

### Comparing `adbui-4.5.8/PKG-INFO` & `adbui-4.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adbui
-Version: 4.5.8
+Version: 4.5.9
 Summary: adbui 所有的功能都是通过 adb 命令，adbui 的特色是可以通过 xpath，ocr 获取 ui 元素。
 Home-page: https://github.com/hao1032/adbui
 Author: Tango Nian
 Author-email: hao1032@gmail.com
 License: MIT
 Description: # 常见问题
         - adbui 交流微信群，加 hao1032，备注 adbui，会拉入微信群
```

### Comparing `adbui-4.5.8/README.md` & `adbui-4.5.9/README.md`

 * *Files identical despite different names*

### Comparing `adbui-4.5.8/setup.py` & `adbui-4.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import io
 from setuptools import setup, find_packages
 
-VERSION = '4.5.8'
+VERSION = '4.5.9'
 
 with io.open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 requires = [
     'lxml',
     'requests',
```

