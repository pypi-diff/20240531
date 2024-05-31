# Comparing `tmp/zcatalyst_sdk-1.0.0rc2.tar.gz` & `tmp/zcatalyst_sdk-1.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zcatalyst_sdk-1.0.0rc2.tar", last modified: Thu Nov 16 05:53:39 2023, max compression
+gzip compressed data, was "zcatalyst_sdk-1.0.0rc3.tar", last modified: Thu May 30 13:55:16 2024, max compression
```

## Comparing `zcatalyst_sdk-1.0.0rc2.tar` & `zcatalyst_sdk-1.0.0rc3.tar`

### file list

```diff
@@ -1,55 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 05:53:39.666728 zcatalyst_sdk-1.0.0rc2/
--rw-rw-r--   0 root         (0) root         (0)      639 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       98 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2150 2023-11-16 05:53:39.666728 zcatalyst_sdk-1.0.0rc2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1441 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-16 05:53:39.666728 zcatalyst_sdk-1.0.0rc2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1129 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 05:53:39.663728 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/
--rw-rw-r--   0 root         (0) root         (0)     6317 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       57 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/__version__.py
--rw-rw-r--   0 root         (0) root         (0)     3747 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/_constants.py
--rw-rw-r--   0 root         (0) root         (0)     7957 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/_http_client.py
--rw-rw-r--   0 root         (0) root         (0)      708 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/_thread_util.py
--rw-rw-r--   0 root         (0) root         (0)      463 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/_util.py
--rw-rw-r--   0 root         (0) root         (0)     8092 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/authentication.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 05:53:39.664728 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/cache/
--rw-rw-r--   0 root         (0) root         (0)     1675 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/cache/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3589 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/cache/_segment.py
--rw-rw-r--   0 root         (0) root         (0)     6578 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/catalyst_app.py
--rw-rw-r--   0 root         (0) root         (0)     2183 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/circuit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 05:53:39.664728 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/connection/
--rw-rw-r--   0 root         (0) root         (0)     2397 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/connection/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4091 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/connection/_connector.py
--rw-rw-r--   0 root         (0) root         (0)    11824 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/credentials.py
--rw-rw-r--   0 root         (0) root         (0)     3313 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/cron.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 05:53:39.665728 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/datastore/
--rw-rw-r--   0 root         (0) root         (0)     1599 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/datastore/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3092 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/datastore/_bulk_job.py
--rw-rw-r--   0 root         (0) root         (0)     5552 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/datastore/_table.py
--rw-rw-r--   0 root         (0) root         (0)     2611 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/email.py
--rw-rw-r--   0 root         (0) root         (0)     3686 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 05:53:39.665728 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/filestore/
--rw-rw-r--   0 root         (0) root         (0)     2001 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/filestore/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4544 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/filestore/_folder.py
--rw-rw-r--   0 root         (0) root         (0)     1140 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 05:53:39.665728 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/push_notification/
--rw-rw-r--   0 root         (0) root         (0)      794 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/push_notification/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1280 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/push_notification/_mobile_notification.py
--rw-rw-r--   0 root         (0) root         (0)     1035 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/push_notification/_web_notificaton.py
--rw-rw-r--   0 root         (0) root         (0)     1193 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/quick_ml.py
--rw-rw-r--   0 root         (0) root         (0)     1203 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/search.py
--rw-rw-r--   0 root         (0) root         (0)     5946 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/smart_browz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 05:53:39.666728 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/types/
--rw-rw-r--   0 root         (0) root         (0)     7441 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/types/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2782 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/types/smart_browz.py
--rw-rw-r--   0 root         (0) root         (0)     2999 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/types/zia.py
--rw-rw-r--   0 root         (0) root         (0)     9919 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/validator.py
--rw-rw-r--   0 root         (0) root         (0)     1235 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/zcql.py
--rw-rw-r--   0 root         (0) root         (0)     8247 2023-11-16 05:45:21.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/zia.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 05:53:39.664728 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2150 2023-11-16 05:53:39.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1317 2023-11-16 05:53:39.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-16 05:53:39.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-11-16 05:53:39.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-11-16 05:53:39.000000 zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:55:16.761133 zcatalyst_sdk-1.0.0rc3/
+-rw-rw-r--   0 root         (0) root         (0)      639 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       98 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2150 2024-05-30 13:55:16.760133 zcatalyst_sdk-1.0.0rc3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1441 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 13:55:16.761133 zcatalyst_sdk-1.0.0rc3/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1129 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:55:16.754133 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/
+-rw-rw-r--   0 root         (0) root         (0)     6317 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       57 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/__version__.py
+-rw-rw-r--   0 root         (0) root         (0)     3725 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/_constants.py
+-rw-rw-r--   0 root         (0) root         (0)     7957 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/_http_client.py
+-rw-rw-r--   0 root         (0) root         (0)      708 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/_thread_util.py
+-rw-rw-r--   0 root         (0) root         (0)      463 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/_util.py
+-rw-rw-r--   0 root         (0) root         (0)     8092 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/authentication.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:55:16.755133 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/cache/
+-rw-rw-r--   0 root         (0) root         (0)     1675 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/cache/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3589 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/cache/_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     6687 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/catalyst_app.py
+-rw-rw-r--   0 root         (0) root         (0)     2183 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/circuit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:55:16.756133 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/connection/
+-rw-rw-r--   0 root         (0) root         (0)     2397 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/connection/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4091 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/connection/_connector.py
+-rw-rw-r--   0 root         (0) root         (0)    11824 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/credentials.py
+-rw-rw-r--   0 root         (0) root         (0)     3313 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/cron.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:55:16.757133 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/datastore/
+-rw-rw-r--   0 root         (0) root         (0)     1599 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/datastore/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3092 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/datastore/_bulk_job.py
+-rw-rw-r--   0 root         (0) root         (0)     5552 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/datastore/_table.py
+-rw-rw-r--   0 root         (0) root         (0)     2611 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/email.py
+-rw-rw-r--   0 root         (0) root         (0)     3838 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:55:16.757133 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/filestore/
+-rw-rw-r--   0 root         (0) root         (0)     2001 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/filestore/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4544 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/filestore/_folder.py
+-rw-rw-r--   0 root         (0) root         (0)     1140 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:55:16.758133 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/nosql/
+-rw-rw-r--   0 root         (0) root         (0)     1410 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/nosql/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3027 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/nosql/_table_items.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:55:16.759133 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/push_notification/
+-rw-rw-r--   0 root         (0) root         (0)      794 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/push_notification/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1280 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/push_notification/_mobile_notification.py
+-rw-rw-r--   0 root         (0) root         (0)     1035 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/push_notification/_web_notificaton.py
+-rw-rw-r--   0 root         (0) root         (0)     1193 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/quick_ml.py
+-rw-rw-r--   0 root         (0) root         (0)     1203 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/search.py
+-rw-rw-r--   0 root         (0) root         (0)     5946 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/smart_browz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:55:16.760133 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/types/
+-rw-rw-r--   0 root         (0) root         (0)     7441 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/types/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4519 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/types/nosql.py
+-rw-rw-r--   0 root         (0) root         (0)     2782 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/types/smart_browz.py
+-rw-rw-r--   0 root         (0) root         (0)     2999 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/types/zia.py
+-rw-rw-r--   0 root         (0) root         (0)     9919 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/validator.py
+-rw-rw-r--   0 root         (0) root         (0)     1196 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/zcql.py
+-rw-rw-r--   0 root         (0) root         (0)     8247 2024-05-30 13:53:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/zia.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:55:16.760133 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2150 2024-05-30 13:55:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1414 2024-05-30 13:55:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 13:55:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-30 13:55:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-30 13:55:16.000000 zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk.egg-info/top_level.txt
```

### Comparing `zcatalyst_sdk-1.0.0rc2/LICENSE` & `zcatalyst_sdk-1.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/PKG-INFO` & `zcatalyst_sdk-1.0.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcatalyst_sdk
-Version: 1.0.0rc2
+Version: 1.0.0rc3
 Summary: Zoho Catalyst SDK for Python
 Home-page: https://catalyst.zoho.com/
 Author: Catalyst by Zoho
 Author-email: support@zohocatalyst.com
 License: Apache License 2.0
 Keywords: zcatalyst,zoho,catalyst,serverless,cloud,SDK,development
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zcatalyst_sdk Version: 1.0.0rc2 Summary: Zoho
+Metadata-Version: 2.1 Name: zcatalyst_sdk Version: 1.0.0rc3 Summary: Zoho
 Catalyst SDK for Python Home-page: https://catalyst.zoho.com/ Author: Catalyst
 by Zoho Author-email: support@zohocatalyst.com License: Apache License 2.0
 Keywords: zcatalyst,zoho,catalyst,serverless,cloud,SDK,development Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Development Status
 :: 4 - Beta Classifier: Intended Audience :: Developers Requires-Python: >= 3.9
