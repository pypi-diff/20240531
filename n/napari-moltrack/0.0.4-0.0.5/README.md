# Comparing `tmp/napari_moltrack-0.0.4.tar.gz` & `tmp/napari_moltrack-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_moltrack-0.0.4.tar", last modified: Fri May 31 11:57:30 2024, max compression
+gzip compressed data, was "napari_moltrack-0.0.5.tar", last modified: Fri May 31 18:42:22 2024, max compression
```

## Comparing `napari_moltrack-0.0.4.tar` & `napari_moltrack-0.0.5.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 11:57:30.435154 napari_moltrack-0.0.4/
--rw-rw-rw-   0        0        0     1515 2024-05-29 16:12:09.000000 napari_moltrack-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      101 2024-05-29 16:12:09.000000 napari_moltrack-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     6468 2024-05-31 11:57:30.435154 napari_moltrack-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2705 2024-05-29 16:12:09.000000 napari_moltrack-0.0.4/README.md
--rw-rw-rw-   0        0        0     3406 2024-05-30 17:30:23.000000 napari_moltrack-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-31 11:57:30.435154 napari_moltrack-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-31 11:57:30.357044 napari_moltrack-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-31 11:57:30.372669 napari_moltrack-0.0.4/src/moltrack/
-drwxrwxrwx   0        0        0        0 2024-05-31 11:57:30.372669 napari_moltrack-0.0.4/src/moltrack/GUI/
--rw-rw-rw-   0        0        0        0 2024-05-29 16:42:16.000000 napari_moltrack-0.0.4/src/moltrack/GUI/__init__.py
--rw-rw-rw-   0        0        0    65137 2024-05-31 11:13:52.000000 napari_moltrack-0.0.4/src/moltrack/GUI/widget_ui.py
--rw-rw-rw-   0        0        0       98 2024-05-31 11:57:10.000000 napari_moltrack-0.0.4/src/moltrack/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 11:57:30.388290 napari_moltrack-0.0.4/src/moltrack/_tests/
--rw-rw-rw-   0        0        0        0 2024-05-29 16:12:09.000000 napari_moltrack-0.0.4/src/moltrack/_tests/__init__.py
--rw-rw-rw-   0        0        0     2172 2024-05-29 16:15:26.000000 napari_moltrack-0.0.4/src/moltrack/_tests/test_widget.py
--rw-rw-rw-   0        0        0     6813 2024-05-31 10:26:05.000000 napari_moltrack-0.0.4/src/moltrack/_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-31 11:57:30.403911 napari_moltrack-0.0.4/src/moltrack/funcs/
--rw-rw-rw-   0        0        0        0 2024-05-30 07:19:51.000000 napari_moltrack-0.0.4/src/moltrack/funcs/__init__.py
--rw-rw-rw-   0        0        0     8053 2024-05-30 10:37:04.000000 napari_moltrack-0.0.4/src/moltrack/funcs/compute_utils.py
--rw-rw-rw-   0        0        0    15766 2024-05-31 11:14:50.000000 napari_moltrack-0.0.4/src/moltrack/funcs/events_utils.py
--rw-rw-rw-   0        0        0     8893 2024-05-30 11:25:33.000000 napari_moltrack-0.0.4/src/moltrack/funcs/export_utils.py
--rw-rw-rw-   0        0        0    12905 2024-05-31 09:24:15.000000 napari_moltrack-0.0.4/src/moltrack/funcs/import_utils.py
--rw-rw-rw-   0        0        0     5422 2024-05-30 10:39:02.000000 napari_moltrack-0.0.4/src/moltrack/funcs/loc_filter_utils.py
--rw-rw-rw-   0        0        0    33767 2024-05-30 17:35:51.000000 napari_moltrack-0.0.4/src/moltrack/funcs/picasso_detect_utils.py
--rw-rw-rw-   0        0        0     3282 2024-05-30 10:49:15.000000 napari_moltrack-0.0.4/src/moltrack/funcs/picasso_render_utils.py
--rw-rw-rw-   0        0        0    19259 2024-05-31 11:13:06.000000 napari_moltrack-0.0.4/src/moltrack/funcs/segmentation_utils.py
--rw-rw-rw-   0        0        0     4161 2024-05-30 10:54:17.000000 napari_moltrack-0.0.4/src/moltrack/funcs/tracking_utils.py
--rw-rw-rw-   0        0        0      495 2024-05-29 16:15:26.000000 napari_moltrack-0.0.4/src/moltrack/napari.yaml
-drwxrwxrwx   0        0        0        0 2024-05-31 11:57:30.435154 napari_moltrack-0.0.4/src/napari_moltrack.egg-info/
--rw-rw-rw-   0        0        0     6468 2024-05-31 11:57:30.000000 napari_moltrack-0.0.4/src/napari_moltrack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      975 2024-05-31 11:57:30.000000 napari_moltrack-0.0.4/src/napari_moltrack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 11:57:30.000000 napari_moltrack-0.0.4/src/napari_moltrack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-05-31 11:57:30.000000 napari_moltrack-0.0.4/src/napari_moltrack.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      234 2024-05-31 11:57:30.000000 napari_moltrack-0.0.4/src/napari_moltrack.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-31 11:57:30.000000 napari_moltrack-0.0.4/src/napari_moltrack.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-31 11:57:30.435154 napari_moltrack-0.0.4/src/pygpufit/
--rw-rw-rw-   0        0        0  1982976 2024-05-21 11:03:35.000000 napari_moltrack-0.0.4/src/pygpufit/Gpufit.dll
--rw-rw-rw-   0        0        0        0 2024-05-21 11:03:35.000000 napari_moltrack-0.0.4/src/pygpufit/__init__.py
--rw-rw-rw-   0        0        0    14512 2024-05-21 11:03:35.000000 napari_moltrack-0.0.4/src/pygpufit/gpufit.py
--rw-rw-rw-   0        0        0      140 2024-05-21 11:03:35.000000 napari_moltrack-0.0.4/src/pygpufit/version.py
+drwxrwxrwx   0        0        0        0 2024-05-31 18:42:22.193609 napari_moltrack-0.0.5/
+-rw-rw-rw-   0        0        0     1515 2024-05-29 16:12:09.000000 napari_moltrack-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-05-29 16:12:09.000000 napari_moltrack-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     6468 2024-05-31 18:42:22.193609 napari_moltrack-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2705 2024-05-29 16:12:09.000000 napari_moltrack-0.0.5/README.md
+-rw-rw-rw-   0        0        0     3406 2024-05-30 17:30:23.000000 napari_moltrack-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-31 18:42:22.193609 napari_moltrack-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-31 18:42:22.108997 napari_moltrack-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-31 18:42:22.124618 napari_moltrack-0.0.5/src/moltrack/
+drwxrwxrwx   0        0        0        0 2024-05-31 18:42:22.124618 napari_moltrack-0.0.5/src/moltrack/GUI/
+-rw-rw-rw-   0        0        0        0 2024-05-29 16:42:16.000000 napari_moltrack-0.0.5/src/moltrack/GUI/__init__.py
+-rw-rw-rw-   0        0        0    65658 2024-05-31 18:12:06.000000 napari_moltrack-0.0.5/src/moltrack/GUI/widget_ui.py
+-rw-rw-rw-   0        0        0       98 2024-05-31 18:42:09.000000 napari_moltrack-0.0.5/src/moltrack/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 18:42:22.140240 napari_moltrack-0.0.5/src/moltrack/_tests/
+-rw-rw-rw-   0        0        0        0 2024-05-29 16:12:09.000000 napari_moltrack-0.0.5/src/moltrack/_tests/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-05-29 16:15:26.000000 napari_moltrack-0.0.5/src/moltrack/_tests/test_widget.py
+-rw-rw-rw-   0        0        0     7816 2024-05-31 18:10:07.000000 napari_moltrack-0.0.5/src/moltrack/_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-31 18:42:22.155861 napari_moltrack-0.0.5/src/moltrack/funcs/
+-rw-rw-rw-   0        0        0        0 2024-05-30 07:19:51.000000 napari_moltrack-0.0.5/src/moltrack/funcs/__init__.py
+-rw-rw-rw-   0        0        0     8053 2024-05-30 10:37:04.000000 napari_moltrack-0.0.5/src/moltrack/funcs/compute_utils.py
+-rw-rw-rw-   0        0        0    15734 2024-05-31 17:45:32.000000 napari_moltrack-0.0.5/src/moltrack/funcs/events_utils.py
+-rw-rw-rw-   0        0        0     9155 2024-05-31 18:41:20.000000 napari_moltrack-0.0.5/src/moltrack/funcs/export_utils.py
+-rw-rw-rw-   0        0        0    12905 2024-05-31 09:24:15.000000 napari_moltrack-0.0.5/src/moltrack/funcs/import_utils.py
+-rw-rw-rw-   0        0        0     5422 2024-05-30 10:39:02.000000 napari_moltrack-0.0.5/src/moltrack/funcs/loc_filter_utils.py
+-rw-rw-rw-   0        0        0    33886 2024-05-31 17:45:56.000000 napari_moltrack-0.0.5/src/moltrack/funcs/picasso_detect_utils.py
+-rw-rw-rw-   0        0        0     3282 2024-05-30 10:49:15.000000 napari_moltrack-0.0.5/src/moltrack/funcs/picasso_render_utils.py
+-rw-rw-rw-   0        0        0    10414 2024-05-31 17:30:34.000000 napari_moltrack-0.0.5/src/moltrack/funcs/segmentation_events.py
+-rw-rw-rw-   0        0        0    19142 2024-05-31 17:31:51.000000 napari_moltrack-0.0.5/src/moltrack/funcs/segmentation_utils.py
+-rw-rw-rw-   0        0        0     4477 2024-05-31 18:18:34.000000 napari_moltrack-0.0.5/src/moltrack/funcs/tracking_utils.py
+-rw-rw-rw-   0        0        0      495 2024-05-29 16:15:26.000000 napari_moltrack-0.0.5/src/moltrack/napari.yaml
+drwxrwxrwx   0        0        0        0 2024-05-31 18:42:22.187104 napari_moltrack-0.0.5/src/napari_moltrack.egg-info/
+-rw-rw-rw-   0        0        0     6468 2024-05-31 18:42:22.000000 napari_moltrack-0.0.5/src/napari_moltrack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2024-05-31 18:42:22.000000 napari_moltrack-0.0.5/src/napari_moltrack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 18:42:22.000000 napari_moltrack-0.0.5/src/napari_moltrack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-31 18:42:22.000000 napari_moltrack-0.0.5/src/napari_moltrack.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      234 2024-05-31 18:42:22.000000 napari_moltrack-0.0.5/src/napari_moltrack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-31 18:42:22.000000 napari_moltrack-0.0.5/src/napari_moltrack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 18:42:22.187104 napari_moltrack-0.0.5/src/pygpufit/
+-rw-rw-rw-   0        0        0  1982976 2024-05-21 11:03:35.000000 napari_moltrack-0.0.5/src/pygpufit/Gpufit.dll
+-rw-rw-rw-   0        0        0        0 2024-05-21 11:03:35.000000 napari_moltrack-0.0.5/src/pygpufit/__init__.py
+-rw-rw-rw-   0        0        0    14512 2024-05-21 11:03:35.000000 napari_moltrack-0.0.5/src/pygpufit/gpufit.py
+-rw-rw-rw-   0        0        0      140 2024-05-21 11:03:35.000000 napari_moltrack-0.0.5/src/pygpufit/version.py
```

### Comparing `napari_moltrack-0.0.4/LICENSE` & `napari_moltrack-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.4/PKG-INFO` & `napari_moltrack-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-moltrack
-Version: 0.0.4
+Version: 0.0.5
 Summary: Single molecule tracking package for Napari
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: 
         Copyright (c) 2024, Piers Turner
         All rights reserved.
