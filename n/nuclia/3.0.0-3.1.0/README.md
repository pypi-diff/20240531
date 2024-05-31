# Comparing `tmp/nuclia-3.0.0.tar.gz` & `tmp/nuclia-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuclia-3.0.0.tar", last modified: Thu May 30 08:38:07 2024, max compression
+gzip compressed data, was "nuclia-3.1.0.tar", last modified: Fri May 31 15:25:18 2024, max compression
```

## Comparing `nuclia-3.0.0.tar` & `nuclia-3.1.0.tar`

### file list

```diff
@@ -1,98 +1,99 @@
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-30 08:38:07.412576 nuclia-3.0.0/
--rw-r--r--   0 ebr        (501) staff       (20)       75 2024-05-17 10:33:03.000000 nuclia-3.0.0/.gitignore
--rw-r--r--   0 ebr        (501) staff       (20)        7 2024-05-17 10:31:16.000000 nuclia-3.0.0/.python-version
--rw-r--r--   0 ebr        (501) staff       (20)     4020 2024-05-30 08:30:30.000000 nuclia-3.0.0/CHANGELOG.md
--rw-r--r--   0 ebr        (501) staff       (20)     1063 2023-06-23 08:56:29.000000 nuclia-3.0.0/LICENSE
--rw-r--r--   0 ebr        (501) staff       (20)       83 2023-06-23 08:56:29.000000 nuclia-3.0.0/MANIFEST.in
--rw-r--r--   0 ebr        (501) staff       (20)      270 2023-12-05 13:45:31.000000 nuclia-3.0.0/Makefile
--rw-r--r--   0 ebr        (501) staff       (20)     2071 2024-05-30 08:38:07.412284 nuclia-3.0.0/PKG-INFO
--rw-r--r--   0 ebr        (501) staff       (20)      967 2023-12-05 13:45:19.000000 nuclia-3.0.0/README.md
--rw-r--r--   0 ebr        (501) staff       (20)        6 2024-05-30 08:30:30.000000 nuclia-3.0.0/VERSION
--rw-r--r--   0 ebr        (501) staff       (20)       24 2023-06-23 08:56:29.000000 nuclia-3.0.0/code-requirements.txt
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-30 08:38:07.336710 nuclia-3.0.0/docs/
--rw-r--r--   0 ebr        (501) staff       (20)      871 2023-12-05 13:45:19.000000 nuclia-3.0.0/docs/01-README.md
--rw-r--r--   0 ebr        (501) staff       (20)     1894 2024-03-07 14:48:18.000000 nuclia-3.0.0/docs/02-auth.md
--rw-r--r--   0 ebr        (501) staff       (20)     5533 2024-05-30 06:48:00.000000 nuclia-3.0.0/docs/03-kb.md
--rw-r--r--   0 ebr        (501) staff       (20)     3285 2024-03-18 16:03:33.000000 nuclia-3.0.0/docs/04-upload.md
--rw-r--r--   0 ebr        (501) staff       (20)     2353 2024-05-30 06:48:00.000000 nuclia-3.0.0/docs/05-search.md
--rw-r--r--   0 ebr        (501) staff       (20)     1234 2023-12-05 13:45:19.000000 nuclia-3.0.0/docs/06-read.md
--rw-r--r--   0 ebr        (501) staff       (20)     3247 2023-12-11 18:33:41.000000 nuclia-3.0.0/docs/07-nua.md
--rw-r--r--   0 ebr        (501) staff       (20)     1987 2023-12-05 13:45:19.000000 nuclia-3.0.0/docs/08-import-export.md
--rw-r--r--   0 ebr        (501) staff       (20)     2072 2023-12-05 13:45:19.000000 nuclia-3.0.0/docs/09-manage.md
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-30 08:38:07.345728 nuclia-3.0.0/nuclia/
--rw-r--r--   0 ebr        (501) staff       (20)      698 2024-05-13 16:41:21.000000 nuclia-3.0.0/nuclia/__init__.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-30 08:38:07.352691 nuclia-3.0.0/nuclia/cli/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-06-23 08:56:29.000000 nuclia-3.0.0/nuclia/cli/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)     1522 2024-02-21 09:09:46.000000 nuclia-3.0.0/nuclia/cli/run.py
--rw-r--r--   0 ebr        (501) staff       (20)     1223 2023-07-05 15:34:25.000000 nuclia-3.0.0/nuclia/cli/utils.py
--rw-r--r--   0 ebr        (501) staff       (20)     8077 2024-02-21 09:09:46.000000 nuclia-3.0.0/nuclia/config.py
--rw-r--r--   0 ebr        (501) staff       (20)     1021 2024-02-26 11:30:29.000000 nuclia-3.0.0/nuclia/data.py
--rw-r--r--   0 ebr        (501) staff       (20)     8242 2024-02-26 11:30:29.000000 nuclia-3.0.0/nuclia/decorators.py
--rw-r--r--   0 ebr        (501) staff       (20)      565 2024-03-27 08:57:22.000000 nuclia-3.0.0/nuclia/exceptions.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-30 08:38:07.360794 nuclia-3.0.0/nuclia/lib/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-06-23 08:56:29.000000 nuclia-3.0.0/nuclia/lib/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      153 2023-07-05 15:34:25.000000 nuclia-3.0.0/nuclia/lib/conversations.py
--rw-r--r--   0 ebr        (501) staff       (20)    15010 2024-05-17 10:00:29.000000 nuclia-3.0.0/nuclia/lib/kb.py
--rw-r--r--   0 ebr        (501) staff       (20)    19017 2024-05-13 16:41:21.000000 nuclia-3.0.0/nuclia/lib/nua.py
--rw-r--r--   0 ebr        (501) staff       (20)    11215 2024-05-16 14:03:49.000000 nuclia-3.0.0/nuclia/lib/nua_responses.py
--rw-r--r--   0 ebr        (501) staff       (20)      589 2024-03-27 08:57:22.000000 nuclia-3.0.0/nuclia/lib/utils.py
--rw-r--r--   0 ebr        (501) staff       (20)        0 2024-05-13 16:41:21.000000 nuclia-3.0.0/nuclia/py.typed
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-30 08:38:07.386967 nuclia-3.0.0/nuclia/sdk/
--rw-r--r--   0 ebr        (501) staff       (20)      822 2024-03-15 16:57:58.000000 nuclia-3.0.0/nuclia/sdk/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      647 2023-12-05 13:45:19.000000 nuclia-3.0.0/nuclia/sdk/accounts.py
--rw-r--r--   0 ebr        (501) staff       (20)     1961 2024-05-30 06:48:00.000000 nuclia-3.0.0/nuclia/sdk/agent.py
--rw-r--r--   0 ebr        (501) staff       (20)    20954 2024-03-08 08:24:24.000000 nuclia-3.0.0/nuclia/sdk/auth.py
--rw-r--r--   0 ebr        (501) staff       (20)     9654 2024-03-15 16:57:58.000000 nuclia-3.0.0/nuclia/sdk/export_import.py
--rw-r--r--   0 ebr        (501) staff       (20)    11245 2024-03-26 08:30:00.000000 nuclia-3.0.0/nuclia/sdk/kb.py
--rw-r--r--   0 ebr        (501) staff       (20)     4648 2024-02-21 09:09:46.000000 nuclia-3.0.0/nuclia/sdk/kbs.py
--rw-r--r--   0 ebr        (501) staff       (20)       57 2023-07-05 15:34:25.000000 nuclia-3.0.0/nuclia/sdk/logger.py
--rw-r--r--   0 ebr        (501) staff       (20)      462 2024-02-29 17:16:47.000000 nuclia-3.0.0/nuclia/sdk/logs.py
--rw-r--r--   0 ebr        (501) staff       (20)      369 2023-12-05 13:45:31.000000 nuclia-3.0.0/nuclia/sdk/nua.py
--rw-r--r--   0 ebr        (501) staff       (20)     1288 2024-03-15 16:57:58.000000 nuclia-3.0.0/nuclia/sdk/nucliadb.py
--rw-r--r--   0 ebr        (501) staff       (20)     8137 2024-05-13 16:41:21.000000 nuclia-3.0.0/nuclia/sdk/predict.py
--rw-r--r--   0 ebr        (501) staff       (20)     2196 2024-02-21 09:09:46.000000 nuclia-3.0.0/nuclia/sdk/process.py
--rw-r--r--   0 ebr        (501) staff       (20)     7018 2024-05-30 06:40:37.000000 nuclia-3.0.0/nuclia/sdk/resource.py
--rw-r--r--   0 ebr        (501) staff       (20)    10143 2024-05-30 06:48:00.000000 nuclia-3.0.0/nuclia/sdk/search.py
--rw-r--r--   0 ebr        (501) staff       (20)      188 2023-06-23 08:56:29.000000 nuclia-3.0.0/nuclia/sdk/train.py
--rw-r--r--   0 ebr        (501) staff       (20)    19774 2024-03-18 16:03:33.000000 nuclia-3.0.0/nuclia/sdk/upload.py
--rw-r--r--   0 ebr        (501) staff       (20)      342 2023-12-11 18:33:41.000000 nuclia-3.0.0/nuclia/sdk/zones.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-30 08:38:07.390415 nuclia-3.0.0/nuclia/tests/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-06-23 08:56:29.000000 nuclia-3.0.0/nuclia/tests/__init__.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-30 08:38:07.391688 nuclia-3.0.0/nuclia/tests/assets/
--rw-r--r--   0 ebr        (501) staff       (20)      348 2023-07-05 15:34:25.000000 nuclia-3.0.0/nuclia/tests/assets/conversation.json
--rw-r--r--   0 ebr        (501) staff       (20)       74 2023-12-05 13:45:31.000000 nuclia-3.0.0/nuclia/tests/conftest.py
--rw-r--r--   0 ebr        (501) staff       (20)     1527 2023-12-05 13:45:31.000000 nuclia-3.0.0/nuclia/tests/fixtures.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-30 08:38:07.400331 nuclia-3.0.0/nuclia/tests/test_kb/
--rw-r--r--   0 ebr        (501) staff       (20)      741 2023-12-05 13:45:19.000000 nuclia-3.0.0/nuclia/tests/test_kb/test_conversation.py
--rw-r--r--   0 ebr        (501) staff       (20)     1019 2023-12-05 13:45:19.000000 nuclia-3.0.0/nuclia/tests/test_kb/test_export_import.py
--rw-r--r--   0 ebr        (501) staff       (20)      879 2023-12-05 13:45:19.000000 nuclia-3.0.0/nuclia/tests/test_kb/test_labels.py
--rw-r--r--   0 ebr        (501) staff       (20)      269 2024-03-15 16:57:58.000000 nuclia-3.0.0/nuclia/tests/test_kb/test_logs.py
--rw-r--r--   0 ebr        (501) staff       (20)      996 2024-03-15 16:57:58.000000 nuclia-3.0.0/nuclia/tests/test_kb/test_resource.py
--rw-r--r--   0 ebr        (501) staff       (20)     1928 2024-05-30 06:48:00.000000 nuclia-3.0.0/nuclia/tests/test_kb/test_search.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-30 08:38:07.403832 nuclia-3.0.0/nuclia/tests/test_manage/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-12-05 13:45:19.000000 nuclia-3.0.0/nuclia/tests/test_manage/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      289 2023-12-05 13:45:19.000000 nuclia-3.0.0/nuclia/tests/test_manage/test_account.py
--rw-r--r--   0 ebr        (501) staff       (20)      540 2023-12-05 13:45:31.000000 nuclia-3.0.0/nuclia/tests/test_manage/test_auth.py
--rw-r--r--   0 ebr        (501) staff       (20)     1015 2023-12-21 17:23:36.000000 nuclia-3.0.0/nuclia/tests/test_manage/test_kb.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-30 08:38:07.406643 nuclia-3.0.0/nuclia/tests/test_nua/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-12-05 13:45:19.000000 nuclia-3.0.0/nuclia/tests/test_nua/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      334 2024-01-08 09:24:24.000000 nuclia-3.0.0/nuclia/tests/test_nua/test_agent.py
--rw-r--r--   0 ebr        (501) staff       (20)     1931 2024-05-16 14:03:49.000000 nuclia-3.0.0/nuclia/tests/test_nua/test_predict.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-30 08:38:07.408136 nuclia-3.0.0/nuclia/tests/test_nucliadb/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-12-05 13:45:19.000000 nuclia-3.0.0/nuclia/tests/test_nucliadb/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)     1235 2024-03-15 16:57:58.000000 nuclia-3.0.0/nuclia/tests/test_nucliadb/test_crud.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-30 08:38:07.409800 nuclia-3.0.0/nuclia/tests/unit/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-12-05 13:45:19.000000 nuclia-3.0.0/nuclia/tests/unit/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      980 2023-12-05 13:45:19.000000 nuclia-3.0.0/nuclia/tests/unit/test_export_import.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-30 08:38:07.411219 nuclia-3.0.0/nuclia.egg-info/
--rw-r--r--   0 ebr        (501) staff       (20)     2071 2024-05-30 08:38:07.000000 nuclia-3.0.0/nuclia.egg-info/PKG-INFO
--rw-r--r--   0 ebr        (501) staff       (20)     1964 2024-05-30 08:38:07.000000 nuclia-3.0.0/nuclia.egg-info/SOURCES.txt
--rw-r--r--   0 ebr        (501) staff       (20)        1 2024-05-30 08:38:07.000000 nuclia-3.0.0/nuclia.egg-info/dependency_links.txt
--rw-r--r--   0 ebr        (501) staff       (20)       46 2024-05-30 08:38:07.000000 nuclia-3.0.0/nuclia.egg-info/entry_points.txt
--rw-r--r--   0 ebr        (501) staff       (20)      161 2024-05-30 08:38:07.000000 nuclia-3.0.0/nuclia.egg-info/requires.txt
--rw-r--r--   0 ebr        (501) staff       (20)        7 2024-05-30 08:38:07.000000 nuclia-3.0.0/nuclia.egg-info/top_level.txt
--rw-r--r--   0 ebr        (501) staff       (20)        1 2023-06-23 09:03:16.000000 nuclia-3.0.0/nuclia.egg-info/zip-safe
--rw-r--r--   0 ebr        (501) staff       (20)      160 2024-05-30 08:30:06.000000 nuclia-3.0.0/requirements.txt
--rw-r--r--   0 ebr        (501) staff       (20)      204 2024-05-30 08:38:07.413612 nuclia-3.0.0/setup.cfg
--rw-r--r--   0 ebr        (501) staff       (20)     1946 2023-12-05 13:45:19.000000 nuclia-3.0.0/setup.py
--rw-r--r--   0 ebr        (501) staff       (20)      228 2024-05-13 16:41:21.000000 nuclia-3.0.0/test-requirements.txt
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-31 15:25:18.644705 nuclia-3.1.0/
+-rw-r--r--   0 ebr        (501) staff       (20)       75 2024-05-31 15:25:17.000000 nuclia-3.1.0/.gitignore
+-rw-r--r--   0 ebr        (501) staff       (20)        7 2024-05-31 15:25:17.000000 nuclia-3.1.0/.python-version
+-rw-r--r--   0 ebr        (501) staff       (20)     4147 2024-05-31 15:25:17.000000 nuclia-3.1.0/CHANGELOG.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1063 2024-05-31 15:25:17.000000 nuclia-3.1.0/LICENSE
+-rw-r--r--   0 ebr        (501) staff       (20)       83 2024-05-31 15:25:17.000000 nuclia-3.1.0/MANIFEST.in
+-rw-r--r--   0 ebr        (501) staff       (20)      270 2024-05-31 15:25:17.000000 nuclia-3.1.0/Makefile
+-rw-r--r--   0 ebr        (501) staff       (20)     2057 2024-05-31 15:25:18.644519 nuclia-3.1.0/PKG-INFO
+-rw-r--r--   0 ebr        (501) staff       (20)      967 2024-05-31 15:25:17.000000 nuclia-3.1.0/README.md
+-rw-r--r--   0 ebr        (501) staff       (20)        6 2024-05-31 15:25:17.000000 nuclia-3.1.0/VERSION
+-rw-r--r--   0 ebr        (501) staff       (20)       24 2024-05-31 15:25:17.000000 nuclia-3.1.0/code-requirements.txt
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-31 15:25:18.613668 nuclia-3.1.0/docs/
+-rw-r--r--   0 ebr        (501) staff       (20)      871 2024-05-31 15:25:17.000000 nuclia-3.1.0/docs/01-README.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1894 2024-05-31 15:25:17.000000 nuclia-3.1.0/docs/02-auth.md
+-rw-r--r--   0 ebr        (501) staff       (20)     5533 2024-05-31 15:25:17.000000 nuclia-3.1.0/docs/03-kb.md
+-rw-r--r--   0 ebr        (501) staff       (20)     3578 2024-05-31 15:25:17.000000 nuclia-3.1.0/docs/04-upload.md
+-rw-r--r--   0 ebr        (501) staff       (20)     2353 2024-05-31 15:25:17.000000 nuclia-3.1.0/docs/05-search.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1234 2024-05-31 15:25:17.000000 nuclia-3.1.0/docs/06-read.md
+-rw-r--r--   0 ebr        (501) staff       (20)     3247 2024-05-31 15:25:17.000000 nuclia-3.1.0/docs/07-nua.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1987 2024-05-31 15:25:17.000000 nuclia-3.1.0/docs/08-import-export.md
+-rw-r--r--   0 ebr        (501) staff       (20)     2072 2024-05-31 15:25:17.000000 nuclia-3.1.0/docs/09-manage.md
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-31 15:25:18.617361 nuclia-3.1.0/nuclia/
+-rw-r--r--   0 ebr        (501) staff       (20)      698 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/__init__.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-31 15:25:18.626149 nuclia-3.1.0/nuclia/cli/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/cli/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1522 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/cli/run.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1223 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/cli/utils.py
+-rw-r--r--   0 ebr        (501) staff       (20)     8077 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/config.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1021 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/data.py
+-rw-r--r--   0 ebr        (501) staff       (20)     8242 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/decorators.py
+-rw-r--r--   0 ebr        (501) staff       (20)      565 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/exceptions.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-31 15:25:18.629168 nuclia-3.1.0/nuclia/lib/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/lib/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      149 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/lib/conversations.py
+-rw-r--r--   0 ebr        (501) staff       (20)    15010 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/lib/kb.py
+-rw-r--r--   0 ebr        (501) staff       (20)    19017 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/lib/nua.py
+-rw-r--r--   0 ebr        (501) staff       (20)    11815 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/lib/nua_responses.py
+-rw-r--r--   0 ebr        (501) staff       (20)      589 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/lib/utils.py
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/py.typed
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-31 15:25:18.635705 nuclia-3.1.0/nuclia/sdk/
+-rw-r--r--   0 ebr        (501) staff       (20)      822 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/sdk/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      647 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/sdk/accounts.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1961 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/sdk/agent.py
+-rw-r--r--   0 ebr        (501) staff       (20)    20954 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/sdk/auth.py
+-rw-r--r--   0 ebr        (501) staff       (20)     9654 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/sdk/export_import.py
+-rw-r--r--   0 ebr        (501) staff       (20)    11245 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/sdk/kb.py
+-rw-r--r--   0 ebr        (501) staff       (20)     4648 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/sdk/kbs.py
+-rw-r--r--   0 ebr        (501) staff       (20)       57 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/sdk/logger.py
+-rw-r--r--   0 ebr        (501) staff       (20)      462 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/sdk/logs.py
+-rw-r--r--   0 ebr        (501) staff       (20)      369 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/sdk/nua.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1288 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/sdk/nucliadb.py
+-rw-r--r--   0 ebr        (501) staff       (20)     8137 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/sdk/predict.py
+-rw-r--r--   0 ebr        (501) staff       (20)     2196 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/sdk/process.py
+-rw-r--r--   0 ebr        (501) staff       (20)     7018 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/sdk/resource.py
+-rw-r--r--   0 ebr        (501) staff       (20)    10103 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/sdk/search.py
+-rw-r--r--   0 ebr        (501) staff       (20)      188 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/sdk/train.py
+-rw-r--r--   0 ebr        (501) staff       (20)    20400 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/sdk/upload.py
+-rw-r--r--   0 ebr        (501) staff       (20)      342 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/sdk/zones.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-31 15:25:18.636557 nuclia-3.1.0/nuclia/tests/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/tests/__init__.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-31 15:25:18.636937 nuclia-3.1.0/nuclia/tests/assets/
+-rw-r--r--   0 ebr        (501) staff       (20)      348 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/tests/assets/conversation.json
+-rw-r--r--   0 ebr        (501) staff       (20)       74 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/tests/conftest.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1527 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/tests/fixtures.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-31 15:25:18.638828 nuclia-3.1.0/nuclia/tests/test_kb/
+-rw-r--r--   0 ebr        (501) staff       (20)      741 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/tests/test_kb/test_conversation.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1019 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/tests/test_kb/test_export_import.py
+-rw-r--r--   0 ebr        (501) staff       (20)      879 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/tests/test_kb/test_labels.py
+-rw-r--r--   0 ebr        (501) staff       (20)      269 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/tests/test_kb/test_logs.py
+-rw-r--r--   0 ebr        (501) staff       (20)      996 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/tests/test_kb/test_resource.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1928 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/tests/test_kb/test_search.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-31 15:25:18.640192 nuclia-3.1.0/nuclia/tests/test_manage/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/tests/test_manage/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      289 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/tests/test_manage/test_account.py
+-rw-r--r--   0 ebr        (501) staff       (20)      540 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/tests/test_manage/test_auth.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1015 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/tests/test_manage/test_kb.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-31 15:25:18.641170 nuclia-3.1.0/nuclia/tests/test_nua/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/tests/test_nua/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      334 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/tests/test_nua/test_agent.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1931 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/tests/test_nua/test_predict.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-31 15:25:18.641692 nuclia-3.1.0/nuclia/tests/test_nucliadb/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/tests/test_nucliadb/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1235 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/tests/test_nucliadb/test_crud.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-31 15:25:18.643288 nuclia-3.1.0/nuclia/tests/unit/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/tests/unit/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      980 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/tests/unit/test_export_import.py
+-rw-r--r--   0 ebr        (501) staff       (20)      319 2024-05-31 15:25:17.000000 nuclia-3.1.0/nuclia/tests/unit/test_nua_responses.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-31 15:25:18.643726 nuclia-3.1.0/nuclia.egg-info/
+-rw-r--r--   0 ebr        (501) staff       (20)     2057 2024-05-31 15:25:18.000000 nuclia-3.1.0/nuclia.egg-info/PKG-INFO
+-rw-r--r--   0 ebr        (501) staff       (20)     2004 2024-05-31 15:25:18.000000 nuclia-3.1.0/nuclia.egg-info/SOURCES.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        1 2024-05-31 15:25:18.000000 nuclia-3.1.0/nuclia.egg-info/dependency_links.txt
+-rw-r--r--   0 ebr        (501) staff       (20)       46 2024-05-31 15:25:18.000000 nuclia-3.1.0/nuclia.egg-info/entry_points.txt
+-rw-r--r--   0 ebr        (501) staff       (20)      147 2024-05-31 15:25:18.000000 nuclia-3.1.0/nuclia.egg-info/requires.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        7 2024-05-31 15:25:18.000000 nuclia-3.1.0/nuclia.egg-info/top_level.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        1 2024-05-31 15:25:18.000000 nuclia-3.1.0/nuclia.egg-info/zip-safe
+-rw-r--r--   0 ebr        (501) staff       (20)      146 2024-05-31 15:25:17.000000 nuclia-3.1.0/requirements.txt
+-rw-r--r--   0 ebr        (501) staff       (20)      204 2024-05-31 15:25:18.645375 nuclia-3.1.0/setup.cfg
+-rw-r--r--   0 ebr        (501) staff       (20)     1946 2024-05-31 15:25:17.000000 nuclia-3.1.0/setup.py
+-rw-r--r--   0 ebr        (501) staff       (20)      228 2024-05-31 15:25:17.000000 nuclia-3.1.0/test-requirements.txt
```

### Comparing `nuclia-3.0.0/CHANGELOG.md` & `nuclia-3.1.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog
 
