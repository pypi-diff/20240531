# Comparing `tmp/besos-2.2.2.tar.gz` & `tmp/besos-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "besos-2.2.2.tar", last modified: Sat Apr  6 22:16:19 2024, max compression
+gzip compressed data, was "besos-2.2.3.tar", last modified: Fri May 31 03:08:57 2024, max compression
```

## Comparing `besos-2.2.2.tar` & `besos-2.2.3.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-06 22:16:19.434650 besos-2.2.2/
--rw-r--r--   0 user      (1000) user      (1000)    35069 2023-09-02 17:28:20.000000 besos-2.2.2/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)       12 2023-09-02 17:28:20.000000 besos-2.2.2/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     8426 2024-04-06 22:16:19.431650 besos-2.2.2/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     6475 2023-09-02 17:28:20.000000 besos-2.2.2/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-06 22:16:19.142648 besos-2.2.2/besos/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-06 22:16:19.190648 besos-2.2.2/besos/.ipynb_checkpoints/
--rw-r--r--   0 user      (1000) user      (1000)      761 2023-09-02 17:28:20.000000 besos-2.2.2/besos/.ipynb_checkpoints/besos_utils-checkpoint.py
--rw-r--r--   0 user      (1000) user      (1000)     2824 2023-09-02 17:28:20.000000 besos-2.2.2/besos/.ipynb_checkpoints/config-checkpoint.py
--rw-r--r--   0 user      (1000) user      (1000)    11982 2023-09-02 19:14:29.000000 besos-2.2.2/besos/.ipynb_checkpoints/eplus_funcs-checkpoint.py
--rw-r--r--   0 user      (1000) user      (1000)    28138 2023-09-02 17:28:20.000000 besos-2.2.2/besos/.ipynb_checkpoints/eppy_funcs-checkpoint.py
--rw-r--r--   0 user      (1000) user      (1000)    35684 2023-10-30 00:44:53.000000 besos-2.2.2/besos/.ipynb_checkpoints/evaluator-checkpoint.py
--rw-r--r--   0 user      (1000) user      (1000)    23107 2023-10-29 18:07:36.000000 besos-2.2.2/besos/.ipynb_checkpoints/parameters-checkpoint.py
--rw-r--r--   0 user      (1000) user      (1000)     4719 2023-10-30 00:54:36.000000 besos-2.2.2/besos/.ipynb_checkpoints/pyehub_funcs-checkpoint.py
--rw-r--r--   0 user      (1000) user      (1000)    23926 2023-09-02 19:14:36.000000 besos-2.2.2/besos/.ipynb_checkpoints/sampling-checkpoint.py
--rw-r--r--   0 user      (1000) user      (1000)    17589 2023-09-02 17:28:20.000000 besos-2.2.2/besos/IDF_class.py
--rw-r--r--   0 user      (1000) user      (1000)     4818 2023-09-02 17:28:20.000000 besos-2.2.2/besos/IO_Objects.py
--rw-r--r--   0 user      (1000) user      (1000)       98 2023-09-02 17:28:20.000000 besos-2.2.2/besos/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-06 22:16:19.255648 besos-2.2.2/besos/__pycache__/
--rw-r--r--   0 user      (1000) user      (1000)    14604 2023-09-02 18:23:33.000000 besos-2.2.2/besos/__pycache__/IDF_class.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)     6844 2023-09-02 18:23:33.000000 besos-2.2.2/besos/__pycache__/IO_Objects.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)      250 2023-09-02 18:23:09.000000 besos-2.2.2/besos/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)      995 2023-09-02 18:24:32.000000 besos-2.2.2/besos/__pycache__/besos_utils.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)      397 2023-09-02 18:23:33.000000 besos-2.2.2/besos/__pycache__/besostypes.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)     1657 2023-09-02 18:23:33.000000 besos-2.2.2/besos/__pycache__/config.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)      402 2023-09-02 18:49:25.000000 besos-2.2.2/besos/__pycache__/dask_utils.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)     8826 2023-10-29 18:10:49.000000 besos-2.2.2/besos/__pycache__/eplus_funcs.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)    21973 2023-09-02 18:23:09.000000 besos-2.2.2/besos/__pycache__/eppy_funcs.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)     1769 2023-09-02 18:23:33.000000 besos-2.2.2/besos/__pycache__/errors.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)    29998 2023-10-31 06:10:03.000000 besos-2.2.2/besos/__pycache__/evaluator.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)    15992 2023-10-29 18:10:48.000000 besos-2.2.2/besos/__pycache__/objectives.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)    12215 2023-09-02 18:49:25.000000 besos-2.2.2/besos/__pycache__/optimizer.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)    22598 2023-10-29 18:10:50.000000 besos-2.2.2/besos/__pycache__/parameters.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)    14204 2023-09-02 18:24:32.000000 besos-2.2.2/besos/__pycache__/problem.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)     2987 2023-10-31 06:09:41.000000 besos-2.2.2/besos/__pycache__/pyehub_funcs.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)    16306 2023-09-02 19:33:27.000000 besos-2.2.2/besos/__pycache__/sampling.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)    17484 2023-09-02 18:55:05.000000 besos-2.2.2/besos/__pycache__/weather.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)      761 2023-09-02 17:28:20.000000 besos-2.2.2/besos/besos_utils.py
--rw-r--r--   0 user      (1000) user      (1000)      272 2023-09-02 17:28:20.000000 besos-2.2.2/besos/besostypes.py
--rw-r--r--   0 user      (1000) user      (1000)     2824 2023-09-02 17:28:20.000000 besos-2.2.2/besos/config.py
--rw-r--r--   0 user      (1000) user      (1000)      221 2023-09-02 17:28:20.000000 besos-2.2.2/besos/dask_utils.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-06 22:16:19.384650 besos-2.2.2/besos/data/
--rw-r--r--   0 user      (1000) user      (1000)  4378096 2023-09-02 17:28:20.000000 besos-2.2.2/besos/data/Custom_Long_Fields.idd
--rw-r--r--   0 user      (1000) user      (1000)  9591568 2023-09-02 17:28:20.000000 besos-2.2.2/besos/data/Energy+.schema.epJSON
--rw-r--r--   0 user      (1000) user      (1000)   230178 2023-09-02 17:28:20.000000 besos-2.2.2/besos/data/example_bad_idf.idf
--rw-r--r--   0 user      (1000) user      (1000)   293683 2023-09-02 17:28:20.000000 besos-2.2.2/besos/data/example_building.epJSON
--rw-r--r--   0 user      (1000) user      (1000)  1639985 2023-09-02 17:28:20.000000 besos-2.2.2/besos/data/example_epw.epw
--rw-r--r--   0 user      (1000) user      (1000)  4364459 2023-09-02 17:28:20.000000 besos-2.2.2/besos/data/example_idd.idd
--rw-r--r--   0 user      (1000) user      (1000)   230171 2023-09-02 17:28:20.000000 besos-2.2.2/besos/data/example_idf.idf
--rw-r--r--   0 user      (1000) user      (1000)    38772 2023-09-02 17:28:20.000000 besos-2.2.2/besos/data/example_xlsx.xlsx
--rw-r--r--   0 user      (1000) user      (1000)    83738 2023-09-02 17:28:20.000000 besos-2.2.2/besos/data/unexpanded.idf
--rw-r--r--   0 user      (1000) user      (1000)    11982 2023-10-29 18:07:36.000000 besos-2.2.2/besos/eplus_funcs.py
--rw-r--r--   0 user      (1000) user      (1000)    28138 2023-09-02 17:28:20.000000 besos-2.2.2/besos/eppy_funcs.py
--rw-r--r--   0 user      (1000) user      (1000)     1564 2023-09-02 17:28:20.000000 besos-2.2.2/besos/errors.py
--rw-r--r--   0 user      (1000) user      (1000)    35617 2024-04-06 22:09:53.000000 besos-2.2.2/besos/evaluator.py
--rw-r--r--   0 user      (1000) user      (1000)     4223 2023-09-02 17:28:20.000000 besos-2.2.2/besos/example_ui.py
--rw-r--r--   0 user      (1000) user      (1000)    19371 2024-04-06 22:09:53.000000 besos-2.2.2/besos/objectives.py
--rw-r--r--   0 user      (1000) user      (1000)    15486 2023-09-02 17:28:20.000000 besos-2.2.2/besos/optimizer.py
--rw-r--r--   0 user      (1000) user      (1000)    23107 2023-10-29 18:07:36.000000 besos-2.2.2/besos/parameters.py
--rw-r--r--   0 user      (1000) user      (1000)    16842 2023-09-02 17:28:20.000000 besos-2.2.2/besos/problem.py
--rw-r--r--   0 user      (1000) user      (1000)     4579 2024-04-06 22:09:53.000000 besos-2.2.2/besos/pyehub_funcs.py
--rw-r--r--   0 user      (1000) user      (1000)    23926 2023-09-02 19:14:36.000000 besos-2.2.2/besos/sampling.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-06 22:16:19.419650 besos-2.2.2/besos.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     8426 2024-04-06 22:16:19.000000 besos-2.2.2/besos.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     2309 2024-04-06 22:16:19.000000 besos-2.2.2/besos.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2024-04-06 22:16:19.000000 besos-2.2.2/besos.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)      384 2024-04-06 22:16:19.000000 besos-2.2.2/besos.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        6 2024-04-06 22:16:19.000000 besos-2.2.2/besos.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2024-04-06 22:16:19.434650 besos-2.2.2/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     1183 2024-04-06 22:09:53.000000 besos-2.2.2/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-06 22:16:19.416650 besos-2.2.2/test/
--rw-r--r--   0 user      (1000) user      (1000)     3327 2023-10-30 00:59:47.000000 besos-2.2.2/test/test_adaptive_surrogate.py
--rw-r--r--   0 user      (1000) user      (1000)     1300 2023-09-02 17:28:21.000000 besos-2.2.2/test/test_eplus_funcs.py
--rw-r--r--   0 user      (1000) user      (1000)     2884 2023-10-31 03:04:31.000000 besos-2.2.2/test/test_eppy_funcs.py
--rw-r--r--   0 user      (1000) user      (1000)     6710 2023-10-29 18:07:37.000000 besos-2.2.2/test/test_error_handling.py
--rw-r--r--   0 user      (1000) user      (1000)    12856 2023-10-31 03:04:31.000000 besos-2.2.2/test/test_evaluators.py
--rw-r--r--   0 user      (1000) user      (1000)     2522 2023-09-02 17:28:21.000000 besos-2.2.2/test/test_fit_surrogate.py
--rw-r--r--   0 user      (1000) user      (1000)     1642 2023-10-29 18:07:37.000000 besos-2.2.2/test/test_mixed_optimisation.py
--rw-r--r--   0 user      (1000) user      (1000)     3121 2023-09-02 17:28:21.000000 besos-2.2.2/test/test_objectives_constraints.py
--rw-r--r--   0 user      (1000) user      (1000)     7785 2023-10-29 18:07:37.000000 besos-2.2.2/test/test_parameter.py
--rw-r--r--   0 user      (1000) user      (1000)     3052 2023-10-29 18:07:37.000000 besos-2.2.2/test/test_platypus.py
--rw-r--r--   0 user      (1000) user      (1000)     1182 2023-10-29 18:07:37.000000 besos-2.2.2/test/test_rbfopt.py
--rw-r--r--   0 user      (1000) user      (1000)     4687 2023-09-02 17:28:21.000000 besos-2.2.2/test/test_selectors.py
--rw-r--r--   0 user      (1000) user      (1000)     3711 2023-09-02 19:14:36.000000 besos-2.2.2/test/test_simulation.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-31 03:08:57.885775 besos-2.2.3/
+-rw-r--r--   0 user      (1000) user      (1000)    35069 2023-09-02 17:28:20.000000 besos-2.2.3/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)       12 2023-09-02 17:28:20.000000 besos-2.2.3/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     8426 2024-05-31 03:08:57.883775 besos-2.2.3/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     6475 2023-09-02 17:28:20.000000 besos-2.2.3/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-31 03:08:57.310770 besos-2.2.3/besos/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-31 03:08:57.346770 besos-2.2.3/besos/.ipynb_checkpoints/
+-rw-r--r--   0 user      (1000) user      (1000)      761 2023-09-02 17:28:20.000000 besos-2.2.3/besos/.ipynb_checkpoints/besos_utils-checkpoint.py
+-rw-r--r--   0 user      (1000) user      (1000)     2824 2023-09-02 17:28:20.000000 besos-2.2.3/besos/.ipynb_checkpoints/config-checkpoint.py
+-rw-r--r--   0 user      (1000) user      (1000)    11982 2023-09-02 19:14:29.000000 besos-2.2.3/besos/.ipynb_checkpoints/eplus_funcs-checkpoint.py
+-rw-r--r--   0 user      (1000) user      (1000)    28138 2023-09-02 17:28:20.000000 besos-2.2.3/besos/.ipynb_checkpoints/eppy_funcs-checkpoint.py
+-rw-r--r--   0 user      (1000) user      (1000)    35684 2023-10-30 00:44:53.000000 besos-2.2.3/besos/.ipynb_checkpoints/evaluator-checkpoint.py
+-rw-r--r--   0 user      (1000) user      (1000)    23107 2023-10-29 18:07:36.000000 besos-2.2.3/besos/.ipynb_checkpoints/parameters-checkpoint.py
+-rw-r--r--   0 user      (1000) user      (1000)     4719 2023-10-30 00:54:36.000000 besos-2.2.3/besos/.ipynb_checkpoints/pyehub_funcs-checkpoint.py
+-rw-r--r--   0 user      (1000) user      (1000)    23926 2023-09-02 19:14:36.000000 besos-2.2.3/besos/.ipynb_checkpoints/sampling-checkpoint.py
+-rw-r--r--   0 user      (1000) user      (1000)    17589 2023-09-02 17:28:20.000000 besos-2.2.3/besos/IDF_class.py
+-rw-r--r--   0 user      (1000) user      (1000)     4818 2023-09-02 17:28:20.000000 besos-2.2.3/besos/IO_Objects.py
+-rw-r--r--   0 user      (1000) user      (1000)       98 2023-09-02 17:28:20.000000 besos-2.2.3/besos/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-31 03:08:57.391770 besos-2.2.3/besos/__pycache__/
+-rw-r--r--   0 user      (1000) user      (1000)    14604 2023-09-02 18:23:33.000000 besos-2.2.3/besos/__pycache__/IDF_class.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)     6844 2023-09-02 18:23:33.000000 besos-2.2.3/besos/__pycache__/IO_Objects.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)      250 2023-09-02 18:23:09.000000 besos-2.2.3/besos/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)      995 2023-09-02 18:24:32.000000 besos-2.2.3/besos/__pycache__/besos_utils.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)      397 2023-09-02 18:23:33.000000 besos-2.2.3/besos/__pycache__/besostypes.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)     1657 2023-09-02 18:23:33.000000 besos-2.2.3/besos/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)      402 2023-09-02 18:49:25.000000 besos-2.2.3/besos/__pycache__/dask_utils.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)     8826 2023-10-29 18:10:49.000000 besos-2.2.3/besos/__pycache__/eplus_funcs.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)    21973 2023-09-02 18:23:09.000000 besos-2.2.3/besos/__pycache__/eppy_funcs.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)     1769 2023-09-02 18:23:33.000000 besos-2.2.3/besos/__pycache__/errors.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)    29998 2024-04-13 17:41:30.000000 besos-2.2.3/besos/__pycache__/evaluator.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)    16061 2024-04-13 17:25:57.000000 besos-2.2.3/besos/__pycache__/objectives.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)    12215 2023-09-02 18:49:25.000000 besos-2.2.3/besos/__pycache__/optimizer.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)    22598 2023-10-29 18:10:50.000000 besos-2.2.3/besos/__pycache__/parameters.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)    14204 2023-09-02 18:24:32.000000 besos-2.2.3/besos/__pycache__/problem.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)     2987 2024-04-13 17:41:15.000000 besos-2.2.3/besos/__pycache__/pyehub_funcs.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)    16306 2023-09-02 19:33:27.000000 besos-2.2.3/besos/__pycache__/sampling.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)    17484 2023-09-02 18:55:05.000000 besos-2.2.3/besos/__pycache__/weather.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)      761 2023-09-02 17:28:20.000000 besos-2.2.3/besos/besos_utils.py
+-rw-r--r--   0 user      (1000) user      (1000)      272 2023-09-02 17:28:20.000000 besos-2.2.3/besos/besostypes.py
+-rw-r--r--   0 user      (1000) user      (1000)     2824 2023-09-02 17:28:20.000000 besos-2.2.3/besos/config.py
+-rw-r--r--   0 user      (1000) user      (1000)      221 2023-09-02 17:28:20.000000 besos-2.2.3/besos/dask_utils.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-31 03:08:57.489771 besos-2.2.3/besos/data/
+-rw-r--r--   0 user      (1000) user      (1000)  4378096 2023-09-02 17:28:20.000000 besos-2.2.3/besos/data/Custom_Long_Fields.idd
+-rw-r--r--   0 user      (1000) user      (1000)  9591568 2023-09-02 17:28:20.000000 besos-2.2.3/besos/data/Energy+.schema.epJSON
+-rw-r--r--   0 user      (1000) user      (1000)   230178 2023-09-02 17:28:20.000000 besos-2.2.3/besos/data/example_bad_idf.idf
+-rw-r--r--   0 user      (1000) user      (1000)   293683 2023-09-02 17:28:20.000000 besos-2.2.3/besos/data/example_building.epJSON
+-rw-r--r--   0 user      (1000) user      (1000)  1639985 2023-09-02 17:28:20.000000 besos-2.2.3/besos/data/example_epw.epw
+-rw-r--r--   0 user      (1000) user      (1000)  4364459 2023-09-02 17:28:20.000000 besos-2.2.3/besos/data/example_idd.idd
+-rw-r--r--   0 user      (1000) user      (1000)   230171 2023-09-02 17:28:20.000000 besos-2.2.3/besos/data/example_idf.idf
+-rw-r--r--   0 user      (1000) user      (1000)    38772 2023-09-02 17:28:20.000000 besos-2.2.3/besos/data/example_xlsx.xlsx
+-rw-r--r--   0 user      (1000) user      (1000)    83738 2023-09-02 17:28:20.000000 besos-2.2.3/besos/data/unexpanded.idf
+-rw-r--r--   0 user      (1000) user      (1000)    11982 2023-10-29 18:07:36.000000 besos-2.2.3/besos/eplus_funcs.py
+-rw-r--r--   0 user      (1000) user      (1000)    28138 2023-09-02 17:28:20.000000 besos-2.2.3/besos/eppy_funcs.py
+-rw-r--r--   0 user      (1000) user      (1000)     1564 2023-09-02 17:28:20.000000 besos-2.2.3/besos/errors.py
+-rw-r--r--   0 user      (1000) user      (1000)    35617 2024-04-06 22:09:53.000000 besos-2.2.3/besos/evaluator.py
+-rw-r--r--   0 user      (1000) user      (1000)     4223 2023-09-02 17:28:20.000000 besos-2.2.3/besos/example_ui.py
+-rw-r--r--   0 user      (1000) user      (1000)    19371 2024-04-06 22:09:53.000000 besos-2.2.3/besos/objectives.py
+-rw-r--r--   0 user      (1000) user      (1000)    15486 2023-09-02 17:28:20.000000 besos-2.2.3/besos/optimizer.py
+-rw-r--r--   0 user      (1000) user      (1000)    23107 2023-10-29 18:07:36.000000 besos-2.2.3/besos/parameters.py
+-rw-r--r--   0 user      (1000) user      (1000)    16842 2023-09-02 17:28:20.000000 besos-2.2.3/besos/problem.py
+-rw-r--r--   0 user      (1000) user      (1000)     4579 2024-04-06 22:09:53.000000 besos-2.2.3/besos/pyehub_funcs.py
+-rw-r--r--   0 user      (1000) user      (1000)    23923 2024-05-31 03:05:16.000000 besos-2.2.3/besos/sampling.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-31 03:08:57.877775 besos-2.2.3/besos.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     8426 2024-05-31 03:08:57.000000 besos-2.2.3/besos.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     2309 2024-05-31 03:08:57.000000 besos-2.2.3/besos.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-05-31 03:08:57.000000 besos-2.2.3/besos.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)      384 2024-05-31 03:08:57.000000 besos-2.2.3/besos.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        6 2024-05-31 03:08:57.000000 besos-2.2.3/besos.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2024-05-31 03:08:57.885775 besos-2.2.3/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     1183 2024-05-31 03:05:16.000000 besos-2.2.3/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-31 03:08:57.828774 besos-2.2.3/test/
+-rw-r--r--   0 user      (1000) user      (1000)     3327 2023-10-30 00:59:47.000000 besos-2.2.3/test/test_adaptive_surrogate.py
+-rw-r--r--   0 user      (1000) user      (1000)     1300 2023-09-02 17:28:21.000000 besos-2.2.3/test/test_eplus_funcs.py
+-rw-r--r--   0 user      (1000) user      (1000)     2884 2023-10-31 03:04:31.000000 besos-2.2.3/test/test_eppy_funcs.py
+-rw-r--r--   0 user      (1000) user      (1000)     6710 2023-10-29 18:07:37.000000 besos-2.2.3/test/test_error_handling.py
+-rw-r--r--   0 user      (1000) user      (1000)    12856 2023-10-31 03:04:31.000000 besos-2.2.3/test/test_evaluators.py
+-rw-r--r--   0 user      (1000) user      (1000)     2522 2023-09-02 17:28:21.000000 besos-2.2.3/test/test_fit_surrogate.py
+-rw-r--r--   0 user      (1000) user      (1000)     1642 2023-10-29 18:07:37.000000 besos-2.2.3/test/test_mixed_optimisation.py
+-rw-r--r--   0 user      (1000) user      (1000)     3121 2023-09-02 17:28:21.000000 besos-2.2.3/test/test_objectives_constraints.py
+-rw-r--r--   0 user      (1000) user      (1000)     7785 2023-10-29 18:07:37.000000 besos-2.2.3/test/test_parameter.py
+-rw-r--r--   0 user      (1000) user      (1000)     3052 2023-10-29 18:07:37.000000 besos-2.2.3/test/test_platypus.py
+-rw-r--r--   0 user      (1000) user      (1000)     1182 2023-10-29 18:07:37.000000 besos-2.2.3/test/test_rbfopt.py
+-rw-r--r--   0 user      (1000) user      (1000)     4687 2023-09-02 17:28:21.000000 besos-2.2.3/test/test_selectors.py
+-rw-r--r--   0 user      (1000) user      (1000)     3711 2023-09-02 19:14:36.000000 besos-2.2.3/test/test_simulation.py
```

### Comparing `besos-2.2.2/LICENSE` & `besos-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/PKG-INFO` & `besos-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: besos
-Version: 2.2.2
+Version: 2.2.3
 Summary: A library for Building and Energy Simulation, Optimization and Surrogate-modelling
 Home-page: https://gitlab.com/energyincities/besos
 Author: Ralph Evins
 Author-email: revins@uvic.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `besos-2.2.2/README.md` & `besos-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/.ipynb_checkpoints/besos_utils-checkpoint.py` & `besos-2.2.3/besos/.ipynb_checkpoints/besos_utils-checkpoint.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/.ipynb_checkpoints/config-checkpoint.py` & `besos-2.2.3/besos/.ipynb_checkpoints/config-checkpoint.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/.ipynb_checkpoints/eplus_funcs-checkpoint.py` & `besos-2.2.3/besos/.ipynb_checkpoints/eplus_funcs-checkpoint.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/.ipynb_checkpoints/eppy_funcs-checkpoint.py` & `besos-2.2.3/besos/.ipynb_checkpoints/eppy_funcs-checkpoint.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/.ipynb_checkpoints/evaluator-checkpoint.py` & `besos-2.2.3/besos/.ipynb_checkpoints/evaluator-checkpoint.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/.ipynb_checkpoints/parameters-checkpoint.py` & `besos-2.2.3/besos/.ipynb_checkpoints/parameters-checkpoint.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/.ipynb_checkpoints/pyehub_funcs-checkpoint.py` & `besos-2.2.3/besos/.ipynb_checkpoints/pyehub_funcs-checkpoint.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/.ipynb_checkpoints/sampling-checkpoint.py` & `besos-2.2.3/besos/.ipynb_checkpoints/sampling-checkpoint.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/IDF_class.py` & `besos-2.2.3/besos/IDF_class.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/IO_Objects.py` & `besos-2.2.3/besos/IO_Objects.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/__pycache__/IDF_class.cpython-38.pyc` & `besos-2.2.3/besos/__pycache__/IDF_class.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/__pycache__/IO_Objects.cpython-38.pyc` & `besos-2.2.3/besos/__pycache__/IO_Objects.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/__pycache__/besos_utils.cpython-38.pyc` & `besos-2.2.3/besos/__pycache__/besos_utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/__pycache__/config.cpython-38.pyc` & `besos-2.2.3/besos/__pycache__/config.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/__pycache__/eplus_funcs.cpython-38.pyc` & `besos-2.2.3/besos/__pycache__/eplus_funcs.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/__pycache__/eppy_funcs.cpython-38.pyc` & `besos-2.2.3/besos/__pycache__/eppy_funcs.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/__pycache__/errors.cpython-38.pyc` & `besos-2.2.3/besos/__pycache__/errors.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/__pycache__/evaluator.cpython-38.pyc` & `besos-2.2.3/besos/__pycache__/evaluator.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Oct 31 03:04:31 2023 UTC, .py size: 35685 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 bf6e 4065 658b 0000  U........n@ee...
+00000000: 550d 0d0a 0000 0000 31c8 1166 218b 0000  U.......1..f!...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 a201 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6403 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 6d07 5a07 6d08 5a08 0100 6401 6404 6c09  m.Z.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6401 6405 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
@@ -1057,15 +1057,15 @@
 00004200: 706c 6163 654e 2907 7260 0000 0072 3200  placeN).r`...r2.
 00004210: 0000 da05 746f 5f64 6672 8b00 0000 7292  ....to_dfr....r.
 00004220: 0000 0072 c400 0000 da0f 6472 6f70 5f64  ...r......drop_d
 00004230: 7570 6c69 6361 7465 7329 0472 3a00 0000  uplicates).r:...
 00004240: 72c4 0000 0072 c700 0000 da08 6e65 775f  r....r......new_
 00004250: 6461 7461 721e 0000 0072 1e00 0000 721f  datar....r....r.
 00004260: 0000 00da 0b61 7070 656e 645f 6461 7461  .....append_data
