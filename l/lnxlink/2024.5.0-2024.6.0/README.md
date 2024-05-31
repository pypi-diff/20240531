# Comparing `tmp/lnxlink-2024.5.0.tar.gz` & `tmp/lnxlink-2024.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnxlink-2024.5.0.tar", last modified: Wed May  1 15:39:44 2024, max compression
+gzip compressed data, was "lnxlink-2024.6.0.tar", last modified: Fri May 31 19:33:47 2024, max compression
```

## Comparing `lnxlink-2024.5.0.tar` & `lnxlink-2024.6.0.tar`

### file list

```diff
@@ -1,64 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:39:44.268826 lnxlink-2024.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-01 15:39:44.268826 lnxlink-2024.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:39:44.260826 lnxlink-2024.5.0/lnxlink/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20496 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8081 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/config_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:39:44.268826 lnxlink-2024.5.0/lnxlink/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/active_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/audio_select.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/bash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/boot_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/camera_used.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/disk_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/display_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/fullscreen.py
--rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/gpio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/idle.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/inference_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/keep_alive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/keyboard_hotkeys.py
--rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/microphone_used.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/notify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/power_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/required_restart.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/restart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/screen_onoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/screenshot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:39:44.268826 lnxlink-2024.5.0/lnxlink/modules/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/scripts/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/send_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/shutdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/speaker_used.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/speech_recognition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/suspend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/sys_updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/systemd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/webcam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/wifi.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/xdg_open.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/system_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:39:44.264826 lnxlink-2024.5.0/lnxlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-01 15:39:44.000000 lnxlink-2024.5.0/lnxlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-01 15:39:44.000000 lnxlink-2024.5.0/lnxlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 15:39:44.000000 lnxlink-2024.5.0/lnxlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-01 15:39:44.000000 lnxlink-2024.5.0/lnxlink.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-01 15:39:44.000000 lnxlink-2024.5.0/lnxlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 15:39:44.000000 lnxlink-2024.5.0/lnxlink.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      943 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-01 15:39:44.268826 lnxlink-2024.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:33:47.363407 lnxlink-2024.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-31 19:33:47.363407 lnxlink-2024.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:33:47.351407 lnxlink-2024.6.0/lnxlink/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20134 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8088 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/config_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:33:47.363407 lnxlink-2024.6.0/lnxlink/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/active_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/audio_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/bash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/boot_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/camera_used.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/disk_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/display_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/fullscreen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/gamepad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/inference_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/keep_alive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/keyboard_hotkeys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9016 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/microphone_used.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/mounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/power_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/required_restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/screen_onoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/screenshot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:33:47.363407 lnxlink-2024.6.0/lnxlink/modules/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/scripts/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/send_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/speaker_used.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/speech_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/suspend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/sys_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/systemd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/webcam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/wifi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/modules/xdg_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/lnxlink/system_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:33:47.355407 lnxlink-2024.6.0/lnxlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-31 19:33:47.000000 lnxlink-2024.6.0/lnxlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-31 19:33:47.000000 lnxlink-2024.6.0/lnxlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 19:33:47.000000 lnxlink-2024.6.0/lnxlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-31 19:33:47.000000 lnxlink-2024.6.0/lnxlink.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-31 19:33:47.000000 lnxlink-2024.6.0/lnxlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 19:33:47.000000 lnxlink-2024.6.0/lnxlink.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      943 2024-05-31 19:33:43.000000 lnxlink-2024.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-31 19:33:47.363407 lnxlink-2024.6.0/setup.cfg
```

### Comparing `lnxlink-2024.5.0/LICENSE.md` & `lnxlink-2024.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.5.0/PKG-INFO` & `lnxlink-2024.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnxlink
-Version: 2024.5.0
+Version: 2024.6.0
 Summary: Internet Of Things (IOT) integration with Linux using MQTT
 Home-page: https://bkbilly.github.io/lnxlink
 Author-email: bkbilly <bkbilly@hotmail.com>
 Project-URL: Source Code, https://github.com/bkbilly/lnxlink
 Project-URL: Documentation, https://bkbilly.gitbook.io/lnxlink
 Keywords: lnxlink
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lnxlink-2024.5.0/README.md` & `lnxlink-2024.6.0/README.md`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.5.0/lnxlink/__main__.py` & `lnxlink-2024.6.0/lnxlink/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 import importlib.metadata
 import ssl
 import traceback
 
 import yaml
 import distro
 import paho.mqtt.client as mqtt
-from . import modules
-from . import config_setup
-from .system_monitor import MonitorSuspend, GracefulKiller
-from .modules.scripts.helpers import syscommand
+from lnxlink import modules
+from lnxlink import config_setup
+from lnxlink.system_monitor import MonitorSuspend, GracefulKiller
+from lnxlink.modules.scripts.helpers import syscommand
 
 
 # Get the current version of the app
 version = importlib.metadata.version(__package__ or __name__)
 path = os.path.dirname(os.path.dirname(os.path.realpath(__file__)))
 if os.path.exists(os.path.join(path, "lnxlink/edit.txt")):
     version += "+edit"
@@ -110,15 +110,15 @@
     def run_module(self, name, method):
         """Runs the method of a module"""
         subtopic = name.lower().replace(" ", "_")
         topic = f"{self.pref_topic}/monitor_controls/{subtopic}"
 
         try:
             start_time = time.time()
-            if isinstance(method, (dict, list, bool)):
+            if isinstance(method, (dict, list, bool, bytes, int, str, float)):
                 pub_data = method
             else:
                 pub_data = method()
             diff_time = round(time.time() - start_time, 5)
             self.inference_times[name] = diff_time
             self.publish_monitor_data(topic, pub_data)
         except Exception as err:
@@ -136,23 +136,14 @@
             if hasattr(addon, "get_info"):
                 methods_to_run.append(
                     {
                         "name": addon.name,
                         "method": addon.get_info,
                     }
                 )
-            if hasattr(addon, "exposed_controls"):
-                for exp_name, options in addon.exposed_controls().items():
-                    if options.get("method") is not None:
-                        methods_to_run.append(
-                            {
-                                "name": f"{addon.name}/{exp_name}",
-                                "method": options["method"],
-                            }
-                        )
         for method in methods_to_run:
             self.run_module(method["name"], method["method"])
 
     def monitor_run_thread(self):
         """Runs method to get sensor information every prespecified interval"""
         self.monitor_run()
 
@@ -333,15 +324,15 @@
                 "model": f"{distro.name()} {distro.version()}",
                 "manufacturer": "LNXlink",
                 "sw_version": version,
             },
         }
         control_name_topic = exp_name.lower().replace(" ", "_")
         subtopic = addon.name.lower().replace(" ", "_")
-        if "method" in options:
+        if "method" in options or options.get("subtopic", False):
             subcontrol = exp_name.lower().replace(" ", "_")
             subtopic = f"{subtopic}/{subcontrol}"
         state_topic = f"{self.pref_topic}/monitor_controls/{subtopic}"
         command_topic = f"{self.pref_topic}/commands/{service}/{control_name_topic}/"
 
         lookup_options = {
             "value_template": {
```

