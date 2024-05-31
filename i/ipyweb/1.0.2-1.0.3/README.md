# Comparing `tmp/ipyweb-1.0.2.tar.gz` & `tmp/ipyweb-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyweb-1.0.2.tar", last modified: Fri May 31 07:24:12 2024, max compression
+gzip compressed data, was "ipyweb-1.0.3.tar", last modified: Fri May 31 12:46:40 2024, max compression
```

## Comparing `ipyweb-1.0.2.tar` & `ipyweb-1.0.3.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 07:24:12.019479 ipyweb-1.0.2/
--rw-rw-rw-   0        0        0     1547 2024-05-16 17:34:29.000000 ipyweb-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     2193 2024-05-31 07:24:12.017479 ipyweb-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       43 2024-05-31 07:23:39.000000 ipyweb-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 07:24:11.886666 ipyweb-1.0.2/ipyweb/
--rw-rw-rw-   0        0        0        0 2024-05-31 04:11:12.000000 ipyweb-1.0.2/ipyweb/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:24:11.904654 ipyweb-1.0.2/ipyweb/addons/
--rw-rw-rw-   0        0        0     3561 2024-05-31 01:15:14.000000 ipyweb-1.0.2/ipyweb/addons/loadingGui.py
--rw-rw-rw-   0        0        0     3713 2024-05-30 23:10:57.000000 ipyweb-1.0.2/ipyweb/app.py
--rw-rw-rw-   0        0        0     4768 2024-05-31 06:41:51.000000 ipyweb-1.0.2/ipyweb/appRunner.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:24:11.907401 ipyweb-1.0.2/ipyweb/builds/
--rw-rw-rw-   0        0        0     7351 2024-05-31 01:13:37.000000 ipyweb-1.0.2/ipyweb/builds/builder.py
--rw-rw-rw-   0        0        0     4779 2024-05-31 01:50:03.000000 ipyweb-1.0.2/ipyweb/cache.py
--rw-rw-rw-   0        0        0      316 2024-05-31 07:19:21.000000 ipyweb-1.0.2/ipyweb/cli.py
--rw-rw-rw-   0        0        0     3568 2024-05-31 00:44:58.000000 ipyweb-1.0.2/ipyweb/command.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:24:11.913439 ipyweb-1.0.2/ipyweb/commands/
--rw-rw-rw-   0        0        0      804 2024-05-31 07:10:00.000000 ipyweb-1.0.2/ipyweb/commands/ipywebBuilder.py
--rw-rw-rw-   0        0        0     2160 2024-05-31 07:07:45.000000 ipyweb-1.0.2/ipyweb/commands/ipywebRunner.py
--rw-rw-rw-   0        0        0     9544 2024-05-31 06:57:42.000000 ipyweb-1.0.2/ipyweb/config.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:24:11.933820 ipyweb-1.0.2/ipyweb/configs/
--rw-rw-rw-   0        0        0     1010 2024-05-28 16:39:36.000000 ipyweb-1.0.2/ipyweb/configs/app.py
--rw-rw-rw-   0        0        0      363 2024-05-30 15:55:41.000000 ipyweb-1.0.2/ipyweb/configs/build.py
--rw-rw-rw-   0        0        0      225 2024-05-12 09:40:00.000000 ipyweb-1.0.2/ipyweb/configs/cache.py
--rw-rw-rw-   0        0        0     1050 2024-05-12 09:51:21.000000 ipyweb-1.0.2/ipyweb/configs/database.py
--rw-rw-rw-   0        0        0       62 2024-05-10 17:35:35.000000 ipyweb-1.0.2/ipyweb/configs/jsonFile.py
--rw-rw-rw-   0        0        0     1130 2024-05-29 18:24:21.000000 ipyweb-1.0.2/ipyweb/configs/logger.py
--rw-rw-rw-   0        0        0     2881 2024-05-30 15:55:40.000000 ipyweb-1.0.2/ipyweb/configs/windows.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:24:11.954853 ipyweb-1.0.2/ipyweb/contracts/
--rw-rw-rw-   0        0        0      104 2024-05-30 15:55:41.000000 ipyweb-1.0.2/ipyweb/contracts/ipywebAddon.py
--rw-rw-rw-   0        0        0      641 2024-05-30 15:55:41.000000 ipyweb-1.0.2/ipyweb/contracts/ipywebController.py
--rw-rw-rw-   0        0        0      422 2024-05-30 15:55:41.000000 ipyweb-1.0.2/ipyweb/contracts/ipywebException.py
--rw-rw-rw-   0        0        0      892 2024-05-30 15:55:40.000000 ipyweb-1.0.2/ipyweb/contracts/ipywebHttpController.py
--rw-rw-rw-   0        0        0      154 2024-05-30 15:55:41.000000 ipyweb-1.0.2/ipyweb/contracts/ipywebModel.py
--rw-rw-rw-   0        0        0      410 2024-05-30 15:55:41.000000 ipyweb-1.0.2/ipyweb/contracts/ipywebPreload.py
--rw-rw-rw-   0        0        0       93 2024-05-30 19:22:02.000000 ipyweb-1.0.2/ipyweb/contracts/ipywebQueue.py
--rw-rw-rw-   0        0        0      154 2024-05-31 01:10:19.000000 ipyweb-1.0.2/ipyweb/contracts/ipywebRunner.py
--rw-rw-rw-   0        0        0     6971 2024-05-31 06:56:48.000000 ipyweb-1.0.2/ipyweb/controller.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:24:11.956848 ipyweb-1.0.2/ipyweb/controllers/
--rw-rw-rw-   0        0        0     7470 2024-05-30 19:21:48.000000 ipyweb-1.0.2/ipyweb/controllers/ipyweb.py
--rw-rw-rw-   0        0        0     4646 2024-05-31 01:49:46.000000 ipyweb-1.0.2/ipyweb/db.py
--rw-rw-rw-   0        0        0    10557 2024-05-31 00:27:17.000000 ipyweb-1.0.2/ipyweb/event.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:24:11.810438 ipyweb-1.0.2/ipyweb/events/
-drwxrwxrwx   0        0        0        0 2024-05-31 07:24:11.959858 ipyweb-1.0.2/ipyweb/events/listener/
--rw-rw-rw-   0        0        0      453 2024-05-30 19:21:37.000000 ipyweb-1.0.2/ipyweb/events/listener/windows.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:24:11.963654 ipyweb-1.0.2/ipyweb/events/register/
--rw-rw-rw-   0        0        0      686 2024-05-30 19:21:42.000000 ipyweb-1.0.2/ipyweb/events/register/windows.py
--rw-rw-rw-   0        0        0     1699 2024-05-30 15:56:03.000000 ipyweb-1.0.2/ipyweb/gui.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:24:11.978526 ipyweb-1.0.2/ipyweb/guis/
--rw-rw-rw-   0        0        0      987 2024-05-30 15:55:41.000000 ipyweb-1.0.2/ipyweb/guis/BottleServer.py
--rw-rw-rw-   0        0        0     3822 2024-05-30 15:55:41.000000 ipyweb-1.0.2/ipyweb/guis/FlaskServer.py
--rw-rw-rw-   0        0        0     3922 2024-05-30 15:56:03.000000 ipyweb-1.0.2/ipyweb/guis/IpywebServer.py
--rw-rw-rw-   0        0        0     1491 2024-05-31 01:07:59.000000 ipyweb-1.0.2/ipyweb/guis/LocalServer.py
--rw-rw-rw-   0        0        0     1446 2024-05-30 19:21:31.000000 ipyweb-1.0.2/ipyweb/guis/RemoteServer.py
--rw-rw-rw-   0        0        0     6365 2024-05-31 00:15:56.000000 ipyweb-1.0.2/ipyweb/ipyweb.py
--rw-rw-rw-   0        0        0     2546 2024-05-31 00:12:02.000000 ipyweb-1.0.2/ipyweb/jsonFile.py
--rw-rw-rw-   0        0        0     2379 2024-05-31 00:08:13.000000 ipyweb-1.0.2/ipyweb/logger.py
--rw-rw-rw-   0        0        0     7935 2024-05-31 00:45:17.000000 ipyweb-1.0.2/ipyweb/module.py
--rw-rw-rw-   0        0        0      247 2024-05-05 11:24:12.000000 ipyweb-1.0.2/ipyweb/multiton.py
--rw-rw-rw-   0        0        0     8722 2024-05-31 00:04:40.000000 ipyweb-1.0.2/ipyweb/preload.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:24:11.815413 ipyweb-1.0.2/ipyweb/preloads/
-drwxrwxrwx   0        0        0        0 2024-05-31 07:24:11.986066 ipyweb-1.0.2/ipyweb/preloads/block/
--rw-rw-rw-   0        0        0     1555 2024-05-31 01:00:22.000000 ipyweb-1.0.2/ipyweb/preloads/block/controllerPreload.py
--rw-rw-rw-   0        0        0      404 2024-05-30 15:56:03.000000 ipyweb-1.0.2/ipyweb/preloads/block/guiPreload.py
--rw-rw-rw-   0        0        0      420 2024-05-30 15:56:03.000000 ipyweb-1.0.2/ipyweb/preloads/block/processPreload.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:24:11.989130 ipyweb-1.0.2/ipyweb/preloads/process/
--rw-rw-rw-   0        0        0      487 2024-05-30 19:20:37.000000 ipyweb-1.0.2/ipyweb/preloads/process/examplePreload.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:24:11.998074 ipyweb-1.0.2/ipyweb/preloads/thread/
--rw-rw-rw-   0        0        0     2981 2024-05-31 01:03:40.000000 ipyweb-1.0.2/ipyweb/preloads/thread/queuePreload.py
--rw-rw-rw-   0        0        0     2953 2024-05-31 01:04:52.000000 ipyweb-1.0.2/ipyweb/preloads/thread/socketPreload.py
--rw-rw-rw-   0        0        0     2216 2024-05-31 01:06:07.000000 ipyweb-1.0.2/ipyweb/preloads/thread/timerPreload.py
--rw-rw-rw-   0        0        0    10336 2024-05-31 00:02:01.000000 ipyweb-1.0.2/ipyweb/process.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:24:12.000077 ipyweb-1.0.2/ipyweb/pywebview/
--rw-rw-rw-   0        0        0     9338 2024-05-31 02:33:23.000000 ipyweb-1.0.2/ipyweb/pywebview/windows.py
--rw-rw-rw-   0        0        0     4590 2024-05-31 06:58:32.000000 ipyweb-1.0.2/ipyweb/service.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:24:12.009483 ipyweb-1.0.2/ipyweb/services/
--rw-rw-rw-   0        0        0     8228 2024-05-31 01:18:35.000000 ipyweb-1.0.2/ipyweb/services/queue.py
--rw-rw-rw-   0        0        0     7691 2024-05-31 01:49:00.000000 ipyweb-1.0.2/ipyweb/services/socketServer.py
--rw-rw-rw-   0        0        0     2671 2024-05-31 00:49:24.000000 ipyweb-1.0.2/ipyweb/services/timer.py
--rw-rw-rw-   0        0        0      470 2024-05-05 11:23:41.000000 ipyweb-1.0.2/ipyweb/singleton.py
--rw-rw-rw-   0        0        0     5026 2024-05-30 23:58:28.000000 ipyweb-1.0.2/ipyweb/thread.py
--rw-rw-rw-   0        0        0     3755 2024-05-31 06:37:42.000000 ipyweb-1.0.2/ipyweb/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:24:12.011479 ipyweb-1.0.2/ipyweb/windowEvents/
--rw-rw-rw-   0        0        0     2163 2024-05-30 15:55:41.000000 ipyweb-1.0.2/ipyweb/windowEvents/main.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:24:12.015540 ipyweb-1.0.2/ipyweb.egg-info/
--rw-rw-rw-   0        0        0     2193 2024-05-31 07:24:11.000000 ipyweb-1.0.2/ipyweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1814 2024-05-31 07:24:11.000000 ipyweb-1.0.2/ipyweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 07:24:11.000000 ipyweb-1.0.2/ipyweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-05-31 07:24:11.000000 ipyweb-1.0.2/ipyweb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       25 2024-05-31 07:24:11.000000 ipyweb-1.0.2/ipyweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-31 07:24:11.000000 ipyweb-1.0.2/ipyweb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1185 2024-05-31 04:23:20.000000 ipyweb-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-31 07:24:12.019479 ipyweb-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.522474 ipyweb-1.0.3/
+-rw-rw-rw-   0        0        0     1547 2024-05-16 17:34:29.000000 ipyweb-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2193 2024-05-31 12:46:40.520954 ipyweb-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2024-05-31 07:23:39.000000 ipyweb-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.402821 ipyweb-1.0.3/ipyweb/
+-rw-rw-rw-   0        0        0        0 2024-05-31 04:11:12.000000 ipyweb-1.0.3/ipyweb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.421437 ipyweb-1.0.3/ipyweb/addons/
+-rw-rw-rw-   0        0        0     3561 2024-05-31 01:15:14.000000 ipyweb-1.0.3/ipyweb/addons/loadingGui.py
+-rw-rw-rw-   0        0        0     3713 2024-05-30 23:10:57.000000 ipyweb-1.0.3/ipyweb/app.py
+-rw-rw-rw-   0        0        0     4937 2024-05-31 12:45:56.000000 ipyweb-1.0.3/ipyweb/appRunner.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.423461 ipyweb-1.0.3/ipyweb/builds/
+-rw-rw-rw-   0        0        0     7351 2024-05-31 01:13:37.000000 ipyweb-1.0.3/ipyweb/builds/builder.py
+-rw-rw-rw-   0        0        0     4779 2024-05-31 01:50:03.000000 ipyweb-1.0.3/ipyweb/cache.py
+-rw-rw-rw-   0        0        0      316 2024-05-31 07:19:21.000000 ipyweb-1.0.3/ipyweb/cli.py
+-rw-rw-rw-   0        0        0     3568 2024-05-31 00:44:58.000000 ipyweb-1.0.3/ipyweb/command.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.428465 ipyweb-1.0.3/ipyweb/commands/
+-rw-rw-rw-   0        0        0      804 2024-05-31 07:10:00.000000 ipyweb-1.0.3/ipyweb/commands/ipywebBuilder.py
+-rw-rw-rw-   0        0        0     2160 2024-05-31 07:07:45.000000 ipyweb-1.0.3/ipyweb/commands/ipywebRunner.py
+-rw-rw-rw-   0        0        0     9804 2024-05-31 11:36:50.000000 ipyweb-1.0.3/ipyweb/config.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.446566 ipyweb-1.0.3/ipyweb/configs/
+-rw-rw-rw-   0        0        0     1010 2024-05-28 16:39:36.000000 ipyweb-1.0.3/ipyweb/configs/app.py
+-rw-rw-rw-   0        0        0      363 2024-05-30 15:55:41.000000 ipyweb-1.0.3/ipyweb/configs/build.py
+-rw-rw-rw-   0        0        0      225 2024-05-12 09:40:00.000000 ipyweb-1.0.3/ipyweb/configs/cache.py
+-rw-rw-rw-   0        0        0     1050 2024-05-12 09:51:21.000000 ipyweb-1.0.3/ipyweb/configs/database.py
+-rw-rw-rw-   0        0        0       62 2024-05-10 17:35:35.000000 ipyweb-1.0.3/ipyweb/configs/jsonFile.py
+-rw-rw-rw-   0        0        0     1130 2024-05-29 18:24:21.000000 ipyweb-1.0.3/ipyweb/configs/logger.py
+-rw-rw-rw-   0        0        0     2881 2024-05-30 15:55:40.000000 ipyweb-1.0.3/ipyweb/configs/windows.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.466382 ipyweb-1.0.3/ipyweb/contracts/
+-rw-rw-rw-   0        0        0      104 2024-05-30 15:55:41.000000 ipyweb-1.0.3/ipyweb/contracts/ipywebAddon.py
+-rw-rw-rw-   0        0        0      641 2024-05-30 15:55:41.000000 ipyweb-1.0.3/ipyweb/contracts/ipywebController.py
+-rw-rw-rw-   0        0        0      422 2024-05-30 15:55:41.000000 ipyweb-1.0.3/ipyweb/contracts/ipywebException.py
+-rw-rw-rw-   0        0        0     1037 2024-05-31 12:37:53.000000 ipyweb-1.0.3/ipyweb/contracts/ipywebHttpController.py
+-rw-rw-rw-   0        0        0      154 2024-05-30 15:55:41.000000 ipyweb-1.0.3/ipyweb/contracts/ipywebModel.py
+-rw-rw-rw-   0        0        0      410 2024-05-30 15:55:41.000000 ipyweb-1.0.3/ipyweb/contracts/ipywebPreload.py
+-rw-rw-rw-   0        0        0       93 2024-05-30 19:22:02.000000 ipyweb-1.0.3/ipyweb/contracts/ipywebQueue.py
+-rw-rw-rw-   0        0        0      154 2024-05-31 01:10:19.000000 ipyweb-1.0.3/ipyweb/contracts/ipywebRunner.py
+-rw-rw-rw-   0        0        0     6971 2024-05-31 06:56:48.000000 ipyweb-1.0.3/ipyweb/controller.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.468382 ipyweb-1.0.3/ipyweb/controllers/
+-rw-rw-rw-   0        0        0     7422 2024-05-31 12:37:17.000000 ipyweb-1.0.3/ipyweb/controllers/ipyweb.py
+-rw-rw-rw-   0        0        0     4646 2024-05-31 01:49:46.000000 ipyweb-1.0.3/ipyweb/db.py
+-rw-rw-rw-   0        0        0    10557 2024-05-31 00:27:17.000000 ipyweb-1.0.3/ipyweb/event.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.335296 ipyweb-1.0.3/ipyweb/events/
+drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.471386 ipyweb-1.0.3/ipyweb/events/listener/
+-rw-rw-rw-   0        0        0      453 2024-05-30 19:21:37.000000 ipyweb-1.0.3/ipyweb/events/listener/windows.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.474945 ipyweb-1.0.3/ipyweb/events/register/
+-rw-rw-rw-   0        0        0      686 2024-05-30 19:21:42.000000 ipyweb-1.0.3/ipyweb/events/register/windows.py
+-rw-rw-rw-   0        0        0     1699 2024-05-30 15:56:03.000000 ipyweb-1.0.3/ipyweb/gui.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.487467 ipyweb-1.0.3/ipyweb/guis/
+-rw-rw-rw-   0        0        0      987 2024-05-30 15:55:41.000000 ipyweb-1.0.3/ipyweb/guis/BottleServer.py
+-rw-rw-rw-   0        0        0     3822 2024-05-30 15:55:41.000000 ipyweb-1.0.3/ipyweb/guis/FlaskServer.py
+-rw-rw-rw-   0        0        0     3922 2024-05-30 15:56:03.000000 ipyweb-1.0.3/ipyweb/guis/IpywebServer.py
+-rw-rw-rw-   0        0        0     1491 2024-05-31 01:07:59.000000 ipyweb-1.0.3/ipyweb/guis/LocalServer.py
+-rw-rw-rw-   0        0        0     1446 2024-05-30 19:21:31.000000 ipyweb-1.0.3/ipyweb/guis/RemoteServer.py
+-rw-rw-rw-   0        0        0     6444 2024-05-31 12:39:13.000000 ipyweb-1.0.3/ipyweb/ipyweb.py
+-rw-rw-rw-   0        0        0     2546 2024-05-31 00:12:02.000000 ipyweb-1.0.3/ipyweb/jsonFile.py
+-rw-rw-rw-   0        0        0     2379 2024-05-31 00:08:13.000000 ipyweb-1.0.3/ipyweb/logger.py
+-rw-rw-rw-   0        0        0     7935 2024-05-31 00:45:17.000000 ipyweb-1.0.3/ipyweb/module.py
+-rw-rw-rw-   0        0        0      247 2024-05-05 11:24:12.000000 ipyweb-1.0.3/ipyweb/multiton.py
+-rw-rw-rw-   0        0        0     8722 2024-05-31 00:04:40.000000 ipyweb-1.0.3/ipyweb/preload.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.339329 ipyweb-1.0.3/ipyweb/preloads/
+drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.495028 ipyweb-1.0.3/ipyweb/preloads/block/
+-rw-rw-rw-   0        0        0     1555 2024-05-31 01:00:22.000000 ipyweb-1.0.3/ipyweb/preloads/block/controllerPreload.py
+-rw-rw-rw-   0        0        0      404 2024-05-30 15:56:03.000000 ipyweb-1.0.3/ipyweb/preloads/block/guiPreload.py
+-rw-rw-rw-   0        0        0      420 2024-05-30 15:56:03.000000 ipyweb-1.0.3/ipyweb/preloads/block/processPreload.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.498024 ipyweb-1.0.3/ipyweb/preloads/process/
+-rw-rw-rw-   0        0        0      487 2024-05-30 19:20:37.000000 ipyweb-1.0.3/ipyweb/preloads/process/examplePreload.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.504555 ipyweb-1.0.3/ipyweb/preloads/thread/
+-rw-rw-rw-   0        0        0     2981 2024-05-31 01:03:40.000000 ipyweb-1.0.3/ipyweb/preloads/thread/queuePreload.py
+-rw-rw-rw-   0        0        0     2953 2024-05-31 01:04:52.000000 ipyweb-1.0.3/ipyweb/preloads/thread/socketPreload.py
+-rw-rw-rw-   0        0        0     2216 2024-05-31 01:06:07.000000 ipyweb-1.0.3/ipyweb/preloads/thread/timerPreload.py
+-rw-rw-rw-   0        0        0    10336 2024-05-31 00:02:01.000000 ipyweb-1.0.3/ipyweb/process.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.506565 ipyweb-1.0.3/ipyweb/pywebview/
+-rw-rw-rw-   0        0        0     9338 2024-05-31 02:33:23.000000 ipyweb-1.0.3/ipyweb/pywebview/windows.py
+-rw-rw-rw-   0        0        0     4587 2024-05-31 11:42:57.000000 ipyweb-1.0.3/ipyweb/service.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.513972 ipyweb-1.0.3/ipyweb/services/
+-rw-rw-rw-   0        0        0     8228 2024-05-31 01:18:35.000000 ipyweb-1.0.3/ipyweb/services/queue.py
+-rw-rw-rw-   0        0        0     7627 2024-05-31 12:38:13.000000 ipyweb-1.0.3/ipyweb/services/socketServer.py
+-rw-rw-rw-   0        0        0     2671 2024-05-31 00:49:24.000000 ipyweb-1.0.3/ipyweb/services/timer.py
+-rw-rw-rw-   0        0        0      470 2024-05-05 11:23:41.000000 ipyweb-1.0.3/ipyweb/singleton.py
+-rw-rw-rw-   0        0        0     5026 2024-05-30 23:58:28.000000 ipyweb-1.0.3/ipyweb/thread.py
+-rw-rw-rw-   0        0        0     4430 2024-05-31 12:44:27.000000 ipyweb-1.0.3/ipyweb/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.515969 ipyweb-1.0.3/ipyweb/windowEvents/
+-rw-rw-rw-   0        0        0     2163 2024-05-30 15:55:41.000000 ipyweb-1.0.3/ipyweb/windowEvents/main.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.518955 ipyweb-1.0.3/ipyweb.egg-info/
+-rw-rw-rw-   0        0        0     2193 2024-05-31 12:46:40.000000 ipyweb-1.0.3/ipyweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1814 2024-05-31 12:46:40.000000 ipyweb-1.0.3/ipyweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 12:46:40.000000 ipyweb-1.0.3/ipyweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-31 12:46:40.000000 ipyweb-1.0.3/ipyweb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       25 2024-05-31 12:46:40.000000 ipyweb-1.0.3/ipyweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-31 12:46:40.000000 ipyweb-1.0.3/ipyweb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1185 2024-05-31 12:35:10.000000 ipyweb-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-31 12:46:40.523467 ipyweb-1.0.3/setup.cfg
```

### Comparing `ipyweb-1.0.2/LICENSE` & `ipyweb-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/PKG-INFO` & `ipyweb-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyweb
-Version: 1.0.2
+Version: 1.0.3
 Summary: A business framework for launching multiple services
 Author-email: sqwindows <sqwindows@qq.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2014-2017, Roman Sirokov
         All rights reserved.
