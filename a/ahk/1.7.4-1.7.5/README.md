# Comparing `tmp/ahk-1.7.4.tar.gz` & `tmp/ahk-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahk-1.7.4.tar", last modified: Tue May 28 08:27:30 2024, max compression
+gzip compressed data, was "ahk-1.7.5.tar", last modified: Fri May 31 00:39:03 2024, max compression
```

## Comparing `ahk-1.7.4.tar` & `ahk-1.7.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:27:30.384937 ahk-1.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-28 08:27:23.000000 ahk-1.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-28 08:27:23.000000 ahk-1.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    28092 2024-05-28 08:27:30.384937 ahk-1.7.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:27:30.380937 ahk-1.7.4/ahk/
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-28 08:27:23.000000 ahk-1.7.4/ahk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:27:30.384937 ahk-1.7.4/ahk/_async/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-28 08:27:23.000000 ahk-1.7.4/ahk/_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   210809 2024-05-28 08:27:23.000000 ahk-1.7.4/ahk/_async/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    48128 2024-05-28 08:27:23.000000 ahk-1.7.4/ahk/_async/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)    30507 2024-05-28 08:27:23.000000 ahk-1.7.4/ahk/_async/window.py
--rw-r--r--   0 runner    (1001) docker     (127)   171952 2024-05-28 08:27:23.000000 ahk-1.7.4/ahk/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    17219 2024-05-28 08:27:23.000000 ahk-1.7.4/ahk/_hotkey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:27:30.384937 ahk-1.7.4/ahk/_sync/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-28 08:27:23.000000 ahk-1.7.4/ahk/_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   203991 2024-05-28 08:27:23.000000 ahk-1.7.4/ahk/_sync/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    43146 2024-05-28 08:27:23.000000 ahk-1.7.4/ahk/_sync/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)    27714 2024-05-28 08:27:23.000000 ahk-1.7.4/ahk/_sync/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-28 08:27:23.000000 ahk-1.7.4/ahk/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-28 08:27:23.000000 ahk-1.7.4/ahk/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-28 08:27:23.000000 ahk-1.7.4/ahk/directives.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-28 08:27:23.000000 ahk-1.7.4/ahk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-28 08:27:23.000000 ahk-1.7.4/ahk/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-05-28 08:27:23.000000 ahk-1.7.4/ahk/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-05-28 08:27:23.000000 ahk-1.7.4/ahk/message.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:27:23.000000 ahk-1.7.4/ahk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:27:30.384937 ahk-1.7.4/ahk/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    80539 2024-05-28 08:27:23.000000 ahk-1.7.4/ahk/templates/daemon-v2.ahk
--rw-r--r--   0 runner    (1001) docker     (127)    81015 2024-05-28 08:27:23.000000 ahk-1.7.4/ahk/templates/daemon.ahk
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-05-28 08:27:23.000000 ahk-1.7.4/ahk/templates/hotkeys-v2.ahk
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-28 08:27:23.000000 ahk-1.7.4/ahk/templates/hotkeys.ahk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:27:30.384937 ahk-1.7.4/ahk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28092 2024-05-28 08:27:30.000000 ahk-1.7.4/ahk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-28 08:27:30.000000 ahk-1.7.4/ahk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 08:27:30.000000 ahk-1.7.4/ahk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-28 08:27:30.000000 ahk-1.7.4/ahk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-28 08:27:30.000000 ahk-1.7.4/ahk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-28 08:27:23.000000 ahk-1.7.4/buildunasync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:27:30.384937 ahk-1.7.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    26719 2024-05-28 08:27:23.000000 ahk-1.7.4/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-28 08:27:23.000000 ahk-1.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-28 08:27:30.388937 ahk-1.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 08:27:23.000000 ahk-1.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:39:03.401953 ahk-1.7.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-31 00:38:54.000000 ahk-1.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-31 00:38:54.000000 ahk-1.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    28092 2024-05-31 00:39:03.401953 ahk-1.7.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:39:03.397953 ahk-1.7.5/ahk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-31 00:38:54.000000 ahk-1.7.5/ahk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:39:03.401953 ahk-1.7.5/ahk/_async/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-31 00:38:54.000000 ahk-1.7.5/ahk/_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   210809 2024-05-31 00:38:54.000000 ahk-1.7.5/ahk/_async/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48128 2024-05-31 00:38:54.000000 ahk-1.7.5/ahk/_async/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30507 2024-05-31 00:38:54.000000 ahk-1.7.5/ahk/_async/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)   173444 2024-05-31 00:38:54.000000 ahk-1.7.5/ahk/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17219 2024-05-31 00:38:54.000000 ahk-1.7.5/ahk/_hotkey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:39:03.401953 ahk-1.7.5/ahk/_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-31 00:38:54.000000 ahk-1.7.5/ahk/_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   203991 2024-05-31 00:38:54.000000 ahk-1.7.5/ahk/_sync/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43146 2024-05-31 00:38:54.000000 ahk-1.7.5/ahk/_sync/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27714 2024-05-31 00:38:54.000000 ahk-1.7.5/ahk/_sync/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-31 00:38:54.000000 ahk-1.7.5/ahk/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-31 00:38:54.000000 ahk-1.7.5/ahk/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-31 00:38:54.000000 ahk-1.7.5/ahk/directives.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-31 00:38:54.000000 ahk-1.7.5/ahk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-31 00:38:54.000000 ahk-1.7.5/ahk/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-05-31 00:38:54.000000 ahk-1.7.5/ahk/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-05-31 00:38:54.000000 ahk-1.7.5/ahk/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 00:38:54.000000 ahk-1.7.5/ahk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:39:03.401953 ahk-1.7.5/ahk/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    82031 2024-05-31 00:38:54.000000 ahk-1.7.5/ahk/templates/daemon-v2.ahk
+-rw-r--r--   0 runner    (1001) docker     (127)    81015 2024-05-31 00:38:54.000000 ahk-1.7.5/ahk/templates/daemon.ahk
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-05-31 00:38:54.000000 ahk-1.7.5/ahk/templates/hotkeys-v2.ahk
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-31 00:38:54.000000 ahk-1.7.5/ahk/templates/hotkeys.ahk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:39:03.401953 ahk-1.7.5/ahk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28092 2024-05-31 00:39:03.000000 ahk-1.7.5/ahk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-31 00:39:03.000000 ahk-1.7.5/ahk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 00:39:03.000000 ahk-1.7.5/ahk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-31 00:39:03.000000 ahk-1.7.5/ahk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-31 00:39:03.000000 ahk-1.7.5/ahk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-31 00:38:54.000000 ahk-1.7.5/buildunasync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:39:03.401953 ahk-1.7.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    26719 2024-05-31 00:38:54.000000 ahk-1.7.5/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-31 00:38:54.000000 ahk-1.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-31 00:39:03.405953 ahk-1.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 00:38:54.000000 ahk-1.7.5/setup.py
```

### Comparing `ahk-1.7.4/LICENSE` & `ahk-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ahk-1.7.4/PKG-INFO` & `ahk-1.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.7.4
+Version: 1.7.5
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Project-URL: Documentation, https://ahk.readthedocs.io/en/latest/
 Project-URL: Funding, https://github.com/sponsors/spyoungtech/
 Project-URL: Source, https://github.com/spyoungtech/ahk