-00004270: 1202 0000 730a 0000 0000 0708 0214 0216  ....s...........
+00004270: 1202 0000 730a 0000 0000 0708 0214 0116  ....s...........
 00004280: 0104 017a 1641 6461 7074 6976 6553 522e  ...z.AdaptiveSR.
 00004290: 6170 7065 6e64 5f64 6174 6129 02da 0e6e  append_data)...n
 000042a0: 756d 5f64 6174 6170 6f69 6e74 7372 3d00  um_datapointsr=.
 000042b0: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
 000042c0: 0000 0001 0000 0043 0000 0073 0800 0000  .......C...s....
 000042d0: 7400 8201 6401 5300 2902 7aef 4765 6e65  t...d.S.).z.Gene
 000042e0: 7261 7465 7320 6461 7461 2074 6861 7420  rates data that 
@@ -1081,15 +1081,15 @@
 00004380: 2020 3a72 6574 7572 6e3a 2074 6865 2064    :return: the d
 00004390: 6174 6170 6f69 6e74 7320 6765 6e65 7261  atapoints genera
 000043a0: 7465 642c 2069 6e20 736f 6d65 2074 6162  ted, in some tab
 000043b0: 756c 6172 2064 6174 6173 7472 7563 7475  ular datastructu
 000043c0: 7265 0a20 2020 2020 2020 204e 2901 724c  re.        N).rL
 000043d0: 0000 0029 0272 3a00 0000 72ce 0000 0072  ...).r:...r....r
 000043e0: 1e00 0000 721e 0000 0072 1f00 0000 da0a  ....r....r......
-000043f0: 6765 745f 696e 6669 6c6c 2102 0000 7302  get_infill!...s.
+000043f0: 6765 745f 696e 6669 6c6c 2002 0000 7302  get_infill ...s.
 00004400: 0000 0000 067a 1541 6461 7074 6976 6553  .....z.AdaptiveS
 00004410: 522e 6765 745f 696e 6669 6c6c 2902 72c4  R.get_infill).r.
 00004420: 0000 0072 3d00 0000 6302 0000 0000 0000  ...r=...c.......
 00004430: 0000 0000 0006 0000 0005 0000 0043 0000  .............C..
 00004440: 0073 7400 0000 7c00 6a00 7d02 7c00 6a01  .st...|.j.}.|.j.
 00004450: 6a02 7c01 6401 6402 6403 6703 6404 8d02  j.|.d.d.d.g.d...
 00004460: 5c02 7d03 7d04 7c04 6401 6701 6b02 7246  \.}.}.|.d.g.k.rF
@@ -1114,15 +1114,15 @@
 00004590: da12 6765 745f 6672 6f6d 5f72 6566 6572  ..get_from_refer
 000045a0: 656e 6365 728b 0000 0072 9200 0000 72cd  encer....r....r.
 000045b0: 0000 0072 c300 0000 da05 7472 6169 6eda  ...r......train.
 000045c0: 0c75 7064 6174 655f 6d6f 6465 6c29 0672  .update_model).r
 000045d0: 3a00 0000 72c4 0000 005a 066f 6c64 5f64  :...r....Z.old_d
 000045e0: 6672 6700 0000 72c2 0000 0072 8700 0000  frg...r....r....
 000045f0: 721e 0000 0072 1e00 0000 721f 0000 00da  r....r....r.....
-00004600: 0964 6f5f 696e 6669 6c6c 2902 0000 7318  .do_infill)...s.
+00004600: 0964 6f5f 696e 6669 6c6c 2802 0000 7318  .do_infill(...s.
 00004610: 0000 0000 0606 0106 0102 0008 ff0a 030a  ................
 00004620: 010a 0112 010a 010a 010a 027a 1441 6461  ...........z.Ada
 00004630: 7074 6976 6553 522e 646f 5f69 6e66 696c  ptiveSR.do_infil
 00004640: 6c29 0372 cc00 0000 da08 6f6c 645f 6461  l).r......old_da
 00004650: 7461 723d 0000 0063 0300 0000 0000 0000  tar=...c........
 00004660: 0000 0000 0300 0000 0200 0000 4300 0000  ............C...
 00004670: 730c 0000 007c 00a0 00a1 0001 0064 0153  s....|.......d.S
@@ -1142,15 +1142,15 @@
 00004750: 696e 7075 7473 2061 6e64 206f 7574 7075  inputs and outpu
 00004760: 7473 2077 6974 686f 7574 2074 6865 206e  ts without the n
 00004770: 6577 2064 6174 610a 2020 2020 2020 2020  ew data.        
 00004780: 3a72 6574 7572 6e3a 204e 6f6e 650a 2020  :return: None.  
 00004790: 2020 2020 2020 4e29 0172 d200 0000 2903        N).r....).
 000047a0: 723a 0000 0072 cc00 0000 72d5 0000 0072  r:...r....r....r
 000047b0: 1e00 0000 721e 0000 0072 1f00 0000 72d3  ....r....r....r.
-000047c0: 0000 003c 0200 0073 0200 0000 0009 7a17  ...<...s......z.
+000047c0: 0000 003b 0200 0073 0200 0000 0009 7a17  ...;...s......z.
 000047d0: 4164 6170 7469 7665 5352 2e75 7064 6174  AdaptiveSR.updat
 000047e0: 655f 6d6f 6465 6c63 0200 0000 0000 0000  e_modelc........
 000047f0: 0000 0000 0400 0000 0600 0000 4300 0000  ............C...
 00004800: 733a 0000 007c 006a 00a0 017c 00a0 027c  s:...|.j...|...|
 00004810: 01a1 0164 01a1 027d 027c 00a0 037c 02a1  ...d...}.|...|..
 00004820: 017d 037c 00a0 0474 056a 067c 027c 0367  .}.|...t.j.|.|.g
 00004830: 0264 0264 038d 02a1 0101 0064 0453 0029  .d.d.......d.S.)
@@ -1167,26 +1167,26 @@
 000048e0: 7572 6e3a 204e 6f6e 650a 2020 2020 2020  urn: None.      
 000048f0: 2020 7254 0000 0072 6600 0000 728a 0000    rT...rf...r...
 00004900: 004e 2907 7232 0000 0072 ca00 0000 72cf  .N).r2...r....r.
 00004910: 0000 0072 d100 0000 72d4 0000 0072 8b00  ...r....r....r..
 00004920: 0000 7292 0000 0029 0472 3a00 0000 72ce  ..r....).r:...r.
 00004930: 0000 0072 5400 0000 7287 0000 0072 1e00  ...rT...r....r..
 00004940: 0000 721e 0000 0072 1f00 0000 da06 696e  ..r....r......in
-00004950: 6669 6c6c 4702 0000 7306 0000 0000 0614  fillG...s.......
+00004950: 6669 6c6c 4602 0000 7306 0000 0000 0614  fillF...s.......
 00004960: 010a 017a 1141 6461 7074 6976 6553 522e  ...z.AdaptiveSR.
 00004970: 696e 6669 6c6c 723c 0000 0063 0100 0000  infillr<...c....
 00004980: 0000 0000 0000 0000 0100 0000 0100 0000  ................
 00004990: 4300 0000 7304 0000 0064 0153 0029 027a  C...s....d.S.).z
 000049a0: 4847 656e 6572 6174 6573 2061 206e 6577  HGenerates a new
 000049b0: 206d 6f64 656c 2075 7369 6e67 2074 6865   model using the
 000049c0: 2073 746f 7265 6420 6461 7461 2c20 616e   stored data, an
 000049d0: 6420 7374 6f72 6573 2069 7420 6173 2073  d stores it as s
 000049e0: 656c 662e 6d6f 6465 6c4e 721e 0000 0072  elf.modelNr....r
 000049f0: 5f00 0000 721e 0000 0072 1e00 0000 721f  _...r....r....r.
-00004a00: 0000 0072 d200 0000 5102 0000 7302 0000  ...r....Q...s...
+00004a00: 0000 0072 d200 0000 5002 0000 7302 0000  ...r....P...s...
 00004a10: 0000 037a 1041 6461 7074 6976 6553 522e  ...z.AdaptiveSR.
 00004a20: 7472 6169 6e72 4d00 0000 6302 0000 0000  trainrM...c.....
 00004a30: 0000 0000 0000 0003 0000 0001 0000 004b  ...............K
 00004a40: 0000 0073 0400 0000 6401 5300 2902 7ad2  ...s....d.S.).z.
 00004a50: 4576 616c 7561 7465 7320 6120 7369 6e67  Evaluates a sing
 00004a60: 6c65 2069 6e70 7574 2070 6f69 6e74 0a0a  le input point..
 00004a70: 2020 2020 2020 2020 3a70 6172 616d 2076          :param v
@@ -1198,15 +1198,15 @@
 00004ad0: 6e74 732e 0a20 2020 2020 2020 203a 7265  nts..        :re
 00004ae0: 7475 726e 3a20 4120 7475 706c 6520 6f66  turn: A tuple of
 00004af0: 2074 6865 2070 7265 6469 6374 6564 206f   the predicted o
 00004b00: 7574 7075 7473 2066 6f72 2074 6869 7320  utputs for this 
 00004b10: 6461 7461 706f 696e 740a 2020 2020 2020  datapoint.      
 00004b20: 2020 4e72 1e00 0000 7250 0000 0072 1e00    Nr....rP...r..
 00004b30: 0000 721e 0000 0072 1f00 0000 7252 0000  ..r....r....rR..
-00004b40: 0056 0200 0073 0200 0000 0008 7a16 4164  .V...s......z.Ad
+00004b40: 0055 0200 0073 0200 0000 0008 7a16 4164  .U...s......z.Ad
 00004b50: 6170 7469 7665 5352 2e65 7661 6c5f 7369  aptiveSR.eval_si
 00004b60: 6e67 6c65 2902 da01 5872 3d00 0000 6302  ngle)...Xr=...c.
 00004b70: 0000 0000 0000 0000 0000 0003 0000 0004  ................
 00004b80: 0000 0043 0000 0073 1a00 0000 7c00 6a00  ...C...s....|.j.
 00004b90: a001 7c01 6401 a102 7d02 7c00 6a02 a003  ..|.d...}.|.j...
 00004ba0: 7c02 a101 5300 2902 7ade 5573 6520 7468  |...S.).z.Use th
 00004bb0: 6520 7265 6665 7265 6e63 6520 6576 616c  e reference eval
@@ -1222,15 +1222,15 @@
 00004c50: 6146 7261 6d65 2063 6f6e 7461 696e 696e  aFrame containin
 00004c60: 6720 7468 6520 7265 7375 6c74 7320 6f66  g the results of
 00004c70: 2074 6865 2064 6174 6170 6f69 6e74 730a   the datapoints.
 00004c80: 2020 2020 2020 2020 7254 0000 0029 0472          rT...).r
 00004c90: 3200 0000 72ca 0000 0072 c000 0000 7295  2...r....r....r.
 00004ca0: 0000 0029 0372 3a00 0000 72d7 0000 0072  ...).r:...r....r
 00004cb0: 6700 0000 721e 0000 0072 1e00 0000 721f  g...r....r....r.
