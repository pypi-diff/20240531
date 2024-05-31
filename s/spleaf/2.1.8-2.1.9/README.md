# Comparing `tmp/spleaf-2.1.8.tar.gz` & `tmp/spleaf-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spleaf-2.1.8.tar", last modified: Fri Nov 24 08:49:09 2023, max compression
+gzip compressed data, was "spleaf-2.1.9.tar", last modified: Tue Mar  5 11:55:22 2024, max compression
```

## Comparing `spleaf-2.1.8.tar` & `spleaf-2.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 08:49:09.358665 spleaf-2.1.8/
--rw-rw-rw-   0 root         (0) root         (0)    35147 2023-11-24 08:48:09.000000 spleaf-2.1.8/COPYING
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-11-24 08:48:09.000000 spleaf-2.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      841 2023-11-24 08:49:09.357665 spleaf-2.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      518 2023-11-24 08:48:09.000000 spleaf-2.1.8/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-11-24 08:48:09.000000 spleaf-2.1.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-24 08:49:09.358665 spleaf-2.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1568 2023-11-24 08:48:09.000000 spleaf-2.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 08:49:09.356665 spleaf-2.1.8/spleaf/
--rw-rw-rw-   0 root         (0) root         (0)      971 2023-11-24 08:48:09.000000 spleaf-2.1.8/spleaf/__info__.py
--rw-rw-rw-   0 root         (0) root         (0)    29194 2023-11-24 08:48:09.000000 spleaf-2.1.8/spleaf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17257 2023-11-24 08:48:09.000000 spleaf-2.1.8/spleaf/cov.py
--rw-rw-rw-   0 root         (0) root         (0)    49962 2023-11-24 08:48:09.000000 spleaf-2.1.8/spleaf/fenrir.py
--rw-rw-rw-   0 root         (0) root         (0)    30205 2023-11-24 08:48:09.000000 spleaf-2.1.8/spleaf/libspleaf.c
--rw-rw-rw-   0 root         (0) root         (0)     4571 2023-11-24 08:48:09.000000 spleaf-2.1.8/spleaf/libspleaf.h
--rw-rw-rw-   0 root         (0) root         (0)    61577 2023-11-24 08:48:09.000000 spleaf-2.1.8/spleaf/pywrapspleaf.c
--rw-rw-rw-   0 root         (0) root         (0)    82399 2023-11-24 08:48:09.000000 spleaf-2.1.8/spleaf/term.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 08:49:09.357665 spleaf-2.1.8/spleaf.egg-info/
--rw-r--r--   0 root         (0) root         (0)      841 2023-11-24 08:49:09.000000 spleaf-2.1.8/spleaf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      384 2023-11-24 08:49:09.000000 spleaf-2.1.8/spleaf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-24 08:49:09.000000 spleaf-2.1.8/spleaf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-11-24 08:49:09.000000 spleaf-2.1.8/spleaf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-11-24 08:49:09.000000 spleaf-2.1.8/spleaf.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 08:49:09.357665 spleaf-2.1.8/test/
--rw-rw-rw-   0 root         (0) root         (0)    27167 2023-11-24 08:48:09.000000 spleaf-2.1.8/test/test_cov.py
--rw-rw-rw-   0 root         (0) root         (0)    11276 2023-11-24 08:48:09.000000 spleaf-2.1.8/test/test_spleaf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 11:55:22.669007 spleaf-2.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)    13827 2024-03-05 11:54:14.000000 spleaf-2.1.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-03-05 11:54:14.000000 spleaf-2.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1099 2024-03-05 11:55:22.669007 spleaf-2.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      498 2024-03-05 11:54:14.000000 spleaf-2.1.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      681 2024-03-05 11:54:14.000000 spleaf-2.1.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-05 11:55:22.669007 spleaf-2.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-03-05 11:54:14.000000 spleaf-2.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 11:55:22.666006 spleaf-2.1.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 11:55:22.668007 spleaf-2.1.9/src/spleaf/
+-rw-rw-rw-   0 root         (0) root         (0)    29710 2024-03-05 11:54:14.000000 spleaf-2.1.9/src/spleaf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16742 2024-03-05 11:54:14.000000 spleaf-2.1.9/src/spleaf/cov.py
+-rw-rw-rw-   0 root         (0) root         (0)    50496 2024-03-05 11:54:14.000000 spleaf-2.1.9/src/spleaf/fenrir.py
+-rw-rw-rw-   0 root         (0) root         (0)    29579 2024-03-05 11:54:14.000000 spleaf-2.1.9/src/spleaf/libspleaf.c
+-rw-rw-rw-   0 root         (0) root         (0)     3945 2024-03-05 11:54:14.000000 spleaf-2.1.9/src/spleaf/libspleaf.h
+-rw-rw-rw-   0 root         (0) root         (0)    60951 2024-03-05 11:54:14.000000 spleaf-2.1.9/src/spleaf/pywrapspleaf.c
+-rw-rw-rw-   0 root         (0) root         (0)    85399 2024-03-05 11:54:14.000000 spleaf-2.1.9/src/spleaf/term.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 11:55:22.669007 spleaf-2.1.9/src/spleaf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1099 2024-03-05 11:55:22.000000 spleaf-2.1.9/src/spleaf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      414 2024-03-05 11:55:22.000000 spleaf-2.1.9/src/spleaf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-05 11:55:22.000000 spleaf-2.1.9/src/spleaf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-03-05 11:55:22.000000 spleaf-2.1.9/src/spleaf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-03-05 11:55:22.000000 spleaf-2.1.9/src/spleaf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 11:55:22.669007 spleaf-2.1.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    27638 2024-03-05 11:54:14.000000 spleaf-2.1.9/tests/test_cov.py
+-rw-rw-rw-   0 root         (0) root         (0)    11463 2024-03-05 11:54:14.000000 spleaf-2.1.9/tests/test_spleaf.py
```

### Comparing `spleaf-2.1.8/spleaf/__init__.py` & `spleaf-2.1.9/src/spleaf/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,20 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2019-2023 Jean-Baptiste Delisle
-#
-# This file is part of spleaf.
-#
-# spleaf is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# spleaf is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with spleaf.  If not, see <http://www.gnu.org/licenses/>.
+# Copyright 2019-2024 Jean-Baptiste Delisle
+# Licensed under the EUPL-1.2 or later
 
 __all__ = ['Spleaf']
 
 import numpy as np
+
 from . import libspleaf
-from .__info__ import __version__
 
 
-class Spleaf():
+class Spleaf:
   r"""
   Symmetric S+LEAF (semiseparable + leaf) matrix.
 
   A symmetric S+LEAF matrix :math:`C` is defined as
 
   .. math:: C = A + \mathrm{tril}(U V^T) + \mathrm{triu}(V U^T) + F,
 
@@ -111,17 +97,30 @@
     # Cholesky decomposition
     self.D = np.empty_like(A)
     self.W = np.empty_like(V)
     self.G = np.empty_like(F)
     self._S = np.empty(self.n * self.r * self.r)
     self._Z = np.empty((self.F.size + self.n) * self.r)
 
-    libspleaf.spleaf_cholesky(self.n, self.r, self.offsetrow, self.b, self.A,
-      self.U, self.V, self.phi, self.F, self.D, self.W, self.G, self._S,
-      self._Z)
+    libspleaf.spleaf_cholesky(
+      self.n,
+      self.r,
+      self.offsetrow,
+      self.b,
+      self.A,
+      self.U,
+      self.V,
+      self.phi,
+      self.F,
+      self.D,
+      self.W,
+      self.G,
+      self._S,
+      self._Z,
+    )
 
     # Back propagation (no init)
     self._grad_A = None
     self._grad_U = None
     self._grad_V = None
     self._grad_phi = None
     self._grad_F = None
@@ -149,34 +148,47 @@
     self._g_solveLT = np.empty(self.n * self.r)
 
   def _copy(self, x, copy):
     r"""
     Perform a copy if required else pass the object.
     """
     if copy and isinstance(x, np.ndarray):
-      return (x.copy())
+      return x.copy()
     else:
-      return (x)
+      return x
 
   def set_param(self, A, U, V, phi, F, copy=False):
     r"""
     Update the initial parameters (`A`, `U`, `V`, `phi`, `F`)
     and recompute the Cholesky decomposition of the matrix.
     """
 
     self.A = self._copy(A, copy)
     self.U = self._copy(U, copy)
     self.V = self._copy(V, copy)
     self.phi = self._copy(phi, copy)
     self.F = self._copy(F, copy)
 
     # Cholesky decomposition
-    libspleaf.spleaf_cholesky(self.n, self.r, self.offsetrow, self.b, self.A,
-      self.U, self.V, self.phi, self.F, self.D, self.W, self.G, self._S,
-      self._Z)
+    libspleaf.spleaf_cholesky(
+      self.n,
+      self.r,
+      self.offsetrow,
+      self.b,
+      self.A,
+      self.U,
+      self.V,
+      self.phi,
+      self.F,
+      self.D,
+      self.W,
+      self.G,
+      self._S,
+      self._Z,
+    )
 
     # Re-init logdet/sqD
     self._logdet_value = None
     self._sqD_value = None
 
   def expand(self):
     r"""
@@ -193,15 +205,15 @@
       for j in range(i - self.b[i], i):
         C[i, j] = self.F[self.offsetrow[i] + j]
       cumphi = np.ones(self.r)
       for j in range(i - 1, -1, -1):
         cumphi *= self.phi[j]
         C[i, j] += np.sum(cumphi * self.U[i] * self.V[j])
         C[j, i] = C[i, j]
-    return (C)
+    return C
 
   def expandL(self):
     r"""
     Expand :math:`L` as a full (n x n) matrix.
 
     Warnings
     --------
@@ -213,15 +225,15 @@
     for i in range(self.n):
       for j in range(i - self.b[i], i):
         L[i, j] = self.G[self.offsetrow[i] + j]
       cumphi = np.ones(self.r)
       for j in range(i - 1, -1, -1):
         cumphi *= self.phi[j]
         L[i, j] += np.sum(cumphi * self.U[i] * self.W[j])
-    return (L)
+    return L
 
   def expandInv(self):
     r"""
     Expand the inverse of the matrix as a full (n x n) matrix.
 
     Warnings
     --------
@@ -231,15 +243,15 @@
 
     invC = np.empty((self.n, self.n))
     ei = np.zeros(self.n)
     for i in range(self.n):
       ei[i] = 1.0
       invC[:, i] = self.solveLT(self.solveL(ei) / self.D)
       ei[i] = 0.0
-    return (invC)
+    return invC
 
   def expandInvL(self):
     r"""
     Expand :math:`L^{-1}` as a full (n x n) matrix.
 
     Warnings
     --------
@@ -249,15 +261,15 @@
 
     invL = np.empty((self.n, self.n))
     ei = np.zeros(self.n)
     for i in range(self.n):
       ei[i] = 1.0
       invL[:, i] = self.solveL(ei)
       ei[i] = 0.0
-    return (invL)
+    return invL
 
   def logdet(self):
     r"""
     Compute the (natural) logarithm of the determinant of the matrix.
 
     Returns
     -------
@@ -267,15 +279,15 @@
     Notes
     -----
     This is a lazy computation (the result is stored for future calls).
     """
 
     if self._logdet_value is None:
       self._logdet_value = np.sum(np.log(self.D))
-    return (self._logdet_value)
+    return self._logdet_value
 
   def sqD(self):
     r"""
     Compute the square-root of `D`.
 
     Returns
     -------
@@ -285,15 +297,15 @@
     Notes
     -----
     This is a lazy computation (the result is stored for future calls).
     """
 
     if self._sqD_value is None:
       self._sqD_value = np.sqrt(self.D)
-    return (self._sqD_value)
+    return self._sqD_value
 
   def dotL(self, x, copy=False):
     r"""
     Compute :math:`y = L x`.
 
     Parameters
     ----------
@@ -306,17 +318,28 @@
     -------
     y : (n,) ndarray
       The dot product :math:`y = L x`.
     """
 
     self._x_dotL = self._copy(x, copy)
     y = np.empty_like(x)
-    libspleaf.spleaf_dotL(self.n, self.r, self.offsetrow, self.b, self.U,
-      self.W, self.phi, self.G, x, y, self._f_dotL)
-    return (y)
+    libspleaf.spleaf_dotL(
+      self.n,
+      self.r,
+      self.offsetrow,
+      self.b,
+      self.U,
+      self.W,
+      self.phi,
+      self.G,
+      x,
+      y,
+      self._f_dotL,
+    )
+    return y
 
   def solveL(self, y, copy=False):
     r"""
     Solve for :math:`x = L^{-1} y`.
 
     Parameters
     ----------
@@ -328,17 +351,28 @@
     Returns
     -------
     x : (n,) ndarray
       The solution :math:`x = L^{-1} y`.
     """
 
     self._x_solveL = np.empty_like(y)
-    libspleaf.spleaf_solveL(self.n, self.r, self.offsetrow, self.b, self.U,
-      self.W, self.phi, self.G, y, self._x_solveL, self._f_solveL)
-    return (self._copy(self._x_solveL, copy))
+    libspleaf.spleaf_solveL(
+      self.n,
+      self.r,
+      self.offsetrow,
+      self.b,
+      self.U,
+      self.W,
+      self.phi,
+      self.G,
+      y,
+      self._x_solveL,
+      self._f_solveL,
+    )
+    return self._copy(self._x_solveL, copy)
 
   def dotLT(self, x, copy=False):
     r"""
     Compute :math:`y = L^T x`.
 
     Parameters
     ----------
@@ -351,17 +385,28 @@
     -------
     y : (n,) ndarray
       The dot product :math:`y = L^T x`.
     """
 
     self._x_dotLT = self._copy(x, copy)
     y = np.empty_like(x)
-    libspleaf.spleaf_dotLT(self.n, self.r, self.offsetrow, self.b, self.U,
-      self.W, self.phi, self.G, x, y, self._g_dotLT)
-    return (y)
+    libspleaf.spleaf_dotLT(
+      self.n,
+      self.r,
+      self.offsetrow,
+      self.b,
+      self.U,
+      self.W,
+      self.phi,
+      self.G,
+      x,
+      y,
+      self._g_dotLT,
+    )
+    return y
 
   def solveLT(self, y, copy=False):
     r"""
     Solve for :math:`x = L^{-T} y`.
 
     Parameters
     ----------
@@ -373,17 +418,28 @@
     Returns
     -------
     x : (n,) ndarray
       The solution :math:`x = L^{-T} y`.
     """
 
     self._x_solveLT = np.empty_like(y)
-    libspleaf.spleaf_solveLT(self.n, self.r, self.offsetrow, self.b, self.U,
-      self.W, self.phi, self.G, y, self._x_solveLT, self._g_solveLT)
-    return (self._copy(self._x_solveLT, copy))
+    libspleaf.spleaf_solveLT(
+      self.n,
+      self.r,
+      self.offsetrow,
+      self.b,
+      self.U,
+      self.W,
+      self.phi,
+      self.G,
+      y,
+      self._x_solveLT,
+      self._g_solveLT,
+    )
+    return self._copy(self._x_solveLT, copy)
 
   def init_grad(self):
     r"""
     Initialize (or reinitialize) the backward propagation of the gradient.
     """
 
     self._grad_A = np.zeros_like(self.A)
@@ -406,19 +462,37 @@
     and to the components of :math:`L` (`U`, `W`, `phi`, `G`),
     to its gradient with respect to the initial components of the matrix
     (`A`, `U`, `V`, `phi`, `F`).
 
     Use :func:`grad_param` to get the results.
     """
 
-    libspleaf.spleaf_cholesky_back(self.n, self.r, self.offsetrow, self.b,
-      self.D, self.U, self.W, self.phi, self.G, self._grad_D, self._grad_Ucho,
-      self._grad_W, self._grad_phicho, self._grad_G, self._grad_A,
-      self._grad_U, self._grad_V, self._grad_phi, self._grad_F, self._S,
-      self._Z)
+    libspleaf.spleaf_cholesky_back(
+      self.n,
+      self.r,
+      self.offsetrow,
+      self.b,
+      self.D,
+      self.U,
+      self.W,
+      self.phi,
+      self.G,
+      self._grad_D,
+      self._grad_Ucho,
+      self._grad_W,
+      self._grad_phicho,
+      self._grad_G,
+      self._grad_A,
+      self._grad_U,
+      self._grad_V,
+      self._grad_phi,
+      self._grad_F,
+      self._S,
+      self._Z,
+    )
 
   def dotL_back(self, grad_y):
     r"""
     Backward propagation of the gradient for :func:`dotL`.
 
     Propagate the gradient of a function with respect to `y`,
     to its gradient with respect to `x`
@@ -437,18 +511,33 @@
     Returns
     -------
     grad_x : (n,) ndarray
       Gradient of the function with respect to `x`.
     """
 
     grad_x = np.empty_like(grad_y)
-    libspleaf.spleaf_dotL_back(self.n, self.r, self.offsetrow, self.b, self.U,
-      self.W, self.phi, self.G, self._x_dotL, grad_y, self._grad_Ucho,
-      self._grad_W, self._grad_phicho, self._grad_G, grad_x, self._f_dotL)
-    return (grad_x)
+    libspleaf.spleaf_dotL_back(
+      self.n,
+      self.r,
+      self.offsetrow,
+      self.b,
+      self.U,
+      self.W,
+      self.phi,
+      self.G,
+      self._x_dotL,
+      grad_y,
+      self._grad_Ucho,
+      self._grad_W,
+      self._grad_phicho,
+      self._grad_G,
+      grad_x,
+      self._f_dotL,
+    )
+    return grad_x
 
   def solveL_back(self, grad_x):
     r"""
     Backward propagation of the gradient for :func:`solveL`.
 
     Propagate the gradient of a function with respect to `x`,
     to its gradient with respect to `y`
@@ -467,19 +556,33 @@
     Returns
     -------
     grad_y : (n,) ndarray
       Gradient of the function with respect to `y`.
     """
 
     grad_y = np.empty_like(grad_x)
-    libspleaf.spleaf_solveL_back(self.n, self.r, self.offsetrow, self.b,
-      self.U, self.W, self.phi, self.G, self._x_solveL, grad_x,
-      self._grad_Ucho, self._grad_W, self._grad_phicho, self._grad_G, grad_y,
-      self._f_solveL)
-    return (grad_y)
+    libspleaf.spleaf_solveL_back(
+      self.n,
+      self.r,
+      self.offsetrow,
+      self.b,
+      self.U,
+      self.W,
+      self.phi,
+      self.G,
+      self._x_solveL,
+      grad_x,
+      self._grad_Ucho,
+      self._grad_W,
+      self._grad_phicho,
+      self._grad_G,
+      grad_y,
+      self._f_solveL,
+    )
+    return grad_y
 
   def dotLT_back(self, grad_y):
     r"""
     Backward propagation of the gradient for :func:`dotLT`.
 
     Propagate the gradient of a function with respect to `y`,
     to its gradient with respect to `x`
@@ -498,18 +601,33 @@
     Returns
     -------
     grad_x : (n,) ndarray
       Gradient of the function with respect to `x`.
     """
 
     grad_x = np.empty_like(grad_y)
-    libspleaf.spleaf_dotLT_back(self.n, self.r, self.offsetrow, self.b, self.U,
-      self.W, self.phi, self.G, self._x_dotLT, grad_y, self._grad_Ucho,
-      self._grad_W, self._grad_phicho, self._grad_G, grad_x, self._g_dotLT)
-    return (grad_x)
+    libspleaf.spleaf_dotLT_back(
+      self.n,
+      self.r,
+      self.offsetrow,
+      self.b,
+      self.U,
+      self.W,
+      self.phi,
+      self.G,
+      self._x_dotLT,
+      grad_y,
+      self._grad_Ucho,
+      self._grad_W,
+      self._grad_phicho,
+      self._grad_G,
+      grad_x,
+      self._g_dotLT,
+    )
+    return grad_x
 
   def solveLT_back(self, grad_x):
     r"""
     Backward propagation of the gradient for :func:`solveLT`.
 
     Propagate the gradient of a function with respect to `x`,
     to its gradient with respect to `y`
@@ -528,19 +646,33 @@
     Returns
     -------
     grad_y : (n,) ndarray
       Gradient of the function with respect to `y`.
     """
 
     grad_y = np.empty_like(grad_x)
-    libspleaf.spleaf_solveLT_back(self.n, self.r, self.offsetrow, self.b,
-      self.U, self.W, self.phi, self.G, self._x_solveLT, grad_x,
-      self._grad_Ucho, self._grad_W, self._grad_phicho, self._grad_G, grad_y,
-      self._g_solveLT)
-    return (grad_y)
+    libspleaf.spleaf_solveLT_back(
+      self.n,
+      self.r,
+      self.offsetrow,
+      self.b,
+      self.U,
+      self.W,
+      self.phi,
+      self.G,
+      self._x_solveLT,
+      grad_x,
+      self._grad_Ucho,
+      self._grad_W,
+      self._grad_phicho,
+      self._grad_G,
+      grad_y,
+      self._g_solveLT,
+    )
+    return grad_y
 
   def grad_param(self, *args, **kwargs):
     r"""
     Gradient of a function with respect to
     the initial parameters (`A`, `U`, `V`, `phi`, `F`),
     after a call to :func:`cholesky_back`.
 
@@ -554,16 +686,15 @@
       Gradient of the function with respect to `V`.
     grad_phi : (n-1, r) ndarray
       Gradient of the function with respect to `phi`.
     grad_F : ndarray
       Gradient of the function with respect to `F`.
     """
 
-    return (self._grad_A, self._grad_U, self._grad_V, self._grad_phi,
-      self._grad_F)
+    return (self._grad_A, self._grad_U, self._grad_V, self._grad_phi, self._grad_F)
 
   def chi2(self, y):
     r"""
     Compute :math:`\chi^2 = y^T C^{-1} y`
     for a given vector of residuals :math:`y`.
 
     Parameters
@@ -574,15 +705,15 @@
     Returns
     -------
     chi2 : float
       The :math:`\chi^2`.
     """
 
     x = self.solveL(y)
-    return (np.sum(x * x / self.D))
+    return np.sum(x * x / self.D)
 
   def loglike(self, y):
     r"""
     Compute the (natural) logarithm of the likelihood
     for a given vector of residuals :math:`y`.
 
     Parameters
@@ -592,16 +723,15 @@
 
     Returns
     -------
     loglike : float
       The natural logarithm of the likelihood.
     """
 
-    return (-0.5 *
-      (self.chi2(y) + self.logdet() + self.n * np.log(2.0 * np.pi)))
+    return -0.5 * (self.chi2(y) + self.logdet() + self.n * np.log(2.0 * np.pi))
 
   def chi2_grad(self, *args, **kwargs):
     r"""
     Compute the gradient of the :math:`\chi^2` (:func:`chi2`)
     with respect to the residuals and to the initial parameters
     (see :func:`grad_param`).
 
@@ -685,40 +815,31 @@
 
     if index is None:
       index = np.arange(self.r)
     ri = index.size
 
     u = self.solveLT(self.solveL(y) / self.D)
     y2 = np.empty(self.n)
-    libspleaf.spleaf_dotsep(self.n, self.r, ri, index, self.U, self.V,
-      self.phi, u, y2)
+    libspleaf.spleaf_dotsep(self.n, self.r, ri, index, self.U, self.V, self.phi, u, y2)
 
     if not calc_cov:
-      return (y2)
+      return y2
 
     K = np.empty((self.n, self.n))
-    libspleaf.spleaf_expandsep(self.n, self.r, ri, index, self.U, self.V,
-      self.phi, K)
+    libspleaf.spleaf_expandsep(self.n, self.r, ri, index, self.U, self.V, self.phi, K)
     H = np.array([self.solveL(Kk) / self.sqD() for Kk in K])
 
     if calc_cov == 'diag':
       return (y2, np.diag(K) - np.sum(H * H, axis=1))
 
     return (y2, K - H @ H.T)
 
-  def conditional(self,
-    y,
-    U2,
-    V2,
-    phi2,
-    ref2left,
-    phi2left,
-    phi2right,
-    calc_cov=False,
-    index=None):
+  def conditional(
+    self, y, U2, V2, phi2, ref2left, phi2left, phi2right, calc_cov=False, index=None
+  ):
     r"""
     Conditional mean and covariance at new abscissas
     of the Gaussian process corresponding to the semiseparable part
     of the covariance matrix, knowning the observed values :math:`y`.
 
     Parameters
     ----------
@@ -770,39 +891,64 @@
     if index is None:
       index = np.arange(self.r)
     ri = index.size
 
     u = self.solveLT(self.solveL(y) / self.D)
     n2 = U2.shape[0]
     y2 = np.empty(n2)
-    libspleaf.spleaf_dotsepmixt(self.n, n2, self.r, ri, index, self.U, self.V,
-      self.phi, U2, V2, ref2left, phi2left, phi2right, u, y2)
+    libspleaf.spleaf_dotsepmixt(
+      self.n,
+      n2,
+      self.r,
+      ri,
+      index,
+      self.U,
+      self.V,
+      self.phi,
+      U2,
+      V2,
+      ref2left,
+      phi2left,
+      phi2right,
+      u,
+      y2,
+    )
 
     if not calc_cov:
-      return (y2)
+      return y2
 
     Km = np.empty((n2, self.n))
-    libspleaf.spleaf_expandsepmixt(self.n, n2, self.r, ri, index, self.U,
-      self.V, self.phi, U2, V2, ref2left, phi2left, phi2right, Km)
+    libspleaf.spleaf_expandsepmixt(
+      self.n,
+      n2,
+      self.r,
+      ri,
+      index,
+      self.U,
+      self.V,
+      self.phi,
+      U2,
+      V2,
+      ref2left,
+      phi2left,
+      phi2right,
+      Km,
+    )
     Hm = np.array([self.solveL(Kmk) / self.sqD() for Kmk in Km])
 
     if calc_cov == 'diag':
-      return (y2,
-        np.sum(U2[:, index] * V2[:, index], axis=1) - np.sum(Hm * Hm, axis=1))
+      return (y2, np.sum(U2[:, index] * V2[:, index], axis=1) - np.sum(Hm * Hm, axis=1))
 
     K = np.empty((n2, n2))
     libspleaf.spleaf_expandsep(n2, self.r, ri, index, U2, V2, phi2, K)
     return (y2, K - Hm @ Hm.T)
 
-  def self_conditional_derivative(self,
-    y,
-    dU=None,
-    dV=None,
-    calc_cov=False,
-    index=None):
+  def self_conditional_derivative(
+    self, y, dU=None, dV=None, calc_cov=False, index=None
+  ):
     r"""
     Conditional mean and covariance
     of the derivative of the Gaussian process corresponding to the semiseparable part
     of the covariance matrix, knowning the observed values :math:`y`.
 
     Parameters
     ----------
@@ -849,45 +995,50 @@
       self._dU = dU
     if dV is not None:
       self._dV = dV
 
     u = self.solveLT(self.solveL(y) / self.D)
     dy = np.empty(self.n)
 
-    libspleaf.spleaf_dotantisep(self.n, self.r, ri, index, self._dU, self.V,
-      self.phi, u, dy)
+    libspleaf.spleaf_dotantisep(
+      self.n, self.r, ri, index, self._dU, self.V, self.phi, u, dy
+    )
 
     if not calc_cov:
-      return (dy)
+      return dy
 
     dK = np.empty((self.n, self.n))
     d2K = np.empty((self.n, self.n))
-    libspleaf.spleaf_expandantisep(self.n, self.r, ri, index, self._dU, self.V,
-      self.phi, dK)
-    libspleaf.spleaf_expandsep(self.n, self.r, ri, index, self._dU, self._dV,
-      self.phi, d2K)
+    libspleaf.spleaf_expandantisep(
+      self.n, self.r, ri, index, self._dU, self.V, self.phi, dK
+    )
+    libspleaf.spleaf_expandsep(
+      self.n, self.r, ri, index, self._dU, self._dV, self.phi, d2K
+    )
     H = np.array([self.solveL(dKk) / self.sqD() for dKk in dK])
 
     if calc_cov == 'diag':
       return (dy, np.diag(d2K) - np.sum(H * H, axis=1))
 
     return (dy, d2K - H @ H.T)
 
-  def conditional_derivative(self,
+  def conditional_derivative(
+    self,
     y,
     dU2,
     V2,
     dV2,
     phi2,
     ref2left,
     phi2left,
     phi2right,
     dU=None,
     calc_cov=False,
-    index=None):
+    index=None,
+  ):
     r"""
     Conditional mean and covariance at new abscissas
     of the derivative of the Gaussian process corresponding to the semiseparable part
     of the covariance matrix, knowning the observed values :math:`y`.
 
     Parameters
     ----------
@@ -945,28 +1096,59 @@
 
     if dU is not None:
       self._dU = dU
 
     u = self.solveLT(self.solveL(y) / self.D)
     n2 = dU2.shape[0]
     y2 = np.empty(n2)
-    libspleaf.spleaf_dotsepmixt(self.n, n2, self.r, ri, index, -self._dU,
-      self.V, self.phi, dU2, V2, ref2left, phi2left, phi2right, u, y2)
+    libspleaf.spleaf_dotsepmixt(
+      self.n,
+      n2,
+      self.r,
+      ri,
+      index,
+      -self._dU,
+      self.V,
+      self.phi,
+      dU2,
+      V2,
+      ref2left,
+      phi2left,
+      phi2right,
+      u,
+      y2,
+    )
 
     if not calc_cov:
-      return (y2)
+      return y2
 
     dKm = np.empty((n2, self.n))
-    libspleaf.spleaf_expandsepmixt(self.n, n2, self.r, ri, index, -self._dU,
-      self.V, self.phi, dU2, V2, ref2left, phi2left, phi2right, dKm)
+    libspleaf.spleaf_expandsepmixt(
+      self.n,
+      n2,
+      self.r,
+      ri,
+      index,
+      -self._dU,
+      self.V,
+      self.phi,
+      dU2,
+      V2,
+      ref2left,
+      phi2left,
+      phi2right,
+      dKm,
+    )
     Hm = np.array([self.solveL(dKmk) / self.sqD() for dKmk in dKm])
 
     if calc_cov == 'diag':
-      return (y2, np.sum(dU2[:, index] * dV2[:, index], axis=1) -
-        np.sum(Hm * Hm, axis=1))
+      return (
+        y2,
+        np.sum(dU2[:, index] * dV2[:, index], axis=1) - np.sum(Hm * Hm, axis=1),
+      )
 
     d2K = np.empty((n2, n2))
     libspleaf.spleaf_expandsep(n2, self.r, ri, index, dU2, dV2, phi2, d2K)
     return (y2, d2K - Hm @ Hm.T)
 
   def sample(self, nreal=None):
     r"""
@@ -987,10 +1169,10 @@
     single = False
     if nreal is None:
       single = True
       nreal = 1
     u = np.random.normal(size=(nreal, self.n))
     y = np.array([self.dotL(self.sqD() * uk) for uk in u])
     if single:
-      return (y[0])
+      return y[0]
     else:
-      return (y)
+      return y
```

### Comparing `spleaf-2.1.8/spleaf/cov.py` & `spleaf-2.1.9/src/spleaf/cov.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,18 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2019-2023 Jean-Baptiste Delisle
-#
-# This file is part of spleaf.
-#
-# spleaf is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# spleaf is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with spleaf.  If not, see <http://www.gnu.org/licenses/>.
+# Copyright 2019-2024 Jean-Baptiste Delisle
+# Licensed under the EUPL-1.2 or later
 
 __all__ = ['Cov']
 
 import numpy as np
-from . import Spleaf, libspleaf
-from .term import Noise, Kernel
+
+from . import Spleaf
+from .term import Kernel, Noise
 
 
 def merge_series(list_t, *args):
   r"""
   Merge and sort several time series by increasing time.
 
   Parameters
@@ -49,16 +36,15 @@
   list_n = [tk.size for tk in list_t]
   cum_n = np.insert(np.cumsum(list_n), 0, 0)
   full_t = np.hstack(list_t)
   ksort = np.argsort(full_t, kind='stable')
   full_t = full_t[ksort]
   full_args = [np.hstack(arg)[ksort] for arg in args]
   series_index = [
-    np.where((ksort >= cum_n[k]) & (ksort < cum_n[k + 1]))[0]
-    for k in range(n_series)
+    np.where((ksort >= cum_n[k]) & (ksort < cum_n[k + 1]))[0] for k in range(n_series)
   ]
   return (full_t, *full_args, series_index)
 
 
 class Cov(Spleaf):
   r"""
   Covariance matrix class.
@@ -106,16 +92,15 @@
   def __init__(self, t, **kwargs):
     self.t = t
     if not isinstance(t, np.ndarray):
       raise Exception('Cov: t is not an array.')
     self.n = t.size
     self.dt = t[1:] - t[:-1]
     if np.min(self.dt) < 0:
-      raise Exception('Cov: the timeseries must be provided'
-        ' in increasing order.')
+      raise Exception('Cov: the timeseries must be provided' ' in increasing order.')
 
     # Read kwargs
     self.noise = {}
     self.b = np.zeros(self.n, dtype=int)
     self.kernel = {}
     self.r = 0
     self.term = {}
@@ -127,34 +112,32 @@
         kwargs[key]._link(self)
         self.b = np.maximum(self.b, kwargs[key]._b)
       elif isinstance(kwargs[key], Kernel):
         self.kernel[key] = kwargs[key]
         kwargs[key]._link(self, self.r)
         self.r += kwargs[key]._r
       else:
-        raise Exception(
-          'The provided argument is not of type Noise or Kernel.')
+        raise Exception('The provided argument is not of type Noise or Kernel.')
       self.term[key] = kwargs[key]
       self.param += [f'{key}.{par}' for par in kwargs[key]._param]
       self._param_dict.update(
-        {f'{key}.{par}': (key, par)
-        for par in kwargs[key]._param})
+        {f'{key}.{par}': (key, par) for par in kwargs[key]._param}
+      )
 
     # Compute S+LEAF representation
     self.A = np.zeros(self.n)
     self.U = np.empty((self.n, self.r))
     self.V = np.empty((self.n, self.r))
     self.phi = np.empty((self.n - 1, self.r))
     self.offsetrow = np.cumsum(self.b - 1) + 1
     self.F = np.zeros(np.sum(self.b))
     for key in self.term:
       self.term[key]._compute()
 
-    super().__init__(self.A, self.U, self.V, self.phi, self.offsetrow, self.b,
-      self.F)
+    super().__init__(self.A, self.U, self.V, self.phi, self.offsetrow, self.b, self.F)
 
     # Kernel derivative
     self._dU = np.empty((self.n, self.r))
     self._dV = np.empty((self.n, self.r))
 
   def get_param(self, param=None):
     r"""
@@ -178,15 +161,15 @@
     if isinstance(param, str):
       param = [param]
       single = True
     value = np.empty(len(param))
     for k, keypar in enumerate(param):
       key, par = self._param_dict[keypar]
       value[k] = self.term[key]._get_param(par)
-    return (value[0] if single else value)
+    return value[0] if single else value
 
   def set_param(self, value, param=None):
     r"""
     Set the values of the parameters.
 
     Parameters
     ----------
@@ -244,17 +227,17 @@
     self._sum_grad_A = np.sum(self._grad_A)
     grad = {}
     for key in term:
       grad_key = self.term[key]._grad_param()
       for par in grad_key:
         grad[f'{key}.{par}'] = grad_key[par]
     if single:
-      return (grad[param[0]])
+      return grad[param[0]]
     else:
-      return (np.array([grad[keypar] for keypar in param]))
+      return np.array([grad[keypar] for keypar in param])
 
   def _kernel_index(self, kernel=None):
     r"""
     List of indices corresponding to the requested kernel terms
     in the semiseparable representation of the matrix.
 
     Parameters
