# Comparing `tmp/napari_moltrack-0.0.3.tar.gz` & `tmp/napari_moltrack-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_moltrack-0.0.3.tar", last modified: Thu May 30 17:38:09 2024, max compression
+gzip compressed data, was "napari_moltrack-0.0.4.tar", last modified: Fri May 31 11:57:30 2024, max compression
```

## Comparing `napari_moltrack-0.0.3.tar` & `napari_moltrack-0.0.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 17:38:09.599934 napari_moltrack-0.0.3/
--rw-rw-rw-   0        0        0     1515 2024-05-29 16:12:09.000000 napari_moltrack-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      101 2024-05-29 16:12:09.000000 napari_moltrack-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6468 2024-05-30 17:38:09.599934 napari_moltrack-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2705 2024-05-29 16:12:09.000000 napari_moltrack-0.0.3/README.md
--rw-rw-rw-   0        0        0     3406 2024-05-30 17:30:23.000000 napari_moltrack-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-30 17:38:09.599934 napari_moltrack-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-30 17:38:09.530942 napari_moltrack-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-30 17:38:09.546564 napari_moltrack-0.0.3/src/moltrack/
-drwxrwxrwx   0        0        0        0 2024-05-30 17:38:09.546564 napari_moltrack-0.0.3/src/moltrack/GUI/
--rw-rw-rw-   0        0        0        0 2024-05-29 16:42:16.000000 napari_moltrack-0.0.3/src/moltrack/GUI/__init__.py
--rw-rw-rw-   0        0        0    61681 2024-05-30 13:51:32.000000 napari_moltrack-0.0.3/src/moltrack/GUI/widget_ui.py
--rw-rw-rw-   0        0        0       98 2024-05-30 17:37:59.000000 napari_moltrack-0.0.3/src/moltrack/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 17:38:09.562213 napari_moltrack-0.0.3/src/moltrack/_tests/
--rw-rw-rw-   0        0        0        0 2024-05-29 16:12:09.000000 napari_moltrack-0.0.3/src/moltrack/_tests/__init__.py
--rw-rw-rw-   0        0        0     2172 2024-05-29 16:15:26.000000 napari_moltrack-0.0.3/src/moltrack/_tests/test_widget.py
--rw-rw-rw-   0        0        0     6368 2024-05-30 17:35:51.000000 napari_moltrack-0.0.3/src/moltrack/_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-30 17:38:09.577834 napari_moltrack-0.0.3/src/moltrack/funcs/
--rw-rw-rw-   0        0        0        0 2024-05-30 07:19:51.000000 napari_moltrack-0.0.3/src/moltrack/funcs/__init__.py
--rw-rw-rw-   0        0        0     8053 2024-05-30 10:37:04.000000 napari_moltrack-0.0.3/src/moltrack/funcs/compute_utils.py
--rw-rw-rw-   0        0        0    13311 2024-05-30 12:41:31.000000 napari_moltrack-0.0.3/src/moltrack/funcs/events_utils.py
--rw-rw-rw-   0        0        0     8893 2024-05-30 11:25:33.000000 napari_moltrack-0.0.3/src/moltrack/funcs/export_utils.py
--rw-rw-rw-   0        0        0    13425 2024-05-30 17:25:19.000000 napari_moltrack-0.0.3/src/moltrack/funcs/import_utils.py
--rw-rw-rw-   0        0        0     5422 2024-05-30 10:39:02.000000 napari_moltrack-0.0.3/src/moltrack/funcs/loc_filter_utils.py
--rw-rw-rw-   0        0        0    33767 2024-05-30 17:35:51.000000 napari_moltrack-0.0.3/src/moltrack/funcs/picasso_detect_utils.py
--rw-rw-rw-   0        0        0     3282 2024-05-30 10:49:15.000000 napari_moltrack-0.0.3/src/moltrack/funcs/picasso_render_utils.py
--rw-rw-rw-   0        0        0    18504 2024-05-30 09:31:37.000000 napari_moltrack-0.0.3/src/moltrack/funcs/segmentation_utils.py
--rw-rw-rw-   0        0        0     4161 2024-05-30 10:54:17.000000 napari_moltrack-0.0.3/src/moltrack/funcs/tracking_utils.py
--rw-rw-rw-   0        0        0      495 2024-05-29 16:15:26.000000 napari_moltrack-0.0.3/src/moltrack/napari.yaml
-drwxrwxrwx   0        0        0        0 2024-05-30 17:38:09.599934 napari_moltrack-0.0.3/src/napari_moltrack.egg-info/
--rw-rw-rw-   0        0        0     6468 2024-05-30 17:38:09.000000 napari_moltrack-0.0.3/src/napari_moltrack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      975 2024-05-30 17:38:09.000000 napari_moltrack-0.0.3/src/napari_moltrack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 17:38:09.000000 napari_moltrack-0.0.3/src/napari_moltrack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-05-30 17:38:09.000000 napari_moltrack-0.0.3/src/napari_moltrack.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      234 2024-05-30 17:38:09.000000 napari_moltrack-0.0.3/src/napari_moltrack.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-30 17:38:09.000000 napari_moltrack-0.0.3/src/napari_moltrack.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-30 17:38:09.599934 napari_moltrack-0.0.3/src/pygpufit/
--rw-rw-rw-   0        0        0  1982976 2024-05-21 11:03:35.000000 napari_moltrack-0.0.3/src/pygpufit/Gpufit.dll
--rw-rw-rw-   0        0        0        0 2024-05-21 11:03:35.000000 napari_moltrack-0.0.3/src/pygpufit/__init__.py
--rw-rw-rw-   0        0        0    14512 2024-05-21 11:03:35.000000 napari_moltrack-0.0.3/src/pygpufit/gpufit.py
--rw-rw-rw-   0        0        0      140 2024-05-21 11:03:35.000000 napari_moltrack-0.0.3/src/pygpufit/version.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:57:30.435154 napari_moltrack-0.0.4/
+-rw-rw-rw-   0        0        0     1515 2024-05-29 16:12:09.000000 napari_moltrack-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-05-29 16:12:09.000000 napari_moltrack-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6468 2024-05-31 11:57:30.435154 napari_moltrack-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2705 2024-05-29 16:12:09.000000 napari_moltrack-0.0.4/README.md
+-rw-rw-rw-   0        0        0     3406 2024-05-30 17:30:23.000000 napari_moltrack-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-31 11:57:30.435154 napari_moltrack-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-31 11:57:30.357044 napari_moltrack-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-31 11:57:30.372669 napari_moltrack-0.0.4/src/moltrack/
+drwxrwxrwx   0        0        0        0 2024-05-31 11:57:30.372669 napari_moltrack-0.0.4/src/moltrack/GUI/
+-rw-rw-rw-   0        0        0        0 2024-05-29 16:42:16.000000 napari_moltrack-0.0.4/src/moltrack/GUI/__init__.py
+-rw-rw-rw-   0        0        0    65137 2024-05-31 11:13:52.000000 napari_moltrack-0.0.4/src/moltrack/GUI/widget_ui.py
+-rw-rw-rw-   0        0        0       98 2024-05-31 11:57:10.000000 napari_moltrack-0.0.4/src/moltrack/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:57:30.388290 napari_moltrack-0.0.4/src/moltrack/_tests/
+-rw-rw-rw-   0        0        0        0 2024-05-29 16:12:09.000000 napari_moltrack-0.0.4/src/moltrack/_tests/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-05-29 16:15:26.000000 napari_moltrack-0.0.4/src/moltrack/_tests/test_widget.py
+-rw-rw-rw-   0        0        0     6813 2024-05-31 10:26:05.000000 napari_moltrack-0.0.4/src/moltrack/_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:57:30.403911 napari_moltrack-0.0.4/src/moltrack/funcs/
+-rw-rw-rw-   0        0        0        0 2024-05-30 07:19:51.000000 napari_moltrack-0.0.4/src/moltrack/funcs/__init__.py
+-rw-rw-rw-   0        0        0     8053 2024-05-30 10:37:04.000000 napari_moltrack-0.0.4/src/moltrack/funcs/compute_utils.py
+-rw-rw-rw-   0        0        0    15766 2024-05-31 11:14:50.000000 napari_moltrack-0.0.4/src/moltrack/funcs/events_utils.py
+-rw-rw-rw-   0        0        0     8893 2024-05-30 11:25:33.000000 napari_moltrack-0.0.4/src/moltrack/funcs/export_utils.py
+-rw-rw-rw-   0        0        0    12905 2024-05-31 09:24:15.000000 napari_moltrack-0.0.4/src/moltrack/funcs/import_utils.py
+-rw-rw-rw-   0        0        0     5422 2024-05-30 10:39:02.000000 napari_moltrack-0.0.4/src/moltrack/funcs/loc_filter_utils.py
+-rw-rw-rw-   0        0        0    33767 2024-05-30 17:35:51.000000 napari_moltrack-0.0.4/src/moltrack/funcs/picasso_detect_utils.py
+-rw-rw-rw-   0        0        0     3282 2024-05-30 10:49:15.000000 napari_moltrack-0.0.4/src/moltrack/funcs/picasso_render_utils.py
+-rw-rw-rw-   0        0        0    19259 2024-05-31 11:13:06.000000 napari_moltrack-0.0.4/src/moltrack/funcs/segmentation_utils.py
+-rw-rw-rw-   0        0        0     4161 2024-05-30 10:54:17.000000 napari_moltrack-0.0.4/src/moltrack/funcs/tracking_utils.py
+-rw-rw-rw-   0        0        0      495 2024-05-29 16:15:26.000000 napari_moltrack-0.0.4/src/moltrack/napari.yaml
+drwxrwxrwx   0        0        0        0 2024-05-31 11:57:30.435154 napari_moltrack-0.0.4/src/napari_moltrack.egg-info/
+-rw-rw-rw-   0        0        0     6468 2024-05-31 11:57:30.000000 napari_moltrack-0.0.4/src/napari_moltrack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      975 2024-05-31 11:57:30.000000 napari_moltrack-0.0.4/src/napari_moltrack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 11:57:30.000000 napari_moltrack-0.0.4/src/napari_moltrack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-31 11:57:30.000000 napari_moltrack-0.0.4/src/napari_moltrack.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      234 2024-05-31 11:57:30.000000 napari_moltrack-0.0.4/src/napari_moltrack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-31 11:57:30.000000 napari_moltrack-0.0.4/src/napari_moltrack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 11:57:30.435154 napari_moltrack-0.0.4/src/pygpufit/
+-rw-rw-rw-   0        0        0  1982976 2024-05-21 11:03:35.000000 napari_moltrack-0.0.4/src/pygpufit/Gpufit.dll
+-rw-rw-rw-   0        0        0        0 2024-05-21 11:03:35.000000 napari_moltrack-0.0.4/src/pygpufit/__init__.py
+-rw-rw-rw-   0        0        0    14512 2024-05-21 11:03:35.000000 napari_moltrack-0.0.4/src/pygpufit/gpufit.py
+-rw-rw-rw-   0        0        0      140 2024-05-21 11:03:35.000000 napari_moltrack-0.0.4/src/pygpufit/version.py
```

### Comparing `napari_moltrack-0.0.3/LICENSE` & `napari_moltrack-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.3/PKG-INFO` & `napari_moltrack-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-moltrack
-Version: 0.0.3
+Version: 0.0.4
 Summary: Single molecule tracking package for Napari
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: 
         Copyright (c) 2024, Piers Turner
         All rights reserved.
```

### Comparing `napari_moltrack-0.0.3/README.md` & `napari_moltrack-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.3/pyproject.toml` & `napari_moltrack-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.3/src/moltrack/GUI/widget_ui.py` & `napari_moltrack-0.0.4/src/moltrack/GUI/widget_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,40 +40,51 @@
         self.tab_15.setObjectName("tab_15")
         self.verticalLayout_18 = QtWidgets.QVBoxLayout(self.tab_15)
         self.verticalLayout_18.setObjectName("verticalLayout_18")
         self.formLayout = QtWidgets.QFormLayout()
         self.formLayout.setObjectName("formLayout")
         self.label_22 = QtWidgets.QLabel(self.tab_15)
         self.label_22.setObjectName("label_22")
-        self.formLayout.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_22)
+        self.formLayout.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_22)
         self.import_crop_mode = QtWidgets.QComboBox(self.tab_15)
         self.import_crop_mode.setObjectName("import_crop_mode")
         self.import_crop_mode.addItem("")
         self.import_crop_mode.addItem("")
         self.import_crop_mode.addItem("")
         self.import_crop_mode.addItem("")
-        self.formLayout.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.import_crop_mode)
+        self.formLayout.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.import_crop_mode)
         self.label_32 = QtWidgets.QLabel(self.tab_15)
         self.label_32.setObjectName("label_32")
         self.formLayout.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_32)
         self.import_limit = QtWidgets.QComboBox(self.tab_15)
         self.import_limit.setObjectName("import_limit")
         self.import_limit.addItem("")
         self.import_limit.addItem("")
         self.import_limit.addItem("")
         self.import_limit.addItem("")
         self.import_limit.addItem("")
         self.import_limit.addItem("")
         self.import_limit.addItem("")
         self.import_limit.addItem("")
         self.formLayout.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.import_limit)
+        self.label_6 = QtWidgets.QLabel(self.tab_15)
+        self.label_6.setObjectName("label_6")
+        self.formLayout.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_6)
+        self.import_mode = QtWidgets.QComboBox(self.tab_15)
+        self.import_mode.setObjectName("import_mode")
+        self.import_mode.addItem("")
+        self.import_mode.addItem("")
+        self.formLayout.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.import_mode)
         self.verticalLayout_18.addLayout(self.formLayout)
         self.import_concatenate = QtWidgets.QCheckBox(self.tab_15)
         self.import_concatenate.setObjectName("import_concatenate")
         self.verticalLayout_18.addWidget(self.import_concatenate)
+        self.frame_averaging = QtWidgets.QCheckBox(self.tab_15)
+        self.frame_averaging.setObjectName("frame_averaging")
+        self.verticalLayout_18.addWidget(self.frame_averaging)
         spacerItem = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout_18.addItem(spacerItem)
         self.import_images = QtWidgets.QPushButton(self.tab_15)
         self.import_images.setObjectName("import_images")
         self.verticalLayout_18.addWidget(self.import_images)
         self.tabWidget_4.addTab(self.tab_15, "")
         self.tab_16 = QtWidgets.QWidget()
@@ -316,18 +327,50 @@
         self.formLayout_26.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.dilatation_size)
         self.verticalLayout_30.addLayout(self.formLayout_26)
         self.dilate_segmentations = QtWidgets.QPushButton(self.tab_26)
         self.dilate_segmentations.setObjectName("dilate_segmentations")
         self.verticalLayout_30.addWidget(self.dilate_segmentations)
         spacerItem6 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout_30.addItem(spacerItem6)
+        self.label_105 = QtWidgets.QLabel(self.tab_26)
+        font = QtGui.QFont()
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_105.setFont(font)
+        self.label_105.setObjectName("label_105")
+        self.verticalLayout_30.addWidget(self.label_105)
+        self.formLayout_32 = QtWidgets.QFormLayout()
+        self.formLayout_32.setObjectName("formLayout_32")
+        self.label_131 = QtWidgets.QLabel(self.tab_26)
+        self.label_131.setObjectName("label_131")
+        self.formLayout_32.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_131)
+        self.translation_size = QtWidgets.QDoubleSpinBox(self.tab_26)
+        self.translation_size.setDecimals(1)
+        self.translation_size.setMinimum(0.1)
+        self.translation_size.setObjectName("translation_size")
+        self.formLayout_32.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.translation_size)
+        self.label_9 = QtWidgets.QLabel(self.tab_26)
+        self.label_9.setObjectName("label_9")
+        self.formLayout_32.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_9)
+        self.translation_target = QtWidgets.QComboBox(self.tab_26)
+        self.translation_target.setObjectName("translation_target")
+        self.translation_target.addItem("")
+        self.translation_target.addItem("")
+        self.translation_target.addItem("")
+        self.formLayout_32.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.translation_target)
+        self.verticalLayout_30.addLayout(self.formLayout_32)
+        self.label_10 = QtWidgets.QLabel(self.tab_26)
+        self.label_10.setObjectName("label_10")
+        self.verticalLayout_30.addWidget(self.label_10)
+        spacerItem7 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_30.addItem(spacerItem7)
         self.tabWidget_7.addTab(self.tab_26, "")
         self.verticalLayout_27.addWidget(self.tabWidget_7)
-        spacerItem7 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_27.addItem(spacerItem7)
+        spacerItem8 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_27.addItem(spacerItem8)
         self.tabWidget.addTab(self.tab_25, "")
         self.tab_2 = QtWidgets.QWidget()
         self.tab_2.setObjectName("tab_2")
         self.verticalLayout_3 = QtWidgets.QVBoxLayout(self.tab_2)
         self.verticalLayout_3.setObjectName("verticalLayout_3")
         self.tabWidget_6 = QtWidgets.QTabWidget(self.tab_2)
         self.tabWidget_6.setObjectName("tabWidget_6")
@@ -449,16 +492,16 @@
         self.gridLayout_6.addWidget(self.picasso_fit, 0, 1, 1, 1)
         self.verticalLayout_23.addLayout(self.gridLayout_6)
         self.picasso_progressbar = QtWidgets.QProgressBar(self.tab_21)
         self.picasso_progressbar.setMaximumSize(QtCore.QSize(16777215, 10))
         self.picasso_progressbar.setProperty("value", 0)
         self.picasso_progressbar.setObjectName("picasso_progressbar")
         self.verticalLayout_23.addWidget(self.picasso_progressbar)
-        spacerItem8 = QtWidgets.QSpacerItem(20, 0, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.MinimumExpanding)
-        self.verticalLayout_23.addItem(spacerItem8)
+        spacerItem9 = QtWidgets.QSpacerItem(20, 0, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.MinimumExpanding)
+        self.verticalLayout_23.addItem(spacerItem9)
         self.tabWidget_6.addTab(self.tab_21, "")
         self.tab_23 = QtWidgets.QWidget()
         self.tab_23.setObjectName("tab_23")
         self.verticalLayout_26 = QtWidgets.QVBoxLayout(self.tab_23)
         self.verticalLayout_26.setObjectName("verticalLayout_26")
         self.label_92 = QtWidgets.QLabel(self.tab_23)
         font = QtGui.QFont()
@@ -571,16 +614,16 @@
         self.picasso_render_min_blur.setSingleStep(0.1)
         self.picasso_render_min_blur.setObjectName("picasso_render_min_blur")
         self.formLayout_20.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.picasso_render_min_blur)
         self.verticalLayout_25.addLayout(self.formLayout_20)
         self.picasso_render = QtWidgets.QPushButton(self.tab_20)
         self.picasso_render.setObjectName("picasso_render")
         self.verticalLayout_25.addWidget(self.picasso_render)
