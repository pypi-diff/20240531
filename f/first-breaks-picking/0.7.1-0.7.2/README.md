# Comparing `tmp/first_breaks_picking-0.7.1.tar.gz` & `tmp/first_breaks_picking-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\a\first_breaks_picking\first_breaks_picking\dist\.tmp-73x7kkyf\first_breaks_picking-0.7.1.tar", last modified: Sun May 26 20:44:33 2024, max compression
+gzip compressed data, was "D:\a\first_breaks_picking\first_breaks_picking\dist\.tmp-en_eky3n\first_breaks_picking-0.7.2.tar", last modified: Fri May 31 07:13:13 2024, max compression
```

## Comparing `first_breaks_picking-0.7.1.tar` & `first_breaks_picking-0.7.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 20:44:33.732417 first_breaks_picking-0.7.1/
--rw-rw-rw-   0        0        0    11558 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/LICENSE
--rw-rw-rw-   0        0        0       98 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/MANIFEST.in
--rw-rw-rw-   0        0        0    40249 2024-05-26 20:44:33.732417 first_breaks_picking-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0    25526 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 20:44:33.701166 first_breaks_picking-0.7.1/first_breaks/
--rw-rw-rw-   0        0        0        5 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/VERSION
--rw-rw-rw-   0        0        0     1176 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/__init__.py
--rw-rw-rw-   0        0        0       96 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/__main__.py
--rw-rw-rw-   0        0        0      369 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/cli.py
--rw-rw-rw-   0        0        0     1144 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/const.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:44:33.716790 first_breaks_picking-0.7.1/first_breaks/data_models/
--rw-rw-rw-   0        0        0        0 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/data_models/__init__.py
--rw-rw-rw-   0        0        0     2695 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/data_models/dependent.py
--rw-rw-rw-   0        0        0     4736 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/data_models/independent.py
--rw-rw-rw-   0        0        0      696 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/data_models/initialised_defaults.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:44:33.716790 first_breaks_picking-0.7.1/first_breaks/desktop/
--rw-rw-rw-   0        0        0        0 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/desktop/__init__.py
--rw-rw-rw-   0        0        0     4586 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/desktop/bandfilter_widget.py
--rw-rw-rw-   0        0        0     5816 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/desktop/byte_encode_unit_widget.py
--rw-rw-rw-   0        0        0     1969 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/desktop/combobox_with_mapping.py
--rw-rw-rw-   0        0        0    10802 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/desktop/export_widgets.py
--rw-rw-rw-   0        0        0    22914 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/desktop/graph.py
--rw-rw-rw-   0        0        0      776 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/desktop/last_folder_manager.py
--rw-rw-rw-   0        0        0    15866 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/desktop/main_gui.py
--rw-rw-rw-   0        0        0    12133 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/desktop/multiselect_widget.py
--rw-rw-rw-   0        0        0     3340 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/desktop/nn_manager.py
--rw-rw-rw-   0        0        0    22055 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/desktop/picks_manager_widget.py
--rw-rw-rw-   0        0        0     2752 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/desktop/radioset_widget.py
--rw-rw-rw-   0        0        0     5246 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/desktop/roi_manager.py
--rw-rw-rw-   0        0        0    15998 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/desktop/settings_processing_widget.py
--rw-rw-rw-   0        0        0     3672 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/desktop/slider_with_values.py
--rw-rw-rw-   0        0        0     5211 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/desktop/spectrum_window.py
--rw-rw-rw-   0        0        0     2978 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/desktop/threads.py
--rw-rw-rw-   0        0        0     6984 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/desktop/tooltip_widget.py
--rw-rw-rw-   0        0        0     8104 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/desktop/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:44:33.716790 first_breaks_picking-0.7.1/first_breaks/exports/
--rw-rw-rw-   0        0        0        0 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/exports/__init__.py
--rw-rw-rw-   0        0        0     4352 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/exports/export_picks.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:44:33.732417 first_breaks_picking-0.7.1/first_breaks/picking/
--rw-rw-rw-   0        0        0        0 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/picking/__init__.py
--rw-rw-rw-   0        0        0     1283 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/picking/ipicker.py
--rw-rw-rw-   0        0        0     6267 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/picking/picker_onnx.py
--rw-rw-rw-   0        0        0     5412 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/picking/picks.py
--rw-rw-rw-   0        0        0     2902 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/picking/task.py
--rw-rw-rw-   0        0        0     2715 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/picking/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:44:33.732417 first_breaks_picking-0.7.1/first_breaks/sgy/
--rw-rw-rw-   0        0        0        0 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/sgy/__init__.py
--rw-rw-rw-   0        0        0     8852 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/sgy/headers.py
--rw-rw-rw-   0        0        0    16909 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/sgy/reader.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:44:33.732417 first_breaks_picking-0.7.1/first_breaks/utils/
--rw-rw-rw-   0        0        0        0 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/utils/__init__.py
--rw-rw-rw-   0        0        0     3058 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/utils/cuda.py
--rw-rw-rw-   0        0        0      654 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/utils/debug.py
--rw-rw-rw-   0        0        0     4195 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/utils/fourier_transforms.py
--rw-rw-rw-   0        0        0     6863 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/utils/utils.py
--rw-rw-rw-   0        0        0     3937 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/first_breaks/utils/visualizations.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:44:33.732417 first_breaks_picking-0.7.1/first_breaks_picking.egg-info/
--rw-rw-rw-   0        0        0    40249 2024-05-26 20:44:33.000000 first_breaks_picking-0.7.1/first_breaks_picking.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1882 2024-05-26 20:44:33.000000 first_breaks_picking-0.7.1/first_breaks_picking.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 20:44:33.000000 first_breaks_picking-0.7.1/first_breaks_picking.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2024-05-26 20:44:33.000000 first_breaks_picking-0.7.1/first_breaks_picking.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      170 2024-05-26 20:44:33.000000 first_breaks_picking-0.7.1/first_breaks_picking.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-26 20:44:33.000000 first_breaks_picking-0.7.1/first_breaks_picking.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2452 2024-05-26 20:43:08.000000 first_breaks_picking-0.7.1/pyproject.toml
--rw-rw-rw-   0        0        0      433 2024-05-26 20:44:33.732417 first_breaks_picking-0.7.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-31 07:13:13.044799 first_breaks_picking-0.7.2/
+-rw-rw-rw-   0        0        0    11558 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/LICENSE
+-rw-rw-rw-   0        0        0       98 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    40120 2024-05-31 07:13:13.044799 first_breaks_picking-0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0    25397 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 07:13:13.013561 first_breaks_picking-0.7.2/first_breaks/
+-rw-rw-rw-   0        0        0        5 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/VERSION
+-rw-rw-rw-   0        0        0     1176 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/__init__.py
+-rw-rw-rw-   0        0        0       96 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/__main__.py
+-rw-rw-rw-   0        0        0      369 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/cli.py
+-rw-rw-rw-   0        0        0     1144 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/const.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:13:13.013561 first_breaks_picking-0.7.2/first_breaks/data_models/
+-rw-rw-rw-   0        0        0        0 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/data_models/__init__.py
+-rw-rw-rw-   0        0        0     2695 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/data_models/dependent.py
+-rw-rw-rw-   0        0        0     4736 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/data_models/independent.py
+-rw-rw-rw-   0        0        0      696 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/data_models/initialised_defaults.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:13:13.029246 first_breaks_picking-0.7.2/first_breaks/desktop/
+-rw-rw-rw-   0        0        0        0 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/desktop/__init__.py
+-rw-rw-rw-   0        0        0     4586 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/desktop/bandfilter_widget.py
+-rw-rw-rw-   0        0        0     5816 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/desktop/byte_encode_unit_widget.py
+-rw-rw-rw-   0        0        0     1969 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/desktop/combobox_with_mapping.py
+-rw-rw-rw-   0        0        0    10802 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/desktop/export_widgets.py
+-rw-rw-rw-   0        0        0    22914 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/desktop/graph.py
+-rw-rw-rw-   0        0        0      776 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/desktop/last_folder_manager.py
+-rw-rw-rw-   0        0        0    15866 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/desktop/main_gui.py
+-rw-rw-rw-   0        0        0    12133 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/desktop/multiselect_widget.py
+-rw-rw-rw-   0        0        0     3340 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/desktop/nn_manager.py
+-rw-rw-rw-   0        0        0    22055 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/desktop/picks_manager_widget.py
+-rw-rw-rw-   0        0        0     2752 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/desktop/radioset_widget.py
+-rw-rw-rw-   0        0        0     5246 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/desktop/roi_manager.py
+-rw-rw-rw-   0        0        0    15998 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/desktop/settings_processing_widget.py
+-rw-rw-rw-   0        0        0     3672 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/desktop/slider_with_values.py
+-rw-rw-rw-   0        0        0     5211 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/desktop/spectrum_window.py
+-rw-rw-rw-   0        0        0     2978 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/desktop/threads.py
+-rw-rw-rw-   0        0        0     6984 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/desktop/tooltip_widget.py
+-rw-rw-rw-   0        0        0     8104 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/desktop/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:13:13.029246 first_breaks_picking-0.7.2/first_breaks/exports/
+-rw-rw-rw-   0        0        0        0 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/exports/__init__.py
+-rw-rw-rw-   0        0        0     4352 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/exports/export_picks.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:13:13.029246 first_breaks_picking-0.7.2/first_breaks/picking/
+-rw-rw-rw-   0        0        0        0 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/picking/__init__.py
+-rw-rw-rw-   0        0        0     1283 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/picking/ipicker.py
+-rw-rw-rw-   0        0        0     6267 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/picking/picker_onnx.py
+-rw-rw-rw-   0        0        0     5412 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/picking/picks.py
+-rw-rw-rw-   0        0        0     2902 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/picking/task.py
+-rw-rw-rw-   0        0        0     2715 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/picking/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:13:13.029246 first_breaks_picking-0.7.2/first_breaks/sgy/
+-rw-rw-rw-   0        0        0        0 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/sgy/__init__.py
+-rw-rw-rw-   0        0        0     8852 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/sgy/headers.py
+-rw-rw-rw-   0        0        0    16909 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/sgy/reader.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:13:13.029246 first_breaks_picking-0.7.2/first_breaks/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/utils/__init__.py
+-rw-rw-rw-   0        0        0     3058 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/utils/cuda.py
+-rw-rw-rw-   0        0        0      654 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/utils/debug.py
+-rw-rw-rw-   0        0        0     4195 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/utils/fourier_transforms.py
+-rw-rw-rw-   0        0        0     6863 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/utils/utils.py
+-rw-rw-rw-   0        0        0     3937 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/first_breaks/utils/visualizations.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:13:13.044799 first_breaks_picking-0.7.2/first_breaks_picking.egg-info/
+-rw-rw-rw-   0        0        0    40120 2024-05-31 07:13:12.000000 first_breaks_picking-0.7.2/first_breaks_picking.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1882 2024-05-31 07:13:12.000000 first_breaks_picking-0.7.2/first_breaks_picking.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 07:13:12.000000 first_breaks_picking-0.7.2/first_breaks_picking.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2024-05-31 07:13:12.000000 first_breaks_picking-0.7.2/first_breaks_picking.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      170 2024-05-31 07:13:12.000000 first_breaks_picking-0.7.2/first_breaks_picking.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 07:13:12.000000 first_breaks_picking-0.7.2/first_breaks_picking.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2452 2024-05-31 07:11:36.000000 first_breaks_picking-0.7.2/pyproject.toml
+-rw-rw-rw-   0        0        0      433 2024-05-31 07:13:13.044799 first_breaks_picking-0.7.2/setup.cfg
```

### Comparing `first_breaks_picking-0.7.1/LICENSE` & `first_breaks_picking-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/PKG-INFO` & `first_breaks_picking-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: first-breaks-picking
-Version: 0.7.1
+Version: 0.7.2
 Summary: Project is devoted to pick waves that are the first to be detected on a seismogram with neural network
 Author: Aleksei Tarasov
 Author-email: Aleksei Tarasov <aleksei.v.tarasov@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -792,38 +792,37 @@
 Click on 2 button to select SGY. After successful reading you can analyze SGY file.
 
 The following mouse interactions are available:
 - Left button drag / Middle button drag: Pan the scene.
 - Right button drag: Scales the scene. Dragging left/right scales horizontally; dragging up/down scales vertically.
 - Right button click: Open dialog with extra options, such as limit by X/Y axes and export.
 - Wheel spin: Zooms the scene in and out.