@@ -265,22 +248,26 @@
     Returns
     -------
     index : (r',) ndarray
       Indices of the corresponding semiseparable terms.
     """
 
     if kernel is None:
-      return (None)
+      return None
     else:
-      return (np.array([
-        s for key in kernel
-        for s in range(self.kernel[key]._offset, self.kernel[key]._offset +
-        self.kernel[key]._r)
-      ],
-        dtype=int))
+      return np.array(
+        [
+          s
+          for key in kernel
+          for s in range(
+            self.kernel[key]._offset, self.kernel[key]._offset + self.kernel[key]._r
+          )
+        ],
+        dtype=int,
+      )
 
   def self_conditional(self, y, calc_cov=False, kernel=None):
     r"""
     Conditional mean and covariance
     of the kernel part, or a subset of kernel terms,
     knowning the observed values :math:`y`.
 
@@ -314,15 +301,15 @@
     :math:`\mathcal{O}(n)`,
     the computational cost of the variance scales as
     :math:`\mathcal{O}(n^2)`,
     and the computational cost of the full covariance scales as
     :math:`\mathcal{O}(n^3)`.
     """
 
-    return (super().self_conditional(y, calc_cov, self._kernel_index(kernel)))
+    return super().self_conditional(y, calc_cov, self._kernel_index(kernel))
 
   def conditional(self, y, t2, calc_cov=False, kernel=None):
     r"""
     Conditional mean and covariance
     of the kernel part, or a subset of kernel terms,
     at new times :math:`t_2`,
     knowning the observed values :math:`y`.
@@ -362,35 +349,46 @@
     and the computational cost of the full covariance scales as
     :math:`\mathcal{O}(n n_2^2)`.
     """
 
     n2 = t2.size
     dt2 = t2[1:] - t2[:-1]
     if np.min(dt2) < 0:
-      raise Exception('Cov.conditional: the timeseries must be provided'
-        ' in increasing order.')
+      raise Exception(
+        'Cov.conditional: the timeseries must be provided' ' in increasing order.'
+      )
     U2 = np.empty((n2, self.r))
     V2 = np.empty((n2, self.r))
     phi2 = np.empty((n2 - 1, self.r))
     phi2left = np.empty((n2, self.r))
     phi2right = np.empty((n2, self.r))
 
     ref2left = np.searchsorted(self.t, t2) - 1
     dt2left = t2 - self.t[ref2left]
     dt2right = self.t[np.minimum(ref2left + 1, self.n - 1)] - t2
     dt2left[ref2left == -1] = 0  # useless but avoid overflow warning
     dt2right[ref2left == self.n - 1] = 0  # useless but avoid overflow warning
 
     kernel_list = self.kernel if kernel is None else kernel
     for key in kernel_list:
-      self.kernel[key]._compute_t2(t2, dt2, U2, V2, phi2, ref2left, dt2left,
-        dt2right, phi2left, phi2right)
-
-    return (super().conditional(y, U2, V2, phi2, ref2left, phi2left, phi2right,
-      calc_cov, self._kernel_index(kernel)))
+      self.kernel[key]._compute_t2(
+        t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right, phi2left, phi2right
+      )
+
+    return super().conditional(
+      y,
+      U2,
+      V2,
+      phi2,
+      ref2left,
+      phi2left,
+      phi2right,
+      calc_cov,
+      self._kernel_index(kernel),
+    )
 
   def self_conditional_derivative(self, y, calc_cov=False, kernel=None):
     r"""
     Conditional mean and covariance
     of the derivative of the kernel part, or a subset of kernel terms,
     knowning the observed values :math:`y`.
 
@@ -433,17 +431,17 @@
     :math:`\mathcal{O}(n^3)`.
     """
 
     kernel_list = self.kernel if kernel is None else kernel
     for key in kernel_list:
       self.kernel[key]._deriv(calc_cov)
 
-    return (super().self_conditional_derivative(y,
-      calc_cov=calc_cov,
-      index=self._kernel_index(kernel)))
+    return super().self_conditional_derivative(
+      y, calc_cov=calc_cov, index=self._kernel_index(kernel)
+    )
 
   def conditional_derivative(self, y, t2, calc_cov=False, kernel=None):
     r"""
     Conditional mean and covariance
     of the derivative of the kernel part, or a subset of kernel terms,
     at new times :math:`t_2`,
     knowning the observed values :math:`y`.
@@ -488,16 +486,18 @@
     and the computational cost of the full covariance scales as
     :math:`\mathcal{O}(n n_2^2)`.
     """
 
     n2 = t2.size
     dt2 = t2[1:] - t2[:-1]
     if np.min(dt2) < 0:
-      raise Exception('Cov.conditional_derivative: the timeseries must be provided'
-        ' in increasing order.')
+      raise Exception(
+        'Cov.conditional_derivative: the timeseries must be provided'
+        ' in increasing order.'
+      )
     dU2 = np.empty((n2, self.r))
     V2 = np.empty((n2, self.r))
     phi2 = np.empty((n2 - 1, self.r))
     phi2left = np.empty((n2, self.r))
     phi2right = np.empty((n2, self.r))
 
     ref2left = np.searchsorted(self.t, t2) - 1
@@ -510,27 +510,30 @@
       dV2 = np.empty((n2, self.r))
     else:
       dV2 = None
 
     kernel_list = self.kernel if kernel is None else kernel
     for key in kernel_list:
       self.kernel[key]._deriv(False)
-      self.kernel[key]._deriv_t2(t2, dt2, dU2, V2, phi2, ref2left, dt2left,
-        dt2right, phi2left, phi2right, dV2)
+      self.kernel[key]._deriv_t2(
+        t2, dt2, dU2, V2, phi2, ref2left, dt2left, dt2right, phi2left, phi2right, dV2
+      )
 
-    return (super().conditional_derivative(y,
+    return super().conditional_derivative(
+      y,
       dU2,
       V2,
       dV2,
       phi2,
       ref2left,
       phi2left,
       phi2right,
       calc_cov=calc_cov,
-      index=self._kernel_index(kernel)))
+      index=self._kernel_index(kernel),
+    )
 
   def eval(self, dt, kernel=None):
     r"""
     Direct evaluation of the kernel part at lag :math:`\delta t`.
 
     Parameters
     ----------
@@ -549,8 +552,8 @@
     Warnings
     --------
     The cost scales as the size of the lag ndarray.
     """
 
     if kernel is None:
       kernel = self.kernel
-    return (sum(self.kernel[key].eval(dt) for key in kernel))
+    return sum(self.kernel[key].eval(dt) for key in kernel)
```

### Comparing `spleaf-2.1.8/spleaf/fenrir.py` & `spleaf-2.1.9/src/spleaf/fenrir.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,27 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2019-2023 Jean-Baptiste Delisle
-#
-# This file is part of spleaf.
-#
-# spleaf is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# spleaf is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with spleaf.  If not, see <http://www.gnu.org/licenses/>.
+# Copyright 2019-2024 Jean-Baptiste Delisle
+# Licensed under the EUPL-1.2 or later
 
 __all__ = [
-  'SpotsSameLat', 'gaussian_weight', 'symmetric_gaussian_weight',
-  'SpotsLatDist', 'SpotsLatDistMag', 'SpotsLatDistInterpolator',
-  'SpotsLatDistMagInterpolator'
+  'SpotsSameLat',
+  'gaussian_weight',
+  'symmetric_gaussian_weight',
+  'SpotsLatDist',
+  'SpotsLatDistMag',
+  'SpotsLatDistInterpolator',
+  'SpotsLatDistMagInterpolator',
 ]
 
+import pickle
+
 import numpy as np
+
 from . import term
-import pickle
 
 
 class SpotsSameLat:
   r"""
   FENRIR model with spots/faculae appearing randomly on the star
   but always at the same latitude :math:`\delta`.
 
@@ -59,33 +51,34 @@
     self._kpn = k[:, np.newaxis] + n[np.newaxis]
     self._kmn = np.abs(k[:, np.newaxis] - n[np.newaxis])
     self._bar_i = 0
     self._delta = 0
 
   def _rv_cb(self):
     alpha = np.zeros(3)
-    alpha[0] = np.sin(self._bar_i)**2 * np.sin(self._delta)**2 + 0.5 * np.cos(
-      self._bar_i)**2 * np.cos(self._delta)**2  # const
-    alpha[1] = 0.5 * np.sin(2 * self._bar_i) * np.sin(
-      2 * self._delta)  # cosphi
-    alpha[2] = 0.5 * np.cos(self._bar_i)**2 * np.cos(self._delta)**2  # cos2phi
-    return (alpha)
+    alpha[0] = (
+      np.sin(self._bar_i) ** 2 * np.sin(self._delta) ** 2
+      + 0.5 * np.cos(self._bar_i) ** 2 * np.cos(self._delta) ** 2
+    )  # const
+    alpha[1] = 0.5 * np.sin(2 * self._bar_i) * np.sin(2 * self._delta)  # cosphi
+    alpha[2] = 0.5 * np.cos(self._bar_i) ** 2 * np.cos(self._delta) ** 2  # cos2phi
+    return alpha
 
   def _rv_phot(self):
     beta = np.zeros(3)
     # Photometric / cos bar_i/2
     beta[1] = np.sin(self._bar_i) * np.sin(2 * self._delta)  # sinphi
-    beta[2] = np.cos(self._bar_i) * np.cos(self._delta)**2  # sin2phi
-    return (beta)
+    beta[2] = np.cos(self._bar_i) * np.cos(self._delta) ** 2  # sin2phi
+    return beta
 
   def _phot(self):
     alpha = np.zeros(2)
     alpha[0] = np.sin(self._bar_i) * np.sin(self._delta)  # const
     alpha[1] = np.cos(self._bar_i) * np.cos(self._delta)  # cosphi
-    return (alpha)
+    return alpha
 
   def _apply_limb_dark(self, coefs, ld, is_alpha=True):
     degree_ld = len(ld)
     nfreq = coefs.shape[0]
 
     coefs_ld = np.zeros((degree_ld, nfreq + degree_ld - 1))
     coefs_ld[0, :nfreq] = coefs
@@ -99,28 +92,30 @@
       coefs_ld[k, 1:] += hb * coefs_ld[k - 1, :-1]
       if is_alpha:
         coefs_ld[k, 1] += hb * coefs_ld[k - 1, 0]  # Add cos (- omega*t) term
       else:
         coefs_ld[k, 0] = 0
       coefs_ld[k] += a * coefs_ld[k - 1]
 
-    return (np.sum(ld[:, np.newaxis] * coefs_ld, axis=0))
+    return np.sum(ld[:, np.newaxis] * coefs_ld, axis=0)
 
-  def compute_Fourier(self,
+  def compute_Fourier(
+    self,
     sig_rv_phot,
     sig_rv_cb,
     sig_phot,
     a180,
     bar_i,
     delta,
     ld_a1,
     ld_a2,
     br_center=None,
     br_a1=None,
-    br_a2=None):
+    br_a2=None,
+  ):
     r"""
     Compute the Fourier decomposition of the kernel.
 
     Parameters
     ----------
     sig_rv_phot, sig_rv_cb, sig_phot : float
       Amplitudes of the three modeled effects
@@ -172,67 +167,66 @@
 
     # Photometric effect
     alpha_phot = self._apply_limb_dark(self._phot(), ld)
     if self._brightening:
       alpha_phot = self._apply_limb_dark(alpha_phot, br)
 
     ab = np.zeros((2, self._nfreq, 2))
-    ab[0, :, 0] = Scp[:, :alpha_rv_cb.shape[0]] @ alpha_rv_cb
+    ab[0, :, 0] = Scp[:, : alpha_rv_cb.shape[0]] @ alpha_rv_cb
     ab[1, :, 0] = Scm[:, 1:] @ beta_rv_phot[1:]
     ab[0, :, 1] = Scp[:, :-1] @ alpha_phot
 
     # Spot at opposite longitude
     ab[:, ::2] *= 1 + a180
     ab[:, 1::2] *= 1 - a180
 
     # Normalized coefs
     if self._normalized:
-      sig_rv_cb /= np.sqrt(np.sum(ab[0, :, 0]**2))
-      sig_rv_phot /= np.sqrt(np.sum(ab[1, :, 0]**2))
-      sig_phot /= np.sqrt(np.sum(ab[0, :, 1]**2))
+      sig_rv_cb /= np.sqrt(np.sum(ab[0, :, 0] ** 2))
+      sig_rv_phot /= np.sqrt(np.sum(ab[1, :, 0] ** 2))
+      sig_phot /= np.sqrt(np.sum(ab[0, :, 1] ** 2))
 
     ab[0, :, 0] *= sig_rv_cb
     ab[1, :, 0] *= sig_rv_phot
     ab[0, :, 1] *= sig_phot
 
-    return (ab)
+    return ab
 
   def _translate_param(self, **kwargs):
     r"""
     Helper function to perform a change of variables.
     Intended to be used with :class:`spleaf.term.TransformKernel`.
     """
 
-    param = {
-      key: kwargs.pop(key)
-      for key in list(kwargs) if key.startswith('decay_')
-    }
+    param = {key: kwargs.pop(key) for key in list(kwargs) if key.startswith('decay_')}
     param['fourier_P'] = kwargs.pop('P')
 
     ab = self.compute_Fourier(**kwargs)
     param['fourier_alpha'] = ab[0, ..., np.newaxis]
     param['fourier_beta'] = ab[1, ..., np.newaxis]
 
-    return (param)
+    return param
 
-  def kernel(self,
+  def kernel(
+    self,
     series_index,
     decay_kernel,
     P,
     sig_rv_phot,
     sig_rv_cb,
     sig_phot,
     a180,
     bar_i,
     delta,
     ld_a1,
     ld_a2,
     br_center=None,
     br_a1=None,
-    br_a2=None):
+    br_a2=None,
+  ):
     r"""
     Generate a S+LEAF kernel corresponding to this FENRIR model,
     to be included in a covariance matrix (:class:`spleaf.cov.Cov`).
 
     Parameters
     ----------
     series_index : list of ndarrays
@@ -257,39 +251,47 @@
       Brightening coefficients (ignored if the brightening is not activated).
 
     Returns
     -------
     kernel : :class:`spleaf.term.Kernel`
       S+LEAF kernel corresponding to this FENRIR model.
     """
-    kwargs = dict(P=P,
+    kwargs = dict(
+      P=P,
       sig_rv_phot=sig_rv_phot,
       sig_rv_cb=sig_rv_cb,
       sig_phot=sig_phot,
       a180=a180,
       bar_i=bar_i,
       delta=delta,
       ld_a1=ld_a1,
-      ld_a2=ld_a2)
+      ld_a2=ld_a2,
+    )
 
     if self._brightening:
       kwargs.update(dict(br_center=br_center, br_a1=br_a1, br_a2=br_a2))
 
-    kwargs.update({
-      f'decay_{key}': decay_kernel._get_param(key)
-      for key in decay_kernel._param
-    })
-
-    return (term.TransformKernel(
-      term.SimpleProductKernel(decay=decay_kernel,
-      fourier=term.MultiFourierKernel(1,
-      np.zeros((self._nfreq, 2, 1)),
-      np.zeros((self._nfreq, 2, 1)),
-      series_index=series_index,
-      vectorize=True)), self._translate_param, **kwargs))
+    kwargs.update(
+      {f'decay_{key}': decay_kernel._get_param(key) for key in decay_kernel._param}
+    )
+
+    return term.TransformKernel(
+      term.SimpleProductKernel(
+        decay=decay_kernel,
+        fourier=term.MultiFourierKernel(
+          1,
+          np.zeros((self._nfreq, 2, 1)),
+          np.zeros((self._nfreq, 2, 1)),
+          series_index=series_index,
+          vectorize=True,
+        ),
+      ),
+      self._translate_param,
+      **kwargs,
+    )
 
 
 def gaussian_weight(delta, delta_mu, delta_sig):
   r"""
   Gaussian distribution of spots/faculae's latitudes.
 
   Parameters
@@ -305,15 +307,15 @@
   -------
   w : (n,) ndarray
     Weight for each latitude.
   """
   u = (delta - delta_mu) / delta_sig
   ew = -u * u / 2
   ew -= np.max(ew)
-  return (np.exp(ew))
+  return np.exp(ew)
 
 
 def symmetric_gaussian_weight(delta, delta_mu, delta_sig):
   r"""
   Symmetric Gaussian distribution of spots/faculae's latitudes.
 
   Parameters
@@ -326,19 +328,18 @@
     Standard deviation of the distribution.
 
   Returns
   -------
   w : (n,) ndarray
     Weight for each latitude.
   """
-  u = np.array([(delta - delta_mu) / delta_sig,
-    (delta + delta_mu) / delta_sig])
+  u = np.array([(delta - delta_mu) / delta_sig, (delta + delta_mu) / delta_sig])
   ew = -u * u / 2
   ew -= np.max(ew)
-  return (np.sum(np.exp(ew), axis=0))
+  return np.sum(np.exp(ew), axis=0)
 
 
 class SpotsLatDist:
   r"""
   FENRIR model with spots/faculae appearing randomly on the star,
   with the spots' latitude following an arbitrary distribution.
 
@@ -362,26 +363,28 @@
     self._nfreq = nharm + 1
     self._ndelta = ndelta
     self._weight = weight
     self._brightening = brightening
     self._spot = SpotsSameLat(nharm, brightening, normalized=False)
     self._u = (np.arange(ndelta) + 0.5) / (ndelta + 1)
 
-  def compute_Fourier(self,
+  def compute_Fourier(
+    self,
     sig_rv_phot,
     sig_rv_cb,
     sig_phot,
     a180,
     bar_i,
     ld_a1,
     ld_a2,
     br_center=None,
     br_a1=None,
     br_a2=None,
-    **kwargs):
+    **kwargs,
+  ):
     r"""
     Compute the Fourier decomposition of the kernel.
 
     Parameters
     ----------
     sig_rv_phot, sig_rv_cb, sig_phot : float
       Amplitudes of the three modeled effects
@@ -408,84 +411,91 @@
     delta_min = max(bar_i, 0) - np.pi / 2
     delta_max = min(bar_i, 0) + np.pi / 2
     delta = delta_min + self._u * (delta_max - delta_min)
 
     w = self._weight(delta, **kwargs)
     sqw = np.sqrt(w)
 
-    ab_delta = np.array([
-      self._spot.compute_Fourier(sqwk, sqwk, sqwk, a180, bar_i, dk, ld_a1,
-      ld_a2, br_center, br_a1, br_a2) for dk, sqwk in zip(delta, sqw)
-    ])
+    ab_delta = np.array(
+      [
+        self._spot.compute_Fourier(
+          sqwk, sqwk, sqwk, a180, bar_i, dk, ld_a1, ld_a2, br_center, br_a1, br_a2
+        )
+        for dk, sqwk in zip(delta, sqw)
+      ]
+    )
 
     # ab_delta : ndelta x alpha/beta=2 x nfreq x nseries=2
     ab = np.zeros((2, self._nfreq, 2, 2))
     for kharm in range(self._nfreq):
-      T = np.tensordot(ab_delta[:, :, kharm],
-        ab_delta[:, :, kharm],
-        axes=(0, 0))
+      T = np.tensordot(ab_delta[:, :, kharm], ab_delta[:, :, kharm], axes=(0, 0))
       # T: alpha/beta x nseries x alpha/beta x nseries
       Tb = T[::-1, :, ::-1].copy()
       Tb[1] *= -1
       Tb[:, :, 1] *= -1
       Tf = (T + Tb).reshape(4, 4)
       eigval, eigvec = np.linalg.eigh(Tf)
       U = eigvec[:, ::2] * np.sqrt(np.maximum(0, eigval[::2]))
       ik = U[3] != 0
       Uik = U[:, ik]
-      rho = np.sqrt(Uik[1]**2 + Uik[3]**2)
-      U[:, ik] = np.array([(Uik[0] * Uik[1] + Uik[2] * Uik[3]) / rho, rho,
-        (Uik[1] * Uik[2] - Uik[0] * Uik[3]) / rho, 0 * rho])
+      rho = np.sqrt(Uik[1] ** 2 + Uik[3] ** 2)
+      U[:, ik] = np.array(
+        [
+          (Uik[0] * Uik[1] + Uik[2] * Uik[3]) / rho,
+          rho,
+          (Uik[1] * Uik[2] - Uik[0] * Uik[3]) / rho,
+          0 * rho,
+        ]
+      )
       U[:, U[1] < 0] *= -1
-      rho = np.sqrt(np.sum(U[1]**2))
+      rho = np.sqrt(np.sum(U[1] ** 2))
       if rho > 0:
         a = U[1, 0] / rho
         b = U[1, 1] / rho
         U[:, 0], U[:, 1] = a * U[:, 0] + b * U[:, 1], b * U[:, 0] - a * U[:, 1]
       ab[:, kharm] = U.reshape((2, 2, 2))
 
-    ab[0, :, 0] *= sig_rv_cb / np.sqrt(np.sum(ab[0, :, 0]**2))
-    ab[1, :, 0] *= sig_rv_phot / np.sqrt(np.sum(ab[1, :, 0]**2))
-    ab[:, :, 1] *= sig_phot / np.sqrt(np.sum(ab[:, :, 1]**2))
+    ab[0, :, 0] *= sig_rv_cb / np.sqrt(np.sum(ab[0, :, 0] ** 2))
+    ab[1, :, 0] *= sig_rv_phot / np.sqrt(np.sum(ab[1, :, 0] ** 2))
+    ab[:, :, 1] *= sig_phot / np.sqrt(np.sum(ab[:, :, 1] ** 2))
 
-    return (ab)
+    return ab
 
   def _translate_param(self, **kwargs):
     r"""
     Helper function to perform a change of variables.
     Intended to be used with :class:`spleaf.term.TransformKernel`.
     """
 
-    param = {
-      key: kwargs.pop(key)
-      for key in list(kwargs) if key.startswith('decay_')
-    }
+    param = {key: kwargs.pop(key) for key in list(kwargs) if key.startswith('decay_')}
     param['fourier_P'] = kwargs.pop('P')
 
     ab = self.compute_Fourier(**kwargs)
     param['fourier_alpha'] = ab[0]
     param['fourier_beta'] = ab[1]
 
-    return (param)
+    return param
 
-  def kernel(self,
+  def kernel(
+    self,
     series_index,
     decay_kernel,
     P,
     sig_rv_phot,
     sig_rv_cb,
     sig_phot,
     a180,
     bar_i,
     ld_a1,
     ld_a2,
     br_center=None,
     br_a1=None,
     br_a2=None,
-    **kwargs):
+    **kwargs,
+  ):
     r"""
     Generate a S+LEAF kernel corresponding to this FENRIR model,
     to be included in a covariance matrix (:class:`spleaf.cov.Cov`).
 
     Parameters
     ----------
     series_index : list of ndarrays
@@ -511,38 +521,47 @@
 
     Returns
     -------
     kernel : :class:`spleaf.term.Kernel`
       S+LEAF kernel corresponding to this FENRIR model.
     """
     kwargs.update(
-      dict(P=P,
-      sig_rv_phot=sig_rv_phot,
-      sig_rv_cb=sig_rv_cb,
-      sig_phot=sig_phot,
-      a180=a180,
-      bar_i=bar_i,
-      ld_a1=ld_a1,
-      ld_a2=ld_a2))
+      dict(
+        P=P,
+        sig_rv_phot=sig_rv_phot,
+        sig_rv_cb=sig_rv_cb,
+        sig_phot=sig_phot,
+        a180=a180,
+        bar_i=bar_i,
+        ld_a1=ld_a1,
+        ld_a2=ld_a2,
+      )
+    )
 
     if self._brightening:
       kwargs.update(dict(br_center=br_center, br_a1=br_a1, br_a2=br_a2))
 
-    kwargs.update({
-      f'decay_{key}': decay_kernel._get_param(key)
-      for key in decay_kernel._param
-    })
-
-    return (term.TransformKernel(
-      term.SimpleProductKernel(decay=decay_kernel,
-      fourier=term.MultiFourierKernel(1,
-      np.zeros((self._nfreq, 2, 2)),
-      np.zeros((self._nfreq, 2, 2)),
-      series_index=series_index,
-      vectorize=True)), self._translate_param, **kwargs))
+    kwargs.update(
+      {f'decay_{key}': decay_kernel._get_param(key) for key in decay_kernel._param}
+    )
+
+    return term.TransformKernel(
+      term.SimpleProductKernel(
+        decay=decay_kernel,
+        fourier=term.MultiFourierKernel(
+          1,
+          np.zeros((self._nfreq, 2, 2)),
+          np.zeros((self._nfreq, 2, 2)),
+          series_index=series_index,
+          vectorize=True,
+        ),
+      ),
+      self._translate_param,
+      **kwargs,
+    )
 
 
 class SpotsLatDistMag:
   r"""
   FENRIR model with spots/faculae appearing randomly on the star,
   with the spots' latitude following an arbitrary distribution,
   and including the effect of the magnetic cycle.
@@ -558,38 +577,39 @@
   brightening : bool
     Whether or not a brightening effect should be included in the model
     (for faculae or mixtures of faculae and spots).
   normalized : bool
     Whether or not the Fourier decomposition should be normalized.
   """
 
-  def __init__(self, nharm, ndelta, weight, brightening=False,
-    normalized=True):
+  def __init__(self, nharm, ndelta, weight, brightening=False, normalized=True):
     self._nharm = nharm
     self._nfreq = nharm + 1
     self._ndelta = ndelta
     self._weight = weight
     self._brightening = brightening
     self._normalized = normalized
     self._spot = SpotsSameLat(nharm, brightening, normalized=False)
     self._u = (np.arange(ndelta) + 0.5) / (ndelta + 1)
 
-  def compute_Fourier(self,
+  def compute_Fourier(
+    self,
     sig_rv_phot,
     sig_rv_cb,
     sig_phot,
     mag_ratio,
     a180,
     bar_i,
     ld_a1,
     ld_a2,
     br_center=None,
     br_a1=None,
     br_a2=None,
-    **kwargs):
+    **kwargs,
+  ):
     r"""
     Compute the Fourier decomposition of the kernel.
 
     Parameters
     ----------
     sig_rv_phot, sig_rv_cb, sig_phot : float
       Amplitudes of the three modeled effects
@@ -625,84 +645,90 @@
     delta_max = min(bar_i, 0) + np.pi / 2
     delta = delta_min + self._u * (delta_max - delta_min)
 
     w = self._weight(delta, **kwargs)
     w /= np.sum(w)
     sqw = np.sqrt(w)
 
-    ab_delta = np.array([
-      self._spot.compute_Fourier(sqwk, sqwk, sqwk, a180, bar_i, dk, ld_a1,
-      ld_a2, br_center, br_a1, br_a2) for dk, sqwk in zip(delta, sqw)
-    ])
+    ab_delta = np.array(
+      [
+        self._spot.compute_Fourier(
+          sqwk, sqwk, sqwk, a180, bar_i, dk, ld_a1, ld_a2, br_center, br_a1, br_a2
+        )
+        for dk, sqwk in zip(delta, sqw)
+      ]
+    )
     # ab_delta : ndelta x alpha/beta=2 x nfreq x nseries=2
 
-    mag_alpha = mag_ratio * np.sum(sqw[:, np.newaxis] * ab_delta[:, 0, 0],
-      axis=0)
+    mag_alpha = mag_ratio * np.sum(sqw[:, np.newaxis] * ab_delta[:, 0, 0], axis=0)
 
     per_ab = np.zeros((2, self._nfreq, 2, 2))
     for kharm in range(self._nfreq):
-      T = np.tensordot(ab_delta[:, :, kharm],
-        ab_delta[:, :, kharm],
-        axes=(0, 0))
+      T = np.tensordot(ab_delta[:, :, kharm], ab_delta[:, :, kharm], axes=(0, 0))
       # T: alpha/beta x nseries x alpha/beta x nseries
       Tb = T[::-1, :, ::-1].copy()
       Tb[1] *= -1
       Tb[:, :, 1] *= -1
       Tf = (T + Tb).reshape(4, 4)
       eigval, eigvec = np.linalg.eigh(Tf)
       U = eigvec[:, ::2] * np.sqrt(np.maximum(0, eigval[::2]))
       ik = U[3] != 0
       Uik = U[:, ik]
-      rho = np.sqrt(Uik[1]**2 + Uik[3]**2)
-      U[:, ik] = np.array([(Uik[0] * Uik[1] + Uik[2] * Uik[3]) / rho, rho,
-        (Uik[1] * Uik[2] - Uik[0] * Uik[3]) / rho, 0 * rho])
+      rho = np.sqrt(Uik[1] ** 2 + Uik[3] ** 2)
+      U[:, ik] = np.array(
+        [
+          (Uik[0] * Uik[1] + Uik[2] * Uik[3]) / rho,
+          rho,
+          (Uik[1] * Uik[2] - Uik[0] * Uik[3]) / rho,
+          0 * rho,
+        ]
+      )
       U[:, U[1] < 0] *= -1
-      rho = np.sqrt(np.sum(U[1]**2))
+      rho = np.sqrt(np.sum(U[1] ** 2))
       if rho > 0:
         a = U[1, 0] / rho
         b = U[1, 1] / rho
         U[:, 0], U[:, 1] = a * U[:, 0] + b * U[:, 1], b * U[:, 0] - a * U[:, 1]
       per_ab[:, kharm] = U.reshape((2, 2, 2))
 
     if self._normalized:
-      sig_rv_cb /= np.sqrt(np.sum(per_ab[0, :, 0]**2) + mag_alpha[0]**2)
-      sig_rv_phot /= np.sqrt(np.sum(per_ab[1, :, 0]**2))
-      sig_phot /= np.sqrt(np.sum(per_ab[:, :, 1]**2) + mag_alpha[1]**2)
+      sig_rv_cb /= np.sqrt(np.sum(per_ab[0, :, 0] ** 2) + mag_alpha[0] ** 2)
+      sig_rv_phot /= np.sqrt(np.sum(per_ab[1, :, 0] ** 2))
+      sig_phot /= np.sqrt(np.sum(per_ab[:, :, 1] ** 2) + mag_alpha[1] ** 2)
     per_ab[0, :, 0] *= sig_rv_cb
     mag_alpha[0] *= sig_rv_cb
     per_ab[1, :, 0] *= sig_rv_phot
     per_ab[:, :, 1] *= sig_phot
     mag_alpha[1] *= sig_phot
     return (per_ab, np.array([[mag_alpha], [2 * [0]]]))
 
   def _translate_param(self, **kwargs):
     r"""
     Helper function to perform a change of variables.
     Intended to be used with :class:`spleaf.term.TransformKernel`.
     """
     param = {
-      f'per_{key}': kwargs.pop(key)
-      for key in list(kwargs) if key.startswith('decay_')
+      f'per_{key}': kwargs.pop(key) for key in list(kwargs) if key.startswith('decay_')
     }
 
-    param.update({
-      key: kwargs.pop(key)
-      for key in list(kwargs) if key.startswith('mag_decay_')
-    })
+    param.update(
+      {key: kwargs.pop(key) for key in list(kwargs) if key.startswith('mag_decay_')}
+    )
 
     param['per_fourier_P'] = kwargs.pop('P')
 
     per_ab, mag_ab = self.compute_Fourier(**kwargs)
     param['per_fourier_alpha'] = per_ab[0]
     param['per_fourier_beta'] = per_ab[1]
     param['mag_fourier_alpha'] = mag_ab[0]
 
-    return (param)
+    return param
 
-  def kernel(self,
+  def kernel(
+    self,
     series_index,
     decay_kernel,
     mag_decay_kernel,
     P,
     sig_rv_phot,
     sig_rv_cb,
     sig_phot,
@@ -710,15 +736,16 @@
     a180,
     bar_i,
     ld_a1,
     ld_a2,
     br_center=None,
     br_a1=None,
     br_a2=None,
-    **kwargs):
+    **kwargs,
+  ):
     r"""
     Generate a S+LEAF kernel corresponding to this FENRIR model,
     to be included in a covariance matrix (:class:`spleaf.cov.Cov`).
 
     Parameters
     ----------
     series_index : list of ndarrays
@@ -752,50 +779,63 @@
 
     Returns
     -------
     kernel : :class:`spleaf.term.Kernel`
       S+LEAF kernel corresponding to this FENRIR model.
     """
     kwargs.update(
-      dict(P=P,
-      sig_rv_phot=sig_rv_phot,
-      sig_rv_cb=sig_rv_cb,
-      sig_phot=sig_phot,
-      mag_ratio=mag_ratio,
-      a180=a180,
-      bar_i=bar_i,
-      ld_a1=ld_a1,
-      ld_a2=ld_a2))
+      dict(
+        P=P,
+        sig_rv_phot=sig_rv_phot,
+        sig_rv_cb=sig_rv_cb,
+        sig_phot=sig_phot,
+        mag_ratio=mag_ratio,
+        a180=a180,
+        bar_i=bar_i,
+        ld_a1=ld_a1,
+        ld_a2=ld_a2,
+      )
+    )
 
     if self._brightening:
       kwargs.update(dict(br_center=br_center, br_a1=br_a1, br_a2=br_a2))
 
-    kwargs.update({
-      f'decay_{key}': decay_kernel._get_param(key)
-      for key in decay_kernel._param
-    })
-
-    kwargs.update({
-      f'mag_decay_{key}': mag_decay_kernel._get_param(key)
-      for key in mag_decay_kernel._param
-    })
-
-    return (term.TransformKernel(
-      term.SimpleSumKernel(per=term.SimpleProductKernel(decay=decay_kernel,
-      fourier=term.MultiFourierKernel(1,
-      np.zeros((self._nfreq, 2, 2)),
-      np.zeros((self._nfreq, 2, 2)),
-      series_index=series_index,
-      vectorize=True)),
-      mag=term.SimpleProductKernel(decay=mag_decay_kernel,
-      fourier=term.MultiFourierKernel(None,
-      np.zeros((1, 2, 1)),
-      None,
-      series_index=series_index,
-      vectorize=True))), self._translate_param, **kwargs))
+    kwargs.update(
+      {f'decay_{key}': decay_kernel._get_param(key) for key in decay_kernel._param}
+    )
+
+    kwargs.update(
+      {
+        f'mag_decay_{key}': mag_decay_kernel._get_param(key)
+        for key in mag_decay_kernel._param
+      }
+    )
+
+    return term.TransformKernel(
+      term.SimpleSumKernel(
+        per=term.SimpleProductKernel(
+          decay=decay_kernel,
+          fourier=term.MultiFourierKernel(
+            1,
+            np.zeros((self._nfreq, 2, 2)),
+            np.zeros((self._nfreq, 2, 2)),
+            series_index=series_index,
+            vectorize=True,
+          ),
+        ),
+        mag=term.SimpleProductKernel(
+          decay=mag_decay_kernel,
+          fourier=term.MultiFourierKernel(
+            None, np.zeros((1, 2, 1)), None, series_index=series_index, vectorize=True
+          ),
+        ),
+      ),
+      self._translate_param,
+      **kwargs,
+    )
 
 
 class SpotsLatDistInterpolator:
   r"""
   FENRIR model interpolating the results of :class:`SpotsLatDist`,
   to improve computational efficiency.
 
@@ -844,29 +884,31 @@
     spi._nfreq = nharm + 1
     with open(basename + '_grid.pkl', 'wb') as f:
       pickle.dump((spi._grid, spi._nharm), f)
     spi._ndim = len(spi._grid)
     spi._listdim = np.arange(spi._ndim)
     sp = SpotsLatDist(nharm, ndelta, weight, brightening)
     gshape = tuple(spi._grid[key].size for key in spi._grid)
-    spi._ab = np.memmap(basename + '_mmap.dat',
+    spi._ab = np.memmap(
+      basename + '_mmap.dat',
       dtype=float,
       mode='w+',
-      shape=gshape + (2, spi._nfreq, 2, 2))
+      shape=gshape + (2, spi._nfreq, 2, 2),
+    )
     ntot = np.prod(gshape)
     for count, inds in enumerate(np.ndindex(gshape)):
       if count % (ntot // 1000) == 0:
         print(f'\r{count/ntot*100:.1f}%', end=' ')
       kwargs = {key: spi._grid[key][ik] for key, ik in zip(spi._grid, inds)}
       kwargs.update(fixed)
       spi._ab[inds] = sp.compute_Fourier(1, 1, 1, 0, **kwargs)
     spi._ab.flush()
     print('\r100%')
     print('done')
-    return (spi)
+    return spi
 
   @staticmethod
   def load(basename):
     r"""
     Load a previously computed grid.
 
     Parameters
