# Comparing `tmp/taguchi-1.0.4.tar.gz` & `tmp/taguchi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taguchi-1.0.4.tar", last modified: Fri May 31 01:38:34 2024, max compression
+gzip compressed data, was "taguchi-1.1.0.tar", last modified: Fri May 31 02:03:45 2024, max compression
```

## Comparing `taguchi-1.0.4.tar` & `taguchi-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-31 01:38:34.458768 taguchi-1.0.4/
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)       29 2024-05-09 03:46:44.000000 taguchi-1.0.4/MANIFEST.in
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     4216 2024-05-31 01:38:34.457768 taguchi-1.0.4/PKG-INFO
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     3786 2024-05-09 03:35:22.000000 taguchi-1.0.4/README.md
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      103 2024-05-04 04:45:54.000000 taguchi-1.0.4/pyproject.toml
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      757 2024-05-31 01:38:34.458768 taguchi-1.0.4/setup.cfg
-drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-31 01:38:34.457768 taguchi-1.0.4/taguchi/
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)       17 2024-05-31 01:37:40.000000 taguchi-1.0.4/taguchi/__init__.py
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     3329 2024-05-17 20:49:51.000000 taguchi-1.0.4/taguchi/__main__.py
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)   127056 2024-05-31 01:37:34.000000 taguchi-1.0.4/taguchi/database.json
-drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-31 01:38:34.457768 taguchi-1.0.4/taguchi.egg-info/
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     4216 2024-05-31 01:38:34.000000 taguchi-1.0.4/taguchi.egg-info/PKG-INFO
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      296 2024-05-31 01:38:34.000000 taguchi-1.0.4/taguchi.egg-info/SOURCES.txt
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-31 01:38:34.000000 taguchi-1.0.4/taguchi.egg-info/dependency_links.txt
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)       54 2024-05-31 01:38:34.000000 taguchi-1.0.4/taguchi.egg-info/entry_points.txt
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-04 04:46:44.000000 taguchi-1.0.4/taguchi.egg-info/not-zip-safe
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)        8 2024-05-31 01:38:34.000000 taguchi-1.0.4/taguchi.egg-info/top_level.txt
+drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-31 02:03:45.225072 taguchi-1.1.0/
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)       29 2024-05-09 03:46:44.000000 taguchi-1.1.0/MANIFEST.in
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     4596 2024-05-31 02:03:45.225072 taguchi-1.1.0/PKG-INFO
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     4166 2024-05-31 02:03:14.000000 taguchi-1.1.0/README.md
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      103 2024-05-04 04:45:54.000000 taguchi-1.1.0/pyproject.toml
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      757 2024-05-31 02:03:45.226072 taguchi-1.1.0/setup.cfg
+drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-31 02:03:45.220072 taguchi-1.1.0/taguchi/
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)       17 2024-05-31 01:58:54.000000 taguchi-1.1.0/taguchi/__init__.py
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     3572 2024-05-31 01:57:39.000000 taguchi-1.1.0/taguchi/__main__.py
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)   127056 2024-05-31 01:37:34.000000 taguchi-1.1.0/taguchi/database.json
+drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-31 02:03:45.224072 taguchi-1.1.0/taguchi.egg-info/
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     4596 2024-05-31 02:03:45.000000 taguchi-1.1.0/taguchi.egg-info/PKG-INFO
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      296 2024-05-31 02:03:45.000000 taguchi-1.1.0/taguchi.egg-info/SOURCES.txt
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-31 02:03:45.000000 taguchi-1.1.0/taguchi.egg-info/dependency_links.txt
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)       54 2024-05-31 02:03:45.000000 taguchi-1.1.0/taguchi.egg-info/entry_points.txt
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-04 04:46:44.000000 taguchi-1.1.0/taguchi.egg-info/not-zip-safe
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)        8 2024-05-31 02:03:45.000000 taguchi-1.1.0/taguchi.egg-info/top_level.txt
```

### Comparing `taguchi-1.0.4/PKG-INFO` & `taguchi-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taguchi
-Version: 1.0.4
+Version: 1.1.0
 Summary: A tool for optimising systems parameterised by environment variables, based on Taguchi/orthogonal array systems of experiments.
 Home-page: https://github.com/jcranney/taguchi
 Author: Jesse Cranney
 Author-email: jesse.cranney@anu.edu.au
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -79,12 +79,19 @@
 ```
 This print-out gives us an indication of the average performance for each parameter at each state level. If one were trying to minimise this function, setting `PARAM_B` to be close to -20 seems to be a good choice, since it seems to have the biggest impact from these tests. 
 
 The novelty of doing this using the `taguchi` method is that reasonably informative results can be obtained over far few experiment runs. For a full search of 3 parameters with 3 values each, one would need $27=3^3$ experiment runs, but using the `taguchi` method, it is done using only 9 experiments.
 
 This library supports up to 20 parameters, with up to 5 states each. In that extreme case, the full search would contain $5^{20}\approx10^{14}$ experiments, whereas the `taguchi` method only requires 100 experiments. If each experiment only takes 1 second to run, then the former method would complete in about 3 million years, and the latter would take less than 2 minutes.
 
+## `--dense`
+Sometimes efficiency is scary, so if you want to run the experiment using every possible combination of parameters and then collate the results, you can do so by running with the dense flag, e.g.,
+```bash
+taguchi --dense
+```
+which will run 27 experiments in the example case, rather than the efficient 9 experiments generated by the orthogonal array/Taguchi method.
+
 ## Wishlist
 This project is not without its shortcomings. 
  - There is currently no capacity to have a different number of states in the `taguchi.yaml` file for each parameter. If you want 1 parameter to have 5 different state values, you must give all parameters 5 different state values (or 1, since it is not varied in that case).
  - The documentation is lacking (arguably non-existent).
  - There is no capacity for parallelisation of the experiments. This might be straightforward in some cases, but in my test cases I can only have one experiment per GPU and that complicates things.
```

