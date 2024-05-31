# Comparing `tmp/zinolib-1.0.4.tar.gz` & `tmp/zinolib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zinolib-1.0.4.tar", last modified: Wed May 29 08:05:02 2024, max compression
+gzip compressed data, was "zinolib-1.1.0.tar", last modified: Fri May 31 11:53:28 2024, max compression
```

## Comparing `zinolib-1.0.4.tar` & `zinolib-1.1.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-29 08:05:02.399951 zinolib-1.0.4/
--rw-rw-r--   0 hm        (1000) hm        (1000)      114 2023-08-23 12:45:06.000000 zinolib-1.0.4/.git-blame-ignore-revs
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-29 08:05:02.395951 zinolib-1.0.4/.github/
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-29 08:05:02.395951 zinolib-1.0.4/.github/workflows/
--rw-rw-r--   0 hm        (1000) hm        (1000)     1654 2024-05-22 06:40:42.000000 zinolib-1.0.4/.github/workflows/linter.yml
--rw-rw-r--   0 hm        (1000) hm        (1000)     1049 2023-10-17 13:10:05.000000 zinolib-1.0.4/.github/workflows/publish-test-results.yml
--rw-rw-r--   0 hm        (1000) hm        (1000)     1406 2024-05-29 08:04:50.000000 zinolib-1.0.4/.github/workflows/test.yml
--rw-rw-r--   0 hm        (1000) hm        (1000)      192 2024-05-22 06:40:42.000000 zinolib-1.0.4/.gitignore
--rw-rw-r--   0 hm        (1000) hm        (1000)      417 2023-08-23 12:43:58.000000 zinolib-1.0.4/.pre-commit-config.yaml
--rw-rw-r--   0 hm        (1000) hm        (1000)    11358 2023-08-23 12:43:58.000000 zinolib-1.0.4/LICENSE
--rw-rw-r--   0 hm        (1000) hm        (1000)      484 2024-05-22 06:40:42.000000 zinolib-1.0.4/Makefile
--rw-r--r--   0 hm        (1000) hm        (1000)    14717 2024-05-29 08:05:02.399951 zinolib-1.0.4/PKG-INFO
--rw-rw-r--   0 hm        (1000) hm        (1000)      955 2023-08-23 12:45:06.000000 zinolib-1.0.4/README.rst
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-29 08:05:02.395951 zinolib-1.0.4/examples/
--rw-rw-r--   0 hm        (1000) hm        (1000)      771 2023-08-23 12:43:58.000000 zinolib-1.0.4/examples/auth.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2993 2023-08-15 12:56:17.000000 zinolib-1.0.4/examples/host_up_cleanup.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2598 2023-08-23 12:43:58.000000 zinolib-1.0.4/examples/monitor.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2261 2023-08-23 12:43:58.000000 zinolib-1.0.4/examples/pm-add.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1932 2023-08-23 12:43:58.000000 zinolib-1.0.4/examples/pm-test.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1930 2023-08-23 12:43:58.000000 zinolib-1.0.4/examples/pm-test2.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2199 2023-08-17 12:47:05.000000 zinolib-1.0.4/examples/reboot.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1902 2023-08-17 12:47:05.000000 zinolib-1.0.4/examples/schedule_reboot_host.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2465 2023-08-23 12:43:58.000000 zinolib-1.0.4/examples/test-with.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2576 2023-08-23 12:43:58.000000 zinolib-1.0.4/examples/test.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1172 2024-05-29 08:02:49.000000 zinolib-1.0.4/pyproject.toml
--rw-rw-r--   0 hm        (1000) hm        (1000)       38 2024-05-29 08:05:02.399951 zinolib-1.0.4/setup.cfg
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-29 08:05:02.395951 zinolib-1.0.4/src/
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-29 08:05:02.395951 zinolib-1.0.4/src/zinolib/
--rw-rw-r--   0 hm        (1000) hm        (1000)     1146 2023-08-24 07:39:23.000000 zinolib-1.0.4/src/zinolib/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      689 2024-05-22 06:40:42.000000 zinolib-1.0.4/src/zinolib/compat.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-29 08:05:02.399951 zinolib-1.0.4/src/zinolib/config/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2024-05-22 06:40:42.000000 zinolib-1.0.4/src/zinolib/config/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      373 2024-05-22 06:40:42.000000 zinolib-1.0.4/src/zinolib/config/models.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     3906 2024-05-22 06:40:42.000000 zinolib-1.0.4/src/zinolib/config/tcl.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      917 2024-05-22 06:40:42.000000 zinolib-1.0.4/src/zinolib/config/toml.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1346 2024-05-22 06:40:42.000000 zinolib-1.0.4/src/zinolib/config/utils.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2545 2024-05-22 06:40:42.000000 zinolib-1.0.4/src/zinolib/config/zino1.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-29 08:05:02.399951 zinolib-1.0.4/src/zinolib/controllers/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2024-05-22 06:40:42.000000 zinolib-1.0.4/src/zinolib/controllers/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2015 2024-05-22 06:40:42.000000 zinolib-1.0.4/src/zinolib/controllers/base.py
--rw-rw-r--   0 hm        (1000) hm        (1000)    19605 2024-05-29 08:01:44.000000 zinolib-1.0.4/src/zinolib/controllers/zino1.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     7270 2024-05-29 07:55:29.000000 zinolib-1.0.4/src/zinolib/event_types.py
--rw-rw-r--   0 hm        (1000) hm        (1000)    38357 2024-05-22 06:40:42.000000 zinolib-1.0.4/src/zinolib/ritz.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2723 2024-05-22 06:40:42.000000 zinolib-1.0.4/src/zinolib/utils.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      411 2024-05-29 08:05:02.000000 zinolib-1.0.4/src/zinolib/version.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     4549 2023-08-23 12:45:06.000000 zinolib-1.0.4/src/zinolib/zino_emu.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-29 08:05:02.399951 zinolib-1.0.4/src/zinolib.egg-info/
--rw-r--r--   0 hm        (1000) hm        (1000)    14717 2024-05-29 08:05:02.000000 zinolib-1.0.4/src/zinolib.egg-info/PKG-INFO
--rw-rw-r--   0 hm        (1000) hm        (1000)     1401 2024-05-29 08:05:02.000000 zinolib-1.0.4/src/zinolib.egg-info/SOURCES.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)        1 2024-05-29 08:05:02.000000 zinolib-1.0.4/src/zinolib.egg-info/dependency_links.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)        1 2024-05-29 08:05:02.000000 zinolib-1.0.4/src/zinolib.egg-info/not-zip-safe
--rw-rw-r--   0 hm        (1000) hm        (1000)       48 2024-05-29 08:05:02.000000 zinolib-1.0.4/src/zinolib.egg-info/requires.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)        8 2024-05-29 08:05:02.000000 zinolib-1.0.4/src/zinolib.egg-info/top_level.txt
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-29 08:05:02.399951 zinolib-1.0.4/tests/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2023-08-24 07:39:23.000000 zinolib-1.0.4/tests/__init__.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-29 08:05:02.399951 zinolib-1.0.4/tests/config/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2024-05-22 06:40:42.000000 zinolib-1.0.4/tests/config/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2840 2024-05-22 06:40:42.000000 zinolib-1.0.4/tests/config/test_tcl.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1664 2024-05-22 06:40:42.000000 zinolib-1.0.4/tests/config/test_toml.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1155 2024-05-22 06:40:42.000000 zinolib-1.0.4/tests/config/test_utils.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2280 2024-05-22 06:40:42.000000 zinolib-1.0.4/tests/config/test_zino1.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-29 08:05:02.399951 zinolib-1.0.4/tests/ritz/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2024-05-22 06:40:42.000000 zinolib-1.0.4/tests/ritz/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     7530 2024-05-22 06:40:42.000000 zinolib-1.0.4/tests/ritz/test_default.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1322 2024-05-22 06:40:42.000000 zinolib-1.0.4/tests/ritz/test_slow.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     9817 2024-05-29 08:01:44.000000 zinolib-1.0.4/tests/test_zinolib_controllers_zino1.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     9548 2024-05-29 07:55:29.000000 zinolib-1.0.4/tests/test_zinolib_event_types.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      390 2023-10-12 09:04:56.000000 zinolib-1.0.4/tests/test_zinolib_utils.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     4082 2024-05-22 06:40:42.000000 zinolib-1.0.4/tests/utils.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1573 2024-05-29 08:02:49.000000 zinolib-1.0.4/tox.ini
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-31 11:53:28.927042 zinolib-1.1.0/
+-rw-rw-r--   0 hm        (1000) hm        (1000)      114 2023-08-23 12:45:06.000000 zinolib-1.1.0/.git-blame-ignore-revs
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-31 11:53:28.923042 zinolib-1.1.0/.github/
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-31 11:53:28.927042 zinolib-1.1.0/.github/workflows/
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1654 2024-05-22 06:40:42.000000 zinolib-1.1.0/.github/workflows/linter.yml
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1049 2023-10-17 13:10:05.000000 zinolib-1.1.0/.github/workflows/publish-test-results.yml
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1413 2024-05-31 09:44:08.000000 zinolib-1.1.0/.github/workflows/test.yml
+-rw-rw-r--   0 hm        (1000) hm        (1000)      192 2024-05-22 06:40:42.000000 zinolib-1.1.0/.gitignore
+-rw-rw-r--   0 hm        (1000) hm        (1000)      417 2023-08-23 12:43:58.000000 zinolib-1.1.0/.pre-commit-config.yaml
+-rw-rw-r--   0 hm        (1000) hm        (1000)    11358 2023-08-23 12:43:58.000000 zinolib-1.1.0/LICENSE
+-rw-rw-r--   0 hm        (1000) hm        (1000)      484 2024-05-22 06:40:42.000000 zinolib-1.1.0/Makefile
+-rw-r--r--   0 hm        (1000) hm        (1000)    14717 2024-05-31 11:53:28.927042 zinolib-1.1.0/PKG-INFO
+-rw-rw-r--   0 hm        (1000) hm        (1000)      955 2023-08-23 12:45:06.000000 zinolib-1.1.0/README.rst
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-31 11:53:28.927042 zinolib-1.1.0/examples/
+-rw-rw-r--   0 hm        (1000) hm        (1000)      771 2023-08-23 12:43:58.000000 zinolib-1.1.0/examples/auth.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2993 2023-08-15 12:56:17.000000 zinolib-1.1.0/examples/host_up_cleanup.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2598 2023-08-23 12:43:58.000000 zinolib-1.1.0/examples/monitor.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2261 2023-08-23 12:43:58.000000 zinolib-1.1.0/examples/pm-add.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1932 2023-08-23 12:43:58.000000 zinolib-1.1.0/examples/pm-test.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1930 2023-08-23 12:43:58.000000 zinolib-1.1.0/examples/pm-test2.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2199 2023-08-17 12:47:05.000000 zinolib-1.1.0/examples/reboot.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1902 2023-08-17 12:47:05.000000 zinolib-1.1.0/examples/schedule_reboot_host.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2465 2023-08-23 12:43:58.000000 zinolib-1.1.0/examples/test-with.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2576 2023-08-23 12:43:58.000000 zinolib-1.1.0/examples/test.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1172 2024-05-29 08:02:49.000000 zinolib-1.1.0/pyproject.toml
+-rw-rw-r--   0 hm        (1000) hm        (1000)       38 2024-05-31 11:53:28.927042 zinolib-1.1.0/setup.cfg
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-31 11:53:28.923042 zinolib-1.1.0/src/
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-31 11:53:28.927042 zinolib-1.1.0/src/zinolib/
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1146 2023-08-24 07:39:23.000000 zinolib-1.1.0/src/zinolib/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      689 2024-05-22 06:40:42.000000 zinolib-1.1.0/src/zinolib/compat.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-31 11:53:28.927042 zinolib-1.1.0/src/zinolib/config/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2024-05-22 06:40:42.000000 zinolib-1.1.0/src/zinolib/config/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      373 2024-05-22 06:40:42.000000 zinolib-1.1.0/src/zinolib/config/models.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     3906 2024-05-22 06:40:42.000000 zinolib-1.1.0/src/zinolib/config/tcl.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      917 2024-05-22 06:40:42.000000 zinolib-1.1.0/src/zinolib/config/toml.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1346 2024-05-22 06:40:42.000000 zinolib-1.1.0/src/zinolib/config/utils.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2509 2024-05-31 11:25:30.000000 zinolib-1.1.0/src/zinolib/config/zino1.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-31 11:53:28.927042 zinolib-1.1.0/src/zinolib/controllers/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2024-05-22 06:40:42.000000 zinolib-1.1.0/src/zinolib/controllers/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2015 2024-05-22 06:40:42.000000 zinolib-1.1.0/src/zinolib/controllers/base.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)    20050 2024-05-31 11:52:30.000000 zinolib-1.1.0/src/zinolib/controllers/zino1.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     7270 2024-05-29 07:55:29.000000 zinolib-1.1.0/src/zinolib/event_types.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)    38357 2024-05-22 06:40:42.000000 zinolib-1.1.0/src/zinolib/ritz.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2723 2024-05-22 06:40:42.000000 zinolib-1.1.0/src/zinolib/utils.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      411 2024-05-31 11:53:28.000000 zinolib-1.1.0/src/zinolib/version.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     4549 2023-08-23 12:45:06.000000 zinolib-1.1.0/src/zinolib/zino_emu.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-31 11:53:28.927042 zinolib-1.1.0/src/zinolib.egg-info/
+-rw-r--r--   0 hm        (1000) hm        (1000)    14717 2024-05-31 11:53:28.000000 zinolib-1.1.0/src/zinolib.egg-info/PKG-INFO
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1401 2024-05-31 11:53:28.000000 zinolib-1.1.0/src/zinolib.egg-info/SOURCES.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)        1 2024-05-31 11:53:28.000000 zinolib-1.1.0/src/zinolib.egg-info/dependency_links.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)        1 2024-05-29 08:05:02.000000 zinolib-1.1.0/src/zinolib.egg-info/not-zip-safe
+-rw-rw-r--   0 hm        (1000) hm        (1000)       48 2024-05-31 11:53:28.000000 zinolib-1.1.0/src/zinolib.egg-info/requires.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)        8 2024-05-31 11:53:28.000000 zinolib-1.1.0/src/zinolib.egg-info/top_level.txt
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-31 11:53:28.927042 zinolib-1.1.0/tests/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2023-08-24 07:39:23.000000 zinolib-1.1.0/tests/__init__.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-31 11:53:28.927042 zinolib-1.1.0/tests/config/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2024-05-22 06:40:42.000000 zinolib-1.1.0/tests/config/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2840 2024-05-22 06:40:42.000000 zinolib-1.1.0/tests/config/test_tcl.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1664 2024-05-22 06:40:42.000000 zinolib-1.1.0/tests/config/test_toml.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1155 2024-05-22 06:40:42.000000 zinolib-1.1.0/tests/config/test_utils.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2308 2024-05-31 11:52:30.000000 zinolib-1.1.0/tests/config/test_zino1.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-31 11:53:28.927042 zinolib-1.1.0/tests/ritz/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2024-05-22 06:40:42.000000 zinolib-1.1.0/tests/ritz/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     7530 2024-05-22 06:40:42.000000 zinolib-1.1.0/tests/ritz/test_default.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1322 2024-05-22 06:40:42.000000 zinolib-1.1.0/tests/ritz/test_slow.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     9817 2024-05-29 08:01:44.000000 zinolib-1.1.0/tests/test_zinolib_controllers_zino1.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     9548 2024-05-29 07:55:29.000000 zinolib-1.1.0/tests/test_zinolib_event_types.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      390 2023-10-12 09:04:56.000000 zinolib-1.1.0/tests/test_zinolib_utils.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     4082 2024-05-22 06:40:42.000000 zinolib-1.1.0/tests/utils.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1573 2024-05-29 08:02:49.000000 zinolib-1.1.0/tox.ini
```

### Comparing `zinolib-1.0.4/.github/workflows/linter.yml` & `zinolib-1.1.0/.github/workflows/linter.yml`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/.github/workflows/publish-test-results.yml` & `zinolib-1.1.0/.github/workflows/publish-test-results.yml`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/.github/workflows/test.yml` & `zinolib-1.1.0/.github/workflows/test.yml`

 * *Files 18% similar despite different names*

```diff
@@ -46,12 +46,12 @@
       uses: actions/upload-artifact@v3
       with:
         name: reports
         path: |
           reports/**/*
 
     - name: "Upload coverage to Codecov"