+## 3.1.0 (2024-05-31)
+
+### Features
+
+- Support table interpretation when uploading a file
+
+### Fixes
+
+- Upgrade to pydantic 2
+
 ## 3.0.0 (2024-05-30)
 
 ### Breaking change
 
 - Rename `chat()` to `ask()`
 
 ## 2.1.0 (2024-05-17)
```

### Comparing `nuclia-3.0.0/LICENSE` & `nuclia-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/PKG-INFO` & `nuclia-3.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclia
-Version: 3.0.0
+Version: 3.1.0
 Home-page: https://nuclia.com
 Author: Nuclia
 Author-email: info@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
 Project-URL: Discord, https://discord.gg/8EvQwmsbzf
@@ -22,16 +22,16 @@
 Requires-Dist: fire
 Requires-Dist: pydantic>=2.0.0
 Requires-Dist: pyyaml>=5.4
 Requires-Dist: requests
 Requires-Dist: httpx
 Requires-Dist: httpcore>=1.0.0
 Requires-Dist: prompt_toolkit
-Requires-Dist: nucliadb_sdk<4,>=3.2.0
-Requires-Dist: nucliadb_models<4,>=3.2.0
+Requires-Dist: nucliadb_sdk>=4
+Requires-Dist: nucliadb_models>=4
 Requires-Dist: tqdm
 Requires-Dist: aiofiles
 Requires-Dist: backoff
 Requires-Dist: deprecated
 
 # Nuclia Python Client