```

### Comparing `zcatalyst_sdk-1.0.0rc2/README.md` & `zcatalyst_sdk-1.0.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/setup.py` & `zcatalyst_sdk-1.0.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/__init__.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/_constants.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/_constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 ADMIN_CRED_TYPE = "admin_cred_type"
 CLIENT_CRED_TYPE = "client_cred_type"
 REFRESH_TOKEN = "refresh_token"
 USER_TYPE = "user_type"
 CONNECTOR_NAME = "connector_name"
 ENVIRONMENT_KEY_NAME = "X-Catalyst-Environment"
 USER_KEY_NAME = "X-CATALYST-USER"
-ZCQL_PARSER = "ZOHO_CATALYST_ZCQL_PARSER"
 CATALYST_ORG_ID_KEY="CATALYST-ORG"
 X_CATALYST_ORG_ENV_KEY = 'X_ZOHO_CATALYST_ORG_ID'
 
 # URL constants
 PROJECT_URL = "project"
 PROJECT_KEY_NAME = "PROJECT_ID"
 URL_SEPARATOR = "/"
@@ -115,14 +114,15 @@
     DATA_STORE = "DataStore"
     FUNCTION = "Function"
     AUTHENTICATION = "Authentication"
     CIRCUIT = "Circuit"
     PUSH_NOTIFICATION = "PushNotification"
     SMART_BROWZ = "SmartBrowz"
     QUICK_ML = "QuickML"
