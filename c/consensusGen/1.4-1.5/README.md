# Comparing `tmp/consensusgen-1.4.tar.gz` & `tmp/consensusgen-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consensusgen-1.4.tar", last modified: Fri May 31 12:54:43 2024, max compression
+gzip compressed data, was "consensusgen-1.5.tar", last modified: Fri May 31 13:20:08 2024, max compression
```

## Comparing `consensusgen-1.4.tar` & `consensusgen-1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:54:43.118082 consensusgen-1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-31 12:54:34.000000 consensusgen-1.4/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 12:54:34.000000 consensusgen-1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-31 12:54:43.118082 consensusgen-1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-31 12:54:34.000000 consensusgen-1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:54:43.118082 consensusgen-1.4/consensusGen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-31 12:54:43.000000 consensusgen-1.4/consensusGen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-31 12:54:43.000000 consensusgen-1.4/consensusGen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 12:54:43.000000 consensusgen-1.4/consensusGen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 12:54:43.000000 consensusgen-1.4/consensusGen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-31 12:54:43.000000 consensusgen-1.4/consensusGen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:54:43.118082 consensusgen-1.4/consensusgen/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 12:54:34.000000 consensusgen-1.4/consensusgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-05-31 12:54:34.000000 consensusgen-1.4/consensusgen/consensusGen.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 12:54:43.118082 consensusgen-1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-31 12:54:34.000000 consensusgen-1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:20:08.763919 consensusgen-1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-31 13:20:00.000000 consensusgen-1.5/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:20:00.000000 consensusgen-1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-31 13:20:08.763919 consensusgen-1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-31 13:20:00.000000 consensusgen-1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:20:08.763919 consensusgen-1.5/consensusGen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-31 13:20:08.000000 consensusgen-1.5/consensusGen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-31 13:20:08.000000 consensusgen-1.5/consensusGen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:20:08.000000 consensusgen-1.5/consensusGen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 13:20:08.000000 consensusgen-1.5/consensusGen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-31 13:20:08.000000 consensusgen-1.5/consensusGen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:20:08.763919 consensusgen-1.5/consensusgen/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 13:20:00.000000 consensusgen-1.5/consensusgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10802 2024-05-31 13:20:00.000000 consensusgen-1.5/consensusgen/consensusGen.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 13:20:08.763919 consensusgen-1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-31 13:20:00.000000 consensusgen-1.5/setup.py
```

### Comparing `consensusgen-1.4/LICENCE.md` & `consensusgen-1.5/LICENCE.md`

 * *Files identical despite different names*

### Comparing `consensusgen-1.4/PKG-INFO` & `consensusgen-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consensusGen
-Version: 1.4
+Version: 1.5
 Summary: Genetic algorithm for consensus building
 Home-page: https://pypi.org/project/consensusGen/
 Author: RomainCoulon (Romain Coulon)
 Author-email: <romain.coulon@bipm.org>
 Project-URL: Documentation, https://github.com/RomainCoulon/consensusGen/
 Keywords: genetic algorithm,inter-laboratory comparison,consenus building
 Classifier: Development Status :: 4 - Beta
```

### Comparing `consensusgen-1.4/consensusGen.egg-info/PKG-INFO` & `consensusgen-1.5/consensusGen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consensusGen
-Version: 1.4
+Version: 1.5
 Summary: Genetic algorithm for consensus building
 Home-page: https://pypi.org/project/consensusGen/
 Author: RomainCoulon (Romain Coulon)
 Author-email: <romain.coulon@bipm.org>
 Project-URL: Documentation, https://github.com/RomainCoulon/consensusGen/
 Keywords: genetic algorithm,inter-laboratory comparison,consenus building
 Classifier: Development Status :: 4 - Beta
```

### Comparing `consensusgen-1.4/consensusgen/consensusGen.py` & `consensusgen-1.5/consensusgen/consensusGen.py`

 * *Files 3% similar despite different names*

```diff
@@ -190,22 +190,26 @@
     mu, u_mu, g0pop, gLpop, w = result
     nX = len(X)
     d, ud, dr, udr = DoE(X,u,mu,u_mu,w=w)
     MAD=np.median(abs(d)) # median of absolute value of degrees of equivalence
     x=d/MAD            # x-coordinates
     y=ud/MAD           # y-coordinates
     
-    print(f"The consensus value is {mu:.4g} ± {u_mu:.2g} (k=1)")
-
+    
     if not lab:
         lab = np.linspace(1, nX, nX)-1
         labstr = [str(int(x)) for x in lab]
     else:
         labstr = lab
-
+    
+    print(f"The consensus value is {mu:.4g} ± {u_mu:.2g} (k=1)")
+    print("The degrees of equivalence are:")
+    for il, lL in enumerate(labstr):
+        print(f"\t {lL}: {d[il]:.2g} ± {ud[il]:.2g} (k=2)")
+    
     # Data plot
     plt.figure("Data")
     plt.clf()
     plt.title("Data points and the reference value")
     plt.errorbar(labstr, X, yerr=u, fmt='ok', capsize=3, ecolor='k', label=r"$x_i$")
     plt.plot(lab, np.ones(nX) * mu, "-r", label=r"$\hat{\mu}$")
     plt.plot(lab, np.ones(nX) * (mu + u_mu), "--r", label=r"$\hat{\mu} + u(\hat{\mu})$")
@@ -281,13 +285,13 @@
     plt.legend() # display the legend
 
     # Show plots
     plt.show()
 
 
 # Example usage (replace with actual function call and data):
-# l = ["A", "B", "C", "D", "E", "F"]
-# X = [10.1, 11, 14, 10, 10.5, 9.8]
-# u = [1, 1, 1, 2, 1, 1.5]
-# result = consensusGen(X, u, ng=1)
-# displayResult(X, u, result, lab=l)
+l = ["A", "B", "C", "D", "E", "F"]
+X = [10.1, 11, 14, 10, 10.5, 9.8]
+u = [1, 1, 1, 2, 1, 1.5]
+result = consensusGen(X, u, ng=1)
+displayResult(X, u, result, lab=l)
```

### Comparing `consensusgen-1.4/setup.py` & `consensusgen-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = "1.4"
+VERSION = "1.5"
 
 
 DESCRIPTION = "Genetic algorithm for consensus building"
 
 with open("README.md", "r") as f:
     long_description = f.read()
```

