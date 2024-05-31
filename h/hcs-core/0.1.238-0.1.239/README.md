# Comparing `tmp/hcs_core-0.1.238.tar.gz` & `tmp/hcs_core-0.1.239.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs_core-0.1.238.tar", last modified: Tue May 21 18:25:48 2024, max compression
+gzip compressed data, was "hcs_core-0.1.239.tar", last modified: Fri May 31 00:19:11 2024, max compression
```

## Comparing `hcs_core-0.1.238.tar` & `hcs_core-0.1.239.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-21 18:25:48.394477 hcs_core-0.1.238/
--rw-r--r--   0 nanw       (503) staff       (20)     1405 2024-05-21 18:25:48.393404 hcs_core-0.1.238/PKG-INFO
--rw-r--r--   0 nanw       (503) staff       (20)       25 2024-05-14 18:28:08.000000 hcs_core-0.1.238/README.md
--rw-r--r--   0 nanw       (503) staff       (20)        7 2024-05-21 18:25:45.000000 hcs_core-0.1.238/VERSION
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-21 18:25:48.302527 hcs_core-0.1.238/hcs_core/
--rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/__init__.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-21 18:25:48.331886 hcs_core-0.1.238/hcs_core/ctxp/
--rw-r--r--   0 nanw       (503) staff       (20)      790 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/ctxp/__init__.py
--rw-r--r--   0 nanw       (503) staff       (20)     1155 2024-05-20 22:21:06.000000 hcs_core-0.1.238/hcs_core/ctxp/_init.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-21 18:25:48.335147 hcs_core-0.1.238/hcs_core/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (503) staff       (20)     3086 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/ctxp/built_in_cmds/_ut.py
--rw-r--r--   0 nanw       (503) staff       (20)     2388 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (503) staff       (20)     4034 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (503) staff       (20)     2274 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/ctxp/cli_options.py
--rw-r--r--   0 nanw       (503) staff       (20)     5800 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (503) staff       (20)      931 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/ctxp/config.py
--rw-r--r--   0 nanw       (503) staff       (20)     1155 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/ctxp/context.py
--rw-r--r--   0 nanw       (503) staff       (20)    14092 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/ctxp/data_util.py
--rw-r--r--   0 nanw       (503) staff       (20)     2856 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/ctxp/duration.py
--rw-r--r--   0 nanw       (503) staff       (20)     1658 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/ctxp/extension.py
--rw-r--r--   0 nanw       (503) staff       (20)     6805 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/ctxp/fstore.py
--rw-r--r--   0 nanw       (503) staff       (20)     4666 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/ctxp/jsondot.py
--rw-r--r--   0 nanw       (503) staff       (20)     6320 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/ctxp/logger.py
--rw-r--r--   0 nanw       (503) staff       (20)     6714 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/ctxp/profile.py
--rw-r--r--   0 nanw       (503) staff       (20)     1565 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/ctxp/profile_store.py
--rw-r--r--   0 nanw       (503) staff       (20)     1767 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/ctxp/recent.py
--rw-r--r--   0 nanw       (503) staff       (20)     1619 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/ctxp/state.py
--rw-r--r--   0 nanw       (503) staff       (20)     8036 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/ctxp/util.py
--rw-r--r--   0 nanw       (503) staff       (20)     3244 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/ctxp/var_template.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-21 18:25:48.347086 hcs_core-0.1.238/hcs_core/plan/
--rw-r--r--   0 nanw       (503) staff       (20)      203 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/plan/__init__.py
--rw-r--r--   0 nanw       (503) staff       (20)      125 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/plan/actions.py
--rw-r--r--   0 nanw       (503) staff       (20)     1298 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/plan/base_provider.py
--rw-r--r--   0 nanw       (503) staff       (20)      116 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/plan/context.py
--rw-r--r--   0 nanw       (503) staff       (20)    20957 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/plan/core.py
--rw-r--r--   0 nanw       (503) staff       (20)    12950 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/plan/dag.py
--rw-r--r--   0 nanw       (503) staff       (20)     7761 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/plan/helper.py
--rw-r--r--   0 nanw       (503) staff       (20)     5454 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/plan/kop.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-21 18:25:48.349838 hcs_core-0.1.238/hcs_core/plan/provider/
--rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/plan/provider/__init__.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-21 18:25:48.353386 hcs_core-0.1.238/hcs_core/plan/provider/dev/
--rw-r--r--   0 nanw       (503) staff       (20)       30 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/plan/provider/dev/__init__.py
--rw-r--r--   0 nanw       (503) staff       (20)       34 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/plan/provider/dev/_prepare.py
--rw-r--r--   0 nanw       (503) staff       (20)     1982 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/plan/provider/dev/dummy.py
--rw-r--r--   0 nanw       (503) staff       (20)     1104 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/plan/provider/dev/fibonacci.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-21 18:25:48.364718 hcs_core-0.1.238/hcs_core/sglib/
--rw-r--r--   0 nanw       (503) staff       (20)      654 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/sglib/__init__.py
--rw-r--r--   0 nanw       (503) staff       (20)     5169 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/sglib/auth.py
--rw-r--r--   0 nanw       (503) staff       (20)     1796 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/sglib/cli_options.py
--rw-r--r--   0 nanw       (503) staff       (20)     8379 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/sglib/client_util.py
--rw-r--r--   0 nanw       (503) staff       (20)     8053 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/sglib/csp.py
--rw-r--r--   0 nanw       (503) staff       (20)     5167 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/sglib/ez_client.py
--rw-r--r--   0 nanw       (503) staff       (20)      901 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/sglib/hcs_client.py
--rw-r--r--   0 nanw       (503) staff       (20)    10128 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/sglib/login_support.py
--rw-r--r--   0 nanw       (503) staff       (20)      683 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/sglib/payload_util.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-21 18:25:48.386412 hcs_core-0.1.238/hcs_core/util/
--rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/util/__init__.py
--rwxr-xr-x   0 nanw       (503) staff       (20)     2535 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/util/check_license.py
--rw-r--r--   0 nanw       (503) staff       (20)     3482 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/util/duration.py
--rw-r--r--   0 nanw       (503) staff       (20)      838 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/util/exit.py
--rw-r--r--   0 nanw       (503) staff       (20)     1755 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/util/hcs_constants.py
--rw-r--r--   0 nanw       (503) staff       (20)     8395 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/util/job_view.py
--rw-r--r--   0 nanw       (503) staff       (20)     5281 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/util/pki_util.py
--rw-r--r--   0 nanw       (503) staff       (20)     1946 2024-05-21 16:11:22.000000 hcs_core-0.1.238/hcs_core/util/query_util.py
--rw-r--r--   0 nanw       (503) staff       (20)     2958 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/util/scheduler.py
--rw-r--r--   0 nanw       (503) staff       (20)     1239 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/util/ssl_util.py
--rw-r--r--   0 nanw       (503) staff       (20)     1727 2024-05-14 18:28:08.000000 hcs_core-0.1.238/hcs_core/util/versions.py
-drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-21 18:25:48.389858 hcs_core-0.1.238/hcs_core.egg-info/
--rw-r--r--   0 nanw       (503) staff       (20)     1405 2024-05-21 18:25:48.000000 hcs_core-0.1.238/hcs_core.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (503) staff       (20)     1788 2024-05-21 18:25:48.000000 hcs_core-0.1.238/hcs_core.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (503) staff       (20)        1 2024-05-21 18:25:48.000000 hcs_core-0.1.238/hcs_core.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (503) staff       (20)      284 2024-05-21 18:25:48.000000 hcs_core-0.1.238/hcs_core.egg-info/requires.txt
--rw-r--r--   0 nanw       (503) staff       (20)        9 2024-05-21 18:25:48.000000 hcs_core-0.1.238/hcs_core.egg-info/top_level.txt
--rw-r--r--   0 nanw       (503) staff       (20)     1250 2024-05-14 18:28:08.000000 hcs_core-0.1.238/pyproject.toml
--rw-r--r--   0 nanw       (503) staff       (20)      284 2024-05-14 18:28:08.000000 hcs_core-0.1.238/requirements.txt
--rw-r--r--   0 nanw       (503) staff       (20)       38 2024-05-21 18:25:48.394865 hcs_core-0.1.238/setup.cfg
--rw-r--r--   0 nanw       (503) staff       (20)      808 2024-05-14 18:28:08.000000 hcs_core-0.1.238/setup.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-05-31 00:19:11.066874 hcs_core-0.1.239/
+-rw-r--r--   0 nanw       (501) staff       (20)     1306 2024-05-31 00:19:11.062116 hcs_core-0.1.239/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)       25 2024-05-30 19:55:05.000000 hcs_core-0.1.239/README.md
+-rw-r--r--   0 nanw       (501) staff       (20)        7 2024-05-31 00:19:07.000000 hcs_core-0.1.239/VERSION
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-05-31 00:19:10.922840 hcs_core-0.1.239/hcs_core/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-05-31 00:19:10.961752 hcs_core-0.1.239/hcs_core/ctxp/
+-rw-r--r--   0 nanw       (501) staff       (20)      790 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/ctxp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1155 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/ctxp/_init.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-05-31 00:19:10.968265 hcs_core-0.1.239/hcs_core/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3086 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/ctxp/built_in_cmds/_ut.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2388 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4034 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2274 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/ctxp/cli_options.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5800 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (501) staff       (20)      931 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/ctxp/config.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1155 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/ctxp/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)    14092 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/ctxp/data_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2856 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/ctxp/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1658 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/ctxp/extension.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6805 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/ctxp/fstore.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4666 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6320 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/ctxp/logger.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6714 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/ctxp/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1565 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/ctxp/profile_store.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1767 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/ctxp/recent.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1619 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/ctxp/state.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8036 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/ctxp/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3244 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/ctxp/var_template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-05-31 00:19:10.982063 hcs_core-0.1.239/hcs_core/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)      203 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      125 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/plan/actions.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1298 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/plan/base_provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)      116 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/plan/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)    21101 2024-05-30 22:53:43.000000 hcs_core-0.1.239/hcs_core/plan/core.py
+-rw-r--r--   0 nanw       (501) staff       (20)    12950 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/plan/dag.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7761 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/plan/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5454 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/plan/kop.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-05-31 00:19:10.986274 hcs_core-0.1.239/hcs_core/plan/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/plan/provider/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-05-31 00:19:10.997497 hcs_core-0.1.239/hcs_core/plan/provider/dev/
+-rw-r--r--   0 nanw       (501) staff       (20)       30 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/plan/provider/dev/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       34 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/plan/provider/dev/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1982 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/plan/provider/dev/dummy.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1104 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/plan/provider/dev/fibonacci.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-05-31 00:19:11.025835 hcs_core-0.1.239/hcs_core/sglib/
+-rw-r--r--   0 nanw       (501) staff       (20)      654 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/sglib/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5169 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/sglib/auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1796 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/sglib/cli_options.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8337 2024-05-30 20:46:14.000000 hcs_core-0.1.239/hcs_core/sglib/client_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8053 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/sglib/csp.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5167 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/sglib/ez_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      901 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)    10128 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/sglib/login_support.py
+-rw-r--r--   0 nanw       (501) staff       (20)      683 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/sglib/payload_util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-05-31 00:19:11.055599 hcs_core-0.1.239/hcs_core/util/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/util/__init__.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/util/check_license.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3482 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/util/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)      838 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/util/exit.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1755 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/util/hcs_constants.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8395 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/util/job_view.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5281 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/util/pki_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1946 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/util/query_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2958 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/util/scheduler.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1239 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/util/ssl_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1727 2024-05-30 19:55:05.000000 hcs_core-0.1.239/hcs_core/util/versions.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-05-31 00:19:11.058448 hcs_core-0.1.239/hcs_core.egg-info/
+-rw-r--r--   0 nanw       (501) staff       (20)     1306 2024-05-31 00:19:10.000000 hcs_core-0.1.239/hcs_core.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     1788 2024-05-31 00:19:10.000000 hcs_core-0.1.239/hcs_core.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        1 2024-05-31 00:19:10.000000 hcs_core-0.1.239/hcs_core.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      231 2024-05-31 00:19:10.000000 hcs_core-0.1.239/hcs_core.egg-info/requires.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        9 2024-05-31 00:19:10.000000 hcs_core-0.1.239/hcs_core.egg-info/top_level.txt
+-rw-r--r--   0 nanw       (501) staff       (20)     1248 2024-05-30 20:34:31.000000 hcs_core-0.1.239/pyproject.toml
+-rw-r--r--   0 nanw       (501) staff       (20)      231 2024-05-30 20:43:57.000000 hcs_core-0.1.239/requirements.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       38 2024-05-31 00:19:11.067345 hcs_core-0.1.239/setup.cfg
+-rw-r--r--   0 nanw       (501) staff       (20)      808 2024-05-30 19:55:05.000000 hcs_core-0.1.239/setup.py
```

### Comparing `hcs_core-0.1.238/PKG-INFO` & `hcs_core-0.1.239/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 Metadata-Version: 2.1
 Name: hcs-core
