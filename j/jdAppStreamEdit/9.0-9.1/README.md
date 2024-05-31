# Comparing `tmp/jdAppStreamEdit-9.0.tar.gz` & `tmp/jdappstreamedit-9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdAppStreamEdit-9.0.tar", last modified: Thu Feb 29 18:55:48 2024, max compression
+gzip compressed data, was "jdappstreamedit-9.1.tar", last modified: Fri May 31 14:10:07 2024, max compression
```

## Comparing `jdAppStreamEdit-9.0.tar` & `jdappstreamedit-9.1.tar`

### file list

```diff
@@ -1,88 +1,89 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 18:55:48.202986 jdAppStreamEdit-9.0/
--rw-r--r--   0 root         (0) root         (0)     2929 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/BuildBackend.py
--rw-r--r--   0 root         (0) root         (0)    35089 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      198 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6574 2024-02-29 18:55:48.202986 jdAppStreamEdit-9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4703 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 18:55:48.198986 jdAppStreamEdit-9.0/jdAppStreamEdit/
--rw-r--r--   0 root         (0) root         (0)     1827 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/AboutWindow.py
--rw-r--r--   0 root         (0) root         (0)    12941 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/AdvancedWidget.py
--rw-r--r--   0 root         (0) root         (0)     7460 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ArtifactWindow.py
--rw-r--r--   0 root         (0) root         (0)     2309 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ChangelogImporter.py
--rw-r--r--   0 root         (0) root         (0)     2828 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ComposeDirectoryWindow.py
--rw-r--r--   0 root         (0) root         (0)      171 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/Constants.py
--rw-r--r--   0 root         (0) root         (0)    11968 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/DescriptionWidget.py
--rw-r--r--   0 root         (0) root         (0)     5271 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/Environment.py
--rw-r--r--   0 root         (0) root         (0)    14628 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ExternalReleasesWindow.py
--rw-r--r--   0 root         (0) root         (0)     6287 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/Functions.py
--rw-r--r--   0 root         (0) root         (0)    18836 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/Icon.svg
--rw-r--r--   0 root         (0) root         (0)     2444 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ImportChangelogWindow.py
--rw-r--r--   0 root         (0) root         (0)      596 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/Interfaces.py
--rw-r--r--   0 root         (0) root         (0)      299 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/Languages.py
--rw-r--r--   0 root         (0) root         (0)    56610 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/MainWindow.py
--rw-r--r--   0 root         (0) root         (0)     4707 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ManageTemplatesWindow.py
--rw-r--r--   0 root         (0) root         (0)    13512 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/OarsWidget.py
--rw-r--r--   0 root         (0) root         (0)      538 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/PluginAPI.py
--rw-r--r--   0 root         (0) root         (0)     3885 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/PluginLoader.py
--rw-r--r--   0 root         (0) root         (0)     2983 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/PluginWindow.py
--rw-r--r--   0 root         (0) root         (0)    11020 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/RelationsWidget.py
--rw-r--r--   0 root         (0) root         (0)    10125 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ReleaseImporter.py
--rw-r--r--   0 root         (0) root         (0)    11927 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ReleasesWidget.py
--rw-r--r--   0 root         (0) root         (0)     6151 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ReleasesWindow.py
--rw-r--r--   0 root         (0) root         (0)    17383 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ScreenshotWindow.py
--rw-r--r--   0 root         (0) root         (0)     1914 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/Settings.py
--rw-r--r--   0 root         (0) root         (0)     5636 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/SettingsWindow.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/SysinfoWindow.py
--rw-r--r--   0 root         (0) root         (0)     9601 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ThumbnailWindow.py
--rw-r--r--   0 root         (0) root         (0)     5500 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/TranslateWindow.py
--rw-r--r--   0 root         (0) root         (0)     1077 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/Types.py
--rw-r--r--   0 root         (0) root         (0)     2563 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ValidateWindow.py
--rw-r--r--   0 root         (0) root         (0)     3742 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ViewCatalogWindow.py
--rw-r--r--   0 root         (0) root         (0)     1082 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ViewXMLWindow.py
--rw-r--r--   0 root         (0) root         (0)     1642 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/XMLHighlighter.py
--rw-r--r--   0 root         (0) root         (0)     3574 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/__init__.py
--rw-r--r--   0 root         (0) root         (0)       48 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 18:55:48.198986 jdAppStreamEdit-9.0/jdAppStreamEdit/data/
--rw-r--r--   0 root         (0) root         (0)     1405 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/data/categories.txt
--rw-r--r--   0 root         (0) root         (0)     2237 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/data/changelog.html
--rw-r--r--   0 root         (0) root         (0)     2446 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/data/language_codes.csv
--rw-r--r--   0 root         (0) root         (0)      740 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/data/metadata_licenses.json
--rw-r--r--   0 root         (0) root         (0)      806 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/data/platform.json
--rw-r--r--   0 root         (0) root         (0)   276811 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/data/project_licenses.json
--rw-r--r--   0 root         (0) root         (0)       39 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/data/translators.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 18:55:48.198986 jdAppStreamEdit-9.0/jdAppStreamEdit/translations/
--rw-r--r--   0 root         (0) root         (0)   161896 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/translations/jdAppStreamEdit_de.ts
--rw-r--r--   0 root         (0) root         (0)   159866 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/translations/jdAppStreamEdit_nl.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 18:55:48.202986 jdAppStreamEdit-9.0/jdAppStreamEdit/ui/
--rw-r--r--   0 root         (0) root         (0)     4012 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ui/AboutWindow.ui
--rw-r--r--   0 root         (0) root         (0)     8438 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ui/AdvancedWidget.ui
--rw-r--r--   0 root         (0) root         (0)     6432 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ui/ArtifactWindow.ui
--rw-r--r--   0 root         (0) root         (0)     3311 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ui/ComposeDirectoryWindow.ui
--rw-r--r--   0 root         (0) root         (0)     2357 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ui/DescriptionWidget.ui
--rw-r--r--   0 root         (0) root         (0)     4757 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ui/ExternalReleasesWindow.ui
--rw-r--r--   0 root         (0) root         (0)     2311 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ui/ImportChangelogWindow.ui
--rw-r--r--   0 root         (0) root         (0)    37654 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ui/MainWindow.ui
--rw-r--r--   0 root         (0) root         (0)     1358 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ui/ManageTemplatesWindow.ui
--rw-r--r--   0 root         (0) root         (0)    25574 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ui/OarsWidget.ui
--rw-r--r--   0 root         (0) root         (0)     4273 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ui/PluginWindow.ui
--rw-r--r--   0 root         (0) root         (0)    20235 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ui/RelationsWidget.ui
--rw-r--r--   0 root         (0) root         (0)     1792 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ui/ReleasesWidget.ui
--rw-r--r--   0 root         (0) root         (0)     4400 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ui/ReleasesWindow.ui
--rw-r--r--   0 root         (0) root         (0)    13384 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ui/ScreenshotWindow.ui
--rw-r--r--   0 root         (0) root         (0)     6157 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ui/SettingsWindow.ui
--rw-r--r--   0 root         (0) root         (0)     1766 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ui/SysinfoWindow.ui
--rw-r--r--   0 root         (0) root         (0)     9624 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ui/ThumbnailWindow.ui
--rw-r--r--   0 root         (0) root         (0)     1895 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ui/TranslateWindow.ui
--rw-r--r--   0 root         (0) root         (0)     2061 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ui/ValidateWindow.ui
--rw-r--r--   0 root         (0) root         (0)     2904 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ui/ViewCatalogWindow.ui
--rw-r--r--   0 root         (0) root         (0)     1983 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/ui/ViewXMLWindow.ui
--rw-r--r--   0 root         (0) root         (0)        4 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/jdAppStreamEdit/version.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 18:55:48.202986 jdAppStreamEdit-9.0/jdAppStreamEdit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6574 2024-02-29 18:55:48.000000 jdAppStreamEdit-9.0/jdAppStreamEdit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2761 2024-02-29 18:55:48.000000 jdAppStreamEdit-9.0/jdAppStreamEdit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-29 18:55:48.000000 jdAppStreamEdit-9.0/jdAppStreamEdit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      140 2024-02-29 18:55:48.000000 jdAppStreamEdit-9.0/jdAppStreamEdit.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      122 2024-02-29 18:55:48.000000 jdAppStreamEdit-9.0/jdAppStreamEdit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-02-29 18:55:48.000000 jdAppStreamEdit-9.0/jdAppStreamEdit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2641 2024-02-29 18:54:59.000000 jdAppStreamEdit-9.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-29 18:55:48.202986 jdAppStreamEdit-9.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 14:10:07.001497 jdappstreamedit-9.1/
+-rw-r--r--   0 root         (0) root         (0)     2929 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/BuildBackend.py
+-rw-r--r--   0 root         (0) root         (0)    35089 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      198 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6574 2024-05-31 14:10:07.001497 jdappstreamedit-9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4703 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 14:10:06.993497 jdappstreamedit-9.1/jdAppStreamEdit/
+-rw-r--r--   0 root         (0) root         (0)     1827 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/AboutWindow.py
+-rw-r--r--   0 root         (0) root         (0)    16279 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/AdvancedWidget.py
+-rw-r--r--   0 root         (0) root         (0)     7460 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ArtifactWindow.py
+-rw-r--r--   0 root         (0) root         (0)     2309 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ChangelogImporter.py
+-rw-r--r--   0 root         (0) root         (0)     2828 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ComposeDirectoryWindow.py
+-rw-r--r--   0 root         (0) root         (0)      171 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/Constants.py
+-rw-r--r--   0 root         (0) root         (0)    11968 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/DescriptionWidget.py
+-rw-r--r--   0 root         (0) root         (0)     5271 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/Environment.py
+-rw-r--r--   0 root         (0) root         (0)    14628 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ExternalReleasesWindow.py
+-rw-r--r--   0 root         (0) root         (0)     6287 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/Functions.py
+-rw-r--r--   0 root         (0) root         (0)    18836 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/Icon.svg
+-rw-r--r--   0 root         (0) root         (0)     2444 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ImportChangelogWindow.py
+-rw-r--r--   0 root         (0) root         (0)      596 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/Interfaces.py
+-rw-r--r--   0 root         (0) root         (0)      364 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/Languages.py
+-rw-r--r--   0 root         (0) root         (0)    56666 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/MainWindow.py
+-rw-r--r--   0 root         (0) root         (0)     4707 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ManageTemplatesWindow.py
+-rw-r--r--   0 root         (0) root         (0)    13512 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/OarsWidget.py
+-rw-r--r--   0 root         (0) root         (0)      538 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/PluginAPI.py
+-rw-r--r--   0 root         (0) root         (0)     3885 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/PluginLoader.py
+-rw-r--r--   0 root         (0) root         (0)     2983 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/PluginWindow.py
+-rw-r--r--   0 root         (0) root         (0)    11020 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/RelationsWidget.py
+-rw-r--r--   0 root         (0) root         (0)    10125 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ReleaseImporter.py
+-rw-r--r--   0 root         (0) root         (0)    11927 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ReleasesWidget.py
+-rw-r--r--   0 root         (0) root         (0)     6151 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ReleasesWindow.py
+-rw-r--r--   0 root         (0) root         (0)    17383 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ScreenshotWindow.py
+-rw-r--r--   0 root         (0) root         (0)     1914 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/Settings.py
+-rw-r--r--   0 root         (0) root         (0)     5636 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/SettingsWindow.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/SysinfoWindow.py
+-rw-r--r--   0 root         (0) root         (0)     9601 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ThumbnailWindow.py
+-rw-r--r--   0 root         (0) root         (0)     5500 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/TranslateWindow.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/Types.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ValidateWindow.py
+-rw-r--r--   0 root         (0) root         (0)     3742 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ViewCatalogWindow.py
+-rw-r--r--   0 root         (0) root         (0)     1082 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ViewXMLWindow.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/XMLHighlighter.py
+-rw-r--r--   0 root         (0) root         (0)     3574 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 14:10:06.993497 jdappstreamedit-9.1/jdAppStreamEdit/data/
+-rw-r--r--   0 root         (0) root         (0)     1405 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/data/categories.txt
+-rw-r--r--   0 root         (0) root         (0)     2339 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/data/changelog.html
+-rw-r--r--   0 root         (0) root         (0)     2446 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/data/language_codes.csv
+-rw-r--r--   0 root         (0) root         (0)      740 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/data/metadata_licenses.json
+-rw-r--r--   0 root         (0) root         (0)      806 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/data/platform.json
+-rw-r--r--   0 root         (0) root         (0)   276811 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/data/project_licenses.json
+-rw-r--r--   0 root         (0) root         (0)       72 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/data/translators.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 14:10:06.997497 jdappstreamedit-9.1/jdAppStreamEdit/translations/
+-rw-r--r--   0 root         (0) root         (0)   162841 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/translations/jdAppStreamEdit_de.ts
+-rw-r--r--   0 root         (0) root         (0)   160819 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/translations/jdAppStreamEdit_nl.ts
+-rw-r--r--   0 root         (0) root         (0)   145898 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/translations/jdAppStreamEdit_ru.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 14:10:07.001497 jdappstreamedit-9.1/jdAppStreamEdit/ui/
+-rw-r--r--   0 root         (0) root         (0)     4012 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ui/AboutWindow.ui
+-rw-r--r--   0 root         (0) root         (0)    10329 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ui/AdvancedWidget.ui
+-rw-r--r--   0 root         (0) root         (0)     6432 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ui/ArtifactWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     3311 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ui/ComposeDirectoryWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     2357 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ui/DescriptionWidget.ui
+-rw-r--r--   0 root         (0) root         (0)     4757 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ui/ExternalReleasesWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     2311 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ui/ImportChangelogWindow.ui
+-rw-r--r--   0 root         (0) root         (0)    38714 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ui/MainWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     1358 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ui/ManageTemplatesWindow.ui
+-rw-r--r--   0 root         (0) root         (0)    25574 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ui/OarsWidget.ui
+-rw-r--r--   0 root         (0) root         (0)     4273 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ui/PluginWindow.ui
+-rw-r--r--   0 root         (0) root         (0)    20235 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ui/RelationsWidget.ui
+-rw-r--r--   0 root         (0) root         (0)     1792 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ui/ReleasesWidget.ui
+-rw-r--r--   0 root         (0) root         (0)     4400 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ui/ReleasesWindow.ui
+-rw-r--r--   0 root         (0) root         (0)    13384 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ui/ScreenshotWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     7171 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ui/SettingsWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ui/SysinfoWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     9624 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ui/ThumbnailWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     1895 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ui/TranslateWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     2061 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ui/ValidateWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     2904 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ui/ViewCatalogWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     1983 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/ui/ViewXMLWindow.ui
+-rw-r--r--   0 root         (0) root         (0)        4 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/jdAppStreamEdit/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 14:10:07.001497 jdappstreamedit-9.1/jdAppStreamEdit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6574 2024-05-31 14:10:06.000000 jdappstreamedit-9.1/jdAppStreamEdit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2812 2024-05-31 14:10:06.000000 jdappstreamedit-9.1/jdAppStreamEdit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 14:10:06.000000 jdappstreamedit-9.1/jdAppStreamEdit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      140 2024-05-31 14:10:06.000000 jdappstreamedit-9.1/jdAppStreamEdit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      122 2024-05-31 14:10:06.000000 jdappstreamedit-9.1/jdAppStreamEdit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-31 14:10:06.000000 jdappstreamedit-9.1/jdAppStreamEdit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2641 2024-05-31 14:08:02.000000 jdappstreamedit-9.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 14:10:07.001497 jdappstreamedit-9.1/setup.cfg
```

### Comparing `jdAppStreamEdit-9.0/BuildBackend.py` & `jdappstreamedit-9.1/BuildBackend.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/LICENSE` & `jdappstreamedit-9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/PKG-INFO` & `jdappstreamedit-9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdAppStreamEdit
-Version: 9.0
+Version: 9.1
 Summary: A graphical Program to create and edit AppStream files
 Author-email: JakobDev <jakobdev@gmx.de>
 License: GPL-3
 Project-URL: Source, https://codeberg.org/JakobDev/jdAppStreamEdit
 Project-URL: Issues, https://codeberg.org/JakobDev/jdAppStreamEdit/issues
 Project-URL: Translate, https://translate.codeberg.org/projects/jdAppStreamEdit
 Project-URL: Donation, https://ko-fi.com/jakobdev
