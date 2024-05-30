# Comparing `tmp/benchnirs-1.2.4.tar.gz` & `tmp/benchnirs-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benchnirs-1.2.4.tar", last modified: Tue May 28 15:13:02 2024, max compression
+gzip compressed data, was "benchnirs-1.2.5.tar", last modified: Thu May 30 22:47:34 2024, max compression
```

## Comparing `benchnirs-1.2.4.tar` & `benchnirs-1.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:13:02.641823 benchnirs-1.2.4/
--rw-rw-rw-   0 root         (0) root         (0)    35083 2024-05-28 15:12:54.000000 benchnirs-1.2.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8063 2024-05-28 15:13:02.640823 benchnirs-1.2.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7524 2024-05-28 15:12:54.000000 benchnirs-1.2.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:13:02.639823 benchnirs-1.2.4/benchnirs/
--rw-rw-rw-   0 root         (0) root         (0)      522 2024-05-28 15:12:54.000000 benchnirs-1.2.4/benchnirs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    50444 2024-05-28 15:12:54.000000 benchnirs-1.2.4/benchnirs/learn.py
--rw-rw-rw-   0 root         (0) root         (0)    25857 2024-05-28 15:12:54.000000 benchnirs-1.2.4/benchnirs/load.py
--rw-rw-rw-   0 root         (0) root         (0)     4108 2024-05-28 15:12:54.000000 benchnirs-1.2.4/benchnirs/process.py
--rw-rw-rw-   0 root         (0) root         (0)     3807 2024-05-28 15:12:54.000000 benchnirs-1.2.4/benchnirs/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:13:02.640823 benchnirs-1.2.4/benchnirs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8063 2024-05-28 15:13:02.000000 benchnirs-1.2.4/benchnirs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      287 2024-05-28 15:13:02.000000 benchnirs-1.2.4/benchnirs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 15:13:02.000000 benchnirs-1.2.4/benchnirs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       88 2024-05-28 15:13:02.000000 benchnirs-1.2.4/benchnirs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-28 15:13:02.000000 benchnirs-1.2.4/benchnirs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 15:13:02.641823 benchnirs-1.2.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      979 2024-05-28 15:12:54.000000 benchnirs-1.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:47:34.158582 benchnirs-1.2.5/
+-rw-rw-rw-   0 root         (0) root         (0)    35083 2024-05-30 22:47:29.000000 benchnirs-1.2.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8295 2024-05-30 22:47:34.157582 benchnirs-1.2.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7523 2024-05-30 22:47:29.000000 benchnirs-1.2.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:47:34.156582 benchnirs-1.2.5/benchnirs/
+-rw-rw-rw-   0 root         (0) root         (0)      522 2024-05-30 22:47:29.000000 benchnirs-1.2.5/benchnirs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    50444 2024-05-30 22:47:29.000000 benchnirs-1.2.5/benchnirs/learn.py
+-rw-rw-rw-   0 root         (0) root         (0)    25861 2024-05-30 22:47:29.000000 benchnirs-1.2.5/benchnirs/load.py
+-rw-rw-rw-   0 root         (0) root         (0)     4108 2024-05-30 22:47:29.000000 benchnirs-1.2.5/benchnirs/process.py
+-rw-rw-rw-   0 root         (0) root         (0)     3807 2024-05-30 22:47:29.000000 benchnirs-1.2.5/benchnirs/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:47:34.157582 benchnirs-1.2.5/benchnirs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8295 2024-05-30 22:47:34.000000 benchnirs-1.2.5/benchnirs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      287 2024-05-30 22:47:34.000000 benchnirs-1.2.5/benchnirs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 22:47:34.000000 benchnirs-1.2.5/benchnirs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2024-05-30 22:47:34.000000 benchnirs-1.2.5/benchnirs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-30 22:47:34.000000 benchnirs-1.2.5/benchnirs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 22:47:34.158582 benchnirs-1.2.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-05-30 22:47:29.000000 benchnirs-1.2.5/setup.py
```

### Comparing `benchnirs-1.2.4/LICENSE` & `benchnirs-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `benchnirs-1.2.4/PKG-INFO` & `benchnirs-1.2.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: benchnirs
-Version: 1.2.4
-Summary: Benchmarking framework for machine learning with fNIRS
-Home-page: https://gitlab.com/HanBnrd/benchnirs
-Author: Johann Benerradi
-Author-email: johann.benerradi@gmail.com
-License: GNU GPLv3+
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # BenchNIRS
 
 <img title="BenchNIRS" align="right" width="150" height="150" src="https://hanbnrd.gitlab.io/assets/img/logos/benchnirs.png" alt="BenchNIRS">
 
 *Benchmarking framework for machine learning with fNIRS*
 
 **Quick links**  
@@ -111,15 +95,15 @@
 - tracking bugs
 
 Contributions are encouraged under the form of [issues](https://gitlab.com/HanBnrd/benchnirs/-/issues) (for reporting bugs or requesting new features) and [merge requests](https://gitlab.com/HanBnrd/benchnirs/-/merge_requests) (for fixing bugs and implementing new features).
 Please refer to [this tutorial](https://docs.gitlab.com/ee/user/project/repository/forking_workflow.html) for creating merge requests from a fork of the repository.
 
 
 ## Acknowledgements
-If you are using *BenchNIRS*, please cite [this article](https://doi.org/10.3389/fnrgo.2023.994969>):
+If you are using *BenchNIRS*, please cite [this article](https://doi.org/10.3389/fnrgo.2023.994969):
 ```
 @article{benerradi2023benchmarking,
   title={Benchmarking framework for machine learning classification from fNIRS data},
   author={Benerradi, Johann and Clos, Jeremie and Landowska, Aleksandra and Valstar, Michel F and Wilson, Max L},
   journal={Frontiers in Neuroergonomics},
   volume={4},
   year={2023},
@@ -181,9 +165,7 @@
 > 	volume={8},
 > 	number={12},
 > 	pages={1486},
 > 	year={2019},
 > 	publisher={Multidisciplinary Digital Publishing Institute}
 > }
 > ```
-
-
```

