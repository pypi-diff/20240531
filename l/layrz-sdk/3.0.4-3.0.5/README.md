# Comparing `tmp/layrz_sdk-3.0.4.tar.gz` & `tmp/layrz_sdk-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layrz_sdk-3.0.4.tar", last modified: Thu May 30 00:16:24 2024, max compression
+gzip compressed data, was "layrz_sdk-3.0.5.tar", last modified: Thu May 30 23:58:53 2024, max compression
```

## Comparing `layrz_sdk-3.0.4.tar` & `layrz_sdk-3.0.5.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:16:24.905996 layrz_sdk-3.0.4/
--rw-rw-r--   0 root         (0) root         (0)     1057 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1458 2024-05-30 00:16:24.905996 layrz_sdk-3.0.4/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      628 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:16:24.893996 layrz_sdk-3.0.4/layrz_sdk/
--rw-rw-r--   0 root         (0) root         (0)       28 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:16:24.893996 layrz_sdk-3.0.4/layrz_sdk/entities/
--rw-rw-r--   0 root         (0) root         (0)     1350 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:16:24.893996 layrz_sdk-3.0.4/layrz_sdk/entities/broadcasts/
--rw-rw-r--   0 root         (0) root         (0)      215 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/broadcasts/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      566 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/broadcasts/request.py
--rw-rw-r--   0 root         (0) root         (0)      586 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/broadcasts/response.py
--rw-rw-r--   0 root         (0) root         (0)     1291 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/broadcasts/result.py
--rw-rw-r--   0 root         (0) root         (0)      543 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/broadcasts/service.py
--rw-rw-r--   0 root         (0) root         (0)      569 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/broadcasts/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:16:24.897996 layrz_sdk-3.0.4/layrz_sdk/entities/cases/
--rw-rw-r--   0 root         (0) root         (0)      135 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/cases/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2786 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/cases/case.py
--rw-rw-r--   0 root         (0) root         (0)      902 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/cases/comment.py
--rw-rw-r--   0 root         (0) root         (0)      629 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/cases/trigger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:16:24.901996 layrz_sdk-3.0.4/layrz_sdk/entities/charts/
--rw-rw-r--   0 root         (0) root         (0)      806 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/charts/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      438 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/charts/alignment.py
--rw-rw-r--   0 root         (0) root         (0)     3867 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/charts/bar.py
--rw-rw-r--   0 root         (0) root         (0)     4928 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/charts/column.py
--rw-rw-r--   0 root         (0) root         (0)      514 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/charts/configuration.py
--rw-rw-r--   0 root         (0) root         (0)      447 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/charts/data_type.py
--rw-rw-r--   0 root         (0) root         (0)      558 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/charts/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)      995 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/charts/html.py
--rw-rw-r--   0 root         (0) root         (0)     6586 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/charts/line.py
--rw-rw-r--   0 root         (0) root         (0)     4230 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/charts/map.py
--rw-rw-r--   0 root         (0) root         (0)      811 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/charts/number.py
--rw-rw-r--   0 root         (0) root         (0)     2972 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/charts/pie.py
--rw-rw-r--   0 root         (0) root         (0)     3155 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/charts/radar.py
--rw-rw-r--   0 root         (0) root         (0)     3011 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/charts/radial_bar.py
--rw-rw-r--   0 root         (0) root         (0)      524 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/charts/render_technology.py
--rw-rw-r--   0 root         (0) root         (0)     4871 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/charts/scatter.py
--rw-rw-r--   0 root         (0) root         (0)     1509 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/charts/serie.py
--rw-rw-r--   0 root         (0) root         (0)      463 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/charts/serie_type.py
--rw-rw-r--   0 root         (0) root         (0)     1344 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/charts/table.py
--rw-rw-r--   0 root         (0) root         (0)     3985 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/charts/timeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:16:24.901996 layrz_sdk-3.0.4/layrz_sdk/entities/checkpoints/
--rw-rw-r--   0 root         (0) root         (0)      126 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/checkpoints/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1040 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/checkpoints/checkpoint.py
--rw-rw-r--   0 root         (0) root         (0)      653 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/checkpoints/geofence.py
--rw-rw-r--   0 root         (0) root         (0)     1236 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/checkpoints/waypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:16:24.901996 layrz_sdk-3.0.4/layrz_sdk/entities/events/
--rw-rw-r--   0 root         (0) root         (0)       49 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/events/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1175 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/events/event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:16:24.901996 layrz_sdk-3.0.4/layrz_sdk/entities/formatting/
--rw-rw-r--   0 root         (0) root         (0)       66 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/formatting/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      467 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/formatting/text_align.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:16:24.901996 layrz_sdk-3.0.4/layrz_sdk/entities/general/
--rw-rw-r--   0 root         (0) root         (0)      218 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/general/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1786 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/general/asset.py
--rw-rw-r--   0 root         (0) root         (0)      569 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/general/asset_operation_mode.py
--rw-rw-r--   0 root         (0) root         (0)      606 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/general/custom_field.py
--rw-rw-r--   0 root         (0) root         (0)      973 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/general/device.py
--rw-rw-r--   0 root         (0) root         (0)      615 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/general/sensor.py
--rw-rw-r--   0 root         (0) root         (0)      527 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/general/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:16:24.901996 layrz_sdk-3.0.4/layrz_sdk/entities/repcom/
--rw-rw-r--   0 root         (0) root         (0)       61 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/repcom/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1461 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/repcom/transaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:16:24.905996 layrz_sdk-3.0.4/layrz_sdk/entities/reports/
--rw-rw-r--   0 root         (0) root         (0)      249 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/reports/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1961 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/reports/col.py
--rw-rw-r--   0 root         (0) root         (0)      442 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/reports/format.py
--rw-rw-r--   0 root         (0) root         (0)     1408 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/reports/header.py
--rw-rw-r--   0 root         (0) root         (0)     1574 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/reports/page.py
--rw-rw-r--   0 root         (0) root         (0)     6444 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/reports/report.py
--rw-rw-r--   0 root         (0) root         (0)      881 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/reports/row.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:16:24.905996 layrz_sdk-3.0.4/layrz_sdk/entities/telemetry/
--rw-rw-r--   0 root         (0) root         (0)       87 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/telemetry/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      789 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/telemetry/message.py
--rw-rw-r--   0 root         (0) root         (0)     1327 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/entities/telemetry/position.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:16:24.905996 layrz_sdk-3.0.4/layrz_sdk/helpers/
--rw-rw-r--   0 root         (0) root         (0)       72 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/helpers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1102 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/helpers/color.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:16:24.905996 layrz_sdk-3.0.4/layrz_sdk/lcl/
--rw-rw-r--   0 root         (0) root         (0)       67 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/lcl/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    22987 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/layrz_sdk/lcl/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:16:24.905996 layrz_sdk-3.0.4/layrz_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1458 2024-05-30 00:16:24.000000 layrz_sdk-3.0.4/layrz_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2570 2024-05-30 00:16:24.000000 layrz_sdk-3.0.4/layrz_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 00:16:24.000000 layrz_sdk-3.0.4/layrz_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-30 00:16:24.000000 layrz_sdk-3.0.4/layrz_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-30 00:16:24.000000 layrz_sdk-3.0.4/layrz_sdk.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)     7589 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 00:16:24.905996 layrz_sdk-3.0.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:16:24.905996 layrz_sdk-3.0.4/tests/
--rw-rw-r--   0 root         (0) root         (0)    28784 2024-05-30 00:15:11.000000 layrz_sdk-3.0.4/tests/test_lcl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:53.261754 layrz_sdk-3.0.5/
+-rw-rw-r--   0 root         (0) root         (0)     1057 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1458 2024-05-30 23:58:53.261754 layrz_sdk-3.0.5/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      628 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:53.249754 layrz_sdk-3.0.5/layrz_sdk/
+-rw-rw-r--   0 root         (0) root         (0)       28 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:53.249754 layrz_sdk-3.0.5/layrz_sdk/entities/
+-rw-rw-r--   0 root         (0) root         (0)     1390 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:53.249754 layrz_sdk-3.0.5/layrz_sdk/entities/broadcasts/
+-rw-rw-r--   0 root         (0) root         (0)      215 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/broadcasts/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      566 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/broadcasts/request.py
+-rw-rw-r--   0 root         (0) root         (0)      586 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/broadcasts/response.py
+-rw-rw-r--   0 root         (0) root         (0)     1291 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/broadcasts/result.py
+-rw-rw-r--   0 root         (0) root         (0)      543 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/broadcasts/service.py
+-rw-rw-r--   0 root         (0) root         (0)      569 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/broadcasts/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:53.249754 layrz_sdk-3.0.5/layrz_sdk/entities/cases/
+-rw-rw-r--   0 root         (0) root         (0)      135 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/cases/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2786 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/cases/case.py
+-rw-rw-r--   0 root         (0) root         (0)      902 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/cases/comment.py
+-rw-rw-r--   0 root         (0) root         (0)      629 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/cases/trigger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:53.253754 layrz_sdk-3.0.5/layrz_sdk/entities/charts/
+-rw-rw-r--   0 root         (0) root         (0)      864 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/charts/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      437 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/charts/alignment.py
+-rw-rw-r--   0 root         (0) root         (0)     6212 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/charts/bar.py
+-rw-rw-r--   0 root         (0) root         (0)      734 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/charts/color.py
+-rw-rw-r--   0 root         (0) root         (0)     7244 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/charts/column.py
+-rw-rw-r--   0 root         (0) root         (0)     1181 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/charts/configuration.py
+-rw-rw-r--   0 root         (0) root         (0)      445 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/charts/data_type.py
+-rw-rw-r--   0 root         (0) root         (0)      558 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/charts/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)      995 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/charts/html.py
+-rw-rw-r--   0 root         (0) root         (0)     8153 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/charts/line.py
+-rw-rw-r--   0 root         (0) root         (0)     4357 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/charts/map.py
+-rw-rw-r--   0 root         (0) root         (0)     1118 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/charts/number.py
+-rw-rw-r--   0 root         (0) root         (0)     3886 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/charts/pie.py
+-rw-rw-r--   0 root         (0) root         (0)     3155 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/charts/radar.py
+-rw-rw-r--   0 root         (0) root         (0)     3931 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/charts/radial_bar.py
+-rw-rw-r--   0 root         (0) root         (0)      606 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/charts/render_technology.py
+-rw-rw-r--   0 root         (0) root         (0)     7586 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/charts/scatter.py
+-rw-rw-r--   0 root         (0) root         (0)     1509 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/charts/serie.py
+-rw-rw-r--   0 root         (0) root         (0)      463 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/charts/serie_type.py
+-rw-rw-r--   0 root         (0) root         (0)     1651 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/charts/table.py
+-rw-rw-r--   0 root         (0) root         (0)     3985 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/charts/timeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:53.257754 layrz_sdk-3.0.5/layrz_sdk/entities/checkpoints/
+-rw-rw-r--   0 root         (0) root         (0)      126 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/checkpoints/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1040 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/checkpoints/checkpoint.py
+-rw-rw-r--   0 root         (0) root         (0)      653 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/checkpoints/geofence.py
+-rw-rw-r--   0 root         (0) root         (0)     1236 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/checkpoints/waypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:53.257754 layrz_sdk-3.0.5/layrz_sdk/entities/events/
+-rw-rw-r--   0 root         (0) root         (0)       49 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/events/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1175 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/events/event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:53.257754 layrz_sdk-3.0.5/layrz_sdk/entities/formatting/
+-rw-rw-r--   0 root         (0) root         (0)       66 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/formatting/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      467 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/formatting/text_align.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:53.257754 layrz_sdk-3.0.5/layrz_sdk/entities/general/
+-rw-rw-r--   0 root         (0) root         (0)      218 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/general/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1786 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/general/asset.py
+-rw-rw-r--   0 root         (0) root         (0)      569 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/general/asset_operation_mode.py
+-rw-rw-r--   0 root         (0) root         (0)      606 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/general/custom_field.py
+-rw-rw-r--   0 root         (0) root         (0)      973 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/general/device.py
+-rw-rw-r--   0 root         (0) root         (0)      615 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/general/sensor.py
+-rw-rw-r--   0 root         (0) root         (0)      527 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/general/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:53.257754 layrz_sdk-3.0.5/layrz_sdk/entities/repcom/
+-rw-rw-r--   0 root         (0) root         (0)       61 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/repcom/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1461 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/repcom/transaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:53.257754 layrz_sdk-3.0.5/layrz_sdk/entities/reports/
+-rw-rw-r--   0 root         (0) root         (0)      249 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/reports/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1961 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/reports/col.py
+-rw-rw-r--   0 root         (0) root         (0)      442 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/reports/format.py
+-rw-rw-r--   0 root         (0) root         (0)     1408 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/reports/header.py
+-rw-rw-r--   0 root         (0) root         (0)     1574 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/reports/page.py
+-rw-rw-r--   0 root         (0) root         (0)     6444 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/reports/report.py
+-rw-rw-r--   0 root         (0) root         (0)      881 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/reports/row.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:53.261754 layrz_sdk-3.0.5/layrz_sdk/entities/telemetry/
+-rw-rw-r--   0 root         (0) root         (0)       87 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/telemetry/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      789 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/telemetry/message.py
+-rw-rw-r--   0 root         (0) root         (0)     1327 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/entities/telemetry/position.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:53.261754 layrz_sdk-3.0.5/layrz_sdk/helpers/
+-rw-rw-r--   0 root         (0) root         (0)       72 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/helpers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1102 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/helpers/color.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:53.261754 layrz_sdk-3.0.5/layrz_sdk/lcl/
+-rw-rw-r--   0 root         (0) root         (0)       67 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/lcl/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    22987 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/layrz_sdk/lcl/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:53.261754 layrz_sdk-3.0.5/layrz_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1458 2024-05-30 23:58:53.000000 layrz_sdk-3.0.5/layrz_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2605 2024-05-30 23:58:53.000000 layrz_sdk-3.0.5/layrz_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 23:58:53.000000 layrz_sdk-3.0.5/layrz_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-30 23:58:53.000000 layrz_sdk-3.0.5/layrz_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-30 23:58:53.000000 layrz_sdk-3.0.5/layrz_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)     7589 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 23:58:53.261754 layrz_sdk-3.0.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:53.261754 layrz_sdk-3.0.5/tests/
+-rw-rw-r--   0 root         (0) root         (0)    28784 2024-05-30 23:58:00.000000 layrz_sdk-3.0.5/tests/test_lcl.py
```

### Comparing `layrz_sdk-3.0.4/LICENSE` & `layrz_sdk-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/PKG-INFO` & `layrz_sdk-3.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layrz-sdk
-Version: 3.0.4
+Version: 3.0.5
 Summary: Layrz SDK for Python
 Author-email: "Golden M, Inc." <software@goldenm.com>
 Maintainer-email: Kenny Mochizuki <kenny@goldenm.com>, Luis Reyes <lreyes@goldenm.com>, Kasen Li <kli@goldenm.com>
 License: MIT License
 Project-URL: Repository, https://github.com/goldenm-software/layrz-sdk
 Project-URL: Changelog, https://github.com/goldenm-software/layrz-sdk/blob/main/CHANGELOG.md
 Keywords: sdk,goldenm,lcl,layrz compute language,layrz