@@ -877,19 +919,21 @@
     spi = SpotsLatDistInterpolator()
     with open(basename + '_grid.pkl', 'rb') as f:
       spi._grid, spi._nharm = pickle.load(f)
     spi._nfreq = spi._nharm + 1
     spi._ndim = len(spi._grid)
     spi._listdim = np.arange(spi._ndim)
     gshape = tuple(g.size for g in spi._grid.values())
-    spi._ab = np.memmap(basename + '_mmap.dat',
+    spi._ab = np.memmap(
+      basename + '_mmap.dat',
       dtype=float,
       mode='r',
-      shape=gshape + (2, spi._nfreq, 2, 2))
-    return (spi)
+      shape=gshape + (2, spi._nfreq, 2, 2),
+    )
+    return spi
 
   def compute_Fourier(self, sig_rv_phot, sig_rv_cb, sig_phot, a180, **kwargs):
     r"""
     Compute the Fourier decomposition of the kernel.
 
     Parameters
     ----------
@@ -905,156 +949,171 @@
     Returns
     -------
     ab : (2, nharm + 1, 2, 2) ndarray
       Fourier coefficients, ordered such as ab[0, 2, 0] and ab[0, 2, 1]
       are the cosine coefficients of the second harmonics of the RV and photometric
       timeseries respectively, while ab[1] are the sine coefficients.
     """
-    self._params = dict(sig_rv_phot=sig_rv_phot,
-      sig_rv_cb=sig_rv_cb,
-      sig_phot=sig_phot,
-      a180=a180)
+    self._params = dict(
+      sig_rv_phot=sig_rv_phot, sig_rv_cb=sig_rv_cb, sig_phot=sig_phot, a180=a180
+    )
     self._params.update(kwargs)
     self._inds = [
       max(
-      1,
-      min(self._grid[key].size - 1,
-      np.searchsorted(self._grid[key], kwargs[key], 'right')))
+        1,
+        min(
+          self._grid[key].size - 1,
+          np.searchsorted(self._grid[key], kwargs[key], 'right'),
+        ),
+      )
       for key in self._grid
     ]
     self._w = np.ones(self._ndim * [2])
     for k, key in enumerate(self._grid):
       g = self._grid[key]
       i = self._inds[k]
       x = kwargs[key]
-      self._w[k * (slice(None), ) + (0, )] *= g[i] - x
-      self._w[k * (slice(None), ) + (1, )] *= x - g[i - 1]
-    self._unscaled_ab = np.tensordot(self._ab[tuple(
-      slice(i - 1, i + 1) for i in self._inds)],
+      self._w[k * (slice(None),) + (0,)] *= g[i] - x
+      self._w[k * (slice(None),) + (1,)] *= x - g[i - 1]
+    self._unscaled_ab = np.tensordot(
+      self._ab[tuple(slice(i - 1, i + 1) for i in self._inds)],
       self._w,
-      axes=(self._listdim, self._listdim))
+      axes=(self._listdim, self._listdim),
+    )
     # Spot at opposite longitude
     self._unscaled_ab_180 = self._unscaled_ab.copy()
     self._unscaled_ab_180[:, ::2] *= 1 + a180
     self._unscaled_ab_180[:, 1::2] *= 1 - a180
     # Scaling
     self._scaled_ab = self._unscaled_ab_180.copy()
-    self._scaled_ab[0, :,
-      0] *= sig_rv_cb / np.sqrt(np.sum(self._scaled_ab[0, :, 0]**2))
-    self._scaled_ab[1, :,
-      0] *= sig_rv_phot / np.sqrt(np.sum(self._scaled_ab[1, :, 0]**2))
-    self._scaled_ab[:, :,
-      1] *= sig_phot / np.sqrt(np.sum(self._scaled_ab[:, :, 1]**2))
-    return (self._scaled_ab)
+    self._scaled_ab[0, :, 0] *= sig_rv_cb / np.sqrt(
+      np.sum(self._scaled_ab[0, :, 0] ** 2)
+    )
+    self._scaled_ab[1, :, 0] *= sig_rv_phot / np.sqrt(
+      np.sum(self._scaled_ab[1, :, 0] ** 2)
+    )
+    self._scaled_ab[:, :, 1] *= sig_phot / np.sqrt(
+      np.sum(self._scaled_ab[:, :, 1] ** 2)
+    )
+    return self._scaled_ab
 
   def compute_Fourier_back(self, grad):
     r"""
     Backward propagation of the gradient for :func:`compute_Fourier`.
     """
     grad_params = dict()
 
     # Scaling
     # self._scaled_ab = self._unscaled_ab_180.copy()
     # self._scaled_ab[0, :,
     #   0] *= sig_rv_cb / np.sqrt(np.sum(self._scaled_ab[0, :, 0]**2))
     cgradc = np.sum(self._scaled_ab[0, :, 0] * grad[0, :, 0])
     grad_params['sig_rv_cb'] = cgradc / self._params['sig_rv_cb']
-    s = np.sqrt(np.sum(self._unscaled_ab_180[0, :, 0]**2))
+    s = np.sqrt(np.sum(self._unscaled_ab_180[0, :, 0] ** 2))
     grad_s = -cgradc / s
     grad[0, :, 0] *= self._params['sig_rv_cb'] / s
     grad[0, :, 0] += self._unscaled_ab_180[0, :, 0] * grad_s / s
 
     # self._scaled_ab[1, :,
     #   0] *= sig_rv_phot / np.sqrt(np.sum(self._scaled_ab[1, :, 0]**2))
     cgradc = np.sum(self._scaled_ab[1, :, 0] * grad[1, :, 0])
     grad_params['sig_rv_phot'] = cgradc / self._params['sig_rv_phot']
-    s = np.sqrt(np.sum(self._unscaled_ab_180[1, :, 0]**2))
+    s = np.sqrt(np.sum(self._unscaled_ab_180[1, :, 0] ** 2))
     grad_s = -cgradc / s
     grad[1, :, 0] *= self._params['sig_rv_phot'] / s
     grad[1, :, 0] += self._unscaled_ab_180[1, :, 0] * grad_s / s
 
     # self._scaled_ab[:, :,
     #   1] *= sig_phot / np.sqrt(np.sum(self._scaled_ab[:, :, 1]**2))
     cgradc = np.sum(self._scaled_ab[:, :, 1] * grad[:, :, 1])
     grad_params['sig_phot'] = cgradc / self._params['sig_phot']
-    s = np.sqrt(np.sum(self._unscaled_ab_180[:, :, 1]**2))
+    s = np.sqrt(np.sum(self._unscaled_ab_180[:, :, 1] ** 2))
     grad_s = -cgradc / s
     grad[:, :, 1] *= self._params['sig_phot'] / s
     grad[:, :, 1] += self._unscaled_ab_180[:, :, 1] * grad_s / s
 
     # Spot at opposite longitude
     # self._unscaled_ab_180 = self._unscaled_ab.copy()
     # self._unscaled_ab_180[:, ::2] *= 1 + a180
     # self._unscaled_ab_180[:, 1::2] *= 1 - a180
-    grad_params['a180'] = np.sum(self._unscaled_ab[:, ::2] *
-      grad[:, ::2]) - np.sum(self._unscaled_ab[:, 1::2] * grad[:, 1::2])
+    grad_params['a180'] = np.sum(self._unscaled_ab[:, ::2] * grad[:, ::2]) - np.sum(
+      self._unscaled_ab[:, 1::2] * grad[:, 1::2]
+    )
     grad[:, ::2] *= 1 + self._params['a180']
     grad[:, 1::2] *= 1 - self._params['a180']
 
     # self._unscaled_ab = np.tensordot(self._ab[tuple(
     #   slice(i - 1, i + 1) for i in self._inds)],
     #   self._w,
     #   axes=(self._listdim, self._listdim))
-    grad_w = np.tensordot(grad,
+    grad_w = np.tensordot(
+      grad,
       self._ab[tuple(slice(i - 1, i + 1) for i in self._inds)],
-      axes=([0, 1, 2, 3], [-4, -3, -2, -1]))
+      axes=([0, 1, 2, 3], [-4, -3, -2, -1]),
+    )
     # self._w = np.ones(self._ndim * [2])
     # for k, key in enumerate(self._grid):
     #   g = self._grid[key]
     #   i = self._inds[k]
     #   x = kwargs[key]
     #   self._w[k * (slice(None), ) + (0, )] *= g[i] - x
     #   self._w[k * (slice(None), ) + (1, )] *= x - g[i - 1]
     for k, key in enumerate(self._grid):
       dw = np.ones(self._ndim * [2])
-      dw[k * (slice(None), ) + (0, )] = -1
+      dw[k * (slice(None),) + (0,)] = -1
       for l, ley in enumerate(self._grid):
         if l == k:
           continue
         g = self._grid[ley]
         i = self._inds[l]
         x = self._params[ley]
-        dw[l * (slice(None), ) + (0, )] *= g[i] - x
-        dw[l * (slice(None), ) + (1, )] *= x - g[i - 1]
+        dw[l * (slice(None),) + (0,)] *= g[i] - x
+        dw[l * (slice(None),) + (1,)] *= x - g[i - 1]
       grad_params[key] = np.sum(grad_w * dw)
 
-    return (grad_params)
+    return grad_params
 
   def _translate_param(self, **kwargs):
     r"""
     Helper function to perform a change of variables.
     Intended to be used with :class:`spleaf.term.TransformKernel`.
     """
-    param = {
-      key: kwargs.pop(key)
-      for key in list(kwargs) if key.startswith('decay_')
-    }
+    param = {key: kwargs.pop(key) for key in list(kwargs) if key.startswith('decay_')}
     param['fourier_P'] = kwargs.pop('P')
 
     ab = self.compute_Fourier(**kwargs)
     param['fourier_alpha'] = ab[0]
     param['fourier_beta'] = ab[1]
 
-    return (param)
+    return param
 
   def _translate_param_back(self, grad):
     r"""
     Backward propagation of the gradient for :func:`_translate_param`.
     """
     grad_param = grad.copy()
     grad_param['P'] = grad_param.pop('fourier_P')
     grad_ab = np.array(
-      [grad_param.pop('fourier_alpha'),
-      grad_param.pop('fourier_beta')])
+      [grad_param.pop('fourier_alpha'), grad_param.pop('fourier_beta')]
+    )
     grad_param.update(self.compute_Fourier_back(grad_ab))
 
-    return (grad_param)
+    return grad_param
 
-  def kernel(self, series_index, decay_kernel, P, sig_rv_phot, sig_rv_cb,
-    sig_phot, a180, **kwargs):
+  def kernel(
+    self,
+    series_index,
+    decay_kernel,
+    P,
+    sig_rv_phot,
+    sig_rv_cb,
+    sig_phot,
+    a180,
+    **kwargs,
+  ):
     r"""
     Generate a S+LEAF kernel corresponding to this FENRIR model,
     to be included in a covariance matrix (:class:`spleaf.cov.Cov`).
 
     Parameters
     ----------
     series_index : list of ndarrays
@@ -1074,33 +1133,38 @@
 
     Returns
     -------
     kernel : :class:`spleaf.term.Kernel`
       S+LEAF kernel corresponding to this FENRIR model.
     """
     kwargs.update(
-      dict(P=P,
-      sig_rv_phot=sig_rv_phot,
-      sig_rv_cb=sig_rv_cb,
-      sig_phot=sig_phot,
-      a180=a180))
+      dict(
+        P=P, sig_rv_phot=sig_rv_phot, sig_rv_cb=sig_rv_cb, sig_phot=sig_phot, a180=a180
+      )
+    )
+
+    kwargs.update(
+      {f'decay_{key}': decay_kernel._get_param(key) for key in decay_kernel._param}
+    )
 
-    kwargs.update({
-      f'decay_{key}': decay_kernel._get_param(key)
-      for key in decay_kernel._param
-    })
-
-    return (term.TransformKernel(
-      term.SimpleProductKernel(decay=decay_kernel,
-      fourier=term.MultiFourierKernel(1,
-      np.zeros((self._nfreq, 2, 2)),
-      np.zeros((self._nfreq, 2, 2)),
-      series_index=series_index,
-      vectorize=True)), self._translate_param, self._translate_param_back,
-      **kwargs))
+    return term.TransformKernel(
+      term.SimpleProductKernel(
+        decay=decay_kernel,
+        fourier=term.MultiFourierKernel(
+          1,
+          np.zeros((self._nfreq, 2, 2)),
+          np.zeros((self._nfreq, 2, 2)),
+          series_index=series_index,
+          vectorize=True,
+        ),
+      ),
+      self._translate_param,
+      self._translate_param_back,
+      **kwargs,
+    )
 
 
 class SpotsLatDistMagInterpolator:
   r"""
   FENRIR model interpolating the results of :class:`SpotsLatDistMag`,
   to improve computational efficiency.
 
@@ -1150,35 +1214,36 @@
     spi._nfreq = nharm + 1
     with open(basename + '_grid.pkl', 'wb') as f:
       pickle.dump((spi._grid, spi._nharm), f)
     spi._ndim = len(spi._grid)
     spi._listdim = np.arange(spi._ndim)
     sp = SpotsLatDistMag(nharm, ndelta, weight, brightening, normalized=False)
     gshape = tuple(spi._grid[key].size for key in spi._grid)
-    spi._per_ab = np.memmap(basename + '_per_mmap.dat',
-      dtype=float,
-      mode='w+',
-      shape=gshape + (2, spi._nfreq, 2, 2))
-    spi._mag_alpha = np.memmap(basename + '_mag_mmap.dat',
+    spi._per_ab = np.memmap(
+      basename + '_per_mmap.dat',
       dtype=float,
       mode='w+',
-      shape=gshape + (2, ))
+      shape=gshape + (2, spi._nfreq, 2, 2),
+    )
+    spi._mag_alpha = np.memmap(
+      basename + '_mag_mmap.dat', dtype=float, mode='w+', shape=gshape + (2,)
+    )
     ntot = np.prod(gshape)
     for count, inds in enumerate(np.ndindex(gshape)):
       if count % (ntot // 1000) == 0:
         print(f'\r{count/ntot*100:.1f}%', end=' ')
       kwargs = {key: spi._grid[key][ik] for key, ik in zip(spi._grid, inds)}
       kwargs.update(fixed)
       spi._per_ab[inds], mc = sp.compute_Fourier(1, 1, 1, 1, 0, **kwargs)
       spi._mag_alpha[inds] = mc[0, 0]
     spi._per_ab.flush()
     spi._mag_alpha.flush()
     print('\r100%')
     print('done')
-    return (spi)
+    return spi
 
   @staticmethod
   def load(basename):
     r"""
     Load a previously computed grid.
 
     Parameters
@@ -1189,26 +1254,28 @@
     spi = SpotsLatDistMagInterpolator()
     with open(basename + '_grid.pkl', 'rb') as f:
       spi._grid, spi._nharm = pickle.load(f)
     spi._nfreq = spi._nharm + 1
     spi._ndim = len(spi._grid)
     spi._listdim = np.arange(spi._ndim)
     gshape = tuple(g.size for g in spi._grid.values())
-    spi._per_ab = np.memmap(basename + '_per_mmap.dat',
+    spi._per_ab = np.memmap(
+      basename + '_per_mmap.dat',
       dtype=float,
       mode='r',
-      shape=gshape + (2, spi._nfreq, 2, 2))
-    spi._mag_alpha = np.memmap(basename + '_mag_mmap.dat',
-      dtype=float,
-      mode='r',
-      shape=gshape + (2, ))
-    return (spi)
+      shape=gshape + (2, spi._nfreq, 2, 2),
+    )
+    spi._mag_alpha = np.memmap(
+      basename + '_mag_mmap.dat', dtype=float, mode='r', shape=gshape + (2,)
+    )
+    return spi
 
   def compute_Fourier(
-      self, sig_rv_phot, sig_rv_cb, sig_phot, mag_ratio, a180, **kwargs):
+    self, sig_rv_phot, sig_rv_cb, sig_phot, mag_ratio, a180, **kwargs
+  ):
     r"""
     Compute the Fourier decomposition of the kernel.
 
     Parameters
     ----------
     sig_rv_phot, sig_rv_cb, sig_phot : float
       Amplitudes of the three modeled effects
@@ -1228,68 +1295,80 @@
       Fourier coefficients for the rotation period related effects,
       ordered such as ab[0, 2, 0] and ab[0, 2, 1]
       are the cosine coefficients of the second harmonics of the RV and photometric
       timeseries respectively, while ab[1] are the sine coefficients.
     mag_ab : (2, 1, 2, 1) ndarray
       Fourier coefficients for the magnetic cycle related effects.
     """
-    self._params = dict(sig_rv_phot=sig_rv_phot,
+    self._params = dict(
+      sig_rv_phot=sig_rv_phot,
       sig_rv_cb=sig_rv_cb,
       sig_phot=sig_phot,
       mag_ratio=mag_ratio,
-      a180=a180)
+      a180=a180,
+    )
     self._params.update(kwargs)
     self._inds = [
       max(
-      1,
-      min(self._grid[key].size - 1,
-      np.searchsorted(self._grid[key], kwargs[key], 'right')))
+        1,
+        min(
+          self._grid[key].size - 1,
+          np.searchsorted(self._grid[key], kwargs[key], 'right'),
+        ),
+      )
       for key in self._grid
     ]
     self._w = np.ones(self._ndim * [2])
     for k, key in enumerate(self._grid):
       g = self._grid[key]
       i = self._inds[k]
       x = kwargs[key]
-      self._w[k * (slice(None), ) + (0, )] *= g[i] - x
-      self._w[k * (slice(None), ) + (1, )] *= x - g[i - 1]
-    self._unscaled_per_ab = np.tensordot(self._per_ab[tuple(
-      slice(i - 1, i + 1) for i in self._inds)],
+      self._w[k * (slice(None),) + (0,)] *= g[i] - x
+      self._w[k * (slice(None),) + (1,)] *= x - g[i - 1]
+    self._unscaled_per_ab = np.tensordot(
+      self._per_ab[tuple(slice(i - 1, i + 1) for i in self._inds)],
       self._w,
-      axes=(self._listdim, self._listdim))
-    self._unscaled_mag_alpha = np.tensordot(self._mag_alpha[tuple(
-      slice(i - 1, i + 1) for i in self._inds)],
+      axes=(self._listdim, self._listdim),
+    )
+    self._unscaled_mag_alpha = np.tensordot(
+      self._mag_alpha[tuple(slice(i - 1, i + 1) for i in self._inds)],
       self._w,
-      axes=(self._listdim, self._listdim))
+      axes=(self._listdim, self._listdim),
+    )
     # Spot at opposite longitude
     self._unscaled_per_ab_180 = self._unscaled_per_ab.copy()
     self._unscaled_mag_alpha_180 = self._unscaled_mag_alpha.copy()
     self._unscaled_per_ab_180[:, ::2] *= 1 + a180
     self._unscaled_per_ab_180[:, 1::2] *= 1 - a180
     self._unscaled_mag_alpha_180 *= mag_ratio * (1 + a180)
 
     # Scaling
     self._scaled_per_ab = self._unscaled_per_ab_180.copy()
     self._scaled_mag_alpha = self._unscaled_mag_alpha_180.copy()
 
     scale_cb = sig_rv_cb / np.sqrt(
-      np.sum(self._scaled_per_ab[0, :, 0]**2) + self._scaled_mag_alpha[0]**2)
+      np.sum(self._scaled_per_ab[0, :, 0] ** 2) + self._scaled_mag_alpha[0] ** 2
+    )
     self._scaled_per_ab[0, :, 0] *= scale_cb
     self._scaled_mag_alpha[0] *= scale_cb
 
-    self._scaled_per_ab[1, :,
-      0] *= sig_rv_phot / np.sqrt(np.sum(self._scaled_per_ab[1, :, 0]**2))
+    self._scaled_per_ab[1, :, 0] *= sig_rv_phot / np.sqrt(
+      np.sum(self._scaled_per_ab[1, :, 0] ** 2)
+    )
 
     scale_phot = sig_phot / np.sqrt(
-      np.sum(self._scaled_per_ab[:, :, 1]**2) + self._scaled_mag_alpha[1]**2)
+      np.sum(self._scaled_per_ab[:, :, 1] ** 2) + self._scaled_mag_alpha[1] ** 2
+    )
     self._scaled_per_ab[:, :, 1] *= scale_phot
     self._scaled_mag_alpha[1] *= scale_phot
 
-    return (self._scaled_per_ab, np.array([[self._scaled_mag_alpha],
-      [2 * [0]]])[..., np.newaxis])
+    return (
+      self._scaled_per_ab,
+      np.array([[self._scaled_mag_alpha], [2 * [0]]])[..., np.newaxis],
+    )
 
   def compute_Fourier_back(self, grad_per, grad_mag):
     r"""
     Backward propagation of the gradient for :func:`compute_Fourier`.
     """
     grad_params = dict()
 
@@ -1300,147 +1379,170 @@
     # self._scaled_mag_alpha = self._unscaled_mag_alpha_180.copy()
 
     # scale_cb = sig_rv_cb / np.sqrt(
     #   np.sum(self._scaled_per_ab[0, :, 0]**2) +
     #   self._scaled_mag_alpha[0]**2)
     # self._scaled_per_ab[0, :, 0] *= scale_cb
     # self._scaled_mag_alpha[0] *= scale_cb
-    cgradc = np.sum(self._scaled_per_ab[0, :, 0] *
-      grad_per[0, :, 0]) + self._scaled_mag_alpha[0] * grad_mag[0]
+    cgradc = (
+      np.sum(self._scaled_per_ab[0, :, 0] * grad_per[0, :, 0])
+      + self._scaled_mag_alpha[0] * grad_mag[0]
+    )
     grad_params['sig_rv_cb'] = cgradc / self._params['sig_rv_cb']
     s = np.sqrt(
-      np.sum(self._unscaled_per_ab_180[0, :, 0]**2) +
-      self._unscaled_mag_alpha_180[0]**2)
+      np.sum(self._unscaled_per_ab_180[0, :, 0] ** 2)
+      + self._unscaled_mag_alpha_180[0] ** 2
+    )
     grad_s = -cgradc / s
     grad_per[0, :, 0] *= self._params['sig_rv_cb'] / s
     grad_per[0, :, 0] += self._unscaled_per_ab_180[0, :, 0] * grad_s / s
     grad_mag[0] *= self._params['sig_rv_cb'] / s
     grad_mag[0] += self._unscaled_mag_alpha_180[0] * grad_s / s
 
     # self._scaled_per_ab[1, :,
     #   0] *= sig_rv_phot / np.sqrt(np.sum(self._scaled_per_ab[1, :, 0]**2))
     cgradc = np.sum(self._scaled_per_ab[1, :, 0] * grad_per[1, :, 0])
     grad_params['sig_rv_phot'] = cgradc / self._params['sig_rv_phot']
-    s = np.sqrt(np.sum(self._unscaled_per_ab_180[1, :, 0]**2))
+    s = np.sqrt(np.sum(self._unscaled_per_ab_180[1, :, 0] ** 2))
     grad_s = -cgradc / s
     grad_per[1, :, 0] *= self._params['sig_rv_phot'] / s
     grad_per[1, :, 0] += self._unscaled_per_ab_180[1, :, 0] * grad_s / s
 
     # scale_phot = sig_phot / np.sqrt(
     #   np.sum(self._scaled_per_ab[:,:,1]**2) + self._scaled_mag_alpha[1]**2)
     # self._scaled_per_ab[:,:,1] *= scale_phot
     # self._scaled_mag_alpha[1] *= scale_phot
-    cgradc = np.sum(self._scaled_per_ab[:, :, 1] *
-      grad_per[:, :, 1]) + self._scaled_mag_alpha[1] * grad_mag[1]
+    cgradc = (
+      np.sum(self._scaled_per_ab[:, :, 1] * grad_per[:, :, 1])
+      + self._scaled_mag_alpha[1] * grad_mag[1]
+    )
     grad_params['sig_phot'] = cgradc / self._params['sig_phot']
     s = np.sqrt(
-      np.sum(self._unscaled_per_ab_180[:, :, 1]**2) +
-      self._unscaled_mag_alpha_180[1]**2)
+      np.sum(self._unscaled_per_ab_180[:, :, 1] ** 2)
+      + self._unscaled_mag_alpha_180[1] ** 2
+    )
     grad_s = -cgradc / s
     grad_per[:, :, 1] *= self._params['sig_phot'] / s
     grad_per[:, :, 1] += self._unscaled_per_ab_180[:, :, 1] * grad_s / s
     grad_mag[1] *= self._params['sig_phot'] / s
     grad_mag[1] += self._unscaled_mag_alpha_180[1] * grad_s / s
 
     # Spot at opposite longitude
     # self._unscaled_per_ab_180 = self._unscaled_per_ab.copy()
     # self._unscaled_mag_alpha_180 = self._unscaled_mag_alpha.copy()
     # self._unscaled_per_ab_180[:, ::2] *= 1 + a180
     # self._unscaled_per_ab_180[:, 1::2] *= 1 - a180
     # self._unscaled_mag_alpha_180 *= mag_ratio * (1 + a180)
     smag = np.sum(self._unscaled_mag_alpha * grad_mag)
-    grad_params['a180'] = np.sum(self._unscaled_per_ab[:, ::2] *
-      grad_per[:, ::2]) + self._params['mag_ratio'] * smag - np.sum(
-      self._unscaled_per_ab[:, 1::2] * grad_per[:, 1::2])
+    grad_params['a180'] = (
+      np.sum(self._unscaled_per_ab[:, ::2] * grad_per[:, ::2])
+      + self._params['mag_ratio'] * smag
+      - np.sum(self._unscaled_per_ab[:, 1::2] * grad_per[:, 1::2])
+    )
     grad_params['mag_ratio'] = (1 + self._params['a180']) * smag
     grad_per[:, ::2] *= 1 + self._params['a180']
     grad_per[:, 1::2] *= 1 - self._params['a180']
     grad_mag *= self._params['mag_ratio'] * (1 + self._params['a180'])
 
     # self._unscaled_per_ab = np.tensordot(self._per_ab[tuple(
     #   slice(i - 1, i + 1) for i in self._inds)],
     #   self._w,
     #   axes=(self._listdim, self._listdim))
     # self._unscaled_mag_alpha = np.tensordot(self._mag_alpha[tuple(
     #   slice(i - 1, i + 1) for i in self._inds)],
     #   self._w,
     #   axes=(self._listdim, self._listdim))
-    grad_w = np.tensordot(grad_per,
+    grad_w = np.tensordot(
+      grad_per,
       self._per_ab[tuple(slice(i - 1, i + 1) for i in self._inds)],
-      axes=([0, 1, 2, 3], [-4, -3, -2, -1])) + np.tensordot(grad_mag,
+      axes=([0, 1, 2, 3], [-4, -3, -2, -1]),
+    ) + np.tensordot(
+      grad_mag,
       self._mag_alpha[tuple(slice(i - 1, i + 1) for i in self._inds)],
-      axes=(0, -1))
+      axes=(0, -1),
+    )
 
     # self._w = np.ones(self._ndim * [2])
     # for k, key in enumerate(self._grid):
     #   g = self._grid[key]
     #   i = self._inds[k]
     #   x = kwargs[key]
     #   self._w[k * (slice(None), ) + (0, )] *= g[i] - x
     #   self._w[k * (slice(None), ) + (1, )] *= x - g[i - 1]
     for k, key in enumerate(self._grid):
       dw = np.ones(self._ndim * [2])
-      dw[k * (slice(None), ) + (0, )] = -1
+      dw[k * (slice(None),) + (0,)] = -1
       for l, ley in enumerate(self._grid):
         if l == k:
           continue
         g = self._grid[ley]
         i = self._inds[l]
         x = self._params[ley]
-        dw[l * (slice(None), ) + (0, )] *= g[i] - x
-        dw[l * (slice(None), ) + (1, )] *= x - g[i - 1]
+        dw[l * (slice(None),) + (0,)] *= g[i] - x
+        dw[l * (slice(None),) + (1,)] *= x - g[i - 1]
       grad_params[key] = np.sum(grad_w * dw)
 
-    return (grad_params)
+    return grad_params
 
   def _translate_param(self, **kwargs):
     r"""
     Helper function to perform a change of variables.
     Intended to be used with :class:`spleaf.term.TransformKernel`.
     """
     param = {
-      f'per_{key}': kwargs.pop(key)
-      for key in list(kwargs) if key.startswith('decay_')
+      f'per_{key}': kwargs.pop(key) for key in list(kwargs) if key.startswith('decay_')
     }
 
-    param.update({
-      key: kwargs.pop(key)
-      for key in list(kwargs) if key.startswith('mag_decay_')
-    })
+    param.update(
+      {key: kwargs.pop(key) for key in list(kwargs) if key.startswith('mag_decay_')}
+    )
 
     param['per_fourier_P'] = kwargs.pop('P')
 
     per_ab, mag_ab = self.compute_Fourier(**kwargs)
     param['per_fourier_alpha'] = per_ab[0]
     param['per_fourier_beta'] = per_ab[1]
     param['mag_fourier_alpha'] = mag_ab[0]
 
-    return (param)
+    return param
 
   def _translate_param_back(self, grad):
     r"""
     Backward propagation of the gradient for :func:`_translate_param`.
     """
     grad_param = grad.copy()
     grad_param['P'] = grad_param.pop('per_fourier_P')
-    grad_param.update({
-      key[4:]: grad_param.pop(key)
-      for key in list(grad_param) if key.startswith('per_decay_')
-    })
-    grad_per = np.array([
-      grad_param.pop('per_fourier_alpha'),
-      grad_param.pop('per_fourier_beta')
-    ])
+    grad_param.update(
+      {
+        key[4:]: grad_param.pop(key)
+        for key in list(grad_param)
+        if key.startswith('per_decay_')
+      }
+    )
+    grad_per = np.array(
+      [grad_param.pop('per_fourier_alpha'), grad_param.pop('per_fourier_beta')]
+    )
     grad_mag = np.array([grad_param.pop('mag_fourier_alpha'), [2 * [[0]]]])
     grad_param.update(self.compute_Fourier_back(grad_per, grad_mag))
 
-    return (grad_param)
+    return grad_param
 
-  def kernel(self, series_index, decay_kernel, mag_decay_kernel, P,
-    sig_rv_phot, sig_rv_cb, sig_phot, mag_ratio, a180, **kwargs):
+  def kernel(
+    self,
+    series_index,
+    decay_kernel,
+    mag_decay_kernel,
+    P,
+    sig_rv_phot,
+    sig_rv_cb,
+    sig_phot,
+    mag_ratio,
+    a180,
+    **kwargs,
+  ):
     r"""
     Generate a S+LEAF kernel corresponding to this FENRIR model,
     to be included in a covariance matrix (:class:`spleaf.cov.Cov`).
 
     Parameters
     ----------
     series_index : list of ndarrays
@@ -1474,38 +1576,51 @@
 
     Returns
     -------
     kernel : :class:`spleaf.term.Kernel`
       S+LEAF kernel corresponding to this FENRIR model.
     """
     kwargs.update(
-      dict(P=P,
-      sig_rv_phot=sig_rv_phot,
-      sig_rv_cb=sig_rv_cb,
-      sig_phot=sig_phot,
-      mag_ratio=mag_ratio,
-      a180=a180))
+      dict(
+        P=P,
+        sig_rv_phot=sig_rv_phot,
+        sig_rv_cb=sig_rv_cb,
+        sig_phot=sig_phot,
+        mag_ratio=mag_ratio,
+        a180=a180,
+      )
+    )
+
+    kwargs.update(
+      {f'decay_{key}': decay_kernel._get_param(key) for key in decay_kernel._param}
+    )
 
