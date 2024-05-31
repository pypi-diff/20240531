# Comparing `tmp/fundamentals-2.6.4.tar.gz` & `tmp/fundamentals-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fundamentals-2.6.4.tar", last modified: Mon Apr 15 14:39:51 2024, max compression
+gzip compressed data, was "fundamentals-2.7.0.tar", last modified: Fri May 31 13:35:38 2024, max compression
```

## Comparing `fundamentals-2.6.4.tar` & `fundamentals-2.7.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-04-15 14:39:51.170292 fundamentals-2.6.4/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      412 2024-04-15 14:33:03.000000 fundamentals-2.6.4/.readthedocs.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4282 2024-04-15 14:33:03.000000 fundamentals-2.6.4/CHANGES.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2024-04-15 14:33:03.000000 fundamentals-2.6.4/LICENSE
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      363 2024-04-15 14:33:03.000000 fundamentals-2.6.4/MANIFEST.in
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3599 2024-04-15 14:39:51.170292 fundamentals-2.6.4/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2654 2024-04-15 14:33:03.000000 fundamentals-2.6.4/README.md
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-04-15 14:39:51.158292 fundamentals-2.6.4/fundamentals/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      351 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/__version__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3944 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/cl_utils.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-04-15 14:39:51.162292 fundamentals-2.6.4/fundamentals/commonutils/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      106 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/commonutils/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      375 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/commonutils/getpackagepath.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5696 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/daemonise.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-04-15 14:39:51.162292 fundamentals-2.6.4/fundamentals/download/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      477 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/download/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1192 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/download/_dump_files_to_local_drive.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1767 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/download/_fetch.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1564 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/download/append_now_datestamp_to_filename.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1369 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/download/extract_filename_from_url.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      997 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/download/get_now_datetime_filestamp.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6824 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/download/multiobject_download.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-04-15 14:39:51.166292 fundamentals-2.6.4/fundamentals/files/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      306 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/files/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1765 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/files/fileChunker.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2121 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/files/list_of_dictionaries_to_mysql_inserts.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2929 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/files/recursive_directory_listing.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6445 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/files/tag.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3087 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/fmultiprocess.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    11610 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/logs.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-04-15 14:39:51.166292 fundamentals-2.6.4/fundamentals/mysql/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      742 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/mysql/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    21529 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/mysql/convert_dictionary_to_mysql_table.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5579 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/mysql/database.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    13993 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/mysql/directory_script_runner.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1584 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/mysql/get_database_table_column_names.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    13281 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/mysql/insert_list_of_dictionaries_into_database_tables.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2801 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/mysql/readquery.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2460 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/mysql/setup_database_connection.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10966 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/mysql/sqlite2mysql.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1406 2024-04-15 14:33:03.000000 fundamentals-2.6.4/fundamentals/mysql/table_exists.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     7416 2024-04-15 14:33:04.000000 fundamentals-2.6.4/fundamentals/mysql/writequery.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9717 2024-04-15 14:33:04.000000 fundamentals-2.6.4/fundamentals/mysql/yaml_to_database.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-04-15 14:39:51.166292 fundamentals-2.6.4/fundamentals/nose2_plugins/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       41 2024-04-15 14:33:04.000000 fundamentals-2.6.4/fundamentals/nose2_plugins/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1384 2024-04-15 14:33:04.000000 fundamentals-2.6.4/fundamentals/nose2_plugins/cprof.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-04-15 14:39:51.170292 fundamentals-2.6.4/fundamentals/renderer/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      162 2024-04-15 14:33:04.000000 fundamentals-2.6.4/fundamentals/renderer/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    20625 2024-04-15 14:33:04.000000 fundamentals-2.6.4/fundamentals/renderer/list_of_dictionaries.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-04-15 14:39:51.170292 fundamentals-2.6.4/fundamentals/stats/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      109 2024-04-15 14:33:04.000000 fundamentals-2.6.4/fundamentals/stats/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2854 2024-04-15 14:33:04.000000 fundamentals-2.6.4/fundamentals/stats/rolling_window_sigma_clip.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3137 2024-04-15 14:33:04.000000 fundamentals-2.6.4/fundamentals/times.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    24029 2024-04-15 14:33:04.000000 fundamentals-2.6.4/fundamentals/tools.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5328 2024-04-15 14:33:04.000000 fundamentals-2.6.4/fundamentals/utKit.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-04-15 14:39:51.162292 fundamentals-2.6.4/fundamentals.egg-info/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3599 2024-04-15 14:39:51.000000 fundamentals-2.6.4/fundamentals.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1902 2024-04-15 14:39:51.000000 fundamentals-2.6.4/fundamentals.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2024-04-15 14:39:51.000000 fundamentals-2.6.4/fundamentals.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      183 2024-04-15 14:39:51.000000 fundamentals-2.6.4/fundamentals.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2024-04-15 14:36:44.000000 fundamentals-2.6.4/fundamentals.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       80 2024-04-15 14:39:51.000000 fundamentals-2.6.4/fundamentals.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       13 2024-04-15 14:39:51.000000 fundamentals-2.6.4/fundamentals.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       79 2024-04-15 14:39:51.170292 fundamentals-2.6.4/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2232 2024-04-15 14:33:04.000000 fundamentals-2.6.4/setup.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-05-31 13:35:38.555157 fundamentals-2.7.0/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      412 2024-05-31 13:26:54.000000 fundamentals-2.7.0/.readthedocs.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4363 2024-05-31 13:26:54.000000 fundamentals-2.7.0/CHANGES.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2024-05-31 13:26:54.000000 fundamentals-2.7.0/LICENSE
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      363 2024-05-31 13:26:54.000000 fundamentals-2.7.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3599 2024-05-31 13:35:38.555157 fundamentals-2.7.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2654 2024-05-31 13:26:54.000000 fundamentals-2.7.0/README.md
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-05-31 13:35:38.507155 fundamentals-2.7.0/fundamentals/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      351 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/__version__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3944 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/cl_utils.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-05-31 13:35:38.511155 fundamentals-2.7.0/fundamentals/commonutils/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      106 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/commonutils/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      375 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/commonutils/getpackagepath.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5696 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/daemonise.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-05-31 13:35:38.511155 fundamentals-2.7.0/fundamentals/download/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      477 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/download/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1192 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/download/_dump_files_to_local_drive.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1767 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/download/_fetch.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1564 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/download/append_now_datestamp_to_filename.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1369 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/download/extract_filename_from_url.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      997 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/download/get_now_datetime_filestamp.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6824 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/download/multiobject_download.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-05-31 13:35:38.539156 fundamentals-2.7.0/fundamentals/files/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      306 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/files/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1765 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/files/fileChunker.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2121 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/files/list_of_dictionaries_to_mysql_inserts.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2929 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/files/recursive_directory_listing.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6445 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/files/tag.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5445 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/fmultiprocess.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    11651 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/logs.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-05-31 13:35:38.551156 fundamentals-2.7.0/fundamentals/mysql/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      742 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/mysql/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    21529 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/mysql/convert_dictionary_to_mysql_table.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5579 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/mysql/database.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    13993 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/mysql/directory_script_runner.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1584 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/mysql/get_database_table_column_names.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    13281 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/mysql/insert_list_of_dictionaries_into_database_tables.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2801 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/mysql/readquery.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2460 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/mysql/setup_database_connection.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10966 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/mysql/sqlite2mysql.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1406 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/mysql/table_exists.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     7416 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/mysql/writequery.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9717 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/mysql/yaml_to_database.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-05-31 13:35:38.551156 fundamentals-2.7.0/fundamentals/nose2_plugins/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       41 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/nose2_plugins/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1384 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/nose2_plugins/cprof.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-05-31 13:35:38.555157 fundamentals-2.7.0/fundamentals/renderer/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      162 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/renderer/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    20625 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/renderer/list_of_dictionaries.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-05-31 13:35:38.555157 fundamentals-2.7.0/fundamentals/stats/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      109 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/stats/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2854 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/stats/rolling_window_sigma_clip.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3137 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/times.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    24029 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/tools.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5328 2024-05-31 13:26:54.000000 fundamentals-2.7.0/fundamentals/utKit.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-05-31 13:35:38.555157 fundamentals-2.7.0/fundamentals.egg-info/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3599 2024-05-31 13:35:38.000000 fundamentals-2.7.0/fundamentals.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1902 2024-05-31 13:35:38.000000 fundamentals-2.7.0/fundamentals.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2024-05-31 13:35:38.000000 fundamentals-2.7.0/fundamentals.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      183 2024-05-31 13:35:38.000000 fundamentals-2.7.0/fundamentals.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2024-05-31 13:32:37.000000 fundamentals-2.7.0/fundamentals.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       80 2024-05-31 13:35:38.000000 fundamentals-2.7.0/fundamentals.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       13 2024-05-31 13:35:38.000000 fundamentals-2.7.0/fundamentals.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       79 2024-05-31 13:35:38.555157 fundamentals-2.7.0/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2232 2024-05-31 13:26:54.000000 fundamentals-2.7.0/setup.py
```

### Comparing `fundamentals-2.6.4/CHANGES.md` & `fundamentals-2.7.0/CHANGES.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 
 ## Release Notes
 