```

### Comparing `layrz_sdk-3.0.4/README.md` & `layrz_sdk-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/__init__.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """ Init file """
 # Broadcast entities
 from .broadcasts import (BroadcastRequest, BroadcastResponse, BroadcastResult, BroadcastStatus, OutboundService)
 # Cases entitites
 from .cases import Case, CaseIgnoredStatus, CaseStatus, Comment, Trigger
 # Charts entities
-from .charts import (AreaChart, BarChart, ChartAlignment, ChartConfiguration, ChartDataSerie, ChartDataSerieType,
-                     ChartDataType, ChartException, ChartRenderTechnology, ColumnChart, HTMLChart, LineChart,
-                     MapCenterType, MapChart, MapPoint, NumberChart, PieChart, RadarChart, RadialBarChart, ScatterChart,
-                     ScatterSerie, ScatterSerieItem, TableChart, TableHeader, TableRow, TimelineChart, TimelineSerie,
-                     TimelineSerieItem)
+from .charts import (AreaChart, AxisConfig, BarChart, ChartAlignment, ChartColor, ChartConfiguration, ChartDataSerie,
+                     ChartDataSerieType, ChartDataType, ChartException, ChartRenderTechnology, ColumnChart, HTMLChart,
+                     LineChart, MapCenterType, MapChart, MapPoint, NumberChart, PieChart, RadarChart, RadialBarChart,
+                     ScatterChart, ScatterSerie, ScatterSerieItem, TableChart, TableHeader, TableRow, TimelineChart,
+                     TimelineSerie, TimelineSerieItem, get_color_list)
 # Checkpoints entities
 from .checkpoints import Checkpoint, Geofence, Waypoint
 # Events entities
 from .events import Event
 # Formatting entities
 from .formatting import TextAlignment
 # General entities
