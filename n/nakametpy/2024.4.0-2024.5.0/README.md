# Comparing `tmp/nakametpy-2024.4.0.tar.gz` & `tmp/nakametpy-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nakametpy-2024.4.0.tar", last modified: Sat Apr 20 09:42:19 2024, max compression
+gzip compressed data, was "nakametpy-2024.5.0.tar", last modified: Fri May 31 14:33:11 2024, max compression
```

## Comparing `nakametpy-2024.4.0.tar` & `nakametpy-2024.5.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 09:42:19.516022 nakametpy-2024.4.0/
--rw-rw-rw-   0        0        0     1555 2024-03-20 13:25:39.000000 nakametpy-2024.4.0/LICENSE
--rw-rw-rw-   0        0        0       58 2024-03-20 13:25:39.000000 nakametpy-2024.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3043 2024-04-20 09:42:19.516022 nakametpy-2024.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     2526 2024-04-20 09:36:49.000000 nakametpy-2024.4.0/README.md
--rw-rw-rw-   0        0        0      668 2024-04-20 09:40:40.000000 nakametpy-2024.4.0/pyproject.toml
--rw-rw-rw-   0        0        0      113 2024-04-20 09:36:49.000000 nakametpy-2024.4.0/requirements.txt
--rw-rw-rw-   0        0        0       81 2024-04-20 09:42:19.518016 nakametpy-2024.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1106 2024-04-20 09:40:40.000000 nakametpy-2024.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 09:42:19.458177 nakametpy-2024.4.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-20 09:42:19.497073 nakametpy-2024.4.0/src/nakametpy/
--rw-rw-rw-   0        0        0      877 2024-03-20 13:25:40.000000 nakametpy-2024.4.0/src/nakametpy/__init__.py
--rw-rw-rw-   0        0        0     6872 2024-04-20 09:36:49.000000 nakametpy-2024.4.0/src/nakametpy/_error.py
--rw-rw-rw-   0        0        0      195 2024-04-20 09:40:40.000000 nakametpy-2024.4.0/src/nakametpy/_version.py
--rw-rw-rw-   0        0        0    68632 2024-03-20 13:25:40.000000 nakametpy-2024.4.0/src/nakametpy/cmaps.py
--rw-rw-rw-   0        0        0     2834 2024-03-20 13:25:40.000000 nakametpy-2024.4.0/src/nakametpy/constants.py
--rw-rw-rw-   0        0        0    12123 2024-03-20 13:25:40.000000 nakametpy-2024.4.0/src/nakametpy/grads.py
--rw-rw-rw-   0        0        0     1265 2024-03-20 13:25:40.000000 nakametpy-2024.4.0/src/nakametpy/jma.py
--rw-rw-rw-   0        0        0    67887 2024-03-20 13:25:40.000000 nakametpy-2024.4.0/src/nakametpy/kinematics.py
--rw-rw-rw-   0        0        0    26216 2024-03-20 13:25:40.000000 nakametpy-2024.4.0/src/nakametpy/thermo.py
--rw-rw-rw-   0        0        0     9905 2024-04-20 09:36:49.000000 nakametpy-2024.4.0/src/nakametpy/util.py
-drwxrwxrwx   0        0        0        0 2024-04-20 09:42:19.514029 nakametpy-2024.4.0/src/nakametpy.egg-info/
--rw-rw-rw-   0        0        0     3043 2024-04-20 09:42:19.000000 nakametpy-2024.4.0/src/nakametpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      548 2024-04-20 09:42:19.000000 nakametpy-2024.4.0/src/nakametpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 09:42:19.000000 nakametpy-2024.4.0/src/nakametpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2024-04-20 09:42:19.000000 nakametpy-2024.4.0/src/nakametpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-20 09:42:19.000000 nakametpy-2024.4.0/src/nakametpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-20 09:42:19.511037 nakametpy-2024.4.0/tests/
--rw-rw-rw-   0        0        0      316 2024-04-20 09:36:49.000000 nakametpy-2024.4.0/tests/test_thermo.py
--rw-rw-rw-   0        0        0    18498 2024-04-20 09:36:49.000000 nakametpy-2024.4.0/tests/test_util.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:33:11.541226 nakametpy-2024.5.0/
+-rw-rw-rw-   0        0        0     1555 2024-03-20 13:25:39.000000 nakametpy-2024.5.0/LICENSE
+-rw-rw-rw-   0        0        0       58 2024-03-20 13:25:39.000000 nakametpy-2024.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3140 2024-05-31 14:33:11.538033 nakametpy-2024.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2526 2024-04-20 09:36:49.000000 nakametpy-2024.5.0/README.md
+-rw-rw-rw-   0        0        0      882 2024-05-31 11:47:47.000000 nakametpy-2024.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0      215 2024-05-31 14:33:07.000000 nakametpy-2024.5.0/requirements.txt
+-rw-rw-rw-   0        0        0       81 2024-05-31 14:33:11.543213 nakametpy-2024.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1106 2024-05-31 11:47:47.000000 nakametpy-2024.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:33:11.477419 nakametpy-2024.5.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-31 14:33:11.519089 nakametpy-2024.5.0/src/nakametpy/
+-rw-rw-rw-   0        0        0      877 2024-03-20 13:25:40.000000 nakametpy-2024.5.0/src/nakametpy/__init__.py
+-rw-rw-rw-   0        0        0     6872 2024-04-20 09:36:49.000000 nakametpy-2024.5.0/src/nakametpy/_error.py
+-rw-rw-rw-   0        0        0      195 2024-05-31 11:47:47.000000 nakametpy-2024.5.0/src/nakametpy/_version.py
+-rw-rw-rw-   0        0        0    68632 2024-03-20 13:25:40.000000 nakametpy-2024.5.0/src/nakametpy/cmaps.py
+-rw-rw-rw-   0        0        0     2834 2024-03-20 13:25:40.000000 nakametpy-2024.5.0/src/nakametpy/constants.py
+-rw-rw-rw-   0        0        0    12123 2024-03-20 13:25:40.000000 nakametpy-2024.5.0/src/nakametpy/grads.py
+-rw-rw-rw-   0        0        0     1265 2024-03-20 13:25:40.000000 nakametpy-2024.5.0/src/nakametpy/jma.py
+-rw-rw-rw-   0        0        0    67887 2024-03-20 13:25:40.000000 nakametpy-2024.5.0/src/nakametpy/kinematics.py
+-rw-rw-rw-   0        0        0    26216 2024-03-20 13:25:40.000000 nakametpy-2024.5.0/src/nakametpy/thermo.py
+-rw-rw-rw-   0        0        0    10475 2024-05-31 11:45:39.000000 nakametpy-2024.5.0/src/nakametpy/util.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:33:11.537035 nakametpy-2024.5.0/src/nakametpy.egg-info/
+-rw-rw-rw-   0        0        0     3140 2024-05-31 14:33:11.000000 nakametpy-2024.5.0/src/nakametpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      548 2024-05-31 14:33:11.000000 nakametpy-2024.5.0/src/nakametpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 14:33:11.000000 nakametpy-2024.5.0/src/nakametpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      202 2024-05-31 14:33:11.000000 nakametpy-2024.5.0/src/nakametpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-31 14:33:11.000000 nakametpy-2024.5.0/src/nakametpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 14:33:11.535040 nakametpy-2024.5.0/tests/
+-rw-rw-rw-   0        0        0      316 2024-04-20 09:36:49.000000 nakametpy-2024.5.0/tests/test_thermo.py
+-rw-rw-rw-   0        0        0    18498 2024-04-20 09:36:49.000000 nakametpy-2024.5.0/tests/test_util.py
```

### Comparing `nakametpy-2024.4.0/LICENSE` & `nakametpy-2024.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.4.0/PKG-INFO` & `nakametpy-2024.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: nakametpy
-Version: 2024.4.0
+Version: 2024.5.0
 Summary: Meteorological modules for calculation and colormap.
 Home-page: https://github.com/muchojp/NakaMetPy
 Author: muchojp
 Author-email: contact.muchiwo@gmail.com
 License: BSD 3-clause
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy<=1.21.1; python_version < "3.11"
-Requires-Dist: numpy>=1.21.2; python_version >= "3.11"
+Requires-Dist: numpy<=1.21.1; python_version == "3.6"
+Requires-Dist: numpy<1.22.0,>=1.21.3; python_version == "3.7"
+Requires-Dist: numpy<1.25.0,>=1.21.3; python_version == "3.8"
+Requires-Dist: numpy>=1.26.4; python_version >= "3.9"
 Requires-Dist: matplotlib>=3.3.0
