# Comparing `tmp/pyswxf-0.6.8.tar.gz` & `tmp/pyswxf-0.6.9.tar.gz`

## Comparing `pyswxf-0.6.8.tar` & `pyswxf-0.6.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 pyswxf-0.6.8/PyPI-Recovery-Codes-luriol-2023-10-13T13_43_44.046510.txt
--rwxr-xr-x   0        0        0      498 2020-02-02 00:00:00.000000 pyswxf-0.6.8/cbwe.py
--rwxr-xr-x   0        0        0      609 2020-02-02 00:00:00.000000 pyswxf-0.6.8/dot_pypirc
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 pyswxf-0.6.8/instructions
--rwxr-xr-x   0        0        0      724 2020-02-02 00:00:00.000000 pyswxf-0.6.8/pyproject.bak
--rwxr-xr-x   0        0        0      592 2020-02-02 00:00:00.000000 pyswxf-0.6.8/pyproject.new
--rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 pyswxf-0.6.8/token
--rwxr-xr-x   0        0        0     5451 2020-02-02 00:00:00.000000 pyswxf-0.6.8/src/pySWXF/AuI_funs (DESKTOP-09M4OT9's conflicted copy 2024-05-15).py
--rwxr-xr-x   0        0        0    21877 2020-02-02 00:00:00.000000 pyswxf-0.6.8/src/pySWXF/AuI_funs.py
--rwxr-xr-x   0        0        0     2479 2020-02-02 00:00:00.000000 pyswxf-0.6.8/src/pySWXF/Br_funs.py
--rwxr-xr-x   0        0        0     3063 2020-02-02 00:00:00.000000 pyswxf-0.6.8/src/pySWXF/NM_clean_NIU_NOKW_Mar26_24_fit4.json
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.6.8/src/pySWXF/__init__.py
--rwxr-xr-x   0        0        0    12009 2020-02-02 00:00:00.000000 pyswxf-0.6.8/src/pySWXF/fluor_fit.py
--rwxr-xr-x   0        0        0     6752 2020-02-02 00:00:00.000000 pyswxf-0.6.8/src/pySWXF/niu_multilayer_fit_params_3_LBL.json
--rwxr-xr-x   0        0        0     6863 2020-02-02 00:00:00.000000 pyswxf-0.6.8/src/pySWXF/refl_funs.py
--rwxr-xr-x   0        0        0    27347 2020-02-02 00:00:00.000000 pyswxf-0.6.8/src/pySWXF/spec_utils.py
--rwxr-xr-x   0        0        0     2747 2020-02-02 00:00:00.000000 pyswxf-0.6.8/src/pySWXF/view_new_multilayer.ipynb
--rwxr-xr-x   0        0        0      952 2020-02-02 00:00:00.000000 pyswxf-0.6.8/src/pySWXF/xray_utils.py
--rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 pyswxf-0.6.8/LICENSE
--rwxr-xr-x   0        0        0     3321 2020-02-02 00:00:00.000000 pyswxf-0.6.8/README.md
--rwxr-xr-x   0        0        0      592 2020-02-02 00:00:00.000000 pyswxf-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 pyswxf-0.6.8/PKG-INFO
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 pyswxf-0.6.9/PyPI-Recovery-Codes-luriol-2023-10-13T13_43_44.046510.txt
+-rwxr-xr-x   0        0        0      498 2020-02-02 00:00:00.000000 pyswxf-0.6.9/cbwe.py
+-rwxr-xr-x   0        0        0      609 2020-02-02 00:00:00.000000 pyswxf-0.6.9/dot_pypirc
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 pyswxf-0.6.9/instructions
+-rwxr-xr-x   0        0        0      724 2020-02-02 00:00:00.000000 pyswxf-0.6.9/pyproject.bak
+-rwxr-xr-x   0        0        0      592 2020-02-02 00:00:00.000000 pyswxf-0.6.9/pyproject.new
+-rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 pyswxf-0.6.9/token
+-rwxr-xr-x   0        0        0     5451 2020-02-02 00:00:00.000000 pyswxf-0.6.9/src/pySWXF/AuI_funs (DESKTOP-09M4OT9's conflicted copy 2024-05-15).py
+-rwxr-xr-x   0        0        0    21877 2020-02-02 00:00:00.000000 pyswxf-0.6.9/src/pySWXF/AuI_funs.py
+-rwxr-xr-x   0        0        0     2479 2020-02-02 00:00:00.000000 pyswxf-0.6.9/src/pySWXF/Br_funs.py
+-rwxr-xr-x   0        0        0     3063 2020-02-02 00:00:00.000000 pyswxf-0.6.9/src/pySWXF/NM_clean_NIU_NOKW_Mar26_24_fit4.json
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.6.9/src/pySWXF/__init__.py
+-rwxr-xr-x   0        0        0    12009 2020-02-02 00:00:00.000000 pyswxf-0.6.9/src/pySWXF/fluor_fit.py
+-rwxr-xr-x   0        0        0     6752 2020-02-02 00:00:00.000000 pyswxf-0.6.9/src/pySWXF/niu_multilayer_fit_params_3_LBL.json
+-rwxr-xr-x   0        0        0     6863 2020-02-02 00:00:00.000000 pyswxf-0.6.9/src/pySWXF/refl_funs.py
+-rwxr-xr-x   0        0        0    27347 2020-02-02 00:00:00.000000 pyswxf-0.6.9/src/pySWXF/spec_utils.py
+-rwxr-xr-x   0        0        0     2747 2020-02-02 00:00:00.000000 pyswxf-0.6.9/src/pySWXF/view_new_multilayer.ipynb
+-rwxr-xr-x   0        0        0      952 2020-02-02 00:00:00.000000 pyswxf-0.6.9/src/pySWXF/xray_utils.py
+-rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 pyswxf-0.6.9/LICENSE
+-rwxr-xr-x   0        0        0     3321 2020-02-02 00:00:00.000000 pyswxf-0.6.9/README.md
+-rwxr-xr-x   0        0        0      592 2020-02-02 00:00:00.000000 pyswxf-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 pyswxf-0.6.9/PKG-INFO
```

### Comparing `pyswxf-0.6.8/dot_pypirc` & `pyswxf-0.6.9/dot_pypirc`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.8/pyproject.bak` & `pyswxf-0.6.9/pyproject.bak`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.8/pyproject.new` & `pyswxf-0.6.9/pyproject.new`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.8/src/pySWXF/AuI_funs (DESKTOP-09M4OT9's conflicted copy 2024-05-15).py` & `pyswxf-0.6.9/src/pySWXF/AuI_funs (DESKTOP-09M4OT9's conflicted copy 2024-05-15).py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.8/src/pySWXF/AuI_funs.py` & `pyswxf-0.6.9/src/pySWXF/AuI_funs.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.8/src/pySWXF/Br_funs.py` & `pyswxf-0.6.9/src/pySWXF/Br_funs.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.8/src/pySWXF/NM_clean_NIU_NOKW_Mar26_24_fit4.json` & `pyswxf-0.6.9/src/pySWXF/NM_clean_NIU_NOKW_Mar26_24_fit4.json`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.8/src/pySWXF/fluor_fit.py` & `pyswxf-0.6.9/src/pySWXF/fluor_fit.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.8/src/pySWXF/niu_multilayer_fit_params_3_LBL.json` & `pyswxf-0.6.9/src/pySWXF/niu_multilayer_fit_params_3_LBL.json`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.8/src/pySWXF/refl_funs.py` & `pyswxf-0.6.9/src/pySWXF/refl_funs.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.8/src/pySWXF/spec_utils.py` & `pyswxf-0.6.9/src/pySWXF/spec_utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.8/src/pySWXF/view_new_multilayer.ipynb` & `pyswxf-0.6.9/src/pySWXF/view_new_multilayer.ipynb`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.8/src/pySWXF/xray_utils.py` & `pyswxf-0.6.9/src/pySWXF/xray_utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.8/LICENSE` & `pyswxf-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.8/README.md` & `pyswxf-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.8/pyproject.toml` & `pyswxf-0.6.9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling==1.17.1"]
 build-backend = "hatchling.build"
 [project]
 name = "pySWXF"
-version = "0.6.8"
+version = "0.6.9"
 authors = [
 	{name="Laurence Lurio", email="llurio@niu.edu" },
 ]
 description = "Routines for calculating standing wave x-ray fluorescence and x-ray reflectivity"
 readme = "README.md"
 requires-python = ">3.7"
 classifiers = [
```

### Comparing `pyswxf-0.6.8/PKG-INFO` & `pyswxf-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySWXF
-Version: 0.6.8
+Version: 0.6.9
 Summary: Routines for calculating standing wave x-ray fluorescence and x-ray reflectivity
 Project-URL: Homepage, https://github.com/pypa/pySWXF
 Project-URL: Bug Tracker, https://github.com/pypa/pySWXF/issues
 Author-email: Laurence Lurio <llurio@niu.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

