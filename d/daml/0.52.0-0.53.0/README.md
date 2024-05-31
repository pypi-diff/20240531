# Comparing `tmp/daml-0.52.0.tar.gz` & `tmp/daml-0.53.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daml-0.52.0.tar", max compression
+gzip compressed data, was "daml-0.53.0.tar", max compression
```

## Comparing `daml-0.52.0.tar` & `daml-0.53.0.tar`

### file list

```diff
@@ -1,49 +1,48 @@
--rw-r--r--   0        0        0     1060 2024-05-10 03:05:41.196777 daml-0.52.0/LICENSE.txt
--rw-r--r--   0        0        0     2528 2024-05-10 03:05:41.196777 daml-0.52.0/README.md
--rw-r--r--   0        0        0     5170 2024-05-10 03:05:55.524837 daml-0.52.0/pyproject.toml
--rw-r--r--   0        0        0      230 2024-05-10 03:05:55.528838 daml-0.52.0/src/daml/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/__init__.py
--rw-r--r--   0        0        0     2412 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/base.py
--rw-r--r--   0        0        0     2912 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/ber.py
--rw-r--r--   0        0        0     2819 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/divergence.py
--rw-r--r--   0        0        0        0 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/drift/__init__.py
--rw-r--r--   0        0        0     8981 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/drift/base.py
--rw-r--r--   0        0        0     3897 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/drift/cvm.py
--rw-r--r--   0        0        0     3924 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/drift/ks.py
--rw-r--r--   0        0        0     6965 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/drift/mmd.py
--rw-r--r--   0        0        0    10866 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/drift/torch.py
--rw-r--r--   0        0        0     5263 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/drift/uncertainty.py
--rw-r--r--   0        0        0        0 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/outlier/__init__.py
--rw-r--r--   0        0        0     2596 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/outlier/ae.py
--rw-r--r--   0        0        0     2364 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/outlier/aegmm.py
--rw-r--r--   0        0        0     6831 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/outlier/base.py
--rw-r--r--   0        0        0    10089 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/outlier/llr.py
--rw-r--r--   0        0        0     2920 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/outlier/vae.py
--rw-r--r--   0        0        0     2790 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/outlier/vaegmm.py
--rw-r--r--   0        0        0    13549 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/sufficiency.py
--rw-r--r--   0        0        0     1145 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/uap.py
--rw-r--r--   0        0        0     2316 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/utils.py
--rw-r--r--   0        0        0        0 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/models/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/models/pytorch/__init__.py
--rw-r--r--   0        0        0     6123 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/models/pytorch/autoencoder.py
--rw-r--r--   0        0        0     1354 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/models/pytorch/blocks.py
--rw-r--r--   0        0        0     1675 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/models/pytorch/utils.py
--rw-r--r--   0        0        0        0 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/models/tensorflow/__init__.py
--rw-r--r--   0        0        0    10008 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/models/tensorflow/autoencoder.py
--rw-r--r--   0        0        0     3640 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/models/tensorflow/gmm.py
--rw-r--r--   0        0        0     3776 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/models/tensorflow/losses.py
--rw-r--r--   0        0        0    48091 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/models/tensorflow/pixelcnn.py
--rw-r--r--   0        0        0     4113 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/models/tensorflow/trainer.py
--rw-r--r--   0        0        0     8613 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/models/tensorflow/utils.py
--rw-r--r--   0        0        0      856 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_prototype/README.md
--rw-r--r--   0        0        0     7273 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_prototype/cleaning.py
--rw-r--r--   0        0        0    21662 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_prototype/linting.py
--rw-r--r--   0        0        0    22416 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_prototype/test_linting.ipynb
--rw-r--r--   0        0        0      594 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/metrics/__init__.py
--rw-r--r--   0        0        0      678 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/metrics/drift/__init__.py
--rw-r--r--   0        0        0      488 2024-05-10 03:05:41.208778 daml-0.52.0/src/daml/metrics/outlier/__init__.py
--rw-r--r--   0        0        0      293 2024-05-10 03:05:41.208778 daml-0.52.0/src/daml/models/__init__.py
--rw-r--r--   0        0        0      408 2024-05-10 03:05:41.208778 daml-0.52.0/src/daml/models/tensorflow/__init__.py
--rw-r--r--   0        0        0      186 2024-05-10 03:05:41.208778 daml-0.52.0/src/daml/models/torch/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 03:05:41.208778 daml-0.52.0/src/daml/py.typed
--rw-r--r--   0        0        0     5034 1970-01-01 00:00:00.000000 daml-0.52.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-31 03:06:00.390164 daml-0.53.0/LICENSE.txt
+-rw-r--r--   0        0        0     2365 2024-05-31 03:06:00.390164 daml-0.53.0/README.md
+-rw-r--r--   0        0        0     5405 2024-05-31 03:06:05.522187 daml-0.53.0/pyproject.toml
+-rw-r--r--   0        0        0      230 2024-05-31 03:06:05.522187 daml-0.53.0/src/daml/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/metrics/__init__.py
+-rw-r--r--   0        0        0     2412 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/metrics/base.py
+-rw-r--r--   0        0        0     3847 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/metrics/ber.py
+-rw-r--r--   0        0        0     2819 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/metrics/divergence.py
+-rw-r--r--   0        0        0        0 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/metrics/drift/__init__.py
+-rw-r--r--   0        0        0     8981 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/metrics/drift/base.py
+-rw-r--r--   0        0        0     3897 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/metrics/drift/cvm.py
+-rw-r--r--   0        0        0     3924 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/metrics/drift/ks.py
+-rw-r--r--   0        0        0     6965 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/metrics/drift/mmd.py
+-rw-r--r--   0        0        0    10866 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/metrics/drift/torch.py
+-rw-r--r--   0        0        0     5263 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/metrics/drift/uncertainty.py
+-rw-r--r--   0        0        0     2778 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/metrics/hash.py
+-rw-r--r--   0        0        0        0 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/metrics/outlier/__init__.py
+-rw-r--r--   0        0        0     2596 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/metrics/outlier/ae.py
+-rw-r--r--   0        0        0     2364 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/metrics/outlier/aegmm.py
+-rw-r--r--   0        0        0     6832 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/metrics/outlier/base.py
+-rw-r--r--   0        0        0    10089 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/metrics/outlier/llr.py
+-rw-r--r--   0        0        0     2920 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/metrics/outlier/vae.py
+-rw-r--r--   0        0        0     2790 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/metrics/outlier/vaegmm.py
+-rw-r--r--   0        0        0     7319 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/metrics/stats.py
+-rw-r--r--   0        0        0    18122 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/metrics/sufficiency.py
+-rw-r--r--   0        0        0     1145 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/metrics/uap.py
+-rw-r--r--   0        0        0     2327 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/metrics/utils.py
+-rw-r--r--   0        0        0        0 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/models/pytorch/__init__.py
+-rw-r--r--   0        0        0     6123 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/models/pytorch/autoencoder.py
+-rw-r--r--   0        0        0     1354 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/models/pytorch/blocks.py
+-rw-r--r--   0        0        0     1675 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/models/pytorch/utils.py
+-rw-r--r--   0        0        0        0 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/models/tensorflow/__init__.py
+-rw-r--r--   0        0        0    10008 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/models/tensorflow/autoencoder.py
+-rw-r--r--   0        0        0     3640 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/models/tensorflow/gmm.py
+-rw-r--r--   0        0        0     3776 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/models/tensorflow/losses.py
+-rw-r--r--   0        0        0    48091 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/models/tensorflow/pixelcnn.py
+-rw-r--r--   0        0        0     4113 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/models/tensorflow/trainer.py
+-rw-r--r--   0        0        0     8613 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/_internal/models/tensorflow/utils.py
+-rw-r--r--   0        0        0      594 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/metrics/__init__.py
+-rw-r--r--   0        0        0      678 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/metrics/drift/__init__.py
+-rw-r--r--   0        0        0      488 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/metrics/outlier/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/metrics/sufficiency/__init__.py
+-rw-r--r--   0        0        0      293 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/models/__init__.py
+-rw-r--r--   0        0        0      408 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/models/tensorflow/__init__.py
+-rw-r--r--   0        0        0      186 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/models/torch/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 03:06:00.402164 daml-0.53.0/src/daml/py.typed
+-rw-r--r--   0        0        0     4968 1970-01-01 00:00:00.000000 daml-0.53.0/PKG-INFO
```

### Comparing `daml-0.52.0/LICENSE.txt` & `daml-0.53.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/README.md` & `daml-0.53.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -49,20 +49,15 @@
 cd daml
 ```
 
 
 
 Install DAML with optional dependencies for development.
 ```
