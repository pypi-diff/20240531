# Comparing `tmp/phasegen-0.0.8b0.tar.gz` & `tmp/phasegen-0.0.9b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phasegen-0.0.8b0.tar", max compression
+gzip compressed data, was "phasegen-0.0.9b0.tar", max compression
```

## Comparing `phasegen-0.0.8b0.tar` & `phasegen-0.0.9b0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      725 2024-04-23 11:44:03.428096 phasegen-0.0.8b0/README.md
--rw-r--r--   0        0        0     4814 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/__init__.py
--rw-r--r--   0        0        0    15356 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/coalescent_models.py
--rw-r--r--   0        0        0    14488 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/comparison.py
--rw-r--r--   0        0        0    37050 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/demography.py
--rw-r--r--   0        0        0    85998 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/distributions.py
--rw-r--r--   0        0        0     3278 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/expm.py
--rw-r--r--   0        0        0    27043 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/inference.py
--rw-r--r--   0        0        0     2378 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/lineage.py
--rw-r--r--   0        0        0     2751 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/locus.py
--rw-r--r--   0        0        0     2653 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/norms.py
--rw-r--r--   0        0        0    18837 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/rewards.py
--rw-r--r--   0        0        0     1121 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/serialization.py
--rw-r--r--   0        0        0    11106 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/spectrum.py
--rw-r--r--   0        0        0    29757 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/state_space.py
--rw-r--r--   0        0        0    53044 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/state_space_old.py
--rw-r--r--   0        0        0     1229 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/utils.py
--rw-r--r--   0        0        0     4478 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/visualization.py
--rw-r--r--   0        0        0      931 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/pyproject.toml
--rw-r--r--   0        0        0     1743 1970-01-01 00:00:00.000000 phasegen-0.0.8b0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-01 09:16:47.974886 phasegen-0.0.9b0/LICENSE
+-rw-r--r--   0        0        0      857 2024-05-01 09:16:47.974886 phasegen-0.0.9b0/README.md
+-rw-r--r--   0        0        0     4814 2024-05-01 09:16:47.986886 phasegen-0.0.9b0/phasegen/__init__.py
+-rw-r--r--   0        0        0    15356 2024-05-01 09:16:47.986886 phasegen-0.0.9b0/phasegen/coalescent_models.py
+-rw-r--r--   0        0        0    14488 2024-05-01 09:16:47.990886 phasegen-0.0.9b0/phasegen/comparison.py
+-rw-r--r--   0        0        0    37050 2024-05-01 09:16:47.990886 phasegen-0.0.9b0/phasegen/demography.py
+-rw-r--r--   0        0        0    91715 2024-05-01 09:16:47.990886 phasegen-0.0.9b0/phasegen/distributions.py
+-rw-r--r--   0        0        0     3278 2024-05-01 09:16:47.990886 phasegen-0.0.9b0/phasegen/expm.py
+-rw-r--r--   0        0        0    27043 2024-05-01 09:16:47.990886 phasegen-0.0.9b0/phasegen/inference.py
+-rw-r--r--   0        0        0     2378 2024-05-01 09:16:47.990886 phasegen-0.0.9b0/phasegen/lineage.py
+-rw-r--r--   0        0        0     2751 2024-05-01 09:16:47.990886 phasegen-0.0.9b0/phasegen/locus.py
+-rw-r--r--   0        0        0     2653 2024-05-01 09:16:47.990886 phasegen-0.0.9b0/phasegen/norms.py
+-rw-r--r--   0        0        0    18837 2024-05-01 09:16:47.990886 phasegen-0.0.9b0/phasegen/rewards.py
+-rw-r--r--   0        0        0     1121 2024-05-01 09:16:47.990886 phasegen-0.0.9b0/phasegen/serialization.py
+-rw-r--r--   0        0        0    11603 2024-05-01 09:16:47.990886 phasegen-0.0.9b0/phasegen/spectrum.py
+-rw-r--r--   0        0        0    29413 2024-05-01 09:16:47.990886 phasegen-0.0.9b0/phasegen/state_space.py
+-rw-r--r--   0        0        0    53044 2024-05-01 09:16:47.990886 phasegen-0.0.9b0/phasegen/state_space_old.py
+-rw-r--r--   0        0        0     1229 2024-05-01 09:16:47.990886 phasegen-0.0.9b0/phasegen/utils.py
+-rw-r--r--   0        0        0     4478 2024-05-01 09:16:47.990886 phasegen-0.0.9b0/phasegen/visualization.py
+-rw-r--r--   0        0        0      930 2024-05-01 09:16:47.990886 phasegen-0.0.9b0/pyproject.toml
+-rw-r--r--   0        0        0     1875 1970-01-01 00:00:00.000000 phasegen-0.0.9b0/PKG-INFO
```

### Comparing `phasegen-0.0.8b0/README.md` & `phasegen-0.0.9b0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # PhaseGen  <img align="right" width="100" src="https://raw.githubusercontent.com/Sendrowski/PhaseGen/master/docs/logo.png">
 
