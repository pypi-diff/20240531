# Comparing `tmp/mbirjax-0.1.0.tar.gz` & `tmp/mbirjax-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbirjax-0.1.0.tar", last modified: Fri May 24 17:23:43 2024, max compression
+gzip compressed data, was "mbirjax-0.2.0.tar", last modified: Thu May 30 22:32:51 2024, max compression
```

## Comparing `mbirjax-0.1.0.tar` & `mbirjax-0.2.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-24 17:23:43.196048 mbirjax-0.1.0/
--rw-r--r--   0 bouman     (501) staff       (20)     1524 2024-05-19 20:53:29.000000 mbirjax-0.1.0/LICENSE
-drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-24 17:23:43.195674 mbirjax-0.1.0/MBIRJAX.egg-info/
--rw-r--r--   0 bouman     (501) staff       (20)     3869 2024-05-24 17:23:43.000000 mbirjax-0.1.0/MBIRJAX.egg-info/PKG-INFO
--rw-r--r--   0 bouman     (501) staff       (20)      978 2024-05-24 17:23:43.000000 mbirjax-0.1.0/MBIRJAX.egg-info/SOURCES.txt
--rw-r--r--   0 bouman     (501) staff       (20)        1 2024-05-24 17:23:43.000000 mbirjax-0.1.0/MBIRJAX.egg-info/dependency_links.txt
--rw-r--r--   0 bouman     (501) staff       (20)       53 2024-05-24 17:23:43.000000 mbirjax-0.1.0/MBIRJAX.egg-info/top_level.txt
--rw-r--r--   0 bouman     (501) staff       (20)     3869 2024-05-24 17:23:43.195867 mbirjax-0.1.0/PKG-INFO
--rw-r--r--   0 bouman     (501) staff       (20)     1745 2024-05-24 17:20:04.000000 mbirjax-0.1.0/README.rst
-drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-24 17:23:43.191387 mbirjax-0.1.0/demo/
--rw-r--r--   0 bouman     (501) staff       (20)     1996 2024-05-24 17:20:04.000000 mbirjax-0.1.0/demo/demo_cone_beam_shepp_logan.py
--rw-r--r--   0 bouman     (501) staff       (20)     1810 2024-05-24 17:20:04.000000 mbirjax-0.1.0/demo/demo_parbeam_shepp_logan.py
-drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-24 17:23:43.189869 mbirjax-0.1.0/docs/
-drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-24 17:23:43.189741 mbirjax-0.1.0/docs/build/
-drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-24 17:23:43.189799 mbirjax-0.1.0/docs/build/html/
-drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-24 17:23:43.191527 mbirjax-0.1.0/docs/build/html/_static/
--rw-r--r--   0 bouman     (501) staff       (20)     6710 2024-05-22 19:42:27.000000 mbirjax-0.1.0/docs/build/html/_static/new_model_template.py
-drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-24 17:23:43.191896 mbirjax-0.1.0/docs/source/
-drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-24 17:23:43.192013 mbirjax-0.1.0/docs/source/_static/
--rw-r--r--   0 bouman     (501) staff       (20)     6710 2024-05-24 17:20:04.000000 mbirjax-0.1.0/docs/source/_static/new_model_template.py
--rw-r--r--   0 bouman     (501) staff       (20)     4066 2024-05-24 17:20:04.000000 mbirjax-0.1.0/docs/source/conf.py
-drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-24 17:23:43.192828 mbirjax-0.1.0/experiments/
--rw-r--r--   0 bouman     (501) staff       (20)     8957 2024-05-24 17:20:13.000000 mbirjax-0.1.0/experiments/cone_beam_dev.py
-drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-24 17:23:43.192950 mbirjax-0.1.0/experiments/cvpr-2024/
--rw-r--r--   0 bouman     (501) staff       (20)     4154 2024-05-24 17:20:04.000000 mbirjax-0.1.0/experiments/cvpr-2024/vcd_figs_for_abst.py
-drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-24 17:23:43.193694 mbirjax-0.1.0/experiments/gpu_performance/
--rw-r--r--   0 bouman     (501) staff       (20)    12172 2024-05-24 17:20:04.000000 mbirjax-0.1.0/experiments/gpu_performance/cumulative_memory.py
--rw-r--r--   0 bouman     (501) staff       (20)     7443 2024-05-24 17:20:04.000000 mbirjax-0.1.0/experiments/gpu_performance/display_results.py
--rw-r--r--   0 bouman     (501) staff       (20)     4636 2024-05-24 17:20:04.000000 mbirjax-0.1.0/experiments/gpu_performance/evaluate_over_indices.py
--rw-r--r--   0 bouman     (501) staff       (20)     1475 2024-05-24 17:20:04.000000 mbirjax-0.1.0/experiments/gpu_performance/initialize_evaluation.py
--rw-r--r--   0 bouman     (501) staff       (20)     6751 2024-05-24 17:20:04.000000 mbirjax-0.1.0/experiments/parallel_model_dev.py
--rw-r--r--   0 bouman     (501) staff       (20)     1997 2024-05-24 17:20:04.000000 mbirjax-0.1.0/experiments/prox_test.py
--rw-r--r--   0 bouman     (501) staff       (20)     2939 2024-05-24 17:20:13.000000 mbirjax-0.1.0/experiments/recon_conebeam.py
--rw-r--r--   0 bouman     (501) staff       (20)     2509 2024-05-24 17:20:04.000000 mbirjax-0.1.0/experiments/recon_parbeam.py
-drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-24 17:23:43.195219 mbirjax-0.1.0/mbirjax/
--rw-r--r--   0 bouman     (501) staff       (20)      223 2024-05-24 17:20:04.000000 mbirjax-0.1.0/mbirjax/__init__.py
--rw-r--r--   0 bouman     (501) staff       (20)     2458 2024-05-24 17:20:04.000000 mbirjax-0.1.0/mbirjax/_utils.py
--rw-r--r--   0 bouman     (501) staff       (20)    33627 2024-05-24 17:20:13.000000 mbirjax-0.1.0/mbirjax/cone_beam.py
--rw-r--r--   0 bouman     (501) staff       (20)     3050 2024-05-24 17:20:04.000000 mbirjax-0.1.0/mbirjax/gpu_memory.py
--rw-r--r--   0 bouman     (501) staff       (20)    16104 2024-05-24 17:20:04.000000 mbirjax-0.1.0/mbirjax/parallel_beam.py
--rw-r--r--   0 bouman     (501) staff       (20)    10773 2024-05-24 17:20:04.000000 mbirjax-0.1.0/mbirjax/parameter_handler.py
--rw-r--r--   0 bouman     (501) staff       (20)    13300 2024-05-24 17:20:13.000000 mbirjax-0.1.0/mbirjax/plot_utils.py
--rw-r--r--   0 bouman     (501) staff       (20)    20872 2024-05-24 17:20:04.000000 mbirjax-0.1.0/mbirjax/projectors.py
--rw-r--r--   0 bouman     (501) staff       (20)    42599 2024-05-24 17:20:04.000000 mbirjax-0.1.0/mbirjax/tomography_model.py
--rw-r--r--   0 bouman     (501) staff       (20)    13574 2024-05-24 17:20:04.000000 mbirjax-0.1.0/mbirjax/vcd_utils.py
--rw-r--r--   0 bouman     (501) staff       (20)      517 2024-05-24 17:20:13.000000 mbirjax-0.1.0/pyproject.toml
--rw-r--r--   0 bouman     (501) staff       (20)       38 2024-05-24 17:23:43.196088 mbirjax-0.1.0/setup.cfg
-drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-24 17:23:43.195348 mbirjax-0.1.0/tests/
--rw-r--r--   0 bouman     (501) staff       (20)     9361 2024-05-24 17:20:04.000000 mbirjax-0.1.0/tests/test_projectors.py
+drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-30 22:32:51.156792 mbirjax-0.2.0/
+-rw-r--r--   0 bouman     (501) staff       (20)     1548 2024-05-30 22:29:02.000000 mbirjax-0.2.0/LICENSE
+drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-30 22:32:51.155989 mbirjax-0.2.0/MBIRJAX.egg-info/
+-rw-r--r--   0 bouman     (501) staff       (20)     4208 2024-05-30 22:32:51.000000 mbirjax-0.2.0/MBIRJAX.egg-info/PKG-INFO
+-rw-r--r--   0 bouman     (501) staff       (20)     1164 2024-05-30 22:32:51.000000 mbirjax-0.2.0/MBIRJAX.egg-info/SOURCES.txt
+-rw-r--r--   0 bouman     (501) staff       (20)        1 2024-05-30 22:32:51.000000 mbirjax-0.2.0/MBIRJAX.egg-info/dependency_links.txt
+-rw-r--r--   0 bouman     (501) staff       (20)      166 2024-05-30 22:32:51.000000 mbirjax-0.2.0/MBIRJAX.egg-info/requires.txt
+-rw-r--r--   0 bouman     (501) staff       (20)       53 2024-05-30 22:32:51.000000 mbirjax-0.2.0/MBIRJAX.egg-info/top_level.txt
+-rw-r--r--   0 bouman     (501) staff       (20)     4208 2024-05-30 22:32:51.156589 mbirjax-0.2.0/PKG-INFO
+-rw-r--r--   0 bouman     (501) staff       (20)     1289 2024-05-30 22:29:02.000000 mbirjax-0.2.0/README.rst
+drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-30 22:32:51.151318 mbirjax-0.2.0/demo/
+-rw-r--r--   0 bouman     (501) staff       (20)     2001 2024-05-30 22:29:02.000000 mbirjax-0.2.0/demo/demo_cone_beam_shepp_logan.py
+-rw-r--r--   0 bouman     (501) staff       (20)     1815 2024-05-30 22:29:02.000000 mbirjax-0.2.0/demo/demo_parbeam_shepp_logan.py
+-rw-r--r--   0 bouman     (501) staff       (20)     1422 2024-05-30 22:29:02.000000 mbirjax-0.2.0/demo/demo_slice_viewer.py
+drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-30 22:32:51.149244 mbirjax-0.2.0/docs/
+drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-30 22:32:51.149103 mbirjax-0.2.0/docs/build/
+drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-30 22:32:51.149163 mbirjax-0.2.0/docs/build/html/
+drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-30 22:32:51.151452 mbirjax-0.2.0/docs/build/html/_static/
+-rw-r--r--   0 bouman     (501) staff       (20)     9883 2024-05-30 21:47:34.000000 mbirjax-0.2.0/docs/build/html/_static/new_model_template.py
+drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-30 22:32:51.151653 mbirjax-0.2.0/docs/source/
+drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-30 22:32:51.151781 mbirjax-0.2.0/docs/source/_static/
+-rw-r--r--   0 bouman     (501) staff       (20)     9883 2024-05-30 22:29:02.000000 mbirjax-0.2.0/docs/source/_static/new_model_template.py
+-rw-r--r--   0 bouman     (501) staff       (20)     4066 2024-05-30 22:29:02.000000 mbirjax-0.2.0/docs/source/conf.py
+drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-30 22:32:51.152394 mbirjax-0.2.0/experiments/
+-rw-r--r--   0 bouman     (501) staff       (20)     8201 2024-05-30 22:29:02.000000 mbirjax-0.2.0/experiments/cone_beam_dev.py
+drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-30 22:32:51.152535 mbirjax-0.2.0/experiments/cvpr-2024/
+-rw-r--r--   0 bouman     (501) staff       (20)     4293 2024-05-30 22:29:02.000000 mbirjax-0.2.0/experiments/cvpr-2024/vcd_figs_for_abst.py
+drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-30 22:32:51.153126 mbirjax-0.2.0/experiments/gpu_performance/
+-rw-r--r--   0 bouman     (501) staff       (20)    12152 2024-05-30 22:29:02.000000 mbirjax-0.2.0/experiments/gpu_performance/cumulative_memory.py
+-rw-r--r--   0 bouman     (501) staff       (20)     7443 2024-05-30 22:29:02.000000 mbirjax-0.2.0/experiments/gpu_performance/display_results.py
+-rw-r--r--   0 bouman     (501) staff       (20)     4624 2024-05-30 22:29:02.000000 mbirjax-0.2.0/experiments/gpu_performance/evaluate_over_indices.py
+-rw-r--r--   0 bouman     (501) staff       (20)     1471 2024-05-30 22:29:02.000000 mbirjax-0.2.0/experiments/gpu_performance/initialize_evaluation.py
+-rw-r--r--   0 bouman     (501) staff       (20)     6739 2024-05-30 22:29:02.000000 mbirjax-0.2.0/experiments/parallel_model_dev.py
+-rw-r--r--   0 bouman     (501) staff       (20)     1995 2024-05-30 22:29:02.000000 mbirjax-0.2.0/experiments/prox_test.py
+-rw-r--r--   0 bouman     (501) staff       (20)     6213 2024-05-30 22:29:02.000000 mbirjax-0.2.0/experiments/recon_experiments.py
+drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-30 22:32:51.154671 mbirjax-0.2.0/mbirjax/
+-rw-r--r--   0 bouman     (501) staff       (20)      225 2024-05-30 22:29:02.000000 mbirjax-0.2.0/mbirjax/__init__.py
+-rw-r--r--   0 bouman     (501) staff       (20)     2457 2024-05-30 22:29:02.000000 mbirjax-0.2.0/mbirjax/_utils.py
+-rw-r--r--   0 bouman     (501) staff       (20)    34103 2024-05-30 22:29:02.000000 mbirjax-0.2.0/mbirjax/cone_beam.py
+-rw-r--r--   0 bouman     (501) staff       (20)     2049 2024-05-30 22:29:02.000000 mbirjax-0.2.0/mbirjax/memory_stats.py
+-rw-r--r--   0 bouman     (501) staff       (20)    15091 2024-05-30 22:29:02.000000 mbirjax-0.2.0/mbirjax/parallel_beam.py
+-rw-r--r--   0 bouman     (501) staff       (20)    10773 2024-05-30 22:29:02.000000 mbirjax-0.2.0/mbirjax/parameter_handler.py
+-rw-r--r--   0 bouman     (501) staff       (20)    13075 2024-05-30 22:29:02.000000 mbirjax-0.2.0/mbirjax/plot_utils.py
+-rw-r--r--   0 bouman     (501) staff       (20)    19584 2024-05-30 22:29:02.000000 mbirjax-0.2.0/mbirjax/projectors.py
+-rw-r--r--   0 bouman     (501) staff       (20)    47781 2024-05-30 22:29:02.000000 mbirjax-0.2.0/mbirjax/tomography_model.py
+-rw-r--r--   0 bouman     (501) staff       (20)    14257 2024-05-30 22:29:02.000000 mbirjax-0.2.0/mbirjax/vcd_utils.py
+-rw-r--r--   0 bouman     (501) staff       (20)     1111 2024-05-30 22:29:07.000000 mbirjax-0.2.0/pyproject.toml
+-rw-r--r--   0 bouman     (501) staff       (20)       38 2024-05-30 22:32:51.156835 mbirjax-0.2.0/setup.cfg
+drwxr-xr-x   0 bouman     (501) staff       (20)        0 2024-05-30 22:32:51.155744 mbirjax-0.2.0/tests/
+-rw-r--r--   0 bouman     (501) staff       (20)     9361 2024-05-30 22:29:02.000000 mbirjax-0.2.0/tests/test_projectors.py
```

### Comparing `mbirjax-0.1.0/LICENSE` & `mbirjax-0.2.0/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2021, Charles A Bouman
+Copyright (c) 2024, Charles A. Bouman and Gregery T. Buzzard
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `mbirjax-0.1.0/MBIRJAX.egg-info/PKG-INFO` & `mbirjax-0.2.0/MBIRJAX.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
-Name: MBIRJAX
-Version: 0.1.0
+Name: mbirjax
+Version: 0.2.0
 Summary: High-performance tomographic reconstruction
 Author-email: MBIRJAX development team <buzzard@purdue.edu>
 License: BSD 3-Clause License
         
-        Copyright (c) 2021, Charles A Bouman
+        Copyright (c) 2024, Charles A. Bouman and Gregery T. Buzzard
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this
            list of conditions and the following disclaimer.
@@ -31,82 +31,79 @@
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: homepage, https://mbirjax.readthedocs.io
 Project-URL: source, https://github.com/cabouman/mbirjax
-Requires-Python: >=3.8
+Keywords: tomography,tomographic reconstruction,computed tomography
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: setuptools
+Requires-Dist: jax
+Requires-Dist: jaxlib
+Requires-Dist: ruamel.yaml
+Requires-Dist: psutil
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinxcontrib-bibtex; extra == "docs"
+Requires-Dist: sphinx-book-theme>=1.0.1; extra == "docs"
+Requires-Dist: sphinx-design; extra == "docs"
+Requires-Dist: sphinx-copybutton; extra == "docs"
 
 .. docs-include-ref
 
-mbirjax
+MBIRJAX
 =======
-Model-Based Iterative Reconstruction (MBIR) for tomographic reconstruction that is based on the JAX programming language.
+
+Model-Based Iterative Reconstruction (MBIR) for tomographic reconstruction that is based on the `JAX <https://github.com/google/jax>`__ library.
 Full documentation is available at https://mbirjax.readthedocs.io .
 
-..
-    Include more detailed description here.
+Installing from PyPI
+--------------------
+
+    .. code-block::
+
+        pip install mbirjax
+
+Installing from Source
+----------------------
 
-Installing
-----------
-1. *Clone or download the repository:*
+1. *Clone the repository:*
 
     .. code-block::
 
         git clone git@github.com:cabouman/mbirjax.git
 
 2. Install the conda environment and package
 
-    a. Option 1: Clean install from dev_scripts
-
-        *******You can skip all other steps if you do a clean install.******
-
-        To do a clean install, use the command:
+    a. Option 1: Clean install using dev_scripts - We provide bash scripts that will do a clean install of MBIRJAX in a new conda environment using the commands:
 
         .. code-block::
 
             cd dev_scripts
             source clean_install_all.sh
 
-    b. Option 2: Manual install
-
-        1. *Create conda environment:*
-
-            Create a new conda environment named ``mbirjax`` using the following commands:
-
-            .. code-block::
-
-                conda create --name mbirjax python=3.10
-                conda activate mbirjax
-                pip install -r requirements.txt
+    b. Option 2: Manual install - You can also manually install MBIRJAX from the main directory of the repository with the following commands:
 
-            Anytime you want to use this package, this ``mbirjax`` environment should be activated with the following:
-
-            .. code-block::
-
-                conda activate mbirjax
-
-
-        2. *Install mbirjax package:*
-
-            Navigate to the main directory ``mbirjax/`` and run the following:
-
-            .. code-block::
-
-                pip install .
-
-            To allow editing of the package source while using the package, use
-
-            .. code-block::
-
-                pip install -e .
+        .. code-block::
 
+            conda create --name mbirjax python=3.10
+            conda activate mbirjax
+            pip install -r requirements.txt
+            pip install .
 
 Running Demo(s)
 ---------------
 
 Run any of the available demo scripts with something like the following:
 
     .. code-block::
```

### Comparing `mbirjax-0.1.0/MBIRJAX.egg-info/SOURCES.txt` & `mbirjax-0.2.0/MBIRJAX.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 LICENSE
 README.rst
 pyproject.toml
 MBIRJAX.egg-info/PKG-INFO
 MBIRJAX.egg-info/SOURCES.txt
 MBIRJAX.egg-info/dependency_links.txt
+MBIRJAX.egg-info/requires.txt
 MBIRJAX.egg-info/top_level.txt
 demo/demo_cone_beam_shepp_logan.py
 demo/demo_parbeam_shepp_logan.py
+demo/demo_slice_viewer.py
 docs/build/html/_static/new_model_template.py
 docs/source/conf.py
 docs/source/_static/new_model_template.py
 experiments/cone_beam_dev.py
 experiments/parallel_model_dev.py
 experiments/prox_test.py
-experiments/recon_conebeam.py
-experiments/recon_parbeam.py
+experiments/recon_experiments.py
 experiments/cvpr-2024/vcd_figs_for_abst.py
 experiments/gpu_performance/cumulative_memory.py
 experiments/gpu_performance/display_results.py
 experiments/gpu_performance/evaluate_over_indices.py
 experiments/gpu_performance/initialize_evaluation.py
 mbirjax/__init__.py
 mbirjax/_utils.py
 mbirjax/cone_beam.py
-mbirjax/gpu_memory.py
+mbirjax/memory_stats.py
 mbirjax/parallel_beam.py
 mbirjax/parameter_handler.py
 mbirjax/plot_utils.py
 mbirjax/projectors.py
 mbirjax/tomography_model.py
 mbirjax/vcd_utils.py
+mbirjax.egg-info/PKG-INFO
+mbirjax.egg-info/SOURCES.txt
+mbirjax.egg-info/dependency_links.txt
+mbirjax.egg-info/requires.txt
+mbirjax.egg-info/top_level.txt
 tests/test_projectors.py
```

### Comparing `mbirjax-0.1.0/PKG-INFO` & `mbirjax-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
-Name: MBIRJAX
-Version: 0.1.0
+Name: mbirjax
+Version: 0.2.0
 Summary: High-performance tomographic reconstruction
 Author-email: MBIRJAX development team <buzzard@purdue.edu>
 License: BSD 3-Clause License
         
-        Copyright (c) 2021, Charles A Bouman
+        Copyright (c) 2024, Charles A. Bouman and Gregery T. Buzzard
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this
            list of conditions and the following disclaimer.
@@ -31,82 +31,79 @@
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: homepage, https://mbirjax.readthedocs.io
 Project-URL: source, https://github.com/cabouman/mbirjax
-Requires-Python: >=3.8
+Keywords: tomography,tomographic reconstruction,computed tomography
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: setuptools
+Requires-Dist: jax
+Requires-Dist: jaxlib
+Requires-Dist: ruamel.yaml
+Requires-Dist: psutil
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinxcontrib-bibtex; extra == "docs"
+Requires-Dist: sphinx-book-theme>=1.0.1; extra == "docs"
+Requires-Dist: sphinx-design; extra == "docs"
+Requires-Dist: sphinx-copybutton; extra == "docs"
 
 .. docs-include-ref
 
-mbirjax
+MBIRJAX
 =======
-Model-Based Iterative Reconstruction (MBIR) for tomographic reconstruction that is based on the JAX programming language.
+
+Model-Based Iterative Reconstruction (MBIR) for tomographic reconstruction that is based on the `JAX <https://github.com/google/jax>`__ library.
 Full documentation is available at https://mbirjax.readthedocs.io .
 
-..
-    Include more detailed description here.
+Installing from PyPI
+--------------------
+
+    .. code-block::
+
+        pip install mbirjax
+
+Installing from Source
+----------------------
 
-Installing
-----------
-1. *Clone or download the repository:*
+1. *Clone the repository:*
 
     .. code-block::
 
         git clone git@github.com:cabouman/mbirjax.git
 
 2. Install the conda environment and package
 
-    a. Option 1: Clean install from dev_scripts
-
-        *******You can skip all other steps if you do a clean install.******
-
-        To do a clean install, use the command:
+    a. Option 1: Clean install using dev_scripts - We provide bash scripts that will do a clean install of MBIRJAX in a new conda environment using the commands:
 
         .. code-block::
 
             cd dev_scripts
             source clean_install_all.sh
 
-    b. Option 2: Manual install
-
-        1. *Create conda environment:*
-
-            Create a new conda environment named ``mbirjax`` using the following commands:
-
-            .. code-block::
-
-                conda create --name mbirjax python=3.10
-                conda activate mbirjax
-                pip install -r requirements.txt
+    b. Option 2: Manual install - You can also manually install MBIRJAX from the main directory of the repository with the following commands:
 
-            Anytime you want to use this package, this ``mbirjax`` environment should be activated with the following:
-
-            .. code-block::
-
-                conda activate mbirjax
-
-
-        2. *Install mbirjax package:*
-
-            Navigate to the main directory ``mbirjax/`` and run the following:
-
-            .. code-block::
-
-                pip install .
-
-            To allow editing of the package source while using the package, use
-
-            .. code-block::
-
-                pip install -e .
+        .. code-block::
 
+            conda create --name mbirjax python=3.10
+            conda activate mbirjax
+            pip install -r requirements.txt
+            pip install .
 
 Running Demo(s)
 ---------------
 
 Run any of the available demo scripts with something like the following:
 
     .. code-block::
```

### Comparing `mbirjax-0.1.0/README.rst` & `mbirjax-0.2.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,48 @@
 .. docs-include-ref
 
-mbirjax
+MBIRJAX
 =======
-Model-Based Iterative Reconstruction (MBIR) for tomographic reconstruction that is based on the JAX programming language.
+
+Model-Based Iterative Reconstruction (MBIR) for tomographic reconstruction that is based on the `JAX <https://github.com/google/jax>`__ library.
 Full documentation is available at https://mbirjax.readthedocs.io .
 
-..
-    Include more detailed description here.
+Installing from PyPI
+--------------------
+
+    .. code-block::
+
+        pip install mbirjax
+
+Installing from Source
+----------------------
 
-Installing
-----------
-1. *Clone or download the repository:*
+1. *Clone the repository:*
 
     .. code-block::
 
         git clone git@github.com:cabouman/mbirjax.git
 
 2. Install the conda environment and package
 
-    a. Option 1: Clean install from dev_scripts
-
-        *******You can skip all other steps if you do a clean install.******
-
-        To do a clean install, use the command:
+    a. Option 1: Clean install using dev_scripts - We provide bash scripts that will do a clean install of MBIRJAX in a new conda environment using the commands:
 
         .. code-block::
 
             cd dev_scripts
             source clean_install_all.sh
 
-    b. Option 2: Manual install
-
-        1. *Create conda environment:*
-
-            Create a new conda environment named ``mbirjax`` using the following commands:
-
-            .. code-block::
-
-                conda create --name mbirjax python=3.10
-                conda activate mbirjax
-                pip install -r requirements.txt
+    b. Option 2: Manual install - You can also manually install MBIRJAX from the main directory of the repository with the following commands:
 
-            Anytime you want to use this package, this ``mbirjax`` environment should be activated with the following:
-
-            .. code-block::
-
-                conda activate mbirjax
-
-
-        2. *Install mbirjax package:*
-
-            Navigate to the main directory ``mbirjax/`` and run the following:
-
-            .. code-block::
-
-                pip install .
-
-            To allow editing of the package source while using the package, use
-
-            .. code-block::
-
-                pip install -e .
+        .. code-block::
 