-- Left click: *After picking with model*, you can manually change picks.
+- Left click: You can manually change values of active picks.
 
 Spectrum analysis:
 - Hold down the **Shift** key, the left mouse button, and select an area: a window with a spectrum will appear.
 You can create as many windows as you like.
 - Move existing windows by dragging with the left mouse button.
 - Delete the window with the spectrum by clicking on it and pressing the **Del** key.
 
 ### Load model
 
 To use picker in desktop app you have to download model. See the `Installation` section for instructions
 on how to download the model.
 
 Click on 1 button and select file with model.
-After successfully loading the model, access to the pick will open.
+After successfully loading the model, access to the pick with NN will open.
 
 ### Settings and Processing
 
 Click on 3 button to open window with different settings and picking parameters:
 
 - The **Processing** section contains parameters for drawing seismograms; these parameters are also used during the
 picking process. Changing them in real time changes the rendering.
 - The **View** section allows you to change the axes' names, content, and orientation.
-- The **External** section allows you to read and display the first picks from the headers of the current file.
 - The **NN Picking** section allows you to select additional parameters for picking the first arrivals and a device
 for calculations. If you have CUDA compatible GPU and installed GPU supported version of library
 (see `Installation` section), you can select `CUDA/GPU` device to use GPU acceleration.
 It can drastically decrease computation time.
 
 A detailed description of the parameters responsible for picking can be found in the `Picking process` chapter.
 