```

### Comparing `nuclia-3.0.0/README.md` & `nuclia-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/docs/01-README.md` & `nuclia-3.1.0/docs/01-README.md`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/docs/02-auth.md` & `nuclia-3.1.0/docs/02-auth.md`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/docs/03-kb.md` & `nuclia-3.1.0/docs/03-kb.md`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/docs/04-upload.md` & `nuclia-3.1.0/docs/04-upload.md`

 * *Files 14% similar despite different names*

```diff
@@ -32,14 +32,28 @@
 
 Streaming a file to a Knowledge Box from an external URL its easy as:
 
 ```bash
 nuclia kb upload remote --origin=REMOTE_FILE_URL
 ```
 
+## Interpret tables in a file
+
+When uploading a file, you can ask Nuclia to interpret tables in the file:
+
+```bash
+nuclia kb upload file --path=FILE_PATH --interpretTables
+```
+
+```python
+from nuclia import sdk
+upload = sdk.NucliaUpload()
+upload.file(path=FILE_PATH, interpretTables=True)
+```
+
 ## Upload a remote file in an existing resource
 
 In case you want to stream a file inside a resource you can use:
 
 ```bash
 nuclia kb upload remote --origin=REMOTE_FILE_URL --rid=RESOURCE_ID --field=FIELD_ID
 ```
```

