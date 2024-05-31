# Comparing `tmp/aicamera-2.1.0.tar.gz` & `tmp/aicamera-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicamera-2.1.0.tar", last modified: Wed May 29 03:48:59 2024, max compression
+gzip compressed data, was "aicamera-2.1.1.tar", last modified: Fri May 31 01:39:34 2024, max compression
```

## Comparing `aicamera-2.1.0.tar` & `aicamera-2.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 03:48:59.855337 aicamera-2.1.0/
--rw-rw-rw-   0        0        0     1093 2024-05-29 03:43:49.000000 aicamera-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     1368 2024-05-29 03:48:59.855337 aicamera-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      824 2024-03-21 08:38:44.000000 aicamera-2.1.0/README.md
--rw-rw-rw-   0        0        0      613 2024-05-29 03:46:34.000000 aicamera-2.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-29 03:48:59.855337 aicamera-2.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-29 03:48:59.821739 aicamera-2.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-29 03:48:59.842773 aicamera-2.1.0/src/aicamera/
--rw-rw-rw-   0        0        0     2179 2024-05-29 02:43:42.000000 aicamera-2.1.0/src/aicamera/__init__.py
--rw-rw-rw-   0        0        0    16075 2024-05-27 11:06:26.000000 aicamera-2.1.0/src/aicamera/cameraSocket.py
--rw-rw-rw-   0        0        0     1182 2024-05-21 11:40:09.000000 aicamera-2.1.0/src/aicamera/image.py
--rw-rw-rw-   0        0        0      211 2024-03-28 07:52:08.000000 aicamera-2.1.0/src/aicamera/lcd.py
--rw-rw-rw-   0        0        0     1693 2024-04-08 02:08:40.000000 aicamera-2.1.0/src/aicamera/rtsp.py
--rw-rw-rw-   0        0        0     4379 2024-05-23 02:32:47.000000 aicamera-2.1.0/src/aicamera/udp.py
--rw-rw-rw-   0        0        0     5147 2024-05-21 11:40:09.000000 aicamera-2.1.0/src/aicamera/util.py
--rw-rw-rw-   0        0        0      282 2024-02-29 08:22:40.000000 aicamera-2.1.0/src/aicamera/wifi.py
-drwxrwxrwx   0        0        0        0 2024-05-29 03:48:59.855337 aicamera-2.1.0/src/aicamera.egg-info/
--rw-rw-rw-   0        0        0     1368 2024-05-29 03:48:59.000000 aicamera-2.1.0/src/aicamera.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2024-05-29 03:48:59.000000 aicamera-2.1.0/src/aicamera.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 03:48:59.000000 aicamera-2.1.0/src/aicamera.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-29 03:48:59.000000 aicamera-2.1.0/src/aicamera.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 01:39:34.654644 aicamera-2.1.1/
+-rw-rw-rw-   0        0        0     1093 2024-05-31 01:35:36.000000 aicamera-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1368 2024-05-31 01:39:34.654644 aicamera-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      613 2024-05-31 01:37:40.000000 aicamera-2.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      824 2024-03-21 08:38:44.000000 aicamera-2.1.1/readme.md
+-rw-rw-rw-   0        0        0       42 2024-05-31 01:39:34.654644 aicamera-2.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-31 01:39:34.623392 aicamera-2.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-31 01:39:34.639019 aicamera-2.1.1/src/aicamera/
+-rw-rw-rw-   0        0        0     2179 2024-05-30 09:13:08.000000 aicamera-2.1.1/src/aicamera/__init__.py
+-rw-rw-rw-   0        0        0    16060 2024-05-30 05:37:41.000000 aicamera-2.1.1/src/aicamera/cameraSocket.py
+-rw-rw-rw-   0        0        0     1237 2024-05-29 09:12:49.000000 aicamera-2.1.1/src/aicamera/image.py
+-rw-rw-rw-   0        0        0      211 2024-03-28 07:52:08.000000 aicamera-2.1.1/src/aicamera/lcd.py
+-rw-rw-rw-   0        0        0     1693 2024-04-08 02:08:40.000000 aicamera-2.1.1/src/aicamera/rtsp.py
+-rw-rw-rw-   0        0        0     4379 2024-05-23 02:32:47.000000 aicamera-2.1.1/src/aicamera/udp.py
+-rw-rw-rw-   0        0        0     5147 2024-05-21 11:40:09.000000 aicamera-2.1.1/src/aicamera/util.py
+-rw-rw-rw-   0        0        0      282 2024-02-29 08:22:40.000000 aicamera-2.1.1/src/aicamera/wifi.py
+drwxrwxrwx   0        0        0        0 2024-05-31 01:39:34.654644 aicamera-2.1.1/src/aicamera.egg-info/
+-rw-rw-rw-   0        0        0     1368 2024-05-31 01:39:34.000000 aicamera-2.1.1/src/aicamera.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2024-05-31 01:39:34.000000 aicamera-2.1.1/src/aicamera.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 01:39:34.000000 aicamera-2.1.1/src/aicamera.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-31 01:39:34.000000 aicamera-2.1.1/src/aicamera.egg-info/top_level.txt
```

### Comparing `aicamera-2.1.0/LICENSE` & `aicamera-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aicamera-2.1.0/PKG-INFO` & `aicamera-2.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicamera
-Version: 2.1.0
+Version: 2.1.1
 Summary: A small example package
 Author-email: xiaoheli <1173324325@qq.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aicamera-2.1.0/README.md` & `aicamera-2.1.1/readme.md`

 * *Files identical despite different names*

### Comparing `aicamera-2.1.0/pyproject.toml` & `aicamera-2.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "aicamera"
-version = "2.1.0"
+version = "2.1.1"
 authors = [
   { name = "xiaoheli", email = "1173324325@qq.com" },
 ]
 dependencies = []
 description = "A small example package"