-Requires-Dist: nose>=1.3.0
 
 # NakaMetPy
 
 [![PyPI version][pypi-image]][pypi-link]
 [![Anaconda version][anaconda-v-image]][anaconda-v-link]
 [![pytest][github-actions-image]][github-actions-link]
```

### Comparing `nakametpy-2024.4.0/README.md` & `nakametpy-2024.5.0/README.md`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.4.0/setup.py` & `nakametpy-2024.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     # 'sample_lib_cli=sample_lib_cli.call:main',
 ]
 
 
 setup(
     name='nakametpy',
     python_requires='>=3.7.0',
-    version='2024.4.0',
+    version='2024.5.0',
     description='Meteorological modules for calculation and colormap.',
     # packages=packages,
     packages=find_packages('src'),
     # install_requires=install_requires,
     package_dir={"": "src"}, 
     install_requires=_requires_from_file('requirements.txt'),
     url = 'https://github.com/muchojp/NakaMetPy',
```

### Comparing `nakametpy-2024.4.0/src/nakametpy/__init__.py` & `nakametpy-2024.5.0/src/nakametpy/__init__.py`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.4.0/src/nakametpy/_error.py` & `nakametpy-2024.5.0/src/nakametpy/_error.py`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.4.0/src/nakametpy/cmaps.py` & `nakametpy-2024.5.0/src/nakametpy/cmaps.py`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.4.0/src/nakametpy/constants.py` & `nakametpy-2024.5.0/src/nakametpy/constants.py`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.4.0/src/nakametpy/grads.py` & `nakametpy-2024.5.0/src/nakametpy/grads.py`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.4.0/src/nakametpy/jma.py` & `nakametpy-2024.5.0/src/nakametpy/jma.py`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.4.0/src/nakametpy/kinematics.py` & `nakametpy-2024.5.0/src/nakametpy/kinematics.py`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.4.0/src/nakametpy/thermo.py` & `nakametpy-2024.5.0/src/nakametpy/thermo.py`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.4.0/src/nakametpy/util.py` & `nakametpy-2024.5.0/src/nakametpy/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,23 +64,24 @@
   else:
     raise NotSupportedExtentionError(_ext1, "bin, tar, gz, gzip")
   return binary
 
 def load_jmara_grib2(file, tar_flag=False, tar_contentname=None):
   r'''気象庁解析雨量やレーダー雨量を返す関数
 
-  欠損値は負の値として表現される
+  欠損値は負の値として表現される。
+  ファイルはgrib2, tar, gz(gzip)を受け付ける
 
   Parameters
   --------
   file: `str`
     file path 
     ファイルのPATH
   tar_flag: `bool`
-    file type whether file is tar or GRIB2 (not tar).
+    file type are GRIB2, tar and gz(gzip).
   tar_contentname: `str`
     content name in tar file.
 
   Returns
   -------
   rain: `numpy.ma.MaskedArray`
     Units(単位) [mm/h]
@@ -158,14 +159,35 @@
   Returns
   -------
   lon: `numpy.ndarray`
   '''
   return np.linspace(118, 150, 1024, endpoint=False) + 1/80 / 2
 
 def get_grib2_latlon(file, tar_flag=False, tar_contentname=None):
