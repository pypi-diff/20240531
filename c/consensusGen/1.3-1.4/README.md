# Comparing `tmp/consensusgen-1.3.tar.gz` & `tmp/consensusgen-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consensusgen-1.3.tar", last modified: Fri May 31 11:57:33 2024, max compression
+gzip compressed data, was "consensusgen-1.4.tar", last modified: Fri May 31 12:54:43 2024, max compression
```

## Comparing `consensusgen-1.3.tar` & `consensusgen-1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:57:33.581230 consensusgen-1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-31 11:57:24.000000 consensusgen-1.3/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 11:57:24.000000 consensusgen-1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-31 11:57:33.581230 consensusgen-1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-31 11:57:24.000000 consensusgen-1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:57:33.581230 consensusgen-1.3/consensusGen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-31 11:57:33.000000 consensusgen-1.3/consensusGen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-31 11:57:33.000000 consensusgen-1.3/consensusGen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 11:57:33.000000 consensusgen-1.3/consensusGen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 11:57:33.000000 consensusgen-1.3/consensusGen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-31 11:57:33.000000 consensusgen-1.3/consensusGen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:57:33.581230 consensusgen-1.3/consensusgen/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 11:57:24.000000 consensusgen-1.3/consensusgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-05-31 11:57:24.000000 consensusgen-1.3/consensusgen/consensusGen.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 11:57:33.581230 consensusgen-1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-31 11:57:24.000000 consensusgen-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:54:43.118082 consensusgen-1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-31 12:54:34.000000 consensusgen-1.4/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 12:54:34.000000 consensusgen-1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-31 12:54:43.118082 consensusgen-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-31 12:54:34.000000 consensusgen-1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:54:43.118082 consensusgen-1.4/consensusGen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-31 12:54:43.000000 consensusgen-1.4/consensusGen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-31 12:54:43.000000 consensusgen-1.4/consensusGen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 12:54:43.000000 consensusgen-1.4/consensusGen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 12:54:43.000000 consensusgen-1.4/consensusGen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-31 12:54:43.000000 consensusgen-1.4/consensusGen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:54:43.118082 consensusgen-1.4/consensusgen/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 12:54:34.000000 consensusgen-1.4/consensusgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-05-31 12:54:34.000000 consensusgen-1.4/consensusgen/consensusGen.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 12:54:43.118082 consensusgen-1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-31 12:54:34.000000 consensusgen-1.4/setup.py
```

### Comparing `consensusgen-1.3/LICENCE.md` & `consensusgen-1.4/LICENCE.md`

 * *Files identical despite different names*

### Comparing `consensusgen-1.3/PKG-INFO` & `consensusgen-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consensusGen
-Version: 1.3
+Version: 1.4
 Summary: Genetic algorithm for consensus building
 Home-page: https://pypi.org/project/consensusGen/
 Author: RomainCoulon (Romain Coulon)
 Author-email: <romain.coulon@bipm.org>
 Project-URL: Documentation, https://github.com/RomainCoulon/consensusGen/
 Keywords: genetic algorithm,inter-laboratory comparison,consenus building
 Classifier: Development Status :: 4 - Beta
```

### Comparing `consensusgen-1.3/consensusGen.egg-info/PKG-INFO` & `consensusgen-1.4/consensusGen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consensusGen
-Version: 1.3
+Version: 1.4
 Summary: Genetic algorithm for consensus building
 Home-page: https://pypi.org/project/consensusGen/
 Author: RomainCoulon (Romain Coulon)
 Author-email: <romain.coulon@bipm.org>
 Project-URL: Documentation, https://github.com/RomainCoulon/consensusGen/
 Keywords: genetic algorithm,inter-laboratory comparison,consenus building
 Classifier: Development Status :: 4 - Beta