-poetry install --all-extras --with test,lint
-```
-
-Alternatively, you can install with optional dependencies used to generate documentation as well.
-```
-poetry install --all-extras --with test,lint,docs
+poetry install --all-extras --with dev
 ```
 
 Now that DAML is installed, you can run commands in the poetry virtual environment by prefixing shell commands with `poetry run`, or activate the virtual environment directly in the shell.
 ```
 poetry shell
 ```
```

### Comparing `daml-0.52.0/pyproject.toml` & `daml-0.53.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "daml"
-version = "0.52.0" # dynamic
+version = "0.53.0" # dynamic
 description = "DAML provides a simple interface to characterize image data and its impact on model performance across classification and object-detection tasks"
 license = "MIT"
 readme = "README.md"
 homepage = "https://daml.ai/"
 repository = "https://github.com/aria-ml/daml/"
 documentation = "https://daml.readthedocs.io/"
 
@@ -28,19 +28,25 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Scientific/Engineering",
 ]
 
+packages = [
+  {include = "daml", from = "src"}
+]
+
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
+hdbscan = {version = ">=0.8.36"}
 matplotlib = {version = "*", optional = true}
-numpy = ">=1.24.2, <2"
+numpy = {version = ">=1.24.2, <2"}
 nvidia-cudnn-cu11 = {version = ">=8.6.0.163", optional = true}