### Comparing `lnxlink-2024.5.0/lnxlink/config_setup.py` & `lnxlink-2024.6.0/lnxlink/config_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import subprocess
 import logging
 import shutil
 from pathlib import Path
 
 import yaml
-from .consts import SERVICEHEADLESS, SERVICEUSER, CONFIGTEMP
+from lnxlink.consts import SERVICEHEADLESS, SERVICEUSER, CONFIGTEMP
 
 logger = logging.getLogger("lnxlink")
 
 
 def setup_config(config_path):
     """Setup and create config file"""
     if not os.path.exists(config_path):
```

### Comparing `lnxlink-2024.5.0/lnxlink/consts.py` & `lnxlink-2024.6.0/lnxlink/consts.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,8 +89,11 @@
   hotkeys:
   disk_usage:
     include_disks: []
     exclude_disks: []
   statistics: "https://analyzer.bkbilly.workers.dev"
   bash:
     expose:
+  mounts:
+    autocheck: false
+    directories: []
 """
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/__init__.py` & `lnxlink-2024.6.0/lnxlink/modules/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """Auto load addons/modules"""
 from importlib import import_module
+from importlib.util import spec_from_file_location, module_from_spec
 import time
 import logging
 import glob
 import os
-import sys
+import requests
 
 logger = logging.getLogger("lnxlink")
 
 
 def autoload_modules(auto_exclude=None):
     """Gather a list of all modules"""
     if auto_exclude is None:
         auto_exclude = []
     modules = []
     modules_path = f"{os.path.dirname(__file__)}/*.py"
     for module_path in glob.glob(modules_path):
         module = os.path.basename(module_path)
-        if "__" not in module and ".py" in module:
+        if "__" not in module and module.endswith(".py"):
             module = module.replace(".py", "")
             if module not in auto_exclude:
                 modules.append(module)
 
     return modules
 
 
@@ -32,31 +33,44 @@
     if custom_modules is not None:
         list_modules.extend(custom_modules)
     modules = {}
     for module_name in list_modules:
         retries = 10
         while retries >= 0:
             try:
-                if ".py" in module_name:
-                    module_path = os.path.dirname(module_name)
-                    module_basename = os.path.basename(module_name)
-                    module_name = os.path.splitext(module_basename)[0]
-                    sys.path.append(module_path)
-                    addon = getattr(import_module(f"{module_name}"), "Addon")
+                if module_name.endswith(".py"):
+                    if module_name.startswith("http"):
+                        logger.info("Downloading custom module: %s", module_name)
+                        module_data = requests.get(module_name, timeout=3).content
+                        module_basename = os.path.basename(module_name)
+                        module_name = f"/tmp/{module_basename}"
+                        with open(module_name, "wb") as handler:
+                            handler.write(module_data)
+                    if os.path.isfile(module_name):
+                        spec = spec_from_file_location("Addon", module_name)
+                        module_spec = module_from_spec(spec)
+                        spec.loader.exec_module(module_spec)
+                        addon = getattr(module_spec, "Addon")
+                    else:
+                        logger.error("Can't find custom module: %s", module_name)
+                        retries = -1
+                        continue
                 else:
                     addon = getattr(import_module(f"{__name__}.{module_name}"), "Addon")
                 addon.service = module_name
                 modules[module_name] = addon
                 retries = -1
             except ModuleNotFoundError as err:
                 logger.error(
                     "Addon %s is not supported, please remove it from your config: %s",
                     module_name,
                     err,
                 )
                 retries = -1
             except Exception as err:
-                logger.error("Error with module %s: %s", module_name, err)
+                logger.error(
+                    "Error with module %s: %s", module_name, err, exc_info=True
+                )
                 time.sleep(2)
                 retries -= 1
     logger.debug("Found addons: %s", ", ".join(modules))
     return modules
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/active_window.py` & `lnxlink-2024.6.0/lnxlink/modules/active_window.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Gets the active window"""
-from .scripts.helpers import import_install_package
+from lnxlink.modules.scripts.helpers import import_install_package
 
 
 class Addon:
     """Addon module"""
 
     def __init__(self, lnxlink):
         """Setup addon"""
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/audio_select.py` & `lnxlink-2024.6.0/lnxlink/modules/audio_select.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Information and control of pulseaudio devices"""
 import logging
-from .scripts.helpers import import_install_package
+from lnxlink.modules.scripts.helpers import import_install_package
 
 logger = logging.getLogger("lnxlink")
 
 
 class Addon:
     """Addon module"""
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/bash.py` & `lnxlink-2024.6.0/lnxlink/modules/send_keys.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-"""Run a terminal command"""
-from .scripts.helpers import syscommand
+"""Uses xdotool to press keyboard keys"""
+import os
+import logging
+from shutil import which
+from lnxlink.modules.scripts.helpers import syscommand
+
+logger = logging.getLogger("lnxlink")
 
 
 class Addon:
     """Addon module"""
 
     def __init__(self, lnxlink):
         """Setup addon"""
-        self.name = "bash"
+        self.name = "Send Keys"
         self.lnxlink = lnxlink
+        if which("xdotool") is None:
+            raise SystemError("System command 'xdotool' not found")
 
     def exposed_controls(self):
         """Exposes to home assistant"""
-        discovery_info = {
-            "Bash_Command": {
+        return {
+            "Send Keys": {
                 "type": "text",
-                "icon": "mdi:bash",
+                "icon": "mdi:keyboard-outline",
             }
         }
-        exposed = self.lnxlink.config["settings"]["bash"]["expose"]
-        exposed = [] if exposed is None else exposed
-        for expose in exposed:
-            discovery_info[f"Bash {expose['name']}"] = {
-                "type": "button",
-                "icon": expose.get("icon", "mdi:script-text"),
-                "payload_press": expose["command"],
-            }
-        return discovery_info
 
     def start_control(self, topic, data):
         """Control system"""
-        stdout, _, _ = syscommand(data, timeout=120)
-        return stdout
+        if os.environ.get("DISPLAY") is None:
+            if self.lnxlink.display is not None:
+                os.environ["DISPLAY"] = self.lnxlink.display
+                logger.info("Initializing empty DISPLAY environment variable")
+        syscommand(f"xdotool key {data}")
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/battery.py` & `lnxlink-2024.6.0/lnxlink/modules/battery.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Gets the battery information of connected devices"""
 from shutil import which
 import jc