-00004cc0: 0000 0072 d100 0000 6002 0000 7304 0000  ...r....`...s...
+00004cc0: 0000 0072 d100 0000 5f02 0000 7304 0000  ...r...._...s...
 00004cd0: 0000 060e 017a 1d41 6461 7074 6976 6553  .....z.AdaptiveS
 00004ce0: 522e 6765 745f 6672 6f6d 5f72 6566 6572  R.get_from_refer
 00004cf0: 656e 6365 2903 4e72 2f00 0000 4e29 0154  ence).Nr/...N).T
 00004d00: 2901 4e29 1e72 ac00 0000 72ad 0000 0072  ).N).r....r....r
 00004d10: ae00 0000 72af 0000 0072 0800 0000 72b2  ....r....r....r.
 00004d20: 0000 0072 6d00 0000 da05 6172 7261 795a  ...rm.....arrayZ
 00004d30: 0774 6162 756c 6172 722e 0000 0072 b000  .tabularr....r..
@@ -1240,15 +1240,15 @@
 00004d70: 0000 72a4 0000 0072 cf00 0000 72d4 0000  ..r....r....r...
 00004d80: 0072 d300 0000 72d6 0000 0072 0300 0000  .r....r....r....
 00004d90: 72d2 0000 0072 0700 0000 7252 0000 0072  r....r....rR...r
 00004da0: d100 0000 72bb 0000 0072 1e00 0000 721e  ....r....r....r.
 00004db0: 0000 0072 b900 0000 721f 0000 0072 bf00  ...r....r....r..
 00004dc0: 0000 d301 0000 7330 0000 0008 0104 220e  ......s0......".
 00004dd0: 0400 0100 0100 fc02 0202 0102 0102 fc10  ................
-00004de0: 1202 010a 0304 0110 0314 0f10 0810 1314  ................
+00004de0: 1202 010a 0304 0110 0314 0e10 0810 1314  ................
 00004df0: 0b10 0a02 0110 0402 0112 0972 bf00 0000  ...........r....
 00004e00: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00004e10: 000c 0000 0000 0000 0073 f400 0000 6500  .........s....e.
 00004e20: 5a01 6400 5a02 6401 5a03 6504 6a05 6402  Z.d.Z.d.Z.e.j.d.
 00004e30: 1900 6504 6a06 6504 6a07 6403 6404 6404  ..e.j.e.j.d.d.d.
 00004e40: 6405 6404 6608 6404 6406 9c01 6508 6509  d.d.f.d.d...e.e.
 00004e50: 6509 6509 650a 650b 650c 1900 650d 6509  e.e.e.e.e...e.e.
@@ -1395,15 +1395,15 @@
 00005720: 7272 b000 0000 da08 656e 6473 7769 7468  rr......endswith
 00005730: 72dc 0000 005a 0c65 7077 5f63 6f6e 7465  r....Z.epw_conte
 00005740: 6e74 7329 0c72 3a00 0000 7232 0000 0072  nts).r:...r2...r
 00005750: e700 0000 72dc 0000 0072 de00 0000 72df  ....r....r....r.
 00005760: 0000 0072 3300 0000 7234 0000 0072 bc00  ...r3...r4...r..
 00005770: 0000 7235 0000 0072 e000 0000 72dd 0000  ..r5...r....r...
 00005780: 0072 b900 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00005790: 723b 0000 006e 0200 0073 4a00 0000 0020  r;...n...sJ.... 
+00005790: 723b 0000 006d 0200 0073 4a00 0000 0020  r;...m...sJ.... 
 000057a0: 0601 0201 0201 0201 02fc 0606 0801 0802  ................
 000057b0: 0e01 0e01 0c02 0601 0e02 0603 1201 0201  ................
 000057c0: 02ff 0603 0401 0401 0201 0201 02ff 02ff  ................
 000057d0: 0406 0401 0401 0202 02fd 0405 1602 1a01  ................
 000057e0: 0201 08ff 0403 0603 7a14 4576 616c 7561  ........z.Evalua
 000057f0: 746f 7245 502e 5f5f 696e 6974 5f5f 4672  torEP.__init__Fr
 00005800: 6600 0000 7230 0000 0029 0272 de00 0000  f...r0...).r....
@@ -1470,15 +1470,15 @@
 00005bd0: 72de 0000 0072 b700 0000 7295 0000 0072  r....r....r....r
 00005be0: 9000 0000 727a 0000 0072 9300 0000 290b  ....rz...r....).
 00005bf0: 723a 0000 0072 6700 0000 7294 0000 0072  r:...rg...r....r
 00005c00: 6800 0000 7278 0000 0072 de00 0000 72ed  h...rx...r....r.
 00005c10: 0000 0072 5100 0000 5a09 7465 6d70 5f73  ...rQ...Z.temp_s
 00005c20: 656c 665a 0874 656d 705f 6f75 7472 5b00  elfZ.temp_outr[.
 00005c30: 0000 72b9 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-00005c40: 0072 9500 0000 be02 0000 7334 0000 0000  .r........s4....
+00005c40: 0072 9500 0000 bd02 0000 7334 0000 0000  .r........s4....
 00005c50: 1606 0104 0104 010a 0206 0102 ff02 0202  ................
 00005c60: 0102 0102 0102 0102 fa04 0702 f906 0a04  ................
 00005c70: 0104 010c 0002 0002 ff06 0304 0106 0104  ................
 00005c80: 0208 017a 1445 7661 6c75 6174 6f72 4550  ...z.EvaluatorEP
 00005c90: 2e64 665f 6170 706c 7929 0172 4e00 0000  .df_apply).rN...
 00005ca0: 6304 0000 0000 0000 0000 0000 000a 0000  c...............
 00005cb0: 0008 0000 000b 0000 0073 c400 0000 7c02  .........s....|.
@@ -1498,25 +1498,25 @@
 00005d90: 72df 0000 0072 dc00 0000 7233 0000 0072  r....r....r3...r
 00005da0: e000 0000 6301 0000 0000 0000 0000 0000  ....c...........
 00005db0: 0002 0000 0003 0000 0033 0000 0073 1600  .........3...s..
 00005dc0: 0000 7c00 5d0e 7d01 7c01 8800 8301 5600  ..|.].}.|.....V.
 00005dd0: 0100 7102 6400 5300 7218 0000 0072 1e00  ..q.d.S.r....r..
 00005de0: 0000 a902 721b 0000 00da 096f 626a 6563  ....r......objec
 00005df0: 7469 7665 a901 da07 7265 7375 6c74 7372  tive....resultsr
-00005e00: 1e00 0000 721f 0000 0072 2000 0000 0a03  ....r....r .....
+00005e00: 1e00 0000 721f 0000 0072 2000 0000 0903  ....r....r .....
 00005e10: 0000 7304 0000 0004 0002 007a 2a45 7661  ..s........z*Eva
 00005e20: 6c75 6174 6f72 4550 2e65 7661 6c5f 7369  luatorEP.eval_si
 00005e30: 6e67 6c65 2e3c 6c6f 6361 6c73 3e2e 3c67  ngle.<locals>.<g
 00005e40: 656e 6578 7072 3e63 0100 0000 0000 0000  enexpr>c........
 00005e50: 0000 0000 0200 0000 0300 0000 3300 0000  ............3...
 00005e60: 7316 0000 007c 005d 0e7d 017c 0188 0083  s....|.].}.|....
 00005e70: 0156 0001 0071 0264 0053 0072 1800 0000  .V...q.d.S.r....
 00005e80: 721e 0000 0029 0272 1b00 0000 da0a 636f  r....).r......co
 00005e90: 6e73 7472 6169 6e74 72f2 0000 0072 1e00  nstraintr....r..
-00005ea0: 0000 721f 0000 0072 2000 0000 0c03 0000  ..r....r .......
+00005ea0: 0000 721f 0000 0072 2000 0000 0b03 0000  ..r....r .......
 00005eb0: 7304 0000 0004 0002 004e 2911 72de 0000  s........N).r...
 00005ec0: 0072 df00 0000 da02 6566 da0c 6765 6e65  .r......ef..gene
 00005ed0: 7261 7465 5f64 6972 da1b 5f67 656e 6572  rate_dir.._gener
 00005ee0: 6174 655f 6275 696c 6469 6e67 5f66 726f  ate_building_fro
 00005ef0: 6d5f 726f 7772 e900 0000 da0c 7275 6e5f  m_rowr......run_
 00005f00: 6275 696c 6469 6e67 72dc 0000 0072 3300  buildingr....r3.
 00005f10: 0000 72e0 0000 0072 2a00 0000 7232 0000  ..r....r*...r2..
@@ -1525,25 +1525,25 @@
 00005f40: 6563 6f72 645f 7265 7375 6c74 7372 a200  ecord_resultsr..
 00005f50: 0000 290a 723a 0000 0072 4e00 0000 72de  ..).r:...rN...r.
 00005f60: 0000 0072 7800 0000 7251 0000 0072 df00  ...rx...rQ...r..
 00005f70: 0000 da10 6375 7272 656e 745f 6275 696c  ....current_buil
 00005f80: 6469 6e67 7287 0000 0072 a900 0000 5a11  dingr....r....Z.
 00005f90: 6578 7472 6163 7465 645f 7265 7375 6c74  extracted_result
 00005fa0: 7372 1e00 0000 72f2 0000 0072 1f00 0000  sr....r....r....
-00005fb0: 7252 0000 00ee 0200 0073 3600 0000 000e  rR.......s6.....
+00005fb0: 7252 0000 00ed 0200 0073 3600 0000 000e  rR.......s6.....
 00005fc0: 0a01 0601 0401 0e01 0a01 0401 02ff 0202  ................
 00005fd0: 0201 0201 0401 0401 04fa 0407 02f9 0609  ................
 00005fe0: 1a01 0201 14ff 0403 0801 0c01 0e01 0801  ................
 00005ff0: 0401 0a02 7a17 4576 616c 7561 746f 7245  ....z.EvaluatorE
 00006000: 502e 6576 616c 5f73 696e 676c 6563 0100  P.eval_singlec..
 00006010: 0000 0000 0000 0000 0000 0100 0000 0100  ................
 00006020: 0000 4300 0000 7306 0000 007c 006a 0053  ..C...s....|.j.S
 00006030: 0072 1800 0000 2901 da09 5f62 7569 6c64  .r....)..._build
 00006040: 696e 6772 5f00 0000 721e 0000 0072 1e00  ingr_...r....r..
-00006050: 0000 721f 0000 0072 e700 0000 1703 0000  ..r....r........
+00006050: 0000 721f 0000 0072 e700 0000 1603 0000  ..r....r........
 00006060: 7302 0000 0000 027a 1445 7661 6c75 6174  s......z.Evaluat
 00006070: 6f72 4550 2e62 7569 6c64 696e 6772 3c00  orEP.buildingr<.
 00006080: 0000 6302 0000 0000 0000 0000 0000 0003  ..c.............
 00006090: 0000 0004 0000 0043 0000 0073 2800 0000  .......C...s(...
 000060a0: 7c00 6a00 4400 5d0e 7d02 7c02 a001 7c01  |.j.D.].}.|...|.
 000060b0: a101 0100 7106 7c00 a002 a100 0100 7c01  ....q.|.......|.
 000060c0: 7c00 5f03 6401 5300 2902 7a98 4368 616e  |._.d.S.).z.Chan
@@ -1556,21 +1556,21 @@
 00006130: 3a20 7468 6520 6275 696c 6469 6e67 2074  : the building t
 00006140: 6f20 7573 650a 2020 2020 2020 2020 3a72  o use.        :r
 00006150: 6574 7572 6e3a 204e 6f6e 650a 2020 2020  eturn: None.    
 00006160: 2020 2020 4e29 0472 3200 0000 da05 7365      N).r2.....se
 00006170: 7475 7072 6000 0000 72fc 0000 0029 0372  tupr`...r....).r
 00006180: 3a00 0000 5a0c 6e65 775f 6275 696c 6469  :...Z.new_buildi
 00006190: 6e67 da02 696f 721e 0000 0072 1e00 0000  ng..ior....r....
-000061a0: 721f 0000 0072 e700 0000 1b03 0000 7308  r....r........s.
+000061a0: 721f 0000 0072 e700 0000 1a03 0000 7308  r....r........s.
 000061b0: 0000 0000 080a 010c 0108 0163 0100 0000  ...........c....
 000061c0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
 000061d0: 4300 0000 7306 0000 007c 006a 0053 0072  C...s....|.j.S.r
 000061e0: 1800 0000 2901 da04 5f65 7077 725f 0000  ....)..._epwr_..
 000061f0: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00006200: 72dc 0000 0028 0300 0073 0200 0000 0002  r....(...s......
+00006200: 72dc 0000 0027 0300 0073 0200 0000 0002  r....'...s......
 00006210: 7a0f 4576 616c 7561 746f 7245 502e 6570  z.EvaluatorEP.ep
 00006220: 7729 0272 2d00 0000 723d 0000 0063 0200  w).r-...r=...c..
 00006230: 0000 0000 0000 0000 0000 0200 0000 0200  ................
 00006240: 0000 4300 0000 7312 0000 007c 00a0 00a1  ..C...s....|....
 00006250: 0001 007c 017c 005f 0164 0153 0029 027a  ...|.|._.d.S.).z
 00006260: ac43 6861 6e67 6573 2074 6865 2065 7077  .Changes the epw
 00006270: 2066 696c 6520 7573 6564 2077 6974 6820   file used with 