```

### Comparing `ipyweb-1.0.2/ipyweb/addons/loadingGui.py` & `ipyweb-1.0.3/ipyweb/addons/loadingGui.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/app.py` & `ipyweb-1.0.3/ipyweb/app.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/appRunner.py` & `ipyweb-1.0.3/ipyweb/appRunner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 import time
 import importlib
 from ipyweb.app import app, appIpyweb
 from ipyweb.utils import utils
+from ipyweb.logger import logger
 from ipyweb.config import config, configIpyweb
 from ipyweb.logger import logger, loggerIpyweb
 from ipyweb.singleton import singleton
 from ipyweb.pywebview.windows import windows
 
 
 class appRunner(metaclass=singleton):
@@ -65,17 +66,19 @@
     def getAppRunner(self):
         self.appName = config.moduleMaps('name',
                                          app.getName()) if app.isExe else app.getName()  # 编译后读取module应用名 非编译环境直接读取
         appModulePath = '.'.join([app.appPath, self.appName, self.appRunnerDefaultName])
         try:
             self.appRunner = utils.smartImportModule(self.appRunnerDefaultName, appModulePath, app.rootPath)
         except ModuleNotFoundError as e:
-            logger.console.error(f'The application startup module does not exist:[{appModulePath}]')
+            logger.console.error(f'The application runner module does not exist:[{appModulePath}]')
         except Exception as e:
-            logger.console.error(f'An exception occurred while retrieving the startup module:[{appModulePath}]')
+            logger.console.error(f'An exception occurred while retrieving the runner module:[{appModulePath}]')
+        if self.appRunner is None:
+            logger.console.error(f'The application runner module does not exist:[{appModulePath}]')
         return self.appRunner
 
     @classmethod
     def getAppRunnerCls(self):
         try:
             if self.appRunner:
                 appRunnerClsAttr = getattr(self.appRunner, self.appRunnerDefaultClsName)
```

### Comparing `ipyweb-1.0.2/ipyweb/builds/builder.py` & `ipyweb-1.0.3/ipyweb/builds/builder.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/cache.py` & `ipyweb-1.0.3/ipyweb/cache.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/command.py` & `ipyweb-1.0.3/ipyweb/command.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/commands/ipywebBuilder.py` & `ipyweb-1.0.3/ipyweb/commands/ipywebBuilder.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/commands/ipywebRunner.py` & `ipyweb-1.0.3/ipyweb/commands/ipywebRunner.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/config.py` & `ipyweb-1.0.3/ipyweb/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,14 @@
                     self._data[name] = dict(self._data[name], **configData)
                 else:
                     self._data.update({name: configData})
                 return True
 
         except ImportError as e:
             logger.console.error(f'Module [{str(modulePath)}] does not exist')