-from .scripts.helpers import syscommand
+from lnxlink.modules.scripts.helpers import syscommand
 
 
 class Addon:
     """Addon module"""
 
     def __init__(self, lnxlink):
         """Setup addon"""
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/boot_select.py` & `lnxlink-2024.6.0/lnxlink/modules/boot_select.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Selects the OS to boot from on GRUB at the next restart"""
 import os
 import re
 from shutil import which
-from .scripts.helpers import syscommand
+from lnxlink.modules.scripts.helpers import syscommand
 
 
 class Addon:
     """Addon module"""
 
     def __init__(self, lnxlink=None):
         """Setup addon"""
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/brightness.py` & `lnxlink-2024.6.0/lnxlink/modules/brightness.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Controls the brightness of the displays"""
 import re
 import logging
 from shutil import which
-from .scripts.helpers import syscommand
+from lnxlink.modules.scripts.helpers import syscommand
 
 logger = logging.getLogger("lnxlink")
 
 
 class Addon:
     """Addon module"""
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/camera_used.py` & `lnxlink-2024.6.0/lnxlink/modules/camera_used.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Checks if the webcam is used"""
-from .scripts.helpers import syscommand
+from lnxlink.modules.scripts.helpers import syscommand
 
 
 class Addon:
     """Addon module"""
 
     def __init__(self, lnxlink):
         """Setup addon"""
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/cpu.py` & `lnxlink-2024.6.0/lnxlink/modules/cpu.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.5.0/lnxlink/modules/disk_usage.py` & `lnxlink-2024.6.0/lnxlink/modules/disk_usage.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.5.0/lnxlink/modules/display_env.py` & `lnxlink-2024.6.0/lnxlink/modules/display_env.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Gets Display Environment"""
-from .scripts.helpers import syscommand
+from lnxlink.modules.scripts.helpers import syscommand
 
 
 class Addon:
     """Addon module"""
 
     def __init__(self, lnxlink):
         """Setup addon"""
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/fullscreen.py` & `lnxlink-2024.6.0/lnxlink/modules/fullscreen.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Checks if a window is in fullscreen"""
-from .scripts.helpers import import_install_package
+from lnxlink.modules.scripts.helpers import import_install_package
 
 
 class Addon:
     """Addon module"""
 
     def __init__(self, lnxlink):
         """Setup addon"""
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/gpio.py` & `lnxlink-2024.6.0/lnxlink/modules/gpio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Checks GPIO pins from a raspberry"""
 import os
 import time
 from collections import deque
 from threading import Thread