-Version: 0.1.238
+Version: 0.1.239
 Summary: Horizon Cloud Service CLI module.
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
 Keywords: Horizon,Horizon Cloud,Horizon Cloud Service,CLI
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: authlib==1.2.1
-Requires-Dist: click>=8.1.3
+Requires-Dist: Authlib>=1.2.1
+Requires-Dist: click>=8.1.7
 Requires-Dist: coloredlogs>=15.0.1
-Requires-Dist: cryptography>=38.0.0
-Requires-Dist: httpx>=0.24.1
-Requires-Dist: packaging>=21.3
-Requires-Dist: PyJWT>=2.6.0
-Requires-Dist: pyOpenSSL>=23.1.1
-Requires-Dist: PyYAML>=6.0
-Requires-Dist: questionary==1.10.0
-Requires-Dist: setuptools>=68.0.0
-Requires-Dist: setuptools_scm==7.1.0
-Requires-Dist: python-ulid>=1.1.0
-Requires-Dist: retry>=0.9.2
-Requires-Dist: graphviz>=0.20.1
-Requires-Dist: rich>=13.4.2
+Requires-Dist: cryptography>=42.0.7
+Requires-Dist: graphviz>=0.20.3
+Requires-Dist: httpx>=0.27.0
+Requires-Dist: packaging>=24.0
 Requires-Dist: portalocker>=2.8.2