+**v2.7.0 - May 31, 2024**
+
+* **FEATURE:** progress bar added to multiprocessing
+
 **v2.6.3 - April 6, 2024**
 
 * **FIXED** fixing 'insert_list_of_dictionaries_into_database_tables' for MySQL 8
 
 **v2.6.2 - January 19, 2024**
 
 * **FIXED** bug fix in collecting settings files from the default location
```

### Comparing `fundamentals-2.6.4/LICENSE` & `fundamentals-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/PKG-INFO` & `fundamentals-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fundamentals
-Version: 2.6.4
+Version: 2.7.0
 Summary: Some fundamental tools required by most self-respecting python-packages bundled in one place. Very opinionated project setup tools including logging, plain-text settings files and database connections.
 Home-page: https://github.com/thespacedoctor/fundamentals
-Download-URL: https://github.com/thespacedoctor/fundamentals/archive/v2.6.4.zip
+Download-URL: https://github.com/thespacedoctor/fundamentals/archive/v2.7.0.zip
 Author: David Young
 Author-email: davidrobertyoung@gmail.com
 License: MIT
 Keywords: logging, database
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `fundamentals-2.6.4/README.md` & `fundamentals-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/cl_utils.py` & `fundamentals-2.7.0/fundamentals/cl_utils.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/daemonise.py` & `fundamentals-2.7.0/fundamentals/daemonise.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/download/_dump_files_to_local_drive.py` & `fundamentals-2.7.0/fundamentals/download/_dump_files_to_local_drive.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/download/_fetch.py` & `fundamentals-2.7.0/fundamentals/download/_fetch.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/download/append_now_datestamp_to_filename.py` & `fundamentals-2.7.0/fundamentals/download/append_now_datestamp_to_filename.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/download/extract_filename_from_url.py` & `fundamentals-2.7.0/fundamentals/download/extract_filename_from_url.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/download/get_now_datetime_filestamp.py` & `fundamentals-2.7.0/fundamentals/download/get_now_datetime_filestamp.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/download/multiobject_download.py` & `fundamentals-2.7.0/fundamentals/download/multiobject_download.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/files/fileChunker.py` & `fundamentals-2.7.0/fundamentals/files/fileChunker.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/files/list_of_dictionaries_to_mysql_inserts.py` & `fundamentals-2.7.0/fundamentals/files/list_of_dictionaries_to_mysql_inserts.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/files/recursive_directory_listing.py` & `fundamentals-2.7.0/fundamentals/files/recursive_directory_listing.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/files/tag.py` & `fundamentals-2.7.0/fundamentals/files/tag.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/logs.py` & `fundamentals-2.7.0/fundamentals/logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -353,7 +353,10 @@
         pass
 
     def critical(self, argu):
         pass
 
     def warning(self, argu):
         pass
+
+    def print(self, argu):
+        pass
```