```

### Comparing `consensusgen-1.3/consensusgen/consensusGen.py` & `consensusgen-1.4/consensusgen/consensusGen.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import numpy as np
 import matplotlib.pyplot as plt
 
 def consensusGen(X, u, *, ng=3, ni=8000):
     """Calculate a reference value using an evolutionary algorithm.
     See: Romain Coulon and Steven Judge 2021 Metrologia 58 065007
-    DOI 10.1088/1681-7575/ac31c0
+    https://doi.org/10.1088/1681-7575/ac31c0
 
     Parameters
     ----------
     X : list of floats
         Measurement values.
     u : list of floats
         Standard uncertainties of measurement values.
@@ -118,14 +118,60 @@
     u_mu = uKCRV[-1] # Return the standard uncerainty of the consensus value from the last generation
     if ng==0: gLpop = Q2
     else: gLpop = Q[G]
     w = Wgth / np.sum(Wgth) # Calculate the normalized weights
 
     return mu, u_mu, Q2, gLpop, w
 
+def DoE(x,u,x_ref,ux_ref,*,w=[],k=2):
+    """This function aims to calculate Degrees of equivalence.
+    
+    References: 
+        [Accred Qual Assur (2008)13:83-89, Metrologia 52(2015)S200]
+        https://link.springer.com/article/10.1007/s00769-007-0330-1
+        https://iopscience.iop.org/article/10.1088/0026-1394/52/3/S200/pdf
+    
+    :param x: Sample of values
+    :type x: array of floats
+    :param u: Sample of standard uncertainties related to the values
+    :type u: array of floats
+    :param x_ref: Estimation of the reference value
+    :type x_ref: float
+    :param ux_ref: Estimation of uncertainty of the reference value
+    :type ux_ref: float
+    
+    :param w: (Optional) Weights associated to each data point.
+    :type w: array of floats
+    :param k: (Optional) Coverage factor (set by default equal to 2)
+    :type k: float    
+    
+    :param d: Estimation of the degrees of equivalence
+    :type d: array of floats
+    :param ud: Estimation of the uncertainties related to the degrees of equivalence
+    :type ud: array of floats    
+    :param dr: Estimation of the relative degrees of equivalence
+    :type dr: array of floats
+    :param udr: Estimation of the uncertainties related to the relative degrees of equivalence
+    :type udr: array of floats  
+    
+    :return y: d, ud, dr, udr
+    :rtype y: tuple
+    """
+    
+    x=np.asarray(x) # format input data
+    u=np.asarray(u) # format input data
+    w=np.asarray(w) # format input data
+    k=2
+    d=x-x_ref  # euclidian distance from the reference value
+    u2d=(1-2*w)*u**2+ux_ref**2 # variance associated with DE (the weight factor is available)
+    ud=k*u2d**0.5     # enlarged standard deviation associated with DoE
+    dr=d/x_ref        # relative DoE
+    udr=ud/x_ref      # relative u(DoE)
+    return d, ud, dr, udr
+
 def displayResult(X, u, result, *, lab=False):
     """
     Display the result of the genetic algorithm consensusGen()
 
     Parameters
     ----------
     X : list of floats
