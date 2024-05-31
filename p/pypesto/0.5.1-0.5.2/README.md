# Comparing `tmp/pypesto-0.5.1.tar.gz` & `tmp/pypesto-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypesto-0.5.1.tar", last modified: Wed Apr 17 08:03:42 2024, max compression
+gzip compressed data, was "pypesto-0.5.2.tar", last modified: Fri May 31 13:47:49 2024, max compression
```

## Comparing `pypesto-0.5.1.tar` & `pypesto-0.5.2.tar`

### file list

```diff
@@ -1,198 +1,202 @@
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.880237 pypesto-0.5.1/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1484 2024-04-17 08:00:04.000000 pypesto-0.5.1/LICENSE
--rw-r--r--   0 dweindl   (1000) dweindl   (1000)    13455 2024-04-17 08:03:42.880237 pypesto-0.5.1/PKG-INFO
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3976 2024-04-17 08:00:04.000000 pypesto-0.5.1/README.md
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.864237 pypesto-0.5.1/pypesto/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    10042 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/C.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      950 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/__init__.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.864237 pypesto-0.5.1/pypesto/engine/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      401 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/engine/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      593 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/engine/base.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1520 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/engine/mpi_pool.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2400 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/engine/multi_process.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2014 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/engine/multi_thread.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      922 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/engine/single_core.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      456 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/engine/task.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.864237 pypesto-0.5.1/pypesto/ensemble/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      673 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/ensemble/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    11811 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/ensemble/covariance_analysis.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9064 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/ensemble/dimension_reduction.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    43778 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/ensemble/ensemble.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      912 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/ensemble/task.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    11609 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/ensemble/util.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.865237 pypesto-0.5.1/pypesto/hierarchical/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1284 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/hierarchical/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     4256 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/hierarchical/base_parameter.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8617 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/hierarchical/base_problem.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1317 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/hierarchical/base_solver.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    20815 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/hierarchical/inner_calculator_collector.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.865237 pypesto-0.5.1/pypesto/hierarchical/ordinal/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1466 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/hierarchical/ordinal/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6877 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/hierarchical/ordinal/calculator.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2716 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/hierarchical/ordinal/parameter.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    27980 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/hierarchical/ordinal/problem.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    42338 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/hierarchical/ordinal/solver.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    24318 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/hierarchical/petab.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.865237 pypesto-0.5.1/pypesto/hierarchical/relative/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1256 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/hierarchical/relative/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    12359 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/hierarchical/relative/calculator.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9797 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/hierarchical/relative/problem.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    21213 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/hierarchical/relative/solver.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    15487 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/hierarchical/relative/util.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.865237 pypesto-0.5.1/pypesto/hierarchical/semiquantitative/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      801 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/hierarchical/semiquantitative/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6907 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/hierarchical/semiquantitative/calculator.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1981 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/hierarchical/semiquantitative/parameter.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    17607 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/hierarchical/semiquantitative/problem.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    36208 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/hierarchical/semiquantitative/solver.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.866237 pypesto-0.5.1/pypesto/history/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      654 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/history/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7892 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/history/amici.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    15368 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/history/base.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9696 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/history/csv.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1480 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/history/generate.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    16419 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/history/hdf5.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3899 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/history/memory.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9808 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/history/optimizer.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3507 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/history/options.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1789 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/history/util.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1902 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/logging.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.866237 pypesto-0.5.1/pypesto/objective/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      313 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/objective/__init__.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.866237 pypesto-0.5.1/pypesto/objective/aesara/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)       77 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/objective/aesara/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8954 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/objective/aesara/base.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5281 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/objective/aggregated.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.866237 pypesto-0.5.1/pypesto/objective/amici/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      141 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/objective/amici/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    23234 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/objective/amici/amici.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7677 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/objective/amici/amici_calculator.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    13242 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/objective/amici/amici_util.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    22677 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/objective/base.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    24307 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/objective/finite_difference.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7764 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/objective/function.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.866237 pypesto-0.5.1/pypesto/objective/jax/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)       71 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/objective/jax/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6578 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/objective/jax/base.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.867237 pypesto-0.5.1/pypesto/objective/julia/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      136 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/objective/julia/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6179 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/objective/julia/base.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7334 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/objective/julia/petabJl.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9757 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/objective/julia/petab_jl_importer.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     4262 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/objective/pre_post_process.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    17128 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/objective/priors.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.867237 pypesto-0.5.1/pypesto/objective/roadrunner/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      279 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/objective/roadrunner/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    13983 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/objective/roadrunner/petab_importer_roadrunner.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     4864 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/objective/roadrunner/road_runner.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    15757 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/objective/roadrunner/roadrunner_calculator.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    14675 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/objective/roadrunner/utils.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.867237 pypesto-0.5.1/pypesto/optimize/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      678 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/optimize/__init__.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.867237 pypesto-0.5.1/pypesto/optimize/ess/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      296 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/optimize/ess/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    23962 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/optimize/ess/ess.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9348 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/optimize/ess/function_evaluator.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7045 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/optimize/ess/refset.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    35553 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/optimize/ess/sacess.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8254 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/optimize/load.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5395 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/optimize/optimize.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    44942 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/optimize/optimizer.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1967 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/optimize/options.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2000 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/optimize/task.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5526 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/optimize/util.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.868237 pypesto-0.5.1/pypesto/petab/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      647 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/petab/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    37790 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/petab/importer.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.868237 pypesto-0.5.1/pypesto/predict/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      211 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/predict/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    17993 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/predict/amici_predictor.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1306 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/predict/task.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.868237 pypesto-0.5.1/pypesto/problem/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      207 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/problem/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    18562 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/problem/base.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3146 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/problem/hierarchical.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.868237 pypesto-0.5.1/pypesto/profile/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      288 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/profile/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3545 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/profile/approximate.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     4210 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/profile/options.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5859 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/profile/profile.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    15436 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/profile/profile_next_guess.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2440 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/profile/task.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6867 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/profile/util.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5230 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/profile/validation_intervals.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5524 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/profile/walk_along_profile.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.868237 pypesto-0.5.1/pypesto/result/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      415 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/result/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    14017 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/result/optimize.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    12314 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/result/predict.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8076 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/result/profile.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1409 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/result/result.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3772 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/result/sample.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.869237 pypesto-0.5.1/pypesto/sample/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      644 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/sample/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7400 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/sample/adaptive_metropolis.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2797 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/sample/adaptive_parallel_tempering.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1760 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/sample/auto_correlation.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3991 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/sample/diagnostics.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    14140 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/sample/dynesty.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7790 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/sample/emcee.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5624 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/sample/geweke_test.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7052 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/sample/metropolis.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    11554 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/sample/parallel_tempering.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7965 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/sample/pymc.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3163 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/sample/sample.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     4131 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/sample/sampler.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3327 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/sample/util.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.869237 pypesto-0.5.1/pypesto/select/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      605 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/select/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    18540 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/select/method.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5501 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/select/misc.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7769 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/select/model_problem.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5522 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/select/postprocessors.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9975 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/select/problem.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.869237 pypesto-0.5.1/pypesto/startpoint/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      483 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/startpoint/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7744 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/startpoint/base.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2895 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/startpoint/latin_hypercube.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1263 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/startpoint/uniform.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      455 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/startpoint/util.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.870237 pypesto-0.5.1/pypesto/store/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      486 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/store/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2553 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/store/auto.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2248 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/store/hdf5.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    10907 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/store/read_from_hdf5.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    10049 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/store/save_to_hdf5.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.870237 pypesto-0.5.1/pypesto/testing/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)       49 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/testing/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     4020 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/testing/examples.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8984 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/util.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)       22 2024-04-17 08:03:33.000000 pypesto-0.5.1/pypesto/version.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.871237 pypesto-0.5.1/pypesto/visualize/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1738 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/visualize/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6826 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/visualize/clust_color.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8804 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/visualize/dimension_reduction.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    12751 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/visualize/ensemble.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    12318 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/visualize/misc.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    13201 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/visualize/model_fit.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    13035 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/visualize/optimization_stats.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1806 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/visualize/optimizer_convergence.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    15936 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/visualize/optimizer_history.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    32168 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/visualize/ordinal_categories.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    20147 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/visualize/parameters.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2711 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/visualize/profile_cis.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    15247 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/visualize/profiles.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5759 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/visualize/reference_points.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    46091 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/visualize/sampling.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6174 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/visualize/select.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    18239 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/visualize/spline_approximation.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    14548 2024-04-17 08:00:04.000000 pypesto-0.5.1/pypesto/visualize/waterfall.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 08:03:42.871237 pypesto-0.5.1/pypesto.egg-info/
--rw-r--r--   0 dweindl   (1000) dweindl   (1000)    13455 2024-04-17 08:03:42.000000 pypesto-0.5.1/pypesto.egg-info/PKG-INFO
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5264 2024-04-17 08:03:42.000000 pypesto-0.5.1/pypesto.egg-info/SOURCES.txt
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)        1 2024-04-17 08:03:42.000000 pypesto-0.5.1/pypesto.egg-info/dependency_links.txt
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2313 2024-04-17 08:03:42.000000 pypesto-0.5.1/pypesto.egg-info/requires.txt
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)        8 2024-04-17 08:03:42.000000 pypesto-0.5.1/pypesto.egg-info/top_level.txt
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1321 2024-04-17 08:00:04.000000 pypesto-0.5.1/pyproject.toml
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3172 2024-04-17 08:03:42.881237 pypesto-0.5.1/setup.cfg
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)       88 2024-04-17 08:00:04.000000 pypesto-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.417183 pypesto-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-31 13:47:38.000000 pypesto-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13450 2024-05-31 13:47:49.417183 pypesto-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-31 13:47:38.000000 pypesto-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.369183 pypesto-0.5.2/pypesto/
+-rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/C.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.369183 pypesto-0.5.2/pypesto/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/engine/mpi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/engine/multi_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/engine/multi_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/engine/single_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/engine/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.373183 pypesto-0.5.2/pypesto/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/ensemble/covariance_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/ensemble/dimension_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43778 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/ensemble/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/ensemble/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11609 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/ensemble/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.373183 pypesto-0.5.2/pypesto/hierarchical/
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/hierarchical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/hierarchical/base_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/hierarchical/base_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/hierarchical/base_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20820 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/hierarchical/inner_calculator_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.373183 pypesto-0.5.2/pypesto/hierarchical/ordinal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/hierarchical/ordinal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/hierarchical/ordinal/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/hierarchical/ordinal/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27980 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/hierarchical/ordinal/problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42344 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/hierarchical/ordinal/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24318 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/hierarchical/petab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.373183 pypesto-0.5.2/pypesto/hierarchical/relative/
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/hierarchical/relative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12364 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/hierarchical/relative/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/hierarchical/relative/problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21257 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/hierarchical/relative/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15991 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/hierarchical/relative/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.373183 pypesto-0.5.2/pypesto/hierarchical/semiquantitative/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/hierarchical/semiquantitative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/hierarchical/semiquantitative/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/hierarchical/semiquantitative/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17607 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/hierarchical/semiquantitative/problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36214 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/hierarchical/semiquantitative/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.377183 pypesto-0.5.2/pypesto/history/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/history/amici.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15368 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/history/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/history/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/history/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16419 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/history/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/history/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/history/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/history/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/history/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.377183 pypesto-0.5.2/pypesto/objective/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/objective/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.377183 pypesto-0.5.2/pypesto/objective/aesara/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/objective/aesara/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/objective/aesara/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/objective/aggregated.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.381183 pypesto-0.5.2/pypesto/objective/amici/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/objective/amici/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23234 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/objective/amici/amici.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/objective/amici/amici_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/objective/amici/amici_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22677 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/objective/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24307 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/objective/finite_difference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7764 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/objective/function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.381183 pypesto-0.5.2/pypesto/objective/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/objective/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/objective/jax/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.381183 pypesto-0.5.2/pypesto/objective/julia/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/objective/julia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/objective/julia/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/objective/julia/petabJl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/objective/julia/petab_jl_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/objective/pre_post_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16931 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/objective/priors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.381183 pypesto-0.5.2/pypesto/objective/roadrunner/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/objective/roadrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13983 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/objective/roadrunner/petab_importer_roadrunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/objective/roadrunner/road_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15757 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/objective/roadrunner/roadrunner_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14675 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/objective/roadrunner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.381183 pypesto-0.5.2/pypesto/optimize/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/optimize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.385183 pypesto-0.5.2/pypesto/optimize/ess/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/optimize/ess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24008 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/optimize/ess/ess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/optimize/ess/function_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/optimize/ess/refset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37267 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/optimize/ess/sacess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/optimize/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/optimize/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44942 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/optimize/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/optimize/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/optimize/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/optimize/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.385183 pypesto-0.5.2/pypesto/petab/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/petab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37754 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/petab/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.385183 pypesto-0.5.2/pypesto/predict/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/predict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17993 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/predict/amici_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/predict/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.385183 pypesto-0.5.2/pypesto/problem/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/problem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19703 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/problem/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/problem/hierarchical.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.389183 pypesto-0.5.2/pypesto/profile/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/profile/approximate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/profile/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/profile/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15436 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/profile/profile_next_guess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/profile/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/profile/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/profile/validation_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/profile/walk_along_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.389183 pypesto-0.5.2/pypesto/result/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/result/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13989 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/result/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12314 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/result/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/result/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/result/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/result/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.393183 pypesto-0.5.2/pypesto/sample/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7400 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/sample/adaptive_metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/sample/adaptive_parallel_tempering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/sample/auto_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/sample/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/sample/dynesty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7789 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/sample/emcee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/sample/geweke_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/sample/metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11525 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/sample/parallel_tempering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/sample/pymc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/sample/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/sample/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/sample/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.393183 pypesto-0.5.2/pypesto/select/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/select/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18540 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/select/method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/select/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/select/model_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/select/postprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9975 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/select/problem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.393183 pypesto-0.5.2/pypesto/startpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/startpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/startpoint/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/startpoint/latin_hypercube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/startpoint/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/startpoint/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.393183 pypesto-0.5.2/pypesto/store/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/store/auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/store/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/store/read_from_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/store/save_to_hdf5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.393183 pypesto-0.5.2/pypesto/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/testing/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.397183 pypesto-0.5.2/pypesto/variational/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/variational/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6487 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/variational/pymc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/variational/variational_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.401183 pypesto-0.5.2/pypesto/visualize/
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/visualize/clust_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/visualize/dimension_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12751 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/visualize/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/visualize/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13231 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/visualize/model_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13249 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/visualize/optimization_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/visualize/optimizer_convergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15936 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/visualize/optimizer_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32202 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/visualize/ordinal_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19576 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/visualize/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/visualize/profile_cis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15247 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/visualize/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/visualize/reference_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46091 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/visualize/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/visualize/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18225 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/visualize/spline_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-05-31 13:47:38.000000 pypesto-0.5.2/pypesto/visualize/waterfall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:47:49.401183 pypesto-0.5.2/pypesto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13450 2024-05-31 13:47:49.000000 pypesto-0.5.2/pypesto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-05-31 13:47:49.000000 pypesto-0.5.2/pypesto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:47:49.000000 pypesto-0.5.2/pypesto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-31 13:47:49.000000 pypesto-0.5.2/pypesto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 13:47:49.000000 pypesto-0.5.2/pypesto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-31 13:47:38.000000 pypesto-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-31 13:47:49.417183 pypesto-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-31 13:47:38.000000 pypesto-0.5.2/setup.py
```

### Comparing `pypesto-0.5.1/LICENSE` & `pypesto-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/PKG-INFO` & `pypesto-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypesto
-Version: 0.5.1
+Version: 0.5.2
 Summary: python-based Parameter EStimation TOolbox
 Home-page: https://github.com/icb-dcm/pypesto
 Download-URL: https://github.com/icb-dcm/pypesto/releases
 Author: The pyPESTO developers
 Author-email: yannik.schaelte@gmail.com
 Maintainer: Paul Jonas Jost, Maren Philipps, Domagoj Dorešić, Fabian Fröhlich
 Maintainer-email: paul.jost@uni-bonn.de, maren.philipps@uni-bonn.de, domagoj.doresic@uni-bonn.de, fabian.frohlich@crick.ac.uk