@@ -1581,15 +1581,15 @@
 000062c0: 3a70 6172 616d 2076 616c 7565 3a20 7061  :param value: pa
 000062d0: 7468 2074 6f20 7468 6520 6e65 7720 6570  th to the new ep
 000062e0: 7720 6669 6c65 2074 6f20 7573 652e 0a20  w file to use.. 
 000062f0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
 00006300: 4e6f 6e65 0a20 2020 2020 2020 204e 2902  None.        N).
 00006310: 7260 0000 0072 ff00 0000 72c6 0000 0072  r`...r....r....r
 00006320: 1e00 0000 721e 0000 0072 1f00 0000 72dc  ....r....r....r.
-00006330: 0000 002c 0300 0073 0400 0000 0008 0801  ...,...s........
+00006330: 0000 002b 0300 0073 0400 0000 0008 0801  ...+...s........
 00006340: 2904 7267 0000 0072 8f00 0000 da09 6669  ).rg...r......fi
 00006350: 6c65 5f6e 616d 6572 3d00 0000 6304 0000  le_namer=...c...
 00006360: 0000 0000 0000 0000 0007 0000 0009 0000  ................
 00006370: 0043 0000 0073 7000 0000 7c01 6a00 a001  .C...sp...|.j...
 00006380: a100 7c02 1900 6401 7402 7c00 6a03 6a04  ..|...d.t.|.j.j.
 00006390: 8301 8502 1900 7d04 7c00 a005 7c04 a101  ......}.|...|...
 000063a0: 7d05 7406 7c05 7407 8302 725c 7408 7c03  }.t.|.t...r\t.|.
@@ -1614,15 +1614,15 @@
 000064d0: 0000 0072 6400 0000 72f7 0000 0072 2600  ...rd...r....r&.
 000064e0: 0000 7227 0000 00da 046f 7065 6eda 046a  ..r'.....open..j
 000064f0: 736f 6eda 0464 756d 70da 0673 6176 6561  son..dump..savea
 00006500: 7329 0772 3a00 0000 7267 0000 0072 8f00  s).r:...rg...r..
 00006510: 0000 7200 0100 00da 016c 72fb 0000 00da  ..r......lr.....
 00006520: 0266 7072 1e00 0000 721e 0000 0072 1f00  .fpr....r....r..
 00006530: 0000 da11 6765 6e65 7261 7465 5f62 7569  ....generate_bui
-00006540: 6c64 696e 6738 0300 0073 0c00 0000 0008  lding8...s......
+00006540: 6c64 696e 6737 0300 0073 0c00 0000 0008  lding7...s......
 00006550: 1e01 0a01 0a01 1201 1802 7a1d 4576 616c  ..........z.Eval
 00006560: 7561 746f 7245 502e 6765 6e65 7261 7465  uatorEP.generate
 00006570: 5f62 7569 6c64 696e 6763 0200 0000 0000  _buildingc......
 00006580: 0000 0000 0000 0500 0000 0500 0000 4300  ..............C.
 00006590: 0000 734c 0000 007c 00a0 007c 01a1 0101  ..sL...|...|....
 000065a0: 0074 01a0 027c 006a 03a1 017d 0264 0164  .t...|.j...}.d.d
 000065b0: 0284 0074 047c 006a 056a 067c 0183 0244  ...t.|.j.j.|...D
@@ -1634,43 +1634,43 @@
 00006610: 6469 6e67 2066 726f 6d20 6120 726f 7720  ding from a row 
 00006620: 6f66 2064 6174 6163 0100 0000 0000 0000  of datac........
 00006630: 0000 0000 0300 0000 0400 0000 5300 0000  ............S...
 00006640: 7316 0000 0069 007c 005d 0e5c 027d 017d  s....i.|.].\.}.}
 00006650: 027c 017c 0293 0271 0453 0072 1e00 0000  .|.|...q.S.r....
 00006660: 721e 0000 00a9 0372 1b00 0000 7265 0000  r......r....re..
 00006670: 0072 2d00 0000 721e 0000 0072 1e00 0000  .r-...r....r....
-00006680: 721f 0000 0072 8600 0000 4e03 0000 7306  r....r....N...s.
+00006680: 721f 0000 0072 8600 0000 4d03 0000 7306  r....r....M...s.
 00006690: 0000 0006 0206 ff02 007a 3b45 7661 6c75  .........z;Evalu
 000066a0: 6174 6f72 4550 2e5f 6765 6e65 7261 7465  atorEP._generate
 000066b0: 5f62 7569 6c64 696e 675f 6672 6f6d 5f72  _building_from_r
 000066c0: 6f77 2e3c 6c6f 6361 6c73 3e2e 3c64 6963  ow.<locals>.<dic
 000066d0: 7463 6f6d 703e 2909 7256 0000 00da 0463  tcomp>).rV.....c
 000066e0: 6f70 79da 0864 6565 7063 6f70 7972 e700  opy..deepcopyr..
 000066f0: 0000 724a 0000 0072 3200 0000 7264 0000  ..rJ...r2...rd..
 00006700: 00da 0a70 6172 616d 6574 6572 73da 1774  ...parameters..t
 00006710: 7261 6e73 666f 726d 6174 696f 6e5f 6675  ransformation_fu
 00006720: 6e63 7469 6f6e 2905 723a 0000 0072 8000  nction).r:...r..
 00006730: 0000 72fb 0000 0072 4e00 0000 da09 7061  ..r....rN.....pa
 00006740: 7261 6d65 7465 7272 1e00 0000 721e 0000  rameterr....r...
-00006750: 0072 1f00 0000 72f7 0000 004a 0300 0073  .r....r....J...s
+00006750: 0072 1f00 0000 72f7 0000 0049 0300 0073  .r....r....I...s
 00006760: 1000 0000 0002 0a01 0c01 0602 0cfe 0607  ................
 00006770: 0c01 0e01 7a27 4576 616c 7561 746f 7245  ....z'EvaluatorE
 00006780: 502e 5f67 656e 6572 6174 655f 6275 696c  P._generate_buil
 00006790: 6469 6e67 5f66 726f 6d5f 726f 7729 0346  ding_from_row).F
 000067a0: 7266 0000 0046 2902 4e46 291a 72ac 0000  rf...F).NF).r...
 000067b0: 0072 ad00 0000 72ae 0000 0072 af00 0000  .r....r....r....
 000067c0: 7211 0000 0072 e800 0000 72de 0000 0072  r....r....r....r
 000067d0: df00 0000 7216 0000 0072 1700 0000 72b0  ....r....r....r.
 000067e0: 0000 0072 0600 0000 720a 0000 0072 b100  ...r....r....r..
 000067f0: 0000 723b 0000 0072 b200 0000 72a4 0000  ..r;...r....r...
 00006800: 0072 9500 0000 7252 0000 0072 d900 0000  .r....rR...r....
 00006810: 72e7 0000 0072 da00 0000 72dc 0000 0072  r....r....r....r
 00006820: 0901 0000 72f7 0000 0072 bb00 0000 721e  ....r....r....r.
 00006830: 0000 0072 1e00 0000 72b9 0000 0072 1f00  ...r....r....r..
-00006840: 0000 72db 0000 006a 0200 0073 6200 0000  ..r....j...sb...
+00006840: 0000 72db 0000 0069 0200 0073 6200 0000  ..r....i...sb...
 00006850: 0801 0407 0801 0401 0401 0201 0201 0201  ................
 00006860: 0201 02f5 020d 02f3 0402 0202 0201 0201  ................
 00006870: 0201 0201 0602 0201 0202 02f3 1053 0001  .............S..
 00006880: 0001 00fb 0207 0401 02f8 0402 0202 0201  ................
 00006890: 0205 02f6 1033 0001 00fc 0202 02fe 0c29  .....3.........)
 000068a0: 0201 0a03 0401 100c 0201 1003 0401 120b  ................
 000068b0: 1412 72db 0000 0063 0000 0000 0000 0000  ..r....c........
@@ -1751,28 +1751,28 @@
 00006d60: 0000 da03 6875 6272 3200 0000 7211 0000  ....hubr2...r...
 00006d70: 00da 0f73 6f6c 7665 725f 7365 7474 696e  ...solver_settin
 00006d80: 6773 da0f 636f 6e66 6967 5f73 6574 7469  gs..config_setti
 00006d90: 6e67 7329 0872 3a00 0000 7232 0000 0072  ngs).r:...r2...r
 00006da0: 1101 0000 72de 0000 0072 df00 0000 7233  ....r....r....r3
 00006db0: 0000 0072 3400 0000 7235 0000 0072 b900  ...r4...r5...r..
 00006dc0: 0000 721e 0000 0072 1f00 0000 723b 0000  ..r....r....r;..
-00006dd0: 005d 0300 0073 1600 0000 0018 0601 0201  .]...s..........
+00006dd0: 005c 0300 0073 1600 0000 0018 0601 0201  .\...s..........
 00006de0: 0201 0201 02fc 0606 0601 0601 0601 0601  ................
 00006df0: 7a14 4576 616c 7561 746f 7245 482e 5f5f  z.EvaluatorEH.__
 00006e00: 696e 6974 5f5f 724d 0000 0063 0200 0000  init__rM...c....
 00006e10: 0000 0000 0000 0000 0200 0000 0600 0000  ................
 00006e20: 4300 0000 7332 0000 0074 007c 0183 017c  C...s2...t.|...|
 00006e30: 006a 016a 026b 0372 2e74 0364 0174 007c  .j.j.k.r.t.d.t.|
 00006e40: 0183 019b 0064 027c 006a 016a 029b 0064  .....d.|.j.j...d
 00006e50: 039d 0583 0182 0164 0053 0029 044e 7261  .......d.S.).Nra
 00006e60: 0000 0072 6200 0000 7263 0000 0029 0472  ...rb...rc...).r
 00006e70: 4800 0000 7232 0000 0072 5800 0000 7245  H...r2...rX...rE
 00006e80: 0000 0029 0272 3a00 0000 724e 0000 0072  ...).r:...rN...r
 00006e90: 1e00 0000 721e 0000 0072 1f00 0000 7256  ....r....r....rV
-00006ea0: 0000 0082 0300 0073 0800 0000 0001 1001  .......s........
+00006ea0: 0000 0081 0300 0073 0800 0000 0001 1001  .......s........
 00006eb0: 0201 18ff 7a14 4576 616c 7561 746f 7245  ....z.EvaluatorE
 00006ec0: 482e 7661 6c69 6461 7465 6302 0000 0000  H.validatec.....
 00006ed0: 0000 0000 0000 0009 0000 0007 0000 0003  ................
 00006ee0: 0000 0073 f000 0000 7400 a001 7c00 6a02  ...s....t...|.j.
 00006ef0: a101 7d02 7c00 a003 7c01 a101 0100 6401  ..}.|...|.....d.
 00006f00: 6402 8400 7404 7c00 6a05 6a06 7c01 8302  d...t.|.j.j.|...
 00006f10: 4400 8301 7d03 7c00 6a05 6a07 4400 5d10  D...}.|.j.j.D.].
@@ -1789,15 +1789,15 @@
 00006fc0: 6a05 a014 7c01 8800 a102 0100 7c00 a015  j...|.......|...
 00006fd0: a100 0100 7c08 5300 290d 4e63 0100 0000  ....|.S.).Nc....
 00006fe0: 0000 0000 0000 0000 0300 0000 0400 0000  ................
 00006ff0: 5300 0000 7316 0000 0069 007c 005d 0e5c  S...s....i.|.].\
 00007000: 027d 017d 027c 017c 0293 0271 0453 0072  .}.}.|.|...q.S.r
 00007010: 1e00 0000 721e 0000 0072 0a01 0000 721e  ....r....r....r.
 00007020: 0000 0072 1e00 0000 721f 0000 0072 8600  ...r....r....r..
-00007030: 0000 8e03 0000 7306 0000 0006 0206 ff02  ......s.........
+00007030: 0000 8d03 0000 7306 0000 0006 0206 ff02  ......s.........
 00007040: 007a 2b45 7661 6c75 6174 6f72 4548 2e65  .z+EvaluatorEH.e
 00007050: 7661 6c5f 7369 6e67 6c65 2e3c 6c6f 6361  val_single.<loca
 00007060: 6c73 3e2e 3c64 6963 7463 6f6d 703e 7287  ls>.<dictcomp>r.
 00007070: 0000 0072 0100 0000 da0b 6f75 7470 7574  ...r......output
 00007080: 5f66 696c 65da 0873 6f6c 7574 696f 6eda  _file..solution.
 00007090: 056f 7468 6572 da10 6361 7061 6369 7479  .other..capacity
 000070a0: 5f73 746f 7261 6765 da0d 6361 7061 6369  _storage..capaci
@@ -1805,15 +1805,15 @@
 000070c0: 7374 6570 73da 0673 6865 6574 7363 0100  steps..sheetsc..
 000070d0: 0000 0000 0000 0000 0000 0200 0000 0500  ................
 000070e0: 0000 3300 0000 7320 0000 007c 005d 187d  ..3...s ...|.].}
 000070f0: 0174 00a0 0188 0064 0019 007c 0167 01a1  .t.....d...|.g..
 00007100: 0256 0001 0071 0264 0153 0029 0272 1501  .V...q.d.S.).r..
 00007110: 0000 4e29 02da 0270 66da 0b67 6574 5f62  ..N)...pf..get_b
 00007120: 795f 7061 7468 72f0 0000 0072 f200 0000  y_pathr....r....
-00007130: 721e 0000 0072 1f00 0000 7220 0000 00a7  r....r....r ....
+00007130: 721e 0000 0072 1f00 0000 7220 0000 00a6  r....r....r ....
 00007140: 0300 0073 0400 0000 0402 02ff 7a2a 4576  ...s........z*Ev
 00007150: 616c 7561 746f 7245 482e 6576 616c 5f73  aluatorEH.eval_s
 00007160: 696e 676c 652e 3c6c 6f63 616c 733e 2e3c  ingle.<locals>.<
 00007170: 6765 6e65 7870 723e 2916 720b 0100 0072  genexpr>).r....r
 00007180: 0c01 0000 7211 0100 0072 5600 0000 724a  ....r....rV...rJ
 00007190: 0000 0072 3200 0000 7264 0000 0072 0d01  ...r2...rd...r..
 000071a0: 0000 720e 0100 0072 5900 0000 da07 636f  ..r....rY.....co
@@ -1822,29 +1822,29 @@
 000071d0: 7248 0000 0072 6a00 0000 722a 0000 0072  rH...rj...r*...r
 000071e0: f900 0000 72fa 0000 0072 a200 0000 2909  ....r....r....).
 000071f0: 723a 0000 0072 4e00 0000 5a0b 6375 7272  r:...rN...Z.curr
 00007200: 656e 745f 6875 625a 0b76 616c 7565 5f70  ent_hubZ.value_p
 00007210: 6169 7273 720f 0100 0072 a800 0000 5a11  airsr....r....Z.
 00007220: 7072 696d 6172 795f 6f62 6a65 6374 6976  primary_objectiv
 00007230: 6572 1401 0000 7287 0000 0072 1e00 0000  er....r....r....
-00007240: 72f2 0000 0072 1f00 0000 7252 0000 0089  r....r....rR....
+00007240: 72f2 0000 0072 1f00 0000 7252 0000 0088  r....r....rR....
 00007250: 0300 0073 3c00 0000 0001 0c03 0a01 0602  ...s<...........
 00007260: 0cfe 0604 0c01 0e02 0c01 0801 0801 0602  ................
 00007270: 0802 0a01 0a01 0c01 0201 0601 0401 0801  ................
 00007280: 08fc 0607 0201 0a02 02fe 04ff 0406 0c01  ................
 00007290: 0e01 0802 7a17 4576 616c 7561 746f 7245  ....z.EvaluatorE
 000072a0: 482e 6576 616c 5f73 696e 676c 6529 1272  H.eval_single).r
 000072b0: ac00 0000 72ad 0000 0072 ae00 0000 72af  ....r....r....r.
 000072c0: 0000 0072 1100 0000 72de 0000 0072 df00  ...r....r....r..
 000072d0: 0000 7216 0000 0072 1700 0000 72b0 0000  ..r....r....r...
 000072e0: 0072 0600 0000 720a 0000 0072 b100 0000  .r....r....r....
 000072f0: 723b 0000 0072 5600 0000 722a 0000 0072  r;...rV...r*...r
 00007300: 5200 0000 72bb 0000 0072 1e00 0000 721e  R...r....r....r.
 00007310: 0000 0072 b900 0000 721f 0000 0072 1001  ...r....r....r..
-00007320: 0000 5a03 0000 7320 0000 0008 0104 0604  ..Z...s ........
+00007320: 0000 5903 0000 7320 0000 0008 0104 0604  ..Y...s ........
 00007330: 0104 0102 0102 0102 f802 0202 0202 0102  ................
 00007340: 0102 0106 0102 f810 2510 0772 1001 0000  ........%..r....
 00007350: 2937 72af 0000 0072 0b01 0000 7204 0100  )7r....r....r...
 00007360: 0072 e200 0000 726a 0000 0072 a600 0000  .r....rj...r....
 00007370: da03 6162 6372 0200 0000 7203 0000 00da  ..abcr....r.....
 00007380: 0770 6174 686c 6962 7204 0000 00da 0674  .pathlibr......t
 00007390: 7970 696e 6772 0500 0000 7206 0000 0072  ypingr....r....r
@@ -1868,8 +1868,8 @@
 000074b0: 0000 7210 0100 0072 1e00 0000 721e 0000  ..r....r....r...
 000074c0: 0072 1e00 0000 721f 0000 00da 083c 6d6f  .r....r......<mo
 000074d0: 6475 6c65 3e01 0000 0073 5000 0000 040c  dule>....sP.....
 000074e0: 0801 0801 0801 0801 0801 1001 0c01 2001  .............. .
 000074f0: 0c03 0801 0801 0801 0801 0c01 0c01 0c01  ................
 00007500: 0c01 0c03 0c01 0c01 0c01 0c01 0c01 0c01  ................
 00007510: 0c03 081b 107f 007f 0059 1027 0201 0201  .........Y.'....
-00007520: 02fe 0404 120a 127f 0018 127f 0071       .............q
+00007520: 02fe 0404 120a 127f 0017 127f 0071       .............q
```

### Comparing `besos-2.2.2/besos/__pycache__/objectives.cpython-38.pyc` & `besos-2.2.3/besos/__pycache__/objectives.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sun Oct 29 18:07:36 2023 UTC, .py size: 19196 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 689f 3e65 fc4a 0000  U.......h.>e.J..
+00000000: 550d 0d0a 0000 0000 31c8 1166 ab4b 0000  U.......1..f.K..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 c201 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6401 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c09 6d0a 5a0a 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6407 6c0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  d.l.m.Z.m.Z.m.Z.
@@ -229,27 +229,27 @@
 00000e40: 292c 2059 4d44 3d28 3f50 3c64 6174 653e  ), YMD=(?P<date>
 00000e50: 5c64 5c64 5c64 5c64 5c2e 5c64 5c64 5c2e  \d\d\d\d\.\d\d\.
 00000e60: 5c64 5c64 2b29 2028 3f50 3c74 696d 653e  \d\d+) (?P<time>
 00000e70: 5c64 3f5c 643a 5c64 5c64 2924 da01 724e  \d?\d:\d\d)$..rN
 00000e80: 7a14 4669 7273 7420 6c69 6e65 206f 6620  z.First line of 
 00000e90: 6669 6c65 3a27 7a24 2720 6469 6420 6e6f  file:'z$' did no
 00000ea0: 7420 6d61 7463 6820 7468 6520 6578 7065  t match the expe
-00000eb0: 6374 6564 2066 6f72 6d61 742e 5a0e 7665  cted format.Z.ve
+00000eb0: 6374 6564 2066 6f72 6d61 742e da0e 7665  cted format...ve
 00000ec0: 7273 696f 6e5f 6e75 6d62 6572 2908 7218  rsion_number).r.
 00000ed0: 0000 0072 1900 0000 da04 6f70 656e da08  ...r......open..
 00000ee0: 7265 6164 6c69 6e65 da05 6d61 7463 68da  readline..match.
 00000ef0: 0a56 616c 7565 4572 726f 7272 0d00 0000  .ValueErrorr....
 00000f00: da05 6772 6f75 7029 0572 4700 0000 5a10  ..group).rG...Z.
 00000f10: 6669 7273 745f 6c69 6e65 5f72 6567 6578  first_line_regex
 00000f20: da01 66da 0a66 6972 7374 5f6c 696e 6572  ..f..first_liner
-00000f30: 4b00 0000 7220 0000 0072 2000 0000 7221  K...r ...r ...r!
+00000f30: 4c00 0000 7220 0000 0072 2000 0000 7221  L...r ...r ...r!
 00000f40: 0000 00da 0f67 6574 5f65 736f 5f76 6572  .....get_eso_ver
 00000f50: 7369 6f6e 6500 0000 7316 0000 0000 0704  sione...s.......
 00000f60: 0102 ff04 050c 0112 010a 0108 0102 010a  ................
-00000f70: ff04 0372 5000 0000 7a0c 6570 6c75 736f  ...rP...z.epluso
+00000f70: ff04 0372 5100 0000 7a0c 6570 6c75 736f  ...rQ...z.epluso
 00000f80: 7574 2e65 736f 2902 da07 6f75 745f 6469  ut.eso)...out_di
 00000f90: 7272 2600 0000 6303 0000 0000 0000 0000  rr&...c.........
 00000fa0: 0000 001a 0000 0009 0000 0043 0000 0073  ...........C...s
 00000fb0: e801 0000 7400 7c00 7c01 8302 7d03 7401  ....t.|.|...}.t.
 00000fc0: 7c03 8301 7d04 7402 7c03 6401 8302 8f0e  |...}.t.|.d.....
 00000fd0: 7d05 7c05 a003 a100 7d06 5700 3500 5100  }.|.....}.W.5.Q.
 00000fe0: 5200 5800 7c02 725e 7404 6402 7405 8302  R.X.|.r^t.d.t...
@@ -343,47 +343,47 @@
 00001560: 007c 018e 0193 0271 0453 0029 0272 1c00  .|.....q.S.).r..
 00001570: 0000 721e 0000 0029 0272 2300 0000 723f  ..r....).r#...r?
 00001580: 0000 0029 0272 2900 0000 da06 7265 7375  ...).r).....resu
 00001590: 6c74 7220 0000 0072 2000 0000 7221 0000  ltr ...r ...r!..
 000015a0: 0072 2f00 0000 cf00 0000 7306 0000 0006  .r/.......s.....
 000015b0: 0202 ff0e 007a 1c72 6561 645f 6573 6f2e  .....z.read_eso.
 000015c0: 3c6c 6f63 616c 733e 2e3c 6469 6374 636f  <locals>.<dictco
-000015d0: 6d70 3e29 1372 0600 0000 7250 0000 0072  mp>).r....rP...r
-000015e0: 4900 0000 da09 7265 6164 6c69 6e65 7372  I.....readlinesr
+000015d0: 6d70 3e29 1372 0600 0000 7251 0000 0072  mp>).r....rQ...r
+000015e0: 4a00 0000 da09 7265 6164 6c69 6e65 7372  J.....readlinesr
 000015f0: 0c00 0000 da0d 4675 7475 7265 5761 726e  ......FutureWarn
-00001600: 696e 6772 0d00 0000 724c 0000 0072 3c00  ingr....rL...r<.
+00001600: 696e 6772 0d00 0000 724d 0000 0072 3c00  ingr....rM...r<.
 00001610: 0000 7222 0000 00da 0373 6574 da06 7365  ..r".....set..se
-00001620: 6172 6368 724d 0000 00da 0573 706c 6974  archrM.....split
+00001620: 6172 6368 724e 0000 00da 0573 706c 6974  archrN.....split
 00001630: da0e 4173 7365 7274 696f 6e45 7272 6f72  ..AssertionError
 00001640: da04 6469 6374 da03 6164 64da 0661 7070  ..dict..add..app
-00001650: 656e 6472 2e00 0000 291a 7251 0000 00da  endr....).rQ....
+00001650: 656e 6472 2e00 0000 291a 7252 0000 00da  endr....).rR....
 00001660: 0966 696c 655f 6e61 6d65 da07 7665 7273  .file_name..vers
 00001670: 696f 6e5a 0865 736f 5f70 6174 685a 0b65  ionZ.eso_pathZ.e
 00001680: 736f 5f76 6572 7369 6f6e da04 6669 6c65  so_version..file
-00001690: 724e 0000 005a 1664 6174 615f 6469 6374  rN...Z.data_dict
+00001690: 724f 0000 005a 1664 6174 615f 6469 6374  rO...Z.data_dict
 000016a0: 696f 6e61 7279 5f68 6561 6465 725a 1564  ionary_headerZ.d
 000016b0: 6174 615f 6469 6374 696f 6e61 7279 5f73  ata_dictionary_s
 000016c0: 7461 7274 5a13 6461 7461 5f64 6963 7469  tartZ.data_dicti
 000016d0: 6f6e 6172 795f 656e 645a 0864 6174 615f  onary_endZ.data_
 000016e0: 656e 64da 0668 6561 6465 725a 0e72 6571  end..headerZ.req
 000016f0: 7565 7374 6564 5f76 6172 7372 2400 0000  uested_varsr$...
 00001700: 5a0e 6461 7461 5f64 6963 745f 6c69 6e65  Z.data_dict_line
 00001710: da05 636f 6465 73da 046b 6579 73da 046c  ..codes..keys..l
-00001720: 696e 6572 4b00 0000 721c 0000 0072 1e00  inerK...r....r..
+00001720: 696e 6572 4c00 0000 721c 0000 0072 1e00  inerL...r....r..
 00001730: 0000 7232 0000 0072 1a00 0000 da03 6b65  ..r2...r......ke
-00001740: 7972 5800 0000 722e 0000 0072 2000 0000  yrX...r....r ...
+00001740: 7972 5900 0000 722e 0000 0072 2000 0000  yrY...r....r ...
 00001750: 7220 0000 0072 2100 0000 da08 7265 6164  r ...r!.....read
 00001760: 5f65 736f 7b00 0000 736e 0000 0000 0f0a  _eso{...sn......
 00001770: 0108 010c 0112 0304 0102 0102 0302 fc04  ................
 00001780: 060c 0102 010e ff04 0402 040c 0206 0204  ................
 00001790: 0204 010a 0104 020c 0110 0110 0206 0104  ................
 000017a0: 0106 0208 010a 0108 010e 010a 010a 010a  ................
 000017b0: 011a 010a 0108 0118 0118 0202 0102 0102  ................
 000017c0: 0108 0102 0102 fb06 0808 010c 0108 010e  ................
-000017d0: 010a 010e 0116 0206 0206 fe72 6a00 0000  ...........rj...
+000017d0: 010a 010e 0116 0206 0206 fe72 6b00 0000  ...........rk...
 000017e0: a901 da07 7265 7375 6c74 7363 0100 0000  ....resultsc....
 000017f0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
 00001800: 4300 0000 7312 0000 0074 0064 0183 0101  C...s....t.d....
 00001810: 007c 006a 0164 0219 0053 0029 037a 8f52  .|.j.d...S.).z.R
 00001820: 6574 7572 6e73 2074 6865 2065 6e74 6972  eturns the entir
 00001830: 6520 7661 6c75 6520 636f 6c75 6d6e 2066  e value column f
 00001840: 726f 6d20 7468 6520 7265 7375 6c74 732e  rom the results.
@@ -394,39 +394,39 @@
 00001890: 2066 726f 6d20 7468 6520 7265 7375 6c74   from the result
 000018a0: 7320 6f62 6a65 6374 2e0a 2020 2020 7a53  s object..    zS
 000018b0: 6074 696d 655f 7365 7269 6573 5f76 616c  `time_series_val
 000018c0: 7565 7360 2069 7320 696e 636f 6d70 6c65  ues` is incomple
 000018d0: 7465 2c20 616e 6420 7265 7475 726e 7320  te, and returns 
 000018e0: 7261 7720 7661 6c75 6573 2c20 6e6f 7420  raw values, not 
 000018f0: 7469 6d65 2073 6572 6965 7320 7661 6c75  time series valu
