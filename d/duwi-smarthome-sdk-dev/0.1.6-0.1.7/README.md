# Comparing `tmp/duwi_smarthome_sdk_dev-0.1.6.tar.gz` & `tmp/duwi_smarthome_sdk_dev-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duwi_smarthome_sdk_dev-0.1.6.tar", last modified: Mon May 27 08:11:47 2024, max compression
+gzip compressed data, was "duwi_smarthome_sdk_dev-0.1.7.tar", last modified: Fri May 31 01:17:10 2024, max compression
```

## Comparing `duwi_smarthome_sdk_dev-0.1.6.tar` & `duwi_smarthome_sdk_dev-0.1.7.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 08:11:47.791089 duwi_smarthome_sdk_dev-0.1.6/
--rw-rw-rw-   0        0        0      722 2024-05-27 08:11:47.790087 duwi_smarthome_sdk_dev-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      163 2024-05-22 07:02:05.000000 duwi_smarthome_sdk_dev-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 08:11:47.722397 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 08:11:47.747531 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/api/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/api/__init__.py
--rw-rw-rw-   0        0        0     2452 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/api/account.py
--rw-rw-rw-   0        0        0     2037 2024-05-22 08:25:29.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/api/control.py
--rw-rw-rw-   0        0        0     4560 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/api/discover.py
--rw-rw-rw-   0        0        0     2671 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/api/floor.py
--rw-rw-rw-   0        0        0     5160 2024-05-23 02:34:08.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/api/group.py
--rw-rw-rw-   0        0        0     2699 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/api/house.py
--rw-rw-rw-   0        0        0     2169 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/api/refresh_token.py
--rw-rw-rw-   0        0        0     2779 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/api/room.py
--rw-rw-rw-   0        0        0     3161 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/api/terminal.py
--rw-rw-rw-   0        0        0     5130 2024-05-23 05:39:52.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/api/ws.py
-drwxrwxrwx   0        0        0        0 2024-05-27 08:11:47.752045 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/const/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/const/__init__.py
--rw-rw-rw-   0        0        0       81 2024-05-15 13:06:39.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/const/const.py
--rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/const/status.py
--rw-rw-rw-   0        0        0     2022 2024-05-27 07:44:21.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/const/type_map.py
-drwxrwxrwx   0        0        0        0 2024-05-27 08:11:47.753039 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/model/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 08:11:47.756039 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/model/req/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/model/req/__init__.py
--rw-rw-rw-   0        0        0     1020 2024-05-22 08:22:28.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/model/req/device_control.py
-drwxrwxrwx   0        0        0        0 2024-05-27 08:11:47.768046 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/model/resp/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/model/resp/__init__.py
--rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/model/resp/auth.py
--rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/model/resp/control.py
--rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/model/resp/device.py
--rw-rw-rw-   0        0        0      901 2024-05-10 01:13:17.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/model/resp/floor.py
--rw-rw-rw-   0        0        0     5369 2024-05-22 07:01:14.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/model/resp/group.py
--rw-rw-rw-   0        0        0     1722 2024-05-10 01:15:23.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/model/resp/house.py
--rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/model/resp/room.py
--rw-rw-rw-   0        0        0     1185 2024-05-14 02:44:23.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/model/resp/terminal.py
-drwxrwxrwx   0        0        0        0 2024-05-27 08:11:47.773044 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/util/__init__.py
--rw-rw-rw-   0        0        0     1848 2024-05-10 01:19:10.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/util/http.py
--rw-rw-rw-   0        0        0      522 2024-05-10 01:19:53.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/util/sign.py
--rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/util/timestamp.py
-drwxrwxrwx   0        0        0        0 2024-05-27 08:11:47.790087 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev.egg-info/
--rw-rw-rw-   0        0        0      722 2024-05-27 08:11:47.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1861 2024-05-27 08:11:47.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 08:11:47.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-27 08:11:47.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-27 08:11:47.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-05-27 08:11:47.000000 duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 08:11:47.792043 duwi_smarthome_sdk_dev-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      950 2024-05-27 08:11:46.000000 duwi_smarthome_sdk_dev-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-27 08:11:47.774040 duwi_smarthome_sdk_dev-0.1.6/test/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.6/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 08:11:47.788098 duwi_smarthome_sdk_dev-0.1.6/test/api/
--rw-rw-rw-   0        0        0        0 2024-05-22 02:20:40.000000 duwi_smarthome_sdk_dev-0.1.6/test/api/__init__.py
--rw-rw-rw-   0        0        0      731 2024-05-22 03:11:13.000000 duwi_smarthome_sdk_dev-0.1.6/test/api/test_account.py
--rw-rw-rw-   0        0        0      988 2024-05-22 08:26:30.000000 duwi_smarthome_sdk_dev-0.1.6/test/api/test_control.py
--rw-rw-rw-   0        0        0      829 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.6/test/api/test_discover.py
--rw-rw-rw-   0        0        0      796 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.6/test/api/test_floor.py
--rw-rw-rw-   0        0        0      765 2024-05-22 03:16:30.000000 duwi_smarthome_sdk_dev-0.1.6/test/api/test_group.py
--rw-rw-rw-   0        0        0      695 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.6/test/api/test_house.py
--rw-rw-rw-   0        0        0      648 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.6/test/api/test_login.py
--rw-rw-rw-   0        0        0      732 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.6/test/api/test_room.py
--rw-rw-rw-   0        0        0      740 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.6/test/api/test_terminal.py
--rw-rw-rw-   0        0        0     1228 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.6/test/api/test_ws.py
+drwxrwxrwx   0        0        0        0 2024-05-31 01:17:10.077580 duwi_smarthome_sdk_dev-0.1.7/
+-rw-rw-rw-   0        0        0      722 2024-05-31 01:17:10.076579 duwi_smarthome_sdk_dev-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2024-05-22 07:02:05.000000 duwi_smarthome_sdk_dev-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 01:17:10.005580 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 01:17:10.030579 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/api/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/api/__init__.py
+-rw-rw-rw-   0        0        0     2452 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/api/account.py
+-rw-rw-rw-   0        0        0     2037 2024-05-22 08:25:29.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/api/control.py
+-rw-rw-rw-   0        0        0     4560 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/api/discover.py
+-rw-rw-rw-   0        0        0     2671 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/api/floor.py
+-rw-rw-rw-   0        0        0     5160 2024-05-23 02:34:08.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/api/group.py
+-rw-rw-rw-   0        0        0     2699 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/api/house.py
+-rw-rw-rw-   0        0        0     2169 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/api/refresh_token.py
+-rw-rw-rw-   0        0        0     2779 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/api/room.py
+-rw-rw-rw-   0        0        0     3161 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/api/terminal.py
+-rw-rw-rw-   0        0        0     5067 2024-05-30 07:29:55.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/api/ws.py
+drwxrwxrwx   0        0        0        0 2024-05-31 01:17:10.035580 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/const/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/const/__init__.py
+-rw-rw-rw-   0        0        0       81 2024-05-15 13:06:39.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/const/const.py
+-rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/const/status.py
+-rw-rw-rw-   0        0        0     2023 2024-05-31 01:16:48.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/const/type_map.py
+drwxrwxrwx   0        0        0        0 2024-05-31 01:17:10.037580 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/model/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 01:17:10.038580 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/model/req/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/model/req/__init__.py
+-rw-rw-rw-   0        0        0     1020 2024-05-22 08:22:28.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/model/req/device_control.py
+drwxrwxrwx   0        0        0        0 2024-05-31 01:17:10.050580 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/model/resp/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/model/resp/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/model/resp/auth.py
+-rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/model/resp/control.py
+-rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/model/resp/device.py
+-rw-rw-rw-   0        0        0      901 2024-05-10 01:13:17.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/model/resp/floor.py
+-rw-rw-rw-   0        0        0     5369 2024-05-22 07:01:14.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/model/resp/group.py
+-rw-rw-rw-   0        0        0     1722 2024-05-10 01:15:23.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/model/resp/house.py
+-rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/model/resp/room.py
+-rw-rw-rw-   0        0        0     1185 2024-05-14 02:44:23.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/model/resp/terminal.py
+drwxrwxrwx   0        0        0        0 2024-05-31 01:17:10.055580 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/util/__init__.py
+-rw-rw-rw-   0        0        0     1848 2024-05-10 01:19:10.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/util/http.py
+-rw-rw-rw-   0        0        0      522 2024-05-10 01:19:53.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/util/sign.py
+-rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/util/timestamp.py
+drwxrwxrwx   0        0        0        0 2024-05-31 01:17:10.075580 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev.egg-info/
+-rw-rw-rw-   0        0        0      722 2024-05-31 01:17:09.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1861 2024-05-31 01:17:09.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 01:17:09.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-31 01:17:09.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-31 01:17:09.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-05-31 01:17:09.000000 duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 01:17:10.077580 duwi_smarthome_sdk_dev-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      950 2024-05-31 01:17:07.000000 duwi_smarthome_sdk_dev-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 01:17:10.056579 duwi_smarthome_sdk_dev-0.1.7/test/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.7/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 01:17:10.073580 duwi_smarthome_sdk_dev-0.1.7/test/api/
+-rw-rw-rw-   0        0        0        0 2024-05-22 02:20:40.000000 duwi_smarthome_sdk_dev-0.1.7/test/api/__init__.py
+-rw-rw-rw-   0        0        0      731 2024-05-22 03:11:13.000000 duwi_smarthome_sdk_dev-0.1.7/test/api/test_account.py
+-rw-rw-rw-   0        0        0      988 2024-05-22 08:26:30.000000 duwi_smarthome_sdk_dev-0.1.7/test/api/test_control.py
+-rw-rw-rw-   0        0        0      977 2024-05-27 09:50:20.000000 duwi_smarthome_sdk_dev-0.1.7/test/api/test_discover.py
+-rw-rw-rw-   0        0        0      796 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.7/test/api/test_floor.py
+-rw-rw-rw-   0        0        0      765 2024-05-22 03:16:30.000000 duwi_smarthome_sdk_dev-0.1.7/test/api/test_group.py
+-rw-rw-rw-   0        0        0      695 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.7/test/api/test_house.py
+-rw-rw-rw-   0        0        0      648 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.7/test/api/test_login.py
+-rw-rw-rw-   0        0        0      732 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.7/test/api/test_room.py
+-rw-rw-rw-   0        0        0      740 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.7/test/api/test_terminal.py
+-rw-rw-rw-   0        0        0     1228 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.7/test/api/test_ws.py
```

### Comparing `duwi_smarthome_sdk_dev-0.1.6/PKG-INFO` & `duwi_smarthome_sdk_dev-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smarthome_sdk_dev
-Version: 0.1.6
+Version: 0.1.7
 Summary: sdk for duwi third platform
 Home-page: https://github.com/duwi2024/homeassistant-sdk
 Author: duwi
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/api/account.py` & `duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/api/account.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/api/control.py` & `duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/api/control.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/api/discover.py` & `duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/api/discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/api/floor.py` & `duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/api/floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/api/group.py` & `duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/api/group.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/api/house.py` & `duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/api/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/api/refresh_token.py` & `duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/api/refresh_token.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/api/room.py` & `duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/api/room.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/api/terminal.py` & `duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/api/terminal.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/api/ws.py` & `duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/api/ws.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,12 +135,11 @@
                 _LOGGER.error(f'An error occurred during keep_alive: {e}')
 
     async def process_messages(self):
         async for message in self._connection:
             try:
                 if message == "KEEPALIVE":
                     continue
