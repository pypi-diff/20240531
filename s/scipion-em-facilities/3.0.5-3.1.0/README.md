# Comparing `tmp/scipion-em-facilities-3.0.5.tar.gz` & `tmp/scipion-em-facilities-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-facilities-3.0.5.tar", last modified: Sat Aug 19 07:34:20 2023, max compression
+gzip compressed data, was "scipion-em-facilities-3.1.0.tar", last modified: Fri May 31 09:36:58 2024, max compression
```

## Comparing `scipion-em-facilities-3.0.5.tar` & `scipion-em-facilities-3.1.0.tar`

### file list

```diff
@@ -1,56 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 07:34:20.936504 scipion-em-facilities-3.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-08-19 07:34:20.936504 scipion-em-facilities-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 07:34:20.932505 scipion-em-facilities-3.0.5/emfacilities/
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 07:34:20.936504 scipion-em-facilities-3.0.5/emfacilities/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/protocols/getnifs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/protocols/protocol_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/protocols/protocol_monitor_2d_streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14395 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/protocols/protocol_monitor_ctf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9659 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/protocols/protocol_monitor_movie_gain.py
--rw-r--r--   0 runner    (1001) docker     (123)    14402 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/protocols/protocol_monitor_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    19663 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/protocols/protocol_monitor_system.py
--rw-r--r--   0 runner    (1001) docker     (123)    41018 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/protocols/protocol_trackUsedItems.py
--rw-r--r--   0 runner    (1001) docker     (123)    55485 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/protocols/pynvml.py
--rw-r--r--   0 runner    (1001) docker     (123)    24315 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/protocols/report_html.py
--rw-r--r--   0 runner    (1001) docker     (123)    23362 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/protocols/report_influx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/protocols/summary_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/protocols/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/scipion_icon.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 07:34:20.936504 scipion-em-facilities-3.0.5/emfacilities/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    39513 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/templates/execution.summary.template.html
--rw-r--r--   0 runner    (1001) docker     (123)    20105 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/templates/facility_SPA_streaming.json.template
--rw-r--r--   0 runner    (1001) docker     (123)    22634 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/templates/to_2Dclassification_noDoseWeithed.json.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 07:34:20.936504 scipion-em-facilities-3.0.5/emfacilities/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 07:34:20.936504 scipion-em-facilities-3.0.5/emfacilities/tests/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/tests/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/tests/protocols/test_protocols_ctf_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/tests/protocols/test_protocols_ctf_streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/tests/protocols/test_protocols_system_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 07:34:20.936504 scipion-em-facilities-3.0.5/emfacilities/tests/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/tests/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/tests/workflows/test_workflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8374 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/tests/workflows/test_workflow_high_throughput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20446 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/tests/workflows/test_workflow_streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 07:34:20.936504 scipion-em-facilities-3.0.5/emfacilities/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24490 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/emfacilities/viewers/viewer_monitors.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 07:34:20.936504 scipion-em-facilities-3.0.5/scipion_em_facilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-08-19 07:34:20.000000 scipion-em-facilities-3.0.5/scipion_em_facilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-08-19 07:34:20.000000 scipion-em-facilities-3.0.5/scipion_em_facilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-19 07:34:20.000000 scipion-em-facilities-3.0.5/scipion_em_facilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-19 07:34:20.000000 scipion-em-facilities-3.0.5/scipion_em_facilities.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-19 07:34:20.000000 scipion-em-facilities-3.0.5/scipion_em_facilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-19 07:34:20.000000 scipion-em-facilities-3.0.5/scipion_em_facilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/secrets_template.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-19 07:34:20.936504 scipion-em-facilities-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-08-19 07:32:26.000000 scipion-em-facilities-3.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:36:58.653657 scipion-em-facilities-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-31 09:36:58.653657 scipion-em-facilities-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:36:58.645657 scipion-em-facilities-3.1.0/emfacilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:36:58.649657 scipion-em-facilities-3.1.0/emfacilities/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/getnifs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14123 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_good_classes_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10597 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_monitor_2d_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14395 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_monitor_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9659 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_monitor_movie_gain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_monitor_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19666 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_monitor_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41018 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_trackUsedItems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_volume_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55485 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/pynvml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24671 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/report_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23362 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/report_influx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/summary_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:36:58.649657 scipion-em-facilities-3.1.0/emfacilities/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    39513 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/templates/execution.summary.template.html
+-rw-r--r--   0 runner    (1001) docker     (127)    18541 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/templates/facility_SPA_streaming.json.template
+-rw-r--r--   0 runner    (1001) docker     (127)    22634 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/templates/to_2Dclassification_noDoseWeithed.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:36:58.649657 scipion-em-facilities-3.1.0/emfacilities/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:36:58.649657 scipion-em-facilities-3.1.0/emfacilities/tests/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/tests/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/tests/protocols/test_protocol_good_classes_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/tests/protocols/test_protocol_volume_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/tests/protocols/test_protocols_ctf_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/tests/protocols/test_protocols_ctf_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/tests/protocols/test_protocols_system_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:36:58.653657 scipion-em-facilities-3.1.0/emfacilities/tests/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/tests/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/tests/workflows/test_workflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8374 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/tests/workflows/test_workflow_high_throughput.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20446 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/tests/workflows/test_workflow_streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:36:58.653657 scipion-em-facilities-3.1.0/emfacilities/viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/viewers/viewer_good_classes_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24490 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/emfacilities/viewers/viewer_monitors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:36:58.653657 scipion-em-facilities-3.1.0/scipion_em_facilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-31 09:36:58.000000 scipion-em-facilities-3.1.0/scipion_em_facilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-31 09:36:58.000000 scipion-em-facilities-3.1.0/scipion_em_facilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 09:36:58.000000 scipion-em-facilities-3.1.0/scipion_em_facilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 09:36:58.000000 scipion-em-facilities-3.1.0/scipion_em_facilities.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-31 09:36:58.000000 scipion-em-facilities-3.1.0/scipion_em_facilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-31 09:36:58.000000 scipion-em-facilities-3.1.0/scipion_em_facilities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/secrets_template.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 09:36:58.653657 scipion-em-facilities-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-31 09:36:18.000000 scipion-em-facilities-3.1.0/setup.py
```

### Comparing `scipion-em-facilities-3.0.5/LICENSE` & `scipion-em-facilities-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.5/PKG-INFO` & `scipion-em-facilities-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scipion-em-facilities
-Version: 3.0.5
+Version: 3.1.0
 Summary: Plugin for Cryo-EM facilities to be used within Scipion framework
 Home-page: https://scipion-em.github.io/docs/docs/facilities/facilities.html
 Author: J.M. De la Rosa Trevin, Roberto Marabini, David Maluenda
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: ======================
         Scipion for facilities