```

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/broadcasts/request.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/broadcasts/request.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/broadcasts/response.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/broadcasts/response.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/broadcasts/result.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/broadcasts/result.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/broadcasts/service.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/broadcasts/service.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/broadcasts/status.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/broadcasts/status.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/cases/case.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/cases/case.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/cases/comment.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/cases/comment.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/cases/trigger.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/cases/trigger.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/charts/bar.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/charts/radar.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-""" Bar chart """
+""" Radar chart """
 from .alignment import ChartAlignment
 from .exceptions import ChartException
 from .serie import ChartDataSerie
 from .serie_type import ChartDataSerieType
 
 
-class BarChart:
+class RadarChart:
   """
-  Bar chart configuration
+  Radar chart configuration
+
   """
 
   def __init__(
     self,
     x_axis: ChartDataSerie,
     y_axis: list[ChartDataSerie],
     title: str = 'Chart',
@@ -41,53 +42,20 @@
       raise ChartException('title must be an instance of str')
     self.title = title
 
     if not isinstance(align, ChartAlignment):
       raise ChartException('align must be an instance of ChartAlignment')
     self.align = align
 
-  def render(self, use_new_definition: bool = False) -> dict | list[dict]:
-    """
-    Render chart to a graphic Library.
-    We have two graphic libraries: GRAPHIC and APEXCHARTS.
-
-    GRAPHIC is a Flutter chart library. To return this option, use the parameter use_new_definition=True.
-    APEXCHARTS is a Javascript chart library. This is the default option.
-    """
-    if use_new_definition:
-      return {
-        'library': 'GRAPHIC',
-        'chart': 'BAR',
-        'configuration': self._render_graphic(),
-      }
-
-    return {
-      'library': 'APEXCHARTS',
-      'chart': 'BAR',
-      'configuration': self._render_apexcharts(),
-    }
-
-  def _render_graphic(self) -> list[dict]:
+  def render(self) -> dict:
     """
-    Converts the configuration of the chart to Flutter library graphic.
+    Render chart to a Javascript Library.
+    Currently only available for ApexCharts.
     """
-
-    series = []
-
-    for serie in self.y_axis:
-      for i, value in enumerate(serie.data):
-        x_axis = self.x_axis.data[i]
-        series.append({
-          'label': serie.label,
-          'color': serie.color,
-          'category': x_axis,
-          'value': value,
-        })
-
-    return series
+    return {'library': 'APEXCHARTS', 'configuration': self._render_apexcharts()}
 
   def _render_apexcharts(self) -> dict:
     """
     Converts the configuration of the chart to Javascript library ApexCharts.
     """
 
     series = []
@@ -105,43 +73,48 @@
     config = {
       'series': series,
       'colors': colors,
       'xaxis': {
         'categories': self.x_axis.data,
         'type': self.x_axis.data_type.value,
         'title': {
-          'text': self.x_axis.label
+          'text': self.x_axis.label,
+          'style': {
+            'fontFamily': 'Fira Sans Condensed',
+            'fontSize': '20px',
+            'fontWeight': 'normal'
+          }
         }
       },
       'title': {
         'text': self.title,
         'align': self.align.value,
         'style': {
           'fontFamily': 'Fira Sans Condensed',
           'fontSize': '20px',
           'fontWeight': 'normal'
         }
       },
-      'plotOptions': {
-        'bar': {
-          'horizontal': True,
-          'borderRadius': 4
-        }
-      },
-      'dataLabels': {
-        'enabled': False
-      },
       'chart': {
-        'type': 'bar',
+        'type': 'radar',
         'animations': {
           'enabled': False
         },
         'toolbar': {
           'show': False
         },
         'zoom': {
           'enabled': False
         }
+      },
+      'dataLabels': {
+        'enabled': True
+      },
+      'plotOptions': {
+        'bar': {
+          'horizontal': True,
+          'borderRadius': 4
+        }
       }
     }
 
     return config
```

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/charts/exceptions.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/charts/exceptions.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/charts/html.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/charts/html.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/charts/line.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/charts/column.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,45 @@
-""" Line chart """
+""" Column chart """
+from layrz_sdk.helpers import convert_to_rgba
 
 from .alignment import ChartAlignment