+Requires-Dist: PyJWT>=2.8.0
+Requires-Dist: pyOpenSSL>=24.1.0
+Requires-Dist: PyYAML>=6.0.1
+Requires-Dist: questionary>=2.0.1
+Requires-Dist: rich>=13.7.1
+Requires-Dist: setuptools>=70.0.0
 
 hcs-cli core component.
```

### Comparing `hcs_core-0.1.238/hcs_core/ctxp/__init__.py` & `hcs_core-0.1.239/hcs_core/ctxp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/ctxp/_init.py` & `hcs_core-0.1.239/hcs_core/ctxp/_init.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/ctxp/built_in_cmds/_ut.py` & `hcs_core-0.1.239/hcs_core/ctxp/built_in_cmds/_ut.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/ctxp/built_in_cmds/context.py` & `hcs_core-0.1.239/hcs_core/ctxp/built_in_cmds/context.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/ctxp/built_in_cmds/profile.py` & `hcs_core-0.1.239/hcs_core/ctxp/built_in_cmds/profile.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/ctxp/cli_options.py` & `hcs_core-0.1.239/hcs_core/ctxp/cli_options.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/ctxp/cli_processor.py` & `hcs_core-0.1.239/hcs_core/ctxp/cli_processor.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/ctxp/config.py` & `hcs_core-0.1.239/hcs_core/ctxp/config.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/ctxp/context.py` & `hcs_core-0.1.239/hcs_core/ctxp/context.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/ctxp/data_util.py` & `hcs_core-0.1.239/hcs_core/ctxp/data_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/ctxp/duration.py` & `hcs_core-0.1.239/hcs_core/ctxp/duration.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/ctxp/extension.py` & `hcs_core-0.1.239/hcs_core/ctxp/extension.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/ctxp/fstore.py` & `hcs_core-0.1.239/hcs_core/ctxp/fstore.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/ctxp/jsondot.py` & `hcs_core-0.1.239/hcs_core/ctxp/jsondot.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/ctxp/logger.py` & `hcs_core-0.1.239/hcs_core/ctxp/logger.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/ctxp/profile.py` & `hcs_core-0.1.239/hcs_core/ctxp/profile.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/ctxp/profile_store.py` & `hcs_core-0.1.239/hcs_core/ctxp/profile_store.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/ctxp/recent.py` & `hcs_core-0.1.239/hcs_core/ctxp/recent.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/ctxp/state.py` & `hcs_core-0.1.239/hcs_core/ctxp/state.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/ctxp/util.py` & `hcs_core-0.1.239/hcs_core/ctxp/util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/ctxp/var_template.py` & `hcs_core-0.1.239/hcs_core/ctxp/var_template.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/plan/base_provider.py` & `hcs_core-0.1.239/hcs_core/plan/base_provider.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/plan/core.py` & `hcs_core-0.1.239/hcs_core/plan/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,15 +259,20 @@
                 handler.destroy(res_data, res_state, False)
             action = actions.create
 
         new_state = None
         if action == actions.create or action is None:
             kop.start(KOP.MODE.create, handler.eta(actions.create, res_data, res_state))
             if _has_save_state(handler.deploy):