+    NOSQL = 'NoSql'
 
 
 class CredentialType:
     token = 'token'
     ticket = 'ticket'
```

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/_http_client.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/_http_client.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/_thread_util.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/_thread_util.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/authentication.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/authentication.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/cache/__init__.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/cache/_segment.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/cache/_segment.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/catalyst_app.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/catalyst_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # pylint: disable=cyclic-import
 import os
 import json
 import threading
 from typing import Dict, Union
 import warnings
+
+from .nosql import NoSql
 from .types import ICatalystConfig
 from . import _constants as APIConstants
 from .credentials import Credential
 from .exceptions import CatalystAppError, CatalystCredentialError
 from .cache import Cache
 from .cron import Cron
 from .datastore import Datastore
@@ -187,12 +189,15 @@
 
     def smart_browz(self) -> SmartBrowz:
         return self._ensure_service('SmartBrowz', SmartBrowz)
 
     def quick_ml(self) -> QuickML:
         return self._ensure_service('QuickML', QuickML)
 
+    def nosql(self) -> NoSql:
+        return self._ensure_service('NoSql', NoSql)
+
     def _ensure_service(self, service_name: str, initializer, **kwargs):
         with self._lock:
             if service_name not in self._services or kwargs.get('override'):
                 self._services[service_name] = initializer(self, **kwargs)
             return self._services[service_name]
```

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/circuit.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/circuit.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/connection/__init__.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/connection/_connector.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/connection/_connector.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/credentials.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/credentials.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/cron.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/cron.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/datastore/__init__.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/datastore/_bulk_job.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/datastore/_bulk_job.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/datastore/_table.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/datastore/_table.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/email.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/email.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/exceptions.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,7 +124,11 @@
     def __init__(self, code, message, value=None):
         CatalystError.__init__(self, code, message, value)
 
 
 class QuickMLError(CatalystError):
     def __init__(self, code, message, value=None):
         CatalystError.__init__(self, code, message, value)
