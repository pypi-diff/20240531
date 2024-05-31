# Comparing `tmp/ngcsimlib-0.2b2.tar.gz` & `tmp/ngcsimlib-0.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngcsimlib-0.2b2.tar", last modified: Sat Mar 30 17:59:16 2024, max compression
+gzip compressed data, was "ngcsimlib-0.3b0.tar", last modified: Fri May 31 17:22:28 2024, max compression
```

## Comparing `ngcsimlib-0.2b2.tar` & `ngcsimlib-0.3b0.tar`

### file list

```diff
@@ -1,30 +1,54 @@
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-30 17:59:16.104944 ngcsimlib-0.2b2/
--rw-rw-r--   0 ago       (1001) ago       (1001)      286 2024-03-28 18:07:06.000000 ngcsimlib-0.2b2/AUTHORS
--rw-rw-r--   0 ago       (1001) ago       (1001)     1548 2024-03-28 18:07:59.000000 ngcsimlib-0.2b2/LICENSE
--rw-r--r--   0 ago       (1001) ago       (1001)     3132 2024-03-30 17:59:16.104944 ngcsimlib-0.2b2/PKG-INFO
--rw-rw-r--   0 ago       (1001) ago       (1001)     2634 2024-03-28 18:03:49.000000 ngcsimlib-0.2b2/README.md
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-30 17:59:16.100944 ngcsimlib-0.2b2/ngcsimlib/
--rw-rw-r--   0 ago       (1001) ago       (1001)     1862 2024-03-30 17:52:23.000000 ngcsimlib-0.2b2/ngcsimlib/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     2882 2024-03-28 17:44:52.000000 ngcsimlib-0.2b2/ngcsimlib/bundle_rules.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-30 17:59:16.104944 ngcsimlib-0.2b2/ngcsimlib/commands/
--rw-rw-r--   0 ago       (1001) ago       (1001)      291 2024-03-28 17:48:02.000000 ngcsimlib-0.2b2/ngcsimlib/commands/__init__.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     1027 2024-03-28 17:47:21.000000 ngcsimlib-0.2b2/ngcsimlib/commands/advanceState.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     2386 2024-03-28 17:47:28.000000 ngcsimlib-0.2b2/ngcsimlib/commands/clamp.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     1330 2024-03-28 17:47:40.000000 ngcsimlib-0.2b2/ngcsimlib/commands/command.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     1641 2024-03-28 17:47:48.000000 ngcsimlib-0.2b2/ngcsimlib/commands/compound.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     1538 2024-03-28 17:47:56.000000 ngcsimlib-0.2b2/ngcsimlib/commands/evolve.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     1841 2024-03-28 17:48:13.000000 ngcsimlib-0.2b2/ngcsimlib/commands/multiclamp.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     1664 2024-03-28 17:48:22.000000 ngcsimlib-0.2b2/ngcsimlib/commands/reset.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     2169 2024-03-28 17:48:38.000000 ngcsimlib-0.2b2/ngcsimlib/commands/save.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     1605 2024-03-28 17:48:50.000000 ngcsimlib-0.2b2/ngcsimlib/commands/snapshot.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     2144 2024-03-28 17:49:02.000000 ngcsimlib-0.2b2/ngcsimlib/commands/track.py
--rw-rw-r--   0 ago       (1001) ago       (1001)    15447 2024-03-28 17:45:13.000000 ngcsimlib-0.2b2/ngcsimlib/component.py
--rw-rw-r--   0 ago       (1001) ago       (1001)    16547 2024-03-28 17:45:50.000000 ngcsimlib-0.2b2/ngcsimlib/controller.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     7977 2024-03-28 17:46:35.000000 ngcsimlib-0.2b2/ngcsimlib/utils.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-30 17:59:16.104944 ngcsimlib-0.2b2/ngcsimlib.egg-info/
--rw-r--r--   0 ago       (1001) ago       (1001)     3132 2024-03-30 17:59:16.000000 ngcsimlib-0.2b2/ngcsimlib.egg-info/PKG-INFO
--rw-rw-r--   0 ago       (1001) ago       (1001)      617 2024-03-30 17:59:16.000000 ngcsimlib-0.2b2/ngcsimlib.egg-info/SOURCES.txt
--rw-rw-r--   0 ago       (1001) ago       (1001)        1 2024-03-30 17:59:16.000000 ngcsimlib-0.2b2/ngcsimlib.egg-info/dependency_links.txt
--rw-rw-r--   0 ago       (1001) ago       (1001)       10 2024-03-30 17:59:16.000000 ngcsimlib-0.2b2/ngcsimlib.egg-info/top_level.txt
--rw-rw-r--   0 ago       (1001) ago       (1001)      598 2024-03-30 17:59:06.000000 ngcsimlib-0.2b2/pyproject.toml
--rw-rw-r--   0 ago       (1001) ago       (1001)       38 2024-03-30 17:59:16.104944 ngcsimlib-0.2b2/setup.cfg
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:22:28.248336 ngcsimlib-0.3b0/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      286 2024-05-14 18:04:23.000000 ngcsimlib-0.3b0/AUTHORS
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1548 2024-05-14 18:04:23.000000 ngcsimlib-0.3b0/LICENSE
+-rw-r--r--   0 ago       (1001) ago       (1001)     3139 2024-05-31 17:22:28.248336 ngcsimlib-0.3b0/PKG-INFO
+-rw-rw-r--   0 ago       (1001) ago       (1001)     2642 2024-05-31 14:13:35.000000 ngcsimlib-0.3b0/README.md
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:22:28.244336 ngcsimlib-0.3b0/ngcsimlib/
+-rw-rw-r--   0 ago       (1001) ago       (1001)     2573 2024-05-31 14:13:35.000000 ngcsimlib-0.3b0/ngcsimlib/__init__.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1144 2024-05-18 21:55:37.000000 ngcsimlib-0.3b0/ngcsimlib/_compartment.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)    11179 2024-05-26 23:07:39.000000 ngcsimlib-0.3b0/ngcsimlib/_context.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1014 2024-05-18 22:20:29.000000 ngcsimlib-0.3b0/ngcsimlib/_metaComponent.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1821 2024-05-18 22:04:30.000000 ngcsimlib-0.3b0/ngcsimlib/_operations.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:22:28.248336 ngcsimlib-0.3b0/ngcsimlib/commands/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      313 2024-05-14 18:04:23.000000 ngcsimlib-0.3b0/ngcsimlib/commands/__init__.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1027 2024-05-14 18:04:23.000000 ngcsimlib-0.3b0/ngcsimlib/commands/advanceState.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     2413 2024-05-31 14:13:35.000000 ngcsimlib-0.3b0/ngcsimlib/commands/clamp.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1885 2024-05-31 14:13:35.000000 ngcsimlib-0.3b0/ngcsimlib/commands/command.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1640 2024-05-14 18:04:23.000000 ngcsimlib-0.3b0/ngcsimlib/commands/compound.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1538 2024-05-14 18:04:23.000000 ngcsimlib-0.3b0/ngcsimlib/commands/evolve.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1781 2024-05-14 18:04:23.000000 ngcsimlib-0.3b0/ngcsimlib/commands/multiclamp.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1593 2024-05-14 18:04:23.000000 ngcsimlib-0.3b0/ngcsimlib/commands/reset.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     2099 2024-05-14 18:04:23.000000 ngcsimlib-0.3b0/ngcsimlib/commands/save.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1650 2024-05-14 18:04:23.000000 ngcsimlib-0.3b0/ngcsimlib/commands/seed.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1605 2024-05-14 18:04:23.000000 ngcsimlib-0.3b0/ngcsimlib/commands/snapshot.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     2055 2024-05-14 18:04:23.000000 ngcsimlib-0.3b0/ngcsimlib/commands/track.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     3861 2024-05-31 14:13:35.000000 ngcsimlib-0.3b0/ngcsimlib/compartment.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:22:28.248336 ngcsimlib-0.3b0/ngcsimlib/compilers/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      185 2024-05-31 14:13:35.000000 ngcsimlib-0.3b0/ngcsimlib/compilers/__init__.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     2312 2024-05-22 15:50:02.000000 ngcsimlib-0.3b0/ngcsimlib/compilers/_command_compiler.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     2392 2024-05-28 14:54:39.000000 ngcsimlib-0.3b0/ngcsimlib/compilers/_component_compiler.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     6602 2024-05-31 14:13:35.000000 ngcsimlib-0.3b0/ngcsimlib/compilers/command_compiler.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     3261 2024-05-31 14:13:35.000000 ngcsimlib-0.3b0/ngcsimlib/compilers/component_compiler.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     2545 2024-05-31 14:13:35.000000 ngcsimlib-0.3b0/ngcsimlib/compilers/op_compiler.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     2731 2024-05-31 14:13:35.000000 ngcsimlib-0.3b0/ngcsimlib/component.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1941 2024-05-31 14:13:35.000000 ngcsimlib-0.3b0/ngcsimlib/configManager.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)    16502 2024-05-31 14:13:35.000000 ngcsimlib-0.3b0/ngcsimlib/context.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)    18516 2024-05-31 14:13:35.000000 ngcsimlib-0.3b0/ngcsimlib/controller.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     2524 2024-05-31 14:13:35.000000 ngcsimlib-0.3b0/ngcsimlib/logger.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     2309 2024-05-31 14:13:35.000000 ngcsimlib-0.3b0/ngcsimlib/metaComponent.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:22:28.248336 ngcsimlib-0.3b0/ngcsimlib/operations/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      140 2024-05-31 14:13:35.000000 ngcsimlib-0.3b0/ngcsimlib/operations/__init__.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)      440 2024-05-31 14:13:35.000000 ngcsimlib-0.3b0/ngcsimlib/operations/add.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     3245 2024-05-31 14:13:35.000000 ngcsimlib-0.3b0/ngcsimlib/operations/baseOp.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)      237 2024-05-31 14:13:35.000000 ngcsimlib-0.3b0/ngcsimlib/operations/negate.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)      286 2024-05-31 14:13:35.000000 ngcsimlib-0.3b0/ngcsimlib/operations/overwrite.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)      370 2024-05-31 14:13:35.000000 ngcsimlib-0.3b0/ngcsimlib/operations/summation.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     5299 2024-05-31 14:13:35.000000 ngcsimlib-0.3b0/ngcsimlib/resolver.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)    10510 2024-05-31 14:13:35.000000 ngcsimlib-0.3b0/ngcsimlib/utils.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:22:28.248336 ngcsimlib-0.3b0/ngcsimlib.egg-info/
+-rw-r--r--   0 ago       (1001) ago       (1001)     3139 2024-05-31 17:22:28.000000 ngcsimlib-0.3b0/ngcsimlib.egg-info/PKG-INFO
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1285 2024-05-31 17:22:28.000000 ngcsimlib-0.3b0/ngcsimlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 ago       (1001) ago       (1001)        1 2024-05-31 17:22:28.000000 ngcsimlib-0.3b0/ngcsimlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 ago       (1001) ago       (1001)       10 2024-05-31 17:22:28.000000 ngcsimlib-0.3b0/ngcsimlib.egg-info/top_level.txt
+-rw-rw-r--   0 ago       (1001) ago       (1001)      597 2024-05-31 17:20:50.000000 ngcsimlib-0.3b0/pyproject.toml
+-rw-rw-r--   0 ago       (1001) ago       (1001)       38 2024-05-31 17:22:28.248336 ngcsimlib-0.3b0/setup.cfg
```

### Comparing `ngcsimlib-0.2b2/LICENSE` & `ngcsimlib-0.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `ngcsimlib-0.2b2/PKG-INFO` & `ngcsimlib-0.3b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: ngcsimlib
-Version: 0.2b2
+Version: 0.3b0
 Summary: Simulation software backend for ngc-learn.
 Author-email: William Gebhardt <wdg1351@rit.edu>, Alexander Ororbia <ago@cs.rit.edu>
 License: BSD-3-Clause License
 Project-URL: Homepage, https://github.com/NACLab/ngc-sim-lib
 Project-URL: Lab Page, https://www.cs.rit.edu/~ago/nac_lab.html
 Keywords: python,complex-systems,simulation
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
 [![Python Version](https://img.shields.io/badge/python-3.10%20%7C%203.11-blue.svg)](https://www.python.org/downloads)[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 [![DOI](https://zenodo.org/badge/734040498.svg)](https://zenodo.org/doi/10.5281/zenodo.10888210)
 
 # NGC-Sim-Lib: Support Library for NGC-Learn
 
-<b>ngc-sim-lib</b> is the support library and central dependency for
+<b>ngc-sim-lib</b> is the support library backend and central dependency for
 <i><a href="https://github.com/NACLab/ngc-learn/">ngc-learn</a></i>, a library
 designed for computational neuroscience and cognitive neuroscience research.
 While ngc-learn contains the JAX-implemented routines and any supporting C
 code, ngc-sim-lib is a pure Python package, primarily meant for providing the
 machinery, routines, and utilities that facilitate the general (abstract)
 simulation of complex adaptive systems made up of dynamical components. For
 information, including anything related to usage instructions and details,
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: ngcsimlib Version: 0.2b2 Summary: Simulation
+Metadata-Version: 2.1 Name: ngcsimlib Version: 0.3b0 Summary: Simulation
 software backend for ngc-learn. Author-email: William Gebhardt
 rit.edu>, Alexander Ororbia
 cs.rit.edu> License: BSD-3-Clause License Project-URL: Homepage, https://
 github.com/NACLab/ngc-sim-lib Project-URL: Lab Page, https://www.cs.rit.edu/
 ~ago/nac_lab.html Keywords: python,complex-systems,simulation Requires-Python:
->=3.10 Description-Content-Type: text/markdown License-File: LICENSE License-
+>=3.8 Description-Content-Type: text/markdown License-File: LICENSE License-
 File: AUTHORS [![Python Version](https://img.shields.io/badge/python-
 3.10%20%7C%203.11-blue.svg)](https://www.python.org/downloads)[![License]
 (https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://
 opensource.org/licenses/BSD-3-Clause)[![Maintenance](https://img.shields.io/
 badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/
 graphs/commit-activity) [![DOI](https://zenodo.org/badge/734040498.svg)](https:
 //zenodo.org/doi/10.5281/zenodo.10888210) # NGC-Sim-Lib: Support Library for
-NGC-Learn nnggcc--ssiimm--lliibb is the support library and central dependency for _n_g_c_-
-_l_e_a_r_n, a library designed for computational neuroscience and cognitive
+NGC-Learn nnggcc--ssiimm--lliibb is the support library backend and central dependency for
+_n_g_c_-_l_e_a_r_n, a library designed for computational neuroscience and cognitive
 neuroscience research. While ngc-learn contains the JAX-implemented routines
 and any supporting C code, ngc-sim-lib is a pure Python package, primarily
 meant for providing the machinery, routines, and utilities that facilitate the
 general (abstract) simulation of complex adaptive systems made up of dynamical
 components. For information, including anything related to usage instructions
 and details, please refer to the ngc-learn README: https://github.com/NACLab/
 ngc-learn/. This package is distributed under the 3-Clause BSD license. It is
```

