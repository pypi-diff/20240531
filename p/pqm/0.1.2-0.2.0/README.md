# Comparing `tmp/pqm-0.1.2.tar.gz` & `tmp/pqm-0.2.0.tar.gz`

## Comparing `pqm-0.1.2.tar` & `pqm-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 pqm-0.1.2/requirements.txt
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 pqm-0.1.2/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 pqm-0.1.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 pqm-0.1.2/src/pqm/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pqm-0.1.2/src/pqm/_version.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 pqm-0.1.2/src/pqm/pqm.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 pqm-0.1.2/src/pqm/test_gaussian.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 pqm-0.1.2/tests/test_gaussian.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pqm-0.1.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pqm-0.1.2/LICENSE
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pqm-0.1.2/README.md
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 pqm-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 pqm-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 pqm-0.2.0/requirements.txt
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 pqm-0.2.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 pqm-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    83241 2020-02-02 00:00:00.000000 pqm-0.2.0/notebooks/mnist.ipynb
+-rw-r--r--   0        0        0   136091 2020-02-02 00:00:00.000000 pqm-0.2.0/notebooks/test.ipynb
+-rw-r--r--   0        0        0   195804 2020-02-02 00:00:00.000000 pqm-0.2.0/notebooks/time_series.ipynb
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pqm-0.2.0/src/pqm/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pqm-0.2.0/src/pqm/_version.py
+-rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 pqm-0.2.0/src/pqm/pqm.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 pqm-0.2.0/src/pqm/test_gaussian.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 pqm-0.2.0/tests/test_gaussian.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pqm-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pqm-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 pqm-0.2.0/README.md
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 pqm-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 pqm-0.2.0/PKG-INFO
```

### Comparing `pqm-0.1.2/.github/workflows/cd.yml` & `pqm-0.2.0/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `pqm-0.1.2/.github/workflows/ci.yml` & `pqm-0.2.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pqm-0.1.2/src/pqm/pqm.py` & `pqm-0.2.0/src/pqm/pqm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,33 @@
 from typing import Optional
 
 import numpy as np
 from scipy.stats import chi2_contingency
 from scipy.spatial import KDTree
 
-__all__ = "pqm_pvalue"
+__all__ = ("pqm_chi2", "pqm_pvalue")
 
-
-def pqm_pvalue(
-    x_samples: np.ndarray,
-    y_samples: np.ndarray,
-    num_refs: int = 100,
-    bootstrap: Optional[int] = None,
-):
+def _pqm_test(x_samples: np.ndarray, y_samples: np.ndarray, num_refs: int):
     """
-    Perform the PQM test of the null hypothesis that `x_samples` and `y_samples` are drawn form the same distribution.
+    Helper function to perform the PQM test and return the results from chi2_contingency.
 
     Parameters
     ----------
     x_samples : np.ndarray
-        Samples from the first distribution. Must have shape (N, *D) N is the number of x samples, and D is the dimensionality of the samples.
+        Samples from the first distribution, test samples.
     y_samples : np.ndarray
-        Samples from the second distribution. Must have shape (M, *D) M is the number of y samples, and D is the dimensionality of the samples.
+        Samples from the second distribution, reference samples.
     num_refs : int
-        Number of reference samples to use. Note that these will be drawn from y_samples, and then removed from the y_samples array.
-    bootstrap : Optional[int]
-        Number of bootstrap iterations to perform. No bootstrap if None (default).
+        Number of reference samples to use.
 
     Returns
     -------
-    float
-        pvalue. Null hypothesis that both samples are drawn from the same distribution.
+    tuple
+        Results from scipy.stats.chi2_contingency function.
     """
-    if bootstrap is not None:
-        return list(pqm_pvalue(x_samples, y_samples, num_refs=num_refs) for _ in range(bootstrap))
     if len(y_samples) < num_refs:
         raise ValueError(
             "Number of reference samples must be less than the number of true samples."
         )
     elif len(y_samples) < 2 * num_refs:
         print(
             "Warning: Number of y_samples is small (less than twice the number of reference samples). Result may have high variance."
@@ -57,9 +47,58 @@
     idx = tree.query(y_samples, k=1, workers=-1)[1]
     counts_y = np.bincount(idx, minlength=num_refs)
 
     # Remove reference samples with no counts
     C = (counts_x > 0) | (counts_y > 0)
     counts_x, counts_y = counts_x[C], counts_y[C]
 
-    _, pvalue, _, _ = chi2_contingency(np.array([counts_x, counts_y]))
+    return chi2_contingency(np.array([counts_x, counts_y]))
+
+def pqm_pvalue(x_samples: np.ndarray, y_samples: np.ndarray, num_refs: int = 100, bootstrap: Optional[int] = None):
+    """
+    Perform the PQM test of the null hypothesis that `x_samples` and `y_samples` are drawn form the same distribution.
+
+    Parameters
+    ----------
+    x_samples : np.ndarray
+        Samples from the first distribution, test samples. Must have shape (N, *D) N is the number of x samples, and D is the dimensionality of the samples.
+    y_samples : np.ndarray
+        Samples from the second distribution, reference samples. Must have shape (M, *D) M is the number of y samples, and D is the dimensionality of the samples.
+    num_refs : int
+        Number of reference samples to use. Note that these will be drawn from y_samples, and then removed from the y_samples array.
+    bootstrap : Optional[int]
+        Number of bootstrap iterations to perform. No bootstrap if None (default).
+
+    Returns
+    -------
+    float or list
+        pvalue(s). Null hypothesis that both samples are drawn from the same distribution.
+    """
+    if bootstrap is not None:
+        return [pqm_pvalue(x_samples, y_samples, num_refs=num_refs) for _ in range(bootstrap)]
+    _, pvalue, _, _ = _pqm_test(x_samples, y_samples, num_refs)
     return pvalue
+
+def pqm_chi2(x_samples: np.ndarray, y_samples: np.ndarray, num_refs: int = 100, bootstrap: Optional[int] = None):
+    """
+    Perform the PQM test of the null hypothesis that `x_samples` and `y_samples` are drawn form the same distribution.
+
+    Parameters
+    ----------
+    x_samples : np.ndarray
+        Samples from the first distribution, test samples. Must have shape (N, *D) N is the number of x samples, and D is the dimensionality of the samples.
+    y_samples : np.ndarray
+        Samples from the second distribution, reference samples. Must have shape (M, *D) M is the number of y samples, and D is the dimensionality of the samples.
+    num_refs : int
+        Number of reference samples to use. Note that these will be drawn from y_samples, and then removed from the y_samples array.
+    bootstrap : Optional[int]
+        Number of bootstrap iterations to perform. No bootstrap if None (default).
+
+    Returns
+    -------
+    float or list
+        chi2 statistic(s) and degree(s) of freedom.
+    """
+    if bootstrap is not None:
+        return [pqm_chi2(x_samples, y_samples, num_refs=num_refs) for _ in range(bootstrap)]
+    chi2_stat, _, dof, _ = _pqm_test(x_samples, y_samples, num_refs)
+    return chi2_stat, dof
```