-from .data_type import ChartDataType
+from .configuration import AxisConfig
 from .exceptions import ChartException
 from .render_technology import ChartRenderTechnology
 from .serie import ChartDataSerie
 from .serie_type import ChartDataSerieType
 
 
-class LineChart:
+class ColumnChart:
   """
-  Line chart configuration
+  Column chart configuration
 
   """
 
   def __init__(
     self,
     x_axis: ChartDataSerie,
     y_axis: list[ChartDataSerie],
     title: str = 'Chart',
     align: ChartAlignment = ChartAlignment.CENTER,
+    x_axis_config: AxisConfig = None,
+    y_axis_config: AxisConfig = None,
   ) -> None:
     """
     Constructor
     ----
     Arguments
       - x_axis : Defines the X Axis of the chart, uses the ChartDataSerie class.
                  Please read the documentation to more information.
       - y_axis : Defines the Y Axis of the chart, uses the ChartDataSerie class.
                  Please read the documentation to more information.
       - title : Title of the chart
       - align : Alignment of the title
+      - x_axis_config : Configuration of the X Axis
+      - y_axis_config : Configuration of the Y Axis
     """
     for i, serie in enumerate(y_axis):
       if not isinstance(serie, ChartDataSerie):
         raise ChartException(f'Y Axis serie {i} must be an instance of ChartDataSerie')
     self.y_axis = y_axis
 
     if not isinstance(x_axis, ChartDataSerie):
@@ -45,185 +50,204 @@
       raise ChartException('title must be an instance of str')
     self.title = title
 
     if not isinstance(align, ChartAlignment):
       raise ChartException('align must be an instance of ChartAlignment')
     self.align = align
 
-  def render(self, technology: ChartRenderTechnology) -> dict | list[dict]:
+    if x_axis_config is None:
+      x_axis_config = AxisConfig()
+
+    if not isinstance(x_axis_config, AxisConfig):
+      raise ChartException('x_axis_config must be an instance of AxisConfig')
+    self.x_axis_config = x_axis_config
+
+    if y_axis_config is None:
+      y_axis_config = AxisConfig()
+
+    if not isinstance(y_axis_config, AxisConfig):
+      raise ChartException('y_axis_config must be an instance of AxisConfig')
+    self.y_axis_config = y_axis_config
+
+  def render(
+    self,
+    technology: ChartRenderTechnology = ChartRenderTechnology.SYNCFUSION_FLUTTER_CHARTS,
+  ) -> dict:
     """
     Render chart to a graphic Library.
-    We have two graphic libraries: GRAPHIC and CANVASJS.
+    We have two graphic libraries: GRAPHIC and APEXCHARTS.
 
     GRAPHIC is a Flutter chart library. To return this option, use the parameter use_new_definition=True.
-    CANVASJS is a Javascript chart library. This is the default option.
+    APEXCHARTS is a Javascript chart library. This is the default option.
     """