-readme = "README.md"
+readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `aicamera-2.1.0/src/aicamera/__init__.py` & `aicamera-2.1.1/src/aicamera/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # 初始化
 sdk.init(arg?=)
 
 
 初始化完毕后可以调用摄像头通讯
 其中 __ 开头得函数代表暂时不对外暴露
 
-version: 2.1.0
+version: 2.1.1
 
 '''
 import threading
 import asyncio
 import time
 from . import udp
 from . import util
```

### Comparing `aicamera-2.1.0/src/aicamera/cameraSocket.py` & `aicamera-2.1.1/src/aicamera/cameraSocket.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,15 +291,15 @@
 
 
 def __hand():
     global __handRes
     __handRes = []
 
 
-resetHand = util.debounce(__hand, 1)
+resetHand = util.debounce(__hand, 0.5)
 
 
 def __saveHandRes(val):
     global __handRes
     __handRes = [[
         0,
         0,
@@ -319,15 +319,15 @@
 
 __cardRes = []
 def __card():
     global __cardRes
     __cardRes = []
 
 
-resetCard = util.debounce(__card, 1)
+resetCard = util.debounce(__card, 0.5)
 def __saveCardRes(val):
     global __cardRes
     __cardRes = [[
         val['x'],
         val['y'],
         val['width'],
         val['height'],
@@ -345,26 +345,26 @@
 
 __carCodeRes = []
 def __carCode():
     global __carCodeRes
     __carCodeRes = []
 
 
-resetCard = util.debounce(__carCode, 1)
+resCarCode = util.debounce(__carCode, 0.5)
 def __saveCarCodeRes(val):
     global __carCodeRes
     __carCodeRes = [[
         val['x'],
         val['y'],
         val['width'],
         val['height'],
         val['conf'],
         val['name'],
     ]]
-    resetCard()
+    resCarCode()
 
 
 
 
 '''
 Date: 2024-04-01 14:19:32
 author: zjs
@@ -384,15 +384,14 @@
 description: 获取卡片模型结果
 '''
 
 
 def __y8CardModelResult(__):
     if not cameraServiceSocket:
         print('摄像头未连接请稍后')
-    print('__cardRes')
     return __cardRes
 
 
 
 '''
 Date: 2024-04-01 14:19:32
 author: zjs
```

### Comparing `aicamera-2.1.0/src/aicamera/image.py` & `aicamera-2.1.1/src/aicamera/image.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,10 +38,11 @@
     if not imgName.endswith('.jpg'):
         imgName += '.jpg'
     saveFile = os.path.normpath(os.path.join(os.getcwd(), imgName))
     # 没有路径创建路径
     saveDir = os.path.dirname(saveFile)
     if not os.path.exists(saveDir):
         os.makedirs(saveDir)
+    imaData = cv2.cvtColor(imaData, cv2.COLOR_BGR2RGB)
     cv2.imwrite(saveFile, imaData)
     cameraSocket.__sendClientWithFn(cameraSocket.__sendClientFnEnum['savePhoto'],saveFile)
     return imgName
```

### Comparing `aicamera-2.1.0/src/aicamera/rtsp.py` & `aicamera-2.1.1/src/aicamera/rtsp.py`

 * *Files identical despite different names*

### Comparing `aicamera-2.1.0/src/aicamera/udp.py` & `aicamera-2.1.1/src/aicamera/udp.py`

 * *Files identical despite different names*

### Comparing `aicamera-2.1.0/src/aicamera/util.py` & `aicamera-2.1.1/src/aicamera/util.py`

 * *Files identical despite different names*

### Comparing `aicamera-2.1.0/src/aicamera.egg-info/PKG-INFO` & `aicamera-2.1.1/src/aicamera.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicamera
-Version: 2.1.0
+Version: 2.1.1
 Summary: A small example package
 Author-email: xiaoheli <1173324325@qq.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

