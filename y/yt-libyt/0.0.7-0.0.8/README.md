# Comparing `tmp/yt_libyt-0.0.7.tar.gz` & `tmp/yt_libyt-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_libyt-0.0.7.tar", last modified: Mon Feb 19 05:15:34 2024, max compression
+gzip compressed data, was "yt_libyt-0.0.8.tar", last modified: Fri May 31 00:40:20 2024, max compression
```

## Comparing `yt_libyt-0.0.7.tar` & `yt_libyt-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 cindytsai  (1001) cindytsai  (1001)        0 2024-02-19 05:15:34.170888 yt_libyt-0.0.7/
--rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)      138 2023-11-09 02:41:13.000000 yt_libyt-0.0.7/AUTHORS.md
--rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)     2488 2023-11-08 21:08:31.000000 yt_libyt-0.0.7/CONTRIBUTING.md
--rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)     1537 2023-11-08 15:44:41.000000 yt_libyt-0.0.7/LICENSE
--rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)      241 2023-11-08 19:53:44.000000 yt_libyt-0.0.7/MANIFEST.in
--rw-r--r--   0 cindytsai  (1001) cindytsai  (1001)     2759 2024-02-19 05:15:34.170888 yt_libyt-0.0.7/PKG-INFO
--rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)      276 2024-02-19 05:12:46.000000 yt_libyt-0.0.7/README.md
--rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)     1212 2024-02-19 02:47:26.000000 yt_libyt-0.0.7/pyproject.toml
--rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)     1228 2024-02-19 05:15:34.170888 yt_libyt-0.0.7/setup.cfg
-drwxrwxr-x   0 cindytsai  (1001) cindytsai  (1001)        0 2024-02-19 05:15:34.166888 yt_libyt-0.0.7/tests/
--rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)      376 2023-11-06 16:26:57.000000 yt_libyt-0.0.7/tests/test_import.py
-drwxrwxr-x   0 cindytsai  (1001) cindytsai  (1001)        0 2024-02-19 05:15:34.170888 yt_libyt-0.0.7/yt_libyt/
--rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)      592 2023-11-08 22:01:33.000000 yt_libyt-0.0.7/yt_libyt/__init__.py
--rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)       22 2024-02-19 05:15:22.000000 yt_libyt-0.0.7/yt_libyt/_version.py
--rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)      565 2023-11-06 16:18:08.000000 yt_libyt-0.0.7/yt_libyt/api.py
--rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)    14558 2024-02-19 03:05:52.000000 yt_libyt-0.0.7/yt_libyt/data_structures.py
--rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)        0 2023-05-08 18:58:47.000000 yt_libyt-0.0.7/yt_libyt/definitions.py
--rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)     1037 2023-11-06 02:42:25.000000 yt_libyt-0.0.7/yt_libyt/fields.py
--rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)    22632 2023-11-06 16:26:57.000000 yt_libyt-0.0.7/yt_libyt/io.py
--rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)        0 2023-05-08 18:58:47.000000 yt_libyt-0.0.7/yt_libyt/misc.py
--rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)        0 2023-11-03 17:26:54.000000 yt_libyt-0.0.7/yt_libyt/py.typed
-drwxrwxr-x   0 cindytsai  (1001) cindytsai  (1001)        0 2024-02-19 05:15:34.170888 yt_libyt-0.0.7/yt_libyt.egg-info/
--rw-r--r--   0 cindytsai  (1001) cindytsai  (1001)     2759 2024-02-19 05:15:34.000000 yt_libyt-0.0.7/yt_libyt.egg-info/PKG-INFO
--rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)      471 2024-02-19 05:15:34.000000 yt_libyt-0.0.7/yt_libyt.egg-info/SOURCES.txt
--rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)        1 2024-02-19 05:15:34.000000 yt_libyt-0.0.7/yt_libyt.egg-info/dependency_links.txt
--rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)        1 2023-11-08 20:39:31.000000 yt_libyt-0.0.7/yt_libyt.egg-info/not-zip-safe
--rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)        3 2024-02-19 05:15:34.000000 yt_libyt-0.0.7/yt_libyt.egg-info/requires.txt
--rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)        9 2024-02-19 05:15:34.000000 yt_libyt-0.0.7/yt_libyt.egg-info/top_level.txt
+drwxrwxr-x   0 cindytsai  (1001) cindytsai  (1001)        0 2024-05-31 00:40:20.616630 yt_libyt-0.0.8/
+-rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)      138 2023-11-09 02:41:13.000000 yt_libyt-0.0.8/AUTHORS.md
+-rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)     2488 2023-11-08 21:08:31.000000 yt_libyt-0.0.8/CONTRIBUTING.md
+-rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)     1537 2023-11-08 15:44:41.000000 yt_libyt-0.0.8/LICENSE
+-rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)      241 2023-11-08 19:53:44.000000 yt_libyt-0.0.8/MANIFEST.in
+-rw-r--r--   0 cindytsai  (1001) cindytsai  (1001)     2944 2024-05-31 00:40:20.616630 yt_libyt-0.0.8/PKG-INFO
+-rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)      461 2024-05-30 04:03:36.000000 yt_libyt-0.0.8/README.md
+-rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)     1212 2024-02-19 02:47:26.000000 yt_libyt-0.0.8/pyproject.toml
+-rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)     1228 2024-05-31 00:40:20.616630 yt_libyt-0.0.8/setup.cfg
+drwxrwxr-x   0 cindytsai  (1001) cindytsai  (1001)        0 2024-05-31 00:40:20.616630 yt_libyt-0.0.8/tests/
+-rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)      376 2023-11-06 16:26:57.000000 yt_libyt-0.0.8/tests/test_import.py
+drwxrwxr-x   0 cindytsai  (1001) cindytsai  (1001)        0 2024-05-31 00:40:20.616630 yt_libyt-0.0.8/yt_libyt/
+-rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)      592 2023-11-08 22:01:33.000000 yt_libyt-0.0.8/yt_libyt/__init__.py
+-rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)       22 2024-05-30 04:03:47.000000 yt_libyt-0.0.8/yt_libyt/_version.py
+-rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)      565 2023-11-06 16:18:08.000000 yt_libyt-0.0.8/yt_libyt/api.py
+-rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)    14684 2024-05-18 17:37:53.000000 yt_libyt-0.0.8/yt_libyt/data_structures.py
+-rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)        0 2023-05-08 18:58:47.000000 yt_libyt-0.0.8/yt_libyt/definitions.py
+-rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)     1037 2023-11-06 02:42:25.000000 yt_libyt-0.0.8/yt_libyt/fields.py
+-rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)    23031 2024-05-30 04:03:23.000000 yt_libyt-0.0.8/yt_libyt/io.py
+-rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)        0 2023-05-08 18:58:47.000000 yt_libyt-0.0.8/yt_libyt/misc.py
+-rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)        0 2023-11-03 17:26:54.000000 yt_libyt-0.0.8/yt_libyt/py.typed
+drwxrwxr-x   0 cindytsai  (1001) cindytsai  (1001)        0 2024-05-31 00:40:20.616630 yt_libyt-0.0.8/yt_libyt.egg-info/
+-rw-r--r--   0 cindytsai  (1001) cindytsai  (1001)     2944 2024-05-31 00:40:20.000000 yt_libyt-0.0.8/yt_libyt.egg-info/PKG-INFO
+-rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)      471 2024-05-31 00:40:20.000000 yt_libyt-0.0.8/yt_libyt.egg-info/SOURCES.txt
+-rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)        1 2024-05-31 00:40:20.000000 yt_libyt-0.0.8/yt_libyt.egg-info/dependency_links.txt
+-rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)        1 2023-11-08 20:39:31.000000 yt_libyt-0.0.8/yt_libyt.egg-info/not-zip-safe
+-rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)        3 2024-05-31 00:40:20.000000 yt_libyt-0.0.8/yt_libyt.egg-info/requires.txt
+-rw-rw-r--   0 cindytsai  (1001) cindytsai  (1001)        9 2024-05-31 00:40:20.000000 yt_libyt-0.0.8/yt_libyt.egg-info/top_level.txt
```

### Comparing `yt_libyt-0.0.7/CONTRIBUTING.md` & `yt_libyt-0.0.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `yt_libyt-0.0.7/LICENSE` & `yt_libyt-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yt_libyt-0.0.7/PKG-INFO` & `yt_libyt-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt_libyt
-Version: 0.0.7
+Version: 0.0.8
 Summary: A yt frontend for libyt
 Author-email: Shin-Rong Tsai <turquoisea.tsai@gmail.com>, Hsi-Yu Schive <hyschive@gmail.com>, Matthew Turk <matthewturk@gmail.com>
 License: 
         
         BSD License
         
         Copyright (c) 2023, Shin-Rong Tsai, Hsi-Yu Schive, Matthew Turk
@@ -54,7 +54,21 @@
 
 This is a [`yt`](https://yt-project.org/) frontend for [`libyt`](https://github.com/yt-project/libyt).
 
 
 * **yt**: https://yt-project.org/
 * **libyt Repo**: https://github.com/yt-project/libyt
 * **libyt Doc**: https://libyt.readthedocs.io/en/latest/
+
+
+### Install
+
+- From PyPI:
+  ```bash
+  pip install yt-libyt
+  ```
+- From source:
+  ```bash
+  git clone https://github.com/data-exp-lab/yt_libyt.git
+  cd yt_libyt
+  pip install .
+  ```
```

