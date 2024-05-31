# Comparing `tmp/inu-1.0.9.tar.gz` & `tmp/inu-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inu-1.0.9.tar", last modified: Thu Dec 14 20:17:22 2023, max compression
+gzip compressed data, was "inu-1.1.0.tar", last modified: Fri May 31 18:20:15 2024, max compression
```

## Comparing `inu-1.0.9.tar` & `inu-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2023-12-14 20:17:22.792895 inu-1.0.9/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1059 2023-09-06 19:38:32.000000 inu-1.0.9/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     2283 2023-12-14 20:17:22.792842 inu-1.0.9/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1829 2023-11-22 20:35:05.000000 inu-1.0.9/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 inu-1.0.9/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      576 2023-12-14 20:17:22.793103 inu-1.0.9/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2023-12-14 20:17:22.790426 inu-1.0.9/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2023-12-14 20:17:22.791859 inu-1.0.9/src/inu/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2023-09-06 20:09:43.000000 inu-1.0.9/src/inu/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    24594 2023-12-14 20:16:28.000000 inu-1.0.9/src/inu/inu.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     3381 2023-12-14 19:50:22.000000 inu-1.0.9/src/inu/test_inu.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2023-12-14 20:17:22.792660 inu-1.0.9/src/inu.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     2283 2023-12-14 20:17:22.000000 inu-1.0.9/src/inu.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      255 2023-12-14 20:17:22.000000 inu-1.0.9/src/inu.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2023-12-14 20:17:22.000000 inu-1.0.9/src/inu.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2023-12-14 20:17:22.000000 inu-1.0.9/src/inu.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2023-12-14 20:17:22.000000 inu-1.0.9/src/inu.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-31 18:20:15.114187 inu-1.1.0/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1059 2023-09-06 19:38:32.000000 inu-1.1.0/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     9164 2024-05-31 18:20:15.114113 inu-1.1.0/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8689 2024-05-31 18:14:43.000000 inu-1.1.0/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 inu-1.1.0/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      583 2024-05-31 18:20:15.114421 inu-1.1.0/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-31 18:20:15.112072 inu-1.1.0/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-31 18:20:15.113138 inu-1.1.0/src/inu/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2023-09-06 20:09:43.000000 inu-1.1.0/src/inu/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    45290 2024-05-31 18:01:13.000000 inu-1.1.0/src/inu/inu.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     3548 2024-05-31 18:01:26.000000 inu-1.1.0/src/inu/test_inu.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-31 18:20:15.113904 inu-1.1.0/src/inu.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     9164 2024-05-31 18:20:15.000000 inu-1.1.0/src/inu.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      255 2024-05-31 18:20:15.000000 inu-1.1.0/src/inu.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-31 18:20:15.000000 inu-1.1.0/src/inu.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       12 2024-05-31 18:20:15.000000 inu-1.1.0/src/inu.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-05-31 18:20:15.000000 inu-1.1.0/src/inu.egg-info/top_level.txt
```

### Comparing `inu-1.0.9/LICENSE.txt` & `inu-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `inu-1.0.9/setup.cfg` & `inu-1.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = inu
-version = 1.0.9
+version = 1.1.0
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = Inertial Navigation Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/inu
 classifiers = 
@@ -15,14 +15,15 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	numpy
+	scipy
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `inu-1.0.9/src/inu/test_inu.py` & `inu-1.1.0/src/inu/test_inu.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Run `pytest` in the terminal.
 
-import inu
+import time
 import numpy as np
-import matplotlib.pyplot as plt
+import scipy as sp
+import inu
+import itrm
 
 
 def fake_path(T, axis=1):
     # Define time.
     K = round(360.0/T) + 1
     t = np.arange(K)*T
 
@@ -21,24 +23,24 @@
     # Transpose.
     if axis == 0:
         llh_t = llh_t.T
 
     return t, llh_t
 
 
-def test_somiliana():
+def test_somigliana():
     # lists
     llh_t = [[np.pi/4, 0, 0],
         [np.pi/5, 0.01, 100.0]]
-    grav = inu.somigliana(llh_t)
-    assert np.allclose(np.linalg.norm(grav, axis=1),
+    gam_t = inu.somigliana(llh_t)
+    assert np.allclose(np.linalg.norm(gam_t, axis=1),
         np.array([9.80619777, 9.79788193]))
     # horizontal time variance
-    grav = inu.somigliana(np.array(llh_t).T)
-    assert np.allclose(np.linalg.norm(grav, axis=0),
+    gam_t = inu.somigliana(np.array(llh_t).T)
+    assert np.allclose(np.linalg.norm(gam_t, axis=0),
         np.array([9.80619777, 9.79788193]))
 
 
 def test_rpy_dcm():
     # multiple single duals
     N = 5
     RPY = np.zeros((3, N))
@@ -87,43 +89,45 @@
 
 def test_mech():
     # ------------------------------------
     # Test with time varying along axis 1.
     # ------------------------------------
 
     # Build path.
-    T = 0.1
+    T = 0.01
     t, llh = fake_path(T)
     vne = inu.llh_to_vne(llh, T)
-    grav = inu.somigliana(llh)
-    rpy = inu.vne_to_rpy(vne, grav[2, :], T)
+    gam = inu.somigliana(llh)
+    rpy = inu.vne_to_rpy(vne, gam[2, :], T)
 
     # Inverse and forward mechanize.
-    hfbbi, hwbbi = inu.inv_mech(llh, vne, rpy, T)
+    tic = time.perf_counter()
+    hfbbi, hwbbi = inu.inv_mech(llh, rpy, T)
+    print(time.perf_counter() - tic)
     tllh, tvne, trpy = inu.mech(hfbbi, hwbbi,
-        llh[:, 0], vne[:, 0], rpy[:, 0], T)
+        llh[:, 0], vne[:, 0], rpy[:, 0], T, show_progress=False)
 
     assert np.allclose(llh, tllh)
     assert np.allclose(vne, tvne)
     assert np.allclose(rpy, trpy)
 
     # ------------------------------------
     # Test with time varying along axis 0.
     # ------------------------------------
 
     # Build path.
-    T = 0.1
+    T = 0.01
     t, llh = fake_path(T, axis=0)
     vne = inu.llh_to_vne(llh, T)
-    grav = inu.somigliana(llh)
-    rpy = inu.vne_to_rpy(vne, grav[:, 2], T)
+    gam = inu.somigliana(llh)
+    rpy = inu.vne_to_rpy(vne, gam[:, 2], T)
 
     # Inverse and forward mechanize.
-    hfbbi, hwbbi = inu.inv_mech(llh, vne, rpy, T)
+    tic = time.perf_counter()
+    hfbbi, hwbbi = inu.inv_mech(llh, rpy, T)
+    print(time.perf_counter() - tic)
     tllh, tvne, trpy = inu.mech(hfbbi, hwbbi,
-        llh[0, :], vne[0, :], rpy[0, :], T)
+        llh[0, :], vne[0, :], rpy[0, :], T, show_progress=False)
 
     assert np.allclose(llh, tllh)
     assert np.allclose(vne, tvne)
     assert np.allclose(rpy, trpy)
-
-test_mech()
```