-                new_state = handler.deploy(res_data, res_state, fn_set_state)
+
+                def _hook_set_state(data):
+                    fn_set_state(data)
+                    kop.id(_get_res_text(handler, data))
+
+                new_state = handler.deploy(res_data, res_state, _hook_set_state)
             else:
                 new_state = handler.deploy(res_data, res_state)
             kop.id(_get_res_text(handler, new_state))
         elif action == actions.update:
             kop.id(_get_res_text(handler, res_state))
             kop.start(KOP.MODE.update, handler.eta(actions.update, res_data, res_state))
             if _has_save_state(handler.update):
```

### Comparing `hcs_core-0.1.238/hcs_core/plan/dag.py` & `hcs_core-0.1.239/hcs_core/plan/dag.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/plan/helper.py` & `hcs_core-0.1.239/hcs_core/plan/helper.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/plan/kop.py` & `hcs_core-0.1.239/hcs_core/plan/kop.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/plan/provider/dev/dummy.py` & `hcs_core-0.1.239/hcs_core/plan/provider/dev/dummy.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/plan/provider/dev/fibonacci.py` & `hcs_core-0.1.239/hcs_core/plan/provider/dev/fibonacci.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/sglib/__init__.py` & `hcs_core-0.1.239/hcs_core/sglib/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/sglib/auth.py` & `hcs_core-0.1.239/hcs_core/sglib/auth.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/sglib/cli_options.py` & `hcs_core-0.1.239/hcs_core/sglib/cli_options.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/sglib/client_util.py` & `hcs_core-0.1.239/hcs_core/sglib/client_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         def _get_page(query_string):
             url = self._base_context + "?" + query_string
             # print(url)
             return self._client.get(url)
 
         return PageRequest(_get_page, **kwargs).get()
 