-            self.dynamic_import_module(name, modulePath)
         except Exception as e:
             logger.console.error(f'An exception occurred while reading the configuration file [{str(modulePath)}]: {e}')
             self._loaded = False
         return False
 
     @classmethod
     def _loadFromModules(self, modulePaths={}):
@@ -210,14 +209,18 @@
         return False
 
     @classmethod
     def _loadYaml(self, configFile=''):
         configData = {}
         try:
             import yaml
+        except ImportError:
+            logger.console.error(f'Please installer module :yaml (pip install yaml)')
+            return False
+        try:
             with open(configFile, 'r', encoding='utf-8') as stream:
                 try:
                     configData = yaml.safe_load(stream)
                 except yaml.YAMLError as e:
                     logger.console.error(f'An exception occurred while reading the yaml file: {e}')
         except Exception as e:
             logger.console.error(f'An exception occurred while opening the  yaml file: {e}')
@@ -225,15 +228,20 @@
 
     @classmethod
     def _loadFromYamlDir(self, folder='', extension='*.yaml'):
         folder = os.path.normpath(folder)
 
         if not folder or not extension:
             return False
-        import yaml
+        try:
+            import yaml
+        except ImportError:
+            logger.console.error(f'Please installer module :yaml (pip install yaml)')
+            return False
+
         for configFile in glob.glob(os.path.join(folder, extension)):
             name, ext = os.path.splitext(os.path.basename(configFile))
             try:
                 with open(configFile, 'r', encoding='utf-8') as stream:
                     try:
                         configData = yaml.safe_load(stream)
                         if configData and type(configData) == dict and len(configData) > 0:
```

### Comparing `ipyweb-1.0.2/ipyweb/configs/app.py` & `ipyweb-1.0.3/ipyweb/configs/app.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/configs/database.py` & `ipyweb-1.0.3/ipyweb/configs/database.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/configs/logger.py` & `ipyweb-1.0.3/ipyweb/configs/logger.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/configs/windows.py` & `ipyweb-1.0.3/ipyweb/configs/windows.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/contracts/ipywebController.py` & `ipyweb-1.0.3/ipyweb/contracts/ipywebController.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/contracts/ipywebHttpController.py` & `ipyweb-1.0.3/ipyweb/contracts/ipywebHttpController.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+from ipyweb.utils import utils
+from ipyweb.logger import logger
 from ipyweb.controller import controller
 from ipyweb.singleton import singleton
-from ipyweb.utils import utils
 
 
 class ipywebHttpController(metaclass=singleton):
     if utils.isModuleInstalled('flask'):
-        from flask import Blueprint
-        blueprint = Blueprint('app', __name__)
+        try:
+            from flask import Blueprint
+            blueprint = Blueprint('app', __name__)
+        except ImportError:
+            logger.console.error('flask is not installed')
 
     def __init__(self):
         if hasattr(self, 'registerRoute'): self.registerRoute()
 
     @classmethod
     def windows(self, name=''):
         return controller._getWindows(name)
