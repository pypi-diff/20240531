# Comparing `tmp/first_breaks_picking_gpu-0.7.3.tar.gz` & `tmp/first_breaks_picking_gpu-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\a\first_breaks_picking\first_breaks_picking\dist\.tmp-6q43zbtl\first_breaks_picking_gpu-0.7.3.tar", last modified: Fri May 31 07:19:47 2024, max compression
+gzip compressed data, was "D:\a\first_breaks_picking\first_breaks_picking\dist\.tmp-8u75n7ct\first_breaks_picking_gpu-0.7.4.tar", last modified: Fri May 31 07:46:18 2024, max compression
```

## Comparing `first_breaks_picking_gpu-0.7.3.tar` & `first_breaks_picking_gpu-0.7.4.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 07:19:47.706612 first_breaks_picking_gpu-0.7.3/
--rw-rw-rw-   0        0        0    11558 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/LICENSE
--rw-rw-rw-   0        0        0       98 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/MANIFEST.in
--rw-rw-rw-   0        0        0    40147 2024-05-31 07:19:47.706612 first_breaks_picking_gpu-0.7.3/PKG-INFO
--rw-rw-rw-   0        0        0    25397 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 07:19:47.675362 first_breaks_picking_gpu-0.7.3/first_breaks/
--rw-rw-rw-   0        0        0        5 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/VERSION
--rw-rw-rw-   0        0        0     1176 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/__init__.py
--rw-rw-rw-   0        0        0       96 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/__main__.py
--rw-rw-rw-   0        0        0      369 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/cli.py
--rw-rw-rw-   0        0        0     1144 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/const.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:19:47.675362 first_breaks_picking_gpu-0.7.3/first_breaks/data_models/
--rw-rw-rw-   0        0        0        0 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/data_models/__init__.py
--rw-rw-rw-   0        0        0     2695 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/data_models/dependent.py
--rw-rw-rw-   0        0        0     4736 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/data_models/independent.py
--rw-rw-rw-   0        0        0      696 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/data_models/initialised_defaults.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:19:47.690986 first_breaks_picking_gpu-0.7.3/first_breaks/desktop/
--rw-rw-rw-   0        0        0        0 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/desktop/__init__.py
--rw-rw-rw-   0        0        0     4586 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/desktop/bandfilter_widget.py
--rw-rw-rw-   0        0        0     5816 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/desktop/byte_encode_unit_widget.py
--rw-rw-rw-   0        0        0     1969 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/desktop/combobox_with_mapping.py
--rw-rw-rw-   0        0        0    10802 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/desktop/export_widgets.py
--rw-rw-rw-   0        0        0    22914 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/desktop/graph.py
--rw-rw-rw-   0        0        0      776 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/desktop/last_folder_manager.py
--rw-rw-rw-   0        0        0    15866 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/desktop/main_gui.py
--rw-rw-rw-   0        0        0    12133 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/desktop/multiselect_widget.py
--rw-rw-rw-   0        0        0     3340 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/desktop/nn_manager.py
--rw-rw-rw-   0        0        0    22055 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/desktop/picks_manager_widget.py
--rw-rw-rw-   0        0        0     2752 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/desktop/radioset_widget.py
--rw-rw-rw-   0        0        0     5246 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/desktop/roi_manager.py
--rw-rw-rw-   0        0        0    15998 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/desktop/settings_processing_widget.py
--rw-rw-rw-   0        0        0     3672 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/desktop/slider_with_values.py
--rw-rw-rw-   0        0        0     5211 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/desktop/spectrum_window.py
--rw-rw-rw-   0        0        0     2978 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/desktop/threads.py
--rw-rw-rw-   0        0        0     6984 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/desktop/tooltip_widget.py
--rw-rw-rw-   0        0        0     8104 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/desktop/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:19:47.690986 first_breaks_picking_gpu-0.7.3/first_breaks/exports/
--rw-rw-rw-   0        0        0        0 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/exports/__init__.py
--rw-rw-rw-   0        0        0     4352 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/exports/export_picks.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:19:47.690986 first_breaks_picking_gpu-0.7.3/first_breaks/picking/
--rw-rw-rw-   0        0        0        0 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/picking/__init__.py
--rw-rw-rw-   0        0        0     1283 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/picking/ipicker.py
--rw-rw-rw-   0        0        0     6267 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/picking/picker_onnx.py
--rw-rw-rw-   0        0        0     5412 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/picking/picks.py
--rw-rw-rw-   0        0        0     2902 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/picking/task.py
--rw-rw-rw-   0        0        0     2715 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/picking/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:19:47.690986 first_breaks_picking_gpu-0.7.3/first_breaks/sgy/
--rw-rw-rw-   0        0        0        0 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/sgy/__init__.py
--rw-rw-rw-   0        0        0     8852 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/sgy/headers.py
--rw-rw-rw-   0        0        0    16909 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/sgy/reader.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:19:47.706612 first_breaks_picking_gpu-0.7.3/first_breaks/utils/
--rw-rw-rw-   0        0        0        0 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/utils/__init__.py
--rw-rw-rw-   0        0        0     3058 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/utils/cuda.py
--rw-rw-rw-   0        0        0      654 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/utils/debug.py
--rw-rw-rw-   0        0        0     4195 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/utils/fourier_transforms.py
--rw-rw-rw-   0        0        0     6863 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/utils/utils.py
--rw-rw-rw-   0        0        0     3937 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/first_breaks/utils/visualizations.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:19:47.706612 first_breaks_picking_gpu-0.7.3/first_breaks_picking_gpu.egg-info/
--rw-rw-rw-   0        0        0    40147 2024-05-31 07:19:47.000000 first_breaks_picking_gpu-0.7.3/first_breaks_picking_gpu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1906 2024-05-31 07:19:47.000000 first_breaks_picking_gpu-0.7.3/first_breaks_picking_gpu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 07:19:47.000000 first_breaks_picking_gpu-0.7.3/first_breaks_picking_gpu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2024-05-31 07:19:47.000000 first_breaks_picking_gpu-0.7.3/first_breaks_picking_gpu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      174 2024-05-31 07:19:47.000000 first_breaks_picking_gpu-0.7.3/first_breaks_picking_gpu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-31 07:19:47.000000 first_breaks_picking_gpu-0.7.3/first_breaks_picking_gpu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2485 2024-05-31 07:18:17.000000 first_breaks_picking_gpu-0.7.3/pyproject.toml
--rw-rw-rw-   0        0        0      433 2024-05-31 07:19:47.706612 first_breaks_picking_gpu-0.7.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-31 07:46:18.328033 first_breaks_picking_gpu-0.7.4/
+-rw-rw-rw-   0        0        0    11558 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/LICENSE
+-rw-rw-rw-   0        0        0       98 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    40147 2024-05-31 07:46:18.328033 first_breaks_picking_gpu-0.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0    25397 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 07:46:18.296779 first_breaks_picking_gpu-0.7.4/first_breaks/
+-rw-rw-rw-   0        0        0        5 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/VERSION
+-rw-rw-rw-   0        0        0     1176 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/__init__.py
+-rw-rw-rw-   0        0        0       96 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/__main__.py
+-rw-rw-rw-   0        0        0      369 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/cli.py
+-rw-rw-rw-   0        0        0     1144 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/const.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:46:18.296779 first_breaks_picking_gpu-0.7.4/first_breaks/data_models/
+-rw-rw-rw-   0        0        0        0 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/data_models/__init__.py
+-rw-rw-rw-   0        0        0     2695 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/data_models/dependent.py
+-rw-rw-rw-   0        0        0     4736 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/data_models/independent.py
+-rw-rw-rw-   0        0        0      696 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/data_models/initialised_defaults.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:46:18.312406 first_breaks_picking_gpu-0.7.4/first_breaks/desktop/
+-rw-rw-rw-   0        0        0        0 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/desktop/__init__.py
+-rw-rw-rw-   0        0        0     4586 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/desktop/bandfilter_widget.py
+-rw-rw-rw-   0        0        0     5816 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/desktop/byte_encode_unit_widget.py
+-rw-rw-rw-   0        0        0     1969 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/desktop/combobox_with_mapping.py
+-rw-rw-rw-   0        0        0    10802 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/desktop/export_widgets.py
+-rw-rw-rw-   0        0        0    23031 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/desktop/graph.py
+-rw-rw-rw-   0        0        0      776 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/desktop/last_folder_manager.py
+-rw-rw-rw-   0        0        0    15866 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/desktop/main_gui.py
+-rw-rw-rw-   0        0        0    12133 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/desktop/multiselect_widget.py
+-rw-rw-rw-   0        0        0     3340 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/desktop/nn_manager.py
+-rw-rw-rw-   0        0        0    22055 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/desktop/picks_manager_widget.py
+-rw-rw-rw-   0        0        0     2752 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/desktop/radioset_widget.py
+-rw-rw-rw-   0        0        0     5246 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/desktop/roi_manager.py
+-rw-rw-rw-   0        0        0    15998 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/desktop/settings_processing_widget.py
+-rw-rw-rw-   0        0        0     3672 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/desktop/slider_with_values.py
+-rw-rw-rw-   0        0        0     5211 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/desktop/spectrum_window.py
+-rw-rw-rw-   0        0        0     2978 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/desktop/threads.py
+-rw-rw-rw-   0        0        0     6984 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/desktop/tooltip_widget.py
+-rw-rw-rw-   0        0        0     8104 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/desktop/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:46:18.312406 first_breaks_picking_gpu-0.7.4/first_breaks/exports/
+-rw-rw-rw-   0        0        0        0 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/exports/__init__.py
+-rw-rw-rw-   0        0        0     4352 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/exports/export_picks.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:46:18.312406 first_breaks_picking_gpu-0.7.4/first_breaks/picking/
+-rw-rw-rw-   0        0        0        0 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/picking/__init__.py
+-rw-rw-rw-   0        0        0     1283 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/picking/ipicker.py
+-rw-rw-rw-   0        0        0     6241 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/picking/picker_onnx.py
+-rw-rw-rw-   0        0        0     5412 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/picking/picks.py
+-rw-rw-rw-   0        0        0     2902 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/picking/task.py
+-rw-rw-rw-   0        0        0     2715 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/picking/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:46:18.312406 first_breaks_picking_gpu-0.7.4/first_breaks/sgy/
+-rw-rw-rw-   0        0        0        0 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/sgy/__init__.py
+-rw-rw-rw-   0        0        0     8852 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/sgy/headers.py
+-rw-rw-rw-   0        0        0    16909 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/sgy/reader.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:46:18.312406 first_breaks_picking_gpu-0.7.4/first_breaks/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/utils/__init__.py
+-rw-rw-rw-   0        0        0     3058 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/utils/cuda.py
+-rw-rw-rw-   0        0        0      654 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/utils/debug.py
+-rw-rw-rw-   0        0        0     4195 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/utils/fourier_transforms.py
+-rw-rw-rw-   0        0        0     6863 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/utils/utils.py
+-rw-rw-rw-   0        0        0     3937 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/first_breaks/utils/visualizations.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:46:18.328033 first_breaks_picking_gpu-0.7.4/first_breaks_picking_gpu.egg-info/
+-rw-rw-rw-   0        0        0    40147 2024-05-31 07:46:18.000000 first_breaks_picking_gpu-0.7.4/first_breaks_picking_gpu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1906 2024-05-31 07:46:18.000000 first_breaks_picking_gpu-0.7.4/first_breaks_picking_gpu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 07:46:18.000000 first_breaks_picking_gpu-0.7.4/first_breaks_picking_gpu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2024-05-31 07:46:18.000000 first_breaks_picking_gpu-0.7.4/first_breaks_picking_gpu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      174 2024-05-31 07:46:18.000000 first_breaks_picking_gpu-0.7.4/first_breaks_picking_gpu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 07:46:18.000000 first_breaks_picking_gpu-0.7.4/first_breaks_picking_gpu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2485 2024-05-31 07:44:34.000000 first_breaks_picking_gpu-0.7.4/pyproject.toml
+-rw-rw-rw-   0        0        0      433 2024-05-31 07:46:18.328033 first_breaks_picking_gpu-0.7.4/setup.cfg
```

### Comparing `first_breaks_picking_gpu-0.7.3/LICENSE` & `first_breaks_picking_gpu-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/PKG-INFO` & `first_breaks_picking_gpu-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: first-breaks-picking-gpu
-Version: 0.7.3
+Version: 0.7.4
 Summary: Project is devoted to pick waves that are the first to be detected on a seismogram with neural network (CUDA accelerated)
 Author: Aleksei Tarasov
 Author-email: Aleksei Tarasov <aleksei.v.tarasov@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `first_breaks_picking_gpu-0.7.3/README.md` & `first_breaks_picking_gpu-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/__init__.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/__init__.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/const.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/const.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/data_models/dependent.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/data_models/dependent.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/data_models/independent.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/data_models/independent.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/data_models/initialised_defaults.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/data_models/initialised_defaults.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/desktop/bandfilter_widget.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/desktop/bandfilter_widget.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/desktop/byte_encode_unit_widget.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/desktop/byte_encode_unit_widget.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/desktop/combobox_with_mapping.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/desktop/combobox_with_mapping.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/desktop/export_widgets.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/desktop/export_widgets.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/desktop/graph.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/desktop/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,22 @@
         self.sgy = sgy
         self.spectrum_window.set_sgy(sgy)
         self.spectrum_window.set_filter_params(f1_f2, f3_f4)
 
         traces = self.sgy.read()
 
         traces = preprocess_gather(
-            traces, gain=gain, clip=clip, normalize=normalize, f1_f2=f1_f2, f3_f4=f3_f4, fs=self.sgy.fs, copy=True
+            traces,
+            gain=gain,
+            clip=clip,
+            normalize=normalize,
+            f1_f2=f1_f2,
+            f3_f4=f3_f4,
+            fs=self.sgy.fs,
+            copy=True,
         )
 
         # we put clearing after preprocessing to reduce time when user see nothing
         self.clear()
         # axes related checks
         if self.vsp_view != vsp_view:
             self.vsp_view = vsp_view
@@ -170,18 +177,14 @@
         self.pos_ax.showLabel()
         self.graph_updated_signal.emit()
 
     def _plot_trace_fast(self, trace: np.ndarray, time: np.ndarray, shift: int, fill_black: Optional[str]) -> None:
         connect = np.ones(len(time), dtype=np.int32)
         connect[-1] = 0
 
-        if fill_black == "right":
-            trace = np.sign(trace) * trace**3
-            trace = np.gradient(np.gradient(trace)) * 10
-
         trace[0] = 0
         trace[-1] = 0
 
         shifted_trace = trace + shift
 
         path_x, path_y = self.resolve_postime2xy(shifted_trace, time)
         path = pg.arrayToQPath(x=path_x, y=path_y, connect=connect)
@@ -257,15 +260,21 @@
     ) -> None:
         self.remove_processing_region()
 
         num_sample, num_traces = self.sgy.shape
         sgy_end_time = (num_sample + 2) * self.sgy.dt_ms
         region_start_time = maximum_time if maximum_time > 0 else sgy_end_time
 
-        contour_pen = QPen(QColor(*region_contour_color), region_contour_width, Qt.DashLine, Qt.FlatCap, Qt.MiterJoin)
+        contour_pen = QPen(
+            QColor(*region_contour_color),
+            region_contour_width,
+            Qt.DashLine,
+            Qt.FlatCap,
+            Qt.MiterJoin,
+        )
         poly_brush = QColor(*region_poly_color)
 
         # Vertical lines
         line_time = np.array([0, region_start_time])
         for idx in np.arange(traces_per_gather + 0.5, num_traces - 1, traces_per_gather):
             line_pos = np.array([idx, idx])
             line_x, line_y = self.resolve_postime2xy(line_pos, line_time)
@@ -445,15 +454,22 @@
                 width = int(width_per_trace * (traces_window[1] - traces_window[0])) + headers_total_pixels
 
         self.avoid_memory_bomb(height, width)
 
         self.x_ax_header = x_axis
 
         self.clear()
-        self.plotseis(sgy, normalize=normalize, clip=clip, gain=gain, fill_black=fill_black, refresh_view=True)
+        self.plotseis(
+            sgy,
+            normalize=normalize,
+            clip=clip,
+            gain=gain,
+            fill_black=fill_black,
+            refresh_view=True,
+        )
 
         if task:
             self.plot_picks(task.picks)
         elif picks is not None:
             self.plot_picks(picks)
 
         if task is not None and show_processing_region:
```

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/desktop/last_folder_manager.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/desktop/last_folder_manager.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/desktop/main_gui.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/desktop/main_gui.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/desktop/multiselect_widget.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/desktop/multiselect_widget.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/desktop/nn_manager.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/desktop/nn_manager.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/desktop/picks_manager_widget.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/desktop/picks_manager_widget.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/desktop/radioset_widget.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/desktop/radioset_widget.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/desktop/roi_manager.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/desktop/roi_manager.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/desktop/settings_processing_widget.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/desktop/settings_processing_widget.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/desktop/slider_with_values.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/desktop/slider_with_values.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/desktop/spectrum_window.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/desktop/spectrum_window.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/desktop/threads.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/desktop/threads.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/desktop/tooltip_widget.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/desktop/tooltip_widget.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/desktop/utils.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/desktop/utils.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/exports/export_picks.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/exports/export_picks.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/picking/ipicker.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/picking/ipicker.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/picking/picker_onnx.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/picking/picker_onnx.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
     def __len__(self) -> int:
         return len(self.idx2gather_ids)
 
     def __getitem__(self, idx: int) -> Dict[str, np.ndarray]:
         gather_ids = self.idx2gather_ids[idx]
         amplitudes = np.array(
-            [-1 if idx in self.task.traces_to_inverse else 1 for idx in range(len(gather_ids))], dtype=np.float32
+            [-1 if idx in self.task.traces_to_inverse else 1 for idx in range(len(gather_ids))],
+            dtype=np.float32,
         )
         gather = self.task.sgy.read_traces_by_ids(gather_ids)
