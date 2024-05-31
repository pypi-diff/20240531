# Comparing `tmp/vbr_devkit-0.0.3.tar.gz` & `tmp/vbr_devkit-0.0.4.tar.gz`

## Comparing `vbr_devkit-0.0.3.tar` & `vbr_devkit-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/datasets/__init__.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/datasets/convert_bag.py
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/datasets/kitti.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/datasets/ros.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/download/__init__.py
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/download/download_data.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/pybind/CMakeLists.txt
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/pybind/stl_vector_eigen.h
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/pybind/vbr_devkit_pybind.cpp
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/tools/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/tools/console.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/tools/image.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/tools/imu.py
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/tools/point_cloud2.py
--rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/tools/run.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/LICENSE
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/README.md
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 vbr_devkit-0.0.4/vbr_devkit/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 vbr_devkit-0.0.4/vbr_devkit/datasets/__init__.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 vbr_devkit-0.0.4/vbr_devkit/datasets/convert_bag.py
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 vbr_devkit-0.0.4/vbr_devkit/datasets/kitti.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 vbr_devkit-0.0.4/vbr_devkit/datasets/ros.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vbr_devkit-0.0.4/vbr_devkit/download/__init__.py
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 vbr_devkit-0.0.4/vbr_devkit/download/download_data.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 vbr_devkit-0.0.4/vbr_devkit/pybind/CMakeLists.txt
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 vbr_devkit-0.0.4/vbr_devkit/pybind/stl_vector_eigen.h
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 vbr_devkit-0.0.4/vbr_devkit/pybind/vbr_devkit_pybind.cpp
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 vbr_devkit-0.0.4/vbr_devkit/tools/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 vbr_devkit-0.0.4/vbr_devkit/tools/console.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 vbr_devkit-0.0.4/vbr_devkit/tools/image.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 vbr_devkit-0.0.4/vbr_devkit/tools/imu.py
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 vbr_devkit-0.0.4/vbr_devkit/tools/point_cloud2.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 vbr_devkit-0.0.4/vbr_devkit/tools/run.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 vbr_devkit-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 vbr_devkit-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 vbr_devkit-0.0.4/README.md
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 vbr_devkit-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 vbr_devkit-0.0.4/PKG-INFO
```

### Comparing `vbr_devkit-0.0.3/vbr_devkit/datasets/convert_bag.py` & `vbr_devkit-0.0.4/vbr_devkit/datasets/convert_bag.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 import sys
-sys.path.append("/home/eg/source/vbr-devkit/python")
 
 from pathlib import Path
 
 from vbr_devkit.datasets import KittiWriter, RosReader
 import typer
 from enum import Enum
 from rich.progress import track
+from rosbags import convert
 
 
 class OutputDataInterface(str, Enum):
     kitti = "kitti",
+    ros2  = "ros2",
     # Can insert additional conversion formats
 
 
 OutputDataInterface_lut = {
     OutputDataInterface.kitti: KittiWriter
 }
 
 def main(to: OutputDataInterface, input_dir: Path, output_dir: Path) -> None:
-    with RosReader(input_dir) as reader:
-        with OutputDataInterface_lut[to](output_dir) as writer:
-            for timestamp, topic, message in track(reader, description="Processing..."):
-                writer.publish(timestamp, topic, message)
+    if to == OutputDataInterface.ros2:
+        if not input_dir.is_dir():
+            print("Processing...")
+            convert.convert(input_dir, output_dir / input_dir.stem)
+        else:
+            for item in track(list(input_dir.iterdir()), description="Processing..."):
+                if item.suffix == '.bag':
+                    convert.convert(item, output_dir / item.stem)
+    else:
+        with RosReader(input_dir) as reader:
+            with OutputDataInterface_lut[to](output_dir) as writer:
+                for timestamp, topic, message in track(reader, description="Processing..."):
+                    writer.publish(timestamp, topic, message)
 
 
 if __name__ == "__main__":
     typer.run(main)
```

### Comparing `vbr_devkit-0.0.3/vbr_devkit/datasets/kitti.py` & `vbr_devkit-0.0.4/vbr_devkit/datasets/kitti.py`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.3/vbr_devkit/datasets/ros.py` & `vbr_devkit-0.0.4/vbr_devkit/datasets/ros.py`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.3/vbr_devkit/download/download_data.py` & `vbr_devkit-0.0.4/vbr_devkit/download/download_data.py`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.3/vbr_devkit/pybind/CMakeLists.txt` & `vbr_devkit-0.0.4/vbr_devkit/pybind/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.3/vbr_devkit/pybind/stl_vector_eigen.h` & `vbr_devkit-0.0.4/vbr_devkit/pybind/stl_vector_eigen.h`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.3/vbr_devkit/pybind/vbr_devkit_pybind.cpp` & `vbr_devkit-0.0.4/vbr_devkit/pybind/vbr_devkit_pybind.cpp`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.3/vbr_devkit/tools/__init__.py` & `vbr_devkit-0.0.4/vbr_devkit/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.3/vbr_devkit/tools/image.py` & `vbr_devkit-0.0.4/vbr_devkit/tools/image.py`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.3/vbr_devkit/tools/imu.py` & `vbr_devkit-0.0.4/vbr_devkit/tools/imu.py`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.3/vbr_devkit/tools/point_cloud2.py` & `vbr_devkit-0.0.4/vbr_devkit/tools/point_cloud2.py`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.3/vbr_devkit/tools/run.py` & `vbr_devkit-0.0.4/vbr_devkit/tools/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import sys
 
-sys.path.append("/home/eg/source/vbr-devkit/python")
 import typer
 from pathlib import Path
 from rich.console import Group
 from rich.panel import Panel
 from rich.progress import track
 from typing import Sequence
 from typing_extensions import Annotated
```

### Comparing `vbr_devkit-0.0.3/LICENSE` & `vbr_devkit-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.3/README.md` & `vbr_devkit-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.3/pyproject.toml` & `vbr_devkit-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "vbr-devkit"
-version = "0.0.3"
+version = "0.0.4"
 description = "Development kit for VBR SLAM dataset"
 readme = "README.md"
 authors = [
     { name = "Emanuele Giacomini", email = "giacomini@diag.uniroma1.it" },
 ]
 requires-python = ">=3.8"
```

### Comparing `vbr_devkit-0.0.3/PKG-INFO` & `vbr_devkit-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: vbr-devkit
-Version: 0.0.3
+Version: 0.0.4
 Summary: Development kit for VBR SLAM dataset
 Project-URL: Homepage, https://github.com/rvp-group/vbr-devkit
 Project-URL: Issues, https://github.com/rvp-group/vbr-devkit/issues
 Author-email: Emanuele Giacomini <giacomini@diag.uniroma1.it>
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: natsort
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: vbr-devkit Version: 0.0.3 Summary: Development kit
+Metadata-Version: 2.3 Name: vbr-devkit Version: 0.0.4 Summary: Development kit
 for VBR SLAM dataset Project-URL: Homepage, https://github.com/rvp-group/vbr-
 devkit Project-URL: Issues, https://github.com/rvp-group/vbr-devkit/issues
 Author-email: Emanuele Giacomini
 diag.uniroma1.it> License-File: LICENSE Requires-Python: >=3.8 Requires-Dist:
 natsort Requires-Dist: numpy Requires-Dist: rich Requires-Dist: rosbags
 Requires-Dist: rosbags-image Requires-Dist: typer[all]>=0.10.0 Description-
 Content-Type: text/markdown
```