```

### Comparing `jdAppStreamEdit-9.0/README.md` & `jdappstreamedit-9.1/README.md`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/AboutWindow.py` & `jdappstreamedit-9.1/jdAppStreamEdit/AboutWindow.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/AdvancedWidget.py` & `jdappstreamedit-9.1/jdAppStreamEdit/RelationsWidget.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,284 +1,224 @@
-from .Functions import stretch_table_widget_colums_size, select_combo_box_data, get_logical_table_row_list, clear_table_widget, list_widget_contains_item, get_sender_table_row
-from PyQt6.QtWidgets import QWidget, QComboBox, QTableWidgetItem, QInputDialog, QMessageBox, QPushButton
-from .ui_compiled.AdvancedWidget import Ui_AdvancedWidget
-from typing import Optional, TYPE_CHECKING
+from PyQt6.QtWidgets import QWidget, QComboBox, QLineEdit, QTableWidget, QTableWidgetItem, QPushButton, QHeaderView
+from .Functions import select_combo_box_data, is_string_number, get_logical_table_row_list, clear_table_widget
+from .ui_compiled.RelationsWidget import Ui_RelationsWidget
+from typing import Optional, List, TYPE_CHECKING
 from PyQt6.QtCore import QCoreApplication
+from PyQt6.QtGui import QIntValidator
 from lxml import etree
+import sys
 
 
 if TYPE_CHECKING:
     from .MainWindow import MainWindow
 
 
-class AdvancedWidget(QWidget, Ui_AdvancedWidget):
+class RelationsWidget(QWidget, Ui_RelationsWidget):
     def __init__(self, main_window: "MainWindow") -> None:
         super().__init__()
 
         self.setupUi(self)
 
         self._main_window = main_window
 
-        stretch_table_widget_colums_size(self.translation_table)
-        stretch_table_widget_colums_size(self.tags_table)
-        stretch_table_widget_colums_size(self.custom_table)
-
-        self.translation_table.verticalHeader().setSectionsMovable(True)
-        self.tags_table.verticalHeader().setSectionsMovable(True)
-        self.custom_table.verticalHeader().setSectionsMovable(True)
-
-        self._update_suggests_edit_remove_button()
-        self._update_replaces_edit_remove_button()
-
-        self.translation_table.verticalHeader().sectionMoved.connect(main_window.set_file_edited)
-        self.translation_add_button.clicked.connect(lambda: self._add_translation_row())
-
-        self.suggests_add_button.clicked.connect(self._add_suggests_clicked)
-        self.suggests_edit_button.clicked.connect(self._edit_suggests_clicked)
-        self.suggests_remove_button.clicked.connect(self._remove_suggests_clicked)
-        self.suggests_list.itemSelectionChanged.connect(self._update_suggests_edit_remove_button)
-
-        self.replaces_add_button.clicked.connect(self._add_replaces_clicked)
-        self.replaces_edit_button.clicked.connect(self._edit_replaces_clicked)
-        self.replaces_remove_button.clicked.connect(self._remove_replaces_clicked)
-        self.replaces_list.itemSelectionChanged.connect(self._update_replaces_edit_remove_button)
-
-        self.tags_table.verticalHeader().sectionMoved.connect(main_window.set_file_edited)
-        self.tags_add_button.clicked.connect(lambda: self._add_tags_row())
-
-        self.custom_table.verticalHeader().sectionMoved.connect(main_window.set_file_edited)
-        self.custom_add_button.clicked.connect(lambda: self._add_custom_row())
-
-        self.tab_widget.setCurrentIndex(0)
-
-    # Translation
-
-    def _add_translation_row(self, translation_type: Optional[str] = None, domain: Optional[str] = None) -> None:
-        row = self.translation_table.rowCount()
-        self.translation_table.insertRow(row)
-
-        type_box = QComboBox()
-        type_box.addItem("gettext", "gettext")
-        type_box.addItem("qt", "qt")
-        type_box.currentIndexChanged.connect(self._main_window.set_file_edited)
-        if translation_type is not None:
-            select_combo_box_data(type_box, translation_type)
-        self.translation_table.setCellWidget(row, 0, type_box)
-
-        domain_item = QTableWidgetItem()
-        if domain is not None:
-            domain_item.setText(domain)
-        self.translation_table.setItem(row, 1, domain_item)
-
-        remove_button = QPushButton(QCoreApplication.translate("AdvancedWidget", "Remove"))
-        remove_button.clicked.connect(self._remove_translation_clicked)
-        self.translation_table.setCellWidget(row, 2, remove_button)
-
-        self._main_window.set_file_edited()
-
-    def _remove_translation_clicked(self) -> None:
-        row = get_sender_table_row(self.translation_table, 2, self.sender())
-        self.translation_table.removeRow(row)
-        self._main_window.set_file_edited()
-
-    # Suggests
-
-    def _add_suggests_clicked(self) -> None:
-        text = QInputDialog.getText(self, QCoreApplication.translate("AdvancedWidget", "New Suggestion"), QCoreApplication.translate("AdvancedWidget", "Please enter a new ID"))[0]
-        if text == "":
-            return
-        if list_widget_contains_item(self.suggests_list, text):
-            QMessageBox.critical(self, QCoreApplication.translate("AdvancedWidget", "ID in List"), QCoreApplication.translate("AdvancedWidget", "This ID is already in the List"))
-            return
-        self.suggests_list.addItem(text)
-        self._update_suggests_edit_remove_button()
-        self._main_window.set_file_edited()
-
-    def _edit_suggests_clicked(self) -> None:
-        if self.suggests_list.currentRow() == -1:
-            return
-        old_text = self.suggests_list.currentItem().text()
-        new_text, ok = QInputDialog.getText(self, QCoreApplication.translate("AdvancedWidget", "Edit Suggestion"), QCoreApplication.translate("AdvancedWidget", "Please edit the ID"), text=old_text)
-        if not ok or old_text == new_text:
-            return
-        if list_widget_contains_item(self.suggests_list, new_text):
-            QMessageBox.critical(self, QCoreApplication.translate("AdvancedWidget", "ID in List"), QCoreApplication.translate("AdvancedWidget", "This ID is already in the List"))
-            return
-        self.suggests_list.currentItem().setText(new_text)
-        self._main_window.set_file_edited()
-
-    def _remove_suggests_clicked(self) -> None:
-        index = self.suggests_list.currentRow()
-        if index != -1:
-            self.suggests_list.takeItem(index)
-            self._update_suggests_edit_remove_button()
-            self._main_window.set_file_edited()
-
-    def _update_suggests_edit_remove_button(self) -> None:
-        if self.suggests_list.currentRow() == -1:
-            self.suggests_edit_button.setEnabled(False)
-            self.suggests_remove_button.setEnabled(False)
-        else:
-            self.suggests_edit_button.setEnabled(True)
-            self.suggests_remove_button.setEnabled(True)
-
-    # Replaces
-
-    def _add_replaces_clicked(self) -> None:
-        text = QInputDialog.getText(self, QCoreApplication.translate("AdvancedWidget", "New Replacement"), QCoreApplication.translate("AdvancedWidget", "Please enter a ID"))[0]
-        if text == "":
-            return
-        if list_widget_contains_item(self.replaces_list, text):
-            QMessageBox.critical(self, QCoreApplication.translate("AdvancedWidget", "ID in List"), QCoreApplication.translate("AdvancedWidget", "This ID is already in the List"))
-            return
-        self.replaces_list.addItem(text)
-        self._update_replaces_edit_remove_button()
-        self._main_window.set_file_edited()
-
-    def _edit_replaces_clicked(self) -> None:
-        if self.replaces_list.currentRow() == -1:
-            return
-        old_text = self.replaces_list.currentItem().text()
-        new_text, ok = QInputDialog.getText(self, QCoreApplication.translate("AdvancedWidget", "Edit Replacement"), QCoreApplication.translate("AdvancedWidget", "Please edit the ID"), text=old_text)
-        if not ok or old_text == new_text:
-            return
-        if list_widget_contains_item(self.replaces_list, new_text):
-            QMessageBox.critical(self, QCoreApplication.translate("AdvancedWidget", "ID in List"), QCoreApplication.translate("AdvancedWidget", "This ID is already in the List"))
-            return
-        self.replaces_list.currentItem().setText(new_text)
-        self._main_window.set_file_edited()
-
-    def _remove_replaces_clicked(self) -> None:
-        index = self.replaces_list.currentRow()
-        if index != -1:
-            self.replaces_list.takeItem(index)
-            self._update_replaces_edit_remove_button()
-            self._main_window.set_file_edited()
-
-    def _update_replaces_edit_remove_button(self) -> None:
-        if self.replaces_list.currentRow() == -1:
-            self.replaces_edit_button.setEnabled(False)
-            self.replaces_remove_button.setEnabled(False)
-        else:
-            self.replaces_edit_button.setEnabled(True)
-            self.replaces_remove_button.setEnabled(True)
-
-    # Tags
-
-    def _add_tags_row(self, namespace: Optional[str] = None, value: Optional[str] = None) -> None:
-        row = self.tags_table.rowCount()
-        self.tags_table.insertRow(row)
-
-        namespace_item = QTableWidgetItem()
-        if namespace is not None:
-            namespace_item.setText(namespace)
-        self.tags_table.setItem(row, 0, namespace_item)
-
-        value_item = QTableWidgetItem()
-        if value is not None:
-            value_item.setText(value)
-        self.tags_table.setItem(row, 1, value_item)
-
-        remove_button = QPushButton(QCoreApplication.translate("AdvancedWidget", "Remove"))
-        remove_button.clicked.connect(self._remove_tags_clicked)
-        self.tags_table.setCellWidget(row, 2, remove_button)
-
-        self._main_window.set_file_edited()
-
-    def _remove_tags_clicked(self) -> None:
-        row = get_sender_table_row(self.tags_table, 2, self.sender())
-        self.tags_table.removeRow(row)
-        self._main_window.set_file_edited()
-
-    # Custom
-
-    def _add_custom_row(self, key: Optional[str] = None, value: Optional[str] = None) -> None:
-        row = self.custom_table.rowCount()
-        self.custom_table.insertRow(row)
-
-        key_item = QTableWidgetItem()
-        if key is not None:
-            key_item.setText(key)
-        self.custom_table.setItem(row, 0, key_item)
-
-        value_item = QTableWidgetItem()
-        if value is not None:
-            value_item.setText(value)
-        self.custom_table.setItem(row, 1, value_item)
-
-        remove_button = QPushButton(QCoreApplication.translate("AdvancedWidget", "Remove"))
-        remove_button.clicked.connect(self._remove_custom_clicked)
-        self.custom_table.setCellWidget(row, 2, remove_button)
-
-        self._main_window.set_file_edited()
-
-    def _remove_custom_clicked(self) -> None:
-        row = get_sender_table_row(self.custom_table, 2, self.sender())
-        self.custom_table.removeRow(row)
-        self._main_window.set_file_edited()
-
-    # Other
+        for key, value in vars(self).items():
+            if key.startswith("edit_screen_custom_") or key.startswith("edit_internet_bandwidth_"):
+                value.setValidator(QIntValidator())
+            elif key.startswith("box_internet_"):
+                value.addItem(QCoreApplication.translate("RelationsWidget", "Not specified"), "none")
+                value.addItem(QCoreApplication.translate("RelationsWidget", "Never uses the internet, even if it’s available"), "offline-only")
+                value.addItem(QCoreApplication.translate("RelationsWidget", "Uses the internet only the first time the application is run"), "first-run")
+                value.addItem(QCoreApplication.translate("RelationsWidget", "Needs internet connectivity to work"), "always")
+
+            if isinstance(value, QComboBox):
+                value.currentIndexChanged.connect(main_window.set_file_edited)
+            elif isinstance(value, QLineEdit):
+                value.textEdited.connect(main_window.set_file_edited)
+
+        self.edit_memory_requires.setValidator(QIntValidator())
+        self.edit_memory_recommends.setValidator(QIntValidator())
+
+        self.modalias_table.horizontalHeader().setSectionResizeMode(1, QHeaderView.ResizeMode.Stretch)
+        self.hardware_table.horizontalHeader().setSectionResizeMode(1, QHeaderView.ResizeMode.Stretch)
+
+        self.modalias_table.verticalHeader().setSectionsMovable(True)
+        self.hardware_table.verticalHeader().setSectionsMovable(True)
+
+        self.button_modalias_add.clicked.connect(self._add_modalias_row)
+        self.button_hardware_add.clicked.connect(self._add_hardware_row)
+
+        self._update_internet_bandwith_enabled()
+
+        self.main_tab_widget.setCurrentIndex(0)
+
+    # Screen
+
+    def _load_screen_data(self, tag_list: List[etree.Element], relation: str) -> None:
+        for i in tag_list:
+            size = i.get("compare")
+            if size is None:
+                size = "ge"
+            if size not in ("ge", "le"):
+                print("Unsupported compare attribute " + size, file=sys.stderr)
+                continue
+            append_string = size + "_" + relation
+            if is_string_number(i.text):
+                getattr(self, "edit_screen_custom_" + append_string).setText(i.text)
+            elif i.text == "xsmall":
+                getattr(self, "edit_screen_custom_" + append_string).setText("360")
+            elif i.text == "small":
+                getattr(self, "edit_screen_custom_" + append_string).setText("420")
+            elif i.text == "medium":
+                getattr(self, "edit_screen_custom_" + append_string).setText("760")
+            elif i.text == "large":
+                getattr(self, "edit_screen_custom_" + append_string).setText("900")
+            elif i.text == "xlarge":
+                getattr(self, "edit_screen_custom_" + append_string).setText("1200")
+
+    def _get_screen_save_data(self, parent_tag: etree.Element, relation: str) -> None:
+        for size in ("ge", "le"):
+            append_string = size + "_" + relation
+            if getattr(self, "edit_screen_custom_" + append_string).text() != "":
+                display_tag = etree.SubElement(parent_tag, "display_length")
+                display_tag.set("compare", size)
+                display_tag.text = getattr(self, "edit_screen_custom_" + append_string).text()
+
+    # Internet
+
+    def _update_internet_bandwith_enabled(self) -> None:
+        for relation in ("supports", "requires", "recommends"):
+            value = getattr(self, f"box_internet_{relation}").currentData()
+            enabled = value in ("first-run", "always")
+            getattr(self, f"label_internet_bandwidth_{relation}").setEnabled(enabled)
+            getattr(self, f"edit_internet_bandwidth_{relation}").setEnabled(enabled)
+            getattr(self, f"label_internet_mbit_{relation}").setEnabled(enabled)
+
+    # Modalias
+
+    def _add_modalias_row(self, relation: Optional[str] = None, chid: Optional[str] = None) -> None:
+        row = self.modalias_table.rowCount()
+        self.modalias_table.insertRow(row)
+
+        relation_box = QComboBox()
+        relation_box.addItem(QCoreApplication.translate("RelationsWidget", "Supported"), "supports")
+        relation_box.addItem(QCoreApplication.translate("RelationsWidget", "Recommend"), "recommends")
+        relation_box.addItem(QCoreApplication.translate("RelationsWidget", "Required"), "requires")
+        if relation is not None:
+            select_combo_box_data(relation_box, relation)
+        relation_box.currentIndexChanged.connect(self._main_window.set_file_edited)
+        self.modalias_table.setCellWidget(row, 0, relation_box)
+
+        item = QTableWidgetItem()
+        if chid is not None:
+            item.setText(chid)
+        self.modalias_table.setItem(row, 1, item)
+
+        remove_button = QPushButton(QCoreApplication.translate("RelationsWidget", "Remove"))
+        remove_button.clicked.connect(self._remove_modalias_clicked)
+        self.modalias_table.setCellWidget(row, 2, remove_button)
+
+        self._main_window.set_file_edited()
+
+    def _remove_modalias_clicked(self) -> None:
+        for i in range(self.modalias_table.rowCount()):
+            if self.modalias_table.cellWidget(i, 2) == self.sender():
+                self.modalias_table.removeRow(i)
+                self._main_window.set_file_edited()
+                return
+
+    # Hardware
+
+    def _add_hardware_row(self, relation: Optional[str] = None, chid: Optional[str] = None) -> None:
+        row = self.hardware_table.rowCount()
+        self.hardware_table.insertRow(row)
+
+        relation_box = QComboBox()
+        relation_box.addItem(QCoreApplication.translate("RelationsWidget", "Supported"), "supports")
+        relation_box.addItem(QCoreApplication.translate("RelationsWidget", "Recommend"), "recommends")
+        relation_box.addItem(QCoreApplication.translate("RelationsWidget", "Required"), "requires")
+        if relation is not None:
+            select_combo_box_data(relation_box, relation)
+        relation_box.currentIndexChanged.connect(self._main_window.set_file_edited)
+        self.hardware_table.setCellWidget(row, 0, relation_box)
+
+        item = QTableWidgetItem()
+        if chid is not None:
+            item.setText(chid)
+        self.hardware_table.setItem(row, 1, item)
+
+        remove_button = QPushButton(QCoreApplication.translate("RelationsWidget", "Remove"))
+        remove_button.clicked.connect(self._remove_hardware_clicked)
+        self.hardware_table.setCellWidget(row, 2, remove_button)
+
+        self._main_window.set_file_edited()
+
+    def _remove_hardware_clicked(self) -> None:
+        for i in range(self.hardware_table.rowCount()):
+            if self.hardware_table.cellWidget(i, 2) == self.sender():
+                self.hardware_table.removeRow(i)
+                self._main_window.set_file_edited()
+                return
 
     def reset_data(self) -> None:
-        clear_table_widget(self.translation_table)
-        self.suggests_list.clear()
-        self.replaces_list.clear()
-        clear_table_widget(self.tags_table)
-        clear_table_widget(self.custom_table)
-
-        self._update_suggests_edit_remove_button
-
-    def load_data(self, root_tag: etree._Element) -> None:
-        for i in root_tag.findall("translation"):
-            self._add_translation_row(translation_type=i.get("type"), domain=i.text)
-
-        suggests_tag = root_tag.find("suggests")
-        if suggests_tag is not None:
-            for i in suggests_tag.findall("id"):
-                self.suggests_list.addItem(i.text)
-
-        replaces_tag = root_tag.find("replaces")
-        if replaces_tag is not None:
-            for i in replaces_tag.findall("id"):
-                self.replaces_list.addItem(i.text)
-
-        tags_tag = root_tag.find("tags")
-        if tags_tag is not None:
-            for i in tags_tag.findall("tag"):
-                self._add_tags_row(namespace=i.get("namespace"), value=i.text)
-
-        custom_tag = root_tag.find("custom")
-        if custom_tag is not None:
-            for i in custom_tag.findall("value"):
-                self._add_custom_row(key=i.get("key"), value=i.text)
-
-    def save_data(self, root_tag: etree.Element) -> None:
-        for i in get_logical_table_row_list(self.translation_table):
-            translation_tag = etree.SubElement(root_tag, "translation")
-            translation_tag.set("type", self.translation_table.cellWidget(i, 0).currentData())
-            translation_tag.text = self.translation_table.item(i, 1).text().strip()
-
-        if self.suggests_list.count() > 0:
-            suggests_tag = etree.SubElement(root_tag, "suggests")
-            for i in range(self.suggests_list.count()):
-                id_tag = etree.SubElement(suggests_tag, "id")
-                id_tag.text = self.suggests_list.item(i).text().strip()
-
-        if self.replaces_list.count() > 0:
-            replaces_tag = etree.SubElement(root_tag, "replaces")
-            for i in range(self.replaces_list.count()):
-                id_tag = etree.SubElement(replaces_tag, "id")
-                id_tag.text = self.replaces_list.item(i).text().strip()
-
-        if self.tags_table.rowCount() > 0:
-            tags_tag = etree.SubElement(root_tag, "tags")
-            for i in get_logical_table_row_list(self.tags_table):
-                tag_tag = etree.SubElement(tags_tag, "tag")
-                tag_tag.set("namespace", self.tags_table.item(i, 0).text())
-                tag_tag.text = self.tags_table.item(i, 1).text().strip()
-
-        if self.custom_table.rowCount() > 0:
-            custom_tag = etree.SubElement(root_tag, "custom")
-            for i in get_logical_table_row_list(self.custom_table):
-                value_tag = etree.SubElement(custom_tag, "value")
-                value_tag.set("key", self.custom_table.item(i, 0).text().strip())
-                value_tag.text = self.custom_table.item(i, 1).text().strip()
+        for key, value in vars(self).items():
+            if key.startswith("rad_screen_device_class_"):
+                value.setChecked(True)
+            elif isinstance(value, QComboBox):
+                value.setCurrentIndex(0)
+            elif isinstance(value, QLineEdit):
+                value.setText("")
+            elif isinstance(value, QTableWidget):
+                clear_table_widget(value)
+
+    def load_data(self, relation_tag: etree.Element) -> None:
+        self._load_screen_data(relation_tag.findall("display_length"), relation_tag.tag)
+
+        memory_tag = relation_tag.find("memory")
+        if memory_tag is not None:
+            if relation_tag.tag == "requires":
+                self.edit_memory_requires.setText(memory_tag.text)
+            elif relation_tag.tag == "recommends":
+                self.edit_memory_recommends.setText(memory_tag.text)
+            else:
+                print("memory tag is only allowd in requires and recommends", file=sys.stderr)
+
+        internet_tag = relation_tag.find("internet")
+        if internet_tag is not None:
+            select_combo_box_data(getattr(self, f"box_internet_{relation_tag.tag}"), internet_tag.text)
+            if "bandwidth_mbitps" in internet_tag.attrib and internet_tag.text in ("first-run", "always"):
+                getattr(self, f"edit_internet_bandwidth_{relation_tag.tag}").setText(internet_tag.get("bandwidth_mbitps"))
+
+        for i in relation_tag.findall("modalias"):
+            self._add_modalias_row(relation=relation_tag.tag, chid=i.text)
+
+        for i in relation_tag.findall("hardware"):
+            self._add_hardware_row(relation=relation_tag.tag, chid=i.text)
+
+    def get_save_data(self, parent_tag: etree.Element, relation: str) -> None:
+        if relation == "requires" or relation == "recommends":
+            self._get_screen_save_data(parent_tag, relation)
+
+        if relation == "requires" and self.edit_memory_requires.text() != "":
+            memory_tag = etree.SubElement(parent_tag, "memory")
+            memory_tag.text = self.edit_memory_requires.text()
+        elif relation == "recommends" and self.edit_memory_recommends.text() != "":
+            memory_tag = etree.SubElement(parent_tag, "memory")
+            memory_tag.text = self.edit_memory_recommends.text()
+
+        internet_value = getattr(self, f"box_internet_{relation}").currentData()
+        if internet_value != "none":
+            internet_tag = etree.SubElement(parent_tag, "internet")
+            internet_tag.text = internet_value
+            if internet_value in ("first-run", "always"):
+                bandwidth = getattr(self, f"edit_internet_bandwidth_{relation}").text()
+                if bandwidth != "":
+                    internet_tag.set("bandwidth_mbitps", bandwidth)
+
+        for i in get_logical_table_row_list(self.modalias_table):
+            if self.modalias_table.cellWidget(i, 0).currentData() == relation:
+                modalias_tag = etree.SubElement(parent_tag, "modalias")
+                modalias_tag.text = self.modalias_table.item(i, 1).text().strip()
+
+        for i in get_logical_table_row_list(self.hardware_table):
+            if self.hardware_table.cellWidget(i, 0).currentData() == relation:
+                hardware_tag = etree.SubElement(parent_tag, "hardware")
+                hardware_tag.text = self.hardware_table.item(i, 1).text().strip()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ArtifactWindow.py` & `jdappstreamedit-9.1/jdAppStreamEdit/ArtifactWindow.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ChangelogImporter.py` & `jdappstreamedit-9.1/jdAppStreamEdit/ChangelogImporter.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ComposeDirectoryWindow.py` & `jdappstreamedit-9.1/jdAppStreamEdit/ComposeDirectoryWindow.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/DescriptionWidget.py` & `jdappstreamedit-9.1/jdAppStreamEdit/DescriptionWidget.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/Environment.py` & `jdappstreamedit-9.1/jdAppStreamEdit/Environment.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ExternalReleasesWindow.py` & `jdappstreamedit-9.1/jdAppStreamEdit/ExternalReleasesWindow.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/Functions.py` & `jdappstreamedit-9.1/jdAppStreamEdit/Functions.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/Icon.svg` & `jdappstreamedit-9.1/jdAppStreamEdit/Icon.svg`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ImportChangelogWindow.py` & `jdappstreamedit-9.1/jdAppStreamEdit/ImportChangelogWindow.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/Interfaces.py` & `jdappstreamedit-9.1/jdAppStreamEdit/Interfaces.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/MainWindow.py` & `jdappstreamedit-9.1/jdAppStreamEdit/MainWindow.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,14 +209,17 @@
         self.donate_action.triggered.connect(lambda: webbrowser.open("https://ko-fi.com/jakobdev"))
         self.about_action.triggered.connect(self._about_window.exec)
         self.about_qt_action.triggered.connect(QApplication.instance().aboutQt)
 
         self.setAcceptDrops(True)
 
         self.main_tab_widget.setCurrentIndex(0)