### Comparing `pqm-0.1.2/LICENSE` & `pqm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pqm-0.1.2/pyproject.toml` & `pqm-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pqm-0.1.2/PKG-INFO` & `pqm-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pqm
-Version: 0.1.2
+Version: 0.2.0
 Summary: Implemenation of the PQMass two sample test from Lemos et al. 2024
 Project-URL: Homepage, https://github.com/Ciela-Institute/PQM
 Project-URL: Documentation, https://github.com/Ciela-Institute/PQM
 Project-URL: Repository, https://github.com/Ciela-Institute/PQM
 Project-URL: Issues, https://github.com/Ciela-Institute/PQM/issues
 Author-email: Pablo Lemos <pablo.lemos@mila.quebec>, Connor Stone <connor.stone@umontreal.ca>, Sammy Sharief <sharief2@illinois.edu>
 License: MIT License
@@ -40,24 +40,67 @@
 Requires-Dist: scipy
 Provides-Extra: dev
 Requires-Dist: pytest-cov<5,>=4.1; extra == 'dev'
 Requires-Dist: pytest-mock<4,>=3.12; extra == 'dev'
 Requires-Dist: pytest<9,>=8.0; extra == 'dev'
 Description-Content-Type: text/markdown
 
-# PQM
+# PQMass: Probabilistic Assessment of the Quality of Generative Models using Probability Mass Estimation
 
-Implementation of the PQMass two sample test from Lemos et al. 2024
+Implementation of the PQMass two sample test from Lemos et al. 2024 [here](https://arxiv.org/abs/2402.04355)
+
+## Install
+
+Just do:
+
+```
+pip install pqm
+```
 
 ## Usage
 
+This is the main use case:
+
 ```python
 from pqm import pqm_pvalue
 import numpy as np
 
 x_sample = np.random.normal(size = (500, 10))
 y_sample = np.random.normal(size = (400, 10))
 
+# To get pvalues from PQMass
 pvalues = pqm_pvalue(x_sample, y_sample, num_refs = 100, bootstrap = 50)
-
 print(np.mean(pvalues), np.std(pvalues))
-```
+
+# To get chi^2 from PQMass
+chi2_stat, dof = pqm_chi2(x_sample, y_sample, num_refs = 100, bootstrap = 50)
+print(np.mean(chi2_stat), np.std(chi2_stat))
+print(np.unqiue(dof)) # This should be the same as num_refs - 1, if it is not, we suggest you use pqm_pvalue
+```
+
+If your two samples are drawn from the same distribution, then the p-value should
+be drawn from the random uniform(0,1) distribution. This means that if you get a
+very small value (i.e., 1e-6), then you have failed the null hypothesis test, and
+the two samples are not drawn from the same distribution.
+
+For the chi^2 metric, given your two sets of samples, if they come from the same
+distribution, the histogram of your chi² values should follow the chi² distribution. 
+The peak of this distribution will be at DoF - 2, and the standard deviation will 
+be √(2 * DoF). If your histogram shifts to the right of the expected chi² distribution, 
+it suggests that the samples are out of distribution. Conversely, if the histogram shifts 
+to the left, it indicates potential duplication or memorization (particularly relevant 
+for generative models).
+
+Note that the chi^2 metric faces limitations if you have a few samples. A solution could
+be to use bootstrapping. Another such solution is to pqm_pvalue. We leave it to the user to 
+identify the best solution for their problem.
+
+## Developing
+
+If you're a developer then:
+
+```
+git clone git@github.com:Ciela-Institute/PQM.git
+cd PQM
+git checkout -b my-new-branch
+pip install -e .
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

