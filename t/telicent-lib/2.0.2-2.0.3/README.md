# Comparing `tmp/telicent_lib-2.0.2.tar.gz` & `tmp/telicent_lib-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telicent_lib-2.0.2.tar", last modified: Wed May 22 14:36:34 2024, max compression
+gzip compressed data, was "telicent_lib-2.0.3.tar", last modified: Fri May 31 14:16:21 2024, max compression
```

## Comparing `telicent_lib-2.0.2.tar` & `telicent_lib-2.0.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:36:34.002628 telicent_lib-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)    15078 2024-05-22 14:36:34.002628 telicent_lib-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 14:36:34.002628 telicent_lib-2.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:36:33.994629 telicent_lib-2.0.2/telicent_lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:36:33.994629 telicent_lib-2.0.2/telicent_lib/access/
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/access/edhv1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/access/edhv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/access/security_labels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:36:33.994629 telicent_lib-2.0.2/telicent_lib/access/ukihm/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/access/ukihm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/access/ukihm/edh_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    27204 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/action.py
--rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:36:33.994629 telicent_lib-2.0.2/telicent_lib/config/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/config/configSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/config/configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:36:33.994629 telicent_lib-2.0.2/telicent_lib/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/middleware/decode_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/projector.py
--rw-r--r--   0 runner    (1001) docker     (127)    11105 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/records.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15129 2024-05-22 14:36:30.000000 telicent_lib-2.0.2/telicent_lib/sbom.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:36:33.998628 telicent_lib-2.0.2/telicent_lib/sinks/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/sinks/dataSink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/sinks/dictSink.py
--rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/sinks/kafkaSink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/sinks/listSink.py
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/sinks/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:36:33.998628 telicent_lib-2.0.2/telicent_lib/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/sources/dataSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/sources/deserializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/sources/dictSource.py
--rw-r--r--   0 runner    (1001) docker     (127)    18619 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/sources/kafkaSource.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/sources/listSource.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/telicent_lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:36:33.998628 telicent_lib-2.0.2/telicent_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15078 2024-05-22 14:36:33.000000 telicent_lib-2.0.2/telicent_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-22 14:36:33.000000 telicent_lib-2.0.2/telicent_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:36:33.000000 telicent_lib-2.0.2/telicent_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-22 14:36:33.000000 telicent_lib-2.0.2/telicent_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 14:36:33.000000 telicent_lib-2.0.2/telicent_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:36:33.998628 telicent_lib-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8890 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_decode_token_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_edh_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_generate_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_projector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_protocol_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13170 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_security_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_security_labels_edhv1.py
--rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_serdes.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_sinks.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-22 14:36:28.000000 telicent_lib-2.0.2/tests/test_sources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:16:21.621380 telicent_lib-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    15078 2024-05-31 14:16:21.617380 telicent_lib-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 14:16:21.621380 telicent_lib-2.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:16:21.609380 telicent_lib-2.0.3/telicent_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:16:21.613380 telicent_lib-2.0.3/telicent_lib/access/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/access/edhv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/access/edhv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/access/security_labels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:16:21.613380 telicent_lib-2.0.3/telicent_lib/access/ukihm/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/access/ukihm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/access/ukihm/edh_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27204 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:16:21.613380 telicent_lib-2.0.3/telicent_lib/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/config/configSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/config/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:16:21.613380 telicent_lib-2.0.3/telicent_lib/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/middleware/decode_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/projector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15129 2024-05-31 14:16:18.000000 telicent_lib-2.0.3/telicent_lib/sbom.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:16:21.613380 telicent_lib-2.0.3/telicent_lib/sinks/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/sinks/dataSink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/sinks/dictSink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/sinks/kafkaSink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/sinks/listSink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/sinks/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:16:21.617380 telicent_lib-2.0.3/telicent_lib/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/sources/dataSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/sources/deserializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/sources/dictSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/sources/kafkaSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/sources/listSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/telicent_lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:16:21.617380 telicent_lib-2.0.3/telicent_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15078 2024-05-31 14:16:21.000000 telicent_lib-2.0.3/telicent_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-31 14:16:21.000000 telicent_lib-2.0.3/telicent_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 14:16:21.000000 telicent_lib-2.0.3/telicent_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-31 14:16:21.000000 telicent_lib-2.0.3/telicent_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-31 14:16:21.000000 telicent_lib-2.0.3/telicent_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:16:21.617380 telicent_lib-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8890 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/tests/test_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/tests/test_decode_token_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/tests/test_edh_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/tests/test_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/tests/test_generate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/tests/test_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/tests/test_projector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/tests/test_protocol_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13126 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/tests/test_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/tests/test_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/tests/test_security_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/tests/test_security_labels_edhv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15540 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/tests/test_serdes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/tests/test_sinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-31 14:16:16.000000 telicent_lib-2.0.3/tests/test_sources.py
```

### Comparing `telicent_lib-2.0.2/LICENSE` & `telicent_lib-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/PKG-INFO` & `telicent_lib-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telicent-lib
-Version: 2.0.2
+Version: 2.0.3
 Summary: A helper package for building Adapters, Mappers and Projectors for Telicent Core
 Author-email: Telicent Ltd <admin@telicent.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `telicent_lib-2.0.2/README.md` & `telicent_lib-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/pyproject.toml` & `telicent_lib-2.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2.0", "wheel==0.41.3", "pip-tools==7.3.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "telicent-lib"
-version = "2.0.2"
+version = "2.0.3"
 authors = [{name = "Telicent Ltd", email = "admin@telicent.io"}]
 description = "A helper package for building Adapters, Mappers and Projectors for Telicent Core"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 readme = "README.md"
 dependencies = [
     "colored==1.4.4",
```

### Comparing `telicent_lib-2.0.2/telicent_lib/__init__.py` & `telicent_lib-2.0.3/telicent_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/telicent_lib/access/__init__.py` & `telicent_lib-2.0.3/telicent_lib/access/__init__.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/telicent_lib/access/edhv1.py` & `telicent_lib-2.0.3/telicent_lib/access/edhv1.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/telicent_lib/access/edhv2.py` & `telicent_lib-2.0.3/telicent_lib/access/edhv2.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/telicent_lib/access/security_labels.py` & `telicent_lib-2.0.3/telicent_lib/access/security_labels.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/telicent_lib/access/ukihm/__init__.py` & `telicent_lib-2.0.3/telicent_lib/access/ukihm/__init__.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/telicent_lib/access/ukihm/edh_model.py` & `telicent_lib-2.0.3/telicent_lib/access/ukihm/edh_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from datetime import datetime, timezone
-from typing import List, Optional, Union
 
 from pydantic import AwareDatetime, BaseModel, PlainSerializer
 from typing_extensions import Annotated
 
 from telicent_lib.access.edhv2 import EDHSecurityLabelsV2
 from telicent_lib.access.security_labels import SecurityLabelBuilder
 
