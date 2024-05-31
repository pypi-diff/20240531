# Comparing `tmp/spacr-0.0.21.tar.gz` & `tmp/spacr-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacr-0.0.21.tar", last modified: Wed May 29 17:33:56 2024, max compression
+gzip compressed data, was "spacr-0.0.35.tar", last modified: Fri May 31 17:21:47 2024, max compression
```

## Comparing `spacr-0.0.21.tar` & `spacr-0.0.35.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxrwxr-x   0 carruthers  (1000) carruthers  (1000)        0 2024-05-29 17:33:56.223083 spacr-0.0.21/
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1083 2024-03-18 14:14:52.000000 spacr-0.0.21/LICENSE
--rw-r--r--   0 carruthers  (1000) carruthers  (1000)     4943 2024-05-29 17:33:56.223083 spacr-0.0.21/PKG-INFO
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     3503 2024-04-19 22:18:02.000000 spacr-0.0.21/README.md
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)       38 2024-05-29 17:33:56.223083 spacr-0.0.21/setup.cfg
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1965 2024-05-29 17:30:50.000000 spacr-0.0.21/setup.py
-drwxrwxr-x   0 carruthers  (1000) carruthers  (1000)        0 2024-05-29 17:33:56.219083 spacr-0.0.21/spacr/
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      879 2024-03-18 14:14:52.000000 spacr-0.0.21/spacr/__init__.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      285 2024-03-18 14:14:52.000000 spacr-0.0.21/spacr/__main__.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    13776 2024-05-28 15:21:47.000000 spacr-0.0.21/spacr/alpha.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    19951 2024-04-29 20:22:59.000000 spacr-0.0.21/spacr/annotate_app.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1800 2024-03-27 18:50:03.000000 spacr-0.0.21/spacr/cli.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)   156457 2024-05-28 22:42:28.000000 spacr-0.0.21/spacr/core.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    33970 2024-04-29 20:23:08.000000 spacr-0.0.21/spacr/foldseek.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     3541 2024-04-29 20:23:07.000000 spacr-0.0.21/spacr/get_alfafold_structures.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    12568 2024-03-21 13:14:11.000000 spacr-0.0.21/spacr/graph_learning.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     3385 2024-03-21 13:14:20.000000 spacr-0.0.21/spacr/graph_learning_lap.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     7965 2024-03-18 17:12:55.000000 spacr-0.0.21/spacr/gui_classify_app.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     8752 2024-05-29 17:30:54.000000 spacr-0.0.21/spacr/gui_mask_app.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     8061 2024-03-21 13:14:27.000000 spacr-0.0.21/spacr/gui_measure_app.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)        0 2024-03-18 17:12:53.000000 spacr-0.0.21/spacr/gui_sim_app.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    30493 2024-05-29 14:11:59.000000 spacr-0.0.21/spacr/gui_utils.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)   108683 2024-05-28 22:42:29.000000 spacr-0.0.21/spacr/io.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      670 2024-03-18 14:14:52.000000 spacr-0.0.21/spacr/logger.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    39278 2024-03-22 19:23:09.000000 spacr-0.0.21/spacr/mask_app.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    54686 2024-05-28 15:21:46.000000 spacr-0.0.21/spacr/measure.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    11226 2024-03-21 13:14:15.000000 spacr-0.0.21/spacr/old_code.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    61655 2024-05-29 17:30:53.000000 spacr-0.0.21/spacr/plot.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    72997 2024-05-23 17:29:19.000000 spacr-0.0.21/spacr/sim.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    39661 2024-04-29 20:23:14.000000 spacr-0.0.21/spacr/timelapse.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    25904 2024-05-28 22:42:27.000000 spacr-0.0.21/spacr/train.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    29370 2024-05-07 16:13:08.000000 spacr-0.0.21/spacr/umap.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)   121205 2024-05-28 22:42:24.000000 spacr-0.0.21/spacr/utils.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      409 2024-03-18 14:14:52.000000 spacr-0.0.21/spacr/version.py
-drwxrwxr-x   0 carruthers  (1000) carruthers  (1000)        0 2024-05-29 17:33:56.223083 spacr-0.0.21/spacr.egg-info/
--rw-r--r--   0 carruthers  (1000) carruthers  (1000)     4943 2024-05-29 17:33:56.000000 spacr-0.0.21/spacr.egg-info/PKG-INFO
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1072 2024-05-29 17:33:56.000000 spacr-0.0.21/spacr.egg-info/SOURCES.txt
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)        1 2024-05-29 17:33:56.000000 spacr-0.0.21/spacr.egg-info/dependency_links.txt
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      290 2024-05-29 17:33:56.000000 spacr-0.0.21/spacr.egg-info/entry_points.txt
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      515 2024-05-29 17:33:56.000000 spacr-0.0.21/spacr.egg-info/requires.txt
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)        6 2024-05-29 17:33:56.000000 spacr-0.0.21/spacr.egg-info/top_level.txt
-drwxrwxr-x   0 carruthers  (1000) carruthers  (1000)        0 2024-05-29 17:33:56.223083 spacr-0.0.21/tests/
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     2289 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_annotate_app.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     2761 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_core.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      775 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_gui_classify_app.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      771 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_gui_mask_app.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      786 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_gui_measure_app.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      766 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_gui_sim_app.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     5555 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_gui_utils.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1786 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_io.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     2127 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_mask_app.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1957 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_measure.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     2075 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_plot.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1097 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_sim.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1644 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_timelapse.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1217 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_train.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1503 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_umap.py
--rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1307 2024-03-18 14:14:52.000000 spacr-0.0.21/tests/test_utils.py
+drwxrwxr-x   0 carruthers  (1000) carruthers  (1000)        0 2024-05-31 17:21:47.894943 spacr-0.0.35/
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1083 2024-03-18 14:14:52.000000 spacr-0.0.35/LICENSE
+-rw-r--r--   0 carruthers  (1000) carruthers  (1000)     4943 2024-05-31 17:21:47.890943 spacr-0.0.35/PKG-INFO
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     3503 2024-04-19 22:18:02.000000 spacr-0.0.35/README.md
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)       38 2024-05-31 17:21:47.894943 spacr-0.0.35/setup.cfg
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1976 2024-05-31 17:18:30.000000 spacr-0.0.35/setup.py
+drwxrwxr-x   0 carruthers  (1000) carruthers  (1000)        0 2024-05-31 17:21:47.886943 spacr-0.0.35/spacr/
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      879 2024-03-18 14:14:52.000000 spacr-0.0.35/spacr/__init__.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      285 2024-03-18 14:14:52.000000 spacr-0.0.35/spacr/__main__.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    13776 2024-05-28 15:21:47.000000 spacr-0.0.35/spacr/alpha.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    20031 2024-05-30 19:38:02.000000 spacr-0.0.35/spacr/annotate_app.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     2418 2024-05-29 22:03:14.000000 spacr-0.0.35/spacr/chris.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1800 2024-03-27 18:50:03.000000 spacr-0.0.35/spacr/cli.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)   156457 2024-05-28 22:42:28.000000 spacr-0.0.35/spacr/core.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    33970 2024-04-29 20:23:08.000000 spacr-0.0.35/spacr/foldseek.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     3541 2024-04-29 20:23:07.000000 spacr-0.0.35/spacr/get_alfafold_structures.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    12568 2024-03-21 13:14:11.000000 spacr-0.0.35/spacr/graph_learning.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     3385 2024-03-21 13:14:20.000000 spacr-0.0.35/spacr/graph_learning_lap.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     6430 2024-05-31 17:18:34.000000 spacr-0.0.35/spacr/gui.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     7917 2024-05-31 17:18:28.000000 spacr-0.0.35/spacr/gui_classify_app.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     9750 2024-05-31 17:18:32.000000 spacr-0.0.35/spacr/gui_mask_app.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     9675 2024-05-31 17:18:25.000000 spacr-0.0.35/spacr/gui_measure_app.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)        0 2024-05-31 13:58:19.000000 spacr-0.0.35/spacr/gui_sim_app.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    40715 2024-05-31 17:18:22.000000 spacr-0.0.35/spacr/gui_utils.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)   108688 2024-05-31 00:53:25.000000 spacr-0.0.35/spacr/io.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      670 2024-03-18 14:14:52.000000 spacr-0.0.35/spacr/logger.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    39376 2024-05-30 19:37:21.000000 spacr-0.0.35/spacr/mask_app.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    54686 2024-05-28 15:21:46.000000 spacr-0.0.35/spacr/measure.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    11226 2024-03-21 13:14:15.000000 spacr-0.0.35/spacr/old_code.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    61655 2024-05-29 17:30:53.000000 spacr-0.0.35/spacr/plot.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    72997 2024-05-23 17:29:19.000000 spacr-0.0.35/spacr/sim.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    39661 2024-04-29 20:23:14.000000 spacr-0.0.35/spacr/timelapse.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    25904 2024-05-28 22:42:27.000000 spacr-0.0.35/spacr/train.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)    29370 2024-05-07 16:13:08.000000 spacr-0.0.35/spacr/umap.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)   120918 2024-05-30 15:28:59.000000 spacr-0.0.35/spacr/utils.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      409 2024-05-30 15:28:57.000000 spacr-0.0.35/spacr/version.py
+drwxrwxr-x   0 carruthers  (1000) carruthers  (1000)        0 2024-05-31 17:21:47.890943 spacr-0.0.35/spacr.egg-info/
+-rw-r--r--   0 carruthers  (1000) carruthers  (1000)     4943 2024-05-31 17:21:47.000000 spacr-0.0.35/spacr.egg-info/PKG-INFO
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1100 2024-05-31 17:21:47.000000 spacr-0.0.35/spacr.egg-info/SOURCES.txt
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)        1 2024-05-31 17:21:47.000000 spacr-0.0.35/spacr.egg-info/dependency_links.txt
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      288 2024-05-31 17:21:47.000000 spacr-0.0.35/spacr.egg-info/entry_points.txt
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      515 2024-05-31 17:21:47.000000 spacr-0.0.35/spacr.egg-info/requires.txt
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)        6 2024-05-31 17:21:47.000000 spacr-0.0.35/spacr.egg-info/top_level.txt
+drwxrwxr-x   0 carruthers  (1000) carruthers  (1000)        0 2024-05-31 17:21:47.890943 spacr-0.0.35/tests/
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     2289 2024-03-18 14:14:52.000000 spacr-0.0.35/tests/test_annotate_app.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     2761 2024-03-18 14:14:52.000000 spacr-0.0.35/tests/test_core.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      775 2024-03-18 14:14:52.000000 spacr-0.0.35/tests/test_gui_classify_app.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      771 2024-03-18 14:14:52.000000 spacr-0.0.35/tests/test_gui_mask_app.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      786 2024-03-18 14:14:52.000000 spacr-0.0.35/tests/test_gui_measure_app.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)      766 2024-03-18 14:14:52.000000 spacr-0.0.35/tests/test_gui_sim_app.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     5555 2024-03-18 14:14:52.000000 spacr-0.0.35/tests/test_gui_utils.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1786 2024-03-18 14:14:52.000000 spacr-0.0.35/tests/test_io.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     2127 2024-03-18 14:14:52.000000 spacr-0.0.35/tests/test_mask_app.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1957 2024-03-18 14:14:52.000000 spacr-0.0.35/tests/test_measure.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     2075 2024-03-18 14:14:52.000000 spacr-0.0.35/tests/test_plot.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1097 2024-03-18 14:14:52.000000 spacr-0.0.35/tests/test_sim.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1644 2024-03-18 14:14:52.000000 spacr-0.0.35/tests/test_timelapse.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1217 2024-03-18 14:14:52.000000 spacr-0.0.35/tests/test_train.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1503 2024-03-18 14:14:52.000000 spacr-0.0.35/tests/test_umap.py
+-rw-rw-r--   0 carruthers  (1000) carruthers  (1000)     1307 2024-03-18 14:14:52.000000 spacr-0.0.35/tests/test_utils.py
```

### Comparing `spacr-0.0.21/LICENSE` & `spacr-0.0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/PKG-INFO` & `spacr-0.0.35/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacr
-Version: 0.0.21
+Version: 0.0.35
 Summary: Spatial phenotype analysis of crisp screens (SpaCr)
 Home-page: https://github.com/EinarOlafsson/spacr
 Author: Einar Birnir Olafsson
 Author-email: olafsson@med.umich.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacr Version: 0.0.21 Summary: Spatial phenotype
