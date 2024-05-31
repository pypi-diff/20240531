# Comparing `tmp/cgt-0.4.0.tar.gz` & `tmp/cgt-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgt-0.4.0.tar", last modified: Wed May 29 03:10:07 2024, max compression
+gzip compressed data, was "cgt-0.4.1.tar", last modified: Fri May 31 15:19:45 2024, max compression
```

## Comparing `cgt-0.4.0.tar` & `cgt-0.4.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:10:07.981596 cgt-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-29 03:10:02.000000 cgt-0.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-29 03:10:02.000000 cgt-0.4.0/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-29 03:10:02.000000 cgt-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-29 03:10:02.000000 cgt-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-29 03:10:07.981596 cgt-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-29 03:10:02.000000 cgt-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-29 03:10:02.000000 cgt-0.4.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:10:07.981596 cgt-0.4.0/cgt/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    23526 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/distances.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/genome.py
--rw-r--r--   0 runner    (1001) docker     (127)    11595 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/hyperoctahedral.py
--rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/pickle_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    24864 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/position_paradigm.py
--rw-r--r--   0 runner    (1001) docker     (127)    15821 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/rearrangements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/simulations.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:10:07.981596 cgt-0.4.0/cgt/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/tests/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/tests/test_hyperoctahedral.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/tests/test_min_distances.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/visualisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:10:07.981596 cgt-0.4.0/cgt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-29 03:10:07.000000 cgt-0.4.0/cgt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-29 03:10:07.000000 cgt-0.4.0/cgt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 03:10:07.000000 cgt-0.4.0/cgt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-29 03:10:07.000000 cgt-0.4.0/cgt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 03:10:07.981596 cgt-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-29 03:10:02.000000 cgt-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:45.397937 cgt-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-31 15:19:38.000000 cgt-0.4.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-31 15:19:38.000000 cgt-0.4.1/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-31 15:19:38.000000 cgt-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-31 15:19:38.000000 cgt-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-31 15:19:45.397937 cgt-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-31 15:19:38.000000 cgt-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-31 15:19:38.000000 cgt-0.4.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:45.393937 cgt-0.4.1/cgt/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-31 15:19:38.000000 cgt-0.4.1/cgt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-31 15:19:38.000000 cgt-0.4.1/cgt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25349 2024-05-31 15:19:38.000000 cgt-0.4.1/cgt/distances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-31 15:19:38.000000 cgt-0.4.1/cgt/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-31 15:19:38.000000 cgt-0.4.1/cgt/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-31 15:19:38.000000 cgt-0.4.1/cgt/genome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11595 2024-05-31 15:19:38.000000 cgt-0.4.1/cgt/hyperoctahedral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-05-31 15:19:38.000000 cgt-0.4.1/cgt/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-31 15:19:38.000000 cgt-0.4.1/cgt/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-31 15:19:38.000000 cgt-0.4.1/cgt/pickle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-31 15:19:38.000000 cgt-0.4.1/cgt/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25036 2024-05-31 15:19:38.000000 cgt-0.4.1/cgt/position_paradigm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15821 2024-05-31 15:19:38.000000 cgt-0.4.1/cgt/rearrangements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-31 15:19:38.000000 cgt-0.4.1/cgt/simulations.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 15:19:38.000000 cgt-0.4.1/cgt/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-31 15:19:38.000000 cgt-0.4.1/cgt/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:45.397937 cgt-0.4.1/cgt/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:38.000000 cgt-0.4.1/cgt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-31 15:19:38.000000 cgt-0.4.1/cgt/tests/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-31 15:19:38.000000 cgt-0.4.1/cgt/tests/test_hyperoctahedral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-31 15:19:38.000000 cgt-0.4.1/cgt/tests/test_min_distances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-31 15:19:38.000000 cgt-0.4.1/cgt/visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:45.397937 cgt-0.4.1/cgt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-31 15:19:45.000000 cgt-0.4.1/cgt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-31 15:19:45.000000 cgt-0.4.1/cgt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:19:45.000000 cgt-0.4.1/cgt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-31 15:19:45.000000 cgt-0.4.1/cgt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:19:45.397937 cgt-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-31 15:19:38.000000 cgt-0.4.1/setup.py
```

### Comparing `cgt-0.4.0/CONTRIBUTING.md` & `cgt-0.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cgt-0.4.0/INSTALL.md` & `cgt-0.4.1/INSTALL.md`

 * *Files identical despite different names*

### Comparing `cgt-0.4.0/LICENSE` & `cgt-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cgt-0.4.0/PKG-INFO` & `cgt-0.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgt
-Version: 0.4.0
+Version: 0.4.1
 Summary: Tools for representing genomes in sage
 Home-page: https://github.com/js51/Circular-genome-tools
 Author: Joshua Stevenson
 Author-email: joshua.stevenson@utas.edu.au
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cgt-0.4.0/README.md` & `cgt-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `cgt-0.4.0/cgt/__init__.py` & `cgt-0.4.1/cgt/__init__.py`

 * *Files identical despite different names*