### Comparing `taguchi-1.0.4/README.md` & `taguchi-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -67,12 +67,19 @@
 ```
 This print-out gives us an indication of the average performance for each parameter at each state level. If one were trying to minimise this function, setting `PARAM_B` to be close to -20 seems to be a good choice, since it seems to have the biggest impact from these tests. 
 
 The novelty of doing this using the `taguchi` method is that reasonably informative results can be obtained over far few experiment runs. For a full search of 3 parameters with 3 values each, one would need $27=3^3$ experiment runs, but using the `taguchi` method, it is done using only 9 experiments.
 
 This library supports up to 20 parameters, with up to 5 states each. In that extreme case, the full search would contain $5^{20}\approx10^{14}$ experiments, whereas the `taguchi` method only requires 100 experiments. If each experiment only takes 1 second to run, then the former method would complete in about 3 million years, and the latter would take less than 2 minutes.
 
+## `--dense`
+Sometimes efficiency is scary, so if you want to run the experiment using every possible combination of parameters and then collate the results, you can do so by running with the dense flag, e.g.,
+```bash
+taguchi --dense
+```
+which will run 27 experiments in the example case, rather than the efficient 9 experiments generated by the orthogonal array/Taguchi method.
+
 ## Wishlist
 This project is not without its shortcomings. 
  - There is currently no capacity to have a different number of states in the `taguchi.yaml` file for each parameter. If you want 1 parameter to have 5 different state values, you must give all parameters 5 different state values (or 1, since it is not varied in that case).
  - The documentation is lacking (arguably non-existent).
  - There is no capacity for parallelisation of the experiments. This might be straightforward in some cases, but in my test cases I can only have one experiment per GPU and that complicates things.
```

### Comparing `taguchi-1.0.4/setup.cfg` & `taguchi-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `taguchi-1.0.4/taguchi/__main__.py` & `taguchi-1.1.0/taguchi/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 #/usr/bin/env python
 import os
 import yaml
 import subprocess
 import argparse
 import json
 from importlib import resources
