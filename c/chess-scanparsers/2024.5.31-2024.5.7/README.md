# Comparing `tmp/chess_scanparsers-2024.5.31.tar.gz` & `tmp/chess_scanparsers-2024.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess_scanparsers-2024.5.31.tar", last modified: Fri May 31 20:32:52 2024, max compression
+gzip compressed data, was "chess_scanparsers-2024.5.7.tar", last modified: Tue May  7 15:00:50 2024, max compression
```

## Comparing `chess_scanparsers-2024.5.31.tar` & `chess_scanparsers-2024.5.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:32:52.233384 chess_scanparsers-2024.5.31/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-31 20:32:52.229384 chess_scanparsers-2024.5.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-31 20:32:46.000000 chess_scanparsers-2024.5.31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:32:52.229384 chess_scanparsers-2024.5.31/chess_scanparsers/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-31 20:32:50.000000 chess_scanparsers-2024.5.31/chess_scanparsers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    53757 2024-05-31 20:32:46.000000 chess_scanparsers-2024.5.31/chess_scanparsers/scanparsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:32:52.229384 chess_scanparsers-2024.5.31/chess_scanparsers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-31 20:32:52.000000 chess_scanparsers-2024.5.31/chess_scanparsers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-31 20:32:52.000000 chess_scanparsers-2024.5.31/chess_scanparsers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:32:52.000000 chess_scanparsers-2024.5.31/chess_scanparsers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-31 20:32:52.000000 chess_scanparsers-2024.5.31/chess_scanparsers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-31 20:32:52.000000 chess_scanparsers-2024.5.31/chess_scanparsers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:32:52.233384 chess_scanparsers-2024.5.31/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1130 2024-05-31 20:32:50.000000 chess_scanparsers-2024.5.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:50.100520 chess_scanparsers-2024.5.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-07 15:00:50.096520 chess_scanparsers-2024.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:44.000000 chess_scanparsers-2024.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:50.096520 chess_scanparsers-2024.5.7/chess-scanparsers/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 15:00:48.000000 chess_scanparsers-2024.5.7/chess-scanparsers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57963 2024-05-07 15:00:44.000000 chess_scanparsers-2024.5.7/chess-scanparsers/scanparsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:50.096520 chess_scanparsers-2024.5.7/chess_scanparsers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-07 15:00:50.000000 chess_scanparsers-2024.5.7/chess_scanparsers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-07 15:00:50.000000 chess_scanparsers-2024.5.7/chess_scanparsers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 15:00:50.000000 chess_scanparsers-2024.5.7/chess_scanparsers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-07 15:00:50.000000 chess_scanparsers-2024.5.7/chess_scanparsers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 15:00:50.000000 chess_scanparsers-2024.5.7/chess_scanparsers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 15:00:50.100520 chess_scanparsers-2024.5.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1130 2024-05-07 15:00:48.000000 chess_scanparsers-2024.5.7/setup.py
```

### Comparing `chess_scanparsers-2024.5.31/chess_scanparsers/scanparsers.py` & `chess_scanparsers-2024.5.7/chess-scanparsers/scanparsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/Abin/env python3
+#!/usr/bin/env python3
 
 # -*- coding: utf-8 -*-
 
 """Parsing data from certain CHESS SPEC scans is supported by a family
 of classes derived from the base class, `ScanParser` (defined
 below). An instance of `ScanParser` represents a single SPEC scan --
 each instance is initialized with the name of a specific spec file and
@@ -479,14 +479,105 @@
         macro for this scan. If there is more than one motor scanned
         (in a "flymesh" scan, for example), the order of motors in the
         returned tuple will go from the fastest moving motor first to
         the slowest moving motor last.
 
         :rtype: tuple
         """