+
+        self.reset_data()
+        self._edited = False
         self.update_window_title()
 
     def set_file_edited(self) -> None:
         self._edited = True
         self.update_window_title()
 
     def update_window_title(self) -> None:
```

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ManageTemplatesWindow.py` & `jdappstreamedit-9.1/jdAppStreamEdit/ManageTemplatesWindow.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/OarsWidget.py` & `jdappstreamedit-9.1/jdAppStreamEdit/OarsWidget.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/PluginAPI.py` & `jdappstreamedit-9.1/jdAppStreamEdit/PluginAPI.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/PluginLoader.py` & `jdappstreamedit-9.1/jdAppStreamEdit/PluginLoader.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/PluginWindow.py` & `jdappstreamedit-9.1/jdAppStreamEdit/PluginWindow.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/RelationsWidget.py` & `jdappstreamedit-9.1/jdAppStreamEdit/ReleasesWidget.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,224 +1,261 @@
-from PyQt6.QtWidgets import QWidget, QComboBox, QLineEdit, QTableWidget, QTableWidgetItem, QPushButton, QHeaderView
-from .Functions import select_combo_box_data, is_string_number, get_logical_table_row_list, clear_table_widget
-from .ui_compiled.RelationsWidget import Ui_RelationsWidget
-from typing import Optional, List, TYPE_CHECKING
-from PyQt6.QtCore import QCoreApplication
-from PyQt6.QtGui import QIntValidator
+from .Functions import stretch_table_widget_colums_size, get_sender_table_row, clear_table_widget, get_logical_table_row_list, select_combo_box_data
+from PyQt6.QtWidgets import QWidget, QPushButton, QComboBox, QDateEdit, QTableWidgetItem, QMessageBox, QMenu, QInputDialog
+from .ui_compiled.ReleasesWidget import Ui_ReleasesWidget
+from PyQt6.QtCore import Qt, QCoreApplication, QDate
+from typing import Optional, Literal, TYPE_CHECKING
+from .ReleasesWindow import ReleasesWindow
+from .Interfaces import ChangelogImporter
+from PyQt6.QtGui import QAction
 from lxml import etree
+import traceback
 import sys
 
 
 if TYPE_CHECKING:
-    from .MainWindow import MainWindow
+    from .Environment import Environment
 
 
-class RelationsWidget(QWidget, Ui_RelationsWidget):
-    def __init__(self, main_window: "MainWindow") -> None:
+class _COLUMNS:
+    VERSION = 0
+    DATE = 1
+    TYPE = 2
+    EDIT_BUTTON = 3
+    REMOVE_BUTTON = 4
+
+
+class ReleasesWidget(QWidget, Ui_ReleasesWidget):
+    def __init__(self, env: "Environment", parent: QWidget) -> None:
         super().__init__()
 
         self.setupUi(self)
 
-        self._main_window = main_window
+        self._parent = parent
+        self._env = env
+
+        self._releases_window = ReleasesWindow(env, self, parent)
+
+        release_importer_menu = QMenu()
+        for i in env.release_importer:
+            importer_action = QAction(i.get_menu_text(), self)
+            importer_action.setData(i.do_import)
+            importer_action.triggered.connect(self._release_import_function)
+            release_importer_menu.addAction(importer_action)
+        release_importer_menu.setFixedWidth(self.import_button.width())
+        self.import_button.setMenu(release_importer_menu)
+        self.import_button.resizeEvent = lambda event: release_importer_menu.setFixedWidth(self.import_button.width())
+
+        stretch_table_widget_colums_size(self.releases_table)
+
+        self.releases_table.verticalHeader().setSectionsMovable(True)
+
+        self.releases_table.verticalHeader().sectionMoved.connect(self._parent.set_file_edited)
+        self.add_button.clicked.connect(self._add_button_clicked)
+        self.sort_button.clicked.connect(self._sort_button_clicked)
+
+    def _set_release_row(self, row: int, version: Optional[str] = "", date: Optional[QDate] = None, release_type: Literal["stable", "development", "snapshot"] = "stable", data: Optional[dict] = None) -> None:
+        version_item = QTableWidgetItem(version)
+        if data:
+            version_item.setData(42, data)
+        else:
+            version_item.setData(42, {})
+        self.releases_table.setItem(row, _COLUMNS.VERSION, version_item)
+
+        date_edit = QDateEdit()
+
+        if date is None:
+            date_edit.setDate(QDate.currentDate())
+        else:
+            date_edit.setDate(date)
+
+        date_edit.dateChanged.connect(self._parent.set_file_edited)
+        self.releases_table.setCellWidget(row, _COLUMNS.DATE, date_edit)
+
+        type_box = QComboBox()
+        type_box.addItem(QCoreApplication.translate("ReleasesWidget", "Stable"), "stable")
+        type_box.addItem(QCoreApplication.translate("ReleasesWidget", "Development"), "development")
+        type_box.addItem(QCoreApplication.translate("ReleasesWidget", "Snapshot"), "snapshot")
+        select_combo_box_data(type_box, release_type)
+        type_box.currentIndexChanged.connect(self._parent.set_file_edited)
+        self.releases_table.setCellWidget(row, _COLUMNS.TYPE, type_box)
+
+        edit_button = QPushButton(QCoreApplication.translate("ReleasesWidget", "Edit"))
+        edit_button.clicked.connect(self._edit_button_clicked)
+        self.releases_table.setCellWidget(row, _COLUMNS.EDIT_BUTTON, edit_button)
+
+        remove_button = QPushButton(QCoreApplication.translate("ReleasesWidget", "Remove"))
+        remove_button.clicked.connect(self._remove_button_clicked)
+        self.releases_table.setCellWidget(row, _COLUMNS.REMOVE_BUTTON, remove_button)
+
+    def _edit_button_clicked(self) -> None:
+        row = get_sender_table_row(self.releases_table, _COLUMNS.EDIT_BUTTON, self.sender())
+        self._releases_window.open_window(row)
+
+    def _remove_button_clicked(self) -> None:
+        row = get_sender_table_row(self.releases_table, _COLUMNS.REMOVE_BUTTON, self.sender())
+        self.releases_table.removeRow(row)
+        self._parent.set_file_edited()
+
+    def _add_button_clicked(self) -> None:
+        self.releases_table.insertRow(0)
+        self._set_release_row(0)
+        self._parent.set_file_edited()
+
+    def _sort_button_clicked(self) -> None:
+        try:
+            import packaging.version
+        except ModuleNotFoundError:
+            QMessageBox.critical(self, QCoreApplication.translate("ReleasesWidget", "packaging not found"), QCoreApplication.translate("ReleasesWidget", "This function needs the packaging python module to work"))
+            return
 
-        for key, value in vars(self).items():
-            if key.startswith("edit_screen_custom_") or key.startswith("edit_internet_bandwidth_"):
-                value.setValidator(QIntValidator())
-            elif key.startswith("box_internet_"):
-                value.addItem(QCoreApplication.translate("RelationsWidget", "Not specified"), "none")
-                value.addItem(QCoreApplication.translate("RelationsWidget", "Never uses the internet, even if it’s available"), "offline-only")
-                value.addItem(QCoreApplication.translate("RelationsWidget", "Uses the internet only the first time the application is run"), "first-run")
-                value.addItem(QCoreApplication.translate("RelationsWidget", "Needs internet connectivity to work"), "always")
-
-            if isinstance(value, QComboBox):
-                value.currentIndexChanged.connect(main_window.set_file_edited)
-            elif isinstance(value, QLineEdit):
-                value.textEdited.connect(main_window.set_file_edited)
-
-        self.edit_memory_requires.setValidator(QIntValidator())
-        self.edit_memory_recommends.setValidator(QIntValidator())
-
-        self.modalias_table.horizontalHeader().setSectionResizeMode(1, QHeaderView.ResizeMode.Stretch)
-        self.hardware_table.horizontalHeader().setSectionResizeMode(1, QHeaderView.ResizeMode.Stretch)
-
-        self.modalias_table.verticalHeader().setSectionsMovable(True)
-        self.hardware_table.verticalHeader().setSectionsMovable(True)
-
-        self.button_modalias_add.clicked.connect(self._add_modalias_row)
-        self.button_hardware_add.clicked.connect(self._add_hardware_row)
-
-        self._update_internet_bandwith_enabled()
-
-        self.main_tab_widget.setCurrentIndex(0)
-
-    # Screen
-
-    def _load_screen_data(self, tag_list: List[etree.Element], relation: str) -> None:
-        for i in tag_list:
-            size = i.get("compare")
-            if size is None:
-                size = "ge"
-            if size not in ("ge", "le"):
-                print("Unsupported compare attribute " + size, file=sys.stderr)
+        version_list = []
+        row_dict = {}
+
+        for row in range(self.releases_table.rowCount()):
+            version_string = self.releases_table.item(row, 0).text().strip()
+
+            if version_string == "":
                 continue
-            append_string = size + "_" + relation
-            if is_string_number(i.text):
-                getattr(self, "edit_screen_custom_" + append_string).setText(i.text)
-            elif i.text == "xsmall":
-                getattr(self, "edit_screen_custom_" + append_string).setText("360")
-            elif i.text == "small":
-                getattr(self, "edit_screen_custom_" + append_string).setText("420")
-            elif i.text == "medium":
-                getattr(self, "edit_screen_custom_" + append_string).setText("760")
-            elif i.text == "large":
-                getattr(self, "edit_screen_custom_" + append_string).setText("900")
-            elif i.text == "xlarge":
-                getattr(self, "edit_screen_custom_" + append_string).setText("1200")
-
-    def _get_screen_save_data(self, parent_tag: etree.Element, relation: str) -> None:
-        for size in ("ge", "le"):
-            append_string = size + "_" + relation
-            if getattr(self, "edit_screen_custom_" + append_string).text() != "":
-                display_tag = etree.SubElement(parent_tag, "display_length")
-                display_tag.set("compare", size)
-                display_tag.text = getattr(self, "edit_screen_custom_" + append_string).text()
-
-    # Internet
-
-    def _update_internet_bandwith_enabled(self) -> None:
-        for relation in ("supports", "requires", "recommends"):
-            value = getattr(self, f"box_internet_{relation}").currentData()
-            enabled = value in ("first-run", "always")
-            getattr(self, f"label_internet_bandwidth_{relation}").setEnabled(enabled)
-            getattr(self, f"edit_internet_bandwidth_{relation}").setEnabled(enabled)
-            getattr(self, f"label_internet_mbit_{relation}").setEnabled(enabled)
-
-    # Modalias
-
-    def _add_modalias_row(self, relation: Optional[str] = None, chid: Optional[str] = None) -> None:
-        row = self.modalias_table.rowCount()
-        self.modalias_table.insertRow(row)
-
-        relation_box = QComboBox()
-        relation_box.addItem(QCoreApplication.translate("RelationsWidget", "Supported"), "supports")
-        relation_box.addItem(QCoreApplication.translate("RelationsWidget", "Recommend"), "recommends")
-        relation_box.addItem(QCoreApplication.translate("RelationsWidget", "Required"), "requires")
-        if relation is not None:
-            select_combo_box_data(relation_box, relation)
-        relation_box.currentIndexChanged.connect(self._main_window.set_file_edited)
-        self.modalias_table.setCellWidget(row, 0, relation_box)
-
-        item = QTableWidgetItem()
-        if chid is not None:
-            item.setText(chid)
-        self.modalias_table.setItem(row, 1, item)
-
-        remove_button = QPushButton(QCoreApplication.translate("RelationsWidget", "Remove"))
-        remove_button.clicked.connect(self._remove_modalias_clicked)
-        self.modalias_table.setCellWidget(row, 2, remove_button)
-
-        self._main_window.set_file_edited()
-
-    def _remove_modalias_clicked(self) -> None:
-        for i in range(self.modalias_table.rowCount()):
-            if self.modalias_table.cellWidget(i, 2) == self.sender():
-                self.modalias_table.removeRow(i)
-                self._main_window.set_file_edited()
+
+            try:
+                version = packaging.version.Version(version_string)
+            except packaging.version.InvalidVersion:
+                QMessageBox.critical(self, QCoreApplication.translate("ReleasesWidget", "Could not parse version"), QCoreApplication.translate("ReleasesWidget", "Could not parse version {{version}}").replace("{{version}}", version_string))
+                return
+
+            row_dict[version] = {"date": self.releases_table.cellWidget(row, 1).date(), "type": self.releases_table.cellWidget(row, 2).currentData() == "development", "data": self.releases_table.item(row, 0).data(42)}
+            version_list.append(version)
+
+        clear_table_widget(self.releases_table)
+
+        version_list.sort(reverse=True)
+
+        for row, version in enumerate(version_list):
+            self.releases_table.insertRow(row)
+            self._set_release_row(row, version=str(version), date=row_dict[version]["date"], release_type=row_dict[version]["type"], data=row_dict[version]["data"])
+
+        self._parent.set_file_edited()
+
+    def _release_import_function(self) -> None:
+        action = self.sender()
+
+        if not action:
+            return
+
+        try:
+            release_data = action.data()(self)
+        except Exception:
+            print(traceback.format_exc(), end="", file=sys.stderr)
+
+            msg_box = QMessageBox()
+            msg_box.setWindowTitle(QCoreApplication.translate("ReleasesWidget", "Error"))
+            msg_box.setText(QCoreApplication.translate("ReleasesWidget", "An Error happened during Import"))
+            msg_box.setDetailedText(traceback.format_exc())
+            msg_box.setIcon(QMessageBox.Icon.Critical)
+            msg_box.exec()
+
+            return
+
+        if release_data is None or len(release_data["releases"]) == 0:
+            return
+
+        changelog_importer: Optional[ChangelogImporter] = None
+        if release_data.get("changelog_importer") is True:
+            changelog_importer_list: list[str] = []
+            changelog_importer_dict: dict[str, ChangelogImporter] = {}
+
+            changelog_importer_list.append(QCoreApplication.translate("ReleasesWidget", "None"))
+            for current_importer in self._env.changelog_importer:
+                changelog_importer_list.append(current_importer.get_name())
+                changelog_importer_dict[current_importer.get_name()] = current_importer
+
+            changelog_importer_name, ok = QInputDialog.getItem(self, QCoreApplication.translate("ReleasesWidget", "Import Changelog"), QCoreApplication.translate("ReleasesWidget", "jdAppStreamEdit can import the changelog if it adheres to a specific format. If this is the case, please choose the appropriate format."), changelog_importer_list, editable=False)
+            if ok and changelog_importer_name in changelog_importer_dict:
+                changelog_importer = changelog_importer_dict[changelog_importer_name]
+
+        if self.releases_table.rowCount() > 0:
+            ans = QMessageBox.question(self, QCoreApplication.translate("ReleasesWidget", "Overwrite everything"), QCoreApplication.translate("ReleasesWidget", "If you proceed, all your chnages in the release tab will be overwritten. Continue?"), QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No)
+            if ans != QMessageBox.StandardButton.Yes:
                 return
 
-    # Hardware
+        clear_table_widget(self.releases_table)
+
+        for count, i in enumerate(release_data["releases"]):
+            changelog_text = i.get("changelog_text", "")
+            if changelog_importer is not None and changelog_text is not None and changelog_text != "":
+                try:
+                    changelog, _ = changelog_importer.do_import(changelog_text)
+
+                    if changelog is not None:
+                        if "data" not in i:
+                            i["data"] = {}
+                        i["data"]["description"] = changelog
+                except Exception:
+                    print(traceback.format_exc(), end="", file=sys.stderr)
+
+            self.releases_table.insertRow(count)
+            try:
+                self._set_release_row(count, version=i["version"], date=i["date"], release_type=i.get("type", "stable"), data=i.get("data", {}))
+            except Exception:
+                print(traceback.format_exc(), end="", file=sys.stderr)
+
+                msg_box = QMessageBox()
+                msg_box.setWindowTitle(QCoreApplication.translate("ReleasesWidget", "Error"))
+                msg_box.setText(QCoreApplication.translate("ReleasesWidget", "An Error happened during Import"))
+                msg_box.setDetailedText(traceback.format_exc())
+                msg_box.setIcon(QMessageBox.Icon.Critical)
+                msg_box.exec()
 
-    def _add_hardware_row(self, relation: Optional[str] = None, chid: Optional[str] = None) -> None:
-        row = self.hardware_table.rowCount()
-        self.hardware_table.insertRow(row)
-
-        relation_box = QComboBox()
-        relation_box.addItem(QCoreApplication.translate("RelationsWidget", "Supported"), "supports")
-        relation_box.addItem(QCoreApplication.translate("RelationsWidget", "Recommend"), "recommends")
-        relation_box.addItem(QCoreApplication.translate("RelationsWidget", "Required"), "requires")
-        if relation is not None:
-            select_combo_box_data(relation_box, relation)
-        relation_box.currentIndexChanged.connect(self._main_window.set_file_edited)
-        self.hardware_table.setCellWidget(row, 0, relation_box)
-
-        item = QTableWidgetItem()
-        if chid is not None:
-            item.setText(chid)
-        self.hardware_table.setItem(row, 1, item)
-
-        remove_button = QPushButton(QCoreApplication.translate("RelationsWidget", "Remove"))
-        remove_button.clicked.connect(self._remove_hardware_clicked)
-        self.hardware_table.setCellWidget(row, 2, remove_button)
-
-        self._main_window.set_file_edited()
-
-    def _remove_hardware_clicked(self) -> None:
-        for i in range(self.hardware_table.rowCount()):
-            if self.hardware_table.cellWidget(i, 2) == self.sender():
-                self.hardware_table.removeRow(i)
-                self._main_window.set_file_edited()
                 return
 
+        self._parent.set_file_edited()
+
     def reset_data(self) -> None:
-        for key, value in vars(self).items():
-            if key.startswith("rad_screen_device_class_"):
-                value.setChecked(True)
-            elif isinstance(value, QComboBox):
-                value.setCurrentIndex(0)
-            elif isinstance(value, QLineEdit):
-                value.setText("")
-            elif isinstance(value, QTableWidget):
-                clear_table_widget(value)
-
-    def load_data(self, relation_tag: etree.Element) -> None:
-        self._load_screen_data(relation_tag.findall("display_length"), relation_tag.tag)
-
-        memory_tag = relation_tag.find("memory")
-        if memory_tag is not None:
-            if relation_tag.tag == "requires":
-                self.edit_memory_requires.setText(memory_tag.text)
-            elif relation_tag.tag == "recommends":
-                self.edit_memory_recommends.setText(memory_tag.text)
-            else:
-                print("memory tag is only allowd in requires and recommends", file=sys.stderr)
-
-        internet_tag = relation_tag.find("internet")
-        if internet_tag is not None:
-            select_combo_box_data(getattr(self, f"box_internet_{relation_tag.tag}"), internet_tag.text)
-            if "bandwidth_mbitps" in internet_tag.attrib and internet_tag.text in ("first-run", "always"):
-                getattr(self, f"edit_internet_bandwidth_{relation_tag.tag}").setText(internet_tag.get("bandwidth_mbitps"))
-
-        for i in relation_tag.findall("modalias"):
-            self._add_modalias_row(relation=relation_tag.tag, chid=i.text)
-
-        for i in relation_tag.findall("hardware"):
-            self._add_hardware_row(relation=relation_tag.tag, chid=i.text)
-
-    def get_save_data(self, parent_tag: etree.Element, relation: str) -> None:
-        if relation == "requires" or relation == "recommends":
-            self._get_screen_save_data(parent_tag, relation)
-
-        if relation == "requires" and self.edit_memory_requires.text() != "":
-            memory_tag = etree.SubElement(parent_tag, "memory")
-            memory_tag.text = self.edit_memory_requires.text()
-        elif relation == "recommends" and self.edit_memory_recommends.text() != "":
-            memory_tag = etree.SubElement(parent_tag, "memory")
-            memory_tag.text = self.edit_memory_recommends.text()
-
-        internet_value = getattr(self, f"box_internet_{relation}").currentData()
-        if internet_value != "none":
-            internet_tag = etree.SubElement(parent_tag, "internet")
-            internet_tag.text = internet_value
-            if internet_value in ("first-run", "always"):
-                bandwidth = getattr(self, f"edit_internet_bandwidth_{relation}").text()
-                if bandwidth != "":
-                    internet_tag.set("bandwidth_mbitps", bandwidth)
-
-        for i in get_logical_table_row_list(self.modalias_table):
-            if self.modalias_table.cellWidget(i, 0).currentData() == relation:
-                modalias_tag = etree.SubElement(parent_tag, "modalias")
-                modalias_tag.text = self.modalias_table.item(i, 1).text().strip()
-
-        for i in get_logical_table_row_list(self.hardware_table):
-            if self.hardware_table.cellWidget(i, 0).currentData() == relation:
-                hardware_tag = etree.SubElement(parent_tag, "hardware")
-                hardware_tag.text = self.hardware_table.item(i, 1).text().strip()
+        clear_table_widget(self.releases_table)
+
+    def load_tag(self, releases_tag: etree._Element) -> None:
+        for i in releases_tag.getchildren():
+            current_row = self.releases_table.rowCount()
+            data = {}
+
+            if i.get("urgency") is not None:
+                data["urgency"] = i.get("urgency")
+
+            url_tag = i.find("url")
+            if url_tag is not None:
+                data["url"] = url_tag.text
+
+            description_tag = i.find("description")
+            if description_tag is not None:
+                data["description"] = description_tag
+
+            artifacts_tag = i.find("artifacts")
+            if artifacts_tag is not None:
+                data["artifacts"] = artifacts_tag
+
+            self.releases_table.insertRow(current_row)
+            self._set_release_row(current_row, version=i.get("version"), date=QDate.fromString(i.get("date"), Qt.DateFormat.ISODate), release_type=(i.get("type", "stable")), data=data)
+
+    def write_tag(self, releases_tag: etree.Element) -> None:
+        for i in get_logical_table_row_list(self.releases_table):
+            version = self.releases_table.item(i, _COLUMNS.VERSION).text().strip()
+            date = self.releases_table.cellWidget(i, _COLUMNS.DATE).date().toString(Qt.DateFormat.ISODate)
+            release_type = self.releases_table.cellWidget(i, _COLUMNS.TYPE).currentData()
+            single_release_tag = etree.SubElement(releases_tag, "release")
+            single_release_tag.set("version", version)
+            single_release_tag.set("date", date)
+            single_release_tag.set("type", release_type)
+
+            data = self.releases_table.item(i, _COLUMNS.VERSION).data(42)
+
+            if "urgency" in data:
+                single_release_tag.set("urgency", data["urgency"])
+
+            if "url" in data:
+                url_tag = etree.SubElement(single_release_tag, "url")
+                url_tag.text = data["url"]
+
+            if "description" in data:
+                single_release_tag.append(data["description"])
+
+            if "artifacts" in data:
+                single_release_tag.append(data["artifacts"])
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ReleaseImporter.py` & `jdappstreamedit-9.1/jdAppStreamEdit/ReleaseImporter.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ReleasesWindow.py` & `jdappstreamedit-9.1/jdAppStreamEdit/ReleasesWindow.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ScreenshotWindow.py` & `jdappstreamedit-9.1/jdAppStreamEdit/ScreenshotWindow.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/Settings.py` & `jdappstreamedit-9.1/jdAppStreamEdit/Settings.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/SettingsWindow.py` & `jdappstreamedit-9.1/jdAppStreamEdit/SettingsWindow.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/SysinfoWindow.py` & `jdappstreamedit-9.1/jdAppStreamEdit/SysinfoWindow.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ThumbnailWindow.py` & `jdappstreamedit-9.1/jdAppStreamEdit/ThumbnailWindow.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/TranslateWindow.py` & `jdappstreamedit-9.1/jdAppStreamEdit/TranslateWindow.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/Types.py` & `jdappstreamedit-9.1/jdAppStreamEdit/Types.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ValidateWindow.py` & `jdappstreamedit-9.1/jdAppStreamEdit/ValidateWindow.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ViewCatalogWindow.py` & `jdappstreamedit-9.1/jdAppStreamEdit/ViewCatalogWindow.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ViewXMLWindow.py` & `jdappstreamedit-9.1/jdAppStreamEdit/ViewXMLWindow.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/XMLHighlighter.py` & `jdappstreamedit-9.1/jdAppStreamEdit/XMLHighlighter.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/__init__.py` & `jdappstreamedit-9.1/jdAppStreamEdit/__init__.py`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/data/categories.txt` & `jdappstreamedit-9.1/jdAppStreamEdit/data/categories.txt`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/data/changelog.html` & `jdappstreamedit-9.1/jdAppStreamEdit/data/changelog.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+<b>9.1</b><br>
+• Added support for branding colors<br>
+• Added Russian translation (0ko)<br>
+<br>
 <b>9.0</b><br>
 • Allow importing the changelog<br>
 • Add support for developer tag<br>
 • Allow multiple launchable<br>
 • Improve license handling (Alexander Wilms)<br>
 <br>
 <b>8.0</b><br>
```

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/data/language_codes.csv` & `jdappstreamedit-9.1/jdAppStreamEdit/data/language_codes.csv`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/data/metadata_licenses.json` & `jdappstreamedit-9.1/jdAppStreamEdit/data/metadata_licenses.json`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/data/platform.json` & `jdappstreamedit-9.1/jdAppStreamEdit/data/platform.json`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/data/project_licenses.json` & `jdappstreamedit-9.1/jdAppStreamEdit/data/project_licenses.json`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/translations/jdAppStreamEdit_de.ts` & `jdappstreamedit-9.1/jdAppStreamEdit/translations/jdAppStreamEdit_de.ts`

 * *Files 1% similar despite different names*

#### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/translations/jdAppStreamEdit_de.ts` & `jdappstreamedit-9.1/jdAppStreamEdit/translations/jdAppStreamEdit_de.ts`

