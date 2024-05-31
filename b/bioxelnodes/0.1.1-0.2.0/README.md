# Comparing `tmp/bioxelnodes-0.1.1.tar.gz` & `tmp/bioxelnodes-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioxelnodes-0.1.1.tar", max compression
+gzip compressed data, was "bioxelnodes-0.2.0.tar", max compression
```

## Comparing `bioxelnodes-0.1.1.tar` & `bioxelnodes-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      600 2024-05-11 06:22:47.294647 bioxelnodes-0.1.1/bioxelnodes/__init__.py
--rw-r--r--   0        0        0  1635596 2024-05-09 06:18:56.470558 bioxelnodes-0.1.1/bioxelnodes/assets/Nodes/BioxelNodes_4.0.blend
--rw-r--r--   0        0        0  1749214 2024-04-24 08:18:13.573093 bioxelnodes-0.1.1/bioxelnodes/assets/Nodes/BioxelNodes_4.1.blend
--rw-r--r--   0        0        0     5249 2024-05-11 05:24:35.143596 bioxelnodes-0.1.1/bioxelnodes/auto_load.py
--rw-r--r--   0        0        0     2131 2024-04-29 09:12:44.852094 bioxelnodes-0.1.1/bioxelnodes/convert.py
--rw-r--r--   0        0        0       30 2024-05-09 00:55:08.265126 bioxelnodes-0.1.1/bioxelnodes/customnodes/__init__.py
--rw-r--r--   0        0        0     6912 2024-05-10 01:37:42.552617 bioxelnodes-0.1.1/bioxelnodes/customnodes/menus.py
--rw-r--r--   0        0        0     3648 2024-04-29 06:52:03.731217 bioxelnodes-0.1.1/bioxelnodes/customnodes/nodes.py
--rw-r--r--   0        0        0       92 2024-04-30 03:51:36.907837 bioxelnodes-0.1.1/bioxelnodes/externalpackage/__init__.py
--rw-r--r--   0        0        0    13381 2024-05-06 04:41:42.458673 bioxelnodes-0.1.1/bioxelnodes/externalpackage/package.py
--rw-r--r--   0        0        0     3465 2024-05-05 07:52:57.079036 bioxelnodes-0.1.1/bioxelnodes/externalpackage/preferences.py
--rw-r--r--   0        0        0    24475 2024-05-14 02:58:19.858419 bioxelnodes-0.1.1/bioxelnodes/io.py
--rw-r--r--   0        0        0     7180 2024-05-09 10:11:03.808490 bioxelnodes-0.1.1/bioxelnodes/io_points.py
--rw-r--r--   0        0        0     1251 2024-05-11 04:28:40.340960 bioxelnodes-0.1.1/bioxelnodes/menus.py
--rw-r--r--   0        0        0     3309 2024-05-10 01:37:12.810836 bioxelnodes-0.1.1/bioxelnodes/misc.py
--rw-r--r--   0        0        0     4975 2024-05-10 02:54:05.390637 bioxelnodes-0.1.1/bioxelnodes/nodes.py
--rw-r--r--   0        0        0     1069 2024-05-11 02:31:51.293418 bioxelnodes-0.1.1/bioxelnodes/preferences.py
--rw-r--r--   0        0        0      175 2024-05-09 00:29:30.364888 bioxelnodes-0.1.1/bioxelnodes/props.py
--rw-r--r--   0        0        0       69 2024-05-14 02:58:19.858419 bioxelnodes-0.1.1/bioxelnodes/requirements.txt
--rw-r--r--   0        0        0     4247 2024-05-13 03:25:36.874364 bioxelnodes-0.1.1/bioxelnodes/utils.py
--rw-r--r--   0        0        0     1085 2024-04-22 14:35:56.279907 bioxelnodes-0.1.1/LICENSE
--rw-r--r--   0        0        0      644 2024-05-14 02:58:19.882198 bioxelnodes-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3048 2024-05-14 02:58:19.857418 bioxelnodes-0.1.1/README.md
--rw-r--r--   0        0        0     3432 1970-01-01 00:00:00.000000 bioxelnodes-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      611 2024-05-27 05:38:14.303729 bioxelnodes-0.2.0/bioxelnodes/__init__.py
+-rw-r--r--   0        0        0  4887206 2024-05-31 00:43:48.682489 bioxelnodes-0.2.0/bioxelnodes/assets/Nodes/BioxelNodes_4.0.blend
+-rw-r--r--   0        0        0  4196897 2024-05-31 00:48:03.095350 bioxelnodes-0.2.0/bioxelnodes/assets/Nodes/BioxelNodes_4.1.blend
+-rw-r--r--   0        0        0     5249 2024-05-11 05:24:35.143596 bioxelnodes-0.2.0/bioxelnodes/auto_load.py
+-rw-r--r--   0        0        0       30 2024-05-09 00:55:08.265126 bioxelnodes-0.2.0/bioxelnodes/customnodes/__init__.py
+-rw-r--r--   0        0        0     6958 2024-05-30 05:53:14.912295 bioxelnodes-0.2.0/bioxelnodes/customnodes/menus.py
+-rw-r--r--   0        0        0     3648 2024-04-29 06:52:03.731217 bioxelnodes-0.2.0/bioxelnodes/customnodes/nodes.py
+-rw-r--r--   0        0        0       92 2024-04-30 03:51:36.907837 bioxelnodes-0.2.0/bioxelnodes/externalpackage/__init__.py
+-rw-r--r--   0        0        0    13381 2024-05-06 04:41:42.458673 bioxelnodes-0.2.0/bioxelnodes/externalpackage/package.py
+-rw-r--r--   0        0        0     3465 2024-05-05 07:52:57.079036 bioxelnodes-0.2.0/bioxelnodes/externalpackage/preferences.py
+-rw-r--r--   0        0        0    28680 2024-05-30 13:52:38.748681 bioxelnodes-0.2.0/bioxelnodes/io.py
+-rw-r--r--   0        0        0     7180 2024-05-09 10:11:03.808490 bioxelnodes-0.2.0/bioxelnodes/io_points.py
+-rw-r--r--   0        0        0     2027 2024-05-28 01:52:34.315838 bioxelnodes-0.2.0/bioxelnodes/menus.py
+-rw-r--r--   0        0        0     2851 2024-05-28 04:41:36.794058 bioxelnodes-0.2.0/bioxelnodes/misc.py
+-rw-r--r--   0        0        0    10294 2024-05-30 23:48:23.589058 bioxelnodes-0.2.0/bioxelnodes/nodes.py
+-rw-r--r--   0        0        0     8608 2024-05-30 06:31:22.286490 bioxelnodes-0.2.0/bioxelnodes/operators.py
+-rw-r--r--   0        0        0      889 2024-05-20 00:10:55.208891 bioxelnodes-0.2.0/bioxelnodes/preferences.py
+-rw-r--r--   0        0        0      175 2024-05-09 00:29:30.364888 bioxelnodes-0.2.0/bioxelnodes/props.py
+-rw-r--r--   0        0        0       69 2024-05-14 02:58:19.858419 bioxelnodes-0.2.0/bioxelnodes/requirements.txt
+-rw-r--r--   0        0        0     4722 2024-05-29 09:18:42.669433 bioxelnodes-0.2.0/bioxelnodes/utils.py
+-rw-r--r--   0        0        0     1085 2024-04-22 14:35:56.279907 bioxelnodes-0.2.0/LICENSE
+-rw-r--r--   0        0        0      644 2024-05-29 02:45:01.171807 bioxelnodes-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3925 2024-05-29 04:29:00.608873 bioxelnodes-0.2.0/README.md
+-rw-r--r--   0        0        0     4296 1970-01-01 00:00:00.000000 bioxelnodes-0.2.0/PKG-INFO
```

### Comparing `bioxelnodes-0.1.1/bioxelnodes/auto_load.py` & `bioxelnodes-0.2.0/bioxelnodes/auto_load.py`

 * *Files identical despite different names*

### Comparing `bioxelnodes-0.1.1/bioxelnodes/customnodes/menus.py` & `bioxelnodes-0.2.0/bioxelnodes/customnodes/menus.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,38 +142,43 @@
 
         menu_classes.append(Menu)
         return Menu
 
     def _find_item(self, found_items, menu_items, node_type: str):
 
         for item in menu_items:
