# Comparing `tmp/boxsers-1.5.0.tar.gz` & `tmp/boxsers-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boxsers-1.5.0.tar", last modified: Tue Apr 23 16:35:05 2024, max compression
+gzip compressed data, was "boxsers-1.5.1.tar", last modified: Fri May 31 13:35:22 2024, max compression
```

## Comparing `boxsers-1.5.0.tar` & `boxsers-1.5.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 16:35:05.392550 boxsers-1.5.0/
--rw-rw-rw-   0        0        0     1093 2021-08-13 16:59:11.000000 boxsers-1.5.0/LICENSE.txt
--rw-rw-rw-   0        0        0     8731 2024-04-23 16:35:05.391325 boxsers-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0    11442 2023-11-28 21:03:07.000000 boxsers-1.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 16:35:05.307386 boxsers-1.5.0/boxsers/
--rw-rw-rw-   0        0        0      775 2023-10-06 21:02:47.000000 boxsers-1.5.0/boxsers/__init__.py
--rw-rw-rw-   0        0        0      987 2022-07-15 15:44:15.000000 boxsers-1.5.0/boxsers/_boxsers_utils.py
--rw-rw-rw-   0        0        0    27673 2024-04-08 16:37:26.000000 boxsers-1.5.0/boxsers/data_augmentation.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:35:05.390411 boxsers-1.5.0/boxsers/machine_learning/
--rw-rw-rw-   0        0        0      380 2022-07-20 13:18:32.000000 boxsers-1.5.0/boxsers/machine_learning/__init__.py
--rw-rw-rw-   0        0        0    12773 2023-11-14 19:19:54.000000 boxsers-1.5.0/boxsers/machine_learning/classification.py
--rw-rw-rw-   0        0        0     7295 2022-07-13 19:35:31.000000 boxsers-1.5.0/boxsers/machine_learning/clustering.py
--rw-rw-rw-   0        0        0      180 2023-10-19 19:42:30.000000 boxsers-1.5.0/boxsers/machine_learning/deep_interpretability.py
--rw-rw-rw-   0        0        0    24227 2024-01-23 20:00:10.000000 boxsers-1.5.0/boxsers/machine_learning/dimension_reduction.py
--rw-rw-rw-   0        0        0    33878 2024-03-06 17:32:40.000000 boxsers-1.5.0/boxsers/machine_learning/neural_networks.py
--rw-rw-rw-   0        0        0     9399 2024-02-23 17:02:55.000000 boxsers-1.5.0/boxsers/machine_learning/validation_metrics.py
--rw-rw-rw-   0        0        0    11346 2024-03-06 18:00:45.000000 boxsers-1.5.0/boxsers/misc_tools.py
--rw-rw-rw-   0        0        0    17859 2024-04-23 16:28:45.000000 boxsers-1.5.0/boxsers/preprocessing.py
--rw-rw-rw-   0        0        0    18846 2024-01-24 17:00:34.000000 boxsers-1.5.0/boxsers/visual_tools.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:35:05.336614 boxsers-1.5.0/boxsers.egg-info/
--rw-rw-rw-   0        0        0     8731 2024-04-23 16:35:05.000000 boxsers-1.5.0/boxsers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      638 2024-04-23 16:35:05.000000 boxsers-1.5.0/boxsers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 16:35:05.000000 boxsers-1.5.0/boxsers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2024-04-23 16:35:05.000000 boxsers-1.5.0/boxsers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-23 16:35:05.000000 boxsers-1.5.0/boxsers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 16:35:05.392550 boxsers-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1096 2024-04-23 16:33:15.000000 boxsers-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:35:22.403271 boxsers-1.5.1/
+-rw-rw-rw-   0        0        0     1093 2021-08-13 16:59:11.000000 boxsers-1.5.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     8731 2024-05-31 13:35:22.403271 boxsers-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11442 2023-11-28 21:03:07.000000 boxsers-1.5.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 13:35:22.292950 boxsers-1.5.1/boxsers/
+-rw-rw-rw-   0        0        0      775 2023-10-06 21:02:47.000000 boxsers-1.5.1/boxsers/__init__.py
+-rw-rw-rw-   0        0        0      987 2022-07-15 15:44:15.000000 boxsers-1.5.1/boxsers/_boxsers_utils.py
+-rw-rw-rw-   0        0        0    27673 2024-04-08 16:37:26.000000 boxsers-1.5.1/boxsers/data_augmentation.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:35:22.403271 boxsers-1.5.1/boxsers/machine_learning/
+-rw-rw-rw-   0        0        0      380 2022-07-20 13:18:32.000000 boxsers-1.5.1/boxsers/machine_learning/__init__.py
+-rw-rw-rw-   0        0        0    12773 2023-11-14 19:19:54.000000 boxsers-1.5.1/boxsers/machine_learning/classification.py
+-rw-rw-rw-   0        0        0     7295 2022-07-13 19:35:31.000000 boxsers-1.5.1/boxsers/machine_learning/clustering.py
+-rw-rw-rw-   0        0        0      180 2023-10-19 19:42:30.000000 boxsers-1.5.1/boxsers/machine_learning/deep_interpretability.py
+-rw-rw-rw-   0        0        0    24227 2024-01-23 20:00:10.000000 boxsers-1.5.1/boxsers/machine_learning/dimension_reduction.py
+-rw-rw-rw-   0        0        0    33878 2024-03-06 17:32:40.000000 boxsers-1.5.1/boxsers/machine_learning/neural_networks.py
+-rw-rw-rw-   0        0        0     9399 2024-02-23 17:02:55.000000 boxsers-1.5.1/boxsers/machine_learning/validation_metrics.py
+-rw-rw-rw-   0        0        0    11346 2024-03-06 18:00:45.000000 boxsers-1.5.1/boxsers/misc_tools.py
+-rw-rw-rw-   0        0        0    20845 2024-05-01 16:30:33.000000 boxsers-1.5.1/boxsers/preprocessing.py
+-rw-rw-rw-   0        0        0    18846 2024-01-24 17:00:34.000000 boxsers-1.5.1/boxsers/visual_tools.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:35:22.324648 boxsers-1.5.1/boxsers.egg-info/
+-rw-rw-rw-   0        0        0     8731 2024-05-31 13:35:21.000000 boxsers-1.5.1/boxsers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2024-05-31 13:35:21.000000 boxsers-1.5.1/boxsers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 13:35:21.000000 boxsers-1.5.1/boxsers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2024-05-31 13:35:21.000000 boxsers-1.5.1/boxsers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-31 13:35:21.000000 boxsers-1.5.1/boxsers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 13:35:22.403271 boxsers-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1096 2024-05-31 13:35:17.000000 boxsers-1.5.1/setup.py
```

### Comparing `boxsers-1.5.0/LICENSE.txt` & `boxsers-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `boxsers-1.5.0/PKG-INFO` & `boxsers-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxsers
-Version: 1.5.0
+Version: 1.5.1
 Summary: Python package that provides a full range of functionality to process and analyze vibrational spectra (Raman, SERS, FTIR, etc.).
 Home-page: https://github.com/ALebrun-108/BoxSERS
 Author: Alexis Lebrun
 Author-email: alexis.lebrun.1@ulaval.ca
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `boxsers-1.5.0/README.md` & `boxsers-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `boxsers-1.5.0/boxsers/__init__.py` & `boxsers-1.5.1/boxsers/__init__.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.5.0/boxsers/_boxsers_utils.py` & `boxsers-1.5.1/boxsers/_boxsers_utils.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.5.0/boxsers/data_augmentation.py` & `boxsers-1.5.1/boxsers/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.5.0/boxsers/machine_learning/classification.py` & `boxsers-1.5.1/boxsers/machine_learning/classification.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.5.0/boxsers/machine_learning/clustering.py` & `boxsers-1.5.1/boxsers/machine_learning/clustering.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.5.0/boxsers/machine_learning/dimension_reduction.py` & `boxsers-1.5.1/boxsers/machine_learning/dimension_reduction.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.5.0/boxsers/machine_learning/neural_networks.py` & `boxsers-1.5.1/boxsers/machine_learning/neural_networks.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.5.0/boxsers/machine_learning/validation_metrics.py` & `boxsers-1.5.1/boxsers/machine_learning/validation_metrics.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.5.0/boxsers/misc_tools.py` & `boxsers-1.5.1/boxsers/misc_tools.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.5.0/boxsers/preprocessing.py` & `boxsers-1.5.1/boxsers/preprocessing.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,34 +109,72 @@
 
     if return_baseline:
         # returns the baseline signal if requested
         return sp - baseline, baseline
     return sp - baseline
 
 
-def _deprecated_cosmic_filter(sp, ks=3):
+def rollingball_baseline_cor(sp, window=40, smoothing_window=None, return_baseline=False):
     """
-    Apply a median filter to the spectrum(s) to remove cosmic rays.
+        Notes:
+            - Kneen, M. A.; Annegarn, H. J. Nuclear Instruments and Methods in Physics Research Section B: Beam
+              Interactions with Materials and Atoms 1996, 109–110, 209–213.
+
+        Parameters:
+            sp : array
+                Input Spectrum(s). Array shape = (n_spectra, n_pixels) for multiple spectra and (n_pixels,)
+                for a single spectrum.
 
-    Parameters:
-        sp : array
-            Input Spectrum(s). Array shape = (n_spectra, n_pixels) for multiple spectra and (n_pixels,)
-             for a single spectrum.
+            window : int, default=50
+                Half-width the window, or radius, of the rolling ball used to calculate the baseline.
 
-        ks : positive odd integer, default = 3
-            Size of the median filter window in pixel.
+            smoothing_window : int, default=None,
+                Half-width of the window used to smooth the baseline in the last step. If None, the rolling ball
+                window value is used as smoothing_window.
+
+            return_baseline : Boolean, default=False
+                If True, the function also returns the baseline array.
+
+        Returns:
+            (array) Baseline substracted spectrum(s). Array shape = (n_spectra, n_pixels) for multiple spectra
+                    and = (n_pixels,) for a single spectrum.
+
+            (array)(OPTIONAL) Baseline signal(s). Array shape = (n_spectra, n_pixels) for multiple spectra
+                    and = (n_pixels,) for a single spectrum.
+        """
+    if smoothing_window is None:
+        # if smoothing_window is None, the rolling ball window value is used as smoothing_window
+        smoothing_window = window
 
-    Returns:
-        (array) Filtered spectrum(s). Array shape = (n_spectra, n_pixels) for multiple spectra and (n_pixels,)
-                for a single spectrum.
-    """
-    sp = np.array(sp, ndmin=2)  # sp is forced to be a two-dimensional array
-    ks_1d = (1, ks)
-    sp_med = medfilt(sp, ks_1d)  # from scipy
-    return sp_med
+    # sp is forced to be a two-dimensional array
+    sp = np.array(sp, ndmin=2)
+    n_spectra, sp_length = sp.shape  # number of spectra, spectrum length
+
+    # initialization and space allocation
+    baseline = np.zeros_like(sp)
+    loc_minima = np.zeros_like(sp)
+    loc_maxima = np.zeros_like(sp)
+
+    for i in np.arange(sp_length):
+        i_start = max(0, i - window)  # first index of the rolling ball, 0 if i-window < 0
+        i_end = min(sp_length, i + window + 1)  # last index of the rolling ball, sp_length if i+window+1 > sp_length
+        loc_minima[:, i] = np.min(sp[:, i_start:i_end], axis=1)  # measures local minima
+    for i in np.arange(sp_length):
+        i_start = max(0, i - window)
+        i_end = min(sp_length, i + window + 1)
+        loc_maxima[:, i] = np.max(loc_minima[:, i_start:i_end], axis=1)  # measures local maxima from minima
+    for i in np.arange(sp_length):
+        i_start = max(0, i - smoothing_window)
+        i_end = min(sp_length, i + smoothing_window + 1)
+        baseline[:, i] = np.mean(loc_maxima[:, i_start:i_end], axis=1)  # Average smoothing of local maxima
+
+    if return_baseline:
+        # returns the baseline signal if requested
+        return sp - baseline, baseline
+    return sp - baseline
 
 
 def cosmic_filter(sp, width=3, threshold=11.0):
     """
     Suppresses cosmic rays using a sliding window that compares each portion of each spectrum with the other spectra.
 
     Notes:
@@ -411,9 +449,35 @@
         new_sp = np.delete(new_sp, error_ind, 0)
         print('Some spectra raised errors and were removed')
         print('Erroneous spectrum indexes are identified by the second output of this function.')
         print('Delete the corresponding label with this command: new_label = np.delete(label, erroneous_index)')
     return new_sp, error_ind
 
 
+def _deprecated_cosmic_filter(sp, ks=3):
+    """
+    Apply a median filter to the spectrum(s) to remove cosmic rays.
+
+    Note:
+        - Former and deprecated version of the cosmic_filter function. It is likely to be removed in
+          subsequent BoxSERS versions.
+
+    Parameters:
+        sp : array
+            Input Spectrum(s). Array shape = (n_spectra, n_pixels) for multiple spectra and (n_pixels,)
+             for a single spectrum.
+
+        ks : positive odd integer, default = 3
+            Size of the median filter window in pixel.
+
+    Returns:
+        (array) Filtered spectrum(s). Array shape = (n_spectra, n_pixels) for multiple spectra and (n_pixels,)
+                for a single spectrum.
+    """
+    sp = np.array(sp, ndmin=2)  # sp is forced to be a two-dimensional array
+    ks_1d = (1, ks)
+    sp_med = medfilt(sp, ks_1d)  # from scipy
+    return sp_med
+
+
 if __name__ == "__main__":
     help(__name__)
```

