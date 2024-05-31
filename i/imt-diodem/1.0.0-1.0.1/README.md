# Comparing `tmp/imt_diodem-1.0.0.tar.gz` & `tmp/imt_diodem-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imt_diodem-1.0.0.tar", last modified: Thu May 30 14:45:05 2024, max compression
+gzip compressed data, was "imt_diodem-1.0.1.tar", last modified: Fri May 31 11:40:59 2024, max compression
```

## Comparing `imt_diodem-1.0.0.tar` & `imt_diodem-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:45:05.608374 imt_diodem-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-30 14:45:05.608374 imt_diodem-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-30 14:44:58.000000 imt_diodem-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-30 14:44:58.000000 imt_diodem-1.0.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-30 14:45:05.608374 imt_diodem-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:45:05.604374 imt_diodem-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:45:05.608374 imt_diodem-1.0.0/src/diodem/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-30 14:44:58.000000 imt_diodem-1.0.0/src/diodem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-30 14:44:58.000000 imt_diodem-1.0.0/src/diodem/_src.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:45:05.608374 imt_diodem-1.0.0/src/diodem/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-30 14:44:58.000000 imt_diodem-1.0.0/src/diodem/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-05-30 14:44:58.000000 imt_diodem-1.0.0/src/diodem/benchmark/_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:45:05.608374 imt_diodem-1.0.0/src/diodem/benchmark/xmls/
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-30 14:44:58.000000 imt_diodem-1.0.0/src/diodem/benchmark/xmls/arm.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-30 14:44:58.000000 imt_diodem-1.0.0/src/diodem/benchmark/xmls/gait.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-30 14:44:58.000000 imt_diodem-1.0.0/src/diodem/dataverse_github.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-30 14:44:58.000000 imt_diodem-1.0.0/src/diodem/test_dataverse_github.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-30 14:44:58.000000 imt_diodem-1.0.0/src/diodem/test_src.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-30 14:44:58.000000 imt_diodem-1.0.0/src/diodem/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-05-30 14:44:58.000000 imt_diodem-1.0.0/src/diodem/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:45:05.608374 imt_diodem-1.0.0/src/imt_diodem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-30 14:45:05.000000 imt_diodem-1.0.0/src/imt_diodem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-30 14:45:05.000000 imt_diodem-1.0.0/src/imt_diodem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:45:05.000000 imt_diodem-1.0.0/src/imt_diodem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-30 14:45:05.000000 imt_diodem-1.0.0/src/imt_diodem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 14:45:05.000000 imt_diodem-1.0.0/src/imt_diodem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:40:59.700289 imt_diodem-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-31 11:40:59.700289 imt_diodem-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-31 11:40:55.000000 imt_diodem-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-31 11:40:55.000000 imt_diodem-1.0.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-31 11:40:59.700289 imt_diodem-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:40:59.696289 imt_diodem-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:40:59.696289 imt_diodem-1.0.1/src/diodem/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-31 11:40:55.000000 imt_diodem-1.0.1/src/diodem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-31 11:40:55.000000 imt_diodem-1.0.1/src/diodem/_src.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:40:59.700289 imt_diodem-1.0.1/src/diodem/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-31 11:40:55.000000 imt_diodem-1.0.1/src/diodem/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-05-31 11:40:55.000000 imt_diodem-1.0.1/src/diodem/benchmark/_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:40:59.700289 imt_diodem-1.0.1/src/diodem/benchmark/xmls/
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-31 11:40:55.000000 imt_diodem-1.0.1/src/diodem/benchmark/xmls/arm.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-05-31 11:40:55.000000 imt_diodem-1.0.1/src/diodem/benchmark/xmls/gait.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-31 11:40:55.000000 imt_diodem-1.0.1/src/diodem/dataverse_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-31 11:40:55.000000 imt_diodem-1.0.1/src/diodem/test_dataverse_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-31 11:40:55.000000 imt_diodem-1.0.1/src/diodem/test_src.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-31 11:40:55.000000 imt_diodem-1.0.1/src/diodem/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-31 11:40:55.000000 imt_diodem-1.0.1/src/diodem/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:40:59.700289 imt_diodem-1.0.1/src/imt_diodem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-31 11:40:59.000000 imt_diodem-1.0.1/src/imt_diodem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-31 11:40:59.000000 imt_diodem-1.0.1/src/imt_diodem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 11:40:59.000000 imt_diodem-1.0.1/src/imt_diodem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-31 11:40:59.000000 imt_diodem-1.0.1/src/imt_diodem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-31 11:40:59.000000 imt_diodem-1.0.1/src/imt_diodem.egg-info/top_level.txt
```

### Comparing `imt_diodem-1.0.0/PKG-INFO` & `imt_diodem-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imt-diodem
-Version: 1.0.0
+Version: 1.0.1
 Summary: DIODEM -- A Diverse Inertial and Optical Dataset of kinEmatic chain Motion
 Author-email: Simon Bachhuber <simon.bachhuber@fau.de>
 Project-URL: Homepage, https://github.com/SimiPixel/diodem
 Project-URL: Issues, https://github.com/SimiPixel/diodem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `imt_diodem-1.0.0/pyproject.toml` & `imt_diodem-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "imt-diodem"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Simon Bachhuber", email="simon.bachhuber@fau.de" },
 ]
 description = "DIODEM -- A Diverse Inertial and Optical Dataset of kinEmatic chain Motion"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `imt_diodem-1.0.0/readme.md` & `imt_diodem-1.0.1/readme.md`

 * *Files identical despite different names*