```

### Comparing `napari_moltrack-0.0.4/README.md` & `napari_moltrack-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.4/pyproject.toml` & `napari_moltrack-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.4/src/moltrack/GUI/widget_ui.py` & `napari_moltrack-0.0.5/src/moltrack/GUI/widget_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -418,30 +418,30 @@
         self.formLayout_3.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.smlm_fit_mode)
         self.picasso_roi_border_width = QtWidgets.QLineEdit(self.tab_21)
         self.picasso_roi_border_width.setObjectName("picasso_roi_border_width")
         self.formLayout_3.setWidget(10, QtWidgets.QFormLayout.FieldRole, self.picasso_roi_border_width)
         self.label_35 = QtWidgets.QLabel(self.tab_21)
         self.label_35.setObjectName("label_35")
         self.formLayout_3.setWidget(10, QtWidgets.QFormLayout.LabelRole, self.label_35)
-        self.stormtracker_window_size = QtWidgets.QSpinBox(self.tab_21)
-        self.stormtracker_window_size.setMaximum(100)
-        self.stormtracker_window_size.setProperty("value", 5)
-        self.stormtracker_window_size.setObjectName("stormtracker_window_size")
-        self.formLayout_3.setWidget(8, QtWidgets.QFormLayout.FieldRole, self.stormtracker_window_size)
-        self.stormtracker_window_size_label = QtWidgets.QLabel(self.tab_21)
-        self.stormtracker_window_size_label.setObjectName("stormtracker_window_size_label")
-        self.formLayout_3.setWidget(8, QtWidgets.QFormLayout.LabelRole, self.stormtracker_window_size_label)
-        self.stormtracker_threshold = QtWidgets.QSpinBox(self.tab_21)
-        self.stormtracker_threshold.setMaximum(255)
-        self.stormtracker_threshold.setProperty("value", 50)
-        self.stormtracker_threshold.setObjectName("stormtracker_threshold")
-        self.formLayout_3.setWidget(7, QtWidgets.QFormLayout.FieldRole, self.stormtracker_threshold)
-        self.stormtracker_threshold_label = QtWidgets.QLabel(self.tab_21)
-        self.stormtracker_threshold_label.setObjectName("stormtracker_threshold_label")
-        self.formLayout_3.setWidget(7, QtWidgets.QFormLayout.LabelRole, self.stormtracker_threshold_label)
+        self.moltrack_window_size = QtWidgets.QSpinBox(self.tab_21)
+        self.moltrack_window_size.setMaximum(100)
+        self.moltrack_window_size.setProperty("value", 5)
+        self.moltrack_window_size.setObjectName("moltrack_window_size")
+        self.formLayout_3.setWidget(8, QtWidgets.QFormLayout.FieldRole, self.moltrack_window_size)
+        self.moltrack_window_size_label = QtWidgets.QLabel(self.tab_21)
+        self.moltrack_window_size_label.setObjectName("moltrack_window_size_label")
+        self.formLayout_3.setWidget(8, QtWidgets.QFormLayout.LabelRole, self.moltrack_window_size_label)
+        self.moltrack_threshold = QtWidgets.QSpinBox(self.tab_21)
+        self.moltrack_threshold.setMaximum(255)
+        self.moltrack_threshold.setProperty("value", 50)
+        self.moltrack_threshold.setObjectName("moltrack_threshold")
+        self.formLayout_3.setWidget(7, QtWidgets.QFormLayout.FieldRole, self.moltrack_threshold)
+        self.moltrack_threshold_label = QtWidgets.QLabel(self.tab_21)
+        self.moltrack_threshold_label.setObjectName("moltrack_threshold_label")
+        self.formLayout_3.setWidget(7, QtWidgets.QFormLayout.LabelRole, self.moltrack_threshold_label)
         self.picasso_min_net_gradient = QtWidgets.QLineEdit(self.tab_21)
         self.picasso_min_net_gradient.setObjectName("picasso_min_net_gradient")
         self.formLayout_3.setWidget(6, QtWidgets.QFormLayout.FieldRole, self.picasso_min_net_gradient)
         self.picasso_min_net_gradient_label = QtWidgets.QLabel(self.tab_21)
         self.picasso_min_net_gradient_label.setObjectName("picasso_min_net_gradient_label")
         self.formLayout_3.setWidget(6, QtWidgets.QFormLayout.LabelRole, self.picasso_min_net_gradient_label)
         self.picasso_box_size = QtWidgets.QComboBox(self.tab_21)
@@ -754,27 +754,34 @@
         self.label_74 = QtWidgets.QLabel(self.tab_6)
         self.label_74.setObjectName("label_74")
         self.verticalLayout_11.addWidget(self.label_74)
         self.formLayout_19 = QtWidgets.QFormLayout()
         self.formLayout_19.setObjectName("formLayout_19")
         self.label_112 = QtWidgets.QLabel(self.tab_6)
         self.label_112.setObjectName("label_112")
-        self.formLayout_19.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_112)
+        self.formLayout_19.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_112)
         self.locs_export_mode = QtWidgets.QComboBox(self.tab_6)
         self.locs_export_mode.setObjectName("locs_export_mode")
         self.locs_export_mode.addItem("")
         self.locs_export_mode.addItem("")
         self.locs_export_mode.addItem("")
-        self.formLayout_19.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.locs_export_mode)
+        self.formLayout_19.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.locs_export_mode)
         self.label_72 = QtWidgets.QLabel(self.tab_6)
         self.label_72.setObjectName("label_72")
-        self.formLayout_19.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_72)
+        self.formLayout_19.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_72)
         self.locs_export_dataset = QtWidgets.QComboBox(self.tab_6)
         self.locs_export_dataset.setObjectName("locs_export_dataset")
-        self.formLayout_19.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.locs_export_dataset)
+        self.formLayout_19.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.locs_export_dataset)
+        self.label_13 = QtWidgets.QLabel(self.tab_6)
+        self.label_13.setObjectName("label_13")
+        self.formLayout_19.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_13)
+        self.locs_export_data = QtWidgets.QComboBox(self.tab_6)
+        self.locs_export_data.setObjectName("locs_export_data")
+        self.locs_export_data.addItem("")
+        self.formLayout_19.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.locs_export_data)
         self.verticalLayout_11.addLayout(self.formLayout_19)
         self.export_localisations = QtWidgets.QPushButton(self.tab_6)
         self.export_localisations.setObjectName("export_localisations")
         self.verticalLayout_11.addWidget(self.export_localisations)
         self.export_progressbar = QtWidgets.QProgressBar(self.tab_6)
         self.export_progressbar.setMaximumSize(QtCore.QSize(16777215, 10))
         self.export_progressbar.setProperty("value", 0)
@@ -901,26 +908,26 @@
         self.translation_target.setItemText(1, _translate("Frame", "Segmentations"))
         self.translation_target.setItemText(2, _translate("Frame", "Both"))
         self.label_10.setText(_translate("Frame", "Press [Control] + [Arrow Key] to move translation target by translation size"))
         self.tabWidget_7.setTabText(self.tabWidget_7.indexOf(self.tab_26), _translate("Frame", "Curate"))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_25), _translate("Frame", "Segment"))
         self.label_3.setText(_translate("Frame", "Detect Localisations"))
         self.label_7.setText(_translate("Frame", "Detect Mode"))
-        self.smlm_detect_mode.setItemText(0, _translate("Frame", "Picasso"))
-        self.smlm_detect_mode.setItemText(1, _translate("Frame", "StormTracker"))
+        self.smlm_detect_mode.setItemText(0, _translate("Frame", "MolTrack"))
+        self.smlm_detect_mode.setItemText(1, _translate("Frame", "Picasso"))
         self.label_11.setText(_translate("Frame", "Dataset"))
         self.label_8.setText(_translate("Frame", "Frame Mode"))
         self.picasso_frame_mode.setItemText(0, _translate("Frame", "Active"))
         self.picasso_frame_mode.setItemText(1, _translate("Frame", "All"))
         self.label.setText(_translate("Frame", "Fit Mode"))
         self.smlm_fit_mode.setItemText(0, _translate("Frame", "Picasso"))
         self.picasso_roi_border_width.setText(_translate("Frame", "5"))
         self.label_35.setText(_translate("Frame", "ROI Border Width (Pixels)"))