### Comparing `boxsers-1.5.0/boxsers/visual_tools.py` & `boxsers-1.5.1/boxsers/visual_tools.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.5.0/boxsers.egg-info/PKG-INFO` & `boxsers-1.5.1/boxsers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxsers
-Version: 1.5.0
+Version: 1.5.1
 Summary: Python package that provides a full range of functionality to process and analyze vibrational spectra (Raman, SERS, FTIR, etc.).
 Home-page: https://github.com/ALebrun-108/BoxSERS
 Author: Alexis Lebrun
 Author-email: alexis.lebrun.1@ulaval.ca
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `boxsers-1.5.0/boxsers.egg-info/SOURCES.txt` & `boxsers-1.5.1/boxsers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boxsers-1.5.0/setup.py` & `boxsers-1.5.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     author='Alexis Lebrun',
     author_email='alexis.lebrun.1@ulaval.ca',
     # dependencies
     install_requires=['numpy', 'pandas', 'matplotlib', 'seaborn', 'scipy', 'scikit-learn', 'tensorflow',
                       'tables', 'scikit-image'],
     python_requires='>=3.6',
     # *strongly* suggested for sharing
-    version='1.5.0',
+    version='1.5.1',
     # The license can be anything you like
     license='MIT',
     description='Python package that provides a full range of functionality to process and analyze vibrational'
                 ' spectra (Raman, SERS, FTIR, etc.).',
     # We will also need a readme eventually (there will be a warning)
     long_description=open('README_pypi.md').read(),
     long_description_content_type="text/markdown",
```