-from .scripts.helpers import import_install_package
+from lnxlink.modules.scripts.helpers import import_install_package
 
 
 class GpioHandle:
     """Handle the Raspberry PI GPIO inputs by fixing spike events"""
 
     def __init__(self, gpio, pin, callback, setup="input"):
         """Start checking for pin values in a new thread"""
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/gpu.py` & `lnxlink-2024.6.0/lnxlink/modules/gpu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Gets GPU information"""
 import re
 import math
 import logging
 from shutil import which
-from .scripts.helpers import import_install_package, syscommand
+from lnxlink.modules.scripts.helpers import import_install_package, syscommand
 
 logger = logging.getLogger("lnxlink")
 
 
 class Addon:
     """Addon module"""
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/idle.py` & `lnxlink-2024.6.0/lnxlink/modules/idle.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Gets the idle time of the system"""
 import logging
-from .scripts.helpers import import_install_package
+from lnxlink.modules.scripts.helpers import import_install_package
 
 logger = logging.getLogger("lnxlink")
 
 
 class Addon:
     """Addon module"""
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/inference_time.py` & `lnxlink-2024.6.0/lnxlink/modules/inference_time.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.5.0/lnxlink/modules/keep_alive.py` & `lnxlink-2024.6.0/lnxlink/modules/keep_alive.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Keeps display on"""
 import re
 from shutil import which
-from .scripts.helpers import syscommand
+from lnxlink.modules.scripts.helpers import syscommand
 
 
 class Addon:
     """Addon module"""
 
     def __init__(self, lnxlink):
         """Setup addon"""
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/keyboard_hotkeys.py` & `lnxlink-2024.6.0/lnxlink/modules/keyboard_hotkeys.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Assign hotkeys to run commands"""
 import json
 import logging
 from requests import post, get