### Comparing `nuclia-3.0.0/docs/05-search.md` & `nuclia-3.1.0/docs/05-search.md`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/docs/06-read.md` & `nuclia-3.1.0/docs/06-read.md`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/docs/07-nua.md` & `nuclia-3.1.0/docs/07-nua.md`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/docs/08-import-export.md` & `nuclia-3.1.0/docs/08-import-export.md`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/docs/09-manage.md` & `nuclia-3.1.0/docs/09-manage.md`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/__init__.py` & `nuclia-3.1.0/nuclia/__init__.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/cli/run.py` & `nuclia-3.1.0/nuclia/cli/run.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/cli/utils.py` & `nuclia-3.1.0/nuclia/cli/utils.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/config.py` & `nuclia-3.1.0/nuclia/config.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/data.py` & `nuclia-3.1.0/nuclia/data.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/decorators.py` & `nuclia-3.1.0/nuclia/decorators.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/exceptions.py` & `nuclia-3.1.0/nuclia/exceptions.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/lib/kb.py` & `nuclia-3.1.0/nuclia/lib/kb.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/lib/nua.py` & `nuclia-3.1.0/nuclia/lib/nua.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/lib/nua_responses.py` & `nuclia-3.1.0/nuclia/lib/nua_responses.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import re
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Literal, Optional, Union, cast
 
