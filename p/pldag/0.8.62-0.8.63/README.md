# Comparing `tmp/pldag-0.8.62.tar.gz` & `tmp/pldag-0.8.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pldag-0.8.62.tar", max compression
+gzip compressed data, was "pldag-0.8.63.tar", max compression
```

## Comparing `pldag-0.8.62.tar` & `pldag-0.8.63.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11356 2024-05-29 06:53:14.527873 pldag-0.8.62/LICENSE
--rw-r--r--   0        0        0     2833 2024-05-29 06:53:14.528024 pldag-0.8.62/README.md
--rw-r--r--   0        0        0    46472 2024-05-29 14:53:40.756937 pldag-0.8.62/pldag/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 06:53:14.528571 pldag-0.8.62/pldag/solver/__init__.py
--rw-r--r--   0        0        0     1045 2024-05-31 11:04:24.708263 pldag-0.8.62/pldag/solver/glpk_solver.py
--rw-r--r--   0        0        0      400 2024-05-31 11:04:43.204200 pldag-0.8.62/pyproject.toml
--rw-r--r--   0        0        0     3325 1970-01-01 00:00:00.000000 pldag-0.8.62/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-29 06:53:14.527873 pldag-0.8.63/LICENSE
+-rw-r--r--   0        0        0     2833 2024-05-29 06:53:14.528024 pldag-0.8.63/README.md
+-rw-r--r--   0        0        0    46514 2024-05-31 11:08:02.519447 pldag-0.8.63/pldag/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 06:53:14.528571 pldag-0.8.63/pldag/solver/__init__.py
+-rw-r--r--   0        0        0     1045 2024-05-31 11:04:24.708263 pldag-0.8.63/pldag/solver/glpk_solver.py
+-rw-r--r--   0        0        0      400 2024-05-31 11:08:08.145142 pldag-0.8.63/pyproject.toml
+-rw-r--r--   0        0        0     3325 1970-01-01 00:00:00.000000 pldag-0.8.63/PKG-INFO
```

### Comparing `pldag-0.8.62/LICENSE` & `pldag-0.8.63/LICENSE`

 * *Files identical despite different names*

### Comparing `pldag-0.8.62/README.md` & `pldag-0.8.63/README.md`

 * *Files identical despite different names*

### Comparing `pldag-0.8.62/pldag/__init__.py` & `pldag-0.8.63/pldag/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1051,15 +1051,15 @@
     
     def cut_sub(self, cuts: Dict[str, str], roots: List[str]) -> "PLDAG":
         """
             Cuts graph on given nodes in `cuts` and then creates a sub graph from the given root IDs.
         """
         return self.cut(cuts).sub(roots)
     
-    def solve(self, objectives: List[Dict[str, int]], assume: Dict[str, complex], solver: Solver, double_bind_constraints: bool = True) -> List[Dict[str, complex]]:
+    def solve(self, objectives: List[Dict[str, int]], assume: Dict[str, complex], solver: Solver, double_bind_constraints: bool = True, minimize: bool = True) -> List[Dict[str, complex]]:
         """
             Solves the model with the given objectives.
 
             Parameters
             ----------
             objectives : List[Dict[str, int]]
                 The objectives to solve for.
@@ -1093,15 +1093,15 @@
         variables = self._col_vars
         obj_mat = np.zeros((len(objectives), len(variables)), dtype=np.int64)
         for i, obj in enumerate(objectives):
             obj_mat[i, [self._col(k) for k in obj]] = list(obj.values())
 
         if solver == Solver.GLPK:
             from pldag.solver.glpk_solver import solve_lp
-            solutions = solve_lp(A, b, obj_mat, set(np.argwhere((self._dvec.real != 0) | (self._dvec.imag != 1)).T[0].tolist()))
+            solutions = solve_lp(A, b, obj_mat, set(np.argwhere((self._dvec.real != 0) | (self._dvec.imag != 1)).T[0].tolist()), minimize=minimize)
         else:
             raise ValueError(f"Solver `{solver}` not installed.")
         
         return list(
             map(
                 lambda solution: dict(
                     zip(
```

### Comparing `pldag-0.8.62/pldag/solver/glpk_solver.py` & `pldag-0.8.63/pldag/solver/glpk_solver.py`

 * *Files identical despite different names*

### Comparing `pldag-0.8.62/PKG-INFO` & `pldag-0.8.63/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pldag
-Version: 0.8.62
+Version: 0.8.63
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