+        raise NotImplementedError
+
+    def get_spec_scan_motor_vals(self):
+        """Return the values visited by each of the scanned motors. If
+        there is more than one motor scanned (in a "flymesh" scan, for
+        example), the order of motor values in the returned tuple will
+        go from the fastest moving motor's values first to the slowest
+        moving motor's values last.
+
+        :rtype: tuple
+        """
+        raise NotImplementedError
+
+    def get_spec_scan_shape(self):
+        """Return the number of points visited by each of the scanned
+        motors. If there is more than one motor scanned (in a
+        "flymesh" scan, for example), the order of number of motor
+        values in the returned tuple will go from the number of points
+        visited by the fastest moving motor first to the the number of
+        points visited by the slowest moving motor last.
+
+        :rtype: tuple
+        """
+        raise NotImplementedError
+
+    def get_spec_scan_dwell(self):
+        """Return the dwell time for each point in the scan as it
+        appears in the command string.
+
+        :rtype: float
+        """
+        raise NotImplementedError
+
+    def get_spec_scan_npts(self):
+        """Return the number of points collected in this SPEC scan.
+
+        :rtype: int
+        """
+        return np.prod(self.spec_scan_shape)
+
+    def get_scan_step(self, scan_step_index:int):
+        """Return the index of each motor coordinate corresponding to
+        the index of a single point in the scan. If there is more than
+        one motor scanned (in a "flymesh" scan, for example), the
+        order of indices in the returned tuple will go from the index
+        of the value of the fastest moving motor first to the index of
+        the value of the slowest moving motor last.
+
+        :param scan_step_index: the index of a single point in the
+            scan.
+        :type scan_step_index: int
+        :rtype: tuple
+        """
+        scan_steps = np.ndindex(self.spec_scan_shape[::-1])
+        i = 0
+        while i <= scan_step_index:
+            scan_step = next(scan_steps)
+            i += 1
+        return scan_step
+
+    def get_scan_step_index(self, scan_step:tuple):
+        """Return the index of a single scan point corresponding to a
+        tuple of indices for each scanned motor coordinate.
+
+        :param scan_step: a tuple of the indices of each scanned motor
+            coordinate. If there is more than one motor scanned (in a
+            "flymesh" scan, for example), the order of indices should
+            go from the index of the value of the fastest moving motor
+            first to the index of the value of the slowest moving
+            motor last.
+        :type scan_step: tuple
+        :trype: int
+        """
+        scan_steps = np.ndindex(self.spec_scan_shape[::-1])
+        scan_step_found = False
+        scan_step_index = -1
+        while not scan_step_found:
+            next_scan_step = next(scan_steps)
+            scan_step_index += 1
+            if next_scan_step == scan_step:
+                scan_step_found = True
+                break
+        return scan_step_index
+
+
+class FMBLinearScanParser(LinearScanParser, FMBScanParser):
+    """Partial implementation of a class representing a typical line
+    or mesh scan in SPEC collected at FMB.
+    """
+
+    def get_spec_scan_motor_mnes(self):
         if self.spec_macro in ('flymesh', 'mesh', 'flydmesh', 'dmesh'):
             m1_mne = self.spec_args[0]
             try:
                 # Try post-summer-2022 format
                 dwell = float(self.spec_args[4])
             except:
                 # Accommodate pre-summer-2022 format
@@ -499,23 +590,15 @@
             return (self.spec_args[0],)
         if self.spec_macro in ('tseries', 'loopscan'):
             return ('Time',)
         raise RuntimeError(f'{self.scan_title}: cannot determine scan motors '
                            f'for scans of type {self.spec_macro}')
 
     def get_spec_scan_motor_vals(self):
-        """Return the values visited by each of the scanned motors. If
-        there is more than one motor scanned (in a "flymesh" scan, for
-        example), the order of motor values in the returned tuple will
-        go from the fastest moving motor's values first to the slowest
-        moving motor's values last.
-
-        :rtype: tuple
-        """
-        if self.spec_macro in ('flymesh', 'mesh'):
+        if self.spec_macro in ('flymesh', 'mesh', 'flydmesh', 'dmesh'):
             m1_start = float(self.spec_args[1])
             m1_end = float(self.spec_args[2])
             m1_npt = int(self.spec_args[3]) + 1
             try:
                 # Try post-summer-2022 format
                 dwell = float(self.spec_args[4])
             except:
@@ -540,24 +623,15 @@
             return (mot_vals,)
         if self.spec_macro in ('tseries', 'loopscan'):
             return (self.spec_scan.data[:,0],)
         raise RuntimeError(f'{self.scan_title}: cannot determine scan motors '
                            f'for scans of type {self.spec_macro}')
 
     def get_spec_scan_shape(self):
-        """Return the number of points visited by each of the scanned
-        motors. If there is more than one motor scanned (in a
-        "flymesh" scan, for example), the order of number of motor
-        values in the returned tuple will go from the number of points
-        visited by the fastest moving motor first to the the number of
-        points visited by the slowest moving motor last.
-
-        :rtype: tuple
-        """
-        if self.spec_macro in ('flymesh', 'mesh'):
+        if self.spec_macro in ('flymesh', 'mesh', 'flydmesh', 'dmesh'):
             fast_mot_npts = int(self.spec_args[3]) + 1
             try:
                 # Try post-summer-2022 format
                 dwell = float(self.spec_args[4])
             except:
                 # Accommodate pre-summer-2022 format
                 m2_nint_i = 7
@@ -570,86 +644,32 @@
             return (mot_npts,)
         if self.spec_macro in ('tseries', 'loopscan'):
             return (len(np.array(self.spec_scan.data[:,0])),)
         raise RuntimeError(f'{self.scan_title}: cannot determine scan shape '
                            f'for scans of type {self.spec_macro}')
 
     def get_spec_scan_dwell(self):
-        """Return the dwell time for each point in the scan as it
-        appears in the command string.
-
-        :rtype: float
-        """
         if self.macro in ('flymesh', 'mesh', 'flydmesh', 'dmesh'):
             try:
                 # Try post-summer-2022 format
                 dwell = float(self.spec_args[4])
             except:
                 # Accommodate pre-summer-2022 format
                 dwell = float(self.spec_args[8])
             return dwell
         if self.spec_macro in ('flyscan', 'ascan'):
             return float(self.spec_args[4])
         if self.spec_macro in ('tseries', 'loopscan'):
             return float(self.spec_args[1])
-        if self.spec_macro in ('wbslew_scan'):
-            return float(self.spec_args[3])
         raise RuntimeError(f'{self.scan_title}: cannot determine dwell for '
                            f'scans of type {self.spec_macro}')
 
-    def get_spec_scan_npts(self):
-        """Return the number of points collected in this SPEC scan.
-
-        :rtype: int
-        """
-        return np.prod(self.spec_scan_shape)
-
-    def get_scan_step(self, scan_step_index:int):
-        """Return the index of each motor coordinate corresponding to
-        the index of a single point in the scan. If there is more than
-        one motor scanned (in a "flymesh" scan, for example), the
-        order of indices in the returned tuple will go from the index
-        of the value of the fastest moving motor first to the index of
-        the value of the slowest moving motor last.
-
-        :param scan_step_index: the index of a single point in the
-            scan.
-        :type scan_step_index: int
-        :rtype: tuple
-        """
-        scan_steps = np.ndindex(self.spec_scan_shape[::-1])
-        i = 0
-        while i <= scan_step_index:
-            scan_step = next(scan_steps)
-            i += 1
-        return scan_step
-
-    def get_scan_step_index(self, scan_step:tuple):
-        """Return the index of a single scan point corresponding to a
-        tuple of indices for each scanned motor coordinate.
+    def get_detector_data_path(self):
+        return os.path.join(self.scan_path, self.scan_title)
 
-        :param scan_step: a tuple of the indices of each scanned motor
-            coordinate. If there is more than one motor scanned (in a
-            "flymesh" scan, for example), the order of indices should
-            go from the index of the value of the fastest moving motor
-            first to the index of the value of the slowest moving
-            motor last.
-        :type scan_step: tuple
-        :trype: int
-        """
-        scan_steps = np.ndindex(self.spec_scan_shape[::-1])
-        scan_step_found = False
-        scan_step_index = -1
-        while not scan_step_found:
-            next_scan_step = next(scan_steps)
-            scan_step_index += 1
-            if next_scan_step == scan_step:
-                scan_step_found = True
-                break
-        return scan_step_index
 
 
 @cache
 def list_fmb_saxswaxs_detector_files(detector_data_path, detector_prefix):
     """Return a sorted list of all data files for the given detector
     in the given directory. This function is cached to improve
     performace for carrying our full FAMB SAXS/WAXS data-processing
@@ -662,28 +682,24 @@
     :type detector_prefix: str
     :return: list of detector filenames
     :rtype: list[str]
     """
     return sorted(
         [f for f in os.listdir(detector_data_path)
         if detector_prefix in f
-        and not f.endswith('.log')
-        and not f.endswith('_master.h5')])
+        and not f.endswith('.log')])
 