-
     if technology == ChartRenderTechnology.GRAPHIC:
       return {
         'library': 'GRAPHIC',
-        'chart': 'LINE',
+        'chart': 'COLUMN',
         'configuration': self._render_graphic(),
       }
 
     if technology == ChartRenderTechnology.SYNCFUSION_FLUTTER_CHARTS:
       return {
         'library': 'SYNCFUSION_FLUTTER_CHARTS',
-        'chart': 'LINE',
+        'chart': 'COLUMN',
         'configuration': self._render_syncfusion_flutter_charts(),
       }
 
+    if technology == ChartRenderTechnology.APEX_CHARTS:
+      return {
+        'library': 'APEXCHARTS',
+        'chart': 'COLUMN',
+        'configuration': self._render_apexcharts(),
+      }
+
     return {
-      'library': 'CANVASJS',
-      'chart': 'LINE',
-      'configuration': self._render_canvasjs(),
+      'library': 'FLUTTER',
+      'chart': 'TEXT',
+      'configuration': [f'Unsupported {technology}'],
     }
 
-  def _render_syncfusion_flutter_charts(self) -> list[dict]:
-    """ 
-    Converts the configuration of the chart to a Flutter library syncfusion_flutter_charts.
+  def _render_syncfusion_flutter_charts(self) -> dict:
+    """
+    Converts the configuration of the chart to Syncfusion Flutter Charts.
     """
     series = []
 
     for serie in self.y_axis:
-      if serie.serie_type not in [ChartDataSerieType.LINE, ChartDataSerieType.AREA]:
-        continue
-
-      points = []
-
-      for i, value in enumerate(self.x_axis.data):
-        x_value = value.timestamp() if self.x_axis.data_type == ChartDataType.DATETIME else value
-        if not isinstance(x_value, (int, float)):
-          continue
-
-        y_value = serie.data[i]
-        if isinstance(y_value, bool):
-          if y_value:
-            y_value = 1
-          else:
-            y_value = 0
-
-        if not isinstance(y_value, (int, float)):
-          continue
-
-        points.append({
-          'xAxis': x_value,
-          'yAxis': y_value,
-        })
+      values = []
+      for i, value in enumerate(serie.data):
+        x_axis = self.x_axis.data[i]
+        values.append({'xAxis': x_axis, 'yAxis': value})
 
       series.append({
-        'color': serie.color,
-        'values': points,
         'label': serie.label,
-        'type': 'AREA' if serie.serie_type == ChartDataSerieType.AREA else 'LINE',
+        'color': serie.color,
+        'values': values,
       })
 
-    return series
+    return {
+      'series': series,
+      'xAxis': {
+        'label': self.x_axis_config.label,
+        'measureUnit': self.x_axis_config.measure_unit,
+        'dataType': self.x_axis_config.data_type.value,
+        'minValue': self.x_axis_config.min_value,
+        'maxValue': self.x_axis_config.max_value,
+      },
+      'yAxis': {
+        'label': self.y_axis_config.label,
+        'measureUnit': self.y_axis_config.measure_unit,
+        'dataType': self.y_axis_config.data_type.value,
+        'minValue': self.y_axis_config.min_value,
+        'maxValue': self.y_axis_config.max_value,
+      },
+    }
 
   def _render_graphic(self) -> list[dict]:
     """
-    Converts the configuration of the chart to a Flutter library Graphic.
+    Converts the configuration of the chart to Flutter library graphic.
     """
+
     series = []
 
     for serie in self.y_axis:
-      if serie.serie_type not in [ChartDataSerieType.LINE, ChartDataSerieType.AREA]:
-        continue
-
-      points = []
-
-      for i, value in enumerate(self.x_axis.data):
-        points.append({
-          'x_axis': {
-            'value': value.timestamp() if self.x_axis.data_type == ChartDataType.DATETIME else value,
-            'is_datetime': self.x_axis.data_type == ChartDataType.DATETIME,
-          },
-          'y_axis': serie.data[i],
+      for i, value in enumerate(serie.data):
+        x_axis = self.x_axis.data[i]
+        series.append({
+          'label': serie.label,
+          'color': serie.color,
+          'category': x_axis,
+          'value': value,
         })
 
-      series.append({
-        'group': serie.label,
-        'color': serie.color,
-        'dashed': serie.serie_type == ChartDataSerieType.LINE and serie.dashed,
-        'type': 'AREA' if serie.serie_type == ChartDataSerieType.AREA else 'LINE',
-        'values': points
-      })
-
     return series
 
-  def _render_canvasjs(self) -> dict:
+  def _render_apexcharts(self) -> dict:
     """