+pillow = {version = ">=10.3.0"}
 scipy = {version = ">=1.10" }
 scikit-learn = {version = ">=1.2.1" }
 tensorflow = [
   {version = "~2.13.1", python = "~3.8.1", optional = true},
   {version = ">=2.14.1,<2.16", python = ">=3.9,<3.12", optional = true},
 ]
 tensorflow-io-gcs-filesystem = [
@@ -48,62 +54,56 @@
   {version = ">=0.35.0,<0.37", python = ">=3.9,<3.12", optional = true},
 ]
 tensorflow_probability = [
   {version = "~0.21.0", python = "~3.8.1", optional = true},
   {version = ">=0.22.1,<0.24", python = ">=3.9,<3.12", optional = true},
 ]
 torch = {version = ">=2.0.1, !=2.2.0", source = "pytorch", optional = true}
+xxhash = {version = ">=3.3"}
 
 [tool.poetry.extras]
 torch = ["torch", "matplotlib", "nvidia-cudnn-cu11"]
 tensorflow = ["tensorflow", "tensorflow-io-gcs-filesystem", "tensorflow-probability", "nvidia-cudnn-cu11"]
 all = ["torch", "matplotlib", "nvidia-cudnn-cu11", "tensorflow", "tensorflow-io-gcs-filesystem", "tensorflow-probability", "nvidia-cudnn-cu11"]
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 ruff = "*"
 codespell = "*"
 
-[tool.poetry.group.test]
+[tool.poetry.group.dev]
 optional = true
 
-[tool.poetry.group.test.dependencies]
-pytest = "*"
-coverage = "*"
+[tool.poetry.group.dev.dependencies]
+# lint
+ruff = {version = "*"}
+codespell = {version = "*"}
+# test
+pytest = {version = "*"}
+pytest-cov = {version = "*"}
+pytest-xdist = {version = "*"}
+coverage = {version = "*", extras = ["toml"]}
 pyright = {version = "*, !=1.1.340"}
 torchmetrics = {version = ">=1.0.0", source = "pytorch"}
 matplotlib = {version = "*"}
-
-[tool.poetry.group.docs]
-optional = true
-
-[tool.poetry.group.docs.dependencies]
+# docs
 ipykernel = {version = "6.26.0", python = ">=3.9,<3.12"}
 ipywidgets = {version = "8.1.1", python = ">=3.9,<3.12"}
 jupyter-client = {version = "8.6.0", python = ">=3.9,<3.12"}
 jupyter-cache = {version = "*", python = ">=3.9,<3.12"}
 myst-nb = {version = "1.0.0", python = ">=3.9,<3.12"} 
 sphinx-rtd-size = {version = "0.2.0", python = ">=3.9,<3.12"}
 sphinx-rtd-theme = {version = "1.3.0", python = ">=3.9,<3.12"}
 sphinx-design = {version = "*", python = ">=3.9,<3.12"}
 sphinx-tabs = {version = "*", python = ">=3.9,<3.12"}
 Sphinx = {version = "7.2.6", python = ">=3.9,<3.12"}
 tensorflow-datasets = {version = "*", python = ">=3.9,<3.12"}
 torchvision = {version = ">=0.16.0", source = "pytorch", python = ">=3.9,<3.12"}
-torchmetrics = {version = ">=1.0.0", source = "pytorch", python = ">=3.9,<3.12"}
-matplotlib = {version = "*", python = ">=3.9,<3.12"}
-pytest = {version = "*", python = ">=3.9,<3.12"}
-
-[tool.poetry.group.jatic]
-optional = true
-
-[tool.poetry.group.jatic.dependencies]
-maite = {version = "*"}
 
 [[tool.poetry.source]]
 name = "pytorch"
 url = "https://download.pytorch.org/whl/cu118"
 priority = "explicit"
 
 [tool.poetry-dynamic-versioning]
@@ -115,18 +115,32 @@
 [tool.poetry-dynamic-versioning.substitution]
 files = ["src/daml/__init__.py"]
 
 [tool.pyright]
 reportMissingImports = false
 
 [tool.pytest.ini_options]
