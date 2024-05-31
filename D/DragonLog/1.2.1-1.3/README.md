# Comparing `tmp/dragonlog-1.2.1.tar.gz` & `tmp/dragonlog-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dragonlog-1.2.1.tar", last modified: Fri May 24 05:53:07 2024, max compression
+gzip compressed data, was "dragonlog-1.3.tar", last modified: Fri May 31 05:28:27 2024, max compression
```

## Comparing `dragonlog-1.2.1.tar` & `dragonlog-1.3.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 05:53:07.445058 dragonlog-1.2.1/
-drwxrwxrwx   0        0        0        0 2024-05-24 05:53:07.440568 dragonlog-1.2.1/DragonLog.egg-info/
--rw-rw-rw-   0        0        0     7455 2024-05-24 05:53:07.000000 dragonlog-1.2.1/DragonLog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1716 2024-05-24 05:53:07.000000 dragonlog-1.2.1/DragonLog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 05:53:07.000000 dragonlog-1.2.1/DragonLog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-24 05:53:07.000000 dragonlog-1.2.1/DragonLog.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       79 2024-05-24 05:53:07.000000 dragonlog-1.2.1/DragonLog.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-24 05:53:07.000000 dragonlog-1.2.1/DragonLog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      158 2024-03-19 12:18:34.000000 dragonlog-1.2.1/LICENCE.txt
--rw-rw-rw-   0        0        0       93 2023-11-21 13:44:18.000000 dragonlog-1.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7455 2024-05-24 05:53:07.443063 dragonlog-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     6453 2024-05-04 08:39:54.000000 dragonlog-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 05:53:07.355237 dragonlog-1.2.1/dragonlog/
--rw-rw-rw-   0        0        0    10600 2024-04-30 18:45:39.000000 dragonlog-1.2.1/dragonlog/CallBook.py
--rw-rw-rw-   0        0        0    67866 2024-05-24 05:41:23.000000 dragonlog-1.2.1/dragonlog/DragonLog.py
--rw-rw-rw-   0        0        0     2062 2024-02-20 17:06:17.000000 dragonlog-1.2.1/dragonlog/DragonLog_AppSelect.py
--rw-rw-rw-   0        0        0     3041 2024-05-24 05:52:06.000000 dragonlog-1.2.1/dragonlog/DragonLog_AppSelect_ui.py
--rw-rw-rw-   0        0        0    26239 2024-05-24 05:52:05.000000 dragonlog-1.2.1/dragonlog/DragonLog_MainWindow_ui.py
--rw-rw-rw-   0        0        0    49415 2024-05-24 05:38:29.000000 dragonlog-1.2.1/dragonlog/DragonLog_QSOForm - Kopie.py
--rw-rw-rw-   0        0        0    49105 2024-05-24 05:44:30.000000 dragonlog-1.2.1/dragonlog/DragonLog_QSOForm.py
--rw-rw-rw-   0        0        0    42694 2024-05-24 05:52:06.000000 dragonlog-1.2.1/dragonlog/DragonLog_QSOForm_ui.py
--rw-rw-rw-   0        0        0    23629 2024-05-24 05:41:23.000000 dragonlog-1.2.1/dragonlog/DragonLog_Settings.py
--rw-rw-rw-   0        0        0    40061 2024-05-24 05:52:06.000000 dragonlog-1.2.1/dragonlog/DragonLog_Settings_ui.py
--rw-rw-rw-   0        0        0     1880 2024-05-24 05:44:57.000000 dragonlog-1.2.1/dragonlog/ListEdit.py
--rw-rw-rw-   0        0        0     2891 2024-05-24 05:52:07.000000 dragonlog-1.2.1/dragonlog/ListEdit_ui.py
--rw-rw-rw-   0        0        0     7403 2024-04-15 17:33:29.000000 dragonlog-1.2.1/dragonlog/LoTW.py
--rw-rw-rw-   0        0        0     2585 2024-04-12 05:48:01.000000 dragonlog-1.2.1/dragonlog/Logger.py
--rw-rw-rw-   0        0        0     1232 2024-05-24 05:41:23.000000 dragonlog-1.2.1/dragonlog/RegEx.py
--rw-rw-rw-   0        0        0        0 2023-11-21 18:25:24.000000 dragonlog-1.2.1/dragonlog/__init__.py
--rw-rw-rw-   0        0        0       45 2023-11-21 18:20:52.000000 dragonlog-1.2.1/dragonlog/__main__.py
--rw-rw-rw-   0        0        0       65 2024-05-24 05:52:05.000000 dragonlog-1.2.1/dragonlog/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 05:53:07.369708 dragonlog-1.2.1/dragonlog/data/
--rw-rw-rw-   0        0        0     6453 2024-05-04 08:39:54.000000 dragonlog-1.2.1/dragonlog/data/README.md
--rw-rw-rw-   0        0        0     1816 2023-10-08 14:01:05.000000 dragonlog-1.2.1/dragonlog/data/bands.json
--rw-rw-rw-   0        0        0     6834 2023-10-09 17:58:49.000000 dragonlog-1.2.1/dragonlog/data/cb_channels.json
--rw-rw-rw-   0        0        0     1115 2023-11-15 18:59:09.000000 dragonlog-1.2.1/dragonlog/data/color_map.json
-drwxrwxrwx   0        0        0        0 2024-05-24 05:53:07.375696 dragonlog-1.2.1/dragonlog/data/i18n/
--rw-rw-rw-   0        0        0    26024 2024-05-24 05:52:10.000000 dragonlog-1.2.1/dragonlog/data/i18n/DragonLog_de.qm
--rw-rw-rw-   0        0        0      108 2024-03-28 07:19:36.000000 dragonlog-1.2.1/dragonlog/data/i18n/ascii_replace_de.json
--rw-rw-rw-   0        0        0     4275 2023-10-11 18:47:43.000000 dragonlog-1.2.1/dragonlog/data/modes.json
--rw-rw-rw-   0        0        0     5348 2024-04-15 17:33:29.000000 dragonlog-1.2.1/dragonlog/eQSL.py
-drwxrwxrwx   0        0        0        0 2024-05-24 05:53:07.437075 dragonlog-1.2.1/dragonlog/icons/
--rw-rw-rw-   0        0        0    84255 2024-04-03 05:47:08.000000 dragonlog-1.2.1/dragonlog/icons/Screenshot.png
--rw-rw-rw-   0        0        0     2775 2006-10-09 18:29:54.000000 dragonlog-1.2.1/dragonlog/icons/db.png
--rw-rw-rw-   0        0        0      935 2006-10-09 18:46:20.000000 dragonlog-1.2.1/dragonlog/icons/edit.png
--rw-rw-rw-   0        0        0     1501 2006-10-09 18:51:24.000000 dragonlog-1.2.1/dragonlog/icons/edit_add.png
--rw-rw-rw-   0        0        0     4853 2023-10-06 05:04:50.000000 dragonlog-1.2.1/dragonlog/icons/edit_addmulti.png
--rw-rw-rw-   0        0        0     4222 2023-10-06 05:13:53.000000 dragonlog-1.2.1/dragonlog/icons/edit_addmulti.xcf
--rw-rw-rw-   0        0        0      901 2006-07-05 03:36:10.000000 dragonlog-1.2.1/dragonlog/icons/edit_remove.png
--rw-rw-rw-   0        0        0     2360 2007-05-26 19:17:06.000000 dragonlog-1.2.1/dragonlog/icons/exit.png
--rw-rw-rw-   0        0        0      697 2024-03-23 19:55:25.000000 dragonlog-1.2.1/dragonlog/icons/file_doc.png
--rw-rw-rw-   0        0        0     2321 2006-10-09 18:55:14.000000 dragonlog-1.2.1/dragonlog/icons/fileexport.png
--rw-rw-rw-   0        0        0     2076 2006-10-09 19:11:50.000000 dragonlog-1.2.1/dragonlog/icons/fileimport.png
--rw-rw-rw-   0        0        0     1900 2006-07-05 03:36:10.000000 dragonlog-1.2.1/dragonlog/icons/filter.png
--rw-rw-rw-   0        0        0     2166 2006-10-09 16:32:12.000000 dragonlog-1.2.1/dragonlog/icons/gear.png
--rw-rw-rw-   0        0        0     2461 2006-10-09 18:22:00.000000 dragonlog-1.2.1/dragonlog/icons/help.png
--rw-rw-rw-   0        0        0     4652 2023-10-04 17:16:16.000000 dragonlog-1.2.1/dragonlog/icons/icons8-dragon-96.png
--rw-rw-rw-   0        0        0    19186 2023-10-06 12:24:58.000000 dragonlog-1.2.1/dragonlog/icons/icons8-dragon-96.xcf
--rw-rw-rw-   0        0        0     2184 2006-10-09 19:49:00.000000 dragonlog-1.2.1/dragonlog/icons/info.png
--rw-rw-rw-   0        0        0    54470 2023-10-06 12:25:24.000000 dragonlog-1.2.1/dragonlog/icons/logo.ico
--rw-rw-rw-   0        0        0     2443 2006-10-09 19:00:44.000000 dragonlog-1.2.1/dragonlog/icons/no.png
--rw-rw-rw-   0        0        0     1518 2006-10-09 20:22:10.000000 dragonlog-1.2.1/dragonlog/icons/ok.png
--rw-rw-rw-   0        0        0     2225 2006-10-09 18:20:08.000000 dragonlog-1.2.1/dragonlog/icons/player_play.png
--rw-rw-rw-   0        0        0     2112 2024-03-05 19:18:39.000000 dragonlog-1.2.1/dragonlog/icons/player_stop.png
--rw-rw-rw-   0        0        0    21406 2024-03-25 10:49:08.000000 dragonlog-1.2.1/dragonlog/icons/upload_lotw.png
--rw-rw-rw-   0        0        0     7906 2024-03-25 10:48:26.000000 dragonlog-1.2.1/dragonlog/icons/upload_lotw.xcf
--rw-rw-rw-   0        0        0     1819 2006-10-17 07:09:30.000000 dragonlog-1.2.1/dragonlog/icons/watch.png
--rw-rw-rw-   0        0        0     1159 2024-03-23 19:55:25.000000 dragonlog-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-24 05:53:07.445558 dragonlog-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1498 2024-03-19 12:15:10.000000 dragonlog-1.2.1/setup_msi.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:28:27.808290 dragonlog-1.3/
+drwxrwxrwx   0        0        0        0 2024-05-31 05:28:27.803300 dragonlog-1.3/DragonLog.egg-info/
+-rw-rw-rw-   0        0        0     7527 2024-05-31 05:28:27.000000 dragonlog-1.3/DragonLog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1732 2024-05-31 05:28:27.000000 dragonlog-1.3/DragonLog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 05:28:27.000000 dragonlog-1.3/DragonLog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-31 05:28:27.000000 dragonlog-1.3/DragonLog.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       79 2024-05-31 05:28:27.000000 dragonlog-1.3/DragonLog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-31 05:28:27.000000 dragonlog-1.3/DragonLog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      158 2024-03-19 12:18:34.000000 dragonlog-1.3/LICENCE.txt
+-rw-rw-rw-   0        0        0       93 2023-11-21 13:44:18.000000 dragonlog-1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     7527 2024-05-31 05:28:27.805796 dragonlog-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6527 2024-05-30 18:36:09.000000 dragonlog-1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 05:28:27.696013 dragonlog-1.3/dragonlog/
+-rw-rw-rw-   0        0        0    10600 2024-04-30 18:45:39.000000 dragonlog-1.3/dragonlog/CallBook.py
+-rw-rw-rw-   0        0        0      801 2024-05-31 05:13:05.000000 dragonlog-1.3/dragonlog/ColorPalettes.py
+-rw-rw-rw-   0        0        0    71088 2024-05-31 05:12:10.000000 dragonlog-1.3/dragonlog/DragonLog.py
+-rw-rw-rw-   0        0        0     2062 2024-02-20 17:06:17.000000 dragonlog-1.3/dragonlog/DragonLog_AppSelect.py
+-rw-rw-rw-   0        0        0     3041 2024-05-31 05:27:07.000000 dragonlog-1.3/dragonlog/DragonLog_AppSelect_ui.py
+-rw-rw-rw-   0        0        0    26458 2024-05-31 05:27:05.000000 dragonlog-1.3/dragonlog/DragonLog_MainWindow_ui.py
+-rw-rw-rw-   0        0        0    48580 2024-05-29 18:15:09.000000 dragonlog-1.3/dragonlog/DragonLog_QSOForm.py
+-rw-rw-rw-   0        0        0    42751 2024-05-31 05:27:05.000000 dragonlog-1.3/dragonlog/DragonLog_QSOForm_ui.py
+-rw-rw-rw-   0        0        0    22809 2024-05-30 06:04:33.000000 dragonlog-1.3/dragonlog/DragonLog_Settings.py
+-rw-rw-rw-   0        0        0    36679 2024-05-31 05:27:06.000000 dragonlog-1.3/dragonlog/DragonLog_Settings_ui.py
+-rw-rw-rw-   0        0        0     1880 2024-05-24 05:44:57.000000 dragonlog-1.3/dragonlog/ListEdit.py
+-rw-rw-rw-   0        0        0     2891 2024-05-31 05:27:08.000000 dragonlog-1.3/dragonlog/ListEdit_ui.py
+-rw-rw-rw-   0        0        0     7403 2024-04-15 17:33:29.000000 dragonlog-1.3/dragonlog/LoTW.py
+-rw-rw-rw-   0        0        0     2585 2024-04-12 05:48:01.000000 dragonlog-1.3/dragonlog/Logger.py
+-rw-rw-rw-   0        0        0     1615 2024-05-24 18:01:32.000000 dragonlog-1.3/dragonlog/RegEx.py
+-rw-rw-rw-   0        0        0        0 2023-11-21 18:25:24.000000 dragonlog-1.3/dragonlog/__init__.py
+-rw-rw-rw-   0        0        0       45 2023-11-21 18:20:52.000000 dragonlog-1.3/dragonlog/__main__.py
+-rw-rw-rw-   0        0        0       63 2024-05-31 05:27:04.000000 dragonlog-1.3/dragonlog/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:28:27.717470 dragonlog-1.3/dragonlog/data/
+-rw-rw-rw-   0        0        0     6527 2024-05-30 18:36:09.000000 dragonlog-1.3/dragonlog/data/README.md
+-rw-rw-rw-   0        0        0      798 2024-05-30 18:43:55.000000 dragonlog-1.3/dragonlog/data/SHORTCUTS.md
+-rw-rw-rw-   0        0        0     1816 2023-10-08 14:01:05.000000 dragonlog-1.3/dragonlog/data/bands.json
+-rw-rw-rw-   0        0        0     6834 2023-10-09 17:58:49.000000 dragonlog-1.3/dragonlog/data/cb_channels.json
+-rw-rw-rw-   0        0        0     1115 2023-11-15 18:59:09.000000 dragonlog-1.3/dragonlog/data/color_map.json
+drwxrwxrwx   0        0        0        0 2024-05-31 05:28:27.722960 dragonlog-1.3/dragonlog/data/i18n/
+-rw-rw-rw-   0        0        0    26317 2024-05-31 05:27:11.000000 dragonlog-1.3/dragonlog/data/i18n/DragonLog_de.qm
+-rw-rw-rw-   0        0        0      108 2024-03-28 07:19:36.000000 dragonlog-1.3/dragonlog/data/i18n/ascii_replace_de.json
+-rw-rw-rw-   0        0        0     4275 2023-10-11 18:47:43.000000 dragonlog-1.3/dragonlog/data/modes.json
+-rw-rw-rw-   0        0        0     5348 2024-04-15 17:33:29.000000 dragonlog-1.3/dragonlog/eQSL.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:28:27.797811 dragonlog-1.3/dragonlog/icons/
+-rw-rw-rw-   0        0        0    84255 2024-04-03 05:47:08.000000 dragonlog-1.3/dragonlog/icons/Screenshot.png
+-rw-rw-rw-   0        0        0     2775 2006-10-09 18:29:54.000000 dragonlog-1.3/dragonlog/icons/db.png
+-rw-rw-rw-   0        0        0      935 2006-10-09 18:46:20.000000 dragonlog-1.3/dragonlog/icons/edit.png
+-rw-rw-rw-   0        0        0     1501 2006-10-09 18:51:24.000000 dragonlog-1.3/dragonlog/icons/edit_add.png
+-rw-rw-rw-   0        0        0     4853 2023-10-06 05:04:50.000000 dragonlog-1.3/dragonlog/icons/edit_addmulti.png
+-rw-rw-rw-   0        0        0     4222 2023-10-06 05:13:53.000000 dragonlog-1.3/dragonlog/icons/edit_addmulti.xcf
+-rw-rw-rw-   0        0        0      901 2006-07-05 03:36:10.000000 dragonlog-1.3/dragonlog/icons/edit_remove.png
+-rw-rw-rw-   0        0        0     2360 2007-05-26 19:17:06.000000 dragonlog-1.3/dragonlog/icons/exit.png
+-rw-rw-rw-   0        0        0      697 2024-03-23 19:55:25.000000 dragonlog-1.3/dragonlog/icons/file_doc.png
+-rw-rw-rw-   0        0        0     2321 2006-10-09 18:55:14.000000 dragonlog-1.3/dragonlog/icons/fileexport.png
+-rw-rw-rw-   0        0        0     2076 2006-10-09 19:11:50.000000 dragonlog-1.3/dragonlog/icons/fileimport.png
+-rw-rw-rw-   0        0        0     1900 2006-07-05 03:36:10.000000 dragonlog-1.3/dragonlog/icons/filter.png
+-rw-rw-rw-   0        0        0     2166 2006-10-09 16:32:12.000000 dragonlog-1.3/dragonlog/icons/gear.png
+-rw-rw-rw-   0        0        0     2461 2006-10-09 18:22:00.000000 dragonlog-1.3/dragonlog/icons/help.png
+-rw-rw-rw-   0        0        0     4652 2023-10-04 17:16:16.000000 dragonlog-1.3/dragonlog/icons/icons8-dragon-96.png
+-rw-rw-rw-   0        0        0    19186 2023-10-06 12:24:58.000000 dragonlog-1.3/dragonlog/icons/icons8-dragon-96.xcf
+-rw-rw-rw-   0        0        0     2184 2006-10-09 19:49:00.000000 dragonlog-1.3/dragonlog/icons/info.png
+-rw-rw-rw-   0        0        0    54470 2023-10-06 12:25:24.000000 dragonlog-1.3/dragonlog/icons/logo.ico
+-rw-rw-rw-   0        0        0     2443 2006-10-09 19:00:44.000000 dragonlog-1.3/dragonlog/icons/no.png
+-rw-rw-rw-   0        0        0     1518 2006-10-09 20:22:10.000000 dragonlog-1.3/dragonlog/icons/ok.png
+-rw-rw-rw-   0        0        0     2225 2006-10-09 18:20:08.000000 dragonlog-1.3/dragonlog/icons/player_play.png
+-rw-rw-rw-   0        0        0     2112 2024-03-05 19:18:39.000000 dragonlog-1.3/dragonlog/icons/player_stop.png
+-rw-rw-rw-   0        0        0    21406 2024-03-25 10:49:08.000000 dragonlog-1.3/dragonlog/icons/upload_lotw.png
+-rw-rw-rw-   0        0        0     7906 2024-03-25 10:48:26.000000 dragonlog-1.3/dragonlog/icons/upload_lotw.xcf
+-rw-rw-rw-   0        0        0     1819 2006-10-17 07:09:30.000000 dragonlog-1.3/dragonlog/icons/watch.png
+-rw-rw-rw-   0        0        0     1159 2024-03-23 19:55:25.000000 dragonlog-1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-31 05:28:27.809288 dragonlog-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1498 2024-03-19 12:15:10.000000 dragonlog-1.3/setup_msi.py
```

### Comparing `dragonlog-1.2.1/DragonLog.egg-info/PKG-INFO` & `dragonlog-1.3/DragonLog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DragonLog
-Version: 1.2.1
+Version: 1.3
 Summary: Log QSO for Ham radio
 Author-email: "Andreas Schawo, DF1ASC" <andreas@schawo.de>
 Project-URL: Homepage, https://github.com/gitandy/DragonLog
 Project-URL: Bug Tracker, https://github.com/gitandy/DragonLog/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Other Audience
 Classifier: Operating System :: OS Independent
@@ -131,14 +131,17 @@
 Starting file watching opens a file dialog where you have to point to the log in question.
 Check the manual of the other program to find the correct path.
 
 If you want to use the worked before feature of the other program consider to export your 
 QSOs beforehand.
 Dragonlog will only import QSOs which are not already included in the current database.
 
+[Keyboard shortcuts](SHORTCUTS.md)
+----------------------------------
+
 Export
 ------
 Following formats are supported for export
 * [ADIF 3](https://adif.org/) format (ADI/ADX)
 * Excel file
 * CSV format (UTF-8 encoding)
```

### Comparing `dragonlog-1.2.1/DragonLog.egg-info/SOURCES.txt` & `dragonlog-1.3/DragonLog.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,33 +6,34 @@
 DragonLog.egg-info/PKG-INFO
 DragonLog.egg-info/SOURCES.txt
 DragonLog.egg-info/dependency_links.txt
 DragonLog.egg-info/entry_points.txt
 DragonLog.egg-info/requires.txt
 DragonLog.egg-info/top_level.txt
 dragonlog/CallBook.py
+dragonlog/ColorPalettes.py
 dragonlog/DragonLog.py
 dragonlog/DragonLog_AppSelect.py
 dragonlog/DragonLog_AppSelect_ui.py
 dragonlog/DragonLog_MainWindow_ui.py
-dragonlog/DragonLog_QSOForm - Kopie.py
 dragonlog/DragonLog_QSOForm.py
 dragonlog/DragonLog_QSOForm_ui.py
 dragonlog/DragonLog_Settings.py
 dragonlog/DragonLog_Settings_ui.py
 dragonlog/ListEdit.py
 dragonlog/ListEdit_ui.py
 dragonlog/LoTW.py
 dragonlog/Logger.py
 dragonlog/RegEx.py
 dragonlog/__init__.py
 dragonlog/__main__.py
 dragonlog/__version__.py
 dragonlog/eQSL.py
 dragonlog/data/README.md
+dragonlog/data/SHORTCUTS.md
 dragonlog/data/bands.json
 dragonlog/data/cb_channels.json
 dragonlog/data/color_map.json
 dragonlog/data/modes.json
 dragonlog/data/i18n/DragonLog_de.qm
 dragonlog/data/i18n/ascii_replace_de.json
 dragonlog/icons/Screenshot.png
```

### Comparing `dragonlog-1.2.1/PKG-INFO` & `dragonlog-1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DragonLog
-Version: 1.2.1
+Version: 1.3
 Summary: Log QSO for Ham radio
 Author-email: "Andreas Schawo, DF1ASC" <andreas@schawo.de>
 Project-URL: Homepage, https://github.com/gitandy/DragonLog
 Project-URL: Bug Tracker, https://github.com/gitandy/DragonLog/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Other Audience
 Classifier: Operating System :: OS Independent
@@ -131,14 +131,17 @@
 Starting file watching opens a file dialog where you have to point to the log in question.
 Check the manual of the other program to find the correct path.
 
 If you want to use the worked before feature of the other program consider to export your 
 QSOs beforehand.
 Dragonlog will only import QSOs which are not already included in the current database.
 
+[Keyboard shortcuts](SHORTCUTS.md)
+----------------------------------
+
 Export
 ------
 Following formats are supported for export
 * [ADIF 3](https://adif.org/) format (ADI/ADX)
 * Excel file
 * CSV format (UTF-8 encoding)
```

### Comparing `dragonlog-1.2.1/README.md` & `dragonlog-1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,17 @@
 Starting file watching opens a file dialog where you have to point to the log in question.
 Check the manual of the other program to find the correct path.
 
 If you want to use the worked before feature of the other program consider to export your 
 QSOs beforehand.
 Dragonlog will only import QSOs which are not already included in the current database.
 
+[Keyboard shortcuts](SHORTCUTS.md)
+----------------------------------
+
 Export
 ------
 Following formats are supported for export
 * [ADIF 3](https://adif.org/) format (ADI/ADX)
 * Excel file
 * CSV format (UTF-8 encoding)
```

### Comparing `dragonlog-1.2.1/dragonlog/CallBook.py` & `dragonlog-1.3/dragonlog/CallBook.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/DragonLog.py` & `dragonlog-1.3/dragonlog/DragonLog.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from . import DragonLog_MainWindow_ui
 from .Logger import Logger
 from .RegEx import find_non_ascii, check_format, REGEX_DATE
 from .DragonLog_QSOForm import QSOForm
 from .DragonLog_Settings import Settings
 from .DragonLog_AppSelect import AppSelect
 from .LoTW import LoTW, LoTWADIFFieldException, LoTWRequestException, LoTWCommunicationException
+from . import ColorPalettes
 
 __prog_name__ = 'DragonLog'
 __prog_desc__ = 'Log QSO for Ham radio'
 __author_name__ = 'Andreas Schawo, DF1ASC'
 __author_email__ = 'andreas@schawo.de'
 __copyright__ = 'Copyright 2023-2024 by Andreas Schawo,licensed under CC BY-SA 4.0'
 
@@ -49,15 +50,15 @@
 
 
 class DatabaseWriteException(Exception):
     pass
 
 
 class BackgroundBrushDelegate(QtWidgets.QStyledItemDelegate):
-    """A delegate to change background color depending on a columns conntent and translation of different columns"""
+    """A delegate to change background color depending on a columns content and translation of different columns"""
 
     def __init__(self, color_map: dict, column: int):
         super(BackgroundBrushDelegate, self).__init__()
 
         self.color_map: dict = color_map
         self.column: int = column
 
@@ -371,14 +372,15 @@
         self.watchTimer = QtCore.QTimer(self)
         self.watchTimer.timeout.connect(self.watchFile)
         self.watchPos = 0
         self.watchFileName = ''
 
         self.lotw = LoTW(self.log)
 
+        self.settings_form.settingsStored.connect(self.qso_form.refreshQTHList)
         self.settings_form.settingsStored.connect(self.qso_form.refreshRadioList)
         self.settings_form.settingsStored.connect(self.qso_form.refreshAntennaList)
 
     @staticmethod
     def int2dock_area(value: int) -> QtCore.Qt.DockWidgetArea:
         dock_area = QtCore.Qt.DockWidgetArea.NoDockWidgetArea
         match value:
@@ -503,16 +505,14 @@
     def connectDB(self, db_file):
         db_file = os.path.abspath(db_file)
         try:
             if self.__db_con__.isOpen():
                 self.__db_con__.close()
 
             self.__db_con__.setDatabaseName(db_file)
-            if self.__db_con__.lastError().text():
-                raise DatabaseOpenException(self.__db_con__.lastError().text())
             self.__db_con__.open()
             self.__db_con__.exec(self.__db_create_stmnt__)
             self.__db_con__.exec(self.__db_create_idx_stmnt__)
 
             if self.__db_con__.lastError().text():
                 raise DatabaseOpenException(self.__db_con__.lastError().text())
 
@@ -588,23 +588,37 @@
                 return "DATE(date_time) > DATE('now', '-183 days')"
             elif recent_filter == self.tr('Last year'):
                 return "DATE(date_time) > DATE('now', '-365 days')"
             else:
                 return ""
 
     def setFilter(self):
-        self.QSOTableView.model().setFilter(self.getFilter())
+        if self.QSOTableView.model():
+            self.QSOTableView.model().setFilter(self.getFilter())
 
     def setTableFilter(self):
         filter_set = []
 
-        if self.fDateFromLineEdit.text() and check_format(REGEX_DATE, self.fDateFromLineEdit.text()):
-            filter_set.append(f"DATE(date_time) >= DATE('{self.fDateFromLineEdit.text()}')")
-        if self.fDateToLineEdit.text() and check_format(REGEX_DATE, self.fDateToLineEdit.text()):
-            filter_set.append(f"DATE(date_time) <= DATE('{self.fDateToLineEdit.text()}')")
+        if self.fDateFromLineEdit.text():
+            if check_format(REGEX_DATE, self.fDateFromLineEdit.text()):
+                filter_set.append(f"DATE(date_time) >= DATE('{self.fDateFromLineEdit.text()}')")
+                self.fDateFromLineEdit.setPalette(ColorPalettes.PaletteDefault)
+            else:
+                self.fDateFromLineEdit.setPalette(ColorPalettes.PaletteFaulty)
+        else:
+            self.fDateFromLineEdit.setPalette(ColorPalettes.PaletteDefault)
+
+        if self.fDateToLineEdit.text():
+            if check_format(REGEX_DATE, self.fDateToLineEdit.text()):
+                filter_set.append(f"DATE(date_time) <= DATE('{self.fDateToLineEdit.text()}')")
+                self.fDateToLineEdit.setPalette(ColorPalettes.PaletteDefault)
+            else:
+                self.fDateToLineEdit.setPalette(ColorPalettes.PaletteFaulty)
+        else:
+            self.fDateToLineEdit.setPalette(ColorPalettes.PaletteDefault)
 
         if self.fCallsignLineEdit.text():
             filter_set.append(f'call_sign LIKE "%{self.fCallsignLineEdit.text()}%"')
         if self.fBandComboBox.currentText():
             filter_set.append(f'band = "{self.fBandComboBox.currentText()}"')
         if self.fModeComboBox.currentText():
             filter_set.append(f'mode = "{self.fModeComboBox.currentText()}"')
@@ -614,15 +628,17 @@
         self.setFilter()
 
     def resetTableFilter(self):
         self.__table_filter__ = ''
         self.setFilter()
 
         self.fDateFromLineEdit.clear()
+        self.fDateFromLineEdit.setPalette(ColorPalettes.PaletteDefault)
         self.fDateToLineEdit.clear()
+        self.fDateToLineEdit.setPalette(ColorPalettes.PaletteDefault)
         self.fCallsignLineEdit.clear()
         self.fBandComboBox.setCurrentIndex(0)
         self.fModeComboBox.setCurrentIndex(0)
 
     def ctrlHamlib(self, start):
         self.settings_form.ctrlRigctld(start)
 
@@ -759,15 +775,15 @@
             while query.next():
                 row = []
                 for i in range(len(self.__sql_cols__)):
                     row.append(query.value(i))
                 writer.writerow(row)
 
     def exportExcel(self, file):
-        self.log.info('Exporting to Excel...')
+        self.log.info('Exporting to XLSX...')
         xl_wb = openpyxl.Workbook()
         xl_wb.properties.title = self.tr('Exported QSO log')
         xl_wb.properties.description = f'{__prog_name__} {__version__}'
         xl_wb.properties.creator = os.getlogin()
 
         xl_ws = xl_wb.active
         xl_ws.title = 'QSOs'
@@ -1102,107 +1118,161 @@
 
         if res[0]:
             imp_formats[res[1]](res[0])
 
             self.settings.setValue('lastImportDir', os.path.dirname(res[0]))
 
     def logImportExcel(self, file):
-        self.log.info('Importing from Excel...')
+        self.log.info('Importing from XLSX...')
 
         xl_wb = openpyxl.load_workbook(file, read_only=True, data_only=True)
         xl_ws = xl_wb.active
 
-        ln = 0
-        for row in xl_ws.iter_rows():
-            ln += 1
+        lines = 0
+
+        for ln, row in enumerate(xl_ws.iter_rows(), 1):
             if ln == 1:  # Skip header
                 continue
 
             row = list(row)
 
-            if len(row) >= len(self.__sql_cols__) and row[1].value:
-                query = QtSql.QSqlQuery(self.__db_con__)
-                query.prepare(self.__db_insert_stmnt__)
-
-                for i, cell in enumerate(row[1:]):
-                    query.bindValue(i, cell.value)
-                query.exec()
-                if query.lastError().text():
-                    QtWidgets.QMessageBox.warning(
-                        self,
-                        self.tr('Log import Excel'),
-                        f'Row {ln} import error ("{query.lastError().text()}").\nSkipped row.'
-                    )
-            else:
+            if not len(row) >= len(self.__sql_cols__):
+                self.log.warning(f'XLSX import, row {ln} has too few columns.\nSkipped row.')
                 QtWidgets.QMessageBox.warning(
                     self,
-                    self.tr('Log import Excel'),
+                    self.tr('Log import XLSX'),
                     f'Row {ln} has too few columns.\nSkipped row.'
                 )
+                continue
+
+            if not row[1].value or not row[4].value:
+                self.log.warning(f'XLSX import, QSO date/time or callsign missing in row {ln}.\nSkipped row.')
+                QtWidgets.QMessageBox.warning(
+                    self,
+                    self.tr('Log import XLSX'),
+                    f'QSO date/time or callsign missing in row {ln}.\nSkipped row.'
+                )
+                continue
+
+            if self.findQSO(row[1].value, row[4].value):
+                self.log.info(
+                    f'XLSX import, QSO row {ln} already exists for {row[1].value} and {row[4].value}. Skipping row.')
+                continue
+
+            query = QtSql.QSqlQuery(self.__db_con__)
+            query.prepare(self.__db_insert_stmnt__)
+
+            for i, cell in enumerate(row[1:]):
+                query.bindValue(i, cell.value)
+            query.exec()
+            if query.lastError().text():
+                QtWidgets.QMessageBox.warning(
+                    self,
+                    self.tr('Log import XLSX'),
+                    f'Row {ln} import error ("{query.lastError().text()}").\nSkipped row.'
+                )
+            else:
+                lines += 1
 
         self.__db_con__.commit()
         self.refreshTableView()
-        self.log.info(f'Imported {ln - 1} QSOs from "{file}"')
+        self.log.info(f'Imported {lines} QSOs from "{file}"')
 
     def logImportCSV(self, file):
         self.log.info('Importing from CSV...')
 
         with open(file, newline='', encoding='utf-8') as cf:
             reader = csv.reader(cf)
+            lines = 0
 
-            ln = 0
-            for row in reader:
-                ln += 1
+            for ln, row in enumerate(reader, 1):
                 if ln == 1:  # Skip header
                     continue
 
-                if len(row) >= len(self.__sql_cols__) and row[1]:
-                    query = QtSql.QSqlQuery(self.__db_con__)
-                    query.prepare(self.__db_insert_stmnt__)
-
-                    for i, val in enumerate(row[1:]):
-                        query.bindValue(i, val)
-                    query.exec()
-                    if query.lastError().text():
-                        QtWidgets.QMessageBox.warning(
-                            self,
-                            self.tr('Log import CSV'),
-                            f'Row {ln} import error ("{query.lastError().text()}").\nSkipped row.'
-                        )
-                else:
+                if not len(row) >= len(self.__sql_cols__):
+                    self.log.warning(f'CSV import, row {ln} has too few columns.\nSkipped row.')
                     QtWidgets.QMessageBox.warning(
                         self,
                         self.tr('Log import CSV'),
                         f'Row {ln} has too few columns.\nSkipped row.'
                     )
 
+                if not row[1] or not row[4]:
+                    self.log.warning(f'CSV import, QSO date/time or callsign missing in row {ln}.\nSkipped row.')
+                    QtWidgets.QMessageBox.warning(
+                        self,
+                        self.tr('Log import CSV'),
+                        f'QSO date/time or callsign missing in row {ln}.\nSkipped row.'
+                    )
+                    continue
+
+                if self.findQSO(row[1], row[4]):
+                    self.log.info(
+                        f'CSV import, QSO row {ln} already exists for {row[1]} and {row[4]}. Skipping row.')
+                    continue
+
+                query = QtSql.QSqlQuery(self.__db_con__)
+                query.prepare(self.__db_insert_stmnt__)
+
+                for i, val in enumerate(row[1:]):
+                    query.bindValue(i, val)
+                query.exec()
+                if query.lastError().text():
+                    QtWidgets.QMessageBox.warning(
+                        self,
+                        self.tr('Log import CSV'),
+                        f'Row {ln} import error ("{query.lastError().text()}").\nSkipped row.'
+                    )
+                else:
+                    lines += 1
+
         self.__db_con__.commit()
         self.refreshTableView()
-        self.log.info(f'Imported {ln - 1} QSOs from "{file}"')
+        self.log.info(f'Imported {lines} QSOs from "{file}"')
 
     def logImportADIF(self, file):
         self.log.info('Importing from ADIF...')
 
         is_adx: bool = os.path.splitext(file)[-1] == '.adx'
 
         if is_adx:
             records: list = adx.load(file)['RECORDS']
         else:
             records: list = adi.load(file)['RECORDS']
 
         imported = 0
         for i, r in enumerate(records, 1):
             if 'QSO_DATE' not in r or 'TIME_ON' not in r:
+                self.log.warning(f'ADIF import, QSO date/time missing in record {i}.\nSkipped record.')
                 QtWidgets.QMessageBox.warning(
                     self,
                     self.tr('Log import ADIF'),
                     f'QSO date/time missing in record {i}.\nSkipped record.'
                 )
                 continue
 
+            if 'CALL' not in r:
+                self.log.warning(f'ADIF import, callsign missing in record {i}.\nSkipped record.')
+                QtWidgets.QMessageBox.warning(
+                    self,
+                    self.tr('Log import ADIF'),
+                    f'Callsign missing in record {i}.\nSkipped record.'
+                )
+                continue
+
+            adi_time = r['TIME_ON']
+            adi_date = r['QSO_DATE']
+            time = f'{adi_time[:2]}:{adi_time[2:4]}' if len(
+                adi_time) == 4 else f'{adi_time[:2]}:{adi_time[2:4]}:{adi_time[4:6]}'
+            timestamp = f'{adi_date[:4]}-{adi_date[4:6]}-{adi_date[6:8]} {time}'
+
+            if self.findQSO(timestamp, r['CALL']):
+                self.log.info(f'ADIF import, QSO {i} already exists for {timestamp} and {r["CALL"]}. Skipping record.')
+                continue
+
             query = QtSql.QSqlQuery(self.__db_con__)
             query.prepare(self.__db_insert_stmnt__)
 
             for j, val in enumerate(self._build_adif_import_(r)):
                 query.bindValue(j, val)
             query.exec()
             if query.lastError().text():
```

### Comparing `dragonlog-1.2.1/dragonlog/DragonLog_AppSelect.py` & `dragonlog-1.3/dragonlog/DragonLog_AppSelect.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/DragonLog_AppSelect_ui.py` & `dragonlog-1.3/dragonlog/DragonLog_AppSelect_ui.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/DragonLog_MainWindow_ui.py` & `dragonlog-1.3/dragonlog/DragonLog_MainWindow_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,130 +158,126 @@
         self.verticalLayout_4.addWidget(self.label_2)
         self.fModeComboBox = QtWidgets.QComboBox(parent=self.dockWidgetContents_2)
         self.fModeComboBox.setObjectName("fModeComboBox")
         self.verticalLayout_4.addWidget(self.fModeComboBox)
         self.horizontalLayout_2.addLayout(self.verticalLayout_4)
         spacerItem2 = QtWidgets.QSpacerItem(10, 20, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Minimum)
         self.horizontalLayout_2.addItem(spacerItem2)
-        self.setFilterPushButton = QtWidgets.QPushButton(parent=self.dockWidgetContents_2)
-        icon1 = QtGui.QIcon()
-        icon1.addPixmap(QtGui.QPixmap("icons:filter.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.setFilterPushButton.setIcon(icon1)
-        self.setFilterPushButton.setObjectName("setFilterPushButton")
-        self.horizontalLayout_2.addWidget(self.setFilterPushButton)
         self.resetFilterPushButton = QtWidgets.QPushButton(parent=self.dockWidgetContents_2)
-        icon2 = QtGui.QIcon()
-        icon2.addPixmap(QtGui.QPixmap("icons:no.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.resetFilterPushButton.setIcon(icon2)
+        icon1 = QtGui.QIcon()
+        icon1.addPixmap(QtGui.QPixmap("icons:no.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.resetFilterPushButton.setIcon(icon1)
         self.resetFilterPushButton.setObjectName("resetFilterPushButton")
         self.horizontalLayout_2.addWidget(self.resetFilterPushButton)
         spacerItem3 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         self.horizontalLayout_2.addItem(spacerItem3)
         self.verticalLayout_8.addLayout(self.horizontalLayout_2)
         spacerItem4 = QtWidgets.QSpacerItem(20, 0, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
         self.verticalLayout_8.addItem(spacerItem4)
         self.filterDockWidget.setWidget(self.dockWidgetContents_2)
         MainWindow.addDockWidget(QtCore.Qt.DockWidgetArea(4), self.filterDockWidget)
         self.actionLog_QSO = QtGui.QAction(parent=MainWindow)
-        icon3 = QtGui.QIcon()
-        icon3.addPixmap(QtGui.QPixmap("icons:edit_add.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionLog_QSO.setIcon(icon3)
+        icon2 = QtGui.QIcon()
+        icon2.addPixmap(QtGui.QPixmap("icons:edit_add.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionLog_QSO.setIcon(icon2)
         self.actionLog_QSO.setObjectName("actionLog_QSO")
         self.actionLog_QSO_TB = QtGui.QAction(parent=MainWindow)
-        self.actionLog_QSO_TB.setIcon(icon3)
+        self.actionLog_QSO_TB.setIcon(icon2)
         self.actionLog_QSO_TB.setObjectName("actionLog_QSO_TB")
         self.actionSelect_DB = QtGui.QAction(parent=MainWindow)
-        icon4 = QtGui.QIcon()
-        icon4.addPixmap(QtGui.QPixmap("icons:db.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionSelect_DB.setIcon(icon4)
+        icon3 = QtGui.QIcon()
+        icon3.addPixmap(QtGui.QPixmap("icons:db.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionSelect_DB.setIcon(icon3)
         self.actionSelect_DB.setObjectName("actionSelect_DB")
         self.actionSelect_DB_TB = QtGui.QAction(parent=MainWindow)
-        self.actionSelect_DB_TB.setIcon(icon4)
+        self.actionSelect_DB_TB.setIcon(icon3)
         self.actionSelect_DB_TB.setObjectName("actionSelect_DB_TB")
         self.actionExit = QtGui.QAction(parent=MainWindow)
-        icon5 = QtGui.QIcon()
-        icon5.addPixmap(QtGui.QPixmap("icons:exit.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionExit.setIcon(icon5)
+        icon4 = QtGui.QIcon()
+        icon4.addPixmap(QtGui.QPixmap("icons:exit.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionExit.setIcon(icon4)
         self.actionExit.setObjectName("actionExit")
         self.actionExport = QtGui.QAction(parent=MainWindow)
-        icon6 = QtGui.QIcon()
-        icon6.addPixmap(QtGui.QPixmap("icons:fileexport.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionExport.setIcon(icon6)
+        icon5 = QtGui.QIcon()
+        icon5.addPixmap(QtGui.QPixmap("icons:fileexport.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionExport.setIcon(icon5)
         self.actionExport.setObjectName("actionExport")
         self.actionImport = QtGui.QAction(parent=MainWindow)
-        icon7 = QtGui.QIcon()
-        icon7.addPixmap(QtGui.QPixmap("icons:fileimport.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionImport.setIcon(icon7)
+        icon6 = QtGui.QIcon()
+        icon6.addPixmap(QtGui.QPixmap("icons:fileimport.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionImport.setIcon(icon6)
         self.actionImport.setObjectName("actionImport")
         self.actionExport_TB = QtGui.QAction(parent=MainWindow)
-        self.actionExport_TB.setIcon(icon6)
+        self.actionExport_TB.setIcon(icon5)
         self.actionExport_TB.setObjectName("actionExport_TB")
         self.actionImport_TB = QtGui.QAction(parent=MainWindow)
-        self.actionImport_TB.setIcon(icon7)
+        self.actionImport_TB.setIcon(icon6)
         self.actionImport_TB.setObjectName("actionImport_TB")
         self.actionAbout = QtGui.QAction(parent=MainWindow)
-        icon8 = QtGui.QIcon()
-        icon8.addPixmap(QtGui.QPixmap("icons:info.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionAbout.setIcon(icon8)
+        icon7 = QtGui.QIcon()
+        icon7.addPixmap(QtGui.QPixmap("icons:info.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionAbout.setIcon(icon7)
         self.actionAbout.setObjectName("actionAbout")
         self.actionAbout_Qt = QtGui.QAction(parent=MainWindow)
-        self.actionAbout_Qt.setIcon(icon8)
+        self.actionAbout_Qt.setIcon(icon7)
         self.actionAbout_Qt.setObjectName("actionAbout_Qt")
         self.actionDelete_log_entry = QtGui.QAction(parent=MainWindow)
-        icon9 = QtGui.QIcon()
-        icon9.addPixmap(QtGui.QPixmap("icons:edit_remove.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionDelete_log_entry.setIcon(icon9)
+        icon8 = QtGui.QIcon()
+        icon8.addPixmap(QtGui.QPixmap("icons:edit_remove.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionDelete_log_entry.setIcon(icon8)
         self.actionDelete_log_entry.setObjectName("actionDelete_log_entry")
         self.actionChange_log_entry = QtGui.QAction(parent=MainWindow)
-        icon10 = QtGui.QIcon()
-        icon10.addPixmap(QtGui.QPixmap("icons:edit.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionChange_log_entry.setIcon(icon10)
+        icon9 = QtGui.QIcon()
+        icon9.addPixmap(QtGui.QPixmap("icons:edit.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionChange_log_entry.setIcon(icon9)
         self.actionChange_log_entry.setObjectName("actionChange_log_entry")
         self.actionSettings = QtGui.QAction(parent=MainWindow)
-        icon11 = QtGui.QIcon()
-        icon11.addPixmap(QtGui.QPixmap("icons:gear.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionSettings.setIcon(icon11)
+        icon10 = QtGui.QIcon()
+        icon10.addPixmap(QtGui.QPixmap("icons:gear.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionSettings.setIcon(icon10)
         self.actionSettings.setObjectName("actionSettings")
         self.actionSettings_TB = QtGui.QAction(parent=MainWindow)
-        self.actionSettings_TB.setIcon(icon11)
+        self.actionSettings_TB.setIcon(icon10)
         self.actionSettings_TB.setObjectName("actionSettings_TB")
         self.actionHelp = QtGui.QAction(parent=MainWindow)
-        icon12 = QtGui.QIcon()
-        icon12.addPixmap(QtGui.QPixmap("icons:help.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionHelp.setIcon(icon12)
+        icon11 = QtGui.QIcon()
+        icon11.addPixmap(QtGui.QPixmap("icons:help.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionHelp.setIcon(icon11)
         self.actionHelp.setObjectName("actionHelp")
         self.actionStart_hamlib_TB = QtGui.QAction(parent=MainWindow)
         self.actionStart_hamlib_TB.setCheckable(True)
-        icon13 = QtGui.QIcon()
-        icon13.addPixmap(QtGui.QPixmap("icons:player_play.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        icon13.addPixmap(QtGui.QPixmap("icons:player_stop.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.On)
-        self.actionStart_hamlib_TB.setIcon(icon13)
+        icon12 = QtGui.QIcon()
+        icon12.addPixmap(QtGui.QPixmap("icons:player_play.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        icon12.addPixmap(QtGui.QPixmap("icons:player_stop.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.On)
+        self.actionStart_hamlib_TB.setIcon(icon12)
         self.actionStart_hamlib_TB.setObjectName("actionStart_hamlib_TB")
         self.actionWatch_file_for_QSOs = QtGui.QAction(parent=MainWindow)
         self.actionWatch_file_for_QSOs.setCheckable(True)
-        icon14 = QtGui.QIcon()
-        icon14.addPixmap(QtGui.QPixmap("icons:watch.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionWatch_file_for_QSOs.setIcon(icon14)
+        icon13 = QtGui.QIcon()
+        icon13.addPixmap(QtGui.QPixmap("icons:watch.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionWatch_file_for_QSOs.setIcon(icon13)
         self.actionWatch_file_for_QSOs.setObjectName("actionWatch_file_for_QSOs")
         self.actionWatch_file_for_QSOs_TB = QtGui.QAction(parent=MainWindow)
         self.actionWatch_file_for_QSOs_TB.setCheckable(True)
-        self.actionWatch_file_for_QSOs_TB.setIcon(icon14)
+        self.actionWatch_file_for_QSOs_TB.setIcon(icon13)
         self.actionWatch_file_for_QSOs_TB.setObjectName("actionWatch_file_for_QSOs_TB")
         self.actionShow_log = QtGui.QAction(parent=MainWindow)
-        icon15 = QtGui.QIcon()
-        icon15.addPixmap(QtGui.QPixmap("icons:file_doc.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionShow_log.setIcon(icon15)
+        icon14 = QtGui.QIcon()
+        icon14.addPixmap(QtGui.QPixmap("icons:file_doc.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionShow_log.setIcon(icon14)
         self.actionShow_log.setObjectName("actionShow_log")
         self.actionUpload_logs_to_LoTW = QtGui.QAction(parent=MainWindow)
-        icon16 = QtGui.QIcon()
-        icon16.addPixmap(QtGui.QPixmap("icons:upload_lotw.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionUpload_logs_to_LoTW.setIcon(icon16)
+        icon15 = QtGui.QIcon()
+        icon15.addPixmap(QtGui.QPixmap("icons:upload_lotw.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionUpload_logs_to_LoTW.setIcon(icon15)
         self.actionUpload_logs_to_LoTW.setObjectName("actionUpload_logs_to_LoTW")
         self.actionShow_filter = QtGui.QAction(parent=MainWindow)
-        self.actionShow_filter.setIcon(icon1)
+        icon16 = QtGui.QIcon()
+        icon16.addPixmap(QtGui.QPixmap("icons:filter.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionShow_filter.setIcon(icon16)
         self.actionShow_filter.setObjectName("actionShow_filter")
         self.menuFile.addAction(self.actionSelect_DB)
         self.menuFile.addSeparator()
         self.menuFile.addAction(self.actionExport)
         self.menuFile.addAction(self.actionImport)
         self.menuFile.addSeparator()
         self.menuFile.addAction(self.actionSettings)
@@ -334,17 +330,21 @@
         self.actionStart_hamlib_TB.triggered['bool'].connect(MainWindow.ctrlHamlib) # type: ignore
         self.actionSelect_DB_TB.triggered.connect(MainWindow.selectDB) # type: ignore
         self.actionWatch_file_for_QSOs.triggered['bool'].connect(MainWindow.ctrlWatching) # type: ignore
         self.actionWatch_file_for_QSOs_TB.triggered['bool'].connect(MainWindow.ctrlWatching) # type: ignore
         self.actionShow_log.triggered.connect(self.logDockWidget.show) # type: ignore
         self.actionUpload_logs_to_LoTW.triggered.connect(MainWindow.lotwUpload) # type: ignore
         self.QSOTableView.clicked['QModelIndex'].connect(MainWindow.clearQSOForm) # type: ignore
-        self.setFilterPushButton.clicked.connect(MainWindow.setTableFilter) # type: ignore
         self.resetFilterPushButton.clicked.connect(MainWindow.resetTableFilter) # type: ignore
         self.actionShow_filter.triggered.connect(self.filterDockWidget.show) # type: ignore
+        self.fCallsignLineEdit.editingFinished.connect(MainWindow.setTableFilter) # type: ignore
+        self.fBandComboBox.currentTextChanged['QString'].connect(MainWindow.setTableFilter) # type: ignore
+        self.fModeComboBox.currentTextChanged['QString'].connect(MainWindow.setTableFilter) # type: ignore
+        self.fDateToLineEdit.editingFinished.connect(MainWindow.setTableFilter) # type: ignore
+        self.fDateFromLineEdit.editingFinished.connect(MainWindow.setTableFilter) # type: ignore
         QtCore.QMetaObject.connectSlotsByName(MainWindow)
 
     def retranslateUi(self, MainWindow):
         _translate = QtCore.QCoreApplication.translate
         MainWindow.setWindowTitle(_translate("MainWindow", "DragonLog"))
         self.menuFile.setTitle(_translate("MainWindow", "File"))
         self.menuEdit.setTitle(_translate("MainWindow", "Edit"))
@@ -356,14 +356,15 @@
         self.label_4.setText(_translate("MainWindow", "Date from"))
         self.fDateFromLineEdit.setPlaceholderText(_translate("MainWindow", "YYYY-MM-DD"))
         self.label_5.setText(_translate("MainWindow", "Date to"))
         self.fDateToLineEdit.setPlaceholderText(_translate("MainWindow", "YYYY-MM-DD"))
         self.label.setText(_translate("MainWindow", "Callsign"))
         self.label_3.setText(_translate("MainWindow", "Band"))
         self.label_2.setText(_translate("MainWindow", "Mode"))
+        self.resetFilterPushButton.setShortcut(_translate("MainWindow", "Ctrl+R"))
         self.actionLog_QSO.setText(_translate("MainWindow", "Log QSO..."))
         self.actionLog_QSO.setShortcut(_translate("MainWindow", "Ctrl+L"))
         self.actionLog_QSO_TB.setText(_translate("MainWindow", "Log QSO..."))
         self.actionSelect_DB.setText(_translate("MainWindow", "Select database..."))
         self.actionSelect_DB_TB.setText(_translate("MainWindow", "Select database..."))
         self.actionExit.setText(_translate("MainWindow", "Exit"))
         self.actionExit.setShortcut(_translate("MainWindow", "Ctrl+Q"))
```

### Comparing `dragonlog-1.2.1/dragonlog/DragonLog_QSOForm - Kopie.py` & `dragonlog-1.3/dragonlog/DragonLog_QSOForm.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from .CallBook import (HamQTHCallBook, QRZCQCallBook, CallBookType, CallBookData,
                        SessionExpiredException, MissingADIFFieldException, LoginException, CallsignNotFoundException,
                        QSORejectedException, CommunicationException)
 from .eQSL import (EQSL, EQSLADIFFieldException, EQSLLoginException,
                    EQSLRequestException, EQSLUserCallMatchException, EQSLQSODuplicateException)
 from .LoTW import (LoTW, LoTWRequestException, LoTWCommunicationException,
                    LoTWLoginException, LoTWNoRecordException)
+from . import ColorPalettes
 
 
 class QSOForm(QtWidgets.QDialog, DragonLog_QSOForm_ui.Ui_QSOForm):
     def __init__(self, parent, dragonlog, bands: dict, modes: dict, prop: dict, settings: QtCore.QSettings,
                  settings_form: Settings, cb_channels: dict, hamlib_error: QtWidgets.QLabel, logger: Logger):
         super().__init__(parent)
         self.dragonlog = dragonlog
@@ -39,30 +40,14 @@
         self.prop_trans = dict(zip(prop.values(), prop.keys()))
         self.settings = settings
         self.settings_form = settings_form
         self.qso_id = None
 
         self.__old_values__ = {}
 
-        self.palette_default = QtGui.QPalette()
-        self.palette_default.setColor(QtGui.QPalette.ColorGroup.Active, QtGui.QPalette.ColorRole.Base,
-                                      QtGui.QColor(255, 255, 255))
-        self.palette_ok = QtGui.QPalette()
-        self.palette_ok.setColor(QtGui.QPalette.ColorGroup.Active, QtGui.QPalette.ColorRole.Base,
-                                 QtGui.QColor(204, 255, 204))
-        self.palette_empty = QtGui.QPalette()
-        self.palette_empty.setColor(QtGui.QPalette.ColorGroup.Active, QtGui.QPalette.ColorRole.Base,
-                                    QtGui.QColor(255, 255, 204))
-        self.palette_faulty = QtGui.QPalette()
-        self.palette_faulty.setColor(QtGui.QPalette.ColorGroup.Active, QtGui.QPalette.ColorRole.Base,
-                                     QtGui.QColor(255, 204, 204))
-        self.palette_worked = QtGui.QPalette()
-        self.palette_worked.setColor(QtGui.QPalette.ColorGroup.Active, QtGui.QPalette.ColorRole.Base,
-                                     QtGui.QColor(204, 204, 255))
-
         self.cb_channels = cb_channels
         self.channelComboBox.insertItems(0, ['-'] + list(cb_channels.keys()))
 
         self.bandComboBox.insertItems(0, bands.keys())
 
         self.propComboBox.insertItems(0, self.prop.values())
 
@@ -476,85 +461,85 @@
             self.modeComboBox.insertItems(0, self.cb_channels[ch]['modes'])
             self.modeComboBox.setCurrentIndex(0)
         else:
             self.freqDoubleSpinBox.setValue(self.bands['11m'][0] - self.bands['11m'][2])
 
     def rstRcvdChanged(self, txt):
         if not txt:
-            self.RSTRcvdLineEdit.setPalette(self.palette_empty)
+            self.RSTRcvdLineEdit.setPalette(ColorPalettes.PaletteEmpty)
         elif check_format(REGEX_RSTFIELD, txt):
-            self.RSTRcvdLineEdit.setPalette(self.palette_ok)
+            self.RSTRcvdLineEdit.setPalette(ColorPalettes.PaletteOk)
         else:
-            self.RSTRcvdLineEdit.setPalette(self.palette_faulty)
+            self.RSTRcvdLineEdit.setPalette(ColorPalettes.PaletteFaulty)
 
     def rstSentChanged(self, txt):
         if not txt:
-            self.RSTSentLineEdit.setPalette(self.palette_empty)
+            self.RSTSentLineEdit.setPalette(ColorPalettes.PaletteEmpty)
         elif check_format(REGEX_RSTFIELD, txt):
-            self.RSTSentLineEdit.setPalette(self.palette_ok)
+            self.RSTSentLineEdit.setPalette(ColorPalettes.PaletteOk)
         else:
-            self.RSTSentLineEdit.setPalette(self.palette_faulty)
+            self.RSTSentLineEdit.setPalette(ColorPalettes.PaletteFaulty)
 
     def callSignChanged(self, txt):
         self.setWorkedBefore()
         if not txt:
-            self.callSignLineEdit.setPalette(self.palette_empty)
+            self.callSignLineEdit.setPalette(ColorPalettes.PaletteEmpty)
         elif check_format(REGEX_CALL, txt):
             worked = self.dragonlog.workedBefore(check_call(txt)[1])
             if not self.__change_mode__ and worked:
                 self.setWorkedBefore(worked)
-                self.callSignLineEdit.setPalette(self.palette_worked)
+                self.callSignLineEdit.setPalette(ColorPalettes.PaletteWorked)
             else:
-                self.callSignLineEdit.setPalette(self.palette_ok)
+                self.callSignLineEdit.setPalette(ColorPalettes.PaletteOk)
         elif self.bandComboBox.currentText() == '11m':
-            self.callSignLineEdit.setPalette(self.palette_ok)
+            self.callSignLineEdit.setPalette(ColorPalettes.PaletteOk)
         else:
-            self.callSignLineEdit.setPalette(self.palette_faulty)
+            self.callSignLineEdit.setPalette(ColorPalettes.PaletteFaulty)
 
     def locatorChanged(self, txt):
         if not txt:
-            self.locatorLineEdit.setPalette(self.palette_empty)
+            self.locatorLineEdit.setPalette(ColorPalettes.PaletteEmpty)
         elif check_format(REGEX_LOCATOR, txt):
-            self.locatorLineEdit.setPalette(self.palette_ok)
+            self.locatorLineEdit.setPalette(ColorPalettes.PaletteOk)
         else:
-            self.locatorLineEdit.setPalette(self.palette_faulty)
+            self.locatorLineEdit.setPalette(ColorPalettes.PaletteFaulty)
 
     def ownCallSignChanged(self, txt):
         if not txt:
-            self.ownCallSignLineEdit.setPalette(self.palette_empty)
+            self.ownCallSignLineEdit.setPalette(ColorPalettes.PaletteEmpty)
         elif check_format(REGEX_CALL, txt):
-            self.ownCallSignLineEdit.setPalette(self.palette_ok)
+            self.ownCallSignLineEdit.setPalette(ColorPalettes.PaletteOk)
         elif self.bandComboBox.currentText() == '11m':
-            self.ownCallSignLineEdit.setPalette(self.palette_ok)
+            self.ownCallSignLineEdit.setPalette(ColorPalettes.PaletteOk)
         else:
-            self.ownCallSignLineEdit.setPalette(self.palette_faulty)
+            self.ownCallSignLineEdit.setPalette(ColorPalettes.PaletteFaulty)
 
     def ownQTHChanged(self, txt):
         if not txt:
-            self.ownQTHComboBox.setPalette(self.palette_empty)
+            self.ownQTHComboBox.setPalette(ColorPalettes.PaletteEmpty)
         elif check_qth(txt.strip()):
-            self.ownQTHComboBox.setPalette(self.palette_ok)
+            self.ownQTHComboBox.setPalette(ColorPalettes.PaletteOk)
         else:
-            self.ownQTHComboBox.setPalette(self.palette_faulty)
+            self.ownQTHComboBox.setPalette(ColorPalettes.PaletteFaulty)
 
     def timeOnChanged(self, txt):
         if not txt:
-            self.timeOnEdit.setPalette(self.palette_empty)
+            self.timeOnEdit.setPalette(ColorPalettes.PaletteEmpty)
         elif check_format(REGEX_TIME, txt):
-            self.timeOnEdit.setPalette(self.palette_ok)
+            self.timeOnEdit.setPalette(ColorPalettes.PaletteOk)
         else:
-            self.timeOnEdit.setPalette(self.palette_faulty)
+            self.timeOnEdit.setPalette(ColorPalettes.PaletteFaulty)
 
     def timeOffChanged(self, txt):
         if not txt:
-            self.timeOffEdit.setPalette(self.palette_empty)
+            self.timeOffEdit.setPalette(ColorPalettes.PaletteEmpty)
         elif check_format(REGEX_TIME, txt):
-            self.timeOffEdit.setPalette(self.palette_ok)
+            self.timeOffEdit.setPalette(ColorPalettes.PaletteOk)
         else:
-            self.timeOffEdit.setPalette(self.palette_faulty)
+            self.timeOffEdit.setPalette(ColorPalettes.PaletteFaulty)
 
     def calc_distance(self, mh_pos1: str, mh_pos2: str):
         # noinspection PyBroadException
         try:
             pos1 = maidenhead.to_location(mh_pos1, True)
             pos2 = maidenhead.to_location(mh_pos2, True)
```

### Comparing `dragonlog-1.2.1/dragonlog/DragonLog_QSOForm_ui.py` & `dragonlog-1.3/dragonlog/DragonLog_QSOForm_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,22 +152,20 @@
         self.stationGroupBox = QtWidgets.QGroupBox(parent=self.mainPage)
         self.stationGroupBox.setCheckable(True)
         self.stationGroupBox.setObjectName("stationGroupBox")
         self.verticalLayout_4 = QtWidgets.QVBoxLayout(self.stationGroupBox)
         self.verticalLayout_4.setObjectName("verticalLayout_4")
         self.horizontalLayout_7 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_7.setObjectName("horizontalLayout_7")
-        self.ownQTHLineEdit = QtWidgets.QLineEdit(parent=self.stationGroupBox)
-        self.ownQTHLineEdit.setEnabled(False)
-        self.ownQTHLineEdit.setObjectName("ownQTHLineEdit")
-        self.horizontalLayout_7.addWidget(self.ownQTHLineEdit)
-        self.ownLocatorLineEdit = QtWidgets.QLineEdit(parent=self.stationGroupBox)
-        self.ownLocatorLineEdit.setEnabled(False)
-        self.ownLocatorLineEdit.setObjectName("ownLocatorLineEdit")
-        self.horizontalLayout_7.addWidget(self.ownLocatorLineEdit)
+        self.ownQTHComboBox = QtWidgets.QComboBox(parent=self.stationGroupBox)
+        self.ownQTHComboBox.setEnabled(False)
+        self.ownQTHComboBox.setAutoFillBackground(True)
+        self.ownQTHComboBox.setEditable(True)
+        self.ownQTHComboBox.setObjectName("ownQTHComboBox")
+        self.horizontalLayout_7.addWidget(self.ownQTHComboBox)
         self.verticalLayout_4.addLayout(self.horizontalLayout_7)
         self.horizontalLayout_6 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_6.setObjectName("horizontalLayout_6")
         self.radioComboBox = QtWidgets.QComboBox(parent=self.stationGroupBox)
         self.radioComboBox.setEnabled(False)
         self.radioComboBox.setEditable(True)
         self.radioComboBox.setObjectName("radioComboBox")
@@ -431,27 +429,24 @@
         self.horizontalLayout_2.addWidget(self.cancelPushButton)
         self.verticalLayout.addLayout(self.horizontalLayout_2)
 
         self.retranslateUi(QSOForm)
         self.toolBox.setCurrentIndex(0)
         self.savePushButton.clicked.connect(QSOForm.saveLog) # type: ignore
         self.autoDateCheckBox.toggled['bool'].connect(self.dateOffEdit.setDisabled) # type: ignore
-        self.stationGroupBox.toggled['bool'].connect(self.ownLocatorLineEdit.setDisabled) # type: ignore
-        self.stationGroupBox.toggled['bool'].connect(self.ownQTHLineEdit.setDisabled) # type: ignore
         self.bandComboBox.currentTextChanged['QString'].connect(QSOForm.bandChanged) # type: ignore
         self.stationGroupBox.toggled['bool'].connect(QSOForm.stationChanged) # type: ignore
         self.identityGroupBox.toggled['bool'].connect(QSOForm.identityChanged) # type: ignore
         self.identityGroupBox.toggled['bool'].connect(self.ownCallSignLineEdit.setDisabled) # type: ignore
         self.identityGroupBox.toggled['bool'].connect(self.ownNameLineEdit.setDisabled) # type: ignore
         self.channelComboBox.currentTextChanged['QString'].connect(QSOForm.channelChanged) # type: ignore
         self.RSTRcvdLineEdit.textEdited['QString'].connect(QSOForm.rstRcvdChanged) # type: ignore
         self.RSTSentLineEdit.textEdited['QString'].connect(QSOForm.rstSentChanged) # type: ignore
         self.locatorLineEdit.textEdited['QString'].connect(QSOForm.locatorChanged) # type: ignore
         self.callSignLineEdit.textEdited['QString'].connect(QSOForm.callSignChanged) # type: ignore
-        self.ownLocatorLineEdit.textEdited['QString'].connect(QSOForm.ownLocatorChanged) # type: ignore
         self.ownCallSignLineEdit.textEdited['QString'].connect(QSOForm.ownCallSignChanged) # type: ignore
         self.callSignLineEdit.editingFinished.connect(QSOForm.setWorkedBefore) # type: ignore
         self.timeNowPushButton.clicked.connect(QSOForm.setStartTimeNow) # type: ignore
         self.searchHamQTHPushButton.clicked.connect(QSOForm.searchHamQTH) # type: ignore
         self.uploadPushButton.clicked.connect(QSOForm.uploadLog) # type: ignore
         self.eqslInboxPushButton.clicked.connect(QSOForm.eqslCheckInbox) # type: ignore
         self.eqslDownloadPushButton.clicked.connect(QSOForm.eqslDownload) # type: ignore
@@ -461,14 +456,16 @@
         self.autoDateCheckBox.toggled['bool'].connect(self.timeOffEdit.setDisabled) # type: ignore
         self.timeOnEdit.textEdited['QString'].connect(QSOForm.timeOnChanged) # type: ignore
         self.timeOffEdit.textEdited['QString'].connect(QSOForm.timeOffChanged) # type: ignore
         self.autoDateCheckBox.toggled['bool'].connect(QSOForm.autoDateCBChanged) # type: ignore
         self.searchQRZCQPushButton.clicked.connect(QSOForm.searchQRZCQ) # type: ignore
         self.stationGroupBox.toggled['bool'].connect(self.antennaComboBox.setDisabled) # type: ignore
         self.stationGroupBox.toggled['bool'].connect(self.radioComboBox.setDisabled) # type: ignore
+        self.stationGroupBox.toggled['bool'].connect(self.ownQTHComboBox.setDisabled) # type: ignore
+        self.ownQTHComboBox.editTextChanged['QString'].connect(QSOForm.ownQTHChanged) # type: ignore
         QtCore.QMetaObject.connectSlotsByName(QSOForm)
         QSOForm.setTabOrder(self.callSignLineEdit, self.searchHamQTHPushButton)
         QSOForm.setTabOrder(self.searchHamQTHPushButton, self.searchQRZCQPushButton)
         QSOForm.setTabOrder(self.searchQRZCQPushButton, self.RSTSentLineEdit)
         QSOForm.setTabOrder(self.RSTSentLineEdit, self.RSTRcvdLineEdit)
         QSOForm.setTabOrder(self.RSTRcvdLineEdit, self.bandComboBox)
         QSOForm.setTabOrder(self.bandComboBox, self.channelComboBox)
@@ -480,17 +477,15 @@
         QSOForm.setTabOrder(self.QTHLineEdit, self.locatorLineEdit)
         QSOForm.setTabOrder(self.locatorLineEdit, self.powerSpinBox)
         QSOForm.setTabOrder(self.powerSpinBox, self.propComboBox)
         QSOForm.setTabOrder(self.propComboBox, self.identityGroupBox)
         QSOForm.setTabOrder(self.identityGroupBox, self.ownCallSignLineEdit)
         QSOForm.setTabOrder(self.ownCallSignLineEdit, self.ownNameLineEdit)
         QSOForm.setTabOrder(self.ownNameLineEdit, self.stationGroupBox)
-        QSOForm.setTabOrder(self.stationGroupBox, self.ownQTHLineEdit)
-        QSOForm.setTabOrder(self.ownQTHLineEdit, self.ownLocatorLineEdit)
-        QSOForm.setTabOrder(self.ownLocatorLineEdit, self.timeNowPushButton)
+        QSOForm.setTabOrder(self.stationGroupBox, self.timeNowPushButton)
         QSOForm.setTabOrder(self.timeNowPushButton, self.autoDateCheckBox)
         QSOForm.setTabOrder(self.autoDateCheckBox, self.dateOnEdit)
         QSOForm.setTabOrder(self.dateOnEdit, self.dateOffEdit)
         QSOForm.setTabOrder(self.dateOffEdit, self.eqslSentCheckBox)
         QSOForm.setTabOrder(self.eqslSentCheckBox, self.lotwSentCheckBox)
         QSOForm.setTabOrder(self.lotwSentCheckBox, self.qslAccBureauCheckBox)
         QSOForm.setTabOrder(self.qslAccBureauCheckBox, self.qslViaLineEdit)
@@ -520,15 +515,17 @@
         _translate = QtCore.QCoreApplication.translate
         QSOForm.setWindowTitle(_translate("QSOForm", "QSO Form"))
         self.nameLineEdit.setPlaceholderText(_translate("QSOForm", "Name"))
         self.callSignLineEdit.setPlaceholderText(_translate("QSOForm", "Call sign"))
         self.QTHLineEdit.setPlaceholderText(_translate("QSOForm", "QTH"))
         self.locatorLineEdit.setPlaceholderText(_translate("QSOForm", "Locator"))
         self.searchHamQTHPushButton.setText(_translate("QSOForm", "HamQTH"))
+        self.searchHamQTHPushButton.setShortcut(_translate("QSOForm", "Ctrl+Alt+H"))
         self.searchQRZCQPushButton.setText(_translate("QSOForm", "QRZCQ"))
+        self.searchQRZCQPushButton.setShortcut(_translate("QSOForm", "Ctrl+Alt+Z"))
         self.label.setText(_translate("QSOForm", "RST Tx"))
         self.RSTSentLineEdit.setText(_translate("QSOForm", "59"))
         self.RSTSentLineEdit.setPlaceholderText(_translate("QSOForm", "RST sent"))
         self.label_2.setText(_translate("QSOForm", "RST Rx"))
         self.RSTRcvdLineEdit.setText(_translate("QSOForm", "59"))
         self.RSTRcvdLineEdit.setPlaceholderText(_translate("QSOForm", "RST received"))
         self.powerLabel.setText(_translate("QSOForm", "Power"))
@@ -542,17 +539,16 @@
         self.modeComboBox.setPlaceholderText(_translate("QSOForm", "Mode"))
         self.submodeComboBox.setPlaceholderText(_translate("QSOForm", "Submode"))
         self.propComboBox.setPlaceholderText(_translate("QSOForm", "Propagation"))
         self.identityGroupBox.setTitle(_translate("QSOForm", "Configured identity"))
         self.ownCallSignLineEdit.setPlaceholderText(_translate("QSOForm", "Own call sign"))
         self.ownNameLineEdit.setPlaceholderText(_translate("QSOForm", "Own name"))
         self.stationGroupBox.setTitle(_translate("QSOForm", "Configured station"))
-        self.ownQTHLineEdit.setPlaceholderText(_translate("QSOForm", "Own QTH"))
-        self.ownLocatorLineEdit.setPlaceholderText(_translate("QSOForm", "Own locator"))
         self.timeNowPushButton.setText(_translate("QSOForm", "Now"))
+        self.timeNowPushButton.setShortcut(_translate("QSOForm", "Ctrl+Alt+N"))
         self.label_4.setText(_translate("QSOForm", "End"))
         self.timeOnEdit.setPlaceholderText(_translate("QSOForm", "Time start"))
         self.autoDateCheckBox.setText(_translate("QSOForm", "Automatically"))
         self.label_3.setText(_translate("QSOForm", "Start"))
         self.dateOnEdit.setDisplayFormat(_translate("QSOForm", "yyyy-MM-dd"))
         self.dateOffEdit.setDisplayFormat(_translate("QSOForm", "yyyy-MM-dd"))
         self.timeOffEdit.setPlaceholderText(_translate("QSOForm", "Time end"))
@@ -574,28 +570,33 @@
         self.qslDirectRadioButton.setText(_translate("QSOForm", "Direct"))
         self.qslSentCheckBox.setText(_translate("QSOForm", "QSL sent"))
         self.qslRcvdCheckBox.setText(_translate("QSOForm", "QSL received"))
         self.eqslGroupBox.setTitle(_translate("QSOForm", "eQSL"))
         self.eqslSentCheckBox.setText(_translate("QSOForm", "eQSL sent"))
         self.eqslRcvdCheckBox.setText(_translate("QSOForm", "eQSL received"))
         self.eqslInboxPushButton.setText(_translate("QSOForm", "Check Inbox"))
+        self.eqslInboxPushButton.setShortcut(_translate("QSOForm", "Ctrl+Alt+E"))
         self.eqslLinkLabel.setText(_translate("QSOForm", "Link to eQSL Card"))
         self.eqslDownloadPushButton.setText(_translate("QSOForm", "Download eQSL"))
+        self.eqslDownloadPushButton.setShortcut(_translate("QSOForm", "Ctrl+Shift+E"))
         self.lotwGroupBox.setTitle(_translate("QSOForm", "LoTW"))
         self.lotwSentCheckBox.setText(_translate("QSOForm", "LoTW sent"))
         self.lotwRcvdCheckBox.setText(_translate("QSOForm", "LoTW received"))
         self.lotwInboxPushButton.setText(_translate("QSOForm", "Check Inbox"))
+        self.lotwInboxPushButton.setShortcut(_translate("QSOForm", "Ctrl+Alt+I"))
         self.callbookGroupBox.setTitle(_translate("QSOForm", "Logbook"))
         self.hamQTHCheckBox.setText(_translate("QSOForm", "HamQTH"))
         self.toolBox.setItemText(self.toolBox.indexOf(self.qslPage), _translate("QSOForm", "QSL && Log upload"))
         self.label_10.setText(_translate("QSOForm", "Contest ID"))
         self.contestComboBox.setPlaceholderText(_translate("QSOForm", "Contest ID"))
         self.label_6.setText(_translate("QSOForm", "Sent QSO ID"))
         self.sentQSOSpinBox.setSpecialValueText(_translate("QSOForm", "n.a."))
         self.label_9.setText(_translate("QSOForm", "Data"))
         self.label_8.setText(_translate("QSOForm", "Rcvd QSO ID"))
         self.rcvdQSOSpinBox.setSpecialValueText(_translate("QSOForm", "n.a."))
         self.toolBox.setItemText(self.toolBox.indexOf(self.contestPage), _translate("QSOForm", "Contest"))
         self.uploadPushButton.setToolTip(_translate("QSOForm", "Uploads only if selected on QSL page"))
         self.uploadPushButton.setText(_translate("QSOForm", "Save && Upload"))
+        self.uploadPushButton.setShortcut(_translate("QSOForm", "Ctrl+U"))
         self.savePushButton.setText(_translate("QSOForm", "Save"))
+        self.savePushButton.setShortcut(_translate("QSOForm", "Ctrl+S"))
         self.cancelPushButton.setText(_translate("QSOForm", "Clear"))
```

### Comparing `dragonlog-1.2.1/dragonlog/DragonLog_Settings.py` & `dragonlog-1.3/dragonlog/DragonLog_Settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 import sys
 import typing
 import logging
 import platform
 import subprocess
 
-import maidenhead
-from PyQt6 import QtWidgets, QtCore, QtGui
+from PyQt6 import QtWidgets, QtCore
 import keyring
 
 from . import DragonLog_Settings_ui
 from .Logger import Logger
-from .RegEx import REGEX_CALL, REGEX_LOCATOR, check_format
+from .RegEx import REGEX_CALL, check_format
 from .CallBook import CallBookType
 from .ListEdit import ListEdit
+from . import ColorPalettes
 
 # Fix problems with importing win32 in frozen executable
 if getattr(sys, 'frozen', False):
     # noinspection PyUnresolvedReferences
     import win32timezone
     from keyring.backends import Windows
 
@@ -36,19 +36,23 @@
 
         self.log = logging.getLogger('Settings')
         self.log.addHandler(logger)
         self.log.setLevel(logger.loglevel)
         self.logger = logger
         self.log.debug('Initialising...')
 
+        self.qthsListEdit = ListEdit(self.listingsWidget, self.tr('QTHs & locators'))
+        self.qthsListEdit.setToolTip(self.tr('Type in as: "City (Locator)", i.e. "Koblenz (JO30ti)"'))
+        self.listingsWidget.layout().addWidget(self.qthsListEdit, 0, 0, 1, 2)
+        self.qthsListEdit.listChanged.connect(self.refreshQTHsComboBox)
         self.rigsListEdit = ListEdit(self.listingsWidget, self.tr('Radios'))
-        self.listingsWidget.layout().addWidget(self.rigsListEdit, 0, 0, 1, 1)
+        self.listingsWidget.layout().addWidget(self.rigsListEdit, 1, 0, 1, 1)
         self.rigsListEdit.listChanged.connect(self.refreshRigsComboBox)
         self.antsListEdit = ListEdit(self.listingsWidget, self.tr('Antennas'))
-        self.listingsWidget.layout().addWidget(self.antsListEdit, 0, 1, 1, 1)
+        self.listingsWidget.layout().addWidget(self.antsListEdit, 1, 1, 1, 1)
         self.antsListEdit.listChanged.connect(self.refreshAntsComboBox)
 
         self.settings = settings
         self.rig_ids = None
         self.rigs = None
         self.rigctld_path = None
         self.rigctld = None
@@ -71,48 +75,35 @@
             self.hamlibPathToolButton.setVisible(False)
             self.checkHamlibLabel.setVisible(False)
             self.init_hamlib('rigctld')
 
         self.checkHamlibTimer = QtCore.QTimer(self)
         self.checkHamlibTimer.timeout.connect(self.checkRigctld)
 
-        self.palette_default = QtGui.QPalette()
-        self.palette_default.setColor(QtGui.QPalette.ColorGroup.Active, QtGui.QPalette.ColorRole.Base,
-                                      QtGui.QColor(255, 255, 255))
-        self.palette_ok = QtGui.QPalette()
-        self.palette_ok.setColor(QtGui.QPalette.ColorGroup.Active, QtGui.QPalette.ColorRole.Base,
-                                 QtGui.QColor(204, 255, 204))
-        self.palette_empty = QtGui.QPalette()
-        self.palette_empty.setColor(QtGui.QPalette.ColorGroup.Active, QtGui.QPalette.ColorRole.Base,
-                                    QtGui.QColor(255, 255, 204))
-        self.palette_faulty = QtGui.QPalette()
-        self.palette_faulty.setColor(QtGui.QPalette.ColorGroup.Active, QtGui.QPalette.ColorRole.Base,
-                                     QtGui.QColor(255, 204, 204))
-
         self.columns = cols
         self.sortComboBox.insertItems(0, cols)
 
         self.callbooks = dict([(cbt.value, cbt.name) for cbt in set(CallBookType)])
         self.callbookComboBox.insertItems(0, self.callbooks.keys())
 
+    def refreshQTHsComboBox(self):
+        self.qthComboBox.clear()
+        self.qthComboBox.insertItems(0, self.qthsListEdit.items())
+        self.qthComboBox.setCurrentText(self.settings.value('station/qth_loc', ''))
+
     def refreshRigsComboBox(self):
         self.radioComboBox.clear()
         self.radioComboBox.insertItems(0, self.rigsListEdit.items())
         self.radioComboBox.setCurrentText(self.settings.value('station/radio', ''))
 
     def refreshAntsComboBox(self):
         self.antennaComboBox.clear()
         self.antennaComboBox.insertItems(0, self.antsListEdit.items())
         self.antennaComboBox.setCurrentText(self.settings.value('station/antenna', ''))
 
-    def calcLocator(self):
-        self.locatorLineEdit.setText(maidenhead.to_maiden(self.latitudeDoubleSpinBox.value(),
-                                                          self.longitudeDoubleSpinBox.value(),
-                                                          4))
-
     def checkRigctld(self):
         if self.rigctld and self.rigctld.poll():
             self.log.error('rigctld died unexpectedly')
             self.ctrlRigctldPushButton.setText(self.tr('Start'))
             self.ctrlRigctldPushButton.setChecked(False)
             self.rig_caps = []
             self.checkHamlibTimer.stop()
@@ -279,35 +270,27 @@
             self.ctrlRigctldPushButton.setText(self.tr('Start'))
             self.parent().actionStart_hamlib_TB.setChecked(False)
             self.parent().actionStart_hamlib_TB.setText(self.tr('Start hamlib'))
             self.rig_status.setText(self.tr('Hamlib') + ': ' + self.tr('inactiv'))
             self.rig_caps = []
             self.rigctldStatusChanged.emit(False)
 
-    def locatorChanged(self, txt):
-        if not txt:
-            self.locatorLineEdit.setPalette(self.palette_empty)
-        elif check_format(REGEX_LOCATOR, txt):
-            self.locatorLineEdit.setPalette(self.palette_ok)
-        else:
-            self.locatorLineEdit.setPalette(self.palette_faulty)
-
     def callSignChanged(self, txt):
         if not txt:
-            self.callsignLineEdit.setPalette(self.palette_empty)
+            self.callsignLineEdit.setPalette(ColorPalettes.PaletteEmpty)
         elif check_format(REGEX_CALL, txt):
-            self.callsignLineEdit.setPalette(self.palette_ok)
+            self.callsignLineEdit.setPalette(ColorPalettes.PaletteOk)
         else:
-            self.callsignLineEdit.setPalette(self.palette_faulty)
+            self.callsignLineEdit.setPalette(ColorPalettes.PaletteFaulty)
 
     def callSignCBChanged(self, txt):
         if not txt:
-            self.callsignCBLineEdit.setPalette(self.palette_empty)
+            self.callsignCBLineEdit.setPalette(ColorPalettes.PaletteEmpty)
         else:
-            self.callsignCBLineEdit.setPalette(self.palette_ok)
+            self.callsignCBLineEdit.setPalette(ColorPalettes.PaletteOk)
 
     def hideCol(self):
         for item in self.colShowListWidget.selectedItems():
             self.colHideListWidget.insertItem(0, item.text())
             self.colShowListWidget.takeItem(self.colShowListWidget.row(item))
 
         self.colHideListWidget.sortItems()
@@ -324,23 +307,24 @@
         self.callbookUserLineEdit.setText(self.settings.value(f'callbook/{self.callbooks[service]}_user', ''))
 
     def exec(self):
         self.log.info('Loading settings...')
         self.catInterfaceLineEdit.setText(self.settings.value('cat/interface', ''))
         self.catBaudComboBox.setCurrentText(self.settings.value('cat/baud', ''))
 
+        self.qthsListEdit.clear()
+        self.qthsListEdit.setItems(self.settings.value('listings/qths'))
         self.rigsListEdit.clear()
         self.rigsListEdit.setItems(self.settings.value('listings/rigs'))
         self.antsListEdit.clear()
         self.antsListEdit.setItems(self.settings.value('listings/antennas'))
 
         self.callsignLineEdit.setText(self.settings.value('station/callSign', ''))
         self.nameLineEdit.setText(self.settings.value('station/name', ''))
-        self.QTHLineEdit.setText(self.settings.value('station/QTH', ''))
-        self.locatorLineEdit.setText(self.settings.value('station/locator', ''))
+        self.qthComboBox.setCurrentText(self.settings.value('station/qth_loc', ''))
         self.radioComboBox.setCurrentText(self.settings.value('station/radio', ''))
         self.antennaComboBox.setCurrentText(self.settings.value('station/antenna', ''))
 
         self.callsignCBLineEdit.setText(self.settings.value('station_cb/callSign', ''))
         self.radioCBLineEdit.setText(self.settings.value('station_cb/radio', ''))
         self.antennaCBLineEdit.setText(self.settings.value('station_cb/antenna', ''))
         self.cbDefaultCheckBox.setChecked(bool(self.settings.value('station_cb/cb_by_default', 0)))
@@ -411,19 +395,19 @@
         self.settings.setValue('cat/interface', self.catInterfaceLineEdit.text())
         self.settings.setValue('cat/baud', self.catBaudComboBox.currentText())
         self.settings.setValue('cat/rigMfr', self.manufacturerComboBox.currentText())
         self.settings.setValue('cat/rigModel', self.modelComboBox.currentText())
 
         self.settings.setValue('station/callSign', self.callsignLineEdit.text())
         self.settings.setValue('station/name', self.nameLineEdit.text())
-        self.settings.setValue('station/QTH', self.QTHLineEdit.text())
-        self.settings.setValue('station/locator', self.locatorLineEdit.text())
+        self.settings.setValue('station/qth_loc', self.qthComboBox.currentText())
         self.settings.setValue('station/radio', self.radioComboBox.currentText())
         self.settings.setValue('station/antenna', self.antennaComboBox.currentText())
 
+        self.settings.setValue('listings/qths', self.qthsListEdit.items())
         self.settings.setValue('listings/rigs', self.rigsListEdit.items())
         self.settings.setValue('listings/antennas', self.antsListEdit.items())
 
         self.settings.setValue('station_cb/callSign', self.callsignCBLineEdit.text())
         self.settings.setValue('station_cb/radio', self.radioCBLineEdit.text())
         self.settings.setValue('station_cb/antenna', self.antennaCBLineEdit.text())
         self.settings.setValue('station_cb/cb_by_default', int(self.cbDefaultCheckBox.isChecked()))
```

### Comparing `dragonlog-1.2.1/dragonlog/DragonLog_Settings_ui.py` & `dragonlog-1.3/dragonlog/DragonLog_Settings_ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,79 +28,42 @@
         self.formLayout.setObjectName("formLayout")
         self.label = QtWidgets.QLabel(parent=self.station)
         self.label.setObjectName("label")
         self.formLayout.setWidget(0, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label)
         self.callsignLineEdit = QtWidgets.QLineEdit(parent=self.station)
         self.callsignLineEdit.setObjectName("callsignLineEdit")
         self.formLayout.setWidget(0, QtWidgets.QFormLayout.ItemRole.FieldRole, self.callsignLineEdit)
-        self.label_3 = QtWidgets.QLabel(parent=self.station)
-        self.label_3.setObjectName("label_3")
-        self.formLayout.setWidget(2, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_3)
-        self.QTHLineEdit = QtWidgets.QLineEdit(parent=self.station)
-        self.QTHLineEdit.setObjectName("QTHLineEdit")
-        self.formLayout.setWidget(2, QtWidgets.QFormLayout.ItemRole.FieldRole, self.QTHLineEdit)
-        self.label_4 = QtWidgets.QLabel(parent=self.station)
-        self.label_4.setObjectName("label_4")
-        self.formLayout.setWidget(3, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_4)
-        self.locatorLineEdit = QtWidgets.QLineEdit(parent=self.station)
-        self.locatorLineEdit.setObjectName("locatorLineEdit")
-        self.formLayout.setWidget(3, QtWidgets.QFormLayout.ItemRole.FieldRole, self.locatorLineEdit)
-        self.horizontalLayout = QtWidgets.QHBoxLayout()
-        self.horizontalLayout.setContentsMargins(-1, -1, -1, 10)
-        self.horizontalLayout.setObjectName("horizontalLayout")
-        self.label_8 = QtWidgets.QLabel(parent=self.station)
-        self.label_8.setLayoutDirection(QtCore.Qt.LayoutDirection.LeftToRight)
-        self.label_8.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
-        self.label_8.setObjectName("label_8")
-        self.horizontalLayout.addWidget(self.label_8)
-        self.latitudeDoubleSpinBox = QtWidgets.QDoubleSpinBox(parent=self.station)
-        self.latitudeDoubleSpinBox.setDecimals(5)
-        self.latitudeDoubleSpinBox.setMinimum(-90.0)
-        self.latitudeDoubleSpinBox.setMaximum(90.0)
-        self.latitudeDoubleSpinBox.setObjectName("latitudeDoubleSpinBox")
-        self.horizontalLayout.addWidget(self.latitudeDoubleSpinBox)
-        self.label_7 = QtWidgets.QLabel(parent=self.station)
-        self.label_7.setLayoutDirection(QtCore.Qt.LayoutDirection.LeftToRight)
-        self.label_7.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
-        self.label_7.setObjectName("label_7")
-        self.horizontalLayout.addWidget(self.label_7)
-        self.longitudeDoubleSpinBox = QtWidgets.QDoubleSpinBox(parent=self.station)
-        self.longitudeDoubleSpinBox.setDecimals(5)
-        self.longitudeDoubleSpinBox.setMinimum(-180.0)
-        self.longitudeDoubleSpinBox.setMaximum(180.0)
-        self.longitudeDoubleSpinBox.setObjectName("longitudeDoubleSpinBox")
-        self.horizontalLayout.addWidget(self.longitudeDoubleSpinBox)
-        spacerItem = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
-        self.horizontalLayout.addItem(spacerItem)
-        self.setLocatorPushButton = QtWidgets.QPushButton(parent=self.station)
-        self.setLocatorPushButton.setObjectName("setLocatorPushButton")
-        self.horizontalLayout.addWidget(self.setLocatorPushButton)
-        self.formLayout.setLayout(4, QtWidgets.QFormLayout.ItemRole.FieldRole, self.horizontalLayout)
-        self.label_5 = QtWidgets.QLabel(parent=self.station)
-        self.label_5.setObjectName("label_5")
-        self.formLayout.setWidget(6, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_5)
-        self.label_6 = QtWidgets.QLabel(parent=self.station)
-        self.label_6.setObjectName("label_6")
-        self.formLayout.setWidget(7, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_6)
-        spacerItem1 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Minimum)
-        self.formLayout.setItem(5, QtWidgets.QFormLayout.ItemRole.FieldRole, spacerItem1)
         self.label_2 = QtWidgets.QLabel(parent=self.station)
         self.label_2.setObjectName("label_2")
         self.formLayout.setWidget(1, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_2)
         self.nameLineEdit = QtWidgets.QLineEdit(parent=self.station)
         self.nameLineEdit.setObjectName("nameLineEdit")
         self.formLayout.setWidget(1, QtWidgets.QFormLayout.ItemRole.FieldRole, self.nameLineEdit)
-        spacerItem2 = QtWidgets.QSpacerItem(20, 500, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
-        self.formLayout.setItem(8, QtWidgets.QFormLayout.ItemRole.FieldRole, spacerItem2)
+        self.label_3 = QtWidgets.QLabel(parent=self.station)
+        self.label_3.setObjectName("label_3")
+        self.formLayout.setWidget(2, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_3)
+        spacerItem = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Minimum)
+        self.formLayout.setItem(3, QtWidgets.QFormLayout.ItemRole.FieldRole, spacerItem)
+        self.label_5 = QtWidgets.QLabel(parent=self.station)
+        self.label_5.setObjectName("label_5")
+        self.formLayout.setWidget(4, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_5)
         self.radioComboBox = QtWidgets.QComboBox(parent=self.station)
         self.radioComboBox.setObjectName("radioComboBox")
-        self.formLayout.setWidget(6, QtWidgets.QFormLayout.ItemRole.FieldRole, self.radioComboBox)
+        self.formLayout.setWidget(4, QtWidgets.QFormLayout.ItemRole.FieldRole, self.radioComboBox)
+        self.label_6 = QtWidgets.QLabel(parent=self.station)
+        self.label_6.setObjectName("label_6")
+        self.formLayout.setWidget(5, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_6)
         self.antennaComboBox = QtWidgets.QComboBox(parent=self.station)
         self.antennaComboBox.setObjectName("antennaComboBox")
-        self.formLayout.setWidget(7, QtWidgets.QFormLayout.ItemRole.FieldRole, self.antennaComboBox)
+        self.formLayout.setWidget(5, QtWidgets.QFormLayout.ItemRole.FieldRole, self.antennaComboBox)
+        spacerItem1 = QtWidgets.QSpacerItem(20, 500, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
+        self.formLayout.setItem(6, QtWidgets.QFormLayout.ItemRole.FieldRole, spacerItem1)
+        self.qthComboBox = QtWidgets.QComboBox(parent=self.station)
+        self.qthComboBox.setObjectName("qthComboBox")
+        self.formLayout.setWidget(2, QtWidgets.QFormLayout.ItemRole.FieldRole, self.qthComboBox)
         self.tabWidget.addTab(self.station, "")
         self.listings = QtWidgets.QWidget()
         self.listings.setObjectName("listings")
         self.verticalLayout_12 = QtWidgets.QVBoxLayout(self.listings)
         self.verticalLayout_12.setObjectName("verticalLayout_12")
         self.listingsWidget = QtWidgets.QWidget(parent=self.listings)
         self.listingsWidget.setObjectName("listingsWidget")
@@ -126,16 +89,16 @@
         self.formLayout_2.setWidget(1, QtWidgets.QFormLayout.ItemRole.FieldRole, self.radioCBLineEdit)
         self.label_11 = QtWidgets.QLabel(parent=self.cb_station)
         self.label_11.setObjectName("label_11")
         self.formLayout_2.setWidget(2, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_11)
         self.antennaCBLineEdit = QtWidgets.QLineEdit(parent=self.cb_station)
         self.antennaCBLineEdit.setObjectName("antennaCBLineEdit")
         self.formLayout_2.setWidget(2, QtWidgets.QFormLayout.ItemRole.FieldRole, self.antennaCBLineEdit)
-        spacerItem3 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
-        self.formLayout_2.setItem(5, QtWidgets.QFormLayout.ItemRole.FieldRole, spacerItem3)
+        spacerItem2 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
+        self.formLayout_2.setItem(5, QtWidgets.QFormLayout.ItemRole.FieldRole, spacerItem2)
         self.cbDefaultCheckBox = QtWidgets.QCheckBox(parent=self.cb_station)
         self.cbDefaultCheckBox.setObjectName("cbDefaultCheckBox")
         self.formLayout_2.setWidget(3, QtWidgets.QFormLayout.ItemRole.FieldRole, self.cbDefaultCheckBox)
         self.expCBQSOsCheckBox = QtWidgets.QCheckBox(parent=self.cb_station)
         self.expCBQSOsCheckBox.setObjectName("expCBQSOsCheckBox")
         self.formLayout_2.setWidget(4, QtWidgets.QFormLayout.ItemRole.FieldRole, self.expCBQSOsCheckBox)
         self.tabWidget.addTab(self.cb_station, "")
@@ -199,31 +162,31 @@
         self.manufacturerComboBox = QtWidgets.QComboBox(parent=self.cat)
         self.manufacturerComboBox.setObjectName("manufacturerComboBox")
         self.horizontalLayout_3.addWidget(self.manufacturerComboBox)
         self.modelComboBox = QtWidgets.QComboBox(parent=self.cat)
         self.modelComboBox.setObjectName("modelComboBox")
         self.horizontalLayout_3.addWidget(self.modelComboBox)
         self.formLayout_3.setLayout(5, QtWidgets.QFormLayout.ItemRole.FieldRole, self.horizontalLayout_3)
-        spacerItem4 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Minimum)
-        self.formLayout_3.setItem(6, QtWidgets.QFormLayout.ItemRole.FieldRole, spacerItem4)
+        spacerItem3 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Minimum)
+        self.formLayout_3.setItem(6, QtWidgets.QFormLayout.ItemRole.FieldRole, spacerItem3)
         self.horizontalLayout_4 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_4.setObjectName("horizontalLayout_4")
         self.ctrlRigctldPushButton = QtWidgets.QPushButton(parent=self.cat)
         self.ctrlRigctldPushButton.setCheckable(True)
         self.ctrlRigctldPushButton.setObjectName("ctrlRigctldPushButton")
         self.horizontalLayout_4.addWidget(self.ctrlRigctldPushButton)
-        spacerItem5 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
-        self.horizontalLayout_4.addItem(spacerItem5)
+        spacerItem4 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
+        self.horizontalLayout_4.addItem(spacerItem4)
         self.formLayout_3.setLayout(7, QtWidgets.QFormLayout.ItemRole.FieldRole, self.horizontalLayout_4)
         self.checkHamlibRunLabel = QtWidgets.QLabel(parent=self.cat)
         self.checkHamlibRunLabel.setText("")
         self.checkHamlibRunLabel.setObjectName("checkHamlibRunLabel")
         self.formLayout_3.setWidget(9, QtWidgets.QFormLayout.ItemRole.FieldRole, self.checkHamlibRunLabel)
-        spacerItem6 = QtWidgets.QSpacerItem(20, 1000, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
-        self.formLayout_3.setItem(8, QtWidgets.QFormLayout.ItemRole.FieldRole, spacerItem6)
+        spacerItem5 = QtWidgets.QSpacerItem(20, 1000, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
+        self.formLayout_3.setItem(8, QtWidgets.QFormLayout.ItemRole.FieldRole, spacerItem5)
         self.tabWidget.addTab(self.cat, "")
         self.userinterface = QtWidgets.QWidget()
         self.userinterface.setObjectName("userinterface")
         self.horizontalLayout_6 = QtWidgets.QHBoxLayout(self.userinterface)
         self.horizontalLayout_6.setObjectName("horizontalLayout_6")
         self.verticalLayout_5 = QtWidgets.QVBoxLayout()
         self.verticalLayout_5.setObjectName("verticalLayout_5")
@@ -232,30 +195,30 @@
         self.horizontalLayout_8 = QtWidgets.QHBoxLayout(self.groupBox_2)
         self.horizontalLayout_8.setObjectName("horizontalLayout_8")
         self.verticalLayout_11 = QtWidgets.QVBoxLayout()
         self.verticalLayout_11.setObjectName("verticalLayout_11")
         self.sortComboBox = QtWidgets.QComboBox(parent=self.groupBox_2)
         self.sortComboBox.setObjectName("sortComboBox")
         self.verticalLayout_11.addWidget(self.sortComboBox)
-        spacerItem7 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
-        self.verticalLayout_11.addItem(spacerItem7)
+        spacerItem6 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
+        self.verticalLayout_11.addItem(spacerItem6)
         self.horizontalLayout_8.addLayout(self.verticalLayout_11)
         self.verticalLayout_10 = QtWidgets.QVBoxLayout()
         self.verticalLayout_10.setObjectName("verticalLayout_10")
         self.sortAscRadioButton = QtWidgets.QRadioButton(parent=self.groupBox_2)
         self.sortAscRadioButton.setChecked(True)
         self.sortAscRadioButton.setObjectName("sortAscRadioButton")
         self.verticalLayout_10.addWidget(self.sortAscRadioButton)
         self.sortDscRadioButton = QtWidgets.QRadioButton(parent=self.groupBox_2)
         self.sortDscRadioButton.setObjectName("sortDscRadioButton")
         self.verticalLayout_10.addWidget(self.sortDscRadioButton)
         self.horizontalLayout_8.addLayout(self.verticalLayout_10)
         self.verticalLayout_5.addWidget(self.groupBox_2)
-        spacerItem8 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
-        self.verticalLayout_5.addItem(spacerItem8)
+        spacerItem7 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
+        self.verticalLayout_5.addItem(spacerItem7)
         self.groupBox_7 = QtWidgets.QGroupBox(parent=self.userinterface)
         self.groupBox_7.setObjectName("groupBox_7")
         self.horizontalLayout_9 = QtWidgets.QHBoxLayout(self.groupBox_7)
         self.horizontalLayout_9.setObjectName("horizontalLayout_9")
         self.label_20 = QtWidgets.QLabel(parent=self.groupBox_7)
         self.label_20.setObjectName("label_20")
         self.horizontalLayout_9.addWidget(self.label_20)
@@ -263,16 +226,16 @@
         self.recentQSOsComboBox.setObjectName("recentQSOsComboBox")
         self.recentQSOsComboBox.addItem("")
         self.recentQSOsComboBox.addItem("")
         self.recentQSOsComboBox.addItem("")
         self.recentQSOsComboBox.addItem("")
         self.recentQSOsComboBox.addItem("")
         self.horizontalLayout_9.addWidget(self.recentQSOsComboBox)
-        spacerItem9 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
-        self.horizontalLayout_9.addItem(spacerItem9)
+        spacerItem8 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
+        self.horizontalLayout_9.addItem(spacerItem8)
         self.verticalLayout_5.addWidget(self.groupBox_7)
         self.groupBox = QtWidgets.QGroupBox(parent=self.userinterface)
         self.groupBox.setObjectName("groupBox")
         self.horizontalLayout_7 = QtWidgets.QHBoxLayout(self.groupBox)
         self.horizontalLayout_7.setObjectName("horizontalLayout_7")
         self.verticalLayout_3 = QtWidgets.QVBoxLayout()
         self.verticalLayout_3.setObjectName("verticalLayout_3")
@@ -282,16 +245,16 @@
         self.colShowListWidget = QtWidgets.QListWidget(parent=self.groupBox)
         self.colShowListWidget.setObjectName("colShowListWidget")
         self.verticalLayout_3.addWidget(self.colShowListWidget)
         self.horizontalLayout_7.addLayout(self.verticalLayout_3)
         self.verticalLayout_2 = QtWidgets.QVBoxLayout()
         self.verticalLayout_2.setSpacing(6)
         self.verticalLayout_2.setObjectName("verticalLayout_2")
-        spacerItem10 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
-        self.verticalLayout_2.addItem(spacerItem10)
+        spacerItem9 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
+        self.verticalLayout_2.addItem(spacerItem9)
         self.hideColPushButton = QtWidgets.QPushButton(parent=self.groupBox)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Minimum)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.hideColPushButton.sizePolicy().hasHeightForWidth())
         self.hideColPushButton.setSizePolicy(sizePolicy)
         self.hideColPushButton.setMaximumSize(QtCore.QSize(20, 16777215))
@@ -302,16 +265,16 @@
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.showColPushButton.sizePolicy().hasHeightForWidth())
         self.showColPushButton.setSizePolicy(sizePolicy)
         self.showColPushButton.setMaximumSize(QtCore.QSize(20, 16777215))
         self.showColPushButton.setObjectName("showColPushButton")
         self.verticalLayout_2.addWidget(self.showColPushButton)
-        spacerItem11 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
-        self.verticalLayout_2.addItem(spacerItem11)
+        spacerItem10 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
+        self.verticalLayout_2.addItem(spacerItem10)
         self.horizontalLayout_7.addLayout(self.verticalLayout_2)
         self.verticalLayout_4 = QtWidgets.QVBoxLayout()
         self.verticalLayout_4.setObjectName("verticalLayout_4")
         self.label_15 = QtWidgets.QLabel(parent=self.groupBox)
         self.label_15.setObjectName("label_15")
         self.verticalLayout_4.addWidget(self.label_15)
         self.colHideListWidget = QtWidgets.QListWidget(parent=self.groupBox)
@@ -339,16 +302,16 @@
         self.logLevelComboBox.setItemText(3, "Error")
         self.logLevelComboBox.addItem("")
         self.logLevelComboBox.setItemText(4, "Critical")
         self.horizontalLayout_10.addWidget(self.logLevelComboBox)
         self.logToFileCheckBox = QtWidgets.QCheckBox(parent=self.groupBox_8)
         self.logToFileCheckBox.setObjectName("logToFileCheckBox")
         self.horizontalLayout_10.addWidget(self.logToFileCheckBox)
-        spacerItem12 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
-        self.horizontalLayout_10.addItem(spacerItem12)
+        spacerItem11 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
+        self.horizontalLayout_10.addItem(spacerItem11)
         self.verticalLayout_5.addWidget(self.groupBox_8)
         self.horizontalLayout_6.addLayout(self.verticalLayout_5)
         self.tabWidget.addTab(self.userinterface, "")
         self.import_export = QtWidgets.QWidget()
         self.import_export.setObjectName("import_export")
         self.verticalLayout_6 = QtWidgets.QVBoxLayout(self.import_export)
         self.verticalLayout_6.setObjectName("verticalLayout_6")
@@ -370,16 +333,16 @@
         self.useCfgIDWatchCheckBox = QtWidgets.QCheckBox(parent=self.groupBox_4)
         self.useCfgIDWatchCheckBox.setObjectName("useCfgIDWatchCheckBox")
         self.verticalLayout_8.addWidget(self.useCfgIDWatchCheckBox)
         self.useCfgStationWatchCheckBox = QtWidgets.QCheckBox(parent=self.groupBox_4)
         self.useCfgStationWatchCheckBox.setObjectName("useCfgStationWatchCheckBox")
         self.verticalLayout_8.addWidget(self.useCfgStationWatchCheckBox)
         self.verticalLayout_6.addWidget(self.groupBox_4)
-        spacerItem13 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
-        self.verticalLayout_6.addItem(spacerItem13)
+        spacerItem12 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
+        self.verticalLayout_6.addItem(spacerItem12)
         self.tabWidget.addTab(self.import_export, "")
         self.credentials = QtWidgets.QWidget()
         self.credentials.setObjectName("credentials")
         self.verticalLayout_9 = QtWidgets.QVBoxLayout(self.credentials)
         self.verticalLayout_9.setObjectName("verticalLayout_9")
         self.groupBox_5 = QtWidgets.QGroupBox(parent=self.credentials)
         self.groupBox_5.setObjectName("groupBox_5")
@@ -448,35 +411,32 @@
         self.formLayout_6.setWidget(3, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_23)
         self.line = QtWidgets.QFrame(parent=self.groupBox_81)
         self.line.setFrameShape(QtWidgets.QFrame.Shape.HLine)
         self.line.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.line.setObjectName("line")
         self.formLayout_6.setWidget(2, QtWidgets.QFormLayout.ItemRole.FieldRole, self.line)
         self.verticalLayout_9.addWidget(self.groupBox_81)
-        spacerItem14 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
-        self.verticalLayout_9.addItem(spacerItem14)
+        spacerItem13 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
+        self.verticalLayout_9.addItem(spacerItem13)
         self.tabWidget.addTab(self.credentials, "")
         self.verticalLayout.addWidget(self.tabWidget)
         self.buttonBox = QtWidgets.QDialogButtonBox(parent=Dialog)
         self.buttonBox.setOrientation(QtCore.Qt.Orientation.Horizontal)
         self.buttonBox.setStandardButtons(QtWidgets.QDialogButtonBox.StandardButton.Cancel|QtWidgets.QDialogButtonBox.StandardButton.Ok)
         self.buttonBox.setObjectName("buttonBox")
         self.verticalLayout.addWidget(self.buttonBox)
 
         self.retranslateUi(Dialog)
         self.tabWidget.setCurrentIndex(0)
         self.logLevelComboBox.setCurrentIndex(1)
         self.buttonBox.accepted.connect(Dialog.accept) # type: ignore
         self.buttonBox.rejected.connect(Dialog.reject) # type: ignore
-        self.setLocatorPushButton.clicked.connect(Dialog.calcLocator) # type: ignore
         self.ctrlRigctldPushButton.toggled['bool'].connect(Dialog.ctrlRigctld) # type: ignore
         self.hamlibPathToolButton.clicked.connect(Dialog.chooseHamlibPath) # type: ignore
         self.manufacturerComboBox.currentTextChanged['QString'].connect(Dialog.mfrChanged) # type: ignore
-        self.locatorLineEdit.textChanged['QString'].connect(Dialog.locatorChanged) # type: ignore
-        self.locatorLineEdit.textEdited['QString'].connect(Dialog.locatorChanged) # type: ignore
         self.callsignCBLineEdit.textChanged['QString'].connect(Dialog.callSignCBChanged) # type: ignore
         self.callsignLineEdit.textChanged['QString'].connect(Dialog.callSignChanged) # type: ignore
         self.callsignCBLineEdit.textEdited['QString'].connect(Dialog.callSignCBChanged) # type: ignore
         self.callsignLineEdit.textEdited['QString'].connect(Dialog.callSignChanged) # type: ignore
         self.hideColPushButton.clicked.connect(Dialog.hideCol) # type: ignore
         self.showColPushButton.clicked.connect(Dialog.showCol) # type: ignore
         self.colHideListWidget.itemDoubleClicked['QListWidgetItem*'].connect(Dialog.showCol) # type: ignore
@@ -484,24 +444,18 @@
         self.callbookComboBox.currentTextChanged['QString'].connect(Dialog.callbookSelected) # type: ignore
         QtCore.QMetaObject.connectSlotsByName(Dialog)
 
     def retranslateUi(self, Dialog):
         _translate = QtCore.QCoreApplication.translate
         Dialog.setWindowTitle(_translate("Dialog", "Settings"))
         self.label.setText(_translate("Dialog", "Call sign"))
-        self.label_3.setText(_translate("Dialog", "QTH"))
-        self.label_4.setText(_translate("Dialog", "Locator"))
-        self.label_8.setText(_translate("Dialog", "Lat"))
-        self.latitudeDoubleSpinBox.setSuffix(_translate("Dialog", "°"))
-        self.label_7.setText(_translate("Dialog", "Lon"))
-        self.longitudeDoubleSpinBox.setSuffix(_translate("Dialog", "°"))
-        self.setLocatorPushButton.setText(_translate("Dialog", "Set locator"))
+        self.label_2.setText(_translate("Dialog", "Name"))
+        self.label_3.setText(_translate("Dialog", "QTH (Locator)"))
         self.label_5.setText(_translate("Dialog", "Radio"))
         self.label_6.setText(_translate("Dialog", "Antenna"))
-        self.label_2.setText(_translate("Dialog", "Name"))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.station), _translate("Dialog", "Station"))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.listings), _translate("Dialog", "Listings"))
         self.label_10.setText(_translate("Dialog", "Call sign"))
         self.label_9.setText(_translate("Dialog", "Radio"))
         self.label_11.setText(_translate("Dialog", "Antenna"))
         self.cbDefaultCheckBox.setText(_translate("Dialog", "Select CB band by default"))
         self.expCBQSOsCheckBox.setToolTip(_translate("Dialog", "On import CB QSOs will always be handled"))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dragonlog-1.2.1/dragonlog/ListEdit.py` & `dragonlog-1.3/dragonlog/ListEdit.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/ListEdit_ui.py` & `dragonlog-1.3/dragonlog/ListEdit_ui.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/LoTW.py` & `dragonlog-1.3/dragonlog/LoTW.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/Logger.py` & `dragonlog-1.3/dragonlog/Logger.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/RegEx.py` & `dragonlog-1.3/dragonlog/RegEx.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,26 +3,40 @@
 
 REGEX_CALL = re.compile(r'([a-zA-Z0-9]{1,3}?/)?([a-zA-Z0-9]{1,3}?[0-9][a-zA-Z0-9]{0,3}?[a-zA-Z])(/[aAmMpPrRtT]{1,2}?)?')
 REGEX_RSTFIELD = re.compile(r'([1-5][1-9][1-9aAcCkKmMsSxX]?)|([rR]?[-+]?[0-9]{1,2})')
 REGEX_LOCATOR = re.compile(r'[a-rA-R]{2}[0-9]{2}([a-xA-X]{2}([0-9]{2})?)?')
 REGEX_NONASCII = re.compile(r'[ -~\n\r]*(.)?')
 REGEX_TIME = re.compile(r'(([0-1][0-9])|(2[0-3])):([0-5][0-9])(:[0-5][0-9])?')
 REGEX_DATE = re.compile(r'([1-9][0-9]{3})-((0[1-9])|(1[0-2]))-((0[1-9])|([1-2][0-9])|(3[0-2]))')
+REGEX_QTH = re.compile(r'(.*)? \(([a-rA-R]{2}[0-9]{2}([a-xA-X]{2}([0-9]{2})?)?)\)')
+
 
 def check_format(exp: re.Pattern, txt: str) -> bool:
     """Test the given text against a regular expression
     :param exp: a compiled pattern
     :param txt: a text
     :return: true if pattern matches"""
     return bool(re.fullmatch(exp, txt))
 
-def check_call(call: str) -> None|tuple:
+
+def check_call(call: str) -> None | tuple:
     """Test a call sign against a regular expression
     :param call: a call sign
     :return: tuple of parts ('Country prefix/', 'Call sign', '/Operation suffix')"""
 
     m = re.fullmatch(REGEX_CALL, call)
     if m:
         return m.groups()
 
+
 def find_non_ascii(text: str) -> set:
     return set(re.findall(REGEX_NONASCII, text))
+
+
+def check_qth(qth_loc: str) -> None | tuple:
+    """Test a QTH + locator against a regular expression
+    :param qth_loc: "QTH (locator)"
+    :return: tuple of parts ('QTH', 'locator')"""
+
+    m = re.fullmatch(REGEX_QTH, qth_loc.strip())
+    if m:
+        return m.groups()[:2]
```

### Comparing `dragonlog-1.2.1/dragonlog/data/README.md` & `dragonlog-1.3/dragonlog/data/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,17 @@
 Starting file watching opens a file dialog where you have to point to the log in question.
 Check the manual of the other program to find the correct path.
 
 If you want to use the worked before feature of the other program consider to export your 
 QSOs beforehand.
 Dragonlog will only import QSOs which are not already included in the current database.
 
+[Keyboard shortcuts](SHORTCUTS.md)
+----------------------------------
+
 Export
 ------
 Following formats are supported for export
 * [ADIF 3](https://adif.org/) format (ADI/ADX)
 * Excel file
 * CSV format (UTF-8 encoding)
```

### Comparing `dragonlog-1.2.1/dragonlog/data/bands.json` & `dragonlog-1.3/dragonlog/data/bands.json`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/data/cb_channels.json` & `dragonlog-1.3/dragonlog/data/cb_channels.json`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/data/color_map.json` & `dragonlog-1.3/dragonlog/data/color_map.json`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/data/i18n/DragonLog_de.qm` & `dragonlog-1.3/dragonlog/data/i18n/DragonLog_de.qm`

 * *Files 6% similar despite different names*

```diff
@@ -1,1627 +1,1645 @@
 00000000: 3cb8 6418 caef 9c95 cd21 1cbf 60a1 bddd  <.d......!..`...
-00000010: a700 0000 0564 655f 4445 4200 000a a800  .....de_DEB.....
+00000010: a700 0000 0564 655f 4445 4200 000a c800  .....de_DEB.....
 00000020: 0000 3c00 0001 5c00 0000 3e00 0001 7800  ..<...\...>...x.
-00000030: 0000 4d00 0058 f300 0000 4e00 0059 2d00  ..M..X....N..Y-.
-00000040: 0000 5200 0059 5f00 0000 5900 0059 9b00  ..R..Y_...Y..Y..
-00000050: 0002 5700 0038 c800 0003 8900 0039 0600  ..W..8.......9..
-00000060: 0005 5b00 0023 f300 000c d000 0011 a600  ..[..#..........
-00000070: 0031 0e00 0000 0000 0047 6400 0001 fe00  .1.......Gd.....
-00000080: 004c 4400 0042 4c00 0052 8400 0007 8c00  .LD..BL..R......
-00000090: 0053 5e00 0008 e900 0055 6700 0046 cf00  .S^......Ug..F..
-000000a0: 0056 7c00 0048 d700 0056 7f00 0026 b000  .V|..H...V...&..
-000000b0: 0056 8800 000a c700 0056 8800 0027 5800  .V.......V...'X.
-000000c0: 0056 8800 004b 2900 0058 f700 000b 4300  .V...K)..X....C.
-000000d0: 026f fa00 0038 e600 0345 3000 0000 3f00  .o...8...E0...?.
-000000e0: 0357 3000 0000 bf00 037b 3000 0000 fe00  .W0......{0.....
-000000f0: 03c9 3000 0001 3d00 0488 4400 0015 4e00  ..0...=...D...N.
-00000100: 0488 4400 0031 2000 0488 4400 003c 5200  ..D..1 ...D..<R.
-00000110: 04a8 a100 0040 f400 04bb 0400 0033 9700  .....@.......3..
-00000120: 04cf 0400 0033 ce00 04d0 2500 0034 6800  .....3....%..4h.
-00000130: 04d6 8d00 0030 2c00 04e7 1000 001e 7700  .....0,.......w.
-00000140: 04ec 3000 001e 4b00 04ec 3000 0034 ba00  ..0...K...0..4..
-00000150: 0534 9700 0008 0f00 0534 9700 0043 c100  .4.......4...C..
-00000160: 0545 a500 0023 1500 0545 a500 0035 9100  .E...#...E...5..
-00000170: 0545 a500 0045 ec00 0548 3500 0009 1100  .E...E...H5.....
-00000180: 0548 3500 0023 3700 0548 3500 0046 0c00  .H5..#7..H5..F..
-00000190: 0596 7c00 000e 8d00 0598 c500 004c 4900  ..|..........LI.
-000001a0: 05ab 6000 0057 4200 06a6 7c00 0011 8700  ..`..WB...|.....
-000001b0: 06a6 7c00 0051 dc00 06fb 2100 0045 b300  ..|..Q....!..E..
-000001c0: 0714 3e00 0052 8000 144b 9e00 000d fa00  ..>..R...K......
-000001d0: 144e e600 0021 6d00 3477 3000 0000 7f00  .N...!m.4w0.....
-000001e0: 34c5 3000 0000 9f00 36b7 3000 0000 de00  4.0.....6.0.....
-000001f0: 376f f400 004f b500 38a9 3000 0001 1d00  7o...O..8.0.....
-00000200: 4796 c400 0013 b400 4796 c400 0030 7700  G.......G....0w.
-00000210: 47ab 7600 002f c900 47ab 7600 0057 d100  G.v../..G.v..W..
-00000220: 4a2b 8200 003f cb00 4c99 6200 001b fe00  J+...?..L.b.....
-00000230: 4c99 6200 0042 7300 5278 bc00 0030 5100  L.b..Bs.Rx...0Q.
-00000240: 52cc bc00 0007 b600 556a c300 0023 c200  R.......Uj...#..
-00000250: 567e 8100 0048 b600 56ae c200 0059 f400  V~...H..V....Y..
-00000260: 576d c200 0025 2200 576d c200 0048 4000  Wm...%".Wm...H@.
-00000270: 587a ff00 000a e500 587a ff00 0027 e700  Xz......Xz...'..
-00000280: 5aa8 9400 000e 4b00 5aa8 9400 004d cc00  Z.....K.Z....M..
-00000290: 5aa8 9400 0056 dd00 67ab 0600 0057 a500  Z....V..g....W..
-000002a0: 6d92 9400 0055 4600 753c 2300 0047 ff00  m....UF.u<#..G..
-000002b0: 8cd2 1500 0010 7700 aa80 2500 001a bd00  ......w...%.....
-000002c0: ab01 d300 0007 e000 ab72 4500 000a 0400  .........rE.....
-000002d0: bf5b b400 0005 fd00 c656 de00 0040 5300  .[.......V...@S.
-000002e0: ff2c 7700 001c 8601 30ed a300 001d 1d01  .,w.....0.......
-000002f0: 48c4 ff00 001a f701 4d8a bc00 0021 e201  H.......M....!..
-00000300: 5478 6c00 0022 7801 945e f800 002a 0701  Txl.."x..^...*..
-00000310: 9942 b500 0046 2c01 9ce8 5e00 004e 9501  .B...F,...^..N..
-00000320: e578 e300 000d 8b01 e907 4500 0046 7c01  .x........E..F|.
-00000330: fdeb 5400 0051 fc02 3222 f900 003b ad02  ..T..Q..2"...;..
-00000340: 33a9 3400 0009 3002 ac2b 0200 0045 2002  3.4...0..+...E .
-00000350: e7d6 5e00 0002 4102 e7d6 5e00 0015 c002  ..^...A...^.....
-00000360: e7d6 5e00 003c db02 e81d 2400 0041 9d03  ..^..<....$..A..
-00000370: 004d 1200 000c 9203 0149 e600 0021 9a03  .M.......I...!..
-00000380: 0cac 0500 0010 0103 0f6b 1200 0047 7e03  .........k...G~.
-00000390: 0f6b 3200 0024 1303 1bec 1200 0014 1303  .k2..$..........
-000003a0: 4485 3000 0000 1e03 45b3 3000 0000 5e03  D.0.....E.0...^.
-000003b0: 4ecb 9200 0037 2603 4ecb 9200 0056 ff03  N....7&.N....V..
-000003c0: 533f be00 005a 1d03 598b 3200 0008 2e03  S?...Z..Y.2.....
-000003d0: 598b 3200 0021 4803 598b 3200 0044 6703  Y.2..!H.Y.2..Dg.
-000003e0: 5d96 0b00 0044 8a03 6cc3 0400 000b fc03  ]....D..l.......
-000003f0: 881f d400 0006 2603 9ce3 f400 001e 9903  ......&.........
-00000400: 9ce9 a500 0025 9403 f5e0 0700 002e a904  .....%..........
-00000410: 07f6 ee00 0024 d304 07f6 ee00 0047 3104  .....$.......G1.
-00000420: 2b4e 0500 001d c604 6c90 3200 0044 ad04  +N......l.2..D..
-00000430: 8c96 8100 0014 9404 8caf 6200 0014 de04  ..........b.....
-00000440: 9c8b 8500 003c 7204 a472 8400 002c 1b04  .....<r..r...,..
-00000450: ab8e f500 0031 d204 ab8e f600 0031 f704  .....1.......1..
-00000460: ab8e fc00 0032 1c04 ab8f 0100 0032 4104  .....2.......2A.
-00000470: ab8f 0700 0032 6604 ab8f 0800 0032 8b04  .....2f......2..
-00000480: b08b a400 0041 2a04 b2b6 6400 0008 a204  .....A*...d.....
-00000490: c4a9 a900 0013 7b04 cf76 9400 0004 9404  ......{..v......
-000004a0: cf76 9400 0033 ff04 d03a c200 0034 9504  .v...3...:...4..
-000004b0: e826 8800 001e 0304 e826 8800 0043 2404  .&.......&...C$.
-000004c0: e842 f200 001e 2704 e842 f200 0055 bc04  .B....'..B...U..
-000004d0: edd3 6400 0039 aa04 f5b6 e700 002b 0b05  ..d..9.......+..
-000004e0: 0476 9400 0034 e705 1f06 1500 0056 1605  .v...4.......V..
-000004f0: 3268 c400 0004 1805 34db 8200 0022 3005  2h......4...."0.
-00000500: 3ddf a300 000b 0505 3fd1 b400 004d 2305  =.......?....M#.
-00000510: 40b8 b400 004c 0a05 4466 8200 004c cb05  @....L..Df...L..
-00000520: 5776 4500 0049 4505 6336 9e00 0035 5005  WvE..IE.c6...5P.
-00000530: 647d 0e00 0031 7e05 684d 7400 0028 b305  d}...1~.hMt..(..
-00000540: 684f 7400 002e 4705 7865 9800 004b 4805  hOt...G.xe...KH.
-00000550: 7865 b800 004b 6a05 87b0 6300 0055 df05  xe...Kj...c..U..
-00000560: 8ed0 0500 0058 8805 ac50 0300 0053 2d05  .....X...P...S-.
-00000570: c7f7 2800 005a 8105 c984 e900 0033 2206  ..(..Z.......3".
-00000580: 011e c400 0002 9c06 778d 0800 0006 d506  ........w.......
-00000590: 778d 0800 001f 7b06 7e7c a100 0026 7d06  w.....{.~|...&}.
-000005a0: 7e7c a100 004a 0b06 830d be00 002a c506  ~|...J.......*..
-000005b0: 97cc 5200 0036 8b06 bdf0 a400 0019 e906  ..R..6..........
-000005c0: be94 d200 0057 6306 d2af d900 005a ab06  .....Wc......Z..
-000005d0: db4d 4200 0028 4c06 e056 d800 0024 9806  .MB..(L..V...$..
-000005e0: e056 d800 0046 f806 f895 8e00 0016 2a07  .V...F........*.
-000005f0: 2f4a 1500 004e 3307 366b 9300 0005 1a07  /J...N3.6k......
-00000600: 50be 3900 0058 0307 68f8 4400 0052 a807  P.9..X..h.D..R..
-00000610: 693d fe00 0034 2407 6941 4e00 0035 0c07  i=...4$.iAN..5..
-00000620: 6cbb 6300 000e ac07 7f18 a400 004f e907  l.c..........O..
-00000630: 86be 4800 003a 2907 8f3a 3e00 0025 5507  ..H..:)..:>..%U.
-00000640: 8f3a 3e00 0048 7107 e67a d700 0033 6f07  .:>..Hq..z...3o.
-00000650: e76d c800 0025 d707 e78f a400 0026 0d07  .m...%.......&..
-00000660: e79f 3400 0026 4507 e79f 3400 0049 cf07  ..4..&E...4..I..
-00000670: e7e0 a400 002f 5307 e7f2 3400 002f 8e07  ...../S...4../..
-00000680: e7f2 3400 0052 4108 14d3 ed00 0035 b408  ..4..RA......5..
-00000690: 14d3 ed00 004a 3c08 3292 cb00 0002 7908  .....J<.2.....y.
-000006a0: 339b 4e00 0031 4308 3587 6a00 002c 7a08  3.N..1C.5.j..,z.
-000006b0: 36b6 5400 0012 bf08 5ac5 0100 0001 9408  6.T.....Z.......
-000006c0: 5ac5 0100 0014 6108 678f b400 0027 7908  Z.....a.g....'y.
-000006d0: 679f 2400 0027 b108 679f 2400 004b ce08  g.$..'..g.$..K..
-000006e0: 7f52 2500 002b ba08 8879 1400 0019 7b08  .R%..+...y....{.
-000006f0: aae3 e400 0009 d108 b63d de00 0038 1408  .........=...8..
-00000700: bd74 5e00 0023 5908 d39b 6400 0043 e108  .t^..#Y...d..C..
-00000710: f89a cb00 0039 2409 14be 9200 004d 6009  .....9$......M`.
-00000720: 1c52 9500 002f 0809 238c 7500 0017 2709  .R.../..#.u...'.
-00000730: 3f8c ad00 000d 0f09 564e 4200 0050 2109  ?.......VNB..P!.
-00000740: 6c61 f400 0013 df09 6c61 f400 0030 a309  la......la...0..
-00000750: 6fe6 7e00 0011 c309 8fa3 8700 0030 d809  o.~..........0..
-00000760: 97c9 1400 0021 0d09 97c9 1400 0044 2609  .....!.......D&.
-00000770: 97d9 8400 0020 d209 9c7f 1a00 003a c609  ..... .......:..
-00000780: a118 8500 0011 4209 a6a8 f100 0028 f209  ......B......(..
-00000790: c004 d700 0003 df09 c4e8 d700 0001 c409  ................
-000007a0: c8df a200 001e ee09 c943 f500 0010 3c09  .........C....<.
-000007b0: c9cf c500 000c 6409 df31 3800 004a b909  ......d..18..J..
-000007c0: e854 fc00 0015 fb09 e854 fc00 003e 3d09  .T.......T...>=.
-000007d0: f42c fb00 001b d80a 16bb 3400 004a 780a  .,........4..Jx.
-000007e0: 2087 bc00 003f 1b0a 2190 e200 0006 8c0a   ....?..!.......
-000007f0: 2190 e200 001f 2f0a 3f0e 9500 0029 be0a  !...../.?....)..
-00000800: 5e68 d900 0026 d10a 643c 1400 0016 f00a  ^h...&..d<......
-00000810: 65ac e400 0017 cc0a 65ac e400 0040 ab0a  e.......e....@..
-00000820: 6789 3b00 0007 140a 6789 3b00 001f bd0a  g.;.....g.;.....
-00000830: 67a9 0200 0007 500a 67a9 0200 001f fc0a  g.....P.g.......
-00000840: 6dc8 3e00 0037 ad0a 7693 dd00 0032 b00a  m.>..7..v....2..
-00000850: 7833 e400 003c 9c0a 7d6b 2400 0018 af0a  x3...<..}k$.....
-00000860: 8a77 ef00 0032 ea0a 92a2 e500 002a 710a  .w...2.......*q.
-00000870: 9612 e500 0029 640a a8b0 0e00 000e 6b0a  .....)d.......k.
-00000880: a8b0 0e00 004d ed0a acdb 7e00 0002 1c0a  .....M....~.....
-00000890: b945 f500 002b f60a b945 f500 004e 100a  .E...+...E...N..
-000008a0: c389 2500 0029 2d0a c5b4 4900 0043 460a  ..%..)-...I..CF.
-000008b0: c897 c500 0006 4e0a cec2 8400 0040 ce0a  ......N......@..
-000008c0: d2f0 b500 0003 090a d382 7700 0003 570a  ..........w...W.
-000008d0: e2b5 9600 0004 b50a f31c 2200 003e a70b  .........."..>..
-000008e0: 1562 0700 0053 620b 1805 3900 0015 700b  .b...Sb...9...p.
-000008f0: 4597 5500 0008 500b 5d8a f400 0020 3b0b  E.U...P.].... ;.
-00000900: 6628 d200 0037 6b0b 7fe2 de00 0035 f30b  f(...7k......5..
-00000910: ad17 7800 001b aa0b ff25 ce00 001c d80c  ..x......%......
-00000920: 08f5 6c00 0041 580c 107d 9300 0003 a10c  ..l..AX..}......
-00000930: 10ba b200 0028 0a0c 1536 f700 002d ed0c  .....(...6...-..
-00000940: 1f2f 0200 0050 720c 242f 6400 0038 8b0c  ./...Pr.$/d..8..
-00000950: 29f2 a400 0053 070c 6a19 e900 0040 040c  )....S..j....@..
-00000960: 8c09 2900 001d 8f0c 8c09 2900 0042 ef0c  ..).......)..B..
-00000970: 9688 9500 0014 b80c a3fa 5f00 001a 7f0c  .........._.....
-00000980: a6e8 d400 003d 810c bb01 7300 000c d20c  .....=....s.....
-00000990: bb01 7300 0036 4a0c c9a0 0e00 002e 840d  ..s..6J.........
-000009a0: 0218 6400 004c 7b0d 07a4 f800 003e 6a0d  ..d..L{......>j.
-000009b0: 1f27 b200 0015 0c0d 3504 b400 003d dd0d  .'......5....=..
-000009c0: 76f7 5900 001c 2d0d 825f 7300 000f 4f0d  v.Y...-.._s...O.
-000009d0: a03c 1200 0054 340d d0ff 4c00 002d a10d  .<...T4...L..-..
-000009e0: f2ea c200 003f 610d fe4e 2400 001a 320d  .....?a..N$...2.
-000009f0: fe4e 2400 0054 fa0e 0543 5500 0024 5a0e  .N$..T...CU..$Z.
-00000a00: 05d1 b500 0054 930e 0743 5500 0047 c30e  .....T...CU..G..
-00000a10: 0906 8800 003b 000e 233d d500 0050 b80e  .....;..#=...P..
-00000a20: 87ac 6400 0020 840e 93fa 5200 0017 f10e  ..d.. ....R.....
-00000a30: a32f e400 0042 a00e c47b 9900 002f fc0e  ./...B...{.../..
-00000a40: c497 a200 000b 730e c72a a600 0005 880e  ......s..*......
-00000a50: de3d a200 003d 140e e46b 3400 004b 8c0e  .=...=...k4..K..
-00000a60: fdeb 3400 0049 8d0f 165e c400 0048 f60f  ..4..I...^...H..
-00000a70: 3562 ce00 0018 520f 6963 bc00 000d 540f  5b....R.ic....T.
-00000a80: 6963 bc00 002b 800f 6963 bc00 0056 a40f  ic...+..ic...V..
-00000a90: 6978 c700 0036 d90f 6c98 6c00 0059 c90f  ix...6..l.l..Y..
-00000aa0: 7ddd 2800 0051 600f 8007 d400 003b ec0f  }.(..Q`......;..
-00000ab0: 8313 8900 0013 480f cb15 5200 0019 310f  ......H...R...1.
-00000ac0: e6f6 3400 0043 6e69 0000 5ad5 03ff ffff  ..4..Cni..Z.....
-00000ad0: ff08 0000 0000 0600 0000 032e 2e2e 0700  ................
-00000ae0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-00000af0: 0000 0000 0600 0000 0631 3135 3230 3007  .........115200.
-00000b00: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
-00000b10: 0800 0000 0006 0000 0004 3132 3030 0700  ..........1200..
-00000b20: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-00000b30: 0000 0000 0600 0000 0631 3238 3030 3007  .........128000.
-00000b40: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
-00000b50: 0800 0000 0006 0000 0005 3134 3430 3007  ..........14400.
+00000030: 0000 4d00 0059 f800 0000 4e00 005a 3200  ..M..Y....N..Z2.
+00000040: 0000 5200 005a 6400 0000 5900 005a a000  ..R..Zd...Y..Z..
+00000050: 0002 5700 0038 2300 0003 8900 0038 6100  ..W..8#......8a.
+00000060: 0005 5b00 0023 2900 0031 0e00 0000 0000  ..[..#)..1......
+00000070: 0047 6400 0001 fe00 004c 4400 0042 d100  .Gd......LD..B..
+00000080: 0055 6700 0047 5400 0056 7c00 0048 de00  .Ug..GT..V|..H..
+00000090: 0056 7f00 0025 e600 0056 8800 0026 8e00  .V...%...V...&..
+000000a0: 0056 8800 004b 3000 0058 f700 000a d900  .V...K0..X......
+000000b0: 026f fa00 0038 4100 0345 3000 0000 3f00  .o...8A..E0...?.
+000000c0: 0357 3000 0000 bf00 037b 3000 0000 fe00  .W0......{0.....
+000000d0: 03c9 3000 0001 3d00 0488 4400 0014 8700  ..0...=...D.....
+000000e0: 0488 4400 0030 5600 0488 4400 003b ad00  ..D..0V...D..;..
+000000f0: 04a8 a100 0041 7900 04bb 0400 0032 f200  .....Ay......2..
+00000100: 04cf 0400 0033 2900 04d0 2500 0033 c300  .....3)...%..3..
+00000110: 04d6 8d00 002f 6200 04e7 1000 001d b000  ...../b.........
+00000120: 04ec 3000 001d 8400 04ec 3000 0034 1500  ..0.......0..4..
+00000130: 0534 9700 0007 e500 0534 9700 0044 4600  .4.......4...DF.
+00000140: 0545 a500 0022 4b00 0545 a500 0034 ec00  .E..."K..E...4..
+00000150: 0545 a500 0046 7100 0548 3500 0008 9d00  .E...Fq..H5.....
+00000160: 0548 3500 0022 6d00 0548 3500 0046 9100  .H5.."m..H5..F..
+00000170: 0596 7c00 000d e300 0598 c500 004c 5000  ..|..........LP.
+00000180: 05ab 6000 0057 8b00 06a6 7c00 0010 dd00  ..`..W....|.....
+00000190: 06a6 7c00 0051 e300 06fb 2100 0046 3800  ..|..Q....!..F8.
+000001a0: 0714 3e00 0052 8700 144b 9e00 000d 5000  ..>..R...K....P.
+000001b0: 144e e600 0020 a600 15e7 b800 0021 1b00  .N... .......!..
+000001c0: 3477 3000 0000 7f00 34c5 3000 0000 9f00  4w0.....4.0.....
+000001d0: 36b7 3000 0000 de00 376f f400 004f bc00  6.0.....7o...O..
+000001e0: 38a9 3000 0001 1d00 4796 c400 0012 ed00  8.0.....G.......
+000001f0: 4796 c400 002f ad00 47ab 7600 002e ff00  G..../..G.v.....
+00000200: 47ab 7600 0058 d600 4a2b 8200 003f 2600  G.v..X..J+...?&.
+00000210: 4c99 6200 001b 3700 4c99 6200 0042 f800  L.b...7.L.b..B..
+00000220: 5278 bc00 002f 8700 52cc bc00 0007 8c00  Rx.../..R.......
+00000230: 556a c300 0022 f800 567e 8100 0048 bd00  Uj..."..V~...H..
+00000240: 56ae c200 005a f900 576d c200 0024 5800  V....Z..Wm...$X.
+00000250: 576d c200 0048 4700 587a ff00 000a 7b00  Wm...HG.Xz....{.
+00000260: 587a ff00 0027 1d00 5aa8 9400 000d a100  Xz...'..Z.......
+00000270: 5aa8 9400 004d d300 5aa8 9400 0057 2600  Z....M..Z....W&.
+00000280: 67ab 0600 0058 aa00 6d92 9400 0055 4d00  g....X..m....UM.
+00000290: 753c 2300 0048 0600 8cd2 1500 000f cd00  u<#..H..........
+000002a0: aa80 2500 0019 f600 ab01 d300 0007 b600  ..%.............
+000002b0: ab72 4500 0009 9000 bf5b b400 0005 fd00  .rE......[......
+000002c0: c656 de00 003f ae00 ff2c 7700 001b bf01  .V...?...,w.....
+000002d0: 30ed a300 001c 5601 48c4 ff00 001a 3001  0.....V.H.....0.
+000002e0: 5478 6c00 0021 ae01 945e f800 0029 3d01  Txl..!...^...)=.
+000002f0: 9942 b500 0046 b101 9ce8 5e00 004e 9c01  .B...F....^..N..
+00000300: e578 e300 000c e101 e907 4500 0047 0101  .x........E..G..
+00000310: fdeb 5400 0052 0302 3222 f900 003b 0802  ..T..R..2"...;..
+00000320: 33a9 3400 0008 bc02 ac2b 0200 0045 a502  3.4......+...E..
+00000330: e7d6 5e00 0002 4102 e7d6 5e00 0014 f902  ..^...A...^.....
+00000340: e7d6 5e00 003c 3602 e81d 2400 0042 2203  ..^..<6...$..B".
+00000350: 0149 e600 0020 d303 0cac 0500 000f 5703  .I... ........W.
+00000360: 0f6b 3200 0023 4903 129b c900 000a 5303  .k2..#I.......S.
+00000370: 1bec 1200 0013 4c03 4485 3000 0000 1e03  ......L.D.0.....
+00000380: 45b3 3000 0000 5e03 4ecb 9200 0036 8103  E.0...^.N....6..
+00000390: 4ecb 9200 0057 4803 533f be00 005b 2203  N....WH.S?...[".
+000003a0: 598b 3200 0020 8103 598b 3200 0044 ec03  Y.2.. ..Y.2..D..
+000003b0: 5d96 0b00 0045 0f03 6cc3 0400 000b 9203  ]....E..l.......
+000003c0: 881f d400 0006 2603 9ce3 f400 001d d203  ......&.........
+000003d0: 9ce9 a500 0024 ca03 f5e0 0700 002d df04  .....$.......-..
+000003e0: 07f6 ee00 0024 0904 07f6 ee00 0047 7d04  .....$.......G}.
+000003f0: 2b4e 0500 001c ff04 6c90 3200 0045 3204  +N......l.2..E2.
+00000400: 8c96 8100 0013 cd04 8caf 6200 0014 1704  ..........b.....
+00000410: 9c8b 8500 003b cd04 a472 8400 002b 5104  .....;...r...+Q.
+00000420: ab8e f500 0031 0804 ab8e f600 0031 2d04  .....1.......1-.
+00000430: ab8e fc00 0031 5204 ab8f 0100 0031 7704  .....1R......1w.
+00000440: ab8f 0200 0031 9c04 ab8f 0300 0041 0d04  .....1.......A..
+00000450: ab8f 0500 0041 5704 ab8f 0700 0031 c104  .....AW......1..
+00000460: ab8f 0800 0031 e604 b08b a400 0041 af04  .....1.......A..
+00000470: b2b6 6400 0008 5604 c4a9 a900 0012 b404  ..d...V.........
+00000480: cf76 9400 0004 9404 cf76 9400 0033 5a04  .v.......v...3Z.
+00000490: d03a c200 0033 f004 e826 8800 001d 3c04  .:...3...&....<.
+000004a0: e826 8800 0043 a904 e842 f200 001d 6004  .&...C...B....`.
+000004b0: e842 f200 0055 c304 edd3 6400 0039 0504  .B...U....d..9..
+000004c0: f5b6 e700 002a 4105 0476 9400 0034 4205  .....*A..v...4B.
+000004d0: 1f06 1500 0056 5f05 3268 c400 0004 1805  .....V_.2h......
+000004e0: 34db 8200 0021 6605 3ddf a300 000a 9b05  4....!f.=.......
+000004f0: 3fd1 b400 004d 2a05 40b8 b400 004c 1105  ?....M*.@....L..
+00000500: 4466 8200 004c d205 5776 4500 0049 4c05  Df...L..WvE..IL.
+00000510: 6336 9e00 0034 ab05 647d 0e00 0030 b405  c6...4..d}...0..
+00000520: 684d 7400 0027 e905 684f 7400 002d 7d05  hMt..'..hOt..-}.
+00000530: 7865 9800 004b 4f05 7865 b800 004b 7105  xe...KO.xe...Kq.
+00000540: 87b0 6300 0056 2805 8ed0 0500 0059 8d05  ..c..V(......Y..
+00000550: ac50 0300 0053 3405 c7f7 2800 005b 8605  .P...S4...(..[..
+00000560: c984 e900 0032 7d06 011e c400 0002 9c06  .....2}.........
+00000570: 778d 0800 0006 d506 778d 0800 001e b406  w.......w.......
+00000580: 7e7c a100 0025 b306 7e7c a100 004a 1206  ~|...%..~|...J..
+00000590: 830d be00 0029 fb06 97cc 5200 0035 e606  .....)....R..5..
+000005a0: bdf0 a400 0019 2206 be94 d200 0057 ac06  ......"......W..
+000005b0: d2af d900 005b b006 db4d 4200 0027 8206  .....[...MB..'..
+000005c0: e056 d800 0023 ce06 f895 8e00 0015 6307  .V...#........c.
+000005d0: 2f4a 1500 004e 3a07 366b 9300 0005 1a07  /J...N:.6k......
+000005e0: 50be 3900 0059 0807 68f8 4400 0052 af07  P.9..Y..h.D..R..
+000005f0: 693d fe00 0033 7f07 6941 4e00 0034 6707  i=...3..iAN..4g.
+00000600: 6cbb 6300 000e 0207 7f18 a400 004f f007  l.c..........O..
+00000610: 86be 4800 0039 8407 8f3a 3e00 0024 8b07  ..H..9...:>..$..
+00000620: 8f3a 3e00 0048 7807 e67a d700 0032 ca07  .:>..Hx..z...2..
+00000630: e76d c800 0025 0d07 e78f a400 0025 4307  .m...%.......%C.
+00000640: e79f 3400 0025 7b07 e79f 3400 0049 d607  ..4..%{...4..I..
+00000650: e7e0 a400 002e 8907 e7f2 3400 002e c407  ..........4.....
+00000660: e7f2 3400 0052 4808 14d3 ed00 0035 0f08  ..4..RH......5..
+00000670: 14d3 ed00 004a 4308 3292 cb00 0002 7908  .....JC.2.....y.
+00000680: 339b 4e00 0030 7908 3587 6a00 002b b008  3.N..0y.5.j..+..
+00000690: 36b6 5400 0011 f808 5ac5 0100 0001 9408  6.T.....Z.......
+000006a0: 5ac5 0100 0013 9a08 678f b400 0026 af08  Z.......g....&..
+000006b0: 679f 2400 0026 e708 679f 2400 004b d508  g.$..&..g.$..K..
+000006c0: 7f52 2500 002a f008 8879 1400 0018 b408  .R%..*...y......
+000006d0: aae3 e400 0009 5d08 b63d de00 0037 6f08  ......]..=...7o.
+000006e0: bd74 5e00 0022 8f08 d39b 6400 0044 6608  .t^.."....d..Df.
+000006f0: f89a cb00 0038 7f09 14be 9200 004d 6709  .....8.......Mg.
+00000700: 1c52 9500 002e 3e09 238c 7500 0016 6009  .R....>.#.u...`.
+00000710: 3f8c ad00 000c 6509 564e 4200 0050 2809  ?.....e.VNB..P(.
+00000720: 6c61 f400 0013 1809 6c61 f400 002f d909  la......la.../..
+00000730: 6fe6 7e00 0010 fc09 8fa3 8700 0030 0e09  o.~..........0..
+00000740: 97c9 1400 0020 4609 97c9 1400 0044 ab09  ..... F......D..
+00000750: 97d9 8400 0020 0b09 9c7f 1a00 003a 2109  ..... .......:!.
+00000760: a118 8500 0010 9809 a6a8 f100 0028 2809  .............((.
+00000770: c004 d700 0003 df09 c4e8 d700 0001 c409  ................
+00000780: c8df a200 001e 2709 c943 f500 000f 9209  ......'..C......
+00000790: c9cf c500 000b fa09 df31 3800 004a c009  .........18..J..
+000007a0: e854 fc00 0015 3409 e854 fc00 003d 9809  .T....4..T...=..
+000007b0: f42c fb00 001b 110a 16bb 3400 004a 7f0a  .,........4..J..
+000007c0: 2087 bc00 003e 760a 2190 e200 0006 8c0a   ....>v.!.......
+000007d0: 2190 e200 001e 680a 3f0e 9500 0028 f40a  !.....h.?....(..
+000007e0: 5e68 d900 0026 070a 643c 1400 0016 290a  ^h...&..d<....).
+000007f0: 65ac e400 0017 050a 65ac e400 0040 060a  e.......e....@..
+00000800: 6789 3b00 0007 140a 6789 3b00 001e f60a  g.;.....g.;.....
+00000810: 67a9 0200 0007 500a 67a9 0200 001f 350a  g.....P.g.....5.
+00000820: 6dc8 3e00 0037 080a 7693 dd00 0032 0b0a  m.>..7..v....2..
+00000830: 7833 e400 003b f70a 7d6b 2400 0017 e80a  x3...;..}k$.....
+00000840: 8a77 ef00 0032 450a 92a2 e500 0029 a70a  .w...2E......)..
+00000850: 9612 e500 0028 9a0a a8b0 0e00 000d c10a  .....(..........
+00000860: a8b0 0e00 004d f40a acdb 7e00 0002 1c0a  .....M....~.....
+00000870: b945 f500 002b 2c0a b945 f500 004e 170a  .E...+,..E...N..
+00000880: c389 2500 0028 630a c5b4 4900 0043 cb0a  ..%..(c...I..C..
+00000890: c897 c500 0006 4e0a ca87 2300 0055 e60a  ......N...#..U..
+000008a0: cec2 8400 0040 290a d2f0 b500 0003 090a  .....@).........
+000008b0: d382 7700 0003 570a e2b5 9600 0004 b50a  ..w...W.........
+000008c0: f31c 2200 003e 020b 1562 0700 0053 690b  .."..>...b...Si.
+000008d0: 1805 3900 0014 a90b 4597 5500 0008 040b  ..9.....E.U.....
+000008e0: 5d8a f400 001f 740b 6628 d200 0036 c60b  ].....t.f(...6..
+000008f0: 7fe2 de00 0035 4e0b ad17 7800 001a e30b  .....5N...x.....
+00000900: ff25 ce00 001c 110c 08f5 6c00 0041 dd0c  .%........l..A..
+00000910: 107d 9300 0003 a10c 10ba b200 0027 400c  .}...........'@.
+00000920: 1536 f700 002d 230c 1f2f 0200 0050 790c  .6...-#../...Py.
+00000930: 242f 6400 0037 e60c 29f2 a400 0053 0e0c  $/d..7..)....S..
+00000940: 6a19 e900 003f 5f0c 8c09 2900 001c c80c  j....?_...).....
+00000950: 8c09 2900 0043 740c 9688 9500 0013 f10c  ..)..Ct.........
+00000960: a3fa 5f00 0019 b80c a6e8 d400 003c dc0c  .._..........<..
+00000970: bb01 7300 000c 280c bb01 7300 0035 a50c  ..s...(...s..5..
+00000980: c9a0 0e00 002d ba0d 0218 6400 004c 820d  .....-....d..L..
+00000990: 03e6 7200 0057 ee0d 07a4 f800 003d c50d  ..r..W.......=..
+000009a0: 1f27 b200 0014 450d 3504 b400 003d 380d  .'....E.5....=8.
+000009b0: 4459 f500 0041 2f0d 76f7 5900 001b 660d  DY...A/.v.Y...f.
+000009c0: 825f 7300 000e a50d a03c 1200 0054 3b0d  ._s......<...T;.
+000009d0: d0ff 4c00 002c d70d f2ea c200 003e bc0d  ..L..,.......>..
+000009e0: fe4e 2400 0019 6b0d fe4e 2400 0055 010e  .N$...k..N$..U..
+000009f0: 0543 5500 0023 900e 05d1 b500 0054 9a0e  .CU..#.......T..
+00000a00: 0743 5500 0047 ca0e 0906 8800 003a 5b0e  .CU..G.......:[.
+00000a10: 233d d500 0050 bf0e 87ac 6400 001f bd0e  #=...P....d.....
+00000a20: 93fa 5200 0017 2a0e a32f e400 0043 250e  ..R...*../...C%.
+00000a30: c47b 9900 002f 320e c497 a200 000b 090e  .{.../2.........
+00000a40: c72a a600 0005 880e de3d a200 003c 6f0e  .*.......=...<o.
+00000a50: e46b 3400 004b 930e f49d 7500 0040 4f0e  .k4..K....u..@O.
+00000a60: f49d 7800 0040 750e f49d 7900 0040 9b0e  ..x..@u...y..@..
+00000a70: f49d 7e00 0040 c10e f49e 8a00 0040 e70e  ..~..@.......@..
+00000a80: fdeb 3400 0049 940f 165e c400 0048 fd0f  ..4..I...^...H..
+00000a90: 3562 ce00 0017 8b0f 6963 bc00 000c aa0f  5b......ic......
+00000aa0: 6963 bc00 002a b60f 6963 bc00 0056 ed0f  ic...*..ic...V..
+00000ab0: 6978 c700 0036 340f 6c98 6c00 005a ce0f  ix...64.l.l..Z..
+00000ac0: 7ddd 2800 0051 670f 8007 d400 003b 470f  }.(..Qg......;G.
+00000ad0: 8313 8900 0012 810f cb15 5200 0018 6a0f  ..........R...j.
+00000ae0: e6f6 3400 0043 f369 0000 5bda 03ff ffff  ..4..C.i..[.....
+00000af0: ff08 0000 0000 0600 0000 032e 2e2e 0700  ................
+00000b00: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
+00000b10: 0000 0000 0600 0000 0631 3135 3230 3007  .........115200.
+00000b20: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
+00000b30: 0800 0000 0006 0000 0004 3132 3030 0700  ..........1200..
+00000b40: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
+00000b50: 0000 0000 0600 0000 0631 3238 3030 3007  .........128000.
 00000b60: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
-00000b70: 0800 0000 0006 0000 0005 3139 3230 3007  ..........19200.
+00000b70: 0800 0000 0006 0000 0005 3134 3430 3007  ..........14400.
 00000b80: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
-00000b90: 0800 0000 0006 0000 0004 3234 3030 0700  ..........2400..
-00000ba0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-00000bb0: 0000 0000 0600 0000 0533 3834 3030 0700  .........38400..
+00000b90: 0800 0000 0006 0000 0005 3139 3230 3007  ..........19200.
+00000ba0: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
+00000bb0: 0800 0000 0006 0000 0004 3234 3030 0700  ..........2400..
 00000bc0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-00000bd0: 0000 0000 0600 0000 0434 3830 3007 0000  .........4800...
-00000be0: 0006 4469 616c 6f67 0103 ffff ffff 0800  ..Dialog........
-00000bf0: 0000 0006 0000 0005 3537 3630 3007 0000  ........57600...
+00000bd0: 0000 0000 0600 0000 0533 3834 3030 0700  .........38400..
+00000be0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
+00000bf0: 0000 0000 0600 0000 0434 3830 3007 0000  .........4800...
 00000c00: 0006 4469 616c 6f67 0103 ffff ffff 0800  ..Dialog........
-00000c10: 0000 0006 0000 0004 3936 3030 0700 0000  ........9600....
-00000c20: 0644 6961 6c6f 6701 03ff ffff ff08 0000  .Dialog.........
-00000c30: 0000 0600 0000 013c 0700 0000 0644 6961  .......<.....Dia
-00000c40: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
-00000c50: 0000 013e 0700 0000 0644 6961 6c6f 6701  ...>.....Dialog.
-00000c60: 0300 0000 0e00 4100 6e00 7400 6500 6e00  ......A.n.t.e.n.
-00000c70: 6e00 6508 0000 0000 0600 0000 0741 6e74  n.e..........Ant
-00000c80: 656e 6e61 0700 0000 0644 6961 6c6f 6701  enna.....Dialog.
-00000c90: 0300 0000 1600 4100 7500 6600 7300 7400  ......A.u.f.s.t.
-00000ca0: 6500 6900 6700 6500 6e00 6408 0000 0000  e.i.g.e.n.d.....
-00000cb0: 0600 0000 0941 7363 656e 6469 6e67 0700  .....Ascending..
-00000cc0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-00000cd0: 0000 0000 0600 0000 0343 4154 0700 0000  .........CAT....
-00000ce0: 0644 6961 6c6f 6701 03ff ffff ff08 0000  .Dialog.........
-00000cf0: 0000 0600 0000 0a43 422d 5374 6174 696f  .......CB-Statio
-00000d00: 6e07 0000 0006 4469 616c 6f67 0103 0000  n.....Dialog....
-00000d10: 0014 0052 0075 0066 007a 0065 0069 0063  ...R.u.f.z.e.i.c
-00000d20: 0068 0065 006e 0800 0000 0006 0000 0009  .h.e.n..........
-00000d30: 4361 6c6c 2073 6967 6e07 0000 0006 4469  Call sign.....Di
-00000d40: 616c 6f67 0103 ffff ffff 0800 0000 0006  alog............
-00000d50: 0000 0008 4361 6c6c 626f 6f6b 0700 0000  ....Callbook....
-00000d60: 0644 6961 6c6f 6701 0300 0000 3800 5a00  .Dialog.....8.Z.
-00000d70: 6500 7200 7400 6900 6600 6900 6b00 6100  e.r.t.i.f.i.k.a.
-00000d80: 7400 2000 6200 6500 6e00 f600 7400 6900  t. .b.e.n...t.i.
-00000d90: 6700 7400 2000 5000 6100 7300 7300 7700  g.t. .P.a.s.s.w.
-00000da0: 6f00 7200 7408 0000 0000 0600 0000 1a43  o.r.t..........C
-00000db0: 6572 7469 6669 6361 7465 206e 6565 6473  ertificate needs
-00000dc0: 2070 6173 7377 6f72 6407 0000 0006 4469   password.....Di
-00000dd0: 616c 6f67 0103 0000 0024 0053 0070 0061  alog.....$.S.p.a
-00000de0: 006c 0074 0065 006e 0020 0076 0065 0072  .l.t.e.n. .v.e.r
-00000df0: 0073 0074 0065 0063 006b 0065 006e 0800  .s.t.e.c.k.e.n..
-00000e00: 0000 0006 0000 000f 436f 6c75 6d6e 7320  ........Columns 
-00000e10: 746f 2068 6964 6507 0000 0006 4469 616c  to hide.....Dial
-00000e20: 6f67 0103 0000 0020 0053 0070 0061 006c  og..... .S.p.a.l
-00000e30: 0074 0065 006e 0020 0061 006e 007a 0065  .t.e.n. .a.n.z.e
-00000e40: 0069 0067 0065 006e 0800 0000 0006 0000  .i.g.e.n........
-00000e50: 000f 436f 6c75 6d6e 7320 746f 2073 686f  ..Columns to sho
-00000e60: 7707 0000 0006 4469 616c 6f67 0103 0000  w.....Dialog....
-00000e70: 0018 0041 006e 006d 0065 006c 0064 0065  ...A.n.m.e.l.d.e
-00000e80: 0064 0061 0074 0065 006e 0800 0000 0006  .d.a.t.e.n......
-00000e90: 0000 000b 4372 6564 656e 7469 616c 7307  ....Credentials.
-00000ea0: 0000 0006 4469 616c 6f67 0103 0000 0014  ....Dialog......
-00000eb0: 0041 0062 0073 0074 0065 0069 0067 0065  .A.b.s.t.e.i.g.e
-00000ec0: 006e 0064 0800 0000 0006 0000 000a 4465  .n.d..........De
-00000ed0: 7363 656e 6469 6e67 0700 0000 0644 6961  scending.....Dia
-00000ee0: 6c6f 6701 0300 0000 3e00 5700 6900 7200  log.....>.W.i.r.
-00000ef0: 6b00 7300 6100 6d00 2000 6e00 6100 6300  k.s.a.m. .n.a.c.
-00000f00: 6800 2000 4100 6e00 7700 6500 6e00 6400  h. .A.n.w.e.n.d.
-00000f10: 7500 6e00 6700 7300 6e00 6500 7500 7300  u.n.g.s.n.e.u.s.
-00000f20: 7400 6100 7200 7408 0000 0000 0600 0000  t.a.r.t.........
-00000f30: 2345 6666 6563 7469 7665 2061 6674 6572  #Effective after
-00000f40: 2061 7070 6c69 6361 7469 6f6e 2072 6573   application res
-00000f50: 7461 7274 0700 0000 0644 6961 6c6f 6701  tart.....Dialog.
-00000f60: 03ff ffff ff08 0000 0000 0600 0000 0645  ...............E
-00000f70: 7870 6f72 7407 0000 0006 4469 616c 6f67  xport.....Dialog
-00000f80: 0103 0000 0034 0045 0078 0070 006f 0072  .....4.E.x.p.o.r
-00000f90: 0074 0069 0065 0072 0065 0020 0043 0042  .t.i.e.r.e. .C.B
-00000fa0: 002d 0051 0053 004f 0073 0020 0069 006e  .-.Q.S.O.s. .i.n
-00000fb0: 0020 0041 0044 0049 0046 0800 0000 0006  . .A.D.I.F......
-00000fc0: 0000 0016 4578 706f 7274 2043 4220 5153  ....Export CB QS
-00000fd0: 4f73 2074 6f20 4144 4946 0700 0000 0644  Os to ADIF.....D
-00000fe0: 6961 6c6f 6701 0300 0000 3c00 4500 7800  ialog.....<.E.x.
-00000ff0: 7000 6f00 7200 7400 6900 6500 7200 6500  p.o.r.t.i.e.r.e.
-00001000: 2000 6e00 7500 7200 2000 6700 6500 6600   .n.u.r. .g.e.f.
-00001010: 6900 6c00 7400 6500 7200 7400 6500 2000  i.l.t.e.r.t.e. .
-00001020: 5100 5300 4f00 7308 0000 0000 0600 0000  Q.S.O.s.........
-00001030: 1745 7870 6f72 7420 6f6e 6c79 2072 6563  .Export only rec
-00001040: 656e 7420 5153 4f73 0700 0000 0644 6961  ent QSOs.....Dia
-00001050: 6c6f 6701 0300 0000 4200 4500 7800 7000  log.....B.E.x.p.
-00001060: 6f00 7200 7400 6900 6500 7200 6500 2000  o.r.t.i.e.r.e. .
-00001070: 6500 6900 6700 6500 6e00 6500 2000 4e00  e.i.g.e.n.e. .N.
-00001080: 6f00 7400 6900 7a00 6500 6e00 2000 6900  o.t.i.z.e.n. .i.
-00001090: 6e00 2000 4100 4400 4900 4608 0000 0000  n. .A.D.I.F.....
-000010a0: 0600 0000 1845 7870 6f72 7420 6f77 6e20  .....Export own 
-000010b0: 6e6f 7465 7320 746f 2041 4449 4607 0000  notes to ADIF...
-000010c0: 0006 4469 616c 6f67 0103 ffff ffff 0800  ..Dialog........
-000010d0: 0000 0006 0000 000e 4861 6d6c 6962 2072  ........Hamlib r
-000010e0: 6967 6374 6c64 0700 0000 0644 6961 6c6f  igctld.....Dialo
-000010f0: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
-00001100: 0d49 6d70 6f72 742f 4578 706f 7274 0700  .Import/Export..
-00001110: 0000 0644 6961 6c6f 6701 0300 0000 1a00  ...Dialog.......
-00001120: 5300 6300 6800 6e00 6900 7400 7400 7300  S.c.h.n.i.t.t.s.
-00001130: 7400 6500 6c00 6c00 6508 0000 0000 0600  t.e.l.l.e.......
-00001140: 0000 0949 6e74 6572 6661 6365 0700 0000  ...Interface....
-00001150: 0644 6961 6c6f 6701 0300 0000 2000 6c00  .Dialog..... .l.
-00001160: 6500 7400 7a00 7400 6500 7300 2000 4800  e.t.z.t.e.s. .H.
-00001170: 6100 6c00 6200 6a00 6100 6800 7208 0000  a.l.b.j.a.h.r...
-00001180: 0000 0600 0000 0e4c 6173 7420 6861 6c66  .......Last half
-00001190: 2079 6561 7207 0000 0006 4469 616c 6f67   year.....Dialog
-000011a0: 0103 0000 001a 006c 0065 0074 007a 0074  .......l.e.t.z.t
-000011b0: 0065 006e 0020 004d 006f 006e 0061 0074  .e.n. .M.o.n.a.t
-000011c0: 0800 0000 0006 0000 000a 4c61 7374 206d  ..........Last m
-000011d0: 6f6e 7468 0700 0000 0644 6961 6c6f 6701  onth.....Dialog.
-000011e0: 0300 0000 1800 6c00 6500 7400 7a00 7400  ......l.e.t.z.t.
-000011f0: 6500 2000 5700 6f00 6300 6800 6508 0000  e. .W.o.c.h.e...
-00001200: 0000 0600 0000 094c 6173 7420 7765 656b  .......Last week
-00001210: 0700 0000 0644 6961 6c6f 6701 0300 0000  .....Dialog.....
-00001220: 1800 6c00 6500 7400 7a00 7400 6500 7300  ..l.e.t.z.t.e.s.
-00001230: 2000 4a00 6100 6800 7208 0000 0000 0600   .J.a.h.r.......
-00001240: 0000 094c 6173 7420 7965 6172 0700 0000  ...Last year....
-00001250: 0644 6961 6c6f 6701 0300 0000 0c00 4200  .Dialog.......B.
-00001260: 7200 6500 6900 7400 6508 0000 0000 0600  r.e.i.t.e.......
-00001270: 0000 034c 6174 0700 0000 0644 6961 6c6f  ...Lat.....Dialo
-00001280: 6701 0300 0000 0a00 5300 7400 7500 6600  g.......S.t.u.f.
-00001290: 6508 0000 0000 0600 0000 054c 6576 656c  e..........Level
-000012a0: 0700 0000 0644 6961 6c6f 6701 0300 0000  .....Dialog.....
-000012b0: 0c00 4c00 6900 7300 7400 6500 6e08 0000  ..L.i.s.t.e.n...
-000012c0: 0000 0600 0000 084c 6973 7469 6e67 7307  .......Listings.
-000012d0: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
-000012e0: 0800 0000 0006 0000 0004 4c6f 5457 0700  ..........LoTW..
-000012f0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-00001300: 0000 0000 0600 0000 074c 6f63 6174 6f72  .........Locator
-00001310: 0700 0000 0644 6961 6c6f 6701 0300 0000  .....Dialog.....
-00001320: 2c00 4c00 6f00 6700 2000 6900 6e00 2000  ,.L.o.g. .i.n. .
-00001330: 4400 6100 7400 6500 6900 2000 7300 6300  D.a.t.e.i. .s.c.
-00001340: 6800 7200 6500 6900 6200 6500 6e08 0000  h.r.e.i.b.e.n...
-00001350: 0000 0600 0000 0b4c 6f67 2074 6f20 6669  .......Log to fi
-00001360: 6c65 0700 0000 0644 6961 6c6f 6701 0300  le.....Dialog...
-00001370: 0000 1e00 4c00 6f00 6700 6700 6900 6e00  ....L.o.g.g.i.n.
-00001380: 6700 2d00 4100 7500 7300 6700 6100 6200  g.-.A.u.s.g.a.b.
-00001390: 6508 0000 0000 0600 0000 0e4c 6f67 6769  e..........Loggi
-000013a0: 6e67 206f 7574 7075 7407 0000 0006 4469  ng output.....Di
-000013b0: 616c 6f67 0103 0000 000a 004c 00e4 006e  alog.......L...n
-000013c0: 0067 0065 0800 0000 0006 0000 0003 4c6f  .g.e..........Lo
-000013d0: 6e07 0000 0006 4469 616c 6f67 0103 ffff  n.....Dialog....
-000013e0: ffff 0800 0000 0006 0000 0004 4e61 6d65  ............Name
-000013f0: 0700 0000 0644 6961 6c6f 6701 0300 0000  .....Dialog.....
-00001400: 5e00 4300 4200 2000 5100 5300 4f00 7300  ^.C.B. .Q.S.O.s.
-00001410: 2000 7700 6500 7200 6400 6500 6e00 2000   .w.e.r.d.e.n. .
-00001420: 6200 6500 6900 6d00 2000 4900 6d00 7000  b.e.i.m. .I.m.p.
-00001430: 6f00 7200 7400 2000 6900 6d00 6d00 6500  o.r.t. .i.m.m.e.
-00001440: 7200 2000 6200 6500 7200 fc00 6300 6b00  r. .b.e.r...c.k.
-00001450: 7300 6900 6300 6800 7400 6900 6700 7408  s.i.c.h.t.i.g.t.
-00001460: 0000 0000 0600 0000 284f 6e20 696d 706f  ........(On impo
-00001470: 7274 2043 4220 5153 4f73 2077 696c 6c20  rt CB QSOs will 
-00001480: 616c 7761 7973 2062 6520 6861 6e64 6c65  always be handle
-00001490: 6407 0000 0006 4469 616c 6f67 0103 0000  d.....Dialog....
-000014a0: 0010 0050 0061 0073 0073 0077 006f 0072  ...P.a.s.s.w.o.r
-000014b0: 0074 0800 0000 0006 0000 0008 5061 7373  .t..........Pass
-000014c0: 776f 7264 0700 0000 0644 6961 6c6f 6701  word.....Dialog.
-000014d0: 0300 0000 7000 5000 6100 7300 7300 7700  ....p.P.a.s.s.w.
-000014e0: 6f00 7200 7400 2000 6400 6500 7300 2000  o.r.t. .d.e.s. .
-000014f0: 4c00 6f00 5400 5700 2d00 4f00 6e00 6c00  L.o.T.W.-.O.n.l.
-00001500: 6900 6e00 6500 2d00 4100 6300 6300 6f00  i.n.e.-.A.c.c.o.
-00001510: 7500 6e00 7400 7300 2c00 2000 6e00 6900  u.n.t.s.,. .n.i.
-00001520: 6300 6800 7400 2000 6400 6500 7300 2000  c.h.t. .d.e.s. .
-00001530: 5a00 6500 7200 7400 6900 6600 6900 6b00  Z.e.r.t.i.f.i.k.
-00001540: 6100 7400 7308 0000 0000 0600 0000 3850  a.t.s.........8P
-00001550: 6173 7377 6f72 6420 666f 7220 4c6f 5457  assword for LoTW
-00001560: 206f 6e6c 696e 6520 6163 636f 756e 7420   online account 
-00001570: 6e6f 7420 666f 7220 7468 6520 6365 7274  not for the cert
-00001580: 6966 6963 6174 6507 0000 0006 4469 616c  ificate.....Dial
-00001590: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
-000015a0: 0003 5154 4807 0000 0006 4469 616c 6f67  ..QTH.....Dialog
-000015b0: 0103 ffff ffff 0800 0000 0006 0000 0005  ................
-000015c0: 5261 6469 6f07 0000 0006 4469 616c 6f67  Radio.....Dialog
-000015d0: 0103 0000 0018 004e 0065 0075 0065 0073  .......N.e.u.e.s
-000015e0: 0074 0065 0020 0051 0053 004f 0073 0800  .t.e. .Q.S.O.s..
-000015f0: 0000 0006 0000 000b 5265 6365 6e74 2051  ........Recent Q
-00001600: 534f 7307 0000 0006 4469 616c 6f67 0103  SOs.....Dialog..
-00001610: 0000 0012 0046 0075 006e 006b 0067 0065  .....F.u.n.k.g.e
-00001620: 0072 00e4 0074 0800 0000 0006 0000 0003  .r...t..........
-00001630: 5269 6707 0000 0006 4469 616c 6f67 0103  Rig.....Dialog..
-00001640: 0000 004c 0053 0069 0065 0068 0065 0020  ...L.S.i.e.h.e. 
-00001650: 0045 0069 006e 0073 0074 0065 006c 006c  .E.i.n.s.t.e.l.l
-00001660: 0075 006e 0067 0065 006e 0020 0052 0065  .u.n.g.e.n. .R.e
-00001670: 0069 0074 0065 0072 0020 0022 0041 006e  .i.t.e.r. .".A.n
-00001680: 0077 0065 006e 0064 0075 006e 0067 0022  .w.e.n.d.u.n.g."
-00001690: 0800 0000 0006 0000 0022 5365 6520 7365  ........."See se
-000016a0: 7474 696e 6773 2070 6167 6520 2255 7365  ttings page "Use
-000016b0: 7220 696e 7465 7266 6163 6522 0700 0000  r interface"....
-000016c0: 0644 6961 6c6f 6701 0300 0000 3400 4300  .Dialog.....4.C.
-000016d0: 4200 2d00 4200 6100 6e00 6400 2000 6100  B.-.B.a.n.d. .a.
-000016e0: 7500 7400 6f00 6d00 6100 7400 6900 7300  u.t.o.m.a.t.i.s.
-000016f0: 6300 6800 2000 7700 e400 6800 6c00 6500  c.h. .w...h.l.e.
-00001700: 6e08 0000 0000 0600 0000 1953 656c 6563  n..........Selec
-00001710: 7420 4342 2062 616e 6420 6279 2064 6566  t CB band by def
-00001720: 6175 6c74 0700 0000 0644 6961 6c6f 6701  ault.....Dialog.
-00001730: 0300 0000 0c00 4400 6900 6500 6e00 7300  ......D.i.e.n.s.
-00001740: 7408 0000 0000 0600 0000 0753 6572 7669  t..........Servi
-00001750: 6365 0700 0000 0644 6961 6c6f 6701 0300  ce.....Dialog...
-00001760: 0000 1a00 5300 6500 7400 7a00 6500 2000  ....S.e.t.z.e. .
-00001770: 4c00 6f00 6300 6100 7400 6f00 7208 0000  L.o.c.a.t.o.r...
-00001780: 0000 0600 0000 0b53 6574 206c 6f63 6174  .......Set locat
-00001790: 6f72 0700 0000 0644 6961 6c6f 6701 0300  or.....Dialog...
-000017a0: 0000 1a00 4500 6900 6e00 7300 7400 6500  ....E.i.n.s.t.e.
-000017b0: 6c00 6c00 7500 6e00 6700 6500 6e08 0000  l.l.u.n.g.e.n...
-000017c0: 0000 0600 0000 0853 6574 7469 6e67 7307  .......Settings.
-000017d0: 0000 0006 4469 616c 6f67 0103 0000 001c  ....Dialog......
-000017e0: 005a 0065 0069 0067 0065 0020 0051 0053  .Z.e.i.g.e. .Q.S
-000017f0: 004f 0073 0020 0066 00fc 0072 0800 0000  .O.s. .f...r....
-00001800: 0006 0000 000e 5368 6f77 2051 534f 7320  ......Show QSOs 
-00001810: 6672 6f6d 0700 0000 0644 6961 6c6f 6701  from.....Dialog.
-00001820: 0300 0000 1400 7a00 6500 6900 6700 6500  ......z.e.i.g.e.
-00001830: 2000 6100 6c00 6c00 6508 0000 0000 0600   .a.l.l.e.......
-00001840: 0000 0853 686f 7720 616c 6c07 0000 0006  ...Show all.....
-00001850: 4469 616c 6f67 0103 0000 0040 0053 0070  Dialog.....@.S.p
-00001860: 0061 006c 0074 0065 006e 0020 0061 006e  .a.l.t.e.n. .a.n
-00001870: 007a 0065 0069 0067 0065 006e 0020 006f  .z.e.i.g.e.n. .o
-00001880: 0064 0065 0072 0020 0076 0065 0072 0073  .d.e.r. .v.e.r.s
-00001890: 0074 0065 0063 006b 0065 006e 0800 0000  .t.e.c.k.e.n....
-000018a0: 0006 0000 0014 5368 6f77 206f 7220 6869  ......Show or hi
-000018b0: 6465 2063 6f6c 756d 6e73 0700 0000 0644  de columns.....D
-000018c0: 6961 6c6f 6701 0300 0000 2800 5300 6f00  ialog.....(.S.o.
-000018d0: 7200 7400 6900 6500 7200 6500 2000 6e00  r.t.i.e.r.e. .n.
-000018e0: 6100 6300 6800 2000 5300 7000 6100 6c00  a.c.h. .S.p.a.l.
-000018f0: 7400 6508 0000 0000 0600 0000 0e53 6f72  t.e..........Sor
-00001900: 7420 6f6e 2063 6f6c 756d 6e07 0000 0006  t on column.....
-00001910: 4469 616c 6f67 0103 ffff ffff 0800 0000  Dialog..........
-00001920: 0006 0000 0005 5374 6172 7407 0000 0006  ......Start.....
-00001930: 4469 616c 6f67 0103 ffff ffff 0800 0000  Dialog..........
-00001940: 0006 0000 0007 5374 6174 696f 6e07 0000  ......Station...
-00001950: 0006 4469 616c 6f67 0103 ffff ffff 0800  ..Dialog........
-00001960: 0000 0006 0000 0004 5451 534c 0700 0000  ........TQSL....
-00001970: 0644 6961 6c6f 6701 0300 0000 6400 5600  .Dialog.....d.V.
-00001980: 6500 7200 7700 6500 6e00 6400 6500 2000  e.r.w.e.n.d.e. .
-00001990: 6400 6900 6500 2000 6b00 6f00 6e00 6600  d.i.e. .k.o.n.f.
-000019a0: 6900 6700 7500 7200 6900 6500 7200 7400  i.g.u.r.i.e.r.t.
-000019b0: 6500 2000 4900 4400 2000 6200 6500 6900  e. .I.D. .b.e.i.
-000019c0: 2000 6600 6500 6800 6c00 6500 6e00 6400   .f.e.h.l.e.n.d.
-000019d0: 6500 6e00 2000 5700 6500 7200 7400 6500  e.n. .W.e.r.t.e.
-000019e0: 6e08 0000 0000 0600 0000 2455 7365 2063  n.........$Use c
-000019f0: 6f6e 6669 6775 7265 6420 4944 2066 6f72  onfigured ID for
-00001a00: 206d 6973 7369 6e67 2076 616c 7565 7307   missing values.
-00001a10: 0000 0006 4469 616c 6f67 0103 0000 006e  ....Dialog.....n
-00001a20: 0056 0065 0072 0077 0065 006e 0064 0065  .V.e.r.w.e.n.d.e
-00001a30: 0020 0064 0069 0065 0020 006b 006f 006e  . .d.i.e. .k.o.n
-00001a40: 0066 0069 0067 0075 0072 0069 0065 0072  .f.i.g.u.r.i.e.r
-00001a50: 0074 0065 0020 0053 0074 0061 0074 0069  .t.e. .S.t.a.t.i
-00001a60: 006f 006e 0020 0062 0065 0069 0020 0066  .o.n. .b.e.i. .f
-00001a70: 0065 0068 006c 0065 006e 0064 0065 006e  .e.h.l.e.n.d.e.n
-00001a80: 0020 0057 0065 0072 0074 0065 006e 0800  . .W.e.r.t.e.n..
-00001a90: 0000 0006 0000 0029 5573 6520 636f 6e66  .......)Use conf
-00001aa0: 6967 7572 6564 2053 7461 7469 6f6e 2066  igured Station f
-00001ab0: 6f72 206d 6973 7369 6e67 2076 616c 7565  or missing value
-00001ac0: 7307 0000 0006 4469 616c 6f67 0103 0000  s.....Dialog....
-00001ad0: 0012 0041 006e 0077 0065 006e 0064 0075  ...A.n.w.e.n.d.u
-00001ae0: 006e 0067 0800 0000 0006 0000 000e 5573  .n.g..........Us
-00001af0: 6572 2069 6e74 6572 6661 6365 0700 0000  er interface....
-00001b00: 0644 6961 6c6f 6701 0300 0000 1800 4200  .Dialog.......B.
-00001b10: 6500 6e00 7500 7400 7a00 6500 7200 6e00  e.n.u.t.z.e.r.n.
-00001b20: 6100 6d00 6508 0000 0000 0600 0000 0855  a.m.e..........U
-00001b30: 7365 726e 616d 6507 0000 0006 4469 616c  sername.....Dial
-00001b40: 6f67 0103 0000 0078 0042 0065 006e 0075  og.....x.B.e.n.u
-00001b50: 0074 007a 0065 0072 006e 0061 006d 0065  .t.z.e.r.n.a.m.e
-00001b60: 0020 0064 0065 0073 0020 004c 006f 0054  . .d.e.s. .L.o.T
-00001b70: 0057 002d 004f 006e 006c 0069 006e 0065  .W.-.O.n.l.i.n.e
-00001b80: 002d 0041 0063 0063 006f 0075 006e 0074  .-.A.c.c.o.u.n.t
-00001b90: 0073 002c 0020 006e 0069 0063 0068 0074  .s.,. .n.i.c.h.t
-00001ba0: 0020 0064 0065 0073 0020 005a 0065 0072  . .d.e.s. .Z.e.r
-00001bb0: 0074 0069 0066 0069 006b 0061 0074 0073  .t.i.f.i.k.a.t.s
-00001bc0: 0800 0000 0006 0000 0038 5573 6572 6e61  .........8Userna
-00001bd0: 6d65 2066 6f72 204c 6f54 5720 6f6e 6c69  me for LoTW onli
-00001be0: 6e65 2061 6363 6f75 6e74 206e 6f74 2066  ne account not f
-00001bf0: 6f72 2074 6865 2063 6572 7469 6669 6361  or the certifica
-00001c00: 7465 0700 0000 0644 6961 6c6f 6701 0300  te.....Dialog...
-00001c10: 0000 2000 4400 6100 7400 6500 6900 fc00  .. .D.a.t.e.i...
-00001c20: 6200 6500 7200 7700 6100 6300 6800 7500  b.e.r.w.a.c.h.u.
-00001c30: 6e00 6708 0000 0000 0600 0000 0a57 6174  n.g..........Wat
-00001c40: 6368 2046 696c 6507 0000 0006 4469 616c  ch File.....Dial
-00001c50: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
-00001c60: 0004 6551 534c 0700 0000 0644 6961 6c6f  ..eQSL.....Dialo
-00001c70: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
-00001c80: 02c2 b007 0000 0006 4469 616c 6f67 0103  ........Dialog..
-00001c90: 0000 009e 0045 0069 006e 0020 0044 0061  .....E.i.n. .D.a
-00001ca0: 0074 0065 006e 0062 0061 006e 006b 002d  .t.e.n.b.a.n.k.-
-00001cb0: 0042 0061 0063 006b 0075 0070 0020 006b  .B.a.c.k.u.p. .k
-00001cc0: 006f 006e 006e 0074 0065 0020 006e 0069  .o.n.n.t.e. .n.i
-00001cd0: 0063 0068 0074 0020 0065 0072 0073 0074  .c.h.t. .e.r.s.t
-00001ce0: 0065 006c 006c 0074 0020 0077 0065 0072  .e.l.l.t. .w.e.r
-00001cf0: 0064 0065 006e 002e 000a 0044 0069 0065  .d.e.n.....D.i.e
-00001d00: 0020 0044 0061 0074 0065 0069 0020 0065  . .D.a.t.e.i. .e
-00001d10: 0078 0069 0073 0074 0069 0065 0072 0074  .x.i.s.t.i.e.r.t
-00001d20: 0020 0062 0065 0072 0065 0069 0074 0073  . .b.e.r.e.i.t.s
-00001d30: 002e 0800 0000 0006 0000 0040 4120 6461  ...........@A da
-00001d40: 7461 6261 7365 2062 6163 6b75 7020 636f  tabase backup co
-00001d50: 756c 6420 6e6f 7420 6265 2063 7265 6174  uld not be creat
-00001d60: 6564 2e0a 5468 6520 6669 6c65 2061 6c72  ed..The file alr
-00001d70: 6561 6479 2065 7869 7374 732e 0700 0000  eady exists.....
-00001d80: 0944 7261 676f 6e4c 6f67 0103 0000 004e  .DragonLog.....N
-00001d90: 0045 0069 006e 0020 0041 0044 0049 0046  .E.i.n. .A.D.I.F
-00001da0: 002d 0046 0065 006c 0064 0020 0066 0065  .-.F.e.l.d. .f.e
-00001db0: 0068 006c 0074 0020 0066 00fc 0072 0020  .h.l.t. .f...r. 
-00001dc0: 0064 0065 006e 0020 004c 006f 0054 0057  .d.e.n. .L.o.T.W
-00001dd0: 002d 0055 0070 006c 006f 0061 0064 0800  .-.U.p.l.o.a.d..
-00001de0: 0000 0006 0000 001d 4120 6669 656c 6420  ........A field 
-00001df0: 6973 206d 6973 7369 6e67 2066 6f72 2075  is missing for u
-00001e00: 706c 6f61 6407 0000 0009 4472 6167 6f6e  pload.....Dragon
-00001e10: 4c6f 6701 03ff ffff ff08 0000 0000 0600  Log.............
-00001e20: 0000 1541 4449 4620 3320 282a 2e61 6469  ...ADIF 3 (*.adi
-00001e30: 202a 2e61 6469 6629 0700 0000 0944 7261   *.adif).....Dra
-00001e40: 676f 6e4c 6f67 0103 ffff ffff 0800 0000  gonLog..........
-00001e50: 0006 0000 001b 4144 4946 2033 2028 2a2e  ......ADIF 3 (*.
-00001e60: 6164 7820 2a2e 6164 6920 2a2e 6164 6966  adx *.adi *.adif
-00001e70: 2907 0000 0009 4472 6167 6f6e 4c6f 6701  ).....DragonLog.
-00001e80: 0300 0000 0800 dc00 6200 6500 7208 0000  ........b.e.r...
-00001e90: 0000 0600 0000 0541 626f 7574 0700 0000  .......About....
-00001ea0: 0944 7261 676f 6e4c 6f67 0103 0000 000e  .DragonLog......
-00001eb0: 00dc 0062 0065 0072 0020 0051 0074 0800  ...b.e.r. .Q.t..
-00001ec0: 0000 0006 0000 0008 4162 6f75 7420 5174  ........About Qt
-00001ed0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00001ee0: 0000 0020 0041 0069 0072 0063 0072 0061  ... .A.i.r.c.r.a
-00001ef0: 0066 0074 002d 0053 0063 0061 0074 0074  .f.t.-.S.c.a.t.t
-00001f00: 0065 0072 0800 0000 0006 0000 0010 4169  .e.r..........Ai
-00001f10: 7263 7261 6674 2053 6361 7474 6572 0700  rcraft Scatter..
-00001f20: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
-00001f30: 000e 0041 006e 0074 0065 006e 006e 0065  ...A.n.t.e.n.n.e
-00001f40: 0800 0000 0006 0000 0007 416e 7465 6e6e  ..........Antenn
-00001f50: 6107 0000 0009 4472 6167 6f6e 4c6f 6701  a.....DragonLog.
-00001f60: 03ff ffff ff08 0000 0000 0600 0000 0641  ...............A
-00001f70: 7572 6f72 6107 0000 0009 4472 6167 6f6e  urora.....Dragon
-00001f80: 4c6f 6701 03ff ffff ff08 0000 0000 0600  Log.............
-00001f90: 0000 0841 7572 6f72 612d 4507 0000 0009  ...Aurora-E.....
-00001fa0: 4472 6167 6f6e 4c6f 6701 0300 0000 0a00  DragonLog.......
-00001fb0: 4100 7500 7400 6f00 7208 0000 0000 0600  A.u.t.o.r.......
-00001fc0: 0000 0641 7574 686f 7207 0000 0009 4472  ...Author.....Dr
-00001fd0: 6167 6f6e 4c6f 6701 0300 0000 1800 4200  agonLog.......B.
-00001fe0: 6100 6300 6b00 2d00 5300 6300 6100 7400  a.c.k.-.S.c.a.t.
-00001ff0: 7400 6500 7208 0000 0000 0600 0000 0c42  t.e.r..........B
-00002000: 6163 6b20 7363 6174 7465 7207 0000 0009  ack scatter.....
-00002010: 4472 6167 6f6e 4c6f 6701 03ff ffff ff08  DragonLog.......
-00002020: 0000 0000 0600 0000 0442 616e 6407 0000  .........Band...
-00002030: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-00002040: 2200 4300 5300 5600 2d00 4400 6100 7400  ".C.S.V.-.D.a.t.
-00002050: 6500 6900 2000 2800 2a00 2e00 6300 7300  e.i. .(.*...c.s.
-00002060: 7600 2908 0000 0000 0600 0000 1043 5356  v.)..........CSV
-00002070: 2d46 696c 6520 282a 2e63 7376 2907 0000  -File (*.csv)...
-00002080: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-00002090: 1400 5200 7500 6600 7a00 6500 6900 6300  ..R.u.f.z.e.i.c.
-000020a0: 6800 6500 6e08 0000 0000 0600 0000 0943  h.e.n..........C
-000020b0: 616c 6c20 7369 676e 0700 0000 0944 7261  all sign.....Dra
-000020c0: 676f 6e4c 6f67 0103 0000 000a 004b 0061  gonLog.......K.a
-000020d0: 006e 0061 006c 0800 0000 0006 0000 0007  .n.a.l..........
-000020e0: 4368 616e 6e65 6c07 0000 0009 4472 6167  Channel.....Drag
-000020f0: 6f6e 4c6f 6701 0300 0000 7400 5000 7200  onLog.....t.P.r.
-00002100: fc00 6600 7500 6e00 6700 2000 6400 6500  ..f.u.n.g. .d.e.
-00002110: 7200 2000 4400 6100 7400 6500 6e00 6200  r. .D.a.t.e.n.b.
-00002120: 6100 6e00 6b00 2000 6600 6500 6800 6c00  a.n.k. .f.e.h.l.
-00002130: 6700 6500 7300 6300 6800 6c00 6100 6700  g.e.s.c.h.l.a.g.
-00002140: 6500 6e00 2e00 2000 4900 6e00 6800 6100  e.n... .I.n.h.a.
-00002150: 6c00 7400 2000 6e00 6900 6300 6800 7400  l.t. .n.i.c.h.t.
-00002160: 2000 6c00 6500 7300 6200 6100 7200 2e08   .l.e.s.b.a.r...
-00002170: 0000 0000 0600 0000 3443 6865 636b 696e  ........4Checkin
-00002180: 6720 6461 7461 6261 7365 2066 6169 6c65  g database faile
-00002190: 642e 2043 6f6e 7465 6e74 2069 7320 6e6f  d. Content is no
-000021a0: 7420 6163 6365 7373 6162 6c65 2e07 0000  t accessable....
-000021b0: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-000021c0: 1200 4b00 6f00 6d00 6d00 6500 6e00 7400  ..K.o.m.m.e.n.t.
-000021d0: 6100 7208 0000 0000 0600 0000 0743 6f6d  a.r..........Com
-000021e0: 6d65 6e74 0700 0000 0944 7261 676f 6e4c  ment.....DragonL
-000021f0: 6f67 0103 0000 0060 0056 0065 0072 0062  og.....`.V.e.r.b
-00002200: 0069 006e 0064 0075 006e 0067 0073 0066  .i.n.d.u.n.g.s.f
-00002210: 0065 0068 006c 0065 0072 0020 006f 0064  .e.h.l.e.r. .o.d
-00002220: 0065 0072 0020 004e 0065 0074 007a 0077  .e.r. .N.e.t.z.w
-00002230: 0065 0072 006b 0020 006e 0069 0063 0068  .e.r.k. .n.i.c.h
-00002240: 0074 0020 0065 0072 0072 0065 0069 0063  .t. .e.r.r.e.i.c
-00002250: 0068 0062 0061 0072 0800 0000 0006 0000  .h.b.a.r........
-00002260: 0027 436f 6e6e 6563 7469 6f6e 2065 7272  .'Connection err
-00002270: 6f72 206f 7220 6e65 7477 6f72 6b20 756e  or or network un
-00002280: 7265 6163 6861 626c 6507 0000 0009 4472  reachable.....Dr
-00002290: 6167 6f6e 4c6f 6701 03ff ffff ff08 0000  agonLog.........
-000022a0: 0000 0600 0000 0743 6f6e 7465 7374 0700  .......Contest..
-000022b0: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
-000022c0: 002e 0044 0061 0074 0065 006e 0062 0061  ...D.a.t.e.n.b.a
-000022d0: 006e 006b 002d 0042 0061 0063 006b 0075  .n.k.-.B.a.c.k.u
-000022e0: 0070 0020 0046 0065 0068 006c 0065 0072  .p. .F.e.h.l.e.r
-000022f0: 0800 0000 0006 0000 0015 4461 7461 6261  ..........Databa
-00002300: 7365 2062 6163 6b75 7020 6572 726f 7207  se backup error.
-00002310: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
-00002320: 0000 2c00 4400 6100 7400 6500 6e00 6200  ..,.D.a.t.e.n.b.
-00002330: 6100 6e00 6b00 6b00 6f00 6e00 7600 6500  a.n.k.k.o.n.v.e.
-00002340: 7200 7400 6900 6500 7200 7500 6e00 6708  r.t.i.e.r.u.n.g.
-00002350: 0000 0000 0600 0000 1344 6174 6162 6173  .........Databas
-00002360: 6520 636f 6e76 6572 7369 6f6e 0700 0000  e conversion....
-00002370: 0944 7261 676f 6e4c 6f67 0103 0000 0048  .DragonLog.....H
-00002380: 0044 0061 0074 0065 006e 0062 0061 006e  .D.a.t.e.n.b.a.n
-00002390: 006b 006b 006f 006e 0076 0065 0072 0074  .k.k.o.n.v.e.r.t
-000023a0: 0069 0065 0072 0075 006e 0067 0020 0061  .i.e.r.u.n.g. .a
-000023b0: 0062 0067 0065 0073 0063 0068 006c 006f  .b.g.e.s.c.h.l.o
-000023c0: 0073 0073 0065 006e 0800 0000 0006 0000  .s.s.e.n........
-000023d0: 001c 4461 7461 6261 7365 2063 6f6e 7665  ..Database conve
-000023e0: 7273 696f 6e20 6669 6e69 7368 6564 0700  rsion finished..
-000023f0: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
-00002400: 001e 0044 0061 0074 0065 006e 0062 0061  ...D.a.t.e.n.b.a
-00002410: 006e 006b 0066 0065 0068 006c 0065 0072  .n.k.f.e.h.l.e.r
-00002420: 0800 0000 0006 0000 000e 4461 7461 6261  ..........Databa
-00002430: 7365 2065 7272 6f72 0700 0000 0944 7261  se error.....Dra
-00002440: 676f 6e4c 6f67 0103 0000 0034 0044 0061  gonLog.....4.D.a
-00002450: 0074 0065 006e 0062 0061 006e 006b 0073  .t.e.n.b.a.n.k.s
-00002460: 0074 0072 0075 006b 0074 0075 0072 0020  .t.r.u.k.t.u.r. 
-00002470: 0076 0065 0072 0061 006c 0074 0065 0074  .v.e.r.a.l.t.e.t
-00002480: 0800 0000 0006 0000 001c 4461 7461 6261  ..........Databa
-00002490: 7365 2073 7472 7563 7475 7265 206f 7574  se structure out
-000024a0: 2d64 6174 6564 0700 0000 0944 7261 676f  -dated.....Drago
-000024b0: 6e4c 6f67 0103 0000 001e 0044 0061 0074  nLog.......D.a.t
-000024c0: 0075 006d 002f 005a 0065 0069 0074 0020  .u.m./.Z.e.i.t. 
-000024d0: 0045 006e 0064 0065 0800 0000 0006 0000  .E.n.d.e........
-000024e0: 000d 4461 7465 2f54 696d 6520 656e 6407  ..Date/Time end.
-000024f0: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
-00002500: 0000 2000 4400 6100 7400 7500 6d00 2f00  .. .D.a.t.u.m./.
-00002510: 5a00 6500 6900 7400 2000 5300 7400 6100  Z.e.i.t. .S.t.a.
-00002520: 7200 7408 0000 0000 0600 0000 0f44 6174  r.t..........Dat
-00002530: 652f 5469 6d65 2073 7461 7274 0700 0000  e/Time start....
-00002540: 0944 7261 676f 6e4c 6f67 0103 0000 0016  .DragonLog......
-00002550: 0051 0053 004f 0020 006c 00f6 0073 0063  .Q.S.O. .l...s.c
-00002560: 0068 0065 006e 0800 0000 0006 0000 000a  .h.e.n..........
-00002570: 4465 6c65 7465 2051 534f 0700 0000 0944  Delete QSO.....D
-00002580: 7261 676f 6e4c 6f67 0103 0000 0014 0045  ragonLog.......E
-00002590: 006e 0074 0066 0065 0072 006e 0075 006e  .n.t.f.e.r.n.u.n
-000025a0: 0067 0800 0000 0006 0000 0008 4469 7374  .g..........Dist
-000025b0: 616e 6365 0700 0000 0944 7261 676f 6e4c  ance.....DragonL
-000025c0: 6f67 0103 0000 0064 0057 006f 006c 006c  og.....d.W.o.l.l
-000025d0: 0065 006e 0020 0073 0069 0065 0020 0064  .e.n. .s.i.e. .d
-000025e0: 0069 0065 0020 0073 0065 006c 0065 006b  .i.e. .s.e.l.e.k
-000025f0: 0074 0069 0065 0072 0074 0065 006e 0020  .t.i.e.r.t.e.n. 
-00002600: 0051 0053 004f 0073 0020 0077 0069 0072  .Q.S.O.s. .w.i.r
-00002610: 006b 006c 0069 0063 0068 0020 006c 00f6  .k.l.i.c.h. .l..
-00002620: 0073 0063 0068 0065 006e 003f 0800 0000  .s.c.h.e.n.?....
-00002630: 0006 0000 0031 446f 2079 6f75 2072 6561  .....1Do you rea
-00002640: 6c6c 7920 7761 6e74 2074 6f20 6465 6c65  lly want to dele
-00002650: 7465 2074 6865 2073 656c 6563 7465 6420  te the selected 
-00002660: 5153 4f28 7329 3f07 0000 0009 4472 6167  QSO(s)?.....Drag
-00002670: 6f6e 4c6f 6701 03ff ffff ff08 0000 0000  onLog...........
-00002680: 0600 0000 1045 6172 7468 2d4d 6f6f 6e2d  .....Earth-Moon-
-00002690: 4561 7274 6807 0000 0009 4472 6167 6f6e  Earth.....Dragon
-000026a0: 4c6f 6701 03ff ffff ff08 0000 0000 0600  Log.............
-000026b0: 0000 0845 6368 6f4c 696e 6b07 0000 0009  ...EchoLink.....
-000026c0: 4472 6167 6f6e 4c6f 6701 0300 0000 0c00  DragonLog.......
-000026d0: 4600 6500 6800 6c00 6500 7208 0000 0000  F.e.h.l.e.r.....
-000026e0: 0600 0000 0545 7272 6f72 0700 0000 0944  .....Error.....D
-000026f0: 7261 676f 6e4c 6f67 0103 0000 0028 0045  ragonLog.....(.E
-00002700: 0078 0063 0065 006c 002d 0044 0061 0074  .x.c.e.l.-.D.a.t
-00002710: 0065 0069 0020 0028 002a 002e 0078 006c  .e.i. .(.*...x.l
-00002720: 0073 0078 0029 0800 0000 0006 0000 0013  .s.x.)..........
-00002730: 4578 6365 6c2d 4669 6c65 2028 2a2e 786c  Excel-File (*.xl
-00002740: 7378 2907 0000 0009 4472 6167 6f6e 4c6f  sx).....DragonLo
-00002750: 6701 0300 0000 2400 4500 7800 7000 6f00  g.....$.E.x.p.o.
-00002760: 7200 7400 6900 6500 7200 6500 2000 5100  r.t.i.e.r.e. .Q.
-00002770: 5300 4f00 2000 6c00 6f00 6708 0000 0000  S.O. .l.o.g.....
-00002780: 0600 0000 1045 7870 6f72 7465 6420 5153  .....Exported QS
-00002790: 4f20 6c6f 6707 0000 0009 4472 6167 6f6e  O log.....Dragon
-000027a0: 4c6f 6701 0300 0000 1a00 4600 3200 2d00  Log.......F.2.-.
-000027b0: 5200 6500 6600 6c00 6500 6b00 7400 6900  R.e.f.l.e.k.t.i.
-000027c0: 6f00 6e08 0000 0000 0600 0000 0d46 3220  o.n..........F2 
-000027d0: 5265 666c 6563 7469 6f6e 0700 0000 0944  Reflection.....D
-000027e0: 7261 676f 6e4c 6f67 0103 0000 0038 0046  ragonLog.....8.F
-000027f0: 0069 0065 006c 0064 002d 0041 006c 0069  .i.e.l.d.-.A.l.i
-00002800: 0067 006e 0065 0064 002d 0049 0072 0072  .g.n.e.d.-.I.r.r
-00002810: 0065 0067 0075 006c 0061 0072 0069 0074  .e.g.u.l.a.r.i.t
-00002820: 0069 0065 0073 0800 0000 0006 0000 001c  .i.e.s..........
-00002830: 4669 656c 6420 416c 6967 6e65 6420 4972  Field Aligned Ir
-00002840: 7265 6775 6c61 7269 7469 6573 0700 0000  regularities....
-00002850: 0944 7261 676f 6e4c 6f67 0103 0000 0010  .DragonLog......
-00002860: 0046 0072 0065 0071 0075 0065 006e 007a  .F.r.e.q.u.e.n.z
-00002870: 0800 0000 0006 0000 0009 4672 6571 7565  ..........Freque
-00002880: 6e63 7907 0000 0009 4472 6167 6f6e 4c6f  ncy.....DragonLo
-00002890: 6701 0300 0000 1400 4200 6f00 6400 6500  g.......B.o.d.e.
-000028a0: 6e00 7700 6500 6c00 6c00 6508 0000 0000  n.w.e.l.l.e.....
-000028b0: 0600 0000 0b47 726f 756e 6420 5761 7665  .....Ground Wave
-000028c0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-000028d0: ffff ffff 0800 0000 0006 0000 0006 4861  ..............Ha
-000028e0: 6d51 5448 0700 0000 0944 7261 676f 6e4c  mQTH.....DragonL
-000028f0: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
-00002900: 0006 4861 6d6c 6962 0700 0000 0944 7261  ..Hamlib.....Dra
-00002910: 676f 6e4c 6f67 0103 0000 000a 0048 0069  gonLog.......H.i
-00002920: 006c 0066 0065 0800 0000 0006 0000 0004  .l.f.e..........
-00002930: 4865 6c70 0700 0000 0944 7261 676f 6e4c  Help.....DragonL
-00002940: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
-00002950: 0004 4952 4c50 0700 0000 0944 7261 676f  ..IRLP.....Drago
-00002960: 6e4c 6f67 0103 0000 0026 0049 006e 0074  nLog.....&.I.n.t
-00002970: 0065 0072 006e 0065 0074 0075 006e 0074  .e.r.n.e.t.u.n.t
-00002980: 0065 0072 0073 0074 00fc 0074 007a 0074  .e.r.s.t...t.z.t
-00002990: 0800 0000 0006 0000 0011 496e 7465 726e  ..........Intern
-000029a0: 6574 2d61 7373 6973 7465 6407 0000 0009  et-assisted.....
-000029b0: 4472 6167 6f6e 4c6f 6701 0300 0000 1800  DragonLog.......
-000029c0: 4900 6f00 6e00 6f00 2d00 5300 6300 6100  I.o.n.o.-.S.c.a.
-000029d0: 7400 7400 6500 7208 0000 0000 0600 0000  t.t.e.r.........
-000029e0: 0b49 6f6e 6f73 6361 7474 6572 0700 0000  .Ionoscatter....
-000029f0: 0944 7261 676f 6e4c 6f67 0103 0000 0020  .DragonLog..... 
-00002a00: 006c 0065 0074 007a 0074 0065 0073 0020  .l.e.t.z.t.e.s. 
-00002a10: 0048 0061 006c 0062 006a 0061 0068 0072  .H.a.l.b.j.a.h.r
-00002a20: 0800 0000 0006 0000 000e 4c61 7374 2068  ..........Last h
-00002a30: 616c 6620 7965 6172 0700 0000 0944 7261  alf year.....Dra
-00002a40: 676f 6e4c 6f67 0103 0000 001a 006c 0065  gonLog.......l.e
-00002a50: 0074 007a 0074 0065 006e 0020 004d 006f  .t.z.t.e.n. .M.o
-00002a60: 006e 0061 0074 0800 0000 0006 0000 000a  .n.a.t..........
-00002a70: 4c61 7374 206d 6f6e 7468 0700 0000 0944  Last month.....D
-00002a80: 7261 676f 6e4c 6f67 0103 0000 0018 006c  ragonLog.......l
-00002a90: 0065 0074 007a 0074 0065 0020 0057 006f  .e.t.z.t.e. .W.o
-00002aa0: 0063 0068 0065 0800 0000 0006 0000 0009  .c.h.e..........
-00002ab0: 4c61 7374 2077 6565 6b07 0000 0009 4472  Last week.....Dr
-00002ac0: 6167 6f6e 4c6f 6701 0300 0000 1800 6c00  agonLog.......l.
-00002ad0: 6500 7400 7a00 7400 6500 7300 2000 4a00  e.t.z.t.e.s. .J.
-00002ae0: 6100 6800 7208 0000 0000 0600 0000 094c  a.h.r..........L
-00002af0: 6173 7420 7965 6172 0700 0000 0944 7261  ast year.....Dra
-00002b00: 676f 6e4c 6f67 0103 0000 001e 0053 0069  gonLog.......S.i
-00002b10: 0063 0068 0074 0076 0065 0072 0062 0069  .c.h.t.v.e.r.b.i
-00002b20: 006e 0064 0075 006e 0067 0800 0000 0006  .n.d.u.n.g......
-00002b30: 0000 000d 4c69 6e65 206f 6620 5369 6768  ....Line of Sigh
-00002b40: 7407 0000 0009 4472 6167 6f6e 4c6f 6701  t.....DragonLog.
-00002b50: 0300 0000 2000 4c00 6f00 5400 5700 2d00  .... .L.o.T.W.-.
-00002b60: 4100 4400 4900 4600 2d00 5500 7000 6c00  A.D.I.F.-.U.p.l.
-00002b70: 6f00 6100 6408 0000 0000 0600 0000 104c  o.a.d..........L
-00002b80: 6f54 5720 4144 4946 2075 706c 6f61 6407  oTW ADIF upload.
-00002b90: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
-00002ba0: 0000 1400 4c00 6f00 5400 5700 2000 6500  ....L.o.T.W. .e.
-00002bb0: 6d00 7000 6600 2e08 0000 0000 0600 0000  m.p.f...........
-00002bc0: 094c 6f54 5720 7263 7664 0700 0000 0944  .LoTW rcvd.....D
-00002bd0: 7261 676f 6e4c 6f67 0103 0000 0014 004c  ragonLog.......L
-00002be0: 006f 0054 0057 0020 0076 0065 0072 0073  .o.T.W. .v.e.r.s
-00002bf0: 002e 0800 0000 0006 0000 0009 4c6f 5457  ............LoTW
-00002c00: 2073 656e 7407 0000 0009 4472 6167 6f6e   sent.....Dragon
-00002c10: 4c6f 6701 03ff ffff ff08 0000 0000 0600  Log.............
-00002c20: 0000 074c 6f63 6174 6f72 0700 0000 0944  ...Locator.....D
-00002c30: 7261 676f 6e4c 6f67 0103 ffff ffff 0800  ragonLog........
-00002c40: 0000 0006 0000 000f 4c6f 6720 696d 706f  ........Log impo
-00002c50: 7274 2041 4449 4607 0000 0009 4472 6167  rt ADIF.....Drag
-00002c60: 6f6e 4c6f 6701 0300 0000 1c00 4c00 6f00  onLog.......L.o.
-00002c70: 6700 2000 4900 6d00 7000 6f00 7200 7400  g. .I.m.p.o.r.t.
-00002c80: 2000 4300 5300 5608 0000 0000 0600 0000   .C.S.V.........
-00002c90: 0e4c 6f67 2069 6d70 6f72 7420 4353 5607  .Log import CSV.
-00002ca0: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
-00002cb0: 0000 2000 4c00 6f00 6700 2000 4900 6d00  .. .L.o.g. .I.m.
-00002cc0: 7000 6f00 7200 7400 2000 4500 7800 6300  p.o.r.t. .E.x.c.
-00002cd0: 6500 6c08 0000 0000 0600 0000 104c 6f67  e.l..........Log
-00002ce0: 2069 6d70 6f72 7420 4578 6365 6c07 0000   import Excel...
-00002cf0: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-00002d00: 1c00 4d00 6500 7400 6500 6f00 7200 2d00  ..M.e.t.e.o.r.-.
-00002d10: 5300 6300 6100 7400 7400 6500 7208 0000  S.c.a.t.t.e.r...
-00002d20: 0000 0600 0000 0e4d 6574 656f 7220 7363  .......Meteor sc
-00002d30: 6174 7465 7207 0000 0009 4472 6167 6f6e  atter.....Dragon
-00002d40: 4c6f 6701 0300 0000 5a00 4b00 6500 6900  Log.....Z.K.e.i.
-00002d50: 6e00 6500 2000 5300 7400 6100 7400 6900  n.e. .S.t.a.t.i.
-00002d60: 6f00 6e00 7300 6b00 6f00 6e00 6600 6900  o.n.s.k.o.n.f.i.
-00002d70: 6700 7500 7200 6100 7400 6900 6f00 6e00  g.u.r.a.t.i.o.n.
-00002d80: 2000 6900 6e00 2000 5400 5100 5300 4c00   .i.n. .T.Q.S.L.
-00002d90: 2000 7600 6500 7200 6600 fc00 6700 6200   .v.e.r.f...g.b.
-00002da0: 6100 7208 0000 0000 0600 0000 254d 6973  a.r.........%Mis
-00002db0: 7369 6e67 2073 7461 7469 6f6e 2063 6f6e  sing station con
-00002dc0: 6669 6775 7261 7469 6f6e 2069 6e20 5451  figuration in TQ
-00002dd0: 534c 0700 0000 0944 7261 676f 6e4c 6f67  SL.....DragonLog
-00002de0: 0103 ffff ffff 0800 0000 0006 0000 0004  ................
-00002df0: 4d6f 6465 0700 0000 0944 7261 676f 6e4c  Mode.....DragonL
-00002e00: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
-00002e10: 0004 4e61 6d65 0700 0000 0944 7261 676f  ..Name.....Drago
-00002e20: 6e4c 6f67 0103 0000 0034 004b 0065 0069  nLog.....4.K.e.i
-00002e30: 006e 0065 0020 0051 0053 004f 0073 0020  .n.e. .Q.S.O.s. 
-00002e40: 0066 00fc 0072 0020 0064 0065 006e 0020  .f...r. .d.e.n. 
-00002e50: 004c 006f 0063 0061 0074 006f 0072 0800  .L.o.c.a.t.o.r..
-00002e60: 0000 0006 0000 0017 4e6f 2072 6563 6f72  ........No recor
-00002e70: 6473 2066 6f72 206c 6f63 6174 696f 6e07  ds for location.
-00002e80: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
-00002e90: 0000 0e00 4e00 6f00 7400 6900 7a00 6500  ....N.o.t.i.z.e.
-00002ea0: 6e08 0000 0000 0600 0000 054e 6f74 6573  n..........Notes
-00002eb0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00002ec0: ffff ffff 0800 0000 0006 0000 0002 4f6b  ..............Ok
-00002ed0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00002ee0: 0000 001e 0045 0069 0067 0065 006e 0065  .....E.i.g.e.n.e
-00002ef0: 0072 0020 004c 006f 0063 0061 0074 006f  .r. .L.o.c.a.t.o
-00002f00: 0072 0800 0000 0006 0000 000b 4f77 6e20  .r..........Own 
-00002f10: 4c6f 6361 746f 7207 0000 0009 4472 6167  Locator.....Drag
-00002f20: 6f6e 4c6f 6701 0300 0000 1800 4500 6900  onLog.......E.i.
-00002f30: 6700 6500 6e00 6500 7200 2000 4e00 6100  g.e.n.e.r. .N.a.
-00002f40: 6d00 6508 0000 0000 0600 0000 084f 776e  m.e..........Own
-00002f50: 204e 616d 6507 0000 0009 4472 6167 6f6e   Name.....Dragon
-00002f60: 4c6f 6701 0300 0000 1600 4500 6900 6700  Log.......E.i.g.
-00002f70: 6500 6e00 6500 7200 2000 5100 5400 4808  e.n.e.r. .Q.T.H.
-00002f80: 0000 0000 0600 0000 074f 776e 2051 5448  .........Own QTH
-00002f90: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00002fa0: 0000 0024 0045 0069 0067 0065 006e 0065  ...$.E.i.g.e.n.e
-00002fb0: 0073 0020 0052 0075 0066 007a 0065 0069  .s. .R.u.f.z.e.i
-00002fc0: 0063 0068 0065 006e 0800 0000 0006 0000  .c.h.e.n........
-00002fd0: 000d 4f77 6e20 6361 6c6c 2073 6967 6e07  ..Own call sign.
-00002fe0: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
-00002ff0: 0000 1000 4c00 6500 6900 7300 7400 7500  ....L.e.i.s.t.u.
-00003000: 6e00 6708 0000 0000 0600 0000 0550 6f77  n.g..........Pow
-00003010: 6572 0700 0000 0944 7261 676f 6e4c 6f67  er.....DragonLog
-00003020: 0103 0000 0016 0041 0075 0073 0062 0072  .......A.u.s.b.r
-00003030: 0065 0069 0074 0075 006e 0067 0800 0000  .e.i.t.u.n.g....
-00003040: 0006 0000 000b 5072 6f70 6167 6174 696f  ......Propagatio
-00003050: 6e07 0000 0009 4472 6167 6f6e 4c6f 6701  n.....DragonLog.
-00003060: 0300 0000 1a00 5100 5300 4c00 2d00 4e00  ......Q.S.L.-.N.
-00003070: 6100 6300 6800 7200 6900 6300 6800 7408  a.c.h.r.i.c.h.t.
-00003080: 0000 0000 0600 0000 0b51 534c 206d 6573  .........QSL mes
-00003090: 7361 6765 0700 0000 0944 7261 676f 6e4c  sage.....DragonL
-000030a0: 6f67 0103 0000 0010 0051 0053 004c 002d  og.......Q.S.L.-
-000030b0: 0050 0066 0061 0064 0800 0000 0006 0000  .P.f.a.d........
-000030c0: 0008 5153 4c20 7061 7468 0700 0000 0944  ..QSL path.....D
-000030d0: 7261 676f 6e4c 6f67 0103 0000 0012 0051  ragonLog.......Q
-000030e0: 0053 004c 0020 0065 006d 0070 0066 002e  .S.L. .e.m.p.f..
-000030f0: 0800 0000 0006 0000 0008 5153 4c20 7263  ..........QSL rc
-00003100: 7664 0700 0000 0944 7261 676f 6e4c 6f67  vd.....DragonLog
-00003110: 0103 0000 0012 0051 0053 004c 0020 0076  .......Q.S.L. .v
-00003120: 0065 0072 0073 002e 0800 0000 0006 0000  .e.r.s..........
-00003130: 0008 5153 4c20 7365 6e74 0700 0000 0944  ..QSL sent.....D
-00003140: 7261 676f 6e4c 6f67 0103 0000 000e 0051  ragonLog.......Q
-00003150: 0053 004c 002d 0056 0069 0061 0800 0000  .S.L.-.V.i.a....
-00003160: 0006 0000 0007 5153 4c20 7669 6107 0000  ......QSL via...
-00003170: 0009 4472 6167 6f6e 4c6f 6701 03ff ffff  ..DragonLog.....
-00003180: ff08 0000 0000 0600 0000 0351 534f 0700  ...........QSO..
-00003190: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
-000031a0: 0048 0051 0053 004f 002d 004c 006f 0067  .H.Q.S.O.-.L.o.g
-000031b0: 0020 0028 002a 002e 0071 006c 006f 0067  . .(.*...q.l.o.g
-000031c0: 0029 003b 003b 0041 006c 006c 0065 0020  .).;.;.A.l.l.e. 
-000031d0: 0044 0061 0074 0065 0069 0065 006e 0020  .D.a.t.e.i.e.n. 
-000031e0: 0028 002a 002e 002a 0029 0800 0000 0006  .(.*...*.)......
-000031f0: 0000 0021 5153 4f2d 4c6f 6720 282a 2e71  ...!QSO-Log (*.q
-00003200: 6c6f 6729 3b3b 416c 6c20 4669 6c65 7320  log);;All Files 
-00003210: 282a 2e2a 2907 0000 0009 4472 6167 6f6e  (*.*).....Dragon
-00003220: 4c6f 6701 03ff ffff ff08 0000 0000 0600  Log.............
-00003230: 0000 0351 5448 0700 0000 0944 7261 676f  ...QTH.....Drago
-00003240: 6e4c 6f67 0103 0000 0012 0052 0053 0054  nLog.......R.S.T
-00003250: 0020 0065 006d 0070 0066 002e 0800 0000  . .e.m.p.f......
-00003260: 0006 0000 0008 5253 5420 7263 7664 0700  ......RST rcvd..
-00003270: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
-00003280: 0010 0052 0053 0054 0020 0067 0065 0073  ...R.S.T. .g.e.s
-00003290: 002e 0800 0000 0006 0000 0008 5253 5420  ............RST 
-000032a0: 7365 6e74 0700 0000 0944 7261 676f 6e4c  sent.....DragonL
-000032b0: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
-000032c0: 0005 5261 6469 6f07 0000 0009 4472 6167  ..Radio.....Drag
-000032d0: 6f6e 4c6f 6701 0300 0000 1800 5200 6100  onLog.......R.a.
-000032e0: 6900 6e00 2d00 5300 6300 6100 7400 7400  i.n.-.S.c.a.t.t.
-000032f0: 6500 7208 0000 0000 0600 0000 0c52 6169  e.r..........Rai
-00003300: 6e20 7363 6174 7465 7207 0000 0009 4472  n scatter.....Dr
-00003310: 6167 6f6e 4c6f 6701 0300 0000 3200 5200  agonLog.....2.R.
-00003320: 6500 7000 6500 6100 7400 6500 7200 2000  e.p.e.a.t.e.r. .
-00003330: 6f00 6400 6500 7200 2000 5400 7200 6100  o.d.e.r. .T.r.a.
-00003340: 6e00 7300 7000 6f00 6e00 6400 6500 7208  n.s.p.o.n.d.e.r.
-00003350: 0000 0000 0600 0000 1752 6570 6561 7465  .........Repeate
-00003360: 7220 6f72 2054 7261 6e73 706f 6e64 6572  r or Transponder
-00003370: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00003380: 0000 0018 0045 006d 0070 0066 002e 0020  .....E.m.p.f... 
-00003390: 0051 0053 004f 0020 0049 0044 0800 0000  .Q.S.O. .I.D....
-000033a0: 0006 0000 0009 5278 2051 534f 2049 4407  ......Rx QSO ID.
-000033b0: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
-000033c0: 0000 1600 4500 6d00 7000 6600 2e00 2000  ....E.m.p.f... .
-000033d0: 4400 6100 7400 6500 6e08 0000 0000 0600  D.a.t.e.n.......
-000033e0: 0000 0752 7820 6461 7461 0700 0000 0944  ...Rx data.....D
-000033f0: 7261 676f 6e4c 6f67 0103 0000 0010 0053  ragonLog.......S
-00003400: 0061 0074 0065 006c 006c 0069 0074 0800  .a.t.e.l.l.i.t..
-00003410: 0000 0006 0000 0009 5361 7465 6c6c 6974  ........Satellit
-00003420: 6507 0000 0009 4472 6167 6f6e 4c6f 6701  e.....DragonLog.
-00003430: 0300 0000 2a00 4500 7800 7000 6f00 7200  ....*.E.x.p.o.r.
-00003440: 7400 6400 6100 7400 6500 6900 2000 7300  t.d.a.t.e.i. .s.
-00003450: 7000 6500 6900 6300 6800 6500 7200 6e08  p.e.i.c.h.e.r.n.
-00003460: 0000 0000 0600 0000 1253 656c 6563 7420  .........Select 
-00003470: 6578 706f 7274 2066 696c 6507 0000 0009  export file.....
-00003480: 4472 6167 6f6e 4c6f 6701 0300 0000 2000  DragonLog..... .
-00003490: 4400 6100 7400 6500 6e00 6200 6100 6e00  D.a.t.e.n.b.a.n.
-000034a0: 6b00 2000 f600 6600 6600 6e00 6500 6e08  k. ...f.f.n.e.n.
-000034b0: 0000 0000 0600 0000 0b53 656c 6563 7420  .........Select 
-000034c0: 6669 6c65 0700 0000 0944 7261 676f 6e4c  file.....DragonL
-000034d0: 6f67 0103 0000 0038 005a 0075 0020 00fc  og.....8.Z.u. ..
-000034e0: 0062 0065 0072 0077 0061 0063 0068 0065  .b.e.r.w.a.c.h.e
-000034f0: 006e 0064 0065 0020 0044 0061 0074 0065  .n.d.e. .D.a.t.e
-00003500: 0069 0020 0077 00e4 0068 006c 0065 006e  .i. .w...h.l.e.n
-00003510: 0800 0000 0006 0000 0014 5365 6c65 6374  ..........Select
-00003520: 2066 696c 6520 746f 2077 6174 6368 0700   file to watch..
-00003530: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
-00003540: 0024 0049 006d 0070 006f 0072 0074 0064  .$.I.m.p.o.r.t.d
-00003550: 0061 0074 0065 0069 0020 00f6 0066 0066  .a.t.e.i. ...f.f
-00003560: 006e 0065 006e 0800 0000 0006 0000 0012  .n.e.n..........
-00003570: 5365 6c65 6374 2069 6d70 6f72 7420 6669  Select import fi
-00003580: 6c65 0700 0000 0944 7261 676f 6e4c 6f67  le.....DragonLog
-00003590: 0103 0000 001a 0057 00e4 0068 006c 0065  .......W...h.l.e
-000035a0: 0020 0053 0074 0061 0074 0069 006f 006e  . .S.t.a.t.i.o.n
-000035b0: 0800 0000 0006 0000 000e 5365 6c65 6374  ..........Select
-000035c0: 2073 7461 7469 6f6e 0700 0000 0944 7261   station.....Dra
-000035d0: 676f 6e4c 6f67 0103 0000 0044 004c 006f  gonLog.....D.L.o
-000035e0: 0054 0057 002d 0053 0065 0072 0076 0065  .T.W.-.S.e.r.v.e
-000035f0: 0072 0020 0068 0061 0074 0020 0064 0061  .r. .h.a.t. .d.a
-00003600: 0073 0020 004c 006f 0067 0020 0061 0062  .s. .L.o.g. .a.b
-00003610: 0067 0065 0077 0069 0065 0073 0065 006e  .g.e.w.i.e.s.e.n
-00003620: 0800 0000 0006 0000 0013 5365 7276 6572  ..........Server
-00003630: 2072 656a 6563 7465 6420 6c6f 6707 0000   rejected log...
-00003640: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-00003650: 1400 7a00 6500 6900 6700 6500 2000 6100  ..z.e.i.g.e. .a.
-00003660: 6c00 6c00 6508 0000 0000 0600 0000 0853  l.l.e..........S
-00003670: 686f 7720 616c 6c07 0000 0009 4472 6167  how all.....Drag
-00003680: 6f6e 4c6f 6701 0300 0000 1400 5300 7000  onLog.......S.p.
-00003690: 6f00 7200 6100 6400 6900 6300 2d00 4508  o.r.a.d.i.c.-.E.
-000036a0: 0000 0000 0600 0000 0a53 706f 7261 6469  .........Sporadi
-000036b0: 6320 4507 0000 0009 4472 6167 6f6e 4c6f  c E.....DragonLo
-000036c0: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
-000036d0: 0753 7562 6d6f 6465 0700 0000 0944 7261  .Submode.....Dra
-000036e0: 676f 6e4c 6f67 0103 0000 002a 0054 0051  gonLog.....*.T.Q
-000036f0: 0053 004c 002d 0053 0069 0067 006e 0061  .S.L.-.S.i.g.n.a
-00003700: 0074 0075 0072 0070 0061 0073 0073 0077  .t.u.r.p.a.s.s.w
-00003710: 006f 0072 0074 0800 0000 0006 0000 0017  .o.r.t..........
-00003720: 5451 534c 2073 6967 6e61 7475 7265 2070  TQSL signature p
-00003730: 6173 7377 6f72 6407 0000 0009 4472 6167  assword.....Drag
-00003740: 6f6e 4c6f 6701 0300 0000 b200 4400 6900  onLog.......D.i.
-00003750: 6500 2000 4400 6100 7400 6500 6e00 6200  e. .D.a.t.e.n.b.
-00003760: 6100 6e00 6b00 7300 7400 7200 7500 6b00  a.n.k.s.t.r.u.k.
-00003770: 7400 7500 7200 2000 6900 7300 7400 2000  t.u.r. .i.s.t. .
-00003780: 7600 6500 7200 6100 6c00 7400 6500 7400  v.e.r.a.l.t.e.t.
-00003790: 2000 7500 6e00 6400 2000 6d00 7500 7300   .u.n.d. .m.u.s.
-000037a0: 7300 2000 6b00 6f00 6e00 7600 6500 7200  s. .k.o.n.v.e.r.
-000037b0: 7400 6900 6500 7200 7400 2000 7700 6500  t.i.e.r.t. .w.e.
-000037c0: 7200 6400 6500 6e00 0a00 0a00 4500 6900  r.d.e.n.....E.i.
-000037d0: 6e00 2000 4200 6100 6300 6b00 7500 7000  n. .B.a.c.k.u.p.
-000037e0: 2000 7700 6900 7200 6400 2000 6500 7200   .w.i.r.d. .e.r.
-000037f0: 7300 7400 6500 6c00 6c00 7400 3a08 0000  s.t.e.l.l.t.:...
-00003800: 0000 0600 0000 5754 6865 2064 6174 6162  ......WThe datab
-00003810: 6173 6520 7374 7275 6374 7572 6520 6973  ase structure is
-00003820: 206f 7574 2d64 6174 6564 2061 6e64 206e   out-dated and n
-00003830: 6565 6473 2061 2063 6f6e 7665 7273 696f  eeds a conversio
-00003840: 6e0a 0a41 2062 6163 6b75 7020 7769 6c6c  n..A backup will
-00003850: 2062 6520 6765 6e65 7261 7465 643a 0700   be generated:..
-00003860: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
-00003870: 001e 0054 0072 0061 006e 0073 0065 0071  ...T.r.a.n.s.e.q
-00003880: 0075 0061 0074 006f 0072 0069 0061 006c  .u.a.t.o.r.i.a.l
-00003890: 0800 0000 0006 0000 0010 5472 616e 732d  ..........Trans-
-000038a0: 6571 7561 746f 7269 616c 0700 0000 0944  equatorial.....D
-000038b0: 7261 676f 6e4c 6f67 0103 0000 0028 0054  ragonLog.....(.T
-000038c0: 0072 006f 0070 006f 0073 0070 0068 0065  .r.o.p.o.s.p.h.e
-000038d0: 0072 0069 0063 002d 0044 0075 0063 0074  .r.i.c.-.D.u.c.t
-000038e0: 0069 006e 0067 0800 0000 0006 0000 0014  .i.n.g..........
-000038f0: 5472 6f70 6f73 7068 6572 6963 2064 7563  Tropospheric duc
-00003900: 7469 6e67 0700 0000 0944 7261 676f 6e4c  ting.....DragonL
-00003910: 6f67 0103 0000 0016 0047 0065 0073 002e  og.......G.e.s..
-00003920: 0020 0051 0053 004f 0020 0049 0044 0800  . .Q.S.O. .I.D..
-00003930: 0000 0006 0000 0009 5478 2051 534f 2049  ........Tx QSO I
-00003940: 4407 0000 0009 4472 6167 6f6e 4c6f 6701  D.....DragonLog.
-00003950: 03ff ffff ff08 0000 0000 0600 0000 0756  ...............V
-00003960: 6572 7369 6f6e 0700 0000 0944 7261 676f  ersion.....Drago
-00003970: 6e4c 6f67 0103 0000 002c 0050 0072 006f  nLog.....,.P.r.o
-00003980: 0067 0072 0061 006d 006d 006c 006f 0067  .g.r.a.m.m.l.o.g
-00003990: 0020 00fc 0062 0065 0072 0077 0061 0063  . ...b.e.r.w.a.c
-000039a0: 0068 0065 006e 0800 0000 0006 0000 0015  .h.e.n..........
-000039b0: 5761 7463 6820 6170 706c 6963 6174 696f  Watch applicatio
-000039c0: 6e20 6c6f 6707 0000 0009 4472 6167 6f6e  n log.....Dragon
-000039d0: 4c6f 6701 0300 0000 2000 4400 6100 7400  Log..... .D.a.t.
-000039e0: 6500 6900 fc00 6200 6500 7200 7700 6100  e.i...b.e.r.w.a.
-000039f0: 6300 6800 7500 6e00 6708 0000 0000 0600  c.h.u.n.g.......
-00003a00: 0000 0d57 6174 6368 696e 6720 6669 6c65  ...Watching file
-00003a10: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00003a20: 0000 0014 0065 0051 0053 004c 0020 0065  .....e.Q.S.L. .e
-00003a30: 006d 0070 0066 002e 0800 0000 0006 0000  .m.p.f..........
-00003a40: 0009 6551 534c 2072 6376 6407 0000 0009  ..eQSL rcvd.....
-00003a50: 4472 6167 6f6e 4c6f 6701 0300 0000 1400  DragonLog.......
-00003a60: 6500 5100 5300 4c00 2000 7600 6500 7200  e.Q.S.L. .v.e.r.
-00003a70: 7300 2e08 0000 0000 0600 0000 0965 5153  s............eQS
-00003a80: 4c20 7365 6e74 0700 0000 0944 7261 676f  L sent.....Drago
-00003a90: 6e4c 6f67 0103 0000 000e 0069 006e 0061  nLog.......i.n.a
-00003aa0: 006b 0074 0069 0076 0800 0000 0006 0000  .k.t.i.v........
-00003ab0: 0007 696e 6163 7469 7607 0000 0009 4472  ..inactiv.....Dr
-00003ac0: 6167 6f6e 4c6f 6701 0300 0000 0c00 2800  agonLog.......(.
-00003ad0: 6c00 6500 6500 7200 2908 0000 0000 0600  l.e.e.r.).......
-00003ae0: 0000 0728 656d 7074 7929 0700 0000 084c  ...(empty).....L
-00003af0: 6973 7445 6469 7401 03ff ffff ff08 0000  istEdit.........
-00003b00: 0000 0600 0000 0446 6f72 6d07 0000 000c  .......Form.....
-00003b10: 4c69 7374 4564 6974 466f 726d 0103 ffff  ListEditForm....
-00003b20: ffff 0800 0000 0006 0000 0005 4c61 6265  ............Labe
-00003b30: 6c07 0000 000c 4c69 7374 4564 6974 466f  l.....ListEditFo
-00003b40: 726d 0103 0000 0008 00dc 0062 0065 0072  rm.........b.e.r
-00003b50: 0800 0000 0006 0000 0005 4162 6f75 7407  ..........About.
-00003b60: 0000 000a 4d61 696e 5769 6e64 6f77 0103  ....MainWindow..
-00003b70: 0000 000e 00dc 0062 0065 0072 0020 0051  .......b.e.r. .Q
-00003b80: 0074 0800 0000 0006 0000 0008 4162 6f75  .t..........Abou
-00003b90: 7420 5174 0700 0000 0a4d 6169 6e57 696e  t Qt.....MainWin
-00003ba0: 646f 7701 0300 0000 1a00 4100 6e00 7700  dow.......A.n.w.
-00003bb0: 6500 6e00 6400 7500 6e00 6700 7300 6c00  e.n.d.u.n.g.s.l.
-00003bc0: 6f00 6708 0000 0000 0600 0000 0f41 7070  o.g..........App
-00003bd0: 6c69 6361 7469 6f6e 204c 6f67 0700 0000  lication Log....
-00003be0: 0a4d 6169 6e57 696e 646f 7701 03ff ffff  .MainWindow.....
-00003bf0: ff08 0000 0000 0600 0000 0442 616e 6407  ...........Band.
-00003c00: 0000 000a 4d61 696e 5769 6e64 6f77 0103  ....MainWindow..
-00003c10: 0000 0014 0052 0075 0066 007a 0065 0069  .....R.u.f.z.e.i
-00003c20: 0063 0068 0065 006e 0800 0000 0006 0000  .c.h.e.n........
-00003c30: 0008 4361 6c6c 7369 676e 0700 0000 0a4d  ..Callsign.....M
-00003c40: 6169 6e57 696e 646f 7701 0300 0000 2200  ainWindow.....".
-00003c50: 4500 6900 6e00 7400 7200 6100 6700 2000  E.i.n.t.r.a.g. .
-00003c60: e400 6e00 6400 6500 7200 6e00 2e00 2e00  ..n.d.e.r.n.....
-00003c70: 2e08 0000 0000 0600 0000 1343 6861 6e67  ...........Chang
-00003c80: 6520 6c6f 6720 656e 7472 792e 2e2e 0700  e log entry.....
-00003c90: 0000 0a4d 6169 6e57 696e 646f 7701 03ff  ...MainWindow...
-00003ca0: ffff ff08 0000 0000 0600 0000 0643 7472  .............Ctr
-00003cb0: 6c2b 4507 0000 000a 4d61 696e 5769 6e64  l+E.....MainWind
-00003cc0: 6f77 0103 ffff ffff 0800 0000 0006 0000  ow..............
-00003cd0: 0006 4374 726c 2b46 0700 0000 0a4d 6169  ..Ctrl+F.....Mai
-00003ce0: 6e57 696e 646f 7701 03ff ffff ff08 0000  nWindow.........
-00003cf0: 0000 0600 0000 0643 7472 6c2b 4c07 0000  .......Ctrl+L...
-00003d00: 000a 4d61 696e 5769 6e64 6f77 0103 ffff  ..MainWindow....
-00003d10: ffff 0800 0000 0006 0000 0006 4374 726c  ............Ctrl
-00003d20: 2b51 0700 0000 0a4d 6169 6e57 696e 646f  +Q.....MainWindo
-00003d30: 7701 03ff ffff ff08 0000 0000 0600 0000  w...............
-00003d40: 0643 7472 6c2b 5707 0000 000a 4d61 696e  .Ctrl+W.....Main
-00003d50: 5769 6e64 6f77 0103 ffff ffff 0800 0000  Window..........
-00003d60: 0006 0000 0006 4374 726c 2b58 0700 0000  ......Ctrl+X....
-00003d70: 0a4d 6169 6e57 696e 646f 7701 0300 0000  .MainWindow.....
-00003d80: 1200 4400 6100 7400 7500 6d00 2000 7600  ..D.a.t.u.m. .v.
-00003d90: 6f00 6e08 0000 0000 0600 0000 0944 6174  o.n..........Dat
-00003da0: 6520 6672 6f6d 0700 0000 0a4d 6169 6e57  e from.....MainW
-00003db0: 696e 646f 7701 0300 0000 1200 4400 6100  indow.......D.a.
-00003dc0: 7400 7500 6d00 2000 6200 6900 7308 0000  t.u.m. .b.i.s...
-00003dd0: 0000 0600 0000 0744 6174 6520 746f 0700  .......Date to..
-00003de0: 0000 0a4d 6169 6e57 696e 646f 7701 0300  ...MainWindow...
-00003df0: 0000 1e00 4500 6900 6e00 7400 7200 6100  ....E.i.n.t.r.a.
-00003e00: 6700 2000 6c00 f600 7300 6300 6800 6500  g. .l...s.c.h.e.
-00003e10: 6e08 0000 0000 0600 0000 1044 656c 6574  n..........Delet
-00003e20: 6520 6c6f 6720 656e 7472 7907 0000 000a  e log entry.....
-00003e30: 4d61 696e 5769 6e64 6f77 0103 ffff ffff  MainWindow......
-00003e40: 0800 0000 0006 0000 0009 4472 6167 6f6e  ..........Dragon
-00003e50: 4c6f 6707 0000 000a 4d61 696e 5769 6e64  Log.....MainWind
-00003e60: 6f77 0103 0000 0014 0042 0065 0061 0072  ow.......B.e.a.r
-00003e70: 0062 0065 0069 0074 0065 006e 0800 0000  .b.e.i.t.e.n....
-00003e80: 0006 0000 0004 4564 6974 0700 0000 0a4d  ......Edit.....M
-00003e90: 6169 6e57 696e 646f 7701 0300 0000 0e00  ainWindow.......
-00003ea0: 4200 6500 6500 6e00 6400 6500 6e08 0000  B.e.e.n.d.e.n...
-00003eb0: 0000 0600 0000 0445 7869 7407 0000 000a  .......Exit.....
-00003ec0: 4d61 696e 5769 6e64 6f77 0103 ffff ffff  MainWindow......
-00003ed0: 0800 0000 0006 0000 0006 4578 706f 7274  ..........Export
-00003ee0: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
-00003ef0: 0300 0000 1c00 4500 7800 7000 6f00 7200  ......E.x.p.o.r.
-00003f00: 7400 6900 6500 7200 6500 6e00 2e00 2e00  t.i.e.r.e.n.....
-00003f10: 2e08 0000 0000 0600 0000 0945 7870 6f72  ...........Expor
-00003f20: 742e 2e2e 0700 0000 0a4d 6169 6e57 696e  t........MainWin
-00003f30: 646f 7701 0300 0000 0a00 4400 6100 7400  dow.......D.a.t.
-00003f40: 6500 6908 0000 0000 0600 0000 0446 696c  e.i..........Fil
-00003f50: 6507 0000 000a 4d61 696e 5769 6e64 6f77  e.....MainWindow
-00003f60: 0103 ffff ffff 0800 0000 0006 0000 0006  ................
-00003f70: 4669 6c74 6572 0700 0000 0a4d 6169 6e57  Filter.....MainW
-00003f80: 696e 646f 7701 0300 0000 0a00 4800 6900  indow.......H.i.
-00003f90: 6c00 6600 6508 0000 0000 0600 0000 0448  l.f.e..........H
-00003fa0: 656c 7007 0000 000a 4d61 696e 5769 6e64  elp.....MainWind
-00003fb0: 6f77 0103 ffff ffff 0800 0000 0006 0000  ow..............
-00003fc0: 0006 496d 706f 7274 0700 0000 0a4d 6169  ..Import.....Mai
-00003fd0: 6e57 696e 646f 7701 0300 0000 1c00 4900  nWindow.......I.
-00003fe0: 6d00 7000 6f00 7200 7400 6900 6500 7200  m.p.o.r.t.i.e.r.
-00003ff0: 6500 6e00 2e00 2e00 2e08 0000 0000 0600  e.n.............
-00004000: 0000 0949 6d70 6f72 742e 2e2e 0700 0000  ...Import.......
-00004010: 0a4d 6169 6e57 696e 646f 7701 0300 0000  .MainWindow.....
-00004020: 1800 4c00 6f00 6700 6700 6500 2000 5100  ..L.o.g.g.e. .Q.
-00004030: 5300 4f00 2e00 2e00 2e08 0000 0000 0600  S.O.............
-00004040: 0000 0a4c 6f67 2051 534f 2e2e 2e07 0000  ...Log QSO......
-00004050: 000a 4d61 696e 5769 6e64 6f77 0103 ffff  ..MainWindow....
-00004060: ffff 0800 0000 0006 0000 0004 4d6f 6465  ............Mode
-00004070: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
-00004080: 0300 0000 1800 5100 5300 4f00 2d00 4600  ......Q.S.O.-.F.
-00004090: 6f00 7200 6d00 7500 6c00 6100 7208 0000  o.r.m.u.l.a.r...
-000040a0: 0000 0600 0000 0851 534f 2046 6f72 6d07  .......QSO Form.
-000040b0: 0000 000a 4d61 696e 5769 6e64 6f77 0103  ....MainWindow..
-000040c0: 0000 0026 0044 0061 0074 0065 006e 0062  ...&.D.a.t.e.n.b
-000040d0: 0061 006e 006b 0020 0077 00e4 0068 006c  .a.n.k. .w...h.l
-000040e0: 0065 006e 002e 002e 002e 0800 0000 0006  .e.n............
-000040f0: 0000 0012 5365 6c65 6374 2064 6174 6162  ....Select datab
-00004100: 6173 652e 2e2e 0700 0000 0a4d 6169 6e57  ase........MainW
-00004110: 696e 646f 7701 0300 0000 1a00 4500 6900  indow.......E.i.
-00004120: 6e00 7300 7400 6500 6c00 6c00 7500 6e00  n.s.t.e.l.l.u.n.
-00004130: 6700 6500 6e08 0000 0000 0600 0000 0853  g.e.n..........S
-00004140: 6574 7469 6e67 7307 0000 000a 4d61 696e  ettings.....Main
-00004150: 5769 6e64 6f77 0103 0000 0024 005a 0065  Window.....$.Z.e
-00004160: 0069 0067 0065 0020 0046 0069 006c 0074  .i.g.e. .F.i.l.t
-00004170: 0065 0072 0064 0069 0061 006c 006f 0067  .e.r.d.i.a.l.o.g
-00004180: 0800 0000 0006 0000 000b 5368 6f77 2066  ..........Show f
-00004190: 696c 7465 7207 0000 000a 4d61 696e 5769  ilter.....MainWi
-000041a0: 6e64 6f77 0103 0000 0026 005a 0065 0069  ndow.....&.Z.e.i
-000041b0: 0067 0065 0020 0041 006e 0077 0065 006e  .g.e. .A.n.w.e.n
-000041c0: 0064 0075 006e 0067 0073 006c 006f 0067  .d.u.n.g.s.l.o.g
-000041d0: 0800 0000 0006 0000 0008 5368 6f77 206c  ..........Show l
-000041e0: 6f67 0700 0000 0a4d 6169 6e57 696e 646f  og.....MainWindo
-000041f0: 7701 0300 0000 1a00 5300 7400 6100 7200  w.......S.t.a.r.
-00004200: 7400 6500 2000 4800 6100 6d00 6c00 6900  t.e. .H.a.m.l.i.
-00004210: 6208 0000 0000 0600 0000 0c53 7461 7274  b..........Start
-00004220: 2068 616d 6c69 6207 0000 000a 4d61 696e   hamlib.....Main
-00004230: 5769 6e64 6f77 0103 0000 001c 0057 0065  Window.......W.e
-00004240: 0072 006b 007a 0065 0075 0067 006c 0065  .r.k.z.e.u.g.l.e
-00004250: 0069 0073 0074 0065 0800 0000 0006 0000  .i.s.t.e........
-00004260: 0007 546f 6f6c 6261 7207 0000 000a 4d61  ..Toolbar.....Ma
-00004270: 696e 5769 6e64 6f77 0103 0000 0032 004c  inWindow.....2.L
-00004280: 006f 0067 0073 0020 007a 0075 0020 004c  .o.g.s. .z.u. .L
-00004290: 006f 0054 0057 0020 0068 006f 0063 0068  .o.T.W. .h.o.c.h
-000042a0: 006c 0061 0064 0065 006e 002e 002e 002e  .l.a.d.e.n......
-000042b0: 0800 0000 0006 0000 0016 5570 6c6f 6164  ..........Upload
-000042c0: 206c 6f67 7320 746f 204c 6f54 572e 2e2e   logs to LoTW...
-000042d0: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
-000042e0: 0300 0000 4200 4400 6100 7400 6500 6900  ....B.D.a.t.e.i.
-000042f0: 2000 6100 7500 6600 2000 6e00 6500 7500   .a.u.f. .n.e.u.
-00004300: 6500 2000 5100 5300 4f00 7300 2000 fc00  e. .Q.S.O.s. ...
-00004310: 6200 6500 7200 7700 6100 6300 6800 6500  b.e.r.w.a.c.h.e.
-00004320: 6e00 2e00 2e00 2e08 0000 0000 0600 0000  n...............
-00004330: 1657 6174 6368 2066 696c 6520 666f 7220  .Watch file for 
-00004340: 5153 4f73 2e2e 2e07 0000 000a 4d61 696e  QSOs........Main
-00004350: 5769 6e64 6f77 0103 0000 0014 004a 004a  Window.......J.J
-00004360: 004a 004a 002d 004d 004d 002d 0054 0054  .J.J.-.M.M.-.T.T
-00004370: 0800 0000 0006 0000 000a 5959 5959 2d4d  ..........YYYY-M
-00004380: 4d2d 4444 0700 0000 0a4d 6169 6e57 696e  M-DD.....MainWin
-00004390: 646f 7701 03ff ffff ff08 0000 0000 0600  dow.............
-000043a0: 0000 0220 5707 0000 0007 5153 4f46 6f72  ... W.....QSOFor
-000043b0: 6d01 03ff ffff ff08 0000 0000 0600 0000  m...............
-000043c0: 0420 6b48 7a07 0000 0007 5153 4f46 6f72  . kHz.....QSOFor
-000043d0: 6d01 03ff ffff ff08 0000 0000 0600 0000  m...............
-000043e0: 0235 3907 0000 0007 5153 4f46 6f72 6d01  .59.....QSOForm.
-000043f0: 0300 0000 4800 4500 6900 6e00 2000 4600  ....H.E.i.n. .F.
-00004400: 6500 6c00 6400 2000 6600 6500 6800 6c00  e.l.d. .f.e.h.l.
-00004410: 7400 2000 6600 fc00 7200 2000 6400 6900  t. .f...r. .d.i.
-00004420: 6500 2000 4900 6e00 6200 6f00 7800 2d00  e. .I.n.b.o.x.-.
-00004430: 5000 7200 fc00 6600 7500 6e00 6708 0000  P.r...f.u.n.g...
-00004440: 0000 0600 0000 2241 2066 6965 6c64 2069  ......"A field i
-00004450: 7320 6d69 7373 696e 6720 666f 7220 696e  s missing for in
-00004460: 626f 7820 6368 6563 6b07 0000 0007 5153  box check.....QS
-00004470: 4f46 6f72 6d01 0300 0000 4200 4600 6500  OForm.....B.F.e.
-00004480: 6800 6c00 6500 6e00 6400 6500 7300 2000  h.l.e.n.d.e.s. .
-00004490: 4600 6500 6c00 6400 2000 6600 fc00 7200  F.e.l.d. .f...r.
-000044a0: 2000 6400 6500 6e00 2000 4c00 6f00 6700   .d.e.n. .L.o.g.
-000044b0: 2d00 5500 7000 6c00 6f00 6100 6408 0000  -.U.p.l.o.a.d...
-000044c0: 0000 0600 0000 2141 2066 6965 6c64 2069  ......!A field i
-000044d0: 7320 6d69 7373 696e 6720 666f 7220 6c6f  s missing for lo
-000044e0: 6720 7570 6c6f 6164 0700 0000 0751 534f  g upload.....QSO
-000044f0: 466f 726d 0103 0000 0056 0046 0065 0068  Form.....V.F.e.h
-00004500: 006c 0065 006e 0064 0065 0073 0020 0046  .l.e.n.d.e.s. .F
-00004510: 0065 006c 0064 0020 0066 00fc 0072 0020  .e.l.d. .f...r. 
-00004520: 0064 0065 006e 0020 004c 006f 0067 002d  .d.e.n. .L.o.g.-
-00004530: 0055 0070 006c 006f 0061 0064 0020 007a  .U.p.l.o.a.d. .z
-00004540: 0075 0020 0048 0061 006d 0051 0054 0048  .u. .H.a.m.Q.T.H
-00004550: 0800 0000 0006 0000 002b 4120 6669 656c  .........+A fiel
-00004560: 6420 6973 206d 6973 7369 6e67 2066 6f72  d is missing for
-00004570: 206c 6f67 2075 706c 6f61 6420 746f 2048   log upload to H
-00004580: 616d 5154 4807 0000 0007 5153 4f46 6f72  amQTH.....QSOFor
-00004590: 6d01 0300 0000 1600 4100 6b00 7a00 6500  m.......A.k.z.e.
-000045a0: 7000 7400 6900 6500 7200 7400 3a08 0000  p.t.i.e.r.t.:...
-000045b0: 0000 0600 0000 0841 6363 6570 7473 3a07  .......Accepts:.
-000045c0: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
-000045d0: 6a00 4500 6900 6e00 2000 4600 6500 6800  j.E.i.n. .F.e.h.
-000045e0: 6c00 6500 7200 2000 7400 7200 6100 7400  l.e.r. .t.r.a.t.
-000045f0: 2000 7700 e400 6800 7200 6500 6e00 6400   .w...h.r.e.n.d.
-00004600: 2000 6400 6500 7200 2000 dc00 6200 6500   .d.e.r. ...b.e.
-00004610: 7200 7400 7200 6100 6700 7500 6e00 6700  r.t.r.a.g.u.n.g.
-00004620: 2000 7a00 7500 2000 4800 6100 6d00 5100   .z.u. .H.a.m.Q.
-00004630: 5400 4800 2000 6100 7500 6608 0000 0000  T.H. .a.u.f.....
-00004640: 0600 0000 2741 6e20 6572 726f 7220 6f63  ....'An error oc
-00004650: 6375 7265 6420 6f6e 2075 706c 6f61 6469  cured on uploadi
-00004660: 6e67 2074 6f20 4861 6d51 5448 0700 0000  ng to HamQTH....
-00004670: 0751 534f 466f 726d 0103 0000 0016 0041  .QSOForm.......A
-00004680: 0075 0074 006f 006d 0061 0074 0069 0073  .u.t.o.m.a.t.i.s
-00004690: 0063 0068 0800 0000 0006 0000 000d 4175  .c.h..........Au
-000046a0: 746f 6d61 7469 6361 6c6c 7907 0000 0007  tomatically.....
-000046b0: 5153 4f46 6f72 6d01 0300 0000 3800 4600  QSOForm.....8.F.
-000046c0: 6500 6800 6c00 6500 7200 6800 6100 6600  e.h.l.e.r.h.a.f.
-000046d0: 7400 6500 7300 2000 4100 6200 6600 7200  t.e.s. .A.b.f.r.
-000046e0: 6100 6700 6500 6500 7200 6700 6500 6200  a.g.e.e.r.g.e.b.
-000046f0: 6e00 6900 7308 0000 0000 0600 0000 1242  n.i.s..........B
-00004700: 6164 2072 6571 7565 7374 2072 6573 756c  ad request resul
-00004710: 7407 0000 0007 5153 4f46 6f72 6d01 03ff  t.....QSOForm...
-00004720: ffff ff08 0000 0000 0600 0000 0442 616e  .............Ban
-00004730: 6407 0000 0007 5153 4f46 6f72 6d01 0300  d.....QSOForm...
-00004740: 0000 0800 4200 fc00 7200 6f08 0000 0000  ....B...r.o.....
-00004750: 0600 0000 0642 7572 6561 7507 0000 0007  .....Bureau.....
-00004760: 5153 4f46 6f72 6d01 0300 0000 1600 4200  QSOForm.......B.
-00004770: fc00 7200 6f00 2f00 4400 6900 7200 6500  ..r.o./.D.i.r.e.
-00004780: 6b00 7408 0000 0000 0600 0000 0d42 7572  k.t..........Bur
-00004790: 6561 752f 4469 7265 6374 0700 0000 0751  eau/Direct.....Q
-000047a0: 534f 466f 726d 0103 0000 0014 0052 0075  SOForm.......R.u
-000047b0: 0066 007a 0065 0069 0063 0068 0065 006e  .f.z.e.i.c.h.e.n
-000047c0: 0800 0000 0006 0000 0009 4361 6c6c 2073  ..........Call s
-000047d0: 6967 6e07 0000 0007 5153 4f46 6f72 6d01  ign.....QSOForm.
-000047e0: 0300 0000 3c00 4600 6500 6800 6c00 6500  ....<.F.e.h.l.e.
-000047f0: 7200 2000 6200 6500 6900 2000 6400 6500  r. .b.e.i. .d.e.
-00004800: 7200 2000 5200 7500 6600 7a00 6500 6900  r. .R.u.f.z.e.i.
-00004810: 6300 6800 6500 6e00 7300 7500 6300 6800  c.h.e.n.s.u.c.h.
-00004820: 6508 0000 0000 0600 0000 1543 616c 6c62  e..........Callb
-00004830: 6f6f 6b20 7365 6172 6368 2065 7272 6f72  ook search error
-00004840: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
-00004850: 002a 0043 0061 006c 006c 0062 006f 006f  .*.C.a.l.l.b.o.o
-00004860: 006b 002d 0053 0075 0063 0068 0065 0072  .k.-.S.u.c.h.e.r
-00004870: 0067 0065 0062 006e 0069 0073 0800 0000  .g.e.b.n.i.s....
-00004880: 0006 0000 0016 4361 6c6c 626f 6f6b 2073  ......Callbook s
-00004890: 6561 7263 6820 7265 7375 6c74 0700 0000  earch result....
-000048a0: 0751 534f 466f 726d 0103 0000 0032 0052  .QSOForm.....2.R
-000048b0: 0075 0066 007a 0065 0069 0063 0068 0065  .u.f.z.e.i.c.h.e
-000048c0: 006e 0020 006e 0069 0063 0068 0074 0020  .n. .n.i.c.h.t. 
-000048d0: 0067 0065 0066 0075 006e 0064 0065 006e  .g.e.f.u.n.d.e.n
-000048e0: 0800 0000 0006 0000 0012 4361 6c6c 7369  ..........Callsi
-000048f0: 676e 206e 6f74 2066 6f75 6e64 0700 0000  gn not found....
-00004900: 0751 534f 466f 726d 0103 0000 000a 004b  .QSOForm.......K
-00004910: 0061 006e 0061 006c 0800 0000 0006 0000  .a.n.a.l........
-00004920: 0007 4368 616e 6e65 6c07 0000 0007 5153  ..Channel.....QS
-00004930: 4f46 6f72 6d01 0300 0000 1600 5000 7200  OForm.......P.r.
-00004940: fc00 6600 6500 2000 4900 6e00 6200 6f00  ..f.e. .I.n.b.o.
-00004950: 7808 0000 0000 0600 0000 0b43 6865 636b  x..........Check
-00004960: 2049 6e62 6f78 0700 0000 0751 534f 466f   Inbox.....QSOFo
-00004970: 726d 0103 0000 0042 0046 0065 0068 006c  rm.....B.F.e.h.l
-00004980: 0065 0072 0020 0062 0065 0069 006d 0020  .e.r. .b.e.i.m. 
-00004990: 0050 0072 00fc 0066 0065 006e 0020 0064  .P.r...f.e.n. .d
-000049a0: 0065 0072 0020 004c 006f 0054 0057 002d  .e.r. .L.o.T.W.-
-000049b0: 0049 006e 0062 006f 0078 0800 0000 0006  .I.n.b.o.x......
-000049c0: 0000 0016 4368 6563 6b20 4c6f 5457 2049  ....Check LoTW I
-000049d0: 6e62 6f78 2065 7272 6f72 0700 0000 0751  nbox error.....Q
-000049e0: 534f 466f 726d 0103 0000 001c 0050 0072  SOForm.......P.r
-000049f0: 00fc 0066 0065 0020 004c 006f 0054 0057  ...f.e. .L.o.T.W
-00004a00: 0020 0051 0053 004c 0800 0000 0006 0000  . .Q.S.L........
-00004a10: 000e 4368 6563 6b20 4c6f 5457 2051 534c  ..Check LoTW QSL
-00004a20: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
-00004a30: 0038 0065 0051 0053 004c 002d 0046 0065  .8.e.Q.S.L.-.F.e
-00004a40: 0068 006c 0065 0072 0020 0070 0072 00fc  .h.l.e.r. .p.r..
-00004a50: 0066 0065 006e 0020 0064 0065 0072 0020  .f.e.n. .d.e.r. 
-00004a60: 0049 006e 0062 006f 0078 0800 0000 0006  .I.n.b.o.x......
-00004a70: 0000 0016 4368 6563 6b20 6551 534c 2049  ....Check eQSL I
-00004a80: 6e62 6f78 2065 7272 6f72 0700 0000 0751  nbox error.....Q
-00004a90: 534f 466f 726d 0103 0000 0018 005a 0075  SOForm.......Z.u
-00004aa0: 0072 00fc 0063 006b 0073 0065 0074 007a  .r...c.k.s.e.t.z
-00004ab0: 0065 006e 0800 0000 0006 0000 0005 436c  .e.n..........Cl
-00004ac0: 6561 7207 0000 0007 5153 4f46 6f72 6d01  ear.....QSOForm.
-00004ad0: 0300 0000 2000 4b00 6f00 6e00 6600 6900  .... .K.o.n.f.i.
-00004ae0: 6700 7500 7200 6900 6500 7200 7400 6500  g.u.r.i.e.r.t.e.
-00004af0: 2000 4900 4408 0000 0000 0600 0000 1343   .I.D..........C
-00004b00: 6f6e 6669 6775 7265 6420 6964 656e 7469  onfigured identi
-00004b10: 7479 0700 0000 0751 534f 466f 726d 0103  ty.....QSOForm..
-00004b20: 0000 002a 004b 006f 006e 0066 0069 0067  ...*.K.o.n.f.i.g
-00004b30: 0075 0072 0069 0065 0072 0074 0065 0020  .u.r.i.e.r.t.e. 
-00004b40: 0053 0074 0061 0074 0069 006f 006e 0800  .S.t.a.t.i.o.n..
-00004b50: 0000 0006 0000 0012 436f 6e66 6967 7572  ........Configur
-00004b60: 6564 2073 7461 7469 6f6e 0700 0000 0751  ed station.....Q
-00004b70: 534f 466f 726d 0103 ffff ffff 0800 0000  SOForm..........
-00004b80: 0006 0000 0007 436f 6e74 6573 7407 0000  ......Contest...
-00004b90: 0007 5153 4f46 6f72 6d01 03ff ffff ff08  ..QSOForm.......
-00004ba0: 0000 0000 0600 0000 0a43 6f6e 7465 7374  .........Contest
-00004bb0: 2049 4407 0000 0007 5153 4f46 6f72 6d01   ID.....QSOForm.
-00004bc0: 0300 0000 1600 4500 6d00 7000 6600 2e00  ......E.m.p.f...
-00004bd0: 2000 4400 6100 7400 6500 6e08 0000 0000   .D.a.t.e.n.....
-00004be0: 0600 0000 0444 6174 6107 0000 0007 5153  .....Data.....QS
-00004bf0: 4f46 6f72 6d01 0300 0000 0c00 6400 6900  OForm.......d.i.
-00004c00: 7200 6500 6b00 7408 0000 0000 0600 0000  r.e.k.t.........
-00004c10: 0644 6972 6563 7407 0000 0007 5153 4f46  .Direct.....QSOF
-00004c20: 6f72 6d01 0300 0000 1c00 6500 5100 5300  orm.......e.Q.S.
-00004c30: 4c00 2000 7300 7000 6500 6900 6300 6800  L. .s.p.e.i.c.h.
-00004c40: 6500 7200 6e08 0000 0000 0600 0000 0d44  e.r.n..........D
-00004c50: 6f77 6e6c 6f61 6420 6551 534c 0700 0000  ownload eQSL....
-00004c60: 0751 534f 466f 726d 0103 0000 006c 0057  .QSOForm.....l.W
-00004c70: 00e4 0068 0072 0065 006e 0064 0020 0064  ...h.r.e.n.d. .d
-00004c80: 0065 0072 0020 0052 0075 0066 007a 0065  .e.r. .R.u.f.z.e
-00004c90: 0069 0063 0068 0065 006e 0073 0075 0063  .i.c.h.e.n.s.u.c
-00004ca0: 0068 0065 0020 0069 0073 0074 0020 0065  .h.e. .i.s.t. .e
-00004cb0: 0069 006e 0020 0046 0065 0068 006c 0065  .i.n. .F.e.h.l.e
-00004cc0: 0072 0020 0061 0075 0066 0067 0065 0074  .r. .a.u.f.g.e.t
-00004cd0: 0072 0065 0074 0065 006e 0800 0000 0006  .r.e.t.e.n......
-00004ce0: 0000 0027 4475 7269 6e67 2063 616c 6c62  ...'During callb
-00004cf0: 6f6f 6b20 7365 6172 6368 2061 6e20 6572  ook search an er
-00004d00: 726f 7220 6f63 6375 7265 6407 0000 0007  ror occured.....
-00004d10: 5153 4f46 6f72 6d01 0300 0000 0800 4500  QSOForm.......E.
-00004d20: 6e00 6400 6508 0000 0000 0600 0000 0345  n.d.e..........E
-00004d30: 6e64 0700 0000 0751 534f 466f 726d 0103  nd.....QSOForm..
-00004d40: 0000 000c 0046 0065 0068 006c 0065 0072  .....F.e.h.l.e.r
-00004d50: 0800 0000 0006 0000 0005 4572 726f 7207  ..........Error.
-00004d60: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
-00004d70: 2400 6500 5100 5300 4c00 2d00 5500 7000  $.e.Q.S.L.-.U.p.
-00004d80: 6c00 6f00 6100 6400 2d00 4600 6500 6800  l.o.a.d.-.F.e.h.
-00004d90: 6c00 6500 7208 0000 0000 0600 0000 0f45  l.e.r..........E
-00004da0: 7272 6f72 206f 6e20 7570 6c6f 6164 0700  rror on upload..
-00004db0: 0000 0751 534f 466f 726d 0103 0000 0010  ...QSOForm......
-00004dc0: 0046 0072 0065 0071 0075 0065 006e 007a  .F.r.e.q.u.e.n.z
-00004dd0: 0800 0000 0006 0000 0009 4672 6571 7565  ..........Freque
-00004de0: 6e63 7907 0000 0007 5153 4f46 6f72 6d01  ncy.....QSOForm.
-00004df0: 03ff ffff ff08 0000 0000 0600 0000 0648  ...............H
-00004e00: 616d 5154 4807 0000 0007 5153 4f46 6f72  amQTH.....QSOFor
-00004e10: 6d01 0300 0000 0400 4900 4408 0000 0000  m.......I.D.....
-00004e20: 0600 0000 0849 6465 6e74 6974 7907 0000  .....Identity...
-00004e30: 0007 5153 4f46 6f72 6d01 0300 0000 2600  ..QSOForm.....&.
-00004e40: 4c00 6900 6e00 6b00 2000 7a00 7500 7200  L.i.n.k. .z.u.r.
-00004e50: 2000 6500 5100 5300 4c00 2d00 4b00 6100   .e.Q.S.L.-.K.a.
-00004e60: 7200 7400 6508 0000 0000 0600 0000 114c  r.t.e..........L
-00004e70: 696e 6b20 746f 2065 5153 4c20 4361 7264  ink to eQSL Card
-00004e80: 0700 0000 0751 534f 466f 726d 0103 ffff  .....QSOForm....
-00004e90: ffff 0800 0000 0006 0000 0004 4c6f 5457  ............LoTW
-00004ea0: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
-00004eb0: 001c 004c 006f 0054 0057 0020 0065 006d  ...L.o.T.W. .e.m
-00004ec0: 0070 0066 0061 006e 0067 0065 006e 0800  .p.f.a.n.g.e.n..
-00004ed0: 0000 0006 0000 000d 4c6f 5457 2072 6563  ........LoTW rec
-00004ee0: 6569 7665 6407 0000 0007 5153 4f46 6f72  eived.....QSOFor
-00004ef0: 6d01 0300 0000 1c00 4c00 6f00 5400 5700  m.......L.o.T.W.
-00004f00: 2000 7600 6500 7200 7300 6500 6e00 6400   .v.e.r.s.e.n.d.
-00004f10: 6500 7408 0000 0000 0600 0000 094c 6f54  e.t..........LoT
-00004f20: 5720 7365 6e74 0700 0000 0751 534f 466f  W sent.....QSOFo
-00004f30: 726d 0103 ffff ffff 0800 0000 0006 0000  rm..............
-00004f40: 0007 4c6f 6361 746f 7207 0000 0007 5153  ..Locator.....QS
-00004f50: 4f46 6f72 6d01 03ff ffff ff08 0000 0000  OForm...........
-00004f60: 0600 0000 074c 6f67 626f 6f6b 0700 0000  .....Logbook....
-00004f70: 0751 534f 466f 726d 0103 0000 0042 004c  .QSOForm.....B.L
-00004f80: 006f 0067 0069 006e 0020 0066 0065 0068  .o.g.i.n. .f.e.h
-00004f90: 006c 0067 0065 0073 0063 0068 006c 0061  .l.g.e.s.c.h.l.a
-00004fa0: 0067 0065 006e 0020 0066 00fc 0072 0020  .g.e.n. .f...r. 
-00004fb0: 0042 0065 006e 0075 0074 007a 0065 0072  .B.e.n.u.t.z.e.r
-00004fc0: 0800 0000 0006 0000 0015 4c6f 6769 6e20  ..........Login 
-00004fd0: 6661 696c 6564 2066 6f72 2075 7365 7207  failed for user.
-00004fe0: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
-00004ff0: 5800 4c00 6f00 6700 6900 6e00 2000 6200  X.L.o.g.i.n. .b.
-00005000: 6500 6900 2000 4800 6100 6d00 5100 5400  e.i. .H.a.m.Q.T.
-00005010: 4800 2000 6600 6500 6800 6c00 6700 6500  H. .f.e.h.l.g.e.
-00005020: 7300 6300 6800 6c00 6100 6700 6500 6e00  s.c.h.l.a.g.e.n.
-00005030: 2000 6600 fc00 7200 2000 4200 6500 6e00   .f...r. .B.e.n.
-00005040: 7500 7400 7a00 6500 7208 0000 0000 0600  u.t.z.e.r.......
-00005050: 0000 1f4c 6f67 696e 2074 6f20 4861 6d51  ...Login to HamQ
-00005060: 5448 2066 6169 6c65 6420 666f 7220 7573  TH failed for us
-00005070: 6572 0700 0000 0751 534f 466f 726d 0103  er.....QSOForm..
-00005080: 0000 0014 0048 0061 0075 0070 0074 0064  .....H.a.u.p.t.d
-00005090: 0061 0074 0065 006e 0800 0000 0006 0000  .a.t.e.n........
-000050a0: 0009 4d61 696e 2064 6174 6107 0000 0007  ..Main data.....
-000050b0: 5153 4f46 6f72 6d01 03ff ffff ff08 0000  QSOForm.........
-000050c0: 0000 0600 0000 044d 6f64 6507 0000 0007  .......Mode.....
-000050d0: 5153 4f46 6f72 6d01 03ff ffff ff08 0000  QSOForm.........
-000050e0: 0000 0600 0000 044e 616d 6507 0000 0007  .......Name.....
-000050f0: 5153 4f46 6f72 6d01 0300 0000 2400 4b00  QSOForm.....$.K.
-00005100: 6500 6900 6e00 2000 5100 5300 4c00 2000  e.i.n. .Q.S.L. .
-00005110: 7600 6500 7200 6600 fc00 6700 6200 6100  v.e.r.f...g.b.a.
-00005120: 7208 0000 0000 0600 0000 104e 6f20 5153  r..........No QS
-00005130: 4c20 6176 6169 6c61 626c 6507 0000 0007  L available.....
-00005140: 5153 4f46 6f72 6d01 0300 0000 2600 4b00  QSOForm.....&.K.
-00005150: 6500 6900 6e00 2000 6500 5100 5300 4c00  e.i.n. .e.Q.S.L.
-00005160: 2000 7600 6500 7200 6600 fc00 6700 6200   .v.e.r.f...g.b.
-00005170: 6100 7208 0000 0000 0600 0000 114e 6f20  a.r..........No 
-00005180: 6551 534c 2061 7661 696c 6162 6c65 0700  eQSL available..
-00005190: 0000 0751 534f 466f 726d 0103 0000 000a  ...QSOForm......
-000051a0: 004a 0065 0074 007a 0074 0800 0000 0006  .J.e.t.z.t......
-000051b0: 0000 0003 4e6f 7707 0000 0007 5153 4f46  ....Now.....QSOF
-000051c0: 6f72 6d01 0300 0000 1600 4500 6900 6700  orm.......E.i.g.
-000051d0: 6500 6e00 6500 7200 2000 5100 5400 4808  e.n.e.r. .Q.T.H.
-000051e0: 0000 0000 0600 0000 074f 776e 2051 5448  .........Own QTH
-000051f0: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
-00005200: 0024 0045 0069 0067 0065 006e 0065 0073  .$.E.i.g.e.n.e.s
-00005210: 0020 0052 0075 0066 007a 0065 0069 0063  . .R.u.f.z.e.i.c
-00005220: 0068 0065 006e 0800 0000 0006 0000 000d  .h.e.n..........
-00005230: 4f77 6e20 6361 6c6c 2073 6967 6e07 0000  Own call sign...
-00005240: 0007 5153 4f46 6f72 6d01 0300 0000 1e00  ..QSOForm.......
-00005250: 4500 6900 6700 6500 6e00 6500 7200 2000  E.i.g.e.n.e.r. .
-00005260: 4c00 6f00 6300 6100 7400 6f00 7208 0000  L.o.c.a.t.o.r...
-00005270: 0000 0600 0000 0b4f 776e 206c 6f63 6174  .......Own locat
-00005280: 6f72 0700 0000 0751 534f 466f 726d 0103  or.....QSOForm..
-00005290: 0000 0018 0045 0069 0067 0065 006e 0065  .....E.i.g.e.n.e
-000052a0: 0072 0020 004e 0061 006d 0065 0800 0000  .r. .N.a.m.e....
-000052b0: 0006 0000 0008 4f77 6e20 6e61 6d65 0700  ......Own name..
-000052c0: 0000 0751 534f 466f 726d 0103 0000 001c  ...QSOForm......
-000052d0: 0045 0069 0067 0065 006e 0065 0020 004e  .E.i.g.e.n.e. .N
-000052e0: 006f 0074 0069 007a 0065 006e 0800 0000  .o.t.i.z.e.n....
-000052f0: 0006 0000 0009 4f77 6e20 6e6f 7465 7307  ......Own notes.
-00005300: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
-00005310: 1000 4c00 6500 6900 7300 7400 7500 6e00  ..L.e.i.s.t.u.n.
-00005320: 6708 0000 0000 0600 0000 0550 6f77 6572  g..........Power
-00005330: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
-00005340: 001e 0041 0075 0073 0062 0072 0065 0069  ...A.u.s.b.r.e.i
-00005350: 0074 0075 006e 0067 0073 0061 0072 0074  .t.u.n.g.s.a.r.t
-00005360: 0800 0000 0006 0000 000b 5072 6f70 6167  ..........Propag
-00005370: 6174 696f 6e07 0000 0007 5153 4f46 6f72  ation.....QSOFor
-00005380: 6d01 03ff ffff ff08 0000 0000 0600 0000  m...............
-00005390: 0551 525a 4351 0700 0000 0751 534f 466f  .QRZCQ.....QSOFo
-000053a0: 726d 0103 ffff ffff 0800 0000 0006 0000  rm..............
-000053b0: 0003 5153 4c07 0000 0007 5153 4f46 6f72  ..QSL.....QSOFor
-000053c0: 6d01 0300 0000 2200 5100 5300 4c00 2000  m.....".Q.S.L. .
-000053d0: 2600 2600 2000 4c00 6f00 6700 2d00 5500  &.&. .L.o.g.-.U.
-000053e0: 7000 6c00 6f00 6100 6408 0000 0000 0600  p.l.o.a.d.......
-000053f0: 0000 1151 534c 2026 2620 4c6f 6720 7570  ...QSL && Log up
-00005400: 6c6f 6164 0700 0000 0751 534f 466f 726d  load.....QSOForm
-00005410: 0103 0000 001c 0051 0053 004c 002d 004b  .......Q.S.L.-.K
-00005420: 0061 0072 0074 0065 006e 0074 0065 0078  .a.r.t.e.n.t.e.x
-00005430: 0074 0800 0000 0006 0000 0010 5153 4c20  .t..........QSL 
-00005440: 6361 7264 206d 6573 7361 6765 0700 0000  card message....
-00005450: 0751 534f 466f 726d 0103 0000 001a 0051  .QSOForm.......Q
-00005460: 0053 004c 0020 0065 006d 0070 0066 0061  .S.L. .e.m.p.f.a
-00005470: 006e 0067 0065 006e 0800 0000 0006 0000  .n.g.e.n........
-00005480: 000c 5153 4c20 7265 6365 6976 6564 0700  ..QSL received..
-00005490: 0000 0751 534f 466f 726d 0103 0000 0018  ...QSOForm......
-000054a0: 0051 0053 004c 0020 0067 0065 0073 0065  .Q.S.L. .g.e.s.e
-000054b0: 006e 0064 0065 0074 0800 0000 0006 0000  .n.d.e.t........
-000054c0: 0008 5153 4c20 7365 6e74 0700 0000 0751  ..QSL sent.....Q
-000054d0: 534f 466f 726d 0103 0000 000e 0051 0053  SOForm.......Q.S
-000054e0: 004c 002d 0056 0069 0061 0800 0000 0006  .L.-.V.i.a......
-000054f0: 0000 0007 5153 4c20 7669 6107 0000 0007  ....QSL via.....
-00005500: 5153 4f46 6f72 6d01 0300 0000 1800 5100  QSOForm.......Q.
-00005510: 5300 4f00 2d00 4600 6f00 7200 6d00 7500  S.O.-.F.o.r.m.u.
-00005520: 6c00 6100 7208 0000 0000 0600 0000 0851  l.a.r..........Q
-00005530: 534f 2046 6f72 6d07 0000 0007 5153 4f46  SO Form.....QSOF
-00005540: 6f72 6d01 0300 0000 1a00 5100 5300 4f00  orm.......Q.S.O.
-00005550: 2d00 4b00 6f00 6d00 6d00 6500 6e00 7400  -.K.o.m.m.e.n.t.
-00005560: 6100 7208 0000 0000 0600 0000 0b51 534f  a.r..........QSO
-00005570: 2063 6f6d 6d65 6e74 0700 0000 0751 534f   comment.....QSO
-00005580: 466f 726d 0103 0000 003e 0051 0053 004f  Form.....>.Q.S.O
-00005590: 0020 0077 0075 0072 0064 0065 0020 0076  . .w.u.r.d.e. .v
-000055a0: 006f 006e 0020 0048 0061 006d 0051 0054  .o.n. .H.a.m.Q.T
-000055b0: 0048 0020 0061 0062 0067 0065 0077 0069  .H. .a.b.g.e.w.i
-000055c0: 0065 0073 0065 006e 0800 0000 0006 0000  .e.s.e.n........
-000055d0: 0016 5153 4f20 7265 6a65 6374 6564 206f  ..QSO rejected o
-000055e0: 6e20 4861 6d51 5448 0700 0000 0751 534f  n HamQTH.....QSO
-000055f0: 466f 726d 0103 ffff ffff 0800 0000 0006  Form............
-00005600: 0000 0003 5154 4807 0000 0007 5153 4f46  ....QTH.....QSOF
-00005610: 6f72 6d01 03ff ffff ff08 0000 0000 0600  orm.............
-00005620: 0000 0652 5354 2052 7807 0000 0007 5153  ...RST Rx.....QS
-00005630: 4f46 6f72 6d01 03ff ffff ff08 0000 0000  OForm...........
-00005640: 0600 0000 0652 5354 2054 7807 0000 0007  .....RST Tx.....
-00005650: 5153 4f46 6f72 6d01 0300 0000 1a00 5200  QSOForm.......R.
-00005660: 5300 5400 2000 6500 6d00 7000 6600 6100  S.T. .e.m.p.f.a.
-00005670: 6e00 6700 6500 6e08 0000 0000 0600 0000  n.g.e.n.........
-00005680: 0c52 5354 2072 6563 6569 7665 6407 0000  .RST received...
-00005690: 0007 5153 4f46 6f72 6d01 0300 0000 1800  ..QSOForm.......
-000056a0: 5200 5300 5400 2000 6700 6500 7300 6500  R.S.T. .g.e.s.e.
-000056b0: 6e00 6400 6500 7408 0000 0000 0600 0000  n.d.e.t.........
-000056c0: 0852 5354 2073 656e 7407 0000 0007 5153  .RST sent.....QS
-000056d0: 4f46 6f72 6d01 0300 0000 1800 4500 6d00  OForm.......E.m.
-000056e0: 7000 6600 2e00 2000 5100 5300 4f00 2000  p.f... .Q.S.O. .
-000056f0: 4900 4408 0000 0000 0600 0000 0b52 6376  I.D..........Rcv
-00005700: 6420 5153 4f20 4944 0700 0000 0751 534f  d QSO ID.....QSO
-00005710: 466f 726d 0103 0000 0012 0053 0070 0065  Form.......S.p.e
-00005720: 0069 0063 0068 0065 0072 006e 0800 0000  .i.c.h.e.r.n....
-00005730: 0006 0000 0004 5361 7665 0700 0000 0751  ......Save.....Q
-00005740: 534f 466f 726d 0103 0000 0026 0053 0070  SOForm.....&.S.p
-00005750: 0065 0069 0063 0068 0065 0072 006e 0020  .e.i.c.h.e.r.n. 
-00005760: 0026 0026 0020 0055 0070 006c 006f 0061  .&.&. .U.p.l.o.a
-00005770: 0064 0800 0000 0006 0000 000e 5361 7665  .d..........Save
-00005780: 2026 2620 5570 6c6f 6164 0700 0000 0751   && Upload.....Q
-00005790: 534f 466f 726d 0103 0000 002a 0065 0051  SOForm.....*.e.Q
-000057a0: 0053 004c 002d 004f 0072 0064 006e 0065  .S.L.-.O.r.d.n.e
-000057b0: 0072 0020 0061 0075 0073 0077 00e4 0068  .r. .a.u.s.w...h
-000057c0: 006c 0065 006e 0800 0000 0006 0000 0012  .l.e.n..........
-000057d0: 5365 6c65 6374 2065 5153 4c20 666f 6c64  Select eQSL fold
-000057e0: 6572 0700 0000 0751 534f 466f 726d 0103  er.....QSOForm..
-000057f0: 0000 0016 0047 0065 0073 002e 0020 0051  .....G.e.s... .Q
-00005800: 0053 004f 0020 0049 0044 0800 0000 0006  .S.O. .I.D......
-00005810: 0000 000b 5365 6e74 2051 534f 2049 4407  ....Sent QSO ID.
-00005820: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
-00005830: 3600 5300 6500 7200 7600 6500 7200 6b00  6.S.e.r.v.e.r.k.
-00005840: 6f00 6d00 6d00 7500 6e00 6900 6b00 6100  o.m.m.u.n.i.k.a.
-00005850: 7400 6900 6f00 6e00 7300 2d00 4600 6500  t.i.o.n.s.-.F.e.
-00005860: 6800 6c00 6500 7208 0000 0000 0600 0000  h.l.e.r.........
-00005870: 1a53 6572 7665 7220 636f 6d6d 756e 6963  .Server communic
-00005880: 6174 696f 6e20 6572 726f 7207 0000 0007  ation error.....
-00005890: 5153 4f46 6f72 6d01 03ff ffff ff08 0000  QSOForm.........
-000058a0: 0000 0600 0000 0553 7461 7274 0700 0000  .......Start....
-000058b0: 0751 534f 466f 726d 0103 ffff ffff 0800  .QSOForm........
-000058c0: 0000 0006 0000 0007 5374 6174 696f 6e07  ........Station.
-000058d0: 0000 0007 5153 4f46 6f72 6d01 03ff ffff  ....QSOForm.....
-000058e0: ff08 0000 0000 0600 0000 0753 7562 6d6f  ...........Submo
-000058f0: 6465 0700 0000 0751 534f 466f 726d 0103  de.....QSOForm..
-00005900: 0000 0030 0044 0061 0073 0020 0051 0053  ...0.D.a.s. .Q.S
-00005910: 004f 0020 0069 0073 0074 0020 0065 0069  .O. .i.s.t. .e.i
-00005920: 006e 0020 0044 0075 0070 006c 0069 006b  .n. .D.u.p.l.i.k
-00005930: 0061 0074 0800 0000 0006 0000 0016 5468  .a.t..........Th
-00005940: 6520 5153 4f20 6973 2061 2064 7570 6c69  e QSO is a dupli
-00005950: 6361 7465 0700 0000 0751 534f 466f 726d  cate.....QSOForm
-00005960: 0103 0000 00b8 0044 0069 0065 0020 0051  .......D.i.e. .Q
-00005970: 0053 004c 002d 0052 006f 0075 0074 0065  .S.L.-.R.o.u.t.e
-00005980: 0020 0064 0065 0072 0020 006b 006f 006e  . .d.e.r. .k.o.n
-00005990: 0074 0061 006b 0074 0069 0065 0072 0074  .t.a.k.t.i.e.r.t
-000059a0: 0065 006e 0020 0053 0074 0061 0074 0069  .e.n. .S.t.a.t.i
-000059b0: 006f 006e 002e 000a 0044 0069 0065 0073  .o.n.....D.i.e.s
-000059c0: 0020 0069 0073 0074 0020 006e 0069 0063  . .i.s.t. .n.i.c
-000059d0: 0068 0074 0020 0064 0069 0065 0020 0041  .h.t. .d.i.e. .A
-000059e0: 0064 0072 0065 0073 0073 0065 0020 0064  .d.r.e.s.s.e. .d
-000059f0: 0065 0073 0020 0051 0053 004c 002d 004d  .e.s. .Q.S.L.-.M
-00005a00: 0061 006e 0061 0067 0065 0072 0073 002f  .a.n.a.g.e.r.s./
-00005a10: 002d 0042 00fc 0072 006f 0073 002e 0800  .-.B...r.o.s....
-00005a20: 0000 0006 0000 004c 5468 6520 636f 6e74  .......LThe cont
-00005a30: 6163 7465 6420 7374 6174 696f 6e20 5153  acted station QS
-00005a40: 4c20 726f 7574 652e 0a54 6869 7320 6973  L route..This is
-00005a50: 206e 6f74 2074 6865 2051 534c 206d 616e   not the QSL man
-00005a60: 6167 6572 2f62 7572 6561 7520 6164 6472  ager/bureau addr
-00005a70: 6573 732e 0700 0000 0751 534f 466f 726d  ess......QSOForm
-00005a80: 0103 0000 0010 0045 006e 0064 0065 007a  .......E.n.d.e.z
-00005a90: 0065 0069 0074 0800 0000 0006 0000 0008  .e.i.t..........
-00005aa0: 5469 6d65 2065 6e64 0700 0000 0751 534f  Time end.....QSO
-00005ab0: 466f 726d 0103 0000 0012 0053 0074 0061  Form.......S.t.a
-00005ac0: 0072 0074 007a 0065 0069 0074 0800 0000  .r.t.z.e.i.t....
-00005ad0: 0006 0000 000a 5469 6d65 2073 7461 7274  ......Time start
-00005ae0: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
-00005af0: 0024 0065 0051 0053 004c 002d 0055 0070  .$.e.Q.S.L.-.U.p
-00005b00: 006c 006f 0061 0064 002d 0046 0065 0068  .l.o.a.d.-.F.e.h
-00005b10: 006c 0065 0072 0800 0000 0006 0000 0011  .l.e.r..........
-00005b20: 5570 6c6f 6164 2065 5153 4c20 6572 726f  Upload eQSL erro
-00005b30: 7207 0000 0007 5153 4f46 6f72 6d01 0300  r.....QSOForm...
-00005b40: 0000 1a00 5500 7000 6c00 6f00 6100 6400  ....U.p.l.o.a.d.
-00005b50: 2d00 4600 6500 6800 6c00 6500 7208 0000  -.F.e.h.l.e.r...
-00005b60: 0000 0600 0000 1055 706c 6f61 6420 6c6f  .......Upload lo
-00005b70: 6720 6572 726f 7207 0000 0007 5153 4f46  g error.....QSOF
-00005b80: 6f72 6d01 0300 0000 6800 5500 7000 6c00  orm.....h.U.p.l.
-00005b90: 6f00 6100 6400 2000 6500 7200 6600 6f00  o.a.d. .e.r.f.o.
-00005ba0: 6c00 6700 7400 2000 6e00 7500 7200 2000  l.g.t. .n.u.r. .
-00005bb0: 7700 6500 6e00 6e00 2000 6100 7500 6600  w.e.n.n. .a.u.f.
-00005bc0: 2000 6400 6500 7200 2000 5100 5300 4c00   .d.e.r. .Q.S.L.
-00005bd0: 2d00 5300 6500 6900 7400 6500 2000 6100  -.S.e.i.t.e. .a.
-00005be0: 7500 7300 6700 6500 7700 e400 6800 6c00  u.s.g.e.w...h.l.
-00005bf0: 7408 0000 0000 0600 0000 2455 706c 6f61  t.........$Uploa
-00005c00: 6473 206f 6e6c 7920 6966 2073 656c 6563  ds only if selec
-00005c10: 7465 6420 6f6e 2051 534c 2070 6167 6507  ted on QSL page.
-00005c20: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
-00005c30: 4800 4400 6500 7200 2000 4e00 7500 7400  H.D.e.r. .N.u.t.
-00005c40: 7a00 6500 7200 2000 4300 6100 6c00 6c00  z.e.r. .C.a.l.l.
-00005c50: 2000 7300 7400 6900 6d00 6d00 7400 2000   .s.t.i.m.m.t. .
-00005c60: 6e00 6900 6300 6800 7400 2000 fc00 6200  n.i.c.h.t. ...b.
-00005c70: 6500 7200 6500 6900 6e08 0000 0000 0600  e.r.e.i.n.......
-00005c80: 0000 1855 7365 7220 6361 6c6c 2064 6f65  ...User call doe
-00005c90: 7320 6e6f 7420 6d61 7463 6807 0000 0007  s not match.....
-00005ca0: 5153 4f46 6f72 6d01 03ff ffff ff08 0000  QSOForm.........
-00005cb0: 0000 0600 0000 0465 5153 4c07 0000 0007  .......eQSL.....
-00005cc0: 5153 4f46 6f72 6d01 0300 0000 1c00 6500  QSOForm.......e.
-00005cd0: 5100 5300 4c00 2000 6500 6d00 7000 6600  Q.S.L. .e.m.p.f.
-00005ce0: 6100 6e00 6700 6500 6e08 0000 0000 0600  a.n.g.e.n.......
-00005cf0: 0000 0d65 5153 4c20 7265 6365 6976 6564  ...eQSL received
-00005d00: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
-00005d10: 001a 0065 0051 0053 004c 0020 0067 0065  ...e.Q.S.L. .g.e
-00005d20: 0073 0065 006e 0064 0065 0074 0800 0000  .s.e.n.d.e.t....
-00005d30: 0006 0000 0009 6551 534c 2073 656e 7407  ......eQSL sent.
-00005d40: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
-00005d50: 0800 6b00 2e00 4100 2e08 0000 0000 0600  ..k...A.........
-00005d60: 0000 046e 2e61 2e07 0000 0007 5153 4f46  ...n.a......QSOF
-00005d70: 6f72 6d01 0300 0000 3400 7200 6900 6700  orm.....4.r.i.g.
-00005d80: 6300 7400 6c00 6400 2000 5a00 6500 6900  c.t.l.d. .Z.e.i.
-00005d90: 7400 fc00 6200 6500 7200 7300 6300 6800  t...b.e.r.s.c.h.
-00005da0: 7200 6500 6900 7400 7500 6e00 6708 0000  r.e.i.t.u.n.g...
-00005db0: 0000 0600 0000 0f72 6967 6374 6c64 2074  .......rigctld t
-00005dc0: 696d 656f 7574 0700 0000 0751 534f 466f  imeout.....QSOFo
-00005dd0: 726d 0103 ffff ffff 0800 0000 0006 0000  rm..............
-00005de0: 000a 7979 7979 2d4d 4d2d 6464 0700 0000  ..yyyy-MM-dd....
-00005df0: 0751 534f 466f 726d 0103 0000 0010 0041  .QSOForm.......A
-00005e00: 006e 0074 0065 006e 006e 0065 006e 0800  .n.t.e.n.n.e.n..
-00005e10: 0000 0006 0000 0008 416e 7465 6e6e 6173  ........Antennas
-00005e20: 0700 0000 0853 6574 7469 6e67 7301 0300  .....Settings...
-00005e30: 0000 7a00 4300 4100 5400 2d00 4500 6900  ..z.C.A.T.-.E.i.
-00005e40: 6e00 7300 7400 6500 6c00 6c00 7500 6e00  n.s.t.e.l.l.u.n.
-00005e50: 6700 2000 7700 7500 7200 6400 2000 6e00  g. .w.u.r.d. .n.
-00005e60: 6f00 6300 6800 2000 6e00 6900 6500 2000  o.c.h. .n.i.e. .
-00005e70: 6700 6500 7300 7000 6500 6900 6300 6800  g.e.s.p.e.i.c.h.
-00005e80: 6500 7200 7400 2000 6f00 7200 2000 5000  e.r.t. .o.r. .P.
-00005e90: 6100 7200 6100 6d00 6500 7400 6500 7200  a.r.a.m.e.t.e.r.
-00005ea0: 2000 6600 6500 6800 6c00 6500 6e08 0000   .f.e.h.l.e.n...
-00005eb0: 0000 0600 0000 3b43 4154 2063 6f6e 6669  ......;CAT confi
-00005ec0: 6775 7261 7469 6f6e 2077 6173 206e 6576  guration was nev
-00005ed0: 6572 2073 6176 6564 206f 7220 6120 7061  er saved or a pa
-00005ee0: 7261 6d65 7465 7220 6973 206d 6973 7369  rameter is missi
-00005ef0: 6e67 0700 0000 0853 6574 7469 6e67 7301  ng.....Settings.
-00005f00: 0300 0000 3000 4300 4100 5400 2d00 4500  ....0.C.A.T.-.E.
-00005f10: 6900 6e00 7300 7400 6500 6c00 6c00 7500  i.n.s.t.e.l.l.u.
-00005f20: 6e00 6700 6500 6e00 2000 4600 6500 6800  n.g.e.n. .F.e.h.
-00005f30: 6c00 6500 7208 0000 0000 0600 0000 1243  l.e.r..........C
-00005f40: 4154 2073 6574 7469 6e67 7320 6572 726f  AT settings erro
-00005f50: 7207 0000 0008 5365 7474 696e 6773 0103  r.....Settings..
-00005f60: 0000 002a 0048 0061 006d 006c 0069 0062  ...*.H.a.m.l.i.b
-00005f70: 0020 0072 0069 0067 0063 0074 006c 0064  . .r.i.g.c.t.l.d
-00005f80: 0020 0077 00e4 0068 006c 0065 006e 0800  . .w...h.l.e.n..
-00005f90: 0000 0006 0000 0020 4368 6f6f 7365 2068  ....... Choose h
-00005fa0: 616d 6c69 6220 7269 6763 746c 6420 6578  amlib rigctld ex
-00005fb0: 6563 7574 6162 6c65 0700 0000 0853 6574  ecutable.....Set
-00005fc0: 7469 6e67 7301 0300 0000 2000 4400 6100  tings..... .D.a.
-00005fd0: 7400 7500 6d00 2f00 5a00 6500 6900 7400  t.u.m./.Z.e.i.t.
-00005fe0: 2000 5300 7400 6100 7200 7408 0000 0000   .S.t.a.r.t.....
-00005ff0: 0600 0000 0f44 6174 652f 5469 6d65 2073  .....Date/Time s
-00006000: 7461 7274 0700 0000 0853 6574 7469 6e67  tart.....Setting
-00006010: 7301 0300 0000 4200 4600 6500 6800 6c00  s.....B.F.e.h.l.
-00006020: 6500 7200 2000 6200 6500 6900 6d00 2000  e.r. .b.e.i.m. .
-00006030: 4100 7500 7300 6600 fc00 6800 7200 6500  A.u.s.f...h.r.e.
-00006040: 6e00 2000 7600 6f00 6e00 2000 7200 6900  n. .v.o.n. .r.i.
-00006050: 6700 6300 7400 6c00 6408 0000 0000 0600  g.c.t.l.d.......
-00006060: 0000 1745 7272 6f72 2065 7865 6375 7469  ...Error executi
-00006070: 6e67 2072 6967 6374 6c64 0700 0000 0853  ng rigctld.....S
-00006080: 6574 7469 6e67 7301 03ff ffff ff08 0000  ettings.........
-00006090: 0000 0600 0000 0648 616d 6c69 6207 0000  .......Hamlib...
-000060a0: 0008 5365 7474 696e 6773 0103 0000 0014  ..Settings......
-000060b0: 0046 0075 006e 006b 0067 0065 0072 00e4  .F.u.n.k.g.e.r..
-000060c0: 0074 0065 0800 0000 0006 0000 0006 5261  .t.e..........Ra
-000060d0: 6469 6f73 0700 0000 0853 6574 7469 6e67  dios.....Setting
-000060e0: 7301 0300 0000 4e00 4400 6900 6500 2000  s.....N.D.i.e. .
-000060f0: 6700 6500 7700 e400 6800 6c00 7400 6500  g.e.w...h.l.t.e.
-00006100: 2000 4400 6100 7400 6500 6900 2000 6900   .D.a.t.e.i. .i.
-00006110: 7300 7400 2000 6e00 6900 6300 6800 7400  s.t. .n.i.c.h.t.
-00006120: 2000 6100 7500 7300 6600 fc00 6800 7200   .a.u.s.f...h.r.
-00006130: 6200 6100 7208 0000 0000 0600 0000 2353  b.a.r.........#S
-00006140: 656c 6563 7465 6420 6669 6c65 2069 7320  elected file is 
-00006150: 6e6f 7420 7468 6520 6578 6563 7574 6162  not the executab
-00006160: 6c65 0700 0000 0853 6574 7469 6e67 7301  le.....Settings.
-00006170: 0300 0000 1400 7a00 6500 6900 6700 6500  ......z.e.i.g.e.
-00006180: 2000 6100 6c00 6c00 6508 0000 0000 0600   .a.l.l.e.......
-00006190: 0000 0853 686f 7720 616c 6c07 0000 0008  ...Show all.....
-000061a0: 5365 7474 696e 6773 0103 ffff ffff 0800  Settings........
-000061b0: 0000 0006 0000 0005 5374 6172 7407 0000  ........Start...
-000061c0: 0008 5365 7474 696e 6773 0103 0000 001a  ..Settings......
-000061d0: 0053 0074 0061 0072 0074 0065 0020 0048  .S.t.a.r.t.e. .H
-000061e0: 0061 006d 006c 0069 0062 0800 0000 0006  .a.m.l.i.b......
-000061f0: 0000 000c 5374 6172 7420 6861 6d6c 6962  ....Start hamlib
-00006200: 0700 0000 0853 6574 7469 6e67 7301 03ff  .....Settings...
-00006210: ffff ff08 0000 0000 0600 0000 0453 746f  .............Sto
-00006220: 7007 0000 0008 5365 7474 696e 6773 0103  p.....Settings..
-00006230: 0000 001a 0053 0074 006f 0070 0070 0065  .....S.t.o.p.p.e
-00006240: 0020 0048 0061 006d 006c 0069 0062 0800  . .H.a.m.l.i.b..
-00006250: 0000 0006 0000 000b 5374 6f70 2068 616d  ........Stop ham
-00006260: 6c69 6207 0000 0008 5365 7474 696e 6773  lib.....Settings
-00006270: 0103 0000 000a 0061 006b 0074 0069 0076  .......a.k.t.i.v
-00006280: 0800 0000 0006 0000 0005 6163 7469 7607  ..........activ.
-00006290: 0000 0008 5365 7474 696e 6773 0103 0000  ....Settings....
-000062a0: 000e 0069 006e 0061 006b 0074 0069 0076  ...i.n.a.k.t.i.v
-000062b0: 0800 0000 0006 0000 0007 696e 6163 7469  ..........inacti
-000062c0: 7607 0000 0008 5365 7474 696e 6773 0103  v.....Settings..
-000062d0: 0000 004a 0072 0069 0067 0063 0074 006c  ...J.r.i.g.c.t.l
-000062e0: 0064 0020 006b 006f 006e 006e 0074 0065  .d. .k.o.n.n.t.e
-000062f0: 0020 006e 0069 0063 0068 0074 0020 0067  . .n.i.c.h.t. .g
-00006300: 0065 0073 0074 0061 0072 0074 0065 0074  .e.s.t.a.r.t.e.t
-00006310: 0020 0077 0065 0072 0064 0065 006e 0800  . .w.e.r.d.e.n..
-00006320: 0000 0006 0000 001e 7269 6763 746c 6420  ........rigctld 
-00006330: 6469 6420 6e6f 7420 7374 6172 7420 7072  did not start pr
-00006340: 6f70 6572 6c79 0700 0000 0853 6574 7469  operly.....Setti
-00006350: 6e67 7301 0300 0000 3600 7200 6900 6700  ngs.....6.r.i.g.
-00006360: 6300 7400 6c00 6400 2000 6900 7300 7400  c.t.l.d. .i.s.t.
-00006370: 2000 6e00 6900 6300 6800 7400 2000 7600   .n.i.c.h.t. .v.
-00006380: 6500 7200 6600 fc00 6700 6200 6100 7208  e.r.f...g.b.a.r.
-00006390: 0000 0000 0600 0000 1872 6967 6374 6c64  .........rigctld
-000063a0: 2069 7320 6e6f 7420 6176 6169 6c61 626c   is not availabl
-000063b0: 6507 0000 0008 5365 7474 696e 6773 0103  e.....Settings..
-000063c0: 0000 0010 0067 0065 00e4 006e 0064 0065  .....g.e...n.d.e
-000063d0: 0072 0074 0800 0000 0006 0000 0001 4d07  .r.t..........M.
-000063e0: 0000 0014 5472 616e 736c 6174 6564 5461  ....TranslatedTa
-000063f0: 626c 654d 6f64 656c 0103 0000 0008 004e  bleModel.......N
-00006400: 0065 0069 006e 0800 0000 0006 0000 0001  .e.i.n..........
-00006410: 4e07 0000 0014 5472 616e 736c 6174 6564  N.....Translated
-00006420: 5461 626c 654d 6f64 656c 0103 0000 0012  TableModel......
-00006430: 0061 006e 0067 0065 0066 0072 0061 0067  .a.n.g.e.f.r.a.g
-00006440: 0074 0800 0000 0006 0000 0001 5207 0000  .t..........R...
-00006450: 0014 5472 616e 736c 6174 6564 5461 626c  ..TranslatedTabl
-00006460: 654d 6f64 656c 0103 0000 0004 004a 0061  eModel.......J.a
-00006470: 0800 0000 0006 0000 0001 5907 0000 0014  ..........Y.....
-00006480: 5472 616e 736c 6174 6564 5461 626c 654d  TranslatedTableM
-00006490: 6f64 656c 0103 ffff ffff 0800 0000 0006  odel............
-000064a0: 0000 0007 4a53 3843 616c 6c07 0000 000f  ....JS8Call.....
-000064b0: 6170 7053 656c 6563 7444 6961 6c6f 6701  appSelectDialog.
-000064c0: 03ff ffff ff08 0000 0000 0600 0000 054f  ...............O
-000064d0: 7468 6572 0700 0000 0f61 7070 5365 6c65  ther.....appSele
-000064e0: 6374 4469 616c 6f67 0103 0000 002a 0041  ctDialog.....*.A
-000064f0: 0075 0073 0077 0061 0068 006c 0020 0064  .u.s.w.a.h.l. .d
-00006500: 0065 0073 0020 0050 0072 006f 0067 0072  .e.s. .P.r.o.g.r
-00006510: 0061 006d 006d 0073 0800 0000 0006 0000  .a.m.m.s........
-00006520: 0016 5365 6c65 6374 2074 6865 2061 7070  ..Select the app
-00006530: 6c69 6361 7469 6f6e 0700 0000 0f61 7070  lication.....app
-00006540: 5365 6c65 6374 4469 616c 6f67 0103 ffff  SelectDialog....
-00006550: ffff 0800 0000 0006 0000 0006 5753 4a54  ............WSJT
-00006560: 2d58 0700 0000 0f61 7070 5365 6c65 6374  -X.....appSelect
-00006570: 4469 616c 6f67 0103 ffff ffff 0800 0000  Dialog..........
-00006580: 0006 0000 0006 666c 6469 6769 0700 0000  ......fldigi....
-00006590: 0f61 7070 5365 6c65 6374 4469 616c 6f67  .appSelectDialog
-000065a0: 0188 0000 0002 0101                      ........
+00000c10: 0000 0006 0000 0005 3537 3630 3007 0000  ........57600...
+00000c20: 0006 4469 616c 6f67 0103 ffff ffff 0800  ..Dialog........
+00000c30: 0000 0006 0000 0004 3936 3030 0700 0000  ........9600....
+00000c40: 0644 6961 6c6f 6701 03ff ffff ff08 0000  .Dialog.........
+00000c50: 0000 0600 0000 013c 0700 0000 0644 6961  .......<.....Dia
+00000c60: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
+00000c70: 0000 013e 0700 0000 0644 6961 6c6f 6701  ...>.....Dialog.
+00000c80: 0300 0000 0e00 4100 6e00 7400 6500 6e00  ......A.n.t.e.n.
+00000c90: 6e00 6508 0000 0000 0600 0000 0741 6e74  n.e..........Ant
+00000ca0: 656e 6e61 0700 0000 0644 6961 6c6f 6701  enna.....Dialog.
+00000cb0: 0300 0000 1600 4100 7500 6600 7300 7400  ......A.u.f.s.t.
+00000cc0: 6500 6900 6700 6500 6e00 6408 0000 0000  e.i.g.e.n.d.....
+00000cd0: 0600 0000 0941 7363 656e 6469 6e67 0700  .....Ascending..
+00000ce0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
+00000cf0: 0000 0000 0600 0000 0343 4154 0700 0000  .........CAT....
+00000d00: 0644 6961 6c6f 6701 03ff ffff ff08 0000  .Dialog.........
+00000d10: 0000 0600 0000 0a43 422d 5374 6174 696f  .......CB-Statio
+00000d20: 6e07 0000 0006 4469 616c 6f67 0103 0000  n.....Dialog....
+00000d30: 0014 0052 0075 0066 007a 0065 0069 0063  ...R.u.f.z.e.i.c
+00000d40: 0068 0065 006e 0800 0000 0006 0000 0009  .h.e.n..........
+00000d50: 4361 6c6c 2073 6967 6e07 0000 0006 4469  Call sign.....Di
+00000d60: 616c 6f67 0103 ffff ffff 0800 0000 0006  alog............
+00000d70: 0000 0008 4361 6c6c 626f 6f6b 0700 0000  ....Callbook....
+00000d80: 0644 6961 6c6f 6701 0300 0000 3800 5a00  .Dialog.....8.Z.
+00000d90: 6500 7200 7400 6900 6600 6900 6b00 6100  e.r.t.i.f.i.k.a.
+00000da0: 7400 2000 6200 6500 6e00 f600 7400 6900  t. .b.e.n...t.i.
+00000db0: 6700 7400 2000 5000 6100 7300 7300 7700  g.t. .P.a.s.s.w.
+00000dc0: 6f00 7200 7408 0000 0000 0600 0000 1a43  o.r.t..........C
+00000dd0: 6572 7469 6669 6361 7465 206e 6565 6473  ertificate needs
+00000de0: 2070 6173 7377 6f72 6407 0000 0006 4469   password.....Di
+00000df0: 616c 6f67 0103 0000 0024 0053 0070 0061  alog.....$.S.p.a
+00000e00: 006c 0074 0065 006e 0020 0076 0065 0072  .l.t.e.n. .v.e.r
+00000e10: 0073 0074 0065 0063 006b 0065 006e 0800  .s.t.e.c.k.e.n..
+00000e20: 0000 0006 0000 000f 436f 6c75 6d6e 7320  ........Columns 
+00000e30: 746f 2068 6964 6507 0000 0006 4469 616c  to hide.....Dial
+00000e40: 6f67 0103 0000 0020 0053 0070 0061 006c  og..... .S.p.a.l
+00000e50: 0074 0065 006e 0020 0061 006e 007a 0065  .t.e.n. .a.n.z.e
+00000e60: 0069 0067 0065 006e 0800 0000 0006 0000  .i.g.e.n........
+00000e70: 000f 436f 6c75 6d6e 7320 746f 2073 686f  ..Columns to sho
+00000e80: 7707 0000 0006 4469 616c 6f67 0103 0000  w.....Dialog....
+00000e90: 0018 0041 006e 006d 0065 006c 0064 0065  ...A.n.m.e.l.d.e
+00000ea0: 0064 0061 0074 0065 006e 0800 0000 0006  .d.a.t.e.n......
+00000eb0: 0000 000b 4372 6564 656e 7469 616c 7307  ....Credentials.
+00000ec0: 0000 0006 4469 616c 6f67 0103 0000 0014  ....Dialog......
+00000ed0: 0041 0062 0073 0074 0065 0069 0067 0065  .A.b.s.t.e.i.g.e
+00000ee0: 006e 0064 0800 0000 0006 0000 000a 4465  .n.d..........De
+00000ef0: 7363 656e 6469 6e67 0700 0000 0644 6961  scending.....Dia
+00000f00: 6c6f 6701 0300 0000 3e00 5700 6900 7200  log.....>.W.i.r.
+00000f10: 6b00 7300 6100 6d00 2000 6e00 6100 6300  k.s.a.m. .n.a.c.
+00000f20: 6800 2000 4100 6e00 7700 6500 6e00 6400  h. .A.n.w.e.n.d.
+00000f30: 7500 6e00 6700 7300 6e00 6500 7500 7300  u.n.g.s.n.e.u.s.
+00000f40: 7400 6100 7200 7408 0000 0000 0600 0000  t.a.r.t.........
+00000f50: 2345 6666 6563 7469 7665 2061 6674 6572  #Effective after
+00000f60: 2061 7070 6c69 6361 7469 6f6e 2072 6573   application res
+00000f70: 7461 7274 0700 0000 0644 6961 6c6f 6701  tart.....Dialog.
+00000f80: 03ff ffff ff08 0000 0000 0600 0000 0645  ...............E
+00000f90: 7870 6f72 7407 0000 0006 4469 616c 6f67  xport.....Dialog
+00000fa0: 0103 0000 0034 0045 0078 0070 006f 0072  .....4.E.x.p.o.r
+00000fb0: 0074 0069 0065 0072 0065 0020 0043 0042  .t.i.e.r.e. .C.B
+00000fc0: 002d 0051 0053 004f 0073 0020 0069 006e  .-.Q.S.O.s. .i.n
+00000fd0: 0020 0041 0044 0049 0046 0800 0000 0006  . .A.D.I.F......
+00000fe0: 0000 0016 4578 706f 7274 2043 4220 5153  ....Export CB QS
+00000ff0: 4f73 2074 6f20 4144 4946 0700 0000 0644  Os to ADIF.....D
+00001000: 6961 6c6f 6701 0300 0000 3c00 4500 7800  ialog.....<.E.x.
+00001010: 7000 6f00 7200 7400 6900 6500 7200 6500  p.o.r.t.i.e.r.e.
+00001020: 2000 6e00 7500 7200 2000 6700 6500 6600   .n.u.r. .g.e.f.
+00001030: 6900 6c00 7400 6500 7200 7400 6500 2000  i.l.t.e.r.t.e. .
+00001040: 5100 5300 4f00 7308 0000 0000 0600 0000  Q.S.O.s.........
+00001050: 1745 7870 6f72 7420 6f6e 6c79 2072 6563  .Export only rec
+00001060: 656e 7420 5153 4f73 0700 0000 0644 6961  ent QSOs.....Dia
+00001070: 6c6f 6701 0300 0000 4200 4500 7800 7000  log.....B.E.x.p.
+00001080: 6f00 7200 7400 6900 6500 7200 6500 2000  o.r.t.i.e.r.e. .
+00001090: 6500 6900 6700 6500 6e00 6500 2000 4e00  e.i.g.e.n.e. .N.
+000010a0: 6f00 7400 6900 7a00 6500 6e00 2000 6900  o.t.i.z.e.n. .i.
+000010b0: 6e00 2000 4100 4400 4900 4608 0000 0000  n. .A.D.I.F.....
+000010c0: 0600 0000 1845 7870 6f72 7420 6f77 6e20  .....Export own 
+000010d0: 6e6f 7465 7320 746f 2041 4449 4607 0000  notes to ADIF...
+000010e0: 0006 4469 616c 6f67 0103 ffff ffff 0800  ..Dialog........
+000010f0: 0000 0006 0000 000e 4861 6d6c 6962 2072  ........Hamlib r
+00001100: 6967 6374 6c64 0700 0000 0644 6961 6c6f  igctld.....Dialo
+00001110: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
+00001120: 0d49 6d70 6f72 742f 4578 706f 7274 0700  .Import/Export..
+00001130: 0000 0644 6961 6c6f 6701 0300 0000 1a00  ...Dialog.......
+00001140: 5300 6300 6800 6e00 6900 7400 7400 7300  S.c.h.n.i.t.t.s.
+00001150: 7400 6500 6c00 6c00 6508 0000 0000 0600  t.e.l.l.e.......
+00001160: 0000 0949 6e74 6572 6661 6365 0700 0000  ...Interface....
+00001170: 0644 6961 6c6f 6701 0300 0000 2000 6c00  .Dialog..... .l.
+00001180: 6500 7400 7a00 7400 6500 7300 2000 4800  e.t.z.t.e.s. .H.
+00001190: 6100 6c00 6200 6a00 6100 6800 7208 0000  a.l.b.j.a.h.r...
+000011a0: 0000 0600 0000 0e4c 6173 7420 6861 6c66  .......Last half
+000011b0: 2079 6561 7207 0000 0006 4469 616c 6f67   year.....Dialog
+000011c0: 0103 0000 001a 006c 0065 0074 007a 0074  .......l.e.t.z.t
+000011d0: 0065 006e 0020 004d 006f 006e 0061 0074  .e.n. .M.o.n.a.t
+000011e0: 0800 0000 0006 0000 000a 4c61 7374 206d  ..........Last m
+000011f0: 6f6e 7468 0700 0000 0644 6961 6c6f 6701  onth.....Dialog.
+00001200: 0300 0000 1800 6c00 6500 7400 7a00 7400  ......l.e.t.z.t.
+00001210: 6500 2000 5700 6f00 6300 6800 6508 0000  e. .W.o.c.h.e...
+00001220: 0000 0600 0000 094c 6173 7420 7765 656b  .......Last week
+00001230: 0700 0000 0644 6961 6c6f 6701 0300 0000  .....Dialog.....
+00001240: 1800 6c00 6500 7400 7a00 7400 6500 7300  ..l.e.t.z.t.e.s.
+00001250: 2000 4a00 6100 6800 7208 0000 0000 0600   .J.a.h.r.......
+00001260: 0000 094c 6173 7420 7965 6172 0700 0000  ...Last year....
+00001270: 0644 6961 6c6f 6701 0300 0000 0a00 5300  .Dialog.......S.
+00001280: 7400 7500 6600 6508 0000 0000 0600 0000  t.u.f.e.........
+00001290: 054c 6576 656c 0700 0000 0644 6961 6c6f  .Level.....Dialo
+000012a0: 6701 0300 0000 0c00 4c00 6900 7300 7400  g.......L.i.s.t.
+000012b0: 6500 6e08 0000 0000 0600 0000 084c 6973  e.n..........Lis
+000012c0: 7469 6e67 7307 0000 0006 4469 616c 6f67  tings.....Dialog
+000012d0: 0103 ffff ffff 0800 0000 0006 0000 0004  ................
+000012e0: 4c6f 5457 0700 0000 0644 6961 6c6f 6701  LoTW.....Dialog.
+000012f0: 0300 0000 2c00 4c00 6f00 6700 2000 6900  ....,.L.o.g. .i.
+00001300: 6e00 2000 4400 6100 7400 6500 6900 2000  n. .D.a.t.e.i. .
+00001310: 7300 6300 6800 7200 6500 6900 6200 6500  s.c.h.r.e.i.b.e.
+00001320: 6e08 0000 0000 0600 0000 0b4c 6f67 2074  n..........Log t
+00001330: 6f20 6669 6c65 0700 0000 0644 6961 6c6f  o file.....Dialo
+00001340: 6701 0300 0000 1e00 4c00 6f00 6700 6700  g.......L.o.g.g.
+00001350: 6900 6e00 6700 2d00 4100 7500 7300 6700  i.n.g.-.A.u.s.g.
+00001360: 6100 6200 6508 0000 0000 0600 0000 0e4c  a.b.e..........L
+00001370: 6f67 6769 6e67 206f 7574 7075 7407 0000  ogging output...
+00001380: 0006 4469 616c 6f67 0103 ffff ffff 0800  ..Dialog........
+00001390: 0000 0006 0000 0004 4e61 6d65 0700 0000  ........Name....
+000013a0: 0644 6961 6c6f 6701 0300 0000 5e00 4300  .Dialog.....^.C.
+000013b0: 4200 2000 5100 5300 4f00 7300 2000 7700  B. .Q.S.O.s. .w.
+000013c0: 6500 7200 6400 6500 6e00 2000 6200 6500  e.r.d.e.n. .b.e.
+000013d0: 6900 6d00 2000 4900 6d00 7000 6f00 7200  i.m. .I.m.p.o.r.
+000013e0: 7400 2000 6900 6d00 6d00 6500 7200 2000  t. .i.m.m.e.r. .
+000013f0: 6200 6500 7200 fc00 6300 6b00 7300 6900  b.e.r...c.k.s.i.
+00001400: 6300 6800 7400 6900 6700 7408 0000 0000  c.h.t.i.g.t.....
+00001410: 0600 0000 284f 6e20 696d 706f 7274 2043  ....(On import C
+00001420: 4220 5153 4f73 2077 696c 6c20 616c 7761  B QSOs will alwa
+00001430: 7973 2062 6520 6861 6e64 6c65 6407 0000  ys be handled...
+00001440: 0006 4469 616c 6f67 0103 0000 0010 0050  ..Dialog.......P
+00001450: 0061 0073 0073 0077 006f 0072 0074 0800  .a.s.s.w.o.r.t..
+00001460: 0000 0006 0000 0008 5061 7373 776f 7264  ........Password
+00001470: 0700 0000 0644 6961 6c6f 6701 0300 0000  .....Dialog.....
+00001480: 7000 5000 6100 7300 7300 7700 6f00 7200  p.P.a.s.s.w.o.r.
+00001490: 7400 2000 6400 6500 7300 2000 4c00 6f00  t. .d.e.s. .L.o.
+000014a0: 5400 5700 2d00 4f00 6e00 6c00 6900 6e00  T.W.-.O.n.l.i.n.
+000014b0: 6500 2d00 4100 6300 6300 6f00 7500 6e00  e.-.A.c.c.o.u.n.
+000014c0: 7400 7300 2c00 2000 6e00 6900 6300 6800  t.s.,. .n.i.c.h.
+000014d0: 7400 2000 6400 6500 7300 2000 5a00 6500  t. .d.e.s. .Z.e.
+000014e0: 7200 7400 6900 6600 6900 6b00 6100 7400  r.t.i.f.i.k.a.t.
+000014f0: 7308 0000 0000 0600 0000 3850 6173 7377  s.........8Passw
+00001500: 6f72 6420 666f 7220 4c6f 5457 206f 6e6c  ord for LoTW onl
+00001510: 696e 6520 6163 636f 756e 7420 6e6f 7420  ine account not 
+00001520: 666f 7220 7468 6520 6365 7274 6966 6963  for the certific
+00001530: 6174 6507 0000 0006 4469 616c 6f67 0103  ate.....Dialog..
+00001540: ffff ffff 0800 0000 0006 0000 000d 5154  ..............QT
+00001550: 4820 284c 6f63 6174 6f72 2907 0000 0006  H (Locator).....
+00001560: 4469 616c 6f67 0103 ffff ffff 0800 0000  Dialog..........
+00001570: 0006 0000 0005 5261 6469 6f07 0000 0006  ......Radio.....
+00001580: 4469 616c 6f67 0103 0000 0018 004e 0065  Dialog.......N.e
+00001590: 0075 0065 0073 0074 0065 0020 0051 0053  .u.e.s.t.e. .Q.S
+000015a0: 004f 0073 0800 0000 0006 0000 000b 5265  .O.s..........Re
+000015b0: 6365 6e74 2051 534f 7307 0000 0006 4469  cent QSOs.....Di
+000015c0: 616c 6f67 0103 0000 0012 0046 0075 006e  alog.......F.u.n
+000015d0: 006b 0067 0065 0072 00e4 0074 0800 0000  .k.g.e.r...t....
+000015e0: 0006 0000 0003 5269 6707 0000 0006 4469  ......Rig.....Di
+000015f0: 616c 6f67 0103 0000 004c 0053 0069 0065  alog.....L.S.i.e
+00001600: 0068 0065 0020 0045 0069 006e 0073 0074  .h.e. .E.i.n.s.t
+00001610: 0065 006c 006c 0075 006e 0067 0065 006e  .e.l.l.u.n.g.e.n
+00001620: 0020 0052 0065 0069 0074 0065 0072 0020  . .R.e.i.t.e.r. 
+00001630: 0022 0041 006e 0077 0065 006e 0064 0075  .".A.n.w.e.n.d.u
+00001640: 006e 0067 0022 0800 0000 0006 0000 0022  .n.g."........."
+00001650: 5365 6520 7365 7474 696e 6773 2070 6167  See settings pag
+00001660: 6520 2255 7365 7220 696e 7465 7266 6163  e "User interfac
+00001670: 6522 0700 0000 0644 6961 6c6f 6701 0300  e".....Dialog...
+00001680: 0000 3400 4300 4200 2d00 4200 6100 6e00  ..4.C.B.-.B.a.n.
+00001690: 6400 2000 6100 7500 7400 6f00 6d00 6100  d. .a.u.t.o.m.a.
+000016a0: 7400 6900 7300 6300 6800 2000 7700 e400  t.i.s.c.h. .w...
+000016b0: 6800 6c00 6500 6e08 0000 0000 0600 0000  h.l.e.n.........
+000016c0: 1953 656c 6563 7420 4342 2062 616e 6420  .Select CB band 
+000016d0: 6279 2064 6566 6175 6c74 0700 0000 0644  by default.....D
+000016e0: 6961 6c6f 6701 0300 0000 0c00 4400 6900  ialog.......D.i.
+000016f0: 6500 6e00 7300 7408 0000 0000 0600 0000  e.n.s.t.........
+00001700: 0753 6572 7669 6365 0700 0000 0644 6961  .Service.....Dia
+00001710: 6c6f 6701 0300 0000 1a00 4500 6900 6e00  log.......E.i.n.
+00001720: 7300 7400 6500 6c00 6c00 7500 6e00 6700  s.t.e.l.l.u.n.g.
+00001730: 6500 6e08 0000 0000 0600 0000 0853 6574  e.n..........Set
+00001740: 7469 6e67 7307 0000 0006 4469 616c 6f67  tings.....Dialog
+00001750: 0103 0000 001c 005a 0065 0069 0067 0065  .......Z.e.i.g.e
+00001760: 0020 0051 0053 004f 0073 0020 0066 00fc  . .Q.S.O.s. .f..
+00001770: 0072 0800 0000 0006 0000 000e 5368 6f77  .r..........Show
+00001780: 2051 534f 7320 6672 6f6d 0700 0000 0644   QSOs from.....D
+00001790: 6961 6c6f 6701 0300 0000 1400 7a00 6500  ialog.......z.e.
+000017a0: 6900 6700 6500 2000 6100 6c00 6c00 6508  i.g.e. .a.l.l.e.
+000017b0: 0000 0000 0600 0000 0853 686f 7720 616c  .........Show al
+000017c0: 6c07 0000 0006 4469 616c 6f67 0103 0000  l.....Dialog....
+000017d0: 0040 0053 0070 0061 006c 0074 0065 006e  .@.S.p.a.l.t.e.n
+000017e0: 0020 0061 006e 007a 0065 0069 0067 0065  . .a.n.z.e.i.g.e
+000017f0: 006e 0020 006f 0064 0065 0072 0020 0076  .n. .o.d.e.r. .v
+00001800: 0065 0072 0073 0074 0065 0063 006b 0065  .e.r.s.t.e.c.k.e
+00001810: 006e 0800 0000 0006 0000 0014 5368 6f77  .n..........Show
+00001820: 206f 7220 6869 6465 2063 6f6c 756d 6e73   or hide columns
+00001830: 0700 0000 0644 6961 6c6f 6701 0300 0000  .....Dialog.....
+00001840: 2800 5300 6f00 7200 7400 6900 6500 7200  (.S.o.r.t.i.e.r.
+00001850: 6500 2000 6e00 6100 6300 6800 2000 5300  e. .n.a.c.h. .S.
+00001860: 7000 6100 6c00 7400 6508 0000 0000 0600  p.a.l.t.e.......
+00001870: 0000 0e53 6f72 7420 6f6e 2063 6f6c 756d  ...Sort on colum
+00001880: 6e07 0000 0006 4469 616c 6f67 0103 ffff  n.....Dialog....
+00001890: ffff 0800 0000 0006 0000 0005 5374 6172  ............Star
+000018a0: 7407 0000 0006 4469 616c 6f67 0103 ffff  t.....Dialog....
+000018b0: ffff 0800 0000 0006 0000 0007 5374 6174  ............Stat
+000018c0: 696f 6e07 0000 0006 4469 616c 6f67 0103  ion.....Dialog..
+000018d0: ffff ffff 0800 0000 0006 0000 0004 5451  ..............TQ
+000018e0: 534c 0700 0000 0644 6961 6c6f 6701 0300  SL.....Dialog...
+000018f0: 0000 6400 5600 6500 7200 7700 6500 6e00  ..d.V.e.r.w.e.n.
+00001900: 6400 6500 2000 6400 6900 6500 2000 6b00  d.e. .d.i.e. .k.
+00001910: 6f00 6e00 6600 6900 6700 7500 7200 6900  o.n.f.i.g.u.r.i.
+00001920: 6500 7200 7400 6500 2000 4900 4400 2000  e.r.t.e. .I.D. .
+00001930: 6200 6500 6900 2000 6600 6500 6800 6c00  b.e.i. .f.e.h.l.
+00001940: 6500 6e00 6400 6500 6e00 2000 5700 6500  e.n.d.e.n. .W.e.
+00001950: 7200 7400 6500 6e08 0000 0000 0600 0000  r.t.e.n.........
+00001960: 2455 7365 2063 6f6e 6669 6775 7265 6420  $Use configured 
+00001970: 4944 2066 6f72 206d 6973 7369 6e67 2076  ID for missing v
+00001980: 616c 7565 7307 0000 0006 4469 616c 6f67  alues.....Dialog
+00001990: 0103 0000 006e 0056 0065 0072 0077 0065  .....n.V.e.r.w.e
+000019a0: 006e 0064 0065 0020 0064 0069 0065 0020  .n.d.e. .d.i.e. 
+000019b0: 006b 006f 006e 0066 0069 0067 0075 0072  .k.o.n.f.i.g.u.r
+000019c0: 0069 0065 0072 0074 0065 0020 0053 0074  .i.e.r.t.e. .S.t
+000019d0: 0061 0074 0069 006f 006e 0020 0062 0065  .a.t.i.o.n. .b.e
+000019e0: 0069 0020 0066 0065 0068 006c 0065 006e  .i. .f.e.h.l.e.n
+000019f0: 0064 0065 006e 0020 0057 0065 0072 0074  .d.e.n. .W.e.r.t
+00001a00: 0065 006e 0800 0000 0006 0000 0029 5573  .e.n.........)Us
+00001a10: 6520 636f 6e66 6967 7572 6564 2053 7461  e configured Sta
+00001a20: 7469 6f6e 2066 6f72 206d 6973 7369 6e67  tion for missing
+00001a30: 2076 616c 7565 7307 0000 0006 4469 616c   values.....Dial
+00001a40: 6f67 0103 0000 0012 0041 006e 0077 0065  og.......A.n.w.e
+00001a50: 006e 0064 0075 006e 0067 0800 0000 0006  .n.d.u.n.g......
+00001a60: 0000 000e 5573 6572 2069 6e74 6572 6661  ....User interfa
+00001a70: 6365 0700 0000 0644 6961 6c6f 6701 0300  ce.....Dialog...
+00001a80: 0000 1800 4200 6500 6e00 7500 7400 7a00  ....B.e.n.u.t.z.
+00001a90: 6500 7200 6e00 6100 6d00 6508 0000 0000  e.r.n.a.m.e.....
+00001aa0: 0600 0000 0855 7365 726e 616d 6507 0000  .....Username...
+00001ab0: 0006 4469 616c 6f67 0103 0000 0078 0042  ..Dialog.....x.B
+00001ac0: 0065 006e 0075 0074 007a 0065 0072 006e  .e.n.u.t.z.e.r.n
+00001ad0: 0061 006d 0065 0020 0064 0065 0073 0020  .a.m.e. .d.e.s. 
+00001ae0: 004c 006f 0054 0057 002d 004f 006e 006c  .L.o.T.W.-.O.n.l
+00001af0: 0069 006e 0065 002d 0041 0063 0063 006f  .i.n.e.-.A.c.c.o
+00001b00: 0075 006e 0074 0073 002c 0020 006e 0069  .u.n.t.s.,. .n.i
+00001b10: 0063 0068 0074 0020 0064 0065 0073 0020  .c.h.t. .d.e.s. 
+00001b20: 005a 0065 0072 0074 0069 0066 0069 006b  .Z.e.r.t.i.f.i.k
+00001b30: 0061 0074 0073 0800 0000 0006 0000 0038  .a.t.s.........8
+00001b40: 5573 6572 6e61 6d65 2066 6f72 204c 6f54  Username for LoT
+00001b50: 5720 6f6e 6c69 6e65 2061 6363 6f75 6e74  W online account
+00001b60: 206e 6f74 2066 6f72 2074 6865 2063 6572   not for the cer
+00001b70: 7469 6669 6361 7465 0700 0000 0644 6961  tificate.....Dia
+00001b80: 6c6f 6701 0300 0000 2000 4400 6100 7400  log..... .D.a.t.
+00001b90: 6500 6900 fc00 6200 6500 7200 7700 6100  e.i...b.e.r.w.a.
+00001ba0: 6300 6800 7500 6e00 6708 0000 0000 0600  c.h.u.n.g.......
+00001bb0: 0000 0a57 6174 6368 2046 696c 6507 0000  ...Watch File...
+00001bc0: 0006 4469 616c 6f67 0103 ffff ffff 0800  ..Dialog........
+00001bd0: 0000 0006 0000 0004 6551 534c 0700 0000  ........eQSL....
+00001be0: 0644 6961 6c6f 6701 0300 0000 9e00 4500  .Dialog.......E.
+00001bf0: 6900 6e00 2000 4400 6100 7400 6500 6e00  i.n. .D.a.t.e.n.
+00001c00: 6200 6100 6e00 6b00 2d00 4200 6100 6300  b.a.n.k.-.B.a.c.
+00001c10: 6b00 7500 7000 2000 6b00 6f00 6e00 6e00  k.u.p. .k.o.n.n.
+00001c20: 7400 6500 2000 6e00 6900 6300 6800 7400  t.e. .n.i.c.h.t.
+00001c30: 2000 6500 7200 7300 7400 6500 6c00 6c00   .e.r.s.t.e.l.l.
+00001c40: 7400 2000 7700 6500 7200 6400 6500 6e00  t. .w.e.r.d.e.n.
+00001c50: 2e00 0a00 4400 6900 6500 2000 4400 6100  ....D.i.e. .D.a.
+00001c60: 7400 6500 6900 2000 6500 7800 6900 7300  t.e.i. .e.x.i.s.
+00001c70: 7400 6900 6500 7200 7400 2000 6200 6500  t.i.e.r.t. .b.e.
+00001c80: 7200 6500 6900 7400 7300 2e08 0000 0000  r.e.i.t.s.......
+00001c90: 0600 0000 4041 2064 6174 6162 6173 6520  ....@A database 
+00001ca0: 6261 636b 7570 2063 6f75 6c64 206e 6f74  backup could not
+00001cb0: 2062 6520 6372 6561 7465 642e 0a54 6865   be created..The
+00001cc0: 2066 696c 6520 616c 7265 6164 7920 6578   file already ex
+00001cd0: 6973 7473 2e07 0000 0009 4472 6167 6f6e  ists......Dragon
+00001ce0: 4c6f 6701 0300 0000 4e00 4500 6900 6e00  Log.....N.E.i.n.
+00001cf0: 2000 4100 4400 4900 4600 2d00 4600 6500   .A.D.I.F.-.F.e.
+00001d00: 6c00 6400 2000 6600 6500 6800 6c00 7400  l.d. .f.e.h.l.t.
+00001d10: 2000 6600 fc00 7200 2000 6400 6500 6e00   .f...r. .d.e.n.
+00001d20: 2000 4c00 6f00 5400 5700 2d00 5500 7000   .L.o.T.W.-.U.p.
+00001d30: 6c00 6f00 6100 6408 0000 0000 0600 0000  l.o.a.d.........
+00001d40: 1d41 2066 6965 6c64 2069 7320 6d69 7373  .A field is miss
+00001d50: 696e 6720 666f 7220 7570 6c6f 6164 0700  ing for upload..
+00001d60: 0000 0944 7261 676f 6e4c 6f67 0103 ffff  ...DragonLog....
+00001d70: ffff 0800 0000 0006 0000 0015 4144 4946  ............ADIF
+00001d80: 2033 2028 2a2e 6164 6920 2a2e 6164 6966   3 (*.adi *.adif
+00001d90: 2907 0000 0009 4472 6167 6f6e 4c6f 6701  ).....DragonLog.
+00001da0: 03ff ffff ff08 0000 0000 0600 0000 1b41  ...............A
+00001db0: 4449 4620 3320 282a 2e61 6478 202a 2e61  DIF 3 (*.adx *.a
+00001dc0: 6469 202a 2e61 6469 6629 0700 0000 0944  di *.adif).....D
+00001dd0: 7261 676f 6e4c 6f67 0103 0000 0008 00dc  ragonLog........
+00001de0: 0062 0065 0072 0800 0000 0006 0000 0005  .b.e.r..........
+00001df0: 4162 6f75 7407 0000 0009 4472 6167 6f6e  About.....Dragon
+00001e00: 4c6f 6701 0300 0000 0e00 dc00 6200 6500  Log.........b.e.
+00001e10: 7200 2000 5100 7408 0000 0000 0600 0000  r. .Q.t.........
+00001e20: 0841 626f 7574 2051 7407 0000 0009 4472  .About Qt.....Dr
+00001e30: 6167 6f6e 4c6f 6701 0300 0000 2000 4100  agonLog..... .A.
+00001e40: 6900 7200 6300 7200 6100 6600 7400 2d00  i.r.c.r.a.f.t.-.
+00001e50: 5300 6300 6100 7400 7400 6500 7208 0000  S.c.a.t.t.e.r...
+00001e60: 0000 0600 0000 1041 6972 6372 6166 7420  .......Aircraft 
+00001e70: 5363 6174 7465 7207 0000 0009 4472 6167  Scatter.....Drag
+00001e80: 6f6e 4c6f 6701 0300 0000 0e00 4100 6e00  onLog.......A.n.
+00001e90: 7400 6500 6e00 6e00 6508 0000 0000 0600  t.e.n.n.e.......
+00001ea0: 0000 0741 6e74 656e 6e61 0700 0000 0944  ...Antenna.....D
+00001eb0: 7261 676f 6e4c 6f67 0103 ffff ffff 0800  ragonLog........
+00001ec0: 0000 0006 0000 0006 4175 726f 7261 0700  ........Aurora..
+00001ed0: 0000 0944 7261 676f 6e4c 6f67 0103 ffff  ...DragonLog....
+00001ee0: ffff 0800 0000 0006 0000 0008 4175 726f  ............Auro
+00001ef0: 7261 2d45 0700 0000 0944 7261 676f 6e4c  ra-E.....DragonL
+00001f00: 6f67 0103 0000 000a 0041 0075 0074 006f  og.......A.u.t.o
+00001f10: 0072 0800 0000 0006 0000 0006 4175 7468  .r..........Auth
+00001f20: 6f72 0700 0000 0944 7261 676f 6e4c 6f67  or.....DragonLog
+00001f30: 0103 0000 0018 0042 0061 0063 006b 002d  .......B.a.c.k.-
+00001f40: 0053 0063 0061 0074 0074 0065 0072 0800  .S.c.a.t.t.e.r..
+00001f50: 0000 0006 0000 000c 4261 636b 2073 6361  ........Back sca
+00001f60: 7474 6572 0700 0000 0944 7261 676f 6e4c  tter.....DragonL
+00001f70: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
+00001f80: 0004 4261 6e64 0700 0000 0944 7261 676f  ..Band.....Drago
+00001f90: 6e4c 6f67 0103 0000 0022 0043 0053 0056  nLog.....".C.S.V
+00001fa0: 002d 0044 0061 0074 0065 0069 0020 0028  .-.D.a.t.e.i. .(
+00001fb0: 002a 002e 0063 0073 0076 0029 0800 0000  .*...c.s.v.)....
+00001fc0: 0006 0000 0010 4353 562d 4669 6c65 2028  ......CSV-File (
+00001fd0: 2a2e 6373 7629 0700 0000 0944 7261 676f  *.csv).....Drago
+00001fe0: 6e4c 6f67 0103 0000 0014 0052 0075 0066  nLog.......R.u.f
+00001ff0: 007a 0065 0069 0063 0068 0065 006e 0800  .z.e.i.c.h.e.n..
+00002000: 0000 0006 0000 0009 4361 6c6c 2073 6967  ........Call sig
+00002010: 6e07 0000 0009 4472 6167 6f6e 4c6f 6701  n.....DragonLog.
+00002020: 0300 0000 0a00 4b00 6100 6e00 6100 6c08  ......K.a.n.a.l.
+00002030: 0000 0000 0600 0000 0743 6861 6e6e 656c  .........Channel
+00002040: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00002050: 0000 0074 0050 0072 00fc 0066 0075 006e  ...t.P.r...f.u.n
+00002060: 0067 0020 0064 0065 0072 0020 0044 0061  .g. .d.e.r. .D.a
+00002070: 0074 0065 006e 0062 0061 006e 006b 0020  .t.e.n.b.a.n.k. 
+00002080: 0066 0065 0068 006c 0067 0065 0073 0063  .f.e.h.l.g.e.s.c
+00002090: 0068 006c 0061 0067 0065 006e 002e 0020  .h.l.a.g.e.n... 
+000020a0: 0049 006e 0068 0061 006c 0074 0020 006e  .I.n.h.a.l.t. .n
+000020b0: 0069 0063 0068 0074 0020 006c 0065 0073  .i.c.h.t. .l.e.s
+000020c0: 0062 0061 0072 002e 0800 0000 0006 0000  .b.a.r..........
+000020d0: 0034 4368 6563 6b69 6e67 2064 6174 6162  .4Checking datab
+000020e0: 6173 6520 6661 696c 6564 2e20 436f 6e74  ase failed. Cont
+000020f0: 656e 7420 6973 206e 6f74 2061 6363 6573  ent is not acces
+00002100: 7361 626c 652e 0700 0000 0944 7261 676f  sable......Drago
+00002110: 6e4c 6f67 0103 0000 0012 004b 006f 006d  nLog.......K.o.m
+00002120: 006d 0065 006e 0074 0061 0072 0800 0000  .m.e.n.t.a.r....
+00002130: 0006 0000 0007 436f 6d6d 656e 7407 0000  ......Comment...
+00002140: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+00002150: 6000 5600 6500 7200 6200 6900 6e00 6400  `.V.e.r.b.i.n.d.
+00002160: 7500 6e00 6700 7300 6600 6500 6800 6c00  u.n.g.s.f.e.h.l.
+00002170: 6500 7200 2000 6f00 6400 6500 7200 2000  e.r. .o.d.e.r. .
+00002180: 4e00 6500 7400 7a00 7700 6500 7200 6b00  N.e.t.z.w.e.r.k.
+00002190: 2000 6e00 6900 6300 6800 7400 2000 6500   .n.i.c.h.t. .e.
+000021a0: 7200 7200 6500 6900 6300 6800 6200 6100  r.r.e.i.c.h.b.a.
+000021b0: 7208 0000 0000 0600 0000 2743 6f6e 6e65  r.........'Conne
+000021c0: 6374 696f 6e20 6572 726f 7220 6f72 206e  ction error or n
+000021d0: 6574 776f 726b 2075 6e72 6561 6368 6162  etwork unreachab
+000021e0: 6c65 0700 0000 0944 7261 676f 6e4c 6f67  le.....DragonLog
+000021f0: 0103 ffff ffff 0800 0000 0006 0000 0007  ................
+00002200: 436f 6e74 6573 7407 0000 0009 4472 6167  Contest.....Drag
+00002210: 6f6e 4c6f 6701 0300 0000 2e00 4400 6100  onLog.......D.a.
+00002220: 7400 6500 6e00 6200 6100 6e00 6b00 2d00  t.e.n.b.a.n.k.-.
+00002230: 4200 6100 6300 6b00 7500 7000 2000 4600  B.a.c.k.u.p. .F.
+00002240: 6500 6800 6c00 6500 7208 0000 0000 0600  e.h.l.e.r.......
+00002250: 0000 1544 6174 6162 6173 6520 6261 636b  ...Database back
+00002260: 7570 2065 7272 6f72 0700 0000 0944 7261  up error.....Dra
+00002270: 676f 6e4c 6f67 0103 0000 002c 0044 0061  gonLog.....,.D.a
+00002280: 0074 0065 006e 0062 0061 006e 006b 006b  .t.e.n.b.a.n.k.k
+00002290: 006f 006e 0076 0065 0072 0074 0069 0065  .o.n.v.e.r.t.i.e
+000022a0: 0072 0075 006e 0067 0800 0000 0006 0000  .r.u.n.g........
+000022b0: 0013 4461 7461 6261 7365 2063 6f6e 7665  ..Database conve
+000022c0: 7273 696f 6e07 0000 0009 4472 6167 6f6e  rsion.....Dragon
+000022d0: 4c6f 6701 0300 0000 4800 4400 6100 7400  Log.....H.D.a.t.
+000022e0: 6500 6e00 6200 6100 6e00 6b00 6b00 6f00  e.n.b.a.n.k.k.o.
+000022f0: 6e00 7600 6500 7200 7400 6900 6500 7200  n.v.e.r.t.i.e.r.
+00002300: 7500 6e00 6700 2000 6100 6200 6700 6500  u.n.g. .a.b.g.e.
+00002310: 7300 6300 6800 6c00 6f00 7300 7300 6500  s.c.h.l.o.s.s.e.
+00002320: 6e08 0000 0000 0600 0000 1c44 6174 6162  n..........Datab
+00002330: 6173 6520 636f 6e76 6572 7369 6f6e 2066  ase conversion f
+00002340: 696e 6973 6865 6407 0000 0009 4472 6167  inished.....Drag
+00002350: 6f6e 4c6f 6701 0300 0000 1e00 4400 6100  onLog.......D.a.
+00002360: 7400 6500 6e00 6200 6100 6e00 6b00 6600  t.e.n.b.a.n.k.f.
+00002370: 6500 6800 6c00 6500 7208 0000 0000 0600  e.h.l.e.r.......
+00002380: 0000 0e44 6174 6162 6173 6520 6572 726f  ...Database erro
+00002390: 7207 0000 0009 4472 6167 6f6e 4c6f 6701  r.....DragonLog.
+000023a0: 0300 0000 3400 4400 6100 7400 6500 6e00  ....4.D.a.t.e.n.
+000023b0: 6200 6100 6e00 6b00 7300 7400 7200 7500  b.a.n.k.s.t.r.u.
+000023c0: 6b00 7400 7500 7200 2000 7600 6500 7200  k.t.u.r. .v.e.r.
+000023d0: 6100 6c00 7400 6500 7408 0000 0000 0600  a.l.t.e.t.......
+000023e0: 0000 1c44 6174 6162 6173 6520 7374 7275  ...Database stru
+000023f0: 6374 7572 6520 6f75 742d 6461 7465 6407  cture out-dated.
+00002400: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
+00002410: 0000 1e00 4400 6100 7400 7500 6d00 2f00  ....D.a.t.u.m./.
+00002420: 5a00 6500 6900 7400 2000 4500 6e00 6400  Z.e.i.t. .E.n.d.
+00002430: 6508 0000 0000 0600 0000 0d44 6174 652f  e..........Date/
+00002440: 5469 6d65 2065 6e64 0700 0000 0944 7261  Time end.....Dra
+00002450: 676f 6e4c 6f67 0103 0000 0020 0044 0061  gonLog..... .D.a
+00002460: 0074 0075 006d 002f 005a 0065 0069 0074  .t.u.m./.Z.e.i.t
+00002470: 0020 0053 0074 0061 0072 0074 0800 0000  . .S.t.a.r.t....
+00002480: 0006 0000 000f 4461 7465 2f54 696d 6520  ......Date/Time 
+00002490: 7374 6172 7407 0000 0009 4472 6167 6f6e  start.....Dragon
+000024a0: 4c6f 6701 0300 0000 1600 5100 5300 4f00  Log.......Q.S.O.
+000024b0: 2000 6c00 f600 7300 6300 6800 6500 6e08   .l...s.c.h.e.n.
+000024c0: 0000 0000 0600 0000 0a44 656c 6574 6520  .........Delete 
+000024d0: 5153 4f07 0000 0009 4472 6167 6f6e 4c6f  QSO.....DragonLo
+000024e0: 6701 0300 0000 1400 4500 6e00 7400 6600  g.......E.n.t.f.
+000024f0: 6500 7200 6e00 7500 6e00 6708 0000 0000  e.r.n.u.n.g.....
+00002500: 0600 0000 0844 6973 7461 6e63 6507 0000  .....Distance...
+00002510: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+00002520: 6400 5700 6f00 6c00 6c00 6500 6e00 2000  d.W.o.l.l.e.n. .
+00002530: 7300 6900 6500 2000 6400 6900 6500 2000  s.i.e. .d.i.e. .
+00002540: 7300 6500 6c00 6500 6b00 7400 6900 6500  s.e.l.e.k.t.i.e.
+00002550: 7200 7400 6500 6e00 2000 5100 5300 4f00  r.t.e.n. .Q.S.O.
+00002560: 7300 2000 7700 6900 7200 6b00 6c00 6900  s. .w.i.r.k.l.i.
+00002570: 6300 6800 2000 6c00 f600 7300 6300 6800  c.h. .l...s.c.h.
+00002580: 6500 6e00 3f08 0000 0000 0600 0000 3144  e.n.?.........1D
+00002590: 6f20 796f 7520 7265 616c 6c79 2077 616e  o you really wan
+000025a0: 7420 746f 2064 656c 6574 6520 7468 6520  t to delete the 
+000025b0: 7365 6c65 6374 6564 2051 534f 2873 293f  selected QSO(s)?
+000025c0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+000025d0: ffff ffff 0800 0000 0006 0000 0010 4561  ..............Ea
+000025e0: 7274 682d 4d6f 6f6e 2d45 6172 7468 0700  rth-Moon-Earth..
+000025f0: 0000 0944 7261 676f 6e4c 6f67 0103 ffff  ...DragonLog....
+00002600: ffff 0800 0000 0006 0000 0008 4563 686f  ............Echo
+00002610: 4c69 6e6b 0700 0000 0944 7261 676f 6e4c  Link.....DragonL
+00002620: 6f67 0103 0000 000c 0046 0065 0068 006c  og.......F.e.h.l
+00002630: 0065 0072 0800 0000 0006 0000 0005 4572  .e.r..........Er
+00002640: 726f 7207 0000 0009 4472 6167 6f6e 4c6f  ror.....DragonLo
+00002650: 6701 0300 0000 2800 4500 7800 6300 6500  g.....(.E.x.c.e.
+00002660: 6c00 2d00 4400 6100 7400 6500 6900 2000  l.-.D.a.t.e.i. .
+00002670: 2800 2a00 2e00 7800 6c00 7300 7800 2908  (.*...x.l.s.x.).
+00002680: 0000 0000 0600 0000 1345 7863 656c 2d46  .........Excel-F
+00002690: 696c 6520 282a 2e78 6c73 7829 0700 0000  ile (*.xlsx)....
+000026a0: 0944 7261 676f 6e4c 6f67 0103 0000 0024  .DragonLog.....$
+000026b0: 0045 0078 0070 006f 0072 0074 0069 0065  .E.x.p.o.r.t.i.e
+000026c0: 0072 0065 0020 0051 0053 004f 0020 006c  .r.e. .Q.S.O. .l
+000026d0: 006f 0067 0800 0000 0006 0000 0010 4578  .o.g..........Ex
+000026e0: 706f 7274 6564 2051 534f 206c 6f67 0700  ported QSO log..
+000026f0: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
+00002700: 001a 0046 0032 002d 0052 0065 0066 006c  ...F.2.-.R.e.f.l
+00002710: 0065 006b 0074 0069 006f 006e 0800 0000  .e.k.t.i.o.n....
+00002720: 0006 0000 000d 4632 2052 6566 6c65 6374  ......F2 Reflect
+00002730: 696f 6e07 0000 0009 4472 6167 6f6e 4c6f  ion.....DragonLo
+00002740: 6701 0300 0000 3800 4600 6900 6500 6c00  g.....8.F.i.e.l.
+00002750: 6400 2d00 4100 6c00 6900 6700 6e00 6500  d.-.A.l.i.g.n.e.
+00002760: 6400 2d00 4900 7200 7200 6500 6700 7500  d.-.I.r.r.e.g.u.
+00002770: 6c00 6100 7200 6900 7400 6900 6500 7308  l.a.r.i.t.i.e.s.
+00002780: 0000 0000 0600 0000 1c46 6965 6c64 2041  .........Field A
+00002790: 6c69 676e 6564 2049 7272 6567 756c 6172  ligned Irregular
+000027a0: 6974 6965 7307 0000 0009 4472 6167 6f6e  ities.....Dragon
+000027b0: 4c6f 6701 0300 0000 1000 4600 7200 6500  Log.......F.r.e.
+000027c0: 7100 7500 6500 6e00 7a08 0000 0000 0600  q.u.e.n.z.......
+000027d0: 0000 0946 7265 7175 656e 6379 0700 0000  ...Frequency....
+000027e0: 0944 7261 676f 6e4c 6f67 0103 0000 0014  .DragonLog......
+000027f0: 0042 006f 0064 0065 006e 0077 0065 006c  .B.o.d.e.n.w.e.l
+00002800: 006c 0065 0800 0000 0006 0000 000b 4772  .l.e..........Gr
+00002810: 6f75 6e64 2057 6176 6507 0000 0009 4472  ound Wave.....Dr
+00002820: 6167 6f6e 4c6f 6701 03ff ffff ff08 0000  agonLog.........
+00002830: 0000 0600 0000 0648 616d 5154 4807 0000  .......HamQTH...
+00002840: 0009 4472 6167 6f6e 4c6f 6701 03ff ffff  ..DragonLog.....
+00002850: ff08 0000 0000 0600 0000 0648 616d 6c69  ...........Hamli
+00002860: 6207 0000 0009 4472 6167 6f6e 4c6f 6701  b.....DragonLog.
+00002870: 0300 0000 0a00 4800 6900 6c00 6600 6508  ......H.i.l.f.e.
+00002880: 0000 0000 0600 0000 0448 656c 7007 0000  .........Help...
+00002890: 0009 4472 6167 6f6e 4c6f 6701 03ff ffff  ..DragonLog.....
+000028a0: ff08 0000 0000 0600 0000 0449 524c 5007  ...........IRLP.
+000028b0: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
+000028c0: 0000 2600 4900 6e00 7400 6500 7200 6e00  ..&.I.n.t.e.r.n.
+000028d0: 6500 7400 7500 6e00 7400 6500 7200 7300  e.t.u.n.t.e.r.s.
+000028e0: 7400 fc00 7400 7a00 7408 0000 0000 0600  t...t.z.t.......
+000028f0: 0000 1149 6e74 6572 6e65 742d 6173 7369  ...Internet-assi
+00002900: 7374 6564 0700 0000 0944 7261 676f 6e4c  sted.....DragonL
+00002910: 6f67 0103 0000 0018 0049 006f 006e 006f  og.......I.o.n.o
+00002920: 002d 0053 0063 0061 0074 0074 0065 0072  .-.S.c.a.t.t.e.r
+00002930: 0800 0000 0006 0000 000b 496f 6e6f 7363  ..........Ionosc
+00002940: 6174 7465 7207 0000 0009 4472 6167 6f6e  atter.....Dragon
+00002950: 4c6f 6701 0300 0000 2000 6c00 6500 7400  Log..... .l.e.t.
+00002960: 7a00 7400 6500 7300 2000 4800 6100 6c00  z.t.e.s. .H.a.l.
+00002970: 6200 6a00 6100 6800 7208 0000 0000 0600  b.j.a.h.r.......
+00002980: 0000 0e4c 6173 7420 6861 6c66 2079 6561  ...Last half yea
+00002990: 7207 0000 0009 4472 6167 6f6e 4c6f 6701  r.....DragonLog.
+000029a0: 0300 0000 1a00 6c00 6500 7400 7a00 7400  ......l.e.t.z.t.
+000029b0: 6500 6e00 2000 4d00 6f00 6e00 6100 7408  e.n. .M.o.n.a.t.
+000029c0: 0000 0000 0600 0000 0a4c 6173 7420 6d6f  .........Last mo
+000029d0: 6e74 6807 0000 0009 4472 6167 6f6e 4c6f  nth.....DragonLo
+000029e0: 6701 0300 0000 1800 6c00 6500 7400 7a00  g.......l.e.t.z.
+000029f0: 7400 6500 2000 5700 6f00 6300 6800 6508  t.e. .W.o.c.h.e.
+00002a00: 0000 0000 0600 0000 094c 6173 7420 7765  .........Last we
+00002a10: 656b 0700 0000 0944 7261 676f 6e4c 6f67  ek.....DragonLog
+00002a20: 0103 0000 0018 006c 0065 0074 007a 0074  .......l.e.t.z.t
+00002a30: 0065 0073 0020 004a 0061 0068 0072 0800  .e.s. .J.a.h.r..
+00002a40: 0000 0006 0000 0009 4c61 7374 2079 6561  ........Last yea
+00002a50: 7207 0000 0009 4472 6167 6f6e 4c6f 6701  r.....DragonLog.
+00002a60: 0300 0000 1e00 5300 6900 6300 6800 7400  ......S.i.c.h.t.
+00002a70: 7600 6500 7200 6200 6900 6e00 6400 7500  v.e.r.b.i.n.d.u.
+00002a80: 6e00 6708 0000 0000 0600 0000 0d4c 696e  n.g..........Lin
+00002a90: 6520 6f66 2053 6967 6874 0700 0000 0944  e of Sight.....D
+00002aa0: 7261 676f 6e4c 6f67 0103 0000 0020 004c  ragonLog..... .L
+00002ab0: 006f 0054 0057 002d 0041 0044 0049 0046  .o.T.W.-.A.D.I.F
+00002ac0: 002d 0055 0070 006c 006f 0061 0064 0800  .-.U.p.l.o.a.d..
+00002ad0: 0000 0006 0000 0010 4c6f 5457 2041 4449  ........LoTW ADI
+00002ae0: 4620 7570 6c6f 6164 0700 0000 0944 7261  F upload.....Dra
+00002af0: 676f 6e4c 6f67 0103 0000 0014 004c 006f  gonLog.......L.o
+00002b00: 0054 0057 0020 0065 006d 0070 0066 002e  .T.W. .e.m.p.f..
+00002b10: 0800 0000 0006 0000 0009 4c6f 5457 2072  ..........LoTW r
+00002b20: 6376 6407 0000 0009 4472 6167 6f6e 4c6f  cvd.....DragonLo
+00002b30: 6701 0300 0000 1400 4c00 6f00 5400 5700  g.......L.o.T.W.
+00002b40: 2000 7600 6500 7200 7300 2e08 0000 0000   .v.e.r.s.......
+00002b50: 0600 0000 094c 6f54 5720 7365 6e74 0700  .....LoTW sent..
+00002b60: 0000 0944 7261 676f 6e4c 6f67 0103 ffff  ...DragonLog....
+00002b70: ffff 0800 0000 0006 0000 0007 4c6f 6361  ............Loca
+00002b80: 746f 7207 0000 0009 4472 6167 6f6e 4c6f  tor.....DragonLo
+00002b90: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
+00002ba0: 0f4c 6f67 2069 6d70 6f72 7420 4144 4946  .Log import ADIF
+00002bb0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00002bc0: 0000 001c 004c 006f 0067 0020 0049 006d  .....L.o.g. .I.m
+00002bd0: 0070 006f 0072 0074 0020 0043 0053 0056  .p.o.r.t. .C.S.V
+00002be0: 0800 0000 0006 0000 000e 4c6f 6720 696d  ..........Log im
+00002bf0: 706f 7274 2043 5356 0700 0000 0944 7261  port CSV.....Dra
+00002c00: 676f 6e4c 6f67 0103 0000 001e 004c 006f  gonLog.......L.o
+00002c10: 0067 0020 0049 006d 0070 006f 0072 0074  .g. .I.m.p.o.r.t
+00002c20: 0020 0058 004c 0053 0058 0800 0000 0006  . .X.L.S.X......
+00002c30: 0000 000f 4c6f 6720 696d 706f 7274 2058  ....Log import X
+00002c40: 4c53 5807 0000 0009 4472 6167 6f6e 4c6f  LSX.....DragonLo
+00002c50: 6701 0300 0000 1c00 4d00 6500 7400 6500  g.......M.e.t.e.
+00002c60: 6f00 7200 2d00 5300 6300 6100 7400 7400  o.r.-.S.c.a.t.t.
+00002c70: 6500 7208 0000 0000 0600 0000 0e4d 6574  e.r..........Met
+00002c80: 656f 7220 7363 6174 7465 7207 0000 0009  eor scatter.....
+00002c90: 4472 6167 6f6e 4c6f 6701 0300 0000 5a00  DragonLog.....Z.
+00002ca0: 4b00 6500 6900 6e00 6500 2000 5300 7400  K.e.i.n.e. .S.t.
+00002cb0: 6100 7400 6900 6f00 6e00 7300 6b00 6f00  a.t.i.o.n.s.k.o.
+00002cc0: 6e00 6600 6900 6700 7500 7200 6100 7400  n.f.i.g.u.r.a.t.
+00002cd0: 6900 6f00 6e00 2000 6900 6e00 2000 5400  i.o.n. .i.n. .T.
+00002ce0: 5100 5300 4c00 2000 7600 6500 7200 6600  Q.S.L. .v.e.r.f.
+00002cf0: fc00 6700 6200 6100 7208 0000 0000 0600  ..g.b.a.r.......
+00002d00: 0000 254d 6973 7369 6e67 2073 7461 7469  ..%Missing stati
+00002d10: 6f6e 2063 6f6e 6669 6775 7261 7469 6f6e  on configuration
+00002d20: 2069 6e20 5451 534c 0700 0000 0944 7261   in TQSL.....Dra
+00002d30: 676f 6e4c 6f67 0103 ffff ffff 0800 0000  gonLog..........
+00002d40: 0006 0000 0004 4d6f 6465 0700 0000 0944  ......Mode.....D
+00002d50: 7261 676f 6e4c 6f67 0103 ffff ffff 0800  ragonLog........
+00002d60: 0000 0006 0000 0004 4e61 6d65 0700 0000  ........Name....
+00002d70: 0944 7261 676f 6e4c 6f67 0103 0000 0034  .DragonLog.....4
+00002d80: 004b 0065 0069 006e 0065 0020 0051 0053  .K.e.i.n.e. .Q.S
+00002d90: 004f 0073 0020 0066 00fc 0072 0020 0064  .O.s. .f...r. .d
+00002da0: 0065 006e 0020 004c 006f 0063 0061 0074  .e.n. .L.o.c.a.t
+00002db0: 006f 0072 0800 0000 0006 0000 0017 4e6f  .o.r..........No
+00002dc0: 2072 6563 6f72 6473 2066 6f72 206c 6f63   records for loc
+00002dd0: 6174 696f 6e07 0000 0009 4472 6167 6f6e  ation.....Dragon
+00002de0: 4c6f 6701 0300 0000 0e00 4e00 6f00 7400  Log.......N.o.t.
+00002df0: 6900 7a00 6500 6e08 0000 0000 0600 0000  i.z.e.n.........
+00002e00: 054e 6f74 6573 0700 0000 0944 7261 676f  .Notes.....Drago
+00002e10: 6e4c 6f67 0103 ffff ffff 0800 0000 0006  nLog............
+00002e20: 0000 0002 4f6b 0700 0000 0944 7261 676f  ....Ok.....Drago
+00002e30: 6e4c 6f67 0103 0000 001e 0045 0069 0067  nLog.......E.i.g
+00002e40: 0065 006e 0065 0072 0020 004c 006f 0063  .e.n.e.r. .L.o.c
+00002e50: 0061 0074 006f 0072 0800 0000 0006 0000  .a.t.o.r........
+00002e60: 000b 4f77 6e20 4c6f 6361 746f 7207 0000  ..Own Locator...
+00002e70: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+00002e80: 1800 4500 6900 6700 6500 6e00 6500 7200  ..E.i.g.e.n.e.r.
+00002e90: 2000 4e00 6100 6d00 6508 0000 0000 0600   .N.a.m.e.......
+00002ea0: 0000 084f 776e 204e 616d 6507 0000 0009  ...Own Name.....
+00002eb0: 4472 6167 6f6e 4c6f 6701 0300 0000 1600  DragonLog.......
+00002ec0: 4500 6900 6700 6500 6e00 6500 7200 2000  E.i.g.e.n.e.r. .
+00002ed0: 5100 5400 4808 0000 0000 0600 0000 074f  Q.T.H..........O
+00002ee0: 776e 2051 5448 0700 0000 0944 7261 676f  wn QTH.....Drago
+00002ef0: 6e4c 6f67 0103 0000 0024 0045 0069 0067  nLog.....$.E.i.g
+00002f00: 0065 006e 0065 0073 0020 0052 0075 0066  .e.n.e.s. .R.u.f
+00002f10: 007a 0065 0069 0063 0068 0065 006e 0800  .z.e.i.c.h.e.n..
+00002f20: 0000 0006 0000 000d 4f77 6e20 6361 6c6c  ........Own call
+00002f30: 2073 6967 6e07 0000 0009 4472 6167 6f6e   sign.....Dragon
+00002f40: 4c6f 6701 0300 0000 1000 4c00 6500 6900  Log.......L.e.i.
+00002f50: 7300 7400 7500 6e00 6708 0000 0000 0600  s.t.u.n.g.......
+00002f60: 0000 0550 6f77 6572 0700 0000 0944 7261  ...Power.....Dra
+00002f70: 676f 6e4c 6f67 0103 0000 0016 0041 0075  gonLog.......A.u
+00002f80: 0073 0062 0072 0065 0069 0074 0075 006e  .s.b.r.e.i.t.u.n
+00002f90: 0067 0800 0000 0006 0000 000b 5072 6f70  .g..........Prop
+00002fa0: 6167 6174 696f 6e07 0000 0009 4472 6167  agation.....Drag
+00002fb0: 6f6e 4c6f 6701 0300 0000 1a00 5100 5300  onLog.......Q.S.
+00002fc0: 4c00 2d00 4e00 6100 6300 6800 7200 6900  L.-.N.a.c.h.r.i.
+00002fd0: 6300 6800 7408 0000 0000 0600 0000 0b51  c.h.t..........Q
+00002fe0: 534c 206d 6573 7361 6765 0700 0000 0944  SL message.....D
+00002ff0: 7261 676f 6e4c 6f67 0103 0000 0010 0051  ragonLog.......Q
+00003000: 0053 004c 002d 0050 0066 0061 0064 0800  .S.L.-.P.f.a.d..
+00003010: 0000 0006 0000 0008 5153 4c20 7061 7468  ........QSL path
+00003020: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00003030: 0000 0012 0051 0053 004c 0020 0065 006d  .....Q.S.L. .e.m
+00003040: 0070 0066 002e 0800 0000 0006 0000 0008  .p.f............
+00003050: 5153 4c20 7263 7664 0700 0000 0944 7261  QSL rcvd.....Dra
+00003060: 676f 6e4c 6f67 0103 0000 0012 0051 0053  gonLog.......Q.S
+00003070: 004c 0020 0076 0065 0072 0073 002e 0800  .L. .v.e.r.s....
+00003080: 0000 0006 0000 0008 5153 4c20 7365 6e74  ........QSL sent
+00003090: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+000030a0: 0000 000e 0051 0053 004c 002d 0056 0069  .....Q.S.L.-.V.i
+000030b0: 0061 0800 0000 0006 0000 0007 5153 4c20  .a..........QSL 
+000030c0: 7669 6107 0000 0009 4472 6167 6f6e 4c6f  via.....DragonLo
+000030d0: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
+000030e0: 0351 534f 0700 0000 0944 7261 676f 6e4c  .QSO.....DragonL
+000030f0: 6f67 0103 0000 0048 0051 0053 004f 002d  og.....H.Q.S.O.-
+00003100: 004c 006f 0067 0020 0028 002a 002e 0071  .L.o.g. .(.*...q
+00003110: 006c 006f 0067 0029 003b 003b 0041 006c  .l.o.g.).;.;.A.l
+00003120: 006c 0065 0020 0044 0061 0074 0065 0069  .l.e. .D.a.t.e.i
+00003130: 0065 006e 0020 0028 002a 002e 002a 0029  .e.n. .(.*...*.)
+00003140: 0800 0000 0006 0000 0021 5153 4f2d 4c6f  .........!QSO-Lo
+00003150: 6720 282a 2e71 6c6f 6729 3b3b 416c 6c20  g (*.qlog);;All 
+00003160: 4669 6c65 7320 282a 2e2a 2907 0000 0009  Files (*.*).....
+00003170: 4472 6167 6f6e 4c6f 6701 03ff ffff ff08  DragonLog.......
+00003180: 0000 0000 0600 0000 0351 5448 0700 0000  .........QTH....
+00003190: 0944 7261 676f 6e4c 6f67 0103 0000 0012  .DragonLog......
+000031a0: 0052 0053 0054 0020 0065 006d 0070 0066  .R.S.T. .e.m.p.f
+000031b0: 002e 0800 0000 0006 0000 0008 5253 5420  ............RST 
+000031c0: 7263 7664 0700 0000 0944 7261 676f 6e4c  rcvd.....DragonL
+000031d0: 6f67 0103 0000 0010 0052 0053 0054 0020  og.......R.S.T. 
+000031e0: 0067 0065 0073 002e 0800 0000 0006 0000  .g.e.s..........
+000031f0: 0008 5253 5420 7365 6e74 0700 0000 0944  ..RST sent.....D
+00003200: 7261 676f 6e4c 6f67 0103 ffff ffff 0800  ragonLog........
+00003210: 0000 0006 0000 0005 5261 6469 6f07 0000  ........Radio...
+00003220: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+00003230: 1800 5200 6100 6900 6e00 2d00 5300 6300  ..R.a.i.n.-.S.c.
+00003240: 6100 7400 7400 6500 7208 0000 0000 0600  a.t.t.e.r.......
+00003250: 0000 0c52 6169 6e20 7363 6174 7465 7207  ...Rain scatter.
+00003260: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
+00003270: 0000 3200 5200 6500 7000 6500 6100 7400  ..2.R.e.p.e.a.t.
+00003280: 6500 7200 2000 6f00 6400 6500 7200 2000  e.r. .o.d.e.r. .
+00003290: 5400 7200 6100 6e00 7300 7000 6f00 6e00  T.r.a.n.s.p.o.n.
+000032a0: 6400 6500 7208 0000 0000 0600 0000 1752  d.e.r..........R
+000032b0: 6570 6561 7465 7220 6f72 2054 7261 6e73  epeater or Trans
+000032c0: 706f 6e64 6572 0700 0000 0944 7261 676f  ponder.....Drago
+000032d0: 6e4c 6f67 0103 0000 0018 0045 006d 0070  nLog.......E.m.p
+000032e0: 0066 002e 0020 0051 0053 004f 0020 0049  .f... .Q.S.O. .I
+000032f0: 0044 0800 0000 0006 0000 0009 5278 2051  .D..........Rx Q
+00003300: 534f 2049 4407 0000 0009 4472 6167 6f6e  SO ID.....Dragon
+00003310: 4c6f 6701 0300 0000 1600 4500 6d00 7000  Log.......E.m.p.
+00003320: 6600 2e00 2000 4400 6100 7400 6500 6e08  f... .D.a.t.e.n.
+00003330: 0000 0000 0600 0000 0752 7820 6461 7461  .........Rx data
+00003340: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00003350: 0000 0010 0053 0061 0074 0065 006c 006c  .....S.a.t.e.l.l
+00003360: 0069 0074 0800 0000 0006 0000 0009 5361  .i.t..........Sa
+00003370: 7465 6c6c 6974 6507 0000 0009 4472 6167  tellite.....Drag
+00003380: 6f6e 4c6f 6701 0300 0000 2a00 4500 7800  onLog.....*.E.x.
+00003390: 7000 6f00 7200 7400 6400 6100 7400 6500  p.o.r.t.d.a.t.e.
+000033a0: 6900 2000 7300 7000 6500 6900 6300 6800  i. .s.p.e.i.c.h.
+000033b0: 6500 7200 6e08 0000 0000 0600 0000 1253  e.r.n..........S
+000033c0: 656c 6563 7420 6578 706f 7274 2066 696c  elect export fil
+000033d0: 6507 0000 0009 4472 6167 6f6e 4c6f 6701  e.....DragonLog.
+000033e0: 0300 0000 2000 4400 6100 7400 6500 6e00  .... .D.a.t.e.n.
+000033f0: 6200 6100 6e00 6b00 2000 f600 6600 6600  b.a.n.k. ...f.f.
+00003400: 6e00 6500 6e08 0000 0000 0600 0000 0b53  n.e.n..........S
+00003410: 656c 6563 7420 6669 6c65 0700 0000 0944  elect file.....D
+00003420: 7261 676f 6e4c 6f67 0103 0000 0038 005a  ragonLog.....8.Z
+00003430: 0075 0020 00fc 0062 0065 0072 0077 0061  .u. ...b.e.r.w.a
+00003440: 0063 0068 0065 006e 0064 0065 0020 0044  .c.h.e.n.d.e. .D
+00003450: 0061 0074 0065 0069 0020 0077 00e4 0068  .a.t.e.i. .w...h
+00003460: 006c 0065 006e 0800 0000 0006 0000 0014  .l.e.n..........
+00003470: 5365 6c65 6374 2066 696c 6520 746f 2077  Select file to w
+00003480: 6174 6368 0700 0000 0944 7261 676f 6e4c  atch.....DragonL
+00003490: 6f67 0103 0000 0024 0049 006d 0070 006f  og.....$.I.m.p.o
+000034a0: 0072 0074 0064 0061 0074 0065 0069 0020  .r.t.d.a.t.e.i. 
+000034b0: 00f6 0066 0066 006e 0065 006e 0800 0000  ...f.f.n.e.n....
+000034c0: 0006 0000 0012 5365 6c65 6374 2069 6d70  ......Select imp
+000034d0: 6f72 7420 6669 6c65 0700 0000 0944 7261  ort file.....Dra
+000034e0: 676f 6e4c 6f67 0103 0000 001a 0057 00e4  gonLog.......W..
+000034f0: 0068 006c 0065 0020 0053 0074 0061 0074  .h.l.e. .S.t.a.t
+00003500: 0069 006f 006e 0800 0000 0006 0000 000e  .i.o.n..........
+00003510: 5365 6c65 6374 2073 7461 7469 6f6e 0700  Select station..
+00003520: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
+00003530: 0044 004c 006f 0054 0057 002d 0053 0065  .D.L.o.T.W.-.S.e
+00003540: 0072 0076 0065 0072 0020 0068 0061 0074  .r.v.e.r. .h.a.t
+00003550: 0020 0064 0061 0073 0020 004c 006f 0067  . .d.a.s. .L.o.g
+00003560: 0020 0061 0062 0067 0065 0077 0069 0065  . .a.b.g.e.w.i.e
+00003570: 0073 0065 006e 0800 0000 0006 0000 0013  .s.e.n..........
+00003580: 5365 7276 6572 2072 656a 6563 7465 6420  Server rejected 
+00003590: 6c6f 6707 0000 0009 4472 6167 6f6e 4c6f  log.....DragonLo
+000035a0: 6701 0300 0000 1400 7a00 6500 6900 6700  g.......z.e.i.g.
+000035b0: 6500 2000 6100 6c00 6c00 6508 0000 0000  e. .a.l.l.e.....
+000035c0: 0600 0000 0853 686f 7720 616c 6c07 0000  .....Show all...
+000035d0: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+000035e0: 1400 5300 7000 6f00 7200 6100 6400 6900  ..S.p.o.r.a.d.i.
+000035f0: 6300 2d00 4508 0000 0000 0600 0000 0a53  c.-.E..........S
+00003600: 706f 7261 6469 6320 4507 0000 0009 4472  poradic E.....Dr
+00003610: 6167 6f6e 4c6f 6701 03ff ffff ff08 0000  agonLog.........
+00003620: 0000 0600 0000 0753 7562 6d6f 6465 0700  .......Submode..
+00003630: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
+00003640: 002a 0054 0051 0053 004c 002d 0053 0069  .*.T.Q.S.L.-.S.i
+00003650: 0067 006e 0061 0074 0075 0072 0070 0061  .g.n.a.t.u.r.p.a
+00003660: 0073 0073 0077 006f 0072 0074 0800 0000  .s.s.w.o.r.t....
+00003670: 0006 0000 0017 5451 534c 2073 6967 6e61  ......TQSL signa
+00003680: 7475 7265 2070 6173 7377 6f72 6407 0000  ture password...
+00003690: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+000036a0: b200 4400 6900 6500 2000 4400 6100 7400  ..D.i.e. .D.a.t.
+000036b0: 6500 6e00 6200 6100 6e00 6b00 7300 7400  e.n.b.a.n.k.s.t.
+000036c0: 7200 7500 6b00 7400 7500 7200 2000 6900  r.u.k.t.u.r. .i.
+000036d0: 7300 7400 2000 7600 6500 7200 6100 6c00  s.t. .v.e.r.a.l.
+000036e0: 7400 6500 7400 2000 7500 6e00 6400 2000  t.e.t. .u.n.d. .
+000036f0: 6d00 7500 7300 7300 2000 6b00 6f00 6e00  m.u.s.s. .k.o.n.
+00003700: 7600 6500 7200 7400 6900 6500 7200 7400  v.e.r.t.i.e.r.t.
+00003710: 2000 7700 6500 7200 6400 6500 6e00 0a00   .w.e.r.d.e.n...
+00003720: 0a00 4500 6900 6e00 2000 4200 6100 6300  ..E.i.n. .B.a.c.
+00003730: 6b00 7500 7000 2000 7700 6900 7200 6400  k.u.p. .w.i.r.d.
+00003740: 2000 6500 7200 7300 7400 6500 6c00 6c00   .e.r.s.t.e.l.l.
+00003750: 7400 3a08 0000 0000 0600 0000 5754 6865  t.:.........WThe
+00003760: 2064 6174 6162 6173 6520 7374 7275 6374   database struct
+00003770: 7572 6520 6973 206f 7574 2d64 6174 6564  ure is out-dated
+00003780: 2061 6e64 206e 6565 6473 2061 2063 6f6e   and needs a con
+00003790: 7665 7273 696f 6e0a 0a41 2062 6163 6b75  version..A backu
+000037a0: 7020 7769 6c6c 2062 6520 6765 6e65 7261  p will be genera
+000037b0: 7465 643a 0700 0000 0944 7261 676f 6e4c  ted:.....DragonL
+000037c0: 6f67 0103 0000 001e 0054 0072 0061 006e  og.......T.r.a.n
+000037d0: 0073 0065 0071 0075 0061 0074 006f 0072  .s.e.q.u.a.t.o.r
+000037e0: 0069 0061 006c 0800 0000 0006 0000 0010  .i.a.l..........
+000037f0: 5472 616e 732d 6571 7561 746f 7269 616c  Trans-equatorial
+00003800: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00003810: 0000 0028 0054 0072 006f 0070 006f 0073  ...(.T.r.o.p.o.s
+00003820: 0070 0068 0065 0072 0069 0063 002d 0044  .p.h.e.r.i.c.-.D
+00003830: 0075 0063 0074 0069 006e 0067 0800 0000  .u.c.t.i.n.g....
+00003840: 0006 0000 0014 5472 6f70 6f73 7068 6572  ......Tropospher
+00003850: 6963 2064 7563 7469 6e67 0700 0000 0944  ic ducting.....D
+00003860: 7261 676f 6e4c 6f67 0103 0000 0016 0047  ragonLog.......G
+00003870: 0065 0073 002e 0020 0051 0053 004f 0020  .e.s... .Q.S.O. 
+00003880: 0049 0044 0800 0000 0006 0000 0009 5478  .I.D..........Tx
+00003890: 2051 534f 2049 4407 0000 0009 4472 6167   QSO ID.....Drag
+000038a0: 6f6e 4c6f 6701 03ff ffff ff08 0000 0000  onLog...........
+000038b0: 0600 0000 0756 6572 7369 6f6e 0700 0000  .....Version....
+000038c0: 0944 7261 676f 6e4c 6f67 0103 0000 002c  .DragonLog.....,
+000038d0: 0050 0072 006f 0067 0072 0061 006d 006d  .P.r.o.g.r.a.m.m
+000038e0: 006c 006f 0067 0020 00fc 0062 0065 0072  .l.o.g. ...b.e.r
+000038f0: 0077 0061 0063 0068 0065 006e 0800 0000  .w.a.c.h.e.n....
+00003900: 0006 0000 0015 5761 7463 6820 6170 706c  ......Watch appl
+00003910: 6963 6174 696f 6e20 6c6f 6707 0000 0009  ication log.....
+00003920: 4472 6167 6f6e 4c6f 6701 0300 0000 2000  DragonLog..... .
+00003930: 4400 6100 7400 6500 6900 fc00 6200 6500  D.a.t.e.i...b.e.
+00003940: 7200 7700 6100 6300 6800 7500 6e00 6708  r.w.a.c.h.u.n.g.
+00003950: 0000 0000 0600 0000 0d57 6174 6368 696e  .........Watchin
+00003960: 6720 6669 6c65 0700 0000 0944 7261 676f  g file.....Drago
+00003970: 6e4c 6f67 0103 0000 0014 0065 0051 0053  nLog.......e.Q.S
+00003980: 004c 0020 0065 006d 0070 0066 002e 0800  .L. .e.m.p.f....
+00003990: 0000 0006 0000 0009 6551 534c 2072 6376  ........eQSL rcv
+000039a0: 6407 0000 0009 4472 6167 6f6e 4c6f 6701  d.....DragonLog.
+000039b0: 0300 0000 1400 6500 5100 5300 4c00 2000  ......e.Q.S.L. .
+000039c0: 7600 6500 7200 7300 2e08 0000 0000 0600  v.e.r.s.........
+000039d0: 0000 0965 5153 4c20 7365 6e74 0700 0000  ...eQSL sent....
+000039e0: 0944 7261 676f 6e4c 6f67 0103 0000 000e  .DragonLog......
+000039f0: 0069 006e 0061 006b 0074 0069 0076 0800  .i.n.a.k.t.i.v..
+00003a00: 0000 0006 0000 0007 696e 6163 7469 7607  ........inactiv.
+00003a10: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
+00003a20: 0000 0c00 2800 6c00 6500 6500 7200 2908  ....(.l.e.e.r.).
+00003a30: 0000 0000 0600 0000 0728 656d 7074 7929  .........(empty)
+00003a40: 0700 0000 084c 6973 7445 6469 7401 03ff  .....ListEdit...
+00003a50: ffff ff08 0000 0000 0600 0000 0446 6f72  .............For
+00003a60: 6d07 0000 000c 4c69 7374 4564 6974 466f  m.....ListEditFo
+00003a70: 726d 0103 ffff ffff 0800 0000 0006 0000  rm..............
+00003a80: 0005 4c61 6265 6c07 0000 000c 4c69 7374  ..Label.....List
+00003a90: 4564 6974 466f 726d 0103 0000 0008 00dc  EditForm........
+00003aa0: 0062 0065 0072 0800 0000 0006 0000 0005  .b.e.r..........
+00003ab0: 4162 6f75 7407 0000 000a 4d61 696e 5769  About.....MainWi
+00003ac0: 6e64 6f77 0103 0000 000e 00dc 0062 0065  ndow.........b.e
+00003ad0: 0072 0020 0051 0074 0800 0000 0006 0000  .r. .Q.t........
+00003ae0: 0008 4162 6f75 7420 5174 0700 0000 0a4d  ..About Qt.....M
+00003af0: 6169 6e57 696e 646f 7701 0300 0000 1a00  ainWindow.......
+00003b00: 4100 6e00 7700 6500 6e00 6400 7500 6e00  A.n.w.e.n.d.u.n.
+00003b10: 6700 7300 6c00 6f00 6708 0000 0000 0600  g.s.l.o.g.......
+00003b20: 0000 0f41 7070 6c69 6361 7469 6f6e 204c  ...Application L
+00003b30: 6f67 0700 0000 0a4d 6169 6e57 696e 646f  og.....MainWindo
+00003b40: 7701 03ff ffff ff08 0000 0000 0600 0000  w...............
+00003b50: 0442 616e 6407 0000 000a 4d61 696e 5769  .Band.....MainWi
+00003b60: 6e64 6f77 0103 0000 0014 0052 0075 0066  ndow.......R.u.f
+00003b70: 007a 0065 0069 0063 0068 0065 006e 0800  .z.e.i.c.h.e.n..
+00003b80: 0000 0006 0000 0008 4361 6c6c 7369 676e  ........Callsign
+00003b90: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
+00003ba0: 0300 0000 2200 4500 6900 6e00 7400 7200  ....".E.i.n.t.r.
+00003bb0: 6100 6700 2000 e400 6e00 6400 6500 7200  a.g. ...n.d.e.r.
+00003bc0: 6e00 2e00 2e00 2e08 0000 0000 0600 0000  n...............
+00003bd0: 1343 6861 6e67 6520 6c6f 6720 656e 7472  .Change log entr
+00003be0: 792e 2e2e 0700 0000 0a4d 6169 6e57 696e  y........MainWin
+00003bf0: 646f 7701 03ff ffff ff08 0000 0000 0600  dow.............
+00003c00: 0000 0643 7472 6c2b 4507 0000 000a 4d61  ...Ctrl+E.....Ma
+00003c10: 696e 5769 6e64 6f77 0103 ffff ffff 0800  inWindow........
+00003c20: 0000 0006 0000 0006 4374 726c 2b46 0700  ........Ctrl+F..
+00003c30: 0000 0a4d 6169 6e57 696e 646f 7701 03ff  ...MainWindow...
+00003c40: ffff ff08 0000 0000 0600 0000 0643 7472  .............Ctr
+00003c50: 6c2b 4c07 0000 000a 4d61 696e 5769 6e64  l+L.....MainWind
+00003c60: 6f77 0103 ffff ffff 0800 0000 0006 0000  ow..............
+00003c70: 0006 4374 726c 2b51 0700 0000 0a4d 6169  ..Ctrl+Q.....Mai
+00003c80: 6e57 696e 646f 7701 03ff ffff ff08 0000  nWindow.........
+00003c90: 0000 0600 0000 0643 7472 6c2b 5207 0000  .......Ctrl+R...
+00003ca0: 000a 4d61 696e 5769 6e64 6f77 0103 ffff  ..MainWindow....
+00003cb0: ffff 0800 0000 0006 0000 0006 4374 726c  ............Ctrl
+00003cc0: 2b57 0700 0000 0a4d 6169 6e57 696e 646f  +W.....MainWindo
+00003cd0: 7701 03ff ffff ff08 0000 0000 0600 0000  w...............
+00003ce0: 0643 7472 6c2b 5807 0000 000a 4d61 696e  .Ctrl+X.....Main
+00003cf0: 5769 6e64 6f77 0103 0000 0012 0044 0061  Window.......D.a
+00003d00: 0074 0075 006d 0020 0076 006f 006e 0800  .t.u.m. .v.o.n..
+00003d10: 0000 0006 0000 0009 4461 7465 2066 726f  ........Date fro
+00003d20: 6d07 0000 000a 4d61 696e 5769 6e64 6f77  m.....MainWindow
+00003d30: 0103 0000 0012 0044 0061 0074 0075 006d  .......D.a.t.u.m
+00003d40: 0020 0062 0069 0073 0800 0000 0006 0000  . .b.i.s........
+00003d50: 0007 4461 7465 2074 6f07 0000 000a 4d61  ..Date to.....Ma
+00003d60: 696e 5769 6e64 6f77 0103 0000 001e 0045  inWindow.......E
+00003d70: 0069 006e 0074 0072 0061 0067 0020 006c  .i.n.t.r.a.g. .l
+00003d80: 00f6 0073 0063 0068 0065 006e 0800 0000  ...s.c.h.e.n....
+00003d90: 0006 0000 0010 4465 6c65 7465 206c 6f67  ......Delete log
+00003da0: 2065 6e74 7279 0700 0000 0a4d 6169 6e57   entry.....MainW
+00003db0: 696e 646f 7701 03ff ffff ff08 0000 0000  indow...........
+00003dc0: 0600 0000 0944 7261 676f 6e4c 6f67 0700  .....DragonLog..
+00003dd0: 0000 0a4d 6169 6e57 696e 646f 7701 0300  ...MainWindow...
+00003de0: 0000 1400 4200 6500 6100 7200 6200 6500  ....B.e.a.r.b.e.
+00003df0: 6900 7400 6500 6e08 0000 0000 0600 0000  i.t.e.n.........
+00003e00: 0445 6469 7407 0000 000a 4d61 696e 5769  .Edit.....MainWi
+00003e10: 6e64 6f77 0103 0000 000e 0042 0065 0065  ndow.......B.e.e
+00003e20: 006e 0064 0065 006e 0800 0000 0006 0000  .n.d.e.n........
+00003e30: 0004 4578 6974 0700 0000 0a4d 6169 6e57  ..Exit.....MainW
+00003e40: 696e 646f 7701 03ff ffff ff08 0000 0000  indow...........
+00003e50: 0600 0000 0645 7870 6f72 7407 0000 000a  .....Export.....
+00003e60: 4d61 696e 5769 6e64 6f77 0103 0000 001c  MainWindow......
+00003e70: 0045 0078 0070 006f 0072 0074 0069 0065  .E.x.p.o.r.t.i.e
+00003e80: 0072 0065 006e 002e 002e 002e 0800 0000  .r.e.n..........
+00003e90: 0006 0000 0009 4578 706f 7274 2e2e 2e07  ......Export....
+00003ea0: 0000 000a 4d61 696e 5769 6e64 6f77 0103  ....MainWindow..
+00003eb0: 0000 000a 0044 0061 0074 0065 0069 0800  .....D.a.t.e.i..
+00003ec0: 0000 0006 0000 0004 4669 6c65 0700 0000  ........File....
+00003ed0: 0a4d 6169 6e57 696e 646f 7701 03ff ffff  .MainWindow.....
+00003ee0: ff08 0000 0000 0600 0000 0646 696c 7465  ...........Filte
+00003ef0: 7207 0000 000a 4d61 696e 5769 6e64 6f77  r.....MainWindow
+00003f00: 0103 0000 000a 0048 0069 006c 0066 0065  .......H.i.l.f.e
+00003f10: 0800 0000 0006 0000 0004 4865 6c70 0700  ..........Help..
+00003f20: 0000 0a4d 6169 6e57 696e 646f 7701 03ff  ...MainWindow...
+00003f30: ffff ff08 0000 0000 0600 0000 0649 6d70  .............Imp
+00003f40: 6f72 7407 0000 000a 4d61 696e 5769 6e64  ort.....MainWind
+00003f50: 6f77 0103 0000 001c 0049 006d 0070 006f  ow.......I.m.p.o
+00003f60: 0072 0074 0069 0065 0072 0065 006e 002e  .r.t.i.e.r.e.n..
+00003f70: 002e 002e 0800 0000 0006 0000 0009 496d  ..............Im
+00003f80: 706f 7274 2e2e 2e07 0000 000a 4d61 696e  port........Main
+00003f90: 5769 6e64 6f77 0103 0000 0018 004c 006f  Window.......L.o
+00003fa0: 0067 0067 0065 0020 0051 0053 004f 002e  .g.g.e. .Q.S.O..
+00003fb0: 002e 002e 0800 0000 0006 0000 000a 4c6f  ..............Lo
+00003fc0: 6720 5153 4f2e 2e2e 0700 0000 0a4d 6169  g QSO........Mai
+00003fd0: 6e57 696e 646f 7701 03ff ffff ff08 0000  nWindow.........
+00003fe0: 0000 0600 0000 044d 6f64 6507 0000 000a  .......Mode.....
+00003ff0: 4d61 696e 5769 6e64 6f77 0103 0000 0018  MainWindow......
+00004000: 0051 0053 004f 002d 0046 006f 0072 006d  .Q.S.O.-.F.o.r.m
+00004010: 0075 006c 0061 0072 0800 0000 0006 0000  .u.l.a.r........
+00004020: 0008 5153 4f20 466f 726d 0700 0000 0a4d  ..QSO Form.....M
+00004030: 6169 6e57 696e 646f 7701 0300 0000 2600  ainWindow.....&.
+00004040: 4400 6100 7400 6500 6e00 6200 6100 6e00  D.a.t.e.n.b.a.n.
+00004050: 6b00 2000 7700 e400 6800 6c00 6500 6e00  k. .w...h.l.e.n.
+00004060: 2e00 2e00 2e08 0000 0000 0600 0000 1253  ...............S
+00004070: 656c 6563 7420 6461 7461 6261 7365 2e2e  elect database..
+00004080: 2e07 0000 000a 4d61 696e 5769 6e64 6f77  ......MainWindow
+00004090: 0103 0000 001a 0045 0069 006e 0073 0074  .......E.i.n.s.t
+000040a0: 0065 006c 006c 0075 006e 0067 0065 006e  .e.l.l.u.n.g.e.n
+000040b0: 0800 0000 0006 0000 0008 5365 7474 696e  ..........Settin
+000040c0: 6773 0700 0000 0a4d 6169 6e57 696e 646f  gs.....MainWindo
+000040d0: 7701 0300 0000 2400 5a00 6500 6900 6700  w.....$.Z.e.i.g.
+000040e0: 6500 2000 4600 6900 6c00 7400 6500 7200  e. .F.i.l.t.e.r.
+000040f0: 6400 6900 6100 6c00 6f00 6708 0000 0000  d.i.a.l.o.g.....
+00004100: 0600 0000 0b53 686f 7720 6669 6c74 6572  .....Show filter
+00004110: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
+00004120: 0300 0000 2600 5a00 6500 6900 6700 6500  ....&.Z.e.i.g.e.
+00004130: 2000 4100 6e00 7700 6500 6e00 6400 7500   .A.n.w.e.n.d.u.
+00004140: 6e00 6700 7300 6c00 6f00 6708 0000 0000  n.g.s.l.o.g.....
+00004150: 0600 0000 0853 686f 7720 6c6f 6707 0000  .....Show log...
+00004160: 000a 4d61 696e 5769 6e64 6f77 0103 0000  ..MainWindow....
+00004170: 001a 0053 0074 0061 0072 0074 0065 0020  ...S.t.a.r.t.e. 
+00004180: 0048 0061 006d 006c 0069 0062 0800 0000  .H.a.m.l.i.b....
+00004190: 0006 0000 000c 5374 6172 7420 6861 6d6c  ......Start haml
+000041a0: 6962 0700 0000 0a4d 6169 6e57 696e 646f  ib.....MainWindo
+000041b0: 7701 0300 0000 1c00 5700 6500 7200 6b00  w.......W.e.r.k.
+000041c0: 7a00 6500 7500 6700 6c00 6500 6900 7300  z.e.u.g.l.e.i.s.
+000041d0: 7400 6508 0000 0000 0600 0000 0754 6f6f  t.e..........Too
+000041e0: 6c62 6172 0700 0000 0a4d 6169 6e57 696e  lbar.....MainWin
+000041f0: 646f 7701 0300 0000 3200 4c00 6f00 6700  dow.....2.L.o.g.
+00004200: 7300 2000 7a00 7500 2000 4c00 6f00 5400  s. .z.u. .L.o.T.
+00004210: 5700 2000 6800 6f00 6300 6800 6c00 6100  W. .h.o.c.h.l.a.
+00004220: 6400 6500 6e00 2e00 2e00 2e08 0000 0000  d.e.n...........
+00004230: 0600 0000 1655 706c 6f61 6420 6c6f 6773  .....Upload logs
+00004240: 2074 6f20 4c6f 5457 2e2e 2e07 0000 000a   to LoTW........
+00004250: 4d61 696e 5769 6e64 6f77 0103 0000 0042  MainWindow.....B
+00004260: 0044 0061 0074 0065 0069 0020 0061 0075  .D.a.t.e.i. .a.u
+00004270: 0066 0020 006e 0065 0075 0065 0020 0051  .f. .n.e.u.e. .Q
+00004280: 0053 004f 0073 0020 00fc 0062 0065 0072  .S.O.s. ...b.e.r
+00004290: 0077 0061 0063 0068 0065 006e 002e 002e  .w.a.c.h.e.n....
+000042a0: 002e 0800 0000 0006 0000 0016 5761 7463  ............Watc
+000042b0: 6820 6669 6c65 2066 6f72 2051 534f 732e  h file for QSOs.
+000042c0: 2e2e 0700 0000 0a4d 6169 6e57 696e 646f  .......MainWindo
+000042d0: 7701 0300 0000 1400 4a00 4a00 4a00 4a00  w.......J.J.J.J.
+000042e0: 2d00 4d00 4d00 2d00 5400 5408 0000 0000  -.M.M.-.T.T.....
+000042f0: 0600 0000 0a59 5959 592d 4d4d 2d44 4407  .....YYYY-MM-DD.
+00004300: 0000 000a 4d61 696e 5769 6e64 6f77 0103  ....MainWindow..
+00004310: ffff ffff 0800 0000 0006 0000 0002 2057  .............. W
+00004320: 0700 0000 0751 534f 466f 726d 0103 ffff  .....QSOForm....
+00004330: ffff 0800 0000 0006 0000 0004 206b 487a  ............ kHz
+00004340: 0700 0000 0751 534f 466f 726d 0103 ffff  .....QSOForm....
+00004350: ffff 0800 0000 0006 0000 0002 3539 0700  ............59..
+00004360: 0000 0751 534f 466f 726d 0103 0000 0048  ...QSOForm.....H
+00004370: 0045 0069 006e 0020 0046 0065 006c 0064  .E.i.n. .F.e.l.d
+00004380: 0020 0066 0065 0068 006c 0074 0020 0066  . .f.e.h.l.t. .f
+00004390: 00fc 0072 0020 0064 0069 0065 0020 0049  ...r. .d.i.e. .I
+000043a0: 006e 0062 006f 0078 002d 0050 0072 00fc  .n.b.o.x.-.P.r..
+000043b0: 0066 0075 006e 0067 0800 0000 0006 0000  .f.u.n.g........
+000043c0: 0022 4120 6669 656c 6420 6973 206d 6973  ."A field is mis
+000043d0: 7369 6e67 2066 6f72 2069 6e62 6f78 2063  sing for inbox c
+000043e0: 6865 636b 0700 0000 0751 534f 466f 726d  heck.....QSOForm
+000043f0: 0103 0000 0042 0046 0065 0068 006c 0065  .....B.F.e.h.l.e
+00004400: 006e 0064 0065 0073 0020 0046 0065 006c  .n.d.e.s. .F.e.l
+00004410: 0064 0020 0066 00fc 0072 0020 0064 0065  .d. .f...r. .d.e
+00004420: 006e 0020 004c 006f 0067 002d 0055 0070  .n. .L.o.g.-.U.p
+00004430: 006c 006f 0061 0064 0800 0000 0006 0000  .l.o.a.d........
+00004440: 0021 4120 6669 656c 6420 6973 206d 6973  .!A field is mis
+00004450: 7369 6e67 2066 6f72 206c 6f67 2075 706c  sing for log upl
+00004460: 6f61 6407 0000 0007 5153 4f46 6f72 6d01  oad.....QSOForm.
+00004470: 0300 0000 5600 4600 6500 6800 6c00 6500  ....V.F.e.h.l.e.
+00004480: 6e00 6400 6500 7300 2000 4600 6500 6c00  n.d.e.s. .F.e.l.
+00004490: 6400 2000 6600 fc00 7200 2000 6400 6500  d. .f...r. .d.e.
+000044a0: 6e00 2000 4c00 6f00 6700 2d00 5500 7000  n. .L.o.g.-.U.p.
+000044b0: 6c00 6f00 6100 6400 2000 7a00 7500 2000  l.o.a.d. .z.u. .
+000044c0: 4800 6100 6d00 5100 5400 4808 0000 0000  H.a.m.Q.T.H.....
+000044d0: 0600 0000 2b41 2066 6965 6c64 2069 7320  ....+A field is 
+000044e0: 6d69 7373 696e 6720 666f 7220 6c6f 6720  missing for log 
+000044f0: 7570 6c6f 6164 2074 6f20 4861 6d51 5448  upload to HamQTH
+00004500: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+00004510: 0016 0041 006b 007a 0065 0070 0074 0069  ...A.k.z.e.p.t.i
+00004520: 0065 0072 0074 003a 0800 0000 0006 0000  .e.r.t.:........
+00004530: 0008 4163 6365 7074 733a 0700 0000 0751  ..Accepts:.....Q
+00004540: 534f 466f 726d 0103 0000 006a 0045 0069  SOForm.....j.E.i
+00004550: 006e 0020 0046 0065 0068 006c 0065 0072  .n. .F.e.h.l.e.r
+00004560: 0020 0074 0072 0061 0074 0020 0077 00e4  . .t.r.a.t. .w..
+00004570: 0068 0072 0065 006e 0064 0020 0064 0065  .h.r.e.n.d. .d.e
+00004580: 0072 0020 00dc 0062 0065 0072 0074 0072  .r. ...b.e.r.t.r
+00004590: 0061 0067 0075 006e 0067 0020 007a 0075  .a.g.u.n.g. .z.u
+000045a0: 0020 0048 0061 006d 0051 0054 0048 0020  . .H.a.m.Q.T.H. 
+000045b0: 0061 0075 0066 0800 0000 0006 0000 0027  .a.u.f.........'
+000045c0: 416e 2065 7272 6f72 206f 6363 7572 6564  An error occured
+000045d0: 206f 6e20 7570 6c6f 6164 696e 6720 746f   on uploading to
+000045e0: 2048 616d 5154 4807 0000 0007 5153 4f46   HamQTH.....QSOF
+000045f0: 6f72 6d01 0300 0000 1600 4100 7500 7400  orm.......A.u.t.
+00004600: 6f00 6d00 6100 7400 6900 7300 6300 6808  o.m.a.t.i.s.c.h.
+00004610: 0000 0000 0600 0000 0d41 7574 6f6d 6174  .........Automat
+00004620: 6963 616c 6c79 0700 0000 0751 534f 466f  ically.....QSOFo
+00004630: 726d 0103 0000 0038 0046 0065 0068 006c  rm.....8.F.e.h.l
+00004640: 0065 0072 0068 0061 0066 0074 0065 0073  .e.r.h.a.f.t.e.s
+00004650: 0020 0041 0062 0066 0072 0061 0067 0065  . .A.b.f.r.a.g.e
+00004660: 0065 0072 0067 0065 0062 006e 0069 0073  .e.r.g.e.b.n.i.s
+00004670: 0800 0000 0006 0000 0012 4261 6420 7265  ..........Bad re
+00004680: 7175 6573 7420 7265 7375 6c74 0700 0000  quest result....
+00004690: 0751 534f 466f 726d 0103 ffff ffff 0800  .QSOForm........
+000046a0: 0000 0006 0000 0004 4261 6e64 0700 0000  ........Band....
+000046b0: 0751 534f 466f 726d 0103 0000 0008 0042  .QSOForm.......B
+000046c0: 00fc 0072 006f 0800 0000 0006 0000 0006  ...r.o..........
+000046d0: 4275 7265 6175 0700 0000 0751 534f 466f  Bureau.....QSOFo
+000046e0: 726d 0103 0000 0016 0042 00fc 0072 006f  rm.......B...r.o
+000046f0: 002f 0044 0069 0072 0065 006b 0074 0800  ./.D.i.r.e.k.t..
+00004700: 0000 0006 0000 000d 4275 7265 6175 2f44  ........Bureau/D
+00004710: 6972 6563 7407 0000 0007 5153 4f46 6f72  irect.....QSOFor
+00004720: 6d01 0300 0000 1400 5200 7500 6600 7a00  m.......R.u.f.z.
+00004730: 6500 6900 6300 6800 6500 6e08 0000 0000  e.i.c.h.e.n.....
+00004740: 0600 0000 0943 616c 6c20 7369 676e 0700  .....Call sign..
+00004750: 0000 0751 534f 466f 726d 0103 0000 003c  ...QSOForm.....<
+00004760: 0046 0065 0068 006c 0065 0072 0020 0062  .F.e.h.l.e.r. .b
+00004770: 0065 0069 0020 0064 0065 0072 0020 0052  .e.i. .d.e.r. .R
+00004780: 0075 0066 007a 0065 0069 0063 0068 0065  .u.f.z.e.i.c.h.e
+00004790: 006e 0073 0075 0063 0068 0065 0800 0000  .n.s.u.c.h.e....
+000047a0: 0006 0000 0015 4361 6c6c 626f 6f6b 2073  ......Callbook s
+000047b0: 6561 7263 6820 6572 726f 7207 0000 0007  earch error.....
+000047c0: 5153 4f46 6f72 6d01 0300 0000 2a00 4300  QSOForm.....*.C.
+000047d0: 6100 6c00 6c00 6200 6f00 6f00 6b00 2d00  a.l.l.b.o.o.k.-.
+000047e0: 5300 7500 6300 6800 6500 7200 6700 6500  S.u.c.h.e.r.g.e.
+000047f0: 6200 6e00 6900 7308 0000 0000 0600 0000  b.n.i.s.........
+00004800: 1643 616c 6c62 6f6f 6b20 7365 6172 6368  .Callbook search
+00004810: 2072 6573 756c 7407 0000 0007 5153 4f46   result.....QSOF
+00004820: 6f72 6d01 0300 0000 3200 5200 7500 6600  orm.....2.R.u.f.
+00004830: 7a00 6500 6900 6300 6800 6500 6e00 2000  z.e.i.c.h.e.n. .
+00004840: 6e00 6900 6300 6800 7400 2000 6700 6500  n.i.c.h.t. .g.e.
+00004850: 6600 7500 6e00 6400 6500 6e08 0000 0000  f.u.n.d.e.n.....
+00004860: 0600 0000 1243 616c 6c73 6967 6e20 6e6f  .....Callsign no
+00004870: 7420 666f 756e 6407 0000 0007 5153 4f46  t found.....QSOF
+00004880: 6f72 6d01 0300 0000 0a00 4b00 6100 6e00  orm.......K.a.n.
+00004890: 6100 6c08 0000 0000 0600 0000 0743 6861  a.l..........Cha
+000048a0: 6e6e 656c 0700 0000 0751 534f 466f 726d  nnel.....QSOForm
+000048b0: 0103 0000 0016 0050 0072 00fc 0066 0065  .......P.r...f.e
+000048c0: 0020 0049 006e 0062 006f 0078 0800 0000  . .I.n.b.o.x....
+000048d0: 0006 0000 000b 4368 6563 6b20 496e 626f  ......Check Inbo
+000048e0: 7807 0000 0007 5153 4f46 6f72 6d01 0300  x.....QSOForm...
+000048f0: 0000 4200 4600 6500 6800 6c00 6500 7200  ..B.F.e.h.l.e.r.
+00004900: 2000 6200 6500 6900 6d00 2000 5000 7200   .b.e.i.m. .P.r.
+00004910: fc00 6600 6500 6e00 2000 6400 6500 7200  ..f.e.n. .d.e.r.
+00004920: 2000 4c00 6f00 5400 5700 2d00 4900 6e00   .L.o.T.W.-.I.n.
+00004930: 6200 6f00 7808 0000 0000 0600 0000 1643  b.o.x..........C
+00004940: 6865 636b 204c 6f54 5720 496e 626f 7820  heck LoTW Inbox 
+00004950: 6572 726f 7207 0000 0007 5153 4f46 6f72  error.....QSOFor
+00004960: 6d01 0300 0000 1c00 5000 7200 fc00 6600  m.......P.r...f.
+00004970: 6500 2000 4c00 6f00 5400 5700 2000 5100  e. .L.o.T.W. .Q.
+00004980: 5300 4c08 0000 0000 0600 0000 0e43 6865  S.L..........Che
+00004990: 636b 204c 6f54 5720 5153 4c07 0000 0007  ck LoTW QSL.....
+000049a0: 5153 4f46 6f72 6d01 0300 0000 3800 6500  QSOForm.....8.e.
+000049b0: 5100 5300 4c00 2d00 4600 6500 6800 6c00  Q.S.L.-.F.e.h.l.
+000049c0: 6500 7200 2000 7000 7200 fc00 6600 6500  e.r. .p.r...f.e.
+000049d0: 6e00 2000 6400 6500 7200 2000 4900 6e00  n. .d.e.r. .I.n.
+000049e0: 6200 6f00 7808 0000 0000 0600 0000 1643  b.o.x..........C
+000049f0: 6865 636b 2065 5153 4c20 496e 626f 7820  heck eQSL Inbox 
+00004a00: 6572 726f 7207 0000 0007 5153 4f46 6f72  error.....QSOFor
+00004a10: 6d01 0300 0000 1800 5a00 7500 7200 fc00  m.......Z.u.r...
+00004a20: 6300 6b00 7300 6500 7400 7a00 6500 6e08  c.k.s.e.t.z.e.n.
+00004a30: 0000 0000 0600 0000 0543 6c65 6172 0700  .........Clear..
+00004a40: 0000 0751 534f 466f 726d 0103 0000 0020  ...QSOForm..... 
+00004a50: 004b 006f 006e 0066 0069 0067 0075 0072  .K.o.n.f.i.g.u.r
+00004a60: 0069 0065 0072 0074 0065 0020 0049 0044  .i.e.r.t.e. .I.D
+00004a70: 0800 0000 0006 0000 0013 436f 6e66 6967  ..........Config
+00004a80: 7572 6564 2069 6465 6e74 6974 7907 0000  ured identity...
+00004a90: 0007 5153 4f46 6f72 6d01 0300 0000 2a00  ..QSOForm.....*.
+00004aa0: 4b00 6f00 6e00 6600 6900 6700 7500 7200  K.o.n.f.i.g.u.r.
+00004ab0: 6900 6500 7200 7400 6500 2000 5300 7400  i.e.r.t.e. .S.t.
+00004ac0: 6100 7400 6900 6f00 6e08 0000 0000 0600  a.t.i.o.n.......
+00004ad0: 0000 1243 6f6e 6669 6775 7265 6420 7374  ...Configured st
+00004ae0: 6174 696f 6e07 0000 0007 5153 4f46 6f72  ation.....QSOFor
+00004af0: 6d01 03ff ffff ff08 0000 0000 0600 0000  m...............
+00004b00: 0743 6f6e 7465 7374 0700 0000 0751 534f  .Contest.....QSO
+00004b10: 466f 726d 0103 ffff ffff 0800 0000 0006  Form............
+00004b20: 0000 000a 436f 6e74 6573 7420 4944 0700  ....Contest ID..
+00004b30: 0000 0751 534f 466f 726d 0103 ffff ffff  ...QSOForm......
+00004b40: 0800 0000 0006 0000 000a 4374 726c 2b41  ..........Ctrl+A
+00004b50: 6c74 2b45 0700 0000 0751 534f 466f 726d  lt+E.....QSOForm
+00004b60: 0103 ffff ffff 0800 0000 0006 0000 000a  ................
+00004b70: 4374 726c 2b41 6c74 2b48 0700 0000 0751  Ctrl+Alt+H.....Q
+00004b80: 534f 466f 726d 0103 ffff ffff 0800 0000  SOForm..........
+00004b90: 0006 0000 000a 4374 726c 2b41 6c74 2b49  ......Ctrl+Alt+I
+00004ba0: 0700 0000 0751 534f 466f 726d 0103 ffff  .....QSOForm....
+00004bb0: ffff 0800 0000 0006 0000 000a 4374 726c  ............Ctrl
+00004bc0: 2b41 6c74 2b4e 0700 0000 0751 534f 466f  +Alt+N.....QSOFo
+00004bd0: 726d 0103 ffff ffff 0800 0000 0006 0000  rm..............
+00004be0: 000a 4374 726c 2b41 6c74 2b5a 0700 0000  ..Ctrl+Alt+Z....
+00004bf0: 0751 534f 466f 726d 0103 ffff ffff 0800  .QSOForm........
+00004c00: 0000 0006 0000 0006 4374 726c 2b53 0700  ........Ctrl+S..
+00004c10: 0000 0751 534f 466f 726d 0103 ffff ffff  ...QSOForm......
+00004c20: 0800 0000 0006 0000 000c 4374 726c 2b53  ..........Ctrl+S
+00004c30: 6869 6674 2b45 0700 0000 0751 534f 466f  hift+E.....QSOFo
+00004c40: 726d 0103 ffff ffff 0800 0000 0006 0000  rm..............
+00004c50: 0006 4374 726c 2b55 0700 0000 0751 534f  ..Ctrl+U.....QSO
+00004c60: 466f 726d 0103 0000 0016 0045 006d 0070  Form.......E.m.p
+00004c70: 0066 002e 0020 0044 0061 0074 0065 006e  .f... .D.a.t.e.n
+00004c80: 0800 0000 0006 0000 0004 4461 7461 0700  ..........Data..
+00004c90: 0000 0751 534f 466f 726d 0103 0000 000c  ...QSOForm......
+00004ca0: 0064 0069 0072 0065 006b 0074 0800 0000  .d.i.r.e.k.t....
+00004cb0: 0006 0000 0006 4469 7265 6374 0700 0000  ......Direct....
+00004cc0: 0751 534f 466f 726d 0103 0000 001c 0065  .QSOForm.......e
+00004cd0: 0051 0053 004c 0020 0073 0070 0065 0069  .Q.S.L. .s.p.e.i
+00004ce0: 0063 0068 0065 0072 006e 0800 0000 0006  .c.h.e.r.n......
+00004cf0: 0000 000d 446f 776e 6c6f 6164 2065 5153  ....Download eQS
+00004d00: 4c07 0000 0007 5153 4f46 6f72 6d01 0300  L.....QSOForm...
+00004d10: 0000 6c00 5700 e400 6800 7200 6500 6e00  ..l.W...h.r.e.n.
+00004d20: 6400 2000 6400 6500 7200 2000 5200 7500  d. .d.e.r. .R.u.
+00004d30: 6600 7a00 6500 6900 6300 6800 6500 6e00  f.z.e.i.c.h.e.n.
+00004d40: 7300 7500 6300 6800 6500 2000 6900 7300  s.u.c.h.e. .i.s.
+00004d50: 7400 2000 6500 6900 6e00 2000 4600 6500  t. .e.i.n. .F.e.
+00004d60: 6800 6c00 6500 7200 2000 6100 7500 6600  h.l.e.r. .a.u.f.
+00004d70: 6700 6500 7400 7200 6500 7400 6500 6e08  g.e.t.r.e.t.e.n.
+00004d80: 0000 0000 0600 0000 2744 7572 696e 6720  ........'During 
+00004d90: 6361 6c6c 626f 6f6b 2073 6561 7263 6820  callbook search 
+00004da0: 616e 2065 7272 6f72 206f 6363 7572 6564  an error occured
+00004db0: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+00004dc0: 0008 0045 006e 0064 0065 0800 0000 0006  ...E.n.d.e......
+00004dd0: 0000 0003 456e 6407 0000 0007 5153 4f46  ....End.....QSOF
+00004de0: 6f72 6d01 0300 0000 0c00 4600 6500 6800  orm.......F.e.h.
+00004df0: 6c00 6500 7208 0000 0000 0600 0000 0545  l.e.r..........E
+00004e00: 7272 6f72 0700 0000 0751 534f 466f 726d  rror.....QSOForm
+00004e10: 0103 0000 0024 0065 0051 0053 004c 002d  .....$.e.Q.S.L.-
+00004e20: 0055 0070 006c 006f 0061 0064 002d 0046  .U.p.l.o.a.d.-.F
+00004e30: 0065 0068 006c 0065 0072 0800 0000 0006  .e.h.l.e.r......
+00004e40: 0000 000f 4572 726f 7220 6f6e 2075 706c  ....Error on upl
+00004e50: 6f61 6407 0000 0007 5153 4f46 6f72 6d01  oad.....QSOForm.
+00004e60: 0300 0000 1000 4600 7200 6500 7100 7500  ......F.r.e.q.u.
+00004e70: 6500 6e00 7a08 0000 0000 0600 0000 0946  e.n.z..........F
+00004e80: 7265 7175 656e 6379 0700 0000 0751 534f  requency.....QSO
+00004e90: 466f 726d 0103 ffff ffff 0800 0000 0006  Form............
+00004ea0: 0000 0006 4861 6d51 5448 0700 0000 0751  ....HamQTH.....Q
+00004eb0: 534f 466f 726d 0103 0000 0004 0049 0044  SOForm.......I.D
+00004ec0: 0800 0000 0006 0000 0008 4964 656e 7469  ..........Identi
+00004ed0: 7479 0700 0000 0751 534f 466f 726d 0103  ty.....QSOForm..
+00004ee0: 0000 0026 004c 0069 006e 006b 0020 007a  ...&.L.i.n.k. .z
+00004ef0: 0075 0072 0020 0065 0051 0053 004c 002d  .u.r. .e.Q.S.L.-
+00004f00: 004b 0061 0072 0074 0065 0800 0000 0006  .K.a.r.t.e......
+00004f10: 0000 0011 4c69 6e6b 2074 6f20 6551 534c  ....Link to eQSL
+00004f20: 2043 6172 6407 0000 0007 5153 4f46 6f72   Card.....QSOFor
+00004f30: 6d01 03ff ffff ff08 0000 0000 0600 0000  m...............
+00004f40: 044c 6f54 5707 0000 0007 5153 4f46 6f72  .LoTW.....QSOFor
+00004f50: 6d01 0300 0000 1c00 4c00 6f00 5400 5700  m.......L.o.T.W.
+00004f60: 2000 6500 6d00 7000 6600 6100 6e00 6700   .e.m.p.f.a.n.g.
+00004f70: 6500 6e08 0000 0000 0600 0000 0d4c 6f54  e.n..........LoT
+00004f80: 5720 7265 6365 6976 6564 0700 0000 0751  W received.....Q
+00004f90: 534f 466f 726d 0103 0000 001c 004c 006f  SOForm.......L.o
+00004fa0: 0054 0057 0020 0076 0065 0072 0073 0065  .T.W. .v.e.r.s.e
+00004fb0: 006e 0064 0065 0074 0800 0000 0006 0000  .n.d.e.t........
+00004fc0: 0009 4c6f 5457 2073 656e 7407 0000 0007  ..LoTW sent.....
+00004fd0: 5153 4f46 6f72 6d01 03ff ffff ff08 0000  QSOForm.........
+00004fe0: 0000 0600 0000 074c 6f63 6174 6f72 0700  .......Locator..
+00004ff0: 0000 0751 534f 466f 726d 0103 ffff ffff  ...QSOForm......
+00005000: 0800 0000 0006 0000 0007 4c6f 6762 6f6f  ..........Logboo
+00005010: 6b07 0000 0007 5153 4f46 6f72 6d01 0300  k.....QSOForm...
+00005020: 0000 4200 4c00 6f00 6700 6900 6e00 2000  ..B.L.o.g.i.n. .
+00005030: 6600 6500 6800 6c00 6700 6500 7300 6300  f.e.h.l.g.e.s.c.
+00005040: 6800 6c00 6100 6700 6500 6e00 2000 6600  h.l.a.g.e.n. .f.
+00005050: fc00 7200 2000 4200 6500 6e00 7500 7400  ..r. .B.e.n.u.t.
+00005060: 7a00 6500 7208 0000 0000 0600 0000 154c  z.e.r..........L
+00005070: 6f67 696e 2066 6169 6c65 6420 666f 7220  ogin failed for 
+00005080: 7573 6572 0700 0000 0751 534f 466f 726d  user.....QSOForm
+00005090: 0103 0000 0058 004c 006f 0067 0069 006e  .....X.L.o.g.i.n
+000050a0: 0020 0062 0065 0069 0020 0048 0061 006d  . .b.e.i. .H.a.m
+000050b0: 0051 0054 0048 0020 0066 0065 0068 006c  .Q.T.H. .f.e.h.l
+000050c0: 0067 0065 0073 0063 0068 006c 0061 0067  .g.e.s.c.h.l.a.g
+000050d0: 0065 006e 0020 0066 00fc 0072 0020 0042  .e.n. .f...r. .B
+000050e0: 0065 006e 0075 0074 007a 0065 0072 0800  .e.n.u.t.z.e.r..
+000050f0: 0000 0006 0000 001f 4c6f 6769 6e20 746f  ........Login to
+00005100: 2048 616d 5154 4820 6661 696c 6564 2066   HamQTH failed f
+00005110: 6f72 2075 7365 7207 0000 0007 5153 4f46  or user.....QSOF
+00005120: 6f72 6d01 0300 0000 1400 4800 6100 7500  orm.......H.a.u.
+00005130: 7000 7400 6400 6100 7400 6500 6e08 0000  p.t.d.a.t.e.n...
+00005140: 0000 0600 0000 094d 6169 6e20 6461 7461  .......Main data
+00005150: 0700 0000 0751 534f 466f 726d 0103 ffff  .....QSOForm....
+00005160: ffff 0800 0000 0006 0000 0004 4d6f 6465  ............Mode
+00005170: 0700 0000 0751 534f 466f 726d 0103 ffff  .....QSOForm....
+00005180: ffff 0800 0000 0006 0000 0004 4e61 6d65  ............Name
+00005190: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+000051a0: 0024 004b 0065 0069 006e 0020 0051 0053  .$.K.e.i.n. .Q.S
+000051b0: 004c 0020 0076 0065 0072 0066 00fc 0067  .L. .v.e.r.f...g
+000051c0: 0062 0061 0072 0800 0000 0006 0000 0010  .b.a.r..........
+000051d0: 4e6f 2051 534c 2061 7661 696c 6162 6c65  No QSL available
+000051e0: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+000051f0: 0026 004b 0065 0069 006e 0020 0065 0051  .&.K.e.i.n. .e.Q
+00005200: 0053 004c 0020 0076 0065 0072 0066 00fc  .S.L. .v.e.r.f..
+00005210: 0067 0062 0061 0072 0800 0000 0006 0000  .g.b.a.r........
+00005220: 0011 4e6f 2065 5153 4c20 6176 6169 6c61  ..No eQSL availa
+00005230: 626c 6507 0000 0007 5153 4f46 6f72 6d01  ble.....QSOForm.
+00005240: 0300 0000 0a00 4a00 6500 7400 7a00 7408  ......J.e.t.z.t.
+00005250: 0000 0000 0600 0000 034e 6f77 0700 0000  .........Now....
+00005260: 0751 534f 466f 726d 0103 0000 0024 0045  .QSOForm.....$.E
+00005270: 0069 0067 0065 006e 0065 0073 0020 0052  .i.g.e.n.e.s. .R
+00005280: 0075 0066 007a 0065 0069 0063 0068 0065  .u.f.z.e.i.c.h.e
+00005290: 006e 0800 0000 0006 0000 000d 4f77 6e20  .n..........Own 
+000052a0: 6361 6c6c 2073 6967 6e07 0000 0007 5153  call sign.....QS
+000052b0: 4f46 6f72 6d01 0300 0000 1800 4500 6900  OForm.......E.i.
+000052c0: 6700 6500 6e00 6500 7200 2000 4e00 6100  g.e.n.e.r. .N.a.
+000052d0: 6d00 6508 0000 0000 0600 0000 084f 776e  m.e..........Own
+000052e0: 206e 616d 6507 0000 0007 5153 4f46 6f72   name.....QSOFor
+000052f0: 6d01 0300 0000 1c00 4500 6900 6700 6500  m.......E.i.g.e.
+00005300: 6e00 6500 2000 4e00 6f00 7400 6900 7a00  n.e. .N.o.t.i.z.
+00005310: 6500 6e08 0000 0000 0600 0000 094f 776e  e.n..........Own
+00005320: 206e 6f74 6573 0700 0000 0751 534f 466f   notes.....QSOFo
+00005330: 726d 0103 0000 0010 004c 0065 0069 0073  rm.......L.e.i.s
+00005340: 0074 0075 006e 0067 0800 0000 0006 0000  .t.u.n.g........
+00005350: 0005 506f 7765 7207 0000 0007 5153 4f46  ..Power.....QSOF
+00005360: 6f72 6d01 0300 0000 1e00 4100 7500 7300  orm.......A.u.s.
+00005370: 6200 7200 6500 6900 7400 7500 6e00 6700  b.r.e.i.t.u.n.g.
+00005380: 7300 6100 7200 7408 0000 0000 0600 0000  s.a.r.t.........
+00005390: 0b50 726f 7061 6761 7469 6f6e 0700 0000  .Propagation....
+000053a0: 0751 534f 466f 726d 0103 ffff ffff 0800  .QSOForm........
+000053b0: 0000 0006 0000 0005 5152 5a43 5107 0000  ........QRZCQ...
+000053c0: 0007 5153 4f46 6f72 6d01 03ff ffff ff08  ..QSOForm.......
+000053d0: 0000 0000 0600 0000 0351 534c 0700 0000  .........QSL....
+000053e0: 0751 534f 466f 726d 0103 0000 0022 0051  .QSOForm.....".Q
+000053f0: 0053 004c 0020 0026 0026 0020 004c 006f  .S.L. .&.&. .L.o
+00005400: 0067 002d 0055 0070 006c 006f 0061 0064  .g.-.U.p.l.o.a.d
+00005410: 0800 0000 0006 0000 0011 5153 4c20 2626  ..........QSL &&
+00005420: 204c 6f67 2075 706c 6f61 6407 0000 0007   Log upload.....
+00005430: 5153 4f46 6f72 6d01 0300 0000 1c00 5100  QSOForm.......Q.
+00005440: 5300 4c00 2d00 4b00 6100 7200 7400 6500  S.L.-.K.a.r.t.e.
+00005450: 6e00 7400 6500 7800 7408 0000 0000 0600  n.t.e.x.t.......
+00005460: 0000 1051 534c 2063 6172 6420 6d65 7373  ...QSL card mess
+00005470: 6167 6507 0000 0007 5153 4f46 6f72 6d01  age.....QSOForm.
+00005480: 0300 0000 1a00 5100 5300 4c00 2000 6500  ......Q.S.L. .e.
+00005490: 6d00 7000 6600 6100 6e00 6700 6500 6e08  m.p.f.a.n.g.e.n.
+000054a0: 0000 0000 0600 0000 0c51 534c 2072 6563  .........QSL rec
+000054b0: 6569 7665 6407 0000 0007 5153 4f46 6f72  eived.....QSOFor
+000054c0: 6d01 0300 0000 1800 5100 5300 4c00 2000  m.......Q.S.L. .
+000054d0: 6700 6500 7300 6500 6e00 6400 6500 7408  g.e.s.e.n.d.e.t.
+000054e0: 0000 0000 0600 0000 0851 534c 2073 656e  .........QSL sen
+000054f0: 7407 0000 0007 5153 4f46 6f72 6d01 0300  t.....QSOForm...
+00005500: 0000 0e00 5100 5300 4c00 2d00 5600 6900  ....Q.S.L.-.V.i.
+00005510: 6108 0000 0000 0600 0000 0751 534c 2076  a..........QSL v
+00005520: 6961 0700 0000 0751 534f 466f 726d 0103  ia.....QSOForm..
+00005530: 0000 0018 0051 0053 004f 002d 0046 006f  .....Q.S.O.-.F.o
+00005540: 0072 006d 0075 006c 0061 0072 0800 0000  .r.m.u.l.a.r....
+00005550: 0006 0000 0008 5153 4f20 466f 726d 0700  ......QSO Form..
+00005560: 0000 0751 534f 466f 726d 0103 0000 001a  ...QSOForm......
+00005570: 0051 0053 004f 002d 004b 006f 006d 006d  .Q.S.O.-.K.o.m.m
+00005580: 0065 006e 0074 0061 0072 0800 0000 0006  .e.n.t.a.r......
+00005590: 0000 000b 5153 4f20 636f 6d6d 656e 7407  ....QSO comment.
+000055a0: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
+000055b0: 3e00 5100 5300 4f00 2000 7700 7500 7200  >.Q.S.O. .w.u.r.
+000055c0: 6400 6500 2000 7600 6f00 6e00 2000 4800  d.e. .v.o.n. .H.
+000055d0: 6100 6d00 5100 5400 4800 2000 6100 6200  a.m.Q.T.H. .a.b.
+000055e0: 6700 6500 7700 6900 6500 7300 6500 6e08  g.e.w.i.e.s.e.n.
+000055f0: 0000 0000 0600 0000 1651 534f 2072 656a  .........QSO rej
+00005600: 6563 7465 6420 6f6e 2048 616d 5154 4807  ected on HamQTH.
+00005610: 0000 0007 5153 4f46 6f72 6d01 03ff ffff  ....QSOForm.....
+00005620: ff08 0000 0000 0600 0000 0351 5448 0700  ...........QTH..
+00005630: 0000 0751 534f 466f 726d 0103 ffff ffff  ...QSOForm......
+00005640: 0800 0000 0006 0000 0006 5253 5420 5278  ..........RST Rx
+00005650: 0700 0000 0751 534f 466f 726d 0103 ffff  .....QSOForm....
+00005660: ffff 0800 0000 0006 0000 0006 5253 5420  ............RST 
+00005670: 5478 0700 0000 0751 534f 466f 726d 0103  Tx.....QSOForm..
+00005680: 0000 001a 0052 0053 0054 0020 0065 006d  .....R.S.T. .e.m
+00005690: 0070 0066 0061 006e 0067 0065 006e 0800  .p.f.a.n.g.e.n..
+000056a0: 0000 0006 0000 000c 5253 5420 7265 6365  ........RST rece
+000056b0: 6976 6564 0700 0000 0751 534f 466f 726d  ived.....QSOForm
+000056c0: 0103 0000 0018 0052 0053 0054 0020 0067  .......R.S.T. .g
+000056d0: 0065 0073 0065 006e 0064 0065 0074 0800  .e.s.e.n.d.e.t..
+000056e0: 0000 0006 0000 0008 5253 5420 7365 6e74  ........RST sent
+000056f0: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+00005700: 0018 0045 006d 0070 0066 002e 0020 0051  ...E.m.p.f... .Q
+00005710: 0053 004f 0020 0049 0044 0800 0000 0006  .S.O. .I.D......
+00005720: 0000 000b 5263 7664 2051 534f 2049 4407  ....Rcvd QSO ID.
+00005730: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
+00005740: 1200 5300 7000 6500 6900 6300 6800 6500  ..S.p.e.i.c.h.e.
+00005750: 7200 6e08 0000 0000 0600 0000 0453 6176  r.n..........Sav
+00005760: 6507 0000 0007 5153 4f46 6f72 6d01 0300  e.....QSOForm...
+00005770: 0000 2600 5300 7000 6500 6900 6300 6800  ..&.S.p.e.i.c.h.
+00005780: 6500 7200 6e00 2000 2600 2600 2000 5500  e.r.n. .&.&. .U.
+00005790: 7000 6c00 6f00 6100 6408 0000 0000 0600  p.l.o.a.d.......
+000057a0: 0000 0e53 6176 6520 2626 2055 706c 6f61  ...Save && Uploa
+000057b0: 6407 0000 0007 5153 4f46 6f72 6d01 0300  d.....QSOForm...
+000057c0: 0000 2a00 6500 5100 5300 4c00 2d00 4f00  ..*.e.Q.S.L.-.O.
+000057d0: 7200 6400 6e00 6500 7200 2000 6100 7500  r.d.n.e.r. .a.u.
+000057e0: 7300 7700 e400 6800 6c00 6500 6e08 0000  s.w...h.l.e.n...
+000057f0: 0000 0600 0000 1253 656c 6563 7420 6551  .......Select eQ
+00005800: 534c 2066 6f6c 6465 7207 0000 0007 5153  SL folder.....QS
+00005810: 4f46 6f72 6d01 0300 0000 1600 4700 6500  OForm.......G.e.
+00005820: 7300 2e00 2000 5100 5300 4f00 2000 4900  s... .Q.S.O. .I.
+00005830: 4408 0000 0000 0600 0000 0b53 656e 7420  D..........Sent 
+00005840: 5153 4f20 4944 0700 0000 0751 534f 466f  QSO ID.....QSOFo
+00005850: 726d 0103 0000 0036 0053 0065 0072 0076  rm.....6.S.e.r.v
+00005860: 0065 0072 006b 006f 006d 006d 0075 006e  .e.r.k.o.m.m.u.n
+00005870: 0069 006b 0061 0074 0069 006f 006e 0073  .i.k.a.t.i.o.n.s
+00005880: 002d 0046 0065 0068 006c 0065 0072 0800  .-.F.e.h.l.e.r..
+00005890: 0000 0006 0000 001a 5365 7276 6572 2063  ........Server c
+000058a0: 6f6d 6d75 6e69 6361 7469 6f6e 2065 7272  ommunication err
+000058b0: 6f72 0700 0000 0751 534f 466f 726d 0103  or.....QSOForm..
+000058c0: ffff ffff 0800 0000 0006 0000 0005 5374  ..............St
+000058d0: 6172 7407 0000 0007 5153 4f46 6f72 6d01  art.....QSOForm.
+000058e0: 03ff ffff ff08 0000 0000 0600 0000 0753  ...............S
+000058f0: 7461 7469 6f6e 0700 0000 0751 534f 466f  tation.....QSOFo
+00005900: 726d 0103 ffff ffff 0800 0000 0006 0000  rm..............
+00005910: 0007 5375 626d 6f64 6507 0000 0007 5153  ..Submode.....QS
+00005920: 4f46 6f72 6d01 0300 0000 3000 4400 6100  OForm.....0.D.a.
+00005930: 7300 2000 5100 5300 4f00 2000 6900 7300  s. .Q.S.O. .i.s.
+00005940: 7400 2000 6500 6900 6e00 2000 4400 7500  t. .e.i.n. .D.u.
+00005950: 7000 6c00 6900 6b00 6100 7408 0000 0000  p.l.i.k.a.t.....
+00005960: 0600 0000 1654 6865 2051 534f 2069 7320  .....The QSO is 
+00005970: 6120 6475 706c 6963 6174 6507 0000 0007  a duplicate.....
+00005980: 5153 4f46 6f72 6d01 0300 0000 b800 4400  QSOForm.......D.
+00005990: 6900 6500 2000 5100 5300 4c00 2d00 5200  i.e. .Q.S.L.-.R.
+000059a0: 6f00 7500 7400 6500 2000 6400 6500 7200  o.u.t.e. .d.e.r.
+000059b0: 2000 6b00 6f00 6e00 7400 6100 6b00 7400   .k.o.n.t.a.k.t.
+000059c0: 6900 6500 7200 7400 6500 6e00 2000 5300  i.e.r.t.e.n. .S.
+000059d0: 7400 6100 7400 6900 6f00 6e00 2e00 0a00  t.a.t.i.o.n.....
+000059e0: 4400 6900 6500 7300 2000 6900 7300 7400  D.i.e.s. .i.s.t.
+000059f0: 2000 6e00 6900 6300 6800 7400 2000 6400   .n.i.c.h.t. .d.
+00005a00: 6900 6500 2000 4100 6400 7200 6500 7300  i.e. .A.d.r.e.s.
+00005a10: 7300 6500 2000 6400 6500 7300 2000 5100  s.e. .d.e.s. .Q.
+00005a20: 5300 4c00 2d00 4d00 6100 6e00 6100 6700  S.L.-.M.a.n.a.g.
+00005a30: 6500 7200 7300 2f00 2d00 4200 fc00 7200  e.r.s./.-.B...r.
+00005a40: 6f00 7300 2e08 0000 0000 0600 0000 4c54  o.s...........LT
+00005a50: 6865 2063 6f6e 7461 6374 6564 2073 7461  he contacted sta
+00005a60: 7469 6f6e 2051 534c 2072 6f75 7465 2e0a  tion QSL route..
+00005a70: 5468 6973 2069 7320 6e6f 7420 7468 6520  This is not the 
+00005a80: 5153 4c20 6d61 6e61 6765 722f 6275 7265  QSL manager/bure
+00005a90: 6175 2061 6464 7265 7373 2e07 0000 0007  au address......
+00005aa0: 5153 4f46 6f72 6d01 0300 0000 1000 4500  QSOForm.......E.
+00005ab0: 6e00 6400 6500 7a00 6500 6900 7408 0000  n.d.e.z.e.i.t...
+00005ac0: 0000 0600 0000 0854 696d 6520 656e 6407  .......Time end.
+00005ad0: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
+00005ae0: 1200 5300 7400 6100 7200 7400 7a00 6500  ..S.t.a.r.t.z.e.
+00005af0: 6900 7408 0000 0000 0600 0000 0a54 696d  i.t..........Tim
+00005b00: 6520 7374 6172 7407 0000 0007 5153 4f46  e start.....QSOF
+00005b10: 6f72 6d01 0300 0000 2400 6500 5100 5300  orm.....$.e.Q.S.
+00005b20: 4c00 2d00 5500 7000 6c00 6f00 6100 6400  L.-.U.p.l.o.a.d.
+00005b30: 2d00 4600 6500 6800 6c00 6500 7208 0000  -.F.e.h.l.e.r...
+00005b40: 0000 0600 0000 1155 706c 6f61 6420 6551  .......Upload eQ
+00005b50: 534c 2065 7272 6f72 0700 0000 0751 534f  SL error.....QSO
+00005b60: 466f 726d 0103 0000 001a 0055 0070 006c  Form.......U.p.l
+00005b70: 006f 0061 0064 002d 0046 0065 0068 006c  .o.a.d.-.F.e.h.l
+00005b80: 0065 0072 0800 0000 0006 0000 0010 5570  .e.r..........Up
+00005b90: 6c6f 6164 206c 6f67 2065 7272 6f72 0700  load log error..
+00005ba0: 0000 0751 534f 466f 726d 0103 0000 0068  ...QSOForm.....h
+00005bb0: 0055 0070 006c 006f 0061 0064 0020 0065  .U.p.l.o.a.d. .e
+00005bc0: 0072 0066 006f 006c 0067 0074 0020 006e  .r.f.o.l.g.t. .n
+00005bd0: 0075 0072 0020 0077 0065 006e 006e 0020  .u.r. .w.e.n.n. 
+00005be0: 0061 0075 0066 0020 0064 0065 0072 0020  .a.u.f. .d.e.r. 
+00005bf0: 0051 0053 004c 002d 0053 0065 0069 0074  .Q.S.L.-.S.e.i.t
+00005c00: 0065 0020 0061 0075 0073 0067 0065 0077  .e. .a.u.s.g.e.w
+00005c10: 00e4 0068 006c 0074 0800 0000 0006 0000  ...h.l.t........
+00005c20: 0024 5570 6c6f 6164 7320 6f6e 6c79 2069  .$Uploads only i
+00005c30: 6620 7365 6c65 6374 6564 206f 6e20 5153  f selected on QS
+00005c40: 4c20 7061 6765 0700 0000 0751 534f 466f  L page.....QSOFo
+00005c50: 726d 0103 0000 0048 0044 0065 0072 0020  rm.....H.D.e.r. 
+00005c60: 004e 0075 0074 007a 0065 0072 0020 0043  .N.u.t.z.e.r. .C
+00005c70: 0061 006c 006c 0020 0073 0074 0069 006d  .a.l.l. .s.t.i.m
+00005c80: 006d 0074 0020 006e 0069 0063 0068 0074  .m.t. .n.i.c.h.t
+00005c90: 0020 00fc 0062 0065 0072 0065 0069 006e  . ...b.e.r.e.i.n
+00005ca0: 0800 0000 0006 0000 0018 5573 6572 2063  ..........User c
+00005cb0: 616c 6c20 646f 6573 206e 6f74 206d 6174  all does not mat
+00005cc0: 6368 0700 0000 0751 534f 466f 726d 0103  ch.....QSOForm..
+00005cd0: ffff ffff 0800 0000 0006 0000 0004 6551  ..............eQ
+00005ce0: 534c 0700 0000 0751 534f 466f 726d 0103  SL.....QSOForm..
+00005cf0: 0000 001c 0065 0051 0053 004c 0020 0065  .....e.Q.S.L. .e
+00005d00: 006d 0070 0066 0061 006e 0067 0065 006e  .m.p.f.a.n.g.e.n
+00005d10: 0800 0000 0006 0000 000d 6551 534c 2072  ..........eQSL r
+00005d20: 6563 6569 7665 6407 0000 0007 5153 4f46  eceived.....QSOF
+00005d30: 6f72 6d01 0300 0000 1a00 6500 5100 5300  orm.......e.Q.S.
+00005d40: 4c00 2000 6700 6500 7300 6500 6e00 6400  L. .g.e.s.e.n.d.
+00005d50: 6500 7408 0000 0000 0600 0000 0965 5153  e.t..........eQS
+00005d60: 4c20 7365 6e74 0700 0000 0751 534f 466f  L sent.....QSOFo
+00005d70: 726d 0103 0000 0008 006b 002e 0041 002e  rm.......k...A..
+00005d80: 0800 0000 0006 0000 0004 6e2e 612e 0700  ..........n.a...
+00005d90: 0000 0751 534f 466f 726d 0103 0000 0034  ...QSOForm.....4
+00005da0: 0072 0069 0067 0063 0074 006c 0064 0020  .r.i.g.c.t.l.d. 
+00005db0: 005a 0065 0069 0074 00fc 0062 0065 0072  .Z.e.i.t...b.e.r
+00005dc0: 0073 0063 0068 0072 0065 0069 0074 0075  .s.c.h.r.e.i.t.u
+00005dd0: 006e 0067 0800 0000 0006 0000 000f 7269  .n.g..........ri
+00005de0: 6763 746c 6420 7469 6d65 6f75 7407 0000  gctld timeout...
+00005df0: 0007 5153 4f46 6f72 6d01 03ff ffff ff08  ..QSOForm.......
+00005e00: 0000 0000 0600 0000 0a79 7979 792d 4d4d  .........yyyy-MM
+00005e10: 2d64 6407 0000 0007 5153 4f46 6f72 6d01  -dd.....QSOForm.
+00005e20: 0300 0000 1000 4100 6e00 7400 6500 6e00  ......A.n.t.e.n.
+00005e30: 6e00 6500 6e08 0000 0000 0600 0000 0841  n.e.n..........A
+00005e40: 6e74 656e 6e61 7307 0000 0008 5365 7474  ntennas.....Sett
+00005e50: 696e 6773 0103 0000 007a 0043 0041 0054  ings.....z.C.A.T
+00005e60: 002d 0045 0069 006e 0073 0074 0065 006c  .-.E.i.n.s.t.e.l
+00005e70: 006c 0075 006e 0067 0020 0077 0075 0072  .l.u.n.g. .w.u.r
+00005e80: 0064 0020 006e 006f 0063 0068 0020 006e  .d. .n.o.c.h. .n
+00005e90: 0069 0065 0020 0067 0065 0073 0070 0065  .i.e. .g.e.s.p.e
+00005ea0: 0069 0063 0068 0065 0072 0074 0020 006f  .i.c.h.e.r.t. .o
+00005eb0: 0072 0020 0050 0061 0072 0061 006d 0065  .r. .P.a.r.a.m.e
+00005ec0: 0074 0065 0072 0020 0066 0065 0068 006c  .t.e.r. .f.e.h.l
+00005ed0: 0065 006e 0800 0000 0006 0000 003b 4341  .e.n.........;CA
+00005ee0: 5420 636f 6e66 6967 7572 6174 696f 6e20  T configuration 
+00005ef0: 7761 7320 6e65 7665 7220 7361 7665 6420  was never saved 
+00005f00: 6f72 2061 2070 6172 616d 6574 6572 2069  or a parameter i
+00005f10: 7320 6d69 7373 696e 6707 0000 0008 5365  s missing.....Se
+00005f20: 7474 696e 6773 0103 0000 0030 0043 0041  ttings.....0.C.A
+00005f30: 0054 002d 0045 0069 006e 0073 0074 0065  .T.-.E.i.n.s.t.e
+00005f40: 006c 006c 0075 006e 0067 0065 006e 0020  .l.l.u.n.g.e.n. 
+00005f50: 0046 0065 0068 006c 0065 0072 0800 0000  .F.e.h.l.e.r....
+00005f60: 0006 0000 0012 4341 5420 7365 7474 696e  ......CAT settin
+00005f70: 6773 2065 7272 6f72 0700 0000 0853 6574  gs error.....Set
+00005f80: 7469 6e67 7301 0300 0000 2a00 4800 6100  tings.....*.H.a.
+00005f90: 6d00 6c00 6900 6200 2000 7200 6900 6700  m.l.i.b. .r.i.g.
+00005fa0: 6300 7400 6c00 6400 2000 7700 e400 6800  c.t.l.d. .w...h.
+00005fb0: 6c00 6500 6e08 0000 0000 0600 0000 2043  l.e.n......... C
+00005fc0: 686f 6f73 6520 6861 6d6c 6962 2072 6967  hoose hamlib rig
+00005fd0: 6374 6c64 2065 7865 6375 7461 626c 6507  ctld executable.
+00005fe0: 0000 0008 5365 7474 696e 6773 0103 0000  ....Settings....
+00005ff0: 0020 0044 0061 0074 0075 006d 002f 005a  . .D.a.t.u.m./.Z
+00006000: 0065 0069 0074 0020 0053 0074 0061 0072  .e.i.t. .S.t.a.r
+00006010: 0074 0800 0000 0006 0000 000f 4461 7465  .t..........Date
+00006020: 2f54 696d 6520 7374 6172 7407 0000 0008  /Time start.....
+00006030: 5365 7474 696e 6773 0103 0000 0042 0046  Settings.....B.F
+00006040: 0065 0068 006c 0065 0072 0020 0062 0065  .e.h.l.e.r. .b.e
+00006050: 0069 006d 0020 0041 0075 0073 0066 00fc  .i.m. .A.u.s.f..
+00006060: 0068 0072 0065 006e 0020 0076 006f 006e  .h.r.e.n. .v.o.n
+00006070: 0020 0072 0069 0067 0063 0074 006c 0064  . .r.i.g.c.t.l.d
+00006080: 0800 0000 0006 0000 0017 4572 726f 7220  ..........Error 
+00006090: 6578 6563 7574 696e 6720 7269 6763 746c  executing rigctl
+000060a0: 6407 0000 0008 5365 7474 696e 6773 0103  d.....Settings..
+000060b0: ffff ffff 0800 0000 0006 0000 0006 4861  ..............Ha
+000060c0: 6d6c 6962 0700 0000 0853 6574 7469 6e67  mlib.....Setting
+000060d0: 7301 0300 0000 1600 5100 5400 4800 2000  s.......Q.T.H. .
+000060e0: 4c00 4f00 6300 6100 6f00 7400 7208 0000  L.O.c.a.o.t.r...
+000060f0: 0000 0600 0000 0f51 5448 7320 2620 6c6f  .......QTHs & lo
+00006100: 6361 746f 7273 0700 0000 0853 6574 7469  cators.....Setti
+00006110: 6e67 7301 0300 0000 1400 4600 7500 6e00  ngs.......F.u.n.
+00006120: 6b00 6700 6500 7200 e400 7400 6508 0000  k.g.e.r...t.e...
+00006130: 0000 0600 0000 0652 6164 696f 7307 0000  .......Radios...
+00006140: 0008 5365 7474 696e 6773 0103 0000 004e  ..Settings.....N
+00006150: 0044 0069 0065 0020 0067 0065 0077 00e4  .D.i.e. .g.e.w..
+00006160: 0068 006c 0074 0065 0020 0044 0061 0074  .h.l.t.e. .D.a.t
+00006170: 0065 0069 0020 0069 0073 0074 0020 006e  .e.i. .i.s.t. .n
+00006180: 0069 0063 0068 0074 0020 0061 0075 0073  .i.c.h.t. .a.u.s
+00006190: 0066 00fc 0068 0072 0062 0061 0072 0800  .f...h.r.b.a.r..
+000061a0: 0000 0006 0000 0023 5365 6c65 6374 6564  .......#Selected
+000061b0: 2066 696c 6520 6973 206e 6f74 2074 6865   file is not the
+000061c0: 2065 7865 6375 7461 626c 6507 0000 0008   executable.....
+000061d0: 5365 7474 696e 6773 0103 0000 0014 007a  Settings.......z
+000061e0: 0065 0069 0067 0065 0020 0061 006c 006c  .e.i.g.e. .a.l.l
+000061f0: 0065 0800 0000 0006 0000 0008 5368 6f77  .e..........Show
+00006200: 2061 6c6c 0700 0000 0853 6574 7469 6e67   all.....Setting
+00006210: 7301 03ff ffff ff08 0000 0000 0600 0000  s...............
+00006220: 0553 7461 7274 0700 0000 0853 6574 7469  .Start.....Setti
+00006230: 6e67 7301 0300 0000 1a00 5300 7400 6100  ngs.......S.t.a.
+00006240: 7200 7400 6500 2000 4800 6100 6d00 6c00  r.t.e. .H.a.m.l.
+00006250: 6900 6208 0000 0000 0600 0000 0c53 7461  i.b..........Sta
+00006260: 7274 2068 616d 6c69 6207 0000 0008 5365  rt hamlib.....Se
+00006270: 7474 696e 6773 0103 ffff ffff 0800 0000  ttings..........
+00006280: 0006 0000 0004 5374 6f70 0700 0000 0853  ......Stop.....S
+00006290: 6574 7469 6e67 7301 0300 0000 1a00 5300  ettings.......S.
+000062a0: 7400 6f00 7000 7000 6500 2000 4800 6100  t.o.p.p.e. .H.a.
+000062b0: 6d00 6c00 6900 6208 0000 0000 0600 0000  m.l.i.b.........
+000062c0: 0b53 746f 7020 6861 6d6c 6962 0700 0000  .Stop hamlib....
+000062d0: 0853 6574 7469 6e67 7301 0300 0000 6a00  .Settings.....j.
+000062e0: 4500 6900 6e00 6700 6100 6200 6500 2000  E.i.n.g.a.b.e. .
+000062f0: 6100 6c00 7300 3a00 2000 2200 4f00 7200  a.l.s.:. .".O.r.
+00006300: 7400 2000 2800 4c00 6f00 6300 6100 7400  t. .(.L.o.c.a.t.
+00006310: 6f00 7200 2900 2200 2c00 2000 7a00 2e00  o.r.).".,. .z...
+00006320: 4200 2e00 2000 2200 4b00 6f00 6200 6c00  B... .".K.o.b.l.
+00006330: 6500 6e00 7a00 2000 2800 4a00 4f00 3300  e.n.z. .(.J.O.3.
+00006340: 3000 7400 6900 2900 2208 0000 0000 0600  0.t.i.).".......
+00006350: 0000 3554 7970 6520 696e 2061 733a 2022  ..5Type in as: "
+00006360: 4369 7479 2028 4c6f 6361 746f 7229 222c  City (Locator)",
+00006370: 2069 2e65 2e20 224b 6f62 6c65 6e7a 2028   i.e. "Koblenz (
+00006380: 4a4f 3330 7469 2922 0700 0000 0853 6574  JO30ti)".....Set
+00006390: 7469 6e67 7301 0300 0000 0a00 6100 6b00  tings.......a.k.
+000063a0: 7400 6900 7608 0000 0000 0600 0000 0561  t.i.v..........a
+000063b0: 6374 6976 0700 0000 0853 6574 7469 6e67  ctiv.....Setting
+000063c0: 7301 0300 0000 0e00 6900 6e00 6100 6b00  s.......i.n.a.k.
+000063d0: 7400 6900 7608 0000 0000 0600 0000 0769  t.i.v..........i
+000063e0: 6e61 6374 6976 0700 0000 0853 6574 7469  nactiv.....Setti
+000063f0: 6e67 7301 0300 0000 4a00 7200 6900 6700  ngs.....J.r.i.g.
+00006400: 6300 7400 6c00 6400 2000 6b00 6f00 6e00  c.t.l.d. .k.o.n.
+00006410: 6e00 7400 6500 2000 6e00 6900 6300 6800  n.t.e. .n.i.c.h.
+00006420: 7400 2000 6700 6500 7300 7400 6100 7200  t. .g.e.s.t.a.r.
+00006430: 7400 6500 7400 2000 7700 6500 7200 6400  t.e.t. .w.e.r.d.
+00006440: 6500 6e08 0000 0000 0600 0000 1e72 6967  e.n..........rig
+00006450: 6374 6c64 2064 6964 206e 6f74 2073 7461  ctld did not sta
+00006460: 7274 2070 726f 7065 726c 7907 0000 0008  rt properly.....
+00006470: 5365 7474 696e 6773 0103 0000 0036 0072  Settings.....6.r
+00006480: 0069 0067 0063 0074 006c 0064 0020 0069  .i.g.c.t.l.d. .i
+00006490: 0073 0074 0020 006e 0069 0063 0068 0074  .s.t. .n.i.c.h.t
+000064a0: 0020 0076 0065 0072 0066 00fc 0067 0062  . .v.e.r.f...g.b
+000064b0: 0061 0072 0800 0000 0006 0000 0018 7269  .a.r..........ri
+000064c0: 6763 746c 6420 6973 206e 6f74 2061 7661  gctld is not ava
+000064d0: 696c 6162 6c65 0700 0000 0853 6574 7469  ilable.....Setti
+000064e0: 6e67 7301 0300 0000 1000 6700 6500 e400  ngs.......g.e...
+000064f0: 6e00 6400 6500 7200 7408 0000 0000 0600  n.d.e.r.t.......
+00006500: 0000 014d 0700 0000 1454 7261 6e73 6c61  ...M.....Transla
+00006510: 7465 6454 6162 6c65 4d6f 6465 6c01 0300  tedTableModel...
+00006520: 0000 0800 4e00 6500 6900 6e08 0000 0000  ....N.e.i.n.....
+00006530: 0600 0000 014e 0700 0000 1454 7261 6e73  .....N.....Trans
+00006540: 6c61 7465 6454 6162 6c65 4d6f 6465 6c01  latedTableModel.
+00006550: 0300 0000 1200 6100 6e00 6700 6500 6600  ......a.n.g.e.f.
+00006560: 7200 6100 6700 7408 0000 0000 0600 0000  r.a.g.t.........
+00006570: 0152 0700 0000 1454 7261 6e73 6c61 7465  .R.....Translate
+00006580: 6454 6162 6c65 4d6f 6465 6c01 0300 0000  dTableModel.....
+00006590: 0400 4a00 6108 0000 0000 0600 0000 0159  ..J.a..........Y
+000065a0: 0700 0000 1454 7261 6e73 6c61 7465 6454  .....TranslatedT
+000065b0: 6162 6c65 4d6f 6465 6c01 03ff ffff ff08  ableModel.......
+000065c0: 0000 0000 0600 0000 074a 5338 4361 6c6c  .........JS8Call
+000065d0: 0700 0000 0f61 7070 5365 6c65 6374 4469  .....appSelectDi
+000065e0: 616c 6f67 0103 ffff ffff 0800 0000 0006  alog............
+000065f0: 0000 0005 4f74 6865 7207 0000 000f 6170  ....Other.....ap
+00006600: 7053 656c 6563 7444 6961 6c6f 6701 0300  pSelectDialog...
+00006610: 0000 2a00 4100 7500 7300 7700 6100 6800  ..*.A.u.s.w.a.h.
+00006620: 6c00 2000 6400 6500 7300 2000 5000 7200  l. .d.e.s. .P.r.
+00006630: 6f00 6700 7200 6100 6d00 6d00 7308 0000  o.g.r.a.m.m.s...
+00006640: 0000 0600 0000 1653 656c 6563 7420 7468  .......Select th
+00006650: 6520 6170 706c 6963 6174 696f 6e07 0000  e application...
+00006660: 000f 6170 7053 656c 6563 7444 6961 6c6f  ..appSelectDialo
+00006670: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
+00006680: 0657 534a 542d 5807 0000 000f 6170 7053  .WSJT-X.....appS
+00006690: 656c 6563 7444 6961 6c6f 6701 03ff ffff  electDialog.....
+000066a0: ff08 0000 0000 0600 0000 0666 6c64 6967  ...........fldig
+000066b0: 6907 0000 000f 6170 7053 656c 6563 7444  i.....appSelectD
+000066c0: 6961 6c6f 6701 8800 0000 0201 01         ialog........
```

### Comparing `dragonlog-1.2.1/dragonlog/data/modes.json` & `dragonlog-1.3/dragonlog/data/modes.json`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/eQSL.py` & `dragonlog-1.3/dragonlog/eQSL.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/Screenshot.png` & `dragonlog-1.3/dragonlog/icons/Screenshot.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/db.png` & `dragonlog-1.3/dragonlog/icons/db.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/edit.png` & `dragonlog-1.3/dragonlog/icons/edit.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/edit_add.png` & `dragonlog-1.3/dragonlog/icons/edit_add.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/edit_addmulti.png` & `dragonlog-1.3/dragonlog/icons/edit_addmulti.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/edit_addmulti.xcf` & `dragonlog-1.3/dragonlog/icons/edit_addmulti.xcf`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/edit_remove.png` & `dragonlog-1.3/dragonlog/icons/edit_remove.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/exit.png` & `dragonlog-1.3/dragonlog/icons/exit.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/file_doc.png` & `dragonlog-1.3/dragonlog/icons/file_doc.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/fileexport.png` & `dragonlog-1.3/dragonlog/icons/fileexport.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/fileimport.png` & `dragonlog-1.3/dragonlog/icons/fileimport.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/filter.png` & `dragonlog-1.3/dragonlog/icons/filter.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/gear.png` & `dragonlog-1.3/dragonlog/icons/gear.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/help.png` & `dragonlog-1.3/dragonlog/icons/help.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/icons8-dragon-96.png` & `dragonlog-1.3/dragonlog/icons/icons8-dragon-96.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/icons8-dragon-96.xcf` & `dragonlog-1.3/dragonlog/icons/icons8-dragon-96.xcf`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/info.png` & `dragonlog-1.3/dragonlog/icons/info.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/logo.ico` & `dragonlog-1.3/dragonlog/icons/logo.ico`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/no.png` & `dragonlog-1.3/dragonlog/icons/no.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/ok.png` & `dragonlog-1.3/dragonlog/icons/ok.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/player_play.png` & `dragonlog-1.3/dragonlog/icons/player_play.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/player_stop.png` & `dragonlog-1.3/dragonlog/icons/player_stop.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/upload_lotw.png` & `dragonlog-1.3/dragonlog/icons/upload_lotw.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/upload_lotw.xcf` & `dragonlog-1.3/dragonlog/icons/upload_lotw.xcf`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/dragonlog/icons/watch.png` & `dragonlog-1.3/dragonlog/icons/watch.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/pyproject.toml` & `dragonlog-1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dragonlog-1.2.1/setup_msi.py` & `dragonlog-1.3/setup_msi.py`

 * *Files identical despite different names*

