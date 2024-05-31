# Comparing `tmp/python-esiclient-0.2.6.tar.gz` & `tmp/python-esiclient-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/tzumainn/development/python-esiclient/dist/tmp7ax8jxet/python-esiclient-0.2.6.tar", last modified: Thu Feb  1 15:59:42 2024, max compression
+gzip compressed data, was "/home/tzumainn/development/python-esiclient/dist/tmpytgiwa_h/python-esiclient-0.2.7.tar", last modified: Fri May 31 05:35:45 2024, max compression
```

## Comparing `python-esiclient-0.2.6.tar` & `python-esiclient-0.2.7.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-02-01 15:59:42.000000 python-esiclient-0.2.6/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-02-01 15:59:42.000000 python-esiclient-0.2.6/.github/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-02-01 15:59:42.000000 python-esiclient-0.2.6/.github/workflows/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      612 2023-04-27 16:05:01.000000 python-esiclient-0.2.6/.github/workflows/tests.yml
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-02-01 15:59:42.000000 python-esiclient-0.2.6/doc/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1198 2020-10-19 18:43:00.000000 python-esiclient-0.2.6/doc/commands.md
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-02-01 15:59:42.000000 python-esiclient-0.2.6/esiclient/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-02-01 15:59:42.000000 python-esiclient-0.2.6/esiclient/tests/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-02-01 15:59:42.000000 python-esiclient-0.2.6/esiclient/tests/functional/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-02-01 15:59:42.000000 python-esiclient-0.2.6/esiclient/tests/functional/v1/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2021-11-03 18:37:16.000000 python-esiclient-0.2.6/esiclient/tests/functional/v1/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6459 2021-11-03 18:37:16.000000 python-esiclient-0.2.6/esiclient/tests/functional/v1/test_image.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6375 2021-11-03 18:37:16.000000 python-esiclient-0.2.6/esiclient/tests/functional/v1/test_metalsmith.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5130 2021-11-03 18:37:16.000000 python-esiclient-0.2.6/esiclient/tests/functional/v1/test_network.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    12541 2022-05-25 15:36:04.000000 python-esiclient-0.2.6/esiclient/tests/functional/v1/test_node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    13268 2022-05-25 15:36:04.000000 python-esiclient-0.2.6/esiclient/tests/functional/v1/test_node_network.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    12758 2022-05-25 15:43:46.000000 python-esiclient-0.2.6/esiclient/tests/functional/v1/test_node_volume.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4667 2021-11-03 18:37:16.000000 python-esiclient-0.2.6/esiclient/tests/functional/v1/test_trunk.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4357 2021-11-03 18:37:16.000000 python-esiclient-0.2.6/esiclient/tests/functional/v1/test_volume.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1677 2022-05-25 15:36:04.000000 python-esiclient-0.2.6/esiclient/tests/functional/README.md
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2021-11-03 18:37:16.000000 python-esiclient-0.2.6/esiclient/tests/functional/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    10458 2022-05-25 15:36:04.000000 python-esiclient-0.2.6/esiclient/tests/functional/base.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      539 2022-05-25 15:43:46.000000 python-esiclient-0.2.6/esiclient/tests/functional/test.conf.sample
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    11615 2022-06-16 16:46:46.000000 python-esiclient-0.2.6/esiclient/tests/functional/utils.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-02-01 15:59:42.000000 python-esiclient-0.2.6/esiclient/tests/unit/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-02-01 15:59:42.000000 python-esiclient-0.2.6/esiclient/tests/unit/v1/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-02-01 15:59:42.000000 python-esiclient-0.2.6/esiclient/tests/unit/v1/cluster/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-01-16 17:15:26.000000 python-esiclient-0.2.6/esiclient/tests/unit/v1/cluster/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    20768 2024-02-01 15:56:34.000000 python-esiclient-0.2.6/esiclient/tests/unit/v1/cluster/test_cluster.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    26078 2024-02-01 15:56:34.000000 python-esiclient-0.2.6/esiclient/tests/unit/v1/cluster/test_openshift.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4223 2024-02-01 15:56:34.000000 python-esiclient-0.2.6/esiclient/tests/unit/v1/cluster/test_utils.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-02-01 15:59:42.000000 python-esiclient-0.2.6/esiclient/tests/unit/v1/mdc/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 15:36:04.000000 python-esiclient-0.2.6/esiclient/tests/unit/v1/mdc/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5468 2022-05-25 15:36:04.000000 python-esiclient-0.2.6/esiclient/tests/unit/v1/mdc/test_mdc_node_baremetal.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2021-11-03 18:37:16.000000 python-esiclient-0.2.6/esiclient/tests/unit/v1/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2225 2023-12-11 17:56:52.000000 python-esiclient-0.2.6/esiclient/tests/unit/v1/test_node_console.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    24268 2023-08-29 13:02:25.000000 python-esiclient-0.2.6/esiclient/tests/unit/v1/test_node_network.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    21019 2022-05-25 15:36:04.000000 python-esiclient-0.2.6/esiclient/tests/unit/v1/test_node_volume.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    54264 2023-08-29 13:02:18.000000 python-esiclient-0.2.6/esiclient/tests/unit/v1/test_switch.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    20635 2023-12-11 17:56:52.000000 python-esiclient-0.2.6/esiclient/tests/unit/v1/test_trunk.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2021-11-03 18:37:16.000000 python-esiclient-0.2.6/esiclient/tests/unit/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1442 2021-11-03 18:37:16.000000 python-esiclient-0.2.6/esiclient/tests/unit/base.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    21352 2023-12-11 17:56:52.000000 python-esiclient-0.2.6/esiclient/tests/unit/test_utils.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      732 2021-11-03 18:37:16.000000 python-esiclient-0.2.6/esiclient/tests/unit/utils.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2020-10-19 18:43:00.000000 python-esiclient-0.2.6/esiclient/tests/__init__.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-02-01 15:59:42.000000 python-esiclient-0.2.6/esiclient/v1/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-02-01 15:59:42.000000 python-esiclient-0.2.6/esiclient/v1/cluster/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-01-16 17:15:26.000000 python-esiclient-0.2.6/esiclient/v1/cluster/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    12997 2024-02-01 15:56:34.000000 python-esiclient-0.2.6/esiclient/v1/cluster/cluster.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    18963 2024-02-01 15:56:34.000000 python-esiclient-0.2.6/esiclient/v1/cluster/openshift.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2359 2024-02-01 15:56:34.000000 python-esiclient-0.2.6/esiclient/v1/cluster/utils.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-02-01 15:59:42.000000 python-esiclient-0.2.6/esiclient/v1/mdc/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 15:36:04.000000 python-esiclient-0.2.6/esiclient/v1/mdc/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2114 2022-05-25 15:36:04.000000 python-esiclient-0.2.6/esiclient/v1/mdc/mdc_node_baremetal.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2020-10-19 18:43:00.000000 python-esiclient-0.2.6/esiclient/v1/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1872 2023-12-11 17:56:52.000000 python-esiclient-0.2.6/esiclient/v1/node_console.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    11535 2023-08-29 13:02:25.000000 python-esiclient-0.2.6/esiclient/v1/node_network.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5539 2022-05-25 15:36:14.000000 python-esiclient-0.2.6/esiclient/v1/node_volume.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    17048 2023-08-29 13:02:18.000000 python-esiclient-0.2.6/esiclient/v1/switch.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     7985 2023-12-11 17:56:52.000000 python-esiclient-0.2.6/esiclient/v1/trunk.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      669 2020-10-19 18:43:24.000000 python-esiclient-0.2.6/esiclient/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1819 2020-10-19 18:43:00.000000 python-esiclient-0.2.6/esiclient/plugin.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     8429 2024-01-09 19:18:17.000000 python-esiclient-0.2.6/esiclient/utils.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-02-01 15:59:42.000000 python-esiclient-0.2.6/python_esiclient.egg-info/
--rw-r--r--   0 tzumainn  (3390) tzumainn  (3390)     8077 2024-02-01 15:59:41.000000 python-esiclient-0.2.6/python_esiclient.egg-info/PKG-INFO
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2190 2024-02-01 15:59:42.000000 python-esiclient-0.2.6/python_esiclient.egg-info/SOURCES.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        1 2024-02-01 15:59:41.000000 python-esiclient-0.2.6/python_esiclient.egg-info/dependency_links.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1590 2024-02-01 15:59:41.000000 python-esiclient-0.2.6/python_esiclient.egg-info/entry_points.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        1 2022-05-25 16:14:01.000000 python-esiclient-0.2.6/python_esiclient.egg-info/not-zip-safe
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       47 2024-02-01 15:59:41.000000 python-esiclient-0.2.6/python_esiclient.egg-info/pbr.json
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      361 2024-02-01 15:59:41.000000 python-esiclient-0.2.6/python_esiclient.egg-info/requires.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       10 2024-02-01 15:59:41.000000 python-esiclient-0.2.6/python_esiclient.egg-info/top_level.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       68 2021-11-03 18:37:16.000000 python-esiclient-0.2.6/.stestr.conf
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      360 2024-02-01 15:59:41.000000 python-esiclient-0.2.6/AUTHORS
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2704 2024-02-01 15:59:41.000000 python-esiclient-0.2.6/ChangeLog
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    11357 2022-06-16 16:46:46.000000 python-esiclient-0.2.6/LICENSE
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       16 2022-06-16 16:46:46.000000 python-esiclient-0.2.6/MANIFEST.in
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     7105 2024-01-16 17:15:26.000000 python-esiclient-0.2.6/README.md
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      716 2024-01-16 17:15:26.000000 python-esiclient-0.2.6/requirements.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2432 2024-02-01 15:59:42.000000 python-esiclient-0.2.6/setup.cfg
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      876 2022-06-16 16:46:46.000000 python-esiclient-0.2.6/setup.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      564 2023-08-09 20:26:09.000000 python-esiclient-0.2.6/test-requirements.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      765 2023-04-27 16:05:01.000000 python-esiclient-0.2.6/tox.ini
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     8077 2024-02-01 15:59:42.000000 python-esiclient-0.2.6/PKG-INFO
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-31 05:35:45.000000 python-esiclient-0.2.7/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-31 05:35:45.000000 python-esiclient-0.2.7/.github/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-31 05:35:45.000000 python-esiclient-0.2.7/.github/workflows/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      612 2023-04-27 16:05:01.000000 python-esiclient-0.2.7/.github/workflows/tests.yml
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-31 05:35:45.000000 python-esiclient-0.2.7/doc/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1198 2020-10-19 18:43:00.000000 python-esiclient-0.2.7/doc/commands.md
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-31 05:35:45.000000 python-esiclient-0.2.7/esiclient/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-31 05:35:45.000000 python-esiclient-0.2.7/esiclient/tests/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-31 05:35:45.000000 python-esiclient-0.2.7/esiclient/tests/functional/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-31 05:35:45.000000 python-esiclient-0.2.7/esiclient/tests/functional/v1/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2021-11-03 18:37:16.000000 python-esiclient-0.2.7/esiclient/tests/functional/v1/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6459 2021-11-03 18:37:16.000000 python-esiclient-0.2.7/esiclient/tests/functional/v1/test_image.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6375 2021-11-03 18:37:16.000000 python-esiclient-0.2.7/esiclient/tests/functional/v1/test_metalsmith.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5130 2021-11-03 18:37:16.000000 python-esiclient-0.2.7/esiclient/tests/functional/v1/test_network.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    12541 2022-05-25 15:36:04.000000 python-esiclient-0.2.7/esiclient/tests/functional/v1/test_node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    13268 2022-05-25 15:36:04.000000 python-esiclient-0.2.7/esiclient/tests/functional/v1/test_node_network.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    12758 2022-05-25 15:43:46.000000 python-esiclient-0.2.7/esiclient/tests/functional/v1/test_node_volume.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4667 2021-11-03 18:37:16.000000 python-esiclient-0.2.7/esiclient/tests/functional/v1/test_trunk.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4357 2021-11-03 18:37:16.000000 python-esiclient-0.2.7/esiclient/tests/functional/v1/test_volume.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1677 2022-05-25 15:36:04.000000 python-esiclient-0.2.7/esiclient/tests/functional/README.md
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2021-11-03 18:37:16.000000 python-esiclient-0.2.7/esiclient/tests/functional/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    10458 2022-05-25 15:36:04.000000 python-esiclient-0.2.7/esiclient/tests/functional/base.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      539 2022-05-25 15:43:46.000000 python-esiclient-0.2.7/esiclient/tests/functional/test.conf.sample
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    11615 2022-06-16 16:46:46.000000 python-esiclient-0.2.7/esiclient/tests/functional/utils.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-31 05:35:45.000000 python-esiclient-0.2.7/esiclient/tests/unit/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-31 05:35:45.000000 python-esiclient-0.2.7/esiclient/tests/unit/v1/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-31 05:35:45.000000 python-esiclient-0.2.7/esiclient/tests/unit/v1/cluster/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-01-16 17:15:26.000000 python-esiclient-0.2.7/esiclient/tests/unit/v1/cluster/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    20768 2024-02-01 15:56:34.000000 python-esiclient-0.2.7/esiclient/tests/unit/v1/cluster/test_cluster.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    26078 2024-02-01 15:56:34.000000 python-esiclient-0.2.7/esiclient/tests/unit/v1/cluster/test_openshift.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4223 2024-02-01 15:56:34.000000 python-esiclient-0.2.7/esiclient/tests/unit/v1/cluster/test_utils.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-31 05:35:45.000000 python-esiclient-0.2.7/esiclient/tests/unit/v1/mdc/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 15:36:04.000000 python-esiclient-0.2.7/esiclient/tests/unit/v1/mdc/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5468 2022-05-25 15:36:04.000000 python-esiclient-0.2.7/esiclient/tests/unit/v1/mdc/test_mdc_node_baremetal.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2021-11-03 18:37:16.000000 python-esiclient-0.2.7/esiclient/tests/unit/v1/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2225 2023-12-11 17:56:52.000000 python-esiclient-0.2.7/esiclient/tests/unit/v1/test_node_console.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    24917 2024-05-31 05:35:11.000000 python-esiclient-0.2.7/esiclient/tests/unit/v1/test_node_network.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    21019 2022-05-25 15:36:04.000000 python-esiclient-0.2.7/esiclient/tests/unit/v1/test_node_volume.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    54264 2023-08-29 13:02:18.000000 python-esiclient-0.2.7/esiclient/tests/unit/v1/test_switch.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    20635 2023-12-11 17:56:52.000000 python-esiclient-0.2.7/esiclient/tests/unit/v1/test_trunk.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2021-11-03 18:37:16.000000 python-esiclient-0.2.7/esiclient/tests/unit/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1442 2021-11-03 18:37:16.000000 python-esiclient-0.2.7/esiclient/tests/unit/base.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    21352 2023-12-11 17:56:52.000000 python-esiclient-0.2.7/esiclient/tests/unit/test_utils.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      732 2021-11-03 18:37:16.000000 python-esiclient-0.2.7/esiclient/tests/unit/utils.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2020-10-19 18:43:00.000000 python-esiclient-0.2.7/esiclient/tests/__init__.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-31 05:35:45.000000 python-esiclient-0.2.7/esiclient/v1/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-31 05:35:45.000000 python-esiclient-0.2.7/esiclient/v1/cluster/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-01-16 17:15:26.000000 python-esiclient-0.2.7/esiclient/v1/cluster/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    12997 2024-02-01 15:56:34.000000 python-esiclient-0.2.7/esiclient/v1/cluster/cluster.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    18963 2024-02-01 15:56:34.000000 python-esiclient-0.2.7/esiclient/v1/cluster/openshift.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2359 2024-02-01 15:56:34.000000 python-esiclient-0.2.7/esiclient/v1/cluster/utils.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-31 05:35:45.000000 python-esiclient-0.2.7/esiclient/v1/mdc/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 15:36:04.000000 python-esiclient-0.2.7/esiclient/v1/mdc/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2114 2022-05-25 15:36:04.000000 python-esiclient-0.2.7/esiclient/v1/mdc/mdc_node_baremetal.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2020-10-19 18:43:00.000000 python-esiclient-0.2.7/esiclient/v1/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1872 2023-12-11 17:56:52.000000 python-esiclient-0.2.7/esiclient/v1/node_console.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    12781 2024-05-31 05:35:11.000000 python-esiclient-0.2.7/esiclient/v1/node_network.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5539 2022-05-25 15:36:14.000000 python-esiclient-0.2.7/esiclient/v1/node_volume.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    17048 2023-08-29 13:02:18.000000 python-esiclient-0.2.7/esiclient/v1/switch.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     7985 2023-12-11 17:56:52.000000 python-esiclient-0.2.7/esiclient/v1/trunk.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      669 2020-10-19 18:43:24.000000 python-esiclient-0.2.7/esiclient/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1819 2020-10-19 18:43:00.000000 python-esiclient-0.2.7/esiclient/plugin.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     8429 2024-01-09 19:18:17.000000 python-esiclient-0.2.7/esiclient/utils.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-31 05:35:45.000000 python-esiclient-0.2.7/python_esiclient.egg-info/
+-rw-r--r--   0 tzumainn  (3390) tzumainn  (3390)     8077 2024-05-31 05:35:44.000000 python-esiclient-0.2.7/python_esiclient.egg-info/PKG-INFO
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2190 2024-05-31 05:35:45.000000 python-esiclient-0.2.7/python_esiclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        1 2024-05-31 05:35:44.000000 python-esiclient-0.2.7/python_esiclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1590 2024-05-31 05:35:44.000000 python-esiclient-0.2.7/python_esiclient.egg-info/entry_points.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        1 2022-05-25 16:14:01.000000 python-esiclient-0.2.7/python_esiclient.egg-info/not-zip-safe
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       47 2024-05-31 05:35:44.000000 python-esiclient-0.2.7/python_esiclient.egg-info/pbr.json
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      361 2024-05-31 05:35:44.000000 python-esiclient-0.2.7/python_esiclient.egg-info/requires.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       10 2024-05-31 05:35:44.000000 python-esiclient-0.2.7/python_esiclient.egg-info/top_level.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       68 2021-11-03 18:37:16.000000 python-esiclient-0.2.7/.stestr.conf
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      360 2024-05-31 05:35:44.000000 python-esiclient-0.2.7/AUTHORS
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2788 2024-05-31 05:35:44.000000 python-esiclient-0.2.7/ChangeLog
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    11357 2022-06-16 16:46:46.000000 python-esiclient-0.2.7/LICENSE
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       16 2022-06-16 16:46:46.000000 python-esiclient-0.2.7/MANIFEST.in
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     7105 2024-01-16 17:15:26.000000 python-esiclient-0.2.7/README.md
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      716 2024-01-16 17:15:26.000000 python-esiclient-0.2.7/requirements.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2432 2024-05-31 05:35:45.000000 python-esiclient-0.2.7/setup.cfg
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      876 2022-06-16 16:46:46.000000 python-esiclient-0.2.7/setup.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      564 2023-08-09 20:26:09.000000 python-esiclient-0.2.7/test-requirements.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      765 2023-04-27 16:05:01.000000 python-esiclient-0.2.7/tox.ini
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     8077 2024-05-31 05:35:45.000000 python-esiclient-0.2.7/PKG-INFO
```

### Comparing `python-esiclient-0.2.6/.github/workflows/tests.yml` & `python-esiclient-0.2.7/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/doc/commands.md` & `python-esiclient-0.2.7/doc/commands.md`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/tests/functional/v1/test_image.py` & `python-esiclient-0.2.7/esiclient/tests/functional/v1/test_image.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/tests/functional/v1/test_metalsmith.py` & `python-esiclient-0.2.7/esiclient/tests/functional/v1/test_metalsmith.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/tests/functional/v1/test_network.py` & `python-esiclient-0.2.7/esiclient/tests/functional/v1/test_network.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/tests/functional/v1/test_node.py` & `python-esiclient-0.2.7/esiclient/tests/functional/v1/test_node.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/tests/functional/v1/test_node_network.py` & `python-esiclient-0.2.7/esiclient/tests/functional/v1/test_node_network.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/tests/functional/v1/test_node_volume.py` & `python-esiclient-0.2.7/esiclient/tests/functional/v1/test_node_volume.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/tests/functional/v1/test_trunk.py` & `python-esiclient-0.2.7/esiclient/tests/functional/v1/test_trunk.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/tests/functional/v1/test_volume.py` & `python-esiclient-0.2.7/esiclient/tests/functional/v1/test_volume.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/tests/functional/README.md` & `python-esiclient-0.2.7/esiclient/tests/functional/README.md`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/tests/functional/base.py` & `python-esiclient-0.2.7/esiclient/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/tests/functional/test.conf.sample` & `python-esiclient-0.2.7/esiclient/tests/functional/test.conf.sample`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/tests/functional/utils.py` & `python-esiclient-0.2.7/esiclient/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/tests/unit/v1/cluster/test_cluster.py` & `python-esiclient-0.2.7/esiclient/tests/unit/v1/cluster/test_cluster.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/tests/unit/v1/cluster/test_openshift.py` & `python-esiclient-0.2.7/esiclient/tests/unit/v1/cluster/test_openshift.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/tests/unit/v1/cluster/test_utils.py` & `python-esiclient-0.2.7/esiclient/tests/unit/v1/cluster/test_utils.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/tests/unit/v1/mdc/test_mdc_node_baremetal.py` & `python-esiclient-0.2.7/esiclient/tests/unit/v1/mdc/test_mdc_node_baremetal.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/tests/unit/v1/test_node_console.py` & `python-esiclient-0.2.7/esiclient/tests/unit/v1/test_node_console.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/tests/unit/v1/test_node_network.py` & `python-esiclient-0.2.7/esiclient/tests/unit/v1/test_node_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,26 +76,35 @@
             "fixed_ips": [{"ip_address": "2.2.2.2"}],
             "trunk_details": None
         })
         self.floating_network = utils.create_mock_object({
             "id": "floating_network_id",
             "name": "floating_network"
         })
-        self.floating_ip1 = utils.create_mock_object({
-            "id": "floating_ip_uuid_1",
-            "floating_ip_address": "9.9.9.9",
-            "floating_network_id": "floating_network_id",
-            "port_id": "neutron_port_uuid_1"
-        })
-        self.floating_ip2 = utils.create_mock_object({
+        self.floating_ip = utils.create_mock_object({
             "id": "floating_ip_uuid_2",
             "floating_ip_address": "8.8.8.8",
             "floating_network_id": "floating_network_id",
             "port_id": "neutron_port_uuid_2"
-
+        })
+        self.floating_ip_pfw = utils.create_mock_object({
+            "id": "floating_ip_uuid_1",
+            "floating_ip_address": "9.9.9.9",
+            "floating_network_id": "floating_network_id",
+            "port_id": None
+        })
+        self.pfw1 = utils.create_mock_object({
+            "internal_port": 22,
+            "external_port": 22,
+            "internal_port_id": "neutron_port_uuid_1"
+        })
+        self.pfw2 = utils.create_mock_object({
+            "internal_port": 23,
+            "external_port": 23,
+            "internal_port_id": "neutron_port_uuid_1"
         })
 
         def mock_node_get(node_uuid):
             if node_uuid == "11111111-2222-3333-4444-aaaaaaaaaaaa":
                 return self.node1
             elif node_uuid == "11111111-2222-3333-4444-bbbbbbbbbbbb":
                 return self.node2
@@ -104,29 +113,36 @@
 
         def mock_neutron_port_get(port_uuid):
             if port_uuid == "neutron_port_uuid_1":
                 return self.neutron_port1
             elif port_uuid == "neutron_port_uuid_2":
                 return self.neutron_port2
             return None
-
         self.app.client_manager.network.get_port.\
             side_effect = mock_neutron_port_get
+
+        def mock_neutron_port_forwardings(fip):
+            if fip.id == "floating_ip_uuid_1":
+                return [self.pfw1, self.pfw2]
+            return []
+        self.app.client_manager.network.port_forwardings.\
+            side_effect = mock_neutron_port_forwardings
+
         self.app.client_manager.network.find_network.\
             return_value = self.network
         self.app.client_manager.network.get_network.\
             return_value = self.network
         self.app.client_manager.network.ports.\
             return_value = [self.neutron_port1, self.neutron_port2]
         self.app.client_manager.network.networks.\
             return_value = [self.network, self.floating_network]
         self.app.client_manager.baremetal.node.list.\
             return_value = [self.node1, self.node2]
         self.app.client_manager.network.ips.\
-            return_value = [self.floating_ip1, self.floating_ip2]
+            return_value = [self.floating_ip, self.floating_ip_pfw]
 
     def test_take_action(self):
         self.app.client_manager.baremetal.port.list.\
             return_value = [self.port1, self.port2, self.port3]
 
         arglist = []
         verifylist = []
@@ -134,15 +150,15 @@
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         results = self.cmd.take_action(parsed_args)
         expected = (
           ["Node", "MAC Address", "Port", "Network", "Fixed IP",
            "Floating Network", "Floating IP"],
           [['node1', 'aa:aa:aa:aa:aa:aa', 'neutron_port_1', 'test_network',
-           '1.1.1.1', 'floating_network', '9.9.9.9'],
+           '1.1.1.1', 'floating_network', '9.9.9.9 (22:22,23:23)'],
            ['node2', 'bb:bb:bb:bb:bb:bb', None, None, None, None, None],
            ['node2', 'cc:cc:cc:cc:cc:cc', 'neutron_port_2', 'test_network',
             '2.2.2.2', 'floating_network', '8.8.8.8']]
         )
         self.assertEqual(expected, results)
         self.app.client_manager.baremetal.port.list.\
             assert_called_once_with(detail=True)
@@ -200,15 +216,15 @@
 
         results = self.cmd.take_action(parsed_args)
         expected = (
             ["Node", "MAC Address", "Port", "Network", "Fixed IP",
              "Floating Network", "Floating IP"],
             [["node1", "aa:aa:aa:aa:aa:aa",
               "neutron_port_1", "test_network", "1.1.1.1",
-              "floating_network", "9.9.9.9"],
+              "floating_network", "9.9.9.9 (22:22,23:23)"],
              ["node2", "cc:cc:cc:cc:cc:cc",
               "neutron_port_2", "test_network", "2.2.2.2",
               "floating_network", "8.8.8.8"]]
         )
         self.assertEqual(expected, results)
         self.app.client_manager.baremetal.port.list.\
             assert_called_once_with(detail=True)
```