-from pydantic import BaseModel, ConstrainedStr, Field
+import pydantic
+from pydantic import BaseModel, Field
+from typing_extensions import Annotated
 
 
 class GenerativeOption(BaseModel):
     name: str
     value: str
     user_prompt: Optional[str] = None
     user_key: Optional[str] = None
@@ -214,17 +215,34 @@
 
 
 class Source(int, Enum):
     HTTP = 0
     INGEST = 1
 
 
-class RestrictedIDString(ConstrainedStr):
-    regex = re.compile(r"^[a-z0-9_-]+$")
-    min_length = 1
+def validate_uuid(value, handler, info):
+    if not value:
+        raise ValueError(f"Invalid uuid: '{value}'. Uuid must be a non-empty string.")
+    try:
+        return handler(value)
+    except pydantic.ValidationError as e:
+        if any(x["type"] == "string_pattern_mismatch" for x in e.errors()):
+            raise ValueError(
+                f"Invalid slug: '{value}'. Slug must be a string with only "
+                "letters, numbers, underscores, colons and dashes."
+            )
+        else:
+            raise e
+
+
+RestrictedIDString = Annotated[
+    str,
+    pydantic.StringConstraints(pattern=r"^[a-z0-9_-]+$"),
+    pydantic.WrapValidator(validate_uuid),
+]
 
 
 class PushProcessingOptions(BaseModel):
     # Enable ML processing
     ml_text: bool = True