```

### Comparing `ahk-1.7.4/ahk/__init__.py` & `ahk-1.7.5/ahk/__init__.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.4/ahk/_async/engine.py` & `ahk-1.7.5/ahk/_async/engine.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.4/ahk/_async/transport.py` & `ahk-1.7.5/ahk/_async/transport.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.4/ahk/_async/window.py` & `ahk-1.7.5/ahk/_async/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.4/ahk/_constants.py` & `ahk-1.7.5/ahk/_constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -5050,15 +5050,21 @@
     current_send_mode := Format("{}", A_SendMode)
 
     if (send_mode != "") {
         SendMode send_mode
     }
 
     if (key_delay != "" or key_press_duration != "") {
-        SetKeyDelay(key_delay, key_press_duration)
+        if (key_delay != "" and key_press_duration != "") {
+            SetKeyDelay(key_delay, key_press_duration)
+        } else if (key_delay != "" and key_press_duration = "") {
+            SetKeyDelay(key_delay)
+        } else if (key_delay = "" and key_press_duration != "") {
+            SetKeyDelay(current_delay, key_press_duration)
+        }
     }
 
 
     Send(str)
 
     if (send_mode != "") {
         SendMode current_send_mode
@@ -5076,15 +5082,21 @@
     str := args[1]
     key_delay := args[2]
     key_press_duration := args[3]
     current_delay := Format("{}", A_KeyDelay)
     current_key_duration := Format("{}", A_KeyDuration)
 
     if (key_delay != "" or key_press_duration != "") {
-        SetKeyDelay(key_delay, key_press_duration)
+        if (key_delay != "" and key_press_duration != "") {
+            SetKeyDelay(key_delay, key_press_duration)
+        } else if (key_delay != "" and key_press_duration = "") {
+            SetKeyDelay(key_delay)
+        } else if (key_delay = "" and key_press_duration != "") {
+            SetKeyDelay(current_delay, key_press_duration)
+        }
     }
 
     Send("{Raw}" str)
 
     if (key_delay != "" or key_press_duration != "") {
         SetKeyDelay(current_delay, current_key_duration)
     }
@@ -5097,15 +5109,21 @@
     str := args[1]
     key_delay := args[2]
     key_press_duration := args[3]
     current_delay := Format("{}", A_KeyDelay)
     current_key_duration := Format("{}", A_KeyDuration)
 
     if (key_delay != "" or key_press_duration != "") {
-        SetKeyDelay(key_delay, key_press_duration)
+        if (key_delay != "" and key_press_duration != "") {
+            SetKeyDelay(key_delay, key_press_duration)
+        } else if (key_delay != "" and key_press_duration = "") {
+            SetKeyDelay(key_delay)
+        } else if (key_delay = "" and key_press_duration != "") {
+            SetKeyDelay(current_delay, key_press_duration)
+        }
     }
 
     SendInput(str)
 
     if (key_delay != "" or key_press_duration != "") {
         SetKeyDelay(current_delay, current_key_duration)
     }
@@ -5118,15 +5136,21 @@
     str := args[1]
     key_delay := args[2]
     key_press_duration := args[3]
     current_delay := Format("{}", A_KeyDelay)
     current_key_duration := Format("{}", A_KeyDuration)
 
     if (key_delay != "" or key_press_duration != "") {
-        SetKeyDelay(key_delay, key_press_duration)
+        if (key_delay != "" and key_press_duration != "") {
+            SetKeyDelay(key_delay, key_press_duration)
+        } else if (key_delay != "" and key_press_duration = "") {
+            SetKeyDelay(key_delay)
+        } else if (key_delay = "" and key_press_duration != "") {
+            SetKeyDelay(current_delay, key_press_duration)
+        }
     }
 
     SendEvent(str)
 
     if (key_delay != "" or key_press_duration != "") {
         SetKeyDelay(current_delay, current_key_duration)
     }
@@ -5139,15 +5163,21 @@
     str := args[1]
     key_delay := args[2]
     key_press_duration := args[3]
     current_delay := Format("{}", A_KeyDelayPlay)
     current_key_duration := Format("{}", A_KeyDurationPlay)
 
     if (key_delay != "" or key_press_duration != "") {
-        SetKeyDelay(key_delay, key_press_duration, "Play")
+        if (key_delay != "" and key_press_duration != "") {
+            SetKeyDelay(key_delay, key_press_duration)
+        } else if (key_delay != "" and key_press_duration = "") {
+            SetKeyDelay(key_delay)
+        } else if (key_delay = "" and key_press_duration != "") {
+            SetKeyDelay(current_delay, key_press_duration)
+        }
     }
 
     SendPlay(str)
 
     if (key_delay != "" or key_press_duration != "") {
         SetKeyDelay(current_delay, current_key_duration)
     }
```

### Comparing `ahk-1.7.4/ahk/_hotkey.py` & `ahk-1.7.5/ahk/_hotkey.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.4/ahk/_sync/engine.py` & `ahk-1.7.5/ahk/_sync/engine.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.4/ahk/_sync/transport.py` & `ahk-1.7.5/ahk/_sync/transport.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.4/ahk/_sync/window.py` & `ahk-1.7.5/ahk/_sync/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.4/ahk/_types.py` & `ahk-1.7.5/ahk/_types.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.4/ahk/_utils.py` & `ahk-1.7.5/ahk/_utils.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.4/ahk/directives.py` & `ahk-1.7.5/ahk/directives.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.4/ahk/extensions.py` & `ahk-1.7.5/ahk/extensions.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.4/ahk/keys.py` & `ahk-1.7.5/ahk/keys.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.4/ahk/message.py` & `ahk-1.7.5/ahk/message.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.4/ahk/templates/daemon-v2.ahk` & `ahk-1.7.5/ahk/templates/daemon-v2.ahk`

 * *Files 8% similar despite different names*

```diff
@@ -2037,15 +2037,21 @@
     current_send_mode := Format("{}", A_SendMode)
 
     if (send_mode != "") {
         SendMode send_mode
     }
 
     if (key_delay != "" or key_press_duration != "") {
-        SetKeyDelay(key_delay, key_press_duration)
+        if (key_delay != "" and key_press_duration != "") {
+            SetKeyDelay(key_delay, key_press_duration)
+        } else if (key_delay != "" and key_press_duration = "") {
+            SetKeyDelay(key_delay)
+        } else if (key_delay = "" and key_press_duration != "") {
+            SetKeyDelay(current_delay, key_press_duration)
+        }
     }
 
 
     Send(str)
 
     if (send_mode != "") {
         SendMode current_send_mode
@@ -2063,15 +2069,21 @@
     str := args[1]
     key_delay := args[2]
     key_press_duration := args[3]
     current_delay := Format("{}", A_KeyDelay)
     current_key_duration := Format("{}", A_KeyDuration)
 
     if (key_delay != "" or key_press_duration != "") {
-        SetKeyDelay(key_delay, key_press_duration)
+        if (key_delay != "" and key_press_duration != "") {
+            SetKeyDelay(key_delay, key_press_duration)
+        } else if (key_delay != "" and key_press_duration = "") {
+            SetKeyDelay(key_delay)
+        } else if (key_delay = "" and key_press_duration != "") {
+            SetKeyDelay(current_delay, key_press_duration)
+        }
     }
 
     Send("{Raw}" str)
 
     if (key_delay != "" or key_press_duration != "") {
         SetKeyDelay(current_delay, current_key_duration)
     }
@@ -2084,15 +2096,21 @@
     str := args[1]
     key_delay := args[2]
     key_press_duration := args[3]
     current_delay := Format("{}", A_KeyDelay)
     current_key_duration := Format("{}", A_KeyDuration)
 
     if (key_delay != "" or key_press_duration != "") {
-        SetKeyDelay(key_delay, key_press_duration)
+        if (key_delay != "" and key_press_duration != "") {
+            SetKeyDelay(key_delay, key_press_duration)
+        } else if (key_delay != "" and key_press_duration = "") {
+            SetKeyDelay(key_delay)
+        } else if (key_delay = "" and key_press_duration != "") {
+            SetKeyDelay(current_delay, key_press_duration)
+        }
     }
 
     SendInput(str)
 
     if (key_delay != "" or key_press_duration != "") {
         SetKeyDelay(current_delay, current_key_duration)
     }
@@ -2105,15 +2123,21 @@
     str := args[1]
     key_delay := args[2]
     key_press_duration := args[3]
     current_delay := Format("{}", A_KeyDelay)
     current_key_duration := Format("{}", A_KeyDuration)
 
     if (key_delay != "" or key_press_duration != "") {
-        SetKeyDelay(key_delay, key_press_duration)
+        if (key_delay != "" and key_press_duration != "") {
+            SetKeyDelay(key_delay, key_press_duration)
+        } else if (key_delay != "" and key_press_duration = "") {
+            SetKeyDelay(key_delay)
+        } else if (key_delay = "" and key_press_duration != "") {
+            SetKeyDelay(current_delay, key_press_duration)
+        }
     }
 
     SendEvent(str)
 
     if (key_delay != "" or key_press_duration != "") {
         SetKeyDelay(current_delay, current_key_duration)
     }
@@ -2126,15 +2150,21 @@
     str := args[1]
     key_delay := args[2]
     key_press_duration := args[3]
     current_delay := Format("{}", A_KeyDelayPlay)
     current_key_duration := Format("{}", A_KeyDurationPlay)
 
     if (key_delay != "" or key_press_duration != "") {
-        SetKeyDelay(key_delay, key_press_duration, "Play")
+        if (key_delay != "" and key_press_duration != "") {
+            SetKeyDelay(key_delay, key_press_duration)
+        } else if (key_delay != "" and key_press_duration = "") {
+            SetKeyDelay(key_delay)
+        } else if (key_delay = "" and key_press_duration != "") {
+            SetKeyDelay(current_delay, key_press_duration)
+        }
     }
 
     SendPlay(str)
 
     if (key_delay != "" or key_press_duration != "") {
         SetKeyDelay(current_delay, current_key_duration)
     }
```

### Comparing `ahk-1.7.4/ahk/templates/daemon.ahk` & `ahk-1.7.5/ahk/templates/daemon.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.7.4/ahk/templates/hotkeys-v2.ahk` & `ahk-1.7.5/ahk/templates/hotkeys-v2.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.7.4/ahk/templates/hotkeys.ahk` & `ahk-1.7.5/ahk/templates/hotkeys.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.7.4/ahk.egg-info/PKG-INFO` & `ahk-1.7.5/ahk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.7.4
+Version: 1.7.5
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Project-URL: Documentation, https://ahk.readthedocs.io/en/latest/
 Project-URL: Funding, https://github.com/sponsors/spyoungtech/
 Project-URL: Source, https://github.com/spyoungtech/ahk
```

### Comparing `ahk-1.7.4/ahk.egg-info/SOURCES.txt` & `ahk-1.7.5/ahk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ahk-1.7.4/buildunasync.py` & `ahk-1.7.5/buildunasync.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.4/docs/README.md` & `ahk-1.7.5/docs/README.md`

 * *Files identical despite different names*

### Comparing `ahk-1.7.4/setup.cfg` & `ahk-1.7.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ahk
-version = 1.7.4
+version = 1.7.5
 author_email = spencer.young@spyoung.com
 author = Spencer Young
 description = A Python wrapper for AHK
 long_description = file: docs/README.md
 long_description_content_type = text/markdown
 url = https://github.com/spyoungtech/ahk
 project_urls =
```