-    Converts the configuration of the chart to Javascript library CanvasJS.
+    Converts the configuration of the chart to Javascript library ApexCharts.
     """
-    datasets = []
+
+    series = []
+    colors = []
+    stroke = {'width': [], 'dashArray': []}
+    markers = []
 
     for serie in self.y_axis:
-      dataset = {
-        'type': 'line',
+      modified_serie = {
         'name': serie.label,
-        'connectNullData': True,
-        'nullDataLineDashType': 'solid',
-        'showInLegend': True,
-        'color': serie.color,
-        'markerSize': 3,
       }
+      if serie.serie_type == ChartDataSerieType.SCATTER:
+        modified_serie['data'] = [{'x': item.x, 'y': item.y} for item in serie.data]
+        modified_serie['type'] = 'scatter'
+        stroke['width'].append(0)
+        markers.append(10)
+      else:
+        modified_serie['data'] = [{'x': self.x_axis.data[i], 'y': item} for i, item in enumerate(serie.data)]
 
-      if serie.serie_type != ChartDataSerieType.NONE:
-        dataset['type'] = serie.serie_type.value
-
-      if serie.serie_type == ChartDataSerieType.AREA:
-        dataset['fillOpacity'] = 0.3
-
-      if self.x_axis.data_type == ChartDataType.DATETIME:
-        dataset['xValueType'] = 'dateTime'
-        dataset['xValueFormatString'] = 'YYYY-MM-DD HH:mm:ss TT'
+        if serie.serie_type is not ChartDataSerieType.NONE:
+          modified_serie['type'] = serie.serie_type.value
+        else:
+          modified_serie['type'] = 'column'
+
+        if serie.dashed and serie.serie_type == ChartDataSerieType.LINE:
+          stroke['dashArray'].append(5)
+        else:
+          stroke['dashArray'].append(0)
 
-      if serie.serie_type == ChartDataSerieType.LINE and serie.dashed:
-        dataset['lineDashType'] = 'dash'
-        dataset['markerSize'] = 0
+        stroke['width'].append(3)
+        markers.append(0)
 
-      points = []
+      series.append(modified_serie)
 
-      if serie.serie_type == ChartDataSerieType.SCATTER:
-        for point in serie.data:
-          points.append({'x': point.x, 'y': point.y})
+      if serie.serie_type == ChartDataSerieType.AREA:
+        color = convert_to_rgba(serie.color)
+        colors.append(f'rgba({color[0]}, {color[1]}, {color[2]}, 0.5)')
       else:
-        for i, value in enumerate(self.x_axis.data):
-          points.append({
-            'x': (value.timestamp() * 1000) if self.x_axis.data_type == ChartDataType.DATETIME else value,
-            'y': serie.data[i],
-          })
-
-      dataset['dataPoints'] = points
-      datasets.append(dataset)
+        colors.append(serie.color)
 
-    return {
-      'animationEnabled': False,
-      'zoomEnabled': True,
+    config = {
+      'series': series,
+      'colors': colors,
+      'xaxis': {
+        'type': self.x_axis.data_type.value,
+        'title': {
+          'text': self.x_axis.label,
+          'style': {
+            'fontFamily': 'Fira Sans Condensed',
+            'fontSize': '20px',
+            'fontWeight': 'normal'
+          }
+        }
+      },
+      'dataLabels': {
+        'enabled': False
+      },
       'title': {
         'text': self.title,
-        'fontFamily': 'Fira Sans Condensed',
-        'fontSize': 20,
-        'horizontalAlign': self.align.value
-      },
-      'data': datasets,
-      'axisX': {
-        'title': self.x_axis.label,
-        'titleFontFamily': 'Fira Sans Condensed',
-        'titleFontSize': 20,
-      },
-      'toolTip': {
-        'animationEnabled': False,
-        'shared': True
+        'align': self.align.value,
+        'style': {
+          'fontFamily': 'Fira Sans Condensed',
+          'fontSize': '20px',
+          'fontWeight': 'normal'
+        }
       },
-      'legend': {
-        'cursor': 'pointer'
+      'markers': {
+        'size': markers
+      },
+      'fill': {
+        'type': 'solid'
+      },
+      'stroke': stroke,
+      'chart': {
+        'animations': {
+          'enabled': False
+        },
+        'toolbar': {
+          'show': False
+        },
+        'zoom': {
+          'enabled': False
+        }
       }
     }
 
-
-class AreaChart(LineChart):
-  """
-  Line chart
-  
-  Deprecation warning: This class will be removed in the next version. Use LineChart instead.
-  """
+    return config
```

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/charts/map.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/charts/map.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ Map chart """
 from enum import Enum
 
 from .exceptions import ChartException
+from .render_technology import ChartRenderTechnology
 
 
 class MapCenterType(Enum):
   """
   Map Chart center type
   """
   FIXED = 'FIXED'
@@ -95,33 +96,33 @@
       raise ChartException('center must be an instance of MapCenterType')
     self.center = center
 
     if self.center == MapCenterType.FIXED and not isinstance(center_latlng, (list, tuple)):
       raise ChartException('center_latlng must be an instance of list or tuple')
     self.center_latlng = center_latlng
 
-  def render(self, use_new_definition: bool = False) -> dict:
+  def render(self, technology: ChartRenderTechnology = ChartRenderTechnology.FLUTTER_MAP) -> dict:
     """
     Render chart to a graphic Library.
     We have two graphic libraries: FLUTTER_MAP and LEAFLET.
 
     FLUTTER_MAP is a Flutter chart library. To return this option, use the parameter use_new_definition=True.
     LEAFLET is a Javascript chart library. This is the default option.
     """
-    if use_new_definition:
+    if technology == ChartRenderTechnology.FLUTTER_MAP:
       return {
         'library': 'FLUTTER_MAP',
         'chart': 'MAP',
         'configuration': self._render_flutter_map(),
       }
 
     return {
-      'library': 'LEAFLET',
-      'chart': 'MAP',
-      'configuration': self._render_leaflet(),
+      'library': 'FLUTTER',
+      'chart': 'TEXT',
+      'configuration': [f'Unsupported {technology}'],
     }
 
   def _render_flutter_map(self) -> dict:
     """
     Converts the configuration to the chart to Flutter Map engine.
     """
     points = []