-    kwargs.update({
-      f'decay_{key}': decay_kernel._get_param(key)
-      for key in decay_kernel._param
-    })
-
-    kwargs.update({
-      f'mag_decay_{key}': mag_decay_kernel._get_param(key)
-      for key in mag_decay_kernel._param
-    })
-
-    return (term.TransformKernel(
-      term.SimpleSumKernel(per=term.SimpleProductKernel(decay=decay_kernel,
-      fourier=term.MultiFourierKernel(1,
-      np.zeros((self._nfreq, 2, 2)),
-      np.zeros((self._nfreq, 2, 2)),
-      series_index=series_index,
-      vectorize=True)),
-      mag=term.SimpleProductKernel(decay=mag_decay_kernel,
-      fourier=term.MultiFourierKernel(None,
-      np.zeros((1, 2, 1)),
-      None,
-      series_index=series_index,
-      vectorize=True))), self._translate_param, self._translate_param_back,
-      **kwargs))
+    kwargs.update(
+      {
+        f'mag_decay_{key}': mag_decay_kernel._get_param(key)
+        for key in mag_decay_kernel._param
+      }
+    )
+
+    return term.TransformKernel(
+      term.SimpleSumKernel(
+        per=term.SimpleProductKernel(
+          decay=decay_kernel,
+          fourier=term.MultiFourierKernel(
+            1,
+            np.zeros((self._nfreq, 2, 2)),
+            np.zeros((self._nfreq, 2, 2)),
+            series_index=series_index,
+            vectorize=True,
+          ),
+        ),
+        mag=term.SimpleProductKernel(
+          decay=mag_decay_kernel,
+          fourier=term.MultiFourierKernel(
+            None, np.zeros((1, 2, 1)), None, series_index=series_index, vectorize=True
+          ),
+        ),
+      ),
+      self._translate_param,
+      self._translate_param_back,
+      **kwargs,
+    )
```

### Comparing `spleaf-2.1.8/spleaf/libspleaf.c` & `spleaf-2.1.9/src/spleaf/libspleaf.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,9 @@
-// Copyright 2019-2023 Jean-Baptiste Delisle
-//
-// This file is part of spleaf.
-//
-// spleaf is free software: you can redistribute it and/or modify
-// it under the terms of the GNU General Public License as published by
-// the Free Software Foundation, either version 3 of the License, or
-// (at your option) any later version.
-//
-// spleaf is distributed in the hope that it will be useful,
-// but WITHOUT ANY WARRANTY; without even the implied warranty of
-// MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-// GNU General Public License for more details.
-//
-// You should have received a copy of the GNU General Public License
-// along with spleaf.  If not, see <http://www.gnu.org/licenses/>.
+// Copyright 2019-2024 Jean-Baptiste Delisle
+// Licensed under the EUPL-1.2 or later
 
 #include "libspleaf.h"
 
 void spleaf_cholesky(
   // Shape
   long n, long r, long *offsetrow, long *b,
   // Input
```

### Comparing `spleaf-2.1.8/spleaf/pywrapspleaf.c` & `spleaf-2.1.9/src/spleaf/pywrapspleaf.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,9 @@
-// Copyright 2019-2023 Jean-Baptiste Delisle
-//
-// This file is part of spleaf.
-//
-// spleaf is free software: you can redistribute it and/or modify
-// it under the terms of the GNU General Public License as published by
-// the Free Software Foundation, either version 3 of the License, or
-// (at your option) any later version.
-//
-// spleaf is distributed in the hope that it will be useful,
-// but WITHOUT ANY WARRANTY; without even the implied warranty of
-// MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-// GNU General Public License for more details.
-//
-// You should have received a copy of the GNU General Public License
-// along with spleaf.  If not, see <http://www.gnu.org/licenses/>.
+// Copyright 2019-2024 Jean-Baptiste Delisle
+// Licensed under the EUPL-1.2 or later
 
 #define NPY_NO_DEPRECATED_API NPY_1_18_API_VERSION
 
 #include "libspleaf.h"
 #include <Python.h>
 #include <numpy/arrayobject.h>
```

### Comparing `spleaf-2.1.8/spleaf/term.py` & `spleaf-2.1.9/src/spleaf/term.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2019-2023 Jean-Baptiste Delisle
-#
-# This file is part of spleaf.
-#
-# spleaf is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# spleaf is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with spleaf.  If not, see <http://www.gnu.org/licenses/>.
+# Copyright 2019-2024 Jean-Baptiste Delisle
+# Licensed under the EUPL-1.2 or later
 
 __all__ = [
-  'Error', 'Jitter', 'InstrumentJitter', 'CalibrationError',
-  'CalibrationJitter', 'ExponentialKernel', 'QuasiperiodicKernel',
-  'Matern12Kernel', 'Matern32Kernel', 'Matern52Kernel', 'SumKernel',
-  'SimpleSumKernel', 'ProductKernel', 'SimpleProductKernel', 'TransformKernel',
-  'USHOKernel', 'OSHOKernel', 'SHOKernel', 'MEPKernel', 'ESKernel',
-  'ESPKernel', 'MultiSeriesKernel', 'MultiFourierKernel'
+  'Error',
+  'Jitter',
+  'InstrumentJitter',
+  'CalibrationError',
+  'CalibrationJitter',
+  'ExponentialKernel',
+  'QuasiperiodicKernel',
+  'Matern12Kernel',
+  'Matern32Kernel',
+  'Matern52Kernel',
+  'SumKernel',
+  'SimpleSumKernel',
+  'ProductKernel',
+  'SimpleProductKernel',
+  'TransformKernel',
+  'USHOKernel',
+  'OSHOKernel',
+  'SHOKernel',
+  'MEPKernel',
+  'ESKernel',
+  'ESPKernel',
+  'MultiSeriesKernel',
+  'MultiFourierKernel',
 ]
 
+import warnings
+
 import numpy as np
 from scipy.special import ive
-import warnings
 
 
 class Term:
   r"""
   Generic class for covariance terms.
   """
 
@@ -41,16 +45,15 @@
     self._param = []
 
   def _link(self, cov):
     r"""
     Link the term to a covariance matrix.
     """
     if self._linked:
-      raise Exception(
-        'This term has already been linked to a covariance matrix.')
+      raise Exception('This term has already been linked to a covariance matrix.')
     self._cov = cov
     self._linked = True
 
   def _compute(self):
     r"""
     Compute the S+LEAF representation of the term.
     """
@@ -68,22 +71,22 @@
     """
     pass
 
   def _get_param(self, par):
     r"""
     Get the term parameters.
     """
-    return (self.__dict__[f'_{par}'])
+    return self.__dict__[f'_{par}']
 
   def _grad_param(self):
     r"""
     Gradient of a function with respect to the term parameters
     (listed in self._param).
     """
-    return ({})
+    return {}
 
 
 class Noise(Term):
   r"""
   Generic class for covariance noise terms.
   """
 
@@ -101,41 +104,44 @@
     super().__init__()
     self._r = 0
 
   def _link(self, cov, offset):
     super()._link(cov)
     self._offset = offset
 
-  def _compute_t2(self, t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right,
-    phi2left, phi2right):
+  def _compute_t2(
+    self, t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right, phi2left, phi2right
+  ):
     r"""
     Compute the S+LEAF representation of the covariance for a new calendar t2.
     """
 
     pass
 
   def _deriv(self, calc_d2=False):
     r"""
     Compute the S+LEAF representation of the derivative of the GP.
     """
 
     pass
 
-  def _deriv_t2(self,
+  def _deriv_t2(
+    self,
     t2,
     dt2,
     dU2,
     V2,
     phi2,
     ref2left,
     dt2left,
     dt2right,
     phi2left,
     phi2right,
-    dV2=None):
+    dV2=None,
+  ):
     r"""
     Compute the S+LEAF representation of the derivative of the GP
     for a new calendar t2.
     """
 
     pass
 
@@ -147,16 +153,15 @@
     pass
 
   def eval(self, dt, series_id=None):
     r"""
     Evaluate the kernel at lag dt.
     """
 
-    raise NotImplementedError(
-      'The eval method should be implemented in Kernel childs.')
+    raise NotImplementedError('The eval method should be implemented in Kernel childs.')
 
 
 class Error(Noise):
   r"""
   Uncorrelated measurement errors.
 
   Parameters
@@ -194,15 +199,15 @@
   def _set_param(self, sig=None):
     if sig is not None:
       self._sig = sig
 
   def _grad_param(self):
     grad = {}
     grad['sig'] = 2 * self._sig * self._cov._sum_grad_A
-    return (grad)
+    return grad
 
 
 class InstrumentJitter(Noise):
   r"""
   Uncorrelated instrument jitter.
 
   Parameters
@@ -225,15 +230,15 @@
   def _set_param(self, sig=None):
     if sig is not None:
       self._sig = sig
 
   def _grad_param(self):
     grad = {}
     grad['sig'] = 2 * self._sig * np.sum(self._cov._grad_A[self._indices])
-    return (grad)
+    return grad
 
 
 class CalibrationError(Noise):
   r"""
   Correlated calibration error.
 
   The calibration error is shared by blocks of measurements
@@ -265,16 +270,15 @@
 
   def _compute(self):
     var = self._sig**2
     self._cov.A += var
     for group in self._groups.values():
       for i in range(1, len(group)):
         for j in range(i):
-          self._cov.F[self._cov.offsetrow[group[i]] +
-            group[j]] += var[group[0]]
+          self._cov.F[self._cov.offsetrow[group[i]] + group[j]] += var[group[0]]
 
 
 class CalibrationJitter(Noise):
   r"""
   Correlated calibration jitter.
 
   The calibration jitter is shared by blocks of measurements
@@ -324,17 +328,23 @@
 
   def _set_param(self, sig=None):
     if sig is not None:
       self._sig = sig
 
   def _grad_param(self):
     grad = {}
-    grad['sig'] = 2 * self._sig * (np.sum(self._cov._grad_A[self._indices]) +
-      np.sum(self._cov._grad_F[self._Fmask]))
-    return (grad)
+    grad['sig'] = (
+      2
+      * self._sig
+      * (
+        np.sum(self._cov._grad_A[self._indices])
+        + np.sum(self._cov._grad_F[self._Fmask])
+      )
+    )
+    return grad
 
 
 class ExponentialKernel(Kernel):
   r"""
   Exponential decay kernel.
 
   This kernel follows:
@@ -366,66 +376,71 @@
     if a is not None:
       self._a = a
     if la is not None:
       self._la = la
 
   def _grad_param(self, grad_dU=None, grad_dV=None):
     grad = {}
-    grad['a'] = self._cov._sum_grad_A + np.sum(self._cov._grad_U[:,
-      self._offset])
-    grad['la'] = -np.sum(self._cov.dt * self._cov.phi[:, self._offset] *
-      self._cov._grad_phi[:, self._offset])
+    grad['a'] = self._cov._sum_grad_A + np.sum(self._cov._grad_U[:, self._offset])
+    grad['la'] = -np.sum(
+      self._cov.dt
+      * self._cov.phi[:, self._offset]
+      * self._cov._grad_phi[:, self._offset]
+    )
 
     if grad_dU is not None:
       # self._cov._dU[:, self._offset] = -self._la * self._a
       sum_grad_dU = np.sum(grad_dU[:, self._offset])
       grad['a'] -= self._la * sum_grad_dU
       grad['la'] -= self._a * sum_grad_dU
 
     if grad_dV is not None:
       # self._cov._dV[:, self._offset] = self._la
       grad['la'] += np.sum(grad_dV[:, self._offset])
 
-    return (grad)
+    return grad
 
-  def _compute_t2(self, t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right,
-    phi2left, phi2right):
+  def _compute_t2(
+    self, t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right, phi2left, phi2right
+  ):
     U2[:, self._offset] = self._a
     V2[:, self._offset] = 1.0
     phi2[:, self._offset] = np.exp(-self._la * dt2)
     phi2left[:, self._offset] = np.exp(-self._la * dt2left)
     phi2right[:, self._offset] = np.exp(-self._la * dt2right)
 
   def _deriv(self, calc_d2=False):
     self._cov._dU[:, self._offset] = -self._la * self._a
     if calc_d2:
       self._cov._dV[:, self._offset] = self._la
 
-  def _deriv_t2(self,
+  def _deriv_t2(
+    self,
     t2,
     dt2,
     dU2,
     V2,
     phi2,
     ref2left,
     dt2left,
     dt2right,
     phi2left,
     phi2right,
-    dV2=None):
+    dV2=None,
+  ):
     dU2[:, self._offset] = -self._la * self._a
     V2[:, self._offset] = 1.0
     phi2[:, self._offset] = np.exp(-self._la * dt2)
     phi2left[:, self._offset] = np.exp(-self._la * dt2left)
     phi2right[:, self._offset] = np.exp(-self._la * dt2right)
     if dV2 is not None:
       dV2[:, self._offset] = self._la
 
   def eval(self, dt, series_id=None):
-    return (self._a * np.exp(-self._la * np.abs(dt)))
+    return self._a * np.exp(-self._la * np.abs(dt))
 
 
 class QuasiperiodicKernel(Kernel):
   r"""
   Quasiperiodic kernel.
 
   This kernel follows:
@@ -455,138 +470,159 @@
   def _compute(self):
     self._cov.A += self._a
     self._nut = self._nu * self._cov.t
     self._cnut = np.cos(self._nut)
     self._snut = np.sin(self._nut)
     self._cov.U[:, self._offset] = self._a * self._cnut + self._b * self._snut
     self._cov.V[:, self._offset] = self._cnut
-    self._cov.U[:,
-      self._offset + 1] = self._a * self._snut - self._b * self._cnut
+    self._cov.U[:, self._offset + 1] = self._a * self._snut - self._b * self._cnut
     self._cov.V[:, self._offset + 1] = self._snut
-    self._cov.phi[:,
-      self._offset:self._offset + 2] = np.exp(-self._la * self._cov.dt)[:,
-      None]
+    self._cov.phi[:, self._offset : self._offset + 2] = np.exp(
+      -self._la * self._cov.dt
+    )[:, None]
 
   def _set_param(self, a=None, b=None, la=None, nu=None):
     if a is not None:
       self._a = a
     if b is not None:
       self._b = b
     if la is not None:
       self._la = la
     if nu is not None:
       self._nu = nu
 
   def _grad_param(self, grad_dU=None, grad_dV=None):
     grad = {}
-    grad['a'] = self._cov._sum_grad_A + np.sum(self._cov.V[:, self._offset] *
-      self._cov._grad_U[:, self._offset] + self._cov.V[:, self._offset + 1] *
-      self._cov._grad_U[:, self._offset + 1])
-    grad['b'] = np.sum(self._cov.V[:, self._offset + 1] *
-      self._cov._grad_U[:, self._offset] -
-      self._cov.V[:, self._offset] * self._cov._grad_U[:, self._offset + 1])
-    grad['la'] = -np.sum(self._cov.dt * self._cov.phi[:, self._offset] *
-      (self._cov._grad_phi[:, self._offset] +
-      self._cov._grad_phi[:, self._offset + 1]))
-    grad['nu'] = np.sum(self._cov.t *
-      (self._cov.U[:, self._offset] * self._cov._grad_U[:, self._offset + 1] -
-      self._cov.U[:, self._offset + 1] * self._cov._grad_U[:, self._offset] +
-      self._cov.V[:, self._offset] * self._cov._grad_V[:, self._offset + 1] -
-      self._cov.V[:, self._offset + 1] * self._cov._grad_V[:, self._offset]))
+    grad['a'] = self._cov._sum_grad_A + np.sum(
+      self._cov.V[:, self._offset] * self._cov._grad_U[:, self._offset]
+      + self._cov.V[:, self._offset + 1] * self._cov._grad_U[:, self._offset + 1]
+    )
+    grad['b'] = np.sum(
+      self._cov.V[:, self._offset + 1] * self._cov._grad_U[:, self._offset]
+      - self._cov.V[:, self._offset] * self._cov._grad_U[:, self._offset + 1]
+    )
+    grad['la'] = -np.sum(
+      self._cov.dt
+      * self._cov.phi[:, self._offset]
+      * (
+        self._cov._grad_phi[:, self._offset] + self._cov._grad_phi[:, self._offset + 1]
+      )
+    )
+    grad['nu'] = np.sum(
+      self._cov.t
+      * (
+        self._cov.U[:, self._offset] * self._cov._grad_U[:, self._offset + 1]
+        - self._cov.U[:, self._offset + 1] * self._cov._grad_U[:, self._offset]
+        + self._cov.V[:, self._offset] * self._cov._grad_V[:, self._offset + 1]
+        - self._cov.V[:, self._offset + 1] * self._cov._grad_V[:, self._offset]
+      )
+    )
 
     if grad_dU is not None:
       # self._cov._dU[:, self._offset] = da * self._cnut + db * self._snut
       # self._cov._dU[:, self._offset + 1] = da * self._snut - db * self._cnut
-      grad_da = np.sum(self._cnut * grad_dU[:, self._offset] +
-        self._snut * grad_dU[:, self._offset + 1])
-      grad_db = np.sum(self._snut * grad_dU[:, self._offset] -
-        self._cnut * grad_dU[:, self._offset + 1])
-      grad['nu'] += np.sum(self._cov.t *
-        (self._cov._dU[:, self._offset] * grad_dU[:, self._offset + 1] -
-        self._cov._dU[:, self._offset + 1] * grad_dU[:, self._offset]))
+      grad_da = np.sum(
+        self._cnut * grad_dU[:, self._offset]
+        + self._snut * grad_dU[:, self._offset + 1]
+      )
+      grad_db = np.sum(
+        self._snut * grad_dU[:, self._offset]
+        - self._cnut * grad_dU[:, self._offset + 1]
+      )
+      grad['nu'] += np.sum(
+        self._cov.t
+        * (
+          self._cov._dU[:, self._offset] * grad_dU[:, self._offset + 1]
+          - self._cov._dU[:, self._offset + 1] * grad_dU[:, self._offset]
+        )
+      )
       # da = -self._la * self._a + self._nu * self._b
       # db = -self._la * self._b - self._nu * self._a
       grad['a'] -= self._la * grad_da + self._nu * grad_db
       grad['b'] += self._nu * grad_da - self._la * grad_db
       grad['la'] -= self._a * grad_da + self._b * grad_db
       grad['nu'] += self._b * grad_da - self._a * grad_db
 
     if grad_dV is not None:
       # self._cov._dV[:, self._offset] = self._la * self._cnut - self._nu * self._snut
       # self._cov._dV[:, self._offset + 1] = self._la * self._snut + self._nu * self._cnut
-      grad['la'] += np.sum(self._cnut * grad_dV[:, self._offset] +
-        self._snut * grad_dV[:, self._offset + 1])
+      grad['la'] += np.sum(
+        self._cnut * grad_dV[:, self._offset]
+        + self._snut * grad_dV[:, self._offset + 1]
+      )
       latp1 = self._la * self._cov.t + 1
-      grad['nu'] += np.sum((latp1 * self._cnut - self._nut * self._snut) *
-        grad_dV[:, self._offset + 1] -
-        (self._nut * self._cnut + latp1 * self._snut) *
-        grad_dV[:, self._offset])
-
-    return (grad)
-
-  def _compute_t2(self, t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right,
-    phi2left, phi2right):
+      grad['nu'] += np.sum(
+        (latp1 * self._cnut - self._nut * self._snut) * grad_dV[:, self._offset + 1]
+        - (self._nut * self._cnut + latp1 * self._snut) * grad_dV[:, self._offset]
+      )
+
+    return grad
+
+  def _compute_t2(
+    self, t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right, phi2left, phi2right
+  ):
     nut2 = self._nu * t2
     cnut2 = np.cos(nut2)
     snut2 = np.sin(nut2)
     U2[:, self._offset] = self._a * cnut2 + self._b * snut2
     V2[:, self._offset] = cnut2
     U2[:, self._offset + 1] = self._a * snut2 - self._b * cnut2
     V2[:, self._offset + 1] = snut2
-    phi2[:, self._offset:self._offset + 2] = np.exp(-self._la * dt2)[:, None]
-    phi2left[:, self._offset:self._offset + 2] = np.exp(-self._la * dt2left)[:,
-      None]
-    phi2right[:,
-      self._offset:self._offset + 2] = np.exp(-self._la * dt2right)[:, None]
+    phi2[:, self._offset : self._offset + 2] = np.exp(-self._la * dt2)[:, None]
+    phi2left[:, self._offset : self._offset + 2] = np.exp(-self._la * dt2left)[:, None]
+    phi2right[:, self._offset : self._offset + 2] = np.exp(-self._la * dt2right)[
+      :, None
+    ]
 
   def _deriv(self, calc_d2=False):
     da = -self._la * self._a + self._nu * self._b
     db = -self._la * self._b - self._nu * self._a
     self._cov._dU[:, self._offset] = da * self._cnut + db * self._snut
     self._cov._dU[:, self._offset + 1] = da * self._snut - db * self._cnut
     if calc_d2:
-      self._cov._dV[:,
-        self._offset] = self._la * self._cnut - self._nu * self._snut
-      self._cov._dV[:,
-        self._offset + 1] = self._la * self._snut + self._nu * self._cnut
+      self._cov._dV[:, self._offset] = self._la * self._cnut - self._nu * self._snut
+      self._cov._dV[:, self._offset + 1] = self._la * self._snut + self._nu * self._cnut
 
-  def _deriv_t2(self,
+  def _deriv_t2(
+    self,
     t2,
     dt2,
     dU2,
     V2,
     phi2,
     ref2left,
     dt2left,
     dt2right,
     phi2left,
     phi2right,
-    dV2=None):
+    dV2=None,
+  ):
     da = -self._la * self._a + self._nu * self._b
     db = -self._la * self._b - self._nu * self._a
     nut2 = self._nu * t2
     cnut2 = np.cos(nut2)
     snut2 = np.sin(nut2)
     dU2[:, self._offset] = da * cnut2 + db * snut2
     V2[:, self._offset] = cnut2
     dU2[:, self._offset + 1] = da * snut2 - db * cnut2
     V2[:, self._offset + 1] = snut2
-    phi2[:, self._offset:self._offset + 2] = np.exp(-self._la * dt2)[:, None]
-    phi2left[:, self._offset:self._offset + 2] = np.exp(-self._la * dt2left)[:,
-      None]
-    phi2right[:,
-      self._offset:self._offset + 2] = np.exp(-self._la * dt2right)[:, None]
+    phi2[:, self._offset : self._offset + 2] = np.exp(-self._la * dt2)[:, None]
+    phi2left[:, self._offset : self._offset + 2] = np.exp(-self._la * dt2left)[:, None]
+    phi2right[:, self._offset : self._offset + 2] = np.exp(-self._la * dt2right)[
+      :, None
+    ]
     if dV2 is not None:
       dV2[:, self._offset] = self._la * cnut2 - self._nu * snut2
       dV2[:, self._offset + 1] = self._la * snut2 + self._nu * cnut2
 
   def eval(self, dt, series_id=None):
     adt = np.abs(dt)
-    return (np.exp(-self._la * adt) *
-      (self._a * np.cos(self._nu * adt) + self._b * np.sin(self._nu * adt)))
+    return np.exp(-self._la * adt) * (
+      self._a * np.cos(self._nu * adt) + self._b * np.sin(self._nu * adt)
+    )
 
 
 class Matern12Kernel(ExponentialKernel):
   r"""
   Matérn 1/2 kernel.
 
   .. math:: k(\Delta t) = \sigma^2 \mathrm{e}^{-\frac{\Delta t}{\rho}}
@@ -614,15 +650,15 @@
       self._la = 1 / rho
 
   def _grad_param(self, grad_dU=None, grad_dV=None):
     sgrad = super()._grad_param(grad_dU, grad_dV)
     grad = {}
     grad['sig'] = 2 * self._sig * sgrad['a']
     grad['rho'] = -self._la * self._la * sgrad['la']
-    return (grad)
+    return grad
 
 
 class Matern32Kernel(Kernel):
   r"""
   Matérn 3/2 kernel.
 
   .. math:: k(\Delta t) = \sigma^2 \mathrm{e}^{-\sqrt{3}\frac{\Delta t}{\rho}}
@@ -655,103 +691,138 @@
     self._x = self._la * self._dt0
     self._1mx = 1 - self._x
     self._cov.A += self._a
     self._cov.U[:, self._offset] = self._a * self._x
     self._cov.V[:, self._offset] = 1.0
     self._cov.U[:, self._offset + 1] = self._a
     self._cov.V[:, self._offset + 1] = self._1mx
-    self._cov.phi[:,
-      self._offset:self._offset + 2] = np.exp(-self._la * self._cov.dt)[:,
-      None]
+    self._cov.phi[:, self._offset : self._offset + 2] = np.exp(
+      -self._la * self._cov.dt
+    )[:, None]
 
   def _set_param(self, sig=None, rho=None):
     if sig is not None:
       self._sig = sig
     if rho is not None:
       self._rho = rho
 
   def _grad_param(self, grad_dU=None, grad_dV=None):
     grad = {}
-    grad['sig'] = 2 * self._sig * (self._cov._sum_grad_A +
-      np.sum(self._x * self._cov._grad_U[:, self._offset] +
-      self._cov._grad_U[:, self._offset + 1]))
-    grad['rho'] = -1 / self._rho * (np.sum(self._x *
-      (self._a * self._cov._grad_U[:, self._offset] -
-      self._cov._grad_V[:, self._offset + 1])) -
-      self._la * np.sum(self._cov.dt * self._cov.phi[:, self._offset] *
-      (self._cov._grad_phi[:, self._offset] +
-      self._cov._grad_phi[:, self._offset + 1])))
+    grad['sig'] = (
+      2
+      * self._sig
+      * (
+        self._cov._sum_grad_A
+        + np.sum(
+          self._x * self._cov._grad_U[:, self._offset]
+          + self._cov._grad_U[:, self._offset + 1]
+        )
+      )
+    )
+    grad['rho'] = (
+      -1
+      / self._rho
+      * (
+        np.sum(
+          self._x
+          * (
+            self._a * self._cov._grad_U[:, self._offset]
+            - self._cov._grad_V[:, self._offset + 1]
+          )
+        )
+        - self._la
+        * np.sum(
+          self._cov.dt
+          * self._cov.phi[:, self._offset]
+          * (
+            self._cov._grad_phi[:, self._offset]
+            + self._cov._grad_phi[:, self._offset + 1]
+          )
+        )
+      )
+    )
 
     if grad_dU is not None:
       # self._cov._dU[:, self._offset] = self._la * self._a * self._1mx
       # self._cov._dU[:, self._offset + 1] = -self._la * self._a
-      sum_grad_dU = np.sum(self._1mx * grad_dU[:, self._offset] -
-        grad_dU[:, self._offset + 1])
+      sum_grad_dU = np.sum(
+        self._1mx * grad_dU[:, self._offset] - grad_dU[:, self._offset + 1]
+      )
       grad['sig'] += 2 * self._sig * self._la * sum_grad_dU
-      grad['rho'] -= self._la / self._rho * self._a * (sum_grad_dU -
-        np.sum(self._x * grad_dU[:, self._offset]))
+      grad['rho'] -= (
+        self._la
+        / self._rho
+        * self._a
+        * (sum_grad_dU - np.sum(self._x * grad_dU[:, self._offset]))
+      )
 
     if grad_dV is not None:
       # self._cov._dV[:, self._offset] = self._la
       # self._cov._dV[:, self._offset + 1] = -self._la * self._x
-      grad['rho'] -= self._la / self._rho * np.sum(grad_dV[:, self._offset] -
-        2 * self._x * grad_dV[:, self._offset + 1])
-
-    return (grad)
-
-  def _compute_t2(self, t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right,
-    phi2left, phi2right):
+      grad['rho'] -= (
+        self._la
+        / self._rho
+        * np.sum(grad_dV[:, self._offset] - 2 * self._x * grad_dV[:, self._offset + 1])
+      )
+
+    return grad
+
+  def _compute_t2(
+    self, t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right, phi2left, phi2right
+  ):
     x2 = self._la * (t2 - self._t0)
     U2[:, self._offset] = self._a * x2
     V2[:, self._offset] = 1.0
     U2[:, self._offset + 1] = self._a
     V2[:, self._offset + 1] = 1 - x2
-    phi2[:, self._offset:self._offset + 2] = np.exp(-self._la * dt2)[:, None]
-    phi2left[:, self._offset:self._offset + 2] = np.exp(-self._la * dt2left)[:,
-      None]
-    phi2right[:,
-      self._offset:self._offset + 2] = np.exp(-self._la * dt2right)[:, None]
+    phi2[:, self._offset : self._offset + 2] = np.exp(-self._la * dt2)[:, None]
+    phi2left[:, self._offset : self._offset + 2] = np.exp(-self._la * dt2left)[:, None]
+    phi2right[:, self._offset : self._offset + 2] = np.exp(-self._la * dt2right)[
+      :, None
+    ]
 
   def _deriv(self, calc_d2=False):
     self._cov._dU[:, self._offset] = self._la * self._a * self._1mx
     self._cov._dU[:, self._offset + 1] = -self._la * self._a
     if calc_d2:
       self._cov._dV[:, self._offset] = self._la
       self._cov._dV[:, self._offset + 1] = -self._la * self._x
 
-  def _deriv_t2(self,
+  def _deriv_t2(
+    self,
     t2,
     dt2,
     dU2,
     V2,
     phi2,
     ref2left,
     dt2left,
     dt2right,
     phi2left,
     phi2right,
-    dV2=None):
+    dV2=None,
+  ):
     x2 = self._la * (t2 - self._t0)
     onemx2 = 1 - x2
     dU2[:, self._offset] = self._la * self._a * onemx2
     V2[:, self._offset] = 1.0
     dU2[:, self._offset + 1] = -self._la * self._a
     V2[:, self._offset + 1] = onemx2
-    phi2[:, self._offset:self._offset + 2] = np.exp(-self._la * dt2)[:, None]
-    phi2left[:, self._offset:self._offset + 2] = np.exp(-self._la * dt2left)[:,
-      None]
-    phi2right[:,
-      self._offset:self._offset + 2] = np.exp(-self._la * dt2right)[:, None]
+    phi2[:, self._offset : self._offset + 2] = np.exp(-self._la * dt2)[:, None]
+    phi2left[:, self._offset : self._offset + 2] = np.exp(-self._la * dt2left)[:, None]
+    phi2right[:, self._offset : self._offset + 2] = np.exp(-self._la * dt2right)[
+      :, None
+    ]
     if dV2 is not None:
       dV2[:, self._offset] = self._la
       dV2[:, self._offset + 1] = -self._la * x2
 
   def eval(self, dt, series_id=None):
     dx = self._la * np.abs(dt)
-    return (self._a * np.exp(-dx) * (1 + dx))
+    return self._a * np.exp(-dx) * (1 + dx)
 
 
 class Matern52Kernel(Kernel):
   r"""
   Matérn 5/2 kernel.
 
   .. math:: k(\Delta t) = \sigma^2 \mathrm{e}^{-\sqrt{5}\frac{\Delta t}{\rho}}
@@ -788,122 +859,166 @@
     self._cov.A += self._a
     self._cov.U[:, self._offset] = self._a * (self._x + self._x2_3)
     self._cov.V[:, self._offset] = 1.0
     self._cov.U[:, self._offset + 1] = self._a
     self._cov.V[:, self._offset + 1] = self._1mx + self._x2_3
     self._cov.U[:, self._offset + 2] = self._a * self._x
     self._cov.V[:, self._offset + 2] = -2 / 3 * self._x
-    self._cov.phi[:,
-      self._offset:self._offset + 3] = np.exp(-self._la * self._cov.dt)[:,
-      None]
+    self._cov.phi[:, self._offset : self._offset + 3] = np.exp(
+      -self._la * self._cov.dt
+    )[:, None]
 
   def _set_param(self, sig=None, rho=None):
     if sig is not None:
       self._sig = sig
     if rho is not None:
       self._rho = rho
 
   def _grad_param(self, grad_dU=None, grad_dV=None):
     grad = {}
-    grad['sig'] = 2 * self._sig * (self._cov._sum_grad_A +
-      np.sum((self._x + self._x2_3) * self._cov._grad_U[:, self._offset] +
-      self._cov._grad_U[:, self._offset + 1] +
-      self._x * self._cov._grad_U[:, self._offset + 2]))
-    grad['rho'] = -1 / self._rho * (np.sum(self._a *
-      (self._x + 2 * self._x2_3) * self._cov._grad_U[:, self._offset] +
-      (2 * self._x2_3 - self._x) * self._cov._grad_V[:, self._offset + 1] +
-      self._x * (self._a * self._cov._grad_U[:, self._offset + 2] -
-      2 / 3 * self._cov._grad_V[:, self._offset + 2])) -
-      self._la * np.sum(self._cov.dt * self._cov.phi[:, self._offset] *
-      (self._cov._grad_phi[:, self._offset] + self._cov._grad_phi[:,
-      self._offset + 1] + self._cov._grad_phi[:, self._offset + 2])))
+    grad['sig'] = (
+      2
+      * self._sig
+      * (
+        self._cov._sum_grad_A
+        + np.sum(
+          (self._x + self._x2_3) * self._cov._grad_U[:, self._offset]
+          + self._cov._grad_U[:, self._offset + 1]
+          + self._x * self._cov._grad_U[:, self._offset + 2]
+        )
+      )
+    )
+    grad['rho'] = (
+      -1
+      / self._rho
+      * (
+        np.sum(
+          self._a * (self._x + 2 * self._x2_3) * self._cov._grad_U[:, self._offset]
+          + (2 * self._x2_3 - self._x) * self._cov._grad_V[:, self._offset + 1]
+          + self._x
+          * (
+            self._a * self._cov._grad_U[:, self._offset + 2]
+            - 2 / 3 * self._cov._grad_V[:, self._offset + 2]
+          )
+        )
+        - self._la
+        * np.sum(
+          self._cov.dt
+          * self._cov.phi[:, self._offset]
+          * (
+            self._cov._grad_phi[:, self._offset]
+            + self._cov._grad_phi[:, self._offset + 1]
+            + self._cov._grad_phi[:, self._offset + 2]
+          )
+        )
+      )
+    )
 
     if grad_dU is not None:
       # self._cov._dU[:,
       #   self._offset] = self._la * self._a * (1 - self._x / 3 - self._x2_3)
       # self._cov._dU[:, self._offset + 1] = -self._la * self._a
       # self._cov._dU[:, self._offset + 2] = self._la * self._1mx * self._a
-      sum_grad_dU = np.sum((1 - self._x / 3 - self._x2_3) *
-        grad_dU[:, self._offset] - grad_dU[:, self._offset + 1] +
-        self._1mx * grad_dU[:, self._offset + 2])
+      sum_grad_dU = np.sum(
+        (1 - self._x / 3 - self._x2_3) * grad_dU[:, self._offset]
+        - grad_dU[:, self._offset + 1]
+        + self._1mx * grad_dU[:, self._offset + 2]
+      )
       grad['sig'] += 2 * self._sig * self._la * sum_grad_dU
-      grad['rho'] -= self._la / self._rho * self._a * (sum_grad_dU -
-        np.sum((self._x / 3 + 2 * self._x2_3) * grad_dU[:, self._offset] +
-        self._x * grad_dU[:, self._offset + 2]))
+      grad['rho'] -= (
+        self._la
+        / self._rho
+        * self._a
+        * (
+          sum_grad_dU
+          - np.sum(
+            (self._x / 3 + 2 * self._x2_3) * grad_dU[:, self._offset]
+            + self._x * grad_dU[:, self._offset + 2]
+          )
+        )
+      )
 
     if grad_dV is not None:
       # self._cov._dV[:, self._offset] = self._la
       # self._cov._dV[:, self._offset + 1] = -self._la * self._x / 3 * self._1mx
       # self._cov._dV[:, self._offset + 2] = -2 / 3 * self._la * (1 + self._x)
-      grad['rho'] -= self._la / self._rho * np.sum(grad_dV[:, self._offset] +
-        (3 * self._x2_3 - 2 / 3 * self._x) * grad_dV[:, self._offset + 1] -
-        2 / 3 * (1 + 2 * self._x) * grad_dV[:, self._offset + 2])
-
-    return (grad)
-
-  def _compute_t2(self, t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right,
-    phi2left, phi2right):
+      grad['rho'] -= (
+        self._la
+        / self._rho
+        * np.sum(
+          grad_dV[:, self._offset]
+          + (3 * self._x2_3 - 2 / 3 * self._x) * grad_dV[:, self._offset + 1]
+          - 2 / 3 * (1 + 2 * self._x) * grad_dV[:, self._offset + 2]
+        )
+      )
+
+    return grad
+
+  def _compute_t2(
+    self, t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right, phi2left, phi2right
+  ):
     x2 = self._la * (t2 - self._t0)
     x22_3 = x2 * x2 / 3
     U2[:, self._offset] = self._a * (x2 + x22_3)
     V2[:, self._offset] = 1.0
     U2[:, self._offset + 1] = self._a
     V2[:, self._offset + 1] = 1 - x2 + x22_3
     U2[:, self._offset + 2] = self._a * x2
     V2[:, self._offset + 2] = -2 / 3 * x2
-    phi2[:, self._offset:self._offset + 3] = np.exp(-self._la * dt2)[:, None]
-    phi2left[:, self._offset:self._offset + 3] = np.exp(-self._la * dt2left)[:,
-      None]
-    phi2right[:,
-      self._offset:self._offset + 3] = np.exp(-self._la * dt2right)[:, None]
+    phi2[:, self._offset : self._offset + 3] = np.exp(-self._la * dt2)[:, None]
+    phi2left[:, self._offset : self._offset + 3] = np.exp(-self._la * dt2left)[:, None]
+    phi2right[:, self._offset : self._offset + 3] = np.exp(-self._la * dt2right)[
+      :, None
+    ]
 
   def _deriv(self, calc_d2=False):
-    self._cov._dU[:,
-      self._offset] = self._la * self._a * (1 - self._x / 3 - self._x2_3)
+    self._cov._dU[:, self._offset] = self._la * self._a * (1 - self._x / 3 - self._x2_3)
     self._cov._dU[:, self._offset + 1] = -self._la * self._a
     self._cov._dU[:, self._offset + 2] = self._la * self._a * self._1mx
     if calc_d2:
       self._cov._dV[:, self._offset] = self._la
       self._cov._dV[:, self._offset + 1] = -self._la * self._x / 3 * self._1mx
       self._cov._dV[:, self._offset + 2] = -2 / 3 * self._la * (1 + self._x)
 
-  def _deriv_t2(self,
+  def _deriv_t2(
+    self,
     t2,
     dt2,
     dU2,
     V2,
     phi2,
     ref2left,
     dt2left,
     dt2right,
     phi2left,
     phi2right,
-    dV2=None):
+    dV2=None,
+  ):
     x2 = self._la * (t2 - self._t0)
     onemx2 = 1 - x2
     x22_3 = x2 * x2 / 3
     dU2[:, self._offset] = self._la * self._a * (1 - x2 / 3 - x22_3)
     V2[:, self._offset] = 1.0
     dU2[:, self._offset + 1] = -self._la * self._a
     V2[:, self._offset + 1] = onemx2 + x22_3
     dU2[:, self._offset + 2] = self._la * onemx2 * self._a
     V2[:, self._offset + 2] = -2 / 3 * x2
-    phi2[:, self._offset:self._offset + 3] = np.exp(-self._la * dt2)[:, None]
-    phi2left[:, self._offset:self._offset + 3] = np.exp(-self._la * dt2left)[:,
-      None]
-    phi2right[:,
-      self._offset:self._offset + 3] = np.exp(-self._la * dt2right)[:, None]
+    phi2[:, self._offset : self._offset + 3] = np.exp(-self._la * dt2)[:, None]
+    phi2left[:, self._offset : self._offset + 3] = np.exp(-self._la * dt2left)[:, None]
+    phi2right[:, self._offset : self._offset + 3] = np.exp(-self._la * dt2right)[
+      :, None
+    ]
     if dV2 is not None:
       dV2[:, self._offset] = self._la
       dV2[:, self._offset + 1] = -self._la * x2 / 3 * onemx2
       dV2[:, self._offset + 2] = -2 / 3 * self._la * (1 + x2)
 
   def eval(self, dt, series_id=None):
     dx = self._la * np.abs(dt)
-    return (self._a * np.exp(-dx) * (1 + dx + dx * dx / 3))
+    return self._a * np.exp(-dx) * (1 + dx + dx * dx / 3)
 
 
 class SumKernel(Kernel):
   r"""
   Generic class for the sum of several kernel terms.
   """
 
@@ -921,95 +1036,96 @@
 
   def _compute(self):
     for kernel in self._kernels:
       kernel._compute()
 
   def _kernel_param(self, **kwargs):
     raise NotImplementedError(
-      'The _kernel_param method should be implemented in SumKernel childs.')
+      'The _kernel_param method should be implemented in SumKernel childs.'
+    )
 
   def _kernel_param_back(self, *args):
     raise NotImplementedError(
-      'The _kernel_param method should be implemented in SumKernel childs.')
+      'The _kernel_param method should be implemented in SumKernel childs.'
+    )
 
   def _set_param(self, *args, **kwargs):
     for karg, arg in enumerate(args):
       par = self._param[karg]
       if par in kwargs:
-        raise Exception(
-          f'SumKernel._set_param: parameter {par} multiply defined.')
+        raise Exception(f'SumKernel._set_param: parameter {par} multiply defined.')
       kwargs[par] = arg
     kernel_param = self._kernel_param(**kwargs)
     for kernel, param in zip(self._kernels, kernel_param):
       kernel._set_param(**param)
 
   def _grad_param(self, grad_dU=None, grad_dV=None):
-    kernel_grad = [
-      kernel._grad_param(grad_dU, grad_dV) for kernel in self._kernels
-    ]
-    return (self._kernel_param_back(*kernel_grad))
+    kernel_grad = [kernel._grad_param(grad_dU, grad_dV) for kernel in self._kernels]
+    return self._kernel_param_back(*kernel_grad)
 
-  def _compute_t2(self, t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right,
-    phi2left, phi2right):
+  def _compute_t2(
+    self, t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right, phi2left, phi2right
+  ):
     for kernel in self._kernels:
-      kernel._compute_t2(t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right,
-        phi2left, phi2right)
+      kernel._compute_t2(
+        t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right, phi2left, phi2right
+      )
 
   def _deriv(self, calc_d2=False):
     for kernel in self._kernels:
       kernel._deriv(calc_d2)
 
-  def _deriv_t2(self,
+  def _deriv_t2(
+    self,
     t2,
     dt2,
     dU2,
     V2,
     phi2,
     ref2left,
     dt2left,
     dt2right,
     phi2left,
     phi2right,
-    dV2=None):
+    dV2=None,
+  ):
     for kernel in self._kernels:
-      kernel._deriv_t2(t2, dt2, dU2, V2, phi2, ref2left, dt2left, dt2right,
-        phi2left, phi2right, dV2)
+      kernel._deriv_t2(
+        t2, dt2, dU2, V2, phi2, ref2left, dt2left, dt2right, phi2left, phi2right, dV2
+      )
 
   def eval(self, dt, series_id=(0, 0)):
-    return (sum(kernel.eval(dt, series_id) for kernel in self._kernels))
+    return sum(kernel.eval(dt, series_id) for kernel in self._kernels)
 
 
 class SimpleSumKernel(SumKernel):
-  r"""
-  """
+  r""" """
 
   def __init__(self, **kwargs):
     self._kerneldic = kwargs
     super().__init__(*kwargs.values())
-    self._param = [
-      f'{kern}_{key}' for kern in kwargs for key in kwargs[kern]._param
-    ]
+    self._param = [f'{kern}_{key}' for kern in kwargs for key in kwargs[kern]._param]
 
   def _kernel_param(self, **kwargs):
     paramKern = {kern: {} for kern in self._kerneldic}
     for par in kwargs:
       kern, key = par.split('_', 1)
       paramKern[kern][key] = kwargs[par]
-    return (paramKern.values())
+    return paramKern.values()
 
   def _kernel_param_back(self, *args):
     grad = {}
     for kern, gk in zip(self._kerneldic, args):
       for key in gk:
         grad[f'{kern}_{key}'] = gk[key]
-    return (grad)
+    return grad
 
   def _get_param(self, par):
     kern, key = par.split('_', 1)
-    return (self._kerneldic[kern]._get_param(key))
+    return self._kerneldic[kern]._get_param(key)
 
   def set_conditional_coef(self, **kwargs):
     r"""
     Set the coefficients used for the conditional computations.
     """
     paramKern = {kern: {} for kern in self._kerneldic}
     for par in kwargs:
@@ -1020,15 +1136,14 @@
         kern, key = par.split('_', 1)
         paramKern[kern][key] = kwargs[par]
     for kern in self._kerneldic:
       self._kerneldic[kern].set_conditional_coef(**paramKern[kern])
 
 
 class _FakeCov:
-
   def __init__(self, t, dt, r):
     self.t = t
     self.dt = dt
     self.n = t.size
     self.r = r
     self.A = np.zeros(self.n)
     self.U = np.empty((self.n, r))
@@ -1069,23 +1184,29 @@
   def _compute(self):
     self._kernel1._cov.A[:] = 0
     self._kernel2._cov.A[:] = 0
     self._kernel1._compute()
     self._kernel2._compute()
     self._cov.A += self._kernel1._cov.A * self._kernel2._cov.A
     for k1 in range(self._kernel1._r):
-      self._cov.U[:, self._offset + k1 * self._kernel2._r:self._offset +
-        (k1 + 1) * self._kernel2._r] = self._kernel1._cov.U[:, k1,
-        None] * self._kernel2._cov.U
-      self._cov.V[:, self._offset + k1 * self._kernel2._r:self._offset +
-        (k1 + 1) * self._kernel2._r] = self._kernel1._cov.V[:, k1,
-        None] * self._kernel2._cov.V
-      self._cov.phi[:, self._offset + k1 * self._kernel2._r:self._offset +
-        (k1 + 1) * self._kernel2._r] = self._kernel1._cov.phi[:, k1,
-        None] * self._kernel2._cov.phi
+      self._cov.U[
+        :,
+        self._offset + k1 * self._kernel2._r : self._offset
+        + (k1 + 1) * self._kernel2._r,
+      ] = self._kernel1._cov.U[:, k1, None] * self._kernel2._cov.U
+      self._cov.V[
+        :,
+        self._offset + k1 * self._kernel2._r : self._offset
+        + (k1 + 1) * self._kernel2._r,
+      ] = self._kernel1._cov.V[:, k1, None] * self._kernel2._cov.V
+      self._cov.phi[
+        :,
+        self._offset + k1 * self._kernel2._r : self._offset
+        + (k1 + 1) * self._kernel2._r,
+      ] = self._kernel1._cov.phi[:, k1, None] * self._kernel2._cov.phi
 
   def _kernel_param(self, **kwargs):
     raise NotImplementedError(
       'The _kernel_param method should be implemented in ProductKernel childs.'
     )
 
   def _kernel_param_back(self, *args):
@@ -1093,243 +1214,386 @@
       'The _kernel_param method should be implemented in ProductKernel childs.'
     )
 
   def _set_param(self, *args, **kwargs):
     for karg, arg in enumerate(args):
       par = self._param[karg]
       if par in kwargs:
-        raise Exception(
-          f'ProductKernel._set_param: parameter {par} multiply defined.')
+        raise Exception(f'ProductKernel._set_param: parameter {par} multiply defined.')
       kwargs[par] = arg
     kernel1_param, kernel2_param = self._kernel_param(**kwargs)
     self._kernel1._set_param(**kernel1_param)
     self._kernel2._set_param(**kernel2_param)
 
   def _grad_param(self, grad_dU=None, grad_dV=None):
     self._kernel1._cov._grad_A = self._kernel2._cov.A * self._cov._grad_A
     self._kernel2._cov._grad_A = self._kernel1._cov.A * self._cov._grad_A
     self._kernel1._cov._sum_grad_A = np.sum(self._kernel1._cov._grad_A)
     self._kernel2._cov._sum_grad_A = np.sum(self._kernel2._cov._grad_A)
     for k1 in range(self._kernel1._r):
-      self._kernel1._cov._grad_U[:,
-        k1] = np.sum(self._kernel2._cov.U * self._cov._grad_U[:, self._offset +
-        k1 * self._kernel2._r:self._offset + (k1 + 1) * self._kernel2._r],
-        axis=1)
-      self._kernel1._cov._grad_V[:,
-        k1] = np.sum(self._kernel2._cov.V * self._cov._grad_V[:, self._offset +
-        k1 * self._kernel2._r:self._offset + (k1 + 1) * self._kernel2._r],
-        axis=1)
-      self._kernel1._cov._grad_phi[:,
-        k1] = np.sum(self._kernel2._cov.phi * self._cov._grad_phi[:,
-        self._offset + k1 * self._kernel2._r:self._offset +
-        (k1 + 1) * self._kernel2._r],
-        axis=1)
+      self._kernel1._cov._grad_U[:, k1] = np.sum(
+        self._kernel2._cov.U
+        * self._cov._grad_U[
+          :,
+          self._offset + k1 * self._kernel2._r : self._offset
+          + (k1 + 1) * self._kernel2._r,
+        ],
+        axis=1,
+      )
+      self._kernel1._cov._grad_V[:, k1] = np.sum(
+        self._kernel2._cov.V
+        * self._cov._grad_V[
+          :,
+          self._offset + k1 * self._kernel2._r : self._offset
+          + (k1 + 1) * self._kernel2._r,
+        ],
+        axis=1,
+      )
+      self._kernel1._cov._grad_phi[:, k1] = np.sum(
+        self._kernel2._cov.phi
+        * self._cov._grad_phi[
+          :,
+          self._offset + k1 * self._kernel2._r : self._offset
+          + (k1 + 1) * self._kernel2._r,
+        ],
+        axis=1,
+      )
       if grad_dU is not None:
-        self._kernel1._cov._grad_U[:, k1] += np.sum(self._kernel2._cov._dU *
-          grad_dU[:, self._offset + k1 * self._kernel2._r:self._offset +
-          (k1 + 1) * self._kernel2._r],
-          axis=1)
-        self._kernel1._cov._grad_dU[:, k1] = np.sum(self._kernel2._cov.U *
-          grad_dU[:, self._offset + k1 * self._kernel2._r:self._offset +
-          (k1 + 1) * self._kernel2._r],
-          axis=1)
+        self._kernel1._cov._grad_U[:, k1] += np.sum(
+          self._kernel2._cov._dU
+          * grad_dU[
+            :,
+            self._offset + k1 * self._kernel2._r : self._offset
+            + (k1 + 1) * self._kernel2._r,
+          ],
+          axis=1,
+        )
+        self._kernel1._cov._grad_dU[:, k1] = np.sum(
+          self._kernel2._cov.U
+          * grad_dU[
+            :,
+            self._offset + k1 * self._kernel2._r : self._offset
+            + (k1 + 1) * self._kernel2._r,
+          ],
+          axis=1,
+        )
       if grad_dV is not None:
-        self._kernel1._cov._grad_V[:, k1] += np.sum(self._kernel2._cov._dV *
-          grad_dV[:, self._offset + k1 * self._kernel2._r:self._offset +
-          (k1 + 1) * self._kernel2._r],
-          axis=1)
-        self._kernel1._cov._grad_dV[:, k1] = np.sum(self._kernel2._cov.V *
-          grad_dV[:, self._offset + k1 * self._kernel2._r:self._offset +
-          (k1 + 1) * self._kernel2._r],
-          axis=1)
+        self._kernel1._cov._grad_V[:, k1] += np.sum(
+          self._kernel2._cov._dV
+          * grad_dV[
+            :,
+            self._offset + k1 * self._kernel2._r : self._offset
+            + (k1 + 1) * self._kernel2._r,
+          ],
+          axis=1,
+        )
+        self._kernel1._cov._grad_dV[:, k1] = np.sum(
+          self._kernel2._cov.V
+          * grad_dV[
+            :,
+            self._offset + k1 * self._kernel2._r : self._offset
+            + (k1 + 1) * self._kernel2._r,
+          ],
+          axis=1,
+        )
 
     for k2 in range(self._kernel2._r):
-      self._kernel2._cov._grad_U[:,
-        k2] = np.sum(self._kernel1._cov.U * self._cov._grad_U[:,
-        self._offset + k2:self._offset + self._r:self._kernel2._r],
-        axis=1)
-      self._kernel2._cov._grad_V[:,
-        k2] = np.sum(self._kernel1._cov.V * self._cov._grad_V[:,
-        self._offset + k2:self._offset + self._r:self._kernel2._r],
-        axis=1)
-      self._kernel2._cov._grad_phi[:,
-        k2] = np.sum(self._kernel1._cov.phi * self._cov._grad_phi[:,
-        self._offset + k2:self._offset + self._r:self._kernel2._r],
-        axis=1)
+      self._kernel2._cov._grad_U[:, k2] = np.sum(
+        self._kernel1._cov.U
+        * self._cov._grad_U[
+          :, self._offset + k2 : self._offset + self._r : self._kernel2._r
+        ],
+        axis=1,
+      )
+      self._kernel2._cov._grad_V[:, k2] = np.sum(
+        self._kernel1._cov.V
+        * self._cov._grad_V[
+          :, self._offset + k2 : self._offset + self._r : self._kernel2._r
+        ],
+        axis=1,
+      )
+      self._kernel2._cov._grad_phi[:, k2] = np.sum(
+        self._kernel1._cov.phi
+        * self._cov._grad_phi[
+          :, self._offset + k2 : self._offset + self._r : self._kernel2._r
+        ],
+        axis=1,
+      )
       if grad_dU is not None:
-        self._kernel2._cov._grad_U[:,
-          k2] += np.sum(self._kernel1._cov._dU * grad_dU[:,
-          self._offset + k2:self._offset + self._r:self._kernel2._r],
-          axis=1)
-        self._kernel2._cov._grad_dU[:,
-          k2] = np.sum(self._kernel1._cov.U * grad_dU[:,
-          self._offset + k2:self._offset + self._r:self._kernel2._r],
-          axis=1)
+        self._kernel2._cov._grad_U[:, k2] += np.sum(
+          self._kernel1._cov._dU
+          * grad_dU[:, self._offset + k2 : self._offset + self._r : self._kernel2._r],
+          axis=1,
+        )
+        self._kernel2._cov._grad_dU[:, k2] = np.sum(
+          self._kernel1._cov.U
+          * grad_dU[:, self._offset + k2 : self._offset + self._r : self._kernel2._r],
+          axis=1,
+        )
       if grad_dV is not None:
-        self._kernel2._cov._grad_V[:,
-          k2] += np.sum(self._kernel1._cov._dV * grad_dV[:,
-          self._offset + k2:self._offset + self._r:self._kernel2._r],
-          axis=1)
-        self._kernel2._cov._grad_dV[:,
-          k2] = np.sum(self._kernel1._cov.V * grad_dV[:,
-          self._offset + k2:self._offset + self._r:self._kernel2._r],
-          axis=1)
+        self._kernel2._cov._grad_V[:, k2] += np.sum(
+          self._kernel1._cov._dV
+          * grad_dV[:, self._offset + k2 : self._offset + self._r : self._kernel2._r],
+          axis=1,
+        )
+        self._kernel2._cov._grad_dV[:, k2] = np.sum(
+          self._kernel1._cov.V
+          * grad_dV[:, self._offset + k2 : self._offset + self._r : self._kernel2._r],
+          axis=1,
+        )
 
     kernel1_grad = self._kernel1._grad_param(
       self._kernel1._cov._grad_dU if grad_dU is not None else None,
-      self._kernel1._cov._grad_dV if grad_dV is not None else None)
+      self._kernel1._cov._grad_dV if grad_dV is not None else None,
+    )
     kernel2_grad = self._kernel2._grad_param(
       self._kernel2._cov._grad_dU if grad_dU is not None else None,
-      self._kernel2._cov._grad_dV if grad_dV is not None else None)
-    return (self._kernel_param_back(kernel1_grad, kernel2_grad))
+      self._kernel2._cov._grad_dV if grad_dV is not None else None,
+    )
+    return self._kernel_param_back(kernel1_grad, kernel2_grad)
 
-  def _compute_t2(self, t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right,
-    phi2left, phi2right):
+  def _compute_t2(
+    self, t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right, phi2left, phi2right
+  ):
     kernel1_U2 = np.empty((t2.size, self._kernel1._r))
     kernel1_V2 = np.empty((t2.size, self._kernel1._r))
     kernel1_phi2 = np.empty((t2.size - 1, self._kernel1._r))
     kernel1_phi2left = np.empty((t2.size, self._kernel1._r))
     kernel1_phi2right = np.empty((t2.size, self._kernel1._r))
-    self._kernel1._compute_t2(t2, dt2, kernel1_U2, kernel1_V2, kernel1_phi2,
-      ref2left, dt2left, dt2right, kernel1_phi2left, kernel1_phi2right)
+    self._kernel1._compute_t2(
+      t2,
+      dt2,
+      kernel1_U2,
+      kernel1_V2,
+      kernel1_phi2,
+      ref2left,
+      dt2left,
+      dt2right,
+      kernel1_phi2left,
+      kernel1_phi2right,
+    )
 
     kernel2_U2 = np.empty((t2.size, self._kernel2._r))
     kernel2_V2 = np.empty((t2.size, self._kernel2._r))
     kernel2_phi2 = np.empty((t2.size - 1, self._kernel2._r))
     kernel2_phi2left = np.empty((t2.size, self._kernel2._r))
     kernel2_phi2right = np.empty((t2.size, self._kernel2._r))
-    self._kernel2._compute_t2(t2, dt2, kernel2_U2, kernel2_V2, kernel2_phi2,
-      ref2left, dt2left, dt2right, kernel2_phi2left, kernel2_phi2right)
+    self._kernel2._compute_t2(
+      t2,
+      dt2,
+      kernel2_U2,
+      kernel2_V2,
+      kernel2_phi2,
+      ref2left,
+      dt2left,
+      dt2right,
+      kernel2_phi2left,
+      kernel2_phi2right,
+    )
 
     for k1 in range(self._kernel1._r):
-      U2[:, self._offset + k1 * self._kernel2._r:self._offset +
-        (k1 + 1) * self._kernel2._r] = kernel1_U2[:, k1, None] * kernel2_U2
-      V2[:, self._offset + k1 * self._kernel2._r:self._offset +
-        (k1 + 1) * self._kernel2._r] = kernel1_V2[:, k1, None] * kernel2_V2
-      phi2[:, self._offset + k1 * self._kernel2._r:self._offset +
-        (k1 + 1) * self._kernel2._r] = kernel1_phi2[:, k1, None] * kernel2_phi2
-      phi2left[:,
-        self._offset + k1 * self._kernel2._r:self._offset + (k1 + 1) *
-        self._kernel2._r] = kernel1_phi2left[:, k1, None] * kernel2_phi2left
-      phi2right[:,
-        self._offset + k1 * self._kernel2._r:self._offset + (k1 + 1) *
-        self._kernel2._r] = kernel1_phi2right[:, k1, None] * kernel2_phi2right
+      U2[
+        :,
+        self._offset + k1 * self._kernel2._r : self._offset
+        + (k1 + 1) * self._kernel2._r,
+      ] = kernel1_U2[:, k1, None] * kernel2_U2
+      V2[
+        :,
+        self._offset + k1 * self._kernel2._r : self._offset
+        + (k1 + 1) * self._kernel2._r,
+      ] = kernel1_V2[:, k1, None] * kernel2_V2
+      phi2[
+        :,
+        self._offset + k1 * self._kernel2._r : self._offset
+        + (k1 + 1) * self._kernel2._r,
+      ] = kernel1_phi2[:, k1, None] * kernel2_phi2
+      phi2left[
+        :,
+        self._offset + k1 * self._kernel2._r : self._offset
+        + (k1 + 1) * self._kernel2._r,
+      ] = kernel1_phi2left[:, k1, None] * kernel2_phi2left
+      phi2right[
+        :,
+        self._offset + k1 * self._kernel2._r : self._offset
+        + (k1 + 1) * self._kernel2._r,
+      ] = kernel1_phi2right[:, k1, None] * kernel2_phi2right
 
   def _deriv(self, calc_d2=False):
     self._kernel1._deriv(calc_d2)
     self._kernel2._deriv(calc_d2)
     for k1 in range(self._kernel1._r):
-      self._cov._dU[:, self._offset + k1 * self._kernel2._r:self._offset +
-        (k1 + 1) * self._kernel2._r] = self._kernel1._cov._dU[:, k1,
-        None] * self._kernel2._cov.U + self._kernel1._cov.U[:, k1,
-        None] * self._kernel2._cov._dU
+      self._cov._dU[
+        :,
+        self._offset + k1 * self._kernel2._r : self._offset
+        + (k1 + 1) * self._kernel2._r,
+      ] = (
+        self._kernel1._cov._dU[:, k1, None] * self._kernel2._cov.U
+        + self._kernel1._cov.U[:, k1, None] * self._kernel2._cov._dU
+      )
       if calc_d2:
-        self._cov._dV[:, self._offset + k1 * self._kernel2._r:self._offset +
-          (k1 + 1) * self._kernel2._r] = self._kernel1._cov._dV[:, k1,
-          None] * self._kernel2._cov.V + self._kernel1._cov.V[:, k1,
-          None] * self._kernel2._cov._dV
+        self._cov._dV[
+          :,
+          self._offset + k1 * self._kernel2._r : self._offset
+          + (k1 + 1) * self._kernel2._r,
+        ] = (
+          self._kernel1._cov._dV[:, k1, None] * self._kernel2._cov.V
+          + self._kernel1._cov.V[:, k1, None] * self._kernel2._cov._dV
+        )
 
-  def _deriv_t2(self,
+  def _deriv_t2(
+    self,
     t2,
     dt2,
     dU2,
     V2,
     phi2,
     ref2left,
     dt2left,
     dt2right,
     phi2left,
     phi2right,
-    dV2=None):
-
+    dV2=None,
+  ):
     kernel1_U2 = np.empty((t2.size, self._kernel1._r))
     kernel1_dU2 = np.empty((t2.size, self._kernel1._r))
     kernel1_V2 = np.empty((t2.size, self._kernel1._r))
     if dV2 is None:
       kernel1_dV2 = None
     else:
       kernel1_dV2 = np.empty((t2.size, self._kernel1._r))
     kernel1_phi2 = np.empty((t2.size - 1, self._kernel1._r))
     kernel1_phi2left = np.empty((t2.size, self._kernel1._r))
     kernel1_phi2right = np.empty((t2.size, self._kernel1._r))
-    self._kernel1._compute_t2(t2, dt2, kernel1_U2, kernel1_V2, kernel1_phi2,
-      ref2left, dt2left, dt2right, kernel1_phi2left, kernel1_phi2right)
-    self._kernel1._deriv_t2(t2, dt2, kernel1_dU2, kernel1_V2, kernel1_phi2,
-      ref2left, dt2left, dt2right, kernel1_phi2left, kernel1_phi2right,
-      kernel1_dV2)
+    self._kernel1._compute_t2(
+      t2,
+      dt2,
+      kernel1_U2,
+      kernel1_V2,
+      kernel1_phi2,
+      ref2left,
+      dt2left,
+      dt2right,
+      kernel1_phi2left,
+      kernel1_phi2right,
+    )
+    self._kernel1._deriv_t2(
+      t2,
+      dt2,
+      kernel1_dU2,
+      kernel1_V2,
+      kernel1_phi2,
+      ref2left,
+      dt2left,
+      dt2right,
+      kernel1_phi2left,
+      kernel1_phi2right,
+      kernel1_dV2,
+    )
 
     kernel2_U2 = np.empty((t2.size, self._kernel2._r))
     kernel2_dU2 = np.empty((t2.size, self._kernel2._r))
     kernel2_V2 = np.empty((t2.size, self._kernel2._r))
     if dV2 is None:
       kernel2_dV2 = None
     else:
       kernel2_dV2 = np.empty((t2.size, self._kernel2._r))
     kernel2_phi2 = np.empty((t2.size - 1, self._kernel2._r))
     kernel2_phi2left = np.empty((t2.size, self._kernel2._r))
     kernel2_phi2right = np.empty((t2.size, self._kernel2._r))
-    self._kernel2._compute_t2(t2, dt2, kernel2_U2, kernel2_V2, kernel2_phi2,
-      ref2left, dt2left, dt2right, kernel2_phi2left, kernel2_phi2right)
-    self._kernel2._deriv_t2(t2, dt2, kernel2_dU2, kernel2_V2, kernel2_phi2,
-      ref2left, dt2left, dt2right, kernel2_phi2left, kernel2_phi2right,
-      kernel2_dV2)
+    self._kernel2._compute_t2(
+      t2,
+      dt2,
+      kernel2_U2,
+      kernel2_V2,
+      kernel2_phi2,
+      ref2left,
+      dt2left,
+      dt2right,
+      kernel2_phi2left,
+      kernel2_phi2right,
+    )
+    self._kernel2._deriv_t2(
+      t2,
+      dt2,
+      kernel2_dU2,
+      kernel2_V2,
+      kernel2_phi2,
+      ref2left,
+      dt2left,
+      dt2right,
+      kernel2_phi2left,
+      kernel2_phi2right,
+      kernel2_dV2,
+    )
 
     for k1 in range(self._kernel1._r):
-      dU2[:, self._offset + k1 * self._kernel2._r:self._offset +
-        (k1 + 1) * self._kernel2._r] = kernel1_dU2[:, k1,
-        None] * kernel2_U2 + kernel1_U2[:, k1, None] * kernel2_dU2
-      V2[:, self._offset + k1 * self._kernel2._r:self._offset +
-        (k1 + 1) * self._kernel2._r] = kernel1_V2[:, k1, None] * kernel2_V2
-      phi2[:, self._offset + k1 * self._kernel2._r:self._offset +
-        (k1 + 1) * self._kernel2._r] = kernel1_phi2[:, k1, None] * kernel2_phi2
-      phi2left[:,
-        self._offset + k1 * self._kernel2._r:self._offset + (k1 + 1) *
-        self._kernel2._r] = kernel1_phi2left[:, k1, None] * kernel2_phi2left
-      phi2right[:,
-        self._offset + k1 * self._kernel2._r:self._offset + (k1 + 1) *
-        self._kernel2._r] = kernel1_phi2right[:, k1, None] * kernel2_phi2right
+      dU2[
+        :,
+        self._offset + k1 * self._kernel2._r : self._offset
+        + (k1 + 1) * self._kernel2._r,
+      ] = kernel1_dU2[:, k1, None] * kernel2_U2 + kernel1_U2[:, k1, None] * kernel2_dU2
+      V2[
+        :,
+        self._offset + k1 * self._kernel2._r : self._offset
+        + (k1 + 1) * self._kernel2._r,
+      ] = kernel1_V2[:, k1, None] * kernel2_V2
+      phi2[
+        :,
+        self._offset + k1 * self._kernel2._r : self._offset
+        + (k1 + 1) * self._kernel2._r,
+      ] = kernel1_phi2[:, k1, None] * kernel2_phi2
+      phi2left[
+        :,
+        self._offset + k1 * self._kernel2._r : self._offset
+        + (k1 + 1) * self._kernel2._r,
+      ] = kernel1_phi2left[:, k1, None] * kernel2_phi2left
+      phi2right[
+        :,
+        self._offset + k1 * self._kernel2._r : self._offset
+        + (k1 + 1) * self._kernel2._r,
+      ] = kernel1_phi2right[:, k1, None] * kernel2_phi2right
       if dV2 is not None:
-        dV2[:, self._offset + k1 * self._kernel2._r:self._offset +
-          (k1 + 1) * self._kernel2._r] = kernel1_dV2[:, k1,
-          None] * kernel2_V2 + kernel1_V2[:, k1, None] * kernel2_dV2
+        dV2[
+          :,
+          self._offset + k1 * self._kernel2._r : self._offset
+          + (k1 + 1) * self._kernel2._r,
+        ] = (
+          kernel1_dV2[:, k1, None] * kernel2_V2 + kernel1_V2[:, k1, None] * kernel2_dV2
+        )
 
   def eval(self, dt, series_id=(0, 0)):
-    return (self._kernel1.eval(dt, series_id) *
-      self._kernel2.eval(dt, series_id))
+    return self._kernel1.eval(dt, series_id) * self._kernel2.eval(dt, series_id)
 
 
 class SimpleProductKernel(ProductKernel):
-  r"""
-  """
+  r""" """
 
   def __init__(self, **kwargs):
     assert len(kwargs) == 2
     self._kerneldic = kwargs
     super().__init__(*kwargs.values())
-    self._param = [
-      f'{kern}_{key}' for kern in kwargs for key in kwargs[kern]._param
-    ]
+    self._param = [f'{kern}_{key}' for kern in kwargs for key in kwargs[kern]._param]
 
   def _kernel_param(self, **kwargs):
     paramKern = {kern: {} for kern in self._kerneldic}
     for par in kwargs:
       kern, key = par.split('_', 1)
       paramKern[kern][key] = kwargs[par]
-    return (paramKern.values())
+    return paramKern.values()
 
   def _kernel_param_back(self, *args):
     grad = {}
     for kern, gk in zip(self._kerneldic, args):
       for key in gk:
         grad[f'{kern}_{key}'] = gk[key]
-    return (grad)
+    return grad
 
   def _get_param(self, par):
     kern, key = par.split('_', 1)
-    return (self._kerneldic[kern]._get_param(key))
+    return self._kerneldic[kern]._get_param(key)
 
   def set_conditional_coef(self, **kwargs):
     r"""
     Set the coefficients used for the conditional computations.
     """
     paramKern = {kern: {} for kern in self._kerneldic}
     for par in kwargs:
@@ -1338,23 +1602,19 @@
           paramKern[kern][par] = kwargs[par]
       else:
         kern, key = par.split('_', 1)
         paramKern[kern][key] = kwargs[par]
     for kern in self._kerneldic:
       self._kerneldic[kern].set_conditional_coef(**paramKern[kern])
 
-class TransformKernel(Kernel):
 
+class TransformKernel(Kernel):
   def __init__(
-      self,
-      inner_kernel,
-      translate_param,
-      translate_param_back=None,
-      **kwargs):
-
+    self, inner_kernel, translate_param, translate_param_back=None, **kwargs
+  ):
     super().__init__()
     self._value = kwargs
     self._translate_param = translate_param
     self._translate_param_back = translate_param_back
     self._kernel = inner_kernel
     self._kernel._set_param(**self._translate_param(**self._value))
     self._r = self._kernel._r
@@ -1364,45 +1624,47 @@
     super()._link(cov, offset)
     self._kernel._link(cov, offset)
 
   def _compute(self):
     self._kernel._compute()
 
   def _get_param(self, par):
-    return (self._value[par])
+    return self._value[par]
 
   def _set_param(self, *args, **kwargs):
     for karg, arg in enumerate(args):
       par = self._param[karg]
       if par in kwargs:
         raise Exception(
-          f'TransformKernel._set_param: parameter {par} multiply defined.')
+          f'TransformKernel._set_param: parameter {par} multiply defined.'
+        )
       kwargs[par] = arg
     self._value.update(kwargs)
     self._kernel._set_param(**self._translate_param(**self._value))
 
   def _grad_param(self, grad_dU=None, grad_dV=None):
     grad_kernel = self._kernel._grad_param(grad_dU, grad_dV)
-    return (self._translate_param_back(grad_kernel))
+    return self._translate_param_back(grad_kernel)
 
   def set_conditional_coef(self, *args, **kwargs):
     r"""
     Set the coefficients used for the conditional computations.
     """
 
     self._kernel.set_conditional_coef(*args, **kwargs)
 
-  def _compute_t2(self, t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right,
-    phi2left, phi2right):
-
-    self._kernel._compute_t2(t2, dt2, U2, V2, phi2, ref2left, dt2left,
-      dt2right, phi2left, phi2right)
+  def _compute_t2(
+    self, t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right, phi2left, phi2right
+  ):
+    self._kernel._compute_t2(
+      t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right, phi2left, phi2right
+    )
 
   def eval(self, dt, series_id=(0, 0)):
-    return (self._kernel.eval(dt, series_id))
+    return self._kernel.eval(dt, series_id)
 
 
 class USHOKernel(QuasiperiodicKernel):
   r"""
   Under-damped SHO Kernel.
 
   This kernel follows the differential equation of
@@ -1449,22 +1711,28 @@
     a, b, la, nu = self._getcoefs()
     super()._set_param(a, b, la, nu)
 
   def _grad_param(self, grad_dU=None, grad_dV=None):
     gradQP = super()._grad_param(grad_dU, grad_dV)
     grad = {}
     grad['sig'] = 2 * self._sig * (gradQP['a'] + gradQP['b'] / self._sqQ)
-    grad['P0'] = -np.pi / (self._P0**2 * self._Q) * (gradQP['la'] +
-      gradQP['nu'] * self._sqQ)
-    grad['Q'] = -np.pi / (self._P0 * self._Q**2) * (gradQP['la'] +
-      gradQP['nu'] * self._sqQ)
+    grad['P0'] = (
+      -np.pi / (self._P0**2 * self._Q) * (gradQP['la'] + gradQP['nu'] * self._sqQ)
+    )
+    grad['Q'] = (
+      -np.pi / (self._P0 * self._Q**2) * (gradQP['la'] + gradQP['nu'] * self._sqQ)
+    )
     if 4 * self._Q**2 - 1 > self._eps:
-      grad['Q'] += 4 * self._Q / self._sqQ * (gradQP['nu'] * self._la -
-        gradQP['b'] * self._a / self._sqQ**2)
-    return (grad)
+      grad['Q'] += (
+        4
+        * self._Q
+        / self._sqQ
+        * (gradQP['nu'] * self._la - gradQP['b'] * self._a / self._sqQ**2)
+      )
+    return grad
 
 
 class OSHOKernel(SumKernel):
   r"""
   Over-damped SHO Kernel.
 
   This kernel follows the differential equation of
@@ -1496,40 +1764,62 @@
     super().__init__(self._exp1, self._exp2)
     self._param = ['sig', 'P0', 'Q']
 
   def _getcoefs(self):
     self._sqQ = np.sqrt(max(1 - 4 * self._Q**2, self._eps))
     self._a = self._sig**2
     self._la = np.pi / (self._P0 * self._Q)
-    return (self._a * (1 + 1 / self._sqQ) / 2, self._la * (1 - self._sqQ),
-      self._a * (1 - 1 / self._sqQ) / 2, self._la * (1 + self._sqQ))
+    return (
+      self._a * (1 + 1 / self._sqQ) / 2,
+      self._la * (1 - self._sqQ),
+      self._a * (1 - 1 / self._sqQ) / 2,
+      self._la * (1 + self._sqQ),
+    )
 
   def _kernel_param(self, sig=None, P0=None, Q=None):
     if sig is not None:
       self._sig = sig
     if P0 is not None:
       self._P0 = P0
     if Q is not None:
       self._Q = Q
     a1, la1, a2, la2 = self._getcoefs()
     return (dict(a=a1, la=la1), dict(a=a2, la=la2))
 
   def _kernel_param_back(self, gradExp1, gradExp2):
     grad = {}