-class FMBSAXSWAXSScanParser(LinearScanParser, FMBScanParser):
+class FMBSAXSWAXSScanParser(FMBLinearScanParser):
     """Concrete implementation of a class representing a scan taken
     with the typical SAXS/WAXS setup at FMB.
     """
 
     def get_scan_title(self):
         return f'{self.scan_name}_{self.scan_number:03d}'
 
-    def get_detector_data_path(self):
-        return os.path.join(self.scan_path, self.scan_title)
-
     def get_detector_data_file(self, detector_prefix, scan_step_index:int):
         detector_files = list_fmb_saxswaxs_detector_files(
             self.detector_data_path, detector_prefix)
         if len(detector_files) == self.spec_scan_npts:
             return os.path.join(
                 self.detector_data_path, detector_files[scan_step_index])
         else:
@@ -704,25 +720,22 @@
         image_file = self.get_detector_data_file(detector_prefix,
                                                  scan_step_index)
         with fabio.open(image_file) as det_file:
             image_data = det_file.data
         return image_data
 
 
-class FMBXRFScanParser(LinearScanParser, FMBScanParser):
+class FMBXRFScanParser(FMBLinearScanParser):
     """Concrete implementation of a class representing a scan taken
     with the typical XRF setup at FMB.
     """
 
     def get_scan_title(self):
         return f'{self.scan_name}_scan{self.scan_number}'
 
