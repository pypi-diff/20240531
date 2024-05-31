# Comparing `tmp/consensusgen-1.1.tar.gz` & `tmp/consensusgen-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consensusgen-1.1.tar", last modified: Fri May 31 11:37:56 2024, max compression
+gzip compressed data, was "consensusgen-1.2.tar", last modified: Fri May 31 11:48:25 2024, max compression
```

## Comparing `consensusgen-1.1.tar` & `consensusgen-1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:37:56.425220 consensusgen-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-31 11:37:47.000000 consensusgen-1.1/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:37:47.000000 consensusgen-1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-31 11:37:56.425220 consensusgen-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-31 11:37:47.000000 consensusgen-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:37:56.425220 consensusgen-1.1/consensusGen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-31 11:37:56.000000 consensusgen-1.1/consensusGen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-31 11:37:56.000000 consensusgen-1.1/consensusGen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 11:37:56.000000 consensusgen-1.1/consensusGen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 11:37:56.000000 consensusgen-1.1/consensusGen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-31 11:37:56.000000 consensusgen-1.1/consensusGen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:37:56.425220 consensusgen-1.1/consensusgen/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-31 11:37:47.000000 consensusgen-1.1/consensusgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-31 11:37:47.000000 consensusgen-1.1/consensusgen/consensusGen.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 11:37:56.425220 consensusgen-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-31 11:37:47.000000 consensusgen-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:48:25.461360 consensusgen-1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-31 11:48:15.000000 consensusgen-1.2/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:48:15.000000 consensusgen-1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-31 11:48:25.461360 consensusgen-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-31 11:48:15.000000 consensusgen-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:48:25.461360 consensusgen-1.2/consensusGen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-31 11:48:25.000000 consensusgen-1.2/consensusGen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-31 11:48:25.000000 consensusgen-1.2/consensusGen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 11:48:25.000000 consensusgen-1.2/consensusGen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 11:48:25.000000 consensusgen-1.2/consensusGen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-31 11:48:25.000000 consensusgen-1.2/consensusGen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:48:25.461360 consensusgen-1.2/consensusgen/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-31 11:48:15.000000 consensusgen-1.2/consensusgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-05-31 11:48:15.000000 consensusgen-1.2/consensusgen/consensusGen.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 11:48:25.461360 consensusgen-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-31 11:48:15.000000 consensusgen-1.2/setup.py
```

### Comparing `consensusgen-1.1/LICENCE.md` & `consensusgen-1.2/LICENCE.md`

 * *Files identical despite different names*

### Comparing `consensusgen-1.1/PKG-INFO` & `consensusgen-1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consensusGen
-Version: 1.1
+Version: 1.2
 Summary: Genetic algorithm for consensus building
 Home-page: https://pypi.org/project/consensusGen/
 Author: RomainCoulon (Romain Coulon)
 Author-email: <romain.coulon@bipm.org>
 Project-URL: Documentation, https://github.com/RomainCoulon/consensusGen/
 Keywords: genetic algorithm,inter-laboratory comparison,consenus building
 Classifier: Development Status :: 4 - Beta
```

### Comparing `consensusgen-1.1/consensusGen.egg-info/PKG-INFO` & `consensusgen-1.2/consensusGen.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consensusGen
-Version: 1.1
+Version: 1.2
 Summary: Genetic algorithm for consensus building
 Home-page: https://pypi.org/project/consensusGen/
 Author: RomainCoulon (Romain Coulon)
 Author-email: <romain.coulon@bipm.org>
 Project-URL: Documentation, https://github.com/RomainCoulon/consensusGen/
 Keywords: genetic algorithm,inter-laboratory comparison,consenus building
 Classifier: Development Status :: 4 - Beta
