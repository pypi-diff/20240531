# Comparing `tmp/interpolator_for_wrfchem-1.2.0.tar.gz` & `tmp/interpolator_for_wrfchem-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interpolator_for_wrfchem-1.2.0.tar", max compression
+gzip compressed data, was "interpolator_for_wrfchem-1.2.1.tar", max compression
```

## Comparing `interpolator_for_wrfchem-1.2.0.tar` & `interpolator_for_wrfchem-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,17 @@
--rw-r--r--   0        0        0     1074 2024-02-06 14:04:33.000000 interpolator_for_wrfchem-1.2.0/LICENSE
--rw-r--r--   0        0        0     3497 2024-05-14 14:44:48.563466 interpolator_for_wrfchem-1.2.0/README.md
--rw-r--r--   0        0        0     7801 2024-05-14 14:02:26.283465 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/__init__.py
--rw-r--r--   0        0        0       50 2023-12-13 14:36:46.000000 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/__main__.py
--rw-r--r--   0        0        0      130 2024-05-14 13:59:05.663473 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/global_models/__init__.py
--rw-r--r--   0        0        0      386 2024-05-14 14:02:29.673465 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/global_models/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     9806 2024-05-14 14:08:58.743470 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/global_models/__pycache__/cams.cpython-312.pyc
--rw-r--r--   0        0        0     1214 2024-05-14 14:02:29.693465 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/global_models/__pycache__/prototype.cpython-312.pyc
--rw-r--r--   0        0        0     7073 2024-05-14 14:08:55.993470 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/global_models/cams.py
--rw-r--r--   0        0        0      546 2024-05-14 13:35:26.773462 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/global_models/prototype.py
--rw-r--r--   0        0        0     2888 2024-05-14 14:45:10.223466 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/interpolation.py
--rw-r--r--   0        0        0     2628 2024-03-20 11:07:17.890811 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/met_em.py
--rw-r--r--   0        0        0        0 2023-12-19 09:13:27.000000 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/res/__init__.py
--rw-r--r--   0        0        0      184 2023-12-19 10:58:50.000000 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/res/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0    10577 2024-05-14 13:43:25.533463 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/res/cams_l137.csv
--rw-r--r--   0        0        0     4603 2023-12-19 09:06:49.000000 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/res/cams_l60.csv
--rw-r--r--   0        0        0     4124 2024-05-14 13:19:32.453465 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/species_map.py
--rw-r--r--   0        0        0     1212 2024-01-09 08:25:51.000000 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/utils.py
--rw-r--r--   0        0        0     2806 2024-05-14 12:56:08.583462 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/wrf.py
--rw-r--r--   0        0        0      658 2024-05-14 14:45:19.553467 interpolator_for_wrfchem-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     4140 1970-01-01 00:00:00.000000 interpolator_for_wrfchem-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-31 17:26:11.161254 interpolator_for_wrfchem-1.2.1/LICENSE
+-rw-r--r--   0        0        0     3497 2024-05-31 17:26:11.161254 interpolator_for_wrfchem-1.2.1/README.md
+-rw-r--r--   0        0        0     7801 2024-05-31 17:26:11.161254 interpolator_for_wrfchem-1.2.1/interpolator_for_wrfchem/__init__.py
+-rw-r--r--   0        0        0       50 2024-05-31 17:26:11.161254 interpolator_for_wrfchem-1.2.1/interpolator_for_wrfchem/__main__.py
+-rw-r--r--   0        0        0      130 2024-05-31 17:26:11.161254 interpolator_for_wrfchem-1.2.1/interpolator_for_wrfchem/global_models/__init__.py
+-rw-r--r--   0        0        0     7073 2024-05-31 17:26:11.161254 interpolator_for_wrfchem-1.2.1/interpolator_for_wrfchem/global_models/cams.py
+-rw-r--r--   0        0        0      546 2024-05-31 17:26:11.161254 interpolator_for_wrfchem-1.2.1/interpolator_for_wrfchem/global_models/prototype.py
+-rw-r--r--   0        0        0     2888 2024-05-31 17:26:11.161254 interpolator_for_wrfchem-1.2.1/interpolator_for_wrfchem/interpolation.py
+-rw-r--r--   0        0        0     2628 2024-05-31 17:26:11.165254 interpolator_for_wrfchem-1.2.1/interpolator_for_wrfchem/met_em.py
+-rw-r--r--   0        0        0        0 2024-05-31 17:26:11.165254 interpolator_for_wrfchem-1.2.1/interpolator_for_wrfchem/res/__init__.py
+-rw-r--r--   0        0        0    10577 2024-05-31 17:26:11.165254 interpolator_for_wrfchem-1.2.1/interpolator_for_wrfchem/res/cams_l137.csv
+-rw-r--r--   0        0        0     4603 2024-05-31 17:26:11.165254 interpolator_for_wrfchem-1.2.1/interpolator_for_wrfchem/res/cams_l60.csv
+-rw-r--r--   0        0        0     4124 2024-05-31 17:26:11.165254 interpolator_for_wrfchem-1.2.1/interpolator_for_wrfchem/species_map.py
+-rw-r--r--   0        0        0     1212 2024-05-31 17:26:11.165254 interpolator_for_wrfchem-1.2.1/interpolator_for_wrfchem/utils.py
+-rw-r--r--   0        0        0     2806 2024-05-31 17:26:11.165254 interpolator_for_wrfchem-1.2.1/interpolator_for_wrfchem/wrf.py
+-rw-r--r--   0        0        0      658 2024-05-31 17:26:11.165254 interpolator_for_wrfchem-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4191 1970-01-01 00:00:00.000000 interpolator_for_wrfchem-1.2.1/PKG-INFO
```

### Comparing `interpolator_for_wrfchem-1.2.0/LICENSE` & `interpolator_for_wrfchem-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `interpolator_for_wrfchem-1.2.0/README.md` & `interpolator_for_wrfchem-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/__init__.py` & `interpolator_for_wrfchem-1.2.1/interpolator_for_wrfchem/__init__.py`

 * *Files identical despite different names*