-from .scripts.helpers import import_install_package, syscommand
+from lnxlink.modules.scripts.helpers import import_install_package, syscommand
 
 
 logger = logging.getLogger("lnxlink")
 
 
 class Addon:
     """Addon module"""
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/media.py` & `lnxlink-2024.6.0/lnxlink/modules/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Control and show information of currently playing media"""
 import re
 import hashlib
 import traceback
 import logging
 import base64
-from .scripts.helpers import import_install_package, syscommand
+from lnxlink.modules.scripts.helpers import import_install_package, syscommand
 
 logger = logging.getLogger("lnxlink")
 
 
 class Addon:
     """Addon module"""
 
     def __init__(self, lnxlink):
         """Setup addon"""
         self.name = "Media Info"
+        self.lnxlink = lnxlink
         self.players = []
         self._requirements()
 
     def _requirements(self):
         self.lib = {
             "dbus": import_install_package(
                 "dbus-python", ">=1.3.2", "dbus.mainloop.glib"
@@ -32,42 +33,42 @@
         return {
             "Media Info": {
                 "type": "sensor",
                 "icon": "mdi:music",
                 "value_template": "{{ value_json.status }}",
                 "attributes_template": "{{ value_json | tojson }}",
             },
-            "playpause": {
+            "PlayPause": {
                 "type": "button",
                 "icon": "mdi:play-pause",
                 "enabled": False,
             },
-            "previous": {
+            "Previous": {
                 "type": "button",
                 "icon": "mdi:skip-previous",
                 "enabled": False,
             },
-            "next": {
+            "Next": {
                 "type": "button",
                 "icon": "mdi:skip-next",
                 "enabled": False,
             },
-            "volume_set": {
+            "Volume Set": {
                 "type": "number",
                 "icon": "mdi:volume-high",
                 "min": 0,
                 "max": 100,
                 "enabled": False,
                 "value_template": "{{ value_json.volume }}",
             },
-            "thumbnail": {
+            "Thumbnail": {
                 "type": "image",
-                "method": self.get_thumbnail,
                 "encoding": "b64",
                 "enabled": False,
+                "subtopic": True,
             },
         }
 
     def start_control(self, topic, data):
         """Control system"""
         if topic[1] == "volume_set":
             mixer = self.lib["alsaaudio"].Mixer()
@@ -107,14 +108,15 @@
             info["title"] = player["title"]
             info["album"] = player["album"]
             info["artist"] = player["artist"]
             info["status"] = player["status"]
             info["position"] = player["position"]
             info["duration"] = player["duration"]
 
+        self.lnxlink.run_module(f"{self.name}/Thumbnail", self.get_thumbnail)
         return info
 
     def get_thumbnail(self):
         """Returns the thumbnail if it exists as a base64 string"""
         if len(self.players) > 0:
             player = self.players[0]
             if player["status"] != "stopped":
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/memory.py` & `lnxlink-2024.6.0/lnxlink/modules/memory.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.5.0/lnxlink/modules/microphone_used.py` & `lnxlink-2024.6.0/lnxlink/modules/microphone_used.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Checks if the microphone is used"""
 import glob
 import json
 import re
-from .scripts.helpers import syscommand
+from lnxlink.modules.scripts.helpers import syscommand
 
 
 class Addon:
     """Addon module"""
 
     def __init__(self, lnxlink):
         """Setup addon"""
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/mouse.py` & `lnxlink-2024.6.0/lnxlink/modules/mouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Uses xdotool to control mouse"""
 import os
 import time
 import logging
 import threading
 from shutil import which
-from .scripts.helpers import syscommand
+from lnxlink.modules.scripts.helpers import syscommand
 
 logger = logging.getLogger("lnxlink")
 
 
 class Addon:
     """Addon module"""
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/network.py` & `lnxlink-2024.6.0/lnxlink/modules/network.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.5.0/lnxlink/modules/power_profile.py` & `lnxlink-2024.6.0/lnxlink/modules/power_profile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Selects the Power Profile"""
 import re
 from shutil import which
-from .scripts.helpers import syscommand
+from lnxlink.modules.scripts.helpers import syscommand
 
 
 class Addon:
     """Addon module"""
 
     def __init__(self, lnxlink=None):
         """Setup addon"""
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/required_restart.py` & `lnxlink-2024.6.0/lnxlink/modules/required_restart.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.5.0/lnxlink/modules/restart.py` & `lnxlink-2024.6.0/lnxlink/modules/restart.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Restarts the system"""
 import logging
-from .scripts.helpers import syscommand
+from lnxlink.modules.scripts.helpers import syscommand
 
 logger = logging.getLogger("lnxlink")
 
 
 class Addon:
     """Addon module"""
 
@@ -22,12 +22,12 @@
             if returncode != 0:
                 self.lnxlink.temp_connection_callback(False)
                 logger.error("Can't shutdown the computer")
 
     def exposed_controls(self):
         """Exposes to home assistant"""
         return {
-            "restart": {
+            "Restart": {
                 "type": "button",
                 "icon": "mdi:restart",
             }
         }
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/screen_onoff.py` & `lnxlink-2024.6.0/lnxlink/modules/screen_onoff.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Turns on or off the screen"""
 import re
 import logging
 from shutil import which
