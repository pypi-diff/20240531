# Comparing `tmp/xurpas_data_quality-1.0.1.tar.gz` & `tmp/xurpas_data_quality-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xurpas_data_quality-1.0.1.tar", last modified: Thu May 30 06:25:54 2024, max compression
+gzip compressed data, was "xurpas_data_quality-1.0.2.tar", last modified: Thu May 30 13:40:48 2024, max compression
```

## Comparing `xurpas_data_quality-1.0.1.tar` & `xurpas_data_quality-1.0.2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 06:25:54.026063 xurpas_data_quality-1.0.1/
--rw-rw-rw-   0        0        0      110 2024-05-07 06:47:23.000000 xurpas_data_quality-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2375 2024-05-30 06:25:54.024177 xurpas_data_quality-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1745 2024-05-30 03:36:27.000000 xurpas_data_quality-1.0.1/README.md
--rw-rw-rw-   0        0        0      871 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-30 06:25:54.026063 xurpas_data_quality-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1166 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 06:25:53.881181 xurpas_data_quality-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-30 06:25:53.904677 xurpas_data_quality-1.0.1/src/xurpas_data_quality/
--rw-rw-rw-   0        0        0       59 2024-05-30 06:24:56.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 06:25:53.926531 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/
--rw-rw-rw-   0        0        0      306 2024-05-24 06:43:35.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 06:25:53.928617 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/alerts/
--rw-rw-rw-   0        0        0        0 2024-05-03 07:10:29.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/alerts/__init__.py
--rw-rw-rw-   0        0        0      953 2024-05-06 00:02:03.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/alerts/alerts.py
-drwxrwxrwx   0        0        0        0 2024-05-30 06:25:53.931098 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/algorithms/
--rw-rw-rw-   0        0        0      105 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/algorithms/__init__.py
--rw-rw-rw-   0        0        0      598 2024-05-24 06:08:48.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/algorithms/algorithms.py
--rw-rw-rw-   0        0        0      344 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/algorithms/summary_algorithms.py
--rw-rw-rw-   0        0        0      117 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/correlations.py
--rw-rw-rw-   0        0        0     1370 2024-05-24 06:13:00.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/dataframe.py
--rw-rw-rw-   0        0        0     6756 2024-05-24 06:45:08.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/describe.py
--rw-rw-rw-   0        0        0     2697 2024-05-27 02:20:43.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/describe_new.py
--rw-rw-rw-   0        0        0     2041 2024-05-30 06:23:27.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/describer.py
--rw-rw-rw-   0        0        0      224 2024-05-06 01:15:30.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/descriptions.py
--rw-rw-rw-   0        0        0      350 2024-04-26 07:12:37.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/pandas_dataframe.py
--rw-rw-rw-   0        0        0     1238 2024-05-30 06:09:15.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/series_describe.py
-drwxrwxrwx   0        0        0        0 2024-05-30 06:25:53.938825 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/type_descriptions/
--rw-rw-rw-   0        0        0      192 2024-05-30 06:14:41.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/type_descriptions/__init__.py
--rw-rw-rw-   0        0        0     1681 2024-05-27 07:17:52.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/type_descriptions/describe_categorical.py
--rw-rw-rw-   0        0        0      899 2024-05-30 06:23:13.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/type_descriptions/describe_date.py
--rw-rw-rw-   0        0        0      989 2024-05-27 01:57:05.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/type_descriptions/describe_generic.py
--rw-rw-rw-   0        0        0     3192 2024-05-30 06:22:46.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/type_descriptions/describe_numeric.py
--rw-rw-rw-   0        0        0      831 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/typeset.py
--rw-rw-rw-   0        0        0      570 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/utils.py
--rw-rw-rw-   0        0        0     3247 2024-05-30 06:02:21.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data_report.py
--rw-rw-rw-   0        0        0        0 2024-05-07 06:51:12.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/py.typed
-drwxrwxrwx   0        0        0        0 2024-05-30 06:25:53.945254 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/
--rw-rw-rw-   0        0        0        0 2024-05-07 05:20:40.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/__init__.py
--rw-rw-rw-   0        0        0      801 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/handler.py
--rw-rw-rw-   0        0        0     5621 2024-05-24 06:52:30.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render.py
-drwxrwxrwx   0        0        0        0 2024-05-30 06:25:53.962697 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/
--rw-rw-rw-   0        0        0      181 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 06:25:53.973332 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/bottom/
--rw-rw-rw-   0        0        0        0 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/bottom/__init__.py
--rw-rw-rw-   0        0        0     2095 2024-05-27 07:28:54.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/bottom/render_bottom_categorical.py
--rw-rw-rw-   0        0        0      518 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/bottom/render_bottom_date.py
--rw-rw-rw-   0        0        0     1571 2024-05-27 00:41:33.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/bottom/render_bottom_numerical.py
--rw-rw-rw-   0        0        0     1158 2024-05-27 05:11:03.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/render_categorical.py
--rw-rw-rw-   0        0        0     1148 2024-05-30 06:23:58.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/render_date.py
--rw-rw-rw-   0        0        0      586 2024-05-27 00:26:47.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/render_generic.py
--rw-rw-rw-   0        0        0     1757 2024-05-27 00:46:11.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/render_numerical.py
--rw-rw-rw-   0        0        0     4608 2024-05-27 02:18:47.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/renderer.py
--rw-rw-rw-   0        0        0      569 2024-05-14 04:40:10.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/template_loader.py
-drwxrwxrwx   0        0        0        0 2024-05-30 06:25:53.995211 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:20:52.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 06:25:53.995211 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/assets/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:21:04.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/assets/__init__.py
--rw-rw-rw-   0        0        0      594 2024-05-06 06:23:01.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/assets/script.js
--rw-rw-rw-   0        0        0      684 2024-05-27 00:34:57.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/assets/style.css
--rw-rw-rw-   0        0        0      249 2024-05-06 06:04:16.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/base.html
--rw-rw-rw-   0        0        0      106 2024-05-01 16:04:49.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/collapse.html
-drwxrwxrwx   0        0        0        0 2024-05-30 06:25:54.012350 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/containers/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:21:13.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/containers/__init__.py
--rw-rw-rw-   0        0        0      209 2024-04-30 07:01:56.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/containers/box.html
--rw-rw-rw-   0        0        0       78 2024-05-03 02:13:15.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/containers/column.html
--rw-rw-rw-   0        0        0      141 2024-05-03 02:44:57.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/containers/default.html
--rw-rw-rw-   0        0        0      340 2024-05-01 12:08:46.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/containers/sections.html
--rw-rw-rw-   0        0        0      835 2024-05-01 16:36:14.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/containers/tabs.html
--rw-rw-rw-   0        0        0       72 2024-05-06 02:07:52.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/containers/test.html
--rw-rw-rw-   0        0        0      277 2024-05-06 05:58:23.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/dropdown.html
--rw-rw-rw-   0        0        0      268 2024-04-29 06:44:51.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/navigation.html
--rw-rw-rw-   0        0        0      407 2024-05-27 02:32:44.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/plot.html
--rw-rw-rw-   0        0        0      449 2024-05-06 06:03:50.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/script.html
--rw-rw-rw-   0        0        0      267 2024-05-06 06:03:51.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/style.html
--rw-rw-rw-   0        0        0      390 2024-05-06 00:49:14.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/table.html
--rw-rw-rw-   0        0        0      300 2024-05-02 00:52:44.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/toggle.html
--rw-rw-rw-   0        0        0      510 2024-05-27 00:51:20.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/variable.html
-drwxrwxrwx   0        0        0        0 2024-05-30 06:25:54.016525 xurpas_data_quality-1.0.1/src/xurpas_data_quality/report/
--rw-rw-rw-   0        0        0       73 2024-05-24 06:08:48.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/report/__init__.py
--rw-rw-rw-   0        0        0      817 2024-05-24 06:08:48.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/report/empty_report.py
--rw-rw-rw-   0        0        0     8076 2024-05-24 06:38:14.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/report/report.py
-drwxrwxrwx   0        0        0        0 2024-05-30 06:25:54.020032 xurpas_data_quality-1.0.1/src/xurpas_data_quality/visuals/
--rw-rw-rw-   0        0        0      170 2024-05-27 01:58:12.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/visuals/__init__.py
--rw-rw-rw-   0        0        0     2833 2024-05-27 02:28:35.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/visuals/plots.py
-drwxrwxrwx   0        0        0        0 2024-05-30 06:25:54.020032 xurpas_data_quality-1.0.1/src/xurpas_data_quality.egg-info/
--rw-rw-rw-   0        0        0     2375 2024-05-30 06:25:53.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3696 2024-05-30 06:25:53.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 06:25:53.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-05-30 06:25:53.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-30 06:25:53.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 13:40:48.483196 xurpas_data_quality-1.0.2/
+-rw-rw-rw-   0        0        0      110 2024-05-07 06:47:23.000000 xurpas_data_quality-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2375 2024-05-30 13:40:48.481850 xurpas_data_quality-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1745 2024-05-30 03:36:27.000000 xurpas_data_quality-1.0.2/README.md
+-rw-rw-rw-   0        0        0      871 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 13:40:48.483196 xurpas_data_quality-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1166 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:40:48.358571 xurpas_data_quality-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 13:40:48.371535 xurpas_data_quality-1.0.2/src/xurpas_data_quality/
+-rw-rw-rw-   0        0        0       59 2024-05-30 13:35:12.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:40:48.410905 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/
+-rw-rw-rw-   0        0        0      306 2024-05-24 06:43:35.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:40:48.413930 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/alerts/
+-rw-rw-rw-   0        0        0        0 2024-05-03 07:10:29.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/alerts/__init__.py
+-rw-rw-rw-   0        0        0      953 2024-05-06 00:02:03.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/alerts/alerts.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:40:48.418139 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/algorithms/
+-rw-rw-rw-   0        0        0      105 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/algorithms/__init__.py
+-rw-rw-rw-   0        0        0      598 2024-05-24 06:08:48.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/algorithms/algorithms.py
+-rw-rw-rw-   0        0        0      344 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/algorithms/summary_algorithms.py
+-rw-rw-rw-   0        0        0      117 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/correlations.py
+-rw-rw-rw-   0        0        0     1370 2024-05-24 06:13:00.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/dataframe.py
+-rw-rw-rw-   0        0        0     6756 2024-05-24 06:45:08.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/describe.py
+-rw-rw-rw-   0        0        0     2836 2024-05-30 13:19:12.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/describe_new.py
+-rw-rw-rw-   0        0        0     2088 2024-05-30 08:58:06.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/describer.py
+-rw-rw-rw-   0        0        0      224 2024-05-06 01:15:30.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/descriptions.py
+-rw-rw-rw-   0        0        0      350 2024-04-26 07:12:37.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/pandas_dataframe.py
+-rw-rw-rw-   0        0        0     1240 2024-05-30 08:56:07.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/series_describe.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:40:48.426055 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/type_descriptions/
+-rw-rw-rw-   0        0        0      192 2024-05-30 06:14:41.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/type_descriptions/__init__.py
+-rw-rw-rw-   0        0        0     1681 2024-05-27 07:17:52.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/type_descriptions/describe_categorical.py
+-rw-rw-rw-   0        0        0      899 2024-05-30 06:23:13.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/type_descriptions/describe_date.py
+-rw-rw-rw-   0        0        0      989 2024-05-27 01:57:05.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/type_descriptions/describe_generic.py
+-rw-rw-rw-   0        0        0     3192 2024-05-30 06:22:46.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/type_descriptions/describe_numeric.py
+-rw-rw-rw-   0        0        0     1510 2024-05-30 13:34:40.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/typeset.py
+-rw-rw-rw-   0        0        0      570 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/utils.py
+-rw-rw-rw-   0        0        0     3322 2024-05-30 13:32:27.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/data_report.py
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:51:12.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-30 13:40:48.433462 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/
+-rw-rw-rw-   0        0        0        0 2024-05-07 05:20:40.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/__init__.py
+-rw-rw-rw-   0        0        0      801 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/handler.py
+-rw-rw-rw-   0        0        0     5699 2024-05-30 08:58:12.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/render.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:40:48.440564 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/render_types/
+-rw-rw-rw-   0        0        0      181 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/render_types/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:40:48.447089 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/render_types/bottom/
+-rw-rw-rw-   0        0        0        0 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/render_types/bottom/__init__.py
+-rw-rw-rw-   0        0        0     2095 2024-05-27 07:28:54.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/render_types/bottom/render_bottom_categorical.py
+-rw-rw-rw-   0        0        0      518 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/render_types/bottom/render_bottom_date.py
+-rw-rw-rw-   0        0        0     1618 2024-05-30 09:03:50.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/render_types/bottom/render_bottom_numerical.py
+-rw-rw-rw-   0        0        0     1158 2024-05-27 05:11:03.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/render_types/render_categorical.py
+-rw-rw-rw-   0        0        0     1148 2024-05-30 06:23:58.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/render_types/render_date.py
+-rw-rw-rw-   0        0        0      586 2024-05-27 00:26:47.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/render_types/render_generic.py
+-rw-rw-rw-   0        0        0     1757 2024-05-27 00:46:11.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/render_types/render_numerical.py
+-rw-rw-rw-   0        0        0     4608 2024-05-30 13:27:06.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/renderer.py
+-rw-rw-rw-   0        0        0      569 2024-05-14 04:40:10.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/template_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:40:48.460143 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:20:52.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:40:48.463143 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/assets/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:21:04.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/assets/__init__.py
+-rw-rw-rw-   0        0        0      594 2024-05-06 06:23:01.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/assets/script.js
+-rw-rw-rw-   0        0        0      684 2024-05-27 00:34:57.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/assets/style.css
+-rw-rw-rw-   0        0        0      249 2024-05-06 06:04:16.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/base.html
+-rw-rw-rw-   0        0        0      106 2024-05-01 16:04:49.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/collapse.html
+drwxrwxrwx   0        0        0        0 2024-05-30 13:40:48.472132 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/containers/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:21:13.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/containers/__init__.py
+-rw-rw-rw-   0        0        0      209 2024-04-30 07:01:56.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/containers/box.html
+-rw-rw-rw-   0        0        0       78 2024-05-03 02:13:15.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/containers/column.html
+-rw-rw-rw-   0        0        0      141 2024-05-03 02:44:57.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/containers/default.html
+-rw-rw-rw-   0        0        0      340 2024-05-01 12:08:46.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/containers/sections.html
+-rw-rw-rw-   0        0        0      835 2024-05-01 16:36:14.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/containers/tabs.html
+-rw-rw-rw-   0        0        0       72 2024-05-06 02:07:52.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/containers/test.html
+-rw-rw-rw-   0        0        0      277 2024-05-06 05:58:23.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/dropdown.html
+-rw-rw-rw-   0        0        0      268 2024-04-29 06:44:51.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/navigation.html
+-rw-rw-rw-   0        0        0      407 2024-05-27 02:32:44.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/plot.html
+-rw-rw-rw-   0        0        0      449 2024-05-06 06:03:50.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/script.html
+-rw-rw-rw-   0        0        0      267 2024-05-06 06:03:51.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/style.html
+-rw-rw-rw-   0        0        0      390 2024-05-06 00:49:14.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/table.html
+-rw-rw-rw-   0        0        0      300 2024-05-02 00:52:44.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/toggle.html
+-rw-rw-rw-   0        0        0      510 2024-05-27 00:51:20.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/variable.html
+drwxrwxrwx   0        0        0        0 2024-05-30 13:40:48.475925 xurpas_data_quality-1.0.2/src/xurpas_data_quality/report/
+-rw-rw-rw-   0        0        0       73 2024-05-24 06:08:48.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/report/__init__.py
+-rw-rw-rw-   0        0        0      817 2024-05-24 06:08:48.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/report/empty_report.py
+-rw-rw-rw-   0        0        0     8076 2024-05-24 06:38:14.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/report/report.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:40:48.478717 xurpas_data_quality-1.0.2/src/xurpas_data_quality/visuals/
+-rw-rw-rw-   0        0        0      170 2024-05-27 01:58:12.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/visuals/__init__.py
+-rw-rw-rw-   0        0        0     2833 2024-05-27 02:28:35.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality/visuals/plots.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:40:48.480729 xurpas_data_quality-1.0.2/src/xurpas_data_quality.egg-info/
+-rw-rw-rw-   0        0        0     2375 2024-05-30 13:40:48.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3696 2024-05-30 13:40:48.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 13:40:48.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-05-30 13:40:48.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-30 13:40:48.000000 xurpas_data_quality-1.0.2/src/xurpas_data_quality.egg-info/top_level.txt
```

### Comparing `xurpas_data_quality-1.0.1/PKG-INFO` & `xurpas_data_quality-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xurpas_data_quality
-Version: 1.0.1
+Version: 1.0.2
 Summary: XAIL Data quality
 Author: Neil Ortaliz
 Author-email: Neil Ortaliz <neil.ortaliz@xurpas.com>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `xurpas_data_quality-1.0.1/README.md` & `xurpas_data_quality-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/pyproject.toml` & `xurpas_data_quality-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/setup.py` & `xurpas_data_quality-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/alerts/alerts.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/algorithms/algorithms.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/algorithms/algorithms.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/dataframe.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/dataframe.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/describe.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/describe.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/describe_new.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/describe_new.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import warnings
 import pandas as pd
 
-from visions import Integer, Float
+from visions import Integer, Date, DateTime
 
 from xurpas_data_quality.data import get_series_descriptions, get_correlations
 from xurpas_data_quality.data.describer import TableDescription
 from xurpas_data_quality.data import XTypeSet
+from xurpas_data_quality.data.typeset import XFloat
 
 warnings.filterwarnings('ignore', category=UserWarning)
 
 def get_variable_type_counts(variable_types: dict)-> dict:
     value_counts = {}
     for _, value in variable_types.items():
-        if value ==Integer or value==Float:
+        if value ==Integer or value==XFloat:
             value = 'Numerical'
+        if value == Date or value == DateTime:
+            value = 'Date'
 
         if value in value_counts:
             value_counts[value] += 1
         else:
             value_counts[value] = 1
 
     return value_counts
```

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/describer.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/describer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pandas as pd
 
 from dataclasses import dataclass