-    def create(self, payload: dict | str, headers: dict = None, **kwargs):
+    def create(self, payload: dict, headers: dict = None, **kwargs):
         url = with_query(f"{self._base_context}", **kwargs)
         # print(url)
         # import json
         # print(json.dumps(payload, indent=4))
         if isinstance(payload, str):
             return self._client.post(url, text=payload, headers=headers)
         if isinstance(payload, dict):
@@ -104,39 +104,39 @@
     def delete(self, id: str, org_id: str, **kwargs):
         if org_id:
             kwargs["org_id"] = org_id
         url = with_query(f"{self._base_context}/{id}", **kwargs)
         # print(url)
         return self._client.delete(url)
 
-    def wait_for_deleted(self, id: str, org_id: str, timeout: str | int, fn_is_error: Callable = None):
+    def wait_for_deleted(self, id: str, org_id: str, timeout: str, fn_is_error: Callable = None):
         name = self._resource_type_name + "/" + id
         fn_get = lambda: self.get(id, org_id)
         return wait_for_res_deleted(name, fn_get, timeout=timeout, fn_is_error=fn_is_error)
 
     def update(self, id: str, org_id: str, data: dict, **kwargs):
         if org_id:
             kwargs["org_id"] = org_id
         url = with_query(f"{self._base_context}/{id}")
         return self._client.patch(url, data)
 
 
-def _parse_timeout(timeout: str | int):
+def _parse_timeout(timeout: str):
     if isinstance(timeout, int):
         return timeout
     if isinstance(timeout, str):
         return duration.to_seconds(timeout)
 
     raise CtxpException(f"Invalid timout. Type={type(timeout).__name__}, value={timeout}")
 
 
 def wait_for_res_deleted(
     resource_name: str,
     fn_get: Callable,
-    timeout: str | int,
+    timeout: str,
     polling_interval_seconds: int = 10,
     fn_is_error: Callable = None,
 ):
     timeout_seconds = _parse_timeout(timeout)
     start = time.time()
     while True:
         t = fn_get()
@@ -157,21 +157,21 @@
             sleep_seconds = polling_interval_seconds
         exit.sleep(sleep_seconds)
 
 
 def wait_for_res_status(
     resource_name: str,
     fn_get: Callable,
-    get_status: str | Callable,
+    get_status: Callable,
     status_map: dict = None,
     is_ready: Callable = None,
     is_error: Callable = None,
     is_transition: Callable = None,
-    timeout: str | int = "10m",
-    polling_interval: str | int = "20s",
+    timeout: str = "10m",
+    polling_interval: str = "20s",
     not_found_as_success: bool = False,
 ):
     timeout_seconds = _parse_timeout(timeout)
     polling_interval_seconds = _parse_timeout(polling_interval)
     if polling_interval_seconds < 3:
         polling_interval_seconds = 3
     start = time.time()