### Comparing `python-esiclient-0.2.6/esiclient/tests/unit/v1/test_node_volume.py` & `python-esiclient-0.2.7/esiclient/tests/unit/v1/test_node_volume.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/tests/unit/v1/test_switch.py` & `python-esiclient-0.2.7/esiclient/tests/unit/v1/test_switch.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/tests/unit/v1/test_trunk.py` & `python-esiclient-0.2.7/esiclient/tests/unit/v1/test_trunk.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/tests/unit/base.py` & `python-esiclient-0.2.7/esiclient/tests/unit/base.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/tests/unit/test_utils.py` & `python-esiclient-0.2.7/esiclient/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/tests/unit/utils.py` & `python-esiclient-0.2.7/esiclient/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/v1/cluster/cluster.py` & `python-esiclient-0.2.7/esiclient/v1/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/v1/cluster/openshift.py` & `python-esiclient-0.2.7/esiclient/v1/cluster/openshift.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/v1/cluster/utils.py` & `python-esiclient-0.2.7/esiclient/v1/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/v1/mdc/mdc_node_baremetal.py` & `python-esiclient-0.2.7/esiclient/v1/mdc/mdc_node_baremetal.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/v1/node_console.py` & `python-esiclient-0.2.7/esiclient/v1/node_console.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/v1/node_network.py` & `python-esiclient-0.2.7/esiclient/v1/node_network.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,23 @@
             '--network',
             dest='network',
             metavar='<network>',
             help=_("Filter by this network (name or UUID).")
         )
         return parser
 