@@ -139,35 +185,61 @@
 
     Returns
     -------
     None.
     """
     mu, u_mu, g0pop, gLpop, w = result
     nX = len(X)
-
-    print(f"The consensus value is {mu:.4g} ± {u_mu:.2g}")
+    d, ud, dr, udr = DoE(X,u,mu,u_mu,w=w)
+    MAD=np.median(abs(d)) # median of absolute value of degrees of equivalence
+    x=d/MAD            # x-coordinates
+    y=ud/MAD           # y-coordinates
+    
+    print(f"The consensus value is {mu:.4g} ± {u_mu:.2g} (k=1)")
 
     if not lab:
-        lab = np.linspace(1, nX, nX)
-    labstr = [str(int(x)) for x in lab]
+        lab = np.linspace(1, nX, nX)-1
+        labstr = [str(int(x)) for x in lab]
+    else:
+        labstr = lab
 
     # Data plot
     plt.figure("Data")
     plt.clf()
+    plt.title("Data points and the reference value")
     plt.errorbar(labstr, X, yerr=u, fmt='ok', capsize=3, ecolor='k', label=r"$x_i$")
-    plt.plot(lab - 1, np.ones(nX) * mu, "-r", label=r"$\hat{\mu}$")
-    plt.plot(lab - 1, np.ones(nX) * (mu + u_mu), "--r", label=r"$\hat{\mu} + u(\hat{\mu})$")
-    plt.plot(lab - 1, np.ones(nX) * (mu - u_mu), "--r", label=r"$\hat{\mu} - u(\hat{\mu})$")
+    plt.plot(lab, np.ones(nX) * mu, "-r", label=r"$\hat{\mu}$")
+    plt.plot(lab, np.ones(nX) * (mu + u_mu), "--r", label=r"$\hat{\mu} + u(\hat{\mu})$")
+    plt.plot(lab, np.ones(nX) * (mu - u_mu), "--r", label=r"$\hat{\mu} - u(\hat{\mu})$")
     plt.ylabel(r'Value', fontsize=12)
     plt.xlabel(r'Participant', fontsize=12)
     plt.legend()
 
+    # Data plot
+    plt.figure("DoE")
+    plt.clf()
+    plt.title("Degrees of equivalence")
+    plt.errorbar(labstr, d, yerr=ud, fmt='ok', capsize=3, ecolor='k')
+    plt.plot(lab, np.zeros(nX), "-r")
+    plt.ylabel(r'Value', fontsize=12)
+    plt.xlabel(r'Participant', fontsize=12)
+
+    # Data plot
+    plt.figure("rDoE")
+    plt.clf()
+    plt.title("Relative degrees of equivalence")
+    plt.errorbar(labstr, dr, yerr=udr, fmt='ok', capsize=3, ecolor='k')
+    plt.plot(lab, np.zeros(nX), "-r")
+    plt.ylabel(r'Value', fontsize=12)
+    plt.xlabel(r'Participant', fontsize=12)
+
     # Weights plot
     plt.figure("Weights")
     plt.clf()
+    plt.title("Weights of the data in the reference value")
     plt.bar(labstr, w)
     plt.ylabel(r'$w_i$', fontsize=12)
     plt.xlabel(r'Participant', fontsize=12)
     plt.legend()
 
     # Distributions plot
     plt.figure("Distributions")
@@ -177,13 +249,45 @@
     plt.ylabel(r'$p(x_i)$', fontsize=12)
     plt.xlabel(r'$x$', fontsize=12)
     plt.legend()
 
     # Show plots
     plt.show()
 
+    # PomPlot
+    plt.figure("PomPlot")
+    plt.clf()
+    # plt.title("PomPlot")
+    # plt.rcParams['xtick.bottom'] = plt.rcParams['xtick.labelbottom'] = False
+    # plt.rcParams['xtick.top'] = plt.rcParams['xtick.labeltop'] = True
+    fig, ax = plt.subplots() # create of subplot object
+    ax.plot(x,y,'ok')
+    # define the frame
+    plt.ylim(1.1*max(y),0)
+    plt.xlim(1.1*min(x),1.1*max(x))
+    # print axes title
+    ax.set_title(r'$D_{i}$/med($D$)', fontsize=14)
+    ax.set_ylabel(r'$u(D_{i})$/med($D$)', fontsize=14)
+    # draw the lignes
+    x0=np.arange(-9,9,1)
+    y0=np.arange(-9,9,1)
+    plt.plot(x0,y0,'-g',label=r'$\zeta=1$')
+    plt.plot(x0,-y0,'-g')
+    plt.plot(x0,y0/2,'-b',label=r'$\zeta=2$')
+    plt.plot(x0,-y0/2,'-b')
+    plt.plot(x0,y0/3,'-r',label=r'$\zeta=3$')
+    plt.plot(x0,-y0/3,'-r')
+    for i,g in enumerate(labstr):
+        plt.text(x[i]+0.1,y[i]+0.1,g)
+    plt.legend() # display the legend
+
+    # Show plots
+    plt.show()
+
+
 # Example usage (replace with actual function call and data):
-# X = [10, 11, 14, 10, 10.5, 10]
+# l = ["A", "B", "C", "D", "E", "F"]
+# X = [10.1, 11, 14, 10, 10.5, 9.8]
 # u = [1, 1, 1, 2, 1, 1.5]
 # result = consensusGen(X, u, ng=1)
-# displayResult(X, u, result)
+# displayResult(X, u, result, lab=l)
```

### Comparing `consensusgen-1.3/setup.py` & `consensusgen-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = "1.3"
+
+VERSION = "1.4"
+
 
 DESCRIPTION = "Genetic algorithm for consensus building"
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
```

