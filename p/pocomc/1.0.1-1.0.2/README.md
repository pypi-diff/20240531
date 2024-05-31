# Comparing `tmp/pocomc-1.0.1.tar.gz` & `tmp/pocomc-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocomc-1.0.1.tar", last modified: Mon Jan 29 23:00:27 2024, max compression
+gzip compressed data, was "pocomc-1.0.2.tar", last modified: Mon Feb 19 00:25:35 2024, max compression
```

## Comparing `pocomc-1.0.1.tar` & `pocomc-1.0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 23:00:27.816594 pocomc-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-29 23:00:15.000000 pocomc-1.0.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-01-29 23:00:27.816594 pocomc-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-01-29 23:00:15.000000 pocomc-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 23:00:27.816594 pocomc-1.0.1/pocomc/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-01-29 23:00:15.000000 pocomc-1.0.1/pocomc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-29 23:00:15.000000 pocomc-1.0.1/pocomc/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    13262 2024-01-29 23:00:15.000000 pocomc-1.0.1/pocomc/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-01-29 23:00:15.000000 pocomc-1.0.1/pocomc/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-01-29 23:00:15.000000 pocomc-1.0.1/pocomc/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16481 2024-01-29 23:00:15.000000 pocomc-1.0.1/pocomc/mcmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    14136 2024-01-29 23:00:15.000000 pocomc-1.0.1/pocomc/particles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-01-29 23:00:15.000000 pocomc-1.0.1/pocomc/prior.py
--rw-r--r--   0 runner    (1001) docker     (127)    27368 2024-01-29 23:00:15.000000 pocomc-1.0.1/pocomc/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    15125 2024-01-29 23:00:15.000000 pocomc-1.0.1/pocomc/scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-01-29 23:00:15.000000 pocomc-1.0.1/pocomc/student.py
--rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-01-29 23:00:15.000000 pocomc-1.0.1/pocomc/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 23:00:27.816594 pocomc-1.0.1/pocomc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-01-29 23:00:27.000000 pocomc-1.0.1/pocomc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-01-29 23:00:27.000000 pocomc-1.0.1/pocomc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 23:00:27.000000 pocomc-1.0.1/pocomc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 23:00:27.000000 pocomc-1.0.1/pocomc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-29 23:00:27.000000 pocomc-1.0.1/pocomc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-29 23:00:27.000000 pocomc-1.0.1/pocomc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-01-29 23:00:27.816594 pocomc-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 23:00:15.000000 pocomc-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 23:00:27.816594 pocomc-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-01-29 23:00:15.000000 pocomc-1.0.1/tests/test_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-01-29 23:00:15.000000 pocomc-1.0.1/tests/test_prior.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-01-29 23:00:15.000000 pocomc-1.0.1/tests/test_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-01-29 23:00:15.000000 pocomc-1.0.1/tests/test_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-01-29 23:00:15.000000 pocomc-1.0.1/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-01-29 23:00:15.000000 pocomc-1.0.1/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:25:35.897504 pocomc-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-19 00:25:24.000000 pocomc-1.0.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-02-19 00:25:35.897504 pocomc-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-02-19 00:25:24.000000 pocomc-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:25:35.897504 pocomc-1.0.2/pocomc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-02-19 00:25:24.000000 pocomc-1.0.2/pocomc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-19 00:25:24.000000 pocomc-1.0.2/pocomc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13262 2024-02-19 00:25:24.000000 pocomc-1.0.2/pocomc/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-02-19 00:25:24.000000 pocomc-1.0.2/pocomc/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-02-19 00:25:24.000000 pocomc-1.0.2/pocomc/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16481 2024-02-19 00:25:24.000000 pocomc-1.0.2/pocomc/mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14136 2024-02-19 00:25:24.000000 pocomc-1.0.2/pocomc/particles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-02-19 00:25:24.000000 pocomc-1.0.2/pocomc/prior.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27368 2024-02-19 00:25:24.000000 pocomc-1.0.2/pocomc/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15080 2024-02-19 00:25:24.000000 pocomc-1.0.2/pocomc/scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-02-19 00:25:24.000000 pocomc-1.0.2/pocomc/student.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-02-19 00:25:24.000000 pocomc-1.0.2/pocomc/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:25:35.897504 pocomc-1.0.2/pocomc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-02-19 00:25:35.000000 pocomc-1.0.2/pocomc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-19 00:25:35.000000 pocomc-1.0.2/pocomc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 00:25:35.000000 pocomc-1.0.2/pocomc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 00:25:35.000000 pocomc-1.0.2/pocomc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-19 00:25:35.000000 pocomc-1.0.2/pocomc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-19 00:25:35.000000 pocomc-1.0.2/pocomc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-02-19 00:25:35.897504 pocomc-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 00:25:24.000000 pocomc-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:25:35.897504 pocomc-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-02-19 00:25:24.000000 pocomc-1.0.2/tests/test_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-02-19 00:25:24.000000 pocomc-1.0.2/tests/test_prior.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-02-19 00:25:24.000000 pocomc-1.0.2/tests/test_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-02-19 00:25:24.000000 pocomc-1.0.2/tests/test_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-02-19 00:25:24.000000 pocomc-1.0.2/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-02-19 00:25:24.000000 pocomc-1.0.2/tests/test_tools.py
```

### Comparing `pocomc-1.0.1/LICENCE` & `pocomc-1.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `pocomc-1.0.1/PKG-INFO` & `pocomc-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocomc
-Version: 1.0.1
+Version: 1.0.2
 Summary: Preconditioned Monte Carlo
 Home-page: https://github.com/minaskar/pocomc
 Author: Minas Karamanis
 Author-email: minaskar@gmail.com
 License: GPLv3
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pocomc-1.0.1/README.md` & `pocomc-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pocomc-1.0.1/pocomc/__init__.py` & `pocomc-1.0.2/pocomc/__init__.py`

 * *Files identical despite different names*