```

### Comparing `scipion-em-facilities-3.0.5/README.rst` & `scipion-em-facilities-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.5/emfacilities/__init__.py` & `scipion-em-facilities-3.1.0/emfacilities/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 """
 
 import os
 import pwem
 
 from .constants import *
 
-__version__ = "3.0.5"
-_logo = "scipion_icon.gif"
+__version__ = "3.1.0"
+_logo = "facilityLogo.png"
 _references = ["delaRosaTrevin201693"]
 
 
 class Plugin(pwem.Plugin):
     _homeVar = EMFACILITIES_HOME_VARNAME 
     _pathVars = [EMFACILITIES_HOME_VARNAME]
```

### Comparing `scipion-em-facilities-3.0.5/emfacilities/bibtex.py` & `scipion-em-facilities-3.1.0/emfacilities/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.5/emfacilities/constants.py` & `scipion-em-facilities-3.1.0/emfacilities/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.5/emfacilities/protocols/__init__.py` & `scipion-em-facilities-3.1.0/emfacilities/protocols/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from .summary_provider import SummaryProvider
 
 from .protocol_monitor_ctf import ProtMonitorCTF, MonitorCTF, CTF_LOG_SQLITE
 from .protocol_monitor_system import ProtMonitorSystem
 from .protocol_monitor_movie_gain import ProtMonitorMovieGain, MonitorMovieGain
 
 from .protocol_monitor_2d_streamer import ProtMonitor2dStreamer
+from .protocol_good_classes_extractor import ProtGoodClassesExtractor
+from .protocol_volume_extractor import ProtVolumeExtractor
 
 from .report_html import ReportHtml
 
 from .protocol_trackUsedItems import UsedItemsTracker
 try:
     from .getnifs import *
 except ImportError:
```

### Comparing `scipion-em-facilities-3.0.5/emfacilities/protocols/getnifs.py` & `scipion-em-facilities-3.1.0/emfacilities/protocols/getnifs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.5/emfacilities/protocols/protocol_monitor.py` & `scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_monitor.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.5/emfacilities/protocols/protocol_monitor_2d_streamer.py` & `scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_monitor_2d_streamer.py`

 * *Files 19% similar despite different names*

```diff
@@ -35,15 +35,19 @@
 
 class ProtMonitor2dStreamer(ProtMonitor):
     """ This protocol will monitor an input set of particles
     (usually in streaming) and will run/schedule many copies
      of a given 2D classification protocol but using subsets
      of the input particles as the 2D classification input.
     """
-    _label = '2d streamer'
+    _label = '2d classification launcher'
+
+    NONE_OPTION = 0
+    CLASSIFICATION_JOBS = 1
+    NUMBER_PARTICLES = 2
 
     def __init__(self, **kwargs):
         ProtMonitor.__init__(self, **kwargs)
         self._runIds = pwobj.CsvList(pType=int)
 
     def _defineParams(self, form):
         form.addSection(label='Input')
@@ -72,14 +76,39 @@
         form.addParam('startingNumber', params.IntParam, default=0,
                       label="Starting number",
                       help="Specify a value greater than 0 if you want to skip "
                            "this amount of particles from the classification "
                            "batches (e.g, if you have classified them for the "
                            "initial 2D classification template. ")
 
+        form.addParam('cumulativeBatch', params.BooleanParam, default=False,
+                      label="Cumulative Batch?",
+                      help="If yes, the batches will be cumulative, and "
+                           "the size of each batch will be equal to: \n"
+                           "Batch size + cumulative population.")
+
+        form.addParam('maximumOption', params.EnumParam,
+                      choices=['None', 'Classification jobs', 'Number of particles'],
+                      default=self.NONE_OPTION,
+                      label="Limit for launching classification jobs", display=params.EnumParam.DISPLAY_COMBO,
+                      help='Select an option to limit the number of classification jobs launched: \n '
+                           '_None_: launch classification jobs until the set is closed. \n '
+                           '_Classification jobs_: set a maximum number of classification jobs to launch. \n'
+                           '_Number particles_: set a maximum number of particles to launch classification jobs.')
+
+        form.addParam('classificationJobs', params.IntParam, default=10,
+                      condition='maximumOption==%d' % self.CLASSIFICATION_JOBS,
+                      label='Maximum number of classification jobs',
+                      help='Set a maximum number of classification jobs to launch.')
+
+        form.addParam('numberParticles', params.IntParam, default=100000,
+                      condition='maximumOption==%d' % self.NUMBER_PARTICLES,
+                      label='Maximum number of particles',
+                      help='Set a maximum number of particles to launch classification jobs.')
+
         group = form.addGroup('Monitoring')
         group.addParam('samplingInterval', params.IntParam, default=10,
                        label="Update interval (min)",
                        help="After how many minutes the protocol should look "
                             "for new input data and schedule more 2D classification"
                             "jobs if necessary. ")
 
@@ -87,14 +116,16 @@
     def _insertAllSteps(self):
         self._insertFunctionStep('monitorStep')
 
     # --------------------------- STEPS functions ----------------------------
     def monitorStep(self):
         interval = self.samplingInterval.get() * 60
         # list of particles that will be inserted in the new set
+        self._counterNewParticles = 0
+        self._counterParticlesProcessed = 0
         self._counter = 0
         self._lastMicId = None
         self._lastPartId = 0
         self._subset = self._createSubset()
         self._runPrerequisites = []
         if self.input2dProtocol.get().isActive():
             self._runPrerequisites.append(self.input2dProtocol.get().getObjId())
@@ -149,23 +180,36 @@
             partId = particle.getObjId()
             subset.append(particle)
             self.debug("micId: %03d, particle: %05s, size: %s"
                       % (micId, partId, subset.getSize()))
 
             # Check the following after finding particles of a new micrograph
             if micId != self._lastMicId:
-                if self._lastMicId is not None and subset.getSize() > self.batchSize:
+                if self.classificationStop():
+                    self._streamClosed = True
+                    self.info("The limit for launching classification jobs has been reached, stopping protocol")
+                    return  # roll back to the monitorStep and finish
+
+                if self._lastMicId is not None and self._counterNewParticles > self.batchSize:  # New particles
                     self._writeSubset(subset)
+                    subsetTmp = subset  # save the previous so we can have the cumulative functionality
                     subset = self._createSubset()
+                    self.debug("Counter of new particles before resetting to 0: %d" % self._counterNewParticles)
+                    self._counterNewParticles = 0
+
+                    if self.cumulativeBatch:
+                        subset.appendFromImages(subsetTmp)
 
                 self._lastMicId = micId
 
             self._lastPartId = partId
+            self._counterNewParticles += 1
+            self._counterParticlesProcessed += 1
 
-        # Write last group of particles if input stream is closed
+            # Write last group of particles if input stream is closed
         if self._streamClosed:
             self._writeSubset(subset)
 
         self._subset = subset
 
     def _iterParticles(self):
         inputParts = self.inputParticles.get()
@@ -175,7 +219,21 @@
 
         for p in inputParts.iterItems(orderBy=['_micId', 'id'],
                                       direction='ASC',
                                       where='id > %d' % self._lastPartId):
             yield p
 
         inputParts.close()
+
+    def classificationStop(self):
+        response = False
+
+        if self.maximumOption == self.NUMBER_PARTICLES:
+            inputSize = self._counterParticlesProcessed
+            if inputSize > self.numberParticles.get():
+                response = True
+
+        if self.maximumOption == self.CLASSIFICATION_JOBS:
+            if self._counter > self.classificationJobs.get():
+                response = True
+
+        return response
```

### Comparing `scipion-em-facilities-3.0.5/emfacilities/protocols/protocol_monitor_ctf.py` & `scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_monitor_ctf.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.5/emfacilities/protocols/protocol_monitor_movie_gain.py` & `scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_monitor_movie_gain.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.5/emfacilities/protocols/protocol_monitor_summary.py` & `scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_monitor_summary.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 import pyworkflow.utils as pwutils
 import pyworkflow.protocol.params as params
 from pyworkflow import VERSION_1_1
 
 from pwem.protocols import ProtCTFMicrographs, ProtAlignMovies
 from pwem import Domain
+import subprocess
 
 from .report_influx import ReportInflux
 from .report_html import ReportHtml
 from .protocol_monitor import ProtMonitor, Monitor
 from .protocol_monitor_ctf import MonitorCTF
 from .protocol_monitor_movie_gain import MonitorMovieGain
 from .protocol_monitor_system import MonitorSystem
@@ -333,8 +334,26 @@
         if not os.path.exists(pathRepoSummary):
             summary.append("No summary file yet.")
         else:
             pathRepoSummary = open(pathRepoSummary, "r")
             for line in pathRepoSummary.readlines():
                 summary.append(line.rstrip())
             pathRepoSummary.close()
-        return summary
+        return summary
+
+
+    def validate(self):
+        errors = []
+        if self.publishCmd.get() != '':
+            self.reportDir = os.path.abspath(
+                self._getExtraPath(self.getProject().getShortName()))
+            pwutils.makePath(self.reportDir)
+
+            cmd = str(self.publishCmd) % {'REPORT_FOLDER': self.reportDir}
+            p = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE,
+                                 stderr=subprocess.PIPE)
+            output, err = p.communicate()
+            if err.decode("utf-8") != '':
+                errors.append('The publish command {} is wrong, please check it{}'.format(cmd, err.decode("utf-8")))
+
+
+        return errors
```

### Comparing `scipion-em-facilities-3.0.5/emfacilities/protocols/protocol_monitor_system.py` & `scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_monitor_system.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,17 +83,17 @@
                       help="Raise alarm if cpu allocated is greater "
                            "than given percentage")
         form.addParam('swapAlert', params.FloatParam, default=101,
                       label="Raise Alarm if Swap > XX%",
                       help="Raise alarm if swap allocated is greater "
                            "than given percentage")
 
-        form.addParam('monitorTime', params.FloatParam, default=300,
-                      label="Total Logging time (min)",
-                      help="Log during this interval")
+        #form.addParam('monitorTime', params.FloatParam, default=300,
+        #              label="Total Logging time (min)",
+        #              help="Log during this interval")
 
         ProtMonitor._sendMailParams(self, form)
         group = form.addGroup('GPU')
         group.addParam('doGpu', params.BooleanParam, default=False,
                        label="Check GPU",
                        help="Set to true if you want to monitor the GPU")
         group.addParam('gpusToUse', params.StringParam, default='0',
```

### Comparing `scipion-em-facilities-3.0.5/emfacilities/protocols/protocol_trackUsedItems.py` & `scipion-em-facilities-3.1.0/emfacilities/protocols/protocol_trackUsedItems.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.5/emfacilities/protocols/pynvml.py` & `scipion-em-facilities-3.1.0/emfacilities/protocols/pynvml.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.5/emfacilities/protocols/report_html.py` & `scipion-em-facilities-3.1.0/emfacilities/protocols/report_html.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 # *
 # **************************************************************************
 
 import json
 import os
 from os.path import join, exists, abspath, basename
 import numpy as np
+import subprocess
 import multiprocessing
 from datetime import datetime
 from statistics import median, mean
 
 from pyworkflow.protocol import getUpdatedProtocol
 import pyworkflow.utils as pwutils
 
@@ -563,10 +564,14 @@
         reportFile.write(reportTemplate)
         reportFile.close()
 
         if self.publishCmd:
             self.info("Publishing the report:")
             cmd = self.publishCmd % {'REPORT_FOLDER': self.reportDir}
             self.info(cmd)
-            os.system(cmd)
-
+            p = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE,
+                                 stderr=subprocess.PIPE)
+            output, err = p.communicate()
+            self.info('{}\n'.format(output.decode("utf-8")))
+            if err.decode("utf-8") != '':
+                self.info('Error publishing the report: {}'.format(err.decode("utf-8") ))
         return reportFinished
```

### Comparing `scipion-em-facilities-3.0.5/emfacilities/protocols/report_influx.py` & `scipion-em-facilities-3.1.0/emfacilities/protocols/report_influx.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.5/emfacilities/protocols/summary_provider.py` & `scipion-em-facilities-3.1.0/emfacilities/protocols/summary_provider.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.5/emfacilities/protocols/transport.py` & `scipion-em-facilities-3.1.0/emfacilities/protocols/transport.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.5/emfacilities/templates/execution.summary.template.html` & `scipion-em-facilities-3.1.0/emfacilities/templates/execution.summary.template.html`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.5/emfacilities/templates/facility_SPA_streaming.json.template` & `scipion-em-facilities-3.1.0/emfacilities/templates/facility_SPA_streaming.json.template`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-This workflow goes from import movies to 2D classes in streaming
+This workflow goes from Movies to 2Dclassification in streaming with estimating and monitoring movie gain.
 [
-    {
+     {
         "object.className": "ProtImportMovies",
-        "object.id": "1649",
-        "object.label": "pwem - import movies (10248)",
+        "object.id": "2284",
+        "object.label": "pwem - import movies",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
-        "runMode": 0,
+        "runMode": 1,
         "importFrom": 0,
-        "filesPath": "~Movie's folder|%(HOME)s|2|moviesPath~",
-        "filesPattern": "*.tiff",
+        "filesPath": "~Movie's folder|%(HOME)s/Movies|2|moviesPath~",
+        "filesPattern": "~Files pattern|*.tiff|0|filesPattern~",
         "copyFiles": false,
         "haveDataBeenPhaseFlipped": false,
         "acquisitionWizard": null,
-        "voltage": 300.0,
-        "sphericalAberration": 2.7,
+        "voltage": "~Voltage|300|3|voltage~",
+        "sphericalAberration": "~Spherical aberration|2.7|4|spherical~",
         "amplitudeContrast": 0.1,
         "magnification": 50000,
         "samplingRateMode": 0,
-        "samplingRate": 0.495,
+        "samplingRate": "~Sampling Rate|0.907|4|sampling~",
         "scannedPixelSize": 7.0,
         "doseInitial": 0.0,
-        "dosePerFrame": 1.0,
-        "gainFile": "~Gain file|%(HOME)s|2|gain~",
+        "dosePerFrame": "~Dose per frame|1.0|4|dosePerFrame~",
+        "gainFile": "~Gain's file|%(HOME)s/Movies/gain.mrc|0|gainPath~",
         "darkFile": null,
-        "dataStreaming": false,
+        "dataStreaming": "~Live acquisition|true|0|streamingImport~",
         "timeout": 43200,
         "fileTimeout": 30,
         "blacklistDateFrom": null,
         "blacklistDateTo": null,
         "useRegexps": true,
         "blacklistFile": null,
         "inputIndividualFrames": false,
@@ -39,42 +39,42 @@
         "stackFrames": false,
         "writeMoviesInProject": false,
         "movieSuffix": "_frames.mrcs",
         "deleteFrames": false
     },
     {
         "object.className": "XmippProtMovieMaxShift",
-        "object.id": "2158",
-        "object.label": "xmipp3 - movie maxshift (copy)",
-        "object.comment": "muy estricto el filtro",
+        "object.id": "1207",
+        "object.label": "xmipp3 - movie maxshift",
+        "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
-        "runMode": 0,
+        "runMode": 1,
         "rejType": 3,
         "maxFrameShift": 5.0,
-        "maxMovieShift": 15.0,
-        "inputMovies": "2193.outputMovies"
+        "maxMovieShift": 20.0,
+        "inputMovies": "1242.outputMovies"
     },
     {
         "object.className": "ProtMotionCorr",
-        "object.id": "2193",
-        "object.label": "motioncorr - movie alignment (gpus 0, 1) (copy)",
+        "object.id": "1242",
+        "object.label": "motioncorr - movie alignment (gpus 0, 1)",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
-        "runMode": 0,
+        "runMode": 1,
         "doSaveAveMic": true,
         "useAlignToSum": true,
         "alignFrame0": 1,
-        "alignFrameN": 35,
-        "binFactor": 1.0,
+        "alignFrameN": 0,
+        "binFactor": "~Binning factor alignment|1.0|4|bin~",
         "cropOffsetX": 0,
         "cropOffsetY": 0,
         "cropDimX": 0,
         "cropDimY": 0,
         "splitEvenOdd": false,
         "doSaveMovie": false,
         "doComputePSD": false,
@@ -100,46 +100,46 @@
         "doMagCor": false,
         "scaleMaj": 1.0,
         "scaleMin": 1.0,
         "angDist": 0.0,
         "hostName": "localhost",
         "numberOfThreads": 3,
         "numberOfMpi": 1,
-        "inputMovies": "1649.outputMovies"
+        "inputMovies": "2284.outputMovies"
     },
     {
         "object.className": "XmippProtTiltAnalysis",
-        "object.id": "2259",
-        "object.label": "xmipp3 - tilt analysis (copy)",
+        "object.id": "1309",
+        "object.label": "xmipp3 - tilt analysis",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
-        "runMode": 0,
+        "runMode": 1,
         "window_size": 1024,
         "objective_resolution": 3.0,
         "meanCorr_threshold": 0.5,
         "stdCorr_threshold": 0.1,
         "saveIntermediateResults": false,
         "hostName": "localhost",
         "numberOfThreads": 4,
         "numberOfMpi": 1,
-        "inputMicrographs": "2158.outputMicrographsDoseWeighted"
+        "inputMicrographs": "1207.outputMicrographsDoseWeighted"
     },
     {
         "object.className": "CistemProtCTFFind",
-        "object.id": "2296",
-        "object.label": "cistem - ctffind4 (copy)",
+        "object.id": "1346",
+        "object.label": "cistem - ctffind4",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
-        "runMode": 0,
+        "runMode": 1,
         "recalculate": false,
         "sqliteFile": null,
         "inputType": 1,
         "avgFrames": 3,
         "usePowerSpectra": false,
         "windowSize": 512,
         "lowRes": 30.0,
@@ -151,40 +151,40 @@
         "fixAstig": true,
         "astigmatism": 100.0,
         "findPhaseShift": false,
         "minPhaseShift": 0.0,
         "maxPhaseShift": 180.0,
         "stepPhaseShift": 10.0,
         "hostName": "localhost",
-        "numberOfThreads": 2,
+        "numberOfThreads": 4,
         "numberOfMpi": 1,
         "streamingWarning": null,
         "streamingSleepOnWait": 0,
         "streamingBatchSize": 1,
-        "inputMicrographs": "2411.outputMicrographs"
+        "inputMicrographs": "1461.outputMicrographs"
     },
     {
         "object.className": "XmippProtCTFConsensus",
-        "object.id": "2354",
-        "object.label": "xmipp3 - ctf consensus (copy)",
+        "object.id": "1404",
+        "object.label": "xmipp3 - ctf consensus",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
-        "runMode": 0,
+        "runMode": 1,
         "useDefocus": true,
         "minDefocus": 1000.0,
         "maxDefocus": 30000.0,
         "useAstigmatism": false,
         "astigmatism": 1000.0,
         "useAstigmatismPercentage": true,
         "astigmatismPer": 0.1,
         "useResolution": true,
-        "resolution": 4.5,
+        "resolution": "~Resolution filter|4.5|4|resolution~",
         "useCritXmipp": false,
         "critFirstZero": 5.0,
         "minCritFirstZeroRatio": 0.9,
         "maxCritFirstZeroRatio": 1.1,
         "critCorr": 0.05,
         "critCtfMargin": 1.5,
         "critIceness": 1.0,
@@ -193,366 +193,236 @@
         "calculateConsensus": false,
         "minConsResol": 4.0,
         "averageDefocus": true,
         "includeSecondary": true,
         "hostName": "localhost",
         "numberOfThreads": 4,
         "numberOfMpi": 1,
-        "inputCTF": "2296.outputCTF"
+        "inputCTF": "1346.outputCTF"
     },
     {
         "object.className": "CryoassessProtMics",
-        "object.id": "2411",
-        "object.label": "cryoassess - assess micrographs (gpu 2) (copy)",
+        "object.id": "1461",
+        "object.label": "cryoassess - assess micrographs (gpu 2)",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
-        "runMode": 0,
+        "runMode": 1,
         "threshold": 0.1,
         "threshold2": 0.1,
         "batchSize": 16,
         "gpuList": "2",
         "hostName": "localhost",
         "numberOfThreads": 1,
         "numberOfMpi": 1,
         "streamingWarning": null,
         "streamingSleepOnWait": 1,
-        "streamingBatchSize": 5,
-        "inputMicrographs": "2259.outputMicrographs"
+        "streamingBatchSize": 8,
+        "inputMicrographs": "1309.outputMicrographs"
     },
     {
         "object.className": "SphireProtCRYOLOPicking",
-        "object.id": "2450",
-        "object.label": "sphire - cryolo picking (gpu 3) (copy)",
+        "object.id": "1500",
+        "object.label": "sphire - cryolo picking",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
-        "runMode": 0,
+        "runMode": 1,
         "inputModelFrom": 0,
         "conservPickVar": 0.3,
         "lowPassFilter": true,
         "absCutOffFreq": 0.1,
         "numCpus": 4,
         "input_size": 1024,
         "boxSize": 0,
         "max_box_per_image": 600,
-        "useGpu": true,
-        "gpuList": "3",
+        "useGpu": false,
+        "gpuList": "0",
         "boxSizeFactor": 1.0,
         "hostName": "localhost",
         "numberOfThreads": 1,
         "numberOfMpi": 1,
         "streamingWarning": null,
         "streamingSleepOnWait": 0,
-        "streamingBatchSize": 4,
-        "inputMicrographs": "2639.outputMicrographs"
+        "streamingBatchSize": 8,
+        "inputMicrographs": "1673.outputMicrographs"
     },
     {
         "object.className": "ProtBoxSizeParameters",
-        "object.id": "2498",
-        "object.label": "pwem - box size related parameters (copy 7)",
+        "object.id": "1548",
+        "object.label": "pwem - box size related parameters",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
-        "runMode": 0,
-        "boxSize": "2450.boxsize",
+        "runMode": 1,
+        "boxSize": "1500.boxsize",
         "boolExtractPartBx": true,
         "factorExtractPartBx": 1.64,
         "boolGautomatchParams": false,
         "factorGautRadius": 0.75,
         "factorGautMinInterPartDist": 0.9,
         "factorGautSigmaDiameter": 1.2,
         "factorGautAvgDiameter": 1.5,
         "boolRelionParams": true,
         "factorMinLoGFilter": 0.9,
         "factorMaxLoGFilter": 1.1,
-        "boolTopazParams": true,
+        "boolTopazParams": false,
         "factorTopazRadius": 0.45,
         "numPartPerImg": 300,
         "boolConsensusParams": true,
         "factorConsensusRadius": 0.9,
         "hostName": "localhost",
         "numberOfThreads": 1,
         "numberOfMpi": 1,
-        "inputMicrographs": "2639.outputMicrographs"
+        "inputMicrographs": "1673.outputMicrographs"
     },
     {
         "object.className": "ProtRelionAutopickLoG",
-        "object.id": "2548",
-        "object.label": "relion - auto-picking LoG (copy)",
+        "object.id": "1596",
+        "object.label": "relion - auto-picking LoG",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
-        "runMode": 0,
-        "boxSize": "2498.boxSizeEven",
-        "minDiameter": "2498.minLoGFilterRelion",
-        "maxDiameter": "2498.maxLoGFilterRelion",
+        "runMode": 1,
+        "boxSize": "1548.boxSizeEven",
+        "minDiameter": "1548.minLoGFilterRelion",
+        "maxDiameter": "1548.maxLoGFilterRelion",
         "areParticlesWhite": false,
         "maxResolution": 20.0,
         "threshold": 0.0,
         "threshold2": 999.0,
         "extraParams": "",
         "streamingWarning": null,
         "streamingSleepOnWait": 0,
-        "streamingBatchSize": 4,
+        "streamingBatchSize": 8,
         "hostName": "localhost",
         "numberOfMpi": 5,
-        "inputMicrographs": "2639.outputMicrographs"
+        "inputMicrographs": "1673.outputMicrographs"
     },
     {
         "object.className": "XmippProtConsensusPicking",
-        "object.id": "2597",
-        "object.label": "xmipp3 - picking consensus (copy)",
+        "object.id": "1639",
+        "object.label": "xmipp3 - picking consensus",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
-        "runMode": 0,
+        "runMode": 1,
         "inputCoordinates": [
-            "2450.outputCoordinates",
-            "2548.outputCoordinates",
-            "3040.outputCoordinates"
+            "1500.outputCoordinates",
+            "1596.outputCoordinates"
         ],
-        "consensusRadius": "2498.radiusConsensus",
-        "consensus": 2,
+        "consensusRadius": "1548.radiusConsensus",
+        "consensus": -1,
         "mode": 0
     },
     {
         "object.className": "XmippProtTriggerData",
-        "object.id": "2639",
-        "object.label": "xmipp3 (\u1e9f) - trigger data (receive stop signal) (copy 2)",
+        "object.id": "1673",
+        "object.label": "xmipp3 (\u1e9f) - trigger data (receive stop signal)",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
-        "runMode": 0,
+        "runMode": 1,
         "triggerWait": true,
         "outputSize": 1,
         "allImages": true,
         "splitImages": false,
         "triggerSignal": false,
         "delay": 4,
-        "inputImages": "2354.outputMicrographs"
-    },
-    {
-        "object.className": "CistemProtCTFFind",
-        "object.id": "2679",
-        "object.label": "cistem - ctffind4 (2) (copy)",
-        "object.comment": "",
-        "_useQueue": false,
-        "_prerequisites": "",
-        "_queueParams": null,
-        "runName": null,
-        "runMode": 0,
-        "recalculate": false,
-        "sqliteFile": null,
-        "inputType": 1,
-        "avgFrames": 3,
-        "usePowerSpectra": false,
-        "windowSize": 512,
-        "lowRes": 30.0,
-        "highRes": 5.0,
-        "minDefocus": 5000.0,
-        "maxDefocus": 50000.0,
-        "stepDefocus": 500.0,
-        "slowSearch": false,
-        "fixAstig": true,
-        "astigmatism": 100.0,
-        "findPhaseShift": false,
-        "minPhaseShift": 0.0,
-        "maxPhaseShift": 180.0,
-        "stepPhaseShift": 10.0,
-        "hostName": "localhost",
-        "numberOfThreads": 2,
-        "numberOfMpi": 1,
-        "streamingWarning": null,
-        "streamingSleepOnWait": 0,
-        "streamingBatchSize": 1,
-        "inputMicrographs": "2639.outputMicrographs"
-    },
-    {
-        "object.className": "TopazProtPicking",
-        "object.id": "3040",
-        "object.label": "topaz - topaz picking (gpu 3) (copy)",
-        "object.comment": "",
-        "_useQueue": false,
-        "_prerequisites": "",
-        "_queueParams": null,
-        "runName": null,
-        "runMode": 0,
-        "modelInitialization": 1,
-        "generalModel": 0,
-        "radius": "2498.radiusTopaz",
-        "boxSize": "2498.boxSizeEven",
-        "threshold": -8.0,
-        "hostName": "localhost",
-        "numberOfThreads": 1,
-        "numberOfMpi": 1,
-        "doDenoise": false,
-        "modelDenoise": 0,
-        "patchSize": -1,
-        "denoiseExtra": "",
-        "scale": 4,
-        "preExtra": "",
-        "gpuList": "3",
-        "streamingWarning": null,
-        "streamingSleepOnWait": 0,
-        "streamingBatchSize": 8,
-        "inputMicrographs": "2639.outputMicrographs"
+        "inputImages": "1404.outputMicrographs"
     },
     {
         "object.className": "XmippProtDeepMicrographScreen",
-        "object.id": "3093",
-        "object.label": "xmipp3 - deep micrograph cleaner (copy)",
+        "object.id": "1820",
+        "object.label": "xmipp3 - deep micrograph cleaner (gpu=2)",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
-        "runMode": 0,
+        "runMode": 1,
         "micsSource": 0,
         "useOtherScale": 0,
-        "threshold": 0.85,
+        "threshold": 0.95,
         "streamingBatchSize": -1,
         "saveMasks": false,
         "useGpu": true,
-        "gpuList": "0",
-        "inputCoordinates": "2597.consensusCoordinates"
+        "gpuList": "3",
+        "inputCoordinates": "1639.consensusCoordinates"
     },
     {
         "object.className": "ProtRelionExtractParticles",
-        "object.id": "4718",
-        "object.label": "relion - particles extraction (copy 3)",
+        "object.id": "1861",
+        "object.label": "relion - particles extraction",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
-        "runMode": 0,
+        "runMode": 1,
         "downsampleType": 0,
-        "boxSize": "2498.boxSizeExtraction",
+        "boxSize": "1548.boxSizeExtraction",
         "doRescale": false,
         "rescaledSize": 128,
         "saveFloat16": false,
         "doInvert": true,
         "doNormalize": true,
         "backDiameter": -1,
         "stddevWhiteDust": -1.0,
         "stddevBlackDust": -1.0,
         "streamingWarning": null,
         "streamingSleepOnWait": 0,
         "streamingBatchSize": 0,
         "hostName": "localhost",
         "numberOfMpi": 4,
-        "ctfRelations": "2679.outputCTF",
-        "inputCoordinates": "3093.outputCoordinates_Auto_085"
+        "ctfRelations": "1404.outputCTF",
+        "inputCoordinates": "1820.outputCoordinates_Auto_095"
     },
     {
         "object.className": "XmippProtTriggerData",
-        "object.id": "4769",
-        "object.label": "xmipp3 (\u1e9f) - trigger data (send stop signal) (copy 3)",
+        "object.id": "1910",
+        "object.label": "xmipp3 (\u1e9f) - trigger data (send stop signal)",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
-        "runMode": 0,
+        "runMode": 1,
         "triggerWait": false,
-        "outputSize": 40000,
+        "outputSize": "~Number of particles to trigger 2D|20000|3|particles~",
         "allImages": true,
         "splitImages": false,
         "triggerSignal": true,
+        "triggerProt": "1673.",
         "delay": 4,
-        "triggerProt": "2639.",
-        "inputImages": "4718.outputParticles"
-    },
-    {
-        "object.className": "ProtCryo2D",
-        "object.id": "4809",
-        "object.label": "cryosparc2 - 2D classification (gpu 3) (copy 3)",
-        "object.comment": "",
-        "_useQueue": false,
-        "_prerequisites": "",
-        "_queueParams": null,
-        "runName": null,
-        "runMode": 0,
-        "numberOfClasses": 50,
-        "maximunResolution": 6,
-        "initialClassification": 2.0,
-        "useCircular2D": true,
-        "class2D_window_inner_A": null,
-        "class2D_window_outer_A": null,
-        "reCenter2D": true,
-        "reCenterMask": 0.2,
-        "reCenterMaskBinary": false,
-        "forceMaxover": true,
-        "ctfFlipPhases": false,
-        "numberFinalIterator": 1,
-        "numberOnlineEMIterator": 20,
-        "batchSizeClass": 100,
-        "initialScale2D": 1,
-        "zeropadFactor": 2,
-        "useFRCRegularized": true,
-        "useFullFRC": true,
-        "iterationToStartAnneling": 2,
-        "iterationToStartAnneal": 15,
-        "useWhiteNoiseModel": false,
-        "compute_use_ssd": false,
-        "gpuList": "3",
-        "compute_lane": "default",
-        "inputParticles": "4769.outputParticles"
-    },
-    {
-        "object.className": "CryoassessProt2D",
-        "object.id": "4865",
-        "object.label": "cryoassess (\u1e9f) - assess 2D classes (copy 3)",
-        "object.comment": "",
-        "_useQueue": false,
-        "_prerequisites": "",
-        "_queueParams": null,
-        "runName": null,
-        "runMode": 0,
-        "batchSize": 32,
-        "inputRefs": "4809.outputClasses"
-    },
-    {
-        "object.className": "ProtClassesSelector",
-        "object.id": "4898",
-        "object.label": "pwem (\u1e9f) - numeric classes extractor (copy 3)",
-        "object.comment": "",
-        "_useQueue": false,
-        "_prerequisites": "",
-        "_queueParams": null,
-        "runName": null,
-        "runMode": 0,
-        "extractRepresentative": false,
-        "firstNElements": 10,
-        "inputClasses": "4865.outputClasses"
+        "inputImages": "1861.outputParticles"
     },
     {
         "object.className": "ProtCryo2D",
-        "object.id": "4932",
-        "object.label": "cryosparc2 - 2D classification (copy 3)",
+        "object.id": "1950",
+        "object.label": "cryosparc2 - 2D classification (gpu 3)",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
-        "runMode": 0,
-        "numberOfClasses": 50,
+        "runMode": 1,
+        "numberOfClasses": "~Number of classes (1st)|50|3|classes~",
         "maximunResolution": 6,
         "initialClassification": 2.0,
         "useCircular2D": true,
         "class2D_window_inner_A": null,
         "class2D_window_outer_A": null,
         "reCenter2D": true,
         "reCenterMask": 0.2,
@@ -568,66 +438,69 @@
         "useFullFRC": true,
         "iterationToStartAnneling": 2,
         "iterationToStartAnneal": 15,
         "useWhiteNoiseModel": false,
         "compute_use_ssd": false,
         "gpuList": "3",
         "compute_lane": "default",
-        "inputParticles": "4898.output"
+        "inputParticles": "1910.outputParticles"
     },
     {
         "object.className": "CryoassessProt2D",
-        "object.id": "4988",
-        "object.label": "cryoassess (\u1e9f) - assess 2D classes (2) (copy 5)",
+        "object.id": "2006",
+        "object.label": "cryoassess (\u1e9f) - assess 2D classes",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
-        "runMode": 0,
+        "runMode": 1,
         "batchSize": 32,
-        "inputRefs": "4932.outputClasses"
+        "hostName": "localhost",
+        "numberOfThreads": 3,
+        "numberOfMpi": 1,
+        "inputRefs": "1950.outputClasses"
     },
     {
         "object.className": "XmippProtMovieGain",
-        "object.id": "9452",
-        "object.label": "xmipp3 - movie gain (copy)",
+        "object.id": "4713",
+        "object.label": "xmipp3 - movie gain",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
-        "runMode": 0,
+        "runMode": 1,
         "estimateGain": true,
         "estimateOrientation": true,
         "estimateResidualGain": true,
         "normalizeGain": true,
         "estimateSigma": false,
         "frameStep": 5,
-        "movieStep": 50,
+        "movieStep": 100,
         "hostName": "localhost",
         "numberOfThreads": 4,
         "numberOfMpi": 1,
-        "inputMovies": "1649.outputMovies"
+        "inputMovies": "2284.outputMovies"
     },
     {
         "object.className": "ProtMonitorSummary",
-        "object.id": "10382",
-        "object.label": "emfacilities - monitor summary (2)",
+        "object.id": "4752",
+        "object.label": "emfacilities - monitor summary",
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
-        "runMode": 0,
+        "runMode": 1,
         "inputProtocols": [
-            "2158",
-            "9452",
-            "2296",
-            "1649"
+            "2284",
+            "1207",
+            "1346",
+            "4713"
         ],
         "samplingInterval": 60,
         "monitorTime": 34560.0,
         "stddevValue": 0.04,
         "ratio1Value": 1.15,
         "ratio2Value": 4.5,
         "maxDefocus": 40000.0,
@@ -643,9 +516,75 @@
         "doDiskIO": false,
         "doMail": false,
         "emailFrom": "from@from.fakeadress.com",
         "emailTo": "to@to.fakeadress.com",
         "smtp": "smtp.fakeadress.com",
         "doInflux": false,
         "publishCmd": ""
+    },
+    {
+        "object.className": "XmippProtCenterParticles",
+        "object.id": "4920",
+        "object.label": "xmipp3 - center particles",
+        "object.comment": "",
+        "_useQueue": false,
+        "_prerequisites": "",
+        "_queueParams": null,
+        "runName": null,
+        "runMode": 1,
+        "hostName": "localhost",
+        "inputMics": "1673.outputMicrographs",
+        "inputClasses": "2006.outputClasses"
+    },
+    {
+        "object.className": "ProtCryo2D",
+        "object.id": "4954",
+        "object.label": "cryosparc2 - 2D classification",
+        "object.comment": "",
+        "_useQueue": false,
+        "_prerequisites": "",
+        "_queueParams": null,
+        "runName": null,
+        "runMode": 1,
+        "numberOfClasses": "~Number of classes (2nd)|30|3|classes~",
+        "maximunResolution": 6,
+        "initialClassification": 2.0,
+        "useCircular2D": true,
+        "class2D_window_inner_A": null,
+        "class2D_window_outer_A": null,
+        "reCenter2D": true,
+        "reCenterMask": 0.2,
+        "reCenterMaskBinary": false,
+        "forceMaxover": true,
+        "ctfFlipPhases": false,
+        "numberFinalIterator": 1,
+        "numberOnlineEMIterator": 20,
+        "batchSizeClass": 100,
+        "initialScale2D": 1,
+        "zeropadFactor": 2,
+        "useFRCRegularized": true,
+        "useFullFRC": true,
+        "iterationToStartAnneling": 2,
+        "iterationToStartAnneal": 15,
+        "useWhiteNoiseModel": false,
+        "compute_use_ssd": false,
+        "gpuList": "3",
+        "compute_lane": "default",
+        "inputParticles": "4920.outputParticles"
+    },
+    {
+        "object.className": "CryoassessProt2D",
+        "object.id": "5010",
+        "object.label": "cryoassess (\u1e9f) - assess 2D classes (2)",
+        "object.comment": "",
+        "_useQueue": false,
+        "_prerequisites": "",
+        "_queueParams": null,
+        "runName": null,
+        "runMode": 1,
+        "batchSize": 32,
+        "hostName": "localhost",
+        "numberOfThreads": 3,
+        "numberOfMpi": 1,
+        "inputRefs": "4954.outputClasses"
     }
-]
+]
```

### Comparing `scipion-em-facilities-3.0.5/emfacilities/templates/to_2Dclassification_noDoseWeithed.json.template` & `scipion-em-facilities-3.1.0/emfacilities/templates/to_2Dclassification_noDoseWeithed.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.5/emfacilities/tests/__init__.py` & `scipion-em-facilities-3.1.0/emfacilities/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.5/emfacilities/tests/protocols/test_protocols_ctf_monitor.py` & `scipion-em-facilities-3.1.0/emfacilities/tests/protocols/test_protocols_ctf_monitor.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.5/emfacilities/tests/protocols/test_protocols_ctf_streaming.py` & `scipion-em-facilities-3.1.0/emfacilities/tests/protocols/test_protocols_ctf_streaming.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.5/emfacilities/tests/protocols/test_protocols_system_monitor.py` & `scipion-em-facilities-3.1.0/emfacilities/tests/protocols/test_protocols_system_monitor.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.5/emfacilities/tests/workflows/test_workflow.py` & `scipion-em-facilities-3.1.0/emfacilities/tests/workflows/test_workflow.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.5/emfacilities/tests/workflows/test_workflow_high_throughput.py` & `scipion-em-facilities-3.1.0/emfacilities/tests/workflows/test_workflow_high_throughput.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.5/emfacilities/tests/workflows/test_workflow_streaming.py` & `scipion-em-facilities-3.1.0/emfacilities/tests/workflows/test_workflow_streaming.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.5/emfacilities/viewers/__init__.py` & `scipion-em-facilities-3.1.0/emfacilities/viewers/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,7 +22,8 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 from .viewer_monitors import (ProtMonitorCTFViewer, ProtMonitorSystemViewer,
                               ProtMonitorMovieGainViewer, ViewerMonitorSummary)
+from .viewer_good_classes_extractor import ViewerGoodClassesExtractor
```

### Comparing `scipion-em-facilities-3.0.5/emfacilities/viewers/viewer_monitors.py` & `scipion-em-facilities-3.1.0/emfacilities/viewers/viewer_monitors.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.5/scipion_em_facilities.egg-info/PKG-INFO` & `scipion-em-facilities-3.1.0/scipion_em_facilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scipion-em-facilities
-Version: 3.0.5
+Version: 3.1.0
 Summary: Plugin for Cryo-EM facilities to be used within Scipion framework
 Home-page: https://scipion-em.github.io/docs/docs/facilities/facilities.html
 Author: J.M. De la Rosa Trevin, Roberto Marabini, David Maluenda
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: ======================
         Scipion for facilities
```

### Comparing `scipion-em-facilities-3.0.5/scipion_em_facilities.egg-info/SOURCES.txt` & `scipion-em-facilities-3.1.0/scipion_em_facilities.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -4,42 +4,47 @@
 README.rst
 requirements.txt
 secrets_template.cfg
 setup.py
 emfacilities/__init__.py
 emfacilities/bibtex.py
 emfacilities/constants.py
-emfacilities/scipion_icon.gif
+emfacilities/protocols.conf
 emfacilities/protocols/__init__.py
 emfacilities/protocols/getnifs.py
+emfacilities/protocols/protocol_good_classes_extractor.py
 emfacilities/protocols/protocol_monitor.py
 emfacilities/protocols/protocol_monitor_2d_streamer.py
 emfacilities/protocols/protocol_monitor_ctf.py
 emfacilities/protocols/protocol_monitor_movie_gain.py
 emfacilities/protocols/protocol_monitor_summary.py
 emfacilities/protocols/protocol_monitor_system.py
 emfacilities/protocols/protocol_trackUsedItems.py
+emfacilities/protocols/protocol_volume_extractor.py
 emfacilities/protocols/pynvml.py
 emfacilities/protocols/report_html.py
 emfacilities/protocols/report_influx.py
 emfacilities/protocols/summary_provider.py
 emfacilities/protocols/transport.py
 emfacilities/templates/execution.summary.template.html
 emfacilities/templates/facility_SPA_streaming.json.template
 emfacilities/templates/to_2Dclassification_noDoseWeithed.json.template
 emfacilities/tests/__init__.py
 emfacilities/tests/protocols/__init__.py
+emfacilities/tests/protocols/test_protocol_good_classes_extractor.py
+emfacilities/tests/protocols/test_protocol_volume_extractor.py
 emfacilities/tests/protocols/test_protocols_ctf_monitor.py
 emfacilities/tests/protocols/test_protocols_ctf_streaming.py
 emfacilities/tests/protocols/test_protocols_system_monitor.py
 emfacilities/tests/workflows/__init__.py
 emfacilities/tests/workflows/test_workflow.py
 emfacilities/tests/workflows/test_workflow_high_throughput.py
 emfacilities/tests/workflows/test_workflow_streaming.py
 emfacilities/viewers/__init__.py
+emfacilities/viewers/viewer_good_classes_extractor.py
 emfacilities/viewers/viewer_monitors.py
 scipion_em_facilities.egg-info/PKG-INFO
 scipion_em_facilities.egg-info/SOURCES.txt
 scipion_em_facilities.egg-info/dependency_links.txt
 scipion_em_facilities.egg-info/entry_points.txt
 scipion_em_facilities.egg-info/requires.txt
 scipion_em_facilities.egg-info/top_level.txt
```

### Comparing `scipion-em-facilities-3.0.5/secrets_template.cfg` & `scipion-em-facilities-3.1.0/secrets_template.cfg`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.5/setup.py` & `scipion-em-facilities-3.1.0/setup.py`

 * *Files identical despite different names*