-    grad['sig'] = 2 * self._sig * (gradExp1['a'] *
-      (1 + 1 / self._sqQ) / 2 + gradExp2['a'] * (1 - 1 / self._sqQ) / 2)
-    grad['P0'] = -np.pi / (self._P0**2 * self._Q) * (gradExp1['la'] *
-      (1 - self._sqQ) + gradExp2['la'] * (1 + self._sqQ))
-    grad['Q'] = -np.pi / (self._P0 * self._Q**2) * (gradExp1['la'] *
-      (1 - self._sqQ) + gradExp2['la'] * (1 + self._sqQ))
+    grad['sig'] = (
+      2
+      * self._sig
+      * (
+        gradExp1['a'] * (1 + 1 / self._sqQ) / 2
+        + gradExp2['a'] * (1 - 1 / self._sqQ) / 2
+      )
+    )
+    grad['P0'] = (
+      -np.pi
+      / (self._P0**2 * self._Q)
+      * (gradExp1['la'] * (1 - self._sqQ) + gradExp2['la'] * (1 + self._sqQ))
+    )
+    grad['Q'] = (
+      -np.pi
+      / (self._P0 * self._Q**2)
+      * (gradExp1['la'] * (1 - self._sqQ) + gradExp2['la'] * (1 + self._sqQ))
+    )
     if 1 - 4 * self._Q**2 > self._eps:
-      grad['Q'] -= 4 * self._Q / self._sqQ * (
-        (gradExp2['a'] - gradExp1['a']) * self._a / (2 * self._sqQ**2) +
-        (gradExp2['la'] - gradExp1['la']) * self._la)
-    return (grad)
+      grad['Q'] -= (
+        4
+        * self._Q
+        / self._sqQ
+        * (
+          (gradExp2['a'] - gradExp1['a']) * self._a / (2 * self._sqQ**2)
+          + (gradExp2['la'] - gradExp1['la']) * self._la
+        )
+      )
+    return grad
 
 
 class SHOKernel(Kernel):
   r"""
   SHO Kernel.
 
   This kernel follows the differential equation of
@@ -1583,57 +1873,64 @@
     if self._Q > 0.5:
       self._usho._set_param(self._sig, self._P0, self._Q)
     else:
       self._osho._set_param(self._sig, self._P0, self._Q)
 
   def _grad_param(self, grad_dU=None, grad_dV=None):
     if self._Q > 0.5:
-      return (self._usho._grad_param(grad_dU, grad_dV))
+      return self._usho._grad_param(grad_dU, grad_dV)
     else:
-      return (self._osho._grad_param(grad_dU, grad_dV))
+      return self._osho._grad_param(grad_dU, grad_dV)
 
-  def _compute_t2(self, t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right,
-    phi2left, phi2right):
+  def _compute_t2(
+    self, t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right, phi2left, phi2right
+  ):
     if self._Q > 0.5:
-      self._usho._compute_t2(t2, dt2, U2, V2, phi2, ref2left, dt2left,
-        dt2right, phi2left, phi2right)
-    else:
-      self._osho._compute_t2(t2, dt2, U2, V2, phi2, ref2left, dt2left,
-        dt2right, phi2left, phi2right)
+      self._usho._compute_t2(
+        t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right, phi2left, phi2right
+      )
+    else:
+      self._osho._compute_t2(
+        t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right, phi2left, phi2right
+      )
 
   def _deriv(self, calc_d2=False):
     if self._Q > 0.5:
       self._usho._deriv(calc_d2)
     else:
       self._osho._deriv(calc_d2)
 
-  def _deriv_t2(self,
+  def _deriv_t2(
+    self,
     t2,
     dt2,
     dU2,
     V2,
     phi2,
     ref2left,
     dt2left,
     dt2right,
     phi2left,
     phi2right,
-    dV2=None):
+    dV2=None,
+  ):
     if self._Q > 0.5:
-      self._usho._deriv_t2(t2, dt2, dU2, V2, phi2, ref2left, dt2left, dt2right,
-        phi2left, phi2right, dV2)
-    else:
-      self._osho._deriv_t2(t2, dt2, dU2, V2, phi2, ref2left, dt2left, dt2right,
-        phi2left, phi2right, dV2)
+      self._usho._deriv_t2(
+        t2, dt2, dU2, V2, phi2, ref2left, dt2left, dt2right, phi2left, phi2right, dV2
+      )
+    else:
+      self._osho._deriv_t2(
+        t2, dt2, dU2, V2, phi2, ref2left, dt2left, dt2right, phi2left, phi2right, dV2
+      )
 
   def eval(self, dt, series_id=None):
     if self._Q > 0.5:
-      return (self._usho.eval(dt))
+      return self._usho.eval(dt)
     else:
-      return (self._osho.eval(dt))
+      return self._osho.eval(dt)
 
 
 class MEPKernel(SumKernel):
   r"""
   The Matérn 3/2 exponential periodic (MEP) kernel
   is a rank 6 kernel roughly approximating
   the squared-exponential periodic (SEP) kernel.
@@ -1713,35 +2010,43 @@
     if P is not None:
       self._P = P
     if rho is not None:
       self._rho = rho
     if eta is not None:
       self._eta = eta
     sig0, a1, a2, b1, b2, la, nu = self._getcoefs()
-    return (dict(sig=sig0, rho=self._rho), dict(a=a1, b=b1, la=la,
-      nu=nu), dict(a=a2, b=b2, la=la, nu=2 * nu))
+    return (
+      dict(sig=sig0, rho=self._rho),
+      dict(a=a1, b=b1, la=la, nu=nu),
+      dict(a=a2, b=b2, la=la, nu=2 * nu),
+    )
 
   def _kernel_param_back(self, gradMat, gradQP1, gradQP2):
     sgs0 = self._mat._sig * gradMat['sig']
     aga1 = self._qp1._a * gradQP1['a']
     aga2 = self._qp2._a * gradQP2['a']
     bgb1 = self._qp1._b * gradQP1['b']
     bgb2 = self._qp2._b * gradQP2['b']
     bgb = bgb1 + bgb2
     sgs = sgs0 + 2 * (aga1 + aga2 + bgb)
 
     grad = {}
     grad['sig'] = sgs / self._sig
-    grad['P'] = (bgb - self._qp1._nu * gradQP1['nu'] -
-      self._qp2._nu * gradQP2['nu']) / self._P
-    grad['rho'] = gradMat['rho'] - (bgb + self._qp1._la *
-      (gradQP1['la'] + gradQP2['la'])) / self._rho
-    grad['eta'] = (sgs * (self._f + self._f2 / 2) / self._deno - 2 *
-      (aga1 + bgb1 + 2 * (aga2 + bgb2))) / self._eta
-    return (grad)
+    grad['P'] = (
+      bgb - self._qp1._nu * gradQP1['nu'] - self._qp2._nu * gradQP2['nu']
+    ) / self._P
+    grad['rho'] = (
+      gradMat['rho']
+      - (bgb + self._qp1._la * (gradQP1['la'] + gradQP2['la'])) / self._rho
+    )
+    grad['eta'] = (
+      sgs * (self._f + self._f2 / 2) / self._deno
+      - 2 * (aga1 + bgb1 + 2 * (aga2 + bgb2))
+    ) / self._eta
+    return grad
 
 
 class ESKernel(SumKernel):
   r"""
   The Exponential-sine (ES) kernel is a rank 3
   twice mean-square differentiable kernel
   approximating the squared-exponential (SE) kernel.
@@ -1771,20 +2076,15 @@
     from the SE kernel is below 0.9%.
   mu : float
     Coefficient :math:`\mu`.
     The default value  is chosen such as the deviation
     from the SE kernel is below 0.9%.
   """
 
-  def __init__(self,
-    sig,
-    rho,
-    coef_la=1.0907260149419182,
-    mu=1.326644517327145):
-
+  def __init__(self, sig, rho, coef_la=1.0907260149419182, mu=1.326644517327145):
     self._sig = sig
     self._rho = rho
 
     self._coef_la = coef_la
     self._mu = mu
     self._coef_b = 1 / self._mu
     self._coef_a0 = 2 / 3 * (1 + self._coef_b**2)
@@ -1811,19 +2111,29 @@
     if rho is not None:
       self._rho = rho
     a0, a, b, la, nu = self._getcoefs()
     return (dict(a=a0, la=la), dict(a=a, b=b, la=la, nu=nu))
 
   def _kernel_param_back(self, gradExp, gradQP):
     grad = {}
-    grad['sig'] = 2 / self._sig * (gradExp['a'] * self._exp._a +
-      gradQP['a'] * self._qp._a + gradQP['b'] * self._qp._b)
-    grad['rho'] = -self._exp._la / self._rho * (gradExp['la'] + gradQP['la'] +
-      self._mu * gradQP['nu'])
-    return (grad)
+    grad['sig'] = (
+      2
+      / self._sig
+      * (
+        gradExp['a'] * self._exp._a
+        + gradQP['a'] * self._qp._a
+        + gradQP['b'] * self._qp._b
+      )
+    )
+    grad['rho'] = (
+      -self._exp._la
+      / self._rho
+      * (gradExp['la'] + gradQP['la'] + self._mu * gradQP['nu'])
+    )
+    return grad
 
 
 class _ESP_PKernel(SumKernel):
   r"""
   Periodic part of the :class:`ESPKernel`.
 
   Warnings
@@ -1834,16 +2144,15 @@
   def __init__(self, P, eta, nharm):
     self._P = P
     self._eta = eta
     self._nharm = nharm
     self._bessel = np.empty(self._nharm + 1)
     self._calccoefs()
     kernels = [ExponentialKernel(self._a[0], 0)] + [
-      QuasiperiodicKernel(self._a[k], 0, 0, k * self._nu)
-      for k in range(1, nharm + 1)
+      QuasiperiodicKernel(self._a[k], 0, 0, k * self._nu) for k in range(1, nharm + 1)
     ]
     super().__init__(*kernels)
     self._param = ['P', 'eta']
 
   def _calccoefs(self):
     self._eta2 = self._eta * self._eta
     self._f = 1 / (4 * self._eta2)
@@ -1857,33 +2166,36 @@
 
   def _kernel_param(self, P=None, eta=None):
     if P is not None:
       self._P = P
     if eta is not None:
       self._eta = eta
     self._calccoefs()
-    return ([dict(a=self._a[0])] +
-      [dict(a=self._a[k], nu=k * self._nu) for k in range(1, self._nharm + 1)])
+    return [dict(a=self._a[0])] + [
+      dict(a=self._a[k], nu=k * self._nu) for k in range(1, self._nharm + 1)
+    ]
 
   def _kernel_param_back(self, *gradkernels):
     grad = {}
-    grad['P'] = -np.sum([
-      self._kernels[k]._nu * gradkernels[k]['nu']
-      for k in range(1, self._nharm + 1)
-    ]) / self._P
+    grad['P'] = (
+      -np.sum(
+        [self._kernels[k]._nu * gradkernels[k]['nu'] for k in range(1, self._nharm + 1)]
+      )
+      / self._P
+    )
 
     ga = np.array([gk['a'] for gk in gradkernels])
     # Use recurrence relations for derivative of Bessel functions:
     da_df = self._bessel[1:] / 2
     da_df[1:] += self._bessel[:-2] / 2
     ddeno_df = np.sum(da_df)
     da_df = (da_df - self._a * ddeno_df) / self._deno
     df_deta = -2 * self._f / self._eta
     grad['eta'] = df_deta * (da_df @ ga)
-    return (grad)
+    return grad
 
 
 class ESPKernel(ProductKernel):
   r"""
   The Exponential-sine periodic (ESP) kernel is a
   twice mean-square differentiable kernel
   approximating the squared-exponential periodic (SEP) kernel.
@@ -1936,15 +2248,15 @@
     if rho is not None:
       self._rho = rho
     if eta is not None:
       self._eta = eta
     return (dict(sig=sig, rho=rho), dict(P=P, eta=eta))
 
   def _kernel_param_back(self, gradES, gradP):
-    return ({**gradES, **gradP})
+    return {**gradES, **gradP}
 
 
 class MultiSeriesKernel(Kernel):
   r"""
   Linear combination of a Kernel and its derivative
   applied to heterogenous time series.
 
@@ -2000,106 +2312,122 @@
     self._kernel._link(_FakeCov(cov.t, cov.dt, self._r), 0)
 
   def _compute(self):
     self._kernel._cov.A[:] = 0
     self._kernel._compute()
     if self._with_derivative:
       self._kernel._deriv(True)
-      self._kernel._cov._B = np.sum(self._kernel._cov._dU *
-        self._kernel._cov._dV,
-        axis=1)
+      self._kernel._cov._B = np.sum(
+        self._kernel._cov._dU * self._kernel._cov._dV, axis=1
+      )
     for k in range(self._nseries):
       ik = self._series_index[k]
       # cov(GP, GP)
-      self._cov.A[ik] += self._alpha[k]**2 * self._kernel._cov.A[ik]
-      self._cov.U[ik, self._offset:self._offset +
-        self._r] = self._alpha[k] * self._kernel._cov.U[ik]
-      self._cov.V[ik, self._offset:self._offset +
-        self._r] = self._alpha[k] * self._kernel._cov.V[ik]
+      self._cov.A[ik] += self._alpha[k] ** 2 * self._kernel._cov.A[ik]
+      self._cov.U[ik, self._offset : self._offset + self._r] = (
+        self._alpha[k] * self._kernel._cov.U[ik]
+      )
+      self._cov.V[ik, self._offset : self._offset + self._r] = (
+        self._alpha[k] * self._kernel._cov.V[ik]
+      )
       if self._with_derivative:
         # cov(GP, dGP), cov(dGP, GP), cov(dGP, dGP)
-        self._cov.A[ik] += self._beta[k]**2 * self._kernel._cov._B[ik]
-        self._cov.U[ik, self._offset:self._offset +
-          self._r] += self._beta[k] * self._kernel._cov._dU[ik]
-        self._cov.V[ik, self._offset:self._offset +
-          self._r] += self._beta[k] * self._kernel._cov._dV[ik]
-    self._cov.phi[:,
-      self._offset:self._offset + self._r] = self._kernel._cov.phi
+        self._cov.A[ik] += self._beta[k] ** 2 * self._kernel._cov._B[ik]
+        self._cov.U[ik, self._offset : self._offset + self._r] += (
+          self._beta[k] * self._kernel._cov._dU[ik]
+        )
+        self._cov.V[ik, self._offset : self._offset + self._r] += (
+          self._beta[k] * self._kernel._cov._dV[ik]
+        )
+    self._cov.phi[:, self._offset : self._offset + self._r] = self._kernel._cov.phi
 
   def _set_param(self, *args, **kwargs):
     for karg, arg in enumerate(args):
       par = self._param[karg]
       if par in kwargs:
         raise Exception(
-          f'MultiSeriesKernel._set_param: parameter {par} multiply defined.')
+          f'MultiSeriesKernel._set_param: parameter {par} multiply defined.'
+        )
       kwargs[par] = arg
     kernel_kwargs = {}
     for par in kwargs:
       if par.startswith('alpha_'):
         self._alpha[int(par.replace('alpha_', ''))] = kwargs[par]
       elif par.startswith('beta_'):
         self._beta[int(par.replace('beta_', ''))] = kwargs[par]
       else:
         kernel_kwargs[par] = kwargs[par]
     self._kernel._set_param(**kernel_kwargs)
 
   def _get_param(self, par):
     if par.startswith('alpha_'):
-      return (self._alpha[int(par.replace('alpha_', ''))])
+      return self._alpha[int(par.replace('alpha_', ''))]
     elif par.startswith('beta_'):
-      return (self._beta[int(par.replace('beta_', ''))])
+      return self._beta[int(par.replace('beta_', ''))]
     else:
-      return (self._kernel._get_param(par))
+      return self._kernel._get_param(par)
 
   def _grad_param(self):
     grad = {}
     for k in range(self._nseries):
       ik = self._series_index[k]
       # cov(GP, GP)
-      grad[f'alpha_{k}'] = 2 * self._alpha[k] * np.sum(
-        self._cov._grad_A[ik] * self._kernel._cov.A[ik])
-      grad[f'alpha_{k}'] += np.sum(self._cov._grad_U[ik,
-        self._offset:self._offset + self._r] * self._kernel._cov.U[ik] +
-        self._cov._grad_V[ik, self._offset:self._offset + self._r] *
-        self._kernel._cov.V[ik])
-      self._kernel._cov._grad_A[ik] = self._alpha[k]**2 * self._cov._grad_A[ik]
-      self._kernel._cov._grad_U[ik] = self._alpha[k] * self._cov._grad_U[ik,
-        self._offset:self._offset + self._r]
-      self._kernel._cov._grad_V[ik] = self._alpha[k] * self._cov._grad_V[ik,
-        self._offset:self._offset + self._r]
+      grad[f'alpha_{k}'] = (
+        2 * self._alpha[k] * np.sum(self._cov._grad_A[ik] * self._kernel._cov.A[ik])
+      )
+      grad[f'alpha_{k}'] += np.sum(
+        self._cov._grad_U[ik, self._offset : self._offset + self._r]
+        * self._kernel._cov.U[ik]
+        + self._cov._grad_V[ik, self._offset : self._offset + self._r]
+        * self._kernel._cov.V[ik]
+      )
+      self._kernel._cov._grad_A[ik] = self._alpha[k] ** 2 * self._cov._grad_A[ik]
+      self._kernel._cov._grad_U[ik] = (
+        self._alpha[k] * self._cov._grad_U[ik, self._offset : self._offset + self._r]
+      )
+      self._kernel._cov._grad_V[ik] = (
+        self._alpha[k] * self._cov._grad_V[ik, self._offset : self._offset + self._r]
+      )
       if self._with_derivative:
         # cov(GP, dGP), cov(dGP, GP), cov(dGP, dGP)
-        grad[f'beta_{k}'] = 2 * self._beta[k] * np.sum(
-          self._cov._grad_A[ik] * self._kernel._cov._B[ik])
-        grad[f'beta_{k}'] += np.sum(self._cov._grad_U[ik,
-          self._offset:self._offset + self._r] * self._kernel._cov._dU[ik] +
-          self._cov._grad_V[ik, self._offset:self._offset + self._r] *
-          self._kernel._cov._dV[ik])
-        self._kernel._cov._grad_B[
-          ik] = self._beta[k]**2 * self._cov._grad_A[ik]
-        self._kernel._cov._grad_dU[ik] = self._beta[k] * self._cov._grad_U[ik,
-          self._offset:self._offset + self._r]
-        self._kernel._cov._grad_dV[ik] = self._beta[k] * self._cov._grad_V[ik,
-          self._offset:self._offset + self._r]
-    self._kernel._cov._grad_phi = self._cov._grad_phi[:,
-      self._offset:self._offset + self._r]
+        grad[f'beta_{k}'] = (
+          2 * self._beta[k] * np.sum(self._cov._grad_A[ik] * self._kernel._cov._B[ik])
+        )
+        grad[f'beta_{k}'] += np.sum(
+          self._cov._grad_U[ik, self._offset : self._offset + self._r]
+          * self._kernel._cov._dU[ik]
+          + self._cov._grad_V[ik, self._offset : self._offset + self._r]
+          * self._kernel._cov._dV[ik]
+        )
+        self._kernel._cov._grad_B[ik] = self._beta[k] ** 2 * self._cov._grad_A[ik]
+        self._kernel._cov._grad_dU[ik] = (
+          self._beta[k] * self._cov._grad_U[ik, self._offset : self._offset + self._r]
+        )
+        self._kernel._cov._grad_dV[ik] = (
+          self._beta[k] * self._cov._grad_V[ik, self._offset : self._offset + self._r]
+        )
+    self._kernel._cov._grad_phi = self._cov._grad_phi[
+      :, self._offset : self._offset + self._r
+    ]
 
     self._kernel._cov._sum_grad_A = np.sum(self._kernel._cov._grad_A)
     if self._with_derivative:
-      self._kernel._cov._grad_dU += self._kernel._cov._dV * self._kernel._cov._grad_B[:,
-        None]
-      self._kernel._cov._grad_dV += self._kernel._cov._dU * self._kernel._cov._grad_B[:,
-        None]
+      self._kernel._cov._grad_dU += (
+        self._kernel._cov._dV * self._kernel._cov._grad_B[:, None]
+      )
+      self._kernel._cov._grad_dV += (
+        self._kernel._cov._dU * self._kernel._cov._grad_B[:, None]
+      )
       grad.update(
-        self._kernel._grad_param(self._kernel._cov._grad_dU,
-        self._kernel._cov._grad_dV))
+        self._kernel._grad_param(self._kernel._cov._grad_dU, self._kernel._cov._grad_dV)
+      )
     else:
       grad.update(self._kernel._grad_param())
 
-    return (grad)
+    return grad
 
   def set_conditional_coef(self, alpha=1, beta=0, series_id=None):
     r"""
     Set the coefficients used for the conditional computations.
 
     Parameters
     ----------
@@ -2123,80 +2451,104 @@
 
   def set_conditionnal_coef(self, *args, **kwargs):
     r"""
     Same as the :func:`set_conditional_coef` method (here for backward-compatibility).
     """
 
     warnings.warn(
-      "Please use the set_conditional_coef method (with a single n).",
-      DeprecationWarning)
+      'Please use the set_conditional_coef method (with a single n).',
+      DeprecationWarning,
+    )
     self.set_conditional_coef(*args, **kwargs)
 
-  def _compute_t2(self, t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right,
-    phi2left, phi2right):
-
+  def _compute_t2(
+    self, t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right, phi2left, phi2right
+  ):
     if self._cond_series_id is None:
       alpha = self._cond_alpha
       if self._with_derivative:
         beta = self._cond_beta
     else:
       alpha = self._alpha[self._cond_series_id]
       if self._with_derivative:
         beta = self._beta[self._cond_series_id]
 
     kernel_U2 = np.empty((t2.size, self._r))
     kernel_V2 = np.empty((t2.size, self._r))
     kernel_phi2 = np.empty((t2.size - 1, self._r))
     kernel_phi2left = np.empty((t2.size, self._r))
     kernel_phi2right = np.empty((t2.size, self._r))
-    self._kernel._compute_t2(t2, dt2, kernel_U2, kernel_V2, kernel_phi2,
-      ref2left, dt2left, dt2right, kernel_phi2left, kernel_phi2right)
+    self._kernel._compute_t2(
+      t2,
+      dt2,
+      kernel_U2,
+      kernel_V2,
+      kernel_phi2,
+      ref2left,
+      dt2left,
+      dt2right,
+      kernel_phi2left,
+      kernel_phi2right,
+    )
     # cov(GP, GP)
-    U2[:, self._offset:self._offset + self._r] = alpha * kernel_U2
-    V2[:, self._offset:self._offset + self._r] = alpha * kernel_V2
-    phi2[:, self._offset:self._offset + self._r] = kernel_phi2
-    phi2left[:, self._offset:self._offset + self._r] = kernel_phi2left
-    phi2right[:, self._offset:self._offset + self._r] = kernel_phi2right
+    U2[:, self._offset : self._offset + self._r] = alpha * kernel_U2
+    V2[:, self._offset : self._offset + self._r] = alpha * kernel_V2
+    phi2[:, self._offset : self._offset + self._r] = kernel_phi2
+    phi2left[:, self._offset : self._offset + self._r] = kernel_phi2left
+    phi2right[:, self._offset : self._offset + self._r] = kernel_phi2right
 
     if self._with_derivative and beta != 0:
       kernel_dU2 = np.empty((t2.size, self._r))
       kernel_dV2 = np.empty((t2.size, self._r))
-      self._kernel._deriv_t2(t2, dt2, kernel_dU2, kernel_V2, kernel_phi2,
-        ref2left, dt2left, dt2right, kernel_phi2left, kernel_phi2right,
-        kernel_dV2)
+      self._kernel._deriv_t2(
+        t2,
+        dt2,
+        kernel_dU2,
+        kernel_V2,
+        kernel_phi2,
+        ref2left,
+        dt2left,
+        dt2right,
+        kernel_phi2left,
+        kernel_phi2right,
+        kernel_dV2,
+      )
       # cov(GP, dGP), cov(dGP, GP), cov(dGP, dGP)
-      U2[:, self._offset:self._offset + self._r] += beta * kernel_dU2
-      V2[:, self._offset:self._offset + self._r] += beta * kernel_dV2
+      U2[:, self._offset : self._offset + self._r] += beta * kernel_dU2
+      V2[:, self._offset : self._offset + self._r] += beta * kernel_dV2
 
   def _deriv(self, calc_d2=False):
     if self._with_derivative:
       raise NotImplementedError()
     else:
       self._kernel._deriv(calc_d2)
       for k in range(self._nseries):
         ik = self._series_index[k]
-        self._cov._dU[ik, self._offset:self._offset +
-          self._r] = self._alpha[k] * self._kernel._cov._dU
+        self._cov._dU[ik, self._offset : self._offset + self._r] = (
+          self._alpha[k] * self._kernel._cov._dU
+        )
         if calc_d2:
-          self._cov._dV[ik, self._offset:self._offset +
-            self._r] = self._alpha[k] * self._kernel._cov._dV
+          self._cov._dV[ik, self._offset : self._offset + self._r] = (
+            self._alpha[k] * self._kernel._cov._dV
+          )
 
-  def _deriv_t2(self,
+  def _deriv_t2(
+    self,
     t2,
     dt2,
     dU2,
     V2,
     phi2,
     ref2left,
     dt2left,
     dt2right,
     phi2left,
     phi2right,
-    dV2=None):
-
+    dV2=None,
+  ):
     if self._with_derivative:
       raise NotImplementedError()
     else:
       if self._cond_series_id is None:
         alpha = self._cond_alpha
       else:
         alpha = self._alpha[self._cond_series_id]
@@ -2205,30 +2557,40 @@
       kernel_phi2 = np.empty((t2.size - 1, self._r))
       kernel_phi2left = np.empty((t2.size, self._r))
       kernel_phi2right = np.empty((t2.size, self._r))
       if dV2 is None:
         kernel_dV2 = None
       else:
         kernel_dV2 = np.empty((t2.size, self._r))
-      self._kernel._deriv_t2(t2, dt2, kernel_dU2, kernel_V2, kernel_phi2,
-        ref2left, dt2left, dt2right, kernel_phi2left, kernel_phi2right,
-        kernel_dV2)
-      dU2[:, self._offset:self._offset + self._r] = alpha * kernel_dU2
-      V2[:, self._offset:self._offset + self._r] = alpha * kernel_V2
+      self._kernel._deriv_t2(
+        t2,
+        dt2,
+        kernel_dU2,
+        kernel_V2,
+        kernel_phi2,
+        ref2left,
+        dt2left,
+        dt2right,
+        kernel_phi2left,
+        kernel_phi2right,
+        kernel_dV2,
+      )
+      dU2[:, self._offset : self._offset + self._r] = alpha * kernel_dU2
+      V2[:, self._offset : self._offset + self._r] = alpha * kernel_V2
       if dV2 is not None:
-        dV2[:, self._offset:self._offset + self._r] = alpha * kernel_dV2
+        dV2[:, self._offset : self._offset + self._r] = alpha * kernel_dV2
 
-      phi2[:, self._offset:self._offset + self._r] = kernel_phi2
-      phi2left[:, self._offset:self._offset + self._r] = kernel_phi2left
-      phi2right[:, self._offset:self._offset + self._r] = kernel_phi2right
+      phi2[:, self._offset : self._offset + self._r] = kernel_phi2
+      phi2left[:, self._offset : self._offset + self._r] = kernel_phi2left
+      phi2right[:, self._offset : self._offset + self._r] = kernel_phi2right
 
   def eval(self, dt, series_id=None):
     if series_id is not None:
       raise NotImplementedError()
-    return (self._kernel.eval(dt))
+    return self._kernel.eval(dt)
 
 
 class MultiFourierKernel(Kernel):
   r"""
   Multivariate Fourier series kernel.
 
   For :math:`m` times series (:math:`y_1,\dots y_m`), the covariance between
@@ -2278,78 +2640,94 @@
     self._cond_series_id = 0
     self._vectorize = vectorize
     if self._vectorize:
       param_alpha = ['alpha']
       param_beta = ['beta']
     else:
       param_alpha = [
-        f'alpha_{h}_{i}_{s}' for h in range(self._nfreq)
-        for i in range(self._nseries) for s in range(self._coef_rank)
+        f'alpha_{h}_{i}_{s}'
+        for h in range(self._nfreq)
+        for i in range(self._nseries)
+        for s in range(self._coef_rank)
       ]
       param_beta = [
-        f'beta_{h}_{i}_{s}' for h in range(self._nfreq)
-        for i in range(self._nseries) for s in range(self._coef_rank)
+        f'beta_{h}_{i}_{s}'
+        for h in range(self._nfreq)
+        for i in range(self._nseries)
+        for s in range(self._coef_rank)
       ]
     if self._nharm == 0:
       self._param = param_alpha
     else:
       self._param = ['P'] + param_alpha + param_beta
 
   def _compute(self):
     if self._nharm == 0:
       for k, ik in enumerate(self._series_index):
         self._cov.A[ik] += np.sum(self._alpha[0, k] * self._alpha[0, k])
-        self._cov.U[ik,
-          self._offset:self._offset + self._coef_rank] = self._alpha[0, k]
+        self._cov.U[ik, self._offset : self._offset + self._coef_rank] = self._alpha[
+          0, k
+        ]
     else:
       self._nu = 2 * np.pi / self._P
       self._nut = self._nu * self._cov.t
       self._cjnut = np.empty((self._cov.n, self._nharm))
       self._sjnut = np.empty((self._cov.n, self._nharm))
       self._cjnut[:, 0] = np.cos(self._nut)
       self._sjnut[:, 0] = np.sin(self._nut)
       for j in range(1, self._nharm):
-        self._cjnut[:, j] = self._cjnut[:, j - 1] * self._cjnut[:,
-          0] - self._sjnut[:, j - 1] * self._sjnut[:, 0]
-        self._sjnut[:, j] = self._sjnut[:, j - 1] * self._cjnut[:,
-          0] + self._cjnut[:, j - 1] * self._sjnut[:, 0]
+        self._cjnut[:, j] = (
+          self._cjnut[:, j - 1] * self._cjnut[:, 0]
+          - self._sjnut[:, j - 1] * self._sjnut[:, 0]
+        )
+        self._sjnut[:, j] = (
+          self._sjnut[:, j - 1] * self._cjnut[:, 0]
+          + self._cjnut[:, j - 1] * self._sjnut[:, 0]
+        )
 
       for k, ik in enumerate(self._series_index):
-        self._cov.A[ik] += np.sum(self._alpha[:, k] * self._alpha[:, k] +
-          self._beta[:, k] * self._beta[:, k])
-        self._cov.U[ik,
-          self._offset:self._offset + self._coef_rank] = self._alpha[0, k]
-        self._cov.U[ik, self._offset + self._coef_rank:self._offset +
-          self._nfreq * self._coef_rank] = (
-          self._alpha[1:, k] * self._cjnut[ik, :, np.newaxis] -
-          self._beta[1:, k] * self._sjnut[ik, :, np.newaxis]).reshape(
-          -1, self._nharm * self._coef_rank)
-        self._cov.U[ik,
-          self._offset + self._nfreq * self._coef_rank:self._offset +
-          self._r] = (self._alpha[1:, k] * self._sjnut[ik, :, np.newaxis] +
-          self._beta[1:, k] * self._cjnut[ik, :, np.newaxis]).reshape(
-          -1, self._nharm * self._coef_rank)
-    self._cov.V[:, self._offset:self._offset + self._r] = self._cov.U[:,
-      self._offset:self._offset + self._r]
-    self._cov.phi[:, self._offset:self._offset + self._r] = 1.0
+        self._cov.A[ik] += np.sum(
+          self._alpha[:, k] * self._alpha[:, k] + self._beta[:, k] * self._beta[:, k]
+        )
+        self._cov.U[ik, self._offset : self._offset + self._coef_rank] = self._alpha[
+          0, k
+        ]
+        self._cov.U[
+          ik,
+          self._offset + self._coef_rank : self._offset + self._nfreq * self._coef_rank,
+        ] = (
+          self._alpha[1:, k] * self._cjnut[ik, :, np.newaxis]
+          - self._beta[1:, k] * self._sjnut[ik, :, np.newaxis]
+        ).reshape(-1, self._nharm * self._coef_rank)
+        self._cov.U[
+          ik, self._offset + self._nfreq * self._coef_rank : self._offset + self._r
+        ] = (
+          self._alpha[1:, k] * self._sjnut[ik, :, np.newaxis]
+          + self._beta[1:, k] * self._cjnut[ik, :, np.newaxis]
+        ).reshape(-1, self._nharm * self._coef_rank)
+    self._cov.V[:, self._offset : self._offset + self._r] = self._cov.U[
+      :, self._offset : self._offset + self._r
+    ]
+    self._cov.phi[:, self._offset : self._offset + self._r] = 1.0
 
   def _get_param(self, par):
     if par.startswith('alpha_'):
-      return (self._alpha[tuple(int(s) for s in par.split('_')[1:])])
+      return self._alpha[tuple(int(s) for s in par.split('_')[1:])]
     elif par.startswith('beta_'):
-      return (self._beta[tuple(int(s) for s in par.split('_')[1:])])
+      return self._beta[tuple(int(s) for s in par.split('_')[1:])]
     else:
-      return (super()._get_param(par))
+      return super()._get_param(par)
 
   def _set_param(self, *args, **kwargs):
     for karg, arg in enumerate(args):
       par = self._param[karg]
       if par in kwargs:
         raise Exception(
-          f'MultiFourierKernel._set_param: parameter {par} multiply defined.')
+          f'MultiFourierKernel._set_param: parameter {par} multiply defined.'
+        )
       kwargs[par] = arg
 
     self._P = kwargs.get('P', self._P)
     if self._vectorize:
       self._alpha = kwargs.get('alpha', self._alpha)
       self._beta = kwargs.get('beta', self._beta)
     else:
@@ -2363,65 +2741,89 @@
 
   def _grad_param(self, grad_dU=None, grad_dV=None):
     if grad_dU is not None or grad_dV is not None:
       raise NotImplementedError()
 
     grad = {}
 
-    grad_U = self._cov._grad_U[:, self._offset:self._offset +
-      self._r] + self._cov._grad_V[:, self._offset:self._offset + self._r]
+    grad_U = (
+      self._cov._grad_U[:, self._offset : self._offset + self._r]
+      + self._cov._grad_V[:, self._offset : self._offset + self._r]
+    )
 
     if self._nharm > 0:
-      grad_nu = self._cov.t @ np.sum(
-        (grad_U[:, self._nfreq * self._coef_rank:] *
-        self._cov.U[:, self._offset + self._coef_rank:self._offset +
-        self._nfreq * self._coef_rank] -
-        grad_U[:, self._coef_rank:self._nfreq * self._coef_rank] *
-        self._cov.U[:, self._offset +
-        self._nfreq * self._coef_rank:self._offset + self._r]).reshape(
-        (-1, self._nharm, self._coef_rank)),
-        axis=2) @ np.arange(1, self._nfreq)
+      grad_nu = (
+        self._cov.t
+        @ np.sum(
+          (
+            grad_U[:, self._nfreq * self._coef_rank :]
+            * self._cov.U[
+              :,
+              self._offset + self._coef_rank : self._offset
+              + self._nfreq * self._coef_rank,
+            ]
+            - grad_U[:, self._coef_rank : self._nfreq * self._coef_rank]
+            * self._cov.U[
+              :, self._offset + self._nfreq * self._coef_rank : self._offset + self._r
+            ]
+          ).reshape((-1, self._nharm, self._coef_rank)),
+          axis=2,
+        )
+        @ np.arange(1, self._nfreq)
+      )
       grad['P'] = -self._nu / self._P * grad_nu
 
     grad_alpha = np.empty((self._nfreq, self._nseries, self._coef_rank))
     grad_beta = np.empty((self._nfreq, self._nseries, self._coef_rank))
     grad_beta[0] = 0
     for k, ik in enumerate(self._series_index):
       grad_A_k = np.sum(self._cov._grad_A[ik])
       grad_alpha[:, k] = 2 * self._alpha[:, k] * grad_A_k
-      grad_alpha[0, k] += np.sum(grad_U[ik, :self._coef_rank], axis=0)
+      grad_alpha[0, k] += np.sum(grad_U[ik, : self._coef_rank], axis=0)
       if self._nharm > 0:
         grad_beta[1:, k] = 2 * self._beta[1:, k] * grad_A_k
-        grad_alpha[1:, k] += np.sum(self._cjnut[ik, :, np.newaxis] *
-          grad_U[ik, self._coef_rank:self._nfreq * self._coef_rank].reshape(
-          -1, self._nharm, self._coef_rank),
-          axis=0)
-        grad_beta[1:, k] -= np.sum(self._sjnut[ik, :, np.newaxis] *
-          grad_U[ik, self._coef_rank:self._nfreq * self._coef_rank].reshape(
-          -1, self._nharm, self._coef_rank),
-          axis=0)
-        grad_alpha[1:, k] += np.sum(self._sjnut[ik, :, np.newaxis] *
-          grad_U[ik, self._nfreq * self._coef_rank:].reshape(
-          -1, self._nharm, self._coef_rank),
-          axis=0)
-        grad_beta[1:, k] += np.sum(self._cjnut[ik, :, np.newaxis] *
-          grad_U[ik, self._nfreq * self._coef_rank:].reshape(
-          -1, self._nharm, self._coef_rank),
-          axis=0)
+        grad_alpha[1:, k] += np.sum(
+          self._cjnut[ik, :, np.newaxis]
+          * grad_U[ik, self._coef_rank : self._nfreq * self._coef_rank].reshape(
+            -1, self._nharm, self._coef_rank
+          ),
+          axis=0,
+        )
+        grad_beta[1:, k] -= np.sum(
+          self._sjnut[ik, :, np.newaxis]
+          * grad_U[ik, self._coef_rank : self._nfreq * self._coef_rank].reshape(
+            -1, self._nharm, self._coef_rank
+          ),
+          axis=0,
+        )
+        grad_alpha[1:, k] += np.sum(
+          self._sjnut[ik, :, np.newaxis]
+          * grad_U[ik, self._nfreq * self._coef_rank :].reshape(
+            -1, self._nharm, self._coef_rank
+          ),
+          axis=0,
+        )
+        grad_beta[1:, k] += np.sum(
+          self._cjnut[ik, :, np.newaxis]
+          * grad_U[ik, self._nfreq * self._coef_rank :].reshape(
+            -1, self._nharm, self._coef_rank
+          ),
+          axis=0,
+        )
     if self._vectorize:
       grad['alpha'] = grad_alpha
       if self._nharm > 0:
         grad['beta'] = grad_beta
     else:
       for ndk in np.ndindex(grad_alpha.shape):
         grad['alpha_' + '_'.join([f'{k}' for k in ndk])] = grad_alpha[ndk]
         if self._nharm > 0:
           grad['beta_' + '_'.join([f'{k}' for k in ndk])] = grad_beta[ndk]
 
-    return (grad)
+    return grad
 
   def set_conditional_coef(self, alpha=None, beta=None, series_id=0):
     r"""
     Set the coefficients used for the conditional computations.
 
     Parameters
     ----------
