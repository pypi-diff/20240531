# Comparing `tmp/eulerpi-0.8.0.tar.gz` & `tmp/eulerpi-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eulerpi-0.8.0.tar", max compression
+gzip compressed data, was "eulerpi-0.8.1.tar", max compression
```

## Comparing `eulerpi-0.8.0.tar` & `eulerpi-0.8.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1117 2024-03-21 09:24:54.472781 eulerpi-0.8.0/LICENSE.md
--rw-r--r--   0        0        0     4999 2024-03-21 09:24:54.472781 eulerpi-0.8.0/README.md
--rw-r--r--   0        0        0      564 2024-03-21 09:24:54.476781 eulerpi-0.8.0/eulerpi/__init__.py
--rw-r--r--   0        0        0      184 2024-03-21 09:24:54.476781 eulerpi-0.8.0/eulerpi/core/__init__.py
--rw-r--r--   0        0        0     8487 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/core/data_transformation.py
--rw-r--r--   0        0        0      412 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/core/data_transformation_types.py
--rw-r--r--   0        0        0    12171 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/core/dense_grid.py
--rw-r--r--   0        0        0      416 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/core/dense_grid_types.py
--rw-r--r--   0        0        0    11029 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/core/inference.py
--rw-r--r--   0        0        0      512 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/core/inference_types.py
--rw-r--r--   0        0        0     5147 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/core/kde.py
--rw-r--r--   0        0        0    21574 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/core/model.py
--rw-r--r--   0        0        0     9994 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/core/model_check.py
--rw-r--r--   0        0        0    15755 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/core/plotting.py
--rw-r--r--   0        0        0    18493 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/core/result_manager.py
--rw-r--r--   0        0        0    16128 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/core/sampling.py
--rw-r--r--   0        0        0    21145 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/core/sparsegrid.py
--rw-r--r--   0        0        0    10122 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/core/transformations.py
--rw-r--r--   0        0        0        0 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/examples/__init__.py
--rw-r--r--   0        0        0    14800 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/examples/corona/CoronaData.csv
--rw-r--r--   0        0        0       94 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/examples/corona/__init__.py
--rw-r--r--   0        0        0     3748 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/examples/corona/corona.py
--rw-r--r--   0        0        0     1295 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/examples/cpp/CMakeLists.txt
--rw-r--r--   0        0        0        0 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/examples/cpp/__init__.py
--rw-r--r--   0        0        0     2214 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/examples/cpp/cpp_model.hpp
--rw-r--r--   0        0        0     1191 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/examples/cpp/cpp_plant.py
--rw-r--r--   0        0        0     2559 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/examples/cpp/python_reference_plants.py
--rw-r--r--   0        0        0      357 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/examples/cpp/wrapper.cpp
--rw-r--r--   0        0        0       82 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/examples/heat/__init__.py
--rw-r--r--   0        0        0    10934 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/examples/heat/heat.py
--rw-r--r--   0        0        0     1811 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml
--rw-r--r--   0        0        0      138 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/examples/sbml/__init__.py
--rw-r--r--   0        0        0     1285 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/examples/sbml/sbml_caffeine_model.py
--rw-r--r--   0        0        0     1705 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/examples/sbml/sbml_menten_model.py
--rw-r--r--   0        0        0     5493 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/examples/sbml/sbml_menten_model.xml
--rw-r--r--   0        0        0     2241 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/examples/simple_models.py
--rw-r--r--   0        0        0     5877 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/examples/temperature/TemperatureArtificialParams.csv
--rw-r--r--   0        0        0     5046 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/examples/temperature/TemperatureData.csv
--rw-r--r--   0        0        0      215 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/examples/temperature/__init__.py
--rw-r--r--   0        0        0     3886 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/examples/temperature/temperature.py
--rw-r--r--   0        0        0     2169 2024-03-21 09:24:54.480780 eulerpi-0.8.0/eulerpi/jax_extension.py
--rw-r--r--   0        0        0     2424 2024-03-21 09:24:54.480780 eulerpi-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     6576 1970-01-01 00:00:00.000000 eulerpi-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1117 2024-05-31 20:27:21.199517 eulerpi-0.8.1/LICENSE.md
+-rw-r--r--   0        0        0     4999 2024-05-31 20:27:21.199517 eulerpi-0.8.1/README.md
+-rw-r--r--   0        0        0      564 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/__init__.py
+-rw-r--r--   0        0        0      184 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/core/__init__.py
+-rw-r--r--   0        0        0     8487 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/core/data_transformation.py
+-rw-r--r--   0        0        0      412 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/core/data_transformation_types.py
+-rw-r--r--   0        0        0    12171 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/core/dense_grid.py
+-rw-r--r--   0        0        0      416 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/core/dense_grid_types.py
+-rw-r--r--   0        0        0    11029 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/core/inference.py
+-rw-r--r--   0        0        0      512 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/core/inference_types.py
+-rw-r--r--   0        0        0     5147 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/core/kde.py
+-rw-r--r--   0        0        0    21578 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/core/model.py
+-rw-r--r--   0        0        0     9994 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/core/model_check.py
+-rw-r--r--   0        0        0    15803 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/core/plotting.py
+-rw-r--r--   0        0        0    18493 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/core/result_manager.py
+-rw-r--r--   0        0        0    14787 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/core/sampling.py
+-rw-r--r--   0        0        0    21145 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/core/sparsegrid.py
+-rw-r--r--   0        0        0    10096 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/core/transformations.py
+-rw-r--r--   0        0        0        0 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/examples/__init__.py
+-rw-r--r--   0        0        0    14800 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/examples/corona/CoronaData.csv
+-rw-r--r--   0        0        0       94 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/examples/corona/__init__.py
+-rw-r--r--   0        0        0     3748 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/examples/corona/corona.py
+-rw-r--r--   0        0        0     1323 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/examples/cpp/CMakeLists.txt
+-rw-r--r--   0        0        0        0 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/examples/cpp/__init__.py
+-rw-r--r--   0        0        0     2214 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/examples/cpp/cpp_model.hpp
+-rw-r--r--   0        0        0     1191 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/examples/cpp/cpp_plant.py
+-rw-r--r--   0        0        0     2559 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/examples/cpp/python_reference_plants.py
+-rw-r--r--   0        0        0      357 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/examples/cpp/wrapper.cpp
+-rw-r--r--   0        0        0       82 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/examples/heat/__init__.py
+-rw-r--r--   0        0        0    10934 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/examples/heat/heat.py
+-rw-r--r--   0        0        0     1811 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml
+-rw-r--r--   0        0        0      138 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/examples/sbml/__init__.py
+-rw-r--r--   0        0        0     1277 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/examples/sbml/sbml_caffeine_model.py
+-rw-r--r--   0        0        0     1705 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/examples/sbml/sbml_menten_model.py
+-rw-r--r--   0        0        0     5493 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/examples/sbml/sbml_menten_model.xml
+-rw-r--r--   0        0        0     2241 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/examples/simple_models.py
+-rw-r--r--   0        0        0     5877 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/examples/temperature/TemperatureArtificialParams.csv
+-rw-r--r--   0        0        0     5046 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/examples/temperature/TemperatureData.csv
+-rw-r--r--   0        0        0      215 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/examples/temperature/__init__.py
+-rw-r--r--   0        0        0     3978 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/examples/temperature/temperature.py
+-rw-r--r--   0        0        0     2169 2024-05-31 20:27:21.207517 eulerpi-0.8.1/eulerpi/jax_extension.py
+-rw-r--r--   0        0        0     2510 2024-05-31 20:27:21.207517 eulerpi-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     6576 1970-01-01 00:00:00.000000 eulerpi-0.8.1/PKG-INFO
```

### Comparing `eulerpi-0.8.0/LICENSE.md` & `eulerpi-0.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eulerpi-0.8.0/README.md` & `eulerpi-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `eulerpi-0.8.0/eulerpi/__init__.py` & `eulerpi-0.8.1/eulerpi/__init__.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.8.0/eulerpi/core/data_transformation.py` & `eulerpi-0.8.1/eulerpi/core/data_transformation.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.8.0/eulerpi/core/dense_grid.py` & `eulerpi-0.8.1/eulerpi/core/dense_grid.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.8.0/eulerpi/core/inference.py` & `eulerpi-0.8.1/eulerpi/core/inference.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.8.0/eulerpi/core/inference_types.py` & `eulerpi-0.8.1/eulerpi/core/inference_types.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.8.0/eulerpi/core/kde.py` & `eulerpi-0.8.1/eulerpi/core/kde.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.8.0/eulerpi/core/model.py` & `eulerpi-0.8.1/eulerpi/core/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,20 +34,20 @@
         param_limits(np.ndarray): Box limits for the parameters. The limits are given as a 2D array with shape (param_dim, 2). The parameter limits are used as limits as well as for the movement policy for MCMC sampling, and as boundaries for the grid when using grid-based inference. Overwrite the function param_is_within_domain if the domain is more complex than a box - the grid will still be build based on param_limits, but actual model evaluations only take place within the limits specified in param_is_within_domain. (Default value = None)
         name(str): The name of the model. The class name is used if no name is given. (Default value = None)
 
     .. note::
         Examples of model implementations can be found in the :doc:`Example Models </examples>`.
     """
 
-    param_dim: Optional[
-        int
-    ] = None  #: The dimension of the parameter space of the model. It must be defined in the subclass.
-    data_dim: Optional[
-        int
-    ] = None  #: The dimension of the data space of the model. It must be defined in the subclass.
+    param_dim: Optional[int] = (
+        None  #: The dimension of the parameter space of the model. It must be defined in the subclass.
+    )
+    data_dim: Optional[int] = (
+        None  #: The dimension of the data space of the model. It must be defined in the subclass.
+    )
 
     def __init_subclass__(cls, **kwargs):
         """Check if the required attributes are set."""
         if not inspect.isabstract(cls):
             for required in (
                 "param_dim",
                 "data_dim",
```