+            conda create --name mbirjax python=3.10
+            conda activate mbirjax
+            pip install -r requirements.txt
+            pip install .
 
 Running Demo(s)
 ---------------
 
 Run any of the available demo scripts with something like the following:
 
     .. code-block::
```

### Comparing `mbirjax-0.1.0/demo/demo_cone_beam_shepp_logan.py` & `mbirjax-0.2.0/demo/demo_cone_beam_shepp_logan.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     # Print out model parameters
     cone_model.print_params()
 
     # ##########################
     # Perform VCD reconstruction
     print('Starting recon')
     time0 = time.time()
-    recon, fm_rmse = cone_model.recon(sinogram, weights=weights)
+    recon, recon_params = cone_model.recon(sinogram, weights=weights)
 
     recon.block_until_ready()
     elapsed = time.time() - time0
     print('Elapsed time for recon is {:.3f} seconds'.format(elapsed))
     # ##########################
 
     # Display results
```

### Comparing `mbirjax-0.1.0/demo/demo_parbeam_shepp_logan.py` & `mbirjax-0.2.0/demo/demo_parbeam_shepp_logan.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     # Print out model parameters
     parallel_model.print_params()
 
     # ##########################
     # Perform VCD reconstruction
     time0 = time.time()
-    recon, fm_rmse = parallel_model.recon(sinogram, weights=weights)
+    recon, recon_params = parallel_model.recon(sinogram, weights=weights)
 
     recon.block_until_ready()
     elapsed = time.time() - time0
     print('Elapsed time for recon is {:.3f} seconds'.format(elapsed))
     # ##########################
 
     # Display results
```

### Comparing `mbirjax-0.1.0/docs/build/html/_static/new_model_template.py` & `mbirjax-0.2.0/docs/build/html/_static/new_model_template.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,22 @@
+import jax
 import jax.numpy as jnp
-from mbirjax import TomographyModel
+from functools import partial
+from collections import namedtuple
+from mbirjax import TomographyModel, ParameterHandler
 
 
 class TemplateModel(TomographyModel):
     """
     This is a template for a class designed to handle a particular geometry that extends the :ref:`TomographyModelDocs`.
     This class inherits all methods and properties from the :ref:`TomographyModelDocs` and may override some
     to suit the specific geometry.
 
+    Items to change for a particular geometry are highlighted with TODO.
+
     Args:
         sinogram_shape (tuple):
             Shape of the sinogram as a tuple in the form `(views, rows, channels)`, where 'views' is the number of
             different projection angles, 'rows' correspond to the number of detector rows, and 'channels' index columns of
             the detector that are assumed to be aligned with the rotation axis.
         param1, param2 (scalars):
             These are view-independent scalar parameters that are required for the geometry and are not already included in the parent class.
@@ -19,110 +24,163 @@
             These are view-dependent parameter vectors each with length = number of views.
         **kwargs (dict):
             Additional keyword arguments that are passed to the :ref:`TomographyModelDocs` constructor. These can
             include settings and configurations specific to the tomography model such as noise models or image dimensions.
             Refer to :ref:`TomographyModelDocs` documentation for a detailed list of possible parameters.
     """
 
+    # TODO: Adjust the signature as needed for a particular geometry and update the docstring to match.
     def __init__(self, sinogram_shape, param1, param2, view_dependent_vec1, view_dependent_vec2, **kwargs):
         # Convert the view-dependent vectors to an array
         view_dependent_vecs = [vec.flatten() for vec in [view_dependent_vec1, view_dependent_vec2]]
         try:
             view_params_array = jnp.stack(view_dependent_vecs, axis=1)
         except ValueError as e:
             raise ValueError("Incompatible view dependent vector lengths:  all view-dependent vectors must have the "
                              "same length.")
 
         super().__init__(sinogram_shape, param1=param1, param2=param2, view_params_array=view_params_array, **kwargs)
 
+    @classmethod
+    def from_file(cls, filename):
+        """
+        Construct a ConeBeamModel from parameters saved using save_params()
+
+        Args:
+            filename (str): Name of the file containing parameters to load.
+
+        Returns:
+            ConeBeamModel with the specified parameters.
+        """
+        # Load the parameters and convert view-dependent parameters to use the geometry-specific keywords.
+        params = ParameterHandler.load_param_dict(filename, values_only=True)
+        view_params_array = params['view_params_array']
+
+        # TODO: Adjust these to match the signature of __init__
+        view_dependent_vec1 = view_params_array[:, 0]
+        view_dependent_vec2 = view_params_array[:, 1]
+        del params['view_params_array']
+        return cls(view_dependent_vec1=view_dependent_vec1, view_dependent_vec2=view_dependent_vec2, **params)
+
     def get_magnification(self):
         """
         Compute the scale factor from a voxel at iso (at the origin on the center of rotation) to
         its projection on the detector.  For parallel beam, this is 1, but it may be parameter-dependent
         for other geometries.
 
         Returns:
             (float): magnification
         """
+        # TODO: Adjust as needed for the geometry.
         magnification = 1.0
         return magnification
 
     def verify_valid_params(self):
         """
         Check that all parameters are compatible for a reconstruction.
-        Extend to include any geometry-specific conditions.
         """
         super().verify_valid_params()
         sinogram_shape, view_params_array = self.get_params(['sinogram_shape', 'view_params_array'])
 
+        # TODO: Modify as needed for the geometry.
         if view_params_array.shape[0] != sinogram_shape[0]:
             error_message = "Number view dependent parameter vectors must equal the number of views. \n"
             error_message += "Got {} for length of view-dependent parameters and "
             error_message += "{} for number of views.".format(view_params_array.shape[0], sinogram_shape[0])
             raise ValueError(error_message)
 
     def get_geometry_parameters(self):
         """
-        Required function to get a list of the view independent geometry parameters required for projection.
+        Required function to get the view independent geometry parameters required for projection.
 
         Returns:
-            List of any parameters required for back_project_one_view_to_pixel_batch or forward_project_pixel_batch_to_one_view.
+            namedtuple of any parameters required for back_project_one_view_to_pixel_batch or forward_project_pixel_batch_to_one_view.
             This does not need to include view dependent parameters, or sinogram_shape or recon_shape, which
             are passed in automatically to projector_params.
         """
-        geometry_params = self.get_params(['delta_det_channel', 'det_channel_offset', 'delta_voxel'])
+        # TODO: Include additional names as needed for the projectors.
+        # First get the parameters managed by ParameterHandler
+        geometry_param_names = ['delta_det_channel', 'det_channel_offset', 'delta_voxel']
+        geometry_param_values = self.get_params(geometry_param_names)
+
+        # Then get additional parameters that are calculated separately, such as psf_radius and magnification.
+        # geometry_param_names += ['psf_radius']
+        # geometry_param_values.append(self.get_psf_radius())
+        # geometry_param_names += ['magnification']
+        # geometry_param_values.append(self.get_magnifiction())
+
+        # Then create a namedtuple to access parameters by name in a way that can be jit-compiled.
+        GeometryParams = namedtuple('GeometryParams', geometry_param_names)
+        geometry_params = GeometryParams(*tuple(geometry_param_values))
 
         return geometry_params
 
     def auto_set_recon_size(self, sinogram_shape, no_compile=True, no_warning=False):
         """Compute the default recon size using the internal parameters delta_channel and delta_pixel plus
           the number of channels from the sinogram"""
+        # TODO: provide code to implement this
         raise NotImplementedError('auto_set_recon_size must be implemented by each specific geometry model.')
 
     @staticmethod
-    def back_project_one_view_to_pixel_batch(sinogram_view, pixel_indices, single_view_params, projector_params, coeff_power=1):
+    @partial(jax.jit, static_argnames='projector_params')
+    def forward_project_pixel_batch_to_one_view(voxel_values, pixel_indices, single_view_params, projector_params):
         """
-        Calculate the backprojection value at a specified recon voxel cylinders given a sinogram view and various parameters.
+        Forward project a set of voxels determined by indices into a single view.
 
         NOTE: This function must be able to be jit-compiled.
 
         Args:
-            sinogram_view (2D jax array): one view of the sinogram to be back projected
-            pixel_indices (1D jax array of int):  indices into flattened array of size num_rows x num_cols.
-            single_view_params: These are the view dependent parameters for the view being back projected.
+            voxel_values (jax array):  2D array of shape (num_indices, num_slices) of voxel values, where
+                voxel_values[i, j] is the value of the voxel in slice j at the location determined by indices[i].
+            pixel_indices (jax array of int):  1D vector of indices into flattened array of size num_rows x num_cols.
+            single_view_params: These are the view dependent parameters for this view.
             projector_params (1D jax array): tuple of (sinogram_shape, recon_shape, get_geometry_params()).
-            coeff_power (int): backproject using the coefficients of (A_ij ** coeff_power).
-                Normally 1, but should be 2 when computing theta 2.
 
         Returns:
-            The voxel values for all slices at the input index (i.e., a voxel cylinder) obtained by backprojecting
-            the input sinogram view.
+            jax array of shape (num_det_rows, num_det_channels)
         """
-        # The number of slices will need to come from geometry_params
-        num_slices = 1
+        # Get all the geometry parameters - we use gp since geometry parameters is a named tuple and we'll access
+        # elements using, for example, gp.delta_det_channel, so a longer name would be clumsy.
+        gp = projector_params.geometry_params  # This is the namedtuple from get_geometry_parameters
+        num_views, num_det_rows, num_det_channels = projector_params.sinogram_shape
+        num_recon_rows, num_recon_columns, num_recon_slices = projector_params.recon_shape
 
-        # Computes the voxel values in all slices corresponding to pixel_index
-        voxel_values_cylinder = jnp.zeros(num_slices)
-        return voxel_values_cylinder
+        # Returns a single view of the sinogram
+        sinogram_view = jnp.zeros((num_det_rows, num_det_channels))
+
+        # TODO:  Provide code to implement forward projection
+
+        return sinogram_view
 
     @staticmethod
-    def forward_project_pixel_batch_to_one_view(voxel_values, pixel_indices, single_view_params, projector_params):
+    @partial(jax.jit, static_argnames='projector_params')
+    def back_project_one_view_to_pixel_batch(sinogram_view, pixel_indices, single_view_params, projector_params, coeff_power=1):
         """
-        Forward project a set of voxels determined by indices into a single view.
+        Calculate the backprojection value at a specified recon voxel cylinders given a sinogram view and various parameters.
 
         NOTE: This function must be able to be jit-compiled.
 
         Args:
-            voxel_values (jax array):  2D array of shape (num_indices, num_slices) of voxel values, where
-                voxel_values[i, j] is the value of the voxel in slice j at the location determined by indices[i].
-            pixel_indices (jax array of int):  1D vector of indices into flattened array of size num_rows x num_cols.
-            single_view_params: These are the view dependent parameters for this view.
+            sinogram_view (2D jax array): one view of the sinogram to be back projected
+            pixel_indices (1D jax array of int):  indices into flattened array of size num_rows x num_cols.
+            single_view_params: These are the view dependent parameters for the view being back projected.
             projector_params (1D jax array): tuple of (sinogram_shape, recon_shape, get_geometry_params()).
+            coeff_power (int): backproject using the coefficients of (A_ij ** coeff_power).
+                Normally 1, but should be 2 when computing theta 2.
 
         Returns:
-            jax array of shape (num_det_rows, num_det_channels)
+            The voxel values for all slices at the input index (i.e., a voxel cylinder) obtained by backprojecting
+            the input sinogram view.
         """
+        # Get all the geometry parameters - we use gp since geometry parameters is a named tuple and we'll access
+        # elements using, for example, gp.delta_det_channel, so a longer name would be clumsy.
+        gp = projector_params.geometry_params  # This is the namedtuple from get_geometry_parameters
+        num_views, num_det_rows, num_det_channels = projector_params.sinogram_shape
+        num_recon_rows, num_recon_columns, num_recon_slices = projector_params.recon_shape
 
-        # Returns a single view of the sinogram
-        sinogram_shape = projector_params[0]
-        sinogram_view = jnp.zeros(sinogram_shape[1:])
-        return sinogram_view
+        # Computes the voxel values in all slices corresponding to pixel_index
+        num_pixels = pixel_indices.shape[0]
+        voxel_values_cylinder = jnp.zeros((num_pixels, num_recon_slices))
+
+        # TODO:  Provide code to implement forward projection
+
+        return voxel_values_cylinder
```

### Comparing `mbirjax-0.1.0/docs/source/_static/new_model_template.py` & `mbirjax-0.2.0/docs/source/_static/new_model_template.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,22 @@
+import jax
 import jax.numpy as jnp
-from mbirjax import TomographyModel
+from functools import partial
+from collections import namedtuple
+from mbirjax import TomographyModel, ParameterHandler
 
 
 class TemplateModel(TomographyModel):
     """
     This is a template for a class designed to handle a particular geometry that extends the :ref:`TomographyModelDocs`.
     This class inherits all methods and properties from the :ref:`TomographyModelDocs` and may override some
     to suit the specific geometry.
 
+    Items to change for a particular geometry are highlighted with TODO.
+
     Args:
         sinogram_shape (tuple):
             Shape of the sinogram as a tuple in the form `(views, rows, channels)`, where 'views' is the number of
             different projection angles, 'rows' correspond to the number of detector rows, and 'channels' index columns of
             the detector that are assumed to be aligned with the rotation axis.
         param1, param2 (scalars):
             These are view-independent scalar parameters that are required for the geometry and are not already included in the parent class.
@@ -19,110 +24,163 @@
             These are view-dependent parameter vectors each with length = number of views.
         **kwargs (dict):
             Additional keyword arguments that are passed to the :ref:`TomographyModelDocs` constructor. These can
             include settings and configurations specific to the tomography model such as noise models or image dimensions.
             Refer to :ref:`TomographyModelDocs` documentation for a detailed list of possible parameters.
     """
 
+    # TODO: Adjust the signature as needed for a particular geometry and update the docstring to match.
     def __init__(self, sinogram_shape, param1, param2, view_dependent_vec1, view_dependent_vec2, **kwargs):
         # Convert the view-dependent vectors to an array
         view_dependent_vecs = [vec.flatten() for vec in [view_dependent_vec1, view_dependent_vec2]]
         try:
             view_params_array = jnp.stack(view_dependent_vecs, axis=1)
         except ValueError as e:
             raise ValueError("Incompatible view dependent vector lengths:  all view-dependent vectors must have the "
                              "same length.")
 
         super().__init__(sinogram_shape, param1=param1, param2=param2, view_params_array=view_params_array, **kwargs)
 
+    @classmethod
+    def from_file(cls, filename):
+        """
+        Construct a ConeBeamModel from parameters saved using save_params()
+
+        Args:
+            filename (str): Name of the file containing parameters to load.
+
+        Returns:
+            ConeBeamModel with the specified parameters.
+        """
+        # Load the parameters and convert view-dependent parameters to use the geometry-specific keywords.
+        params = ParameterHandler.load_param_dict(filename, values_only=True)
+        view_params_array = params['view_params_array']
+
+        # TODO: Adjust these to match the signature of __init__
+        view_dependent_vec1 = view_params_array[:, 0]
+        view_dependent_vec2 = view_params_array[:, 1]
+        del params['view_params_array']
+        return cls(view_dependent_vec1=view_dependent_vec1, view_dependent_vec2=view_dependent_vec2, **params)
+
     def get_magnification(self):
         """
         Compute the scale factor from a voxel at iso (at the origin on the center of rotation) to
         its projection on the detector.  For parallel beam, this is 1, but it may be parameter-dependent
         for other geometries.
 
         Returns:
             (float): magnification
         """
+        # TODO: Adjust as needed for the geometry.
         magnification = 1.0
         return magnification
 
     def verify_valid_params(self):
         """
         Check that all parameters are compatible for a reconstruction.
-        Extend to include any geometry-specific conditions.
         """
         super().verify_valid_params()
         sinogram_shape, view_params_array = self.get_params(['sinogram_shape', 'view_params_array'])
 
+        # TODO: Modify as needed for the geometry.
         if view_params_array.shape[0] != sinogram_shape[0]:
             error_message = "Number view dependent parameter vectors must equal the number of views. \n"
             error_message += "Got {} for length of view-dependent parameters and "
             error_message += "{} for number of views.".format(view_params_array.shape[0], sinogram_shape[0])
             raise ValueError(error_message)
 
     def get_geometry_parameters(self):
         """
-        Required function to get a list of the view independent geometry parameters required for projection.
+        Required function to get the view independent geometry parameters required for projection.
 
         Returns:
-            List of any parameters required for back_project_one_view_to_pixel_batch or forward_project_pixel_batch_to_one_view.
+            namedtuple of any parameters required for back_project_one_view_to_pixel_batch or forward_project_pixel_batch_to_one_view.
             This does not need to include view dependent parameters, or sinogram_shape or recon_shape, which
             are passed in automatically to projector_params.
         """
-        geometry_params = self.get_params(['delta_det_channel', 'det_channel_offset', 'delta_voxel'])
+        # TODO: Include additional names as needed for the projectors.
+        # First get the parameters managed by ParameterHandler
+        geometry_param_names = ['delta_det_channel', 'det_channel_offset', 'delta_voxel']
+        geometry_param_values = self.get_params(geometry_param_names)
+
+        # Then get additional parameters that are calculated separately, such as psf_radius and magnification.
+        # geometry_param_names += ['psf_radius']
+        # geometry_param_values.append(self.get_psf_radius())
+        # geometry_param_names += ['magnification']
+        # geometry_param_values.append(self.get_magnifiction())
+
+        # Then create a namedtuple to access parameters by name in a way that can be jit-compiled.
+        GeometryParams = namedtuple('GeometryParams', geometry_param_names)
+        geometry_params = GeometryParams(*tuple(geometry_param_values))
 
         return geometry_params
 
     def auto_set_recon_size(self, sinogram_shape, no_compile=True, no_warning=False):
         """Compute the default recon size using the internal parameters delta_channel and delta_pixel plus
           the number of channels from the sinogram"""
+        # TODO: provide code to implement this
         raise NotImplementedError('auto_set_recon_size must be implemented by each specific geometry model.')
 
     @staticmethod
-    def back_project_one_view_to_pixel_batch(sinogram_view, pixel_indices, single_view_params, projector_params, coeff_power=1):
+    @partial(jax.jit, static_argnames='projector_params')
+    def forward_project_pixel_batch_to_one_view(voxel_values, pixel_indices, single_view_params, projector_params):
         """
-        Calculate the backprojection value at a specified recon voxel cylinders given a sinogram view and various parameters.
+        Forward project a set of voxels determined by indices into a single view.
 
         NOTE: This function must be able to be jit-compiled.
 
         Args:
-            sinogram_view (2D jax array): one view of the sinogram to be back projected
-            pixel_indices (1D jax array of int):  indices into flattened array of size num_rows x num_cols.
-            single_view_params: These are the view dependent parameters for the view being back projected.
+            voxel_values (jax array):  2D array of shape (num_indices, num_slices) of voxel values, where
+                voxel_values[i, j] is the value of the voxel in slice j at the location determined by indices[i].
+            pixel_indices (jax array of int):  1D vector of indices into flattened array of size num_rows x num_cols.
+            single_view_params: These are the view dependent parameters for this view.
             projector_params (1D jax array): tuple of (sinogram_shape, recon_shape, get_geometry_params()).
-            coeff_power (int): backproject using the coefficients of (A_ij ** coeff_power).
-                Normally 1, but should be 2 when computing theta 2.
 
         Returns:
-            The voxel values for all slices at the input index (i.e., a voxel cylinder) obtained by backprojecting
-            the input sinogram view.
+            jax array of shape (num_det_rows, num_det_channels)
         """
-        # The number of slices will need to come from geometry_params
-        num_slices = 1
+        # Get all the geometry parameters - we use gp since geometry parameters is a named tuple and we'll access
+        # elements using, for example, gp.delta_det_channel, so a longer name would be clumsy.
+        gp = projector_params.geometry_params  # This is the namedtuple from get_geometry_parameters
+        num_views, num_det_rows, num_det_channels = projector_params.sinogram_shape
+        num_recon_rows, num_recon_columns, num_recon_slices = projector_params.recon_shape
 
-        # Computes the voxel values in all slices corresponding to pixel_index
-        voxel_values_cylinder = jnp.zeros(num_slices)
-        return voxel_values_cylinder
+        # Returns a single view of the sinogram
+        sinogram_view = jnp.zeros((num_det_rows, num_det_channels))
+
+        # TODO:  Provide code to implement forward projection
+
+        return sinogram_view
 
     @staticmethod
-    def forward_project_pixel_batch_to_one_view(voxel_values, pixel_indices, single_view_params, projector_params):
+    @partial(jax.jit, static_argnames='projector_params')
+    def back_project_one_view_to_pixel_batch(sinogram_view, pixel_indices, single_view_params, projector_params, coeff_power=1):
         """
-        Forward project a set of voxels determined by indices into a single view.
+        Calculate the backprojection value at a specified recon voxel cylinders given a sinogram view and various parameters.
 
         NOTE: This function must be able to be jit-compiled.
 
         Args:
-            voxel_values (jax array):  2D array of shape (num_indices, num_slices) of voxel values, where
-                voxel_values[i, j] is the value of the voxel in slice j at the location determined by indices[i].
-            pixel_indices (jax array of int):  1D vector of indices into flattened array of size num_rows x num_cols.
-            single_view_params: These are the view dependent parameters for this view.
+            sinogram_view (2D jax array): one view of the sinogram to be back projected
+            pixel_indices (1D jax array of int):  indices into flattened array of size num_rows x num_cols.
+            single_view_params: These are the view dependent parameters for the view being back projected.
             projector_params (1D jax array): tuple of (sinogram_shape, recon_shape, get_geometry_params()).
+            coeff_power (int): backproject using the coefficients of (A_ij ** coeff_power).
+                Normally 1, but should be 2 when computing theta 2.
 
         Returns:
-            jax array of shape (num_det_rows, num_det_channels)
+            The voxel values for all slices at the input index (i.e., a voxel cylinder) obtained by backprojecting
+            the input sinogram view.
         """
+        # Get all the geometry parameters - we use gp since geometry parameters is a named tuple and we'll access
+        # elements using, for example, gp.delta_det_channel, so a longer name would be clumsy.
+        gp = projector_params.geometry_params  # This is the namedtuple from get_geometry_parameters
+        num_views, num_det_rows, num_det_channels = projector_params.sinogram_shape
+        num_recon_rows, num_recon_columns, num_recon_slices = projector_params.recon_shape
 
-        # Returns a single view of the sinogram
-        sinogram_shape = projector_params[0]
-        sinogram_view = jnp.zeros(sinogram_shape[1:])
-        return sinogram_view
+        # Computes the voxel values in all slices corresponding to pixel_index
+        num_pixels = pixel_indices.shape[0]
+        voxel_values_cylinder = jnp.zeros((num_pixels, num_recon_slices))
+
+        # TODO:  Provide code to implement forward projection
+
+        return voxel_values_cylinder
```

### Comparing `mbirjax-0.1.0/docs/source/conf.py` & `mbirjax-0.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mbirjax-0.1.0/experiments/cone_beam_dev.py` & `mbirjax-0.2.0/experiments/cone_beam_dev.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,38 +10,42 @@
 
 if __name__ == "__main__":
     """
     This is a script to develop, debug, and tune the cone beam beam projector
     """
     # ##########################
     # Do all the setup
-    view_batch_size = 32
+    view_batch_size = 2  # Reduce this for large detector row/channel count, increase for smaller
     pixel_batch_size = 2048
 
-    # Initialize sinogram
+    # Initialize sinogram parameters
     num_views = 128
-    num_det_rows = 20
+    num_det_rows = 128
     num_det_channels = 128
+    view_step_size = None  # Set to a small, positive integer to subsample the views
+
+    view_indices = np.arange(start=0, stop=num_views, step=view_step_size)
 
     source_detector_distance = 4 * num_det_channels
     source_iso_distance = source_detector_distance
     delta_voxel = 1
-    start_angle = 0
-    extra_angle = 0  # jnp.atan2(magnification * num_det_channels / 2, source_detector_distance)
-    end_angle = jnp.pi + extra_angle
-    sinogram = jnp.zeros((num_views, num_det_rows, num_det_channels))
+    detector_cone_angle = 2 * np.arctan2(num_det_channels / 2, source_detector_distance)
+    start_angle = -(np.pi + detector_cone_angle) * (1/2)
+    end_angle = (np.pi + detector_cone_angle) * (1/2)
+
+    sinogram_shape = (num_views, num_det_rows, num_det_channels)
     angles = jnp.linspace(start_angle, jnp.pi, num_views, endpoint=False)
 
     # Initialize a random key
     seed_value = 0  #np.random.randint(1000000)
     key = jax.random.PRNGKey(seed_value)
 
     # Set up parallel beam model
     # conebeam_model = mbirjax.ConeBeamModel.from_file('params_conebeam.yaml')
-    conebeam_model = mbirjax.ConeBeamModel(sinogram.shape, angles, source_detector_distance, source_iso_distance)
+    conebeam_model = mbirjax.ConeBeamModel(sinogram_shape, angles, source_detector_distance, source_iso_distance)
     # conebeam_model.to_file('params_conebeam.yaml')
 
     # conebeam_model.set_params(delta_voxel=delta_voxel)
 
     # Generate phantom
     recon_shape = conebeam_model.get_params('recon_shape')
     num_recon_rows, num_recon_cols, num_recon_slices = recon_shape[:3]
@@ -49,84 +53,53 @@
 
     # Generate indices of pixels
     num_subsets = 1
     full_indices = mbirjax.gen_pixel_partition(recon_shape, num_subsets)
     num_subsets = 5
     subset_indices = mbirjax.gen_pixel_partition(recon_shape, num_subsets)
 
-    ###
-    # # Test vertical fan beam
-    #
-    # geometry_params = conebeam_model.get_geometry_parameters()
-    # sinogram_shape, recon_shape = conebeam_model.get_params(['sinogram_shape', 'recon_shape'])
-    # projector_params = (tuple(sinogram_shape), tuple(recon_shape), tuple(geometry_params))
-    # angle = angles[10]
-    # pixel_indices = full_indices[0][12000:12001]
-    # voxel_values = np.random.rand(1, recon_shape[2])
-    #
-    # projection1 = conebeam_model.forward_project_pixel_batch_to_one_view(voxel_values, pixel_indices, angle, projector_params)
-    # center = np.where(np.amax(projection1, axis=0) > 0)[0][1]
-    # projection1 = projection1[:, center]
-    # voxel_values = voxel_values.reshape(-1)
-    # projection2 = conebeam_model.forward_vertical_fan_one_pixel_to_one_view(voxel_values, pixel_indices, angle, projector_params)
-    # A = np.amax(np.abs(projection2 / projection1 - projection2[0] / projection1[0]))
-    # print(A)
-    ##
-
-    # # ##########################
-    # # Show the forward and back projection from a single pixel
-    # i, j = num_recon_rows // 4, num_recon_cols // 3
-    # x = jnp.zeros(recon_shape)
-    # x = x.at[i, j, :].set(1)
-    # voxel_values = x.reshape((-1, num_recon_slices))[full_indices[0]]
-    #
-    # Ax = conebeam_model.sparse_forward_project(voxel_values, full_indices[0])
-    # Ax = np.array(Ax)
-    # Aty = conebeam_model.sparse_back_project(Ax, full_indices[0])
-    # Aty = np.array(Aty)
-
     # Generate sinogram data
