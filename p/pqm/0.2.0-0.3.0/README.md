# Comparing `tmp/pqm-0.2.0.tar.gz` & `tmp/pqm-0.3.0.tar.gz`

## Comparing `pqm-0.2.0.tar` & `pqm-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 pqm-0.2.0/requirements.txt
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 pqm-0.2.0/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 pqm-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0    83241 2020-02-02 00:00:00.000000 pqm-0.2.0/notebooks/mnist.ipynb
--rw-r--r--   0        0        0   136091 2020-02-02 00:00:00.000000 pqm-0.2.0/notebooks/test.ipynb
--rw-r--r--   0        0        0   195804 2020-02-02 00:00:00.000000 pqm-0.2.0/notebooks/time_series.ipynb
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pqm-0.2.0/src/pqm/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pqm-0.2.0/src/pqm/_version.py
--rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 pqm-0.2.0/src/pqm/pqm.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 pqm-0.2.0/src/pqm/test_gaussian.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 pqm-0.2.0/tests/test_gaussian.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pqm-0.2.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pqm-0.2.0/LICENSE
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 pqm-0.2.0/README.md
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 pqm-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 pqm-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 pqm-0.3.0/requirements.txt
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 pqm-0.3.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 pqm-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    83241 2020-02-02 00:00:00.000000 pqm-0.3.0/notebooks/mnist.ipynb
+-rw-r--r--   0        0        0   136091 2020-02-02 00:00:00.000000 pqm-0.3.0/notebooks/test.ipynb
+-rw-r--r--   0        0        0   195804 2020-02-02 00:00:00.000000 pqm-0.3.0/notebooks/time_series.ipynb
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pqm-0.3.0/src/pqm/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pqm-0.3.0/src/pqm/_version.py
+-rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 pqm-0.3.0/src/pqm/pqm.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 pqm-0.3.0/src/pqm/test_gaussian.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 pqm-0.3.0/tests/test_gaussian.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pqm-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pqm-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 pqm-0.3.0/README.md
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 pqm-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 pqm-0.3.0/PKG-INFO
```

### Comparing `pqm-0.2.0/.github/workflows/cd.yml` & `pqm-0.3.0/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `pqm-0.2.0/.github/workflows/ci.yml` & `pqm-0.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pqm-0.2.0/notebooks/mnist.ipynb` & `pqm-0.3.0/notebooks/mnist.ipynb`

 * *Files identical despite different names*

### Comparing `pqm-0.2.0/notebooks/test.ipynb` & `pqm-0.3.0/notebooks/test.ipynb`

 * *Files identical despite different names*

### Comparing `pqm-0.2.0/notebooks/time_series.ipynb` & `pqm-0.3.0/notebooks/time_series.ipynb`

 * *Files identical despite different names*

### Comparing `pqm-0.2.0/src/pqm/pqm.py` & `pqm-0.3.0/src/pqm/pqm.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 from typing import Optional
 
 import numpy as np
-from scipy.stats import chi2_contingency
+from scipy.stats import chi2_contingency, chi2
 from scipy.spatial import KDTree
 
 __all__ = ("pqm_chi2", "pqm_pvalue")
 
-def _pqm_test(x_samples: np.ndarray, y_samples: np.ndarray, num_refs: int):
+
+def _pqm_test(x_samples: np.ndarray, y_samples: np.ndarray, num_refs: int, whiten: bool):
     """
     Helper function to perform the PQM test and return the results from chi2_contingency.
 
     Parameters
     ----------
     x_samples : np.ndarray
         Samples from the first distribution, test samples.
     y_samples : np.ndarray
         Samples from the second distribution, reference samples.
     num_refs : int
         Number of reference samples to use.
+    whiten : bool
+        If True, whiten the samples by subtracting the mean and dividing by the standard deviation.
 
     Returns
     -------
     tuple
         Results from scipy.stats.chi2_contingency function.
     """
     if len(y_samples) < num_refs:
         raise ValueError(
             "Number of reference samples must be less than the number of true samples."
         )
     elif len(y_samples) < 2 * num_refs:
         print(
             "Warning: Number of y_samples is small (less than twice the number of reference samples). Result may have high variance."
         )
+    if whiten:
+        mean = np.mean(y_samples, axis=0)
+        std = np.std(y_samples, axis=0)
+        y_samples = (y_samples - mean) / std
+        x_samples = (x_samples - mean) / std
 
     refs = np.random.choice(len(y_samples), num_refs, replace=False)
     N = np.arange(len(y_samples))
     N[refs] = -1
     N = N[N >= 0]
     refs, y_samples = y_samples[refs], y_samples[N]
 
@@ -49,56 +57,85 @@
 
     # Remove reference samples with no counts
     C = (counts_x > 0) | (counts_y > 0)
     counts_x, counts_y = counts_x[C], counts_y[C]
 
     return chi2_contingency(np.array([counts_x, counts_y]))
 