+    def _get_ports(self, neutron_client, network=None):
+        if network:
+            filter_network = neutron_client.find_network(network)
+            neutron_ports = list(neutron_client.ports(
+                network_id=filter_network.id))
+        else:
+            neutron_ports = list(neutron_client.ports())
+        return neutron_ports
+
     def take_action(self, parsed_args):
         self.log.debug("take_action(%s)", parsed_args)
 
         ironic_client = self.app.client_manager.baremetal
         neutron_client = self.app.client_manager.network
 
         if parsed_args.node:
@@ -63,26 +72,41 @@
                 f2 = executor.submit(ironic_client.node.list)
                 ports = f1.result()
                 nodes = f2.result()
 
         filter_network = None
         if parsed_args.network:
             filter_network = neutron_client.find_network(parsed_args.network)
-            neutron_ports = list(neutron_client.ports(
-                network_id=filter_network.id))
-        else:
-            neutron_ports = list(neutron_client.ports())
 
-        floating_ips = list(neutron_client.ips())
-
-        networks = list(neutron_client.networks())
-        networks_dict = {n.id: n for n in networks}
+        # base network information
+        with concurrent.futures.ThreadPoolExecutor() as executor:
+            f1 = executor.submit(neutron_client.ips)
+            f2 = executor.submit(neutron_client.networks)
+            f3 = executor.submit(
+                self._get_ports, neutron_client, filter_network)
+            floating_ips = list(f1.result())
+            networks = list(f2.result())
+            networks_dict = {n.id: n for n in networks}
+            neutron_ports = f3.result()
+
+        # update floating IP list to include port forwarding information
+        for fip in floating_ips:
+            # no need to do this for floating IPs associated with a port,
+            # as port forwarding is irrelevant in such a case
+            if not fip.port_id:
+                pfws = list(neutron_client.port_forwardings(fip))
+                if len(pfws):
+                    fip.port_id = pfws[0].internal_port_id
+                    pfw_ports = ["%s:%s" % (pfw.internal_port,
+                                            pfw.external_port)
+                                 for pfw in pfws]
+                    fip.floating_ip_address = "%s (%s)" % (
+                        fip.floating_ip_address, ','.join(pfw_ports))
 
         data = []
