# Comparing `tmp/attpc_spyral-0.7.0.tar.gz` & `tmp/attpc_spyral-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attpc_spyral-0.7.0.tar", last modified: Wed May 22 17:59:50 2024, max compression
+gzip compressed data, was "attpc_spyral-0.8.0.tar", last modified: Fri May 31 16:38:38 2024, max compression
```

## Comparing `attpc_spyral-0.7.0.tar` & `attpc_spyral-0.8.0.tar`

### file list

```diff
@@ -1,63 +1,62 @@
--rw-r--r--   0        0        0    35149 2024-05-22 17:59:36.450208 attpc_spyral-0.7.0/LICENSE
--rw-r--r--   0        0        0     6290 2024-05-22 17:59:36.450208 attpc_spyral-0.7.0/README.md
--rw-r--r--   0        0        0      820 2024-05-22 17:59:50.238369 attpc_spyral-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      759 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/__init__.py
--rw-r--r--   0        0        0     7509 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/cluster.py
--rw-r--r--   0        0        0    11603 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/clusterize.py
--rw-r--r--   0        0        0     8107 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/config.py
--rw-r--r--   0        0        0     2241 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/constants.py
--rw-r--r--   0        0        0    10702 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/estimator.py
--rw-r--r--   0        0        0     2202 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/hardware_id.py
--rw-r--r--   0        0        0     1353 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/legacy_beam_pads.py
--rw-r--r--   0        0        0     8708 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/pad_map.py
--rw-r--r--   0        0        0     7456 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/phase.py
--rw-r--r--   0        0        0    10125 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/pipeline.py
--rw-r--r--   0        0        0     7040 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/point_cloud.py
--rw-r--r--   0        0        0     4316 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/run_stacks.py
--rw-r--r--   0        0        0     4575 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/spy_log.py
--rw-r--r--   0        0        0      537 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/status_message.py
--rw-r--r--   0        0        0    20110 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/core/track_generator.py
--rw-r--r--   0        0        0      128 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/correction/__init__.py
--rw-r--r--   0        0        0     2579 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/correction/electron_corrector.py
--rw-r--r--   0        0        0     4367 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/correction/generate.py
--rw-r--r--   0        0        0        0 2024-05-22 17:59:36.454208 attpc_spyral-0.7.0/src/spyral/data/__init__.py
--rw-r--r--   0        0        0   151675 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/data/pad_electronics.csv
--rw-r--r--   0        0        0   140922 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/data/pad_electronics_legacy.csv
--rw-r--r--   0        0        0    28681 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/data/pad_gain_map.csv
--rw-r--r--   0        0        0    47110 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/data/pad_scale.csv
--rw-r--r--   0        0        0    94283 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/data/pad_time_correction.csv
--rw-r--r--   0        0        0   213104 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/data/padxy.csv
--rw-r--r--   0        0        0   213104 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/data/padxy_legacy.csv
--rw-r--r--   0        0        0        0 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/geometry/__init__.py
--rw-r--r--   0        0        0     2477 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/geometry/circle.py
--rw-r--r--   0        0        0       89 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/interpolate/__init__.py
--rw-r--r--   0        0        0     9011 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/interpolate/bilinear.py
--rw-r--r--   0        0        0     3474 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/interpolate/linear.py
--rw-r--r--   0        0        0    13187 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/interpolate/track_interpolator.py
--rw-r--r--   0        0        0        0 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/phases/__init__.py
--rw-r--r--   0        0        0     5819 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/phases/cluster_phase.py
--rw-r--r--   0        0        0     6305 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/phases/estimation_phase.py
--rw-r--r--   0        0        0    11667 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/phases/interp_solver_phase.py
--rw-r--r--   0        0        0     7750 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/phases/pointcloud_legacy_phase.py
--rw-r--r--   0        0        0    12121 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/phases/pointcloud_phase.py
--rw-r--r--   0        0        0     1226 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/phases/schema.py
--rw-r--r--   0        0        0        0 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/solvers/__init__.py
--rw-r--r--   0        0        0     1591 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/solvers/guess.py
--rw-r--r--   0        0        0    10600 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/solvers/solver_interp.py
--rw-r--r--   0        0        0        0 2024-05-22 17:59:36.458208 attpc_spyral-0.7.0/src/spyral/trace/__init__.py
--rw-r--r--   0        0        0    11463 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/src/spyral/trace/frib_event.py
--rw-r--r--   0        0        0     4827 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/src/spyral/trace/frib_scalers.py
--rw-r--r--   0        0        0     3993 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/src/spyral/trace/frib_trace.py
--rw-r--r--   0        0        0     4542 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/src/spyral/trace/get_event.py
--rw-r--r--   0        0        0     5737 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/src/spyral/trace/get_legacy_event.py
--rw-r--r--   0        0        0     6140 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/src/spyral/trace/get_trace.py
--rw-r--r--   0        0        0      899 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/src/spyral/trace/peak.py
--rw-r--r--   0        0        0        0 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0       67 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/tests/run_0000.h5
--rw-r--r--   0        0        0      121 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/tests/run_0001.h5
--rw-r--r--   0        0        0      396 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/tests/test_circle.py
--rw-r--r--   0        0        0     3970 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/tests/test_default_pipeline.py
--rw-r--r--   0        0        0     1573 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/tests/test_pad.py
--rw-r--r--   0        0        0     1172 2024-05-22 17:59:36.462209 attpc_spyral-0.7.0/tests/test_runs.py
--rw-r--r--   0        0        0     6832 1970-01-01 00:00:00.000000 attpc_spyral-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-31 16:38:25.213096 attpc_spyral-0.8.0/LICENSE
+-rw-r--r--   0        0        0     6220 2024-05-31 16:38:25.213096 attpc_spyral-0.8.0/README.md
+-rw-r--r--   0        0        0      876 2024-05-31 16:38:38.977083 attpc_spyral-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      759 2024-05-31 16:38:25.217096 attpc_spyral-0.8.0/src/spyral/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 16:38:25.217096 attpc_spyral-0.8.0/src/spyral/core/__init__.py
+-rw-r--r--   0        0        0     7545 2024-05-31 16:38:25.217096 attpc_spyral-0.8.0/src/spyral/core/cluster.py
+-rw-r--r--   0        0        0    11603 2024-05-31 16:38:25.217096 attpc_spyral-0.8.0/src/spyral/core/clusterize.py
+-rw-r--r--   0        0        0     8083 2024-05-31 16:38:25.217096 attpc_spyral-0.8.0/src/spyral/core/config.py
+-rw-r--r--   0        0        0     2241 2024-05-31 16:38:25.217096 attpc_spyral-0.8.0/src/spyral/core/constants.py
+-rw-r--r--   0        0        0    10702 2024-05-31 16:38:25.217096 attpc_spyral-0.8.0/src/spyral/core/estimator.py
+-rw-r--r--   0        0        0     2202 2024-05-31 16:38:25.217096 attpc_spyral-0.8.0/src/spyral/core/hardware_id.py
+-rw-r--r--   0        0        0     1353 2024-05-31 16:38:25.217096 attpc_spyral-0.8.0/src/spyral/core/legacy_beam_pads.py
+-rw-r--r--   0        0        0     9150 2024-05-31 16:38:25.217096 attpc_spyral-0.8.0/src/spyral/core/pad_map.py
+-rw-r--r--   0        0        0     7530 2024-05-31 16:38:25.217096 attpc_spyral-0.8.0/src/spyral/core/phase.py
+-rw-r--r--   0        0        0    10422 2024-05-31 16:38:25.217096 attpc_spyral-0.8.0/src/spyral/core/pipeline.py
+-rw-r--r--   0        0        0     7029 2024-05-31 16:38:25.217096 attpc_spyral-0.8.0/src/spyral/core/point_cloud.py
+-rw-r--r--   0        0        0     4316 2024-05-31 16:38:25.221096 attpc_spyral-0.8.0/src/spyral/core/run_stacks.py
+-rw-r--r--   0        0        0     4575 2024-05-31 16:38:25.221096 attpc_spyral-0.8.0/src/spyral/core/spy_log.py
+-rw-r--r--   0        0        0      537 2024-05-31 16:38:25.221096 attpc_spyral-0.8.0/src/spyral/core/status_message.py
+-rw-r--r--   0        0        0    20110 2024-05-31 16:38:25.221096 attpc_spyral-0.8.0/src/spyral/core/track_generator.py
+-rw-r--r--   0        0        0      128 2024-05-31 16:38:25.221096 attpc_spyral-0.8.0/src/spyral/correction/__init__.py
+-rw-r--r--   0        0        0     2579 2024-05-31 16:38:25.221096 attpc_spyral-0.8.0/src/spyral/correction/electron_corrector.py
+-rw-r--r--   0        0        0     4367 2024-05-31 16:38:25.221096 attpc_spyral-0.8.0/src/spyral/correction/generate.py
+-rw-r--r--   0        0        0        0 2024-05-31 16:38:25.221096 attpc_spyral-0.8.0/src/spyral/data/__init__.py
+-rw-r--r--   0        0        0   151675 2024-05-31 16:38:25.221096 attpc_spyral-0.8.0/src/spyral/data/pad_electronics.csv
+-rw-r--r--   0        0        0   140922 2024-05-31 16:38:25.221096 attpc_spyral-0.8.0/src/spyral/data/pad_electronics_legacy.csv
+-rw-r--r--   0        0        0    28681 2024-05-31 16:38:25.221096 attpc_spyral-0.8.0/src/spyral/data/pad_gain_map.csv
+-rw-r--r--   0        0        0    47110 2024-05-31 16:38:25.221096 attpc_spyral-0.8.0/src/spyral/data/pad_scale.csv
+-rw-r--r--   0        0        0    94283 2024-05-31 16:38:25.221096 attpc_spyral-0.8.0/src/spyral/data/pad_time_correction.csv
+-rw-r--r--   0        0        0   213104 2024-05-31 16:38:25.221096 attpc_spyral-0.8.0/src/spyral/data/padxy.csv
+-rw-r--r--   0        0        0        0 2024-05-31 16:38:25.221096 attpc_spyral-0.8.0/src/spyral/geometry/__init__.py
+-rw-r--r--   0        0        0     2477 2024-05-31 16:38:25.221096 attpc_spyral-0.8.0/src/spyral/geometry/circle.py
+-rw-r--r--   0        0        0       89 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/src/spyral/interpolate/__init__.py
+-rw-r--r--   0        0        0     9011 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/src/spyral/interpolate/bilinear.py
+-rw-r--r--   0        0        0     3474 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/src/spyral/interpolate/linear.py
+-rw-r--r--   0        0        0    13187 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/src/spyral/interpolate/track_interpolator.py
+-rw-r--r--   0        0        0        0 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/src/spyral/phases/__init__.py
+-rw-r--r--   0        0        0     5819 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/src/spyral/phases/cluster_phase.py
+-rw-r--r--   0        0        0     6305 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/src/spyral/phases/estimation_phase.py
+-rw-r--r--   0        0        0    11667 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/src/spyral/phases/interp_solver_phase.py
+-rw-r--r--   0        0        0     7750 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/src/spyral/phases/pointcloud_legacy_phase.py
+-rw-r--r--   0        0        0    12121 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/src/spyral/phases/pointcloud_phase.py
+-rw-r--r--   0        0        0     1226 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/src/spyral/phases/schema.py
+-rw-r--r--   0        0        0        0 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/src/spyral/solvers/__init__.py
+-rw-r--r--   0        0        0     1591 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/src/spyral/solvers/guess.py
+-rw-r--r--   0        0        0    10600 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/src/spyral/solvers/solver_interp.py
+-rw-r--r--   0        0        0        0 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/src/spyral/trace/__init__.py
+-rw-r--r--   0        0        0    11463 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/src/spyral/trace/frib_event.py
+-rw-r--r--   0        0        0     4827 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/src/spyral/trace/frib_scalers.py
+-rw-r--r--   0        0        0     3993 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/src/spyral/trace/frib_trace.py
+-rw-r--r--   0        0        0     4542 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/src/spyral/trace/get_event.py
+-rw-r--r--   0        0        0     5737 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/src/spyral/trace/get_legacy_event.py
+-rw-r--r--   0        0        0     6140 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/src/spyral/trace/get_trace.py
+-rw-r--r--   0        0        0      899 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/src/spyral/trace/peak.py
+-rw-r--r--   0        0        0        0 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0       67 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/tests/run_0000.h5
+-rw-r--r--   0        0        0      121 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/tests/run_0001.h5
+-rw-r--r--   0        0        0      396 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/tests/test_circle.py
+-rw-r--r--   0        0        0     3938 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/tests/test_default_pipeline.py
+-rw-r--r--   0        0        0     1501 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/tests/test_pad.py
+-rw-r--r--   0        0        0     1172 2024-05-31 16:38:25.225096 attpc_spyral-0.8.0/tests/test_runs.py
+-rw-r--r--   0        0        0     6792 1970-01-01 00:00:00.000000 attpc_spyral-0.8.0/PKG-INFO
```

### Comparing `attpc_spyral-0.7.0/LICENSE` & `attpc_spyral-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/README.md` & `attpc_spyral-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,14 @@
 run_max = 94
 n_processes = 4
 
 pad_params = PadParameters(
     is_default=True,
     is_default_legacy=False,
     pad_geometry_path=INVALID_PATH,
-    pad_gain_path=INVALID_PATH,
     pad_time_path=INVALID_PATH,
     pad_electronics_path=INVALID_PATH,
     pad_scale_path=INVALID_PATH,
 )
 
 get_params = GetParameters(
     baseline_window_scale=20.0,
@@ -101,15 +100,14 @@
 cluster_params = ClusterParameters(
     min_cloud_size=50,
     min_points=3,
     min_size_scale_factor=0.05,
     min_size_lower_cutoff=10,
     cluster_selection_epsilon=10.0,
     circle_overlap_ratio=0.5,
-    fractional_charge_threshold=0.8,
     outlier_scale_factor=0.05,
 )
 
 estimate_params = EstimateParameters(
     min_total_trajectory_points=30, smoothing_factor=100.0
 )
 
@@ -172,8 +170,7 @@
 ### Logs and Output
 
 Spyral creates a set of logfiles when it is run (located in the log directory of the workspace). These logfiles can contain critical information describing the state of Spyral. In particular, if Spyral has a crash, the logfiles can be useful for determining what went wrong. A logfile is created for each process (including the parent process). The files are labeld by process number (or as parent in the case of the parent).
 
 ## Notebooks
 
 See the [spyral_notebooks](https://github.com/attpc/spyral_notebooks) repository for notebooks which demonstrate the behavior of the default Phases of Spyral.
-
```

### Comparing `attpc_spyral-0.7.0/pyproject.toml` & `attpc_spyral-0.8.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [project]
 name = "attpc_spyral"
-version = "0.7.0"
+version = "0.8.0"
 description = "AT-TPC analysis pipeline"
 authors = [
     { name = "gwm17", email = "gordonmccann215@gmail.com" },
+    { name = "turinath", email = "turi@frib.msu.edu" },
 ]
 dependencies = [
     "spyral-utils>=1.0.0",
     "black>=24.4.0",
     "contourpy>=1.2.1",
     "h5py>=3.11.0",
     "lmfit>=1.3.0",
```

### Comparing `attpc_spyral-0.7.0/src/spyral/__init__.py` & `attpc_spyral-0.8.0/src/spyral/__init__.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/core/cluster.py` & `attpc_spyral-0.8.0/src/spyral/core/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         if neighbors < 2:
             neighbors = 2
         test_data = self.data[:, :3].copy()
         neigh = LocalOutlierFactor(n_neighbors=neighbors)
         result = neigh.fit_predict(test_data)
         mask = result > 0
         self.data = self.data[mask]  # label=-1 is an outlier
-        return np.flatnonzero(mask)
+        return np.flatnonzero(~mask)  # Invert the mask to get outliers
 
     def create_splines(self, smoothing: float = 1.0) -> None:
         """Create smoothing splines for the x,y,charge dimensions
 
         Create smoothing splines along the z-coordinate for x, y, and charge.
         The degree of smoothing is controlled by the smoothing parameter. smoothing = 0.0 is
         no smoothing (pure interpolation) and higher values gives a higher degree of smoothing.
```

### Comparing `attpc_spyral-0.7.0/src/spyral/core/clusterize.py` & `attpc_spyral-0.8.0/src/spyral/core/clusterize.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/core/config.py` & `attpc_spyral-0.8.0/src/spyral/core/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     pad_electronics_path: Path
         Path to the csv file containing the pad electronics ids
     """
 
     is_default: bool
     is_default_legacy: bool
     pad_geometry_path: Path
-    pad_gain_path: Path
     pad_time_path: Path
     pad_electronics_path: Path
     pad_scale_path: Path
 
 
 @dataclass
 class RunParameters:
```

### Comparing `attpc_spyral-0.7.0/src/spyral/core/constants.py` & `attpc_spyral-0.8.0/src/spyral/core/constants.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/core/estimator.py` & `attpc_spyral-0.8.0/src/spyral/core/estimator.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/core/hardware_id.py` & `attpc_spyral-0.8.0/src/spyral/core/hardware_id.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/core/legacy_beam_pads.py` & `attpc_spyral-0.8.0/src/spyral/core/legacy_beam_pads.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/core/pad_map.py` & `attpc_spyral-0.8.0/src/spyral/core/pad_map.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,32 +87,38 @@
 
         suffix = ""
         if is_legacy:
             suffix = "_legacy"
 
         directory = resources.files("spyral.data")
 
-        geom_handle = directory.joinpath(f"padxy{suffix}.csv")
+        geom_handle = directory.joinpath(f"padxy.csv")
         with resources.as_file(geom_handle) as geopath:
             geofile = open(geopath, "r")
             geofile.readline()  # Remove header
             lines = geofile.readlines()
             for pad_number, line in enumerate(lines):
                 entries = line.split(",")
                 self.map[pad_number] = PadData(x=float(entries[0]), y=float(entries[1]))
             geofile.close()
-        gain_handle = directory.joinpath("pad_gain_map.csv")
-        with resources.as_file(gain_handle) as gainpath:
-            gainfile = open(gainpath, "r")
-            gainfile.readline()
-            lines = gainfile.readlines()
-            for pad_number, line in enumerate(lines):
-                entries = line.split(",")
-                self.map[pad_number].gain = float(entries[0])
-            gainfile.close()
+        #
+        # NOTE This is left in as a comment to show how a gain map could
+        # be implemented. This is not used in current Spyral as it has no
+        # impact on the analysis
+        #
+        # gain_handle = directory.joinpath("pad_gain_map.csv")
+        # with resources.as_file(gain_handle) as gainpath:
+        #     gainfile = open(gainpath, "r")
+        #     gainfile.readline()
+        #     lines = gainfile.readlines()
+        #     for pad_number, line in enumerate(lines):
+        #         entries = line.split(",")
+        #         self.map[pad_number].gain = float(entries[0])
+        #     gainfile.close()
+        #
         time_handle = directory.joinpath("pad_time_correction.csv")
         with resources.as_file(time_handle) as timepath:
             timefile = open(timepath, "r")
             timefile.readline()
             lines = timefile.readlines()
             for pad_number, line in enumerate(lines):
                 entries = line.split(",")
@@ -156,20 +162,26 @@
         """
         with open(params.pad_geometry_path, "r") as geofile:
             geofile.readline()  # Remove header
             lines = geofile.readlines()
             for pad_number, line in enumerate(lines):
                 entries = line.split(",")
                 self.map[pad_number] = PadData(x=float(entries[0]), y=float(entries[1]))
-        with open(params.pad_gain_path, "r") as gainfile:
-            gainfile.readline()
-            lines = gainfile.readlines()
-            for pad_number, line in enumerate(lines):
-                entries = line.split(",")
-                self.map[pad_number].gain = float(entries[0])
+        #
+        # NOTE This is left in as a comment to show how a gain map could
+        # be implemented. This is not used in current Spyral as it has no
+        # impact on the analysis
+        #
+        # with open(params.pad_gain_path, "r") as gainfile:
+        #     gainfile.readline()
+        #     lines = gainfile.readlines()
+        #     for pad_number, line in enumerate(lines):
+        #         entries = line.split(",")
+        #         self.map[pad_number].gain = float(entries[0])
+        #
         with open(params.pad_time_path, "r") as timefile:
             timefile.readline()
             lines = timefile.readlines()
             for pad_number, line in enumerate(lines):
                 entries = line.split(",")
                 self.map[pad_number].time_offset = float(entries[0])
```

### Comparing `attpc_spyral-0.7.0/src/spyral/core/phase.py` & `attpc_spyral-0.8.0/src/spyral/core/phase.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sys
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from pathlib import Path
 from multiprocessing import SimpleQueue
 from numpy.random import Generator
+from collections import Counter
 
 if sys.version_info < (3, 11):
     from typing_extensions import Self
 else:
     from typing import Self
 from typing import Any
 
@@ -41,15 +42,17 @@
 
         Returns
         -------
         bool
             True if the schemas are equivalent or False if they are different
 
         """
-        return self.extension == value.extension and self.structure == value.structure
+        return self.extension == value.extension and (
+            Counter(self.structure) == Counter(value.structure)
+        )
 
 
 @dataclass
 class PhaseResult:
     """Dataclass representing the result of a Phase
 
     Attributes
```

### Comparing `attpc_spyral-0.7.0/src/spyral/core/pipeline.py` & `attpc_spyral-0.8.0/src/spyral/core/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 from .run_stacks import form_run_string, create_run_stacks
 from .status_message import StatusMessage
 from .phase import PhaseLike, PhaseResult
-from .spy_log import init_spyral_logger_parent, init_spyral_logger_child, spyral_info
+from .spy_log import (
+    init_spyral_logger_parent,
+    init_spyral_logger_child,
+    spyral_info,
+    spyral_warn,
+)
 
 from tqdm import tqdm
 from pathlib import Path
 from multiprocessing import SimpleQueue, Process
 from copy import deepcopy
 from numpy.random import SeedSequence, default_rng
 import time
@@ -235,14 +240,22 @@
         print("")
         print("Pipeline validation failed!")
         print(f"Status: {result}")
         return
     print("Pipeline successfully validated.")
 
     stacks = create_run_stacks(pipeline.traces, run_min, run_max, n_procs)
+    stack_count = 0
+    for stack in stacks:
+        stack_count += len(stack)
+    if len(stack) == 0:
+        spyral_warn(
+            __name__,
+            f"No runs were found in trace path: {pipeline.traces}. Traces must exist to create workload!",
+        )
     spyral_info(__name__, f"Run stacks: {stacks}")
 
     seq = SeedSequence()
 
     queues: list[SimpleQueue] = []
     processes: list[Process] = []
     pbars: list[tqdm] = []
```

### Comparing `attpc_spyral-0.7.0/src/spyral/core/point_cloud.py` & `attpc_spyral-0.8.0/src/spyral/core/point_cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             for peak in trace.get_peaks():
                 self.cloud[idx, 0] = pad.x  # X-coordinate, geometry
                 self.cloud[idx, 1] = pad.y  # Y-coordinate, geometry
                 self.cloud[idx, 2] = (
                     peak.centroid + pad.time_offset
                 )  # Z-coordinate, time with correction until calibrated with calibrate_z_position()
                 self.cloud[idx, 3] = peak.amplitude
-                self.cloud[idx, 4] = peak.integral * pad.gain
+                self.cloud[idx, 4] = peak.integral
                 self.cloud[idx, 5] = trace.hw_id.pad_id
                 self.cloud[idx, 6] = (
                     peak.centroid + pad.time_offset
                 )  # Time bucket with correction
                 self.cloud[idx, 7] = pad.scale
                 idx += 1
         self.cloud = self.cloud[self.cloud[:, 3] != 0.0]
```

### Comparing `attpc_spyral-0.7.0/src/spyral/core/run_stacks.py` & `attpc_spyral-0.8.0/src/spyral/core/run_stacks.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/core/spy_log.py` & `attpc_spyral-0.8.0/src/spyral/core/spy_log.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/core/status_message.py` & `attpc_spyral-0.8.0/src/spyral/core/status_message.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/core/track_generator.py` & `attpc_spyral-0.8.0/src/spyral/core/track_generator.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/correction/electron_corrector.py` & `attpc_spyral-0.8.0/src/spyral/correction/electron_corrector.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/correction/generate.py` & `attpc_spyral-0.8.0/src/spyral/correction/generate.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/data/pad_electronics.csv` & `attpc_spyral-0.8.0/src/spyral/data/pad_electronics.csv`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/data/pad_electronics_legacy.csv` & `attpc_spyral-0.8.0/src/spyral/data/pad_electronics_legacy.csv`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/data/pad_time_correction.csv` & `attpc_spyral-0.8.0/src/spyral/data/pad_time_correction.csv`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/data/padxy.csv` & `attpc_spyral-0.8.0/src/spyral/data/padxy.csv`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/geometry/circle.py` & `attpc_spyral-0.8.0/src/spyral/geometry/circle.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/interpolate/bilinear.py` & `attpc_spyral-0.8.0/src/spyral/interpolate/bilinear.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/interpolate/linear.py` & `attpc_spyral-0.8.0/src/spyral/interpolate/linear.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/interpolate/track_interpolator.py` & `attpc_spyral-0.8.0/src/spyral/interpolate/track_interpolator.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/phases/cluster_phase.py` & `attpc_spyral-0.8.0/src/spyral/phases/cluster_phase.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/phases/estimation_phase.py` & `attpc_spyral-0.8.0/src/spyral/phases/estimation_phase.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/phases/interp_solver_phase.py` & `attpc_spyral-0.8.0/src/spyral/phases/interp_solver_phase.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/phases/pointcloud_legacy_phase.py` & `attpc_spyral-0.8.0/src/spyral/phases/pointcloud_legacy_phase.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/phases/pointcloud_phase.py` & `attpc_spyral-0.8.0/src/spyral/phases/pointcloud_phase.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/phases/schema.py` & `attpc_spyral-0.8.0/src/spyral/phases/schema.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/solvers/guess.py` & `attpc_spyral-0.8.0/src/spyral/solvers/guess.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/solvers/solver_interp.py` & `attpc_spyral-0.8.0/src/spyral/solvers/solver_interp.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/trace/frib_event.py` & `attpc_spyral-0.8.0/src/spyral/trace/frib_event.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/trace/frib_scalers.py` & `attpc_spyral-0.8.0/src/spyral/trace/frib_scalers.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/trace/frib_trace.py` & `attpc_spyral-0.8.0/src/spyral/trace/frib_trace.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/trace/get_event.py` & `attpc_spyral-0.8.0/src/spyral/trace/get_event.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/trace/get_legacy_event.py` & `attpc_spyral-0.8.0/src/spyral/trace/get_legacy_event.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/trace/get_trace.py` & `attpc_spyral-0.8.0/src/spyral/trace/get_trace.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/src/spyral/trace/peak.py` & `attpc_spyral-0.8.0/src/spyral/trace/peak.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/tests/test_default_pipeline.py` & `attpc_spyral-0.8.0/tests/test_default_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 workspace_path = Path(__file__).parent / "test_workspace"
 trace_path = Path(__file__).parent
 
 pad_params = PadParameters(
     is_default=True,
     is_default_legacy=False,
     pad_geometry_path=INVALID_PATH,
-    pad_gain_path=INVALID_PATH,
     pad_time_path=INVALID_PATH,
     pad_electronics_path=INVALID_PATH,
     pad_scale_path=INVALID_PATH,
 )
 get_params = GetParameters(
     baseline_window_scale=20.0,
     peak_separation=50.0,
```

### Comparing `attpc_spyral-0.7.0/tests/test_pad.py` & `attpc_spyral-0.8.0/tests/test_pad.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,56 +4,54 @@
 
 
 def test_default_pads():
     params = PadParameters(
         is_default=True,
         is_default_legacy=False,
         pad_geometry_path=INVALID_PATH,
-        pad_gain_path=INVALID_PATH,
         pad_time_path=INVALID_PATH,
         pad_electronics_path=INVALID_PATH,
         pad_scale_path=INVALID_PATH,
     )
 
     default_pmap = PadMap(params)
 
     assert default_pmap.is_valid
 
     pad0 = default_pmap.get_pad_data(0)
     assert pad0 is not None
     assert pad0.x == -269.95294
     assert pad0.y == 4.2506561
-    assert pad0.gain == 1.3
+    assert pad0.gain == 1.0
     assert pad0.time_offset == 0
     assert pad0.scale == 1.0
 
     reverse0 = default_pmap.get_pad_from_hardware(pad0.hardware)
     assert reverse0 is not None
     assert reverse0 == 0
 
 
 def test_default_legacy_pads():
     params = PadParameters(
         is_default=False,
         is_default_legacy=True,
         pad_geometry_path=INVALID_PATH,
-        pad_gain_path=INVALID_PATH,
         pad_time_path=INVALID_PATH,
         pad_electronics_path=INVALID_PATH,
         pad_scale_path=INVALID_PATH,
     )
 
     default_pmap = PadMap(params)
 
     assert default_pmap.is_valid
 
     pad0 = default_pmap.get_pad_data(0)
     assert pad0 is not None
     assert pad0.x == -269.95294
     assert pad0.y == 4.2506561
-    assert pad0.gain == 1.3
+    assert pad0.gain == 1.0
     assert pad0.time_offset == 0
     assert pad0.scale == 1.0
 
     reverse0 = default_pmap.get_pad_from_hardware(pad0.hardware)
     assert reverse0 is not None
     assert reverse0 == 0
```

### Comparing `attpc_spyral-0.7.0/tests/test_runs.py` & `attpc_spyral-0.8.0/tests/test_runs.py`

 * *Files identical despite different names*

### Comparing `attpc_spyral-0.7.0/PKG-INFO` & `attpc_spyral-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: attpc_spyral
-Version: 0.7.0
+Version: 0.8.0
 Summary: AT-TPC analysis pipeline
-Author-Email: gwm17 <gordonmccann215@gmail.com>
+Author-Email: gwm17 <gordonmccann215@gmail.com>, turinath <turi@frib.msu.edu>
 License: GPL-3
 Requires-Python: <3.13,>=3.10
 Requires-Dist: spyral-utils>=1.0.0
 Requires-Dist: black>=24.4.0
 Requires-Dist: contourpy>=1.2.1
 Requires-Dist: h5py>=3.11.0
 Requires-Dist: lmfit>=1.3.0
@@ -76,15 +76,14 @@
 run_max = 94
 n_processes = 4
 
 pad_params = PadParameters(
     is_default=True,
     is_default_legacy=False,
     pad_geometry_path=INVALID_PATH,
-    pad_gain_path=INVALID_PATH,
     pad_time_path=INVALID_PATH,
     pad_electronics_path=INVALID_PATH,
     pad_scale_path=INVALID_PATH,
 )
 
 get_params = GetParameters(
     baseline_window_scale=20.0,
@@ -120,15 +119,14 @@
 cluster_params = ClusterParameters(
     min_cloud_size=50,
     min_points=3,
     min_size_scale_factor=0.05,
     min_size_lower_cutoff=10,
     cluster_selection_epsilon=10.0,
     circle_overlap_ratio=0.5,
-    fractional_charge_threshold=0.8,
     outlier_scale_factor=0.05,
 )
 
 estimate_params = EstimateParameters(
     min_total_trajectory_points=30, smoothing_factor=100.0
 )
 
@@ -191,8 +189,7 @@
 ### Logs and Output
 
 Spyral creates a set of logfiles when it is run (located in the log directory of the workspace). These logfiles can contain critical information describing the state of Spyral. In particular, if Spyral has a crash, the logfiles can be useful for determining what went wrong. A logfile is created for each process (including the parent process). The files are labeld by process number (or as parent in the case of the parent).
 
 ## Notebooks
 
 See the [spyral_notebooks](https://github.com/attpc/spyral_notebooks) repository for notebooks which demonstrate the behavior of the default Phases of Spyral.
-
```