-from .scripts.helpers import syscommand
+from lnxlink.modules.scripts.helpers import syscommand
 
 logger = logging.getLogger("lnxlink")
 
 
 class Addon:
     """Addon module"""
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/screenshot.py` & `lnxlink-2024.6.0/lnxlink/modules/screenshot.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 """Shows an image of the desktop as a camera entity"""
 import base64
-from .scripts.helpers import import_install_package
+from threading import Thread
+from lnxlink.modules.scripts.helpers import import_install_package
 
 
 class Addon:
     """Addon module"""
 
     def __init__(self, lnxlink):
         """Setup addon"""
+        self.lnxlink = lnxlink
         self.name = "Screenshot"
         self.run = False
         self._requirements()
+        self.read_thr = None
 
     def _requirements(self):
         self.lib = {
             "cv2": import_install_package("opencv-python", ">=4.7.0.68", "cv2"),
             "mss": import_install_package("mss", ">=7.0.1"),
             "np": import_install_package("numpy", ">=1.24.0"),
         }
 
     def get_camera_frame(self):
         """Convert screen image to Base64 text"""
         if self.run:
             with self.lib["mss"].mss() as sct:
-                sct_img = sct.grab(sct.monitors[1])
-                frame = self.lib["np"].array(sct_img)
-            _, buffer = self.lib["cv2"].imencode(".jpg", frame)
-            frame = base64.b64encode(buffer)
-            return frame
-        return None
+                while True:
+                    if not self.run:
+                        break
+                    sct_img = sct.grab(sct.monitors[1])
+                    frame = self.lib["np"].array(sct_img)
+                    _, buffer = self.lib["cv2"].imencode(".jpg", frame)
+                    frame = base64.b64encode(buffer)
+                    self.lnxlink.run_module(f"{self.name}/Screenshot feed", frame)
 
     def get_info(self):
         """Gather information from the system"""
         return self.run
 
     def exposed_controls(self):
         """Exposes to home assistant"""
@@ -40,18 +45,24 @@
             "Screenshot": {
                 "type": "switch",
                 "icon": "mdi:monitor-screenshot",
                 "entity_category": "config",
             },
             "Screenshot feed": {
                 "type": "camera",
-                "method": self.get_camera_frame,
                 "encoding": "b64",
+                "subtopic": True,
             },
         }
 
     def start_control(self, topic, data):
         """Control system"""
         if data.lower() == "off":
             self.run = False
+            if self.read_thr is not None:
+                self.read_thr.join()
+                self.read_thr = None
         elif data.lower() == "on":
             self.run = True
+            if self.read_thr is None:
+                self.read_thr = Thread(target=self.get_camera_frame, daemon=True)
+                self.read_thr.start()
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/scripts/helpers.py` & `lnxlink-2024.6.0/lnxlink/modules/scripts/helpers.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.5.0/lnxlink/modules/send_keys.py` & `lnxlink-2024.6.0/lnxlink/modules/xdg_open.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,30 @@
-"""Uses xdotool to press keyboard keys"""
-import os
+"""Open URLs or files"""
 import logging
 from shutil import which
-from .scripts.helpers import syscommand
+from lnxlink.modules.scripts.helpers import syscommand
 
 logger = logging.getLogger("lnxlink")
 
 
 class Addon:
     """Addon module"""
 
     def __init__(self, lnxlink):
         """Setup addon"""