-00001900: 6573 2e72 5500 0000 2902 720c 0000 0072  es.rU...).r....r
-00001910: 2400 0000 726b 0000 0072 2000 0000 7220  $...rk...r ...r 
+00001900: 6573 2e72 5600 0000 2902 720c 0000 0072  es.rV...).r....r
+00001910: 2400 0000 726c 0000 0072 2000 0000 7220  $...rl...r ...r 
 00001920: 0000 0072 2100 0000 da12 7469 6d65 5f73  ...r!.....time_s
 00001930: 6572 6965 735f 7661 6c75 6573 d500 0000  eries_values....
-00001940: 7308 0000 0000 0b02 0102 ff04 0372 6d00  s............rm.
-00001950: 0000 a902 726c 0000 0072 2600 0000 6301  ....rl...r&...c.
+00001940: 7308 0000 0000 0b02 0102 ff04 0372 6e00  s............rn.
+00001950: 0000 a902 726d 0000 0072 2600 0000 6301  ....rm...r&...c.
 00001960: 0000 0000 0000 0000 0000 0001 0000 0002  ................
 00001970: 0000 0043 0000 0073 0e00 0000 7c00 6a00  ...C...s....|.j.
 00001980: 6401 1900 a001 a100 5300 2902 7aba 5265  d.......S.).z.Re
 00001990: 7475 726e 7320 7468 6520 7375 6d20 6f76  turns the sum ov
 000019a0: 6572 2074 6865 2056 616c 7565 2063 6f6c  er the Value col
 000019b0: 756d 6e20 6672 6f6d 2073 6f6d 6520 7265  umn from some re
 000019c0: 7375 6c74 730a 0a20 2020 203a 7061 7261  sults..    :para
 000019d0: 6d20 7265 7375 6c74 733a 2074 6865 2072  m results: the r
 000019e0: 6573 756c 7473 206f 626a 6563 7420 746f  esults object to
 000019f0: 2073 756d 206f 7665 720a 2020 2020 3a72   sum over.    :r
 00001a00: 6574 7572 6e3a 2074 6865 2073 756d 206f  eturn: the sum o
 00001a10: 6620 7468 6520 6669 7273 7420 7661 6c75  f the first valu
 00001a20: 6520 666f 7220 6561 6368 2065 6e74 7279  e for each entry
 00001a30: 2069 6e20 7468 6520 636f 6c6c 6563 7469   in the collecti
-00001a40: 6f6e 2e0a 2020 2020 7255 0000 0029 0272  on..    rU...).r
-00001a50: 2400 0000 da03 7375 6d72 6b00 0000 7220  $.....sumrk...r 
+00001a40: 6f6e 2e0a 2020 2020 7256 0000 0029 0272  on..    rV...).r
+00001a50: 2400 0000 da03 7375 6d72 6c00 0000 7220  $.....sumrl...r 
 00001a60: 0000 0072 2000 0000 7221 0000 00da 0a73  ...r ...r!.....s
 00001a70: 756d 5f76 616c 7565 73e6 0000 0073 0200  um_values....s..
-00001a80: 0000 0006 7270 0000 00da 0361 6c6c 2902  ....rp.....all).
+00001a80: 0000 0006 7271 0000 00da 0361 6c6c 2902  ....rq.....all).
 00001a90: da07 6f75 7470 7574 7372 2600 0000 6302  ..outputsr&...c.
 00001aa0: 0000 0000 0000 0000 0000 0005 0000 0005  ................
 00001ab0: 0000 0003 0000 0073 fc00 0000 7400 a001  .......s....t...
 00001ac0: 7c00 a101 8902 8802 6401 6b02 721e 7c00  |.......d.k.r.|.
 00001ad0: 6a02 8900 7403 7d02 6e1a 8802 6402 6b02  j...t.}.n...d.k.
 00001ae0: 7230 7c00 8900 7404 7d02 6e08 7405 8802  r0|...t.}.n.t...
 00001af0: 8301 8201 8700 8702 6602 6403 6404 8408  ........f.d.d...
@@ -475,15 +475,15 @@
 00001da0: 0000 0072 2000 0000 7221 0000 00da 093c  ...r ...r!.....<
 00001db0: 7365 7463 6f6d 703e 0701 0000 7306 0000  setcomp>....s...
 00001dc0: 0006 0202 0114 fe7a 2e63 6c65 6172 5f6f  .......z.clear_o
 00001dd0: 7574 7075 7473 2e3c 6c6f 6361 6c73 3e2e  utputs.<locals>.
 00001de0: 6669 6e64 2e3c 6c6f 6361 6c73 3e2e 3c73  find.<locals>.<s
 00001df0: 6574 636f 6d70 3e72 2000 0000 722b 0000  etcomp>r ...r+..
 00001e00: 0029 02da 0e62 7569 6c64 696e 675f 6974  .)...building_it
-00001e10: 656d 7372 7a00 0000 722b 0000 0072 2100  emsrz...r+...r!.
+00001e10: 656d 7372 7b00 0000 722b 0000 0072 2100  emsr{...r+...r!.
 00001e20: 0000 da04 6669 6e64 0601 0000 7306 0000  ....find....s...
 00001e30: 0000 010c 0202 fe7a 1b63 6c65 6172 5f6f  .......z.clear_o
 00001e40: 7574 7075 7473 2e3c 6c6f 6361 6c73 3e2e  utputs.<locals>.
 00001e50: 6669 6e64 7a0d 4f75 7470 7574 3a4d 6574  findz.Output:Met
 00001e60: 6572 3a7a 0c4f 7574 7075 743a 4d65 7465  er:z.Output:Mete
 00001e70: 727a 214f 7574 7075 743a 456e 7669 726f  rz!Output:Enviro
 00001e80: 6e6d 656e 7461 6c49 6d70 6163 7446 6163  nmentalImpactFac
@@ -492,39 +492,39 @@
 00001eb0: 6d7a 154d 6574 6572 3a43 7573 746f 6d44  mz.Meter:CustomD
 00001ec0: 6563 7265 6d65 6e74 5a0f 696e 7465 726e  ecrementZ.intern
 00001ed0: 616c 5f6d 6574 6572 737a 0d4f 7574 7075  al_metersz.Outpu
 00001ee0: 743a 5461 626c 653a da06 7461 626c 6573  t:Table:..tables
 00001ef0: 7a07 4f75 7470 7574 3ada 066f 7574 7075  z.Output:..outpu
 00001f00: 747a 0e4f 7574 7075 7443 6f6e 7472 6f6c  tz.OutputControl
 00001f10: 3a5a 0d6f 7574 7075 7463 6f6e 7472 6f6c  :Z.outputcontrol
-00001f20: 5a06 6d65 7465 7273 7271 0000 0063 0100  Z.metersrq...c..
+00001f20: 5a06 6d65 7465 7273 7272 0000 0063 0100  Z.metersrr...c..
 00001f30: 0000 0000 0000 0000 0000 0200 0000 0500  ................
 00001f40: 0000 3300 0000 731c 0000 007c 005d 147d  ..3...s....|.].}
 00001f50: 0188 00a0 007c 017c 0167 01a1 0256 0001  .....|.|.g...V..
 00001f60: 0071 0264 0053 00a9 014e 2901 7231 0000  .q.d.S...N).r1..
-00001f70: 0029 0272 2900 0000 727f 0000 0029 01da  .).r)...r....)..
+00001f70: 0029 0272 2900 0000 7280 0000 0029 01da  .).r)...r....)..
 00001f80: 0b63 6c61 7373 5f6e 616d 6573 7220 0000  .class_namesr ..
 00001f90: 0072 2100 0000 da09 3c67 656e 6578 7072  .r!.....<genexpr
 00001fa0: 3e24 0100 0073 0400 0000 0400 0200 7a20  >$...s........z 
 00001fb0: 636c 6561 725f 6f75 7470 7574 732e 3c6c  clear_outputs.<l
 00001fc0: 6f63 616c 733e 2e3c 6765 6e65 7870 723e  ocals>.<genexpr>
-00001fd0: 4e29 0b72 7700 0000 da08 6765 745f 6d6f  N).rw.....get_mo
+00001fd0: 4e29 0b72 7800 0000 da08 6765 745f 6d6f  N).rx.....get_mo
 00001fe0: 6465 da0a 6964 666f 626a 6563 7473 da04  de..idfobjects..