```

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/charts/pie.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/charts/radial_bar.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-""" Pie chart """
+""" Radial Bar chart """
 from .alignment import ChartAlignment
 from .exceptions import ChartException
+from .render_technology import ChartRenderTechnology
 from .serie import ChartDataSerie
 
 
-class PieChart:
+class RadialBarChart:
   """
-  Pie chart configuration
+  Radial Bar chart configuration
   """
 
   def __init__(
     self,
     series: list[ChartDataSerie],
     title: str = 'Chart',
     align: ChartAlignment = ChartAlignment.CENTER,
@@ -33,34 +34,67 @@
       raise ChartException('title must be an instance of str')
     self.title = title
 
     if not isinstance(align, ChartAlignment):
       raise ChartException('align must be an instance of ChartAlignment')
     self.align = align
 
-  def render(self, use_new_definition: bool = False) -> dict | list[dict]:
+  def render(
+    self,
+    technology: ChartRenderTechnology = ChartRenderTechnology.SYNCFUSION_FLUTTER_CHARTS,
+  ) -> dict | list[dict]:
     """
     Render chart to a graphic Library.
     We have two graphic libraries: GRAPHIC and CANVASJS.
 
     GRAPHIC is a Flutter chart library. To return this option, use the parameter use_new_definition=True.
     CANVASJS is a Javascript chart library. This is the default option.
     """
-    if use_new_definition:
+    if technology == ChartRenderTechnology.GRAPHIC:
       return {
         'library': 'GRAPHIC',
-        'chart': 'PIE',
+        'chart': 'RADIALBAR',
         'configuration': self._render_graphic(),
       }
+
+    if technology == ChartRenderTechnology.APEX_CHARTS:
+      return {
+        'library': 'APEXCHARTS',
+        'chart': 'RADIALBAR',
+        'configuration': self._render_apexcharts(),
+      }
+
+    if technology == ChartRenderTechnology.SYNCFUSION_FLUTTER_CHARTS:
+      return {
+        'library': 'SYNCFUSION_FLUTTER_CHARTS',
+        'chart': 'RADIALBAR',
+        'configuration': self._render_syncfusion_flutter_charts(),
+      }
+
     return {
-      'library': 'APEXCHARTS',
-      'chart': 'PIE',
-      'configuration': self._render_apexcharts(),
+      'library': 'FLUTTER',
+      'chart': 'TEXT',
+      'configuration': [f'Unsupported {technology}'],
     }
 
+  def _render_syncfusion_flutter_charts(self) -> dict:
+    """
+    Converts the configuration of the chart to Syncfusion Flutter Charts.
+    """
+    series = []
+
+    for serie in self.series:
+      series.append({
+        'label': serie.label,
+        'color': serie.color,
+        'value': serie.data[0],
+      })
+
+    return {'series': series}
+
   def _render_graphic(self) -> list[dict]:
     """
     Converts the configuration of the chart to a Flutter library Graphic.
     """
     series = []
 
     for serie in self.series:
@@ -96,24 +130,24 @@
         'style': {
           'fontFamily': 'Fira Sans Condensed',
           'fontSize': '20px',
           'fontWeight': 'normal'
         }
       },
       'chart': {
-        'type': 'pie',
+        'type': 'radialBar',
         'animations': {
           'enabled': False
         },
         'toolbar': {
           'show': False
         },
         'zoom': {
           'enabled': False
         }
       },
       'dataLabels': {
         'enabled': True
-      }
+      },
     }
 
     return config
```

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/charts/radial_bar.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/charts/pie.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-""" Radial Bar chart """
+""" Pie chart """
 from .alignment import ChartAlignment
 from .exceptions import ChartException
+from .render_technology import ChartRenderTechnology
 from .serie import ChartDataSerie
 
 
-class RadialBarChart:
+class PieChart:
   """
-  Radial Bar chart configuration
+  Pie chart configuration
   """
 
   def __init__(
     self,
     series: list[ChartDataSerie],
     title: str = 'Chart',
     align: ChartAlignment = ChartAlignment.CENTER,
@@ -33,34 +34,67 @@
       raise ChartException('title must be an instance of str')
     self.title = title
 
     if not isinstance(align, ChartAlignment):
       raise ChartException('align must be an instance of ChartAlignment')
     self.align = align
 
-  def render(self, use_new_definition: bool = False) -> dict | list[dict]:
+  def render(
+    self,
+    technology: ChartRenderTechnology = ChartRenderTechnology.SYNCFUSION_FLUTTER_CHARTS,
+  ) -> dict | list[dict]:
     """
     Render chart to a graphic Library.
     We have two graphic libraries: GRAPHIC and CANVASJS.
 
     GRAPHIC is a Flutter chart library. To return this option, use the parameter use_new_definition=True.
     CANVASJS is a Javascript chart library. This is the default option.
     """
-    if use_new_definition:
+    if technology == ChartRenderTechnology.GRAPHIC:
       return {
         'library': 'GRAPHIC',
-        'chart': 'RADIALBAR',
+        'chart': 'PIE',
         'configuration': self._render_graphic(),
       }
+
+    if technology == ChartRenderTechnology.SYNCFUSION_FLUTTER_CHARTS:
+      return {
+        'library': 'SYNCFUSION_FLUTTER_CHARTS',
+        'chart': 'PIE',
+        'configuration': self._render_syncfusion_flutter_charts(),
+      }
+
+    if technology == ChartRenderTechnology.APEX_CHARTS:
+      return {
+        'library': 'APEXCHARTS',
+        'chart': 'PIE',
+        'configuration': self._render_apexcharts(),
+      }
+
     return {
-      'library': 'APEXCHARTS',
-      'chart': 'RADIALBAR',
-      'configuration': self._render_apexcharts(),
+      'library': 'FLUTTER',
+      'chart': 'TEXT',
+      'configuration': [f'Unsupported {technology}'],
     }
 
+  def _render_syncfusion_flutter_charts(self) -> dict:
+    """
+    Converts the configuration of the chart to Syncfusion Flutter Charts.
+    """
+    series = []
+
+    for serie in self.series:
+      series.append({
+        'label': serie.label,
+        'color': serie.color,
+        'value': serie.data[0],
+      })
+
+    return {'series': series}
+
   def _render_graphic(self) -> list[dict]:
     """
     Converts the configuration of the chart to a Flutter library Graphic.
     """
     series = []
 
     for serie in self.series:
@@ -96,24 +130,24 @@
         'style': {
           'fontFamily': 'Fira Sans Condensed',
           'fontSize': '20px',
           'fontWeight': 'normal'
         }
       },
       'chart': {
-        'type': 'radialBar',
+        'type': 'pie',
         'animations': {
           'enabled': False
         },
         'toolbar': {
           'show': False
         },
         'zoom': {
           'enabled': False
         }
       },
       'dataLabels': {
         'enabled': True
-      },
+      }
     }
 
     return config