@@ -832,24 +831,26 @@
 
 ### Processing grid
 
 Click on 4 button to toggle the display of the processing grid on or off. Horizontal line
 shows `Maximum time` and vertical lines are drawn at intervals equal to `Traces per gather`. The neural network
 processes blocks independently, as separate images.
 
-### Save results
+### Picks manager
 
-Click on 5 button to save picks into file. Depending on file extension, results will be saved as `json`,
-as plain `txt`, or as `segy` file.
+Click on 5 button to open picks manager. 
 
-For extensions `txt` and `json`, picking parameters and model confidence for each peak are additionally saved.
+When picking with a neural network, the result of the picking will appear here. You can also: add manual picks, 
+load picks from headers, duplicate picks, aggregate several picks, or remove picks.
 
-When choosing an extension `segy`, the copy of original SGY file is saved with the values of the first breaks in the
-trace headers. After selecting a file, you will be prompted to choose in which byte to save (counting starts from 1),
-in which units of measurement and how to encode.
+As control and navigation tools, you can choose to show picks or not (checkbox), select active picks (radio button), 
+and change color (color label).
+
+After selecting one of the picks, you can double-click or click the button with the “save” icon to show the 
+export options.
 
 # Picking process
 
 Neural network process file as series of **images**. There is why **the traces should not be random**,
 since we are using information about adjacent traces.
 
 To obtain the first breaks we do the following steps:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `first_breaks_picking-0.7.1/README.md` & `first_breaks_picking-0.7.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -554,38 +554,37 @@
 Click on 2 button to select SGY. After successful reading you can analyze SGY file.
 
 The following mouse interactions are available:
 - Left button drag / Middle button drag: Pan the scene.
 - Right button drag: Scales the scene. Dragging left/right scales horizontally; dragging up/down scales vertically.
 - Right button click: Open dialog with extra options, such as limit by X/Y axes and export.
 - Wheel spin: Zooms the scene in and out.
-- Left click: *After picking with model*, you can manually change picks.
+- Left click: You can manually change values of active picks.
 
 Spectrum analysis:
 - Hold down the **Shift** key, the left mouse button, and select an area: a window with a spectrum will appear.
 You can create as many windows as you like.
 - Move existing windows by dragging with the left mouse button.
 - Delete the window with the spectrum by clicking on it and pressing the **Del** key.
 
 ### Load model
 
 To use picker in desktop app you have to download model. See the `Installation` section for instructions
 on how to download the model.
 
 Click on 1 button and select file with model.
-After successfully loading the model, access to the pick will open.
+After successfully loading the model, access to the pick with NN will open.
 
 ### Settings and Processing
 
 Click on 3 button to open window with different settings and picking parameters:
 
 - The **Processing** section contains parameters for drawing seismograms; these parameters are also used during the
 picking process. Changing them in real time changes the rendering.
 - The **View** section allows you to change the axes' names, content, and orientation.
-- The **External** section allows you to read and display the first picks from the headers of the current file.
 - The **NN Picking** section allows you to select additional parameters for picking the first arrivals and a device
 for calculations. If you have CUDA compatible GPU and installed GPU supported version of library
 (see `Installation` section), you can select `CUDA/GPU` device to use GPU acceleration.
 It can drastically decrease computation time.
 
 A detailed description of the parameters responsible for picking can be found in the `Picking process` chapter.
 
@@ -594,24 +593,26 @@
 
 ### Processing grid
 
 Click on 4 button to toggle the display of the processing grid on or off. Horizontal line
 shows `Maximum time` and vertical lines are drawn at intervals equal to `Traces per gather`. The neural network
 processes blocks independently, as separate images.
 
-### Save results
+### Picks manager
 
-Click on 5 button to save picks into file. Depending on file extension, results will be saved as `json`,
-as plain `txt`, or as `segy` file.
+Click on 5 button to open picks manager. 
 
-For extensions `txt` and `json`, picking parameters and model confidence for each peak are additionally saved.
+When picking with a neural network, the result of the picking will appear here. You can also: add manual picks, 
+load picks from headers, duplicate picks, aggregate several picks, or remove picks.
 
-When choosing an extension `segy`, the copy of original SGY file is saved with the values of the first breaks in the
-trace headers. After selecting a file, you will be prompted to choose in which byte to save (counting starts from 1),
-in which units of measurement and how to encode.
+As control and navigation tools, you can choose to show picks or not (checkbox), select active picks (radio button), 
+and change color (color label).
+
+After selecting one of the picks, you can double-click or click the button with the “save” icon to show the 
+export options.
 
 # Picking process
 
 Neural network process file as series of **images**. There is why **the traces should not be random**,
 since we are using information about adjacent traces.
 
 To obtain the first breaks we do the following steps:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `first_breaks_picking-0.7.1/first_breaks/__init__.py` & `first_breaks_picking-0.7.2/first_breaks/__init__.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/const.py` & `first_breaks_picking-0.7.2/first_breaks/const.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/data_models/dependent.py` & `first_breaks_picking-0.7.2/first_breaks/data_models/dependent.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/data_models/independent.py` & `first_breaks_picking-0.7.2/first_breaks/data_models/independent.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/data_models/initialised_defaults.py` & `first_breaks_picking-0.7.2/first_breaks/data_models/initialised_defaults.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/desktop/bandfilter_widget.py` & `first_breaks_picking-0.7.2/first_breaks/desktop/bandfilter_widget.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/desktop/byte_encode_unit_widget.py` & `first_breaks_picking-0.7.2/first_breaks/desktop/byte_encode_unit_widget.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/desktop/combobox_with_mapping.py` & `first_breaks_picking-0.7.2/first_breaks/desktop/combobox_with_mapping.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/desktop/export_widgets.py` & `first_breaks_picking-0.7.2/first_breaks/desktop/export_widgets.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/desktop/graph.py` & `first_breaks_picking-0.7.2/first_breaks/desktop/graph.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/desktop/last_folder_manager.py` & `first_breaks_picking-0.7.2/first_breaks/desktop/last_folder_manager.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/desktop/main_gui.py` & `first_breaks_picking-0.7.2/first_breaks/desktop/main_gui.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/desktop/multiselect_widget.py` & `first_breaks_picking-0.7.2/first_breaks/desktop/multiselect_widget.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/desktop/nn_manager.py` & `first_breaks_picking-0.7.2/first_breaks/desktop/nn_manager.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/desktop/picks_manager_widget.py` & `first_breaks_picking-0.7.2/first_breaks/desktop/picks_manager_widget.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/desktop/radioset_widget.py` & `first_breaks_picking-0.7.2/first_breaks/desktop/radioset_widget.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/desktop/roi_manager.py` & `first_breaks_picking-0.7.2/first_breaks/desktop/roi_manager.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/desktop/settings_processing_widget.py` & `first_breaks_picking-0.7.2/first_breaks/desktop/settings_processing_widget.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/desktop/slider_with_values.py` & `first_breaks_picking-0.7.2/first_breaks/desktop/slider_with_values.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/desktop/spectrum_window.py` & `first_breaks_picking-0.7.2/first_breaks/desktop/spectrum_window.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/desktop/threads.py` & `first_breaks_picking-0.7.2/first_breaks/desktop/threads.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/desktop/tooltip_widget.py` & `first_breaks_picking-0.7.2/first_breaks/desktop/tooltip_widget.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/desktop/utils.py` & `first_breaks_picking-0.7.2/first_breaks/desktop/utils.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/exports/export_picks.py` & `first_breaks_picking-0.7.2/first_breaks/exports/export_picks.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/picking/ipicker.py` & `first_breaks_picking-0.7.2/first_breaks/picking/ipicker.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/picking/picker_onnx.py` & `first_breaks_picking-0.7.2/first_breaks/picking/picker_onnx.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/picking/picks.py` & `first_breaks_picking-0.7.2/first_breaks/picking/picks.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/picking/task.py` & `first_breaks_picking-0.7.2/first_breaks/picking/task.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/picking/utils.py` & `first_breaks_picking-0.7.2/first_breaks/picking/utils.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/sgy/headers.py` & `first_breaks_picking-0.7.2/first_breaks/sgy/headers.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/sgy/reader.py` & `first_breaks_picking-0.7.2/first_breaks/sgy/reader.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/utils/cuda.py` & `first_breaks_picking-0.7.2/first_breaks/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/utils/debug.py` & `first_breaks_picking-0.7.2/first_breaks/utils/debug.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/utils/fourier_transforms.py` & `first_breaks_picking-0.7.2/first_breaks/utils/fourier_transforms.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/utils/utils.py` & `first_breaks_picking-0.7.2/first_breaks/utils/utils.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks/utils/visualizations.py` & `first_breaks_picking-0.7.2/first_breaks/utils/visualizations.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/first_breaks_picking.egg-info/PKG-INFO` & `first_breaks_picking-0.7.2/first_breaks_picking.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: first-breaks-picking