-                _LOGGER.info(f"ws receive message:{message}")
                 message = str.replace(message, "&excision&", "")
                 await self._on_callback(message)
             except Exception as e:
                 _LOGGER.error(f"error message detail: \n{traceback.format_exc()}")
```

### Comparing `duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/const/status.py` & `duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/const/status.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/const/type_map.py` & `duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/const/type_map.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,41 +31,40 @@
     "8-001-003": "XiangWangMusicS8",
     "8-001-004": "ShengBiKeMusic",
     "8-001-005": "BoShengMusic",
     "8-001-006": "SonosMusic",
 }
 
 sensor_type_map = {
-    "7-001-001": ["Temperature"],
-    "7-001-002": ["Temperature"],
-    "7-002-001": ["Humidity"],
-    "7-003-001": ["Light"],
-    "7-004-001": ["Formaldehyde"],
-    "7-005-001": ["Pm25"],
-    "7-006-001": ["CarbonDioxide"],
-    "7-007-001": ["AirQuality"],
-    "7-008-001": ["Human"],
-    "7-008-002": ["Human"],
-    "7-009-001": ["Trigger"],
-    "7-009-002": ["Trigger"],
-    "7-009-003": ["Trigger"],
-    "7-009-004": ["Trigger"],
-    "7-009-005": ["Trigger"],
-    "7-009-006": ["Trigger"],
-    "7-009-007": ["Trigger"],
-    "7-009-008": ["Trigger"],
-    "7-009-009": ["Trigger"],
-    "7-009-010": ["Trigger"],
-    "7-010-001": ["CarbonMonoxide"],
-    "7-011-001": ["Tvoc"],
-    "7-012-001": ["Temperature", "Humidity", "Tvoc", "Formaldehyde", "Pm25", "CarbonDioxide", "Pm10", "AirQuality"],
-    "7-012-002": ["CarbonMonoxide"],
-    "7-013-001": ["Light", "Human"],
+    "7-001-001": ["temperature"],
+    "7-002-001": ["humidity"],
+    "7-003-001": ["light"],
+    "7-004-001": ["formaldehyde"],
+    "7-005-001": ["pm25"],
+    "7-006-001": ["carbon_dioxide"],
+    "7-007-001": ["air_quality"],
+    "7-008-001": ["human"],
+    "7-008-002": ["human"],
+    "7-008-003": ["human", "light"],
+    "7-009-001": ["trigger"],
+    "7-009-002": ["trigger"],
+    "7-009-003": ["trigger", "light"],
+    "7-009-004": ["trigger"],
+    "7-009-005": ["trigger"],
+    "7-009-006": ["trigger"],
+    "7-009-007": ["trigger"],
+    "7-009-008": ["trigger"],
+    "7-009-009": ["trigger"],
+    "7-009-010": ["trigger"],
+    "7-010-001": ["carbon_monoxide"],
+    "7-011-001": ["tvoc"],
+    "7-012-001": ["temperature", "humidity", "tvoc", "pm25", "formaldehyde", "carbon_dioxide", "pm10"],
+    "7-012-002": ["carbon_monoxide"],
+    "7-013-001": ["light", "human"],
 }