```

### Comparing `nuclia-3.0.0/nuclia/lib/utils.py` & `nuclia-3.1.0/nuclia/lib/utils.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/sdk/__init__.py` & `nuclia-3.1.0/nuclia/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/sdk/accounts.py` & `nuclia-3.1.0/nuclia/sdk/accounts.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/sdk/agent.py` & `nuclia-3.1.0/nuclia/sdk/agent.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/sdk/auth.py` & `nuclia-3.1.0/nuclia/sdk/auth.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/sdk/export_import.py` & `nuclia-3.1.0/nuclia/sdk/export_import.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/sdk/kb.py` & `nuclia-3.1.0/nuclia/sdk/kb.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/sdk/kbs.py` & `nuclia-3.1.0/nuclia/sdk/kbs.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/sdk/nucliadb.py` & `nuclia-3.1.0/nuclia/sdk/nucliadb.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/sdk/predict.py` & `nuclia-3.1.0/nuclia/sdk/predict.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/sdk/process.py` & `nuclia-3.1.0/nuclia/sdk/process.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/sdk/resource.py` & `nuclia-3.1.0/nuclia/sdk/resource.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/sdk/search.py` & `nuclia-3.1.0/nuclia/sdk/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                 sys.exit(1)
         elif isinstance(query, AskRequest):
             req = query
         else:
             raise ValueError("Invalid query type. Must be str, dict or AskRequest.")
 
         ask_response: SyncAskResponse = ndb.ndb.ask(kbid=ndb.kbid, content=req)