-        spacerItem9 = QtWidgets.QSpacerItem(413, 173, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_25.addItem(spacerItem9)
+        spacerItem10 = QtWidgets.QSpacerItem(413, 173, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_25.addItem(spacerItem10)
         self.tabWidget_6.addTab(self.tab_20, "")
         self.tab_27 = QtWidgets.QWidget()
         self.tab_27.setObjectName("tab_27")
         self.verticalLayout_29 = QtWidgets.QVBoxLayout(self.tab_27)
         self.verticalLayout_29.setObjectName("verticalLayout_29")
         self.label_80 = QtWidgets.QLabel(self.tab_27)
         font = QtGui.QFont()
@@ -620,16 +663,16 @@
         self.verticalLayout_29.addLayout(self.formLayout_25)
         self.remove_unlinked = QtWidgets.QCheckBox(self.tab_27)
         self.remove_unlinked.setObjectName("remove_unlinked")
         self.verticalLayout_29.addWidget(self.remove_unlinked)
         self.link_localisations = QtWidgets.QPushButton(self.tab_27)
         self.link_localisations.setObjectName("link_localisations")
         self.verticalLayout_29.addWidget(self.link_localisations)
-        spacerItem10 = QtWidgets.QSpacerItem(20, 122, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_29.addItem(spacerItem10)
+        spacerItem11 = QtWidgets.QSpacerItem(20, 122, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_29.addItem(spacerItem11)
         self.tabWidget_6.addTab(self.tab_27, "")
         self.tab_22 = QtWidgets.QWidget()
         self.tab_22.setObjectName("tab_22")
         self.verticalLayout_24 = QtWidgets.QVBoxLayout(self.tab_22)
         self.verticalLayout_24.setObjectName("verticalLayout_24")
         self.label_27 = QtWidgets.QLabel(self.tab_22)
         font = QtGui.QFont()
@@ -693,20 +736,20 @@
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.gridLayout_14.addWidget(self.picasso_vis_edge_width, 1, 3, 1, 1)
         self.verticalLayout_24.addLayout(self.gridLayout_14)
-        spacerItem11 = QtWidgets.QSpacerItem(354, 254, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_24.addItem(spacerItem11)
+        spacerItem12 = QtWidgets.QSpacerItem(354, 254, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_24.addItem(spacerItem12)
         self.tabWidget_6.addTab(self.tab_22, "")
         self.verticalLayout_3.addWidget(self.tabWidget_6)
-        spacerItem12 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_3.addItem(spacerItem12)
+        spacerItem13 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_3.addItem(spacerItem13)
         self.tabWidget.addTab(self.tab_2, "")
         self.tab_6 = QtWidgets.QWidget()
         self.tab_6.setObjectName("tab_6")
         self.verticalLayout_11 = QtWidgets.QVBoxLayout(self.tab_6)
         self.verticalLayout_11.setObjectName("verticalLayout_11")
         self.label_74 = QtWidgets.QLabel(self.tab_6)
         self.label_74.setObjectName("label_74")
@@ -733,16 +776,16 @@
         self.export_localisations.setObjectName("export_localisations")
         self.verticalLayout_11.addWidget(self.export_localisations)
         self.export_progressbar = QtWidgets.QProgressBar(self.tab_6)
         self.export_progressbar.setMaximumSize(QtCore.QSize(16777215, 10))
         self.export_progressbar.setProperty("value", 0)
         self.export_progressbar.setObjectName("export_progressbar")
         self.verticalLayout_11.addWidget(self.export_progressbar)
-        spacerItem13 = QtWidgets.QSpacerItem(354, 414, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_11.addItem(spacerItem13)
+        spacerItem14 = QtWidgets.QSpacerItem(354, 414, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_11.addItem(spacerItem14)
         self.tabWidget.addTab(self.tab_6, "")
         self.verticalLayout.addWidget(self.tabWidget)
         self.label_12 = QtWidgets.QLabel(Frame)
         font = QtGui.QFont()
         font.setBold(True)
         font.setWeight(75)
         self.label_12.setFont(font)
@@ -782,17 +825,21 @@
         self.import_limit.setItemText(1, _translate("Frame", "10"))
         self.import_limit.setItemText(2, _translate("Frame", "50"))
         self.import_limit.setItemText(3, _translate("Frame", "100"))
         self.import_limit.setItemText(4, _translate("Frame", "200"))
         self.import_limit.setItemText(5, _translate("Frame", "300"))
         self.import_limit.setItemText(6, _translate("Frame", "400"))
         self.import_limit.setItemText(7, _translate("Frame", "500"))
+        self.label_6.setText(_translate("Frame", "Import Mode"))
+        self.import_mode.setItemText(0, _translate("Frame", "Data"))
+        self.import_mode.setItemText(1, _translate("Frame", "Segmentation Image"))
         self.import_concatenate.setText(_translate("Frame", "Concatenate Imported Files"))
+        self.frame_averaging.setText(_translate("Frame", "Frame Averaging"))
         self.import_images.setText(_translate("Frame", "Import"))
-        self.tabWidget_4.setTabText(self.tabWidget_4.indexOf(self.tab_15), _translate("Frame", "Import Images"))
+        self.tabWidget_4.setTabText(self.tabWidget_4.indexOf(self.tab_15), _translate("Frame", "Import Data"))
         self.label_76.setText(_translate("Frame", "Localisation Type"))
         self.import_picasso_type.setItemText(0, _translate("Frame", "Localisations"))
         self.import_picasso_type.setItemText(1, _translate("Frame", "Bounding Boxes"))
         self.label_2.setText(_translate("Frame", "Dataset"))
         self.import_picasso.setText(_translate("Frame", "Import Picasso Localisations"))
         self.tabWidget_4.setTabText(self.tabWidget_4.indexOf(self.tab_16), _translate("Frame", "Import Localisations"))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab), _translate("Frame", "Import"))
@@ -843,14 +890,21 @@
         self.cellpose_load_model.setText(_translate("Frame", "Load Custom Model"))
         self.segment_all.setText(_translate("Frame", "Segment All Images"))
         self.segment_active.setText(_translate("Frame", "Segment Active Image"))
         self.tabWidget_7.setTabText(self.tabWidget_7.indexOf(self.tab_24), _translate("Frame", "Cellpose"))
         self.label_103.setText(_translate("Frame", "Dilate Segmentations"))
         self.label_111.setText(_translate("Frame", "Pixels"))
         self.dilate_segmentations.setText(_translate("Frame", "Dilate Segmentations"))
+        self.label_105.setText(_translate("Frame", "Translate Segmentations"))
+        self.label_131.setText(_translate("Frame", "Translation Size (Pixels)"))
+        self.label_9.setText(_translate("Frame", "Translation Target"))
+        self.translation_target.setItemText(0, _translate("Frame", "Segmentation Image"))
+        self.translation_target.setItemText(1, _translate("Frame", "Segmentations"))
+        self.translation_target.setItemText(2, _translate("Frame", "Both"))
+        self.label_10.setText(_translate("Frame", "Press [Control] + [Arrow Key] to move translation target by translation size"))
         self.tabWidget_7.setTabText(self.tabWidget_7.indexOf(self.tab_26), _translate("Frame", "Curate"))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_25), _translate("Frame", "Segment"))
         self.label_3.setText(_translate("Frame", "Detect Localisations"))
         self.label_7.setText(_translate("Frame", "Detect Mode"))
         self.smlm_detect_mode.setItemText(0, _translate("Frame", "Picasso"))
         self.smlm_detect_mode.setItemText(1, _translate("Frame", "StormTracker"))
         self.label_11.setText(_translate("Frame", "Dataset"))
```

### Comparing `napari_moltrack-0.0.3/src/moltrack/_tests/test_widget.py` & `napari_moltrack-0.0.4/src/moltrack/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.3/src/moltrack/_widget.py` & `napari_moltrack-0.0.4/src/moltrack/_widget.py`

 * *Files 12% similar despite different names*

```diff
@@ -113,20 +113,23 @@
         self.viewer.dims.events.current_step.connect(self.slider_event)
 
     def initialise_keybindings(self):
 
 
         self.viewer.bind_key('d', self.devfunc)
 
-        pass
+        self.viewer.bind_key(key='Control-Right', func=lambda event: self.moltract_translation(direction="right"), overwrite=True)
+        self.viewer.bind_key(key='Control-Left', func=lambda event: self.moltract_translation(direction="left"), overwrite=True)
+        self.viewer.bind_key(key='Control-Up', func=lambda event: self.moltract_translation(direction="up"), overwrite=True)
+        self.viewer.bind_key(key='Control-Down', func=lambda event: self.moltract_translation(direction="down"), overwrite=True)
+
 
     def devfunc(self, viewer=None):
 
-        self.create_shared_image_chunks()
-        self.restore_shared_image_chunks()
+        self.update_ui()
 
     def check_gpufit_availibility(self):
 
         self.gpufit_available = False
 
         try:
             from pygpufit import gpufit as gf
```

### Comparing `napari_moltrack-0.0.3/src/moltrack/funcs/compute_utils.py` & `napari_moltrack-0.0.4/src/moltrack/funcs/compute_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.3/src/moltrack/funcs/events_utils.py` & `napari_moltrack-0.0.4/src/moltrack/funcs/events_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,827 +6,981 @@
 00000050: 7274 6961 6c2c 2077 7261 7073 0d0a 6672  rtial, wraps..fr
 00000060: 6f6d 2071 7470 792e 5174 5769 6467 6574  om qtpy.QtWidget
 00000070: 7320 696d 706f 7274 2028 5153 6c69 6465  s import (QSlide
 00000080: 722c 2051 4c61 6265 6c29 0d0a 696d 706f  r, QLabel)..impo
 00000090: 7274 2074 696d 650d 0a66 726f 6d20 6e61  rt time..from na
 000000a0: 7061 7269 2e75 7469 6c73 2e6e 6f74 6966  pari.utils.notif
 000000b0: 6963 6174 696f 6e73 2069 6d70 6f72 7420  ications import 
-000000c0: 7368 6f77 5f69 6e66 6f0d 0a0d 0a63 6c61  show_info....cla
-000000d0: 7373 205f 6576 656e 7473 5f75 7469 6c73  ss _events_utils
-000000e0: 3a0d 0a0d 0a20 2020 2064 6566 206d 6f6c  :....    def mol
-000000f0: 7472 6163 6b5f 7072 6f67 7265 7373 2873  track_progress(s
-00000100: 656c 662c 2070 726f 6772 6573 732c 2070  elf, progress, p
-00000110: 726f 6772 6573 735f 6261 7229 3a0d 0a0d  rogress_bar):...
-00000120: 0a20 2020 2020 2020 2070 726f 6772 6573  .        progres
-00000130: 735f 6261 722e 7365 7456 616c 7565 2870  s_bar.setValue(p
-00000140: 726f 6772 6573 7329 0d0a 0d0a 2020 2020  rogress)....    
-00000150: 2020 2020 6966 2070 726f 6772 6573 7320      if progress 
-00000160: 3d3d 2031 3030 3a0d 0a20 2020 2020 2020  == 100:..       
-00000170: 2020 2020 2070 726f 6772 6573 735f 6261       progress_ba
-00000180: 722e 7365 7456 616c 7565 2830 290d 0a20  r.setValue(0).. 
-00000190: 2020 2020 2020 2020 2020 2070 726f 6772             progr
-000001a0: 6573 735f 6261 722e 7365 7448 6964 6465  ess_bar.setHidde
-000001b0: 6e28 5472 7565 290d 0a20 2020 2020 2020  n(True)..       
-000001c0: 2020 2020 2070 726f 6772 6573 735f 6261       progress_ba
-000001d0: 722e 7365 7445 6e61 626c 6564 2846 616c  r.setEnabled(Fal
-000001e0: 7365 290d 0a20 2020 2020 2020 2065 6c73  se)..        els
-000001f0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00000200: 7072 6f67 7265 7373 5f62 6172 2e73 6574  progress_bar.set
-00000210: 4869 6464 656e 2846 616c 7365 290d 0a20  Hidden(False).. 
-00000220: 2020 2020 2020 2020 2020 2070 726f 6772             progr
-00000230: 6573 735f 6261 722e 7365 7445 6e61 626c  ess_bar.setEnabl
-00000240: 6564 2854 7275 6529 0d0a 0d0a 2020 2020  ed(True)....    
-00000250: 6465 6620 6d6f 6c74 7261 636b 5f6e 6f74  def moltrack_not
-00000260: 6966 6963 6174 696f 6e28 7365 6c66 2c20  ification(self, 
-00000270: 6d65 7373 6167 6529 3a0d 0a20 2020 2020  message):..     
-00000280: 2020 2073 686f 775f 696e 666f 286d 6573     show_info(mes
-00000290: 7361 6765 290d 0a0d 0a20 2020 2064 6566  sage)....    def
-000002a0: 2075 7064 6174 655f 7569 2873 656c 662c   update_ui(self,
-000002b0: 2065 7272 6f72 3d4e 6f6e 652c 2069 6e69   error=None, ini
-000002c0: 7420 3d20 4661 6c73 6529 3a0d 0a0d 0a20  t = False):.... 
-000002d0: 2020 2020 2020 2074 7279 3a0d 0a0d 0a20         try:.... 
-000002e0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-000002f0: 6c66 2e76 6572 626f 7365 3a0d 0a20 2020  lf.verbose:..   
-00000300: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00000310: 6e74 2866 2255 7064 6174 696e 6720 5549  nt(f"Updating UI
-00000320: 2c20 696e 6974 203d 207b 696e 6974 7d22  , init = {init}"
-00000330: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00000340: 2063 6f6e 7472 6f6c 7320 3d20 5b22 696d   controls = ["im
-00000350: 706f 7274 5f69 6d61 6765 7322 2c0d 0a20  port_images",.. 
-00000360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000370: 2020 2020 2020 2022 696d 706f 7274 5f70         "import_p
-00000380: 6963 6173 736f 222c 0d0a 2020 2020 2020  icasso",..      
+000000c0: 7368 6f77 5f69 6e66 6f0d 0a69 6d70 6f72  show_info..impor
+000000d0: 7420 6e61 7061 7269 0d0a 6672 6f6d 2073  t napari..from s
+000000e0: 6369 7079 2e6e 6469 6d61 6765 2069 6d70  cipy.ndimage imp
+000000f0: 6f72 7420 7368 6966 740d 0a0d 0a63 6c61  ort shift....cla
+00000100: 7373 205f 6576 656e 7473 5f75 7469 6c73  ss _events_utils
+00000110: 3a0d 0a0d 0a20 2020 2064 6566 206d 6f6c  :....    def mol
+00000120: 7472 6163 6b5f 7072 6f67 7265 7373 2873  track_progress(s
+00000130: 656c 662c 2070 726f 6772 6573 732c 2070  elf, progress, p
+00000140: 726f 6772 6573 735f 6261 7229 3a0d 0a0d  rogress_bar):...
+00000150: 0a20 2020 2020 2020 2070 726f 6772 6573  .        progres
+00000160: 735f 6261 722e 7365 7456 616c 7565 2870  s_bar.setValue(p
+00000170: 726f 6772 6573 7329 0d0a 0d0a 2020 2020  rogress)....    
+00000180: 2020 2020 6966 2070 726f 6772 6573 7320      if progress 
+00000190: 3d3d 2031 3030 3a0d 0a20 2020 2020 2020  == 100:..       
+000001a0: 2020 2020 2070 726f 6772 6573 735f 6261       progress_ba
+000001b0: 722e 7365 7456 616c 7565 2830 290d 0a20  r.setValue(0).. 
+000001c0: 2020 2020 2020 2020 2020 2070 726f 6772             progr
+000001d0: 6573 735f 6261 722e 7365 7448 6964 6465  ess_bar.setHidde
+000001e0: 6e28 5472 7565 290d 0a20 2020 2020 2020  n(True)..       
+000001f0: 2020 2020 2070 726f 6772 6573 735f 6261       progress_ba
+00000200: 722e 7365 7445 6e61 626c 6564 2846 616c  r.setEnabled(Fal
+00000210: 7365 290d 0a20 2020 2020 2020 2065 6c73  se)..        els
+00000220: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00000230: 7072 6f67 7265 7373 5f62 6172 2e73 6574  progress_bar.set
+00000240: 4869 6464 656e 2846 616c 7365 290d 0a20  Hidden(False).. 
+00000250: 2020 2020 2020 2020 2020 2070 726f 6772             progr
+00000260: 6573 735f 6261 722e 7365 7445 6e61 626c  ess_bar.setEnabl
+00000270: 6564 2854 7275 6529 0d0a 0d0a 2020 2020  ed(True)....    
+00000280: 6465 6620 6d6f 6c74 7261 636b 5f6e 6f74  def moltrack_not
+00000290: 6966 6963 6174 696f 6e28 7365 6c66 2c20  ification(self, 
+000002a0: 6d65 7373 6167 6529 3a0d 0a20 2020 2020  message):..     
+000002b0: 2020 2073 686f 775f 696e 666f 286d 6573     show_info(mes
+000002c0: 7361 6765 290d 0a0d 0a20 2020 2064 6566  sage)....    def
+000002d0: 2075 7064 6174 655f 7569 2873 656c 662c   update_ui(self,
+000002e0: 2065 7272 6f72 3d4e 6f6e 652c 2069 6e69   error=None, ini
+000002f0: 7420 3d20 4661 6c73 6529 3a0d 0a0d 0a20  t = False):.... 
+00000300: 2020 2020 2020 2074 7279 3a0d 0a0d 0a20         try:.... 
+00000310: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00000320: 6c66 2e76 6572 626f 7365 3a0d 0a20 2020  lf.verbose:..   
+00000330: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+00000340: 6e74 2866 2255 7064 6174 696e 6720 5549  nt(f"Updating UI
+00000350: 2c20 696e 6974 203d 207b 696e 6974 7d22  , init = {init}"
+00000360: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00000370: 2063 6f6e 7472 6f6c 7320 3d20 5b22 696d   controls = ["im
+00000380: 706f 7274 5f69 6d61 6765 7322 2c0d 0a20  port_images",.. 
 00000390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003a0: 2020 2263 656c 6c70 6f73 655f 6c6f 6164    "cellpose_load
-000003b0: 5f6d 6f64 656c 222c 0d0a 2020 2020 2020  _model",..      
+000003a0: 2020 2020 2020 2022 696d 706f 7274 5f70         "import_p
+000003b0: 6963 6173 736f 222c 0d0a 2020 2020 2020  icasso",..      
 000003c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003d0: 2020 2273 6567 6d65 6e74 5f61 6374 6976    "segment_activ
-000003e0: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
-000003f0: 2020 2020 2020 2020 2020 2020 2022 7365               "se
-00000400: 676d 656e 745f 616c 6c22 2c0d 0a20 2020  gment_all",..   
-00000410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000420: 2020 2020 2022 6469 6c61 7465 5f73 6567       "dilate_seg
-00000430: 6d65 6e74 6174 696f 6e73 222c 0d0a 2020  mentations",..  
+000003d0: 2020 2263 656c 6c70 6f73 655f 6c6f 6164    "cellpose_load
+000003e0: 5f6d 6f64 656c 222c 0d0a 2020 2020 2020  _model",..      
+000003f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000400: 2020 2273 6567 6d65 6e74 5f61 6374 6976    "segment_activ
+00000410: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
+00000420: 2020 2020 2020 2020 2020 2020 2022 7365               "se
+00000430: 676d 656e 745f 616c 6c22 2c0d 0a20 2020  gment_all",..   
 00000440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000450: 2020 2020 2020 2270 6963 6173 736f 5f64        "picasso_d
-00000460: 6574 6563 7422 2c0d 0a20 2020 2020 2020  etect",..       
+00000450: 2020 2020 2022 6469 6c61 7465 5f73 6567       "dilate_seg
+00000460: 6d65 6e74 6174 696f 6e73 222c 0d0a 2020  mentations",..  
 00000470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000480: 2022 7069 6361 7373 6f5f 6669 7422 2c0d   "picasso_fit",.
-00000490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000004a0: 2020 2020 2020 2020 2022 7069 6361 7373           "picass
-000004b0: 6f5f 6465 7465 6374 6669 7422 2c0d 0a20  o_detectfit",.. 
-000004c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000004d0: 2020 2020 2020 2022 6669 6c74 6572 5f6c         "filter_l
-000004e0: 6f63 616c 6973 6174 696f 6e73 222c 0d0a  ocalisations",..
+00000480: 2020 2020 2020 2270 6963 6173 736f 5f64        "picasso_d
+00000490: 6574 6563 7422 2c0d 0a20 2020 2020 2020  etect",..       
+000004a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000004b0: 2022 7069 6361 7373 6f5f 6669 7422 2c0d   "picasso_fit",.
+000004c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000004d0: 2020 2020 2020 2020 2022 7069 6361 7373           "picass
+000004e0: 6f5f 6465 7465 6374 6669 7422 2c0d 0a20  o_detectfit",.. 
 000004f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000500: 2020 2020 2020 2020 2270 6963 6173 736f          "picasso
-00000510: 5f72 656e 6465 7222 2c0d 0a20 2020 2020  _render",..     
+00000500: 2020 2020 2020 2022 6669 6c74 6572 5f6c         "filter_l
+00000510: 6f63 616c 6973 6174 696f 6e73 222c 0d0a  ocalisations",..
 00000520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000530: 2020 2022 6c69 6e6b 5f6c 6f63 616c 6973     "link_localis
-00000540: 6174 696f 6e73 222c 0d0a 2020 2020 2020  ations",..      
+00000530: 2020 2020 2020 2020 2270 6963 6173 736f          "picasso
+00000540: 5f72 656e 6465 7222 2c0d 0a20 2020 2020  _render",..     
 00000550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000560: 2020 2265 7870 6f72 745f 6c6f 6361 6c69    "export_locali
-00000570: 7361 7469 6f6e 7322 2c0d 0a20 2020 2020  sations",..     
+00000560: 2020 2022 6c69 6e6b 5f6c 6f63 616c 6973     "link_localis
+00000570: 6174 696f 6e73 222c 0d0a 2020 2020 2020  ations",..      
 00000580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000590: 2020 205d 0d0a 0d0a 2020 2020 2020 2020     ]....        
-000005a0: 2020 2020 7072 6f67 7265 7373 6261 7273      progressbars
-000005b0: 203d 205b 2269 6d70 6f72 745f 7072 6f67   = ["import_prog
-000005c0: 7265 7373 6261 7222 2c0d 0a20 2020 2020  ressbar",..     
-000005d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005e0: 2020 2020 2020 2022 6365 6c6c 706f 7365         "cellpose
-000005f0: 5f70 726f 6772 6573 7362 6172 222c 0d0a  _progressbar",..
+00000590: 2020 2265 7870 6f72 745f 6c6f 6361 6c69    "export_locali
+000005a0: 7361 7469 6f6e 7322 2c0d 0a20 2020 2020  sations",..     
+000005b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005c0: 2020 205d 0d0a 0d0a 2020 2020 2020 2020     ]....        
+000005d0: 2020 2020 7072 6f67 7265 7373 6261 7273      progressbars
+000005e0: 203d 205b 2269 6d70 6f72 745f 7072 6f67   = ["import_prog
+000005f0: 7265 7373 6261 7222 2c0d 0a20 2020 2020  ressbar",..     
 00000600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000610: 2020 2020 2020 2020 2020 2020 2270 6963              "pic
-00000620: 6173 736f 5f70 726f 6772 6573 7362 6172  asso_progressbar
-00000630: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000650: 2265 7870 6f72 745f 7072 6f67 7265 7373  "export_progress
-00000660: 6261 7222 2c0d 0a20 2020 2020 2020 2020  bar",..         
+00000610: 2020 2020 2020 2022 6365 6c6c 706f 7365         "cellpose
+00000620: 5f70 726f 6772 6573 7362 6172 222c 0d0a  _progressbar",..
+00000630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000640: 2020 2020 2020 2020 2020 2020 2270 6963              "pic
+00000650: 6173 736f 5f70 726f 6772 6573 7362 6172  asso_progressbar
+00000660: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
 00000670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000680: 2020 205d 0d0a 0d0a 2020 2020 2020 2020     ]....        
-00000690: 2020 2020 666f 7220 7072 6f67 7265 7373      for progress
-000006a0: 6261 7220 696e 2070 726f 6772 6573 7362  bar in progressb
-000006b0: 6172 733a 0d0a 2020 2020 2020 2020 2020  ars:..          
-000006c0: 2020 2020 2020 6966 2068 6173 6174 7472        if hasattr
-000006d0: 2873 656c 662e 6775 692c 2070 726f 6772  (self.gui, progr
-000006e0: 6573 7362 6172 293a 0d0a 2020 2020 2020  essbar):..      
-000006f0: 2020 2020 2020 2020 2020 2020 2020 6765                ge
-00000700: 7461 7474 7228 7365 6c66 2e67 7569 2c20  tattr(self.gui, 
-00000710: 7072 6f67 7265 7373 6261 7229 2e73 6574  progressbar).set
-00000720: 5661 6c75 6528 3029 0d0a 0d0a 2020 2020  Value(0)....    
-00000730: 2020 2020 2020 2020 6966 2069 6e69 7420          if init 
-00000740: 6973 2054 7275 653a 0d0a 0d0a 2020 2020  is True:....    
-00000750: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00000760: 636f 6e74 726f 6c20 696e 2063 6f6e 7472  control in contr
-00000770: 6f6c 733a 0d0a 2020 2020 2020 2020 2020  ols:..          
-00000780: 2020 2020 2020 2020 2020 6765 7461 7474            getatt
-00000790: 7228 7365 6c66 2e67 7569 2c20 636f 6e74  r(self.gui, cont
-000007a0: 726f 6c29 2e73 6574 456e 6162 6c65 6428  rol).setEnabled(
-000007b0: 4661 6c73 6529 0d0a 0d0a 2020 2020 2020  False)....      
-000007c0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-000007d0: 746f 705f 6576 656e 742e 636c 6561 7228  top_event.clear(
-000007e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000007f0: 2020 2073 656c 662e 6d75 6c74 6970 726f     self.multipro
-00000800: 6365 7373 696e 675f 6163 7469 7665 203d  cessing_active =
-00000810: 2054 7275 650d 0a0d 0a20 2020 2020 2020   True....       
-00000820: 2020 2020 2065 6c73 653a 0d0a 0d0a 2020       else:....  
-00000830: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00000840: 7220 636f 6e74 726f 6c20 696e 2063 6f6e  r control in con
-00000850: 7472 6f6c 733a 0d0a 2020 2020 2020 2020  trols:..        
-00000860: 2020 2020 2020 2020 2020 2020 6765 7461              geta
-00000870: 7474 7228 7365 6c66 2e67 7569 2c20 636f  ttr(self.gui, co
-00000880: 6e74 726f 6c29 2e73 6574 456e 6162 6c65  ntrol).setEnable
-00000890: 6428 5472 7565 290d 0a0d 0a20 2020 2020  d(True)....     
-000008a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000008b0: 6d75 6c74 6970 726f 6365 7373 696e 675f  multiprocessing_
-000008c0: 6163 7469 7665 203d 2046 616c 7365 0d0a  active = False..
-000008d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000008e0: 2020 7365 6c66 2e73 746f 705f 6576 656e    self.stop_even
-000008f0: 742e 636c 6561 7228 290d 0a20 2020 2020  t.clear()..     
-00000900: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00000910: 6d75 6c74 6970 726f 6365 7373 696e 675f  multiprocessing_
-00000920: 6163 7469 7665 203d 2046 616c 7365 0d0a  active = False..
-00000930: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00000940: 2065 7272 6f72 2069 7320 6e6f 7420 4e6f   error is not No
-00000950: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00000960: 2020 2020 2070 7269 6e74 2865 7272 6f72       print(error
-00000970: 290d 0a0d 0a20 2020 2020 2020 2065 7863  )....        exc
-00000980: 6570 743a 0d0a 2020 2020 2020 2020 2020  ept:..          
-00000990: 2020 7072 696e 7428 7472 6163 6562 6163    print(tracebac
-000009a0: 6b2e 666f 726d 6174 5f65 7863 2829 290d  k.format_exc()).
-000009b0: 0a20 2020 2020 2020 2020 2020 2070 6173  .            pas
-000009c0: 730d 0a0d 0a0d 0a0d 0a20 2020 2064 6566  s........    def
-000009d0: 2069 6d61 6765 5f6c 6179 6572 5f61 7574   image_layer_aut
-000009e0: 6f5f 636f 6e74 7261 7374 2873 656c 662c  o_contrast(self,
-000009f0: 2069 6d61 6765 2c20 6461 7461 7365 7429   image, dataset)
-00000a00: 3a0d 0a0d 0a20 2020 2020 2020 2063 6f6e  :....        con
-00000a10: 7472 6173 745f 6c69 6d69 7473 203d 204e  trast_limits = N
-00000a20: 6f6e 650d 0a0d 0a20 2020 2020 2020 2074  one....        t
-00000a30: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
-00000a40: 2061 7574 6f63 6f6e 7472 6173 7420 3d20   autocontrast = 
-00000a50: 5472 7565 0d0a 0d0a 2020 2020 2020 2020  True....        
-00000a60: 2020 2020 6966 2064 6174 6173 6574 2069      if dataset i
-00000a70: 6e20 7365 6c66 2e63 6f6e 7472 6173 745f  n self.contrast_
-00000a80: 6469 6374 2e6b 6579 7328 293a 0d0a 0d0a  dict.keys():....
-00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000aa0: 6175 746f 636f 6e74 7261 7374 203d 2046  autocontrast = F
-00000ab0: 616c 7365 0d0a 0d0a 2020 2020 2020 2020  alse....        
-00000ac0: 2020 2020 2020 2020 636f 6e74 7261 7374          contrast
-00000ad0: 5f6c 696d 6974 7320 3d20 7365 6c66 2e63  _limits = self.c
-00000ae0: 6f6e 7472 6173 745f 6469 6374 5b64 6174  ontrast_dict[dat
-00000af0: 6173 6574 5d5b 2263 6f6e 7472 6173 745f  aset]["contrast_
-00000b00: 6c69 6d69 7473 225d 0d0a 2020 2020 2020  limits"]..      
-00000b10: 2020 2020 2020 2020 2020 6761 6d6d 6120            gamma 
-00000b20: 3d20 7365 6c66 2e63 6f6e 7472 6173 745f  = self.contrast_
-00000b30: 6469 6374 5b64 6174 6173 6574 5d5b 2267  dict[dataset]["g
-00000b40: 616d 6d61 225d 0d0a 0d0a 2020 2020 2020  amma"]....      
-00000b50: 2020 2020 2020 2020 2020 6966 2068 6173            if has
-00000b60: 6174 7472 2873 656c 662c 2022 696d 6167  attr(self, "imag
-00000b70: 655f 6c61 7965 7222 293a 0d0a 2020 2020  e_layer"):..    
-00000b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b90: 7365 6c66 2e69 6d61 6765 5f6c 6179 6572  self.image_layer
-00000ba0: 2e67 616d 6d61 203d 2067 616d 6d61 0d0a  .gamma = gamma..
+00000680: 2265 7870 6f72 745f 7072 6f67 7265 7373  "export_progress
+00000690: 6261 7222 2c0d 0a20 2020 2020 2020 2020  bar",..         
+000006a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006b0: 2020 205d 0d0a 0d0a 2020 2020 2020 2020     ]....        
+000006c0: 2020 2020 666f 7220 7072 6f67 7265 7373      for progress
+000006d0: 6261 7220 696e 2070 726f 6772 6573 7362  bar in progressb
+000006e0: 6172 733a 0d0a 2020 2020 2020 2020 2020  ars:..          
+000006f0: 2020 2020 2020 6966 2068 6173 6174 7472        if hasattr
+00000700: 2873 656c 662e 6775 692c 2070 726f 6772  (self.gui, progr
+00000710: 6573 7362 6172 293a 0d0a 2020 2020 2020  essbar):..      
+00000720: 2020 2020 2020 2020 2020 2020 2020 6765                ge
+00000730: 7461 7474 7228 7365 6c66 2e67 7569 2c20  tattr(self.gui, 
+00000740: 7072 6f67 7265 7373 6261 7229 2e73 6574  progressbar).set
+00000750: 5661 6c75 6528 3029 0d0a 0d0a 2020 2020  Value(0)....    
+00000760: 2020 2020 2020 2020 6966 2069 6e69 7420          if init 
+00000770: 6973 2054 7275 653a 0d0a 0d0a 2020 2020  is True:....    
+00000780: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00000790: 636f 6e74 726f 6c20 696e 2063 6f6e 7472  control in contr
+000007a0: 6f6c 733a 0d0a 2020 2020 2020 2020 2020  ols:..          
+000007b0: 2020 2020 2020 2020 2020 6765 7461 7474            getatt
+000007c0: 7228 7365 6c66 2e67 7569 2c20 636f 6e74  r(self.gui, cont
+000007d0: 726f 6c29 2e73 6574 456e 6162 6c65 6428  rol).setEnabled(
+000007e0: 4661 6c73 6529 0d0a 0d0a 2020 2020 2020  False)....      
+000007f0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00000800: 746f 705f 6576 656e 742e 636c 6561 7228  top_event.clear(
+00000810: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00000820: 2020 2073 656c 662e 6d75 6c74 6970 726f     self.multipro
+00000830: 6365 7373 696e 675f 6163 7469 7665 203d  cessing_active =
+00000840: 2054 7275 650d 0a0d 0a20 2020 2020 2020   True....       
+00000850: 2020 2020 2065 6c73 653a 0d0a 0d0a 2020       else:....  
+00000860: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00000870: 7220 636f 6e74 726f 6c20 696e 2063 6f6e  r control in con
+00000880: 7472 6f6c 733a 0d0a 2020 2020 2020 2020  trols:..        
+00000890: 2020 2020 2020 2020 2020 2020 6765 7461              geta
+000008a0: 7474 7228 7365 6c66 2e67 7569 2c20 636f  ttr(self.gui, co
+000008b0: 6e74 726f 6c29 2e73 6574 456e 6162 6c65  ntrol).setEnable
+000008c0: 6428 5472 7565 290d 0a0d 0a20 2020 2020  d(True)....     
+000008d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000008e0: 6d75 6c74 6970 726f 6365 7373 696e 675f  multiprocessing_
+000008f0: 6163 7469 7665 203d 2046 616c 7365 0d0a  active = False..
+00000900: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000910: 2020 7365 6c66 2e73 746f 705f 6576 656e    self.stop_even
+00000920: 742e 636c 6561 7228 290d 0a20 2020 2020  t.clear()..     
+00000930: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00000940: 6d75 6c74 6970 726f 6365 7373 696e 675f  multiprocessing_
+00000950: 6163 7469 7665 203d 2046 616c 7365 0d0a  active = False..
+00000960: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00000970: 2065 7272 6f72 2069 7320 6e6f 7420 4e6f   error is not No
+00000980: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00000990: 2020 2020 2070 7269 6e74 2865 7272 6f72       print(error
+000009a0: 290d 0a0d 0a20 2020 2020 2020 2065 7863  )....        exc
+000009b0: 6570 743a 0d0a 2020 2020 2020 2020 2020  ept:..          
+000009c0: 2020 7072 696e 7428 7472 6163 6562 6163    print(tracebac
+000009d0: 6b2e 666f 726d 6174 5f65 7863 2829 290d  k.format_exc()).
+000009e0: 0a20 2020 2020 2020 2020 2020 2070 6173  .            pas
+000009f0: 730d 0a0d 0a0d 0a0d 0a20 2020 2064 6566  s........    def
+00000a00: 2069 6d61 6765 5f6c 6179 6572 5f61 7574   image_layer_aut
+00000a10: 6f5f 636f 6e74 7261 7374 2873 656c 662c  o_contrast(self,
+00000a20: 2069 6d61 6765 2c20 6461 7461 7365 7429   image, dataset)
+00000a30: 3a0d 0a0d 0a20 2020 2020 2020 2063 6f6e  :....        con
+00000a40: 7472 6173 745f 6c69 6d69 7473 203d 204e  trast_limits = N
+00000a50: 6f6e 650d 0a0d 0a20 2020 2020 2020 2074  one....        t
+00000a60: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+00000a70: 2061 7574 6f63 6f6e 7472 6173 7420 3d20   autocontrast = 
+00000a80: 5472 7565 0d0a 0d0a 2020 2020 2020 2020  True....        
+00000a90: 2020 2020 6966 2064 6174 6173 6574 2069      if dataset i
+00000aa0: 6e20 7365 6c66 2e63 6f6e 7472 6173 745f  n self.contrast_
+00000ab0: 6469 6374 2e6b 6579 7328 293a 0d0a 0d0a  dict.keys():....
+00000ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ad0: 6175 746f 636f 6e74 7261 7374 203d 2046  autocontrast = F
+00000ae0: 616c 7365 0d0a 0d0a 2020 2020 2020 2020  alse....        
+00000af0: 2020 2020 2020 2020 636f 6e74 7261 7374          contrast
+00000b00: 5f6c 696d 6974 7320 3d20 7365 6c66 2e63  _limits = self.c
+00000b10: 6f6e 7472 6173 745f 6469 6374 5b64 6174  ontrast_dict[dat
+00000b20: 6173 6574 5d5b 2263 6f6e 7472 6173 745f  aset]["contrast_
+00000b30: 6c69 6d69 7473 225d 0d0a 2020 2020 2020  limits"]..      
+00000b40: 2020 2020 2020 2020 2020 6761 6d6d 6120            gamma 
+00000b50: 3d20 7365 6c66 2e63 6f6e 7472 6173 745f  = self.contrast_
+00000b60: 6469 6374 5b64 6174 6173 6574 5d5b 2267  dict[dataset]["g
+00000b70: 616d 6d61 225d 0d0a 0d0a 2020 2020 2020  amma"]....      
+00000b80: 2020 2020 2020 2020 2020 6966 2068 6173            if has
+00000b90: 6174 7472 2873 656c 662c 2022 696d 6167  attr(self, "imag
+00000ba0: 655f 6c61 7965 7222 293a 0d0a 2020 2020  e_layer"):..    
 00000bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bc0: 2020 2020 7365 6c66 2e69 6d61 6765 5f6c      self.image_l
-00000bd0: 6179 6572 2e63 6f6e 7472 6173 745f 6c69  ayer.contrast_li
-00000be0: 6d69 7473 203d 2063 6f6e 7472 6173 745f  mits = contrast_
-00000bf0: 6c69 6d69 7473 0d0a 0d0a 2020 2020 2020  limits....      
-00000c00: 2020 2020 2020 6966 2061 7574 6f63 6f6e        if autocon
-00000c10: 7472 6173 7420 6973 2054 7275 653a 0d0a  trast is True:..
-00000c20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000c30: 2020 6675 6c6c 5f72 616e 6765 203d 205b    full_range = [
-00000c40: 6e70 2e6d 696e 2869 6d61 6765 292c 206e  np.min(image), n
-00000c50: 702e 6d61 7828 696d 6167 6529 5d0d 0a0d  p.max(image)]...
-00000c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c70: 2069 6620 6d61 7828 6675 6c6c 5f72 616e   if max(full_ran
-00000c80: 6765 2920 3e20 6d69 6e28 6675 6c6c 5f72  ge) > min(full_r
-00000c90: 616e 6765 293a 0d0a 2020 2020 2020 2020  ange):..        
-00000ca0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00000cb0: 7261 7374 5f6c 696d 6974 7320 3d20 6e70  rast_limits = np
-00000cc0: 2e70 6572 6365 6e74 696c 6528 696d 6167  .percentile(imag
-00000cd0: 655b 3a31 305d 2e63 6f70 7928 292c 205b  e[:10].copy(), [
-00000ce0: 302e 312c 2039 392e 3939 5d29 0d0a 0d0a  0.1, 99.99])....
-00000cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d00: 2020 2020 6761 6d6d 6120 3d20 312e 300d      gamma = 1.0.
-00000d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000d20: 2020 2020 2069 6620 636f 6e74 7261 7374       if contrast
-00000d30: 5f6c 696d 6974 735b 315d 203e 2063 6f6e  _limits[1] > con
-00000d40: 7472 6173 745f 6c69 6d69 7473 5b30 5d3a  trast_limits[0]:
-00000d50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000d60: 2020 2020 2020 2020 2020 6761 6d6d 6120            gamma 
-00000d70: 3d20 6e70 2e6c 6f67 2830 2e35 2920 2f20  = np.log(0.5) / 
-00000d80: 6e70 2e6c 6f67 2828 636f 6e74 7261 7374  np.log((contrast
-00000d90: 5f6c 696d 6974 735b 315d 202d 2063 6f6e  _limits[1] - con
-00000da0: 7472 6173 745f 6c69 6d69 7473 5b30 5d29  trast_limits[0])
-00000db0: 202f 2028 6675 6c6c 5f72 616e 6765 5b31   / (full_range[1
-00000dc0: 5d20 2d20 6675 6c6c 5f72 616e 6765 5b30  ] - full_range[0
-00000dd0: 5d29 290d 0a0d 0a20 2020 2020 2020 2020  ]))....         
-00000de0: 2020 2020 2020 2020 2020 2069 6620 6861             if ha
-00000df0: 7361 7474 7228 7365 6c66 2c20 2269 6d61  sattr(self, "ima
-00000e00: 6765 5f6c 6179 6572 2229 3a0d 0a20 2020  ge_layer"):..   
-00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e20: 2020 2020 2073 656c 662e 696d 6167 655f       self.image_
-00000e30: 6c61 7965 722e 6761 6d6d 6120 3d20 6761  layer.gamma = ga
-00000e40: 6d6d 610d 0a20 2020 2020 2020 2020 2020  mma..           
-00000e50: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00000e60: 662e 696d 6167 655f 6c61 7965 722e 636f  f.image_layer.co
-00000e70: 6e74 7261 7374 5f6c 696d 6974 7320 3d20  ntrast_limits = 
-00000e80: 636f 6e74 7261 7374 5f6c 696d 6974 730d  contrast_limits.
-00000e90: 0a0d 0a20 2020 2020 2020 2065 7863 6570  ...        excep
-00000ea0: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
-00000eb0: 7072 696e 7428 7472 6163 6562 6163 6b2e  print(traceback.
-00000ec0: 666f 726d 6174 5f65 7863 2829 290d 0a0d  format_exc())...
-00000ed0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000ee0: 636f 6e74 7261 7374 5f6c 696d 6974 730d  contrast_limits.
-00000ef0: 0a0d 0a0d 0a20 2020 2064 6566 2075 7064  .....    def upd
-00000f00: 6174 655f 636f 6e74 7261 7374 5f64 6963  ate_contrast_dic
-00000f10: 7428 7365 6c66 293a 0d0a 0d0a 2020 2020  t(self):....    
-00000f20: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-00000f30: 2020 2020 2020 6461 7461 7365 7420 3d20        dataset = 
-00000f40: 7365 6c66 2e61 6374 6976 655f 6461 7461  self.active_data
-00000f50: 7365 740d 0a0d 0a20 2020 2020 2020 2020  set....         
-00000f60: 2020 2069 6620 6461 7461 7365 7420 696e     if dataset in
-00000f70: 2073 656c 662e 6461 7461 7365 745f 6469   self.dataset_di
-00000f80: 6374 2e6b 6579 7328 293a 0d0a 0d0a 2020  ct.keys():....  
-00000f90: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00000fa0: 2064 6174 6173 6574 206e 6f74 2069 6e20   dataset not in 
-00000fb0: 7365 6c66 2e63 6f6e 7472 6173 745f 6469  self.contrast_di
-00000fc0: 6374 2e6b 6579 7328 293a 0d0a 2020 2020  ct.keys():..    
-00000fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bc0: 7365 6c66 2e69 6d61 6765 5f6c 6179 6572  self.image_layer
+00000bd0: 2e67 616d 6d61 203d 2067 616d 6d61 0d0a  .gamma = gamma..
+00000be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bf0: 2020 2020 7365 6c66 2e69 6d61 6765 5f6c      self.image_l
+00000c00: 6179 6572 2e63 6f6e 7472 6173 745f 6c69  ayer.contrast_li
+00000c10: 6d69 7473 203d 2063 6f6e 7472 6173 745f  mits = contrast_
+00000c20: 6c69 6d69 7473 0d0a 0d0a 2020 2020 2020  limits....      
+00000c30: 2020 2020 2020 6966 2061 7574 6f63 6f6e        if autocon
+00000c40: 7472 6173 7420 6973 2054 7275 653a 0d0a  trast is True:..
+00000c50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000c60: 2020 6675 6c6c 5f72 616e 6765 203d 205b    full_range = [
+00000c70: 6e70 2e6d 696e 2869 6d61 6765 292c 206e  np.min(image), n
+00000c80: 702e 6d61 7828 696d 6167 6529 5d0d 0a0d  p.max(image)]...
+00000c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000ca0: 2069 6620 6d61 7828 6675 6c6c 5f72 616e   if max(full_ran
+00000cb0: 6765 2920 3e20 6d69 6e28 6675 6c6c 5f72  ge) > min(full_r
+00000cc0: 616e 6765 293a 0d0a 2020 2020 2020 2020  ange):..        
+00000cd0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+00000ce0: 7261 7374 5f6c 696d 6974 7320 3d20 6e70  rast_limits = np
+00000cf0: 2e70 6572 6365 6e74 696c 6528 696d 6167  .percentile(imag
+00000d00: 655b 3a31 305d 2e63 6f70 7928 292c 205b  e[:10].copy(), [
+00000d10: 302e 312c 2039 392e 3939 5d29 0d0a 0d0a  0.1, 99.99])....
+00000d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d30: 2020 2020 6761 6d6d 6120 3d20 312e 300d      gamma = 1.0.
+00000d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000d50: 2020 2020 2069 6620 636f 6e74 7261 7374       if contrast
+00000d60: 5f6c 696d 6974 735b 315d 203e 2063 6f6e  _limits[1] > con
+00000d70: 7472 6173 745f 6c69 6d69 7473 5b30 5d3a  trast_limits[0]:
+00000d80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000d90: 2020 2020 2020 2020 2020 6761 6d6d 6120            gamma 
+00000da0: 3d20 6e70 2e6c 6f67 2830 2e35 2920 2f20  = np.log(0.5) / 
+00000db0: 6e70 2e6c 6f67 2828 636f 6e74 7261 7374  np.log((contrast
+00000dc0: 5f6c 696d 6974 735b 315d 202d 2063 6f6e  _limits[1] - con
+00000dd0: 7472 6173 745f 6c69 6d69 7473 5b30 5d29  trast_limits[0])
+00000de0: 202f 2028 6675 6c6c 5f72 616e 6765 5b31   / (full_range[1
+00000df0: 5d20 2d20 6675 6c6c 5f72 616e 6765 5b30  ] - full_range[0
+00000e00: 5d29 290d 0a0d 0a20 2020 2020 2020 2020  ]))....         
+00000e10: 2020 2020 2020 2020 2020 2069 6620 6861             if ha
+00000e20: 7361 7474 7228 7365 6c66 2c20 2269 6d61  sattr(self, "ima
+00000e30: 6765 5f6c 6179 6572 2229 3a0d 0a20 2020  ge_layer"):..   
+00000e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e50: 2020 2020 2073 656c 662e 696d 6167 655f       self.image_
+00000e60: 6c61 7965 722e 6761 6d6d 6120 3d20 6761  layer.gamma = ga
+00000e70: 6d6d 610d 0a20 2020 2020 2020 2020 2020  mma..           
+00000e80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00000e90: 662e 696d 6167 655f 6c61 7965 722e 636f  f.image_layer.co
+00000ea0: 6e74 7261 7374 5f6c 696d 6974 7320 3d20  ntrast_limits = 
+00000eb0: 636f 6e74 7261 7374 5f6c 696d 6974 730d  contrast_limits.
+00000ec0: 0a0d 0a20 2020 2020 2020 2065 7863 6570  ...        excep
+00000ed0: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
+00000ee0: 7072 696e 7428 7472 6163 6562 6163 6b2e  print(traceback.
+00000ef0: 666f 726d 6174 5f65 7863 2829 290d 0a0d  format_exc())...
+00000f00: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000f10: 636f 6e74 7261 7374 5f6c 696d 6974 730d  contrast_limits.
+00000f20: 0a0d 0a0d 0a20 2020 2064 6566 2075 7064  .....    def upd
+00000f30: 6174 655f 636f 6e74 7261 7374 5f64 6963  ate_contrast_dic
+00000f40: 7428 7365 6c66 293a 0d0a 0d0a 2020 2020  t(self):....    
+00000f50: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00000f60: 2020 2020 2020 6461 7461 7365 7420 3d20        dataset = 
+00000f70: 7365 6c66 2e61 6374 6976 655f 6461 7461  self.active_data
+00000f80: 7365 740d 0a0d 0a20 2020 2020 2020 2020  set....         
+00000f90: 2020 2069 6620 6461 7461 7365 7420 696e     if dataset in
+00000fa0: 2073 656c 662e 6461 7461 7365 745f 6469   self.dataset_di
+00000fb0: 6374 2e6b 6579 7328 293a 0d0a 0d0a 2020  ct.keys():....  
+00000fc0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00000fd0: 2064 6174 6173 6574 206e 6f74 2069 6e20   dataset not in 
 00000fe0: 7365 6c66 2e63 6f6e 7472 6173 745f 6469  self.contrast_di
-00000ff0: 6374 5b64 6174 6173 6574 5d20 3d20 7b7d  ct[dataset] = {}
-00001000: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00001010: 2020 2020 6c61 7965 725f 6e61 6d65 203d      layer_name =
-00001020: 205b 6c61 7965 722e 6e61 6d65 2066 6f72   [layer.name for
-00001030: 206c 6179 6572 2069 6e20 7365 6c66 2e76   layer in self.v
-00001040: 6965 7765 722e 6c61 7965 7273 2069 6620  iewer.layers if 
-00001050: 6461 7461 7365 7420 696e 206c 6179 6572  dataset in layer
-00001060: 2e6e 616d 655d 0d0a 0d0a 2020 2020 2020  .name]....      
-00001070: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-00001080: 286c 6179 6572 5f6e 616d 6529 203e 2030  (layer_name) > 0
-00001090: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
-000010a0: 2020 2020 2020 2020 2069 6d61 6765 5f6c           image_l
-000010b0: 6179 6572 203d 2073 656c 662e 7669 6577  ayer = self.view
-000010c0: 6572 2e6c 6179 6572 735b 6c61 7965 725f  er.layers[layer_
-000010d0: 6e61 6d65 5b30 5d5d 0d0a 2020 2020 2020  name[0]]..      
-000010e0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000010f0: 6e74 7261 7374 5f6c 696d 6974 7320 3d20  ntrast_limits = 
-00001100: 696d 6167 655f 6c61 7965 722e 636f 6e74  image_layer.cont
-00001110: 7261 7374 5f6c 696d 6974 730d 0a20 2020  rast_limits..   
-00001120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001130: 2067 616d 6d61 203d 2069 6d61 6765 5f6c   gamma = image_l
-00001140: 6179 6572 2e67 616d 6d61 0d0a 0d0a 2020  ayer.gamma....  
+00000ff0: 6374 2e6b 6579 7328 293a 0d0a 2020 2020  ct.keys():..    
+00001000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001010: 7365 6c66 2e63 6f6e 7472 6173 745f 6469  self.contrast_di
+00001020: 6374 5b64 6174 6173 6574 5d20 3d20 7b7d  ct[dataset] = {}
+00001030: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00001040: 2020 2020 6c61 7965 725f 6e61 6d65 203d      layer_name =
+00001050: 205b 6c61 7965 722e 6e61 6d65 2066 6f72   [layer.name for
+00001060: 206c 6179 6572 2069 6e20 7365 6c66 2e76   layer in self.v
+00001070: 6965 7765 722e 6c61 7965 7273 2069 6620  iewer.layers if 
+00001080: 6461 7461 7365 7420 696e 206c 6179 6572  dataset in layer
+00001090: 2e6e 616d 655d 0d0a 0d0a 2020 2020 2020  .name]....      
+000010a0: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+000010b0: 286c 6179 6572 5f6e 616d 6529 203e 2030  (layer_name) > 0
+000010c0: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
+000010d0: 2020 2020 2020 2020 2069 6d61 6765 5f6c           image_l
+000010e0: 6179 6572 203d 2073 656c 662e 7669 6577  ayer = self.view
+000010f0: 6572 2e6c 6179 6572 735b 6c61 7965 725f  er.layers[layer_
+00001100: 6e61 6d65 5b30 5d5d 0d0a 2020 2020 2020  name[0]]..      
+00001110: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00001120: 6e74 7261 7374 5f6c 696d 6974 7320 3d20  ntrast_limits = 
+00001130: 696d 6167 655f 6c61 7965 722e 636f 6e74  image_layer.cont
+00001140: 7261 7374 5f6c 696d 6974 730d 0a20 2020  rast_limits..   
 00001150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001160: 2020 7365 6c66 2e63 6f6e 7472 6173 745f    self.contrast_
-00001170: 6469 6374 5b64 6174 6173 6574 5d20 3d20  dict[dataset] = 
-00001180: 7b22 636f 6e74 7261 7374 5f6c 696d 6974  {"contrast_limit
-00001190: 7322 3a20 636f 6e74 7261 7374 5f6c 696d  s": contrast_lim
-000011a0: 6974 732c 0d0a 2020 2020 2020 2020 2020  its,..          
-000011b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011d0: 2020 2020 2020 2020 2022 6761 6d6d 6122           "gamma"
-000011e0: 3a20 6761 6d6d 617d 0d0a 0d0a 2020 2020  : gamma}....    
-000011f0: 2020 2020 6578 6365 7074 3a0d 0a20 2020      except:..   
-00001200: 2020 2020 2020 2020 2070 7269 6e74 2874           print(t
-00001210: 7261 6365 6261 636b 2e66 6f72 6d61 745f  raceback.format_
-00001220: 6578 6328 2929 0d0a 0d0a 0d0a 0d0a 2020  exc())........  
-00001230: 2020 6465 6620 7570 6461 7465 5f61 6374    def update_act
-00001240: 6976 655f 696d 6167 6528 7365 6c66 2c20  ive_image(self, 
-00001250: 6461 7461 7365 743d 4e6f 6e65 2c20 6576  dataset=None, ev
-00001260: 656e 743d 4e6f 6e65 293a 0d0a 0d0a 2020  ent=None):....  
-00001270: 2020 2020 2020 7472 793a 0d0a 0d0a 2020        try:....  
-00001280: 2020 2020 2020 2020 2020 6966 2064 6174            if dat
-00001290: 6173 6574 203d 3d20 4e6f 6e65 206f 7220  aset == None or 
-000012a0: 6461 7461 7365 7420 6e6f 7420 696e 2073  dataset not in s
-000012b0: 656c 662e 6461 7461 7365 745f 6469 6374  elf.dataset_dict
-000012c0: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
-000012d0: 2020 2020 2020 2020 2020 6461 7461 7365            datase
-000012e0: 745f 6e61 6d65 203d 2073 656c 662e 6775  t_name = self.gu
-000012f0: 692e 6d6f 6c74 7261 636b 5f64 6174 6173  i.moltrack_datas
-00001300: 6574 5f73 656c 6563 746f 722e 6375 7272  et_selector.curr
-00001310: 656e 7454 6578 7428 290d 0a20 2020 2020  entText()..     
-00001320: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00001330: 2020 2020 2020 2020 2020 2020 2020 6461                da
-00001340: 7461 7365 745f 6e61 6d65 203d 2064 6174  taset_name = dat
-00001350: 6173 6574 0d0a 0d0a 2020 2020 2020 2020  aset....        
-00001360: 2020 2020 6966 2064 6174 6173 6574 5f6e      if dataset_n
-00001370: 616d 6520 696e 2073 656c 662e 6461 7461  ame in self.data
-00001380: 7365 745f 6469 6374 2e6b 6579 7328 293a  set_dict.keys():
-00001390: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000013a0: 2020 2020 7365 6c66 2e75 7064 6174 655f      self.update_
-000013b0: 636f 6e74 7261 7374 5f64 6963 7428 290d  contrast_dict().
-000013c0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000013d0: 2020 2073 656c 662e 6163 7469 7665 5f64     self.active_d
-000013e0: 6174 6173 6574 203d 2064 6174 6173 6574  ataset = dataset
-000013f0: 5f6e 616d 650d 0a0d 0a20 2020 2020 2020  _name....       
-00001400: 2020 2020 2020 2020 2069 6620 2264 6174           if "dat
-00001410: 6122 2069 6e20 7365 6c66 2e64 6174 6173  a" in self.datas
-00001420: 6574 5f64 6963 745b 6461 7461 7365 745f  et_dict[dataset_
-00001430: 6e61 6d65 5d2e 6b65 7973 2829 3a0d 0a0d  name].keys():...
-00001440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001450: 2020 2020 2069 6d61 6765 203d 2073 656c       image = sel
-00001460: 662e 6461 7461 7365 745f 6469 6374 5b64  f.dataset_dict[d
-00001470: 6174 6173 6574 5f6e 616d 655d 5b22 6461  ataset_name]["da
-00001480: 7461 225d 0d0a 0d0a 2020 2020 2020 2020  ta"]....        
-00001490: 2020 2020 2020 2020 2020 2020 6966 2068              if h
-000014a0: 6173 6174 7472 2873 656c 662c 2022 696d  asattr(self, "im
-000014b0: 6167 655f 6c61 7965 7222 2920 3d3d 2046  age_layer") == F
-000014c0: 616c 7365 3a0d 0a0d 0a20 2020 2020 2020  alse:....       
-000014d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014e0: 2073 656c 662e 696d 6167 655f 6c61 7965   self.image_laye
-000014f0: 7220 3d20 7365 6c66 2e76 6965 7765 722e  r = self.viewer.
-00001500: 6164 645f 696d 6167 6528 696d 6167 652c  add_image(image,
-00001510: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001520: 2020 2020 2020 2020 2020 2020 2020 6e61                na
-00001530: 6d65 3d64 6174 6173 6574 5f6e 616d 652c  me=dataset_name,
-00001540: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001550: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00001560: 6c6f 726d 6170 3d22 6772 6179 222c 0d0a  lormap="gray",..
-00001570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001580: 2020 2020 2020 2020 2020 2020 626c 656e              blen
-00001590: 6469 6e67 3d22 6164 6469 7469 7665 222c  ding="additive",
-000015a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000015b0: 2020 2020 2020 2020 2020 2020 2020 7669                vi
-000015c0: 7369 626c 653d 5472 7565 290d 0a0d 0a20  sible=True).... 
-000015d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015e0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-000015f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001600: 2020 7365 6c66 2e69 6d61 6765 5f6c 6179    self.image_lay
-00001610: 6572 2e64 6174 6120 3d20 696d 6167 650d  er.data = image.
-00001620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001630: 2020 2020 2020 2020 2073 656c 662e 696d           self.im
-00001640: 6167 655f 6c61 7965 722e 6e61 6d65 203d  age_layer.name =
-00001650: 2064 6174 6173 6574 5f6e 616d 650d 0a20   dataset_name.. 
-00001660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001670: 2020 2020 2020 2073 656c 662e 696d 6167         self.imag
-00001680: 655f 6c61 7965 722e 7265 6672 6573 6828  e_layer.refresh(
-00001690: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-000016a0: 2020 2020 2020 2020 2073 656c 662e 696d           self.im
-000016b0: 6167 655f 6c61 7965 725f 6175 746f 5f63  age_layer_auto_c
-000016c0: 6f6e 7472 6173 7428 696d 6167 652c 2064  ontrast(image, d
-000016d0: 6174 6173 6574 5f6e 616d 6529 0d0a 0d0a  ataset_name)....
-000016e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016f0: 2020 2020 6461 7461 7365 745f 6e61 6d65      dataset_name
-00001700: 7320 3d20 7365 6c66 2e64 6174 6173 6574  s = self.dataset
-00001710: 5f64 6963 742e 6b65 7973 2829 0d0a 2020  _dict.keys()..  
-00001720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001730: 2020 6163 7469 7665 5f64 6174 6173 6574    active_dataset
-00001740: 5f69 6e64 6578 203d 206c 6973 7428 6461  _index = list(da
-00001750: 7461 7365 745f 6e61 6d65 7329 2e69 6e64  taset_names).ind
-00001760: 6578 2864 6174 6173 6574 5f6e 616d 6529  ex(dataset_name)
-00001770: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00001780: 2020 2020 2020 2020 6461 7461 7365 745f          dataset_
-00001790: 7365 6c65 6374 6f72 203d 2073 656c 662e  selector = self.
-000017a0: 6775 692e 6d6f 6c74 7261 636b 5f64 6174  gui.moltrack_dat
-000017b0: 6173 6574 5f73 656c 6563 746f 720d 0a0d  aset_selector...
-000017c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000017d0: 2020 2020 2064 6174 6173 6574 5f73 656c       dataset_sel
-000017e0: 6563 746f 722e 626c 6f63 6b53 6967 6e61  ector.blockSigna
-000017f0: 6c73 2854 7275 6529 0d0a 2020 2020 2020  ls(True)..      
-00001800: 2020 2020 2020 2020 2020 2020 2020 6461                da
-00001810: 7461 7365 745f 7365 6c65 6374 6f72 2e63  taset_selector.c
-00001820: 6c65 6172 2829 0d0a 2020 2020 2020 2020  lear()..        
-00001830: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00001840: 7365 745f 7365 6c65 6374 6f72 2e61 6464  set_selector.add
-00001850: 4974 656d 7328 6461 7461 7365 745f 6e61  Items(dataset_na
-00001860: 6d65 7329 0d0a 2020 2020 2020 2020 2020  mes)..          
-00001870: 2020 2020 2020 2020 2020 6461 7461 7365            datase
-00001880: 745f 7365 6c65 6374 6f72 2e73 6574 4375  t_selector.setCu
-00001890: 7272 656e 7449 6e64 6578 2861 6374 6976  rrentIndex(activ
-000018a0: 655f 6461 7461 7365 745f 696e 6465 7829  e_dataset_index)
-000018b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000018c0: 2020 2020 2020 6461 7461 7365 745f 7365        dataset_se
-000018d0: 6c65 6374 6f72 2e62 6c6f 636b 5369 676e  lector.blockSign
-000018e0: 616c 7328 4661 6c73 6529 0d0a 0d0a 2020  als(False)....  
-000018f0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-00001900: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00001910: 2020 2073 656c 662e 6163 7469 7665 5f64     self.active_d
-00001920: 6174 6173 6574 203d 204e 6f6e 650d 0a0d  ataset = None...
-00001930: 0a20 2020 2020 2020 2020 2020 2023 2073  .            # s
-00001940: 656c 662e 6472 6177 5f6c 6f63 616c 6973  elf.draw_localis
-00001950: 6174 696f 6e73 2875 7064 6174 655f 7669  ations(update_vi
-00001960: 733d 5472 7565 290d 0a20 2020 2020 2020  s=True)..       
-00001970: 2020 2020 2073 656c 662e 7570 6461 7465       self.update
-00001980: 5f6f 7665 726c 6179 5f74 6578 7428 290d  _overlay_text().
-00001990: 0a0d 0a20 2020 2020 2020 2065 7863 6570  ...        excep
-000019a0: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
-000019b0: 7072 696e 7428 7472 6163 6562 6163 6b2e  print(traceback.
-000019c0: 666f 726d 6174 5f65 7863 2829 290d 0a20  format_exc()).. 
-000019d0: 2020 2020 2020 2020 2020 2070 6173 730d             pass.
-000019e0: 0a0d 0a20 2020 2064 6566 2075 7064 6174  ...    def updat
-000019f0: 655f 6f76 6572 6c61 795f 7465 7874 2873  e_overlay_text(s
-00001a00: 656c 6629 3a0d 0a0d 0a20 2020 2020 2020  elf):....       
-00001a10: 2074 7279 3a0d 0a0d 0a20 2020 2020 2020   try:....       
-00001a20: 2020 2020 2069 6620 7365 6c66 2e64 6174       if self.dat
-00001a30: 6173 6574 5f64 6963 7420 2021 3d20 7b7d  aset_dict  != {}
-00001a40: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
-00001a50: 2020 2020 2064 6174 6173 6574 5f6e 616d       dataset_nam
-00001a60: 6520 3d20 7365 6c66 2e67 7569 2e6d 6f6c  e = self.gui.mol
-00001a70: 7472 6163 6b5f 6461 7461 7365 745f 7365  track_dataset_se
-00001a80: 6c65 6374 6f72 2e63 7572 7265 6e74 5465  lector.currentTe
-00001a90: 7874 2829 0d0a 0d0a 2020 2020 2020 2020  xt()....        
-00001aa0: 2020 2020 2020 2020 6966 2064 6174 6173          if datas
-00001ab0: 6574 5f6e 616d 6520 696e 2073 656c 662e  et_name in self.
-00001ac0: 6461 7461 7365 745f 6469 6374 2e6b 6579  dataset_dict.key
-00001ad0: 7328 293a 0d0a 0d0a 2020 2020 2020 2020  s():....        
-00001ae0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00001af0: 5f64 6963 7420 3d20 7365 6c66 2e64 6174  _dict = self.dat
-00001b00: 6173 6574 5f64 6963 745b 6461 7461 7365  aset_dict[datase
-00001b10: 745f 6e61 6d65 5d2e 636f 7079 2829 0d0a  t_name].copy()..
-00001b20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001b30: 2020 2020 2020 7061 7468 203d 2064 6174        path = dat
-00001b40: 615f 6469 6374 5b22 7061 7468 225d 0d0a  a_dict["path"]..
-00001b50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001b60: 2020 2020 2020 6966 2074 7970 6528 7061        if type(pa
-00001b70: 7468 2920 3d3d 206c 6973 743a 0d0a 2020  th) == list:..  
-00001b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b90: 2020 2020 2020 6375 7272 656e 745f 7374        current_st
-00001ba0: 6570 203d 2073 656c 662e 7669 6577 6572  ep = self.viewer
-00001bb0: 2e64 696d 732e 6375 7272 656e 745f 7374  .dims.current_st
-00001bc0: 6570 5b30 5d0d 0a20 2020 2020 2020 2020  ep[0]..         
-00001bd0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00001be0: 6174 6820 3d20 7061 7468 5b63 7572 7265  ath = path[curre
-00001bf0: 6e74 5f73 7465 705d 0d0a 0d0a 2020 2020  nt_step]....    
-00001c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c10: 6669 6c65 5f6e 616d 6520 3d20 6f73 2e70  file_name = os.p
-00001c20: 6174 682e 6261 7365 6e61 6d65 2870 6174  ath.basename(pat
-00001c30: 6829 0d0a 0d0a 2020 2020 2020 2020 2020  h)....          
-00001c40: 2020 2020 2020 2020 2020 6f76 6572 6c61            overla
-00001c50: 795f 7374 7269 6e67 203d 2022 220d 0a20  y_string = "".. 
-00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c70: 2020 206f 7665 726c 6179 5f73 7472 696e     overlay_strin
-00001c80: 6720 2b3d 2066 2246 696c 653a 207b 6669  g += f"File: {fi
-00001c90: 6c65 5f6e 616d 657d 5c6e 220d 0a0d 0a20  le_name}\n".... 
-00001ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cb0: 2020 2069 6620 6f76 6572 6c61 795f 7374     if overlay_st
-00001cc0: 7269 6e67 2021 3d20 2222 3a0d 0a20 2020  ring != "":..   
-00001cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ce0: 2020 2020 2073 656c 662e 7669 6577 6572       self.viewer
-00001cf0: 2e74 6578 745f 6f76 6572 6c61 792e 7669  .text_overlay.vi
-00001d00: 7369 626c 6520 3d20 5472 7565 0d0a 2020  sible = True..  
-00001d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d20: 2020 2020 2020 7365 6c66 2e76 6965 7765        self.viewe
-00001d30: 722e 7465 7874 5f6f 7665 726c 6179 2e70  r.text_overlay.p
-00001d40: 6f73 6974 696f 6e20 3d20 2274 6f70 5f6c  osition = "top_l
-00001d50: 6566 7422 0d0a 2020 2020 2020 2020 2020  eft"..          
-00001d60: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00001d70: 6c66 2e76 6965 7765 722e 7465 7874 5f6f  lf.viewer.text_o
-00001d80: 7665 726c 6179 2e74 6578 7420 3d20 6f76  verlay.text = ov
-00001d90: 6572 6c61 795f 7374 7269 6e67 2e6c 7374  erlay_string.lst
-00001da0: 7269 7028 225c 6e22 290d 0a20 2020 2020  rip("\n")..     
-00001db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001dc0: 2020 2073 656c 662e 7669 6577 6572 2e74     self.viewer.t
-00001dd0: 6578 745f 6f76 6572 6c61 792e 636f 6c6f  ext_overlay.colo
-00001de0: 7220 3d20 2272 6564 220d 0a20 2020 2020  r = "red"..     
+00001160: 2067 616d 6d61 203d 2069 6d61 6765 5f6c   gamma = image_l
+00001170: 6179 6572 2e67 616d 6d61 0d0a 0d0a 2020  ayer.gamma....  
+00001180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001190: 2020 7365 6c66 2e63 6f6e 7472 6173 745f    self.contrast_
+000011a0: 6469 6374 5b64 6174 6173 6574 5d20 3d20  dict[dataset] = 
+000011b0: 7b22 636f 6e74 7261 7374 5f6c 696d 6974  {"contrast_limit
+000011c0: 7322 3a20 636f 6e74 7261 7374 5f6c 696d  s": contrast_lim
+000011d0: 6974 732c 0d0a 2020 2020 2020 2020 2020  its,..          
+000011e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001200: 2020 2020 2020 2020 2022 6761 6d6d 6122           "gamma"
+00001210: 3a20 6761 6d6d 617d 0d0a 0d0a 2020 2020  : gamma}....    
+00001220: 2020 2020 6578 6365 7074 3a0d 0a20 2020      except:..   
+00001230: 2020 2020 2020 2020 2070 7269 6e74 2874           print(t
+00001240: 7261 6365 6261 636b 2e66 6f72 6d61 745f  raceback.format_
+00001250: 6578 6328 2929 0d0a 0d0a 0d0a 2020 2020  exc())......    
+00001260: 6465 6620 6472 6177 5f73 6567 6d65 6e74  def draw_segment
+00001270: 6174 696f 6e5f 696d 6167 6528 7365 6c66  ation_image(self
+00001280: 293a 0d0a 0d0a 2020 2020 2020 2020 6966  ):....        if
+00001290: 2068 6173 6174 7472 2873 656c 662c 2022   hasattr(self, "
+000012a0: 7365 676d 656e 7461 7469 6f6e 5f69 6d61  segmentation_ima
+000012b0: 6765 2229 3a0d 0a0d 0a20 2020 2020 2020  ge"):....       
+000012c0: 2020 2020 2069 6620 6861 7361 7474 7228       if hasattr(
+000012d0: 7365 6c66 2c20 2273 6567 6d65 6e74 6174  self, "segmentat
+000012e0: 696f 6e5f 6c61 7965 7222 293a 0d0a 2020  ion_layer"):..  
+000012f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00001300: 6c66 2e73 6567 6d65 6e74 6174 696f 6e5f  lf.segmentation_
+00001310: 6c61 7965 722e 6461 7461 203d 2073 656c  layer.data = sel
+00001320: 662e 7365 676d 656e 7461 7469 6f6e 5f69  f.segmentation_i
+00001330: 6d61 6765 2e63 6f70 7928 290d 0a20 2020  mage.copy()..   
+00001340: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00001350: 662e 7365 676d 656e 7461 7469 6f6e 5f6c  f.segmentation_l
+00001360: 6179 6572 2e72 6566 7265 7368 2829 0d0a  ayer.refresh()..
+00001370: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00001380: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00001390: 2020 2073 656c 662e 7365 676d 656e 7461     self.segmenta
+000013a0: 7469 6f6e 5f6c 6179 6572 203d 2073 656c  tion_layer = sel
+000013b0: 662e 7669 6577 6572 2e61 6464 5f69 6d61  f.viewer.add_ima
+000013c0: 6765 2873 656c 662e 7365 676d 656e 7461  ge(self.segmenta
+000013d0: 7469 6f6e 5f69 6d61 6765 2c0d 0a20 2020  tion_image,..   
+000013e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013f0: 206e 616d 653d 2253 6567 6d65 6e74 6174   name="Segmentat
+00001400: 696f 6e20 496d 6167 6522 2c20 7669 7369  ion Image", visi
+00001410: 626c 653d 5472 7565 290d 0a20 2020 2020  ble=True)..     
+00001420: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00001430: 7365 676d 656e 7461 7469 6f6e 5f6c 6179  segmentation_lay
+00001440: 6572 2e72 6566 7265 7368 2829 0d0a 0d0a  er.refresh()....
+00001450: 2020 2020 6465 6620 7570 6461 7465 5f61      def update_a
+00001460: 6374 6976 655f 696d 6167 6528 7365 6c66  ctive_image(self
+00001470: 2c20 6461 7461 7365 743d 4e6f 6e65 2c20  , dataset=None, 
+00001480: 6576 656e 743d 4e6f 6e65 293a 0d0a 0d0a  event=None):....
+00001490: 2020 2020 2020 2020 7472 793a 0d0a 0d0a          try:....
+000014a0: 2020 2020 2020 2020 2020 2020 6966 2064              if d
+000014b0: 6174 6173 6574 203d 3d20 4e6f 6e65 206f  ataset == None o
+000014c0: 7220 6461 7461 7365 7420 6e6f 7420 696e  r dataset not in
+000014d0: 2073 656c 662e 6461 7461 7365 745f 6469   self.dataset_di
+000014e0: 6374 2e6b 6579 7328 293a 0d0a 2020 2020  ct.keys():..    
+000014f0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00001500: 7365 745f 6e61 6d65 203d 2073 656c 662e  set_name = self.
+00001510: 6775 692e 6d6f 6c74 7261 636b 5f64 6174  gui.moltrack_dat
+00001520: 6173 6574 5f73 656c 6563 746f 722e 6375  aset_selector.cu
+00001530: 7272 656e 7454 6578 7428 290d 0a20 2020  rrentText()..   
+00001540: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00001550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001560: 6461 7461 7365 745f 6e61 6d65 203d 2064  dataset_name = d
+00001570: 6174 6173 6574 0d0a 0d0a 2020 2020 2020  ataset....      
+00001580: 2020 2020 2020 6966 2064 6174 6173 6574        if dataset
+00001590: 5f6e 616d 6520 696e 2073 656c 662e 6461  _name in self.da
+000015a0: 7461 7365 745f 6469 6374 2e6b 6579 7328  taset_dict.keys(
+000015b0: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
+000015c0: 2020 2020 2020 7365 6c66 2e75 7064 6174        self.updat
+000015d0: 655f 636f 6e74 7261 7374 5f64 6963 7428  e_contrast_dict(
+000015e0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+000015f0: 2020 2020 2073 656c 662e 6163 7469 7665       self.active
+00001600: 5f64 6174 6173 6574 203d 2064 6174 6173  _dataset = datas
+00001610: 6574 5f6e 616d 650d 0a0d 0a20 2020 2020  et_name....     
+00001620: 2020 2020 2020 2020 2020 2069 6620 2264             if "d
+00001630: 6174 6122 2069 6e20 7365 6c66 2e64 6174  ata" in self.dat
+00001640: 6173 6574 5f64 6963 745b 6461 7461 7365  aset_dict[datase
+00001650: 745f 6e61 6d65 5d2e 6b65 7973 2829 3a0d  t_name].keys():.
+00001660: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00001670: 2020 2020 2020 2069 6d61 6765 203d 2073         image = s
+00001680: 656c 662e 6461 7461 7365 745f 6469 6374  elf.dataset_dict
+00001690: 5b64 6174 6173 6574 5f6e 616d 655d 5b22  [dataset_name]["
+000016a0: 6461 7461 225d 0d0a 0d0a 2020 2020 2020  data"]....      
+000016b0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000016c0: 2068 6173 6174 7472 2873 656c 662c 2022   hasattr(self, "
+000016d0: 696d 6167 655f 6c61 7965 7222 2920 3d3d  image_layer") ==
+000016e0: 2046 616c 7365 3a0d 0a0d 0a20 2020 2020   False:....     
+000016f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001700: 2020 2073 656c 662e 696d 6167 655f 6c61     self.image_la
+00001710: 7965 7220 3d20 7365 6c66 2e76 6965 7765  yer = self.viewe
+00001720: 722e 6164 645f 696d 6167 6528 696d 6167  r.add_image(imag
+00001730: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00001740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001750: 6e61 6d65 3d64 6174 6173 6574 5f6e 616d  name=dataset_nam
+00001760: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00001770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001780: 636f 6c6f 726d 6170 3d22 6772 6179 222c  colormap="gray",
+00001790: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000017a0: 2020 2020 2020 2020 2020 2020 2020 626c                bl
+000017b0: 656e 6469 6e67 3d22 6164 6469 7469 7665  ending="additive
+000017c0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+000017d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017e0: 7669 7369 626c 653d 5472 7565 290d 0a0d  visible=True)...
+000017f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001800: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00001810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001820: 2020 2020 7365 6c66 2e69 6d61 6765 5f6c      self.image_l
+00001830: 6179 6572 2e64 6174 6120 3d20 696d 6167  ayer.data = imag
+00001840: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+00001850: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00001860: 696d 6167 655f 6c61 7965 722e 6e61 6d65  image_layer.name
+00001870: 203d 2064 6174 6173 6574 5f6e 616d 650d   = dataset_name.
+00001880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001890: 2020 2020 2020 2020 2073 656c 662e 696d           self.im
+000018a0: 6167 655f 6c61 7965 722e 7265 6672 6573  age_layer.refres
+000018b0: 6828 290d 0a0d 0a20 2020 2020 2020 2020  h()....         
+000018c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000018d0: 696d 6167 655f 6c61 7965 725f 6175 746f  image_layer_auto
+000018e0: 5f63 6f6e 7472 6173 7428 696d 6167 652c  _contrast(image,
+000018f0: 2064 6174 6173 6574 5f6e 616d 6529 0d0a   dataset_name)..
+00001900: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001910: 2020 2020 2020 6461 7461 7365 745f 6e61        dataset_na
+00001920: 6d65 7320 3d20 7365 6c66 2e64 6174 6173  mes = self.datas
+00001930: 6574 5f64 6963 742e 6b65 7973 2829 0d0a  et_dict.keys()..
+00001940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001950: 2020 2020 6163 7469 7665 5f64 6174 6173      active_datas
+00001960: 6574 5f69 6e64 6578 203d 206c 6973 7428  et_index = list(
+00001970: 6461 7461 7365 745f 6e61 6d65 7329 2e69  dataset_names).i
+00001980: 6e64 6578 2864 6174 6173 6574 5f6e 616d  ndex(dataset_nam
+00001990: 6529 0d0a 0d0a 2020 2020 2020 2020 2020  e)....          
+000019a0: 2020 2020 2020 2020 2020 6461 7461 7365            datase
+000019b0: 745f 7365 6c65 6374 6f72 203d 2073 656c  t_selector = sel
+000019c0: 662e 6775 692e 6d6f 6c74 7261 636b 5f64  f.gui.moltrack_d
+000019d0: 6174 6173 6574 5f73 656c 6563 746f 720d  ataset_selector.
+000019e0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000019f0: 2020 2020 2020 2064 6174 6173 6574 5f73         dataset_s
+00001a00: 656c 6563 746f 722e 626c 6f63 6b53 6967  elector.blockSig
+00001a10: 6e61 6c73 2854 7275 6529 0d0a 2020 2020  nals(True)..    
+00001a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a30: 6461 7461 7365 745f 7365 6c65 6374 6f72  dataset_selector
+00001a40: 2e63 6c65 6172 2829 0d0a 2020 2020 2020  .clear()..      
+00001a50: 2020 2020 2020 2020 2020 2020 2020 6461                da
+00001a60: 7461 7365 745f 7365 6c65 6374 6f72 2e61  taset_selector.a
+00001a70: 6464 4974 656d 7328 6461 7461 7365 745f  ddItems(dataset_
+00001a80: 6e61 6d65 7329 0d0a 2020 2020 2020 2020  names)..        
+00001a90: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00001aa0: 7365 745f 7365 6c65 6374 6f72 2e73 6574  set_selector.set
+00001ab0: 4375 7272 656e 7449 6e64 6578 2861 6374  CurrentIndex(act
+00001ac0: 6976 655f 6461 7461 7365 745f 696e 6465  ive_dataset_inde
+00001ad0: 7829 0d0a 2020 2020 2020 2020 2020 2020  x)..            
+00001ae0: 2020 2020 2020 2020 6461 7461 7365 745f          dataset_
+00001af0: 7365 6c65 6374 6f72 2e62 6c6f 636b 5369  selector.blockSi
+00001b00: 676e 616c 7328 4661 6c73 6529 0d0a 0d0a  gnals(False)....
+00001b10: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00001b20: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
+00001b30: 2020 2020 2073 656c 662e 6163 7469 7665       self.active
+00001b40: 5f64 6174 6173 6574 203d 204e 6f6e 650d  _dataset = None.
+00001b50: 0a0d 0a20 2020 2020 2020 2020 2020 2023  ...            #
+00001b60: 2073 656c 662e 6472 6177 5f6c 6f63 616c   self.draw_local
+00001b70: 6973 6174 696f 6e73 2875 7064 6174 655f  isations(update_
+00001b80: 7669 733d 5472 7565 290d 0a20 2020 2020  vis=True)..     
+00001b90: 2020 2020 2020 2073 656c 662e 7570 6461         self.upda
+00001ba0: 7465 5f6f 7665 726c 6179 5f74 6578 7428  te_overlay_text(
+00001bb0: 290d 0a0d 0a20 2020 2020 2020 2065 7863  )....        exc
+00001bc0: 6570 743a 0d0a 2020 2020 2020 2020 2020  ept:..          
+00001bd0: 2020 7072 696e 7428 7472 6163 6562 6163    print(tracebac
+00001be0: 6b2e 666f 726d 6174 5f65 7863 2829 290d  k.format_exc()).
+00001bf0: 0a20 2020 2020 2020 2020 2020 2070 6173  .            pas
+00001c00: 730d 0a0d 0a20 2020 2064 6566 2075 7064  s....    def upd
+00001c10: 6174 655f 6f76 6572 6c61 795f 7465 7874  ate_overlay_text
+00001c20: 2873 656c 6629 3a0d 0a0d 0a20 2020 2020  (self):....     
+00001c30: 2020 2074 7279 3a0d 0a0d 0a20 2020 2020     try:....     
+00001c40: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
+00001c50: 6174 6173 6574 5f64 6963 7420 2021 3d20  ataset_dict  != 
+00001c60: 7b7d 3a0d 0a0d 0a20 2020 2020 2020 2020  {}:....         
+00001c70: 2020 2020 2020 2064 6174 6173 6574 5f6e         dataset_n
+00001c80: 616d 6520 3d20 7365 6c66 2e67 7569 2e6d  ame = self.gui.m
+00001c90: 6f6c 7472 6163 6b5f 6461 7461 7365 745f  oltrack_dataset_
+00001ca0: 7365 6c65 6374 6f72 2e63 7572 7265 6e74  selector.current
+00001cb0: 5465 7874 2829 0d0a 0d0a 2020 2020 2020  Text()....      
+00001cc0: 2020 2020 2020 2020 2020 6966 2064 6174            if dat
+00001cd0: 6173 6574 5f6e 616d 6520 696e 2073 656c  aset_name in sel
+00001ce0: 662e 6461 7461 7365 745f 6469 6374 2e6b  f.dataset_dict.k
+00001cf0: 6579 7328 293a 0d0a 0d0a 2020 2020 2020  eys():....      
+00001d00: 2020 2020 2020 2020 2020 2020 2020 6461                da
+00001d10: 7461 5f64 6963 7420 3d20 7365 6c66 2e64  ta_dict = self.d
+00001d20: 6174 6173 6574 5f64 6963 745b 6461 7461  ataset_dict[data
+00001d30: 7365 745f 6e61 6d65 5d2e 636f 7079 2829  set_name].copy()
+00001d40: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00001d50: 2020 2020 2020 2020 7061 7468 203d 2064          path = d
+00001d60: 6174 615f 6469 6374 5b22 7061 7468 225d  ata_dict["path"]
+00001d70: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00001d80: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
+00001d90: 7061 7468 2920 3d3d 206c 6973 743a 0d0a  path) == list:..
+00001da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001db0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00001dc0: 7374 6570 203d 2073 656c 662e 7669 6577  step = self.view
+00001dd0: 6572 2e64 696d 732e 6375 7272 656e 745f  er.dims.current_
+00001de0: 7374 6570 5b30 5d0d 0a20 2020 2020 2020  step[0]..       
 00001df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e00: 2020 2073 656c 662e 7669 6577 6572 2e74     self.viewer.t
-00001e10: 6578 745f 6f76 6572 6c61 792e 666f 6e74  ext_overlay.font
-00001e20: 5f73 697a 6520 3d20 390d 0a20 2020 2020  _size = 9..     
-00001e30: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00001e40: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00001e50: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00001e60: 6c66 2e76 6965 7765 722e 7465 7874 5f6f  lf.viewer.text_o
-00001e70: 7665 726c 6179 2e76 6973 6962 6c65 203d  verlay.visible =
-00001e80: 2046 616c 7365 0d0a 0d0a 2020 2020 2020   False....      
-00001e90: 2020 6578 6365 7074 3a0d 0a20 2020 2020    except:..     
-00001ea0: 2020 2020 2020 2070 7269 6e74 2874 7261         print(tra
-00001eb0: 6365 6261 636b 2e66 6f72 6d61 745f 6578  ceback.format_ex
-00001ec0: 6328 2929 0d0a 0d0a 0d0a 2020 2020 6465  c())......    de
-00001ed0: 6620 736c 6964 6572 5f65 7665 6e74 2873  f slider_event(s
-00001ee0: 656c 662c 2076 6965 7765 723d 4e6f 6e65  elf, viewer=None
-00001ef0: 293a 0d0a 0d0a 2020 2020 2020 2020 7365  ):....        se
-00001f00: 6c66 2e75 7064 6174 655f 6f76 6572 6c61  lf.update_overla
-00001f10: 795f 7465 7874 2829 0d0a 2020 2020 2020  y_text()..      
-00001f20: 2020 7365 6c66 2e64 7261 775f 6c6f 6361    self.draw_loca
-00001f30: 6c69 7361 7469 6f6e 7328 290d 0a0d 0a20  lisations().... 
-00001f40: 2020 2064 6566 2064 7261 775f 6c6f 6361     def draw_loca
-00001f50: 6c69 7361 7469 6f6e 7328 7365 6c66 2c20  lisations(self, 
-00001f60: 7570 6461 7465 5f76 6973 3d46 616c 7365  update_vis=False
-00001f70: 293a 0d0a 0d0a 2020 2020 2020 2020 7265  ):....        re
-00001f80: 6d6f 7665 5f6c 6f63 616c 6973 6174 696f  move_localisatio
-00001f90: 6e73 203d 2054 7275 650d 0a0d 0a20 2020  ns = True....   
-00001fa0: 2020 2020 2069 6620 6861 7361 7474 7228       if hasattr(
-00001fb0: 7365 6c66 2c20 226c 6f63 616c 6973 6174  self, "localisat
-00001fc0: 696f 6e5f 6469 6374 2229 3a0d 0a0d 0a20  ion_dict"):.... 
-00001fd0: 2020 2020 2020 2020 2020 2069 6620 6861             if ha
-00001fe0: 7361 7474 7228 7365 6c66 2c20 2266 6964  sattr(self, "fid
-00001ff0: 7563 6961 6c5f 6c61 7965 7222 293a 0d0a  ucial_layer"):..
-00002000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002010: 7368 6f77 5f6c 6f63 616c 6973 6174 696f  show_localisatio
-00002020: 6e73 203d 2073 656c 662e 6c6f 635f 6c61  ns = self.loc_la
-00002030: 7965 722e 7669 7369 626c 650d 0a20 2020  yer.visible..   
-00002040: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00001e00: 2070 6174 6820 3d20 7061 7468 5b63 7572   path = path[cur
+00001e10: 7265 6e74 5f73 7465 705d 0d0a 0d0a 2020  rent_step]....  
+00001e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e30: 2020 6669 6c65 5f6e 616d 6520 3d20 6f73    file_name = os
+00001e40: 2e70 6174 682e 6261 7365 6e61 6d65 2870  .path.basename(p
+00001e50: 6174 6829 0d0a 0d0a 2020 2020 2020 2020  ath)....        
+00001e60: 2020 2020 2020 2020 2020 2020 6f76 6572              over
+00001e70: 6c61 795f 7374 7269 6e67 203d 2022 220d  lay_string = "".
+00001e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001e90: 2020 2020 206f 7665 726c 6179 5f73 7472       overlay_str
+00001ea0: 696e 6720 2b3d 2066 2246 696c 653a 207b  ing += f"File: {
+00001eb0: 6669 6c65 5f6e 616d 657d 5c6e 220d 0a0d  file_name}\n"...
+00001ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001ed0: 2020 2020 2069 6620 6f76 6572 6c61 795f       if overlay_
+00001ee0: 7374 7269 6e67 2021 3d20 2222 3a0d 0a20  string != "":.. 
+00001ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f00: 2020 2020 2020 2073 656c 662e 7669 6577         self.view
+00001f10: 6572 2e74 6578 745f 6f76 6572 6c61 792e  er.text_overlay.
+00001f20: 7669 7369 626c 6520 3d20 5472 7565 0d0a  visible = True..
+00001f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f40: 2020 2020 2020 2020 7365 6c66 2e76 6965          self.vie
+00001f50: 7765 722e 7465 7874 5f6f 7665 726c 6179  wer.text_overlay
+00001f60: 2e70 6f73 6974 696f 6e20 3d20 2274 6f70  .position = "top
+00001f70: 5f6c 6566 7422 0d0a 2020 2020 2020 2020  _left"..        
+00001f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f90: 7365 6c66 2e76 6965 7765 722e 7465 7874  self.viewer.text
+00001fa0: 5f6f 7665 726c 6179 2e74 6578 7420 3d20  _overlay.text = 
+00001fb0: 6f76 6572 6c61 795f 7374 7269 6e67 2e6c  overlay_string.l
+00001fc0: 7374 7269 7028 225c 6e22 290d 0a20 2020  strip("\n")..   
+00001fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fe0: 2020 2020 2073 656c 662e 7669 6577 6572       self.viewer
+00001ff0: 2e74 6578 745f 6f76 6572 6c61 792e 636f  .text_overlay.co
+00002000: 6c6f 7220 3d20 2272 6564 220d 0a20 2020  lor = "red"..   
+00002010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002020: 2020 2020 2073 656c 662e 7669 6577 6572       self.viewer
+00002030: 2e74 6578 745f 6f76 6572 6c61 792e 666f  .text_overlay.fo
+00002040: 6e74 5f73 697a 6520 3d20 390d 0a20 2020  nt_size = 9..   
 00002050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002060: 7368 6f77 5f6c 6f63 616c 6973 6174 696f  show_localisatio
-00002070: 6e73 203d 2054 7275 650d 0a0d 0a20 2020  ns = True....   
-00002080: 2020 2020 2020 2020 2069 6620 7368 6f77           if show
-00002090: 5f6c 6f63 616c 6973 6174 696f 6e73 3a0d  _localisations:.
-000020a0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000020b0: 2020 206c 6179 6572 5f6e 616d 6573 203d     layer_names =
-000020c0: 205b 6c61 7965 722e 6e61 6d65 2066 6f72   [layer.name for
-000020d0: 206c 6179 6572 2069 6e20 7365 6c66 2e76   layer in self.v
-000020e0: 6965 7765 722e 6c61 7965 7273 5d0d 0a0d  iewer.layers]...
-000020f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002100: 2061 6374 6976 655f 6672 616d 6520 3d20   active_frame = 
-00002110: 7365 6c66 2e76 6965 7765 722e 6469 6d73  self.viewer.dims
-00002120: 2e63 7572 7265 6e74 5f73 7465 705b 305d  .current_step[0]
-00002130: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00002140: 2020 2020 6461 7461 7365 745f 6e61 6d65      dataset_name
-00002150: 203d 2073 656c 662e 6775 692e 6d6f 6c74   = self.gui.molt
-00002160: 7261 636b 5f64 6174 6173 6574 5f73 656c  rack_dataset_sel
-00002170: 6563 746f 722e 6375 7272 656e 7454 6578  ector.currentTex
-00002180: 7428 290d 0a0d 0a20 2020 2020 2020 2020  t()....         
-00002190: 2020 2020 2020 2069 6620 6461 7461 7365         if datase
-000021a0: 745f 6e61 6d65 2069 6e20 7365 6c66 2e6c  t_name in self.l
-000021b0: 6f63 616c 6973 6174 696f 6e5f 6469 6374  ocalisation_dict
-000021c0: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
-000021d0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-000021e0: 6361 6c69 7361 7469 6f6e 5f64 6963 7420  calisation_dict 
-000021f0: 3d20 7365 6c66 2e6c 6f63 616c 6973 6174  = self.localisat
-00002200: 696f 6e5f 6469 6374 5b64 6174 6173 6574  ion_dict[dataset
-00002210: 5f6e 616d 655d 2e63 6f70 7928 290d 0a0d  _name].copy()...
-00002220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002230: 2020 2020 2069 6620 226c 6f63 616c 6973       if "localis
-00002240: 6174 696f 6e73 2220 696e 206c 6f63 616c  ations" in local
-00002250: 6973 6174 696f 6e5f 6469 6374 2e6b 6579  isation_dict.key
-00002260: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
-00002270: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00002280: 6373 203d 206c 6f63 616c 6973 6174 696f  cs = localisatio
-00002290: 6e5f 6469 6374 5b22 6c6f 6361 6c69 7361  n_dict["localisa
-000022a0: 7469 6f6e 7322 5d0d 0a0d 0a20 2020 2020  tions"]....     
-000022b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022c0: 2020 2069 6620 6163 7469 7665 5f66 7261     if active_fra
-000022d0: 6d65 2069 6e20 6c6f 6373 2e66 7261 6d65  me in locs.frame
-000022e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000022f0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00002300: 7261 6d65 5f6c 6f63 7320 3d20 6c6f 6373  rame_locs = locs
-00002310: 5b6c 6f63 732e 6672 616d 6520 3d3d 2061  [locs.frame == a
-00002320: 6374 6976 655f 6672 616d 655d 2e63 6f70  ctive_frame].cop
-00002330: 7928 290d 0a20 2020 2020 2020 2020 2020  y()..           
-00002340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002350: 2072 656e 6465 725f 6c6f 6373 203d 206e   render_locs = n
-00002360: 702e 7673 7461 636b 2828 6672 616d 655f  p.vstack((frame_
-00002370: 6c6f 6373 2e79 2c20 6672 616d 655f 6c6f  locs.y, frame_lo
-00002380: 6373 2e78 2929 2e54 2e74 6f6c 6973 7428  cs.x)).T.tolist(
-00002390: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-000023a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023b0: 2076 6973 5f6d 6f64 6520 3d20 7365 6c66   vis_mode = self
-000023c0: 2e67 7569 2e70 6963 6173 736f 5f76 6973  .gui.picasso_vis
-000023d0: 5f6d 6f64 652e 6375 7272 656e 7454 6578  _mode.currentTex
-000023e0: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
+00002060: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00002070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002080: 7365 6c66 2e76 6965 7765 722e 7465 7874  self.viewer.text
+00002090: 5f6f 7665 726c 6179 2e76 6973 6962 6c65  _overlay.visible
+000020a0: 203d 2046 616c 7365 0d0a 0d0a 2020 2020   = False....    
+000020b0: 2020 2020 6578 6365 7074 3a0d 0a20 2020      except:..   
+000020c0: 2020 2020 2020 2020 2070 7269 6e74 2874           print(t
+000020d0: 7261 6365 6261 636b 2e66 6f72 6d61 745f  raceback.format_
+000020e0: 6578 6328 2929 0d0a 0d0a 0d0a 2020 2020  exc())......    
+000020f0: 6465 6620 736c 6964 6572 5f65 7665 6e74  def slider_event
+00002100: 2873 656c 662c 2076 6965 7765 723d 4e6f  (self, viewer=No
+00002110: 6e65 293a 0d0a 0d0a 2020 2020 2020 2020  ne):....        
+00002120: 7365 6c66 2e75 7064 6174 655f 6f76 6572  self.update_over
+00002130: 6c61 795f 7465 7874 2829 0d0a 2020 2020  lay_text()..    
+00002140: 2020 2020 7365 6c66 2e64 7261 775f 6c6f      self.draw_lo
+00002150: 6361 6c69 7361 7469 6f6e 7328 290d 0a0d  calisations()...
+00002160: 0a20 2020 2064 6566 2064 7261 775f 6c6f  .    def draw_lo
+00002170: 6361 6c69 7361 7469 6f6e 7328 7365 6c66  calisations(self
+00002180: 2c20 7570 6461 7465 5f76 6973 3d46 616c  , update_vis=Fal
+00002190: 7365 293a 0d0a 0d0a 2020 2020 2020 2020  se):....        
+000021a0: 7265 6d6f 7665 5f6c 6f63 616c 6973 6174  remove_localisat
+000021b0: 696f 6e73 203d 2054 7275 650d 0a0d 0a20  ions = True.... 
+000021c0: 2020 2020 2020 2069 6620 6861 7361 7474         if hasatt
+000021d0: 7228 7365 6c66 2c20 226c 6f63 616c 6973  r(self, "localis
+000021e0: 6174 696f 6e5f 6469 6374 2229 3a0d 0a0d  ation_dict"):...
+000021f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00002200: 6861 7361 7474 7228 7365 6c66 2c20 2266  hasattr(self, "f
+00002210: 6964 7563 6961 6c5f 6c61 7965 7222 293a  iducial_layer"):
+00002220: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002230: 2020 7368 6f77 5f6c 6f63 616c 6973 6174    show_localisat
+00002240: 696f 6e73 203d 2073 656c 662e 6c6f 635f  ions = self.loc_
+00002250: 6c61 7965 722e 7669 7369 626c 650d 0a20  layer.visible.. 
+00002260: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00002270: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002280: 2020 7368 6f77 5f6c 6f63 616c 6973 6174    show_localisat
+00002290: 696f 6e73 203d 2054 7275 650d 0a0d 0a20  ions = True.... 
+000022a0: 2020 2020 2020 2020 2020 2069 6620 7368             if sh
+000022b0: 6f77 5f6c 6f63 616c 6973 6174 696f 6e73  ow_localisations
+000022c0: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
+000022d0: 2020 2020 206c 6179 6572 5f6e 616d 6573       layer_names
+000022e0: 203d 205b 6c61 7965 722e 6e61 6d65 2066   = [layer.name f
+000022f0: 6f72 206c 6179 6572 2069 6e20 7365 6c66  or layer in self
+00002300: 2e76 6965 7765 722e 6c61 7965 7273 5d0d  .viewer.layers].
+00002310: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00002320: 2020 2061 6374 6976 655f 6672 616d 6520     active_frame 
+00002330: 3d20 7365 6c66 2e76 6965 7765 722e 6469  = self.viewer.di
+00002340: 6d73 2e63 7572 7265 6e74 5f73 7465 705b  ms.current_step[
+00002350: 305d 0d0a 0d0a 2020 2020 2020 2020 2020  0]....          
+00002360: 2020 2020 2020 6461 7461 7365 745f 6e61        dataset_na
+00002370: 6d65 203d 2073 656c 662e 6775 692e 6d6f  me = self.gui.mo
+00002380: 6c74 7261 636b 5f64 6174 6173 6574 5f73  ltrack_dataset_s
+00002390: 656c 6563 746f 722e 6375 7272 656e 7454  elector.currentT
+000023a0: 6578 7428 290d 0a0d 0a20 2020 2020 2020  ext()....       
+000023b0: 2020 2020 2020 2020 2069 6620 6461 7461           if data
+000023c0: 7365 745f 6e61 6d65 2069 6e20 7365 6c66  set_name in self
+000023d0: 2e6c 6f63 616c 6973 6174 696f 6e5f 6469  .localisation_di
+000023e0: 6374 2e6b 6579 7328 293a 0d0a 2020 2020  ct.keys():..    
 000023f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002400: 2076 6973 5f73 697a 6520 3d20 666c 6f61   vis_size = floa
-00002410: 7428 7365 6c66 2e67 7569 2e70 6963 6173  t(self.gui.picas
-00002420: 736f 5f76 6973 5f73 697a 652e 6375 7272  so_vis_size.curr
-00002430: 656e 7454 6578 7428 2929 0d0a 2020 2020  entText())..    
-00002440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002450: 2020 2020 2020 2020 7669 735f 6f70 6163          vis_opac
-00002460: 6974 7920 3d20 666c 6f61 7428 7365 6c66  ity = float(self
-00002470: 2e67 7569 2e70 6963 6173 736f 5f76 6973  .gui.picasso_vis
-00002480: 5f6f 7061 6369 7479 2e63 7572 7265 6e74  _opacity.current
-00002490: 5465 7874 2829 290d 0a20 2020 2020 2020  Text())..       
-000024a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024b0: 2020 2020 2076 6973 5f65 6467 655f 7769       vis_edge_wi
-000024c0: 6474 6820 3d20 666c 6f61 7428 7365 6c66  dth = float(self
-000024d0: 2e67 7569 2e70 6963 6173 736f 5f76 6973  .gui.picasso_vis
-000024e0: 5f65 6467 655f 7769 6474 682e 6375 7272  _edge_width.curr
-000024f0: 656e 7454 6578 7428 2929 0d0a 0d0a 2020  entText())....  
-00002500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002510: 2020 2020 2020 2020 2020 6966 2076 6973            if vis
-00002520: 5f6d 6f64 652e 6c6f 7765 7228 2920 3d3d  _mode.lower() ==
-00002530: 2022 7371 7561 7265 223a 0d0a 2020 2020   "square":..    
-00002540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002550: 2020 2020 2020 2020 2020 2020 7379 6d62              symb
-00002560: 6f6c 203d 2022 7371 7561 7265 220d 0a20  ol = "square".. 
-00002570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002580: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00002590: 7669 735f 6d6f 6465 2e6c 6f77 6572 2829  vis_mode.lower()
-000025a0: 203d 3d20 2264 6973 6b22 3a0d 0a20 2020   == "disk":..   
-000025b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025c0: 2020 2020 2020 2020 2020 2020 2073 796d               sym
-000025d0: 626f 6c20 3d20 2264 6973 6322 0d0a 2020  bol = "disc"..  
-000025e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025f0: 2020 2020 2020 2020 2020 656c 6966 2076            elif v
-00002600: 6973 5f6d 6f64 652e 6c6f 7765 7228 2920  is_mode.lower() 
-00002610: 3d3d 2022 7822 3a0d 0a20 2020 2020 2020  == "x":..       
-00002620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002630: 2020 2020 2020 2020 2073 796d 626f 6c20           symbol 
-00002640: 3d20 2263 726f 7373 220d 0a0d 0a20 2020  = "cross"....   
-00002650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002660: 2020 2020 2020 2020 2072 656d 6f76 655f           remove_
-00002670: 6c6f 6361 6c69 7361 7469 6f6e 7320 3d20  localisations = 
-00002680: 4661 6c73 650d 0a0d 0a20 2020 2020 2020  False....       
-00002690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026a0: 2020 2020 2069 6620 226c 6f63 616c 6973       if "localis
-000026b0: 6174 696f 6e73 2220 6e6f 7420 696e 206c  ations" not in l
-000026c0: 6179 6572 5f6e 616d 6573 3a0d 0a20 2020  ayer_names:..   
-000026d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000026f0: 7365 6c66 2e76 6572 626f 7365 3a0d 0a20  self.verbose:.. 
-00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002720: 2020 2070 7269 6e74 2822 4472 6177 696e     print("Drawin
-00002730: 6720 6c6f 6361 6c69 7361 7469 6f6e 7322  g localisations"
-00002740: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00002750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002760: 2020 2020 2073 656c 662e 6c6f 635f 6c61       self.loc_la
-00002770: 7965 7220 3d20 7365 6c66 2e76 6965 7765  yer = self.viewe
-00002780: 722e 6164 645f 706f 696e 7473 2872 656e  r.add_points(ren
-00002790: 6465 725f 6c6f 6373 2c0d 0a20 2020 2020  der_locs,..     
-000027a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027b0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000027c0: 6469 6d3d 322c 2065 6467 655f 636f 6c6f  dim=2, edge_colo
-000027d0: 723d 2272 6564 222c 2066 6163 655f 636f  r="red", face_co
-000027e0: 6c6f 723d 5b30 2c20 302c 2030 2c20 305d  lor=[0, 0, 0, 0]
-000027f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00002400: 6c6f 6361 6c69 7361 7469 6f6e 5f64 6963  localisation_dic
+00002410: 7420 3d20 7365 6c66 2e6c 6f63 616c 6973  t = self.localis
+00002420: 6174 696f 6e5f 6469 6374 5b64 6174 6173  ation_dict[datas
+00002430: 6574 5f6e 616d 655d 2e63 6f70 7928 290d  et_name].copy().
+00002440: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00002450: 2020 2020 2020 2069 6620 226c 6f63 616c         if "local
+00002460: 6973 6174 696f 6e73 2220 696e 206c 6f63  isations" in loc
+00002470: 616c 6973 6174 696f 6e5f 6469 6374 2e6b  alisation_dict.k
+00002480: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
+00002490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024a0: 6c6f 6373 203d 206c 6f63 616c 6973 6174  locs = localisat
+000024b0: 696f 6e5f 6469 6374 5b22 6c6f 6361 6c69  ion_dict["locali
+000024c0: 7361 7469 6f6e 7322 5d0d 0a0d 0a20 2020  sations"]....   
+000024d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024e0: 2020 2020 2069 6620 6163 7469 7665 5f66       if active_f
+000024f0: 7261 6d65 2069 6e20 6c6f 6373 2e66 7261  rame in locs.fra
+00002500: 6d65 3a0d 0a20 2020 2020 2020 2020 2020  me:..           
+00002510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002520: 2066 7261 6d65 5f6c 6f63 7320 3d20 6c6f   frame_locs = lo
+00002530: 6373 5b6c 6f63 732e 6672 616d 6520 3d3d  cs[locs.frame ==
+00002540: 2061 6374 6976 655f 6672 616d 655d 2e63   active_frame].c
+00002550: 6f70 7928 290d 0a20 2020 2020 2020 2020  opy()..         
+00002560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002570: 2020 2072 656e 6465 725f 6c6f 6373 203d     render_locs =
+00002580: 206e 702e 7673 7461 636b 2828 6672 616d   np.vstack((fram
+00002590: 655f 6c6f 6373 2e79 2c20 6672 616d 655f  e_locs.y, frame_
+000025a0: 6c6f 6373 2e78 2929 2e54 2e74 6f6c 6973  locs.x)).T.tolis
+000025b0: 7428 290d 0a0d 0a20 2020 2020 2020 2020  t()....         
+000025c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025d0: 2020 2076 6973 5f6d 6f64 6520 3d20 7365     vis_mode = se
+000025e0: 6c66 2e67 7569 2e70 6963 6173 736f 5f76  lf.gui.picasso_v
+000025f0: 6973 5f6d 6f64 652e 6375 7272 656e 7454  is_mode.currentT
+00002600: 6578 7428 290d 0a20 2020 2020 2020 2020  ext()..         
+00002610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002620: 2020 2076 6973 5f73 697a 6520 3d20 666c     vis_size = fl
+00002630: 6f61 7428 7365 6c66 2e67 7569 2e70 6963  oat(self.gui.pic
+00002640: 6173 736f 5f76 6973 5f73 697a 652e 6375  asso_vis_size.cu
+00002650: 7272 656e 7454 6578 7428 2929 0d0a 2020  rrentText())..  
+00002660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002670: 2020 2020 2020 2020 2020 7669 735f 6f70            vis_op
+00002680: 6163 6974 7920 3d20 666c 6f61 7428 7365  acity = float(se
+00002690: 6c66 2e67 7569 2e70 6963 6173 736f 5f76  lf.gui.picasso_v
+000026a0: 6973 5f6f 7061 6369 7479 2e63 7572 7265  is_opacity.curre
+000026b0: 6e74 5465 7874 2829 290d 0a20 2020 2020  ntText())..     
+000026c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026d0: 2020 2020 2020 2076 6973 5f65 6467 655f         vis_edge_
+000026e0: 7769 6474 6820 3d20 666c 6f61 7428 7365  width = float(se
+000026f0: 6c66 2e67 7569 2e70 6963 6173 736f 5f76  lf.gui.picasso_v
+00002700: 6973 5f65 6467 655f 7769 6474 682e 6375  is_edge_width.cu
+00002710: 7272 656e 7454 6578 7428 2929 0d0a 0d0a  rrentText())....
+00002720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002730: 2020 2020 2020 2020 2020 2020 6966 2076              if v
+00002740: 6973 5f6d 6f64 652e 6c6f 7765 7228 2920  is_mode.lower() 
+00002750: 3d3d 2022 7371 7561 7265 223a 0d0a 2020  == "square":..  
+00002760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002770: 2020 2020 2020 2020 2020 2020 2020 7379                sy
+00002780: 6d62 6f6c 203d 2022 7371 7561 7265 220d  mbol = "square".
+00002790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000027a0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+000027b0: 6620 7669 735f 6d6f 6465 2e6c 6f77 6572  f vis_mode.lower
+000027c0: 2829 203d 3d20 2264 6973 6b22 3a0d 0a20  () == "disk":.. 
+000027d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000027f0: 796d 626f 6c20 3d20 2264 6973 6322 0d0a  ymbol = "disc"..
 00002800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002810: 2020 2020 2020 206f 7061 6369 7479 3d76         opacity=v
-00002820: 6973 5f6f 7061 6369 7479 2c20 6e61 6d65  is_opacity, name
-00002830: 3d22 6c6f 6361 6c69 7361 7469 6f6e 7322  ="localisations"
-00002840: 2c20 7379 6d62 6f6c 3d73 796d 626f 6c2c  , symbol=symbol,
-00002850: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002870: 2020 2020 2020 7369 7a65 3d76 6973 5f73        size=vis_s
-00002880: 697a 652c 2065 6467 655f 7769 6474 683d  ize, edge_width=
-00002890: 7669 735f 6564 6765 5f77 6964 7468 2c20  vis_edge_width, 
-000028a0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00002810: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00002820: 2076 6973 5f6d 6f64 652e 6c6f 7765 7228   vis_mode.lower(
+00002830: 2920 3d3d 2022 7822 3a0d 0a20 2020 2020  ) == "x":..     
+00002840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002850: 2020 2020 2020 2020 2020 2073 796d 626f             symbo
+00002860: 6c20 3d20 2263 726f 7373 220d 0a0d 0a20  l = "cross".... 
+00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002880: 2020 2020 2020 2020 2020 2072 656d 6f76             remov
+00002890: 655f 6c6f 6361 6c69 7361 7469 6f6e 7320  e_localisations 
+000028a0: 3d20 4661 6c73 650d 0a0d 0a20 2020 2020  = False....     
 000028b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028c0: 2020 2020 2075 7064 6174 655f 7669 7320       update_vis 
-000028d0: 3d20 5472 7565 0d0a 0d0a 2020 2020 2020  = True....      
-000028e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028f0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00002900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002910: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00002920: 7365 6c66 2e76 6572 626f 7365 3a0d 0a20  self.verbose:.. 
+000028c0: 2020 2020 2020 2069 6620 226c 6f63 616c         if "local
+000028d0: 6973 6174 696f 6e73 2220 6e6f 7420 696e  isations" not in
+000028e0: 206c 6179 6572 5f6e 616d 6573 3a0d 0a20   layer_names:.. 
+000028f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002900: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00002910: 6620 7365 6c66 2e76 6572 626f 7365 3a0d  f self.verbose:.
+00002920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00002930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002950: 2020 2070 7269 6e74 2822 5570 6461 7469     print("Updati
-00002960: 6e67 2066 6964 7563 6961 6c20 6461 7461  ng fiducial data
-00002970: 2229 0d0a 0d0a 2020 2020 2020 2020 2020  ")....          
-00002980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002990: 2020 2020 2020 7365 6c66 2e6c 6f63 5f6c        self.loc_l
-000029a0: 6179 6572 2e64 6174 6120 3d20 7265 6e64  ayer.data = rend
-000029b0: 6572 5f6c 6f63 730d 0a20 2020 2020 2020  er_locs..       
+00002940: 2020 2020 2070 7269 6e74 2822 4472 6177       print("Draw
+00002950: 696e 6720 6c6f 6361 6c69 7361 7469 6f6e  ing localisation
+00002960: 7322 290d 0a0d 0a20 2020 2020 2020 2020  s")....         
+00002970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002980: 2020 2020 2020 2073 656c 662e 6c6f 635f         self.loc_
+00002990: 6c61 7965 7220 3d20 7365 6c66 2e76 6965  layer = self.vie
+000029a0: 7765 722e 6164 645f 706f 696e 7473 2872  wer.add_points(r
+000029b0: 656e 6465 725f 6c6f 6373 2c0d 0a20 2020  ender_locs,..   
 000029c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029d0: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
-000029e0: 635f 6c61 7965 722e 7365 6c65 6374 6564  c_layer.selected
-000029f0: 5f64 6174 6120 3d20 5b5d 0d0a 0d0a 2020  _data = []....  
-00002a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a10: 2020 2020 2020 2020 2020 6966 2075 7064            if upd
-00002a20: 6174 655f 7669 733a 0d0a 2020 2020 2020  ate_vis:..      
-00002a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a40: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00002a50: 662e 7665 7262 6f73 653a 0d0a 2020 2020  f.verbose:..    
-00002a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a80: 7072 696e 7428 2255 7064 6174 696e 6720  print("Updating 
-00002a90: 6669 6475 6369 616c 2076 6973 7561 6c69  fiducial visuali
-00002aa0: 7361 7469 6f6e 2073 6574 7469 6e67 7322  sation settings"
-00002ab0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00002ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ad0: 2020 2020 2073 656c 662e 6c6f 635f 6c61       self.loc_la
-00002ae0: 7965 722e 7365 6c65 6374 6564 5f64 6174  yer.selected_dat
-00002af0: 6120 3d20 6c69 7374 2872 616e 6765 286c  a = list(range(l
-00002b00: 656e 2873 656c 662e 6c6f 635f 6c61 7965  en(self.loc_laye
-00002b10: 722e 6461 7461 2929 290d 0a20 2020 2020  r.data)))..     
+000029d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029e0: 206e 6469 6d3d 322c 2065 6467 655f 636f   ndim=2, edge_co
+000029f0: 6c6f 723d 2272 6564 222c 2066 6163 655f  lor="red", face_
+00002a00: 636f 6c6f 723d 5b30 2c20 302c 2030 2c20  color=[0, 0, 0, 
+00002a10: 305d 2c0d 0a20 2020 2020 2020 2020 2020  0],..           
+00002a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a30: 2020 2020 2020 2020 206f 7061 6369 7479           opacity
+00002a40: 3d76 6973 5f6f 7061 6369 7479 2c20 6e61  =vis_opacity, na
+00002a50: 6d65 3d22 6c6f 6361 6c69 7361 7469 6f6e  me="localisation
+00002a60: 7322 2c20 7379 6d62 6f6c 3d73 796d 626f  s", symbol=symbo
+00002a70: 6c2c 0d0a 2020 2020 2020 2020 2020 2020  l,..            
+00002a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a90: 2020 2020 2020 2020 7369 7a65 3d76 6973          size=vis
+00002aa0: 5f73 697a 652c 2065 6467 655f 7769 6474  _size, edge_widt
+00002ab0: 683d 7669 735f 6564 6765 5f77 6964 7468  h=vis_edge_width
+00002ac0: 2c20 290d 0a0d 0a20 2020 2020 2020 2020  , )....         
+00002ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ae0: 2020 2020 2020 2075 7064 6174 655f 7669         update_vi
+00002af0: 7320 3d20 5472 7565 0d0a 0d0a 2020 2020  s = True....    
+00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b10: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
 00002b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00002b40: 6c6f 635f 6c61 7965 722e 6f70 6163 6974  loc_layer.opacit
-00002b50: 7920 3d20 7669 735f 6f70 6163 6974 790d  y = vis_opacity.
-00002b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b80: 2073 656c 662e 6c6f 635f 6c61 7965 722e   self.loc_layer.
-00002b90: 7379 6d62 6f6c 203d 2073 796d 626f 6c0d  symbol = symbol.
-00002ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bc0: 2073 656c 662e 6c6f 635f 6c61 7965 722e   self.loc_layer.
-00002bd0: 7369 7a65 203d 2076 6973 5f73 697a 650d  size = vis_size.
-00002be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c00: 2073 656c 662e 6c6f 635f 6c61 7965 722e   self.loc_layer.
-00002c10: 6564 6765 5f77 6964 7468 203d 2076 6973  edge_width = vis
-00002c20: 5f65 6467 655f 7769 6474 680d 0a20 2020  _edge_width..   
-00002c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00002c50: 662e 6c6f 635f 6c61 7965 722e 6564 6765  f.loc_layer.edge
-00002c60: 5f63 6f6c 6f72 203d 2022 7265 6422 0d0a  _color = "red"..
-00002c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b30: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00002b40: 6620 7365 6c66 2e76 6572 626f 7365 3a0d  f self.verbose:.
+00002b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b70: 2020 2020 2070 7269 6e74 2822 5570 6461       print("Upda
+00002b80: 7469 6e67 2066 6964 7563 6961 6c20 6461  ting fiducial da
+00002b90: 7461 2229 0d0a 0d0a 2020 2020 2020 2020  ta")....        
+00002ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bb0: 2020 2020 2020 2020 7365 6c66 2e6c 6f63          self.loc
+00002bc0: 5f6c 6179 6572 2e64 6174 6120 3d20 7265  _layer.data = re
+00002bd0: 6e64 6572 5f6c 6f63 730d 0a20 2020 2020  nder_locs..     
+00002be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002c00: 6c6f 635f 6c61 7965 722e 7365 6c65 6374  loc_layer.select
+00002c10: 6564 5f64 6174 6120 3d20 5b5d 0d0a 0d0a  ed_data = []....
+00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c30: 2020 2020 2020 2020 2020 2020 6966 2075              if u
+00002c40: 7064 6174 655f 7669 733a 0d0a 2020 2020  pdate_vis:..    
+00002c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c60: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00002c70: 656c 662e 7665 7262 6f73 653a 0d0a 2020  elf.verbose:..  
 00002c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c90: 7365 6c66 2e6c 6f63 5f6c 6179 6572 2e73  self.loc_layer.s
-00002ca0: 656c 6563 7465 645f 6461 7461 203d 205b  elected_data = [
-00002cb0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00002cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cd0: 2020 2073 656c 662e 6c6f 635f 6c61 7965     self.loc_laye
-00002ce0: 722e 7265 6672 6573 6828 290d 0a0d 0a20  r.refresh().... 
-00002cf0: 2020 2020 2020 2020 2020 2069 6620 7265             if re
-00002d00: 6d6f 7665 5f6c 6f63 616c 6973 6174 696f  move_localisatio
-00002d10: 6e73 3a0d 0a20 2020 2020 2020 2020 2020  ns:..           
-00002d20: 2020 2020 2069 6620 226c 6f63 616c 6973       if "localis
-00002d30: 6174 696f 6e73 2220 696e 206c 6179 6572  ations" in layer
-00002d40: 5f6e 616d 6573 3a0d 0a20 2020 2020 2020  _names:..       
+00002c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ca0: 2020 7072 696e 7428 2255 7064 6174 696e    print("Updatin
+00002cb0: 6720 6669 6475 6369 616c 2076 6973 7561  g fiducial visua
+00002cc0: 6c69 7361 7469 6f6e 2073 6574 7469 6e67  lisation setting
+00002cd0: 7322 290d 0a0d 0a20 2020 2020 2020 2020  s")....         
+00002ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cf0: 2020 2020 2020 2073 656c 662e 6c6f 635f         self.loc_
+00002d00: 6c61 7965 722e 7365 6c65 6374 6564 5f64  layer.selected_d
+00002d10: 6174 6120 3d20 6c69 7374 2872 616e 6765  ata = list(range
+00002d20: 286c 656e 2873 656c 662e 6c6f 635f 6c61  (len(self.loc_la
+00002d30: 7965 722e 6461 7461 2929 290d 0a20 2020  yer.data)))..   
+00002d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002d50: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00002d60: 662e 7669 6577 6572 2e6c 6179 6572 735b  f.viewer.layers[
-00002d70: 226c 6f63 616c 6973 6174 696f 6e73 225d  "localisations"]
-00002d80: 2e64 6174 6120 3d20 5b5d 0d0a 0d0a 2020  .data = []....  
-00002d90: 2020 2020 2020 2020 2020 666f 7220 6c61            for la
-00002da0: 7965 7220 696e 206c 6179 6572 5f6e 616d  yer in layer_nam
-00002db0: 6573 3a0d 0a20 2020 2020 2020 2020 2020  es:..           
-00002dc0: 2020 2020 2073 656c 662e 7669 6577 6572       self.viewer
-00002dd0: 2e6c 6179 6572 735b 6c61 7965 725d 2e72  .layers[layer].r
-00002de0: 6566 7265 7368 2829 0d0a 0d0a 2020 2020  efresh()....    
-00002df0: 6465 6620 636c 6561 725f 6c69 7665 5f69  def clear_live_i
-00002e00: 6d61 6765 7328 7365 6c66 293a 0d0a 0d0a  mages(self):....
-00002e10: 2020 2020 2020 2020 7472 793a 0d0a 0d0a          try:....
-00002e20: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00002e30: 656c 662e 7665 7262 6f73 653a 0d0a 2020  elf.verbose:..  
-00002e40: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00002e50: 696e 7428 2243 6c65 6172 696e 6720 6c69  int("Clearing li
-00002e60: 7665 2069 6d61 6765 7322 290d 0a0d 0a20  ve images").... 
-00002e70: 2020 2020 2020 2020 2020 2069 6d61 6765             image
-00002e80: 5f6c 6179 6572 7320 3d20 5b6c 6179 6572  _layers = [layer
-00002e90: 2066 6f72 206c 6179 6572 2069 6e20 7365   for layer in se
-00002ea0: 6c66 2e76 6965 7765 722e 6c61 7965 7273  lf.viewer.layers
-00002eb0: 2069 6620 6973 696e 7374 616e 6365 286c   if isinstance(l
-00002ec0: 6179 6572 2c20 6e61 7061 7269 2e6c 6179  ayer, napari.lay
-00002ed0: 6572 732e 496d 6167 6529 5d0d 0a0d 0a20  ers.Image)].... 
-00002ee0: 2020 2020 2020 2020 2020 2066 6f72 206c             for l
-00002ef0: 6179 6572 2069 6e20 696d 6167 655f 6c61  ayer in image_la
-00002f00: 7965 7273 3a0d 0a0d 0a20 2020 2020 2020  yers:....       
-00002f10: 2020 2020 2020 2020 2066 7261 6d65 5f73           frame_s
-00002f20: 6861 7065 203d 206c 6179 6572 2e64 6174  hape = layer.dat
-00002f30: 612e 7368 6170 655b 313a 5d0d 0a20 2020  a.shape[1:]..   
-00002f40: 2020 2020 2020 2020 2020 2020 2065 6d70               emp
-00002f50: 7479 5f66 7261 6d65 203d 206e 702e 7a65  ty_frame = np.ze
-00002f60: 726f 7328 6672 616d 655f 7368 6170 652c  ros(frame_shape,
-00002f70: 2064 7479 7065 3d6c 6179 6572 2e64 6174   dtype=layer.dat
-00002f80: 612e 6474 7970 6529 0d0a 2020 2020 2020  a.dtype)..      
-00002f90: 2020 2020 2020 2020 2020 6c61 7965 722e            layer.
-00002fa0: 6461 7461 203d 2065 6d70 7479 5f66 7261  data = empty_fra
-00002fb0: 6d65 0d0a 0d0a 2020 2020 2020 2020 6578  me....        ex
-00002fc0: 6365 7074 3a0d 0a20 2020 2020 2020 2020  cept:..         
-00002fd0: 2020 2070 7269 6e74 2874 7261 6365 6261     print(traceba
-00002fe0: 636b 2e66 6f72 6d61 745f 6578 6328 2929  ck.format_exc())
-00002ff0: 0d0a 2020 2020 2020 2020 2020 2020 7061  ..            pa
-00003000: 7373 0d0a 0d0a 2020 2020 6465 6620 7570  ss....    def up
-00003010: 6461 7465 5f64 6574 6563 745f 6f70 7469  date_detect_opti
-00003020: 6f6e 7328 7365 6c66 2c20 6576 656e 743d  ons(self, event=
-00003030: 4e6f 6e65 293a 0d0a 0d0a 2020 2020 2020  None):....      
-00003040: 2020 6966 2073 656c 662e 6775 692e 736d    if self.gui.sm
-00003050: 6c6d 5f64 6574 6563 745f 6d6f 6465 2e63  lm_detect_mode.c
-00003060: 7572 7265 6e74 5465 7874 2829 203d 3d20  urrentText() == 
-00003070: 2250 6963 6173 736f 223a 0d0a 0d0a 2020  "Picasso":....  
-00003080: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
-00003090: 7569 2e70 6963 6173 736f 5f62 6f78 5f73  ui.picasso_box_s
-000030a0: 697a 655f 6c61 6265 6c2e 7368 6f77 2829  ize_label.show()
-000030b0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-000030c0: 6c66 2e67 7569 2e70 6963 6173 736f 5f62  lf.gui.picasso_b
-000030d0: 6f78 5f73 697a 652e 7368 6f77 2829 0d0a  ox_size.show()..
-000030e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000030f0: 2e67 7569 2e70 6963 6173 736f 5f6d 696e  .gui.picasso_min
-00003100: 5f6e 6574 5f67 7261 6469 656e 745f 6c61  _net_gradient_la
-00003110: 6265 6c2e 7368 6f77 2829 0d0a 2020 2020  bel.show()..    
-00003120: 2020 2020 2020 2020 7365 6c66 2e67 7569          self.gui
-00003130: 2e70 6963 6173 736f 5f6d 696e 5f6e 6574  .picasso_min_net
-00003140: 5f67 7261 6469 656e 742e 7368 6f77 2829  _gradient.show()
-00003150: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00003160: 7365 6c66 2e67 7569 2e73 746f 726d 7472  self.gui.stormtr
-00003170: 6163 6b65 725f 7468 7265 7368 6f6c 645f  acker_threshold_
-00003180: 6c61 6265 6c2e 6869 6465 2829 0d0a 2020  label.hide()..  
-00003190: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
-000031a0: 7569 2e73 746f 726d 7472 6163 6b65 725f  ui.stormtracker_
-000031b0: 7468 7265 7368 6f6c 642e 6869 6465 2829  threshold.hide()
-000031c0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-000031d0: 6c66 2e67 7569 2e73 746f 726d 7472 6163  lf.gui.stormtrac
-000031e0: 6b65 725f 7769 6e64 6f77 5f73 697a 655f  ker_window_size_
-000031f0: 6c61 6265 6c2e 6869 6465 2829 0d0a 2020  label.hide()..  
-00003200: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
-00003210: 7569 2e73 746f 726d 7472 6163 6b65 725f  ui.stormtracker_
-00003220: 7769 6e64 6f77 5f73 697a 652e 6869 6465  window_size.hide
-00003230: 2829 0d0a 0d0a 2020 2020 2020 2020 656c  ()....        el
-00003240: 7365 3a0d 0a0d 0a20 2020 2020 2020 2020  se:....         
-00003250: 2020 2073 656c 662e 6775 692e 7069 6361     self.gui.pica
-00003260: 7373 6f5f 626f 785f 7369 7a65 5f6c 6162  sso_box_size_lab
-00003270: 656c 2e68 6964 6528 290d 0a20 2020 2020  el.hide()..     
-00003280: 2020 2020 2020 2073 656c 662e 6775 692e         self.gui.
-00003290: 7069 6361 7373 6f5f 626f 785f 7369 7a65  picasso_box_size
-000032a0: 2e68 6964 6528 290d 0a20 2020 2020 2020  .hide()..       
-000032b0: 2020 2020 2073 656c 662e 6775 692e 7069       self.gui.pi
-000032c0: 6361 7373 6f5f 6d69 6e5f 6e65 745f 6772  casso_min_net_gr
-000032d0: 6164 6965 6e74 5f6c 6162 656c 2e68 6964  adient_label.hid
-000032e0: 6528 290d 0a20 2020 2020 2020 2020 2020  e()..           
-000032f0: 2073 656c 662e 6775 692e 7069 6361 7373   self.gui.picass
-00003300: 6f5f 6d69 6e5f 6e65 745f 6772 6164 6965  o_min_net_gradie
-00003310: 6e74 2e68 6964 6528 290d 0a0d 0a20 2020  nt.hide()....   
-00003320: 2020 2020 2020 2020 2073 656c 662e 6775           self.gu
-00003330: 692e 7374 6f72 6d74 7261 636b 6572 5f74  i.stormtracker_t
-00003340: 6872 6573 686f 6c64 5f6c 6162 656c 2e73  hreshold_label.s
-00003350: 686f 7728 290d 0a20 2020 2020 2020 2020  how()..         
-00003360: 2020 2073 656c 662e 6775 692e 7374 6f72     self.gui.stor
-00003370: 6d74 7261 636b 6572 5f74 6872 6573 686f  mtracker_thresho
-00003380: 6c64 2e73 686f 7728 290d 0a20 2020 2020  ld.show()..     
-00003390: 2020 2020 2020 2073 656c 662e 6775 692e         self.gui.
-000033a0: 7374 6f72 6d74 7261 636b 6572 5f77 696e  stormtracker_win
-000033b0: 646f 775f 7369 7a65 5f6c 6162 656c 2e73  dow_size_label.s
-000033c0: 686f 7728 290d 0a20 2020 2020 2020 2020  how()..         
-000033d0: 2020 2073 656c 662e 6775 692e 7374 6f72     self.gui.stor
-000033e0: 6d74 7261 636b 6572 5f77 696e 646f 775f  mtracker_window_
-000033f0: 7369 7a65 2e73 686f 7728 290d 0a0d 0a    size.show()....
+00002d60: 662e 6c6f 635f 6c61 7965 722e 6f70 6163  f.loc_layer.opac
+00002d70: 6974 7920 3d20 7669 735f 6f70 6163 6974  ity = vis_opacit
+00002d80: 790d 0a20 2020 2020 2020 2020 2020 2020  y..             
+00002d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002da0: 2020 2073 656c 662e 6c6f 635f 6c61 7965     self.loc_laye
+00002db0: 722e 7379 6d62 6f6c 203d 2073 796d 626f  r.symbol = symbo
+00002dc0: 6c0d 0a20 2020 2020 2020 2020 2020 2020  l..             
+00002dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002de0: 2020 2073 656c 662e 6c6f 635f 6c61 7965     self.loc_laye
+00002df0: 722e 7369 7a65 203d 2076 6973 5f73 697a  r.size = vis_siz
+00002e00: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+00002e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e20: 2020 2073 656c 662e 6c6f 635f 6c61 7965     self.loc_laye
+00002e30: 722e 6564 6765 5f77 6964 7468 203d 2076  r.edge_width = v
+00002e40: 6973 5f65 6467 655f 7769 6474 680d 0a20  is_edge_width.. 
+00002e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00002e70: 656c 662e 6c6f 635f 6c61 7965 722e 6564  elf.loc_layer.ed
+00002e80: 6765 5f63 6f6c 6f72 203d 2022 7265 6422  ge_color = "red"
+00002e90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002eb0: 2020 7365 6c66 2e6c 6f63 5f6c 6179 6572    self.loc_layer
+00002ec0: 2e73 656c 6563 7465 645f 6461 7461 203d  .selected_data =
+00002ed0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00002ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ef0: 2020 2020 2073 656c 662e 6c6f 635f 6c61       self.loc_la
+00002f00: 7965 722e 7265 6672 6573 6828 290d 0a0d  yer.refresh()...
+00002f10: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00002f20: 7265 6d6f 7665 5f6c 6f63 616c 6973 6174  remove_localisat
+00002f30: 696f 6e73 3a0d 0a20 2020 2020 2020 2020  ions:..         
+00002f40: 2020 2020 2020 2069 6620 226c 6f63 616c         if "local
+00002f50: 6973 6174 696f 6e73 2220 696e 206c 6179  isations" in lay
+00002f60: 6572 5f6e 616d 6573 3a0d 0a20 2020 2020  er_names:..     
+00002f70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00002f80: 656c 662e 7669 6577 6572 2e6c 6179 6572  elf.viewer.layer
+00002f90: 735b 226c 6f63 616c 6973 6174 696f 6e73  s["localisations
+00002fa0: 225d 2e64 6174 6120 3d20 5b5d 0d0a 0d0a  "].data = []....
+00002fb0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00002fc0: 6c61 7965 7220 696e 206c 6179 6572 5f6e  layer in layer_n
+00002fd0: 616d 6573 3a0d 0a20 2020 2020 2020 2020  ames:..         
+00002fe0: 2020 2020 2020 2073 656c 662e 7669 6577         self.view
+00002ff0: 6572 2e6c 6179 6572 735b 6c61 7965 725d  er.layers[layer]
+00003000: 2e72 6566 7265 7368 2829 0d0a 0d0a 2020  .refresh()....  
+00003010: 2020 6465 6620 636c 6561 725f 6c69 7665    def clear_live
+00003020: 5f69 6d61 6765 7328 7365 6c66 293a 0d0a  _images(self):..
+00003030: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
+00003040: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00003050: 2073 656c 662e 7665 7262 6f73 653a 0d0a   self.verbose:..
+00003060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003070: 7072 696e 7428 2243 6c65 6172 696e 6720  print("Clearing 
+00003080: 6c69 7665 2069 6d61 6765 7322 290d 0a0d  live images")...
+00003090: 0a20 2020 2020 2020 2020 2020 2069 6d61  .            ima
+000030a0: 6765 5f6c 6179 6572 7320 3d20 5b6c 6179  ge_layers = [lay
+000030b0: 6572 2066 6f72 206c 6179 6572 2069 6e20  er for layer in 
+000030c0: 7365 6c66 2e76 6965 7765 722e 6c61 7965  self.viewer.laye
+000030d0: 7273 2069 6620 6973 696e 7374 616e 6365  rs if isinstance
+000030e0: 286c 6179 6572 2c20 6e61 7061 7269 2e6c  (layer, napari.l
+000030f0: 6179 6572 732e 496d 6167 6529 5d0d 0a0d  ayers.Image)]...
+00003100: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00003110: 206c 6179 6572 2069 6e20 696d 6167 655f   layer in image_
+00003120: 6c61 7965 7273 3a0d 0a0d 0a20 2020 2020  layers:....     
+00003130: 2020 2020 2020 2020 2020 2066 7261 6d65             frame
+00003140: 5f73 6861 7065 203d 206c 6179 6572 2e64  _shape = layer.d
+00003150: 6174 612e 7368 6170 655b 313a 5d0d 0a20  ata.shape[1:].. 
+00003160: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00003170: 6d70 7479 5f66 7261 6d65 203d 206e 702e  mpty_frame = np.
+00003180: 7a65 726f 7328 6672 616d 655f 7368 6170  zeros(frame_shap
+00003190: 652c 2064 7479 7065 3d6c 6179 6572 2e64  e, dtype=layer.d
+000031a0: 6174 612e 6474 7970 6529 0d0a 2020 2020  ata.dtype)..    
+000031b0: 2020 2020 2020 2020 2020 2020 6c61 7965              laye
+000031c0: 722e 6461 7461 203d 2065 6d70 7479 5f66  r.data = empty_f
+000031d0: 7261 6d65 0d0a 0d0a 2020 2020 2020 2020  rame....        
+000031e0: 6578 6365 7074 3a0d 0a20 2020 2020 2020  except:..       
+000031f0: 2020 2020 2070 7269 6e74 2874 7261 6365       print(trace
+00003200: 6261 636b 2e66 6f72 6d61 745f 6578 6328  back.format_exc(
+00003210: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00003220: 7061 7373 0d0a 0d0a 2020 2020 6465 6620  pass....    def 
+00003230: 7570 6461 7465 5f64 6574 6563 745f 6f70  update_detect_op
+00003240: 7469 6f6e 7328 7365 6c66 2c20 6576 656e  tions(self, even
+00003250: 743d 4e6f 6e65 293a 0d0a 0d0a 2020 2020  t=None):....    
+00003260: 2020 2020 6966 2073 656c 662e 6775 692e      if self.gui.
+00003270: 736d 6c6d 5f64 6574 6563 745f 6d6f 6465  smlm_detect_mode
+00003280: 2e63 7572 7265 6e74 5465 7874 2829 203d  .currentText() =
+00003290: 3d20 2250 6963 6173 736f 223a 0d0a 0d0a  = "Picasso":....
+000032a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000032b0: 2e67 7569 2e70 6963 6173 736f 5f62 6f78  .gui.picasso_box
+000032c0: 5f73 697a 655f 6c61 6265 6c2e 7368 6f77  _size_label.show
+000032d0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+000032e0: 7365 6c66 2e67 7569 2e70 6963 6173 736f  self.gui.picasso
+000032f0: 5f62 6f78 5f73 697a 652e 7368 6f77 2829  _box_size.show()
+00003300: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00003310: 6c66 2e67 7569 2e70 6963 6173 736f 5f6d  lf.gui.picasso_m
+00003320: 696e 5f6e 6574 5f67 7261 6469 656e 745f  in_net_gradient_
+00003330: 6c61 6265 6c2e 7368 6f77 2829 0d0a 2020  label.show()..  
+00003340: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
+00003350: 7569 2e70 6963 6173 736f 5f6d 696e 5f6e  ui.picasso_min_n
+00003360: 6574 5f67 7261 6469 656e 742e 7368 6f77  et_gradient.show
+00003370: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
+00003380: 2020 7365 6c66 2e67 7569 2e73 746f 726d    self.gui.storm
+00003390: 7472 6163 6b65 725f 7468 7265 7368 6f6c  tracker_threshol
+000033a0: 645f 6c61 6265 6c2e 6869 6465 2829 0d0a  d_label.hide()..
+000033b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000033c0: 2e67 7569 2e73 746f 726d 7472 6163 6b65  .gui.stormtracke
+000033d0: 725f 7468 7265 7368 6f6c 642e 6869 6465  r_threshold.hide
+000033e0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+000033f0: 7365 6c66 2e67 7569 2e73 746f 726d 7472  self.gui.stormtr
+00003400: 6163 6b65 725f 7769 6e64 6f77 5f73 697a  acker_window_siz
+00003410: 655f 6c61 6265 6c2e 6869 6465 2829 0d0a  e_label.hide()..
+00003420: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003430: 2e67 7569 2e73 746f 726d 7472 6163 6b65  .gui.stormtracke
+00003440: 725f 7769 6e64 6f77 5f73 697a 652e 6869  r_window_size.hi
+00003450: 6465 2829 0d0a 0d0a 2020 2020 2020 2020  de()....        
+00003460: 656c 7365 3a0d 0a0d 0a20 2020 2020 2020  else:....       
+00003470: 2020 2020 2073 656c 662e 6775 692e 7069       self.gui.pi
+00003480: 6361 7373 6f5f 626f 785f 7369 7a65 5f6c  casso_box_size_l
+00003490: 6162 656c 2e68 6964 6528 290d 0a20 2020  abel.hide()..   
+000034a0: 2020 2020 2020 2020 2073 656c 662e 6775           self.gu
+000034b0: 692e 7069 6361 7373 6f5f 626f 785f 7369  i.picasso_box_si
+000034c0: 7a65 2e68 6964 6528 290d 0a20 2020 2020  ze.hide()..     
+000034d0: 2020 2020 2020 2073 656c 662e 6775 692e         self.gui.
+000034e0: 7069 6361 7373 6f5f 6d69 6e5f 6e65 745f  picasso_min_net_
+000034f0: 6772 6164 6965 6e74 5f6c 6162 656c 2e68  gradient_label.h
+00003500: 6964 6528 290d 0a20 2020 2020 2020 2020  ide()..         
+00003510: 2020 2073 656c 662e 6775 692e 7069 6361     self.gui.pica
+00003520: 7373 6f5f 6d69 6e5f 6e65 745f 6772 6164  sso_min_net_grad
+00003530: 6965 6e74 2e68 6964 6528 290d 0a0d 0a20  ient.hide().... 
+00003540: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003550: 6775 692e 7374 6f72 6d74 7261 636b 6572  gui.stormtracker
+00003560: 5f74 6872 6573 686f 6c64 5f6c 6162 656c  _threshold_label
+00003570: 2e73 686f 7728 290d 0a20 2020 2020 2020  .show()..       
+00003580: 2020 2020 2073 656c 662e 6775 692e 7374       self.gui.st
+00003590: 6f72 6d74 7261 636b 6572 5f74 6872 6573  ormtracker_thres
+000035a0: 686f 6c64 2e73 686f 7728 290d 0a20 2020  hold.show()..   
+000035b0: 2020 2020 2020 2020 2073 656c 662e 6775           self.gu
+000035c0: 692e 7374 6f72 6d74 7261 636b 6572 5f77  i.stormtracker_w
+000035d0: 696e 646f 775f 7369 7a65 5f6c 6162 656c  indow_size_label
+000035e0: 2e73 686f 7728 290d 0a20 2020 2020 2020  .show()..       
+000035f0: 2020 2020 2073 656c 662e 6775 692e 7374       self.gui.st
+00003600: 6f72 6d74 7261 636b 6572 5f77 696e 646f  ormtracker_windo
+00003610: 775f 7369 7a65 2e73 686f 7728 290d 0a0d  w_size.show()...
+00003620: 0a20 2020 2064 6566 206d 6f6c 7472 6163  .    def moltrac
+00003630: 745f 7472 616e 736c 6174 696f 6e28 7365  t_translation(se
+00003640: 6c66 2c20 6576 656e 7420 3d20 4e6f 6e65  lf, event = None
+00003650: 2c20 6469 7265 6374 696f 6e20 3d20 226c  , direction = "l
+00003660: 6566 7422 293a 0d0a 0d0a 2020 2020 2020  eft"):....      
+00003670: 2020 7472 793a 0d0a 0d0a 2020 2020 2020    try:....      
+00003680: 2020 2020 2020 7472 616e 736c 6174 696f        translatio
+00003690: 6e5f 7461 7267 6574 203d 2073 656c 662e  n_target = self.
+000036a0: 6775 692e 7472 616e 736c 6174 696f 6e5f  gui.translation_
+000036b0: 7461 7267 6574 2e63 7572 7265 6e74 5465  target.currentTe
+000036c0: 7874 2829 0d0a 2020 2020 2020 2020 2020  xt()..          
+000036d0: 2020 7369 7a65 203d 2073 656c 662e 6775    size = self.gu
+000036e0: 692e 7472 616e 736c 6174 696f 6e5f 7369  i.translation_si
+000036f0: 7a65 2e76 616c 7565 2829 0d0a 0d0a 2020  ze.value()....  
+00003700: 2020 2020 2020 2020 2020 6966 2064 6972            if dir
+00003710: 6563 7469 6f6e 203d 3d20 2275 7022 3a0d  ection == "up":.
+00003720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003730: 2073 6869 6674 5f76 6563 746f 7220 3d20   shift_vector = 
+00003740: 5b2d 7369 7a65 2c20 302e 305d 0d0a 2020  [-size, 0.0]..  
+00003750: 2020 2020 2020 2020 2020 656c 6966 2064            elif d
+00003760: 6972 6563 7469 6f6e 203d 3d20 2264 6f77  irection == "dow
+00003770: 6e22 3a0d 0a20 2020 2020 2020 2020 2020  n":..           
+00003780: 2020 2020 2073 6869 6674 5f76 6563 746f       shift_vecto
+00003790: 7220 3d20 5b73 697a 652c 2030 2e30 5d0d  r = [size, 0.0].
+000037a0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+000037b0: 6620 6469 7265 6374 696f 6e20 3d3d 2022  f direction == "
+000037c0: 6c65 6674 223a 0d0a 2020 2020 2020 2020  left":..        
+000037d0: 2020 2020 2020 2020 7368 6966 745f 7665          shift_ve
+000037e0: 6374 6f72 203d 205b 302e 302c 202d 7369  ctor = [0.0, -si
+000037f0: 7a65 5d0d 0a20 2020 2020 2020 2020 2020  ze]..           
+00003800: 2065 6c69 6620 6469 7265 6374 696f 6e20   elif direction 
+00003810: 3d3d 2022 7269 6768 7422 3a0d 0a20 2020  == "right":..   
+00003820: 2020 2020 2020 2020 2020 2020 2073 6869               shi
+00003830: 6674 5f76 6563 746f 7220 3d20 5b30 2e30  ft_vector = [0.0
+00003840: 2c20 7369 7a65 5d0d 0a0d 0a20 2020 2020  , size]....     
+00003850: 2020 2020 2020 2069 6620 7472 616e 736c         if transl
+00003860: 6174 696f 6e5f 7461 7267 6574 2069 6e20  ation_target in 
+00003870: 5b22 5365 676d 656e 7461 7469 6f6e 2049  ["Segmentation I
+00003880: 6d61 6765 222c 2022 426f 7468 225d 3a0d  mage", "Both"]:.
+00003890: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000038a0: 2020 2069 6620 6861 7361 7474 7228 7365     if hasattr(se
+000038b0: 6c66 2c20 2273 6567 6d65 6e74 6174 696f  lf, "segmentatio
+000038c0: 6e5f 696d 6167 6522 293a 0d0a 0d0a 2020  n_image"):....  
+000038d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038e0: 2020 696d 6167 6520 3d20 7365 6c66 2e73    image = self.s
+000038f0: 6567 6d65 6e74 6174 696f 6e5f 696d 6167  egmentation_imag
+00003900: 652e 636f 7079 2829 0d0a 0d0a 2020 2020  e.copy()....    
+00003910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003920: 6966 206c 656e 2869 6d61 6765 2e73 6861  if len(image.sha
+00003930: 7065 2920 3d3d 2032 3a0d 0a20 2020 2020  pe) == 2:..     
+00003940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003950: 2020 2069 6d61 6765 203d 2073 6869 6674     image = shift
+00003960: 2869 6d61 6765 2c20 7368 6966 743d 7368  (image, shift=sh
+00003970: 6966 745f 7665 6374 6f72 290d 0a20 2020  ift_vector)..   
+00003980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003990: 2020 2020 2073 656c 662e 7365 676d 656e       self.segmen
+000039a0: 7461 7469 6f6e 5f69 6d61 6765 203d 2069  tation_image = i
+000039b0: 6d61 6765 0d0a 0d0a 2020 2020 2020 2020  mage....        
+000039c0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000039d0: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
+000039e0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+000039f0: 2066 616d 655f 696e 6465 782c 2066 7261   fame_index, fra
+00003a00: 6d65 2069 6e20 656e 756d 6572 6174 6528  me in enumerate(
+00003a10: 696d 6167 6529 3a0d 0a20 2020 2020 2020  image):..       
+00003a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a30: 2020 2020 2069 6d61 6765 5b66 616d 655f       image[fame_
+00003a40: 696e 6465 785d 203d 2073 6869 6674 2866  index] = shift(f
+00003a50: 7261 6d65 2c20 7368 6966 743d 7368 6966  rame, shift=shif
+00003a60: 745f 7665 6374 6f72 290d 0a20 2020 2020  t_vector)..     
+00003a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a80: 2020 2073 656c 662e 7365 676d 656e 7461     self.segmenta
+00003a90: 7469 6f6e 5f69 6d61 6765 203d 2069 6d61  tion_image = ima
+00003aa0: 6765 0d0a 0d0a 2020 2020 2020 2020 2020  ge....          
+00003ab0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00003ac0: 7261 775f 7365 676d 656e 7461 7469 6f6e  raw_segmentation
+00003ad0: 5f69 6d61 6765 2829 0d0a 0d0a 2020 2020  _image()....    
+00003ae0: 2020 2020 2020 2020 6966 2074 7261 6e73          if trans
+00003af0: 6c61 7469 6f6e 5f74 6172 6765 7420 696e  lation_target in
+00003b00: 205b 2253 6567 6d65 6e74 6174 696f 6e73   ["Segmentations
+00003b10: 222c 2242 6f74 6822 5d3a 0d0a 0d0a 2020  ","Both"]:....  
+00003b20: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00003b30: 2068 6173 6174 7472 2873 656c 662c 2022   hasattr(self, "
+00003b40: 7365 674c 6179 6572 2229 3a0d 0a0d 0a20  segLayer"):.... 
+00003b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b60: 2020 2073 6567 5f64 6174 6120 3d20 7365     seg_data = se
+00003b70: 6c66 2e73 6567 4c61 7965 722e 6461 7461  lf.segLayer.data
+00003b80: 2e63 6f70 7928 290d 0a0d 0a20 2020 2020  .copy()....     
+00003b90: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00003ba0: 6f72 2073 6567 5f69 6e64 6578 2c20 7365  or seg_index, se
+00003bb0: 6720 696e 2065 6e75 6d65 7261 7465 2873  g in enumerate(s
+00003bc0: 6567 5f64 6174 6129 3a0d 0a0d 0a20 2020  eg_data):....   
+00003bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003be0: 2020 2020 2069 6620 7365 672e 7368 6170       if seg.shap
+00003bf0: 655b 315d 203d 3d20 323a 0d0a 2020 2020  e[1] == 2:..    
+00003c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c10: 2020 2020 2020 2020 7365 6720 3d20 7365          seg = se
+00003c20: 6720 2b20 7368 6966 745f 7665 6374 6f72  g + shift_vector
+00003c30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003c40: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003c50: 675f 6461 7461 5b73 6567 5f69 6e64 6578  g_data[seg_index
+00003c60: 5d20 3d20 7365 670d 0a20 2020 2020 2020  ] = seg..       
+00003c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c80: 2069 6620 7365 672e 7368 6170 655b 315d   if seg.shape[1]
+00003c90: 203d 3d20 333a 0d0a 2020 2020 2020 2020   == 3:..        
+00003ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003cb0: 2020 2020 7365 675b 3a2c 2031 3a5d 203d      seg[:, 1:] =
+00003cc0: 2073 6567 5b3a 2c20 313a 5d20 2b20 7368   seg[:, 1:] + sh
+00003cd0: 6966 745f 7665 6374 6f72 0d0a 2020 2020  ift_vector..    
+00003ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003cf0: 2020 2020 2020 2020 7365 675f 6461 7461          seg_data
+00003d00: 5b73 6567 5f69 6e64 6578 5d20 3d20 7365  [seg_index] = se
+00003d10: 670d 0a0d 0a0d 0a20 2020 2020 2020 2020  g......         
+00003d20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003d30: 7365 674c 6179 6572 2e64 6174 6120 3d20  segLayer.data = 
+00003d40: 7365 675f 6461 7461 0d0a 0d0a 0d0a 0d0a  seg_data........
+00003d50: 0d0a 0d0a 0d0a 0d0a 0d0a 0d0a 2020 2020  ............    
+00003d60: 2020 2020 6578 6365 7074 3a0d 0a20 2020      except:..   
+00003d70: 2020 2020 2020 2020 2070 7269 6e74 2874           print(t
+00003d80: 7261 6365 6261 636b 2e66 6f72 6d61 745f  raceback.format_
+00003d90: 6578 6328 2929                           exc())
```

### Comparing `napari_moltrack-0.0.3/src/moltrack/funcs/export_utils.py` & `napari_moltrack-0.0.4/src/moltrack/funcs/export_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.3/src/moltrack/funcs/import_utils.py` & `napari_moltrack-0.0.4/src/moltrack/funcs/import_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,104 +9,114 @@
 from multiprocessing import shared_memory, Manager
 from functools import partial
 import tifffile
 import concurrent.futures
 from astropy.io import fits
 
 
+def crop_frame(image, crop_mode):
+
+    try:
+
+        if "left" in crop_mode.lower():
+            crop = image[:, :image.shape[1]//2]
+        elif "right" in crop_mode.lower():
+            crop = image[:, image.shape[1]//2:]
+        elif "brightest" in crop_mode.lower():
+            left = image[:, :image.shape[1]//2]
+            right = image[:, image.shape[1]//2:]
+            crop = left if np.mean(left) > np.mean(right) else right
+        else:
+            crop = image
+
+    except:
+        print(traceback.format_exc())
+        crop = image
+
+    return crop
+
 def import_image_data(dat, progress_dict={}, index=0):
 
     try:
 
         path = dat["path"]
-        import_crop_mode = dat["import_crop_mode"]
-        n_frames = dat["n_frames"]
+        crop_mode = dat["import_crop_mode"]
+        import_limit = dat["import_limit"]
+        frame_averaging = dat["frame_averaging"]
 
         base, ext = os.path.splitext(path)
 
+        images = []
+
         if ext.lower() == ".tif":
 
             with Image.open(path) as image:
 
+                n_frames = image.n_frames
+
+                if import_limit != "None":
+                    if import_limit.isdigit():
+                        import_limit = int(import_limit)
+                        if n_frames > import_limit:
+                            n_frames = import_limit
+
                 for frame_index in range(n_frames):
 
                     image.seek(frame_index)
                     img_frame = np.array(image)
 
-                    shared_mem = dat["shared_image"]
-                    np_array = np.ndarray(dat["image_shape"], dtype=dat["dtype"], buffer=shared_mem.buf)
-                    np_array[frame_index] = img_frame
+                    img_frame = crop_frame(img_frame, crop_mode)
+
+                    images.append(img_frame)
 
                     progress = int(((frame_index + 1) / n_frames)*100)
                     progress_dict[index] = progress
 
         elif ext.lower() == ".fits":
 
-            time_start = time.time()
-
             with fits.open(path) as hdul:
 
-                shared_mem = dat["shared_image"]
-                np_array = np.ndarray(dat["image_shape"], dtype=dat["dtype"], buffer=shared_mem.buf)
+                n_frames = hdul[0].data.shape[0]
+
+                if import_limit != "None":
+                    if import_limit.isdigit():
+                        import_limit = int(import_limit)
+                        if n_frames > import_limit:
+                            n_frames = import_limit
 
                 for frame_index in range(n_frames):
 
                     img_frame = hdul[0].data[frame_index]
 
-                    np_array[frame_index] = img_frame
+                    img_frame = crop_frame(img_frame, crop_mode)
+
+                    images.append(img_frame)
 
                     progress = int(((frame_index + 1) / n_frames)*100)
                     progress_dict[index] = progress
 
-            end_time = time.time()
-            print(f"Time taken: {end_time - time_start}")
+        if len(images) > 0:
+            images = np.stack(images, axis=0)
+
+            if frame_averaging == True:
+                images = np.mean(images, axis=0)
+                images = np.expand_dims(images, axis=0)
+
+            dat["data"] = images
 
     except:
         print(traceback.format_exc())
         pass
 
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
+    return dat
 
 
 
 class _import_utils:
 
-    def create_import_shared_image(self, image_size):
-
-        shared_mem = None
-
-        try:
-
-            if self.verbose:
-                print("Creating shared image...")
-
-            shared_mem = shared_memory.SharedMemory(create=True, size=image_size)
-
-        except:
-            print(traceback.format_exc())
-            pass
-
-        return shared_mem
 
     def get_image_info(self, path):
 
         if self.verbose:
             print(f"Getting image info for {path}")
 
         base, ext = os.path.splitext(path)
@@ -173,90 +183,48 @@
         except:
             print(traceback.format_exc())
             pass
 
         return path
 
 
-    def populate_import_lists(self, progress_callback=None, paths=[]):
+    def populate_import_jobs(self, progress_callback=None, paths=[]):
 
-        image_list = []
-        import_dict = {}
-        shared_images = {}
+        import_jobs = []
 
         try:
 
-            if self.verbose:
-                print("Populating import lists/metadata...")
-
             import_crop_mode = self.gui.import_crop_mode.currentText()
-            import_limit_combo = self.gui.import_limit.currentText()
+            import_limit = self.gui.import_limit.currentText()
+            frame_averaging = self.gui.frame_averaging.isChecked()
 
             for path_index, path in enumerate(paths):
 
                 path = self.format_import_path(path)
                 dataset_name = os.path.basename(path)
 
-                if dataset_name not in shared_images.keys():
-                    shared_images[dataset_name] = {}
-
-                n_frames, image_shape, dtype, image_size = self.get_image_info(path)
-
-                if import_limit_combo != "None":
-                    import_limit = int(import_limit_combo)
-                else:
-                    import_limit = n_frames
-
-                if import_crop_mode != "None":
-                    image_shape[2] = image_shape[2]//2
-
-                image_shape = (import_limit, image_shape[1], image_shape[2])
-
-                shared_image = self.create_import_shared_image(image_size)
-                shared_images[dataset_name] = shared_image
-
                 image_dict = {"path": path,
                               "dataset_name": dataset_name,
-                              "shared_image": shared_image,
+                              "import_limit": import_limit,
                               "import_crop_mode": import_crop_mode,
-                              "n_frames": n_frames,
-                              "image_shape": image_shape,
-                              "dtype": dtype,
+                              "frame_averaging": frame_averaging
                               }
 
-                image_list.append(image_dict)
-
-                if dataset_name not in import_dict.keys():
-                    import_dict[dataset_name] = {"path":path,
-                                                 "import_limit": import_limit,
-                                                 "import_crop_mode": import_crop_mode,
-                                                 "image_shape": image_shape,
-                                                 "dtype": dtype,}
+                import_jobs.append(image_dict)
 
         except:
             print(traceback.format_exc())
 
-        return image_list, shared_images, import_dict
+        return import_jobs
 
-    def populate_import_compute_jobs(self, image_list):
-
-        if self.verbose:
-            print(f"Populating import compute jobs.")
-
-        compute_jobs = []
-
-        for image_dict in image_list:
-
-            compute_jobs.append({"stop_event": self.stop_event,
-                                 **image_dict})
-
-        return compute_jobs
 
     def process_compute_jobs(self, compute_jobs, progress_callback=None):
 
+        results = []
+
         if self.verbose:
             print(f"Processing {len(compute_jobs)} compute jobs.")
 
         cpu_count = int(multiprocessing.cpu_count() * 0.75)
         timeout_duration = 10  # Timeout in seconds
 
         with Manager() as manager:
@@ -275,58 +243,50 @@
                         progress_callback.emit(overall_progress)
                     time.sleep(0.1)  # Update frequency
 
                 # Wait for all futures to complete
                 concurrent.futures.wait(futures)
 
                 # Retrieve and process results
-                results = [future.result() for future in futures]
+                results = [future.result() for future in futures if future.done()]
 
         if self.verbose:
             print("Finished processing compute jobs.")
 
-    def populate_import_dataset_dict(self, import_dict):
+        return results
+
+    def populate_import_dataset_dict(self, import_list):
 
         try:
 
             concat_images = self.gui.import_concatenate.isChecked()
 
             if self.verbose:
                 print("Populating dataset dict")
 
-            image_dict = {}
-
-            for dataset_name, dataset_dict in import_dict.items():
-
-                path = dataset_dict["path"]
-                image_shape = dataset_dict["image_shape"]
-                dtype = dataset_dict["dtype"]
+            import_dict = {}
 
-                shared_mem = self.shared_images[dataset_name]
+            for import_data in import_list:
 
-                image = np.ndarray(image_shape, dtype=dtype, buffer=shared_mem.buf).copy()
-                image = image.astype(np.uint16)
+                if type(import_data) == dict:
 
-                shared_mem.close()
-                shared_mem.unlink()
+                    if "data" in import_data.keys():
 
-                if dataset_name not in import_dict.keys():
-                    import_dict[dataset_name] = {"data": []}
-
-                import_dict[dataset_name]["data"] = image
-                import_dict[dataset_name]["path"] = path
+                        dataset_name = import_data["dataset_name"]
+                        import_dict[dataset_name] = import_data
 
             if concat_images == True:
 
                 dataset_list = list(import_dict.keys())
 
                 image_list = []
                 path_list = []
 
                 for dataset_name in dataset_list:
+
                     dataset_image = import_dict[dataset_name].pop("data")
                     dataset_path = import_dict[dataset_name].pop("path")
 
                     dataset_path = [dataset_path]*dataset_image.shape[0]
 
                     image_list.append(dataset_image)
                     path_list.extend(dataset_path)
@@ -343,29 +303,36 @@
                     dataset_dict = import_dict.pop(dataset_name)
                     self.dataset_dict[dataset_name] = dataset_dict
 
         except:
             print(traceback.format_exc())
             pass
 
-    def import_data(self, progress_callback=None, paths=[]):
+    def import_data(self, progress_callback=None, paths=[], import_mode="data"):
 
-        image_list, self.shared_images, import_dict = self.populate_import_lists(paths=paths)
+        import_jobs = self.populate_import_jobs(paths=paths)
 
-        compute_jobs = self.populate_import_compute_jobs(image_list)
+        results = self.process_compute_jobs(import_jobs,
+            progress_callback=progress_callback)
 
-        self.process_compute_jobs(compute_jobs, progress_callback=progress_callback)
+        if import_mode.lower() == "data":
+            self.populate_import_dataset_dict(results)
+        else:
 
-        self.populate_import_dataset_dict(import_dict)
+            if len(results) > 0:
+                if type(results[0]) == dict:
+                    if "data" in results[0].keys():
+                        self.segmentation_image = results[0]["data"]
 
     def import_data_finished(self):
 
         self.populate_dataset_selectors()
         self.update_ui()
-        # self.update_active_image()
+        self.update_active_image()
+        self.draw_segmentation_image()
 
     def populate_dataset_selectors(self):
 
         dataset_selectors = ["import_picasso_dataset",
                              "cellpose_dataset",
                              "moltrack_dataset_selector",
                              "picasso_dataset",
@@ -376,38 +343,52 @@
                              ]
 
         for selector_name in dataset_selectors:
 
             dataset_names = list(self.dataset_dict.keys())
 
             if selector_name in ["picasso_dataset","locs_export_dataset"] and len(dataset_names) > 1:
-                dataset_names.append("All Datasets")
+                dataset_names.insert(0, "All Datasets")
+
+            if selector_name == "cellpose_dataset":
+                if hasattr(self, "segmentation_image"):
+                    dataset_names.insert(0, "Segmentation Image")
 
             if hasattr(self.gui, selector_name):
                 getattr(self.gui, selector_name).clear()
                 getattr(self.gui, selector_name).addItems(dataset_names)
 
-
     def init_import_data(self):
 
         try:
 
+            import_mode = self.gui.import_mode.currentText()
             desktop = os.path.expanduser("~/Desktop")
-            paths = QFileDialog.getOpenFileNames(self, 'Open file', desktop, "Image files (*.tif *.fits)")[0]
 
-            paths = [path for path in paths if path != ""]
+            if import_mode.lower() == "data":
+
+                paths = QFileDialog.getOpenFileNames(self, 'Open file',
+                    desktop, "Image files (*.tif *.fits)")[0]
+
+                paths = [path for path in paths if path != ""]
+
+            else:
+                path = QFileDialog.getOpenFileName(self, 'Open file',
+                    desktop, "Image files (*.tif *.fits)")[0]
+                paths = [path]
 
             if paths != []:
 
                 self.update_ui(init=True)
 
-                self.worker = Worker(self.import_data, paths=paths)
+                self.worker = Worker(self.import_data, paths=paths, import_mode=import_mode)
                 self.worker.signals.progress.connect(partial(self.moltrack_progress,
                     progress_bar=self.gui.import_progressbar))
                 self.worker.signals.finished.connect(self.import_data_finished)
                 self.worker.signals.error.connect(self.update_ui)
                 self.threadpool.start(self.worker)
 
+
         except:
             self.update_ui()
             print(traceback.format_exc())
             pass
```

### Comparing `napari_moltrack-0.0.3/src/moltrack/funcs/loc_filter_utils.py` & `napari_moltrack-0.0.4/src/moltrack/funcs/loc_filter_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.3/src/moltrack/funcs/picasso_detect_utils.py` & `napari_moltrack-0.0.4/src/moltrack/funcs/picasso_detect_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.3/src/moltrack/funcs/picasso_render_utils.py` & `napari_moltrack-0.0.4/src/moltrack/funcs/picasso_render_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.3/src/moltrack/funcs/segmentation_utils.py` & `napari_moltrack-0.0.4/src/moltrack/funcs/segmentation_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -180,82 +180,104 @@
                         show_info(f"Could not load model")
 
         except:
             print(traceback.format_exc())
 
         return model, gpu, omnipose_model, labels_to_flows
 
-    def initialise_cellpose(self, mode = "active"):
 
-        try:
+    def get_segmentation_images(self, mode = "active"):
+
+        images = []
 
-            if self.dataset_dict != {}:
+        if self.dataset_dict != {} or hasattr(self, "segmentation_image"):
 
-                dataset = self.gui.cellpose_dataset.currentText()
-                current_frame = self.viewer.dims.current_step[0]
+            dataset = self.gui.cellpose_dataset.currentText()
+            current_frame = self.viewer.dims.current_step[0]
 
-                images = []
+            if dataset == "Segmentation Image":
+                if hasattr(self, "segmentation_image"):
+                    images = self.segmentation_image.copy()
 
+                    if mode == "active":
+                        images = [images[current_frame]]
+                    else:
+                        if len(images.shape) == 3:
+                            images = [frame for frame in images]
+                        else:
+                            images = [images]
+            else:
                 if mode == "active":
                     images = [self.dataset_dict[dataset]["data"][current_frame]]
                 else:
                     images = self.dataset_dict[dataset]["data"].copy()
 
                     if len(images.shape) == 3:
                         images = [frame for frame in images]
                     else:
                         images = [images]
 
-                if len(images) > 0:
+        return images
+
+
+    def initialise_cellpose(self, mode = "active"):
+
+        try:
 
-                    self.update_ui(init=True)
+            images = self.get_segmentation_images(mode = mode)
 
-                    self.worker = Worker(self.pixseq_segment, images = images, mode = mode)
-                    self.worker.signals.result.connect(self.process_cellpose_result)
-                    self.worker.signals.finished.connect(self.run_cellpose_finished)
-                    self.worker.signals.progress.connect(partial(self.moltrack_progress, progress_bar=self.gui.cellpose_progressbar))
-                    self.threadpool.start(self.worker)
+            if len(images) > 0:
+
+                self.update_ui(init=True)
+
+                self.worker = Worker(self.pixseq_segment, images = images, mode = mode)
+                self.worker.signals.result.connect(self.process_cellpose_result)
+                self.worker.signals.finished.connect(self.run_cellpose_finished)
+                self.worker.signals.progress.connect(partial(self.moltrack_progress,
+                    progress_bar=self.gui.cellpose_progressbar))
+                self.threadpool.start(self.worker)
 
         except:
             self.update_ui(init=False)
             print(traceback.format_exc())
             pass
 
     def process_cellpose_result(self, result):
 
         try:
 
             layer_names = [layer.name for layer in self.viewer.layers]
 
             mode, masks = result
 
-            if "Segmentations" not in layer_names:
-                self.segLayer = self.viewer.add_shapes(name="Segmentations", shape_type="polygon",
-                    opacity=0.5, face_color="red", edge_color="black", edge_width=1)
-
-            self.segLayer.data = []
-
             if mode == "active":
-
-                shapes = self.mask_to_shape(masks[0])
-                self.segLayer.data = shapes
+                shapes = self.mask_to_shape(masks[0], frame = 0)
+                ndim = 2
             else:
-
+                shapes = []
+                ndim = 3
                 for i, mask in enumerate(masks):
-                    shapes = self.mask_to_shape(mask, frame = i)
-                    self.segLayer.add(shapes, shape_type="polygon")
+                    layer_shapes = self.mask_to_shape(mask)
+                    shapes.extend(layer_shapes)
+
+            if len(shapes) > 0:
+                if "Segmentations" in layer_names:
+                    self.viewer.layers.remove("Segmentations")
+
+                self.segLayer = self.viewer.add_shapes(shapes, shape_type="polygon",
+                    name="Segmentations", opacity=0.3, face_color="red")
 
         except:
             print(traceback.format_exc())
             pass
 
     def mask_to_shape(self, mask, frame = None):
 
         """converts mask to napari shapes"""
-
+        mask = mask.copy()
         shapes = []
         try:
 
             for label in np.unique(mask):
                 if label == 0:
                     continue  # Skip background
                 # Create a binary mask for the current object
```

### Comparing `napari_moltrack-0.0.3/src/moltrack/funcs/tracking_utils.py` & `napari_moltrack-0.0.4/src/moltrack/funcs/tracking_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.3/src/napari_moltrack.egg-info/PKG-INFO` & `napari_moltrack-0.0.4/src/napari_moltrack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-moltrack
-Version: 0.0.3
+Version: 0.0.4
 Summary: Single molecule tracking package for Napari
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: 
         Copyright (c) 2024, Piers Turner
         All rights reserved.
```

### Comparing `napari_moltrack-0.0.3/src/napari_moltrack.egg-info/SOURCES.txt` & `napari_moltrack-0.0.4/src/napari_moltrack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.3/src/pygpufit/Gpufit.dll` & `napari_moltrack-0.0.4/src/pygpufit/Gpufit.dll`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.3/src/pygpufit/gpufit.py` & `napari_moltrack-0.0.4/src/pygpufit/gpufit.py`

 * *Files identical despite different names*