@@ -39,28 +38,28 @@
         builder.add_multiple(EDHSecurityLabelsV2.AND_GROUPS.value, *self.andGroups)
         builder.add_multiple(EDHSecurityLabelsV2.OR_GROUPS.value, *self.orGroups)
 
         return builder.build()
 
 
 class EDHModel(EDHMixin):
-    apiVersion: Union[str, None] = "v1alpha"
-    specification: Union[str, None] = "UKIC v3.0"
+    apiVersion: str | None = "v1alpha"
+    specification: str | None = "UKIC v3.0"
     identifier: str
     classification: str
-    permittedOrgs: List[str]
-    permittedNats: List[str]
-    orGroups: List[str]
-    andGroups: List[str]
-
-    createdDateTime: Optional[SerialisableDt] = DEFAULT_OPTIONAL_DT
-    originator: Optional[str] = None
-    custodian: Optional[str] = None
-    policyRef: Optional[str] = None
-    dataSet: List[str]
-    authRef: List[str]
-    dispositionDate: Optional[SerialisableDt] = DEFAULT_OPTIONAL_DT
-    dispositionProcess: Optional[str] = None
-    dissemination: List[str]
+    permittedOrgs: list[str]
+    permittedNats: list[str]
+    orGroups: list[str]
+    andGroups: list[str]
+
+    createdDateTime: SerialisableDt | None = DEFAULT_OPTIONAL_DT
+    originator: str | None = None
+    custodian: str | None = None
+    policyRef: str | None = None
+    dataSet: list[str]
+    authRef: list[str]
+    dispositionDate: SerialisableDt | None = DEFAULT_OPTIONAL_DT
+    dispositionProcess: str | None = None
+    dissemination: list[str]
 
     def build_security_labels(self):
         return super().build_security_labels()
```

### Comparing `telicent_lib-2.0.2/telicent_lib/action.py` & `telicent_lib-2.0.3/telicent_lib/action.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/telicent_lib/adapter.py` & `telicent_lib-2.0.3/telicent_lib/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import uuid
-from typing import Iterable, Union
+from typing import Iterable
 
 from colored import fore
 from opentelemetry.trace.propagation.tracecontext import TraceContextTextMapPropagator
 
 from telicent_lib.access import EDHModel
 from telicent_lib.action import DEFAULT_REPORTING_BATCH_SIZE, OutputAction
 from telicent_lib.records import Record, RecordAdapter, RecordUtils
@@ -119,15 +119,15 @@
     function cannot do as easily.
     """
 
     def __init__(self, target: DataSink, adapter_function: RecordAdapter,
                  text_colour=fore.LIGHT_CYAN, reporting_batch_size=DEFAULT_REPORTING_BATCH_SIZE,
                  name: str = None, source_name: str = None, source_type: str = None, has_reporter: bool = True,
                  reporter_sink=None, has_error_handler: bool = True, error_handler=None,
-                 policy_information: Union[dict, None] = None,
+                 policy_information: dict | None = None,
                  **adapter_args):
         """
         Creates a new automatic adapter that imports data into a data sink.
 
         :param target: A sink for the data
         :type target: DataSink
         :param adapter_function:
```

### Comparing `telicent_lib-2.0.2/telicent_lib/config/__init__.py` & `telicent_lib-2.0.3/telicent_lib/config/__init__.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/telicent_lib/config/configSource.py` & `telicent_lib-2.0.3/telicent_lib/config/configSource.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/telicent_lib/config/configurator.py` & `telicent_lib-2.0.3/telicent_lib/config/configurator.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/telicent_lib/errors.py` & `telicent_lib-2.0.3/telicent_lib/errors.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/telicent_lib/exceptions.py` & `telicent_lib-2.0.3/telicent_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/telicent_lib/logging.py` & `telicent_lib-2.0.3/telicent_lib/logging.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/telicent_lib/mapper.py` & `telicent_lib-2.0.3/telicent_lib/mapper.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/telicent_lib/middleware/__init__.py` & `telicent_lib-2.0.3/telicent_lib/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/telicent_lib/middleware/decode_token.py` & `telicent_lib-2.0.3/telicent_lib/middleware/decode_token.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/telicent_lib/projector.py` & `telicent_lib-2.0.3/telicent_lib/projector.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/telicent_lib/records.py` & `telicent_lib-2.0.3/telicent_lib/records.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import collections
 import json
-from typing import Any, Dict, Iterable, List, Optional, Protocol, Tuple, Union, runtime_checkable
+from typing import Any, Iterable, Protocol, runtime_checkable
 
 __license__ = """
 Copyright (c) Telicent Ltd.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
@@ -30,15 +30,15 @@
 
 @runtime_checkable
 class RecordMapper(Protocol):
     """
     Represents a callable function that maps an input record into zero or more output records.
     """
 
-    def __call__(self, record: Record) -> Union[Record, List[Record], None]:
+    def __call__(self, record: Record) -> Record | list[Record] | None:
         """
         Maps an input record into zero or more output records.
         :param record: Input record
         :type record: Record
         :return: Output record(s)
         """
         pass
@@ -76,37 +76,37 @@
 
 class RecordUtils:
     """
     Provides static utility methods for working with Record tuples
     """
 
     @staticmethod
-    def __decode_header_value__(value: Any) -> Optional[str]:
+    def __decode_header_value__(value: Any) -> str | None:
         if value is None:
             return None
 
         if isinstance(value, str):
             return value
         elif isinstance(value, bytes):
             return value.decode("utf-8")
         else:
             raise TypeError("Header value is not a str/bytes")
 
     @staticmethod
-    def __encode_header_value(value: Union[str, bytes, dict, None]) -> Any:
+    def __encode_header_value(value: str | bytes | dict | None) -> Any:
         if value is None:
             return None
         elif isinstance(value, bytes):
             return value
         elif isinstance(value, dict):
             return json.dumps(value).encode("utf-8")
         return value.encode("utf-8")
 
     @staticmethod
-    def get_first_header(record: Record, header: str) -> Optional[str]:
+    def get_first_header(record: Record, header: str) -> str | None:
         """
         Gets the first value for a given header (if any)
 
         :param record: Record
         :param header:
             Header whose value you want to retrieve, this is matched with the record header keys in a case-insensitive
             manner
