# Comparing `tmp/ipyweb-1.0.3.tar.gz` & `tmp/ipyweb-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyweb-1.0.3.tar", last modified: Fri May 31 12:46:40 2024, max compression
+gzip compressed data, was "ipyweb-1.0.4.tar", last modified: Fri May 31 13:34:28 2024, max compression
```

## Comparing `ipyweb-1.0.3.tar` & `ipyweb-1.0.4.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.522474 ipyweb-1.0.3/
--rw-rw-rw-   0        0        0     1547 2024-05-16 17:34:29.000000 ipyweb-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     2193 2024-05-31 12:46:40.520954 ipyweb-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       43 2024-05-31 07:23:39.000000 ipyweb-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.402821 ipyweb-1.0.3/ipyweb/
--rw-rw-rw-   0        0        0        0 2024-05-31 04:11:12.000000 ipyweb-1.0.3/ipyweb/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.421437 ipyweb-1.0.3/ipyweb/addons/
--rw-rw-rw-   0        0        0     3561 2024-05-31 01:15:14.000000 ipyweb-1.0.3/ipyweb/addons/loadingGui.py
--rw-rw-rw-   0        0        0     3713 2024-05-30 23:10:57.000000 ipyweb-1.0.3/ipyweb/app.py
--rw-rw-rw-   0        0        0     4937 2024-05-31 12:45:56.000000 ipyweb-1.0.3/ipyweb/appRunner.py
-drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.423461 ipyweb-1.0.3/ipyweb/builds/
--rw-rw-rw-   0        0        0     7351 2024-05-31 01:13:37.000000 ipyweb-1.0.3/ipyweb/builds/builder.py
--rw-rw-rw-   0        0        0     4779 2024-05-31 01:50:03.000000 ipyweb-1.0.3/ipyweb/cache.py
--rw-rw-rw-   0        0        0      316 2024-05-31 07:19:21.000000 ipyweb-1.0.3/ipyweb/cli.py
--rw-rw-rw-   0        0        0     3568 2024-05-31 00:44:58.000000 ipyweb-1.0.3/ipyweb/command.py
-drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.428465 ipyweb-1.0.3/ipyweb/commands/
--rw-rw-rw-   0        0        0      804 2024-05-31 07:10:00.000000 ipyweb-1.0.3/ipyweb/commands/ipywebBuilder.py
--rw-rw-rw-   0        0        0     2160 2024-05-31 07:07:45.000000 ipyweb-1.0.3/ipyweb/commands/ipywebRunner.py
--rw-rw-rw-   0        0        0     9804 2024-05-31 11:36:50.000000 ipyweb-1.0.3/ipyweb/config.py
-drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.446566 ipyweb-1.0.3/ipyweb/configs/
--rw-rw-rw-   0        0        0     1010 2024-05-28 16:39:36.000000 ipyweb-1.0.3/ipyweb/configs/app.py
--rw-rw-rw-   0        0        0      363 2024-05-30 15:55:41.000000 ipyweb-1.0.3/ipyweb/configs/build.py
--rw-rw-rw-   0        0        0      225 2024-05-12 09:40:00.000000 ipyweb-1.0.3/ipyweb/configs/cache.py
--rw-rw-rw-   0        0        0     1050 2024-05-12 09:51:21.000000 ipyweb-1.0.3/ipyweb/configs/database.py
--rw-rw-rw-   0        0        0       62 2024-05-10 17:35:35.000000 ipyweb-1.0.3/ipyweb/configs/jsonFile.py
--rw-rw-rw-   0        0        0     1130 2024-05-29 18:24:21.000000 ipyweb-1.0.3/ipyweb/configs/logger.py
--rw-rw-rw-   0        0        0     2881 2024-05-30 15:55:40.000000 ipyweb-1.0.3/ipyweb/configs/windows.py
-drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.466382 ipyweb-1.0.3/ipyweb/contracts/
--rw-rw-rw-   0        0        0      104 2024-05-30 15:55:41.000000 ipyweb-1.0.3/ipyweb/contracts/ipywebAddon.py
--rw-rw-rw-   0        0        0      641 2024-05-30 15:55:41.000000 ipyweb-1.0.3/ipyweb/contracts/ipywebController.py
--rw-rw-rw-   0        0        0      422 2024-05-30 15:55:41.000000 ipyweb-1.0.3/ipyweb/contracts/ipywebException.py
--rw-rw-rw-   0        0        0     1037 2024-05-31 12:37:53.000000 ipyweb-1.0.3/ipyweb/contracts/ipywebHttpController.py
--rw-rw-rw-   0        0        0      154 2024-05-30 15:55:41.000000 ipyweb-1.0.3/ipyweb/contracts/ipywebModel.py
--rw-rw-rw-   0        0        0      410 2024-05-30 15:55:41.000000 ipyweb-1.0.3/ipyweb/contracts/ipywebPreload.py
--rw-rw-rw-   0        0        0       93 2024-05-30 19:22:02.000000 ipyweb-1.0.3/ipyweb/contracts/ipywebQueue.py
--rw-rw-rw-   0        0        0      154 2024-05-31 01:10:19.000000 ipyweb-1.0.3/ipyweb/contracts/ipywebRunner.py
--rw-rw-rw-   0        0        0     6971 2024-05-31 06:56:48.000000 ipyweb-1.0.3/ipyweb/controller.py
-drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.468382 ipyweb-1.0.3/ipyweb/controllers/
--rw-rw-rw-   0        0        0     7422 2024-05-31 12:37:17.000000 ipyweb-1.0.3/ipyweb/controllers/ipyweb.py
--rw-rw-rw-   0        0        0     4646 2024-05-31 01:49:46.000000 ipyweb-1.0.3/ipyweb/db.py
--rw-rw-rw-   0        0        0    10557 2024-05-31 00:27:17.000000 ipyweb-1.0.3/ipyweb/event.py
-drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.335296 ipyweb-1.0.3/ipyweb/events/
-drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.471386 ipyweb-1.0.3/ipyweb/events/listener/
--rw-rw-rw-   0        0        0      453 2024-05-30 19:21:37.000000 ipyweb-1.0.3/ipyweb/events/listener/windows.py
-drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.474945 ipyweb-1.0.3/ipyweb/events/register/
--rw-rw-rw-   0        0        0      686 2024-05-30 19:21:42.000000 ipyweb-1.0.3/ipyweb/events/register/windows.py
--rw-rw-rw-   0        0        0     1699 2024-05-30 15:56:03.000000 ipyweb-1.0.3/ipyweb/gui.py
-drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.487467 ipyweb-1.0.3/ipyweb/guis/
--rw-rw-rw-   0        0        0      987 2024-05-30 15:55:41.000000 ipyweb-1.0.3/ipyweb/guis/BottleServer.py
--rw-rw-rw-   0        0        0     3822 2024-05-30 15:55:41.000000 ipyweb-1.0.3/ipyweb/guis/FlaskServer.py
--rw-rw-rw-   0        0        0     3922 2024-05-30 15:56:03.000000 ipyweb-1.0.3/ipyweb/guis/IpywebServer.py
--rw-rw-rw-   0        0        0     1491 2024-05-31 01:07:59.000000 ipyweb-1.0.3/ipyweb/guis/LocalServer.py
--rw-rw-rw-   0        0        0     1446 2024-05-30 19:21:31.000000 ipyweb-1.0.3/ipyweb/guis/RemoteServer.py
--rw-rw-rw-   0        0        0     6444 2024-05-31 12:39:13.000000 ipyweb-1.0.3/ipyweb/ipyweb.py
--rw-rw-rw-   0        0        0     2546 2024-05-31 00:12:02.000000 ipyweb-1.0.3/ipyweb/jsonFile.py
--rw-rw-rw-   0        0        0     2379 2024-05-31 00:08:13.000000 ipyweb-1.0.3/ipyweb/logger.py
--rw-rw-rw-   0        0        0     7935 2024-05-31 00:45:17.000000 ipyweb-1.0.3/ipyweb/module.py
--rw-rw-rw-   0        0        0      247 2024-05-05 11:24:12.000000 ipyweb-1.0.3/ipyweb/multiton.py
--rw-rw-rw-   0        0        0     8722 2024-05-31 00:04:40.000000 ipyweb-1.0.3/ipyweb/preload.py
-drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.339329 ipyweb-1.0.3/ipyweb/preloads/
-drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.495028 ipyweb-1.0.3/ipyweb/preloads/block/
--rw-rw-rw-   0        0        0     1555 2024-05-31 01:00:22.000000 ipyweb-1.0.3/ipyweb/preloads/block/controllerPreload.py
--rw-rw-rw-   0        0        0      404 2024-05-30 15:56:03.000000 ipyweb-1.0.3/ipyweb/preloads/block/guiPreload.py
--rw-rw-rw-   0        0        0      420 2024-05-30 15:56:03.000000 ipyweb-1.0.3/ipyweb/preloads/block/processPreload.py
-drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.498024 ipyweb-1.0.3/ipyweb/preloads/process/
--rw-rw-rw-   0        0        0      487 2024-05-30 19:20:37.000000 ipyweb-1.0.3/ipyweb/preloads/process/examplePreload.py
-drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.504555 ipyweb-1.0.3/ipyweb/preloads/thread/
--rw-rw-rw-   0        0        0     2981 2024-05-31 01:03:40.000000 ipyweb-1.0.3/ipyweb/preloads/thread/queuePreload.py
--rw-rw-rw-   0        0        0     2953 2024-05-31 01:04:52.000000 ipyweb-1.0.3/ipyweb/preloads/thread/socketPreload.py
--rw-rw-rw-   0        0        0     2216 2024-05-31 01:06:07.000000 ipyweb-1.0.3/ipyweb/preloads/thread/timerPreload.py
--rw-rw-rw-   0        0        0    10336 2024-05-31 00:02:01.000000 ipyweb-1.0.3/ipyweb/process.py
-drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.506565 ipyweb-1.0.3/ipyweb/pywebview/
--rw-rw-rw-   0        0        0     9338 2024-05-31 02:33:23.000000 ipyweb-1.0.3/ipyweb/pywebview/windows.py
--rw-rw-rw-   0        0        0     4587 2024-05-31 11:42:57.000000 ipyweb-1.0.3/ipyweb/service.py
-drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.513972 ipyweb-1.0.3/ipyweb/services/
--rw-rw-rw-   0        0        0     8228 2024-05-31 01:18:35.000000 ipyweb-1.0.3/ipyweb/services/queue.py
--rw-rw-rw-   0        0        0     7627 2024-05-31 12:38:13.000000 ipyweb-1.0.3/ipyweb/services/socketServer.py
--rw-rw-rw-   0        0        0     2671 2024-05-31 00:49:24.000000 ipyweb-1.0.3/ipyweb/services/timer.py
--rw-rw-rw-   0        0        0      470 2024-05-05 11:23:41.000000 ipyweb-1.0.3/ipyweb/singleton.py
--rw-rw-rw-   0        0        0     5026 2024-05-30 23:58:28.000000 ipyweb-1.0.3/ipyweb/thread.py
--rw-rw-rw-   0        0        0     4430 2024-05-31 12:44:27.000000 ipyweb-1.0.3/ipyweb/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.515969 ipyweb-1.0.3/ipyweb/windowEvents/
--rw-rw-rw-   0        0        0     2163 2024-05-30 15:55:41.000000 ipyweb-1.0.3/ipyweb/windowEvents/main.py
-drwxrwxrwx   0        0        0        0 2024-05-31 12:46:40.518955 ipyweb-1.0.3/ipyweb.egg-info/
--rw-rw-rw-   0        0        0     2193 2024-05-31 12:46:40.000000 ipyweb-1.0.3/ipyweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1814 2024-05-31 12:46:40.000000 ipyweb-1.0.3/ipyweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 12:46:40.000000 ipyweb-1.0.3/ipyweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-05-31 12:46:40.000000 ipyweb-1.0.3/ipyweb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       25 2024-05-31 12:46:40.000000 ipyweb-1.0.3/ipyweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-31 12:46:40.000000 ipyweb-1.0.3/ipyweb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1185 2024-05-31 12:35:10.000000 ipyweb-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-31 12:46:40.523467 ipyweb-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-31 13:34:28.961080 ipyweb-1.0.4/
+-rw-rw-rw-   0        0        0     1547 2024-05-16 17:34:29.000000 ipyweb-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2193 2024-05-31 13:34:28.957076 ipyweb-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2024-05-31 07:23:39.000000 ipyweb-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 13:34:28.798167 ipyweb-1.0.4/ipyweb/
+-rw-rw-rw-   0        0        0        0 2024-05-31 04:11:12.000000 ipyweb-1.0.4/ipyweb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:34:28.816225 ipyweb-1.0.4/ipyweb/addons/
+-rw-rw-rw-   0        0        0     3561 2024-05-31 01:15:14.000000 ipyweb-1.0.4/ipyweb/addons/loadingGui.py
+-rw-rw-rw-   0        0        0     3713 2024-05-30 23:10:57.000000 ipyweb-1.0.4/ipyweb/app.py
+-rw-rw-rw-   0        0        0     4937 2024-05-31 12:45:56.000000 ipyweb-1.0.4/ipyweb/appRunner.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:34:28.819225 ipyweb-1.0.4/ipyweb/builds/
+-rw-rw-rw-   0        0        0     7351 2024-05-31 01:13:37.000000 ipyweb-1.0.4/ipyweb/builds/builder.py
+-rw-rw-rw-   0        0        0     4779 2024-05-31 01:50:03.000000 ipyweb-1.0.4/ipyweb/cache.py
+-rw-rw-rw-   0        0        0      316 2024-05-31 07:19:21.000000 ipyweb-1.0.4/ipyweb/cli.py
+-rw-rw-rw-   0        0        0     3568 2024-05-31 00:44:58.000000 ipyweb-1.0.4/ipyweb/command.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:34:28.828489 ipyweb-1.0.4/ipyweb/commands/
+-rw-rw-rw-   0        0        0      804 2024-05-31 07:10:00.000000 ipyweb-1.0.4/ipyweb/commands/ipywebBuilder.py
+-rw-rw-rw-   0        0        0     2160 2024-05-31 07:07:45.000000 ipyweb-1.0.4/ipyweb/commands/ipywebRunner.py
+-rw-rw-rw-   0        0        0     9804 2024-05-31 11:36:50.000000 ipyweb-1.0.4/ipyweb/config.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:34:28.850495 ipyweb-1.0.4/ipyweb/configs/
+-rw-rw-rw-   0        0        0     1010 2024-05-28 16:39:36.000000 ipyweb-1.0.4/ipyweb/configs/app.py
+-rw-rw-rw-   0        0        0      363 2024-05-30 15:55:41.000000 ipyweb-1.0.4/ipyweb/configs/build.py
+-rw-rw-rw-   0        0        0      225 2024-05-12 09:40:00.000000 ipyweb-1.0.4/ipyweb/configs/cache.py
+-rw-rw-rw-   0        0        0     1050 2024-05-12 09:51:21.000000 ipyweb-1.0.4/ipyweb/configs/database.py
+-rw-rw-rw-   0        0        0       62 2024-05-10 17:35:35.000000 ipyweb-1.0.4/ipyweb/configs/jsonFile.py
+-rw-rw-rw-   0        0        0     1130 2024-05-29 18:24:21.000000 ipyweb-1.0.4/ipyweb/configs/logger.py
+-rw-rw-rw-   0        0        0     2881 2024-05-30 15:55:40.000000 ipyweb-1.0.4/ipyweb/configs/windows.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:34:28.880090 ipyweb-1.0.4/ipyweb/contracts/
+-rw-rw-rw-   0        0        0      104 2024-05-30 15:55:41.000000 ipyweb-1.0.4/ipyweb/contracts/ipywebAddon.py
+-rw-rw-rw-   0        0        0      641 2024-05-30 15:55:41.000000 ipyweb-1.0.4/ipyweb/contracts/ipywebController.py
+-rw-rw-rw-   0        0        0      422 2024-05-30 15:55:41.000000 ipyweb-1.0.4/ipyweb/contracts/ipywebException.py
+-rw-rw-rw-   0        0        0     1037 2024-05-31 12:37:53.000000 ipyweb-1.0.4/ipyweb/contracts/ipywebHttpController.py
+-rw-rw-rw-   0        0        0      154 2024-05-30 15:55:41.000000 ipyweb-1.0.4/ipyweb/contracts/ipywebModel.py
+-rw-rw-rw-   0        0        0      410 2024-05-30 15:55:41.000000 ipyweb-1.0.4/ipyweb/contracts/ipywebPreload.py
+-rw-rw-rw-   0        0        0       93 2024-05-30 19:22:02.000000 ipyweb-1.0.4/ipyweb/contracts/ipywebQueue.py
+-rw-rw-rw-   0        0        0      154 2024-05-31 01:10:19.000000 ipyweb-1.0.4/ipyweb/contracts/ipywebRunner.py
+-rw-rw-rw-   0        0        0     6971 2024-05-31 06:56:48.000000 ipyweb-1.0.4/ipyweb/controller.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:34:28.884213 ipyweb-1.0.4/ipyweb/controllers/
+-rw-rw-rw-   0        0        0     7422 2024-05-31 12:37:17.000000 ipyweb-1.0.4/ipyweb/controllers/ipyweb.py
+-rw-rw-rw-   0        0        0     4646 2024-05-31 01:49:46.000000 ipyweb-1.0.4/ipyweb/db.py
+-rw-rw-rw-   0        0        0    10557 2024-05-31 00:27:17.000000 ipyweb-1.0.4/ipyweb/event.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:34:28.717092 ipyweb-1.0.4/ipyweb/events/
+drwxrwxrwx   0        0        0        0 2024-05-31 13:34:28.887240 ipyweb-1.0.4/ipyweb/events/listener/
+-rw-rw-rw-   0        0        0      453 2024-05-30 19:21:37.000000 ipyweb-1.0.4/ipyweb/events/listener/windows.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:34:28.891209 ipyweb-1.0.4/ipyweb/events/register/
+-rw-rw-rw-   0        0        0      686 2024-05-30 19:21:42.000000 ipyweb-1.0.4/ipyweb/events/register/windows.py
+-rw-rw-rw-   0        0        0     1699 2024-05-30 15:56:03.000000 ipyweb-1.0.4/ipyweb/gui.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:34:28.908258 ipyweb-1.0.4/ipyweb/guis/
+-rw-rw-rw-   0        0        0      987 2024-05-30 15:55:41.000000 ipyweb-1.0.4/ipyweb/guis/BottleServer.py
+-rw-rw-rw-   0        0        0     3822 2024-05-30 15:55:41.000000 ipyweb-1.0.4/ipyweb/guis/FlaskServer.py
+-rw-rw-rw-   0        0        0     3922 2024-05-30 15:56:03.000000 ipyweb-1.0.4/ipyweb/guis/IpywebServer.py
+-rw-rw-rw-   0        0        0     1491 2024-05-31 01:07:59.000000 ipyweb-1.0.4/ipyweb/guis/LocalServer.py
+-rw-rw-rw-   0        0        0     1446 2024-05-30 19:21:31.000000 ipyweb-1.0.4/ipyweb/guis/RemoteServer.py
+-rw-rw-rw-   0        0        0     6444 2024-05-31 12:39:13.000000 ipyweb-1.0.4/ipyweb/ipyweb.py
+-rw-rw-rw-   0        0        0     2546 2024-05-31 00:12:02.000000 ipyweb-1.0.4/ipyweb/jsonFile.py
+-rw-rw-rw-   0        0        0     2379 2024-05-31 00:08:13.000000 ipyweb-1.0.4/ipyweb/logger.py
+-rw-rw-rw-   0        0        0     7935 2024-05-31 00:45:17.000000 ipyweb-1.0.4/ipyweb/module.py
+-rw-rw-rw-   0        0        0      247 2024-05-05 11:24:12.000000 ipyweb-1.0.4/ipyweb/multiton.py
+-rw-rw-rw-   0        0        0     8722 2024-05-31 00:04:40.000000 ipyweb-1.0.4/ipyweb/preload.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:34:28.723166 ipyweb-1.0.4/ipyweb/preloads/
+drwxrwxrwx   0        0        0        0 2024-05-31 13:34:28.916780 ipyweb-1.0.4/ipyweb/preloads/block/
+-rw-rw-rw-   0        0        0     1555 2024-05-31 01:00:22.000000 ipyweb-1.0.4/ipyweb/preloads/block/controllerPreload.py
+-rw-rw-rw-   0        0        0      404 2024-05-30 15:56:03.000000 ipyweb-1.0.4/ipyweb/preloads/block/guiPreload.py
+-rw-rw-rw-   0        0        0      420 2024-05-30 15:56:03.000000 ipyweb-1.0.4/ipyweb/preloads/block/processPreload.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:34:28.919777 ipyweb-1.0.4/ipyweb/preloads/process/
+-rw-rw-rw-   0        0        0      487 2024-05-30 19:20:37.000000 ipyweb-1.0.4/ipyweb/preloads/process/examplePreload.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:34:28.930298 ipyweb-1.0.4/ipyweb/preloads/thread/
+-rw-rw-rw-   0        0        0     2981 2024-05-31 01:03:40.000000 ipyweb-1.0.4/ipyweb/preloads/thread/queuePreload.py
+-rw-rw-rw-   0        0        0     2953 2024-05-31 01:04:52.000000 ipyweb-1.0.4/ipyweb/preloads/thread/socketPreload.py
+-rw-rw-rw-   0        0        0     2216 2024-05-31 01:06:07.000000 ipyweb-1.0.4/ipyweb/preloads/thread/timerPreload.py
+-rw-rw-rw-   0        0        0    10336 2024-05-31 00:02:01.000000 ipyweb-1.0.4/ipyweb/process.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:34:28.933867 ipyweb-1.0.4/ipyweb/pywebview/
+-rw-rw-rw-   0        0        0     9338 2024-05-31 02:33:23.000000 ipyweb-1.0.4/ipyweb/pywebview/windows.py
+-rw-rw-rw-   0        0        0     4587 2024-05-31 11:42:57.000000 ipyweb-1.0.4/ipyweb/service.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:34:28.945466 ipyweb-1.0.4/ipyweb/services/
+-rw-rw-rw-   0        0        0     8227 2024-05-31 13:15:40.000000 ipyweb-1.0.4/ipyweb/services/queue.py
+-rw-rw-rw-   0        0        0     7626 2024-05-31 13:15:03.000000 ipyweb-1.0.4/ipyweb/services/socketServer.py
+-rw-rw-rw-   0        0        0     2671 2024-05-31 00:49:24.000000 ipyweb-1.0.4/ipyweb/services/timer.py
+-rw-rw-rw-   0        0        0      470 2024-05-05 11:23:41.000000 ipyweb-1.0.4/ipyweb/singleton.py
+-rw-rw-rw-   0        0        0     5026 2024-05-30 23:58:28.000000 ipyweb-1.0.4/ipyweb/thread.py
+-rw-rw-rw-   0        0        0     4429 2024-05-31 13:32:15.000000 ipyweb-1.0.4/ipyweb/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:34:28.948505 ipyweb-1.0.4/ipyweb/windowEvents/
+-rw-rw-rw-   0        0        0     2163 2024-05-30 15:55:41.000000 ipyweb-1.0.4/ipyweb/windowEvents/main.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:34:28.954018 ipyweb-1.0.4/ipyweb.egg-info/
+-rw-rw-rw-   0        0        0     2193 2024-05-31 13:34:28.000000 ipyweb-1.0.4/ipyweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1814 2024-05-31 13:34:28.000000 ipyweb-1.0.4/ipyweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 13:34:28.000000 ipyweb-1.0.4/ipyweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-31 13:34:28.000000 ipyweb-1.0.4/ipyweb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       25 2024-05-31 13:34:28.000000 ipyweb-1.0.4/ipyweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-31 13:34:28.000000 ipyweb-1.0.4/ipyweb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1185 2024-05-31 13:34:05.000000 ipyweb-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-31 13:34:28.962064 ipyweb-1.0.4/setup.cfg
```

### Comparing `ipyweb-1.0.3/LICENSE` & `ipyweb-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/PKG-INFO` & `ipyweb-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyweb
-Version: 1.0.3
+Version: 1.0.4
 Summary: A business framework for launching multiple services
 Author-email: sqwindows <sqwindows@qq.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2014-2017, Roman Sirokov
         All rights reserved.