@@ -13,18 +13,18 @@
 Project-URL: Documentation, https://pypesto.readthedocs.io
 Project-URL: Changelog, https://pypesto.readthedocs.io/en/latest/changelog.html
 Keywords: parameter inference,optimization,sampling,profiles,ODE,AMICI,systems biology
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy!=1.24.0,>=1.19.1
 Requires-Dist: scipy>=1.5.2
 Requires-Dist: pandas>=1.5.0
 Requires-Dist: cloudpickle>=1.5.0
 Requires-Dist: matplotlib>=3.6.2
@@ -41,15 +41,14 @@
 Requires-Dist: nlopt>=2.6.2; extra == "all"
 Requires-Dist: pyswarm>=0.6; extra == "all"
 Requires-Dist: cma>=3.0.3; extra == "all"
 Requires-Dist: pyswarms>=1.3.0; extra == "all"
 Requires-Dist: fides>=0.6.1; extra == "all"
 Requires-Dist: mpi4py>=3.0.3; extra == "all"
 Requires-Dist: arviz>=0.12.1; extra == "all"
-Requires-Dist: scipy<1.13.0; extra == "all"
 Requires-Dist: aesara>=2.8.6; extra == "all"
 Requires-Dist: pymc>=4.2.1; extra == "all"
 Requires-Dist: aesara>=2.0.5; extra == "all"
 Requires-Dist: jax>=0.4.1; extra == "all"
 Requires-Dist: jaxlib>=0.4.1; extra == "all"
 Requires-Dist: julia>=0.5.7; extra == "all"
 Requires-Dist: ipython>=8.4.0; extra == "all"
@@ -67,15 +66,14 @@
 Requires-Dist: ipython>=8.4.0; extra == "all"
 Requires-Dist: myst-parser>=0.18.0; extra == "all"
 Requires-Dist: ipykernel==6.23.1; extra == "all"
 Requires-Dist: julia>=0.5.7; extra == "all"
 Requires-Dist: ipython>=8.4.0; extra == "all"
 Requires-Dist: pygments>=2.12.0; extra == "all"
 Requires-Dist: arviz>=0.12.1; extra == "all"
-Requires-Dist: scipy<1.13.0; extra == "all"
 Requires-Dist: aesara>=2.8.6; extra == "all"
 Requires-Dist: pymc>=4.2.1; extra == "all"
 Requires-Dist: emcee>=3.0.2; extra == "all"
 Requires-Dist: dynesty>=2.0.3; extra == "all"
 Requires-Dist: nlopt>=2.6.2; extra == "all"
 Requires-Dist: pyswarm>=0.6; extra == "all"
 Requires-Dist: notebook>=6.1.4; extra == "all"
@@ -88,15 +86,14 @@
 Requires-Dist: jax>=0.4.1; extra == "all"
 Requires-Dist: jaxlib>=0.4.1; extra == "all"
 Requires-Dist: libroadrunner>=2.6.0; extra == "all"
 Requires-Dist: julia>=0.5.7; extra == "all"
 Requires-Dist: ipython>=8.4.0; extra == "all"
 Requires-Dist: pygments>=2.12.0; extra == "all"
 Requires-Dist: arviz>=0.12.1; extra == "all"
-Requires-Dist: scipy<1.13.0; extra == "all"
 Requires-Dist: aesara>=2.8.6; extra == "all"
 Requires-Dist: pymc>=4.2.1; extra == "all"
 Requires-Dist: emcee>=3.0.2; extra == "all"
 Requires-Dist: dynesty>=2.0.3; extra == "all"
 Requires-Dist: nlopt>=2.6.2; extra == "all"
 Requires-Dist: pyswarm>=0.6; extra == "all"
 Requires-Dist: notebook>=6.1.4; extra == "all"
@@ -136,15 +133,14 @@
 Requires-Dist: pyswarms>=1.3.0; extra == "pyswarms"
 Provides-Extra: fides
 Requires-Dist: fides>=0.6.1; extra == "fides"
 Provides-Extra: mpi
 Requires-Dist: mpi4py>=3.0.3; extra == "mpi"
 Provides-Extra: pymc
 Requires-Dist: arviz>=0.12.1; extra == "pymc"
-Requires-Dist: scipy<1.13.0; extra == "pymc"
 Requires-Dist: aesara>=2.8.6; extra == "pymc"
 Requires-Dist: pymc>=4.2.1; extra == "pymc"
 Provides-Extra: aesara
 Requires-Dist: aesara>=2.0.5; extra == "aesara"
 Provides-Extra: jax
 Requires-Dist: jax>=0.4.1; extra == "jax"
 Requires-Dist: jaxlib>=0.4.1; extra == "jax"
@@ -169,15 +165,14 @@
 Requires-Dist: ipython>=8.4.0; extra == "doc"
 Requires-Dist: myst-parser>=0.18.0; extra == "doc"
 Requires-Dist: ipykernel==6.23.1; extra == "doc"
 Requires-Dist: julia>=0.5.7; extra == "doc"
 Requires-Dist: ipython>=8.4.0; extra == "doc"
 Requires-Dist: pygments>=2.12.0; extra == "doc"
 Requires-Dist: arviz>=0.12.1; extra == "doc"
-Requires-Dist: scipy<1.13.0; extra == "doc"
 Requires-Dist: aesara>=2.8.6; extra == "doc"
 Requires-Dist: pymc>=4.2.1; extra == "doc"
 Requires-Dist: emcee>=3.0.2; extra == "doc"
 Requires-Dist: dynesty>=2.0.3; extra == "doc"
 Requires-Dist: nlopt>=2.6.2; extra == "doc"
 Requires-Dist: pyswarm>=0.6; extra == "doc"
 Requires-Dist: notebook>=6.1.4; extra == "doc"
@@ -191,15 +186,14 @@
 Requires-Dist: jaxlib>=0.4.1; extra == "doc"
 Requires-Dist: libroadrunner>=2.6.0; extra == "doc"
 Provides-Extra: example
 Requires-Dist: julia>=0.5.7; extra == "example"
 Requires-Dist: ipython>=8.4.0; extra == "example"
 Requires-Dist: pygments>=2.12.0; extra == "example"
 Requires-Dist: arviz>=0.12.1; extra == "example"
-Requires-Dist: scipy<1.13.0; extra == "example"
 Requires-Dist: aesara>=2.8.6; extra == "example"
 Requires-Dist: pymc>=4.2.1; extra == "example"
 Requires-Dist: emcee>=3.0.2; extra == "example"
 Requires-Dist: dynesty>=2.0.3; extra == "example"
 Requires-Dist: nlopt>=2.6.2; extra == "example"
 Requires-Dist: pyswarm>=0.6; extra == "example"
 Requires-Dist: notebook>=6.1.4; extra == "example"