@@ -123,15 +123,15 @@
         for key, value in record.headers:
             if key.casefold() == header:
                 return RecordUtils.__decode_header_value__(value)
 
         return None
 
     @staticmethod
-    def get_last_header(record: Record, header: str) -> Optional[str]:
+    def get_last_header(record: Record, header: str) -> str | None:
         """
         Gets the last value for a given header (if any)
 
         :param record: Record
         :param header:
             Header whose value you want to retrieve, this is matched with record header keys in a case-insensitive
             manner
@@ -139,15 +139,15 @@
         """
         try:
             return list(RecordUtils.get_headers(record, header))[-1]
         except IndexError:
             return None
 
     @staticmethod
-    def get_headers(record: Record, header: str) -> Iterable[Optional[str]]:
+    def get_headers(record: Record, header: str) -> Iterable[str | None]:
         """
         Gets all values for a given header (if any)
 
         :param record: Record
         :param header:
             Header whose value(s) you want to retrieve, this is matched with the record header keys in a
             case-insensitive manner
@@ -163,15 +163,15 @@
 
         for key, value in record.headers:
             if key.casefold() == header:
                 yield RecordUtils.__decode_header_value__(value)
         return
 
     @staticmethod
-    def add_header(record: Record, header: str, value: Union[str, dict, bytes, None]) -> Record:
+    def add_header(record: Record, header: str, value: str | dict | bytes | None) -> Record:
         """
         Adds a header, this produces a new copy of the Record with the new header added
 
         :param record: Record
         :param header: Header key to add
         :param value: Header value to add
         :return: New record with the header added
@@ -187,15 +187,15 @@
             for key, current_value in record.headers:
                 new_headers.append((key, current_value))
 
         new_headers.append((header, RecordUtils.__encode_header_value(value)))
         return Record(new_headers, record.key, record.value, record.raw)
 
     @staticmethod
-    def add_headers(record: Record, headers: List[Tuple[str, Union[str, bytes, dict, None]]]) -> Record:
+    def add_headers(record: Record, headers: list[tuple[str, str | bytes | dict | None]]) -> Record:
         """
         Adds multiple headers, this produces a new copy of the Record with the new headers added
 
         :param record: Record
         :param headers: New headers
         :return: New record with the headers added
         """
@@ -214,15 +214,15 @@
             for key, value in record.headers:
                 new_headers.append((key, value))
         for key, value in headers:
             new_headers.append((key, RecordUtils.__encode_header_value(value)))
         return Record(new_headers, record.key, record.value, record.raw)
 
     @staticmethod
-    def replace_or_add_header(record: Record, header: str, value: Union[str, bytes, None] = None) -> Record:
+    def replace_or_add_header(record: Record, header: str, value: str | bytes | None = None) -> Record:
         """
         Replaces or adds a header to a new copy of the record.
 
         If the header already exists the first instance of it has its value updated.  If the header does not exist then
         it is added as a new header.
         :param record: Record
         :param header: Header key
@@ -246,15 +246,15 @@
                     new_headers.append((key, current_value))
         if not replaced:
             new_headers.append((header, value))
 
         return Record(new_headers, record.key, record.value, record.raw)
 
     @staticmethod
-    def remove_header(record: Record, header: str, value: Union[str, bytes, None] = None) -> Record:
+    def remove_header(record: Record, header: str, value: str | bytes | None = None) -> Record:
         """
         Removes a header, this produces a new copy of the Record with the header removed
 
         :param record: Record
         :param header: Header key to remove, this is matched in a case-insensitive manner
         :param value:
             Header value to remove, if None then any header with the key is removed, if a value then only a header with
@@ -278,23 +278,23 @@
                 new_headers.append((key, current_value))
             elif value is not None and value != current_value:
                 new_headers.append((key, current_value))
 
         return Record(new_headers, record.key, record.value, record.raw)
 
     @staticmethod
-    def to_headers(headers: Dict[str, Union[str, bytes, None]],
-                   existing_headers: List[Tuple[str, Union[str, bytes, None]]] = None) \
-            -> List[Tuple[str, Union[str, bytes, None]]]:
+    def to_headers(headers: dict[str, str | bytes | None],
+                   existing_headers: list[tuple[str, str | bytes | None]] = None) \
+            -> list[tuple[str, str | bytes | None]]:
         """
         Convenience function to convert from a Python dictionary into the header list format that Record's use
 
         :param headers: Dictionary of headers
         :param existing_headers: Existing headers to append the given headers to, a copy of these will be taken
-        :return: List of header tuples
+        :return: list of header tuples
         """
         if headers is None:
             if existing_headers is None:
                 return []
             else:
                 return existing_headers
