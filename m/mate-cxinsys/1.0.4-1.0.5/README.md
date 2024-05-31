# Comparing `tmp/mate_cxinsys-1.0.4.tar.gz` & `tmp/mate_cxinsys-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mate_cxinsys-1.0.4.tar", last modified: Tue May 28 08:29:40 2024, max compression
+gzip compressed data, was "mate_cxinsys-1.0.5.tar", last modified: Fri May 31 08:48:25 2024, max compression
```

## Comparing `mate_cxinsys-1.0.4.tar` & `mate_cxinsys-1.0.5.tar`

### file list

```diff
@@ -1,30 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:29:40.519612 mate_cxinsys-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-28 08:29:32.000000 mate_cxinsys-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-28 08:29:40.519612 mate_cxinsys-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-05-28 08:29:32.000000 mate_cxinsys-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:29:40.515612 mate_cxinsys-1.0.4/mate/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-28 08:29:32.000000 mate_cxinsys-1.0.4/mate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:29:40.515612 mate_cxinsys-1.0.4/mate/array/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-28 08:29:32.000000 mate_cxinsys-1.0.4/mate/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21368 2024-05-28 08:29:32.000000 mate_cxinsys-1.0.4/mate/array/module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:29:40.515612 mate_cxinsys-1.0.4/mate/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 08:29:32.000000 mate_cxinsys-1.0.4/mate/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-28 08:29:32.000000 mate_cxinsys-1.0.4/mate/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-05-28 08:29:32.000000 mate_cxinsys-1.0.4/mate/mate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-28 08:29:32.000000 mate_cxinsys-1.0.4/mate/matelightning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:29:40.515612 mate_cxinsys-1.0.4/mate/transferentropy/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-28 08:29:32.000000 mate_cxinsys-1.0.4/mate/transferentropy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-05-28 08:29:32.000000 mate_cxinsys-1.0.4/mate/transferentropy/telightning.py
--rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-05-28 08:29:32.000000 mate_cxinsys-1.0.4/mate/transferentropy/transferentropy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:29:40.515612 mate_cxinsys-1.0.4/mate/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 08:29:32.000000 mate_cxinsys-1.0.4/mate/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-28 08:29:32.000000 mate_cxinsys-1.0.4/mate/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:29:40.519612 mate_cxinsys-1.0.4/mate_cxinsys.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-28 08:29:40.000000 mate_cxinsys-1.0.4/mate_cxinsys.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-28 08:29:40.000000 mate_cxinsys-1.0.4/mate_cxinsys.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 08:29:40.000000 mate_cxinsys-1.0.4/mate_cxinsys.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 08:29:40.000000 mate_cxinsys-1.0.4/mate_cxinsys.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 08:29:40.000000 mate_cxinsys-1.0.4/mate_cxinsys.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-28 08:29:40.000000 mate_cxinsys-1.0.4/mate_cxinsys.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 08:29:40.519612 mate_cxinsys-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-28 08:29:40.000000 mate_cxinsys-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:48:25.170103 mate_cxinsys-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-31 08:48:14.000000 mate_cxinsys-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-31 08:48:25.170103 mate_cxinsys-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-05-31 08:48:14.000000 mate_cxinsys-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:48:25.166103 mate_cxinsys-1.0.5/mate/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-31 08:48:14.000000 mate_cxinsys-1.0.5/mate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:48:25.166103 mate_cxinsys-1.0.5/mate/array/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-31 08:48:14.000000 mate_cxinsys-1.0.5/mate/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22053 2024-05-31 08:48:14.000000 mate_cxinsys-1.0.5/mate/array/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:48:25.166103 mate_cxinsys-1.0.5/mate/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-31 08:48:14.000000 mate_cxinsys-1.0.5/mate/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-31 08:48:14.000000 mate_cxinsys-1.0.5/mate/dataset/mlpair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-05-31 08:48:14.000000 mate_cxinsys-1.0.5/mate/mate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-31 08:48:14.000000 mate_cxinsys-1.0.5/mate/matelightning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:48:25.170103 mate_cxinsys-1.0.5/mate/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-31 08:48:14.000000 mate_cxinsys-1.0.5/mate/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-31 08:48:14.000000 mate_cxinsys-1.0.5/mate/preprocess/discretizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-31 08:48:14.000000 mate_cxinsys-1.0.5/mate/preprocess/discretizerfactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-31 08:48:14.000000 mate_cxinsys-1.0.5/mate/preprocess/interpdiscretizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-31 08:48:14.000000 mate_cxinsys-1.0.5/mate/preprocess/shiftdiscretizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-31 08:48:14.000000 mate_cxinsys-1.0.5/mate/preprocess/tagdiscretizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:48:25.170103 mate_cxinsys-1.0.5/mate/transferentropy/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-31 08:48:14.000000 mate_cxinsys-1.0.5/mate/transferentropy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-05-31 08:48:14.000000 mate_cxinsys-1.0.5/mate/transferentropy/telightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12093 2024-05-31 08:48:14.000000 mate_cxinsys-1.0.5/mate/transferentropy/transferentropy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:48:25.170103 mate_cxinsys-1.0.5/mate/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-31 08:48:14.000000 mate_cxinsys-1.0.5/mate/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-31 08:48:14.000000 mate_cxinsys-1.0.5/mate/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:48:25.170103 mate_cxinsys-1.0.5/mate_cxinsys.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-31 08:48:25.000000 mate_cxinsys-1.0.5/mate_cxinsys.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-31 08:48:25.000000 mate_cxinsys-1.0.5/mate_cxinsys.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 08:48:25.000000 mate_cxinsys-1.0.5/mate_cxinsys.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 08:48:25.000000 mate_cxinsys-1.0.5/mate_cxinsys.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 08:48:25.000000 mate_cxinsys-1.0.5/mate_cxinsys.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-31 08:48:25.000000 mate_cxinsys-1.0.5/mate_cxinsys.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 08:48:25.170103 mate_cxinsys-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-31 08:48:24.000000 mate_cxinsys-1.0.5/setup.py
```

### Comparing `mate_cxinsys-1.0.4/LICENSE` & `mate_cxinsys-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mate_cxinsys-1.0.4/PKG-INFO` & `mate_cxinsys-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mate-cxinsys
-Version: 1.0.4
+Version: 1.0.5
 Summary: MATE
 Home-page: https://github.com/cxinsys/mate
 Author: Complex Intelligent Systems Laboratory (CISLAB)
 Author-email: daewon4you@gmail.com
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mate_cxinsys-1.0.4/README.md` & `mate_cxinsys-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mate_cxinsys-1.0.4/mate/array/module.py` & `mate_cxinsys-1.0.5/mate/array/module.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,14 +99,17 @@
 
     def array(self, *args, **kwargs):
         return np.array(*args, **kwargs)
 
     def take(self, *args, **kwargs):
         return np.take(*args, **kwargs)
 