@@ -236,20 +230,23 @@
 * Interface to [AMICI](https://github.com/AMICI-dev/AMICI/) for efficient
   simulation and sensitivity analysis of ordinary differential equation (ODE)
   models
   ([example](https://github.com/ICB-DCM/pyPESTO/blob/main/doc/example/amici.ipynb))
 * Parameter estimation pipeline for systems biology problems specified in
   [SBML](http://sbml.org/) and [PEtab](https://github.com/PEtab-dev/PEtab)
   ([example](https://github.com/ICB-DCM/pyPESTO/blob/master/doc/example/petab_import.ipynb))
+* Parameter estimation with relative (scaled and offset) data as described in
+  [Schmiester et al. (2020)](https://doi.org/10.1093/bioinformatics/btz581).
+  ([example](https://github.com/ICB-DCM/pyPESTO/blob/master/doc/example/relative_data.ipynb))
 * Parameter estimation with ordinal data as described in
   [Schmiester et al. (2020)](https://doi.org/10.1007/s00285-020-01522-w) and
   [Schmiester et al. (2021)](https://doi.org/10.1093/bioinformatics/btab512).
-  ([example](https://github.com/ICB-DCM/pyPESTO/blob/master/doc/example/ordinal.ipynb))
-* Parameter estimation with censored data. ([example](https://github.com/ICB-DCM/pyPESTO/blob/master/doc/example/censored.ipynb))
-* Parameter estimation with nonlinear-monotone data. ([example](https://github.com/ICB-DCM/pyPESTO/blob/master/doc/example/nonlinear_monotone.ipynb))
+  ([example](https://github.com/ICB-DCM/pyPESTO/blob/master/doc/example/ordinal_data.ipynb))
+* Parameter estimation with censored data. ([example](https://github.com/ICB-DCM/pyPESTO/blob/master/doc/example/censored_data.ipynb))
+* Parameter estimation with nonlinear-monotone data. ([example](https://github.com/ICB-DCM/pyPESTO/blob/master/doc/example/semiquantitative_data.ipynb))
 
 ## Quick install
 
 The simplest way to install **pyPESTO** is via pip:
 
 ```shell
 pip3 install pypesto
```

### Comparing `pypesto-0.5.1/README.md` & `pypesto-0.5.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -21,20 +21,23 @@
 * Interface to [AMICI](https://github.com/AMICI-dev/AMICI/) for efficient
   simulation and sensitivity analysis of ordinary differential equation (ODE)
   models
   ([example](https://github.com/ICB-DCM/pyPESTO/blob/main/doc/example/amici.ipynb))
 * Parameter estimation pipeline for systems biology problems specified in
   [SBML](http://sbml.org/) and [PEtab](https://github.com/PEtab-dev/PEtab)
   ([example](https://github.com/ICB-DCM/pyPESTO/blob/master/doc/example/petab_import.ipynb))
+* Parameter estimation with relative (scaled and offset) data as described in
+  [Schmiester et al. (2020)](https://doi.org/10.1093/bioinformatics/btz581).
+  ([example](https://github.com/ICB-DCM/pyPESTO/blob/master/doc/example/relative_data.ipynb))
 * Parameter estimation with ordinal data as described in
   [Schmiester et al. (2020)](https://doi.org/10.1007/s00285-020-01522-w) and
   [Schmiester et al. (2021)](https://doi.org/10.1093/bioinformatics/btab512).
-  ([example](https://github.com/ICB-DCM/pyPESTO/blob/master/doc/example/ordinal.ipynb))
-* Parameter estimation with censored data. ([example](https://github.com/ICB-DCM/pyPESTO/blob/master/doc/example/censored.ipynb))
-* Parameter estimation with nonlinear-monotone data. ([example](https://github.com/ICB-DCM/pyPESTO/blob/master/doc/example/nonlinear_monotone.ipynb))
+  ([example](https://github.com/ICB-DCM/pyPESTO/blob/master/doc/example/ordinal_data.ipynb))
+* Parameter estimation with censored data. ([example](https://github.com/ICB-DCM/pyPESTO/blob/master/doc/example/censored_data.ipynb))
+* Parameter estimation with nonlinear-monotone data. ([example](https://github.com/ICB-DCM/pyPESTO/blob/master/doc/example/semiquantitative_data.ipynb))
 
 ## Quick install
 
 The simplest way to install **pyPESTO** is via pip:
 
 ```shell
 pip3 install pypesto
```

### Comparing `pypesto-0.5.1/pypesto/C.py` & `pypesto-0.5.2/pypesto/C.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/__init__.py` & `pypesto-0.5.2/pypesto/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/engine/base.py` & `pypesto-0.5.2/pypesto/engine/base.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/engine/mpi_pool.py` & `pypesto-0.5.2/pypesto/engine/mpi_pool.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/engine/multi_process.py` & `pypesto-0.5.2/pypesto/engine/multi_process.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/engine/multi_thread.py` & `pypesto-0.5.2/pypesto/engine/multi_thread.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/engine/single_core.py` & `pypesto-0.5.2/pypesto/engine/single_core.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/ensemble/__init__.py` & `pypesto-0.5.2/pypesto/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/ensemble/covariance_analysis.py` & `pypesto-0.5.2/pypesto/ensemble/covariance_analysis.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/ensemble/dimension_reduction.py` & `pypesto-0.5.2/pypesto/ensemble/dimension_reduction.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/ensemble/ensemble.py` & `pypesto-0.5.2/pypesto/ensemble/ensemble.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/ensemble/task.py` & `pypesto-0.5.2/pypesto/ensemble/task.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/ensemble/util.py` & `pypesto-0.5.2/pypesto/ensemble/util.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/hierarchical/__init__.py` & `pypesto-0.5.2/pypesto/hierarchical/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/hierarchical/base_parameter.py` & `pypesto-0.5.2/pypesto/hierarchical/base_parameter.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/hierarchical/base_problem.py` & `pypesto-0.5.2/pypesto/hierarchical/base_problem.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/hierarchical/base_solver.py` & `pypesto-0.5.2/pypesto/hierarchical/base_solver.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/hierarchical/inner_calculator_collector.py` & `pypesto-0.5.2/pypesto/hierarchical/inner_calculator_collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     filter_return_dict,
     init_return_values,
 )
 
 try:
     import amici
     import petab
-    from amici.parameter_mapping import ParameterMapping
+    from amici.petab.parameter_mapping import ParameterMapping
 except ImportError:
     petab = None
     ParameterMapping = None
 
 from .ordinal import OrdinalCalculator, OrdinalInnerSolver, OrdinalProblem
 from .relative import RelativeAmiciCalculator, RelativeInnerProblem
 from .semiquantitative import (
@@ -321,15 +321,15 @@
             Ids of optimization parameters.
         parameter_mapping:
             Mapping of optimization to simulation parameters.
         fim_for_hess:
             Whether to use the FIM (if available) instead of the Hessian (if
             requested).
         """
-        import amici.parameter_mapping
+        from amici.petab.conditions import fill_in_parameters
 
         if mode == MODE_RES and any(
             data_type in self.data_types
             for data_type in [ORDINAL, CENSORED, SEMIQUANTITATIVE]
         ):
             raise NotImplementedError(
                 f"Mode {mode} is not implemented for ordinal, censored or semi-quantitative data. "
@@ -399,15 +399,15 @@
             sensi_order = max(sensi_orders)
 
         amici_solver.setSensitivityOrder(sensi_order)
 
         x_dct = copy.deepcopy(x_dct)
         x_dct.update(self.necessary_par_dummy_values)
         # fill in parameters
-        amici.parameter_mapping.fill_in_parameters(
+        fill_in_parameters(
             edatas=edatas,
             problem_parameters=x_dct,
             scaled_parameters=True,
             parameter_mapping=parameter_mapping,
             amici_model=amici_model,
         )
```

### Comparing `pypesto-0.5.1/pypesto/hierarchical/ordinal/__init__.py` & `pypesto-0.5.2/pypesto/hierarchical/ordinal/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/hierarchical/ordinal/calculator.py` & `pypesto-0.5.2/pypesto/hierarchical/ordinal/calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,16 @@
     init_return_values,
 )
 from .problem import OrdinalProblem
 from .solver import OrdinalInnerSolver
 
 try:
     import amici
-    from amici.parameter_mapping import ParameterMapping
+    from amici.petab.conditions import fill_in_parameters
+    from amici.petab.parameter_mapping import ParameterMapping
 except ImportError:
     pass
 
 
 class OrdinalCalculator(AmiciCalculator):
     """A calculator is passed as `calculator` to the pypesto.AmiciObjective.
 
@@ -151,15 +152,15 @@
         # If AMICI ReturnData is not provided, we need to simulate the model
         if rdatas is None:
             amici_solver.setSensitivityOrder(sensi_order)
 
             x_dct = copy.deepcopy(x_dct)
 
             # fill in parameters
-            amici.parameter_mapping.fill_in_parameters(
+            fill_in_parameters(
                 edatas=edatas,
                 problem_parameters=x_dct,
                 scaled_parameters=True,
                 parameter_mapping=parameter_mapping,
                 amici_model=amici_model,
             )
             # run amici simulation
```

### Comparing `pypesto-0.5.1/pypesto/hierarchical/ordinal/parameter.py` & `pypesto-0.5.2/pypesto/hierarchical/ordinal/parameter.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/hierarchical/ordinal/problem.py` & `pypesto-0.5.2/pypesto/hierarchical/ordinal/problem.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/hierarchical/ordinal/solver.py` & `pypesto-0.5.2/pypesto/hierarchical/ordinal/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     InnerParameterType,
 )
 from ..base_solver import InnerSolver
 from .parameter import OrdinalParameter
 from .problem import OrdinalProblem
 
 try:
-    from amici.parameter_mapping import ParameterMapping
+    from amici.petab.parameter_mapping import ParameterMapping
 except ImportError:
     pass
 
 
 class OrdinalInnerSolver(InnerSolver):
     """Solve the inner subproblem of the optimal scaling approach for ordinal data.
```

### Comparing `pypesto-0.5.1/pypesto/hierarchical/petab.py` & `pypesto-0.5.2/pypesto/hierarchical/petab.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/hierarchical/relative/__init__.py` & `pypesto-0.5.2/pypesto/hierarchical/relative/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/hierarchical/relative/calculator.py` & `pypesto-0.5.2/pypesto/hierarchical/relative/calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import copy
 from collections.abc import Sequence
 
 import numpy as np
 
 try:
     import amici
-    import amici.parameter_mapping
-    from amici.parameter_mapping import ParameterMapping
+    from amici.petab.conditions import fill_in_parameters
+    from amici.petab.parameter_mapping import ParameterMapping
 except ImportError:
     pass
 
 from ...C import (
     AMICI_SIGMAY,
     AMICI_SSIGMAY,
     AMICI_SY,
@@ -292,15 +292,15 @@
             sensi_order = max(sensi_orders)
 
         # if AMICI ReturnData is not provided, we need to simulate the model
         if rdatas is None:
             amici_solver.setSensitivityOrder(sensi_order)
             x_dct.update(self.inner_problem.get_dummy_values(scaled=True))
             # fill in parameters
-            amici.parameter_mapping.fill_in_parameters(
+            fill_in_parameters(
                 edatas=edatas,
                 problem_parameters=x_dct,
                 scaled_parameters=True,
                 parameter_mapping=parameter_mapping,
                 amici_model=amici_model,
             )
             # run amici simulation
```

### Comparing `pypesto-0.5.1/pypesto/hierarchical/relative/problem.py` & `pypesto-0.5.2/pypesto/hierarchical/relative/problem.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/hierarchical/relative/solver.py` & `pypesto-0.5.2/pypesto/hierarchical/relative/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     compute_optimal_offset_coupled,
     compute_optimal_scaling,
     compute_optimal_sigma,
 )
 
 try:
     import amici
-    from amici.parameter_mapping import ParameterMapping
+    from amici.petab.parameter_mapping import ParameterMapping
 except ImportError:
     pass
 
 
 class RelativeInnerSolver(InnerSolver):
     """Base class for the relative inner solver."""
 
@@ -78,15 +78,15 @@
         for x in problem.get_xs_for_type(InnerParameterType.SIGMA):
             apply_sigma(
                 sigma_value=inner_parameters[x.inner_parameter_id],
                 sigma=sigma,
                 mask=x.ixs,
             )
 
-        return compute_nllh(relevant_data, sim, sigma)
+        return compute_nllh(relevant_data, sim, sigma, problem.data_mask)
 
     def calculate_gradients(
         self,
         problem: InnerProblem,
         sim: list[np.ndarray],
         ssim: list[np.ndarray],
         sigma: list[np.ndarray],
@@ -498,15 +498,15 @@
                     apply_sigma(x_val, _sigma, mask)
                 else:
                     raise ValueError(
                         "Can't handle parameter type "
                         f"`{par.inner_parameter_type}`."
                     )
 
-            return compute_nllh(_data, _sim, _sigma)
+            return compute_nllh(_data, _sim, _sigma, problem.data_mask)
 
         # TODO gradient
         objective = Objective(fun)
 
         # optimization problem
         pypesto_problem = Problem(
             objective, lb=lb, ub=ub, x_names=x_names, **self.problem_kwargs
```

### Comparing `pypesto-0.5.1/pypesto/hierarchical/relative/util.py` & `pypesto-0.5.2/pypesto/hierarchical/relative/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -358,14 +358,19 @@
     # Make all non-masked data and sim nan's in the original one
     relevant_data = copy.deepcopy(data)
     relevant_sim = copy.deepcopy(sim)
     for i in range(len(data)):
         relevant_data[i][~s.ixs[i]] = np.nan
         relevant_sim[i][~s.ixs[i]] = np.nan
 
+    # Get relevant data mask
+    relevant_data_mask = []
+    for i in range(len(data)):
+        relevant_data_mask.append(~np.isnan(relevant_data[i]))
+
     # Get bounds
     s_bounds = s.get_bounds()
     b_bounds = b.get_bounds()
 
     # Get unsatisfied bounds
     s_unsatisfied = s.get_unsatisfied_bound(s_opt_value)
     b_unsatisfied = b.get_unsatisfied_bound(b_opt_value)
@@ -403,14 +408,15 @@
             compute_nllh(
                 data=relevant_data,
                 sim=[
                     sim_i * candidate_point[0] + candidate_point[1]
                     for sim_i in relevant_sim
                 ],
                 sigma=sigma,
+                data_mask=relevant_data_mask,
             )
             for candidate_point in candidate_points
         ]
         # The constrained solution is the candidate point with the lowest
         # objective value
         constrained_solution = candidate_points[
             np.argmin(candidate_objective_values)
@@ -443,26 +449,39 @@
             b_bounds[b_unsatisfied],
         )
 
     return constrained_solution
 
 
 def compute_nllh(
-    data: list[np.ndarray], sim: list[np.ndarray], sigma: list[np.ndarray]
+    data: list[np.ndarray],
+    sim: list[np.ndarray],
+    sigma: list[np.ndarray],
+    data_mask: list[np.ndarray],
 ) -> float:
     """Compute negative log-likelihood.
 
     Compute negative log-likelihood of the data, given the model outputs and
     sigmas.
     """
-    return sum(
-        0.5 * np.nansum(np.log(2 * np.pi * sigma_i**2))
-        + 0.5 * np.nansum((data_i - sim_i) ** 2 / sigma_i**2)
-        for data_i, sim_i, sigma_i in zip(data, sim, sigma)
-    )
+    nllh = 0.0
+    for data_i, sim_i, sigma_i, data_mask_i in zip(
+        data, sim, sigma, data_mask
+    ):
+        # Mask the data, sim and sigma
+        data_i = data_i[data_mask_i]
+        sim_i = sim_i[data_mask_i]
+        sigma_i = sigma_i[data_mask_i]
+
+        # Compute the negative log-likelihood
+        nllh += 0.5 * np.nansum(
+            np.log(2 * np.pi * sigma_i**2)
+        ) + 0.5 * np.nansum((data_i - sim_i) ** 2 / sigma_i**2)
+
+    return nllh
 
 
 def compute_nllh_gradient_for_condition(
     data: np.ndarray,
     sim: np.ndarray,
     sigma: np.ndarray,
     ssim: np.ndarray,
```

### Comparing `pypesto-0.5.1/pypesto/hierarchical/semiquantitative/__init__.py` & `pypesto-0.5.2/pypesto/hierarchical/semiquantitative/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/hierarchical/semiquantitative/calculator.py` & `pypesto-0.5.2/pypesto/hierarchical/semiquantitative/calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
     init_return_values,
 )
 from .problem import SemiquantProblem
 from .solver import SemiquantInnerSolver
 
 try:
     import amici
-    from amici.parameter_mapping import ParameterMapping
+    from amici.petab.conditions import fill_in_parameters
+    from amici.petab.parameter_mapping import ParameterMapping
 except ImportError:
     pass
 
 
 class SemiquantCalculator(AmiciCalculator):
     """A calculator is passed as `calculator` to the pypesto.AmiciObjective.
 
@@ -150,15 +151,15 @@
 
             x_dct = copy.deepcopy(x_dct)
             x_dct.update(
                 self.inner_problem.get_noise_dummy_values(scaled=True)
             )
 
             # fill in parameters
-            amici.parameter_mapping.fill_in_parameters(
+            fill_in_parameters(
                 edatas=edatas,
                 problem_parameters=x_dct,
                 scaled_parameters=True,
                 parameter_mapping=parameter_mapping,
                 amici_model=amici_model,
             )
             # run amici simulation
```

### Comparing `pypesto-0.5.1/pypesto/hierarchical/semiquantitative/parameter.py` & `pypesto-0.5.2/pypesto/hierarchical/semiquantitative/parameter.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/hierarchical/semiquantitative/problem.py` & `pypesto-0.5.2/pypesto/hierarchical/semiquantitative/problem.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/hierarchical/semiquantitative/solver.py` & `pypesto-0.5.2/pypesto/hierarchical/semiquantitative/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     InnerParameterType,
 )
 from ..base_solver import InnerSolver
 from .parameter import SplineInnerParameter
 from .problem import SemiquantProblem
 
 try:
-    from amici.parameter_mapping import ParameterMapping
+    from amici.petab.parameter_mapping import ParameterMapping
 except ImportError:
     pass
 
 
 class SemiquantInnerSolver(InnerSolver):
     """Solver of the inner subproblem of spline approximation for nonlinear-monotone data.
```

### Comparing `pypesto-0.5.1/pypesto/history/__init__.py` & `pypesto-0.5.2/pypesto/history/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/history/amici.py` & `pypesto-0.5.2/pypesto/history/amici.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,26 @@
         id: str,
         file: Union[str, Path],
         options: Union[HistoryOptions, dict, None] = None,
     ):
         super().__init__(id, file, options=options)
 
     @staticmethod
+    def load(
+        id: str,
+        file: Union[str, Path],
+        options: Union[HistoryOptions, dict] = None,
+    ) -> "Hdf5AmiciHistory":
+        """Load the History object from memory."""
+        history = Hdf5AmiciHistory(id=id, file=file, options=options)
+        if options is None:
+            history.recover_options(file)
+        return history
+
+    @staticmethod
     def _simulation_to_values(x, result, used_time):
         values = Hdf5History._simulation_to_values(x, result, used_time)
         # default unit for time in amici is [ms], converted to [s]
         values |= {
             key: sum([rdata[key] for rdata in result[RDATAS]]) * 0.001
             for key in (
                 CPU_TIME_TOTAL,
```

### Comparing `pypesto-0.5.1/pypesto/history/base.py` & `pypesto-0.5.2/pypesto/history/base.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/history/csv.py` & `pypesto-0.5.2/pypesto/history/csv.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/history/generate.py` & `pypesto-0.5.2/pypesto/history/generate.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/history/hdf5.py` & `pypesto-0.5.2/pypesto/history/hdf5.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/history/memory.py` & `pypesto-0.5.2/pypesto/history/memory.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/history/optimizer.py` & `pypesto-0.5.2/pypesto/history/optimizer.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/history/options.py` & `pypesto-0.5.2/pypesto/history/options.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/history/util.py` & `pypesto-0.5.2/pypesto/history/util.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/logging.py` & `pypesto-0.5.2/pypesto/logging.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/objective/aesara/base.py` & `pypesto-0.5.2/pypesto/objective/aesara/base.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/objective/aggregated.py` & `pypesto-0.5.2/pypesto/objective/aggregated.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/objective/amici/amici.py` & `pypesto-0.5.2/pypesto/objective/amici/amici.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/objective/amici/amici_calculator.py` & `pypesto-0.5.2/pypesto/objective/amici/amici_calculator.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/objective/amici/amici_util.py` & `pypesto-0.5.2/pypesto/objective/amici/amici_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     ModeType,
 )
 from ...logging import log_level_active
 
 if TYPE_CHECKING:
     try:
         import amici
-        from amici.parameter_mapping import (
+        from amici.petab.parameter_mapping import (
             ParameterMapping,
             ParameterMappingForCondition,
         )
     except ImportError:
         ParameterMapping = ParameterMappingForCondition = None
 
 AmiciModel = Union["amici.Model", "amici.ModelPtr"]
@@ -120,31 +120,33 @@
 ) -> ParameterMapping:
     """Create a dummy identity parameter mapping table.
 
     This fills in only the dynamic parameters. Values for fixed parameters,
     both in preequilibration and simulation, are assumed to be provided
     correctly in model or edatas already.
     """
-    import amici.parameter_mapping
+    from amici.petab.parameter_mapping import (
+        ParameterMapping,
+        ParameterMappingForCondition,
+        amici_to_petab_scale,
+    )
 
     x_ids = list(amici_model.getParameterIds())
     x_scales = list(amici_model.getParameterScale())
-    parameter_mapping = amici.parameter_mapping.ParameterMapping()
+    parameter_mapping = ParameterMapping()
     for _ in range(n_conditions):
         condition_map_sim_var = {x_id: x_id for x_id in x_ids}
         condition_scale_map_sim_var = {
-            x_id: amici.parameter_mapping.amici_to_petab_scale(x_scale)
+            x_id: amici_to_petab_scale(x_scale)
             for x_id, x_scale in zip(x_ids, x_scales)
         }
         # assumes fixed parameters are filled in already
-        mapping_for_condition = (
-            amici.parameter_mapping.ParameterMappingForCondition(
-                map_sim_var=condition_map_sim_var,
-                scale_map_sim_var=condition_scale_map_sim_var,
-            )
+        mapping_for_condition = ParameterMappingForCondition(
+            map_sim_var=condition_map_sim_var,
+            scale_map_sim_var=condition_scale_map_sim_var,
         )
 
         parameter_mapping.append(mapping_for_condition)
     return parameter_mapping
 
 
 def par_index_slices(
```

### Comparing `pypesto-0.5.1/pypesto/objective/base.py` & `pypesto-0.5.2/pypesto/objective/base.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/objective/finite_difference.py` & `pypesto-0.5.2/pypesto/objective/finite_difference.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/objective/function.py` & `pypesto-0.5.2/pypesto/objective/function.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/objective/jax/base.py` & `pypesto-0.5.2/pypesto/objective/jax/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Adds an interface for the construction of loss functions
 incorporating jax models. This permits computation of derivatives using a
 combination of objective based methods and jax based autodiff.
 """
 
 import copy
 from functools import partial
-from typing import Union
+from typing import Callable, Union
 
 import numpy as np
 
 from ...C import MODE_FUN, ModeType
 from ..base import ObjectiveBase, ResultDict
 
 try:
@@ -22,59 +22,89 @@
 except ImportError:
     raise ImportError(
         "Using a jax objective requires an installation of "
         "the python package jax. Please install jax via "
         "`pip install jax jaxlib`."
     ) from None
 
+
+def _base_objective_as_jax_array_tuple(func: Callable):
+    def decorator(*args, **kwargs):
+        # make sure return is a tuple of jax arrays
+        results = func(*args, **kwargs)
+        if isinstance(results, tuple):
+            return tuple(jnp.array(r) for r in results)
+        return jnp.array(results)
+
+    return decorator
+
+
 # jax compatible (jit-able) objective function using external callback, see
 # https://jax.readthedocs.io/en/latest/notebooks/external_callbacks.html
 
 
 @partial(custom_jvp, nondiff_argnums=(0,))
-def _device_fun(base_objective: ObjectiveBase, x: jnp.array):
+def _device_fun(base_objective: ObjectiveBase, x: jnp.array) -> jnp.array:
     """Jax compatible objective function execution using external callback.
 
     Parameters
     ----------
     obj:
         The wrapped jax objective.
     x:
         jax computed input array.
+
+    Returns
+    -------
+    fval : jnp.array
+        The function value as 0-dimensional jax array.
     """
     return jax.pure_callback(
-        partial(base_objective, sensi_orders=(0,)),
+        _base_objective_as_jax_array_tuple(
+            partial(base_objective, sensi_orders=(0,))
+        ),
         jax.ShapeDtypeStruct((), x.dtype),
         x,
     )
 
 
-def _device_fun_value_and_grad(base_objective: ObjectiveBase, x: jnp.array):
+def _device_fun_value_and_grad(
+    base_objective: ObjectiveBase, x: jnp.array
+) -> tuple[jnp.array, jnp.array]:
     """Jax compatible objective gradient execution using external callback.
 
     This function will be called when computing the gradient of the
     `JaxObjective` using `jax.grad` or `jax.value_and_grad`. In the latter
     case, the function will return both the function value and the gradient,
     so no caching is necessary. For higher order derivatives, caching would
     be advantageous, but unclear how to implement this.
 
     Parameters
     ----------
     obj:
         The wrapped jax objective.
     x:
         jax computed input array.
+
+    Returns
+    -------
+    fval : jnp.array
+        The function value as 0-dimensional jax array.
+    grad : jnp.array
+        The gradient as jax array.
     """
     return jax.pure_callback(
-        partial(
-            base_objective,
-            sensi_orders=(
-                0,
-                1,
-            ),
+        _base_objective_as_jax_array_tuple(
+            partial(
+                base_objective,
+                sensi_orders=(
+                    0,
+                    1,
+                ),
+            )
         ),
         (
             jax.ShapeDtypeStruct((), x.dtype),
             jax.ShapeDtypeStruct(
                 x.shape,  # bootstrap from cached value
                 x.dtype,
             ),
@@ -108,15 +138,15 @@
     Parameters
     ----------
     objective:
         pyPESTO objective to be wrapped.
 
     Note
     ----
-    Currently only implements MODE_FUN and sensi_orders=(0,). Support for
+    Currently only implements MODE_FUN and sensi_orders<=1. Support for
     MODE_RES should be straightforward to add.
     """
 
     def __init__(
         self,
         objective: ObjectiveBase,
     ):
@@ -139,15 +169,15 @@
     def check_sensi_orders(self, sensi_orders, mode: ModeType) -> bool:
         """See `ObjectiveBase` documentation."""
         if not self.check_mode(mode):
             return False
         else:
             return (
                 self.base_objective.check_sensi_orders(sensi_orders, mode)
-                and max(sensi_orders) == 0
+                and max(sensi_orders) <= 1
             )
 
     def __call__(
         self,
         x: jnp.ndarray,
         sensi_orders: tuple[int, ...] = (0,),
         mode: ModeType = MODE_FUN,
@@ -200,19 +230,24 @@
         other = JaxObjective(
             copy.deepcopy(self.base_objective),
         )
         return other
 
     @property
     def history(self):
-        """Exposes the history of the inner objective."""
+        """Expose the history of the inner objective."""
         return self.base_objective.history
 
     @property
     def pre_post_processor(self):
-        """Exposes the pre_post_processor of inner objective."""
+        """Expose the pre_post_processor of inner objective."""
         return self.base_objective.pre_post_processor
 
+    @pre_post_processor.setter
+    def pre_post_processor(self, new_pre_post_processor):
+        """Set the pre_post_processor of inner objective."""
+        self.base_objective.pre_post_processor = new_pre_post_processor
+
     @property
     def x_names(self):
-        """Exposes the x_names of inner objective."""
+        """Expose the x_names of inner objective."""
         return self.base_objective.x_names
```

### Comparing `pypesto-0.5.1/pypesto/objective/julia/base.py` & `pypesto-0.5.2/pypesto/objective/julia/base.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/objective/julia/petabJl.py` & `pypesto-0.5.2/pypesto/objective/julia/petabJl.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/objective/julia/petab_jl_importer.py` & `pypesto-0.5.2/pypesto/objective/julia/petab_jl_importer.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/objective/pre_post_process.py` & `pypesto-0.5.2/pypesto/objective/pre_post_process.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/objective/priors.py` & `pypesto-0.5.2/pypesto/objective/priors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 import math
 from collections.abc import Sequence
-from copy import deepcopy
 from typing import Callable, Union
 
 import numpy as np
 
 from .. import C
 from .aggregated import AggregatedObjective
 from .base import ResultDict
@@ -64,19 +63,14 @@
             Format see above.
         x_names:
             Sequence of parameter names (optional).
         """
         self.prior_list = prior_list
         super().__init__(x_names)
 
-    def __deepcopy__(self, memodict=None):
-        """Create deepcopy of object."""
-        other = NegLogParameterPriors(deepcopy(self.prior_list))
-        return other
-
     def call_unprocessed(
         self,
         x: np.ndarray,
         sensi_orders: tuple[int, ...],
         mode: C.ModeType,
         **kwargs,
     ) -> ResultDict:
```

### Comparing `pypesto-0.5.1/pypesto/objective/roadrunner/petab_importer_roadrunner.py` & `pypesto-0.5.2/pypesto/objective/roadrunner/petab_importer_roadrunner.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/objective/roadrunner/road_runner.py` & `pypesto-0.5.2/pypesto/objective/roadrunner/road_runner.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/objective/roadrunner/roadrunner_calculator.py` & `pypesto-0.5.2/pypesto/objective/roadrunner/roadrunner_calculator.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/objective/roadrunner/utils.py` & `pypesto-0.5.2/pypesto/objective/roadrunner/utils.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/optimize/__init__.py` & `pypesto-0.5.2/pypesto/optimize/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/optimize/ess/ess.py` & `pypesto-0.5.2/pypesto/optimize/ess/ess.py`

 * *Files 1% similar despite different names*

```diff
@@ -643,13 +643,13 @@
         with np.printoptions(
             edgeitems=5,
             threshold=10,
             linewidth=100000,
             formatter={"float": lambda x: "%.3g" % x},
         ):
             self.logger.info(
-                f"-- Final ESS fval after {self.n_iter} "
-                f"iterations: {self.fx_best}. "
+                f"-- Final ESS fval after {self.n_iter} iterations, "
+                f"{self.evaluator.n_eval} function evaluations: {self.fx_best}. "
                 f"Exit flag: {self.exit_flag.name}. "
                 f"Num local solutions: {len(self.local_solutions)}."
             )
             self.logger.debug(f"Final refset: {np.sort(self.refset.fx)} ")
```

### Comparing `pypesto-0.5.1/pypesto/optimize/ess/function_evaluator.py` & `pypesto-0.5.2/pypesto/optimize/ess/function_evaluator.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/optimize/ess/refset.py` & `pypesto-0.5.2/pypesto/optimize/ess/refset.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/optimize/ess/sacess.py` & `pypesto-0.5.2/pypesto/optimize/ess/sacess.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import itertools
 import logging
 import logging.handlers
 import multiprocessing
 import os
 import time
+from dataclasses import dataclass
 from math import ceil, sqrt
 from multiprocessing import get_context
 from multiprocessing.managers import SyncManager
 from pathlib import Path
 from typing import Any, Callable, Optional, Union
 from uuid import uuid1
 from warnings import warn
@@ -124,14 +125,15 @@
                 f"{self.__class__.__name__} needs at least 2 workers."
             )
         self.ess_init_args = ess_init_args
         self.max_walltime_s = max_walltime_s
         self.exit_flag = ESSExitFlag.DID_NOT_RUN
         self.ess_loglevel = ess_loglevel
         self.sacess_loglevel = sacess_loglevel
+        self.worker_results: list[SacessWorkerResult] = []
         logger.setLevel(self.sacess_loglevel)
 
         self._tmpdir = tmpdir
         if self._tmpdir is None:
             while self._tmpdir is None or self._tmpdir.exists():
                 self._tmpdir = Path(f"SacessOptimizerTemp-{str(uuid1())[:8]}")
         self._tmpdir = Path(self._tmpdir).absolute()
@@ -245,29 +247,37 @@
 
             # start logging thread only AFTER starting the worker processes
             #  to prevent deadlocks
             logging_thread.start()
 
             # wait for finish
             # collect results
-            histories = [
+            self.worker_results = [
                 sacess_manager._result_queue.get()
                 for _ in range(self.num_workers)
             ]
-            self.histories = histories
             for p in worker_processes:
                 p.join()
 
         logging_thread.stop()
+
+        self.histories = [
+            worker_result.history for worker_result in self.worker_results
+        ]
+
         result = self._create_result(problem)
 
         walltime = time.time() - start_time
+        n_eval_total = sum(
+            worker_result.n_eval for worker_result in self.worker_results
+        )
         logger.info(
-            f"{self.__class__.__name__} stopped after {walltime:3g}s with global best "
-            f"{result.optimize_result[0].fval}."
+            f"{self.__class__.__name__} stopped after {walltime:3g}s "
+            f"and {n_eval_total} objective evaluations "
+            f"with global best {result.optimize_result[0].fval}."
         )
 
         return result
 
     def _create_result(self, problem: Problem) -> pypesto.Result:
         """Create result object.
 
@@ -441,18 +451,23 @@
                 self._worker_scores[sender_idx] = (
                     self._worker_comms[sender_idx] * elapsed_time_s
                 )
             else:
                 # reject solution
                 self._rejections.value += 1
 
+                rel_change = (
+                    abs(abs_change / self._best_known_fx.value)
+                    if self._best_known_fx.value != 0
+                    else np.nan
+                )
                 self._logger.debug(
                     f"Rejected solution from worker {sender_idx} "
                     f"abs change: {abs_change} "
-                    f"rel change: {abs(abs_change / self._best_known_fx.value):.4g} "
+                    f"rel change: {rel_change:.4g} "
                     f"(threshold: {self._rejection_threshold.value}) "
                     f"(total rejections: {self._rejections.value})."
                 )
                 # adapt acceptance threshold if too many solutions have been
                 #  rejected
                 if self._rejections.value > self._num_workers:
                     self._rejection_threshold.value /= 2
@@ -573,19 +588,28 @@
             self._best_known_fx = min(ess.fx_best, self._best_known_fx)
 
             self._cooperate()
             self._maybe_adapt(problem)
 
             self._logger.info(
                 f"sacess worker {self._worker_idx} iteration {ess.n_iter} "
-                f"(best: {self._best_known_fx})."
+                f"(best: {self._best_known_fx}, "
+                f"n_eval: {ess.evaluator.n_eval})."
             )
 
         ess.history.finalize(exitflag=ess.exit_flag.name)
-        self._manager._result_queue.put(ess.history)
+        worker_result = SacessWorkerResult(
+            x=ess.x_best,
+            fx=ess.fx_best,
+            history=ess.history,
+            n_eval=ess.evaluator.n_eval,
+            n_iter=ess.n_iter,
+            exit_flag=ess.exit_flag,
+        )
+        self._manager._result_queue.put(worker_result)
         ess._report_final()
 
     def _setup_ess(self, startpoint_method: StartpointMethod) -> ESSOptimizer:
         """Run ESS."""
         ess_kwargs = self._ess_kwargs.copy()
         # account for sacess walltime limit
         ess_kwargs["max_walltime_s"] = min(
@@ -646,18 +670,21 @@
             self._logger.debug(
                 f"Updated settings on worker {self._worker_idx} to "
                 f"{self._ess_kwargs}"
             )
 
     def maybe_update_best(self, x: np.array, fx: float):
         """Maybe update the best known solution and send it to the manager."""
+        rel_change = (
+            abs((fx - self._best_known_fx) / fx) if fx != 0 else np.nan
+        )
         self._logger.debug(
             f"Worker {self._worker_idx} maybe sending solution {fx}. "
             f"best known: {self._best_known_fx}, "
-            f"rel change: {(fx - self._best_known_fx) / fx:.4g}, "
+            f"rel change: {rel_change:.4g}, "
             f"threshold: {self._acceptance_threshold}"
         )
 
         # solution improves best value by at least a factor of ...
         if (
             (np.isfinite(fx) and not np.isfinite(self._best_known_fx))
             or (self._best_known_fx == 0 and fx < 0)
@@ -1012,7 +1039,39 @@
             options[FidesOptions.MAXITER] = int(max_eval)
         return pypesto.optimize.FidesOptimizer(
             **self._fides_kwargs, options=options
         )
 
     def __repr__(self):
         return f"{self.__class__.__name__}(fides_options={self._fides_options}, fides_kwargs={self._fides_kwargs})"
+
+
+@dataclass
+class SacessWorkerResult:
+    """Container for :class:`SacessWorker` results.
+
+    Contains various information about the optimization process of a single
+    :class:`SacessWorker` instance that is to be sent to
+    :class:`SacessOptimizer`.
+
+    Attributes
+    ----------
+    x:
+        Best parameters found.
+    fx:
+        Objective value corresponding to ``x``.
+    n_eval:
+        Number of objective evaluations performed.
+    n_iter:
+        Number of scatter search iterations performed.
+    history:
+        History object containing information about the optimization process.
+    exit_flag:
+        Exit flag of the optimization process.
+    """
+
+    x: np.array
+    fx: float
+    n_eval: int
+    n_iter: int
+    history: "pypesto.history.memory.MemoryHistory"
+    exit_flag: ESSExitFlag
```

### Comparing `pypesto-0.5.1/pypesto/optimize/load.py` & `pypesto-0.5.2/pypesto/optimize/load.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/optimize/optimize.py` & `pypesto-0.5.2/pypesto/optimize/optimize.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/optimize/optimizer.py` & `pypesto-0.5.2/pypesto/optimize/optimizer.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/optimize/options.py` & `pypesto-0.5.2/pypesto/optimize/options.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/optimize/task.py` & `pypesto-0.5.2/pypesto/optimize/task.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/optimize/util.py` & `pypesto-0.5.2/pypesto/optimize/util.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/petab/__init__.py` & `pypesto-0.5.2/pypesto/petab/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/petab/importer.py` & `pypesto-0.5.2/pypesto/petab/importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,23 @@
 from typing import (
     Any,
     Callable,
 )
 
 import numpy as np
 import pandas as pd
+import petab
+from petab.C import (
+    ESTIMATE,
+    NOISE_PARAMETERS,
+    OBSERVABLE_ID,
+    PREEQUILIBRATION_CONDITION_ID,
+    SIMULATION_CONDITION_ID,
+)
+from petab.models import MODEL_TYPE_SBML
 
 from ..C import (
     CENSORED,
     CENSORING_TYPES,
     CONDITION_SEP,
     MEASUREMENT_TYPE,
     MODE_FUN,
@@ -46,24 +55,15 @@
 
 try:
     import amici
     import amici.petab
     import amici.petab.conditions
     import amici.petab.parameter_mapping
     import amici.petab.simulations
-    import petab
     from amici.petab.import_helpers import check_model
-    from petab.C import (
-        ESTIMATE,
-        NOISE_PARAMETERS,
-        OBSERVABLE_ID,
-        PREEQUILIBRATION_CONDITION_ID,
-        SIMULATION_CONDITION_ID,
-    )
-    from petab.models import MODEL_TYPE_SBML
 except ImportError:
     amici = None
 
 logger = logging.getLogger(__name__)
 
 
 class PetabImporter(AmiciObjectBuilder):
```

### Comparing `pypesto-0.5.1/pypesto/predict/amici_predictor.py` & `pypesto-0.5.2/pypesto/predict/amici_predictor.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/predict/task.py` & `pypesto-0.5.2/pypesto/predict/task.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/problem/base.py` & `pypesto-0.5.2/pypesto/problem/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import copy
 import logging
+import sys
 from collections.abc import Iterable
 from typing import (
     Callable,
     Optional,
     SupportsFloat,
     SupportsInt,
     Union,
@@ -11,14 +12,15 @@
 
 import numpy as np
 import pandas as pd
 
 from ..objective import ObjectiveBase
 from ..objective.priors import NegLogParameterPriors
 from ..startpoint import StartpointMethod, to_startpoint_method, uniform
+from ..version import __version__
 
 SupportsFloatIterableOrValue = Union[Iterable[SupportsFloat], SupportsFloat]
 SupportsIntIterableOrValue = Union[Iterable[SupportsInt], SupportsInt]
 
 logger = logging.getLogger(__name__)
 
 
@@ -160,14 +162,17 @@
         self._check_x_guesses()
 
         # startpoint method
         if startpoint_method is None:
             startpoint_method = uniform
         # convert startpoint method to class instance
         self.startpoint_method = to_startpoint_method(startpoint_method)
+        # save python and pypesto version
+        self.python_version = ".".join(map(str, sys.version_info[:3]))
+        self.pypesto_version = __version__
 
     @property
     def lb(self) -> np.ndarray:
         """Return lower bounds of free parameters."""
         return self.lb_full[self.x_free_indices]
 
     @property
@@ -233,14 +238,23 @@
         self.objective.update_from_problem(
             dim_full=self.dim_full,
             x_free_indices=self.x_free_indices,
             x_fixed_indices=self.x_fixed_indices,
             x_fixed_vals=self.x_fixed_vals,
         )
 
+        # make prior aware of fixed parameters (for sampling etc.)
+        if self.x_priors is not None:
+            self.x_priors.update_from_problem(
+                dim_full=self.dim_full,
+                x_free_indices=self.x_free_indices,
+                x_fixed_indices=self.x_fixed_indices,
+                x_fixed_vals=self.x_fixed_vals,
+            )
+
         # sanity checks
         if len(self.x_scales) != self.dim_full:
             raise AssertionError("x_scales dimension invalid.")
         if len(self.x_names) != self.dim_full:
             raise AssertionError("x_names must be of length dim_full.")
         if len(self.x_fixed_indices) != len(self.x_fixed_vals):
             raise AssertionError(
@@ -328,27 +342,30 @@
                 fixed_x_index = self.x_fixed_indices.index(index)
                 self.x_fixed_indices.pop(fixed_x_index)
                 self.x_fixed_vals.pop(fixed_x_index)
 
         self.normalize()
 
     def get_full_vector(
-        self, x: Union[np.ndarray, None], x_fixed_vals: Iterable[float] = None
+        self,
+        x: Union[np.ndarray, None],
+        x_fixed_vals: Iterable[float] = None,
+        x_is_grad: bool = False,
     ) -> Union[np.ndarray, None]:
         """
         Map vector from dim to dim_full. Usually used for x, grad.
 
         Parameters
         ----------
         x: array_like, shape=(dim,)
             The vector in dimension dim.
         x_fixed_vals: array_like, ndim=1, optional
-            The values to be used for the fixed indices. If None, then nans are
-            inserted. Usually, None will be used for grad and
-            problem.x_fixed_vals for x.
+            The values to be used for the fixed indices. If None and x_is_grad=False, problem.x_fixed_vals is used; for x_is_grad=True, nans are inserted.
+        x_is_grad: bool
+            If true, x is treated as gradients.
         """
         if x is None:
             return None
 
         # make sure it is an array
         x = np.array(x)
 
@@ -358,14 +375,17 @@
         # Note: The funny indexing construct is to handle residual gradients,
         # where the last dimension is assumed to be the parameter one.
         x_full = np.zeros(x.shape[:-1] + (self.dim_full,))
         x_full[:] = np.nan
         x_full[..., self.x_free_indices] = x
         if x_fixed_vals is not None:
             x_full[..., self.x_fixed_indices] = x_fixed_vals
+            return x_full
+        if not x_is_grad:
+            x_full[..., self.x_fixed_indices] = self.x_fixed_vals
         return x_full
 
     def get_full_matrix(
         self, x: Union[np.ndarray, None]
     ) -> Union[np.ndarray, None]:
         """
         Map matrix from dim to dim_full. Usually used for hessian.
@@ -475,14 +495,30 @@
                     ],
                     "lb_full": self.lb_full,
                     "ub_full": self.ub_full,
                 },
             )
         )
 
+    def get_startpoints(self, n_starts: int) -> np.ndarray:
+        """
+        Sample startpoints from method.
+
+        Parameters
+        ----------
+        n_starts:
+            Number of start points.
+
+        Returns
+        -------
+        xs:
+            Start points, shape (n_starts, dim).
+        """
+        return self.startpoint_method(n_starts, self)
+
 
 _convtypes = {
     "float": {"attr": "__float__", "conv": float},
     "int": {"attr": "__int__", "conv": int},
 }
```

### Comparing `pypesto-0.5.1/pypesto/problem/hierarchical.py` & `pypesto-0.5.2/pypesto/problem/hierarchical.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/profile/approximate.py` & `pypesto-0.5.2/pypesto/profile/approximate.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/profile/options.py` & `pypesto-0.5.2/pypesto/profile/options.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/profile/profile.py` & `pypesto-0.5.2/pypesto/profile/profile.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/profile/profile_next_guess.py` & `pypesto-0.5.2/pypesto/profile/profile_next_guess.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/profile/task.py` & `pypesto-0.5.2/pypesto/profile/task.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/profile/util.py` & `pypesto-0.5.2/pypesto/profile/util.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/profile/validation_intervals.py` & `pypesto-0.5.2/pypesto/profile/validation_intervals.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/profile/walk_along_profile.py` & `pypesto-0.5.2/pypesto/profile/walk_along_profile.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/result/optimize.py` & `pypesto-0.5.2/pypesto/result/optimize.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,18 +187,18 @@
 
         Parameters
         ----------
         problem:
             problem which contains info about how to convert to full vectors
             or matrices
         """
-        self.x = problem.get_full_vector(self.x, problem.x_fixed_vals)
-        self.grad = problem.get_full_vector(self.grad)
+        self.x = problem.get_full_vector(self.x)
+        self.grad = problem.get_full_vector(self.grad, x_is_grad=True)
         self.hess = problem.get_full_matrix(self.hess)
-        self.x0 = problem.get_full_vector(self.x0, problem.x_fixed_vals)
+        self.x0 = problem.get_full_vector(self.x0)
         self.free_indices = np.array(problem.x_free_indices)
 
 
 class OptimizeResult:
     """Result of the :py:func:`pypesto.optimize.minimize` function."""
 
     def __init__(self):
```

### Comparing `pypesto-0.5.1/pypesto/result/predict.py` & `pypesto-0.5.2/pypesto/result/predict.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/result/profile.py` & `pypesto-0.5.2/pypesto/result/profile.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/result/result.py` & `pypesto-0.5.2/pypesto/result/result.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/result/sample.py` & `pypesto-0.5.2/pypesto/result/sample.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/sample/__init__.py` & `pypesto-0.5.2/pypesto/sample/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/sample/adaptive_metropolis.py` & `pypesto-0.5.2/pypesto/sample/adaptive_metropolis.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/sample/adaptive_parallel_tempering.py` & `pypesto-0.5.2/pypesto/sample/adaptive_parallel_tempering.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/sample/auto_correlation.py` & `pypesto-0.5.2/pypesto/sample/auto_correlation.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/sample/diagnostics.py` & `pypesto-0.5.2/pypesto/sample/diagnostics.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/sample/dynesty.py` & `pypesto-0.5.2/pypesto/sample/dynesty.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/sample/emcee.py` & `pypesto-0.5.2/pypesto/sample/emcee.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         self.problem = problem
 
         # extract for pickling efficiency
         objective = self.problem.objective
         lb = self.problem.lb
         ub = self.problem.ub
 
-        # parameter dimenstion
+        # parameter dimension
         ndim = len(self.problem.x_free_indices)
 
         def log_prob(x):
             """Log-probability density function."""
             # check if parameter lies within bounds
             if any(x < lb) or any(x > ub):
                 return -np.inf
```

### Comparing `pypesto-0.5.1/pypesto/sample/geweke_test.py` & `pypesto-0.5.2/pypesto/sample/geweke_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,19 @@
     )
     n = len(x)
     if n < nw:
         x[nw] = 0
         n = nw
 
     # Number of windows
-    k = np.floor((n - n_overlap) / (nw - n_overlap)).astype(int)
+    k = (
+        np.floor((n - n_overlap) / (nw - n_overlap)).astype(int)
+        if nw != n_overlap
+        else 0
+    )
     index = np.arange(nw)
     # Normalizing scale factor
     kmu = k * np.linalg.norm(w) ** 2
     spectral_density = np.zeros(nfft)
 
     for _ in range(k):
         xw = w * x[index]
```

### Comparing `pypesto-0.5.1/pypesto/sample/metropolis.py` & `pypesto-0.5.2/pypesto/sample/metropolis.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,22 @@
         if np.isnan(lpost_new):
             # will not be accepted
             lpost_new = -np.inf
 
         # compute log prior
         lprior_new = -self.neglogprior(x_new)
 
+        # if lpost_new is -inf, x_new will not be accepted
+        if lpost_new == -np.inf:
+            # update proposal
+            self._update_proposal(
+                x, lpost, -np.inf, len(self.trace_neglogpost) + 1
+            )
+            return x, lpost, lprior
+
         if not self.temper_lpost:
             # extract current log likelihood value
             llh = lpost - lprior
             # extract proposed log likelihood value
             llh_new = lpost_new - lprior_new
             # log acceptance probability (temper log likelihood)
             log_p_acc = min(beta * (llh_new - llh) + (lprior_new - lprior), 0)
```

### Comparing `pypesto-0.5.1/pypesto/sample/parallel_tempering.py` & `pypesto-0.5.2/pypesto/sample/parallel_tempering.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,14 @@
                 x=temps,
             )
         elif method == "simpson":
             log_evidence = simpson(
                 # integrate from low to high temperature
                 y=mean_loglike_per_beta,
                 x=temps,
-                even="last",
             )
         else:
             raise ValueError(
                 f"Unknown method {method}. Choose 'trapezoid' or 'simpson'."
             )
 
         return log_evidence
```

### Comparing `pypesto-0.5.1/pypesto/sample/pymc.py` & `pypesto-0.5.2/pypesto/sample/pymc.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/sample/sample.py` & `pypesto-0.5.2/pypesto/sample/sample.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/sample/sampler.py` & `pypesto-0.5.2/pypesto/sample/sampler.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/sample/util.py` & `pypesto-0.5.2/pypesto/sample/util.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/select/__init__.py` & `pypesto-0.5.2/pypesto/select/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/select/method.py` & `pypesto-0.5.2/pypesto/select/method.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/select/misc.py` & `pypesto-0.5.2/pypesto/select/misc.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/select/model_problem.py` & `pypesto-0.5.2/pypesto/select/model_problem.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/select/postprocessors.py` & `pypesto-0.5.2/pypesto/select/postprocessors.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/select/problem.py` & `pypesto-0.5.2/pypesto/select/problem.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/startpoint/base.py` & `pypesto-0.5.2/pypesto/startpoint/base.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/startpoint/latin_hypercube.py` & `pypesto-0.5.2/pypesto/startpoint/latin_hypercube.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/startpoint/uniform.py` & `pypesto-0.5.2/pypesto/startpoint/uniform.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/store/auto.py` & `pypesto-0.5.2/pypesto/store/auto.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/store/hdf5.py` & `pypesto-0.5.2/pypesto/store/hdf5.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/store/read_from_hdf5.py` & `pypesto-0.5.2/pypesto/store/read_from_hdf5.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/store/save_to_hdf5.py` & `pypesto-0.5.2/pypesto/store/save_to_hdf5.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
             for problem_attr in attrs_to_save:
                 value = getattr(problem, problem_attr)
                 if isinstance(value, (list, np.ndarray)):
                     value = np.asarray(value)
                     if value.size:
                         write_array(problem_grp, problem_attr, value)
-                elif isinstance(value, Integral):
+                elif isinstance(value, (Integral, str)):
                     problem_grp.attrs[problem_attr] = value
 
 
 class OptimizationResultHDF5Writer:
     """
     Writer of the HDF5 result files.
 
@@ -312,7 +312,13 @@
     if profile:
         pypesto_profile_writer = ProfileResultHDF5Writer(filename)
         pypesto_profile_writer.write(result, overwrite=overwrite)
 
     if sample:
         pypesto_sample_writer = SamplingResultHDF5Writer(filename)
         pypesto_sample_writer.write(result, overwrite=overwrite)
+
+    if hasattr(result, "variational_result"):
+        logger.warning(
+            "Results from variational inference are not saved in the hdf5 file. "
+            "You have to save them manually."
+        )
```

### Comparing `pypesto-0.5.1/pypesto/testing/examples.py` & `pypesto-0.5.2/pypesto/testing/examples.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/util.py` & `pypesto-0.5.2/pypesto/util.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/visualize/__init__.py` & `pypesto-0.5.2/pypesto/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/visualize/clust_color.py` & `pypesto-0.5.2/pypesto/visualize/clust_color.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/visualize/dimension_reduction.py` & `pypesto-0.5.2/pypesto/visualize/dimension_reduction.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/visualize/ensemble.py` & `pypesto-0.5.2/pypesto/visualize/ensemble.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/visualize/misc.py` & `pypesto-0.5.2/pypesto/visualize/misc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import warnings
 from collections.abc import Iterable
 from numbers import Number
 from typing import Optional, Union
 
 import numpy as np
 
@@ -19,14 +20,16 @@
     RGBA_MIN,
     RGBA_WHITE,
 )
 from ..result import Result
 from ..util import assign_clusters, delete_nan_inf
 from .clust_color import assign_colors_for_list
 
+logger = logging.getLogger(__name__)
+
 
 def process_result_list(
     results: Union[Result, list[Result]], colors=None, legends=None
 ):
     """
     Assign colors and legends to a list of results, check user provided lists.
 
@@ -299,16 +302,16 @@
 def process_start_indices(
     result: Result,
     start_indices: Union[str, int, Iterable[int]] = None,
 ) -> np.ndarray:
     """
     Process the start_indices.
 
-    Create an array of indices if a number was provided and checks that the
-    indices do not exceed the max_index.
+    Create an array of indices if a number was provided, checks that the indices
+    do not exceed the max_index and removes starts with non-finite fval.
 
     Parameters
     ----------
     start_indices:
         list of indices or int specifying an endpoint of the sequence of
         indices. Furthermore the following strings are possible:
             * 'all', this is the default, using all start indices.
@@ -319,33 +322,33 @@
     result:
         Result to determine maximum allowed length and/or clusters.
     """
     if start_indices is None:
         start_indices = ALL
     if isinstance(start_indices, str):
         if start_indices == ALL:
-            return np.asarray(range(len(result.optimize_result)))
+            start_indices = np.asarray(range(len(result.optimize_result)))
         elif start_indices == ALL_CLUSTERED:
             clust_ind, clust_size = assign_clusters(
                 delete_nan_inf(result.optimize_result.fval)[1]
             )
             # get all clusters that have size >= 2 and cluster of best start:
             clust_gr2 = np.where(clust_size > 2)[0]
             clust_gr2 = (
                 np.append(clust_gr2, 0) if 0 not in clust_gr2 else clust_gr2
             )
             start_indices = np.concatenate(
                 [np.where(clust_ind == i_clust)[0] for i_clust in clust_gr2]
             )
-            return start_indices
+            start_indices = start_indices
         elif start_indices == FIRST_CLUSTER:
             clust_ind = assign_clusters(
                 delete_nan_inf(result.optimize_result.fval)[1]
             )[0]
-            return np.where(clust_ind == 0)[0]
+            start_indices = np.where(clust_ind == 0)[0]
         else:
             raise ValueError(
                 f"Permissible values for start_indices are {ALL}, "
                 f"{ALL_CLUSTERED}, {FIRST_CLUSTER}, an integer or a "
                 f"list of indices."
             )
     # if it is an integer n, select the first n starts
@@ -355,14 +358,26 @@
     # filter out the indices that exceed the range of possible start indices
     start_indices = [
         start_index
         for start_index in start_indices
         if start_index < len(result.optimize_result)
     ]
 
+    # filter out the indices that are not finite
+    start_indices_unfiltered = len(start_indices)
+    start_indices = [
+        start_index
+        for start_index in start_indices
+        if np.isfinite(result.optimize_result[start_index].fval)
+    ]
+    if len(start_indices) != start_indices_unfiltered:
+        logger.warning(
+            "Some start indices were removed due to inf or nan function values."
+        )
+
     return np.asarray(start_indices)
 
 
 def process_parameter_indices(
     result: Result,
     parameter_indices: Union[str, Iterable[int]] = FREE_ONLY,
 ) -> list:
```

### Comparing `pypesto-0.5.1/pypesto/visualize/model_fit.py` & `pypesto-0.5.2/pypesto/visualize/model_fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import amici
 import amici.plotting
 import matplotlib.axes
 import matplotlib.pyplot as plt
 import numpy as np
 import petab
+from amici.petab.conditions import fill_in_parameters
 from amici.petab.simulations import rdatas_to_simulation_df
 from petab.visualize import plot_problem
 
 from ..C import CENSORED, ORDINAL, RDATAS, SEMIQUANTITATIVE
 from ..petab.importer import get_petab_non_quantitative_data_types
 from ..problem import HierarchicalProblem, Problem
 from ..result import Result
@@ -265,15 +266,15 @@
         # disable sensitivities to improve computation time
         amici_solver = copy.deepcopy(problem.objective.amici_solver)
         amici_solver.setSensitivityOrder(amici.SensitivityOrder.none)
 
         for j in range(len(edatas)):
             edatas[j].setTimepoints(simulation_timepoints)
 
-        amici.parameter_mapping.fill_in_parameters(
+        fill_in_parameters(
             edatas=edatas,
             problem_parameters=x_dct,
             scaled_parameters=True,
             parameter_mapping=parameter_mapping,
             amici_model=amici_model,
         )
```

### Comparing `pypesto-0.5.1/pypesto/visualize/optimization_stats.py` & `pypesto-0.5.2/pypesto/visualize/optimization_stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,23 +49,27 @@
     Returns
     -------
     ax:
         The plot axes.
 
     Examples
     --------
-    optimization_properties_per_multistart(
-        result1,
-        properties_to_plot=['time'],
-        colors=[.5, .9, .9, .3])
-
-    optimization_properties_per_multistart(
-        result1,
-        properties_to_plot=['time', 'n_grad'],
-        colors=[[.5, .9, .9, .3], [.2, .1, .9, .5]])
+    .. code-block:: python
+
+        optimization_run_properties_one_plot(
+            result1,
+            properties_to_plot=['time'],
+            colors=[.5, .9, .9, .3]
+        )
+
+        optimization_run_properties_one_plot(
+            result1,
+            properties_to_plot=['time', 'n_grad'],
+            colors=[[.5, .9, .9, .3], [.2, .1, .9, .5]]
+        )
     """
     if properties_to_plot is None:
         properties_to_plot = [
             "time",
             "n_fval",
             "n_grad",
             "n_hess",
@@ -152,32 +156,38 @@
     Returns
     -------
     ax:
     The plot axes.
 
     Examples
     --------
-    optimization_properties_per_multistart(
-        result1,
-        properties_to_plot=['time'],
-        colors=[.5, .9, .9, .3])
-
-    optimization_properties_per_multistart(
-        [result1, result2],
-        properties_to_plot=['time'],
-        colors=[[.5, .9, .9, .3], [.2, .1, .9, .5]])
-
-    optimization_properties_per_multistart(
-        result1,
-        properties_to_plot=['time', 'n_grad'],
-        colors=[.5, .9, .9, .3])
-
-    optimization_properties_per_multistart(
-        [result1, result2], properties_to_plot=['time', 'n_fval'],
-        colors=[[.5, .9, .9, .3], [.2, .1, .9, .5]])
+    .. code-block:: python
+
+        optimization_run_properties_per_multistart(
+            result1,
+            properties_to_plot=['time'],
+            colors=[.5, .9, .9, .3]
+        )
+
+        optimization_run_properties_per_multistart(
+            [result1, result2],
+            properties_to_plot=['time'],
+            colors=[[.5, .9, .9, .3], [.2, .1, .9, .5]]
+        )
+
+        optimization_run_properties_per_multistart(
+            result1,
+            properties_to_plot=['time', 'n_grad'],
+            colors=[.5, .9, .9, .3]
+        )
+
+        optimization_run_properties_per_multistart(
+            [result1, result2], properties_to_plot=['time', 'n_fval'],
+            colors=[[.5, .9, .9, .3], [.2, .1, .9, .5]]
+        )
     """
     if properties_to_plot is None:
         properties_to_plot = [
             "time",
             "n_fval",
             "n_grad",
             "n_hess",
```

### Comparing `pypesto-0.5.1/pypesto/visualize/optimizer_convergence.py` & `pypesto-0.5.2/pypesto/visualize/optimizer_convergence.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/visualize/optimizer_history.py` & `pypesto-0.5.2/pypesto/visualize/optimizer_history.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/visualize/ordinal_categories.py` & `pypesto-0.5.2/pypesto/visualize/ordinal_categories.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     import pypesto
 
 import matplotlib.pyplot as plt
 import numpy as np
 
 try:
     import amici
+    from amici.petab.conditions import fill_in_parameters
     from petab.C import OBSERVABLE_ID
 
     from ..hierarchical.ordinal.calculator import OrdinalCalculator
     from ..hierarchical.ordinal.parameter import OrdinalParameter
     from ..hierarchical.ordinal.solver import (
         compute_interval_constraints,
         get_bounds_for_category,
@@ -82,15 +83,15 @@
     amici_solver = pypesto_result.problem.objective.amici_solver
     petab_problem = (
         pypesto_result.problem.objective.amici_object_builder.petab_problem
     )
     n_threads = pypesto_result.problem.objective.n_threads
 
     # Fill in the parameters.
-    amici.parameter_mapping.fill_in_parameters(
+    fill_in_parameters(
         edatas=edatas,
         problem_parameters=x_dct,
         scaled_parameters=True,
         parameter_mapping=parameter_mapping,
         amici_model=amici_model,
     )
```

### Comparing `pypesto-0.5.1/pypesto/visualize/parameters.py` & `pypesto-0.5.2/pypesto/visualize/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -413,16 +413,16 @@
             xs_out[ix] = result.problem.get_reduced_vector(
                 x, parameter_indices
             )
         lb = result.problem.get_reduced_vector(lb, parameter_indices)
         ub = result.problem.get_reduced_vector(ub, parameter_indices)
         x_labels = [x_labels[int(i)] for i in parameter_indices]
     else:
-        lb = result.problem.get_full_vector(lb)
-        ub = result.problem.get_full_vector(ub)
+        lb = result.problem.lb_full
+        ub = result.problem.ub_full
 
     if inner_xs is not None and plot_inner_parameters:
         lb = np.concatenate([lb, inner_lb])
         ub = np.concatenate([ub, inner_ub])
         x_labels = x_labels + inner_xs_names
         xs_out = [
             np.concatenate([x, inner_x]) if x is not None else None
@@ -597,31 +597,18 @@
 
     start_indices = process_start_indices(
         start_indices=start_indices, result=result
     )
     parameter_indices = process_parameter_indices(
         parameter_indices=parameter_indices, result=result
     )
-    # remove all start indices that encounter an inf value at the start
-    # resulting in optimize_result[start]["x"] being None
-    start_indices_finite = start_indices[
-        [
-            result.optimize_result[i_start]["x"] is not None
-            for i_start in start_indices
-        ]
-    ]
-    # compare start_indices with start_indices_finite and log a warning
-    if len(start_indices) != len(start_indices_finite):
-        logger.warning(
-            "Some start indices were removed due to inf values at the start."
-        )
     # put all parameters into a dataframe, where columns are parameters
     parameters = [
         result.optimize_result[i_start]["x"][parameter_indices]
-        for i_start in start_indices_finite
+        for i_start in start_indices
     ]
     x_labels = [
         result.problem.x_names[parameter_index]
         for parameter_index in parameter_indices
     ]
     df = pd.DataFrame(parameters, columns=x_labels)
```

### Comparing `pypesto-0.5.1/pypesto/visualize/profile_cis.py` & `pypesto-0.5.2/pypesto/visualize/profile_cis.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/visualize/profiles.py` & `pypesto-0.5.2/pypesto/visualize/profiles.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/visualize/reference_points.py` & `pypesto-0.5.2/pypesto/visualize/reference_points.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/visualize/sampling.py` & `pypesto-0.5.2/pypesto/visualize/sampling.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/visualize/select.py` & `pypesto-0.5.2/pypesto/visualize/select.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto/visualize/spline_approximation.py` & `pypesto-0.5.2/pypesto/visualize/spline_approximation.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     SPLINE_KNOTS,
 )
 from ..problem import Problem
 from ..result import Result
 
 try:
     import amici
+    from amici.petab.conditions import fill_in_parameters
 
     from ..hierarchical import InnerCalculatorCollector
     from ..hierarchical.semiquantitative.calculator import SemiquantCalculator
     from ..hierarchical.semiquantitative.solver import (
         SemiquantInnerSolver,
         _calculate_regularization_for_group,
         extract_expdata_using_mask,
@@ -101,15 +102,15 @@
     parameter_mapping = pypesto_result.problem.objective.parameter_mapping
     amici_model = pypesto_result.problem.objective.amici_model
     amici_solver = pypesto_result.problem.objective.amici_solver
     n_threads = pypesto_result.problem.objective.n_threads
     observable_ids = amici_model.getObservableIds()
 
     # Fill in the parameters.
-    amici.parameter_mapping.fill_in_parameters(
+    fill_in_parameters(
         edatas=edatas,
         problem_parameters=x_dct,
         scaled_parameters=True,
         parameter_mapping=parameter_mapping,
         amici_model=amici_model,
     )
 
@@ -375,15 +376,15 @@
     edatas = pypesto_problem.objective.edatas
     parameter_mapping = pypesto_problem.objective.parameter_mapping
     amici_model = pypesto_problem.objective.amici_model
     amici_solver = pypesto_problem.objective.amici_solver
     n_threads = pypesto_problem.objective.n_threads
 
     # Fill in the parameters.
-    amici.parameter_mapping.fill_in_parameters(
+    fill_in_parameters(
         edatas=edatas,
         problem_parameters=x_dct,
         scaled_parameters=True,
         parameter_mapping=parameter_mapping,
         amici_model=amici_model,
     )
 
@@ -524,15 +525,15 @@
     edatas = pypesto_result.problem.objective.edatas
     parameter_mapping = pypesto_result.problem.objective.parameter_mapping
     amici_model = pypesto_result.problem.objective.amici_model
     amici_solver = pypesto_result.problem.objective.amici_solver
     n_threads = pypesto_result.problem.objective.n_threads
 
     # Fill in the parameters.
-    amici.parameter_mapping.fill_in_parameters(
+    fill_in_parameters(
         edatas=edatas,
         problem_parameters=x_dct,
         scaled_parameters=True,
         parameter_mapping=parameter_mapping,
         amici_model=amici_model,
     )
```

### Comparing `pypesto-0.5.1/pypesto/visualize/waterfall.py` & `pypesto-0.5.2/pypesto/visualize/waterfall.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/pypesto.egg-info/PKG-INFO` & `pypesto-0.5.2/pypesto.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypesto
-Version: 0.5.1
+Version: 0.5.2
 Summary: python-based Parameter EStimation TOolbox
 Home-page: https://github.com/icb-dcm/pypesto
 Download-URL: https://github.com/icb-dcm/pypesto/releases
 Author: The pyPESTO developers
 Author-email: yannik.schaelte@gmail.com
 Maintainer: Paul Jonas Jost, Maren Philipps, Domagoj Dorešić, Fabian Fröhlich
 Maintainer-email: paul.jost@uni-bonn.de, maren.philipps@uni-bonn.de, domagoj.doresic@uni-bonn.de, fabian.frohlich@crick.ac.uk
@@ -13,18 +13,18 @@
 Project-URL: Documentation, https://pypesto.readthedocs.io
 Project-URL: Changelog, https://pypesto.readthedocs.io/en/latest/changelog.html
 Keywords: parameter inference,optimization,sampling,profiles,ODE,AMICI,systems biology
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy!=1.24.0,>=1.19.1
 Requires-Dist: scipy>=1.5.2
 Requires-Dist: pandas>=1.5.0
 Requires-Dist: cloudpickle>=1.5.0
 Requires-Dist: matplotlib>=3.6.2
@@ -41,15 +41,14 @@
 Requires-Dist: nlopt>=2.6.2; extra == "all"
 Requires-Dist: pyswarm>=0.6; extra == "all"
 Requires-Dist: cma>=3.0.3; extra == "all"
 Requires-Dist: pyswarms>=1.3.0; extra == "all"
 Requires-Dist: fides>=0.6.1; extra == "all"
 Requires-Dist: mpi4py>=3.0.3; extra == "all"
 Requires-Dist: arviz>=0.12.1; extra == "all"
-Requires-Dist: scipy<1.13.0; extra == "all"
 Requires-Dist: aesara>=2.8.6; extra == "all"
 Requires-Dist: pymc>=4.2.1; extra == "all"
 Requires-Dist: aesara>=2.0.5; extra == "all"
 Requires-Dist: jax>=0.4.1; extra == "all"
 Requires-Dist: jaxlib>=0.4.1; extra == "all"
 Requires-Dist: julia>=0.5.7; extra == "all"
 Requires-Dist: ipython>=8.4.0; extra == "all"
@@ -67,15 +66,14 @@
 Requires-Dist: ipython>=8.4.0; extra == "all"
 Requires-Dist: myst-parser>=0.18.0; extra == "all"
 Requires-Dist: ipykernel==6.23.1; extra == "all"
 Requires-Dist: julia>=0.5.7; extra == "all"
 Requires-Dist: ipython>=8.4.0; extra == "all"
 Requires-Dist: pygments>=2.12.0; extra == "all"
 Requires-Dist: arviz>=0.12.1; extra == "all"
-Requires-Dist: scipy<1.13.0; extra == "all"
 Requires-Dist: aesara>=2.8.6; extra == "all"
 Requires-Dist: pymc>=4.2.1; extra == "all"
 Requires-Dist: emcee>=3.0.2; extra == "all"
 Requires-Dist: dynesty>=2.0.3; extra == "all"
 Requires-Dist: nlopt>=2.6.2; extra == "all"
 Requires-Dist: pyswarm>=0.6; extra == "all"
 Requires-Dist: notebook>=6.1.4; extra == "all"
@@ -88,15 +86,14 @@
 Requires-Dist: jax>=0.4.1; extra == "all"
 Requires-Dist: jaxlib>=0.4.1; extra == "all"
 Requires-Dist: libroadrunner>=2.6.0; extra == "all"
 Requires-Dist: julia>=0.5.7; extra == "all"
 Requires-Dist: ipython>=8.4.0; extra == "all"
 Requires-Dist: pygments>=2.12.0; extra == "all"
 Requires-Dist: arviz>=0.12.1; extra == "all"
-Requires-Dist: scipy<1.13.0; extra == "all"
 Requires-Dist: aesara>=2.8.6; extra == "all"
 Requires-Dist: pymc>=4.2.1; extra == "all"
 Requires-Dist: emcee>=3.0.2; extra == "all"
 Requires-Dist: dynesty>=2.0.3; extra == "all"
 Requires-Dist: nlopt>=2.6.2; extra == "all"
 Requires-Dist: pyswarm>=0.6; extra == "all"
 Requires-Dist: notebook>=6.1.4; extra == "all"
@@ -136,15 +133,14 @@
 Requires-Dist: pyswarms>=1.3.0; extra == "pyswarms"
 Provides-Extra: fides
 Requires-Dist: fides>=0.6.1; extra == "fides"
 Provides-Extra: mpi
 Requires-Dist: mpi4py>=3.0.3; extra == "mpi"
 Provides-Extra: pymc
 Requires-Dist: arviz>=0.12.1; extra == "pymc"
-Requires-Dist: scipy<1.13.0; extra == "pymc"
 Requires-Dist: aesara>=2.8.6; extra == "pymc"
 Requires-Dist: pymc>=4.2.1; extra == "pymc"
 Provides-Extra: aesara
 Requires-Dist: aesara>=2.0.5; extra == "aesara"
 Provides-Extra: jax
 Requires-Dist: jax>=0.4.1; extra == "jax"
 Requires-Dist: jaxlib>=0.4.1; extra == "jax"
@@ -169,15 +165,14 @@
 Requires-Dist: ipython>=8.4.0; extra == "doc"
 Requires-Dist: myst-parser>=0.18.0; extra == "doc"
 Requires-Dist: ipykernel==6.23.1; extra == "doc"
 Requires-Dist: julia>=0.5.7; extra == "doc"
 Requires-Dist: ipython>=8.4.0; extra == "doc"
 Requires-Dist: pygments>=2.12.0; extra == "doc"
 Requires-Dist: arviz>=0.12.1; extra == "doc"
-Requires-Dist: scipy<1.13.0; extra == "doc"
 Requires-Dist: aesara>=2.8.6; extra == "doc"
 Requires-Dist: pymc>=4.2.1; extra == "doc"
 Requires-Dist: emcee>=3.0.2; extra == "doc"
 Requires-Dist: dynesty>=2.0.3; extra == "doc"
 Requires-Dist: nlopt>=2.6.2; extra == "doc"
 Requires-Dist: pyswarm>=0.6; extra == "doc"
 Requires-Dist: notebook>=6.1.4; extra == "doc"
@@ -191,15 +186,14 @@
 Requires-Dist: jaxlib>=0.4.1; extra == "doc"
 Requires-Dist: libroadrunner>=2.6.0; extra == "doc"
 Provides-Extra: example
 Requires-Dist: julia>=0.5.7; extra == "example"
 Requires-Dist: ipython>=8.4.0; extra == "example"
 Requires-Dist: pygments>=2.12.0; extra == "example"
 Requires-Dist: arviz>=0.12.1; extra == "example"
-Requires-Dist: scipy<1.13.0; extra == "example"
 Requires-Dist: aesara>=2.8.6; extra == "example"
 Requires-Dist: pymc>=4.2.1; extra == "example"
 Requires-Dist: emcee>=3.0.2; extra == "example"
 Requires-Dist: dynesty>=2.0.3; extra == "example"
 Requires-Dist: nlopt>=2.6.2; extra == "example"
 Requires-Dist: pyswarm>=0.6; extra == "example"
 Requires-Dist: notebook>=6.1.4; extra == "example"
@@ -236,20 +230,23 @@
 * Interface to [AMICI](https://github.com/AMICI-dev/AMICI/) for efficient
   simulation and sensitivity analysis of ordinary differential equation (ODE)
   models
   ([example](https://github.com/ICB-DCM/pyPESTO/blob/main/doc/example/amici.ipynb))
 * Parameter estimation pipeline for systems biology problems specified in
   [SBML](http://sbml.org/) and [PEtab](https://github.com/PEtab-dev/PEtab)
   ([example](https://github.com/ICB-DCM/pyPESTO/blob/master/doc/example/petab_import.ipynb))
+* Parameter estimation with relative (scaled and offset) data as described in
+  [Schmiester et al. (2020)](https://doi.org/10.1093/bioinformatics/btz581).
+  ([example](https://github.com/ICB-DCM/pyPESTO/blob/master/doc/example/relative_data.ipynb))
 * Parameter estimation with ordinal data as described in
   [Schmiester et al. (2020)](https://doi.org/10.1007/s00285-020-01522-w) and
   [Schmiester et al. (2021)](https://doi.org/10.1093/bioinformatics/btab512).
-  ([example](https://github.com/ICB-DCM/pyPESTO/blob/master/doc/example/ordinal.ipynb))
-* Parameter estimation with censored data. ([example](https://github.com/ICB-DCM/pyPESTO/blob/master/doc/example/censored.ipynb))
-* Parameter estimation with nonlinear-monotone data. ([example](https://github.com/ICB-DCM/pyPESTO/blob/master/doc/example/nonlinear_monotone.ipynb))
+  ([example](https://github.com/ICB-DCM/pyPESTO/blob/master/doc/example/ordinal_data.ipynb))
+* Parameter estimation with censored data. ([example](https://github.com/ICB-DCM/pyPESTO/blob/master/doc/example/censored_data.ipynb))
+* Parameter estimation with nonlinear-monotone data. ([example](https://github.com/ICB-DCM/pyPESTO/blob/master/doc/example/semiquantitative_data.ipynb))
 
 ## Quick install
 
 The simplest way to install **pyPESTO** is via pip:
 
 ```shell
 pip3 install pypesto
```

### Comparing `pypesto-0.5.1/pypesto.egg-info/SOURCES.txt` & `pypesto-0.5.2/pypesto.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,17 @@
 pypesto/store/__init__.py
 pypesto/store/auto.py
 pypesto/store/hdf5.py
 pypesto/store/read_from_hdf5.py
 pypesto/store/save_to_hdf5.py
 pypesto/testing/__init__.py
 pypesto/testing/examples.py
+pypesto/variational/__init__.py
+pypesto/variational/pymc.py
+pypesto/variational/variational_inference.py
 pypesto/visualize/__init__.py
 pypesto/visualize/clust_color.py
 pypesto/visualize/dimension_reduction.py
 pypesto/visualize/ensemble.py
 pypesto/visualize/misc.py
 pypesto/visualize/model_fit.py
 pypesto/visualize/optimization_stats.py
```

### Comparing `pypesto-0.5.1/pypesto.egg-info/requires.txt` & `pypesto-0.5.2/pypesto.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 nlopt>=2.6.2
 pyswarm>=0.6
 cma>=3.0.3
 pyswarms>=1.3.0
 fides>=0.6.1
 mpi4py>=3.0.3
 arviz>=0.12.1
-scipy<1.13.0
 aesara>=2.8.6
 pymc>=4.2.1
 aesara>=2.0.5
 jax>=0.4.1
 jaxlib>=0.4.1
 julia>=0.5.7
 ipython>=8.4.0
@@ -82,15 +81,14 @@
 sphinxcontrib-bibtex>=2.5.0
 ipython>=8.4.0
 myst-parser>=0.18.0
 ipykernel==6.23.1
 julia>=0.5.7
 pygments>=2.12.0
 arviz>=0.12.1
-scipy<1.13.0
 aesara>=2.8.6
 pymc>=4.2.1
 emcee>=3.0.2
 dynesty>=2.0.3
 nlopt>=2.6.2
 pyswarm>=0.6
 notebook>=6.1.4
@@ -111,15 +109,14 @@
 emcee>=3.0.2
 
 [example]
 julia>=0.5.7
 ipython>=8.4.0
 pygments>=2.12.0
 arviz>=0.12.1
-scipy<1.13.0
 aesara>=2.8.6
 pymc>=4.2.1
 emcee>=3.0.2
 dynesty>=2.0.3
 nlopt>=2.6.2
 pyswarm>=0.6
 notebook>=6.1.4
@@ -150,15 +147,14 @@
 nlopt>=2.6.2
 
 [petab]
 petab>=0.2.0
 
 [pymc]
 arviz>=0.12.1
-scipy<1.13.0
 aesara>=2.8.6
 pymc>=4.2.1
 
 [pyswarm]
 pyswarm>=0.6
 
 [pyswarms]
```

### Comparing `pypesto-0.5.1/pyproject.toml` & `pypesto-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pypesto-0.5.1/setup.cfg` & `pypesto-0.5.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 license = BSD-3-Clause
 license_files = LICENSE
 classifiers = 
 	Development Status :: 4 - Beta
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python
+	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.10
-	Programming Language :: Python :: 3.9
 keywords = 
 	parameter inference
 	optimization
 	sampling
 	profiles
 	ODE
 	AMICI
@@ -41,15 +41,15 @@
 	cloudpickle >= 1.5.0
 	matplotlib >= 3.6.2
 	more-itertools >= 9.0.0
 	seaborn >= 0.11.2
 	h5py >= 3.1.0
 	tqdm >= 4.46.0
 	tabulate >= 0.8.10
-python_requires = >=3.9
+python_requires = >=3.10
 include_package_data = True
 packages = find:
 
 [options.packages.find]
 include = pypesto*
 
 [options.extras_require]
@@ -98,15 +98,14 @@
 	pyswarms >= 1.3.0
 fides = 
 	fides >= 0.6.1
 mpi = 
 	mpi4py >= 3.0.3
 pymc = 
 	arviz >= 0.12.1
-	scipy < 1.13.0 # https://github.com/ICB-DCM/pyPESTO/issues/1354
 	aesara >= 2.8.6
 	pymc >= 4.2.1
 aesara = 
 	aesara >= 2.0.5
 jax = 
 	jax >= 0.4.1
 	jaxlib >= 0.4.1
```