```diff
@@ -44,69 +44,69 @@
     <name>AdvancedWidget</name>
     <message>
       <location filename="../ui/AdvancedWidget.ui" line="0"/>
       <location filename="../ui/AdvancedWidget.ui" line="0"/>
       <location filename="../ui/AdvancedWidget.ui" line="0"/>
       <location filename="../ui/AdvancedWidget.ui" line="0"/>
       <location filename="../ui/AdvancedWidget.ui" line="0"/>
-      <location filename="../AdvancedWidget.py" line="208"/>
-      <location filename="../AdvancedWidget.py" line="181"/>
-      <location filename="../AdvancedWidget.py" line="72"/>
+      <location filename="../AdvancedWidget.py" line="246"/>
+      <location filename="../AdvancedWidget.py" line="189"/>
+      <location filename="../AdvancedWidget.py" line="80"/>
       <source>Remove</source>
       <translation>Löschen</translation>
     </message>
     <message>
-      <location filename="../AdvancedWidget.py" line="86"/>
+      <location filename="../AdvancedWidget.py" line="94"/>
       <source>New Suggestion</source>
       <translation>Neuer Vorschlag</translation>
     </message>
     <message>
-      <location filename="../AdvancedWidget.py" line="86"/>
+      <location filename="../AdvancedWidget.py" line="94"/>
       <source>Please enter a new ID</source>
       <translation>Bitte gib eine ID ein</translation>
     </message>
     <message>
-      <location filename="../AdvancedWidget.py" line="145"/>
-      <location filename="../AdvancedWidget.py" line="131"/>
-      <location filename="../AdvancedWidget.py" line="104"/>
-      <location filename="../AdvancedWidget.py" line="90"/>
+      <location filename="../AdvancedWidget.py" line="153"/>
+      <location filename="../AdvancedWidget.py" line="139"/>
+      <location filename="../AdvancedWidget.py" line="112"/>
+      <location filename="../AdvancedWidget.py" line="98"/>
       <source>ID in List</source>
       <translation>ID in der Liste</translation>
     </message>
     <message>
-      <location filename="../AdvancedWidget.py" line="145"/>
-      <location filename="../AdvancedWidget.py" line="131"/>
-      <location filename="../AdvancedWidget.py" line="104"/>
-      <location filename="../AdvancedWidget.py" line="90"/>
+      <location filename="../AdvancedWidget.py" line="153"/>
+      <location filename="../AdvancedWidget.py" line="139"/>
+      <location filename="../AdvancedWidget.py" line="112"/>
+      <location filename="../AdvancedWidget.py" line="98"/>
       <source>This ID is already in the List</source>
       <translation>Diese ID ist bereits in der Liste</translation>
     </message>
     <message>
-      <location filename="../AdvancedWidget.py" line="100"/>
+      <location filename="../AdvancedWidget.py" line="108"/>
       <source>Edit Suggestion</source>
       <translation>Vorschlag bearbeiten</translation>
     </message>
     <message>
-      <location filename="../AdvancedWidget.py" line="141"/>
-      <location filename="../AdvancedWidget.py" line="100"/>
+      <location filename="../AdvancedWidget.py" line="149"/>
+      <location filename="../AdvancedWidget.py" line="108"/>
       <source>Please edit the ID</source>
       <translation>Bitte bearbeite die ID</translation>
     </message>
     <message>
-      <location filename="../AdvancedWidget.py" line="127"/>
+      <location filename="../AdvancedWidget.py" line="135"/>
       <source>New Replacement</source>
       <translation>Neuer Ersatz</translation>
     </message>
     <message>
-      <location filename="../AdvancedWidget.py" line="127"/>
+      <location filename="../AdvancedWidget.py" line="135"/>
       <source>Please enter a ID</source>
       <translation>Bitte gib eine ID ein</translation>
     </message>
     <message>
-      <location filename="../AdvancedWidget.py" line="141"/>
+      <location filename="../AdvancedWidget.py" line="149"/>
       <source>Edit Replacement</source>
       <translation>Ersatz bearbeiten</translation>
     </message>
     <message>
       <location filename="../ui/AdvancedWidget.ui" line="0"/>
       <source>Translation</source>
       <translation>Übersetzung</translation>
@@ -180,14 +180,36 @@
       <location filename="../ui/AdvancedWidget.ui" line="0"/>
       <location filename="../ui/AdvancedWidget.ui" line="0"/>
       <source>Value</source>
       <translation>Wert</translation>
     </message>
     <message>
       <location filename="../ui/AdvancedWidget.ui" line="0"/>
+      <source>Branding</source>
+      <translation>Marke</translation>
+    </message>
+    <message>
+      <location filename="../ui/AdvancedWidget.ui" line="0"/>
+      <source>Set branding colors</source>
+      <translation>Markenfarben festlegen</translation>
+    </message>
+    <message>
+      <location filename="../ui/AdvancedWidget.ui" line="0"/>
+      <source>Light:</source>
+      <extracomment>Theme</extracomment>
+      <translation>Hell:</translation>
+    </message>
+    <message>
+      <location filename="../ui/AdvancedWidget.ui" line="0"/>
+      <source>Dark:</source>
+      <extracomment>Theme</extracomment>
+      <translation>Dunkel:</translation>
+    </message>
+    <message>
+      <location filename="../ui/AdvancedWidget.ui" line="0"/>
       <source>Custom</source>
       <translation>Eigen</translation>
     </message>
     <message>
       <location filename="../ui/AdvancedWidget.ui" line="0"/>
       <source>You can add custom values here. For more information take a look at the documentation.</source>
       <translation>Du kannst hier eigene Werte eintragen. Für mehr Informationen wirf einen Blick in die Dokumentation.</translation>
@@ -840,25 +862,30 @@
       <translation>Deutsch</translation>
     </message>
     <message>
       <location filename="../Languages.py" line="8"/>
       <source>Dutch</source>
       <translation>Niederländisch</translation>
     </message>
+    <message>
+      <location filename="../Languages.py" line="9"/>
+      <source>Russian</source>
+      <translation>Russisch</translation>
+    </message>
   </context>
   <context>
     <name>MainWindow</name>
     <message>
-      <location filename="../MainWindow.py" line="456"/>
+      <location filename="../MainWindow.py" line="459"/>
       <location filename="../ExternalReleasesWindow.py" line="224"/>
       <source>No Plugins installed</source>
       <translation>Keine Plugins installiert</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="456"/>
+      <location filename="../MainWindow.py" line="459"/>
       <location filename="../ExternalReleasesWindow.py" line="224"/>
       <source>You have no Plugins installed</source>
       <translation>Du jast keine Plugins installiert</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="83"/>
       <source>Not specified</source>
@@ -931,305 +958,305 @@
     </message>
     <message>
       <location filename="../MainWindow.py" line="129"/>
       <source>Unknown</source>
       <translation>Unbekannt</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="226"/>
+      <location filename="../MainWindow.py" line="229"/>
       <source>Untitled</source>
       <translation>Unbenannt</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="772"/>
-      <location filename="../MainWindow.py" line="748"/>
-      <location filename="../MainWindow.py" line="232"/>
+      <location filename="../MainWindow.py" line="775"/>
+      <location filename="../MainWindow.py" line="751"/>
+      <location filename="../MainWindow.py" line="235"/>
       <source>Error</source>
       <translation>Fehler</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="243"/>
+      <location filename="../MainWindow.py" line="246"/>
       <source>No templates found</source>
       <translation>Keine Vorlagen gefunden</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="257"/>
+      <location filename="../MainWindow.py" line="260"/>
       <source>No recent files</source>
       <translation>Keine zuletzt geöffneten Dateien</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="270"/>
+      <location filename="../MainWindow.py" line="273"/>
       <source>Clear</source>
       <translation>Löschen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="287"/>
+      <location filename="../MainWindow.py" line="290"/>
       <source>Unsaved changes</source>
       <translation>Nicht gespeicherte Änderungen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="287"/>
+      <location filename="../MainWindow.py" line="290"/>
       <source>You have unsaved changes. Do you want to save now?</source>
       <translation>Du hast nicht gespeicherte Änderungen. Möchtest du sie jetzt speichern?</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="298"/>
+      <location filename="../MainWindow.py" line="301"/>
       <source>Welcome to jdAppStreamEdit!</source>
       <translation>Willkommen bei jdAppStreamEdit!</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="299"/>
+      <location filename="../MainWindow.py" line="302"/>
       <source>With jdAppStreamEdit you can create and edit AppStream files (*.metainfo.xml or .appdata.xml). This files are to provide data for your Application (Description, Screenshots etc.) to Software Centers.</source>
       <translation>Mit jdAppStreamEditt kannst du AppStream Dateien (*.metainfo.xml oder *.appdata.xml) erstellen und bearbeiten. Diese Dateien stellen Informationen (z.B. Beschreibung, Screeenshots usw.) für Software Center zur Verfügung.</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="300"/>
+      <location filename="../MainWindow.py" line="303"/>
       <source>It is highly recommend to read the the AppStream Documentation before using this Program. You can open it under ?&gt;AppStream documentation.</source>
       <translation>Es wird empfohlen vor der benutzung die AppStream Dokumentation zu lesen. Du findest sie unter ?&gt;AppStream Dokumentation.</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="301"/>
+      <location filename="../MainWindow.py" line="304"/>
       <source>You can check if your AppStream is valid under Tools&gt;Validate.</source>
       <translation>Du kannst deine AppStream Datei unter Werkzeuge&gt;Validieren auf Gültigkeit überprüfen.</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="304"/>
+      <location filename="../MainWindow.py" line="307"/>
       <source>Show this dialog at startup</source>
       <translation>Diesen Dialog beim Programmstart anzeigen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="308"/>
+      <location filename="../MainWindow.py" line="311"/>
       <source>Welcome</source>
       <translation>Willkommen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="329"/>
+      <location filename="../MainWindow.py" line="332"/>
       <source>desktop-entry-lib not found</source>
       <translation>desktop-entrylib nicht gefunden</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="329"/>
+      <location filename="../MainWindow.py" line="332"/>
       <source>This function needs the desktop-entry-lib python module to work</source>
       <translation>Diese Funktion benötigt das desktop-entry-lib Python Modul</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="337"/>
+      <location filename="../MainWindow.py" line="340"/>
       <source>Desktop Entry Files</source>
       <translation>Desktopeinträge</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="433"/>
-      <location filename="../MainWindow.py" line="395"/>
-      <location filename="../MainWindow.py" line="337"/>
+      <location filename="../MainWindow.py" line="436"/>
+      <location filename="../MainWindow.py" line="398"/>
+      <location filename="../MainWindow.py" line="340"/>
       <source>All Files</source>
       <translation>Alle Dateien</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="345"/>
+      <location filename="../MainWindow.py" line="348"/>
       <source>Could not read file</source>
       <translation>Konnte Datei nicht lesen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="345"/>
+      <location filename="../MainWindow.py" line="348"/>
       <source>Could not read {{path}}. Make sure it is a valid desktop entry and you have the Permission to read it.</source>
       <translation>Konnte {{path}} nicht lesen. Stelle sicher, dass die Datei ein gültiger Desktopeintrag ist und du Leserechte besitzt.</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="433"/>
-      <location filename="../MainWindow.py" line="395"/>
+      <location filename="../MainWindow.py" line="436"/>
+      <location filename="../MainWindow.py" line="398"/>
       <source>AppStream Files</source>
       <translation>AppStream Dateien</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="417"/>
+      <location filename="../MainWindow.py" line="420"/>
       <source>Enter URL</source>
       <translation>URL eingeben</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="417"/>
+      <location filename="../MainWindow.py" line="420"/>
       <source>Please enter a URL</source>
       <translation>Bitte gib eine URL ein</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
-      <location filename="../MainWindow.py" line="485"/>
+      <location filename="../MainWindow.py" line="488"/>
       <source>Edit</source>
       <translation>Bearbeiten</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
-      <location filename="../MainWindow.py" line="646"/>
-      <location filename="../MainWindow.py" line="609"/>
-      <location filename="../MainWindow.py" line="489"/>
+      <location filename="../MainWindow.py" line="649"/>
+      <location filename="../MainWindow.py" line="612"/>
+      <location filename="../MainWindow.py" line="492"/>
       <source>Remove</source>
       <translation>Löschen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="763"/>
-      <location filename="../MainWindow.py" line="557"/>
-      <location filename="../MainWindow.py" line="497"/>
+      <location filename="../MainWindow.py" line="766"/>
+      <location filename="../MainWindow.py" line="560"/>
+      <location filename="../MainWindow.py" line="500"/>
       <source>Invalid URL</source>
       <translation>Ungültige URL</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="497"/>
+      <location filename="../MainWindow.py" line="500"/>
       <source>The URL {{url}} does not work</source>
       <translation>Die URL {{url}} funktioniert nicht</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="559"/>
-      <location filename="../MainWindow.py" line="499"/>
+      <location filename="../MainWindow.py" line="562"/>
+      <location filename="../MainWindow.py" line="502"/>
       <source>Everything OK</source>
       <translation>Alles in Ordnung</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="559"/>
-      <location filename="../MainWindow.py" line="499"/>
+      <location filename="../MainWindow.py" line="562"/>
+      <location filename="../MainWindow.py" line="502"/>
       <source>All URLs are working</source>
       <translation>Alle URLs funktionieren</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="557"/>
+      <location filename="../MainWindow.py" line="560"/>
       <source>The URL {url} does not work</source>
       <translation>Die URL {url} funktioniert nicht</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="570"/>
+      <location filename="../MainWindow.py" line="573"/>
       <source>Add a Categorie</source>
       <translation>Kategorie hinzufügen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="570"/>
+      <location filename="../MainWindow.py" line="573"/>
       <source>Please select a Categorie from the list below</source>
       <translation>Bitte wähle eine Kategorie aus</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="574"/>
+      <location filename="../MainWindow.py" line="577"/>
       <source>Categorie already added</source>
       <translation>Kategorie bereits vorhanden</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="574"/>
+      <location filename="../MainWindow.py" line="577"/>
       <source>You can't add the same Categorie twice</source>
       <translation>Du kannst dieselbe Kategorie nicht ein zweites Mal hinzufügen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="662"/>
+      <location filename="../MainWindow.py" line="665"/>
       <source>New Keyword</source>
       <translation>Neues Schlüsselwort</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="662"/>
+      <location filename="../MainWindow.py" line="665"/>
       <source>Please enter a new Keyword</source>
       <translation>Bitte gib ein neues Schlüsselwort ein</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="682"/>
-      <location filename="../MainWindow.py" line="666"/>
+      <location filename="../MainWindow.py" line="685"/>
+      <location filename="../MainWindow.py" line="669"/>
       <source>Keyword in List</source>
       <translation>Schlüsselwort in Liste</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="682"/>
-      <location filename="../MainWindow.py" line="666"/>
+      <location filename="../MainWindow.py" line="685"/>
+      <location filename="../MainWindow.py" line="669"/>
       <source>This Keyword is already in the List</source>
       <translation>ADs Schlüsselwort befindet sich bereits in der Liste</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="676"/>
+      <location filename="../MainWindow.py" line="679"/>
       <source>Edit Keyword</source>
       <translation>Schlüsselwort bearbeiten</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="676"/>
+      <location filename="../MainWindow.py" line="679"/>
       <source>Please edit the Keyword</source>
       <translation>Bitte bearbeite das Schlüsselwort</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="745"/>
+      <location filename="../MainWindow.py" line="748"/>
       <source>File not found</source>
       <translation>datei nicht gefunden</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="745"/>
+      <location filename="../MainWindow.py" line="748"/>
       <source>{{path}} does not exists</source>
       <translation>{{path}} existiert nicht</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="748"/>
+      <location filename="../MainWindow.py" line="751"/>
       <source>An error occurred while trying to open {{path}}</source>
       <translation>Während des öffnens von {{path}} ist ein Fehler aufgetreten</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="763"/>
+      <location filename="../MainWindow.py" line="766"/>
       <source>{{url}} is not a valid http/https URL</source>
       <translation>{{url}} ist keine gültige http/https URL</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="769"/>
+      <location filename="../MainWindow.py" line="772"/>
       <source>Could not connect</source>
       <translation>Kann nicht verbinden</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="769"/>
+      <location filename="../MainWindow.py" line="772"/>
       <source>Could not connect to {{url}}</source>
       <translation>Es kann keine Verbindung zu {{url}} aufgebaut werden</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="772"/>
+      <location filename="../MainWindow.py" line="775"/>
       <source>An error occurred while trying to connect to {{url}}</source>
       <translation>Während des verbindens zu {{url}} ist ein fehler aufgetreten</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="833"/>
+      <location filename="../MainWindow.py" line="836"/>
       <source>XML parsing failed</source>
       <translation>XML parsen fehlgeschlagen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="837"/>
+      <location filename="../MainWindow.py" line="840"/>
       <source>No component tag</source>
       <translation>Kein component Tag</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="837"/>
+      <location filename="../MainWindow.py" line="840"/>
       <source>This XML file has no component tag</source>
       <translation>Die XML Datei hat keinen component Tag</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="840"/>
+      <location filename="../MainWindow.py" line="843"/>
       <source>Too many component tags</source>
       <translation>Zu viele components Tags</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="840"/>
+      <location filename="../MainWindow.py" line="843"/>
       <source>Only files with one component tag are supported</source>
       <translation>Nur ein component Tag ist erlaubt</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="1178"/>
+      <location filename="../MainWindow.py" line="1185"/>
       <source>No ID</source>
       <translation>Keine ID</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="1178"/>
+      <location filename="../MainWindow.py" line="1185"/>
       <source>You need to set a ID to use this feature</source>
       <translation>Du benötigst eine ID, um dieses Feature nutzen zu können</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="1197"/>
+      <location filename="../MainWindow.py" line="1204"/>
       <source>{{binary}} not found</source>
       <translation>{{binary}} nicht gefunden</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="1197"/>
+      <location filename="../MainWindow.py" line="1204"/>
       <source>{{binary}} was not found. Make sure it is installed and in PATH.</source>
       <translation>{{binary}} wurde nicht gefunden. Stelle sicher, dass es installiert und im PATH ist.</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>General</source>
       <translation>Allgemein</translation>
```

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/translations/jdAppStreamEdit_nl.ts` & `jdappstreamedit-9.1/jdAppStreamEdit/translations/jdAppStreamEdit_nl.ts`

 * *Files 1% similar despite different names*

#### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/translations/jdAppStreamEdit_nl.ts` & `jdappstreamedit-9.1/jdAppStreamEdit/translations/jdAppStreamEdit_nl.ts`