+
+class CatalystNoSqlError(CatalystError):
+    def __init__(self, code, message, value=None):
+        CatalystError.__init__(self, code, message, value)
```

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/filestore/__init__.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/filestore/__init__.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/filestore/_folder.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/filestore/_folder.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/functions.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/functions.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/push_notification/__init__.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/push_notification/__init__.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/push_notification/_mobile_notification.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/push_notification/_mobile_notification.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/push_notification/_web_notificaton.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/push_notification/_web_notificaton.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/quick_ml.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/quick_ml.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/search.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/search.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/smart_browz.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/smart_browz.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/types/__init__.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/types/__init__.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/types/smart_browz.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/types/smart_browz.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/types/zia.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/types/zia.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/validator.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/validator.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/zcql.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/zcql.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-import os
 from typing import Dict, List, TypedDict
 from .types import Component
 from .exceptions import CatalystZCQLError
 from ._http_client import AuthorizedHttpClient
 from ._constants import (
     RequestMethod,
     CredentialUser,
     Components,
-    AcceptHeader,
-    ZCQL_PARSER
+    AcceptHeader
 )
 
 ZcqlQueryOutput = TypedDict('ZcqlQueryOutput', {'table_name': Dict})
 
 
 class Zcql(Component):
     def __init__(self, app) -> None:
@@ -32,11 +30,13 @@
             'query': query
         }
         resp = self._requester.request(
             method=RequestMethod.POST,
             path='/query',
             json=req_json,
             user=CredentialUser.USER,
-            headers={AcceptHeader.KEY: AcceptHeader.ZCQL} if os.getenv(ZCQL_PARSER) == 'V2' else {}
+            headers={
+                AcceptHeader.KEY: AcceptHeader.ZCQL
+            }
         )
         resp_json = resp.response_json
         return resp_json.get('data')
```

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk/zia.py` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk/zia.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk.egg-info/PKG-INFO` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: zcatalyst-sdk
-Version: 1.0.0rc2
+Name: zcatalyst_sdk
+Version: 1.0.0rc3
 Summary: Zoho Catalyst SDK for Python
 Home-page: https://catalyst.zoho.com/
 Author: Catalyst by Zoho
 Author-email: support@zohocatalyst.com
 License: Apache License 2.0
 Keywords: zcatalyst,zoho,catalyst,serverless,cloud,SDK,development
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zcatalyst-sdk Version: 1.0.0rc2 Summary: Zoho
+Metadata-Version: 2.1 Name: zcatalyst_sdk Version: 1.0.0rc3 Summary: Zoho
 Catalyst SDK for Python Home-page: https://catalyst.zoho.com/ Author: Catalyst
 by Zoho Author-email: support@zohocatalyst.com License: Apache License 2.0
 Keywords: zcatalyst,zoho,catalyst,serverless,cloud,SDK,development Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Development Status
 :: 4 - Beta Classifier: Intended Audience :: Developers Requires-Python: >= 3.9
```

### Comparing `zcatalyst_sdk-1.0.0rc2/zcatalyst_sdk.egg-info/SOURCES.txt` & `zcatalyst_sdk-1.0.0rc3/zcatalyst_sdk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -32,13 +32,16 @@
 zcatalyst_sdk/connection/__init__.py
 zcatalyst_sdk/connection/_connector.py
 zcatalyst_sdk/datastore/__init__.py
 zcatalyst_sdk/datastore/_bulk_job.py
 zcatalyst_sdk/datastore/_table.py
 zcatalyst_sdk/filestore/__init__.py
 zcatalyst_sdk/filestore/_folder.py
+zcatalyst_sdk/nosql/__init__.py
+zcatalyst_sdk/nosql/_table_items.py
 zcatalyst_sdk/push_notification/__init__.py
 zcatalyst_sdk/push_notification/_mobile_notification.py
 zcatalyst_sdk/push_notification/_web_notificaton.py
 zcatalyst_sdk/types/__init__.py
+zcatalyst_sdk/types/nosql.py
 zcatalyst_sdk/types/smart_browz.py
 zcatalyst_sdk/types/zia.py
```