+    def take_along_axis(self, *args, **kwargs):
+        return np.take_along_axis(*args, **kwargs)
+
     def repeat(self, *args, **kwargs):
         return np.repeat(*args, **kwargs)
 
     def concatenate(self, *args, **kwargs):
         return np.concatenate(*args, **kwargs)
 
     def stack(self, *args, **kwargs):
@@ -197,14 +200,18 @@
         with cp.cuda.Device(self.device_id):
             return cp.array(*args, **kwargs)
 
     def take(self, *args, **kwargs):
         with cp.cuda.Device(self.device_id):
             return cp.take(*args, **kwargs)
 
+    def take_along_axis(self, *args, **kwargs):
+        with cp.cuda.Device(self.device_id):
+            return cp.take_along_axis(*args, **kwargs)
+
     def repeat(self, array, repeats):
         with cp.cuda.Device(self.device_id):
             repeats = cp.asnumpy(repeats).tolist()
             return cp.repeat(array, repeats)
 
     def concatenate(self, *args, **kwargs):
         with cp.cuda.Device(self.device_id):
@@ -338,14 +345,17 @@
 
     def array(self, *args, **kwargs):
         return device_put(jnp.array(*args, **kwargs), jax.devices()[self.device_id])
 
     def take(self, *args, **kwargs):
         return jnp.take(*args, **kwargs)
 
+    def take_along_axis(self, *args, **kwargs):
+        return jnp.take_along_axis(*args, **kwargs)
+
     def repeat(self, *args, **kwargs):
         return jnp.repeat(*args, **kwargs)
 
     def concatenate(self, *args, **kwargs):
         return jnp.concatenate(*args, **kwargs)
 
     def stack(self, *args, **kwargs):
@@ -435,14 +445,18 @@
 
     def take(self, *args, **kwargs):
         if len(args)+len(kwargs) == 3:
             return torch.index_select(args[0], kwargs['axis'], args[1])
         else:
             return torch.take(args[0], args[1])
 
+    def take_along_axis(self, *args, **kwargs):
+        val_dim = kwargs.pop('axis')
+        return torch.take_along_dim(args[0], args[1].to(torch.int64), dim=val_dim)
+
     def repeat(self, *args, **kwargs):
         return torch.repeat_interleave(*args, **kwargs)
 
     def concatenate(self, *args, **kwargs):
         val_dim = kwargs.pop('axis')
         return torch.concatenate(*args, **kwargs, dim=val_dim)
 
@@ -544,14 +558,18 @@
         with tf.device(f'/GPU:{self.device_id}'):
             tf.constant(*args, **kwargs)
 
     def take(self, *args, **kwargs):
         with tf.device(f'/GPU:{self.device_id}'):
             tf.gather(*args, **kwargs)
 
+    def take_along_axis(self, *args, **kwargs):
+        with tf.device(f'/GPU:{self.device_id}'):
+            tf.experimental.numpy.take_along_axis(*args, **kwargs)
+
     def repeat(self, *args, **kwargs):
         with tf.device(f'/GPU:{self.device_id}'):
             tf.repeat(*args, **kwargs)
 
     def concatenate(self, *args, **kwargs):
         with tf.device(f'/GPU:{self.device_id}'):
             tf.concat(*args, **kwargs)
```

### Comparing `mate_cxinsys-1.0.4/mate/dataset/dataset.py` & `mate_cxinsys-1.0.5/mate/dataset/mlpair.py`

 * *Files identical despite different names*

### Comparing `mate_cxinsys-1.0.4/mate/matelightning.py` & `mate_cxinsys-1.0.5/mate/matelightning.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,57 +6,57 @@
 import lightning as L
 import torch
 from torch.utils.data import Dataset, DataLoader
 
 from mate.transferentropy import TELightning
 from mate import MATE
 from mate.dataset import PairDataSet