```

### Comparing `ipyweb-1.0.3/ipyweb/addons/loadingGui.py` & `ipyweb-1.0.4/ipyweb/addons/loadingGui.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/app.py` & `ipyweb-1.0.4/ipyweb/app.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/appRunner.py` & `ipyweb-1.0.4/ipyweb/appRunner.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/builds/builder.py` & `ipyweb-1.0.4/ipyweb/builds/builder.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/cache.py` & `ipyweb-1.0.4/ipyweb/cache.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/command.py` & `ipyweb-1.0.4/ipyweb/command.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/commands/ipywebBuilder.py` & `ipyweb-1.0.4/ipyweb/commands/ipywebBuilder.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/commands/ipywebRunner.py` & `ipyweb-1.0.4/ipyweb/commands/ipywebRunner.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/config.py` & `ipyweb-1.0.4/ipyweb/config.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/configs/app.py` & `ipyweb-1.0.4/ipyweb/configs/app.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/configs/database.py` & `ipyweb-1.0.4/ipyweb/configs/database.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/configs/logger.py` & `ipyweb-1.0.4/ipyweb/configs/logger.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/configs/windows.py` & `ipyweb-1.0.4/ipyweb/configs/windows.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/contracts/ipywebController.py` & `ipyweb-1.0.4/ipyweb/contracts/ipywebController.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/contracts/ipywebHttpController.py` & `ipyweb-1.0.4/ipyweb/contracts/ipywebHttpController.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/controller.py` & `ipyweb-1.0.4/ipyweb/controller.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/controllers/ipyweb.py` & `ipyweb-1.0.4/ipyweb/controllers/ipyweb.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/db.py` & `ipyweb-1.0.4/ipyweb/db.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/event.py` & `ipyweb-1.0.4/ipyweb/event.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/events/register/windows.py` & `ipyweb-1.0.4/ipyweb/events/register/windows.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/gui.py` & `ipyweb-1.0.4/ipyweb/gui.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/guis/BottleServer.py` & `ipyweb-1.0.4/ipyweb/guis/BottleServer.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/guis/FlaskServer.py` & `ipyweb-1.0.4/ipyweb/guis/FlaskServer.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/guis/IpywebServer.py` & `ipyweb-1.0.4/ipyweb/guis/IpywebServer.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/guis/LocalServer.py` & `ipyweb-1.0.4/ipyweb/guis/LocalServer.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/guis/RemoteServer.py` & `ipyweb-1.0.4/ipyweb/guis/RemoteServer.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/ipyweb.py` & `ipyweb-1.0.4/ipyweb/ipyweb.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/jsonFile.py` & `ipyweb-1.0.4/ipyweb/jsonFile.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/logger.py` & `ipyweb-1.0.4/ipyweb/logger.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/module.py` & `ipyweb-1.0.4/ipyweb/module.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/preload.py` & `ipyweb-1.0.4/ipyweb/preload.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/preloads/block/controllerPreload.py` & `ipyweb-1.0.4/ipyweb/preloads/block/controllerPreload.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/preloads/thread/queuePreload.py` & `ipyweb-1.0.4/ipyweb/preloads/thread/queuePreload.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/preloads/thread/socketPreload.py` & `ipyweb-1.0.4/ipyweb/preloads/thread/socketPreload.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/preloads/thread/timerPreload.py` & `ipyweb-1.0.4/ipyweb/preloads/thread/timerPreload.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/process.py` & `ipyweb-1.0.4/ipyweb/process.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/pywebview/windows.py` & `ipyweb-1.0.4/ipyweb/pywebview/windows.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/service.py` & `ipyweb-1.0.4/ipyweb/service.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/services/queue.py` & `ipyweb-1.0.4/ipyweb/services/queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,20 +146,20 @@
             if useProcess:
                 (process.runPool if usePool else process.run)(**params)
             else:
                 (thread.runPool if usePool else thread.run)(**params)
 
             onStart = self._config.get('onStart', None)
             if callable(onStart): onStart(self._userQueue)
