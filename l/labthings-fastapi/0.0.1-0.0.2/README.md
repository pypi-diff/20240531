# Comparing `tmp/labthings_fastapi-0.0.1.tar.gz` & `tmp/labthings_fastapi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labthings_fastapi-0.0.1.tar", last modified: Thu May 30 21:08:44 2024, max compression
+gzip compressed data, was "labthings_fastapi-0.0.2.tar", last modified: Thu May 30 22:38:11 2024, max compression
```

## Comparing `labthings_fastapi-0.0.1.tar` & `labthings_fastapi-0.0.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:08:44.255917 labthings_fastapi-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-05-30 21:08:44.255917 labthings_fastapi-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 21:08:44.255917 labthings_fastapi-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:08:44.243917 labthings_fastapi-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:08:44.243917 labthings_fastapi-0.0.1/src/labthings_fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:08:44.247918 labthings_fastapi-0.0.1/src/labthings_fastapi/actions/
--rw-r--r--   0 runner    (1001) docker     (127)    16265 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/actions/invocation_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:08:44.247918 labthings_fastapi-0.0.1/src/labthings_fastapi/client/
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/client/in_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/client/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:08:44.247918 labthings_fastapi-0.0.1/src/labthings_fastapi/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/decorators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:08:44.247918 labthings_fastapi-0.0.1/src/labthings_fastapi/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/dependencies/blocking_portal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/dependencies/invocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/dependencies/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/dependencies/raw_thing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/dependencies/thing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:08:44.247918 labthings_fastapi-0.0.1/src/labthings_fastapi/descriptors/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/descriptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8873 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/descriptors/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/descriptors/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/descriptors/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:08:44.247918 labthings_fastapi-0.0.1/src/labthings_fastapi/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8816 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/outputs/blob.py
--rw-r--r--   0 runner    (1001) docker     (127)     8200 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/outputs/mjpeg_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/thing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:08:44.247918 labthings_fastapi-0.0.1/src/labthings_fastapi/thing_description/
--rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/thing_description/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/thing_description/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/thing_description/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/thing_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/thing_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:08:44.251917 labthings_fastapi-0.0.1/src/labthings_fastapi/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/types/numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:08:44.251917 labthings_fastapi-0.0.1/src/labthings_fastapi/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/utilities/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/src/labthings_fastapi/websockets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:08:44.251917 labthings_fastapi-0.0.1/src/labthings_fastapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-05-30 21:08:44.000000 labthings_fastapi-0.0.1/src/labthings_fastapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-30 21:08:44.000000 labthings_fastapi-0.0.1/src/labthings_fastapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 21:08:44.000000 labthings_fastapi-0.0.1/src/labthings_fastapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-30 21:08:44.000000 labthings_fastapi-0.0.1/src/labthings_fastapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 21:08:44.000000 labthings_fastapi-0.0.1/src/labthings_fastapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:08:44.251917 labthings_fastapi-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/tests/test_action_cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/tests/test_action_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/tests/test_action_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/tests/test_blob_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/tests/test_dependencies_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/tests/test_dependency_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/tests/test_endpoint_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/tests/test_introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/tests/test_numpy_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/tests/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/tests/test_td_dataschema_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/tests/test_temp_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/tests/test_thing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/tests/test_thing_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/tests/test_thing_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-30 21:08:40.000000 labthings_fastapi-0.0.1/tests/test_websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:38:11.239647 labthings_fastapi-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-30 22:38:11.239647 labthings_fastapi-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 22:38:11.239647 labthings_fastapi-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:38:11.227647 labthings_fastapi-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:38:11.231647 labthings_fastapi-0.0.2/src/labthings_fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:38:11.231647 labthings_fastapi-0.0.2/src/labthings_fastapi/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)    16265 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/actions/invocation_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:38:11.231647 labthings_fastapi-0.0.2/src/labthings_fastapi/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/client/in_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/client/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:38:11.231647 labthings_fastapi-0.0.2/src/labthings_fastapi/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/decorators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:38:11.231647 labthings_fastapi-0.0.2/src/labthings_fastapi/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/dependencies/blocking_portal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/dependencies/invocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/dependencies/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/dependencies/raw_thing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/dependencies/thing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:38:11.235647 labthings_fastapi-0.0.2/src/labthings_fastapi/descriptors/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/descriptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8873 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/descriptors/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/descriptors/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/descriptors/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:38:11.235647 labthings_fastapi-0.0.2/src/labthings_fastapi/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8816 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/outputs/blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8200 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/outputs/mjpeg_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/thing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:38:11.235647 labthings_fastapi-0.0.2/src/labthings_fastapi/thing_description/
+-rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/thing_description/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/thing_description/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/thing_description/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/thing_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/thing_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:38:11.235647 labthings_fastapi-0.0.2/src/labthings_fastapi/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/types/numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:38:11.235647 labthings_fastapi-0.0.2/src/labthings_fastapi/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/utilities/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/src/labthings_fastapi/websockets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:38:11.239647 labthings_fastapi-0.0.2/src/labthings_fastapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-30 22:38:11.000000 labthings_fastapi-0.0.2/src/labthings_fastapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-30 22:38:11.000000 labthings_fastapi-0.0.2/src/labthings_fastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 22:38:11.000000 labthings_fastapi-0.0.2/src/labthings_fastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-30 22:38:11.000000 labthings_fastapi-0.0.2/src/labthings_fastapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 22:38:11.000000 labthings_fastapi-0.0.2/src/labthings_fastapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:38:11.239647 labthings_fastapi-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/tests/test_action_cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/tests/test_action_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/tests/test_action_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/tests/test_blob_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/tests/test_dependencies_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/tests/test_dependency_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/tests/test_endpoint_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/tests/test_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/tests/test_numpy_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/tests/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/tests/test_td_dataschema_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/tests/test_temp_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/tests/test_thing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/tests/test_thing_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/tests/test_thing_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-30 22:38:07.000000 labthings_fastapi-0.0.2/tests/test_websocket.py
```

### Comparing `labthings_fastapi-0.0.1/LICENSE` & `labthings_fastapi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/PKG-INFO` & `labthings_fastapi-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: labthings-fastapi
-Version: 0.0.1
+Version: 0.0.2
 Summary: A test implementation of LabThings using FastAPI
 Author-email: Richard Bowman <richard.bowman@cantab.net>
 Project-URL: Homepage, https://github.com/rwb27/labthings-fastapi
 Project-URL: Bug Tracker, https://github.com/rwb27/labthings-fastapi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic>=2.0.0
 Requires-Dist: jsonschema
 Requires-Dist: typing_extensions
 Requires-Dist: anyio~=4.0