+from mate.preprocess import DiscretizerFactory
 
 # try:
 #     from .mate.models.layer import LightningTE
 #     from .mate.dataset.dataset import PairDataSet
 # except (ImportError, ModuleNotFoundError) as err:
 #     from mate.models.layer import LightningTE
 #     from mate.dataset.dataset import PairDataSet
 
 class MATELightning(MATE):
     def __init__(self,
                  arr=None,
                  pairs=None,
                  kp=0.5,
                  num_kernels=1,
-                 method='pushing',
+                 method='default',
                  percentile=0,
                  smooth_func=None,
                  smooth_param=None,
                  len_time=None,
-                 dt=1):
+                 dt=1,
+                 surrogate=False,
+                 num_surrogate=1000,
+                 threshold=0.05,
+                 seed=1
+                 ):
         super().__init__()
 
-        self._pairs = pairs
-        self._arr = arr
-        self._bin_arr, self._n_bins = self.create_kde_array(kp=kp,
-                                                              num_kernels=num_kernels,
-                                                              method=method)
-        self._devices = None
-
-        self.model = TELightning(arr=self._bin_arr, len_time=len_time, dt=dt, n_bins=self._n_bins)
-        self.dset_pair = PairDataSet(arr=self._bin_arr, pairs=self._pairs)
+        np.random.seed(seed)
 
-    def kernel_width(self, arr, kp=None, percentile=None):
-        if percentile > 0:
-            arr.sort(axis=1)
-            i_beg = int(arr.shape[1] / 100 * percentile)
-            std = np.std(arr[:, i_beg:-i_beg], axis=1, ddof=1)
-        else:
-            std = np.std(arr, axis=1, ddof=1)
-        kw = kp * std
-        kw[kw == 0] = 1
+        dicretizer = DiscretizerFactory.create(method=method, kp=kp)
+        bin_arr, n_bins = dicretizer.binning(arr)
+        self._devices = None
 
-        return kw
+        self.model = TELightning(arr=bin_arr,
+                                 len_time=len_time,
+                                 dt=dt,
+                                 n_bins=n_bins,
+                                 surrogate=surrogate,
+                                 num_surrogate=num_surrogate,
+                                 threshold=threshold,
+                                 )
+        self.dset_pair = PairDataSet(arr=bin_arr, pairs=pairs)
 
     def custom_collate(self, batch):
         n_devices = None
 
         if type(self._devices)==int:
             n_devices = self._devices
         elif type(self._devices)==list:
```

### Comparing `mate_cxinsys-1.0.4/mate/transferentropy/telightning.py` & `mate_cxinsys-1.0.5/mate/transferentropy/telightning.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import time
 
 import numpy as np
 import torch
 from torch import nn
 import lightning.pytorch as pl
+from scipy.stats import norm
+from tqdm import tqdm
 
 
 def lexsort(keys, dim=-1):
     if keys.ndim < 2:
         raise ValueError(f"keys must be at least 2 dimensional, but {keys.ndim=}.")
     if len(keys) == 0:
         raise ValueError(f"Must have at least 1 key, but {len(keys)=}.")
@@ -15,109 +17,162 @@
     idx = keys[0].argsort(dim=dim, stable=True)
     for k in keys[1:]:
         idx = idx.index_select(dim, k.index_select(dim, idx).argsort(dim=dim, stable=True))
 
     return idx
 
 class TELightning(pl.LightningModule):
-    def __init__(self, arr=None, len_time=None, dt=1, n_bins=None):
+    def __init__(self,
+                 arr=None,
+                 len_time=None,
+                 dt=1,
+                 n_bins=None,
+                 surrogate=False,
+                 num_surrogate=1000,
+                 threshold=0.05,
+                 ):
         super().__init__()
         self._arr = arr
         self._len_time = len_time
         self._dt = dt
         self._n_bins = n_bins
 
         self._result_matrix = np.zeros((len(arr), len(arr)), dtype=np.float32)
 
         self._batch_predict_ef = []
         self._batch_predict_pairs = []
-    def forward(self, pairs):
-        arr = self._arr
-
-        arr = torch.tensor(arr, dtype=torch.float32, device=self.device)
-        pairs = torch.tensor(pairs, dtype=torch.int32, device=self.device)
 
-        if self._len_time is None:
-            self._len_time = arr.shape[1]
-
-        inds_pair = torch.arange(len(pairs)).to(self.device)
-
-        t_pairs = pairs[:, 0]
-        s_pairs = pairs[:, 1]
-
-        tile_inds_pair = torch.repeat_interleave(inds_pair, self._len_time-1)
-        tile_inds_pair = torch.tile(tile_inds_pair, (arr.shape[-1],))
+        self._surrogate = surrogate
+        self._num_surr = num_surrogate
+        self._threshold = threshold
+
+    def compute_te(self,
+                   arr=None,
+                   t_pairs=None,
+                   s_pairs=None,
+                   tile_inds_pair=None,
+                   ):
 
         target_arr = torch.index_select(arr, 0, t_pairs)
         source_arr = torch.index_select(arr, 0, s_pairs)
         vals = torch.stack((target_arr[:, self._dt:, :],
-                           target_arr[:, :-self._dt, :],
-                           source_arr[:, :-self._dt, :]),
+                            target_arr[:, :-self._dt, :],
+                            source_arr[:, :-self._dt, :]),
                            dim=3)
 
         t_vals = torch.permute(vals, dims=(2, 0, 1, 3))
 
         pair_vals = torch.concatenate((tile_inds_pair[:, None], torch.reshape(t_vals, (-1, 3))), dim=1)
 
