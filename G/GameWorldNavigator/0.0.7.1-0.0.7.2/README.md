# Comparing `tmp/GameWorldNavigator-0.0.7.1.tar.gz` & `tmp/GameWorldNavigator-0.0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GameWorldNavigator-0.0.7.1.tar", last modified: Thu May 30 14:27:42 2024, max compression
+gzip compressed data, was "GameWorldNavigator-0.0.7.2.tar", last modified: Fri May 31 06:33:50 2024, max compression
```

## Comparing `GameWorldNavigator-0.0.7.1.tar` & `GameWorldNavigator-0.0.7.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 14:27:42.302103 GameWorldNavigator-0.0.7.1/
-drwxrwxrwx   0        0        0        0 2024-05-30 14:27:42.288026 GameWorldNavigator-0.0.7.1/GameWorldNavigator.egg-info/
--rw-rw-rw-   0        0        0      790 2024-05-30 14:27:42.000000 GameWorldNavigator-0.0.7.1/GameWorldNavigator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      677 2024-05-30 14:27:42.000000 GameWorldNavigator-0.0.7.1/GameWorldNavigator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 14:27:42.000000 GameWorldNavigator-0.0.7.1/GameWorldNavigator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-30 14:27:42.000000 GameWorldNavigator-0.0.7.1/GameWorldNavigator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1084 2023-11-14 15:46:54.000000 GameWorldNavigator-0.0.7.1/LICENSE
--rw-rw-rw-   0        0        0      790 2024-05-30 14:27:42.301411 GameWorldNavigator-0.0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-11-15 07:38:05.000000 GameWorldNavigator-0.0.7.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 14:27:42.295901 GameWorldNavigator-0.0.7.1/gamenavigator/
--rw-rw-rw-   0        0        0      575 2024-05-25 01:28:35.000000 GameWorldNavigator-0.0.7.1/gamenavigator/__init__.py
--rw-rw-rw-   0        0        0      253 2023-11-14 15:30:21.000000 GameWorldNavigator-0.0.7.1/gamenavigator/config.py
--rw-rw-rw-   0        0        0     4997 2024-05-30 14:20:09.000000 GameWorldNavigator-0.0.7.1/gamenavigator/controller.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:27:42.300631 GameWorldNavigator-0.0.7.1/gamenavigator/core/
--rw-rw-rw-   0        0        0      149 2024-05-30 14:04:45.000000 GameWorldNavigator-0.0.7.1/gamenavigator/core/__init__.py
--rw-rw-rw-   0        0        0      609 2024-05-26 04:19:24.000000 GameWorldNavigator-0.0.7.1/gamenavigator/core/image.py
--rw-rw-rw-   0        0        0     3766 2024-05-30 14:08:11.000000 GameWorldNavigator-0.0.7.1/gamenavigator/core/interface.py
--rw-rw-rw-   0        0        0     1811 2024-05-26 14:20:48.000000 GameWorldNavigator-0.0.7.1/gamenavigator/core/pos.py
--rw-rw-rw-   0        0        0      758 2023-11-19 02:27:01.000000 GameWorldNavigator-0.0.7.1/gamenavigator/core/rect.py
--rw-rw-rw-   0        0        0      372 2023-11-16 09:39:18.000000 GameWorldNavigator-0.0.7.1/gamenavigator/exception.py
--rw-rw-rw-   0        0        0    17077 2024-05-28 08:45:58.000000 GameWorldNavigator-0.0.7.1/gamenavigator/game_controller.py
--rw-rw-rw-   0        0        0     3237 2024-05-27 07:11:03.000000 GameWorldNavigator-0.0.7.1/gamenavigator/game_interface_controller.py
--rw-rw-rw-   0        0        0     4148 2024-05-26 11:24:27.000000 GameWorldNavigator-0.0.7.1/gamenavigator/image_recognition.py
--rw-rw-rw-   0        0        0     4325 2023-11-19 02:56:31.000000 GameWorldNavigator-0.0.7.1/gamenavigator/keyboard_mouse_simulation.py
--rw-rw-rw-   0        0        0      778 2023-11-15 07:05:17.000000 GameWorldNavigator-0.0.7.1/gamenavigator/listener.py
--rw-rw-rw-   0        0        0      703 2023-11-15 09:41:12.000000 GameWorldNavigator-0.0.7.1/gamenavigator/log.py
--rw-rw-rw-   0        0        0     1974 2024-05-26 09:59:22.000000 GameWorldNavigator-0.0.7.1/gamenavigator/ocr_recognition.py
--rw-rw-rw-   0        0        0       42 2024-05-30 14:27:42.302103 GameWorldNavigator-0.0.7.1/setup.cfg
--rw-rw-rw-   0        0        0      674 2024-05-30 14:27:02.000000 GameWorldNavigator-0.0.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:33:50.265701 GameWorldNavigator-0.0.7.2/
+drwxrwxrwx   0        0        0        0 2024-05-31 06:33:50.243065 GameWorldNavigator-0.0.7.2/GameWorldNavigator.egg-info/
+-rw-rw-rw-   0        0        0      790 2024-05-31 06:33:50.000000 GameWorldNavigator-0.0.7.2/GameWorldNavigator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      718 2024-05-31 06:33:50.000000 GameWorldNavigator-0.0.7.2/GameWorldNavigator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 06:33:50.000000 GameWorldNavigator-0.0.7.2/GameWorldNavigator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-31 06:33:50.000000 GameWorldNavigator-0.0.7.2/GameWorldNavigator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-31 06:33:50.000000 GameWorldNavigator-0.0.7.2/GameWorldNavigator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1084 2023-11-14 15:46:54.000000 GameWorldNavigator-0.0.7.2/LICENSE
+-rw-rw-rw-   0        0        0      790 2024-05-31 06:33:50.264696 GameWorldNavigator-0.0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-11-15 07:38:05.000000 GameWorldNavigator-0.0.7.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 06:33:50.260165 GameWorldNavigator-0.0.7.2/gamenavigator/
+-rw-rw-rw-   0        0        0      575 2024-05-25 01:28:35.000000 GameWorldNavigator-0.0.7.2/gamenavigator/__init__.py
+-rw-rw-rw-   0        0        0      253 2023-11-14 15:30:21.000000 GameWorldNavigator-0.0.7.2/gamenavigator/config.py
+-rw-rw-rw-   0        0        0     4997 2024-05-30 14:20:09.000000 GameWorldNavigator-0.0.7.2/gamenavigator/controller.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:33:50.263700 GameWorldNavigator-0.0.7.2/gamenavigator/core/
+-rw-rw-rw-   0        0        0      149 2024-05-30 14:04:45.000000 GameWorldNavigator-0.0.7.2/gamenavigator/core/__init__.py
+-rw-rw-rw-   0        0        0      609 2024-05-26 04:19:24.000000 GameWorldNavigator-0.0.7.2/gamenavigator/core/image.py
+-rw-rw-rw-   0        0        0     3766 2024-05-30 14:08:11.000000 GameWorldNavigator-0.0.7.2/gamenavigator/core/interface.py
+-rw-rw-rw-   0        0        0     1811 2024-05-26 14:20:48.000000 GameWorldNavigator-0.0.7.2/gamenavigator/core/pos.py
+-rw-rw-rw-   0        0        0      758 2023-11-19 02:27:01.000000 GameWorldNavigator-0.0.7.2/gamenavigator/core/rect.py
+-rw-rw-rw-   0        0        0      372 2023-11-16 09:39:18.000000 GameWorldNavigator-0.0.7.2/gamenavigator/exception.py
+-rw-rw-rw-   0        0        0    17077 2024-05-28 08:45:58.000000 GameWorldNavigator-0.0.7.2/gamenavigator/game_controller.py
+-rw-rw-rw-   0        0        0     3237 2024-05-27 07:11:03.000000 GameWorldNavigator-0.0.7.2/gamenavigator/game_interface_controller.py
+-rw-rw-rw-   0        0        0     4148 2024-05-31 06:19:05.000000 GameWorldNavigator-0.0.7.2/gamenavigator/image_recognition.py
+-rw-rw-rw-   0        0        0     4325 2023-11-19 02:56:31.000000 GameWorldNavigator-0.0.7.2/gamenavigator/keyboard_mouse_simulation.py
+-rw-rw-rw-   0        0        0      778 2023-11-15 07:05:17.000000 GameWorldNavigator-0.0.7.2/gamenavigator/listener.py
+-rw-rw-rw-   0        0        0      703 2023-11-15 09:41:12.000000 GameWorldNavigator-0.0.7.2/gamenavigator/log.py
+-rw-rw-rw-   0        0        0     1974 2024-05-26 09:59:22.000000 GameWorldNavigator-0.0.7.2/gamenavigator/ocr_recognition.py
+-rw-rw-rw-   0        0        0       42 2024-05-31 06:33:50.265701 GameWorldNavigator-0.0.7.2/setup.cfg
+-rw-rw-rw-   0        0        0      860 2024-05-31 06:33:06.000000 GameWorldNavigator-0.0.7.2/setup.py
```

### Comparing `GameWorldNavigator-0.0.7.1/GameWorldNavigator.egg-info/PKG-INFO` & `GameWorldNavigator-0.0.7.2/GameWorldNavigator.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GameWorldNavigator
-Version: 0.0.7.1
+Version: 0.0.7.2
 Summary: A framework for game automation
 Home-page: https://github.com/JunNanLYS/GameWorldNavigator
 Author: NanJunLYS
 Author-email: 18906571516@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `GameWorldNavigator-0.0.7.1/GameWorldNavigator.egg-info/SOURCES.txt` & `GameWorldNavigator-0.0.7.2/GameWorldNavigator.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.py
 GameWorldNavigator.egg-info/PKG-INFO
 GameWorldNavigator.egg-info/SOURCES.txt
 GameWorldNavigator.egg-info/dependency_links.txt
+GameWorldNavigator.egg-info/requires.txt
 GameWorldNavigator.egg-info/top_level.txt
 gamenavigator/__init__.py
 gamenavigator/config.py
 gamenavigator/controller.py
 gamenavigator/exception.py
 gamenavigator/game_controller.py
 gamenavigator/game_interface_controller.py
```