-from visions import VisionsTypeset, Generic, Float, Integer, Categorical, Date, DateTime
+from visions import VisionsTypeset, Generic, Integer, Categorical, Date, DateTime
 from typing import Dict, List, Callable
 
 from xurpas_data_quality.data.type_descriptions import describe_numeric, describe_categorical, describe_generic, describe_date
+from xurpas_data_quality.data.typeset import XFloat
 
 @dataclass
 class TableDescription:
     df: pd.DataFrame
     dataset_statistics: Dict
     variable_types: Dict
     variables: Dict
@@ -18,15 +19,15 @@
     """Describer of series. Contains mapping per type"""
 
     def __init__(self, 
                 type_mapping: Dict[str, List[Callable]] = {
                      Generic : [
                          describe_generic,
                      ],
-                     Float : [
+                     XFloat : [
                          describe_generic,
                          describe_numeric
                      ],
                      Integer : [
                          describe_generic,
                          describe_numeric
                      ],
```

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/series_describe.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/series_describe.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 
 from typing import Tuple
 
 from xurpas_data_quality.data import Describer, XTypeSet
 
 def describe_series(col_name: str, series: pd.Series, data_types:dict=None)->Tuple[str, dict]:
     describer = Describer()
-
     if data_types is not None and col_name in data_types:
         series_type = data_types[col_name]
 
     else:
         series_type = XTypeSet.infer_type(series)
         series = XTypeSet.cast_to_inferred(series)
-
+    
     series_description = describer.summarize(dtype=series_type, series=series)
     series_description.update({'type': series_type})
 
     return col_name, series_description
 
 def get_series_descriptions(df: pd.DataFrame, data_types: dict=None)-> dict:
     """
```

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/type_descriptions/describe_categorical.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/type_descriptions/describe_categorical.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/type_descriptions/describe_date.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/type_descriptions/describe_date.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/type_descriptions/describe_generic.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/type_descriptions/describe_generic.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/type_descriptions/describe_numeric.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/type_descriptions/describe_numeric.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/utils.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/data/utils.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data_report.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/data_report.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pathlib import Path
 
 import pandas as pd
 
 from xurpas_data_quality.report import get_report, get_empty_report
 from xurpas_data_quality.data import check_dtypes, describe, load_dataframe,validate_dataframe ,check_col_names
 
+warnings.filterwarnings("ignore", category=UserWarning, module='visions')
 
 class DataReport:
     def __init__(self, file:str=None, 
                  df:pd.DataFrame=None, 
                  report_name:str="Data Report", 
                  file_path:str="report.html",
                  data_types:dict=None):
```

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/handler.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/handler.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/render.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 import pandas as pd
 
 from typing import Any
-from visions import Float, Integer, Categorical, Date
+from visions import Integer, Categorical, Date
 
+from xurpas_data_quality.data.typeset import XFloat
 from xurpas_data_quality.data.describer import TableDescription
 from xurpas_data_quality.render.renderer import HTMLBase, HTMLContainer, HTMLTable, HTMLVariable, HTMLPlot, HTMLToggle, HTMLCollapse, HTMLDropdown
 from xurpas_data_quality.visuals import plot_to_base64, create_tiny_histogram, create_histogram, create_distribution_plot, create_heatmap, create_interaction_plot
 from xurpas_data_quality.render.render_types import render_numerical, render_categorical, render_date, render_generic
 
+
 def render_variable(data: dict, column: str):
-    if data['type'] == Integer or data['type'] == Float:
+    if data['type'] == Integer or data['type'] == XFloat:
         return render_numerical(data, column)
     
     elif data['type'] == Categorical:
         return render_categorical(data, column)
     
     elif data['type'] == Date:
         return render_date(data, column)
     
     else:
         return render_generic(data, column)
     
 def render_variables_section(data: TableDescription):
     vars = []
     for key, value in data.variables.items():
-        vars.append(render_variable(value, key))
+        variable = render_variable(value, key)
+        vars.append(variable)
     #return [render_variable(value,key) for key, value in data.variables.items()]
     return vars
 
 def render_correlation_section(data: pd.DataFrame):
     return HTMLContainer(
         type="box",
         name="Correlation",
```

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/bottom/render_bottom_categorical.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/render_types/bottom/render_bottom_categorical.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/bottom/render_bottom_date.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/render_types/bottom/render_bottom_date.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/bottom/render_bottom_numerical.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/render_types/bottom/render_bottom_numerical.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from visions import Generic, Float, Integer
+from visions import Generic, Integer
 
+from xurpas_data_quality.data.typeset import XFloat
 from xurpas_data_quality.render.handler import Handler
 from xurpas_data_quality.render.renderer import HTMLBase, HTMLContainer, HTMLTable, HTMLVariable, HTMLPlot, HTMLToggle, HTMLCollapse, HTMLDropdown
 from xurpas_data_quality.visuals import plot_to_base64, create_tiny_histogram, create_histogram, create_distribution_plot, create_heatmap, create_interaction_plot
 
 
-@Handler.register(Float)
+@Handler.register(XFloat)
 @Handler.register(Integer)
 def render_bottom_numerical(data, col_name:str,*args, **kwargs):
     variable_bottom = [
         HTMLContainer(
             type="default",
             name="Statistics",
             id="stats",
```

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/render_categorical.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/render_types/render_categorical.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/render_date.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/render_types/render_date.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/render_generic.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/render_types/render_generic.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/render_numerical.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/render_types/render_numerical.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/renderer.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/renderer.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/template_loader.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/template_loader.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/assets/script.js` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/assets/script.js`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/assets/style.css` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/assets/style.css`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/containers/tabs.html` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/render/templates/containers/tabs.html`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/report/empty_report.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/report/empty_report.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/report/report.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/report/report.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality/visuals/plots.py` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality/visuals/plots.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality.egg-info/PKG-INFO` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xurpas_data_quality
-Version: 1.0.1
+Version: 1.0.2
 Summary: XAIL Data quality
 Author: Neil Ortaliz
 Author-email: Neil Ortaliz <neil.ortaliz@xurpas.com>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `xurpas_data_quality-1.0.1/src/xurpas_data_quality.egg-info/SOURCES.txt` & `xurpas_data_quality-1.0.2/src/xurpas_data_quality.egg-info/SOURCES.txt`

 * *Files identical despite different names*