### Comparing `fundamentals-2.6.4/fundamentals/mysql/__init__.py` & `fundamentals-2.7.0/fundamentals/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/mysql/convert_dictionary_to_mysql_table.py` & `fundamentals-2.7.0/fundamentals/mysql/convert_dictionary_to_mysql_table.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/mysql/database.py` & `fundamentals-2.7.0/fundamentals/mysql/database.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/mysql/directory_script_runner.py` & `fundamentals-2.7.0/fundamentals/mysql/directory_script_runner.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/mysql/get_database_table_column_names.py` & `fundamentals-2.7.0/fundamentals/mysql/get_database_table_column_names.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/mysql/insert_list_of_dictionaries_into_database_tables.py` & `fundamentals-2.7.0/fundamentals/mysql/insert_list_of_dictionaries_into_database_tables.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/mysql/readquery.py` & `fundamentals-2.7.0/fundamentals/mysql/readquery.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/mysql/setup_database_connection.py` & `fundamentals-2.7.0/fundamentals/mysql/setup_database_connection.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/mysql/sqlite2mysql.py` & `fundamentals-2.7.0/fundamentals/mysql/sqlite2mysql.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/mysql/table_exists.py` & `fundamentals-2.7.0/fundamentals/mysql/table_exists.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/mysql/writequery.py` & `fundamentals-2.7.0/fundamentals/mysql/writequery.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/mysql/yaml_to_database.py` & `fundamentals-2.7.0/fundamentals/mysql/yaml_to_database.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/nose2_plugins/cprof.py` & `fundamentals-2.7.0/fundamentals/nose2_plugins/cprof.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/renderer/list_of_dictionaries.py` & `fundamentals-2.7.0/fundamentals/renderer/list_of_dictionaries.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/stats/rolling_window_sigma_clip.py` & `fundamentals-2.7.0/fundamentals/stats/rolling_window_sigma_clip.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/times.py` & `fundamentals-2.7.0/fundamentals/times.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/tools.py` & `fundamentals-2.7.0/fundamentals/tools.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals/utKit.py` & `fundamentals-2.7.0/fundamentals/utKit.py`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/fundamentals.egg-info/PKG-INFO` & `fundamentals-2.7.0/fundamentals.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fundamentals
-Version: 2.6.4
+Version: 2.7.0
 Summary: Some fundamental tools required by most self-respecting python-packages bundled in one place. Very opinionated project setup tools including logging, plain-text settings files and database connections.
 Home-page: https://github.com/thespacedoctor/fundamentals
-Download-URL: https://github.com/thespacedoctor/fundamentals/archive/v2.6.4.zip
+Download-URL: https://github.com/thespacedoctor/fundamentals/archive/v2.7.0.zip
 Author: David Young
 Author-email: davidrobertyoung@gmail.com
 License: MIT
 Keywords: logging, database
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `fundamentals-2.6.4/fundamentals.egg-info/SOURCES.txt` & `fundamentals-2.7.0/fundamentals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fundamentals-2.6.4/setup.py` & `fundamentals-2.7.0/setup.py`

 * *Files identical despite different names*