+    # mbirjax.slice_viewer(phantom)
     voxel_values = phantom.reshape((-1,) + recon_shape[2:])[full_indices]
 
     conebeam_model.set_params(view_batch_size=view_batch_size, pixel_batch_size=pixel_batch_size)
 
-    print('Starting forward projection')
-    sinogram = conebeam_model.sparse_forward_project(voxel_values[0][23:27], full_indices[0][23:27])
+    num_projected_views = len(view_indices) if len(view_indices) != 0 else num_views
+    print('Starting forward projection with {} views out of {} total'.format(num_projected_views, num_views))
+    view_subset_sinogram = conebeam_model.sparse_forward_project(voxel_values[0], full_indices[0], view_indices=view_indices)
+    # mbirjax.slice_viewer(view_subset_sinogram, slice_axis=0, slice_label='View')
 
     # Determine resulting number of views, slices, and channels and image size
-    print('Sinogram shape: {}'.format(sinogram.shape))
+    print('View subset sinogram shape: {}'.format(view_subset_sinogram.shape))
     print('Memory stats after forward projection')
-    mbirjax.get_gpu_memory_stats(print_results=True)
+    mbirjax.get_memory_stats(print_results=True)
 
     # Get the vector of indices
     indices = jnp.arange(num_recon_rows * num_recon_cols)
     num_trials = 3
     indices = jnp.mod(np.arange(num_trials, dtype=int).reshape((-1, 1)) + indices.reshape((1, -1)), num_recon_rows * num_recon_cols)
 
-    sinogram = jnp.array(sinogram)
-    indices = jnp.array(indices)
-
     # Run once to finish compiling
     print('Starting back projection')
-    bp = conebeam_model.sparse_back_project(sinogram, indices[0])
+    bp = conebeam_model.sparse_back_project(view_subset_sinogram, indices[0], view_indices=view_indices)
     print('Recon shape: ({}, {}, {})'.format(num_recon_rows, num_recon_cols, num_recon_slices))
     print('Memory stats after back projection')
-    mbirjax.get_gpu_memory_stats(print_results=True)
+    mbirjax.get_memory_stats(print_results=True)
     # ##########################
     # Test the adjoint property
     # Get a random 3D phantom to test the adjoint property
     key, subkey = jax.random.split(key)
     x = jax.random.uniform(subkey, shape=bp.shape)
     key, subkey = jax.random.split(key)
-    y = jax.random.uniform(subkey, shape=sinogram.shape)
+    y = jax.random.uniform(subkey, shape=view_subset_sinogram.shape)
 
     # Do a forward projection, then a backprojection
     voxel_values = x.reshape((-1, num_recon_slices))[indices[0]]
-    Ax = conebeam_model.sparse_forward_project(voxel_values, indices[0])
-    Aty = conebeam_model.sparse_back_project(y, indices[0])
+    Ax = conebeam_model.sparse_forward_project(voxel_values, indices[0], view_indices=view_indices)
+    Aty = conebeam_model.sparse_back_project(y, indices[0], view_indices=view_indices)
 
     # Calculate <Aty, x> and <y, Ax>
     Aty_x = jnp.sum(Aty * x)
     y_Ax = jnp.sum(y * Ax)
 
     adjoint_result = np.allclose(Aty_x, y_Ax)
     if adjoint_result:
@@ -138,27 +111,27 @@
     del Ax, Aty, bp
     del phantom
     del x, y
     gc.collect()
 
     # ##########################
     ## Test the hessian against a finite difference approximation ## #
-    hessian = conebeam_model.compute_hessian_diagonal()
+    hessian = conebeam_model.compute_hessian_diagonal(view_indices=view_indices)
 
     x = jnp.zeros(recon_shape)
     key, subkey = jax.random.split(key)
     i, j = jax.random.randint(subkey, shape=(2,), minval=0, maxval=num_recon_rows)
     key, subkey = jax.random.split(key)
     k = jax.random.randint(subkey, shape=(), minval=0, maxval=num_recon_slices)
 
     eps = 0.01
     x = x.at[i, j, k].set(eps)
     voxel_values = x.reshape((-1, num_recon_slices))[indices[0]]
-    Ax = conebeam_model.sparse_forward_project(voxel_values, indices[0])
-    AtAx = conebeam_model.sparse_back_project(Ax, indices[0]).reshape(x.shape)
+    Ax = conebeam_model.sparse_forward_project(voxel_values, indices[0], view_indices=view_indices)
+    AtAx = conebeam_model.sparse_back_project(Ax, indices[0], view_indices=view_indices).reshape(x.shape)
     finite_diff_hessian = AtAx[i, j, k] / eps
     hessian_result = jnp.allclose(hessian.reshape(x.shape)[i, j, k], finite_diff_hessian)
     if hessian_result:
         print('Hessian matches finite difference: {}'.format(hessian_result))
     else:
         warnings.warn('Hessian does not match finite difference.')
 
@@ -167,15 +140,15 @@
     #  NOTE: recompiling happens whenever sparse_forward_project is called with a new *length* of input indices
     time_taken = 0
 
     print('\nStarting multiple forward projections...')
     for j in range(num_trials):
         voxel_values = x.reshape((-1, num_recon_slices))[indices[j]]
         t0 = time.time()
-        fp = conebeam_model.sparse_forward_project(voxel_values, indices[j])
+        fp = conebeam_model.sparse_forward_project(voxel_values, indices[j], view_indices=view_indices)
         time_taken += time.time() - t0
         del fp
         gc.collect()
 
     print('Mean time per call = {}'.format(time_taken / num_trials))
     print('Done')
 
@@ -183,49 +156,46 @@
     # Check the time taken per backprojection
     #  NOTE: recompiling happens whenever sparse_back_project is called with a new *length* of input indices
     time_taken = 0
 
     print('\nStarting multiple backprojections...')
     for j in range(num_trials):
         t0 = time.time()
-        bp = conebeam_model.sparse_back_project(sinogram, indices[j])
+        bp = conebeam_model.sparse_back_project(view_subset_sinogram, indices[j], view_indices=view_indices)
         time_taken += time.time() - t0
         del bp
         gc.collect()
 
     print('Mean time per call = {}'.format(time_taken / num_trials))
     print('Done')
 
+    print('Memory stats after all multiple projections')
+    mbirjax.get_memory_stats(print_results=True)
+
     # ##########################
     # Show the forward and back projection from a single pixel
     i, j = num_recon_rows // 4, num_recon_cols // 3
     x = jnp.zeros(recon_shape)
     x = x.at[i, j, :].set(1)
     voxel_values = x.reshape((-1, num_recon_slices))[indices[0]]
 
-    Ax = conebeam_model.sparse_forward_project(voxel_values, indices[0])
-    Aty = conebeam_model.sparse_back_project(Ax, indices[0])
+    Ax = conebeam_model.sparse_forward_project(voxel_values, indices[0], view_indices=view_indices)
+    Aty = conebeam_model.sparse_back_project(Ax, indices[0], view_indices=view_indices)
     Aty = conebeam_model.reshape_recon(Aty)
 
-    y = jnp.zeros_like(sinogram)
-    view_index = 30
-    y = y.at[view_index].set(sinogram[view_index])
-    index = jnp.ravel_multi_index((6, 6), (num_recon_rows, num_recon_cols))
-    a1 = conebeam_model.sparse_back_project(y, indices[0])
-
     slice_index = (num_recon_slices + 1) // 2
     fig, ax = plt.subplots(nrows=1, ncols=3, figsize=(15, 5))
     cax = ax[0].imshow(x[:, :, slice_index])
     ax[0].set_title('x = phantom')
     fig.colorbar(cax, ax=ax[0])
     cax = ax[1].imshow(Ax[:, slice_index, :])
     ax[1].set_title('y = Ax')
     fig.colorbar(cax, ax=ax[1])
     cax = ax[2].imshow(Aty[:, :, slice_index])
     ax[2].set_title('Aty = AtAx')
     fig.colorbar(cax, ax=ax[2])
     plt.pause(2)
 
     print('Final memory stats:')
-    mbirjax.get_gpu_memory_stats(print_results=True)
+    mbirjax.get_memory_stats(print_results=True)
     input('Press return to exit')
     a = 0
```

### Comparing `mbirjax-0.1.0/experiments/cvpr-2024/vcd_figs_for_abst.py` & `mbirjax-0.2.0/experiments/cvpr-2024/vcd_figs_for_abst.py`

 * *Files 9% similar despite different names*

```diff
@@ -66,28 +66,31 @@
     granularity = np.array(parallel_model.get_params('granularity'))
 
     # Print out model parameters
     parallel_model.print_params()
 
     # ##########################
     # Perform VCD reconstruction
-    recon_vcd, fm_rmse_vcd = parallel_model.recon(sinogram, weights=weights)
+    recon_vcd, recon_params_vcd = parallel_model.recon(sinogram, weights=weights)
+    fm_rmse_vcd = recon_params_vcd.fm_rmse
     default_partition_sequence = parallel_model.get_params('partition_sequence')
     partition_sequence = mbirjax.gen_partition_sequence(default_partition_sequence, num_iterations=13)
     granularity_sequence_vcd = granularity[partition_sequence]
 
     # Perform GD reconstruction
     parallel_model.set_params(partition_sequence=[0,])
-    recon_gd, fm_rmse_gd = parallel_model.recon(sinogram, weights=weights)
+    recon_gd, recon_params_gd = parallel_model.recon(sinogram, weights=weights)
+    fm_rmse_gd = recon_params_gd.fm_rmse
     partition_sequence = mbirjax.gen_partition_sequence(partition_sequence, num_iterations=13)
     granularity_sequence_gd = granularity[partition_sequence]
 
     # Perform CD reconstruction
     parallel_model.set_params(partition_sequence=[3,])
-    recon_cd, fm_rmse_cd = parallel_model.recon(sinogram, weights=weights)
+    recon_cd, recon_params_cd = parallel_model.recon(sinogram, weights=weights)
+    fm_rmse_cd =recon_params_cd.fm_rmse
     partition_sequence = mbirjax.gen_partition_sequence(partition_sequence, num_iterations=13)
     granularity_sequence_cd = granularity[partition_sequence]
     # ##########################
 
 
     # Display reconstructions
     labels = ['Gradient Descent', 'Vectorized Coordinate Descent', 'Coordinate Descent']
```

### Comparing `mbirjax-0.1.0/experiments/gpu_performance/cumulative_memory.py` & `mbirjax-0.2.0/experiments/gpu_performance/cumulative_memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,18 +134,18 @@
     outer_values = [num_views, num_channels]
     inner_labels = ['# det rows', '# indices']
     inner_values = [num_det_rows, num_indices]
 
     vmin = -3.5
     vmax = 1.5
 
-    if mbirjax.get_gpu_memory_stats() is None:
+    if mbirjax.get_memory_stats() is None:
         raise EnvironmentError('This script is for gpu only.')
 
-    m1 = mbirjax.get_gpu_memory_stats()
+    m1 = mbirjax.get_memory_stats()
     max_avail_gb = m1[0]['bytes_limit'] / (1024 ** 3)
 
     # Make room for the data
     mem_values = np.zeros((len(num_views), len(num_channels), len(num_det_rows), len(num_indices)))
     time_values = np.zeros_like(mem_values)
 
     # Set up for projections
@@ -174,15 +174,15 @@
                     voxel_values = phantom.reshape((-1,) + recon_shape[2:])[indices]
 
                     if eval_type_index == 0:
 
                         print('Initial forward projection for memory: nv={}, nc={}, nr={}, ni={}'.format(nv, nc, nr, ni))
                         try:
                             sinogram = parallel_model.forward_project(voxel_values, indices)
-                            m1 = mbirjax.get_gpu_memory_stats()
+                            m1 = mbirjax.get_memory_stats()
                             peak_mem_gb = m1[0]['peak_bytes_in_use'] / (1024 ** 3)
                         except:
                             print('Out of memory')
                             peak_mem_gb = 1000 * max_avail_gb
                         mem_values[i, j, k, l] = peak_mem_gb
                         print('Peak GB used = {}'.format(peak_mem_gb))
 
@@ -202,15 +202,15 @@
                         try:
                             sinogram = parallel_model.forward_project(voxel_values, indices)
                         except:
                             print('Out of memory in forward projector')
                             sinogram = np.ones((nv, nr, nc))
                         try:
                             bp = parallel_model.back_project(sinogram, indices)
-                            m1 = mbirjax.get_gpu_memory_stats()
+                            m1 = mbirjax.get_memory_stats()
                             peak_mem_gb = m1[0]['peak_bytes_in_use'] / (1024 ** 3)
                         except:
                             print('Out of memory')
                             peak_mem_gb = 1000 * max_avail_gb
 
                         mem_values[i, j, k, l] = peak_mem_gb
                         print('Peak GB used = {}'.format(peak_mem_gb))
@@ -223,15 +223,15 @@
                             print('Out of memory on pass 2')
                         t1 = time.time()
                         time_diff_secs = t1 - t0
                         time_values[i, j, k, l] = time_diff_secs
                         print('Elapsed time = {}'.format(time_diff_secs))
 
 