### Comparing `GameWorldNavigator-0.0.7.1/LICENSE` & `GameWorldNavigator-0.0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.1/PKG-INFO` & `GameWorldNavigator-0.0.7.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GameWorldNavigator
-Version: 0.0.7.1
+Version: 0.0.7.2
 Summary: A framework for game automation
 Home-page: https://github.com/JunNanLYS/GameWorldNavigator
 Author: NanJunLYS
 Author-email: 18906571516@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `GameWorldNavigator-0.0.7.1/gamenavigator/__init__.py` & `GameWorldNavigator-0.0.7.2/gamenavigator/__init__.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.1/gamenavigator/controller.py` & `GameWorldNavigator-0.0.7.2/gamenavigator/controller.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.1/gamenavigator/core/image.py` & `GameWorldNavigator-0.0.7.2/gamenavigator/core/image.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.1/gamenavigator/core/interface.py` & `GameWorldNavigator-0.0.7.2/gamenavigator/core/interface.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.1/gamenavigator/core/pos.py` & `GameWorldNavigator-0.0.7.2/gamenavigator/core/pos.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.1/gamenavigator/core/rect.py` & `GameWorldNavigator-0.0.7.2/gamenavigator/core/rect.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.1/gamenavigator/game_controller.py` & `GameWorldNavigator-0.0.7.2/gamenavigator/game_controller.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.1/gamenavigator/game_interface_controller.py` & `GameWorldNavigator-0.0.7.2/gamenavigator/game_interface_controller.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.1/gamenavigator/image_recognition.py` & `GameWorldNavigator-0.0.7.2/gamenavigator/image_recognition.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.1/gamenavigator/keyboard_mouse_simulation.py` & `GameWorldNavigator-0.0.7.2/gamenavigator/keyboard_mouse_simulation.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.1/gamenavigator/listener.py` & `GameWorldNavigator-0.0.7.2/gamenavigator/listener.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.1/gamenavigator/log.py` & `GameWorldNavigator-0.0.7.2/gamenavigator/log.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7.1/gamenavigator/ocr_recognition.py` & `GameWorldNavigator-0.0.7.2/gamenavigator/ocr_recognition.py`

 * *Files identical despite different names*