-        self.stormtracker_window_size_label.setText(_translate("Frame", "Window Size"))
-        self.stormtracker_threshold_label.setText(_translate("Frame", "Threshold"))
+        self.moltrack_window_size_label.setText(_translate("Frame", "Window Size"))
+        self.moltrack_threshold_label.setText(_translate("Frame", "Threshold"))
         self.picasso_min_net_gradient.setText(_translate("Frame", "1000"))
         self.picasso_min_net_gradient_label.setText(_translate("Frame", "Min Net Gradient"))
         self.picasso_box_size.setItemText(0, _translate("Frame", "3"))
         self.picasso_box_size.setItemText(1, _translate("Frame", "5"))
         self.picasso_box_size.setItemText(2, _translate("Frame", "7"))
         self.picasso_box_size.setItemText(3, _translate("Frame", "9"))
         self.picasso_box_size.setItemText(4, _translate("Frame", "11"))
@@ -1007,11 +1014,13 @@
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_2), _translate("Frame", "SMLM"))
         self.label_74.setText(_translate("Frame", "Localisations will be exported at the import directory"))
         self.label_112.setText(_translate("Frame", "Export Mode"))
         self.locs_export_mode.setItemText(0, _translate("Frame", "Picasso HDF5"))
         self.locs_export_mode.setItemText(1, _translate("Frame", "CSV"))
         self.locs_export_mode.setItemText(2, _translate("Frame", "POS.OUT"))
         self.label_72.setText(_translate("Frame", "Dataset"))
+        self.label_13.setText(_translate("Frame", "Export Data"))
+        self.locs_export_data.setItemText(0, _translate("Frame", "Localisations"))
         self.export_localisations.setText(_translate("Frame", "Export Localisations"))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_6), _translate("Frame", "Export"))
         self.label_12.setText(_translate("Frame", "Display Mode"))
         self.label_14.setText(_translate("Frame", "Dataset"))
```

### Comparing `napari_moltrack-0.0.4/src/moltrack/_tests/test_widget.py` & `napari_moltrack-0.0.5/src/moltrack/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.4/src/moltrack/_widget.py` & `napari_moltrack-0.0.5/src/moltrack/_widget.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,43 @@
+from functools import partial
+from multiprocessing import Manager
 from typing import TYPE_CHECKING
 
-from qtpy.QtWidgets import QWidget
-from multiprocessing import Manager
-from functools import partial
-from qtpy.QtCore import QThreadPool
-from qtpy.QtWidgets import QVBoxLayout
 import pyqtgraph as pg
+from qtpy.QtCore import QThreadPool
+from qtpy.QtWidgets import QVBoxLayout, QWidget
 
 if TYPE_CHECKING:
     import napari
 
-from moltrack.GUI.widget_ui import Ui_Frame as gui
-
-from moltrack.funcs.import_utils import _import_utils
 from moltrack.funcs.compute_utils import _compute_utils
 from moltrack.funcs.events_utils import _events_utils
-from moltrack.funcs.segmentation_utils import _segmentation_utils
-from moltrack.funcs.picasso_detect_utils import _picasso_detect_utils
+from moltrack.funcs.export_utils import _export_utils
+from moltrack.funcs.import_utils import _import_utils
 from moltrack.funcs.loc_filter_utils import _loc_filter_utils
+from moltrack.funcs.picasso_detect_utils import _picasso_detect_utils
 from moltrack.funcs.picasso_render_utils import _picasso_render_utils
+from moltrack.funcs.segmentation_events import _segmentation_events
+from moltrack.funcs.segmentation_utils import _segmentation_utils
 from moltrack.funcs.tracking_utils import _tracking_utils
-from moltrack.funcs.export_utils import _export_utils
+from moltrack.GUI.widget_ui import Ui_Frame as gui
+
+subclasses = [
+    _import_utils,
+    _compute_utils,
+    _events_utils,
+    _segmentation_utils,
+    _picasso_detect_utils,
+    _loc_filter_utils,
+    _picasso_render_utils,
+    _tracking_utils,
+    _export_utils,
+    _segmentation_events,
+]
 
-subclasses = [_import_utils, _compute_utils,
-              _events_utils, _segmentation_utils,
-              _picasso_detect_utils, _loc_filter_utils,
-              _picasso_render_utils, _tracking_utils, _export_utils]
 
 class CustomPyQTGraphWidget(pg.GraphicsLayoutWidget):
 
     def __init__(self, parent):
         super().__init__()
 
         self.parent = parent
@@ -45,123 +53,184 @@
         self.viewer = viewer
 
         # create UI
         self.gui = gui()
         self.gui.setupUi(self)
 
         from moltrack.__init__ import __version__ as version
+
         print(f"napari-moltrack version: {version}")
 
         self.initialise_variables()
         self.initialise_events()
         self.initialise_keybindings()
 
         self.check_gpufit_availibility()
         self.update_detect_options()
 
-        #create threadpool and stop event
+        # create threadpool and stop event
         self.threadpool = QThreadPool()
         manager = Manager()
         self.stop_event = manager.Event()
 
     def initialise_variables(self):
 
-        #initialise graph PyQtGraph canvases
+        # initialise graph PyQtGraph canvases
         self.gui.filter_graph_container.setLayout(QVBoxLayout())
         self.filter_graph_canvas = CustomPyQTGraphWidget(self)
-        self.gui.filter_graph_container.layout().addWidget(self.filter_graph_canvas)
+        self.gui.filter_graph_container.layout().addWidget(
+            self.filter_graph_canvas
+        )
 
         self.dataset_dict = {}
         self.localisation_dict = {}
+        self.tracking_dict = {}
         self.contrast_dict = {}
 
         self.active_dataset = None
 
         self.verbose = False
 
+        self.segmentation_mode = "panzoom"
+        self.interface_mode = "segment"
+
     def initialise_events(self):
 
         self.gui.import_images.clicked.connect(self.init_import_data)
-        self.gui.moltrack_dataset_selector.currentIndexChanged.connect(self.update_active_image)
-
-        self.gui.segment_active.clicked.connect(partial(self.initialise_cellpose, mode = "active"))
-        self.gui.segment_all.clicked.connect(partial(self.initialise_cellpose, mode = "all"))
+        self.gui.moltrack_dataset_selector.currentIndexChanged.connect(
+            self.update_active_image
+        )
+
+        self.gui.segment_active.clicked.connect(
+            partial(self.initialise_cellpose, mode="active")
+        )
+        self.gui.segment_all.clicked.connect(
+            partial(self.initialise_cellpose, mode="all")
+        )
         self.gui.cellpose_load_model.clicked.connect(self.load_cellpose_model)
-        self.gui.dilate_segmentations.clicked.connect(self.dilate_segmentations)
-
-        self.gui.smlm_detect_mode.currentIndexChanged.connect(self.update_detect_options)
-
-        self.gui.picasso_detect.clicked.connect(partial(self.init_picasso, detect = True, fit=False))
-        self.gui.picasso_fit.clicked.connect(partial(self.init_picasso, detect = False, fit=True))
-        self.gui.picasso_detectfit.clicked.connect(partial(self.init_picasso, detect=True, fit=True))
-
-        self.gui.picasso_filter_dataset.currentIndexChanged.connect(self.update_filter_criterion)
-        self.gui.filter_criterion.currentIndexChanged.connect(self.update_criterion_ranges)
-        self.gui.filter_localisations.clicked.connect(self.pixseq_filter_localisations)
-        self.gui.picasso_filter_type.currentIndexChanged.connect(self.update_filter_dataset)
-
-        self.gui.picasso_vis_mode.currentIndexChanged.connect(partial(self.draw_localisations, update_vis=True))
-        self.gui.picasso_vis_size.currentIndexChanged.connect(partial(self.draw_localisations, update_vis=True))
-        self.gui.picasso_vis_opacity.currentIndexChanged.connect(partial(self.draw_localisations, update_vis=True))
-        self.gui.picasso_vis_edge_width.currentIndexChanged.connect(partial(self.draw_localisations, update_vis=True))
+        self.gui.dilate_segmentations.clicked.connect(
+            self.dilate_segmentations
+        )
+
+        self.gui.smlm_detect_mode.currentIndexChanged.connect(
+            self.update_detect_options
+        )
+
+        self.gui.picasso_detect.clicked.connect(
+            partial(self.init_picasso, detect=True, fit=False)
+        )
+        self.gui.picasso_fit.clicked.connect(
+            partial(self.init_picasso, detect=False, fit=True)
+        )
+        self.gui.picasso_detectfit.clicked.connect(
+            partial(self.init_picasso, detect=True, fit=True)
+        )
+
+        self.gui.picasso_filter_dataset.currentIndexChanged.connect(
+            self.update_filter_criterion
+        )
+        self.gui.filter_criterion.currentIndexChanged.connect(
+            self.update_criterion_ranges
+        )
+        self.gui.filter_localisations.clicked.connect(
+            self.pixseq_filter_localisations
+        )
+        self.gui.picasso_filter_type.currentIndexChanged.connect(
+            self.update_filter_dataset
+        )
+
+        self.gui.picasso_vis_mode.currentIndexChanged.connect(
+            partial(self.draw_localisations, update_vis=True)
+        )
+        self.gui.picasso_vis_size.currentIndexChanged.connect(
+            partial(self.draw_localisations, update_vis=True)
+        )
+        self.gui.picasso_vis_opacity.currentIndexChanged.connect(
+            partial(self.draw_localisations, update_vis=True)
+        )
+        self.gui.picasso_vis_edge_width.currentIndexChanged.connect(
+            partial(self.draw_localisations, update_vis=True)
+        )
 
         self.gui.picasso_render.clicked.connect(self.initialise_picasso_render)
 
         self.gui.link_localisations.clicked.connect(self.initialise_tracking)
 
-        self.gui.export_localisations.clicked.connect(self.initialise_export_locs)
+        self.gui.export_localisations.clicked.connect(
+            self.initialise_export_locs
+        )
 
         self.viewer.dims.events.current_step.connect(self.slider_event)
 
     def initialise_keybindings(self):
 