### Comparing `cgt-0.4.0/cgt/distances.py` & `cgt-0.4.1/cgt/distances.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     - MFPT: the mean first passage time from the identity to a given genome, where the target is an absorbing state
     - MLE: the maximum likelihood estimate of the time elapsed between the identity and a given genome
 
 Individual likelihood functions for the time elapsed between the identity and a given genome can also be obtained
 """
 
 from cgt.enums import ALGEBRA, DISTANCE, DATA, SYMMETRY
-from cgt.constants import VALUES_OF_N_WITH_SAVED_IRREPS_OF_Z
+from cgt.constants import VALUES_OF_N_WITH_SAVED_IRREPS_OF_Z, ERROR_CORRECTION_ENABLED
 import numpy as np
 import networkx as nx
 from sage.all import matrix, real, exp, round
 import scipy
 from scipy.optimize import minimize_scalar
 from cgt import pickle_manager
 from warnings import warn
@@ -53,27 +53,27 @@
     return distance_func(framework, model, [genome_instance])
 
 
 def distance_between(framework, model, genome_instance_1, genome_instance_2, distance_measure):
     return distance(framework, model, genome_instance_1.inverse() * genome_instance_2, distance_measure)
 
 
-def mle(framework, model, genome_instance, show_work=False):
+def mle(framework, model, genome_instance, show_work=False, use_eigenvectors=True):
     """
     Returns the maximum likelihood estimate for a given genome instance under the given model and framework.
 
     Args:
         framework (PositionParadigmFramework): the framework
         model (Model): the model
         genome_instance (group element): the genome instance to compute the MLE for
 
     Returns:
         float: the maximum likelihood estimate
     """
-    L = likelihood_function(framework, model, genome_instance)
+    L = likelihood_function(framework, model, genome_instance, use_eigenvectors=use_eigenvectors)
     max_t = maximise(framework, L)
     if show_work:
         return max_t, L
     else:
         return max_t
 
 
@@ -276,15 +276,15 @@
         )
     dims = [irrep_of_zs.nrows() for irrep_of_zs in irreps_of_zs]
 
     def prob_in_steps(k):
         alpha = 0
         for ptrace, dim, eig_list in zip(traces.values(), dims, eig_lists):
             term = 0
-            for e, eig in enumerate(eig_list):
+            for e, eig in enumerate(ptrace.keys()):
                 term += (eig**k) * ptrace[eig]
             alpha += dim * term
         return (Z.order() / G.order()) * alpha
 
     return prob_in_steps
 
 
@@ -360,32 +360,34 @@
         for e, eigenvalue in enumerate(eig_lists[r]):
             if zero_irrep:  # matrix of zeros
                 traces[r][eigenvalue] = 0
             else:
                 traces[r][eigenvalue] = real((sigd.numpy() @ projections[r][e]).trace())
     return traces
 
-
 def _partial_traces_for_genome_using_eigenvectors(
     framework, model, instance, irreps, irreps_of_zs, irreps_of_z
 ):
     """Return dictionary of partial traces, indexed first by irrep index and then by eigenvalaue"""
     instance_inverse = instance.inverse()
     eigen_data = _eigen_data(framework, model, irreps_of_zs)
     if DATA.partial_traces in model.data_bundle and instance_inverse in model.data_bundle[DATA.partial_traces]:
         return eigen_data[DATA.eigval_sets], model.data_bundle[DATA.partial_traces][instance_inverse]
     traces = {}
     irreps_of_z_np = model.data_bundle[DATA.irreps_z_np]
     for r, irrep in enumerate(irreps):  # Iterate over irreducible representations
         # Faster convert to numpy
         traces[r] = {}
         irrep_instance = irrep(instance_inverse)
-        irrep_instance_np = np.zeros(irrep_instance.dimensions())
-        for (i, j), val in irrep_instance.items():
-            irrep_instance_np[i,j] = val
+        try:
+            irrep_instance_np = np.zeros(irrep_instance.dimensions())
+            for (i, j), val in irrep_instance.items():
+                irrep_instance_np[i,j] = val
+        except AttributeError:
+            irrep_instance_np = irrep_instance.numpy()
         eigenvalue_list = eigen_data[DATA.eigval_lists][r]
         if not irreps_of_z[r]:  # matrix of zeros
             irrep_of_g_inverse_z_np = irreps_of_z[r]
             traces[r] = {eigenvalue: 0 for eigenvalue in eigenvalue_list}
         else:
             irrep_of_g_inverse_z_np = irreps_of_z_np[r] @ irrep_instance_np
             eigenvectors = eigen_data[DATA.eigvec_lists][r]
@@ -396,15 +398,34 @@
                     traces[r][eig] += mat[v]
                 else:
                     traces[r][eig] = mat[v]
         full_trace = irrep_of_g_inverse_z_np.trace()
         sum_of_partial_traces = sum(traces[r].values())
         if not sum_of_partial_traces - full_trace < 1e-04:
             print(f"Sum of partial traces ({round(sum_of_partial_traces, 5)}) is very different from the full trace ({round(full_trace, 5)}) for irrep {r}.")
+            # Add missing partial trace that we think is missing due to error.
+            error = full_trace - sum_of_partial_traces
+            very_small_eigenvalue = 10**(-10)
+            traces[r][very_small_eigenvalue] = error
     
+    if ERROR_CORRECTION_ENABLED:
+        dims = [irrep_z.shape[0] for irrep_z in irreps_of_z_np]
+        L_0 = (1/framework.num_genomes()) * sum(
+            dim * sum(traces[r].values())
+            for r, dim in enumerate(dims)
+        )
+        print(L_0)
+        error = 0.0 - L_0
+        error_per_dim = (error / len(dims)) * (framework.
+        num_genomes())
+        print(f"Error of {error} found. Correcting by {error_per_dim} per dimension.")
+        for r, dim in enumerate(dims):
+            for eigenvalue in traces[r].keys():
+                traces[r][eigenvalue] += (error_per_dim / (dim * len(traces[r].keys())))
+
     if DATA.partial_traces not in model.data_bundle:
         model.data_bundle[DATA.partial_traces] = {}
     model.data_bundle[DATA.partial_traces][instance_inverse] = traces
 
     return eigen_data[DATA.eigval_sets], traces
 
 
@@ -448,28 +469,29 @@
             eig_lists,
             irreps_of_z,
         )
     else:
         eig_lists, traces = _partial_traces_for_genome_using_eigenvectors(
             framework, model, instance, irreps, irreps_of_zs, irreps_of_z
         )
+        eig_lists = [list(traces[r].keys()) for r in range(len(traces))]
     dims = [irrep_of_zs.nrows() for irrep_of_zs in irreps_of_zs]
 
     def likelihood(t):
         ans = 0
         for r, dim in enumerate(dims):
-                ans += (
-                    Z.order()
-                    * (exp(-t) / G.order())
-                    * dim
-                    * sum(
-                        exp(eigenvalue * t) * traces[r][eigenvalue]
-                        for eigenvalue in eig_lists[r]
-                    )
+            ans += (
+                Z.order()
+                * (exp(-t) / G.order())
+                * dim
+                * sum(
+                    exp(eigenvalue * t) * traces[r][eigenvalue]
+                    for eigenvalue in eig_lists[r]
                 )
+            )
         return real(ans)
 
     return likelihood
 
 
 def min_distance(framework, model, genome_reps=None, weighted=False):
     """Return dictionary of minimum distances ref->genome, using inverse of model probabilities as weights (or not)"""
@@ -540,15 +562,35 @@
     return MFTP_distances
 
 def fast_MFPT(framework, model):
     reg_rep, genomes = framework.fast_reg_rep_of_zs(model)
     Q = reg_rep[1:,1:] # Remove the absorbing state
     m = Q.shape[0] # n - 1
     A = scipy.sparse.identity(m) - Q
-    scipy.sparse.linalg.cg(A, np.ones(m))
+    result = [0] + scipy.sparse.linalg.cg(A, np.ones(m))[0].tolist()
+    output_dict = {}
+    for genome, index in genomes.items():
+        output_dict[genome] = result[index]
+    return output_dict
+
+def fast_step_probabilities(framework, model, limit=20):
+    reg_rep, genomes = framework.fast_reg_rep_of_zs(model)
+    vector = reg_rep[0,:]
+    probs = []
+    for _ in range(limit - 1):
+        probs.append(vector.todense())
+        vector = vector @ reg_rep
+    probabilities = np.array(probs).transpose()
+    output_dict = {}
+    for genome, index in genomes.items():
+        output_dict[genome] = [0] + probabilities[index].tolist()[0]
+    identity = framework.one_row(framework.identity_instance())
+    output_dict[identity][0] = 1
+    return output_dict
+    
 
 def dict_to_distance_matrix(distances, framework, genomes=None):
     """If need to convert to pairwise distances, supply a list of genomes."""
     if genomes is not None:
         D = np.zeros((len(genomes), len(genomes)))
         for i in range(len(genomes)):
             canonical_i = framework.canonical_instance(
```

### Comparing `cgt-0.4.0/cgt/enums.py` & `cgt-0.4.1/cgt/enums.py`

 * *Files identical despite different names*

### Comparing `cgt-0.4.0/cgt/hyperoctahedral.py` & `cgt-0.4.1/cgt/hyperoctahedral.py`

 * *Files identical despite different names*

### Comparing `cgt-0.4.0/cgt/models.py` & `cgt-0.4.1/cgt/models.py`

 * *Files identical despite different names*

### Comparing `cgt-0.4.0/cgt/parsers.py` & `cgt-0.4.1/cgt/parsers.py`

 * *Files identical despite different names*

### Comparing `cgt-0.4.0/cgt/plotting.py` & `cgt-0.4.1/cgt/plotting.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 import cgt
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from cycler import cycler
 import numpy as np
+from cgt.enums import DATA
 
 
 def latex_figure_setup():
     """
     Sets up the matplotlib environment to use LaTeX for all text.
     """
     nice_fonts = {
@@ -31,30 +32,36 @@
         * cycler("linestyle", ["-", "--", ":"])
     )
     plt.rc("axes", prop_cycle=monochrome)
 
 
 def x_axis_limit_for_framework(framework):
     n = framework.n
-    from_testing = {1: 10, 2: 10, 3: 10, 4: 14, 5: 22, 6: 26, 7: 34, 8: 40, 9: 98}
+    from_testing = { 1: 10, 2: 10, 3: 10, 4: 14, 5: 22, 6: 26, 7: 34, 8: 40, 9: 98 }
     if n in from_testing:
         return from_testing[n]
     else:
         return from_testing[2 * max(from_testing.keys())]
 
 
 def plot_likelihood_and_probability(framework, model, instance, width=6, height=4, tmax = None, dpi=300, use_eigenvectors=True):
-    a = cgt.distances.prob_to_reach_in_steps_func(framework, model, instance, use_eigenvectors=use_eigenvectors)
+    canonical_instance = framework.canonical_instance(instance)
     L = cgt.distances.likelihood_function(
         framework, model, instance, use_eigenvectors=use_eigenvectors
     )
     if tmax is None:
         max_x = x_axis_limit_for_framework(framework)
     else:
         max_x = tmax
+    if DATA.reg_rep_of_zs in model.data_bundle:
+        stepwise_dists = cgt.distances.fast_step_probabilities(framework, model, limit = max_x + 1)[canonical_instance]
+        def a(k):
+            return stepwise_dists[k]
+    else:
+        a = cgt.distances.prob_to_reach_in_steps_func(framework, model, instance, use_eigenvectors=use_eigenvectors)
     tvec_L = list(np.arange(0, max_x + 1, 0.2))
     tvec = list(np.arange(0, max_x + 1, 1))
     latex_figure_setup()
     plt.figure(figsize=(width, height), dpi=dpi)
     plt.scatter(tvec, [a(t) for t in tvec], color="black", s=3)
     plt.plot(
         tvec,
@@ -67,15 +74,15 @@
     plt.plot(
         tvec_L,
         [L(t) for t in tvec_L],
         color="black",
         linestyle="solid",
         label="Likelihood",
     )
-    plt.title(f"Genome: z{str(framework.canonical_instance(instance))}")
+    plt.title(f"Genome: z{str(canonical_instance)}")
     n = framework.n
     if n < 9:
         x_tick_list = list(range(0, 9, 1)) + list(range(10, max_x + 1, 2))
     else: 
         x_tick_list = list(range(0, max_x + 1, 5))
     plt.xticks(x_tick_list)
     # Legend without border
```

### Comparing `cgt-0.4.0/cgt/position_paradigm.py` & `cgt-0.4.1/cgt/position_paradigm.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,14 +412,17 @@
         for elt in subgroup:
             yield one_row(elt) if not cycles else self.cycles(one_row(elt))
 
     def fast_reg_rep_of_zs(self, model):
         """
         
         """
+        if self.symmetry is not SYMMETRY.circular:
+            raise NotImplementedError("Only circular genomes are supported for now. Use another regular rep function.")
+
         if DATA.reg_rep_of_zs in model.data_bundle:
             return model.data_bundle[DATA.reg_rep_of_zs]
         
         signed_perms = SignedPermutations(self.n)
 
         def one_row(elt):
             elt_dict = elt.dict()
```

### Comparing `cgt-0.4.0/cgt/rearrangements.py` & `cgt-0.4.1/cgt/rearrangements.py`

 * *Files identical despite different names*

### Comparing `cgt-0.4.0/cgt/simulations.py` & `cgt-0.4.1/cgt/simulations.py`

 * *Files identical despite different names*

### Comparing `cgt-0.4.0/cgt/structures.py` & `cgt-0.4.1/cgt/structures.py`

 * *Files identical despite different names*

### Comparing `cgt-0.4.0/cgt/tests/test_conversions.py` & `cgt-0.4.1/cgt/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `cgt-0.4.0/cgt/tests/test_hyperoctahedral.py` & `cgt-0.4.1/cgt/tests/test_hyperoctahedral.py`

 * *Files identical despite different names*

### Comparing `cgt-0.4.0/cgt/tests/test_min_distances.py` & `cgt-0.4.1/cgt/tests/test_min_distances.py`

 * *Files identical despite different names*

### Comparing `cgt-0.4.0/cgt/visualisation.py` & `cgt-0.4.1/cgt/visualisation.py`

 * *Files identical despite different names*

### Comparing `cgt-0.4.0/cgt.egg-info/PKG-INFO` & `cgt-0.4.1/cgt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgt
-Version: 0.4.0
+Version: 0.4.1
 Summary: Tools for representing genomes in sage
 Home-page: https://github.com/js51/Circular-genome-tools
 Author: Joshua Stevenson
 Author-email: joshua.stevenson@utas.edu.au
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cgt-0.4.0/cgt.egg-info/SOURCES.txt` & `cgt-0.4.1/cgt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cgt-0.4.0/setup.py` & `cgt-0.4.1/setup.py`

 * *Files identical despite different names*