```diff
@@ -44,69 +44,69 @@
     <name>AdvancedWidget</name>
     <message>
       <location filename="../ui/AdvancedWidget.ui" line="0"/>
       <location filename="../ui/AdvancedWidget.ui" line="0"/>
       <location filename="../ui/AdvancedWidget.ui" line="0"/>
       <location filename="../ui/AdvancedWidget.ui" line="0"/>
       <location filename="../ui/AdvancedWidget.ui" line="0"/>
-      <location filename="../AdvancedWidget.py" line="208"/>
-      <location filename="../AdvancedWidget.py" line="181"/>
-      <location filename="../AdvancedWidget.py" line="72"/>
+      <location filename="../AdvancedWidget.py" line="246"/>
+      <location filename="../AdvancedWidget.py" line="189"/>
+      <location filename="../AdvancedWidget.py" line="80"/>
       <source>Remove</source>
       <translation>Verwijderen</translation>
     </message>
     <message>
-      <location filename="../AdvancedWidget.py" line="86"/>
+      <location filename="../AdvancedWidget.py" line="94"/>
       <source>New Suggestion</source>
       <translation>Nieuwe suggestie</translation>
     </message>
     <message>
-      <location filename="../AdvancedWidget.py" line="86"/>
+      <location filename="../AdvancedWidget.py" line="94"/>
       <source>Please enter a new ID</source>
       <translation>Voer een nieuwe id in</translation>
     </message>
     <message>
-      <location filename="../AdvancedWidget.py" line="145"/>
-      <location filename="../AdvancedWidget.py" line="131"/>
-      <location filename="../AdvancedWidget.py" line="104"/>
-      <location filename="../AdvancedWidget.py" line="90"/>
+      <location filename="../AdvancedWidget.py" line="153"/>
+      <location filename="../AdvancedWidget.py" line="139"/>
+      <location filename="../AdvancedWidget.py" line="112"/>
+      <location filename="../AdvancedWidget.py" line="98"/>
       <source>ID in List</source>
       <translation>ID bestaat al</translation>
     </message>
     <message>
-      <location filename="../AdvancedWidget.py" line="145"/>
-      <location filename="../AdvancedWidget.py" line="131"/>
-      <location filename="../AdvancedWidget.py" line="104"/>
-      <location filename="../AdvancedWidget.py" line="90"/>
+      <location filename="../AdvancedWidget.py" line="153"/>
+      <location filename="../AdvancedWidget.py" line="139"/>
+      <location filename="../AdvancedWidget.py" line="112"/>
+      <location filename="../AdvancedWidget.py" line="98"/>
       <source>This ID is already in the List</source>
       <translation>Deze id staat al op de lijst</translation>
     </message>
     <message>
-      <location filename="../AdvancedWidget.py" line="100"/>
+      <location filename="../AdvancedWidget.py" line="108"/>
       <source>Edit Suggestion</source>
       <translation>Suggestie bewerken</translation>
     </message>
     <message>
-      <location filename="../AdvancedWidget.py" line="141"/>
-      <location filename="../AdvancedWidget.py" line="100"/>
+      <location filename="../AdvancedWidget.py" line="149"/>
+      <location filename="../AdvancedWidget.py" line="108"/>
       <source>Please edit the ID</source>
       <translation>Bewerk de id</translation>
     </message>
     <message>
-      <location filename="../AdvancedWidget.py" line="127"/>
+      <location filename="../AdvancedWidget.py" line="135"/>
       <source>New Replacement</source>
       <translation>Nieuwe vervanging</translation>
     </message>
     <message>
-      <location filename="../AdvancedWidget.py" line="127"/>
+      <location filename="../AdvancedWidget.py" line="135"/>
       <source>Please enter a ID</source>
       <translation>Voer een id in</translation>
     </message>
     <message>
-      <location filename="../AdvancedWidget.py" line="141"/>
+      <location filename="../AdvancedWidget.py" line="149"/>
       <source>Edit Replacement</source>
       <translation>Vervanging bewerken</translation>
     </message>
     <message>
       <location filename="../ui/AdvancedWidget.ui" line="0"/>
       <source>Translation</source>
       <translation>Vertalingen</translation>
@@ -180,14 +180,36 @@
       <location filename="../ui/AdvancedWidget.ui" line="0"/>
       <location filename="../ui/AdvancedWidget.ui" line="0"/>
       <source>Value</source>
       <translation>Waarde</translation>
     </message>
     <message>
       <location filename="../ui/AdvancedWidget.ui" line="0"/>
+      <source>Branding</source>
+      <translation>Merkmarketing</translation>
+    </message>
+    <message>
+      <location filename="../ui/AdvancedWidget.ui" line="0"/>
+      <source>Set branding colors</source>
+      <translation>Merkkleuren instellen</translation>
+    </message>
+    <message>
+      <location filename="../ui/AdvancedWidget.ui" line="0"/>
+      <source>Light:</source>
+      <extracomment>Theme</extracomment>
+      <translation>Licht:</translation>
+    </message>
+    <message>
+      <location filename="../ui/AdvancedWidget.ui" line="0"/>
+      <source>Dark:</source>
+      <extracomment>Theme</extracomment>
+      <translation>Donker:</translation>
+    </message>
+    <message>
+      <location filename="../ui/AdvancedWidget.ui" line="0"/>
       <source>Custom</source>
       <translation>Aangepast</translation>
     </message>
     <message>
       <location filename="../ui/AdvancedWidget.ui" line="0"/>
       <source>You can add custom values here. For more information take a look at the documentation.</source>
       <translation>Hier kunt u aangepaste waarden toevoegen. Bekijk voor meer informatie de documentatie.</translation>
@@ -840,25 +862,30 @@
       <translation>Duits</translation>
     </message>
     <message>
       <location filename="../Languages.py" line="8"/>
       <source>Dutch</source>
       <translation>Nederlands</translation>
     </message>
+    <message>
+      <location filename="../Languages.py" line="9"/>
+      <source>Russian</source>
+      <translation>Russisch</translation>
+    </message>
   </context>
   <context>
     <name>MainWindow</name>
     <message>
-      <location filename="../MainWindow.py" line="456"/>
+      <location filename="../MainWindow.py" line="459"/>
       <location filename="../ExternalReleasesWindow.py" line="224"/>
       <source>No Plugins installed</source>
       <translation>Er zijn plug-ins geïnstalleerd</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="456"/>
+      <location filename="../MainWindow.py" line="459"/>
       <location filename="../ExternalReleasesWindow.py" line="224"/>
       <source>You have no Plugins installed</source>
       <translation>U heeft geen plug-ins geïnstalleerd</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="83"/>
       <source>Not specified</source>
@@ -931,305 +958,305 @@
     </message>
     <message>
       <location filename="../MainWindow.py" line="129"/>
       <source>Unknown</source>
       <translation>Onbekend</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="226"/>
+      <location filename="../MainWindow.py" line="229"/>
       <source>Untitled</source>
       <translation>Naamloos</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="772"/>
-      <location filename="../MainWindow.py" line="748"/>
-      <location filename="../MainWindow.py" line="232"/>
+      <location filename="../MainWindow.py" line="775"/>
+      <location filename="../MainWindow.py" line="751"/>
+      <location filename="../MainWindow.py" line="235"/>
       <source>Error</source>
       <translation>Foutmelding</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="243"/>
+      <location filename="../MainWindow.py" line="246"/>
       <source>No templates found</source>
       <translation>Er zijn geen sjablonen aangetroffen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="257"/>
+      <location filename="../MainWindow.py" line="260"/>
       <source>No recent files</source>
       <translation>Er zijn geen onlangs geopende bestanden</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="270"/>
+      <location filename="../MainWindow.py" line="273"/>
       <source>Clear</source>
       <translation>Wissen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="287"/>
+      <location filename="../MainWindow.py" line="290"/>
       <source>Unsaved changes</source>
       <translation>Niet-opgeslagen wijzigingen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="287"/>
+      <location filename="../MainWindow.py" line="290"/>
       <source>You have unsaved changes. Do you want to save now?</source>
       <translation>U heeft niet-opgeslagen wijzigingen. Wilt u deze nu opslaan?</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="298"/>
+      <location filename="../MainWindow.py" line="301"/>
       <source>Welcome to jdAppStreamEdit!</source>
       <translation>Welkom in jdAppStreamEdit!</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="299"/>
+      <location filename="../MainWindow.py" line="302"/>
       <source>With jdAppStreamEdit you can create and edit AppStream files (*.metainfo.xml or .appdata.xml). This files are to provide data for your Application (Description, Screenshots etc.) to Software Centers.</source>
       <translation>Met jdAppStreamEdit kunt u AppStream-bestanden (*.metainfo.xml of .appdata.xml) maken en bewerken. Deze bestanden bieden gegevens voor uw programma (omschrijving, schermfoto's, etc.) voor gebruik in softwarecentra.</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="300"/>
+      <location filename="../MainWindow.py" line="303"/>
       <source>It is highly recommend to read the the AppStream Documentation before using this Program. You can open it under ?&gt;AppStream documentation.</source>
       <translation>Wij raden ten zeerste aan de AppStream-documentatie door te nemen alvorens dit programma te gebruiken, te openen via ? → AppStream-documentatie.</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="301"/>
+      <location filename="../MainWindow.py" line="304"/>
       <source>You can check if your AppStream is valid under Tools&gt;Validate.</source>
       <translation>U kunt uw AppStream-bestand valideren via Hulpmiddelen → Valideren.</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="304"/>
+      <location filename="../MainWindow.py" line="307"/>
       <source>Show this dialog at startup</source>
       <translation>Venster tonen na elke opstart</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="308"/>
+      <location filename="../MainWindow.py" line="311"/>
       <source>Welcome</source>
       <translation>Welkom</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="329"/>
+      <location filename="../MainWindow.py" line="332"/>
       <source>desktop-entry-lib not found</source>
       <translation>desktop-entry-lib niet aangetroffen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="329"/>
+      <location filename="../MainWindow.py" line="332"/>
       <source>This function needs the desktop-entry-lib python module to work</source>
       <translation>Deze functie vereist de desktop-entry-lib Python-module</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="337"/>
+      <location filename="../MainWindow.py" line="340"/>
       <source>Desktop Entry Files</source>
       <translation>Desktopitembestanden</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="433"/>
-      <location filename="../MainWindow.py" line="395"/>
-      <location filename="../MainWindow.py" line="337"/>
+      <location filename="../MainWindow.py" line="436"/>
+      <location filename="../MainWindow.py" line="398"/>
+      <location filename="../MainWindow.py" line="340"/>
       <source>All Files</source>
       <translation>Alle bestanden</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="345"/>
+      <location filename="../MainWindow.py" line="348"/>
       <source>Could not read file</source>
       <translation>Het bestand kan niet worden ingelezen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="345"/>
+      <location filename="../MainWindow.py" line="348"/>
       <source>Could not read {{path}}. Make sure it is a valid desktop entry and you have the Permission to read it.</source>
       <translation>{{path}} kan niet worden ingelezen. Zorg er voor dat het een geldig .desktop-bestand is en dat u over de juiste rechten beschikt.</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="433"/>
-      <location filename="../MainWindow.py" line="395"/>
+      <location filename="../MainWindow.py" line="436"/>
+      <location filename="../MainWindow.py" line="398"/>
       <source>AppStream Files</source>
       <translation>AppStream-bestanden</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="417"/>
+      <location filename="../MainWindow.py" line="420"/>
       <source>Enter URL</source>
       <translation>Voer een url in</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="417"/>
+      <location filename="../MainWindow.py" line="420"/>
       <source>Please enter a URL</source>
       <translation>Voer een url in</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
-      <location filename="../MainWindow.py" line="485"/>
+      <location filename="../MainWindow.py" line="488"/>
       <source>Edit</source>
       <translation>Bewerken</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
-      <location filename="../MainWindow.py" line="646"/>
-      <location filename="../MainWindow.py" line="609"/>
-      <location filename="../MainWindow.py" line="489"/>
+      <location filename="../MainWindow.py" line="649"/>
+      <location filename="../MainWindow.py" line="612"/>
+      <location filename="../MainWindow.py" line="492"/>
       <source>Remove</source>
       <translation>Verwijderen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="763"/>
-      <location filename="../MainWindow.py" line="557"/>
-      <location filename="../MainWindow.py" line="497"/>
+      <location filename="../MainWindow.py" line="766"/>
+      <location filename="../MainWindow.py" line="560"/>
+      <location filename="../MainWindow.py" line="500"/>
       <source>Invalid URL</source>
       <translation>Ongeldige url</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="497"/>
+      <location filename="../MainWindow.py" line="500"/>
       <source>The URL {{url}} does not work</source>
       <translation>{{url}} werkt niet</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="559"/>
-      <location filename="../MainWindow.py" line="499"/>
+      <location filename="../MainWindow.py" line="562"/>
+      <location filename="../MainWindow.py" line="502"/>
       <source>Everything OK</source>
       <translation>Alles werkt</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="559"/>
-      <location filename="../MainWindow.py" line="499"/>
+      <location filename="../MainWindow.py" line="562"/>
+      <location filename="../MainWindow.py" line="502"/>
       <source>All URLs are working</source>
       <translation>Alle url's werken</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="557"/>
+      <location filename="../MainWindow.py" line="560"/>
       <source>The URL {url} does not work</source>
       <translation>De url, {url}, werkt niet</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="570"/>
+      <location filename="../MainWindow.py" line="573"/>
       <source>Add a Categorie</source>
       <translation>Categorie toevoegen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="570"/>
+      <location filename="../MainWindow.py" line="573"/>
       <source>Please select a Categorie from the list below</source>
       <translation>Kies een categorie van onderstaande lijst</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="574"/>
+      <location filename="../MainWindow.py" line="577"/>
       <source>Categorie already added</source>
       <translation>Categorie is al toegevoegd</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="574"/>
+      <location filename="../MainWindow.py" line="577"/>
       <source>You can't add the same Categorie twice</source>
       <translation>U kunt niet tweemaal dezelfde categorie kiezen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="662"/>
+      <location filename="../MainWindow.py" line="665"/>
       <source>New Keyword</source>
       <translation>Nieuw trefwoord</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="662"/>
+      <location filename="../MainWindow.py" line="665"/>
       <source>Please enter a new Keyword</source>
       <translation>Voer een nieuw trefwoord in</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="682"/>
-      <location filename="../MainWindow.py" line="666"/>
+      <location filename="../MainWindow.py" line="685"/>
+      <location filename="../MainWindow.py" line="669"/>
       <source>Keyword in List</source>
       <translation>Bestaand trefwoord</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="682"/>
-      <location filename="../MainWindow.py" line="666"/>
+      <location filename="../MainWindow.py" line="685"/>
+      <location filename="../MainWindow.py" line="669"/>
       <source>This Keyword is already in the List</source>
       <translation>Dit trefwoord is al toegevoegd</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="676"/>
+      <location filename="../MainWindow.py" line="679"/>
       <source>Edit Keyword</source>
       <translation>Trefwoord bewerken</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="676"/>
+      <location filename="../MainWindow.py" line="679"/>
       <source>Please edit the Keyword</source>
       <translation>Bewerk het trefwoord</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="745"/>
+      <location filename="../MainWindow.py" line="748"/>
       <source>File not found</source>
       <translation>Bestand niet aangetroffen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="745"/>
+      <location filename="../MainWindow.py" line="748"/>
       <source>{{path}} does not exists</source>
       <translation>{{path}} bestaat niet</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="748"/>
+      <location filename="../MainWindow.py" line="751"/>
       <source>An error occurred while trying to open {{path}}</source>
       <translation>Er is een fout opgetreden tijdens het openen van {{path}}</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="763"/>
+      <location filename="../MainWindow.py" line="766"/>
       <source>{{url}} is not a valid http/https URL</source>
       <translation>{{url}} is geen geldige http-/https-url</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="769"/>
+      <location filename="../MainWindow.py" line="772"/>
       <source>Could not connect</source>
       <translation>Kan geen verbinding maken</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="769"/>
+      <location filename="../MainWindow.py" line="772"/>
       <source>Could not connect to {{url}}</source>
       <translation>Er kan geen verbinding worden gemaakt met {{url}}</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="772"/>
+      <location filename="../MainWindow.py" line="775"/>
       <source>An error occurred while trying to connect to {{url}}</source>
       <translation>Er is een fout opgetreden tijdens het openen van {{url}}</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="833"/>
+      <location filename="../MainWindow.py" line="836"/>
       <source>XML parsing failed</source>
       <translation>Xml-verwerking mislukt</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="837"/>
+      <location filename="../MainWindow.py" line="840"/>
       <source>No component tag</source>
       <translation>Geen onderdeeltag</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="837"/>
+      <location filename="../MainWindow.py" line="840"/>
       <source>This XML file has no component tag</source>
       <translation>Het xml-bestand bevat geen onderdeeltag</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="840"/>
+      <location filename="../MainWindow.py" line="843"/>
       <source>Too many component tags</source>
       <translation>Teveel onderdeeltags</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="840"/>
+      <location filename="../MainWindow.py" line="843"/>
       <source>Only files with one component tag are supported</source>
       <translation>Er is alleen ondersteuning voor bestanden met één onderdeeltag</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="1178"/>
+      <location filename="../MainWindow.py" line="1185"/>
       <source>No ID</source>
       <translation>Geen id</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="1178"/>
+      <location filename="../MainWindow.py" line="1185"/>
       <source>You need to set a ID to use this feature</source>
       <translation>Ken een id toe om deze functie te gebruiken</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="1197"/>
+      <location filename="../MainWindow.py" line="1204"/>
       <source>{{binary}} not found</source>
       <translation>{{binary}} niet aangetroffen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="1197"/>
+      <location filename="../MainWindow.py" line="1204"/>
       <source>{{binary}} was not found. Make sure it is installed and in PATH.</source>
       <translation>{{binary}} is niet aangetroffen. Zorg er voor dat het bestand bestaat en toegevoegd is aan uw PATH.</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>General</source>
       <translation>Algemeen</translation>
```

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/AboutWindow.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/AboutWindow.ui`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/AdvancedWidget.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/AdvancedWidget.ui`

 * *Files 24% similar despite different names*

#### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/AdvancedWidget.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/AdvancedWidget.ui`

```diff
@@ -25,15 +25,15 @@
       </property>
       <property name="bottomMargin">
         <number>0</number>
       </property>
       <item>
         <widget class="QTabWidget" name="tab_widget">
           <property name="currentIndex">
-            <number>2</number>
+            <number>4</number>
           </property>
           <widget class="QWidget" name="translation_tab">
             <attribute name="title">
               <string>Translation</string>
             </attribute>
             <layout class="QVBoxLayout" name="verticalLayout_2">
               <item>
@@ -223,14 +223,73 @@
                   <property name="text">
                     <string>Add</string>
                   </property>
                 </widget>
               </item>
             </layout>
           </widget>
+          <widget class="QWidget" name="tab_2">
+            <attribute name="title">
+              <string>Branding</string>
+            </attribute>
+            <layout class="QVBoxLayout" name="verticalLayout_7">
+              <item>
+                <widget class="QCheckBox" name="branding_colors_check_box">
+                  <property name="text">
+                    <string>Set branding colors</string>
+                  </property>
+                </widget>
+              </item>
+              <item>
+                <layout class="QGridLayout" name="branding_colors_layout">
+                  <item row="0" column="0">
+                    <widget class="QLabel" name="label_6">
+                      <property name="text">
+                        <string extracomment="Theme">Light:</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="0" column="1">
+                    <widget class="QPushButton" name="light_branding_color_button">
+                      <property name="text">
+                        <string notr="true"/>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="1" column="0">
+                    <widget class="QLabel" name="label_7">
+                      <property name="text">
+                        <string extracomment="Theme">Dark:</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="1" column="1">
+                    <widget class="QPushButton" name="dark_branding_color_button">
+                      <property name="text">
+                        <string notr="true"/>
+                      </property>
+                    </widget>
+                  </item>
+                </layout>
+              </item>
+              <item>
+                <spacer name="verticalSpacer">
+                  <property name="orientation">
+                    <enum>Qt::Vertical</enum>
+                  </property>
+                  <property name="sizeHint" stdset="0">
+                    <size>
+                      <width>20</width>
+                      <height>40</height>
+                    </size>
+                  </property>
+                </spacer>
+              </item>
+            </layout>
+          </widget>
           <widget class="QWidget" name="custom_tab">
             <attribute name="title">
               <string>Custom</string>
             </attribute>
             <layout class="QVBoxLayout" name="verticalLayout_5">
               <item>
                 <widget class="QLabel" name="label_4">
```

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/ArtifactWindow.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/ArtifactWindow.ui`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/ComposeDirectoryWindow.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/ComposeDirectoryWindow.ui`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/DescriptionWidget.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/DescriptionWidget.ui`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/ExternalReleasesWindow.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/ExternalReleasesWindow.ui`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/ImportChangelogWindow.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/ImportChangelogWindow.ui`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/MainWindow.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/MainWindow.ui`

 * *Files 3% similar despite different names*

#### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/MainWindow.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/MainWindow.ui`

```diff
@@ -29,30 +29,37 @@
         </property>
         <property name="bottomMargin">
           <number>0</number>
         </property>
         <item>
           <widget class="QTabWidget" name="main_tab_widget">
             <property name="currentIndex">
-              <number>9</number>
+              <number>0</number>
             </property>
             <widget class="QWidget" name="tab">
               <attribute name="title">
                 <string>General</string>
               </attribute>
               <layout class="QFormLayout" name="formLayout">
                 <item row="0" column="0">
                   <widget class="QLabel" name="label_22">
                     <property name="text">
                       <string>Type:</string>
                     </property>
                   </widget>
                 </item>
                 <item row="0" column="1">
-                  <widget class="QComboBox" name="component_type_box"/>
+                  <widget class="QComboBox" name="component_type_box">
+                    <property name="sizePolicy">
+                      <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
+                        <horstretch>0</horstretch>
+                        <verstretch>0</verstretch>
+                      </sizepolicy>
+                    </property>
+                  </widget>
                 </item>
                 <item row="1" column="0">
                   <widget class="QLabel" name="label">
                     <property name="text">
                       <string>ID:</string>
                     </property>
                   </widget>
@@ -169,25 +176,38 @@
                   <widget class="QLabel" name="label_3">
                     <property name="text">
                       <string>Metadata License:</string>
                     </property>
                   </widget>
                 </item>
                 <item row="6" column="1">
-                  <widget class="QComboBox" name="metadata_license_box"/>
+                  <widget class="QComboBox" name="metadata_license_box">
+                    <property name="sizePolicy">
+                      <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
+                        <horstretch>0</horstretch>
+                        <verstretch>0</verstretch>
+                      </sizepolicy>
+                    </property>
+                  </widget>
                 </item>
                 <item row="7" column="0">
                   <widget class="QLabel" name="label_4">
                     <property name="text">
                       <string>Project License:</string>
                     </property>
                   </widget>
                 </item>
                 <item row="7" column="1">
                   <widget class="QComboBox" name="project_license_box">
+                    <property name="sizePolicy">
+                      <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
+                        <horstretch>0</horstretch>
+                        <verstretch>0</verstretch>
+                      </sizepolicy>
+                    </property>
                     <property name="editable">
                       <bool>false</bool>
                     </property>
                   </widget>
                 </item>
                 <item row="8" column="0">
                   <widget class="QLabel" name="label_5">
@@ -259,15 +279,15 @@
               <attribute name="title">
                 <string>Screenshots</string>
               </attribute>
               <layout class="QVBoxLayout" name="verticalLayout">
                 <item>
                   <widget class="QTableWidget" name="screenshot_table">
                     <property name="selectionBehavior">
-                      <enum>QAbstractItemView::SelectRows</enum>
+                      <enum>QAbstractItemView::SelectionBehavior::SelectRows</enum>
                     </property>
                     <property name="rowCount">
                       <number>0</number>
                     </property>
                     <property name="columnCount">
                       <number>4</number>
                     </property>
@@ -327,15 +347,15 @@
                 </item>
                 <item>
                   <widget class="QLabel" name="releases_widget_placeholder">
                     <property name="text">
                       <string notr="true">Releases Widget Placeholder</string>
                     </property>
                     <property name="alignment">
-                      <set>Qt::AlignCenter</set>
+                      <set>Qt::AlignmentFlag::AlignCenter</set>
                     </property>
                   </widget>
                 </item>
                 <item>
                   <widget class="QRadioButton" name="external_releases_radio_button">
                     <property name="text">
                       <string>External</string>
@@ -505,15 +525,15 @@
                       <string>Check URLs</string>
                     </property>
                   </widget>
                 </item>
                 <item>
                   <spacer name="verticalSpacer">
                     <property name="orientation">
-                      <enum>Qt::Vertical</enum>
+                      <enum>Qt::Orientation::Vertical</enum>
                     </property>
                     <property name="sizeHint" stdset="0">
                       <size>
                         <width>20</width>
                         <height>40</height>
                       </size>
                     </property>
@@ -525,15 +545,15 @@
               <attribute name="title">
                 <string>Categories</string>
               </attribute>
               <layout class="QVBoxLayout" name="verticalLayout_4">
                 <item>
                   <widget class="QListWidget" name="categorie_list">
                     <property name="dragDropMode">
-                      <enum>QAbstractItemView::InternalMove</enum>
+                      <enum>QAbstractItemView::DragDropMode::InternalMove</enum>
                     </property>
                   </widget>
                 </item>
                 <item>
                   <layout class="QHBoxLayout" name="horizontalLayout_4">
                     <item>
                       <widget class="QPushButton" name="categorie_add_button">
@@ -731,15 +751,15 @@
                       </layout>
                     </item>
                   </layout>
                 </item>
                 <item>
                   <spacer name="verticalSpacer_2">
                     <property name="orientation">
-                      <enum>Qt::Vertical</enum>
+                      <enum>Qt::Orientation::Vertical</enum>
                     </property>
                     <property name="sizeHint" stdset="0">
                       <size>
                         <width>20</width>
                         <height>40</height>
                       </size>
                     </property>
@@ -795,28 +815,28 @@
               <layout class="QVBoxLayout" name="verticalLayout_2">
                 <item>
                   <widget class="QLabel" name="label_19">
                     <property name="text">
                       <string>Indicates possible methods to launch the software described in this component</string>
                     </property>
                     <property name="alignment">
-                      <set>Qt::AlignCenter</set>
+                      <set>Qt::AlignmentFlag::AlignCenter</set>
                     </property>
                     <property name="wordWrap">
                       <bool>true</bool>
                     </property>
                   </widget>
                 </item>
                 <item>
                   <widget class="QTableWidget" name="launchable_table">
                     <property name="dragDropMode">
-                      <enum>QAbstractItemView::InternalMove</enum>
+                      <enum>QAbstractItemView::DragDropMode::InternalMove</enum>
                     </property>
                     <property name="selectionBehavior">
-                      <enum>QAbstractItemView::SelectRows</enum>
+                      <enum>QAbstractItemView::SelectionBehavior::SelectRows</enum>
                     </property>
                     <column>
                       <property name="text">
                         <string>Type</string>
                       </property>
                     </column>
                     <column>
@@ -847,22 +867,22 @@
               <layout class="QVBoxLayout" name="verticalLayout_6">
                 <item>
                   <widget class="QLabel" name="label_20">
                     <property name="text">
                       <string>This is for advanced users. For more information take a look at the Appstream documentation.</string>
                     </property>
                     <property name="alignment">
-                      <set>Qt::AlignCenter</set>
+                      <set>Qt::AlignmentFlag::AlignCenter</set>
                     </property>
                   </widget>
                 </item>
                 <item>
                   <widget class="QTableWidget" name="provides_table">
                     <property name="selectionBehavior">
-                      <enum>QAbstractItemView::SelectRows</enum>
+                      <enum>QAbstractItemView::SelectionBehavior::SelectRows</enum>
                     </property>
                     <column>
                       <property name="text">
                         <string>Type</string>
                       </property>
                     </column>
                     <column>
@@ -893,22 +913,22 @@
               <layout class="QVBoxLayout" name="verticalLayout_7">
                 <item>
                   <widget class="QLabel" name="label_21">
                     <property name="text">
                       <string>You can manage the Keywords for the Software here</string>
                     </property>
                     <property name="alignment">
-                      <set>Qt::AlignCenter</set>
+                      <set>Qt::AlignmentFlag::AlignCenter</set>
                     </property>
                   </widget>
                 </item>
                 <item>
                   <widget class="QListWidget" name="keyword_list">
                     <property name="dragDropMode">
-                      <enum>QAbstractItemView::InternalMove</enum>
+                      <enum>QAbstractItemView::DragDropMode::InternalMove</enum>
                     </property>
                   </widget>
                 </item>
                 <item>
                   <layout class="QHBoxLayout" name="horizontalLayout_8">
                     <item>
                       <widget class="QPushButton" name="keyword_add_button">
@@ -963,30 +983,30 @@
     </widget>
     <widget class="QMenuBar" name="menubar">
       <property name="geometry">
         <rect>
           <x>0</x>
           <y>0</y>
           <width>944</width>
-          <height>21</height>
+          <height>30</height>
         </rect>
       </property>
       <widget class="QMenu" name="menuFile">
         <property name="title">
-          <string>File</string>
+          <string>Fi&amp;le</string>
         </property>
         <widget class="QMenu" name="recent_files_menu">
           <property name="title">
-            <string>Open recent</string>
+            <string>Open &amp;recent</string>
           </property>
           <addaction name="actionPlaceholder"/>
         </widget>
         <widget class="QMenu" name="new_template_file_menu">
           <property name="title">
-            <string>New (from Template)</string>
+            <string>Ne&amp;w (from Template)</string>
           </property>
           <addaction name="actionPlaceholder_2"/>
         </widget>
         <addaction name="new_action"/>
         <addaction name="new_desktop_file_action"/>
         <addaction name="new_template_file_menu"/>
         <addaction name="separator"/>
@@ -1012,23 +1032,23 @@
         <addaction name="donate_action"/>
         <addaction name="separator"/>
         <addaction name="about_action"/>
         <addaction name="about_qt_action"/>
       </widget>
       <widget class="QMenu" name="menuSettings">
         <property name="title">
-          <string>Settings</string>
+          <string>Setti&amp;ngs</string>
         </property>
         <addaction name="settings_action"/>
         <addaction name="manage_templates_action"/>
         <addaction name="plugins_action"/>
       </widget>
       <widget class="QMenu" name="menuTools">
         <property name="title">
-          <string>Tools</string>
+          <string>&amp;Tools</string>
         </property>
         <addaction name="validate_action"/>
         <addaction name="view_xml_action"/>
         <addaction name="preview_gnome_software"/>
         <addaction name="view_catalog_action"/>
         <addaction name="compose_directory_action"/>
         <addaction name="sysinfo_action"/>
@@ -1036,151 +1056,151 @@
       <addaction name="menuFile"/>
       <addaction name="menuSettings"/>
       <addaction name="menuTools"/>
       <addaction name="menu"/>
     </widget>
     <action name="open_action">
       <property name="text">
-        <string>Open</string>
+        <string>&amp;Open</string>
       </property>
       <property name="shortcut">
         <string notr="true">Ctrl+O</string>
       </property>
     </action>
     <action name="save_action">
       <property name="text">
-        <string>Save</string>
+        <string>&amp;Save</string>
       </property>
       <property name="shortcut">
         <string notr="true">Ctrl+S</string>
       </property>
     </action>
     <action name="save_as_action">
       <property name="text">
-        <string>Save As...</string>
+        <string>Save &amp;As...</string>
       </property>
     </action>
     <action name="about_action">
       <property name="text">
-        <string>About</string>
+        <string>A&amp;bout</string>
       </property>
     </action>
     <action name="about_qt_action">
       <property name="text">
-        <string>About Qt</string>
+        <string>About &amp;Qt</string>
       </property>
     </action>
     <action name="exit_action">
       <property name="text">
-        <string>Exit</string>
+        <string>&amp;Exit</string>
       </property>
       <property name="shortcut">
         <string notr="true">Ctrl+Q</string>
       </property>
     </action>
     <action name="new_action">
       <property name="text">
-        <string>New</string>
+        <string>&amp;New</string>
       </property>
       <property name="shortcut">
         <string notr="true">Ctrl+N</string>
       </property>
     </action>
     <action name="settings_action">
       <property name="text">
-        <string>Settings</string>
+        <string>&amp;Settings</string>
       </property>
     </action>
     <action name="validate_action">
       <property name="text">
-        <string>Validate</string>
+        <string>&amp;Validate</string>
       </property>
     </action>
     <action name="actionPlaceholder">
       <property name="text">
-        <string notr="true">Placeholder</string>
+        <string notr="true">&amp;Placeholder</string>
       </property>
     </action>
     <action name="documentation_action">
       <property name="text">
-        <string>AppStream documentation</string>
+        <string>&amp;AppStream documentation</string>
       </property>
     </action>
     <action name="view_xml_action">
       <property name="text">
-        <string>View XML</string>
+        <string>View &amp;XML</string>
       </property>
     </action>
     <action name="preview_gnome_software">
       <property name="text">
-        <string>Preview in Gnome Software</string>
+        <string>&amp;Preview in Gnome Software</string>
       </property>
     </action>
     <action name="welcome_dialog_action">
       <property name="text">
-        <string>Show welcome dialog</string>
+        <string>&amp;Show welcome dialog</string>
       </property>
     </action>
     <action name="open_url_action">
       <property name="text">
-        <string>Open from URL</string>
+        <string>Open from &amp;URL</string>
       </property>
     </action>
     <action name="new_desktop_file_action">
       <property name="text">
-        <string>New (from .desktop file)</string>
+        <string>New (&amp;from .desktop file)</string>
       </property>
     </action>
     <action name="manage_templates_action">
       <property name="text">
-        <string>Manage templates</string>
+        <string>&amp;Manage templates</string>
       </property>
     </action>
     <action name="actionPlaceholder_2">
       <property name="text">
-        <string notr="true">Placeholder</string>
+        <string notr="true">&amp;Placeholder</string>
       </property>
     </action>
     <action name="view_source_action">
       <property name="text">
-        <string>View Source</string>
+        <string>&amp;View Source</string>
       </property>
     </action>
     <action name="report_bug_action">
       <property name="text">
-        <string>Report Bug</string>
+        <string>&amp;Report Bug</string>
       </property>
     </action>
     <action name="translate_action">
       <property name="text">
-        <string>Translate</string>
+        <string>&amp;Translate</string>
       </property>
     </action>
     <action name="donate_action">
       <property name="text">
-        <string>Donate</string>
+        <string>&amp;Donate</string>
       </property>
     </action>
     <action name="plugins_action">
       <property name="text">
-        <string>Plugins</string>
+        <string>&amp;Plugins</string>
       </property>
     </action>
     <action name="compose_directory_action">
       <property name="text">
-        <string>Compose existing Directory</string>
+        <string>&amp;Compose existing Directory</string>
       </property>
     </action>
     <action name="view_catalog_action">
       <property name="text">
-        <string>View Catalog</string>
+        <string>V&amp;iew Catalog</string>
       </property>
     </action>
     <action name="sysinfo_action">
       <property name="text">
-        <string>Sysinfo</string>
+        <string>&amp;Sysinfo</string>
       </property>
     </action>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/ManageTemplatesWindow.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/ManageTemplatesWindow.ui`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/OarsWidget.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/OarsWidget.ui`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/PluginWindow.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/PluginWindow.ui`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/RelationsWidget.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/RelationsWidget.ui`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/ReleasesWidget.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/ReleasesWidget.ui`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/ReleasesWindow.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/ReleasesWindow.ui`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/ScreenshotWindow.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/ScreenshotWindow.ui`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/SettingsWindow.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/SettingsWindow.ui`

 * *Files 18% similar despite different names*

#### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/SettingsWindow.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/SettingsWindow.ui`

