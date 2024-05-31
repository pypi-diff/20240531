# Comparing `tmp/tmgtoolkit-0.1.4.tar.gz` & `tmp/tmgtoolkit-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmgtoolkit-0.1.4.tar", last modified: Thu May 23 21:42:08 2024, max compression
+gzip compressed data, was "tmgtoolkit-0.1.5.tar", last modified: Fri May 31 06:23:12 2024, max compression
```

## Comparing `tmgtoolkit-0.1.4.tar` & `tmgtoolkit-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-23 21:42:08.187594 tmgtoolkit-0.1.4/
--rw-r--r--   0 ej        (1000) wheel      (998)    34916 2024-04-10 06:55:31.000000 tmgtoolkit-0.1.4/LICENSE.md
--rw-r--r--   0 ej        (1000) wheel      (998)     1259 2024-05-23 21:42:08.187594 tmgtoolkit-0.1.4/PKG-INFO
--rw-r--r--   0 ej        (1000) wheel      (998)      563 2024-04-10 07:01:19.000000 tmgtoolkit-0.1.4/README.md
--rw-r--r--   0 ej        (1000) wheel      (998)      103 2024-04-10 07:09:13.000000 tmgtoolkit-0.1.4/pyproject.toml
--rw-r--r--   0 ej        (1000) wheel      (998)      754 2024-05-23 21:42:08.187594 tmgtoolkit-0.1.4/setup.cfg
-drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-23 21:42:08.180928 tmgtoolkit-0.1.4/src/
-drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-23 21:42:08.184261 tmgtoolkit-0.1.4/src/tmgtoolkit/
--rw-r--r--   0 ej        (1000) wheel      (998)        0 2024-04-09 14:32:51.000000 tmgtoolkit-0.1.4/src/tmgtoolkit/__init__.py
--rw-r--r--   0 ej        (1000) wheel      (998)     6958 2024-05-20 20:55:42.000000 tmgtoolkit-0.1.4/src/tmgtoolkit/constants.py
--rw-r--r--   0 ej        (1000) wheel      (998)    16033 2024-05-10 15:04:33.000000 tmgtoolkit-0.1.4/src/tmgtoolkit/plotting.py
--rw-r--r--   0 ej        (1000) wheel      (998)    13745 2024-05-10 15:04:51.000000 tmgtoolkit-0.1.4/src/tmgtoolkit/spm.py
--rw-r--r--   0 ej        (1000) wheel      (998)    18744 2024-05-14 21:23:52.000000 tmgtoolkit-0.1.4/src/tmgtoolkit/time_series.py
--rw-r--r--   0 ej        (1000) wheel      (998)    15481 2024-05-21 17:51:44.000000 tmgtoolkit-0.1.4/src/tmgtoolkit/tmgio.py
-drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-23 21:42:08.187594 tmgtoolkit-0.1.4/src/tmgtoolkit.egg-info/
--rw-r--r--   0 ej        (1000) wheel      (998)     1259 2024-05-23 21:42:08.000000 tmgtoolkit-0.1.4/src/tmgtoolkit.egg-info/PKG-INFO
--rw-r--r--   0 ej        (1000) wheel      (998)      443 2024-05-23 21:42:08.000000 tmgtoolkit-0.1.4/src/tmgtoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 ej        (1000) wheel      (998)        1 2024-05-23 21:42:08.000000 tmgtoolkit-0.1.4/src/tmgtoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 ej        (1000) wheel      (998)       50 2024-05-23 21:42:08.000000 tmgtoolkit-0.1.4/src/tmgtoolkit.egg-info/requires.txt
--rw-r--r--   0 ej        (1000) wheel      (998)       11 2024-05-23 21:42:08.000000 tmgtoolkit-0.1.4/src/tmgtoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-23 21:42:08.187594 tmgtoolkit-0.1.4/tests/
--rw-r--r--   0 ej        (1000) wheel      (998)       85 2024-05-19 13:02:48.000000 tmgtoolkit-0.1.4/tests/test_mwe.py
--rw-r--r--   0 ej        (1000) wheel      (998)     7349 2024-05-20 20:56:27.000000 tmgtoolkit-0.1.4/tests/test_split_data_for_spm.py
+drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-31 06:23:12.420205 tmgtoolkit-0.1.5/
+-rw-r--r--   0 ej        (1000) wheel      (998)    34916 2024-04-10 06:55:31.000000 tmgtoolkit-0.1.5/LICENSE.md
+-rw-r--r--   0 ej        (1000) wheel      (998)     1259 2024-05-31 06:23:12.420205 tmgtoolkit-0.1.5/PKG-INFO
+-rw-r--r--   0 ej        (1000) wheel      (998)      563 2024-04-10 07:01:19.000000 tmgtoolkit-0.1.5/README.md
+-rw-r--r--   0 ej        (1000) wheel      (998)      103 2024-04-10 07:09:13.000000 tmgtoolkit-0.1.5/pyproject.toml
+-rw-r--r--   0 ej        (1000) wheel      (998)      754 2024-05-31 06:23:12.420205 tmgtoolkit-0.1.5/setup.cfg
+drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-31 06:23:12.413538 tmgtoolkit-0.1.5/src/
+drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-31 06:23:12.416872 tmgtoolkit-0.1.5/src/tmgtoolkit/
+-rw-r--r--   0 ej        (1000) wheel      (998)        0 2024-04-09 14:32:51.000000 tmgtoolkit-0.1.5/src/tmgtoolkit/__init__.py
+-rw-r--r--   0 ej        (1000) wheel      (998)     6972 2024-05-31 06:12:51.000000 tmgtoolkit-0.1.5/src/tmgtoolkit/constants.py
+-rw-r--r--   0 ej        (1000) wheel      (998)    16033 2024-05-10 15:04:33.000000 tmgtoolkit-0.1.5/src/tmgtoolkit/plotting.py
+-rw-r--r--   0 ej        (1000) wheel      (998)    13745 2024-05-10 15:04:51.000000 tmgtoolkit-0.1.5/src/tmgtoolkit/spm.py
+-rw-r--r--   0 ej        (1000) wheel      (998)    18991 2024-05-31 06:20:41.000000 tmgtoolkit-0.1.5/src/tmgtoolkit/time_series.py
+-rw-r--r--   0 ej        (1000) wheel      (998)    15481 2024-05-21 17:51:44.000000 tmgtoolkit-0.1.5/src/tmgtoolkit/tmgio.py
+drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-31 06:23:12.416872 tmgtoolkit-0.1.5/src/tmgtoolkit.egg-info/
+-rw-r--r--   0 ej        (1000) wheel      (998)     1259 2024-05-31 06:23:12.000000 tmgtoolkit-0.1.5/src/tmgtoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 ej        (1000) wheel      (998)      443 2024-05-31 06:23:12.000000 tmgtoolkit-0.1.5/src/tmgtoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 ej        (1000) wheel      (998)        1 2024-05-31 06:23:12.000000 tmgtoolkit-0.1.5/src/tmgtoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 ej        (1000) wheel      (998)       50 2024-05-31 06:23:12.000000 tmgtoolkit-0.1.5/src/tmgtoolkit.egg-info/requires.txt
+-rw-r--r--   0 ej        (1000) wheel      (998)       11 2024-05-31 06:23:12.000000 tmgtoolkit-0.1.5/src/tmgtoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-31 06:23:12.416872 tmgtoolkit-0.1.5/tests/
+-rw-r--r--   0 ej        (1000) wheel      (998)       85 2024-05-19 13:02:48.000000 tmgtoolkit-0.1.5/tests/test_mwe.py
+-rw-r--r--   0 ej        (1000) wheel      (998)     7349 2024-05-20 20:56:27.000000 tmgtoolkit-0.1.5/tests/test_split_data_for_spm.py
```

### Comparing `tmgtoolkit-0.1.4/LICENSE.md` & `tmgtoolkit-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tmgtoolkit-0.1.4/PKG-INFO` & `tmgtoolkit-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmgtoolkit
-Version: 0.1.4
+Version: 0.1.5
 Summary: Time series analysis of tensiomyography (TMG) data
 Home-page: https://github.com/ejmastnak/tmgtoolkit
 Author: Elijan Mastnak
 Author-email: admin@ejmastnak.com
 Project-URL: Bug Tracker, https://github.com/ejmastnak/tmgtoolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tmgtoolkit-0.1.4/README.md` & `tmgtoolkit-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tmgtoolkit-0.1.4/setup.cfg` & `tmgtoolkit-0.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tmgtoolkit