```

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/charts/render_technology.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/charts/render_technology.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 class ChartRenderTechnology(Enum):
   """
   Chart Alignment
   """
   CANVAS_JS = 'CANVAS_JS'
   GRAPHIC = 'GRAPHIC'
   SYNCFUSION_FLUTTER_CHARTS = 'SYNCFUSION_FLUTTER_CHARTS'
+  FLUTTER_MAP = 'FLUTTER_MAP'
+  APEX_CHARTS = 'APEX_CHARTS'
+  FLUTTER = 'FLUTTER'
 
   @property
   def _readable(self) -> str:
     """ Readable """
     return f'ChartRenderTechnology.{self.value}'
 
   def __str__(self) -> str:
```

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/charts/serie.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/charts/serie.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   """
 
   def __init__(
     self,
     data: list[float | int | bool],
     color: str = '#000000',
     label: str = '',
-    serie_type: ChartDataSerieType = ChartDataSerieType.NONE,
+    serie_type: ChartDataSerieType = ChartDataSerieType.LINE,
     data_type: ChartDataType = ChartDataType.NUMBER,
     dashed: bool = False,
   ):
     """
     Constructor
 
     Args
```

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/charts/table.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/charts/table.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ Number chart """
+from .render_technology import ChartRenderTechnology
 
 
 class TableHeader:
   """ Table header chart configuration """
 
   def __init__(self, label: str, key: str) -> None:
     """ Constructor
@@ -39,22 +40,29 @@
     Arguments
       - columns : List of columns
       - rows : List of rows
     """
     self.columns = columns
     self.rows = rows
 
-  def render(self) -> dict:
+  def render(self, technology: ChartRenderTechnology = ChartRenderTechnology.FLUTTER) -> dict:
     """
     Render chart to a graphic Library.
     """
+    if technology == ChartRenderTechnology.FLUTTER:
+      return {
+        'library': 'FLUTTER',
+        'chart': 'TABLE',
+        'configuration': self._render_flutter(),
+      }
+
     return {
       'library': 'FLUTTER',
-      'chart': 'TABLE',
-      'configuration': self._render_flutter(),
+      'chart': 'TEXT',
+      'configuration': [f'Unsupported {technology}'],
     }
 
   def _render_flutter(self) -> dict:
     """
     Converts the configuration of the chart to a Flutter native components.
     """
     return {
```

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/charts/timeline.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/charts/timeline.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/checkpoints/checkpoint.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/checkpoints/checkpoint.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/checkpoints/geofence.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/checkpoints/geofence.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/checkpoints/waypoint.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/checkpoints/waypoint.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/events/event.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/events/event.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/general/asset.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/general/asset.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/general/asset_operation_mode.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/general/asset_operation_mode.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/general/custom_field.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/general/custom_field.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/general/device.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/general/device.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/general/sensor.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/general/sensor.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/general/user.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/general/user.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/repcom/transaction.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/repcom/transaction.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/reports/col.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/reports/col.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/reports/header.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/reports/header.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/reports/page.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/reports/page.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/reports/report.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/reports/report.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/reports/row.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/reports/row.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/telemetry/message.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/telemetry/message.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/entities/telemetry/position.py` & `layrz_sdk-3.0.5/layrz_sdk/entities/telemetry/position.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/helpers/color.py` & `layrz_sdk-3.0.5/layrz_sdk/helpers/color.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk/lcl/core.py` & `layrz_sdk-3.0.5/layrz_sdk/lcl/core.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.4/layrz_sdk.egg-info/PKG-INFO` & `layrz_sdk-3.0.5/layrz_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layrz-sdk
-Version: 3.0.4
+Version: 3.0.5
 Summary: Layrz SDK for Python
 Author-email: "Golden M, Inc." <software@goldenm.com>
 Maintainer-email: Kenny Mochizuki <kenny@goldenm.com>, Luis Reyes <lreyes@goldenm.com>, Kasen Li <kli@goldenm.com>
 License: MIT License
 Project-URL: Repository, https://github.com/goldenm-software/layrz-sdk
 Project-URL: Changelog, https://github.com/goldenm-software/layrz-sdk/blob/main/CHANGELOG.md
 Keywords: sdk,goldenm,lcl,layrz compute language,layrz
```

### Comparing `layrz_sdk-3.0.4/layrz_sdk.egg-info/SOURCES.txt` & `layrz_sdk-3.0.5/layrz_sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 layrz_sdk/entities/cases/__init__.py
 layrz_sdk/entities/cases/case.py
 layrz_sdk/entities/cases/comment.py
 layrz_sdk/entities/cases/trigger.py
 layrz_sdk/entities/charts/__init__.py
 layrz_sdk/entities/charts/alignment.py
 layrz_sdk/entities/charts/bar.py
+layrz_sdk/entities/charts/color.py
 layrz_sdk/entities/charts/column.py
 layrz_sdk/entities/charts/configuration.py
 layrz_sdk/entities/charts/data_type.py
 layrz_sdk/entities/charts/exceptions.py
 layrz_sdk/entities/charts/html.py
 layrz_sdk/entities/charts/line.py
 layrz_sdk/entities/charts/map.py
```

### Comparing `layrz_sdk-3.0.4/pyproject.toml` & `layrz_sdk-3.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "layrz-sdk"
-version = "3.0.4"
+version = "3.0.5"
 description = "Layrz SDK for Python"
 authors = [
   {name = "Golden M, Inc.", email = "software@goldenm.com"}
 ]
 requires-python = ">=3.10"
 
 maintainers = [
```

### Comparing `layrz_sdk-3.0.4/tests/test_lcl.py` & `layrz_sdk-3.0.5/tests/test_lcl.py`

 * *Files identical despite different names*