+from itertools import product
 
 parser = argparse.ArgumentParser(
                     prog='taguchi',
                     description='performs taguchi based experiments',
                     epilog='see https://github.com/jcranney/taguchi for more info.')
 
 parser.add_argument('-v', '--verbose',
             action='count', default=0)  # on/off flag
+parser.add_argument('-d', '--dense',
+            action='count', default=0)  # on/off flag
 args = parser.parse_args()
 verbose = args.verbose
+dense = args.dense
 
 with open("./taguchi.yaml","r") as f:
     a : dict = yaml.full_load(f)
 
 command = a.pop("command")
 
 params = []
@@ -48,18 +52,21 @@
         raise ValueError("All parameters must have the same number of states (for now)")
 
 filename = resources.files("taguchi")/"database.json"
 
 with open(filename,"r") as f:
     orthogonal_arrays = json.load(f)
 
-try:
-    array = orthogonal_arrays[f"{n_params:d},{n_states:d}"]
-except KeyError as e:
-    raise NotImplementedError(f"{n_params:d} params with {n_states:d} states not supported.")
+if dense:
+    array = list(product(range(n_states),repeat=n_params))
+else:
+    try:
+        array = orthogonal_arrays[f"{n_params:d},{n_states:d}"]
+    except KeyError as e:
+        raise NotImplementedError(f"{n_params:d} params with {n_states:d} states not supported, try --dense")
 
 if verbose:
     print(f"Doing {len(array)} experiments in total!\n")
 if verbose > 1:
     print("Experiments:")
     print(array)
```

### Comparing `taguchi-1.0.4/taguchi/database.json` & `taguchi-1.1.0/taguchi/database.json`

 * *Files identical despite different names*

### Comparing `taguchi-1.0.4/taguchi.egg-info/PKG-INFO` & `taguchi-1.1.0/taguchi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taguchi
-Version: 1.0.4
+Version: 1.1.0
 Summary: A tool for optimising systems parameterised by environment variables, based on Taguchi/orthogonal array systems of experiments.
 Home-page: https://github.com/jcranney/taguchi
 Author: Jesse Cranney
 Author-email: jesse.cranney@anu.edu.au
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -79,12 +79,19 @@
 ```
 This print-out gives us an indication of the average performance for each parameter at each state level. If one were trying to minimise this function, setting `PARAM_B` to be close to -20 seems to be a good choice, since it seems to have the biggest impact from these tests. 
 
 The novelty of doing this using the `taguchi` method is that reasonably informative results can be obtained over far few experiment runs. For a full search of 3 parameters with 3 values each, one would need $27=3^3$ experiment runs, but using the `taguchi` method, it is done using only 9 experiments.
 
 This library supports up to 20 parameters, with up to 5 states each. In that extreme case, the full search would contain $5^{20}\approx10^{14}$ experiments, whereas the `taguchi` method only requires 100 experiments. If each experiment only takes 1 second to run, then the former method would complete in about 3 million years, and the latter would take less than 2 minutes.
 
+## `--dense`
+Sometimes efficiency is scary, so if you want to run the experiment using every possible combination of parameters and then collate the results, you can do so by running with the dense flag, e.g.,
+```bash
+taguchi --dense
+```
+which will run 27 experiments in the example case, rather than the efficient 9 experiments generated by the orthogonal array/Taguchi method.
+
 ## Wishlist
 This project is not without its shortcomings. 
  - There is currently no capacity to have a different number of states in the `taguchi.yaml` file for each parameter. If you want 1 parameter to have 5 different state values, you must give all parameters 5 different state values (or 1, since it is not varied in that case).
  - The documentation is lacking (arguably non-existent).
  - There is no capacity for parallelisation of the experiments. This might be straightforward in some cases, but in my test cases I can only have one experiment per GPU and that complicates things.
```

