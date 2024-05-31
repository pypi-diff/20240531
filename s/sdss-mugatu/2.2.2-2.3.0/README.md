# Comparing `tmp/sdss-mugatu-2.2.2.tar.gz` & `tmp/sdss_mugatu-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss-mugatu-2.2.2.tar", max compression
+gzip compressed data, was "sdss_mugatu-2.3.0.tar", max compression
```

## Comparing `sdss-mugatu-2.2.2.tar` & `sdss_mugatu-2.3.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1504 2020-12-17 23:08:43.845089 sdss-mugatu-2.2.2/LICENSE.md
--rw-r--r--   0        0        0      468 2022-07-21 18:15:27.339825 sdss-mugatu-2.2.2/README.md
--rw-r--r--   0        0        0      815 2023-10-03 17:06:53.677496 sdss-mugatu-2.2.2/pyproject.toml
--rw-r--r--   0        0        0      544 2020-12-17 23:08:43.893921 sdss-mugatu-2.2.2/python/mugatu/__init__.py
--rw-r--r--   0        0        0    12505 2021-05-26 17:34:23.788221 sdss-mugatu-2.2.2/python/mugatu/comm_designs.py
--rw-r--r--   0        0        0    70908 2023-07-26 14:58:39.926632 sdss-mugatu-2.2.2/python/mugatu/designmode.py
--rw-r--r--   0        0        0    24128 2023-08-24 17:06:03.341196 sdss-mugatu-2.2.2/python/mugatu/designs_to_targetdb.py
--rw-r--r--   0        0        0      123 2020-12-17 23:08:43.929881 sdss-mugatu-2.2.2/python/mugatu/etc/mugatu.yml
--rw-r--r--   0        0        0     2345 2022-04-11 22:05:06.045880 sdss-mugatu-2.2.2/python/mugatu/exceptions.py
--rw-r--r--   0        0        0    56688 2023-07-26 14:58:39.929781 sdss-mugatu-2.2.2/python/mugatu/fpsdesign.py
--rw-r--r--   0        0        0     2912 2021-12-15 21:36:43.244598 sdss-mugatu-2.2.2/python/mugatu/templates/dmode_check_w_dists.html
--rw-r--r--   0        0        0     3648 2021-12-15 21:31:24.094630 sdss-mugatu-2.2.2/python/mugatu/templates/dmode_check_w_dists_sky.html
--rw-r--r--   0        0        0     2545 2023-09-28 16:37:23.922441 sdss-mugatu-2.2.2/python/mugatu/templates/main_validation_page.html
--rw-r--r--   0        0        0      669 2021-12-15 20:58:33.216830 sdss-mugatu-2.2.2/python/mugatu/templates/valid_check.html
--rw-r--r--   0        0        0     1200 2021-12-15 21:26:38.661378 sdss-mugatu-2.2.2/python/mugatu/templates/valid_check_w_dists.html
--rw-r--r--   0        0        0     2726 2023-10-03 17:07:47.303537 sdss-mugatu-2.2.2/setup.py
--rw-r--r--   0        0        0     1543 2023-10-03 17:07:47.303972 sdss-mugatu-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1504 2020-12-17 23:08:43.845089 sdss_mugatu-2.3.0/LICENSE.md
+-rw-r--r--   0        0        0      468 2024-05-31 21:38:10.226573 sdss_mugatu-2.3.0/README.md
+-rw-r--r--   0        0        0      817 2024-05-31 21:40:16.027068 sdss_mugatu-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      544 2020-12-17 23:08:43.893921 sdss_mugatu-2.3.0/python/mugatu/__init__.py
+-rw-r--r--   0        0        0    12505 2021-05-26 17:34:23.788221 sdss_mugatu-2.3.0/python/mugatu/comm_designs.py
+-rw-r--r--   0        0        0    72644 2024-05-31 20:11:01.217025 sdss_mugatu-2.3.0/python/mugatu/designmode.py
+-rw-r--r--   0        0        0    24128 2023-08-24 17:06:03.341196 sdss_mugatu-2.3.0/python/mugatu/designs_to_targetdb.py
+-rw-r--r--   0        0        0      123 2020-12-17 23:08:43.929881 sdss_mugatu-2.3.0/python/mugatu/etc/mugatu.yml
+-rw-r--r--   0        0        0     2345 2022-04-11 22:05:06.045880 sdss_mugatu-2.3.0/python/mugatu/exceptions.py
+-rw-r--r--   0        0        0    56688 2023-07-26 14:58:39.929781 sdss_mugatu-2.3.0/python/mugatu/fpsdesign.py
+-rw-r--r--   0        0        0     2912 2021-12-15 21:36:43.244598 sdss_mugatu-2.3.0/python/mugatu/templates/dmode_check_w_dists.html
+-rw-r--r--   0        0        0     3648 2021-12-15 21:31:24.094630 sdss_mugatu-2.3.0/python/mugatu/templates/dmode_check_w_dists_sky.html
+-rw-r--r--   0        0        0     2545 2023-09-28 16:37:23.922441 sdss_mugatu-2.3.0/python/mugatu/templates/main_validation_page.html
+-rw-r--r--   0        0        0      669 2021-12-15 20:58:33.216830 sdss_mugatu-2.3.0/python/mugatu/templates/valid_check.html
+-rw-r--r--   0        0        0     1200 2021-12-15 21:26:38.661378 sdss_mugatu-2.3.0/python/mugatu/templates/valid_check_w_dists.html
+-rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 sdss_mugatu-2.3.0/PKG-INFO
```

### Comparing `sdss-mugatu-2.2.2/LICENSE.md` & `sdss_mugatu-2.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss-mugatu-2.2.2/pyproject.toml` & `sdss_mugatu-2.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "sdss-mugatu"
-version = "2.2.2"
+version = "2.3.0"
 description = "Package to read, write and validate FPS designs"
 authors = ["Ilija Medan"]
 license = "BSD 3-Clause License"
 homepage = "https://pypi.org/project/sdss-mugatu/"
 repository = "https://github.com/sdss/mugatu"
 documentation = "https://mugatu.readthedocs.io/en/latest/"
 readme = "README.md"
 packages = [
     { include = "mugatu", from = "python" }
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 numpy = "^1.19.5"
 fitsio = "^1.0.5"
 sdssdb = "^0.5.4"
 sdss-access = "1.1.1"
 sdss-coordio = "^1.8.1"
 sdss-kaiju = "1.3.1"
 scipy = "^1.6.0"
 jupyter = "^1.0.0"
 ortools = "^9.1.9490"
 DateTime = "^4.3"
 notebook = "^6.4.12"
-astropy = "^5.1"
+astropy = "^5.3.3"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sdss-mugatu-2.2.2/python/mugatu/__init__.py` & `sdss_mugatu-2.3.0/python/mugatu/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss-mugatu-2.2.2/python/mugatu/comm_designs.py` & `sdss_mugatu-2.3.0/python/mugatu/comm_designs.py`

 * *Files identical despite different names*

### Comparing `sdss-mugatu-2.2.2/python/mugatu/designmode.py` & `sdss_mugatu-2.3.0/python/mugatu/designmode.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 except:
     _database = False
 
 from sdssdb.peewee.sdss5db.targetdb import Carton, Category, Magnitude, CartonToTarget, Target
 from sdssdb.peewee.sdss5db.targetdb import DesignMode as DesignModeDB
 from sdssdb.peewee.sdss5db import catalogdb
 from sdssdb.peewee.sdss5db import targetdb
+from sdssdb.peewee.sdss5db import opsdb
 
 
 def ang_sep(ra1, dec1, ra2, dec2):
     """
     Returns angular separation between objects.
 
     Parameters
@@ -1638,7 +1639,60 @@
             verbose_output += 'Bright Neighbor Check (BOSS):     | %d out of %d\n' % (check_tot, design_tot)
 
             check_tot = self.bright_neighbor_check['APOGEE_metric'][0]
             design_tot = self.bright_neighbor_check['APOGEE_metric'][1]
             verbose_output += 'Bright Neighbor Check (APOGEE):   | %d out of %d\n' % (check_tot, design_tot)
 
             print(verbose_output)
+
+
+def check_design_to_status(design_id):
+    """
+    check if the design_id is done
+    """
+    dts = opsdb.DesignToStatus.get_or_none(design_id=design_id)
+    if dts is None:
+        return False
+    else:
+        if dts.status.label == 'done':
+            return True
+        else:
+            return False
+
+
+def designid_status_valid(design_id, field_id, field_exposure):
+    """
+    check if design_id assocatied in rsFieldAssignments file
+    is based on 'done' designs in database.
+
+    Parameters
+    ----------
+    design_id: int
+        The design_id to be validated. If -1, then checks
+        all possible field_exposures in the field.
+    
+    field_id: int
+        field_id for the design.
+
+    field_exposure: int
+        field_exposure for the design.
+
+    Returns
+    -------
+    status: bool
+        If the design_id is set correctly for the design_status.
+    """
+    if design_id != -1:
+        status = check_design_to_status(design_id)
+    else:
+        # grab all design_ids for current field_exposure in all verisons
+        # of the field
+        designs = targetdb.DesignToField.select()\
+                                        .join(targetdb.Field)\
+                                        .where(targetdb.Field.field_id == field_id,
+                                               targetdb.DesignToField.field_exposure == field_exposure)
+        # check all of the designs to see if they are marked done
+        design_status = np.zeros(len(designs), dtype=bool)
+        for i, d in enumerate(designs):
+            design_status[i] = check_design_to_status(d.design_id)
+        status = ~np.any(design_status)  # should all be False if design_id = -1
+    return status
```

### Comparing `sdss-mugatu-2.2.2/python/mugatu/designs_to_targetdb.py` & `sdss_mugatu-2.3.0/python/mugatu/designs_to_targetdb.py`

 * *Files identical despite different names*

### Comparing `sdss-mugatu-2.2.2/python/mugatu/exceptions.py` & `sdss_mugatu-2.3.0/python/mugatu/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss-mugatu-2.2.2/python/mugatu/fpsdesign.py` & `sdss_mugatu-2.3.0/python/mugatu/fpsdesign.py`

 * *Files identical despite different names*

### Comparing `sdss-mugatu-2.2.2/python/mugatu/templates/dmode_check_w_dists.html` & `sdss_mugatu-2.3.0/python/mugatu/templates/dmode_check_w_dists.html`

 * *Files identical despite different names*

### Comparing `sdss-mugatu-2.2.2/python/mugatu/templates/dmode_check_w_dists_sky.html` & `sdss_mugatu-2.3.0/python/mugatu/templates/dmode_check_w_dists_sky.html`

 * *Files identical despite different names*

### Comparing `sdss-mugatu-2.2.2/python/mugatu/templates/main_validation_page.html` & `sdss_mugatu-2.3.0/python/mugatu/templates/main_validation_page.html`

 * *Files identical despite different names*

### Comparing `sdss-mugatu-2.2.2/python/mugatu/templates/valid_check.html` & `sdss_mugatu-2.3.0/python/mugatu/templates/valid_check.html`

 * *Files identical despite different names*

### Comparing `sdss-mugatu-2.2.2/python/mugatu/templates/valid_check_w_dists.html` & `sdss_mugatu-2.3.0/python/mugatu/templates/valid_check_w_dists.html`

 * *Files identical despite different names*

### Comparing `sdss-mugatu-2.2.2/PKG-INFO` & `sdss_mugatu-2.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: sdss-mugatu
-Version: 2.2.2
+Version: 2.3.0
 Summary: Package to read, write and validate FPS designs
 Home-page: https://pypi.org/project/sdss-mugatu/
 License: BSD 3-Clause License
 Author: Ilija Medan
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: DateTime (>=4.3,<5.0)
-Requires-Dist: astropy (>=5.1,<6.0)
+Requires-Dist: astropy (>=5.3.3,<6.0.0)
 Requires-Dist: fitsio (>=1.0.5,<2.0.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: notebook (>=6.4.12,<7.0.0)
 Requires-Dist: numpy (>=1.19.5,<2.0.0)
 Requires-Dist: ortools (>=9.1.9490,<10.0.0)
 Requires-Dist: scipy (>=1.6.0,<2.0.0)
 Requires-Dist: sdss-access (==1.1.1)
@@ -24,15 +26,15 @@
 Requires-Dist: sdssdb (>=0.5.4,<0.6.0)
 Project-URL: Documentation, https://mugatu.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/sdss/mugatu
 Description-Content-Type: text/markdown
 
 # mugatu
 
-![Versions](https://img.shields.io/badge/python->3.8-blue)
+![Versions](https://img.shields.io/badge/python->3.9-blue)
 [![Documentation Status](https://readthedocs.org/projects/mugatu/badge/?version=latest)](https://mugatu.readthedocs.io/en/latest/#)
 <!---
 [![Travis (.org)](https://img.shields.io/travis/sdss/mugatu)](https://travis-ci.org/sdss/mugatu)
 [![codecov](https://codecov.io/gh/sdss/mugatu/branch/main/graph/badge.svg)](https://codecov.io/gh/sdss/mugatu)
 -->
 
 Package to read, write and validate FPS designs
```