```

### Comparing `telicent_lib-2.0.2/telicent_lib/reporter.py` & `telicent_lib-2.0.3/telicent_lib/reporter.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/telicent_lib/sbom.json` & `telicent_lib-2.0.3/telicent_lib/sbom.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9198682177197802%*

 * *Differences: {"'components'": "{21: {'description': 'requirements line 51: typing-extensions==4.12.0', 'purl': "*

 * *                 "'pkg:pypi/typing-extensions@4.12.0', 'version': '4.12.0'}, 25: {'description': "*

 * *                 "'requirements line 62: zipp==3.19.0', 'purl': 'pkg:pypi/zipp@3.19.0', 'version': "*

 * *                 "'3.19.0'}}",*

 * * "'metadata'": "{'timestamp': '2024-05-31T14:15:45.956735+00:00', 'tools': {1: {'version': "*

 * *               "'7.4.0'}}}",*

 * * "'serialNumber'": "'urn:uuid:946281b8-e0fd-4414-867f-441f2 […]*

```diff
@@ -315,26 +315,26 @@
             "name": "six",
             "purl": "pkg:pypi/six@1.16.0",
             "type": "library",
             "version": "1.16.0"
         },
         {
             "bom-ref": "requirements-L51",
-            "description": "requirements line 51: typing-extensions==4.11.0",
+            "description": "requirements line 51: typing-extensions==4.12.0",
             "externalReferences": [
                 {
                     "comment": "implicit dist url",
                     "type": "distribution",
                     "url": "https://pypi.org/simple/typing-extensions/"
                 }
             ],
             "name": "typing-extensions",
-            "purl": "pkg:pypi/typing-extensions@4.11.0",
+            "purl": "pkg:pypi/typing-extensions@4.12.0",
             "type": "library",
-            "version": "4.11.0"
+            "version": "4.12.0"
         },
         {
             "bom-ref": "requirements-L56",
             "description": "requirements line 56: urllib3==2.2.1",
             "externalReferences": [
                 {
                     "comment": "implicit dist url",
@@ -375,26 +375,26 @@
             "name": "wrapt",
             "purl": "pkg:pypi/wrapt@1.16.0",
             "type": "library",
             "version": "1.16.0"
         },
         {
             "bom-ref": "requirements-L62",
-            "description": "requirements line 62: zipp==3.18.2",
+            "description": "requirements line 62: zipp==3.19.0",
             "externalReferences": [
                 {
                     "comment": "implicit dist url",
                     "type": "distribution",
                     "url": "https://pypi.org/simple/zipp/"
                 }
             ],
             "name": "zipp",
-            "purl": "pkg:pypi/zipp@3.18.2",
+            "purl": "pkg:pypi/zipp@3.19.0",
             "type": "library",
-            "version": "3.18.2"
+            "version": "3.19.0"
         }
     ],
     "dependencies": [
         {
             "ref": "requirements-L11"
         },
         {
@@ -470,15 +470,15 @@
             "ref": "requirements-L7"
         },
         {
             "ref": "requirements-L9"
         }
     ],
     "metadata": {
-        "timestamp": "2024-05-22T14:35:51.571327+00:00",
+        "timestamp": "2024-05-31T14:15:45.956735+00:00",
         "tools": [
             {
                 "externalReferences": [
                     {
                         "type": "build-system",
                         "url": "https://github.com/CycloneDX/cyclonedx-python/actions"
                     },
@@ -548,15 +548,15 @@
                     {
                         "type": "website",
                         "url": "https://github.com/CycloneDX/cyclonedx-python-lib/#readme"
                     }
                 ],
                 "name": "cyclonedx-python-lib",
                 "vendor": "CycloneDX",
-                "version": "7.3.4"
+                "version": "7.4.0"
             }
         ]
     },
-    "serialNumber": "urn:uuid:f74a1260-447a-4def-a456-91afe45a6504",
+    "serialNumber": "urn:uuid:946281b8-e0fd-4414-867f-441f2d572028",
     "specVersion": "1.5",
     "version": 1
 }
```

### Comparing `telicent_lib-2.0.2/telicent_lib/sinks/__init__.py` & `telicent_lib-2.0.3/telicent_lib/sinks/__init__.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/telicent_lib/sinks/dataSink.py` & `telicent_lib-2.0.3/telicent_lib/sinks/dataSink.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/telicent_lib/sinks/dictSink.py` & `telicent_lib-2.0.3/telicent_lib/sinks/dictSink.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict
+from typing import Any
 
 from telicent_lib import Record
 from telicent_lib.sinks import DataSink
 
 __license__ = """
 Copyright (c) Telicent Ltd.
 
@@ -23,20 +23,20 @@
 class DictionarySink(DataSink):
     """
     A Data Sink backed by a Dictionary intended for test and development purposes only
     """
 
     def __init__(self):
         super().__init__("Dictionary")
-        self.data: Dict[Any, Any] = {}
+        self.data: dict[Any, Any] = {}
 
     def send(self, record: Record):
         if record is None:
             return
         self.data[record.key] = record.value
 
-    def get(self) -> Dict[Any, Any]:
+    def get(self) -> dict[Any, Any]:
         """Gets the underlying dictionary"""
         return self.data
 
     def __str__(self):
         return "In-Memory Dictionary"
```

### Comparing `telicent_lib-2.0.2/telicent_lib/sinks/kafkaSink.py` & `telicent_lib-2.0.3/telicent_lib/sinks/kafkaSink.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,17 +88,17 @@
         :param topic: Kafka topic to send data to
         :type topic: str
         :param broker: Deprecated, please specify broker through kafka_config
         :type broker: str
         :param kafka_config: Kafka configuration
         :type kafka_config: dict
         :param key_serializer: A serialization function/class used to serialize the record keys to bytes
-        :type key_serializer: Union[SerializerFunction, Serializer]
+        :type key_serializer: SerializerFunction | Serializer
         :param value_serializer: A serialization function/class used to serialize the record values to bytes
-        :type value_serializer: Union[SerializerFunction, Serializer]
+        :type value_serializer: SerializerFunction | Serializer
         """
         if broker is not None:
             warnings.warn(
                 "Parameter 'broker' has been deprecated. Please provide 'kafka_config'.",
                 DeprecationWarning,
                 stacklevel=2
             )
```

### Comparing `telicent_lib-2.0.2/telicent_lib/sinks/listSink.py` & `telicent_lib-2.0.3/telicent_lib/sinks/listSink.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 
-from typing import List
 
 from telicent_lib.records import Record
 from telicent_lib.sinks import DataSink
 
 __license__ = """
 Copyright (c) Telicent Ltd.
 
@@ -24,20 +23,20 @@
 class ListSink(DataSink):
     """
     A Data Sink backed by a List intended for test and development purposes only
     """
 
     def __init__(self):
         super().__init__("List")
-        self.data: List[Record] = []
+        self.data: list[Record] = []
 
     def send(self, record: Record):
         if record is None:
             return
         self.data.append(record)
 
-    def get(self) -> List[Record]:
+    def get(self) -> list[Record]:
         """Gets the underlying list"""
         return self.data
 
     def __str__(self):
         return "In-Memory List"
```

### Comparing `telicent_lib-2.0.2/telicent_lib/sinks/serializers.py` & `telicent_lib-2.0.3/telicent_lib/sinks/serializers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import zlib
-from typing import Any, Optional, Protocol, runtime_checkable
+from typing import Any, Protocol, runtime_checkable
 
 # noinspection PyProtectedMember
 from confluent_kafka.serialization import Serializer
 from rdflib import Graph
 
 __license__ = """
 Copyright (c) Telicent Ltd.
@@ -25,51 +25,51 @@
 
 @runtime_checkable
 class SerializerFunction(Protocol):
     """
     A protocol for serializer functions that can encode Python objects into bytes
     """
 
-    def __call__(self, data: Any) -> Optional[bytes]:
+    def __call__(self, data: Any) -> bytes | None:
         """
         Encodes a Python object into bytes
         :param data: Python Object
         :return: Byte representation of the object
         """
         pass
 
 
 class Serializers:
     """
     Provides some built-in serializer functions
     """
 
     @staticmethod
-    def to_zipped_binary(data: Any) -> Optional[bytes]:
+    def to_zipped_binary(data: Any) -> bytes | None:
         """
         Serializes data by first converting it into bytes and then compressing those bytes with zlib
 
         :param data: Data to encode
         :return: Compressed data
         :rtype: bytes
         """
         if data is None:
             return None
-        binary_data: Optional[bytes]
+        binary_data: bytes | None
         if isinstance(data, bytes):
             binary_data = data
         else:
             binary_data = Serializers.to_binary(data)
 
         if binary_data is None:
             return None
         return zlib.compress(binary_data)
 
     @staticmethod
-    def to_binary(data: Any) -> Optional[bytes]:
+    def to_binary(data: Any) -> bytes | None:
         """
         Serializes data into bytes
 
         If the data is already bytes then it is left unchanged.
 
         If the data is a string then it is encoded using UTF-8 encoding.
 
@@ -85,15 +85,15 @@
         if isinstance(data, bytes):
             return data
         if isinstance(data, str):
             return data.encode("utf-8")
         return bytes(data)
 
     @staticmethod
-    def as_is(data: Any) -> Optional[bytes]:
+    def as_is(data: Any) -> bytes | None:
         """
         A serializer that assumes the data is already bytes i.e. assumes the records will already have the relevant
         fields represented as bytes.
 
         If the data is not bytes then a TypeError is raised
 
         :param data: Data
@@ -104,15 +104,15 @@
         if data is None:
             return None
         if not isinstance(data, bytes):
             raise TypeError('Expected data to already be bytes')
         return data
 
     @staticmethod
-    def to_json(data: Any) -> Optional[bytes]:
+    def to_json(data: Any) -> bytes | None:
         """
         A serializer that converts the data into a JSON string and then encodes that into UTF-8 bytes
 
         If the data is None then None is returned
         :param data: Data
         :return: Bytes
         :rtype: bytes
```

### Comparing `telicent_lib-2.0.2/telicent_lib/sources/dataSource.py` & `telicent_lib-2.0.3/telicent_lib/sources/dataSource.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from typing import Iterable, Optional
+from typing import Iterable
 
 from telicent_lib.records import Record
 
 
 class DataSource:
     """Represents a source from which data can be read"""
     def __init__(self, source_name: str = None):
@@ -11,15 +11,15 @@
             raise TypeError("DataSource must be provided a source name")
         self.__source = source_name
 
     def data(self) -> Iterable[Record]:
         """Provides an iterable over the data"""
         raise NotImplementedError
 
-    def remaining(self) -> Optional[int]:
+    def remaining(self) -> int | None:
         """
         Returns the remaining number of records
 
         This may be None if this is unknown.  The return value may also change over time both as records are consumed
         from the data source and if the data source is actively receiving new records.
         """
         return None
```

### Comparing `telicent_lib-2.0.2/telicent_lib/sources/deserializers.py` & `telicent_lib-2.0.3/telicent_lib/sources/deserializers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import json
 import zlib
-from typing import Any, Optional, Protocol, runtime_checkable
+from typing import Any, Protocol, runtime_checkable
 
 # noinspection PyProtectedMember
 from confluent_kafka.serialization import Deserializer
 from rdflib import Dataset
 from rdflib.graph import DATASET_DEFAULT_GRAPH_ID
 
 
 @runtime_checkable
 class DeserializerFunction(Protocol):
     """
     A protocol for deserializer functions that can decode the raw bytes that records are stored as in underlying storage
     into some more useful Python object
     """
 
-    def __call__(self, data: Optional[bytes]) -> Any:
+    def __call__(self, data: bytes | None) -> Any:
         """
         Decodes bytes into any Python object
 
         :param data:
             Bytes, may be None if there is nothing to deserialize and implementations must expect this possibility
         :return: Python object
         """
@@ -28,41 +28,41 @@
 
 class Deserializers:
     """
     Provides some built-in deserializer functions
     """
 
     @staticmethod
-    def unzip_to_string(data: Optional[bytes]) -> Optional[str]:
+    def unzip_to_string(data: bytes | None) -> str | None:
         """
         A deserializer which decompresses the data with zlib and decodes into a string assuming UTF-8 encoding
 
         :param data: The data to decode
         :return: Decoded data
         :rtype: str
         """
         if data is None:
             return None
         return zlib.decompress(data).decode('utf-8')
 
     @staticmethod
-    def binary_to_string(data: Optional[bytes]) -> Optional[str]:
+    def binary_to_string(data: bytes | None) -> str | None:
         """
         A deserializer which decodes the data into a string assuming UTF-8 encoding
 
         :param data: The data to decode
         :return: Decoded data
         :rtype: str
         """
         if data is None:
             return None
         return data.decode('utf-8')
 
     @staticmethod
-    def from_json(data: Optional[bytes]) -> Optional[Any]:
+    def from_json(data: bytes | None) -> Any | None:
         """
         A deserializer which decodes the data into an object by deserializing it as JSON
 
         :param data: The data to decode which is assumed to be a UTF-8 bytes encoding of a JSON string
         :return: Python object resulting from deserializing the JSON
         """
         if data is None:
```

### Comparing `telicent_lib-2.0.2/telicent_lib/sources/dictSource.py` & `telicent_lib-2.0.3/telicent_lib/sources/dictSource.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/telicent_lib/sources/kafkaSource.py` & `telicent_lib-2.0.3/telicent_lib/sources/kafkaSource.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,17 +84,17 @@
         :param topic: The Kafka topic from which data will be read
         :type topic: str
         :param broker: Deprecated, please specify broker through kafka_config
         :type broker: str
         :param kafka_config: Kafka configuration
         :type kafka_config: dict
         :param key_deserializer: The deserializer function/class to use to deserialize record keys
-        :type key_deserializer: Union[DeserializerFunction, Deserializer]
+        :type key_deserializer: DeserializerFunction | Deserializer
         :param value_deserializer: The deserializer function/class to use to deserialize record values
-        :type value_deserializer: Union[DeserializerFunction, Deserializer]
+        :type value_deserializer: DeserializerFunction | Deserializer
         :param commit_interval:
             How often to commit the read position to Kafka.  Defaults to 10,000 i.e. every 10,000 records read the read
             position will be committed.  Note that the read position is also committed whenever the source is closed
             **but** we cannot guarantee that we will be closed gracefully, so we commit the read position as we go.
         :param debug:
             Deprecated, please use a logger
         :type debug: bool
```

### Comparing `telicent_lib-2.0.2/telicent_lib/sources/listSource.py` & `telicent_lib-2.0.3/telicent_lib/sources/listSource.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/telicent_lib/status.py` & `telicent_lib-2.0.3/telicent_lib/status.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/telicent_lib/utils.py` & `telicent_lib-2.0.3/telicent_lib/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import inspect
 from inspect import Parameter
 from itertools import islice
-from typing import Any, Dict, Optional
+from typing import Any
 
 from confluent_kafka.admin import AdminClient
 
 __license__ = """
 Copyright (c) Telicent Ltd.
 
 Licensed under the Apache License, Version 2.0 (the "License");
@@ -18,29 +18,29 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 
-def __get_signature__(function: Any) -> Optional[inspect.Signature]:
+def __get_signature__(function: Any) -> inspect.Signature | None:
     """
     Gets the signature for a function (if any)
     :param function: A function or class
     :return: Signature, or None if not a valid function object
     """
     try:
         return inspect.signature(function)
     except TypeError:
         return None
     except ValueError:
         return None
 
 
-def __get_nth_value__(dictionary: Dict[Any, Any], n: int) -> Any:
+def __get_nth_value__(dictionary: dict[Any, Any], n: int) -> Any:
     """
     Gets the Nth value in a dictionary, only reliable if the dictionary is an ordered dictionary
     :param dictionary: Dictionary
     :param n: Index of value to return
     :return: Value, or None if no Nth value
     """
     iterator = iter(dictionary.items())
@@ -85,21 +85,14 @@
     sig_inspection = None
     if callable(protocol):
         sig_inspection = protocol.__call__
     required_signature = inspect.signature(sig_inspection)  # type: ignore
     if required_signature is None:
         raise TypeError(f"{protocol} is not a protocol whose validity can be checked")
 
-    # Validate return type
-    if signature.return_annotation != required_signature.return_annotation:
-        if signature.return_annotation == inspect.Signature.empty or required_signature.return_annotation != Any:
-            raise TypeError(f"Wrong return type {signature.return_annotation} for protocol {str(protocol)}, "
-                            f"expected {required_signature.return_annotation} but function {function} returns "
-                            f"{signature.return_annotation}")
-
     has_self = False
     adj = 0
     for i, parameter_tuple in enumerate(required_signature.parameters.items()):
         name, parameter = parameter_tuple
 
         # Special handling for self parameter
         # Since a protocol is a class its __call__() method will have a self parameter, the function we are trying to
```

### Comparing `telicent_lib-2.0.2/telicent_lib.egg-info/PKG-INFO` & `telicent_lib-2.0.3/telicent_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telicent-lib
-Version: 2.0.2
+Version: 2.0.3
 Summary: A helper package for building Adapters, Mappers and Projectors for Telicent Core
 Author-email: Telicent Ltd <admin@telicent.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `telicent_lib-2.0.2/telicent_lib.egg-info/SOURCES.txt` & `telicent_lib-2.0.3/telicent_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/tests/test_adapter.py` & `telicent_lib-2.0.3/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/tests/test_decode_token_middleware.py` & `telicent_lib-2.0.3/tests/test_decode_token_middleware.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/tests/test_edh_model.py` & `telicent_lib-2.0.3/tests/test_edh_model.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/tests/test_error_handler.py` & `telicent_lib-2.0.3/tests/test_error_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from typing import Iterable, List, Union
+from typing import Iterable
 from unittest import TestCase, mock
 
 from telicent_lib import AutomaticAdapter, Mapper, Projector, Record
 from telicent_lib.errors import ErrorHandler, ErrorLevel
 from telicent_lib.sinks.listSink import ListSink
 from telicent_lib.sources.listSource import ListSource
 
@@ -22,15 +22,15 @@
         self.closed = True
 
 
 def fake_adapter_function() -> Iterable[Record]:
     raise Exception('Test Exception')
 
 
-def fake_mapper_function(record: Record) -> Union[Record, List[Record], None]:
+def fake_mapper_function(record: Record) -> Record | list[Record] | None:
     raise Exception('Test Exception')
 
 
 def fake_projector_function(record: Record) -> None:
     raise Exception('Test Exception')
```

### Comparing `telicent_lib-2.0.2/tests/test_generate_ids.py` & `telicent_lib-2.0.3/tests/test_generate_ids.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Iterable, List, Union
+from typing import Iterable
 from unittest import TestCase
 
 from telicent_lib import Adapter, AutomaticAdapter, Mapper, Projector, Record
 from telicent_lib.action import Action, InputAction, InputOutputAction, OutputAction
 from telicent_lib.sinks.listSink import ListSink
 from telicent_lib.sources.listSource import ListSource
 
@@ -70,23 +70,23 @@
     def test_id_is_name(self):
         action = InputOutputAction(
             source=ListSource(), target=ListSink(), has_error_handler=False, has_reporter=False, disable_metrics=True
         )
         self.assertEqual('None-from-In-Memory List(0 records)-to-In-Memory List', action.generate_id())
 
     def test_id_is_name_adapter(self):
-        def my_func(record: Record) -> Union[Record, List[Record], None]:
+        def my_func(record: Record) -> Record | list[Record] | None:
             pass
         action = Mapper(
             source=ListSource(), target=ListSink(), has_error_handler=False, has_reporter=False,
             map_function=my_func, disable_metrics=True
         )
         self.assertEqual('Mapper-from-In-Memory List(0 records)-to-In-Memory List', action.generate_id())
 
     def test_named_action(self):
-        def my_func(record: Record) -> Union[Record, List[Record], None]:
+        def my_func(record: Record) -> Record | list[Record] | None:
             pass
         action = Mapper(
             source=ListSource(), target=ListSink(), has_error_handler=False, has_reporter=False, map_function=my_func,
             name='Test Action', disable_metrics=True
         )
         self.assertEqual('Test-Action', action.generate_id())
```

### Comparing `telicent_lib-2.0.2/tests/test_mapper.py` & `telicent_lib-2.0.3/tests/test_mapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 
 import unittest
-from typing import List, Union
 from unittest.mock import patch
 
 from telicent_lib import Mapper, Record, RecordMapper
 from telicent_lib.sinks.listSink import ListSink
 from telicent_lib.sources.listSource import ListSource
 from tests.delaySink import DelaySink
 from tests.test_records import RecordVerifier
 
 
-def __cube_keys__(record: Record) -> Union[Record, List[Record], None]:
+def __cube_keys__(record: Record) -> Record | list[Record] | None:
     if record is None:
         return None
     if isinstance(record.key, str):
         raise ValueError(record.key)
     return Record(record.headers, record.key * record.key * record.key, record.value, record.raw)
 
 
-def __power_keys__(record: Record, **map_args) -> Union[Record, List[Record], None]:
+def __power_keys__(record: Record, **map_args) -> Record | list[Record] | None:
     if record is None:
         return None
     return Record(record.headers, record.key ** map_args["power"], record.value, record.raw)
 
 
-def __fail_mapping__(record: Record) -> Union[Record, List[Record], None]:
+def __fail_mapping__(record: Record) -> Record | list[Record] | None:
     raise ValueError("Can't map this record")
 
 
 class SideChannelMapper(RecordMapper):
     def __init__(self):
-        self.data: List[Record] = []
+        self.data: list[Record] = []
 
-    def __call__(self, record: Record) -> Union[Record, List[Record], None]:
+    def __call__(self, record: Record) -> Record | list[Record] | None:
         self.data.append(record)
         return __cube_keys__(record)
 
     def get(self):
         return self.data
```

### Comparing `telicent_lib-2.0.2/tests/test_projector.py` & `telicent_lib-2.0.3/tests/test_projector.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 
 import unittest
-from typing import List
 
 from telicent_lib import Projector, Record, RecordProjector
 from telicent_lib.sources.listSource import ListSource
 from tests.test_records import RecordVerifier
 
 
 def __noop_projector__(record: Record) -> None:
@@ -17,39 +16,34 @@
 
 def __args_projector__(record: Record, **kwargs) -> None:
     print(kwargs["test"])
 
 
 class CollectingProjector(RecordProjector):
     def __init__(self):
-        self.data: List[Record] = []
+        self.data: list[Record] = []
 
     def __call__(self, record: Record) -> None:
         self.data.append(record)
 
-    def get(self) -> List[Record]:
+    def get(self) -> list[Record]:
         return self.data
 
 
 class TestProjector(RecordVerifier):
 
     def test_bad_projector_01(self):
         with self.assertRaisesRegex(TypeError, expected_regex=".*required positional argument.*projector_function.*"):
             Projector(source=ListSource(), target_store="Test", has_reporter=False, has_error_handler=False)
 
     def test_bad_projector_02(self):
         with self.assertRaisesRegex(ValueError, expected_regex=".*cannot be None"):
             Projector(source=ListSource(), target_store="Test", projector_function=None,
                       has_reporter=False, has_error_handler=False)
 
-    def test_bad_projector_03(self):
-        with self.assertRaisesRegex(TypeError, expected_regex=".*for protocol.*RecordProjector.*"):
-            Projector(source=ListSource(), target_store="Test", projector_function=self.test_bad_projector_02,
-                      has_reporter=False, has_error_handler=False)
-
     def test_projector_01(self):
         source = ListSource(self.__generate_records__(10))
         projector = Projector(source=source, target_store="Test", projector_function=__noop_projector__,
                               has_reporter=False, has_error_handler=False)
         projector.run()
 
     def test_projector_02(self):
```

### Comparing `telicent_lib-2.0.2/tests/test_protocol_validation.py` & `telicent_lib-2.0.3/tests/test_protocol_validation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 
 import unittest
-from typing import Any, Optional, Protocol, runtime_checkable
+from typing import Any, Protocol, runtime_checkable
 
-from telicent_lib.sinks import SerializerFunction
 from telicent_lib.sources import DeserializerFunction
 from telicent_lib.utils import validate_callable_protocol
 
 
 def not_a_deserializer(a: int, b: int) -> int:
     return a + b
 
 
 def nearly_a_deserializer(data: int) -> int:
     return data
 
 
-def a_deserializer(data: Optional[bytes]) -> Any:
+def a_deserializer(data: bytes | None) -> Any:
     return data
 
 
-def kwargs_deserializer(data: Optional[bytes], **kwargs) -> Any:
+def kwargs_deserializer(data: bytes | None, **kwargs) -> Any:
     return data
 
 
 def not_an_adder(a: int, b: int, c: bool) -> int:
     if c:
         return a * b
     else:
@@ -52,18 +51,14 @@
             validate_callable_protocol(a_deserializer, None)
 
     def test_protocol_validation_not_a_function(self) -> None:
         value = 45678
         with self.assertRaisesRegex(TypeError, expected_regex=".* not a function.*"):
             validate_callable_protocol(value, DeserializerFunction)
 
-    def test_protocol_validation_wrong_return_type(self) -> None:
-        with self.assertRaisesRegex(TypeError, expected_regex="Wrong return type.*"):
-            validate_callable_protocol(a_deserializer, SerializerFunction)
-
     def test_protocol_validation_wrong_parameter_type(self) -> None:
         with self.assertRaisesRegex(TypeError, expected_regex="Wrong parameter type.*.*bytes.*'int'.*"):
             validate_callable_protocol(not_a_deserializer, DeserializerFunction)
 
     def test_protocol_validation_good(self) -> None:
         validate_callable_protocol(a_deserializer, DeserializerFunction)
```

### Comparing `telicent_lib-2.0.2/tests/test_records.py` & `telicent_lib-2.0.3/tests/test_records.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import unittest
-from typing import Any, Callable, Iterable, List, Optional, Tuple, Union
+from typing import Any, Callable, Iterable
 
 from telicent_lib import Record, RecordUtils
 
 
 class RecordVerifier(unittest.TestCase):
 
     def __validate_record__(self, record: Record, headers: Any = None, key: Any = None, value: Any = None,
@@ -13,15 +13,15 @@
         self.assertIsNotNone(record)
         self.assertEqual(record.headers, headers, "Record headers don't match")
         self.assertEqual(record.key, key, "Record keys don't match")
         self.assertEqual(record.value, value, "Record values don't match")
         self.assertEqual(record.raw, raw, "Raw Records don't match")
 
     @staticmethod
-    def __generate_records__(total: int, value_function: Callable[[int], Any] = str) -> List[Record]:
+    def __generate_records__(total: int, value_function: Callable[[int], Any] = str) -> list[Record]:
         records = []
         for i in range(1, total + 1):
             records.append(Record(None, i, value_function(i)))
         return records
 
 
 class TestRecords(RecordVerifier):
@@ -66,15 +66,15 @@
         with self.assertRaisesRegex(TypeError, expected_regex=".*missing.*required positional argument.*"):
             Record(None, None)  # type: ignore
 
     def test_bad_record_04(self) -> None:
         with self.assertRaisesRegex(TypeError, expected_regex=".*missing.*required positional arguments.*"):
             Record(raw=[(1, "test")])  # type: ignore
 
-    def __validate_expected_headers__(self, iterable: Iterable[Optional[str]], expected_items: List[Optional[str]]):
+    def __validate_expected_headers__(self, iterable: Iterable[str | None], expected_items: list[str | None]):
         count = 0
         for i, item in enumerate(iterable):
             if i + 1 > len(expected_items):
                 self.fail("More header values found than expected")
             self.assertEqual(item, expected_items[i], "Header value not as expected")
             count += 1
 
@@ -221,15 +221,15 @@
         self.assertEqual(RecordUtils.get_first_header(record, "Test"), "12345")
         self.assertEqual(RecordUtils.get_last_header(record, "Test"), "12345")
         self.__validate_expected_headers__(RecordUtils.get_headers(record, "Test"), ["12345"])
         self.assertEqual(RecordUtils.get_first_header(record, "Exec-Path"), "foo")
         self.__validate_expected_headers__(RecordUtils.get_headers(record, "Exec-Path"), ["foo"])
 
     def test_header_preparation_02(self) -> None:
-        headers: Optional[List[Tuple[str, Union[str, bytes, None]]]] = [("Test", "12345"),
+        headers: list[tuple[str, str | bytes | None]] | None = [("Test", "12345"),
                                                                         ("Exec-Path", b"foo")]
         record = Record(RecordUtils.to_headers({"Test": "6789", "Exec-Path": "bar"}, headers), "key", "value")
 
         self.assertIsNotNone(record.headers)
         self.assertEqual(RecordUtils.get_first_header(record, "Test"), "12345")
         self.assertEqual(RecordUtils.get_last_header(record, "Test"), "6789")
         self.__validate_expected_headers__(RecordUtils.get_headers(record, "Test"), ["12345", "6789"])
```

### Comparing `telicent_lib-2.0.2/tests/test_reporter.py` & `telicent_lib-2.0.3/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/tests/test_security_labels.py` & `telicent_lib-2.0.3/tests/test_security_labels.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/tests/test_security_labels_edhv1.py` & `telicent_lib-2.0.3/tests/test_security_labels_edhv1.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/tests/test_serdes.py` & `telicent_lib-2.0.3/tests/test_serdes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 
 import inspect
 import unittest
 from json import JSONDecodeError
-from typing import Any, Callable, List, Optional, Tuple
+from typing import Any, Callable
 
 from confluent_kafka import KafkaException
 from confluent_kafka.serialization import Deserializer, Serializer
 from rdflib import RDF, RDFS, BNode, Dataset, Graph, URIRef
 from rdflib.compare import to_isomorphic
 from rdflib.graph import DATASET_DEFAULT_GRAPH_ID
 
 from telicent_lib.sinks import KafkaSink, Serializers
 from telicent_lib.sinks.serializers import RdfSerializer, SerializerFunction
 from telicent_lib.sources import Deserializers, KafkaSource
 from telicent_lib.sources.deserializers import DeserializerFunction, RdfDeserializer
 
 
-def __default_serdes__() -> List[Tuple[Callable[[Any], Optional[bytes]], Callable[[Optional[bytes]], Optional[Any]]]]:
+def __default_serdes__() -> list[tuple[Callable[[Any], bytes | None], Callable[[bytes | None], bytes | Any]]]:
     return [
         (Serializers.to_binary, Deserializers.binary_to_string),
         (Serializers.to_zipped_binary, Deserializers.unzip_to_string),
         (Serializers.to_json, Deserializers.from_json)
     ]
 
 
@@ -60,31 +60,31 @@
         print(b_iso.serialize(destination=None, encoding=None, format="nt11"))
 
     return a_iso == b_iso
 
 
 class ExtendedSerializerFunction(SerializerFunction):
 
-    def __call__(self, data: Optional[Any]) -> Optional[bytes]:
+    def __call__(self, data: Any | None) -> bytes | None:
         if data is None:
             return None
         return bytes(data)
 
 
 class ExtendedDeserializerFunction(DeserializerFunction):
 
-    def __call__(self, data: Optional[bytes]) -> Any:
+    def __call__(self, data: bytes | None) -> Any:
         return data
 
 
 class TestSerdes(unittest.TestCase):
 
-    def _verify_round_trip(self, data: Any, serializer_function: Callable[[Any], Optional[bytes]] = None,
+    def _verify_round_trip(self, data: Any, serializer_function: Callable[[Any], bytes | None] = None,
                            serializer_class: Serializer = None,
-                           deserializer_function: Callable[[Optional[bytes]], Optional[Any]] = None,
+                           deserializer_function: Callable[[bytes | None], Any | None] = None,
                            deserializer_class: Deserializer = None,
                            comparison_function: Callable[[Any, Any], bool] = None):
         if serializer_function:
             serialized_data = serializer_function(data)
         elif serializer_class:
             serialized_data = serializer_class(data)
         else:
```

### Comparing `telicent_lib-2.0.2/tests/test_sinks.py` & `telicent_lib-2.0.3/tests/test_sinks.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.2/tests/test_sources.py` & `telicent_lib-2.0.3/tests/test_sources.py`

 * *Files identical despite different names*