-    m1 = mbirjax.get_gpu_memory_stats()
+    m1 = mbirjax.get_memory_stats()
     peak_mem_gb = m1[0]['peak_bytes_in_use'] / (1024 ** 3)
     max_percent_used_gb = 100 * peak_mem_gb / max_avail_gb
     print('Max percentage GB used = {}%'.format(max_percent_used_gb))
 
     mem_title = 'GB_secs used for ' + eval_types[eval_type_index]
     np.savez(mem_title, mem_values=mem_values, time_values=time_values, eval_type_index=np.array(eval_type_index),
              max_percent_used_gb=np.array(max_percent_used_gb),
```

### Comparing `mbirjax-0.1.0/experiments/gpu_performance/display_results.py` & `mbirjax-0.2.0/experiments/gpu_performance/display_results.py`

 * *Files identical despite different names*

### Comparing `mbirjax-0.1.0/experiments/gpu_performance/evaluate_over_indices.py` & `mbirjax-0.2.0/experiments/gpu_performance/evaluate_over_indices.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import jax.numpy as jnp
 import time
 import sys
 
 
 def evaluate_over_indices(filename, nv, nc, nr):
 
-    if mbirjax.get_gpu_memory_stats() is None:
+    if mbirjax.get_memory_stats() is None:
         raise EnvironmentError('This script is for gpu only.')
 
     # Load the existing data
     data = np.load(filename, allow_pickle=True)
     mem_values = data['mem_values']
     time_values = data['time_values']
     eval_type_index = data['eval_type_index']
@@ -50,15 +50,15 @@
         voxel_values = phantom.reshape((-1,) + recon_shape[2:])[indices]
 
         if eval_type_index == 0:
             print(
                 'Initial forward projection for memory: nv={}, nc={}, nr={}, ni={}'.format(nv, nc, nr, ni))
             try:
                 sinogram = parallel_model.sparse_forward_project(voxel_values, indices)
-                m1 = mbirjax.get_gpu_memory_stats()
+                m1 = mbirjax.get_memory_stats()
                 peak_mem_gb = m1[0]['peak_bytes_in_use'] / (1024 ** 3)
             except MemoryError as e:
                 print('Out of memory')
                 peak_mem_gb = 1000 * max_avail_gb
             mem_values[i, j, k, l] = peak_mem_gb
             print('Peak GB used = {}'.format(peak_mem_gb))
 
@@ -74,15 +74,15 @@
             print('Elapsed time = {}'.format(time_diff_secs))
 
         else:
             print('Initial back projection for memory: nv={}, nc={}, nr={}, ni={}'.format(nv, nc, nr, ni))
             sinogram = np.ones((nv, nr, nc))
             try:
                 bp = parallel_model.sparse_back_project(sinogram, indices)
-                m1 = mbirjax.get_gpu_memory_stats()
+                m1 = mbirjax.get_memory_stats()
                 peak_mem_gb = m1[0]['peak_bytes_in_use'] / (1024 ** 3)
             except MemoryError as e:
                 print('Out of memory')
                 peak_mem_gb = 1000 * max_avail_gb
 
             mem_values[i, j, k, l] = peak_mem_gb
             print('Peak GB used = {}'.format(peak_mem_gb))
```

### Comparing `mbirjax-0.1.0/experiments/gpu_performance/initialize_evaluation.py` & `mbirjax-0.2.0/experiments/gpu_performance/initialize_evaluation.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     eval_types = ['Forward_projection', 'Backward_projection']
 
     # Make room for the data
     mem_values = np.zeros((len(num_views), len(num_channels), len(num_det_rows), len(num_indices)))
     time_values = np.zeros_like(mem_values)
     max_percent_used_gb = 0
 
-    m1 = mbirjax.get_gpu_memory_stats()
+    m1 = mbirjax.get_memory_stats()
     max_avail_gb = m1[0]['bytes_limit'] / (1024 ** 3)
 
     filename = 'GB_secs_used_for_' + eval_types[eval_type_index]
     np.savez(filename, mem_values=mem_values, time_values=time_values, eval_type_index=np.array(eval_type_index),
              pixel_batch_size=np.array(pixel_batch_size),
              max_percent_used_gb=np.array(max_percent_used_gb), max_avail_gb=np.array(max_avail_gb),
              num_views=np.array(num_views), num_channels=np.array(num_channels),
```

### Comparing `mbirjax-0.1.0/experiments/parallel_model_dev.py` & `mbirjax-0.2.0/experiments/parallel_model_dev.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,30 +52,30 @@
 
     print('Starting forward projection')
     sinogram = parallel_model.sparse_forward_project(voxel_values[0], full_indices[0])
 
     # Determine resulting number of views, slices, and channels and image size
     print('Sinogram shape: {}'.format(sinogram.shape))
     print('Memory stats after forward projection')
-    mbirjax.get_gpu_memory_stats(print_results=True)
+    mbirjax.get_memory_stats(print_results=True)
 
     # Get the vector of indices
     indices = jnp.arange(num_recon_rows * num_recon_cols)
     num_trials = 3
     indices = jnp.mod(np.arange(num_trials, dtype=int).reshape((-1, 1)) + indices.reshape((1, -1)), num_recon_rows * num_recon_cols)
 
     sinogram = jnp.array(sinogram)
     indices = jnp.array(indices)
 
     # Run once to finish compiling
     print('Starting back projection')
     bp = parallel_model.sparse_back_project(sinogram, indices[0])
     print('Recon shape: ({}, {}, {})'.format(num_recon_rows, num_recon_cols, num_recon_slices))
     print('Memory stats after back projection')
-    mbirjax.get_gpu_memory_stats(print_results=True)
+    mbirjax.get_memory_stats(print_results=True)
     # ##########################
     # Test the adjoint property
     # Get a random 3D phantom to test the adjoint property
     key, subkey = jax.random.split(key)
     x = jax.random.uniform(subkey, shape=bp.shape)
     key, subkey = jax.random.split(key)
     y = jax.random.uniform(subkey, shape=sinogram.shape)
@@ -172,10 +172,10 @@
     ax[1].imshow(Ax[:, slice_index, :])
     ax[1].set_title('y = Ax')
     ax[2].imshow(Aty[:, :, slice_index])
     ax[2].set_title('Aty = AtAx')
     plt.pause(2)
 
     print('Final memory stats:')
-    mbirjax.get_gpu_memory_stats(print_results=True)
+    mbirjax.get_memory_stats(print_results=True)
     input('Press return to exit')
     a = 0
```

### Comparing `mbirjax-0.1.0/experiments/prox_test.py` & `mbirjax-0.2.0/experiments/prox_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     sinogram = parallel_model.forward_project(phantom)
 
     # Generate weights array
     weights = parallel_model.gen_weights(sinogram / sinogram.max(), weight_type='transmission_root')
 
     # Set reconstruction parameter values
     parallel_model.set_params(sharpness=sharpness, verbose=1)
-    # cone_model.set_params(positivity_flag=True)
+    # ct_model.set_params(positivity_flag=True)
 
     # Print out model parameters
     parallel_model.print_params()
 
     # ##########################
     # Test proximal map for fixed point
     # Run auto regularization. If auto_regularize_flag is False, then this will have no effect
```

### Comparing `mbirjax-0.1.0/mbirjax/_utils.py` & `mbirjax-0.2.0/mbirjax/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 _reconstruction_defaults_dict = {
     'auto_regularize_flag': {'val': True, 'recompile_flag': False},
     'positivity_flag': {'val': False, 'recompile_flag': False},
     'snr_db': {'val': 30.0, 'recompile_flag': False},
     'sharpness': {'val': 0.0, 'recompile_flag': False},
     'granularity': {'val': [1, 8, 64, 256], 'recompile_flag': False},
     'partition_sequence': {'val': [0, 1, 2, 3, 2, 3, 2, 3], 'recompile_flag': False},
-    'verbose': {'val': 0, 'recompile_flag': False},
+    'verbose': {'val': 1, 'recompile_flag': False},
     'pixel_batch_size': {'val': 2048, 'recompile_flag': True},  # TODO: Determine batch sizes dynamically.
-    'view_batch_size': {'val': 32, 'recompile_flag': True}
+    'view_batch_size': {'val': 4, 'recompile_flag': True}
 }
 
 # These headings should match the dictionaries
 headings = ['Forward model parameters', 'Recon parameters', 'Reconstruction parameters']
 
 dicts = [_forward_model_defaults_dict,
          _recon_model_defaults_dict,
```

### Comparing `mbirjax-0.1.0/mbirjax/cone_beam.py` & `mbirjax-0.2.0/mbirjax/cone_beam.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import warnings
-
 import jax
 import jax.numpy as jnp
 from functools import partial
+from collections import namedtuple
 from mbirjax import TomographyModel, ParameterHandler
 
 
 class ConeBeamModel(TomographyModel):
     """
     A class designed for handling forward and backward projections in a cone beam geometry, extending the
     :ref:`TomographyModelDocs`. This class offers specialized methods and parameters tailored for cone beam setups.
@@ -74,15 +73,18 @@
         """
         Returns the magnification for the cone beam geometry.
 
         Returns:
             magnification = source_detector_dist / source_iso_dist
         """
         source_detector_dist, source_iso_dist = self.get_params(['source_detector_dist', 'source_iso_dist'])
-        magnification = source_detector_dist / source_iso_dist
+        if jnp.isinf(source_detector_dist):
+            magnification = 1
+        else:
+            magnification = source_detector_dist / source_iso_dist
         return magnification
 
     def verify_valid_params(self):
         """
         Check that all parameters are compatible for a reconstruction.
 
         Note:
@@ -103,41 +105,50 @@
         #     raise ValueError("Invalid geometry: Recon volume extends too close to source.")
 
     def get_geometry_parameters(self):
         """
         Function to get a list of the primary geometry parameters for cone beam projection.
 
         Returns:
-            List of required geometry parameters.
+            namedtuple of required geometry parameters.
         """
-        geometry_params = self.get_params(
+        # First get the parameters managed by ParameterHandler
+        geometry_param_names = \
             ['delta_det_row', 'delta_det_channel', 'det_row_offset', 'det_channel_offset', 'det_rotation',
-             'source_detector_dist', 'delta_voxel', 'recon_slice_offset'])
-        geometry_params.append(self.get_magnification())
+             'source_detector_dist', 'delta_voxel', 'recon_slice_offset']
+        geometry_param_values = self.get_params(geometry_param_names)
 
-        # Append psf_radius to list of geometry params
-        psf_radius = self.get_psf_radius()
-        geometry_params.append(psf_radius)
+        # Then get additional parameters:
+        geometry_param_names += ['magnification', 'psf_radius']
+        geometry_param_values.append(self.get_magnification())
+        geometry_param_values.append(self.get_psf_radius())
+
+        # Then create a namedtuple to access parameters by name in a way that can be jit-compiled.  
+        GeometryParams = namedtuple('GeometryParams', geometry_param_names)
+        geometry_params = GeometryParams(*tuple(geometry_param_values))
 
         return geometry_params
 
     def get_psf_radius(self):
         """Computes the integer radius of the PSF kernel for cone beam projection.
         """
         delta_det_row, delta_det_channel, source_detector_dist, recon_shape, delta_voxel = self.get_params(
             ['delta_det_row', 'delta_det_channel', 'source_detector_dist', 'recon_shape', 'delta_voxel'])
         magnification = self.get_magnification()
 
         # Compute minimum detector pitch
         delta_det = jnp.minimum(delta_det_row, delta_det_channel)
 
         # Compute maximum magnification
-        source_to_iso_dist = source_detector_dist/magnification
-        source_to_closest_pixel = source_to_iso_dist - jnp.maximum(recon_shape[0], recon_shape[1])*delta_voxel
-        max_magnification = source_detector_dist/source_to_closest_pixel
+        if jnp.isinf(source_detector_dist):
+            max_magnification = 1
+        else:
+            source_to_iso_dist = source_detector_dist/magnification
+            source_to_closest_pixel = source_to_iso_dist - jnp.maximum(recon_shape[0], recon_shape[1])*delta_voxel
+            max_magnification = source_detector_dist/source_to_closest_pixel
 
         # Compute the maximum number of detector rows/channels on either side of the center detector hit by a voxel
         psf_radius = int(jnp.ceil(jnp.ceil((delta_voxel*max_magnification/delta_det))/2))
 
         return psf_radius
 
     def auto_set_recon_size(self, sinogram_shape, no_compile=True, no_warning=False):
@@ -152,29 +163,30 @@
         num_recon_cols = num_recon_rows
         num_recon_slices = int(jnp.round(num_det_rows * ((delta_det_row / delta_voxel) / magnification)))
 
         recon_shape = (num_recon_rows, num_recon_cols, num_recon_slices)
         self.set_params(no_compile=no_compile, no_warning=no_warning, recon_shape=recon_shape)
 
     @staticmethod
+    @partial(jax.jit, static_argnames='projector_params')
     def forward_project_pixel_batch_to_one_view(voxel_values, pixel_indices, angle, projector_params):
         """
         Forward project a set of voxels determined by indices into the flattened array of size num_rows x num_cols.
 
         Args:
             voxel_values (jax array):  2D array of shape (num_indices, num_slices) of voxel values, where
                 voxel_values[i, j] is the value of the voxel in slice j at the location determined by indices[i].
             pixel_indices (jax array of int):  1D vector of indices into flattened array of size num_rows x num_cols.
             angle (float):  Angle for this view
-            projector_params (tuple):  tuple of (sinogram_shape, recon_shape, get_geometry_params())
+            projector_params (namedtuple):  tuple of (sinogram_shape, recon_shape, get_geometry_params())
 
         Returns:
             jax array of shape (num_det_rows, num_det_channels)
         """
-        recon_shape = projector_params[1]
+        recon_shape = projector_params.recon_shape
         num_recon_slices = recon_shape[2]
         if voxel_values.shape[0] != pixel_indices.shape[0] or len(voxel_values.shape) < 2 or \
                 voxel_values.shape[1] != num_recon_slices:
             raise ValueError('voxel_values must have shape[0:2] = (num_indices, num_slices)')
 
         vertical_fan_projector = ConeBeamModel.forward_vertical_fan_pixel_batch_to_one_view
         horizontal_fan_projector = ConeBeamModel.forward_horizontal_fan_pixel_batch_to_one_view
@@ -194,388 +206,374 @@
 
         Args:
             voxel_values (jax array):  2D array of shape (num_pixels, num_recon_slices) of voxel values, where
                 voxel_values[i, j] is the value of the voxel in slice j at the location determined by indices[i].
             pixel_indices (jax array of int):  1D vector of shape (len(pixel_indices), ) holding the indices into
                 the flattened array of size num_rows x num_cols.
             angle (float):  Angle for this view
-            projector_params (tuple):  tuple of (sinogram_shape, recon_shape, get_geometry_params())
+            projector_params (namedtuple):  tuple of (sinogram_shape, recon_shape, get_geometry_params())
 
         Returns:
             jax array of shape (num_pixels, num_det_rows)
         """
         pixel_map = jax.vmap(ConeBeamModel.forward_vertical_fan_one_pixel_to_one_view,
                              in_axes=(0, 0, None, None))
         new_pixels = pixel_map(voxel_values, pixel_indices, angle, projector_params)
 
         return new_pixels
 
     @staticmethod
-    @partial(jax.jit, static_argnames='projector_params')
     def forward_horizontal_fan_pixel_batch_to_one_view(voxel_values, pixel_indices, angle, projector_params):
         """
         Apply a horizontal fan beam transformation to a set of voxel cylinders. These cylinders are assumed to have
         slices aligned with detector rows, so that a horizontal fan beam maps a cylinder slice to a detector row.
         This function returns the resulting sinogram view.
 
         Args:
             voxel_values (jax array):  2D array of shape (num_pixels, num_recon_slices) of voxel values, where
                 voxel_values[i, j] is the value of the voxel in slice j at the location determined by indices[i].
             pixel_indices (jax array of int):  1D vector of shape (len(pixel_indices), ) holding the indices into
                 the flattened array of size num_rows x num_cols.
             angle (float):  Angle for this view
-            projector_params (tuple):  tuple of (sinogram_shape, recon_shape, get_geometry_params())
+            projector_params (namedtuple):  tuple of (sinogram_shape, recon_shape, get_geometry_params())
 
         Returns:
             jax array of shape (num_det_rows, num_det_channels)
         """
 
-        # Get all the geometry parameters
-        geometry_params = projector_params[2]
-        (delta_det_channel, delta_det_row, det_channel_offset, det_row_offset, det_rotation, source_detector_dist,
-         delta_voxel, recon_slice_offset, magnification, psf_radius) = geometry_params
-        num_views, num_det_rows, num_det_channels = projector_params[0]
+        # Get all the geometry parameters - we use gp since geometry parameters is a named tuple and we'll access
+        # elements using, for example, gp.delta_det_channel, so a longer name would be clumsy.
+        gp = projector_params.geometry_params
+        num_views, num_det_rows, num_det_channels = projector_params.sinogram_shape
 
         # Get the data needed for horizontal projection
         n_p, n_p_center, W_p_c, cos_alpha_p_xy = ConeBeamModel.compute_horizontal_data(pixel_indices, angle, projector_params)
         L_max = jnp.minimum(1, W_p_c)
 
         # Allocate the sinogram array
         sinogram_view = jnp.zeros((num_det_rows, num_det_channels))
 
         # Define the horizontal projector, which will be vmapped over slices.
         def project_slice(sinogram_view_row, voxel_values_slice):
-            for n_offset in jnp.arange(start=-psf_radius, stop=psf_radius+1):
+            for n_offset in jnp.arange(start=-gp.psf_radius, stop=gp.psf_radius+1):
                 n = n_p_center + n_offset
                 abs_delta_p_c_n = jnp.abs(n_p - n)
                 L_p_c_n = jnp.clip((W_p_c + 1) / 2 - abs_delta_p_c_n, 0, L_max)
-                A_chan_n = delta_voxel * L_p_c_n / cos_alpha_p_xy
+                A_chan_n = gp.delta_voxel * L_p_c_n / cos_alpha_p_xy
                 A_chan_n *= (n >= 0) * (n < num_det_channels)
                 sinogram_view_row = sinogram_view_row.at[n].add(A_chan_n * voxel_values_slice)
 
             return sinogram_view_row
 
         sinogram_view = jax.vmap(project_slice, in_axes=(0, 1))(sinogram_view, voxel_values)
 
         return sinogram_view
 
     @staticmethod
-    @partial(jax.jit, static_argnames='projector_params')
     def forward_vertical_fan_one_pixel_to_one_view(voxel_values, pixel_index, angle, projector_params):
         """
         Apply a fan beam forward projection in the vertical direction to the pixel determined by indices
         into the flattened array of size num_rows x num_cols.  This returns a vector obtained from the projection of
         the original voxel cylinder onto a detector column, so the output vector has length num_det_rows.
 
         Args:
             voxel_values (jax array):  2D array of shape (num_pixels, num_recon_slices) of voxel values, where
                 voxel_values[i, j] is the value of the voxel in slice j at the location determined by indices[i].
             pixel_index (int):  Index into the flattened array of size num_rows x num_cols.
             angle (float):  Angle for this view.
-            projector_params (tuple):  tuple of (sinogram_shape, recon_shape, get_geometry_params())
+            projector_params (namedtuple):  tuple of (sinogram_shape, recon_shape, get_geometry_params())
 
         Returns:
             jax array of shape (num_pixels, num_det_rows)
 
         Note:
             This is a helper function used in vmap in :meth:`ConeBeamModel.forward_vertical_fan_pixel_batch_to_one_view`
         This method has the same signature and output as that method, except single int pixel_index is used
         in place of the 1D pixel_indices, and likewise only a single voxel cylinder is returned.
         """
-        # Get all the geometry parameters
-        geometry_params = projector_params[2]
-        (delta_det_channel, delta_det_row, det_channel_offset, det_row_offset, det_rotation, source_detector_dist,
-         delta_voxel, recon_slice_offset, magnification, psf_radius) = geometry_params
-        num_views, num_det_rows, num_det_channels = projector_params[0]
+        # Get all the geometry parameters - we use gp since geometry parameters is a named tuple and we'll access
+        # elements using, for example, gp.delta_det_channel, so a longer name would be clumsy.
+        gp = projector_params.geometry_params
+        num_views, num_det_rows, num_det_channels = projector_params.sinogram_shape
 
         # Get the data needed for vertical projection
         m_p, m_p_center, W_p_r, cos_alpha_p_z = ConeBeamModel.compute_vertical_data_single_pixel(pixel_index, angle,
                                                                                                  projector_params)
         L_max = jnp.minimum(1, W_p_r)
 
         # Allocate the output cylinder
         new_voxel_cylinder = jnp.zeros(num_det_rows)
 
         # Do the vertical projection
-        for m_offset in jnp.arange(start=-psf_radius, stop=psf_radius+1):
+        for m_offset in jnp.arange(start=-gp.psf_radius, stop=gp.psf_radius+1):
             m = m_p_center + m_offset
             abs_delta_p_r_m = jnp.abs(m_p - m)
             L_p_r_m = jnp.clip((W_p_r + 1) / 2 - abs_delta_p_r_m, 0, L_max)
             A_row_m = L_p_r_m / cos_alpha_p_z
             A_row_m *= (m >= 0) * (m < num_det_rows)
             new_voxel_cylinder = new_voxel_cylinder.at[m].add(A_row_m * voxel_values)
 
         return new_voxel_cylinder
 
     @staticmethod
+    @partial(jax.jit, static_argnames='projector_params')
     def back_project_one_view_to_pixel_batch(sinogram_view, pixel_indices, single_view_params, projector_params, coeff_power=1):
         """
         Use vmap to do a backprojection from one view to multiple pixels (voxel cylinders).
 
         Args:
             sinogram_view (2D jax array): one view of the sinogram to be back projected.
                 2D jax array of shape (num_det_rows)x(num_det_channels)
             pixel_indices (1D jax array of int):  indices into flattened array of size num_rows x num_cols.
             single_view_params: These are the view dependent parameters for the view being back projected.
-            projector_params (tuple): tuple of (sinogram_shape, recon_shape, get_geometry_params()).
+            projector_params (namedtuple): tuple of (sinogram_shape, recon_shape, get_geometry_params()).
             coeff_power (int): backproject using the coefficients of (A_ij ** coeff_power).
                 Normally 1, but should be 2 when computing Hessian diagonal.
 
         Returns:
             The voxel values for all slices at the input index (i.e., a voxel cylinder) obtained by backprojecting
             the input sinogram view.
         """
 
-        vertical_fan_projector = ConeBeamModel.back_vertical_fan_pixel_batch_to_one_view
-        horizontal_fan_projector = ConeBeamModel.back_horizontal_fan_pixel_batch_to_one_view
+        vertical_fan_projector = ConeBeamModel.back_vertical_fan_one_view_to_pixel_batch
+        horizontal_fan_projector = ConeBeamModel.back_horizontal_fan_one_view_to_pixel_batch
 
         det_voxel_cylinder = horizontal_fan_projector(sinogram_view, pixel_indices, single_view_params,
                                                       projector_params, coeff_power=coeff_power)
         back_projection = vertical_fan_projector(det_voxel_cylinder, pixel_indices, single_view_params,
                                                  projector_params, coeff_power=coeff_power)
 
         return back_projection
 
     @staticmethod
-    @partial(jax.jit, static_argnames='projector_params')
-    def back_horizontal_fan_pixel_batch_to_one_view(sinogram_view, pixel_indices, angle,
+    def back_horizontal_fan_one_view_to_pixel_batch(sinogram_view, pixel_indices, angle,
                                                     projector_params, coeff_power=1):
         """
         Apply the back projection of a horizontal fan beam transformation to a single sinogram view
         and return the resulting voxel cylinders.
 
         Args:
             sinogram_view (2D jax array): one view of the sinogram to be back projected.
                 2D jax array of shape (num_det_rows)x(num_det_channels)
             pixel_indices (1D jax array of int):  indices into flattened array of size num_rows x num_cols.
             angle (float): The projection angle in radians for this view.
-            projector_params (tuple): tuple of (sinogram_shape, recon_shape, get_geometry_params()).
+            projector_params (namedtuple): tuple of (sinogram_shape, recon_shape, get_geometry_params()).
             coeff_power (int): backproject using the coefficients of (A_ij ** coeff_power).
                 Normally 1, but should be 2 when computing Hessian diagonal.
         Returns:
-
+            jax array of shape (len(pixel_indices), num_det_rows)
         """
+        # Get all the geometry parameters - we use gp since geometry parameters is a named tuple and we'll access
+        # elements using, for example, gp.delta_det_channel, so a longer name would be clumsy.
+        gp = projector_params.geometry_params
 
-        # Get all the geometry parameters
-        geometry_params = projector_params[2]
-        (delta_det_channel, delta_det_row, det_channel_offset, det_row_offset, det_rotation, source_detector_dist,
-         delta_voxel, recon_slice_offset, magnification, psf_radius) = geometry_params
-
-        num_views, num_det_rows, num_det_channels = projector_params[0]
+        num_views, num_det_rows, num_det_channels = projector_params.sinogram_shape
         num_pixels = pixel_indices.shape[0]
 
         # Get the data needed for horizontal projection
         n_p, n_p_center, W_p_c, cos_alpha_p_xy = ConeBeamModel.compute_horizontal_data(pixel_indices, angle, projector_params)
         L_max = jnp.minimum(1, W_p_c)
 
         # Allocate the voxel cylinder array
         det_voxel_cylinder = jnp.zeros((num_pixels, num_det_rows))
 
         # Define the horizontal projector, which will be vmapped over slices.
         def project_slice(det_voxel_row, sinogram_view_row):
-            for n_offset in jnp.arange(start=-psf_radius, stop=psf_radius+1):
+            for n_offset in jnp.arange(start=-gp.psf_radius, stop=gp.psf_radius+1):
                 n = n_p_center + n_offset
                 abs_delta_p_c_n = jnp.abs(n_p - n)
                 L_p_c_n = jnp.clip((W_p_c + 1) / 2 - abs_delta_p_c_n, 0, L_max)
-                A_chan_n = delta_voxel * L_p_c_n / cos_alpha_p_xy
+                A_chan_n = gp.delta_voxel * L_p_c_n / cos_alpha_p_xy
                 A_chan_n *= (n >= 0) * (n < num_det_channels)
                 A_chan_n = A_chan_n ** coeff_power
                 det_voxel_row = jnp.add(det_voxel_row, A_chan_n * sinogram_view_row[n])
 
             return det_voxel_row
 
         det_voxel_cylinder = jax.vmap(project_slice, in_axes=(1, 0), out_axes=1)(det_voxel_cylinder, sinogram_view)
 
         return det_voxel_cylinder
 
     @staticmethod
-    @partial(jax.jit, static_argnames='projector_params')
-    def back_vertical_fan_pixel_batch_to_one_view(det_voxel_cylinder, pixel_indices, single_view_params,
+    def back_vertical_fan_one_view_to_pixel_batch(det_voxel_cylinder, pixel_indices, single_view_params,
                                                   projector_params, coeff_power=1):
         """
         Apply a fan beam backward projection in the vertical direction to the pixel determined by indices
         into the flattened array of size num_rows x num_cols.  This returns a vector obtained from the projection of
         the detector-based voxel cylinders onto voxel cylinders in recon space, so the output vector has length
         num_recon_slices.
 
         Args:
             det_voxel_cylinder (2D jax array): 2D array of shape (num_pixels, num_det_rows) of voxel values, where
                 det_voxel_cylinder[i, j] is the value of the voxel in row j at the location determined by indices[i].
             pixel_indices (1D jax array of int):  indices into flattened array of size num_rows x num_cols.
             single_view_params: These are the view dependent parameters for the view being back projected.
-            projector_params (tuple): tuple of (sinogram_shape, recon_shape, get_geometry_params()).
+            projector_params (namedtuple): tuple of (sinogram_shape, recon_shape, get_geometry_params()).
             coeff_power (int): backproject using the coefficients of (A_ij ** coeff_power).
                 Normally 1, but should be 2 when computing Hessian diagonal.
 
         Returns:
             2D jax array of shape (num_pixels, num_recon_slices) of voxel values.
         """
-        pixel_map = jax.vmap(ConeBeamModel.back_vertical_fan_one_pixel_one_view,
+        pixel_map = jax.vmap(ConeBeamModel.back_vertical_fan_one_view_to_one_pixel,
                              in_axes=(0, 0, None, None, None))
         new_pixels = pixel_map(det_voxel_cylinder, pixel_indices, single_view_params, projector_params, coeff_power)
 
         return new_pixels
 
     @staticmethod
-    @partial(jax.jit, static_argnames='projector_params')
-    def back_vertical_fan_one_pixel_one_view(detector_column_values, pixel_index, angle, projector_params,
-                                             coeff_power=1):
+    def back_vertical_fan_one_view_to_one_pixel(detector_column_values, pixel_index, angle, projector_params,
+                                                coeff_power=1):
         """
         Apply the back projection of a vertical fan beam transformation to a single voxel cylinder and return the column
         vector of the resulting values.
 
         Args:
             detector_column_values (1D jax array): 1D array of shape (num_det_rows,) of voxel values, where
                 detector_column_values[i, j] is the value of the voxel in row j at the location determined by indices[i].
             pixel_index (int):  Index into flattened array of size num_rows x num_cols.
             angle (float): The projection angle in radians for this view.
-            projector_params (tuple): tuple of (sinogram_shape, recon_shape, get_geometry_params()).
+            projector_params (namedtuple): tuple of (sinogram_shape, recon_shape, get_geometry_params()).
             coeff_power (int): backproject using the coefficients of (A_ij ** coeff_power).
                 Normally 1, but should be 2 when computing Hessian diagonal.
 
         Returns:
             1D jax array of shape (num_recon_slices,) of voxel values.
         """
-        # Get all the geometry parameters
-        geometry_params = projector_params[2]
-        (delta_det_channel, delta_det_row, det_channel_offset, det_row_offset, det_rotation, source_detector_dist,
-         delta_voxel, recon_slice_offset, magnification, psf_radius) = geometry_params
-        num_views, num_det_rows, num_det_channels = projector_params[0]
-        recon_shape = projector_params[1]
+        # Get all the geometry parameters - we use gp since geometry parameters is a named tuple and we'll access
+        # elements using, for example, gp.delta_det_channel, so a longer name would be clumsy.
+        gp = projector_params.geometry_params
+
+        num_views, num_det_rows, num_det_channels = projector_params.sinogram_shape
+        recon_shape = projector_params.recon_shape
         num_recon_rows, num_recon_cols, num_recon_slices = recon_shape
 
         # Get the data needed for vertical projection
         m_p, m_p_center, W_p_r, cos_alpha_p_z = ConeBeamModel.compute_vertical_data_single_pixel(pixel_index, angle,
                                                                                                  projector_params)
         L_max = jnp.minimum(1, W_p_r)
 
         # Allocate space
         recon_voxel_cylinder = jnp.zeros(num_recon_slices)
 
         # Do the vertical projection for this pixel.
-        for m_offset in jnp.arange(start=-psf_radius, stop=psf_radius+1):
+        for m_offset in jnp.arange(start=-gp.psf_radius, stop=gp.psf_radius+1):
             m = m_p_center + m_offset
             abs_delta_p_r_m = jnp.abs(m_p - m)
             L_p_r_m = jnp.clip((W_p_r + 1) / 2 - abs_delta_p_r_m, 0, L_max)
             A_row_m = L_p_r_m / cos_alpha_p_z
             A_row_m *= (m >= 0) * (m < num_det_rows)
             A_row_m = A_row_m ** coeff_power
             recon_voxel_cylinder = jnp.add(recon_voxel_cylinder, A_row_m * detector_column_values[m])
 
         return recon_voxel_cylinder
 
     @staticmethod
-    @partial(jax.jit, static_argnames='projector_params')
     def compute_vertical_data_single_pixel(pixel_index, angle, projector_params):
         """
         Compute the quantities m_p, m_p_center, W_p_r, cos_alpha_p_z needed for vertical projection.
 
         Args:
             pixel_index (int):  Index into flattened array of size num_rows x num_cols.
             angle (float): The projection angle in radians for this view.
-            projector_params (tuple): tuple of (sinogram_shape, recon_shape, get_geometry_params()).
+            projector_params (namedtuple): tuple of (sinogram_shape, recon_shape, get_geometry_params()).
 
         Returns:
             m_p, m_p_center, W_p_r, cos_alpha_p_z
         """
+        # Get all the geometry parameters - we use gp since geometry parameters is a named tuple and we'll access
+        # elements using, for example, gp.delta_det_channel, so a longer name would be clumsy.
+        gp = projector_params.geometry_params
 
-        # Get all the geometry parameters
-        geometry_params = projector_params[2]
-        (delta_det_channel, delta_det_row, det_channel_offset, det_row_offset, det_rotation, source_detector_dist,
-         delta_voxel, recon_slice_offset, magnification, psf_radius) = geometry_params
-
-        num_views, num_det_rows, num_det_channels = projector_params[0]
-        recon_shape = projector_params[1]
+        num_views, num_det_rows, num_det_channels = projector_params.sinogram_shape
+        recon_shape = projector_params.recon_shape
         num_recon_rows, num_recon_cols, num_recon_slices = recon_shape
 
         # Convert the index into (i,j,k) coordinates corresponding to the indices into the 3D voxel array
         row_index, col_index = jnp.unravel_index(pixel_index, recon_shape[:2])
         slice_index = jnp.arange(num_recon_slices)
 
-        x_p, y_p, z_p = ConeBeamModel.recon_ijk_to_xyz(row_index, col_index, slice_index, delta_voxel,
-                                                       recon_shape, recon_slice_offset, angle)
+        x_p, y_p, z_p = ConeBeamModel.recon_ijk_to_xyz(row_index, col_index, slice_index, gp.delta_voxel,
+                                                       recon_shape, gp.recon_slice_offset, angle)
 
         # Convert from xyz to coordinates on detector
-        u_p, v_p, pixel_mag = ConeBeamModel.geometry_xyz_to_uv_mag(x_p, y_p, z_p, source_detector_dist, magnification)
+        u_p, v_p, pixel_mag = ConeBeamModel.geometry_xyz_to_uv_mag(x_p, y_p, z_p, gp.source_detector_dist, gp.magnification)
         # Convert from uv to index coordinates in detector and get the vector of center detector rows for this cylinder
-        m_p, _ = ConeBeamModel.detector_uv_to_mn(u_p, v_p, delta_det_channel, delta_det_row, det_channel_offset,
-                                                 det_row_offset, num_det_rows, num_det_channels, det_rotation)
+        m_p, _ = ConeBeamModel.detector_uv_to_mn(u_p, v_p, gp.delta_det_channel, gp.delta_det_row, gp.det_channel_offset,
+                                                 gp.det_row_offset, num_det_rows, num_det_channels, gp.det_rotation)
         m_p_center = jnp.round(m_p).astype(int)
 
         # Compute vertical cone angle of pixel
-        phi_p = jnp.arctan2(v_p, source_detector_dist)
+        phi_p = jnp.arctan2(v_p, gp.source_detector_dist)
 
         # Compute cos alpha for row and columns
         cos_phi_p = jnp.cos(phi_p)
         cos_alpha_p_z = jnp.maximum(jnp.abs(cos_phi_p), jnp.abs(jnp.sin(phi_p)))
 
         # Get the length of projection of flattened voxel on detector (in fraction of detector size)
-        W_p_r = pixel_mag * (delta_voxel / delta_det_row) * cos_alpha_p_z / cos_phi_p
+        W_p_r = pixel_mag * (gp.delta_voxel / gp.delta_det_row) * cos_alpha_p_z / cos_phi_p
 
         vertical_data = (m_p, m_p_center, W_p_r, cos_alpha_p_z)
 
         return vertical_data
 
     @staticmethod
-    @partial(jax.jit, static_argnames='projector_params')
     def compute_horizontal_data(pixel_indices, angle, projector_params):
         """
         Compute the quantities n_p, n_p_center, W_p_c, cos_alpha_p_xy needed for vertical projection.
 
         Args:
             pixel_indices (1D jax array of int):  indices into flattened array of size num_rows x num_cols.
             angle (float): The projection angle in radians for this view.
-            projector_params (tuple): tuple of (sinogram_shape, recon_shape, get_geometry_params()).
+            projector_params (namedtuple): tuple of (sinogram_shape, recon_shape, get_geometry_params()).
 
         Returns:
             n_p, n_p_center, W_p_c, cos_alpha_p_xy
         """
+        # Get all the geometry parameters - we use gp since geometry parameters is a named tuple and we'll access
+        # elements using, for example, gp.delta_det_channel, so a longer name would be clumsy.
+        gp = projector_params.geometry_params
 
-        # Get all the geometry parameters
-        geometry_params = projector_params[2]
-        (delta_det_channel, delta_det_row, det_channel_offset, det_row_offset, det_rotation, source_detector_dist,
-         delta_voxel, recon_slice_offset, magnification, psf_radius) = geometry_params
-
-        num_views, num_det_rows, num_det_channels = projector_params[0]
-        recon_shape = projector_params[1]
+        num_views, num_det_rows, num_det_channels = projector_params.sinogram_shape
+        recon_shape = projector_params.recon_shape
         num_recon_rows, num_recon_cols, num_recon_slices = recon_shape
 
         # Convert the index into (i,j,k) coordinates corresponding to the indices into the 3D voxel array
         row_index, col_index = jnp.unravel_index(pixel_indices, recon_shape[:2])
         slice_index = jnp.arange(num_recon_slices)
 
-        x_p, y_p, _ = ConeBeamModel.recon_ijk_to_xyz(row_index, col_index, slice_index, delta_voxel,
-                                                       recon_shape, recon_slice_offset, angle)
+        x_p, y_p, _ = ConeBeamModel.recon_ijk_to_xyz(row_index, col_index, slice_index, gp.delta_voxel,
+                                                       recon_shape, gp.recon_slice_offset, angle)
 
         # Convert from xyz to coordinates on detector
-        pixel_mag = 1 / (1 / magnification - y_p / source_detector_dist)  # This should be kept in terms of magnification
+        # pixel_mag should be kept in terms of magnification to allow for source_detector_dist = jnp.Inf
+        pixel_mag = 1 / (1 / gp.magnification - y_p / gp.source_detector_dist)
         # Compute the physical position that this voxel projects onto the detector
         u_p = pixel_mag * x_p
         det_center_channel = (num_det_channels - 1) / 2.0  # num_of_cols
 
         # Calculate indices on the detector grid
-        n_p = (u_p / delta_det_channel) + det_center_channel + det_channel_offset
+        n_p = (u_p / gp.delta_det_channel) + det_center_channel + gp.det_channel_offset
         n_p_center = jnp.round(n_p).astype(int)
 
         # Compute horizontal and vertical cone angle of pixel
-        theta_p = jnp.arctan2(u_p, source_detector_dist)
+        theta_p = jnp.arctan2(u_p, gp.source_detector_dist)
 
         # Compute cos alpha for row and columns
         cos_alpha_p_xy = jnp.maximum(jnp.abs(jnp.cos(angle - theta_p)),
                                     jnp.abs(jnp.sin(angle - theta_p)))
 
         # Compute projected voxel width along columns and rows (in fraction of detector size)
-        W_p_c = pixel_mag * (delta_voxel / delta_det_channel) * (cos_alpha_p_xy / jnp.cos(theta_p))
+        W_p_c = pixel_mag * (gp.delta_voxel / gp.delta_det_channel) * (cos_alpha_p_xy / jnp.cos(theta_p))
 
         horizontal_data = (n_p, n_p_center, W_p_c, cos_alpha_p_xy)
 
         return horizontal_data
 
     @staticmethod
-    @jax.jit
     def recon_ijk_to_xyz(i, j, k, delta_voxel, recon_shape,
                          recon_slice_offset, angle):
         """
         Convert (i, j, k) indices into the recon volume to corresponding (x, y, z) coordinates.
         """
 
         num_recon_rows, num_recon_cols, num_recon_slices = recon_shape
@@ -592,15 +590,14 @@
         x = cosine * x_tilde - sine * y_tilde
         y = sine * x_tilde + cosine * y_tilde
 
         z = delta_voxel * (k - (num_recon_slices - 1) / 2.0) + recon_slice_offset
         return x, y, z
 
     @staticmethod
-    @jax.jit
     def geometry_xyz_to_uv_mag(x, y, z, source_detector_dist, magnification):
         """
         Convert (x, y, z) coordinates to to (u, v) detector coordinates plus the pixel-dependent magnification.
         """
         # Compute the magnification at this specific voxel
         # The following expression is valid even when source_detector_dist = jnp.Inf
         pixel_mag = 1 / (1 / magnification - y / source_detector_dist)
```

### Comparing `mbirjax-0.1.0/mbirjax/parallel_beam.py` & `mbirjax-0.2.0/mbirjax/parallel_beam.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-import warnings
-
 import jax
 import jax.numpy as jnp
 from functools import partial
+from collections import namedtuple
 from mbirjax import TomographyModel, ParameterHandler
 
 
 class ParallelBeamModel(TomographyModel):
     """
     A class designed for handling forward and backward projections in a parallel beam geometry, extending the
     :ref:`TomographyModelDocs`. This class offers specialized methods and parameters tailored for parallel beam setups.
 
     This class inherits all methods and properties from the :ref:`TomographyModelDocs` and may override some
     to suit parallel beam geometrical requirements. See the documentation of the parent class for standard methods
     like setting parameters and performing projections and reconstructions.
 
     Args:
-        angles (jnp.ndarray):
-            A 1D array of projection angles, in radians, specifying the angle of each projection relative to the origin.
         sinogram_shape (tuple):
             Shape of the sinogram as a tuple in the form `(views, rows, channels)`, where 'views' is the number of
             different projection angles, 'rows' correspond to the number of detector rows, and 'channels' index columns of
             the detector that are assumed to be aligned with the rotation axis.
+        angles (jnp.ndarray):
+            A 1D array of projection angles, in radians, specifying the angle of each projection relative to the origin.
         **kwargs (dict):
             Additional keyword arguments that are passed to the :ref:`TomographyModelDocs` constructor. These can
             include settings and configurations specific to the tomography model such as noise models or image dimensions.
             Refer to :ref:`TomographyModelDocs` documentation for a detailed list of possible parameters.
 
     Examples
     --------
@@ -59,15 +58,15 @@
 
         Args:
             filename (str): Name of the file containing parameters to load.
 
         Returns:
             ConeBeamModel with the specified parameters.
         """
-        # Load the parameters and convert to use the ConeBeamModel keywords.
+        # Load the parameters and convert to use the ParallelBeamModel keywords.
         params = ParameterHandler.load_param_dict(filename, values_only=True)
         angles = params['view_params_array']
         del params['view_params_array']
         return cls(angles=angles, **params)
 
     def get_magnification(self):
         """
@@ -104,21 +103,27 @@
             raise ValueError(error_message)
 
     def get_geometry_parameters(self):
         """
         Function to get a list of the primary geometry parameters for for parallel beam projection.
 
         Returns:
-            List of required geometry parameters.
+            namedtuple of required geometry parameters.
         """
-        geometry_params = self.get_params(['delta_det_channel', 'det_channel_offset', 'delta_voxel'])
-
-        # Append psf_radius to list of geometry params
-        psf_radius = self.get_psf_radius()
-        geometry_params.append(psf_radius)
+        # First get the parameters managed by ParameterHandler
+        geometry_param_names = ['delta_det_channel', 'det_channel_offset', 'delta_voxel']
+        geometry_param_values = self.get_params(geometry_param_names)
+
+        # Then get additional parameters:
+        geometry_param_names += ['psf_radius']
+        geometry_param_values.append(self.get_psf_radius())
+
+        # Then create a namedtuple to access parameters by name in a way that can be jit-compiled.
+        GeometryParams = namedtuple('GeometryParams', geometry_param_names)
+        geometry_params = GeometryParams(*tuple(geometry_param_values))
 
         return geometry_params
 
     def get_psf_radius(self):
         """Computes the integer radius of the PSF kernel for parallel beam projection.
         """
         delta_det_channel, delta_voxel = self.get_params(['delta_det_channel', 'delta_voxel'])
@@ -138,175 +143,165 @@
         num_recon_rows = int(jnp.ceil(num_det_channels * delta_det_channel / (delta_voxel * magnification)))
         num_recon_cols = num_recon_rows
         num_recon_slices = int(jnp.round(num_det_rows * ((delta_det_row / delta_voxel) / magnification)))
         recon_shape = (num_recon_rows, num_recon_cols, num_recon_slices)
         self.set_params(no_compile=no_compile, no_warning=no_warning, recon_shape=recon_shape)
 
     @staticmethod
-    def back_project_one_view_to_pixel_batch(sinogram_view, pixel_indices, single_view_params, projector_params, coeff_power=1):
+    @partial(jax.jit, static_argnames='projector_params')
+    def forward_project_pixel_batch_to_one_view(voxel_values, pixel_indices, angle, projector_params):
         """
-        Use vmap to do a backprojection from one view to multiple pixels (voxel cylinders).
+        Apply a parallel beam transformation to a set of voxel cylinders. These cylinders are assumed to have
+        slices aligned with detector rows, so that a parallel beam maps a cylinder slice to a detector row.
+        This function returns the resulting sinogram view.
 
         Args:
-            sinogram_view (2D jax array): one view of the sinogram to be back projected
-            pixel_indices (1D jax array of int):  indices into flattened array of size num_rows x num_cols.
-            single_view_params: These are the view dependent parameters for the view being back projected.
-            projector_params (1D jax array): tuple of (sinogram_shape, recon_shape, get_geometry_params()).
-            coeff_power (int): backproject using the coefficients of (A_ij ** coeff_power).
-                Normally 1, but should be 2 when computing Hessian diagonal.
+            voxel_values (jax array):  2D array of shape (num_pixels, num_recon_slices) of voxel values, where
+                voxel_values[i, j] is the value of the voxel in slice j at the location determined by indices[i].
+            pixel_indices (jax array of int):  1D vector of shape (len(pixel_indices), ) holding the indices into
+                the flattened array of size num_rows x num_cols.
+            angle (float):  Angle for this view
+            projector_params (namedtuple):  tuple of (sinogram_shape, recon_shape, get_geometry_params())
 
         Returns:
-            The voxel values for all slices at the input index (i.e., a voxel cylinder) obtained by backprojecting
-            the input sinogram view.
-
-        """
-        bp_vmap = jax.vmap(ParallelBeamModel.back_project_one_view_to_pixel, in_axes=(None, 0, None, None, None))
-        bp = bp_vmap(sinogram_view, pixel_indices, single_view_params, projector_params, coeff_power)
-        return bp
-
-    @staticmethod
-    def back_project_one_view_to_pixel(sinogram_view, pixel_index, angle, projector_params, coeff_power=1):
+            jax array of shape (num_det_rows, num_det_channels)
         """
-        Calculate the backprojection value to a specified recon voxel cylinder specified by a pixel location. 
-        Takes as input one sinogram view and various parameters. This code uses the distance driven projector.
+        # Get all the geometry parameters - we use gp since geometry parameters is a named tuple and we'll access
+        # elements using, for example, gp.delta_det_channel, so a longer name would be clumsy.
+        gp = projector_params.geometry_params
+        num_views, num_det_rows, num_det_channels = projector_params.sinogram_shape
+
+        # Get the data needed for horizontal projection
+        n_p, n_p_center, W_p_c, cos_alpha_p_xy = ParallelBeamModel.compute_proj_data(pixel_indices, angle, projector_params)
+        L_max = jnp.minimum(1, W_p_c)
+
+        # Allocate the sinogram array
+        sinogram_view = jnp.zeros((num_det_rows, num_det_channels))
+
+        # Define the projector, which will be vmapped over slices.
+        def project_slice(sinogram_view_row, voxel_values_slice):
+            for n_offset in jnp.arange(start=-gp.psf_radius, stop=gp.psf_radius+1):
+                n = n_p_center + n_offset
+                abs_delta_p_c_n = jnp.abs(n_p - n)
+                L_p_c_n = jnp.clip((W_p_c + 1) / 2 - abs_delta_p_c_n, 0, L_max)
+                A_chan_n = gp.delta_voxel * L_p_c_n / cos_alpha_p_xy
+                A_chan_n *= (n >= 0) * (n < num_det_channels)
+                sinogram_view_row = sinogram_view_row.at[n].add(A_chan_n * voxel_values_slice)
 
-        Args:
-            sinogram_view (jax array): one view of the sinogram to be back projected
-            pixel_index: the integer index into flattened recon - need to apply unravel_index(pixel_index, recon_shape) to get i, j, k
-            angle (float): The angle in radians for this view.
-            projector_params (tuple):  tuple of (sinogram_shape, recon_shape, get_geometry_params()).
-            coeff_power: [int] backproject using the coefficients of (A_ij ** coeff_power).
-                Normally 1, but should be 2 for compute_hessian_diagonal.
+            return sinogram_view_row
 
-        Returns:
-            The value of the voxel for all slices at the input index (i.e., a voxel cylinder) obtained by backprojecting
-            the input sinogram view.
-        """
+        sinogram_view = jax.vmap(project_slice, in_axes=(0, 1))(sinogram_view, voxel_values)
 
-        # Get the part of the system matrix and channel indices for this voxel cylinder
-        sinogram_view_shape = (1,) + sinogram_view.shape  # Adjoin a leading 1 to indicate a single view sinogram
-        view_projector_params = (sinogram_view_shape,) + projector_params[1:]
-        Aij_value, Aij_index = ParallelBeamModel.compute_sparse_A_single_view(pixel_index, angle, view_projector_params)
-
-        # Extract out the relevant entries from the sinogram
-        sinogram_array = sinogram_view[:, Aij_index.T.flatten()]
-
-        # Compute dot product
-        back_projection = jnp.sum(sinogram_array * (Aij_value**coeff_power), axis=1)
-        # jax.debug.breakpoint()
-        return back_projection
+        return sinogram_view
 
     @staticmethod
-    def forward_project_pixel_batch_to_one_view(voxel_values, pixel_indices, angle, projector_params):
+    @partial(jax.jit, static_argnames='projector_params')
+    def back_project_one_view_to_pixel_batch(sinogram_view, pixel_indices, angle, projector_params, coeff_power=1):
         """
-        Forward project a set of voxel cylinders determined by indices into the flattened array of size 
-        num_rows x num_cols.
+        Apply parallel back projection to a single sinogram view and return the resulting voxel cylinders.
 
         Args:
-            voxel_values (jax array):  2D array of shape (num_indices, num_slices) of voxel values, where
-                voxel_values[i, j] is the value of the voxel in slice j at the location determined by indices[i].
-            pixel_indices (jax array of int):  1D vector of indices into flattened array of size num_rows x num_cols.
-            angle (float):  Angle for this view
-            projector_params (tuple):  tuple of (sinogram_shape, recon_shape, get_geometry_params())
-
+            sinogram_view (2D jax array): one view of the sinogram to be back projected.
+                2D jax array of shape (num_det_rows)x(num_det_channels)
+            pixel_indices (1D jax array of int):  indices into flattened array of size num_rows x num_cols.
+            angle (float): The projection angle in radians for this view.
+            projector_params (namedtuple): tuple of (sinogram_shape, recon_shape, get_geometry_params()).
+            coeff_power (int): backproject using the coefficients of (A_ij ** coeff_power).
+                Normally 1, but should be 2 when computing Hessian diagonal.
         Returns:
-            jax array of shape (num_det_rows, num_det_channels)
+            jax array of shape (len(pixel_indices), num_det_rows)
         """
-        if voxel_values.ndim != 2:
-            raise ValueError('voxel_values must have shape (num_indices, num_slices)')
+        # Get all the geometry parameters - we use gp since geometry parameters is a named tuple and we'll access
+        # elements using, for example, gp.delta_det_channel, so a longer name would be clumsy.
+        gp = projector_params.geometry_params
+        num_views, num_det_rows, num_det_channels = projector_params.sinogram_shape
+
+        num_pixels = pixel_indices.shape[0]
+
+        # Get the data needed for horizontal projection
+        n_p, n_p_center, W_p_c, cos_alpha_p_xy = ParallelBeamModel.compute_proj_data(pixel_indices, angle, projector_params)
+        L_max = jnp.minimum(1, W_p_c)
+
+        # Allocate the voxel cylinder array
+        voxel_cylinder = jnp.zeros((num_pixels, num_det_rows))
+
+        # Define the horizontal projector, which will be vmapped over slices.
+        def project_slice(recon_voxel_slice, sinogram_view_row):
+            for n_offset in jnp.arange(start=-gp.psf_radius, stop=gp.psf_radius+1):
+                n = n_p_center + n_offset
+                abs_delta_p_c_n = jnp.abs(n_p - n)
+                L_p_c_n = jnp.clip((W_p_c + 1) / 2 - abs_delta_p_c_n, 0, L_max)
+                A_chan_n = gp.delta_voxel * L_p_c_n / cos_alpha_p_xy
+                A_chan_n *= (n >= 0) * (n < num_det_channels)
+                A_chan_n = A_chan_n ** coeff_power
+                recon_voxel_slice = jnp.add(recon_voxel_slice, A_chan_n * sinogram_view_row[n])
 
-        # Get the geometry parameters and the system matrix and channel indices
-        num_views, num_det_rows, num_det_channels = projector_params[0]
-        Aij_value, Aij_channel = ParallelBeamModel.compute_sparse_A_single_view(pixel_indices, angle, projector_params)
-
-        # Add axes to be able to broadcast while multiplying.
-        # sinogram_values has shape num_indices x (2p+1) x num_slices
-        sinogram_values = (Aij_value[:, :, None] * voxel_values[:, None, :])
-
-        # Now sum over indices into the locations specified by Aij_channel.
-        # Directly using index_add for indexed updates
-        sinogram_view = jnp.zeros((num_det_rows, num_det_channels))  # num_det_rows x num_det_channels
-
-        # Apply the vectorized update function with a vmap over slices
-        # sinogram_view is num_det_rows x num_det_channels, sinogram_values is num_indices x (2p+1) x num_det_rows
-        sinogram_values = sinogram_values.transpose((2, 0, 1))
-        sinogram_view = sinogram_view.at[:, Aij_channel].add(sinogram_values)
-        del Aij_value, Aij_channel
-        return sinogram_view
+            return recon_voxel_slice
+
+        voxel_cylinder = jax.vmap(project_slice, in_axes=(1, 0), out_axes=1)(voxel_cylinder, sinogram_view)
 
+        return voxel_cylinder
 
     @staticmethod
     @partial(jax.jit, static_argnames='projector_params')
-    def compute_sparse_A_single_view(pixel_indices, angle, projector_params):
+    def compute_proj_data(pixel_indices, angle, projector_params):
         """
-        Calculate the sparse system matrix for a subset of voxels and a single view.
-        The function returns a sparse matrix specified by the matrix values and associated detector column index.
-        Since this is for parallel beam geometry, the values are assumed to be the same for each row/slice pair.
+        Compute the quantities n_p, n_p_center, W_p_c, cos_alpha_p_xy needed for vertical projection.
 
         Args:
-            pixel_indices (jax array of int):  1D vector of indices into flattened array of size num_rows x num_cols.
-            angle (float):  Angle for this single view
-            projector_params (tuple):  tuple of (sinogram_shape, recon_shape, get_geometry_params())
+            pixel_indices (1D jax array of int):  indices into flattened array of size num_rows x num_cols.
+            angle (float): The projection angle in radians for this view.
+            projector_params (namedtuple): tuple of (sinogram_shape, recon_shape, get_geometry_params()).
 
         Returns:
-            Aij_value (num indices, 2p+1), Aji_channel (num indices, 2p+1)
+            n_p, n_p_center, W_p_c, cos_alpha_p_xy
         """
-        # Get all the geometry parameters
-        geometry_params = projector_params[2]
-        delta_det_channel, det_channel_offset, delta_voxel, psf_radius = geometry_params
+        # Get all the geometry parameters - we use gp since geometry parameters is a named tuple and we'll access
+        # elements using, for example, gp.delta_det_channel, so a longer name would be clumsy.
+        gp = projector_params.geometry_params
 
-        num_views, num_det_rows, num_det_channels = projector_params[0]
-        num_recon_rows, num_recon_cols = projector_params[1][:2]
+        num_views, num_det_rows, num_det_channels = projector_params.sinogram_shape
+        recon_shape = projector_params.recon_shape
 
         # Convert the index into (i,j,k) coordinates corresponding to the indices into the 3D voxel array
-        recon_shape_2d = (num_recon_rows, num_recon_cols)
-        row_index, col_index = jnp.unravel_index(pixel_indices, recon_shape_2d)
+        row_index, col_index = jnp.unravel_index(pixel_indices, recon_shape[:2])
+
+        x_p = ParallelBeamModel.recon_ij_to_x(row_index, col_index, gp.delta_voxel, recon_shape, angle)
+
+        det_center_channel = (num_det_channels - 1) / 2.0  # num_of_cols
+
+        # Calculate indices on the detector grid
+        n_p = (x_p / gp.delta_det_channel) + det_center_channel + gp.det_channel_offset
+        n_p_center = jnp.round(n_p).astype(int)
+
+        # Compute cos alpha for row and columns
+        cos_alpha_p_xy = jnp.maximum(jnp.abs(jnp.cos(angle)),
+                                    jnp.abs(jnp.sin(angle)))
+
+        # Compute projected voxel width along columns and rows (in fraction of detector size)
+        W_p_c = (gp.delta_voxel / gp.delta_det_channel) * cos_alpha_p_xy
+
+        proj_data = (n_p, n_p_center, W_p_c, cos_alpha_p_xy)
+
+        return proj_data
+
+    @staticmethod
+    @jax.jit
+    def recon_ij_to_x(i, j, delta_voxel, recon_shape, angle):
+        """
+        Convert (i, j, k) indices into the recon volume to corresponding (x, y, z) coordinates.
+        """
+        num_recon_rows, num_recon_cols, num_recon_slices = recon_shape
+
+        # Compute the un-rotated coordinates relative to iso
+        # Note the change in order from (i, j) to (y, x)!!
+        y_tilde = delta_voxel * (i - (num_recon_rows - 1) / 2.0)
+        x_tilde = delta_voxel * (j - (num_recon_cols - 1) / 2.0)
+
+        # Precompute cosine and sine of view angle, then do the rotation
+        cosine = jnp.cos(angle)  # length = num_views
+        sine = jnp.sin(angle)  # length = num_views
 
-        # Compute the x,y position of the voxel relative to the center of rotation
-        # Assumes: rows index top to bottom; slice is viewed from the top; rotation of object is clockwise
-        y_pos = delta_voxel * (row_index - ((num_recon_rows - 1.0) / 2.0))  # length = num_indices
-        x_pos = delta_voxel * (col_index - ((num_recon_cols - 1.0) / 2.0))
-
-        # Compute projection of the scalar center-of-rotation onto the detector in ALUs
-        channel_center = (delta_det_channel * (num_det_channels - 1.0) / 2.0) + det_channel_offset
-
-        # Precompute cosine and sine of view angle
-        cosine = jnp.cos(angle)    # length = num_views
-        sine = jnp.sin(angle)      # length = num_views
-
-        # Rotate coordinates of pixel
-        x_pos_rot = cosine * x_pos - sine * y_pos  # length = num_indices
-        # y_pos_rot = sine*x_pos + cosine*y_pos
-
-        # Calculate cos alpha = cos ( smallest angle between source-voxel line and voxel edge )
-        cos_alpha = jnp.maximum(jnp.abs(cosine), jnp.abs(sine))  # length = num_indices
-
-        # Calculate W = length of projection of flattened voxel on detector
-        W = delta_voxel * cos_alpha  # length = num_indices
-
-        # Compute the location on the detector in ALU of the projected center of the voxel
-        x_pos_on_detector = x_pos_rot + channel_center  # length = num_indices
-
-        # Compute a jnp array with 2p+1 entries that are the channel indices of the relevant channels
-        Aij_channel = jnp.round(x_pos_on_detector / delta_det_channel).astype(int)  # length = num_indices
-        Aij_channel = Aij_channel.reshape((-1, 1))
-
-        # Compute channel indices for 2p+1 adjacent channels at each view angle
-        # Should be num_indices x 2p+1
-        # Aij_channel = jnp.concatenate([Aij_channel - 1, Aij_channel, Aij_channel + 1], axis=-1)
-        Aij_channel = jnp.concatenate([Aij_channel + j for j in range(-psf_radius, psf_radius+1)], axis=-1)
-
-        # Compute the distance of each channel from the projected center of the voxel
-        delta = jnp.abs(
-            Aij_channel * delta_det_channel - x_pos_on_detector.reshape((-1, 1)))  # Should be num_indices x 2p+1
-
-        # Calculate L = length of intersection between detector element and projection of flattened voxel
-        tmp1 = (W + delta_det_channel) / 2.0  # length = num_indices
-        tmp2 = (W - delta_det_channel) / 2.0  # length = num_indices
-        Lv = jnp.maximum(tmp1 - jnp.maximum(jnp.abs(tmp2), delta), 0)  # Should be num_indices x 2p+1
-
-        # Compute the values of Aij
-        Aij_value = (delta_voxel / cos_alpha) * (Lv / delta_det_channel)  # Should be num_indices x 2p+1
-        Aij_value = Aij_value * (Aij_channel >= 0) * (Aij_channel < num_det_channels)
+        x = cosine * x_tilde - sine * y_tilde
+        y = sine * x_tilde + cosine * y_tilde
 
-        # jax.debug.breakpoint()
-        return Aij_value, Aij_channel
+        return x
```

### Comparing `mbirjax-0.1.0/mbirjax/parameter_handler.py` & `mbirjax-0.2.0/mbirjax/parameter_handler.py`

 * *Files identical despite different names*

### Comparing `mbirjax-0.1.0/mbirjax/plot_utils.py` & `mbirjax-0.2.0/mbirjax/plot_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,163 +1,157 @@
 import matplotlib.pyplot as plt
+import numpy
 import numpy as np
 from mpl_toolkits.axes_grid1 import make_axes_locatable
+from matplotlib import gridspec
+from matplotlib.widgets import RangeSlider, Slider
 
-global slice_index, slice_line, vmin_cur, vmax_cur, vmin_line, vmax_line, intensity_line, ax, fig, cur_fig, img
 
-
-def slice_viewer(data, data2=None, title='', vmin=None, vmax=None, slice_label='Slice'):
+def slice_viewer(data, data2=None, title='', vmin=None, vmax=None, slice_label='Slice', slice_label2=None,
+                 slice_axis=2, slice_axis2=None, cmap='gray'):
     """
     Display slices of one or two 3D image volumes with a consistent grayscale across slices.
-    Allows interactive selection of slices via a draggable line on a colorbar-like axis. If two images are provided,
-    they are displayed side by side for comparative purposes.
+    Allows interactive selection of slices and intensity window. If two images are provided,
+    they are displayed side by side for comparative purposes.  If the two images have the same shape, then zoom
+    and pan will be applied to each image simultaneously.  If not pan and zoom are applied to one image at a time.
 
     Args:
-        data (numpy.ndarray or jax.numpy.DeviceArray): 3D image volume with shape (height, width, depth).
-        data2 (numpy.ndarray or jax.numpy.DeviceArray, optional): Second 3D image volume with the same shape as the first.
+        data (ndarray or jax array): 3D image volume with shape (height, width, depth).
+        data2 (numpy array or jax array, optional): Second 3D image volume with the same shape as the first.
         title (string, optional, default=''): Figure super title
-        vmin (float): minimum for displayed intensity
-        vmax (float): maximum for displayed intensity
-        slice_label (str): Text label to be used for a given slice.  Defaults to 'Slice'
-
-    The function sets up a matplotlib figure with interactive controls to view different slices
-    by clicking and dragging on a custom colorbar. Each slice is displayed using the same grayscale range
-    determined by the global min and max of the entire volume.
+        vmin (float, optional): minimum for displayed intensity
+        vmax (float, optional): maximum for displayed intensity
+        slice_label (str, optional): Text label to be used for a given slice.  Defaults to 'Slice'
+        slice_label2 (str, optional): Text label to be used for a given slice for data2.  Defaults to slice_label.
+        slice_axis (int, optional): The dimension of data to use for the slice index.  That is, if slice_axis=1, then the
+            displayed images will be data[:, slice_index, :]
+        slice_axis2 (int, optional): The dimension of data to use for the slice index for data2.
+
+    Example:
+        .. code-block:: python
+
+            data1 = np.random.rand(100, 100, 50)  # Random 3D volume
+            data2 = np.random.rand(100, 100, 50)  # Another random 3D volume
+            slice_viewer(data1, data2, slice_axis=2, title='Slice Demo', slice_label='Current slice')  # View slices of both volumes side by side
     """
-    global slice_index, slice_line, vmin_cur, vmax_cur, vmin_line, vmax_line, intensity_line, cur_fig
-
-    slice_index = data.shape[2] // 2  # Initial slice index
+    if data.ndim != 3:  # or (data2 is not None and data.shape[slice_axis] != data2.shape[slice_axis]):
+        error_msg = 'The input data must be a 3D array'  #, and if data2 is provided, then data.shape[slice_axis] '
+        # error_msg += 'must equal data2.shape[slice_axis])'
+        raise ValueError(error_msg)
+
+    # Move the specified slice axis into the last position
+    data = numpy.moveaxis(data, slice_axis, 2)
+    if data2 is not None:
+        if slice_axis2 is None:
+            slice_axis2 = slice_axis
+        data2 = numpy.moveaxis(data2, slice_axis2, 2)
+        if slice_label2 is None:
+            slice_label2 = slice_label
 
     # Define min and max grayscale values for consistent coloring across slices
     if vmin is None:
         vmin = min(data.min(), data2.min()) if data2 is not None else data.min()
     if vmax is None:
         vmax = max(data.max(), data2.max()) if data2 is not None else data.max()
     if vmin > vmax:
         raise ValueError('vmin must be less than or equal to vmax')
     if vmin == vmax:
         eps = 1e-6  # This is not floating point epsilon, just a small number for display purposes.
         scale = np.clip(eps * np.abs(vmax), a_min=eps, a_max=None)
         vmin = vmin - scale
         vmax = vmax + scale
 
-    vmin_cur, vmax_cur = vmin, vmax
-    cur_fig = None
+    # Set up the plot
+    figwidth = 6 if data2 is None else 10
+    fig = plt.figure(figsize=(figwidth, 6))
+    fig.suptitle(title)
+
+    # Set up the subplots. One or two images in the first row along with colorbars.
+    gs = gridspec.GridSpec(nrows=3, ncols=2, height_ratios=[10, 1, 1])
+    ax_data, ax_data2 = None, None
+    if data2 is None:
+        ax_data = fig.add_subplot(gs[0, :])
+    else:
+        ax_data = fig.add_subplot(gs[0, 0])
+        share_axis = ax_data if data.shape == data2.shape else None
+        ax_data2 = fig.add_subplot(gs[0, 1], sharex=share_axis, sharey=share_axis)
+
+    # Show the initial slice
+    slice_index = data.shape[2] // 2
+    im = ax_data.imshow(data[:, :, slice_index], cmap=cmap, vmin=vmin, vmax=vmax)
+    im2 = None
+    if data2 is not None:
+        slice_index2 = data2.shape[2] // 2
+        im2 = ax_data2.imshow(data2[:, :, slice_index2], cmap=cmap, vmin=vmin, vmax=vmax)
+        ax_data2.set_title(f'{slice_label2} {slice_index2}')
+
+    # Set up a colorbar next to the rightmost image, but add extra space to both to make them the same size.
+    divider = make_axes_locatable(ax_data)
+    cax = divider.append_axes('right', size='5%', pad=0.05)
+    if data2 is not None:
+        divider2 = make_axes_locatable(ax_data2)
+        cax.axis('off')
+        cax = divider2.append_axes('right', size='5%', pad=0.05)
+
+    fig.colorbar(im, cax=cax, orientation='vertical')
+
+    # Then add the slice slider
+    ax_slice_slider = fig.add_subplot(gs[1, :])
+    slice_slider = Slider(ax=ax_slice_slider, label=slice_label, valmin=0, valmax=data.shape[2],
+                          valinit=slice_index, valfmt='%0.0f')
+
+    # Then the intensity slider
+    ax_intensity_slider = fig.add_subplot(gs[2, :])
+    log_intensity_range = np.log10(vmax - vmin)
+    num_digits = max(- int(np.round(log_intensity_range)) + 2, 0)
+    valfmt = '%0.' + str(num_digits) + 'f'
+    valinit = (vmin, vmax)
+    intensity_slider = RangeSlider(ax_intensity_slider, "Intensity\nrange", vmin, vmax,
+                                   valinit=valinit, valfmt=valfmt)
+
+    ax_data.set_title(f'{slice_label} {slice_index}')
+
+    fig.text(0.01, 0.95, 'Close plot \nto continue')
+
+    # Set up the callback functions for the sliders
+    def update_intensity(val):
+        # The val passed to a callback by the RangeSlider will
+        # be a tuple of (min, max), which are used to set vmin and vmax for both images.
+
+        # Update the image's colormap
+        im.norm.vmin = val[0]
+        im.norm.vmax = val[1]
 
-    def update_slice(x):
-        """Update the displayed slice based on the position of the mouse click or drag on the colorbar axis."""
-        global slice_index, slice_line, cur_fig
-        slice_index = int(0.5 + x / ax_slice_slider.get_xlim()[1] * (data.shape[2] - 1))
-        slice_line.set_xdata([slice_index, slice_index])
-        redraw_fig(cur_fig)
-
-    def update_intensity(x):
-        global vmin_cur, vmax_cur, vmin_line, vmax_line, intensity_line, cur_fig
-        # Determine whether x is closer to vmin_cur or vmax_cur and set the line appropriately
-        if x - vmin_cur < vmax_cur - x:
-            vmin_cur = x
-            vmin_line.set_xdata([vmin_cur, vmin_cur])
-        else:
-            vmax_cur = x
-            vmax_line.set_xdata([vmax_cur, vmax_cur])
-
-        xmin_cur = (vmin_cur - vmin) / (vmax - vmin)
-        xmax_cur = (vmax_cur - vmin) / (vmax - vmin)
-
-        intensity_line.set_xdata([xmin_cur, xmax_cur])
-        redraw_fig(cur_fig)
-
-    def redraw_fig(fig, first_pass=False):
-        """Redraw the figure to update the slice and its display.
-        The colorbar is drawn only at initialization.
-        """
-        ax.clear()
         if data2 is not None:
-            image_divider = vmax * np.ones((data.shape[0], 5))
-            cur_data = np.concatenate((data[:, :, slice_index], image_divider, data2[:, :, slice_index]), axis=1)
-            ax.set_title(f'{slice_label} {slice_index} Comparison')
-        else:
-            cur_data = data[:, :, slice_index]
-            ax.set_title(f'{slice_label} {slice_index}')
-        im = ax.imshow(np.clip(cur_data, vmin_cur, vmax_cur), cmap='gray', vmin=vmin_cur, vmax=vmax_cur)
-        if not first_pass:
-            fig.axes[5].remove()
-        divider = make_axes_locatable(ax)
-        cax = divider.append_axes('right', size='5%', pad=0.05)
+            im2.norm.vmin = val[0]
+            im2.norm.vmax = val[1]
 
-        fig.colorbar(im, cax=cax, orientation='vertical')
+        # Redraw the figure to ensure it updates
         fig.canvas.draw_idle()
 
-    def on_press(event):
-        """Handle mouse press events for interactive slice selection."""
-        if event.inaxes == ax_slice_slider:
-            update_slice(event.xdata)
-        if event.inaxes == ax_intensity_slider:
-            update_intensity(event.xdata)
-
-    def on_motion(event):
-        """Handle mouse motion events for continuous slice selection while dragging."""
-        if event.inaxes == ax_slice_slider and event.button == 1:
-            update_slice(event.xdata)
-        if event.inaxes == ax_intensity_slider and event.button == 1:
-            update_intensity(event.xdata)
-
-    # Setup the plot
-    plt.ion()  # Turn on interactive mode
-    fig, axes = plt.subplots(nrows=5, ncols=1, figsize=(6, 6), gridspec_kw={'height_ratios': [10, 1, 0.5, 1, 0.5]})
-    fig.suptitle(title)
-    ax = axes[0]
-    ax_slice_slider, ax_slice_instruction = axes[1], axes[2]
-    ax_intensity_slider, ax_intensity_instructions = axes[3], axes[4]
-
-    # Setup the interactive vertical line in the slice slider
-    ax_slice_slider.set_xlim(0, data.shape[2] - 1)
-    ax_slice_slider.set_ylim(0, 1)
-    slice_line = ax_slice_slider.axvline(slice_index, color='black', linewidth=4)  # Movable line
-    ax_slice_slider.set_facecolor('white')
-    ax_slice_slider.set_yticks([])
-    ax_slice_slider.set_xticks([])
-
-    # Add a label below the slider
-    ax_slice_instruction.text(0.5, 0.5, f'Click and drag to change {slice_label.lower()}', ha='center', va='center', fontsize=10)
-    ax_slice_instruction.set_axis_off()
-
-    # Setup the interactive window in the intensity slider
-    ax_intensity_slider.set_xlim(vmin, vmax)
-    ax_intensity_slider.set_ylim(0, 1)
-    intensity_line = ax_intensity_slider.axhline(y=0.5, color='red', linewidth=4)
-    ax_intensity_slider.set_facecolor('white')
-    ax_intensity_slider.set_yticks([])
-    ax_intensity_slider.set_xticks([vmin, vmax])
-    vmin_line = ax_intensity_slider.axvline(vmin, color='blue', linewidth=4)  # Movable line
-    vmax_line = ax_intensity_slider.axvline(vmax, color='red', linewidth=4)
-
-    # Add a label below the slider
-    ax_intensity_instructions.text(0.5, 0.5, 'Click and drag to change intensity window', ha='center', va='center', fontsize=10)
-    ax_intensity_instructions.set_axis_off()
-
-    # Connect events
-    fig.canvas.mpl_connect('button_press_event', on_press)
-    fig.canvas.mpl_connect('motion_notify_event', on_motion)
-
-    # Initial drawing
-    cur_fig = fig
-    redraw_fig(fig, first_pass=True)  # Call redraw to handle initial display for single or dual images
-
-    plt.pause(0.1)  # Delay to ensure window stays open
-    input("Press any key to close ")
-
-    plt.ioff()  # Turn off interactive mode
-    plt.close()
-
-
-# Example usage:
-# data1 = np.random.rand(100, 100, 50)  # Random 3D volume
-# data2 = np.random.rand(100, 100, 50)  # Another random 3D volume
-# slice_viewer(data1, data2)  # View slices of both volumes side by side
+    def update_slice(val):
+        # The val passed to a callback by the Slider is a single float.  We cast it to an int to index the slice.
+        cur_slice = int(np.round(val))
+        im.set_data(data[:, :, cur_slice])
+        ax_data.set_title(f'{slice_label} {cur_slice}')
+        if data2 is not None:
+            slice_fraction = cur_slice / data.shape[2]
+            cur_slice2 = int(np.round(slice_fraction * data2.shape[2]))
+            im2.set_data(data2[:, :, cur_slice2])
+            ax_data2.set_title(f'{slice_label2} {cur_slice2}')
+
+        # Redraw the figure to ensure it updates
+        fig.canvas.draw_idle()
+
+    # Connect the sliders to the callback functions
+    intensity_slider.on_changed(update_intensity)
+    slice_slider.on_changed(update_slice)
+
+    plt.tight_layout()
+    plt.show()
 
 
 def debug_plot_partitions(partitions, recon_shape):
     """
     Visualizes a set of partitions as color images in a single row, where each partition is represented by a different color.
 
     Parameters:
```

### Comparing `mbirjax-0.1.0/mbirjax/projectors.py` & `mbirjax-0.2.0/mbirjax/projectors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-import warnings
-from functools import partial
+from collections import namedtuple
 import jax
 import jax.numpy as jnp
 
 
 class Projectors:
 
-    def __init__(self, tomography_model, forward_core, backward_core):
+    def __init__(self, tomography_model):
 
         self.tomography_model = tomography_model
         self.sparse_forward_project, self.sparse_back_project, self.compute_hessian_diagonal = None, None, None
-        self.create_projectors(forward_core, backward_core)
+        self.create_projectors(tomography_model)
 
-    def create_projectors(self, forward_project_pixel_batch_to_one_view, back_project_one_view_to_pixel_batch):
+    def create_projectors(self, tomography_model):
         """
         Compute the forward and back projectors for this geometry and current view parameters
-        
+
         Args:
-            forward_project_pixel_batch_to_one_view (callable): jit-compilable function implementing
-                :meth:`TomographyModel.forward_project_pixel_batch_to_one_view`
-            back_project_one_view_to_pixel_batch (callable): jit-compilable function implementing
-                :meth:`TomographyModel.back_project_one_view_to_pixel_batch`
+            tomography_model (mbirjax.TomographyModel): An instance describing the current geometry and implementing the following 2 functions:
+
+                * forward_project_pixel_batch_to_one_view (callable): jit-compilable function implementing :meth:`TomographyModel.forward_project_pixel_batch_to_one_view`
+                * back_project_one_view_to_pixel_batch (callable): jit-compilable function implementing :meth:`TomographyModel.back_project_one_view_to_pixel_batch`
 
         Returns:
             Nothing, but the class variables `sparse_forward_project`, `sparse_back_project`, and
             `compute_hessian_diagonal` are set to callable functions.  These are used to implement the following
             methods:
 
             * `sparse_forward_project`: :meth:`TomographyModel.sparse_forward_project`
@@ -35,98 +34,119 @@
             The returned functions will be jit compiled each time they are called with a new shape of input.  If
             called multiple times with the same shape of input, then the cached version will be used, which will
             give reduced execution time relative to the initial call.
 
             This method requires geometry-specific implementations of
             :meth:`TomographyModel.forward_project_pixel_batch_to_one_view` and
             :meth:`TomographyModel.back_project_one_view_to_pixel_batch`.
+
         """
+        forward_project_pixel_batch_to_one_view = tomography_model.forward_project_pixel_batch_to_one_view
+        back_project_one_view_to_pixel_batch = tomography_model.back_project_one_view_to_pixel_batch
+
         geometry_params = self.tomography_model.get_geometry_parameters()
         sinogram_shape, recon_shape = self.tomography_model.get_params(['sinogram_shape', 'recon_shape'])
-        projector_params = (tuple(sinogram_shape), tuple(recon_shape), tuple(geometry_params))
+
+        # Combine the needed parameters into a named tuple for named access compatible with jit
+        projector_param_names = ['sinogram_shape', 'recon_shape', 'geometry_params']
+        projector_param_values = (sinogram_shape, recon_shape, geometry_params)
+        ProjectorParams = namedtuple('ProjectorParams', projector_param_names)
+        projector_params = ProjectorParams(*tuple(projector_param_values))
+
         view_params_array = self.tomography_model.get_params('view_params_array')
         pixel_batch_size, view_batch_size = self.tomography_model.get_params(['pixel_batch_size', 'view_batch_size'])
 
-        def sparse_forward_project_fcn(voxel_values, pixel_indices):
+        def sparse_forward_project_fcn(voxel_values, pixel_indices, view_indices=()):
             """
             Compute the sinogram obtained by forward projecting the specified voxels. The voxel sare determined
             using 2D indices into a flattened array of shape (num_recon_rows, num_recon_cols),
             and for each such 2D index, the voxels in all slices at that location are projected.
 
             This function batches over pixels, applies sparse_forward_project_pixel_batch to each batch,
             then adds the results to get the sinogram.
 
             Args:
                 voxel_values (ndarray or jax array): 2D array of shape (len(pixel_indices), num_slices) of voxel values
                 pixel_indices (ndarray or jax array): 1D array of indices into a flattened array of shape (num_rows, num_cols)
+                view_indices (ndarray or jax array, optional): 1D array of indices into the view parameters array.
+                    If None, then all views are used.
 
             Returns:
-                3D array of shape (num_views, num_det_rows, num_det_cols)
+                3D array of shape (num_views, num_det_rows, num_det_cols), where num_views is len(view_indices) if view_indices is not None
             """
             num_pixels = pixel_indices.shape[0]
             # Apply the batch projector directly to a batch if the batch is small enough.
             if pixel_batch_size is None or pixel_batch_size >= num_pixels:
-                sinogram = sparse_forward_project_pixel_batch(voxel_values, pixel_indices)
+                sinogram = sparse_forward_project_pixel_batch(voxel_values, pixel_indices, view_indices=view_indices)
             # Otherwise subdivide into batches, apply the batch projector, and then add.
             else:
                 num_batches = num_pixels // pixel_batch_size
                 length_of_batches = num_batches * pixel_batch_size
                 voxel_values_batched = jnp.reshape(voxel_values[:length_of_batches],
                                                     (num_batches, pixel_batch_size,) + voxel_values.shape[1:])
                 pixel_indices_batched = jnp.reshape(pixel_indices[:length_of_batches], (num_batches, pixel_batch_size))
 
                 # Set up a scan over the voxel batches.  We'll project one batch to a sinogram,
                 # then add that to the accumulated sinogram
-                initial_sinogram = jnp.zeros(sinogram_shape)
-                initial_carry = [initial_sinogram]
+                num_views = view_params_array.shape[0]
+                if len(view_indices) > 0:
+                    num_views = len(view_indices)
+                initial_sinogram = jnp.zeros((num_views,) + sinogram_shape[1:])
+                initial_carry = [initial_sinogram, view_indices]
                 values_indices = (voxel_values_batched, pixel_indices_batched)
                 final_carry, _ = jax.lax.scan(forward_project_accumulate, initial_carry, values_indices)
 
                 # Get the sinogram from these batches, and add in any leftover voxels
                 sinogram = final_carry[0]
                 num_remaining = num_pixels - num_batches * pixel_batch_size
                 if num_remaining > 0:
                     end_batch_values = voxel_values[-num_remaining:]
                     end_batch_indices = pixel_indices[-num_remaining:]
-                    sinogram += sparse_forward_project_pixel_batch(end_batch_values, end_batch_indices)
+                    sinogram += sparse_forward_project_pixel_batch(end_batch_values, end_batch_indices, view_indices=view_indices)
 
             return sinogram
 
         def forward_project_accumulate(carry, values_indices_batch):
             """
 
             Args:
                 carry:
                 values_indices_batch:
 
             Returns:
 
             """
-            cur_sino = carry[0]
+            cur_sino, view_indices = carry
             voxel_values, pixel_indices = values_indices_batch
-            cur_sino += sparse_forward_project_pixel_batch(voxel_values, pixel_indices)
+            cur_sino += sparse_forward_project_pixel_batch(voxel_values, pixel_indices, view_indices=view_indices)
 
-            return [cur_sino], None
+            return [cur_sino, view_indices], None
 
-        def sparse_forward_project_pixel_batch(voxel_values, pixel_indices):
+        def sparse_forward_project_pixel_batch(voxel_values, pixel_indices, view_indices=()):
             """
             Compute the sinogram obtained by forward projecting the specified batch of voxels. The voxels
             are determined using 2D indices into a flattened array of shape (num_rows, num_cols),
             and for each such 2D index, the voxels in all slices at that location are projected.
 
             This function creates batches of views and collects the results to form the full sinogram.
 
             Args:
                 voxel_values: 2D array of shape (len(pixel_indices), num_slices) of voxel values
                 pixel_indices: 1D array of indices into a flattened array of shape (num_rows, num_cols)
+                view_indices (ndarray or jax array, optional): 1D array of indices into the view parameters array.
+                    If None, then all views are used.
 
             Returns:
                 3D array of shape (num_views, num_det_rows, num_det_cols)
             """
             num_views = view_params_array.shape[0]
+            cur_view_params_array = view_params_array
+            if len(view_indices) > 0:
+                num_views = len(view_indices)
+                cur_view_params_array = view_params_array[view_indices]
 
             def forward_project_single_view(single_view_params):
                 # Use closure to define a mappable function that operates on a single view with the given voxel values.
                 return forward_project_pixel_batch_to_one_view(voxel_values, pixel_indices,
                                                                single_view_params, projector_params)
 
             def forward_project_view_batch(view_params_batch):
@@ -136,78 +156,86 @@
 
                 sino_view_batch = jax.vmap(forward_project_single_view)(view_params_batch)
 
                 return sino_view_batch
 
             # Apply the function on a single batch of views if the batch is small enough.
             if view_batch_size is None or view_batch_size >= num_views:
-                sinogram = forward_project_view_batch(view_params_array)
+                sinogram = forward_project_view_batch(cur_view_params_array)
             # Otherwise break the views up into batches and apply the function to each batch use another level of map.
             else:
                 num_batches = num_views // view_batch_size
-                view_params_batched = jnp.reshape(view_params_array[0:num_batches * view_batch_size],
+                view_params_batched = jnp.reshape(cur_view_params_array[0:num_batches * view_batch_size],
                                                   (num_batches, view_batch_size, -1))
 
                 sinogram = jax.lax.map(forward_project_view_batch, view_params_batched)
                 sinogram = jnp.reshape(sinogram, (num_batches * view_batch_size,) + sinogram.shape[2:])
                 num_remaining = num_views - num_batches * view_batch_size
                 if num_remaining > 0:
-                    end_batch = view_params_array[-num_remaining:]
+                    end_batch = cur_view_params_array[-num_remaining:]
                     end_views = forward_project_view_batch(end_batch)
                     sinogram = jnp.concatenate((sinogram, end_views), axis=0)
 
             return sinogram
 
-        def sparse_back_project_fcn_new(sinogram, pixel_indices, coeff_power=1):
+        def sparse_back_project_fcn(sinogram, pixel_indices, coeff_power=1, view_indices=()):
             """
             Compute the voxel values obtained by back projecting the sinogram to the specified voxels. The voxels
             are determined using 2D indices into a flattened array of shape (num_recon_rows, num_recon_cols),
             and for each such 2D index, the voxels in all slices at that location are projected.
 
             This function batches over views, applies sparse_back_project_view_batch to each batch,
             then adds the results to get the voxel values.
 
             Args:
-                sinogram (ndarray or jax array): 3D array of shape (num_views, num_det_rows, num_det_cols)
+                sinogram (ndarray or jax array): 3D array of shape (cur_num_views, num_det_rows, num_det_cols), where
+                    cur_num_views is recon_shape[0] if view_indices is () and len(view_indices)
+                    otherwise, in which case the views in sinogram should match those indicated by view_indices.
                 pixel_indices (ndarray or jax array): 1D array of indices into a flattened array of shape
                 (num_recon_rows, num_recon_cols)
                 coeff_power (int): backproject using the coefficients of (A_ij ** coeff_power).
-                Normally 1, but should be 2 when computing Hessian diagonal.
+                    Normally 1, but should be 2 when computing Hessian diagonal.
+                view_indices (ndarray or jax array, optional): 1D array of indices into the view parameters array.
+                    If None, then all views are used.
 
             Returns:
                 2D array of shape (num_pixels, num_recon_slices)
             """
-            num_views = sinogram.shape[0]
+            num_views = view_params_array.shape[0]
+            cur_view_params_array = view_params_array
+            if len(view_indices) > 0:
+                num_views = len(view_indices)
+                cur_view_params_array = view_params_array[view_indices]
             num_pixels = pixel_indices.shape[0]
             num_recon_slices = recon_shape[2]
             # Apply the batch projector directly to a batch if the batch is small enough.
             if view_batch_size is None or view_batch_size >= num_views:
-                voxel_values = sparse_back_project_view_batch(sinogram, view_params_array, pixel_indices, coeff_power)
+                voxel_values = sparse_back_project_view_batch(sinogram, cur_view_params_array, pixel_indices, coeff_power)
             # Otherwise subdivide into batches, apply the batch projector, and then add.
             else:
                 num_batches = num_views // view_batch_size
                 length_of_batches = num_batches * view_batch_size
                 sinogram_batched = jnp.reshape(sinogram[:length_of_batches],
                                                (num_batches, view_batch_size,) + sinogram.shape[1:])
-                view_params_batched = jnp.reshape(view_params_array[:length_of_batches],
-                                                  (num_batches, view_batch_size,) + view_params_array.shape[1:])
+                view_params_batched = jnp.reshape(cur_view_params_array[:length_of_batches],
+                                                  (num_batches, view_batch_size,) + cur_view_params_array.shape[1:])
 
                 # Set up a scan over the view batches.  We'll project one batch to voxels,
                 # then add that to the accumulated voxel_values
                 initial_voxel_values = jnp.zeros((num_pixels, num_recon_slices))
                 initial_carry = [initial_voxel_values, pixel_indices, coeff_power]
                 sino_and_params = (sinogram_batched, view_params_batched)
                 final_carry, _ = jax.lax.scan(back_project_accumulate, initial_carry, sino_and_params)
 
                 # Get the voxel values from these batches and add in any leftover views
                 voxel_values = final_carry[0]
                 num_remaining = num_views - num_batches * view_batch_size
                 if num_remaining > 0:
                     end_batch_views = sinogram[-num_remaining:]
-                    end_batch_params = view_params_array[-num_remaining:]
+                    end_batch_params = cur_view_params_array[-num_remaining:]
                     voxel_values += sparse_back_project_view_batch(end_batch_views, end_batch_params,
                                                                    pixel_indices, coeff_power)
 
             return voxel_values
 
         def back_project_accumulate(carry, view_and_params_batch):
             cur_voxel_values, local_pixel_indices, local_coeff_power = carry
@@ -262,122 +290,46 @@
                 if num_remaining > 0:
                     end_batch_indices = pixel_indices[-num_remaining:]
                     end_batch_voxel_values = back_project_pixel_batch(end_batch_indices)
                     new_voxel_values = jnp.concatenate((new_voxel_values, end_batch_voxel_values), axis=0)
 
             return new_voxel_values
 
-        def sparse_back_project_fcn(sinogram, pixel_indices, coeff_power=1):
-            """
-            Compute the voxel values obtained by back projecting the sinogram to the specified voxels. The voxels
-            are determined using 2D indices into a flattened array of shape (num_recon_rows, num_recon_cols),
-            and for each such 2D index, the voxels in all slices at that location are projected.
-
-            Args:
-                sinogram (ndarray or jax array): 3D array of shape (num_views, num_det_rows, num_det_cols)
-                pixel_indices (ndarray or jax array): 1D array of indices into a flattened array of shape
-                (num_recon_rows, num_recon_cols)
-
-            Returns:
-                2D array of shape (num_pixels, num_recon_slices)
-            """
-            new_voxel_values = sparse_back_project_fcn_new(sinogram, pixel_indices, coeff_power)
-            return new_voxel_values
-
-            num_pixels = len(pixel_indices)
-            if pixel_batch_size is None or pixel_batch_size >= num_pixels:
-                voxel_values = back_project_to_pixels_scan(sinogram, pixel_indices, coeff_power=coeff_power)
-            else:
-                num_batches = num_pixels // pixel_batch_size
-                length_of_batches = num_batches * pixel_batch_size
-                indices_batched = jnp.reshape(pixel_indices[:length_of_batches], (num_batches, pixel_batch_size))
-
-                def backward_map(indices_batch):
-                    return back_project_to_pixels_scan(sinogram, indices_batch, coeff_power=coeff_power)
-
-                voxel_values = jax.lax.map(backward_map, indices_batched)
-                voxel_values = voxel_values.reshape((length_of_batches, -1))
-                num_remaining = num_pixels - num_batches * pixel_batch_size
-                if num_remaining > 0:
-                    end_batch = pixel_indices[-num_remaining:]
-                    end_values = backward_map(end_batch)
-                    voxel_values = jnp.concatenate((voxel_values, end_values), axis=0)
-            return voxel_values
-
-        def back_project_to_pixels_scan(sinogram, pixel_indices, coeff_power=1):
-            """
-            Use jax.lax.scan to backproject one view at a time and accumulate the results in the specified voxels.
-            The individual backprojections from each view must be added to get the full backprojection.  This is
-            done using the helper function backproject_accumulate.
-
-            Args:
-                sinogram:
-                pixel_indices:
-                coeff_power:
-
-            Returns:
-
-            """
-            # jax.lax.scan applies a function to each entry indexed by the leading dimension of its input, then
-            # incorporates the output of that function into an accumulator.  Here we apply backproject_accumulate to
-            # one sinogram view and the corresponding view_params.
-            num_recon_slices = recon_shape[2]
-            initial_bp = jnp.zeros((pixel_indices.shape[0], num_recon_slices))
-            extra_args = pixel_indices, coeff_power
-            initial_carry = [extra_args, initial_bp]
-            sino_view_params = (sinogram, view_params_array)
-            # Use lax.scan to process each (slice, view_params) pair of 'sino_view_params'
-            final_carry, _ = jax.lax.scan(backproject_accumulate, initial_carry, sino_view_params)
-
-            return final_carry[1]
-
-        def backproject_accumulate(carry, view_params_pair):
-            """
-
-            Args:
-                carry:
-                view_params_pair:
-
-            Returns:
-
-            """
-            extra_args, accumulated = carry
-            sinogram_view, view_params = view_params_pair
-            pixel_indices, coeff_power = extra_args
-            bp_view = back_project_one_view_to_pixel_batch(sinogram_view, pixel_indices, view_params, projector_params, coeff_power)
-            accumulated += bp_view
-            del bp_view
-            return [extra_args, accumulated], None
-
-        def compute_hessian_diagonal(weights=None):
+        def compute_hessian_diagonal(weights=None, view_indices=()):
             """
             Computes the diagonal of the Hessian matrix, which is computed by doing a backprojection of the weight
             matrix except using the square of the coefficients in the backprojection to a given voxel.
             One of weights or sinogram_shape must be not None. If weights is not None, it must be an array with the same
             shape as the sinogram to be backprojected.  If weights is None, then a weights matrix will be computed as an
             array of ones of size sinogram_shape.
 
             Args:
-                weights (ndarray or None): The weights with shape (views, rows, channels)
+               weights (ndarray or jax array or None, optional): 3D array of shape
+                    (cur_num_views, num_det_rows, num_det_cols), where cur_num_views is recon_shape[0]
+                    if view_indices is () and len(view_indices) otherwise, in which case the views in weights should
+                    match those indicated by view_indices.
+               view_indices (ndarray or jax array, optional): 1D array of indices into the view parameters array.
+                    If None, then all views are used.
 
             Returns:
                 An array that is the same size as the reconstruction.
             """
+            num_views = len(view_indices) if len(view_indices) != 0 else sinogram_shape[0]
             if weights is None:
-                weights = jnp.ones(sinogram_shape)
-            elif weights.shape != sinogram_shape:
-                error_message = 'Weights must be constant or an array of the same shape as sinogram'
+                weights = jnp.ones((num_views,) + sinogram_shape[1:])
+            elif weights.shape != (num_views,) + sinogram_shape[1:]:
+                error_message = 'Weights must be constant or an array compatible with sinogram'
                 error_message += '\nGot weights.shape = {}, but sinogram.shape = {}'.format(weights.shape, sinogram_shape)
                 raise ValueError(error_message)
 
             num_recon_rows, num_recon_cols, num_recon_slices = recon_shape[:3]
             max_index = num_recon_rows * num_recon_cols
             indices = jnp.arange(max_index)
 
-            hessian_diagonal = self.sparse_back_project(weights, indices, coeff_power=2)
+            hessian_diagonal = self.sparse_back_project(weights, indices, coeff_power=2, view_indices=view_indices)
 
             return hessian_diagonal.reshape((num_recon_rows, num_recon_cols, num_recon_slices))
 
         # Set the compiled projectors and Hessian function
         projector_functions = (jax.jit(sparse_forward_project_fcn),
                                jax.jit(sparse_back_project_fcn, static_argnames='coeff_power'),
                                compute_hessian_diagonal)
```

### Comparing `mbirjax-0.1.0/mbirjax/tomography_model.py` & `mbirjax-0.2.0/mbirjax/tomography_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import numpy as np
 import warnings
 import gc
 import jax
 import jax.numpy as jnp
 import mbirjax
 from mbirjax import ParameterHandler
+from functools import partial
+from collections import namedtuple
 
 
 class TomographyModel(ParameterHandler):
     """
     Represents a general model for tomographic reconstruction using MBIRJAX. This class encapsulates the parameters and
     methods for the forward and back projection processes required in tomographic imaging.
 
@@ -24,16 +26,16 @@
 
     Sets up the reconstruction size and parameters.
     """
 
     def __init__(self, sinogram_shape, recon_shape=None, **kwargs):
 
         super().__init__()
-        self._sparse_forward_project, self._sparse_back_project = None, None  # These are callable functions compiled in set_params
-        self._compute_hessian_diagonal = None
+        self.sparse_forward_project, self.sparse_back_project = None, None  # These are callable functions compiled in set_params
+        self.compute_hessian_diagonal = None
         self.set_params(no_compile=True, no_warning=True, sinogram_shape=sinogram_shape, recon_shape=recon_shape, **kwargs)
         delta_voxel = self.get_params('delta_voxel')
         if delta_voxel is None:
             magnification = self.get_magnification()
             delta_det_channel = self.get_params('delta_det_channel')
             delta_voxel = delta_det_channel / magnification
             self.set_params(no_compile=True, no_warning=True, delta_voxel=delta_voxel)
@@ -76,34 +78,33 @@
         Creates an instance of the Projectors class and set the local instance variables needed for forward
         and back projection and compute_hessian_diagonal.  This method requires that the current geometry has
         implementations of :meth:`forward_project_pixel_batch_to_one_view` and :meth:`back_project_one_view_to_pixel_batch`
 
         Returns:
             Nothing, but creates jit-compiled functions.
         """
-        projector_functions = mbirjax.Projectors(self, self.forward_project_pixel_batch_to_one_view,
-                                                 self.back_project_one_view_to_pixel_batch)
-        self._sparse_forward_project = projector_functions.sparse_forward_project
-        self._sparse_back_project = projector_functions.sparse_back_project
-        self._compute_hessian_diagonal = projector_functions.compute_hessian_diagonal
+        projector_functions = mbirjax.Projectors(self)
+        self.sparse_forward_project = projector_functions.sparse_forward_project
+        self.sparse_back_project = projector_functions.sparse_back_project
+        self.compute_hessian_diagonal = projector_functions.compute_hessian_diagonal
 
     @staticmethod
     def forward_project_pixel_batch_to_one_view(voxel_values, pixel_indices, view_params, projector_params):
         """
         Forward project a set of voxels determined by indices into the flattened array of size num_rows x num_cols.
 
         Note:
             This method must be overridden for a specific geometry.
 
         Args:
             voxel_values (jax array):  2D array of shape (num_indices, num_slices) of voxel values, where
                 voxel_values[i, j] is the value of the voxel in slice j at the location determined by indices[i].
             pixel_indices (jax array of int):  1D vector of indices into flattened array of size num_rows x num_cols.
             view_params (jax array):  A 1D array of view-specific parameters (such as angle) for the current view.
-            projector_params (tuple):  Tuple containing (sinogram_shape, recon_shape, get_geometry_params())
+            projector_params (namedtuple):  Tuple containing (sinogram_shape, recon_shape, get_geometry_params())
 
         Returns:
             jax array of shape (num_det_rows, num_det_channels)
         """
         warnings.warn('Forward projector not implemented for TomographyModel.')
         return None
 
@@ -115,15 +116,15 @@
         Note:
             This method must be overridden for a specific geometry.
 
         Args:
             sinogram_view (jax array): one view of the sinogram to be back projected
             pixel_indices (jax array of int):  1D vector of indices into flattened array of size num_rows x num_cols.
             single_view_params (jax array): A 1D array of view-specific parameters (such as angle) for the current view.
-            projector_params (tuple):  Tuple containing (sinogram_shape, recon_shape, get_geometry_params())
+            projector_params (namedtuple):  Tuple containing (sinogram_shape, recon_shape, get_geometry_params())
             coeff_power (int): backproject using the coefficients of (A_ij ** coeff_power).
                 Normally 1, but should be 2 for compute_hessian_diagonal.
 
         Returns:
             The value of the voxel for all slices at the input index (i.e., a voxel cylinder) obtained by backprojecting
             the input sinogram view.
         """
@@ -165,59 +166,65 @@
         """
         recon_shape = self.get_params('recon_shape')
         full_indices = mbirjax.gen_full_indices(recon_shape)
         recon = self.sparse_back_project(sinogram, full_indices)
 
         return self.reshape_recon(recon)
 
-    def sparse_forward_project(self, voxel_values, indices):
+    def sparse_forward_project(self, voxel_values, indices, view_indices=()):
         """
         Forward project the given voxel values to a sinogram.
         The indices are into a flattened 2D array of shape (recon_rows, recon_cols), and the projection is done using
         all voxels with those indices across all the slices.
 
         Args:
             voxel_values (jax.numpy.DeviceArray): 2D array of voxel values to project, size (len(pixel_indices), num_recon_slices).
             indices (numpy.ndarray): Array of indices specifying which voxels to project.
+            view_indices (ndarray or jax array, optional): 1D array of indices into the view parameters array.
+                If None, then all views are used.
 
         Returns:
             jnp array: The resulting 3D sinogram after projection.
         """
-        sinogram = self._sparse_forward_project(voxel_values, indices).block_until_ready()
+        sinogram = self.sparse_forward_project(voxel_values, indices, view_indices=view_indices).block_until_ready()
         gc.collect()
         return sinogram
 
-    def sparse_back_project(self, sinogram, indices):
+    def sparse_back_project(self, sinogram, indices, view_indices=()):
         """
         Back project the given sinogram to the voxels given by the indices.
         The indices are into a flattened 2D array of shape (recon_rows, recon_cols), and the projection is done using
         all voxels with those indices across all the slices.
 
         Args:
             sinogram (jnp array): 3D jax array containing sinogram.
             indices (jnp array): Array of indices specifying which voxels to back project.
+            view_indices (ndarray or jax array, optional): 1D array of indices into the view parameters array.
+                If None, then all views are used.
 
         Returns:
             A jax array of shape (len(indices), num_slices)
         """
-        recon_at_indices = self._sparse_back_project(sinogram, indices).block_until_ready()
+        recon_at_indices = self.sparse_back_project(sinogram, indices, view_indices=view_indices).block_until_ready()
         gc.collect()
         return recon_at_indices
 
-    def compute_hessian_diagonal(self, weights=None):
+    def compute_hessian_diagonal(self, weights=None, view_indices=()):
         """
         Computes the diagonal elements of the Hessian matrix for given weights.
 
         Args:
             weights (jnp array): Sinogram Weights for the Hessian computation.
+            view_indices (ndarray or jax array, optional): 1D array of indices into the view parameters array.
+                If None, then all views are used.
 
         Returns:
             jnp array: Diagonal of the Hessian matrix with same shape as recon.
         """
-        hessian = self._compute_hessian_diagonal(weights).block_until_ready()
+        hessian = self.compute_hessian_diagonal(weights, view_indices=view_indices).block_until_ready()
         gc.collect()
         return hessian
 
     def set_params(self, no_warning=False, no_compile=False, **kwargs):
         """
         Updates parameters using keyword arguments.
         After setting parameters, it checks if key geometry-related parameters have changed and, if so, recompiles the projectors.
@@ -238,21 +245,31 @@
         """
         Automatically sets the regularization parameters (self.sigma_y, self.sigma_x, and self.sigma_p) used in MBIR reconstruction based on the provided sinogram and optional weights.
 
         Args:
             sinogram (jnp.array): 3D jax array containing the sinogram with shape (num_views, num_det_rows, num_det_channels).
             weights (scalar or jnp.array, optional): Scalar value or 3D weights array with the same shape as the sinogram. Defaults to 1.
 
+        Returns:
+            namedtuple containing the parameters sigma_y, sigma_x, sigma_p
+
         The method adjusts the regularization parameters only if `auto_regularize_flag` is set to True within the model's parameters.
         """
         if self.get_params('auto_regularize_flag'):
             self.auto_set_sigma_y(sinogram, weights)
             self.auto_set_sigma_x(sinogram)
             self.auto_set_sigma_p(sinogram)
 
+        auto_param_names = ['sigma_y', 'sigma_x', 'sigma_p']
+        AutoParams = namedtuple('AutoParams', auto_param_names)
+        auto_param_values = self.get_params(auto_param_names)
+        auto_params = AutoParams(*tuple(auto_param_values))
+
+        return auto_params
+
     def auto_set_sigma_y(self, sinogram, weights=1):
         """
         Sets the value of the parameter sigma_y used for use in MBIR reconstruction.
 
         Args:
             sinogram (jax array): 3D jax array containing sinogram with shape (num_views, num_det_rows, num_det_channels).
             weights (scalar or 3D jax array): scalar value or 3D weights array with the same shape as sinogram.
@@ -393,44 +410,51 @@
             num_iterations (int): number of iterations of the VCD algorithm to perform.
             init_recon (jax array): optional reconstruction to be used for initialization.
 
         Returns:
             [recon, fm_rmse]: reconstruction and array of loss for each iteration.
         """
         # Run auto regularization. If auto_regularize_flag is False, then this will have no effect
-        self.auto_set_regularization_params(sinogram, weights=weights)
+        auto_params = self.auto_set_regularization_params(sinogram, weights=weights)
 
         # Generate set of voxel partitions
         recon_shape, granularity = self.get_params(['recon_shape', 'granularity'])
         partitions = mbirjax.gen_set_of_pixel_partitions(recon_shape, granularity)
 
         # Generate sequence of partitions to use
         partition_sequence = self.get_params('partition_sequence')
         partition_sequence = mbirjax.gen_partition_sequence(partition_sequence, num_iterations=num_iterations)
 
         # Compute reconstruction
         recon, fm_rmse = self.vcd_recon(sinogram, partitions, partition_sequence, weights=weights,
                                         init_recon=init_recon)
 
-        return recon, fm_rmse
+        # Return num_iterations, granularity, partition_sequence, fm_rmse values, auto_regularization_parameters
+        recon_param_names = ['num_iterations', 'granularity', 'partition_sequence', 'fm_rmse',
+                             'auto_regularization_parameters']
+        ReconParams = namedtuple('ReconParams', recon_param_names)
+        recon_param_values = [num_iterations, granularity, partition_sequence, fm_rmse, auto_params]
+        recon_params = ReconParams(*tuple(recon_param_values))
+
+        return recon, recon_params
 
     def vcd_recon(self, sinogram, partitions, partition_sequence, weights=1.0, init_recon=None, prox_input=None):
         """
         Perform MBIR reconstruction using the Multi-Granular Vector Coordinate Descent algorithm
         for a given set of partitions and a prescribed partition sequence.
 
         Args:
             sinogram (jax array): 3D sinogram data with shape (num_views, num_det_rows, num_det_channels).
             partitions (tuple): A collection of K partitions, with each partition being an (N_indices) integer index array of voxels to be updated in a flattened recon.
             partition_sequence (jax array): A sequence of integers that specify which partition should be used at each iteration.
             weights (scalar or jax array): scalar or 3D positive weights with same shape as error_sinogram.
             init_recon (jax array): Initial reconstruction to use in reconstruction.
 
         Returns:
-            [recon, fm_rmse]: reconstruction and array of loss for each iteration.
+            [recon, fm_rmse]: 3D reconstruction and array of loss for each iteration.
         """
         # Get required parameters
         num_iters = partition_sequence.size
         recon_shape = self.get_params('recon_shape')
 
         if init_recon is None:
             # Initialize VCD recon, and error sinogram
@@ -444,174 +468,241 @@
                                                                                               init_recon.shape)
                 raise ValueError(error_message)
 
             # Initialize VCD recon, and error sinogram
             recon = jnp.array(init_recon)
             error_sinogram = sinogram - self.forward_project(recon)
 
+        # Test to make sure the prox_input input is correct
+        if prox_input is not None:
+            # Make sure that prox_input has the correct size
+            if prox_input.shape != recon.shape:
+                error_message = "prox_input does not have the correct size. \n"
+                error_message += "Expected {}, but got shape {} for prox_input shape.".format(recon.shape,
+                                                                                              prox_input.shape)
+                raise ValueError(error_message)
+
+            # If used, make sure that prox_input has the correct a 3D shape and type
+            prox_input = jnp.array(prox_input.reshape(recon.shape))
+
         # Initialize the diagonal of the hessian of the forward model
-        hessian = self.compute_hessian_diagonal(weights=weights)
+        num_recon_slices = recon_shape[2]
+        fm_hessian = self.compute_hessian_diagonal(weights=weights).reshape((-1, num_recon_slices))
 
-        # Initialize forward model normalized RMSE error array
-        fm_rmse = np.zeros(num_iters)
+        # Initialize the emtpy recon
+        flat_recon = recon.reshape((-1, num_recon_slices))
+
+        # Create the finer grained recon update operators
+        vcd_subset_iterator = self.create_vcd_subset_iterator(fm_hessian, weights=weights, prox_input=prox_input)
+        vcd_partition_iterator = TomographyModel.create_vcd_partition_iterator(vcd_subset_iterator)
 
+        verbose, sigma_y = self.get_params(['verbose', 'sigma_y'])
+
+        if verbose >= 1:
+            print('Starting VCD iterations')
+            mbirjax.get_memory_stats(print_results=True)
+            print('--------')
+
+        # Do the iterations
+        fm_rmse = np.zeros(num_iters)
         for i in range(num_iters):
-            error_sinogram, recon = self.vcd_partition_iteration(error_sinogram, recon,
-                                                                 partitions[partition_sequence[i]], hessian,
-                                                                 weights=weights, prox_input=prox_input)
-            fm_rmse[i] = self.get_forward_model_loss(error_sinogram)
-            if self.get_params('verbose') >= 1:
+            partition = partitions[partition_sequence[i]]
+            subset_indices = np.random.permutation(partition.shape[0])
+            error_sinogram, flat_recon = vcd_partition_iterator([error_sinogram, flat_recon, partition], subset_indices)
+            fm_rmse[i] = self.get_forward_model_loss(error_sinogram, sigma_y)
+            if verbose >= 1:
                 print(f'VCD iteration={i}; Loss={fm_rmse[i]}')
+                mbirjax.get_memory_stats(print_results=True)
+                print('--------')
 
-        return recon, fm_rmse
+        return self.reshape_recon(flat_recon), fm_rmse
 
-    def vcd_partition_iteration(self, error_sinogram, recon, partition, fm_hessian, weights=1.0, prox_input=None):
+    @staticmethod
+    def create_vcd_partition_iterator(vcd_subset_iterator):
         """
-        Calculate an iteration of the VCD algorithm for each subset of the partition
-        Each iteration of the algorithm should return a better reconstructed recon. The error_sinogram should always be:
-        error_sinogram = measured_sinogram - forward_proj(recon)
-        where measured_sinogram is the measured sinogram and recon is the current reconstruction.
+        Create a jit-compiled function to update all the pixels in the recon and error sinogram by applying
+        the supplied vcd_subset_iterator to each subset in a partition.
 
         Args:
-            error_sinogram (jax array): 3D error sinogram with shape (num_views, num_det_rows, num_det_channels).
-            partition (int array): (K, N_indices) an integer index arrays that partitions
-                the voxels into K arrays, each of which indexes into a flattened recon.
-            recon (jax array): 3D array reconstruction with shape (num_recon_rows, num_recon_cols, num_recon_slices).
-            fm_hessian (jax array): Array with same shape as recon containing diagonal of hessian for forward model loss.
-            weights (scalar or jax array): scalar or 3D positive weights with same shape as error_sinogram.
+            vcd_subset_iterator (callable):  The function returned by create_vcd_subset_iterator.
 
         Returns:
-            [error_sinogram, recon]: Both have the same shape as above, but are updated to reduce overall loss function.
+            (callable) vcd_partition_iterator(error_sinogram, flat_recon, partition, subset_indices
         """
-        for subset in np.random.permutation(partition.shape[0]):
-            error_sinogram, recon = self.vcd_subset_iteration(error_sinogram, recon, partition[subset], fm_hessian,
-                                                              weights=weights, prox_input=prox_input)
-
-        return error_sinogram, recon
-
-    def vcd_subset_iteration(self, error_sinogram, recon, indices, fm_hessian, weights=1.0, prox_input=None):
-        """
-        Calculate an iteration of the VCD algorithm on a single subset of the partition
-        Each iteration of the algorithm should return a better reconstructed recon.
-        The combination of (error_sinogram, recon) form a overcomplete state that make computation efficient.
-        However, it is important that at each application the state should meet the constraint that:
-        error_sinogram = measured_sinogram - forward_proj(recon)
-        where measured_sinogram forward_proj() is whatever forward projection is being used in reconstruction.
-
-        Args:
-            error_sinogram (jax array): 3D error sinogram with shape (num_views, num_det_rows, num_det_channels).
-            indices (int array): (N_indices) integer index array of voxels to be updated in a flattened recon.
-            recon (jax array): 3D array reconstruction with shape (num_recon_rows, num_recon_cols, num_recon_slices).
-            fm_hessian (jax array): Array with same shape as recon containing diagonal of hessian for forward model loss.
-            weights (scalar or jax array): scalar or 3D positive weights with same shape as error_sinogram.
-            prox_input (jax array): optional input for proximal map with same shape as reconstruction.
 
-        Returns:
-            [error_sinogram, recon]: Both have the same shape as above, but are updated to reduce overall loss function.
-        """
-        # Get positivity flag
-        positivity_flag = self.get_params('positivity_flag')
+        def vcd_partition_iterator(sinogram_recon_partition, subset_indices):
+            """
+            Calculate a full iteration of the VCD algorithm by scanning over the subsets of the partition.
+            Each iteration of the algorithm should return a better reconstructed recon.
+            The error_sinogram should always be:  error_sinogram = measured_sinogram - forward_proj(recon)
+            where measured_sinogram is the measured sinogram and recon is the current reconstruction.
 
-        # Recover recon shape parameters and make sure that recon has a 3D shape
-        recon = self.reshape_recon(recon)
+            Args:
+                sinogram_recon_partition (list): 3 element tuple containing
 
-        # Test to make sure the prox_input input is correct
-        if prox_input is not None:
-            # Make sure that prox_input has the correct size
-            if prox_input.size != recon.size:
-                error_message = "prox_input does not have the correct size. \n"
-                error_message += "Expected {}, but got shape {} for prox_input shape.".format(recon.size,
-                                                                                              prox_input.size)
-                raise ValueError(error_message)
+                    * error_sinogram (jax array): 3D error sinogram with shape (num_views, num_det_rows, num_det_channels).
+                    * flat_recon (jax array): 2D array reconstruction with shape (num_recon_rows x num_recon_cols, num_recon_slices).
+                    * partition (jax array): 2D array where partition[subset_index] gives a 1D array of pixel indices.
 
-            # If used, make sure that prox_input has the correct a 3D shape and type
-            prox_input = jnp.array(prox_input.reshape(recon.shape))
+                subset_indices (jax array): An array of indices into the partition - this gives the order in which the subsets are updated.
 
-        # flatten the hessian if it is not already flat
-        num_recon_slices = recon.shape[2]
-        fm_hessian = fm_hessian.reshape((-1, num_recon_slices))
-
-        # Compute the forward model gradient and hessian at each pixel in the index set.
-        # Assumes Loss(delta) = 1/(2 sigma_y^2) || error_sinogram - A delta ||_weights^2
-        constant = 1.0 / (self.get_params('sigma_y') ** 2.0)
-
-        fm_gradient = -constant * self._sparse_back_project(error_sinogram * weights, indices)
-        fm_sparse_hessian = constant * fm_hessian[indices]
-
-        # Compute the prior model gradient and hessian (i.e., second derivative) terms
-        if prox_input is None:
-            # This is for the qGGMRF prior
-            # Compute the prior model gradient and hessian at each pixel in the index set.
-            sigma_x, p, q, T, b = self.get_params(['sigma_x', 'p', 'q', 'T', 'b'])
-            pm_gradient, pm_hessian = pm_qggmrf_gradient_and_hessian_at_indices(recon, indices, sigma_x, p, q, T, b)
-        else:
-            # This is for the proximal map prior
-            sigma_p = self.get_params('sigma_p')
-            pm_hessian = sigma_p ** 2
+            Returns:
+                [error_sinogram, recon]: Both have the same shape as above, but are updated to reduce overall loss function.
+            """
 
-            # Compute the prior model gradient at each pixel in the index set.
-            pm_gradient = pm_prox_gradient_at_indices(recon, prox_input, indices, sigma_p)
+            # Scan over the subsets of the partition, using the subset_indices to order them.
+            sinogram_recon_partition, _ = jax.lax.scan(vcd_subset_iterator, sinogram_recon_partition, subset_indices)
 
-        # Compute update vector update direction in recon domain
-        delta_recon_at_indices = (- fm_gradient - pm_gradient) / (fm_sparse_hessian + pm_hessian)
+            error_sinogram, flat_recon, _ = sinogram_recon_partition
+            return error_sinogram, flat_recon
 
-        # Compute update direction in sinogram domain
-        delta_sinogram = self._sparse_forward_project(delta_recon_at_indices, indices)
+        return jax.jit(vcd_partition_iterator)
 
-        # Compute "optimal" update step
-        # This is really only optimal for the forward model component.
-        # We can compute the truly optimal update, but it's complicated so maybe this is good enough
-        alpha = jnp.sum(error_sinogram * delta_sinogram * weights) / (
-                    jnp.sum(delta_sinogram * delta_sinogram * weights) + jnp.finfo(np.float32).eps)
-        # TODO: test for alpha<0 and terminate.
+    def create_vcd_subset_iterator(self, fm_hessian, weights=1.0, prox_input=None):
+        """
+        Create a jit-compiled function to update a subset of pixels in the recon and error sinogram.
 
-        # Flatten recon for next steps
-        recon = recon.reshape((-1, num_recon_slices))
+        Args:
+            fm_hessian (jax array): Array with same shape as recon containing diagonal of hessian for forward model loss.
+            weights (scalar or jax array): scalar or 3D positive weights with same shape as error_sinogram.
+            prox_input (jax array): optional input for proximal map with same shape as reconstruction.
 
-        # Enforce positivity constraint if desired
-        # Greg, this may result in excess compilation. Not sure.
-        if positivity_flag is True:
-            # Get recon at indices
-            recon_at_indices = recon[indices]
+        Returns:
+            (callable) vcd_subset_iterator(error_sinogram, flat_recon, pixel_indices) that updates the recon.
+        """
 
-            # Clip updates to ensure non-negativity
-            constant = 1.0 / (alpha + jnp.finfo(np.float32).eps)
-            delta_recon_at_indices = jnp.maximum(-constant * recon_at_indices, delta_recon_at_indices)
+        positivity_flag = self.get_params('positivity_flag')
+        fm_constant = 1.0 / (self.get_params('sigma_y') ** 2.0)
+        sigma_x, p, q, T, b = self.get_params(['sigma_x', 'p', 'q', 'T', 'b'])
+        sigma_p = self.get_params('sigma_p')
+        pixel_batch_size = self.get_params('pixel_batch_size')
+        recon_shape = self.get_params('recon_shape')
+        sparse_back_project = self.sparse_back_project
+        sparse_forward_project = self.sparse_forward_project
 
-            # Recompute sinogram projection
-            delta_sinogram = self._sparse_forward_project(delta_recon_at_indices, indices)
+        def vcd_subset_iterator(sinogram_recon_partition, subset_index):
+            """
+            Calculate an iteration of the VCD algorithm on a single subset of the partition
+            Each iteration of the algorithm should return a better reconstructed recon.
+            The combination of (error_sinogram, recon) forms an overcomplete state that makes computation efficient.
+            However, it is important that at each application the state should meet the constraint that:
+            error_sinogram = measured_sinogram - forward_proj(recon)
+            where measured_sinogram forward_proj() is whatever forward projection is being used in reconstruction.
+
+            Args:
+                sinogram_recon_partition (list): 3 element tuple containing
+
+                    * error_sinogram (jax array): 3D error sinogram with shape (num_views, num_det_rows, num_det_channels).
+                    * flat_recon (jax array): 2D array reconstruction with shape (num_recon_rows x num_recon_cols, num_recon_slices).
+                    * partition (jax array): 2D array where partition[subset_index] gives a 1D array of pixel indices.
+
+                subset_index (int): integer index of the subset within the partition.
+
+            Returns:
+                [error_sinogram, flat_recon]: Both have the same shape as above, but are updated to reduce overall loss function.
+            """
+            error_sinogram, flat_recon, partition = sinogram_recon_partition
+            pixel_indices = partition[subset_index]
+
+            def delta_recon_batch(index_batch):
+                # Compute the forward model gradient and hessian at each pixel in the index set.
+                # Assumes Loss(delta) = 1/(2 sigma_y^2) || error_sinogram - A delta ||_weights^2
+                fm_gradient = -fm_constant * sparse_back_project(error_sinogram * weights, index_batch)
+                fm_sparse_hessian = fm_constant * fm_hessian[index_batch]
+
+                # Compute the prior model gradient and hessian (i.e., second derivative) terms
+                if prox_input is None:
+                    # This is for the qGGMRF prior - compute the prior model gradient and hessian at each pixel in the index set.
+                    pm_gradient, pm_hessian = pm_qggmrf_gradient_and_hessian_at_indices(flat_recon, recon_shape, index_batch, sigma_x, p, q, T, b)
+                else:
+                    # This is for the proximal map prior - compute the prior model gradient at each pixel in the index set.
+                    pm_hessian = sigma_p ** 2
+                    pm_gradient = pm_prox_gradient_at_indices(flat_recon, prox_input, index_batch, sigma_p)
+
+                # Compute update vector update direction in recon domain
+                delta_recon_at_indices_batch = (- fm_gradient - pm_gradient) / (fm_sparse_hessian + pm_hessian)
+                return delta_recon_at_indices_batch
+
+            # Apply the function on a single batch of pixels if the batch is small enough
+            num_pixels = len(pixel_indices)
+            max_index_subsets = 10
+            cur_pixel_batch_size = max(pixel_batch_size, flat_recon.shape[0] // (max_index_subsets - 1))
+            if cur_pixel_batch_size >= num_pixels:
+                delta_recon_at_indices = delta_recon_batch(pixel_indices)
+
+            # Otherwise batch the pixels and map over the batches.
+            else:
+                num_batches = num_pixels // cur_pixel_batch_size
+                length_of_batches = num_batches * cur_pixel_batch_size
+                pixel_indices_batched = jnp.reshape(pixel_indices[:length_of_batches], (num_batches, cur_pixel_batch_size))
+
+                batched_voxel_values = jax.lax.map(delta_recon_batch, pixel_indices_batched)
+                delta_recon_at_indices = batched_voxel_values.reshape((length_of_batches,) + batched_voxel_values.shape[2:])
+
+                # Add in any leftover pixels
+                num_remaining = num_pixels - num_batches * cur_pixel_batch_size
+                if num_remaining > 0:
+                    end_batch_indices = pixel_indices[-num_remaining:]
+                    end_batch_voxel_values = delta_recon_batch(end_batch_indices)
+                    delta_recon_at_indices = jnp.concatenate((delta_recon_at_indices, end_batch_voxel_values), axis=0)
+
+            # Compute update direction in sinogram domain
+            delta_sinogram = sparse_forward_project(delta_recon_at_indices, pixel_indices)
+
+            # Compute "optimal" update step
+            # This is really only optimal for the forward model component.
+            # We can compute the truly optimal update, but it's complicated so maybe this is good enough
+            alpha = jnp.sum(error_sinogram * delta_sinogram * weights) / (
+                        jnp.sum(delta_sinogram * delta_sinogram * weights) + jnp.finfo(np.float32).eps)
+            # TODO: test for alpha<0 and terminate.
+
+            # Enforce positivity constraint if desired
+            # Greg, this may result in excess compilation. Not sure.
+            if positivity_flag is True:
+                # Get recon at index_batch
+                recon_at_indices = flat_recon[pixel_indices]
+
+                # Clip updates to ensure non-negativity
+                pos_constant = 1.0 / (alpha + jnp.finfo(np.float32).eps)
+                delta_recon_at_indices = jnp.maximum(-pos_constant * recon_at_indices, delta_recon_at_indices)
+
+                # Recompute sinogram projection
+                delta_sinogram = sparse_forward_project(delta_recon_at_indices, pixel_indices)
+
+            # Perform sparse updates at index locations
+            flat_recon = flat_recon.at[pixel_indices].add(alpha * delta_recon_at_indices)
 
-        # Perform sparse updates at index locations, and reshape as 3D array
-        recon = recon.at[indices].add(alpha * delta_recon_at_indices)
-        recon = self.reshape_recon(recon)
+            # Update sinogram
+            error_sinogram = error_sinogram - alpha * delta_sinogram
 
-        # Update sinogram
-        error_sinogram = error_sinogram - alpha * delta_sinogram
+            return [error_sinogram, flat_recon, partition], None
 
-        return error_sinogram, recon
+        return jax.jit(vcd_subset_iterator)
 
-    def get_forward_model_loss(self, error_sinogram, weights=1.0, normalize=True):
+    @staticmethod
+    def get_forward_model_loss(error_sinogram, sigma_y, weights=1.0, normalize=True):
         """
         Calculate the loss function for the forward model from the error_sinogram and weights.
         The error sinogram should be error_sinogram = measured_sinogram - forward_proj(recon)
 
         Args:
             error_sinogram (jax array): 3D error sinogram with shape (num_views, num_det_rows, num_det_channels).
+            sigma_y (float): Estimate obtained from auto_set_sigma_y or get_params('sigma_y')
             weights (jax array, optional, default=1.0): 3D weights array with same shape as sinogram
             normalize (bool, optional, default=True):  If true, then
 
         Returns:
             [loss].
         """
         if normalize:
             avg_weight = jnp.average(weights)
-            loss = jnp.sqrt((1.0 / (self.get_params('sigma_y') ** 2)) * jnp.mean(
+            loss = jnp.sqrt((1.0 / (sigma_y ** 2)) * jnp.mean(
                 (error_sinogram * error_sinogram) * (weights / avg_weight)))
         else:
-            loss = (1.0 / (2 * self.get_params('sigma_y') ** 2)) * jnp.sum((error_sinogram * error_sinogram) * weights)
+            loss = (1.0 / (2 * sigma_y ** 2)) * jnp.sum((error_sinogram * error_sinogram) * weights)
         return loss
 
     def prox_map(self, prox_input, sinogram, weights=1.0, num_iterations=3, init_recon=None):
         """
         Proximal Map function for use in Plug-and-Play applications.
         This function is similar to recon, but it essentially uses a prior with a mean of prox_input and a standard deviation of sigma_p.
 
@@ -684,20 +775,19 @@
         return phantom
 
     def reshape_recon(self, recon):
         """
         Reshape recon into its 3D form.
 
         Args:
-            recon (ndarray or jnp.array): A 3D numpy array of shape specified by (num_recon_rows, num_recon_cols, num_recon_slices)
+            recon (ndarray or jax array): A 3D array of shape specified by (num_recon_rows, num_recon_cols, num_recon_slices)
         """
         recon_shape = self.get_params('recon_shape')
         return recon.reshape(recon_shape)
 
-
 @jax.jit
 def pm_gradient_and_hessian(delta_prime, b, sigma_x, p, q, T):
     """
     Computes the first and second derivatives of the surrogate function at a pixel for the qGGMRF prior model.
     Calculations taken from Figure 8.5 (page 119) of FCI for the qGGMRF prior model.
 
     Args:
@@ -716,22 +806,23 @@
 
     # Compute second derivative
     pm_second_derivative = jnp.sum(2 * btilde, axis=-1)
 
     return pm_first_derivative, pm_second_derivative
 
 
-@jax.jit
-def pm_qggmrf_gradient_and_hessian_at_indices(recon, indices, sigma_x, p, q, T, b):
+@partial(jax.jit, static_argnames='recon_shape')
+def pm_qggmrf_gradient_and_hessian_at_indices(voxel_values, recon_shape, pixel_indices, sigma_x, p, q, T, b):
     """
     Calculate the gradient and hessian at each index location in a reconstructed image using the qGGMRF prior.
 
     Args:
-        recon (jax.array): 3D reconstructed image array with shape (num_recon_rows, num_recon_cols, num_recon_slices).
-        indices (int array): Array of shape (N_indices, num_recon_slices) representing the indices of voxels in a flattened array to be updated.
+        voxel_values (jax.array): 2D reconstructed image array with shape (num_recon_rows x num_recon_cols, num_recon_slices).
+        recon_shape (tuple of ints): shape of the original recon:  (num_recon_rows, num_recon_cols, num_recon_slices).
+        pixel_indices (int array): Array of shape (N_indices, num_recon_slices) representing the indices of voxels in a flattened array to be updated.
         sigma_x (float): Standard deviation parameter of the qGGMRF prior.
         p (float): Norm parameter p in the qGGMRF prior.
         q (float): Norm parameter q in the qGGMRF prior.
         T (float): Scaling parameter in the qGGMRF prior.
         b (list of 6 float): list of 6 qGGMRF prior neightborhood weights.
 
     Returns:
@@ -740,28 +831,31 @@
     """
     # Initialize the neighborhood weights for averaging surrounding pixel values.
     # Order is (I think) [row+1, row-1, col+1, col-1, slice+1, slice-1]
     b = jnp.array(b).reshape(1, -1)
     b /= jnp.sum(b)
 
     # Extract the shape of the reconstruction array.
-    num_rows, num_cols, num_slices = recon.shape[:3]
+    num_rows, num_cols, num_slices = recon_shape[:3]
 
     # Convert flat indices to 2D indices for row and column access.
-    row_index, col_index = jnp.unravel_index(indices, shape=(num_rows, num_cols))
+    row_index, col_index = jnp.unravel_index(pixel_indices, shape=(num_rows, num_cols))
 
-    # Access the central voxels' values at the given indices. Shape of xs is (num indices)x(num slices)
-    xs = recon[row_index, col_index]
+    # Access the central voxels' values at the given pixel_indices. Shape of xs is (num indices)x(num slices)
+    xs = voxel_values[pixel_indices]
 
     # Define relative positions for accessing neighborhood voxels.
     offsets = [[1, 0], [-1, 0], [0, 1], [0, -1]]
 
     # Create a list derived from 4 neighbors, each entry in list is a 1D vector containing the recon values at that
     # location over all slices.
-    xr = [recon[row_index + offset[0], col_index + offset[1]] for offset in offsets]
+    xr = []
+    for offset in offsets:
+        new_indices = jnp.ravel_multi_index([row_index + offset[0], col_index + offset[1]], dims=(num_rows, num_cols), mode='clip')
+        xr.append(voxel_values[new_indices])
 
     # Shift slices up with zero padding
     xs_up = jnp.roll(xs, shift=-1, axis=1).at[:, -1].set(0)
 
     # Shift slices down with zero padding
     xs_down = jnp.roll(xs, shift=1, axis=1).at[:, 0].set(0)
 
@@ -784,33 +878,30 @@
     first_derivative = first_derivative.reshape(-1, num_slices)
     second_derivative = second_derivative.reshape(-1, num_slices)
 
     return first_derivative, second_derivative
 
 
 @jax.jit
-def pm_prox_gradient_at_indices(recon, prox_input, indices, sigma_p):
+def pm_prox_gradient_at_indices(recon, prox_input, pixel_indices, sigma_p):
     """
     Calculate the gradient and hessian at each index location in a reconstructed image using the qGGMRF prior.
 
     Args:
-        recon (jax.array): 3D reconstructed image array with shape (num_recon_rows, num_recon_cols, num_recon_slices).
-        recon (jax.array): 3D reconstructed image array with shape (num_recon_rows, num_recon_cols, num_recon_slices).
-        indices (int array): Array of shape (N_indices, num_recon_slices) representing the indices of voxels in a flattened array to be updated.
+        recon (jax.array): 2D reconstructed image array with shape (num_recon_rows x num_recon_cols, num_recon_slices).
+        prox_input (jax.array): 2D reconstructed image array with shape (num_recon_rows x num_recon_cols, num_recon_slices).
+        pixel_indices (int array): Array of shape (N_indices, num_recon_slices) representing the indices of voxels in a flattened array to be updated.
         sigma_p (float): Standard deviation parameter of the proximal map.
 
     Returns:
         first_derivative of shape (N_indices, num_recon_slices) representing the gradient of the prox term at specified indices.
     """
-    # Convert flat indices to 2D indices for row and column access.
-    num_rows, num_cols = recon.shape[:2]
-    row_index, col_index = jnp.unravel_index(indices, shape=(num_rows, num_cols))
 
     # Compute the prior model gradient at all voxels
-    cur_diff = recon[row_index, col_index] - prox_input[row_index, col_index]
+    cur_diff = recon[pixel_indices] - prox_input[pixel_indices]
     pm_gradient = (1.0 / (sigma_p ** 2.0)) * cur_diff
 
     # Shape of pm_gradient is (num indices)x(num slices)
     return pm_gradient
 
 
 def _get_rho(delta, b, sigma_x, p, q, T):
```

### Comparing `mbirjax-0.1.0/mbirjax/vcd_utils.py` & `mbirjax-0.2.0/mbirjax/vcd_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 import jax.numpy as jnp
+import jax
 
 
 def get_2d_ror_mask(recon_shape):
     """
     Get a binary mask for the region of reconstruction.
 
     Args:
@@ -126,45 +127,14 @@
     """
     partition = gen_pixel_partition(recon_shape, num_subsets=1)
     full_indices = partition[0]
 
     return full_indices
 
 
-def gen_indices_d2(recon_shape, block_width):
-    """
-    Generates an index array for a 2D reconstruction using a block size of block_width x block_width
-
-    Args:
-        recon_shape (tuple): Shape of recon in (rows, columns, slices)
-        block_width (int): side length of block
-
-    Returns:
-
-    """
-    num_recon_rows, num_recon_cols = recon_shape[:2]
-    max_index_val = num_recon_rows * num_recon_cols
-
-    # Make sure rows and columns are divisible by block_width, but make sure to round up
-    num_recon_rows = block_width * ((num_recon_rows // block_width) + (num_recon_rows % block_width))
-    num_recon_cols = block_width * ((num_recon_cols // block_width) + (num_recon_cols % block_width))
-
-    # Generate an array, but make sure its values don't go outside the valid range
-    indices = np.arange(num_recon_rows * num_recon_cols) % max_index_val
-
-    indices = indices.reshape(num_recon_rows, num_recon_cols // block_width, block_width)
-    indices = np.transpose(indices, axes=(2, 1, 0))
-    indices = indices.reshape(block_width, num_recon_cols // block_width, num_recon_rows // block_width, block_width)
-    indices = np.transpose(indices, axes=(0, 3, 2, 1))
-    indices = indices.reshape(block_width * block_width,
-                              (num_recon_rows // block_width) * (num_recon_cols // block_width))
-
-    return jnp.array(indices)
-
-
 def gen_cube_phantom(recon_shape):
     """Code to generate a simple phantom """
     # Compute phantom height and width
     num_recon_rows, num_recon_cols, num_recon_slices = recon_shape[:3]
     phantom_rows = num_recon_rows // 4  # Phantom height
     phantom_cols = num_recon_cols // 4  # Phantom width
 
@@ -180,38 +150,64 @@
         shift_cols = int(slice_index * phantom_cols / num_recon_slices)
         phantom[start_rows:stop_rows, (shift_cols + start_cols):(shift_cols + stop_cols), slice_index] = 1.0 / max(
             phantom_rows, phantom_cols)
 
     return jnp.array(phantom)
 
 
-def ellipsoid(x0, y0, z0, a, b, c, N, M, P, angle=0, intensity=1.0):
-    x = jnp.linspace(-1, 1, N)
-    y = jnp.linspace(-1, 1, M)
-    z = jnp.linspace(-1, 1, P)
-    X, Y, Z = jnp.meshgrid(x, y, z, indexing='ij')
-
-    cos_angle = jnp.cos(np.deg2rad(angle))
-    sin_angle = jnp.sin(np.deg2rad(angle))
-    Xr = cos_angle * (X - x0) + sin_angle * (Y - y0)
-    Yr = -sin_angle * (X - x0) + cos_angle * (Y - y0)
-    Zr = Z - z0
+@jax.jit
+def add_ellipsoid(current_volume, grids, z_locations, x0, y0, z0, a, b, c, angle=0, intensity=1.0):
+    """
+    Add an ellipsoid to an existing jax array.  This is done using lax.scan over the z slices to avoid
+    using really large arrays when the volume is large.
+
+    Args:
+        current_volume (jax array): 3D volume
+        grids (tuple):  A tuple of x_grid, y_grid, i_grid, j_grid obtained as in generate_3d_shepp_logan_low_dynamic_range
+        z_locations (jax array): A 1D array of z coordinates of the volume
+        x0 (float): x center for the ellipsoid
+        y0 (float): y center for the ellipsoid
+        z0 (float): z center for the ellipsoid
+        a (float): x radius
+        b (float): y radius
+        c (float): z radius
+        angle (float): angle of rotation of the ellipsoid in the xy plane around (x0, y0)
+        intensity (float): The constant value of the ellipsoid to be added.
+
+    Returns:
+        3D jax array: current_volume + ellipsoid
+    """
+
+    # Unpack the grids and determine the xy locations for this angle
+    x_grid, y_grid, i_grid, j_grid = grids
+    cos_angle = jnp.cos(jnp.deg2rad(angle))
+    sin_angle = jnp.sin(jnp.deg2rad(angle))
+    Xr = cos_angle * (x_grid - x0) + sin_angle * (y_grid - y0)
+    Yr = -sin_angle * (x_grid - x0) + cos_angle * (y_grid - y0)
+
+    # Determine which xy locations will be updated for this ellipsoid
+    xy_norm = Xr**2 / a**2 + Yr**2 / b**2
+
+    def add_slice_vmap(volume_slice, z):
+        return volume_slice + intensity * ((xy_norm + (z - z0)**2 / c**2) <= 1).astype(float)
+
+    volume_map = jax.vmap(add_slice_vmap, in_axes=(2, 0), out_axes=2)
+    current_volume = volume_map(current_volume, z_locations)
 
-    ellipsoid = (Xr**2 / a**2 + Yr**2 / b**2 + Zr**2 / c**2) <= 1
-    return ellipsoid * intensity
+    return current_volume
 
 
 def _gen_ellipsoid(x_grid, y_grid, z_grid, x0, y0, z0, a, b, c, gray_level, alpha=0, beta=0, gamma=0):
     """
     Return an image with a 3D ellipsoid in a 3D plane with a center of [x0,y0,z0] and ...
 
     Args:
-        x_grid(float): 3D grid of X coordinate values.
-        y_grid(float): 3D grid of Y coordinate values.
-        z_grid(float): 3D grid of Z coordinate values.
+        x_grid(jax array): 3D grid of X coordinate values.
+        y_grid(jax array): 3D grid of Y coordinate values.
+        z_grid(jax array): 3D grid of Z coordinate values.
         x0(float): horizontal center of ellipsoid.
         y0(float): vertical center of ellipsoid.
         z0(float): normal center of ellipsoid.
         a(float): X-axis radius.
         b(float): Y-axis radius.
         c(float): Z-axis radius.
         gray_level(float): Gray level for the ellipse.
@@ -240,20 +236,22 @@
 def generate_3d_shepp_logan_reference(phantom_shape):
     """
     Generate a 3D Shepp Logan phantom based on below reference.
 
     Kak AC, Slaney M. Principles of computerized tomographic imaging. Page.102. IEEE Press, New York, 1988. https://engineering.purdue.edu/~malcolm/pct/CTI_Ch03.pdf
 
     Args:
-        num_rows: int, number of rows.
-        num_cols: int, number of cols.
-        num_slices: int, number of slices.
+        phantom_shape (tuple or list of ints): num_rows, num_cols, num_slices
 
     Return:
         out_image: 3D array, num_slices*num_rows*num_cols
+
+    Note:
+        This function produces 6 intermediate arrays that each have shape phantom_shape, so if phantom_shape is
+        large, then this will use a lot of peak memory.
     """
 
     # The function describing the phantom is defined as the sum of 10 ellipsoids inside a 2×2×2 cube:
     sl3d_paras = [
         {'x0': 0.0, 'y0': 0.0, 'z0': 0.0, 'a': 0.69, 'b': 0.92, 'c': 0.9, 'gamma': 0, 'gray_level': 2.0},
         {'x0': 0.0, 'y0': 0.0, 'z0': 0.0, 'a': 0.6624, 'b': 0.874, 'c': 0.88, 'gamma': 0, 'gray_level': -0.98},
         {'x0': -0.22, 'y0': 0.0, 'z0': -0.25, 'a': 0.41, 'b': 0.16, 'c': 0.21, 'gamma': 108, 'gray_level': -0.02},
@@ -289,24 +287,34 @@
     Generates a 3D Shepp-Logan phantom with specified dimensions.
 
     Args:
         phantom_shape (tuple): Phantom shape in (rows, columns, slices).
 
     Returns:
         ndarray: A 3D numpy array of shape phantom_shape representing the voxel intensities of the phantom.
+
+    Note:
+        This function uses a memory-efficient approach to generating large phantoms.
     """
-    phantom = np.zeros(phantom_shape)
+    # Get space for the result and set up the grids for add_ellipsoid
+    phantom = jnp.zeros(phantom_shape)
     N, M, P = phantom_shape
+    x_locations = jnp.linspace(-1, 1, N)
+    y_locations = jnp.linspace(-1, 1, M)
+    z_locations = jnp.linspace(-1, 1, P)
+    x_grid, y_grid = jnp.meshgrid(x_locations, y_locations, indexing='ij')
+    i_grid, j_grid = jnp.meshgrid(jnp.arange(N), jnp.arange(M), indexing='ij')
+    grids = (x_grid, y_grid, i_grid, j_grid)
 
     # Main ellipsoid
-    phantom += ellipsoid(0, 0, 0, 0.69, 0.92, 0.9, N, M, P, intensity=1)
+    phantom = add_ellipsoid(phantom, grids, z_locations, 0, 0, 0, 0.69, 0.92, 0.9, intensity=1)
     # Smaller ellipsoids and other structures
-    phantom += ellipsoid(0, 0.0184, 0, 0.6624, 0.874, 0.88, N, M, P, intensity=-0.8)
-    phantom += ellipsoid(0.22, 0, 0, 0.41, 0.16, 0.21, N, M, P, angle=108, intensity=-0.2)
-    phantom += ellipsoid(-0.22, 0, 0, 0.31, 0.11, 0.22, N, M, P, angle=72, intensity=-0.2)
-    phantom += ellipsoid(0, 0.35, 0, 0.21, 0.25, 0.5, N, M, P, intensity=0.1)
-    phantom += ellipsoid(0, 0.1, 0, 0.046, 0.046, 0.046, N, M, P, intensity=0.1)
-    phantom += ellipsoid(0, -0.1, 0, 0.046, 0.046, 0.046, N, M, P, intensity=0.1)
-    phantom += ellipsoid(-0.08, -0.605, 0, 0.046, 0.023, 0.02, N, M, P, angle=0, intensity=0.1)
-    phantom += ellipsoid(0, -0.605, 0, 0.023, 0.023, 0.02, N, M, P, angle=0, intensity=0.1)
+    phantom = add_ellipsoid(phantom, grids, z_locations, 0, 0.0184, 0, 0.6624, 0.874, 0.88, intensity=-0.8)
+    phantom = add_ellipsoid(phantom, grids, z_locations, 0.22, 0, 0, 0.41, 0.16, 0.21, angle=108, intensity=-0.2)
+    phantom = add_ellipsoid(phantom, grids, z_locations, -0.22, 0, 0, 0.31, 0.11, 0.22, angle=72, intensity=-0.2)
+    phantom = add_ellipsoid(phantom, grids, z_locations, 0, 0.35, 0, 0.21, 0.25, 0.5, intensity=0.1)
+    phantom = add_ellipsoid(phantom, grids, z_locations, 0, 0.1, 0, 0.046, 0.046, 0.046, intensity=0.1)
+    phantom = add_ellipsoid(phantom, grids, z_locations, 0, -0.1, 0, 0.046, 0.046, 0.046, intensity=0.1)
+    phantom = add_ellipsoid(phantom, grids, z_locations, -0.08, -0.605, 0, 0.046, 0.023, 0.02, angle=0, intensity=0.1)
+    phantom = add_ellipsoid(phantom, grids, z_locations, 0, -0.605, 0, 0.023, 0.023, 0.02, angle=0, intensity=0.1)
 
-    return jnp.array(phantom)
+    return phantom
```

### Comparing `mbirjax-0.1.0/tests/test_projectors.py` & `mbirjax-0.2.0/tests/test_projectors.py`

 * *Files identical despite different names*