```

### Comparing `consensusgen-1.1/consensusgen/consensusGen.py` & `consensusgen-1.2/consensusgen/consensusGen.py`

 * *Files 21% similar despite different names*

```diff
@@ -34,93 +34,97 @@
         Linear Pool distribution.
     gLpop : list of floats
         EA filtered distribution.
     w : list of floats
         Weights associated with laboratories.
     """
 
-    m = len(X)
+    m = len(X) # Number of groups
     ni_per_group = ni // m  # Number of individuals per group
 
+    # Initialize vectors of indices for generations, groups and individuals per group 
     if ng == 0:
         generations = 0
     else:
         generations = range(ng)
 
     group_indices = range(m)
     individual_indices = range(ni_per_group)
 
     # Initialize matrices and arrays
     Gen2 = np.empty((m, ni_per_group))
     Gen3 = np.empty((m, ni_per_group))
-    q = np.empty((m, ni_per_group))
-    q2 = np.zeros((m, ni_per_group))
+    q = np.empty((m, ni_per_group)) # Matrix of phenotypes before the evolution step 
+    q2 = np.zeros((m, ni_per_group)) # Matrix of phenotypes after the evolution step 
     w = np.ones((m, ni_per_group))
 
-    KCRV = np.empty(ng)  # Mean of the whole population at each generation
-    uKCRV = np.empty(ng)  # Standard deviation of the whole population at each generation
+    if ng == 0:
+        KCRV = np.empty(1)  # Mean of the whole population at each generation
+        uKCRV = np.empty(1)  # Standard deviation of the whole population at each generation
+    else:
+        KCRV = np.empty(ng)  # Mean of the whole population at each generation
+        uKCRV = np.empty(ng)  # Standard deviation of the whole population at each generation
 
     # Generate the first generation
     for i in group_indices:
-        q[i] = np.random.normal(X[i], u[i], ni_per_group)
+        q[i] = np.random.normal(X[i], u[i], ni_per_group) # Generate individuals from Normal distributions 
 
     Q2 = q.ravel()  # Suppress the group separation
 
     if ng == 0:
-        KCRV[0] = np.mean(Q2)
-        uKCRV[0] = np.std(Q2) / np.sqrt(m)
-        Q = Q2
-        Wgth = np.ones(m)
+        KCRV[0] = np.mean(Q2) # Calculate the mean of the linear pooling
+        uKCRV[0] = np.std(Q2) / np.sqrt(m) # Calculate the standard uncertainty of the mean of the linear pooling
+        Wgth = np.ones(m) # set equal weights to each group
     else:
         # Assign initial genomes to each individual
         for i in group_indices:
-            Gen2[i, :] = i + 1
+            Gen2[i, :] = i + 1 # Give the same genome to all individals within a group - genome is encoded by the group indice
             Gen3[i, :] = i + 1
 
-        for t in generations:
+        for t in generations: # Run an evolution step
             q2.fill(0)  # Reset q2 for the new generation
 
             for i in group_indices:
                 for j in individual_indices:
-                    if w[i, j] != 0:
-                        # Find the nearest phenotype
+                    if w[i, j] != 0: # if not already killed
+                        # Find the nearest phenotype of the individuals (i,j)
                         Mat1 = np.abs(q[i, j] - q)
                         Mat1[i, j] = float("inf")  # Exclude self
                         nearest_idx = np.unravel_index(np.argmin(Mat1), Mat1.shape)
-                        l, c = nearest_idx
+                        l, c = nearest_idx # indices of the nearest phenotype
 
-                        if Gen2[i, j] != Gen2[l, c]:
+                        if Gen2[i, j] != Gen2[l, c]: # Outbreading
                             r = np.random.rand()
                             q2[i, j] = r * q[i, j] + (1 - r) * q[l, c]  # Crossover
-                            Gen3[i, j] = np.sqrt(Gen2[i, j] * Gen2[l, c])
-                        else:
-                            w[i, j] = 0
-                            q2[i, j] = q[i, j]
+                            Gen3[i, j] = np.sqrt(Gen2[i, j] * Gen2[l, c]) # Attribute a new genome
+                        else: # Inbreading
+                            w[i, j] = 0  # Kill the individuals
+                            q2[i, j] = q[i, j] # Record 
                     else:
-                        w[i, j] = 0
-                        q2[i, j] = q[i, j]
+                        w[i, j] = 0 # Kill the individuals 
+                        q2[i, j] = q[i, j] # Record
 
-            q = q2.copy()
-            Gen2 = Gen3.copy()
-            Q = q.ravel()
-            W = w.ravel()
-            G = np.where(W != 0)
-
-            Wgth = np.array([np.sum(w[i] != 0) / ni_per_group for i in group_indices])
-
-            KCRV[t] = np.mean(Q[G])
-            uKCRV[t] = np.std(Q[G]) / np.sqrt(m)
-
-    mu = KCRV[-1]
-    u_mu = uKCRV[-1]
-    g0pop = Q2
-    gLpop = Q[G]
-    w = Wgth / np.sum(Wgth)
+            q = q2.copy() # Memorize the phenotypes
+            Gen2 = Gen3.copy() # Memorize the genotype
+            Q = q.ravel() # Suppress the group separation
+            W = w.ravel() # Suppress the group separation
+            G = np.where(W != 0) # Indices of alived individuals
+
+            Wgth = np.array([np.sum(w[i] != 0) / ni_per_group for i in group_indices]) # Calculation of the weights of each group
+
+            KCRV[t] = np.mean(Q[G]) # Calculate the mean of the new distribution 
+            uKCRV[t] = np.std(Q[G]) / np.sqrt(m) # Calculate the standard uncertainty of the mean of the new distribution 
+
+    mu = KCRV[-1] # Return the consensus value from the last generation
+    u_mu = uKCRV[-1] # Return the standard uncerainty of the consensus value from the last generation
+    if ng==0: gLpop = Q2
+    else: gLpop = Q[G]
+    w = Wgth / np.sum(Wgth) # Calculate the normalized weights
 
-    return mu, u_mu, g0pop, gLpop, w
+    return mu, u_mu, Q2, gLpop, w
 
 def displayResult(X, u, result, *, lab=False):
     """
     Display the result of the genetic algorithm consensusGen()
 
     Parameters
     ----------
@@ -174,12 +178,12 @@
     plt.xlabel(r'$x$', fontsize=12)
     plt.legend()
 
     # Show plots
     plt.show()
 
 # Example usage (replace with actual function call and data):
-# X = [your_data]
-# u = [your_uncertainties]
-# result = consensusGen(X, u)
+# X = [10, 11, 14, 10, 10.5, 10]
+# u = [1, 1, 1, 2, 1, 1.5]
+# result = consensusGen(X, u, ng=1)
 # displayResult(X, u, result)
```

### Comparing `consensusgen-1.1/setup.py` & `consensusgen-1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = "1.1"
+VERSION = "1.2"
+
 DESCRIPTION = "Genetic algorithm for consensus building"
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name = "consensusGen",
```