### Comparing `yt_libyt-0.0.7/pyproject.toml` & `yt_libyt-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yt_libyt-0.0.7/setup.cfg` & `yt_libyt-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `yt_libyt-0.0.7/yt_libyt/__init__.py` & `yt_libyt-0.0.8/yt_libyt/__init__.py`

 * *Files identical despite different names*

### Comparing `yt_libyt-0.0.7/yt_libyt/api.py` & `yt_libyt-0.0.8/yt_libyt/api.py`

 * *Files identical despite different names*

### Comparing `yt_libyt-0.0.7/yt_libyt/data_structures.py` & `yt_libyt-0.0.8/yt_libyt/data_structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     def __repr__(self):
         return "libytGrid_%09i (dimension = %s)" % (self.id, self.ActiveDimensions)
 
 
 class libytHierarchy(GridIndex):
     grid = libytGrid
     libyt = None
+
     # _preload_implemented = True # Not sure about this option
 
     def __init__(self, ds, dataset_type="libyt"):
         self.dataset_type = dataset_type
         self.dataset = weakref.proxy(ds)
         self.directory = os.getcwd()
         self.float_type = "float64"
@@ -270,14 +271,17 @@
         # currently libyt assumes cgs
         setdefaultattr(self, "length_unit", self.quan(self.libyt.param_yt["length_unit"], "cm"))
         setdefaultattr(self, "mass_unit", self.quan(self.libyt.param_yt["mass_unit"], "g"))
         setdefaultattr(self, "time_unit", self.quan(self.libyt.param_yt["time_unit"], "s"))
         setdefaultattr(
             self, "magnetic_unit", self.quan(self.libyt.param_yt["magnetic_unit"], "gauss")
         )