-
         for port in ports:
             if not parsed_args.node:
                 node_name = next((node for node in nodes
                                   if node.uuid == port.node_uuid), None).name
 
             neutron_port_id = port.internal_info.get('tenant_vif_port_id')
             neutron_port = None
```

### Comparing `python-esiclient-0.2.6/esiclient/v1/node_volume.py` & `python-esiclient-0.2.7/esiclient/v1/node_volume.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/v1/switch.py` & `python-esiclient-0.2.7/esiclient/v1/switch.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/v1/trunk.py` & `python-esiclient-0.2.7/esiclient/v1/trunk.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/__init__.py` & `python-esiclient-0.2.7/esiclient/__init__.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/plugin.py` & `python-esiclient-0.2.7/esiclient/plugin.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/esiclient/utils.py` & `python-esiclient-0.2.7/esiclient/utils.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/python_esiclient.egg-info/PKG-INFO` & `python-esiclient-0.2.7/python_esiclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-esiclient
-Version: 0.2.6
+Version: 0.2.7
 Summary: ESI client
 Home-page: UNKNOWN
 Author: ESI
 Author-email: esi@lists.massopen.cloud
 License: Apache License, Version 2.0
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `python-esiclient-0.2.6/python_esiclient.egg-info/SOURCES.txt` & `python-esiclient-0.2.7/python_esiclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/python_esiclient.egg-info/entry_points.txt` & `python-esiclient-0.2.7/python_esiclient.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/ChangeLog` & `python-esiclient-0.2.7/ChangeLog`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+0.2.7
+-----
+
+* Update \`node network list\` to include floating IP port forwarding
+
 0.2.6
 -----
 
 * Updated openshift orchestration to cluster paradigm
 
 0.2.5
 -----
```

### Comparing `python-esiclient-0.2.6/LICENSE` & `python-esiclient-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/README.md` & `python-esiclient-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/requirements.txt` & `python-esiclient-0.2.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/setup.cfg` & `python-esiclient-0.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/setup.py` & `python-esiclient-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/test-requirements.txt` & `python-esiclient-0.2.7/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/tox.ini` & `python-esiclient-0.2.7/tox.ini`

 * *Files identical despite different names*

### Comparing `python-esiclient-0.2.6/PKG-INFO` & `python-esiclient-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-esiclient
-Version: 0.2.6
+Version: 0.2.7
 Summary: ESI client
 Home-page: UNKNOWN
 Author: ESI
 Author-email: esi@lists.massopen.cloud
 License: Apache License, Version 2.0
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