### Comparing `eulerpi-0.8.0/eulerpi/core/model_check.py` & `eulerpi-0.8.1/eulerpi/core/model_check.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.8.0/eulerpi/core/plotting.py` & `eulerpi-0.8.1/eulerpi/core/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     reference_sample: Union[str, os.PathLike, np.ndarray, None] = None,
     run_name: str = "default_run",
     what_to_plot: str = "param",
     credibility_level: float = 0.95,
     num_vertical_grid_points: int = 100,
     axis_labels: Optional[list[str]] = None,
 ) -> axes:
-
     """Creates an overview figure with one violin plot for each marginal distribution.
        Can be used for parameters and simulation results and compares reference (or true underlying) and inferred values when possible.
 
     Args:
         model(Model): The model describing the mapping from parameters to data.
         reference_sample(Union[str, os.PathLike, np.ndarray]): Depending on what_to_plot, this is either the data sample used for the inference, or a reference sample of "true" parameter samples. If a string is given, it is assumed to be a path to a file containing the respective sample. (Default value = None)
         run_name(str): The name of the inference run. (Default value = "default_run")
@@ -257,17 +256,17 @@
             # fill the violin envelopes
 
             ax.fill_betweenx(
                 vertical_grid_1d[reference_konfidence_index],
                 reference_left_bound_konf,
                 reference_right_bound_konf,
                 color=colorOrig,
-                label=r"$\Phi_\mathcal{" + variable_name + "}$"
-                if i == 0
-                else "",
+                label=(
+                    r"$\Phi_\mathcal{" + variable_name + "}$" if i == 0 else ""
+                ),
                 alpha=0.3,
             )
 
             # draw arrows to show the width of the violin envelopes
             ax.arrow(
                 np.amin(reference_left_bound),
                 max_density_argument,
@@ -367,17 +366,19 @@
             )
 
         ax.fill_betweenx(
             vertical_grid_1d[reconstructed_konfidence_index],
             reconstructed_left_bound_konf,
             reconstructed_right_bound_konf,
             color=colorAppr,
-            label=r"$\Phi_{\hat{\mathcal{" + variable_name + "}}}$"
-            if i == 0
-            else "",
+            label=(
+                r"$\Phi_{\hat{\mathcal{" + variable_name + "}}}$"
+                if i == 0
+                else ""
+            ),
             alpha=0.3,
         )
 
         if not reference_available:
             # draw arrows to show the width of the violin envelopes
             ax.arrow(
                 np.amin(reconstructed_left_bound),
```

### Comparing `eulerpi-0.8.0/eulerpi/core/result_manager.py` & `eulerpi-0.8.1/eulerpi/core/result_manager.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.8.0/eulerpi/core/sampling.py` & `eulerpi-0.8.1/eulerpi/core/sampling.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 .. note::
 
     The functions in this module are mainly intended for internal use and are accessed by :func:`inference <eulerpi.core.inference>` function.
     Read the documentation of :func:`inference_mcmc <inference_mcmc>` to learn more about the available options for the MCMC based inference.
 """
 