-Version: 0.7.1
+Version: 0.7.2
 Summary: Project is devoted to pick waves that are the first to be detected on a seismogram with neural network
 Author: Aleksei Tarasov
 Author-email: Aleksei Tarasov <aleksei.v.tarasov@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -792,38 +792,37 @@
 Click on 2 button to select SGY. After successful reading you can analyze SGY file.
 
 The following mouse interactions are available:
 - Left button drag / Middle button drag: Pan the scene.
 - Right button drag: Scales the scene. Dragging left/right scales horizontally; dragging up/down scales vertically.
 - Right button click: Open dialog with extra options, such as limit by X/Y axes and export.
 - Wheel spin: Zooms the scene in and out.
-- Left click: *After picking with model*, you can manually change picks.
+- Left click: You can manually change values of active picks.
 
 Spectrum analysis:
 - Hold down the **Shift** key, the left mouse button, and select an area: a window with a spectrum will appear.
 You can create as many windows as you like.
 - Move existing windows by dragging with the left mouse button.
 - Delete the window with the spectrum by clicking on it and pressing the **Del** key.
 
 ### Load model
 
 To use picker in desktop app you have to download model. See the `Installation` section for instructions
 on how to download the model.
 
 Click on 1 button and select file with model.
-After successfully loading the model, access to the pick will open.
+After successfully loading the model, access to the pick with NN will open.
 
 ### Settings and Processing
 
 Click on 3 button to open window with different settings and picking parameters:
 
 - The **Processing** section contains parameters for drawing seismograms; these parameters are also used during the
 picking process. Changing them in real time changes the rendering.
 - The **View** section allows you to change the axes' names, content, and orientation.