+Metadata-Version: 2.1 Name: spacr Version: 0.0.35 Summary: Spatial phenotype
 analysis of crisp screens (SpaCr) Home-page: https://github.com/EinarOlafsson/
 spacr Author: Einar Birnir Olafsson Author-email: olafsson@med.umich.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent License-
 File: LICENSE Requires-Dist: torch>=2.2.1 Requires-Dist: torchvision>=0.17.1
 Requires-Dist: torch-geometric>=2.5.1 Requires-Dist: numpy>=1.26.4 Requires-
 Dist: pandas>=2.2.1 Requires-Dist: statsmodels>=0.14.1 Requires-Dist: scikit-
```

### Comparing `spacr-0.0.21/README.md` & `spacr-0.0.35/README.md`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/setup.py` & `spacr-0.0.35/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,30 +31,31 @@
     'xgboost>=2.0.3',
     'PyWavelets>=1.6.0',
     'lxml>=5.1.0'
 ]
 
 setup(
     name="spacr",
-    version="0.0.21",
+    version="0.0.35",
     author="Einar Birnir Olafsson",
     author_email="olafsson@med.umich.com",
     description="Spatial phenotype analysis of crisp screens (SpaCr)",
     long_description=long_description,
     url="https://github.com/EinarOlafsson/spacr",
     packages=find_packages(exclude=["tests.*", "tests"]),
     install_requires=dependencies,
     entry_points={
         'console_scripts': [
-            'gui_mask=spacr.gui_mask_app:gui_mask',
-            'gui_measure=spacr.gui_measure_app:gui_measure',
-            'gui_make_masks=spacr.mask_app:gui_make_masks',
-            'gui_annotation=spacr.annotate_app:gui_annotation',
-            'gui_classify=spacr.gui_classify_app:gui_classify',
-            'gui_sim=spacr.gui_sim_app:gui_sim',
+            'mask=spacr.gui_mask_app:gui_mask',
+            'measure=spacr.gui_measure_app:gui_measure',
+            'make_masks=spacr.mask_app:gui_make_masks',
+            'annotate=spacr.annotate_app:gui_annotation',
+            'classify=spacr.gui_classify_app:gui_classify',
+            'sim=spacr.gui_sim_app:gui_sim',
+            'gui=spacr.gui:gui_app',
         ],
     },
     extras_require={
         'dev': ['pytest>=3.9'],
         'headless': ['opencv-python-headless'],
         'full': ['opencv-python'],
     },
```

### Comparing `spacr-0.0.21/spacr/__init__.py` & `spacr-0.0.35/spacr/__init__.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/spacr/alpha.py` & `spacr-0.0.35/spacr/alpha.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/spacr/annotate_app.py` & `spacr-0.0.35/spacr/annotate_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from IPython.display import display, HTML
 import tkinter as tk
 from tkinter import ttk
 from ttkthemes import ThemedTk
 
 from .logger import log_function_call
 
