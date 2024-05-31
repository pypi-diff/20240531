# Comparing `tmp/sccross-1.0.4.tar.gz` & `tmp/sccross-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sccross-1.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sccross-1.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sccross-1.0.4.tar` & `sccross-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1091 2023-10-28 18:30:45.294486 sccross-1.0.4/LICENSE
--rw-r--r--   0        0        0     2426 2023-11-30 11:28:02.743664 sccross-1.0.4/README.md
--rw-r--r--   0        0        0     1937 2024-05-14 07:00:30.528885 sccross-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      629 2023-10-28 18:30:45.455335 sccross-1.0.4/sccross/__init__.py
--rw-r--r--   0        0        0    17811 2023-10-28 18:30:45.456327 sccross-1.0.4/sccross/data.py
--rw-r--r--   0        0        0     8859 2023-10-28 18:30:45.457323 sccross-1.0.4/sccross/metrics.py
--rw-r--r--   0        0        0     3014 2023-10-28 18:30:45.457323 sccross-1.0.4/sccross/models/__init__.py
--rw-r--r--   0        0        0    11735 2023-10-28 18:30:45.458320 sccross-1.0.4/sccross/models/data.py
--rw-r--r--   0        0        0    17422 2024-04-08 20:25:48.188384 sccross-1.0.4/sccross/models/layers.py
--rw-r--r--   0        0        0    76422 2024-05-14 06:53:55.596888 sccross-1.0.4/sccross/models/sccross.py
--rw-r--r--   0        0        0    25980 2023-10-28 18:30:45.461102 sccross-1.0.4/sccross/models/utils.py
--rw-r--r--   0        0        0    29842 2023-10-28 18:30:45.462102 sccross-1.0.4/sccross/utils.py
--rw-r--r--   0        0        0     4503 1970-01-01 00:00:00.000000 sccross-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-10-28 18:30:45.294486 sccross-1.0.5/LICENSE
+-rw-r--r--   0        0        0     2426 2023-11-30 11:28:02.743664 sccross-1.0.5/README.md
+-rw-r--r--   0        0        0     1937 2024-05-31 04:17:00.852042 sccross-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      629 2023-10-28 18:30:45.455335 sccross-1.0.5/sccross/__init__.py
+-rw-r--r--   0        0        0    17811 2023-10-28 18:30:45.456327 sccross-1.0.5/sccross/data.py
+-rw-r--r--   0        0        0     8859 2023-10-28 18:30:45.457323 sccross-1.0.5/sccross/metrics.py
+-rw-r--r--   0        0        0     3014 2023-10-28 18:30:45.457323 sccross-1.0.5/sccross/models/__init__.py
+-rw-r--r--   0        0        0    11735 2023-10-28 18:30:45.458320 sccross-1.0.5/sccross/models/data.py
+-rw-r--r--   0        0        0    15533 2024-05-31 03:57:23.061392 sccross-1.0.5/sccross/models/layers.py
+-rw-r--r--   0        0        0    76422 2024-05-14 06:53:55.596888 sccross-1.0.5/sccross/models/sccross.py
+-rw-r--r--   0        0        0    25980 2023-10-28 18:30:45.461102 sccross-1.0.5/sccross/models/utils.py
+-rw-r--r--   0        0        0    29842 2023-10-28 18:30:45.462102 sccross-1.0.5/sccross/utils.py
+-rw-r--r--   0        0        0     4503 1970-01-01 00:00:00.000000 sccross-1.0.5/PKG-INFO
```

### Comparing `sccross-1.0.4/LICENSE` & `sccross-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sccross-1.0.4/README.md` & `sccross-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sccross-1.0.4/pyproject.toml` & `sccross-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel", "flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "sccross"
-version = "1.0.4"
+version = "1.0.5"
 description = "Single cell multi-omics cross modal generation, multi-omics simulation and perturbation"
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE"}
 
 keywords = ["bioinformatics", "deep-learning", "single-cell", "single-cell-multiomics"]
 classifiers = [
```

### Comparing `sccross-1.0.4/sccross/__init__.py` & `sccross-1.0.5/sccross/__init__.py`

 * *Files identical despite different names*

### Comparing `sccross-1.0.4/sccross/data.py` & `sccross-1.0.5/sccross/data.py`

 * *Files identical despite different names*

### Comparing `sccross-1.0.4/sccross/metrics.py` & `sccross-1.0.5/sccross/metrics.py`

 * *Files identical despite different names*

### Comparing `sccross-1.0.4/sccross/models/__init__.py` & `sccross-1.0.5/sccross/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sccross-1.0.4/sccross/models/data.py` & `sccross-1.0.5/sccross/models/data.py`

 * *Files identical despite different names*

### Comparing `sccross-1.0.4/sccross/models/layers.py` & `sccross-1.0.5/sccross/models/layers.py`

 * *Files 4% similar despite different names*

```diff
@@ -585,80 +585,8 @@
         self.register_buffer("std", std)
 
     def forward(self) -> D.Normal:
         return D.Normal(self.loc, self.std)
 
 
 
-class IndDataDecoder(DataDecoder):
 
-    r"""
-    Data decoder mixin that makes decoding independent of feature latent
-
-    Parameters
-    ----------
-    in_features
-        Input dimensionality
-    out_features
-        Output dimensionality
-    n_batches
-        Number of batches
-    """
-
-    def __init__(  # pylint: disable=unused-argument
-            self, in_features: int, out_features: int, n_batches: int = 1
-    ) -> None:
-        super().__init__(out_features, n_batches=n_batches)
-        self.v = torch.nn.Parameter(torch.zeros(out_features, in_features))
-
-    def forward(  # pylint: disable=arguments-differ
-            self, u: torch.Tensor, b: torch.Tensor,
-            l: Optional[torch.Tensor]
-    ) -> D.Distribution:
-        r"""
-        Decode data from sample latent
-
-        Parameters
-        ----------
-        u
-            Sample latent
-        b
-            Batch index
-        l
-            Optional normalizer
-
-        Returns
-        -------
-        recon
-            Data reconstruction distribution
-        """
-        return super().forward(u, self.v, b, l)
-
-
-class IndNormalDataDocoder(IndDataDecoder, NormalDataDecoder):
-    r"""
-    Normal data decoder independent of feature latent
-    """
-
-
-class IndZINDataDecoder(IndDataDecoder, ZINDataDecoder):
-    r"""
-    Zero-inflated normal data decoder independent of feature latent
-    """
-
-
-class IndZILNDataDecoder(IndDataDecoder, ZILNDataDecoder):
-    r"""
-    Zero-inflated log-normal data decoder independent of feature latent
-    """
-
-
-class IndNBDataDecoder(IndDataDecoder, NBDataDecoder):
-    r"""
-    Negative binomial data decoder independent of feature latent
-    """
-
-
-class IndZINBDataDecoder(IndDataDecoder, ZINBDataDecoder):
-    r"""
-    Zero-inflated negative binomial data decoder independent of feature latent
-    """
```

### Comparing `sccross-1.0.4/sccross/models/sccross.py` & `sccross-1.0.5/sccross/models/sccross.py`

 * *Files identical despite different names*

### Comparing `sccross-1.0.4/sccross/models/utils.py` & `sccross-1.0.5/sccross/models/utils.py`

 * *Files identical despite different names*

### Comparing `sccross-1.0.4/sccross/utils.py` & `sccross-1.0.5/sccross/utils.py`

 * *Files identical despite different names*

### Comparing `sccross-1.0.4/PKG-INFO` & `sccross-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sccross
-Version: 1.0.4
+Version: 1.0.5
 Summary: Single cell multi-omics cross modal generation, multi-omics simulation and perturbation
 Keywords: bioinformatics,deep-learning,single-cell,single-cell-multiomics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

