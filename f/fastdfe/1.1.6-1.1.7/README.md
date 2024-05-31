# Comparing `tmp/fastdfe-1.1.6.tar.gz` & `tmp/fastdfe-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastdfe-1.1.6.tar", max compression
+gzip compressed data, was "fastdfe-1.1.7.tar", max compression
```

## Comparing `fastdfe-1.1.6.tar` & `fastdfe-1.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1087 2024-04-20 09:19:01.722933 fastdfe-1.1.6/LICENSE
--rw-r--r--   0        0        0     1154 2024-04-20 09:19:01.722933 fastdfe-1.1.6/README.md
--rw-r--r--   0        0        0     6050 2024-04-20 09:19:01.742933 fastdfe-1.1.6/fastdfe/__init__.py
--rw-r--r--   0        0        0    22930 2024-04-20 09:19:01.742933 fastdfe-1.1.6/fastdfe/abstract_inference.py
--rw-r--r--   0        0        0   159257 2024-04-20 09:19:01.742933 fastdfe-1.1.6/fastdfe/annotation.py
--rw-r--r--   0        0        0    55241 2024-04-20 09:19:01.742933 fastdfe-1.1.6/fastdfe/base_inference.py
--rw-r--r--   0        0        0     4953 2024-04-20 09:19:01.742933 fastdfe-1.1.6/fastdfe/bootstrap.py
--rw-r--r--   0        0        0    11527 2024-04-20 09:19:01.742933 fastdfe-1.1.6/fastdfe/config.py
--rw-r--r--   0        0        0    16167 2024-04-20 09:19:01.742933 fastdfe-1.1.6/fastdfe/discretization.py
--rw-r--r--   0        0        0    21750 2024-04-20 09:19:01.742933 fastdfe-1.1.6/fastdfe/filtration.py
--rw-r--r--   0        0        0    23736 2024-04-20 09:19:01.746933 fastdfe-1.1.6/fastdfe/io_handlers.py
--rw-r--r--   0        0        0    52126 2024-04-20 09:19:01.746933 fastdfe-1.1.6/fastdfe/joint_inference.py
--rw-r--r--   0        0        0     3912 2024-04-20 09:19:01.746933 fastdfe-1.1.6/fastdfe/json_handlers.py
--rw-r--r--   0        0        0     2556 2024-04-20 09:19:01.746933 fastdfe-1.1.6/fastdfe/likelihood.py
--rw-r--r--   0        0        0    41556 2024-04-20 09:19:01.746933 fastdfe-1.1.6/fastdfe/optimization.py
--rw-r--r--   0        0        0    30449 2024-04-20 09:19:01.746933 fastdfe-1.1.6/fastdfe/parametrization.py
--rw-r--r--   0        0        0    46334 2024-04-20 09:19:01.746933 fastdfe-1.1.6/fastdfe/parser.py
--rw-r--r--   0        0        0    13173 2024-04-20 09:19:01.746933 fastdfe-1.1.6/fastdfe/polydfe.py
--rw-r--r--   0        0        0     5274 2024-04-20 09:19:01.746933 fastdfe-1.1.6/fastdfe/polydfe_utils.py
--rw-r--r--   0        0        0      276 2024-04-20 09:19:01.746933 fastdfe-1.1.6/fastdfe/settings.py
--rw-r--r--   0        0        0    30571 2024-04-20 09:19:01.746933 fastdfe-1.1.6/fastdfe/spectrum.py
--rw-r--r--   0        0        0    32440 2024-04-20 09:19:01.746933 fastdfe-1.1.6/fastdfe/visualization.py
--rw-r--r--   0        0        0     1016 2024-04-20 09:19:01.746933 fastdfe-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     2326 1970-01-01 00:00:00.000000 fastdfe-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-31 11:30:15.802239 fastdfe-1.1.7/LICENSE
+-rw-r--r--   0        0        0     1355 2024-05-31 11:30:15.802239 fastdfe-1.1.7/README.md
+-rw-r--r--   0        0        0     5887 2024-05-31 11:30:15.822239 fastdfe-1.1.7/fastdfe/__init__.py
+-rw-r--r--   0        0        0    22854 2024-05-31 11:30:15.822239 fastdfe-1.1.7/fastdfe/abstract_inference.py
+-rw-r--r--   0        0        0   164627 2024-05-31 11:30:15.822239 fastdfe-1.1.7/fastdfe/annotation.py
+-rw-r--r--   0        0        0    55351 2024-05-31 11:30:15.822239 fastdfe-1.1.7/fastdfe/base_inference.py
+-rw-r--r--   0        0        0     4927 2024-05-31 11:30:15.822239 fastdfe-1.1.7/fastdfe/bootstrap.py
+-rw-r--r--   0        0        0    11557 2024-05-31 11:30:15.822239 fastdfe-1.1.7/fastdfe/config.py
+-rw-r--r--   0        0        0    16185 2024-05-31 11:30:15.822239 fastdfe-1.1.7/fastdfe/discretization.py
+-rw-r--r--   0        0        0    21750 2024-05-31 11:30:15.822239 fastdfe-1.1.7/fastdfe/filtration.py
+-rw-r--r--   0        0        0    23850 2024-05-31 11:30:15.822239 fastdfe-1.1.7/fastdfe/io_handlers.py
+-rw-r--r--   0        0        0    52136 2024-05-31 11:30:15.822239 fastdfe-1.1.7/fastdfe/joint_inference.py
+-rw-r--r--   0        0        0     3912 2024-05-31 11:30:15.822239 fastdfe-1.1.7/fastdfe/json_handlers.py
+-rw-r--r--   0        0        0     2556 2024-05-31 11:30:15.822239 fastdfe-1.1.7/fastdfe/likelihood.py
+-rw-r--r--   0        0        0    41557 2024-05-31 11:30:15.822239 fastdfe-1.1.7/fastdfe/optimization.py
+-rw-r--r--   0        0        0    30541 2024-05-31 11:30:15.822239 fastdfe-1.1.7/fastdfe/parametrization.py
+-rw-r--r--   0        0        0    45947 2024-05-31 11:30:15.822239 fastdfe-1.1.7/fastdfe/parser.py
+-rw-r--r--   0        0        0    13173 2024-05-31 11:30:15.822239 fastdfe-1.1.7/fastdfe/polydfe.py
+-rw-r--r--   0        0        0     5274 2024-05-31 11:30:15.822239 fastdfe-1.1.7/fastdfe/polydfe_utils.py
+-rw-r--r--   0        0        0      276 2024-05-31 11:30:15.822239 fastdfe-1.1.7/fastdfe/settings.py
+-rw-r--r--   0        0        0    30525 2024-05-31 11:30:15.822239 fastdfe-1.1.7/fastdfe/spectrum.py
+-rw-r--r--   0        0        0    32261 2024-05-31 11:30:15.826239 fastdfe-1.1.7/fastdfe/visualization.py
+-rw-r--r--   0        0        0     1016 2024-05-31 11:30:15.826239 fastdfe-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2527 1970-01-01 00:00:00.000000 fastdfe-1.1.7/PKG-INFO
```

### Comparing `fastdfe-1.1.6/README.md` & `fastdfe-1.1.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # fastDFE  <img align="right" width="100" src="https://raw.githubusercontent.com/Sendrowski/fastDFE/master/docs/logo.png">
 [![tests](https://github.com/Sendrowski/fastDFE/actions/workflows/run-tests.yml/badge.svg?branch=master)](https://github.com/Sendrowski/fastDFE/actions/workflows/run-tests.yml)
 [![codecov](https://codecov.io/gh/Sendrowski/fastDFE/branch/master/graph/badge.svg?token=0LUE8SZYBJ)](https://codecov.io/gh/Sendrowski/fastDFE)
 [![Documentation Status](https://readthedocs.org/projects/fastdfe/badge/?version=latest)](https://fastdfe.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/fastdfe.svg)](https://badge.fury.io/py/fastdfe)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![Downloads](https://static.pepy.tech/badge/fastdfe)](https://pepy.tech/project/fastdfe)
 [![DOI](https://img.shields.io/badge/DOI-10.1093/molbev/msae070-blue)](https://doi.org/10.1093/molbev/msae070)
 
-
 ``fastdfe`` is a package for fast, flexible, and hierarchical inference of the distribution of fitness effects (DFE) from site frequency spectra (SFS). It also contains a versatile VCF-to-SFS parser with support for ancestral allele and site-degeneracy annotation.
 
 Please see the [documentation](https://fastdfe.readthedocs.io/en/latest/) for all the details.
```

### Comparing `fastdfe-1.1.6/fastdfe/__init__.py` & `fastdfe-1.1.7/fastdfe/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 fastDFE package.
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-03-10"
 
-__version__ = '1.1.6'
+__version__ = '1.1.7'
 
 import logging
 import sys
-import warnings
 
 import jsonpickle
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
 
 from .json_handlers import DataframeHandler, SpectrumHandler, SpectraHandler, NumpyArrayHandler
@@ -107,28 +106,22 @@
 
 # define a Formatter with colors
 formatter = ColoredFormatter('%(levelname)s:%(name)s: %(message)s')
 
 handler.setFormatter(formatter)
 logger.addHandler(handler)
 
-
-def raise_on_warning(message, category, filename, lineno, file=None, line=None):
-    """
-    Raise exception on warning.
-    """
-    raise Exception(warnings.formatwarning(message, category, filename, lineno, line))
-
+# def raise_on_warning(message, category, filename, lineno, file=None, line=None):
+#    """
+#    Raise exception on warning.
+#    """
+#    raise Exception(warnings.formatwarning(message, category, filename, lineno, line))
 
 # warnings.showwarning = raise_on_warning
 
-# configure default colormap
-# plt.rcParams['image.cmap'] = 'Dark2'
-# plt.rcParams['axes.prop_cycle'] = cycler('color', plt.get_cmap('Dark2').colors)
-
 # load class from modules
 from .parametrization import Parametrization, GammaExpParametrization, DiscreteParametrization, \
     GammaDiscreteParametrization, DisplacedGammaParametrization, DiscreteFractionalParametrization
 from .config import Config
 from .settings import Settings
 from .abstract_inference import Inference
 from .base_inference import BaseInference, InferenceResults
```

### Comparing `fastdfe-1.1.6/fastdfe/abstract_inference.py` & `fastdfe-1.1.7/fastdfe/abstract_inference.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-03-12"
 
 import logging
 from abc import ABC, abstractmethod
-from typing import List, Optional, Literal, Tuple, Dict
+from typing import List, Optional, Literal, Tuple, Dict, Sequence
 
 import jsonpickle
 import numpy as np
 import pandas as pd
 from typing_extensions import Self
 
 from .bootstrap import Bootstrap
@@ -25,22 +25,22 @@
     """
     Static utility methods for inference objects.
     """
 
     @staticmethod
     def plot_discretized(
             inferences: List['AbstractInference'],
-            intervals: list | np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
+            intervals: Sequence = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             file: str = None,
             show: bool = True,
             title: str = 'discretized DFEs',
-            labels: list | np.ndarray = None,
+            labels: Sequence = None,
             ax: 'plt.Axes' = None,
             kwargs_legend: dict = dict(prop=dict(size=8)),
             **kwargs
 
     ) -> 'plt.Axes':
         """
         Visualize several discretized DFEs given by the list of inference objects.
@@ -94,15 +94,15 @@
             intervals: np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             file: str = None,
             show: bool = True,
             title: str = 'continuous DFEs',
-            labels: list | np.ndarray = None,
+            labels: Sequence = None,
             scale: Literal['lin', 'log', 'symlog'] = 'lin',
             scale_density: bool = False,
             ax: 'plt.Axes' = None,
             kwargs_legend: dict = dict(prop=dict(size=8)),
             **kwargs
 
     ) -> 'plt.Axes':
@@ -152,15 +152,15 @@
             bins=intervals,
             **locals()
         )
 
     @staticmethod
     def plot_inferred_parameters(
             inferences: List['AbstractInference'],
-            labels: list | np.ndarray,
+            labels: Sequence,
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             file: str = None,
             show: bool = True,
             title: str = 'parameter estimates',
             scale: Literal['lin', 'log', 'symlog'] = 'log',
@@ -219,15 +219,15 @@
             kwargs_legend=kwargs_legend,
             ax=ax,
         )
 
     @staticmethod
     def plot_inferred_parameters_boxplot(
             inferences: List['AbstractInference'],
-            labels: list | np.ndarray,
+            labels: Sequence,
             file: str = None,
             show: bool = True,
             title: str = 'parameter estimates',
             **kwargs
     ) -> 'plt.Axes':
         """
         Visualize several discretized DFEs given by the list of inference objects.
@@ -265,16 +265,16 @@
         )
 
     @staticmethod
     def get_cis_params_mle(
             bootstrap_type: Literal['percentile', 'bca'],
             ci_level: float,
             inferences: List['AbstractInference'],
-            labels: list | np.ndarray,
-            param_names: list | np.ndarray
+            labels: Sequence,
+            param_names: Sequence
     ) -> dict[str, Optional[Dict[str, Tuple[float, float]]]]:
         """
         Get confidence intervals for the MLE parameters.
 
         :param bootstrap_type: Type of bootstrap to use for confidence intervals.
         :param ci_level: Confidence level for confidence intervals.
         :param inferences: List of inference objects.
@@ -304,16 +304,16 @@
 
     @staticmethod
     def get_errors_params_mle(
             bootstrap_type: Literal['percentile', 'bca'],
             ci_level: float,
             confidence_intervals: bool,
             inferences: List['AbstractInference'],
-            labels: list | np.ndarray,
-            param_names: list | np.ndarray
+            labels: Sequence,
+            param_names: Sequence
     ) -> (Dict[str, Tuple[np.ndarray, np.ndarray] | None], Dict[str, np.ndarray]):
         """
         Get errors and values for MLE params of inferences.
 
         :param bootstrap_type: Type of bootstrap to use.
         :param ci_level: Confidence level for confidence intervals.
         :param confidence_intervals: Whether to compute confidence intervals.
@@ -346,15 +346,15 @@
                 errors[label] = None
 
         return errors, values
 
     @staticmethod
     def get_discretized(
             inferences: List['AbstractInference'],
-            labels: list | np.ndarray,
+            labels: Sequence,
             intervals: np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile'
 
     ) -> (np.ndarray, Optional[np.ndarray]):
         """
@@ -500,15 +500,15 @@
         """
         Get discretized DFE.
 
         :param bootstrap_type: Type of bootstrap
         :param ci_level: Confidence interval level
         :param confidence_intervals: Whether to return confidence intervals
         :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bins.
-        :return: Array of values and array of errors
+        :return: Array of values and array of deviations
         """
         values, errors = Inference.get_discretized(
             inferences=[self],
             labels=['all'],
             intervals=intervals,
             confidence_intervals=confidence_intervals,
             ci_level=ci_level,
```

### Comparing `fastdfe-1.1.6/fastdfe/annotation.py` & `fastdfe-1.1.7/fastdfe/annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 import itertools
 import logging
 import re
 import subprocess
 import tempfile
 from abc import ABC, abstractmethod
 from collections import Counter, defaultdict
-from dataclasses import dataclass, field
 from enum import Enum
 from functools import cached_property
 from io import StringIO
 from itertools import product
 from typing import List, Optional, Dict, Tuple, Callable, Literal, Iterable, cast, Any, Generator
 
 import Bio.Data.CodonTable
+import jsonpickle
 import numpy as np
 import pandas as pd
 from Bio import Phylo
 from Bio.Phylo.BaseTree import Clade, Tree
 from Bio.Seq import Seq
 from Bio.SeqRecord import SeqRecord
 from cyvcf2 import Variant, Writer, VCF
@@ -187,15 +187,15 @@
         #: The current contig.
         self._contig: Optional[SeqRecord] = None
 
         #: The variants that could not be annotated correctly.
         self.mismatches: List[Variant] = []
 
         #: The variant that were skipped because they were not in coding regions.
-        self.n_skipped = 0
+        self.n_skipped: int = 0
 
         #: The variants for which the codon could not be determined.
         self.errors: List[Variant] = []
 
     def _setup(self, handler: MultiHandler):
         """
         Provide context to the annotator.
@@ -906,15 +906,15 @@
 
 class SubstitutionModel(ABC):
     """
     Base class for substitution models.
     """
 
     #: The possible transitions
-    _transitions: np.ndarray[int, (..., ...)] = np.array([
+    _transitions: np.ndarray = np.array([
         (base_indices['A'], base_indices['G']),
         (base_indices['G'], base_indices['A']),
         (base_indices['C'], base_indices['T']),
         (base_indices['T'], base_indices['C'])
     ])
 
     def __init__(
@@ -1177,87 +1177,114 @@
         if (b1, b2) in [(0, 2), (2, 0), (1, 3), (3, 1)]:
             return K * np.exp(-K) * (k / (k + 2) + K * 1 / (k ** 2 + 4 * k + 4))
 
         # if we have a transversion
         return K * np.exp(-K) * (1 / (k + 2) + K * k / (k ** 2 + 4 * k + 4))
 
 
-@dataclass
 class SiteConfig:
     """
     Ancestral allele site configuration for a single subsample.
     """
 
-    #: The number of major alleles.
-    n_major: int
+    def __init__(
+            self,
+            n_major: int,
+            major_base: int,
+            minor_base: int,
+            outgroup_bases: np.ndarray,
+            multiplicity: float = 1.0,
+            sites: np.ndarray = None,
+            p_minor: float = np.nan,
+            p_major: float = np.nan
+    ):
+        """
+        Create a new site configuration instance.
+        """
+        #: The number of major alleles.
+        self.n_major: int = n_major
 
-    #: The major allele base index.
-    major_base: int
+        #: The major allele base index.
+        self.major_base: int = major_base
 
-    #: The minor base index.
-    minor_base: int
+        #: The minor base index.
+        self.minor_base: int = minor_base
 
-    #: The outgroup base indices.
-    outgroup_bases: np.ndarray[int]
+        #: The outgroup base indices.
+        self.outgroup_bases: np.ndarray = outgroup_bases
 
-    #: The multiplicity of the site.
-    multiplicity: float = 1.0
+        #: The multiplicity of the site.
+        self.multiplicity: float = multiplicity
 
-    #: The site indices.
-    sites: np.ndarray[int] = field(default_factory=lambda: np.array([]))
+        #: The site indices.
+        self.sites: np.ndarray = np.array([]) if sites is None else sites
 
-    # The probability of the minor allele.
-    p_minor: np.float64 = np.nan
+        #: The probability of the minor allele.
+        self.p_minor: float = p_minor
 
-    # The probability of the major allele.
-    p_major: np.float64 = np.nan
+        #: The probability of the major allele.
+        self.p_major: float = p_major
 
 
-@dataclass
 class SiteInfo:
     """
     Ancestral allele information on a single site.
     """
 
-    #: Dictionary mapping number of major alleles to its probability of observation.
-    n_major: Dict[int, float]
+    def __init__(
+            self,
+            n_major: Dict[int, float],
+            major_base: str,
+            minor_base: str,
+            outgroup_bases: List[str],
+            p_minor: float = np.nan,
+            p_major: float = np.nan,
+            p_major_ancestral: float = np.nan,
+            major_ancestral: str = '.',
+            p_bases_first_node: Dict[str, float] = None,
+            p_first_node_ancestral: float = np.nan,
+            first_node_ancestral: str = '.',
+            rate_params: Dict[str, float] = None
+    ):
+        #: Dictionary mapping number of major alleles to its probability of observation.
+        self.n_major: Dict[int, float] = n_major
 
-    #: The major allele base.
-    major_base: str
+        #: The major allele base.
+        self.major_base: str = major_base
 
-    #: The minor base index.
-    minor_base: str
+        #: The minor base index.
+        self.minor_base: str = minor_base
 
-    #: The outgroup base indices.
-    outgroup_bases: List[str]
+        #: The outgroup base indices.
+        self.outgroup_bases: List[str] = outgroup_bases
 
-    #: The probability of the minor allele being the ancestral allele (without prior).
-    p_minor: float = np.nan
+        #: The probability of the minor allele being the ancestral allele (without prior).
+        self.p_minor: float = p_minor
 
-    #: The probability of the major allele being the ancestral allele (without prior).
-    p_major: float = np.nan
+        #: The probability of the major allele being the ancestral allele (without prior).
+        self.p_major: float = p_major
 
-    #: The probability of the major allele being the ancestral allele rather than the minor allele
-    #: (possibly with prior if specified).
-    p_major_ancestral: float = np.nan
+        #: The probability of the major allele being the ancestral allele rather than the minor allele
+        #: (possibly with prior if specified).
+        self.p_major_ancestral: float = p_major_ancestral
 
-    #: The ancestral base based on comparing major and minor allele.
-    major_ancestral: str = '.'
+        #: The ancestral base based on comparing major and minor allele.
+        self.major_ancestral: str = major_ancestral
 
-    #: The probability of each base being the ancestral base for the first internal node.
-    p_bases_first_node: Dict[str, float] = field(default_factory=dict)
+        #: The probability of each base being the ancestral base for the first internal node.
+        self.p_bases_first_node: Dict[str, float] = {} if p_bases_first_node is None else p_bases_first_node
 
-    #: The probability that the mostly likely base for the first internal node is the ancestral base.
-    p_first_node_ancestral: float = np.nan
+        #: The probability that the mostly likely base for the first internal node is the ancestral base.
+        self.p_first_node_ancestral: float = p_first_node_ancestral
 
-    #: The ancestral base index for the first internal node.
-    first_node_ancestral: str = '.'
+        #: The ancestral base index for the first internal node.
+        self.first_node_ancestral: str = first_node_ancestral
 
-    #: The branch rates.
-    rate_params: Dict[str, float] = field(default_factory=dict)
+        #: The branch rates.
+        self.rate_params: Dict[str, float] = {} if rate_params is None else rate_params
 
     def plot_tree(
             self,
             ax: 'plt.Axes' = None,
             show: bool = True,
     ):
         """
@@ -1332,20 +1359,34 @@
         for pos in ['top', 'right', 'left']:
             ax.spines[pos].set_visible(False)
 
         if show:
             plt.show()
 
 
+class _TooFewIngroupsSiteError(ValueError):
+    """
+    Raised when there are too few ingroups to consider a site for ancestral allele annotation.
+    """
+    pass
+
+
+class _PolyAllelicSiteError(ValueError):
+    """
+    Raised when a site has more than two alleles.
+    """
+    pass
+
+
 class BaseType(Enum):
     """
     The base type, either major or minor.
     """
-    MINOR = 0
-    MAJOR = 1
+    MINOR: int = 0
+    MAJOR: int = 1
 
 
 class PolarizationPrior(ABC):
     """
     Base class for priors to be used with the :class:`MaximumLikelihoodAncestralAnnotation`.
     Using a prior, we incorporate information about the general probability of the major allele being the ancestral 
     allele across all sites with the same minor allele count, is useful in general as it provides more information 
@@ -1371,15 +1412,15 @@
         #: The logger.
         self._logger = logger.getChild(self.__class__.__name__)
 
         #: Whether to allow divergence.
         self.allow_divergence: bool = allow_divergence
 
         #: The polarization probabilities.
-        self.probabilities: np.ndarray[float, (...,)] | None = None
+        self.probabilities: np.ndarray | None = None
 
     def _add_divergence(self):
         """
         Add divergence to the polarization probabilities.
         """
         # take divergence probabilities to be the same as alleles of frequency 1
         if self.allow_divergence:
@@ -1503,15 +1544,15 @@
         #: The random number generator.
         self.rng: np.random.Generator = np.random.default_rng(seed=self.seed)
 
     def _get_prior(
             self,
             configs: pd.DataFrame,
             n_ingroups: int
-    ) -> np.ndarray[float, (...,)]:
+    ) -> np.ndarray:
         """
         Get the polarization probabilities.
 
         :param configs: The site configurations.
         :param n_ingroups: The number of ingroups.
         :return: The polarization probabilities.
         """
@@ -1548,15 +1589,15 @@
         # get initial values
         initial_values = np.array([self.rng.uniform() for _ in range(data.shape[0])])
 
         # add initial values
         data = np.hstack((data, initial_values.reshape((-1, 1))))
 
         # run the optimization in parallel for each frequency bin over n_runs
-        results: np.ndarray[OptimizeResult] = parallelize_func(
+        results: np.ndarray = parallelize_func(
             func=optimize_polarization,
             data=data,
             parallelize=self.parallelize,
             pbar=True,
             desc=f"{self.__class__.__name__}>Optimizing polarization priors",
             dtype=object
         ).reshape(len(freq_indices), self.n_runs)
@@ -1642,42 +1683,46 @@
         return compute_likelihood
 
 
 class _OutgroupAncestralAlleleAnnotation(AncestralAlleleAnnotation, ABC):
     """
     Abstract class for annotation of ancestral alleles using outgroup information.
     """
-    #: Subsample mode.
-    subsample_mode: Literal['random', 'probabilistic'] = 'random'
 
     def __init__(
             self,
             outgroups: List[str],
             n_ingroups: int,
             ingroups: List[str] | None = None,
             exclude: List[str] = [],
             seed: int | None = 0,
+            subsample_mode: Literal['random', 'probabilistic'] = 'random'
     ):
         """
         Create a new ancestral allele annotation instance.
 
         :param outgroups: The outgroup samples to consider when determining the ancestral allele. A list of
             sample names as they appear in the VCF file.
         :param n_ingroups:  The minimum number of ingroups that must be present at a site for it to be considered
             for ancestral allele inference.
         :param ingroups: The ingroup samples to consider when determining the ancestral allele. A list of
             sample names as they appear in the VCF file. If ``None``, all samples except the outgroups are
             considered.
         :param exclude: Samples to exclude from the ingroup. A list of sample names as they appear in the VCF file.
         :param seed: The seed for the random number generator.
+        :param subsample_mode: The subsampling mode. Either 'random' or 'probabilistic'.
         """
         # make sure the number of ingroups is at least 2
         if n_ingroups < 2:
             raise ValueError("The number of ingroups must be at least 2.")
 
+        # check subsample mode
+        if subsample_mode not in ['random', 'probabilistic']:
+            raise ValueError(f"Invalid subsample mode: {subsample_mode}")
+
         super().__init__()
 
         #: The ingroup samples to consider when determining the ancestral allele.
         self.ingroups: List[str] | None = ingroups
 
         #: The samples excluded from the ingroup.
         self.exclude: List[str] = exclude
@@ -1690,25 +1735,28 @@
 
         #: The number of outgroups.
         self.n_outgroups: int = len(outgroups)
 
         #: The seed for the random number generator.
         self.seed: int | None = seed
 
+        #: The subsampling mode.
+        self.subsample_mode: Literal['random', 'probabilistic'] = subsample_mode
+
         #: The random number generator.
         self.rng: np.random.Generator = np.random.default_rng(seed=self.seed)
 
         #: The outgroup mask.
-        self._outgroup_mask: np.ndarray[bool] | None = None
+        self._outgroup_mask: np.ndarray | None = None
 
         #: The outgroup indices.
-        self._outgroup_indices: np.ndarray[int] | None = None
+        self._outgroup_indices: np.ndarray | None = None
 
         #: The ingroup mask.
-        self._ingroup_mask: np.ndarray[bool] | None = None
+        self._ingroup_mask: np.ndarray | None = None
 
         #: 1-based positions of lowest and highest site position per contig (only when target_site_counter is used)
         # noinspection PyTypeChecker
         self._contig_bounds: Dict[str, Tuple[int, int]] = defaultdict(lambda: (np.inf, -np.inf))
 
     def _prepare_masks(self, samples: List[str]):
         """
@@ -1764,18 +1812,18 @@
         self._reader = self._handler.load_vcf()
 
         # prepare masks
         self._prepare_masks(handler._reader.samples)
 
     @staticmethod
     def _subsample(
-            genotypes: np.ndarray[Any],
+            genotypes: np.ndarray,
             size: int,
             rng: np.random.Generator
-    ) -> np.ndarray[str]:
+    ) -> np.ndarray:
         """
         Subsample a set of bases.
 
         :param genotypes: A list of bases.
         :param size: The size of the subsample.
         :return: A subsample of the bases.
         """
@@ -1788,17 +1836,17 @@
             replace=False
         )
 
         return genotypes[subsamples]
 
     @staticmethod
     def _get_outgroup_bases(
-            genotypes: np.ndarray[str],
+            genotypes: np.ndarray,
             n_outgroups: int
-    ) -> np.ndarray[str]:
+    ) -> np.ndarray:
         """
         Get the outgroup bases for a variant.
 
         :param genotypes: The VCF genotype strings.
         :param n_outgroups: The number of outgroups.
         :return: The outgroup bases.
         """
@@ -1813,17 +1861,17 @@
         return outgroup_bases
 
     @classmethod
     def _subsample_site(
             cls,
             mode: Literal['random', 'probabilistic'],
             n: int,
-            samples: np.ndarray[str],
+            samples: np.ndarray,
             rng: np.random.Generator
-    ) -> Tuple[np.ndarray[str], np.ndarray[int], np.ndarray[float]]:
+    ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         """
         Subsample a site, either randomly or probabilistically.
 
         :param mode: The subsampling mode.
         :param n: The number of ingroups to subsample to.
         :param samples: The samples.
         :return: Major alleles, major allele counts, and multiplicities,
@@ -1863,86 +1911,90 @@
             # flip alleles where the ref allele is not the major allele
             flip = n_majors < (n + 1) // 2
             n_majors[flip] = n - n_majors[flip]
             major_alleles[flip] = alt_allele
 
         return major_alleles, n_majors, m
 
-    def _parse_variant(self, variant: Variant | DummyVariant) -> List[SiteConfig] | None:
+    def _parse_variant(self, variant: Variant | DummyVariant) -> List[SiteConfig]:
         """
         Parse a VCF variant. We only consider sites that are at most bi-allelic in the in- and outgroups.
 
         :param variant: The variant.
-        :return: list of site configurations containing a single element if subsample_mode is `random` or
+        :return: List of site configurations containing a single element if subsample_mode is `random` or
             multiple elements if subsample_mode is `probabilistic` or ``None`` if the site is not valid.
+        :raises _TooFewIngroupsSiteError: If there are too few ingroups to consider a site for ancestral allele
+            annotation. _PolyAllelicSiteError: If a site has more than two alleles.
         """
         # get the called ingroup bases
         ingroups = get_called_bases(variant.gt_bases[self._ingroup_mask])
 
         # get the numer of called ingroup and outgroup bases
         n_ingroups = len(ingroups)
 
-        # only consider sites with enough ingroups
-        if n_ingroups >= self.n_ingroups:
+        # make sure we have enough ingroups
+        if n_ingroups < self.n_ingroups:
+            raise _TooFewIngroupsSiteError()
+
+        # get the called outgroup bases
+        # the order does not matter here
+        outgroups = get_called_bases(variant.gt_bases[self._outgroup_mask])
+
+        # get total base counts
+        counts = Counter(np.concatenate((ingroups, outgroups)))
+
+        # make sure we have at most two alleles
+        if len(counts) > 2:
+            raise _PolyAllelicSiteError()
+
+        # get the bases
+        b: List[str] = list(counts.keys())
+
+        # subsample ingroups either randomly or probabilistically
+        major_alleles, n_majors, multiplicities = self._subsample_site(
+            mode=self.subsample_mode,
+            n=self.n_ingroups,
+            samples=ingroups,
+            rng=self.rng
+        )
 
-            # get the called outgroup bases
-            # the order does not matter here
-            outgroups = get_called_bases(variant.gt_bases[self._outgroup_mask])
-
-            # get total base counts
-            counts = Counter(np.concatenate((ingroups, outgroups)))
-
-            # only consider sites where the in- and outgroups are at most bi-allelic
-            if len(counts) <= 2:
-
-                # get the bases
-                b: List[str] = list(counts.keys())
-
-                # subsample ingroups either randomly or probabilistically
-                major_alleles, n_majors, multiplicities = self._subsample_site(
-                    mode=self.subsample_mode,
-                    n=self.n_ingroups,
-                    samples=ingroups,
-                    rng=self.rng
-                )
+        # Get the outgroup bases.
+        # The outgroup order is important, so we can't use the mask here.
+        outgroup_bases = self.get_base_index(self._get_outgroup_bases(
+            genotypes=np.array([variant.gt_bases[i] for i in self._outgroup_indices]),
+            n_outgroups=self.n_outgroups
+        ))
 
-                # Get the outgroup bases.
-                # The outgroup order is important, so we can't use the mask here.
-                outgroup_bases = self.get_base_index(self._get_outgroup_bases(
-                    genotypes=np.array([variant.gt_bases[i] for i in self._outgroup_indices]),
-                    n_outgroups=self.n_outgroups
-                ))
-
-                # create site configurations
-                sites = []
-                for i, (major_allele, n_major, multiplicity) in enumerate(zip(major_alleles, n_majors, multiplicities)):
-
-                    if multiplicity > 0:
-                        if len(counts) == 2:
-                            # Take the other allele as the minor allele. We keep track of the minor allele
-                            # even if it wasn't contained in the ingroup subsample.
-                            minor_base: str = b[0] if b[0] != major_allele else b[1]
-                        else:
-                            minor_base: str = '.'
+        # create site configurations
+        sites = []
+        for i, (major_allele, n_major, multiplicity) in enumerate(zip(major_alleles, n_majors, multiplicities)):
+
+            if multiplicity > 0:
+                if len(counts) == 2:
+                    # Take the other allele as the minor allele. We keep track of the minor allele
+                    # even if it wasn't contained in the ingroup subsample.
+                    minor_base: str = b[0] if b[0] != major_allele else b[1]
+                else:
+                    minor_base: str = '.'
 
-                        # create site configuration
-                        site = SiteConfig(
-                            major_base=base_indices[major_allele],
-                            n_major=n_major,
-                            minor_base=self.get_base_index(minor_base),
-                            outgroup_bases=outgroup_bases,
-                            multiplicity=multiplicity
-                        )
+                # create site configuration
+                site = SiteConfig(
+                    major_base=base_indices[major_allele],
+                    n_major=n_major,
+                    minor_base=self.get_base_index(minor_base),
+                    outgroup_bases=outgroup_bases,
+                    multiplicity=multiplicity
+                )
 
-                        sites.append(site)
+                sites.append(site)
 
-                return sites
+        return sites
 
     @staticmethod
-    def get_base_string(indices: int | np.ndarray[int]) -> str | np.ndarray[str]:
+    def get_base_string(indices: int | np.ndarray) -> str | np.ndarray:
         """
         Get base string(s) from base index/indices.
 
         :param indices: The base index/indices.
         :return: Base string(s).
         """
         if isinstance(indices, np.ndarray):
@@ -1960,15 +2012,15 @@
         # assume integer
         if indices != -1:
             return bases[indices]
 
         return '.'
 
     @classmethod
-    def get_base_index(cls, base_string: str | np.ndarray[str]) -> int | np.ndarray[int]:
+    def get_base_index(cls, base_string: str | np.ndarray) -> int | np.ndarray:
         """
         Get base index/indices from base string(s).
 
         :param base_string: The base string(s).
         :return: Base index/indices.
         """
         if isinstance(base_string, np.ndarray):
@@ -2064,17 +2116,17 @@
     def __init__(
             self,
             outgroups: List[str],
             n_ingroups: int = 11,
             ingroups: List[str] | None = None,
             exclude: List[str] | None = None,
             n_runs: int = 10,
-            model: SubstitutionModel = K2SubstitutionModel(),
+            model: SubstitutionModel = None,
             parallelize: bool = True,
-            prior: PolarizationPrior | None = KingmanPolarizationPrior(),
+            prior: PolarizationPrior | None = '',
             max_sites: int = 10000,
             seed: int | None = 0,
             confidence_threshold: float = 0,
             n_target_sites: int | None = None,
             subsample_mode: Literal['random', 'probabilistic'] = 'probabilistic'
     ):
         """
@@ -2106,22 +2158,25 @@
             number of ingroups.
         :param ingroups: The ingroup samples to consider when determining the ancestral allele. If ``None``,
             all (non-outgroup) samples are considered. A list of sample names as they appear in the VCF file.
             Has to be at least as large as ``n_ingroups``.
         :param exclude: Samples to exclude from the ingroup. A list of sample names as they appear in the VCF file.
         :param n_runs: The number of optimization runs to perform when determining the branch rates. You can
             check that the likelihoods of the different runs are similar by calling :meth:`plot_likelihoods`.
+        :param model: The substitution model to use. By default, :class:`K2SubstitutionModel` is used.
         :param parallelize: Whether to parallelize the computation across multiple cores.
-        :param prior: The prior to use for the polarization probabilities. See :class:`PolarizationPrior`, 
-            :class:`KingmanPolarizationPrior` and :class:`AdaptivePolarizationPrior` for more information.
+        :param prior: The prior to use for the polarization probabilities. See
+            :class:`KingmanPolarizationPrior` and :class:`AdaptivePolarizationPrior` for more information. By default,
+            :class:`KingmanPolarizationPrior` is used. Use ``None`` for no prior.
         :param max_sites: The maximum number of sites to consider. This is useful if the number of sites is very large.
             Choosing a reasonably large subset of sites (on the order of a few thousand bi-allelic sites) can speed up
             the computation considerably as parsing can be slow. This subset is then used to calibrate the rate
             parameters, and possibly the polarization priors.
-        :param seed: The seed for the random number generator. If ``None``, a random seed is chosen.
+        :param seed: The seed for the random number generator. If ``None``, a random seed is chosen. By default, the
+            seed is set to 0.
         :param confidence_threshold: The confidence threshold for the ancestral allele annotation.
             Only if the probability of the major allele being ancestral as opposed to
             the minor allele is not within ``((1 - confidence_threshold) / 2, 1 - (1 - confidence_threshold) / 2)``,
             the ancestral allele is annotated. This is useful to avoid annotating sites where the ancestral allele
             state is not clear. Use values close to ``0`` to annotate as many sites as possible, and values close to
             ``1`` to annotate only sites where the ancestral allele state is very clear.
 
@@ -2147,15 +2202,16 @@
             recommended.
         """
         super().__init__(
             ingroups=ingroups,
             exclude=exclude,
             outgroups=outgroups,
             n_ingroups=n_ingroups,
-            seed=seed
+            seed=seed,
+            subsample_mode=subsample_mode
         )
 
         # check that we have at least one outgroup
         if len(outgroups) < 1:
             raise ValueError("Must specify at least one outgroup. If you do not have any outgroup "
                              "information, consider using MaximumParsimonyAncestralAnnotation instead.")
 
@@ -2166,53 +2222,49 @@
                                  "provide sufficiently many ingroups.")
 
         # raise warning on bias
         if confidence_threshold > 0:
             self._logger.warning("Please be aware that a confidence threshold of greater than 0 biases the SFS "
                                  "towards fewer high-frequency derived alleles.")
 
-        # check subsample mode
-        if subsample_mode not in ['random', 'probabilistic']:
-            raise ValueError(f"Invalid subsample mode: {subsample_mode}")
-
         #: Whether to parallelize the computation.
         self.parallelize: bool = parallelize
 
         #: Maximum number of sites to consider
         self.max_sites: int = max_sites
 
         #: The confidence threshold for the ancestral allele annotation.
         self.confidence_threshold: float = confidence_threshold
 
         #: The prior to use for the polarization probabilities.
-        self.prior: PolarizationPrior | None = prior
+        self.prior: PolarizationPrior | None = KingmanPolarizationPrior() if prior == '' else prior
 
         #: Number of random ML starts when determining the rate parameters
         self.n_runs: int = int(n_runs)
 
         #: The substitution model.
-        self.model: SubstitutionModel = model
+        self.model: SubstitutionModel = K2SubstitutionModel() if model is None else model
 
         #: The VCF reader.
         self._reader: VCF | None = None
 
         #: The data frame holding all site configurations.
         self.configs: pd.DataFrame | None = None
 
         #: The probability of all sites per frequency bin.
-        self.p_bins: Dict[str, np.ndarray[float, (n_ingroups - 1,)]] | None = None
+        self.p_bins: Dict[str, np.ndarray | None] = None
 
         #: The total number of valid sites parsed (including sites not considered for ancestral allele inference).
         self.n_sites: int | None = None
 
         #: The parameter names in the order they are passed to the optimizer.
         self.param_names: List[str] = list(self.model.get_bounds(self.n_outgroups).keys())
 
         #: The log likelihoods for the different runs when optimizing the rate parameters.
-        self.likelihoods: np.ndarray[float, (...,)] | None = None
+        self.likelihoods: np.ndarray | None = None
 
         #: The best log likelihood when optimizing the rate parameters.
         self.likelihood: float | None = None
 
         #: Optimization result of the best run.
         self.result: Optional['scipy.optimize.OptimizeResult'] = None
 
@@ -2223,17 +2275,14 @@
         # This is only computed when annotating a VCF file, and only contains the mismatches
         # for sites that were actually annotated.
         self.mismatches: List[SiteInfo] = []
 
         #: The total number of target sites.
         self.n_target_sites: int | None = n_target_sites
 
-        #: The subsampling mode.
-        self.subsample_mode: Literal['random', 'probabilistic'] = subsample_mode
-
     def _setup(self, handler: MultiHandler):
         """
         Parse the VCF file and perform the optimization.
 
         :param handler: The handler.
         """
         from .parser import Parser, TargetSiteCounter
@@ -2448,17 +2497,17 @@
         # return new columns only
         return data.drop(range(n_outgroups + 1), axis=1)
 
     @classmethod
     def from_est_sfs(
             cls,
             file: str,
-            prior: PolarizationPrior | None = KingmanPolarizationPrior(),
+            prior: PolarizationPrior | None = '',
             n_runs: int = 10,
-            model: SubstitutionModel = K2SubstitutionModel(),
+            model: SubstitutionModel = None,
             parallelize: bool = True,
             seed: int = 0,
             chunk_size: int = 100000
     ) -> 'MaximumLikelihoodAncestralAnnotation':
         """
         Create instance from EST-SFS input file.
 
@@ -2558,26 +2607,87 @@
                     '\n'
                 )
 
                 # break if we reached the maximum number of sites
                 if i + 1 >= self.max_sites:
                     break
 
+    def to_file(self, file: str):
+        """
+        Save object to file.
+
+        .. note::
+            References to the handler and the reader are discarded.
+
+        :param file: File path.
+        """
+        with open(file, 'w') as fh:
+            fh.write(self.to_json())
+
+    @classmethod
+    def from_file(cls, file: str) -> 'MaximumLikelihoodAncestralAnnotation':
+        """
+        Load object from file.
+
+        .. note::
+            The handler and the reader are not restored, so serialization is mostly useful
+            for analyzing the results in detail, not for further processing.
+
+        :param file: File path.
+        :return: The object.
+        """
+        with open(file, 'r') as fh:
+            return cls.from_json(fh.read())
+
+    def to_json(self) -> str:
+        """
+        Serialize object.
+
+        .. note::
+            References to the handler and the reader are discarded.
+
+        :return: JSON string
+        """
+        self._reader = None
+        self._handler = None
+
+        return jsonpickle.encode(self, indent=4, warn=True)
+
+    @classmethod
+    def from_json(cls, json: str) -> 'MaximumLikelihoodAncestralAnnotation':
+        """
+        Load object from file.
+
+        .. note::
+            The handler and the reader are not restored, so serialization is mostly useful
+            for analyzing the results in detail, not for further processing.
+
+        :param json: JSON string.
+        :return: The object.
+        """
+        anc = jsonpickle.decode(json)
+
+        # convert index to int if necessary
+        if 'index' in anc.configs:
+            anc.configs.index = anc.configs.index.astype(int)
+
+        return anc
+
     @classmethod
     def from_data(
             cls,
             n_major: Iterable[int],
             major_base: Iterable[str | int],
             minor_base: Iterable[str | int],
             outgroup_bases: Iterable[Iterable[str | int]],
             n_ingroups: int,
             n_runs: int = 10,
-            model: SubstitutionModel = K2SubstitutionModel(),
+            model: SubstitutionModel = None,
             parallelize: bool = True,
-            prior: PolarizationPrior | None = KingmanPolarizationPrior(),
+            prior: PolarizationPrior | None = '',
             seed: int = 0,
             pass_indices: bool = False,
             confidence_threshold: float = 0
     ) -> 'MaximumLikelihoodAncestralAnnotation':
         """
         Create an instance by passing the data directly.
 
@@ -2704,17 +2814,17 @@
 
     @classmethod
     def from_dataframe(
             cls,
             data: pd.DataFrame,
             n_ingroups: int,
             n_runs: int = 10,
-            model: SubstitutionModel = K2SubstitutionModel(),
+            model: SubstitutionModel = None,
             parallelize: bool = True,
-            prior: PolarizationPrior | None = KingmanPolarizationPrior(),
+            prior: PolarizationPrior | None = '',
             seed: int = 0,
             grouped: bool = False,
             confidence_threshold: float = 0
     ) -> 'MaximumLikelihoodAncestralAnnotation':
         """
         Create an instance from a dataframe.
 
@@ -2738,15 +2848,14 @@
 
         if not grouped:
             # only keep the columns that are needed
             data = data[cls._group_cols]
 
             # disable chained assignment warning
             with pd.option_context('mode.chained_assignment', None):
-
                 # retain site index
                 data['sites'] = data.index
 
                 # convert outgroup bases to tuples
                 data['outgroup_bases'] = data['outgroup_bases'].apply(tuple)
 
             # group by all columns in the chunk and keep track of the site indices
@@ -2781,22 +2890,32 @@
             confidence_threshold=confidence_threshold,
             subsample_mode='random'
         )
 
         # assign data frame
         anc.configs = data
 
+        # convert outgroup bases to tuples of native integers
+        anc._convert_outgroup_bases_to_native_types()
+
         # set the number of sites (which coincides with number of sites parsed)
         anc.n_sites = anc._get_n_sites()
 
         # notify about the number of sites
         anc._logger.info(f"Included {int(anc._get_mle_configs().multiplicity.sum())} sites for the inference.")
 
         return anc
 
+    def _convert_outgroup_bases_to_native_types(self):
+        """
+        Convert outgroup bases to tuples of native integers
+        numpy types cause problems when serializing
+        """
+        self.configs.outgroup_bases = self.configs.outgroup_bases.apply(lambda x: tuple(int(i) for i in x))
+
     def _parse_vcf(self):
         """
         Parse variants from VCF file.
         """
         # initialize data frame
         self.configs = pd.DataFrame(columns=list(self._dtypes.keys()))
         self.configs.astype(self._dtypes)
@@ -2819,18 +2938,21 @@
         # create progress bar
         with self._handler.get_pbar(desc=f"{self.__class__.__name__}>Parsing sites", total=total) as pbar:
 
             # iterate over sites
             for i, variant in enumerate(self._reader):
 
                 # parse the site
-                configs = self._parse_variant(variant)
+                try:
+                    configs = self._parse_variant(variant)
 
-                # check if site is not None
-                if configs is not None:
+                except (_PolyAllelicSiteError, _TooFewIngroupsSiteError):
+                    pass
+
+                else:
 
                     if self.n_target_sites is not None:
                         # update bounds
                         low, high = self._contig_bounds[variant.CHROM]
                         self._contig_bounds[variant.CHROM] = (min(low, variant.POS), max(high, variant.POS))
 
                     for config in configs:
@@ -2869,14 +2991,17 @@
         # create column for number of outgroups
         self.configs['n_outgroups'] = None
 
         if len(self.configs) > 0:
             # determine number of outgroups
             self.configs['n_outgroups'] = np.sum(np.array(self.configs.outgroup_bases.to_list()) != -1, axis=1)
 
+        # convert outgroup bases to tuples of native integers
+        self._convert_outgroup_bases_to_native_types()
+
         # total number of sites considered
         self.n_sites = i + 1
 
     def infer(self):
         """
         Infer the ancestral allele probabilities for the data provided. This method is only supposed to be called
         manually if the data is provided directly, e.g. using :meth:`from_data`, :meth:`from_dataframe` or
@@ -3022,30 +3147,30 @@
         # get the outgroup divergence
         div = self.get_outgroup_divergence()
 
         # check if the outgroup divergence is monotonically increasing
         return all(div[i] <= div[i + 1] for i in range(len(div) - 1))
 
     @cached_property
-    def p_polarization(self) -> np.ndarray[float, (...,)] | None:
+    def p_polarization(self) -> np.ndarray | None:
         """
         Get the polarization probabilities or ``None`` if ``prior`` is ``no``.
         """
         if isinstance(self.prior, PolarizationPrior):
             return self.prior._get_prior(
                 configs=self.configs,
                 n_ingroups=self.n_ingroups
             )
 
     @staticmethod
     def get_p_tree(
             base: int,
             n_outgroups: int,
-            internal_nodes: List[int] | np.ndarray[int],
-            outgroup_bases: List[int] | np.ndarray[int],
+            internal_nodes: List[int] | np.ndarray,
+            outgroup_bases: List[int] | np.ndarray,
             params: Dict[str, float],
             model: SubstitutionModel
     ) -> float:
         """
         Get the probability of a tree.
 
         :param base: An observed ingroup base index.
@@ -3100,15 +3225,15 @@
     @classmethod
     def get_p_config(
             cls,
             config: SiteConfig,
             base_type: BaseType,
             params: Dict[str, float],
             model: SubstitutionModel = K2SubstitutionModel(),
-            internal: np.ndarray[int] | None = None
+            internal: np.ndarray | None = None
     ) -> float:
         """
         Get the probability for a site configuration.
 
         :param config: The site configuration.
         :param base_type: The base type.
         :param params: The parameters for the substitution model.
@@ -3168,15 +3293,15 @@
     @classmethod
     def get_p_configs(
             cls,
             configs: pd.DataFrame,
             model: SubstitutionModel,
             base_type: BaseType,
             params: Dict[str, float]
-    ) -> np.ndarray[float, (...,)]:
+    ) -> np.ndarray:
         """
         Get the probabilities for each site configuration.
 
         :param configs: The site configurations.
         :param model: The substitution model.
         :param base_type: The base type.
         :param params: A dictionary of the rate parameters.
@@ -3307,18 +3432,18 @@
             for j in config.sites:
                 indices[j] = i
 
         return indices
 
     def _get_ancestral_from_prob(
             self,
-            p_major_ancestral: np.ndarray[float] | float,
-            major_base: np.ndarray[str] | str,
-            minor_base: np.ndarray[str] | str
-    ) -> np.ndarray[float] | float:
+            p_major_ancestral: np.ndarray | float,
+            major_base: np.ndarray | str,
+            minor_base: np.ndarray | str
+    ) -> np.ndarray | float:
         """
         Get the ancestral allele from the probability of the major allele being ancestral.
 
         :param p_major_ancestral: The probabilities of the major allele being ancestral.
         :param major_base: The major bases.
         :param minor_base: The minor bases.
         :return: Array of ancestral alleles.
@@ -3338,15 +3463,15 @@
         ancestral_bases[p_major_ancestral < 0.5] = minor_base[p_major_ancestral < 0.5]
 
         return ancestral_bases
 
     def _get_internal_prob(
             self,
             site: SiteConfig,
-            internal: np.ndarray[int] | None = None
+            internal: np.ndarray | None = None
     ) -> float:
         """
         Get the ancestral allele for each site.
 
         :param site: The site configuration.
         :param internal: Base indices of internal nodes of the tree if fixed. If ``None``, the internal nodes
             are considered as free parameters. -1 also indicates a free parameter.
@@ -3373,15 +3498,15 @@
 
         return p_minor + p_major
 
     def _get_internal_probs(
             self,
             site: SiteConfig,
             i_internal: int,
-    ) -> np.ndarray[float, (...,)]:
+    ) -> np.ndarray:
         """
         Get the internal probabilities for the sites used to estimate the parameters.
 
         :param site: The site configuration.
         :param i_internal: The index of the internal node.
         :return: The probabilities for each base and site.
         """
@@ -3515,15 +3640,15 @@
         )
 
     def get_site_info(
             self,
             n_major: int,
             major_base: int | str,
             minor_base: int | str,
-            outgroup_bases: List[int | str] | np.ndarray[int | str],
+            outgroup_bases: List[int | str] | np.ndarray,
             pass_indices: bool = False
     ) -> SiteInfo:
         """
         Get information on the specified sites using the inferred parameters.
 
         :param n_major: The number of copies of the major allele.
         :param major_base: The major bases indices or strings.
@@ -3545,18 +3670,18 @@
             outgroup_bases=outgroup_bases
         )
 
         return self._get_site_info([config])
 
     def _calculate_p_major_ancestral(
             self,
-            p_minor: float | np.ndarray[float],
-            p_major: float | np.ndarray[float],
-            n_major: int | np.ndarray[int]
-    ) -> float | np.ndarray[float]:
+            p_minor: float | np.ndarray,
+            p_major: float | np.ndarray,
+            n_major: int | np.ndarray
+    ) -> float | np.ndarray:
         """
         Calculate the probability that the ancestral allele is the major allele.
 
         :param p_minor: The probability or probabilities of the minor allele.
         :param p_major: The probability or probabilities of the major allele.
         :param n_major: The number or numbers of major alleles.
         :return: The probability or probabilities that the ancestral allele is the major allele.
@@ -3596,29 +3721,35 @@
         Annotate a single site.
 
         :param variant: The variant to annotate.
         :return: The annotated variant.
         """
         # set default values
         ancestral_base = '.'
-        ancestral_info = '.'
 
         # use maximum parsimony if we don't have an SNP
         if isinstance(variant, DummyVariant) or not variant.is_snp:
             ancestral_base = MaximumParsimonyAncestralAnnotation._get_ancestral(variant, self._ingroup_mask)
             ancestral_info = 'monomorphic'
 
             # increase the number of annotated sites
             self.n_annotated += 1
 
         else:
 
-            configs = self._parse_variant(variant)
+            try:
+                configs = self._parse_variant(variant)
+
+            except _PolyAllelicSiteError:
+                ancestral_info = 'polyallelic'
 
-            if configs is not None:
+            except _TooFewIngroupsSiteError:
+                ancestral_info = 'too few ingroups'
+
+            else:
                 site = self._get_site_info(configs)
 
                 # only proceed if the ancestral allele is known
                 if site.major_ancestral in bases:
 
                     # get site information dictionary
                     site_dict = site.__dict__
@@ -3650,14 +3781,20 @@
 
                         # update ancestral base
                         ancestral_base = site.major_ancestral
 
                         # increase the number of annotated sites
                         self.n_annotated += 1
 
+                    else:
+                        ancestral_info = 'below confidence threshold'
+
+                else:
+                    ancestral_info = 'invalid or unknown ancestral allele'
+
         # set the ancestral allele
         variant.INFO[self._handler.info_ancestral] = ancestral_base
 
         # set info field
         variant.INFO[self._handler.info_ancestral + "_info"] = ancestral_info
 
     def plot_likelihoods(
@@ -3742,15 +3879,15 @@
 
         :param params: The parameters.
         :param i: The index.
         :return: The branch rate.
         """
         return params['K'] if 'K' in params else params[f'K{i}']
 
-    def get_outgroup_divergence(self) -> np.ndarray[float]:
+    def get_outgroup_divergence(self) -> np.ndarray:
         """
         Get the inferred branch rates between the ingroup and outgroups by combining the inferred branch rates.
 
         :return: One rate for each outgroup.
         """
         if self.params_mle is None:
             raise RuntimeError("No maximum likelihood parameters available.")
@@ -3816,59 +3953,63 @@
 
         return dict(
             ancestral_base=ancestral_base
         )
 
     def annotate_site(self, variant: Variant | DummyVariant):
         """
-        Annotate a single sites. Mono-allelic sites are assigned the major allele as ancestral. Sites with
+        Annotate a single site. Mono-allelic sites are assigned the major allele as ancestral. Sites with
         more than two alleles are ignored.
 
         :param variant: The variant to annotate.
         :return: The annotated variant.
         """
         ancestral_base = '.'
-        ancestral_info = '.'
 
         # use maximum parsimony if we have a mono-allelic site
         if isinstance(variant, DummyVariant) or not variant.is_snp:
             ancestral_base = MaximumParsimonyAncestralAnnotation._get_ancestral(variant, self._ingroup_mask)
             ancestral_info = 'monomorphic'
+            self.n_annotated += 1
+        else:
 
-        # parse the site
-        configs = self._parse_variant(variant)
+            try:
+                # parse the site
+                configs = self._parse_variant(variant)
 
-        if configs is not None:
+            except _PolyAllelicSiteError:
+                ancestral_info = 'polyallelic'
 
-            # use most likely configuration as reference
-            ref = configs[np.argmax([c.multiplicity for c in configs])]
+            except _TooFewIngroupsSiteError:
+                ancestral_info = 'too few ingroups'
 
-            # get site information dictionary
-            site = self._get_site_info(ref)
+            else:
 
-            # only proceed if the ancestral allele is known
-            if site['ancestral_base'] in bases:
+                # use config with the highest multiplicity
+                ref = configs[np.argmax([c.multiplicity for c in configs])]
 
-                if site['major_base'] != site['ancestral_base']:
-                    self._logger.debug(dict(site=f"{variant.CHROM}:{variant.POS}") | site)
+                # get site information dictionary
+                site = self._get_site_info(ref)
 
-                ancestral_base = site['ancestral_base']
-                ancestral_info = str(site)
+                # only proceed if the ancestral allele is known
+                if site['ancestral_base'] in bases:
+                    ancestral_base = site['ancestral_base']
+                    ancestral_info = str(site)
+                    self.n_annotated += 1
+                else:
+                    ancestral_info = 'invalid or unknown ancestral allele'
 
         # set the ancestral allele
         variant.INFO[self._handler.info_ancestral] = ancestral_base
 
         # set info field
         variant.INFO[self._handler.info_ancestral + "_info"] = ancestral_info
 
-        # increase the number of annotated sites
-        self.n_annotated += 1
 
-
-class _ESTSFSAncestralAnnotation(AncestralAlleleAnnotation):
+class _ESTSFSAncestralAnnotation(AncestralAlleleAnnotation):  # pragma: no cover
     """
     A wrapper around EST-SFS. Used for testing.
     """
 
     def __init__(
             self,
             anc: MaximumLikelihoodAncestralAnnotation
@@ -3880,15 +4021,15 @@
         """
         super().__init__()
 
         #: The ancestral annotation.
         self.anc = anc
 
         #: The likelihoods for each run.
-        self.likelihoods: np.ndarray[float] | None = None
+        self.likelihoods: np.ndarray | None = None
 
         #: The minimum likelihood.
         self.likelihood: float | None = None
 
         #: The MLE parameters.
         self.params_mle: Dict[str, float] | None = None
 
@@ -4021,14 +4162,54 @@
         Not implemented.
 
         :param variant: The variant to annotate.
         :raises: NotImplementedError
         """
         raise NotImplementedError
 
+    def to_file(self, file: str):
+        """
+        Save object to file (without reference to AncestralAlleleAnnotation object).
+
+        :param file: File path.
+        """
+        self.anc = None
+
+        with open(file, 'w') as fh:
+            fh.write(self.to_json())
+
+    def to_json(self) -> str:
+        """
+        Serialize object.
+
+        :return: JSON string
+        """
+        return jsonpickle.encode(self, indent=4, warn=True)
+
+    @classmethod
+    def from_json(cls, json: str, classes=None) -> 'Self':
+        """
+        Unserialize object.
+
+        :param classes: Classes to be used for unserialization
+        :param json: JSON string
+        """
+        return jsonpickle.decode(json, classes=classes)
+
+    @classmethod
+    def from_file(cls, file: str, classes=None) -> 'Self':
+        """
+        Load object from file.
+
+        :param classes: Classes to be used for unserialization
+        :param file: File to load from
+        """
+        with open(file, 'r') as fh:
+            return cls.from_json(fh.read(), classes)
+
 
 class Annotator(MultiHandler):
     """
     Annotate a VCF file with the given annotations.
 
     Example usage:
```

### Comparing `fastdfe-1.1.6/fastdfe/base_inference.py` & `fastdfe-1.1.7/fastdfe/base_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import copy
 import functools
 import itertools
 import json
 import logging
 import time
-from typing import List, Optional, Dict, Literal, cast, Tuple
+from typing import List, Optional, Dict, Literal, cast, Tuple, Sequence
 
 import jsonpickle
 import multiprocess as mp
 import numpy as np
 import pandas as pd
 from numpy.linalg import norm
 from scipy.stats import chi2
@@ -92,16 +92,16 @@
         # gtol=1e-10
     )
 
     def __init__(
             self,
             sfs_neut: Spectra | Spectrum,
             sfs_sel: Spectra | Spectrum,
-            intervals_del: (float, float, int) = (-1.0e+8, -1.0e-5, 1000),
-            intervals_ben: (float, float, int) = (1.0e-5, 1.0e4, 1000),
+            intervals_del: Tuple[float, float, int] = (-1.0e+8, -1.0e-5, 1000),
+            intervals_ben: Tuple[float, float, int] = (1.0e-5, 1.0e4, 1000),
             integration_mode: Literal['midpoint', 'quad'] = 'midpoint',
             linearized: bool = True,
             model: Parametrization | str = 'GammaExpParametrization',
             seed: int = 0,
             x0: Dict[str, Dict[str, float]] = {},
             bounds: Dict[str, Tuple[float, float]] = {},
             scales: Dict[str, Literal['lin', 'log', 'symlog']] = {},
@@ -289,30 +289,32 @@
 
             if not fixed_dele.issubset(fixed):
                 self._logger.warning("You are estimating the full DFE, but the SFS are folded. "
                                      "This is not recommend as the folded SFS contains little information "
                                      "on beneficial mutations.")
 
         #: Initial values
-        self.x0 = dict(all=self.model.x0 | self._default_x0 | (x0['all'] if 'all' in x0 else {}))
+        self.x0: Dict[str, Dict[str, float]] = dict(
+            all=self.model.x0 | self._default_x0 | (x0['all'] if 'all' in x0 else {})
+        )
 
         #: Bootstrapped MLE parameter estimates
         self.bootstraps: Optional[pd.DataFrame] = None
 
         #: Bootstrap optimization results
         self.bootstrap_results: Optional[List['scipy.optimize.OptimizeResult']] = None
 
         #: L2 norm of differential between modelled and observed SFS
         self.L2_residual: Optional[float] = None
 
         #: Random number generator seed
         self.seed: int | None = int(seed) if seed is not None else None
 
         #: Random generator instance
-        self.rng = np.random.default_rng(seed=seed)
+        self.rng: np.random.Generator = np.random.default_rng(seed=seed)
 
         #: Total execution time in seconds
         self.execution_time: float = 0
 
         #: Whether inferences can be run from the class itself
         self.locked: bool = locked
 
@@ -567,16 +569,17 @@
         param_string = str(flatten_dict(params)).replace('\'', '')
 
         self._logger.info(f"Inferred parameters: {param_string}.")
 
     def update_properties(self, **kwargs) -> Self:
         """
         Update the properties of this class with the given dictionary
-        given that its entries are not None.
+        given that its entries are not ``None``.
 
+        :meta private:
         :param kwargs: Dictionary of properties to update.
         :return: Self.
         """
         for key, value in kwargs.items():
             if value is not None:
                 setattr(self, key, value)
 
@@ -939,15 +942,15 @@
         )
 
     @_run_if_required_wrapper
     def plot_interval_density(
             self,
             file: str = None,
             show: bool = True,
-            intervals: list | np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
+            intervals: Sequence = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             interval_labels: List[str] = None,
             color: str = 'C0',
             ax: 'plt.Axes' = None
     ) -> 'plt.Axes':
         """
         Plot density of the discretization intervals chosen. Note that although this plot looks similar, this is
         not the DFE!
```

### Comparing `fastdfe-1.1.6/fastdfe/bootstrap.py` & `fastdfe-1.1.7/fastdfe/bootstrap.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-02-26"
 
 import logging
-from typing import Literal
+from typing import Literal, Sequence
 
 import numpy as np
 from scipy.stats import norm as normal
 
 # get logger
 logger = logging.getLogger('fastdfe').getChild('Bootstrap')
 
 
 class Bootstrap:
     """
     Bootstrap utilities.
     """
 
     @staticmethod
-    def get_bounds_from_quantile(data: list | np.ndarray, a1: float, a2: float, n: int) -> (float, float):
+    def get_bounds_from_quantile(data: Sequence, a1: float, a2: float, n: int) -> (float, float):
         """
         Get confidence interval bounds.
 
         :param data: Sorted data
         :param a1: Lower quantile
         :param a2: Upper quantile
         :param n: Number of data points
@@ -34,39 +34,39 @@
         """
         if np.isnan(a1) or np.isnan(a2):
             return [None, None]
 
         return data[max(round(a1 * n), 0)], data[min(round(a2 * n), n - 1)]
 
     @staticmethod
-    def get_ci_percentile(bootstraps: list | np.ndarray, a: float) -> (float, float):
+    def get_ci_percentile(bootstraps: Sequence, a: float) -> (float, float):
         """
         Get the (1 - a)% confidence intervals using the percentile bootstrap.
 
         :param bootstraps: List of bootstraps
         :param a: Confidence level
         :return: lower bound and upper bound
         """
         if not 0 <= a <= 0.5:
             raise ValueError('Confidence level must be between 0 and 0.5.')
 
         return Bootstrap.get_bounds_from_quantile(np.sort(bootstraps), a, 1 - a, len(bootstraps))
 
     @staticmethod
-    def get_ci_bca(bootstraps: list | np.ndarray, original: float, a: float) -> (float, float):
+    def get_ci_bca(bootstraps: Sequence, original: float, a: float) -> (float, float):
         """
         Get the (1 - a)% confidence intervals using the BCa method.
         cf. An Introduction to the Bootstrap, Bradley Efron, Robert J. Tibshirani, section 14.2.
 
         :param bootstraps: List of bootstraps
         :param original: Original value
         :param a: Confidence level
         :return: lower bound and upper bound
         """
-        if sum(bootstraps) == 0:
+        if len(bootstraps) == 0:
             return [0, 0]
 
         n = len(bootstraps)
         data = np.sort(np.array(bootstraps))
 
         theta_hat_i = np.array([np.var(np.delete(data, i)) for i in range(n)])
         theta_hat = sum(theta_hat_i) / n
@@ -80,15 +80,15 @@
         a1 = normal.cdf(z0_hat + (z0_hat + z_a) / (1 - a_hat * (z0_hat + z_a)))
         a2 = normal.cdf(z0_hat + (z0_hat - z_a) / (1 - a_hat * (z0_hat - z_a)))
 
         return Bootstrap.get_bounds_from_quantile(data, a1, a2, n)
 
     @staticmethod
     def get_errors(
-            values: list | np.ndarray,
+            values: Sequence,
             bs: np.ndarray,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile'
     ) -> (np.ndarray, np.ndarray):
         """
         Get error values and confidence intervals from the list of original
         values and its bootstraps for a list of parameters.
```

### Comparing `fastdfe-1.1.6/fastdfe/config.py` & `fastdfe-1.1.7/fastdfe/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,16 @@
     def __init__(
             self,
             polydfe_spectra_config: str = None,
             polydfe_init_file: str = None,
             polydfe_init_file_id: int = 1,
             sfs_neut: Spectra | Spectrum = None,
             sfs_sel: Spectra | Spectrum = None,
-            intervals_del: (float, float, int) = (-1.0e+8, -1.0e-5, 1000),
-            intervals_ben: (float, float, int) = (1.0e-5, 1.0e4, 1000),
+            intervals_del: Tuple[float, float, int] = (-1.0e+8, -1.0e-5, 1000),
+            intervals_ben: Tuple[float, float, int] = (1.0e-5, 1.0e4, 1000),
             integration_mode: Literal['midpoint', 'quad'] = 'midpoint',
             linearized: bool = True,
             model: Parametrization | str = 'GammaExpParametrization',
             seed: int = 0,
             x0: Dict[str, Dict[str, float]] = {},
             bounds: Dict[str, Tuple[float, float]] = {},
             scales: Dict[str, Literal['lin', 'log', 'symlog']] = {},
@@ -288,15 +288,15 @@
         :param file: Path to file, possibly gzipped.
         :param cache: Whether to use the cache if available.
         :return: Config object.
         """
         with open(download_if_url(file, cache=cache, desc=f'{cls.__name__}>Downloading file'), 'r') as fh:
             return Config.from_yaml(fh.read())
 
-    def get_polydfe_model(self) -> str:
+    def get_polydfe_model(self) -> str:  # pragma: no cover
         """
         Get the model name in polyDFE that corresponds
         to the configured DFE parametrization.
 
         :return: polyDFE model name.
         """
         # get name of configured model
```

### Comparing `fastdfe-1.1.6/fastdfe/discretization.py` & `fastdfe-1.1.7/fastdfe/discretization.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-02-26"
 
 import logging
 from functools import cached_property, wraps
-from typing import Literal
+from typing import Literal, Sequence, Tuple
 
 import mpmath as mp
 import numpy as np
 from scipy.integrate import quad
 
 from .optimization import parallelize as parallelize_func
 from .parametrization import Parametrization
@@ -200,16 +200,16 @@
     in each optimizing iteration.
     The loss function supports Poisson likelihoods and the L2 norm.
     """
 
     def __init__(
             self,
             n: int,
-            intervals_del: (float, float, int) = (-1.0e+8, -1.0e-5, 1000),
-            intervals_ben: (float, float, int) = (1.0e-5, 1.0e4, 1000),
+            intervals_del: Tuple[float, float, int] = (-1.0e+8, -1.0e-5, 1000),
+            intervals_ben: Tuple[float, float, int] = (1.0e-5, 1.0e4, 1000),
             integration_mode: Literal['midpoint', 'quad'] = 'midpoint',
             linearized: bool = True,
             parallelize: bool = True,
     ):
         """
         Create Discretization instance.
 
@@ -465,15 +465,15 @@
         """
         y = model._discretize(params, self.bins) * H_fixed_regularized(self.s)
 
         return np.sum(y[self.s > 0]) / np.sum(y)
 
     def get_interval_density(
             self,
-            inter: list | np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf])
+            inter: Sequence = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf])
     ) -> np.ndarray:
         """
         Get interval density.
 
         :param inter: Intervals
         :return: Interval density
         """
```

### Comparing `fastdfe-1.1.6/fastdfe/filtration.py` & `fastdfe-1.1.7/fastdfe/filtration.py`

 * *Files identical despite different names*

### Comparing `fastdfe-1.1.6/fastdfe/io_handlers.py` & `fastdfe-1.1.7/fastdfe/io_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import logging
 import os
 import shutil
 import tempfile
 import warnings
 from collections import Counter
 from functools import cached_property
-from typing import List, Iterable, TextIO, Dict, Optional, Tuple, Union
+from typing import List, Iterable, TextIO, Dict, Optional, Tuple, Union, Sequence
 from urllib.parse import urlparse
 
 import numpy as np
 import pandas as pd
 import requests
 from Bio import SeqIO
 from Bio.SeqIO.FastaIO import FastaIterator
@@ -33,15 +33,15 @@
 #: The DNA bases
 bases = ["A", "C", "G", "T"]
 
 # logger
 logger = logging.getLogger('fastdfe')
 
 
-def get_called_bases(genotypes: np.ndarray | List[str]) -> np.ndarray:
+def get_called_bases(genotypes: Sequence[str]) -> np.ndarray:
     """
     Get the called bases from a list of calls.
 
     :param genotypes: Array of genotypes in the form of strings.
     :return: Array of called bases.
     """
     # join genotypes
@@ -50,15 +50,15 @@
     # convert to numpy array of characters
     char_array = np.array(list(joined_genotypes))
 
     # return only characters that are in the bases list
     return char_array[np.isin(char_array, bases)]
 
 
-def get_major_base(genotypes: np.ndarray | List[str]) -> str | None:
+def get_major_base(genotypes: Sequence[str]) -> str | None:
     """
     Get the major base from a list of calls.
 
     :param genotypes: Array of genotypes in the form of strings.
     :return: Major base.
     """
     # get the called bases
@@ -534,15 +534,18 @@
     def remove_overlaps(df: pd.DataFrame) -> pd.DataFrame:
         """
         Remove overlapping coding sequences.
 
         :param df: The coding sequences.
         :return: The coding sequences without overlaps.
         """
-        df['overlap'] = df['start'].shift(-1) <= df['end']
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore", category=SettingWithCopyWarning)
+
+            df['overlap'] = df['start'].shift(-1) <= df['end']
 
         df = df[~df['overlap']]
 
         return df.drop(columns=['overlap'])
 
     @staticmethod
     def _add_lengths(cds: pd.DataFrame, remove_overlaps: bool = False, contigs: List[str] = None) -> pd.DataFrame:
```

### Comparing `fastdfe-1.1.6/fastdfe/joint_inference.py` & `fastdfe-1.1.7/fastdfe/joint_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,16 +70,16 @@
     """
 
     def __init__(
             self,
             sfs_neut: Spectra,
             sfs_sel: Spectra,
             include_divergence: bool = None,
-            intervals_del: (float, float, int) = (-1.0e+8, -1.0e-5, 1000),
-            intervals_ben: (float, float, int) = (1.0e-5, 1.0e4, 1000),
+            intervals_del: Tuple[float, float, int] = (-1.0e+8, -1.0e-5, 1000),
+            intervals_ben: Tuple[float, float, int] = (1.0e-5, 1.0e4, 1000),
             integration_mode: Literal['midpoint', 'quad'] = 'midpoint',
             linearized: bool = True,
             model: Parametrization | str = 'GammaExpParametrization',
             seed: int = 0,
             x0: Dict[str, Dict[str, float]] = {},
             bounds: Dict[str, Tuple[float, float]] = {},
             scales: Dict[str, Literal['lin', 'log', 'symlog']] = {},
```

### Comparing `fastdfe-1.1.6/fastdfe/json_handlers.py` & `fastdfe-1.1.7/fastdfe/json_handlers.py`

 * *Files identical despite different names*

### Comparing `fastdfe-1.1.6/fastdfe/likelihood.py` & `fastdfe-1.1.7/fastdfe/likelihood.py`

 * *Files identical despite different names*

### Comparing `fastdfe-1.1.6/fastdfe/optimization.py` & `fastdfe-1.1.7/fastdfe/optimization.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-02-26"
 
 import copy
 import logging
 import math
 from dataclasses import dataclass
-from typing import Callable, List, Dict, Literal, Tuple, Optional
+from typing import Callable, List, Dict, Literal, Tuple, Optional, Sequence
 
 import multiprocess as mp
 import numpy as np
 from numpy.linalg import norm
 from numpy.random import Generator
 from scipy.stats import loguniform, uniform
 from tqdm import tqdm
@@ -24,15 +24,15 @@
 
 # get logger
 logger = logging.getLogger('fastdfe').getChild('Optimization')
 
 
 def parallelize(
         func: Callable,
-        data: list | np.ndarray,
+        data: Sequence,
         parallelize: bool = True,
         pbar: bool = None,
         desc: str = None,
         dtype: type = object
 ) -> np.ndarray:
     """
     Parallelize given function or execute sequentially.
```

### Comparing `fastdfe-1.1.6/fastdfe/parametrization.py` & `fastdfe-1.1.7/fastdfe/parametrization.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-02-26"
 
 import logging
 from abc import abstractmethod, ABC
 from functools import wraps
-from typing import Callable, List, Union, Dict, Tuple, Literal
+from typing import Callable, List, Union, Dict, Tuple, Literal, Sequence
 
 import numpy as np
 from scipy.stats import gamma, expon
 
 # get logger
 logger = logging.getLogger('fastdfe')
 
@@ -158,15 +158,15 @@
         """
         # do nothing by default
         return params
 
     def plot(
             self,
             params: dict,
-            intervals: list | np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
+            intervals: Sequence = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             file: str = None,
             show: bool = True,
             title: str = 'discretized DFE',
             ax: 'plt.Axes' = None
 
     ) -> 'plt.Axes':
         """
@@ -592,40 +592,40 @@
     the number of parameters is larger than those of the other models, however. We generally also observe larger
     confidence intervals for this parametrization, and the optimization procedure may well be less efficient as
     we have to re-normalize the parameters to make sure they sum up to 1.
     """
 
     def __init__(
             self,
-            intervals: np.ndarray | list = np.array([-100000, -100, -10, -1, 0, 1, 1000])
+            intervals: Sequence = np.array([-100000, -100, -10, -1, 0, 1, 1000])
     ):
         """
         Constructor.
 
         :param intervals: The intervals of the discrete distribution.
         """
         super().__init__()
 
         #: Intervals
-        self.intervals = np.concatenate(([-np.inf], intervals, [np.inf]))
+        self.intervals: np.ndarray = np.concatenate(([-np.inf], intervals, [np.inf]))
 
         #: Interval sizes
-        self.interval_sizes = self.intervals[1:] - self.intervals[:-1]
+        self.interval_sizes: np.ndarray = self.intervals[1:] - self.intervals[:-1]
 
         #: Number of intervals, including the two infinite ones
-        self.k = self.intervals.shape[0] - 1
+        self.k: int = self.intervals.shape[0] - 1
 
         #: All parameter names, including the fixed ones
-        self.params = np.array([f"S{i}" for i in range(self.k)])
+        self.params: np.ndarray = np.array([f"S{i}" for i in range(self.k)])
 
         #: Parameter names that are not fixed
         self.param_names: List[str] = self.params[1:-1].tolist()
 
         #: Fixed parameters
-        self.fixed_params = {self.params[0]: 0, self.params[-1]: 0}
+        self.fixed_params: Dict[str, int] = {self.params[0]: 0, self.params[-1]: 0}
 
         #: Default initial parameters
         self.x0: Dict[str, float] = dict((p, 1 / (self.k - 2)) for p in self.param_names)
 
         #: Default parameter bounds
         self.bounds: Dict[str, Tuple[float, float]] = dict((p, (0, 1)) for p in self.param_names)
 
@@ -747,37 +747,37 @@
     the number of parameters is larger than those of the other models, however. It is more easily optimized than
     :class:`DiscreteParametrization` as it has one parameter less but its parameters are more difficult to interpret.
     One disadvantage with discrete parametrizations is that there may be `gaps` in the estimated DFE.
     """
 
     def __init__(
             self,
-            intervals: np.ndarray | list = np.array([-100000, -100, -10, -1, 0, 1, 1000])
+            intervals: Sequence = np.array([-100000, -100, -10, -1, 0, 1, 1000])
     ):
         """
         Constructor.
 
         :param intervals: The intervals of the discrete distribution.
         """
         super().__init__()
 
         #: Intervals
-        self.intervals = np.concatenate(([-np.inf], intervals, [np.inf]))
+        self.intervals: np.ndarray = np.concatenate(([-np.inf], intervals, [np.inf]))
 
         #: Interval sizes
-        self.interval_sizes = self.intervals[1:] - self.intervals[:-1]
+        self.interval_sizes: np.ndarray = self.intervals[1:] - self.intervals[:-1]
 
         #: Number of intervals, including the two infinite ones
-        self.k = self.intervals.shape[0] - 1
+        self.k: int = self.intervals.shape[0] - 1
 
         #: All parameter names, including fixed parameters
-        self.params = np.array([f"S{i}" for i in range(self.k)])
+        self.params: np.ndarray = np.array([f"S{i}" for i in range(self.k)])
 
         #: Parameter names that are not fixed
-        self.param_names = self.params[1:-2].tolist()
+        self.param_names: List[str] = self.params[1:-2].tolist()
 
         #: Fixed parameters
         self.fixed_params = {self.params[0]: 0, self.params[-2]: 1, self.params[-1]: 0}
 
         #: Default initial parameters
         self.x0: Dict[str, float] = self.to_fractional(dict((p, 1 / (self.k - 2)) for p in self.param_names))
```

### Comparing `fastdfe-1.1.6/fastdfe/parser.py` & `fastdfe-1.1.7/fastdfe/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 __date__ = "2023-03-26"
 
 import functools
 import itertools
 import logging
 from abc import ABC, abstractmethod
 from collections import Counter, defaultdict
-from scipy.stats import hypergeom
 from typing import List, Callable, Literal, Optional, Dict, Tuple
 
 import numpy as np
 from Bio.SeqRecord import SeqRecord
 from cyvcf2 import Variant
+from scipy.stats import hypergeom
 from tqdm import tqdm
 
 from .annotation import Annotation, SynonymyAnnotation, DegeneracyAnnotation, AncestralAlleleAnnotation
 from .filtration import Filtration, PolyAllelicFiltration, SNPFiltration
 from .io_handlers import bases, get_called_bases, FASTAHandler, NoTypeException, \
     DummyVariant, MultiHandler, VCFHandler, is_monomorphic_snp
 from .settings import Settings
@@ -883,15 +883,15 @@
             n: int,
             gff: str | None = None,
             fasta: str | None = None,
             info_ancestral: str = 'AA',
             skip_non_polarized: bool = True,
             stratifications: List[Stratification] = [],
             annotations: List[Annotation] = [],
-            filtrations: List[Filtration] = [PolyAllelicFiltration()],
+            filtrations: List[Filtration] = None,
             include_samples: List[str] = None,
             exclude_samples: List[str] = None,
             max_sites: int = np.inf,
             seed: int | None = 0,
             cache: bool = True,
             aliases: Dict[str, List[str]] = {},
             target_site_counter: TargetSiteCounter = None,
@@ -906,19 +906,20 @@
         :param fasta: The path to the FASTA file, possibly gzipped or a URL. This file is optional and depends on
             the annotations and filtrations that are used.
         :param n: The size of the resulting SFS. We down-sample to this number by drawing without replacement from
             the set of all available genotypes per site. Sites with fewer than ``n`` genotypes are skipped.
         :param info_ancestral: The tag in the INFO field that contains ancestral allele information. Consider using
             an ancestral allele annotation if this information is not available yet.
         :param skip_non_polarized: Whether to skip poly-morphic sites that are not polarized, i.e., without a valid
-            info tag providing the ancestral allele. If ``False``, we use the reference allele as ancestral allele (
-            only recommended if working with folded spectra).
+            info tag providing the ancestral allele. If ``False``, we use the reference allele as ancestral allele
+            (only recommended if working with folded spectra).
         :param stratifications: List of stratifications to use.
         :param annotations: List of annotations to use.
-        :param filtrations: List of filtrations to use.
+        :param filtrations: List of filtrations to use. By default, we use
+            :class:`~fastdfe.filtration.PolyAllelicFiltration`.
         :param include_samples: List of sample names to consider when determining the SFS. If ``None``, all samples
             are used. Note that this restriction does not apply to the annotations and filtrations.
         :param exclude_samples: List of sample names to exclude when determining the SFS. If ``None``, no samples
             are excluded. Note that this restriction does not apply to the annotations and filtrations.
         :param max_sites: Maximum number of sites to parse from the VCF file.
         :param seed: Seed for the random number generator. Use ``None`` for no seed.
         :param cache: Whether to cache files downloaded from URLs.
@@ -968,15 +969,15 @@
         #: List of stratifications to use
         self.stratifications: List[Stratification] = stratifications
 
         #: List of annotations to use
         self.annotations: List[Annotation] = annotations
 
         #: List of filtrations to use
-        self.filtrations: List[Filtration] = filtrations
+        self.filtrations: List[Filtration] = [PolyAllelicFiltration()] if filtrations is None else filtrations
 
         #: The number of sites that were skipped for various reasons
         self.n_skipped: int = 0
 
         #: The number of sites that were skipped because they had no valid ancestral allele
         self.n_no_ancestral: int = 0
 
@@ -1019,32 +1020,14 @@
         # we return the reference allele if valid
         if variant.REF in bases:
             return variant.REF
 
         # if the reference allele is not a valid base, we raise an error
         raise NoTypeException("Reference allele is not a valid base")
 
-    def _create_sfs_dictionary(self) -> Dict[str, np.ndarray]:
-        """
-        Create an SFS dictionary initialized with all possible base contexts.
-
-        :return: SFS dictionary
-        """
-        types = [s.get_types() for s in self.stratifications]
-
-        # define the DNA bases
-        contexts = ['.'.join(t) for t in itertools.product(*types)]
-
-        # create dict
-        sfs = {}
-        for context in contexts:
-            sfs[context] = np.zeros(self.n + 1)
-
-        return sfs
-
     def _parse_site(self, variant: Variant | DummyVariant) -> bool:
         """
         Parse a single site.
 
         :param variant: The variant.
         :return: Whether the site was included in the SFS.
         """
```

### Comparing `fastdfe-1.1.6/fastdfe/polydfe.py` & `fastdfe-1.1.7/fastdfe/polydfe.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 import subprocess
 import tempfile
 import time
 from typing import Callable, List, Optional, Literal, Dict
 
 import numpy as np
 import pandas as pd
-import rpy2.robjects as ro
-from rpy2.robjects.packages import importr
-from rpy2.robjects.vectors import ListVector
+
 from typing_extensions import Self
 
 from .abstract_inference import AbstractInference, Inference
 from .config import Config
 from .parametrization import _from_string, Parametrization, DiscreteParametrization
 from .polydfe_utils import create_sfs_config, models
 
@@ -75,14 +73,16 @@
 
     def parse_output(self) -> dict:
         """
         Parse output from polyDFE output file.
 
         :return: Dictionary of parsed data
         """
+        from rpy2.robjects.packages import importr
+
         # use the polyDFE R postprocessing script to parse the output file
         output = self.get_postprocessing_wrapper().parseOutput(self.output_file)[0]
 
         # convert to JSON
         rj = importr('RJSONIO')
         json_str = rj.toJSON(output)[0]
 
@@ -103,28 +103,30 @@
                 r=[data['values'][0][f"r {i}"] for i in range(2, data['n'])]
             ),
             n=data['n'],
             expec=data['expec'][0],
             alpha=self.get_alpha(output)
         )
 
-    def get_alpha(self, parsed_output: ListVector) -> float:
+    def get_alpha(self, parsed_output: 'rpy2.robjects.vectors.ListVector') -> float:
         """
         Get alpha, the proportion of beneficial non-synonymous substitutions.
 
         :return: Parsed output from polyDFE
         """
         return self.get_postprocessing_wrapper().estimateAlpha(parsed_output)[0]
 
-    def get_postprocessing_wrapper(self) -> ro.R:
+    def get_postprocessing_wrapper(self) -> 'ro.R':
         """
         Get the wrapped polyDFE postprocessing source.
 
         :return: R object
         """
+        import rpy2.robjects as ro
+
         ps = ro.r
         ps.source(self.postprocessing_source)
 
         return ps
 
     def to_json(self) -> str:
         """
```

### Comparing `fastdfe-1.1.6/fastdfe/polydfe_utils.py` & `fastdfe-1.1.7/fastdfe/polydfe_utils.py`

 * *Files identical despite different names*

### Comparing `fastdfe-1.1.6/fastdfe/spectrum.py` & `fastdfe-1.1.7/fastdfe/spectrum.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2022-07-24"
 
 import logging
 from functools import cached_property
-from typing import Dict, List, Union, Iterable, Any, Literal
+from typing import Dict, List, Union, Iterable, Any, Literal, Sequence
 
 import numpy as np
 import pandas as pd
 from scipy.stats import hypergeom
 
 from .io_handlers import download_if_url
 
@@ -26,30 +26,30 @@
 
     :param n: Standard Kingman SFS
     :return: Spectrum
     """
     return Spectrum(pad(1 / np.arange(1, int(n))))
 
 
-def pad(counts: list | np.ndarray) -> np.ndarray:
+def pad(counts: Sequence) -> np.ndarray:
     """
     Pad array with monomorphic counts.
 
     :param counts: SFS counts to pad
     :return: Padded array
     """
     return np.array([0] + list(counts) + [0])
 
 
 class Spectrum(Iterable):
     """
     Class for holding and manipulating a site-frequency spectrum.
     """
 
-    def __init__(self, data: list | np.ndarray):
+    def __init__(self, data: Sequence[float]):
         """
         Initialize spectrum.
 
         :param data: SFS counts
         """
         self.data: np.ndarray = np.array(data, dtype=float)
 
@@ -272,36 +272,36 @@
         Copy the spectrum.
 
         :return: Copy of the spectrum
         """
         return Spectrum(self.data.copy())
 
     @staticmethod
-    def from_polymorphic(data: list | np.ndarray) -> 'Spectrum':
+    def from_polymorphic(data: Sequence) -> 'Spectrum':
         """
         Create Spectrum from polymorphic counts only.
 
         :param data: Polymorphic counts
         :return: Spectrum
         """
         return Spectrum([0] + list(data) + [0])
 
     @staticmethod
-    def from_list(data: list | np.ndarray) -> 'Spectrum':
+    def from_list(data: Sequence) -> 'Spectrum':
         """
         Create Spectrum from list.
 
         :param data: SFS counts
         :return: Spectrum
         """
         return Spectrum(data)
 
     @staticmethod
     def from_polydfe(
-            polymorphic: list | np.ndarray,
+            polymorphic: Sequence,
             n_sites: float,
             n_div: float
     ) -> 'Spectrum':
         """
         Create Spectra from polyDFE specification which treats the number
         of mutational target sites and the divergence counts separately.
 
@@ -441,15 +441,15 @@
 
 
 class Spectra:
     """
     Class for holding and manipulating site-frequency spectra of multiple types.
     """
 
-    def __init__(self, data: Dict[str, list | np.ndarray]):
+    def __init__(self, data: Dict[str, Sequence]):
         """
         Initialize spectra.
 
         :param data: Dictionary of SFS counts keyed by type
         """
         self.data: pd.DataFrame = pd.DataFrame(data)
 
@@ -495,15 +495,15 @@
         The total number of polymorphic counts.
 
         :return: Total number of polymorphic counts for each type
         """
         return self.polymorphic.sum()
 
     @staticmethod
-    def from_list(data: list | np.ndarray, types: List) -> 'Spectra':
+    def from_list(data: Sequence, types: List) -> 'Spectra':
         """
         Create from array of spectra.
         Note that data.ndim needs to be 2.
 
         :param data: Array of spectra
         :param types: Types
         :return: Spectra
```

### Comparing `fastdfe-1.1.6/fastdfe/visualization.py` & `fastdfe-1.1.7/fastdfe/visualization.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-02-26"
 
 import functools
 import logging
-from typing import Callable, List, Literal, Dict
+from typing import Callable, List, Literal, Dict, Sequence
 
 import matplotlib.colors as mcolors
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from matplotlib import colors
@@ -132,17 +132,17 @@
 
         return bracket_left + format_number(left) + ', ' + format_number(right) + bracket_right
 
     @staticmethod
     @clear_show_save
     def plot_discretized(
             ax: plt.Axes,
-            values: list | np.ndarray,
-            errors: list | np.ndarray = None,
-            labels: list | np.ndarray = None,
+            values: Sequence,
+            errors: Sequence = None,
+            labels: Sequence = None,
             file: str = None,
             show: bool = True,
             intervals: np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             title: str = 'discretized DFE',
             interval_labels: List[str] = None,
             kwargs_legend: dict = dict(prop=dict(size=8)),
 
@@ -216,17 +216,17 @@
         return ax
 
     @staticmethod
     @clear_show_save
     def plot_continuous(
             ax: plt.Axes,
             bins: np.ndarray,
-            values: list | np.ndarray,
-            errors: list | np.ndarray = None,
-            labels: list | np.ndarray = None,
+            values: Sequence,
+            errors: Sequence = None,
+            labels: Sequence = None,
             file: str = None,
             show: bool = True,
             title: str = 'continuous DFE',
             scale: Literal['log', 'linear'] = 'lin',
             ylim: float = 1e-2,
             scale_density: bool = False,
             kwargs_legend: dict = dict(prop=dict(size=8)),
@@ -315,16 +315,16 @@
 
         ax.set_xticks(ticks)
         ax.set_xticklabels(ticks_new)
 
     @staticmethod
     def name_to_label(
             key: str,
-            param_names: list | np.ndarray = None,
-            vals: list | np.ndarray = None
+            param_names: Sequence = None,
+            vals: Sequence = None
     ) -> str:
         """
         Map parameter name to label.
 
         :param key: Parameter name
         :param param_names: Parameter names
         :param vals: Parameter values
@@ -353,16 +353,16 @@
         return '$-' + key + '$'
 
     @staticmethod
     @clear_show_save
     def plot_inferred_parameters(
             ax: plt.Axes,
             values: Dict[str, np.ndarray],
-            labels: list | np.ndarray,
-            param_names: list | np.ndarray,
+            labels: Sequence,
+            param_names: Sequence,
             errors: Dict[str, np.ndarray | None],
             file: str = None,
             show: bool = True,
             title: str = 'parameter estimates',
             legend: bool = True,
             scale: Literal['lin', 'log', 'symlog'] = 'log',
             kwargs_legend: dict = dict(prop=dict(size=8), loc='upper right')
@@ -445,15 +445,15 @@
         ax.autoscale(tight=True, axis='x')
 
         return ax
 
     @staticmethod
     def plot_inferred_parameters_boxplot(
             values: Dict[str, pd.DataFrame],
-            param_names: list | np.ndarray,
+            param_names: Sequence,
             file: str = None,
             show: bool = True,
             title: str = 'parameter estimates'
     ) -> plt.Axes:
         """
         Visualize the inferred parameters using a boxplot.
 
@@ -768,15 +768,15 @@
         ax.margins(x=0)
 
         return ax
 
     @staticmethod
     @clear_show_save
     def plot_scatter(
-            values: list | np.ndarray,
+            values: Sequence,
             file: str,
             show: bool,
             ax: plt.Axes,
             title: str | None = None,
             scale: Literal['lin', 'log', 'symlog'] = 'lin',
             ylabel: str = 'lnl'
     ) -> plt.Axes:
@@ -805,16 +805,16 @@
 
         return ax
 
     @staticmethod
     @clear_show_save
     def plot_buckets_sizes(
             n_intervals: int,
-            bins: list | np.ndarray,
-            sizes: list | np.ndarray,
+            bins: Sequence,
+            sizes: Sequence,
             title: str,
             file: str,
             show: bool,
             ax: plt.Axes
     ) -> plt.Axes:
         """
         A line plot of the bucket sizes.
@@ -843,16 +843,16 @@
 
         return ax
 
     @staticmethod
     @clear_show_save
     def plot_nested_models(
             P: np.ndarray,
-            labels_x: list | np.ndarray,
-            labels_y: list | np.ndarray,
+            labels_x: Sequence,
+            labels_y: Sequence,
             ax: plt.Axes,
             file: str = None,
             show: bool = True,
             cmap: str = None,
             title: str = None,
             vmin: float = 1e-10,
             vmax: float = 1,
@@ -937,15 +937,15 @@
         return ax
 
     @staticmethod
     @clear_show_save
     def plot_interval_density(
             ax: plt.Axes,
             density: np.ndarray,
-            intervals: list | np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
+            intervals: Sequence = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             interval_labels: List[str] = None,
             file: str = None,
             show: bool = True,
             color: str = 'C0',
     ) -> plt.Axes:
         """
         Plot density of the discretization intervals chosen.
@@ -988,20 +988,20 @@
         ax.autoscale(tight=True, axis='x')
 
         return ax
 
     @staticmethod
     @clear_show_save
     def plot_covariate(
-            covariates: list | np.ndarray,
-            values: list | np.ndarray,
+            covariates: Sequence,
+            values: Sequence,
             xlabel: str,
             ylabel: str,
-            labels: list | np.ndarray = None,
-            errors: list | np.ndarray = None,
+            labels: Sequence = None,
+            errors: Sequence = None,
             file: str = None,
             show: bool = True,
             title: str = 'likelihoods',
             ax: plt.Axes = None
     ) -> plt.Axes:
         """
```

### Comparing `fastdfe-1.1.6/pyproject.toml` & `fastdfe-1.1.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastdfe"
-version = "1.1.6"
+version = "1.1.7"
 description = "Fast and flexible inference of the distribution of fitness effects (DFE), VCF-SFS parsing with ancestral allele and site-degeneracy annotation."
 authors = ["Sendrowski <sendrowski.janek@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10.0,<3.13"
@@ -21,18 +21,18 @@
 mpmath = "^1.3.0"
 biopython = ">=1.80,<1.82"
 requests = ">=2.28"
 scipy = "^1.10.1"
 
 [tool.poetry.group.dev.dependencies]
 urllib3 = "^1.26.0" # problems with poetry and urllib3 version 2
-sphinx-rtd-theme = "^1.2.0"
-sphinx-autodoc-typehints = "^1.23.0"
+sphinx_book_theme = "^1.1.2"
+sphinx-autodoc-typehints = "^2.1.0"
 sphinx-copybutton = "^0.5.2"
-myst-nb = "^0.17.2"
-sphinx = "5.3.0"
+myst-nb = "^1.1.0"
+sphinx = "^7.3.7"
 pygments = "^2.15.1"
-sphinxcontrib-bibtex = "^2.5.0"
+sphinxcontrib-bibtex = "^2.6.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fastdfe-1.1.6/PKG-INFO` & `fastdfe-1.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastdfe
-Version: 1.1.6
+Version: 1.1.7
 Summary: Fast and flexible inference of the distribution of fitness effects (DFE), VCF-SFS parsing with ancestral allele and site-degeneracy annotation.
 License: MIT
 Author: Sendrowski
 Author-email: sendrowski.janek@gmail.com
 Requires-Python: >=3.10.0,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -28,14 +28,15 @@
 Description-Content-Type: text/markdown
 
 # fastDFE  <img align="right" width="100" src="https://raw.githubusercontent.com/Sendrowski/fastDFE/master/docs/logo.png">
 [![tests](https://github.com/Sendrowski/fastDFE/actions/workflows/run-tests.yml/badge.svg?branch=master)](https://github.com/Sendrowski/fastDFE/actions/workflows/run-tests.yml)
 [![codecov](https://codecov.io/gh/Sendrowski/fastDFE/branch/master/graph/badge.svg?token=0LUE8SZYBJ)](https://codecov.io/gh/Sendrowski/fastDFE)
 [![Documentation Status](https://readthedocs.org/projects/fastdfe/badge/?version=latest)](https://fastdfe.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/fastdfe.svg)](https://badge.fury.io/py/fastdfe)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![Downloads](https://static.pepy.tech/badge/fastdfe)](https://pepy.tech/project/fastdfe)
 [![DOI](https://img.shields.io/badge/DOI-10.1093/molbev/msae070-blue)](https://doi.org/10.1093/molbev/msae070)
 
-
 ``fastdfe`` is a package for fast, flexible, and hierarchical inference of the distribution of fitness effects (DFE) from site frequency spectra (SFS). It also contains a versatile VCF-to-SFS parser with support for ancestral allele and site-degeneracy annotation.
 
 Please see the [documentation](https://fastdfe.readthedocs.io/en/latest/) for all the details.
```