-- The **External** section allows you to read and display the first picks from the headers of the current file.
 - The **NN Picking** section allows you to select additional parameters for picking the first arrivals and a device
 for calculations. If you have CUDA compatible GPU and installed GPU supported version of library
 (see `Installation` section), you can select `CUDA/GPU` device to use GPU acceleration.
 It can drastically decrease computation time.
 
 A detailed description of the parameters responsible for picking can be found in the `Picking process` chapter.
 
@@ -832,24 +831,26 @@
 
 ### Processing grid
 
 Click on 4 button to toggle the display of the processing grid on or off. Horizontal line
 shows `Maximum time` and vertical lines are drawn at intervals equal to `Traces per gather`. The neural network
 processes blocks independently, as separate images.
 
-### Save results
+### Picks manager
 
-Click on 5 button to save picks into file. Depending on file extension, results will be saved as `json`,
-as plain `txt`, or as `segy` file.
+Click on 5 button to open picks manager. 
 
-For extensions `txt` and `json`, picking parameters and model confidence for each peak are additionally saved.
+When picking with a neural network, the result of the picking will appear here. You can also: add manual picks, 
+load picks from headers, duplicate picks, aggregate several picks, or remove picks.
 
-When choosing an extension `segy`, the copy of original SGY file is saved with the values of the first breaks in the
-trace headers. After selecting a file, you will be prompted to choose in which byte to save (counting starts from 1),
-in which units of measurement and how to encode.
+As control and navigation tools, you can choose to show picks or not (checkbox), select active picks (radio button), 
+and change color (color label).
+
+After selecting one of the picks, you can double-click or click the button with the “save” icon to show the 
+export options.
 
 # Picking process
 
 Neural network process file as series of **images**. There is why **the traces should not be random**,
 since we are using information about adjacent traces.
 
 To obtain the first breaks we do the following steps:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `first_breaks_picking-0.7.1/first_breaks_picking.egg-info/SOURCES.txt` & `first_breaks_picking-0.7.2/first_breaks_picking.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `first_breaks_picking-0.7.1/pyproject.toml` & `first_breaks_picking-0.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 exclude = ["first_breaks._pytorch*"]
 include = ["first_breaks*"]
 
 
 [tool.briefcase]
 project_name = "FirstBreaksPicking"
 bundle = "com.example"
-version = "0.7.1"
+version = "0.7.2"
 url = "https://github.com/DaloroAT/first_breaks_picking"
 license = {file = "LICENSE"}
 
 [tool.briefcase.app.first_breaks]
 formal_name = "FirstBreaksPicking"
 #description = "Project is devoted to pick waves that are the first to be detected on a seismogram with neural network"
 #icon = "src/mypysideapp/resources/appicon" # Briecase will choose the right extension depending the os (png,ico,...)
```

