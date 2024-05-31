# Comparing `tmp/maadebugger-1.1.0b2.tar.gz` & `tmp/maadebugger-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maadebugger-1.1.0b2.tar", last modified: Wed May  8 08:05:47 2024, max compression
+gzip compressed data, was "maadebugger-1.2.0.tar", last modified: Fri May 31 15:34:32 2024, max compression
```

## Comparing `maadebugger-1.1.0b2.tar` & `maadebugger-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1063 2024-05-08 08:05:21.476698 maadebugger-1.1.0b2/LICENSE
--rw-r--r--   0        0        0      123 2024-05-08 08:05:21.476698 maadebugger-1.1.0b2/README.md
--rw-r--r--   0        0        0      479 2024-05-08 08:05:47.448804 maadebugger-1.1.0b2/pyproject.toml
--rw-r--r--   0        0        0       62 2024-05-08 08:05:21.476698 maadebugger-1.1.0b2/src/MaaDebugger/__main__.py
--rw-r--r--   0        0        0     4854 2024-05-08 08:05:21.476698 maadebugger-1.1.0b2/src/MaaDebugger/maafw/__init__.py
--rw-r--r--   0        0        0      254 2024-05-08 08:05:21.476698 maadebugger-1.1.0b2/src/MaaDebugger/main.py
--rw-r--r--   0        0        0      201 2024-05-08 08:05:21.476698 maadebugger-1.1.0b2/src/MaaDebugger/utils/__init__.py
--rw-r--r--   0        0        0      799 2024-05-08 08:05:21.476698 maadebugger-1.1.0b2/src/MaaDebugger/webpage/components/status_indicator.py
--rw-r--r--   0        0        0      240 2024-05-08 08:05:21.476698 maadebugger-1.1.0b2/src/MaaDebugger/webpage/index_page/__init__.py
--rw-r--r--   0        0        0     8775 2024-05-08 08:05:21.476698 maadebugger-1.1.0b2/src/MaaDebugger/webpage/index_page/master_control.py
--rw-r--r--   0        0        0     2788 2024-05-08 08:05:21.476698 maadebugger-1.1.0b2/src/MaaDebugger/webpage/index_page/runtime_control.py
--rw-r--r--   0        0        0      901 2024-05-08 08:05:21.476698 maadebugger-1.1.0b2/src/MaaDebugger/webpage/reco_page/__init__.py
--rw-r--r--   0        0        0      386 1970-01-01 00:00:00.000000 maadebugger-1.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-31 15:34:20.682694 maadebugger-1.2.0/LICENSE
+-rw-r--r--   0        0        0      289 2024-05-31 15:34:20.682694 maadebugger-1.2.0/README.md
+-rw-r--r--   0        0        0      479 2024-05-31 15:34:32.026806 maadebugger-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       62 2024-05-31 15:34:20.686694 maadebugger-1.2.0/src/MaaDebugger/__main__.py
+-rw-r--r--   0        0        0     4994 2024-05-31 15:34:20.686694 maadebugger-1.2.0/src/MaaDebugger/maafw/__init__.py
+-rw-r--r--   0        0        0      254 2024-05-31 15:34:20.686694 maadebugger-1.2.0/src/MaaDebugger/main.py
+-rw-r--r--   0        0        0      201 2024-05-31 15:34:20.686694 maadebugger-1.2.0/src/MaaDebugger/utils/__init__.py
+-rw-r--r--   0        0        0      799 2024-05-31 15:34:20.686694 maadebugger-1.2.0/src/MaaDebugger/webpage/components/status_indicator.py
+-rw-r--r--   0        0        0      240 2024-05-31 15:34:20.686694 maadebugger-1.2.0/src/MaaDebugger/webpage/index_page/__init__.py
+-rw-r--r--   0        0        0     9950 2024-05-31 15:34:20.686694 maadebugger-1.2.0/src/MaaDebugger/webpage/index_page/master_control.py
+-rw-r--r--   0        0        0     2788 2024-05-31 15:34:20.686694 maadebugger-1.2.0/src/MaaDebugger/webpage/index_page/runtime_control.py
+-rw-r--r--   0        0        0      901 2024-05-31 15:34:20.686694 maadebugger-1.2.0/src/MaaDebugger/webpage/reco_page/__init__.py
+-rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 maadebugger-1.2.0/PKG-INFO
```

### Comparing `maadebugger-1.1.0b2/LICENSE` & `maadebugger-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `maadebugger-1.1.0b2/src/MaaDebugger/maafw/__init__.py` & `maadebugger-1.2.0/src/MaaDebugger/maafw/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,19 +58,23 @@
         connected = await self.controller.connect()
         if not connected:
             print(f"Failed to connect {path} {address}")
             return False
 
         return True
 
-    async def connect_win32hwnd(self, hwnd: int | str) -> bool:
+    async def connect_win32hwnd(
+        self, hwnd: int | str, screencap_type: int, input_type: int
+    ) -> bool:
         if isinstance(hwnd, str):
             hwnd = int(hwnd, 16)
 
-        self.controller = Win32Controller(hwnd)
+        self.controller = Win32Controller(
+            hwnd, screencap_type=screencap_type, touch_type=input_type, key_type=0
+        )
         connected = await self.controller.connect()
         if not connected:
             print(f"Failed to connect {hwnd}")
             return False
 
         return True
```

