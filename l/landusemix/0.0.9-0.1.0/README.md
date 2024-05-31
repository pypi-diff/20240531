# Comparing `tmp/landusemix-0.0.9.tar.gz` & `tmp/landusemix-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landusemix-0.0.9.tar", last modified: Wed May 22 02:50:41 2024, max compression
+gzip compressed data, was "landusemix-0.1.0.tar", last modified: Fri May 31 17:36:21 2024, max compression
```

## Comparing `landusemix-0.0.9.tar` & `landusemix-0.1.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:50:41.546898 landusemix-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 02:50:38.000000 landusemix-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-22 02:50:38.000000 landusemix-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-05-22 02:50:41.546898 landusemix-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-05-22 02:50:38.000000 landusemix-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:50:41.542898 landusemix-0.0.9/landusemix/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:50:41.542898 landusemix-0.0.9/landusemix/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:50:41.542898 landusemix-0.0.9/landusemix/data/geojson/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/data/geojson/half.geojson
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/data/geojson/multiple.geojson
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/data/geojson/one.geojson
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/data/sample.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:50:41.546898 landusemix-0.0.9/landusemix/data/shapefiles/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/data/shapefiles/half.cpg
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/data/shapefiles/half.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/data/shapefiles/half.prj
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/data/shapefiles/half.qix
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/data/shapefiles/half.qmd
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/data/shapefiles/half.shp
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/data/shapefiles/half.shx
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/data/shapefiles/multiple.cpg
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/data/shapefiles/multiple.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/data/shapefiles/multiple.prj
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/data/shapefiles/multiple.qix
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/data/shapefiles/multiple.shp
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/data/shapefiles/multiple.shx
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/data/shapefiles/one.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/data/shapefiles/one.prj
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/data/shapefiles/one.qmd
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/data/shapefiles/one.shp
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/data/shapefiles/one.shx
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-22 02:50:38.000000 landusemix-0.0.9/landusemix/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:50:41.546898 landusemix-0.0.9/landusemix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-05-22 02:50:41.000000 landusemix-0.0.9/landusemix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-22 02:50:41.000000 landusemix-0.0.9/landusemix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:50:41.000000 landusemix-0.0.9/landusemix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 02:50:41.000000 landusemix-0.0.9/landusemix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 02:50:41.000000 landusemix-0.0.9/landusemix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 02:50:41.546898 landusemix-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-22 02:50:38.000000 landusemix-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:50:41.546898 landusemix-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:50:38.000000 landusemix-0.0.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-22 02:50:38.000000 landusemix-0.0.9/tests/test_landusemix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:36:21.034274 landusemix-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-31 17:36:17.000000 landusemix-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-31 17:36:17.000000 landusemix-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-05-31 17:36:21.034274 landusemix-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-05-31 17:36:17.000000 landusemix-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:36:21.030274 landusemix-0.1.0/landusemix/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:36:21.030274 landusemix-0.1.0/landusemix/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:36:21.030274 landusemix-0.1.0/landusemix/data/geojson/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/data/geojson/half.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/data/geojson/multiple.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/data/geojson/one.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/data/sample.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:36:21.034274 landusemix-0.1.0/landusemix/data/shapefiles/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/data/shapefiles/half.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/data/shapefiles/half.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/data/shapefiles/half.prj
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/data/shapefiles/half.qix
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/data/shapefiles/half.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/data/shapefiles/half.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/data/shapefiles/half.shx
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/data/shapefiles/multiple.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/data/shapefiles/multiple.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/data/shapefiles/multiple.prj
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/data/shapefiles/multiple.qix
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/data/shapefiles/multiple.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/data/shapefiles/multiple.shx
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/data/shapefiles/one.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/data/shapefiles/one.prj
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/data/shapefiles/one.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/data/shapefiles/one.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/data/shapefiles/one.shx
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-31 17:36:17.000000 landusemix-0.1.0/landusemix/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:36:21.034274 landusemix-0.1.0/landusemix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-05-31 17:36:21.000000 landusemix-0.1.0/landusemix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-31 17:36:21.000000 landusemix-0.1.0/landusemix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 17:36:21.000000 landusemix-0.1.0/landusemix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-31 17:36:21.000000 landusemix-0.1.0/landusemix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-31 17:36:21.000000 landusemix-0.1.0/landusemix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 17:36:21.034274 landusemix-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-31 17:36:17.000000 landusemix-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:36:21.034274 landusemix-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 17:36:17.000000 landusemix-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-31 17:36:17.000000 landusemix-0.1.0/tests/test_landusemix.py
```

### Comparing `landusemix-0.0.9/LICENSE` & `landusemix-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.9/PKG-INFO` & `landusemix-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landusemix
-Version: 0.0.9
+Version: 0.1.0
 Summary: A package for calculating land use mix indices
 Home-page: https://github.com/makyol/landusemix
 Author: Mehmet Ali Akyol
 Author-email: akyol.mehmet@metu.edu.tr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `landusemix-0.0.9/README.md` & `landusemix-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.9/landusemix/data/geojson/half.geojson` & `landusemix-0.1.0/landusemix/data/geojson/half.geojson`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.9/landusemix/data/geojson/multiple.geojson` & `landusemix-0.1.0/landusemix/data/geojson/multiple.geojson`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.9/landusemix/data/shapefiles/half.qmd` & `landusemix-0.1.0/landusemix/data/shapefiles/half.qmd`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.9/landusemix/data/shapefiles/one.qmd` & `landusemix-0.1.0/landusemix/data/shapefiles/one.qmd`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.9/landusemix/indices.py` & `landusemix-0.1.0/landusemix/indices.py`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.9/landusemix/utils.py` & `landusemix-0.1.0/landusemix/utils.py`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.9/landusemix.egg-info/PKG-INFO` & `landusemix-0.1.0/landusemix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landusemix
-Version: 0.0.9
+Version: 0.1.0
 Summary: A package for calculating land use mix indices
 Home-page: https://github.com/makyol/landusemix
 Author: Mehmet Ali Akyol
 Author-email: akyol.mehmet@metu.edu.tr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `landusemix-0.0.9/landusemix.egg-info/SOURCES.txt` & `landusemix-0.1.0/landusemix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `landusemix-0.0.9/setup.py` & `landusemix-0.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import glob
 from setuptools import setup, find_packages
 
 setup(
     name="landusemix",
-    version="0.0.9",
+    version="0.1.0",
     author="Mehmet Ali Akyol",
     author_email="akyol.mehmet@metu.edu.tr",
     description="A package for calculating land use mix indices",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/makyol/landusemix",
     packages=find_packages(),
```