### Comparing `benchnirs-1.2.4/README.md` & `benchnirs-1.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: benchnirs
+Version: 1.2.5
+Summary: Benchmarking framework for machine learning with fNIRS
+Home-page: https://gitlab.com/HanBnrd/benchnirs
+Author: Johann Benerradi
+Author-email: johann.benerradi@gmail.com
+License: GNU GPLv3+
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: lazy_loader
+Requires-Dist: tqdm
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: scipy
+Requires-Dist: mne
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
+Requires-Dist: scikit-learn
+Requires-Dist: torch
+Requires-Dist: nirsimple
+
 # BenchNIRS
 
 <img title="BenchNIRS" align="right" width="150" height="150" src="https://hanbnrd.gitlab.io/assets/img/logos/benchnirs.png" alt="BenchNIRS">
 
 *Benchmarking framework for machine learning with fNIRS*
 
 **Quick links**  
@@ -95,15 +121,15 @@
 - tracking bugs
 
 Contributions are encouraged under the form of [issues](https://gitlab.com/HanBnrd/benchnirs/-/issues) (for reporting bugs or requesting new features) and [merge requests](https://gitlab.com/HanBnrd/benchnirs/-/merge_requests) (for fixing bugs and implementing new features).
 Please refer to [this tutorial](https://docs.gitlab.com/ee/user/project/repository/forking_workflow.html) for creating merge requests from a fork of the repository.
 
 
 ## Acknowledgements
-If you are using *BenchNIRS*, please cite [this article](https://doi.org/10.3389/fnrgo.2023.994969>):
+If you are using *BenchNIRS*, please cite [this article](https://doi.org/10.3389/fnrgo.2023.994969):
 ```
 @article{benerradi2023benchmarking,
   title={Benchmarking framework for machine learning classification from fNIRS data},
   author={Benerradi, Johann and Clos, Jeremie and Landowska, Aleksandra and Valstar, Michel F and Wilson, Max L},
   journal={Frontiers in Neuroergonomics},
   volume={4},
   year={2023},
```

### Comparing `benchnirs-1.2.4/benchnirs/__init__.py` & `benchnirs-1.2.5/benchnirs/__init__.py`

 * *Files identical despite different names*

### Comparing `benchnirs-1.2.4/benchnirs/learn.py` & `benchnirs-1.2.5/benchnirs/learn.py`

 * *Files identical despite different names*

### Comparing `benchnirs-1.2.4/benchnirs/load.py` & `benchnirs-1.2.5/benchnirs/load.py`

 * *Files 0% similar despite different names*

```diff
@@ -451,15 +451,15 @@
     def load(self, subject, path=PATH_BAK_2019):
         data = {}
         data['sides'] = {'Right MC HbO': range(10, 20),
                          'Right MC HbR': range(30, 40),
                          'Left MC HbO': range(0, 10),
                          'Left MC HbR': range(20, 30)}
         data['event_id'] = {'right': 1, 'left': 2, 'foot': 3}
-        data['tmin'] = -2
+        data['tmin'] = -1.925
         data['tmax'] = 10
 
         # Load data matrices
         mat = scipy.io.loadmat(f'{path}/{subject}.mat')
 
         # Get sampling frequency (in Hz)
         data['sfreq'] = mat['dat']['fs'][0, 0][0, 0]
```

### Comparing `benchnirs-1.2.4/benchnirs/process.py` & `benchnirs-1.2.5/benchnirs/process.py`

 * *Files identical despite different names*

### Comparing `benchnirs-1.2.4/benchnirs/viz.py` & `benchnirs-1.2.5/benchnirs/viz.py`

 * *Files identical despite different names*

### Comparing `benchnirs-1.2.4/benchnirs.egg-info/PKG-INFO` & `benchnirs-1.2.5/benchnirs.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 Metadata-Version: 2.1
 Name: benchnirs
-Version: 1.2.4
+Version: 1.2.5
 Summary: Benchmarking framework for machine learning with fNIRS
 Home-page: https://gitlab.com/HanBnrd/benchnirs
 Author: Johann Benerradi
 Author-email: johann.benerradi@gmail.com
 License: GNU GPLv3+
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: lazy_loader
+Requires-Dist: tqdm
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: scipy
+Requires-Dist: mne
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
+Requires-Dist: scikit-learn
+Requires-Dist: torch
+Requires-Dist: nirsimple
 
 # BenchNIRS
 
 <img title="BenchNIRS" align="right" width="150" height="150" src="https://hanbnrd.gitlab.io/assets/img/logos/benchnirs.png" alt="BenchNIRS">
 
 *Benchmarking framework for machine learning with fNIRS*
 
@@ -111,15 +121,15 @@
 - tracking bugs
 
 Contributions are encouraged under the form of [issues](https://gitlab.com/HanBnrd/benchnirs/-/issues) (for reporting bugs or requesting new features) and [merge requests](https://gitlab.com/HanBnrd/benchnirs/-/merge_requests) (for fixing bugs and implementing new features).
 Please refer to [this tutorial](https://docs.gitlab.com/ee/user/project/repository/forking_workflow.html) for creating merge requests from a fork of the repository.
 
 
 ## Acknowledgements
-If you are using *BenchNIRS*, please cite [this article](https://doi.org/10.3389/fnrgo.2023.994969>):
+If you are using *BenchNIRS*, please cite [this article](https://doi.org/10.3389/fnrgo.2023.994969):
 ```
 @article{benerradi2023benchmarking,
   title={Benchmarking framework for machine learning classification from fNIRS data},
   author={Benerradi, Johann and Clos, Jeremie and Landowska, Aleksandra and Valstar, Michel F and Wilson, Max L},
   journal={Frontiers in Neuroergonomics},
   volume={4},
   year={2023},
@@ -181,9 +191,7 @@
 > 	volume={8},
 > 	number={12},
 > 	pages={1486},
 > 	year={2019},
 > 	publisher={Multidisciplinary Digital Publishing Institute}
 > }
 > ```
-
-
```

### Comparing `benchnirs-1.2.4/setup.py` & `benchnirs-1.2.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="benchnirs",
-    version="1.2.4",
+    version="1.2.5",
     author="Johann Benerradi",
     author_email="johann.benerradi@gmail.com",
     description="Benchmarking framework for machine learning with fNIRS",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/HanBnrd/benchnirs",
     license="GNU GPLv3+",
```