-version = 0.1.4
+version = 0.1.5
 author = Elijan Mastnak
 author_email = admin@ejmastnak.com
 description = Time series analysis of tensiomyography (TMG) data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejmastnak/tmgtoolkit
 project_urls =
```

### Comparing `tmgtoolkit-0.1.4/src/tmgtoolkit/constants.py` & `tmgtoolkit-0.1.5/src/tmgtoolkit/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,14 +139,15 @@
             'x_axis_linestyle': ':',
             'legend_alpha': 1.0,
             }
 
 class NamedTupleTypes:
     TmgParams = namedtuple('TmgParams', [
         'dm',
+        'tm',
         'td',
         'tc',
         'ts',
         'tr'
         ])
     ExtremumParams = namedtuple('ExtremumParams', [
         'max_time',
```

### Comparing `tmgtoolkit-0.1.4/src/tmgtoolkit/plotting.py` & `tmgtoolkit-0.1.5/src/tmgtoolkit/plotting.py`

 * *Files identical despite different names*

### Comparing `tmgtoolkit-0.1.4/src/tmgtoolkit/spm.py` & `tmgtoolkit-0.1.5/src/tmgtoolkit/spm.py`

 * *Files identical despite different names*

### Comparing `tmgtoolkit-0.1.4/src/tmgtoolkit/time_series.py` & `tmgtoolkit-0.1.5/src/tmgtoolkit/time_series.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,49 +68,53 @@
 
     Returns
     -------
     params : TmgParams
         A TmgParams namedtuple holding the computed TMG parameter values. The
         TmgParams namedtuple has the following fields:
         - `dm` (float): value of Dm, in the same units as `y`.
+        - `tm` (float): time of Dm, in the same units as `t`.
         - `td` (float): value of Td, in the same units as `t`.
         - `tc` (float): value of Tc, in the same units as `t`.
         - `ts` (float): value of Ts, in the same units as `t`.
         - `tr` (float): value of Tr, in the same units as `t`.
         Access fields with e.g. `params.dm` for value of `dm`.
     """
     if ignore_maxima_with_idx_less_than is None:
         ignore_maxima_with_idx_less_than = TimeSeriesConstants.TMG_PARAMS['ignore_maxima_with_idx_less_than']
     if ignore_maxima_less_than is None:
         ignore_maxima_less_than = TimeSeriesConstants.TMG_PARAMS['ignore_maxima_less_than']
 
-    dm_idx, dm, _ = _get_dm_idx_and_value(y, ignore_maxima_with_idx_less_than,
-                                          ignore_maxima_less_than,
-                                          use_first_max_as_dm, interpolate_dm)
+    dm_idx, dm, float_dm_idx = _get_dm_idx_and_value(y,
+                                                     ignore_maxima_with_idx_less_than,
+                                                     ignore_maxima_less_than,
+                                                     use_first_max_as_dm,
+                                                     interpolate_dm)
 
     t10_left_idx = _interpolate_idx_of_target_amplitude(y, 0.1*dm, True)
     t50_left_idx = _interpolate_idx_of_target_amplitude(y, 0.5*dm, True)
     t90_left_idx = _interpolate_idx_of_target_amplitude(y, 0.9*dm, True)
     t90_right_idx = _interpolate_idx_of_target_amplitude(y, 0.9*dm, False, start_search_at_idx=dm_idx)
     t50_right_idx = _interpolate_idx_of_target_amplitude(y, 0.5*dm, False, start_search_at_idx=dm_idx)
 
     # Convert indices to time
+    tm = _idx_to_time(float_dm_idx, t)
     t10_left = _idx_to_time(t10_left_idx, t)
     t50_left = _idx_to_time(t50_left_idx, t)
     t90_left = _idx_to_time(t90_left_idx, t)
     t90_right = _idx_to_time(t90_right_idx, t)
     t50_right = _idx_to_time(t50_right_idx, t)
 
     # Compute standard TMG time parameters
     td = t10_left
     tc = t90_left - t10_left
     ts = t50_right - t50_left
     tr = t50_right - t90_right
 
-    return NamedTupleTypes.TmgParams(dm=dm, td=td, tc=tc, ts=ts, tr=tr)
+    return NamedTupleTypes.TmgParams(dm=dm, tm=tm, td=td, tc=tc, ts=ts, tr=tr)
 
 
 def get_derivative_of_time_series(y, t=None):
     """Returns the derivative of a time series.
 
     Returns the derivative with respect to time of the inputted time series.
```

### Comparing `tmgtoolkit-0.1.4/src/tmgtoolkit/tmgio.py` & `tmgtoolkit-0.1.5/src/tmgtoolkit/tmgio.py`

 * *Files identical despite different names*

### Comparing `tmgtoolkit-0.1.4/src/tmgtoolkit.egg-info/PKG-INFO` & `tmgtoolkit-0.1.5/src/tmgtoolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmgtoolkit
-Version: 0.1.4
+Version: 0.1.5
 Summary: Time series analysis of tensiomyography (TMG) data
 Home-page: https://github.com/ejmastnak/tmgtoolkit
 Author: Elijan Mastnak
 Author-email: admin@ejmastnak.com
 Project-URL: Bug Tracker, https://github.com/ejmastnak/tmgtoolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tmgtoolkit-0.1.4/tests/test_split_data_for_spm.py` & `tmgtoolkit-0.1.5/tests/test_split_data_for_spm.py`

 * *Files identical despite different names*