-      if: "github.repository_owner == 'Uninett'"
-      uses: codecov/codecov-action@v3
+      if: github.repository_owner == 'Uninett'
+      uses: codecov/codecov-action@v4
       with:
         fail_ci_if_error: true
-        token: ${{ secrets.CODECOV_TOKEN }} # not required for public repos
+        token: ${{ secrets.CODECOV_TOKEN }} # not required for forks of public repos
```

### Comparing `zinolib-1.0.4/LICENSE` & `zinolib-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/PKG-INFO` & `zinolib-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zinolib
-Version: 1.0.4
+Version: 1.1.0
 Summary: Python interface to Zino
 Author-email: Runar Borge <runar.borge@sikt.no>
 Maintainer-email: Uninett Opensource <opensource@uninett.no>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `zinolib-1.0.4/README.rst` & `zinolib-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/examples/auth.py` & `zinolib-1.1.0/examples/auth.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/examples/host_up_cleanup.py` & `zinolib-1.1.0/examples/host_up_cleanup.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/examples/monitor.py` & `zinolib-1.1.0/examples/monitor.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/examples/pm-add.py` & `zinolib-1.1.0/examples/pm-add.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/examples/pm-test.py` & `zinolib-1.1.0/examples/pm-test.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/examples/pm-test2.py` & `zinolib-1.1.0/examples/pm-test2.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/examples/reboot.py` & `zinolib-1.1.0/examples/reboot.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/examples/schedule_reboot_host.py` & `zinolib-1.1.0/examples/schedule_reboot_host.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/examples/test-with.py` & `zinolib-1.1.0/examples/test-with.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/examples/test.py` & `zinolib-1.1.0/examples/test.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/pyproject.toml` & `zinolib-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/src/zinolib/__init__.py` & `zinolib-1.1.0/src/zinolib/__init__.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/src/zinolib/compat.py` & `zinolib-1.1.0/src/zinolib/compat.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/src/zinolib/config/tcl.py` & `zinolib-1.1.0/src/zinolib/config/tcl.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/src/zinolib/config/toml.py` & `zinolib-1.1.0/src/zinolib/config/toml.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/src/zinolib/config/utils.py` & `zinolib-1.1.0/src/zinolib/config/utils.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/src/zinolib/config/zino1.py` & `zinolib-1.1.0/src/zinolib/config/zino1.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     connection = fixed_dict["connections"][section]
     options = fixed_dict["global_options"]
     connection['password'] = connection.pop("secret")
     connection['port'] = int(connection.pop("port"))
     return connection, options
 
 
-class ZinoV1Config(UserConfig, ServerV1Config, Options):
+class ZinoV1Config(ServerV1Config, Options):
     """
     How to use::
 
     Given a legacy tcl config file stored on disk, containing at minimum server,
     username and secret::
 
         > config = ZinoV1Config.from_tcl()
@@ -37,33 +37,33 @@
 
         > config.update_from_args(args)
     """
     DEFAULT_SECTION: ClassVar = "default"
 
     @classmethod
     def get_legacy_class(cls):
-        return type("ZinoV1LegacyConfig", (UserConfig, ServerV1Config, Options, cls))
+        return type("ZinoV1LegacyConfig", (UserConfig, cls), dict())
 
     @classmethod
     def get_class(cls):
-        return type("ZinoV1Config", (OptionalUserConfig, ServerV1Config, Options, cls))
+        return type("ZinoV1Config", (OptionalUserConfig, cls), dict())
 
     @classmethod
     def from_dict(cls, config_dict, section=DEFAULT_SECTION):
         connection = config_dict["connections"][section]
         options = config_dict.get("options", {})
         classobj = cls.get_class()
-        return cls(**connection, **options)
+        return classobj(**connection, **options)
 
     @classmethod
     def from_tcl(cls, filename=None, section=DEFAULT_SECTION):
         config_dict = tcl.parse_tcl_config(filename)
         connection, options = _parse_tcl(config_dict, section)
         classobj = cls.get_legacy_class()
-        return cls(**connection, **options)
+        return classobj(**connection, **options)
 
     @classmethod
     def from_toml(cls, filename=None, section=DEFAULT_SECTION):
         config_dict = toml.parse_toml_config(filename)
         return cls.from_dict(config_dict)
 
     def set_userauth(self, username, password):
```