-markers = [
-  "interop: marks external library interop tests",
-  "functional: marks slower functional tests",
+norecursedirs = ["prototype"]
+addopts = ["--pythonwarnings=ignore::DeprecationWarning", "--verbose", "--durations=20", "--durations-min=1.0"]
+
+[tool.coverage.run]
+source = ["daml"]
+branch = true
+
+[tool.coverage.report]
+exclude_also = [
+    "raise NotImplementedError"
+]
+omit = [
+  "*/_internal/models/tensorflow/pixelcnn.py",
+  "*/_prototype/*",
+  "/tmp/*",
+  "tests/*"
 ]
+fail_under = 90
 
 # Ruff rules - https://docs.astral.sh/ruff/rules/
 [tool.ruff]
 exclude = [
   ".devcontainer",
   ".github",
   ".vscode",
```

### Comparing `daml-0.52.0/src/daml/_internal/metrics/base.py` & `daml-0.53.0/src/daml/_internal/metrics/base.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/src/daml/_internal/metrics/ber.py` & `daml-0.53.0/src/daml/_internal/metrics/ber.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,74 +7,95 @@
 https://arxiv.org/abs/1811.06419
 """
 
 from typing import Callable, Dict, Literal, Tuple
 
 import numpy as np
 from scipy.sparse import coo_matrix
+from scipy.stats import mode
 
 from daml._internal.metrics.base import EvaluateMixin, MethodsMixin
 
 from .utils import compute_neighbors, get_classes_counts, minimum_spanning_tree
 
 
-def _mst(X: np.ndarray, y: np.ndarray) -> Tuple[float, float]:
+def _mst(X: np.ndarray, y: np.ndarray, _: int) -> Tuple[float, float]:
     M, N = get_classes_counts(y)
 
     tree = coo_matrix(minimum_spanning_tree(X))
     matches = np.sum([y[tree.row[i]] != y[tree.col[i]] for i in range(N - 1)])
     deltas = matches / (2 * N)
     upper = 2 * deltas
-    lower = ((M - 1) / (M)) * (1 - (1 - 2 * ((M) / (M - 1)) * deltas) ** 0.5)
+    lower = ((M - 1) / (M)) * (1 - max(1 - 2 * ((M) / (M - 1)) * deltas, 0) ** 0.5)
     return upper, lower
 
 
-def _knn(X: np.ndarray, y: np.ndarray) -> Tuple[float, float]:
+def _knn(X: np.ndarray, y: np.ndarray, k: int) -> Tuple[float, float]:
     M, N = get_classes_counts(y)
 
     # All features belong on second dimension
     X = X.reshape((X.shape[0], -1))
-    nn_indices = compute_neighbors(X, X)
-    deltas = float(np.count_nonzero(y[nn_indices] - y) / (2 * N))
-    upper = 2 * deltas
-    lower = ((M - 1) / (M)) * (1 - (1 - 2 * ((M) / (M - 1)) * deltas) ** 0.5)
+    nn_indices = compute_neighbors(X, X, k=k)
+    nn_indices = np.expand_dims(nn_indices, axis=1) if nn_indices.ndim == 1 else nn_indices
+    modal_class = mode(y[nn_indices], axis=1).mode.squeeze()
+    upper = float(np.count_nonzero(modal_class - y) / N)
+    lower = _knn_lowerbound(upper, M, k)
     return upper, lower
 
 
+def _knn_lowerbound(value: float, classes: int, k: int) -> float:
+    "Several cases for computing the BER lower bound"
+    if value <= 1e-10:
+        return 0.0
+
+    if classes == 2 and k != 1:
+        if k > 5:
+            # Property 2 (Devroye, 1981) cited in Snoopy paper, not in snoopy repo
+            alpha = 0.3399
+            beta = 0.9749
+            a_k = alpha * np.sqrt(k) / (k - 3.25) * (1 + beta / (np.sqrt(k - 3)))
+            return value / (1 + a_k)
+        if k > 2:
+            return value / (1 + (1 / np.sqrt(k)))
+        # k == 2:
+        return value / 2
+
+    return ((classes - 1) / classes) * (1 - np.sqrt(max(0, 1 - ((classes / (classes - 1)) * value))))
+
+
 _METHODS = Literal["MST", "KNN"]
-_FUNCTION = Callable[[np.ndarray, np.ndarray], Tuple[float, float]]
+_FUNCTION = Callable[[np.ndarray, np.ndarray, int], Tuple[float, float]]
 
 
 class BER(EvaluateMixin, MethodsMixin[_METHODS, _FUNCTION]):
     """
     An estimator for Multi-class Bayes Error Rate using FR or KNN test statistic basis
 
     Parameters
     ----------
     data : np.ndarray
         Array of images or image embeddings
     labels : np.ndarray
         Array of labels for each image or image embedding
-    method : Literal["MST", "KNN"], default "MST"
+    method : Literal["MST", "KNN"], default "KNN"
         Method to use when estimating the Bayes error rate
+    k : int, default 1
+        number of nearest neighbors for KNN estimator -- ignored by MST estimator
+
 
     See Also
     --------
     `Learning to Bound the Multi-class Bayes Error (Th. 3 and Th. 4) <https://arxiv.org/abs/1811.06419>`_
 
     """
 
-    def __init__(
-        self,
-        data: np.ndarray,
-        labels: np.ndarray,
-        method: _METHODS = "MST",
-    ) -> None:
+    def __init__(self, data: np.ndarray, labels: np.ndarray, method: _METHODS = "KNN", k: int = 1) -> None:
         self.data = data
         self.labels = labels
+        self.k = k
         self._set_method(method)
 
     @classmethod
     def _methods(
         cls,
     ) -> Dict[str, _FUNCTION]:
         return {"MST": _mst, "KNN": _knn}
@@ -92,9 +113,9 @@
                 The estimated upper bounds of the Bayes Error Rate
 
         Raises
         ------
         ValueError
             If unique classes M < 2
         """
-        upper, lower = self._method(self.data, self.labels)
+        upper, lower = self._method(self.data, self.labels, self.k)
         return {"ber": upper, "ber_lower": lower}
```

### Comparing `daml-0.52.0/src/daml/_internal/metrics/divergence.py` & `daml-0.53.0/src/daml/_internal/metrics/divergence.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/src/daml/_internal/metrics/drift/base.py` & `daml-0.53.0/src/daml/_internal/metrics/drift/base.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/src/daml/_internal/metrics/drift/cvm.py` & `daml-0.53.0/src/daml/_internal/metrics/drift/cvm.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/src/daml/_internal/metrics/drift/ks.py` & `daml-0.53.0/src/daml/_internal/metrics/drift/ks.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/src/daml/_internal/metrics/drift/mmd.py` & `daml-0.53.0/src/daml/_internal/metrics/drift/mmd.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/src/daml/_internal/metrics/drift/torch.py` & `daml-0.53.0/src/daml/_internal/metrics/drift/torch.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/src/daml/_internal/metrics/drift/uncertainty.py` & `daml-0.53.0/src/daml/_internal/metrics/drift/uncertainty.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/src/daml/_internal/metrics/outlier/ae.py` & `daml-0.53.0/src/daml/_internal/metrics/outlier/ae.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/src/daml/_internal/metrics/outlier/aegmm.py` & `daml-0.53.0/src/daml/_internal/metrics/outlier/aegmm.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/src/daml/_internal/metrics/outlier/base.py` & `daml-0.53.0/src/daml/_internal/metrics/outlier/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     Parameters
     ----------
     instance_score : np.ndarray
         Instance score of the evaluated dataset.
     feature_score : Optional[np.ndarray], default None
         Feature score, if available, of the evaluated dataset.
     """
+
     instance_score: np.ndarray
     feature_score: Optional[np.ndarray] = None
 
     def get(self, outlier_type: Literal["instance", "feature"]) -> np.ndarray:
         return self.instance_score if outlier_type == "instance" or self.feature_score is None else self.feature_score
```

### Comparing `daml-0.52.0/src/daml/_internal/metrics/outlier/llr.py` & `daml-0.53.0/src/daml/_internal/metrics/outlier/llr.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/src/daml/_internal/metrics/outlier/vae.py` & `daml-0.53.0/src/daml/_internal/metrics/outlier/vae.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/src/daml/_internal/metrics/outlier/vaegmm.py` & `daml-0.53.0/src/daml/_internal/metrics/outlier/vaegmm.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/src/daml/_internal/metrics/sufficiency.py` & `daml-0.53.0/src/daml/_internal/metrics/sufficiency.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, Dict, List, Optional, Sequence, Union, cast
+from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union, cast
 
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
 import torch.nn as nn
 from matplotlib.figure import Figure
 from scipy.optimize import basinhopping
@@ -28,38 +28,60 @@
     -------
     np.ndarray
         Data points for the line of best fit
     """
     return x[0] * n_i ** (-x[1]) + x[2]
 
 
-def calc_params(p_i: np.ndarray, n_i: np.ndarray) -> np.ndarray:
+def f_inv_out(y_i: np.ndarray, x: np.ndarray) -> np.ndarray:
+    """
+    Inverse function for f_out()
+
+    Parameters
+    ----------
+    y_i : np.ndarray
+        Data points for the line of best fit
+    x : np.ndarray
+        Array of inverse power curve coefficients
+
+    Returns
+    -------
+    np.ndarray
+        Array of sample sizes
+    """
+    n_i = ((y_i - x[2]) / x[0]) ** (-1 / x[1])
+    return n_i
+
+
+def calc_params(p_i: np.ndarray, n_i: np.ndarray, niter: int) -> np.ndarray:
     """
     Retrieves the inverse power curve coefficients for the line of best fit.
     Global minimization is done via basin hopping. More info on this algorithm
     can be found here: https://arxiv.org/abs/cond-mat/9803344 .
 
     Parameters
     ----------
     p_i : np.ndarray
         Array of corresponding losses
     n_i : np.ndarray
         Array of sample sizes
+    niter : int
+        Number of iterations to perform in the basin-hopping
+        numerical process to curve-fit p_i
 
     Returns
     -------
     np.ndarray
         Array of parameters to recreate line of best fit
     """
 
     def f(x):
-        inner = np.sum(np.square(p_i - x[0] * n_i ** (-x[1]) - x[2]))
-        return inner
+        return np.sum(np.square(p_i - x[0] * n_i ** (-x[1]) - x[2]))
 
-    res = basinhopping(f, np.array([0.5, 0.5, 0.1]))
+    res = basinhopping(f, np.array([0.5, 0.5, 0.1]), niter=niter)
     return res.x
 
 
 def reset_parameters(model: nn.Module):
     """
     Re-initializes each layer in the model using
     the layer's defined weight_init function
@@ -98,28 +120,72 @@
             raise ValueError("f{m} does not contain the expected number ({c}) of data points.")
 
 
 def project_steps(
     measure: np.ndarray,
     steps: np.ndarray,
     projection: np.ndarray,
-) -> np.ndarray:
+    niter: int = 1000,
+) -> Tuple[np.ndarray, np.ndarray]:
     """Projects the measures for each value of X
 
     Parameters
     ----------
     measure : np.ndarray
         Measures from which to extrapolate projection
     steps : np.ndarray
         Steps of the taken measures
     projection : np.ndarray
         Steps to extrapolate
+    niter : int, default 1000
+        Number of iterations to perform in the basin-hopping
+        numerical process to curve-fit measure
+
+    Returns
+    -------
+    np.ndarray
+        Extrapolated measure values at each projection step
+    np.ndarray
+        length-3 array of the parameters for the fit curve.
+
     """
-    params = calc_params(p_i=(1 - measure), n_i=steps)
-    return 1 - f_out(projection, params)
+    params = calc_params(p_i=(1 - measure), n_i=steps, niter=niter)
+    projected_steps = 1 - f_out(projection, params)
+    return projected_steps, params
+
+
+def inv_project_steps(
+    measure: np.ndarray,
+    steps: np.ndarray,
+    accuracies: np.ndarray,
+    params: np.ndarray = np.zeros(0),
+) -> np.ndarray:
+    """Inverse function for project_steps()
+
+    Parameters
+    ----------
+    measure : np.ndarray
+        Measures from which to extrapolate projection
+    steps : np.ndarray
+        Steps of the taken measures
+    accuracies : np.ndarray
+        Desired accuracy values
+    params : np.ndarray, default np.zeros(0)
+        length-3 array of the parameters for the sufficiency curve to study.
+        If not provided, we curve-fit the parameters at runtime. Curve-fitting
+        is very slow, and we recommend pre-computing the parameters.
+
+    Returns
+    -------
+    np.ndarray
+        Array of sample sizes
+    """
+    if len(params) == 0:
+        params = calc_params(p_i=(1 - measure), n_i=steps, niter=1000)
+    return f_inv_out(1 - np.array(accuracies), params)
 
 
 def plot_measure(
     name: str,
     steps: np.ndarray,
     measure: np.ndarray,
     projection: np.ndarray,
@@ -136,15 +202,15 @@
 
     # Plot measure over each step
     ax.scatter(steps, measure, label=f"Model Results ({name})", s=15, c="black")
 
     # Plot extrapolation
     ax.plot(
         projection,
-        project_steps(measure, steps, projection),
+        project_steps(measure, steps, projection)[0],
         linestyle="dashed",
         label=f"Potential Model Results ({name})",
     )
 
     ax.legend()
     return fig
 
@@ -166,17 +232,17 @@
         (torch.utils.data.Dataset), indices to train on and executes model
         training against the data.
     eval_fn : Callable[[nn.Module, Dataset], Dict[str, float]]
         Function which takes a model (torch.nn.Module), a dataset
         (torch.utils.data.Dataset) and returns a dictionary of metric
         values (Dict[str, float]) which is used to assess model performance
         given the model and data.
-    runs : int
+    runs : int, default 1
         Number of models to run over all subsets
-    substeps : int
+    substeps : int, default 5
         Total number of dataset partitions that each model will train on
     train_kwargs : Dict[str, Any] | None, default None
         Additional arguments required for custom training function
     eval_kwargs : Dict[str, Any] | None, default None
         Additional arguments required for custom evaluation function
     """
 
@@ -257,31 +323,40 @@
     def eval_kwargs(self) -> Dict[str, Any]:
         return self._eval_kwargs
 
     @eval_kwargs.setter
     def eval_kwargs(self, value: Optional[Dict[str, Any]]):
         self._eval_kwargs = {} if value is None else value
 
-    def evaluate(self) -> Dict[str, np.ndarray]:
+    def evaluate(self, eval_at: Optional[np.ndarray] = None) -> Dict[str, np.ndarray]:
         """
         Creates data indices, trains models, and returns plotting data
 
+        Inputs
+        ------
+        eval_at : Optional[np.ndarray]
+            Specify this to collect accuracies over a specific set of dataset lengths,
+            rather than letting Sufficiency internally create the lengths
+            to evaluate at.
+
         Returns
         -------
         Dict[str, np.ndarray]
             Dictionary containing the average of each measure per substep
         """
-
-        geomshape = (
-            0.01 * self._length,
-            self._length,
-            self.substeps,
-        )  # Start, Stop, Num steps
-        ranges = np.geomspace(*geomshape).astype(np.int64)
-
+        if eval_at is not None:
+            ranges = eval_at
+        else:
+            geomshape = (
+                0.01 * self._length,
+                self._length,
+                self.substeps,
+            )  # Start, Stop, Num steps
+            ranges = np.geomspace(*geomshape).astype(np.int64)
+        substeps = len(ranges)
         metric_outputs = {}
 
         # Run each model over all indices
         for _ in range(self.runs):
             # Create a randomized set of indices to use
             indices = np.random.randint(0, self._length, size=self._length)
             # Reset the network weights to "create" an untrained model
@@ -305,15 +380,15 @@
 
                 # Keep track of each measures values
                 for name, value in output.items():
                     if name == STEPS_KEY:
                         raise KeyError(f"Cannot use '{STEPS_KEY}' as a metric name.")
 
                     if name not in metric_outputs:
-                        shape = (self.substeps, len(value)) if isinstance(value, np.ndarray) else self.substeps
+                        shape = (substeps, len(value)) if isinstance(value, np.ndarray) else substeps
                         metric_outputs[name] = np.zeros(shape)
 
                     # Sum result into current substep iteration to be averaged later
                     metric_outputs[name][iteration] += value
 
         output = {STEPS_KEY: ranges}
         # The mean for each measure must be calculated before being returned
@@ -322,23 +397,27 @@
         return output
 
     @classmethod
     def project(
         cls,
         data: Dict[str, np.ndarray],
         projection: Union[int, Sequence[int], np.ndarray],
+        niter: int = 1000,
     ) -> Dict[str, np.ndarray]:
         """Projects the measures for each value of X
 
         Parameters
         ----------
         data : Dict[str, np.ndarray]
             Dataclass containing the average of each measure per substep
         steps : Union[int, np.ndarray]
             Step or steps to project
+        niter : int, default 1000
+            Number of iterations to perform in the basin-hopping
+            numerical process to curve-fit data
 
         Raises
         ------
         KeyError
             If STEPS_KEY or measure is not a valid key
         ValueError
             If the length of data points in the measures do not match
@@ -348,26 +427,29 @@
         projection = [projection] if isinstance(projection, int) else projection
         projection = np.array(projection) if isinstance(projection, Sequence) else projection
         if not isinstance(projection, np.ndarray):
             raise ValueError("'steps' must be an int, Sequence[int] or ndarray")
 
         output = {}
         output[STEPS_KEY] = projection
+        params_cache = []
         for name, measure in data.items():
             if name == STEPS_KEY:
                 continue
 
-            if len(measure.shape) > 1:
+            if measure.ndim > 1:
                 result = []
                 for i in range(measure.shape[1]):
-                    projected = project_steps(measure[:, i], data[STEPS_KEY], projection)
+                    projected, params = project_steps(measure[:, i], data[STEPS_KEY], projection, niter)
+                    params_cache.append(params)
                     result.append(projected)
                 output[name] = np.array(result).T
             else:
-                output[name] = project_steps(measure, data[STEPS_KEY], projection)
+                output[name], params = project_steps(measure, data[STEPS_KEY], projection, niter)
+                params_cache.append(params)
         return output
 
     @classmethod
     def plot(cls, data: Dict[str, np.ndarray], class_names: Optional[Sequence[str]] = None) -> List[Figure]:
         """Plotting function for data sufficiency tasks
 
         Parameters
@@ -419,7 +501,61 @@
                     plots.append(fig)
 
             else:
                 fig = plot_measure(name, steps, measure, extrapolated)
                 plots.append(fig)
 
         return plots
+
+    @classmethod
+    def inv_project(
+        cls, targets: np.ndarray, data: Dict[str, np.ndarray], params_cache: np.ndarray = np.zeros((1, 0))
+    ) -> np.ndarray:
+        """
+        Calculate he number of training samples needed to achieve the target model
+        metric values.
+
+        Parameters
+        ----------
+        targets : np.ndarray
+            List of the target metric scores (from 0.0 to 1.0) that we want to achieve.
+
+        data : Dict[str, np.ndarray]
+            Dataclass containing the average of each measure per substep
+
+        params_cache : np.ndarray, default np.zeros((1,0))
+            1 x 3 List of cached parameters for the sufficiency curve. The parameters
+            can be precomputed by using the project() function.
+            TODO: The first axis should represent the number of data columns. It's
+            currently hardcoded to assume only one column.
+
+
+        Returns
+        -------
+        np.ndarray(np.int64)
+            List of the number of training samples needed to achieve each
+            corresponding entry in targets
+        """
+
+        validate_output(data)
+
+        
+
+        # Iterate through the elements of the data dictionary until
+        # we reach the array of measures, which are then used to predict
+        # the number of needed training samples
+        for name, measure in data.items():
+            if name == STEPS_KEY:
+                continue
+
+            # Select the cached parameters associated with the current column of measure
+            # TODO: We currently assume measure only has one axis
+            params = params_cache[0]
+
+            # X, y data
+            steps = data[STEPS_KEY]
+
+            num_samples_needed = inv_project_steps(measure, steps, targets, params)
+            return np.array(np.ceil(num_samples_needed), dtype=np.int64)
+
+        # TODO: Is this a reasonable error response
+        return np.array([np.int64(-1)])
```

### Comparing `daml-0.52.0/src/daml/_internal/metrics/uap.py` & `daml-0.53.0/src/daml/_internal/metrics/uap.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/src/daml/_internal/metrics/utils.py` & `daml-0.53.0/src/daml/_internal/metrics/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,10 +87,10 @@
     See Also
     --------
     :func:`sklearn.neighbors.NearestNeighbors`
     """
 
     nbrs = NearestNeighbors(n_neighbors=k + 1, algorithm=algorithm).fit(B)
     nns = nbrs.kneighbors(A)[1]
-    nns = nns[:, 1]
+    nns = nns[:, 1:].squeeze()
 
     return nns
```

### Comparing `daml-0.52.0/src/daml/_internal/models/pytorch/autoencoder.py` & `daml-0.53.0/src/daml/_internal/models/pytorch/autoencoder.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/src/daml/_internal/models/pytorch/blocks.py` & `daml-0.53.0/src/daml/_internal/models/pytorch/blocks.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/src/daml/_internal/models/pytorch/utils.py` & `daml-0.53.0/src/daml/_internal/models/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/src/daml/_internal/models/tensorflow/autoencoder.py` & `daml-0.53.0/src/daml/_internal/models/tensorflow/autoencoder.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/src/daml/_internal/models/tensorflow/gmm.py` & `daml-0.53.0/src/daml/_internal/models/tensorflow/gmm.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/src/daml/_internal/models/tensorflow/losses.py` & `daml-0.53.0/src/daml/_internal/models/tensorflow/losses.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/src/daml/_internal/models/tensorflow/pixelcnn.py` & `daml-0.53.0/src/daml/_internal/models/tensorflow/pixelcnn.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/src/daml/_internal/models/tensorflow/trainer.py` & `daml-0.53.0/src/daml/_internal/models/tensorflow/trainer.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/src/daml/_internal/models/tensorflow/utils.py` & `daml-0.53.0/src/daml/_internal/models/tensorflow/utils.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/src/daml/metrics/__init__.py` & `daml-0.53.0/src/daml/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/src/daml/metrics/drift/__init__.py` & `daml-0.53.0/src/daml/metrics/drift/__init__.py`

 * *Files identical despite different names*

### Comparing `daml-0.52.0/PKG-INFO` & `daml-0.53.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daml
-Version: 0.52.0
+Version: 0.53.0
 Summary: DAML provides a simple interface to characterize image data and its impact on model performance across classification and object-detection tasks
 Home-page: https://daml.ai/
 License: MIT
 Author: Andrew Weng
 Author-email: andrew.weng@ariacoustics.com
 Maintainer: ARiA
 Maintainer-email: daml@ariacoustics.com
@@ -19,26 +19,29 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering
 Provides-Extra: all
 Provides-Extra: tensorflow
 Provides-Extra: torch
+Requires-Dist: hdbscan (>=0.8.36)
 Requires-Dist: matplotlib ; extra == "torch" or extra == "all"
 Requires-Dist: numpy (>=1.24.2,<2)
 Requires-Dist: nvidia-cudnn-cu11 (>=8.6.0.163) ; extra == "torch" or extra == "tensorflow" or extra == "all" or extra == "all"
+Requires-Dist: pillow (>=10.3.0)
 Requires-Dist: scikit-learn (>=1.2.1)
 Requires-Dist: scipy (>=1.10)
 Requires-Dist: tensorflow (>=2.13.1,<2.14.0) ; (python_full_version >= "3.8.1" and python_full_version < "3.9.0") and (extra == "tensorflow" or extra == "all")
 Requires-Dist: tensorflow (>=2.14.1,<2.16) ; (python_version >= "3.9" and python_version < "3.12") and (extra == "tensorflow" or extra == "all")
 Requires-Dist: tensorflow-io-gcs-filesystem (>=0.34.0,<0.35.0) ; (python_full_version >= "3.8.1" and python_full_version < "3.9.0") and (extra == "tensorflow" or extra == "all")
 Requires-Dist: tensorflow-io-gcs-filesystem (>=0.35.0,<0.37) ; (python_version >= "3.9" and python_version < "3.12") and (extra == "tensorflow" or extra == "all")
 Requires-Dist: tensorflow_probability (>=0.21.0,<0.22.0) ; (python_full_version >= "3.8.1" and python_full_version < "3.9.0") and (extra == "tensorflow" or extra == "all")
 Requires-Dist: tensorflow_probability (>=0.22.1,<0.24) ; (python_version >= "3.9" and python_version < "3.12") and (extra == "tensorflow" or extra == "all")
 Requires-Dist: torch (>=2.0.1,!=2.2.0) ; extra == "torch" or extra == "all"
+Requires-Dist: xxhash (>=3.3)
 Project-URL: Documentation, https://daml.readthedocs.io/
 Project-URL: Repository, https://github.com/aria-ml/daml/
 Description-Content-Type: text/markdown
 
 # Data-Analysis Metrics Library (DAML)
 
 ## About DAML
@@ -90,20 +93,15 @@
 cd daml
 ```
 
 
 
 Install DAML with optional dependencies for development.
 ```
-poetry install --all-extras --with test,lint
-```
-
-Alternatively, you can install with optional dependencies used to generate documentation as well.
-```
-poetry install --all-extras --with test,lint,docs
+poetry install --all-extras --with dev
 ```
 
 Now that DAML is installed, you can run commands in the poetry virtual environment by prefixing shell commands with `poetry run`, or activate the virtual environment directly in the shell.
 ```
 poetry shell
 ```
```