+        setdefaultattr(
+            self, "velocity_unit", self.quan(self.libyt.param_yt["velocity_unit"], "cm/s")
+        )
 
     def _parse_parameter_file(self):
         # dataset identifier
         self.unique_identifier = time.time()
 
         # user-specific parameters
         self.parameters.update(self.libyt.param_user)
```

### Comparing `yt_libyt-0.0.7/yt_libyt/fields.py` & `yt_libyt-0.0.8/yt_libyt/fields.py`

 * *Files identical despite different names*

### Comparing `yt_libyt-0.0.7/yt_libyt/io.py` & `yt_libyt-0.0.8/yt_libyt/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,20 +285,33 @@
                         )
                     offset += g.select(selector, data_view, rv[field], offset)
             assert offset == size
         return rv
 
     @staticmethod
     def _get_my_rank():
-        from mpi4py import MPI
+        import libyt
 
-        comm = MPI.COMM_WORLD
-        return comm.Get_rank()
+        if libyt.libyt_info["SERIAL_MODE"] is False:
+            try:
+                from mpi4py import MPI
+
+                comm = MPI.COMM_WORLD
+                return comm.Get_rank()
+            except ImportError:
+                raise ImportError("Need mpi4py in parallel mode (SERIAL_MODE = false)")
+        else:
+            return 0
 
     def _distinguish_nonlocal_grids(self, chunks):
+
+        if self.libyt.libyt_info["SERIAL_MODE"] is True:
+            # we don't need rma
+            return False, [], [], []
+
         # Split local and non-local grids.
         from mpi4py import MPI
 
         comm = MPI.COMM_WORLD
 
         local_id = []
         nonlocal_id = []
```

### Comparing `yt_libyt-0.0.7/yt_libyt.egg-info/PKG-INFO` & `yt_libyt-0.0.8/yt_libyt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt_libyt
-Version: 0.0.7
+Version: 0.0.8
 Summary: A yt frontend for libyt
 Author-email: Shin-Rong Tsai <turquoisea.tsai@gmail.com>, Hsi-Yu Schive <hyschive@gmail.com>, Matthew Turk <matthewturk@gmail.com>
 License: 
         
         BSD License
         
         Copyright (c) 2023, Shin-Rong Tsai, Hsi-Yu Schive, Matthew Turk
@@ -54,7 +54,21 @@
 
 This is a [`yt`](https://yt-project.org/) frontend for [`libyt`](https://github.com/yt-project/libyt).
 
 
 * **yt**: https://yt-project.org/
 * **libyt Repo**: https://github.com/yt-project/libyt
 * **libyt Doc**: https://libyt.readthedocs.io/en/latest/
+
+
+### Install
+
+- From PyPI:
+  ```bash
+  pip install yt-libyt
+  ```
+- From source:
+  ```bash
+  git clone https://github.com/data-exp-lab/yt_libyt.git
+  cd yt_libyt
+  pip install .
+  ```
```