@@ -2436,68 +2838,67 @@
     if series_id is None:
       self._cond_alpha = alpha
       self._cond_beta = beta
     else:
       self._cond_alpha = None
       self._cond_beta = None
 
-  def _compute_t2(self, t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right,
-    phi2left, phi2right):
+  def _compute_t2(
+    self, t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right, phi2left, phi2right
+  ):
     if self._cond_series_id is None:
       alpha = self._cond_alpha
       beta = self._cond_beta
     else:
       alpha = self._alpha[:, self._cond_series_id]
       if self._nharm > 0:
         beta = self._beta[:, self._cond_series_id]
 
-    U2[:, self._offset:self._offset + self._coef_rank] = alpha[0]
+    U2[:, self._offset : self._offset + self._coef_rank] = alpha[0]
     if self._nharm > 0:
       nut2 = self._nu * t2
       cjnut2 = np.empty((t2.size, self._nharm))
       sjnut2 = np.empty((t2.size, self._nharm))
       cjnut2[:, 0] = np.cos(nut2)
       sjnut2[:, 0] = np.sin(nut2)
       for j in range(1, self._nharm):
-        cjnut2[:, j] = cjnut2[:, j - 1] * cjnut2[:, 0] - sjnut2[:,
-          j - 1] * sjnut2[:, 0]
-        sjnut2[:, j] = sjnut2[:, j - 1] * cjnut2[:, 0] + cjnut2[:,
-          j - 1] * sjnut2[:, 0]
-      U2[:, self._offset + self._coef_rank:self._offset +
-        self._nfreq * self._coef_rank] = (
-        alpha[1:] * cjnut2[:, :, np.newaxis] -
-        beta[1:] * sjnut2[:, :, np.newaxis]).reshape(
-        -1, self._nharm * self._coef_rank)
-      U2[:, self._offset + self._nfreq * self._coef_rank:self._offset +
-        self._r] = (alpha[1:] * sjnut2[:, :, np.newaxis] +
-        beta[1:] * cjnut2[:, :, np.newaxis]).reshape(
-        -1, self._nharm * self._coef_rank)
-    V2[:, self._offset:self._offset + self._r] = U2[:,
-      self._offset:self._offset + self._r]
-    phi2[:, self._offset:self._offset + self._r] = 1.0
-    phi2left[:, self._offset:self._offset + self._r] = 1.0
-    phi2right[:, self._offset:self._offset + self._r] = 1.0
+        cjnut2[:, j] = cjnut2[:, j - 1] * cjnut2[:, 0] - sjnut2[:, j - 1] * sjnut2[:, 0]
+        sjnut2[:, j] = sjnut2[:, j - 1] * cjnut2[:, 0] + cjnut2[:, j - 1] * sjnut2[:, 0]
+      U2[
+        :, self._offset + self._coef_rank : self._offset + self._nfreq * self._coef_rank
+      ] = (
+        alpha[1:] * cjnut2[:, :, np.newaxis] - beta[1:] * sjnut2[:, :, np.newaxis]
+      ).reshape(-1, self._nharm * self._coef_rank)
+      U2[:, self._offset + self._nfreq * self._coef_rank : self._offset + self._r] = (
+        alpha[1:] * sjnut2[:, :, np.newaxis] + beta[1:] * cjnut2[:, :, np.newaxis]
+      ).reshape(-1, self._nharm * self._coef_rank)
+    V2[:, self._offset : self._offset + self._r] = U2[
+      :, self._offset : self._offset + self._r
+    ]
+    phi2[:, self._offset : self._offset + self._r] = 1.0
+    phi2left[:, self._offset : self._offset + self._r] = 1.0
+    phi2right[:, self._offset : self._offset + self._r] = 1.0
 
   def eval(self, dt, series_id=(0, 0)):
     k = np.sum(self._alpha[0, series_id[0]] * self._alpha[0, series_id[1]])
     if self._nharm > 0:
       a = np.sum(
-        self._alpha[1:, series_id[0]] * self._alpha[1:, series_id[1]] +
-        self._beta[1:, series_id[0]] * self._beta[1:, series_id[1]],
-        axis=1)
+        self._alpha[1:, series_id[0]] * self._alpha[1:, series_id[1]]
+        + self._beta[1:, series_id[0]] * self._beta[1:, series_id[1]],
+        axis=1,
+      )
       b = np.sum(
-        self._alpha[1:, series_id[0]] * self._beta[1:, series_id[1]] -
-        self._beta[1:, series_id[0]] * self._alpha[1:, series_id[1]],
-        axis=1)
+        self._alpha[1:, series_id[0]] * self._beta[1:, series_id[1]]
+        - self._beta[1:, series_id[0]] * self._alpha[1:, series_id[1]],
+        axis=1,
+      )
 
       cjnudt = np.empty((dt.size, self._nharm))
       sjnudt = np.empty((dt.size, self._nharm))
       nudt = self._nu * dt
       cjnudt[:, 0] = np.cos(nudt)
       sjnudt[:, 0] = np.sin(nudt)
       for j in range(1, self._nharm):
-        cjnudt[:, j] = cjnudt[:, j - 1] * cjnudt[:, 0] - sjnudt[:,
-          j - 1] * sjnudt[:, 0]
-        sjnudt[:, j] = sjnudt[:, j - 1] * cjnudt[:, 0] + cjnudt[:,
-          j - 1] * sjnudt[:, 0]
+        cjnudt[:, j] = cjnudt[:, j - 1] * cjnudt[:, 0] - sjnudt[:, j - 1] * sjnudt[:, 0]
+        sjnudt[:, j] = sjnudt[:, j - 1] * cjnudt[:, 0] + cjnudt[:, j - 1] * sjnudt[:, 0]
       k += cjnudt @ a + sjnudt @ b
-    return (k)
+    return k
```

### Comparing `spleaf-2.1.8/test/test_cov.py` & `spleaf-2.1.9/tests/test_cov.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-import pytest
+# -*- coding: utf-8 -*-
+
+# Copyright 2019-2024 Jean-Baptiste Delisle
+# Licensed under the EUPL-1.2 or later
+
 import numpy as np
 from spleaf.cov import Cov
 from spleaf.term import *
 
 prec = 1e-12
 n = 143
 ninst = 3
@@ -39,440 +43,458 @@
       deltaxk *= 2.0
     elif df > deltafmax:
       deltaxk /= 2.0
     else:
       break
     xb[k] = x[k] + deltaxk
     fxb = f(xb, *args)
-  return ((fxb - fx) / deltaxk)
+  return (fxb - fx) / deltaxk
 
 
-def grad(x,
+def grad(
+  x,
   f,
   deltax0=1e-8,
   deltafmin=1e-8,
   deltafmax=5e-8,
   maxiter=50,
   absolute=False,
-  args=()):
+  args=(),
+):
   if isinstance(deltax0, float):
     deltax = np.full_like(x, deltax0)
   else:
     deltax = deltax0
-  return (np.array([
-    _grad1d(x, f, k, deltax[k], deltafmin, deltafmax, maxiter, absolute, args)
-    for k in range(x.size)
-  ]))
+  return np.array(
+    [
+      _grad1d(x, f, k, deltax[k], deltafmin, deltafmax, maxiter, absolute, args)
+      for k in range(x.size)
+    ]
+  )
 
 
 def _generate_random_C(seed=0, deriv=False):
   np.random.seed(seed)
-  t = np.cumsum(10**np.random.uniform(-2, 1.5, n))
+  t = np.cumsum(10 ** np.random.uniform(-2, 1.5, n))
   sig_err = np.random.uniform(0.5, 1.5, n)
   sig_jitter = np.random.uniform(0.5, 1.5)
   inst_id = np.random.randint(0, ninst, n)
   sig_jitter_inst = np.random.uniform(0.5, 1.5, ninst)
   calib_file = np.empty(n, dtype=object)
   sig_calib_meas = np.empty(n)
-  lastfileinst = ["" for _ in range(ninst)]
+  lastfileinst = ['' for _ in range(ninst)]
   lastvarinst = [0 for _ in range(ninst)]
   nlastinst = [0 for _ in range(ninst)]
   for k in range(n):
     i = inst_id[k]
-    if lastfileinst[i] == "" or nlastinst[i] == calibmax or np.random.rand(
-    ) > calibprob:
+    if (
+      lastfileinst[i] == '' or nlastinst[i] == calibmax or np.random.rand() > calibprob
+    ):
       calib_file[k] = '{}'.format(k)
       sig_calib_meas[k] = np.random.uniform(0.5, 1.5)
       lastfileinst[i] = calib_file[k]
       lastvarinst[i] = sig_calib_meas[k]
       nlastinst[i] = 1
     else:
       calib_file[k] = lastfileinst[i]
       sig_calib_meas[k] = lastvarinst[i]
       nlastinst[i] += 1
   sig_calib_inst = np.random.uniform(0.5, 1.5, ninst)
   if not deriv:
     a_exp = np.random.uniform(0.5, 1.5, nexp)
-    la_exp = 10**np.random.uniform(-2, 2, nexp)
+    la_exp = 10 ** np.random.uniform(-2, 2, nexp)
     a_qper = np.random.uniform(0.5, 1.5, nqper)
     b_qper = np.random.uniform(0.05, 0.15, nqper)
-    la_qper = 10**np.random.uniform(-2, 2, nqper)
-    nu_qper = 10**np.random.uniform(-2, 2, nqper)
+    la_qper = 10 ** np.random.uniform(-2, 2, nqper)
+    nu_qper = 10 ** np.random.uniform(-2, 2, nqper)
   sig_mat32 = np.random.uniform(0.5, 1.5, nmat32)
-  rho_mat32 = 10**np.random.uniform(-2, 2, nmat32)
+  rho_mat32 = 10 ** np.random.uniform(-2, 2, nmat32)
   sig_mat52 = np.random.uniform(0.5, 1.5, nmat52)
-  rho_mat52 = 10**np.random.uniform(-2, 2, nmat52)
+  rho_mat52 = 10 ** np.random.uniform(-2, 2, nmat52)
   sig_es = np.random.uniform(0.5, 1.5, nes)
-  rho_es = 10**np.random.uniform(-2, 2, nes)
+  rho_es = 10 ** np.random.uniform(-2, 2, nes)
   sig_usho = np.random.uniform(0.5, 1.5, nusho)
-  P0_usho = 10**np.random.uniform(-2, 2, nusho)
+  P0_usho = 10 ** np.random.uniform(-2, 2, nusho)
   Q_usho = np.random.uniform(0.5, 20.0, nusho)
   sig_osho = np.random.uniform(0.5, 1.5, nosho)
-  P0_osho = 10**np.random.uniform(-2, 2, nosho)
+  P0_osho = 10 ** np.random.uniform(-2, 2, nosho)
   Q_osho = np.random.uniform(0.01, 0.5, nosho)
   sig_sho = np.random.uniform(0.5, 1.5, nsho)
-  P0_sho = 10**np.random.uniform(-2, 2, nsho)
+  P0_sho = 10 ** np.random.uniform(-2, 2, nsho)
   Q_sho = np.random.uniform(0.01, 2.0, nsho)
   sig_mep = np.random.uniform(0.5, 1.5, nmep)
-  P_mep = 10**np.random.uniform(-2, 2, nmep)
-  rho_mep = 10**np.random.uniform(-2, 2, nmep)
-  eta_mep = 10**np.random.uniform(-2, 1, nmep)
+  P_mep = 10 ** np.random.uniform(-2, 2, nmep)
+  rho_mep = 10 ** np.random.uniform(-2, 2, nmep)
+  eta_mep = 10 ** np.random.uniform(-2, 1, nmep)
   sig_esp = np.random.uniform(0.5, 1.5, nesp)
-  P_esp = 10**np.random.uniform(-2, 2, nesp)
-  rho_esp = 10**np.random.uniform(-2, 2, nesp)
-  eta_esp = 10**np.random.uniform(-2, 1, nesp)
+  P_esp = 10 ** np.random.uniform(-2, 2, nesp)
+  rho_esp = 10 ** np.random.uniform(-2, 2, nesp)
+  eta_esp = 10 ** np.random.uniform(-2, 1, nesp)
 
   if deriv:
-    return (Cov(t,
+    return Cov(
+      t,
       err=Error(sig_err),
       jit=Jitter(sig_jitter),
       **{
-      f'insjit_{k}': InstrumentJitter(inst_id == k, sig_jitter_inst[k])
-      for k in range(ninst)
+        f'insjit_{k}': InstrumentJitter(inst_id == k, sig_jitter_inst[k])
+        for k in range(ninst)
       },
       calerr=CalibrationError(calib_file, sig_calib_meas),
       **{
-      f'caljit_{k}': CalibrationJitter(inst_id == k, calib_file,
-      sig_calib_inst[k])
-      for k in range(ninst)
+        f'caljit_{k}': CalibrationJitter(inst_id == k, calib_file, sig_calib_inst[k])
+        for k in range(ninst)
       },
       **{
-      f'mat32_{k}': Matern32Kernel(sig_mat32[k], rho_mat32[k])
-      for k in range(nmat32)
+        f'mat32_{k}': Matern32Kernel(sig_mat32[k], rho_mat32[k]) for k in range(nmat32)
       },
       **{
-      f'mat52_{k}': Matern52Kernel(sig_mat52[k], rho_mat52[k])
-      for k in range(nmat52)
+        f'mat52_{k}': Matern52Kernel(sig_mat52[k], rho_mat52[k]) for k in range(nmat52)
       },
-      **{f'es_{k}': ESKernel(sig_es[k], rho_es[k])
-      for k in range(nes)},
+      **{f'es_{k}': ESKernel(sig_es[k], rho_es[k]) for k in range(nes)},
       **{
-      f'usho_{k}': USHOKernel(sig_usho[k], P0_usho[k], Q_usho[k])
-      for k in range(nusho)
+        f'usho_{k}': USHOKernel(sig_usho[k], P0_usho[k], Q_usho[k])
+        for k in range(nusho)
       },
       **{
-      f'osho_{k}': OSHOKernel(sig_osho[k], P0_osho[k], Q_osho[k])
-      for k in range(nosho)
+        f'osho_{k}': OSHOKernel(sig_osho[k], P0_osho[k], Q_osho[k])
+        for k in range(nosho)
       },
+      **{f'sho_{k}': SHOKernel(sig_sho[k], P0_sho[k], Q_sho[k]) for k in range(nsho)},
       **{
-      f'sho_{k}': SHOKernel(sig_sho[k], P0_sho[k], Q_sho[k])
-      for k in range(nsho)
+        f'mep_{k}': MEPKernel(sig_mep[k], P_mep[k], rho_mep[k], eta_mep[k])
+        for k in range(nmep)
       },
       **{
-      f'mep_{k}': MEPKernel(sig_mep[k], P_mep[k], rho_mep[k], eta_mep[k])
-      for k in range(nmep)
+        f'esp_{k}': ESPKernel(sig_esp[k], P_esp[k], rho_esp[k], eta_esp[k])
+        for k in range(nesp)
       },
-      **{
-      f'esp_{k}': ESPKernel(sig_esp[k], P_esp[k], rho_esp[k], eta_esp[k])
-      for k in range(nesp)
-      }))
+    )
   else:
-    return (Cov(t,
+    return Cov(
+      t,
       err=Error(sig_err),
       jit=Jitter(sig_jitter),
       **{
-      f'insjit_{k}': InstrumentJitter(inst_id == k, sig_jitter_inst[k])
-      for k in range(ninst)
+        f'insjit_{k}': InstrumentJitter(inst_id == k, sig_jitter_inst[k])
+        for k in range(ninst)
       },
       calerr=CalibrationError(calib_file, sig_calib_meas),
       **{
-      f'caljit_{k}': CalibrationJitter(inst_id == k, calib_file,
-      sig_calib_inst[k])
-      for k in range(ninst)
+        f'caljit_{k}': CalibrationJitter(inst_id == k, calib_file, sig_calib_inst[k])
+        for k in range(ninst)
       },
+      **{f'exp_{k}': ExponentialKernel(a_exp[k], la_exp[k]) for k in range(nexp)},
       **{
-      f'exp_{k}': ExponentialKernel(a_exp[k], la_exp[k])
-      for k in range(nexp)
+        f'qper_{k}': QuasiperiodicKernel(a_qper[k], b_qper[k], la_qper[k], nu_qper[k])
+        for k in range(nqper)
       },
       **{
-      f'qper_{k}': QuasiperiodicKernel(a_qper[k], b_qper[k], la_qper[k],
-      nu_qper[k])
-      for k in range(nqper)
+        f'mat32_{k}': Matern32Kernel(sig_mat32[k], rho_mat32[k]) for k in range(nmat32)
       },
       **{
-      f'mat32_{k}': Matern32Kernel(sig_mat32[k], rho_mat32[k])
-      for k in range(nmat32)
+        f'mat52_{k}': Matern52Kernel(sig_mat52[k], rho_mat52[k]) for k in range(nmat52)
       },
+      **{f'es_{k}': ESKernel(sig_es[k], rho_es[k]) for k in range(nes)},
       **{
-      f'mat52_{k}': Matern52Kernel(sig_mat52[k], rho_mat52[k])
-      for k in range(nmat52)
+        f'usho_{k}': USHOKernel(sig_usho[k], P0_usho[k], Q_usho[k])
+        for k in range(nusho)
       },
-      **{f'es_{k}': ESKernel(sig_es[k], rho_es[k])
-      for k in range(nes)},
       **{
-      f'usho_{k}': USHOKernel(sig_usho[k], P0_usho[k], Q_usho[k])
-      for k in range(nusho)
+        f'osho_{k}': OSHOKernel(sig_osho[k], P0_osho[k], Q_osho[k])
+        for k in range(nosho)
       },
+      **{f'sho_{k}': SHOKernel(sig_sho[k], P0_sho[k], Q_sho[k]) for k in range(nsho)},
       **{
-      f'osho_{k}': OSHOKernel(sig_osho[k], P0_osho[k], Q_osho[k])
-      for k in range(nosho)
+        f'mep_{k}': MEPKernel(sig_mep[k], P_mep[k], rho_mep[k], eta_mep[k])
+        for k in range(nmep)
       },
       **{
-      f'sho_{k}': SHOKernel(sig_sho[k], P0_sho[k], Q_sho[k])
-      for k in range(nsho)
+        f'esp_{k}': ESPKernel(sig_esp[k], P_esp[k], rho_esp[k], eta_esp[k])
+        for k in range(nesp)
       },
-      **{
-      f'mep_{k}': MEPKernel(sig_mep[k], P_mep[k], rho_mep[k], eta_mep[k])
-      for k in range(nmep)
-      },
-      **{
-      f'esp_{k}': ESPKernel(sig_esp[k], P_esp[k], rho_esp[k], eta_esp[k])
-      for k in range(nesp)
-      }))
+    )
 
 
 def _generate_random_param(seed=1):
   np.random.seed(seed)
   sig_jitter = np.random.uniform(0.5, 1.5, 1)
   sig_jitter_inst = np.random.uniform(0.5, 1.5, ninst)
   sig_calib_inst = np.random.uniform(0.5, 1.5, ninst)
   a_exp = np.random.uniform(0.5, 1.5, nexp)
-  la_exp = 10**np.random.uniform(-2, 2, nexp)
+  la_exp = 10 ** np.random.uniform(-2, 2, nexp)
   a_qper = np.random.uniform(0.5, 1.5, nqper)
   b_qper = np.random.uniform(0.05, 0.15, nqper)
-  la_qper = 10**np.random.uniform(-2, 2, nqper)
-  nu_qper = 10**np.random.uniform(-2, 2, nqper)
+  la_qper = 10 ** np.random.uniform(-2, 2, nqper)
+  nu_qper = 10 ** np.random.uniform(-2, 2, nqper)
   sig_mat32 = np.random.uniform(0.5, 1.5, nmat32)
-  rho_mat32 = 10**np.random.uniform(-2, 2, nmat32)
+  rho_mat32 = 10 ** np.random.uniform(-2, 2, nmat32)
   sig_mat52 = np.random.uniform(0.5, 1.5, nmat52)
-  rho_mat52 = 10**np.random.uniform(-2, 2, nmat52)
+  rho_mat52 = 10 ** np.random.uniform(-2, 2, nmat52)
   sig_es = np.random.uniform(0.5, 1.5, nes)
-  rho_es = 10**np.random.uniform(-2, 2, nes)
+  rho_es = 10 ** np.random.uniform(-2, 2, nes)
   sig_usho = np.random.uniform(0.5, 1.5, nusho)
-  P0_usho = 10**np.random.uniform(-2, 2, nusho)
+  P0_usho = 10 ** np.random.uniform(-2, 2, nusho)
   Q_usho = np.random.uniform(0.5, 20.0, nusho)
   sig_osho = np.random.uniform(0.5, 1.5, nosho)
-  P0_osho = 10**np.random.uniform(-2, 2, nosho)
+  P0_osho = 10 ** np.random.uniform(-2, 2, nosho)
   Q_osho = np.random.uniform(0.01, 0.5, nosho)
   sig_sho = np.random.uniform(0.5, 1.5, nsho)
-  P0_sho = 10**np.random.uniform(-2, 2, nsho)
+  P0_sho = 10 ** np.random.uniform(-2, 2, nsho)
   Q_sho = np.random.uniform(0.01, 2.0, nsho)
   sig_mep = np.random.uniform(0.5, 1.5, nmep)
-  P_mep = 10**np.random.uniform(-2, 2, nmep)
-  rho_mep = 10**np.random.uniform(-2, 2, nmep)
-  eta_mep = 10**np.random.uniform(-2, 1, nmep)
+  P_mep = 10 ** np.random.uniform(-2, 2, nmep)
+  rho_mep = 10 ** np.random.uniform(-2, 2, nmep)
+  eta_mep = 10 ** np.random.uniform(-2, 1, nmep)
   sig_esp = np.random.uniform(0.5, 1.5, nesp)
-  P_esp = 10**np.random.uniform(-2, 2, nesp)
-  rho_esp = 10**np.random.uniform(-2, 2, nesp)
-  eta_esp = 10**np.random.uniform(-2, 1, nesp)
-
-  return (sig_jitter, sig_jitter_inst, sig_calib_inst, a_exp, la_exp, a_qper,
-    b_qper, la_qper, nu_qper, sig_mat32, rho_mat32, sig_mat52, rho_mat52,
-    sig_es, rho_es, sig_usho, P0_usho, Q_usho, sig_osho, P0_osho, Q_osho,
-    sig_sho, P0_sho, Q_sho, sig_mep, P_mep, rho_mep, eta_mep, sig_esp, P_esp,
-    rho_esp, eta_esp)
+  P_esp = 10 ** np.random.uniform(-2, 2, nesp)
+  rho_esp = 10 ** np.random.uniform(-2, 2, nesp)
+  eta_esp = 10 ** np.random.uniform(-2, 1, nesp)
+
+  return (
+    sig_jitter,
+    sig_jitter_inst,
+    sig_calib_inst,
+    a_exp,
+    la_exp,
+    a_qper,
+    b_qper,
+    la_qper,
+    nu_qper,
+    sig_mat32,
+    rho_mat32,
+    sig_mat52,
+    rho_mat52,
+    sig_es,
+    rho_es,
+    sig_usho,
+    P0_usho,
+    Q_usho,
+    sig_osho,
+    P0_osho,
+    Q_osho,
+    sig_sho,
+    P0_sho,
+    Q_sho,
+    sig_mep,
+    P_mep,
+    rho_mep,
+    eta_mep,
+    sig_esp,
+    P_esp,
+    rho_esp,
+    eta_esp,
+  )
 
 
 def test_Cov():
   C = _generate_random_C()
 
   C_full = C.expand()
   L_full = C.expandL()
   D_full = np.diag(C.D)
 
   LDLt_full = L_full @ D_full @ L_full.T
-  err = np.max(
-    np.abs(C_full - LDLt_full)) / np.max(np.abs(C_full) + np.abs(LDLt_full))
-  assert err < prec, ('Cholesky decomposition not working'
-    ' at required precision ({} > {})').format(err, prec)
+  err = np.max(np.abs(C_full - LDLt_full)) / np.max(np.abs(C_full) + np.abs(LDLt_full))
+  assert err < prec, (
+    'Cholesky decomposition not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
 
 def test_set_param():
   C = _generate_random_C()
   param = list(_generate_random_param())
-  Cb = Cov(C.t,
+  Cb = Cov(
+    C.t,
     err=Error(C.term['err']._sig),
     jit=Jitter(param[0][0]),
     **{
-    f'insjit_{k}': InstrumentJitter(C.term[f'insjit_{k}']._indices,
-    param[1][k])
-    for k in range(ninst)
+      f'insjit_{k}': InstrumentJitter(C.term[f'insjit_{k}']._indices, param[1][k])
+      for k in range(ninst)
     },
     calerr=CalibrationError(C.term['calerr']._calib_id, C.term['calerr']._sig),
     **{
-    f'caljit_{k}': CalibrationJitter(C.term[f'insjit_{k}']._indices,
-    C.term['calerr']._calib_id, param[2][k])
-    for k in range(ninst)
-    },
-    **{
-    f'exp_{k}': ExponentialKernel(param[3][k], param[4][k])
-    for k in range(nexp)
-    },
-    **{
-    f'qper_{k}': QuasiperiodicKernel(param[5][k], param[6][k], param[7][k],
-    param[8][k])
-    for k in range(nqper)
+      f'caljit_{k}': CalibrationJitter(
+        C.term[f'insjit_{k}']._indices, C.term['calerr']._calib_id, param[2][k]
+      )
+      for k in range(ninst)
     },
+    **{f'exp_{k}': ExponentialKernel(param[3][k], param[4][k]) for k in range(nexp)},
     **{
-    f'mat32_{k}': Matern32Kernel(param[9][k], param[10][k])
-    for k in range(nmat32)
+      f'qper_{k}': QuasiperiodicKernel(
+        param[5][k], param[6][k], param[7][k], param[8][k]
+      )
+      for k in range(nqper)
     },
+    **{f'mat32_{k}': Matern32Kernel(param[9][k], param[10][k]) for k in range(nmat32)},
+    **{f'mat52_{k}': Matern52Kernel(param[11][k], param[12][k]) for k in range(nmat52)},
+    **{f'es_{k}': ESKernel(param[13][k], param[14][k]) for k in range(nes)},
     **{
-    f'mat52_{k}': Matern52Kernel(param[11][k], param[12][k])
-    for k in range(nmat52)
+      f'usho_{k}': USHOKernel(param[15][k], param[16][k], param[17][k])
+      for k in range(nusho)
     },
-    **{f'es_{k}': ESKernel(param[13][k], param[14][k])
-    for k in range(nes)},
     **{
-    f'usho_{k}': USHOKernel(param[15][k], param[16][k], param[17][k])
-    for k in range(nusho)
+      f'osho_{k}': OSHOKernel(param[18][k], param[19][k], param[20][k])
+      for k in range(nosho)
     },
     **{
-    f'osho_{k}': OSHOKernel(param[18][k], param[19][k], param[20][k])
-    for k in range(nosho)
+      f'sho_{k}': SHOKernel(param[21][k], param[22][k], param[23][k])
+      for k in range(nsho)
     },
     **{
-    f'sho_{k}': SHOKernel(param[21][k], param[22][k], param[23][k])
-    for k in range(nsho)
+      f'mep_{k}': MEPKernel(param[24][k], param[25][k], param[26][k], param[27][k])
+      for k in range(nmep)
     },
     **{
-    f'mep_{k}': MEPKernel(param[24][k], param[25][k], param[26][k],
-    param[27][k])
-    for k in range(nmep)
+      f'esp_{k}': ESPKernel(param[28][k], param[29][k], param[30][k], param[31][k])
+      for k in range(nesp)
     },
-    **{
-    f'esp_{k}': ESPKernel(param[28][k], param[29][k], param[30][k],
-    param[31][k])
-    for k in range(nesp)
-    })
-
-  C.set_param(np.concatenate(param),
-    ['jit.sig'] + [f'insjit_{k}.sig'
-    for k in range(ninst)] + [f'caljit_{k}.sig'
-    for k in range(ninst)] + [f'exp_{k}.a'
-    for k in range(nexp)] + [f'exp_{k}.la'
-    for k in range(nexp)] + [f'qper_{k}.a'
-    for k in range(nqper)] + [f'qper_{k}.b'
-    for k in range(nqper)] + [f'qper_{k}.la'
-    for k in range(nqper)] + [f'qper_{k}.nu'
-    for k in range(nqper)] + [f'mat32_{k}.sig'
-    for k in range(nmat32)] + [f'mat32_{k}.rho'
-    for k in range(nmat32)] + [f'mat52_{k}.sig'
-    for k in range(nmat52)] + [f'mat52_{k}.rho'
-    for k in range(nmat52)] + [f'es_{k}.sig'
-    for k in range(nes)] + [f'es_{k}.rho'
-    for k in range(nes)] + [f'usho_{k}.sig'
-    for k in range(nusho)] + [f'usho_{k}.P0'
-    for k in range(nusho)] + [f'usho_{k}.Q'
-    for k in range(nusho)] + [f'osho_{k}.sig'
-    for k in range(nosho)] + [f'osho_{k}.P0'
-    for k in range(nosho)] + [f'osho_{k}.Q'
-    for k in range(nosho)] + [f'sho_{k}.sig'
-    for k in range(nsho)] + [f'sho_{k}.P0'
-    for k in range(nsho)] + [f'sho_{k}.Q'
-    for k in range(nsho)] + [f'mep_{k}.sig'
-    for k in range(nmep)] + [f'mep_{k}.P'
-    for k in range(nmep)] + [f'mep_{k}.rho'
-    for k in range(nmep)] + [f'mep_{k}.eta'
-    for k in range(nmep)] + [f'esp_{k}.sig'
-    for k in range(nesp)] + [f'esp_{k}.P'
-    for k in range(nesp)] + [f'esp_{k}.rho'
-    for k in range(nesp)] + [f'esp_{k}.eta' for k in range(nesp)])
+  )
+
+  C.set_param(
+    np.concatenate(param),
+    ['jit.sig']
+    + [f'insjit_{k}.sig' for k in range(ninst)]
+    + [f'caljit_{k}.sig' for k in range(ninst)]
+    + [f'exp_{k}.a' for k in range(nexp)]
+    + [f'exp_{k}.la' for k in range(nexp)]
+    + [f'qper_{k}.a' for k in range(nqper)]
+    + [f'qper_{k}.b' for k in range(nqper)]
+    + [f'qper_{k}.la' for k in range(nqper)]
+    + [f'qper_{k}.nu' for k in range(nqper)]
+    + [f'mat32_{k}.sig' for k in range(nmat32)]
+    + [f'mat32_{k}.rho' for k in range(nmat32)]
+    + [f'mat52_{k}.sig' for k in range(nmat52)]
+    + [f'mat52_{k}.rho' for k in range(nmat52)]
+    + [f'es_{k}.sig' for k in range(nes)]
+    + [f'es_{k}.rho' for k in range(nes)]
+    + [f'usho_{k}.sig' for k in range(nusho)]
+    + [f'usho_{k}.P0' for k in range(nusho)]
+    + [f'usho_{k}.Q' for k in range(nusho)]
+    + [f'osho_{k}.sig' for k in range(nosho)]
+    + [f'osho_{k}.P0' for k in range(nosho)]
+    + [f'osho_{k}.Q' for k in range(nosho)]
+    + [f'sho_{k}.sig' for k in range(nsho)]
+    + [f'sho_{k}.P0' for k in range(nsho)]
+    + [f'sho_{k}.Q' for k in range(nsho)]
+    + [f'mep_{k}.sig' for k in range(nmep)]
+    + [f'mep_{k}.P' for k in range(nmep)]
+    + [f'mep_{k}.rho' for k in range(nmep)]
+    + [f'mep_{k}.eta' for k in range(nmep)]
+    + [f'esp_{k}.sig' for k in range(nesp)]
+    + [f'esp_{k}.P' for k in range(nesp)]
+    + [f'esp_{k}.rho' for k in range(nesp)]
+    + [f'esp_{k}.eta' for k in range(nesp)],
+  )
 
   C_full = C.expand()
   Cb_full = Cb.expand()
   L_full = C.expandL()
   Lb_full = Cb.expandL()
 
-  err = np.max(
-    np.abs(C_full - Cb_full)) / np.max(np.abs(C_full) + np.abs(Cb_full))
+  err = np.max(np.abs(C_full - Cb_full)) / np.max(np.abs(C_full) + np.abs(Cb_full))
   err = max(
-    err,
-    np.max(np.abs(L_full - Lb_full)) /
-    np.max(np.abs(L_full) + np.abs(Lb_full)))
-  err = max(err,
-    np.max(np.abs(C.D - Cb.D)) / np.max(np.abs(C.D) + np.abs(Cb.D)))
-
-  assert err < prec, ('set_param not working'
-    ' at required precision ({} > {})').format(err, prec)
+    err, np.max(np.abs(L_full - Lb_full)) / np.max(np.abs(L_full) + np.abs(Lb_full))
+  )
+  err = max(err, np.max(np.abs(C.D - Cb.D)) / np.max(np.abs(C.D) + np.abs(Cb.D)))
+
+  assert err < prec, (
+    'set_param not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
 
 def test_inv():
   C = _generate_random_C()
 
   C_full = C.expand()
   invC_full = C.expandInv()
 
   CinvC_full = C_full @ invC_full
   err = np.max(np.abs(CinvC_full - np.identity(n)))
-  assert err < prec, ('Inversion not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'Inversion not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
 
 def test_invL():
   C = _generate_random_C()
 
   L_full = C.expandL()
   invL_full = C.expandInvL()
 
   LinvL_full = L_full @ invL_full
   err = np.max(np.abs(LinvL_full - np.identity(n)))
-  assert err < prec, ('Cholesky inversion not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'Cholesky inversion not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
 
 def test_logdet():
   C = _generate_random_C()
 
   logdet = C.logdet()
 
   C_full = C.expand()
   sign_full, logdet_full = np.linalg.slogdet(C_full)
 
   err = abs(logdet / logdet_full - 1)
 
   assert sign_full > 0, 'logdet is not positive'
-  assert err < prec, ('logdet not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, ('logdet not working' ' at required precision ({} > {})').format(
+    err, prec
+  )
 
 
 def test_dotL():
   C = _generate_random_C()
   x = np.random.normal(0.0, 1.0, C.n)
 
   y = C.dotL(x)
 
   L_full = C.expandL()
   y_full = L_full.dot(x)
 
   err = np.max(np.abs(y - y_full)) / np.max(np.abs(y) + np.abs(y_full))
 
-  assert err < prec, ('dotL not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, ('dotL not working' ' at required precision ({} > {})').format(
+    err, prec
+  )
 
 
 def test_solveL():
   C = _generate_random_C()
   y = np.random.normal(0.0, 5.0, C.n)
 
   x = C.solveL(y)
 
   L_full = C.expandL()
   x_full = np.linalg.solve(L_full, y)
 
   err = np.max(np.abs(x - x_full)) / np.max(np.abs(x) + np.abs(x_full))
 
-  assert err < prec, ('solveL not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, ('solveL not working' ' at required precision ({} > {})').format(
+    err, prec
+  )
 
 
 def test_chi2():
   C = _generate_random_C()
   y = np.random.normal(0.0, 5.0, C.n)
 
   chi2 = C.chi2(y)
 
   C_full = C.expand()
   invC_full = np.linalg.inv(C_full)
   chi2_full = y.T @ invC_full @ y
 
   err = abs(chi2 - chi2_full) / (abs(chi2) + abs(chi2_full))
 
-  assert err < prec, ('chi2 not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, ('chi2 not working' ' at required precision ({} > {})').format(
+    err, prec
+  )
 
 
 def test_loglike():
   C = _generate_random_C()
   y = np.random.normal(0.0, 5.0, C.n)
 
   loglike = C.loglike(y)
@@ -480,16 +502,17 @@
   C_full = C.expand()
   invC_full = np.linalg.inv(C_full)
   chi2_full = y.T @ invC_full @ y
   _, logdet_full = np.linalg.slogdet(C_full)
   loglike_full = -0.5 * (chi2_full + logdet_full + C.n * np.log(2.0 * np.pi))
 
   err = abs(loglike - loglike_full) / (abs(loglike) + abs(loglike_full))
-  assert err < prec, ('loglike not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, ('loglike not working' ' at required precision ({} > {})').format(
+    err, prec
+  )
 
 
 def _test_method_back(method):
   """
   Common code for testing dotL_back, solveL_back, dotLT_back, solveLT_back
   """
   C = _generate_random_C()
@@ -503,43 +526,48 @@
   grad_a = getattr(C, method + '_back')(grad_b)
   C.cholesky_back()
   grad_param = C.grad_param()
 
   # Numerical grad
   def func_param(x):
     C.set_param(x)
-    return (func(a))
+    return func(a)
 
   grad_a_num = []
   grad_param_num = []
   for delta0 in [delta, coef_delta * delta]:
     grad_a_num.append(grad(a, func, deltax0=delta0) @ grad_b)
-    grad_param_num.append(
-      grad(C.get_param(), func_param, deltax0=delta0) @ grad_b)
+    grad_param_num.append(grad(C.get_param(), func_param, deltax0=delta0) @ grad_b)
 
   # Comparison
   err = np.max(
-    np.abs(grad_a - np.mean(grad_a_num, axis=0)) /
-    (np.abs(grad_a_num[1]) + np.abs(grad_a_num[0])))
+    np.abs(grad_a - np.mean(grad_a_num, axis=0))
+    / (np.abs(grad_a_num[1]) + np.abs(grad_a_num[0]))
+  )
   num_err = np.max(
-    np.abs(grad_a_num[1] - grad_a_num[0]) /
-    (np.abs(grad_a_num[1]) + np.abs(grad_a_num[0])))
+    np.abs(grad_a_num[1] - grad_a_num[0])
+    / (np.abs(grad_a_num[1]) + np.abs(grad_a_num[0]))
+  )
   err = max(0.0, err - coef_num_err * num_err)
-  assert err < prec, ('{}_back (a) not working'
-    ' at required precision ({} > {})').format(method, err, prec)
+  assert err < prec, (
+    '{}_back (a) not working' ' at required precision ({} > {})'
+  ).format(method, err, prec)
 
   err = np.max(
-    np.abs(grad_param - np.mean(grad_param_num, axis=0)) /
-    (np.abs(grad_param_num[1]) + np.abs(grad_param_num[0])))
+    np.abs(grad_param - np.mean(grad_param_num, axis=0))
+    / (np.abs(grad_param_num[1]) + np.abs(grad_param_num[0]))
+  )
   num_err = np.max(
-    np.abs(grad_param_num[1] - grad_param_num[0]) /
-    (np.abs(grad_param_num[1]) + np.abs(grad_param_num[0])))
+    np.abs(grad_param_num[1] - grad_param_num[0])
+    / (np.abs(grad_param_num[1]) + np.abs(grad_param_num[0]))
+  )
   err = max(0.0, err - coef_num_err * num_err)