```

### Comparing `hcs_core-0.1.238/hcs_core/sglib/csp.py` & `hcs_core-0.1.239/hcs_core/sglib/csp.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/sglib/ez_client.py` & `hcs_core-0.1.239/hcs_core/sglib/ez_client.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/sglib/hcs_client.py` & `hcs_core-0.1.239/hcs_core/sglib/hcs_client.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/sglib/login_support.py` & `hcs_core-0.1.239/hcs_core/sglib/login_support.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/sglib/payload_util.py` & `hcs_core-0.1.239/hcs_core/sglib/payload_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/util/check_license.py` & `hcs_core-0.1.239/hcs_core/util/check_license.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/util/duration.py` & `hcs_core-0.1.239/hcs_core/util/duration.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/util/exit.py` & `hcs_core-0.1.239/hcs_core/util/exit.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/util/hcs_constants.py` & `hcs_core-0.1.239/hcs_core/util/hcs_constants.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/util/job_view.py` & `hcs_core-0.1.239/hcs_core/util/job_view.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/util/pki_util.py` & `hcs_core-0.1.239/hcs_core/util/pki_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/util/query_util.py` & `hcs_core-0.1.239/hcs_core/util/query_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/util/scheduler.py` & `hcs_core-0.1.239/hcs_core/util/scheduler.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/util/ssl_util.py` & `hcs_core-0.1.239/hcs_core/util/ssl_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core/util/versions.py` & `hcs_core-0.1.239/hcs_core/util/versions.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/hcs_core.egg-info/PKG-INFO` & `hcs_core-0.1.239/hcs_core.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 Metadata-Version: 2.1
 Name: hcs-core
-Version: 0.1.238
+Version: 0.1.239
 Summary: Horizon Cloud Service CLI module.
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
 Keywords: Horizon,Horizon Cloud,Horizon Cloud Service,CLI
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: authlib==1.2.1
-Requires-Dist: click>=8.1.3
+Requires-Dist: Authlib>=1.2.1
+Requires-Dist: click>=8.1.7
 Requires-Dist: coloredlogs>=15.0.1
-Requires-Dist: cryptography>=38.0.0
-Requires-Dist: httpx>=0.24.1
-Requires-Dist: packaging>=21.3
-Requires-Dist: PyJWT>=2.6.0
-Requires-Dist: pyOpenSSL>=23.1.1
-Requires-Dist: PyYAML>=6.0
-Requires-Dist: questionary==1.10.0
-Requires-Dist: setuptools>=68.0.0
-Requires-Dist: setuptools_scm==7.1.0
-Requires-Dist: python-ulid>=1.1.0
-Requires-Dist: retry>=0.9.2
-Requires-Dist: graphviz>=0.20.1
-Requires-Dist: rich>=13.4.2
+Requires-Dist: cryptography>=42.0.7
+Requires-Dist: graphviz>=0.20.3
+Requires-Dist: httpx>=0.27.0
+Requires-Dist: packaging>=24.0
 Requires-Dist: portalocker>=2.8.2
+Requires-Dist: PyJWT>=2.8.0
+Requires-Dist: pyOpenSSL>=24.1.0
+Requires-Dist: PyYAML>=6.0.1
+Requires-Dist: questionary>=2.0.1
+Requires-Dist: rich>=13.7.1
+Requires-Dist: setuptools>=70.0.0
 
 hcs-cli core component.
```

### Comparing `hcs_core-0.1.238/hcs_core.egg-info/SOURCES.txt` & `hcs_core-0.1.239/hcs_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.238/pyproject.toml` & `hcs_core-0.1.239/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "hcs-core"
 description = "Horizon Cloud Service CLI module."
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 authors = [
   { name="Nanw1103", email="nanw1103@gmail.com" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
@@ -26,14 +26,14 @@
 "Bug Tracker" = "https://github.com/vmware/horizon-cloud-service-cli/issues"
 documentation = "https://readthedocs.org"
 repository = "https://github.com/vmware/horizon-cloud-service-cli"
 changelog = "https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md"
 
 [tool.black]
 line-length = 120
-target-version = ['py310']
+target-version = ['py39']
 include = '\.pyi?$'
 extend-exclude = '''
 # A regex preceded with ^/ will apply only to files and directories
 # in the root of the project.
 ^/foo.py  # exclude a file named foo.py in the root of the project (in addition to the defaults)
 '''
```

### Comparing `hcs_core-0.1.238/setup.py` & `hcs_core-0.1.239/setup.py`

 * *Files identical despite different names*