### Comparing `interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/global_models/cams.py` & `interpolator_for_wrfchem-1.2.1/interpolator_for_wrfchem/global_models/cams.py`

 * *Files identical despite different names*

### Comparing `interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/global_models/prototype.py` & `interpolator_for_wrfchem-1.2.1/interpolator_for_wrfchem/global_models/prototype.py`

 * *Files identical despite different names*

### Comparing `interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/interpolation.py` & `interpolator_for_wrfchem-1.2.1/interpolator_for_wrfchem/interpolation.py`

 * *Files identical despite different names*

### Comparing `interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/met_em.py` & `interpolator_for_wrfchem-1.2.1/interpolator_for_wrfchem/met_em.py`

 * *Files identical despite different names*

### Comparing `interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/res/cams_l137.csv` & `interpolator_for_wrfchem-1.2.1/interpolator_for_wrfchem/res/cams_l137.csv`

 * *Files identical despite different names*

### Comparing `interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/res/cams_l60.csv` & `interpolator_for_wrfchem-1.2.1/interpolator_for_wrfchem/res/cams_l60.csv`

 * *Files identical despite different names*

### Comparing `interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/species_map.py` & `interpolator_for_wrfchem-1.2.1/interpolator_for_wrfchem/species_map.py`

 * *Files identical despite different names*

### Comparing `interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/utils.py` & `interpolator_for_wrfchem-1.2.1/interpolator_for_wrfchem/utils.py`

 * *Files identical despite different names*

### Comparing `interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/wrf.py` & `interpolator_for_wrfchem-1.2.1/interpolator_for_wrfchem/wrf.py`

 * *Files identical despite different names*

### Comparing `interpolator_for_wrfchem-1.2.0/PKG-INFO` & `interpolator_for_wrfchem-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: interpolator-for-wrfchem
-Version: 1.2.0
+Version: 1.2.1
 Summary: Interpolates global chemistry fields for use with WRF-CHEM
 Author: Thanasis Georgiou
 Author-email: ageorgiou@noa.gr
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cftime (>=1.6.3,<2.0.0)
 Requires-Dist: netcdf4 (>=1.6.5,<2.0.0)
 Requires-Dist: numpy (>=1.26.2,<2.0.0)
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
 Requires-Dist: scipy (>=1.11.4,<2.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
```