-        n_bins = torch.tensor(self._n_bins, dtype=torch.int32, device=self.device)
-        n_bins = torch.index_select(n_bins, 0, t_pairs)
-        n_bins = torch.repeat_interleave(n_bins, (self._len_time - 1))
-        n_bins = torch.tile(n_bins, (arr.shape[-1],))
-
-        left_bools = torch.tensor(
-            torch.logical_and(
-                torch.greater_equal(pair_vals[:, 2], 0),
-                torch.less(pair_vals[:, 2], n_bins)
-            )
-        )
-        left_inds = torch.where(left_bools)[0]
-
-        pair_vals = torch.index_select(pair_vals, 0, left_inds)
+        # n_bins = torch.tensor(self._n_bins, dtype=torch.int32, device=self.device)
+        # n_bins = torch.index_select(n_bins, 0, t_pairs)
+        # n_bins = torch.repeat_interleave(n_bins, (self._len_time - 1))
+        # n_bins = torch.tile(n_bins, (arr.shape[-1],))
+        #
+        # left_bools = torch.tensor(
+        #     torch.logical_and(
+        #         torch.greater_equal(pair_vals[:, 2], 0),
+        #         torch.less(pair_vals[:, 2], n_bins)
+        #     )
+        # )
+        # left_inds = torch.where(left_bools)[0]
+        #
+        # pair_vals = torch.index_select(pair_vals, 0, left_inds)
 
         uvals_xt1_xt_yt, cnts_xt1_xt_yt = torch.unique(pair_vals, return_counts=True, dim=0)
         uvals_xt1_xt, cnts_xt1_xt = torch.unique(pair_vals[:, :-1], return_counts=True, dim=0)
-        uvals_xt_yt, cnts_xt_yt = torch.unique(torch.index_select(pair_vals, 1, torch.tensor([0, 2, 3], device=self.device)),
-                                                 return_counts=True, dim=0)
+        uvals_xt_yt, cnts_xt_yt = torch.unique(
+            torch.index_select(pair_vals, 1, torch.tensor([0, 2, 3], device=self.device)),
+            return_counts=True, dim=0)
         uvals_xt, cnts_xt = torch.unique(torch.index_select(pair_vals, 1, torch.tensor([0, 2], device=self.device)),
-                                               return_counts=True, dim=0)
+                                         return_counts=True, dim=0)
 
         subuvals_xt1_xt, n_subuvals_xt1_xt = torch.unique(uvals_xt1_xt_yt[:, :-1], return_counts=True, dim=0)
-        subuvals_xt_yt, n_subuvals_xt_yt = torch.unique(torch.index_select(uvals_xt1_xt_yt, 1, torch.tensor([0, 2, 3], device=self.device)),
-                                                          return_counts=True, dim=0)
-        subuvals_xt, n_subuvals_xt = torch.unique(torch.index_select(uvals_xt1_xt_yt, 1, torch.tensor([0, 2], device=self.device)),
-                                                    return_counts=True, dim=0)
+        subuvals_xt_yt, n_subuvals_xt_yt = torch.unique(
+            torch.index_select(uvals_xt1_xt_yt, 1, torch.tensor([0, 2, 3], device=self.device)),
+            return_counts=True, dim=0)
+        subuvals_xt, n_subuvals_xt = torch.unique(
+            torch.index_select(uvals_xt1_xt_yt, 1, torch.tensor([0, 2], device=self.device)),
+            return_counts=True, dim=0)
 
         cnts_xt1_xt = torch.repeat_interleave(cnts_xt1_xt, n_subuvals_xt1_xt)
 
         cnts_xt_yt = torch.repeat_interleave(cnts_xt_yt, n_subuvals_xt_yt)
         ind_xt_yt = lexsort(torch.index_select(uvals_xt1_xt_yt, 1, torch.tensor([3, 2, 0], device=self.device)).T)
         ind2ori_xt_yt = torch.argsort(ind_xt_yt)
         cnts_xt_yt = torch.take(cnts_xt_yt, ind2ori_xt_yt)
 
         cnts_xt = torch.repeat_interleave(cnts_xt, n_subuvals_xt)
         ind_xt = lexsort(torch.index_select(uvals_xt1_xt_yt, 1, torch.tensor([2, 0], device=self.device)).T)
         ind2ori_xt = torch.argsort(ind_xt)
         cnts_xt = torch.take(cnts_xt, ind2ori_xt)
 
         p_xt1_xt_yt = torch.divide(cnts_xt1_xt_yt, (self._len_time - 1) * arr.shape[-1])
-        # p_xt1_xt = torch.divide(cnts_xt1_xt, (self._len_time - 1))
-        # p_xt_yt = torch.divide(cnts_xt_yt, (self._len_time - 1))
-        # p_xt = torch.divide(cnts_xt, (self._len_time - 1))
 
         numer = torch.multiply(cnts_xt1_xt_yt, cnts_xt)
         denom = torch.multiply(cnts_xt1_xt, cnts_xt_yt)
         fraction = torch.divide(numer, denom)
         log_val = torch.log2(fraction)
         entropies = torch.multiply(p_xt1_xt_yt, log_val)
 
         uvals_tot, n_subuvals_tot = torch.unique(uvals_xt1_xt_yt[:, 0], return_counts=True)
         final_bins = torch.repeat_interleave(uvals_tot, n_subuvals_tot)
 
         entropy_final = torch.bincount(final_bins.to(torch.int32), weights=entropies)
 