```diff
@@ -3,15 +3,15 @@
   <class>SettingsWindow</class>
   <widget class="QDialog" name="SettingsWindow">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>374</width>
-        <height>527</height>
+        <height>558</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>Settings</string>
     </property>
     <layout class="QVBoxLayout" name="verticalLayout_3">
       <item>
@@ -29,14 +29,20 @@
                     </property>
                   </widget>
                 </item>
                 <item row="0" column="1">
                   <layout class="QHBoxLayout" name="horizontalLayout_4">
                     <item>
                       <widget class="QComboBox" name="language_box">
+                        <property name="sizePolicy">
+                          <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
+                            <horstretch>0</horstretch>
+                            <verstretch>0</verstretch>
+                          </sizepolicy>
+                        </property>
                         <property name="maximumSize">
                           <size>
                             <width>200</width>
                             <height>16777215</height>
                           </size>
                         </property>
                       </widget>
@@ -54,25 +60,39 @@
                   <widget class="QLabel" name="label_3">
                     <property name="text">
                       <string>Length of recent files list:</string>
                     </property>
                   </widget>
                 </item>
                 <item row="1" column="1">
-                  <widget class="QSpinBox" name="recent_files_spin_box"/>
+                  <widget class="QSpinBox" name="recent_files_spin_box">
+                    <property name="sizePolicy">
+                      <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
+                        <horstretch>0</horstretch>
+                        <verstretch>0</verstretch>
+                      </sizepolicy>
+                    </property>
+                  </widget>
                 </item>
                 <item row="2" column="0">
                   <widget class="QLabel" name="label_4">
                     <property name="text">
                       <string>Window title:</string>
                     </property>
                   </widget>
                 </item>
                 <item row="2" column="1">
-                  <widget class="QComboBox" name="window_title_box"/>
+                  <widget class="QComboBox" name="window_title_box">
+                    <property name="sizePolicy">
+                      <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
+                        <horstretch>0</horstretch>
+                        <verstretch>0</verstretch>
+                      </sizepolicy>
+                    </property>
+                  </widget>
                 </item>
               </layout>
             </item>
             <item>
               <widget class="QCheckBox" name="title_edited_check_box">
                 <property name="text">
                   <string>Show in Title if File is edited</string>
@@ -108,15 +128,22 @@
                   <widget class="QLabel" name="whitespace_label">
                     <property name="text">
                       <string>Whitespaces:</string>
                     </property>
                   </widget>
                 </item>
                 <item>
-                  <widget class="QSpinBox" name="whitespace_spin_box"/>
+                  <widget class="QSpinBox" name="whitespace_spin_box">
+                    <property name="sizePolicy">
+                      <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
+                        <horstretch>0</horstretch>
+                        <verstretch>0</verstretch>
+                      </sizepolicy>
+                    </property>
+                  </widget>
                 </item>
               </layout>
             </item>
             <item>
               <widget class="QCheckBox" name="use_tabs_check_box">
                 <property name="text">
                   <string>Use tabs instead of spaces</string>
@@ -145,32 +172,32 @@
                   <string>Sort languages by</string>
                 </property>
               </widget>
             </item>
             <item>
               <widget class="QRadioButton" name="name_language_translate_rad">
                 <property name="text">
-                  <string extracomment="The name of the language">Name</string>
+                  <string extracomment="The name of the language">&amp;Name</string>
                 </property>
               </widget>
             </item>
             <item>
               <widget class="QRadioButton" name="code_language_translate_rad">
                 <property name="text">
-                  <string extracomment="The alpha-2 code of the language">Code</string>
+                  <string extracomment="The alpha-2 code of the language">&amp;Code</string>
                 </property>
               </widget>
             </item>
           </layout>
         </widget>
       </item>
       <item>
         <spacer name="verticalSpacer">
           <property name="orientation">
-            <enum>Qt::Vertical</enum>
+            <enum>Qt::Orientation::Vertical</enum>
           </property>
           <property name="sizeHint" stdset="0">
             <size>
               <width>20</width>
               <height>40</height>
             </size>
           </property>
@@ -184,15 +211,15 @@
                 <string>Reset</string>
               </property>
             </widget>
           </item>
           <item>
             <spacer name="horizontalSpacer">
               <property name="orientation">
-                <enum>Qt::Horizontal</enum>
+                <enum>Qt::Orientation::Horizontal</enum>
               </property>
               <property name="sizeHint" stdset="0">
                 <size>
                   <width>40</width>
                   <height>20</height>
                 </size>
               </property>
```

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/SysinfoWindow.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/SysinfoWindow.ui`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/ThumbnailWindow.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/ThumbnailWindow.ui`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/TranslateWindow.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/TranslateWindow.ui`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/ValidateWindow.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/ValidateWindow.ui`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/ViewCatalogWindow.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/ViewCatalogWindow.ui`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit/ui/ViewXMLWindow.ui` & `jdappstreamedit-9.1/jdAppStreamEdit/ui/ViewXMLWindow.ui`

 * *Files identical despite different names*

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit.egg-info/PKG-INFO` & `jdappstreamedit-9.1/jdAppStreamEdit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdAppStreamEdit
-Version: 9.0
+Version: 9.1
 Summary: A graphical Program to create and edit AppStream files
 Author-email: JakobDev <jakobdev@gmx.de>
 License: GPL-3
 Project-URL: Source, https://codeberg.org/JakobDev/jdAppStreamEdit
 Project-URL: Issues, https://codeberg.org/JakobDev/jdAppStreamEdit/issues
 Project-URL: Translate, https://translate.codeberg.org/projects/jdAppStreamEdit
 Project-URL: Donation, https://ko-fi.com/jakobdev
```

### Comparing `jdAppStreamEdit-9.0/jdAppStreamEdit.egg-info/SOURCES.txt` & `jdappstreamedit-9.1/jdAppStreamEdit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 jdAppStreamEdit/data/language_codes.csv
 jdAppStreamEdit/data/metadata_licenses.json
 jdAppStreamEdit/data/platform.json
 jdAppStreamEdit/data/project_licenses.json
 jdAppStreamEdit/data/translators.json
 jdAppStreamEdit/translations/jdAppStreamEdit_de.ts
 jdAppStreamEdit/translations/jdAppStreamEdit_nl.ts
+jdAppStreamEdit/translations/jdAppStreamEdit_ru.ts
 jdAppStreamEdit/ui/AboutWindow.ui
 jdAppStreamEdit/ui/AdvancedWidget.ui
 jdAppStreamEdit/ui/ArtifactWindow.ui
 jdAppStreamEdit/ui/ComposeDirectoryWindow.ui
 jdAppStreamEdit/ui/DescriptionWidget.ui
 jdAppStreamEdit/ui/ExternalReleasesWindow.ui
 jdAppStreamEdit/ui/ImportChangelogWindow.ui
```

### Comparing `jdAppStreamEdit-9.0/pyproject.toml` & `jdappstreamedit-9.1/pyproject.toml`

 * *Files identical despite different names*