```

### Comparing `ipyweb-1.0.2/ipyweb/controller.py` & `ipyweb-1.0.3/ipyweb/controller.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/controllers/ipyweb.py` & `ipyweb-1.0.3/ipyweb/controllers/ipyweb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ipyweb.app import app
 from ipyweb.singleton import singleton
 from ipyweb.contracts.ipywebController import ipywebController
 from ipyweb.pywebview.windows import windows
 
+
 class ipyweb(ipywebController, metaclass=singleton):
     def version(self, window, *args):
         try:
 
             return self.success('获取版本信息成功', {
                 'ver': app.ver,
                 'version': app.version
@@ -18,15 +19,14 @@
         try:
             if type(args) != dict:
                 return self.error('参数类型不正确')
             args['target'] = True
             if args.get('url', '') == '' and args.get('html', '') == '':
                 return self.error('html和url必须设置一个')
             flag = windows().run(args)
-            print(flag)
             if type(flag) == str:
                 return self.error(flag)
             return self.success('打开成功')
         except Exception as e:
             return self.error(f'获取版本信息异常:{e}')
 
     def set_title(self, window, args):
@@ -162,15 +162,14 @@
             return self.success('窗口大小设置成功')
         except Exception as e:
             return self.error(f'窗口大小设置异常:{e}')
 
     def open_file_dialog(self, window, args=None):
         try:
             import webview
-            print(args)
             if type(args) != dict:
                 return self.error('打开目录窗口参数异常')
             file_type = args.get('file_type', 'Image Files (*.bmp;*.jpg;*.gif)')
             file_types = (file_type, 'All files (*.*)')
             allow_multiple = args.get('allow_multiple', True)
             files = window.create_file_dialog(
                 dialog_type=webview.OPEN_DIALOG,
```

### Comparing `ipyweb-1.0.2/ipyweb/db.py` & `ipyweb-1.0.3/ipyweb/db.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/event.py` & `ipyweb-1.0.3/ipyweb/event.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/events/register/windows.py` & `ipyweb-1.0.3/ipyweb/events/register/windows.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/gui.py` & `ipyweb-1.0.3/ipyweb/gui.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/guis/BottleServer.py` & `ipyweb-1.0.3/ipyweb/guis/BottleServer.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/guis/FlaskServer.py` & `ipyweb-1.0.3/ipyweb/guis/FlaskServer.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/guis/IpywebServer.py` & `ipyweb-1.0.3/ipyweb/guis/IpywebServer.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/guis/LocalServer.py` & `ipyweb-1.0.3/ipyweb/guis/LocalServer.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/guis/RemoteServer.py` & `ipyweb-1.0.3/ipyweb/guis/RemoteServer.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/ipyweb.py` & `ipyweb-1.0.3/ipyweb/ipyweb.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import time
 from ipyweb.app import app, appIpyweb
 from ipyweb.config import configIpyweb
+from ipyweb.logger import logger
 from ipyweb.contracts import ipywebException
 from ipyweb.logger import loggerIpyweb
 from ipyweb.module import moduleIpyweb
 from ipyweb.preload import preloadIpyweb
 from ipyweb.event import eventIpyweb
 from ipyweb.appRunner import appRunner
 
@@ -87,17 +88,17 @@
                 self.bootPreloader()  # 预载器
                 self.loaded = True
             self.bootTime['ipywebEnd'] = time.time()
             self.bootTime['ipywebRun'] = self.bootTime['ipywebEnd'] - self.bootTime['ipywebStart']
             if callable(self.onPreloaded): self.onPreloaded()
             self.bootAppRunner()  # 应用启动
         except Exception as e:
-            print(f'An exception occurred during application [{appName}] boot: {e}')
+            logger.console.error(f'An exception occurred during application [{appName}] boot: {e}')
         except ipywebException as e:
-            print(f'An exception occurred during application [{appName}] boot: {e}')
+            logger.console.error(f'An exception occurred during application [{appName}] boot: {e}')
         return self
 
     @classmethod  # 重新启动
     def reboot(self, appName=''):
         self.loaded = False
         self.boot(appName, True)
         return self
@@ -106,15 +107,15 @@
     def bootAppRunner(self):
         self.bootTime['bootAppStart'] = time.time()
 
         def onWindowsOpened(appName):
             self.bootTime['bootAppEnd'] = time.time()
             self.bootTime['bootAppRun'] = self.bootTime['bootAppEnd'] - self.bootTime['bootAppStart']
             self.bootTime['totalTime'] = self.bootTime['ipywebRun'] + self.bootTime['bootAppRun']
-            print(
+            logger.console.error(
                 f'The time taken for loading basic:{round(self.bootTime["ipywebBoots"]["bootBaserRun"], 3)}s,'
                 f'The time taken for loading preload  (including application preload):{round(self.bootTime["ipywebBoots"]["bootPreloaderRun"], 3)}s,'
                 f'The time taken for windows:{round(self.bootTime["bootAppRun"], 3)}s')
             if callable(self.onOpened): self.onOpened()
 
         appRunner.setOnWindowsOpened(onWindowsOpened).boot()
         return self
```

### Comparing `ipyweb-1.0.2/ipyweb/jsonFile.py` & `ipyweb-1.0.3/ipyweb/jsonFile.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/logger.py` & `ipyweb-1.0.3/ipyweb/logger.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/module.py` & `ipyweb-1.0.3/ipyweb/module.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/preload.py` & `ipyweb-1.0.3/ipyweb/preload.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/preloads/block/controllerPreload.py` & `ipyweb-1.0.3/ipyweb/preloads/block/controllerPreload.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/preloads/thread/queuePreload.py` & `ipyweb-1.0.3/ipyweb/preloads/thread/queuePreload.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/preloads/thread/socketPreload.py` & `ipyweb-1.0.3/ipyweb/preloads/thread/socketPreload.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/preloads/thread/timerPreload.py` & `ipyweb-1.0.3/ipyweb/preloads/thread/timerPreload.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/process.py` & `ipyweb-1.0.3/ipyweb/process.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/pywebview/windows.py` & `ipyweb-1.0.3/ipyweb/pywebview/windows.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/service.py` & `ipyweb-1.0.3/ipyweb/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,19 +60,19 @@
 
             if hasattr(classModule, className):
                 classAttr = getattr(classModule, className)
                 classInstance = classAttr(*args, **kwargs)
                 return classInstance
             else:
                 logger.console.error(
-                    f' The name [{className}] of the instantiated service class [{invokeCls}] is incorrect')
+                    f' The name [{className}] of the instantiated module class [{invokeCls}] is incorrect')
         except ImportError as e:
-            logger.console.error(f'The instantiated service class [{str(invokeCls)}] does not exist')
+            logger.console.error(f'The instantiated module class [{str(invokeCls)}] does not exist')
         except Exception as e:
-            logger.console.error(f'An exception occurred while instantiating the service class [{invokeCls}] : {e}')
+            logger.console.error(f'An exception occurred while instantiating the module class [{invokeCls}] : {e}')
         return None
 
     @classmethod
     def _loadModule(self, invokeCls='', spaceName=app.servicesName):
         try:
             prerix = f'{app.appPath}.{app.getName()}.{app.backendName}'
             if len(invokeCls.split('.')) == 1:
```

### Comparing `ipyweb-1.0.2/ipyweb/services/queue.py` & `ipyweb-1.0.3/ipyweb/services/queue.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/services/socketServer.py` & `ipyweb-1.0.3/ipyweb/services/socketServer.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,14 @@
                 try:
                     if callable(onMessage): await onMessage(message)
                 except Exception as e:
                     onError = self.config.get('onError', None)
                     if callable(onError):
                         await onError(e)
         # except websockets.ConnectionClosed as e:
-        #     print(f"Connection closed: {e.code} {e.reason}")
         #     self.websocket = None
         #     self.path = ''
         #     onClosed = self.config.get('onClosed', None)
         #     if callable(onClosed): await onClosed()
         except Exception as e:
             onError = self.config.get('onError', None)
             if callable(onError): await onError(e)
```

### Comparing `ipyweb-1.0.2/ipyweb/services/timer.py` & `ipyweb-1.0.3/ipyweb/services/timer.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/thread.py` & `ipyweb-1.0.3/ipyweb/thread.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb/utils.py` & `ipyweb-1.0.3/ipyweb/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,18 +12,33 @@
             importlib.import_module(name)
             return True
         except ImportError:
             return False
 
     @classmethod
     def pathExists(self, path='') -> bool:
-        if os.path.exists(path):
-            return True if os.path.isdir(path) else False
-        else:
+        try:
+            if os.path.exists(path):
+                return True if os.path.isdir(path) else False
+            else:
+                return False
+        except Exception:
             return False
+        return False
+
+    @classmethod
+    def fileExists(self, filePath='') -> bool:
+        try:
+            if os.path.exists(filePath):
+                return True if os.path.isfile(file_path) else False
+            else:
+                return False
+        except Exception:
+            return False
+        return False
 
     @classmethod
     def tuple(self, data=(), index=0, default=None):
         try:
             return data[index]
         except IndexError:
             return default
@@ -113,15 +128,17 @@
         import importlib
         try:
             module = importlib.import_module(modulePath)
         except ImportError as e:
             try:
                 modulePath = modulePath.replace('.', '/') + '.py'
                 modulePath = os.path.normpath(f'{rootPrefix}/{modulePath}')
-                spec = importlib.util.spec_from_file_location(name, modulePath)
-                module = importlib.util.module_from_spec(spec)
-                spec.loader.exec_module(module)
+                if self.fileExists(modulePath):
+                    spec = importlib.util.spec_from_file_location(name, modulePath)
+                    if spec:
+                        module = importlib.util.module_from_spec(spec)
+                        spec.loader.exec_module(module)
             except Exception as e:
-                pass
+                print(f'An exception occurred while importing a module from a file [{modulePath}]:{e}')
         except Exception as e:
-            pass
+            print(f'An exception occurred while importing a module [{modulePath}]:{e}')
         return module
```

### Comparing `ipyweb-1.0.2/ipyweb/windowEvents/main.py` & `ipyweb-1.0.3/ipyweb/windowEvents/main.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/ipyweb.egg-info/PKG-INFO` & `ipyweb-1.0.3/ipyweb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyweb
-Version: 1.0.2
+Version: 1.0.3
 Summary: A business framework for launching multiple services
 Author-email: sqwindows <sqwindows@qq.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2014-2017, Roman Sirokov
         All rights reserved.
```

### Comparing `ipyweb-1.0.2/ipyweb.egg-info/SOURCES.txt` & `ipyweb-1.0.3/ipyweb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.2/pyproject.toml` & `ipyweb-1.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ipyweb"
-version = "1.0.2"
+version = "1.0.3"
 description = "A business framework for launching multiple services"
 authors = [
     { name = "sqwindows", email = "sqwindows@qq.com" },
 ]
 
 keywords = ["gui", "webkit", "html", "web"]
 requires-python = ">=3.8"
```

