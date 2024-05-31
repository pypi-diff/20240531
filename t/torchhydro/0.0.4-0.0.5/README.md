# Comparing `tmp/torchhydro-0.0.4.tar.gz` & `tmp/torchhydro-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchhydro-0.0.4.tar", last modified: Wed Nov 29 11:54:49 2023, max compression
+gzip compressed data, was "torchhydro-0.0.5.tar", last modified: Fri May 31 03:37:04 2024, max compression
```

## Comparing `torchhydro-0.0.4.tar` & `torchhydro-0.0.5.tar`

### file list

```diff
@@ -1,63 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-11-29 11:54:49.562348 torchhydro-0.0.4/
--rw-rw-rw-   0        0        0      174 2022-09-09 06:33:14.000000 torchhydro-0.0.4/AUTHORS.rst
--rw-rw-rw-   0        0        0     1538 2022-09-09 06:33:14.000000 torchhydro-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      129 2022-09-09 06:33:14.000000 torchhydro-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3667 2023-11-29 11:54:49.558353 torchhydro-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2195 2023-11-29 11:27:57.000000 torchhydro-0.0.4/README.md
--rw-rw-rw-   0        0        0      339 2023-11-29 11:27:57.000000 torchhydro-0.0.4/requirements.txt
--rw-rw-rw-   0        0        0      481 2023-11-29 11:54:49.571351 torchhydro-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2191 2023-11-29 11:29:23.000000 torchhydro-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-29 11:54:49.241861 torchhydro-0.0.4/tests/
--rw-rw-rw-   0        0        0     2520 2023-11-29 11:27:57.000000 torchhydro-0.0.4/tests/test_caravan_train.py
--rw-rw-rw-   0        0        0     1988 2023-11-29 11:27:57.000000 torchhydro-0.0.4/tests/test_data.py
--rw-rw-rw-   0        0        0     3852 2023-11-29 11:27:57.000000 torchhydro-0.0.4/tests/test_dpl4xaj.py
--rw-rw-rw-   0        0        0     4694 2023-11-29 11:27:57.000000 torchhydro-0.0.4/tests/test_ensemble_exps.py
--rw-rw-rw-   0        0        0     3088 2023-11-29 11:27:57.000000 torchhydro-0.0.4/tests/test_evaluate_model.py
--rw-rw-rw-   0        0        0     2093 2023-11-29 11:27:57.000000 torchhydro-0.0.4/tests/test_federated_learning.py
--rw-rw-rw-   0        0        0     3289 2023-11-29 11:27:57.000000 torchhydro-0.0.4/tests/test_tl_opendata.py
--rw-rw-rw-   0        0        0     2121 2023-11-29 11:27:57.000000 torchhydro-0.0.4/tests/test_train_camels_lstm.py
--rw-rw-rw-   0        0        0     3188 2023-11-29 11:27:57.000000 torchhydro-0.0.4/tests/test_transfer_learning.py
--rw-rw-rw-   0        0        0     1611 2023-11-29 11:27:57.000000 torchhydro-0.0.4/tests/test_weight_analysis.py
-drwxrwxrwx   0        0        0        0 2023-11-29 11:54:49.246860 torchhydro-0.0.4/torchhydro/
--rw-rw-rw-   0        0        0      530 2023-11-29 11:29:23.000000 torchhydro-0.0.4/torchhydro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-29 11:54:49.390404 torchhydro-0.0.4/torchhydro/configs/
--rw-rw-rw-   0        0        0        0 2023-09-24 01:24:43.000000 torchhydro-0.0.4/torchhydro/configs/__init__.py
--rw-rw-rw-   0        0        0    36325 2023-11-29 11:27:57.000000 torchhydro-0.0.4/torchhydro/configs/config.py
--rw-rw-rw-   0        0        0     5078 2023-09-24 01:24:43.000000 torchhydro-0.0.4/torchhydro/configs/model_config.py
-drwxrwxrwx   0        0        0        0 2023-11-29 11:54:49.440940 torchhydro-0.0.4/torchhydro/datasets/
--rw-rw-rw-   0        0        0        0 2022-12-14 07:04:22.000000 torchhydro-0.0.4/torchhydro/datasets/__init__.py
--rw-rw-rw-   0        0        0      804 2023-11-29 11:27:57.000000 torchhydro-0.0.4/torchhydro/datasets/data_dict.py
--rw-rw-rw-   0        0        0    15531 2023-11-29 11:27:57.000000 torchhydro-0.0.4/torchhydro/datasets/data_scalers.py
--rw-rw-rw-   0        0        0    16117 2023-11-29 11:27:57.000000 torchhydro-0.0.4/torchhydro/datasets/data_sets.py
--rw-rw-rw-   0        0        0    20948 2023-11-29 11:27:57.000000 torchhydro-0.0.4/torchhydro/datasets/data_sources.py
--rw-rw-rw-   0        0        0    13347 2023-11-29 11:27:57.000000 torchhydro-0.0.4/torchhydro/datasets/data_utils.py
--rw-rw-rw-   0        0        0     4325 2023-11-29 11:27:57.000000 torchhydro-0.0.4/torchhydro/datasets/sampler.py
-drwxrwxrwx   0        0        0        0 2023-11-29 11:54:49.452937 torchhydro-0.0.4/torchhydro/explainers/
--rw-rw-rw-   0        0        0        0 2023-11-29 11:27:57.000000 torchhydro-0.0.4/torchhydro/explainers/__init__.py
--rw-rw-rw-   0        0        0     6594 2023-11-29 11:27:57.000000 torchhydro-0.0.4/torchhydro/explainers/shap.py
--rw-rw-rw-   0        0        0     8967 2023-11-29 11:27:57.000000 torchhydro-0.0.4/torchhydro/explainers/weight_anlysis.py
-drwxrwxrwx   0        0        0        0 2023-11-29 11:54:49.513946 torchhydro-0.0.4/torchhydro/models/
--rw-rw-rw-   0        0        0      243 2023-09-24 01:24:43.000000 torchhydro-0.0.4/torchhydro/models/__init__.py
--rw-rw-rw-   0        0        0     3500 2023-11-29 11:27:57.000000 torchhydro-0.0.4/torchhydro/models/ann.py
--rw-rw-rw-   0        0        0    28481 2023-09-24 01:24:43.000000 torchhydro-0.0.4/torchhydro/models/crits.py
--rw-rw-rw-   0        0        0    19625 2023-11-29 11:27:57.000000 torchhydro-0.0.4/torchhydro/models/cudnnlstm.py
--rw-rw-rw-   0        0        0    40718 2023-11-29 11:27:57.000000 torchhydro-0.0.4/torchhydro/models/dpl4xaj.py
--rw-rw-rw-   0        0        0     1455 2023-11-29 11:27:57.000000 torchhydro-0.0.4/torchhydro/models/dropout.py
--rw-rw-rw-   0        0        0     4667 2023-10-06 11:30:22.000000 torchhydro-0.0.4/torchhydro/models/kernel_conv.py
--rw-rw-rw-   0        0        0     1621 2023-11-29 11:27:57.000000 torchhydro-0.0.4/torchhydro/models/model_dict_function.py
--rw-rw-rw-   0        0        0     1067 2023-09-24 01:24:43.000000 torchhydro-0.0.4/torchhydro/models/model_utils.py
--rw-rw-rw-   0        0        0     3595 2023-11-29 11:27:57.000000 torchhydro-0.0.4/torchhydro/models/simple_lstm.py
-drwxrwxrwx   0        0        0        0 2023-11-29 11:54:49.538955 torchhydro-0.0.4/torchhydro/trainers/
--rw-rw-rw-   0        0        0        0 2022-09-11 14:23:56.000000 torchhydro-0.0.4/torchhydro/trainers/__init__.py
--rw-rw-rw-   0        0        0    28623 2023-11-29 11:27:57.000000 torchhydro-0.0.4/torchhydro/trainers/deep_hydro.py
--rw-rw-rw-   0        0        0     6226 2023-11-29 11:27:57.000000 torchhydro-0.0.4/torchhydro/trainers/train_logger.py
--rw-rw-rw-   0        0        0    11475 2023-11-29 11:27:57.000000 torchhydro-0.0.4/torchhydro/trainers/train_utils.py
--rw-rw-rw-   0        0        0    16112 2023-11-29 11:27:57.000000 torchhydro-0.0.4/torchhydro/trainers/trainer.py
-drwxrwxrwx   0        0        0        0 2023-11-29 11:54:49.547356 torchhydro-0.0.4/torchhydro.egg-info/
--rw-rw-rw-   0        0        0     3667 2023-11-29 11:54:48.000000 torchhydro-0.0.4/torchhydro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1531 2023-11-29 11:54:48.000000 torchhydro-0.0.4/torchhydro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      317 2023-11-29 11:54:48.000000 torchhydro-0.0.4/torchhydro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-11-29 11:54:48.000000 torchhydro-0.0.4/torchhydro.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-11-29 11:54:48.000000 torchhydro-0.0.4/torchhydro.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      314 2023-11-29 11:54:48.000000 torchhydro-0.0.4/torchhydro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-11-29 11:54:48.000000 torchhydro-0.0.4/torchhydro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:37:04.735306 torchhydro-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-31 03:36:54.000000 torchhydro-0.0.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-31 03:36:54.000000 torchhydro-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-31 03:36:54.000000 torchhydro-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-05-31 03:37:04.735306 torchhydro-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-31 03:36:54.000000 torchhydro-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-31 03:36:54.000000 torchhydro-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-31 03:37:04.735306 torchhydro-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-31 03:36:54.000000 torchhydro-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:37:04.727306 torchhydro-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-31 03:36:54.000000 torchhydro-0.0.5/tests/test_caravan_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-31 03:36:54.000000 torchhydro-0.0.5/tests/test_data_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-31 03:36:54.000000 torchhydro-0.0.5/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-05-31 03:36:54.000000 torchhydro-0.0.5/tests/test_deep_hydro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-31 03:36:54.000000 torchhydro-0.0.5/tests/test_dpl4xaj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-31 03:36:54.000000 torchhydro-0.0.5/tests/test_ensemble_exps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-31 03:36:54.000000 torchhydro-0.0.5/tests/test_evaluate_grid_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-31 03:36:54.000000 torchhydro-0.0.5/tests/test_evaluate_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-31 03:36:54.000000 torchhydro-0.0.5/tests/test_evaluate_seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-31 03:36:54.000000 torchhydro-0.0.5/tests/test_federated_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-31 03:36:54.000000 torchhydro-0.0.5/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-31 03:36:54.000000 torchhydro-0.0.5/tests/test_pretrain_dataenhanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-31 03:36:54.000000 torchhydro-0.0.5/tests/test_pretrain_datafusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-31 03:36:54.000000 torchhydro-0.0.5/tests/test_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-31 03:36:54.000000 torchhydro-0.0.5/tests/test_tl_selfmadedata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-31 03:36:54.000000 torchhydro-0.0.5/tests/test_train_camels_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-31 03:36:54.000000 torchhydro-0.0.5/tests/test_train_camelspro_mtl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-31 03:36:54.000000 torchhydro-0.0.5/tests/test_train_grid_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-31 03:36:54.000000 torchhydro-0.0.5/tests/test_train_mean_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-05-31 03:36:54.000000 torchhydro-0.0.5/tests/test_train_seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-31 03:36:54.000000 torchhydro-0.0.5/tests/test_train_with_gpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-31 03:36:54.000000 torchhydro-0.0.5/tests/test_transfer_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-31 03:36:54.000000 torchhydro-0.0.5/tests/test_weight_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:37:04.727306 torchhydro-0.0.5/torchhydro/
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:37:04.727306 torchhydro-0.0.5/torchhydro/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38260 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/configs/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/configs/model_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:37:04.731306 torchhydro-0.0.5/torchhydro/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/datasets/data_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16947 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/datasets/data_scalers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28930 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/datasets/data_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24931 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/datasets/data_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11103 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/datasets/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/datasets/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:37:04.731306 torchhydro-0.0.5/torchhydro/explainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/explainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/explainers/shap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8678 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/explainers/weight_anlysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:37:04.731306 torchhydro-0.0.5/torchhydro/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/models/ann.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28654 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/models/crits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21133 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/models/cudnnlstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39634 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/models/dpl4xaj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/models/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/models/kernel_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/models/model_dict_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/models/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/models/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/models/simple_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11185 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/models/spplstm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:37:04.735306 torchhydro-0.0.5/torchhydro/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37228 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/trainers/deep_hydro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11302 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/trainers/resulter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/trainers/train_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14223 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/trainers/train_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7980 2024-05-31 03:36:54.000000 torchhydro-0.0.5/torchhydro/trainers/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:37:04.735306 torchhydro-0.0.5/torchhydro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-05-31 03:37:04.000000 torchhydro-0.0.5/torchhydro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-31 03:37:04.000000 torchhydro-0.0.5/torchhydro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-31 03:37:04.000000 torchhydro-0.0.5/torchhydro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-31 03:37:04.000000 torchhydro-0.0.5/torchhydro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 03:37:04.000000 torchhydro-0.0.5/torchhydro.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-31 03:37:04.000000 torchhydro-0.0.5/torchhydro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 03:37:04.000000 torchhydro-0.0.5/torchhydro.egg-info/top_level.txt
```

### Comparing `torchhydro-0.0.4/LICENSE` & `torchhydro-0.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-
-
-BSD License
-
-Copyright (c) 2022, Wenyu Ouyang
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without modification,
-are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice, this
-  list of conditions and the following disclaimer in the documentation and/or
-  other materials provided with the distribution.
-
-* Neither the name of the copyright holder nor the names of its
-  contributors may be used to endorse or promote products derived from this
-  software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
-IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
-INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
-BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
-OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
-OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED
-OF THE POSSIBILITY OF SUCH DAMAGE.
-
+
+
+BSD License
+
+Copyright (c) 2022, Wenyu Ouyang
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without modification,
+are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice, this
+  list of conditions and the following disclaimer in the documentation and/or
+  other materials provided with the distribution.
+
+* Neither the name of the copyright holder nor the names of its
+  contributors may be used to endorse or promote products derived from this
+  software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
+IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
+INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
+BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
+OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
+OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED
+OF THE POSSIBILITY OF SUCH DAMAGE.
+
```

### Comparing `torchhydro-0.0.4/setup.py` & `torchhydro-0.0.5/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-#!/usr/bin/env python
-
-"""
-Author: Wenyu Ouyang
-Date: 2023-07-31 08:40:43
-LastEditTime: 2023-09-18 16:11:57
-LastEditors: Wenyu Ouyang
-Description: The setup script
-FilePath: /torchhydro/setup.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-import io
-from os import path as op
-from setuptools import setup, find_packages
-
-with open("README.md") as readme_file:
-    readme = readme_file.read()
-
-here = op.abspath(op.dirname(__file__))
-
-# get the dependencies and installs
-with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
-    all_reqs = f.read().split("\n")
-
-install_requires = [x.strip() for x in all_reqs if "git+" not in x]
-dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
-
-requirements = []
-
-setup_requirements = [
-    "pytest-runner",
-]
-
-test_requirements = [
-    "pytest>=3",
-]
-
-setup(
-    author="Wenyu Ouyang",
-    author_email="wenyuouyang@outlook.com",
-    python_requires=">=3.8",
-    classifiers=[
-        "Development Status :: 2 - Pre-Alpha",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: BSD License",
-        "Natural Language :: English",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-    ],
-    description="datasets, samplers, transforms, and pre-trained models for hydrology and water resources",
-    entry_points={
-        "console_scripts": [
-            "torchhydro=torchhydro.cli:main",
-        ],
-    },
-    install_requires=install_requires,
-    dependency_links=dependency_links,
-    license="BSD license",
-    long_description=readme,
-    long_description_content_type="text/markdown",
-    include_package_data=True,
-    keywords="torchhydro",
-    name="torchhydro",
-    packages=find_packages(include=["torchhydro", "torchhydro.*"]),
-    setup_requires=setup_requirements,
-    test_suite="tests",
-    tests_require=test_requirements,
-    url="https://github.com/OuyangWenyu/torchhydro",
-    version='0.0.4',
-    zip_safe=False,
-)
+#!/usr/bin/env python
+
+"""
+Author: Wenyu Ouyang
+Date: 2023-07-31 08:40:43
+LastEditTime: 2024-05-31 11:34:36
+LastEditors: Wenyu Ouyang
+Description: The setup script
+FilePath: \torchhydro\setup.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+import io
+from os import path as op
+from setuptools import setup, find_packages
+
+with open("README.md", "r", encoding="utf-8") as readme_file:
+    readme = readme_file.read()
+
+here = op.abspath(op.dirname(__file__))
+
+# get the dependencies and installs
+with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
+    all_reqs = f.read().split("\n")
+
+install_requires = [x.strip() for x in all_reqs if "git+" not in x]
+dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
+
+requirements = []
+
+setup_requirements = [
+    "pytest-runner",
+]
+
+test_requirements = [
+    "pytest>=3",
+]
+
+setup(
+    author="Wenyu Ouyang",
+    author_email="wenyuouyang@outlook.com",
+    python_requires=">=3.8",
+    classifiers=[
+        "Development Status :: 2 - Pre-Alpha",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: BSD License",
+        "Natural Language :: English",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+    ],
+    description="datasets, samplers, transforms, and pre-trained models for hydrology and water resources",
+    entry_points={
+        "console_scripts": [
+            "torchhydro=torchhydro.cli:main",
+        ],
+    },
+    install_requires=install_requires,
+    dependency_links=dependency_links,
+    license="BSD license",
+    long_description=readme,
+    long_description_content_type="text/markdown",
+    include_package_data=True,
+    keywords="torchhydro",
+    name="torchhydro",
+    packages=find_packages(include=["torchhydro", "torchhydro.*"]),
+    setup_requires=setup_requirements,
+    test_suite="tests",
+    tests_require=test_requirements,
+    url="https://github.com/OuyangWenyu/torchhydro",
+    version='0.0.5',
+    zip_safe=False,
+)
```

### Comparing `torchhydro-0.0.4/tests/test_caravan_train.py` & `torchhydro-0.0.5/tests/test_caravan_train.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,91 @@
-"""
-Author: Wenyu Ouyang
-Date: 2023-07-25 16:47:19
-LastEditTime: 2023-10-18 15:58:42
-LastEditors: Wenyu Ouyang
-Description: Test a full training and evaluating process
-FilePath: \torchhydro\tests\test_caravan_train.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-import os
-import pytest
-import hydrodataset as hds
-from torchhydro.configs.config import cmd, default_config_file, update_cfg
-from torchhydro.trainers.trainer import train_and_evaluate
-
-
-@pytest.fixture()
-def var_c():
-    return ["area", "p_mean", "pet_mean", "aridity", "frac_snow", "moisture_index"]
-
-
-@pytest.fixture()
-def var_t():
-    return [
-        "surface_net_solar_radiation_mean",
-        "total_precipitation_sum",
-        "potential_evaporation_sum",
-        "temperature_2m_max",
-        "temperature_2m_min",
-        "surface_pressure_mean",
-    ]
-
-
-@pytest.fixture()
-def config(var_c, var_t):
-    project_name = "test_caravan/exp5"
-    config_data = default_config_file()
-    args = cmd(
-        sub=project_name,
-        source="Caravan",
-        source_path=os.path.join(hds.ROOT_DIR, "caravan"),
-        source_region="Global",
-        download=0,
-        ctx=[-1],
-        model_name="CpuLSTM",
-        model_hyperparam={
-            "n_input_features": len(var_t) + len(var_c),
-            "n_output_features": 1,
-            "n_hidden_states": 256,
-        },
-        gage_id=[
-            "camels_01022500",
-            "camels_01031500",
-            "camels_01047000",
-            "camels_01052500",
-            "camels_01054200",
-            "camels_01055000",
-            "camels_01057000",
-            "camelsaus_102101A",
-            "camelsaus_108003A",
-            "hysets_06444000",
-        ],
-        batch_size=8,
-        rho=20,
-        var_t=var_t,
-        var_c=var_c,
-        var_out=["streamflow"],
-        dataset="StreamflowDataset",
-        sampler="KuaiSampler",
-        scaler="DapengScaler",
-        train_epoch=2,
-        save_epoch=1,
-        te=2,
-        train_period=["2000-10-01", "2001-10-01"],
-        valid_period=["2001-10-01", "2002-10-01"],
-        test_period=["2002-10-01", "2003-10-01"],
-        loss_func="RMSESum",
-        opt="Adam",
-        # key is epoch, start from 1
-        lr_scheduler={1: 1e-2, 2: 5e-3, 3: 1e-3},
-        which_first_tensor="sequence",
-    )
-    update_cfg(config_data, args)
-    return config_data
-
-
-def test_train_evaluate(config):
-    train_and_evaluate(config)
+"""
+Author: Wenyu Ouyang
+Date: 2023-07-25 16:47:19
+LastEditTime: 2024-05-27 16:22:15
+LastEditors: Wenyu Ouyang
+Description: Test a full training and evaluating process
+FilePath: \torchhydro\tests\test_caravan_train.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+
+import os
+import pytest
+from torchhydro import SETTING
+from torchhydro.configs.config import cmd, default_config_file, update_cfg
+from torchhydro.trainers.trainer import train_and_evaluate
+
+
+@pytest.fixture()
+def var_c():
+    return ["area", "p_mean", "pet_mean", "aridity", "frac_snow", "moisture_index"]
+
+
+@pytest.fixture()
+def var_t():
+    return [
+        "surface_net_solar_radiation_mean",
+        "total_precipitation_sum",
+        "potential_evaporation_sum",
+        "temperature_2m_max",
+        "temperature_2m_min",
+        "surface_pressure_mean",
+    ]
+
+
+@pytest.fixture()
+def config(var_c, var_t):
+    project_name = "test_caravan/exp5"
+    config_data = default_config_file()
+    args = cmd(
+        sub=project_name,
+        source="Caravan",
+        source_path=os.path.join(
+            SETTING["local_data_path"]["datasets-origin"], "caravan"
+        ),
+        source_region="Global",
+        ctx=[-1],
+        model_name="CpuLSTM",
+        model_hyperparam={
+            "n_input_features": len(var_t) + len(var_c),
+            "n_output_features": 1,
+            "n_hidden_states": 256,
+        },
+        gage_id=[
+            "camels_01022500",
+            "camels_01031500",
+            "camels_01047000",
+            "camels_01052500",
+            "camels_01054200",
+            "camels_01055000",
+            "camels_01057000",
+            "camelsaus_102101A",
+            "camelsaus_108003A",
+            "hysets_06444000",
+        ],
+        batch_size=8,
+        forecast_history=0,
+        forecast_length=20,
+        var_t=var_t,
+        var_c=var_c,
+        var_out=["streamflow"],
+        dataset="StreamflowDataset",
+        sampler="KuaiSampler",
+        scaler="DapengScaler",
+        train_epoch=2,
+        save_epoch=1,
+        te=2,
+        train_period=["2000-10-01", "2001-10-01"],
+        valid_period=["2001-10-01", "2002-10-01"],
+        test_period=["2002-10-01", "2003-10-01"],
+        loss_func="RMSESum",
+        opt="Adam",
+        # key is epoch, start from 1
+        lr_scheduler={1: 1e-2, 2: 5e-3, 3: 1e-3},
+        which_first_tensor="sequence",
+    )
+    update_cfg(config_data, args)
+    return config_data
+
+
+def test_train_evaluate(config):
+    train_and_evaluate(config)
```

### Comparing `torchhydro-0.0.4/tests/test_dpl4xaj.py` & `torchhydro-0.0.5/tests/test_dpl4xaj.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-import numpy as np
-import pytest
-
-import torch
-
-from torchhydro.models.dpl4xaj import DplLstmXaj
-from torchhydro.models.kernel_conv import uh_conv, uh_gamma
-
-
-@pytest.fixture()
-def device():
-    return "cuda:0" if torch.cuda.is_available() else "cpu"
-
-
-@pytest.fixture()
-def dpl(device):
-    dpl_ = DplLstmXaj(5, 15, 64, kernel_size=15, warmup_length=5)
-    return dpl_.to(device)
-
-
-@pytest.fixture()
-def dpl_eh(device):
-    dpl_ = DplLstmXaj(
-        5,
-        15,
-        64,
-        kernel_size=15,
-        warmup_length=5,
-        source_book="EH",
-        source_type="sources",
-    )
-    return dpl_.to(device)
-
-
-@pytest.fixture()
-def dpl_eh5mm(device):
-    dpl_ = DplLstmXaj(
-        5,
-        15,
-        64,
-        kernel_size=15,
-        warmup_length=5,
-        source_book="EH",
-        source_type="sources5mm",
-    )
-    return dpl_.to(device)
-
-
-def test_dpl_lstm_xaj(device, dpl):
-    # sequence-first tensor: time_sequence, batch, feature_size (assume that they are p, pet, srad, tmax, tmin)
-    x = torch.rand(20, 10, 5).to(device)
-    z = torch.rand(20, 10, 5).to(device)
-    q = dpl(x, z)
-    assert len(q.shape) == 3
-    assert q.shape == (15, 10, 1)
-    q.backward(torch.ones_like(q))
-    assert type(q) == torch.Tensor
-
-
-def test_dpl_lstm_xaj_eh(device, dpl_eh):
-    # sequence-first tensor: time_sequence, batch, feature_size (assume that they are p, pet, srad, tmax, tmin)
-    x = torch.rand(20, 10, 5).to(device)
-    z = torch.rand(20, 10, 5).to(device)
-    q = dpl_eh(x, z)
-    assert len(q.shape) == 3
-    assert q.shape == (15, 10, 1)
-    q.backward(torch.ones_like(q))
-    assert type(q) == torch.Tensor
-
-
-def test_dpl_lstm_xaj_eh5mm(device, dpl_eh5mm):
-    # sequence-first tensor: time_sequence, batch, feature_size (assume that they are p, pet, srad, tmax, tmin)
-    x = torch.rand(20, 10, 5).to(device)
-    z = torch.rand(20, 10, 5).to(device)
-    q = dpl_eh5mm(x, z)
-    assert len(q.shape) == 3
-    assert q.shape == (15, 10, 1)
-    q.backward(torch.ones_like(q))
-    assert type(q) == torch.Tensor
-
-
-def test_uh_gamma():
-    # batch = 10
-    tempa = torch.Tensor(np.full(10, [2.5]))
-    tempb = torch.Tensor(np.full(10, [3.5]))
-    # repeat for 20 periods and add one dim as feature: time_seq, batch, feature
-    routa = tempa.repeat(20, 1).unsqueeze(-1)
-    routb = tempb.repeat(20, 1).unsqueeze(-1)
-    uh = uh_gamma(routa, routb, len_uh=15)
-    np.testing.assert_almost_equal(
-        uh.numpy()[:, 0, :],
-        np.array(
-            [
-                [0.0069],
-                [0.0314],
-                [0.0553],
-                [0.0738],
-                [0.0860],
-                [0.0923],
-                [0.0939],
-                [0.0919],
-                [0.0875],
-                [0.0814],
-                [0.0744],
-                [0.0670],
-                [0.0597],
-                [0.0525],
-                [0.0459],
-            ]
-        ),
-        decimal=3,
-    )
-
-
-def test_uh():
-    uh_from_gamma = torch.full((5, 3, 1), 1.0)
-    # uh_from_gamma = torch.Tensor(np.arange(15).reshape(5, 3, 1))
-    rf = torch.Tensor(np.arange(30).reshape(10, 3, 1) / 100)
-    qs = uh_conv(rf, uh_from_gamma)
-    np.testing.assert_almost_equal(
-        np.array(
-            [
-                [0.0000, 0.0100, 0.0200],
-                [0.0300, 0.0500, 0.0700],
-                [0.0900, 0.1200, 0.1500],
-                [0.1800, 0.2200, 0.2600],
-                [0.3000, 0.3500, 0.4000],
-                [0.4500, 0.5000, 0.5500],
-                [0.6000, 0.6500, 0.7000],
-                [0.7500, 0.8000, 0.8500],
-                [0.9000, 0.9500, 1.0000],
-                [1.0500, 1.1000, 1.1500],
-            ]
-        ),
-        qs.numpy()[:, :, 0],
-        decimal=3,
-    )
+import numpy as np
+import pytest
+
+import torch
+
+from torchhydro.models.dpl4xaj import DplLstmXaj
+from torchhydro.models.kernel_conv import uh_conv, uh_gamma
+
+
+@pytest.fixture()
+def device():
+    return "cuda:0" if torch.cuda.is_available() else "cpu"
+
+
+@pytest.fixture()
+def dpl(device):
+    dpl_ = DplLstmXaj(5, 15, 64, kernel_size=15, warmup_length=5)
+    return dpl_.to(device)
+
+
+@pytest.fixture()
+def dpl_eh(device):
+    dpl_ = DplLstmXaj(
+        5,
+        15,
+        64,
+        kernel_size=15,
+        warmup_length=5,
+        source_book="EH",
+        source_type="sources",
+    )
+    return dpl_.to(device)
+
+
+@pytest.fixture()
+def dpl_eh5mm(device):
+    dpl_ = DplLstmXaj(
+        5,
+        15,
+        64,
+        kernel_size=15,
+        warmup_length=5,
+        source_book="EH",
+        source_type="sources5mm",
+    )
+    return dpl_.to(device)
+
+
+def test_dpl_lstm_xaj(device, dpl):
+    # sequence-first tensor: time_sequence, batch, feature_size (assume that they are p, pet, srad, tmax, tmin)
+    x = torch.rand(20, 10, 5).to(device)
+    z = torch.rand(20, 10, 5).to(device)
+    q = dpl(x, z)
+    assert len(q.shape) == 3
+    assert q.shape == (15, 10, 1)
+    q.backward(torch.ones_like(q))
+    assert type(q) == torch.Tensor
+
+
+def test_dpl_lstm_xaj_eh(device, dpl_eh):
+    # sequence-first tensor: time_sequence, batch, feature_size (assume that they are p, pet, srad, tmax, tmin)
+    x = torch.rand(20, 10, 5).to(device)
+    z = torch.rand(20, 10, 5).to(device)
+    q = dpl_eh(x, z)
+    assert len(q.shape) == 3
+    assert q.shape == (15, 10, 1)
+    q.backward(torch.ones_like(q))
+    assert type(q) == torch.Tensor
+
+
+def test_dpl_lstm_xaj_eh5mm(device, dpl_eh5mm):
+    # sequence-first tensor: time_sequence, batch, feature_size (assume that they are p, pet, srad, tmax, tmin)
+    x = torch.rand(20, 10, 5).to(device)
+    z = torch.rand(20, 10, 5).to(device)
+    q = dpl_eh5mm(x, z)
+    assert len(q.shape) == 3
+    assert q.shape == (15, 10, 1)
+    q.backward(torch.ones_like(q))
+    assert type(q) == torch.Tensor
+
+
+def test_uh_gamma():
+    # batch = 10
+    tempa = torch.Tensor(np.full(10, [2.5]))
+    tempb = torch.Tensor(np.full(10, [3.5]))
+    # repeat for 20 periods and add one dim as feature: time_seq, batch, feature
+    routa = tempa.repeat(20, 1).unsqueeze(-1)
+    routb = tempb.repeat(20, 1).unsqueeze(-1)
+    uh = uh_gamma(routa, routb, len_uh=15)
+    np.testing.assert_almost_equal(
+        uh.numpy()[:, 0, :],
+        np.array(
+            [
+                [0.0069],
+                [0.0314],
+                [0.0553],
+                [0.0738],
+                [0.0860],
+                [0.0923],
+                [0.0939],
+                [0.0919],
+                [0.0875],
+                [0.0814],
+                [0.0744],
+                [0.0670],
+                [0.0597],
+                [0.0525],
+                [0.0459],
+            ]
+        ),
+        decimal=3,
+    )
+
+
+def test_uh():
+    uh_from_gamma = torch.full((5, 3, 1), 1.0)
+    # uh_from_gamma = torch.Tensor(np.arange(15).reshape(5, 3, 1))
+    rf = torch.Tensor(np.arange(30).reshape(10, 3, 1) / 100)
+    qs = uh_conv(rf, uh_from_gamma)
+    np.testing.assert_almost_equal(
+        np.array(
+            [
+                [0.0000, 0.0100, 0.0200],
+                [0.0300, 0.0500, 0.0700],
+                [0.0900, 0.1200, 0.1500],
+                [0.1800, 0.2200, 0.2600],
+                [0.3000, 0.3500, 0.4000],
+                [0.4500, 0.5000, 0.5500],
+                [0.6000, 0.6500, 0.7000],
+                [0.7500, 0.8000, 0.8500],
+                [0.9000, 0.9500, 1.0000],
+                [1.0500, 1.1000, 1.1500],
+            ]
+        ),
+        qs.numpy()[:, :, 0],
+        decimal=3,
+    )
```

### Comparing `torchhydro-0.0.4/tests/test_ensemble_exps.py` & `torchhydro-0.0.5/tests/test_ensemble_exps.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,171 +1,172 @@
-import pytest
-import os
-import hydrodataset as hds
-from hydroutils import hydro_file
-from torchhydro.configs.config import cmd, default_config_file, update_cfg
-from torchhydro.trainers.trainer import ensemble_train_and_evaluate
-
-
-@pytest.fixture()
-def var_c_target():
-    return [
-        "p_mean",
-        "pet_mean",
-        "Area",
-        "geol_class_1st",
-        "elev",
-        "SNDPPT",
-    ]
-
-
-@pytest.fixture()
-def var_c_source():
-    return [
-        "elev_mean",
-        "slope_mean",
-        "area_gages2",
-        "frac_forest",
-        "lai_max",
-        "lai_diff",
-        "dom_land_cover_frac",
-        "dom_land_cover",
-        "root_depth_50",
-        "soil_depth_statsgo",
-        "soil_porosity",
-        "soil_conductivity",
-        "max_water_content",
-        "geol_1st_class",
-        "geol_2nd_class",
-        "geol_porostiy",
-        "geol_permeability",
-    ]
-
-
-@pytest.fixture()
-def var_t_target():
-    # mainly from ERA5LAND
-    return ["total_precipitation", "potential_evaporation", "temperature_2m"]
-
-
-@pytest.fixture()
-def var_t_source():
-    return ["dayl", "prcp", "srad", "tmax", "tmin", "vp"]
-
-
-@pytest.fixture()
-def gage_id():
-    return [
-        "61561",
-    ]
-
-
-def test_run_lstm_cross_val(var_c_target, var_t_target, gage_id):
-    config = default_config_file()
-    project_name = "test_camels/expcccv61561"
-    kfold = 2
-    train_period = ["2018-10-01", "2021-10-01"]
-    valid_period = ["2015-10-01", "2018-10-01"]
-    args = cmd(
-        sub=project_name,
-        source="SelfMadeCAMELS",
-        source_path=os.path.join(
-            hds.ROOT_DIR, "waterism", "datasets-interim", "camels_cc"
-        ),
-        download=0,
-        ctx=[0],
-        model_name="KuaiLSTM",
-        model_hyperparam={
-            "n_input_features": len(var_c_target) + len(var_t_target),
-            "n_output_features": 1,
-            "n_hidden_states": 256,
-        },
-        opt="Adadelta",
-        # opt_param=opt_param,
-        loss_func="RMSESum",
-        train_period=train_period,
-        test_period=valid_period,
-        batch_size=20,
-        rho=365,
-        scaler="DapengScaler",
-        dataset="StreamflowDataset",
-        continue_train=True,
-        warmup_length=0,
-        train_epoch=10,
-        te=10,
-        var_t=var_t_target,
-        var_t_type="era5land",
-        var_c=var_c_target,
-        var_out=["streamflow"],
-        gage_id=gage_id,
-        ensemble=True,
-        ensemble_items={
-            "kfold": kfold,
-            "batch_sizes": [20, 50],
-        },
-    )
-    update_cfg(config, args)
-    ensemble_train_and_evaluate(config)
-    print("All processes are finished!")
-
-
-def test_run_cross_val_tlcamelsus2cc(
-    var_c_source, var_c_target, var_t_source, var_t_target, gage_id
-):
-    weight_dir = os.path.join(
-        os.getcwd(),
-        "results",
-        "test_camels",
-        "exp1",
-    )
-    weight_path = hydro_file.get_lastest_file_in_a_dir(weight_dir)
-    project_name = "test_camels/exptl4cccv61561"
-    train_period = ["2018-10-01", "2021-10-01"]
-    valid_period = ["2015-10-01", "2018-10-01"]
-    args = cmd(
-        sub=project_name,
-        source="SelfMadeCAMELS",
-        # cc means China continent
-        source_path=os.path.join(
-            hds.ROOT_DIR, "waterism", "datasets-interim", "camels_cc"
-        ),
-        download=0,
-        ctx=[0],
-        model_type="TransLearn",
-        model_name="KaiLSTM",
-        model_hyperparam={
-            "linear_size": len(var_c_target) + len(var_t_target),
-            "n_input_features": len(var_c_source) + len(var_t_source),
-            "n_output_features": 1,
-            "n_hidden_states": 256,
-        },
-        opt="Adadelta",
-        loss_func="RMSESum",
-        batch_size=5,
-        rho=20,
-        rs=1234,
-        train_period=train_period,
-        test_period=valid_period,
-        scaler="DapengScaler",
-        # sampler="KuaiSampler",
-        dataset="StreamflowDataset",
-        weight_path=weight_path,
-        weight_path_add={
-            "freeze_params": ["lstm.b_hh", "lstm.b_ih", "lstm.w_hh", "lstm.w_ih"]
-        },
-        continue_train=True,
-        train_epoch=10,
-        te=10,
-        var_t=var_t_target,
-        var_c=var_c_target,
-        var_out=["streamflow"],
-        gage_id=gage_id,
-        ensemble=True,
-        ensemble_items={
-            "kfold": 2,
-            "batch_sizes": [20, 50],
-        },
-    )
-    cfg = default_config_file()
-    update_cfg(cfg, args)
-    ensemble_train_and_evaluate(cfg)
-    print("All processes are finished!")
+import pytest
+import os
+from hydroutils import hydro_file
+
+from torchhydro import SETTING
+from torchhydro.configs.config import cmd, default_config_file, update_cfg
+from torchhydro.trainers.trainer import ensemble_train_and_evaluate
+
+
+@pytest.fixture()
+def var_c_target():
+    return [
+        "p_mean",
+        "pet_mean",
+        "Area",
+        "geol_class_1st",
+        "elev",
+        "SNDPPT",
+    ]
+
+
+@pytest.fixture()
+def var_c_source():
+    return [
+        "elev_mean",
+        "slope_mean",
+        "area_gages2",
+        "frac_forest",
+        "lai_max",
+        "lai_diff",
+        "dom_land_cover_frac",
+        "dom_land_cover",
+        "root_depth_50",
+        "soil_depth_statsgo",
+        "soil_porosity",
+        "soil_conductivity",
+        "max_water_content",
+        "geol_1st_class",
+        "geol_2nd_class",
+        "geol_porostiy",
+        "geol_permeability",
+    ]
+
+
+@pytest.fixture()
+def var_t_target():
+    # mainly from ERA5LAND
+    return ["total_precipitation", "potential_evaporation", "temperature_2m"]
+
+
+@pytest.fixture()
+def var_t_source():
+    return ["dayl", "prcp", "srad", "tmax", "tmin", "vp"]
+
+
+@pytest.fixture()
+def gage_id():
+    return [
+        "61561",
+    ]
+
+
+def test_run_lstm_cross_val(var_c_target, var_t_target, gage_id):
+    config = default_config_file()
+    project_name = "test_camels/expcccv61561"
+    kfold = 2
+    train_period = ["2018-10-01", "2021-10-01"]
+    valid_period = ["2015-10-01", "2018-10-01"]
+    args = cmd(
+        sub=project_name,
+        source="SelfMadeCAMELS",
+        source_path=os.path.join(
+            SETTING["local_data_path"]["datasets-interim"], "camels_cc"
+        ),
+        ctx=[0],
+        model_name="KuaiLSTM",
+        model_hyperparam={
+            "n_input_features": len(var_c_target) + len(var_t_target),
+            "n_output_features": 1,
+            "n_hidden_states": 256,
+        },
+        opt="Adadelta",
+        # opt_param=opt_param,
+        loss_func="RMSESum",
+        train_period=train_period,
+        test_period=valid_period,
+        batch_size=20,
+        forecast_history=0,
+        forecast_length=365,
+        scaler="DapengScaler",
+        dataset="StreamflowDataset",
+        continue_train=True,
+        warmup_length=0,
+        train_epoch=10,
+        te=10,
+        var_t=var_t_target,
+        var_t_type="era5land",
+        var_c=var_c_target,
+        var_out=["streamflow"],
+        gage_id=gage_id,
+        ensemble=True,
+        ensemble_items={
+            "kfold": kfold,
+            "batch_sizes": [20, 50],
+        },
+    )
+    update_cfg(config, args)
+    ensemble_train_and_evaluate(config)
+    print("All processes are finished!")
+
+
+def test_run_cross_val_tlcamelsus2cc(
+    var_c_source, var_c_target, var_t_source, var_t_target, gage_id
+):
+    weight_dir = os.path.join(
+        os.getcwd(),
+        "results",
+        "test_camels",
+        "exp1",
+    )
+    weight_path = hydro_file.get_lastest_file_in_a_dir(weight_dir)
+    project_name = "test_camels/exptl4cccv61561"
+    train_period = ["2018-10-01", "2021-10-01"]
+    valid_period = ["2015-10-01", "2018-10-01"]
+    args = cmd(
+        sub=project_name,
+        source="SelfMadeCAMELS",
+        # cc means China continent
+        source_path=os.path.join(
+            SETTING["local_data_path"]["datasets-interim"], "camels_cc"
+        ),
+        ctx=[0],
+        model_type="TransLearn",
+        model_name="KaiLSTM",
+        model_hyperparam={
+            "linear_size": len(var_c_target) + len(var_t_target),
+            "n_input_features": len(var_c_source) + len(var_t_source),
+            "n_output_features": 1,
+            "n_hidden_states": 256,
+        },
+        opt="Adadelta",
+        loss_func="RMSESum",
+        batch_size=5,
+        forecast_history=0,
+        forecast_length=20,
+        rs=1234,
+        train_period=train_period,
+        test_period=valid_period,
+        scaler="DapengScaler",
+        # sampler="KuaiSampler",
+        dataset="StreamflowDataset",
+        weight_path=weight_path,
+        weight_path_add={
+            "freeze_params": ["lstm.b_hh", "lstm.b_ih", "lstm.w_hh", "lstm.w_ih"]
+        },
+        continue_train=True,
+        train_epoch=10,
+        te=10,
+        var_t=var_t_target,
+        var_c=var_c_target,
+        var_out=["streamflow"],
+        gage_id=gage_id,
+        ensemble=True,
+        ensemble_items={
+            "kfold": 2,
+            "batch_sizes": [20, 50],
+        },
+    )
+    cfg = default_config_file()
+    update_cfg(cfg, args)
+    ensemble_train_and_evaluate(cfg)
+    print("All processes are finished!")
```

### Comparing `torchhydro-0.0.4/tests/test_federated_learning.py` & `torchhydro-0.0.5/tests/test_federated_learning.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,75 @@
-"""
-Author: Wenyu Ouyang
-Date: 2023-09-24 14:28:48
-LastEditTime: 2023-09-25 15:12:55
-LastEditors: Wenyu Ouyang
-Description: A test for federated learning
-FilePath: /torchhydro/tests/test_federated_learning.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-import os
-import pytest
-import hydrodataset as hds
-from torchhydro.configs.config import cmd, default_config_file, update_cfg
-from torchhydro.trainers.trainer import train_and_evaluate
-
-
-@pytest.fixture()
-def config():
-    project_name = "test_camels/exp3"
-    config_data = default_config_file()
-    args = cmd(
-        sub=project_name,
-        source="CAMELS",
-        source_path=os.path.join(hds.ROOT_DIR, "camels", "camels_us"),
-        source_region="US",
-        download=0,
-        ctx=[-1],
-        model_type="FedLearn",
-        model_name="CpuLSTM",
-        model_hyperparam={
-            "n_input_features": 23,
-            "n_output_features": 1,
-            "n_hidden_states": 256,
-        },
-        gage_id=[
-            "01013500",
-            "01022500",
-            "01030500",
-            "01031500",
-            "01047000",
-            "01052500",
-            "01054200",
-            "01055000",
-            "01057000",
-            "01170100",
-        ],
-        batch_size=8,
-        rho=20,
-        var_t=["dayl", "prcp", "srad", "tmax", "tmin", "vp"],
-        # var_c=["None"],
-        var_out=["streamflow"],
-        dataset="StreamflowDataset",
-        sampler="KuaiSampler",
-        scaler="DapengScaler",
-        train_epoch=2,
-        save_epoch=1,
-        te=2,
-        train_period=["2000-10-01", "2001-10-01"],
-        valid_period=["2001-10-01", "2002-10-01"],
-        test_period=["2002-10-01", "2003-10-01"],
-        loss_func="RMSESum",
-        opt="Adam",
-        # key is epoch, start from 1
-        lr_scheduler={1: 1e-2, 2: 5e-3, 3: 1e-3},
-        which_first_tensor="sequence",
-    )
-    update_cfg(config_data, args)
-    return config_data
-
-
-def test_train_evaluate(config):
-    train_and_evaluate(config)
+"""
+Author: Wenyu Ouyang
+Date: 2023-09-24 14:28:48
+LastEditTime: 2023-12-18 09:11:55
+LastEditors: Wenyu Ouyang
+Description: A test for federated learning
+FilePath: \torchhydro\tests\test_federated_learning.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+import os
+import pytest
+
+from torchhydro import SETTING
+from torchhydro.configs.config import cmd, default_config_file, update_cfg
+from torchhydro.trainers.trainer import train_and_evaluate
+
+
+@pytest.fixture()
+def config():
+    project_name = "test_camels/exp3"
+    config_data = default_config_file()
+    args = cmd(
+        sub=project_name,
+        source="CAMELS",
+        source_path=os.path.join(
+            SETTING["local_data_path"]["datasets-origin"], "camels", "camels_us"
+        ),
+        source_region="US",
+        ctx=[-1],
+        model_type="FedLearn",
+        model_name="CpuLSTM",
+        model_hyperparam={
+            "n_input_features": 23,
+            "n_output_features": 1,
+            "n_hidden_states": 256,
+        },
+        gage_id=[
+            "01013500",
+            "01022500",
+            "01030500",
+            "01031500",
+            "01047000",
+            "01052500",
+            "01054200",
+            "01055000",
+            "01057000",
+            "01170100",
+        ],
+        batch_size=8,
+        forecast_history=0,
+        forecast_length=20,
+        var_t=["dayl", "prcp", "srad", "tmax", "tmin", "vp"],
+        # var_c=["None"],
+        var_out=["streamflow"],
+        dataset="StreamflowDataset",
+        sampler="KuaiSampler",
+        scaler="DapengScaler",
+        train_epoch=2,
+        save_epoch=1,
+        te=2,
+        train_period=["2000-10-01", "2001-10-01"],
+        valid_period=["2001-10-01", "2002-10-01"],
+        test_period=["2002-10-01", "2003-10-01"],
+        loss_func="RMSESum",
+        opt="Adam",
+        # key is epoch, start from 1
+        lr_scheduler={1: 1e-2, 2: 5e-3, 3: 1e-3},
+        which_first_tensor="sequence",
+    )
+    update_cfg(config_data, args)
+    return config_data
+
+
+def test_train_evaluate(config):
+    train_and_evaluate(config)
```

### Comparing `torchhydro-0.0.4/tests/test_weight_analysis.py` & `torchhydro-0.0.5/tests/test_weight_analysis.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,60 +1,59 @@
-"""
-Author: Wenyu Ouyang
-Date: 2023-11-21 07:20:41
-LastEditTime: 2023-11-27 20:45:36
-LastEditors: Wenyu Ouyang
-Description: Test weight analysis
-FilePath: \torchhydro\tests\test_weight_analysis.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-import os
-import matplotlib
-import pandas as pd
-import pytest
-
-
-from torchhydro.explainers.weight_anlysis import (
-    plot_param_hist_model,
-)
-
-
-@pytest.fixture()
-def result_dir():
-    project_dir = os.getcwd()
-    return os.path.join(project_dir, "results")
-
-
-def test_weight_analysis(result_dir):
-    basin_id = "61561"
-    # NOTICE: THE ORDER CANNOT BE MODIFIED WITHOUT DEBUGGING THE CODE IN plot_param_hist_model_fold
-    chosen_layer_for_hist = [
-        "former_linear.bias",
-        "former_linear.weight",
-        "linearIn.bias",
-        "linearIn.weight",
-        "linearOut.bias",
-        "linearOut.weight",
-        "lstm.b_hh",
-        "lstm.b_ih",
-        "lstm.w_hh",
-        "lstm.w_ih",
-    ]
-    # too many figures lead to "Fail to allocate bitmap"
-    show_hist_b = 20
-    fold = 0
-    exp61561_dir = os.path.join(result_dir, "test_camels", "expcccv61561_0")
-    _, chosen_layers_consine = plot_param_hist_model(
-        "lstm",
-        exp61561_dir,
-        show_hist_b,
-        chosen_layer_for_hist,
-        start_epoch=0,
-        end_epoch=10,
-        epoch_interval=1,
-    )
-    pd.DataFrame(chosen_layers_consine).to_csv(
-        os.path.join(
-            exp61561_dir,
-            f"{basin_id}_bs{show_hist_b}_fold{fold}_chosen_layer_consine.csv",
-        )
-    )
+"""
+Author: Wenyu Ouyang
+Date: 2023-11-21 07:20:41
+LastEditTime: 2023-12-18 09:16:10
+LastEditors: Wenyu Ouyang
+Description: Test weight analysis
+FilePath: \torchhydro\tests\test_weight_analysis.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+import os
+import pandas as pd
+import pytest
+
+
+from torchhydro.explainers.weight_anlysis import (
+    plot_param_hist_model,
+)
+
+
+@pytest.fixture()
+def result_dir():
+    project_dir = os.getcwd()
+    return os.path.join(project_dir, "results")
+
+
+def test_weight_analysis(result_dir):
+    basin_id = "61561"
+    # NOTICE: THE ORDER CANNOT BE MODIFIED WITHOUT DEBUGGING THE CODE IN plot_param_hist_model_fold
+    chosen_layer_for_hist = [
+        "former_linear.bias",
+        "former_linear.weight",
+        "linearIn.bias",
+        "linearIn.weight",
+        "linearOut.bias",
+        "linearOut.weight",
+        "lstm.b_hh",
+        "lstm.b_ih",
+        "lstm.w_hh",
+        "lstm.w_ih",
+    ]
+    # too many figures lead to "Fail to allocate bitmap"
+    show_hist_b = 20
+    fold = 0
+    exp61561_dir = os.path.join(result_dir, "test_camels", "expcccv61561_0")
+    _, chosen_layers_consine = plot_param_hist_model(
+        "lstm",
+        exp61561_dir,
+        show_hist_b,
+        chosen_layer_for_hist,
+        start_epoch=0,
+        end_epoch=10,
+        epoch_interval=1,
+    )
+    pd.DataFrame(chosen_layers_consine).to_csv(
+        os.path.join(
+            exp61561_dir,
+            f"{basin_id}_bs{show_hist_b}_fold{fold}_chosen_layer_consine.csv",
+        )
+    )
```

### Comparing `torchhydro-0.0.4/torchhydro/configs/config.py` & `torchhydro-0.0.5/torchhydro/configs/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,1020 +1,1097 @@
-"""
-Author: Wenyu Ouyang
-Date: 2021-12-31 11:08:29
-LastEditTime: 2023-11-24 18:19:55
-LastEditors: Wenyu Ouyang
-Description: Config for hydroDL
-FilePath: /torchhydro/torchhydro/configs/config.py
-Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
-"""
-import argparse
-import fnmatch
-import json
-import logging
-import os
-import pandas as pd
-import numpy as np
-from hydroutils import hydro_file
-
-DAYMET_NAME = "daymet"
-SSM_SMAP_NAME = "ssm"
-ET_MODIS_NAME = "ET"
-Q_CAMELS_US_NAME = "usgsFlow"
-# Q_CAMELS_CC_NAME = "Q_fix"
-Q_CAMELS_CC_NAME = "Q"
-PRCP_DAYMET_NAME = "prcp"
-PRCP_NLDAS_NAME = "total_precipitation"
-PET_MODIS_NAME = "PET"
-PET_NLDAS_NAME = "potential_evaporation"
-NLDAS_NAME = "nldas"
-ERA5LAND_NAME = "era5land"
-ET_ERA5LAND_NAME = "total_evaporation"
-PRCP_ERA5LAND_NAME = "total_precipitation"
-PET_DAYMET_NAME = "PET"
-PET_ERA5LAND_NAME = "potential_evaporation"
-
-
-def default_config_file():
-    """
-    Default config file for all models/data/training parameters in this repo
-
-    Returns
-    -------
-    dict
-        configurations
-    """
-
-    return {
-        "model_cfgs": {
-            # model_type including normal deep learning (Normal), federated learning (FedLearn), transfer learing (TransLearn), multi-task learning, etc.
-            "model_type": "Normal",
-            # supported models can be seen in hydroDL/model_dict_function.py
-            "model_name": "LSTM",
-            # the details of model parameters for the "model_name" model
-            "model_hyperparam": {
-                # the rho in LSTM
-                "seq_length": 30,
-                # the size of input (feature number)
-                "input_size": 24,
-                # the length of output time-sequence (feature number)
-                "output_size": 1,
-                "hidden_size": 20,
-                "num_layers": 1,
-                "bias": True,
-                "batch_size": 100,
-            },
-            "weight_path": None,
-            "continue_train": True,
-            # the name of the model's wrapper class
-            "model_wrapper": None,
-            # the wrapper class's parameters
-            "model_wrapper_param": None,
-            # federated learning parameters
-            "fl_hyperparam": {
-                # sampling for federated learning
-                "fl_sample": "basin",
-                # number of users for federated learning
-                # TODO: we don't use this parameter now, but we may use it in the future
-                "fl_num_users": 10,
-                # the number of local epochs
-                "fl_local_ep": 5,
-                # local batch size
-                "fl_local_bs": 6,
-                # the fraction of clients
-                "fl_frac": 0.1,
-            },
-            "tl_hyperparam": {
-                # part of transfer learning in a model: a list of layers' names, such as ["lstm"]
-                "tl_part": None,
-            },
-        },
-        "data_cfgs": {
-            "data_source_name": "CAMELS",
-            "data_path": "../../example/camels_us",
-            "data_region": None,
-            "download": True,
-            "validation_path": None,
-            "test_path": None,
-            "batch_size": 100,
-            # the rho in LSTM
-            "forecast_history": 30,
-            "forecast_length": 1,
-            # modeled objects
-            "object_ids": "ALL",
-            # modeling time range
-            "t_range_train": ["1992-01-01", "1993-01-01"],
-            "t_range_valid": None,
-            "t_range_test": ["1993-01-01", "1994-01-01"],
-            # For physics-based models, we need warmup; default is 0 as DL models generally don't need it
-            "warmup_length": 0,
-            # the output
-            "target_cols": [Q_CAMELS_US_NAME],
-            "target_rm_nan": False,
-            # only for cases in which target data will be used as input:
-            # data assimilation -- use streamflow from period 0 to t-1 (TODO: not included now)
-            # for physics-based model -- use streamflow to calibrate models
-            "target_as_input": False,
-            # the time series input
-            # TODO: now we only support one forcing type
-            "relevant_types": [DAYMET_NAME],
-            "relevant_cols": [
-                "dayl",
-                PRCP_DAYMET_NAME,
-                "srad",
-                "swe",
-                "tmax",
-                "tmin",
-                "vp",
-            ],
-            "relevant_rm_nan": True,
-            # the attribute input
-            "constant_cols": [
-                "elev_mean",
-                "slope_mean",
-                "area_gages2",
-                "frac_forest",
-                "lai_max",
-                "lai_diff",
-                "dom_land_cover_frac",
-                "dom_land_cover",
-                "root_depth_50",
-                "soil_depth_statsgo",
-                "soil_porosity",
-                "soil_conductivity",
-                "max_water_content",
-                "geol_1st_class",
-                "geol_2nd_class",
-                "geol_porostiy",
-                "geol_permeability",
-            ],
-            "constant_rm_nan": True,
-            # if constant_only, we will only use constant data as DL models' input: this is only for dpl models now
-            "constant_only": False,
-            # more other cols, use dict to express!
-            "other_cols": None,
-            # only numerical scaler: for categorical vars, they are transformed to numerical vars when reading them
-            "scaler": "StandardScaler",
-            # Some parameters for the chosen scaler function, default is DapengScaler's
-            "scaler_params": {
-                "prcp_norm_cols": [
-                    Q_CAMELS_US_NAME,
-                    "streamflow",
-                    Q_CAMELS_CC_NAME,
-                    "qobs",
-                ],
-                "gamma_norm_cols": [
-                    PRCP_DAYMET_NAME,
-                    "pr",
-                    # PRCP_ERA5LAND_NAME is same as PRCP_NLDAS_NAME
-                    PRCP_NLDAS_NAME,
-                    "pre",
-                    # pet may be negative, but we set negative as 0 because of gamma_norm_cols
-                    # https://earthscience.stackexchange.com/questions/12031/does-negative-reference-evapotranspiration-make-sense-using-fao-penman-monteith
-                    "pet",
-                    # PET_ERA5LAND_NAME is same as PET_NLDAS_NAME
-                    PET_NLDAS_NAME,
-                    ET_MODIS_NAME,
-                    "LE",
-                    PET_MODIS_NAME,
-                    "PLE",
-                    "GPP",
-                    "Ec",
-                    "Es",
-                    "Ei",
-                    "ET_water",
-                    "ET_sum",
-                    SSM_SMAP_NAME,
-                    "susm",
-                    "smp",
-                    "ssma",
-                    "susma",
-                ],
-                "pbm_norm": False,
-            },
-            "stat_dict_file": None,
-            # dataset for pytorch dataset
-            "dataset": "StreamflowDataset",
-            # sampler for pytorch dataloader, here we mainly use it for Kuai Fang's sampler in all his DL papers
-            "sampler": None,
-        },
-        "training_cfgs": {
-            # if train_mode is False, don't train and evaluate
-            "train_mode": True,
-            "criterion": "RMSE",
-            "criterion_params": None,
-            "optimizer": "Adam",
-            "optim_params": {
-                "lr": 0.001,
-            },
-            "lr_scheduler": None,
-            "epochs": 20,
-            # save_epoch ==0 means only save once in the final epoch
-            "save_epoch": 0,
-            # save_iter ==0 means we don't save model during training in a epoch
-            "save_iter": 0,
-            # when we train a model for long time, some accidents may interrupt our training.
-            # Then we need retrain the model with saved weights, and the start_epoch is not 1 yet.
-            "start_epoch": 1,
-            "batch_size": 100,
-            "random_seed": 1234,
-            "device": [0],
-            "multi_targets": 1,
-            "num_workers": 0,
-            # sometimes we want to directly use the trained model in each epoch during training,
-            # for example, we want to save each epoch's log again, and in this time, we will set train_but_not_real to True
-            "train_but_not_real": False,
-            "which_first_tensor": "sequence",
-            # for ensemble exp:
-            # basically we set kfold/seeds/hyper_params for trianing such as batch_sizes
-            "ensemble": False,
-            "ensemble_items": {
-                # kfold means a time cross validation,
-                # concatenate train ,valid, and test data together,
-                # then split them into k folds
-                "kfold": None,
-                "batch_sizes": None,
-                # if seeds is not None,
-                # we will use different seeds for different sub-exps
-                "seeds": None,
-            },
-        },
-        # For evaluation
-        "evaluation_cfgs": {
-            "metrics": ["NSE"],
-            "fill_nan": "no",
-            "test_epoch": 20,
-            "explainer": None,
-        },
-    }
-
-
-def cmd(
-    sub=None,
-    source="CAMELS",
-    source_path=None,
-    source_region=None,
-    download=0,
-    scaler=None,
-    scaler_params=None,
-    dataset=None,
-    sampler=None,
-    fl_sample=None,
-    fl_num_users=None,
-    fl_local_ep=None,
-    fl_local_bs=None,
-    fl_frac=None,
-    ctx=None,
-    rs=None,
-    gage_id_file=None,
-    gage_id=None,
-    train_period=None,
-    valid_period=None,
-    test_period=None,
-    opt=None,
-    lr_scheduler=None,
-    opt_param=None,
-    batch_size=None,
-    rho=None,
-    train_mode=None,
-    train_epoch=None,
-    save_epoch=None,
-    save_iter=None,
-    te=None,
-    model_type=None,
-    model_name=None,
-    weight_path=None,
-    continue_train=None,
-    var_c=None,
-    c_rm_nan=1,
-    var_t=None,
-    t_rm_nan=1,
-    n_output=None,
-    loss_func=None,
-    model_hyperparam=None,
-    weight_path_add=None,
-    var_t_type=None,
-    var_o=None,
-    var_out=None,
-    out_rm_nan=0,
-    target_as_input=0,
-    constant_only=0,
-    gage_id_screen=None,
-    loss_param=None,
-    metrics=None,
-    fill_nan=None,
-    warmup_length=0,
-    start_epoch=1,
-    stat_dict_file=None,
-    model_wrapper=None,
-    model_wrapper_param=None,
-    num_workers=None,
-    train_but_not_real=None,
-    which_first_tensor=None,
-    ensemble=0,
-    ensemble_items=None,
-):
-    """input args from cmd"""
-    parser = argparse.ArgumentParser(
-        description="Train a Time-Series Deep Learning Model for Basins"
-    )
-    parser.add_argument(
-        "--sub", dest="sub", help="subset and sub experiment", default=sub, type=str
-    )
-    parser.add_argument(
-        "--source",
-        dest="source",
-        help="name of data source such as CAMELS",
-        default=source,
-        type=str,
-    )
-    parser.add_argument(
-        "--source_path",
-        dest="source_path",
-        help="directory of data source",
-        default=source_path,
-        nargs="+",
-    )
-    parser.add_argument(
-        "--source_region",
-        dest="source_region",
-        help="region(s) of data source such as US, or ['US','CE']",
-        default=source_region,
-        nargs="+",
-    )
-    parser.add_argument(
-        "--download",
-        dest="download",
-        help="Do we need to download data",
-        default=download,
-        type=int,
-    )
-    parser.add_argument(
-        "--scaler",
-        dest="scaler",
-        help="Choose a Scaler function",
-        default=scaler,
-        type=str,
-    )
-    parser.add_argument(
-        "--scaler_params",
-        dest="scaler_params",
-        help="Parameters of the chosen Scaler function",
-        default=scaler_params,
-        type=json.loads,
-    )
-    parser.add_argument(
-        "--dataset",
-        dest="dataset",
-        help="Choose a dataset class for PyTorch",
-        default=dataset,
-        type=str,
-    )
-    parser.add_argument(
-        "--sampler",
-        dest="sampler",
-        help="None or KuaiSampler",
-        default=sampler,
-        type=str,
-    )
-    parser.add_argument(
-        "--fl_sample",
-        dest="fl_sample",
-        help="sampling method for federated learning",
-        default=fl_sample,
-        type=str,
-    )
-    parser.add_argument(
-        "--fl_num_users",
-        dest="fl_num_users",
-        help="number of users for federated learning",
-        default=fl_num_users,
-        type=int,
-    )
-    parser.add_argument(
-        "--fl_local_ep",
-        dest="fl_local_ep",
-        help="number of local epochs for federated learning",
-        default=fl_local_ep,
-        type=int,
-    )
-    parser.add_argument(
-        "--fl_local_bs",
-        dest="fl_local_bs",
-        help="local batch size for federated learning",
-        default=fl_local_bs,
-        type=float,
-    )
-    parser.add_argument(
-        "--fl_frac",
-        dest="fl_frac",
-        help="the fraction of clients for federated learning",
-        default=fl_frac,
-        type=float,
-    )
-    parser.add_argument(
-        "--ctx",
-        dest="ctx",
-        help="Running Context -- gpu num or cpu. E.g `--ctx 0 1` means run code in gpu 0 and 1; -1 means cpu",
-        default=ctx,
-        nargs="+",
-    )
-    parser.add_argument("--rs", dest="rs", help="random seed", default=rs, type=int)
-    parser.add_argument("--te", dest="te", help="test epoch", default=te, type=int)
-    # There is something wrong with "bool", so I used 1 as True, 0 as False
-    parser.add_argument(
-        "--train_mode",
-        dest="train_mode",
-        help="If 0, no train or test, just read data; else train + test",
-        default=train_mode,
-        type=int,
-    )
-    parser.add_argument(
-        "--train_epoch",
-        dest="train_epoch",
-        help="epoches of training period",
-        default=train_epoch,
-        type=int,
-    )
-    parser.add_argument(
-        "--save_epoch",
-        dest="save_epoch",
-        help="save for every save_epoch epoches",
-        default=save_epoch,
-        type=int,
-    )
-    parser.add_argument(
-        "--save_iter",
-        dest="save_iter",
-        help="save for every save_iter in save_epoches",
-        default=save_iter,
-        type=int,
-    )
-    parser.add_argument(
-        "--loss_func",
-        dest="loss_func",
-        help="choose loss function",
-        default=loss_func,
-        type=str,
-    )
-    parser.add_argument(
-        "--loss_param",
-        dest="loss_param",
-        help="choose parameters of loss function",
-        default=loss_param,
-        type=json.loads,
-    )
-    parser.add_argument(
-        "--train_period",
-        dest="train_period",
-        help="The training period",
-        default=train_period,
-        nargs="+",
-    )
-    parser.add_argument(
-        "--valid_period",
-        dest="valid_period",
-        help="The validating period",
-        default=valid_period,
-        nargs="+",
-    )
-    parser.add_argument(
-        "--test_period",
-        dest="test_period",
-        help="The test period",
-        default=test_period,
-        nargs="+",
-    )
-    parser.add_argument(
-        "--batch_size",
-        dest="batch_size",
-        help="batch_size",
-        default=batch_size,
-        type=int,
-    )
-    parser.add_argument(
-        "--rho",
-        dest="rho",
-        help="length of time sequence when training",
-        default=rho,
-        type=int,
-    )
-    parser.add_argument(
-        "--model_type",
-        dest="model_type",
-        help="The type of DL model",
-        default=model_type,
-        type=str,
-    )
-    parser.add_argument(
-        "--model_name",
-        dest="model_name",
-        help="The name of DL model. now in the zoo",
-        default=model_name,
-        type=str,
-    )
-    parser.add_argument(
-        "--weight_path",
-        dest="weight_path",
-        help="The weights of trained model",
-        default=weight_path,
-        type=str,
-    )
-    parser.add_argument(
-        "--weight_path_add",
-        dest="weight_path_add",
-        help="More info about the weights of trained model",
-        default=weight_path_add,
-        type=json.loads,
-    )
-    parser.add_argument(
-        "--continue_train",
-        dest="continue_train",
-        help="Continue to train the model from weight_path when continue_train>0",
-        default=continue_train,
-        type=int,
-    )
-    parser.add_argument(
-        "--gage_id",
-        dest="gage_id",
-        help="just select some sites",
-        default=gage_id,
-        nargs="+",
-    )
-    parser.add_argument(
-        "--gage_id_screen",
-        dest="gage_id_screen",
-        help="the criterion to chose some gages",
-        default=gage_id_screen,
-        type=json.loads,
-    )
-    parser.add_argument(
-        "--gage_id_file",
-        dest="gage_id_file",
-        help="select some sites from a file",
-        default=gage_id_file,
-        type=str,
-    )
-    parser.add_argument(
-        "--opt", dest="opt", help="choose an optimizer", default=opt, type=str
-    )
-    parser.add_argument(
-        "--opt_param",
-        dest="opt_param",
-        help="the optimizer parameters",
-        default=opt_param,
-        type=json.loads,
-    )
-    parser.add_argument(
-        "--var_c", dest="var_c", help="types of attributes", default=var_c, nargs="+"
-    )
-    parser.add_argument(
-        "--c_rm_nan",
-        dest="c_rm_nan",
-        help="if true, we remove NaN value for var_c data when scaling",
-        default=c_rm_nan,
-        type=int,
-    )
-    parser.add_argument(
-        "--var_t", dest="var_t", help="types of forcing", default=var_t, nargs="+"
-    )
-    parser.add_argument(
-        "--t_rm_nan",
-        dest="t_rm_nan",
-        help="if true, we remove NaN value for var_t data when scaling",
-        default=t_rm_nan,
-        type=int,
-    )
-    parser.add_argument(
-        "--var_t_type",
-        dest="var_t_type",
-        help="types of forcing data_source",
-        default=var_t_type,
-        nargs="+",
-    )
-    parser.add_argument(
-        "--var_o",
-        dest="var_o",
-        help="more other inputs except for var_c and var_t",
-        default=var_o,
-        type=json.loads,
-    )
-    parser.add_argument(
-        "--var_out", dest="var_out", help="type of outputs", default=var_out, nargs="+"
-    )
-    parser.add_argument(
-        "--out_rm_nan",
-        dest="out_rm_nan",
-        help="if true, we remove NaN value for var_out data when scaling",
-        default=out_rm_nan,
-        type=int,
-    )
-    parser.add_argument(
-        "--target_as_input",
-        dest="target_as_input",
-        help="if true, we will use target data as input for data assimilation or physics-based models",
-        default=target_as_input,
-        type=int,
-    )
-    parser.add_argument(
-        "--constant_only",
-        dest="constant_only",
-        help="if true, we will only use attribute data as input for deep learning models; "
-        "now it is only for dpl models and it is only used when target_as_input is False",
-        default=constant_only,
-        type=int,
-    )
-    parser.add_argument(
-        "--n_output",
-        dest="n_output",
-        help="the number of output features",
-        default=n_output,
-        type=int,
-    )
-    parser.add_argument(
-        "--model_hyperparam",
-        dest="model_hyperparam",
-        help="the model_hyperparam in model_cfgs",
-        default=model_hyperparam,
-        type=json.loads,
-    )
-    parser.add_argument(
-        "--metrics",
-        dest="metrics",
-        help="The evaluating metrics",
-        default=metrics,
-        nargs="+",
-    )
-    parser.add_argument(
-        "--fill_nan",
-        dest="fill_nan",
-        help="how to fill nan values when evaluating",
-        default=fill_nan,
-        nargs="+",
-    )
-    parser.add_argument(
-        "--warmup_length",
-        dest="warmup_length",
-        help="Physical hydro models need warmup",
-        default=warmup_length,
-        type=int,
-    )
-    parser.add_argument(
-        "--start_epoch",
-        dest="start_epoch",
-        help="The index of epoch when starting training, default is 1. "
-        "When retraining after an interrupt, it will be larger than 1",
-        default=start_epoch,
-        type=int,
-    )
-    parser.add_argument(
-        "--stat_dict_file",
-        dest="stat_dict_file",
-        help="for testing sometimes such as pub cases, we need stat_dict_file from trained dataset",
-        default=stat_dict_file,
-        type=str,
-    )
-    parser.add_argument(
-        "--model_wrapper",
-        dest="model_wrapper",
-        help="Sometimes we need a wrapper for the DL models to add some functions",
-        default=model_wrapper,
-        type=str,
-    )
-    parser.add_argument(
-        "--model_wrapper_param",
-        dest="model_wrapper_param",
-        help="The parameters for model_wrapper",
-        default=model_wrapper_param,
-        type=json.loads,
-    )
-    parser.add_argument(
-        "--num_workers",
-        dest="num_workers",
-        help="The number of workers used in Dataloader",
-        default=num_workers,
-        type=int,
-    )
-    parser.add_argument(
-        "--train_but_not_real",
-        dest="train_but_not_real",
-        help="If true, we will enter the training function but not really train the model and just use the trained model during training",
-        default=train_but_not_real,
-        type=int,
-    )
-    parser.add_argument(
-        "--which_first_tensor",
-        dest="which_first_tensor",
-        help="sequence_first or batch_first",
-        default=which_first_tensor,
-        type=str,
-    )
-    parser.add_argument(
-        "--lr_scheduler",
-        dest="lr_scheduler",
-        help="The learning rate scheduler",
-        default=lr_scheduler,
-        type=json.loads,
-    )
-    parser.add_argument(
-        "--ensemble",
-        dest="ensemble",
-        help="ensemble config",
-        default=ensemble,
-        type=int,
-    )
-    parser.add_argument(
-        "--ensemble_items",
-        dest="ensemble_items",
-        help="ensemble config",
-        default=ensemble_items,
-        type=json.loads,
-    )
-    # To make pytest work in PyCharm, here we use the following code instead of "args = parser.parse_args()":
-    # https://blog.csdn.net/u014742995/article/details/100119905
-    args, unknown = parser.parse_known_args()
-    return args
-
-
-def update_nested_dict(d, keys, value):
-    """update nested dict
-
-    Parameters
-    ----------
-    d
-        the dict to be updated
-    keys
-        the keys of the dict
-    value
-        the updated value of the dict
-    """
-    if len(keys) == 1:
-        d[keys[0]] = value
-    else:
-        update_nested_dict(d[keys[0]], keys[1:], value)
-
-
-def update_cfg(cfg_file, new_args):
-    """
-    Update default config with new arguments
-
-    Parameters
-    ----------
-    cfg_file
-        default config
-    new_args
-        new arguments
-
-    Returns
-    -------
-    None
-        in-place operation for cfg_file
-    """
-    print("update config file")
-    project_dir = os.getcwd()
-    result_dir = os.path.join(project_dir, "results")
-    if os.path.exists(result_dir) is False:
-        os.makedirs(result_dir)
-    if new_args.sub is not None:
-        subset, subexp = new_args.sub.split("/")
-        cfg_file["data_cfgs"]["validation_path"] = os.path.join(
-            project_dir, "results", subset, subexp
-        )
-        cfg_file["data_cfgs"]["test_path"] = os.path.join(result_dir, subset, subexp)
-    if new_args.source is not None:
-        cfg_file["data_cfgs"]["data_source_name"] = new_args.source
-    if new_args.source_path is not None:
-        cfg_file["data_cfgs"]["data_path"] = new_args.source_path
-        if type(new_args.source_path) == list and len(new_args.source_path) == 1:
-            cfg_file["data_cfgs"]["data_path"] = new_args.source_path[0]
-    if new_args.source_region is not None:
-        cfg_file["data_cfgs"]["data_region"] = new_args.source_region
-        if len(new_args.source_region) == 1:
-            cfg_file["data_cfgs"]["data_region"] = new_args.source_region[0]
-    if new_args.download is not None:
-        if new_args.download == 0:
-            cfg_file["data_cfgs"]["download"] = False
-        else:
-            cfg_file["data_cfgs"]["download"] = True
-    if new_args.scaler is not None:
-        cfg_file["data_cfgs"]["scaler"] = new_args.scaler
-    if new_args.scaler_params is not None:
-        cfg_file["data_cfgs"]["scaler_params"] = new_args.scaler_params
-    if new_args.dataset is not None:
-        cfg_file["data_cfgs"]["dataset"] = new_args.dataset
-    if new_args.sampler is not None:
-        cfg_file["data_cfgs"]["sampler"] = new_args.sampler
-    if new_args.fl_sample is not None:
-        if new_args.fl_sample not in ["basin", "region"]:
-            # basin means each client is a basin
-            raise ValueError("fl_sample must be 'basin' or 'region'")
-        cfg_file["model_cfgs"]["fl_hyperparam"]["fl_sample"] = new_args.fl_sample
-    if new_args.fl_num_users is not None:
-        cfg_file["model_cfgs"]["fl_hyperparam"]["fl_num_users"] = new_args.fl_num_users
-    if new_args.fl_local_ep is not None:
-        cfg_file["model_cfgs"]["fl_hyperparam"]["fl_local_ep"] = new_args.fl_local_ep
-    if new_args.fl_local_bs is not None:
-        cfg_file["model_cfgs"]["fl_hyperparam"]["fl_local_bs"] = new_args.fl_local_bs
-    if new_args.fl_frac is not None:
-        cfg_file["model_cfgs1"]["fl_hyperparam"]["fl_frac"] = new_args.fl_frac
-    if new_args.ctx is not None:
-        cfg_file["training_cfgs"]["device"] = new_args.ctx
-    if new_args.rs is not None:
-        cfg_file["training_cfgs"]["random_seed"] = new_args.rs
-    if new_args.train_mode is not None:
-        if new_args.train_mode > 0:
-            cfg_file["training_cfgs"]["train_mode"] = True
-        else:
-            cfg_file["training_cfgs"]["train_mode"] = False
-    if new_args.loss_func is not None:
-        cfg_file["training_cfgs"]["criterion"] = new_args.loss_func
-        if new_args.loss_param is not None:
-            cfg_file["training_cfgs"]["criterion_params"] = new_args.loss_param
-    if new_args.train_period is not None:
-        cfg_file["data_cfgs"]["t_range_train"] = new_args.train_period
-    if new_args.valid_period is not None:
-        cfg_file["data_cfgs"]["t_range_valid"] = new_args.valid_period
-    if new_args.test_period is not None:
-        cfg_file["data_cfgs"]["t_range_test"] = new_args.test_period
-    if new_args.gage_id is not None or new_args.gage_id_file is not None:
-        if new_args.gage_id_file is not None:
-            gage_id_lst = (
-                pd.read_csv(new_args.gage_id_file, dtype={0: str}).iloc[:, 0].values
-            )
-            cfg_file["data_cfgs"]["object_ids"] = gage_id_lst.tolist()
-        else:
-            cfg_file["data_cfgs"]["object_ids"] = new_args.gage_id
-    if new_args.opt is not None:
-        cfg_file["training_cfgs"]["optimizer"] = new_args.opt
-        if new_args.opt_param is not None:
-            cfg_file["training_cfgs"]["optim_params"] = new_args.opt_param
-        else:
-            cfg_file["training_cfgs"]["optim_params"] = {}
-    if new_args.var_c is not None:
-        # I don't find a method to receive empty list for argparse, so if we input "None" or "" or " ", we treat it as []
-        if (
-            new_args.var_c == ["None"]
-            or new_args.var_c == [""]
-            or new_args.var_c == [" "]
-        ):
-            cfg_file["data_cfgs"]["constant_cols"] = []
-        else:
-            cfg_file["data_cfgs"]["constant_cols"] = new_args.var_c
-    if new_args.c_rm_nan == 0:
-        cfg_file["data_cfgs"]["constant_rm_nan"] = False
-    else:
-        cfg_file["data_cfgs"]["constant_rm_nan"] = True
-    if new_args.var_t is not None:
-        cfg_file["data_cfgs"]["relevant_cols"] = new_args.var_t
-    if new_args.var_t_type is not None:
-        cfg_file["data_cfgs"]["relevant_types"] = new_args.var_t_type
-    if new_args.t_rm_nan == 0:
-        cfg_file["data_cfgs"]["relevant_rm_nan"] = False
-    else:
-        cfg_file["data_cfgs"]["relevant_rm_nan"] = True
-    if new_args.var_o is not None:
-        cfg_file["data_cfgs"]["other_cols"] = new_args.var_o
-    if new_args.var_out is not None:
-        cfg_file["data_cfgs"]["target_cols"] = new_args.var_out
-    if new_args.out_rm_nan == 0:
-        cfg_file["data_cfgs"]["target_rm_nan"] = False
-    else:
-        cfg_file["data_cfgs"]["target_rm_nan"] = True
-    if new_args.target_as_input == 0:
-        cfg_file["data_cfgs"]["target_as_input"] = False
-        if new_args.constant_only == 0:
-            cfg_file["data_cfgs"]["constant_only"] = False
-        else:
-            cfg_file["data_cfgs"]["constant_only"] = True
-    else:
-        cfg_file["data_cfgs"]["target_as_input"] = True
-    if new_args.train_epoch is not None:
-        cfg_file["training_cfgs"]["epochs"] = new_args.train_epoch
-    if new_args.save_epoch is not None:
-        cfg_file["training_cfgs"]["save_epoch"] = new_args.save_epoch
-    if new_args.save_iter is not None:
-        cfg_file["training_cfgs"]["save_iter"] = new_args.save_iter
-    if new_args.model_type is not None:
-        cfg_file["model_cfgs"]["model_type"] = new_args.model_type
-    if new_args.model_name is not None:
-        cfg_file["model_cfgs"]["model_name"] = new_args.model_name
-    if new_args.weight_path is not None:
-        cfg_file["model_cfgs"]["weight_path"] = new_args.weight_path
-        if new_args.continue_train is None or new_args.continue_train == 0:
-            continue_train = False
-        else:
-            continue_train = True
-        cfg_file["model_cfgs"]["continue_train"] = continue_train
-    if new_args.weight_path_add is not None:
-        cfg_file["model_cfgs"]["weight_path_add"] = new_args.weight_path_add
-    if new_args.n_output is not None:
-        cfg_file["training_cfgs"]["multi_targets"] = new_args.n_output
-        if len(cfg_file["data_cfgs"]["target_cols"]) != new_args.n_output:
-            raise AttributeError(
-                "Please make sure size of vars in data_cfgs/target_cols is same as n_output"
-            )
-    if new_args.model_hyperparam is None:
-        if new_args.batch_size is not None:
-            batch_size = new_args.batch_size
-            cfg_file["model_cfgs"]["model_hyperparam"]["batch_size"] = batch_size
-            cfg_file["data_cfgs"]["batch_size"] = batch_size
-            cfg_file["training_cfgs"]["batch_size"] = batch_size
-        if new_args.rho is not None:
-            rho = new_args.rho
-            cfg_file["model_cfgs"]["model_hyperparam"]["seq_length"] = rho
-            cfg_file["data_cfgs"]["forecast_history"] = rho
-        if new_args.n_output is not None:
-            cfg_file["model_cfgs"]["model_hyperparam"][
-                "output_seq_len"
-            ] = new_args.n_output
-    else:
-        cfg_file["model_cfgs"]["model_hyperparam"] = new_args.model_hyperparam
-        if "batch_size" in new_args.model_hyperparam.keys():
-            cfg_file["data_cfgs"]["batch_size"] = new_args.model_hyperparam[
-                "batch_size"
-            ]
-            cfg_file["training_cfgs"]["batch_size"] = new_args.model_hyperparam[
-                "batch_size"
-            ]
-        elif new_args.batch_size is not None:
-            batch_size = new_args.batch_size
-            cfg_file["data_cfgs"]["batch_size"] = batch_size
-            cfg_file["training_cfgs"]["batch_size"] = batch_size
-        else:
-            raise NotImplemented("Please set the batch_size!!!")
-        if "seq_length" in new_args.model_hyperparam.keys():
-            cfg_file["data_cfgs"]["forecast_history"] = new_args.model_hyperparam[
-                "seq_length"
-            ]
-        elif "forecast_history" in new_args.model_hyperparam.keys():
-            cfg_file["data_cfgs"]["forecast_history"] = new_args.model_hyperparam[
-                "forecast_history"
-            ]
-        elif new_args.rho is not None:
-            cfg_file["data_cfgs"]["forecast_history"] = new_args.rho
-        else:
-            raise NotImplemented(
-                "Please set the time_sequence length in a batch when training!!!"
-            )
-        if (
-            "output_seq_len" in new_args.model_hyperparam.keys()
-            and new_args.n_output is not None
-        ):
-            assert new_args.model_hyperparam["output_seq_len"] == new_args.n_output
-    if new_args.metrics is not None:
-        cfg_file["evaluation_cfgs"]["metrics"] = new_args.metrics
-    if new_args.fill_nan is not None:
-        cfg_file["evaluation_cfgs"]["fill_nan"] = new_args.fill_nan
-    if new_args.te is not None:
-        cfg_file["evaluation_cfgs"]["test_epoch"] = new_args.te
-        if new_args.train_epoch is not None and new_args.te > new_args.train_epoch:
-            raise RuntimeError("testing epoch cannot be larger than training epoch")
-    if new_args.warmup_length > 0:
-        cfg_file["data_cfgs"]["warmup_length"] = new_args.warmup_length
-        if "warmup_length" in new_args.model_hyperparam.keys() and (
-            not cfg_file["data_cfgs"]["warmup_length"]
-            == new_args.model_hyperparam["warmup_length"]
-        ):
-            raise RuntimeError(
-                "Please set same warmup_length in model_cfgs and data_cfgs"
-            )
-    if new_args.start_epoch > 1:
-        cfg_file["training_cfgs"]["start_epoch"] = new_args.start_epoch
-    if new_args.stat_dict_file is not None:
-        cfg_file["data_cfgs"]["stat_dict_file"] = new_args.stat_dict_file
-
-    if new_args.model_wrapper is not None:
-        cfg_file["model_cfgs"]["model_wrapper"] = new_args.model_wrapper
-    if new_args.model_wrapper_param is not None:
-        cfg_file["model_cfgs"]["model_wrapper_param"] = new_args.model_wrapper_param
-    if new_args.num_workers is not None and new_args.num_workers > 0:
-        cfg_file["training_cfgs"]["num_workers"] = new_args.num_workers
-    if new_args.train_but_not_real is not None and new_args.train_but_not_real > 0:
-        cfg_file["training_cfgs"]["train_but_not_real"] = True
-    if new_args.which_first_tensor is not None:
-        cfg_file["training_cfgs"]["which_first_tensor"] = new_args.which_first_tensor
-    if new_args.lr_scheduler is not None:
-        cfg_file["training_cfgs"]["lr_scheduler"] = new_args.lr_scheduler
-    if new_args.ensemble == 0:
-        cfg_file["training_cfgs"]["ensemble"] = False
-    else:
-        cfg_file["training_cfgs"]["ensemble"] = True
-    if new_args.ensemble_items is not None:
-        cfg_file["training_cfgs"]["ensemble_items"] = new_args.ensemble_items
-    # print("the updated config:\n", json.dumps(cfg_file, indent=4, ensure_ascii=False))
-
-
-def get_config_file(cfg_dir):
-    json_files_lst = []
-    json_files_ctime = []
-    for file in os.listdir(cfg_dir):
-        if (
-            fnmatch.fnmatch(file, "*.json")
-            and "_stat" not in file  # statistics json file
-            and "_dict" not in file  # data cache json file
-        ):
-            json_files_lst.append(os.path.join(cfg_dir, file))
-            json_files_ctime.append(os.path.getctime(os.path.join(cfg_dir, file)))
-    sort_idx = np.argsort(json_files_ctime)
-    cfg_file = json_files_lst[sort_idx[-1]]
-    cfg = hydro_file.unserialize_json(cfg_file)
-    return cfg
+"""
+Author: Wenyu Ouyang
+Date: 2021-12-31 11:08:29
+LastEditTime: 2024-05-31 11:00:18
+LastEditors: Wenyu Ouyang
+Description: Config for hydroDL
+FilePath: \torchhydro\torchhydro\configs\config.py
+Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
+"""
+
+import argparse
+import fnmatch
+import json
+import os
+
+import numpy as np
+import pandas as pd
+from hydroutils import hydro_file
+
+DAYMET_NAME = "daymet"
+SSM_SMAP_NAME = "ssm"
+ET_MODIS_NAME = "ET"
+Q_CAMELS_US_NAME = "streamflow"
+Q_CAMELS_CC_NAME = "Q"
+PRCP_DAYMET_NAME = "prcp"
+PRCP_NLDAS_NAME = "total_precipitation"
+PET_MODIS_NAME = "PET"
+PET_NLDAS_NAME = "potential_evaporation"
+NLDAS_NAME = "nldas"
+ERA5LAND_NAME = "era5land"
+ET_ERA5LAND_NAME = "total_evaporation"
+PRCP_ERA5LAND_NAME = "total_precipitation"
+PET_DAYMET_NAME = "PET"
+PET_ERA5LAND_NAME = "potential_evaporation"
+DATE_FORMATS = ["%Y-%m-%d-%H", "%Y-%m-%d"]  # 带小时的日期格式  # 不带小时的日期格式
+
+
+def default_config_file():
+    """
+    Default config file for all models/data/training parameters in this repo
+
+    Returns
+    -------
+    dict
+        configurations
+    """
+
+    return {
+        "model_cfgs": {
+            # model_type including normal deep learning (Normal), federated learning (FedLearn), transfer learing (TransLearn), multi-task learning (MTL), etc.
+            "model_type": "Normal",
+            # supported models can be seen in hydroDL/model_dict_function.py
+            "model_name": "LSTM",
+            # the details of model parameters for the "model_name" model
+            "model_hyperparam": {
+                # <- warmup -><- forecast_history -><- forecast_length ->
+                "forecast_history": 30,
+                "forecast_length": 30,
+                # the size of input (feature number)
+                "input_size": 24,
+                # the length of output time-sequence (feature number)
+                "output_size": 1,
+                "hidden_size": 20,
+                "num_layers": 1,
+                "bias": True,
+                "batch_size": 100,
+                "dropout": 0.2,
+            },
+            "weight_path": None,
+            "continue_train": True,
+            # federated learning parameters
+            "fl_hyperparam": {
+                # sampling for federated learning
+                "fl_sample": "basin",
+                # number of users for federated learning
+                # TODO: we don't use this parameter now, but we may use it in the future
+                "fl_num_users": 10,
+                # the number of local epochs
+                "fl_local_ep": 5,
+                # local batch size
+                "fl_local_bs": 6,
+                # the fraction of clients
+                "fl_frac": 0.1,
+            },
+            "tl_hyperparam": {
+                # part of transfer learning in a model: a list of layers' names, such as ["lstm"]
+                "tl_part": None,
+            },
+        },
+        "data_cfgs": {
+            "source_cfgs": {
+                # the name of data source, such as CAMELS
+                "source_names": ["CAMELS"],
+                "source_paths": ["../../example/camels_us"],
+            },
+            "validation_path": None,
+            "test_path": None,
+            "batch_size": 100,
+            # we generally have three times: [warmup, forecast_history, forecast_length]
+            # For physics-based models, we need warmup; default is 0 as DL models generally don't need it
+            "warmup_length": 0,
+            # the length of the history data for forecasting
+            "forecast_history": 30,
+            # the length of the forecast data
+            "forecast_length": 1,
+            # the min time step of the input data
+            "min_time_unit": "D",
+            # the min time interval of the input data
+            "min_time_interval": 1,
+            # modeled objects
+            "object_ids": "ALL",
+            # modeling time range
+            "t_range_train": ["1992-01-01", "1993-01-01"],
+            "t_range_valid": None,
+            "t_range_test": ["1993-01-01", "1994-01-01"],
+            # the output
+            "target_cols": [Q_CAMELS_US_NAME],
+            "target_rm_nan": True,
+            # only for cases in which target data will be used as input:
+            # data assimilation -- use streamflow from period 0 to t-1 (TODO: not included now)
+            # for physics-based model -- use streamflow to calibrate models
+            "target_as_input": False,
+            # the time series input
+            # TODO: now we only support one forcing type
+            "relevant_types": [DAYMET_NAME],
+            "relevant_cols": [
+                "dayl",
+                PRCP_DAYMET_NAME,
+                "srad",
+                "swe",
+                "tmax",
+                "tmin",
+                "vp",
+            ],
+            "relevant_rm_nan": True,
+            # the attribute input
+            "constant_cols": [
+                "elev_mean",
+                "slope_mean",
+                "area_gages2",
+                "frac_forest",
+                "lai_max",
+                "lai_diff",
+                "dom_land_cover_frac",
+                "dom_land_cover",
+                "root_depth_50",
+                "soil_depth_statsgo",
+                "soil_porosity",
+                "soil_conductivity",
+                "max_water_content",
+                "geol_1st_class",
+                "geol_2nd_class",
+                "geol_porostiy",
+                "geol_permeability",
+            ],
+            # specify the data source of each variable
+            "var_to_source_map": None,
+            # {
+            #     "temperature": "nldas4camels",
+            #     "specific_humidity": "nldas4camels",
+            #     "usgsFlow": "camels_us",
+            #     "ET": "modiset4camels",
+            # },
+            "constant_rm_nan": True,
+            # if constant_only, we will only use constant data as DL models' input: this is only for dpl models now
+            "constant_only": False,
+            # more other cols, use dict to express!
+            "other_cols": None,
+            # only numerical scaler: for categorical vars, they are transformed to numerical vars when reading them
+            "scaler": "StandardScaler",
+            # Some parameters for the chosen scaler function, default is DapengScaler's
+            "scaler_params": {
+                "prcp_norm_cols": [
+                    Q_CAMELS_US_NAME,
+                    "streamflow",
+                    Q_CAMELS_CC_NAME,
+                    "qobs",
+                    "qobs_mm_per_hour",
+                ],
+                "gamma_norm_cols": [
+                    PRCP_DAYMET_NAME,
+                    "pr",
+                    # PRCP_ERA5LAND_NAME is same as PRCP_NLDAS_NAME
+                    PRCP_NLDAS_NAME,
+                    "pre",
+                    # pet may be negative, but we set negative as 0 because of gamma_norm_cols
+                    # https://earthscience.stackexchange.com/questions/12031/does-negative-reference-evapotranspiration-make-sense-using-fao-penman-monteith
+                    "pet",
+                    # PET_ERA5LAND_NAME is same as PET_NLDAS_NAME
+                    PET_NLDAS_NAME,
+                    ET_MODIS_NAME,
+                    "LE",
+                    PET_MODIS_NAME,
+                    "PLE",
+                    "GPP",
+                    "Ec",
+                    "Es",
+                    "Ei",
+                    "ET_water",
+                    "ET_sum",
+                    SSM_SMAP_NAME,
+                    "susm",
+                    "smp",
+                    "ssma",
+                    "susma",
+                ],
+                "pbm_norm": False,
+            },
+            "stat_dict_file": None,
+            # dataset for pytorch dataset
+            "dataset": "StreamflowDataset",
+            # sampler for pytorch dataloader, here we mainly use it for Kuai Fang's sampler in all his DL papers
+            "sampler": None,
+        },
+        "training_cfgs": {
+            "master_addr": "localhost",
+            "port": "12335",
+            # if train_mode is False, don't train and evaluate
+            "train_mode": True,
+            "criterion": "RMSE",
+            "criterion_params": None,
+            # "weight_decay": None, a regularization term in loss func
+            "optimizer": "Adam",
+            "optim_params": {},
+            "lr_scheduler": {
+                # 1st opt config, all epochs use this lr
+                "lr": 0.001,
+                # 2nd opt config, diff epoch uses diff lr, key is epoch,
+                # start from 0, each value means the decay rate
+                # "lr_scheduler": {0: 1, 1: 0.5, 2: 0.2},
+                # 3rd opt config, lr as a initial value, and lr_factor as an exponential decay factor
+                # "lr": 0.001, "lr_factor": 0.1,
+                # 4th opt config, lr as a initial value,
+                # lr_patience represent how many epochs without opt (we watch val_loss) could be tolerated
+                # if lr_patience is satisfied, then lr will be decayed by lr_factor by a linear way
+                # "lr": 0.001, "lr_factor": 0.1, "lr_patience": 1,
+            },
+            "early_stopping": False,
+            "patience": 1,
+            "epochs": 20,
+            # save_epoch ==0 means only save once in the final epoch
+            "save_epoch": 0,
+            # save_iter ==0 means we don't save model during training in a epoch
+            "save_iter": 0,
+            # when we train a model for long time, some accidents may interrupt our training.
+            # Then we need retrain the model with saved weights, and the start_epoch is not 1 yet.
+            "start_epoch": 1,
+            "batch_size": 100,
+            "random_seed": 1234,
+            "device": [0, 1, 2],
+            "multi_targets": 1,
+            "num_workers": 0,
+            "which_first_tensor": "sequence",
+            # for ensemble exp:
+            # basically we set kfold/seeds/hyper_params for trianing such as batch_sizes
+            "ensemble": False,
+            "ensemble_items": {
+                # kfold means a time cross validation,
+                # concatenate train ,valid, and test data together,
+                # then split them into k folds
+                "kfold": None,
+                "batch_sizes": None,
+                # if seeds is not None,
+                # we will use different seeds for different sub-exps
+                "seeds": None,
+                "patience": None,
+                "early_stopping": None,
+                "kfold_continuous": True,
+            },
+        },
+        # For evaluation
+        "evaluation_cfgs": {
+            # there are some different loading way of trained model weights
+            # 'epoch' means we load the weights of the specified epoch;
+            # 'best' means we load the best weights during training especially for early stopping
+            # 'latest' means we load the latest weights during training
+            # 'pth' means we load the weights from the specified path
+            "model_loader": {"load_way": "specified", "test_epoch": 20},
+            # "model_loader": {"load_way": "best"},
+            # "model_loader": {"load_way": "latest"},
+            # "model_loader": {"load_way": "pth", "pth": "path/to/weights"},
+            "metrics": ["NSE", "RMSE", "R2", "KGE", "FHV", "FLV"],
+            "fill_nan": "no",
+            "explainer": None,
+            "rolling": None,
+            "long_seq_pred": True,
+            "calc_metrics": True,
+        },
+    }
+
+
+def cmd(
+    sub=None,
+    source_cfgs=None,
+    scaler=None,
+    scaler_params=None,
+    dataset=None,
+    model_loader=None,
+    sampler=None,
+    fl_sample=None,
+    fl_num_users=None,
+    fl_local_ep=None,
+    fl_local_bs=None,
+    fl_frac=None,
+    master_addr=None,
+    port=None,
+    ctx=None,
+    rs=None,
+    gage_id_file=None,
+    gage_id=None,
+    train_period=None,
+    valid_period=None,
+    test_period=None,
+    opt=None,
+    lr_scheduler=None,
+    opt_param=None,
+    batch_size=None,
+    warmup_length=0,
+    forecast_history=None,
+    forecast_length=None,
+    train_mode=None,
+    train_epoch=None,
+    save_epoch=None,
+    save_iter=None,
+    model_type=None,
+    model_name=None,
+    weight_path=None,
+    continue_train=None,
+    var_c=None,
+    c_rm_nan=1,
+    var_t=None,
+    t_rm_nan=1,
+    n_output=None,
+    loss_func=None,
+    model_hyperparam=None,
+    dropout=None,
+    weight_path_add=None,
+    var_t_type=None,
+    var_o=None,
+    var_out=None,
+    var_to_source_map=None,
+    out_rm_nan=0,
+    target_as_input=0,
+    constant_only=0,
+    gage_id_screen=None,
+    loss_param=None,
+    metrics=None,
+    fill_nan=None,
+    explainer=None,
+    rolling=None,
+    long_seq_pred=None,
+    calc_metrics=None,
+    start_epoch=1,
+    stat_dict_file=None,
+    num_workers=None,
+    which_first_tensor=None,
+    ensemble=0,
+    ensemble_items=None,
+    early_stopping=None,
+    patience=None,
+    min_time_unit=None,
+    min_time_interval=None,
+):
+    """input args from cmd"""
+    parser = argparse.ArgumentParser(
+        description="Train a Time-Series Deep Learning Model for Basins"
+    )
+    parser.add_argument(
+        "--sub", dest="sub", help="subset and sub experiment", default=sub, type=str
+    )
+    parser.add_argument(
+        "--source_cfgs",
+        dest="source_cfgs",
+        help="configs for data sources",
+        default=source_cfgs,
+        type=json.loads,
+    )
+    parser.add_argument(
+        "--scaler",
+        dest="scaler",
+        help="Choose a Scaler function",
+        default=scaler,
+        type=str,
+    )
+    parser.add_argument(
+        "--scaler_params",
+        dest="scaler_params",
+        help="Parameters of the chosen Scaler function",
+        default=scaler_params,
+        type=json.loads,
+    )
+    parser.add_argument(
+        "--dataset",
+        dest="dataset",
+        help="Choose a dataset class for PyTorch",
+        default=dataset,
+        type=str,
+    )
+    parser.add_argument(
+        "--sampler",
+        dest="sampler",
+        help="None or KuaiSampler",
+        default=sampler,
+        type=str,
+    )
+    parser.add_argument(
+        "--fl_sample",
+        dest="fl_sample",
+        help="sampling method for federated learning",
+        default=fl_sample,
+        type=str,
+    )
+    parser.add_argument(
+        "--fl_num_users",
+        dest="fl_num_users",
+        help="number of users for federated learning",
+        default=fl_num_users,
+        type=int,
+    )
+    parser.add_argument(
+        "--fl_local_ep",
+        dest="fl_local_ep",
+        help="number of local epochs for federated learning",
+        default=fl_local_ep,
+        type=int,
+    )
+    parser.add_argument(
+        "--fl_local_bs",
+        dest="fl_local_bs",
+        help="local batch size for federated learning",
+        default=fl_local_bs,
+        type=float,
+    )
+    parser.add_argument(
+        "--fl_frac",
+        dest="fl_frac",
+        help="the fraction of clients for federated learning",
+        default=fl_frac,
+        type=float,
+    )
+    parser.add_argument(
+        "--master_addr",
+        dest="master_addr",
+        help="Running Context --default is localhost if you only train model on your computer",
+        default=master_addr,
+        nargs="+",
+    )
+    parser.add_argument(
+        "--port",
+        dest="port",
+        help="Running Context -- which port do you want to use when using DistributedDataParallel",
+        default=port,
+        nargs="+",
+    )
+    parser.add_argument(
+        "--ctx",
+        dest="ctx",
+        help="Running Context -- gpu num or cpu. E.g `--ctx 0 1` means run code in gpu 0 and 1; -1 means cpu",
+        default=ctx,
+        nargs="+",
+    )
+    parser.add_argument("--rs", dest="rs", help="random seed", default=rs, type=int)
+    # There is something wrong with "bool", so I used 1 as True, 0 as False
+    parser.add_argument(
+        "--train_mode",
+        dest="train_mode",
+        help="If 0, no train or test, just read data; else train + test",
+        default=train_mode,
+        type=int,
+    )
+    parser.add_argument(
+        "--train_epoch",
+        dest="train_epoch",
+        help="epoches of training period",
+        default=train_epoch,
+        type=int,
+    )
+    parser.add_argument(
+        "--save_epoch",
+        dest="save_epoch",
+        help="save for every save_epoch epoches",
+        default=save_epoch,
+        type=int,
+    )
+    parser.add_argument(
+        "--save_iter",
+        dest="save_iter",
+        help="save for every save_iter in save_epoches",
+        default=save_iter,
+        type=int,
+    )
+    parser.add_argument(
+        "--loss_func",
+        dest="loss_func",
+        help="choose loss function",
+        default=loss_func,
+        type=str,
+    )
+    parser.add_argument(
+        "--loss_param",
+        dest="loss_param",
+        help="choose parameters of loss function",
+        default=loss_param,
+        type=json.loads,
+    )
+    parser.add_argument(
+        "--train_period",
+        dest="train_period",
+        help="The training period",
+        default=train_period,
+        nargs="+",
+    )
+    parser.add_argument(
+        "--valid_period",
+        dest="valid_period",
+        help="The validating period",
+        default=valid_period,
+        nargs="+",
+    )
+    parser.add_argument(
+        "--test_period",
+        dest="test_period",
+        help="The test period",
+        default=test_period,
+        nargs="+",
+    )
+    parser.add_argument(
+        "--batch_size",
+        dest="batch_size",
+        help="batch_size",
+        default=batch_size,
+        type=int,
+    )
+    parser.add_argument(
+        "--dropout",
+        dest="dropout",
+        help="dropout",
+        default=dropout,
+        type=float,
+    )
+    parser.add_argument(
+        "--warmup_length",
+        dest="warmup_length",
+        help="Physical hydro models need warmup",
+        default=warmup_length,
+        type=int,
+    )
+    parser.add_argument(
+        "--forecast_history",
+        dest="forecast_history",
+        help="length of time sequence when training in encoder part, for decoder-only models, forecast_history=0",
+        default=forecast_history,
+        type=int,
+    )
+    parser.add_argument(
+        "--forecast_length",
+        dest="forecast_length",
+        help="length of time sequence when training in decoder part",
+        default=forecast_length,
+        type=int,
+    )
+    parser.add_argument(
+        "--model_type",
+        dest="model_type",
+        help="The type of DL model",
+        default=model_type,
+        type=str,
+    )
+    parser.add_argument(
+        "--model_name",
+        dest="model_name",
+        help="The name of DL model. now in the zoo",
+        default=model_name,
+        type=str,
+    )
+    parser.add_argument(
+        "--weight_path",
+        dest="weight_path",
+        help="The weights of trained model",
+        default=weight_path,
+        type=str,
+    )
+    parser.add_argument(
+        "--weight_path_add",
+        dest="weight_path_add",
+        help="More info about the weights of trained model",
+        default=weight_path_add,
+        type=json.loads,
+    )
+    parser.add_argument(
+        "--continue_train",
+        dest="continue_train",
+        help="Continue to train the model from weight_path when continue_train>0",
+        default=continue_train,
+        type=int,
+    )
+    parser.add_argument(
+        "--gage_id",
+        dest="gage_id",
+        help="just select some sites",
+        default=gage_id,
+        nargs="+",
+    )
+    parser.add_argument(
+        "--gage_id_screen",
+        dest="gage_id_screen",
+        help="the criterion to chose some gages",
+        default=gage_id_screen,
+        type=json.loads,
+    )
+    parser.add_argument(
+        "--gage_id_file",
+        dest="gage_id_file",
+        help="choose some sites from a file",
+        default=gage_id_file,
+        type=str,
+    )
+    parser.add_argument(
+        "--opt", dest="opt", help="choose an optimizer", default=opt, type=str
+    )
+    parser.add_argument(
+        "--opt_param",
+        dest="opt_param",
+        help="the optimizer parameters",
+        default=opt_param,
+        type=json.loads,
+    )
+    parser.add_argument(
+        "--var_c", dest="var_c", help="types of attributes", default=var_c, nargs="+"
+    )
+    parser.add_argument(
+        "--c_rm_nan",
+        dest="c_rm_nan",
+        help="if true, we remove NaN value for var_c data when scaling",
+        default=c_rm_nan,
+        type=int,
+    )
+    parser.add_argument(
+        "--var_t", dest="var_t", help="types of forcing", default=var_t, nargs="+"
+    )
+    parser.add_argument(
+        "--t_rm_nan",
+        dest="t_rm_nan",
+        help="if true, we remove NaN value for var_t data when scaling",
+        default=t_rm_nan,
+        type=int,
+    )
+    parser.add_argument(
+        "--var_t_type",
+        dest="var_t_type",
+        help="types of forcing data_source",
+        default=var_t_type,
+        nargs="+",
+    )
+    parser.add_argument(
+        "--var_o",
+        dest="var_o",
+        help="more other inputs except for var_c and var_t",
+        default=var_o,
+        type=json.loads,
+    )
+    parser.add_argument(
+        "--var_out", dest="var_out", help="type of outputs", default=var_out, nargs="+"
+    )
+    parser.add_argument(
+        "--var_to_source_map",
+        dest="var_to_source_map",
+        help="var_to_source_map",
+        default=var_to_source_map,
+        type=json.loads,
+    )
+    parser.add_argument(
+        "--out_rm_nan",
+        dest="out_rm_nan",
+        help="if true, we remove NaN value for var_out data when scaling",
+        default=out_rm_nan,
+        type=int,
+    )
+    parser.add_argument(
+        "--target_as_input",
+        dest="target_as_input",
+        help="if true, we will use target data as input for data assimilation or physics-based models",
+        default=target_as_input,
+        type=int,
+    )
+    parser.add_argument(
+        "--constant_only",
+        dest="constant_only",
+        help="if true, we will only use attribute data as input for deep learning models; "
+        "now it is only for dpl models and it is only used when target_as_input is False",
+        default=constant_only,
+        type=int,
+    )
+    parser.add_argument(
+        "--n_output",
+        dest="n_output",
+        help="the number of output features",
+        default=n_output,
+        type=int,
+    )
+    parser.add_argument(
+        "--model_hyperparam",
+        dest="model_hyperparam",
+        help="the model_hyperparam in model_cfgs",
+        default=model_hyperparam,
+        type=json.loads,
+    )
+    parser.add_argument(
+        "--metrics",
+        dest="metrics",
+        help="The evaluating metrics",
+        default=metrics,
+        nargs="+",
+    )
+    parser.add_argument(
+        "--fill_nan",
+        dest="fill_nan",
+        help="how to fill nan values when evaluating",
+        default=fill_nan,
+        nargs="+",
+    )
+    parser.add_argument(
+        "--explainer",
+        dest="explainer",
+        help="explainer what when evaluating",
+        default=explainer,
+        nargs="+",
+    )
+    parser.add_argument(
+        "--rolling",
+        dest="rolling",
+        help="if False, evaluate 1-period output with a rolling window",
+        default=rolling,
+        type=bool,
+    )
+    parser.add_argument(
+        "--model_loader",
+        dest="model_loader",
+        help="the way to load weights of trained model",
+        default=model_loader,
+        type=int,
+    )
+    parser.add_argument(
+        "--long_seq_pred",
+        dest="long_seq_pred",
+        help="if True, direct, one-step, long-term sequence prediction",
+        default=long_seq_pred,
+        type=bool,
+    )
+    parser.add_argument(
+        "--calc_metrics",
+        dest="calc_metrics",
+        help="if False, calculate valid loss only",
+        default=calc_metrics,
+        type=bool,
+    )
+    parser.add_argument(
+        "--start_epoch",
+        dest="start_epoch",
+        help="The index of epoch when starting training, default is 1. "
+        "When retraining after an interrupt, it will be larger than 1",
+        default=start_epoch,
+        type=int,
+    )
+    parser.add_argument(
+        "--stat_dict_file",
+        dest="stat_dict_file",
+        help="for testing sometimes such as pub cases, we need stat_dict_file from trained dataset",
+        default=stat_dict_file,
+        type=str,
+    )
+    parser.add_argument(
+        "--num_workers",
+        dest="num_workers",
+        help="The number of workers used in Dataloader",
+        default=num_workers,
+        type=int,
+    )
+    parser.add_argument(
+        "--which_first_tensor",
+        dest="which_first_tensor",
+        help="sequence_first or batch_first",
+        default=which_first_tensor,
+        type=str,
+    )
+    parser.add_argument(
+        "--lr_scheduler",
+        dest="lr_scheduler",
+        help="The learning rate scheduler",
+        default=lr_scheduler,
+        type=json.loads,
+    )
+    parser.add_argument(
+        "--ensemble",
+        dest="ensemble",
+        help="ensemble config",
+        default=ensemble,
+        type=int,
+    )
+    parser.add_argument(
+        "--ensemble_items",
+        dest="ensemble_items",
+        help="ensemble config",
+        default=ensemble_items,
+        type=json.loads,
+    )
+    parser.add_argument(
+        "--early_stopping",
+        dest="early_stopping",
+        help="early_stopping config",
+        default=early_stopping,
+        type=bool,
+    )
+    parser.add_argument(
+        "--patience",
+        dest="patience",
+        help="patience config",
+        default=patience,
+        type=int,
+    )
+    parser.add_argument(
+        "--min_time_unit",
+        dest="min_time_unit",
+        help="The min time type of the input data",
+        default=min_time_unit,
+        type=str,
+    )
+    parser.add_argument(
+        "--min_time_interval",
+        dest="min_time_interval",
+        help="The min time interval of the input data",
+        default=min_time_interval,
+        type=int,
+    )
+    # To make pytest work in PyCharm, here we use the following code instead of "args = parser.parse_args()":
+    # https://blog.csdn.net/u014742995/article/details/100119905
+    args, unknown = parser.parse_known_args()
+    return args
+
+
+def update_nested_dict(d, keys, value):
+    """update nested dict
+
+    Parameters
+    ----------
+    d
+        the dict to be updated
+    keys
+        the keys of the dict
+    value
+        the updated value of the dict
+    """
+    if len(keys) == 1:
+        d[keys[0]] = value
+    else:
+        update_nested_dict(d[keys[0]], keys[1:], value)
+
+
+def update_cfg(cfg_file, new_args):
+    """
+    Update default config with new arguments
+
+    Parameters
+    ----------
+    cfg_file
+        default config
+    new_args
+        new arguments
+
+    Returns
+    -------
+    None
+        in-place operation for cfg_file
+    """
+    print("update config file")
+    project_dir = os.getcwd()
+    result_dir = os.path.join(project_dir, "results")
+    if os.path.exists(result_dir) is False:
+        os.makedirs(result_dir)
+    if new_args.sub is not None:
+        subset, subexp = new_args.sub.split(os.sep)
+        cfg_file["data_cfgs"]["validation_path"] = os.path.join(
+            project_dir, "results", subset, subexp
+        )
+        cfg_file["data_cfgs"]["test_path"] = os.path.join(result_dir, subset, subexp)
+    if new_args.source_cfgs is not None:
+        cfg_file["data_cfgs"]["source_cfgs"] = new_args.source_cfgs
+    if new_args.scaler is not None:
+        cfg_file["data_cfgs"]["scaler"] = new_args.scaler
+    if new_args.scaler_params is not None:
+        cfg_file["data_cfgs"]["scaler_params"] = new_args.scaler_params
+    if new_args.dataset is not None:
+        cfg_file["data_cfgs"]["dataset"] = new_args.dataset
+    if new_args.sampler is not None:
+        cfg_file["data_cfgs"]["sampler"] = new_args.sampler
+    if new_args.fl_sample is not None:
+        if new_args.fl_sample not in ["basin", "region"]:
+            # basin means each client is a basin
+            raise ValueError("fl_sample must be 'basin' or 'region'")
+        cfg_file["model_cfgs"]["fl_hyperparam"]["fl_sample"] = new_args.fl_sample
+    if new_args.fl_num_users is not None:
+        cfg_file["model_cfgs"]["fl_hyperparam"]["fl_num_users"] = new_args.fl_num_users
+    if new_args.fl_local_ep is not None:
+        cfg_file["model_cfgs"]["fl_hyperparam"]["fl_local_ep"] = new_args.fl_local_ep
+    if new_args.fl_local_bs is not None:
+        cfg_file["model_cfgs"]["fl_hyperparam"]["fl_local_bs"] = new_args.fl_local_bs
+    if new_args.fl_frac is not None:
+        cfg_file["model_cfgs1"]["fl_hyperparam"]["fl_frac"] = new_args.fl_frac
+    if new_args.master_addr is not None:
+        cfg_file["training_cfgs"]["master_addr"] = new_args.master_addr
+    if new_args.port is not None:
+        cfg_file["training_cfgs"]["port"] = new_args.port
+    if new_args.ctx is not None:
+        cfg_file["training_cfgs"]["device"] = new_args.ctx
+    if new_args.rs is not None:
+        cfg_file["training_cfgs"]["random_seed"] = new_args.rs
+    if new_args.train_mode is not None:
+        cfg_file["training_cfgs"]["train_mode"] = bool(new_args.train_mode > 0)
+    if new_args.loss_func is not None:
+        cfg_file["training_cfgs"]["criterion"] = new_args.loss_func
+        if new_args.loss_param is not None:
+            cfg_file["training_cfgs"]["criterion_params"] = new_args.loss_param
+    if new_args.train_period is not None:
+        cfg_file["data_cfgs"]["t_range_train"] = new_args.train_period
+    if new_args.valid_period is not None:
+        cfg_file["data_cfgs"]["t_range_valid"] = new_args.valid_period
+    if new_args.test_period is not None:
+        cfg_file["data_cfgs"]["t_range_test"] = new_args.test_period
+    if (
+        new_args.gage_id is not None
+        and new_args.gage_id_file is not None
+        or new_args.gage_id is None
+        and new_args.gage_id_file is not None
+    ):
+        gage_id_lst = (
+            pd.read_csv(new_args.gage_id_file, dtype={0: str}).iloc[:, 0].values
+        )
+        cfg_file["data_cfgs"]["object_ids"] = gage_id_lst.tolist()
+    elif new_args.gage_id is not None:
+        cfg_file["data_cfgs"]["object_ids"] = new_args.gage_id
+    if new_args.opt is not None:
+        cfg_file["training_cfgs"]["optimizer"] = new_args.opt
+        if new_args.opt_param is not None:
+            cfg_file["training_cfgs"]["optim_params"] = new_args.opt_param
+        else:
+            cfg_file["training_cfgs"]["optim_params"] = {}
+    if new_args.var_c is not None:
+        # I don't find a method to receive empty list for argparse, so if we input "None" or "" or " ", we treat it as []
+        if (
+            new_args.var_c == ["None"]
+            or new_args.var_c == [""]
+            or new_args.var_c == [" "]
+        ):
+            cfg_file["data_cfgs"]["constant_cols"] = []
+        else:
+            cfg_file["data_cfgs"]["constant_cols"] = new_args.var_c
+    cfg_file["data_cfgs"]["constant_rm_nan"] = bool(new_args.c_rm_nan != 0)
+    if new_args.var_t is not None:
+        cfg_file["data_cfgs"]["relevant_cols"] = new_args.var_t
+    if new_args.var_t_type is not None:
+        cfg_file["data_cfgs"]["relevant_types"] = new_args.var_t_type
+    cfg_file["data_cfgs"]["relevant_rm_nan"] = bool(new_args.t_rm_nan != 0)
+    if new_args.var_o is not None:
+        cfg_file["data_cfgs"]["other_cols"] = new_args.var_o
+    if new_args.var_out is not None:
+        cfg_file["data_cfgs"]["target_cols"] = new_args.var_out
+    if new_args.var_to_source_map is not None:
+        cfg_file["data_cfgs"]["var_to_source_map"] = new_args.var_to_source_map
+    cfg_file["data_cfgs"]["target_rm_nan"] = bool(new_args.out_rm_nan != 0)
+    if new_args.target_as_input == 0:
+        cfg_file["data_cfgs"]["target_as_input"] = False
+        if new_args.constant_only == 0:
+            cfg_file["data_cfgs"]["constant_only"] = False
+        else:
+            cfg_file["data_cfgs"]["constant_only"] = True
+    else:
+        cfg_file["data_cfgs"]["target_as_input"] = True
+    if new_args.long_seq_pred is not None:
+        cfg_file["evaluation_cfgs"]["long_seq_pred"] = new_args.long_seq_pred
+    if new_args.calc_metrics is not None:
+        cfg_file["evaluation_cfgs"]["calc_metrics"] = new_args.calc_metrics
+    if new_args.train_epoch is not None:
+        cfg_file["training_cfgs"]["epochs"] = new_args.train_epoch
+    if new_args.save_epoch is not None:
+        cfg_file["training_cfgs"]["save_epoch"] = new_args.save_epoch
+    if new_args.save_iter is not None:
+        cfg_file["training_cfgs"]["save_iter"] = new_args.save_iter
+    if new_args.model_type is not None:
+        cfg_file["model_cfgs"]["model_type"] = new_args.model_type
+    if new_args.model_name is not None:
+        cfg_file["model_cfgs"]["model_name"] = new_args.model_name
+    if new_args.weight_path is not None:
+        cfg_file["model_cfgs"]["weight_path"] = new_args.weight_path
+        if new_args.continue_train is None or new_args.continue_train == 0:
+            continue_train = False
+        else:
+            continue_train = True
+        cfg_file["model_cfgs"]["continue_train"] = continue_train
+    if new_args.weight_path_add is not None:
+        cfg_file["model_cfgs"]["weight_path_add"] = new_args.weight_path_add
+    if new_args.n_output is not None:
+        cfg_file["training_cfgs"]["multi_targets"] = new_args.n_output
+        if len(cfg_file["data_cfgs"]["target_cols"]) != new_args.n_output:
+            raise AttributeError(
+                "Please make sure size of vars in data_cfgs/target_cols is same as n_output"
+            )
+    if new_args.model_hyperparam is None:
+        raise AttributeError("Please set the model_hyperparam!!!")
+    else:
+        cfg_file["model_cfgs"]["model_hyperparam"] = new_args.model_hyperparam
+        if "batch_size" in new_args.model_hyperparam.keys():
+            cfg_file["data_cfgs"]["batch_size"] = new_args.model_hyperparam[
+                "batch_size"
+            ]
+            cfg_file["training_cfgs"]["batch_size"] = new_args.model_hyperparam[
+                "batch_size"
+            ]
+        if "forecast_length" in new_args.model_hyperparam.keys():
+            cfg_file["data_cfgs"]["forecast_length"] = new_args.model_hyperparam[
+                "forecast_length"
+            ]
+        if "prec_window" in new_args.model_hyperparam.keys():
+            cfg_file["data_cfgs"]["prec_window"] = new_args.model_hyperparam[
+                "prec_window"
+            ]
+    if new_args.batch_size is None:
+        raise AttributeError("Please set the batch_size!!!")
+    if new_args.batch_size is not None:
+        batch_size = new_args.batch_size
+        cfg_file["data_cfgs"]["batch_size"] = batch_size
+        cfg_file["training_cfgs"]["batch_size"] = batch_size
+    if new_args.min_time_unit is not None:
+        if new_args.min_time_unit not in ["h", "D"]:
+            raise ValueError("min_time_unit must be 'h' (HOURLY) or 'D' (DAILY)")
+        cfg_file["data_cfgs"]["min_time_unit"] = new_args.min_time_unit
+    if new_args.min_time_interval is not None:
+        cfg_file["data_cfgs"]["min_time_interval"] = new_args.min_time_interval
+    if new_args.metrics is not None:
+        cfg_file["evaluation_cfgs"]["metrics"] = new_args.metrics
+    if new_args.fill_nan is not None:
+        cfg_file["evaluation_cfgs"]["fill_nan"] = new_args.fill_nan
+    if new_args.explainer is not None:
+        cfg_file["evaluation_cfgs"]["explainer"] = new_args.explainer
+    if new_args.rolling is not None:
+        cfg_file["evaluation_cfgs"]["rolling"] = new_args.rolling
+    if new_args.model_loader is not None:
+        cfg_file["evaluation_cfgs"]["model_loader"] = new_args.model_loader
+    if new_args.warmup_length > 0:
+        cfg_file["data_cfgs"]["warmup_length"] = new_args.warmup_length
+        if "warmup_length" in new_args.model_hyperparam.keys() and (
+            not cfg_file["data_cfgs"]["warmup_length"]
+            == new_args.model_hyperparam["warmup_length"]
+        ):
+            raise RuntimeError(
+                "Please set same warmup_length in model_cfgs and data_cfgs"
+            )
+    if new_args.forecast_history is not None:
+        cfg_file["data_cfgs"]["forecast_history"] = new_args.forecast_history
+    if new_args.forecast_length is not None:
+        cfg_file["data_cfgs"]["forecast_length"] = new_args.forecast_length
+    if new_args.start_epoch > 1:
+        cfg_file["training_cfgs"]["start_epoch"] = new_args.start_epoch
+    if new_args.stat_dict_file is not None:
+        cfg_file["data_cfgs"]["stat_dict_file"] = new_args.stat_dict_file
+    if new_args.num_workers is not None and new_args.num_workers > 0:
+        cfg_file["training_cfgs"]["num_workers"] = new_args.num_workers
+    if new_args.which_first_tensor is not None:
+        cfg_file["training_cfgs"]["which_first_tensor"] = new_args.which_first_tensor
+    if new_args.ensemble == 0:
+        cfg_file["training_cfgs"]["ensemble"] = False
+    else:
+        cfg_file["training_cfgs"]["ensemble"] = True
+    if new_args.ensemble_items is not None:
+        cfg_file["training_cfgs"]["ensemble_items"] = new_args.ensemble_items
+    if new_args.patience is not None:
+        cfg_file["training_cfgs"]["patience"] = new_args.patience
+    if new_args.early_stopping is not None:
+        cfg_file["training_cfgs"]["early_stopping"] = new_args.early_stopping
+    if new_args.lr_scheduler is not None:
+        cfg_file["training_cfgs"]["lr_scheduler"] = new_args.lr_scheduler
+    # print("the updated config:\n", json.dumps(cfg_file, indent=4, ensure_ascii=False))
+
+
+def get_config_file(cfg_dir):
+    json_files_lst = []
+    json_files_ctime = []
+    for file in os.listdir(cfg_dir):
+        if (
+            fnmatch.fnmatch(file, "*.json")
+            and "_stat" not in file  # statistics json file
+            and "_dict" not in file  # data cache json file
+        ):
+            json_files_lst.append(os.path.join(cfg_dir, file))
+            json_files_ctime.append(os.path.getctime(os.path.join(cfg_dir, file)))
+    sort_idx = np.argsort(json_files_ctime)
+    cfg_file = json_files_lst[sort_idx[-1]]
+    return hydro_file.unserialize_json(cfg_file)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `torchhydro-0.0.4/torchhydro/datasets/data_scalers.py` & `torchhydro-0.0.5/torchhydro/datasets/data_scalers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,433 +1,490 @@
-import copy
-import json
-import os
-import pickle as pkl
-import shutil
-import pint_xarray  # noqa: F401
-import xarray as xr
-from hydrodataset import HydroDataset
-import numpy as np
-from sklearn.preprocessing import (
-    StandardScaler,
-    RobustScaler,
-    MinMaxScaler,
-    MaxAbsScaler,
-)
-
-from hydroutils.hydro_stat import (
-    cal_stat_prcp_norm,
-    cal_stat_gamma,
-    cal_stat,
-)
-
-from torchhydro.datasets.data_utils import (
-    _trans_norm,
-    _prcp_norm,
-    wrap_t_s_dict,
-    unify_streamflow_unit,
-)
-
-SCALER_DICT = {
-    "StandardScaler": StandardScaler,
-    "RobustScaler": RobustScaler,
-    "MinMaxScaler": MinMaxScaler,
-    "MaxAbsScaler": MaxAbsScaler,
-}
-
-
-class ScalerHub(object):
-    """
-    A class for Scaler
-    """
-
-    def __init__(
-        self,
-        target_vars: np.array,
-        relevant_vars: np.array,
-        constant_vars: np.array = None,
-        data_cfgs: dict = None,
-        is_tra_val_te: str = None,
-        **kwargs,
-    ):
-        """
-        Perform normalization
-
-        Parameters
-        ----------
-        target_vars
-            output variables
-        relevant_vars
-            dynamic input variables
-        constant_vars
-            static input variables
-        other_vars
-            other required variables
-        data_cfgs
-            configs for reading data
-        is_tra_val_te
-            train, valid or test
-        kwargs
-            other optional parameters for ScalerHub
-        """
-        self.data_cfgs = data_cfgs
-        norm_keys = ["target_vars", "relevant_vars", "constant_vars"]
-        norm_dict = {}
-        scaler_type = data_cfgs["scaler"]
-        if scaler_type == "DapengScaler":
-            assert "data_source" in list(kwargs.keys())
-            gamma_norm_cols = data_cfgs["scaler_params"]["gamma_norm_cols"]
-            prcp_norm_cols = data_cfgs["scaler_params"]["prcp_norm_cols"]
-            pbm_norm = data_cfgs["scaler_params"]["pbm_norm"]
-            scaler = DapengScaler(
-                target_vars,
-                relevant_vars,
-                constant_vars,
-                data_cfgs,
-                is_tra_val_te,
-                kwargs["data_source"],
-                prcp_norm_cols=prcp_norm_cols,
-                gamma_norm_cols=gamma_norm_cols,
-                pbm_norm=pbm_norm,
-            )
-            x, y, c = scaler.load_data()
-            self.target_scaler = scaler
-        elif scaler_type in SCALER_DICT.keys():
-            # TODO: not fully tested, espacially for pbm models
-            all_vars = [target_vars, relevant_vars, constant_vars]
-            for i in range(len(all_vars)):
-                data_tmp = all_vars[i]
-                scaler = SCALER_DICT[scaler_type]()
-                if data_tmp.ndim == 3:
-                    # for forcings and outputs
-                    num_instances, num_time_steps, num_features = data_tmp.shape
-                    data_tmp = data_tmp.to_numpy().reshape(-1, num_features)
-                    save_file = os.path.join(
-                        data_cfgs["test_path"], f"{norm_keys[i]}_scaler.pkl"
-                    )
-                    if is_tra_val_te == "train" and data_cfgs["stat_dict_file"] is None:
-                        data_norm = scaler.fit_transform(data_tmp)
-                        # Save scaler in test_path for valid/test
-                        with open(save_file, "wb") as outfile:
-                            pkl.dump(scaler, outfile)
-                    else:
-                        if data_cfgs["stat_dict_file"] is not None:
-                            shutil.copy(data_cfgs["stat_dict_file"], save_file)
-                        if not os.path.isfile(save_file):
-                            raise FileNotFoundError(
-                                "Please genereate xx_scaler.pkl file"
-                            )
-                        with open(save_file, "rb") as infile:
-                            scaler = pkl.load(infile)
-                            data_norm = scaler.transform(data_tmp)
-                    data_norm = data_norm.reshape(
-                        num_instances, num_time_steps, num_features
-                    )
-                else:
-                    # for attributes
-                    save_file = os.path.join(
-                        data_cfgs["test_path"], f"{norm_keys[i]}_scaler.pkl"
-                    )
-                    if is_tra_val_te == "train" and data_cfgs["stat_dict_file"] is None:
-                        data_norm = scaler.fit_transform(data_tmp)
-                        # Save scaler in test_path for valid/test
-                        with open(save_file, "wb") as outfile:
-                            pkl.dump(scaler, outfile)
-                    else:
-                        if data_cfgs["stat_dict_file"] is not None:
-                            shutil.copy(data_cfgs["stat_dict_file"], save_file)
-                        assert os.path.isfile(save_file)
-                        with open(save_file, "rb") as infile:
-                            scaler = pkl.load(infile)
-                            data_norm = scaler.transform(data_tmp)
-                norm_dict[norm_keys[i]] = data_norm
-                if i == 0:
-                    self.target_scaler = scaler
-            x = norm_dict["relevant_vars"]
-            y = norm_dict["target_vars"]
-            c = norm_dict["constant_vars"]
-        else:
-            raise NotImplementedError(
-                "We don't provide this Scaler now!!! Please choose another one: DapengScaler or key in SCALER_DICT"
-            )
-        print("Finish Normalization\n")
-        self.x = x
-        self.y = y
-        self.c = c
-
-
-class DapengScaler(object):
-    def __init__(
-        self,
-        target_vars: np.array,
-        relevant_vars: np.array,
-        constant_vars: np.array,
-        data_cfgs: dict,
-        is_tra_val_te: str,
-        data_source: HydroDataset,
-        other_vars: dict = None,
-        prcp_norm_cols=None,
-        gamma_norm_cols=None,
-        pbm_norm=False,
-    ):
-        """
-        The normalization and denormalization methods from Dapeng's 1st WRR paper.
-        Some use StandardScaler, and some use special norm methods
-
-        Parameters
-        ----------
-        target_vars
-            output variables
-        relevant_vars
-            input dynamic variables
-        constant_vars
-            input static variables
-        data_cfgs
-            data parameter config in data source
-        is_tra_val_te
-            train/valid/test
-        data_source
-            all config about data source
-        other_vars
-            if more input are needed, list them in other_vars
-        prcp_norm_cols
-            data items which use _prcp_norm method to normalize
-        gamma_norm_cols
-            data items which use log(\sqrt(x)+.1) method to normalize
-        pbm_norm
-            if true, use pbm_norm method to normalize; the output of pbms is not normalized data, so its inverse is different.
-        """
-        if prcp_norm_cols is None:
-            prcp_norm_cols = [
-                "streamflow",
-            ]
-        if gamma_norm_cols is None:
-            gamma_norm_cols = [
-                "prcp",
-                "pr",
-                "total_precipitation",
-                "pet",
-                "potential_evaporation",
-                "PET",
-            ]
-        self.data_target = target_vars
-        self.data_forcing = relevant_vars
-        self.data_attr = constant_vars
-        self.data_source = data_source
-        self.data_cfgs = data_cfgs
-        self.t_s_dict = wrap_t_s_dict(data_source, data_cfgs, is_tra_val_te)
-        self.data_other = other_vars
-        self.prcp_norm_cols = prcp_norm_cols
-        self.gamma_norm_cols = gamma_norm_cols
-        # both prcp_norm_cols and gamma_norm_cols use log(\sqrt(x)+.1) method to normalize
-        self.log_norm_cols = gamma_norm_cols + prcp_norm_cols
-        self.pbm_norm = pbm_norm
-        # save stat_dict of training period in test_path for valid/test
-        stat_file = os.path.join(data_cfgs["test_path"], "dapengscaler_stat.json")
-        # for testing sometimes such as pub cases, we need stat_dict_file from trained dataset
-        if is_tra_val_te == "train" and data_cfgs["stat_dict_file"] is None:
-            self.stat_dict = self.cal_stat_all()
-            with open(stat_file, "w") as fp:
-                json.dump(self.stat_dict, fp)
-        else:
-            # for valid/test, we need to load stat_dict from train
-            if data_cfgs["stat_dict_file"] is not None:
-                # we used a assigned stat file, typically for PUB exps
-                shutil.copy(data_cfgs["stat_dict_file"], stat_file)
-            assert os.path.isfile(stat_file)
-            with open(stat_file, "r") as fp:
-                self.stat_dict = json.load(fp)
-
-    def inverse_transform(self, target_values):
-        """
-        Denormalization for output variables
-
-        Parameters
-        ----------
-        target_values
-            output variables
-
-        Returns
-        -------
-        np.array
-            denormalized predictions
-        """
-        stat_dict = self.stat_dict
-        target_cols = self.data_cfgs["target_cols"]
-        if self.pbm_norm:
-            # for pbm's output, its unit is mm/day, so we don't need to recover its unit
-            pred = target_values
-        else:
-            pred = _trans_norm(
-                target_values,
-                target_cols,
-                stat_dict,
-                log_norm_cols=self.log_norm_cols,
-                to_norm=False,
-            )
-            for i in range(len(self.data_cfgs["target_cols"])):
-                var = self.data_cfgs["target_cols"][i]
-                if var in self.prcp_norm_cols:
-                    mean_prep = self.data_source.read_mean_prcp(
-                        self.t_s_dict["sites_id"]
-                    )
-                    pred.loc[dict(variable=var)] = _prcp_norm(
-                        pred.sel(variable=var).to_numpy(),
-                        mean_prep.to_array().to_numpy().T,
-                        to_norm=False,
-                    )
-        # add attrs for units
-        pred.attrs.update(self.data_target.attrs)
-        # trans to xarray dataset
-        pred_ds = pred.to_dataset(dim="variable")
-        pred_ds = pred_ds.pint.quantify(pred_ds.attrs["units"])
-        area = self.data_source.read_area(self.t_s_dict["sites_id"])
-        return unify_streamflow_unit(pred_ds, area=area, inverse=True)
-
-    def cal_stat_all(self):
-        """
-        Calculate statistics of outputs(streamflow etc), and inputs(forcing and attributes)
-
-        Returns
-        -------
-        dict
-            a dict with statistic values
-        """
-        # streamflow
-        target_cols = self.data_cfgs["target_cols"]
-        stat_dict = {}
-        for i in range(len(target_cols)):
-            var = target_cols[i]
-            if var in self.prcp_norm_cols:
-                mean_prep = self.data_source.read_mean_prcp(self.t_s_dict["sites_id"])
-                stat_dict[var] = cal_stat_prcp_norm(
-                    self.data_target.sel(variable=var).to_numpy(),
-                    mean_prep.to_array().to_numpy().T,
-                )
-            elif var in self.gamma_norm_cols:
-                stat_dict[var] = cal_stat_gamma(
-                    self.data_target.sel(variable=var).to_numpy()
-                )
-            else:
-                stat_dict[var] = cal_stat(self.data_target.sel(variable=var).to_numpy())
-
-        # forcing
-        forcing_lst = self.data_cfgs["relevant_cols"]
-        x = self.data_forcing
-        for k in range(len(forcing_lst)):
-            var = forcing_lst[k]
-            if var in self.gamma_norm_cols:
-                stat_dict[var] = cal_stat_gamma(x.sel(variable=var).to_numpy())
-            else:
-                stat_dict[var] = cal_stat(x.sel(variable=var).to_numpy())
-
-        # const attribute
-        attr_data = self.data_attr
-        attr_lst = self.data_cfgs["constant_cols"]
-        for k in range(len(attr_lst)):
-            var = attr_lst[k]
-            stat_dict[var] = cal_stat(attr_data.sel(variable=var).to_numpy())
-
-        return stat_dict
-
-    def get_data_obs(self, to_norm: bool = True) -> np.array:
-        """
-        Get observation values
-
-        Parameters
-        ----------
-        rm_nan
-            if true, fill NaN value with 0
-        to_norm
-            if true, perform normalization
-
-        Returns
-        -------
-        np.array
-            the output value for modeling
-        """
-        stat_dict = self.stat_dict
-        data = self.data_target
-        out = xr.full_like(data, np.nan)
-        # if we don't set a copy() here, the attrs of data will be changed, which is not our wish
-        out.attrs = copy.deepcopy(data.attrs)
-        target_cols = self.data_cfgs["target_cols"]
-        for i in range(len(target_cols)):
-            var = target_cols[i]
-            if var in self.prcp_norm_cols:
-                mean_prep = self.data_source.read_mean_prcp(self.t_s_dict["sites_id"])
-                out.loc[dict(variable=var)] = _prcp_norm(
-                    data.sel(variable=var).to_numpy(),
-                    mean_prep.to_array().to_numpy().T,
-                    to_norm=True,
-                )
-                out.attrs["units"][var] = "dimensionless"
-        out = _trans_norm(
-            out,
-            target_cols,
-            stat_dict,
-            log_norm_cols=self.log_norm_cols,
-            to_norm=to_norm,
-        )
-        return out
-
-    def get_data_ts(self, to_norm=True) -> np.array:
-        """
-        Get dynamic input data
-
-        Parameters
-        ----------
-        rm_nan
-            if true, fill NaN value with 0
-        to_norm
-            if true, perform normalization
-
-        Returns
-        -------
-        np.array
-            the dynamic inputs for modeling
-        """
-        stat_dict = self.stat_dict
-        var_lst = self.data_cfgs["relevant_cols"]
-        data = self.data_forcing
-        data = _trans_norm(
-            data, var_lst, stat_dict, log_norm_cols=self.log_norm_cols, to_norm=to_norm
-        )
-        return data
-
-    def get_data_const(self, to_norm=True) -> np.array:
-        """
-        Attr data and normalization
-
-        Parameters
-        ----------
-        rm_nan
-            if true, fill NaN value with 0
-        to_norm
-            if true, perform normalization
-
-        Returns
-        -------
-        np.array
-            the static inputs for modeling
-        """
-        stat_dict = self.stat_dict
-        var_lst = self.data_cfgs["constant_cols"]
-        data = self.data_attr
-        data = _trans_norm(data, var_lst, stat_dict, to_norm=to_norm)
-        return data
-
-    def load_data(self):
-        """
-        Read data and perform normalization for DL models
-
-        Returns
-        -------
-        tuple
-            x: 3-d  gages_num*time_num*var_num
-            y: 3-d  gages_num*time_num*1
-            c: 2-d  gages_num*var_num
-        """
-        x = self.get_data_ts()
-        y = self.get_data_obs()
-        c = self.get_data_const()
-        return x, y, c
+"""
+Author: Wenyu Ouyang
+Date: 2024-04-08 18:17:44
+LastEditTime: 2024-05-27 14:50:10
+LastEditors: Wenyu Ouyang
+Description: normalize the data
+FilePath: \torchhydro\torchhydro\datasets\data_scalers.py
+Copyright (c) 2024-2024 Wenyu Ouyang. All rights reserved.
+"""
+
+import copy
+import json
+import os
+import pickle as pkl
+import shutil
+import pint_xarray  # noqa: F401
+import xarray as xr
+import numpy as np
+from shutil import SameFileError
+from sklearn.preprocessing import (
+    StandardScaler,
+    RobustScaler,
+    MinMaxScaler,
+    MaxAbsScaler,
+)
+
+from hydroutils.hydro_stat import (
+    cal_stat_prcp_norm,
+    cal_stat_gamma,
+    cal_stat,
+    cal_4_stat_inds,
+)
+from hydrodatasource.reader.data_source import HydroBasins
+
+from torchhydro.datasets.data_utils import (
+    _trans_norm,
+    _prcp_norm,
+    wrap_t_s_dict,
+    unify_streamflow_unit,
+)
+
+SCALER_DICT = {
+    "StandardScaler": StandardScaler,
+    "RobustScaler": RobustScaler,
+    "MinMaxScaler": MinMaxScaler,
+    "MaxAbsScaler": MaxAbsScaler,
+}
+
+
+class ScalerHub(object):
+    """
+    A class for Scaler
+    """
+
+    def __init__(
+        self,
+        target_vars: np.array,
+        relevant_vars: np.array,
+        constant_vars: np.array = None,
+        data_cfgs: dict = None,
+        is_tra_val_te: str = None,
+        data_source: object = None,
+        **kwargs,
+    ):
+        """
+        Perform normalization
+
+        Parameters
+        ----------
+        target_vars
+            output variables
+        relevant_vars
+            dynamic input variables
+        constant_vars
+            static input variables
+        other_vars
+            other required variables
+        data_cfgs
+            configs for reading data
+        is_tra_val_te
+            train, valid or test
+        kwargs
+            other optional parameters for ScalerHub
+        """
+        self.data_cfgs = data_cfgs
+        norm_keys = ["target_vars", "relevant_vars", "constant_vars"]
+        norm_dict = {}
+        scaler_type = data_cfgs["scaler"]
+        if scaler_type == "DapengScaler":
+            gamma_norm_cols = data_cfgs["scaler_params"]["gamma_norm_cols"]
+            prcp_norm_cols = data_cfgs["scaler_params"]["prcp_norm_cols"]
+            pbm_norm = data_cfgs["scaler_params"]["pbm_norm"]
+            scaler = DapengScaler(
+                target_vars,
+                relevant_vars,
+                constant_vars,
+                data_cfgs,
+                is_tra_val_te,
+                prcp_norm_cols=prcp_norm_cols,
+                gamma_norm_cols=gamma_norm_cols,
+                pbm_norm=pbm_norm,
+                data_source=data_source,
+            )
+            x, y, c = scaler.load_data()
+            self.target_scaler = scaler
+
+        elif scaler_type in SCALER_DICT.keys():
+            # TODO: not fully tested, espacially for pbm models
+            all_vars = [target_vars, relevant_vars, constant_vars]
+            for i in range(len(all_vars)):
+                data_tmp = all_vars[i]
+                scaler = SCALER_DICT[scaler_type]()
+                if data_tmp.ndim == 3:
+                    # for forcings and outputs
+                    num_instances, num_time_steps, num_features = data_tmp.transpose(
+                        "basin", "time", "variable"
+                    ).shape
+                    data_tmp = data_tmp.to_numpy().reshape(-1, num_features)
+                    save_file = os.path.join(
+                        data_cfgs["test_path"], f"{norm_keys[i]}_scaler.pkl"
+                    )
+                    if is_tra_val_te == "train" and data_cfgs["stat_dict_file"] is None:
+                        data_norm = scaler.fit_transform(data_tmp)
+                        # Save scaler in test_path for valid/test
+                        with open(save_file, "wb") as outfile:
+                            pkl.dump(scaler, outfile)
+                    else:
+                        if data_cfgs["stat_dict_file"] is not None:
+                            shutil.copy(data_cfgs["stat_dict_file"], save_file)
+                        if not os.path.isfile(save_file):
+                            raise FileNotFoundError(
+                                "Please genereate xx_scaler.pkl file"
+                            )
+                        with open(save_file, "rb") as infile:
+                            scaler = pkl.load(infile)
+                            data_norm = scaler.transform(data_tmp)
+                    data_norm = data_norm.reshape(
+                        num_instances, num_time_steps, num_features
+                    )
+                else:
+                    # for attributes
+                    save_file = os.path.join(
+                        data_cfgs["test_path"], f"{norm_keys[i]}_scaler.pkl"
+                    )
+                    if is_tra_val_te == "train" and data_cfgs["stat_dict_file"] is None:
+                        data_norm = scaler.fit_transform(data_tmp)
+                        # Save scaler in test_path for valid/test
+                        with open(save_file, "wb") as outfile:
+                            pkl.dump(scaler, outfile)
+                    else:
+                        if data_cfgs["stat_dict_file"] is not None:
+                            shutil.copy(data_cfgs["stat_dict_file"], save_file)
+                        assert os.path.isfile(save_file)
+                        with open(save_file, "rb") as infile:
+                            scaler = pkl.load(infile)
+                            data_norm = scaler.transform(data_tmp)
+                norm_dict[norm_keys[i]] = data_norm
+                if i == 0:
+                    self.target_scaler = scaler
+            x_ = norm_dict["relevant_vars"]
+            y_ = norm_dict["target_vars"]
+            c_ = norm_dict["constant_vars"]
+            # TODO: need more test for real data
+            x = xr.DataArray(
+                x_,
+                coords={
+                    "basin": target_vars.coords["basin"],
+                    "time": target_vars.coords["time"],
+                    "variable": target_vars.coords["variable"],
+                },
+                dims=["basin", "time", "variable"],
+            )
+            y = xr.DataArray(
+                y_,
+                coords={
+                    "basin": relevant_vars.coords["basin"],
+                    "time": relevant_vars.coords["time"],
+                    "variable": relevant_vars.coords["variable"],
+                },
+                dims=["basin", "time", "variable"],
+            )
+            c = xr.DataArray(
+                c_,
+                coords={
+                    "basin": constant_vars.coords["basin"],
+                    "variable": constant_vars.coords["variable"],
+                },
+                dims=["basin", "variable"],
+            )
+        else:
+            raise NotImplementedError(
+                "We don't provide this Scaler now!!! Please choose another one: DapengScaler or key in SCALER_DICT"
+            )
+        print("Finish Normalization\n")
+        self.x = x
+        self.y = y
+        self.c = c
+
+
+class DapengScaler(object):
+    def __init__(
+        self,
+        target_vars: np.array,
+        relevant_vars: np.array,
+        constant_vars: np.array,
+        data_cfgs: dict,
+        is_tra_val_te: str,
+        other_vars: dict = None,
+        prcp_norm_cols=None,
+        gamma_norm_cols=None,
+        pbm_norm=False,
+        data_source: object = None,
+    ):
+        """
+        The normalization and denormalization methods from Dapeng's 1st WRR paper.
+        Some use StandardScaler, and some use special norm methods
+
+        Parameters
+        ----------
+        target_vars
+            output variables
+        relevant_vars
+            input dynamic variables
+        constant_vars
+            input static variables
+        data_cfgs
+            data parameter config in data source
+        is_tra_val_te
+            train/valid/test
+        other_vars
+            if more input are needed, list them in other_vars
+        prcp_norm_cols
+            data items which use _prcp_norm method to normalize
+        gamma_norm_cols
+            data items which use log(\sqrt(x)+.1) method to normalize
+        pbm_norm
+            if true, use pbm_norm method to normalize; the output of pbms is not normalized data, so its inverse is different.
+        """
+        if prcp_norm_cols is None or isinstance(data_source, HydroBasins):
+            prcp_norm_cols = [
+                "streamflow",
+            ]
+        if gamma_norm_cols is None or isinstance(data_source, HydroBasins):
+            gamma_norm_cols = [
+                "gpm_tp",
+                "sta_tp",
+                "total_precipitation_hourly",
+                "temperature_2m",
+                "dewpoint_temperature_2m",
+                "surface_net_solar_radiation",
+                "sm_surface",
+                "sm_rootzone",
+            ]
+        self.data_target = target_vars
+        self.data_forcing = relevant_vars
+        self.data_attr = constant_vars
+        self.data_cfgs = data_cfgs
+        self.t_s_dict = wrap_t_s_dict(data_cfgs, is_tra_val_te)
+        self.data_other = other_vars
+        self.prcp_norm_cols = prcp_norm_cols
+        self.gamma_norm_cols = gamma_norm_cols
+        # both prcp_norm_cols and gamma_norm_cols use log(\sqrt(x)+.1) method to normalize
+        self.log_norm_cols = gamma_norm_cols + prcp_norm_cols
+        self.pbm_norm = pbm_norm
+        self.data_source = data_source
+        # save stat_dict of training period in test_path for valid/test
+        stat_file = os.path.join(data_cfgs["test_path"], "dapengscaler_stat.json")
+        # for testing sometimes such as pub cases, we need stat_dict_file from trained dataset
+        if is_tra_val_te == "train" and data_cfgs["stat_dict_file"] is None:
+            self.stat_dict = self.cal_stat_all()
+            with open(stat_file, "w") as fp:
+                json.dump(self.stat_dict, fp)
+        else:
+            # for valid/test, we need to load stat_dict from train
+            if data_cfgs["stat_dict_file"] is not None:
+                # we used a assigned stat file, typically for PUB exps
+                # shutil.copy(data_cfgs["stat_dict_file"], stat_file)
+                try:
+                    shutil.copy(data_cfgs["stat_dict_file"], stat_file)
+                except SameFileError:
+                    print(
+                        f"源文件和目标文件是同一个文件: {data_cfgs['stat_dict_file']}，跳过复制操作"
+                    )
+                except Exception as e:
+                    print(f"发生错误: {e}")
+            assert os.path.isfile(stat_file)
+            with open(stat_file, "r") as fp:
+                self.stat_dict = json.load(fp)
+
+    @property
+    def mean_prcp(self):
+        return (
+            self.data_source.read_MP(
+                self.t_s_dict["sites_id"],
+                self.data_cfgs["source_cfgs"]["source_path"]["attributes"],
+            ).values.reshape(-1, 1)
+            if isinstance(self.data_source, HydroBasins)
+            else self.data_source.read_mean_prcp(self.t_s_dict["sites_id"])
+            .to_array()
+            .to_numpy()
+            .T  # TODO: check why T is needed
+        )
+
+    def inverse_transform(self, target_values):
+        """
+        Denormalization for output variables
+
+        Parameters
+        ----------
+        target_values
+            output variables
+
+        Returns
+        -------
+        np.array
+            denormalized predictions
+        """
+        stat_dict = self.stat_dict
+        target_cols = self.data_cfgs["target_cols"]
+        if self.pbm_norm:
+            # for pbm's output, its unit is mm/day, so we don't need to recover its unit
+            pred = target_values
+        else:
+            pred = _trans_norm(
+                target_values,
+                target_cols,
+                stat_dict,
+                log_norm_cols=self.log_norm_cols,
+                to_norm=False,
+            )
+            for i in range(len(self.data_cfgs["target_cols"])):
+                var = self.data_cfgs["target_cols"][i]
+                pred.loc[dict(variable=var)] = _prcp_norm(
+                    pred.sel(variable=var).to_numpy(),
+                    self.mean_prcp,
+                    to_norm=False,
+                )
+        # add attrs for units
+        pred.attrs.update(self.data_target.attrs)
+        return pred.to_dataset(dim="variable")
+
+    def cal_stat_all(self):
+        """
+        Calculate statistics of outputs(streamflow etc), and inputs(forcing and attributes)
+
+        Returns
+        -------
+        dict
+            a dict with statistic values
+        """
+        # streamflow, et, ssm, etc
+        target_cols = self.data_cfgs["target_cols"]
+        stat_dict = {}
+        for i in range(len(target_cols)):
+            var = target_cols[i]
+            if var in self.prcp_norm_cols:
+                stat_dict[var] = cal_stat_prcp_norm(
+                    self.data_target.sel(variable=var).to_numpy(),
+                    self.mean_prcp,
+                )
+            elif var in self.gamma_norm_cols:
+                stat_dict[var] = cal_stat_gamma(
+                    self.data_target.sel(variable=var).to_numpy()
+                )
+            else:
+                stat_dict[var] = cal_stat(self.data_target.sel(variable=var).to_numpy())
+
+        # forcing
+        forcing_lst = self.data_cfgs["relevant_cols"]
+        x = self.data_forcing
+        for k in range(len(forcing_lst)):
+            var = forcing_lst[k]
+            if var in self.gamma_norm_cols:
+                stat_dict[var] = cal_stat_gamma(x.sel(variable=var).to_numpy())
+            else:
+                stat_dict[var] = cal_stat(x.sel(variable=var).to_numpy())
+
+        # const attribute
+        attr_data = self.data_attr
+        attr_lst = self.data_cfgs["constant_cols"]
+        for k in range(len(attr_lst)):
+            var = attr_lst[k]
+            stat_dict[var] = cal_stat(attr_data.sel(variable=var).to_numpy())
+
+        return stat_dict
+
+    def get_data_obs(self, to_norm: bool = True) -> np.array:
+        """
+        Get observation values
+
+        Parameters
+        ----------
+        rm_nan
+            if true, fill NaN value with 0
+        to_norm
+            if true, perform normalization
+
+        Returns
+        -------
+        np.array
+            the output value for modeling
+        """
+        stat_dict = self.stat_dict
+        data = self.data_target
+        out = xr.full_like(data, np.nan)
+        # if we don't set a copy() here, the attrs of data will be changed, which is not our wish
+        out.attrs = copy.deepcopy(data.attrs)
+        target_cols = self.data_cfgs["target_cols"]
+        for i in range(len(target_cols)):
+            var = target_cols[i]
+            if var in self.prcp_norm_cols:
+                out.loc[dict(variable=var)] = _prcp_norm(
+                    data.sel(variable=var).to_numpy(),
+                    self.mean_prcp,
+                    to_norm=True,
+                )
+            else:
+                out.loc[dict(variable=var)] = data.sel(variable=var).to_numpy()
+            out.attrs["units"][var] = "dimensionless"
+        out = _trans_norm(
+            out,
+            target_cols,
+            stat_dict,
+            log_norm_cols=self.log_norm_cols,
+            to_norm=to_norm,
+        )
+        return out
+
+    def get_data_ts(self, to_norm=True) -> np.array:
+        """
+        Get dynamic input data
+
+        Parameters
+        ----------
+        rm_nan
+            if true, fill NaN value with 0
+        to_norm
+            if true, perform normalization
+
+        Returns
+        -------
+        np.array
+            the dynamic inputs for modeling
+        """
+        stat_dict = self.stat_dict
+        var_lst = self.data_cfgs["relevant_cols"]
+        data = self.data_forcing
+        data = _trans_norm(
+            data, var_lst, stat_dict, log_norm_cols=self.log_norm_cols, to_norm=to_norm
+        )
+        return data
+
+    def get_data_const(self, to_norm=True) -> np.array:
+        """
+        Attr data and normalization
+
+        Parameters
+        ----------
+        rm_nan
+            if true, fill NaN value with 0
+        to_norm
+            if true, perform normalization
+
+        Returns
+        -------
+        np.array
+            the static inputs for modeling
+        """
+        stat_dict = self.stat_dict
+        var_lst = self.data_cfgs["constant_cols"]
+        data = self.data_attr
+        data = _trans_norm(data, var_lst, stat_dict, to_norm=to_norm)
+        return data
+
+    def load_data(self):
+        """
+        Read data and perform normalization for DL models
+
+        Returns
+        -------
+        tuple
+            x: 3-d  gages_num*time_num*var_num
+            y: 3-d  gages_num*time_num*1
+            c: 2-d  gages_num*var_num
+        """
+        x = self.get_data_ts()
+        y = self.get_data_obs()
+        c = self.get_data_const()
+        return x, y, c
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `torchhydro-0.0.4/torchhydro/datasets/data_utils.py` & `torchhydro-0.0.5/torchhydro/datasets/data_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,434 +1,384 @@
-"""
-Author: Wenyu Ouyang
-Date: 2023-09-21 15:37:58
-LastEditTime: 2023-10-11 10:52:09
-LastEditors: Wenyu Ouyang
-Description: Some basic funtions for dealing with data
-FilePath: \torchhydro\torchhydro\datasets\data_utils.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-from typing import Union
-from hydrodataset import HydroDataset
-from collections import OrderedDict
-import numpy as np
-import xarray as xr
-import pint_xarray  # noqa: F401
-import warnings
-
-
-def warn_if_nan(dataarray, max_display=5):
-    """
-    Issue a warning if the dataarray contains any NaN values and display their locations.
-
-    Parameters
-    -----------
-    dataarray: xr.DataArray
-        Input dataarray to check for NaN values.
-    max_display: int
-        Maximum number of NaN locations to display in the warning.
-    """
-    nan_indices = np.argwhere(np.isnan(dataarray.values))
-    total_nans = len(nan_indices)
-
-    if total_nans <= 0:
-        return False
-    message = f"The dataarray contains {total_nans} NaN values!"
-
-    # Displaying only the first few NaN locations if there are too many
-    display_indices = nan_indices[:max_display].tolist()
-    message += (
-        f" Here are the indices of the first {max_display} NaNs: {display_indices}..."
-        if total_nans > max_display
-        else f" Here are the indices of the NaNs: {display_indices}"
-    )
-    warnings.warn(message)
-
-    return True
-
-
-def unify_streamflow_unit(ds: xr.Dataset, area=None, inverse=False):
-    """Unify the unit of xr_dataset to be mm/day in a basin or inverse
-
-    Parameters
-    ----------
-    ds: xarray dataset
-        _description_
-    area:
-        area of each basin
-
-    Returns
-    -------
-    _type_
-        _description_
-    """
-    # use pint to convert unit
-    if not inverse:
-        target_unit = "mm/d"
-        q = ds.pint.quantify()
-        a = area.pint.quantify()
-        r = q[list(q.keys())[0]] / a[list(a.keys())[0]]
-        result = r.pint.to(target_unit).to_dataset(name=list(q.keys())[0])
-    else:
-        target_unit = "m^3/s"
-        r = ds.pint.quantify()
-        a = area.pint.quantify()
-        q = r[list(r.keys())[0]] * a[list(a.keys())[0]]
-        result = q.pint.to(target_unit).to_dataset(name=list(r.keys())[0])
-    # dequantify to get normal xr_dataset
-    return result.pint.dequantify()
-
-
-def wrap_t_s_dict(
-    data_source: HydroDataset, data_cfgs: dict, is_tra_val_te: str
-) -> OrderedDict:
-    """
-    Basins and periods
-
-    Parameters
-    ----------
-    data_source
-        source data object
-    data_cfgs
-        configs for reading from data source
-    is_tra_val_te
-        train, valid or test
-
-    Returns
-    -------
-    OrderedDict
-        OrderedDict(sites_id=basins_id, t_final_range=t_range_list)
-    """
-    basins_id = data_cfgs["object_ids"]
-    if type(basins_id) is str and basins_id == "ALL":
-        basins_id = data_source.read_object_ids().tolist()
-    # assert all(x < y for x, y in zip(basins_id, basins_id[1:]))
-    if f"t_range_{is_tra_val_te}" in data_cfgs:
-        t_range_list = data_cfgs[f"t_range_{is_tra_val_te}"]
-    else:
-        raise Exception(
-            f"Error! The mode {is_tra_val_te} was not found in the data_source params dict. Please add it."
-        )
-    return OrderedDict(sites_id=basins_id, t_final_range=t_range_list)
-
-
-def _trans_norm(
-    x: xr.DataArray,
-    var_lst: list,
-    stat_dict: dict,
-    log_norm_cols: list = None,
-    to_norm: bool = True,
-    **kwargs,
-) -> np.array:
-    """
-    Normalization or inverse normalization
-
-    There are two normalization formulas:
-
-    .. math:: normalized_x = (x - mean) / std
-
-    and
-
-     .. math:: normalized_x = [log_{10}(\sqrt{x} + 0.1) - mean] / std
-
-     The later is only for vars in log_norm_cols; mean is mean value; std means standard deviation
-
-    Parameters
-    ----------
-    x
-        data to be normalized or denormalized
-    var_lst
-        the type of variables
-    stat_dict
-        statistics of all variables
-    log_norm_cols
-        which cols use the second norm method
-    to_norm
-        if true, normalize; else denormalize
-
-    Returns
-    -------
-    np.array
-        normalized or denormalized data
-    """
-    if x is None:
-        return None
-    if log_norm_cols is None:
-        log_norm_cols = []
-    if type(var_lst) is str:
-        var_lst = [var_lst]
-    out = xr.full_like(x, np.nan)
-    for item in var_lst:
-        stat = stat_dict[item]
-        if to_norm:
-            out.loc[dict(variable=item)] = (
-                (np.log10(np.sqrt(x.sel(variable=item)) + 0.1) - stat[2]) / stat[3]
-                if item in log_norm_cols
-                else (x.sel(variable=item) - stat[2]) / stat[3]
-            )
-        elif item in log_norm_cols:
-            out.loc[dict(variable=item)] = (
-                np.power(10, x.sel(variable=item) * stat[3] + stat[2]) - 0.1
-            ) ** 2
-        else:
-            out.loc[dict(variable=item)] = x.sel(variable=item) * stat[3] + stat[2]
-    if to_norm:
-        # after normalization, all units are dimensionless
-        out.attrs = {}
-    # after denormalization, recover units
-    else:
-        if "recover_units" in kwargs.keys() and kwargs["recover_units"] is not None:
-            recover_units = kwargs["recover_units"]
-            for item in var_lst:
-                out.attrs["units"][item] = recover_units[item]
-    return out
-
-
-def _prcp_norm(x: np.array, mean_prep: np.array, to_norm: bool) -> np.array:
-    """
-    Normalize or denormalize data with mean precipitation.
-
-    The formula is as follows when normalizing (denormalize equation is its inversion):
-
-    .. math:: normalized_x = \frac{x}{precipitation}
-
-    Parameters
-    ----------
-    x
-        data to be normalized or denormalized
-    mean_prep
-        basins' mean precipitation
-    to_norm
-        if true, normalize; else denormalize
-
-    Returns
-    -------
-    np.array
-        normalized or denormalized data
-    """
-    tempprep = np.tile(mean_prep, (1, x.shape[1]))
-    return x / tempprep if to_norm else x * tempprep
-
-
-def dor_reservoirs_chosen(gages, usgs_id, dor_chosen) -> list:
-    """
-    choose basins of small DOR(calculated by NOR_STORAGE/RUNAVE7100)
-
-    """
-
-    dors = get_dor_values(gages, usgs_id)
-    if type(dor_chosen) in [list, tuple]:
-        # right half-open range
-        chosen_id = [
-            usgs_id[i]
-            for i in range(dors.size)
-            if dor_chosen[0] <= dors[i] < dor_chosen[1]
-        ]
-    elif dor_chosen < 0:
-        chosen_id = [usgs_id[i] for i in range(dors.size) if dors[i] < -dor_chosen]
-    else:
-        chosen_id = [usgs_id[i] for i in range(dors.size) if dors[i] >= dor_chosen]
-
-    assert all(x < y for x, y in zip(chosen_id, chosen_id[1:]))
-    return chosen_id
-
-
-def usgs_screen_streamflow(
-    gages, usgs_ids: list, time_range: list, flow_type=None, **kwargs
-) -> list:
-    """
-    according to the criteria and its ancillary condition--thresh of streamflow data,
-    choose appropriate ones from the given usgs sites
-
-    Parameters
-    ----------
-    gages
-        Camels, CamelsSeries, Gages or GagesPro object
-    usgs_ids: list
-        given sites' ids
-    time_range: list
-        chosen time range
-    flow_type
-        flow's name in data file; default is usgsFlow for CAMELS-US
-    kwargs
-        all criteria
-
-    Returns
-    -------
-    list
-        sites_chosen: [] -- ids of chosen gages
-
-    Examples
-    --------
-        >>> usgs_screen_streamflow(gages, ["02349000","08168797"], ["1995-01-01","2015-01-01"], **{'missing_data_ratio': 0, 'zero_value_ratio': 1})
-    """
-    usgs_values = gages.read_target_cols(usgs_ids, time_range, [flow_type])[:, :, 0]
-    sites_index = np.arange(usgs_values.shape[0])
-    sites_chosen = np.ones(usgs_values.shape[0])
-    for i in range(sites_index.size):
-        # loop for every site
-        runoff = usgs_values[i, :]
-        for criteria, thresh in kwargs.items():
-            # if any criteria is not matched, we can filter this site
-            if sites_chosen[sites_index[i]] == 0:
-                break
-            if criteria == "missing_data_ratio":
-                nan_length = runoff[np.isnan(runoff)].size
-                sites_chosen[sites_index[i]] = (
-                    0 if nan_length / runoff.size > thresh else 1
-                )
-            elif criteria == "zero_value_ratio":
-                zero_length = runoff.size - np.count_nonzero(runoff)
-                thresh = kwargs[criteria]
-                sites_chosen[sites_index[i]] = (
-                    0 if zero_length / runoff.size > thresh else 1
-                )
-            else:
-                print(
-                    "Oops! That is not valid value. Try missing_data_ratio or zero_value_ratio ..."
-                )
-    return [usgs_ids[i] for i in range(len(sites_chosen)) if sites_chosen[i] > 0]
-
-
-def choose_sites_in_ecoregion(
-    gages, site_ids: list, ecoregion: Union[list, tuple]
-) -> list:
-    """
-    Choose sites in ecoregions
-
-    Parameters
-    ----------
-    gages : Gages
-        Only gages dataset has ecoregion attribute
-    site_ids : list
-        all ids of sites
-    ecoregion : Union[list, tuple]
-        which ecoregions
-
-    Returns
-    -------
-    list
-        chosen sites' ids
-
-    Raises
-    ------
-    NotImplementedError
-        PLease choose 'ECO2_CODE' or 'ECO3_CODE'
-    NotImplementedError
-        must be in EC02 code list
-    NotImplementedError
-        must be in EC03 code list
-    """
-    if ecoregion[0] not in ["ECO2_CODE", "ECO3_CODE"]:
-        raise NotImplementedError("PLease choose 'ECO2_CODE' or 'ECO3_CODE'")
-    if ecoregion[0] == "ECO2_CODE":
-        ec02_code_lst = [
-            5.2,
-            5.3,
-            6.2,
-            7.1,
-            8.1,
-            8.2,
-            8.3,
-            8.4,
-            8.5,
-            9.2,
-            9.3,
-            9.4,
-            9.5,
-            9.6,
-            10.1,
-            10.2,
-            10.4,
-            11.1,
-            12.1,
-            13.1,
-        ]
-        if ecoregion[1] not in ec02_code_lst:
-            raise NotImplementedError(
-                f"No such EC02 code, please choose from {ec02_code_lst}"
-            )
-        attr_name = "ECO2_BAS_DOM"
-    elif ecoregion[1] in np.arange(1, 85):
-        attr_name = "ECO3_BAS_DOM"
-    else:
-        raise NotImplementedError("No such EC03 code, please choose from 1 - 85")
-    attr_lst = [attr_name]
-    data_attr = gages.read_constant_cols(site_ids, attr_lst)
-    eco_names = data_attr[:, 0]
-    return [site_ids[i] for i in range(eco_names.size) if eco_names[i] == ecoregion[1]]
-
-
-def choose_basins_with_area(
-    gages,
-    usgs_ids: list,
-    smallest_area: float,
-    largest_area: float,
-) -> list:
-    """
-    choose basins with not too large or too small area
-
-    Parameters
-    ----------
-    gages
-        Camels, CamelsSeries, Gages or GagesPro object
-    usgs_ids: list
-        given sites' ids
-    smallest_area
-        lower limit; unit is km2
-    largest_area
-        upper limit; unit is km2
-
-    Returns
-    -------
-    list
-        sites_chosen: [] -- ids of chosen gages
-
-    """
-    basins_areas = gages.read_basin_area(usgs_ids).flatten()
-    sites_index = np.arange(len(usgs_ids))
-    sites_chosen = np.ones(len(usgs_ids))
-    for i in range(sites_index.size):
-        # loop for every site
-        if basins_areas[i] < smallest_area or basins_areas[i] > largest_area:
-            sites_chosen[sites_index[i]] = 0
-        else:
-            sites_chosen[sites_index[i]] = 1
-    return [usgs_ids[i] for i in range(len(sites_chosen)) if sites_chosen[i] > 0]
-
-
-def diversion_chosen(gages, usgs_id):
-    diversion_strs = ["diversion", "divert"]
-    assert all(x < y for x, y in zip(usgs_id, usgs_id[1:]))
-    attr_lst = ["WR_REPORT_REMARKS", "SCREENING_COMMENTS"]
-    data_attr = gages.read_attr_origin(usgs_id, attr_lst)
-    diversion_strs_lower = [elem.lower() for elem in diversion_strs]
-    data_attr0_lower = np.array(
-        [elem.lower() if type(elem) == str else elem for elem in data_attr[0]]
-    )
-    data_attr1_lower = np.array(
-        [elem.lower() if type(elem) == str else elem for elem in data_attr[1]]
-    )
-    data_attr_lower = np.vstack((data_attr0_lower, data_attr1_lower)).T
-    return [
-        usgs_id[i]
-        for i in range(len(usgs_id))
-        if is_any_elem_in_a_lst(diversion_strs_lower, data_attr_lower[i], include=True)
-    ]
-
-
-def dam_num_chosen(gages, usgs_id, dam_num):
-    """choose basins of dams"""
-    assert all(x < y for x, y in zip(usgs_id, usgs_id[1:]))
-    attr_lst = ["NDAMS_2009"]
-    data_attr = gages.read_constant_cols(usgs_id, attr_lst)
-    return (
-        [
-            usgs_id[i]
-            for i in range(data_attr.size)
-            if dam_num[0] <= data_attr[:, 0][i] < dam_num[1]
-        ]
-        if type(dam_num) == list
-        else [
-            usgs_id[i] for i in range(data_attr.size) if data_attr[:, 0][i] == dam_num
-        ]
-    )
+"""
+Author: Wenyu Ouyang
+Date: 2023-09-21 15:37:58
+LastEditTime: 2024-04-14 15:10:02
+LastEditors: Wenyu Ouyang
+Description: Some basic funtions for dealing with data
+FilePath: \torchhydro\torchhydro\datasets\data_utils.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+
+from typing import Union
+from collections import OrderedDict
+import numpy as np
+import xarray as xr
+import pint_xarray  # noqa: F401
+import warnings
+
+
+def warn_if_nan(dataarray, max_display=5, nan_mode="any"):
+    """
+    Issue a warning if the dataarray contains any NaN values and display their locations.
+
+    Parameters
+    -----------
+    dataarray: xr.DataArray
+        Input dataarray to check for NaN values.
+    max_display: int
+        Maximum number of NaN locations to display in the warning.
+    nan_mode: str
+        Mode of NaN checking: 'any' for any NaNs, 'all' for all values being NaNs.
+    """
+    if nan_mode not in ["any", "all"]:
+        raise ValueError("nan_mode must be 'any' or 'all'")
+
+    if nan_mode == "all" and np.all(np.isnan(dataarray.values)):
+        raise ValueError("The dataarray contains only NaN values!")
+
+    nan_indices = np.argwhere(np.isnan(dataarray.values))
+    total_nans = len(nan_indices)
+
+    if total_nans <= 0:
+        return False
+    message = f"The dataarray contains {total_nans} NaN values!"
+
+    # Displaying only the first few NaN locations if there are too many
+    display_indices = nan_indices[:max_display].tolist()
+    message += (
+        f" Here are the indices of the first {max_display} NaNs: {display_indices}..."
+        if total_nans > max_display
+        else f" Here are the indices of the NaNs: {display_indices}"
+    )
+    warnings.warn(message)
+
+    return True
+
+
+def unify_streamflow_unit(ds: xr.Dataset, area=None, inverse=False):
+    """Unify the unit of xr_dataset to be mm/day in a basin or inverse
+
+    Parameters
+    ----------
+    ds: xarray dataset
+        _description_
+    area:
+        area of each basin
+
+    Returns
+    -------
+    _type_
+        _description_
+    """
+    # use pint to convert unit
+    if not inverse:
+        target_unit = "mm/d"
+        q = ds.pint.quantify()
+        a = area.pint.quantify()
+        r = q[list(q.keys())[0]] / a[list(a.keys())[0]]
+        result = r.pint.to(target_unit).to_dataset(name=list(q.keys())[0])
+    else:
+        target_unit = "m^3/s"
+        r = ds.pint.quantify()
+        a = area.pint.quantify()
+        q = r[list(r.keys())[0]] * a[list(a.keys())[0]]
+        # q = q.pint.quantify()
+        result = q.pint.to(target_unit).to_dataset(name=list(r.keys())[0])
+    # dequantify to get normal xr_dataset
+    return result.pint.dequantify()
+
+
+def wrap_t_s_dict(data_cfgs: dict, is_tra_val_te: str) -> OrderedDict:
+    """
+    Basins and periods
+
+    Parameters
+    ----------
+
+    data_cfgs
+        configs for reading from data source
+    is_tra_val_te
+        train, valid or test
+
+    Returns
+    -------
+    OrderedDict
+        OrderedDict(sites_id=basins_id, t_final_range=t_range_list)
+    """
+    basins_id = data_cfgs["object_ids"]
+    # if type(basins_id) is str and basins_id == "ALL":
+    #     basins_id = data_source.read_object_ids().tolist()
+    # assert all(x < y for x, y in zip(basins_id, basins_id[1:]))
+    if f"t_range_{is_tra_val_te}" in data_cfgs:
+        t_range_list = data_cfgs[f"t_range_{is_tra_val_te}"]
+    else:
+        raise Exception(
+            f"Error! The mode {is_tra_val_te} was not found. Please add it."
+        )
+    return OrderedDict(sites_id=basins_id, t_final_range=t_range_list)
+
+
+def _trans_norm(
+    x: xr.DataArray,
+    var_lst: list,
+    stat_dict: dict,
+    log_norm_cols: list = None,
+    to_norm: bool = True,
+    **kwargs,
+) -> np.array:
+    """
+    Normalization or inverse normalization
+
+    There are two normalization formulas:
+
+    .. math:: normalized_x = (x - mean) / std
+
+    and
+
+     .. math:: normalized_x = [log_{10}(\sqrt{x} + 0.1) - mean] / std
+
+     The later is only for vars in log_norm_cols; mean is mean value; std means standard deviation
+
+    Parameters
+    ----------
+    x
+        data to be normalized or denormalized
+    var_lst
+        the type of variables
+    stat_dict
+        statistics of all variables
+    log_norm_cols
+        which cols use the second norm method
+    to_norm
+        if true, normalize; else denormalize
+
+    Returns
+    -------
+    np.array
+        normalized or denormalized data
+    """
+    if x is None:
+        return None
+    if log_norm_cols is None:
+        log_norm_cols = []
+    if type(var_lst) is str:
+        var_lst = [var_lst]
+    out = xr.full_like(x, np.nan)
+    for item in var_lst:
+        stat = stat_dict[item]
+        if to_norm:
+            out.loc[dict(variable=item)] = (
+                (np.log10(np.sqrt(np.abs(x.sel(variable=item))) + 0.1) - stat[2])
+                / stat[3]
+                if item in log_norm_cols
+                else (x.sel(variable=item) - stat[2]) / stat[3]
+            )
+        elif item in log_norm_cols:
+            out.loc[dict(variable=item)] = (
+                np.power(10, x.sel(variable=item) * stat[3] + stat[2]) - 0.1
+            ) ** 2
+        else:
+            out.loc[dict(variable=item)] = x.sel(variable=item) * stat[3] + stat[2]
+    if to_norm:
+        # after normalization, all units are dimensionless
+        out.attrs = {}
+    # after denormalization, recover units
+    else:
+        if "recover_units" in kwargs.keys() and kwargs["recover_units"] is not None:
+            recover_units = kwargs["recover_units"]
+            for item in var_lst:
+                out.attrs["units"][item] = recover_units[item]
+    return out
+
+
+def _prcp_norm(x: np.array, mean_prep: np.array, to_norm: bool) -> np.array:
+    """
+    Normalize or denormalize data with mean precipitation.
+
+    The formula is as follows when normalizing (denormalize equation is its inversion):
+
+    .. math:: normalized_x = \frac{x}{precipitation}
+
+    Parameters
+    ----------
+    x
+        data to be normalized or denormalized
+    mean_prep
+        basins' mean precipitation
+    to_norm
+        if true, normalize; else denormalize
+
+    Returns
+    -------
+    np.array
+        normalized or denormalized data
+    """
+    tempprep = np.tile(mean_prep, (1, x.shape[1]))
+    return x / tempprep if to_norm else x * tempprep
+
+
+def dor_reservoirs_chosen(gages, usgs_id, dor_chosen) -> list:
+    """
+    choose basins of small DOR(calculated by NOR_STORAGE/RUNAVE7100)
+
+    """
+
+    dors = get_dor_values(gages, usgs_id)
+    if type(dor_chosen) in [list, tuple]:
+        # right half-open range
+        chosen_id = [
+            usgs_id[i]
+            for i in range(dors.size)
+            if dor_chosen[0] <= dors[i] < dor_chosen[1]
+        ]
+    elif dor_chosen < 0:
+        chosen_id = [usgs_id[i] for i in range(dors.size) if dors[i] < -dor_chosen]
+    else:
+        chosen_id = [usgs_id[i] for i in range(dors.size) if dors[i] >= dor_chosen]
+
+    assert all(x < y for x, y in zip(chosen_id, chosen_id[1:]))
+    return chosen_id
+
+
+def choose_sites_in_ecoregion(
+    gages, site_ids: list, ecoregion: Union[list, tuple]
+) -> list:
+    """
+    Choose sites in ecoregions
+
+    Parameters
+    ----------
+    gages : Gages
+        Only gages dataset has ecoregion attribute
+    site_ids : list
+        all ids of sites
+    ecoregion : Union[list, tuple]
+        which ecoregions
+
+    Returns
+    -------
+    list
+        chosen sites' ids
+
+    Raises
+    ------
+    NotImplementedError
+        PLease choose 'ECO2_CODE' or 'ECO3_CODE'
+    NotImplementedError
+        must be in EC02 code list
+    NotImplementedError
+        must be in EC03 code list
+    """
+    if ecoregion[0] not in ["ECO2_CODE", "ECO3_CODE"]:
+        raise NotImplementedError("PLease choose 'ECO2_CODE' or 'ECO3_CODE'")
+    if ecoregion[0] == "ECO2_CODE":
+        ec02_code_lst = [
+            5.2,
+            5.3,
+            6.2,
+            7.1,
+            8.1,
+            8.2,
+            8.3,
+            8.4,
+            8.5,
+            9.2,
+            9.3,
+            9.4,
+            9.5,
+            9.6,
+            10.1,
+            10.2,
+            10.4,
+            11.1,
+            12.1,
+            13.1,
+        ]
+        if ecoregion[1] not in ec02_code_lst:
+            raise NotImplementedError(
+                f"No such EC02 code, please choose from {ec02_code_lst}"
+            )
+        attr_name = "ECO2_BAS_DOM"
+    elif ecoregion[1] in np.arange(1, 85):
+        attr_name = "ECO3_BAS_DOM"
+    else:
+        raise NotImplementedError("No such EC03 code, please choose from 1 - 85")
+    attr_lst = [attr_name]
+    data_attr = gages.read_constant_cols(site_ids, attr_lst)
+    eco_names = data_attr[:, 0]
+    return [site_ids[i] for i in range(eco_names.size) if eco_names[i] == ecoregion[1]]
+
+
+def choose_basins_with_area(
+    gages,
+    usgs_ids: list,
+    smallest_area: float,
+    largest_area: float,
+) -> list:
+    """
+    choose basins with not too large or too small area
+
+    Parameters
+    ----------
+    gages
+        Camels, CamelsSeries, Gages or GagesPro object
+    usgs_ids: list
+        given sites' ids
+    smallest_area
+        lower limit; unit is km2
+    largest_area
+        upper limit; unit is km2
+
+    Returns
+    -------
+    list
+        sites_chosen: [] -- ids of chosen gages
+
+    """
+    basins_areas = gages.read_basin_area(usgs_ids).flatten()
+    sites_index = np.arange(len(usgs_ids))
+    sites_chosen = np.ones(len(usgs_ids))
+    for i in range(sites_index.size):
+        # loop for every site
+        if basins_areas[i] < smallest_area or basins_areas[i] > largest_area:
+            sites_chosen[sites_index[i]] = 0
+        else:
+            sites_chosen[sites_index[i]] = 1
+    return [usgs_ids[i] for i in range(len(sites_chosen)) if sites_chosen[i] > 0]
+
+
+def diversion_chosen(gages, usgs_id):
+    diversion_strs = ["diversion", "divert"]
+    assert all(x < y for x, y in zip(usgs_id, usgs_id[1:]))
+    attr_lst = ["WR_REPORT_REMARKS", "SCREENING_COMMENTS"]
+    data_attr = gages.read_attr_origin(usgs_id, attr_lst)
+    diversion_strs_lower = [elem.lower() for elem in diversion_strs]
+    data_attr0_lower = np.array(
+        [elem.lower() if type(elem) == str else elem for elem in data_attr[0]]
+    )
+    data_attr1_lower = np.array(
+        [elem.lower() if type(elem) == str else elem for elem in data_attr[1]]
+    )
+    data_attr_lower = np.vstack((data_attr0_lower, data_attr1_lower)).T
+    return [
+        usgs_id[i]
+        for i in range(len(usgs_id))
+        if is_any_elem_in_a_lst(diversion_strs_lower, data_attr_lower[i], include=True)
+    ]
+
+
+def dam_num_chosen(gages, usgs_id, dam_num):
+    """choose basins of dams"""
+    assert all(x < y for x, y in zip(usgs_id, usgs_id[1:]))
+    attr_lst = ["NDAMS_2009"]
+    data_attr = gages.read_constant_cols(usgs_id, attr_lst)
+    return (
+        [
+            usgs_id[i]
+            for i in range(data_attr.size)
+            if dam_num[0] <= data_attr[:, 0][i] < dam_num[1]
+        ]
+        if type(dam_num) == list
+        else [
+            usgs_id[i] for i in range(data_attr.size) if data_attr[:, 0][i] == dam_num
+        ]
+    )
```

### Comparing `torchhydro-0.0.4/torchhydro/explainers/shap.py` & `torchhydro-0.0.5/torchhydro/explainers/shap.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,188 +1,233 @@
-"""
-Author: Wenyu Ouyang
-Date: 2023-10-19 21:34:29
-LastEditTime: 2023-10-28 13:00:52
-LastEditors: Wenyu Ouyang
-Description: SHAP methods for deep learning models
-FilePath: \torchhydro\torchhydro\explainers\shap.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-from typing import List
-import torch
-import numpy as np
-import shap
-import matplotlib.pyplot as plt
-import seaborn as sns
-
-
-def plot_summary_shap_values(shap_values: torch.tensor, columns):
-    mean_shap_values = shap_values.mean(dim=(0, 1))
-
-    # Tensor to NumPy array to use matplotlib and seaborn
-    mean_shap_values = mean_shap_values.abs().mean(dim=0).numpy()
-
-    # seaborn barplot
-    plt.figure(figsize=(10, 8))
-    sns.barplot(x=mean_shap_values, y=columns, order=columns[::-1], orient="h")
-    plt.xlabel("Mean Absolute SHAP Value")
-    plt.title("Summary Plot of SHAP Values")
-    plt.show()
-
-
-def plot_summary_shap_values_over_time_series(shap_values: torch.tensor, columns):
-    # Compute the absolute mean SHAP values over batches
-    abs_mean_shap_values = shap_values.mean(dim=1).abs()
-
-    # Further compute the mean over observations
-    multi_shap_values = abs_mean_shap_values.mean(dim=1).numpy()
-
-    # Plotting
-    plt.figure(figsize=(10, 8))
-
-    bottom = np.zeros(len(columns))
-    for i, pred_shap_values in enumerate(multi_shap_values):
-        plt.barh(columns[::-1], pred_shap_values, label=f"time-step {i}", left=bottom)
-        bottom += pred_shap_values
-
-    plt.xlabel("Mean Absolute SHAP Value Over Time Steps")
-    plt.title("Summary Plot of SHAP Values Over Time Series")
-    plt.legend()
-    plt.show()
-
-
-def jitter(values, jitter_strength=0.005):
-    """Add some jitter to the values."""
-    return values + jitter_strength * np.random.randn(*values.shape)
-
-
-def plot_shap_values_from_history(shap_values: torch.tensor, history: torch.tensor):
-    # Compute mean values across the specified axes
-    mean_shap_values = shap_values.mean(dim=[0, 1])
-    mean_history_values = history.mean(dim=1)
-    figs: List[plt.Figure] = []
-    # Loop through features and plot each scatter plot
-    for feature_history, feature_shap_values in zip(
-        mean_history_values.unbind(0), mean_shap_values.unbind(0)
-    ):
-        fig, ax = plt.subplots(figsize=(8, 6))
-        # Convert tensor to numpy array for plotting
-        feature_shap_values_np = feature_shap_values.numpy()
-        feature_history_np = feature_history.numpy()
-        scatter = ax.scatter(
-            feature_shap_values_np,
-            jitter(feature_shap_values_np),
-            c=feature_history_np,
-            cmap="bwr",  # Blue to Red color map
-            marker="o",
-        )
-        ax.set_ylim(-0.05, 0.05)
-        ax.set_xlabel("shap value")
-        ax.set_yticks([])  # Hide y-axis ticks as they represent jittered values
-        # Colorbar configuration
-        cbar = plt.colorbar(scatter, ax=ax)
-        cbar.set_label("feature values")
-        figs.append(fig)
-    return figs
-
-
-def deep_explain_model_summary_plot(dl_model, test_dataset) -> None:
-    """Generate feature summary plot for trained deep learning models
-
-    Parameters
-    ----------
-    model
-        trained model
-    test_dataset
-        test dataset
-    """
-    dl_model.eval()
-    history = test_dataset.__getitem__(0)[0].unsqueeze(0)
-    dl_model = dl_model.to("cpu")
-    deep_explainer = shap.DeepExplainer(dl_model, history)
-    shap_values = shap_results(deep_explainer, history)
-    # summary plot shows overall feature ranking
-    # by average absolute shap values
-    fig = plot_summary_shap_values(shap_values, test_dataset.df.columns)
-    abs_mean_shap_values = shap_values.mean(axis=["preds", "batches"])
-    multi_shap_values = abs_mean_shap_values.mean(axis="observations")
-    # summary plot for multi-step outputs
-    # multi_shap_values = shap_values.apply_along_axis(np.mean, 'batches')
-    fig = plot_summary_shap_values_over_time_series(
-        shap_values, test_dataset.df.columns
-    )
-    history_numpy = torch.tensor(
-        history.cpu().numpy(), names=["batches", "observations", "features"]
-    )
-
-    shap_values = shap_results(deep_explainer, history)
-    figs = plot_shap_values_from_history(shap_values, history_numpy)
-
-
-def shap_results(deep_explainer, history):
-    result = deep_explainer.shap_values(history)
-    result = np.stack(result)
-    # shap_values needs to be 4-dimensional
-    if len(result.shape) != 4:
-        result = np.expand_dims(result, axis=0)
-    result = torch.tensor(
-        result, names=["preds", "batches", "observations", "features"]
-    )
-
-    return result
-
-
-def plot_shap_value_heatmaps(shap_values: torch.tensor):
-    # Compute the average shap values over batches
-    average_shap_value_over_batches = shap_values.mean(dim=shap_values.dim() - 1)
-
-    figs: List[plt.Figure] = []
-
-    # Extracting the shapes of the data for the x and y ticks
-    x = list(range(average_shap_value_over_batches.size(-1)))
-    y = list(range(average_shap_value_over_batches.size(0)))
-
-    # Iterate through features and plot each heatmap
-    for shap_values_features in average_shap_value_over_batches.unbind(0):
-        fig, ax = plt.subplots(figsize=(8, 6))
-
-        # Convert tensor to numpy array for plotting
-        shap_values_features_np = shap_values_features.numpy()
-
-        # Plotting heatmap
-        cax = ax.matshow(shap_values_features_np, cmap="bwr", aspect="auto")
-
-        ax.set_xticks(x)
-        ax.set_yticks(y)
-        ax.set_xlabel("sequence history steps")
-        ax.set_ylabel("prediction steps")
-
-        # Adding colorbar to the right of the heatmap
-        cbar = fig.colorbar(cax, ax=ax)
-        cbar.set_label("feature values")
-
-        figs.append(fig)
-
-    return figs
-
-
-def deep_explain_model_heatmap(dl_model, test_dataset) -> None:
-    """Generate feature heatmap for prediction at a start time
-    Parameters
-    ----------
-    model
-        trained model
-    test_dataset
-        test dataset
-    Returns
-    -------
-    None
-    """
-    dl_model.eval()
-    history = test_dataset.__getitem__(0)[0]
-    # background shape (L, N, M)
-    # L - batch size, N - history length, M - feature size
-    # for each element in each N x M batch in L,
-    # attribute to each prediction in forecast len
-    deep_explainer = shap.DeepExplainer(dl_model, history)
-    shap_values = shap_results(deep_explainer, history)
-    figs = plot_shap_value_heatmaps(shap_values)
+"""
+Author: Wenyu Ouyang
+Date: 2023-10-19 21:34:29
+LastEditTime: 2023-12-29 11:05:57
+LastEditors: Xinzhuo Wu
+Description: SHAP methods for deep learning models
+FilePath: \torchhydro\torchhydro\explainers\shap.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+from typing import List
+import torch
+import numpy as np
+import shap
+import matplotlib.pyplot as plt
+import seaborn as sns
+import os
+
+
+def plot_summary_shap_values(shap_values: torch.tensor, columns):
+    mean_shap_values = shap_values.mean(dim=(0, 1))
+
+    # Tensor to NumPy array to use matplotlib and seaborn
+    mean_shap_values = mean_shap_values.abs().mean(dim=0).numpy()
+
+    # seaborn barplot
+    plt.figure(figsize=(10, 8))
+    sns.barplot(x=mean_shap_values, y=columns, order=columns[::-1], orient="h")
+    plt.xlabel("Mean Absolute SHAP Value")
+    plt.title("Summary Plot of SHAP Values")
+    plt.show()
+
+
+def plot_summary_shap_values_over_time_series(shap_values: torch.tensor, columns):
+    # Compute the absolute mean SHAP values over batches
+    abs_mean_shap_values = shap_values.mean(dim=1).abs()
+
+    # Further compute the mean over observations
+    multi_shap_values = abs_mean_shap_values.mean(dim=1).numpy()
+
+    # Plotting
+    plt.figure(figsize=(10, 8))
+
+    bottom = np.zeros(len(columns))
+    for i, pred_shap_values in enumerate(multi_shap_values):
+        plt.barh(columns[::-1], pred_shap_values, label=f"time-step {i}", left=bottom)
+        bottom += pred_shap_values
+
+    plt.xlabel("Mean Absolute SHAP Value Over Time Steps")
+    plt.title("Summary Plot of SHAP Values Over Time Series")
+    plt.legend()
+    plt.show()
+
+
+def jitter(values, jitter_strength=0.005):
+    """Add some jitter to the values."""
+    return values + jitter_strength * np.random.randn(*values.shape)
+
+
+def plot_shap_values_from_history(shap_values: torch.tensor, history: torch.tensor):
+    # Compute mean values across the specified axes
+    mean_shap_values = shap_values.mean(dim=[0, 1])
+    mean_history_values = history.mean(dim=1)
+    figs: List[plt.Figure] = []
+    # Loop through features and plot each scatter plot
+    for feature_history, feature_shap_values in zip(
+        mean_history_values.unbind(0), mean_shap_values.unbind(0)
+    ):
+        fig, ax = plt.subplots(figsize=(8, 6))
+        # Convert tensor to numpy array for plotting
+        feature_shap_values_np = feature_shap_values.numpy()
+        feature_history_np = feature_history.numpy()
+        scatter = ax.scatter(
+            feature_shap_values_np,
+            jitter(feature_shap_values_np),
+            c=feature_history_np,
+            cmap="bwr",  # Blue to Red color map
+            marker="o",
+        )
+        ax.set_ylim(-0.05, 0.05)
+        ax.set_xlabel("shap value")
+        ax.set_yticks([])  # Hide y-axis ticks as they represent jittered values
+        # Colorbar configuration
+        cbar = plt.colorbar(scatter, ax=ax)
+        cbar.set_label("feature values")
+        figs.append(fig)
+    return figs
+
+
+def deep_explain_model_summary_plot(dl_model, test_dataset) -> None:
+    """Generate feature summary plot for trained deep learning models
+
+    Parameters
+    ----------
+    model
+        trained model
+    test_dataset
+        test dataset
+    """
+    dl_model.eval()
+    history = test_dataset.__getitem__(0)[0].unsqueeze(0)
+    dl_model = dl_model.to("cpu")
+    deep_explainer = shap.DeepExplainer(dl_model, history)
+    shap_values = shap_results(deep_explainer, history)
+    # summary plot shows overall feature ranking
+    # by average absolute shap values
+    fig = plot_summary_shap_values(shap_values, test_dataset.df.columns)
+    abs_mean_shap_values = shap_values.mean(axis=["preds", "batches"])
+    multi_shap_values = abs_mean_shap_values.mean(axis="observations")
+    # summary plot for multi-step outputs
+    # multi_shap_values = shap_values.apply_along_axis(np.mean, 'batches')
+    fig = plot_summary_shap_values_over_time_series(
+        shap_values, test_dataset.df.columns
+    )
+    history_numpy = torch.tensor(
+        history.cpu().numpy(), names=["batches", "observations", "features"]
+    )
+
+    shap_values = shap_results(deep_explainer, history)
+    figs = plot_shap_values_from_history(shap_values, history_numpy)
+
+
+def shap_results(deep_explainer, history):
+    result = deep_explainer.shap_values(history)
+    result = np.stack(result)
+    # shap_values needs to be 4-dimensional
+    if len(result.shape) != 4:
+        result = np.expand_dims(result, axis=0)
+    result = torch.tensor(
+        result, names=["preds", "batches", "observations", "features"]
+    )
+
+    return result
+
+
+def plot_shap_value_heatmaps(shap_values: torch.tensor):
+    # Compute the average shap values over batches
+    average_shap_value_over_batches = shap_values.mean(dim=shap_values.dim() - 1)
+
+    figs: List[plt.Figure] = []
+
+    # Extracting the shapes of the data for the x and y ticks
+    x = list(range(average_shap_value_over_batches.size(-1)))
+    y = list(range(average_shap_value_over_batches.size(0)))
+
+    # Iterate through features and plot each heatmap
+    for shap_values_features in average_shap_value_over_batches.unbind(0):
+        fig, ax = plt.subplots(figsize=(8, 6))
+
+        # Convert tensor to numpy array for plotting
+        shap_values_features_np = shap_values_features.numpy()
+
+        # Plotting heatmap
+        cax = ax.matshow(shap_values_features_np, cmap="bwr", aspect="auto")
+
+        ax.set_xticks(x)
+        ax.set_yticks(y)
+        ax.set_xlabel("sequence history steps")
+        ax.set_ylabel("prediction steps")
+
+        # Adding colorbar to the right of the heatmap
+        cbar = fig.colorbar(cax, ax=ax)
+        cbar.set_label("feature values")
+
+        figs.append(fig)
+
+    return figs
+
+
+def deep_explain_model_heatmap(dl_model, test_dataset) -> None:
+    """Generate feature heatmap for prediction at a start time
+    Parameters
+    ----------
+    model
+        trained model
+    test_dataset
+        test dataset
+    Returns
+    -------
+    None
+    """
+    dl_model.eval()
+    history = test_dataset.__getitem__(0)[0]
+    # background shape (L, N, M)
+    # L - batch size, N - history length, M - feature size
+    # for each element in each N x M batch in L,
+    # attribute to each prediction in forecast len
+    deep_explainer = shap.DeepExplainer(dl_model, history)
+    shap_values = shap_results(deep_explainer, history)
+    figs = plot_shap_value_heatmaps(shap_values)
+
+
+def shap_summary_plot(dl_model, train_dataset, test_dataset) -> None:
+    dl_model.eval()
+
+    history_list = []
+    for i in range(
+        int(train_dataset.num_samples / len(train_dataset.data_cfgs["object_ids"]))
+    ):
+        h = train_dataset.__getitem__(i)[0]
+        history_list.append(h)
+    history = torch.cat(history_list).cuda()
+
+    test_list = []
+    for i in range(
+        int(test_dataset.num_samples / len(test_dataset.data_cfgs["object_ids"]))
+    ):
+        t = test_dataset.__getitem__(i)[0]
+        test_list.append(t)
+    test = torch.cat(test_list).cuda()
+
+    dl_model = dl_model.cuda()
+    torch.backends.cudnn.enabled = False
+    e = shap.DeepExplainer(dl_model, history)
+    shap_values = e.shap_values(test)[0]
+
+    shap_values_avg = (
+        shap_values.squeeze(2)
+        .reshape(shap_values.shape[0], shap_values.shape[1], -1)
+        .mean(axis=-2)
+    )
+    test_tensor_avg = (
+        test.squeeze(2).reshape(test.shape[0], test.shape[1], -1).mean(axis=-2)
+    ).to("cpu")
+    np.save(
+        os.path.join(test_dataset.data_cfgs["test_path"], "shap_values_avg.npy"),
+        shap_values_avg,
+    )
+    torch.save(
+        test_tensor_avg,
+        os.path.join(test_dataset.data_cfgs["test_path"], "test_tensor_avg.pth"),
+    )
+    shap.summary_plot(shap_values_avg, test_tensor_avg)
+    plt.savefig(os.path.join(test_dataset.data_cfgs["test_path"], "shap.png"))
```

### Comparing `torchhydro-0.0.4/torchhydro/explainers/weight_anlysis.py` & `torchhydro-0.0.5/torchhydro/explainers/weight_anlysis.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,289 +1,289 @@
-import os
-from pathlib import Path
-import shutil
-import numpy as np
-import pandas as pd
-from tbparse import SummaryReader
-from matplotlib import cm, colors, pyplot as plt
-from scipy.spatial.distance import cosine
-
-from hydroutils import hydro_plot as hplt
-
-
-def read_layer_name_from_tb_hist(hist_cols):
-    layer_names = []
-    for col in hist_cols:
-        if "counts" in col:
-            layer_name = col.split("/")[0]
-            if layer_name not in layer_names:
-                layer_names.append(layer_name)
-    return layer_names
-
-
-def epochs_hist_for_chosen_layer(epoch_interval, layer_name, df_hist):
-    df = pd.DataFrame()
-    all_epochs = df_hist.shape[0]
-    limit_uppers = []
-    limit_lowers = []
-    for i in range(0, all_epochs, epoch_interval):
-        limits = df_hist[layer_name + "/limits"][i]
-        limit_uppers.append(limits.max())
-        limit_lowers.append(limits.min())
-    for i in range(0, all_epochs, epoch_interval):
-        counts = df_hist[layer_name + "/counts"][i]
-        limits = df_hist[layer_name + "/limits"][i]
-        x, y = SummaryReader.histogram_to_bins(
-            counts,
-            limits,
-            lower_bound=min(limit_lowers),
-            upper_bound=max(limit_uppers),
-            # n_bins=100,
-        )
-        df[i] = y
-    df.index = x
-    return df
-
-
-def plot_layer_hist_for_basin_model_fold(
-    model_name,
-    chosen_layer_values,
-    layers,
-    save_fig_dir,
-    cmap_str="Oranges",
-):
-    """_summary_
-
-    Parameters
-    ----------
-    model_name : _type_
-        _description_
-    chosen_layer_values : _type_
-        _description_
-    layers : _type_
-        _description_
-    bsize : _type_
-        _description_
-    cmap_str : str, optional
-        chose from here: https://matplotlib.org/stable/tutorials/colors/colormaps.html#sequential, by default "Oranges"
-    """
-    if not os.path.exists(save_fig_dir):
-        os.makedirs(save_fig_dir)
-    for layer in layers:
-        two_model_layers = chosen_layer_values[layer]
-        try:
-            df_lstm_show = two_model_layers[model_name]
-        except KeyError:
-            # if the model does not have this layer, skip
-            continue
-        lstm_x_lst = []
-        lstm_y_lst = []
-        lstm_dash_lines = []
-        color_str = ""
-        lw_lst = []
-        alpha_lst = []
-        cmap = cm.get_cmap(cmap_str)
-        rgb_lst = []
-        norm_color = colors.Normalize(vmin=0, vmax=df_lstm_show.shape[1])
-        for i in df_lstm_show:
-            lstm_x_lst.append(df_lstm_show.index.values)
-            lstm_y_lst.append(df_lstm_show[i].values)
-            lstm_dash_lines.append(True)
-            color_str = color_str + "r"
-            rgba = cmap(norm_color(i))
-            rgb_lst.append(rgba)
-            alpha_lst.append(0.5)
-            lw_lst.append(0.5)
-        # the first and last line should be solid, have dark color and wide width
-        rgb_lst[0] = rgba
-        lstm_dash_lines[-1] = False
-        alpha_lst[-1] = 1
-        alpha_lst[0] = 1
-        lw_lst[-1] = 1
-        lw_lst[0] = 1
-        hplt.plot_ts(
-            lstm_x_lst,
-            lstm_y_lst,
-            dash_lines=lstm_dash_lines,
-            fig_size=(8, 4),
-            xlabel="weight_bias_value",
-            ylabel="hist_num",
-            # c_lst=color_str,
-            c_lst=rgb_lst,
-            linewidth=lw_lst,
-            alpha=alpha_lst,
-            leg_lst=None,
-        )
-        plt.savefig(
-            os.path.join(
-                save_fig_dir,
-                f"{model_name}_{layer}_hist.png",
-            ),
-            dpi=600,
-            bbox_inches="tight",
-        )
-
-
-def chosen_layer_in_layers(layers, chosen_layers):
-    the_layers = []
-    for layer in layers:
-        the_layers.extend(
-            layer for a_chosen_layer in chosen_layers if a_chosen_layer in layer
-        )
-    return the_layers
-
-
-def get_latest_event_file(event_file_lst):
-    """Get the latest event file in the current directory.
-
-    Returns
-    -------
-    str
-        The latest event file.
-    """
-    event_files = [Path(f) for f in event_file_lst]
-    event_file_names_lst = [event_file.stem.split(".") for event_file in event_files]
-    ctimes = [
-        int(event_file_names[event_file_names.index("tfevents") + 1])
-        for event_file_names in event_file_names_lst
-    ]
-    return event_files[ctimes.index(max(ctimes))]
-
-
-def copy_latest_tblog_file(log_dir, result_dir):
-    if not os.path.exists(result_dir):
-        os.makedirs(result_dir)
-        copy_lst = [
-            os.path.join(log_dir, f)
-            for f in os.listdir(log_dir)
-            if f.startswith("events")
-        ]
-        copy_file = get_latest_event_file(copy_lst)
-        shutil.copy(copy_file, result_dir)
-
-
-def read_tb_log(the_exp_dir, shown_batchsize, where_save=None):
-    """Copy a recent log file to the current directory and read the log file.
-
-    Parameters
-    ----------
-    the_exp_dir : str
-        saving directory for one experiment
-    shown_batchsize : int
-        batch size for the experiment
-    where_save : str, optional
-        A directory for saving plots, by default None,
-        which means same directory as the_exp_dir.
-        The reason we use a new dir different from the_exp_dir is that
-        ... (I forgot why... haha)
-
-    Returns
-    -------
-    _type_
-        _description_
-
-    Raises
-    ------
-    FileNotFoundError
-        _description_
-    """
-    log_dir = os.path.join(
-        the_exp_dir,
-        f"opt_Adadelta_lr_1.0_bsize_{str(shown_batchsize)}",
-    )
-    if not os.path.exists(log_dir):
-        raise FileNotFoundError(f"Log dir {log_dir} not found!")
-    if where_save is None:
-        where_save = the_exp_dir
-        plot_save_dir = os.path.join(
-            where_save,
-            f"opt_Adadelta_lr_1.0_bsize_{str(shown_batchsize)}",
-        )
-    else:
-        plot_save_dir = os.path.join(
-            where_save,
-            f"opt_Adadelta_lr_1.0_bsize_{str(shown_batchsize)}",
-        )
-        copy_latest_tblog_file(log_dir, plot_save_dir)
-    scalar_file = os.path.join(plot_save_dir, "scalars.csv")
-    if not os.path.exists(scalar_file):
-        reader = SummaryReader(plot_save_dir)
-        df_scalar = reader.scalars
-        df_scalar.to_csv(scalar_file, index=False)
-    else:
-        df_scalar = pd.read_csv(scalar_file)
-
-    # reader = SummaryReader(result_dir)
-    histgram_file = os.path.join(plot_save_dir, "histograms.pkl")
-    if not os.path.exists(histgram_file):
-        reader = SummaryReader(plot_save_dir, pivot=True)
-        df_histgram = reader.histograms
-        # https://www.statology.org/pandas-save-dataframe/
-        df_histgram.to_pickle(histgram_file)
-    else:
-        df_histgram = pd.read_pickle(histgram_file)
-    return df_scalar, df_histgram
-
-
-# plot param hist for each basin
-def plot_param_hist_model(
-    model_name,
-    the_exp_dir,
-    batchsize,
-    chosen_layer_for_hist,
-    start_epoch=0,
-    end_epoch=100,
-    epoch_interval=10,
-    save_fig_dir=None,
-):
-    """plot paramter histogram for each basin
-
-    Parameters
-    ----------
-    model_name: str
-        name of a DL model
-    the_exp_dir : str
-        saving directory for one experiment
-    batchsize : int
-        batch size
-    chosen_layer_for_hist : _type_
-        _description_
-
-    Returns
-    -------
-    _type_
-        _description_
-    """
-    chosen_layer_values = {layer: {} for layer in chosen_layer_for_hist}
-    chosen_layer_values_consine = {layer: {} for layer in chosen_layer_for_hist}
-    _, df_histgram = read_tb_log(the_exp_dir, batchsize)
-    hist_cols = df_histgram.columns.values
-    model_layers = read_layer_name_from_tb_hist(hist_cols)
-    chosen_layers = chosen_layer_in_layers(model_layers, chosen_layer_for_hist)
-    k = 0
-    for layer in chosen_layer_for_hist:
-        if layer not in chosen_layers[k]:
-            continue
-        df_epochs_hist = epochs_hist_for_chosen_layer(
-            epoch_interval, chosen_layers[k], df_histgram
-        )
-        chosen_layer_values[layer][model_name] = df_epochs_hist
-        end_epoch_idx = int((end_epoch / epoch_interval - 1) * epoch_interval)
-        chosen_layer_values_consine[layer][model_name] = 1 - cosine(
-            df_epochs_hist[start_epoch], df_epochs_hist[end_epoch_idx]
-        )
-        k = k + 1
-    if save_fig_dir is None:
-        save_fig_dir = the_exp_dir
-    plot_layer_hist_for_basin_model_fold(
-        model_name,
-        chosen_layer_values,
-        chosen_layer_for_hist,
-        save_fig_dir=save_fig_dir,
-        cmap_str="Reds",
-    )
-    return chosen_layer_values, chosen_layer_values_consine
-
-
-def merge_value(arrs_lst):
-    arrs = np.array(arrs_lst)
-    return np.mean(arrs, axis=0)
+import os
+from pathlib import Path
+import shutil
+import numpy as np
+import pandas as pd
+from tbparse import SummaryReader
+from matplotlib import cm, colors, pyplot as plt
+from scipy.spatial.distance import cosine
+
+from hydroutils import hydro_plot as hplt
+
+
+def read_layer_name_from_tb_hist(hist_cols):
+    layer_names = []
+    for col in hist_cols:
+        if "counts" in col:
+            layer_name = col.split("/")[0]
+            if layer_name not in layer_names:
+                layer_names.append(layer_name)
+    return layer_names
+
+
+def epochs_hist_for_chosen_layer(epoch_interval, layer_name, df_hist):
+    df = pd.DataFrame()
+    all_epochs = df_hist.shape[0]
+    limit_uppers = []
+    limit_lowers = []
+    for i in range(0, all_epochs, epoch_interval):
+        limits = df_hist[layer_name + "/limits"][i]
+        limit_uppers.append(limits.max())
+        limit_lowers.append(limits.min())
+    for i in range(0, all_epochs, epoch_interval):
+        counts = df_hist[layer_name + "/counts"][i]
+        limits = df_hist[layer_name + "/limits"][i]
+        x, y = SummaryReader.histogram_to_bins(
+            counts,
+            limits,
+            lower_bound=min(limit_lowers),
+            upper_bound=max(limit_uppers),
+            # n_bins=100,
+        )
+        df[i] = y
+    df.index = x
+    return df
+
+
+def plot_layer_hist_for_basin_model_fold(
+    model_name,
+    chosen_layer_values,
+    layers,
+    save_fig_dir,
+    cmap_str="Oranges",
+):
+    """_summary_
+
+    Parameters
+    ----------
+    model_name : _type_
+        _description_
+    chosen_layer_values : _type_
+        _description_
+    layers : _type_
+        _description_
+    bsize : _type_
+        _description_
+    cmap_str : str, optional
+        chose from here: https://matplotlib.org/stable/tutorials/colors/colormaps.html#sequential, by default "Oranges"
+    """
+    if not os.path.exists(save_fig_dir):
+        os.makedirs(save_fig_dir)
+    for layer in layers:
+        two_model_layers = chosen_layer_values[layer]
+        try:
+            df_lstm_show = two_model_layers[model_name]
+        except KeyError:
+            # if the model does not have this layer, skip
+            continue
+        lstm_x_lst = []
+        lstm_y_lst = []
+        lstm_dash_lines = []
+        color_str = ""
+        lw_lst = []
+        alpha_lst = []
+        cmap = cm.get_cmap(cmap_str)
+        rgb_lst = []
+        norm_color = colors.Normalize(vmin=0, vmax=df_lstm_show.shape[1])
+        for i in df_lstm_show:
+            lstm_x_lst.append(df_lstm_show.index.values)
+            lstm_y_lst.append(df_lstm_show[i].values)
+            lstm_dash_lines.append(True)
+            color_str = color_str + "r"
+            rgba = cmap(norm_color(i))
+            rgb_lst.append(rgba)
+            alpha_lst.append(0.5)
+            lw_lst.append(0.5)
+        # the first and last line should be solid, have dark color and wide width
+        rgb_lst[0] = rgba
+        lstm_dash_lines[-1] = False
+        alpha_lst[-1] = 1
+        alpha_lst[0] = 1
+        lw_lst[-1] = 1
+        lw_lst[0] = 1
+        hplt.plot_ts(
+            lstm_x_lst,
+            lstm_y_lst,
+            dash_lines=lstm_dash_lines,
+            fig_size=(8, 4),
+            xlabel="weight_bias_value",
+            ylabel="hist_num",
+            # c_lst=color_str,
+            c_lst=rgb_lst,
+            linewidth=lw_lst,
+            alpha=alpha_lst,
+            leg_lst=None,
+        )
+        plt.savefig(
+            os.path.join(
+                save_fig_dir,
+                f"{model_name}_{layer}_hist.png",
+            ),
+            dpi=600,
+            bbox_inches="tight",
+        )
+
+
+def chosen_layer_in_layers(layers, chosen_layers):
+    the_layers = []
+    for layer in layers:
+        the_layers.extend(
+            layer for a_chosen_layer in chosen_layers if a_chosen_layer in layer
+        )
+    return the_layers
+
+
+def get_latest_event_file(event_file_lst):
+    """Get the latest event file in the current directory.
+
+    Returns
+    -------
+    str
+        The latest event file.
+    """
+    event_files = [Path(f) for f in event_file_lst]
+    event_file_names_lst = [event_file.stem.split(".") for event_file in event_files]
+    ctimes = [
+        int(event_file_names[event_file_names.index("tfevents") + 1])
+        for event_file_names in event_file_names_lst
+    ]
+    return event_files[ctimes.index(max(ctimes))]
+
+
+def copy_latest_tblog_file(log_dir, result_dir):
+    if not os.path.exists(result_dir):
+        os.makedirs(result_dir)
+        copy_lst = [
+            os.path.join(log_dir, f)
+            for f in os.listdir(log_dir)
+            if f.startswith("events")
+        ]
+        copy_file = get_latest_event_file(copy_lst)
+        shutil.copy(copy_file, result_dir)
+
+
+def read_tb_log(the_exp_dir, shown_batchsize, where_save=None):
+    """Copy a recent log file to the current directory and read the log file.
+
+    Parameters
+    ----------
+    the_exp_dir : str
+        saving directory for one experiment
+    shown_batchsize : int
+        batch size for the experiment
+    where_save : str, optional
+        A directory for saving plots, by default None,
+        which means same directory as the_exp_dir.
+        The reason we use a new dir different from the_exp_dir is that
+        ... (I forgot why... haha)
+
+    Returns
+    -------
+    _type_
+        _description_
+
+    Raises
+    ------
+    FileNotFoundError
+        _description_
+    """
+    log_dir = os.path.join(
+        the_exp_dir,
+        f"opt_Adadelta_lr_1.0_bsize_{str(shown_batchsize)}",
+    )
+    if not os.path.exists(log_dir):
+        raise FileNotFoundError(f"Log dir {log_dir} not found!")
+    if where_save is None:
+        where_save = the_exp_dir
+        plot_save_dir = os.path.join(
+            where_save,
+            f"opt_Adadelta_lr_1.0_bsize_{str(shown_batchsize)}",
+        )
+    else:
+        plot_save_dir = os.path.join(
+            where_save,
+            f"opt_Adadelta_lr_1.0_bsize_{str(shown_batchsize)}",
+        )
+        copy_latest_tblog_file(log_dir, plot_save_dir)
+    scalar_file = os.path.join(plot_save_dir, "scalars.csv")
+    if not os.path.exists(scalar_file):
+        reader = SummaryReader(plot_save_dir)
+        df_scalar = reader.scalars
+        df_scalar.to_csv(scalar_file, index=False)
+    else:
+        df_scalar = pd.read_csv(scalar_file)
+
+    # reader = SummaryReader(result_dir)
+    histgram_file = os.path.join(plot_save_dir, "histograms.pkl")
+    if not os.path.exists(histgram_file):
+        reader = SummaryReader(plot_save_dir, pivot=True)
+        df_histgram = reader.histograms
+        # https://www.statology.org/pandas-save-dataframe/
+        df_histgram.to_pickle(histgram_file)
+    else:
+        df_histgram = pd.read_pickle(histgram_file)
+    return df_scalar, df_histgram
+
+
+# plot param hist for each basin
+def plot_param_hist_model(
+    model_name,
+    the_exp_dir,
+    batchsize,
+    chosen_layer_for_hist,
+    start_epoch=0,
+    end_epoch=100,
+    epoch_interval=10,
+    save_fig_dir=None,
+):
+    """plot paramter histogram for each basin
+
+    Parameters
+    ----------
+    model_name: str
+        name of a DL model
+    the_exp_dir : str
+        saving directory for one experiment
+    batchsize : int
+        batch size
+    chosen_layer_for_hist : _type_
+        _description_
+
+    Returns
+    -------
+    _type_
+        _description_
+    """
+    chosen_layer_values = {layer: {} for layer in chosen_layer_for_hist}
+    chosen_layer_values_consine = {layer: {} for layer in chosen_layer_for_hist}
+    _, df_histgram = read_tb_log(the_exp_dir, batchsize)
+    hist_cols = df_histgram.columns.values
+    model_layers = read_layer_name_from_tb_hist(hist_cols)
+    chosen_layers = chosen_layer_in_layers(model_layers, chosen_layer_for_hist)
+    k = 0
+    for layer in chosen_layer_for_hist:
+        if layer not in chosen_layers[k]:
+            continue
+        df_epochs_hist = epochs_hist_for_chosen_layer(
+            epoch_interval, chosen_layers[k], df_histgram
+        )
+        chosen_layer_values[layer][model_name] = df_epochs_hist
+        end_epoch_idx = int((end_epoch / epoch_interval - 1) * epoch_interval)
+        chosen_layer_values_consine[layer][model_name] = 1 - cosine(
+            df_epochs_hist[start_epoch], df_epochs_hist[end_epoch_idx]
+        )
+        k = k + 1
+    if save_fig_dir is None:
+        save_fig_dir = the_exp_dir
+    plot_layer_hist_for_basin_model_fold(
+        model_name,
+        chosen_layer_values,
+        chosen_layer_for_hist,
+        save_fig_dir=save_fig_dir,
+        cmap_str="Reds",
+    )
+    return chosen_layer_values, chosen_layer_values_consine
+
+
+def merge_value(arrs_lst):
+    arrs = np.array(arrs_lst)
+    return np.mean(arrs, axis=0)
```

### Comparing `torchhydro-0.0.4/torchhydro/models/ann.py` & `torchhydro-0.0.5/torchhydro/models/ann.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-"""
-Author: Wenyu Ouyang
-Date: 2021-12-17 18:02:27
-LastEditTime: 2023-10-06 19:26:09
-LastEditors: Wenyu Ouyang
-Description: ANN model
-FilePath: \torchhydro\torchhydro\models\ann.py
-Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
-"""
-from typing import Union
-
-import torch
-import torch.nn.functional as F
-
-
-class SimpleAnn(torch.nn.Module):
-    def __init__(self, nx: int, ny: int, hidden_size: Union[int, tuple, list] = None,
-                 dr: Union[float, tuple, list] = 0.0):
-        """
-        A simple multi-layer NN model with final linear layer
-
-        Parameters
-        ----------
-        nx
-            number of input neurons
-        ny
-            number of output neurons
-        hidden_size
-            a list/tuple which contains number of neurons in each hidden layer;
-            if int, only one hidden layer except for hidden_size=0
-        dr
-            dropout rate of layers, default is 0.0 which means no dropout;
-            here we set number of dropout layers to (number of nn layers - 1)
-        """
-        super(SimpleAnn, self).__init__()
-        linear_list = torch.nn.ModuleList()
-        dropout_list = torch.nn.ModuleList()
-        if (
-                hidden_size is None
-                or (type(hidden_size) is int and hidden_size == 0)
-                or (type(hidden_size) in [tuple, list] and len(hidden_size) < 1)
-        ):
-            linear_list.add_module("linear1", torch.nn.Linear(nx, ny))
-        elif type(hidden_size) is int:
-            if type(dr) in [tuple, list]:
-                dr = dr[0]
-            linear_list.add_module("linear1", torch.nn.Linear(nx, hidden_size))
-            # dropout layer do not have additional weights, so we do not name them here
-            dropout_list.append(torch.nn.Dropout(dr))
-            linear_list.add_module("linear2", torch.nn.Linear(hidden_size, ny))
-        else:
-            linear_list.add_module("linear1", torch.nn.Linear(nx, hidden_size[0]))
-            if type(dr) is float:
-                dr = [dr] * len(hidden_size)
-            elif len(dr) != len(hidden_size):
-                raise ArithmeticError(
-                    "We set dropout layer for each nn layer, please check the number of dropout layers")
-            # dropout_list.add_module("dropout1", torch.nn.Dropout(dr[0]))
-            dropout_list.append(torch.nn.Dropout(dr[0]))
-            for i in range(len(hidden_size) - 1):
-                linear_list.add_module(
-                    "linear%d" % (i + 1 + 1),
-                    torch.nn.Linear(hidden_size[i], hidden_size[i + 1]),
-                )
-                dropout_list.append(
-                    torch.nn.Dropout(dr[i + 1]),
-                )
-            linear_list.add_module(
-                "linear%d" % (len(hidden_size) + 1),
-                torch.nn.Linear(hidden_size[-1], ny),
-            )
-        self.linear_list = linear_list
-        self.dropout_list = dropout_list
-
-    def forward(self, x):
-        for i, model in enumerate(self.linear_list):
-            if i == 0:
-                if len(self.linear_list) == 1:
-                    return model(x)
-                else:
-                    out = F.relu(self.dropout_list[i](model(x)))
-            elif i == len(self.linear_list) - 1:
-                # in final layer, no relu again
-                return model(out)
-            else:
-                out = F.relu(self.dropout_list[i](model(out)))
+"""
+Author: Wenyu Ouyang
+Date: 2021-12-17 18:02:27
+LastEditTime: 2023-10-06 19:26:09
+LastEditors: Wenyu Ouyang
+Description: ANN model
+FilePath: \torchhydro\torchhydro\models\ann.py
+Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
+"""
+from typing import Union
+
+import torch
+import torch.nn.functional as F
+
+
+class SimpleAnn(torch.nn.Module):
+    def __init__(self, nx: int, ny: int, hidden_size: Union[int, tuple, list] = None,
+                 dr: Union[float, tuple, list] = 0.0):
+        """
+        A simple multi-layer NN model with final linear layer
+
+        Parameters
+        ----------
+        nx
+            number of input neurons
+        ny
+            number of output neurons
+        hidden_size
+            a list/tuple which contains number of neurons in each hidden layer;
+            if int, only one hidden layer except for hidden_size=0
+        dr
+            dropout rate of layers, default is 0.0 which means no dropout;
+            here we set number of dropout layers to (number of nn layers - 1)
+        """
+        super(SimpleAnn, self).__init__()
+        linear_list = torch.nn.ModuleList()
+        dropout_list = torch.nn.ModuleList()
+        if (
+                hidden_size is None
+                or (type(hidden_size) is int and hidden_size == 0)
+                or (type(hidden_size) in [tuple, list] and len(hidden_size) < 1)
+        ):
+            linear_list.add_module("linear1", torch.nn.Linear(nx, ny))
+        elif type(hidden_size) is int:
+            if type(dr) in [tuple, list]:
+                dr = dr[0]
+            linear_list.add_module("linear1", torch.nn.Linear(nx, hidden_size))
+            # dropout layer do not have additional weights, so we do not name them here
+            dropout_list.append(torch.nn.Dropout(dr))
+            linear_list.add_module("linear2", torch.nn.Linear(hidden_size, ny))
+        else:
+            linear_list.add_module("linear1", torch.nn.Linear(nx, hidden_size[0]))
+            if type(dr) is float:
+                dr = [dr] * len(hidden_size)
+            elif len(dr) != len(hidden_size):
+                raise ArithmeticError(
+                    "We set dropout layer for each nn layer, please check the number of dropout layers")
+            # dropout_list.add_module("dropout1", torch.nn.Dropout(dr[0]))
+            dropout_list.append(torch.nn.Dropout(dr[0]))
+            for i in range(len(hidden_size) - 1):
+                linear_list.add_module(
+                    "linear%d" % (i + 1 + 1),
+                    torch.nn.Linear(hidden_size[i], hidden_size[i + 1]),
+                )
+                dropout_list.append(
+                    torch.nn.Dropout(dr[i + 1]),
+                )
+            linear_list.add_module(
+                "linear%d" % (len(hidden_size) + 1),
+                torch.nn.Linear(hidden_size[-1], ny),
+            )
+        self.linear_list = linear_list
+        self.dropout_list = dropout_list
+
+    def forward(self, x):
+        for i, model in enumerate(self.linear_list):
+            if i == 0:
+                if len(self.linear_list) == 1:
+                    return model(x)
+                else:
+                    out = F.relu(self.dropout_list[i](model(x)))
+            elif i == len(self.linear_list) - 1:
+                # in final layer, no relu again
+                return model(out)
+            else:
+                out = F.relu(self.dropout_list[i](model(out)))
```

### Comparing `torchhydro-0.0.4/torchhydro/models/crits.py` & `torchhydro-0.0.5/torchhydro/models/crits.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,753 +1,791 @@
-"""
-Author: Wenyu Ouyang
-Date: 2021-12-31 11:08:29
-LastEditTime: 2023-07-29 10:53:25
-LastEditors: Wenyu Ouyang
-Description: Loss functions
-FilePath: \HydroTL\hydrotl\models\crits.py
-Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
-"""
-from typing import Union
-
-import torch
-from torch import distributions as tdist, Tensor
-from torchhydro.models.model_utils import get_the_device
-
-
-def deal_gap_data(output, target, data_gap, device):
-    """
-    How to handle with gap data
-
-    When there are NaN values in observation, we will perform a "reduce" operation on prediction.
-    For example, pred = [0,1,2,3,4], obs=[5, nan, nan, 6, nan]; the "reduce" is sum;
-    then, pred_sum = [0+1+2, 3+4], obs_sum=[5,6], loss = loss_func(pred_sum, obs_sum).
-    Notice: when "sum", actually final index is not chosen,
-    because the whole observation may be [5, nan, nan, 6, nan, nan, 7, nan, nan], 6 means sum of three elements.
-    Just as the rho is 5, the final one is not chosen
-
-    Parameters
-    ----------
-    output
-        model output for k-th variable
-    target
-        target for k-th variable
-    data_gap
-        data_gap=1: reduce is sum
-        data_gap=2: reduce is mean
-    device
-        where to save the data
-
-    Returns
-    -------
-    tuple[tensor, tensor]
-        output and target after dealing with gap
-    """
-    # all members in a batch has different NaN-gap, so we need a loop
-    seg_p_lst = []
-    seg_t_lst = []
-    for j in range(target.shape[1]):
-        non_nan_idx = [
-            i for i in range(len(target[:, j])) if not torch.isnan(target[i, j])
-        ]
-        scatter_index = []
-        idx_tmp = 0
-        if not non_nan_idx:
-            raise ArithmeticError("All NaN elements, please check your data")
-        for i in range(non_nan_idx[0], len(target[:, j])):
-            if i > non_nan_idx[0] and (not torch.isnan(target[i, j])):
-                idx_tmp = idx_tmp + 1
-            scatter_index.append(idx_tmp)
-        if data_gap == 1:
-            seg = segment_csr(
-                output[:, j],
-                torch.tensor(non_nan_idx).to(device=device),
-                reduce="sum",
-            )
-        elif data_gap == 2:
-            if non_nan_idx[-1] != len(target[:, j]):
-                # this will be used in t_j = target[non_nan_idx[:-1], j, k]
-                non_nan_idx += [len(target[:, j])]
-            seg = scatter(
-                output[non_nan_idx[0] :, j],
-                torch.tensor(scatter_index).to(device=device),
-                reduce="mean",
-            )
-                    # the following code cause grad nan, so we use scatter rather than segment_csr.
-                    # But notice start index of output become non_nan_idx[0] rather than 0
-                    # seg = segment_csr(output[:, j], torch.tensor(non_nan_idx).to(device=self.device),
-                    #                   reduce="mean")
-        else:
-            raise NotImplementedError(
-                "We have not provided this reduce way now!! Please choose 1 or 2!!"
-            )
-        seg_p_lst.append(seg)
-        # t0_j = target[:, j, k]
-        # mask_j = t0_j == t0_j
-        # t_j = t0_j[mask_j]
-        # Accordingly, we only chose target[non_nan_idx[:-1], j, k] rather than [non_nan_idx, j, k]
-        t_j = target[non_nan_idx[:-1], j]
-        seg_t_lst.append(t_j)
-    p = torch.cat(seg_p_lst)
-    t = torch.cat(seg_t_lst)
-    return p, t
-
-
-class SigmaLoss(torch.nn.Module):
-    def __init__(self, prior="gauss"):
-        super(SigmaLoss, self).__init__()
-        self.reduction = "elementwise_mean"
-        self.prior = None if prior == "" else prior.split("+")
-
-    def forward(self, output, target):
-        ny = target.shape[-1]
-        lossMean = 0
-        for k in range(ny):
-            p0 = output[:, :, k * 2]
-            s0 = output[:, :, k * 2 + 1]
-            t0 = target[:, :, k]
-            mask = t0 == t0
-            p = p0[mask]
-            s = s0[mask]
-            t = t0[mask]
-            if self.prior[0] == "gauss":
-                loss = torch.exp(-s).mul((p - t) ** 2) / 2 + s / 2
-            elif self.prior[0] == "invGamma":
-                c1 = float(self.prior[1])
-                c2 = float(self.prior[2])
-                nt = p.shape[0]
-                loss = (
-                    torch.exp(-s).mul((p - t) ** 2 + c2 / nt) / 2
-                    + (1 / 2 + c1 / nt) * s
-                )
-            lossMean = lossMean + torch.mean(loss)
-        return lossMean
-
-
-class NSELoss(torch.nn.Module):
-    # Same as Fredrick 2019
-    def __init__(self):
-        super(NSELoss, self).__init__()
-
-    def forward(self, output, target):
-        Ngage = target.shape[1]
-        losssum = 0
-        nsample = 0
-        for ii in range(Ngage):
-            t0 = target[:, ii, 0]
-            mask = t0 == t0
-            if len(mask[mask]) > 0:
-                p0 = output[:, ii, 0]
-                p = p0[mask]
-                t = t0[mask]
-                tmean = t.mean()
-                SST = torch.sum((t - tmean) ** 2)
-                SSRes = torch.sum((t - p) ** 2)
-                temp = SSRes / ((torch.sqrt(SST) + 0.1) ** 2)
-                # original NSE
-                # temp = SSRes / SST
-                losssum = losssum + temp
-                nsample = nsample + 1
-        return losssum / nsample
-
-
-class MASELoss(torch.nn.Module):
-    def __init__(self, baseline_method):
-        """
-        This implements the MASE loss function (e.g. MAE_MODEL/MAE_NAIEVE)
-        """
-        super(MASELoss, self).__init__()
-        self.method_dict = {
-            "mean": lambda x, y: torch.mean(x, 1).unsqueeze(1).repeat(1, y[1], 1)
-        }
-        self.baseline_method = self.method_dict[baseline_method]
-
-    def forward(
-        self, target: torch.Tensor, output: torch.Tensor, train_data: torch.Tensor, m=1
-    ) -> torch.Tensor:
-        # Ugh why can't all tensors have batch size... Fixes for modern
-        if len(train_data.shape) < 3:
-            train_data = train_data.unsqueeze(0)
-        if m == 1 and len(target.shape) == 1:
-            output = output.unsqueeze(0)
-            output = output.unsqueeze(2)
-            target = target.unsqueeze(0)
-            target = target.unsqueeze(2)
-        if len(target.shape) == 2:
-            output = output.unsqueeze(0)
-            target = target.unsqueeze(0)
-        result_baseline = self.baseline_method(train_data, output.shape)
-        MAE = torch.nn.L1Loss()
-        mae2 = MAE(output, target)
-        mase4 = MAE(result_baseline, target)
-        # Prevent divison by zero/loss exploding
-        if mase4 < 0.001:
-            mase4 = 0.001
-        return mae2 / mase4
-
-
-class RMSELoss(torch.nn.Module):
-    def __init__(self, variance_penalty=0.0):
-        """
-        Calculate RMSE
-
-        using:
-            target -> True y
-            output -> Prediction by model
-            source: https://discuss.pytorch.org/t/rmse-loss-function/16540/3
-
-        Parameters
-        ----------
-        variance_penalty
-            penalty for big variance; default is 0
-        """
-        super().__init__()
-        self.mse = torch.nn.MSELoss()
-        self.variance_penalty = variance_penalty
-
-    def forward(self, output: torch.Tensor, target: torch.Tensor):
-        if len(output) <= 1 or self.variance_penalty <= 0.0:
-            return torch.sqrt(self.mse(target, output))
-        diff = torch.sub(target, output)
-        std_dev = torch.std(diff)
-        var_penalty = self.variance_penalty * std_dev
-
-        return torch.sqrt(self.mse(target, output)) + var_penalty
-
-
-class MAPELoss(torch.nn.Module):
-    """
-    Returns MAPE using:
-    target -> True y
-    output -> Predtion by model
-    """
-
-    def __init__(self, variance_penalty=0.0):
-        super().__init__()
-        self.variance_penalty = variance_penalty
-
-    def forward(self, output: torch.Tensor, target: torch.Tensor):
-        if len(output) > 1:
-            return torch.mean(
-                torch.abs(torch.sub(target, output) / target)
-            ) + self.variance_penalty * torch.std(torch.sub(target, output))
-        else:
-            return torch.mean(torch.abs(torch.sub(target, output) / target))
-
-
-class PenalizedMSELoss(torch.nn.Module):
-    """
-    Returns MSE using:
-    target -> True y
-    output -> Predtion by model
-    source: https://discuss.pytorch.org/t/rmse-loss-function/16540/3
-    """
-
-    def __init__(self, variance_penalty=0.0):
-        super().__init__()
-        self.mse = torch.nn.MSELoss()
-        self.variance_penalty = variance_penalty
-
-    def forward(self, output: torch.Tensor, target: torch.Tensor):
-        return self.mse(target, output) + self.variance_penalty * torch.std(
-            torch.sub(target, output)
-        )
-
-
-class GaussianLoss(torch.nn.Module):
-    def __init__(self, mu=0, sigma=0):
-        """Compute the negative log likelihood of Gaussian Distribution
-        From https://arxiv.org/abs/1907.00235
-        """
-        super(GaussianLoss, self).__init__()
-        self.mu = mu
-        self.sigma = sigma
-
-    def forward(self, x: torch.Tensor):
-        loss = -tdist.Normal(self.mu, self.sigma).log_prob(x)
-        return torch.sum(loss) / (loss.size(0) * loss.size(1))
-
-
-class QuantileLoss(torch.nn.Module):
-    """From https://medium.com/the-artificial-impostor/quantile-regression-part-2-6fdbc26b2629"""
-
-    def __init__(self, quantiles):
-        super().__init__()
-        self.quantiles = quantiles
-
-    def forward(self, preds, target):
-        assert not target.requires_grad
-        assert preds.size(0) == target.size(0)
-        losses = []
-        for i, q in enumerate(self.quantiles):
-            errors = target - preds[:, i]
-            losses.append(torch.max((q - 1) * errors, q * errors).unsqueeze(1))
-        return torch.mean(torch.sum(torch.cat(losses, dim=1), dim=1))
-
-
-class NegativeLogLikelihood(torch.nn.Module):
-    """
-    target -> True y
-    output -> predicted distribution
-    """
-
-    def __init__(self):
-        super().__init__()
-
-    def forward(self, output: torch.distributions, target: torch.Tensor):
-        """
-        calculates NegativeLogLikelihood
-        """
-        return -output.log_prob(target).sum()
-
-
-def l1_regularizer(model, lambda_l1=0.01):
-    """
-    source: https://stackoverflow.com/questions/58172188/how-to-add-l1-regularization-to-pytorch-nn-model
-    """
-    lossl1 = 0
-    for model_param_name, model_param_value in model.named_parameters():
-        if model_param_name.endswith("weight"):
-            lossl1 += lambda_l1 * model_param_value.abs().sum()
-        return lossl1
-
-
-def orth_regularizer(model, lambda_orth=0.01):
-    """
-    source: https://stackoverflow.com/questions/58172188/how-to-add-l1-regularization-to-pytorch-nn-model
-    """
-    lossorth = 0
-    for model_param_name, model_param_value in model.named_parameters():
-        if model_param_name.endswith("weight"):
-            param_flat = model_param_value.view(model_param_value.shape[0], -1)
-            sym = torch.mm(param_flat, torch.t(param_flat))
-            sym -= torch.eye(param_flat.shape[0])
-            lossorth += lambda_orth * sym.sum()
-
-        return lossorth
-
-
-class RmseLoss(torch.nn.Module):
-    def __init__(self):
-        """
-        RMSE loss which could ignore NaN values
-
-        Now we only support 3-d tensor and 1-d tensor
-        """
-        super(RmseLoss, self).__init__()
-
-    def forward(self, output, target):
-        if target.dim() == 1:
-            mask = target == target
-            p = output[mask]
-            t = target[mask]
-            return torch.sqrt(((p - t) ** 2).mean())
-        ny = target.shape[2]
-        loss = 0
-        for k in range(ny):
-            p0 = output[:, :, k]
-            t0 = target[:, :, k]
-            mask = t0 == t0
-            p = p0[mask]
-            t = t0[mask]
-            temp = torch.sqrt(((p - t) ** 2).mean())
-            loss = loss + temp
-        return loss
-
-
-class MultiOutLoss(torch.nn.Module):
-    def __init__(
-        self,
-        loss_funcs: Union[torch.nn.Module, list],
-        data_gap: list = None,
-        device: list = None,
-        limit_part: list = None,
-        item_weight: list = None,
-    ):
-        """
-        Loss function for multiple output
-
-        Parameters
-        ----------
-        loss_funcs
-            The loss functions for each output
-        data_gap
-            It belongs to the feature dim.
-            If 1, then the corresponding value is uniformly-spaced with NaN values filling the gap;
-            in addition, the first non-nan value means the aggregated value of the following interval,
-            for example, in [5, nan, nan, nan], 5 means all four data's sum, although the next 3 values are nan
-            hence the calculation is a little different;
-            if 2, the first non-nan value means the average value of the following interval,
-            for example, in [5, nan, nan, nan], 5 means all four data's mean value;
-            default is [0, 2]
-        device
-            the number of device: -1 -> "cpu" or "cuda:x" (x is 0, 1 or ...)
-        limit_part
-            when transfer learning, we may ignore some part;
-            the default is None, which means no ignorance;
-            other choices are list, such as [0], [0, 1] or [1,2,..];
-            0 means the first variable;
-            tensor is [seq, time, var] or [time, seq, var]
-        item_weight
-            use different weight for each item's loss;
-            for example, the default values [0.5, 0.5] means 0.5 * loss1 + 0.5 * loss2
-        """
-        if data_gap is None:
-            data_gap = [0, 2]
-        if device is None:
-            device = [0]
-        if item_weight is None:
-            item_weight = [0.5, 0.5]
-        super(MultiOutLoss, self).__init__()
-        self.loss_funcs = loss_funcs
-        self.data_gap = data_gap
-        self.device = get_the_device(device)
-        self.limit_part = limit_part
-        self.item_weight = item_weight
-
-    def forward(self, output: Tensor, target: Tensor):
-        """
-        Calculate the sum of losses for different variables
-
-        When there are NaN values in observation, we will perform a "reduce" operation on prediction.
-        For example, pred = [0,1,2,3,4], obs=[5, nan, nan, 6, nan]; the "reduce" is sum;
-        then, pred_sum = [0+1+2, 3+4], obs_sum=[5,6], loss = loss_func(pred_sum, obs_sum).
-        Notice: when "sum", actually final index is not chosen,
-        because the whole observation may be [5, nan, nan, 6, nan, nan, 7, nan, nan], 6 means sum of three elements.
-        Just as the rho is 5, the final one is not chosen
-
-
-        Parameters
-        ----------
-        output
-            the prediction tensor; 3-dims are time sequence, batch and feature, respectively
-        target
-            the observation tensor
-
-        Returns
-        -------
-        Tensor
-            Whole loss
-        """
-        n_out = target.shape[-1]
-        loss = 0
-        for k in range(n_out):
-            if self.limit_part is not None and k in self.limit_part:
-                continue
-            p0 = output[:, :, k]
-            t0 = target[:, :, k]
-            mask = t0 == t0
-            p = p0[mask]
-            t = t0[mask]
-            if self.data_gap[k] > 0:
-                p, t = deal_gap_data(p0, t0, self.data_gap[k], self.device)
-            if type(self.loss_funcs) is list:
-                temp = self.item_weight[k] * self.loss_funcs[k](p, t)
-            else:
-                temp = self.item_weight[k] * self.loss_funcs(p, t)
-            # sum of all k-th loss
-            loss = loss + temp
-        return loss
-
-
-# ref: https://github.com/median-research-group/LibMTL
-class UncertaintyWeights(torch.nn.Module):
-    r"""Uncertainty Weights (UW).
-
-    This method is proposed in `Multi-Task Learning Using Uncertainty to Weigh Losses for Scene Geometry and Semantics (CVPR 2018) <https://openaccess.thecvf.com/content_cvpr_2018/papers/Kendall_Multi-Task_Learning_Using_CVPR_2018_paper.pdf>`_ \
-    and implemented by us.
-
-    """
-
-    def __init__(
-        self,
-        loss_funcs: Union[torch.nn.Module, list],
-        data_gap: list = None,
-        device: list = None,
-        limit_part: list = None,
-    ):
-        if data_gap is None:
-            data_gap = [0, 2]
-        if device is None:
-            device = [0]
-        super(UncertaintyWeights, self).__init__()
-        self.loss_funcs = loss_funcs
-        self.data_gap = data_gap
-        self.device = get_the_device(device)
-        self.limit_part = limit_part
-
-    def forward(self, output, target, log_vars):
-        """
-
-        Parameters
-        ----------
-        output
-        target
-        log_vars
-            sigma in uncertainty weighting;
-            default is None, meaning we manually set weights for different target's loss;
-            more info could be seen in
-            https://libmtl.readthedocs.io/en/latest/docs/_autoapi/LibMTL/weighting/index.html#LibMTL.weighting.UW
-
-        Returns
-        -------
-        torch.Tensor
-            multi-task loss by uncertainty weighting method
-        """
-        n_out = target.shape[-1]
-        loss = 0
-        for k in range(n_out):
-            precision = torch.exp(-log_vars[k])
-            if self.limit_part is not None and k in self.limit_part:
-                continue
-            p0 = output[:, :, k]
-            t0 = target[:, :, k]
-            mask = t0 == t0
-            p = p0[mask]
-            t = t0[mask]
-            if self.data_gap[k] > 0:
-                p, t = deal_gap_data(p0, t0, self.data_gap[k], self.device)
-            if type(self.loss_funcs) is list:
-                temp = self.loss_funcs[k](p, t)
-            else:
-                temp = self.loss_funcs(p, t)
-            loss += torch.sum(precision * temp + log_vars[k], -1)
-        return loss
-
-
-# ref: https://openaccess.thecvf.com/content_ECCV_2018/html/Michelle_Guo_Focus_on_the_ECCV_2018_paper.html
-class DynamicTaskPrior(torch.nn.Module):
-    r"""Dynamic Task Prioritization
-
-    This method is proposed in https://openaccess.thecvf.com/content_ECCV_2018/html/Michelle_Guo_Focus_on_the_ECCV_2018_paper.html
-    In contrast to UW and other curriculum learning methods, where easy tasks are prioritized above difficult tasks,
-    It shows the importance of prioritizing difficult tasks first.
-    It automatically prioritize more difficult tasks by adaptively adjusting the mixing weight of each task’s loss.
-    Here we choose correlation as KPI. As KPI must be in [0,1], we set (corr+1)/2 as KPI
-    """
-
-    def __init__(
-        self,
-        loss_funcs: Union[torch.nn.Module, list],
-        data_gap: list = None,
-        device: list = None,
-        limit_part: list = None,
-        gamma=2,
-        alpha=0.5,
-    ):
-        """
-
-        Parameters
-        ----------
-        loss_funcs
-        data_gap
-        device
-        limit_part
-        gamma
-            the example-level focusing parameter
-        alpha
-            default is 1, which means we only use the newest KPI value
-        """
-        if data_gap is None:
-            data_gap = [0, 2]
-        if device is None:
-            device = [0]
-        super(DynamicTaskPrior, self).__init__()
-        self.loss_funcs = loss_funcs
-        self.data_gap = data_gap
-        self.device = get_the_device(device)
-        self.limit_part = limit_part
-        self.gamma = gamma
-        self.alpha = alpha
-
-    def forward(self, output, target, kpi_last=None):
-        """
-        Parameters
-        ----------
-        output
-            model's prediction
-        target
-            observation
-
-        kpi_last
-            the KPI value of last iteration; each element for an output
-            It use a moving average KPI as the weighting coefficient: KPI_i = alpha * KPI_i + (1-alpha) * KPI_{i-1}
-
-        Returns
-        -------
-        torch.Tensor
-            multi-task loss by Dynamic Task Prioritization method
-        """
-        n_out = target.shape[-1]
-        loss = 0
-        kpis = torch.zeros(n_out).to(self.device)
-        for k in range(n_out):
-            if self.limit_part is not None and k in self.limit_part:
-                continue
-            p0 = output[:, :, k]
-            t0 = target[:, :, k]
-            mask = t0 == t0
-            p = p0[mask]
-            t = t0[mask]
-            if self.data_gap[k] > 0:
-                p, t = deal_gap_data(p0, t0, self.data_gap[k], self.device)
-            if type(self.loss_funcs) is list:
-                temp = self.loss_funcs[k](p, t)
-            else:
-                temp = self.loss_funcs(p, t)
-            # kpi must be in [0, 1], as corr's range is [-1, 1], just trans corr to  (corr+1)/2
-            kpi = (torch.corrcoef(torch.stack([p, t], 1).T)[0, 1] + 1) / 2
-            if self.alpha < 1:
-                assert kpi_last is not None
-                kpi = kpi * self.alpha + kpi_last[k] * (1 - self.alpha)
-                # if we exclude kpi from the backward, it trans to a normal multi-task model
-                # kpi = kpi.detach().clone() * self.alpha + kpi_last[k] * (1 - self.alpha)
-            kpis[k] = kpi
-            # focal loss
-            fl = -((1 - kpi) ** self.gamma) * torch.log(kpi)
-            loss += torch.sum(fl * temp, -1)
-        # if kpi has grad_fn, backward will repeat. It won't work
-        return loss, kpis.detach().clone()
-
-
-class MultiOutWaterBalanceLoss(torch.nn.Module):
-    def __init__(self, loss_funcs: Union[torch.nn.Module, list], data_gap: list = None, device: list = None, limit_part: list = None, item_weight: list = None, alpha=0.5, beta=0.0, wb_loss_func=None, means=None, stds=None):
-        """
-        Loss function for multiple output considering water balance
-
-        loss = alpha * water_balance_loss + (1-alpha) * mtl_loss
-
-        This loss function is only for p, q, et now
-        we use the difference between p_obs_mean-q_obs_mean-et_obs_mean and p_pred_mean-q_pred_mean-et_pred_mean as water balance loss
-        which is the difference between (q_obs_mean + et_obs_mean) and (q_pred_mean + et_pred_mean)
-
-        Parameters
-        ----------
-        loss_funcs
-            The loss functions for each output
-        data_gap
-            It belongs to the feature dim.
-            If 1, then the corresponding value is uniformly-spaced with NaN values filling the gap;
-            in addition, the first non-nan value means the aggregated value of the following interval,
-            for example, in [5, nan, nan, nan], 5 means all four data's sum, although the next 3 values are nan
-            hence the calculation is a little different;
-            if 2, the first non-nan value means the average value of the following interval,
-            for example, in [5, nan, nan, nan], 5 means all four data's mean value;
-            default is [0, 2]
-        device
-            the number of device: -1 -> "cpu" or "cuda:x" (x is 0, 1 or ...)
-        limit_part
-            when transfer learning, we may ignore some part;
-            the default is None, which means no ignorance;
-            other choices are list, such as [0], [0, 1] or [1,2,..];
-            0 means the first variable;
-            tensor is [seq, time, var] or [time, seq, var]
-        item_weight
-            use different weight for each item's loss;
-            for example, the default values [0.5, 0.5] means 0.5 * loss1 + 0.5 * loss2
-        alpha
-            the weight of the water-balance item's loss
-        beta
-            the weight of real water-balance item's loss, et_mean/p_mean + q_mean/p_mean = 1 can be a loss.
-            It is not strictly correct as training batch only have about one year data, but still could be a constraint
-        wb_loss_func
-            the loss function for water balance item, by default it is None, which means we use function in loss_funcs
-        """
-        if data_gap is None:
-            data_gap = [0, 2]
-        if device is None:
-            device = [0]
-        if item_weight is None:
-            item_weight = [0.5, 0.5]
-        super(MultiOutWaterBalanceLoss, self).__init__()
-        self.loss_funcs = loss_funcs
-        self.data_gap = data_gap
-        self.device = get_the_device(device)
-        self.limit_part = limit_part
-        self.item_weight = item_weight
-        self.alpha = alpha
-        self.beta = beta
-        self.wb_loss_func = wb_loss_func
-        self.means = means
-        self.stds = stds
-
-    def forward(self, output: Tensor, target: Tensor):
-        """
-        Calculate the sum of losses for different variables and water-balance loss
-
-        When there are NaN values in observation, we will perform a "reduce" operation on prediction.
-        For example, pred = [0,1,2,3,4], obs=[5, nan, nan, 6, nan]; the "reduce" is sum;
-        then, pred_sum = [0+1+2, 3+4], obs_sum=[5,6], loss = loss_func(pred_sum, obs_sum).
-        Notice: when "sum", actually final index is not chosen,
-        because the whole observation may be [5, nan, nan, 6, nan, nan, 7, nan, nan], 6 means sum of three elements.
-        Just as the rho is 5, the final one is not chosen
-
-
-        Parameters
-        ----------
-        output
-            the prediction tensor; 3-dims are time sequence, batch and feature, respectively
-        target
-            the observation tensor
-
-        Returns
-        -------
-        Tensor
-            Whole loss
-        """
-        n_out = target.shape[-1]
-        loss = 0
-        p_means = []
-        t_means = []
-        all_means = self.means
-        all_stds = self.stds
-        for k in range(n_out):
-            if self.limit_part is not None and k in self.limit_part:
-                continue
-            p0 = output[:, :, k]
-            t0 = target[:, :, k]
-            # for water balance loss
-            if all_means is not None:
-                # denormalize for q and et
-                p1 = p0 * all_stds[k] + all_means[k]
-                t1 = t0 * all_stds[k] + all_means[k]
-                p2 = (10**p1 - 0.1) ** 2
-                t2 = (10**t1 - 0.1) ** 2
-                p_mean = torch.nanmean(p2, dim=0)
-                t_mean = torch.nanmean(t2, dim=0)
-            else:
-                p_mean = torch.nanmean(p0, dim=0)
-                t_mean = torch.nanmean(t0, dim=0)
-            p_means.append(p_mean)
-            t_means.append(t_mean)
-            # for mtl normal loss
-            mask = t0 == t0
-            p = p0[mask]
-            t = t0[mask]
-            if self.data_gap[k] > 0:
-                p, t = deal_gap_data(p0, t0, self.data_gap[k], self.device)
-            if type(self.loss_funcs) is list:
-                temp = self.item_weight[k] * self.loss_funcs[k](p, t)
-            else:
-                temp = self.item_weight[k] * self.loss_funcs(p, t)
-            # sum of all k-th loss
-            loss = loss + temp
-        # water balance loss
-        p_mean_q_plus_et = torch.sum(torch.stack(p_means), dim=0)
-        t_mean_q_plus_et = torch.sum(torch.stack(t_means), dim=0)
-        wb_ones = torch.ones_like(t_mean_q_plus_et)
-        if self.wb_loss_func is None:
-            if type(self.loss_funcs) is list:
-                # if wb_loss_func is None, we use the first loss function in loss_funcs
-                wb_loss = self.loss_funcs[0](p_mean_q_plus_et, t_mean_q_plus_et)
-                wb_1loss = self.loss_funcs[0](p_mean_q_plus_et, wb_ones)
-            else:
-                wb_loss = self.loss_funcs(p_mean_q_plus_et, t_mean_q_plus_et)
-                wb_1loss = self.loss_funcs(p_mean_q_plus_et, wb_ones)
-        else:
-            wb_loss = self.wb_loss_func(p_mean_q_plus_et, t_mean_q_plus_et)
-            wb_1loss = self.wb_loss_func(p_mean_q_plus_et, wb_ones)
-        return (
-            self.alpha * wb_loss
-            + (1 - self.alpha - self.beta) * loss
-            + self.beta * wb_1loss
-        )
+"""
+Author: Wenyu Ouyang
+Date: 2021-12-31 11:08:29
+LastEditTime: 2024-05-17 11:29:13
+LastEditors: Wenyu Ouyang
+Description: Loss functions
+FilePath: \torchhydro\torchhydro\models\crits.py
+Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
+"""
+
+from typing import Union
+import torch
+from torch import distributions as tdist, Tensor
+from torchhydro.models.model_utils import get_the_device
+
+
+def deal_gap_data(output, target, data_gap, device):
+    """
+    How to handle with gap data
+
+    When there are NaN values in observation, we will perform a "reduce" operation on prediction.
+    For example, pred = [0,1,2,3,4], obs=[5, nan, nan, 6, nan]; the "reduce" is sum;
+    then, pred_sum = [0+1+2, 3+4], obs_sum=[5,6], loss = loss_func(pred_sum, obs_sum).
+    Notice: when "sum", actually final index is not chosen,
+    because the whole observation may be [5, nan, nan, 6, nan, nan, 7, nan, nan], 6 means sum of three elements.
+    Just as the rho is 5, the final one is not chosen
+
+    Parameters
+    ----------
+    output
+        model output for k-th variable
+    target
+        target for k-th variable
+    data_gap
+        data_gap=1: reduce is sum
+        data_gap=2: reduce is mean
+    device
+        where to save the data
+
+    Returns
+    -------
+    tuple[tensor, tensor]
+        output and target after dealing with gap
+    """
+    # all members in a batch has different NaN-gap, so we need a loop
+    seg_p_lst = []
+    seg_t_lst = []
+    for j in range(target.shape[1]):
+        non_nan_idx = torch.nonzero(
+            ~torch.isnan(target[:, j]), as_tuple=False
+        ).squeeze()
+        if len(non_nan_idx) < 1:
+            raise ArithmeticError("All NaN elements, please check your data")
+
+        # 使用 cumsum 生成 scatter_index
+        is_not_nan = ~torch.isnan(target[:, j])
+        cumsum_is_not_nan = torch.cumsum(is_not_nan.to(torch.int), dim=0)
+        first_non_nan = non_nan_idx[0]
+        scatter_index = torch.full_like(
+            target[:, j], fill_value=-1, dtype=torch.long
+        )  # 将所有值初始化为 -1
+        scatter_index[first_non_nan:] = cumsum_is_not_nan[first_non_nan:] - 1
+        scatter_index = scatter_index.to(device=device)
+
+        # 创建掩码，只保留有效的索引
+        valid_mask = scatter_index >= 0
+
+        if data_gap == 1:
+            seg = torch.zeros(
+                len(non_nan_idx), device=device, dtype=output.dtype
+            ).scatter_add_(0, scatter_index[valid_mask], output[valid_mask, j])
+            # for sum, better exclude final non-nan value as it didn't include all necessary periods
+            seg_p_lst.append(seg[:-1])
+            seg_t_lst.append(target[non_nan_idx[:-1], j])
+
+        elif data_gap == 2:
+            counts = torch.zeros(
+                len(non_nan_idx), device=device, dtype=output.dtype
+            ).scatter_add_(
+                0,
+                scatter_index[valid_mask],
+                torch.ones_like(output[valid_mask, j], dtype=output.dtype),
+            )
+            seg = torch.zeros(
+                len(non_nan_idx), device=device, dtype=output.dtype
+            ).scatter_add_(0, scatter_index[valid_mask], output[valid_mask, j])
+            seg = seg / counts.clamp(min=1)
+            # for mean, we can include all periods
+            seg_p_lst.append(seg)
+            seg_t_lst.append(target[non_nan_idx, j])
+        else:
+            raise NotImplementedError(
+                "We have not provided this reduce way now!! Please choose 1 or 2!!"
+            )
+
+    p = torch.cat(seg_p_lst)
+    t = torch.cat(seg_t_lst)
+    return p, t
+
+
+class SigmaLoss(torch.nn.Module):
+    def __init__(self, prior="gauss"):
+        super(SigmaLoss, self).__init__()
+        self.reduction = "elementwise_mean"
+        self.prior = None if prior == "" else prior.split("+")
+
+    def forward(self, output, target):
+        ny = target.shape[-1]
+        lossMean = 0
+        for k in range(ny):
+            p0 = output[:, :, k * 2]
+            s0 = output[:, :, k * 2 + 1]
+            t0 = target[:, :, k]
+            mask = t0 == t0
+            p = p0[mask]
+            s = s0[mask]
+            t = t0[mask]
+            if self.prior[0] == "gauss":
+                loss = torch.exp(-s).mul((p - t) ** 2) / 2 + s / 2
+            elif self.prior[0] == "invGamma":
+                c1 = float(self.prior[1])
+                c2 = float(self.prior[2])
+                nt = p.shape[0]
+                loss = (
+                    torch.exp(-s).mul((p - t) ** 2 + c2 / nt) / 2
+                    + (1 / 2 + c1 / nt) * s
+                )
+            lossMean = lossMean + torch.mean(loss)
+        return lossMean
+
+
+class NSELoss(torch.nn.Module):
+    # Same as Fredrick 2019
+    def __init__(self):
+        super(NSELoss, self).__init__()
+
+    def forward(self, output, target):
+        Ngage = target.shape[1]
+        losssum = 0
+        nsample = 0
+        for ii in range(Ngage):
+            t0 = target[:, ii, 0]
+            mask = t0 == t0
+            if len(mask[mask]) > 0:
+                p0 = output[:, ii, 0]
+                p = p0[mask]
+                t = t0[mask]
+                tmean = t.mean()
+                SST = torch.sum((t - tmean) ** 2)
+                SSRes = torch.sum((t - p) ** 2)
+                temp = SSRes / ((torch.sqrt(SST) + 0.1) ** 2)
+                # original NSE
+                # temp = SSRes / SST
+                losssum = losssum + temp
+                nsample = nsample + 1
+        return losssum / nsample
+
+
+class MASELoss(torch.nn.Module):
+    def __init__(self, baseline_method):
+        """
+        This implements the MASE loss function (e.g. MAE_MODEL/MAE_NAIEVE)
+        """
+        super(MASELoss, self).__init__()
+        self.method_dict = {
+            "mean": lambda x, y: torch.mean(x, 1).unsqueeze(1).repeat(1, y[1], 1)
+        }
+        self.baseline_method = self.method_dict[baseline_method]
+
+    def forward(
+        self, target: torch.Tensor, output: torch.Tensor, train_data: torch.Tensor, m=1
+    ) -> torch.Tensor:
+        # Ugh why can't all tensors have batch size... Fixes for modern
+        if len(train_data.shape) < 3:
+            train_data = train_data.unsqueeze(0)
+        if m == 1 and len(target.shape) == 1:
+            output = output.unsqueeze(0)
+            output = output.unsqueeze(2)
+            target = target.unsqueeze(0)
+            target = target.unsqueeze(2)
+        if len(target.shape) == 2:
+            output = output.unsqueeze(0)
+            target = target.unsqueeze(0)
+        result_baseline = self.baseline_method(train_data, output.shape)
+        MAE = torch.nn.L1Loss()
+        mae2 = MAE(output, target)
+        mase4 = MAE(result_baseline, target)
+        # Prevent divison by zero/loss exploding
+        if mase4 < 0.001:
+            mase4 = 0.001
+        return mae2 / mase4
+
+
+class RMSELoss(torch.nn.Module):
+    def __init__(self, variance_penalty=0.0):
+        """
+        Calculate RMSE
+
+        using:
+            target -> True y
+            output -> Prediction by model
+            source: https://discuss.pytorch.org/t/rmse-loss-function/16540/3
+
+        Parameters
+        ----------
+        variance_penalty
+            penalty for big variance; default is 0
+        """
+        super().__init__()
+        self.mse = torch.nn.MSELoss()
+        self.variance_penalty = variance_penalty
+
+    def forward(self, output: torch.Tensor, target: torch.Tensor):
+        if len(output) <= 1 or self.variance_penalty <= 0.0:
+            return torch.sqrt(self.mse(target, output))
+        diff = torch.sub(target, output)
+        std_dev = torch.std(diff)
+        var_penalty = self.variance_penalty * std_dev
+
+        return torch.sqrt(self.mse(target, output)) + var_penalty
+
+
+class MAPELoss(torch.nn.Module):
+    """
+    Returns MAPE using:
+    target -> True y
+    output -> Predtion by model
+    """
+
+    def __init__(self, variance_penalty=0.0):
+        super().__init__()
+        self.variance_penalty = variance_penalty
+
+    def forward(self, output: torch.Tensor, target: torch.Tensor):
+        if len(output) > 1:
+            return torch.mean(
+                torch.abs(torch.sub(target, output) / target)
+            ) + self.variance_penalty * torch.std(torch.sub(target, output))
+        else:
+            return torch.mean(torch.abs(torch.sub(target, output) / target))
+
+
+class MAELoss(torch.nn.Module):
+    def __init__(self):
+        super().__init__()
+
+    def forward(self, output: torch.Tensor, target: torch.Tensor):
+        # Create a mask to filter out NaN values
+        mask = ~torch.isnan(target)
+
+        # Apply the mask to both target and output
+        target = target[mask]
+        output = output[mask]
+
+        # Calculate MAE for the non-NaN values
+        return torch.mean(torch.abs(target - output))
+
+
+class PenalizedMSELoss(torch.nn.Module):
+    """
+    Returns MSE using:
+    target -> True y
+    output -> Predtion by model
+    source: https://discuss.pytorch.org/t/rmse-loss-function/16540/3
+    """
+
+    def __init__(self, variance_penalty=0.0):
+        super().__init__()
+        self.mse = torch.nn.MSELoss()
+        self.variance_penalty = variance_penalty
+
+    def forward(self, output: torch.Tensor, target: torch.Tensor):
+        return self.mse(target, output) + self.variance_penalty * torch.std(
+            torch.sub(target, output)
+        )
+
+
+class GaussianLoss(torch.nn.Module):
+    def __init__(self, mu=0, sigma=0):
+        """Compute the negative log likelihood of Gaussian Distribution
+        From https://arxiv.org/abs/1907.00235
+        """
+        super(GaussianLoss, self).__init__()
+        self.mu = mu
+        self.sigma = sigma
+
+    def forward(self, x: torch.Tensor):
+        loss = -tdist.Normal(self.mu, self.sigma).log_prob(x)
+        return torch.sum(loss) / (loss.size(0) * loss.size(1))
+
+
+class QuantileLoss(torch.nn.Module):
+    """From https://medium.com/the-artificial-impostor/quantile-regression-part-2-6fdbc26b2629"""
+
+    def __init__(self, quantiles):
+        super().__init__()
+        self.quantiles = quantiles
+
+    def forward(self, preds, target):
+        assert not target.requires_grad
+        assert preds.size(0) == target.size(0)
+        losses = []
+        for i, q in enumerate(self.quantiles):
+            errors = target - preds[:, i]
+            losses.append(torch.max((q - 1) * errors, q * errors).unsqueeze(1))
+        return torch.mean(torch.sum(torch.cat(losses, dim=1), dim=1))
+
+
+class NegativeLogLikelihood(torch.nn.Module):
+    """
+    target -> True y
+    output -> predicted distribution
+    """
+
+    def __init__(self):
+        super().__init__()
+
+    def forward(self, output: torch.distributions, target: torch.Tensor):
+        """
+        calculates NegativeLogLikelihood
+        """
+        return -output.log_prob(target).sum()
+
+
+def l1_regularizer(model, lambda_l1=0.01):
+    """
+    source: https://stackoverflow.com/questions/58172188/how-to-add-l1-regularization-to-pytorch-nn-model
+    """
+    lossl1 = 0
+    for model_param_name, model_param_value in model.named_parameters():
+        if model_param_name.endswith("weight"):
+            lossl1 += lambda_l1 * model_param_value.abs().sum()
+        return lossl1
+
+
+def orth_regularizer(model, lambda_orth=0.01):
+    """
+    source: https://stackoverflow.com/questions/58172188/how-to-add-l1-regularization-to-pytorch-nn-model
+    """
+    lossorth = 0
+    for model_param_name, model_param_value in model.named_parameters():
+        if model_param_name.endswith("weight"):
+            param_flat = model_param_value.view(model_param_value.shape[0], -1)
+            sym = torch.mm(param_flat, torch.t(param_flat))
+            sym -= torch.eye(param_flat.shape[0])
+            lossorth += lambda_orth * sym.sum()
+
+        return lossorth
+
+
+class RmseLoss(torch.nn.Module):
+    def __init__(self):
+        """
+        RMSE loss which could ignore NaN values
+
+        Now we only support 3-d tensor and 1-d tensor
+        """
+        super(RmseLoss, self).__init__()
+
+    def forward(self, output, target):
+        if target.dim() == 1:
+            mask = target == target
+            p = output[mask]
+            t = target[mask]
+            return torch.sqrt(((p - t) ** 2).mean())
+        ny = target.shape[2]
+        loss = 0
+        for k in range(ny):
+            p0 = output[:, :, k]
+            t0 = target[:, :, k]
+            mask = t0 == t0
+            p = p0[mask]
+            p = torch.where(torch.isnan(p), torch.full_like(p, 0), p)
+            t = t0[mask]
+            t = torch.where(torch.isnan(t), torch.full_like(t, 0), t)
+            temp = torch.sqrt(((p - t) ** 2).mean())
+            loss = loss + temp
+        return loss
+
+
+class MultiOutLoss(torch.nn.Module):
+    def __init__(
+        self,
+        loss_funcs: Union[torch.nn.Module, list],
+        data_gap: list = None,
+        device: list = None,
+        limit_part: list = None,
+        item_weight: list = None,
+    ):
+        """
+        Loss function for multiple output
+
+        Parameters
+        ----------
+        loss_funcs
+            The loss functions for each output
+        data_gap
+            It belongs to the feature dim.
+            If 1, then the corresponding value is uniformly-spaced with NaN values filling the gap;
+            in addition, the first non-nan value means the aggregated value of the following interval,
+            for example, in [5, nan, nan, nan], 5 means all four data's sum, although the next 3 values are nan
+            hence the calculation is a little different;
+            if 2, the first non-nan value means the average value of the following interval,
+            for example, in [5, nan, nan, nan], 5 means all four data's mean value;
+            default is [0, 2]
+        device
+            the number of device: -1 -> "cpu" or "cuda:x" (x is 0, 1 or ...)
+        limit_part
+            when transfer learning, we may ignore some part;
+            the default is None, which means no ignorance;
+            other choices are list, such as [0], [0, 1] or [1,2,..];
+            0 means the first variable;
+            tensor is [seq, time, var] or [time, seq, var]
+        item_weight
+            use different weight for each item's loss;
+            for example, the default values [0.5, 0.5] means 0.5 * loss1 + 0.5 * loss2
+        """
+        if data_gap is None:
+            data_gap = [0, 2]
+        if device is None:
+            device = [0]
+        if item_weight is None:
+            item_weight = [0.5, 0.5]
+        super(MultiOutLoss, self).__init__()
+        self.loss_funcs = loss_funcs
+        self.data_gap = data_gap
+        self.device = get_the_device(device)
+        self.limit_part = limit_part
+        self.item_weight = item_weight
+
+    def forward(self, output: Tensor, target: Tensor):
+        """
+        Calculate the sum of losses for different variables
+
+        When there are NaN values in observation, we will perform a "reduce" operation on prediction.
+        For example, pred = [0,1,2,3,4], obs=[5, nan, nan, 6, nan]; the "reduce" is sum;
+        then, pred_sum = [0+1+2, 3+4], obs_sum=[5,6], loss = loss_func(pred_sum, obs_sum).
+        Notice: when "sum", actually final index is not chosen,
+        because the whole observation may be [5, nan, nan, 6, nan, nan, 7, nan, nan], 6 means sum of three elements.
+        Just as the rho is 5, the final one is not chosen
+
+
+        Parameters
+        ----------
+        output
+            the prediction tensor; 3-dims are time sequence, batch and feature, respectively
+        target
+            the observation tensor
+
+        Returns
+        -------
+        Tensor
+            Whole loss
+        """
+        n_out = target.shape[-1]
+        loss = 0
+        for k in range(n_out):
+            if self.limit_part is not None and k in self.limit_part:
+                continue
+            p0 = output[:, :, k]
+            t0 = target[:, :, k]
+            mask = t0 == t0
+            p = p0[mask]
+            t = t0[mask]
+            if self.data_gap[k] > 0:
+                p, t = deal_gap_data(p0, t0, self.data_gap[k], self.device)
+            if type(self.loss_funcs) is list:
+                temp = self.item_weight[k] * self.loss_funcs[k](p, t)
+            else:
+                temp = self.item_weight[k] * self.loss_funcs(p, t)
+            # sum of all k-th loss
+            if torch.isnan(temp).any():
+                continue
+            loss = loss + temp
+        return loss
+
+
+# ref: https://github.com/median-research-group/LibMTL
+class UncertaintyWeights(torch.nn.Module):
+    r"""Uncertainty Weights (UW).
+
+    This method is proposed in `Multi-Task Learning Using Uncertainty to Weigh Losses for Scene Geometry and Semantics (CVPR 2018) <https://openaccess.thecvf.com/content_cvpr_2018/papers/Kendall_Multi-Task_Learning_Using_CVPR_2018_paper.pdf>`_ \
+    and implemented by us.
+
+    """
+
+    def __init__(
+        self,
+        loss_funcs: Union[torch.nn.Module, list],
+        data_gap: list = None,
+        device: list = None,
+        limit_part: list = None,
+    ):
+        if data_gap is None:
+            data_gap = [0, 2]
+        if device is None:
+            device = [0]
+        super(UncertaintyWeights, self).__init__()
+        self.loss_funcs = loss_funcs
+        self.data_gap = data_gap
+        self.device = get_the_device(device)
+        self.limit_part = limit_part
+
+    def forward(self, output, target, log_vars):
+        """
+
+        Parameters
+        ----------
+        output
+        target
+        log_vars
+            sigma in uncertainty weighting;
+            default is None, meaning we manually set weights for different target's loss;
+            more info could be seen in
+            https://libmtl.readthedocs.io/en/latest/docs/_autoapi/LibMTL/weighting/index.html#LibMTL.weighting.UW
+
+        Returns
+        -------
+        torch.Tensor
+            multi-task loss by uncertainty weighting method
+        """
+        n_out = target.shape[-1]
+        loss = 0
+        for k in range(n_out):
+            precision = torch.exp(-log_vars[k])
+            if self.limit_part is not None and k in self.limit_part:
+                continue
+            p0 = output[:, :, k]
+            t0 = target[:, :, k]
+            mask = t0 == t0
+            p = p0[mask]
+            t = t0[mask]
+            if self.data_gap[k] > 0:
+                p, t = deal_gap_data(p0, t0, self.data_gap[k], self.device)
+            if type(self.loss_funcs) is list:
+                temp = self.loss_funcs[k](p, t)
+            else:
+                temp = self.loss_funcs(p, t)
+            loss += torch.sum(precision * temp + log_vars[k], -1)
+        return loss
+
+
+# ref: https://openaccess.thecvf.com/content_ECCV_2018/html/Michelle_Guo_Focus_on_the_ECCV_2018_paper.html
+class DynamicTaskPrior(torch.nn.Module):
+    r"""Dynamic Task Prioritization
+
+    This method is proposed in https://openaccess.thecvf.com/content_ECCV_2018/html/Michelle_Guo_Focus_on_the_ECCV_2018_paper.html
+    In contrast to UW and other curriculum learning methods, where easy tasks are prioritized above difficult tasks,
+    It shows the importance of prioritizing difficult tasks first.
+    It automatically prioritize more difficult tasks by adaptively adjusting the mixing weight of each task’s loss.
+    Here we choose correlation as KPI. As KPI must be in [0,1], we set (corr+1)/2 as KPI
+    """
+
+    def __init__(
+        self,
+        loss_funcs: Union[torch.nn.Module, list],
+        data_gap: list = None,
+        device: list = None,
+        limit_part: list = None,
+        gamma=2,
+        alpha=0.5,
+    ):
+        """
+
+        Parameters
+        ----------
+        loss_funcs
+        data_gap
+        device
+        limit_part
+        gamma
+            the example-level focusing parameter
+        alpha
+            default is 1, which means we only use the newest KPI value
+        """
+        if data_gap is None:
+            data_gap = [0, 2]
+        if device is None:
+            device = [0]
+        super(DynamicTaskPrior, self).__init__()
+        self.loss_funcs = loss_funcs
+        self.data_gap = data_gap
+        self.device = get_the_device(device)
+        self.limit_part = limit_part
+        self.gamma = gamma
+        self.alpha = alpha
+
+    def forward(self, output, target, kpi_last=None):
+        """
+        Parameters
+        ----------
+        output
+            model's prediction
+        target
+            observation
+
+        kpi_last
+            the KPI value of last iteration; each element for an output
+            It use a moving average KPI as the weighting coefficient: KPI_i = alpha * KPI_i + (1-alpha) * KPI_{i-1}
+
+        Returns
+        -------
+        torch.Tensor
+            multi-task loss by Dynamic Task Prioritization method
+        """
+        n_out = target.shape[-1]
+        loss = 0
+        kpis = torch.zeros(n_out).to(self.device)
+        for k in range(n_out):
+            if self.limit_part is not None and k in self.limit_part:
+                continue
+            p0 = output[:, :, k]
+            t0 = target[:, :, k]
+            mask = t0 == t0
+            p = p0[mask]
+            t = t0[mask]
+            if self.data_gap[k] > 0:
+                p, t = deal_gap_data(p0, t0, self.data_gap[k], self.device)
+            if type(self.loss_funcs) is list:
+                temp = self.loss_funcs[k](p, t)
+            else:
+                temp = self.loss_funcs(p, t)
+            # kpi must be in [0, 1], as corr's range is [-1, 1], just trans corr to  (corr+1)/2
+            kpi = (torch.corrcoef(torch.stack([p, t], 1).T)[0, 1] + 1) / 2
+            if self.alpha < 1:
+                assert kpi_last is not None
+                kpi = kpi * self.alpha + kpi_last[k] * (1 - self.alpha)
+                # if we exclude kpi from the backward, it trans to a normal multi-task model
+                # kpi = kpi.detach().clone() * self.alpha + kpi_last[k] * (1 - self.alpha)
+            kpis[k] = kpi
+            # focal loss
+            fl = -((1 - kpi) ** self.gamma) * torch.log(kpi)
+            loss += torch.sum(fl * temp, -1)
+        # if kpi has grad_fn, backward will repeat. It won't work
+        return loss, kpis.detach().clone()
+
+
+class MultiOutWaterBalanceLoss(torch.nn.Module):
+    def __init__(
+        self,
+        loss_funcs: Union[torch.nn.Module, list],
+        data_gap: list = None,
+        device: list = None,
+        limit_part: list = None,
+        item_weight: list = None,
+        alpha=0.5,
+        beta=0.0,
+        wb_loss_func=None,
+        means=None,
+        stds=None,
+    ):
+        """
+        Loss function for multiple output considering water balance
+
+        loss = alpha * water_balance_loss + (1-alpha) * mtl_loss
+
+        This loss function is only for p, q, et now
+        we use the difference between p_obs_mean-q_obs_mean-et_obs_mean and p_pred_mean-q_pred_mean-et_pred_mean as water balance loss
+        which is the difference between (q_obs_mean + et_obs_mean) and (q_pred_mean + et_pred_mean)
+
+        Parameters
+        ----------
+        loss_funcs
+            The loss functions for each output
+        data_gap
+            It belongs to the feature dim.
+            If 1, then the corresponding value is uniformly-spaced with NaN values filling the gap;
+            in addition, the first non-nan value means the aggregated value of the following interval,
+            for example, in [5, nan, nan, nan], 5 means all four data's sum, although the next 3 values are nan
+            hence the calculation is a little different;
+            if 2, the first non-nan value means the average value of the following interval,
+            for example, in [5, nan, nan, nan], 5 means all four data's mean value;
+            default is [0, 2]
+        device
+            the number of device: -1 -> "cpu" or "cuda:x" (x is 0, 1 or ...)
+        limit_part
+            when transfer learning, we may ignore some part;
+            the default is None, which means no ignorance;
+            other choices are list, such as [0], [0, 1] or [1,2,..];
+            0 means the first variable;
+            tensor is [seq, time, var] or [time, seq, var]
+        item_weight
+            use different weight for each item's loss;
+            for example, the default values [0.5, 0.5] means 0.5 * loss1 + 0.5 * loss2
+        alpha
+            the weight of the water-balance item's loss
+        beta
+            the weight of real water-balance item's loss, et_mean/p_mean + q_mean/p_mean = 1 can be a loss.
+            It is not strictly correct as training batch only have about one year data, but still could be a constraint
+        wb_loss_func
+            the loss function for water balance item, by default it is None, which means we use function in loss_funcs
+        """
+        if data_gap is None:
+            data_gap = [0, 2]
+        if device is None:
+            device = [0]
+        if item_weight is None:
+            item_weight = [0.5, 0.5]
+        super(MultiOutWaterBalanceLoss, self).__init__()
+        self.loss_funcs = loss_funcs
+        self.data_gap = data_gap
+        self.device = get_the_device(device)
+        self.limit_part = limit_part
+        self.item_weight = item_weight
+        self.alpha = alpha
+        self.beta = beta
+        self.wb_loss_func = wb_loss_func
+        self.means = means
+        self.stds = stds
+
+    def forward(self, output: Tensor, target: Tensor):
+        """
+        Calculate the sum of losses for different variables and water-balance loss
+
+        When there are NaN values in observation, we will perform a "reduce" operation on prediction.
+        For example, pred = [0,1,2,3,4], obs=[5, nan, nan, 6, nan]; the "reduce" is sum;
+        then, pred_sum = [0+1+2, 3+4], obs_sum=[5,6], loss = loss_func(pred_sum, obs_sum).
+        Notice: when "sum", actually final index is not chosen,
+        because the whole observation may be [5, nan, nan, 6, nan, nan, 7, nan, nan], 6 means sum of three elements.
+        Just as the rho is 5, the final one is not chosen
+
+
+        Parameters
+        ----------
+        output
+            the prediction tensor; 3-dims are time sequence, batch and feature, respectively
+        target
+            the observation tensor
+
+        Returns
+        -------
+        Tensor
+            Whole loss
+        """
+        n_out = target.shape[-1]
+        loss = 0
+        p_means = []
+        t_means = []
+        all_means = self.means
+        all_stds = self.stds
+        for k in range(n_out):
+            if self.limit_part is not None and k in self.limit_part:
+                continue
+            p0 = output[:, :, k]
+            t0 = target[:, :, k]
+            # for water balance loss
+            if all_means is not None:
+                # denormalize for q and et
+                p1 = p0 * all_stds[k] + all_means[k]
+                t1 = t0 * all_stds[k] + all_means[k]
+                p2 = (10**p1 - 0.1) ** 2
+                t2 = (10**t1 - 0.1) ** 2
+                p_mean = torch.nanmean(p2, dim=0)
+                t_mean = torch.nanmean(t2, dim=0)
+            else:
+                p_mean = torch.nanmean(p0, dim=0)
+                t_mean = torch.nanmean(t0, dim=0)
+            p_means.append(p_mean)
+            t_means.append(t_mean)
+            # for mtl normal loss
+            mask = t0 == t0
+            p = p0[mask]
+            t = t0[mask]
+            if self.data_gap[k] > 0:
+                p, t = deal_gap_data(p0, t0, self.data_gap[k], self.device)
+            if type(self.loss_funcs) is list:
+                temp = self.item_weight[k] * self.loss_funcs[k](p, t)
+            else:
+                temp = self.item_weight[k] * self.loss_funcs(p, t)
+            # sum of all k-th loss
+            loss = loss + temp
+        # water balance loss
+        p_mean_q_plus_et = torch.sum(torch.stack(p_means), dim=0)
+        t_mean_q_plus_et = torch.sum(torch.stack(t_means), dim=0)
+        wb_ones = torch.ones_like(t_mean_q_plus_et)
+        if self.wb_loss_func is None:
+            if type(self.loss_funcs) is list:
+                # if wb_loss_func is None, we use the first loss function in loss_funcs
+                wb_loss = self.loss_funcs[0](p_mean_q_plus_et, t_mean_q_plus_et)
+                wb_1loss = self.loss_funcs[0](p_mean_q_plus_et, wb_ones)
+            else:
+                wb_loss = self.loss_funcs(p_mean_q_plus_et, t_mean_q_plus_et)
+                wb_1loss = self.loss_funcs(p_mean_q_plus_et, wb_ones)
+        else:
+            wb_loss = self.wb_loss_func(p_mean_q_plus_et, t_mean_q_plus_et)
+            wb_1loss = self.wb_loss_func(p_mean_q_plus_et, wb_ones)
+        return (
+            self.alpha * wb_loss
+            + (1 - self.alpha - self.beta) * loss
+            + self.beta * wb_1loss
+        )
```

### Comparing `torchhydro-0.0.4/torchhydro/models/cudnnlstm.py` & `torchhydro-0.0.5/torchhydro/models/cudnnlstm.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,547 +1,589 @@
-"""
-Author: MHPI group, Wenyu Ouyang
-Date: 2021-12-31 11:08:29
-LastEditTime: 2023-10-11 11:38:48
-LastEditors: Wenyu Ouyang
-Description: LSTM with dropout implemented by Kuai Fang and more LSTMs using it
-FilePath: /torchhydro/torchhydro/models/cudnnlstm.py
-Copyright (c) 2021-2022 MHPI group, Wenyu Ouyang. All rights reserved.
-"""
-
-import math
-from typing import Union
-
-import torch
-import torch.nn as nn
-from torch.nn import Parameter
-import torch.nn.functional as F
-
-from torchhydro.models.ann import SimpleAnn
-from torchhydro.models.dropout import DropMask, create_mask
-
-
-class LstmCellTied(nn.Module):
-    """
-    LSTM with dropout implemented by Kuai Fang: https://github.com/mhpi/hydroDL/blob/release/hydroDL/model/rnn.py
-
-    the name of "Tied" comes from this paper:
-    http://papers.nips.cc/paper/6241-a-theoretically-grounded-application-of-dropout-in-recurrent-neural-networks.pdf
-    which means the weights of all gates will be tied together to be used (eq. 6 in this paper).
-    this code is mainly used as a CPU version of CudnnLstm
-    """
-
-    def __init__(
-        self,
-        *,
-        input_size,
-        hidden_size,
-        mode="train",
-        dr=0.5,
-        dr_method="drX+drW+drC",
-        gpu=1
-    ):
-        super(LstmCellTied, self).__init__()
-
-        self.inputSize = input_size
-        self.hiddenSize = hidden_size
-        self.dr = dr
-
-        self.w_ih = Parameter(torch.Tensor(hidden_size * 4, input_size))
-        self.w_hh = Parameter(torch.Tensor(hidden_size * 4, hidden_size))
-        self.b_ih = Parameter(torch.Tensor(hidden_size * 4))
-        self.b_hh = Parameter(torch.Tensor(hidden_size * 4))
-
-        self.drMethod = dr_method.split("+")
-        self.gpu = gpu
-        self.mode = mode
-        if mode == "train":
-            self.train(mode=True)
-        elif mode in ["test", "drMC"]:
-            self.train(mode=False)
-        if gpu >= 0:
-            self = self.cuda()
-            self.is_cuda = True
-        else:
-            self.is_cuda = False
-        self.reset_parameters()
-
-    def reset_parameters(self):
-        stdv = 1.0 / math.sqrt(self.hiddenSize)
-        for weight in self.parameters():
-            weight.data.uniform_(-stdv, stdv)
-
-    def reset_mask(self, x, h, c):
-        self.mask_x = create_mask(x, self.dr)
-        self.mask_h = create_mask(h, self.dr)
-        self.mask_c = create_mask(c, self.dr)
-        self.mask_w_ih = create_mask(self.w_ih, self.dr)
-        self.mask_w_hh = create_mask(self.w_hh, self.dr)
-
-    def forward(self, x, hidden, *, do_reset_mask=True, do_drop_mc=False):
-        do_drop = self.dr > 0 and (do_drop_mc is True or self.training is True)
-        batch_size = x.size(0)
-        h0, c0 = hidden
-        if h0 is None:
-            h0 = x.new_zeros(batch_size, self.hiddenSize, requires_grad=False)
-        if c0 is None:
-            c0 = x.new_zeros(batch_size, self.hiddenSize, requires_grad=False)
-
-        if self.dr > 0 and self.training is True and do_reset_mask is True:
-            self.reset_mask(x, h0, c0)
-
-        if do_drop and "drH" in self.drMethod:
-            h0 = DropMask.apply(h0, self.mask_h, True)
-
-        if do_drop and "drX" in self.drMethod:
-            x = DropMask.apply(x, self.mask_x, True)
-
-        if do_drop and "drW" in self.drMethod:
-            w_ih = DropMask.apply(self.w_ih, self.mask_w_ih, True)
-            w_hh = DropMask.apply(self.w_hh, self.mask_w_hh, True)
-        else:
-            # self.w are parameters, while w are not
-            w_ih = self.w_ih
-            w_hh = self.w_hh
-
-        gates = F.linear(x, w_ih, self.b_ih) + F.linear(h0, w_hh, self.b_hh)
-        gate_i, gate_f, gate_c, gate_o = gates.chunk(4, 1)
-
-        gate_i = torch.sigmoid(gate_i)
-        gate_f = torch.sigmoid(gate_f)
-        gate_c = torch.tanh(gate_c)
-        gate_o = torch.sigmoid(gate_o)
-
-        if self.training is True and "drC" in self.drMethod:
-            gate_c = gate_c.mul(self.mask_c)
-
-        c1 = (gate_f * c0) + (gate_i * gate_c)
-        h1 = gate_o * torch.tanh(c1)
-
-        return h1, c1
-
-
-class CpuLstmModel(nn.Module):
-    """Cpu version of CudnnLstmModel"""
-
-    def __init__(self, *, n_input_features, n_output_features, n_hidden_states, dr=0.5):
-        super(CpuLstmModel, self).__init__()
-        self.nx = n_input_features
-        self.ny = n_output_features
-        self.hiddenSize = n_hidden_states
-        self.ct = 0
-        self.nLayer = 1
-        self.linearIn = torch.nn.Linear(n_input_features, n_hidden_states)
-        self.lstm = LstmCellTied(
-            input_size=n_hidden_states,
-            hidden_size=n_hidden_states,
-            dr=dr,
-            dr_method="drW",
-            gpu=-1,
-        )
-        self.linearOut = torch.nn.Linear(n_hidden_states, n_output_features)
-        self.gpu = -1
-
-    def forward(self, x, do_drop_mc=False):
-        # x0 = F.relu(self.linearIn(x))
-        # outLSTM, (hn, cn) = self.lstm(x0, do_drop_mc=do_drop_mc)
-        # out = self.linearOut(outLSTM)
-        # return out
-        nt, ngrid, nx = x.shape
-        yt = torch.zeros(ngrid, 1)
-        out = torch.zeros(nt, ngrid, self.ny)
-        ht = None
-        ct = None
-        reset_mask = True
-        for t in range(nt):
-            xt = x[t, :, :]
-            x0 = F.relu(self.linearIn(xt))
-            ht, ct = self.lstm(x0, hidden=(ht, ct), do_reset_mask=reset_mask)
-            yt = self.linearOut(ht)
-            reset_mask = False
-            out[t, :, :] = yt
-        return out
-
-
-class CudnnLstm(nn.Module):
-    """
-    LSTM with dropout implemented by Kuai Fang: https://github.com/mhpi/hydroDL/blob/release/hydroDL/model/rnn.py
-
-    Only run in GPU; the CPU version is LstmCellTied in this file
-    """
-
-    def __init__(self, *, input_size, hidden_size, dr=0.5):
-        """
-
-        Parameters
-        ----------
-        input_size
-            number of neurons in input layer
-        hidden_size
-            number of neurons in hidden layer
-        dr
-            dropout rate
-        """
-        super(CudnnLstm, self).__init__()
-        self.input_size = input_size
-        self.hidden_size = hidden_size
-        self.dr = dr
-        self.w_ih = Parameter(torch.Tensor(hidden_size * 4, input_size))
-        self.w_hh = Parameter(torch.Tensor(hidden_size * 4, hidden_size))
-        self.b_ih = Parameter(torch.Tensor(hidden_size * 4))
-        self.b_hh = Parameter(torch.Tensor(hidden_size * 4))
-        self._all_weights = [["w_ih", "w_hh", "b_ih", "b_hh"]]
-        # self.cuda()
-
-        self.reset_mask()
-        self.reset_parameters()
-
-    def _apply(self, fn):
-        return super()._apply(fn)
-
-    def __setstate__(self, d):  # this func will be called when loading the model
-        super().__setstate__(d)
-        self.__dict__.setdefault("_data_ptrs", [])
-        if "all_weights" in d:
-            self._all_weights = d["all_weights"]
-        if isinstance(self._all_weights[0][0], str):
-            return
-        self._all_weights = [["w_ih", "w_hh", "b_ih", "b_hh"]]
-
-    def reset_mask(self):
-        self.mask_w_ih = create_mask(self.w_ih, self.dr)
-        self.mask_w_hh = create_mask(self.w_hh, self.dr)
-
-    def reset_parameters(self):
-        stdv = 1.0 / math.sqrt(self.hidden_size)
-        for weight in self.parameters():
-            weight.data.uniform_(-stdv, stdv)
-
-    def forward(self, input, hx=None, cx=None, do_drop_mc=False, dropout_false=False):
-        # dropout_false: it will ensure do_drop is false, unless do_drop_mc is true
-        if dropout_false and (not do_drop_mc):
-            do_drop = False
-        elif self.dr > 0 and (do_drop_mc is True or self.training is True):
-            do_drop = True
-        else:
-            do_drop = False
-
-        batch_size = input.size(1)
-
-        if hx is None:
-            hx = input.new_zeros(1, batch_size, self.hidden_size, requires_grad=False)
-        if cx is None:
-            cx = input.new_zeros(1, batch_size, self.hidden_size, requires_grad=False)
-
-        # handle = torch.backends.cudnn.get_handle()
-        if do_drop is True:
-            # cuDNN backend - disabled flat weight
-            freeze_mask = False
-            if not freeze_mask:
-                self.reset_mask()
-            weight = [
-                DropMask.apply(self.w_ih, self.mask_w_ih, True),
-                DropMask.apply(self.w_hh, self.mask_w_hh, True),
-                self.b_ih,
-                self.b_hh,
-            ]
-        else:
-            weight = [self.w_ih, self.w_hh, self.b_ih, self.b_hh]
-        if torch.__version__ < "1.8":
-            output, hy, cy, reserve, new_weight_buf = torch._cudnn_rnn(
-                input,
-                weight,
-                4,
-                None,
-                hx,
-                cx,
-                2,  # 2 means LSTM
-                self.hidden_size,
-                1,
-                False,
-                0,
-                self.training,
-                False,
-                (),
-                None,
-            )
-        else:
-            output, hy, cy, reserve, new_weight_buf = torch._cudnn_rnn(
-                input,
-                weight,
-                4,
-                None,
-                hx,
-                cx,
-                2,  # 2 means LSTM
-                self.hidden_size,
-                0,
-                1,
-                False,
-                0,
-                self.training,
-                False,
-                (),
-                None,
-            )
-        return output, (hy, cy)
-
-    @property
-    def all_weights(self):
-        return [
-            [getattr(self, weight) for weight in weights]
-            for weights in self._all_weights
-        ]
-
-
-class CudnnLstmModel(nn.Module):
-    def __init__(self, n_input_features, n_output_features, n_hidden_states, dr=0.5):
-        """
-        An LSTM model writen by Kuai Fang from this paper: https://doi.org/10.1002/2017GL075619
-
-        only gpu version
-
-        Parameters
-        ----------
-        n_input_features
-            the number of input features
-        n_output_features
-            the number of output features
-        n_hidden_states
-            the number of hidden features
-        dr
-            dropout rate and its default is 0.5
-        """
-        super(CudnnLstmModel, self).__init__()
-        self.nx = n_input_features
-        self.ny = n_output_features
-        self.hidden_size = n_hidden_states
-        self.ct = 0
-        self.nLayer = 1
-        self.linearIn = torch.nn.Linear(self.nx, self.hidden_size)
-        self.lstm = CudnnLstm(
-            input_size=self.hidden_size, hidden_size=self.hidden_size, dr=dr
-        )
-        self.linearOut = torch.nn.Linear(self.hidden_size, self.ny)
-
-    def forward(self, x, do_drop_mc=False, dropout_false=False, return_h_c=False):
-        x0 = F.relu(self.linearIn(x))
-        out_lstm, (hn, cn) = self.lstm(
-            x0, do_drop_mc=do_drop_mc, dropout_false=dropout_false
-        )
-        out = self.linearOut(out_lstm)
-        return (out, (hn, cn)) if return_h_c else out
-
-
-class LinearCudnnLstmModel(CudnnLstmModel):
-    """This model is nonlinear layer + CudnnLSTM/CudnnLstm-MultiOutput-Model.
-    kai_tl: model from this paper by Ma et al. -- https://doi.org/10.1029/2020WR028600
-    """
-
-    def __init__(self, linear_size, **kwargs):
-        """
-
-        Parameters
-        ----------
-        linear_size
-            the number of input features for the first input linear layer
-        """
-        super(LinearCudnnLstmModel, self).__init__(**kwargs)
-        self.former_linear = torch.nn.Linear(linear_size, kwargs["n_input_features"])
-
-    def forward(self, x, do_drop_mc=False, dropout_false=False):
-        x0 = F.relu(self.former_linear(x))
-        return super(LinearCudnnLstmModel, self).forward(
-            x0, do_drop_mc=do_drop_mc, dropout_false=dropout_false
-        )
-
-
-class CNN1dLCmodel(nn.Module):
-    # Directly add the CNN extracted features into LSTM inputSize
-    def __init__(
-        self,
-        nx,
-        ny,
-        nobs,
-        hidden_size,
-        n_kernel: Union[list, tuple] = (10, 5),
-        kernel_size: Union[list, tuple] = (3, 3),
-        stride: Union[list, tuple] = (2, 1),
-        dr=0.5,
-        pool_opt=None,
-        cnn_dr=0.5,
-        cat_first=True,
-    ):
-        """cat_first means: we will concatenate the CNN output with the x, then input them to the CudnnLstm model;
-        if not cat_first, it is relu_first, meaning we will relu the CNN output firstly, then concatenate it with x
-        """
-        # two convolutional layer
-        super(CNN1dLCmodel, self).__init__()
-        self.nx = nx
-        self.ny = ny
-        self.obs = nobs
-        self.hiddenSize = hidden_size
-        n_layer = len(n_kernel)
-        self.features = nn.Sequential()
-        n_in_chan = 1
-        lout = nobs
-        for ii in range(n_layer):
-            conv_layer = CNN1dKernel(
-                n_in_channel=n_in_chan,
-                n_kernel=n_kernel[ii],
-                kernel_size=kernel_size[ii],
-                stride=stride[ii],
-            )
-            self.features.add_module("CnnLayer%d" % (ii + 1), conv_layer)
-            if cnn_dr != 0.0:
-                self.features.add_module("dropout%d" % (ii + 1), nn.Dropout(p=cnn_dr))
-            n_in_chan = n_kernel[ii]
-            lout = cal_conv_size(lin=lout, kernel=kernel_size[ii], stride=stride[ii])
-            self.features.add_module("Relu%d" % (ii + 1), nn.ReLU())
-            if pool_opt is not None:
-                self.features.add_module(
-                    "Pooling%d" % (ii + 1), nn.MaxPool1d(pool_opt[ii])
-                )
-                lout = cal_pool_size(lin=lout, kernel=pool_opt[ii])
-        self.N_cnn_out = int(
-            lout * n_kernel[-1]
-        )  # total CNN feature number after convolution
-        self.cat_first = cat_first
-        if cat_first:
-            nf = self.N_cnn_out + nx
-            self.linearIn = torch.nn.Linear(nf, hidden_size)
-            self.lstm = CudnnLstm(
-                input_size=hidden_size, hidden_size=hidden_size, dr=dr
-            )
-        else:
-            nf = self.N_cnn_out + hidden_size
-            self.linearIn = torch.nn.Linear(nx, hidden_size)
-            self.lstm = CudnnLstm(input_size=nf, hidden_size=hidden_size, dr=dr)
-        self.linearOut = torch.nn.Linear(hidden_size, ny)
-        self.gpu = 1
-
-    def forward(self, x, z, do_drop_mc=False):
-        # z = n_grid*nVar add a channel dimension
-        z = z.t()
-        n_grid, nobs = z.shape
-        rho, bs, n_var = x.shape
-        # add a channel dimension
-        z = torch.unsqueeze(z, dim=1)
-        z0 = self.features(z)
-        # z0 = (n_grid) * n_kernel * sizeafterconv
-        z0 = z0.view(n_grid, self.N_cnn_out).repeat(rho, 1, 1)
-        if self.cat_first:
-            x = torch.cat((x, z0), dim=2)
-            x0 = F.relu(self.linearIn(x))
-        else:
-            x = F.relu(self.linearIn(x))
-            x0 = torch.cat((x, z0), dim=2)
-        out_lstm, (hn, cn) = self.lstm(x0, do_drop_mc=do_drop_mc)
-        return self.linearOut(out_lstm)
-
-
-class CudnnLstmModelLstmKernel(nn.Module):
-    """use a trained/un-trained CudnnLstm as a kernel generator before another CudnnLstm."""
-
-    def __init__(
-        self,
-        nx,
-        ny,
-        hidden_size,
-        nk=None,
-        hidden_size_later=None,
-        cut=False,
-        dr=0.5,
-        delta_s=False,
-    ):
-        """delta_s means we will use the difference of the first lstm's output and the second's as the final output"""
-        super(CudnnLstmModelLstmKernel, self).__init__()
-        # These three layers are same with CudnnLstmModel to be used for transfer learning or just vanilla-use
-        self.linearIn = torch.nn.Linear(nx, hidden_size)
-        self.lstm = CudnnLstm(input_size=hidden_size, hidden_size=hidden_size, dr=dr)
-        self.linearOut = torch.nn.Linear(hidden_size, ny)
-        # if cut is True, we will only select the final index in nk, and repeat it, then concatenate with x
-        self.cut = cut
-        # the second lstm has more input than the previous
-        if nk is None:
-            nk = ny
-        if hidden_size_later is None:
-            hidden_size_later = hidden_size
-        self.linear_in_later = torch.nn.Linear(nx + nk, hidden_size_later)
-        self.lstm_later = CudnnLstm(
-            input_size=hidden_size_later, hidden_size=hidden_size_later, dr=dr
-        )
-        self.linear_out_later = torch.nn.Linear(hidden_size_later, ny)
-
-        self.delta_s = delta_s
-        # when delta_s is true, cut cannot be true, because they have to have same number params
-        assert not (cut and delta_s)
-
-    def forward(self, x, do_drop_mc=False, dropout_false=False):
-        x0 = F.relu(self.linearIn(x))
-        out_lstm1, (hn1, cn1) = self.lstm(
-            x0, do_drop_mc=do_drop_mc, dropout_false=dropout_false
-        )
-        gen = self.linearOut(out_lstm1)
-        if self.cut:
-            gen = gen[-1, :, :].repeat(x.shape[0], 1, 1)
-        x1 = torch.cat((x, gen), dim=len(gen.shape) - 1)
-        x2 = F.relu(self.linear_in_later(x1))
-        out_lstm2, (hn2, cn2) = self.lstm_later(
-            x2, do_drop_mc=do_drop_mc, dropout_false=dropout_false
-        )
-        out = self.linear_out_later(out_lstm2)
-        return gen - out if self.delta_s else (out, gen)
-
-
-class CudnnLstmModelMultiOutput(nn.Module):
-    def __init__(
-        self,
-        n_input_features,
-        n_output_features,
-        n_hidden_states,
-        layer_hidden_size=(128, 64),
-        dr=0.5,
-        dr_hidden=0.0,
-    ):
-        """
-        Multiple output CudnnLSTM.
-
-        It has multiple output layers, each for one output, so that we can easily freeze any output layer.
-
-        Parameters
-        ----------
-        n_input_features
-            the size of input features
-        n_output_features
-            the size of output features; in this model, we set different nonlinear layer for each output
-        n_hidden_states
-            the size of LSTM's hidden features
-        layer_hidden_size
-            hidden_size for multi-layers
-        dr
-            dropout rate
-        dr_hidden
-            dropout rates of hidden layers
-        """
-        super(CudnnLstmModelMultiOutput, self).__init__()
-        self.ct = 0
-        multi_layers = torch.nn.ModuleList()
-        for i in range(n_output_features):
-            multi_layers.add_module(
-                "layer%d" % (i + 1),
-                SimpleAnn(n_hidden_states, 1, layer_hidden_size, dr=dr_hidden),
-            )
-        self.multi_layers = multi_layers
-        self.linearIn = torch.nn.Linear(n_input_features, n_hidden_states)
-        self.lstm = CudnnLstm(
-            input_size=n_hidden_states, hidden_size=n_hidden_states, dr=dr
-        )
-
-    def forward(self, x, do_drop_mc=False, dropout_false=False, return_h_c=False):
-        x0 = F.relu(self.linearIn(x))
-        out_lstm, (hn, cn) = self.lstm(
-            x0, do_drop_mc=do_drop_mc, dropout_false=dropout_false
-        )
-        outs = [mod(out_lstm) for mod in self.multi_layers]
-        final = torch.cat(outs, dim=-1)
-        return (final, (hn, cn)) if return_h_c else final
+"""
+Author: MHPI group, Wenyu Ouyang
+Date: 2021-12-31 11:08:29
+LastEditTime: 2024-05-27 16:01:38
+LastEditors: Wenyu Ouyang
+Description: LSTM with dropout implemented by Kuai Fang and more LSTMs using it
+FilePath: \torchhydro\torchhydro\models\cudnnlstm.py
+Copyright (c) 2021-2022 MHPI group, Wenyu Ouyang. All rights reserved.
+"""
+
+import math
+from typing import Union
+
+import torch
+import torch.nn as nn
+from torch.nn import Parameter
+import torch.nn.functional as F
+
+from torchhydro.models.ann import SimpleAnn
+from torchhydro.models.dropout import DropMask, create_mask
+
+
+class LstmCellTied(nn.Module):
+    """
+    LSTM with dropout implemented by Kuai Fang: https://github.com/mhpi/hydroDL/blob/release/hydroDL/model/rnn.py
+
+    the name of "Tied" comes from this paper:
+    http://papers.nips.cc/paper/6241-a-theoretically-grounded-application-of-dropout-in-recurrent-neural-networks.pdf
+    which means the weights of all gates will be tied together to be used (eq. 6 in this paper).
+    this code is mainly used as a CPU version of CudnnLstm
+    """
+
+    def __init__(
+        self,
+        *,
+        input_size,
+        hidden_size,
+        mode="train",
+        dr=0.5,
+        dr_method="drX+drW+drC",
+        gpu=1
+    ):
+        super(LstmCellTied, self).__init__()
+
+        self.inputSize = input_size
+        self.hiddenSize = hidden_size
+        self.dr = dr
+
+        self.w_ih = Parameter(torch.Tensor(hidden_size * 4, input_size))
+        self.w_hh = Parameter(torch.Tensor(hidden_size * 4, hidden_size))
+        self.b_ih = Parameter(torch.Tensor(hidden_size * 4))
+        self.b_hh = Parameter(torch.Tensor(hidden_size * 4))
+
+        self.drMethod = dr_method.split("+")
+        self.gpu = gpu
+        self.mode = mode
+        if mode == "train":
+            self.train(mode=True)
+        elif mode in ["test", "drMC"]:
+            self.train(mode=False)
+        if gpu >= 0:
+            self = self.cuda()
+            self.is_cuda = True
+        else:
+            self.is_cuda = False
+        self.reset_parameters()
+
+    def reset_parameters(self):
+        stdv = 1.0 / math.sqrt(self.hiddenSize)
+        for weight in self.parameters():
+            weight.data.uniform_(-stdv, stdv)
+
+    def reset_mask(self, x, h, c):
+        self.mask_x = create_mask(x, self.dr)
+        self.mask_h = create_mask(h, self.dr)
+        self.mask_c = create_mask(c, self.dr)
+        self.mask_w_ih = create_mask(self.w_ih, self.dr)
+        self.mask_w_hh = create_mask(self.w_hh, self.dr)
+
+    def forward(self, x, hidden, *, do_reset_mask=True, do_drop_mc=False):
+        do_drop = self.dr > 0 and (do_drop_mc is True or self.training is True)
+        batch_size = x.size(0)
+        h0, c0 = hidden
+        if h0 is None:
+            h0 = x.new_zeros(batch_size, self.hiddenSize, requires_grad=False)
+        if c0 is None:
+            c0 = x.new_zeros(batch_size, self.hiddenSize, requires_grad=False)
+
+        if self.dr > 0 and self.training is True and do_reset_mask is True:
+            self.reset_mask(x, h0, c0)
+
+        if do_drop and "drH" in self.drMethod:
+            h0 = DropMask.apply(h0, self.mask_h, True)
+
+        if do_drop and "drX" in self.drMethod:
+            x = DropMask.apply(x, self.mask_x, True)
+
+        if do_drop and "drW" in self.drMethod:
+            w_ih = DropMask.apply(self.w_ih, self.mask_w_ih, True)
+            w_hh = DropMask.apply(self.w_hh, self.mask_w_hh, True)
+        else:
+            # self.w are parameters, while w are not
+            w_ih = self.w_ih
+            w_hh = self.w_hh
+
+        gates = F.linear(x, w_ih, self.b_ih) + F.linear(h0, w_hh, self.b_hh)
+        gate_i, gate_f, gate_c, gate_o = gates.chunk(4, 1)
+
+        gate_i = torch.sigmoid(gate_i)
+        gate_f = torch.sigmoid(gate_f)
+        gate_c = torch.tanh(gate_c)
+        gate_o = torch.sigmoid(gate_o)
+
+        if self.training is True and "drC" in self.drMethod:
+            gate_c = gate_c.mul(self.mask_c)
+
+        c1 = (gate_f * c0) + (gate_i * gate_c)
+        h1 = gate_o * torch.tanh(c1)
+
+        return h1, c1
+
+
+class CpuLstmModel(nn.Module):
+    """Cpu version of CudnnLstmModel"""
+
+    def __init__(self, *, n_input_features, n_output_features, n_hidden_states, dr=0.5):
+        super(CpuLstmModel, self).__init__()
+        self.nx = n_input_features
+        self.ny = n_output_features
+        self.hiddenSize = n_hidden_states
+        self.ct = 0
+        self.nLayer = 1
+        self.linearIn = torch.nn.Linear(n_input_features, n_hidden_states)
+        self.lstm = LstmCellTied(
+            input_size=n_hidden_states,
+            hidden_size=n_hidden_states,
+            dr=dr,
+            dr_method="drW",
+            gpu=-1,
+        )
+        self.linearOut = torch.nn.Linear(n_hidden_states, n_output_features)
+        self.gpu = -1
+
+    def forward(self, x, do_drop_mc=False):
+        # x0 = F.relu(self.linearIn(x))
+        # outLSTM, (hn, cn) = self.lstm(x0, do_drop_mc=do_drop_mc)
+        # out = self.linearOut(outLSTM)
+        # return out
+        nt, ngrid, nx = x.shape
+        yt = torch.zeros(ngrid, 1)
+        out = torch.zeros(nt, ngrid, self.ny)
+        ht = None
+        ct = None
+        reset_mask = True
+        for t in range(nt):
+            xt = x[t, :, :]
+            xt = torch.where(torch.isnan(xt), torch.full_like(xt, 0), xt)
+            x0 = F.relu(self.linearIn(xt))
+            ht, ct = self.lstm(x0, hidden=(ht, ct), do_reset_mask=reset_mask)
+            yt = self.linearOut(ht)
+            reset_mask = False
+            out[t, :, :] = yt
+        return out
+
+
+class CudnnLstm(nn.Module):
+    """
+    LSTM with dropout implemented by Kuai Fang: https://github.com/mhpi/hydroDL/blob/release/hydroDL/model/rnn.py
+
+    Only run in GPU; the CPU version is LstmCellTied in this file
+    """
+
+    def __init__(self, *, input_size, hidden_size, dr=0.5):
+        """
+
+        Parameters
+        ----------
+        input_size
+            number of neurons in input layer
+        hidden_size
+            number of neurons in hidden layer
+        dr
+            dropout rate
+        """
+        super(CudnnLstm, self).__init__()
+        self.input_size = input_size
+        self.hidden_size = hidden_size
+        self.dr = dr
+        self.w_ih = Parameter(torch.Tensor(hidden_size * 4, input_size))
+        self.w_hh = Parameter(torch.Tensor(hidden_size * 4, hidden_size))
+        self.b_ih = Parameter(torch.Tensor(hidden_size * 4))
+        self.b_hh = Parameter(torch.Tensor(hidden_size * 4))
+        self._all_weights = [["w_ih", "w_hh", "b_ih", "b_hh"]]
+        # self.cuda()
+
+        self.reset_mask()
+        self.reset_parameters()
+
+    def _apply(self, fn):
+        return super()._apply(fn)
+
+    def __setstate__(self, d):  # this func will be called when loading the model
+        super().__setstate__(d)
+        self.__dict__.setdefault("_data_ptrs", [])
+        if "all_weights" in d:
+            self._all_weights = d["all_weights"]
+        if isinstance(self._all_weights[0][0], str):
+            return
+        self._all_weights = [["w_ih", "w_hh", "b_ih", "b_hh"]]
+
+    def reset_mask(self):
+        self.mask_w_ih = create_mask(self.w_ih, self.dr)
+        self.mask_w_hh = create_mask(self.w_hh, self.dr)
+
+    def reset_parameters(self):
+        stdv = 1.0 / math.sqrt(self.hidden_size)
+        for weight in self.parameters():
+            weight.data.uniform_(-stdv, stdv)
+
+    def forward(self, input, hx=None, cx=None, do_drop_mc=False, dropout_false=False):
+        # dropout_false: it will ensure do_drop is false, unless do_drop_mc is true
+        if dropout_false and (not do_drop_mc):
+            do_drop = False
+        elif self.dr > 0 and (do_drop_mc is True or self.training is True):
+            do_drop = True
+        else:
+            do_drop = False
+
+        batch_size = input.size(1)
+
+        if hx is None:
+            hx = input.new_zeros(1, batch_size, self.hidden_size, requires_grad=False)
+        if cx is None:
+            cx = input.new_zeros(1, batch_size, self.hidden_size, requires_grad=False)
+
+        # handle = torch.backends.cudnn.get_handle()
+        if do_drop is True:
+            # cuDNN backend - disabled flat weight
+            freeze_mask = False
+            if not freeze_mask:
+                self.reset_mask()
+            weight = [
+                DropMask.apply(self.w_ih, self.mask_w_ih, True),
+                DropMask.apply(self.w_hh, self.mask_w_hh, True),
+                self.b_ih,
+                self.b_hh,
+            ]
+        else:
+            weight = [self.w_ih, self.w_hh, self.b_ih, self.b_hh]
+        if torch.__version__ < "1.8":
+            output, hy, cy, reserve, new_weight_buf = torch._cudnn_rnn(
+                input,
+                weight,
+                4,
+                None,
+                hx,
+                cx,
+                2,  # 2 means LSTM
+                self.hidden_size,
+                1,
+                False,
+                0,
+                self.training,
+                False,
+                (),
+                None,
+            )
+        else:
+            output, hy, cy, reserve, new_weight_buf = torch._cudnn_rnn(
+                input,
+                weight,
+                4,
+                None,
+                hx,
+                cx,
+                2,  # 2 means LSTM
+                self.hidden_size,
+                0,
+                1,
+                False,
+                0,
+                self.training,
+                False,
+                (),
+                None,
+            )
+        return output, (hy, cy)
+
+    @property
+    def all_weights(self):
+        return [
+            [getattr(self, weight) for weight in weights]
+            for weights in self._all_weights
+        ]
+
+
+class CudnnLstmModel(nn.Module):
+    def __init__(self, n_input_features, n_output_features, n_hidden_states, dr=0.5):
+        """
+        An LSTM model writen by Kuai Fang from this paper: https://doi.org/10.1002/2017GL075619
+
+        only gpu version
+
+        Parameters
+        ----------
+        n_input_features
+            the number of input features
+        n_output_features
+            the number of output features
+        n_hidden_states
+            the number of hidden features
+        dr
+            dropout rate and its default is 0.5
+        """
+        super(CudnnLstmModel, self).__init__()
+        self.nx = n_input_features
+        self.ny = n_output_features
+        self.hidden_size = n_hidden_states
+        self.ct = 0
+        self.nLayer = 1
+        self.linearIn = torch.nn.Linear(self.nx, self.hidden_size)
+        self.lstm = CudnnLstm(
+            input_size=self.hidden_size, hidden_size=self.hidden_size, dr=dr
+        )
+        self.linearOut = torch.nn.Linear(self.hidden_size, self.ny)
+
+    def forward(self, x, do_drop_mc=False, dropout_false=False, return_h_c=False):
+        x0 = F.relu(self.linearIn(x))
+        out_lstm, (hn, cn) = self.lstm(
+            x0, do_drop_mc=do_drop_mc, dropout_false=dropout_false
+        )
+        out = self.linearOut(out_lstm)
+        return (out, (hn, cn)) if return_h_c else out
+
+
+class LinearCudnnLstmModel(CudnnLstmModel):
+    """This model is nonlinear layer + CudnnLSTM/CudnnLstm-MultiOutput-Model.
+    kai_tl: model from this paper by Ma et al. -- https://doi.org/10.1029/2020WR028600
+    """
+
+    def __init__(self, linear_size, **kwargs):
+        """
+
+        Parameters
+        ----------
+        linear_size
+            the number of input features for the first input linear layer
+        """
+        super(LinearCudnnLstmModel, self).__init__(**kwargs)
+        self.former_linear = torch.nn.Linear(linear_size, kwargs["n_input_features"])
+
+    def forward(self, x, do_drop_mc=False, dropout_false=False):
+        x0 = F.relu(self.former_linear(x))
+        return super(LinearCudnnLstmModel, self).forward(
+            x0, do_drop_mc=do_drop_mc, dropout_false=dropout_false
+        )
+
+
+def cal_conv_size(lin, kernel, stride, padding=0, dilation=1):
+    lout = (lin + 2 * padding - dilation * (kernel - 1) - 1) / stride + 1
+    return int(lout)
+
+
+def cal_pool_size(lin, kernel, stride=None, padding=0, dilation=1):
+    if stride is None:
+        stride = kernel
+    lout = (lin + 2 * padding - dilation * (kernel - 1) - 1) / stride + 1
+    return int(lout)
+
+
+class CNN1dKernel(torch.nn.Module):
+    def __init__(self, *, ninchannel=1, nkernel=3, kernelSize=3, stride=1, padding=0):
+        super(CNN1dKernel, self).__init__()
+        self.cnn1d = torch.nn.Conv1d(
+            in_channels=ninchannel,
+            out_channels=nkernel,
+            kernel_size=kernelSize,
+            padding=padding,
+            stride=stride,
+        )
+        self.name = "CNN1dkernel"
+        self.is_legacy = True
+
+    def forward(self, x):
+        return F.relu(self.cnn1d(x))
+
+
+class CNN1dLCmodel(nn.Module):
+    # Directly add the CNN extracted features into LSTM inputSize
+    def __init__(
+        self,
+        nx,
+        ny,
+        nobs,
+        hidden_size,
+        n_kernel: Union[list, tuple] = (10, 5),
+        kernel_size: Union[list, tuple] = (3, 3),
+        stride: Union[list, tuple] = (2, 1),
+        dr=0.5,
+        pool_opt=None,
+        cnn_dr=0.5,
+        cat_first=True,
+    ):
+        """cat_first means: we will concatenate the CNN output with the x, then input them to the CudnnLstm model;
+        if not cat_first, it is relu_first, meaning we will relu the CNN output firstly, then concatenate it with x
+        """
+        # two convolutional layer
+        super(CNN1dLCmodel, self).__init__()
+        # N_cnn_out代表输出的特征数量
+        # nx代表历史的输入
+        # ny代表最后线性层输出的维度，如果只预报流量，则为1
+        # nobs代表要输入到CNN的维度
+        # hidden_size是线性层的隐藏层的节点数
+        self.nx = nx
+        self.ny = ny
+        self.obs = nobs
+        self.hiddenSize = hidden_size
+        n_layer = len(n_kernel)
+        self.features = nn.Sequential()
+        n_in_chan = 1
+        lout = nobs
+        for ii in range(n_layer):
+            conv_layer = CNN1dKernel(
+                ninchannel=n_in_chan,
+                nkernel=n_kernel[ii],
+                kernelSize=kernel_size[ii],
+                stride=stride[ii],
+            )
+            self.features.add_module("CnnLayer%d" % (ii + 1), conv_layer)
+            if cnn_dr != 0.0:
+                self.features.add_module("dropout%d" % (ii + 1), nn.Dropout(p=cnn_dr))
+            n_in_chan = n_kernel[ii]
+            lout = cal_conv_size(lin=lout, kernel=kernel_size[ii], stride=stride[ii])
+            self.features.add_module("Relu%d" % (ii + 1), nn.ReLU())
+            if pool_opt is not None:
+                self.features.add_module(
+                    "Pooling%d" % (ii + 1), nn.MaxPool1d(pool_opt[ii])
+                )
+                lout = cal_pool_size(lin=lout, kernel=pool_opt[ii])
+        self.N_cnn_out = int(
+            lout * n_kernel[-1]
+        )  # total CNN feature number after convolution
+        self.cat_first = cat_first
+        # 要不要先拼接？
+        # 先拼接，则代表线性层中，输入的维度是未来的降水等输入输出的CNN特征维度，和历史观测的等时间序列的特征数量，通过线性层合并成一个，然后再把这些特征输出到一个线性层中
+        # 如果不拼接，那么历史观测数据先进入一个线性层
+        if cat_first:
+            nf = self.N_cnn_out + nx
+            self.linearIn = torch.nn.Linear(nf, hidden_size)
+            # CudnnLstm除了最基础的部分以外，主要是有个h和c两个门为空的纠错，这个在论文里讲述的是因为可能输入缺失，但是又不想用插值处理
+            # 不想用插值处理是因为认为会暴露未来信息
+            # 采用了置零操作，原文的表述是这种缺失点较少，在模型的不断更新参数后，这种置零的影响对于模型的输出影响很小
+            self.lstm = CudnnLstm(
+                input_size=hidden_size, hidden_size=hidden_size, dr=dr
+            )
+        else:
+            nf = self.N_cnn_out + hidden_size
+            self.linearIn = torch.nn.Linear(nx, hidden_size)
+            self.lstm = CudnnLstm(input_size=nf, hidden_size=hidden_size, dr=dr)
+        self.linearOut = torch.nn.Linear(hidden_size, ny)
+        self.gpu = 1
+
+    def forward(self, x, z, do_drop_mc=False):
+        # z = n_grid*nVar add a channel dimension
+        # z = z.t()
+        n_grid, nobs, _ = z.shape
+        z = z.reshape(n_grid * nobs, 1)
+        n_t, bs, n_var = x.shape
+        # add a channel dimension
+        z = torch.unsqueeze(z, dim=1)
+        z0 = self.features(z)
+        # z0 = (n_grid) * n_kernel * sizeafterconv
+        z0 = z0.view(n_grid, self.N_cnn_out).repeat(n_t, 1, 1)
+        if self.cat_first:
+            x = torch.cat((x, z0), dim=2)
+            x0 = F.relu(self.linearIn(x))
+        else:
+            x = F.relu(self.linearIn(x))
+            x0 = torch.cat((x, z0), dim=2)
+        out_lstm, (hn, cn) = self.lstm(x0, do_drop_mc=do_drop_mc)
+        return self.linearOut(out_lstm)
+
+
+class CudnnLstmModelLstmKernel(nn.Module):
+    """use a trained/un-trained CudnnLstm as a kernel generator before another CudnnLstm."""
+
+    def __init__(
+        self,
+        nx,
+        ny,
+        hidden_size,
+        nk=None,
+        hidden_size_later=None,
+        cut=False,
+        dr=0.5,
+        delta_s=False,
+    ):
+        """delta_s means we will use the difference of the first lstm's output and the second's as the final output"""
+        super(CudnnLstmModelLstmKernel, self).__init__()
+        # These three layers are same with CudnnLstmModel to be used for transfer learning or just vanilla-use
+        self.linearIn = torch.nn.Linear(nx, hidden_size)
+        self.lstm = CudnnLstm(input_size=hidden_size, hidden_size=hidden_size, dr=dr)
+        self.linearOut = torch.nn.Linear(hidden_size, ny)
+        # if cut is True, we will only select the final index in nk, and repeat it, then concatenate with x
+        self.cut = cut
+        # the second lstm has more input than the previous
+        if nk is None:
+            nk = ny
+        if hidden_size_later is None:
+            hidden_size_later = hidden_size
+        self.linear_in_later = torch.nn.Linear(nx + nk, hidden_size_later)
+        self.lstm_later = CudnnLstm(
+            input_size=hidden_size_later, hidden_size=hidden_size_later, dr=dr
+        )
+        self.linear_out_later = torch.nn.Linear(hidden_size_later, ny)
+
+        self.delta_s = delta_s
+        # when delta_s is true, cut cannot be true, because they have to have same number params
+        assert not (cut and delta_s)
+
+    def forward(self, x, do_drop_mc=False, dropout_false=False):
+        x0 = F.relu(self.linearIn(x))
+        out_lstm1, (hn1, cn1) = self.lstm(
+            x0, do_drop_mc=do_drop_mc, dropout_false=dropout_false
+        )
+        gen = self.linearOut(out_lstm1)
+        if self.cut:
+            gen = gen[-1, :, :].repeat(x.shape[0], 1, 1)
+        x1 = torch.cat((x, gen), dim=len(gen.shape) - 1)
+        x2 = F.relu(self.linear_in_later(x1))
+        out_lstm2, (hn2, cn2) = self.lstm_later(
+            x2, do_drop_mc=do_drop_mc, dropout_false=dropout_false
+        )
+        out = self.linear_out_later(out_lstm2)
+        return gen - out if self.delta_s else (out, gen)
+
+
+class CudnnLstmModelMultiOutput(nn.Module):
+    def __init__(
+        self,
+        n_input_features,
+        n_output_features,
+        n_hidden_states,
+        layer_hidden_size=(128, 64),
+        dr=0.5,
+        dr_hidden=0.0,
+    ):
+        """
+        Multiple output CudnnLSTM.
+
+        It has multiple output layers, each for one output, so that we can easily freeze any output layer.
+
+        Parameters
+        ----------
+        n_input_features
+            the size of input features
+        n_output_features
+            the size of output features; in this model, we set different nonlinear layer for each output
+        n_hidden_states
+            the size of LSTM's hidden features
+        layer_hidden_size
+            hidden_size for multi-layers
+        dr
+            dropout rate
+        dr_hidden
+            dropout rates of hidden layers
+        """
+        super(CudnnLstmModelMultiOutput, self).__init__()
+        self.ct = 0
+        multi_layers = torch.nn.ModuleList()
+        for i in range(n_output_features):
+            multi_layers.add_module(
+                "layer%d" % (i + 1),
+                SimpleAnn(n_hidden_states, 1, layer_hidden_size, dr=dr_hidden),
+            )
+        self.multi_layers = multi_layers
+        self.linearIn = torch.nn.Linear(n_input_features, n_hidden_states)
+        self.lstm = CudnnLstm(
+            input_size=n_hidden_states, hidden_size=n_hidden_states, dr=dr
+        )
+
+    def forward(self, x, do_drop_mc=False, dropout_false=False, return_h_c=False):
+        x0 = F.relu(self.linearIn(x))
+        out_lstm, (hn, cn) = self.lstm(
+            x0, do_drop_mc=do_drop_mc, dropout_false=dropout_false
+        )
+        outs = [mod(out_lstm) for mod in self.multi_layers]
+        final = torch.cat(outs, dim=-1)
+        return (final, (hn, cn)) if return_h_c else final
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `torchhydro-0.0.4/torchhydro/models/dpl4xaj.py` & `torchhydro-0.0.5/torchhydro/models/dpl4xaj.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,1084 +1,1084 @@
-"""
-Author: Wenyu Ouyang
-Date: 2023-09-19 09:36:25
-LastEditTime: 2023-10-06 19:31:02
-LastEditors: Wenyu Ouyang
-Description: 
-FilePath: \torchhydro\torchhydro\models\dpl4xaj.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-"""
-The method comes from this paper: https://doi.org/10.1038/s41467-021-26107-z
-It use Deep Learning (DL) methods to Learn the Parameters of physics-based models (PBM),
-which is called "differentiable parameter learning" (dPL).
-"""
-from typing import Optional, Union
-import torch
-from torch import nn
-from torch import Tensor
-from torch.nn import functional as F
-
-from torchhydro.configs.model_config import MODEL_PARAM_DICT
-from torchhydro.models.ann import SimpleAnn
-from torchhydro.models.kernel_conv import KernelConv
-from torchhydro.models.simple_lstm import SimpleLSTM
-
-
-PRECISION = 1e-5
-
-
-def calculate_evap(
-    lm, c, wu0, wl0, prcp, pet
-) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
-    """
-    Three-layers evaporation model from "Watershed Hydrologic Simulation" written by Prof. RenJun Zhao.
-
-    The book is Chinese, and its real name is 《流域水文模拟》;
-    The three-layers evaporation model is descibed in Page 76;
-    The method is same with that in Page 22-23 in "Hydrologic Forecasting (5-th version)" written by Prof. Weimin Bao.
-    This book's Chinese name is 《水文预报》
-
-    Parameters
-    ----------
-    lm
-        average soil moisture storage capacity of lower layer (mm)
-    c
-        coefficient of deep layer
-    wu0
-        initial soil moisture of upper layer; update in each time step (mm)
-    wl0
-        initial soil moisture of lower layer; update in each time step (mm)
-    prcp
-        basin mean precipitation (mm/day)
-    pet
-        potential evapotranspiration (mm/day)
-
-    Returns
-    -------
-    torch.Tensor
-        eu/el/ed are evaporation from upper/lower/deeper layer, respectively
-    """
-    tensor_min = torch.full(wu0.size(), 0.0).to(prcp.device)
-    # when using torch.where, please see here: https://github.com/pytorch/pytorch/issues/9190
-    # it's element-wise operation, no problem here. For example:
-    # In: torch.where(torch.Tensor([2,1])>torch.Tensor([1,1]),torch.Tensor([1,2]),torch.Tensor([3,4]))
-    # Out: tensor([1., 4.])
-    eu = torch.where(wu0 + prcp >= pet, pet, wu0 + prcp)
-    ed = torch.where(
-        (wl0 < c * lm) & (wl0 < c * (pet - eu)), c * (pet - eu) - wl0, tensor_min
-    )
-    el = torch.where(
-        wu0 + prcp >= pet,
-        tensor_min,
-        torch.where(
-            wl0 >= c * lm,
-            (pet - eu) * wl0 / lm,
-            torch.where(wl0 >= c * (pet - eu), c * (pet - eu), wl0),
-        ),
-    )
-    return eu, el, ed
-
-
-def calculate_prcp_runoff(b, im, wm, w0, pe):
-    """
-    Calculates the amount of runoff generated from rainfall after entering the underlying surface
-
-    Same in "Watershed Hydrologic Simulation" and "Hydrologic Forecasting (5-th version)"
-
-    Parameters
-    ----------
-    b
-        B exponent coefficient
-    im
-        IMP imperiousness coefficient
-    wm
-        average soil moisture storage capacity
-    w0
-        initial soil moisture
-    pe
-        net precipitation
-
-    Returns
-    -------
-    torch.Tensor
-        r -- runoff; r_im -- runoff of impervious part
-    """
-    wmm = wm * (1 + b)
-    a = wmm * (1 - (1 - w0 / wm) ** (1 / (1 + b)))
-    if any(torch.isnan(a)):
-        raise ValueError(
-            "Error: NaN values detected. Try set clamp function or check your data!!!"
-        )
-    r_cal = torch.where(
-        pe > 0.0,
-        torch.where(
-            pe + a < wmm,
-            # torch.clamp is used for gradient not to be NaN, see more in xaj_sources function
-            pe - (wm - w0) + wm * (1 - torch.clamp(a + pe, max=wmm) / wmm) ** (1 + b),
-            pe - (wm - w0),
-        ),
-        torch.full(pe.size(), 0.0).to(pe.device),
-    )
-    if any(torch.isnan(r_cal)):
-        raise ValueError(
-            "Error: NaN values detected. Try set clamp function or check your data!!!"
-        )
-    r = torch.clamp(r_cal, min=0.0)
-    r_im_cal = pe * im
-    r_im = torch.clamp(r_im_cal, min=0.0)
-    return r, r_im
-
-
-def calculate_w_storage(um, lm, dm, wu0, wl0, wd0, eu, el, ed, pe, r):
-    """
-    Update the soil moisture values of the three layers.
-
-    According to the runoff-generation equation 2.60 in the book "SHUIWENYUBAO", dW = dPE - dR
-
-    Parameters
-    ----------
-    um
-        average soil moisture storage capacity of the upper layer (mm)
-    lm
-        average soil moisture storage capacity of the lower layer (mm)
-    dm
-        average soil moisture storage capacity of the deep layer (mm)
-    wu0
-        initial values of soil moisture in upper layer
-    wl0
-        initial values of soil moisture in lower layer
-    wd0
-        initial values of soil moisture in deep layer
-    eu
-        evaporation of the upper layer; it isn't used in this function
-    el
-        evaporation of the lower layer
-    ed
-        evaporation of the deep layer
-    pe
-        net precipitation; it is able to be negative value in this function
-    r
-        runoff
-
-    Returns
-    -------
-    torch.Tensor
-        wu,wl,wd -- soil moisture in upper, lower and deep layer
-    """
-    xaj_device = pe.device
-    tensor_zeros = torch.full(wu0.size(), 0.0).to(xaj_device)
-    # pe>0: the upper soil moisture was added firstly, then lower layer, and the final is deep layer
-    # pe<=0: no additional water, just remove evapotranspiration,
-    # but note the case: e >= p > 0
-    # (1) if wu0 + p > e, then e = eu (2) else, wu must be zero
-    wu = torch.where(
-        pe > 0.0,
-        torch.where(wu0 + pe - r < um, wu0 + pe - r, um),
-        torch.where(wu0 + pe > 0.0, wu0 + pe, tensor_zeros),
-    )
-    # calculate wd before wl because it is easier to cal using where statement
-    wd = torch.where(
-        pe > 0.0,
-        torch.where(
-            wu0 + wl0 + pe - r > um + lm, wu0 + wl0 + wd0 + pe - r - um - lm, wd0
-        ),
-        wd0 - ed,
-    )
-    # water balance (equation 2.2 in Page 13, also shown in Page 23)
-    # if wu0 + p > e, then e = eu; else p must be used in upper layer,
-    # so no matter what the case is, el didn't include p, neither ed
-    wl = torch.where(pe > 0.0, wu0 + wl0 + wd0 + pe - r - wu - wd, wl0 - el)
-    # the water storage should be in reasonable range
-    tensor_mins = torch.full(um.size(), 0.0).to(xaj_device)
-    wu_ = torch.clamp(wu, min=tensor_mins, max=um)
-    wl_ = torch.clamp(wl, min=tensor_mins, max=lm)
-    wd_ = torch.clamp(wd, min=tensor_mins, max=dm)
-    return wu_, wl_, wd_
-
-
-def xaj_generation(
-    p_and_e: Tensor,
-    k,
-    b,
-    im,
-    um,
-    lm,
-    dm,
-    c,
-    wu0: Tensor = None,
-    wl0: Tensor = None,
-    wd0: Tensor = None,
-) -> tuple:
-    """
-    Single-step runoff generation in XAJ.
-
-    Parameters
-    ----------
-    p_and_e
-        precipitation and potential evapotranspiration (mm/day)
-    k
-        ratio of potential evapotranspiration to reference crop evaporation
-    b
-        exponent parameter
-    um
-        average soil moisture storage capacity of the upper layer (mm)
-    lm
-        average soil moisture storage capacity of the lower layer (mm)
-    dm
-        average soil moisture storage capacity of the deep layer (mm)
-    im
-        impermeability coefficient
-    c
-        coefficient of deep layer
-    wu0
-        initial values of soil moisture in upper layer (mm)
-    wl0
-        initial values of soil moisture in lower layer (mm)
-    wd0
-        initial values of soil moisture in deep layer (mm)
-
-    Returns
-    -------
-    tuple[torch.Tensor]
-        (r, rim, e, pe), (wu, wl, wd)
-    """
-    # make sure physical variables' value ranges are correct
-    prcp = torch.clamp(p_and_e[:, 0], min=0.0)
-    pet = torch.clamp(p_and_e[:, 1] * k, min=0.0)
-    # wm
-    wm = um + lm + dm
-    if wu0 is None:
-        # use detach func to make wu0 no_grad as it is an initial value
-        wu0 = 0.6 * (um.detach())
-    if wl0 is None:
-        wl0 = 0.6 * (lm.detach())
-    if wd0 is None:
-        wd0 = 0.6 * (dm.detach())
-    w0_ = wu0 + wl0 + wd0
-    # w0 need locate in correct range so that following calculation could be right
-    # To make sure the gradient is also not NaN (see case in xaj_sources),
-    # we'd better minus a precision (1e-5), although we've not met this situation (grad is NaN)
-    w0 = torch.clamp(w0_, max=wm - 1e-5)
-
-    # Calculate the amount of evaporation from storage
-    eu, el, ed = calculate_evap(lm, c, wu0, wl0, prcp, pet)
-    e = eu + el + ed
-
-    # Calculate the runoff generated by net precipitation
-    prcp_difference = prcp - e
-    pe = torch.clamp(prcp_difference, min=0.0)
-    r, rim = calculate_prcp_runoff(b, im, wm, w0, pe)
-    # Update wu, wl, wd;
-    # we use prcp_difference rather than pe, as when pe<0 but prcp>0, prcp should be considered
-    wu, wl, wd = calculate_w_storage(
-        um, lm, dm, wu0, wl0, wd0, eu, el, ed, prcp_difference, r
-    )
-
-    return (r, rim, e, pe), (wu, wl, wd)
-
-
-def xaj_sources(
-    pe,
-    r,
-    sm,
-    ex,
-    ki,
-    kg,
-    s0: Optional[Tensor] = None,
-    fr0: Optional[Tensor] = None,
-    book="HF",
-) -> tuple:
-    """
-    Divide the runoff to different sources
-
-    We use the initial version from the paper of the inventor of the XAJ model -- Prof. Renjun Zhao:
-    "Analysis of parameters of the XinAnJiang model". Its Chinese name is <<新安江模型参数的分析>>,
-    which could be found by searching in "Baidu Xueshu".
-    The module's code can also be found in "Watershed Hydrologic Simulation" (WHS) Page 174.
-    It is nearly same with that in "Hydrologic Forecasting" (HF) Page 148-149
-    We use the period average runoff as input and the unit period is day so we don't need to difference it as books show
-
-
-    Parameters
-    ------------
-    pe
-        net precipitation (mm/day)
-    r
-        runoff from xaj_generation (mm/day)
-    sm
-        areal mean free water capacity of the surface layer (mm)
-    ex
-        exponent of the free water capacity curve
-    ki
-        outflow coefficients of the free water storage to interflow relationships
-    kg
-        outflow coefficients of the free water storage to groundwater relationships
-    s0
-        initial free water capacity (mm)
-    fr0
-        runoff area of last period
-
-    Return
-    ------------
-    torch.Tensor
-        rs -- surface runoff; ri-- interflow runoff; rg -- groundwater runoff
-
-    """
-    xaj_device = pe.device
-    # maximum free water storage capacity in a basin
-    ms = sm * (1 + ex)
-    if fr0 is None:
-        fr0 = torch.full(sm.shape[0], 0.1).to(xaj_device)
-    if s0 is None:
-        s0 = 0.5 * (sm.clone().detach())
-    # For free water storage, because s is related to fr and s0 and fr0 are both values of last period,
-    # we have to trans the initial value of s from last period to this one.
-    # both WHS（流域水文模拟）'s sample code and HF（水文预报） use s = fr0 * s0 / fr.
-    # I think they both think free water reservoir as a cubic tank. Its height is s and area of bottom rectangle is fr
-    # we will have a cubic tank with varying bottom and height,
-    # and fixed boundary (in HF sm is fixed) or none-fixed boundary (in EH smmf is not fixed)
-    # but notice r's list like" [1,0] which 1 is the 1st period's runoff and 0 is the 2nd period's runoff
-    # after 1st period, the s1 could not be zero, but in the 2nd period, fr=0, then we cannot set s=0, because some water still in the tank
-    # fr's formula could be found in Eq. 9 in "Analysis of parameters of the XinAnJiang model",
-    # Here our r doesn't include rim, so there is no need to remove rim from r; this is also the method in HF
-    # Moreover, to make sure ss is not larger than sm, otherwise au will be nan value.
-    # It is worth to note that we have to use a precision here -- 1e-5, otherwise the gradient will be NaN;
-    # I guess maybe when calculating gradient -- Δy/Δx, Δ brings some precision problem when we need exponent function.
-
-    # NOTE: when r is 0, fr should be 0, however, s1 may not be zero and it still hold some water,
-    # then fr can not be 0, otherwise when fr is used as denominator it lead to error,
-    # so we have to deal with this case later, for example, when r=0, we cannot use pe * fr to replace r
-    # because fr get the value of last period, and it is not 0
-
-    # cannot use torch.where, because it will cause some error when calculating gradient
-    # fr = torch.where(r > 0.0, r / pe, fr0)
-    # fr just use fr0, and it can be included in the computation graph, so we don't detach it
-    fr = torch.clone(fr0)
-    fr_mask = r > 0.0
-    fr[fr_mask] = r[fr_mask] / pe[fr_mask]
-    if any(torch.isnan(fr)):
-        raise ValueError(
-            "Error: NaN values detected. Try set clamp function or check your data!!!"
-        )
-    if any(fr == 0.0):
-        raise ArithmeticError(
-            "Please check fr's value, fr==0.0 will cause error in the next step!"
-        )
-    ss = torch.clone(s0)
-    s = torch.clone(s0)
-
-    ss[fr_mask] = fr0[fr_mask] * s0[fr_mask] / fr[fr_mask]
-
-    if book == "HF":
-        ss = torch.clamp(ss, max=sm - PRECISION)
-        au = ms * (1.0 - (1.0 - ss / sm) ** (1.0 / (1.0 + ex)))
-        if any(torch.isnan(au)):
-            raise ValueError(
-                "Error: NaN values detected. Try set clamp function or check your data!!!"
-            )
-
-        rs = torch.full_like(r, 0.0, device=xaj_device)
-        rs[fr_mask] = torch.where(
-            pe[fr_mask] + au[fr_mask] < ms[fr_mask],
-            # equation 2-85 in HF
-            # it's weird here, but we have to clamp so that the gradient could be not NaN;
-            # otherwise, even the forward calculation is correct, the gradient is still NaN;
-            # maybe when calculating gradient -- Δy/Δx, Δ brings some precision problem
-            # if we need exponent function.
-            fr[fr_mask]
-            * (
-                pe[fr_mask]
-                - sm[fr_mask]
-                + ss[fr_mask]
-                + sm[fr_mask]
-                * (
-                    (
-                        1
-                        - torch.clamp(pe[fr_mask] + au[fr_mask], max=ms[fr_mask])
-                        / ms[fr_mask]
-                    )
-                    ** (1 + ex[fr_mask])
-                )
-            ),
-            # equation 2-86 in HF
-            fr[fr_mask] * (pe[fr_mask] + ss[fr_mask] - sm[fr_mask]),
-        )
-        rs = torch.clamp(rs, max=r)
-        # ri's mask is not same as rs's, because last period's s may not be 0
-        # and in this time, ri and rg could be larger than 0
-        # we need firstly calculate the updated s, s's mask is same as fr_mask,
-        # when r==0, then s will be equal to last period's
-        # equation 2-87 in HF, some free water leave or save, so we update free water storage
-        s[fr_mask] = ss[fr_mask] + (r[fr_mask] - rs[fr_mask]) / fr[fr_mask]
-        s = torch.clamp(s, max=sm)
-    elif book == "EH":
-        smmf = ms * (1 - (1 - fr) ** (1 / ex))
-        smf = smmf / (1 + ex)
-        ss = torch.clamp(ss, max=smf - PRECISION)
-        au = smmf * (1 - (1 - ss / smf) ** (1 / (1 + ex)))
-        if torch.isnan(au).any():
-            raise ArithmeticError(
-                "Error: NaN values detected. Try set clip function or check your data!!!"
-            )
-        rs = torch.full_like(r, 0.0, device=xaj_device)
-        rs[fr_mask] = torch.where(
-            pe[fr_mask] + au[fr_mask] < smmf[fr_mask],
-            (
-                pe[fr_mask]
-                - smf[fr_mask]
-                + ss[fr_mask]
-                + smf[fr_mask]
-                * (
-                    1
-                    - torch.clamp(
-                        pe[fr_mask] + au[fr_mask],
-                        max=smmf[fr_mask],
-                    )
-                    / smmf[fr_mask]
-                )
-                ** (ex[fr_mask] + 1)
-            )
-            * fr[fr_mask],
-            (pe[fr_mask] + ss[fr_mask] - smf[fr_mask]) * fr[fr_mask],
-        )
-        rs = torch.clamp(rs, max=r)
-        s[fr_mask] = ss[fr_mask] + (r[fr_mask] - rs[fr_mask]) / fr[fr_mask]
-        s[fr_mask] = torch.clamp(s[fr_mask], max=smf[fr_mask])
-        s = torch.clamp(s, max=smf)
-    else:
-        raise ValueError("Please set book as 'HF' or 'EH'!")
-    # equation 2-88 in HF, next interflow and ground water will be released from the updated free water storage
-    # We use the period average runoff as input and the unit period is day.
-    # Hence, we directly use ki and kg rather than ki_{Δt} in books.
-    ri = ki * s * fr
-    rg = kg * s * fr
-    # equation 2-89 in HF; although it looks different with that in WHS, they are actually same
-    # Finally, calculate the final free water storage
-    s1 = s * (1 - ki - kg)
-    return (rs, ri, rg), (s1, fr)
-
-
-def xaj_sources5mm(
-    pe,
-    runoff,
-    sm,
-    ex,
-    ki,
-    kg,
-    s0=None,
-    fr0=None,
-    book="HF",
-):
-    """
-    Divide the runoff to different sources according to books -- 《水文预报》HF 5th edition and 《工程水文学》EH 3rd edition
-
-    Parameters
-    ----------
-    pe
-        net precipitation
-    runoff
-        runoff from xaj_generation
-    sm
-        areal mean free water capacity of the surface layer
-    ex
-        exponent of the free water capacity curve
-    ki
-        outflow coefficients of the free water storage to interflow relationships
-    kg
-        outflow coefficients of the free water storage to groundwater relationships
-    s0
-        initial free water capacity
-    fr0
-        initial area of generation
-    time_interval_hours
-        由于Ki、Kg、Ci、Cg都是以24小时为时段长定义的,需根据时段长转换
-    book
-        the methods in 《水文预报》HF 5th edition and 《工程水文学》EH 3rd edition are different,
-        hence, both are provided, and the default is the former -- "ShuiWenYuBao";
-        the other one is "GongChengShuiWenXue"
-
-    Returns
-    -------
-    tuple[tuple, tuple]
-        rs_s -- surface runoff; rss_s-- interflow runoff; rg_s -- groundwater runoff;
-        (fr_ds[-1], s_ds[-1]): state variables' final value;
-        all variables are numpy array
-    """
-    xaj_device = pe.device
-    # 流域最大点自由水蓄水容量深
-    smm = sm * (1 + ex)
-    if fr0 is None:
-        fr0 = torch.full_like(sm, 0.1, device=xaj_device)
-    if s0 is None:
-        s0 = 0.5 * (sm.clone().detach())
-    fr = torch.clone(fr0)
-    fr_mask = runoff > 0.0
-    fr[fr_mask] = runoff[fr_mask] / pe[fr_mask]
-    if torch.all(runoff < 5):
-        n = 1
-    else:
-        r_max = torch.max(runoff).detach().cpu().numpy()
-        residue_temp = r_max % 5
-        if residue_temp != 0:
-            residue_temp = 1
-        n = int(r_max / 5) + residue_temp
-    rn = runoff / n
-    pen = pe / n
-    kss_d = (1 - (1 - (ki + kg)) ** (1 / n)) / (1 + kg / ki)
-    kg_d = kss_d * kg / ki
-    if torch.isnan(kss_d).any() or torch.isnan(kg_d).any():
-        raise ValueError("Error: NaN values detected. Check your parameters setting!!!")
-    # kss_d = ki
-    # kg_d = kg
-
-    rs = torch.full_like(runoff, 0.0, device=xaj_device)
-    rss = torch.full_like(runoff, 0.0, device=xaj_device)
-    rg = torch.full_like(runoff, 0.0, device=xaj_device)
-
-    s_ds = []
-    fr_ds = []
-    s_ds.append(s0)
-    fr_ds.append(fr0)
-    for j in range(n):
-        fr0_d = fr_ds[j]
-        s0_d = s_ds[j]
-        # equation 5-32 in HF, but strange, cause each period, rn/pen is same
-        # fr_d = torch.full_like(fr0_d, PRECISION, device=xaj_device)
-        # fr_d_mask = fr > PRECISION
-        # fr_d[fr_d_mask] = 1 - (1 - fr[fr_d_mask]) ** (1 / n)
-        fr_d = fr
-
-        ss_d = torch.clone(s0_d)
-        s_d = torch.clone(s0_d)
-
-        ss_d[fr_mask] = fr0_d[fr_mask] * s0_d[fr_mask] / fr_d[fr_mask]
-
-        if book == "HF":
-            # ms = smm
-            ss_d = torch.clamp(ss_d, max=sm - PRECISION)
-            au = smm * (1.0 - (1.0 - ss_d / sm) ** (1.0 / (1.0 + ex)))
-            if torch.isnan(au).any():
-                raise ValueError(
-                    "Error: NaN values detected. Try set clip function or check your data!!!"
-                )
-            rs_j = torch.full_like(rn, 0.0, device=xaj_device)
-            rs_j[fr_mask] = torch.where(
-                pen[fr_mask] + au[fr_mask] < smm[fr_mask],
-                # equation 5-26 in HF
-                fr_d[fr_mask]
-                * (
-                    pen[fr_mask]
-                    - sm[fr_mask]
-                    + ss_d[fr_mask]
-                    + sm[fr_mask]
-                    * (
-                        (
-                            1
-                            - torch.clamp(pen[fr_mask] + au[fr_mask], max=smm[fr_mask])
-                            / smm[fr_mask]
-                        )
-                        ** (1 + ex[fr_mask])
-                    )
-                ),
-                # equation 5-27 in HF
-                fr_d[fr_mask] * (pen[fr_mask] + ss_d[fr_mask] - sm[fr_mask]),
-            )
-            rs_j = torch.clamp(rs_j, max=rn)
-            s_d[fr_mask] = ss_d[fr_mask] + (rn[fr_mask] - rs_j[fr_mask]) / fr_d[fr_mask]
-            s_d = torch.clamp(s_d, max=sm)
-
-        elif book == "EH":
-            smmf = smm * (1 - (1 - fr_d) ** (1 / ex))
-            smf = smmf / (1 + ex)
-            ss_d = torch.clamp(ss_d, max=smf - PRECISION)
-            au = smmf * (1 - (1 - ss_d / smf) ** (1 / (1 + ex)))
-            if torch.isnan(au).any():
-                raise ValueError(
-                    "Error: NaN values detected. Try set clip function or check your data!!!"
-                )
-            rs_j = torch.full(rn.size(), 0.0).to(xaj_device)
-            rs_j[fr_mask] = torch.where(
-                pen[fr_mask] + au[fr_mask] < smmf[fr_mask],
-                (
-                    pen[fr_mask]
-                    - smf[fr_mask]
-                    + ss_d[fr_mask]
-                    + smf[fr_mask]
-                    * (
-                        1
-                        - torch.clamp(
-                            pen[fr_mask] + au[fr_mask],
-                            max=smmf[fr_mask],
-                        )
-                        / smmf[fr_mask]
-                    )
-                    ** (ex[fr_mask] + 1)
-                )
-                * fr_d[fr_mask],
-                (pen[fr_mask] + ss_d[fr_mask] - smf[fr_mask]) * fr_d[fr_mask],
-            )
-            rs_j = torch.clamp(rs_j, max=rn)
-            s_d[fr_mask] = ss_d[fr_mask] + (rn[fr_mask] - rs_j[fr_mask]) / fr_d[fr_mask]
-            s_d = torch.clamp(s_d, max=smf)
-        else:
-            raise NotImplementedError(
-                "We don't have this implementation! Please chose 'HF' or 'EH'!!"
-            )
-
-        rss_j = s_d * kss_d * fr_d
-        rg_j = s_d * kg_d * fr_d
-        s1_d = s_d * (1 - kss_d - kg_d)
-
-        rs = rs + rs_j
-        rss = rss + rss_j
-        rg = rg + rg_j
-        # 赋值s_d和fr_d到数组中，以给下一段做初值
-        s_ds.append(s1_d)
-        fr_ds.append(fr_d)
-
-    return (rs, rss, rg), (s_ds[-1], fr_ds[-1])
-
-
-def linear_reservoir(x, weight, last_y: Optional[Tensor] = None):
-    """
-    Linear reservoir's release function
-
-    Parameters
-    ----------
-    x
-        the input to the linear reservoir
-    weight
-        the coefficient of linear reservoir
-    last_y
-        the output of last period
-
-    Returns
-    -------
-    torch.Tensor
-        one-step forward result
-    """
-    weight1 = 1 - weight
-    if last_y is None:
-        last_y = torch.full(weight.size(), 0.001).to(x.device)
-    y = weight * last_y + weight1 * x
-    return y
-
-
-class Xaj4Dpl(nn.Module):
-    """
-    XAJ model for Differential Parameter learning
-    """
-
-    def __init__(
-        self,
-        kernel_size: int,
-        warmup_length: int,
-        source_book="HF",
-        source_type="sources",
-    ):
-        """
-        Parameters
-        ----------
-        kernel_size
-            the time length of unit hydrograph
-        warmup_length
-            the length of warmup periods;
-            XAJ needs a warmup period to generate reasonable initial state values
-        """
-        super(Xaj4Dpl, self).__init__()
-        self.params_names = MODEL_PARAM_DICT["xaj_mz"]["param_name"]
-        param_range = MODEL_PARAM_DICT["xaj_mz"]["param_range"]
-        self.k_scale = param_range["K"]
-        self.b_scale = param_range["B"]
-        self.im_sacle = param_range["IM"]
-        self.um_scale = param_range["UM"]
-        self.lm_scale = param_range["LM"]
-        self.dm_scale = param_range["DM"]
-        self.c_scale = param_range["C"]
-        self.sm_scale = param_range["SM"]
-        self.ex_scale = param_range["EX"]
-        self.ki_scale = param_range["KI"]
-        self.kg_scale = param_range["KG"]
-        self.a_scale = param_range["A"]
-        self.theta_scale = param_range["THETA"]
-        self.ci_scale = param_range["CI"]
-        self.cg_scale = param_range["CG"]
-        self.kernel_size = kernel_size
-        self.warmup_length = warmup_length
-        # there are 2 input variables in XAJ: P and PET
-        self.feature_size = 2
-        self.source_book = source_book
-        self.source_type = source_type
-
-    def forward(self, p_and_e, parameters, return_state=False):
-        """
-        run XAJ model
-
-        Parameters
-        ----------
-        p_and_e
-            precipitation and potential evapotranspiration
-        parameters
-            parameters of XAJ model
-        return_state
-            if True, return state values, mainly for warmup periods
-
-        Returns
-        -------
-        torch.Tensor
-            streamflow got by XAJ
-        """
-        xaj_device = p_and_e.device
-        # denormalize the parameters to general range
-        k = self.k_scale[0] + parameters[:, 0] * (self.k_scale[1] - self.k_scale[0])
-        b = self.b_scale[0] + parameters[:, 1] * (self.b_scale[1] - self.b_scale[0])
-        im = self.im_sacle[0] + parameters[:, 2] * (self.im_sacle[1] - self.im_sacle[0])
-        um = self.um_scale[0] + parameters[:, 3] * (self.um_scale[1] - self.um_scale[0])
-        lm = self.lm_scale[0] + parameters[:, 4] * (self.lm_scale[1] - self.lm_scale[0])
-        dm = self.dm_scale[0] + parameters[:, 5] * (self.dm_scale[1] - self.dm_scale[0])
-        c = self.c_scale[0] + parameters[:, 6] * (self.c_scale[1] - self.c_scale[0])
-        sm = self.sm_scale[0] + parameters[:, 7] * (self.sm_scale[1] - self.sm_scale[0])
-        ex = self.ex_scale[0] + parameters[:, 8] * (self.ex_scale[1] - self.ex_scale[0])
-        ki_ = self.ki_scale[0] + parameters[:, 9] * (
-            self.ki_scale[1] - self.ki_scale[0]
-        )
-        kg_ = self.kg_scale[0] + parameters[:, 10] * (
-            self.kg_scale[1] - self.kg_scale[0]
-        )
-        # ki+kg should be smaller than 1; if not, we scale them, but note float only contain 4 digits, so we need 0.999
-        ki = torch.where(
-            ki_ + kg_ < 1.0,
-            ki_,
-            (1 - PRECISION) / (ki_ + kg_) * ki_,
-        )
-        kg = torch.where(
-            ki_ + kg_ < 1.0,
-            kg_,
-            (1 - PRECISION) / (ki_ + kg_) * kg_,
-        )
-        a = self.a_scale[0] + parameters[:, 11] * (self.a_scale[1] - self.a_scale[0])
-        theta = self.theta_scale[0] + parameters[:, 12] * (
-            self.theta_scale[1] - self.theta_scale[0]
-        )
-        ci = self.ci_scale[0] + parameters[:, 13] * (
-            self.ci_scale[1] - self.ci_scale[0]
-        )
-        cg = self.cg_scale[0] + parameters[:, 14] * (
-            self.cg_scale[1] - self.cg_scale[0]
-        )
-
-        # initialize state values
-        warmup_length = self.warmup_length
-        if warmup_length > 0:
-            # set no_grad for warmup periods
-            with torch.no_grad():
-                p_and_e_warmup = p_and_e[0:warmup_length, :, :]
-                cal_init_xaj4dpl = Xaj4Dpl(
-                    self.kernel_size, 0, self.source_book, self.source_type
-                )
-                if cal_init_xaj4dpl.warmup_length > 0:
-                    raise RuntimeError("Please set init model's warmup length to 0!!!")
-                _, _, *w0, s0, fr0, qi0, qg0 = cal_init_xaj4dpl(
-                    p_and_e_warmup, parameters, return_state=True
-                )
-        else:
-            # use detach func to make wu0 no_grad as it is an initial value
-            w0 = (0.5 * (um.detach()), 0.5 * (lm.detach()), 0.5 * (dm.detach()))
-            s0 = 0.5 * (sm.detach())
-            fr0 = torch.full(ci.size(), 0.1).to(xaj_device)
-            qi0 = torch.full(ci.size(), 0.1).to(xaj_device)
-            qg0 = torch.full(cg.size(), 0.1).to(xaj_device)
-
-        inputs = p_and_e[warmup_length:, :, :]
-        runoff_ims_ = torch.full(inputs.shape[:2], 0.0).to(xaj_device)
-        rss_ = torch.full(inputs.shape[:2], 0.0).to(xaj_device)
-        ris_ = torch.full(inputs.shape[:2], 0.0).to(xaj_device)
-        rgs_ = torch.full(inputs.shape[:2], 0.0).to(xaj_device)
-        es_ = torch.full(inputs.shape[:2], 0.0).to(xaj_device)
-        for i in range(inputs.shape[0]):
-            if i == 0:
-                (r, rim, e, pe), w = xaj_generation(
-                    inputs[i, :, :], k, b, im, um, lm, dm, c, *w0
-                )
-                if self.source_type == "sources":
-                    (rs, ri, rg), (s, fr) = xaj_sources(
-                        pe, r, sm, ex, ki, kg, s0, fr0, book=self.source_book
-                    )
-                elif self.source_type == "sources5mm":
-                    (rs, ri, rg), (s, fr) = xaj_sources5mm(
-                        pe, r, sm, ex, ki, kg, s0, fr0, book=self.source_book
-                    )
-                else:
-                    raise NotImplementedError("No such divide-sources method")
-            else:
-                (r, rim, e, pe), w = xaj_generation(
-                    inputs[i, :, :], k, b, im, um, lm, dm, c, *w
-                )
-                if self.source_type == "sources":
-                    (rs, ri, rg), (s, fr) = xaj_sources(
-                        pe, r, sm, ex, ki, kg, s, fr, book=self.source_book
-                    )
-                elif self.source_type == "sources5mm":
-                    (rs, ri, rg), (s, fr) = xaj_sources5mm(
-                        pe, r, sm, ex, ki, kg, s, fr, book=self.source_book
-                    )
-                else:
-                    raise NotImplementedError("No such divide-sources method")
-            # impevious part is pe * im
-            runoff_ims_[i, :] = rim
-            # so for non-imprvious part, the result should be corrected
-            rss_[i, :] = rs * (1 - im)
-            ris_[i, :] = ri * (1 - im)
-            rgs_[i, :] = rg * (1 - im)
-            es_[i, :] = e
-            # rss_[i, :] = 0.7 * r
-            # ris_[i, :] = 0.2 * r
-            # rgs_[i, :] = 0.1 * r
-        # seq, batch, feature
-        runoff_im = torch.unsqueeze(runoff_ims_, dim=2)
-        rss = torch.unsqueeze(rss_, dim=2)
-        es = torch.unsqueeze(es_, dim=2)
-
-        conv_uh = KernelConv(a, theta, self.kernel_size)
-        qs_ = conv_uh(runoff_im + rss)
-        qs = torch.full(inputs.shape[:2], 0.0).to(xaj_device)
-        for i in range(inputs.shape[0]):
-            if i == 0:
-                qi = linear_reservoir(ris_[i], ci, qi0)
-                qg = linear_reservoir(rgs_[i], cg, qg0)
-            else:
-                qi = linear_reservoir(ris_[i], ci, qi)
-                qg = linear_reservoir(rgs_[i], cg, qg)
-            qs[i, :] = qs_[i, :, 0] + qi + qg
-        # seq, batch, feature
-        q_sim = torch.unsqueeze(qs, dim=2)
-        if return_state:
-            return q_sim, es, *w, s, fr, qi, qg
-        return q_sim, es
-
-
-class DplLstmXaj(nn.Module):
-    def __init__(
-        self,
-        n_input_features,
-        n_output_features,
-        n_hidden_states,
-        kernel_size,
-        warmup_length,
-        param_limit_func="sigmoid",
-        param_test_way="final",
-        source_book="HF",
-        source_type="sources",
-    ):
-        """
-        Differential Parameter learning model: LSTM -> Param -> XAJ
-
-        The principle can be seen here: https://doi.org/10.1038/s41467-021-26107-z
-
-        Parameters
-        ----------
-        n_input_features
-            the number of input features of LSTM
-        n_output_features
-            the number of output features of LSTM, and it should be equal to the number of learning parameters in XAJ
-        n_hidden_states
-            the number of hidden features of LSTM
-        kernel_size
-            the time length of unit hydrograph
-        warmup_length
-            the length of warmup periods;
-            hydrologic models need a warmup period to generate reasonable initial state values
-        param_limit_func
-            function used to limit the range of params; now it is sigmoid or clamp function
-        param_test_way
-            how we use parameters from dl model when testing;
-            now we have three ways:
-            1. "final" -- use the final period's parameter for each period
-            2. "mean_time" -- Mean values of all periods' parameters is used
-            3. "mean_basin" -- Mean values of all basins' final periods' parameters is used
-        """
-        super(DplLstmXaj, self).__init__()
-        self.dl_model = SimpleLSTM(n_input_features, n_output_features, n_hidden_states)
-        self.pb_model = Xaj4Dpl(
-            kernel_size, warmup_length, source_book=source_book, source_type=source_type
-        )
-        self.param_func = param_limit_func
-        self.param_test_way = param_test_way
-
-    def forward(self, x, z):
-        """
-        Differential parameter learning
-
-        z (normalized input) -> lstm -> param -> + x (not normalized) -> xaj -> q
-        Parameters will be denormalized in xaj model
-
-        Parameters
-        ----------
-        x
-            not normalized data used for physical model; a sequence-first 3-dim tensor. [sequence, batch, feature]
-        z
-            normalized data used for DL model; a sequence-first 3-dim tensor. [sequence, batch, feature]
-
-        Returns
-        -------
-        torch.Tensor
-            one time forward result
-        """
-        q, e = lstm_pbm(self.dl_model, self.pb_model, self.param_func, x, z)
-        return q
-
-
-class DplAnnXaj(nn.Module):
-    def __init__(
-        self,
-        n_input_features: int,
-        n_output_features: int,
-        n_hidden_states: Union[int, tuple, list],
-        dr: Union[int, tuple, list],
-        kernel_size: int,
-        warmup_length: int,
-        param_limit_func="sigmoid",
-        param_test_way="final",
-        source_book="HF",
-        source_type="sources",
-    ):
-        """
-        Differential Parameter learning model only with attributes as DL model's input: ANN -> Param -> Gr4j
-
-        The principle can be seen here: https://doi.org/10.1038/s41467-021-26107-z
-
-        Parameters
-        ----------
-        n_input_features
-            the number of input features of ANN
-        n_output_features
-            the number of output features of ANN, and it should be equal to the number of learning parameters in XAJ
-        n_hidden_states
-            the number of hidden features of ANN; it could be Union[int, tuple, list]
-        kernel_size
-            the time length of unit hydrograph
-        warmup_length
-            the length of warmup periods;
-            hydrologic models need a warmup period to generate reasonable initial state values
-        param_limit_func
-            function used to limit the range of params; now it is sigmoid or clamp function
-        param_test_way
-            how we use parameters from dl model when testing;
-            now we have three ways:
-            1. "final" -- use the final period's parameter for each period
-            2. "mean_time" -- Mean values of all periods' parameters is used
-            3. "mean_basin" -- Mean values of all basins' final periods' parameters is used
-        """
-        super(DplAnnXaj, self).__init__()
-        self.dl_model = SimpleAnn(
-            n_input_features, n_output_features, n_hidden_states, dr
-        )
-        self.pb_model = Xaj4Dpl(
-            kernel_size, warmup_length, source_book=source_book, source_type=source_type
-        )
-        self.param_func = param_limit_func
-        self.param_test_way = param_test_way
-
-    def forward(self, x, z):
-        """
-        Differential parameter learning
-
-        z (normalized input) -> ANN -> param -> + x (not normalized) -> gr4j -> q
-        Parameters will be denormalized in gr4j model
-
-        Parameters
-        ----------
-        x
-            not normalized data used for physical model; a sequence-first 3-dim tensor. [sequence, batch, feature]
-        z
-            normalized data used for DL model; a 2-dim tensor. [batch, feature]
-
-        Returns
-        -------
-        torch.Tensor
-            one time forward result
-        """
-        q, e = ann_pbm(self.dl_model, self.pb_model, self.param_func, x, z)
-        return q
-
-
-def lstm_pbm(dl_model, pb_model, param_func, x, z):
-    """
-    Differential parameter learning
-
-    z (normalized input) -> lstm -> param -> + x (not normalized) -> pbm -> q
-    Parameters will be denormalized in pbm model
-
-    Parameters
-    ----------
-    dl_model
-        lstm model
-    pb_model
-        physics-based model
-    param_func
-        function used to limit the range of params; now it is sigmoid or clamp function
-    x
-        not normalized data used for physical model; a sequence-first 3-dim tensor. [sequence, batch, feature]
-    z
-        normalized data used for DL model; a sequence-first 3-dim tensor. [sequence, batch, feature]
-
-    Returns
-    -------
-    torch.Tensor
-            one time forward result
-    """
-    gen = dl_model(z)
-    if torch.isnan(gen).any():
-        raise ValueError("Error: NaN values detected. Check your data firstly!!!")
-    # we set all params' values in [0, 1] and will scale them when forwarding
-    if param_func == "sigmoid":
-        params_ = F.sigmoid(gen)
-    elif param_func == "clamp":
-        params_ = torch.clamp(gen, min=0.0, max=1.0)
-    else:
-        raise NotImplementedError(
-            "We don't provide this way to limit parameters' range!! Please choose sigmoid or clamp"
-        )
-    # just get one-period values, here we use the final period's values
-    params = params_[-1, :, :]
-    return pb_model(x[:, :, : pb_model.feature_size], params)
-
-
-def ann_pbm(dl_model, pb_model, param_func, x, z):
-    """
-    Differential parameter learning
-
-    z (normalized input) -> ann -> param -> + x (not normalized) -> pbm -> q
-    Parameters will be denormalized in pbm model
-
-    Parameters
-    ----------
-    dl_model
-        ann model
-    pb_model
-        physics-based model
-    param_func
-        function used to limit the range of params; now it is sigmoid or clamp function
-    x
-        not normalized data used for physical model; a sequence-first 3-dim tensor. [sequence, batch, feature]
-    z
-        normalized data used for DL model; a 2-dim tensor. [batch, feature]
-
-    Returns
-    -------
-    torch.Tensor
-        one time forward result
-    """
-    gen = dl_model(z)
-    if torch.isnan(gen).any():
-        raise ValueError("Error: NaN values detected. Check your data firstly!!!")
-    # we set all params' values in [0, 1] and will scale them when forwarding
-    if param_func == "sigmoid":
-        params = F.sigmoid(gen)
-    elif param_func == "clamp":
-        params = torch.clamp(gen, min=0.0, max=1.0)
-    else:
-        raise NotImplementedError(
-            "We don't provide this way to limit parameters' range!! Please choose sigmoid or clamp"
-        )
-    return pb_model(x[:, :, : pb_model.feature_size], params)
+"""
+Author: Wenyu Ouyang
+Date: 2023-09-19 09:36:25
+LastEditTime: 2023-10-06 19:31:02
+LastEditors: Wenyu Ouyang
+Description: 
+FilePath: \torchhydro\torchhydro\models\dpl4xaj.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+"""
+The method comes from this paper: https://doi.org/10.1038/s41467-021-26107-z
+It use Deep Learning (DL) methods to Learn the Parameters of physics-based models (PBM),
+which is called "differentiable parameter learning" (dPL).
+"""
+from typing import Optional, Union
+import torch
+from torch import nn
+from torch import Tensor
+from torch.nn import functional as F
+
+from torchhydro.configs.model_config import MODEL_PARAM_DICT
+from torchhydro.models.ann import SimpleAnn
+from torchhydro.models.kernel_conv import KernelConv
+from torchhydro.models.simple_lstm import SimpleLSTM
+
+
+PRECISION = 1e-5
+
+
+def calculate_evap(
+    lm, c, wu0, wl0, prcp, pet
+) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+    """
+    Three-layers evaporation model from "Watershed Hydrologic Simulation" written by Prof. RenJun Zhao.
+
+    The book is Chinese, and its real name is 《流域水文模拟》;
+    The three-layers evaporation model is descibed in Page 76;
+    The method is same with that in Page 22-23 in "Hydrologic Forecasting (5-th version)" written by Prof. Weimin Bao.
+    This book's Chinese name is 《水文预报》
+
+    Parameters
+    ----------
+    lm
+        average soil moisture storage capacity of lower layer (mm)
+    c
+        coefficient of deep layer
+    wu0
+        initial soil moisture of upper layer; update in each time step (mm)
+    wl0
+        initial soil moisture of lower layer; update in each time step (mm)
+    prcp
+        basin mean precipitation (mm/day)
+    pet
+        potential evapotranspiration (mm/day)
+
+    Returns
+    -------
+    torch.Tensor
+        eu/el/ed are evaporation from upper/lower/deeper layer, respectively
+    """
+    tensor_min = torch.full(wu0.size(), 0.0).to(prcp.device)
+    # when using torch.where, please see here: https://github.com/pytorch/pytorch/issues/9190
+    # it's element-wise operation, no problem here. For example:
+    # In: torch.where(torch.Tensor([2,1])>torch.Tensor([1,1]),torch.Tensor([1,2]),torch.Tensor([3,4]))
+    # Out: tensor([1., 4.])
+    eu = torch.where(wu0 + prcp >= pet, pet, wu0 + prcp)
+    ed = torch.where(
+        (wl0 < c * lm) & (wl0 < c * (pet - eu)), c * (pet - eu) - wl0, tensor_min
+    )
+    el = torch.where(
+        wu0 + prcp >= pet,
+        tensor_min,
+        torch.where(
+            wl0 >= c * lm,
+            (pet - eu) * wl0 / lm,
+            torch.where(wl0 >= c * (pet - eu), c * (pet - eu), wl0),
+        ),
+    )
+    return eu, el, ed
+
+
+def calculate_prcp_runoff(b, im, wm, w0, pe):
+    """
+    Calculates the amount of runoff generated from rainfall after entering the underlying surface
+
+    Same in "Watershed Hydrologic Simulation" and "Hydrologic Forecasting (5-th version)"
+
+    Parameters
+    ----------
+    b
+        B exponent coefficient
+    im
+        IMP imperiousness coefficient
+    wm
+        average soil moisture storage capacity
+    w0
+        initial soil moisture
+    pe
+        net precipitation
+
+    Returns
+    -------
+    torch.Tensor
+        r -- runoff; r_im -- runoff of impervious part
+    """
+    wmm = wm * (1 + b)
+    a = wmm * (1 - (1 - w0 / wm) ** (1 / (1 + b)))
+    if any(torch.isnan(a)):
+        raise ValueError(
+            "Error: NaN values detected. Try set clamp function or check your data!!!"
+        )
+    r_cal = torch.where(
+        pe > 0.0,
+        torch.where(
+            pe + a < wmm,
+            # torch.clamp is used for gradient not to be NaN, see more in xaj_sources function
+            pe - (wm - w0) + wm * (1 - torch.clamp(a + pe, max=wmm) / wmm) ** (1 + b),
+            pe - (wm - w0),
+        ),
+        torch.full(pe.size(), 0.0).to(pe.device),
+    )
+    if any(torch.isnan(r_cal)):
+        raise ValueError(
+            "Error: NaN values detected. Try set clamp function or check your data!!!"
+        )
+    r = torch.clamp(r_cal, min=0.0)
+    r_im_cal = pe * im
+    r_im = torch.clamp(r_im_cal, min=0.0)
+    return r, r_im
+
+
+def calculate_w_storage(um, lm, dm, wu0, wl0, wd0, eu, el, ed, pe, r):
+    """
+    Update the soil moisture values of the three layers.
+
+    According to the runoff-generation equation 2.60 in the book "SHUIWENYUBAO", dW = dPE - dR
+
+    Parameters
+    ----------
+    um
+        average soil moisture storage capacity of the upper layer (mm)
+    lm
+        average soil moisture storage capacity of the lower layer (mm)
+    dm
+        average soil moisture storage capacity of the deep layer (mm)
+    wu0
+        initial values of soil moisture in upper layer
+    wl0
+        initial values of soil moisture in lower layer
+    wd0
+        initial values of soil moisture in deep layer
+    eu
+        evaporation of the upper layer; it isn't used in this function
+    el
+        evaporation of the lower layer
+    ed
+        evaporation of the deep layer
+    pe
+        net precipitation; it is able to be negative value in this function
+    r
+        runoff
+
+    Returns
+    -------
+    torch.Tensor
+        wu,wl,wd -- soil moisture in upper, lower and deep layer
+    """
+    xaj_device = pe.device
+    tensor_zeros = torch.full(wu0.size(), 0.0).to(xaj_device)
+    # pe>0: the upper soil moisture was added firstly, then lower layer, and the final is deep layer
+    # pe<=0: no additional water, just remove evapotranspiration,
+    # but note the case: e >= p > 0
+    # (1) if wu0 + p > e, then e = eu (2) else, wu must be zero
+    wu = torch.where(
+        pe > 0.0,
+        torch.where(wu0 + pe - r < um, wu0 + pe - r, um),
+        torch.where(wu0 + pe > 0.0, wu0 + pe, tensor_zeros),
+    )
+    # calculate wd before wl because it is easier to cal using where statement
+    wd = torch.where(
+        pe > 0.0,
+        torch.where(
+            wu0 + wl0 + pe - r > um + lm, wu0 + wl0 + wd0 + pe - r - um - lm, wd0
+        ),
+        wd0 - ed,
+    )
+    # water balance (equation 2.2 in Page 13, also shown in Page 23)
+    # if wu0 + p > e, then e = eu; else p must be used in upper layer,
+    # so no matter what the case is, el didn't include p, neither ed
+    wl = torch.where(pe > 0.0, wu0 + wl0 + wd0 + pe - r - wu - wd, wl0 - el)
+    # the water storage should be in reasonable range
+    tensor_mins = torch.full(um.size(), 0.0).to(xaj_device)
+    wu_ = torch.clamp(wu, min=tensor_mins, max=um)
+    wl_ = torch.clamp(wl, min=tensor_mins, max=lm)
+    wd_ = torch.clamp(wd, min=tensor_mins, max=dm)
+    return wu_, wl_, wd_
+
+
+def xaj_generation(
+    p_and_e: Tensor,
+    k,
+    b,
+    im,
+    um,
+    lm,
+    dm,
+    c,
+    wu0: Tensor = None,
+    wl0: Tensor = None,
+    wd0: Tensor = None,
+) -> tuple:
+    """
+    Single-step runoff generation in XAJ.
+
+    Parameters
+    ----------
+    p_and_e
+        precipitation and potential evapotranspiration (mm/day)
+    k
+        ratio of potential evapotranspiration to reference crop evaporation
+    b
+        exponent parameter
+    um
+        average soil moisture storage capacity of the upper layer (mm)
+    lm
+        average soil moisture storage capacity of the lower layer (mm)
+    dm
+        average soil moisture storage capacity of the deep layer (mm)
+    im
+        impermeability coefficient
+    c
+        coefficient of deep layer
+    wu0
+        initial values of soil moisture in upper layer (mm)
+    wl0
+        initial values of soil moisture in lower layer (mm)
+    wd0
+        initial values of soil moisture in deep layer (mm)
+
+    Returns
+    -------
+    tuple[torch.Tensor]
+        (r, rim, e, pe), (wu, wl, wd)
+    """
+    # make sure physical variables' value ranges are correct
+    prcp = torch.clamp(p_and_e[:, 0], min=0.0)
+    pet = torch.clamp(p_and_e[:, 1] * k, min=0.0)
+    # wm
+    wm = um + lm + dm
+    if wu0 is None:
+        # use detach func to make wu0 no_grad as it is an initial value
+        wu0 = 0.6 * (um.detach())
+    if wl0 is None:
+        wl0 = 0.6 * (lm.detach())
+    if wd0 is None:
+        wd0 = 0.6 * (dm.detach())
+    w0_ = wu0 + wl0 + wd0
+    # w0 need locate in correct range so that following calculation could be right
+    # To make sure the gradient is also not NaN (see case in xaj_sources),
+    # we'd better minus a precision (1e-5), although we've not met this situation (grad is NaN)
+    w0 = torch.clamp(w0_, max=wm - 1e-5)
+
+    # Calculate the amount of evaporation from storage
+    eu, el, ed = calculate_evap(lm, c, wu0, wl0, prcp, pet)
+    e = eu + el + ed
+
+    # Calculate the runoff generated by net precipitation
+    prcp_difference = prcp - e
+    pe = torch.clamp(prcp_difference, min=0.0)
+    r, rim = calculate_prcp_runoff(b, im, wm, w0, pe)
+    # Update wu, wl, wd;
+    # we use prcp_difference rather than pe, as when pe<0 but prcp>0, prcp should be considered
+    wu, wl, wd = calculate_w_storage(
+        um, lm, dm, wu0, wl0, wd0, eu, el, ed, prcp_difference, r
+    )
+
+    return (r, rim, e, pe), (wu, wl, wd)
+
+
+def xaj_sources(
+    pe,
+    r,
+    sm,
+    ex,
+    ki,
+    kg,
+    s0: Optional[Tensor] = None,
+    fr0: Optional[Tensor] = None,
+    book="HF",
+) -> tuple:
+    """
+    Divide the runoff to different sources
+
+    We use the initial version from the paper of the inventor of the XAJ model -- Prof. Renjun Zhao:
+    "Analysis of parameters of the XinAnJiang model". Its Chinese name is <<新安江模型参数的分析>>,
+    which could be found by searching in "Baidu Xueshu".
+    The module's code can also be found in "Watershed Hydrologic Simulation" (WHS) Page 174.
+    It is nearly same with that in "Hydrologic Forecasting" (HF) Page 148-149
+    We use the period average runoff as input and the unit period is day so we don't need to difference it as books show
+
+
+    Parameters
+    ------------
+    pe
+        net precipitation (mm/day)
+    r
+        runoff from xaj_generation (mm/day)
+    sm
+        areal mean free water capacity of the surface layer (mm)
+    ex
+        exponent of the free water capacity curve
+    ki
+        outflow coefficients of the free water storage to interflow relationships
+    kg
+        outflow coefficients of the free water storage to groundwater relationships
+    s0
+        initial free water capacity (mm)
+    fr0
+        runoff area of last period
+
+    Return
+    ------------
+    torch.Tensor
+        rs -- surface runoff; ri-- interflow runoff; rg -- groundwater runoff
+
+    """
+    xaj_device = pe.device
+    # maximum free water storage capacity in a basin
+    ms = sm * (1 + ex)
+    if fr0 is None:
+        fr0 = torch.full(sm.shape[0], 0.1).to(xaj_device)
+    if s0 is None:
+        s0 = 0.5 * (sm.clone().detach())
+    # For free water storage, because s is related to fr and s0 and fr0 are both values of last period,
+    # we have to trans the initial value of s from last period to this one.
+    # both WHS（流域水文模拟）'s sample code and HF（水文预报） use s = fr0 * s0 / fr.
+    # I think they both think free water reservoir as a cubic tank. Its height is s and area of bottom rectangle is fr
+    # we will have a cubic tank with varying bottom and height,
+    # and fixed boundary (in HF sm is fixed) or none-fixed boundary (in EH smmf is not fixed)
+    # but notice r's list like" [1,0] which 1 is the 1st period's runoff and 0 is the 2nd period's runoff
+    # after 1st period, the s1 could not be zero, but in the 2nd period, fr=0, then we cannot set s=0, because some water still in the tank
+    # fr's formula could be found in Eq. 9 in "Analysis of parameters of the XinAnJiang model",
+    # Here our r doesn't include rim, so there is no need to remove rim from r; this is also the method in HF
+    # Moreover, to make sure ss is not larger than sm, otherwise au will be nan value.
+    # It is worth to note that we have to use a precision here -- 1e-5, otherwise the gradient will be NaN;
+    # I guess maybe when calculating gradient -- Δy/Δx, Δ brings some precision problem when we need exponent function.
+
+    # NOTE: when r is 0, fr should be 0, however, s1 may not be zero and it still hold some water,
+    # then fr can not be 0, otherwise when fr is used as denominator it lead to error,
+    # so we have to deal with this case later, for example, when r=0, we cannot use pe * fr to replace r
+    # because fr get the value of last period, and it is not 0
+
+    # cannot use torch.where, because it will cause some error when calculating gradient
+    # fr = torch.where(r > 0.0, r / pe, fr0)
+    # fr just use fr0, and it can be included in the computation graph, so we don't detach it
+    fr = torch.clone(fr0)
+    fr_mask = r > 0.0
+    fr[fr_mask] = r[fr_mask] / pe[fr_mask]
+    if any(torch.isnan(fr)):
+        raise ValueError(
+            "Error: NaN values detected. Try set clamp function or check your data!!!"
+        )
+    if any(fr == 0.0):
+        raise ArithmeticError(
+            "Please check fr's value, fr==0.0 will cause error in the next step!"
+        )
+    ss = torch.clone(s0)
+    s = torch.clone(s0)
+
+    ss[fr_mask] = fr0[fr_mask] * s0[fr_mask] / fr[fr_mask]
+
+    if book == "HF":
+        ss = torch.clamp(ss, max=sm - PRECISION)
+        au = ms * (1.0 - (1.0 - ss / sm) ** (1.0 / (1.0 + ex)))
+        if any(torch.isnan(au)):
+            raise ValueError(
+                "Error: NaN values detected. Try set clamp function or check your data!!!"
+            )
+
+        rs = torch.full_like(r, 0.0, device=xaj_device)
+        rs[fr_mask] = torch.where(
+            pe[fr_mask] + au[fr_mask] < ms[fr_mask],
+            # equation 2-85 in HF
+            # it's weird here, but we have to clamp so that the gradient could be not NaN;
+            # otherwise, even the forward calculation is correct, the gradient is still NaN;
+            # maybe when calculating gradient -- Δy/Δx, Δ brings some precision problem
+            # if we need exponent function.
+            fr[fr_mask]
+            * (
+                pe[fr_mask]
+                - sm[fr_mask]
+                + ss[fr_mask]
+                + sm[fr_mask]
+                * (
+                    (
+                        1
+                        - torch.clamp(pe[fr_mask] + au[fr_mask], max=ms[fr_mask])
+                        / ms[fr_mask]
+                    )
+                    ** (1 + ex[fr_mask])
+                )
+            ),
+            # equation 2-86 in HF
+            fr[fr_mask] * (pe[fr_mask] + ss[fr_mask] - sm[fr_mask]),
+        )
+        rs = torch.clamp(rs, max=r)
+        # ri's mask is not same as rs's, because last period's s may not be 0
+        # and in this time, ri and rg could be larger than 0
+        # we need firstly calculate the updated s, s's mask is same as fr_mask,
+        # when r==0, then s will be equal to last period's
+        # equation 2-87 in HF, some free water leave or save, so we update free water storage
+        s[fr_mask] = ss[fr_mask] + (r[fr_mask] - rs[fr_mask]) / fr[fr_mask]
+        s = torch.clamp(s, max=sm)
+    elif book == "EH":
+        smmf = ms * (1 - (1 - fr) ** (1 / ex))
+        smf = smmf / (1 + ex)
+        ss = torch.clamp(ss, max=smf - PRECISION)
+        au = smmf * (1 - (1 - ss / smf) ** (1 / (1 + ex)))
+        if torch.isnan(au).any():
+            raise ArithmeticError(
+                "Error: NaN values detected. Try set clip function or check your data!!!"
+            )
+        rs = torch.full_like(r, 0.0, device=xaj_device)
+        rs[fr_mask] = torch.where(
+            pe[fr_mask] + au[fr_mask] < smmf[fr_mask],
+            (
+                pe[fr_mask]
+                - smf[fr_mask]
+                + ss[fr_mask]
+                + smf[fr_mask]
+                * (
+                    1
+                    - torch.clamp(
+                        pe[fr_mask] + au[fr_mask],
+                        max=smmf[fr_mask],
+                    )
+                    / smmf[fr_mask]
+                )
+                ** (ex[fr_mask] + 1)
+            )
+            * fr[fr_mask],
+            (pe[fr_mask] + ss[fr_mask] - smf[fr_mask]) * fr[fr_mask],
+        )
+        rs = torch.clamp(rs, max=r)
+        s[fr_mask] = ss[fr_mask] + (r[fr_mask] - rs[fr_mask]) / fr[fr_mask]
+        s[fr_mask] = torch.clamp(s[fr_mask], max=smf[fr_mask])
+        s = torch.clamp(s, max=smf)
+    else:
+        raise ValueError("Please set book as 'HF' or 'EH'!")
+    # equation 2-88 in HF, next interflow and ground water will be released from the updated free water storage
+    # We use the period average runoff as input and the unit period is day.
+    # Hence, we directly use ki and kg rather than ki_{Δt} in books.
+    ri = ki * s * fr
+    rg = kg * s * fr
+    # equation 2-89 in HF; although it looks different with that in WHS, they are actually same
+    # Finally, calculate the final free water storage
+    s1 = s * (1 - ki - kg)
+    return (rs, ri, rg), (s1, fr)
+
+
+def xaj_sources5mm(
+    pe,
+    runoff,
+    sm,
+    ex,
+    ki,
+    kg,
+    s0=None,
+    fr0=None,
+    book="HF",
+):
+    """
+    Divide the runoff to different sources according to books -- 《水文预报》HF 5th edition and 《工程水文学》EH 3rd edition
+
+    Parameters
+    ----------
+    pe
+        net precipitation
+    runoff
+        runoff from xaj_generation
+    sm
+        areal mean free water capacity of the surface layer
+    ex
+        exponent of the free water capacity curve
+    ki
+        outflow coefficients of the free water storage to interflow relationships
+    kg
+        outflow coefficients of the free water storage to groundwater relationships
+    s0
+        initial free water capacity
+    fr0
+        initial area of generation
+    time_interval_hours
+        由于Ki、Kg、Ci、Cg都是以24小时为时段长定义的,需根据时段长转换
+    book
+        the methods in 《水文预报》HF 5th edition and 《工程水文学》EH 3rd edition are different,
+        hence, both are provided, and the default is the former -- "ShuiWenYuBao";
+        the other one is "GongChengShuiWenXue"
+
+    Returns
+    -------
+    tuple[tuple, tuple]
+        rs_s -- surface runoff; rss_s-- interflow runoff; rg_s -- groundwater runoff;
+        (fr_ds[-1], s_ds[-1]): state variables' final value;
+        all variables are numpy array
+    """
+    xaj_device = pe.device
+    # 流域最大点自由水蓄水容量深
+    smm = sm * (1 + ex)
+    if fr0 is None:
+        fr0 = torch.full_like(sm, 0.1, device=xaj_device)
+    if s0 is None:
+        s0 = 0.5 * (sm.clone().detach())
+    fr = torch.clone(fr0)
+    fr_mask = runoff > 0.0
+    fr[fr_mask] = runoff[fr_mask] / pe[fr_mask]
+    if torch.all(runoff < 5):
+        n = 1
+    else:
+        r_max = torch.max(runoff).detach().cpu().numpy()
+        residue_temp = r_max % 5
+        if residue_temp != 0:
+            residue_temp = 1
+        n = int(r_max / 5) + residue_temp
+    rn = runoff / n
+    pen = pe / n
+    kss_d = (1 - (1 - (ki + kg)) ** (1 / n)) / (1 + kg / ki)
+    kg_d = kss_d * kg / ki
+    if torch.isnan(kss_d).any() or torch.isnan(kg_d).any():
+        raise ValueError("Error: NaN values detected. Check your parameters setting!!!")
+    # kss_d = ki
+    # kg_d = kg
+
+    rs = torch.full_like(runoff, 0.0, device=xaj_device)
+    rss = torch.full_like(runoff, 0.0, device=xaj_device)
+    rg = torch.full_like(runoff, 0.0, device=xaj_device)
+
+    s_ds = []
+    fr_ds = []
+    s_ds.append(s0)
+    fr_ds.append(fr0)
+    for j in range(n):
+        fr0_d = fr_ds[j]
+        s0_d = s_ds[j]
+        # equation 5-32 in HF, but strange, cause each period, rn/pen is same
+        # fr_d = torch.full_like(fr0_d, PRECISION, device=xaj_device)
+        # fr_d_mask = fr > PRECISION
+        # fr_d[fr_d_mask] = 1 - (1 - fr[fr_d_mask]) ** (1 / n)
+        fr_d = fr
+
+        ss_d = torch.clone(s0_d)
+        s_d = torch.clone(s0_d)
+
+        ss_d[fr_mask] = fr0_d[fr_mask] * s0_d[fr_mask] / fr_d[fr_mask]
+
+        if book == "HF":
+            # ms = smm
+            ss_d = torch.clamp(ss_d, max=sm - PRECISION)
+            au = smm * (1.0 - (1.0 - ss_d / sm) ** (1.0 / (1.0 + ex)))
+            if torch.isnan(au).any():
+                raise ValueError(
+                    "Error: NaN values detected. Try set clip function or check your data!!!"
+                )
+            rs_j = torch.full_like(rn, 0.0, device=xaj_device)
+            rs_j[fr_mask] = torch.where(
+                pen[fr_mask] + au[fr_mask] < smm[fr_mask],
+                # equation 5-26 in HF
+                fr_d[fr_mask]
+                * (
+                    pen[fr_mask]
+                    - sm[fr_mask]
+                    + ss_d[fr_mask]
+                    + sm[fr_mask]
+                    * (
+                        (
+                            1
+                            - torch.clamp(pen[fr_mask] + au[fr_mask], max=smm[fr_mask])
+                            / smm[fr_mask]
+                        )
+                        ** (1 + ex[fr_mask])
+                    )
+                ),
+                # equation 5-27 in HF
+                fr_d[fr_mask] * (pen[fr_mask] + ss_d[fr_mask] - sm[fr_mask]),
+            )
+            rs_j = torch.clamp(rs_j, max=rn)
+            s_d[fr_mask] = ss_d[fr_mask] + (rn[fr_mask] - rs_j[fr_mask]) / fr_d[fr_mask]
+            s_d = torch.clamp(s_d, max=sm)
+
+        elif book == "EH":
+            smmf = smm * (1 - (1 - fr_d) ** (1 / ex))
+            smf = smmf / (1 + ex)
+            ss_d = torch.clamp(ss_d, max=smf - PRECISION)
+            au = smmf * (1 - (1 - ss_d / smf) ** (1 / (1 + ex)))
+            if torch.isnan(au).any():
+                raise ValueError(
+                    "Error: NaN values detected. Try set clip function or check your data!!!"
+                )
+            rs_j = torch.full(rn.size(), 0.0).to(xaj_device)
+            rs_j[fr_mask] = torch.where(
+                pen[fr_mask] + au[fr_mask] < smmf[fr_mask],
+                (
+                    pen[fr_mask]
+                    - smf[fr_mask]
+                    + ss_d[fr_mask]
+                    + smf[fr_mask]
+                    * (
+                        1
+                        - torch.clamp(
+                            pen[fr_mask] + au[fr_mask],
+                            max=smmf[fr_mask],
+                        )
+                        / smmf[fr_mask]
+                    )
+                    ** (ex[fr_mask] + 1)
+                )
+                * fr_d[fr_mask],
+                (pen[fr_mask] + ss_d[fr_mask] - smf[fr_mask]) * fr_d[fr_mask],
+            )
+            rs_j = torch.clamp(rs_j, max=rn)
+            s_d[fr_mask] = ss_d[fr_mask] + (rn[fr_mask] - rs_j[fr_mask]) / fr_d[fr_mask]
+            s_d = torch.clamp(s_d, max=smf)
+        else:
+            raise NotImplementedError(
+                "We don't have this implementation! Please chose 'HF' or 'EH'!!"
+            )
+
+        rss_j = s_d * kss_d * fr_d
+        rg_j = s_d * kg_d * fr_d
+        s1_d = s_d * (1 - kss_d - kg_d)
+
+        rs = rs + rs_j
+        rss = rss + rss_j
+        rg = rg + rg_j
+        # 赋值s_d和fr_d到数组中，以给下一段做初值
+        s_ds.append(s1_d)
+        fr_ds.append(fr_d)
+
+    return (rs, rss, rg), (s_ds[-1], fr_ds[-1])
+
+
+def linear_reservoir(x, weight, last_y: Optional[Tensor] = None):
+    """
+    Linear reservoir's release function
+
+    Parameters
+    ----------
+    x
+        the input to the linear reservoir
+    weight
+        the coefficient of linear reservoir
+    last_y
+        the output of last period
+
+    Returns
+    -------
+    torch.Tensor
+        one-step forward result
+    """
+    weight1 = 1 - weight
+    if last_y is None:
+        last_y = torch.full(weight.size(), 0.001).to(x.device)
+    y = weight * last_y + weight1 * x
+    return y
+
+
+class Xaj4Dpl(nn.Module):
+    """
+    XAJ model for Differential Parameter learning
+    """
+
+    def __init__(
+        self,
+        kernel_size: int,
+        warmup_length: int,
+        source_book="HF",
+        source_type="sources",
+    ):
+        """
+        Parameters
+        ----------
+        kernel_size
+            the time length of unit hydrograph
+        warmup_length
+            the length of warmup periods;
+            XAJ needs a warmup period to generate reasonable initial state values
+        """
+        super(Xaj4Dpl, self).__init__()
+        self.params_names = MODEL_PARAM_DICT["xaj_mz"]["param_name"]
+        param_range = MODEL_PARAM_DICT["xaj_mz"]["param_range"]
+        self.k_scale = param_range["K"]
+        self.b_scale = param_range["B"]
+        self.im_sacle = param_range["IM"]
+        self.um_scale = param_range["UM"]
+        self.lm_scale = param_range["LM"]
+        self.dm_scale = param_range["DM"]
+        self.c_scale = param_range["C"]
+        self.sm_scale = param_range["SM"]
+        self.ex_scale = param_range["EX"]
+        self.ki_scale = param_range["KI"]
+        self.kg_scale = param_range["KG"]
+        self.a_scale = param_range["A"]
+        self.theta_scale = param_range["THETA"]
+        self.ci_scale = param_range["CI"]
+        self.cg_scale = param_range["CG"]
+        self.kernel_size = kernel_size
+        self.warmup_length = warmup_length
+        # there are 2 input variables in XAJ: P and PET
+        self.feature_size = 2
+        self.source_book = source_book
+        self.source_type = source_type
+
+    def forward(self, p_and_e, parameters, return_state=False):
+        """
+        run XAJ model
+
+        Parameters
+        ----------
+        p_and_e
+            precipitation and potential evapotranspiration
+        parameters
+            parameters of XAJ model
+        return_state
+            if True, return state values, mainly for warmup periods
+
+        Returns
+        -------
+        torch.Tensor
+            streamflow got by XAJ
+        """
+        xaj_device = p_and_e.device
+        # denormalize the parameters to general range
+        k = self.k_scale[0] + parameters[:, 0] * (self.k_scale[1] - self.k_scale[0])
+        b = self.b_scale[0] + parameters[:, 1] * (self.b_scale[1] - self.b_scale[0])
+        im = self.im_sacle[0] + parameters[:, 2] * (self.im_sacle[1] - self.im_sacle[0])
+        um = self.um_scale[0] + parameters[:, 3] * (self.um_scale[1] - self.um_scale[0])
+        lm = self.lm_scale[0] + parameters[:, 4] * (self.lm_scale[1] - self.lm_scale[0])
+        dm = self.dm_scale[0] + parameters[:, 5] * (self.dm_scale[1] - self.dm_scale[0])
+        c = self.c_scale[0] + parameters[:, 6] * (self.c_scale[1] - self.c_scale[0])
+        sm = self.sm_scale[0] + parameters[:, 7] * (self.sm_scale[1] - self.sm_scale[0])
+        ex = self.ex_scale[0] + parameters[:, 8] * (self.ex_scale[1] - self.ex_scale[0])
+        ki_ = self.ki_scale[0] + parameters[:, 9] * (
+            self.ki_scale[1] - self.ki_scale[0]
+        )
+        kg_ = self.kg_scale[0] + parameters[:, 10] * (
+            self.kg_scale[1] - self.kg_scale[0]
+        )
+        # ki+kg should be smaller than 1; if not, we scale them, but note float only contain 4 digits, so we need 0.999
+        ki = torch.where(
+            ki_ + kg_ < 1.0,
+            ki_,
+            (1 - PRECISION) / (ki_ + kg_) * ki_,
+        )
+        kg = torch.where(
+            ki_ + kg_ < 1.0,
+            kg_,
+            (1 - PRECISION) / (ki_ + kg_) * kg_,
+        )
+        a = self.a_scale[0] + parameters[:, 11] * (self.a_scale[1] - self.a_scale[0])
+        theta = self.theta_scale[0] + parameters[:, 12] * (
+            self.theta_scale[1] - self.theta_scale[0]
+        )
+        ci = self.ci_scale[0] + parameters[:, 13] * (
+            self.ci_scale[1] - self.ci_scale[0]
+        )
+        cg = self.cg_scale[0] + parameters[:, 14] * (
+            self.cg_scale[1] - self.cg_scale[0]
+        )
+
+        # initialize state values
+        warmup_length = self.warmup_length
+        if warmup_length > 0:
+            # set no_grad for warmup periods
+            with torch.no_grad():
+                p_and_e_warmup = p_and_e[0:warmup_length, :, :]
+                cal_init_xaj4dpl = Xaj4Dpl(
+                    self.kernel_size, 0, self.source_book, self.source_type
+                )
+                if cal_init_xaj4dpl.warmup_length > 0:
+                    raise RuntimeError("Please set init model's warmup length to 0!!!")
+                _, _, *w0, s0, fr0, qi0, qg0 = cal_init_xaj4dpl(
+                    p_and_e_warmup, parameters, return_state=True
+                )
+        else:
+            # use detach func to make wu0 no_grad as it is an initial value
+            w0 = (0.5 * (um.detach()), 0.5 * (lm.detach()), 0.5 * (dm.detach()))
+            s0 = 0.5 * (sm.detach())
+            fr0 = torch.full(ci.size(), 0.1).to(xaj_device)
+            qi0 = torch.full(ci.size(), 0.1).to(xaj_device)
+            qg0 = torch.full(cg.size(), 0.1).to(xaj_device)
+
+        inputs = p_and_e[warmup_length:, :, :]
+        runoff_ims_ = torch.full(inputs.shape[:2], 0.0).to(xaj_device)
+        rss_ = torch.full(inputs.shape[:2], 0.0).to(xaj_device)
+        ris_ = torch.full(inputs.shape[:2], 0.0).to(xaj_device)
+        rgs_ = torch.full(inputs.shape[:2], 0.0).to(xaj_device)
+        es_ = torch.full(inputs.shape[:2], 0.0).to(xaj_device)
+        for i in range(inputs.shape[0]):
+            if i == 0:
+                (r, rim, e, pe), w = xaj_generation(
+                    inputs[i, :, :], k, b, im, um, lm, dm, c, *w0
+                )
+                if self.source_type == "sources":
+                    (rs, ri, rg), (s, fr) = xaj_sources(
+                        pe, r, sm, ex, ki, kg, s0, fr0, book=self.source_book
+                    )
+                elif self.source_type == "sources5mm":
+                    (rs, ri, rg), (s, fr) = xaj_sources5mm(
+                        pe, r, sm, ex, ki, kg, s0, fr0, book=self.source_book
+                    )
+                else:
+                    raise NotImplementedError("No such divide-sources method")
+            else:
+                (r, rim, e, pe), w = xaj_generation(
+                    inputs[i, :, :], k, b, im, um, lm, dm, c, *w
+                )
+                if self.source_type == "sources":
+                    (rs, ri, rg), (s, fr) = xaj_sources(
+                        pe, r, sm, ex, ki, kg, s, fr, book=self.source_book
+                    )
+                elif self.source_type == "sources5mm":
+                    (rs, ri, rg), (s, fr) = xaj_sources5mm(
+                        pe, r, sm, ex, ki, kg, s, fr, book=self.source_book
+                    )
+                else:
+                    raise NotImplementedError("No such divide-sources method")
+            # impevious part is pe * im
+            runoff_ims_[i, :] = rim
+            # so for non-imprvious part, the result should be corrected
+            rss_[i, :] = rs * (1 - im)
+            ris_[i, :] = ri * (1 - im)
+            rgs_[i, :] = rg * (1 - im)
+            es_[i, :] = e
+            # rss_[i, :] = 0.7 * r
+            # ris_[i, :] = 0.2 * r
+            # rgs_[i, :] = 0.1 * r
+        # seq, batch, feature
+        runoff_im = torch.unsqueeze(runoff_ims_, dim=2)
+        rss = torch.unsqueeze(rss_, dim=2)
+        es = torch.unsqueeze(es_, dim=2)
+
+        conv_uh = KernelConv(a, theta, self.kernel_size)
+        qs_ = conv_uh(runoff_im + rss)
+        qs = torch.full(inputs.shape[:2], 0.0).to(xaj_device)
+        for i in range(inputs.shape[0]):
+            if i == 0:
+                qi = linear_reservoir(ris_[i], ci, qi0)
+                qg = linear_reservoir(rgs_[i], cg, qg0)
+            else:
+                qi = linear_reservoir(ris_[i], ci, qi)
+                qg = linear_reservoir(rgs_[i], cg, qg)
+            qs[i, :] = qs_[i, :, 0] + qi + qg
+        # seq, batch, feature
+        q_sim = torch.unsqueeze(qs, dim=2)
+        if return_state:
+            return q_sim, es, *w, s, fr, qi, qg
+        return q_sim, es
+
+
+class DplLstmXaj(nn.Module):
+    def __init__(
+        self,
+        n_input_features,
+        n_output_features,
+        n_hidden_states,
+        kernel_size,
+        warmup_length,
+        param_limit_func="sigmoid",
+        param_test_way="final",
+        source_book="HF",
+        source_type="sources",
+    ):
+        """
+        Differential Parameter learning model: LSTM -> Param -> XAJ
+
+        The principle can be seen here: https://doi.org/10.1038/s41467-021-26107-z
+
+        Parameters
+        ----------
+        n_input_features
+            the number of input features of LSTM
+        n_output_features
+            the number of output features of LSTM, and it should be equal to the number of learning parameters in XAJ
+        n_hidden_states
+            the number of hidden features of LSTM
+        kernel_size
+            the time length of unit hydrograph
+        warmup_length
+            the length of warmup periods;
+            hydrologic models need a warmup period to generate reasonable initial state values
+        param_limit_func
+            function used to limit the range of params; now it is sigmoid or clamp function
+        param_test_way
+            how we use parameters from dl model when testing;
+            now we have three ways:
+            1. "final" -- use the final period's parameter for each period
+            2. "mean_time" -- Mean values of all periods' parameters is used
+            3. "mean_basin" -- Mean values of all basins' final periods' parameters is used
+        """
+        super(DplLstmXaj, self).__init__()
+        self.dl_model = SimpleLSTM(n_input_features, n_output_features, n_hidden_states)
+        self.pb_model = Xaj4Dpl(
+            kernel_size, warmup_length, source_book=source_book, source_type=source_type
+        )
+        self.param_func = param_limit_func
+        self.param_test_way = param_test_way
+
+    def forward(self, x, z):
+        """
+        Differential parameter learning
+
+        z (normalized input) -> lstm -> param -> + x (not normalized) -> xaj -> q
+        Parameters will be denormalized in xaj model
+
+        Parameters
+        ----------
+        x
+            not normalized data used for physical model; a sequence-first 3-dim tensor. [sequence, batch, feature]
+        z
+            normalized data used for DL model; a sequence-first 3-dim tensor. [sequence, batch, feature]
+
+        Returns
+        -------
+        torch.Tensor
+            one time forward result
+        """
+        q, e = lstm_pbm(self.dl_model, self.pb_model, self.param_func, x, z)
+        return q
+
+
+class DplAnnXaj(nn.Module):
+    def __init__(
+        self,
+        n_input_features: int,
+        n_output_features: int,
+        n_hidden_states: Union[int, tuple, list],
+        dr: Union[int, tuple, list],
+        kernel_size: int,
+        warmup_length: int,
+        param_limit_func="sigmoid",
+        param_test_way="final",
+        source_book="HF",
+        source_type="sources",
+    ):
+        """
+        Differential Parameter learning model only with attributes as DL model's input: ANN -> Param -> Gr4j
+
+        The principle can be seen here: https://doi.org/10.1038/s41467-021-26107-z
+
+        Parameters
+        ----------
+        n_input_features
+            the number of input features of ANN
+        n_output_features
+            the number of output features of ANN, and it should be equal to the number of learning parameters in XAJ
+        n_hidden_states
+            the number of hidden features of ANN; it could be Union[int, tuple, list]
+        kernel_size
+            the time length of unit hydrograph
+        warmup_length
+            the length of warmup periods;
+            hydrologic models need a warmup period to generate reasonable initial state values
+        param_limit_func
+            function used to limit the range of params; now it is sigmoid or clamp function
+        param_test_way
+            how we use parameters from dl model when testing;
+            now we have three ways:
+            1. "final" -- use the final period's parameter for each period
+            2. "mean_time" -- Mean values of all periods' parameters is used
+            3. "mean_basin" -- Mean values of all basins' final periods' parameters is used
+        """
+        super(DplAnnXaj, self).__init__()
+        self.dl_model = SimpleAnn(
+            n_input_features, n_output_features, n_hidden_states, dr
+        )
+        self.pb_model = Xaj4Dpl(
+            kernel_size, warmup_length, source_book=source_book, source_type=source_type
+        )
+        self.param_func = param_limit_func
+        self.param_test_way = param_test_way
+
+    def forward(self, x, z):
+        """
+        Differential parameter learning
+
+        z (normalized input) -> ANN -> param -> + x (not normalized) -> gr4j -> q
+        Parameters will be denormalized in gr4j model
+
+        Parameters
+        ----------
+        x
+            not normalized data used for physical model; a sequence-first 3-dim tensor. [sequence, batch, feature]
+        z
+            normalized data used for DL model; a 2-dim tensor. [batch, feature]
+
+        Returns
+        -------
+        torch.Tensor
+            one time forward result
+        """
+        q, e = ann_pbm(self.dl_model, self.pb_model, self.param_func, x, z)
+        return q
+
+
+def lstm_pbm(dl_model, pb_model, param_func, x, z):
+    """
+    Differential parameter learning
+
+    z (normalized input) -> lstm -> param -> + x (not normalized) -> pbm -> q
+    Parameters will be denormalized in pbm model
+
+    Parameters
+    ----------
+    dl_model
+        lstm model
+    pb_model
+        physics-based model
+    param_func
+        function used to limit the range of params; now it is sigmoid or clamp function
+    x
+        not normalized data used for physical model; a sequence-first 3-dim tensor. [sequence, batch, feature]
+    z
+        normalized data used for DL model; a sequence-first 3-dim tensor. [sequence, batch, feature]
+
+    Returns
+    -------
+    torch.Tensor
+            one time forward result
+    """
+    gen = dl_model(z)
+    if torch.isnan(gen).any():
+        raise ValueError("Error: NaN values detected. Check your data firstly!!!")
+    # we set all params' values in [0, 1] and will scale them when forwarding
+    if param_func == "sigmoid":
+        params_ = F.sigmoid(gen)
+    elif param_func == "clamp":
+        params_ = torch.clamp(gen, min=0.0, max=1.0)
+    else:
+        raise NotImplementedError(
+            "We don't provide this way to limit parameters' range!! Please choose sigmoid or clamp"
+        )
+    # just get one-period values, here we use the final period's values
+    params = params_[-1, :, :]
+    return pb_model(x[:, :, : pb_model.feature_size], params)
+
+
+def ann_pbm(dl_model, pb_model, param_func, x, z):
+    """
+    Differential parameter learning
+
+    z (normalized input) -> ann -> param -> + x (not normalized) -> pbm -> q
+    Parameters will be denormalized in pbm model
+
+    Parameters
+    ----------
+    dl_model
+        ann model
+    pb_model
+        physics-based model
+    param_func
+        function used to limit the range of params; now it is sigmoid or clamp function
+    x
+        not normalized data used for physical model; a sequence-first 3-dim tensor. [sequence, batch, feature]
+    z
+        normalized data used for DL model; a 2-dim tensor. [batch, feature]
+
+    Returns
+    -------
+    torch.Tensor
+        one time forward result
+    """
+    gen = dl_model(z)
+    if torch.isnan(gen).any():
+        raise ValueError("Error: NaN values detected. Check your data firstly!!!")
+    # we set all params' values in [0, 1] and will scale them when forwarding
+    if param_func == "sigmoid":
+        params = F.sigmoid(gen)
+    elif param_func == "clamp":
+        params = torch.clamp(gen, min=0.0, max=1.0)
+    else:
+        raise NotImplementedError(
+            "We don't provide this way to limit parameters' range!! Please choose sigmoid or clamp"
+        )
+    return pb_model(x[:, :, : pb_model.feature_size], params)
```

### Comparing `torchhydro-0.0.4/torchhydro/models/dropout.py` & `torchhydro-0.0.5/torchhydro/models/dropout.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-"""
-Author: Wenyu Ouyang
-Date: 2023-07-11 17:39:09
-LastEditTime: 2023-10-06 18:12:54
-LastEditors: Wenyu Ouyang
-Description: Functions for dropout. Code is from Kuai Fang's repo: hydroDL
-FilePath: \torchhydro\torchhydro\models\dropout.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-import torch.nn
-
-
-def create_mask(x, dr):
-    """
-    Dropout method in Gal & Ghahramami: A Theoretically Grounded Application of Dropout in RNNs.
-    http://papers.nips.cc/paper/6241-a-theoretically-grounded-application-of-dropout-in-recurrent-neural-networks.pdf
-
-    Parameters
-    ----------
-    x
-    dr
-
-    Returns
-    -------
-
-    """
-    return x.new().resize_as_(x).bernoulli_(1 - dr).div_(1 - dr).detach_()
-
-
-class DropMask(torch.autograd.function.InplaceFunction):
-    @classmethod
-    def forward(cls, ctx, input, mask, train=False, inplace=False):
-        ctx.master_train = train
-        ctx.inplace = inplace
-        ctx.mask = mask
-
-        if not ctx.master_train:
-            return input
-        if ctx.inplace:
-            ctx.mark_dirty(input)
-            output = input
-        else:
-            output = input.clone()
-        output.mul_(ctx.mask)
-
-        return output
-
-    @staticmethod
-    def backward(ctx, grad_output):
-        if ctx.master_train:
-            return grad_output * ctx.mask, None, None, None
-        else:
-            return grad_output, None, None, None
+"""
+Author: Wenyu Ouyang
+Date: 2023-07-11 17:39:09
+LastEditTime: 2023-10-06 18:12:54
+LastEditors: Wenyu Ouyang
+Description: Functions for dropout. Code is from Kuai Fang's repo: hydroDL
+FilePath: \torchhydro\torchhydro\models\dropout.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+import torch.nn
+
+
+def create_mask(x, dr):
+    """
+    Dropout method in Gal & Ghahramami: A Theoretically Grounded Application of Dropout in RNNs.
+    http://papers.nips.cc/paper/6241-a-theoretically-grounded-application-of-dropout-in-recurrent-neural-networks.pdf
+
+    Parameters
+    ----------
+    x
+    dr
+
+    Returns
+    -------
+
+    """
+    return x.new().resize_as_(x).bernoulli_(1 - dr).div_(1 - dr).detach_()
+
+
+class DropMask(torch.autograd.function.InplaceFunction):
+    @classmethod
+    def forward(cls, ctx, input, mask, train=False, inplace=False):
+        ctx.master_train = train
+        ctx.inplace = inplace
+        ctx.mask = mask
+
+        if not ctx.master_train:
+            return input
+        if ctx.inplace:
+            ctx.mark_dirty(input)
+            output = input
+        else:
+            output = input.clone()
+        output.mul_(ctx.mask)
+
+        return output
+
+    @staticmethod
+    def backward(ctx, grad_output):
+        if ctx.master_train:
+            return grad_output * ctx.mask, None, None, None
+        else:
+            return grad_output, None, None, None
```

### Comparing `torchhydro-0.0.4/torchhydro/models/kernel_conv.py` & `torchhydro-0.0.5/torchhydro/models/kernel_conv.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-import torch.nn as nn
-import torch
-from torch.nn import functional as F
-
-
-class KernelConv(nn.Module):
-    def __init__(self, a, theta, kernel_size):
-        """
-        The convolution kernel for the convolution operation in routing module
-
-        We use two-parameter gamma distribution to determine the unit hydrograph,
-        which comes from [mizuRoute](http://www.geosci-model-dev.net/9/2223/2016/)
-
-        Parameters
-        ----------
-        a
-            shape parameter
-        theta
-            timescale parameter
-        kernel_size
-            the size of conv kernel
-        """
-        super(KernelConv, self).__init__()
-        self.a = a
-        self.theta = theta
-        routa = self.a.repeat(kernel_size, 1).unsqueeze(-1)
-        routb = self.theta.repeat(kernel_size, 1).unsqueeze(-1)
-        self.uh_gamma = uh_gamma(routa, routb, len_uh=kernel_size)
-
-    def forward(self, x):
-        """
-        1d-convolution calculation
-
-        Parameters
-        ----------
-        x
-            x is a sequence-first variable, so the dim of x is [seq, batch, feature]
-
-        Returns
-        -------
-        torch.Tensor
-            convolution
-        """
-        # dim: permute from [len_uh, batch, feature] to [batch, feature, len_uh]
-        uh = self.uh_gamma.permute(1, 2, 0)
-        # the dim of conv kernel in F.conv1d is out_channels, in_channels (feature)/groups, width (seq)
-        # the dim of inputs in F.conv1d are batch, in_channels (feature) and width (seq),
-        # each element in a batch should has its own conv kernel,
-        # hence set groups = batch_size and permute input's batch-dim to channel-dim to make "groups" work
-        inputs = x.permute(2, 1, 0)
-        batch_size = x.shape[1]
-        # conv1d in NN is different from the general convolution: it is lack of a flip
-        outputs = F.conv1d(
-            inputs, torch.flip(uh, [2]), groups=batch_size, padding=uh.shape[-1] - 1
-        )
-        # permute from [feature, batch, seq] to [seq, batch, feature]
-        return outputs[:, :, : -(uh.shape[-1] - 1)].permute(2, 1, 0)
-
-
-def uh_conv(x, uh_made) -> torch.Tensor:
-    """
-    Function for 1d-convolution calculation
-
-    Parameters
-    ----------
-    x
-        x is a sequence-first variable, so the dim of x is [seq, batch, feature]
-    uh_made
-        unit hydrograph from uh_gamma or other unit-hydrograph method
-
-    Returns
-    -------
-    torch.Tensor
-        convolution, [seq, batch, feature]; the length of seq is same as x's
-    """
-    uh = uh_made.permute(1, 2, 0)
-    # the dim of conv kernel in F.conv1d is out_channels, in_channels (feature)/groups, width (seq)
-    # the dim of inputs in F.conv1d are batch, in_channels (feature) and width (seq),
-    # each element in a batch should has its own conv kernel,
-    # hence set groups = batch_size and permute input's batch-dim to channel-dim to make "groups" work
-    inputs = x.permute(2, 1, 0)
-    batch_size = x.shape[1]
-    # conv1d in NN is different from the general convolution: it is lack of a flip
-    outputs = F.conv1d(
-        inputs, torch.flip(uh, [2]), groups=batch_size, padding=uh.shape[-1] - 1
-    )
-    # cut to same shape with x and permute from [feature, batch, seq] to [seq, batch, feature]
-    return outputs[:, :, : x.shape[0]].permute(2, 1, 0)
-
-
-def uh_gamma(a, theta, len_uh=10):
-    """
-    A simple two-parameter Gamma distribution as a unit-hydrograph to route instantaneous runoff from a hydrologic model
-
-    The method comes from mizuRoute -- http://www.geosci-model-dev.net/9/2223/2016/
-
-    Parameters
-    ----------
-    a
-        shape parameter
-    theta
-        timescale parameter
-    len_uh
-        the time length of the unit hydrograph
-
-    Returns
-    -------
-    torch.Tensor
-        the unit hydrograph, dim: [seq, batch, feature]
-
-    """
-    # dims of a: time_seq (same all time steps), batch, feature=1
-    m = a.shape
-    assert len_uh <= m[0]
-    # aa > 0, here we set minimum 0.1 (min of a is 0, set when calling this func); First dimension of a is repeat
-    aa = F.relu(a[0:len_uh, :, :]) + 0.1
-    # theta > 0, here set minimum 0.5
-    theta = F.relu(theta[0:len_uh, :, :]) + 0.5
-    # len_f, batch, feature
-    t = (
-        torch.arange(0.5, len_uh * 1.0)
-        .view([len_uh, 1, 1])
-        .repeat([1, m[1], m[2]])
-        .to(aa.device)
-    )
-    denominator = (aa.lgamma().exp()) * (theta**aa)
-    # [len_f, m[1], m[2]]
-    w = 1 / denominator * (t ** (aa - 1)) * (torch.exp(-t / theta))
-    w = w / w.sum(0)  # scale to 1 for each UH
-    return w
+import torch.nn as nn
+import torch
+from torch.nn import functional as F
+
+
+class KernelConv(nn.Module):
+    def __init__(self, a, theta, kernel_size):
+        """
+        The convolution kernel for the convolution operation in routing module
+
+        We use two-parameter gamma distribution to determine the unit hydrograph,
+        which comes from [mizuRoute](http://www.geosci-model-dev.net/9/2223/2016/)
+
+        Parameters
+        ----------
+        a
+            shape parameter
+        theta
+            timescale parameter
+        kernel_size
+            the size of conv kernel
+        """
+        super(KernelConv, self).__init__()
+        self.a = a
+        self.theta = theta
+        routa = self.a.repeat(kernel_size, 1).unsqueeze(-1)
+        routb = self.theta.repeat(kernel_size, 1).unsqueeze(-1)
+        self.uh_gamma = uh_gamma(routa, routb, len_uh=kernel_size)
+
+    def forward(self, x):
+        """
+        1d-convolution calculation
+
+        Parameters
+        ----------
+        x
+            x is a sequence-first variable, so the dim of x is [seq, batch, feature]
+
+        Returns
+        -------
+        torch.Tensor
+            convolution
+        """
+        # dim: permute from [len_uh, batch, feature] to [batch, feature, len_uh]
+        uh = self.uh_gamma.permute(1, 2, 0)
+        # the dim of conv kernel in F.conv1d is out_channels, in_channels (feature)/groups, width (seq)
+        # the dim of inputs in F.conv1d are batch, in_channels (feature) and width (seq),
+        # each element in a batch should has its own conv kernel,
+        # hence set groups = batch_size and permute input's batch-dim to channel-dim to make "groups" work
+        inputs = x.permute(2, 1, 0)
+        batch_size = x.shape[1]
+        # conv1d in NN is different from the general convolution: it is lack of a flip
+        outputs = F.conv1d(
+            inputs, torch.flip(uh, [2]), groups=batch_size, padding=uh.shape[-1] - 1
+        )
+        # permute from [feature, batch, seq] to [seq, batch, feature]
+        return outputs[:, :, : -(uh.shape[-1] - 1)].permute(2, 1, 0)
+
+
+def uh_conv(x, uh_made) -> torch.Tensor:
+    """
+    Function for 1d-convolution calculation
+
+    Parameters
+    ----------
+    x
+        x is a sequence-first variable, so the dim of x is [seq, batch, feature]
+    uh_made
+        unit hydrograph from uh_gamma or other unit-hydrograph method
+
+    Returns
+    -------
+    torch.Tensor
+        convolution, [seq, batch, feature]; the length of seq is same as x's
+    """
+    uh = uh_made.permute(1, 2, 0)
+    # the dim of conv kernel in F.conv1d is out_channels, in_channels (feature)/groups, width (seq)
+    # the dim of inputs in F.conv1d are batch, in_channels (feature) and width (seq),
+    # each element in a batch should has its own conv kernel,
+    # hence set groups = batch_size and permute input's batch-dim to channel-dim to make "groups" work
+    inputs = x.permute(2, 1, 0)
+    batch_size = x.shape[1]
+    # conv1d in NN is different from the general convolution: it is lack of a flip
+    outputs = F.conv1d(
+        inputs, torch.flip(uh, [2]), groups=batch_size, padding=uh.shape[-1] - 1
+    )
+    # cut to same shape with x and permute from [feature, batch, seq] to [seq, batch, feature]
+    return outputs[:, :, : x.shape[0]].permute(2, 1, 0)
+
+
+def uh_gamma(a, theta, len_uh=10):
+    """
+    A simple two-parameter Gamma distribution as a unit-hydrograph to route instantaneous runoff from a hydrologic model
+
+    The method comes from mizuRoute -- http://www.geosci-model-dev.net/9/2223/2016/
+
+    Parameters
+    ----------
+    a
+        shape parameter
+    theta
+        timescale parameter
+    len_uh
+        the time length of the unit hydrograph
+
+    Returns
+    -------
+    torch.Tensor
+        the unit hydrograph, dim: [seq, batch, feature]
+
+    """
+    # dims of a: time_seq (same all time steps), batch, feature=1
+    m = a.shape
+    assert len_uh <= m[0]
+    # aa > 0, here we set minimum 0.1 (min of a is 0, set when calling this func); First dimension of a is repeat
+    aa = F.relu(a[0:len_uh, :, :]) + 0.1
+    # theta > 0, here set minimum 0.5
+    theta = F.relu(theta[0:len_uh, :, :]) + 0.5
+    # len_f, batch, feature
+    t = (
+        torch.arange(0.5, len_uh * 1.0)
+        .view([len_uh, 1, 1])
+        .repeat([1, m[1], m[2]])
+        .to(aa.device)
+    )
+    denominator = (aa.lgamma().exp()) * (theta**aa)
+    # [len_f, m[1], m[2]]
+    w = 1 / denominator * (t ** (aa - 1)) * (torch.exp(-t / theta))
+    w = w / w.sum(0)  # scale to 1 for each UH
+    return w
```

### Comparing `torchhydro-0.0.4/torchhydro/models/model_utils.py` & `torchhydro-0.0.5/torchhydro/models/model_utils.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-"""
-Author: Wenyu Ouyang
-Date: 2021-08-09 10:19:13
-LastEditTime: 2023-09-21 16:47:05
-LastEditors: Wenyu Ouyang
-Description: Some util functions for modeling
-FilePath: /torchhydro/torchhydro/models/model_utils.py
-Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
-"""
-
-from typing import Union
-import warnings
-import torch
-
-
-def get_the_device(device_num: Union[list, int]):
-    """
-    Get device for torch according to its name
-
-    Parameters
-    ----------
-    device_num : Union[list, int]
-        number of the device -- -1 means "cpu" or 0, 1, ... means "cuda:x"
-    """
-    if device_num in [[-1], -1, ["-1"]]:
-        return torch.device("cpu")
-    if torch.cuda.is_available():
-        return (
-            torch.device(f"cuda:{str(device_num)}")
-            if type(device_num) is not list
-            else torch.device(f"cuda:{str(device_num[0])}")
-        )
-    if device_num not in [[-1], -1, ["-1"]]:
-        warnings.warn("You don't have GPU, so have to choose cpu for models")
-    return torch.device("cpu")
+"""
+Author: Wenyu Ouyang
+Date: 2021-08-09 10:19:13
+LastEditTime: 2023-09-21 16:47:05
+LastEditors: Wenyu Ouyang
+Description: Some util functions for modeling
+FilePath: /torchhydro/torchhydro/models/model_utils.py
+Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
+"""
+
+from typing import Union
+import warnings
+import torch
+
+
+def get_the_device(device_num: Union[list, int]):
+    """
+    Get device for torch according to its name
+
+    Parameters
+    ----------
+    device_num : Union[list, int]
+        number of the device -- -1 means "cpu" or 0, 1, ... means "cuda:x"
+    """
+    if device_num in [[-1], -1, ["-1"]]:
+        return torch.device("cpu")
+    if torch.cuda.is_available():
+        return (
+            torch.device(f"cuda:{str(device_num)}")
+            if type(device_num) is not list
+            else torch.device(f"cuda:{str(device_num[0])}")
+        )
+    if device_num not in [[-1], -1, ["-1"]]:
+        warnings.warn("You don't have GPU, so have to choose cpu for models")
+    return torch.device("cpu")
```

### Comparing `torchhydro-0.0.4/torchhydro/models/simple_lstm.py` & `torchhydro-0.0.5/torchhydro/models/simple_lstm.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,104 +1,119 @@
-"""
-Author: Wenyu Ouyang
-Date: 2023-09-19 09:36:25
-LastEditTime: 2023-11-29 11:34:29
-LastEditors: Wenyu Ouyang
-Description: 
-FilePath: \torchhydro\torchhydro\models\simple_lstm.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-import math
-import torch as th
-import torch.nn as nn
-from torch.nn import functional as F
-from torch import Tensor as T
-from torch.nn import Parameter as P
-
-
-class SimpleLSTM(nn.Module):
-    def __init__(self, input_size, output_size, hidden_size, dr=0.0):
-        super(SimpleLSTM, self).__init__()
-        self.linearIn = nn.Linear(input_size, hidden_size)
-        self.lstm = nn.LSTM(
-            hidden_size,
-            hidden_size,
-            1,
-            dropout=dr,
-        )
-        self.linearOut = nn.Linear(hidden_size, output_size)
-
-    def forward(self, x):
-        x0 = F.relu(self.linearIn(x))
-        out_lstm, (hn, cn) = self.lstm(x0)
-        return self.linearOut(out_lstm)
-
-
-class SlowLSTM(nn.Module):
-    """
-    A pedagogic implementation of Hochreiter & Schmidhuber:
-    'Long-Short Term Memory'
-    http://www.bioinf.jku.at/publications/older/2604.pdf
-    """
-
-    def __init__(self, input_size, hidden_size, bias=True, dropout=0.0):
-        super(SlowLSTM, self).__init__()
-        self.input_size = input_size
-        self.hidden_size = hidden_size
-        self.bias = bias
-        self.dropout = dropout
-        # input to hidden weights
-        self.w_xi = P(T(hidden_size, input_size))
-        self.w_xf = P(T(hidden_size, input_size))
-        self.w_xo = P(T(hidden_size, input_size))
-        self.w_xc = P(T(hidden_size, input_size))
-        # hidden to hidden weights
-        self.w_hi = P(T(hidden_size, hidden_size))
-        self.w_hf = P(T(hidden_size, hidden_size))
-        self.w_ho = P(T(hidden_size, hidden_size))
-        self.w_hc = P(T(hidden_size, hidden_size))
-        # bias terms
-        self.b_i = T(hidden_size).fill_(0)
-        self.b_f = T(hidden_size).fill_(0)
-        self.b_o = T(hidden_size).fill_(0)
-        self.b_c = T(hidden_size).fill_(0)
-
-        # Wrap biases as parameters if desired, else as variables without gradients
-        W = P if bias else (lambda x: P(x, requires_grad=False))
-        self.b_i = W(self.b_i)
-        self.b_f = W(self.b_f)
-        self.b_o = W(self.b_o)
-        self.b_c = W(self.b_c)
-        self.reset_parameters()
-
-    def reset_parameters(self):
-        std = 1.0 / math.sqrt(self.hidden_size)
-        for w in self.parameters():
-            w.data.uniform_(-std, std)
-
-    def forward(self, x, hidden):
-        h, c = hidden
-        h = h.view(h.size(0), -1)
-        c = c.view(h.size(0), -1)
-        x = x.view(x.size(0), -1)
-        # Linear mappings
-        i_t = th.mm(x, self.w_xi) + th.mm(h, self.w_hi) + self.b_i
-        f_t = th.mm(x, self.w_xf) + th.mm(h, self.w_hf) + self.b_f
-        o_t = th.mm(x, self.w_xo) + th.mm(h, self.w_ho) + self.b_o
-        # activations
-        i_t.sigmoid_()
-        f_t.sigmoid_()
-        o_t.sigmoid_()
-        # cell computations
-        c_t = th.mm(x, self.w_xc) + th.mm(h, self.w_hc) + self.b_c
-        c_t.tanh_()
-        c_t = th.mul(c, f_t) + th.mul(i_t, c_t)
-        h_t = th.mul(o_t, th.tanh(c_t))
-        # Reshape for compatibility
-        h_t = h_t.view(h_t.size(0), 1, -1)
-        c_t = c_t.view(c_t.size(0), 1, -1)
-        if self.dropout > 0.0:
-            F.dropout(h_t, p=self.dropout, training=self.training, inplace=True)
-        return h_t, (h_t, c_t)
-
-    def sample_mask(self):
-        pass
+"""
+Author: Wenyu Ouyang
+Date: 2023-09-19 09:36:25
+LastEditTime: 2024-04-09 15:29:35
+LastEditors: Wenyu Ouyang
+Description: Some self-made LSTMs
+FilePath: \torchhydro\torchhydro\models\simple_lstm.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+
+import math
+import torch as th
+import torch.nn as nn
+from torch.nn import functional as F
+from torch import Tensor as T
+from torch.nn import Parameter as P
+
+
+class SimpleLSTM(nn.Module):
+    def __init__(self, input_size, output_size, hidden_size, dr=0.0):
+        super(SimpleLSTM, self).__init__()
+        self.linearIn = nn.Linear(input_size, hidden_size)
+        self.lstm = nn.LSTM(
+            hidden_size,
+            hidden_size,
+            1,
+            dropout=dr,
+        )
+        self.linearOut = nn.Linear(hidden_size, output_size)
+
+    def forward(self, x):
+        x0 = F.relu(self.linearIn(x))
+        out_lstm, (hn, cn) = self.lstm(x0)
+        return self.linearOut(out_lstm)
+
+
+class SimpleLSTMForecast(SimpleLSTM):
+    def __init__(self, input_size, output_size, hidden_size, forecast_length, dr=0.0):
+        super(SimpleLSTMForecast, self).__init__(
+            input_size, output_size, hidden_size, dr
+        )
+        self.forecast_length = forecast_length
+
+    def forward(self, x):
+        # 调用父类的forward方法获取完整的输出
+        full_output = super(SimpleLSTMForecast, self).forward(x)
+
+        return full_output[-self.forecast_length :, :, :]
+
+
+class SlowLSTM(nn.Module):
+    """
+    A pedagogic implementation of Hochreiter & Schmidhuber:
+    'Long-Short Term Memory'
+    http://www.bioinf.jku.at/publications/older/2604.pdf
+    """
+
+    def __init__(self, input_size, hidden_size, bias=True, dropout=0.0):
+        super(SlowLSTM, self).__init__()
+        self.input_size = input_size
+        self.hidden_size = hidden_size
+        self.bias = bias
+        self.dropout = dropout
+        # input to hidden weights
+        self.w_xi = P(T(hidden_size, input_size))
+        self.w_xf = P(T(hidden_size, input_size))
+        self.w_xo = P(T(hidden_size, input_size))
+        self.w_xc = P(T(hidden_size, input_size))
+        # hidden to hidden weights
+        self.w_hi = P(T(hidden_size, hidden_size))
+        self.w_hf = P(T(hidden_size, hidden_size))
+        self.w_ho = P(T(hidden_size, hidden_size))
+        self.w_hc = P(T(hidden_size, hidden_size))
+        # bias terms
+        self.b_i = T(hidden_size).fill_(0)
+        self.b_f = T(hidden_size).fill_(0)
+        self.b_o = T(hidden_size).fill_(0)
+        self.b_c = T(hidden_size).fill_(0)
+
+        # Wrap biases as parameters if desired, else as variables without gradients
+        W = P if bias else (lambda x: P(x, requires_grad=False))
+        self.b_i = W(self.b_i)
+        self.b_f = W(self.b_f)
+        self.b_o = W(self.b_o)
+        self.b_c = W(self.b_c)
+        self.reset_parameters()
+
+    def reset_parameters(self):
+        std = 1.0 / math.sqrt(self.hidden_size)
+        for w in self.parameters():
+            w.data.uniform_(-std, std)
+
+    def forward(self, x, hidden):
+        h, c = hidden
+        h = h.view(h.size(0), -1)
+        c = c.view(h.size(0), -1)
+        x = x.view(x.size(0), -1)
+        # Linear mappings
+        i_t = th.mm(x, self.w_xi) + th.mm(h, self.w_hi) + self.b_i
+        f_t = th.mm(x, self.w_xf) + th.mm(h, self.w_hf) + self.b_f
+        o_t = th.mm(x, self.w_xo) + th.mm(h, self.w_ho) + self.b_o
+        # activations
+        i_t.sigmoid_()
+        f_t.sigmoid_()
+        o_t.sigmoid_()
+        # cell computations
+        c_t = th.mm(x, self.w_xc) + th.mm(h, self.w_hc) + self.b_c
+        c_t.tanh_()
+        c_t = th.mul(c, f_t) + th.mul(i_t, c_t)
+        h_t = th.mul(o_t, th.tanh(c_t))
+        # Reshape for compatibility
+        h_t = h_t.view(h_t.size(0), 1, -1)
+        c_t = c_t.view(c_t.size(0), 1, -1)
+        if self.dropout > 0.0:
+            F.dropout(h_t, p=self.dropout, training=self.training, inplace=True)
+        return h_t, (h_t, c_t)
+
+    def sample_mask(self):
+        pass
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `torchhydro-0.0.4/torchhydro/trainers/deep_hydro.py` & `torchhydro-0.0.5/torchhydro/trainers/deep_hydro.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,710 +1,958 @@
-"""
-Author: Wenyu Ouyang
-Date: 2021-12-31 11:08:29
-LastEditTime: 2023-10-28 13:22:06
-LastEditors: Wenyu Ouyang
-Description: HydroDL model class
-FilePath: \torchhydro\torchhydro\trainers\deep_hydro.py
-Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
-"""
-
-from abc import ABC, abstractmethod
-from collections import defaultdict
-import copy
-from functools import reduce
-import os
-from typing import Dict, Tuple
-from hydroutils.hydro_stat import stat_error
-import numpy as np
-import torch
-from torch import nn
-from hydrodataset import HydroDataset
-from torch.utils.data import DataLoader
-from tqdm import tqdm
-from torchhydro.explainers.shap import (
-    deep_explain_model_heatmap,
-    deep_explain_model_summary_plot,
-)
-from torchhydro.configs.config import update_nested_dict
-from torchhydro.datasets.sampler import KuaiSampler, fl_sample_basin, fl_sample_region
-from torchhydro.datasets.data_dict import datasets_dict
-from torchhydro.models.model_dict_function import (
-    pytorch_criterion_dict,
-    pytorch_model_dict,
-    pytorch_model_wrapper_dict,
-    pytorch_opt_dict,
-)
-from torchhydro.models.model_utils import get_the_device
-from torchhydro.trainers.train_utils import (
-    EarlyStopper,
-    average_weights,
-    denormalize4eval,
-    evaluate_validation,
-    compute_validation,
-    model_infer,
-    torch_single_train,
-    cellstates_when_inference,
-)
-from torchhydro.trainers.train_logger import TrainLogger
-
-
-class DeepHydroInterface(ABC):
-    """
-    An abstract class used to handle different configurations
-    of hydrological deep learning models + hyperparams for training, test, and predict functions.
-    This class assumes that data is already split into test train and validation at this point.
-    """
-
-    def __init__(self, data_source: HydroDataset, cfgs: Dict):
-        """
-        Parameters
-        ----------
-        data_source
-            the digital twin of a data_source in reality
-        cfgs
-            configs for initializing DeepHydro
-        """
-        self._data_source = data_source
-        self._cfgs = cfgs
-
-    @property
-    def data_source(self):
-        """data source"""
-        return self._data_source
-
-    @property
-    def cfgs(self):
-        """all configs"""
-        return self._cfgs
-
-    @property
-    def weight_path(self):
-        """weight path"""
-        return self._cfgs["model_cfgs"]["weight_path"]
-
-    @weight_path.setter
-    def weight_path(self, weight_path):
-        self._cfgs["model_cfgs"]["weight_path"] = weight_path
-
-    @abstractmethod
-    def load_model(self) -> object:
-        """Get a Hydro DL model"""
-        raise NotImplementedError
-
-    @abstractmethod
-    def make_dataset(self, is_tra_val_te: str) -> object:
-        """
-        Initializes a pytorch dataset based on the provided data_source.
-
-        Parameters
-        ----------
-        is_tra_val_te
-            train or valid or test
-
-        Returns
-        -------
-        object
-            a dataset class loading data from data source
-        """
-        raise NotImplementedError
-
-    @abstractmethod
-    def model_train(self):
-        """
-        Train the model
-        """
-        raise NotImplementedError
-
-    @abstractmethod
-    def model_evaluate(self):
-        """
-        Evaluate the model
-        """
-        raise NotImplementedError
-
-
-class DeepHydro(DeepHydroInterface):
-    """
-    The Base Trainer class for Hydrological Deep Learning models
-    """
-
-    def __init__(
-        self,
-        data_source: HydroDataset,
-        cfgs: Dict,
-        pre_model=None,
-    ):
-        """
-        Parameters
-        ----------
-        data_source
-            data source where we read data from
-        cfgs
-            configs for the model
-        pre_model
-            a pre-trained model, if it is not None,
-            we will use its weights to initialize this model
-            by default None
-        """
-        self.device_num = cfgs["training_cfgs"]["device"]
-        self.device = get_the_device(self.device_num)
-        self.pre_model = pre_model
-        super().__init__(data_source, cfgs)
-        self.model = self.load_model()
-        self.traindataset = self.make_dataset("train")
-        if cfgs["data_cfgs"]["t_range_valid"] is not None:
-            self.validdataset = self.make_dataset("valid")
-        self.testdataset = self.make_dataset("test")
-        print(f"Torch is using {str(self.device)}")
-
-    def load_model(self):
-        """
-        Load a time series forecast model in pytorch_model_dict in model_dict_function.py
-
-        Returns
-        -------
-        object
-            model in pytorch_model_dict in model_dict_function.py
-        """
-        model_cfgs = self.cfgs["model_cfgs"]
-        model_name = model_cfgs["model_name"]
-        if model_name not in pytorch_model_dict:
-            raise NotImplementedError(
-                f"Error the model {model_name} was not found in the model dict. Please add it."
-            )
-        if self.pre_model is not None:
-            model = self._load_pretrain_model()
-        elif self.weight_path is not None:
-            # load model from pth file (saved weights and biases)
-            model = self._load_model_from_pth()
-        else:
-            model = pytorch_model_dict[model_name](**model_cfgs["model_hyperparam"])
-        if torch.cuda.device_count() > 1 and len(self.device_num) > 1:
-            print("Let's use", torch.cuda.device_count(), "GPUs!")
-            which_first_tensor = self.cfgs["training_cfgs"]["which_first_tensor"]
-            sequece_first = which_first_tensor == "sequence"
-            parallel_dim = 1 if sequece_first else 0
-            model = nn.DataParallel(model, device_ids=self.device_num, dim=parallel_dim)
-        model.to(self.device)
-        return model
-
-    def _load_pretrain_model(self):
-        """load a pretrained model as the initial model"""
-        return self.pre_model
-
-    def _load_model_from_pth(self):
-        weight_path = self.weight_path
-        model_cfgs = self.cfgs["model_cfgs"]
-        model_name = model_cfgs["model_name"]
-        model = pytorch_model_dict[model_name](**model_cfgs["model_hyperparam"])
-        checkpoint = torch.load(weight_path, map_location=self.device)
-        model.load_state_dict(checkpoint)
-        print("Weights sucessfully loaded")
-        return model
-
-    def make_dataset(self, is_tra_val_te: str):
-        """
-        Initializes a pytorch dataset based on the provided data_source.
-
-        Parameters
-        ----------
-        is_tra_val_te
-            train or valid or test
-
-        Returns
-        -------
-        object
-            an object initializing from class in datasets_dict in data_dict.py
-        """
-        data_cfgs = self.cfgs["data_cfgs"]
-        dataset_name = data_cfgs["dataset"]
-        data_source = self.data_source
-        if dataset_name in list(datasets_dict.keys()):
-            dataset = datasets_dict[dataset_name](data_source, data_cfgs, is_tra_val_te)
-        else:
-            raise NotImplementedError(
-                f"Error the dataset {str(dataset_name)} was not found in the dataset dict. Please add it."
-            )
-        return dataset
-
-    def model_train(self) -> None:
-        """train a hydrological DL model"""
-        # A dictionary of the necessary parameters for training
-        training_cfgs = self.cfgs["training_cfgs"]
-        # The file path to load model weights from; defaults to "model_save"
-        model_filepath = self.cfgs["data_cfgs"]["test_path"]
-        data_cfgs = self.cfgs["data_cfgs"]
-        es = None
-        if "early_stopping" in self.cfgs:
-            es = EarlyStopper(self.cfgs["early_stopping"]["patience"])
-        criterion = self._get_loss_func(training_cfgs)
-        opt = self._get_optimizer(training_cfgs)
-        lr_scheduler = training_cfgs["lr_scheduler"]
-        max_epochs = training_cfgs["epochs"]
-        start_epoch = training_cfgs["start_epoch"]
-        # use PyTorch's DataLoader to load the data into batches in each epoch
-        data_loader, validation_data_loader = self._get_dataloader(
-            training_cfgs, data_cfgs
-        )
-        logger = TrainLogger(model_filepath, self.cfgs, opt)
-        for epoch in range(start_epoch, max_epochs + 1):
-            with logger.log_epoch_train(epoch) as train_logs:
-                if lr_scheduler is not None and epoch in lr_scheduler.keys():
-                    # now we only support manual setting lr scheduler
-                    for param_group in opt.param_groups:
-                        param_group["lr"] = lr_scheduler[epoch]
-                total_loss, n_iter_ep = torch_single_train(
-                    self.model,
-                    opt,
-                    criterion,
-                    data_loader,
-                    device=self.device,
-                    which_first_tensor=training_cfgs["which_first_tensor"],
-                )
-                train_logs["train_loss"] = total_loss
-                train_logs["model"] = self.model
-
-            valid_loss = None
-            valid_metrics = None
-            if data_cfgs["t_range_valid"] is not None:
-                with logger.log_epoch_valid(epoch) as valid_logs:
-                    valid_obss_np, valid_preds_np, valid_loss = compute_validation(
-                        self.model,
-                        criterion,
-                        validation_data_loader,
-                        device=self.device,
-                        which_first_tensor=training_cfgs["which_first_tensor"],
-                    )
-                    evaluation_metrics = self.cfgs["evaluation_cfgs"]["metrics"]
-                    fill_nan = self.cfgs["evaluation_cfgs"]["fill_nan"]
-                    target_col = self.cfgs["data_cfgs"]["target_cols"]
-                    valid_metrics = evaluate_validation(
-                        validation_data_loader,
-                        valid_preds_np,
-                        valid_obss_np,
-                        evaluation_metrics,
-                        fill_nan,
-                        target_col,
-                    )
-                    valid_logs["valid_loss"] = valid_loss
-                    valid_logs["valid_metrics"] = valid_metrics
-            logger.save_session_param(
-                epoch, total_loss, n_iter_ep, valid_loss, valid_metrics
-            )
-            logger.save_model_and_params(self.model, epoch, self.cfgs)
-            if es and not es.check_loss(self.model, valid_loss):
-                print("Stopping model now")
-                self.model.load_state_dict(torch.load("checkpoint.pth"))
-                break
-
-        logger.tb.close()
-        # return the trained model weights and bias and the epoch loss
-        return self.model.state_dict(), sum(logger.epoch_loss) / len(logger.epoch_loss)
-
-    def model_evaluate(self) -> Tuple[Dict, np.array, np.array]:
-        """
-        A function to evaluate a model, called at end of training.
-
-        Returns
-        -------
-        tuple[dict, np.array, np.array]
-            eval_log, denormalized predictions and observations
-        """
-        # types of observations
-        target_col = self.cfgs["data_cfgs"]["target_cols"]
-        evaluation_metrics = self.cfgs["evaluation_cfgs"]["metrics"]
-        # fill_nan: "no" means ignoring the NaN value;
-        #           "sum" means calculate the sum of the following values in the NaN locations.
-        #           For example, observations are [1, nan, nan, 2], and predictions are [0.3, 0.3, 0.3, 1.5].
-        #           Then, "no" means [1, 2] v.s. [0.3, 1.5] while "sum" means [1, 2] v.s. [0.3 + 0.3 + 0.3, 1.5].
-        #           If it is a str, then all target vars use same fill_nan method;
-        #           elif it is a list, each for a var
-        fill_nan = self.cfgs["evaluation_cfgs"]["fill_nan"]
-        # save result here
-        eval_log = {}
-
-        # test the trained model
-        test_epoch = self.cfgs["evaluation_cfgs"]["test_epoch"]
-        train_epoch = self.cfgs["training_cfgs"]["epochs"]
-        if test_epoch != train_epoch:
-            # Generally we use same epoch for train and test, but sometimes not
-            # TODO: better refactor this part, because sometimes we save multi models for multi hyperparameters
-            model_filepath = self.cfgs["data_cfgs"]["test_path"]
-            self.model = self.load_model(
-                self.cfgs["model_cfgs"],
-                weight_path=os.path.join(
-                    model_filepath, f"model_Ep{str(test_epoch)}.pth"
-                ),
-            )
-        preds_xr, obss_xr, test_data = self.inference()
-        #  Then evaluate the model metrics
-        if type(fill_nan) is list and len(fill_nan) != len(target_col):
-            raise ValueError("length of fill_nan must be equal to target_col's")
-        for i in range(len(target_col)):
-            obs_xr = obss_xr[list(obss_xr.data_vars.keys())[i]]
-            pred_xr = preds_xr[list(preds_xr.data_vars.keys())[i]]
-            if type(fill_nan) is str:
-                inds = stat_error(
-                    obs_xr.to_numpy(),
-                    pred_xr.to_numpy(),
-                    fill_nan,
-                )
-            else:
-                inds = stat_error(
-                    obs_xr.to_numpy(),
-                    pred_xr.to_numpy(),
-                    fill_nan[i],
-                )
-            for evaluation_metric in evaluation_metrics:
-                eval_log[f"{evaluation_metric} of {target_col[i]}"] = inds[
-                    evaluation_metric
-                ]
-
-        # Finally, try to explain model behaviour using shap
-        is_shap = self.cfgs["evaluation_cfgs"]["explainer"] == "shap"
-        if is_shap:
-            deep_explain_model_summary_plot(self.model, test_data)
-            deep_explain_model_heatmap(self.model, test_data)
-
-        return eval_log, preds_xr, obss_xr
-
-    def inference(self) -> Tuple[torch.Tensor, torch.Tensor]:
-        """infer using trained model and unnormalized results"""
-        data_cfgs = self.cfgs["data_cfgs"]
-        training_cfgs = self.cfgs["training_cfgs"]
-        device = get_the_device(self.cfgs["training_cfgs"]["device"])
-        test_dataloader = DataLoader(
-            self.testdataset,
-            batch_size=training_cfgs["batch_size"],
-            shuffle=False,
-            sampler=None,
-            batch_sampler=None,
-            drop_last=False,
-            timeout=0,
-            worker_init_fn=None,
-        )
-        seq_first = training_cfgs["which_first_tensor"] == "sequence"
-        self.model.eval()
-        # here the batch is just an index of lookup table, so any batch size could be chosen
-        test_preds = []
-        obss = []
-        with torch.no_grad():
-            for xs, ys in test_dataloader:
-                # here the a batch doesn't mean a basin; it is only an index in lookup table
-                # for NtoN mode, only basin is index in lookup table, so the batch is same as basin
-                # for Nto1 mode, batch is only an index
-                ys, output = model_infer(seq_first, device, self.model, xs, ys)
-                test_preds.append(output.cpu().numpy())
-                obss.append(ys.cpu().numpy())
-            pred = reduce(lambda x, y: np.vstack((x, y)), test_preds)
-            obs = reduce(lambda x, y: np.vstack((x, y)), obss)
-        if pred.ndim == 2:
-            # TODO: check
-            # the ndim is 2 meaning we use an Nto1 mode
-            # as lookup table is (basin 1's all time length, basin 2's all time length, ...)
-            # params of reshape should be (basin size, time length)
-            pred = pred.flatten().reshape(test_dataloader.test_data.y.shape[0], -1, 1)
-            obs = obs.flatten().reshape(test_dataloader.test_data.y.shape[0], -1, 1)
-        # TODO: not support return_cell_states yet
-        return_cell_state = False
-        if return_cell_state:
-            return cellstates_when_inference(seq_first, data_cfgs, pred)
-        pred_xr, obs_xr = denormalize4eval(test_dataloader, pred, obs)
-        return pred_xr, obs_xr, self.testdataset
-
-    def _get_optimizer(self, training_cfgs):
-        params_in_opt = self.model.parameters()
-        return pytorch_opt_dict[training_cfgs["optimizer"]](
-            params_in_opt, **training_cfgs["optim_params"]
-        )
-
-    def _get_loss_func(self, training_cfgs):
-        criterion_init_params = {}
-        if "criterion_params" in training_cfgs:
-            loss_param = training_cfgs["criterion_params"]
-            if loss_param is not None:
-                for key in loss_param.keys():
-                    if key == "loss_funcs":
-                        criterion_init_params[key] = pytorch_criterion_dict[
-                            loss_param[key]
-                        ]()
-                    else:
-                        criterion_init_params[key] = loss_param[key]
-        return pytorch_criterion_dict[training_cfgs["criterion"]](
-            **criterion_init_params
-        )
-
-    def _get_dataloader(self, training_cfgs, data_cfgs):
-        worker_num = 0
-        pin_memory = False
-        if "num_workers" in training_cfgs:
-            worker_num = training_cfgs["num_workers"]
-            print(f"using {str(worker_num)} workers")
-        if "pin_memory" in training_cfgs:
-            pin_memory = training_cfgs["pin_memory"]
-            print(f"Pin memory set to {str(pin_memory)}")
-        train_dataset = self.traindataset
-        sampler = None
-        if data_cfgs["sampler"] is not None:
-            # now we only have one special sampler from Kuai Fang's Deep Learning papers
-            batch_size = data_cfgs["batch_size"]
-            rho = data_cfgs["forecast_history"]
-            warmup_length = data_cfgs["warmup_length"]
-            ngrid = train_dataset.y.basin.size
-            nt = train_dataset.y.time.size
-            sampler = KuaiSampler(
-                train_dataset,
-                batch_size=batch_size,
-                warmup_length=warmup_length,
-                rho=rho,
-                ngrid=ngrid,
-                nt=nt,
-            )
-        data_loader = DataLoader(
-            train_dataset,
-            batch_size=training_cfgs["batch_size"],
-            shuffle=(sampler is None),
-            sampler=sampler,
-            num_workers=worker_num,
-            pin_memory=pin_memory,
-            timeout=0,
-        )
-        if data_cfgs["t_range_valid"] is not None:
-            valid_dataset = self.validdataset
-            validation_data_loader = DataLoader(
-                valid_dataset,
-                batch_size=training_cfgs["batch_size"],
-                shuffle=False,
-                num_workers=worker_num,
-                pin_memory=pin_memory,
-                timeout=0,
-            )
-            return data_loader, validation_data_loader
-
-        return data_loader, None
-
-
-class FedLearnHydro(DeepHydro):
-    """Federated Learning Hydrological DL model"""
-
-    def __init__(self, data_source: HydroDataset, cfgs: Dict):
-        super().__init__(data_source, cfgs)
-        # a user group which is a dict where the keys are the user index
-        # and the values are the corresponding data for each of those users
-        train_dataset = self.traindataset
-        fl_hyperparam = self.cfgs["model_cfgs"]["fl_hyperparam"]
-        # sample training data amongst users
-        if fl_hyperparam["fl_sample"] == "basin":
-            # Sample a basin for a user
-            user_groups = fl_sample_basin(train_dataset)
-        elif fl_hyperparam["fl_sample"] == "region":
-            # Sample a region for a user
-            user_groups = fl_sample_region(train_dataset)
-        else:
-            raise NotImplementedError()
-        self.user_groups = user_groups
-
-    @property
-    def num_users(self):
-        """number of users in federated learning"""
-        return len(self.user_groups)
-
-    def model_train(self) -> None:
-        # BUILD MODEL
-        global_model = self.model
-
-        # copy weights
-        global_weights = global_model.state_dict()
-
-        # Training
-        train_loss, train_accuracy = [], []
-        print_every = 2
-
-        training_cfgs = self.cfgs["training_cfgs"]
-        model_cfgs = self.cfgs["model_cfgs"]
-        max_epochs = training_cfgs["epochs"]
-        start_epoch = training_cfgs["start_epoch"]
-        fl_hyperparam = model_cfgs["fl_hyperparam"]
-        # total rounds in a FL system is max_epochs
-        for epoch in tqdm(range(start_epoch, max_epochs + 1)):
-            local_weights, local_losses = [], []
-            print(f"\n | Global Training Round : {epoch} |\n")
-
-            global_model.train()
-            m = max(int(fl_hyperparam["fl_frac"] * self.num_users), 1)
-            # randomly select m users, they will be the clients in this round
-            idxs_users = np.random.choice(range(self.num_users), m, replace=False)
-
-            for idx in idxs_users:
-                # each user will be used to train the model locally
-                # user_gourps[idx] means the idx of dataset for a user
-                user_cfgs = self._get_a_user_cfgs(idx)
-                local_model = DeepHydro(
-                    self.data_source,
-                    user_cfgs,
-                    pre_model=copy.deepcopy(global_model),
-                )
-                w, loss = local_model.model_train()
-                local_weights.append(copy.deepcopy(w))
-                local_losses.append(copy.deepcopy(loss))
-
-            # update global weights
-            global_weights = average_weights(local_weights)
-
-            # update global weights
-            global_model.load_state_dict(global_weights)
-
-            loss_avg = sum(local_losses) / len(local_losses)
-            train_loss.append(loss_avg)
-
-            # Calculate avg training accuracy over all users at every epoch
-            list_acc = []
-            global_model.eval()
-            for c in range(self.num_users):
-                one_user_cfg = self._get_a_user_cfgs(c)
-                local_model = DeepHydro(
-                    self.data_source,
-                    one_user_cfg,
-                    pre_model=global_model,
-                )
-                acc, _, _ = local_model.model_evaluate()
-                list_acc.append(acc)
-            values = [list(d.values())[0][0] for d in list_acc]
-            filtered_values = [v for v in values if not np.isnan(v)]
-            train_accuracy.append(sum(filtered_values) / len(filtered_values))
-
-            # print global training loss after every 'i' rounds
-            if (epoch + 1) % print_every == 0:
-                print(f" \nAvg Training Stats after {epoch+1} global rounds:")
-                print(f"Training Loss : {np.mean(np.array(train_loss))}")
-                print("Train Accuracy: {:.2f}% \n".format(100 * train_accuracy[-1]))
-
-    def _get_a_user_cfgs(self, idx):
-        """To get a user's configs for local training"""
-        user = self.user_groups[idx]
-
-        # update data_cfgs
-        # Use defaultdict to collect dates for each basin
-        basin_dates = defaultdict(list)
-
-        for _, (basin, time) in user.items():
-            basin_dates[basin].append(time)
-
-        # Initialize a list to store distinct basins
-        basins = []
-
-        # for each basin, we can find its date range
-        date_ranges = {}
-        for basin, times in basin_dates.items():
-            basins.append(basin)
-            date_ranges[basin] = (np.min(times), np.max(times))
-        # get the longest date range
-        longest_date_range = max(date_ranges.values(), key=lambda x: x[1] - x[0])
-        # transform the date range of numpy data into string
-        longest_date_range = [
-            np.datetime_as_string(dt, unit="D") for dt in longest_date_range
-        ]
-        user_cfgs = copy.deepcopy(self.cfgs)
-        # update data_cfgs
-        update_nested_dict(
-            user_cfgs, ["data_cfgs", "t_range_train"], longest_date_range
-        )
-        # for local training in FL, we don't need a validation set
-        update_nested_dict(user_cfgs, ["data_cfgs", "t_range_valid"], None)
-        # for local training in FL, we don't need a test set, but we should set one to avoid error
-        update_nested_dict(user_cfgs, ["data_cfgs", "t_range_test"], longest_date_range)
-        update_nested_dict(user_cfgs, ["data_cfgs", "object_ids"], basins)
-
-        # update training_cfgs
-        # we also need to update some training params for local training from FL settings
-        update_nested_dict(
-            user_cfgs,
-            ["training_cfgs", "epochs"],
-            user_cfgs["model_cfgs"]["fl_hyperparam"]["fl_local_ep"],
-        )
-        update_nested_dict(
-            user_cfgs,
-            ["evaluation_cfgs", "test_epoch"],
-            user_cfgs["model_cfgs"]["fl_hyperparam"]["fl_local_ep"],
-        )
-        # don't need to save model weights for local training
-        update_nested_dict(
-            user_cfgs,
-            ["training_cfgs", "save_epoch"],
-            None,
-        )
-        # there are two settings for batch size in configs, we need to update both of them
-        update_nested_dict(
-            user_cfgs,
-            ["training_cfgs", "batch_size"],
-            user_cfgs["model_cfgs"]["fl_hyperparam"]["fl_local_bs"],
-        )
-        update_nested_dict(
-            user_cfgs,
-            ["data_cfgs", "batch_size"],
-            user_cfgs["model_cfgs"]["fl_hyperparam"]["fl_local_bs"],
-        )
-
-        # update model_cfgs finally
-        # For local model, its model_type is Normal
-        update_nested_dict(user_cfgs, ["model_cfgs", "model_type"], "Normal")
-        update_nested_dict(
-            user_cfgs,
-            ["model_cfgs", "fl_hyperparam"],
-            None,
-        )
-        return user_cfgs
-
-
-class TransLearnHydro(DeepHydro):
-    def __init__(self, data_source: HydroDataset, cfgs: Dict, pre_model=None):
-        super().__init__(data_source, cfgs, pre_model)
-
-    def load_model(self):
-        """Load model for transfer learning"""
-        model_cfgs = self.cfgs["model_cfgs"]
-        if self.weight_path is None and self.pre_model is None:
-            raise NotImplementedError(
-                "For transfer learning, we need a pre-trained model"
-            )
-        model = super().load_model()
-        if (
-            "weight_path_add" in model_cfgs
-            and "freeze_params" in model_cfgs["weight_path_add"]
-        ):
-            freeze_params = model_cfgs["weight_path_add"]["freeze_params"]
-            for param in freeze_params:
-                exec(f"model.{param}.requires_grad = False")
-        if ("model_wrapper" in list(model_cfgs.keys())) and (
-            model_cfgs["model_wrapper"] is not None
-        ):
-            wrapper_name = model_cfgs["model_wrapper"]
-            wrapper_params = model_cfgs["model_wrapper_param"]
-            model = pytorch_model_wrapper_dict[wrapper_name](model, **wrapper_params)
-        return model
-
-    def _load_model_from_pth(self):
-        weight_path = self.weight_path
-        model_cfgs = self.cfgs["model_cfgs"]
-        model_name = model_cfgs["model_name"]
-        model = pytorch_model_dict[model_name](**model_cfgs["model_hyperparam"])
-        checkpoint = torch.load(weight_path, map_location=self.device)
-        if "weight_path_add" in model_cfgs:
-            if "excluded_layers" in model_cfgs["weight_path_add"]:
-                # delete some layers from source model if we don't need them
-                excluded_layers = model_cfgs["weight_path_add"]["excluded_layers"]
-                for layer in excluded_layers:
-                    del checkpoint[layer]
-                print("sucessfully deleted layers")
-            else:
-                print("directly loading identically-named layers of source model")
-        model.load_state_dict(checkpoint, strict=False)
-        print("Weights sucessfully loaded")
-        return model
-
-
-model_type_dict = {
-    "Normal": DeepHydro,
-    "FedLearn": FedLearnHydro,
-    "TransLearn": TransLearnHydro,
-}
+"""
+Author: Wenyu Ouyang
+Date: 2024-04-08 18:15:48
+LastEditTime: 2024-05-27 09:40:00
+LastEditors: Wenyu Ouyang
+Description: HydroDL model class
+FilePath: \torchhydro\torchhydro\trainers\deep_hydro.py
+Copyright (c) 2024-2024 Wenyu Ouyang. All rights reserved.
+"""
+
+import copy
+import os
+from abc import ABC, abstractmethod
+from collections import defaultdict
+from functools import reduce
+from typing import Dict, Tuple
+
+import numpy as np
+import torch
+import torch.distributed as dist
+import torch.nn as nn
+from hydroutils.hydro_file import get_lastest_file_in_a_dir
+from torch.nn.parallel import DistributedDataParallel as DDP
+from torch.optim.lr_scheduler import *
+from torch.utils.data import DataLoader, DistributedSampler
+from tqdm import tqdm
+
+from torchhydro.configs.config import update_nested_dict
+from torchhydro.datasets.data_dict import datasets_dict
+from torchhydro.datasets.data_sets import BaseDataset
+from torchhydro.datasets.sampler import (
+    KuaiSampler,
+    fl_sample_basin,
+    fl_sample_region,
+    HydroSampler,
+)
+from torchhydro.models.model_dict_function import (
+    pytorch_criterion_dict,
+    pytorch_model_dict,
+    pytorch_opt_dict,
+)
+from torchhydro.models.model_utils import get_the_device
+from torchhydro.trainers.train_logger import TrainLogger
+from torchhydro.trainers.train_utils import (
+    EarlyStopper,
+    average_weights,
+    denormalize4eval,
+    evaluate_validation,
+    compute_validation,
+    model_infer,
+    torch_single_train,
+    cellstates_when_inference,
+    calculate_and_record_metrics,
+)
+
+
+class DeepHydroInterface(ABC):
+    """
+    An abstract class used to handle different configurations
+    of hydrological deep learning models + hyperparams for training, test, and predict functions.
+    This class assumes that data is already split into test train and validation at this point.
+    """
+
+    def __init__(self, cfgs: Dict):
+        """
+        Parameters
+        ----------
+        cfgs
+            configs for initializing DeepHydro
+        """
+
+        self._cfgs = cfgs
+
+    @property
+    def cfgs(self):
+        """all configs"""
+        return self._cfgs
+
+    @property
+    def weight_path(self):
+        """weight path"""
+        return self._cfgs["model_cfgs"]["weight_path"]
+
+    @weight_path.setter
+    def weight_path(self, weight_path):
+        self._cfgs["model_cfgs"]["weight_path"] = weight_path
+
+    @abstractmethod
+    def load_model(self, mode="train") -> object:
+        """Get a Hydro DL model"""
+        raise NotImplementedError
+
+    @abstractmethod
+    def make_dataset(self, is_tra_val_te: str) -> object:
+        """
+        Initializes a pytorch dataset.
+
+        Parameters
+        ----------
+        is_tra_val_te
+            train or valid or test
+
+        Returns
+        -------
+        object
+            a dataset class loading data from data source
+        """
+        raise NotImplementedError
+
+    @abstractmethod
+    def model_train(self):
+        """
+        Train the model
+        """
+        raise NotImplementedError
+
+    @abstractmethod
+    def model_evaluate(self):
+        """
+        Evaluate the model
+        """
+        raise NotImplementedError
+
+
+class DeepHydro(DeepHydroInterface):
+    """
+    The Base Trainer class for Hydrological Deep Learning models
+    """
+
+    def __init__(
+        self,
+        cfgs: Dict,
+        pre_model=None,
+    ):
+        """
+        Parameters
+        ----------
+        cfgs
+            configs for the model
+        pre_model
+            a pre-trained model, if it is not None,
+            we will use its weights to initialize this model
+            by default None
+        """
+        super().__init__(cfgs)
+        self.device_num = cfgs["training_cfgs"]["device"]
+        self.device = get_the_device(self.device_num)
+        self.pre_model = pre_model
+        self.model = self.load_model()
+        if cfgs["training_cfgs"]["train_mode"]:
+            self.traindataset = self.make_dataset("train")
+            if cfgs["data_cfgs"]["t_range_valid"] is not None:
+                self.validdataset = self.make_dataset("valid")
+        self.testdataset: BaseDataset = self.make_dataset("test")
+        print(f"Torch is using {str(self.device)}")
+
+    def load_model(self, mode="train"):
+        """
+        Load a time series forecast model in pytorch_model_dict in model_dict_function.py
+
+        Returns
+        -------
+        object
+            model in pytorch_model_dict in model_dict_function.py
+        """
+        if mode == "infer":
+            self.weight_path = self._get_trained_model()
+        elif mode != "train":
+            raise ValueError("Invalid mode; must be 'train' or 'infer'")
+        model_cfgs = self.cfgs["model_cfgs"]
+        model_name = model_cfgs["model_name"]
+        if model_name not in pytorch_model_dict:
+            raise NotImplementedError(
+                f"Error the model {model_name} was not found in the model dict. Please add it."
+            )
+        if self.pre_model is not None:
+            model = self._load_pretrain_model()
+        elif self.weight_path is not None:
+            # load model from pth file (saved weights and biases)
+            model = self._load_model_from_pth()
+        else:
+            model = pytorch_model_dict[model_name](**model_cfgs["model_hyperparam"])
+            # model_data = torch.load(weight_path)
+            # model.load_state_dict(model_data)
+        if torch.cuda.device_count() > 1 and len(self.device_num) > 1:
+            print("Let's use", torch.cuda.device_count(), "GPUs!")
+            which_first_tensor = self.cfgs["training_cfgs"]["which_first_tensor"]
+            sequece_first = which_first_tensor == "sequence"
+            parallel_dim = 1 if sequece_first else 0
+            model = nn.DataParallel(model, device_ids=self.device_num, dim=parallel_dim)
+        model.to(self.device)
+        return model
+
+    def _load_pretrain_model(self):
+        """load a pretrained model as the initial model"""
+        return self.pre_model
+
+    def _load_model_from_pth(self):
+        weight_path = self.weight_path
+        model_cfgs = self.cfgs["model_cfgs"]
+        model_name = model_cfgs["model_name"]
+        model = pytorch_model_dict[model_name](**model_cfgs["model_hyperparam"])
+        checkpoint = torch.load(weight_path, map_location=self.device)
+        model.load_state_dict(checkpoint)
+        print("Weights sucessfully loaded")
+        return model
+
+    def make_dataset(self, is_tra_val_te: str):
+        """
+        Initializes a pytorch dataset.
+
+        Parameters
+        ----------
+        is_tra_val_te
+            train or valid or test
+
+        Returns
+        -------
+        object
+            an object initializing from class in datasets_dict in data_dict.py
+        """
+        data_cfgs = self.cfgs["data_cfgs"]
+        dataset_name = data_cfgs["dataset"]
+
+        if dataset_name in list(datasets_dict.keys()):
+            dataset = datasets_dict[dataset_name](data_cfgs, is_tra_val_te)
+        else:
+            raise NotImplementedError(
+                f"Error the dataset {str(dataset_name)} was not found in the dataset dict. Please add it."
+            )
+        return dataset
+
+    def model_train(self) -> None:
+        """train a hydrological DL model"""
+        # A dictionary of the necessary parameters for training
+        training_cfgs = self.cfgs["training_cfgs"]
+        # The file path to load model weights from; defaults to "model_save"
+        model_filepath = self.cfgs["data_cfgs"]["test_path"]
+        data_cfgs = self.cfgs["data_cfgs"]
+        es = None
+        if training_cfgs["early_stopping"]:
+            es = EarlyStopper(training_cfgs["patience"])
+        criterion = self._get_loss_func(training_cfgs)
+        opt = self._get_optimizer(training_cfgs)
+        scheduler = self._get_scheduler(training_cfgs, opt)
+        max_epochs = training_cfgs["epochs"]
+        start_epoch = training_cfgs["start_epoch"]
+        # use PyTorch's DataLoader to load the data into batches in each epoch
+        data_loader, validation_data_loader = self._get_dataloader(
+            training_cfgs, data_cfgs
+        )
+        logger = TrainLogger(model_filepath, self.cfgs, opt)
+        for epoch in range(start_epoch, max_epochs + 1):
+            with logger.log_epoch_train(epoch) as train_logs:
+                total_loss, n_iter_ep = torch_single_train(
+                    self.model,
+                    opt,
+                    criterion,
+                    data_loader,
+                    device=self.device,
+                    which_first_tensor=training_cfgs["which_first_tensor"],
+                )
+                train_logs["train_loss"] = total_loss
+                train_logs["model"] = self.model
+
+            valid_loss = None
+            valid_metrics = None
+            if data_cfgs["t_range_valid"] is not None:
+                with logger.log_epoch_valid(epoch) as valid_logs:
+                    valid_loss, valid_metrics = self._1epoch_valid(
+                        training_cfgs, criterion, validation_data_loader, valid_logs
+                    )
+
+            self._scheduler_step(training_cfgs, scheduler, valid_loss)
+            logger.save_session_param(
+                epoch, total_loss, n_iter_ep, valid_loss, valid_metrics
+            )
+            logger.save_model_and_params(self.model, epoch, self.cfgs)
+            if es and not es.check_loss(
+                self.model,
+                valid_loss,
+                self.cfgs["data_cfgs"]["test_path"],
+            ):
+                print("Stopping model now")
+                break
+        # logger.plot_model_structure(self.model)
+        logger.tb.close()
+
+        # return the trained model weights and bias and the epoch loss
+        return self.model.state_dict(), sum(logger.epoch_loss) / len(logger.epoch_loss)
+
+    def _get_scheduler(self, training_cfgs, opt):
+        lr_scheduler_cfg = training_cfgs["lr_scheduler"]
+
+        if "lr" in lr_scheduler_cfg and "lr_factor" not in lr_scheduler_cfg:
+            scheduler = LambdaLR(opt, lr_lambda=lambda epoch: 1.0)
+        elif isinstance(lr_scheduler_cfg, dict) and all(
+            isinstance(epoch, int) for epoch in lr_scheduler_cfg
+        ):
+            scheduler = LambdaLR(
+                opt, lr_lambda=lambda epoch: lr_scheduler_cfg.get(epoch, 1.0)
+            )
+        elif "lr_factor" in lr_scheduler_cfg and "lr_patience" not in lr_scheduler_cfg:
+            scheduler = ExponentialLR(opt, gamma=lr_scheduler_cfg["lr_factor"])
+        elif "lr_factor" in lr_scheduler_cfg:
+            scheduler = ReduceLROnPlateau(
+                opt,
+                mode="min",
+                factor=lr_scheduler_cfg["lr_factor"],
+                patience=lr_scheduler_cfg["lr_patience"],
+            )
+        else:
+            raise ValueError("Invalid lr_scheduler configuration")
+
+        return scheduler
+
+    def _scheduler_step(self, training_cfgs, scheduler, valid_loss):
+        lr_scheduler_cfg = training_cfgs["lr_scheduler"]
+        required_keys = {"lr_factor", "lr_patience"}
+        if required_keys.issubset(lr_scheduler_cfg.keys()):
+            scheduler.step(valid_loss)
+        else:
+            scheduler.step()
+
+    def _1epoch_valid(
+        self, training_cfgs, criterion, validation_data_loader, valid_logs
+    ):
+        valid_obss_np, valid_preds_np, valid_loss = compute_validation(
+            self.model,
+            criterion,
+            validation_data_loader,
+            device=self.device,
+            which_first_tensor=training_cfgs["which_first_tensor"],
+        )
+        valid_logs["valid_loss"] = valid_loss
+        if self.cfgs["evaluation_cfgs"]["calc_metrics"]:
+            target_col = self.cfgs["data_cfgs"]["target_cols"]
+            valid_metrics = evaluate_validation(
+                validation_data_loader,
+                valid_preds_np,
+                valid_obss_np,
+                self.cfgs["evaluation_cfgs"],
+                target_col,
+            )
+            valid_logs["valid_metrics"] = valid_metrics
+            return valid_loss, valid_metrics
+        return valid_loss, None
+
+    def _get_trained_model(self):
+        model_loader = self.cfgs["evaluation_cfgs"]["model_loader"]
+        model_pth_dir = self.cfgs["data_cfgs"]["test_path"]
+        if model_loader["load_way"] == "specified":
+            test_epoch = model_loader["test_epoch"]
+            weight_path = os.path.join(model_pth_dir, f"model_Ep{str(test_epoch)}.pth")
+        elif model_loader["load_way"] == "best":
+            weight_path = os.path.join(model_pth_dir, "best_model.pth")
+        elif model_loader["load_way"] == "latest":
+            weight_path = get_lastest_file_in_a_dir(model_pth_dir)
+        elif model_loader["load_way"] == "pth":
+            weight_path = model_loader["pth_path"]
+        else:
+            raise ValueError("Invalid load_way")
+        return weight_path
+
+    def model_evaluate(self) -> Tuple[Dict, np.array, np.array]:
+        """
+        A function to evaluate a model, called at end of training.
+
+        Returns
+        -------
+        tuple[dict, np.array, np.array]
+            eval_log, denormalized predictions and observations
+        """
+        self.model = self.load_model(mode="infer")
+        preds_xr, obss_xr = self.inference()
+        return preds_xr, obss_xr
+
+    def inference(self) -> Tuple[torch.Tensor, torch.Tensor]:
+        """infer using trained model and unnormalized results"""
+        data_cfgs = self.cfgs["data_cfgs"]
+        training_cfgs = self.cfgs["training_cfgs"]
+        evaluation_cfgs = self.cfgs["evaluation_cfgs"]
+        device = get_the_device(self.cfgs["training_cfgs"]["device"])
+
+        ngrid = self.testdataset.ngrid
+        if data_cfgs["sampler"] == "HydroSampler":
+            test_num_samples = self.testdataset.num_samples
+            test_dataloader = DataLoader(
+                self.testdataset,
+                batch_size=test_num_samples // ngrid,
+                shuffle=False,
+                drop_last=False,
+                timeout=0,
+            )
+        else:
+            test_dataloader = DataLoader(
+                self.testdataset,
+                batch_size=training_cfgs["batch_size"],
+                shuffle=False,
+                sampler=None,
+                batch_sampler=None,
+                drop_last=False,
+                timeout=0,
+                worker_init_fn=None,
+            )
+        seq_first = training_cfgs["which_first_tensor"] == "sequence"
+        self.model.eval()
+        # here the batch is just an index of lookup table, so any batch size could be chosen
+        test_preds = []
+        obss = []
+        with torch.no_grad():
+            for xs, ys in test_dataloader:
+                # here the a batch doesn't mean a basin; it is only an index in lookup table
+                # for NtoN mode, only basin is index in lookup table, so the batch is same as basin
+                # for Nto1 mode, batch is only an index
+                ys, pred = model_infer(seq_first, device, self.model, xs, ys)
+                test_preds.append(pred.cpu().numpy())
+                obss.append(ys.cpu().numpy())
+            pred = reduce(lambda x, y: np.vstack((x, y)), test_preds)
+            obs = reduce(lambda x, y: np.vstack((x, y)), obss)
+        if pred.ndim == 2:
+            # TODO: check
+            # the ndim is 2 meaning we use an Nto1 mode
+            # as lookup table is (basin 1's all time length, basin 2's all time length, ...)
+            # params of reshape should be (basin size, time length)
+            pred = pred.flatten().reshape(test_dataloader.test_data.y.shape[0], -1, 1)
+            obs = obs.flatten().reshape(test_dataloader.test_data.y.shape[0], -1, 1)
+        # TODO: not support return_cell_states yet
+        return_cell_state = False
+        if return_cell_state:
+            return cellstates_when_inference(seq_first, data_cfgs, pred)
+
+        if not evaluation_cfgs["long_seq_pred"]:
+            target_len = len(data_cfgs["target_cols"])
+            prec_window = data_cfgs["prec_window"]
+            batch_size = test_dataloader.batch_size
+            if evaluation_cfgs["rolling"]:
+                forecast_length = data_cfgs["forecast_length"]
+                pred = pred[:, prec_window:, :].reshape(
+                    ngrid, batch_size, forecast_length, target_len
+                )
+                obs = obs[:, prec_window:, :].reshape(
+                    ngrid, batch_size, forecast_length, target_len
+                )
+
+                pred = pred[:, ::forecast_length, :, :]
+                obs = obs[:, ::forecast_length, :, :]
+
+                pred = np.concatenate(pred, axis=0).reshape(ngrid, -1, target_len)
+                obs = np.concatenate(obs, axis=0).reshape(ngrid, -1, target_len)
+
+                pred = pred[:, :batch_size, :]
+                obs = obs[:, :batch_size, :]
+            else:
+                pred = pred[:, prec_window, :].reshape(ngrid, batch_size, target_len)
+                obs = obs[:, prec_window, :].reshape(ngrid, batch_size, target_len)
+            pred_xr, obs_xr = denormalize4eval(
+                test_dataloader, pred, obs, long_seq_pred=False
+            )
+            fill_nan = evaluation_cfgs["fill_nan"]
+            eval_log = {}
+            for i, col in enumerate(data_cfgs["target_cols"]):
+                obs = obs_xr[col].to_numpy()
+                pred = pred_xr[col].to_numpy()
+                eval_log = calculate_and_record_metrics(
+                    obs,
+                    pred,
+                    evaluation_cfgs["metrics"],
+                    col,
+                    fill_nan[i] if isinstance(fill_nan, list) else fill_nan,
+                    eval_log,
+                )
+            test_log = f" Best Metric {eval_log}"
+            print(test_log)
+        else:
+            pred_xr, obs_xr = denormalize4eval(test_dataloader, pred, obs)
+        return pred_xr, obs_xr
+
+    def _get_optimizer(self, training_cfgs):
+        params_in_opt = self.model.parameters()
+        return pytorch_opt_dict[training_cfgs["optimizer"]](
+            params_in_opt, **training_cfgs["optim_params"]
+        )
+
+    def _get_loss_func(self, training_cfgs):
+        criterion_init_params = {}
+        if "criterion_params" in training_cfgs:
+            loss_param = training_cfgs["criterion_params"]
+            if loss_param is not None:
+                for key in loss_param.keys():
+                    if key == "loss_funcs":
+                        criterion_init_params[key] = pytorch_criterion_dict[
+                            loss_param[key]
+                        ]()
+                    else:
+                        criterion_init_params[key] = loss_param[key]
+        return pytorch_criterion_dict[training_cfgs["criterion"]](
+            **criterion_init_params
+        )
+
+    def _get_dataloader(self, training_cfgs, data_cfgs):
+        worker_num = 0
+        pin_memory = False
+        if "num_workers" in training_cfgs:
+            worker_num = training_cfgs["num_workers"]
+            print(f"using {str(worker_num)} workers")
+        if "pin_memory" in training_cfgs:
+            pin_memory = training_cfgs["pin_memory"]
+            print(f"Pin memory set to {str(pin_memory)}")
+        train_dataset: BaseDataset = self.traindataset
+        sampler = None
+        if data_cfgs["sampler"] is not None:
+            # now we only have one special sampler from Kuai Fang's Deep Learning papers
+            batch_size = data_cfgs["batch_size"]
+            rho = data_cfgs["forecast_history"]
+            warmup_length = data_cfgs["warmup_length"]
+            horizon = data_cfgs["forecast_length"]
+            ngrid = train_dataset.ngrid
+            nt = train_dataset.nt
+            if data_cfgs["sampler"] == "HydroSampler":
+                sampler = HydroSampler(train_dataset)
+            elif data_cfgs["sampler"] == "KuaiSampler":
+                sampler = KuaiSampler(
+                    train_dataset,
+                    batch_size=batch_size,
+                    warmup_length=warmup_length,
+                    rho_horizon=rho + horizon,
+                    ngrid=ngrid,
+                    nt=nt,
+                )
+            elif data_cfgs["sampler"] == "DistSampler":
+                sampler = DistributedSampler(train_dataset)
+            else:
+                raise NotImplementedError("This sampler not implemented yet")
+        data_loader = DataLoader(
+            train_dataset,
+            batch_size=training_cfgs["batch_size"],
+            shuffle=(sampler is None),
+            sampler=sampler,
+            num_workers=worker_num,
+            pin_memory=pin_memory,
+            timeout=0,
+        )
+        if data_cfgs["t_range_valid"] is not None:
+            valid_dataset: BaseDataset = self.validdataset
+            batch_size_valid = training_cfgs["batch_size"]
+            if data_cfgs["sampler"] == "HydroSampler":
+                # for HydroSampler when evaluating, we need to set new batch size
+                batch_size_valid = valid_dataset.num_samples // ngrid
+            validation_data_loader = DataLoader(
+                valid_dataset,
+                batch_size=batch_size_valid,
+                shuffle=False,
+                num_workers=worker_num,
+                pin_memory=pin_memory,
+                timeout=0,
+            )
+            return data_loader, validation_data_loader
+
+        return data_loader, None
+
+
+class FedLearnHydro(DeepHydro):
+    """Federated Learning Hydrological DL model"""
+
+    def __init__(self, cfgs: Dict):
+        super().__init__(cfgs)
+        # a user group which is a dict where the keys are the user index
+        # and the values are the corresponding data for each of those users
+        train_dataset = self.traindataset
+        fl_hyperparam = self.cfgs["model_cfgs"]["fl_hyperparam"]
+        # sample training data amongst users
+        if fl_hyperparam["fl_sample"] == "basin":
+            # Sample a basin for a user
+            user_groups = fl_sample_basin(train_dataset)
+        elif fl_hyperparam["fl_sample"] == "region":
+            # Sample a region for a user
+            user_groups = fl_sample_region(train_dataset)
+        else:
+            raise NotImplementedError()
+        self.user_groups = user_groups
+
+    @property
+    def num_users(self):
+        """number of users in federated learning"""
+        return len(self.user_groups)
+
+    def model_train(self) -> None:
+        # BUILD MODEL
+        global_model = self.model
+
+        # copy weights
+        global_weights = global_model.state_dict()
+
+        # Training
+        train_loss, train_accuracy = [], []
+        print_every = 2
+
+        training_cfgs = self.cfgs["training_cfgs"]
+        model_cfgs = self.cfgs["model_cfgs"]
+        max_epochs = training_cfgs["epochs"]
+        start_epoch = training_cfgs["start_epoch"]
+        fl_hyperparam = model_cfgs["fl_hyperparam"]
+        # total rounds in a FL system is max_epochs
+        for epoch in tqdm(range(start_epoch, max_epochs + 1)):
+            local_weights, local_losses = [], []
+            print(f"\n | Global Training Round : {epoch} |\n")
+
+            global_model.train()
+            m = max(int(fl_hyperparam["fl_frac"] * self.num_users), 1)
+            # randomly select m users, they will be the clients in this round
+            idxs_users = np.random.choice(range(self.num_users), m, replace=False)
+
+            for idx in idxs_users:
+                # each user will be used to train the model locally
+                # user_gourps[idx] means the idx of dataset for a user
+                user_cfgs = self._get_a_user_cfgs(idx)
+                local_model = DeepHydro(
+                    user_cfgs,
+                    pre_model=copy.deepcopy(global_model),
+                )
+                w, loss = local_model.model_train()
+                local_weights.append(copy.deepcopy(w))
+                local_losses.append(copy.deepcopy(loss))
+
+            # update global weights
+            global_weights = average_weights(local_weights)
+
+            # update global weights
+            global_model.load_state_dict(global_weights)
+
+            loss_avg = sum(local_losses) / len(local_losses)
+            train_loss.append(loss_avg)
+
+            # Calculate avg training accuracy over all users at every epoch
+            list_acc = []
+            global_model.eval()
+            for c in range(self.num_users):
+                one_user_cfg = self._get_a_user_cfgs(c)
+                local_model = DeepHydro(
+                    one_user_cfg,
+                    pre_model=global_model,
+                )
+                acc, _, _ = local_model.model_evaluate()
+                list_acc.append(acc)
+            values = [list(d.values())[0][0] for d in list_acc]
+            filtered_values = [v for v in values if not np.isnan(v)]
+            train_accuracy.append(sum(filtered_values) / len(filtered_values))
+
+            # print global training loss after every 'i' rounds
+            if (epoch + 1) % print_every == 0:
+                print(f" \nAvg Training Stats after {epoch+1} global rounds:")
+                print(f"Training Loss : {np.mean(np.array(train_loss))}")
+                print("Train Accuracy: {:.2f}% \n".format(100 * train_accuracy[-1]))
+
+    def _get_a_user_cfgs(self, idx):
+        """To get a user's configs for local training"""
+        user = self.user_groups[idx]
+
+        # update data_cfgs
+        # Use defaultdict to collect dates for each basin
+        basin_dates = defaultdict(list)
+
+        for _, (basin, time) in user.items():
+            basin_dates[basin].append(time)
+
+        # Initialize a list to store distinct basins
+        basins = []
+
+        # for each basin, we can find its date range
+        date_ranges = {}
+        for basin, times in basin_dates.items():
+            basins.append(basin)
+            date_ranges[basin] = (np.min(times), np.max(times))
+        # get the longest date range
+        longest_date_range = max(date_ranges.values(), key=lambda x: x[1] - x[0])
+        # transform the date range of numpy data into string
+        longest_date_range = [
+            np.datetime_as_string(dt, unit="D") for dt in longest_date_range
+        ]
+        user_cfgs = copy.deepcopy(self.cfgs)
+        # update data_cfgs
+        update_nested_dict(
+            user_cfgs, ["data_cfgs", "t_range_train"], longest_date_range
+        )
+        # for local training in FL, we don't need a validation set
+        update_nested_dict(user_cfgs, ["data_cfgs", "t_range_valid"], None)
+        # for local training in FL, we don't need a test set, but we should set one to avoid error
+        update_nested_dict(user_cfgs, ["data_cfgs", "t_range_test"], longest_date_range)
+        update_nested_dict(user_cfgs, ["data_cfgs", "object_ids"], basins)
+
+        # update training_cfgs
+        # we also need to update some training params for local training from FL settings
+        update_nested_dict(
+            user_cfgs,
+            ["training_cfgs", "epochs"],
+            user_cfgs["model_cfgs"]["fl_hyperparam"]["fl_local_ep"],
+        )
+        update_nested_dict(
+            user_cfgs,
+            ["evaluation_cfgs", "test_epoch"],
+            user_cfgs["model_cfgs"]["fl_hyperparam"]["fl_local_ep"],
+        )
+        # don't need to save model weights for local training
+        update_nested_dict(
+            user_cfgs,
+            ["training_cfgs", "save_epoch"],
+            None,
+        )
+        # there are two settings for batch size in configs, we need to update both of them
+        update_nested_dict(
+            user_cfgs,
+            ["training_cfgs", "batch_size"],
+            user_cfgs["model_cfgs"]["fl_hyperparam"]["fl_local_bs"],
+        )
+        update_nested_dict(
+            user_cfgs,
+            ["data_cfgs", "batch_size"],
+            user_cfgs["model_cfgs"]["fl_hyperparam"]["fl_local_bs"],
+        )
+
+        # update model_cfgs finally
+        # For local model, its model_type is Normal
+        update_nested_dict(user_cfgs, ["model_cfgs", "model_type"], "Normal")
+        update_nested_dict(
+            user_cfgs,
+            ["model_cfgs", "fl_hyperparam"],
+            None,
+        )
+        return user_cfgs
+
+
+class TransLearnHydro(DeepHydro):
+    def __init__(self, cfgs: Dict, pre_model=None):
+        super().__init__(cfgs, pre_model)
+
+    def load_model(self, mode="train"):
+        """Load model for transfer learning"""
+        model_cfgs = self.cfgs["model_cfgs"]
+        if self.weight_path is None and self.pre_model is None:
+            raise NotImplementedError(
+                "For transfer learning, we need a pre-trained model"
+            )
+        model = super().load_model(mode)
+        if (
+            "weight_path_add" in model_cfgs
+            and "freeze_params" in model_cfgs["weight_path_add"]
+        ):
+            freeze_params = model_cfgs["weight_path_add"]["freeze_params"]
+            for param in freeze_params:
+                exec(f"model.{param}.requires_grad = False")
+        return model
+
+    def _load_model_from_pth(self):
+        weight_path = self.weight_path
+        model_cfgs = self.cfgs["model_cfgs"]
+        model_name = model_cfgs["model_name"]
+        model = pytorch_model_dict[model_name](**model_cfgs["model_hyperparam"])
+        checkpoint = torch.load(weight_path, map_location=self.device)
+        if "weight_path_add" in model_cfgs:
+            if "excluded_layers" in model_cfgs["weight_path_add"]:
+                # delete some layers from source model if we don't need them
+                excluded_layers = model_cfgs["weight_path_add"]["excluded_layers"]
+                for layer in excluded_layers:
+                    del checkpoint[layer]
+                print("sucessfully deleted layers")
+            else:
+                print("directly loading identically-named layers of source model")
+        model.load_state_dict(checkpoint, strict=False)
+        print("Weights sucessfully loaded")
+        return model
+
+
+class MultiTaskHydro(DeepHydro):
+    def __init__(self, cfgs: Dict, pre_model=None):
+        super().__init__(cfgs, pre_model)
+
+    def _get_optimizer(self, training_cfgs):
+        params_in_opt = self.model.parameters()
+        if training_cfgs["criterion"] == "UncertaintyWeights":
+            # log_var = torch.zeros((1,), requires_grad=True)
+            log_vars = [
+                torch.zeros((1,), requires_grad=True, device=self.device)
+                for _ in range(training_cfgs["multi_targets"])
+            ]
+            params_in_opt = list(self.model.parameters()) + log_vars
+        return pytorch_opt_dict[training_cfgs["optimizer"]](
+            params_in_opt, **training_cfgs["optim_params"]
+        )
+
+    def _get_loss_func(self, training_cfgs):
+        if "criterion_params" in training_cfgs:
+            loss_param = training_cfgs["criterion_params"]
+            if loss_param is not None:
+                criterion_init_params = {
+                    key: (
+                        pytorch_criterion_dict[loss_param[key]]()
+                        if key == "loss_funcs"
+                        else loss_param[key]
+                    )
+                    for key in loss_param.keys()
+                }
+        if training_cfgs["criterion"] == "MultiOutWaterBalanceLoss":
+            # TODO: hard code for streamflow and ET
+            stat_dict = self.traindataset.target_scaler.stat_dict
+            stat_dict_keys = list(stat_dict.keys())
+            q_name = np.intersect1d(
+                [
+                    "usgsFlow",
+                    "streamflow",
+                    "Q",
+                    "qobs",
+                ],
+                stat_dict_keys,
+            )[0]
+            et_name = np.intersect1d(
+                [
+                    "ET",
+                    "LE",
+                    "GPP",
+                    "Ec",
+                    "Es",
+                    "Ei",
+                    "ET_water",
+                    # sum pf ET components in PML V2
+                    "ET_sum",
+                ],
+                stat_dict_keys,
+            )[0]
+            q_mean = self.training.target_scaler.stat_dict[q_name][2]
+            q_std = self.training.target_scaler.stat_dict[q_name][3]
+            et_mean = self.training.target_scaler.stat_dict[et_name][2]
+            et_std = self.training.target_scaler.stat_dict[et_name][3]
+            means = [q_mean, et_mean]
+            stds = [q_std, et_std]
+            criterion_init_params["means"] = means
+            criterion_init_params["stds"] = stds
+        return pytorch_criterion_dict[training_cfgs["criterion"]](
+            **criterion_init_params
+        )
+
+
+class DistributedDeepHydro(MultiTaskHydro):
+    def __init__(self, world_size, cfgs: Dict):
+        super().__init__(cfgs, cfgs["model_cfgs"]["weight_path"])
+        self.world_size = world_size
+
+    def setup(self, rank):
+        os.environ["MASTER_ADDR"] = self.cfgs["training_cfgs"]["master_addr"]
+        os.environ["MASTER_PORT"] = self.cfgs["training_cfgs"]["port"]
+        dist.init_process_group(
+            backend="nccl", init_method="env://", world_size=self.world_size, rank=rank
+        )
+        torch.cuda.set_device(rank)
+        self.device = torch.device(rank)
+        self.rank = rank
+
+    def cleanup(self):
+        dist.destroy_process_group()
+
+    def load_model(self, mode="train"):
+        if mode == "infer":
+            if self.weight_path is None:
+                # for continue training
+                self.weight_path = self._get_trained_model()
+        elif mode != "train":
+            raise ValueError("Invalid mode; must be 'train' or 'infer'")
+        model_cfgs = self.cfgs["model_cfgs"]
+        model_name = model_cfgs["model_name"]
+        if model_name not in pytorch_model_dict:
+            raise NotImplementedError(
+                f"Error the model {model_name} was not found in the model dict. Please add it."
+            )
+        if self.pre_model is not None:
+            return self._load_pretrain_model()
+        elif self.weight_path is not None:
+            # load model from pth file (saved weights and biases)
+            return self._load_model_from_pth()
+        else:
+            return pytorch_model_dict[model_name](**model_cfgs["model_hyperparam"])
+
+    def model_train(self):
+        model = self.load_model().to(self.device)
+        self.model = DDP(model, device_ids=[self.rank])
+        training_cfgs = self.cfgs["training_cfgs"]
+        # The file path to load model weights from; defaults to "model_save"
+        model_filepath = self.cfgs["data_cfgs"]["test_path"]
+        data_cfgs = self.cfgs["data_cfgs"]
+        es = None
+        if training_cfgs["early_stopping"]:
+            es = EarlyStopper(training_cfgs["patience"])
+        criterion = self._get_loss_func(training_cfgs)
+        opt = self._get_optimizer(training_cfgs)
+        scheduler = self._get_scheduler(training_cfgs, opt)
+        max_epochs = training_cfgs["epochs"]
+        start_epoch = training_cfgs["start_epoch"]
+        # use PyTorch's DataLoader to load the data into batches in each epoch
+        data_loader, validation_data_loader = self._get_dataloader(
+            training_cfgs, data_cfgs
+        )
+        logger = TrainLogger(model_filepath, self.cfgs, opt)
+        for epoch in range(start_epoch, max_epochs + 1):
+            data_loader.sampler.set_epoch(epoch)
+            with logger.log_epoch_train(epoch) as train_logs:
+                total_loss, n_iter_ep = torch_single_train(
+                    self.model,
+                    opt,
+                    criterion,
+                    data_loader,
+                    device=self.device,
+                    which_first_tensor=training_cfgs["which_first_tensor"],
+                )
+                train_logs["train_loss"] = total_loss
+                train_logs["model"] = self.model
+
+            valid_loss = None
+            valid_metrics = None
+            if data_cfgs["t_range_valid"] is not None:
+                with logger.log_epoch_valid(epoch) as valid_logs:
+                    valid_loss, valid_metrics = self._1epoch_valid(
+                        training_cfgs, criterion, validation_data_loader, valid_logs
+                    )
+
+            self._scheduler_step(training_cfgs, scheduler, valid_loss)
+            logger.save_session_param(
+                epoch, total_loss, n_iter_ep, valid_loss, valid_metrics
+            )
+            logger.save_model_and_params(self.model, epoch, self.cfgs)
+            if es and not es.check_loss(
+                self.model,
+                valid_loss,
+                self.cfgs["data_cfgs"]["test_path"],
+            ):
+                print("Stopping model now")
+                break
+        # if self.rank == 0:
+        # logging.log(1, f"Training complete in: {time.time() - start_time:.2f} seconds"
+
+    def run(self):
+        self.setup(self.rank)
+        self.model_train()
+        self.model_evaluate()
+        self.cleanup()
+
+
+def train_worker(rank, world_size, cfgs):
+    trainer = DistributedDeepHydro(world_size, cfgs)
+    trainer.rank = rank
+    trainer.run()
+
+
+model_type_dict = {
+    "Normal": DeepHydro,
+    "FedLearn": FedLearnHydro,
+    "TransLearn": TransLearnHydro,
+    "MTL": MultiTaskHydro,
+    "DDP_MTL": DistributedDeepHydro,
+}
```

### Comparing `torchhydro-0.0.4/torchhydro.egg-info/SOURCES.txt` & `torchhydro-0.0.5/torchhydro.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -2,21 +2,34 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
 tests/test_caravan_train.py
-tests/test_data.py
+tests/test_data_sets.py
+tests/test_data_utils.py
+tests/test_deep_hydro.py
 tests/test_dpl4xaj.py
 tests/test_ensemble_exps.py
+tests/test_evaluate_grid_lstm.py
 tests/test_evaluate_model.py
+tests/test_evaluate_seq2seq.py
 tests/test_federated_learning.py
-tests/test_tl_opendata.py
+tests/test_model.py
+tests/test_pretrain_dataenhanced.py
+tests/test_pretrain_datafusion.py
+tests/test_sampler.py
+tests/test_tl_selfmadedata.py
 tests/test_train_camels_lstm.py
+tests/test_train_camelspro_mtl.py
+tests/test_train_grid_lstm.py
+tests/test_train_mean_lstm.py
+tests/test_train_seq2seq.py
+tests/test_train_with_gpm.py
 tests/test_transfer_learning.py
 tests/test_weight_analysis.py
 torchhydro/__init__.py
 torchhydro.egg-info/PKG-INFO
 torchhydro.egg-info/SOURCES.txt
 torchhydro.egg-info/dependency_links.txt
 torchhydro.egg-info/entry_points.txt
@@ -41,13 +54,16 @@
 torchhydro/models/crits.py
 torchhydro/models/cudnnlstm.py
 torchhydro/models/dpl4xaj.py
 torchhydro/models/dropout.py
 torchhydro/models/kernel_conv.py
 torchhydro/models/model_dict_function.py
 torchhydro/models/model_utils.py
+torchhydro/models/seq2seq.py
 torchhydro/models/simple_lstm.py
+torchhydro/models/spplstm.py
 torchhydro/trainers/__init__.py
 torchhydro/trainers/deep_hydro.py
+torchhydro/trainers/resulter.py
 torchhydro/trainers/train_logger.py
 torchhydro/trainers/train_utils.py
 torchhydro/trainers/trainer.py
```