-
 group_type_map = {
     "SWITCH": {
         "Breaker": "On",
     },
     "LIGHT": {
         "Light": "Dim",
         "Color": "Temp",
```

### Comparing `duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/model/req/device_control.py` & `duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/model/req/device_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/model/resp/auth.py` & `duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/model/resp/auth.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/model/resp/device.py` & `duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/model/resp/device.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/model/resp/floor.py` & `duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/model/resp/floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/model/resp/group.py` & `duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/model/resp/group.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/model/resp/house.py` & `duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/model/resp/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/model/resp/room.py` & `duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/model/resp/room.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/model/resp/terminal.py` & `duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/model/resp/terminal.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/util/http.py` & `duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/util/http.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev/util/sign.py` & `duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev/util/sign.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev.egg-info/PKG-INFO` & `duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smarthome_sdk_dev
-Version: 0.1.6
+Version: 0.1.7
 Summary: sdk for duwi third platform
 Home-page: https://github.com/duwi2024/homeassistant-sdk
 Author: duwi
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smarthome_sdk_dev-0.1.6/duwi_smarthome_sdk_dev.egg-info/SOURCES.txt` & `duwi_smarthome_sdk_dev-0.1.7/duwi_smarthome_sdk_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/setup.py` & `duwi_smarthome_sdk_dev-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.6'
+VERSION = '0.1.7'
 DESCRIPTION = 'sdk for duwi third platform'
 
 setup(
     name="duwi_smarthome_sdk_dev",
     version=VERSION,
     author="duwi",
     author_email="ledgerbiggg@gmail.com",
```

### Comparing `duwi_smarthome_sdk_dev-0.1.6/test/api/test_account.py` & `duwi_smarthome_sdk_dev-0.1.7/test/api/test_account.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/test/api/test_control.py` & `duwi_smarthome_sdk_dev-0.1.7/test/api/test_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/test/api/test_discover.py` & `duwi_smarthome_sdk_dev-0.1.7/test/api/test_group.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import asyncio
 from unittest import TestCase
-from duwi_smarthome_sdk_dev.api.discover import DiscoverClient
-from duwi_smarthome_sdk_dev.model.resp.device import Device
+from duwi_smarthome_sdk_dev.api.group import GroupClient
 
 
 class TestDiscoverClient(TestCase):
     def test_discover(self):
         async def run_test():
-            cc = DiscoverClient(
+            cc = GroupClient(
                 app_key="2e479831-1fb7-751e-7017-7534f7f99fc1",
                 app_secret="26af4883a943083a4c34083897fcea10",
                 access_token="715d1c63-85c0-4d74-9a89-5a0aa4806f74",
                 app_version="0.0.1",
                 client_version="0.0.1",
                 client_model="homeassistant",
             )
 
-            rexs = await cc.discover(
+            res = await cc.discover_groups(
                 house_no="c7bf567d-225a-4533-ab72-5dc080b794f5",
             )
             print(res)
 
         asyncio.run(run_test())
```

### Comparing `duwi_smarthome_sdk_dev-0.1.6/test/api/test_floor.py` & `duwi_smarthome_sdk_dev-0.1.7/test/api/test_floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/test/api/test_group.py` & `duwi_smarthome_sdk_dev-0.1.7/test/api/test_discover.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import asyncio
 from unittest import TestCase
-from duwi_smarthome_sdk_dev.api.group import GroupClient
+from duwi_smarthome_sdk_dev.api.discover import DiscoverClient
+from duwi_smarthome_sdk_dev.model.resp.device import Device
 
 
 class TestDiscoverClient(TestCase):
     def test_discover(self):
         async def run_test():
-            cc = GroupClient(
+            cc = DiscoverClient(
                 app_key="2e479831-1fb7-751e-7017-7534f7f99fc1",
                 app_secret="26af4883a943083a4c34083897fcea10",
                 access_token="715d1c63-85c0-4d74-9a89-5a0aa4806f74",
                 app_version="0.0.1",
                 client_version="0.0.1",
                 client_model="homeassistant",
             )
 
-            res = await cc.discover_groups(
+            status,devices = await cc.discover(
                 house_no="c7bf567d-225a-4533-ab72-5dc080b794f5",
             )
-            print(res)
-
+            print(status)
+            for d in devices:
+                if d.device_type_no.startswith("8"):
+                    print(d)
+            print(1)
         asyncio.run(run_test())
```

### Comparing `duwi_smarthome_sdk_dev-0.1.6/test/api/test_house.py` & `duwi_smarthome_sdk_dev-0.1.7/test/api/test_house.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/test/api/test_login.py` & `duwi_smarthome_sdk_dev-0.1.7/test/api/test_login.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/test/api/test_room.py` & `duwi_smarthome_sdk_dev-0.1.7/test/api/test_room.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/test/api/test_terminal.py` & `duwi_smarthome_sdk_dev-0.1.7/test/api/test_terminal.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.6/test/api/test_ws.py` & `duwi_smarthome_sdk_dev-0.1.7/test/api/test_ws.py`

 * *Files identical despite different names*