+            if item == 'separator':
+                continue
+
             if item.get("node_type") == node_type:
                 found_items.append(item)
 
-            item_items = item.get('items') if item != 'separator' else None
+            item_items = item.get('items')
             if item_items:
                 self._find_item(found_items, item_items, node_type)
 
     def find_item(self, node_type: str):
         found_items = []
         self._find_item(found_items, self.menu_items, node_type)
         return found_items[0] if len(found_items) > 0 else None
 
     def add_node(self, node_tree, node_type: str):
         item = self.find_item(node_type)
+        op = AddCustomNode()
+        op.nodes_file = self.nodes_file
+        op.node_type = node_type
         if item:
-            op = AddCustomNode()
-            op.nodes_file = self.nodes_file
-            op.node_type = item['node_type']
             op.node_label = item.get('label') or ""
             op.node_link = item.get('link') or True
             op.node_callback = item.get('node_callback') or ""
-            return op.add_node(node_tree)
         else:
-            raise RuntimeError("No custom node type found.")
+            op.node_label = ""
+            op.node_link = True
+            op.node_callback = ""
+        return op.add_node(node_tree)
 
     def register(self):
         for cls in self.menu_classes:
             bpy.utils.register_class(cls)
 
         bpy.types.NODE_MT_add.append(self.add_node_menu)
         bpy.types.Scene.custom_nodes_dir = bpy.props.StringProperty(
```

### Comparing `bioxelnodes-0.1.1/bioxelnodes/customnodes/nodes.py` & `bioxelnodes-0.2.0/bioxelnodes/customnodes/nodes.py`

 * *Files identical despite different names*

### Comparing `bioxelnodes-0.1.1/bioxelnodes/externalpackage/package.py` & `bioxelnodes-0.2.0/bioxelnodes/externalpackage/package.py`

 * *Files identical despite different names*

### Comparing `bioxelnodes-0.1.1/bioxelnodes/externalpackage/preferences.py` & `bioxelnodes-0.2.0/bioxelnodes/externalpackage/preferences.py`

 * *Files identical despite different names*

### Comparing `bioxelnodes-0.1.1/bioxelnodes/io.py` & `bioxelnodes-0.2.0/bioxelnodes/io.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 import shutil
 from bpy_extras.io_utils import axis_conversion
 import pyopenvdb as vdb
 import numpy as np
 from pathlib import Path
 from uuid import uuid4
 import mathutils
-import math
-from .utils import calc_bbox_verts, get_text_index_str, get_bioxels_obj, get_node_by_type, show_message
+
 from .nodes import custom_nodes
 from .props import BIOXELNODES_Series
+from .utils import (calc_bbox_verts, get_container, get_layer, get_text_index_str,
+                    get_node_by_type, hide_in_ray, lock_transform, show_message)
+
 try:
     import SimpleITK as sitk
 except:
     ...
 
-SUPPORT_EXTS = ['.dcm', '.DICOM',
+SUPPORT_EXTS = ['.dcm', '.DCM', '.DICOM',
                 '.bmp', '.BMP',
                 '.PIC', '.pic',
                 '.gipl', '.gipl.gz',
                 '.jpg', '.JPG', '.jpeg', '.JPEG',
                 '.lsm', '.LSM',
                 '.tif', '.TIF', '.tiff', '.TIFF',
                 '.mnc', '.MNC',
@@ -27,35 +29,35 @@
                 '.mha', '.mhd',
                 '.hdf', '.h4', '.hdf4', '.he2', '.h5', '.hdf5', '.he5',
                 '.nia', '.nii', '.nii.gz', '.hdr', '.img', '.img.gz',
                 '.nrrd', '.nhdr',
                 '.png', '.PNG',
                 '.vtk']
 
-SEQUENCE_EXTS = ['.dcm', '.DICOM',
+SEQUENCE_EXTS = ['.dcm', '.DCM', '.DICOM',
                  '.bmp', '.BMP',
                  '.jpg', '.JPG', '.jpeg', '.JPEG',
                  '.tif', '.TIF', '.tiff', '.TIFF',
                  '.png', '.PNG']
 
-DICOM_EXTS = ['.dcm', '.DICOM']
+DICOM_EXTS = ['.dcm', '.DCM', '.DICOM']
 
-FH_EXTS = ['.dcm', '.DICOM',
+FH_EXTS = ['.dcm', '.DCM', '.DICOM',
            '.gipl', '.gipl.gz',
            '.mnc', '.MNC',
            '.mrc', '.rec',
            '.mha', '.mhd',
            '.nia', '.nii', '.nii.gz', '.hdr', '.img', '.img.gz',
            '.hdf', '.h4', '.hdf4', '.he2', '.h5', '.hdf5', '.he5',
            '.nrrd', '.nhdr',
            '.vtk',
            '.gz']
 
 
-def get_bioxels_shape(bioxel_size: float, orig_shape: tuple, orig_spacing: tuple):
+def get_layer_shape(bioxel_size: float, orig_shape: tuple, orig_spacing: tuple):
     shape = (int(orig_shape[0] / bioxel_size * orig_spacing[0]),
              int(orig_shape[1] / bioxel_size * orig_spacing[1]),
              int(orig_shape[2] / bioxel_size * orig_spacing[2]))
 
     return (shape[0] if shape[0] > 0 else 1,
             shape[1] if shape[1] > 0 else 1,
             shape[2] if shape[2] > 0 else 1)
@@ -128,76 +130,82 @@
         name = Path(filepath).name.removesuffix(ext)
 
     return image, name
 
 
 def rgb2gray(image):
     # Convert sRGB image to gray scale and rescale results to [0,255]
-    channels = [sitk.VectorIndexSelectionCast(
+    layers = [sitk.VectorIndexSelectionCast(
         image, i, sitk.sitkFloat32) for i in range(image.GetNumberOfComponentsPerPixel())]
     # linear mapping
-    I = (0.2126*channels[0] + 0.7152*channels[1] + 0.0722*channels[2])
+    I = (0.2126*layers[0] + 0.7152*layers[1] + 0.0722*layers[2])
 
     return sitk.Cast(I, sitk.sitkFloat32)
 
+
 def x2gray(image):
     return sitk.VectorIndexSelectionCast(image, 0, sitk.sitkUInt16)
 
+
 class ImportVolumeDataDialog(bpy.types.Operator):
     bl_idname = "bioxelnodes.import_volume_data_dialog"
-    bl_label = "Volume Data as Bioxels"
-    bl_description = "Import Volume Data as Bioxels (VDB)"
+    bl_label = "Volume Data as Bioxel Layer"
+    bl_description = "Import Volume Data as Bioxel Layer"
     bl_options = {'UNDO'}
 
     filepath: bpy.props.StringProperty(
-        subtype="FILE_PATH",
-        options={'HIDDEN'}
+        subtype="FILE_PATH"
     )  # type: ignore
 
+    container_name: bpy.props.StringProperty(
+        name="Container Name"
+    )   # type: ignore
+
+    layer_name: bpy.props.StringProperty(
+        name="Layer Name",
+    )   # type: ignore
+
     series_id: bpy.props.StringProperty()   # type: ignore
 
     resample_method: bpy.props.EnumProperty(
         name="Resample Method",
         default="linear",
         items=[("linear", "Linear", ""),
                ("nearest_neighbor", "Nearest Neighbor", ""),
                ("gaussian", "Gaussian", "")]
     )  # type: ignore
 
+    container: bpy.props.StringProperty()   # type: ignore
+
     read_as: bpy.props.EnumProperty(
         name="Read as",
         default="scalar",
         items=[("scalar", "Scalar", ""),
                ("labels", "Labels", "")]
     )  # type: ignore
 
-    label_index: bpy.props.IntProperty(
-        name="Label Index",
-        default=1
-    )  # type: ignore
-
     bioxel_size: bpy.props.FloatProperty(
         name="Bioxel Size (Larger size means small resolution)",
         soft_min=0.1, soft_max=10.0,
-        min=1e-2, max=1e2,
+        min=0.1, max=1e2,
         default=1,
     )  # type: ignore
 
     orig_spacing: bpy.props.FloatVectorProperty(
         name="Original Spacing",
         default=(1, 1, 1),
     )  # type: ignore
 
     orig_shape: bpy.props.IntVectorProperty(
         name="Original Shape",
         default=(100, 100, 100)
     )  # type: ignore
 
     scene_scale: bpy.props.FloatProperty(
-        name="Scene Scale (Bioxels Unit pre Blender Unit)",
+        name="Scene Scale (Bioxel Unit pre Blender Unit)",
         soft_min=0.001, soft_max=100.0,
         min=1e-6, max=1e6,
         default=0.01,
     )  # type: ignore
 
     do_orient: bpy.props.BoolProperty(
         name="Orient to RAS",
@@ -206,63 +214,66 @@
 
     invert_scalar: bpy.props.BoolProperty(
         name="Invert Scalar (Background value maybe higher than object)",
         default=False,
     )  # type: ignore
 
     def execute(self, context):
-        image, bioxels_name = read_image(self.filepath, self.series_id)
-
+        image, name = read_image(self.filepath, self.series_id)
+        container_name = self.container_name or name
         bioxel_size = self.bioxel_size
         orig_spacing = self.orig_spacing
         image_spacing = image.GetSpacing()
         image_shape = image.GetSize()
 
-        bioxels_spacing = (
+        layer_spacing = (
             image_spacing[0] / orig_spacing[0] * bioxel_size,
             image_spacing[1] / orig_spacing[1] * bioxel_size,
             image_spacing[2] / orig_spacing[2] * bioxel_size
         )
 
-        bioxels_shape = get_bioxels_shape(
+        layer_shape = get_layer_shape(
             bioxel_size, image_shape, orig_spacing)
 
         if self.read_as == "labels":
             if "vector" in image.GetPixelIDTypeAsString():
-                print("Convet to Grayscale...")
+                print("Conveting to Grayscale...")
                 image = x2gray(image)
             else:
                 image = sitk.Cast(image, sitk.sitkUInt16)
             default_value = 0
         elif self.read_as == "scalar":
             if "vector" in image.GetPixelIDTypeAsString():
-                print("Convet to Grayscale...")
+                print("Conveting to Grayscale...")
                 image = rgb2gray(image)
             else:
                 image = sitk.Cast(image, sitk.sitkFloat32)
 
             stats = sitk.StatisticsImageFilter()
             stats.Execute(image)
             default_value = stats.GetMaximum() if self.invert_scalar else stats.GetMinimum()
 
         if self.resample_method == "linear":
             interpolator = sitk.sitkLinear
         elif self.resample_method == "nearest_neighbor":
             interpolator = sitk.sitkNearestNeighbor
         elif self.resample_method == "gaussian":
             interpolator = sitk.sitkGaussian
+            
+        if self.read_as == "labels":
+            interpolator = sitk.sitkNearestNeighbor
 
         print(f"Resampling...")
         image = sitk.Resample(
             image1=image,
-            size=bioxels_shape,
+            size=layer_shape,
             transform=sitk.Transform(),
             interpolator=interpolator,
             outputOrigin=image.GetOrigin(),
-            outputSpacing=bioxels_spacing,
+            outputSpacing=layer_spacing,
             outputDirection=image.GetDirection(),
             defaultPixelValue=default_value,
             outputPixelType=image.GetPixelID(),
         )
 
         if self.do_orient:
             print("Orienting to RAS...")
@@ -277,71 +288,23 @@
         # https://www.slicer.org/wiki/Coordinate_systems
 
         # ITK                  Numpy      3D
         # R (ight)     i   ->    k   ->   x
         # A (nterior)  j   ->    j   ->   y
         # S (uperior)  k   ->    i   ->   z
         array = sitk.GetArrayFromImage(image)
-
         orig_dtype = str(array.dtype)
         # print(f"Coverting Dtype from {orig_dtype} to float...")
         # array = array.astype(float)
 
         if array.ndim == 4:
-            # if array.shape[0] == 3 and self.read_as == "scalar":
-            #     # RGB -> Grayscale
-            #     array = np.dot(array[..., :3], [0.2989, 0.5870, 0.1140])
-            # else:
-            #     array = array[:, :, :, 0]
             array = array[:, :, :, 0]
 
         array = np.transpose(array)
 
-        bioxels_shape = array.shape
-        bioxels_offset = 0.0
-
-        if self.read_as == "labels":
-            array = array == np.full_like(array, self.label_index)
-            bioxels_default_threshold = 1.0
-            bioxels_max = 1.0
-            bioxels_min = 0.0
-            bioxels_name = f"{bioxels_name}_{self.label_index}"
-        else:
-            if self.invert_scalar:
-                array = -array
-
-            orig_max = float(np.max(array))
-            orig_min = float(np.min(array))
-            orig_median = float(np.median(array))
-            orig_percentile80 = float(np.percentile(array, 80)) \
-                if self.invert_scalar else float(np.percentile(array, 80))
-
-            # if (orig_dtype[0] != "u" and orig_min < 0) \
-            #         or (orig_dtype[0] == "u" and self.invert_scalar):
-            if orig_min < 0:
-                bioxels_offset = -orig_min
-                array = array + np.full_like(array, bioxels_offset)
-
-            bioxels_default_threshold = orig_percentile80
-            bioxels_max = float(np.max(array))
-            bioxels_min = float(np.min(array))
-
-            stats_table = [("Max", orig_max),
-                           ("Min", orig_min),
-                           ("Median", orig_median),
-                           ("80%", orig_percentile80)]
-
-            print("Bioxels Value Stats:")
-            for stats in stats_table:
-                print("| {: >10} | {: >40} |".format(*stats))
-
-        # # Build VDB
-        grid = vdb.BoolGrid() if self.read_as == "labels" else vdb.FloatGrid()
-        grid.copyFromArray(array.copy().astype(float))
-
         # After sitk.DICOMOrient(), origin and direction will also orient base on LPS
         # so we need to convert them into RAS
         mat_lps2ras = axis_conversion(
             from_forward='-Z',
             from_up='-Y',
             to_forward='-Z',
             to_up='Y'
@@ -361,164 +324,263 @@
         mat_scale = mathutils.Matrix.Scale(
             bioxel_size, 4
         )
 
         transfrom = mat_lps2ras @ mat_location @ mat_rotation @ mat_scale \
             if self.do_orient else mat_location @ mat_rotation @ mat_scale
 
-        grid.transform = vdb.createLinearTransform(transfrom.transposed())
-        grid.name = "scalar"
+        # Wrapper a Container
+        if not self.container:
+            # Make transformation
+            scene_scale = float(self.scene_scale)
+
+            # (S)uperior  -Z -> Y
+            # (A)osterior  Y -> Z
+            mat_ras2blender = axis_conversion(
+                from_forward='-Z',
+                from_up='Y',
+                to_forward='Y',
+                to_up='Z'
+            ).to_4x4()
+
+            mat_scene_scale = mathutils.Matrix.Scale(
+                scene_scale, 4
+            )
+
+            bpy.ops.mesh.primitive_cube_add(
+                enter_editmode=False, align='WORLD', location=(0, 0, 0), scale=(1, 1, 1)
+            )
+            container = bpy.context.active_object
+
+            bbox_verts = calc_bbox_verts((0, 0, 0), array.shape)
+            for index, vert in enumerate(container.data.vertices):
+                bbox_transform = transfrom
+                vert.co = bbox_transform @ mathutils.Vector(bbox_verts[index])
+
+            container.matrix_world = mat_ras2blender @ mat_scene_scale
+            container.name = container_name
+            container.data.name = container_name
+
+            container['bioxel_container'] = True
+            container['scene_scale'] = scene_scale
+            bpy.ops.node.new_geometry_nodes_modifier()
+            container_node_tree = container.modifiers[0].node_group
+            input_node = get_node_by_type(container_node_tree.nodes,
+                                          'NodeGroupInput')[0]
+            container_node_tree.links.remove(input_node.outputs[0].links[0])
+
+            # bpy.ops.mesh.primitive_cube_add(
+            #     enter_editmode=False, align='WORLD', location=(0, 0, 0), scale=(1, 1, 1)
+            # )
+            # frame = bpy.context.active_object
+            # bbox_verts = calc_bbox_verts((0, 0, 0), array.shape)
+            # for index, vert in enumerate(frame.data.vertices):
+            #     # bbox_transform = mat_ras2blender @ mat_scene_scale @ transfrom
+            #     bbox_transform = transfrom
+            #     vert.co = bbox_transform @ mathutils.Vector(bbox_verts[index])
+
+            # frame.name = f"Frame_{container_name}"
+            # frame.data.name = f"Frame_{container_name}"
+            # lock_transform(frame)
+            # hide_in_ray(frame)
+            # frame.hide_select = True
+            # frame.hide_render = True
+            # frame.display_type = 'WIRE'
+            # frame.parent = container
+
+        else:
+            container = bpy.data.objects[self.container]
+            container_node_tree = container.modifiers[0].node_group
 
         preferences = context.preferences.addons[__package__].preferences
-        vdb_dirpath = Path(preferences.cache_dir, 'VDBs')
-        vdb_dirpath.mkdir(parents=True, exist_ok=True)
-        vdb_path = Path(vdb_dirpath, f"{uuid4()}.vdb")
-
-        print(f"Storing the VDB file ({str(vdb_path)})...")
-        vdb.write(str(vdb_path), grids=[grid])
-
-        # Read VDB
-        print(f"Importing the VDB file to Blender scene...")
-        bpy.ops.object.volume_import(
-            filepath=str(vdb_path), align='WORLD', location=(0, 0, 0), scale=(1, 1, 1))
-
-        bioxels_obj = bpy.context.active_object
-
-        # Set props to VDB object
-        bioxels_obj.name = f"{bioxels_name}_Bioxels"
-        bioxels_obj.data.name = f"{bioxels_name}_Bioxels"
-
-        # Make transformation
-        scene_scale = float(self.scene_scale)
-
-        # (S)uperior  -Z -> Y
-        # (A)osterior  Y -> Z
-        mat_ras2blender = axis_conversion(
-            from_forward='-Z',
-            from_up='Y',
-            to_forward='Y',
-            to_up='Z'
-        ).to_4x4()
+        cache_dir = Path(preferences.cache_dir, 'VDBs')
+        cache_dir.mkdir(parents=True, exist_ok=True)
 
-        mat_scene_scale = mathutils.Matrix.Scale(
-            scene_scale, 4
-        )
+        loc, rot, sca = transfrom.decompose()
 
-        bioxels_obj.matrix_world = mat_ras2blender @ mat_scene_scale
-        bioxels_obj.lock_location[0] = True
-        bioxels_obj.lock_location[1] = True
-        bioxels_obj.lock_location[2] = True
-        bioxels_obj.lock_rotation[0] = True
-        bioxels_obj.lock_rotation[1] = True
-        bioxels_obj.lock_rotation[2] = True
-        bioxels_obj.lock_scale[0] = True
-        bioxels_obj.lock_scale[1] = True
-        bioxels_obj.lock_scale[2] = True
-        bioxels_obj.hide_select = True
-        bioxels_obj['bioxels'] = True
+        layer_origin = tuple(loc)
+        layer_rotation = tuple(rot.to_euler())
+        layer_shape = tuple(array.shape)
+
+        def create_layer(array, layer_name, layer_type="scalar"):
+            grid = vdb.FloatGrid()
+            array = array.copy().astype(float)
+            grid.copyFromArray(array)
+            grid.transform = vdb.createLinearTransform(transfrom.transposed())
+            grid.name = layer_type
+
+            vdb_path = Path(cache_dir, f"{uuid4()}.vdb")
+            print(f"Storing the cache ({str(vdb_path)})...")
+            vdb.write(str(vdb_path), grids=[grid])
+
+            # Read VDB
+            print(f"Loading the cache to Blender scene...")
+            bpy.ops.object.volume_import(
+                filepath=str(vdb_path), align='WORLD', location=(0, 0, 0), scale=(1, 1, 1))
+
+            layer = bpy.context.active_object
+
+            # Set props to VDB object
+            layer.name = layer_name
+            layer.data.name = layer_name
+
+            lock_transform(layer)
+            hide_in_ray(layer)
+            layer.hide_select = True
+            layer.hide_render = True
+            layer.hide_viewport = True
+            layer.data.display.use_slice = True
+            layer.data.display.density = 1e-05
+
+            layer['bioxel_layer'] = True
+            layer['bioxel_layer_type'] = layer_type
+            layer.parent = container
+
+            for collection in layer.users_collection:
+                collection.objects.unlink(layer)
 
-        bpy.ops.node.new_geometry_nodes_modifier()
-        node_tree = bioxels_obj.modifiers[0].node_group
+            for collection in container.users_collection:
+                collection.objects.link(layer)
 
-        # Wrapper a Container
-        bpy.ops.mesh.primitive_cube_add(
-            enter_editmode=False, align='WORLD', location=(0, 0, 0), scale=(1, 1, 1)
-        )
-        container_obj = bpy.context.active_object
-        bbox_verts = calc_bbox_verts((0, 0, 0), bioxels_shape)
-        for index, vert in enumerate(container_obj.data.vertices):
-            bbox_transform = mat_ras2blender @ mat_scene_scale @ transfrom
-            vert.co = bbox_transform @ mathutils.Vector(bbox_verts[index])
-
-        bioxels_obj.parent = container_obj
-        container_obj.name = bioxels_name
-        container_obj.data.name = bioxels_name
-        container_obj.visible_camera = False
-        container_obj.visible_diffuse = False
-        container_obj.visible_glossy = False
-        container_obj.visible_transmission = False
-        container_obj.visible_volume_scatter = False
-        container_obj.visible_shadow = False
-        container_obj.display_type = 'WIRE'
-        container_obj['bioxels_container'] = True
-        container_obj['scene_scale'] = scene_scale
-        container_obj['bioxel_size'] = bioxel_size
-        container_obj['bioxels_max'] = bioxels_max
-        container_obj['bioxels_min'] = bioxels_min
-        container_obj['bioxels_offset'] = bioxels_offset
-        container_obj['bioxels_shape'] = bioxels_shape
-
-        bpy.ops.object.modifier_add(type='NODES')
-        container_obj.modifiers[0].node_group = node_tree
-        container_obj.modifiers[0].show_in_editmode = False
-        container_obj.modifiers[0].show_viewport = False
-        container_obj.modifiers[0].show_render = False
+            print(f"Creating layer ...")
 
-        # Create BioxelNodes to VDB object
-        print(f"Creating BioxelNodes to the VDB...")
-
-        if preferences.do_add_segmentnode:
+            bpy.ops.node.new_geometry_nodes_modifier()
+            node_tree = layer.modifiers[0].node_group
             nodes = node_tree.nodes
             links = node_tree.links
 
             input_node = get_node_by_type(nodes, 'NodeGroupInput')[0]
             output_node = get_node_by_type(nodes, 'NodeGroupOutput')[0]
 
-            segment_node = custom_nodes.add_node(
-                nodes, 'BioxelNodes_Segment')
+            to_layer_node = custom_nodes.add_node(nodes, "BioxelNodes__ConvertToLayer")
+
+            links.new(input_node.outputs[0], to_layer_node.inputs[0])
+            links.new(to_layer_node.outputs[0], output_node.inputs[0])
+
+            to_layer_node.inputs['Bioxel Size'].default_value = bioxel_size
+            to_layer_node.inputs['Shape'].default_value = layer_shape
+            to_layer_node.inputs['Origin'].default_value = layer_origin
+            to_layer_node.inputs['Rotation'].default_value = layer_rotation
+
+            return layer
+
+        if self.read_as == "labels":
+            orig_max = int(np.max(array))
+            orig_min = int(np.min(array))
+            layer_name = self.layer_name or "Label"
+
+            for i in range(orig_max):
+                label = array == np.full_like(array, i+1)
+                layer = create_layer(array=label,
+                                     layer_name=f"{container_name}_{layer_name}_{i+1}",
+                                     layer_type="label")
+
+                output_node = get_node_by_type(container_node_tree.nodes,
+                                               'NodeGroupOutput')[0]
+                mask_node = custom_nodes.add_node(container_node_tree.nodes,
+                                                  'BioxelNodes_MaskByLabel')
+                mask_node.inputs[0].default_value = layer
+                if len(output_node.inputs[0].links) == 0:
+                    container_node_tree.links.new(mask_node.outputs[0],
+                                                  output_node.inputs[0])
+
+        else:
+            if self.invert_scalar:
+                array = -array
+
+            orig_max = float(np.max(array))
+            orig_min = float(np.min(array))
+            orig_median = float(np.median(array))
+            orig_percentile80 = float(np.percentile(array, 80)) \
+                if self.invert_scalar else float(np.percentile(array, 80))
+
+            stats_table = [("Max", orig_max),
+                           ("Min", orig_min),
+                           ("Median", orig_median),
+                           ("80%", orig_percentile80)]
+
+            print("Volume Data Stats:")
+            for stats in stats_table:
+                print("| {: >10} | {: >40} |".format(*stats))
+
+            scalar_offset = 0
+            if orig_min < 0:
+                scalar_offset = -orig_min
+                array = array + np.full_like(array, scalar_offset)
 
-            segment_node.inputs['Threshold'].default_value = bioxels_default_threshold
+            layer_name = self.layer_name or "Scalar"
+            layer = create_layer(array=array,
+                                 layer_name=f"{container_name}_{layer_name}",
+                                 layer_type="scalar")
+
+            layer_node_tree = layer.modifiers[0].node_group
+            to_layer_node = layer_node_tree.nodes['BioxelNodes__ConvertToLayer']
+            to_layer_node.inputs['Scalar Offset'].default_value = scalar_offset
+            to_layer_node.inputs['Scalar Max'].default_value = orig_max
+            to_layer_node.inputs['Scalar Min'].default_value = orig_min
+
+            output_node = get_node_by_type(container_node_tree.nodes,
+                                           'NodeGroupOutput')[0]
+            mask_node = custom_nodes.add_node(container_node_tree.nodes,
+                                              'BioxelNodes_MaskByThreshold')
+            mask_node.inputs[0].default_value = layer
+
+            if len(output_node.inputs[0].links) == 0:
+                container_node_tree.links.new(mask_node.outputs[0],
+                                              output_node.inputs[0])
 
-            links.new(input_node.outputs[0], segment_node.inputs[0])
-            links.new(segment_node.outputs[0], output_node.inputs[0])
+        bpy.context.view_layer.objects.active = container
 
         # Change render setting for better result
         if preferences.do_change_render_setting:
             bpy.context.scene.render.engine = 'CYCLES'
             bpy.context.scene.cycles.volume_bounces = 12
-            bpy.context.scene.cycles.transparent_max_bounces = 64
+            bpy.context.scene.cycles.transparent_max_bounces = 16
+            bpy.context.scene.cycles.volume_preview_step_rate = 10
 
         self.report({"INFO"}, "Successfully Imported")
 
         return {'FINISHED'}
 
     def invoke(self, context, event):
-        min_size = min(
-            self.orig_spacing[0], self.orig_spacing[1], self.orig_spacing[2])
-        default_size = 1.0
-        self.bioxel_size = min_size if min_size > default_size else default_size
-        context.window_manager.invoke_props_dialog(self, width=400)
+        context.window_manager.invoke_props_dialog(self, width=500)
         return {'RUNNING_MODAL'}
 
     def draw(self, context):
-        layout = self.layout
-        bioxels_shape = get_bioxels_shape(
+        layer_shape = get_layer_shape(
             self.bioxel_size, self.orig_shape, self.orig_spacing)
-        bioxel_count = bioxels_shape[0] * bioxels_shape[1] * bioxels_shape[2]
-        text = f"Shape will be: {str(bioxels_shape)} {bioxel_count:,} "
+        bioxel_count = layer_shape[0] * layer_shape[1] * layer_shape[2]
+        text = f"Shape will be: {str(layer_shape)} {bioxel_count:,} "
         if bioxel_count > 100000000:
             text += "**TOO LARGE!**"
 
+        layout = self.layout
+        panel = layout.box()
+        panel.prop(self, "container_name")
+        panel.prop(self, "layer_name")
+
         panel = layout.box()
         panel.prop(self, "resample_method")
         panel.prop(self, "bioxel_size")
         row = panel.row()
         row.prop(self, "orig_spacing")
         panel.label(text=text)
 
         panel = layout.box()
+        panel.prop(self, "do_orient")
+
+        panel = layout.box()
         panel.prop(self, "read_as")
         if self.read_as == "labels":
-            panel.prop(self, "label_index")
+            ...
         else:
             panel.prop(self, "invert_scalar")
 
         panel = layout.box()
         panel.prop(self, "scene_scale")
-        panel.prop(self, "do_orient")
 
 
 def get_series_ids(self, context):
     items = []
     for index, series_id in enumerate(self.series_ids):
         items.append((
             series_id.id,
@@ -526,22 +588,23 @@
             "",
             index
         ))
 
     return items
 
 
-class ReadDICOM(bpy.types.Operator):
-    bl_idname = "bioxelnodes.read_dicom"
-    bl_label = "Volume Data as Bioxels"
-    bl_description = "Import Volume Data as Bioxels (VDB)"
+class ParseVolumeData(bpy.types.Operator):
+    bl_idname = "bioxelnodes.parse_volume_data"
+    bl_label = "Volume Data as Bioxel Layer"
+    bl_description = "Import Volume Data as Bioxel Layer"
     bl_options = {'UNDO'}
 
     filepath: bpy.props.StringProperty(subtype="FILE_PATH")  # type: ignore
     directory: bpy.props.StringProperty(subtype='DIR_PATH')  # type: ignore
+    container: bpy.props.StringProperty()   # type: ignore
 
     series_id: bpy.props.EnumProperty(
         name="Select Series",
         items=get_series_ids
     )  # type: ignore
 
     series_ids: bpy.props.CollectionProperty(
@@ -551,33 +614,49 @@
         ext = get_ext(self.filepath)
         if ext not in SUPPORT_EXTS:
             self.report({"WARNING"}, "Not supported extension.")
             return {'CANCELLED'}
 
         print("Collecting Meta Data...")
         image, name = read_image(self.filepath, self.series_id)
+
         stats_table = [("Shape", str(image.GetSize())),
                        ("Spacing", str(image.GetSpacing())),
                        ("Origin", str(image.GetOrigin())),
                        ("Direction", str(image.GetDirection())),
                        ("Data Type", image.GetPixelIDTypeAsString())]
+        for k in image.GetMetaDataKeys():
+            stats_table.append((k, str(image.GetMetaData(k))))
 
         print("Meta Data:")
         for stats in stats_table:
-            print("| {: >10} | {: >40} |".format(*stats))
+            print("| {: >20} | {: >100} |".format(*stats))
 
         do_orient = ext not in SEQUENCE_EXTS or ext in DICOM_EXTS
 
+        orig_shape = image.GetSize()
+        orig_spacing = image.GetSpacing()
+        min_size = min(orig_spacing[0], orig_spacing[1], orig_spacing[2])
+        bioxel_size = max(min_size, 1.0)
+        if self.container:
+            container = bpy.data.objects[self.container]
+            container_name = container.name
+        else:
+            container_name = name
+
         bpy.ops.bioxelnodes.import_volume_data_dialog(
             'INVOKE_DEFAULT',
             filepath=self.filepath,
-            orig_shape=image.GetSize(),
-            orig_spacing=image.GetSpacing(),
+            container_name=container_name,
+            orig_shape=orig_shape,
+            orig_spacing=orig_spacing,
+            bioxel_size=bioxel_size,
             series_id=self.series_id or "",
-            do_orient=do_orient
+            do_orient=do_orient,
+            container=self.container
         )
 
         self.report({"INFO"}, "Successfully Readed.")
 
         return {'FINISHED'}
 
     def modal(self, context, event):
@@ -619,23 +698,23 @@
             text="Reading image data, it may take a while...")
         layout.label(
             text="Please be patient...")
 
 
 class ImportVolumeData(bpy.types.Operator):
     bl_idname = "bioxelnodes.import_volume_data"
-    bl_label = "Volume Data as Bioxels"
-    bl_description = "Import Volume Data as Bioxels (VDB)"
+    bl_label = "Volume Data as Bioxel Layer"
+    bl_description = "Import Volume Data as Bioxel Layer"
     bl_options = {'UNDO'}
 
     filepath: bpy.props.StringProperty(subtype="FILE_PATH")  # type: ignore
     directory: bpy.props.StringProperty(subtype='DIR_PATH')  # type: ignore
 
     def execute(self, context):
-        bpy.ops.bioxelnodes.read_dicom(
+        bpy.ops.bioxelnodes.parse_volume_data(
             'INVOKE_DEFAULT',
             filepath=self.filepath,
             directory=self.directory
         )
         return {'FINISHED'}
 
     def invoke(self, context, event):
@@ -643,58 +722,81 @@
         return {'RUNNING_MODAL'}
 
 
 try:
     class BIOXELNODES_FH_ImportVolumeData(bpy.types.FileHandler):
         bl_idname = "BIOXELNODES_FH_ImportVolumeData"
         bl_label = "File handler for dicom import"
-        bl_import_operator = "bioxelnodes.read_dicom"
+        bl_import_operator = "bioxelnodes.parse_volume_data"
         bl_file_extensions = ";".join(FH_EXTS)
 
         @classmethod
         def poll_drop(cls, context):
             return (context.area and context.area.type == 'VIEW_3D')
 except:
     ...
 
 
+class AddVolumeData(bpy.types.Operator):
+    bl_idname = "bioxelnodes.add_volume_data"
+    bl_label = "Add Volume Data to Container"
+    bl_description = "Add Volume Data to Container"
+    bl_options = {'UNDO'}
+
+    filepath: bpy.props.StringProperty(subtype="FILE_PATH")  # type: ignore
+    directory: bpy.props.StringProperty(subtype='DIR_PATH')  # type: ignore
+
+    @classmethod
+    def poll(cls, context):
+        container = get_container(bpy.context.active_object)
+        return True if container else False
+
+    def execute(self, context):
+        container = get_container(bpy.context.active_object)
+
+        bpy.ops.bioxelnodes.parse_volume_data(
+            'INVOKE_DEFAULT',
+            filepath=self.filepath,
+            directory=self.directory,
+            container=container.name
+        )
+        return {'FINISHED'}
+
+    def invoke(self, context, event):
+        context.window_manager.fileselect_add(self)
+        return {'RUNNING_MODAL'}
+
+
 class ExportVDB(bpy.types.Operator):
     bl_idname = "bioxelnodes.export_vdb"
-    bl_label = "Bioxels as VDB"
-    bl_description = "Export Bioxels original VDB data"
+    bl_label = "Bioxel Layer as VDB"
+    bl_description = "Export Bioxel Layer as VDB"
     bl_options = {'UNDO'}
 
     filepath: bpy.props.StringProperty(
         subtype="FILE_PATH"
     )  # type: ignore
 
     filename_ext = ".vdb"
 
     @classmethod
     def poll(cls, context):
-        bioxels_obj = None
-        for obj in bpy.context.selected_objects:
-            bioxels_obj = get_bioxels_obj(obj)
-            break
-
-        return True if bioxels_obj else False
+        layer = get_layer(bpy.context.active_object)
+        return True if layer else False
 
     def invoke(self, context, event):
         context.window_manager.fileselect_add(self)
         return {'RUNNING_MODAL'}
 
     def execute(self, context):
-        bioxels_obj = None
-        for obj in bpy.context.selected_objects:
-            bioxels_obj = get_bioxels_obj(obj)
-            break
+        layer = get_layer(bpy.context.active_object)
 
         filepath = f"{self.filepath.split('.')[0]}.vdb"
         # "//"
-        source_dir = bpy.path.abspath(bioxels_obj.data.filepath)
+        source_dir = bpy.path.abspath(layer.data.filepath)
 
         output_path: Path = Path(filepath).resolve()
         source_path: Path = Path(source_dir).resolve()
         # print('output_path', output_path)
         # print('source_path', source_path)
         shutil.copy(source_path, output_path)
```

### Comparing `bioxelnodes-0.1.1/bioxelnodes/io_points.py` & `bioxelnodes-0.2.0/bioxelnodes/io_points.py`

 * *Files identical despite different names*

### Comparing `bioxelnodes-0.1.1/bioxelnodes/preferences.py` & `bioxelnodes-0.2.0/bioxelnodes/preferences.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,19 +8,14 @@
 
     cache_dir: bpy.props.StringProperty(
         name="Set Cache Directory",
         subtype='DIR_PATH',
         default=str(Path(Path.home(), '.bioxelnodes'))
     )  # type: ignore
 
-    do_add_segmentnode: bpy.props.BoolProperty(
-        name="Add Segment Node",
-        default=True,
-    )  # type: ignore
-
     do_change_render_setting: bpy.props.BoolProperty(
         name="Change Render Setting",
         default=True,
     )  # type: ignore
 
     def draw(self, context):
         layout = self.layout
@@ -29,8 +24,7 @@
         self.requirements_dir = str(Path(__file__).parent)
         super().draw(context)
 
         layout.label(text="Configuration")
         layout.prop(self, 'cache_dir')
 
         layout.prop(self, "do_change_render_setting")
-        layout.prop(self, "do_add_segmentnode")
```

### Comparing `bioxelnodes-0.1.1/bioxelnodes/utils.py` & `bioxelnodes-0.2.0/bioxelnodes/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 def get_type(cls):
     return type(cls).__name__
 
 
 def get_node_by_type(nodes, type_name: str):
     return [node for node in nodes if get_type(node) == type_name]
 
+
 def show_message(message="", title="Message Box", icon='INFO'):
 
     def draw(self, context):
         self.layout.label(text=message)
 
     bpy.context.window_manager.popup_menu(draw, title=title, icon=icon)
 
@@ -63,41 +64,65 @@
             bbox_origin[1] + bbox_size[1],
             bbox_origin[2] + bbox_size[2],
         ),
     ]
     return bbox_verts
 
 
-def get_bioxels_obj(current_obj):
-    bioxels_obj = None
-    if current_obj.get('bioxels_container'):
-        bioxels_values = []
-        for obj in bpy.data.objects:
-            if obj.parent == current_obj and obj.get('bioxels'):
-                bioxels_values.append(obj)
-
-        if len(bioxels_values) > 0:
-            bioxels_obj = bioxels_values[0]
-
-    elif current_obj.get('bioxels') and current_obj.parent:
-        if current_obj.parent.get('bioxels_container'):
-            bioxels_obj = current_obj
+def lock_transform(obj):
+    obj.lock_location[0] = True
+    obj.lock_location[1] = True
+    obj.lock_location[2] = True
+    obj.lock_rotation[0] = True
+    obj.lock_rotation[1] = True
+    obj.lock_rotation[2] = True
+    obj.lock_scale[0] = True
+    obj.lock_scale[1] = True
+    obj.lock_scale[2] = True
+
+
+def hide_in_ray(obj):
+    obj.visible_camera = False
+    obj.visible_diffuse = False
+    obj.visible_glossy = False
+    obj.visible_transmission = False
+    obj.visible_volume_scatter = False
+    obj.visible_shadow = False
+
+
+def get_container(current_obj):
+    if current_obj:
+        return current_obj if current_obj.get('bioxel_container') else None
+    return None
+
+
+def get_layer(current_obj):
+    if current_obj:
+        if current_obj.get('bioxel_layer') and current_obj.parent:
+            if current_obj.parent.get('bioxel_container'):
+                return current_obj
+    return None
+
 
-    return bioxels_obj
+def get_container_layers(container):
+    layers = []
+    for obj in bpy.data.objects:
+        if obj.parent == container and get_layer(obj):
+            layers.append(obj)
 
+    return layers
 
-def get_all_bioxels_objs():
-    bioxels_objs = []
 
+def get_all_layers():
+    layers = []
     for obj in bpy.data.objects:
-        if obj.parent:
-            if obj.parent.get('bioxels_container') and obj.get('bioxels'):
-                bioxels_objs.append(obj)
+        if get_layer(obj):
+            layers.append(obj)
 
-    return list(set(bioxels_objs))
+    return layers
 
 
 def get_text_index_str(text):
     # Initialize an empty string to store the digits
     digits = ""
 
     # Iterate through the characters in reverse order
```

### Comparing `bioxelnodes-0.1.1/LICENSE` & `bioxelnodes-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bioxelnodes-0.1.1/pyproject.toml` & `bioxelnodes-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bioxelnodes"
-version = "0.1.1"
+version = "0.2.0"
 description = ""
 authors = ["Ma Nan <icrdr2010@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "~=3.10.0"
```

### Comparing `bioxelnodes-0.1.1/README.md` & `bioxelnodes-0.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 ![Static Badge](https://img.shields.io/badge/Blender-orange?style=for-the-badge&logo=blender&logoColor=white)
 ![GitHub License](https://img.shields.io/github/license/OmooLab/BioxelNodes?style=for-the-badge)
 ![GitHub Release](https://img.shields.io/github/v/release/OmooLab/BioxelNodes?style=for-the-badge)
 ![GitHub Repo stars](https://img.shields.io/github/stars/OmooLab/BioxelNodes?style=for-the-badge)
 
 Bioxel Nodes is a Blender add-on for scientific volumetric data visualization. It using Blender's powerful Geometry Nodes | Cycles to process and render volumetric data.
 
-# About
+## About
 
 Before us, there have been many tutorials and add-ons for importing volumetric data into Blender. However, we found that there were many details that were not addressed in place, some scientific facts were ignored, and the volume rendering was not pretty enough. With Bioxel Nodes, you can easily import the volumetric data into Blender, and more importantly, it can quickly make a beautiful realistic rendering of it.
 
 Below are some examples with Bioxel Nodes. Thanks to Cycles Render, the volumetric data can be rendered with great detail:
 
 ![gallery](docs/assets/gallery.png)
 
-The "Bioxel" in "BioxelNodes", is a combination of the words "Bio-" and "Voxel". Bioxel is a voxel that stores biological data. The volumetric data made up of Bioxel is called Bioxels. We are developing a toolkit around Bioxels for better biological data visualization. but before its release, we made this Blender version of bioxels toolkit first, in order to let more people to have fun with volumetric data. [Getting Started](https://omoolab.github.io/BioxelNodes/latest/getting-started)
+The "Bioxel" in "Bioxel Nodes", is a combination of the words "Bio-" and "Voxel". Bioxel is a voxel that stores biological data. We are developing a toolkit around Bioxel for better biological data visualization. but before its release, we made this Blender version of bioxels toolkit first, in order to let more people to have fun with volumetric data. [Getting Started](https://omoolab.github.io/BioxelNodes/latest/getting-started)
 
-# Supported Format
+## Supported Format
 
 | Format | EXT                                      | Test    |
 | ------ | ---------------------------------------- | ------- |
 | DICOM  | .dcm, .DICOM                             | ✅ pass |
 | BMP    | .bmp, .BMP                               | ✅ pass |
 | JPEG   | .jpg, .JPG, .jpeg, .JPEG                 | ✅ pass |
 | PNG    | .png, .PNG                               | ✅ pass |
@@ -35,11 +35,24 @@
 | VTK    | .vtk                                     | yet     |
 | BioRad | .PIC, .pic                               | yet     |
 | Gipl   | .gipl, .gipl.gz                          | yet     |
 | LSM    | .lsm, .LSM                               | yet     |
 | MINC   | .mnc, .MNC                               | yet     |
 | MRC    | .mrc, .rec                               | yet     |
 
-# Known limitations
+## Known Limitations
 
-- Sections cannot be generated
-- Time sequence volume not supported (will be supported soon)
+-   Sections cannot be generated (will be supported soon)
+-   Time sequence volume not supported (will be supported soon)
+
+## To Upgrade Add-on
+
+To upgrade from an older version of the add-on to the latest, you need to do the following:
+
+1. Remove the old version of Bioxel Nodes at Preferences > Add-ons
+2. Add the new version and restart Blender.
+
+It is not support editing the same blender file across add-on versions. In order to make sure that the previous file works properly. You need to save the staged data before upgrading ( read the last section of [Getting Started](https://omoolab.github.io/BioxelNodes/latest/getting-started/#share-your-file) ).
+
+But even then, there is still no guarantee that the new version of the add-on will work on the old blender file. Therefore, it is highly recommended to open a new blender file to start the creating, not based on the old one.
+
+Alternatively, objects from the old file that have nothing to do with Bioxel Nodes could be append to the new blender file.
```

### Comparing `bioxelnodes-0.1.1/PKG-INFO` & `bioxelnodes-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioxelnodes
-Version: 0.1.1
+Version: 0.2.0
 Summary: 
 License: MIT
 Author: Ma Nan
 Author-email: icrdr2010@outlook.com
 Requires-Python: >=3.10.0,<3.11.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,25 +20,25 @@
 ![Static Badge](https://img.shields.io/badge/Blender-orange?style=for-the-badge&logo=blender&logoColor=white)
 ![GitHub License](https://img.shields.io/github/license/OmooLab/BioxelNodes?style=for-the-badge)
 ![GitHub Release](https://img.shields.io/github/v/release/OmooLab/BioxelNodes?style=for-the-badge)
 ![GitHub Repo stars](https://img.shields.io/github/stars/OmooLab/BioxelNodes?style=for-the-badge)
 
 Bioxel Nodes is a Blender add-on for scientific volumetric data visualization. It using Blender's powerful Geometry Nodes | Cycles to process and render volumetric data.
 
-# About
+## About
 
 Before us, there have been many tutorials and add-ons for importing volumetric data into Blender. However, we found that there were many details that were not addressed in place, some scientific facts were ignored, and the volume rendering was not pretty enough. With Bioxel Nodes, you can easily import the volumetric data into Blender, and more importantly, it can quickly make a beautiful realistic rendering of it.
 
 Below are some examples with Bioxel Nodes. Thanks to Cycles Render, the volumetric data can be rendered with great detail:
 
 ![gallery](docs/assets/gallery.png)
 
-The "Bioxel" in "BioxelNodes", is a combination of the words "Bio-" and "Voxel". Bioxel is a voxel that stores biological data. The volumetric data made up of Bioxel is called Bioxels. We are developing a toolkit around Bioxels for better biological data visualization. but before its release, we made this Blender version of bioxels toolkit first, in order to let more people to have fun with volumetric data. [Getting Started](https://omoolab.github.io/BioxelNodes/latest/getting-started)
+The "Bioxel" in "Bioxel Nodes", is a combination of the words "Bio-" and "Voxel". Bioxel is a voxel that stores biological data. We are developing a toolkit around Bioxel for better biological data visualization. but before its release, we made this Blender version of bioxels toolkit first, in order to let more people to have fun with volumetric data. [Getting Started](https://omoolab.github.io/BioxelNodes/latest/getting-started)
 
-# Supported Format
+## Supported Format
 
 | Format | EXT                                      | Test    |
 | ------ | ---------------------------------------- | ------- |
 | DICOM  | .dcm, .DICOM                             | ✅ pass |
 | BMP    | .bmp, .BMP                               | ✅ pass |
 | JPEG   | .jpg, .JPG, .jpeg, .JPEG                 | ✅ pass |
 | PNG    | .png, .PNG                               | ✅ pass |
@@ -50,12 +50,25 @@
 | VTK    | .vtk                                     | yet     |
 | BioRad | .PIC, .pic                               | yet     |
 | Gipl   | .gipl, .gipl.gz                          | yet     |
 | LSM    | .lsm, .LSM                               | yet     |
 | MINC   | .mnc, .MNC                               | yet     |
 | MRC    | .mrc, .rec                               | yet     |
 
-# Known limitations
+## Known Limitations
 
-- Sections cannot be generated
-- Time sequence volume not supported (will be supported soon)
+-   Sections cannot be generated (will be supported soon)
+-   Time sequence volume not supported (will be supported soon)
+
+## To Upgrade Add-on
+
+To upgrade from an older version of the add-on to the latest, you need to do the following:
+
+1. Remove the old version of Bioxel Nodes at Preferences > Add-ons
+2. Add the new version and restart Blender.
+
+It is not support editing the same blender file across add-on versions. In order to make sure that the previous file works properly. You need to save the staged data before upgrading ( read the last section of [Getting Started](https://omoolab.github.io/BioxelNodes/latest/getting-started/#share-your-file) ).
+
+But even then, there is still no guarantee that the new version of the add-on will work on the old blender file. Therefore, it is highly recommended to open a new blender file to start the creating, not based on the old one.
+
+Alternatively, objects from the old file that have nothing to do with Bioxel Nodes could be append to the new blender file.
```

