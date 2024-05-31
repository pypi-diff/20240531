# Comparing `tmp/treat2p-0.0.4.tar.gz` & `tmp/treat2p-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treat2p-0.0.4.tar", last modified: Thu Apr 11 10:25:05 2024, max compression
+gzip compressed data, was "treat2p-0.0.5.tar", last modified: Fri May 31 16:24:10 2024, max compression
```

## Comparing `treat2p-0.0.4.tar` & `treat2p-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 10:25:05.810577 treat2p-0.0.4/
--rw-r--r--   0 root         (0) root         (0)      845 2024-04-11 10:25:05.810577 treat2p-0.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1280 2024-04-11 10:24:56.000000 treat2p-0.0.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 10:25:05.814577 treat2p-0.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1504 2024-04-11 10:24:56.000000 treat2p-0.0.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 10:25:05.810577 treat2p-0.0.4/treat2p/
--rw-rw-rw-   0 root         (0) root         (0)       90 2024-04-11 10:24:56.000000 treat2p-0.0.4/treat2p/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17760 2024-04-11 10:24:56.000000 treat2p-0.0.4/treat2p/calculations.py
--rw-rw-rw-   0 root         (0) root         (0)    10906 2024-04-11 10:24:56.000000 treat2p-0.0.4/treat2p/core.py
--rw-rw-rw-   0 root         (0) root         (0)     1466 2024-04-11 10:24:56.000000 treat2p-0.0.4/treat2p/corrections.py
--rw-rw-rw-   0 root         (0) root         (0)     4905 2024-04-11 10:24:56.000000 treat2p-0.0.4/treat2p/normalisation.py
--rw-rw-rw-   0 root         (0) root         (0)    13631 2024-04-11 10:24:56.000000 treat2p-0.0.4/treat2p/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 10:25:05.810577 treat2p-0.0.4/treat2p.egg-info/
--rw-r--r--   0 root         (0) root         (0)      845 2024-04-11 10:25:05.000000 treat2p-0.0.4/treat2p.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      297 2024-04-11 10:25:05.000000 treat2p-0.0.4/treat2p.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 10:25:05.000000 treat2p-0.0.4/treat2p.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       35 2024-04-11 10:25:05.000000 treat2p-0.0.4/treat2p.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-11 10:25:05.000000 treat2p-0.0.4/treat2p.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 16:24:10.546915 treat2p-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)      845 2024-05-31 16:24:10.546915 treat2p-0.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1280 2024-05-31 16:24:00.000000 treat2p-0.0.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 16:24:10.546915 treat2p-0.0.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2024-05-31 16:24:00.000000 treat2p-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 16:24:10.546915 treat2p-0.0.5/treat2p/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2024-05-31 16:24:00.000000 treat2p-0.0.5/treat2p/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17760 2024-05-31 16:24:00.000000 treat2p-0.0.5/treat2p/calculations.py
+-rw-rw-rw-   0 root         (0) root         (0)    10956 2024-05-31 16:24:00.000000 treat2p-0.0.5/treat2p/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2024-05-31 16:24:00.000000 treat2p-0.0.5/treat2p/corrections.py
+-rw-rw-rw-   0 root         (0) root         (0)     4905 2024-05-31 16:24:00.000000 treat2p-0.0.5/treat2p/normalisation.py
+-rw-rw-rw-   0 root         (0) root         (0)    13631 2024-05-31 16:24:00.000000 treat2p-0.0.5/treat2p/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 16:24:10.546915 treat2p-0.0.5/treat2p.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      845 2024-05-31 16:24:10.000000 treat2p-0.0.5/treat2p.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      297 2024-05-31 16:24:10.000000 treat2p-0.0.5/treat2p.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 16:24:10.000000 treat2p-0.0.5/treat2p.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2024-05-31 16:24:10.000000 treat2p-0.0.5/treat2p.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-31 16:24:10.000000 treat2p-0.0.5/treat2p.egg-info/top_level.txt
```

### Comparing `treat2p-0.0.4/PKG-INFO` & `treat2p-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treat2p
-Version: 0.0.4
+Version: 0.0.5
 Summary: Projects specific python code pipeline for analysis
 Home-page: https://gitlab.pasteur.fr/haisslab/analysis-packages/treat2p
 Author: Timothé Jost-MOUSSEAU
 Author-email: timothe.jost-mousseau@pasteur.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `treat2p-0.0.4/README.md` & `treat2p-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `treat2p-0.0.4/setup.py` & `treat2p-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `treat2p-0.0.4/treat2p/calculations.py` & `treat2p-0.0.5/treat2p/calculations.py`

 * *Files identical despite different names*

### Comparing `treat2p-0.0.4/treat2p/core.py` & `treat2p-0.0.5/treat2p/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 from logging import getLogger
 from tqdm import tqdm
+from sys import stdout
 from joblib import parallel_backend, delayed, Parallel
 from .utils import ParameterRegistrator, tqdm_joblib
 from .corrections import neuropil, slow_trend
 from .normalisation import center_normalize, delta_over_F
 import numpy as np
 
 
@@ -92,15 +93,17 @@
 
     original_stats = np.load(stat_file, allow_pickle=True)
     original_ops = np.load(ops_file, allow_pickle=True).item()
 
     local_log.info(f"Found F, Fneu, stats and ops files at the specified root : {suite2p_results_path}")
 
     local_log.info(f"Running the signal treatment pipeline over {Fs.shape[0]} rois on {n_jobs} processors. Hold tight.")
-    with parallel_backend(backend, n_jobs=n_jobs), tqdm_joblib(tqdm(desc="Treating ROIS signal", total=Fs.shape[0])):
+    with parallel_backend(backend, n_jobs=n_jobs), tqdm_joblib(
+        tqdm(desc="Treating ROIS signal", total=Fs.shape[0], file=stdout)
+    ):
         results = Parallel()(delayed(pipeline)(F, Fneu, **kwargs) for F, Fneu in zip(Fs, Fneus))
 
     local_log.info("Processing finished. About to save the output")
 
     # save outputs to suite2p results folder
     outputs, corr_stats, final_ops = (
         [item[0] for item in results],
```

### Comparing `treat2p-0.0.4/treat2p/corrections.py` & `treat2p-0.0.5/treat2p/corrections.py`

 * *Files identical despite different names*

### Comparing `treat2p-0.0.4/treat2p/normalisation.py` & `treat2p-0.0.5/treat2p/normalisation.py`

 * *Files identical despite different names*

### Comparing `treat2p-0.0.4/treat2p/utils.py` & `treat2p-0.0.5/treat2p/utils.py`

 * *Files identical despite different names*

### Comparing `treat2p-0.0.4/treat2p.egg-info/PKG-INFO` & `treat2p-0.0.5/treat2p.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treat2p
-Version: 0.0.4
+Version: 0.0.5
 Summary: Projects specific python code pipeline for analysis
 Home-page: https://gitlab.pasteur.fr/haisslab/analysis-packages/treat2p
 Author: Timothé Jost-MOUSSEAU
 Author-email: timothe.jost-mousseau@pasteur.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