-00001ff0: 6c69 7374 725f 0000 0072 1100 0000 7205  listr_...r....r.
+00001ff0: 6c69 7374 7260 0000 0072 1100 0000 7205  listr`...r....r.
 00002000: 0000 0072 2e00 0000 da0a 6973 696e 7374  ...r......isinst
-00002010: 616e 6365 7244 0000 0072 5b00 0000 2905  ancerD...r[...).
-00002020: da08 6275 696c 6469 6e67 7272 0000 00da  ..buildingrr....
-00002030: 0565 6d70 7479 727d 0000 0072 7f00 0000  .emptyr}...r....
-00002040: 7220 0000 0029 0372 7c00 0000 7281 0000  r ...).r|...r...
-00002050: 0072 7a00 0000 7221 0000 00da 0d63 6c65  .rz...r!.....cle
+00002010: 616e 6365 7244 0000 0072 5c00 0000 2905  ancerD...r\...).
+00002020: da08 6275 696c 6469 6e67 7273 0000 00da  ..buildingrs....
+00002030: 0565 6d70 7479 727e 0000 0072 8000 0000  .emptyr~...r....
+00002040: 7220 0000 0029 0372 7d00 0000 7282 0000  r ...).r}...r...
+00002050: 0072 7b00 0000 7221 0000 00da 0d63 6c65  .r{...r!.....cle
 00002060: 6172 5f6f 7574 7075 7473 f000 0000 7336  ar_outputs....s6
 00002070: 0000 0000 0b0a 0208 0106 0106 0108 0104  ................
 00002080: 0106 0208 020e 0806 0206 0102 0102 fe0a  ................
 00002090: 040c 010c 020c 010c 030e ff06 0408 010e  ................
-000020a0: 020a 0106 021a 0208 0172 8900 0000 6300  .........r....c.
+000020a0: 020a 0106 021a 0208 0172 8a00 0000 6300  .........r....c.
 000020b0: 0000 0000 0000 0000 0000 0000 0000 0005  ................
 000020c0: 0000 0000 0000 0073 8200 0000 6500 5a01  .......s....e.Z.
 000020d0: 6400 5a02 5500 6503 5a04 6505 6506 6401  d.Z.U.e.Z.e.e.d.
 000020e0: 3c00 6402 6507 6403 6603 6508 6404 9c01  <.d.e.d.f.e.d...
 000020f0: 8700 6601 6405 6406 840d 5a09 6407 6408  ..f.d.d...Z.d.d.
 00002100: 8400 5a0a 6409 640a 8400 5a0b 640b 640c  ..Z.d.d...Z.d.d.
 00002110: 8400 5a0c 640d 640e 8400 5a0d 6402 640f  ..Z.d.d...Z.d.d.
@@ -539,51 +539,51 @@
 000021a0: 005f 027c 027c 005f 037c 006a 0464 0264  ._.|.|._.|.j.d.d
 000021b0: 0367 0264 0464 058d 0201 007c 037c 005f  .g.d.d.....|.|._
 000021c0: 057c 00a0 0664 0664 07a1 0201 0064 0053  .|...d.d.....d.S
 000021d0: 0029 084e 2901 721c 0000 00da 0a63 6c61  .).N).r......cla
 000021e0: 7373 5f6e 616d 6572 1e00 0000 54a9 01da  ss_namer....T...
 000021f0: 0563 6865 636b da04 6675 6e63 da08 5f70  .check..func.._p
 00002200: 726f 6365 7373 2907 da05 7375 7065 72da  rocess)...super.
-00002210: 085f 5f69 6e69 745f 5f72 8d00 0000 721e  .__init__r....r.
-00002220: 0000 00da 0a5f 6164 645f 7265 7072 7372  ....._add_reprsr
-00002230: 9100 0000 da09 5f61 6464 5f72 6570 7229  ......_add_repr)
-00002240: 05da 0473 656c 6672 8d00 0000 721e 0000  ...selfr....r...
-00002250: 0072 9000 0000 721c 0000 00a9 01da 095f  .r....r........_
+00002210: 085f 5f69 6e69 745f 5f72 8e00 0000 721e  .__init__r....r.
+00002220: 0000 005a 0a5f 6164 645f 7265 7072 7372  ...Z._add_reprsr
+00002230: 9200 0000 da09 5f61 6464 5f72 6570 7229  ......_add_repr)
+00002240: 05da 0473 656c 6672 8e00 0000 721e 0000  ...selfr....r...
+00002250: 0072 9100 0000 721c 0000 00a9 01da 095f  .r....r........_
 00002260: 5f63 6c61 7373 5f5f 7220 0000 0072 2100  _class__r ...r!.
-00002270: 0000 7293 0000 002d 0100 0073 0c00 0000  ..r....-...s....
+00002270: 0000 7294 0000 002d 0100 0073 0c00 0000  ..r....-...s....
 00002280: 0001 0e01 0601 0603 1202 0601 7a11 4550  ............z.EP
 00002290: 5265 6164 6572 2e5f 5f69 6e69 745f 5f63  Reader.__init__c
 000022a0: 0300 0000 0000 0000 0000 0000 0800 0000  ................
 000022b0: 0700 0000 0300 0000 737a 0000 007c 0264  ........sz...|.d
 000022c0: 016b 0272 1687 0066 0164 0264 0384 087d  .k.r...f.d.d...}
 000022d0: 036e 1e7c 0264 046b 0272 2c87 0066 0164  .n.|.d.k.r,..f.d
 000022e0: 0564 0384 087d 036e 0874 007c 0283 0182  .d...}.n.t.|....
 000022f0: 017c 006a 0144 005d 3a5c 027d 047d 0574  .|.j.D.]:\.}.}.t
 00002300: 027c 007c 0483 027d 067c 0374 03a0 047c  .|.|...}.|.t...|
 00002310: 0564 067c 02a1 0383 017d 077c 0664 006b  .d.|.....}.|.d.k
 00002320: 0972 3a7c 077c 066b 0372 3a01 0064 0753  .r:|.|.k.r:..d.S
-00002330: 0071 3a64 0853 0029 094e 7273 0000 0063  .q:d.S.).Nrs...c
+00002330: 0071 3a64 0853 0029 094e 7274 0000 0063  .q:d.S.).Nrt...c
 00002340: 0100 0000 0000 0000 0000 0000 0100 0000  ................
 00002350: 0300 0000 1300 0000 730a 0000 0074 0088  ........s....t..
-00002360: 007c 0083 0253 0072 8000 0000 2901 da07  .|...S.r....)...
+00002360: 007c 0083 0253 0072 8100 0000 2901 da07  .|...S.r....)...
 00002370: 6765 7461 7474 72a9 01da 0961 7474 7269  getattr....attri
 00002380: 6275 7465 a901 da09 6f62 6a65 6374 6976  bute....objectiv
 00002390: 6572 2000 0000 7221 0000 0072 3100 0000  er ...r!...r1...
 000023a0: 3b01 0000 7302 0000 0000 017a 1f45 5052  ;...s......z.EPR
 000023b0: 6561 6465 722e 6368 6563 6b5f 616c 6c2e  eader.check_all.
-000023c0: 3c6c 6f63 616c 733e 2e67 6574 7274 0000  <locals>.getrt..
+000023c0: 3c6c 6f63 616c 733e 2e67 6574 7275 0000  <locals>.getru..
 000023d0: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
 000023e0: 0000 0200 0000 1300 0000 7308 0000 0088  ..........s.....
-000023f0: 007c 0019 0053 0072 8000 0000 7220 0000  .|...S.r....r ..
+000023f0: 007c 0019 0053 0072 8100 0000 7220 0000  .|...S.r....r ..
 00002400: 0072 9a00 0000 729c 0000 0072 2000 0000  .r....r....r ...
 00002410: 7221 0000 0072 3100 0000 4001 0000 7302  r!...r1...@...s.
 00002420: 0000 0000 01da 0566 6965 6c64 4654 2905  .......fieldFT).
-00002430: 7211 0000 0072 8b00 0000 7299 0000 0072  r....r....r....r
-00002440: 7700 0000 7278 0000 0029 0872 9600 0000  w...rx...).r....
-00002450: 729d 0000 0072 7a00 0000 7231 0000 005a  r....rz...r1...Z
+00002430: 7211 0000 0072 8c00 0000 7299 0000 0072  r....r....r....r
+00002440: 7800 0000 7279 0000 0029 0872 9600 0000  x...ry...).r....
+00002450: 729d 0000 0072 7b00 0000 7231 0000 005a  r....r{...r1...Z
 00002460: 0973 656c 665f 6174 7472 5a0e 6f62 6a65  .self_attrZ.obje
 00002470: 6374 6976 655f 6174 7472 5a0a 7365 6c66  ctive_attrZ.self
 00002480: 5f76 616c 7565 5a0f 6f62 6a65 6374 6976  _valueZ.objectiv
 00002490: 655f 7661 6c75 6572 2000 0000 729c 0000  e_valuer ...r...
 000024a0: 0072 2100 0000 da09 6368 6563 6b5f 616c  .r!.....check_al
 000024b0: 6c38 0100 0073 1600 0000 0001 0802 0e03  l8...s..........
 000024c0: 0802 0e04 0801 0e01 0a01 1201 1001 0801  ................
@@ -613,22 +613,22 @@
 00002640: 6469 6e67 2773 2064 6174 6120 636f 7272  ding's data corr
 00002650: 6573 706f 6e64 696e 6720 746f 2074 6869  esponding to thi
 00002660: 7320 4f62 6a65 6374 6976 652e 0a20 2020  s Objective..   
 00002670: 2020 2020 2020 2020 2054 6865 2072 6574           The ret
 00002680: 7572 6e20 7479 7065 2076 6172 6965 7320  urn type varies 
 00002690: 6265 7477 6565 6e20 6a73 6f6e 2061 6e64  between json and
 000026a0: 2069 6466 2062 7569 6c64 696e 6773 0a20   idf buildings. 
-000026b0: 2020 2020 2020 2072 7300 0000 7275 0000         rs...ru..
-000026c0: 0072 7400 0000 7a1e 4361 6e6e 6f74 2066  .rt...z.Cannot f
+000026b0: 2020 2020 2020 2072 7400 0000 7276 0000         rt...rv..
+000026c0: 0072 7500 0000 7a1e 4361 6e6e 6f74 2066  .ru...z.Cannot f
 000026d0: 696e 6420 7468 6520 6f62 6a65 6374 6976  ind the objectiv
-000026e0: 6520 666f 7220 4e29 0a72 7700 0000 7283  e for N).rw...r.
-000026f0: 0000 0072 8400 0000 7278 0000 0072 8d00  ...r....rx...r..
+000026e0: 6520 666f 7220 4e29 0a72 7800 0000 7284  e for N).rx...r.
+000026f0: 0000 0072 8500 0000 7279 0000 0072 8e00  ...r....ry...r..
 00002700: 0000 722e 0000 0072 1100 0000 729f 0000  ..r....r....r...
-00002710: 0072 4c00 0000 da04 7265 7072 2905 7296  .rL.....repr).r.
-00002720: 0000 0072 8700 0000 727a 0000 00da 0a6f  ...r....rz.....o
+00002710: 0072 4d00 0000 da04 7265 7072 2905 7296  .rM.....repr).r.
+00002720: 0000 0072 8800 0000 727b 0000 00da 0a6f  ...r....r{.....o
 00002730: 626a 6563 7469 7665 7372 9d00 0000 7220  bjectivesr....r 
 00002740: 0000 0072 2000 0000 7221 0000 00da 0d67  ...r ...r!.....g
 00002750: 6574 5f6f 626a 6563 7469 7665 4c01 0000  et_objectiveL...
 00002760: 731c 0000 0000 070a 0208 0104 010e ff06  s...............
 00002770: 0308 0102 010e ff0a 0408 0108 010c 010a  ................
 00002780: 017a 1645 5052 6561 6465 722e 6765 745f  .z.EPReader.get_
 00002790: 6f62 6a65 6374 6976 6563 0200 0000 0000  objectivec......
@@ -661,48 +661,48 @@
 00002940: 626a 6563 7469 7665 2066 6f72 207a 0f20  bjective for z. 
 00002950: 616c 7265 6164 7920 6578 6973 7473 6301  already existsc.
 00002960: 0000 0000 0000 0000 0000 0003 0000 0007  ................
 00002970: 0000 0013 0000 0073 3000 0000 6900 7c00  .......s0...i.|.
 00002980: 5d28 5c02 7d01 7d02 7400 8801 7c01 8302  ](\.}.}.t...|...
 00002990: 7204 7401 a002 7c02 6400 8800 a103 7400  r.t...|.d.....t.
 000029a0: 8801 7c01 8302 9302 7104 5300 2901 729e  ..|.....q.S.).r.
-000029b0: 0000 0029 0372 9900 0000 7277 0000 0072  ...).r....rw...r
-000029c0: 7800 0000 2903 7229 0000 00da 0461 7474  x...).r).....att
-000029d0: 7272 9e00 0000 a902 727a 0000 0072 9600  rr......rz...r..
+000029b0: 0000 0029 0372 9900 0000 7278 0000 0072  ...).r....rx...r
+000029c0: 7900 0000 2903 7229 0000 00da 0461 7474  y...).r).....att
+000029d0: 7272 9e00 0000 a902 727b 0000 0072 9600  rr......r{...r..
 000029e0: 0000 7220 0000 0072 2100 0000 722f 0000  ..r ...r!...r/..
 000029f0: 0073 0100 0073 0800 0000 0602 0601 0afe  .s...s..........
 00002a00: 0c00 7a2a 4550 5265 6164 6572 2e61 6464  ..z*EPReader.add
 00002a10: 5f6f 626a 6563 7469 7665 2e3c 6c6f 6361  _objective.<loca
 00002a20: 6c73 3e2e 3c64 6963 7463 6f6d 703e 4e5a  ls>.<dictcomp>NZ
 00002a30: 0648 6f75 726c 79da 1352 6570 6f72 7469  .Hourly..Reporti
 00002a40: 6e67 5f46 7265 7175 656e 6379 729e 0000  ng_Frequencyr...
-00002a50: 0072 7300 0000 7269 0000 0072 7500 0000  .rs...ri...ru...
-00002a60: 7274 0000 0072 1600 0000 7a26 5468 6520  rt...r....z&The 
+00002a50: 0072 7400 0000 726a 0000 0072 7600 0000  .rt...rj...rv...
+00002a60: 7275 0000 0072 1600 0000 7a26 5468 6520  ru...r....z&The 
 00002a70: 6275 696c 6469 6e67 2068 6173 2069 6e63  building has inc
 00002a80: 6f72 7265 6374 6c79 206e 756d 6265 7265  orrectly numbere
 00002a90: 6420 7a08 2065 6e74 7269 6573 290c 72a2  d z. entries).r.
-00002aa0: 0000 0072 4c00 0000 72a0 0000 0072 7700  ...rL...r....rw.
-00002ab0: 0000 7283 0000 0072 8b00 0000 721e 0000  ..r....r....r...
-00002ac0: 0072 7800 0000 5a0c 6e65 7769 6466 6f62  .rx...Z.newidfob
-00002ad0: 6a65 6374 728d 0000 0072 3300 0000 725e  jectr....r3...r^
-00002ae0: 0000 0029 0672 9600 0000 7287 0000 005a  ...).r....r....Z
+00002aa0: 0000 0072 4d00 0000 72a0 0000 0072 7800  ...rM...r....rx.
+00002ab0: 0000 7284 0000 0072 8c00 0000 721e 0000  ..r....r....r...
+00002ac0: 0072 7900 0000 da0c 6e65 7769 6466 6f62  .ry.....newidfob
+00002ad0: 6a65 6374 728e 0000 0072 3300 0000 725f  jectr....r3...r_
+00002ae0: 0000 0029 0672 9600 0000 7288 0000 005a  ...).r....r....Z
 00002af0: 0f6e 6577 5f6f 626a 6563 745f 6469 6374  .new_object_dict
 00002b00: 72a1 0000 00da 036e 756d da07 6e65 775f  r......num..new_
 00002b10: 6b65 7972 2000 0000 72a4 0000 0072 2100  keyr ...r....r!.
 00002b20: 0000 da0d 6164 645f 6f62 6a65 6374 6976  ....add_objectiv
 00002b30: 6564 0100 0073 3a00 0000 0006 0201 0e01  ed...s:.........
 00002b40: 0e01 0602 1402 0a02 0c02 04fe 0605 0a03  ................
 00002b50: 02fe 0201 0cff 0203 0801 0801 0eff 0201  ................
 00002b60: 02ff 0803 0802 0a01 0801 1002 06ff 0402  ................
 00002b70: 0cfe 0403 7a16 4550 5265 6164 6572 2e61  ....z.EPReader.a
 00002b80: 6464 5f6f 626a 6563 7469 7665 6302 0000  dd_objectivec...
 00002b90: 0000 0000 0000 0000 0002 0000 0003 0000  ................
 00002ba0: 0043 0000 0073 0e00 0000 7c00 a000 7c01  .C...s....|...|.
-00002bb0: a101 0100 6400 5300 7280 0000 0029 0172  ....d.S.r....).r
-00002bc0: a200 0000 a902 7296 0000 0072 8700 0000  ......r....r....
+00002bb0: a101 0100 6400 5300 7281 0000 0029 0172  ....d.S.r....).r
+00002bc0: a200 0000 a902 7296 0000 0072 8800 0000  ......r....r....
 00002bd0: 7220 0000 0072 2000 0000 7221 0000 00da  r ...r ...r!....
 00002be0: 0876 616c 6964 6174 658a 0100 0073 0200  .validate....s..
 00002bf0: 0000 0001 7a11 4550 5265 6164 6572 2e76  ....z.EPReader.v
 00002c00: 616c 6964 6174 6572 2500 0000 6302 0000  alidater%...c...
 00002c10: 0000 0000 0000 0000 0002 0000 0008 0000  ................
 00002c20: 0043 0000 0073 3c00 0000 7a0e 7c00 a000  .C...s<...z.|...
 00002c30: 7c01 a101 0100 5700 6e1e 0400 7401 6b0a  |.....W.n...t.k.
@@ -713,70 +713,70 @@
 00002c80: 7420 6974 2773 206f 7574 7075 7420 6361  t it's output ca
 00002c90: 6e20 6265 2072 6561 6420 6279 2074 6869  n be read by thi
 00002ca0: 7320 6d65 7465 722e 0a0a 2020 2020 2020  s meter...      
 00002cb0: 2020 3a70 6172 616d 2062 7569 6c64 696e    :param buildin
 00002cc0: 673a 2074 6865 2069 6466 2074 6f20 6d6f  g: the idf to mo
 00002cd0: 6469 6679 0a20 2020 2020 2020 203a 7265  dify.        :re
 00002ce0: 7475 726e 3a20 4e6f 6e65 0a20 2020 2020  turn: None.     
-00002cf0: 2020 204e 2904 72a2 0000 0072 4c00 0000     N).r....rL...
-00002d00: 72a8 0000 0072 aa00 0000 72a9 0000 0072  r....r....r....r
+00002cf0: 2020 204e 2904 72a2 0000 0072 4d00 0000     N).r....rM...
+00002d00: 72a9 0000 0072 ab00 0000 72aa 0000 0072  r....r....r....r
 00002d10: 2000 0000 7220 0000 0072 2100 0000 da05   ...r ...r!.....
 00002d20: 7365 7475 708d 0100 0073 0a00 0000 0006  setup....s......
 00002d30: 0201 0e01 0e01 1001 7a0e 4550 5265 6164  ........z.EPRead
 00002d40: 6572 2e73 6574 7570 6301 0000 0000 0000  er.setupc.......
 00002d50: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-00002d60: 0073 0400 0000 6400 5300 7280 0000 0072  .s....d.S.r....r
+00002d60: 0073 0400 0000 6400 5300 7281 0000 0072  .s....d.S.r....r
 00002d70: 2000 0000 a901 7296 0000 0072 2000 0000   .....r....r ...
 00002d80: 7220 0000 0072 2100 0000 da0c 7265 7375  r ...r!.....resu
 00002d90: 6c74 735f 6e61 6d65 9901 0000 7302 0000  lts_name....s...
 00002da0: 0000 027a 1545 5052 6561 6465 722e 7265  ...z.EPReader.re
-00002db0: 7375 6c74 735f 6e61 6d65 726e 0000 0063  sults_namern...c
+00002db0: 7375 6c74 735f 6e61 6d65 726f 0000 0063  sults_namero...c
 00002dc0: 0200 0000 0000 0000 0000 0000 0700 0000  ................
 00002dd0: 0400 0000 4300 0000 735e 0000 007c 00a0  ....C...s^...|..
 00002de0: 00a1 007d 027c 006a 0172 1e7c 017c 027c  ...}.|.j.r.|.|.|
 00002df0: 006a 0166 0219 007d 036e 367c 01a0 02a1  .j.f...}.n6|....
 00002e00: 0044 005d 1c5c 025c 027d 047d 057d 067c  .D.].\.\.}.}.}.|
 00002e10: 047c 026b 0272 267c 067d 0301 0071 5471  .|.k.r&|.}...qTq
 00002e20: 2674 0364 017c 029b 0064 029d 0383 0182  &t.d.|...d......
 00002e30: 017c 00a0 047c 03a1 0153 0029 034e fa13  .|...|...S.).N..
 00002e40: 4e6f 206d 6574 6572 2077 6974 6820 6e61  No meter with na
-00002e50: 6d65 20fa 0620 666f 756e 6429 0572 ad00  me .. found).r..
-00002e60: 0000 721e 0000 0072 3200 0000 724c 0000  ..r....r2...rL..
-00002e70: 0072 9100 0000 2907 7296 0000 0072 6c00  .r....).r....rl.
-00002e80: 0000 72ad 0000 00da 0d6d 6574 6572 5f72  ..r......meter_r
+00002e50: 6d65 20fa 0620 666f 756e 6429 0572 ae00  me .. found).r..
+00002e60: 0000 721e 0000 0072 3200 0000 724d 0000  ..r....r2...rM..
+00002e70: 0072 9200 0000 2907 7296 0000 0072 6d00  .r....).r....rm.
+00002e80: 0000 72ae 0000 00da 0d6d 6574 6572 5f72  ..r......meter_r
 00002e90: 6573 756c 7473 721c 0000 0072 2800 0000  esultsr....r(...
 00002ea0: da01 7672 2000 0000 7220 0000 0072 2100  ..vr ...r ...r!.
 00002eb0: 0000 da08 5f5f 6361 6c6c 5f5f 9d01 0000  ....__call__....
 00002ec0: 7312 0000 0000 0108 0106 0110 0214 0108  s...............
 00002ed0: 0104 0106 0210 017a 1145 5052 6561 6465  .......z.EPReade
 00002ee0: 722e 5f5f 6361 6c6c 5f5f 2915 7240 0000  r.__call__).r@..
 00002ef0: 0072 4100 0000 7242 0000 00da 0e4e 6f74  .rA...rB.....Not
-00002f00: 496d 706c 656d 656e 7465 6472 8b00 0000  Implementedr....
-00002f10: da05 7475 706c 6572 4500 0000 7270 0000  ..tuplerE...rp..
-00002f20: 0072 4400 0000 7293 0000 0072 9f00 0000  .rD...r....r....
-00002f30: 72a2 0000 0072 a800 0000 72aa 0000 0072  r....r....r....r
-00002f40: ab00 0000 7203 0000 0072 ad00 0000 da0f  ....r....r......
+00002f00: 496d 706c 656d 656e 7465 6472 8c00 0000  Implementedr....
+00002f10: da05 7475 706c 6572 4500 0000 7271 0000  ..tuplerE...rq..
+00002f20: 0072 4400 0000 7294 0000 0072 9f00 0000  .rD...r....r....
+00002f30: 72a2 0000 0072 a900 0000 72ab 0000 0072  r....r....r....r
+00002f40: ac00 0000 7203 0000 0072 ae00 0000 da0f  ....r....r......
 00002f50: 5f72 6573 756c 7473 5f66 6f72 6d61 7472  _results_formatr
-00002f60: 5600 0000 72b2 0000 00da 0d5f 5f63 6c61  V...r......__cla
+00002f60: 5700 0000 72b3 0000 00da 0d5f 5f63 6c61  W...r......__cla
 00002f70: 7373 6365 6c6c 5f5f 7220 0000 0072 2000  sscell__r ...r .
-00002f80: 0000 7297 0000 0072 2100 0000 728a 0000  ..r....r!...r...
+00002f80: 0000 7297 0000 0072 2100 0000 728b 0000  ..r....r!...r...
 00002f90: 002a 0100 0073 1400 0000 0a01 0c02 1a0b  .*...s..........
-00002fa0: 0814 0818 0826 0803 0e0c 0201 0a03 728a  .....&........r.
+00002fa0: 0814 0818 0826 0803 0e0c 0201 0a03 728b  .....&........r.
 00002fb0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
 00002fc0: 0000 0000 0700 0000 0000 0000 734e 0000  ............sN..
 00002fd0: 0065 005a 0164 005a 0264 015a 0365 046a  .e.Z.d.Z.d.Z.e.j
 00002fe0: 0564 0265 0664 0366 0465 0765 0765 0765  .d.e.d.f.e.e.e.e
 00002ff0: 0865 0764 049c 0587 0066 0164 0564 0684  .e.d.....f.d.d..
 00003000: 0d5a 0964 0764 0884 005a 0a65 0b64 0964  .Z.d.d...Z.e.d.d
 00003010: 0a84 0083 015a 0c87 0004 005a 0d53 0029  .....Z.....Z.S.)
 00003020: 0bda 0b4d 6574 6572 5265 6164 6572 2902  ...MeterReader).
 00003030: 2902 da08 6b65 795f 6e61 6d65 5a08 4b65  )...key_nameZ.Ke
 00003040: 795f 4e61 6d65 a902 721e 0000 0072 a500  y_Name..r....r..
-00003050: 0000 4e72 8c00 0000 2905 72b8 0000 0072  ..Nr....).r....r
-00003060: 8d00 0000 721e 0000 0072 9000 0000 721c  ....r....r....r.
+00003050: 0000 4e72 8d00 0000 2905 72b9 0000 0072  ..Nr....).r....r
+00003060: 8e00 0000 721e 0000 0072 9100 0000 721c  ....r....r....r.
 00003070: 0000 0063 0600 0000 0000 0000 0000 0000  ...c............
 00003080: 0600 0000 0600 0000 0300 0000 732c 0000  ............s,..
 00003090: 0074 0083 006a 017c 027c 037c 047c 0564  .t...j.|.|.|.|.d
 000030a0: 018d 0401 007c 017c 005f 027c 006a 0364  .....|.|._.|.j.d
 000030b0: 0264 0364 048d 0201 0064 0553 0029 0661  .d.d.....d.S.).a
 000030c0: 9501 0000 0a0a 2020 2020 2020 2020 3a70  ......        :p
 000030d0: 6172 616d 206b 6579 5f6e 616d 653a 2057  aram key_name: W
@@ -799,63 +799,63 @@
 000031e0: 6520 7265 7375 6c74 7320 7265 6164 2066  e results read f
 000031f0: 726f 6d20 7468 6520 6669 6c65 2e0a 2020  rom the file..  
 00003200: 2020 2020 2020 3a70 6172 616d 206e 616d        :param nam
 00003210: 653a 2074 6865 206e 616d 6520 6f66 2074  e: the name of t
 00003220: 6865 206f 7574 7075 7420 636f 6c75 6d6e  he output column
 00003230: 2063 6f72 7265 7370 6f6e 6469 6e67 2074   corresponding t
 00003240: 6f20 7468 6973 206f 626a 6563 7469 7665  o this objective
-00003250: 0a20 2020 2020 2020 20a9 0472 8d00 0000  .        ..r....
-00003260: 721e 0000 0072 9000 0000 721c 0000 0072  r....r....r....r
-00003270: b800 0000 5472 8e00 0000 4e29 0472 9200  ....Tr....N).r..
-00003280: 0000 7293 0000 0072 b800 0000 7295 0000  ..r....r....r...
-00003290: 0029 0672 9600 0000 72b8 0000 0072 8d00  .).r....r....r..
-000032a0: 0000 721e 0000 0072 9000 0000 721c 0000  ..r....r....r...
+00003250: 0a20 2020 2020 2020 20a9 0472 8e00 0000  .        ..r....
+00003260: 721e 0000 0072 9100 0000 721c 0000 0072  r....r....r....r
+00003270: b900 0000 5472 8f00 0000 4e29 0472 9300  ....Tr....N).r..
+00003280: 0000 7294 0000 0072 b900 0000 7295 0000  ..r....r....r...
+00003290: 0029 0672 9600 0000 72b9 0000 0072 8e00  .).r....r....r..
+000032a0: 0000 721e 0000 0072 9100 0000 721c 0000  ..r....r....r...
 000032b0: 0072 9700 0000 7220 0000 0072 2100 0000  .r....r ...r!...
-000032c0: 7293 0000 00ae 0100 0073 1000 0000 0010  r........s......
+000032c0: 7294 0000 00ae 0100 0073 1000 0000 0010  r........s......
 000032d0: 0601 0200 0200 0200 02ff 0603 0601 7a14  ..............z.
 000032e0: 4d65 7465 7252 6561 6465 722e 5f5f 696e  MeterReader.__in
 000032f0: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
 00003300: 0001 0000 0001 0000 0043 0000 0073 0600  .........C...s..
-00003310: 0000 7c00 6a00 5300 7280 0000 00a9 0172  ..|.j.S.r......r
-00003320: b800 0000 72ac 0000 0072 2000 0000 7220  ....r....r ...r 
-00003330: 0000 0072 2100 0000 72ad 0000 00c4 0100  ...r!...r.......
+00003310: 0000 7c00 6a00 5300 7281 0000 00a9 0172  ..|.j.S.r......r
+00003320: b900 0000 72ad 0000 0072 2000 0000 7220  ....r....r ...r 
+00003330: 0000 0072 2100 0000 72ae 0000 00c4 0100  ...r!...r.......
 00003340: 0073 0200 0000 0001 7a18 4d65 7465 7252  .s......z.MeterR
 00003350: 6561 6465 722e 7265 7375 6c74 735f 6e61  eader.results_na
 00003360: 6d65 6301 0000 0000 0000 0000 0000 0001  mec.............
 00003370: 0000 0001 0000 0043 0000 0073 0600 0000  .......C...s....
-00003380: 7c00 6a00 5300 7280 0000 0072 bb00 0000  |.j.S.r....r....
-00003390: 72ac 0000 0072 2000 0000 7220 0000 0072  r....r ...r ...r
+00003380: 7c00 6a00 5300 7281 0000 0072 bc00 0000  |.j.S.r....r....
+00003390: 72ad 0000 0072 2000 0000 7220 0000 0072  r....r ...r ...r
 000033a0: 2100 0000 da0d 5f64 6566 6175 6c74 5f6e  !....._default_n
 000033b0: 616d 65c7 0100 0073 0200 0000 0002 7a19  ame....s......z.
 000033c0: 4d65 7465 7252 6561 6465 722e 5f64 6566  MeterReader._def
 000033d0: 6175 6c74 5f6e 616d 6529 0e72 4000 0000  ault_name).r@...
-000033e0: 7241 0000 0072 4200 0000 728b 0000 0072  rA...rB...r....r
+000033e0: 7241 0000 0072 4200 0000 728c 0000 0072  rA...rB...r....r
 000033f0: 0e00 0000 da14 6f62 6a65 6374 6976 655f  ......objective_
-00003400: 6d65 7465 725f 7479 7065 7270 0000 0072  meter_typerp...r
-00003410: 4400 0000 720b 0000 0072 9300 0000 72ad  D...r....r....r.
-00003420: 0000 00da 0870 726f 7065 7274 7972 bc00  .....propertyr..
-00003430: 0000 72b6 0000 0072 2000 0000 7220 0000  ..r....r ...r ..
-00003440: 0072 9700 0000 7221 0000 0072 b700 0000  .r....r!...r....
+00003400: 6d65 7465 725f 7479 7065 7271 0000 0072  meter_typerq...r
+00003410: 4400 0000 720b 0000 0072 9400 0000 72ae  D...r....r....r.
+00003420: 0000 00da 0870 726f 7065 7274 7972 bd00  .....propertyr..
+00003430: 0000 72b7 0000 0072 2000 0000 7220 0000  ..r....r ...r ..
+00003440: 0072 9700 0000 7221 0000 0072 b800 0000  .r....r!...r....
 00003450: ab01 0000 731e 0000 0008 0104 0504 0102  ....s...........
 00003460: 0102 0102 fa02 0202 0102 0102 0102 0102  ................
-00003470: fa10 1608 0302 0172 b700 0000 6300 0000  .......r....c...
+00003470: fa10 1608 0302 0172 b800 0000 6300 0000  .......r....c...
 00003480: 0000 0000 0000 0000 0000 0000 0005 0000  ................
 00003490: 0000 0000 0073 5a00 0000 6500 5a01 6400  .....sZ...e.Z.d.
 000034a0: 5a02 6401 5a03 6402 6504 6a05 6403 6506  Z.d.Z.d.e.j.d.e.
 000034b0: 6404 6605 6507 6508 6405 9c02 8700 6601  d.f.e.e.d.....f.
 000034c0: 6406 6407 840d 5a09 6408 6409 8400 5a0a  d.d...Z.d.d...Z.
 000034d0: 650b 640a 640b 8400 8301 5a0c 650d 650e  e.d.d.....Z.e.e.
 000034e0: 640c 9c02 640d 640e 8404 5a0f 8700 0400  d...d.d...Z.....
 000034f0: 5a10 5300 290f da0e 5661 7269 6162 6c65  Z.S.)...Variable
 00003500: 5265 6164 6572 2903 2902 da09 6b65 795f  Reader).)...key_
 00003510: 7661 6c75 655a 094b 6579 5f56 616c 7565  valueZ.Key_Value
 00003520: 2902 da0d 7661 7269 6162 6c65 5f6e 616d  )...variable_nam
 00003530: 655a 0d56 6172 6961 626c 655f 4e61 6d65  eZ.Variable_Name
-00003540: 72b9 0000 00da 012a 4e72 8c00 0000 2902  r......*Nr....).
-00003550: 721e 0000 0072 9000 0000 6307 0000 0000  r....r....c.....
+00003540: 72ba 0000 00da 012a 4e72 8d00 0000 2902  r......*Nr....).
+00003550: 721e 0000 0072 9100 0000 6307 0000 0000  r....r....c.....
 00003560: 0000 0000 0000 0007 0000 0006 0000 0003  ................
 00003570: 0000 0073 4200 0000 7400 8300 6a01 7c03  ...sB...t...j.|.
 00003580: 7c04 7c05 7c06 6401 8d04 0100 7c01 7c00  |.|.|.d.....|.|.
 00003590: 5f02 7c00 a003 6402 a101 0100 7c02 7c00  _.|...d.....|.|.
 000035a0: 5f04 7c00 6a04 6403 6b03 723e 7c00 a003  _.|.j.d.k.r>|...
 000035b0: 6404 a101 0100 6405 5300 2906 61b6 0200  d.....d.S.).a...
 000035c0: 0052 6561 6473 2074 6865 2076 616c 7565  .Reads the value
@@ -897,104 +897,108 @@
 00003800: 6573 756c 7473 2072 6561 6420 6672 6f6d  esults read from
 00003810: 2074 6865 2066 696c 652e 0a20 2020 2020   the file..     
 00003820: 2020 203a 7061 7261 6d20 6e61 6d65 3a20     :param name: 
 00003830: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
 00003840: 6f75 7470 7574 2063 6f6c 756d 6e20 636f  output column co
 00003850: 7272 6573 706f 6e64 696e 6720 746f 2074  rresponding to t
 00003860: 6869 7320 6f62 6a65 6374 6976 652e 0a20  his objective.. 
-00003870: 2020 2020 2020 2072 ba00 0000 72c0 0000         r....r...
-00003880: 0072 c200 0000 72c1 0000 004e 2905 7292  .r....r....N).r.
-00003890: 0000 0072 9300 0000 72c0 0000 0072 9500  ...r....r....r..
-000038a0: 0000 72c1 0000 0029 0772 9600 0000 72c0  ..r....).r....r.
-000038b0: 0000 0072 c100 0000 728d 0000 0072 1e00  ...r....r....r..
-000038c0: 0000 7290 0000 0072 1c00 0000 7297 0000  ..r....r....r...
-000038d0: 0072 2000 0000 7221 0000 0072 9300 0000  .r ...r!...r....
+00003870: 2020 2020 2020 2072 bb00 0000 72c1 0000         r....r...
+00003880: 0072 c300 0000 72c2 0000 004e 2905 7293  .r....r....N).r.
+00003890: 0000 0072 9400 0000 72c1 0000 0072 9500  ...r....r....r..
+000038a0: 0000 72c2 0000 0029 0772 9600 0000 72c1  ..r....).r....r.
+000038b0: 0000 0072 c200 0000 728e 0000 0072 1e00  ...r....r....r..
+000038c0: 0000 7291 0000 0072 1c00 0000 7297 0000  ..r....r....r...
+000038d0: 0072 2000 0000 7221 0000 0072 9400 0000  .r ...r!...r....
 000038e0: d401 0000 7316 0000 0000 1406 0102 0002  ....s...........
 000038f0: 0002 0002 ff06 0306 010a 0106 010a 017a  ...............z
 00003900: 1756 6172 6961 626c 6552 6561 6465 722e  .VariableReader.
 00003910: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
 00003920: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
-00003930: 0073 1600 0000 7c00 6a00 a001 a100 9b00  .s....|.j.......
-00003940: 6401 7c00 6a02 9b00 9d03 5300 2902 4e72  d.|.j.....S.).Nr
-00003950: 1500 0000 2903 72c0 0000 00da 0575 7070  ....).r......upp
-00003960: 6572 72c1 0000 0072 ac00 0000 7220 0000  err....r....r ..
-00003970: 0072 2000 0000 7221 0000 0072 ad00 0000  .r ...r!...r....
-00003980: f101 0000 7302 0000 0000 037a 1b56 6172  ....s......z.Var
-00003990: 6961 626c 6552 6561 6465 722e 7265 7375  iableReader.resu
-000039a0: 6c74 735f 6e61 6d65 6301 0000 0000 0000  lts_namec.......
-000039b0: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-000039c0: 0073 0600 0000 7c00 6a00 5300 7280 0000  .s....|.j.S.r...
-000039d0: 0029 0172 c100 0000 72ac 0000 0072 2000  .).r....r....r .
-000039e0: 0000 7220 0000 0072 2100 0000 72bc 0000  ..r ...r!...r...
-000039f0: 00f6 0100 0073 0200 0000 0002 7a1c 5661  .....s......z.Va
-00003a00: 7269 6162 6c65 5265 6164 6572 2e5f 6465  riableReader._de
-00003a10: 6661 756c 745f 6e61 6d65 726e 0000 0063  fault_namern...c
-00003a20: 0200 0000 0000 0000 0000 0000 0800 0000  ................
-00003a30: 0600 0000 4300 0000 73aa 0000 007c 00a0  ....C...s....|..
-00003a40: 00a1 007d 0267 007d 037c 006a 0172 2a7c  ...}.g.}.|.j.r*|
-00003a50: 017c 027c 006a 0166 0219 007d 047c 00a0  .|.|.j.f...}.|..
-00003a60: 027c 04a1 0153 007c 01a0 03a1 0044 005d  .|...S.|.....D.]
-00003a70: 5a5c 025c 027d 057d 067d 077c 006a 0464  Z\.\.}.}.}.|.j.d
-00003a80: 016b 0372 647c 057c 026b 0272 8c7c 077d  .k.rd|.|.k.r.|.}
-00003a90: 047c 00a0 027c 04a1 0102 0001 0053 0071  .|...|.......S.q
-00003aa0: 3274 05a0 0664 027c 006a 079b 009d 027c  2t...d.|.j.....|
-00003ab0: 05a1 0272 327c 077d 047c 03a0 087c 00a0  ...r2|.}.|...|..
-00003ac0: 027c 04a1 01a1 0101 0071 327c 0372 967c  .|.......q2|.r.|
-00003ad0: 0353 0074 0964 037c 029b 0064 049d 0383  .S.t.d.|...d....
-00003ae0: 0182 0164 0053 0029 054e 72c2 0000 007a  ...d.S.).Nr....z
-00003af0: 045c 772b 2c72 ae00 0000 72af 0000 0029  .\w+,r....r....)
-00003b00: 0a72 ad00 0000 721e 0000 0072 9100 0000  .r....r....r....
-00003b10: 7232 0000 0072 c000 0000 7218 0000 0072  r2...r....r....r
-00003b20: 4b00 0000 72c1 0000 0072 6100 0000 724c  K...r....ra...rL
-00003b30: 0000 0029 0872 9600 0000 726c 0000 0072  ...).r....rl...r
-00003b40: ad00 0000 5a0c 7265 7375 6c74 735f 6c69  ....Z.results_li
-00003b50: 7374 72b0 0000 0072 1c00 0000 7228 0000  str....r....r(..
-00003b60: 0072 b100 0000 7220 0000 0072 2000 0000  .r....r ...r ...
-00003b70: 7221 0000 0072 b200 0000 fb01 0000 7320  r!...r........s 
-00003b80: 0000 0000 0108 0104 0206 010e 010a 0214  ................
-00003b90: 010a 0108 0104 0110 0214 0104 0112 0204  ................
-00003ba0: 0104 027a 1756 6172 6961 626c 6552 6561  ...z.VariableRea
-00003bb0: 6465 722e 5f5f 6361 6c6c 5f5f 2911 7240  der.__call__).r@
-00003bc0: 0000 0072 4100 0000 7242 0000 0072 8b00  ...rA...rB...r..
-00003bd0: 0000 720e 0000 00da 176f 626a 6563 7469  ..r......objecti
-00003be0: 7665 5f76 6172 6961 626c 655f 7479 7065  ve_variable_type
-00003bf0: 7270 0000 0072 4400 0000 720b 0000 0072  rp...rD...r....r
-00003c00: 9300 0000 72ad 0000 0072 be00 0000 72bc  ....r....r....r.
-00003c10: 0000 0072 b500 0000 7285 0000 0072 b200  ...r....r....r..
-00003c20: 0000 72b6 0000 0072 2000 0000 7220 0000  ..r....r ...r ..
-00003c30: 0072 9700 0000 7221 0000 0072 bf00 0000  .r....r!...r....
-00003c40: cc01 0000 731c 0000 0008 0104 0a02 0104  ....s...........
-00003c50: 0102 0102 0102 f902 0502 0102 fa10 1d08  ................
-00003c60: 0502 010a 0472 bf00 0000 2901 7271 0000  .....r....).rq..
-00003c70: 0029 3872 4300 0000 7218 0000 00da 0361  .)8rC...r......a
-00003c80: 6263 7202 0000 0072 0300 0000 da0b 6461  bcr....r......da
-00003c90: 7461 636c 6173 7365 7372 0400 0000 da09  taclassesr......
-00003ca0: 6974 6572 746f 6f6c 7372 0500 0000 da07  itertoolsr......
-00003cb0: 7061 7468 6c69 6272 0600 0000 da06 7479  pathlibr......ty
-00003cc0: 7069 6e67 7207 0000 0072 0800 0000 7209  pingr....r....r.
-00003cd0: 0000 0072 0a00 0000 720b 0000 00da 0877  ...r....r......w
-00003ce0: 6172 6e69 6e67 7372 0c00 0000 da06 7061  arningsr......pa
-00003cf0: 6e64 6173 7234 0000 00da 1170 6163 6b61  ndasr4.....packa
-00003d00: 6769 6e67 2e76 6572 7369 6f6e 720d 0000  ging.versionr...
-00003d10: 00da 0562 6573 6f73 720e 0000 0072 0f00  ...besosr....r..
-00003d20: 0000 7277 0000 00da 1062 6573 6f73 2e49  ..rw.....besos.I
-00003d30: 4f5f 4f62 6a65 6374 7372 1000 0000 5a0c  O_Objectsr....Z.
-00003d40: 6265 736f 732e 6572 726f 7273 7211 0000  besos.errorsr...
-00003d50: 005a 1062 6573 6f73 2e62 6573 6f73 7479  .Z.besos.besosty
-00003d60: 7065 7372 1200 0000 da07 6c6f 6767 696e  pesr......loggin
-00003d70: 6772 1300 0000 5a03 6c67 64da 0967 6574  gr....Z.lgd..get
-00003d80: 4c6f 6767 6572 7240 0000 00da 036c 6f67  Loggerr@.....log
-00003d90: da0a 6164 6448 616e 646c 6572 da0b 4e75  ..addHandler..Nu
-00003da0: 6c6c 4861 6e64 6c65 7272 2200 0000 7256  llHandlerr"...rV
-00003db0: 0000 005a 125f 7661 6c75 6573 5f63 6f6c  ...Z._values_col
-00003dc0: 6c65 6374 696f 6e72 2300 0000 7244 0000  lectionr#...rD..
-00003dd0: 0072 b500 0000 7250 0000 0072 5100 0000  .r....rP...rQ...
-00003de0: 726a 0000 0072 6d00 0000 7270 0000 0072  rj...rm...rp...r
-00003df0: 8900 0000 728a 0000 0072 b700 0000 72bf  ....r....r....r.
-00003e00: 0000 0072 2000 0000 7220 0000 0072 2000  ...r ...r ...r .
-00003e10: 0000 7221 0000 00da 083c 6d6f 6475 6c65  ..r!.....<module
-00003e20: 3e01 0000 0073 4e00 0000 0410 0801 1001  >....sN.........
-00003e30: 0c01 0c01 0c01 1c01 0c03 0801 0c03 0c01  ................
-00003e40: 0c01 0c01 0c01 0c02 0801 0c01 0802 0a01  ................
-00003e50: 0e03 080e 0c03 0201 1024 1403 1017 0401  .........$......
-00003e60: 0201 02fd 0201 0203 02fc 0c5a 0e11 100a  ...........Z....
-00003e70: 1e3a 127f 0002 1021                      .:.....!
+00003930: 0073 3e00 0000 7c00 6a00 a001 a100 6401  .s>...|.j.....d.
+00003940: 6b02 7224 7c00 6a00 a001 a100 9b00 6402  k.r$|.j.......d.
+00003950: 7c00 6a02 9b00 9d03 5300 7c00 6a00 a003  |.j.....S.|.j...
+00003960: a100 9b00 6402 7c00 6a02 9b00 9d03 5300  ....d.|.j.....S.
+00003970: 6400 5300 2903 4eda 0b45 6e76 6972 6f6e  d.S.).N..Environ
+00003980: 6d65 6e74 7215 0000 0029 0472 c100 0000  mentr....).r....
+00003990: da0a 6361 7069 7461 6c69 7a65 72c2 0000  ..capitalizer...
+000039a0: 00da 0575 7070 6572 72ad 0000 0072 2000  ...upperr....r .
+000039b0: 0000 7220 0000 0072 2100 0000 72ae 0000  ..r ...r!...r...
+000039c0: 00f1 0100 0073 0600 0000 0003 0e01 1602  .....s..........
+000039d0: 7a1b 5661 7269 6162 6c65 5265 6164 6572  z.VariableReader
+000039e0: 2e72 6573 756c 7473 5f6e 616d 6563 0100  .results_namec..
+000039f0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+00003a00: 0000 4300 0000 7306 0000 007c 006a 0053  ..C...s....|.j.S
+00003a10: 0072 8100 0000 2901 72c2 0000 0072 ad00  .r....).r....r..
+00003a20: 0000 7220 0000 0072 2000 0000 7221 0000  ..r ...r ...r!..
+00003a30: 0072 bd00 0000 f901 0000 7302 0000 0000  .r........s.....
+00003a40: 027a 1c56 6172 6961 626c 6552 6561 6465  .z.VariableReade
+00003a50: 722e 5f64 6566 6175 6c74 5f6e 616d 6572  r._default_namer
+00003a60: 6f00 0000 6302 0000 0000 0000 0000 0000  o...c...........
+00003a70: 0008 0000 0006 0000 0043 0000 0073 aa00  .........C...s..
+00003a80: 0000 7c00 a000 a100 7d02 6700 7d03 7c00  ..|.....}.g.}.|.
+00003a90: 6a01 722a 7c01 7c02 7c00 6a01 6602 1900  j.r*|.|.|.j.f...
+00003aa0: 7d04 7c00 a002 7c04 a101 5300 7c01 a003  }.|...|...S.|...
+00003ab0: a100 4400 5d5a 5c02 5c02 7d05 7d06 7d07  ..D.]Z\.\.}.}.}.
+00003ac0: 7c00 6a04 6401 6b03 7264 7c05 7c02 6b02  |.j.d.k.rd|.|.k.
+00003ad0: 728c 7c07 7d04 7c00 a002 7c04 a101 0200  r.|.}.|...|.....
+00003ae0: 0100 5300 7132 7405 a006 6402 7c00 6a07  ..S.q2t...d.|.j.
+00003af0: 9b00 9d02 7c05 a102 7232 7c07 7d04 7c03  ....|...r2|.}.|.
+00003b00: a008 7c00 a002 7c04 a101 a101 0100 7132  ..|...|.......q2
+00003b10: 7c03 7296 7c03 5300 7409 6403 7c02 9b00  |.r.|.S.t.d.|...
+00003b20: 6404 9d03 8301 8201 6400 5300 2905 4e72  d.......d.S.).Nr
+00003b30: c300 0000 7a04 5c77 2b2c 72af 0000 0072  ....z.\w+,r....r
+00003b40: b000 0000 290a 72ae 0000 0072 1e00 0000  ....).r....r....
+00003b50: 7292 0000 0072 3200 0000 72c1 0000 0072  r....r2...r....r
+00003b60: 1800 0000 724c 0000 0072 c200 0000 7262  ....rL...r....rb
+00003b70: 0000 0072 4d00 0000 2908 7296 0000 0072  ...rM...).r....r
+00003b80: 6d00 0000 72ae 0000 005a 0c72 6573 756c  m...r....Z.resul
+00003b90: 7473 5f6c 6973 7472 b100 0000 721c 0000  ts_listr....r...
+00003ba0: 0072 2800 0000 72b2 0000 0072 2000 0000  .r(...r....r ...
+00003bb0: 7220 0000 0072 2100 0000 72b3 0000 00fe  r ...r!...r.....
+00003bc0: 0100 0073 2000 0000 0001 0801 0402 0601  ...s ...........
+00003bd0: 0e01 0a02 1401 0a01 0801 0401 1002 1401  ................
+00003be0: 0401 1202 0401 0402 7a17 5661 7269 6162  ........z.Variab
+00003bf0: 6c65 5265 6164 6572 2e5f 5f63 616c 6c5f  leReader.__call_
+00003c00: 5f29 1172 4000 0000 7241 0000 0072 4200  _).r@...rA...rB.
+00003c10: 0000 728c 0000 0072 0e00 0000 da17 6f62  ..r....r......ob
+00003c20: 6a65 6374 6976 655f 7661 7269 6162 6c65  jective_variable
+00003c30: 5f74 7970 6572 7100 0000 7244 0000 0072  _typerq...rD...r
+00003c40: 0b00 0000 7294 0000 0072 ae00 0000 72bf  ....r....r....r.
+00003c50: 0000 0072 bd00 0000 72b6 0000 0072 8600  ...r....r....r..
+00003c60: 0000 72b3 0000 0072 b700 0000 7220 0000  ..r....r....r ..
+00003c70: 0072 2000 0000 7297 0000 0072 2100 0000  .r ...r....r!...
+00003c80: 72c0 0000 00cc 0100 0073 1c00 0000 0801  r........s......
+00003c90: 040a 0201 0401 0201 0201 02f9 0205 0201  ................
+00003ca0: 02fa 101d 0808 0201 0a04 72c0 0000 0029  ..........r....)
+00003cb0: 0172 7200 0000 2938 7243 0000 0072 1800  .rr...)8rC...r..
+00003cc0: 0000 da03 6162 6372 0200 0000 7203 0000  ....abcr....r...
+00003cd0: 00da 0b64 6174 6163 6c61 7373 6573 7204  ...dataclassesr.
+00003ce0: 0000 00da 0969 7465 7274 6f6f 6c73 7205  .....itertoolsr.
+00003cf0: 0000 00da 0770 6174 686c 6962 7206 0000  .....pathlibr...
+00003d00: 00da 0674 7970 696e 6772 0700 0000 7208  ...typingr....r.
+00003d10: 0000 0072 0900 0000 720a 0000 0072 0b00  ...r....r....r..
+00003d20: 0000 da08 7761 726e 696e 6773 720c 0000  ....warningsr...
+00003d30: 00da 0670 616e 6461 7372 3400 0000 da11  ...pandasr4.....
+00003d40: 7061 636b 6167 696e 672e 7665 7273 696f  packaging.versio
+00003d50: 6e72 0d00 0000 da05 6265 736f 7372 0e00  nr......besosr..
+00003d60: 0000 720f 0000 0072 7800 0000 5a10 6265  ..r....rx...Z.be
+00003d70: 736f 732e 494f 5f4f 626a 6563 7473 7210  sos.IO_Objectsr.
+00003d80: 0000 00da 0c62 6573 6f73 2e65 7272 6f72  .....besos.error
+00003d90: 7372 1100 0000 da10 6265 736f 732e 6265  sr......besos.be
+00003da0: 736f 7374 7970 6573 7212 0000 00da 076c  sostypesr......l
+00003db0: 6f67 6769 6e67 7213 0000 005a 036c 6764  oggingr....Z.lgd
+00003dc0: da09 6765 744c 6f67 6765 7272 4000 0000  ..getLoggerr@...
+00003dd0: da03 6c6f 67da 0a61 6464 4861 6e64 6c65  ..log..addHandle
+00003de0: 72da 0b4e 756c 6c48 616e 646c 6572 7222  r..NullHandlerr"
+00003df0: 0000 0072 5700 0000 5a12 5f76 616c 7565  ...rW...Z._value
+00003e00: 735f 636f 6c6c 6563 7469 6f6e 7223 0000  s_collectionr#..
+00003e10: 0072 4400 0000 72b6 0000 0072 5100 0000  .rD...r....rQ...
+00003e20: 7252 0000 0072 6b00 0000 726e 0000 0072  rR...rk...rn...r
+00003e30: 7100 0000 728a 0000 0072 8b00 0000 72b8  q...r....r....r.
+00003e40: 0000 0072 c000 0000 7220 0000 0072 2000  ...r....r ...r .
+00003e50: 0000 7220 0000 0072 2100 0000 da08 3c6d  ..r ...r!.....<m
+00003e60: 6f64 756c 653e 0100 0000 734e 0000 0004  odule>....sN....
+00003e70: 1008 0110 010c 010c 010c 011c 010c 0308  ................
+00003e80: 010c 030c 010c 010c 010c 010c 0208 010c  ................
+00003e90: 0108 020a 010e 0308 0e0c 0302 0110 2414  ..............$.
+00003ea0: 0310 1704 0102 0102 fd02 0102 0302 fc0c  ................
+00003eb0: 5a0e 1110 0a1e 3a12 7f00 0210 21         Z.....:.....!
```