+[![codecov](https://codecov.io/gh/Sendrowski/PhaseGen/graph/badge.svg?token=RMCUGD6CAX)](https://codecov.io/gh/Sendrowski/PhaseGen)
 [![Documentation Status](https://readthedocs.org/projects/phasegen/badge/?version=latest)](https://phasegen.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/phasegen.svg)](https://badge.fury.io/py/phasegen)
 
 
 ``phasegen`` is a package for simulation and inference on exact solutions of coalescent distributions under diverse demographic scenarios. ``phasegen`` leverages phase-type theory and supports a wide range of demographic models and coalescent tree statistics.
 
 Please see the [documentation](https://phasegen.readthedocs.io/en/latest/) for all the details.
```

### Comparing `phasegen-0.0.8b0/phasegen/__init__.py` & `phasegen-0.0.9b0/phasegen/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 PhaseGen package.
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-04-09"
 
-__version__ = '0.0.8-beta'
+__version__ = '0.0.9-beta'
 
 import logging
 import os
 import sys
 
 import jsonpickle.ext.numpy as jsonpickle_numpy
 from tqdm import tqdm
```

### Comparing `phasegen-0.0.8b0/phasegen/coalescent_models.py` & `phasegen-0.0.9b0/phasegen/coalescent_models.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.8b0/phasegen/comparison.py` & `phasegen-0.0.9b0/phasegen/comparison.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.8b0/phasegen/demography.py` & `phasegen-0.0.9b0/phasegen/demography.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.8b0/phasegen/distributions.py` & `phasegen-0.0.9b0/phasegen/distributions.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import copy
 import itertools
 import logging
 from abc import ABC, abstractmethod
 from collections.abc import Mapping
 from functools import cached_property, cache
 from math import factorial
-from typing import Generator, List, Callable, Tuple, Dict, Collection, Iterable, Iterator
+from typing import Generator, List, Callable, Tuple, Dict, Collection, Iterable, Iterator, Optional
 
 import numpy as np
 from scipy.ndimage import gaussian_filter1d
 
 from .coalescent_models import StandardCoalescent, CoalescentModel, BetaCoalescent, DiracCoalescent
 from .demography import Demography, PopSizeChanges
 from .expm import Backend
@@ -362,19 +362,20 @@
     def quantile(self, q: float) -> float:
         """
         Get the qth quantile.
         """
         pass
 
     @abstractmethod
-    def pdf(self, t: float | np.ndarray) -> float | np.ndarray:
+    def pdf(self, t: float | np.ndarray, **kwargs) -> float | np.ndarray:
         """
         Density function.
 
         :param t: Value or values to evaluate the density function at.
+        :param kwargs: Additional keyword arguments.
         :return: Density.
         """
         pass
 
     def plot_cdf(
             self,
             ax: 'plt.Axes' = None,
@@ -419,38 +420,43 @@
             self,
             ax: 'plt.Axes' = None,
             t: np.ndarray = None,
             show: bool = True,
             file: str = None,
             clear: bool = True,
             label: str = None,
-            title: str = 'Tree height PDF'
+            title: str = 'Tree height PDF',
+            dx: float = None
     ) -> 'plt.Axes':
         """
         Plot density function.
 
         :param ax: The axes to plot on.
         :param t: Values to evaluate the density function at.
             By default, 200 evenly spaced values between 0 and the 99th percentile.
         :param show: Whether to show the plot.
         :param file: File to save the plot to.
         :param clear: Whether to clear the plot before plotting.
         :param label: Label for the plot.
         :param title: Title of the plot.
+        :param dx: Step size for numerical differentiation. By default, the 99th percentile divided by 1e10.
         :return: Axes.
         """
         from .visualization import Visualization
 
+        if dx is None:
+            dx = self.quantile(0.99) / 1e10
+
         if t is None:
             t = np.linspace(0, self.quantile(0.99), 200)
 
         return Visualization.plot(
             ax=ax,
             x=t,
-            y=self.pdf(t),
+            y=self.pdf(t, dx=dx),
             xlabel='t',
             ylabel='f(t)',
             label=label,
             file=file,
             show=show,
             clear=clear,
             title=title
@@ -582,101 +588,40 @@
             initializing the distribution or the time until almost sure absorption.
         :param center: Whether to center the moment around the mean.
         :param permute: For cross-moments, whether to average over all permutations of rewards. Default is ``True``,
             which will provide the correct cross-moment. If set to ``False``, the cross-moment will be conditioned on
             the order of rewards.
         :return: The kth moment
         """
-        if rewards is None:
-            rewards = [self.reward] * k
-
-        if k != len(rewards):
-            raise ValueError(f"Number of specified rewards for moment of order {k} must be {k}.")
-
-        if k == 0:
-            return 1
-
-        # center moments around the mean
-        if center and k > 1:
-
-            components = []
-
-            # first order moments
-            means = [
-                PhaseTypeDistribution.moment(
-                    self,
-                    k=1,
-                    rewards=(rewards[i],),
-                    start_time=start_time,
-                    end_time=end_time
-                ) for i in range(k)
-            ]
-
-            for i in range(k + 1):
-                # iterate over all possible subsets of rewards of size i
-                for indices in itertools.combinations(range(k), i):
-
-                    # joint moment
-                    mu_i = PhaseTypeDistribution.moment(
-                        self,
-                        k=i,
-                        rewards=tuple(rewards[j] for j in indices),
-                        start_time=start_time,
-                        end_time=end_time,
-                        center=False,
-                        permute=permute
-                    )
-
-                    # product of means of remaining rewards
-                    mu1 = np.prod([means[j] for j in range(k) if j not in indices])
-
-                    components += [(-1) ** (k - i) * mu_i * mu1]
-
-            return sum(components)
-
-        if permute:
-            # get all possible permutations of rewards
-            permutations = list(itertools.permutations(rewards))
-
-            # compute average over all permutations
-            return sum(self._raw_moment(k, r, start_time, end_time) for r in permutations) / len(permutations)
-
-        return self._raw_moment(k, rewards, start_time, end_time)
-
-    @cache
-    def _raw_moment(
-            self,
-            k: int,
-            rewards: Tuple[Reward, ...] = None,
-            start_time: float = None,
-            end_time: float = None
-    ) -> float:
-        """
-        Get the raw kth-order (non-central) moment. Note that for cross-moments, we need average over all possible
-        reward permutations.
-
-        :param k: The order of the moment.
-        :param rewards: Tuple of k rewards. By default, the reward of the underlying distribution.
-        :param start_time: Time when to start accumulation of moments. By default, the start time specified when
-            initializing the distribution.
-        :param end_time: Time when to end accumulation of moments. By default, either the end time specified when
-            initializing the distribution or the time until almost sure absorption.
-        :return: The kth moment
-        """
         if start_time is None:
             start_time = self.tree_height.start_time
 
         if end_time is None:
             end_time = self.tree_height.t_max
 
         if start_time > 0:
-            m_start, m_end = PhaseTypeDistribution.accumulate(self, k, [start_time, end_time], rewards)
+            m_start, m_end = PhaseTypeDistribution.accumulate(
+                self,
+                k=k,
+                end_times=[start_time, end_time],
+                rewards=rewards,
+                center=center,
+                permute=permute
+            )
+
             m = float(m_end - m_start)
         else:
-            m = float(PhaseTypeDistribution.accumulate(self, k, [end_time], rewards)[0])
+            m = float(PhaseTypeDistribution.accumulate(
+                self,
+                k=k,
+                end_times=[end_time],
+                rewards=rewards,
+                center=center,
+                permute=permute
+            )[0])
 
         if np.isnan(m):
             raise ValueError(
                 "NaN value encountered when computing moment. "
                 "This is likely due to an ill-conditioned rate matrix."
             )
 
@@ -713,30 +658,100 @@
                 f"min: {rates.min()}, max: {rates.max()}. "
                 f"This may potentially lead to numerical instability, despite matrix regularization."
             )
 
     def accumulate(
             self,
             k: int,
-            end_times: Iterable[float] | float,
-            rewards: Tuple[Reward, ...] = None
-    ) -> np.ndarray | float:
+            end_times: Iterable[float],
+            rewards: Tuple[Reward, ...] = None,
+            center: bool = True,
+            permute: bool = True
+    ) -> np.ndarray:
         """
         Evaluate the kth (non-central) moment at different end times.
 
         :param k: The order of the moment.
         :param end_times: List of ends times or end time when to evaluate the moment.
         :param rewards: Tuple of k rewards. By default, the reward of the underlying distribution.
+        :param center: Whether to center the moment around the mean.
+        :param permute: For cross-moments, whether to average over all permutations of rewards. Default is ``True``,
+            which will provide the correct cross-moment. If set to ``False``, the cross-moment will be conditioned on
+            the order of rewards.
         :return: The moment accumulated at the specified times or time.
         """
-        # handle scalar input
-        if not isinstance(end_times, Iterable):
-            return self.accumulate(k, [end_times], rewards)[0]
+        if rewards is None:
+            rewards = [self.reward] * k
 
-        end_times = np.array(list(end_times))
+        if k != len(rewards):
+            raise ValueError(f"Number of specified rewards for moment of order {k} must be {k}.")
+
+        if k == 0:
+            return np.ones_like(list(end_times))
+
+        # center moments around the mean
+        if center and k > 1:
+
+            components = []
+
+            # first order moments
+            means = [
+                PhaseTypeDistribution.accumulate(
+                    self,
+                    k=1,
+                    rewards=(rewards[i],),
+                    end_times=end_times
+                ) for i in range(k)
+            ]
+
+            for i in range(k + 1):
+                # iterate over all possible subsets of rewards of size i
+                for indices in itertools.combinations(range(k), i):
+                    # joint moment
+                    mu_i = PhaseTypeDistribution.accumulate(
+                        self,
+                        k=i,
+                        rewards=tuple(rewards[j] for j in indices),
+                        end_times=end_times,
+                        center=False,
+                        permute=permute
+                    )
+
+                    # product of means of remaining rewards
+                    mu1 = np.prod([means[j] for j in range(k) if j not in indices], axis=0)
+
+                    components += [(-1) ** (k - i) * mu_i * mu1]
+
+            return np.sum(components, axis=0)
+
+        if permute:
+            # get all possible permutations of rewards
+            permutations = list(itertools.permutations(rewards))
+
+            # compute average over all permutations
+            return np.sum([self._accumulate(k, tuple(end_times), r) for r in permutations], axis=0) / len(permutations)
+
+        return self._accumulate(k, tuple(end_times), rewards)
+
+    @cache
+    def _accumulate(
+            self,
+            k: int,
+            end_times: Tuple[float, ...],
+            rewards: Tuple[Reward, ...] = None
+    ) -> np.ndarray:
+        """
+        Evaluate the kth (non-central) moment at different end times.
+
+        :param k: The order of the moment.
+        :param end_times: Tuple of ends times or end time when to evaluate the moment.
+        :param rewards: Tuple of k rewards. By default, the reward of the underlying distribution.
+        :return: The moment accumulated at the specified times or time.
+        """
+        end_times = np.array(end_times)
 
         # check for negative values
         if np.any(end_times < 0):
             raise ValueError("Negative end times are not allowed.")
 
         # use default reward if not specified
         if rewards is None:
@@ -819,14 +834,16 @@
         return moments
 
     def plot_accumulation(
             self,
             k: int = 1,
             end_times: Iterable[float] = None,
             rewards: Tuple[Reward, ...] = None,
+            center: bool = True,
+            permute: bool = True,
             ax: 'plt.Axes' = None,
             show: bool = True,
             file: str = None,
             clear: bool = True,
             label: str = None,
             title: str = None
     ) -> 'plt.Axes':
@@ -836,14 +853,18 @@
         .. note:: This is different from a CDF, as it shows the accumulation of moments rather than the probability
             of having reached absorption at a certain time.
 
         :param k: The order of the moment.
         :param end_times: Times when to evaluate the moment. By default, 200 evenly spaced values between 0 and the
             99th percentile.
         :param rewards: Tuple of k rewards. By default, the reward of the underlying distribution.
+        :param center: Whether to center the moment around the mean.
+        :param permute: For cross-moments, whether to average over all permutations of rewards. Default is ``True``,
+            which will provide the correct cross-moment. If set to ``False``, the cross-moment will be conditioned on
+            the order of rewards.
         :param ax: The axes to plot on.
         :param show: Whether to show the plot.
         :param file: File to save the plot to.
         :param clear: Whether to clear the plot before plotting.
         :param label: Label for the plot.
         :param title: Title of the plot.
         :return: Axes.
@@ -855,18 +876,20 @@
 
         if rewards is None:
             rewards = (self.reward,) * k
 
         if title is None:
             title = f"Moment accumulation ({', '.join(r.__class__.__name__.replace('Reward', '') for r in rewards)})"
 
+        y = self.accumulate(k, end_times, rewards, center, permute)
+
         Visualization.plot(
             ax=ax,
             x=end_times,
-            y=self.accumulate(k, end_times, rewards),
+            y=y,
             xlabel='t',
             ylabel='moment',
             label=label,
             file=file,
             show=show,
             clear=clear,
             title=title
@@ -1101,23 +1124,26 @@
 
         # warn if maximum number of iterations reached
         if i - 1 == max_iter:
             raise RuntimeError("Maximum number of iterations reached when determining quantile.")
 
         return (a + b) / 2
 
-    def pdf(self, t: float | np.ndarray, dx: float = 1e-10) -> float | np.ndarray:
+    def pdf(self, t: float | np.ndarray, dx: float = None) -> float | np.ndarray:
         """
         Density function. We use numerical differentiation of the CDF to calculate the density. This provides good
         results as the CDF is exact and continuous.
 
         :param t: Value or values to evaluate the density function at.
-        :param dx: Step size for numerical differentiation.
+        :param dx: Step size for numerical differentiation. By default, the 99th percentile divided by 1e10.
         :return: Density
         """
+        if dx is None:
+            dx = self.quantile(0.99) / 1e10
+
         # determine (non-negative) evaluation points
         x1 = np.max([t - dx / 2, np.zeros_like(t)], axis=0)
         x2 = x1 + dx
 
         return (self.cdf(x2) - self.cdf(x1)) / dx
 
     @cached_property
@@ -1290,15 +1316,15 @@
             rewards: Tuple[SFSReward, ...] = None,
             start_time: float = None,
             end_time: float = None,
             center: bool = True,
             permute: bool = True
     ) -> float:
         """
-        Get the kth raw moment for the ith site-frequency count.
+        Get the kth moment for the ith site-frequency count.
 
         :param k: The order of the moment
         :param i: The ith site-frequency count
         :param rewards: Tuple of k rewards
         :param start_time: Time when to start accumulation of moments. By default, the start time specified when
             initializing the distribution.
         :param end_time: Time when to end accumulation of moments. By default, either the end time specified when
@@ -1318,28 +1344,31 @@
             center=center,
             permute=permute
         )
 
     def accumulate(
             self,
             k: int,
-            end_times: Iterable[float] | float,
-            rewards: Tuple[Reward, ...] = None
+            end_times: Iterable[float],
+            rewards: Tuple[Reward, ...] = None,
+            center: bool = True,
+            permute: bool = True
     ) -> np.ndarray:
         """
         Evaluate the kth (non-central) moments at different end times.
 
         :param k: The order of the moment.
         :param end_times: Times or time when to evaluate the moment.
         :param rewards: Tuple of k rewards. By default, the reward of the underlying distribution.
+        :param center: Whether to center the moment around the mean.
+        :param permute: For cross-moments, whether to average over all permutations of rewards. Default is ``True``,
+            which will provide the correct cross-moment. If set to ``False``, the cross-moment will be conditioned on
+            the order of rewards.
         :return: Array of moments accumulated at the specified times, one for each site-frequency count.
         """
-        if not isinstance(end_times, Iterable):
-            return self.accumulate(k, [end_times], rewards)[:, 0]
-
         indices = self._get_indices()
         end_times = np.array(list(end_times))
 
         accumulation = parallelize(
             func=lambda x: self.get_accumulation(*x),
             data=[[k, i, end_times, rewards] for i in indices],
             desc=f"Calculating accumulation of {k}-moments",
@@ -1355,14 +1384,16 @@
         ])
 
     def plot_accumulation(
             self,
             k: int = 1,
             end_times: Iterable[float] = None,
             rewards: Tuple[Reward, ...] = None,
+            center: bool = True,
+            permute: bool = True,
             ax: 'plt.Axes' = None,
             show: bool = True,
             file: str = None,
             clear: bool = True,
             label: str = None,
             title: str = None
     ) -> 'plt.Axes':
@@ -1372,14 +1403,18 @@
         .. note:: This is different from a CDF, as it shows the accumulation of moments rather than the probability
             of having reached absorption at a certain time.
 
         :param k: The order of the moment.
         :param end_times: Times when to evaluate the moment. By default, 200 evenly spaced values between 0 and
             the 99th percentile.
         :param rewards: Tuple of k rewards. By default, the reward of the underlying distribution.
+        :param center: Whether to center the moment around the mean.
+        :param permute: For cross-moments, whether to average over all permutations of rewards. Default is ``True``,
+            which will provide the correct cross-moment. If set to ``False``, the cross-moment will be conditioned on
+            the order of rewards.
         :param ax: The axes to plot on.
         :param show: Whether to show the plot.
         :param file: File to save the plot to.
         :param clear: Whether to clear the plot before plotting.
         :param label: Label for the plot.
         :param title: Title of the plot.
         :return: Axes.
@@ -1397,15 +1432,15 @@
             rewards = (self.reward,) * k
 
         if title is None:
             title = (f"SFS Moment accumulation "
                      f"({', '.join(r.__class__.__name__.replace('Reward', '') for r in rewards)})")
 
         # get accumulation of moments
-        accumulation = self.accumulate(k, end_times, rewards)
+        accumulation = self.accumulate(k, end_times, rewards, center, permute)
 
         for i, acc in zip(self._get_indices(), accumulation[1: -1]):
             Visualization.plot(
                 ax=ax,
                 x=end_times,
                 y=acc,
                 xlabel='t',
@@ -1420,32 +1455,40 @@
         return ax
 
     def get_accumulation(
             self,
             k: int,
             i: int,
             end_times: Iterable[float] | float,
-            rewards: Tuple[SFSReward, ...] = None
+            rewards: Tuple[SFSReward, ...] = None,
+            center: bool = True,
+            permute: bool = True
     ) -> np.ndarray | float:
         """
         Get accumulation of moments for the ith site-frequency count.
 
         :param k: The order of the moment
         :param i: The ith site-frequency count.
         :param end_times: Times or time when to evaluate the moment.
         :param rewards: Tuple of k rewards.
+        :param center: Whether to center the moment around the mean.
+        :param permute: For cross-moments, whether to average over all permutations of rewards. Default is ``True``,
+            which will provide the correct cross-moment. If set to ``False``, the cross-moment will be conditioned on
+            the order of rewards.
         :return: The kth SFS (cross)-moment accumulations at the ith site-frequency count
         """
         if rewards is None:
             rewards = [self.reward] * k
 
         return super().accumulate(
             k=k,
             end_times=end_times,
-            rewards=tuple([CombinedReward([r, self._get_sfs_reward(i)]) for r in rewards])
+            rewards=tuple([CombinedReward([r, self._get_sfs_reward(i)]) for r in rewards]),
+            center=center,
+            permute=permute
         )
 
     @cached_property
     def cov(self) -> SFS2:
         """
         Covariance matrix across site-frequency counts.
         """
@@ -1570,15 +1613,15 @@
         Get the indices for the site-frequency spectrum.
 
         :return: The indices.
         """
         return np.arange(1, self.lineage_config.n // 2 + 1)
 
 
-class EmpiricalDistribution(DensityAwareDistribution):
+class EmpiricalDistribution(DensityAwareDistribution):  # pragma: no cover
     """
     Probability distribution based on realisations.
     """
 
     def __init__(self, samples: np.ndarray | list):
         """
         Create object.
@@ -1728,15 +1771,15 @@
         # smooth using gaussian filter
         if sigma is not None:
             y = gaussian_filter1d(y, sigma=sigma)
 
         return y
 
 
-class EmpiricalSFSDistribution(EmpiricalDistribution):
+class EmpiricalSFSDistribution(EmpiricalDistribution):  # pragma: no cover
     """
     SFS probability distribution based on realisations.
     """
 
     def __init__(self, samples: np.ndarray | list):
         """
         Create object.
@@ -1777,22 +1820,22 @@
     def corr(self) -> SFS2:
         """
         Correlation matrix.
         """
         return SFS2(np.nan_to_num(np.corrcoef(self.samples, rowvar=False)))
 
 
-class DictContainer(dict):
+class DictContainer(dict):  # pragma: no cover
     """
     Dictionary container.
     """
     pass
 
 
-class EmpiricalPhaseTypeDistribution(EmpiricalDistribution):
+class EmpiricalPhaseTypeDistribution(EmpiricalDistribution):  # pragma: no cover
     """
     Phase-type distribution based on realisations.
     """
 
     def __init__(
             self,
             samples: np.ndarray | list,
@@ -1882,15 +1925,15 @@
 
         loci.cov = self.loci_cov
         loci.corr = self.loci_corr
 
         return loci
 
 
-class EmpiricalPhaseTypeSFSDistribution(EmpiricalPhaseTypeDistribution):
+class EmpiricalPhaseTypeSFSDistribution(EmpiricalPhaseTypeDistribution):  # pragma: no cover
     """
     SFS phase-type distribution based on realisations.
     """
 
     def __init__(
             self,
             samples: np.ndarray | list,
@@ -2175,14 +2218,16 @@
         )
 
     def _get_dist(self, k: int, rewards: Iterable[Reward] = None) -> PhaseTypeDistribution:
         """
         Get the kth-order phase-type distribution with state space inferred from the rewards.
         The returned phase-type distribution is configured with the unit reward.
 
+        :param k: Order of the moment.
+        :param rewards: Tuple of k rewards. By default, tree height rewards are used.
         :return: Distribution.
         """
         if rewards is None:
             rewards = [TreeHeightReward()] * k
 
         if Reward.support(DefaultStateSpace, rewards):
             state_space = self.default_state_space
@@ -2217,17 +2262,15 @@
             initializing the distribution or the time until almost sure absorption.
         :param center: Whether to center the moment.
         :param permute: For cross-moments, whether to average over all permutations of rewards. Default is ``True``,
             which will provide the correct cross-moment. If set to ``False``, the cross-moment will be conditioned on
             the order of rewards.
         :return: The kth moment
         """
-        dist = self._get_dist(k, rewards)
-
-        return dist.moment(
+        return self._get_dist(k, rewards).moment(
             k=k,
             rewards=rewards,
             start_time=start_time,
             end_time=end_time,
             center=center,
             permute=permute
         )
@@ -2246,17 +2289,98 @@
         :param rewards: Tuple of k rewards. By default, tree height rewards are used.
         :param start_time: Time when to start accumulation of moments. By default, the start time specified when
             initializing the distribution.
         :param end_time: Time when to end accumulation of moments. By default, either the end time specified when
             initializing the distribution or the time until almost sure absorption.
         :return: The kth raw moment
         """
-        dist = self._get_dist(k, rewards)
+        return self.moment(
+            k=k,
+            rewards=rewards,
+            start_time=start_time,
+            end_time=end_time,
+            center=False,
+            permute=False
+        )
 
-        return dist._raw_moment(k=k, rewards=rewards, start_time=start_time, end_time=end_time)
+    def accumulate(
+            self,
+            k: int,
+            end_times: Iterable[float],
+            rewards: Tuple[Reward, ...] = None,
+            center: bool = True,
+            permute: bool = True
+    ) -> np.ndarray:
+        """
+        Accumulate moments at different times.
+
+        :param k: The order of the moment.
+        :param end_times: Times when to evaluate the moment. By default, 200 evenly spaced values between 0 and
+            the 99th percentile.
+        :param rewards: Tuple of k rewards. By default, the reward of the underlying distribution.
+        :param center: Whether to center the moment around the mean.
+        :param permute: For cross-moments, whether to average over all permutations of rewards. Default is ``True``,
+            which will provide the correct cross-moment. If set to ``False``, the cross-moment will be conditioned on
+            the order of rewards.
+        :return: Accumulation of moments.
+        """
+        return self._get_dist(k, rewards).accumulate(
+            k=k,
+            end_times=end_times,
+            rewards=rewards,
+            center=center,
+            permute=permute
+        )
+
+    def plot_accumulation(
+            self,
+            k: int = 1,
+            end_times: Iterable[float] = None,
+            rewards: Tuple[Reward, ...] = None,
+            center: bool = True,
+            permute: bool = True,
+            ax: 'plt.Axes' = None,
+            show: bool = True,
+            file: str = None,
+            clear: bool = False,
+            label: str = None,
+            title: str = None
+    ) -> 'plt.Axes':
+        """
+        Plot the accumulation of moments.
+
+        :param k: The order of the moment.
+        :param end_times: Times when to evaluate the moment. By default, 200 evenly spaced values between 0 and
+            the 99th percentile.
+        :param rewards: Tuple of k rewards. By default, the reward of the underlying distribution.
+        :param center: Whether to center the moment around the mean.
+        :param permute: For cross-moments, whether to average over all permutations of rewards. Default is ``True``,
+            which will provide the correct cross-moment. If set to ``False``, the cross-moment will be conditioned on
+            the order of rewards.
+        :param ax: Axes to plot on.
+        :param show: Whether to show the plot.
+        :param file: File to save the plot to.
+        :param clear: Whether to clear the plot before plotting.
+        :param label: Label for the plot.
+        :param title: Title of the plot.
+        :return: Axes.
+        """
+        self._get_dist(k, rewards).plot_accumulation(
+            k=k,
+            end_times=end_times,
+            rewards=rewards,
+            center=center,
+            permute=permute,
+            ax=ax,
+            show=show,
+            file=file,
+            clear=clear,
+            label=label,
+            title=title
+        )
 
     def drop_cache(self):
         """
         Drop state space cache.
         """
         self.default_state_space.drop_cache()
         self.block_counting_state_space.drop_cache()
@@ -2301,15 +2425,16 @@
         return super(self.__class__, other).to_json()
 
     def _to_msprime(
             self,
             num_replicates: int = 10000,
             n_threads: int = 10,
             parallelize: bool = True,
-            record_migration: bool = False
+            record_migration: bool = False,
+            seed: int = None
     ) -> 'MsprimeCoalescent':
         """
         Convert to msprime coalescent.
 
         :param num_replicates: Number of replicates.
         :param n_threads: Number of threads.
         :param parallelize: Whether to parallelize.
@@ -2325,19 +2450,20 @@
             model=self.model,
             loci=self.locus_config,
             recombination_rate=self.locus_config.recombination_rate,
             end_time=self.end_time,
             num_replicates=num_replicates,
             n_threads=n_threads,
             parallelize=parallelize,
-            record_migration=record_migration
+            record_migration=record_migration,
+            seed=seed
         )
 
 
-class MsprimeCoalescent(AbstractCoalescent):
+class MsprimeCoalescent(AbstractCoalescent):  # pragma: no cover
     """
     Empirical coalescent distribution based on msprime simulations.
     """
 
     def __init__(
             self,
             n: int | Dict[str, int] | List[int] | LineageConfig,
@@ -2345,28 +2471,30 @@
             model: CoalescentModel = StandardCoalescent(),
             loci: int | LocusConfig = 1,
             recombination_rate: float = None,
             end_time: float = None,
             num_replicates: int = 10000,
             n_threads: int = 100,
             parallelize: bool = True,
-            record_migration: bool = False
+            record_migration: bool = False,
+            seed: int = None
     ):
         """
         Simulate data using msprime.
 
         :param n: Number of Lineages.
         :param demography: Demography.
         :param model: Coalescent model.
         :param loci: Number of loci or locus configuration.
         :param end_time: Time when to end the simulation.
         :param num_replicates: Number of replicates.
         :param n_threads: Number of threads.
         :param parallelize: Whether to parallelize.
         :param record_migration: Whether to record migrations which is necessary to calculate statistics per deme.
+        :param seed: Random seed.
         """
         super().__init__(
             n=n,
             model=model,
             loci=loci,
             recombination_rate=recombination_rate,
             demography=demography,
@@ -2377,14 +2505,15 @@
         self.total_branch_lengths: np.ndarray | None = None
         self.heights: np.ndarray | None = None
 
         self.num_replicates: int = num_replicates
         self.n_threads: int = n_threads
         self.parallelize: bool = parallelize
         self.record_migration: bool = record_migration
+        self.seed: int = seed
 
         self.p_accepted: int = 0
 
     def get_coalescent_model(self) -> 'msprime.AncestryModel':
         """
         Get the coalescent model.
 
@@ -2411,19 +2540,19 @@
         samples = self.lineage_config.lineage_dict
         demography = self.demography.to_msprime()
         model = self.get_coalescent_model()
         end_time = self.end_time
         n_pops = self.demography.n_pops
         sample_size = self.lineage_config.n
 
-        def simulate_batch(_) -> (np.ndarray, np.ndarray, np.ndarray):
+        def simulate_batch(seed: Optional[int]) -> (np.ndarray, np.ndarray, np.ndarray):
             """
             Simulate statistics.
 
-            :param _:
+            :param seed: Random seed.
             :return: Statistics.
             """
             import msprime as ms
             import tskit
 
             # simulate trees
             g: Generator = ms.sim_ancestry(
@@ -2431,15 +2560,16 @@
                 recombination_rate=self.locus_config.recombination_rate,
                 samples=samples,
                 num_replicates=num_replicates,
                 record_migrations=self.record_migration,
                 demography=demography,
                 model=model,
                 ploidy=1,
-                end_time=end_time
+                end_time=end_time,
+                random_seed=seed
             )
 
             # initialize variables
             heights = np.zeros((self.locus_config.n, n_pops, num_replicates), dtype=float)
             total_branch_lengths = np.zeros((self.locus_config.n, n_pops, num_replicates), dtype=float)
             sfs = np.zeros((self.locus_config.n, n_pops, num_replicates, sample_size + 1), dtype=float)
 
@@ -2519,15 +2649,15 @@
                             sfs[j, 0, i, n] += t
 
             return np.concatenate([[heights.T], [total_branch_lengths.T], sfs.T])
 
         # parallelize and add up results
         res = np.hstack(parallelize(
             func=simulate_batch,
-            data=[None] * self.n_threads,
+            data=[self.seed + i if self.seed is not None else None for i in range(self.n_threads)],
             parallelize=self.parallelize,
             batch_size=num_replicates,
             desc="Simulating trees"
         ))
 
         # store results
         self.heights, self.total_branch_lengths, self.sfs_counts = res[0].T, res[1].T, res[2:].T
```

### Comparing `phasegen-0.0.8b0/phasegen/expm.py` & `phasegen-0.0.9b0/phasegen/expm.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.8b0/phasegen/inference.py` & `phasegen-0.0.9b0/phasegen/inference.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.8b0/phasegen/lineage.py` & `phasegen-0.0.9b0/phasegen/lineage.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.8b0/phasegen/locus.py` & `phasegen-0.0.9b0/phasegen/locus.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.8b0/phasegen/norms.py` & `phasegen-0.0.9b0/phasegen/norms.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.8b0/phasegen/rewards.py` & `phasegen-0.0.9b0/phasegen/rewards.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.8b0/phasegen/serialization.py` & `phasegen-0.0.9b0/phasegen/serialization.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.8b0/phasegen/spectrum.py` & `phasegen-0.0.9b0/phasegen/spectrum.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,29 +31,29 @@
         Construct from data matrix.
         
         :param data:
         """
         data = np.array(data).copy()
 
         if data.ndim != 2:
-            raise AssertionError('Data has to be 2-dimensional')
+            raise ValueError('Data has to be 2-dimensional')
 
         if data.shape[0] != data.shape[1]:
-            raise AssertionError('Matrix has to be square.')
+            raise ValueError('Matrix has to be square.')
 
         self.n = data.shape[0]
 
         # width
         self.w = self.n // 2 + 1 if self.n % 2 == 1 else self.n // 2
 
         self.data = data
 
     def to_file(self, file):
         """
-        Save to file.
+        Save to file (in JSON format).
         
         :param file: File path.
         """
         with open(file, 'w') as f:
             f.write(self.to_json())
 
     def to_json(self) -> str:
@@ -65,14 +65,40 @@
         obj = copy.deepcopy(self)
 
         # convert numpy array to list
         obj.data = obj.data.tolist()
 
         return jsonpickle.encode(obj)
 
+    @staticmethod
+    def from_file(file: str) -> 'SFS2':
+        """
+        Load from file.
+
+        :param file: File path.
+        :return: SFS2
+        """
+        with open(file, 'r') as f:
+            return SFS2.from_json(f.read())
+
+    @staticmethod
+    def from_json(json: str) -> 'SFS2':
+        """
+        Load from JSON string.
+
+        :param json: JSON string.
+        :return: SFS2
+        """
+        obj = jsonpickle.decode(json)
+
+        # convert list to numpy array
+        obj.data = np.array(obj.data)
+
+        return obj
+
     def is_folded(self) -> bool:
         """
         Check if the 2-SFS is folded.
 
         :return: Whether the 2-SFS is folded.
         """
         return np.all(self.data == self.fold().data)
@@ -363,18 +389,17 @@
             norm=SymLogNorm(
                 linthresh=max_abs / 10,
                 vmin=-max_abs,
                 vmax=max_abs
             )
         )
 
-        if log_scale:
-            pass  # log scale currently doesn't work
-            # ax.yaxis.set_scale('log')
-            # ax.set_yscale('log', base=1.001)
+        # if log_scale:
+        # ax.yaxis.set_scale('log')
+        # ax.set_yscale('log', base=1.001)
 
         if title is not None:
             ax.set_title(title)
 
         if show:
             plt.show()
```

### Comparing `phasegen-0.0.8b0/phasegen/state_space.py` & `phasegen-0.0.9b0/phasegen/state_space.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 import logging
 import time
 from abc import ABC, abstractmethod
 from functools import cached_property
 from itertools import product
-from typing import List, Tuple, Dict, Callable, Iterable, cast
+from typing import List, Tuple, Dict, Callable, cast
 
 import numpy as np
 
 from .coalescent_models import CoalescentModel, StandardCoalescent
 from .demography import Epoch
 from .lineage import LineageConfig
 from .locus import LocusConfig
@@ -72,17 +72,14 @@
 
         #: Cached rate matrices
         self._cache: Dict[Epoch, Tuple[Dict[Tuple['State', 'State'], Tuple[float, str]], List['State']]] = {}
 
         #: Ordered list of states
         self.__states: List['State'] = []
 
-        #: State counter
-        self._i_state: int = 0
-
         # number of lineages linked across loci
         self.linked: np.ndarray | None = None
 
         # time in seconds to compute original rate matrix
         self.time: float | None = None
 
     @cached_property
@@ -149,18 +146,60 @@
 
     def get_transitions(self) -> Tuple[Dict[Tuple['State', 'State'], Tuple[float, str]], List['State']]:
         """
         Get all possible transitions from the given state.
 
         :return: All possible transitions from the given state.
         """
-        # reset state counter
-        self._i_state = 0
+        sources = [self._get_initial()]
+        transitions = {}
+        visited = []
+        i = 0
+
+        while True:
+
+            targets_new = {}
+
+            for source in sources:
+
+                # skip if source has been visited already
+                if source in visited:
+                    continue
+
+                # get all possible transitions from source
+                targets = self.transition.transit(source)
+
+                # add visited source state
+                visited += [source]
+
+                # add transitions to dictionary
+                for target, transition in targets.items():
+                    transitions[(source, target)] = transition
+
+                # add targets to new targets
+                targets_new |= targets
 
-        return self._get_transitions([self._get_initial()], {}, [])
+                # increment state counter
+                i += 1
+
+                if i in [1000, 10000, 100000]:
+                    levels = {1000: 'slow', 10000: 'very slow', 100000: 'extremely slow'}
+
+                    self._logger.warning(
+                        f'State space size exceeds {i} states. Computation may be {levels[i]}.'
+                    )
+
+            # break if no more targets
+            if len(targets_new) == 0:
+                break
+
+            # take new targets as source states
+            sources = tuple(targets_new.keys())
+
+        return transitions, visited
 
     @cached_property
     def e(self) -> np.ndarray:
         """
         Vector with ones of size ``k``.
         """
         return np.ones(self.k)
@@ -304,59 +343,14 @@
             S[ordering[source], ordering[target]] = transition[0]
 
         # fill diagonal with negative sum of row
         S[np.diag_indices_from(S)] = -np.sum(S, axis=1)
 
         return S
 
-    def _get_transitions(
-            self,
-            states: Iterable['State'],
-            transitions: Dict[Tuple['State', 'State'], Tuple[float, str]],
-            visited: List['State']
-    ) -> Tuple[Dict[Tuple['State', 'State'], Tuple[float, str]], List['State']]:
-        """
-        Get all possible transitions from the given states.
-
-        :param states: States.
-        :param transitions: Transitions.
-        :return: All possible transitions from the given state.
-        """
-        for source in states:
-
-            # skip if source has been visited
-            if source in visited:
-                continue
-
-            # get all possible transitions from source
-            targets = self.transition.transit(source)
-
-            # add visited source state
-            visited += [source]
-
-            # increment state counter
-            self._i_state += 1
-
-            if self._i_state in [1000, 10000, 100000]:
-
-                levels = {1000: 'slow', 10000: 'very slow', 100000: 'extremely slow'}
-
-                self._logger.warning(
-                    f'State space size exceeds {self._i_state} states. Computation may be {levels[self._i_state]}.'
-                )
-
-            # add transitions to dictionary
-            for target, transition in targets.items():
-                transitions[(source, target)] = transition
-
-            # get transitions from target states
-            self._get_transitions(targets.keys(), transitions, visited)
-
-        return transitions, visited
-
     def _get_sparsity(self) -> float:
         """
         Get the sparsity of the rate matrix.
 
         :return: The sparsity.
         """
         return 1 - np.count_nonzero(self.S) / self.S.size
```

### Comparing `phasegen-0.0.8b0/phasegen/state_space_old.py` & `phasegen-0.0.9b0/phasegen/state_space_old.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.8b0/phasegen/utils.py` & `phasegen-0.0.9b0/phasegen/utils.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.8b0/phasegen/visualization.py` & `phasegen-0.0.9b0/phasegen/visualization.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.8b0/pyproject.toml` & `phasegen-0.0.9b0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phasegen"
-version = "0.0.8-beta"
+version = "0.0.9-beta"
 description = "Simulation and inference on exact solutions of coalescent distributions under diverse demographic scenarios."
 authors = ["Sendrowski <sendrowski.janek@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
@@ -19,17 +19,17 @@
 tqdm = "^4.60.0"
 scipy = "^1.13.0"
 fastdfe = ">=1.1.3"
 
 # problems installing msprime with poetry
 [tool.poetry.group.dev.dependencies]
 urllib3 = "^1.26.0" # problems with poetry and urllib3 version 2
-sphinx-rtd-theme = "^1.2.0"
-sphinx-autodoc-typehints = "^1.23.0"
+sphinx-rtd-theme = "^2.0.0"
+sphinx-autodoc-typehints = "^2.1.0"
 sphinx-copybutton = "^0.5.2"
-myst-nb = "^0.17.2"
-sphinx = "5.3.0"
+myst-nb = "^1.1.0"
+sphinx = "^7.3.7"
 pygments = "^2.15.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `phasegen-0.0.8b0/PKG-INFO` & `phasegen-0.0.9b0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phasegen
-Version: 0.0.8b0
+Version: 0.0.9b0
 Summary: Simulation and inference on exact solutions of coalescent distributions under diverse demographic scenarios.
 License: MIT
 Author: Sendrowski
 Author-email: sendrowski.janek@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -22,14 +22,15 @@
 Requires-Dist: seaborn (>=0.13.0,<0.14.0)
 Requires-Dist: tqdm (>=4.60.0,<5.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # PhaseGen  <img align="right" width="100" src="https://raw.githubusercontent.com/Sendrowski/PhaseGen/master/docs/logo.png">
 
+[![codecov](https://codecov.io/gh/Sendrowski/PhaseGen/graph/badge.svg?token=RMCUGD6CAX)](https://codecov.io/gh/Sendrowski/PhaseGen)
 [![Documentation Status](https://readthedocs.org/projects/phasegen/badge/?version=latest)](https://phasegen.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/phasegen.svg)](https://badge.fury.io/py/phasegen)
 
 
 ``phasegen`` is a package for simulation and inference on exact solutions of coalescent distributions under diverse demographic scenarios. ``phasegen`` leverages phase-type theory and supports a wide range of demographic models and coalescent tree statistics.
 
 Please see the [documentation](https://phasegen.readthedocs.io/en/latest/) for all the details.
```