-  
+
         result = AskAnswer(
             answer=ask_response.answer.encode(),
             learning_id=ask_response.learning_id,
             relations_result=ask_response.relations,
             find_result=ask_response.retrieval_results,
             citations=ask_response.citations,
             timings=None,
@@ -308,11 +308,9 @@
                     result.timings = ask_response_item.timings.dict()
                 if ask_response_item.tokens:
                     result.tokens = ask_response_item.tokens.dict()
             elif ask_response_item.type == "status":
                 # Status is ignored
                 pass
             else:  # pragma: no cover
-                warnings.warn(
-                    f"Unknown ask stream item type: {ask_response_item.type}"
-                )
+                warnings.warn(f"Unknown ask stream item type: {ask_response_item.type}")
         return result
```

### Comparing `nuclia-3.0.0/nuclia/sdk/upload.py` & `nuclia-3.1.0/nuclia/sdk/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,23 +56,26 @@
     @kb
     def file(
         self,
         *,
         path: str,
         rid: Optional[str] = None,
         field: Optional[str] = None,
+        interpretTables: Optional[bool] = False,
         **kwargs,
     ) -> str:
         """Upload a file from filesystem to a Nuclia KnowledgeBox"""
         ndb: NucliaDBClient = kwargs["ndb"]
         filename = path.split("/")[-1]
         size = os.path.getsize(path)
         mimetype = mimetypes.guess_type(path)[0]
         if not mimetype:
             mimetype = "application/octet-stream"
+        if interpretTables:
+            mimetype += '+aitable'
         rid, is_new_resource = self._get_or_create_resource(
             rid=rid, icon=mimetype, **kwargs
         )
         if not field:
             field = uuid4().hex
         md5_hash = hashlib.md5()
 
@@ -102,15 +105,17 @@
                     ndb.ndb.delete_resource(kbid=ndb.kbid, rid=rid)
                 raise
         return rid
 
     @kb
     def conversation(self, *, path: str, **kwargs) -> str:
         """Upload a conversation from a JSON located on the filesystem to a Nuclia KnowledgeBox"""
-        conversation = Conversation.parse_file(path).__root__
+        with open(path, "rb") as f:
+            json_data = f.read()
+            conversation = Conversation.model_validate_json(json_data).root
         if conversation is None or len(conversation) == 0:
             return ""
 
         field = kwargs.get("field") or uuid4().hex
         conversations = {
             field: {
                 "messages": [
@@ -228,14 +233,15 @@
     @kb
     def remote(
         self,
         *,
         origin: str,
         rid: Optional[str] = None,
         field: Optional[str] = "file",
+        interpretTables: Optional[bool] = False,
         **kwargs,
     ) -> str:
         """Upload a remote url to a Nuclia KnowledgeBox"""
         ndb = kwargs["ndb"]
         with requests.get(origin, stream=True) as r:
             try:
                 r.raise_for_status()
@@ -245,14 +251,16 @@
                 ) from ex
             filename = origin.split("/")[-1]
             size_str = r.headers.get("Content-Length")
             if size_str is None:
                 size_str = "-1"
             size = int(size_str)
             mimetype = r.headers.get("Content-Type", "application/octet-stream")
+            if interpretTables:
+                mimetype += '+aitable'
             rid, is_new_resource = self._get_or_create_resource(
                 rid=rid, icon=mimetype, **kwargs
             )
             try:
                 upload_url = ndb.start_tus_upload(
                     rid=rid,
                     field=field,
@@ -335,23 +343,26 @@
     async def file(
         self,
         *,
         path: str,
         rid: Optional[str] = None,
         field: Optional[str] = None,
         mimetype: Optional[str] = None,
+        interpretTables: Optional[bool] = False,
         **kwargs,
     ) -> str:
         """Upload a file from filesystem to a Nuclia KnowledgeBox"""
         ndb: AsyncNucliaDBClient = kwargs["ndb"]
         filename = path.split("/")[-1]
         size = os.path.getsize(path)
         mimetype = mimetype or mimetypes.guess_type(path)[0]
         if not mimetype:
             mimetype = "application/octet-stream"
+        if interpretTables:
+            mimetype += '+aitable'
         rid, is_new_resource = await self._get_or_create_resource(
             rid=rid, icon=mimetype, **kwargs
         )
         if not field:
             field = uuid4().hex
         md5_hash = hashlib.md5()
 
@@ -380,15 +391,17 @@
                     await ndb.ndb.delete_resource(kbid=ndb.kbid, rid=rid)
                 raise
         return rid
 
     @kb
     async def conversation(self, *, path: str, **kwargs) -> str:
         """Upload a conversation from a JSON located on the filesystem to a Nuclia KnowledgeBox"""
-        conversation = Conversation.parse_file(path).__root__
+        with open(path, "rb") as f:
+            json_data = f.read()
+        conversation = Conversation.model_validate_json(json_data).root
         if conversation is None or len(conversation) == 0:
             return ""
 
         field = kwargs.get("field") or uuid4().hex
         conversations = {
             field: {
                 "messages": [
@@ -504,26 +517,29 @@
     @kb
     async def remote(
         self,
         *,
         origin: str,
         rid: Optional[str] = None,
         field: Optional[str] = "file",
+        interpretTables: Optional[bool] = False,
         **kwargs,
     ) -> str:
         """Upload a remote url to a Nuclia KnowledgeBox"""
         ndb: AsyncNucliaDBClient = kwargs["ndb"]
         client = AsyncClient()
         async with client.stream("GET", origin) as r:
             filename = origin.split("/")[-1]
             size_str = r.headers.get("Content-Length")
             if size_str is None:
                 size_str = "-1"
             size = int(size_str)
             mimetype = r.headers.get("Content-Type", "application/octet-stream")
+            if interpretTables:
+                mimetype += '+aitable'
             rid, is_new_resource = await self._get_or_create_resource(
                 rid=rid, icon=mimetype, **kwargs
             )
             try:
                 upload_url = await ndb.start_tus_upload(
                     rid=rid,
                     field=field,
```

### Comparing `nuclia-3.0.0/nuclia/tests/fixtures.py` & `nuclia-3.1.0/nuclia/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/tests/test_kb/test_conversation.py` & `nuclia-3.1.0/nuclia/tests/test_kb/test_conversation.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/tests/test_kb/test_export_import.py` & `nuclia-3.1.0/nuclia/tests/test_kb/test_export_import.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/tests/test_kb/test_labels.py` & `nuclia-3.1.0/nuclia/tests/test_kb/test_labels.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/tests/test_kb/test_resource.py` & `nuclia-3.1.0/nuclia/tests/test_kb/test_resource.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/tests/test_kb/test_search.py` & `nuclia-3.1.0/nuclia/tests/test_kb/test_search.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/tests/test_manage/test_auth.py` & `nuclia-3.1.0/nuclia/tests/test_manage/test_auth.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/tests/test_manage/test_kb.py` & `nuclia-3.1.0/nuclia/tests/test_manage/test_kb.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/tests/test_nua/test_predict.py` & `nuclia-3.1.0/nuclia/tests/test_nua/test_predict.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/tests/test_nucliadb/test_crud.py` & `nuclia-3.1.0/nuclia/tests/test_nucliadb/test_crud.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia/tests/unit/test_export_import.py` & `nuclia-3.1.0/nuclia/tests/unit/test_export_import.py`

 * *Files identical despite different names*

### Comparing `nuclia-3.0.0/nuclia.egg-info/PKG-INFO` & `nuclia-3.1.0/nuclia.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclia
-Version: 3.0.0
+Version: 3.1.0
 Home-page: https://nuclia.com
 Author: Nuclia
 Author-email: info@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
 Project-URL: Discord, https://discord.gg/8EvQwmsbzf
@@ -22,16 +22,16 @@
 Requires-Dist: fire
 Requires-Dist: pydantic>=2.0.0
 Requires-Dist: pyyaml>=5.4
 Requires-Dist: requests
 Requires-Dist: httpx
 Requires-Dist: httpcore>=1.0.0
 Requires-Dist: prompt_toolkit
-Requires-Dist: nucliadb_sdk<4,>=3.2.0
-Requires-Dist: nucliadb_models<4,>=3.2.0
+Requires-Dist: nucliadb_sdk>=4
+Requires-Dist: nucliadb_models>=4
 Requires-Dist: tqdm
 Requires-Dist: aiofiles
 Requires-Dist: backoff
 Requires-Dist: deprecated
 
 # Nuclia Python Client
```

### Comparing `nuclia-3.0.0/nuclia.egg-info/SOURCES.txt` & `nuclia-3.1.0/nuclia.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -76,8 +76,9 @@
 nuclia/tests/test_manage/test_kb.py
 nuclia/tests/test_nua/__init__.py
 nuclia/tests/test_nua/test_agent.py
 nuclia/tests/test_nua/test_predict.py
 nuclia/tests/test_nucliadb/__init__.py
 nuclia/tests/test_nucliadb/test_crud.py
 nuclia/tests/unit/__init__.py
-nuclia/tests/unit/test_export_import.py
+nuclia/tests/unit/test_export_import.py
+nuclia/tests/unit/test_nua_responses.py
```

### Comparing `nuclia-3.0.0/setup.py` & `nuclia-3.1.0/setup.py`

 * *Files identical despite different names*