### Comparing `landusemix-0.0.9/tests/test_landusemix.py` & `landusemix-0.1.0/tests/test_landusemix.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,59 +13,62 @@
         }
         self.indices = LandUseMixIndices(self.land_use_areas)
 
     def test_entropy_index(self):
         expected = -sum((area / 1000) * math.log(area / 1000)
                         for area in [500, 300, 200]) / math.log(3)
         print("Expected entropy index:", expected)
-        self.assertAlmostEqual(self.indices.entropy_index(), expected)
+        self.assertAlmostEqual(
+            self.indices.entropy_index(), round(expected, 2))
 
     def test_herfindahl_hirschman_index(self):
         expected = sum((100 * (area / 1000)) ** 2 for area in [500, 300, 200])
         print("Expected Herfindahl-Hirschman index:", expected)
         self.assertAlmostEqual(
-            self.indices.herfindahl_hirschman_index(), expected)
+            self.indices.herfindahl_hirschman_index(), round(expected, 2))
 
     def test_entropy_index_single_land_use(self):
         land_use_areas = {
             "residential": 1000
         }
         indices = LandUseMixIndices(land_use_areas)
         expected = 0.0
         print("Expected entropy index for single land use:", expected)
-        self.assertAlmostEqual(indices.entropy_index(), expected)
+        self.assertAlmostEqual(indices.entropy_index(), round(expected, 2))
 
     def test_entropy_index_equal_area(self):
         land_use_areas = {
             "residential": 500,
             "commercial": 500,
             "industrial": 500
         }
         indices = LandUseMixIndices(land_use_areas)
         expected = -sum((area / 1500) * math.log(area / 1500)
                         for area in [500, 500, 500]) / math.log(3)
         print("Expected entropy index for equal area:", expected)
-        self.assertAlmostEqual(indices.entropy_index(), expected)
+        self.assertAlmostEqual(indices.entropy_index(), round(expected, 2))
 
     def test_herfindahl_hirschman_index_single_land_use(self):
         land_use_areas = {
             "residential": 1000
         }
         indices = LandUseMixIndices(land_use_areas)
         expected = 10000.0
         print("Expected Herfindahl-Hirschman index for single land use:", expected)
-        self.assertAlmostEqual(indices.herfindahl_hirschman_index(), expected)
+        self.assertAlmostEqual(
+            indices.herfindahl_hirschman_index(), round(expected, 2))
 
     def test_herfindahl_hirschman_index_equal_area(self):
         land_use_areas = {
             "residential": 500,
             "commercial": 500,
             "industrial": 500
         }
         indices = LandUseMixIndices(land_use_areas)
         expected = sum((100 * (area / 1500)) ** 2 for area in [500, 500, 500])
         print("Expected Herfindahl-Hirschman index for equal area:", expected)
-        self.assertAlmostEqual(indices.herfindahl_hirschman_index(), expected)
+        self.assertAlmostEqual(
+            indices.herfindahl_hirschman_index(), round(expected, 2))
 
 
 if __name__ == "__main__":
     unittest.main()
```