+Requires-Dist: httpx
 Provides-Extra: dev
 Requires-Dist: pytest<8,>=7.4.0; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: mypy<2,>=1.6.1; extra == "dev"
 Requires-Dist: ruff>=0.1.3; extra == "dev"
 Requires-Dist: types-jsonschema; extra == "dev"
 Requires-Dist: numpy~=1.20; extra == "dev"
```

### Comparing `labthings_fastapi-0.0.1/README.md` & `labthings_fastapi-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/pyproject.toml` & `labthings_fastapi-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "labthings-fastapi"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Richard Bowman", email="richard.bowman@cantab.net" },
 ]
 description = "A test implementation of LabThings using FastAPI"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -13,14 +13,15 @@
   "Operating System :: OS Independent",
 ]
 dependencies = [
   "pydantic>=2.0.0",
   "jsonschema",
   "typing_extensions",
   "anyio ~=4.0",
+  "httpx",
 ]
 
 [project.optional-dependencies]
 dev = [
   "pytest>=7.4.0, <8",
   "pytest-cov",
   "mypy>=1.6.1, <2",
```

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/actions/__init__.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/actions/invocation_model.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/actions/invocation_model.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/client/__init__.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/client/__init__.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/client/in_server.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/client/in_server.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/client/outputs.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/client/outputs.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/decorators/__init__.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/dependencies/blocking_portal.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/dependencies/blocking_portal.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/dependencies/invocation.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/dependencies/invocation.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/dependencies/metadata.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/dependencies/metadata.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/dependencies/raw_thing.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/dependencies/raw_thing.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/dependencies/thing.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/dependencies/thing.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/descriptors/action.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/descriptors/action.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/descriptors/endpoint.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/descriptors/endpoint.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/descriptors/property.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/descriptors/property.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/file_manager.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/file_manager.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/notifications.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/notifications.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/outputs/blob.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/outputs/blob.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/outputs/mjpeg_stream.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/outputs/mjpeg_stream.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/thing.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/thing.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/thing_description/__init__.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/thing_description/__init__.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/thing_description/model.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/thing_description/model.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/thing_description/validation.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/thing_description/validation.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/thing_server.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/thing_server.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/thing_settings.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/thing_settings.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/types/numpy.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/types/numpy.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/utilities/__init__.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/utilities/introspection.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/utilities/introspection.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi/websockets.py` & `labthings_fastapi-0.0.2/src/labthings_fastapi/websockets.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi.egg-info/PKG-INFO` & `labthings_fastapi-0.0.2/src/labthings_fastapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: labthings-fastapi
-Version: 0.0.1
+Version: 0.0.2
 Summary: A test implementation of LabThings using FastAPI
 Author-email: Richard Bowman <richard.bowman@cantab.net>
 Project-URL: Homepage, https://github.com/rwb27/labthings-fastapi
 Project-URL: Bug Tracker, https://github.com/rwb27/labthings-fastapi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic>=2.0.0
 Requires-Dist: jsonschema
 Requires-Dist: typing_extensions
 Requires-Dist: anyio~=4.0
+Requires-Dist: httpx
 Provides-Extra: dev
 Requires-Dist: pytest<8,>=7.4.0; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: mypy<2,>=1.6.1; extra == "dev"
 Requires-Dist: ruff>=0.1.3; extra == "dev"
 Requires-Dist: types-jsonschema; extra == "dev"
 Requires-Dist: numpy~=1.20; extra == "dev"
```

### Comparing `labthings_fastapi-0.0.1/src/labthings_fastapi.egg-info/SOURCES.txt` & `labthings_fastapi-0.0.2/src/labthings_fastapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/tests/test_action_cancel.py` & `labthings_fastapi-0.0.2/tests/test_action_cancel.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/tests/test_action_logging.py` & `labthings_fastapi-0.0.2/tests/test_action_logging.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/tests/test_action_manager.py` & `labthings_fastapi-0.0.2/tests/test_action_manager.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/tests/test_actions.py` & `labthings_fastapi-0.0.2/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/tests/test_blob_output.py` & `labthings_fastapi-0.0.2/tests/test_blob_output.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/tests/test_dependencies.py` & `labthings_fastapi-0.0.2/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/tests/test_dependencies_2.py` & `labthings_fastapi-0.0.2/tests/test_dependencies_2.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/tests/test_dependency_metadata.py` & `labthings_fastapi-0.0.2/tests/test_dependency_metadata.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/tests/test_endpoint_decorator.py` & `labthings_fastapi-0.0.2/tests/test_endpoint_decorator.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/tests/test_introspection.py` & `labthings_fastapi-0.0.2/tests/test_introspection.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/tests/test_properties.py` & `labthings_fastapi-0.0.2/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/tests/test_td_dataschema_generation.py` & `labthings_fastapi-0.0.2/tests/test_td_dataschema_generation.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/tests/test_temp_files.py` & `labthings_fastapi-0.0.2/tests/test_temp_files.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/tests/test_thing.py` & `labthings_fastapi-0.0.2/tests/test_thing.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/tests/test_thing_dependencies.py` & `labthings_fastapi-0.0.2/tests/test_thing_dependencies.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/tests/test_thing_lifecycle.py` & `labthings_fastapi-0.0.2/tests/test_thing_lifecycle.py`

 * *Files identical despite different names*

### Comparing `labthings_fastapi-0.0.1/tests/test_websocket.py` & `labthings_fastapi-0.0.2/tests/test_websocket.py`

 * *Files identical despite different names*