-    def get_detector_data_path(self):
-        return os.path.join(self.scan_path, self.scan_title)
-
     def get_detector_data_file(self, detector_prefix, scan_step_index:int):
         scan_step = self.get_scan_step(scan_step_index)
         file_name = f'scan{self.scan_number}_{scan_step[0]:03d}.hdf5'
         file_name_full = os.path.join(self.detector_data_path, file_name)
         if os.path.isfile(file_name_full):
             return file_name_full
         raise RuntimeError(f'{self.scan_title}: could not find detector image '
@@ -742,14 +755,107 @@
         return detector_data
 
 
 class SMBLinearScanParser(LinearScanParser, SMBScanParser):
     """Concrete implementation of a class representing a scan taken
     with the typical powder diffraction setup at SMB.
     """
+
+    def get_spec_scan_dwell(self):
+        if self.spec_macro in ('flymesh', 'mesh'):
+            try:
+                # Try post-summer-2022 format
+                dwell = float(self.spec_args[4])
+            except:
+                # Accommodate pre-summer-2022 format
+                dwell = float(self.spec_args[8])
+            return dwell
+        if self.spec_macro in ('flyscan', 'ascan'):
+            return float(self.spec_args[4])
+        if self.spec_macro == 'tseries':
+            return float(self.spec_args[1])
+        if self.spec_macro == 'wbslew_scan':
+            return float(self.spec_args[3])
+        raise RuntimeError(f'{self.scan_title}: cannot determine dwell time '
+                           f'for scans of type {self.spec_macro}')
+
+    def get_spec_scan_motor_mnes(self):
+        if self.spec_macro in ('flymesh', 'mesh'):
+            m1_mne = self.spec_args[0]
+            try:
+                # Try post-summer-2022 format
+                dwell = float(self.spec_args[4])
+            except:
+                # Accommodate pre-summer-2022 format
+                m2_mne_i = 4
+            else:
+                m2_mne_i = 5
+            m2_mne = self.spec_args[m2_mne_i]
+            return (m1_mne, m2_mne)
+        if self.spec_macro in ('flyscan', 'ascan'):
+            return (self.spec_args[0],)
+        if self.spec_macro in ('tseries', 'loopscan'):
+            return ('Time',)
+        raise RuntimeError(f'{self.scan_title}: cannot determine scan motors '
+                           f'for scans of type {self.spec_macro}')
+
+    def get_spec_scan_motor_vals(self):
+        if self.spec_macro in ('flymesh', 'mesh'):
+            m1_start = float(self.spec_args[1])
+            m1_end = float(self.spec_args[2])
+            m1_npt = int(self.spec_args[3]) + 1
+            try:
+                # Try post-summer-2022 format
+                dwell = float(self.spec_args[4])
+            except:
+                # Accommodate pre-summer-2022 format
+                m2_start_i = 5
+                m2_end_i = 6
+                m2_nint_i = 7
+            else:
+                m2_start_i = 6
+                m2_end_i = 7
+                m2_nint_i = 8
+            m2_start = float(self.spec_args[m2_start_i])
+            m2_end = float(self.spec_args[m2_end_i])
+            m2_npt = int(self.spec_args[m2_nint_i]) + 1
+            fast_mot_vals = np.linspace(m1_start, m1_end, m1_npt)
+            slow_mot_vals = np.linspace(m2_start, m2_end, m2_npt)
+            return (fast_mot_vals, slow_mot_vals)
+        if self.spec_macro in ('flyscan', 'ascan'):
+            mot_vals = np.linspace(float(self.spec_args[1]),
+                                   float(self.spec_args[2]),
+                                   int(self.spec_args[3])+1)
+            return (mot_vals,)
+        if self.spec_macro in ('tseries', 'loopscan'):
+            return (self.spec_scan.data[:,0],)
+        raise RuntimeError(f'{self.scan_title}: cannot determine scan motors '
+                           f'for scans of type {self.spec_macro}')
+
+    def get_spec_scan_shape(self):
+        if self.spec_macro in ('flymesh', 'mesh'):
+            fast_mot_npts = int(self.spec_args[3]) + 1
+            try:
+                # Try post-summer-2022 format
+                dwell = float(self.spec_args[4])
+            except:
+                # Accommodate pre-summer-2022 format
+                m2_nint_i = 7
+            else:
+                m2_nint_i = 8
+            slow_mot_npts = int(self.spec_args[m2_nint_i]) + 1
+            return (fast_mot_npts, slow_mot_npts)
+        if self.spec_macro in ('flyscan', 'ascan'):
+            mot_npts = int(self.spec_args[3])+1
+            return (mot_npts,)
+        if self.spec_macro in ('tseries', 'loopscan'):
+            return (len(np.array(self.spec_scan.data[:,0])),)
+        raise RuntimeError(f'{self.scan_title}: cannot determine scan shape '
+                           f'for scans of type {self.spec_macro}')
+
     def get_detector_data_path(self):
         return os.path.join(self.scan_path, str(self.scan_number))
 
     def get_detector_data_file(self, detector_prefix, scan_step_index:int):
         scan_step = self.get_scan_step(scan_step_index)
         if len(scan_step) == 1:
             scan_step = (0, *scan_step)
```

### Comparing `chess_scanparsers-2024.5.31/setup.py` & `chess_scanparsers-2024.5.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,31 +8,31 @@
 to run tests : python setup.py test
 """
 
 import os
 import setuptools
 
 # [set version]
-version = 'v2024.05.31'
+version = 'v2024.05.07'
 # [version set]
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name='chess_scanparsers',
+    name='chess-scanparsers',
     version=version,
     author='Keara Soloway, Rolf Verberg',
     author_email='',
     description='Utilities for parsing data and metadata for CHESS scans.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/CHESSComputing/chess-scanparsers',
-    packages=['chess_scanparsers'],
-    package_dir={'chess_scanparsers': 'chess_scanparsers'},
+    packages=['chess-scanparsers'],
+    package_dir={'chess-scanparsers': 'chess-scanparsers'},
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.8',
     install_requires=[
```