-def pqm_pvalue(x_samples: np.ndarray, y_samples: np.ndarray, num_refs: int = 100, bootstrap: Optional[int] = None):
+
+def pqm_pvalue(
+    x_samples: np.ndarray,
+    y_samples: np.ndarray,
+    num_refs: int = 100,
+    bootstrap: Optional[int] = None,
+    whiten: bool = False,
+):
     """
     Perform the PQM test of the null hypothesis that `x_samples` and `y_samples` are drawn form the same distribution.
 
     Parameters
     ----------
     x_samples : np.ndarray
         Samples from the first distribution, test samples. Must have shape (N, *D) N is the number of x samples, and D is the dimensionality of the samples.
     y_samples : np.ndarray
         Samples from the second distribution, reference samples. Must have shape (M, *D) M is the number of y samples, and D is the dimensionality of the samples.
     num_refs : int
         Number of reference samples to use. Note that these will be drawn from y_samples, and then removed from the y_samples array.
     bootstrap : Optional[int]
         Number of bootstrap iterations to perform. No bootstrap if None (default).
+    whiten : bool
+        If True, whiten the samples by subtracting the mean and dividing by the standard deviation.
 
     Returns
     -------
     float or list
         pvalue(s). Null hypothesis that both samples are drawn from the same distribution.
     """
     if bootstrap is not None:
-        return [pqm_pvalue(x_samples, y_samples, num_refs=num_refs) for _ in range(bootstrap)]
-    _, pvalue, _, _ = _pqm_test(x_samples, y_samples, num_refs)
+        return [
+            pqm_pvalue(x_samples, y_samples, num_refs=num_refs, whiten=whiten)
+            for _ in range(bootstrap)
+        ]
+    _, pvalue, _, _ = _pqm_test(x_samples, y_samples, num_refs, whiten)
     return pvalue
 
-def pqm_chi2(x_samples: np.ndarray, y_samples: np.ndarray, num_refs: int = 100, bootstrap: Optional[int] = None):
+
+def pqm_chi2(
+    x_samples: np.ndarray,
+    y_samples: np.ndarray,
+    num_refs: int = 100,
+    bootstrap: Optional[int] = None,
+    whiten: bool = False,
+):
     """
     Perform the PQM test of the null hypothesis that `x_samples` and `y_samples` are drawn form the same distribution.
 
     Parameters
     ----------
     x_samples : np.ndarray
         Samples from the first distribution, test samples. Must have shape (N, *D) N is the number of x samples, and D is the dimensionality of the samples.
     y_samples : np.ndarray
         Samples from the second distribution, reference samples. Must have shape (M, *D) M is the number of y samples, and D is the dimensionality of the samples.
     num_refs : int
         Number of reference samples to use. Note that these will be drawn from y_samples, and then removed from the y_samples array.
     bootstrap : Optional[int]
         Number of bootstrap iterations to perform. No bootstrap if None (default).
+    whiten : bool
+        If True, whiten the samples by subtracting the mean and dividing by the standard deviation.
 
     Returns
     -------
     float or list
         chi2 statistic(s) and degree(s) of freedom.
     """
     if bootstrap is not None:
-        return [pqm_chi2(x_samples, y_samples, num_refs=num_refs) for _ in range(bootstrap)]
-    chi2_stat, _, dof, _ = _pqm_test(x_samples, y_samples, num_refs)
-    return chi2_stat, dof
+        return [
+            pqm_chi2(x_samples, y_samples, num_refs=num_refs, whiten=whiten)
+            for _ in range(bootstrap)
+        ]
+    chi2_stat, _, dof, _ = _pqm_test(x_samples, y_samples, num_refs, whiten)
+    if dof != num_refs - 1:
+        # Rescale chi2 to new value which has the same cumulative probability
+        cp = chi2.cdf(chi2_stat, dof)
+        chi2_stat = chi2.ppf(cp, num_refs - 1)
+        dof = num_refs - 1
+    return chi2_stat, dof
```

### Comparing `pqm-0.2.0/LICENSE` & `pqm-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pqm-0.2.0/README.md` & `pqm-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pqm-0.2.0/pyproject.toml` & `pqm-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pqm-0.2.0/PKG-INFO` & `pqm-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pqm
-Version: 0.2.0
+Version: 0.3.0
 Summary: Implemenation of the PQMass two sample test from Lemos et al. 2024
 Project-URL: Homepage, https://github.com/Ciela-Institute/PQM
 Project-URL: Documentation, https://github.com/Ciela-Institute/PQM
 Project-URL: Repository, https://github.com/Ciela-Institute/PQM
 Project-URL: Issues, https://github.com/Ciela-Institute/PQM/issues
 Author-email: Pablo Lemos <pablo.lemos@mila.quebec>, Connor Stone <connor.stone@umontreal.ca>, Sammy Sharief <sharief2@illinois.edu>
 License: MIT License
```

