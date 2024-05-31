# Comparing `tmp/airbyte_source_aws_cloudtrail-0.1.7.tar.gz` & `tmp/airbyte_source_aws_cloudtrail-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_aws_cloudtrail-0.1.7.tar", last modified: Fri Apr 26 04:08:08 2024, max compression
+gzip compressed data, was "airbyte_source_aws_cloudtrail-0.1.8.tar", max compression
```

## Comparing `airbyte_source_aws_cloudtrail-0.1.7.tar` & `airbyte_source_aws_cloudtrail-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,8 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 04:08:08.639559 airbyte_source_aws_cloudtrail-0.1.7/
--rw-r--r--   0 root         (0) root         (0)     7603 2024-04-26 04:08:08.639559 airbyte_source_aws_cloudtrail-0.1.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8104 2024-04-26 04:04:47.000000 airbyte_source_aws_cloudtrail-0.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 04:08:08.639559 airbyte_source_aws_cloudtrail-0.1.7/airbyte_source_aws_cloudtrail.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7603 2024-04-26 04:08:08.000000 airbyte_source_aws_cloudtrail-0.1.7/airbyte_source_aws_cloudtrail.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2024-04-26 04:08:08.000000 airbyte_source_aws_cloudtrail-0.1.7/airbyte_source_aws_cloudtrail.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 04:08:08.000000 airbyte_source_aws_cloudtrail-0.1.7/airbyte_source_aws_cloudtrail.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2024-04-26 04:08:08.000000 airbyte_source_aws_cloudtrail-0.1.7/airbyte_source_aws_cloudtrail.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       87 2024-04-26 04:08:08.000000 airbyte_source_aws_cloudtrail-0.1.7/airbyte_source_aws_cloudtrail.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-26 04:08:08.000000 airbyte_source_aws_cloudtrail-0.1.7/airbyte_source_aws_cloudtrail.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 04:08:08.639559 airbyte_source_aws_cloudtrail-0.1.7/integration_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-26 04:04:47.000000 airbyte_source_aws_cloudtrail-0.1.7/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       61 2024-04-26 04:04:47.000000 airbyte_source_aws_cloudtrail-0.1.7/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-04-26 04:04:47.000000 airbyte_source_aws_cloudtrail-0.1.7/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)      387 2024-04-26 04:04:47.000000 airbyte_source_aws_cloudtrail-0.1.7/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)      141 2024-04-26 04:04:47.000000 airbyte_source_aws_cloudtrail-0.1.7/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       61 2024-04-26 04:04:47.000000 airbyte_source_aws_cloudtrail-0.1.7/integration_tests/state.json
--rw-r--r--   0 root         (0) root         (0)     7506 2024-04-26 04:08:08.639559 airbyte_source_aws_cloudtrail-0.1.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      950 2024-04-26 04:08:06.000000 airbyte_source_aws_cloudtrail-0.1.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 04:08:08.639559 airbyte_source_aws_cloudtrail-0.1.7/source_aws_cloudtrail/
--rw-r--r--   0 root         (0) root         (0)     1148 2024-04-26 04:04:47.000000 airbyte_source_aws_cloudtrail-0.1.7/source_aws_cloudtrail/__init__.py
--rw-r--r--   0 root         (0) root         (0)      252 2024-04-26 04:04:47.000000 airbyte_source_aws_cloudtrail-0.1.7/source_aws_cloudtrail/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 04:08:08.639559 airbyte_source_aws_cloudtrail-0.1.7/source_aws_cloudtrail/schemas/
--rw-r--r--   0 root         (0) root         (0)     1728 2024-04-26 04:04:47.000000 airbyte_source_aws_cloudtrail-0.1.7/source_aws_cloudtrail/schemas/management_events.json
--rw-r--r--   0 root         (0) root         (0)     7560 2024-04-26 04:04:47.000000 airbyte_source_aws_cloudtrail-0.1.7/source_aws_cloudtrail/source.py
--rw-r--r--   0 root         (0) root         (0)     1705 2024-04-26 04:04:47.000000 airbyte_source_aws_cloudtrail-0.1.7/source_aws_cloudtrail/spec.json
+-rw-r--r--   0        0        0     4640 2024-05-31 07:56:03.000000 airbyte_source_aws_cloudtrail-0.1.8/README.md
+-rw-r--r--   0        0        0      808 2024-05-31 08:08:04.384081 airbyte_source_aws_cloudtrail-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1148 2024-05-31 07:56:03.000000 airbyte_source_aws_cloudtrail-0.1.8/source_aws_cloudtrail/__init__.py
+-rw-r--r--   0        0        0      252 2024-05-31 07:56:03.000000 airbyte_source_aws_cloudtrail-0.1.8/source_aws_cloudtrail/run.py
+-rw-r--r--   0        0        0     1728 2024-05-31 07:56:03.000000 airbyte_source_aws_cloudtrail-0.1.8/source_aws_cloudtrail/schemas/management_events.json
+-rw-r--r--   0        0        0     7560 2024-05-31 07:56:03.000000 airbyte_source_aws_cloudtrail-0.1.8/source_aws_cloudtrail/source.py
+-rw-r--r--   0        0        0     1705 2024-05-31 07:56:03.000000 airbyte_source_aws_cloudtrail-0.1.8/source_aws_cloudtrail/spec.json
+-rw-r--r--   0        0        0     5400 1970-01-01 00:00:00.000000 airbyte_source_aws_cloudtrail-0.1.8/PKG-INFO
```

### Comparing `airbyte_source_aws_cloudtrail-0.1.7/source_aws_cloudtrail/__init__.py` & `airbyte_source_aws_cloudtrail-0.1.8/source_aws_cloudtrail/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_aws_cloudtrail-0.1.7/source_aws_cloudtrail/schemas/management_events.json` & `airbyte_source_aws_cloudtrail-0.1.8/source_aws_cloudtrail/schemas/management_events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_aws_cloudtrail-0.1.7/source_aws_cloudtrail/source.py` & `airbyte_source_aws_cloudtrail-0.1.8/source_aws_cloudtrail/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_aws_cloudtrail-0.1.7/source_aws_cloudtrail/spec.json` & `airbyte_source_aws_cloudtrail-0.1.8/source_aws_cloudtrail/spec.json`

 * *Files identical despite different names*