### Comparing `imt_diodem-1.0.0/src/diodem/_src.py` & `imt_diodem-1.0.1/src/diodem/_src.py`

 * *Files identical despite different names*

### Comparing `imt_diodem-1.0.0/src/diodem/benchmark/_benchmark.py` & `imt_diodem-1.0.1/src/diodem/benchmark/_benchmark.py`

 * *Files identical despite different names*

### Comparing `imt_diodem-1.0.0/src/diodem/benchmark/xmls/arm.xml` & `imt_diodem-1.0.1/src/diodem/benchmark/xmls/arm.xml`

 * *Files identical despite different names*

### Comparing `imt_diodem-1.0.0/src/diodem/benchmark/xmls/gait.xml` & `imt_diodem-1.0.1/src/diodem/benchmark/xmls/gait.xml`

 * *Files 20% similar despite different names*

#### Comparing `imt_diodem-1.0.0/src/diodem/benchmark/xmls/gait.xml` & `imt_diodem-1.0.1/src/diodem/benchmark/xmls/gait.xml`

```diff
@@ -1,48 +1,58 @@
 <?xml version="1.0" encoding="utf-8"?>
 <x_xy model="gait">
   <options gravity="0 0 9.81" dt="0.01"/>
   <defaults>
     <geom edge_color="black" color="1 0.8 0.7 1"/>
   </defaults>
   <worldbody>
-    <body name="seg5" joint="free" euler="0 -90 0" damping="5 5 5 25 25 25">
+    <body name="seg5" joint="free" damping="5 5 5 25 25 25">
       <omc name="seg5" pos_marker="4" pos="0 0 -.02"/>
-      <geom type="box" mass="1" pos="0.1 0 0" dim="0.2 0.05 0.05"/>
+      <geom type="box" mass="1" pos="0.1 0 0" dim="0.2 0.05 0.05" color="dustin_exp_white"/>
+      <geom type="box" mass="0.1" pos="0.03 -0.05 0" dim="0.01 0.1 0.01" color="black"/>
+      <geom type="box" mass="0.1" pos="0.17 -0.05 0" dim="0.01 0.1 0.01" color="black"/>
       <body name="imu5" joint="frozen" pos="0.1 0.0 0.035" pos_min="0.05 -0.05 -0.05" pos_max="0.15 0.05 0.05">
         <omc name="seg5" pos_marker="4" pos=".1 0 .015"/>
-        <geom type="box" mass="0.1" dim="0.05 0.03 0.02" color="green"/>
+        <geom type="box" mass="0.1" dim="0.05 0.03 0.02" color="dustin_exp_orange"/>
       </body>
       <body name="seg1" joint="ry" pos="0.2 0 0" pos_min="0.15 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3">
         <omc name="seg1" pos_marker="2" pos="0 0 -.02"/>
-        <geom type="box" mass="1" pos="0.1 0 0" dim="0.2 0.05 0.05"/>
+        <geom type="box" mass="1" pos="0.1 0 0" dim="0.2 0.05 0.05" color="dustin_exp_blue"/>
+        <geom type="box" mass="0.1" pos="0.03 -0.05 0" dim="0.01 0.1 0.01" color="dustin_exp_white"/>
+        <geom type="box" mass="0.1" pos="0.17 0.05 0" dim="0.01 0.1 0.01" color="dustin_exp_white"/>
         <body name="imu1" joint="frozen" pos="0.1 0.0 0.035" pos_min="0.05 -0.05 -0.05" pos_max="0.15 0.05 0.05">
           <omc name="seg1" pos_marker="2" pos=".1 0 .015"/>
-          <geom type="box" mass="0.1" dim="0.05 0.03 0.02" color="orange"/>
+          <geom type="box" mass="0.1" dim="0.05 0.03 0.02" color="dustin_exp_orange"/>
         </body>
-        <body name="seg2" joint="saddle" pos="0.2 0 0" pos_min="0.15 -0.05 -0.05" pos_max="0.35 0.05 0.05" euler="0 0 90" damping="3 3">
+        <body name="seg2" joint="saddle" pos="0.2 0 0" pos_min="0.15 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3 3">
           <omc name="seg2" pos_marker="2" pos="0 0 -.02"/>
-          <geom type="box" mass="1" pos="0.1 0 0" dim="0.2 0.05 0.05"/>
+          <geom type="box" mass="1" pos="0.1 0 0" dim="0.2 0.05 0.05" color="dustin_exp_white"/>
+          <geom type="box" mass="0.1" pos="0.03 -0.05 0" dim="0.01 0.1 0.01" color="dustin_exp_white"/>
+          <geom type="box" mass="0.1" pos="0.17 -0.05 0" dim="0.01 0.1 0.01" color="dustin_exp_white"/>
           <body name="imu2" joint="frozen" pos="0.1 0.0 0.035" pos_min="0.05 -0.05 -0.05" pos_max="0.15 0.05 0.05">
             <omc name="seg2" pos_marker="2" pos=".1 0 .015"/>
-            <geom type="box" mass="0.1" dim="0.05 0.03 0.02" color="orange"/>
+            <geom type="box" mass="0.1" dim="0.05 0.03 0.02" color="dustin_exp_orange"/>
           </body>
-          <body name="seg3" joint="saddle" pos="0.2 0 0" pos_min="0.15 -0.05 -0.05" pos_max="0.35 0.05 0.05" euler="0 0 90" damping="3 3">
+          <body name="seg3" joint="saddle" pos="0.2 0 0" pos_min="0.15 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3 3">
             <omc name="seg3" pos_marker="1" pos="0 0 -.02"/>
-            <geom type="box" mass="1" pos="0.1 0 0" dim="0.2 0.05 0.05"/>
+            <geom type="box" mass="1" pos="0.1 0 0" dim="0.2 0.05 0.05" color="dustin_exp_blue"/>
+            <geom type="box" mass="0.1" pos="0.05 0.05 0" dim="0.01 0.1 0.01" color="black"/>
+            <geom type="box" mass="0.1" pos="0.15 -0.05 0" dim="0.01 0.1 0.01" color="black"/>
             <body name="imu3" joint="frozen" pos="0.1 0.0 0.035" pos_min="0.05 -0.05 -0.05" pos_max="0.15 0.05 0.05">
               <omc name="seg3" pos_marker="1" pos=".1 0 .015"/>
-              <geom type="box" mass="0.1" dim="0.05 0.03 0.02" color="orange"/>
+              <geom type="box" mass="0.1" dim="0.05 0.03 0.02" color="dustin_exp_orange"/>
             </body>
             <body name="seg4" joint="ry" pos="0.2 0 0" pos_min="0.15 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3">
               <omc name="seg4" pos_marker="2" pos="0 0 -.02"/>
-              <geom type="box" mass="1" pos="0.1 0 0" dim="0.2 0.05 0.05"/>
+              <geom type="box" mass="1" pos="0.1 0 0" dim="0.2 0.05 0.05" color="dustin_exp_white"/>
+              <geom type="box" mass="0.1" pos="0.1 0.05 0" dim="0.01 0.1 0.01" color="black"/>
+              <geom type="box" mass="0.1" pos="0.15 -0.05 0" dim="0.01 0.1 0.01" color="black"/>
               <body name="imu4" joint="frozen" pos="0.1 0.0 0.035" pos_min="0.05 -0.05 -0.05" pos_max="0.15 0.05 0.05">
                 <omc name="seg4" pos_marker="2" pos=".1 0 .015"/>
-                <geom type="box" mass="0.1" dim="0.05 0.03 0.02" color="blue"/>
+                <geom type="box" mass="0.1" dim="0.05 0.03 0.02" color="dustin_exp_orange"/>
               </body>
             </body>
           </body>
         </body>
       </body>
     </body>
   </worldbody>
```