### Comparing `pocomc-1.0.1/pocomc/flow.py` & `pocomc-1.0.2/pocomc/flow.py`

 * *Files identical despite different names*

### Comparing `pocomc-1.0.1/pocomc/geometry.py` & `pocomc-1.0.2/pocomc/geometry.py`

 * *Files identical despite different names*

### Comparing `pocomc-1.0.1/pocomc/input_validation.py` & `pocomc-1.0.2/pocomc/input_validation.py`

 * *Files identical despite different names*

### Comparing `pocomc-1.0.1/pocomc/mcmc.py` & `pocomc-1.0.2/pocomc/mcmc.py`

 * *Files identical despite different names*

### Comparing `pocomc-1.0.1/pocomc/particles.py` & `pocomc-1.0.2/pocomc/particles.py`

 * *Files identical despite different names*

### Comparing `pocomc-1.0.1/pocomc/prior.py` & `pocomc-1.0.2/pocomc/prior.py`

 * *Files identical despite different names*

### Comparing `pocomc-1.0.1/pocomc/sampler.py` & `pocomc-1.0.2/pocomc/sampler.py`

 * *Files identical despite different names*

### Comparing `pocomc-1.0.1/pocomc/scaler.py` & `pocomc-1.0.2/pocomc/scaler.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,15 +262,15 @@
         J = np.empty(u.shape)
 
         x[:, self.mask_none], J[:, self.mask_none] = self._inverse_none(u)
         x[:, self.mask_left], J[:, self.mask_left] = self._inverse_left(u)
         x[:, self.mask_right], J[:, self.mask_right] = self._inverse_right(u)
         x[:, self.mask_both], J[:, self.mask_both] = self._inverse_both(u)
 
-        log_det_J = np.array([np.linalg.slogdet(Ji * np.identity(len(Ji)))[1] for Ji in J])
+        log_det_J = np.log(np.prod(J, axis=1))
 
         return x, log_det_J
 
     def _forward_affine(self, x: np.ndarray):
         """
         Forward affine transformation.
```

### Comparing `pocomc-1.0.1/pocomc/student.py` & `pocomc-1.0.2/pocomc/student.py`

 * *Files identical despite different names*

### Comparing `pocomc-1.0.1/pocomc/tools.py` & `pocomc-1.0.2/pocomc/tools.py`

 * *Files identical despite different names*

### Comparing `pocomc-1.0.1/pocomc.egg-info/PKG-INFO` & `pocomc-1.0.2/pocomc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocomc
-Version: 1.0.1
+Version: 1.0.2
 Summary: Preconditioned Monte Carlo
 Home-page: https://github.com/minaskar/pocomc
 Author: Minas Karamanis
 Author-email: minaskar@gmail.com
 License: GPLv3
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pocomc-1.0.1/pocomc.egg-info/SOURCES.txt` & `pocomc-1.0.2/pocomc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pocomc-1.0.1/setup.cfg` & `pocomc-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pocomc-1.0.1/tests/test_flow.py` & `pocomc-1.0.2/tests/test_flow.py`

 * *Files identical despite different names*

### Comparing `pocomc-1.0.1/tests/test_prior.py` & `pocomc-1.0.2/tests/test_prior.py`

 * *Files identical despite different names*

### Comparing `pocomc-1.0.1/tests/test_sampler.py` & `pocomc-1.0.2/tests/test_sampler.py`

 * *Files identical despite different names*

### Comparing `pocomc-1.0.1/tests/test_scaler.py` & `pocomc-1.0.2/tests/test_scaler.py`

 * *Files identical despite different names*

### Comparing `pocomc-1.0.1/tests/test_state.py` & `pocomc-1.0.2/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `pocomc-1.0.1/tests/test_tools.py` & `pocomc-1.0.2/tests/test_tools.py`

 * *Files identical despite different names*