### Comparing `zinolib-1.0.4/src/zinolib/controllers/base.py` & `zinolib-1.1.0/src/zinolib/controllers/base.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/src/zinolib/controllers/zino1.py` & `zinolib-1.1.0/src/zinolib/controllers/zino1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 """
 Get a live Zino 1 session to use::
 
     > from zinolib.config.zino1 import ZinoV1Config
-    > from zinolib.zino1 import Zino1EventManager
+    > from zinolib.controllers.zino1 import Zino1EventManager
     > config = ZinoV1Config.from_tcl('.ritz.tcl', 'default')
     > event_manager = Zino1EventManager.configure(config)
     > event_manager.connect()
 
 The configuration can also be stored in a toml-file::
 
     > config = ZinoV1Config.from_toml('.ritz.toml', 'default')
 
+.. or in a dict with the format::
+
+    > config_dict = {"connections": "default": { "server": ACTUAL CONFIG .. }}
+    > config = ZinoV1Config.from_dict(config_dict, 'default')
+
+Do not initialize ZinoV1Config directly, avoid ``ZinoV1Config(**dict)``.
+
 Authenticate using a username and password from the config-file::
 
     > event_manager.authenticate()
 
 Explicitly autenticate with a username and password::
 
     > event_manager.authenticate(username, password)