-        self.name = "Send Keys"
-        self.lnxlink = lnxlink
-        if which("xdotool") is None:
-            raise SystemError("System command 'xdotool' not found")
+        self.name = "xdg_open"
+        if which("xdg-open") is None:
+            raise SystemError("System command 'xdg-open' not found")
 
     def exposed_controls(self):
         """Exposes to home assistant"""
         return {
-            "Send_Keys": {
+            "XDG Open": {
                 "type": "text",
-                "icon": "mdi:keyboard-outline",
+                "icon": "mdi:file-find-outline",
             }
         }
 
     def start_control(self, topic, data):
         """Control system"""
-        if os.environ.get("DISPLAY") is None:
-            if self.lnxlink.display is not None:
-                os.environ["DISPLAY"] = self.lnxlink.display
-                logger.info("Initializing empty DISPLAY environment variable")
-        syscommand(f"xdotool key {data}")
+        logger.info("xdg-open %s", data)
+        syscommand(f"xdg-open {data}", background=True)
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/shutdown.py` & `lnxlink-2024.6.0/lnxlink/modules/shutdown.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Shutdown the system"""
 import logging
-from .scripts.helpers import syscommand
+from lnxlink.modules.scripts.helpers import syscommand
 
 logger = logging.getLogger("lnxlink")
 
 
 class Addon:
     """Addon module"""
 
@@ -22,12 +22,12 @@
             if returncode != 0:
                 self.lnxlink.temp_connection_callback(False)
                 logger.error("Can't restart the computer")
 
     def exposed_controls(self):
         """Exposes to home assistant"""
         return {
-            "shutdown": {
+            "Shutdown": {
                 "type": "button",
                 "icon": "mdi:power",
             }
         }
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/speaker_used.py` & `lnxlink-2024.6.0/lnxlink/modules/speaker_used.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Checks if the Speaker is used"""
 import glob
 import json
 import re
-from .scripts.helpers import syscommand
+from lnxlink.modules.scripts.helpers import syscommand
 
 
 class Addon:
     """Addon module"""
 
     def __init__(self, lnxlink):
         """Setup addon"""
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/speech_recognition.py` & `lnxlink-2024.6.0/lnxlink/modules/speech_recognition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Checks if the microphone is used"""
 from importlib import import_module
 from threading import Thread
 import logging
-from .scripts.helpers import import_install_package
+from lnxlink.modules.scripts.helpers import import_install_package
 
 logger = logging.getLogger("lnxlink")
 
 
 class Addon:
     """Addon module"""
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/statistics.py` & `lnxlink-2024.6.0/lnxlink/modules/statistics.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.5.0/lnxlink/modules/suspend.py` & `lnxlink-2024.6.0/lnxlink/modules/suspend.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Suspend/sleep the system"""
-from .scripts.helpers import syscommand
+from lnxlink.modules.scripts.helpers import syscommand
 
 
 class Addon:
     """Addon module"""
 
     def __init__(self, lnxlink):
         """Setup addon"""
@@ -12,12 +12,12 @@
     def start_control(self, topic, data):
         """Control system"""
         syscommand("systemctl suspend")
 
     def exposed_controls(self):
         """Exposes to home assistant"""
         return {
-            "suspend": {
+            "Suspend": {
                 "type": "button",
                 "icon": "mdi:progress-clock",
             }
         }
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/sys_updates.py` & `lnxlink-2024.6.0/lnxlink/modules/sys_updates.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Checks for system updates"""
 import time
 from shutil import which
-from .scripts.helpers import syscommand
+from lnxlink.modules.scripts.helpers import syscommand
 
 
 class Addon:
     """Addon module"""
 
     def __init__(self, lnxlink):
         """Setup addon"""
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/systemd.py` & `lnxlink-2024.6.0/lnxlink/modules/systemd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Controls systemd services"""
 import logging
 from shutil import which
-from .scripts.helpers import syscommand
+from lnxlink.modules.scripts.helpers import syscommand
 
 logger = logging.getLogger("lnxlink")
 
 
 class Addon:
     """Addon module"""
 
@@ -35,15 +35,15 @@
         return info
 
     def exposed_controls(self):
         """Exposes to home assistant"""
         discovery_info = {}
         for service in self.services:
             name = service.replace(".service", "")
-            discovery_info[f"systemd_{name}"] = {
+            discovery_info[f"Systemd {name}"] = {
                 "type": "switch",
                 "icon": "mdi:application-cog",
                 "value_template": f"{{{{ value_json.get('{name}') }}}}",
             }
         return discovery_info
 
     def start_control(self, topic, data):
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/temperature.py` & `lnxlink-2024.6.0/lnxlink/modules/temperature.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.5.0/lnxlink/modules/update.py` & `lnxlink-2024.6.0/lnxlink/modules/update.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Checks for LNXlink updates"""
 import re
 import sys
 import logging
 import time
 import requests
-from .scripts.helpers import syscommand
+from lnxlink.modules.scripts.helpers import syscommand
 
 logger = logging.getLogger("lnxlink")
 
 
 class Addon:
     """Addon module"""
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/webcam.py` & `lnxlink-2024.6.0/lnxlink/modules/webcam.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 """Shows an image from the webcamera"""
 import base64
-from .scripts.helpers import import_install_package
+from threading import Thread
+from lnxlink.modules.scripts.helpers import import_install_package
 
 
 class Addon:
     """Addon module"""
 
     def __init__(self, lnxlink):
         """Setup addon"""
+        self.lnxlink = lnxlink
         self.name = "Webcam"
         self.vid = None
         self._requirements()
+        self.read_thr = None
 
     def _requirements(self):
         self.lib = {
             "cv2": import_install_package("opencv-python", ">=4.7.0.68", "cv2"),
         }
 
     def get_camera_frame(self):
         """Convert camera feed to Base64 text"""
         if self.vid is not None:
-            _, frame = self.vid.read()
-            _, buffer = self.lib["cv2"].imencode(".jpg", frame)
-            frame = base64.b64encode(buffer)
-            return frame
-        return None
+            while True:
+                _, frame = self.vid.read()
+                _, buffer = self.lib["cv2"].imencode(".jpg", frame)
+                frame = base64.b64encode(buffer)
+                self.lnxlink.run_module(f"{self.name}/Webcam feed", frame)
 
     def get_info(self):
         """Gather information from the system"""
         if self.vid is not None:
             return True
         return False
 
@@ -38,19 +41,25 @@
             "Webcam": {
                 "type": "switch",
                 "icon": "mdi:webcam",
                 "entity_category": "config",
             },
             "Webcam feed": {
                 "type": "camera",
-                "method": self.get_camera_frame,
                 "encoding": "b64",
+                "subtopic": True,
             },
         }
 
     def start_control(self, topic, data):
         """Control system"""
         if data.lower() == "off":
             self.vid.release()
             self.vid = None
+            if self.read_thr is not None:
+                self.read_thr.join()
+                self.read_thr = None
         elif data.lower() == "on":
             self.vid = self.lib["cv2"].VideoCapture(0)
+            if self.read_thr is None:
+                self.read_thr = Thread(target=self.get_camera_frame, daemon=True)
+                self.read_thr.start()
```

### Comparing `lnxlink-2024.5.0/lnxlink/modules/wifi.py` & `lnxlink-2024.6.0/lnxlink/modules/wifi.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Gets WiFi information"""
 import os
 import re
 from shutil import which
-from .scripts.helpers import syscommand
+from lnxlink.modules.scripts.helpers import syscommand
 
 
 class Addon:
     """Addon module"""
 
     def __init__(self, lnxlink):
         """Setup addon"""
```

### Comparing `lnxlink-2024.5.0/lnxlink/system_monitor.py` & `lnxlink-2024.6.0/lnxlink/system_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Monitors for shutdown/sleep events"""
 
 import threading
 import signal
 import logging
 import traceback
 
-from .modules.scripts.helpers import import_install_package
+from lnxlink.modules.scripts.helpers import import_install_package
 
 logger = logging.getLogger("lnxlink")
 
 
 class MonitorSuspend:
     """Monitor DBUS for Suspend and Shutdown events"""
```

### Comparing `lnxlink-2024.5.0/lnxlink.egg-info/PKG-INFO` & `lnxlink-2024.6.0/lnxlink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnxlink
-Version: 2024.5.0
+Version: 2024.6.0
 Summary: Internet Of Things (IOT) integration with Linux using MQTT
 Home-page: https://bkbilly.github.io/lnxlink
 Author-email: bkbilly <bkbilly@hotmail.com>
 Project-URL: Source Code, https://github.com/bkbilly/lnxlink
 Project-URL: Documentation, https://bkbilly.gitbook.io/lnxlink
 Keywords: lnxlink
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lnxlink-2024.5.0/lnxlink.egg-info/SOURCES.txt` & `lnxlink-2024.6.0/lnxlink.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,23 +21,25 @@
 lnxlink/modules/boot_select.py
 lnxlink/modules/brightness.py
 lnxlink/modules/camera_used.py
 lnxlink/modules/cpu.py
 lnxlink/modules/disk_usage.py
 lnxlink/modules/display_env.py
 lnxlink/modules/fullscreen.py
+lnxlink/modules/gamepad.py
 lnxlink/modules/gpio.py
 lnxlink/modules/gpu.py
 lnxlink/modules/idle.py
 lnxlink/modules/inference_time.py
 lnxlink/modules/keep_alive.py
 lnxlink/modules/keyboard_hotkeys.py
 lnxlink/modules/media.py
 lnxlink/modules/memory.py
 lnxlink/modules/microphone_used.py
+lnxlink/modules/mounts.py
 lnxlink/modules/mouse.py
 lnxlink/modules/network.py
 lnxlink/modules/notify.py
 lnxlink/modules/power_profile.py
 lnxlink/modules/required_restart.py
 lnxlink/modules/restart.py
 lnxlink/modules/screen_onoff.py
```

### Comparing `lnxlink-2024.5.0/pyproject.toml` & `lnxlink-2024.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=68.0.0", "wheel~=0.40.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name              = "lnxlink"
-version           = "2024.5.0"
+version           = "2024.6.0"
 description       = "Internet Of Things (IOT) integration with Linux using MQTT"
 readme            = "README.md"
 keywords          = ["lnxlink"]
 requires-python   = ">=3.7.0"
 authors     = [
     {name="bkbilly", email="bkbilly@hotmail.com"}
 ]
```