### Comparing `besos-2.2.2/besos/__pycache__/optimizer.cpython-38.pyc` & `besos-2.2.3/besos/__pycache__/optimizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/__pycache__/parameters.cpython-38.pyc` & `besos-2.2.3/besos/__pycache__/parameters.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/__pycache__/problem.cpython-38.pyc` & `besos-2.2.3/besos/__pycache__/problem.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/__pycache__/pyehub_funcs.cpython-38.pyc` & `besos-2.2.3/besos/__pycache__/pyehub_funcs.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Oct 31 03:04:31 2023 UTC, .py size: 4719 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 bf6e 4065 6f12 0000  U........n@eo...
+00000000: 550d 0d0a 0000 0000 31c8 1166 e311 0000  U.......1..f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 c600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6402 6c06 5a07 6401 6402 6c08  ..d.d.l.Z.d.d.l.
 00000060: 5a09 6401 6402 6c0a 5a0a 6401 6405 6c0b  Z.d.d.l.Z.d.d.l.
 00000070: 6d0b 5a0b 0100 6401 6406 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
@@ -92,20 +92,20 @@
 000005b0: 7920 6875 6220 666f 7220 7468 6520 7061  y hub for the pa
 000005c0: 7261 6d65 7465 7273 2073 7065 6369 6669  rameters specifi
 000005d0: 6564 0a20 2020 206f 6e20 696e 6974 6961  ed.    on initia
 000005e0: 6c69 7a61 7469 6f6e 2077 6974 6820 7468  lization with th
 000005f0: 6520 7661 6c75 6573 2067 6976 656e 2074  e values given t
 00000600: 6f20 6576 616c 7561 746f 722e 4e29 03da  o evaluator.N)..
 00000610: 037a 6970 da08 7365 6c65 6374 6f72 da03  .zip..selector..