@@ -287,15 +294,15 @@
     def close_push_channel(session):
         if hasattr(session.push, '_sock'):
             session.push._sock.close()
         session.push = None
 
     @classmethod
     def close_session(cls, session):
-        cls.close_push_channel()
+        cls.close_push_channel(session)
         session.request.close()
         session.request = None
         return None
 
 
 class EventAdapter:
     FIELD_MAP = {
@@ -481,14 +488,15 @@
 class Zino1EventManager(EventManager):
     # Easily replaced in order to ease testing
     _session_adapter = SessionAdapter
     _event_adapter = EventAdapter
     _history_adapter = HistoryAdapter
     _log_adapter = LogAdapter
     removed_ids: Set[int] = set()
+    config = None
 
     @property
     def is_authenticated(self):
         session_ok = self._verify_session(quiet=True)
         return self.session.request.authenticated if session_ok else False
 
     @property
@@ -509,18 +517,21 @@
                 return False
             raise ValueError
         return True
 
     @classmethod
     def configure(cls, config):
         session = cls._session_adapter.create_session(config)
-        return cls(session)
+        classobj = cls(session)
+        classobj.config = config
+        return classobj
 
     def connect(self):
-        self._verify_session()
+        if not self._verify_session(quiet=True):
+            self.session =  self._session_adapter.create_session(self.config)
         self.session = self._session_adapter.connect_session(self.session)
 
     def connect_push_channel(self):
         self.session = self._session_adapter.connect_push_channel(self.session)
 
     def authenticate(self, username=None, password=None):
         try:
```

### Comparing `zinolib-1.0.4/src/zinolib/event_types.py` & `zinolib-1.1.0/src/zinolib/event_types.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/src/zinolib/ritz.py` & `zinolib-1.1.0/src/zinolib/ritz.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/src/zinolib/utils.py` & `zinolib-1.1.0/src/zinolib/utils.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/src/zinolib/zino_emu.py` & `zinolib-1.1.0/src/zinolib/zino_emu.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/src/zinolib.egg-info/PKG-INFO` & `zinolib-1.1.0/src/zinolib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zinolib
-Version: 1.0.4
+Version: 1.1.0
 Summary: Python interface to Zino
 Author-email: Runar Borge <runar.borge@sikt.no>
 Maintainer-email: Uninett Opensource <opensource@uninett.no>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `zinolib-1.0.4/src/zinolib.egg-info/SOURCES.txt` & `zinolib-1.1.0/src/zinolib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/tests/config/test_tcl.py` & `zinolib-1.1.0/tests/config/test_tcl.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/tests/config/test_toml.py` & `zinolib-1.1.0/tests/config/test_toml.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/tests/config/test_utils.py` & `zinolib-1.1.0/tests/config/test_utils.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/tests/config/test_zino1.py` & `zinolib-1.1.0/tests/config/test_zino1.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,16 +45,16 @@
         "password": "0123456789",
         "server": "example.org",
         "username": "admin",
     }
 
     def manually_create_config(self, connection=None):
         connection = connection or self.example_connection
-        options = {}
-        return ZinoV1Config(**connection, **options)
+        _dict = {"connections": {"default": connection}}
+        return ZinoV1Config.from_dict(_dict)
 
     def test_manually_create_config(self):
         config = self.manually_create_config()
         self.assertEqual(config.port, 8001)
 
     def test_set_userauth(self):
         config = self.manually_create_config()
```

### Comparing `zinolib-1.0.4/tests/ritz/test_default.py` & `zinolib-1.1.0/tests/ritz/test_default.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/tests/ritz/test_slow.py` & `zinolib-1.1.0/tests/ritz/test_slow.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/tests/test_zinolib_controllers_zino1.py` & `zinolib-1.1.0/tests/test_zinolib_controllers_zino1.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/tests/test_zinolib_event_types.py` & `zinolib-1.1.0/tests/test_zinolib_event_types.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/tests/utils.py` & `zinolib-1.1.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.4/tox.ini` & `zinolib-1.1.0/tox.ini`

 * *Files identical despite different names*