-
 import typing
 from multiprocessing import get_context
 from os import path
 
 import emcee
 import numpy as np
 
@@ -23,50 +22,14 @@
 from eulerpi.core.data_transformation import DataTransformation
 from eulerpi.core.inference_types import InferenceType
 from eulerpi.core.kde import calc_kernel_width
 from eulerpi.core.model import Model
 from eulerpi.core.result_manager import ResultManager
 from eulerpi.core.transformations import eval_log_transformed_density
 
-# TODO: This works on the blob
-# Return the samples.
-# return sampler.get_chain(discard=0, thin=1, flat=True)
-# TODO: This stores the sample as 2d array in the format walker1_step1, walker2_step1, walker3_step1, walker1_step2, walker2_step2, walker3_step2, ...
-# sampler_results = samplerBlob.reshape(
-#     num_walkers * num_steps, sampling_dim + data_dim + 1
-# )
-
-
-def evaluate_sample(
-    param: np.ndarray,
-    model: Model,
-    data: np.ndarray,
-    data_transformation: DataTransformation,
-    data_stdevs: np.ndarray,
-    slice: np.ndarray,
-) -> typing.Tuple[float, np.ndarray]:
-    """Evaluate the log transformed density at the given parameter values.
-
-    Args:
-        param (np.ndarray): parameter values
-        model (Model): The model which will be sampled
-        data (np.ndarray): data
-        data_transformation (DataTransformation): The data transformation used to normalize the data.
-        data_stdevs (np.ndarray): kernel width for the data
-        slice (np.ndarray): slice of the parameter space which will be sampled
-
-    Returns:
-        typing.Tuple[float, np.ndarray]: log transformed density and the sampler result
-    """
-
-    log_samplerresult = eval_log_transformed_density(
-        param, model, data, data_transformation, data_stdevs, slice
-    )
-    return log_samplerresult
-
 
 def run_emcee_once(
     model: Model,
     data: np.ndarray,
     data_transformation: DataTransformation,
     data_stdevs: np.ndarray,
     slice: np.ndarray,
@@ -98,15 +61,15 @@
     sampling_dim = slice.shape[0]
 
     # Call the sampler for all parallel workers (possibly use arg moves = movePolicy)
     try:
         sampler = emcee.EnsembleSampler(
             num_walkers,
             sampling_dim,
-            evaluate_sample,
+            eval_log_transformed_density,
             pool=pool,
             args=[model, data, data_transformation, data_stdevs, slice],
         )
         # Extract the final walker position and close the pool of worker processes.
         final_walker_positions, _, _, _ = sampler.run_mcmc(
             initial_walker_positions, num_steps, tune=True, progress=True
         )
@@ -180,23 +143,22 @@
         typing.Tuple[np.ndarray, np.ndarray, np.ndarray]: Array with all params, array with all data, array with all log probabilities
         TODO check: are those really log probabilities?
 
     """
     # Calculate the standard deviation of the data for each dimension
     data_stdevs = calc_kernel_width(data)
     sampling_dim = slice.shape[0]
-    central_param = model.central_param
-    param_limits = model.param_limits
 
     # Initialize each walker at a Gaussian-drawn random, slightly different parameter close to the central parameter.
     # compute element-wise min of the difference between the central parameter and the lower sampling limit and the difference between the central parameter and the upper sampling limit
     d_min = np.minimum(
-        central_param - param_limits[:, 0], param_limits[:, 1] - central_param
+        model.central_param - model.param_limits[:, 0],
+        model.param_limits[:, 1] - model.central_param,
     )
-    initial_walker_positions = central_param[slice] + d_min[slice] * (
+    initial_walker_positions = model.central_param[slice] + d_min[slice] * (
         np.random.rand(num_walkers, sampling_dim) - 0.5
     )
 
     # Count and print how many runs have already been performed for this model
     num_existing_files = result_manager.count_emcee_sub_runs(slice)
     logger.debug(f"{num_existing_files} existing files found")
```

### Comparing `eulerpi-0.8.0/eulerpi/core/sparsegrid.py` & `eulerpi-0.8.1/eulerpi/core/sparsegrid.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.8.0/eulerpi/core/transformations.py` & `eulerpi-0.8.1/eulerpi/core/transformations.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,18 +76,16 @@
         # all_res is the concatenation of the evaluated parameter, the simulation result arising from that parameter and the inferred paramter density. Decompose as follows:
         eval_param = all_res[0:model.param_dim]
         sim_result = all_res[model.param_dim:model.param_dim+model.data_dim]
         central_param_density = all_res[-1]
 
     """
 
-    limits = model.param_limits
-
     # Build the full parameter vector for evaluation based on the passed param slice and the constant central points
-    fullParam = model.central_param
+    fullParam = model.central_param.copy()
     fullParam[slice] = param
 
     # Check if the tried parameter is within the just-defined bounds and return the lowest possible density if not.
     if (
         np.any(param < model.param_limits[slice, 0])
         or np.any(param > model.param_limits[slice, 1])
         or not model.param_is_within_domain(fullParam)
```

### Comparing `eulerpi-0.8.0/eulerpi/examples/corona/CoronaData.csv` & `eulerpi-0.8.1/eulerpi/examples/corona/CoronaData.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.8.0/eulerpi/examples/corona/corona.py` & `eulerpi-0.8.1/eulerpi/examples/corona/corona.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.8.0/eulerpi/examples/cpp/CMakeLists.txt` & `eulerpi-0.8.1/eulerpi/examples/cpp/CMakeLists.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-cmake_minimum_required(VERSION 3.4...3.18)
+cmake_minimum_required(VERSION 3.4...3.29)
 project(cpp_model LANGUAGES CXX)
 
 find_package(Eigen3 REQUIRED)
 # Maybe you have to do something linke this: sudo ln -s /usr/include/eigen3/Eigen /usr/include/Eigen
 message(STATUS "Eigen3 version ${EIGEN3_VERSION} found in ${EIGEN3_INCLUDE_DIR}")
 
+set(PYBIND11_FINDPYTHON ON)
 find_package(pybind11 REQUIRED)
 pybind11_add_module(cpp_model wrapper.cpp cpp_model.hpp) # Add wrapper code and all library source files
 
 set(CMAKE_CXX_STANDARD 14 CACHE STRING "C++ version selection")  # or 11, 14, 17, 20
 set(CMAKE_CXX_STANDARD_REQUIRED ON)  # optional, ensure standard is supported
 set(CMAKE_CXX_EXTENSIONS OFF)  # optional, keep compiler extensions off
```

### Comparing `eulerpi-0.8.0/eulerpi/examples/cpp/cpp_model.hpp` & `eulerpi-0.8.1/eulerpi/examples/cpp/cpp_model.hpp`

 * *Files identical despite different names*

### Comparing `eulerpi-0.8.0/eulerpi/examples/cpp/cpp_plant.py` & `eulerpi-0.8.1/eulerpi/examples/cpp/cpp_plant.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.8.0/eulerpi/examples/cpp/python_reference_plants.py` & `eulerpi-0.8.1/eulerpi/examples/cpp/python_reference_plants.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.8.0/eulerpi/examples/heat/heat.py` & `eulerpi-0.8.1/eulerpi/examples/heat/heat.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.8.0/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml` & `eulerpi-0.8.1/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml`

 * *Files identical despite different names*

### Comparing `eulerpi-0.8.0/eulerpi/examples/sbml/sbml_caffeine_model.py` & `eulerpi-0.8.1/eulerpi/examples/sbml/sbml_caffeine_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self,
         central_param: np.ndarray = CENTRAL_PARAM,
         param_limits: np.ndarray = PARAM_LIMITS,
         **kwargs,
     ) -> None:
         param_ids = ["A", "B"]
         timepoints = np.array([0.5, 1.0])
-        sbml_files = files(package="eulerpi.examples.sbml")
+        sbml_files = files("eulerpi.examples.sbml")
         sbml_file_name = "Caffeine_2Wks_Exponential_decay.xml"
         with as_file(sbml_files.joinpath(sbml_file_name)) as sbml_file:
             super().__init__(
                 sbml_file,
                 central_param,
                 param_limits,
                 timepoints,
```

### Comparing `eulerpi-0.8.0/eulerpi/examples/sbml/sbml_menten_model.py` & `eulerpi-0.8.1/eulerpi/examples/sbml/sbml_menten_model.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.8.0/eulerpi/examples/sbml/sbml_menten_model.xml` & `eulerpi-0.8.1/eulerpi/examples/sbml/sbml_menten_model.xml`

 * *Files identical despite different names*

### Comparing `eulerpi-0.8.0/eulerpi/examples/simple_models.py` & `eulerpi-0.8.1/eulerpi/examples/simple_models.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.8.0/eulerpi/examples/temperature/TemperatureArtificialParams.csv` & `eulerpi-0.8.1/eulerpi/examples/temperature/TemperatureArtificialParams.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.8.0/eulerpi/examples/temperature/TemperatureData.csv` & `eulerpi-0.8.1/eulerpi/examples/temperature/TemperatureData.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.8.0/eulerpi/examples/temperature/temperature.py` & `eulerpi-0.8.1/eulerpi/examples/temperature/temperature.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,18 +65,19 @@
             \\frac{dy}{dq} = -60 \\cdot \\sin{(q)}
         """
         return jnp.array([60.0 * jnp.sin(jnp.abs(param[0]))])
 
 
 class TemperatureArtificial(Temperature, ArtificialModelInterface):
     def generate_artificial_params(self, num_data_points: int = -1):
-        paramPath = importlib.resources.path(
-            "eulerpi.examples.temperature", "TemperatureArtificialParams.csv"
-        )
-        true_param_sample = np.loadtxt(paramPath, delimiter=",", ndmin=2)
+        param_resource = importlib.resources.files(
+            "eulerpi.examples.temperature"
+        ).joinpath("TemperatureArtificialParams.csv")
+        with importlib.resources.as_file(param_resource) as param_file:
+            true_param_sample = np.loadtxt(param_file, delimiter=",", ndmin=2)
         return true_param_sample
 
 
 class TemperatureWithFixedParams(Temperature):
     """The model describes the temperature :math:`y` in degree celsius at a given latitude :math:`q` in degree.
 
     .. note::
```

### Comparing `eulerpi-0.8.0/eulerpi/jax_extension.py` & `eulerpi-0.8.1/eulerpi/jax_extension.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.8.0/pyproject.toml` & `eulerpi-0.8.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eulerpi"
-version = "0.8.0"
+version = "0.8.1"
 description = "The eulerian parameter inference (eulerpi) returns a parameter distribution, which is consistent with the observed data by solving the inverse problem directly. In the case of a one-to-one mapping, this is the true underlying distribution."
 authors = ["Lars Kaiser <lars.g.kaiser@gmx.de>", "Sebastian Hoepfl <sebastian.hoepfl@ist.uni-stuttgart.de>", "Vincent Wagner <vincent.wagner@ist.uni-stuttgart.de>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -31,27 +31,29 @@
 amici = { version = "^0.16.1", optional = true }
 scikit-learn = "^1.3.1"
 
 [tool.poetry.extras]
 sbml = ["amici"]
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^3.5.0"
-black = "^23.10.0"
-flake8 = "^6.1.0"
-isort = "^5.12.0"
-pytest = "^7.4.2"
-pyproject-flake8 = "^6.1.0"
-coverage = "^7.3.2"
-ipykernel = "^6.25.2"
-sphinx = "^7"
+pre-commit = "^3.7.1"
+black = "^24.4.2"
+flake8 = "^7.0.0"
+isort = "^5.13.2"
+pytest = "^8.2.0"
+pyproject-flake8 = "^7.0.0"
+coverage = "^7.5.0"
+sphinx = "^7.3.7"
 sphinx-copybutton = "^0.5.2"
 sphinx-togglebutton = "^0.3.2"
-sphinx-rtd-theme = "^1.3.0"
-myst-parser = "^2.0.0"
+sphinx-rtd-theme = "^2.0.0"
+myst-parser = "^3.0.1"
+jupyter = "^1.0.0"
+nbmake = "^1.5.3"
+pyqt6 = "^6.7.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 79
@@ -66,21 +68,23 @@
 [tool.flake8]
 extend-ignore = ["E501", "E203", "F841"] # Length of lines already handled by black, spacing, unused variables
 per-file-ignores = ["__init__.py: F401"]
 
 [tool.pytest.ini_options]
 testpaths = [
   "tests",
+  "docs/source/tutorial_material",
 ]
 norecursedirs = [
     "generated_sbml_models",
     "Data",
     "Applications",
     "build",
 ]
 addopts = [
     "--import-mode=importlib",
+    "--nbmake",
 ]
 pythonpath = ["eulerpi"]
 filterwarnings = [
     'ignore:FigureCanvasTemplate is non-interactive, and thus cannot be shown',
 ]
```

### Comparing `eulerpi-0.8.0/PKG-INFO` & `eulerpi-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eulerpi
-Version: 0.8.0
+Version: 0.8.1
 Summary: The eulerian parameter inference (eulerpi) returns a parameter distribution, which is consistent with the observed data by solving the inverse problem directly. In the case of a one-to-one mapping, this is the true underlying distribution.
 Author: Lars Kaiser
 Author-email: lars.g.kaiser@gmx.de
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