+        self.viewer.bind_key("d", self.devfunc)
 
-        self.viewer.bind_key('d', self.devfunc)
-
-        self.viewer.bind_key(key='Control-Right', func=lambda event: self.moltract_translation(direction="right"), overwrite=True)
-        self.viewer.bind_key(key='Control-Left', func=lambda event: self.moltract_translation(direction="left"), overwrite=True)
-        self.viewer.bind_key(key='Control-Up', func=lambda event: self.moltract_translation(direction="up"), overwrite=True)
-        self.viewer.bind_key(key='Control-Down', func=lambda event: self.moltract_translation(direction="down"), overwrite=True)
+        self.viewer.bind_key(
+            key="Control-Right",
+            func=lambda event: self.moltract_translation(direction="right"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-Left",
+            func=lambda event: self.moltract_translation(direction="left"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-Up",
+            func=lambda event: self.moltract_translation(direction="up"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-Down",
+            func=lambda event: self.moltract_translation(direction="down"),
+            overwrite=True,
+        )
 
+        self.register_segmentation_keybinds(self.viewer)
 
     def devfunc(self, viewer=None):
 
         self.update_ui()
 
     def check_gpufit_availibility(self):
 
         self.gpufit_available = False
 
         try:
             from pygpufit import gpufit as gf
+
             package_installed = True
         except:
             package_installed = False
 
         if package_installed:
 
             if not gf.cuda_available():
                 print("Pygpufit not available due to missing CUDA")
             else:
                 runtime_version, driver_version = gf.get_cuda_version()
 
-                runtime_version = ".".join([str(v) for v in list(runtime_version)])
-                driver_version = ".".join([str(v) for v in list(driver_version)])
+                runtime_version = ".".join(
+                    [str(v) for v in list(runtime_version)]
+                )
+                driver_version = ".".join(
+                    [str(v) for v in list(driver_version)]
+                )
 
                 if runtime_version != driver_version:
-                    print(f"Pygpufit not available due to CUDA version mismatch. "
-                          f"Runtime: {runtime_version}, Driver: {driver_version}")
+                    print(
+                        f"Pygpufit not available due to CUDA version mismatch. "
+                        f"Runtime: {runtime_version}, Driver: {driver_version}"
+                    )
 
                 else:
                     self.gpufit_available = True
 
         else:
             print("Pygpufit not available due to missing package")
             print("Install pygpufit package into napari-PixSeq root directory")
 
         if self.gpufit_available:
             print("GPUFit available")
             self.gui.smlm_fit_mode.addItem("GPUFit")
             self.gui.smlm_fit_mode.setCurrentIndex(1)
-
-
-
```

### Comparing `napari_moltrack-0.0.4/src/moltrack/funcs/compute_utils.py` & `napari_moltrack-0.0.5/src/moltrack/funcs/compute_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.4/src/moltrack/funcs/events_utils.py` & `napari_moltrack-0.0.5/src/moltrack/funcs/events_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -818,169 +818,167 @@
 00003310: 6c66 2e67 7569 2e70 6963 6173 736f 5f6d  lf.gui.picasso_m
 00003320: 696e 5f6e 6574 5f67 7261 6469 656e 745f  in_net_gradient_
 00003330: 6c61 6265 6c2e 7368 6f77 2829 0d0a 2020  label.show()..  
 00003340: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
 00003350: 7569 2e70 6963 6173 736f 5f6d 696e 5f6e  ui.picasso_min_n
 00003360: 6574 5f67 7261 6469 656e 742e 7368 6f77  et_gradient.show
 00003370: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
-00003380: 2020 7365 6c66 2e67 7569 2e73 746f 726d    self.gui.storm
-00003390: 7472 6163 6b65 725f 7468 7265 7368 6f6c  tracker_threshol
-000033a0: 645f 6c61 6265 6c2e 6869 6465 2829 0d0a  d_label.hide()..
-000033b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000033c0: 2e67 7569 2e73 746f 726d 7472 6163 6b65  .gui.stormtracke
-000033d0: 725f 7468 7265 7368 6f6c 642e 6869 6465  r_threshold.hide
-000033e0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-000033f0: 7365 6c66 2e67 7569 2e73 746f 726d 7472  self.gui.stormtr
-00003400: 6163 6b65 725f 7769 6e64 6f77 5f73 697a  acker_window_siz
-00003410: 655f 6c61 6265 6c2e 6869 6465 2829 0d0a  e_label.hide()..
-00003420: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003430: 2e67 7569 2e73 746f 726d 7472 6163 6b65  .gui.stormtracke
-00003440: 725f 7769 6e64 6f77 5f73 697a 652e 6869  r_window_size.hi
-00003450: 6465 2829 0d0a 0d0a 2020 2020 2020 2020  de()....        
-00003460: 656c 7365 3a0d 0a0d 0a20 2020 2020 2020  else:....       
-00003470: 2020 2020 2073 656c 662e 6775 692e 7069       self.gui.pi
-00003480: 6361 7373 6f5f 626f 785f 7369 7a65 5f6c  casso_box_size_l
-00003490: 6162 656c 2e68 6964 6528 290d 0a20 2020  abel.hide()..   
-000034a0: 2020 2020 2020 2020 2073 656c 662e 6775           self.gu
-000034b0: 692e 7069 6361 7373 6f5f 626f 785f 7369  i.picasso_box_si
-000034c0: 7a65 2e68 6964 6528 290d 0a20 2020 2020  ze.hide()..     
-000034d0: 2020 2020 2020 2073 656c 662e 6775 692e         self.gui.
-000034e0: 7069 6361 7373 6f5f 6d69 6e5f 6e65 745f  picasso_min_net_
-000034f0: 6772 6164 6965 6e74 5f6c 6162 656c 2e68  gradient_label.h
-00003500: 6964 6528 290d 0a20 2020 2020 2020 2020  ide()..         
-00003510: 2020 2073 656c 662e 6775 692e 7069 6361     self.gui.pica
-00003520: 7373 6f5f 6d69 6e5f 6e65 745f 6772 6164  sso_min_net_grad
-00003530: 6965 6e74 2e68 6964 6528 290d 0a0d 0a20  ient.hide().... 
-00003540: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003550: 6775 692e 7374 6f72 6d74 7261 636b 6572  gui.stormtracker
-00003560: 5f74 6872 6573 686f 6c64 5f6c 6162 656c  _threshold_label
-00003570: 2e73 686f 7728 290d 0a20 2020 2020 2020  .show()..       
-00003580: 2020 2020 2073 656c 662e 6775 692e 7374       self.gui.st
-00003590: 6f72 6d74 7261 636b 6572 5f74 6872 6573  ormtracker_thres
-000035a0: 686f 6c64 2e73 686f 7728 290d 0a20 2020  hold.show()..   
-000035b0: 2020 2020 2020 2020 2073 656c 662e 6775           self.gu
-000035c0: 692e 7374 6f72 6d74 7261 636b 6572 5f77  i.stormtracker_w
-000035d0: 696e 646f 775f 7369 7a65 5f6c 6162 656c  indow_size_label
-000035e0: 2e73 686f 7728 290d 0a20 2020 2020 2020  .show()..       
-000035f0: 2020 2020 2073 656c 662e 6775 692e 7374       self.gui.st
-00003600: 6f72 6d74 7261 636b 6572 5f77 696e 646f  ormtracker_windo
-00003610: 775f 7369 7a65 2e73 686f 7728 290d 0a0d  w_size.show()...
-00003620: 0a20 2020 2064 6566 206d 6f6c 7472 6163  .    def moltrac
-00003630: 745f 7472 616e 736c 6174 696f 6e28 7365  t_translation(se
-00003640: 6c66 2c20 6576 656e 7420 3d20 4e6f 6e65  lf, event = None
-00003650: 2c20 6469 7265 6374 696f 6e20 3d20 226c  , direction = "l
-00003660: 6566 7422 293a 0d0a 0d0a 2020 2020 2020  eft"):....      
-00003670: 2020 7472 793a 0d0a 0d0a 2020 2020 2020    try:....      
-00003680: 2020 2020 2020 7472 616e 736c 6174 696f        translatio
-00003690: 6e5f 7461 7267 6574 203d 2073 656c 662e  n_target = self.
-000036a0: 6775 692e 7472 616e 736c 6174 696f 6e5f  gui.translation_
-000036b0: 7461 7267 6574 2e63 7572 7265 6e74 5465  target.currentTe
-000036c0: 7874 2829 0d0a 2020 2020 2020 2020 2020  xt()..          
-000036d0: 2020 7369 7a65 203d 2073 656c 662e 6775    size = self.gu
-000036e0: 692e 7472 616e 736c 6174 696f 6e5f 7369  i.translation_si
-000036f0: 7a65 2e76 616c 7565 2829 0d0a 0d0a 2020  ze.value()....  
-00003700: 2020 2020 2020 2020 2020 6966 2064 6972            if dir
-00003710: 6563 7469 6f6e 203d 3d20 2275 7022 3a0d  ection == "up":.
-00003720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003730: 2073 6869 6674 5f76 6563 746f 7220 3d20   shift_vector = 
-00003740: 5b2d 7369 7a65 2c20 302e 305d 0d0a 2020  [-size, 0.0]..  
-00003750: 2020 2020 2020 2020 2020 656c 6966 2064            elif d
-00003760: 6972 6563 7469 6f6e 203d 3d20 2264 6f77  irection == "dow
-00003770: 6e22 3a0d 0a20 2020 2020 2020 2020 2020  n":..           
-00003780: 2020 2020 2073 6869 6674 5f76 6563 746f       shift_vecto
-00003790: 7220 3d20 5b73 697a 652c 2030 2e30 5d0d  r = [size, 0.0].
-000037a0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-000037b0: 6620 6469 7265 6374 696f 6e20 3d3d 2022  f direction == "
-000037c0: 6c65 6674 223a 0d0a 2020 2020 2020 2020  left":..        
-000037d0: 2020 2020 2020 2020 7368 6966 745f 7665          shift_ve
-000037e0: 6374 6f72 203d 205b 302e 302c 202d 7369  ctor = [0.0, -si
-000037f0: 7a65 5d0d 0a20 2020 2020 2020 2020 2020  ze]..           
-00003800: 2065 6c69 6620 6469 7265 6374 696f 6e20   elif direction 
-00003810: 3d3d 2022 7269 6768 7422 3a0d 0a20 2020  == "right":..   
-00003820: 2020 2020 2020 2020 2020 2020 2073 6869               shi
-00003830: 6674 5f76 6563 746f 7220 3d20 5b30 2e30  ft_vector = [0.0
-00003840: 2c20 7369 7a65 5d0d 0a0d 0a20 2020 2020  , size]....     
-00003850: 2020 2020 2020 2069 6620 7472 616e 736c         if transl
-00003860: 6174 696f 6e5f 7461 7267 6574 2069 6e20  ation_target in 
-00003870: 5b22 5365 676d 656e 7461 7469 6f6e 2049  ["Segmentation I
-00003880: 6d61 6765 222c 2022 426f 7468 225d 3a0d  mage", "Both"]:.
-00003890: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000038a0: 2020 2069 6620 6861 7361 7474 7228 7365     if hasattr(se
-000038b0: 6c66 2c20 2273 6567 6d65 6e74 6174 696f  lf, "segmentatio
-000038c0: 6e5f 696d 6167 6522 293a 0d0a 0d0a 2020  n_image"):....  
-000038d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038e0: 2020 696d 6167 6520 3d20 7365 6c66 2e73    image = self.s
-000038f0: 6567 6d65 6e74 6174 696f 6e5f 696d 6167  egmentation_imag
-00003900: 652e 636f 7079 2829 0d0a 0d0a 2020 2020  e.copy()....    
-00003910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003920: 6966 206c 656e 2869 6d61 6765 2e73 6861  if len(image.sha
-00003930: 7065 2920 3d3d 2032 3a0d 0a20 2020 2020  pe) == 2:..     
-00003940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003950: 2020 2069 6d61 6765 203d 2073 6869 6674     image = shift
-00003960: 2869 6d61 6765 2c20 7368 6966 743d 7368  (image, shift=sh
-00003970: 6966 745f 7665 6374 6f72 290d 0a20 2020  ift_vector)..   
-00003980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003990: 2020 2020 2073 656c 662e 7365 676d 656e       self.segmen
-000039a0: 7461 7469 6f6e 5f69 6d61 6765 203d 2069  tation_image = i
-000039b0: 6d61 6765 0d0a 0d0a 2020 2020 2020 2020  mage....        
-000039c0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-000039d0: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
-000039e0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-000039f0: 2066 616d 655f 696e 6465 782c 2066 7261   fame_index, fra
-00003a00: 6d65 2069 6e20 656e 756d 6572 6174 6528  me in enumerate(
-00003a10: 696d 6167 6529 3a0d 0a20 2020 2020 2020  image):..       
-00003a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a30: 2020 2020 2069 6d61 6765 5b66 616d 655f       image[fame_
-00003a40: 696e 6465 785d 203d 2073 6869 6674 2866  index] = shift(f
-00003a50: 7261 6d65 2c20 7368 6966 743d 7368 6966  rame, shift=shif
-00003a60: 745f 7665 6374 6f72 290d 0a20 2020 2020  t_vector)..     
-00003a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a80: 2020 2073 656c 662e 7365 676d 656e 7461     self.segmenta
-00003a90: 7469 6f6e 5f69 6d61 6765 203d 2069 6d61  tion_image = ima
-00003aa0: 6765 0d0a 0d0a 2020 2020 2020 2020 2020  ge....          
-00003ab0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-00003ac0: 7261 775f 7365 676d 656e 7461 7469 6f6e  raw_segmentation
-00003ad0: 5f69 6d61 6765 2829 0d0a 0d0a 2020 2020  _image()....    
-00003ae0: 2020 2020 2020 2020 6966 2074 7261 6e73          if trans
-00003af0: 6c61 7469 6f6e 5f74 6172 6765 7420 696e  lation_target in
-00003b00: 205b 2253 6567 6d65 6e74 6174 696f 6e73   ["Segmentations
-00003b10: 222c 2242 6f74 6822 5d3a 0d0a 0d0a 2020  ","Both"]:....  
-00003b20: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00003b30: 2068 6173 6174 7472 2873 656c 662c 2022   hasattr(self, "
-00003b40: 7365 674c 6179 6572 2229 3a0d 0a0d 0a20  segLayer"):.... 
-00003b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b60: 2020 2073 6567 5f64 6174 6120 3d20 7365     seg_data = se
-00003b70: 6c66 2e73 6567 4c61 7965 722e 6461 7461  lf.segLayer.data
-00003b80: 2e63 6f70 7928 290d 0a0d 0a20 2020 2020  .copy()....     
-00003b90: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00003ba0: 6f72 2073 6567 5f69 6e64 6578 2c20 7365  or seg_index, se
-00003bb0: 6720 696e 2065 6e75 6d65 7261 7465 2873  g in enumerate(s
-00003bc0: 6567 5f64 6174 6129 3a0d 0a0d 0a20 2020  eg_data):....   
-00003bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003be0: 2020 2020 2069 6620 7365 672e 7368 6170       if seg.shap
-00003bf0: 655b 315d 203d 3d20 323a 0d0a 2020 2020  e[1] == 2:..    
-00003c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c10: 2020 2020 2020 2020 7365 6720 3d20 7365          seg = se
-00003c20: 6720 2b20 7368 6966 745f 7665 6374 6f72  g + shift_vector
-00003c30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003c40: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00003c50: 675f 6461 7461 5b73 6567 5f69 6e64 6578  g_data[seg_index
-00003c60: 5d20 3d20 7365 670d 0a20 2020 2020 2020  ] = seg..       
-00003c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c80: 2069 6620 7365 672e 7368 6170 655b 315d   if seg.shape[1]
-00003c90: 203d 3d20 333a 0d0a 2020 2020 2020 2020   == 3:..        
-00003ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cb0: 2020 2020 7365 675b 3a2c 2031 3a5d 203d      seg[:, 1:] =
-00003cc0: 2073 6567 5b3a 2c20 313a 5d20 2b20 7368   seg[:, 1:] + sh
-00003cd0: 6966 745f 7665 6374 6f72 0d0a 2020 2020  ift_vector..    
-00003ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cf0: 2020 2020 2020 2020 7365 675f 6461 7461          seg_data
-00003d00: 5b73 6567 5f69 6e64 6578 5d20 3d20 7365  [seg_index] = se
-00003d10: 670d 0a0d 0a0d 0a20 2020 2020 2020 2020  g......         
-00003d20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003d30: 7365 674c 6179 6572 2e64 6174 6120 3d20  segLayer.data = 
-00003d40: 7365 675f 6461 7461 0d0a 0d0a 0d0a 0d0a  seg_data........
-00003d50: 0d0a 0d0a 0d0a 0d0a 0d0a 0d0a 2020 2020  ............    
-00003d60: 2020 2020 6578 6365 7074 3a0d 0a20 2020      except:..   
-00003d70: 2020 2020 2020 2020 2070 7269 6e74 2874           print(t
-00003d80: 7261 6365 6261 636b 2e66 6f72 6d61 745f  raceback.format_
-00003d90: 6578 6328 2929                           exc())
+00003380: 2020 7365 6c66 2e67 7569 2e6d 6f6c 7472    self.gui.moltr
+00003390: 6163 6b5f 7468 7265 7368 6f6c 645f 6c61  ack_threshold_la
+000033a0: 6265 6c2e 6869 6465 2829 0d0a 2020 2020  bel.hide()..    
+000033b0: 2020 2020 2020 2020 7365 6c66 2e67 7569          self.gui
+000033c0: 2e6d 6f6c 7472 6163 6b5f 7468 7265 7368  .moltrack_thresh
+000033d0: 6f6c 642e 6869 6465 2829 0d0a 2020 2020  old.hide()..    
+000033e0: 2020 2020 2020 2020 7365 6c66 2e67 7569          self.gui
+000033f0: 2e6d 6f6c 7472 6163 6b5f 7769 6e64 6f77  .moltrack_window
+00003400: 5f73 697a 655f 6c61 6265 6c2e 6869 6465  _size_label.hide
+00003410: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00003420: 7365 6c66 2e67 7569 2e6d 6f6c 7472 6163  self.gui.moltrac
+00003430: 6b5f 7769 6e64 6f77 5f73 697a 652e 6869  k_window_size.hi
+00003440: 6465 2829 0d0a 0d0a 2020 2020 2020 2020  de()....        
+00003450: 656c 7365 3a0d 0a0d 0a20 2020 2020 2020  else:....       
+00003460: 2020 2020 2073 656c 662e 6775 692e 7069       self.gui.pi
+00003470: 6361 7373 6f5f 626f 785f 7369 7a65 5f6c  casso_box_size_l
+00003480: 6162 656c 2e68 6964 6528 290d 0a20 2020  abel.hide()..   
+00003490: 2020 2020 2020 2020 2073 656c 662e 6775           self.gu
+000034a0: 692e 7069 6361 7373 6f5f 626f 785f 7369  i.picasso_box_si
+000034b0: 7a65 2e68 6964 6528 290d 0a20 2020 2020  ze.hide()..     
+000034c0: 2020 2020 2020 2073 656c 662e 6775 692e         self.gui.
+000034d0: 7069 6361 7373 6f5f 6d69 6e5f 6e65 745f  picasso_min_net_
+000034e0: 6772 6164 6965 6e74 5f6c 6162 656c 2e68  gradient_label.h
+000034f0: 6964 6528 290d 0a20 2020 2020 2020 2020  ide()..         
+00003500: 2020 2073 656c 662e 6775 692e 7069 6361     self.gui.pica
+00003510: 7373 6f5f 6d69 6e5f 6e65 745f 6772 6164  sso_min_net_grad
+00003520: 6965 6e74 2e68 6964 6528 290d 0a0d 0a20  ient.hide().... 
+00003530: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003540: 6775 692e 6d6f 6c74 7261 636b 5f74 6872  gui.moltrack_thr
+00003550: 6573 686f 6c64 5f6c 6162 656c 2e73 686f  eshold_label.sho
+00003560: 7728 290d 0a20 2020 2020 2020 2020 2020  w()..           
+00003570: 2073 656c 662e 6775 692e 6d6f 6c74 7261   self.gui.moltra
+00003580: 636b 5f74 6872 6573 686f 6c64 2e73 686f  ck_threshold.sho
+00003590: 7728 290d 0a20 2020 2020 2020 2020 2020  w()..           
+000035a0: 2073 656c 662e 6775 692e 6d6f 6c74 7261   self.gui.moltra
+000035b0: 636b 5f77 696e 646f 775f 7369 7a65 5f6c  ck_window_size_l
+000035c0: 6162 656c 2e73 686f 7728 290d 0a20 2020  abel.show()..   
+000035d0: 2020 2020 2020 2020 2073 656c 662e 6775           self.gu
+000035e0: 692e 6d6f 6c74 7261 636b 5f77 696e 646f  i.moltrack_windo
+000035f0: 775f 7369 7a65 2e73 686f 7728 290d 0a0d  w_size.show()...
+00003600: 0a20 2020 2064 6566 206d 6f6c 7472 6163  .    def moltrac
+00003610: 745f 7472 616e 736c 6174 696f 6e28 7365  t_translation(se
+00003620: 6c66 2c20 6576 656e 7420 3d20 4e6f 6e65  lf, event = None
+00003630: 2c20 6469 7265 6374 696f 6e20 3d20 226c  , direction = "l
+00003640: 6566 7422 293a 0d0a 0d0a 2020 2020 2020  eft"):....      
+00003650: 2020 7472 793a 0d0a 0d0a 2020 2020 2020    try:....      
+00003660: 2020 2020 2020 7472 616e 736c 6174 696f        translatio
+00003670: 6e5f 7461 7267 6574 203d 2073 656c 662e  n_target = self.
+00003680: 6775 692e 7472 616e 736c 6174 696f 6e5f  gui.translation_
+00003690: 7461 7267 6574 2e63 7572 7265 6e74 5465  target.currentTe
+000036a0: 7874 2829 0d0a 2020 2020 2020 2020 2020  xt()..          
+000036b0: 2020 7369 7a65 203d 2073 656c 662e 6775    size = self.gu
+000036c0: 692e 7472 616e 736c 6174 696f 6e5f 7369  i.translation_si
+000036d0: 7a65 2e76 616c 7565 2829 0d0a 0d0a 2020  ze.value()....  
+000036e0: 2020 2020 2020 2020 2020 6966 2064 6972            if dir
+000036f0: 6563 7469 6f6e 203d 3d20 2275 7022 3a0d  ection == "up":.
+00003700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003710: 2073 6869 6674 5f76 6563 746f 7220 3d20   shift_vector = 
+00003720: 5b2d 7369 7a65 2c20 302e 305d 0d0a 2020  [-size, 0.0]..  
+00003730: 2020 2020 2020 2020 2020 656c 6966 2064            elif d
+00003740: 6972 6563 7469 6f6e 203d 3d20 2264 6f77  irection == "dow
+00003750: 6e22 3a0d 0a20 2020 2020 2020 2020 2020  n":..           
+00003760: 2020 2020 2073 6869 6674 5f76 6563 746f       shift_vecto
+00003770: 7220 3d20 5b73 697a 652c 2030 2e30 5d0d  r = [size, 0.0].
+00003780: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+00003790: 6620 6469 7265 6374 696f 6e20 3d3d 2022  f direction == "
+000037a0: 6c65 6674 223a 0d0a 2020 2020 2020 2020  left":..        
+000037b0: 2020 2020 2020 2020 7368 6966 745f 7665          shift_ve
+000037c0: 6374 6f72 203d 205b 302e 302c 202d 7369  ctor = [0.0, -si
+000037d0: 7a65 5d0d 0a20 2020 2020 2020 2020 2020  ze]..           
+000037e0: 2065 6c69 6620 6469 7265 6374 696f 6e20   elif direction 
+000037f0: 3d3d 2022 7269 6768 7422 3a0d 0a20 2020  == "right":..   
+00003800: 2020 2020 2020 2020 2020 2020 2073 6869               shi
+00003810: 6674 5f76 6563 746f 7220 3d20 5b30 2e30  ft_vector = [0.0
+00003820: 2c20 7369 7a65 5d0d 0a0d 0a20 2020 2020  , size]....     
+00003830: 2020 2020 2020 2069 6620 7472 616e 736c         if transl
+00003840: 6174 696f 6e5f 7461 7267 6574 2069 6e20  ation_target in 
+00003850: 5b22 5365 676d 656e 7461 7469 6f6e 2049  ["Segmentation I
+00003860: 6d61 6765 222c 2022 426f 7468 225d 3a0d  mage", "Both"]:.
+00003870: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00003880: 2020 2069 6620 6861 7361 7474 7228 7365     if hasattr(se
+00003890: 6c66 2c20 2273 6567 6d65 6e74 6174 696f  lf, "segmentatio
+000038a0: 6e5f 696d 6167 6522 293a 0d0a 0d0a 2020  n_image"):....  
+000038b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038c0: 2020 696d 6167 6520 3d20 7365 6c66 2e73    image = self.s
+000038d0: 6567 6d65 6e74 6174 696f 6e5f 696d 6167  egmentation_imag
+000038e0: 652e 636f 7079 2829 0d0a 0d0a 2020 2020  e.copy()....    
+000038f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003900: 6966 206c 656e 2869 6d61 6765 2e73 6861  if len(image.sha
+00003910: 7065 2920 3d3d 2032 3a0d 0a20 2020 2020  pe) == 2:..     
+00003920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003930: 2020 2069 6d61 6765 203d 2073 6869 6674     image = shift
+00003940: 2869 6d61 6765 2c20 7368 6966 743d 7368  (image, shift=sh
+00003950: 6966 745f 7665 6374 6f72 290d 0a20 2020  ift_vector)..   
+00003960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003970: 2020 2020 2073 656c 662e 7365 676d 656e       self.segmen
+00003980: 7461 7469 6f6e 5f69 6d61 6765 203d 2069  tation_image = i
+00003990: 6d61 6765 0d0a 0d0a 2020 2020 2020 2020  mage....        
+000039a0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000039b0: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
+000039c0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+000039d0: 2066 616d 655f 696e 6465 782c 2066 7261   fame_index, fra
+000039e0: 6d65 2069 6e20 656e 756d 6572 6174 6528  me in enumerate(
+000039f0: 696d 6167 6529 3a0d 0a20 2020 2020 2020  image):..       
+00003a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a10: 2020 2020 2069 6d61 6765 5b66 616d 655f       image[fame_
+00003a20: 696e 6465 785d 203d 2073 6869 6674 2866  index] = shift(f
+00003a30: 7261 6d65 2c20 7368 6966 743d 7368 6966  rame, shift=shif
+00003a40: 745f 7665 6374 6f72 290d 0a20 2020 2020  t_vector)..     
+00003a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a60: 2020 2073 656c 662e 7365 676d 656e 7461     self.segmenta
+00003a70: 7469 6f6e 5f69 6d61 6765 203d 2069 6d61  tion_image = ima
+00003a80: 6765 0d0a 0d0a 2020 2020 2020 2020 2020  ge....          
+00003a90: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00003aa0: 7261 775f 7365 676d 656e 7461 7469 6f6e  raw_segmentation
+00003ab0: 5f69 6d61 6765 2829 0d0a 0d0a 2020 2020  _image()....    
+00003ac0: 2020 2020 2020 2020 6966 2074 7261 6e73          if trans
+00003ad0: 6c61 7469 6f6e 5f74 6172 6765 7420 696e  lation_target in
+00003ae0: 205b 2253 6567 6d65 6e74 6174 696f 6e73   ["Segmentations
+00003af0: 222c 2242 6f74 6822 5d3a 0d0a 0d0a 2020  ","Both"]:....  
+00003b00: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00003b10: 2068 6173 6174 7472 2873 656c 662c 2022   hasattr(self, "
+00003b20: 7365 674c 6179 6572 2229 3a0d 0a0d 0a20  segLayer"):.... 
+00003b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b40: 2020 2073 6567 5f64 6174 6120 3d20 7365     seg_data = se
+00003b50: 6c66 2e73 6567 4c61 7965 722e 6461 7461  lf.segLayer.data
+00003b60: 2e63 6f70 7928 290d 0a0d 0a20 2020 2020  .copy()....     
+00003b70: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00003b80: 6f72 2073 6567 5f69 6e64 6578 2c20 7365  or seg_index, se
+00003b90: 6720 696e 2065 6e75 6d65 7261 7465 2873  g in enumerate(s
+00003ba0: 6567 5f64 6174 6129 3a0d 0a0d 0a20 2020  eg_data):....   
+00003bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bc0: 2020 2020 2069 6620 7365 672e 7368 6170       if seg.shap
+00003bd0: 655b 315d 203d 3d20 323a 0d0a 2020 2020  e[1] == 2:..    
+00003be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bf0: 2020 2020 2020 2020 7365 6720 3d20 7365          seg = se
+00003c00: 6720 2b20 7368 6966 745f 7665 6374 6f72  g + shift_vector
+00003c10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003c20: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003c30: 675f 6461 7461 5b73 6567 5f69 6e64 6578  g_data[seg_index
+00003c40: 5d20 3d20 7365 670d 0a20 2020 2020 2020  ] = seg..       
+00003c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c60: 2069 6620 7365 672e 7368 6170 655b 315d   if seg.shape[1]
+00003c70: 203d 3d20 333a 0d0a 2020 2020 2020 2020   == 3:..        
+00003c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c90: 2020 2020 7365 675b 3a2c 2031 3a5d 203d      seg[:, 1:] =
+00003ca0: 2073 6567 5b3a 2c20 313a 5d20 2b20 7368   seg[:, 1:] + sh
+00003cb0: 6966 745f 7665 6374 6f72 0d0a 2020 2020  ift_vector..    
+00003cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003cd0: 2020 2020 2020 2020 7365 675f 6461 7461          seg_data
+00003ce0: 5b73 6567 5f69 6e64 6578 5d20 3d20 7365  [seg_index] = se
+00003cf0: 670d 0a0d 0a0d 0a20 2020 2020 2020 2020  g......         
+00003d00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003d10: 7365 674c 6179 6572 2e64 6174 6120 3d20  segLayer.data = 
+00003d20: 7365 675f 6461 7461 0d0a 0d0a 0d0a 0d0a  seg_data........
+00003d30: 0d0a 0d0a 0d0a 0d0a 0d0a 0d0a 2020 2020  ............    
+00003d40: 2020 2020 6578 6365 7074 3a0d 0a20 2020      except:..   
+00003d50: 2020 2020 2020 2020 2070 7269 6e74 2874           print(t
+00003d60: 7261 6365 6261 636b 2e66 6f72 6d61 745f  raceback.format_
+00003d70: 6578 6328 2929                           exc())
```

### Comparing `napari_moltrack-0.0.4/src/moltrack/funcs/export_utils.py` & `napari_moltrack-0.0.5/src/moltrack/funcs/export_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -126,14 +126,46 @@
     except Exception as e:
         print(traceback.format_exc())
 
 
 class _export_utils:
 
 
+    def get_export_locs(self, dataset):
+
+        locs = []
+        fitted = False
+        box_size = int(self.gui.picasso_box_size.currentText())
+        min_net_gradient = int(self.gui.picasso_min_net_gradient.text())
+
+        locs_export_data = self.gui.locs_export_data.currentText()
+
+        if dataset in self.localisation_dict.keys():
+            if "localisations" in self.localisation_dict[dataset].keys():
+
+                loc_dict = self.localisation_dict[dataset]
+
+                fitted = loc_dict["fitted"]
+                box_size = loc_dict["box_size"]
+
+                if "min_net_gradient" in loc_dict.keys():
+                    min_net_gradient = loc_dict["min_net_gradient"]
+
+                locs = loc_dict["localisations"]
+
+            if locs_export_data == "Tracks":
+
+                if dataset in self.tracking_dict.keys():
+                    locs = self.tracking_dict[dataset]
+                else:
+                    locs = []
+
+        return locs, fitted, box_size, min_net_gradient
+
+
     def export_locs(self, progress_callback = None, export_dataset = ""):
 
         try:
 
             export_loc_mode = self.gui.locs_export_mode.currentText()
 
             export_loc_jobs = []
@@ -141,66 +173,55 @@
             if export_dataset == "All Datasets":
                 dataset_list = list(self.dataset_dict.keys())
             else:
                 dataset_list = [export_dataset]
 
             for dataset_name in dataset_list:
 
-                if dataset_name in self.localisation_dict.keys():
-                    loc_dict = self.localisation_dict[dataset_name]
+                locs, fitted, box_size, min_net_gradient = self.get_export_locs(dataset_name)
+
+                n_locs = len(locs)
+
+                if n_locs > 0:
+
+                    print(fitted, box_size, min_net_gradient, n_locs, dataset_name)
+
+                    import_path = self.dataset_dict[dataset_name]["path"]
+                    image_shape = self.dataset_dict[dataset_name]["data"].shape
+
+                    base, ext = os.path.splitext(import_path)
+
+                    hdf5_path = base + f"_moltrack_localisations.hdf5"
+                    info_path = base + f"_moltrack_localisations.yaml"
+
+                    if export_loc_mode == "CSV":
+                        export_path = base + f"_moltrack_localisations.csv"
+                    elif export_loc_mode == "POS.OUT":
+                        export_path = base + f"_moltrack_localisations.pos.out"
 
-                    if "localisations" in loc_dict.keys():
-                        locs = loc_dict["localisations"].copy()
+                    else:
+                        export_path = ""
 
-                        n_locs = len(locs)
-                        fitted = loc_dict["fitted"]
+                    picasso_info = [{"Byte Order": "<", "Data Type": "uint16", "File": import_path,
+                                     "Frames": image_shape[0], "Height": image_shape[1],
+                                     "Micro-Manager Acquisiton Comments": "", "Width":image_shape[2],},
+                                    {"Box Size": box_size, "Fit method": "LQ, Gaussian", "Generated by": "Picasso Localize",
+                                     "Min. Net Gradient": min_net_gradient, "Pixelsize": 130, "ROI": None, }]
 
-                        if n_locs > 0 and fitted == True:
-
-                            locs = loc_dict["localisations"]
-                            box_size = loc_dict["box_size"]
-
-                            if "min_net_gradient" in loc_dict.keys():
-                                min_net_gradient = loc_dict["min_net_gradient"]
-                            else:
-                                min_net_gradient = int(self.gui.picasso_min_net_gradient.text())
-
-                            import_path = self.dataset_dict[dataset_name]["path"]
-                            image_shape = self.dataset_dict[dataset_name]["data"].shape
-
-                            base, ext = os.path.splitext(import_path)
-
-                            hdf5_path = base + f"_moltrack_localisations.hdf5"
-                            info_path = base + f"_moltrack_localisations.yaml"
-
-                            if export_loc_mode == "CSV":
-                                export_path = base + f"_moltrack_localisations.csv"
-                            elif export_loc_mode == "POS.OUT":
-                                export_path = base + f"_moltrack_localisations.pos.out"
-
-                            else:
-                                export_path = ""
-
-                            picasso_info = [{"Byte Order": "<", "Data Type": "uint16", "File": import_path,
-                                             "Frames": image_shape[0], "Height": image_shape[1],
-                                             "Micro-Manager Acquisiton Comments": "", "Width":image_shape[2],},
-                                            {"Box Size": box_size, "Fit method": "LQ, Gaussian", "Generated by": "Picasso Localize",
-                                             "Min. Net Gradient": min_net_gradient, "Pixelsize": 130, "ROI": None, }]
-
-                            export_loc_job = { "dataset_name": dataset_name,
-                                               "locs": locs,
-                                               "fitted": fitted,
-                                               "export_mode": export_loc_mode,
-                                               "hdf5_path": hdf5_path,
-                                               "info_path": info_path,
-                                               "export_path": export_path,
-                                               "picasso_info": picasso_info,
-                                              }
+                    export_loc_job = { "dataset_name": dataset_name,
+                                       "locs": locs,
+                                       "fitted": fitted,
+                                       "export_mode": export_loc_mode,
+                                       "hdf5_path": hdf5_path,
+                                       "info_path": info_path,
+                                       "export_path": export_path,
+                                       "picasso_info": picasso_info,
+                                      }
 
-                        export_loc_jobs.append(export_loc_job)
+                    export_loc_jobs.append(export_loc_job)
 
             if len(export_loc_jobs) > 0:
 
                 with concurrent.futures.ThreadPoolExecutor(max_workers=1) as executor:
                     futures = [executor.submit(initialise_localisation_export, job) for job in export_loc_jobs]
 
                     for future in concurrent.futures.as_completed(futures):
```

### Comparing `napari_moltrack-0.0.4/src/moltrack/funcs/import_utils.py` & `napari_moltrack-0.0.5/src/moltrack/funcs/import_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.4/src/moltrack/funcs/loc_filter_utils.py` & `napari_moltrack-0.0.5/src/moltrack/funcs/loc_filter_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.4/src/moltrack/funcs/picasso_detect_utils.py` & `napari_moltrack-0.0.5/src/moltrack/funcs/picasso_detect_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     image_filtered[image_filtered < 0] = 0
 
     return image_filtered
 
 
 
-def detect_stormtracker_locs(dat, progress_list, fit_list):
+def detect_moltrack_locs(dat, progress_list, fit_list):
 
     result = None
 
     try:
         min_net_gradient = dat["min_net_gradient"]
         box_size = dat["box_size"]
         roi = dat["roi"]
@@ -202,45 +202,51 @@
             a = np.maximum(theta[:, 3], theta[:, 4])
             b = np.minimum(theta[:, 3], theta[:, 4])
             ellipticity = (a - b) / a
             photons = theta[:, 0]
             sx = theta[:, 3]
             sy = theta[:, 4]
             bg = theta[:, 5]
-            net_gradient = locs.net_gradient
         else:
             x = theta[:, 0] + locs.x  # - box_offset
             y = theta[:, 1] + locs.y  # - box_offset
             lpx = postprocess.localization_precision(theta[:, 2], theta[:, 4], theta[:, 3], em=em)
             lpy = postprocess.localization_precision(theta[:, 2], theta[:, 5], theta[:, 3], em=em)
             a = np.maximum(theta[:, 4], theta[:, 5])
             b = np.minimum(theta[:, 4], theta[:, 5])
             ellipticity = (a - b) / a
             photons = theta[:, 2]
             sx = theta[:, 4]
             sy = theta[:, 5]
             bg = theta[:, 3]
+
+        if "net_gradient" in locs.dtype.names:
             net_gradient = locs.net_gradient
+        else:
+            net_gradient = None
 
         locs = pd.DataFrame(locs)
 
         locs["x"] = x
         locs["y"] = y
         locs["photons"] = photons
         locs["sx"] = sx
         locs["sy"] = sy
         locs["bg"] = bg
         locs["lpx"] = lpx
         locs["lpy"] = lpy
         locs["ellipticity"] = ellipticity
-        locs["net_gradient"] = net_gradient
+
+        if net_gradient is not None:
+            locs["net_gradient"] = net_gradient
 
         locs = locs.to_records(index=False)
 
     except:
+        print(traceback.format_exc())
         pass
 
     return locs
 
 def fit_spots_lq(spots, locs, box, progress_list):
 
     theta = np.empty((len(spots), 6), dtype=np.float32)
@@ -521,16 +527,16 @@
 
             compute_jobs = []
             n_frames = 0
 
             box_size = int(self.gui.picasso_box_size.currentText())
             remove_overlapping = self.gui.picasso_remove_overlapping.isChecked()
             polygon_filter = self.gui.picasso_segmentation_filtering.isChecked()
-            threshold = int(self.gui.stormtracker_threshold.text())
-            window_size = int(self.gui.stormtracker_window_size.text())
+            threshold = int(self.gui.moltrack_threshold.text())
+            window_size = int(self.gui.moltrack_window_size.text())
 
             segmentation_polygons = self.get_segmentation_polygons()
 
             compute_jobs = []
 
             if self.verbose:
                 print("Creating Picasso compute jobs...")
@@ -575,15 +581,15 @@
 
         progress_list = manager.list()
         fit_jobs = manager.list()
 
         if detect_mode == "Picasso":
             detect_fn = detect_picaso_locs
         else:
-            detect_fn = detect_stormtracker_locs
+            detect_fn = detect_moltrack_locs
 
         start_time = time.time()
 
         futures = {executor.submit(detect_fn,
             job, progress_list, fit_jobs,): job for job in detect_jobs}
 
         while any(not future.done() for future in futures):
```

### Comparing `napari_moltrack-0.0.4/src/moltrack/funcs/picasso_render_utils.py` & `napari_moltrack-0.0.5/src/moltrack/funcs/picasso_render_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.4/src/moltrack/funcs/segmentation_utils.py` & `napari_moltrack-0.0.5/src/moltrack/funcs/segmentation_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,29 +246,28 @@
         try:
 
             layer_names = [layer.name for layer in self.viewer.layers]
 
             mode, masks = result
 
             if mode == "active":
-                shapes = self.mask_to_shape(masks[0], frame = 0)
-                ndim = 2
+                shapes = self.mask_to_shape(masks[0])
             else:
                 shapes = []
-                ndim = 3
                 for i, mask in enumerate(masks):
                     layer_shapes = self.mask_to_shape(mask)
                     shapes.extend(layer_shapes)
 
             if len(shapes) > 0:
-                if "Segmentations" in layer_names:
-                    self.viewer.layers.remove("Segmentations")
 
-                self.segLayer = self.viewer.add_shapes(shapes, shape_type="polygon",
-                    name="Segmentations", opacity=0.3, face_color="red")
+                self.initialise_segLayer(shapes)
+
+
+
+
 
         except:
             print(traceback.format_exc())
             pass
 
     def mask_to_shape(self, mask, frame = None):
 
@@ -490,14 +489,17 @@
             if "Segmentations" in layer_names and filter:
 
                 self.update_ui(init=True)
 
                 segLayer = self.viewer.layers["Segmentations"]
 
                 segmentations = segLayer.data.copy()
+                shape_types = segLayer.shape_type
+
+                segmentations = [seg for seg, shape in zip(segmentations, shape_types) if shape == "polygon"]
 
                 for index, seg in enumerate(segmentations):
 
                     ndim = segmentations[0].shape[1]
 
                     if ndim == 2:
```

### Comparing `napari_moltrack-0.0.4/src/moltrack/funcs/tracking_utils.py` & `napari_moltrack-0.0.5/src/moltrack/funcs/tracking_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import traceback
+
+import numpy as np
 import pandas as pd
 import trackpy as tp
-import numpy as np
+
 from moltrack.funcs.compute_utils import Worker
 
-class _tracking_utils:
 
+class _tracking_utils:
 
     def run_tracking(self, locs, progress_callback=None):
 
         tracks_array = []
 
         try:
 
@@ -17,95 +19,98 @@
             memory = int(self.gui.trackpy_memory.value())
             min_track_length = int(self.gui.min_track_length.value())
 
             columns = list(locs.dtype.names)
 
             locdf = pd.DataFrame(locs, columns=columns)
 
-            tracks_df = tp.link(locdf, search_range=search_range, memory=memory)
+            tracks_df = tp.link(
+                locdf, search_range=search_range, memory=memory
+            )
 
             # Count the frames per track
-            track_lengths = tracks_df.groupby('particle').size()
+            track_lengths = tracks_df.groupby("particle").size()
 
             # Filter tracks by length
-            valid_tracks = track_lengths[track_lengths >= min_track_length].index
-            tracks_df = tracks_df[tracks_df['particle'].isin(valid_tracks)]
+            valid_tracks = track_lengths[
+                track_lengths >= min_track_length
+            ].index
+            tracks_df = tracks_df[tracks_df["particle"].isin(valid_tracks)]
 
             self.tracks = tracks_df
 
             track_index = 1
             for particle, group in tracks_df.groupby("particle"):
                 tracks_df.loc[group.index, "particle"] = track_index
                 track_index += 1
 
-            tracks_df = tracks_df[['particle', 'frame', 'y', 'x']]
+            # tracks_df = tracks_df[['particle', 'frame', 'y', 'x']]
             tracks_df = tracks_df.sort_values(by=["particle", "frame"])
-
-            tracks_array = tracks_df.to_records(index=False)
-            tracks_array = [list(track) for track in tracks_array]
-            tracks_array = np.array(tracks_array)
+            tracks = tracks_df.to_records(index=False)
 
         except:
             print(traceback.format_exc())
 
-        return tracks_array
+        return tracks
 
-    def process_tracking_results(self, tracks_array):
+    def process_tracking_results(self, tracks):
 
         try:
-
             dataset = self.gui.tracking_dataset.currentText()
-            remove_unlinked = self.gui.remove_unlinked.isChecked()
 
+            if dataset not in self.tracking_dict.keys():
+                self.tracking_dict[dataset] = tracks
+
+            remove_unlinked = self.gui.remove_unlinked.isChecked()
             n_frames = self.dataset_dict[dataset]["data"].shape[0]
 
             layers_names = [layer.name for layer in self.viewer.layers]
 
-            render_tracks = tracks_array.copy()
-            render_tracks[:,1] = 0
+            render_tracks = pd.DataFrame(tracks)
+            render_tracks = render_tracks[["particle", "frame", "y", "x"]]
+            render_tracks = render_tracks.to_records(index=False)
+            render_tracks = [list(track) for track in render_tracks]
+            render_tracks = np.array(render_tracks).copy()
+            render_tracks[:, 1] = 0
 
             if "Tracks" not in layers_names:
-                self.track_layer = self.viewer.add_tracks(render_tracks, name="Tracks")
+                self.track_layer = self.viewer.add_tracks(
+                    render_tracks, name="Tracks"
+                )
             else:
                 self.track_layer.data = render_tracks
 
             self.track_layer.tail_length = n_frames * 2
 
+            self.gui.locs_export_data.clear()
+            self.gui.locs_export_data.addItems(["Localisations","Tracks"])
+
             if remove_unlinked:
 
                 loc_dict = self.localisation_dict[dataset]
 
                 locs = loc_dict["localisations"]
                 n_locs = len(locs)
-
-                filtered_locs = pd.DataFrame(tracks_array,
-                    columns=["particle", "frame", "y", "x"])
-                filtered_locs = filtered_locs.to_records(index=False)
-
-                n_filtered = len(filtered_locs)
+                n_filtered = len(tracks)
 
                 n_removed = n_locs - n_filtered
 
                 if n_removed > 0:
                     print(f"Removed {n_removed} unlinked localisations")
 
-                    loc_dict["localisations"] = filtered_locs
-
-
+                    loc_dict["localisations"] = tracks
 
         except:
             print(traceback.format_exc())
 
-
     def tracking_finished(self):
 
         self.draw_localisations()
         self.update_ui()
 
-
     def initialise_tracking(self):
 
         try:
 
             dataset = self.gui.tracking_dataset.currentText()
 
             if dataset in self.localisation_dict.keys():
@@ -119,19 +124,19 @@
                     if len(locs) > 0:
 
                         self.update_ui(init=True)
 
                         locs = loc_dict["localisations"].copy()
 
                         worker = Worker(self.run_tracking, locs)
-                        worker.signals.result.connect(self.process_tracking_results)
+                        worker.signals.result.connect(
+                            self.process_tracking_results
+                        )
                         worker.signals.finished.connect(self.tracking_finished)
                         self.threadpool.start(worker)
 
             else:
                 print(f"No localisations found for {dataset}`")
 
         except:
             print(traceback.format_exc())
             self.update_ui()
-
-
```

### Comparing `napari_moltrack-0.0.4/src/napari_moltrack.egg-info/PKG-INFO` & `napari_moltrack-0.0.5/src/napari_moltrack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-moltrack
-Version: 0.0.4
+Version: 0.0.5
 Summary: Single molecule tracking package for Napari
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: 
         Copyright (c) 2024, Piers Turner
         All rights reserved.
```

### Comparing `napari_moltrack-0.0.4/src/napari_moltrack.egg-info/SOURCES.txt` & `napari_moltrack-0.0.5/src/napari_moltrack.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 src/moltrack/funcs/compute_utils.py
 src/moltrack/funcs/events_utils.py
 src/moltrack/funcs/export_utils.py
 src/moltrack/funcs/import_utils.py
 src/moltrack/funcs/loc_filter_utils.py
 src/moltrack/funcs/picasso_detect_utils.py
 src/moltrack/funcs/picasso_render_utils.py
+src/moltrack/funcs/segmentation_events.py
 src/moltrack/funcs/segmentation_utils.py
 src/moltrack/funcs/tracking_utils.py
 src/napari_moltrack.egg-info/PKG-INFO
 src/napari_moltrack.egg-info/SOURCES.txt
 src/napari_moltrack.egg-info/dependency_links.txt
 src/napari_moltrack.egg-info/entry_points.txt
 src/napari_moltrack.egg-info/requires.txt
```

### Comparing `napari_moltrack-0.0.4/src/pygpufit/Gpufit.dll` & `napari_moltrack-0.0.5/src/pygpufit/Gpufit.dll`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.4/src/pygpufit/gpufit.py` & `napari_moltrack-0.0.5/src/pygpufit/gpufit.py`

 * *Files identical despite different names*