-        # gather = np.sign(gather) * gather ** 2
-        # gather = np.gradient(np.gradient(gather, axis=0), axis=0)
+
         gather = preprocess_gather(
             data=gather,
             gain=self.task.gain,
             clip=self.task.clip,
             normalize=self.task.normalize,
             f1_f2=self.task.f1_f2,
             f3_f4=self.task.f3_f4,
@@ -63,15 +63,18 @@
             for idx in ids:
                 item = self[idx]
                 gather_batch.append(item[self.gather_key][None, ...])
                 gather_ids_batch.append(item[self.gather_ids_key])
 
             gather_batch = np.stack(gather_batch, axis=0)
             gather_ids_batch = np.hstack(gather_ids_batch)
-            batch = {self.gather_key: gather_batch, self.gather_ids_key: gather_ids_batch}
+            batch = {
+                self.gather_key: gather_batch,
+                self.gather_ids_key: gather_ids_batch,
+            }
             yield batch
 
 
 class PickerONNX(IPicker):
     def __init__(
         self,
         model_path: Optional[Union[str, Path]] = None,
@@ -97,15 +100,17 @@
         sess_opt = ort.SessionOptions()
         sess_opt.graph_optimization_level = ort.GraphOptimizationLevel.ORT_ENABLE_ALL
         if self.device == "cuda":
             sess_opt = ort.SessionOptions()
             sess_opt.intra_op_num_threads = 2
             sess_opt.inter_op_num_threads = 2
         self.model = ort.InferenceSession(
-            str(self.model_path), providers=[ONNX_DEVICE2PROVIDER[self.device]], sess_options=sess_opt
+            str(self.model_path),
+            providers=[ONNX_DEVICE2PROVIDER[self.device]],
+            sess_options=sess_opt,
         )
 
     def change_settings(  # type: ignore
         self, *args: Any, device: Optional[str] = None, batch_size: Optional[int] = None
     ) -> "PickerONNX":
         if args:
             raise ValueError("Use named arguments instead of positional")
```

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/picking/picks.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/picking/picks.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/picking/task.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/picking/task.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/picking/utils.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/picking/utils.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/sgy/headers.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/sgy/headers.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/sgy/reader.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/sgy/reader.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/utils/cuda.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/utils/debug.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/utils/debug.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/utils/fourier_transforms.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/utils/fourier_transforms.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/utils/utils.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/utils/utils.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks/utils/visualizations.py` & `first_breaks_picking_gpu-0.7.4/first_breaks/utils/visualizations.py`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks_picking_gpu.egg-info/PKG-INFO` & `first_breaks_picking_gpu-0.7.4/first_breaks_picking_gpu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: first-breaks-picking-gpu
-Version: 0.7.3
+Version: 0.7.4
 Summary: Project is devoted to pick waves that are the first to be detected on a seismogram with neural network (CUDA accelerated)
 Author: Aleksei Tarasov
 Author-email: Aleksei Tarasov <aleksei.v.tarasov@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `first_breaks_picking_gpu-0.7.3/first_breaks_picking_gpu.egg-info/SOURCES.txt` & `first_breaks_picking_gpu-0.7.4/first_breaks_picking_gpu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `first_breaks_picking_gpu-0.7.3/pyproject.toml` & `first_breaks_picking_gpu-0.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 exclude = ["first_breaks._pytorch*"]
 include = ["first_breaks*"]
 
 
 [tool.briefcase]
 project_name = "FirstBreaksPickingGPU"
 bundle = "com.example"
-version = "0.7.3"
+version = "0.7.4"
 url = "https://github.com/DaloroAT/first_breaks_picking"
 license = {file = "LICENSE"}
 
 [tool.briefcase.app.first_breaks]
 formal_name = "FirstBreaksPickingGPU"
 #description = "Project is devoted to pick waves that are the first to be detected on a seismogram with neural network"
 #icon = "src/mypysideapp/resources/appicon" # Briecase will choose the right extension depending the os (png,ico,...)
```

