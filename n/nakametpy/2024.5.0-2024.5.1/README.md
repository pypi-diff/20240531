# Comparing `tmp/nakametpy-2024.5.0.tar.gz` & `tmp/nakametpy-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nakametpy-2024.5.0.tar", last modified: Fri May 31 14:33:11 2024, max compression
+gzip compressed data, was "nakametpy-2024.5.1.tar", last modified: Fri May 31 14:48:53 2024, max compression
```

## Comparing `nakametpy-2024.5.0.tar` & `nakametpy-2024.5.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 14:33:11.541226 nakametpy-2024.5.0/
--rw-rw-rw-   0        0        0     1555 2024-03-20 13:25:39.000000 nakametpy-2024.5.0/LICENSE
--rw-rw-rw-   0        0        0       58 2024-03-20 13:25:39.000000 nakametpy-2024.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3140 2024-05-31 14:33:11.538033 nakametpy-2024.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     2526 2024-04-20 09:36:49.000000 nakametpy-2024.5.0/README.md
--rw-rw-rw-   0        0        0      882 2024-05-31 11:47:47.000000 nakametpy-2024.5.0/pyproject.toml
--rw-rw-rw-   0        0        0      215 2024-05-31 14:33:07.000000 nakametpy-2024.5.0/requirements.txt
--rw-rw-rw-   0        0        0       81 2024-05-31 14:33:11.543213 nakametpy-2024.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1106 2024-05-31 11:47:47.000000 nakametpy-2024.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-31 14:33:11.477419 nakametpy-2024.5.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-31 14:33:11.519089 nakametpy-2024.5.0/src/nakametpy/
--rw-rw-rw-   0        0        0      877 2024-03-20 13:25:40.000000 nakametpy-2024.5.0/src/nakametpy/__init__.py
--rw-rw-rw-   0        0        0     6872 2024-04-20 09:36:49.000000 nakametpy-2024.5.0/src/nakametpy/_error.py
--rw-rw-rw-   0        0        0      195 2024-05-31 11:47:47.000000 nakametpy-2024.5.0/src/nakametpy/_version.py
--rw-rw-rw-   0        0        0    68632 2024-03-20 13:25:40.000000 nakametpy-2024.5.0/src/nakametpy/cmaps.py
--rw-rw-rw-   0        0        0     2834 2024-03-20 13:25:40.000000 nakametpy-2024.5.0/src/nakametpy/constants.py
--rw-rw-rw-   0        0        0    12123 2024-03-20 13:25:40.000000 nakametpy-2024.5.0/src/nakametpy/grads.py
--rw-rw-rw-   0        0        0     1265 2024-03-20 13:25:40.000000 nakametpy-2024.5.0/src/nakametpy/jma.py
--rw-rw-rw-   0        0        0    67887 2024-03-20 13:25:40.000000 nakametpy-2024.5.0/src/nakametpy/kinematics.py
--rw-rw-rw-   0        0        0    26216 2024-03-20 13:25:40.000000 nakametpy-2024.5.0/src/nakametpy/thermo.py
--rw-rw-rw-   0        0        0    10475 2024-05-31 11:45:39.000000 nakametpy-2024.5.0/src/nakametpy/util.py
-drwxrwxrwx   0        0        0        0 2024-05-31 14:33:11.537035 nakametpy-2024.5.0/src/nakametpy.egg-info/
--rw-rw-rw-   0        0        0     3140 2024-05-31 14:33:11.000000 nakametpy-2024.5.0/src/nakametpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      548 2024-05-31 14:33:11.000000 nakametpy-2024.5.0/src/nakametpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 14:33:11.000000 nakametpy-2024.5.0/src/nakametpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      202 2024-05-31 14:33:11.000000 nakametpy-2024.5.0/src/nakametpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-31 14:33:11.000000 nakametpy-2024.5.0/src/nakametpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-31 14:33:11.535040 nakametpy-2024.5.0/tests/
--rw-rw-rw-   0        0        0      316 2024-04-20 09:36:49.000000 nakametpy-2024.5.0/tests/test_thermo.py
--rw-rw-rw-   0        0        0    18498 2024-04-20 09:36:49.000000 nakametpy-2024.5.0/tests/test_util.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:48:53.070978 nakametpy-2024.5.1/
+-rw-rw-rw-   0        0        0     1555 2024-03-20 13:25:39.000000 nakametpy-2024.5.1/LICENSE
+-rw-rw-rw-   0        0        0       58 2024-03-20 13:25:39.000000 nakametpy-2024.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3140 2024-05-31 14:48:53.069983 nakametpy-2024.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2526 2024-04-20 09:36:49.000000 nakametpy-2024.5.1/README.md
+-rw-rw-rw-   0        0        0      882 2024-05-31 14:48:18.000000 nakametpy-2024.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0      215 2024-05-31 14:33:07.000000 nakametpy-2024.5.1/requirements.txt
+-rw-rw-rw-   0        0        0       81 2024-05-31 14:48:53.072973 nakametpy-2024.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1106 2024-05-31 14:48:18.000000 nakametpy-2024.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:48:53.006940 nakametpy-2024.5.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-31 14:48:53.050037 nakametpy-2024.5.1/src/nakametpy/
+-rw-rw-rw-   0        0        0      877 2024-03-20 13:25:40.000000 nakametpy-2024.5.1/src/nakametpy/__init__.py
+-rw-rw-rw-   0        0        0     6872 2024-04-20 09:36:49.000000 nakametpy-2024.5.1/src/nakametpy/_error.py
+-rw-rw-rw-   0        0        0      195 2024-05-31 14:48:18.000000 nakametpy-2024.5.1/src/nakametpy/_version.py
+-rw-rw-rw-   0        0        0    68632 2024-03-20 13:25:40.000000 nakametpy-2024.5.1/src/nakametpy/cmaps.py
+-rw-rw-rw-   0        0        0     2834 2024-03-20 13:25:40.000000 nakametpy-2024.5.1/src/nakametpy/constants.py
+-rw-rw-rw-   0        0        0    12123 2024-03-20 13:25:40.000000 nakametpy-2024.5.1/src/nakametpy/grads.py
+-rw-rw-rw-   0        0        0     1265 2024-03-20 13:25:40.000000 nakametpy-2024.5.1/src/nakametpy/jma.py
+-rw-rw-rw-   0        0        0    67887 2024-03-20 13:25:40.000000 nakametpy-2024.5.1/src/nakametpy/kinematics.py
+-rw-rw-rw-   0        0        0    26216 2024-03-20 13:25:40.000000 nakametpy-2024.5.1/src/nakametpy/thermo.py
+-rw-rw-rw-   0        0        0    10475 2024-05-31 11:45:39.000000 nakametpy-2024.5.1/src/nakametpy/util.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:48:53.068985 nakametpy-2024.5.1/src/nakametpy.egg-info/
+-rw-rw-rw-   0        0        0     3140 2024-05-31 14:48:52.000000 nakametpy-2024.5.1/src/nakametpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      548 2024-05-31 14:48:52.000000 nakametpy-2024.5.1/src/nakametpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 14:48:52.000000 nakametpy-2024.5.1/src/nakametpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      202 2024-05-31 14:48:52.000000 nakametpy-2024.5.1/src/nakametpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-31 14:48:52.000000 nakametpy-2024.5.1/src/nakametpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 14:48:53.065995 nakametpy-2024.5.1/tests/
+-rw-rw-rw-   0        0        0      316 2024-04-20 09:36:49.000000 nakametpy-2024.5.1/tests/test_thermo.py
+-rw-rw-rw-   0        0        0    18560 2024-05-31 14:47:29.000000 nakametpy-2024.5.1/tests/test_util.py
```

### Comparing `nakametpy-2024.5.0/LICENSE` & `nakametpy-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.5.0/PKG-INFO` & `nakametpy-2024.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nakametpy
-Version: 2024.5.0
+Version: 2024.5.1
 Summary: Meteorological modules for calculation and colormap.
 Home-page: https://github.com/muchojp/NakaMetPy
 Author: muchojp
 Author-email: contact.muchiwo@gmail.com
 License: BSD 3-clause
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `nakametpy-2024.5.0/README.md` & `nakametpy-2024.5.1/README.md`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.5.0/pyproject.toml` & `nakametpy-2024.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "NakaMetPy"
-version = "2024.5.0"
+version = "2024.5.1"
 description = "Meteorological Tools for Calculation and Colormap."
 authors = ["muchojp <contact.muchiwo@mail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/muchojp/NakaMetPy"
 repository = "https://github.com/muchojp/NakaMetPy"
 documentation = "https://muchojp.github.io/NakaMetPy/"
```

### Comparing `nakametpy-2024.5.0/setup.py` & `nakametpy-2024.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     # 'sample_lib_cli=sample_lib_cli.call:main',
 ]
 
 
 setup(
     name='nakametpy',
     python_requires='>=3.7.0',
-    version='2024.5.0',
+    version='2024.5.1',
     description='Meteorological modules for calculation and colormap.',
     # packages=packages,
     packages=find_packages('src'),
     # install_requires=install_requires,
     package_dir={"": "src"}, 
     install_requires=_requires_from_file('requirements.txt'),
     url = 'https://github.com/muchojp/NakaMetPy',
```

### Comparing `nakametpy-2024.5.0/src/nakametpy/__init__.py` & `nakametpy-2024.5.1/src/nakametpy/__init__.py`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.5.0/src/nakametpy/_error.py` & `nakametpy-2024.5.1/src/nakametpy/_error.py`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.5.0/src/nakametpy/cmaps.py` & `nakametpy-2024.5.1/src/nakametpy/cmaps.py`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.5.0/src/nakametpy/constants.py` & `nakametpy-2024.5.1/src/nakametpy/constants.py`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.5.0/src/nakametpy/grads.py` & `nakametpy-2024.5.1/src/nakametpy/grads.py`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.5.0/src/nakametpy/jma.py` & `nakametpy-2024.5.1/src/nakametpy/jma.py`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.5.0/src/nakametpy/kinematics.py` & `nakametpy-2024.5.1/src/nakametpy/kinematics.py`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.5.0/src/nakametpy/thermo.py` & `nakametpy-2024.5.1/src/nakametpy/thermo.py`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.5.0/src/nakametpy/util.py` & `nakametpy-2024.5.1/src/nakametpy/util.py`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.5.0/src/nakametpy.egg-info/PKG-INFO` & `nakametpy-2024.5.1/src/nakametpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nakametpy
-Version: 2024.5.0
+Version: 2024.5.1
 Summary: Meteorological modules for calculation and colormap.
 Home-page: https://github.com/muchojp/NakaMetPy
 Author: muchojp
 Author-email: contact.muchiwo@gmail.com
 License: BSD 3-clause
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `nakametpy-2024.5.0/src/nakametpy.egg-info/SOURCES.txt` & `nakametpy-2024.5.1/src/nakametpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.5.0/tests/test_util.py` & `nakametpy-2024.5.1/tests/test_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import unittest
 from src.nakametpy.util import dt_ymdhm, dt_yyyymmdd, unit_ms1_knots, unit_knots_ms1,\
                                anom_levels, concat_array, myglob, check_tar_content,\
                                load_jmara_grib2, get_jmara_lat, get_jmara_lon,\
                                get_grib2_latlon, get_gsmap_lat, get_gsmap_lon,\
                                jma_rain_lat, jma_rain_lon, gsmap_lat, gsmap_lon
 from src.nakametpy._error import NotHaveSetArgError, NotMatchTarContentNameError
+import os
 import numpy as np
 
 class UtilTest(unittest.TestCase):
   def test_dt_ymdhm_001(self):
     """
     test case: test_dt_ymdhm_001
     method:
@@ -313,52 +314,49 @@
     method:
       myglob
     args:
       path: `str`
     """
     # print(self.test_myglob_001.__doc__)
     
-    import glob
     path = "./tests/data/util/myglob/*"
     actual = myglob(path)
-    expected = list(("./tests/data/util/myglob/test1.txt", "./tests/data/util/myglob/test2.txt"))
+    expected = list((os.path.join("./tests/data/util/myglob", "test1.txt"), os.path.join("./tests/data/util/myglob", "test2.txt")))
     self.assertEqual(actual, expected)
 
   def test_myglob_002(self):
     """
     test case: test_myglob_002
     method:
       myglob
     args:
       path: `str`
       reverse=False: `bool`
     """
     # print(self.test_myglob_002.__doc__)
     
-    import glob
     path = "./tests/data/util/myglob/*"
     actual = myglob(path, reverse=False)
-    expected = list(("./tests/data/util/myglob/test1.txt", "./tests/data/util/myglob/test2.txt"))
+    expected = list((os.path.join("./tests/data/util/myglob", "test1.txt"), os.path.join("./tests/data/util/myglob", "test2.txt")))
     self.assertEqual(actual, expected)
 
   def test_myglob_003(self):
     """
     test case: test_myglob_003
     method:
       myglob
     args:
       path: `str`
       reverse=True: `bool`
     """
     # print(self.test_myglob_003.__doc__)
     
-    import glob
     path = "./tests/data/util/myglob/*"
     actual = myglob(path, reverse=True)
-    expected = list(("./tests/data/util/myglob/test2.txt", "./tests/data/util/myglob/test1.txt"))
+    expected = list((os.path.join("./tests/data/util/myglob", "test2.txt"), os.path.join("./tests/data/util/myglob", "test1.txt")))
     self.assertEqual(actual, expected)
   
   def test_check_tar_content_001(self):
     """
     test case: test_check_tar_content_001
     method:
       check_tar_content
```

