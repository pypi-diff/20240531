# Comparing `tmp/pldag-0.8.61.tar.gz` & `tmp/pldag-0.8.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pldag-0.8.61.tar", max compression
+gzip compressed data, was "pldag-0.8.62.tar", max compression
```

## Comparing `pldag-0.8.61.tar` & `pldag-0.8.62.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11356 2024-05-29 06:53:14.527873 pldag-0.8.61/LICENSE
--rw-r--r--   0        0        0     2833 2024-05-29 06:53:14.528024 pldag-0.8.61/README.md
--rw-r--r--   0        0        0    46472 2024-05-29 14:53:40.756937 pldag-0.8.61/pldag/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 06:53:14.528571 pldag-0.8.61/pldag/solver/__init__.py
--rw-r--r--   0        0        0     1021 2024-05-29 06:53:14.528701 pldag-0.8.61/pldag/solver/glpk_solver.py
--rw-r--r--   0        0        0      400 2024-05-29 14:53:53.269697 pldag-0.8.61/pyproject.toml
--rw-r--r--   0        0        0     3325 1970-01-01 00:00:00.000000 pldag-0.8.61/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-29 06:53:14.527873 pldag-0.8.62/LICENSE
+-rw-r--r--   0        0        0     2833 2024-05-29 06:53:14.528024 pldag-0.8.62/README.md
+-rw-r--r--   0        0        0    46472 2024-05-29 14:53:40.756937 pldag-0.8.62/pldag/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 06:53:14.528571 pldag-0.8.62/pldag/solver/__init__.py
+-rw-r--r--   0        0        0     1045 2024-05-31 11:04:24.708263 pldag-0.8.62/pldag/solver/glpk_solver.py
+-rw-r--r--   0        0        0      400 2024-05-31 11:04:43.204200 pldag-0.8.62/pyproject.toml
+-rw-r--r--   0        0        0     3325 1970-01-01 00:00:00.000000 pldag-0.8.62/PKG-INFO
```

### Comparing `pldag-0.8.61/LICENSE` & `pldag-0.8.62/LICENSE`

 * *Files identical despite different names*

### Comparing `pldag-0.8.61/README.md` & `pldag-0.8.62/README.md`

 * *Files identical despite different names*

### Comparing `pldag-0.8.61/pldag/__init__.py` & `pldag-0.8.62/pldag/__init__.py`

 * *Files identical despite different names*

### Comparing `pldag-0.8.61/pldag/solver/glpk_solver.py` & `pldag-0.8.62/pldag/solver/glpk_solver.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 from .. import NoSolutionsException
 
 try:
     import npycvx
 except ImportError:
     raise ImportError("Please install the npycvx package to use GLPK solver module.")
 
-def solve_lp(A: np.ndarray, b: np.ndarray, objectives: np.ndarray, int_vrs: set=set()):
+def solve_lp(A: np.ndarray, b: np.ndarray, objectives: np.ndarray, int_vrs: set=set(), minimize: bool=True):
     """
     Solve the linear programming problem:
     minimize c^T x
     subject to Ax >= b
 
     for each c in objectives.
     """
 
     # Load solve-function with the now converted numpy
     # matrices/vectors into cvxopt data type...
     solve_part_fn = functools.partial(
         npycvx.solve_lp, 
         *npycvx.convert_numpy(A, b, int_vrs=int_vrs), 
-        False
+        minimize
     )
 
     # Exectue each objective with solver function
     solutions = list(
         map(
             solve_part_fn, 
             objectives
```

### Comparing `pldag-0.8.61/PKG-INFO` & `pldag-0.8.62/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pldag
-Version: 0.8.61
+Version: 0.8.62
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