+  r'''気象庁解析雨量やレーダー雨量の緯度経度を返す関数
+
+  欠損値は負の値として表現される。
+  ファイルはgrib2, tar, gz(gzip)を受け付ける
+
+  Parameters
+  --------
+  file: `str`
+    file path 
+    ファイルのPATH
+  tar_flag: `bool`
+    file type are GRIB2, tar and gz(gzip).
+  tar_contentname: `str`
+    content name in tar file.
+
+  Returns
+  -------
+  latlon: set(`numpy.ma.MaskedArray`, `numpy.ma.MaskedArray`)
+    (Latitude, Longitude)
+  '''
+  
   binary = _get_binary(file=file, tar_flag=tar_flag, tar_contentname=tar_contentname)
   
   # The Sector 0, 1, 3, 4, 6 are fixed.
   len_ = {'sec0':16, 'sec1':21, 'sec3':72, 'sec4':82, 'sec6':6}
   end1 = len_['sec0'] + len_['sec1'] - 1
   # +31 is octet of grid numbers align latitude line.
   nlon = struct.unpack_from('>I', binary, end1+31)[0]
```

### Comparing `nakametpy-2024.4.0/src/nakametpy.egg-info/PKG-INFO` & `nakametpy-2024.5.0/src/nakametpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: nakametpy
-Version: 2024.4.0
+Version: 2024.5.0
 Summary: Meteorological modules for calculation and colormap.
 Home-page: https://github.com/muchojp/NakaMetPy
 Author: muchojp
 Author-email: contact.muchiwo@gmail.com
 License: BSD 3-clause
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy<=1.21.1; python_version < "3.11"
-Requires-Dist: numpy>=1.21.2; python_version >= "3.11"
+Requires-Dist: numpy<=1.21.1; python_version == "3.6"
+Requires-Dist: numpy<1.22.0,>=1.21.3; python_version == "3.7"
+Requires-Dist: numpy<1.25.0,>=1.21.3; python_version == "3.8"
+Requires-Dist: numpy>=1.26.4; python_version >= "3.9"
 Requires-Dist: matplotlib>=3.3.0
-Requires-Dist: nose>=1.3.0
 
 # NakaMetPy
 
 [![PyPI version][pypi-image]][pypi-link]
 [![Anaconda version][anaconda-v-image]][anaconda-v-link]
 [![pytest][github-actions-image]][github-actions-link]
```

### Comparing `nakametpy-2024.4.0/src/nakametpy.egg-info/SOURCES.txt` & `nakametpy-2024.5.0/src/nakametpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.4.0/tests/test_util.py` & `nakametpy-2024.5.0/tests/test_util.py`

 * *Files identical despite different names*