-            logger.console.debug(f"Queue [{self._name}] has been started")
+            logger.console.info(f"Queue [{self._name}] has been started")
         except Exception as e:
             msg = f"An exception occurred while starting  the queue: {e}"
             onError = self._config.get('onError', None)
             if callable(onError): onError(msg, e)
-            logger.console.debug(msg)
+            logger.console.error(msg)
 
         return self
 
     def _getQueue(self):
         if self.queue is None:
             self._setQueue()
         return self.queue
```

### Comparing `ipyweb-1.0.3/ipyweb/services/socketServer.py` & `ipyweb-1.0.4/ipyweb/services/socketServer.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             from webview import generate_ssl_cert
             ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
             keyfile, certfile = generate_ssl_cert()
             ssl_context.load_cert_chain(certfile=certfile, keyfile=keyfile)
             serveConfig['ssl'] = ssl_context
 
         async with websockets.serve(**serveConfig) as server:
-            logger().console.debug(
+            logger().console.info(
                 f'Socket [{self.name}][ws://{self.config.get("host")}:{self.config.get("port")}] use [{self._logUseTxt}] has been started [PID:{os.getpid()}]')
             onReady = self.config.get('onReady', None)
             if callable(onReady): await onReady(server)
             await server.wait_closed()
 
     async def _start(self):
```

### Comparing `ipyweb-1.0.3/ipyweb/services/timer.py` & `ipyweb-1.0.4/ipyweb/services/timer.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/thread.py` & `ipyweb-1.0.4/ipyweb/thread.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb/utils.py` & `ipyweb-1.0.4/ipyweb/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             return False
         return False
 
     @classmethod
     def fileExists(self, filePath='') -> bool:
         try:
             if os.path.exists(filePath):
-                return True if os.path.isfile(file_path) else False
+                return True if os.path.isfile(filePath) else False
             else:
                 return False
         except Exception:
             return False
         return False
 
     @classmethod
```

### Comparing `ipyweb-1.0.3/ipyweb/windowEvents/main.py` & `ipyweb-1.0.4/ipyweb/windowEvents/main.py`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/ipyweb.egg-info/PKG-INFO` & `ipyweb-1.0.4/ipyweb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyweb
-Version: 1.0.3
+Version: 1.0.4
 Summary: A business framework for launching multiple services
 Author-email: sqwindows <sqwindows@qq.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2014-2017, Roman Sirokov
         All rights reserved.
```

### Comparing `ipyweb-1.0.3/ipyweb.egg-info/SOURCES.txt` & `ipyweb-1.0.4/ipyweb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipyweb-1.0.3/pyproject.toml` & `ipyweb-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ipyweb"
-version = "1.0.3"
+version = "1.0.4"
 description = "A business framework for launching multiple services"
 authors = [
     { name = "sqwindows", email = "sqwindows@qq.com" },
 ]
 
 keywords = ["gui", "webkit", "html", "web"]
 requires-python = ">=3.8"
```