-  assert err < prec, ('{}_back (param) not working'
-    ' at required precision ({} > {})').format(method, err, prec)
+  assert err < prec, (
+    '{}_back (param) not working' ' at required precision ({} > {})'
+  ).format(method, err, prec)
 
 
 def test_dotL_back():
   _test_method_back('dotL')
 
 
 def test_solveL_back():
@@ -565,42 +593,48 @@
   func = getattr(C, method)
   _ = func(y)
   f_grad_res, f_grad_param = getattr(C, method + '_grad')()
 
   # Numerical grad
   def func_param(x):
     C.set_param(x)
-    return (func(y))
+    return func(y)
 
   f_grad_res_num = []
   f_grad_param_num = []
   for delta0 in [delta, coef_delta * delta]:
     f_grad_res_num.append(grad(y, func, deltax0=delta0))
     f_grad_param_num.append(grad(C.get_param(), func_param, deltax0=delta0))
 
   # Comparison
   err = np.max(
-    np.abs(f_grad_res - np.mean(f_grad_res_num, axis=0)) /
-    (np.abs(f_grad_res_num[1]) + np.abs(f_grad_res_num[0])))
+    np.abs(f_grad_res - np.mean(f_grad_res_num, axis=0))
+    / (np.abs(f_grad_res_num[1]) + np.abs(f_grad_res_num[0]))
+  )
   num_err = np.max(
-    np.abs(f_grad_res_num[1] - f_grad_res_num[0]) /
-    (np.abs(f_grad_res_num[1]) + np.abs(f_grad_res_num[0])))
+    np.abs(f_grad_res_num[1] - f_grad_res_num[0])
+    / (np.abs(f_grad_res_num[1]) + np.abs(f_grad_res_num[0]))
+  )
   err = max(0.0, err - coef_num_err * num_err)
-  assert err < prec, ('{}_grad (y) not working'
-    ' at required precision ({} > {})').format(method, err, prec)
+  assert err < prec, (
+    '{}_grad (y) not working' ' at required precision ({} > {})'
+  ).format(method, err, prec)
 
   err = np.max(
-    np.abs(f_grad_param - np.mean(f_grad_param_num, axis=0)) /
-    (np.abs(f_grad_param_num[1]) + np.abs(f_grad_param_num[0])))
+    np.abs(f_grad_param - np.mean(f_grad_param_num, axis=0))
+    / (np.abs(f_grad_param_num[1]) + np.abs(f_grad_param_num[0]))
+  )
   num_err = np.max(
-    np.abs(f_grad_param_num[1] - f_grad_param_num[0]) /
-    (np.abs(f_grad_param_num[1]) + np.abs(f_grad_param_num[0])))
+    np.abs(f_grad_param_num[1] - f_grad_param_num[0])
+    / (np.abs(f_grad_param_num[1]) + np.abs(f_grad_param_num[0]))
+  )
   err = max(0.0, err - coef_num_err * num_err)
-  assert err < prec, ('{}_grad (param) not working'
-    ' at required precision ({} > {})').format(method, err, prec)
+  assert err < prec, (
+    '{}_grad (param) not working' ' at required precision ({} > {})'
+  ).format(method, err, prec)
 
 
 def test_chi2_grad():
   _test_method_grad('chi2')
 
 
 def test_loglike_grad():
@@ -619,41 +653,47 @@
   invC_full = C.expandInv()
   invCy_full = invC_full.dot(y)
   term = {}
   if kernel is None:
     kernel = C.kernel
   for key in kernel:
     term[key] = C.kernel[key].__class__(
-      *[getattr(C.kernel[key], f'_{param}') for param in C.kernel[key]._param])
+      *[getattr(C.kernel[key], f'_{param}') for param in C.kernel[key]._param]
+    )
   print(term)
   K = Cov(C.t, **term)
   K_full = K.expand()
   mu_full = K_full @ invCy_full
   cov_full = K_full - K_full @ invC_full @ K_full
   var_full = np.diag(cov_full)
 
   err = np.max(np.abs(mu - mu_full)) / np.max(np.abs(mu) + np.abs(mu_full))
-  assert err < prec, ('self_conditional not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'self_conditional not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
   err = np.max(np.abs(muv - mu_full)) / np.max(np.abs(muv) + np.abs(mu_full))
-  assert err < prec, ('self_conditional not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'self_conditional not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
   err = np.max(np.abs(muc - mu_full)) / np.max(np.abs(muc) + np.abs(mu_full))
-  assert err < prec, ('self_conditional not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'self_conditional not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
   err = np.max(np.abs(var - var_full)) / np.max(np.abs(var) + np.abs(var_full))
-  assert err < prec, ('self_conditional not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'self_conditional not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
   err = np.max(np.abs(cov - cov_full)) / np.max(np.abs(cov) + np.abs(cov_full))
-  assert err < prec, ('self_conditional not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'self_conditional not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
 
 def _test_conditional(kernel=None):
   C = _generate_random_C()
   y = C.sample()
 
   n2 = 300
@@ -668,40 +708,46 @@
   invCy_full = invC_full.dot(y)
   Km_full = C.eval(t2[:, None] - C.t[None, :], kernel=kernel)
   term = {}
   if kernel is None:
     kernel = C.kernel
   for key in kernel:
     term[key] = C.kernel[key].__class__(
-      *[getattr(C.kernel[key], f'_{param}') for param in C.kernel[key]._param])
+      *[getattr(C.kernel[key], f'_{param}') for param in C.kernel[key]._param]
+    )
   K = Cov(t2, **term)
   K_full = K.expand()
   mu_full = Km_full @ invCy_full
   cov_full = K_full - Km_full @ invC_full @ Km_full.T
   var_full = np.diag(cov_full)
 
   err = np.max(np.abs(mu - mu_full)) / np.max(np.abs(mu) + np.abs(mu_full))
-  assert err < prec, ('conditional not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'conditional not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
   err = np.max(np.abs(muv - mu_full)) / np.max(np.abs(muv) + np.abs(mu_full))
-  assert err < prec, ('conditional not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'conditional not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
   err = np.max(np.abs(muc - mu_full)) / np.max(np.abs(muc) + np.abs(mu_full))
-  assert err < prec, ('conditional not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'conditional not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
   err = np.max(np.abs(var - var_full)) / np.max(np.abs(var) + np.abs(var_full))
-  assert err < prec, ('conditional not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'conditional not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
   err = np.max(np.abs(cov - cov_full)) / np.max(np.abs(cov) + np.abs(cov_full))
-  assert err < prec, ('conditional not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'conditional not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
 
 def _test_self_conditional_derivative(kernel=None):
   C = _generate_random_C(deriv=True)
   y = C.sample()
 
   # Analytical derivative
@@ -713,59 +759,67 @@
   num_dmu = []
   num_dcov = []
   for dt in [delta, coef_delta * delta]:
     tfull = np.sort(np.concatenate((C.t, C.t + dt)))
     mu, cov = C.conditional(y, tfull, calc_cov=True, kernel=kernel)
     num_dmu.append((mu[1::2] - mu[::2]) / abs(dt))
     num_dcov.append(
-      (cov[1::2, 1::2] + cov[::2, ::2] - cov[1::2, ::2] - cov[::2, 1::2]) /
-      dt**2)
+      (cov[1::2, 1::2] + cov[::2, ::2] - cov[1::2, ::2] - cov[::2, 1::2]) / dt**2
+    )
 
   num_dmu_mean = (num_dmu[0] + num_dmu[1]) / 2
-  num_dmu_err = np.max(np.abs(num_dmu[0] -
-    num_dmu[1])) / np.max(np.abs(num_dmu[0]) + np.abs(num_dmu[1]))
+  num_dmu_err = np.max(np.abs(num_dmu[0] - num_dmu[1])) / np.max(
+    np.abs(num_dmu[0]) + np.abs(num_dmu[1])
+  )
 
   num_dcov_mean = (num_dcov[0] + num_dcov[1]) / 2
-  num_dcov_err = np.max(np.abs(num_dcov[0] -
-    num_dcov[1])) / np.max(np.abs(num_dcov[0]) + np.abs(num_dcov[1]))
+  num_dcov_err = np.max(np.abs(num_dcov[0] - num_dcov[1])) / np.max(
+    np.abs(num_dcov[0]) + np.abs(num_dcov[1])
+  )
 
   num_dvar_mean = num_dcov_mean.diagonal()
   num_dvar_err = np.max(
-    np.abs(num_dcov[0].diagonal() - num_dcov[1].diagonal())) / np.max(
-    np.abs(num_dcov[0].diagonal()) + np.abs(num_dcov[1].diagonal()))
+    np.abs(num_dcov[0].diagonal() - num_dcov[1].diagonal())
+  ) / np.max(np.abs(num_dcov[0].diagonal()) + np.abs(num_dcov[1].diagonal()))
 
-  err = np.max(np.abs(dmu -
-    num_dmu_mean)) / np.max(np.abs(num_dmu[0]) + np.abs(num_dmu[1]))
+  err = np.max(np.abs(dmu - num_dmu_mean)) / np.max(
+    np.abs(num_dmu[0]) + np.abs(num_dmu[1])
+  )
   err = max(0.0, err - coef_num_err * num_dmu_err)
-  assert err < prec, ('self_conditional_derivative not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'self_conditional_derivative not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
-  err = np.max(
-    np.abs(dmuv - num_dmu)) / np.max(np.abs(num_dmu[0]) + np.abs(num_dmu[1]))
+  err = np.max(np.abs(dmuv - num_dmu)) / np.max(np.abs(num_dmu[0]) + np.abs(num_dmu[1]))
   err = max(0.0, err - coef_num_err * num_dmu_err)
-  assert err < prec, ('self_conditional_derivative not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'self_conditional_derivative not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
-  err = np.max(
-    np.abs(dmuc - num_dmu)) / np.max(np.abs(num_dmu[0]) + np.abs(num_dmu[1]))
+  err = np.max(np.abs(dmuc - num_dmu)) / np.max(np.abs(num_dmu[0]) + np.abs(num_dmu[1]))
   err = max(0.0, err - coef_num_err * num_dmu_err)
-  assert err < prec, ('self_conditional_derivative not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'self_conditional_derivative not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
   err = np.max(np.abs(dvar - num_dvar_mean)) / np.max(
-    np.abs(num_dcov[0].diagonal()) + np.abs(num_dcov[1].diagonal()))
+    np.abs(num_dcov[0].diagonal()) + np.abs(num_dcov[1].diagonal())
+  )
   err = max(0.0, err - coef_num_err * num_dvar_err)
-  assert err < prec, ('self_conditional_derivative not working'
-    ' at required precision ({} > {})').format(err, prec)
-
-  err = np.max(np.abs(dcov -
-    num_dcov_mean)) / np.max(np.abs(num_dcov[0]) + np.abs(num_dcov[1]))
+  assert err < prec, (
+    'self_conditional_derivative not working' ' at required precision ({} > {})'
+  ).format(err, prec)
+
+  err = np.max(np.abs(dcov - num_dcov_mean)) / np.max(
+    np.abs(num_dcov[0]) + np.abs(num_dcov[1])
+  )
   err = max(0.0, err - coef_num_err * num_dcov_err)
-  assert err < prec, ('self_conditional_derivative not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'self_conditional_derivative not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
 
 def _test_conditional_derivative(kernel=None):
   C = _generate_random_C(deriv=True)
   y = C.dotL(np.random.normal(0.0, C.sqD()))
 
   n2 = 1001
@@ -782,63 +836,77 @@
   num_dmu = []
   num_dcov = []
   for dt in [delta, coef_delta * delta]:
     tfull = np.sort(np.concatenate((t2, t2 + dt)))
     mu, cov = C.conditional(y, tfull, calc_cov=True, kernel=kernel)
     num_dmu.append((mu[1::2] - mu[::2]) / abs(dt))
     num_dcov.append(
-      (cov[1::2, 1::2] + cov[::2, ::2] - cov[1::2, ::2] - cov[::2, 1::2]) /
-      dt**2)
+      (cov[1::2, 1::2] + cov[::2, ::2] - cov[1::2, ::2] - cov[::2, 1::2]) / dt**2
+    )
 
   num_dmu_mean = (num_dmu[0] + num_dmu[1]) / 2
-  num_dmu_err = np.max(np.abs(num_dmu[0] -
-    num_dmu[1])) / np.max(np.abs(num_dmu[0]) + np.abs(num_dmu[1]))
+  num_dmu_err = np.max(np.abs(num_dmu[0] - num_dmu[1])) / np.max(
+    np.abs(num_dmu[0]) + np.abs(num_dmu[1])
+  )
 
   num_dcov_mean = (num_dcov[0] + num_dcov[1]) / 2
-  num_dcov_err = np.max(np.abs(num_dcov[0] -
-    num_dcov[1])) / np.max(np.abs(num_dcov[0]) + np.abs(num_dcov[1]))
+  num_dcov_err = np.max(np.abs(num_dcov[0] - num_dcov[1])) / np.max(
+    np.abs(num_dcov[0]) + np.abs(num_dcov[1])
+  )
 
   num_dvar_mean = num_dcov_mean.diagonal()
   num_dvar_err = np.max(
-    np.abs(num_dcov[0].diagonal() - num_dcov[1].diagonal())) / np.max(
-    np.abs(num_dcov[0].diagonal()) + np.abs(num_dcov[1].diagonal()))
+    np.abs(num_dcov[0].diagonal() - num_dcov[1].diagonal())
+  ) / np.max(np.abs(num_dcov[0].diagonal()) + np.abs(num_dcov[1].diagonal()))
 
-  err = np.max(np.abs(dmu -
-    num_dmu_mean)) / np.max(np.abs(num_dmu[0]) + np.abs(num_dmu[1]))
+  err = np.max(np.abs(dmu - num_dmu_mean)) / np.max(
+    np.abs(num_dmu[0]) + np.abs(num_dmu[1])
+  )
   err = max(0.0, err - coef_num_err * num_dmu_err)
-  assert err < prec, ('conditional_derivative not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'conditional_derivative not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
-  err = np.max(
-    np.abs(dmuv - num_dmu)) / np.max(np.abs(num_dmu[0]) + np.abs(num_dmu[1]))
+  err = np.max(np.abs(dmuv - num_dmu)) / np.max(np.abs(num_dmu[0]) + np.abs(num_dmu[1]))
   err = max(0.0, err - coef_num_err * num_dmu_err)
-  assert err < prec, ('conditional_derivative not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'conditional_derivative not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
-  err = np.max(
-    np.abs(dmuc - num_dmu)) / np.max(np.abs(num_dmu[0]) + np.abs(num_dmu[1]))
+  err = np.max(np.abs(dmuc - num_dmu)) / np.max(np.abs(num_dmu[0]) + np.abs(num_dmu[1]))
   err = max(0.0, err - coef_num_err * num_dmu_err)
-  assert err < prec, ('conditional_derivative not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'conditional_derivative not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
   err = np.max(np.abs(dvar - num_dvar_mean)) / np.max(
-    np.abs(num_dcov[0].diagonal()) + np.abs(num_dcov[1].diagonal()))
+    np.abs(num_dcov[0].diagonal()) + np.abs(num_dcov[1].diagonal())
+  )
   err = max(0.0, err - coef_num_err * num_dvar_err)
-  assert err < prec, ('conditional_derivative not working'
-    ' at required precision ({} > {})').format(err, prec)
-
-  err = np.max(np.abs(dcov -
-    num_dcov_mean)) / np.max(np.abs(num_dcov[0]) + np.abs(num_dcov[1]))
+  assert err < prec, (
+    'conditional_derivative not working' ' at required precision ({} > {})'
+  ).format(err, prec)
+
+  err = np.max(np.abs(dcov - num_dcov_mean)) / np.max(
+    np.abs(num_dcov[0]) + np.abs(num_dcov[1])
+  )
   err = max(0.0, err - coef_num_err * num_dcov_err)
-  assert err < prec, ('conditional_derivative not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'conditional_derivative not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
 
 def test_all_conditional():
   for kernel in [
-      None, ['mat32_0', 'usho_0'], ['osho_0'], ['mat52_0', 'sho_0'],
-    ['es_0', 'sho_0'], ['mep_0'], ['esp_0']
+    None,
+    ['mat32_0', 'usho_0'],
+    ['osho_0'],
+    ['mat52_0', 'sho_0'],
+    ['es_0', 'sho_0'],
+    ['mep_0'],
+    ['esp_0'],
   ]:
+    print(kernel)
     _test_self_conditional(kernel)
     _test_conditional(kernel)
     _test_self_conditional_derivative(kernel)
     _test_conditional_derivative(kernel)
```

### Comparing `spleaf-2.1.8/test/test_spleaf.py` & `spleaf-2.1.9/tests/test_spleaf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-import pytest
+# -*- coding: utf-8 -*-
+
+# Copyright 2019-2024 Jean-Baptiste Delisle
+# Licensed under the EUPL-1.2 or later
+
 import numpy as np
 from spleaf import Spleaf
 
 prec = 1e-12
 n = 143
 r = 11
 bmax = 11
@@ -18,48 +22,49 @@
   V = np.random.uniform(0.5, 1.5, (n, r))
   log10phi = np.random.uniform(-4, 0, (n - 1, r))
   phi = 10**log10phi
 
   b = np.minimum(k, np.random.randint(bmax + 1))
   offsetrow = np.cumsum(b - 1) + 1
   nF = offsetrow[-1] + n - 1
-  F = np.random.uniform(0.25, 0.5, nF)**2
+  F = np.random.uniform(0.25, 0.5, nF) ** 2
 
-  A = np.random.uniform(1.5, 2.5, n)**2 + np.sum(U * V, axis=1)
+  A = np.random.uniform(1.5, 2.5, n) ** 2 + np.sum(U * V, axis=1)
 
-  return (Spleaf(A, U, V, phi, offsetrow, b, F))
+  return Spleaf(A, U, V, phi, offsetrow, b, F)
 
 
 def _generate_random_param(C, seed=1):
   np.random.seed(seed)
 
   U = np.random.uniform(0.5, 1.5, (n, r))
   V = np.random.uniform(0.5, 1.5, (n, r))
   log10phi = np.random.uniform(-4, 0, (n - 1, r))
   phi = 10**log10phi
 
   nF = C.offsetrow[-1] + n - 1
-  F = np.random.uniform(0.25, 0.5, nF)**2
+  F = np.random.uniform(0.25, 0.5, nF) ** 2
 
-  A = np.random.uniform(1.5, 2.5, n)**2 + np.sum(U * V, axis=1)
+  A = np.random.uniform(1.5, 2.5, n) ** 2 + np.sum(U * V, axis=1)
 
   return (A, U, V, phi, F)
 
 
 def test_Spleaf():
   C = _generate_random_C()
 
   C_full = C.expand()
   L_full = C.expandL()
   D_full = np.diag(C.D)
 
   LDLt_full = L_full @ D_full @ L_full.T
   err = np.max(np.abs(C_full - LDLt_full))
-  assert err < prec, ('Cholesky decomposition not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'Cholesky decomposition not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
 
 def test_set_param():
   C = _generate_random_C()
   A, U, V, phi, F = _generate_random_param(C)
   Cb = Spleaf(A, U, V, phi, C.offsetrow, C.b, F)
   C.set_param(A, U, V, phi, F)
@@ -69,115 +74,123 @@
   L_full = C.expandL()
   Lb_full = Cb.expandL()
 
   err = np.max(np.abs(C_full - Cb_full))
   err = max(err, np.max(np.abs(L_full - Lb_full)))
   err = max(err, np.max(np.abs(C.D - Cb.D)))
 
-  assert err < prec, ('set_param not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'set_param not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
 
 def test_expandInv():
   C = _generate_random_C()
 
   C_full = C.expand()
   invC_full = C.expandInv()
 
   CinvC_full = C_full @ invC_full
   err = np.max(np.abs(CinvC_full - np.identity(n)))
-  assert err < prec, ('Inversion not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'Inversion not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
 
 def test_expandInvL():
   C = _generate_random_C()
 
   L_full = C.expandL()
   invL_full = C.expandInvL()
 
   LinvL_full = L_full @ invL_full
   err = np.max(np.abs(LinvL_full - np.identity(n)))
-  assert err < prec, ('Cholesky inversion not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'Cholesky inversion not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
 
 def test_logdet():
   C = _generate_random_C()
 
   logdet = C.logdet()
 
   C_full = C.expand()
   sign_full, logdet_full = np.linalg.slogdet(C_full)
 
   err = abs(logdet / logdet_full - 1)
 
   assert sign_full > 0, 'logdet is not positive'
-  assert err < prec, ('logdet not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, ('logdet not working' ' at required precision ({} > {})').format(
+    err, prec
+  )
 
 
 def test_dotL():
   C = _generate_random_C()
   x = np.random.normal(0.0, 1.0, C.n)
 
   y = C.dotL(x)
 
   L_full = C.expandL()
   y_full = L_full.dot(x)
 
   err = np.max(np.abs(y - y_full))
 
-  assert err < prec, ('dotL not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, ('dotL not working' ' at required precision ({} > {})').format(
+    err, prec
+  )
 
 
 def test_solveL():
   C = _generate_random_C()
   y = np.random.normal(0.0, 5.0, C.n)
 
   x = C.solveL(y)
 
   L_full = C.expandL()
   x_full = np.linalg.solve(L_full, y)
 
   err = np.max(np.abs(x - x_full))
 
-  assert err < prec, ('solveL not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, ('solveL not working' ' at required precision ({} > {})').format(
+    err, prec
+  )
 
 
 def test_dotLT():
   C = _generate_random_C()
   x = np.random.normal(0.0, 1.0, C.n)
 
   y = C.dotLT(x)
 
   L_full = C.expandL()
   y_full = L_full.T.dot(x)
 
   err = np.max(np.abs(y - y_full))
 
-  assert err < prec, ('dotL not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, ('dotL not working' ' at required precision ({} > {})').format(
+    err, prec
+  )
 
 
 def test_solveLT():
   C = _generate_random_C()
   y = np.random.normal(0.0, 5.0, C.n)
 
   x = C.solveLT(y)
 
   L_full = C.expandL()
   x_full = np.linalg.solve(L_full.T, y)
 
   err = np.max(np.abs(x - x_full))
 
-  assert err < prec, ('solveL not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, ('solveL not working' ' at required precision ({} > {})').format(
+    err, prec
+  )
 
 
 def _test_method_back(method):
   """
   Common code for testing dotL_back, solveL_back, dotLT_back, solveLT_back
   """
   C = _generate_random_C()
@@ -201,16 +214,17 @@
       grad_a_num_dx.append(db @ grad_b / dx)
       a[k] -= dx
     grad_a_num.append(grad_a_num_dx)
   grad_a_num = np.array(grad_a_num)
   err = np.max(np.abs(grad_a - np.mean(grad_a_num, axis=0)))
   num_err = np.max(np.abs(grad_a_num[1] - grad_a_num[0]))
   err = max(0.0, err - num_err)
-  assert err < prec, ('{}_back (a) not working'
-    ' at required precision ({} > {})').format(method, err, prec)
+  assert err < prec, (
+    '{}_back (a) not working' ' at required precision ({} > {})'
+  ).format(method, err, prec)
 
   # grad_param
   kwargs = {'A': C.A, 'U': C.U, 'V': C.V, 'phi': C.phi, 'F': C.F}
   for kparam, param in enumerate(['A', 'U', 'V', 'phi', 'F']):
     grad_param_num = []
     for dx in [delta, -delta]:
       grad_param_num_dx = []
@@ -222,20 +236,20 @@
         db = getattr(C, method)(a) - b
         grad_param_num_dx.append(db @ grad_b / dx)
         Cparam.flat[k] -= dx
       kwargs[param] = Cparam
       C.set_param(**kwargs)
       grad_param_num.append(grad_param_num_dx)
     grad_param_num = np.array(grad_param_num)
-    err = np.max(
-      np.abs(grad_param[kparam].flat - np.mean(grad_param_num, axis=0)))
+    err = np.max(np.abs(grad_param[kparam].flat - np.mean(grad_param_num, axis=0)))
     num_err = np.max(np.abs(grad_param_num[1] - grad_param_num[0]))
     err = max(0.0, err - num_err)
-    assert err < prec, ('{}_back ({}) not working'
-      ' at required precision ({} > {})').format(method, param, err, prec)
+    assert err < prec, (
+      '{}_back ({}) not working' ' at required precision ({} > {})'
+    ).format(method, param, err, prec)
 
 
 def test_dotL_back():
   _test_method_back('dotL')
 
 
 def test_solveL_back():
@@ -258,16 +272,17 @@
 
   C_full = C.expand()
   invC_full = np.linalg.inv(C_full)
   chi2_full = y.T @ invC_full @ y
 
   err = abs(chi2 - chi2_full)
 
-  assert err < prec, ('chi2 not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, ('chi2 not working' ' at required precision ({} > {})').format(
+    err, prec
+  )
 
 
 def test_loglike():
   C = _generate_random_C()
   y = np.random.normal(0.0, 5.0, C.n)
 
   loglike = C.loglike(y)
@@ -275,16 +290,17 @@
   C_full = C.expand()
   invC_full = np.linalg.inv(C_full)
   chi2_full = y.T @ invC_full @ y
   _, logdet_full = np.linalg.slogdet(C_full)
   loglike_full = -0.5 * (chi2_full + logdet_full + C.n * np.log(2.0 * np.pi))
 
   err = abs(loglike - loglike_full)
-  assert err < prec, ('loglike not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, ('loglike not working' ' at required precision ({} > {})').format(
+    err, prec
+  )
 
 
 def _test_method_grad(method):
   """
   Common code for testing chi2_grad, loglike_grad
   """
   C = _generate_random_C()
@@ -304,16 +320,17 @@
       f_grad_num_dx.append(df / dx)
       y[k] -= dx
     f_grad_num.append(f_grad_num_dx)
   f_grad_num = np.array(f_grad_num)
   err = np.max(np.abs(f_grad_res - np.mean(f_grad_num, axis=0)))
   num_err = np.max(np.abs(f_grad_num[1] - f_grad_num[0]))
   err = max(0.0, err - num_err)
-  assert err < prec, ('{}_grad (y) not working'
-    ' at required precision ({} > {})').format(method, err, prec)
+  assert err < prec, (
+    '{}_grad (y) not working' ' at required precision ({} > {})'
+  ).format(method, err, prec)
 
   # grad_param
   kwargs = {'A': C.A, 'U': C.U, 'V': C.V, 'phi': C.phi, 'F': C.F}
   for kparam, param in enumerate(['A', 'U', 'V', 'phi', 'F']):
     f_grad_num = []
     for dx in [delta, -delta]:
       f_grad_num_dx = []
@@ -325,20 +342,20 @@
         df = getattr(C, method)(y) - f
         f_grad_num_dx.append(df / dx)
         Cparam.flat[k] -= dx
       kwargs[param] = Cparam
       C.set_param(**kwargs)
       f_grad_num.append(f_grad_num_dx)
     f_grad_num = np.array(f_grad_num)
-    err = np.max(
-      np.abs(f_grad_param[kparam].flat - np.mean(f_grad_num, axis=0)))
+    err = np.max(np.abs(f_grad_param[kparam].flat - np.mean(f_grad_num, axis=0)))
     num_err = np.max(np.abs(f_grad_num[1] - f_grad_num[0]))
     err = max(0.0, err - num_err)
-    assert err < prec, ('{}_grad ({}) not working'
-      ' at required precision ({} > {})').format(method, param, err, prec)
+    assert err < prec, (
+      '{}_grad ({}) not working' ' at required precision ({} > {})'
+    ).format(method, param, err, prec)
 
 
 def test_chi2_grad():
   _test_method_grad('chi2')
 
 
 def test_loglike_grad():
@@ -358,61 +375,70 @@
   offsetrow = np.cumsum(b - 1) + 1
   F = np.zeros(0)
   K_full = Spleaf(A, C.U, C.V, C.phi, offsetrow, b, F).expand()
   mu_full = K_full @ np.linalg.solve(C_full, y)
   cov_full = K_full - K_full @ np.linalg.inv(C_full) @ K_full
 
   err = np.max(np.abs(mu - mu_full))
-  assert err < prec, ('conditional mean not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'conditional mean not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
   err = np.max(np.abs(muv - mu_full))
-  assert err < prec, ('conditional mean not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'conditional mean not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
   err = np.max(np.abs(muc - mu_full))
-  assert err < prec, ('conditional mean not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'conditional mean not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
   err = np.max(np.abs(var - np.diag(cov_full)))
-  assert err < prec, ('conditional var not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'conditional var not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
   err = np.max(np.abs(cov - cov_full))
-  assert err < prec, ('conditional cov not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'conditional cov not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
 
 def test_conditional():
   C = _generate_random_C()
   y = C.sample()
   mu_self, cov_self = C.self_conditional(y, True)
   _, var_self = C.self_conditional(y, 'diag')
 
   ref = np.arange(C.n)
   phi2left = np.ones((C.n, C.r))
   phi2right = np.concatenate((C.phi, np.ones((1, C.r))))
 
   mu = C.conditional(y, C.U, C.V, C.phi, ref, phi2left, phi2right)
-  muv, var = C.conditional(y, C.U, C.V, C.phi, ref, phi2left, phi2right,
-    'diag')
+  muv, var = C.conditional(y, C.U, C.V, C.phi, ref, phi2left, phi2right, 'diag')
   muc, cov = C.conditional(y, C.U, C.V, C.phi, ref, phi2left, phi2right, True)
 
   err = np.max(np.abs(mu - mu_self))
-  assert err < prec, ('conditional mean not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'conditional mean not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
   err = np.max(np.abs(muv - mu_self))
-  assert err < prec, ('conditional mean not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'conditional mean not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
   err = np.max(np.abs(muc - mu_self))
-  assert err < prec, ('conditional mean not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'conditional mean not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
   err = np.max(np.abs(var - var_self))
-  assert err < prec, ('conditional var not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'conditional var not working' ' at required precision ({} > {})'
+  ).format(err, prec)
 
   err = np.max(np.abs(cov - cov_self))
-  assert err < prec, ('conditional cov not working'
-    ' at required precision ({} > {})').format(err, prec)
+  assert err < prec, (
+    'conditional cov not working' ' at required precision ({} > {})'
+  ).format(err, prec)
```