### Comparing `ngcsimlib-0.2b2/README.md` & `ngcsimlib-0.3b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![Python Version](https://img.shields.io/badge/python-3.10%20%7C%203.11-blue.svg)](https://www.python.org/downloads)[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 [![DOI](https://zenodo.org/badge/734040498.svg)](https://zenodo.org/doi/10.5281/zenodo.10888210)
 
 # NGC-Sim-Lib: Support Library for NGC-Learn
 
-<b>ngc-sim-lib</b> is the support library and central dependency for
+<b>ngc-sim-lib</b> is the support library backend and central dependency for
 <i><a href="https://github.com/NACLab/ngc-learn/">ngc-learn</a></i>, a library
 designed for computational neuroscience and cognitive neuroscience research.
 While ngc-learn contains the JAX-implemented routines and any supporting C
 code, ngc-sim-lib is a pure Python package, primarily meant for providing the
 machinery, routines, and utilities that facilitate the general (abstract)
 simulation of complex adaptive systems made up of dynamical components. For
 information, including anything related to usage instructions and details,
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
 [![Python Version](https://img.shields.io/badge/python-3.10%20%7C%203.11-
 blue.svg)](https://www.python.org/downloads)[![License](https://img.shields.io/
 badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-
 Clause)[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-
 green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) [!
 [DOI](https://zenodo.org/badge/734040498.svg)](https://zenodo.org/doi/10.5281/
 zenodo.10888210) # NGC-Sim-Lib: Support Library for NGC-Learn nnggcc--ssiimm--lliibb is
-the support library and central dependency for _n_g_c_-_l_e_a_r_n, a library designed
-for computational neuroscience and cognitive neuroscience research. While ngc-
-learn contains the JAX-implemented routines and any supporting C code, ngc-sim-
-lib is a pure Python package, primarily meant for providing the machinery,
-routines, and utilities that facilitate the general (abstract) simulation of
-complex adaptive systems made up of dynamical components. For information,
-including anything related to usage instructions and details, please refer to
-the ngc-learn README: https://github.com/NACLab/ngc-learn/. This package is
-distributed under the 3-Clause BSD license. It is currently maintained by the
-_N_e_u_r_a_l_ _A_d_a_p_t_i_v_e_ _C_o_m_p_u_t_i_n_g_ _(_N_A_C_)_ _l_a_b_o_r_a_t_o_r_y. ## IInnssttaallllaattiioonn:: Setup: Ensure that
-you have installed the following base dependencies in your system. Note that
-this library was developed and tested on Ubuntu 22.04.3 LTS. ngc-sim-lib
-requires: `Python (>=3.10)`. Once you have ensured that the appropriate Python
-is installed, you can then have the ngcsimlib package installed on your system
-using either the official pip install:
+the support library backend and central dependency for _n_g_c_-_l_e_a_r_n, a library
+designed for computational neuroscience and cognitive neuroscience research.
+While ngc-learn contains the JAX-implemented routines and any supporting C
+code, ngc-sim-lib is a pure Python package, primarily meant for providing the
+machinery, routines, and utilities that facilitate the general (abstract)
+simulation of complex adaptive systems made up of dynamical components. For
+information, including anything related to usage instructions and details,
+please refer to the ngc-learn README: https://github.com/NACLab/ngc-learn/.
+This package is distributed under the 3-Clause BSD license. It is currently
+maintained by the _N_e_u_r_a_l_ _A_d_a_p_t_i_v_e_ _C_o_m_p_u_t_i_n_g_ _(_N_A_C_)_ _l_a_b_o_r_a_t_o_r_y. ## IInnssttaallllaattiioonn::
+Setup: Ensure that you have installed the following base dependencies in your
+system. Note that this library was developed and tested on Ubuntu 22.04.3 LTS.
+ngc-sim-lib requires: `Python (>=3.10)`. Once you have ensured that the
+appropriate Python is installed, you can then have the ngcsimlib package
+installed on your system using either the official pip install:
 $ pip install ngcsimlib
 or, if you download this repo and use pip locally, you can run the following:
 $ pip install .
 Alternatively, if you are doing development, then do an editable install via:
 $ pip install --editable . # OR pip install -e .
 **Version:**
 0.2.0 Authors: William Gebhardt, Alexander G. Ororbia II
```

### Comparing `ngcsimlib-0.2b2/ngcsimlib/commands/advanceState.py` & `ngcsimlib-0.3b0/ngcsimlib/commands/advanceState.py`

 * *Files identical despite different names*

### Comparing `ngcsimlib-0.2b2/ngcsimlib/commands/clamp.py` & `ngcsimlib-0.3b0/ngcsimlib/commands/clamp.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from ngcsimlib.commands.command import Command
 from ngcsimlib.utils import extract_args
-
+from ngcsimlib.logger import error
+from ngcsimlib.compartment import Compartment
 
 class Clamp(Command):
     """
     All components in ngclearn have compartments where they store information
     pertaining to their internal state that can be read into or out of by
     commands. The Clamp command is the primary way to manually set the value of
     a compartment on a set of components. The Clamp command requires a
@@ -26,33 +27,34 @@
 
             command_name: the name of the command on the controller
 
         """
         super().__init__(components=components, command_name=command_name,
                          required_calls=['clamp'])
         if compartment is None:
-            raise RuntimeError(
-                self.name + " requires a \'compartment\' to clamp to for construction")
+            error(self.name, "requires a \'compartment\' to clamp to for construction")
         if clamp_name is None:
-            raise RuntimeError(
-                self.name + " requires a \'clamp_name\' to bind to for construction")
+            error(self.name, "requires a \'clamp_name\' to bind to for construction")
 
         self.clamp_name = clamp_name
         self.compartment = compartment
 
-        for component in self.components:
-            if self.compartment not in self.components[component].compartments.keys():
-                raise RuntimeError(self.name + " is attempting to "
-                                               "initialize clamp to "
-                                               "non-existent compartment.")
+        for name, component in self.components.items():
+            mapped = hasattr(component, self.compartment)
+            if mapped:
+                if Compartment.is_compartment(getattr(compartment, self.compartment)):
+                    continue
+
+            error(self.name, " is attempting to initialize clamp to non-existent compartment \"",
+                  self.compartment, "\" on ", name, sep=" ")
+
 
     def __call__(self, *args, **kwargs):
         try:
             vals = extract_args([self.clamp_name], *args, **kwargs)
         except RuntimeError:
-            raise RuntimeError(self.name + ", " + str(
-                self.clamp_name) + " is missing from keyword arguments or a positional "
-                                   "arguments can be provided")
+            error(self.name, ",", self.clamp_name,
+                  "is missing from keyword arguments or a positional arguments can be provided")
 
         for component in self.components:
             self.components[component].clamp(self.compartment, vals[self.clamp_name])
```

### Comparing `ngcsimlib-0.2b2/ngcsimlib/commands/compound.py` & `ngcsimlib-0.3b0/ngcsimlib/commands/compound.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ngcsimlib.commands import Command
 from ngcsimlib.utils import check_attributes
-import warnings
+from ngcsimlib.logger import warn, error
 
 class Compound(Command):
     """
     There is sometimes a need by controllers to be able to call a set of commands
     in series without writing custom command(s) for each combination. The
     compound node/command is used to fill this need. A compound command set is
     very similar to the cycle found inside/within a controller / simulation object.
@@ -21,17 +21,17 @@
 
             command_list: a list of all commands to be called
 
             controller: the controller that will be calling these commands
         """
         super().__init__(components=components, command_name=command_name)
         if controller is None:
-            raise RuntimeError("The controller is needed to build a compound command (This should be passed in by default)")
+            error("The controller is needed to build a compound command (This should be passed in by default)")
         if command_list is None or len(command_list) == 0:
-            warnings.warn("The command list for command " + self.name + " is None or empty")
+            warn("The command list for command", self.name, "is None or empty")
 
         self.command_list = command_list
         self.controller = controller
 
         check_attributes(self.controller, self.command_list, fatal=True)
 
     def __call__(self, *args, **kwargs):
```

### Comparing `ngcsimlib-0.2b2/ngcsimlib/commands/evolve.py` & `ngcsimlib-0.3b0/ngcsimlib/commands/evolve.py`

 * *Files identical despite different names*

### Comparing `ngcsimlib-0.2b2/ngcsimlib/commands/multiclamp.py` & `ngcsimlib-0.3b0/ngcsimlib/commands/multiclamp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ngcsimlib.commands.command import Command
 from ngcsimlib.utils import extract_args, check_attributes
-
+from ngcsimlib.logger import error
 
 class Multiclamp(Command):
     """
     There are times when a model will have many clamp calls as there might be a
     need to clamp many different values to a model at the same time. As a
     solution to this, ngcsimlib provides the `multiclamp` command. This command is
     used to set a wide range of values to all compartments with the same name
@@ -21,22 +21,22 @@
             clamp_name: a keyword to bind the input for this command do
 
             command_name: the name of the command on the controller
         """
         super().__init__(components=components, command_name=command_name,
                          required_calls=['clamp'])
         if clamp_name is None:
-            raise RuntimeError(self.name + " requires a \'clamp_name\' to bind to for construction")
+            error(self.name, "requires a \'clamp_name\' to bind to for construction")
 
         self.clamp_name = clamp_name
 
     def __call__(self, *args, **kwargs):
         try:
             vals = extract_args([self.clamp_name], *args, **kwargs)
         except RuntimeError:
-            raise RuntimeError(self.name + ", " + str(self.clamp_name) + " is missing from keyword arguments or a "
-                                                                       "positional arguments can be provided")
+            error(self.name, ",", self.clamp_name,
+                  "is missing from keyword arguments or a positional arguments can be provided")
 
         for compartment, value in vals[self.clamp_name].items():
             for component in self.components:
                 if check_attributes(component, compartment, fatal=False):
                     self.components[component].clamp(compartment, value)
```

### Comparing `ngcsimlib-0.2b2/ngcsimlib/commands/reset.py` & `ngcsimlib-0.3b0/ngcsimlib/commands/reset.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from ngcsimlib.commands import Command
 from ngcsimlib.utils import extract_args
-import warnings
-
+from ngcsimlib.logger import warn, error
 class Reset(Command):
     """
     In every model/system, there is a need to reset components back to some
     intial state value(s). As such, many components that maintain a state have a
     reset method implemented within them. The reset command will go through
     the list of components and trigger the reset within each of them.
     """
@@ -20,21 +19,21 @@
             reset_name: the keyword for the flag on if the reset should happen
 
             command_name: the name of the command on the controller
         """
         super().__init__(components=components, command_name=command_name,
                          required_calls=['reset'])
         if reset_name is None:
-            raise RuntimeError(self.name + " requires a \'reset_name\' to bind to for construction")
+            error(self.name, "requires a \'reset_name\' to bind to for construction")
         self.reset_name = reset_name
 
     def __call__(self, *args, **kwargs):
         try:
             vals = extract_args([self.reset_name], *args, **kwargs)
         except RuntimeError:
-            warnings.warn(self.name + ", " + str(self.reset_name) + " is missing from keyword arguments and no "
-                                                             "positional arguments were provided", stacklevel=6)
+            warn(self.name, ",", self.reset_name,
+                 "is missing from keyword arguments and no positional arguments were provided")
             return
 
         if vals[self.reset_name]:
             for component in self.components:
                 self.components[component].reset()
```

### Comparing `ngcsimlib-0.2b2/ngcsimlib/commands/save.py` & `ngcsimlib-0.3b0/ngcsimlib/commands/save.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from ngcsimlib.commands import Command
 from ngcsimlib.utils import extract_args
-import warnings
+from ngcsimlib.logger import warn, error
+
 
 class Save(Command):
     """
     When training models, there is often a need to snapshot the model and save
     it to disk. The base controller in ngcsimlib is able to save all of the
     commands, components, connections, and steps to a file in order to rebuild
     the model at a later time. However, there is a good chance that the model
@@ -26,21 +27,22 @@
             directory_flag: keyword for flag for the directory to save to
 
             command_name: the name of the command on the controller
         """
         super().__init__(components=components, command_name=command_name,
                          required_calls=['save'])
         if directory_flag is None:
-            raise RuntimeError(self.name + " requires a \'directory_flag\' to bind to for construction")
+            error(self.name, "requires a \'directory_flag\' to bind to for construction")
+
         self.directory_flag = directory_flag
 
     def __call__(self, *args, **kwargs):
         try:
             vals = extract_args([self.directory_flag], *args, **kwargs)
         except RuntimeError:
-            warnings.warn(self.name + ", " + str(self.directory_flag) + " is missing from keyword arguments and no "
-                                                                "positional arguments were provided", stacklevel=6)
+            warn(self.name + ",", self.directory_flag,
+                 "is missing from keyword arguments and no positional arguments were provided")
             return
 
         if vals[self.directory_flag]:
             for component in self.components:
                 self.components[component].save(vals[self.directory_flag])
```

### Comparing `ngcsimlib-0.2b2/ngcsimlib/commands/snapshot.py` & `ngcsimlib-0.3b0/ngcsimlib/commands/snapshot.py`

 * *Files identical despite different names*

### Comparing `ngcsimlib-0.2b2/ngcsimlib/commands/track.py` & `ngcsimlib-0.3b0/ngcsimlib/commands/track.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ngcsimlib.commands import Command
 from ngcsimlib.utils import extract_args
-import warnings
+from ngcsimlib.logger import warn, error
 
 class Track(Command):
     """
     When running a model or complex system, there is often a need to track a
     compartment value over time, usually for visualization. To do this, ngcsimlib
     provides a track utility command. This command stores the values of a
     compartment from a set of components into a provided object. This provided
@@ -24,27 +24,27 @@
 
             tracker: the keyword for which the tracking object will be passed in by
 
             command_name: the name of the command on the controller
         """
         super().__init__(components=components, command_name=command_name)
         if compartment is None:
-            raise RuntimeError(self.name + " requires a \'compartment\' to clamp to for construction")
+            error(self.name, "requires a \'compartment\' to clamp to for construction")
         if tracker is None:
-            raise RuntimeError(self.name + " requires a \'tracker\' to bind to for construction")
+            error(self.name,"requires a \'tracker\' to bind to for construction")
 
         self.tracker = tracker
         self.compartment = compartment
 
 
     def __call__(self, *args, **kwargs):
         try:
             vals = extract_args([self.tracker], *args, **kwargs)
         except RuntimeError:
-            warnings.warn(self.name + ", " + str(self.tracker) + " is missing from keyword arguments and no "
-                                                                "positional arguments were provided", stacklevel=6)
+            warn(self.name, ",", self.tracker,
+                 "is missing from keyword arguments and no positional arguments were provided")
             return
 
         v = []
         for component in self.components:
             v.append(self.components[component].compartments[self.compartment])
         vals[self.tracker].append(v)
```

### Comparing `ngcsimlib-0.2b2/ngcsimlib/controller.py` & `ngcsimlib-0.3b0/ngcsimlib/controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from ngcsimlib.utils import check_attributes, load_from_path, make_unique_path, check_serializable
-import json, os, warnings, inspect
+from ngcsimlib.logger import warn, error, info
+import json, os, inspect
 
 
 class Controller:
     """
     The ngc controller is the foundation of all ngclearn models and the central
     operational construct for simulating complex systems. The controller is the
     object that organizes all of the components, commands, and connections
     that characterize a complex system and/or model to be simulated over time
     (and was referred to as the "nodes-and-cables" system in earlier versions of
     ngc-learn).
     """
+
     def __init__(self):
+        warn("Controllers have been deprecated in favor of contexts and will be removed in the future")
         self.steps = []
         self.commands = {}
-        self.components = {} ## components/nodes that characterize system/simulation object
+        self.components = {}  ## components/nodes that characterize system/simulation object
         self.connections = []  ## cables that characterize system/simulation object
 
         self._json_objects = {
             "commands": [],
             "steps": [],
             "components": [],
             "connections": []
@@ -52,42 +55,44 @@
         """
         for component in self.components.keys():
             if skip_components is not None and component.name in skip_components:
                 continue
             else:
                 self.components[component].verify_connections()
 
-    def connect(self, source_component_name, source_compartment_name, destination_component_name,
+    def connect(self, source_component_name, source_compartment_name, target_component_name,
                 target_compartment_name, bundle=None):
         """
         Creates a cable from one component to another.
 
         Args:
             source_component_name: the name of the component providing the value
 
             source_compartment_name: the name of the compartment containing the
                 source value
 
-            destination_component_name: the name of the component receiving
+            target_component_name: the name of the component receiving
                 the value
 
             target_compartment_name: the name of the compartment to store the
                 source value in
 
             bundle: the number of the bundle rule to be used when using this
                 cable (Default: None)
         """
-        self.components[destination_component_name].create_incoming_connection(
-            self.components[source_component_name].create_outgoing_connection(source_compartment_name), target_compartment_name,
+        self.components[target_component_name].create_incoming_connection(
+            self.components[source_component_name].create_outgoing_connection(source_compartment_name),
+            target_compartment_name,
             bundle)
-        self.connections.append((source_component_name, source_compartment_name, destination_component_name, target_compartment_name, bundle))
+        self.connections.append((source_component_name, source_compartment_name, target_component_name,
+                                 target_compartment_name, bundle))
         self._json_objects['connections'].append({
             "source_component_name": source_component_name,
             "source_compartment_name": source_compartment_name,
-            "target_component_name": destination_component_name,
+            "target_component_name": target_component_name,
             "target_compartment_name": target_compartment_name,
             "bundle": bundle})
 
     def make_connections(self, path_to_cables_file):
         """
         Loads a collection of cables from a json file. Follow `cables.schema`
         for the specific format of the required json file.
@@ -111,17 +116,29 @@
                 and extension
 
             custom_file_dir: the path to the custom directory for custom load methods,
                 this directory is named `custom` if the save_to_json method is
                 used. (Default: None)
         """
         with open(path_to_components_file, 'r') as file:
-            components = json.load(file)
+            componentsConfig = json.load(file)
+
+            parameterMap = {}
+            components = componentsConfig["components"]
+            if "hyperparameters" in componentsConfig.keys():
+                for component in components:
+                    for pKey, pValue in componentsConfig["hyperparameters"].items():
+                        for cKey, cValue in component.items():
+                            if pKey == cValue:
+                                component[cKey] = pValue
+                                parameterMap[cKey] = pKey
+
             for component in components:
-                self.add_component(**component, directory=custom_file_dir)
+                self.add_component(**component, directory=custom_file_dir,
+                                   parameterMap=parameterMap)
 
     def make_steps(self, path_to_steps_file):
         """
         Loads a collection of steps from a json file. Follow `steps.schema` for
         the specific format of this json file.
 
         Args:
@@ -190,36 +207,35 @@
         Component_class = load_from_path(path=component_type, match_case=match_case, absolute_path=absolute_path)
 
         if inspect.isclass(Component_class):
             call = Component_class.__init__
         elif inspect.isfunction(Component_class):
             call = Component_class
         else:
-            raise RuntimeError("Given component type " + str(component_type)
-                               + " is not callable")
+            error("Given component type", component_type, "is not callable")
 
-
-
-        count = call.__code__.co_argcount - 1
-        named_args = call.__code__.co_varnames[1:count]
         try:
             component = Component_class(**kwargs)
         except TypeError as E:
-            print(E)
-            raise RuntimeError(str(E) + "\nProvided keyword arguments:\t" + str(list(kwargs.keys())) +
-                               "\nRequired keyword arguments:\t" + str(list(named_args)))
+            count = call.__code__.co_argcount - 1
+            named_args = call.__code__.co_varnames[1:count]
+            error(E, "\nProvided keyword arguments:\t", list(kwargs.keys()),
+                  "\nRequired keyword arguments:\t", list(named_args))
 
         check_attributes(component, ["name", "verify_connections"], fatal=True)
         self.components[component.name] = component
 
         obj = {"component_type": component_type, "match_case": match_case, "absolute_path": absolute_path} | kwargs
         bad_keys = check_serializable(obj)
         for key in bad_keys:
             del obj[key]
-            print("Failed to serialize \"" + str(key) + "\" in " + component.name)
+            info("Failed to serialize \"", key, "\" in ", component.name, sep="")
+
+        if "directory" in obj.keys():
+            del obj["directory"]
 
         self._json_objects['components'].append(obj)
 
         return component
 
     def add_command(self, command_type, command_name, match_case=False, absolute_path=False, component_names=None,
                     **kwargs):
@@ -260,48 +276,46 @@
                 keyword arguments.
 
         Returns:
             the created command (Command is also automatically added to the controller)
         """
         Command_class = load_from_path(path=command_type, match_case=match_case, absolute_path=absolute_path)
         if not callable(Command_class):
-            raise RuntimeError("The object named \"" + Command_class.__name__ + "\" is not callable. Please make sure "
-                                                                                "the object is callable and returns a "
-                                                                                "callable object")
+            error("The object named \"", Command_class.__name__,
+                  "\" is not callable. Please make sure the object is callable and returns a callable object", sep="")
+
         if component_names is not None:
             componentObjs = [self.components[name] for name in component_names]
         else:
             componentObjs = []
 
         if inspect.isclass(Command_class):
             call = Command_class.__init__
         elif inspect.isfunction(Command_class):
             call = Command_class
         else:
-            raise RuntimeError("Given command type " + str(command_type)
-                               + " is not callable")
+            error("Given command type", command_type, "is not callable")
 
         count = call.__code__.co_argcount - 1
         named_args = call.__code__.co_varnames[1:count]
         try:
             command = Command_class(components=componentObjs, controller=self, command_name=command_name, **kwargs)
         except TypeError as E:
-            print(E)
-            raise RuntimeError(str(E) + "\nProvided keyword arguments:\t" + str(list(kwargs.keys())) +
-                               "\nRequired keyword arguments:\t" + str(list(named_args)))
+            error(E, "\nProvided keyword arguments:\t", list(kwargs.keys()),
+                  "\nRequired keyword arguments:\t", list(named_args))
 
         self.commands[command_name] = command
         self.__setattr__(command_name, command)
 
         obj = {"command_type": command_type, "command_name": command_name, "match_case": match_case,
                "absolute_path": absolute_path, "component_names": component_names} | kwargs
         bad_keys = check_serializable(obj)
         for key in bad_keys:
             del obj[key]
-            print("Failed to serialize \"" + str(key) + "\" in " + command_name)
+            info("Failed to serialize \"", key, "\" in ", command_name, sep="")
 
         self._json_objects['commands'].append(obj)
         return command
 
     def runCommand(self, command_name, *args, **kwargs):
         """
         Runs the given command.
@@ -311,15 +325,15 @@
 
             args: positional arguments to be passed into the command
 
             kwargs: keyword arguments to be passed into the command
         """
         command = self.commands.get(command_name, None)
         if command is None:
-            raise RuntimeError("Can not find command: " + str(command_name))
+            error("Can not find command:", command_name)
         command(*args, **kwargs)
 
     def save_to_json(self, directory, model_name=None, custom_save=True):
         """
         Dumps all the required json files to rebuild the current controller to a specified directory. If there is a
         `save` command present on the controller and custom_save is True, it will run that command as well.
 
@@ -343,25 +357,63 @@
         with open(path + "/commands.json", 'w') as fp:
             json.dump(self._json_objects['commands'], fp, indent=4)
 
         with open(path + "/steps.json", 'w') as fp:
             json.dump(self._json_objects['steps'], fp, indent=4)
 
         with open(path + "/components.json", 'w') as fp:
-            json.dump(self._json_objects['components'], fp, indent=4)
+            hyperparameters = {}
+
+            for idx, component in enumerate(self._json_objects['components']):
+                if component.get('parameterMap', None) is not None:
+                    for cKey, pKey in component['parameterMap'].items():
+                        pVal = component[cKey]
+                        if pKey not in hyperparameters.keys():
+                            hyperparameters[pKey] = []
+                        hyperparameters[pKey].append((idx, cKey, pVal))
+
+            hp = {}
+            for param in hyperparameters.keys():
+                matched = True
+                hp[param] = None
+                for _, _, pVal in hyperparameters[param]:
+                    if hp[param] is None:
+                        hp[param] = pVal
+                    elif hp[param] != pVal:
+                        del hp[param]
+                        matched = False
+                        break
+
+                for idx, cKey, _ in hyperparameters[param]:
+                    if matched:
+                        self._json_objects['components'][idx][cKey] = param
+
+                    else:
+                        warn("Unable to extract hyperparameter", param,
+                             "as it is mismatched between components. Parameter will not be extracted")
+
+            for component in self._json_objects['components']:
+                if "parameterMap" in component.keys():
+                    del component["parameterMap"]
+
+            obj = {"components": self._json_objects['components']}
+            if len(hp.keys()) != 0:
+                obj["hyperparameters"] = hp
+
+            json.dump(obj, fp, indent=4)
 
         with open(path + "/connections.json", 'w') as fp:
             json.dump(self._json_objects['connections'], fp, indent=4)
 
         if custom_save:
             os.mkdir(path + "/custom")
             if check_attributes(self, ['save']):
                 self.save(path + "/custom")
             else:
-                warnings.warn("Controller doesn't have a save command registered. No custom saving happened")
+                warn("Controller doesn't have a save command registered. No custom saving happened")
 
         return (path, path + "/custom") if custom_save else (path, None)
 
     def load_from_dir(self, directory, custom_folder="/custom"):
         """
         Builds a controller from a directory. Designed to be used with
         `save_to_json`.
```

### Comparing `ngcsimlib-0.2b2/ngcsimlib.egg-info/PKG-INFO` & `ngcsimlib-0.3b0/ngcsimlib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: ngcsimlib
-Version: 0.2b2
+Version: 0.3b0
 Summary: Simulation software backend for ngc-learn.
 Author-email: William Gebhardt <wdg1351@rit.edu>, Alexander Ororbia <ago@cs.rit.edu>
 License: BSD-3-Clause License
 Project-URL: Homepage, https://github.com/NACLab/ngc-sim-lib
 Project-URL: Lab Page, https://www.cs.rit.edu/~ago/nac_lab.html
 Keywords: python,complex-systems,simulation
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
 [![Python Version](https://img.shields.io/badge/python-3.10%20%7C%203.11-blue.svg)](https://www.python.org/downloads)[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 [![DOI](https://zenodo.org/badge/734040498.svg)](https://zenodo.org/doi/10.5281/zenodo.10888210)
 
 # NGC-Sim-Lib: Support Library for NGC-Learn
 
-<b>ngc-sim-lib</b> is the support library and central dependency for
+<b>ngc-sim-lib</b> is the support library backend and central dependency for
 <i><a href="https://github.com/NACLab/ngc-learn/">ngc-learn</a></i>, a library
 designed for computational neuroscience and cognitive neuroscience research.
 While ngc-learn contains the JAX-implemented routines and any supporting C
 code, ngc-sim-lib is a pure Python package, primarily meant for providing the
 machinery, routines, and utilities that facilitate the general (abstract)
 simulation of complex adaptive systems made up of dynamical components. For
 information, including anything related to usage instructions and details,
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: ngcsimlib Version: 0.2b2 Summary: Simulation
+Metadata-Version: 2.1 Name: ngcsimlib Version: 0.3b0 Summary: Simulation
 software backend for ngc-learn. Author-email: William Gebhardt
 rit.edu>, Alexander Ororbia
 cs.rit.edu> License: BSD-3-Clause License Project-URL: Homepage, https://
 github.com/NACLab/ngc-sim-lib Project-URL: Lab Page, https://www.cs.rit.edu/
 ~ago/nac_lab.html Keywords: python,complex-systems,simulation Requires-Python:
->=3.10 Description-Content-Type: text/markdown License-File: LICENSE License-
+>=3.8 Description-Content-Type: text/markdown License-File: LICENSE License-
 File: AUTHORS [![Python Version](https://img.shields.io/badge/python-
 3.10%20%7C%203.11-blue.svg)](https://www.python.org/downloads)[![License]
 (https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://
 opensource.org/licenses/BSD-3-Clause)[![Maintenance](https://img.shields.io/
 badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/
 graphs/commit-activity) [![DOI](https://zenodo.org/badge/734040498.svg)](https:
 //zenodo.org/doi/10.5281/zenodo.10888210) # NGC-Sim-Lib: Support Library for
-NGC-Learn nnggcc--ssiimm--lliibb is the support library and central dependency for _n_g_c_-
-_l_e_a_r_n, a library designed for computational neuroscience and cognitive
+NGC-Learn nnggcc--ssiimm--lliibb is the support library backend and central dependency for
+_n_g_c_-_l_e_a_r_n, a library designed for computational neuroscience and cognitive
 neuroscience research. While ngc-learn contains the JAX-implemented routines
 and any supporting C code, ngc-sim-lib is a pure Python package, primarily
 meant for providing the machinery, routines, and utilities that facilitate the
 general (abstract) simulation of complex adaptive systems made up of dynamical
 components. For information, including anything related to usage instructions
 and details, please refer to the ngc-learn README: https://github.com/NACLab/
 ngc-learn/. This package is distributed under the 3-Clause BSD license. It is
```

### Comparing `ngcsimlib-0.2b2/pyproject.toml` & `ngcsimlib-0.3b0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ngcsimlib"
-version = "0.2.beta2"
+version = "0.3.beta0"
 
 description = "Simulation software backend for ngc-learn."
 authors = [
   {name = "William Gebhardt", email = "wdg1351@rit.edu"},
   {name = "Alexander Ororbia", email = "ago@cs.rit.edu"},
 ]
 readme = "README.md"
 keywords = ['python', 'complex-systems', 'simulation']
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 license = {text = "BSD-3-Clause License"}
 
 [project.urls]
 Homepage = "https://github.com/NACLab/ngc-sim-lib"
 "Lab Page" = "https://www.cs.rit.edu/~ago/nac_lab.html"
```