-from .gui_utils import ScrollableFrame, set_default_font, set_dark_style, create_dark_mode
+from .gui_utils import ScrollableFrame, set_default_font, set_dark_style, create_dark_mode, style_text_boxes, create_menu_bar
 
 class ImageApp:
     """
     A class representing an image application.
 
     Attributes:
     - root (tkinter.Tk): The root window of the application.
@@ -421,15 +421,16 @@
 
 @log_function_call
 def initiate_annotation_app_root(width, height):
     theme = 'breeze'
     root = ThemedTk(theme=theme)
     style = ttk.Style(root)
     set_dark_style(style)
-    set_default_font(root, font_name="Arial", size=10)
+    style_text_boxes(style)
+    set_default_font(root, font_name="Arial", size=8)
     root.geometry(f"{width}x{height}")
     root.title("Annotation App")
 
     container = tk.PanedWindow(root, orient=tk.HORIZONTAL)
     container.pack(fill=tk.BOTH, expand=True)
 
     scrollable_frame = ScrollableFrame(container, bg='#333333')
@@ -469,24 +470,25 @@
         # Destroy the initial settings window
         root.destroy()
         
         # Create a new root window for the application
         new_root = tk.Tk()
         new_root.geometry(f"{width}x{height}")
         new_root.title("Mask Application")
+        
 
         # Start the annotation application in the new root window
         app_instance = annotate(db, image_type, channels, annotation_column, geom, img_size, rows, columns)
         
         new_root.mainloop()
         
     create_dark_mode(root, style, console_output=None)
 
     run_button = ttk.Button(scrollable_frame.scrollable_frame, text="Run", command=run_app)
-    run_button.grid(row=row, column=0, columnspan=2, pady=10)
+    run_button.grid(row=row, column=0, columnspan=2, pady=10, padx=10)
 
     return root
 
 def gui_annotation():
     root = initiate_annotation_app_root(500, 350)
     root.mainloop()
```

### Comparing `spacr-0.0.21/spacr/cli.py` & `spacr-0.0.35/spacr/cli.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/spacr/core.py` & `spacr-0.0.35/spacr/core.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/spacr/foldseek.py` & `spacr-0.0.35/spacr/foldseek.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/spacr/get_alfafold_structures.py` & `spacr-0.0.35/spacr/get_alfafold_structures.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/spacr/graph_learning.py` & `spacr-0.0.35/spacr/graph_learning.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/spacr/graph_learning_lap.py` & `spacr-0.0.35/spacr/graph_learning_lap.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/spacr/gui_classify_app.py` & `spacr-0.0.35/spacr/gui_classify_app.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 try:
     ctypes.windll.shcore.SetProcessDpiAwareness(True)
 except AttributeError:
     pass
 
 from .logger import log_function_call
-from .gui_utils import ScrollableFrame, StdoutRedirector, create_dark_mode, set_dark_style, set_default_font, generate_fields, process_stdout_stderr, safe_literal_eval, clear_canvas, main_thread_update_function
-from .gui_utils import classify_variables, check_classify_gui_settings, train_test_model_wrapper, read_settings_from_csv, update_settings_from_csv  
+from .gui_utils import ScrollableFrame, StdoutRedirector, CustomButton, set_dark_style, set_default_font, generate_fields, process_stdout_stderr, clear_canvas, main_thread_update_function
+from .gui_utils import classify_variables, check_classify_gui_settings, train_test_model_wrapper, read_settings_from_csv, update_settings_from_csv, style_text_boxes, create_menu_bar
 
 thread_control = {"run_thread": None, "stop_requested": False}
 
 @log_function_call
 def initiate_abort():
     global thread_control
     if thread_control.get("stop_requested") is not None:
@@ -66,132 +66,123 @@
     csv_file_path = filedialog.askopenfilename(filetypes=[("CSV files", "*.csv")])
     csv_settings = read_settings_from_csv(csv_file_path)
     variables = classify_variables()
     new_settings = update_settings_from_csv(variables, csv_settings)
     vars_dict = generate_fields(new_settings, scrollable_frame)
 
 @log_function_call
-def initiate_classify_root(width, height):
-    global root, vars_dict, q, canvas, fig_queue, canvas_widget, thread_control
-        
-    theme = 'breeze'
+def initiate_classify_root(parent_frame, width, height):
+    global vars_dict, q, canvas, fig_queue, canvas_widget, thread_control
     
-    if theme in ['clam']:
-        root = tk.Tk()
-        style = ttk.Style(root)
-        style.theme_use(theme) #plastik, clearlooks, elegance, default was clam #alt, breeze, arc
-        set_dark_style(style)
-    elif theme in ['breeze']:
-        root = ThemedTk(theme="breeze")
-        style = ttk.Style(root)
-        set_dark_style(style)
-        
-    set_default_font(root, font_name="Arial", size=10)
-    #root.state('zoomed')  # For Windows to maximize the window
-    root.attributes('-fullscreen', True)
-    root.geometry(f"{width}x{height}")
-    root.title("SpaCer: generate masks")
+    style = ttk.Style(parent_frame)
+    set_dark_style(style)
+    style_text_boxes(style)
+    set_default_font(parent_frame, font_name="Open Sans", size=8)
+
+    parent_frame.configure(bg='#333333')
+    parent_frame.grid_rowconfigure(0, weight=1)
+    parent_frame.grid_columnconfigure(0, weight=1)
     fig_queue = Queue()
-            
+
     def _process_fig_queue():
         global canvas
         try:
             while not fig_queue.empty():
                 clear_canvas(canvas)
                 fig = fig_queue.get_nowait()
-                #set_fig_text_properties(fig, font_size=8)
                 for ax in fig.get_axes():
                     ax.set_xticks([])  # Remove x-axis ticks
                     ax.set_yticks([])  # Remove y-axis ticks
                     ax.xaxis.set_visible(False)  # Hide the x-axis
                     ax.yaxis.set_visible(False)  # Hide the y-axis
-                    #ax.title.set_fontsize(14) 
-                #disable_interactivity(fig)
                 fig.tight_layout()
                 fig.set_facecolor('#333333')
                 canvas.figure = fig
                 fig_width, fig_height = canvas_widget.winfo_width(), canvas_widget.winfo_height()
                 fig.set_size_inches(fig_width / fig.dpi, fig_height / fig.dpi, forward=True)
-                canvas.draw_idle() 
+                canvas.draw_idle()
         except Exception as e:
             traceback.print_exc()
-            #pass
         finally:
             canvas_widget.after(100, _process_fig_queue)
-            
-    # Process queue for console output
+
     def _process_console_queue():
         while not q.empty():
             message = q.get_nowait()
             console_output.insert(tk.END, message)
             console_output.see(tk.END)
         console_output.after(100, _process_console_queue)
-        
-    # Vertical container for settings and console
-    vertical_container = tk.PanedWindow(root, orient=tk.HORIZONTAL) #VERTICAL
-    vertical_container.pack(fill=tk.BOTH, expand=True)
-
-    # Scrollable Frame for user settings
-    scrollable_frame = ScrollableFrame(vertical_container, bg='#333333')
-    vertical_container.add(scrollable_frame, stretch="always")
+
+    vertical_container = tk.PanedWindow(parent_frame, orient=tk.HORIZONTAL)
+    vertical_container.grid(row=0, column=0, sticky=tk.NSEW)
+    parent_frame.grid_rowconfigure(0, weight=1)
+    parent_frame.grid_columnconfigure(0, weight=1)
+
+    # Settings Section
+    settings_frame = tk.Frame(vertical_container, bg='#333333')
+    vertical_container.add(settings_frame, stretch="always")
+    settings_label = ttk.Label(settings_frame, text="Settings", background="#333333", foreground="white")
+    settings_label.grid(row=0, column=0, pady=10, padx=10)
+    scrollable_frame = ScrollableFrame(settings_frame, width=500)
+    scrollable_frame.grid(row=1, column=0, sticky="nsew")
+    settings_frame.grid_rowconfigure(1, weight=1)
+    settings_frame.grid_columnconfigure(0, weight=1)
 
     # Setup for user input fields (variables)
     variables = classify_variables()
     vars_dict = generate_fields(variables, scrollable_frame)
-    
-    # Horizontal container for Matplotlib figure and the vertical pane (for settings and console)
-    horizontal_container = tk.PanedWindow(vertical_container, orient=tk.VERTICAL) #HORIZONTAL
-    vertical_container.add(horizontal_container, stretch="always")
 
-    # Matplotlib figure setup
+    # Button section
+    import_btn = CustomButton(scrollable_frame.scrollable_frame, text="Import Settings", command=lambda: import_settings(scrollable_frame))
+    import_btn.grid(row=47, column=0, pady=20, padx=20)
+    run_button = CustomButton(scrollable_frame.scrollable_frame, text="Run", command=lambda: start_process(q, fig_queue))
+    run_button.grid(row=45, column=0, pady=20, padx=20)
+    abort_button = CustomButton(scrollable_frame.scrollable_frame, text="Abort", command=initiate_abort)
+    abort_button.grid(row=45, column=1, pady=20, padx=20)
+    progress_label = ttk.Label(scrollable_frame.scrollable_frame, text="Processing: 0%", background="black", foreground="white") # Create progress field
+    progress_label.grid(row=50, column=0, columnspan=2, sticky="ew", pady=(5, 0), padx=10)
+
+    # Plot Canvas Section
+    plot_frame = tk.PanedWindow(vertical_container, orient=tk.VERTICAL)
+    vertical_container.add(plot_frame, stretch="always")
     figure = Figure(figsize=(30, 4), dpi=100, facecolor='#333333')
     plot = figure.add_subplot(111)
-    plot.plot([], [])  # This creates an empty plot.
+    plot.plot([], [])
     plot.axis('off')
-
-    # Embedding the Matplotlib figure in the Tkinter window
-    canvas = FigureCanvasTkAgg(figure, master=horizontal_container)
+    canvas = FigureCanvasTkAgg(figure, master=plot_frame)
     canvas.get_tk_widget().configure(cursor='arrow', background='#333333', highlightthickness=0)
-    #canvas.get_tk_widget().configure(cursor='arrow')
     canvas_widget = canvas.get_tk_widget()
-    horizontal_container.add(canvas_widget, stretch="always")
+    plot_frame.add(canvas_widget, stretch="always")
     canvas.draw()
     canvas.figure = figure
 
-    # Console output setup below the settings
-    console_output = scrolledtext.ScrolledText(vertical_container, height=10)
-    vertical_container.add(console_output, stretch="always")
+    # Console Section
+    console_frame = tk.Frame(vertical_container, bg='#333333')
+    vertical_container.add(console_frame, stretch="always")
+    console_label = ttk.Label(console_frame, text="Console", background="#333333", foreground="white")
+    console_label.grid(row=0, column=0, pady=10, padx=10)
+    console_output = scrolledtext.ScrolledText(console_frame, height=10, bg='#333333', fg='white', insertbackground='white')
+    console_output.grid(row=1, column=0, sticky="nsew")
+    console_frame.grid_rowconfigure(1, weight=1)
+    console_frame.grid_columnconfigure(0, weight=1)
 
-    # Queue and redirection setup for updating console output safely
     q = Queue()
     sys.stdout = StdoutRedirector(console_output)
     sys.stderr = StdoutRedirector(console_output)
-    
-    # This is your GUI setup where you create the Run button
-    run_button = ttk.Button(scrollable_frame.scrollable_frame, text="Run",command=lambda: start_process(q, fig_queue))
-    run_button.grid(row=40, column=0, pady=10)
-    
-    abort_button = ttk.Button(scrollable_frame.scrollable_frame, text="Abort", command=initiate_abort)
-    abort_button.grid(row=40, column=1, pady=10)
-    
-    progress_label = ttk.Label(scrollable_frame.scrollable_frame, text="Processing: 0%", background="#333333", foreground="white")
-    progress_label.grid(row=41, column=0, columnspan=2, sticky="ew", pady=(5, 0))
-    
-    # Create the Import Settings button
-    import_btn = tk.Button(root, text="Import Settings", command=lambda: import_settings(scrollable_frame))
-    import_btn.pack(pady=20)
-    
+
     _process_console_queue()
     _process_fig_queue()
-    create_dark_mode(root, style, console_output)
-    
-    root.after(100, lambda: main_thread_update_function(root, q, fig_queue, canvas_widget, progress_label))
-    
-    return root, vars_dict
+
+    parent_frame.after(100, lambda: main_thread_update_function(parent_frame, q, fig_queue, canvas_widget, progress_label))
+
+    return parent_frame, vars_dict
 
 def gui_classify():
-    global vars_dict, root
-    root, vars_dict = initiate_classify_root(1000, 1500)
+    root = tk.Tk()
+    root.geometry("1000x800")
+    root.title("SpaCer: generate masks")
+    initiate_classify_root(root, 1000, 800)
+    create_menu_bar(root)
     root.mainloop()
 
 if __name__ == "__main__":
-    gui_classify()
+    gui_classify()
```

### Comparing `spacr-0.0.21/spacr/gui_mask_app.py` & `spacr-0.0.35/spacr/gui_mask_app.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,219 +1,222 @@
 import sys, ctypes, matplotlib
 import tkinter as tk
 from tkinter import ttk, scrolledtext
 from ttkthemes import ThemedTk
 from matplotlib.figure import Figure
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
-from matplotlib.figure import Figure
 matplotlib.use('Agg')
 from tkinter import filedialog
 from multiprocessing import Process, Queue, Value
 import traceback
 
 try:
     ctypes.windll.shcore.SetProcessDpiAwareness(True)
 except AttributeError:
     pass
 
 from .logger import log_function_call
-from .gui_utils import ScrollableFrame, StdoutRedirector, clear_canvas, main_thread_update_function, create_dark_mode, set_dark_style, generate_fields, process_stdout_stderr, set_default_font, style_text_boxes
-from .gui_utils import mask_variables, check_mask_gui_settings, preprocess_generate_masks_wrapper, read_settings_from_csv, update_settings_from_csv#, toggle_advanced_settings
+from .gui_utils import ScrollableFrame, StdoutRedirector, ToggleSwitch, CustomButton
+from .gui_utils import clear_canvas, main_thread_update_function, set_dark_style, generate_fields, process_stdout_stderr, set_default_font, style_text_boxes
+from .gui_utils import mask_variables, check_mask_gui_settings, preprocess_generate_masks_wrapper, read_settings_from_csv, update_settings_from_csv, create_menu_bar
 
 thread_control = {"run_thread": None, "stop_requested": False}
 
+def toggle_test_mode():
+    global vars_dict
+    current_state = vars_dict['test_mode'][2].get()
+    new_state = not current_state
+    vars_dict['test_mode'][2].set(new_state)
+    if new_state:
+        test_mode_button.config(bg="blue")
+    else:
+        test_mode_button.config(bg="gray")
+
 def toggle_advanced_settings():
-    advanced = advanced_var.get()
-    for widget in advanced_widgets:
-        if advanced:
-            widget.grid()
+    global vars_dict
+
+    timelapse_settings = ['timelapse', 'timelapse_memory', 'timelapse_remove_transient', 'timelapse_mode', 'timelapse_objects', 'timelapse_displacement', 'timelapse_frame_limits', 'fps']
+    misc_settings = ['examples_to_plot', 'all_to_mip', 'pick_slice', 'skip_mode']
+    opperational_settings = ['preprocess', 'masks', 'randomize', 'batch_size', 'custom_regex', 'merge', 'normalize_plots', 'workers', 'plot', 'remove_background', 'lower_quantile']
+
+    advanced_settings = timelapse_settings+misc_settings+opperational_settings
+
+    # Toggle visibility of advanced settings
+    for setting in advanced_settings:
+        label, widget, var = vars_dict[setting]
+        if advanced_var.get() is False:
+            label.grid_remove()  # Hide the label
+            widget.grid_remove()  # Hide the widget
         else:
-            widget.grid_remove()
+            label.grid()  # Show the label
+            widget.grid()  # Show the widget
 
 @log_function_call
 def initiate_abort():
     global thread_control
     if thread_control.get("stop_requested") is not None:
         thread_control["stop_requested"].value = 1
 
     if thread_control.get("run_thread") is not None:
         thread_control["run_thread"].join(timeout=5)
         if thread_control["run_thread"].is_alive():
             thread_control["run_thread"].terminate()
         thread_control["run_thread"] = None
-        
+
 @log_function_call
 def run_mask_gui(q, fig_queue, stop_requested):
     global vars_dict
     process_stdout_stderr(q)
     try:
         settings = check_mask_gui_settings(vars_dict)
-        #settings = add_mask_gui_defaults(settings)
-        #for key in settings:
-        #    value = settings[key]
-        #    print(key, value, type(value))
         preprocess_generate_masks_wrapper(settings, q, fig_queue)
     except Exception as e:
         q.put(f"Error during processing: {e}")
         traceback.print_exc()
     finally:
         stop_requested.value = 1
-    
+
 @log_function_call
 def start_process(q, fig_queue):
     global thread_control
     if thread_control.get("run_thread") is not None:
         initiate_abort()
 
     stop_requested = Value('i', 0)  # multiprocessing shared value for inter-process communication
     thread_control["stop_requested"] = stop_requested
     thread_control["run_thread"] = Process(target=run_mask_gui, args=(q, fig_queue, stop_requested))
     thread_control["run_thread"].start()
-    
+
 def import_settings(scrollable_frame):
     global vars_dict
 
     csv_file_path = filedialog.askopenfilename(filetypes=[("CSV files", "*.csv")])
     csv_settings = read_settings_from_csv(csv_file_path)
     variables = mask_variables()
-    #variables = add_mask_gui_defaults(variables)
     new_settings = update_settings_from_csv(variables, csv_settings)
     vars_dict = generate_fields(new_settings, scrollable_frame)
-    
+
 @log_function_call
-def initiate_mask_root(width, height):
-    global root, vars_dict, q, canvas, fig_queue, canvas_widget, thread_control, advanced_widgets, advanced_var
-        
-    theme = 'breeze'
-    
-    if theme in ['clam']:
-        root = tk.Tk()
-        style = ttk.Style(root)
-        style.theme_use(theme) #plastik, clearlooks, elegance, default was clam #alt, breeze, arc
-        set_dark_style(style)
-    elif theme in ['breeze']:
-        root = ThemedTk(theme="breeze")
-        style = ttk.Style(root)
-        set_dark_style(style)
-        
+def initiate_mask_root(parent_frame, width, height):
+    global vars_dict, q, canvas, fig_queue, canvas_widget, thread_control, advanced_var, scrollable_frame
+
+    style = ttk.Style(parent_frame)
+    set_dark_style(style)
     style_text_boxes(style)
-    set_default_font(root, font_name="Arial", size=8)
-    #root.state('zoomed')  # For Windows to maximize the window
-    root.attributes('-fullscreen', True)
-    root.geometry(f"{width}x{height}")
-    root.title("SpaCer: generate masks")
+    set_default_font(parent_frame, font_name="Open Sans", size=8)
+    parent_frame.configure(bg='black')
+    parent_frame.grid_rowconfigure(0, weight=1)
+    parent_frame.grid_columnconfigure(0, weight=1)
+    
     fig_queue = Queue()
-            
+
     def _process_fig_queue():
         global canvas
         try:
             while not fig_queue.empty():
                 clear_canvas(canvas)
                 fig = fig_queue.get_nowait()
-                #set_fig_text_properties(fig, font_size=8)
                 for ax in fig.get_axes():
                     ax.set_xticks([])  # Remove x-axis ticks
                     ax.set_yticks([])  # Remove y-axis ticks
                     ax.xaxis.set_visible(False)  # Hide the x-axis
                     ax.yaxis.set_visible(False)  # Hide the y-axis
-                    #ax.title.set_fontsize(14) 
-                #disable_interactivity(fig)
                 fig.tight_layout()
-                fig.set_facecolor('#333333')
+                fig.set_facecolor('black')
                 canvas.figure = fig
                 fig_width, fig_height = canvas_widget.winfo_width(), canvas_widget.winfo_height()
                 fig.set_size_inches(fig_width / fig.dpi, fig_height / fig.dpi, forward=True)
-                canvas.draw_idle() 
+                canvas.draw_idle()
         except Exception as e:
             traceback.print_exc()
-            #pass
         finally:
             canvas_widget.after(100, _process_fig_queue)
-            
-    # Process queue for console output
+
     def _process_console_queue():
         while not q.empty():
             message = q.get_nowait()
             console_output.insert(tk.END, message)
             console_output.see(tk.END)
         console_output.after(100, _process_console_queue)
-        
-    # Vertical container for settings and console
-    vertical_container = tk.PanedWindow(root, orient=tk.HORIZONTAL) #VERTICAL
-    vertical_container.pack(fill=tk.BOTH, expand=True)
-
-    # Scrollable Frame for user settings
-    scrollable_frame = ScrollableFrame(vertical_container, bg='#333333')
-    vertical_container.add(scrollable_frame, stretch="always")
 
-    # Setup for user input fields (variables)
+    vertical_container = tk.PanedWindow(parent_frame, orient=tk.HORIZONTAL)
+    vertical_container.grid(row=0, column=0, sticky=tk.NSEW)
+    parent_frame.grid_rowconfigure(0, weight=1)
+    parent_frame.grid_columnconfigure(0, weight=1)
+
+    # Settings Section
+    settings_frame = tk.Frame(vertical_container, bg='black')
+    vertical_container.add(settings_frame, stretch="always")
+    settings_label = ttk.Label(settings_frame, text="Settings", style="Custom.TLabel")
+    settings_label.grid(row=0, column=0, pady=10, padx=10)
+    scrollable_frame = ScrollableFrame(settings_frame, width=600)
+    scrollable_frame.grid(row=1, column=0, sticky="nsew")
+    settings_frame.grid_rowconfigure(1, weight=1)
+    settings_frame.grid_columnconfigure(0, weight=1)
+    
+    # Create advanced settings checkbox
+    advanced_var = tk.BooleanVar(value=False)
+    advanced_Toggle = ToggleSwitch(scrollable_frame.scrollable_frame, text="Advanced Settings", variable=advanced_var, command=toggle_advanced_settings)
+    advanced_Toggle.grid(row=48, column=0, pady=10, padx=10)
     variables = mask_variables()
     vars_dict = generate_fields(variables, scrollable_frame)
-    #del vars_dict['fps']
-
-    # Debugging: print vars_dict to ensure it is populated correctly
-    #print("vars_dict:", vars_dict)
+    toggle_advanced_settings()
+    vars_dict['Test mode'] = (None, None, tk.BooleanVar(value=False))
     
-    # Horizontal container for Matplotlib figure and the vertical pane (for settings and console)
-    horizontal_container = tk.PanedWindow(vertical_container, orient=tk.VERTICAL) #HORIZONTAL
-    vertical_container.add(horizontal_container, stretch="always")
-
-    # Matplotlib figure setup
-    figure = Figure(figsize=(30, 4), dpi=100, facecolor='#333333')
+    # Button section
+    test_mode_button = CustomButton(scrollable_frame.scrollable_frame, text="Test Mode", command=toggle_test_mode)
+    test_mode_button.grid(row=47, column=1, pady=10, padx=10)
+    import_btn = CustomButton(scrollable_frame.scrollable_frame, text="Import Settings", command=lambda: import_settings(scrollable_frame))
+    import_btn.grid(row=47, column=0, pady=20, padx=20)
+    run_button = CustomButton(scrollable_frame.scrollable_frame, text="Run", command=lambda: start_process(q, fig_queue))
+    run_button.grid(row=45, column=0, pady=20, padx=20)
+    abort_button = CustomButton(scrollable_frame.scrollable_frame, text="Abort", command=initiate_abort)
+    abort_button.grid(row=45, column=1, pady=20, padx=20)
+    progress_label = ttk.Label(scrollable_frame.scrollable_frame, text="Processing: 0%", background="black", foreground="white") # Create progress field
+    progress_label.grid(row=50, column=0, columnspan=2, sticky="ew", pady=(5, 0), padx=10)
+
+    # Plot Canvas Section
+    plot_frame = tk.PanedWindow(vertical_container, orient=tk.VERTICAL) # Horizontal container for Matplotlib figure and the vertical pane (for settings and console)
+    vertical_container.add(plot_frame, stretch="always")
+    figure = Figure(figsize=(30, 4), dpi=100, facecolor='black') # Matplotlib figure setup
     plot = figure.add_subplot(111)
     plot.plot([], [])  # This creates an empty plot.
     plot.axis('off')
-
-    # Embedding the Matplotlib figure in the Tkinter window
-    canvas = FigureCanvasTkAgg(figure, master=horizontal_container)
-    canvas.get_tk_widget().configure(cursor='arrow', background='#333333', highlightthickness=0)
-    #canvas.get_tk_widget().configure(cursor='arrow')
+    canvas = FigureCanvasTkAgg(figure, master=plot_frame) # Embedd Matplotlib figure in Tkinter window
+    canvas.get_tk_widget().configure(cursor='arrow', background='black', highlightthickness=0)
     canvas_widget = canvas.get_tk_widget()
-    horizontal_container.add(canvas_widget, stretch="always")
+    plot_frame.add(canvas_widget, stretch="always")
     canvas.draw()
     canvas.figure = figure
 
-    # Console output setup below the settings
-    console_output = scrolledtext.ScrolledText(vertical_container, height=10)
-    vertical_container.add(console_output, stretch="always")
+    # Console Section
+    console_frame = tk.Frame(vertical_container, bg='black')
+    vertical_container.add(console_frame, stretch="always")
+    console_label = ttk.Label(console_frame, text="Console", background="black", foreground="white")
+    console_label.grid(row=0, column=0, pady=10, padx=10)
+    console_output = scrolledtext.ScrolledText(console_frame, height=10, bg='black', fg='white', insertbackground='white')
+    console_output.grid(row=1, column=0, sticky="nsew")
+    console_frame.grid_rowconfigure(1, weight=1)
+    console_frame.grid_columnconfigure(0, weight=1)
 
-    # Queue and redirection setup for updating console output safely
     q = Queue()
     sys.stdout = StdoutRedirector(console_output)
     sys.stderr = StdoutRedirector(console_output)
 
-    advanced_var = tk.BooleanVar()
-    advanced_checkbox = ttk.Checkbutton(scrollable_frame.scrollable_frame, text="Advanced Settings", variable=advanced_var, command=toggle_advanced_settings)
-    advanced_checkbox.grid(row=46, column=1, pady=10, padx=10)
-    
-    # This is your GUI setup where you create the Run button
-    run_button = ttk.Button(scrollable_frame.scrollable_frame, text="Run",command=lambda: start_process(q, fig_queue))
-    run_button.grid(row=45, column=0, pady=10, padx=10)
-    
-    abort_button = ttk.Button(scrollable_frame.scrollable_frame, text="Abort", command=initiate_abort)
-    abort_button.grid(row=45, column=1, pady=10, padx=10)
-    
-    progress_label = ttk.Label(scrollable_frame.scrollable_frame, text="Processing: 0%", background="#333333", foreground="white")
-    progress_label.grid(row=41, column=0, columnspan=2, sticky="ew", pady=(5, 0), padx=10)
-
-    # Create the Import Settings button
-    import_btn = tk.Button(root, text="Import Settings", command=lambda: import_settings(scrollable_frame))
-    import_btn.pack(pady=20, padx=10)
-
-    
-
     _process_console_queue()
     _process_fig_queue()
-    create_dark_mode(root, style, console_output)
-    
-    root.after(100, lambda: main_thread_update_function(root, q, fig_queue, canvas_widget, progress_label))
     
-    return root, vars_dict
+    parent_frame.after(100, lambda: main_thread_update_function(parent_frame, q, fig_queue, canvas_widget, progress_label))
+
+    return parent_frame, vars_dict
 
 def gui_mask():
-    global vars_dict, root
-    root, vars_dict = initiate_mask_root(1000, 1500)
-    
+    root = tk.Tk()
+    root.geometry("1000x800")
+    root.title("SpaCer: generate masks")
+    initiate_mask_root(root, 1000, 800)
+    create_menu_bar(root)
     root.mainloop()
-    
+
 if __name__ == "__main__":
-    gui_mask()
+    gui_mask()
+
```

### Comparing `spacr-0.0.21/spacr/gui_measure_app.py` & `spacr-0.0.35/spacr/gui_measure_app.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,66 @@
-import sys, traceback, matplotlib, ctypes, csv
+import sys, traceback, matplotlib, ctypes
 import tkinter as tk
 from tkinter import ttk, scrolledtext
 from matplotlib.figure import Figure
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 import matplotlib.pyplot as plt
 matplotlib.use('Agg')  # Use the non-GUI Agg backend
 from multiprocessing import Process, Queue, Value
 from ttkthemes import ThemedTk
-from tkinter import filedialog, StringVar, BooleanVar, IntVar, DoubleVar, Tk
+from tkinter import filedialog
 
 try:
     ctypes.windll.shcore.SetProcessDpiAwareness(True)
 except AttributeError:
     pass
 
 from .logger import log_function_call
-from .gui_utils import ScrollableFrame, StdoutRedirector, process_stdout_stderr, set_dark_style, set_default_font, generate_fields, create_dark_mode, main_thread_update_function
-from .gui_utils import measure_variables, measure_crop_wrapper, clear_canvas, safe_literal_eval, check_measure_gui_settings, read_settings_from_csv, update_settings_from_csv
+from .gui_utils import ScrollableFrame, StdoutRedirector, CustomButton, ToggleSwitch
+from .gui_utils import process_stdout_stderr, set_dark_style, set_default_font, generate_fields, main_thread_update_function, create_menu_bar
+from .gui_utils import measure_variables, measure_crop_wrapper, clear_canvas, check_measure_gui_settings, read_settings_from_csv, update_settings_from_csv, style_text_boxes
 
 thread_control = {"run_thread": None, "stop_requested": False}
 
+def toggle_test_mode():
+    global vars_dict
+    current_state = vars_dict['test_mode'][2].get()
+    new_state = not current_state
+    vars_dict['test_mode'][2].set(new_state)
+    if new_state:
+        test_mode_button.config(bg="blue")
+    else:
+        test_mode_button.config(bg="gray")
+
+def toggle_advanced_settings():
+    global vars_dict
+
+    timelapse_settings = ['timelapse', 'timelapse_objects']
+    misc_settings = ['representative_images', 'plot', 'plot_filtration', 'include_uninfected', 'dialate_pngs', 'dialate_png_ratios']
+    opperational_settings = ['max_workers','experiment','cells','cell_loc','pathogens','pathogen_loc','treatments','treatment_loc','channel_of_interest','compartments','measurement','nr_imgs', 'um_per_pixel']
+    
+    advanced_settings = timelapse_settings+misc_settings+opperational_settings
+
+    # Toggle visibility of advanced settings
+    for setting in advanced_settings:
+        label, widget, var = vars_dict[setting]
+        if advanced_var.get() is False:
+            label.grid_remove()  # Hide the label
+            widget.grid_remove()  # Hide the widget
+        else:
+            label.grid()  # Show the label
+            widget.grid()  # Show the widget
+
 @log_function_call
 def run_measure_gui(q, fig_queue, stop_requested):
     global vars_dict
     process_stdout_stderr(q)
     try:
         print('hello')
         settings = check_measure_gui_settings(vars_dict)
-        #for key in settings:
-        #    value = settings[key]
-        #    print(key, value, type(value))
         measure_crop_wrapper(settings=settings, q=q, fig_queue=fig_queue)
     except Exception as e:
         q.put(f"Error during processing: {e}")
         traceback.print_exc()
     finally:
         stop_requested.value = 1
 
@@ -67,134 +94,130 @@
     csv_file_path = filedialog.askopenfilename(filetypes=[("CSV files", "*.csv")])
     csv_settings = read_settings_from_csv(csv_file_path)
     variables = measure_variables()
     new_settings = update_settings_from_csv(variables, csv_settings)
     vars_dict = generate_fields(new_settings, scrollable_frame)
 
 @log_function_call
-def initiate_measure_root(width, height):
-    global root, vars_dict, q, canvas, fig_queue, canvas_widget, thread_control, variables
-    
-    theme = 'breeze'
+def initiate_measure_root(parent_frame, width, height):
+    global vars_dict, q, canvas, fig_queue, canvas_widget, thread_control, variables, advanced_var, scrollable_frame
     
-    if theme in ['clam']:
-        root = tk.Tk()
-        style = ttk.Style(root)
-        style.theme_use(theme) #plastik, clearlooks, elegance, default was clam #alt, breeze, arc
-        set_dark_style(style)
-
-    elif theme in ['breeze']:
-        root = ThemedTk(theme="breeze")
-        style = ttk.Style(root)
-        set_dark_style(style)
-    
-    set_default_font(root, font_name="Arial", size=10)
-    #root.state('zoomed')  # For Windows to maximize the window
-    root.attributes('-fullscreen', True)
-    root.geometry(f"{width}x{height}")
-    root.configure(bg='#333333')
-    root.title("SpaCer: generate masks")
+    style = ttk.Style(parent_frame)
+    set_dark_style(style)
+    style_text_boxes(style)
+    set_default_font(parent_frame, font_name="Open Sans", size=8)
+
+    parent_frame.configure(bg='black')
+    parent_frame.grid_rowconfigure(0, weight=1)
+    parent_frame.grid_columnconfigure(0, weight=1)
     fig_queue = Queue()
     
     def _process_fig_queue():
         global canvas
         try:
             while not fig_queue.empty():
                 clear_canvas(canvas)
                 fig = fig_queue.get_nowait()
-                #set_fig_text_properties(fig, font_size=8)
                 for ax in fig.get_axes():
                     ax.set_xticks([])  # Remove x-axis ticks
                     ax.set_yticks([])  # Remove y-axis ticks
                     ax.xaxis.set_visible(False)  # Hide the x-axis
                     ax.yaxis.set_visible(False)  # Hide the y-axis
-                    #ax.title.set_fontsize(14) 
-                #disable_interactivity(fig)
                 fig.tight_layout()
-                fig.set_facecolor('#333333')
+                fig.set_facecolor('black')
                 canvas.figure = fig
                 fig_width, fig_height = canvas_widget.winfo_width(), canvas_widget.winfo_height()
                 fig.set_size_inches(fig_width / fig.dpi, fig_height / fig.dpi, forward=True)
-                canvas.draw_idle() 
+                canvas.draw_idle()
         except Exception as e:
             traceback.print_exc()
-            #pass
         finally:
             canvas_widget.after(100, _process_fig_queue)
-            
-    # Process queue for console output
+
     def _process_console_queue():
         while not q.empty():
             message = q.get_nowait()
             console_output.insert(tk.END, message)
             console_output.see(tk.END)
         console_output.after(100, _process_console_queue)
 
-    # Vertical container for settings and console
-    vertical_container = tk.PanedWindow(root, orient=tk.HORIZONTAL) #VERTICAL
-    vertical_container.pack(fill=tk.BOTH, expand=True)
-
-    # Scrollable Frame for user settings
-    scrollable_frame = ScrollableFrame(vertical_container)
-    vertical_container.add(scrollable_frame, stretch="always")
-
-    # Setup for user input fields (variables)
+    vertical_container = tk.PanedWindow(parent_frame, orient=tk.HORIZONTAL)
+    vertical_container.grid(row=0, column=0, sticky=tk.NSEW)
+    parent_frame.grid_rowconfigure(0, weight=1)
+    parent_frame.grid_columnconfigure(0, weight=1)
+
+    # Settings Section
+    settings_frame = tk.Frame(vertical_container, bg='black')
+    vertical_container.add(settings_frame, stretch="always")
+    settings_label = ttk.Label(settings_frame, text="Settings", background="black", foreground="white")
+    settings_label.grid(row=0, column=0, pady=10, padx=10)
+    scrollable_frame = ScrollableFrame(settings_frame, width=500)
+    scrollable_frame.grid(row=1, column=0, sticky="nsew")
+    settings_frame.grid_rowconfigure(1, weight=1)
+    settings_frame.grid_columnconfigure(0, weight=1)
+    
+    # Create advanced settings checkbox
+    advanced_var = tk.BooleanVar(value=False)
+    advanced_Toggle = ToggleSwitch(scrollable_frame.scrollable_frame, text="Advanced Settings", variable=advanced_var, command=toggle_advanced_settings)
+    advanced_Toggle.grid(row=48, column=0, pady=10, padx=10)
     variables = measure_variables()
     vars_dict = generate_fields(variables, scrollable_frame)
+    toggle_advanced_settings()
+    vars_dict['Test mode'] = (None, None, tk.BooleanVar(value=False))
     
-    # Horizontal container for Matplotlib figure and the vertical pane (for settings and console)
-    horizontal_container = tk.PanedWindow(vertical_container, orient=tk.VERTICAL) #HORIZONTAL
-    vertical_container.add(horizontal_container, stretch="always")
-
-    # Matplotlib figure setup
-    figure = Figure(figsize=(30, 4), dpi=100, facecolor='#333333')
+    # Button section
+    test_mode_button = CustomButton(scrollable_frame.scrollable_frame, text="Test Mode", command=toggle_test_mode)
+    test_mode_button.grid(row=47, column=1, pady=10, padx=10)
+    import_btn = CustomButton(scrollable_frame.scrollable_frame, text="Import Settings", command=lambda: import_settings(scrollable_frame))
+    import_btn.grid(row=47, column=0, pady=20, padx=20)
+    run_button = CustomButton(scrollable_frame.scrollable_frame, text="Run", command=lambda: start_process(q, fig_queue))
+    run_button.grid(row=45, column=0, pady=20, padx=20)
+    abort_button = CustomButton(scrollable_frame.scrollable_frame, text="Abort", command=initiate_abort)
+    abort_button.grid(row=45, column=1, pady=20, padx=20)
+    progress_label = ttk.Label(scrollable_frame.scrollable_frame, text="Processing: 0%", background="black", foreground="white") # Create progress field
+    progress_label.grid(row=50, column=0, columnspan=2, sticky="ew", pady=(5, 0), padx=10)
+
+    # Plot Canvas Section
+    plot_frame = tk.PanedWindow(vertical_container, orient=tk.VERTICAL)
+    vertical_container.add(plot_frame, stretch="always")
+    figure = Figure(figsize=(30, 4), dpi=100, facecolor='black')
     plot = figure.add_subplot(111)
-    plot.plot([], [])  # This creates an empty plot.
+    plot.plot([], [])
     plot.axis('off')
-
-    # Embedding the Matplotlib figure in the Tkinter window
-    canvas = FigureCanvasTkAgg(figure, master=horizontal_container)
-    canvas.get_tk_widget().configure(cursor='arrow', background='#333333', highlightthickness=0)
-    #canvas.get_tk_widget().configure(cursor='arrow')
+    canvas = FigureCanvasTkAgg(figure, master=plot_frame)
+    canvas.get_tk_widget().configure(cursor='arrow', background='black', highlightthickness=0)
     canvas_widget = canvas.get_tk_widget()
-    horizontal_container.add(canvas_widget, stretch="always")
+    plot_frame.add(canvas_widget, stretch="always")
     canvas.draw()
     canvas.figure = figure
 
-    # Console output setup below the settings
-    console_output = scrolledtext.ScrolledText(vertical_container, height=10)
-    vertical_container.add(console_output, stretch="always")
+    # Console Section
+    console_frame = tk.Frame(vertical_container, bg='black')
+    vertical_container.add(console_frame, stretch="always")
+    console_label = ttk.Label(console_frame, text="Console", background="black", foreground="white")
+    console_label.grid(row=0, column=0, pady=10, padx=10)
+    console_output = scrolledtext.ScrolledText(console_frame, height=10, bg='black', fg='white', insertbackground='white')
+    console_output.grid(row=1, column=0, sticky="nsew")
+    console_frame.grid_rowconfigure(1, weight=1)
+    console_frame.grid_columnconfigure(0, weight=1)
 
-    # Queue and redirection setup for updating console output safely
     q = Queue()
     sys.stdout = StdoutRedirector(console_output)
     sys.stderr = StdoutRedirector(console_output)
     
-    # This is your GUI setup where you create the Run button
-    run_button = ttk.Button(scrollable_frame.scrollable_frame, text="Run",command=lambda: start_process(q, fig_queue))
-    run_button.grid(row=40, column=0, pady=10)
-    
-    abort_button = ttk.Button(scrollable_frame.scrollable_frame, text="Abort", command=initiate_abort)
-    abort_button.grid(row=40, column=1, pady=10)
-    
-    progress_label = ttk.Label(scrollable_frame.scrollable_frame, text="Progress: ", background="#333333", foreground="white")
-    progress_label.grid(row=41, column=0, columnspan=2, sticky="ew", pady=(5, 0))
-    
-    # Create the Import Settings button
-    import_btn = tk.Button(root, text="Import Settings", command=lambda: import_settings(scrollable_frame))
-    import_btn.pack(pady=20)
-    
     _process_console_queue()
     _process_fig_queue()
-    create_dark_mode(root, style, console_output)
     
-    #root.after(100, lambda: main_thread_update_function(root, q, fig_queue, canvas_widget, progress_label))
+    parent_frame.after(100, lambda: main_thread_update_function(parent_frame, q, fig_queue, canvas_widget, progress_label))
     
-    return root, vars_dict
+    return parent_frame, vars_dict
 
 def gui_measure():
-    global vars_dict, root
-    root, vars_dict = initiate_measure_root(1000, 1500)
+    root = tk.Tk()
+    root.geometry("1000x800")
+    root.title("SpaCer: generate masks")
+    initiate_measure_root(root, 1000, 800)
+    create_menu_bar(root)
     root.mainloop()
 
 if __name__ == "__main__":
     gui_measure()
```

### Comparing `spacr-0.0.21/spacr/io.py` & `spacr-0.0.35/spacr/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -1296,14 +1296,15 @@
     src = settings['src']
     valid_ext = ['tif', 'tiff', 'png', 'jpeg']
     files = os.listdir(src)
     extensions = [file.split('.')[-1] for file in files]
     extension_counts = Counter(extensions)
     most_common_extension = extension_counts.most_common(1)[0][0]
     img_format = None
+    
 
     delete_empty_subdirectories(src)
 
     # Check if the most common extension is one of the specified image formats
     if most_common_extension in valid_ext:
         img_format = f'.{most_common_extension}'
         print(f'Found {extension_counts[most_common_extension]} {most_common_extension} files')
```

### Comparing `spacr-0.0.21/spacr/logger.py` & `spacr-0.0.35/spacr/logger.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/spacr/mask_app.py` & `spacr-0.0.35/spacr/mask_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from scipy.ndimage import binary_fill_holes, label
 import tkinter as tk
 from tkinter import ttk
 from ttkthemes import ThemedTk
 
 from .logger import log_function_call
 
-from .gui_utils import ScrollableFrame, set_dark_style, set_default_font, create_dark_mode
+from .gui_utils import ScrollableFrame, set_dark_style, set_default_font, create_dark_mode, style_text_boxes, create_menu_bar
 
 class modify_masks:
 
     def __init__(self, root, folder_path, scale_factor, width, height):
         self.root = root
         self.folder_path = folder_path
         self.scale_factor = scale_factor
@@ -755,17 +755,20 @@
 
 @log_function_call
 def initiate_mask_app_root(width, height):
     theme = 'breeze'
     root = ThemedTk(theme=theme)
     style = ttk.Style(root)
     set_dark_style(style)
-    set_default_font(root, font_name="Arial", size=10)
+
+    style_text_boxes(style)
+    set_default_font(root, font_name="Arial", size=8)
     root.geometry(f"{width}x{height}")
     root.title("Mask App")
+    create_menu_bar(root)
 
     container = tk.PanedWindow(root, orient=tk.HORIZONTAL)
     container.pack(fill=tk.BOTH, expand=True)
 
     scrollable_frame = ScrollableFrame(container, bg='#333333')
     container.add(scrollable_frame, stretch="always")
 
@@ -802,15 +805,15 @@
         # Start the modify_masks application in the new root window
         app_instance = modify_masks(new_root, folder_path, scale_factor, width, height)
         new_root.mainloop()
         
     create_dark_mode(root, style, console_output=None)
 
     run_button = ttk.Button(scrollable_frame.scrollable_frame, text="Run", command=run_app)
-    run_button.grid(row=row, column=0, columnspan=2, pady=10)
+    run_button.grid(row=row, column=0, columnspan=2, pady=10, padx=10)
 
     return root
 
 def gui_make_masks():
     root = initiate_mask_app_root(400, 200)
     root.mainloop()
```

### Comparing `spacr-0.0.21/spacr/measure.py` & `spacr-0.0.35/spacr/measure.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/spacr/old_code.py` & `spacr-0.0.35/spacr/old_code.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/spacr/plot.py` & `spacr-0.0.35/spacr/plot.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/spacr/sim.py` & `spacr-0.0.35/spacr/sim.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/spacr/timelapse.py` & `spacr-0.0.35/spacr/timelapse.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/spacr/train.py` & `spacr-0.0.35/spacr/train.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/spacr/umap.py` & `spacr-0.0.35/spacr/umap.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/spacr/utils.py` & `spacr-0.0.35/spacr/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,20 +42,14 @@
 from sklearn.linear_model import Lasso, Ridge
 from sklearn.preprocessing import OneHotEncoder
 from sklearn.cluster import KMeans
 from torchvision.models.resnet import ResNet18_Weights, ResNet34_Weights, ResNet50_Weights, ResNet101_Weights, ResNet152_Weights
 
 from .logger import log_function_call
 
-#from .io import _read_and_join_tables, _save_figure
-#from .timelapse import _btrack_track_cells, _trackpy_track_cells
-#from .plot import _plot_images_on_grid, plot_masks, _plot_histograms_and_stats, plot_resize, _plot_plates, _reg_v_plot, plot_masks
-#from .core import identify_masks
-
-
 def _gen_rgb_image(image, cahnnels):
     rgb_image = np.take(image, cahnnels, axis=-1)
     rgb_image = rgb_image.astype(float)
     rgb_image -= rgb_image.min()
     rgb_image /= rgb_image.max()
     return rgb_image
```

### Comparing `spacr-0.0.21/spacr.egg-info/PKG-INFO` & `spacr-0.0.35/spacr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacr
-Version: 0.0.21
+Version: 0.0.35
 Summary: Spatial phenotype analysis of crisp screens (SpaCr)
 Home-page: https://github.com/EinarOlafsson/spacr
 Author: Einar Birnir Olafsson
 Author-email: olafsson@med.umich.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacr Version: 0.0.21 Summary: Spatial phenotype
+Metadata-Version: 2.1 Name: spacr Version: 0.0.35 Summary: Spatial phenotype
 analysis of crisp screens (SpaCr) Home-page: https://github.com/EinarOlafsson/
 spacr Author: Einar Birnir Olafsson Author-email: olafsson@med.umich.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent License-
 File: LICENSE Requires-Dist: torch>=2.2.1 Requires-Dist: torchvision>=0.17.1
 Requires-Dist: torch-geometric>=2.5.1 Requires-Dist: numpy>=1.26.4 Requires-
 Dist: pandas>=2.2.1 Requires-Dist: statsmodels>=0.14.1 Requires-Dist: scikit-
```

### Comparing `spacr-0.0.21/spacr.egg-info/SOURCES.txt` & `spacr-0.0.35/spacr.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 LICENSE
 README.md
 setup.py
 spacr/__init__.py
 spacr/__main__.py
 spacr/alpha.py
 spacr/annotate_app.py
+spacr/chris.py
 spacr/cli.py
 spacr/core.py
 spacr/foldseek.py
 spacr/get_alfafold_structures.py
 spacr/graph_learning.py
 spacr/graph_learning_lap.py
+spacr/gui.py
 spacr/gui_classify_app.py
 spacr/gui_mask_app.py
 spacr/gui_measure_app.py
 spacr/gui_sim_app.py
 spacr/gui_utils.py
 spacr/io.py
 spacr/logger.py
```

### Comparing `spacr-0.0.21/spacr.egg-info/requires.txt` & `spacr-0.0.35/spacr.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/tests/test_annotate_app.py` & `spacr-0.0.35/tests/test_annotate_app.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/tests/test_core.py` & `spacr-0.0.35/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/tests/test_gui_classify_app.py` & `spacr-0.0.35/tests/test_gui_classify_app.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/tests/test_gui_mask_app.py` & `spacr-0.0.35/tests/test_gui_mask_app.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/tests/test_gui_measure_app.py` & `spacr-0.0.35/tests/test_gui_measure_app.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/tests/test_gui_sim_app.py` & `spacr-0.0.35/tests/test_gui_sim_app.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/tests/test_gui_utils.py` & `spacr-0.0.35/tests/test_gui_utils.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/tests/test_io.py` & `spacr-0.0.35/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/tests/test_mask_app.py` & `spacr-0.0.35/tests/test_mask_app.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/tests/test_measure.py` & `spacr-0.0.35/tests/test_measure.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/tests/test_plot.py` & `spacr-0.0.35/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/tests/test_sim.py` & `spacr-0.0.35/tests/test_sim.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/tests/test_timelapse.py` & `spacr-0.0.35/tests/test_timelapse.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/tests/test_train.py` & `spacr-0.0.35/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/tests/test_umap.py` & `spacr-0.0.35/tests/test_umap.py`

 * *Files identical despite different names*

### Comparing `spacr-0.0.21/tests/test_utils.py` & `spacr-0.0.35/tests/test_utils.py`

 * *Files identical despite different names*