### Comparing `maadebugger-1.1.0b2/src/MaaDebugger/webpage/components/status_indicator.py` & `maadebugger-1.2.0/src/MaaDebugger/webpage/components/status_indicator.py`

 * *Files identical despite different names*

### Comparing `maadebugger-1.1.0b2/src/MaaDebugger/webpage/index_page/master_control.py` & `maadebugger-1.2.0/src/MaaDebugger/webpage/index_page/master_control.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 from pathlib import Path
 
+from maa.define import MaaWin32ControllerTypeEnum
 from nicegui import app, binding, ui
 
 from ...maafw import maafw
 from ...webpage.components.status_indicator import Status, StatusIndicator
 
 binding.MAX_PROPAGATION_TIME = 1
 
@@ -133,20 +134,48 @@
 
 async def connect_win32_control():
     StatusIndicator(GlobalStatus, "ctrl_connecting")
 
     hwnd_input = (
         ui.input("HWND").props("size=30").bind_value(app.storage.general, "hwnd")
     )
+
+    SCREENCAP_DICT = {
+        MaaWin32ControllerTypeEnum.Screencap_GDI: "Screencap_GDI",
+        MaaWin32ControllerTypeEnum.Screencap_DXGI_DesktopDup: "Screencap_DXGI_DesktopDup",
+        MaaWin32ControllerTypeEnum.Screencap_DXGI_FramePool: "Screencap_DXGI_FramePool",
+    }
+    screencap_select = ui.select(
+        SCREENCAP_DICT, value=MaaWin32ControllerTypeEnum.Screencap_DXGI_DesktopDup
+    ).bind_value(app.storage.general, "win32_screencap")
+
+    INPUT_DICT = {
+        (
+            MaaWin32ControllerTypeEnum.Touch_SendMessage
+            | MaaWin32ControllerTypeEnum.Key_SendMessage
+        ): "Input_SendMessage",
+        (
+            MaaWin32ControllerTypeEnum.Touch_Seize
+            | MaaWin32ControllerTypeEnum.Key_Seize
+        ): "Input_Seize",
+    }
+    input_select = ui.select(
+        INPUT_DICT,
+        value=(
+            MaaWin32ControllerTypeEnum.Touch_Seize
+            | MaaWin32ControllerTypeEnum.Key_Seize
+        ),
+    ).bind_value(app.storage.general, "win32_input")
+
     ui.button(
         "Connect",
         on_click=lambda: on_click_connect(),
     )
     window_name_input = (
-        ui.input("Window Regex")
+        ui.input("Search Window Name", placeholder="Supports regex, eg: File Explorer")
         .props("size=30")
         .bind_value(app.storage.general, "window_name")
     )
     ui.button(
         icon="wifi_find",
         on_click=lambda: on_click_detect(),
     )
@@ -168,15 +197,17 @@
     async def on_click_connect():
         GlobalStatus.ctrl_connecting = Status.RUNNING
 
         if not hwnd_input.value:
             GlobalStatus.ctrl_connecting = Status.FAILURE
             return
 
-        connected = await maafw.connect_win32hwnd(hwnd_input.value)
+        connected = await maafw.connect_win32hwnd(
+            hwnd_input.value, screencap_select.value, input_select.value
+        )
         if not connected:
             GlobalStatus.ctrl_connecting = Status.FAILURE
             return
 
         GlobalStatus.ctrl_connecting = Status.SUCCESS
         GlobalStatus.ctrl_detecting = Status.PENDING
```

### Comparing `maadebugger-1.1.0b2/src/MaaDebugger/webpage/index_page/runtime_control.py` & `maadebugger-1.2.0/src/MaaDebugger/webpage/index_page/runtime_control.py`

 * *Files identical despite different names*

### Comparing `maadebugger-1.1.0b2/src/MaaDebugger/webpage/reco_page/__init__.py` & `maadebugger-1.2.0/src/MaaDebugger/webpage/reco_page/__init__.py`

 * *Files identical despite different names*