### Comparing `imt_diodem-1.0.0/src/diodem/dataverse_github.py` & `imt_diodem-1.0.1/src/diodem/dataverse_github.py`

 * *Files identical despite different names*

### Comparing `imt_diodem-1.0.0/src/diodem/test_dataverse_github.py` & `imt_diodem-1.0.1/src/diodem/test_dataverse_github.py`

 * *Files identical despite different names*

### Comparing `imt_diodem-1.0.0/src/diodem/test_src.py` & `imt_diodem-1.0.1/src/diodem/test_src.py`

 * *Files identical despite different names*

### Comparing `imt_diodem-1.0.0/src/diodem/test_utils.py` & `imt_diodem-1.0.1/src/diodem/test_utils.py`

 * *Files identical despite different names*

### Comparing `imt_diodem-1.0.0/src/imt_diodem.egg-info/PKG-INFO` & `imt_diodem-1.0.1/src/imt_diodem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imt-diodem
-Version: 1.0.0
+Version: 1.0.1
 Summary: DIODEM -- A Diverse Inertial and Optical Dataset of kinEmatic chain Motion
 Author-email: Simon Bachhuber <simon.bachhuber@fau.de>
 Project-URL: Homepage, https://github.com/SimiPixel/diodem
 Project-URL: Issues, https://github.com/SimiPixel/diodem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `imt_diodem-1.0.0/src/imt_diodem.egg-info/SOURCES.txt` & `imt_diodem-1.0.1/src/imt_diodem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