+        return entropy_final
+
+    def forward(self, pairs):
+        arr = self._arr
+
+        arr = torch.tensor(arr, dtype=torch.float32, device=self.device)
+        pairs = torch.tensor(pairs, dtype=torch.int32, device=self.device)
+
+        if self._len_time is None:
+            self._len_time = arr.shape[1]
+
+        inds_pair = torch.arange(len(pairs)).to(self.device)
+
+        tile_inds_pair = torch.repeat_interleave(inds_pair, self._len_time - 1)
+        tile_inds_pair = torch.tile(tile_inds_pair, (arr.shape[-1],))
+
+        t_pairs = pairs[:, 0]
+        s_pairs = pairs[:, 1]
+
+        entropy_final = self.compute_te(arr=arr,
+                                        t_pairs=t_pairs,
+                                        s_pairs=s_pairs,
+                                        tile_inds_pair=tile_inds_pair
+                                        )
+
+        if self._surrogate is True:
+            surrogate_tes = []
+            for i in tqdm(range(self._num_surr)):
+                idx = np.random.rand(*arr.shape).argsort(axis=1)
+                arr = torch.take_along_dim(arr, torch.tensor(idx).to(self.device), dim=1)
+
+                entropy_surrogate = self.compute_te(arr=arr,
+                                                    t_pairs=t_pairs,
+                                                    s_pairs=s_pairs,
+                                                    tile_inds_pair=tile_inds_pair)
+
+                entropy_surrogate = entropy_surrogate.detach().cpu().numpy()
+
+                surrogate_tes.append(entropy_surrogate)
+
+            surrogate_tes = np.array(surrogate_tes)
+
+            # # 2안: surrogate의 각 TE로부터 분포 구성 -> 상위 k% 값 추출
+            means = np.mean(surrogate_tes, axis=0)
+            std = np.std(surrogate_tes, axis=0)
+            top_values = norm.ppf((1 - self._threshold), loc=means, scale=std)
+
+            # original te 값과 비교 -> original te < surrogate top te 이면 0
+            entropy_final[entropy_final <= torch.tensor(top_values).to(self.device)] = 0.0
+
         return entropy_final, pairs
 
     def predict_step(self, batch, batch_idx, dataloader_idx=0):
         pairs = batch
         # print(pairs.shape)
         # print(pairs)
         ef, pairs = self(pairs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mate_cxinsys-1.0.4/mate/transferentropy/transferentropy.py` & `mate_cxinsys-1.0.5/mate/transferentropy/transferentropy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import os.path as osp
 import time
 from multiprocessing import Process, shared_memory, Semaphore
 
 import numpy as np
+from tqdm import tqdm
+from scipy.stats import norm
 
 from mate.array import get_array_module
 
 class TransferEntropy(object):
     def __init__(self,
                  device=None,
                  batch_size=None,
@@ -16,15 +18,15 @@
                  inds_pair=None,
                  bin_arrs=None,
                  n_bins=None,
                  len_time=None,
                  shm_name=None,
                  result_matrix=None,
                  sem=None,
-                 dt=1
+                 dt=1,
                  ):
 
         self._am = get_array_module(device)
 
         self._batch_size = batch_size
         self._pairs = pairs
         self._n_pairs = n_pairs
@@ -45,34 +47,123 @@
 
         self._shm_name = shm_name
         self._result_matrix = result_matrix
         self._sem = sem
 
         self._dt = dt
 
-        # self.fpath_log = osp.join('./', 'elapsed_time_per_task.csv')
-        #
-        # if not osp.exists(self.fpath_log):
-        #     with open(self.fpath_log, 'w') as f:
-        #         f.write("Task, " \
-        #                 "Elapsed time \n")
-
     @property
     def am(self):
         return self._am
 
+    def compute_te(self,
+                   bin_arrs=None,
+                   t_pairs=None,
+                   s_pairs=None,
+                   tile_inds_pair=None,
+                   n_bins=None,
+                   dt=1,
+                   len_time=None):
+
+        target_arr = self.am.take(bin_arrs, t_pairs, axis=0)
+        source_arr = self.am.take(bin_arrs, s_pairs, axis=0)
+        vals = self.am.stack((target_arr[:, dt:, :],
+                              target_arr[:, :-dt, :],
+                              source_arr[:, :-dt, :]),
+                             axis=3)
+
+        t_vals = self.am.transpose(vals, axes=(2, 0, 1, 3))
+
+        pair_vals = self.am.concatenate((tile_inds_pair[:, None], self.am.reshape(t_vals, (-1, 3))), axis=1)
+
+        # # 허수 제거
+        # t_bins = self.am.take(n_bins, t_pairs, axis=0)
+        # t_bins = self.am.repeat(t_bins, (len_time - 1))
+        # t_bins = self.am.tile(t_bins, bin_arrs.shape[-1])
+        #
+        # left_bools = self.am.logical_and(
+        #     self.am.greater_equal(pair_vals[:, 2], 0),
+        #     self.am.less(pair_vals[:, 2], t_bins)
+        # )
+        #
+        # left_inds = self.am.where(left_bools)[0]
+        #
+        # pair_vals = self.am.take(pair_vals, left_inds, axis=0)
+        # # 허수 제거
+
+        uvals_xt1_xt_yt, cnts_xt1_xt_yt = self.am.unique(pair_vals, return_counts=True, axis=0)
+
+        uvals_xt1_xt, cnts_xt1_xt = self.am.unique(pair_vals[:, :-1], return_counts=True, axis=0)
+        uvals_xt_yt, cnts_xt_yt = self.am.unique(self.am.take(pair_vals, self.am.array([0, 2, 3]), axis=1),
+                                                 return_counts=True, axis=0)
+        uvals_xt, cnts_xt = self.am.unique(self.am.take(pair_vals, self.am.array([0, 2]), axis=1), return_counts=True,
+                                           axis=0)
+
+        subuvals_xt1_xt, n_subuvals_xt1_xt = self.am.unique(uvals_xt1_xt_yt[:, :-1], return_counts=True, axis=0)
+        subuvals_xt_yt, n_subuvals_xt_yt = self.am.unique(
+            self.am.take(uvals_xt1_xt_yt, self.am.array([0, 2, 3]), axis=1), return_counts=True, axis=0)
+        subuvals_xt, n_subuvals_xt = self.am.unique(self.am.take(uvals_xt1_xt_yt, self.am.array([0, 2]), axis=1),
+                                                    return_counts=True, axis=0)
+
+        cnts_xt1_xt = self.am.repeat(cnts_xt1_xt, n_subuvals_xt1_xt)
+
+        cnts_xt_yt = self.am.repeat(cnts_xt_yt, n_subuvals_xt_yt)
+
+        ind_xt_yt = self.am.lexsort(self.am.take(uvals_xt1_xt_yt, self.am.array([3, 2, 0]), axis=1).T)
+        ind2ori_xt_yt = self.am.argsort(ind_xt_yt)
+        cnts_xt_yt = self.am.take(cnts_xt_yt, ind2ori_xt_yt)
+
+        cnts_xt = self.am.repeat(cnts_xt, n_subuvals_xt)
+
+        ind_xt = self.am.lexsort(self.am.take(uvals_xt1_xt_yt, self.am.array([2, 0]), axis=1).T)
+        ind2ori_xt = self.am.argsort(ind_xt)
+        cnts_xt = self.am.take(cnts_xt, ind2ori_xt)
+
+        # TE
+        p_xt1_xt_yt = self.am.divide(cnts_xt1_xt_yt, (len_time - 1) * bin_arrs.shape[-1])
+        # p_xt1_xt_yt = self.am.divide(cnts_xt1_xt_yt, (len_time - 1))
+
+        numer = self.am.multiply(cnts_xt1_xt_yt, cnts_xt)
+        denom = self.am.multiply(cnts_xt1_xt, cnts_xt_yt)
+        fraction = self.am.divide(numer, denom)
+        log_val = self.am.log2(fraction)
+        entropies = self.am.multiply(p_xt1_xt_yt, log_val)
+
+        uvals_tot, n_subuvals_tot = self.am.unique(uvals_xt1_xt_yt[:, 0], return_counts=True)
+        final_bins = self.am.repeat(uvals_tot, n_subuvals_tot)
+        final_bins = self.am.astype(x=final_bins, dtype='int32')
+        entropy_final = self.am.bincount(final_bins, weights=entropies)
+
+        # # LocalTE
+        # numer = self.am.multiply(cnts_xt1_xt_yt, cnts_xt)
+        # denom = self.am.multiply(cnts_xt1_xt, cnts_xt_yt)
+        # fraction = self.am.divide(numer, denom)
+        # log_val = self.am.log2(fraction)
+        #
+        # uvals_tot, n_subuvals_tot = self.am.unique(uvals_xt1_xt_yt[:, 0], return_counts=True)
+        # final_bins = self.am.repeat(uvals_tot, n_subuvals_tot)
+        # final_bins = self.am.astype(x=final_bins, dtype='int32')
+        # entropies = self.am.bincount(final_bins, weights=log_val)
+        #
+        # entropy_final = self.am.divide(entropies, len_time - 1)
+
+        return entropy_final
+
     def solve(self,
               batch_size=None,
               pairs=None,
               bin_arrs=None,
               n_bins=None,
               shm_name=None,
               result_matrix=None,
               sem=None,
               dt=1,
+              surrogate=False,
+              num_surrogate=1000,
+              threshold=0.05,
               n_pairs=None,
               inds_pair=None,
               len_time=None,
               ):
 
         if not batch_size:
             if not self._batch_size:
@@ -129,14 +220,16 @@
             if not self._dt:
                 self._dt = dt = 1
             dt = self._dt
 
         bin_arrs = self.am.array(bin_arrs, dtype=bin_arrs.dtype)
         g_pairs = self.am.array(pairs, dtype=pairs.dtype)
 
+        n_bins = self.am.array(n_bins, dtype=n_bins.dtype)
+
         for i_iter, i_beg in enumerate(range(0, n_pairs, batch_size)):
             t_beg_batch = time.time()
 
             print("[%s ID: %d, Batch #%d]" % (str(self.am.device).upper(), self.am.device_id, i_iter + 1))
 
             stime_preproc = time.time()
 
@@ -145,152 +238,66 @@
 
             t_pairs = g_pairs[i_beg:i_end, 0]
             s_pairs = g_pairs[i_beg:i_end, 1]
 
             tile_inds_pair = self.am.repeat(inds_pair, (len_time - 1)) # (pairs, time * kernel)
             tile_inds_pair = self.am.tile(tile_inds_pair, bin_arrs.shape[-1])
 
-            target_arr = self.am.take(bin_arrs, t_pairs, axis=0)
-            source_arr = self.am.take(bin_arrs, s_pairs, axis=0)
-            vals = self.am.stack((target_arr[:, dt:, :],
-                                  target_arr[:, :-dt, :],
-                                  source_arr[:, :-dt, :]),
-                                  axis=3)
-
-
-            t_vals = self.am.transpose(vals, axes=(2, 0, 1, 3))
-
-            pair_vals = self.am.concatenate((tile_inds_pair[:, None], self.am.reshape(t_vals, (-1, 3))), axis=1)
-
-            # stime_imaginary = time.time()
-            # with open(self.fpath_log, 'a') as f:
-            #     f.write("Preprocess, " \
-            #             f"{stime_imaginary - stime_preproc} \n")
-
-            # 허수 제거
-            n_bins = self.am.array(n_bins, dtype=n_bins.dtype)
-            n_bins = self.am.take(n_bins, t_pairs, axis=0)
-            n_bins = self.am.repeat(n_bins, (len_time - 1))
-            n_bins = self.am.tile(n_bins, bin_arrs.shape[-1])
-
-            # left_bools = self.am.array(
-            #     self.am.logical_and(
-            #         self.am.greater_equal(pair_vals[:, 2], 0),
-            #         self.am.less(pair_vals[:, 2], n_bins)
-            #     )
-            # )
-            left_bools = self.am.logical_and(
-                self.am.greater_equal(pair_vals[:, 2], 0),
-                self.am.less(pair_vals[:, 2], n_bins)
-            )
-
-            left_inds = self.am.where(left_bools)[0]
-
-            pair_vals = self.am.take(pair_vals, left_inds, axis=0)
-            # 허수 제거
-
-            # stime_unique = time.time()
-            # with open(self.fpath_log, 'a') as f:
-            #     f.write("Remove imaginary, " \
-            #             f"{stime_unique - stime_imaginary} \n")
-
-            uvals_xt1_xt_yt, cnts_xt1_xt_yt = self.am.unique(pair_vals, return_counts=True, axis=0)
-
-            uvals_xt1_xt, cnts_xt1_xt = self.am.unique(pair_vals[:, :-1], return_counts=True, axis=0)
-            uvals_xt_yt, cnts_xt_yt = self.am.unique(self.am.take(pair_vals, self.am.array([0, 2, 3]), axis=1),
-                                                     return_counts=True, axis=0)
-            uvals_xt, cnts_xt = self.am.unique(self.am.take(pair_vals, self.am.array([0, 2]), axis=1), return_counts=True,
-                                               axis=0)
-
-            subuvals_xt1_xt, n_subuvals_xt1_xt = self.am.unique(uvals_xt1_xt_yt[:, :-1], return_counts=True, axis=0)
-            subuvals_xt_yt, n_subuvals_xt_yt = self.am.unique(self.am.take(uvals_xt1_xt_yt, self.am.array([0, 2, 3]), axis=1), return_counts=True, axis=0)
-            subuvals_xt, n_subuvals_xt = self.am.unique(self.am.take(uvals_xt1_xt_yt, self.am.array([0, 2]), axis=1), return_counts=True, axis=0)
-
-            # s_time = time.time()
-            # tmp_cnts_xt1_xt = self.am.concatenate([self.am.broadcast_to(cnt, self.am.take(n_subuvals_xt1_xt, i).item()) for i, cnt in enumerate(cnts_xt1_xt)])
-            # print(time.time() - s_time)
-
-            # stime_repeat1 = time.time()
-            # with open(self.fpath_log, 'a') as f:
-            #     f.write("Uniques, " \
-            #             f"{stime_repeat1 - stime_unique} \n")
-            cnts_xt1_xt = self.am.repeat(cnts_xt1_xt, n_subuvals_xt1_xt)
-
-            # stime_repeat2 = time.time()
-            # with open(self.fpath_log, 'a') as f:
-            #     f.write("Repeat1, " \
-            #             f"{stime_repeat2 - stime_repeat1} \n")
-            cnts_xt_yt = self.am.repeat(cnts_xt_yt, n_subuvals_xt_yt)
-
-            # stime_sort1 = time.time()
-            # with open(self.fpath_log, 'a') as f:
-            #     f.write("Repeat2, " \
-            #             f"{stime_sort1 - stime_repeat2} \n")
-            ind_xt_yt = self.am.lexsort(self.am.take(uvals_xt1_xt_yt, self.am.array([3, 2, 0]), axis=1).T)
-            ind2ori_xt_yt = self.am.argsort(ind_xt_yt)
-            cnts_xt_yt = self.am.take(cnts_xt_yt, ind2ori_xt_yt)
-
-            # stime_repeat3 = time.time()
-            # with open(self.fpath_log, 'a') as f:
-            #     f.write("Sort1, " \
-            #             f"{stime_repeat3 - stime_sort1} \n")
-            cnts_xt = self.am.repeat(cnts_xt, n_subuvals_xt)
-
-            # stime_sort2 = time.time()
-            # with open(self.fpath_log, 'a') as f:
-            #     f.write("Repeat3, " \
-            #             f"{stime_sort2 - stime_repeat3} \n")
-            ind_xt = self.am.lexsort(self.am.take(uvals_xt1_xt_yt, self.am.array([2, 0]), axis=1).T)
-            ind2ori_xt = self.am.argsort(ind_xt)
-            cnts_xt = self.am.take(cnts_xt, ind2ori_xt)
-
-            # stime_te = time.time()
-            # with open(self.fpath_log, 'a') as f:
-            #     f.write("Sort2, " \
-            #             f"{stime_te - stime_sort2} \n")
-            # TE
-            p_xt1_xt_yt = self.am.divide(cnts_xt1_xt_yt, (len_time - 1) * bin_arrs.shape[-1])
-            # p_xt1_xt_yt = self.am.divide(cnts_xt1_xt_yt, (len_time - 1))
-
-            numer = self.am.multiply(cnts_xt1_xt_yt, cnts_xt)
-            denom = self.am.multiply(cnts_xt1_xt, cnts_xt_yt)
-            fraction = self.am.divide(numer, denom)
-            log_val = self.am.log2(fraction)
-            entropies = self.am.multiply(p_xt1_xt_yt, log_val)
-
-            # stime_bincount = time.time()
-            # with open(self.fpath_log, 'a') as f:
-            #     f.write("TE, " \
-            #             f"{stime_bincount - stime_te} \n")
-            uvals_tot, n_subuvals_tot = self.am.unique(uvals_xt1_xt_yt[:, 0], return_counts=True)
-            final_bins = self.am.repeat(uvals_tot, n_subuvals_tot)
-            final_bins = self.am.astype(x=final_bins, dtype='int32')
-            entropy_final = self.am.bincount(final_bins, weights=entropies)
-
-            # etime = time.time()
-            # with open(self.fpath_log, 'a') as f:
-            #     f.write("Bincount, " \
-            #             f"{etime - stime_bincount} \n")
-
-            # # LocalTE
-            # numer = self.am.multiply(cnts_xt1_xt_yt, cnts_xt)
-            # denom = self.am.multiply(cnts_xt1_xt, cnts_xt_yt)
-            # fraction = self.am.divide(numer, denom)
-            # log_val = self.am.log2(fraction)
-            #
-            # uvals_tot, n_subuvals_tot = self.am.unique(uvals_xt1_xt_yt[:, 0], return_counts=True)
-            # final_bins = self.am.repeat(uvals_tot, n_subuvals_tot)
-            # final_bins = self.am.astype(x=final_bins, dtype='int32')
-            # entropies = self.am.bincount(final_bins, weights=log_val)
-            #
-            # entropy_final = self.am.divide(entropies, len_time - 1)
-
+            entropy_final = self.compute_te(bin_arrs=bin_arrs,
+                                            t_pairs=t_pairs,
+                                            s_pairs=s_pairs,
+                                            tile_inds_pair=tile_inds_pair,
+                                            n_bins=n_bins,
+                                            dt=dt,
+                                            len_time=len_time)
             # end TE
             entropy_final = self.am.asnumpy(entropy_final)
 
+            if surrogate is True:
+                surrogate_tes = []
+                for i in tqdm(range(num_surrogate)):
+                    idx = np.random.rand(*bin_arrs.shape).argsort(axis=1)
+                    # shuffle array along trajectory axis
+                    bin_arrs = self.am.take_along_axis(bin_arrs, self.am.array(idx), axis=1)
+
+                    entropy_surrogate = self.compute_te(bin_arrs=bin_arrs,
+                                                        t_pairs=t_pairs,
+                                                        s_pairs=s_pairs,
+                                                        tile_inds_pair=tile_inds_pair,
+                                                        n_bins=n_bins,
+                                                        dt=dt,
+                                                        len_time=len_time)
+
+                    entropy_surrogate = self.am.asnumpy(entropy_surrogate)
+
+                    surrogate_tes.append(entropy_surrogate)
+
+                print("[Making surrogate is done]")
+                surrogate_tes = np.array(surrogate_tes)
+
+                # 배열 크기가 GPU 메모리보다 클 경우 오류 발생 가능성 존재
+                # surrogate_tes = self.am.array(surrogate_tes)
+
+                # surrogate_tes.shape -> (batch, surrogates)
+                # 1안: 단순 5% 값 사용
+                # threshold_ind = int(np.ceil(len(surrogate_tes) * threshold))
+                # sorted_ind = surrogate_tes.argsort(axis=0)
+                # sorted_arr = np.take_along_axis(surrogate_tes, sorted_ind, axis=0)
+                # top_values = sorted_arr[-threshold_ind, :]
+
+                # # 2안: surrogate의 각 TE로부터 분포 구성 -> 상위 k% 값 추출
+                means = np.mean(surrogate_tes, axis=0)
+                std = np.std(surrogate_tes, axis=0)
+                top_values = norm.ppf((1 - threshold), loc=means, scale=std)
+
+                # original te 값과 비교 -> original te < surrogate top te 이면 0
+                entropy_final[entropy_final <= top_values] = 0.0
+                print("Number of entropies after eleminating FD")
+                print(f'[Before] {len(entropy_final)}, [Num. zero val] {len(entropy_final) - len(np.nonzero(entropy_final)[0])}')
+
             sem.acquire()
 
             new_shm = shared_memory.SharedMemory(name=shm_name)
             tmp_arr = np.ndarray(result_matrix.shape, dtype=result_matrix.dtype, buffer=new_shm.buf)
             tmp_arr[pairs[i_beg:i_end, 0], pairs[i_beg:i_end, 1]] = entropy_final
 
             new_shm.close()
```

### Comparing `mate_cxinsys-1.0.4/mate_cxinsys.egg-info/PKG-INFO` & `mate_cxinsys-1.0.5/mate_cxinsys.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mate-cxinsys
-Version: 1.0.4
+Version: 1.0.5
 Summary: MATE
 Home-page: https://github.com/cxinsys/mate
 Author: Complex Intelligent Systems Laboratory (CISLAB)
 Author-email: daewon4you@gmail.com
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mate_cxinsys-1.0.4/setup.py` & `mate_cxinsys-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='mate-cxinsys',
-      version='1.0.4',
+      version='1.0.5',
       description='MATE',
       url='https://github.com/cxinsys/mate',
       author='Complex Intelligent Systems Laboratory (CISLAB)',
       author_email='daewon4you@gmail.com',
       license='BSD-3-Clause',
       long_description=open('README.md').read(),
       long_description_content_type='text/markdown',
```