-00000620: 7365 7429 055a 0368 7562 721a 0000 0072  set).Z.hubr....r
+00000620: 7365 7429 05da 0368 7562 721a 0000 0072  set)...hubr....r
 00000630: 1b00 0000 da09 7061 7261 6d65 7465 7272  ......parameterr
 00000640: 1600 0000 7209 0000 0072 0900 0000 720a  ....r....r....r.
 00000650: 0000 00da 1770 7965 6875 625f 7061 7261  .....pyehub_para
 00000660: 6d65 7465 725f 6564 6974 6f72 3000 0000  meter_editor0...
-00000670: 7304 0000 0000 0a12 0172 2000 0000 6301  s........r ...c.
+00000670: 7304 0000 0000 0a12 0172 2100 0000 6301  s........r!...c.
 00000680: 0000 0000 0000 0000 0000 0003 0000 0003  ................
 00000690: 0000 0043 0000 0073 2c00 0000 7c00 a000  ...C...s,...|...
 000006a0: 6401 a101 7d01 7c01 a001 a100 7d01 7c00  d...}.|.....}.|.
 000006b0: a002 6401 a101 7d02 7c02 a001 a100 7d02  ..d...}.|.....}.
 000006c0: 7c01 7c02 6602 5300 2902 7a8a 0a20 2020  |.|.f.S.).z..   
 000006d0: 2053 706c 6974 7320 7468 6520 686f 7572   Splits the hour
 000006e0: 6c79 2073 6572 6965 7320 6f66 2045 5020  ly series of EP 
@@ -114,19 +114,19 @@
 00000710: 6c65 2064 6179 7320 696e 2064 6966 6665  le days in diffe
 00000720: 7265 6e74 2073 6561 736f 6e73 2069 6e74  rent seasons int
 00000730: 6f20 7370 6563 6966 6963 2065 6e65 7267  o specific energ
 00000740: 7968 7562 2074 696d 6520 7365 7269 6573  yhub time series
 00000750: 2e0a 2020 2020 e918 0000 0029 03da 0468  ..    .....)...h
 00000760: 6561 64da 0b72 6573 6574 5f69 6e64 6578  ead..reset_index
 00000770: da04 7461 696c 2903 5a0d 686f 7572 6c79  ..tail).Z.hourly
-00000780: 5f73 6572 6965 735a 0772 6573 756c 7431  _seriesZ.result1
+00000780: 5f73 6572 6965 73da 0772 6573 756c 7431  _series..result1
 00000790: da07 7265 7375 6c74 3272 0900 0000 7209  ..result2r....r.
 000007a0: 0000 0072 0a00 0000 da0e 5f73 706c 6974  ...r......_split
 000007b0: 5f45 505f 6461 7973 3e00 0000 730a 0000  _EP_days>...s...
-000007c0: 0000 050a 0108 010a 0108 0172 2600 0000  ...........r&...
+000007c0: 0000 050a 0108 010a 0108 0172 2800 0000  ...........r(...
 000007d0: 6302 0000 0000 0000 0000 0000 0011 0000  c...............
 000007e0: 0006 0000 0043 0000 0073 f000 0000 7c00  .....C...s....|.
 000007f0: a000 a100 7d02 6700 7d03 7c02 4400 5d0e  ....}.g.}.|.D.].
 00000800: 7d04 7c03 a001 7c04 a101 0100 7110 7402  }.|...|.....q.t.
 00000810: 6a03 7c03 6401 8d01 7d05 7c02 4400 5dba  j.|.d...}.|.D.].
 00000820: 7d06 7c02 7c06 1900 4400 5dac 7d07 7c02  }.|.|...D.].}.|.
 00000830: 7c06 1900 7c07 1900 a004 a100 7d08 7405  |...|.......}.t.
@@ -146,15 +146,15 @@
 00000910: 5079 4548 7562 2063 6f6d 7061 7469 626c  PyEHub compatibl
 00000920: 6520 696e 7075 7473 2e0a 2020 2020 2901  e inputs..    ).
 00000930: da07 636f 6c75 6d6e 7369 80ee 3600 da05  ..columnsi..6...
 00000940: 5661 6c75 6554 2901 da0c 6967 6e6f 7265  ValueT)...ignore
 00000950: 5f69 6e64 6578 2909 da07 746f 5f64 6963  _index)...to_dic
 00000960: 74da 0661 7070 656e 64da 0270 64da 0944  t..append..pd..D
 00000970: 6174 6146 7261 6d65 da08 746f 5f66 7261  ataFrame..to_fra
-00000980: 6d65 7226 0000 00da 026e 70da 0561 7272  mer&.....np..arr
+00000980: 6d65 7228 0000 00da 026e 70da 0561 7272  mer(.....np..arr
 00000990: 6179 da06 636f 6e63 6174 2911 da05 696e  ay..concat)...in
 000009a0: 7075 74da 0a69 6e64 6578 5f73 697a 65da  put..index_size.
 000009b0: 0a69 6e70 7574 5f64 6963 745a 0b63 6f6c  .input_dictZ.col
 000009c0: 756d 6e6e 616d 6573 da01 6a5a 0864 665f  umnnames..jZ.df_
 000009d0: 696e 7075 74da 096f 626a 6563 7469 7665  input..objective
 000009e0: da06 7365 7269 6573 da06 7265 7375 6c74  ..series..result
 000009f0: 5a0b 636f 6c64 5f72 6573 756c 745a 0b77  Z.cold_resultZ.w
@@ -163,25 +163,25 @@
 00000a20: 5a0a 636f 6c64 5f69 6e70 7574 5a0a 7761  Z.cold_inputZ.wa
 00000a30: 726d 5f69 6e70 7574 5a08 7465 6d70 5f64  rm_inputZ.temp_d
 00000a40: 6631 5a08 7465 6d70 5f64 6632 7209 0000  f1Z.temp_df2r...
 00000a50: 0072 0900 0000 720a 0000 00da 0865 705f  .r....r......ep_
 00000a60: 746f 5f65 684c 0000 0073 2c00 0000 0006  to_ehL...s,.....
 00000a70: 0804 0401 0801 0c09 0c02 0801 0c01 1002  ................
 00000a80: 0c04 0801 0801 0801 0801 0801 0802 0601  ................
-00000a90: 0602 1601 1608 1201 1602 7239 0000 0029  ..........r9...)
+00000a90: 0602 1601 1606 1201 1602 723b 0000 0029  ..........r;...)
 00000aa0: 1bda 075f 5f64 6f63 5f5f 7210 0000 00da  ...__doc__r.....
 00000ab0: 0966 756e 6374 6f6f 6c73 7202 0000 00da  .functoolsr.....
 00000ac0: 0674 7970 696e 6772 0300 0000 da05 6e75  .typingr......nu
-00000ad0: 6d70 7972 2f00 0000 da06 7061 6e64 6173  mpyr/.....pandas
-00000ae0: 722c 0000 0072 0d00 0000 7204 0000 005a  r,...r....r....Z
+00000ad0: 6d70 7972 3100 0000 da06 7061 6e64 6173  mpyr1.....pandas
+00000ae0: 722e 0000 0072 0d00 0000 7204 0000 005a  r....r....r....Z
 00000af0: 1c70 7965 6875 622e 656e 6572 6779 5f68  .pyehub.energy_h
 00000b00: 7562 2e65 6875 625f 6d6f 6465 6c72 0500  ub.ehub_modelr..
 00000b10: 0000 da05 6265 736f 7372 0600 0000 da05  ....besosr......
 00000b20: 6669 6c65 73da 0367 6574 da03 7374 7272  files..get..strr
 00000b30: 0b00 0000 720f 0000 0072 1400 0000 7217  ....r....r....r.
-00000b40: 0000 00da 046c 6973 7472 2000 0000 7226  .....listr ...r&
-00000b50: 0000 0072 3900 0000 7209 0000 0072 0900  ...r9...r....r..
+00000b40: 0000 00da 046c 6973 7472 2100 0000 7228  .....listr!...r(
+00000b50: 0000 0072 3b00 0000 7209 0000 0072 0900  ...r;...r....r..
 00000b60: 0000 7209 0000 0072 0a00 0000 da08 3c6d  ..r....r......<m
 00000b70: 6f64 756c 653e 0100 0000 732c 0000 0004  odule>....s,....
 00000b80: 0508 010c 010c 0308 0108 0108 010c 010c  ................
 00000b90: 030c 061a 0408 0808 0608 0602 0102 0102  ................
 00000ba0: fe04 0606 0002 ff0e 0908 0e              ...........
```

### Comparing `besos-2.2.2/besos/__pycache__/sampling.cpython-38.pyc` & `besos-2.2.3/besos/__pycache__/sampling.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/__pycache__/weather.cpython-38.pyc` & `besos-2.2.3/besos/__pycache__/weather.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/besos_utils.py` & `besos-2.2.3/besos/besos_utils.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/config.py` & `besos-2.2.3/besos/config.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/data/Custom_Long_Fields.idd` & `besos-2.2.3/besos/data/Custom_Long_Fields.idd`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/data/Energy+.schema.epJSON` & `besos-2.2.3/besos/data/Energy+.schema.epJSON`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/data/example_bad_idf.idf` & `besos-2.2.3/besos/data/example_bad_idf.idf`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/data/example_building.epJSON` & `besos-2.2.3/besos/data/example_building.epJSON`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/data/example_epw.epw` & `besos-2.2.3/besos/data/example_epw.epw`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/data/example_idd.idd` & `besos-2.2.3/besos/data/example_idd.idd`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/data/example_idf.idf` & `besos-2.2.3/besos/data/example_idf.idf`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/data/example_xlsx.xlsx` & `besos-2.2.3/besos/data/example_xlsx.xlsx`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/data/unexpanded.idf` & `besos-2.2.3/besos/data/unexpanded.idf`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/eplus_funcs.py` & `besos-2.2.3/besos/eplus_funcs.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/eppy_funcs.py` & `besos-2.2.3/besos/eppy_funcs.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/errors.py` & `besos-2.2.3/besos/errors.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/evaluator.py` & `besos-2.2.3/besos/evaluator.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/example_ui.py` & `besos-2.2.3/besos/example_ui.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/objectives.py` & `besos-2.2.3/besos/objectives.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/optimizer.py` & `besos-2.2.3/besos/optimizer.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/parameters.py` & `besos-2.2.3/besos/parameters.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/problem.py` & `besos-2.2.3/besos/problem.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/pyehub_funcs.py` & `besos-2.2.3/besos/pyehub_funcs.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/besos/sampling.py` & `besos-2.2.3/besos/sampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
     :param samples: the number of samples
     :param attributes: number of parameters that are to be varied
     :param level: [in args/kwargs for dist_sampler]
 
     :returns: an array of floats between 0 and 1 to be transformed in dist_sampler
     """
     if level is None:
-        level = np.int(np.exp(np.log(samples) / attributes))
+        level = int(np.exp(np.log(samples) / attributes))
         if (level**attributes) > level:
             print(
                 f"Total number of samples ({level**attributes}) is smaller  than input ({samples}) "
                 f"to have an even number of factor levels ({level}) for all parameters."
             )
     return pyDOE2.fullfact((np.ones([attributes]) * level).astype(int)) / level
```

### Comparing `besos-2.2.2/besos.egg-info/PKG-INFO` & `besos-2.2.3/besos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: besos
-Version: 2.2.2
+Version: 2.2.3
 Summary: A library for Building and Energy Simulation, Optimization and Surrogate-modelling
 Home-page: https://gitlab.com/energyincities/besos
 Author: Ralph Evins
 Author-email: revins@uvic.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `besos-2.2.2/besos.egg-info/SOURCES.txt` & `besos-2.2.3/besos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/setup.py` & `besos-2.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     dev = f.read().splitlines()
 
 complete = complete[1:]  # Remove reference to requirements file
 dev = dev[1:]  # Remove reference to requirement-complete file
 
 setup(
     name="besos",
-    version="2.2.2",
+    version="2.2.3",
     description="A library for Building and Energy Simulation, Optimization and Surrogate-modelling",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Ralph Evins",
     author_email="revins@uvic.ca",
     url="https://gitlab.com/energyincities/besos",
     packages=["besos"],
```

### Comparing `besos-2.2.2/test/test_adaptive_surrogate.py` & `besos-2.2.3/test/test_adaptive_surrogate.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/test/test_eplus_funcs.py` & `besos-2.2.3/test/test_eplus_funcs.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/test/test_eppy_funcs.py` & `besos-2.2.3/test/test_eppy_funcs.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/test/test_error_handling.py` & `besos-2.2.3/test/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/test/test_evaluators.py` & `besos-2.2.3/test/test_evaluators.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/test/test_fit_surrogate.py` & `besos-2.2.3/test/test_fit_surrogate.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/test/test_mixed_optimisation.py` & `besos-2.2.3/test/test_mixed_optimisation.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/test/test_objectives_constraints.py` & `besos-2.2.3/test/test_objectives_constraints.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/test/test_parameter.py` & `besos-2.2.3/test/test_parameter.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/test/test_platypus.py` & `besos-2.2.3/test/test_platypus.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/test/test_rbfopt.py` & `besos-2.2.3/test/test_rbfopt.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/test/test_selectors.py` & `besos-2.2.3/test/test_selectors.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.2/test/test_simulation.py` & `besos-2.2.3/test/test_simulation.py`

 * *Files identical despite different names*

