# Comparing `tmp/pimms-learn-0.2.0.tar.gz` & `tmp/pimms_learn-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pimms-learn-0.2.0.tar", last modified: Tue Dec 12 15:52:40 2023, max compression
+gzip compressed data, was "pimms_learn-0.3.0.tar", last modified: Mon May  6 11:28:14 2024, max compression
```

## Comparing `pimms-learn-0.2.0.tar` & `pimms_learn-0.3.0.tar`

### file list

```diff
@@ -1,68 +1,382 @@
-drwxrwxrwx   0        0        0        0 2023-12-12 15:52:40.594267 pimms-learn-0.2.0/
--rw-rw-rw-   0        0        0    12118 2023-12-12 15:52:40.593266 pimms-learn-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    11005 2023-12-12 15:46:07.000000 pimms-learn-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-12-12 15:52:40.590263 pimms-learn-0.2.0/pimms_learn.egg-info/
--rw-rw-rw-   0        0        0    12118 2023-12-12 15:52:40.000000 pimms-learn-0.2.0/pimms_learn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1285 2023-12-12 15:52:40.000000 pimms-learn-0.2.0/pimms_learn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-12 15:52:40.000000 pimms-learn-0.2.0/pimms_learn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      160 2023-12-12 15:52:40.000000 pimms-learn-0.2.0/pimms_learn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-12-12 15:52:40.000000 pimms-learn-0.2.0/pimms_learn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-09-06 16:01:02.000000 pimms-learn-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0     1311 2023-12-12 15:52:40.597265 pimms-learn-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-09-28 13:06:54.000000 pimms-learn-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-12 15:52:40.537879 pimms-learn-0.2.0/vaep/
--rw-rw-rw-   0        0        0      966 2023-12-12 15:49:41.000000 pimms-learn-0.2.0/vaep/__init__.py
--rw-rw-rw-   0        0        0      273 2023-09-18 09:34:48.000000 pimms-learn-0.2.0/vaep/__main__.py
-drwxrwxrwx   0        0        0        0 2023-12-12 15:52:40.544360 pimms-learn-0.2.0/vaep/analyzers/
--rw-rw-rw-   0        0        0      215 2023-09-18 09:34:50.000000 pimms-learn-0.2.0/vaep/analyzers/__init__.py
--rw-rw-rw-   0        0        0    20731 2023-10-17 08:29:11.000000 pimms-learn-0.2.0/vaep/analyzers/analyzers.py
--rw-rw-rw-   0        0        0     2867 2023-09-18 09:34:49.000000 pimms-learn-0.2.0/vaep/analyzers/compare_predictions.py
--rw-rw-rw-   0        0        0     1363 2023-09-18 09:34:49.000000 pimms-learn-0.2.0/vaep/analyzers/diff_analysis.py
--rw-rw-rw-   0        0        0     1956 2023-09-06 16:01:02.000000 pimms-learn-0.2.0/vaep/data_handling.py
-drwxrwxrwx   0        0        0        0 2023-12-12 15:52:40.546360 pimms-learn-0.2.0/vaep/databases/
--rw-rw-rw-   0        0        0        0 2023-10-16 13:09:42.000000 pimms-learn-0.2.0/vaep/databases/__init__.py
--rw-rw-rw-   0        0        0      731 2023-09-15 15:14:19.000000 pimms-learn-0.2.0/vaep/databases/diseases.py
--rw-rw-rw-   0        0        0     9256 2023-09-06 16:01:02.000000 pimms-learn-0.2.0/vaep/imputation.py
-drwxrwxrwx   0        0        0        0 2023-12-12 15:52:40.557361 pimms-learn-0.2.0/vaep/io/
--rw-rw-rw-   0        0        0     4994 2023-09-18 09:34:54.000000 pimms-learn-0.2.0/vaep/io/__init__.py
--rw-rw-rw-   0        0        0     5387 2023-09-18 09:34:50.000000 pimms-learn-0.2.0/vaep/io/dataloaders.py
--rw-rw-rw-   0        0        0     6431 2023-09-18 09:34:51.000000 pimms-learn-0.2.0/vaep/io/datasets.py
--rw-rw-rw-   0        0        0     8198 2023-09-18 09:34:51.000000 pimms-learn-0.2.0/vaep/io/datasplits.py
--rw-rw-rw-   0        0        0     1089 2023-09-18 09:34:52.000000 pimms-learn-0.2.0/vaep/io/format.py
--rw-rw-rw-   0        0        0      247 2023-09-18 09:34:53.000000 pimms-learn-0.2.0/vaep/io/test_logging.py
--rw-rw-rw-   0        0        0      884 2023-09-18 09:34:53.000000 pimms-learn-0.2.0/vaep/io/types.py
--rw-rw-rw-   0        0        0     2217 2023-10-12 12:49:30.000000 pimms-learn-0.2.0/vaep/logging.py
--rw-rw-rw-   0        0        0     5236 2023-09-18 09:34:47.000000 pimms-learn-0.2.0/vaep/model.py
-drwxrwxrwx   0        0        0        0 2023-12-12 15:52:40.567362 pimms-learn-0.2.0/vaep/models/
--rw-rw-rw-   0        0        0    10582 2023-09-18 09:34:55.000000 pimms-learn-0.2.0/vaep/models/__init__.py
--rw-rw-rw-   0        0        0    14414 2023-09-18 09:34:54.000000 pimms-learn-0.2.0/vaep/models/ae.py
--rw-rw-rw-   0        0        0      417 2023-09-18 08:13:48.000000 pimms-learn-0.2.0/vaep/models/analysis.py
--rw-rw-rw-   0        0        0     1585 2023-09-18 09:34:54.000000 pimms-learn-0.2.0/vaep/models/cmd.py
--rw-rw-rw-   0        0        0     8241 2023-09-28 13:06:54.000000 pimms-learn-0.2.0/vaep/models/collab.py
--rw-rw-rw-   0        0        0     1742 2023-09-18 09:34:55.000000 pimms-learn-0.2.0/vaep/models/collect_dumps.py
--rw-rw-rw-   0        0        0     4056 2023-09-18 09:34:55.000000 pimms-learn-0.2.0/vaep/models/vae.py
--rw-rw-rw-   0        0        0     3904 2023-09-18 09:34:48.000000 pimms-learn-0.2.0/vaep/nb.py
--rw-rw-rw-   0        0        0     3018 2023-09-18 09:34:48.000000 pimms-learn-0.2.0/vaep/normalization.py
-drwxrwxrwx   0        0        0        0 2023-12-12 15:52:40.572265 pimms-learn-0.2.0/vaep/pandas/
--rw-rw-rw-   0        0        0     9298 2023-10-16 13:09:42.000000 pimms-learn-0.2.0/vaep/pandas/__init__.py
--rw-rw-rw-   0        0        0     1341 2023-09-06 16:01:02.000000 pimms-learn-0.2.0/vaep/pandas/calc_errors.py
--rw-rw-rw-   0        0        0      925 2023-09-18 09:34:55.000000 pimms-learn-0.2.0/vaep/pandas/missing_data.py
-drwxrwxrwx   0        0        0        0 2023-12-12 15:52:40.580263 pimms-learn-0.2.0/vaep/plotting/
--rw-rw-rw-   0        0        0    11102 2023-11-26 17:19:14.000000 pimms-learn-0.2.0/vaep/plotting/__init__.py
--rw-rw-rw-   0        0        0    11426 2023-12-09 11:54:02.000000 pimms-learn-0.2.0/vaep/plotting/data.py
--rw-rw-rw-   0        0        0     4003 2023-11-27 09:07:59.000000 pimms-learn-0.2.0/vaep/plotting/defaults.py
--rw-rw-rw-   0        0        0     4581 2023-11-28 15:51:50.000000 pimms-learn-0.2.0/vaep/plotting/errors.py
--rw-rw-rw-   0        0        0     1015 2022-10-31 12:26:49.000000 pimms-learn-0.2.0/vaep/plotting/metrics.py
--rw-rw-rw-   0        0        0     1651 2023-09-06 16:01:02.000000 pimms-learn-0.2.0/vaep/plotting/plotly.py
--rw-rw-rw-   0        0        0     3608 2023-09-18 09:34:48.000000 pimms-learn-0.2.0/vaep/sampling.py
-drwxrwxrwx   0        0        0        0 2023-12-12 15:52:40.585264 pimms-learn-0.2.0/vaep/sklearn/
--rw-rw-rw-   0        0        0     3033 2023-09-06 16:01:02.000000 pimms-learn-0.2.0/vaep/sklearn/__init__.py
--rw-rw-rw-   0        0        0     4946 2023-09-06 16:01:02.000000 pimms-learn-0.2.0/vaep/sklearn/ae_transformer.py
--rw-rw-rw-   0        0        0     6112 2023-09-06 16:01:02.000000 pimms-learn-0.2.0/vaep/sklearn/cf_transformer.py
--rw-rw-rw-   0        0        0     1169 2023-09-06 16:01:02.000000 pimms-learn-0.2.0/vaep/sklearn/types.py
-drwxrwxrwx   0        0        0        0 2023-12-12 15:52:40.588264 pimms-learn-0.2.0/vaep/stats/
--rw-rw-rw-   0        0        0       28 2023-09-18 09:34:58.000000 pimms-learn-0.2.0/vaep/stats/__init__.py
--rw-rw-rw-   0        0        0     3836 2023-09-18 09:34:58.000000 pimms-learn-0.2.0/vaep/stats/diff_analysis.py
--rw-rw-rw-   0        0        0     2006 2023-09-18 09:34:48.000000 pimms-learn-0.2.0/vaep/tf_board.py
--rw-rw-rw-   0        0        0     6421 2023-09-18 09:34:48.000000 pimms-learn-0.2.0/vaep/transform.py
--rw-rw-rw-   0        0        0     2562 2023-10-16 13:09:42.000000 pimms-learn-0.2.0/vaep/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.945059 pimms_learn-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.869059 pimms_learn-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.881059 pimms_learn-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/.github/workflows/workflow_website.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12562 2024-05-06 11:28:14.945059 pimms_learn-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11258 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.881059 pimms_learn-0.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.885059 pimms_learn-0.3.0/docs/Figures/
+-rw-r--r--   0 runner    (1001) docker     (127)   644446 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/docs/Figures/Molecular_structures_of_the_21_proteinogenic_amino_acids.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   250559 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/docs/Figures/amino_acids_iupac_iub_1983.png
+-rw-r--r--   0 runner    (1001) docker     (127)   192389 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/docs/Figures/fig_proteomics_pipeline.png
+-rw-r--r--   0 runner    (1001) docker     (127)   211649 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/docs/Figures/schema_orbitrap_instrument.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/docs/docutils.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.885059 pimms_learn-0.3.0/docs/other/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/docs/other/project_readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/docs/other/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/docs/proteomics_intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/docs/venv_setup.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.945059 pimms_learn-0.3.0/pimms_learn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12562 2024-05-06 11:28:14.000000 pimms_learn-0.3.0/pimms_learn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13012 2024-05-06 11:28:14.000000 pimms_learn-0.3.0/pimms_learn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 11:28:14.000000 pimms_learn-0.3.0/pimms_learn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-06 11:28:14.000000 pimms_learn-0.3.0/pimms_learn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-06 11:28:14.000000 pimms_learn-0.3.0/pimms_learn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 11:28:14.000000 pimms_learn-0.3.0/pimms_learn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.901059 pimms_learn-0.3.0/project/
+-rw-r--r--   0 runner    (1001) docker     (127)    17364 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/00_5_training_data_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/00_6_0_permute_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/00_6_0_permute_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/00_8_add_random_missing_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47909 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/01_0_split_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    30864 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/01_0_split_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/01_0_transform_data_to_wide_format.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/01_0_transform_data_to_wide_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18462 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/01_1_train_CF.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9261 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/01_1_train_CF.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22918 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/01_1_train_DAE.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/01_1_train_DAE.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12830 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/01_1_train_KNN.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/01_1_train_KNN.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15698 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/01_1_train_Median.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8074 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/01_1_train_Median.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12734 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/01_1_train_NAGuideR_methods.R
+-rw-r--r--   0 runner    (1001) docker     (127)    19707 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/01_1_train_NAGuideR_methods.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13256 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/01_1_train_RSN.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/01_1_train_RSN.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26488 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/01_1_train_VAE.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12898 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/01_1_train_VAE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8814 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/01_1_transfer_NAGuideR_pred.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/01_1_transfer_NAGuideR_pred.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44144 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/01_2_performance_plots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24429 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/01_2_performance_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/02_1_aggregate_metrics.py.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/02_1_aggregate_metrics.py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/02_1_join_metrics.py.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/02_1_join_metrics.py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/02_2_aggregate_configs.py.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/02_2_aggregate_configs.py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/02_2_join_configs.py.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/02_2_join_configs.py.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52319 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/02_3_grid_search_analysis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    28743 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/02_3_grid_search_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22768 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/02_4_best_models_over_all_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13422 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/02_4_best_models_over_all_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/03_1_best_models_comparison.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/03_1_best_models_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/03_2_best_models_comparison_fig2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/03_2_best_models_comparison_fig2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/03_3_combine_experiment_result_tables.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/03_3_combine_experiment_result_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/03_4_join_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/03_5_join_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/03_6_setup_comparison_rev3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7944 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/04_1_train_DAE_VAE_wo_val_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/04_1_train_DAE_VAE_wo_val_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17938 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/04_1_train_pimms_models.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9354 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/04_1_train_pimms_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54653 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/10_0_ald_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24479 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/10_0_ald_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/10_0_ald_data_3v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20024 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/10_1_ald_diff_analysis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/10_1_ald_diff_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23443 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/10_2_ald_compare_methods.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/10_2_ald_compare_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20429 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/10_3_ald_ml_new_feat.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12040 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/10_3_ald_ml_new_feat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22801 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/10_4_ald_compare_single_pg.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13609 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/10_4_ald_compare_single_pg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10414 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/10_5_comp_diff_analysis_repetitions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/10_5_comp_diff_analysis_repetitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/10_6_interpret_repeated_ald_da.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/10_7_ald_reduced_dataset_plots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/10_7_ald_reduced_dataset_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.901059 pimms_learn-0.3.0/project/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/bin/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1437 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/bin/create_qsub_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/bin/run_snakemake.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/bin/run_snakemake_cluster.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.901059 pimms_learn-0.3.0/project/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.901059 pimms_learn-0.3.0/project/config/across_datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/across_datasets/collab.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/across_datasets/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/across_datasets/dae.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/across_datasets/shared_splits.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/across_datasets/vae.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/ald_data.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.873059 pimms_learn-0.3.0/project/config/appl_ald_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.873059 pimms_learn-0.3.0/project/config/appl_ald_data/plasma/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.901059 pimms_learn-0.3.0/project/config/appl_ald_data/plasma/aggPeptides/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/appl_ald_data/plasma/aggPeptides/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/appl_ald_data/plasma/aggPeptides/split.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/appl_ald_data/plasma/aggPeptides/train.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.901059 pimms_learn-0.3.0/project/config/appl_ald_data/plasma/grid_search/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/appl_ald_data/plasma/grid_search/config_grid.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.905059 pimms_learn-0.3.0/project/config/appl_ald_data/plasma/proteinGroups/
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/appl_ald_data/plasma/proteinGroups/comparison.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/appl_ald_data/plasma/proteinGroups/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/appl_ald_data/plasma/proteinGroups/config_reps.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/appl_ald_data/plasma/proteinGroups/inspect_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/appl_ald_data/plasma/proteinGroups/split.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/appl_ald_data/plasma/proteinGroups/train_CF.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/appl_ald_data/plasma/proteinGroups/train_DAE.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/appl_ald_data/plasma/proteinGroups/train_KNN.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/appl_ald_data/plasma/proteinGroups/train_Median.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/appl_ald_data/plasma/proteinGroups/train_RSN.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/appl_ald_data/plasma/proteinGroups/train_VAE.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.905059 pimms_learn-0.3.0/project/config/appl_ald_data/plasma/proteinGroups_80perc_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/appl_ald_data/plasma/proteinGroups_80perc_dataset/comparison.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/appl_ald_data/plasma/proteinGroups_80perc_dataset/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/appl_ald_data/plasma/proteinGroups_80perc_dataset/split.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/erda_dumps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.905059 pimms_learn-0.3.0/project/config/grid_search_large_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/grid_search_large_data/config_grid.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/grid_search_large_data/config_grid_small.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/grid_search_large_data/evidence_split.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/grid_search_large_data/peptides_split.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/grid_search_large_data/proteinGroups_split.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.905059 pimms_learn-0.3.0/project/config/grid_search_small_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/grid_search_small_data/config_grid.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/grid_search_small_data/evidence_split.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/grid_search_small_data/peptides_split.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/grid_search_small_data/proteinGroups_split.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.873059 pimms_learn-0.3.0/project/config/knn_comparison/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.905059 pimms_learn-0.3.0/project/config/knn_comparison/ald_pgs_all/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/knn_comparison/ald_pgs_all/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/knn_comparison/ald_pgs_all/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.909059 pimms_learn-0.3.0/project/config/knn_comparison/hela_pgs_large/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/knn_comparison/hela_pgs_large/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/knn_comparison/hela_pgs_large/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/knn_comparison/hela_pgs_large/inspect_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/knn_comparison/hela_pgs_large/split.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.909059 pimms_learn-0.3.0/project/config/permuted_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/permuted_dataset/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/permuted_dataset/split.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.909059 pimms_learn-0.3.0/project/config/repeat_best/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/repeat_best/split.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/repeat_best/train.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.873059 pimms_learn-0.3.0/project/config/single_dev_dataset/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.909059 pimms_learn-0.3.0/project/config/single_dev_dataset/evidence/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/evidence/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/evidence/split.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/evidence/train_CF.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/evidence/train_DAE.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/evidence/train_KNN.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/evidence/train_Median.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/evidence/train_VAE.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.909059 pimms_learn-0.3.0/project/config/single_dev_dataset/evidence_N50/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/evidence_N50/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/evidence_N50/split.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/evidence_N50/train_CF.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/evidence_N50/train_DAE.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/evidence_N50/train_KNN.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/evidence_N50/train_Median.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/evidence_N50/train_VAE.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.913059 pimms_learn-0.3.0/project/config/single_dev_dataset/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/example/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/example/split.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/example/train_CF.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/example/train_DAE.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/example/train_KNN.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/example/train_Median.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/example/train_RSN.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/example/train_VAE.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.913059 pimms_learn-0.3.0/project/config/single_dev_dataset/mnar_mcar/
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/mnar_mcar/evi_l.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2390 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/mnar_mcar/evi_m.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/mnar_mcar/pep_l.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2120 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/mnar_mcar/pep_m.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2015 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/mnar_mcar/pg_l.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/mnar_mcar/pg_m.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.913059 pimms_learn-0.3.0/project/config/single_dev_dataset/peptides/
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/peptides/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/peptides/split.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/peptides/train_CF.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/peptides/train_DAE.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/peptides/train_KNN.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/peptides/train_Median.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/peptides/train_VAE.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.917059 pimms_learn-0.3.0/project/config/single_dev_dataset/peptides_N50/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/peptides_N50/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/peptides_N50/split.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/peptides_N50/train_CF.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/peptides_N50/train_DAE.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/peptides_N50/train_KNN.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/peptides_N50/train_Median.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/peptides_N50/train_VAE.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.917059 pimms_learn-0.3.0/project/config/single_dev_dataset/proteinGroups/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/proteinGroups/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/proteinGroups/inspect_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/proteinGroups/split.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/proteinGroups/train_CF.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/proteinGroups/train_DAE.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/proteinGroups/train_KNN.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/proteinGroups/train_Median.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/proteinGroups/train_VAE.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.917059 pimms_learn-0.3.0/project/config/single_dev_dataset/proteinGroups_N50/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/proteinGroups_N50/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/proteinGroups_N50/config_v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/proteinGroups_N50/split.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/proteinGroups_N50/train_CF.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/proteinGroups_N50/train_DAE.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/proteinGroups_N50/train_KNN.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/proteinGroups_N50/train_Median.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/config/single_dev_dataset/proteinGroups_N50/train_VAE.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.917059 pimms_learn-0.3.0/project/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.921059 pimms_learn-0.3.0/project/data/ALD_study/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/data/ALD_study/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/data/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.873059 pimms_learn-0.3.0/project/data/dev_datasets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.925059 pimms_learn-0.3.0/project/data/dev_datasets/HeLa_6070/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/data/dev_datasets/HeLa_6070/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/data/dev_datasets/HeLa_6070/files_selected_metadata_N50.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2314772 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/data/dev_datasets/HeLa_6070/protein_groups_wide_N50.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   122763 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/data/dev_datasets/HeLa_6070/protein_groups_wide_N50_M227.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   231185 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/data/dev_datasets/HeLa_6070/protein_groups_wide_N50_M454.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    21037 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/data/mqpar_example.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/jupytext.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/misc_embeddings.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/misc_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/misc_illustrations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/misc_illustrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/misc_json_formats.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/misc_json_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21269 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/misc_pytorch_fastai_dataloaders.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11211 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/misc_pytorch_fastai_dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/misc_pytorch_fastai_dataset.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/misc_pytorch_fastai_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8313 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/misc_sampling_in_pandas.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/misc_sampling_in_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.873059 pimms_learn-0.3.0/project/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.925059 pimms_learn-0.3.0/project/src/R_NAGuideR/
+-rw-r--r--   0 runner    (1001) docker     (127)   142758 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/src/R_NAGuideR/GMSimpute_0.0.1.1.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/src/R_NAGuideR/GSimp.R
+-rw-r--r--   0 runner    (1001) docker     (127)    13784 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/src/R_NAGuideR/Imput_funcs.r
+-rw-r--r--   0 runner    (1001) docker     (127)   936661 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/src/R_NAGuideR/SeqKnn_1.0.1.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.929059 pimms_learn-0.3.0/project/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)    19704 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/tutorials/pandas_categorical.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/tutorials/pandas_multiindex.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.929059 pimms_learn-0.3.0/project/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/workflow/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/workflow/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/workflow/Snakefile_ald_comparison.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/workflow/Snakefile_ald_comparison_repeated.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/workflow/Snakefile_best_across_datasets.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/workflow/Snakefile_best_repeated_split.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/workflow/Snakefile_best_repeated_train.smk
+-rw-r--r--   0 runner    (1001) docker     (127)    12604 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/workflow/Snakefile_grid.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/workflow/Snakefile_small_N.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/workflow/Snakefile_v2
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/workflow/TestNotebooks.smk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.929059 pimms_learn-0.3.0/project/workflow/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/workflow/bin/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      863 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/workflow/bin/qsub-status.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      947 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/workflow/bin/qsub-status_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.929059 pimms_learn-0.3.0/project/workflow/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/workflow/notebooks/best_repeated_split_collect_metrics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/workflow/notebooks/best_repeated_split_collect_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/workflow/notebooks/best_repeated_train_collect_metrics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/workflow/notebooks/best_repeated_train_collect_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.933059 pimms_learn-0.3.0/project/workflow/rulegraphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7686 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/workflow/rulegraphs/default.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9365 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/workflow/rulegraphs/rulegraph_ald_comparison.png
+-rw-r--r--   0 runner    (1001) docker     (127)    77942 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/project/workflow/rulegraphs/rulegraph_gridsearch.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/requirements_R.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-06 11:28:14.945059 pimms_learn-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.937059 pimms_learn-0.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.937059 pimms_learn-0.3.0/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/tests/io/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/tests/io/test_data_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/tests/io/test_dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8677 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/tests/io/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/tests/io/test_datasplits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.877059 pimms_learn-0.3.0/tests/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.937059 pimms_learn-0.3.0/tests/models/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/tests/models/__pycache__/test_collect_dumps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.937059 pimms_learn-0.3.0/tests/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/tests/pandas/test_calc_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.937059 pimms_learn-0.3.0/tests/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/tests/plotting/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/tests/random_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/tests/test_ae.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/tests/test_collab.py
+-rw-r--r--   0 runner    (1001) docker     (127)   793607 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/tests/test_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/tests/test_imputation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/tests/test_nb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/tests/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/tests/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/tests/test_transfrom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.937059 pimms_learn-0.3.0/vaep/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.937059 pimms_learn-0.3.0/vaep/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19054 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/analyzers/analyzers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/analyzers/compare_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/analyzers/diff_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.941059 pimms_learn-0.3.0/vaep/cmd_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/cmd_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/cmd_interface/setup_imp_cp_website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/data_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.941059 pimms_learn-0.3.0/vaep/databases/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/databases/diseases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9005 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/imputation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.941059 pimms_learn-0.3.0/vaep/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/io/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/io/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/io/datasplits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/io/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/io/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/io/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.941059 pimms_learn-0.3.0/vaep/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/models/ae.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/models/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/models/collab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/models/collect_dumps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/models/vae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/nb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.941059 pimms_learn-0.3.0/vaep/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)     8816 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/pandas/calc_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/pandas/missing_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.945059 pimms_learn-0.3.0/vaep/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)    10846 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/plotting/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/plotting/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/plotting/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/plotting/plotly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8323 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.945059 pimms_learn-0.3.0/vaep/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/sklearn/ae_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/sklearn/cf_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:14.945059 pimms_learn-0.3.0/vaep/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-06 11:28:03.000000 pimms_learn-0.3.0/vaep/utils.py
```

### Comparing `pimms-learn-0.2.0/PKG-INFO` & `pimms_learn-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,265 +1,270 @@
-Metadata-Version: 2.1
-Name: pimms-learn
-Version: 0.2.0
-Summary: Imputing (MS-based prote-) omics data using self supervised deep learning models
-Home-page: https://github.com/RasmussenLab/pimms
-Author: Henry Webel
-Author-email: "Henry Webel" <henry.webel@cpr.ku.dk>
-License: gpl-3.0
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Intended Audience :: Healthcare Industry
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Description-Content-Type: text/markdown
-Requires-Dist: numpy
-Requires-Dist: matplotlib
-Requires-Dist: pandas
-Requires-Dist: plotly
-Requires-Dist: torch
-Requires-Dist: scikit-learn>=1.0
-Requires-Dist: scipy
-Requires-Dist: seaborn
-Requires-Dist: fastai
-Requires-Dist: omegaconf
-Requires-Dist: tqdm
-Requires-Dist: mrmr-selection
-Requires-Dist: pingouin
-Provides-Extra: docs
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: sphinx-book-theme; extra == "docs"
-Requires-Dist: myst-parser; extra == "docs"
-
-# PIMMS
-
-PIMMS stands for Proteomics Imputation Modeling Mass Spectrometry 
-and is a hommage to our dear British friends 
-who are missing as part of the EU for far too long already
-(Pimms is also a British summer drink).
-
-The pre-print is available [on biorxiv](https://doi.org/10.1101/2023.01.12.523792).
-
-
-> `PIMMS` was called `vaep` during development.  
-> Before entire refactoring has to been completed the imported package will be
-`vaep`.
-
-We provide functionality as a python package, an excutable workflow and notebooks.
-
-The models can be used with the scikit-learn interface in the spirit of other scikit-learn imputers. You can try this in colab. [![open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RasmussenLab/pimms/blob/dev/project/04_1_train_pimms_models.ipynb)
-
-
-## Python package
-
-For interactive use of the models provided in PIMMS, you can use our
-[python package `pimms-learn`](https://pypi.org/project/pimms-learn/).
-The interface is similar to scikit-learn.
-
-
-```
-pip install pimms-learn
-```
-
-
-Then you can use the models on a pandas DataFrame with missing values. Try this in the tutorial on Colab:
-[![open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RasmussenLab/pimms/blob/dev/project/04_1_train_pimms_models.ipynb)
-
-## Notebooks as scripts using papermill
-
-If you want to run a model on your prepared data, you can run notebooks prefixed with 
-`01_`, i.e. [`project/01_*.ipynb`](https://github.com/RasmussenLab/pimms/tree/HEAD/project) after cloning the repository. Using jupytext also python percentage script versions
-are saved.
-
-```
-cd project # project folder as pwd
-papermill 01_0_split_data.ipynb --help-notebook
-papermill 01_1_train_vae.ipynb --help-notebook
-```
-
-> Misstyped argument names won't throw an error when using papermill
-
-
-
-
-## Setup for PIMMS comparison workflow
-
-The package is available as a standalone software on pypi. However, running the entire snakemake workflow in enabled using 
-conda (or mamba) and pip to setup the environment. For a detailed description of setting up
-conda (or mamba), see [instructions on setting up a virtual environment](https://github.com/RasmussenLab/pimms/blob/HEAD/docs/venv_setup.md).
-
-Download the repository
-
-```
-git clone https://github.com/RasmussenLab/pimms.git
-cd pimms
-```
-
-Using conda (or mamba), install the dependencies and the package in editable mode
-
-```
-# from main folder of repository (containing environment.yml)
-conda env create -n pimms -f environment.yml # slower
-mamba env create -n pimms -f environment.yml # faster, less then 5mins
-```
-
-If on Mac M1, M2 or having otherwise issue using your accelerator (e.g. GPUs): Install the pytorch dependencies first, then the rest of the environment.
-
-### Install development dependencies
-
-Check how to install pytorch for your system [here](https://pytorch.org/get-started/previous-versions/#v1131).
-
-- select the version compatible with your cuda version if you have an nvidia gpu
-
-```bash
-conda create -n vaep_manuel python=3.8 pip
-conda activate vaep_manuel
-conda update pytorch==1.13.1 torchvision==0.14.1 torchaudio==0.13.1 pytorch-cuda=11.7 -c pytorch -c nvidia # might be different
-pip install . # pimms-learn
-pip install papermill jupyterlab # use run notebook interactive or as a script
-cd project
-papermill 04_1_train_pimms_models.ipynb 04_1_train_pimms_models_test.ipynb # second notebook is output
-python 04_1_train_pimms_models.ipynb # just execute the code
-# jupyter lab # open 04_1_train_pimms_models.ipynb
-```
-
-### Entire development installation
-
-
-```bash
-conda create -n pimms_dev -c pytorch -c nvidia -c fastai -c bioconda -c plotly -c conda-forge --file requirements.txt --file requirements_R.txt --file requirements_dev.txt
-pip install -e . # other pip dependencies missing
-snakemake --configfile config/single_dev_dataset/example/config.yaml -F -n
-```
-
-or if you want to update an existing environment
-
-
-```
-conda update  -c defaults -c conda-forge -c fastai -c bioconda -c plotly --file requirements.txt --file requirements_R.txt --file requirements_dev.txt
-```
-
-or using the environment.yml file (can fail on certain systems)
-
-```
-conda env create -f environment.yml
-```
-
-
-### Troubleshooting
-
-Trouble shoot your R installation by opening jupyter lab
-
-```
-# in projects folder
-jupyter lab # open 01_1_train_NAGuideR.ipynb
-
-## Run Demo
-
-Change to the [`project` folder](./project) and see it's [README](project/README.md)
-
-> Currently there are only notebooks and scripts under `project`, 
-> but shared functionality will be added under `vaep` folder-package: This can 
-> then be imported using `import vaep`. See [`vaep/README.md`](vaep/README.md)
-
-You can subselect models by editing the config file:  [`config.yaml`](project/config/single_dev_dataset/proteinGroups_N50/config.yaml) file.
-
-```
-conda activate pimms # activate virtual environment
-cd project # go to project folder
-pwd # so be in ./pimms/project
-snakemake -c1 -p -n # dryrun demo workflow
-snakemake -c1 -p
-```
-
-The demo will run an example on a small data set of 50 HeLa samples (protein groups):
-  1. it describes the data and does create the splits based on the [example data](project/data/dev_datasets/HeLa_6070/README.md)
-     - see `01_0_split_data.ipynb`
-  2. it runs the three semi-supervised models next to some default heuristic methods
-     - see `01_1_train_collab.ipynb`, `01_1_train_dae.ipynb`, `01_1_train_vae.ipynb`
-  3. it creates an comparison
-     - see `01_2_performance_plots.ipynb`
-
-The results are written to `./pimms/project/runs/example`, including `html` versions of the 
-notebooks for inspection, having the following structure:
-
-```
-│   01_0_split_data.html
-│   01_0_split_data.ipynb
-│   01_1_train_collab.html
-│   01_1_train_collab.ipynb
-│   01_1_train_dae.html
-│   01_1_train_dae.ipynb
-│   01_1_train_vae.html
-│   01_1_train_vae.ipynb
-│   01_2_performance_plots.html
-│   01_2_performance_plots.ipynb
-│   data_config.yaml
-│   tree_folder.txt
-|---data
-|---figures
-|---metrics
-|---models
-|---preds
-```
-
-The predictions of the three semi-supervised models can be found under `./pimms/project/runs/example/preds`.
-To combine them with the observed data you can run
-
-```python
-# ipython or python session
-# be in ./pimms/project
-folder_data = 'runs/example/data'
-data = vaep.io.datasplits.DataSplits.from_folder(
-    folder_data, file_format='pkl')
-observed = pd.concat([data.train_X, data.val_y, data.test_y])
-# load predictions for missing values of a certain model
-model = 'vae'
-fpath_pred = f'runs/example/preds/pred_real_na_{model}.csv '
-pred = pd.read_csv(fpath_pred, index_col=[0, 1]).squeeze()
-df_imputed = pd.concat([observed, pred]).unstack()
-# assert no missing values for retained features
-assert df_imputed.isna().sum().sum() == 0
-df_imputed
-```
-
-## Available imputation methods
-
-Packages either are based on this repository, or were referenced by NAGuideR (Table S1).
-From the brief description in the table the exact procedure is not always clear.
-
-| Method        | Package           | source       | status | name              |
-| ------------- | ----------------- | ------       | ------ |------------------ | 
-| CF            | pimms             | pip          | | Collaborative Filtering |
-| DAE           | pimms             | pip          | | Denoising Autoencoder   |
-| VAE           | pimms             | pip          | | Variational Autoencoder |     
-|  |   | | | 
-| ZERO          | -                 | -            | | replace NA with 0 |
-| MINIMUM       | -                 | -            | | replace NA with global minimum    |
-| COLMEDIAN     | e1071             | CRAN         | | replace NA with column median  |
-| ROWMEDIAN     | e1071             | CRAN         | | replace NA with row median     |
-| KNN_IMPUTE    | impute            | BIOCONDUCTOR | | k nearest neighbor imputation   |
-| SEQKNN        | SeqKnn            | tar file     | | Sequential k- nearest neighbor imputation <br> starts with feature with least missing values and re-use imputed values for not yet imputed features
-| BPCA          | pcaMethods        | BIOCONDUCTOR | | Bayesian PCA missing value imputation
-| SVDMETHOD     | pcaMethods        | BIOCONDUCTOR | | replace NA initially with zero, use k most significant eigenvalues using Singular Value Decomposition for imputation until convergence
-| LLS           | pcaMethods        | BIOCONDUCTOR | | Local least squares imputation of a feature based on k most correlated features
-| MLE           | norm              | CRAN         | | Maximum likelihood estimation
-| QRILC         | imputeLCMD        | CRAN         | | quantile regression imputation of left-censored data, i.e. by random draws from a truncated distribution which parameters were estimated by quantile regression
-| MINDET        | imputeLCMD        | CRAN         | | replace NA with q-quantile minimum in a sample
-| MINPROB       | imputeLCMD        | CRAN         | | replace NA by random draws from q-quantile minimum centered distribution
-| IRM           | VIM               | CRAN         | | iterativ robust model-based imputation (one feature at at time)
-| IMPSEQ        | rrcovNA           | CRAN         | | Sequential imputation of missing values by minimizing the determinant of the covariance matrix with imputed values
-| IMPSEQROB     | rrcovNA           | CRAN         | | Sequential imputation of missing values using robust estimators
-| MICE-NORM     | mice              | CRAN         | | Multivariate Imputation by Chained Equations (MICE) using Bayesian linear regression
-| MICE-CART     | mice              | CRAN         | | Multivariate Imputation by Chained Equations (MICE) using regression trees
-| TRKNN         | -                 | script       | | truncation k-nearest neighbor imputation 
-| RF            | missForest        | CRAN         | | Random Forest imputation (one feature at a time)
-| PI            | -                 | -            | | Downshifted normal distribution (per sample)
-| GSIMP         | -                 | script       | | QRILC initialization and iterative Gibbs sampling with generalized linear models (glmnet)
-| MSIMPUTE      | msImpute          | BIOCONDUCTOR | | Missing at random algorithm using low rank approximation
-| MSIMPUTE_MNAR | msImpute          | BIOCONDUCTOR | | Missing not at random algorithm using low rank approximation
-| ~~grr~~       | DreamAI           | -            | Fails to install | Rigde regression 
-| ~~GMS~~       | GMSimpute         | tar file     | Fails on Windows | Lasso model
-
-
-## Build status
-[![Documentation Status](https://readthedocs.org/projects/pimms/badge/?version=latest)](https://pimms.readthedocs.io/en/latest/?badge=latest)
+Metadata-Version: 2.1
+Name: pimms-learn
+Version: 0.3.0
+Summary: Imputing (MS-based prote-) omics data using self supervised deep learning models.
+Author-email: Henry Webel <henry.webel@sund.ku.dk>
+Project-URL: Bug Tracker, https://github.com/RasmussenLab/pimms/issues
+Project-URL: Homepage, https://github.com/RasmussenLab/pimms
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Intended Audience :: Healthcare Industry
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: njab>=0.0.5
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: plotly
+Requires-Dist: torch
+Requires-Dist: scikit-learn>=1.0
+Requires-Dist: scipy
+Requires-Dist: seaborn<0.13
+Requires-Dist: fastai
+Requires-Dist: omegaconf
+Requires-Dist: tqdm
+Requires-Dist: mrmr-selection
+Requires-Dist: pingouin
+Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-book-theme; extra == "docs"
+Requires-Dist: myst-nb; extra == "docs"
+Requires-Dist: ipywidgets; extra == "docs"
+Requires-Dist: sphinx-new-tab-link!=0.2.2; extra == "docs"
+
+# PIMMS
+[![Read the Docs](https://img.shields.io/readthedocs/pimms)](https://readthedocs.org/projects/pimms/) [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/RasmussenLab/pimms/ci.yaml)](https://github.com/RasmussenLab/pimms/actions)
+
+
+PIMMS stands for Proteomics Imputation Modeling Mass Spectrometry 
+and is a hommage to our dear British friends 
+who are missing as part of the EU for far too long already
+(Pimms is also a British summer drink).
+
+The pre-print is available [on biorxiv](https://doi.org/10.1101/2023.01.12.523792).
+
+> `PIMMS` was called `vaep` during development.  
+> Before entire refactoring has to been completed the imported package will be
+`vaep`.
+
+We provide functionality as a python package, an excutable workflow and notebooks.
+
+The models can be used with the scikit-learn interface in the spirit of other scikit-learn imputers. You can try this in colab. [![open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RasmussenLab/pimms/blob/HEAD/project/04_1_train_pimms_models.ipynb)
+
+
+## Python package
+
+For interactive use of the models provided in PIMMS, you can use our
+[python package `pimms-learn`](https://pypi.org/project/pimms-learn/).
+The interface is similar to scikit-learn.
+
+```
+pip install pimms-learn
+```
+
+Then you can use the models on a pandas DataFrame with missing values. Try this in the tutorial on Colab:
+[![open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RasmussenLab/pimms/blob/HEAD/project/04_1_train_pimms_models.ipynb)
+
+## Notebooks as scripts using papermill
+
+If you want to run a model on your prepared data, you can run notebooks prefixed with 
+`01_`, i.e. [`project/01_*.ipynb`](https://github.com/RasmussenLab/pimms/tree/HEAD/project) after cloning the repository. Using jupytext also python percentage script versions
+are saved.
+
+```
+cd project # project folder as pwd
+papermill 01_0_split_data.ipynb --help-notebook
+papermill 01_1_train_vae.ipynb --help-notebook
+```
+
+> Mistyped argument names won't throw an error when using papermill
+
+## PIMMS comparison workflow
+
+The PIMMS comparison workflow is a snakemake workflow that runs the all selected PIMMS models and R-models on 
+a user-provided dataset and compares the results. An example for the smaller HeLa development dataset on the 
+protein groups level is re-built regularly and available at: [rasmussenlab.org/pimms](https://www.rasmussenlab.org/pimms/)
+
+### Setup comparison workflow
+
+The core funtionality is available as a standalone software on PyPI under the name `pimms-learn`. However, running the entire snakemake workflow in enabled using 
+conda (or mamba) and pip to setup an analysis environment. For a detailed description of setting up
+conda (or mamba), see [instructions on setting up a virtual environment](https://github.com/RasmussenLab/pimms/blob/HEAD/docs/venv_setup.md).
+
+Download the repository
+
+```
+git clone https://github.com/RasmussenLab/pimms.git
+cd pimms
+```
+
+Using conda (or mamba), install the dependencies and the package in editable mode
+
+```
+# from main folder of repository (containing environment.yml)
+conda env create -n pimms -f environment.yml # slower
+mamba env create -n pimms -f environment.yml # faster, less then 5mins
+```
+
+If on Mac M1, M2 or having otherwise issue using your accelerator (e.g. GPUs): Install the pytorch dependencies first, then the rest of the environment:
+
+### Install development dependencies
+
+Check how to install pytorch for your system [here](https://pytorch.org/get-started).
+
+- select the version compatible with your cuda version if you have an nvidia gpu or a Mac M-chip.
+
+```bash
+conda create -n vaep python=3.8 pip
+conda activate vaep
+# Follow instructions on https://pytorch.org/get-started 
+# conda env update -f environment.yml -n vaep # should not install the rest.
+pip install pimms-learn
+pip install jupyterlab papermill # use run notebook interactively or as a script
+
+cd project
+# choose one of the following to test the code
+jupyter lab # open 04_1_train_pimms_models.ipynb
+papermill 04_1_train_pimms_models.ipynb 04_1_train_pimms_models_test.ipynb # second notebook is output
+python 04_1_train_pimms_models.py # just execute the code
+```
+
+### Entire development installation
+
+
+```bash
+conda create -n pimms_dev -c pytorch -c nvidia -c fastai -c bioconda -c plotly -c conda-forge --file requirements.txt --file requirements_R.txt --file requirements_dev.txt
+pip install -e . # other pip dependencies missing
+snakemake --configfile config/single_dev_dataset/example/config.yaml -F -n
+```
+
+or if you want to update an existing environment
+
+
+```
+conda update  -c defaults -c conda-forge -c fastai -c bioconda -c plotly --file requirements.txt --file requirements_R.txt --file requirements_dev.txt
+```
+
+or using the environment.yml file (can fail on certain systems)
+
+```
+conda env create -f environment.yml
+```
+
+
+### Troubleshooting
+
+Trouble shoot your R installation by opening jupyter lab
+
+```
+# in projects folder
+jupyter lab # open 01_1_train_NAGuideR.ipynb
+```
+
+## Run an analysis
+
+Change to the [`project` folder](./project) and see it's [README](project/README.md)
+You can subselect models by editing the config file:  [`config.yaml`](project/config/single_dev_dataset/proteinGroups_N50/config.yaml) file.
+
+```
+conda activate pimms # activate virtual environment
+cd project # go to project folder
+pwd # so be in ./pimms/project
+snakemake -c1 -p -n # dryrun demo workflow
+snakemake -c1 -p
+```
+
+The demo will run an example on a small data set of 50 HeLa samples (protein groups):
+  1. it describes the data and does create the splits based on the [example data](project/data/dev_datasets/HeLa_6070/README.md)
+     - see `01_0_split_data.ipynb`
+  2. it runs the three semi-supervised models next to some default heuristic methods
+     - see `01_1_train_collab.ipynb`, `01_1_train_dae.ipynb`, `01_1_train_vae.ipynb`
+  3. it creates an comparison
+     - see `01_2_performance_plots.ipynb`
+
+The results are written to `./pimms/project/runs/example`, including `html` versions of the 
+notebooks for inspection, having the following structure:
+
+```
+│   01_0_split_data.html
+│   01_0_split_data.ipynb
+│   01_1_train_collab.html
+│   01_1_train_collab.ipynb
+│   01_1_train_dae.html
+│   01_1_train_dae.ipynb
+│   01_1_train_vae.html
+│   01_1_train_vae.ipynb
+│   01_2_performance_plots.html
+│   01_2_performance_plots.ipynb
+│   data_config.yaml
+│   tree_folder.txt
+|---data
+|---figures
+|---metrics
+|---models
+|---preds
+```
+
+The predictions of the three semi-supervised models can be found under `./pimms/project/runs/example/preds`.
+To combine them with the observed data you can run
+
+```python
+# ipython or python session
+# be in ./pimms/project
+folder_data = 'runs/example/data'
+data = vaep.io.datasplits.DataSplits.from_folder(
+    folder_data, file_format='pkl')
+observed = pd.concat([data.train_X, data.val_y, data.test_y])
+# load predictions for missing values of a certain model
+model = 'vae'
+fpath_pred = f'runs/example/preds/pred_real_na_{model}.csv '
+pred = pd.read_csv(fpath_pred, index_col=[0, 1]).squeeze()
+df_imputed = pd.concat([observed, pred]).unstack()
+# assert no missing values for retained features
+assert df_imputed.isna().sum().sum() == 0
+df_imputed
+```
+
+## Available imputation methods
+
+Packages either are based on this repository, or were referenced by NAGuideR (Table S1).
+From the brief description in the table the exact procedure is not always clear.
+
+| Method        | Package           | source       | status | name              |
+| ------------- | ----------------- | ------       | ------ |------------------ | 
+| CF            | pimms             | pip          | | Collaborative Filtering |
+| DAE           | pimms             | pip          | | Denoising Autoencoder   |
+| VAE           | pimms             | pip          | | Variational Autoencoder |     
+|  |   | | | 
+| ZERO          | -                 | -            | | replace NA with 0 |
+| MINIMUM       | -                 | -            | | replace NA with global minimum    |
+| COLMEDIAN     | e1071             | CRAN         | | replace NA with column median  |
+| ROWMEDIAN     | e1071             | CRAN         | | replace NA with row median     |
+| KNN_IMPUTE    | impute            | BIOCONDUCTOR | | k nearest neighbor imputation   |
+| SEQKNN        | SeqKnn            | tar file     | | Sequential k- nearest neighbor imputation <br> starts with feature with least missing values and re-use imputed values for not yet imputed features
+| BPCA          | pcaMethods        | BIOCONDUCTOR | | Bayesian PCA missing value imputation
+| SVDMETHOD     | pcaMethods        | BIOCONDUCTOR | | replace NA initially with zero, use k most significant eigenvalues using Singular Value Decomposition for imputation until convergence
+| LLS           | pcaMethods        | BIOCONDUCTOR | | Local least squares imputation of a feature based on k most correlated features
+| MLE           | norm              | CRAN         | | Maximum likelihood estimation
+| QRILC         | imputeLCMD        | CRAN         | | quantile regression imputation of left-censored data, i.e. by random draws from a truncated distribution which parameters were estimated by quantile regression
+| MINDET        | imputeLCMD        | CRAN         | | replace NA with q-quantile minimum in a sample
+| MINPROB       | imputeLCMD        | CRAN         | | replace NA by random draws from q-quantile minimum centered distribution
+| IRM           | VIM               | CRAN         | | iterativ robust model-based imputation (one feature at at time)
+| IMPSEQ        | rrcovNA           | CRAN         | | Sequential imputation of missing values by minimizing the determinant of the covariance matrix with imputed values
+| IMPSEQROB     | rrcovNA           | CRAN         | | Sequential imputation of missing values using robust estimators
+| MICE-NORM     | mice              | CRAN         | | Multivariate Imputation by Chained Equations (MICE) using Bayesian linear regression
+| MICE-CART     | mice              | CRAN         | | Multivariate Imputation by Chained Equations (MICE) using regression trees
+| TRKNN         | -                 | script       | | truncation k-nearest neighbor imputation 
+| RF            | missForest        | CRAN         | | Random Forest imputation (one feature at a time)
+| PI            | -                 | -            | | Downshifted normal distribution (per sample)
+| GSIMP         | -                 | script       | | QRILC initialization and iterative Gibbs sampling with generalized linear models (glmnet)
+| MSIMPUTE      | msImpute          | BIOCONDUCTOR | | Missing at random algorithm using low rank approximation
+| MSIMPUTE_MNAR | msImpute          | BIOCONDUCTOR | | Missing not at random algorithm using low rank approximation
+| ~~grr~~       | DreamAI           | -            | Fails to install | Rigde regression 
+| ~~GMS~~       | GMSimpute         | tar file     | Fails on Windows | Lasso model
+
+
+## Build status
+[![Documentation Status](https://readthedocs.org/projects/pimms/badge/?version=latest)](https://pimms.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `pimms-learn-0.2.0/README.md` & `pimms_learn-0.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,233 +1,234 @@
-# PIMMS
-
-PIMMS stands for Proteomics Imputation Modeling Mass Spectrometry 
-and is a hommage to our dear British friends 
-who are missing as part of the EU for far too long already
-(Pimms is also a British summer drink).
-
-The pre-print is available [on biorxiv](https://doi.org/10.1101/2023.01.12.523792).
-
-
-> `PIMMS` was called `vaep` during development.  
-> Before entire refactoring has to been completed the imported package will be
-`vaep`.
-
-We provide functionality as a python package, an excutable workflow and notebooks.
-
-The models can be used with the scikit-learn interface in the spirit of other scikit-learn imputers. You can try this in colab. [![open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RasmussenLab/pimms/blob/dev/project/04_1_train_pimms_models.ipynb)
-
-
-## Python package
-
-For interactive use of the models provided in PIMMS, you can use our
-[python package `pimms-learn`](https://pypi.org/project/pimms-learn/).
-The interface is similar to scikit-learn.
-
-
-```
-pip install pimms-learn
-```
-
-
-Then you can use the models on a pandas DataFrame with missing values. Try this in the tutorial on Colab:
-[![open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RasmussenLab/pimms/blob/dev/project/04_1_train_pimms_models.ipynb)
-
-## Notebooks as scripts using papermill
-
-If you want to run a model on your prepared data, you can run notebooks prefixed with 
-`01_`, i.e. [`project/01_*.ipynb`](https://github.com/RasmussenLab/pimms/tree/HEAD/project) after cloning the repository. Using jupytext also python percentage script versions
-are saved.
-
-```
-cd project # project folder as pwd
-papermill 01_0_split_data.ipynb --help-notebook
-papermill 01_1_train_vae.ipynb --help-notebook
-```
-
-> Misstyped argument names won't throw an error when using papermill
-
-
-
-
-## Setup for PIMMS comparison workflow
-
-The package is available as a standalone software on pypi. However, running the entire snakemake workflow in enabled using 
-conda (or mamba) and pip to setup the environment. For a detailed description of setting up
-conda (or mamba), see [instructions on setting up a virtual environment](https://github.com/RasmussenLab/pimms/blob/HEAD/docs/venv_setup.md).
-
-Download the repository
-
-```
-git clone https://github.com/RasmussenLab/pimms.git
-cd pimms
-```
-
-Using conda (or mamba), install the dependencies and the package in editable mode
-
-```
-# from main folder of repository (containing environment.yml)
-conda env create -n pimms -f environment.yml # slower
-mamba env create -n pimms -f environment.yml # faster, less then 5mins
-```
-
-If on Mac M1, M2 or having otherwise issue using your accelerator (e.g. GPUs): Install the pytorch dependencies first, then the rest of the environment.
-
-### Install development dependencies
-
-Check how to install pytorch for your system [here](https://pytorch.org/get-started/previous-versions/#v1131).
-
-- select the version compatible with your cuda version if you have an nvidia gpu
-
-```bash
-conda create -n vaep_manuel python=3.8 pip
-conda activate vaep_manuel
-conda update pytorch==1.13.1 torchvision==0.14.1 torchaudio==0.13.1 pytorch-cuda=11.7 -c pytorch -c nvidia # might be different
-pip install . # pimms-learn
-pip install papermill jupyterlab # use run notebook interactive or as a script
-cd project
-papermill 04_1_train_pimms_models.ipynb 04_1_train_pimms_models_test.ipynb # second notebook is output
-python 04_1_train_pimms_models.ipynb # just execute the code
-# jupyter lab # open 04_1_train_pimms_models.ipynb
-```
-
-### Entire development installation
-
-
-```bash
-conda create -n pimms_dev -c pytorch -c nvidia -c fastai -c bioconda -c plotly -c conda-forge --file requirements.txt --file requirements_R.txt --file requirements_dev.txt
-pip install -e . # other pip dependencies missing
-snakemake --configfile config/single_dev_dataset/example/config.yaml -F -n
-```
-
-or if you want to update an existing environment
-
-
-```
-conda update  -c defaults -c conda-forge -c fastai -c bioconda -c plotly --file requirements.txt --file requirements_R.txt --file requirements_dev.txt
-```
-
-or using the environment.yml file (can fail on certain systems)
-
-```
-conda env create -f environment.yml
-```
-
-
-### Troubleshooting
-
-Trouble shoot your R installation by opening jupyter lab
-
-```
-# in projects folder
-jupyter lab # open 01_1_train_NAGuideR.ipynb
-
-## Run Demo
-
-Change to the [`project` folder](./project) and see it's [README](project/README.md)
-
-> Currently there are only notebooks and scripts under `project`, 
-> but shared functionality will be added under `vaep` folder-package: This can 
-> then be imported using `import vaep`. See [`vaep/README.md`](vaep/README.md)
-
-You can subselect models by editing the config file:  [`config.yaml`](project/config/single_dev_dataset/proteinGroups_N50/config.yaml) file.
-
-```
-conda activate pimms # activate virtual environment
-cd project # go to project folder
-pwd # so be in ./pimms/project
-snakemake -c1 -p -n # dryrun demo workflow
-snakemake -c1 -p
-```
-
-The demo will run an example on a small data set of 50 HeLa samples (protein groups):
-  1. it describes the data and does create the splits based on the [example data](project/data/dev_datasets/HeLa_6070/README.md)
-     - see `01_0_split_data.ipynb`
-  2. it runs the three semi-supervised models next to some default heuristic methods
-     - see `01_1_train_collab.ipynb`, `01_1_train_dae.ipynb`, `01_1_train_vae.ipynb`
-  3. it creates an comparison
-     - see `01_2_performance_plots.ipynb`
-
-The results are written to `./pimms/project/runs/example`, including `html` versions of the 
-notebooks for inspection, having the following structure:
-
-```
-│   01_0_split_data.html
-│   01_0_split_data.ipynb
-│   01_1_train_collab.html
-│   01_1_train_collab.ipynb
-│   01_1_train_dae.html
-│   01_1_train_dae.ipynb
-│   01_1_train_vae.html
-│   01_1_train_vae.ipynb
-│   01_2_performance_plots.html
-│   01_2_performance_plots.ipynb
-│   data_config.yaml
-│   tree_folder.txt
-|---data
-|---figures
-|---metrics
-|---models
-|---preds
-```
-
-The predictions of the three semi-supervised models can be found under `./pimms/project/runs/example/preds`.
-To combine them with the observed data you can run
-
-```python
-# ipython or python session
-# be in ./pimms/project
-folder_data = 'runs/example/data'
-data = vaep.io.datasplits.DataSplits.from_folder(
-    folder_data, file_format='pkl')
-observed = pd.concat([data.train_X, data.val_y, data.test_y])
-# load predictions for missing values of a certain model
-model = 'vae'
-fpath_pred = f'runs/example/preds/pred_real_na_{model}.csv '
-pred = pd.read_csv(fpath_pred, index_col=[0, 1]).squeeze()
-df_imputed = pd.concat([observed, pred]).unstack()
-# assert no missing values for retained features
-assert df_imputed.isna().sum().sum() == 0
-df_imputed
-```
-
-## Available imputation methods
-
-Packages either are based on this repository, or were referenced by NAGuideR (Table S1).
-From the brief description in the table the exact procedure is not always clear.
-
-| Method        | Package           | source       | status | name              |
-| ------------- | ----------------- | ------       | ------ |------------------ | 
-| CF            | pimms             | pip          | | Collaborative Filtering |
-| DAE           | pimms             | pip          | | Denoising Autoencoder   |
-| VAE           | pimms             | pip          | | Variational Autoencoder |     
-|  |   | | | 
-| ZERO          | -                 | -            | | replace NA with 0 |
-| MINIMUM       | -                 | -            | | replace NA with global minimum    |
-| COLMEDIAN     | e1071             | CRAN         | | replace NA with column median  |
-| ROWMEDIAN     | e1071             | CRAN         | | replace NA with row median     |
-| KNN_IMPUTE    | impute            | BIOCONDUCTOR | | k nearest neighbor imputation   |
-| SEQKNN        | SeqKnn            | tar file     | | Sequential k- nearest neighbor imputation <br> starts with feature with least missing values and re-use imputed values for not yet imputed features
-| BPCA          | pcaMethods        | BIOCONDUCTOR | | Bayesian PCA missing value imputation
-| SVDMETHOD     | pcaMethods        | BIOCONDUCTOR | | replace NA initially with zero, use k most significant eigenvalues using Singular Value Decomposition for imputation until convergence
-| LLS           | pcaMethods        | BIOCONDUCTOR | | Local least squares imputation of a feature based on k most correlated features
-| MLE           | norm              | CRAN         | | Maximum likelihood estimation
-| QRILC         | imputeLCMD        | CRAN         | | quantile regression imputation of left-censored data, i.e. by random draws from a truncated distribution which parameters were estimated by quantile regression
-| MINDET        | imputeLCMD        | CRAN         | | replace NA with q-quantile minimum in a sample
-| MINPROB       | imputeLCMD        | CRAN         | | replace NA by random draws from q-quantile minimum centered distribution
-| IRM           | VIM               | CRAN         | | iterativ robust model-based imputation (one feature at at time)
-| IMPSEQ        | rrcovNA           | CRAN         | | Sequential imputation of missing values by minimizing the determinant of the covariance matrix with imputed values
-| IMPSEQROB     | rrcovNA           | CRAN         | | Sequential imputation of missing values using robust estimators
-| MICE-NORM     | mice              | CRAN         | | Multivariate Imputation by Chained Equations (MICE) using Bayesian linear regression
-| MICE-CART     | mice              | CRAN         | | Multivariate Imputation by Chained Equations (MICE) using regression trees
-| TRKNN         | -                 | script       | | truncation k-nearest neighbor imputation 
-| RF            | missForest        | CRAN         | | Random Forest imputation (one feature at a time)
-| PI            | -                 | -            | | Downshifted normal distribution (per sample)
-| GSIMP         | -                 | script       | | QRILC initialization and iterative Gibbs sampling with generalized linear models (glmnet)
-| MSIMPUTE      | msImpute          | BIOCONDUCTOR | | Missing at random algorithm using low rank approximation
-| MSIMPUTE_MNAR | msImpute          | BIOCONDUCTOR | | Missing not at random algorithm using low rank approximation
-| ~~grr~~       | DreamAI           | -            | Fails to install | Rigde regression 
-| ~~GMS~~       | GMSimpute         | tar file     | Fails on Windows | Lasso model
-
-
-## Build status
+# PIMMS
+[![Read the Docs](https://img.shields.io/readthedocs/pimms)](https://readthedocs.org/projects/pimms/) [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/RasmussenLab/pimms/ci.yaml)](https://github.com/RasmussenLab/pimms/actions)
+
+
+PIMMS stands for Proteomics Imputation Modeling Mass Spectrometry 
+and is a hommage to our dear British friends 
+who are missing as part of the EU for far too long already
+(Pimms is also a British summer drink).
+
+The pre-print is available [on biorxiv](https://doi.org/10.1101/2023.01.12.523792).
+
+> `PIMMS` was called `vaep` during development.  
+> Before entire refactoring has to been completed the imported package will be
+`vaep`.
+
+We provide functionality as a python package, an excutable workflow and notebooks.
+
+The models can be used with the scikit-learn interface in the spirit of other scikit-learn imputers. You can try this in colab. [![open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RasmussenLab/pimms/blob/HEAD/project/04_1_train_pimms_models.ipynb)
+
+
+## Python package
+
+For interactive use of the models provided in PIMMS, you can use our
+[python package `pimms-learn`](https://pypi.org/project/pimms-learn/).
+The interface is similar to scikit-learn.
+
+```
+pip install pimms-learn
+```
+
+Then you can use the models on a pandas DataFrame with missing values. Try this in the tutorial on Colab:
+[![open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RasmussenLab/pimms/blob/HEAD/project/04_1_train_pimms_models.ipynb)
+
+## Notebooks as scripts using papermill
+
+If you want to run a model on your prepared data, you can run notebooks prefixed with 
+`01_`, i.e. [`project/01_*.ipynb`](https://github.com/RasmussenLab/pimms/tree/HEAD/project) after cloning the repository. Using jupytext also python percentage script versions
+are saved.
+
+```
+cd project # project folder as pwd
+papermill 01_0_split_data.ipynb --help-notebook
+papermill 01_1_train_vae.ipynb --help-notebook
+```
+
+> Mistyped argument names won't throw an error when using papermill
+
+## PIMMS comparison workflow
+
+The PIMMS comparison workflow is a snakemake workflow that runs the all selected PIMMS models and R-models on 
+a user-provided dataset and compares the results. An example for the smaller HeLa development dataset on the 
+protein groups level is re-built regularly and available at: [rasmussenlab.org/pimms](https://www.rasmussenlab.org/pimms/)
+
+### Setup comparison workflow
+
+The core funtionality is available as a standalone software on PyPI under the name `pimms-learn`. However, running the entire snakemake workflow in enabled using 
+conda (or mamba) and pip to setup an analysis environment. For a detailed description of setting up
+conda (or mamba), see [instructions on setting up a virtual environment](https://github.com/RasmussenLab/pimms/blob/HEAD/docs/venv_setup.md).
+
+Download the repository
+
+```
+git clone https://github.com/RasmussenLab/pimms.git
+cd pimms
+```
+
+Using conda (or mamba), install the dependencies and the package in editable mode
+
+```
+# from main folder of repository (containing environment.yml)
+conda env create -n pimms -f environment.yml # slower
+mamba env create -n pimms -f environment.yml # faster, less then 5mins
+```
+
+If on Mac M1, M2 or having otherwise issue using your accelerator (e.g. GPUs): Install the pytorch dependencies first, then the rest of the environment:
+
+### Install development dependencies
+
+Check how to install pytorch for your system [here](https://pytorch.org/get-started).
+
+- select the version compatible with your cuda version if you have an nvidia gpu or a Mac M-chip.
+
+```bash
+conda create -n vaep python=3.8 pip
+conda activate vaep
+# Follow instructions on https://pytorch.org/get-started 
+# conda env update -f environment.yml -n vaep # should not install the rest.
+pip install pimms-learn
+pip install jupyterlab papermill # use run notebook interactively or as a script
+
+cd project
+# choose one of the following to test the code
+jupyter lab # open 04_1_train_pimms_models.ipynb
+papermill 04_1_train_pimms_models.ipynb 04_1_train_pimms_models_test.ipynb # second notebook is output
+python 04_1_train_pimms_models.py # just execute the code
+```
+
+### Entire development installation
+
+
+```bash
+conda create -n pimms_dev -c pytorch -c nvidia -c fastai -c bioconda -c plotly -c conda-forge --file requirements.txt --file requirements_R.txt --file requirements_dev.txt
+pip install -e . # other pip dependencies missing
+snakemake --configfile config/single_dev_dataset/example/config.yaml -F -n
+```
+
+or if you want to update an existing environment
+
+
+```
+conda update  -c defaults -c conda-forge -c fastai -c bioconda -c plotly --file requirements.txt --file requirements_R.txt --file requirements_dev.txt
+```
+
+or using the environment.yml file (can fail on certain systems)
+
+```
+conda env create -f environment.yml
+```
+
+
+### Troubleshooting
+
+Trouble shoot your R installation by opening jupyter lab
+
+```
+# in projects folder
+jupyter lab # open 01_1_train_NAGuideR.ipynb
+```
+
+## Run an analysis
+
+Change to the [`project` folder](./project) and see it's [README](project/README.md)
+You can subselect models by editing the config file:  [`config.yaml`](project/config/single_dev_dataset/proteinGroups_N50/config.yaml) file.
+
+```
+conda activate pimms # activate virtual environment
+cd project # go to project folder
+pwd # so be in ./pimms/project
+snakemake -c1 -p -n # dryrun demo workflow
+snakemake -c1 -p
+```
+
+The demo will run an example on a small data set of 50 HeLa samples (protein groups):
+  1. it describes the data and does create the splits based on the [example data](project/data/dev_datasets/HeLa_6070/README.md)
+     - see `01_0_split_data.ipynb`
+  2. it runs the three semi-supervised models next to some default heuristic methods
+     - see `01_1_train_collab.ipynb`, `01_1_train_dae.ipynb`, `01_1_train_vae.ipynb`
+  3. it creates an comparison
+     - see `01_2_performance_plots.ipynb`
+
+The results are written to `./pimms/project/runs/example`, including `html` versions of the 
+notebooks for inspection, having the following structure:
+
+```
+│   01_0_split_data.html
+│   01_0_split_data.ipynb
+│   01_1_train_collab.html
+│   01_1_train_collab.ipynb
+│   01_1_train_dae.html
+│   01_1_train_dae.ipynb
+│   01_1_train_vae.html
+│   01_1_train_vae.ipynb
+│   01_2_performance_plots.html
+│   01_2_performance_plots.ipynb
+│   data_config.yaml
+│   tree_folder.txt
+|---data
+|---figures
+|---metrics
+|---models
+|---preds
+```
+
+The predictions of the three semi-supervised models can be found under `./pimms/project/runs/example/preds`.
+To combine them with the observed data you can run
+
+```python
+# ipython or python session
+# be in ./pimms/project
+folder_data = 'runs/example/data'
+data = vaep.io.datasplits.DataSplits.from_folder(
+    folder_data, file_format='pkl')
+observed = pd.concat([data.train_X, data.val_y, data.test_y])
+# load predictions for missing values of a certain model
+model = 'vae'
+fpath_pred = f'runs/example/preds/pred_real_na_{model}.csv '
+pred = pd.read_csv(fpath_pred, index_col=[0, 1]).squeeze()
+df_imputed = pd.concat([observed, pred]).unstack()
+# assert no missing values for retained features
+assert df_imputed.isna().sum().sum() == 0
+df_imputed
+```
+
+## Available imputation methods
+
+Packages either are based on this repository, or were referenced by NAGuideR (Table S1).
+From the brief description in the table the exact procedure is not always clear.
+
+| Method        | Package           | source       | status | name              |
+| ------------- | ----------------- | ------       | ------ |------------------ | 
+| CF            | pimms             | pip          | | Collaborative Filtering |
+| DAE           | pimms             | pip          | | Denoising Autoencoder   |
+| VAE           | pimms             | pip          | | Variational Autoencoder |     
+|  |   | | | 
+| ZERO          | -                 | -            | | replace NA with 0 |
+| MINIMUM       | -                 | -            | | replace NA with global minimum    |
+| COLMEDIAN     | e1071             | CRAN         | | replace NA with column median  |
+| ROWMEDIAN     | e1071             | CRAN         | | replace NA with row median     |
+| KNN_IMPUTE    | impute            | BIOCONDUCTOR | | k nearest neighbor imputation   |
+| SEQKNN        | SeqKnn            | tar file     | | Sequential k- nearest neighbor imputation <br> starts with feature with least missing values and re-use imputed values for not yet imputed features
+| BPCA          | pcaMethods        | BIOCONDUCTOR | | Bayesian PCA missing value imputation
+| SVDMETHOD     | pcaMethods        | BIOCONDUCTOR | | replace NA initially with zero, use k most significant eigenvalues using Singular Value Decomposition for imputation until convergence
+| LLS           | pcaMethods        | BIOCONDUCTOR | | Local least squares imputation of a feature based on k most correlated features
+| MLE           | norm              | CRAN         | | Maximum likelihood estimation
+| QRILC         | imputeLCMD        | CRAN         | | quantile regression imputation of left-censored data, i.e. by random draws from a truncated distribution which parameters were estimated by quantile regression
+| MINDET        | imputeLCMD        | CRAN         | | replace NA with q-quantile minimum in a sample
+| MINPROB       | imputeLCMD        | CRAN         | | replace NA by random draws from q-quantile minimum centered distribution
+| IRM           | VIM               | CRAN         | | iterativ robust model-based imputation (one feature at at time)
+| IMPSEQ        | rrcovNA           | CRAN         | | Sequential imputation of missing values by minimizing the determinant of the covariance matrix with imputed values
+| IMPSEQROB     | rrcovNA           | CRAN         | | Sequential imputation of missing values using robust estimators
+| MICE-NORM     | mice              | CRAN         | | Multivariate Imputation by Chained Equations (MICE) using Bayesian linear regression
+| MICE-CART     | mice              | CRAN         | | Multivariate Imputation by Chained Equations (MICE) using regression trees
+| TRKNN         | -                 | script       | | truncation k-nearest neighbor imputation 
+| RF            | missForest        | CRAN         | | Random Forest imputation (one feature at a time)
+| PI            | -                 | -            | | Downshifted normal distribution (per sample)
+| GSIMP         | -                 | script       | | QRILC initialization and iterative Gibbs sampling with generalized linear models (glmnet)
+| MSIMPUTE      | msImpute          | BIOCONDUCTOR | | Missing at random algorithm using low rank approximation
+| MSIMPUTE_MNAR | msImpute          | BIOCONDUCTOR | | Missing not at random algorithm using low rank approximation
+| ~~grr~~       | DreamAI           | -            | Fails to install | Rigde regression 
+| ~~GMS~~       | GMSimpute         | tar file     | Fails on Windows | Lasso model
+
+
+## Build status
 [![Documentation Status](https://readthedocs.org/projects/pimms/badge/?version=latest)](https://pimms.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `pimms-learn-0.2.0/pimms_learn.egg-info/PKG-INFO` & `pimms_learn-0.3.0/pimms_learn.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,265 +1,270 @@
-Metadata-Version: 2.1
-Name: pimms-learn
-Version: 0.2.0
-Summary: Imputing (MS-based prote-) omics data using self supervised deep learning models
-Home-page: https://github.com/RasmussenLab/pimms
-Author: Henry Webel
-Author-email: "Henry Webel" <henry.webel@cpr.ku.dk>
-License: gpl-3.0
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Intended Audience :: Healthcare Industry
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Description-Content-Type: text/markdown
-Requires-Dist: numpy
-Requires-Dist: matplotlib
-Requires-Dist: pandas
-Requires-Dist: plotly
-Requires-Dist: torch
-Requires-Dist: scikit-learn>=1.0
-Requires-Dist: scipy
-Requires-Dist: seaborn
-Requires-Dist: fastai
-Requires-Dist: omegaconf
-Requires-Dist: tqdm
-Requires-Dist: mrmr-selection
-Requires-Dist: pingouin
-Provides-Extra: docs
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: sphinx-book-theme; extra == "docs"
-Requires-Dist: myst-parser; extra == "docs"
-
-# PIMMS
-
-PIMMS stands for Proteomics Imputation Modeling Mass Spectrometry 
-and is a hommage to our dear British friends 
-who are missing as part of the EU for far too long already
-(Pimms is also a British summer drink).
-
-The pre-print is available [on biorxiv](https://doi.org/10.1101/2023.01.12.523792).
-
-
-> `PIMMS` was called `vaep` during development.  
-> Before entire refactoring has to been completed the imported package will be
-`vaep`.
-
-We provide functionality as a python package, an excutable workflow and notebooks.
-
-The models can be used with the scikit-learn interface in the spirit of other scikit-learn imputers. You can try this in colab. [![open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RasmussenLab/pimms/blob/dev/project/04_1_train_pimms_models.ipynb)
-
-
-## Python package
-
-For interactive use of the models provided in PIMMS, you can use our
-[python package `pimms-learn`](https://pypi.org/project/pimms-learn/).
-The interface is similar to scikit-learn.
-
-
-```
-pip install pimms-learn
-```
-
-
-Then you can use the models on a pandas DataFrame with missing values. Try this in the tutorial on Colab:
-[![open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RasmussenLab/pimms/blob/dev/project/04_1_train_pimms_models.ipynb)
-
-## Notebooks as scripts using papermill
-
-If you want to run a model on your prepared data, you can run notebooks prefixed with 
-`01_`, i.e. [`project/01_*.ipynb`](https://github.com/RasmussenLab/pimms/tree/HEAD/project) after cloning the repository. Using jupytext also python percentage script versions
-are saved.
-
-```
-cd project # project folder as pwd
-papermill 01_0_split_data.ipynb --help-notebook
-papermill 01_1_train_vae.ipynb --help-notebook
-```
-
-> Misstyped argument names won't throw an error when using papermill
-
-
-
-
-## Setup for PIMMS comparison workflow
-
-The package is available as a standalone software on pypi. However, running the entire snakemake workflow in enabled using 
-conda (or mamba) and pip to setup the environment. For a detailed description of setting up
-conda (or mamba), see [instructions on setting up a virtual environment](https://github.com/RasmussenLab/pimms/blob/HEAD/docs/venv_setup.md).
-
-Download the repository
-
-```
-git clone https://github.com/RasmussenLab/pimms.git
-cd pimms
-```
-
-Using conda (or mamba), install the dependencies and the package in editable mode
-
-```
-# from main folder of repository (containing environment.yml)
-conda env create -n pimms -f environment.yml # slower
-mamba env create -n pimms -f environment.yml # faster, less then 5mins
-```
-
-If on Mac M1, M2 or having otherwise issue using your accelerator (e.g. GPUs): Install the pytorch dependencies first, then the rest of the environment.
-
-### Install development dependencies
-
-Check how to install pytorch for your system [here](https://pytorch.org/get-started/previous-versions/#v1131).
-
-- select the version compatible with your cuda version if you have an nvidia gpu
-
-```bash
-conda create -n vaep_manuel python=3.8 pip
-conda activate vaep_manuel
-conda update pytorch==1.13.1 torchvision==0.14.1 torchaudio==0.13.1 pytorch-cuda=11.7 -c pytorch -c nvidia # might be different
-pip install . # pimms-learn
-pip install papermill jupyterlab # use run notebook interactive or as a script
-cd project
-papermill 04_1_train_pimms_models.ipynb 04_1_train_pimms_models_test.ipynb # second notebook is output
-python 04_1_train_pimms_models.ipynb # just execute the code
-# jupyter lab # open 04_1_train_pimms_models.ipynb
-```
-
-### Entire development installation
-
-
-```bash
-conda create -n pimms_dev -c pytorch -c nvidia -c fastai -c bioconda -c plotly -c conda-forge --file requirements.txt --file requirements_R.txt --file requirements_dev.txt
-pip install -e . # other pip dependencies missing
-snakemake --configfile config/single_dev_dataset/example/config.yaml -F -n
-```
-
-or if you want to update an existing environment
-
-
-```
-conda update  -c defaults -c conda-forge -c fastai -c bioconda -c plotly --file requirements.txt --file requirements_R.txt --file requirements_dev.txt
-```
-
-or using the environment.yml file (can fail on certain systems)
-
-```
-conda env create -f environment.yml
-```
-
-
-### Troubleshooting
-
-Trouble shoot your R installation by opening jupyter lab
-
-```
-# in projects folder
-jupyter lab # open 01_1_train_NAGuideR.ipynb
-
-## Run Demo
-
-Change to the [`project` folder](./project) and see it's [README](project/README.md)
-
-> Currently there are only notebooks and scripts under `project`, 
-> but shared functionality will be added under `vaep` folder-package: This can 
-> then be imported using `import vaep`. See [`vaep/README.md`](vaep/README.md)
-
-You can subselect models by editing the config file:  [`config.yaml`](project/config/single_dev_dataset/proteinGroups_N50/config.yaml) file.
-
-```
-conda activate pimms # activate virtual environment
-cd project # go to project folder
-pwd # so be in ./pimms/project
-snakemake -c1 -p -n # dryrun demo workflow
-snakemake -c1 -p
-```
-
-The demo will run an example on a small data set of 50 HeLa samples (protein groups):
-  1. it describes the data and does create the splits based on the [example data](project/data/dev_datasets/HeLa_6070/README.md)
-     - see `01_0_split_data.ipynb`
-  2. it runs the three semi-supervised models next to some default heuristic methods
-     - see `01_1_train_collab.ipynb`, `01_1_train_dae.ipynb`, `01_1_train_vae.ipynb`
-  3. it creates an comparison
-     - see `01_2_performance_plots.ipynb`
-
-The results are written to `./pimms/project/runs/example`, including `html` versions of the 
-notebooks for inspection, having the following structure:
-
-```
-│   01_0_split_data.html
-│   01_0_split_data.ipynb
-│   01_1_train_collab.html
-│   01_1_train_collab.ipynb
-│   01_1_train_dae.html
-│   01_1_train_dae.ipynb
-│   01_1_train_vae.html
-│   01_1_train_vae.ipynb
-│   01_2_performance_plots.html
-│   01_2_performance_plots.ipynb
-│   data_config.yaml
-│   tree_folder.txt
-|---data
-|---figures
-|---metrics
-|---models
-|---preds
-```
-
-The predictions of the three semi-supervised models can be found under `./pimms/project/runs/example/preds`.
-To combine them with the observed data you can run
-
-```python
-# ipython or python session
-# be in ./pimms/project
-folder_data = 'runs/example/data'
-data = vaep.io.datasplits.DataSplits.from_folder(
-    folder_data, file_format='pkl')
-observed = pd.concat([data.train_X, data.val_y, data.test_y])
-# load predictions for missing values of a certain model
-model = 'vae'
-fpath_pred = f'runs/example/preds/pred_real_na_{model}.csv '
-pred = pd.read_csv(fpath_pred, index_col=[0, 1]).squeeze()
-df_imputed = pd.concat([observed, pred]).unstack()
-# assert no missing values for retained features
-assert df_imputed.isna().sum().sum() == 0
-df_imputed
-```
-
-## Available imputation methods
-
-Packages either are based on this repository, or were referenced by NAGuideR (Table S1).
-From the brief description in the table the exact procedure is not always clear.
-
-| Method        | Package           | source       | status | name              |
-| ------------- | ----------------- | ------       | ------ |------------------ | 
-| CF            | pimms             | pip          | | Collaborative Filtering |
-| DAE           | pimms             | pip          | | Denoising Autoencoder   |
-| VAE           | pimms             | pip          | | Variational Autoencoder |     
-|  |   | | | 
-| ZERO          | -                 | -            | | replace NA with 0 |
-| MINIMUM       | -                 | -            | | replace NA with global minimum    |
-| COLMEDIAN     | e1071             | CRAN         | | replace NA with column median  |
-| ROWMEDIAN     | e1071             | CRAN         | | replace NA with row median     |
-| KNN_IMPUTE    | impute            | BIOCONDUCTOR | | k nearest neighbor imputation   |
-| SEQKNN        | SeqKnn            | tar file     | | Sequential k- nearest neighbor imputation <br> starts with feature with least missing values and re-use imputed values for not yet imputed features
-| BPCA          | pcaMethods        | BIOCONDUCTOR | | Bayesian PCA missing value imputation
-| SVDMETHOD     | pcaMethods        | BIOCONDUCTOR | | replace NA initially with zero, use k most significant eigenvalues using Singular Value Decomposition for imputation until convergence
-| LLS           | pcaMethods        | BIOCONDUCTOR | | Local least squares imputation of a feature based on k most correlated features
-| MLE           | norm              | CRAN         | | Maximum likelihood estimation
-| QRILC         | imputeLCMD        | CRAN         | | quantile regression imputation of left-censored data, i.e. by random draws from a truncated distribution which parameters were estimated by quantile regression
-| MINDET        | imputeLCMD        | CRAN         | | replace NA with q-quantile minimum in a sample
-| MINPROB       | imputeLCMD        | CRAN         | | replace NA by random draws from q-quantile minimum centered distribution
-| IRM           | VIM               | CRAN         | | iterativ robust model-based imputation (one feature at at time)
-| IMPSEQ        | rrcovNA           | CRAN         | | Sequential imputation of missing values by minimizing the determinant of the covariance matrix with imputed values
-| IMPSEQROB     | rrcovNA           | CRAN         | | Sequential imputation of missing values using robust estimators
-| MICE-NORM     | mice              | CRAN         | | Multivariate Imputation by Chained Equations (MICE) using Bayesian linear regression
-| MICE-CART     | mice              | CRAN         | | Multivariate Imputation by Chained Equations (MICE) using regression trees
-| TRKNN         | -                 | script       | | truncation k-nearest neighbor imputation 
-| RF            | missForest        | CRAN         | | Random Forest imputation (one feature at a time)
-| PI            | -                 | -            | | Downshifted normal distribution (per sample)
-| GSIMP         | -                 | script       | | QRILC initialization and iterative Gibbs sampling with generalized linear models (glmnet)
-| MSIMPUTE      | msImpute          | BIOCONDUCTOR | | Missing at random algorithm using low rank approximation
-| MSIMPUTE_MNAR | msImpute          | BIOCONDUCTOR | | Missing not at random algorithm using low rank approximation
-| ~~grr~~       | DreamAI           | -            | Fails to install | Rigde regression 
-| ~~GMS~~       | GMSimpute         | tar file     | Fails on Windows | Lasso model
-
-
-## Build status
-[![Documentation Status](https://readthedocs.org/projects/pimms/badge/?version=latest)](https://pimms.readthedocs.io/en/latest/?badge=latest)
+Metadata-Version: 2.1
+Name: pimms-learn
+Version: 0.3.0
+Summary: Imputing (MS-based prote-) omics data using self supervised deep learning models.
+Author-email: Henry Webel <henry.webel@sund.ku.dk>
+Project-URL: Bug Tracker, https://github.com/RasmussenLab/pimms/issues
+Project-URL: Homepage, https://github.com/RasmussenLab/pimms
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Intended Audience :: Healthcare Industry
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: njab>=0.0.5
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: plotly
+Requires-Dist: torch
+Requires-Dist: scikit-learn>=1.0
+Requires-Dist: scipy
+Requires-Dist: seaborn<0.13
+Requires-Dist: fastai
+Requires-Dist: omegaconf
+Requires-Dist: tqdm
+Requires-Dist: mrmr-selection
+Requires-Dist: pingouin
+Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-book-theme; extra == "docs"
+Requires-Dist: myst-nb; extra == "docs"
+Requires-Dist: ipywidgets; extra == "docs"
+Requires-Dist: sphinx-new-tab-link!=0.2.2; extra == "docs"
+
+# PIMMS
+[![Read the Docs](https://img.shields.io/readthedocs/pimms)](https://readthedocs.org/projects/pimms/) [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/RasmussenLab/pimms/ci.yaml)](https://github.com/RasmussenLab/pimms/actions)
+
+
+PIMMS stands for Proteomics Imputation Modeling Mass Spectrometry 
+and is a hommage to our dear British friends 
+who are missing as part of the EU for far too long already
+(Pimms is also a British summer drink).
+
+The pre-print is available [on biorxiv](https://doi.org/10.1101/2023.01.12.523792).
+
+> `PIMMS` was called `vaep` during development.  
+> Before entire refactoring has to been completed the imported package will be
+`vaep`.
+
+We provide functionality as a python package, an excutable workflow and notebooks.
+
+The models can be used with the scikit-learn interface in the spirit of other scikit-learn imputers. You can try this in colab. [![open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RasmussenLab/pimms/blob/HEAD/project/04_1_train_pimms_models.ipynb)
+
+
+## Python package
+
+For interactive use of the models provided in PIMMS, you can use our
+[python package `pimms-learn`](https://pypi.org/project/pimms-learn/).
+The interface is similar to scikit-learn.
+
+```
+pip install pimms-learn
+```
+
+Then you can use the models on a pandas DataFrame with missing values. Try this in the tutorial on Colab:
+[![open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RasmussenLab/pimms/blob/HEAD/project/04_1_train_pimms_models.ipynb)
+
+## Notebooks as scripts using papermill
+
+If you want to run a model on your prepared data, you can run notebooks prefixed with 
+`01_`, i.e. [`project/01_*.ipynb`](https://github.com/RasmussenLab/pimms/tree/HEAD/project) after cloning the repository. Using jupytext also python percentage script versions
+are saved.
+
+```
+cd project # project folder as pwd
+papermill 01_0_split_data.ipynb --help-notebook
+papermill 01_1_train_vae.ipynb --help-notebook
+```
+
+> Mistyped argument names won't throw an error when using papermill
+
+## PIMMS comparison workflow
+
+The PIMMS comparison workflow is a snakemake workflow that runs the all selected PIMMS models and R-models on 
+a user-provided dataset and compares the results. An example for the smaller HeLa development dataset on the 
+protein groups level is re-built regularly and available at: [rasmussenlab.org/pimms](https://www.rasmussenlab.org/pimms/)
+
+### Setup comparison workflow
+
+The core funtionality is available as a standalone software on PyPI under the name `pimms-learn`. However, running the entire snakemake workflow in enabled using 
+conda (or mamba) and pip to setup an analysis environment. For a detailed description of setting up
+conda (or mamba), see [instructions on setting up a virtual environment](https://github.com/RasmussenLab/pimms/blob/HEAD/docs/venv_setup.md).
+
+Download the repository
+
+```
+git clone https://github.com/RasmussenLab/pimms.git
+cd pimms
+```
+
+Using conda (or mamba), install the dependencies and the package in editable mode
+
+```
+# from main folder of repository (containing environment.yml)
+conda env create -n pimms -f environment.yml # slower
+mamba env create -n pimms -f environment.yml # faster, less then 5mins
+```
+
+If on Mac M1, M2 or having otherwise issue using your accelerator (e.g. GPUs): Install the pytorch dependencies first, then the rest of the environment:
+
+### Install development dependencies
+
+Check how to install pytorch for your system [here](https://pytorch.org/get-started).
+
+- select the version compatible with your cuda version if you have an nvidia gpu or a Mac M-chip.
+
+```bash
+conda create -n vaep python=3.8 pip
+conda activate vaep
+# Follow instructions on https://pytorch.org/get-started 
+# conda env update -f environment.yml -n vaep # should not install the rest.
+pip install pimms-learn
+pip install jupyterlab papermill # use run notebook interactively or as a script
+
+cd project
+# choose one of the following to test the code
+jupyter lab # open 04_1_train_pimms_models.ipynb
+papermill 04_1_train_pimms_models.ipynb 04_1_train_pimms_models_test.ipynb # second notebook is output
+python 04_1_train_pimms_models.py # just execute the code
+```
+
+### Entire development installation
+
+
+```bash
+conda create -n pimms_dev -c pytorch -c nvidia -c fastai -c bioconda -c plotly -c conda-forge --file requirements.txt --file requirements_R.txt --file requirements_dev.txt
+pip install -e . # other pip dependencies missing
+snakemake --configfile config/single_dev_dataset/example/config.yaml -F -n
+```
+
+or if you want to update an existing environment
+
+
+```
+conda update  -c defaults -c conda-forge -c fastai -c bioconda -c plotly --file requirements.txt --file requirements_R.txt --file requirements_dev.txt
+```
+
+or using the environment.yml file (can fail on certain systems)
+
+```
+conda env create -f environment.yml
+```
+
+
+### Troubleshooting
+
+Trouble shoot your R installation by opening jupyter lab
+
+```
+# in projects folder
+jupyter lab # open 01_1_train_NAGuideR.ipynb
+```
+
+## Run an analysis
+
+Change to the [`project` folder](./project) and see it's [README](project/README.md)
+You can subselect models by editing the config file:  [`config.yaml`](project/config/single_dev_dataset/proteinGroups_N50/config.yaml) file.
+
+```
+conda activate pimms # activate virtual environment
+cd project # go to project folder
+pwd # so be in ./pimms/project
+snakemake -c1 -p -n # dryrun demo workflow
+snakemake -c1 -p
+```
+
+The demo will run an example on a small data set of 50 HeLa samples (protein groups):
+  1. it describes the data and does create the splits based on the [example data](project/data/dev_datasets/HeLa_6070/README.md)
+     - see `01_0_split_data.ipynb`
+  2. it runs the three semi-supervised models next to some default heuristic methods
+     - see `01_1_train_collab.ipynb`, `01_1_train_dae.ipynb`, `01_1_train_vae.ipynb`
+  3. it creates an comparison
+     - see `01_2_performance_plots.ipynb`
+
+The results are written to `./pimms/project/runs/example`, including `html` versions of the 
+notebooks for inspection, having the following structure:
+
+```
+│   01_0_split_data.html
+│   01_0_split_data.ipynb
+│   01_1_train_collab.html
+│   01_1_train_collab.ipynb
+│   01_1_train_dae.html
+│   01_1_train_dae.ipynb
+│   01_1_train_vae.html
+│   01_1_train_vae.ipynb
+│   01_2_performance_plots.html
+│   01_2_performance_plots.ipynb
+│   data_config.yaml
+│   tree_folder.txt
+|---data
+|---figures
+|---metrics
+|---models
+|---preds
+```
+
+The predictions of the three semi-supervised models can be found under `./pimms/project/runs/example/preds`.
+To combine them with the observed data you can run
+
+```python
+# ipython or python session
+# be in ./pimms/project
+folder_data = 'runs/example/data'
+data = vaep.io.datasplits.DataSplits.from_folder(
+    folder_data, file_format='pkl')
+observed = pd.concat([data.train_X, data.val_y, data.test_y])
+# load predictions for missing values of a certain model
+model = 'vae'
+fpath_pred = f'runs/example/preds/pred_real_na_{model}.csv '
+pred = pd.read_csv(fpath_pred, index_col=[0, 1]).squeeze()
+df_imputed = pd.concat([observed, pred]).unstack()
+# assert no missing values for retained features
+assert df_imputed.isna().sum().sum() == 0
+df_imputed
+```
+
+## Available imputation methods
+
+Packages either are based on this repository, or were referenced by NAGuideR (Table S1).
+From the brief description in the table the exact procedure is not always clear.
+
+| Method        | Package           | source       | status | name              |
+| ------------- | ----------------- | ------       | ------ |------------------ | 
+| CF            | pimms             | pip          | | Collaborative Filtering |
+| DAE           | pimms             | pip          | | Denoising Autoencoder   |
+| VAE           | pimms             | pip          | | Variational Autoencoder |     
+|  |   | | | 
+| ZERO          | -                 | -            | | replace NA with 0 |
+| MINIMUM       | -                 | -            | | replace NA with global minimum    |
+| COLMEDIAN     | e1071             | CRAN         | | replace NA with column median  |
+| ROWMEDIAN     | e1071             | CRAN         | | replace NA with row median     |
+| KNN_IMPUTE    | impute            | BIOCONDUCTOR | | k nearest neighbor imputation   |
+| SEQKNN        | SeqKnn            | tar file     | | Sequential k- nearest neighbor imputation <br> starts with feature with least missing values and re-use imputed values for not yet imputed features
+| BPCA          | pcaMethods        | BIOCONDUCTOR | | Bayesian PCA missing value imputation
+| SVDMETHOD     | pcaMethods        | BIOCONDUCTOR | | replace NA initially with zero, use k most significant eigenvalues using Singular Value Decomposition for imputation until convergence
+| LLS           | pcaMethods        | BIOCONDUCTOR | | Local least squares imputation of a feature based on k most correlated features
+| MLE           | norm              | CRAN         | | Maximum likelihood estimation
+| QRILC         | imputeLCMD        | CRAN         | | quantile regression imputation of left-censored data, i.e. by random draws from a truncated distribution which parameters were estimated by quantile regression
+| MINDET        | imputeLCMD        | CRAN         | | replace NA with q-quantile minimum in a sample
+| MINPROB       | imputeLCMD        | CRAN         | | replace NA by random draws from q-quantile minimum centered distribution
+| IRM           | VIM               | CRAN         | | iterativ robust model-based imputation (one feature at at time)
+| IMPSEQ        | rrcovNA           | CRAN         | | Sequential imputation of missing values by minimizing the determinant of the covariance matrix with imputed values
+| IMPSEQROB     | rrcovNA           | CRAN         | | Sequential imputation of missing values using robust estimators
+| MICE-NORM     | mice              | CRAN         | | Multivariate Imputation by Chained Equations (MICE) using Bayesian linear regression
+| MICE-CART     | mice              | CRAN         | | Multivariate Imputation by Chained Equations (MICE) using regression trees
+| TRKNN         | -                 | script       | | truncation k-nearest neighbor imputation 
+| RF            | missForest        | CRAN         | | Random Forest imputation (one feature at a time)
+| PI            | -                 | -            | | Downshifted normal distribution (per sample)
+| GSIMP         | -                 | script       | | QRILC initialization and iterative Gibbs sampling with generalized linear models (glmnet)
+| MSIMPUTE      | msImpute          | BIOCONDUCTOR | | Missing at random algorithm using low rank approximation
+| MSIMPUTE_MNAR | msImpute          | BIOCONDUCTOR | | Missing not at random algorithm using low rank approximation
+| ~~grr~~       | DreamAI           | -            | Fails to install | Rigde regression 
+| ~~GMS~~       | GMSimpute         | tar file     | Fails on Windows | Lasso model
+
+
+## Build status
+[![Documentation Status](https://readthedocs.org/projects/pimms/badge/?version=latest)](https://pimms.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `pimms-learn-0.2.0/vaep/analyzers/analyzers.py` & `pimms_learn-0.3.0/vaep/analyzers/analyzers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,579 +1,541 @@
-from collections import namedtuple
-from pathlib import Path
-from types import SimpleNamespace
-from typing import Tuple, Union, List
-
-import logging
-import random
-
-
-import numpy as np
-import pandas as pd
-
-import matplotlib.pyplot as plt
-import matplotlib.dates as mdates
-import seaborn
-
-from sklearn.decomposition import PCA
-from sklearn.impute import SimpleImputer
-
-import vaep
-from vaep.analyzers import Analysis
-
-from vaep.pandas import _add_indices
-from vaep.io.datasplits import long_format, wide_format
-
-
-logger = logging.getLogger(__name__)
-
-__doc__ = 'A collection of Analyzers to perform certain type of analysis.'
-
-
-ALPHA = 0.5
-
-
-def verify_df(df,
-              fname,
-              index_col: str,  # could be potentially 0 for the first column
-              verify_fname: bool = False,
-              usecols=None,
-              ):
-    if usecols and isinstance(index_col, str):
-        assert index_col in usecols, 'Add index_col to usecols Sequence'
-    if verify_fname:
-        if not len(df.shape) == 2:
-            raise ValueError(f"Expected 2 -dimensional array, not {len(df.shape)} -dimensional,"
-                             f" of type: {type(df)}")
-        N, M = df.shape
-        assert f'N{N:05d}' in str(fname) and f'M{M:05d}' in str(fname), \
-            ("Filename number don't match loaded numbers: "
-                f"{fname} should contain N{N} and M{M}")
-
-
-class AnalyzePeptides(SimpleNamespace):
-    """Namespace for current analysis
-
-    Attributes
-    ----------
-    df:  pandas.DataFrame
-        current eagerly loaded data in wide format only: sample index, features in columns
-    stats: types.SimpleNamespace
-        Some statistics of certain aspects. Normally each will be a DataFrame.
-
-    Many more attributes are set dynamically depending on the concrete analysis.
-    """
-
-    def __init__(self, data: pd.DataFrame,
-                 is_log_transformed: bool = False,
-                 is_wide_format: bool = True, ind_unstack: str = '',):
-        if not is_wide_format:
-            if not ind_unstack:
-                raise ValueError("Please specify index level for unstacking via "
-                                 f"'ind_unstack' from: {data.index.names}")
-            data = data.unstack(ind_unstack)
-            is_wide_format = True
-        self.df = data  # assume wide
-        self.N, self.M = self.df.shape
-        self.stats = SimpleNamespace()
-        self.is_log_transformed = is_log_transformed
-        self.is_wide_format = is_wide_format
-        self.index_col = self.df.index.name
-
-    @classmethod
-    def from_csv(cls, fname: str,
-                 nrows: int = None,
-                 # could be potentially 0 for the first column
-                 index_col: Union[int, str, List] = 'Sample ID',
-                 verify_fname: bool = False,
-                 usecols=None,
-                 **kwargs):
-        df = pd.read_csv(fname, index_col=index_col, low_memory=False,
-                         nrows=nrows, usecols=usecols).squeeze('columns')
-        if len(df.shape) == 1:
-            # unstack all but first column
-            df = df.unstack(df.index.names[1:])
-        verify_df(df=df, fname=fname,
-                  index_col=index_col,
-                  verify_fname=verify_fname,
-                  usecols=usecols)
-        return cls(data=df, **kwargs)  # all __init__ parameters are kwargs
-
-    @classmethod
-    # @delegates(from_csv)  # does only include parameters with defaults
-    def from_pickle(cls, fname: str,
-                    # could be potentially 0 for the first column
-                    index_col: Union[int, str, List] = 'Sample ID',
-                    verify_fname: bool = False,
-                    usecols=None,
-                    **kwargs):
-        df = pd.read_pickle(fname).squeeze()
-        if len(df.shape) == 1:
-            df = df.unstack(df.index.names[1:])
-        verify_df(df=df, fname=fname,
-                  index_col=index_col,
-                  verify_fname=verify_fname,
-                  usecols=usecols)
-        return cls(data=df, **kwargs)  # all __init__ parameters are kwargs
-
-    def get_consecutive_dates(self, n_samples, seed=42):
-        """Select n consecutive samples using a seed.
-
-        Updated the original DataFrame attribute: df
-        """
-        self.df.sort_index(inplace=True)
-        n_samples = min(len(self.df), n_samples) if n_samples else len(self.df)
-        print(f"Get {n_samples} samples.")
-
-        if seed:
-            random.seed(42)
-
-        _attr_name = f'df_{n_samples}'
-        setattr(self, _attr_name, get_consecutive_data_indices(self.df, n_samples))
-        print("Training data referenced unter:", _attr_name)
-        self.df = getattr(self, _attr_name)
-        print("Updated attribute: df")
-        return self.df
-
-    @property
-    def df_long(self):
-        if hasattr(self, '_df_long'):
-            return self._df_long
-        return self.to_long_format(colname_values='intensity', index_name=self.index_col)
-
-    def to_long_format(
-            self,
-            colname_values: str = 'intensity',
-            index_name: str = 'Sample ID',
-            inplace: str = False) -> pd.DataFrame:
-        """[summary]
-
-        Parameters
-        ----------
-        colname_values : str, optional
-            New column name for values in matrix, by default 'intensity'
-        index_name : str, optional
-            Name of column to assign as index (based on long-data format), by default 'Sample ID'
-        inplace : bool, optional
-            Assign result to df_long (False), or to df (True) attribute, by default False
-        Returns
-        -------
-        pd.DataFrame
-            Data in long-format as DataFrame
-        """
-
-        """Build long data view."""
-        if not self.is_wide_format:
-            return self.df
-        if hasattr(self, '_df_long'):
-            return self._df_long  # rm attribute to overwrite
-
-        df_long = long_format(
-            self.df,
-            colname_values=colname_values,
-            # index_name=index_name
-        )
-
-        if inplace:
-            self.df = df_long
-            self.is_wide_format = False
-            return self.df
-        self._df_long = df_long
-        return df_long
-
-    @property
-    def df_wide(self):
-        return self.to_wide_format()
-
-    def to_wide_format(
-            self,
-            columns: str = 'Sample ID',
-            name_values: str = 'intensity',
-            inplace: bool = False) -> pd.DataFrame:
-        """[summary]
-
-        Parameters
-        ----------
-        columns : str, optional
-            Index level to be shown as columns, by default 'Sample ID'
-        name_values : str, optional
-            Column in long-data format to be used as values, by default 'intensity'
-        inplace : bool, optional
-            Assign result to df_wide (False), or to df (True) attribute, by default False
-
-        Returns
-        -------
-        pd.DataFrame
-            [description]
-        """
-
-        """Build wide data view.
-
-        Return df attribute in case this is in wide-format. If df attribute is in long-format
-        this is used. If df is wide, but long-format exist, then the wide format is build.
-
-
-        """
-        if self.is_wide_format:
-            return self.df
-
-        if hasattr(self, '_df_long'):
-            df = self._df_long
-        else:
-            df = self.df
-
-        df_wide = wide_format(df, columns=columns, name_values=name_values)
-
-        if inplace:
-            self.df = df_wide
-            self.is_wide_format = True
-            return self.df
-        self._df_wide = df_wide
-        print(f"Set attribute: df_wide")
-        return df_wide
-
-    def describe_peptides(self, sample_n: int = None):
-        if sample_n:
-            df = self.df.sample(n=sample_n, axis=1)
-        else:
-            df = self.df
-        stats = df.describe()
-        stats.loc['CV'] = stats.loc['std'] / stats.loc['mean']
-        self.stats.peptides = stats
-        return stats
-
-    def get_prop_not_na(self):
-        """Get prop. of not NA values for each sample."""
-        return self.df.notna().sum(axis=1) / self.df.shape[-1]
-
-    def get_PCA(self, n_components=2, imputer=SimpleImputer):
-        self.imputer_ = imputer()
-        X = self.imputer_.fit_transform(self.df)
-        X = _add_indices(X, self.df)
-        assert all(X.notna())
-
-        PCs, self.pca_ = run_pca(X, n_components=n_components)
-        if not hasattr(self, 'df_meta'):
-            logger.warning('No metadata available, please set "df_meta" first.')
-        try:
-            PCs['ms_instrument'] = self.df_meta['ms_instrument'].astype('category')
-        except KeyError:
-            logger.warning("No MS instrument added.")
-        except AttributeError:
-            logger.warning("No metadata available, please set 'df_meta' first.")
-            logger.warning("No MS instrument added.")
-        return PCs
-
-    def calculate_PCs(self, new_df, is_wide=True):
-        if not is_wide:
-            new_df = new_df.unstack(new_df.index.names[1:])
-
-        X = self.imputer_.transform(new_df)
-        X = _add_indices(X, new_df)
-        PCs = self.pca_.transform(X)
-        PCs = _add_indices(PCs, new_df, index_only=True)
-        PCs.columns = [f'PC {i+1}' for i in range(PCs.shape[-1])]
-        return PCs
-
-    def plot_pca(self,):
-        """Create principal component plot with three heatmaps showing
-        instrument, degree of non NA data and sample by date."""
-        if not self.is_wide_format:
-            self.df = self.df.unstack(self.df.index.names[1:])
-            self.is_wide_format = True
-
-        if not hasattr(self, 'df_meta'):
-            raise AttributeError('No metadata available, please set "df_meta" first.')
-
-        PCs = self.get_PCA()
-        cols = list(PCs.columns)
-
-        fig, axes = plt.subplots(nrows=3, ncols=1, figsize=(
-            15, 20), constrained_layout=True)
-
-        Dim = namedtuple('DimensionsData', 'N M')
-        self.dim = Dim(*self.df.shape)
-
-        fig.suptitle(
-            f'First two Principal Components of {self.dim.M} most abundant peptides \n for {self.dim.N} samples',
-            fontsize=30)
-
-        # by instrument
-        ax = axes[0]
-        seaborn_scatter(df=PCs.iloc[:, :2], fig=fig, ax=ax,
-                        meta=PCs['ms_instrument'], title='by MS instrument')
-        ax.legend(loc='center right', bbox_to_anchor=(1.11, 0.5))
-
-        # by complettness/missingness
-        # continues colormap will be a bit trickier using seaborn: https://stackoverflow.com/a/44642014/9684872
-        ax = axes[1]
-        plot_scatter(df=PCs.iloc[:, :2], fig=fig, ax=ax,
-                     meta=self.df_meta['prop_not_na'], title='by number on na')
-
-        # by dates
-        ax = axes[2]
-        plot_date_map(df=PCs.iloc[:, :2],
-                      ax=ax, dates=self.df_meta.date)
-
-        return fig
-
-    def log_transform(self, log_fct: np.ufunc):
-        """Log transform data in-place.
-
-        Parameters
-        ----------
-        log_fct : np.ufunc
-            Numpy log-function
-
-        Raises
-        ------
-        Exception
-            if data has been previously log-transformed.
-        """
-        if self.is_log_transformed:
-            raise Exception(
-                f'Data was already log transformed, using {self.__class__.__name__}.log_fct: {self.log_fct}')
-        else:
-            self.df = log_fct(self.df)
-            self.is_log_transformed = True
-            self.log_fct = log_fct
-
-    def get_dectection_limit(self):
-        """Compute information on detection limit in dataset.
-
-        Returns
-        -------
-        str
-            Information on detection limit
-        """
-        self.detection_limit = self.df.min().min() if self.is_log_transformed else np.log10(
-            self.df).min().min()  # all zeros become nan.
-        return "Detection limit: {:6.3f}, corresponding to intensity value of {:,d}".format(
-            self.detection_limit,
-            int(10 ** self.detection_limit))
-
-    def __repr__(self):
-        keys = sorted(self.__dict__)
-        items = ("{}".format(k, self.__dict__[k]) for k in keys)
-        return "{} with attributes: {}".format(type(self).__name__, ", ".join(items))
-
-    # def __dir__(self):
-    #     return sorted(self.__dict__)
-
-    @property
-    def fname_stub(self):
-        assert hasattr(self, 'df'), f'Attribute df is missing: {self}'
-        return 'N{:05d}_M{:05d}'.format(*self.df.shape)
-
-
-class LatentAnalysis(Analysis):
-
-    def __init__(self, latent_space: pd.DataFrame, meta_data: pd.DataFrame, model_name: str,
-                 fig_size: Tuple[int, int] = (15, 15), folder: Path = None):
-        self.latent_space, self.meta_data = latent_space, meta_data
-        self.fig_size, self.folder = fig_size, folder
-        self.model_name = model_name
-        self.folder = Path(self.folder) if self.folder else Path('.')
-        assert len(
-            self.latent_space.shape) == 2, "Expected a two dimensional DataFrame."
-        self.latent_dim = self.latent_space.shape[-1]
-        if self.latent_dim > 2:
-            # pca, add option for different methods
-            self.latent_reduced, self.pca_ = run_pca(self.latent_space)
-        else:
-            self.latent_reduced = self.latent_space
-
-    def plot_by_date(self, meta_key: str = 'date', save: bool = True):
-        fig, ax = self._plot(fct=plot_date_map, meta_key=meta_key, save=save)
-        return fig, ax
-
-    def plot_by_category(self, meta_key: str, save: bool = True):
-        fig, ax = self._plot(fct=seaborn_scatter, meta_key=meta_key, save=save)
-        return fig, ax
-
-    def _plot(self, fct, meta_key: str, save: bool = True):
-        try:
-            meta_data = self.meta_data[meta_key]
-        except KeyError:
-            raise ValueError(f"Requested key: '{meta_key}' is not in available,"
-                             f" use: {', '.join(x for x in self.meta_data.columns)}")
-        fig, ax = plt.subplots(figsize=self.fig_size)
-        _ = fct(df=self.latent_reduced, ax=ax,
-                meta=meta_data.loc[self.latent_reduced.index],
-                title=f'{self.model_name} latent space PCA of {self.latent_dim} dimensions by {meta_key}')
-        if save:
-            vaep.plotting._savefig(fig, name=f'{self.model_name}_latent_by_{meta_key}',
-                                   folder=self.folder)
-        return fig, ax
-
-
-# def read_csv(fname:str, nrows:int, index_col:str=None)-> pd.DataFrame:
-#     return pd.read_csv(fname, index_col=index_col, low_memory=False, nrows=nrows)
-
-
-def get_consecutive_data_indices(df, n_samples):
-    index = df.sort_index().index
-    start_sample = len(index) - n_samples
-    start_sample = random.randint(0, start_sample)
-    return df.loc[index[start_sample:start_sample + n_samples]]
-
-
-def corr_lower_triangle(df):
-    """Compute the correlation matrix, returning only unique values."""
-    corr_df = df.corr()
-    lower_triangle = pd.DataFrame(
-        np.tril(np.ones(corr_df.shape), -1)).astype(bool)
-    lower_triangle.index, lower_triangle.columns = corr_df.index, corr_df.columns
-    return corr_df.where(lower_triangle)
-
-
-def plot_corr_histogram(corr_lower_triangle, bins=10):
-    fig, axes = plt.subplots(ncols=2, gridspec_kw={"width_ratios": [
-        5, 1], "wspace": 0.2}, figsize=(8, 4))
-    values = pd.Series(corr_lower_triangle.to_numpy().flatten()).dropna()
-    ax = axes[0]
-    ax = values.hist(ax=ax, bins=bins)
-    ax.yaxis.set_major_formatter("{x:,.0f}")
-    ax = axes[1]
-    plt.axis('off')
-    data = values.describe(percentiles=np.linspace(0.1, 1, 10)).round(2)
-    data.name = ''
-    _ = pd.plotting.table(ax=ax, data=data, loc="best", edges="open")
-    return fig, axes
-
-
-def run_pca(df_wide: pd.DataFrame, n_components: int = 2) -> Tuple[pd.DataFrame, PCA]:
-    """Run PCA on DataFrame and return result.
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        DataFrame in wide format to fit features on.
-    n_components : int, optional
-        Number of Principal Components to fit, by default 2
-
-    Returns
-    -------
-    Tuple[pd.DataFrame, PCA]
-        principal compoments of DataFrame with same indices as in original DataFrame,
-        and fitted PCA model of sklearn
-    """
-    pca = PCA(n_components=n_components)
-    PCs = pca.fit_transform(df_wide)
-    cols = [f'principal component {i+1} ({var_explained*100:.2f} %)' for i,
-            var_explained in enumerate(pca.explained_variance_ratio_)]
-    PCs = pd.DataFrame(PCs, index=df_wide.index, columns=cols)
-    return PCs, pca
-
-
-def plot_date_map(df, ax,
-                  dates: pd.Series = None,
-                  meta: pd.Series = None,
-                  title: str = 'by date',
-                  fontsize=8,
-                  size=2):
-    if dates is not None and meta is not None:
-        raise ValueError("Only set either dates or meta parameters.")
-        # ToDo: Clean up arguments
-    if dates is None:
-        dates = meta
-    cols = list(df.columns)
-    assert len(cols) == 2, f'Please provide two dimensons, not {df.columns}'
-    ax.set_title(title, fontsize=fontsize)
-    ax.set_xlabel(cols[0])
-    ax.set_ylabel(cols[1])
-    path_collection = scatter_plot_w_dates(
-        ax, df, dates=dates, errors='raise')
-    cbar = add_date_colorbar(path_collection, ax=ax)
-
-
-def plot_scatter(df, ax,
-                 meta: pd.Series,
-                 title: str = 'by some metadata',
-                 alpha=ALPHA,
-                 fontsize=8,
-                 size=2):
-    cols = list(df.columns)
-    assert len(cols) == 2, f'Please provide two dimensons, not {df.columns}'
-    ax.set_title(title, fontsize=fontsize)
-    ax.set_xlabel(cols[0])
-    ax.set_ylabel(cols[1])
-    path_collection = ax.scatter(
-        x=cols[0], y=cols[1], s=size, c=meta, data=df, alpha=alpha)
-    cbar = ax.get_figure().colorbar(path_collection, ax=ax)
-
-
-def seaborn_scatter(df, ax,
-                    meta: pd.Series,
-                    title: str = 'by some metadata',
-                    alpha=ALPHA,
-                    fontsize=5,
-                    size=5):
-    cols = list(df.columns)
-    assert len(cols) == 2, f'Please provide two dimensons, not {df.columns}'
-    seaborn.scatterplot(x=df[cols[0]], y=df[cols[1]],
-                        hue=meta, ax=ax, palette='deep', s=size, alpha=alpha)
-    _ = ax.legend(fontsize=fontsize,
-                  title_fontsize=fontsize,
-                  markerscale=0.4,
-                  title=meta.name,
-                  )
-    ax.set_title(title, fontsize=fontsize)
-    return ax
-
-
-def scatter_plot_w_dates(ax, df,
-                         dates=None,
-                         marker=None,
-                         errors='raise',
-                         size=2):
-    """plot first vs. second column in DataFrame.
-    Use dates to color data.
-
-
-
-    errors : {'ignore', 'raise', 'coerce'}, default 'raise'
-        Passed on to pandas.to_datetime
-        - If 'raise', then invalid parsing will raise an exception.
-        - If 'coerce', then invalid parsing will be set as NaT.
-        - If 'ignore', then invalid parsing will return the input.
-    """
-    # Inspiration:  https://stackoverflow.com/a/59685599/9684872
-    cols = df.columns
-
-    if isinstance(dates, str):
-        dates = df['dates']
-
-    path_collection = ax.scatter(
-        x=df[cols[0]],
-        y=df[cols[1]],
-        c=[mdates.date2num(t) for t in pd.to_datetime(dates, errors=errors)
-           ] if dates is not None else None,
-        alpha=ALPHA,
-        s=size,
-        marker=marker,
-    )
-    return path_collection
-
-
-def add_date_colorbar(mappable, ax):
-    loc = mdates.AutoDateLocator()
-    cbar = ax.get_figure().colorbar(mappable, ax=ax, ticks=loc,
-                                    format=mdates.AutoDateFormatter(loc))
-    return cbar
-
-
-def cast_object_to_category(df: pd.DataFrame) -> pd.DataFrame:
-    """Cast object columns to category dtype.
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        DataFrame with columns
-
-    Returns
-    -------
-    pd.DataFrame
-        DataFrame with category columns instead of object columns.
-    """
-    _columns = df.select_dtypes(include='object').columns
-    return df.astype({col: 'category' for col in _columns})
+import logging
+import random
+from collections import namedtuple
+from pathlib import Path
+from types import SimpleNamespace
+from typing import List, Optional, Tuple, Union
+
+import matplotlib.dates as mdates
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
+import seaborn
+from njab.sklearn import run_pca
+from sklearn.impute import SimpleImputer
+
+import vaep
+from vaep.analyzers import Analysis
+from vaep.io.datasplits import long_format, wide_format
+from vaep.io.load import verify_df
+from vaep.pandas import _add_indices
+
+logger = logging.getLogger(__name__)
+
+__doc__ = 'A collection of Analyzers to perform certain type of analysis.'
+
+
+ALPHA = 0.5
+
+# ! deprecate AnalyzePeptides
+
+
+class AnalyzePeptides(SimpleNamespace):
+    """Namespace for current analysis
+
+    Attributes
+    ----------
+    df:  pandas.DataFrame
+        current eagerly loaded data in wide format only: sample index, features in columns
+    stats: types.SimpleNamespace
+        Some statistics of certain aspects. Normally each will be a DataFrame.
+
+    Many more attributes are set dynamically depending on the concrete analysis.
+    """
+
+    def __init__(self, data: pd.DataFrame,
+                 is_log_transformed: bool = False,
+                 is_wide_format: bool = True, ind_unstack: str = '',):
+        if not is_wide_format:
+            if not ind_unstack:
+                raise ValueError("Please specify index level for unstacking via "
+                                 f"'ind_unstack' from: {data.index.names}")
+            data = data.unstack(ind_unstack)
+            is_wide_format = True
+        self.df = data  # assume wide
+        self.N, self.M = self.df.shape
+        self.stats = SimpleNamespace()
+        self.is_log_transformed = is_log_transformed
+        self.is_wide_format = is_wide_format
+        self.index_col = self.df.index.name
+
+    @classmethod
+    def from_csv(cls, fname: str,
+                 nrows: int = None,
+                 # could be potentially 0 for the first column
+                 index_col: Union[int, str, List] = 'Sample ID',
+                 verify_fname: bool = False,
+                 usecols=None,
+                 **kwargs):
+        df = pd.read_csv(fname, index_col=index_col, low_memory=False,
+                         nrows=nrows, usecols=usecols).squeeze('columns')
+        if len(df.shape) == 1:
+            # unstack all but first column
+            df = df.unstack(df.index.names[1:])
+        verify_df(df=df, fname=fname,
+                  index_col=index_col,
+                  verify_fname=verify_fname,
+                  usecols=usecols)
+        return cls(data=df, **kwargs)  # all __init__ parameters are kwargs
+
+    @classmethod
+    # @delegates(from_csv)  # does only include parameters with defaults
+    def from_pickle(cls, fname: str,
+                    # could be potentially 0 for the first column
+                    index_col: Union[int, str, List] = 'Sample ID',
+                    verify_fname: bool = False,
+                    usecols=None,
+                    **kwargs):
+        df = pd.read_pickle(fname).squeeze()
+        if len(df.shape) == 1:
+            df = df.unstack(df.index.names[1:])
+        verify_df(df=df, fname=fname,
+                  index_col=index_col,
+                  verify_fname=verify_fname,
+                  usecols=usecols)
+        return cls(data=df, **kwargs)  # all __init__ parameters are kwargs
+
+    def get_consecutive_dates(self, n_samples, seed=42):
+        """Select n consecutive samples using a seed.
+
+        Updated the original DataFrame attribute: df
+        """
+        self.df.sort_index(inplace=True)
+        n_samples = min(len(self.df), n_samples) if n_samples else len(self.df)
+        print(f"Get {n_samples} samples.")
+
+        if seed:
+            random.seed(42)
+
+        _attr_name = f'df_{n_samples}'
+        setattr(self, _attr_name, get_consecutive_data_indices(self.df, n_samples))
+        print("Training data referenced unter:", _attr_name)
+        self.df = getattr(self, _attr_name)
+        print("Updated attribute: df")
+        return self.df
+
+    @property
+    def df_long(self):
+        if hasattr(self, '_df_long'):
+            return self._df_long
+        return self.to_long_format(colname_values='intensity', index_name=self.index_col)
+
+    def to_long_format(
+            self,
+            colname_values: str = 'intensity',
+            index_name: str = 'Sample ID',
+            inplace: str = False) -> pd.DataFrame:
+        """[summary]
+
+        Parameters
+        ----------
+        colname_values : str, optional
+            New column name for values in matrix, by default 'intensity'
+        index_name : str, optional
+            Name of column to assign as index (based on long-data format), by default 'Sample ID'
+        inplace : bool, optional
+            Assign result to df_long (False), or to df (True) attribute, by default False
+        Returns
+        -------
+        pd.DataFrame
+            Data in long-format as DataFrame
+        """
+
+        """Build long data view."""
+        if not self.is_wide_format:
+            return self.df
+        if hasattr(self, '_df_long'):
+            return self._df_long  # rm attribute to overwrite
+
+        df_long = long_format(
+            self.df,
+            colname_values=colname_values,
+            # index_name=index_name
+        )
+
+        if inplace:
+            self.df = df_long
+            self.is_wide_format = False
+            return self.df
+        self._df_long = df_long
+        return df_long
+
+    @property
+    def df_wide(self):
+        return self.to_wide_format()
+
+    def to_wide_format(
+            self,
+            columns: str = 'Sample ID',
+            name_values: str = 'intensity',
+            inplace: bool = False) -> pd.DataFrame:
+        """[summary]
+
+        Parameters
+        ----------
+        columns : str, optional
+            Index level to be shown as columns, by default 'Sample ID'
+        name_values : str, optional
+            Column in long-data format to be used as values, by default 'intensity'
+        inplace : bool, optional
+            Assign result to df_wide (False), or to df (True) attribute, by default False
+
+        Returns
+        -------
+        pd.DataFrame
+            [description]
+        """
+
+        """Build wide data view.
+
+        Return df attribute in case this is in wide-format. If df attribute is in long-format
+        this is used. If df is wide, but long-format exist, then the wide format is build.
+
+
+        """
+        if self.is_wide_format:
+            return self.df
+
+        if hasattr(self, '_df_long'):
+            df = self._df_long
+        else:
+            df = self.df
+
+        df_wide = wide_format(df, columns=columns, name_values=name_values)
+
+        if inplace:
+            self.df = df_wide
+            self.is_wide_format = True
+            return self.df
+        self._df_wide = df_wide
+        print("Set attribute: df_wide")
+        return df_wide
+
+    def describe_peptides(self, sample_n: int = None):
+        if sample_n:
+            df = self.df.sample(n=sample_n, axis=1)
+        else:
+            df = self.df
+        stats = df.describe()
+        stats.loc['CV'] = stats.loc['std'] / stats.loc['mean']
+        self.stats.peptides = stats
+        return stats
+
+    def get_prop_not_na(self):
+        """Get prop. of not NA values for each sample."""
+        return self.df.notna().sum(axis=1) / self.df.shape[-1]
+
+    def get_PCA(self, n_components=2, imputer=SimpleImputer):
+        self.imputer_ = imputer()
+        X = self.imputer_.fit_transform(self.df)
+        X = _add_indices(X, self.df)
+        assert all(X.notna())
+
+        PCs, self.pca_ = run_pca(X, n_components=n_components)
+        if not hasattr(self, 'df_meta'):
+            logger.warning('No metadata available, please set "df_meta" first.')
+        try:
+            PCs['ms_instrument'] = self.df_meta['ms_instrument'].astype('category')
+        except KeyError:
+            logger.warning("No MS instrument added.")
+        except AttributeError:
+            logger.warning("No metadata available, please set 'df_meta' first.")
+            logger.warning("No MS instrument added.")
+        return PCs
+
+    def calculate_PCs(self, new_df, is_wide=True):
+        if not is_wide:
+            new_df = new_df.unstack(new_df.index.names[1:])
+
+        X = self.imputer_.transform(new_df)
+        X = _add_indices(X, new_df)
+        PCs = self.pca_.transform(X)
+        PCs = _add_indices(PCs, new_df, index_only=True)
+        PCs.columns = [f'PC {i+1}' for i in range(PCs.shape[-1])]
+        return PCs
+
+    def plot_pca(self,):
+        """Create principal component plot with three heatmaps showing
+        instrument, degree of non NA data and sample by date."""
+        if not self.is_wide_format:
+            self.df = self.df.unstack(self.df.index.names[1:])
+            self.is_wide_format = True
+
+        if not hasattr(self, 'df_meta'):
+            raise AttributeError('No metadata available, please set "df_meta" first.')
+
+        PCs = self.get_PCA()
+
+        fig, axes = plt.subplots(nrows=3, ncols=1, figsize=(
+            15, 20), constrained_layout=True)
+
+        Dim = namedtuple('DimensionsData', 'N M')
+        self.dim = Dim(*self.df.shape)
+
+        fig.suptitle(
+            f'First two Principal Components of {self.dim.M} most abundant peptides \n for {self.dim.N} samples',
+            fontsize=30)
+
+        # by instrument
+        ax = axes[0]
+        seaborn_scatter(df=PCs.iloc[:, :2], fig=fig, ax=ax,
+                        meta=PCs['ms_instrument'], title='by MS instrument')
+        ax.legend(loc='center right', bbox_to_anchor=(1.11, 0.5))
+
+        # by complettness/missingness
+        # continues colormap will be a bit trickier using seaborn: https://stackoverflow.com/a/44642014/9684872
+        ax = axes[1]
+        plot_scatter(df=PCs.iloc[:, :2], fig=fig, ax=ax,
+                     meta=self.df_meta['prop_not_na'], title='by number on na')
+
+        # by dates
+        ax = axes[2]
+        plot_date_map(df=PCs.iloc[:, :2],
+                      ax=ax, dates=self.df_meta.date)
+
+        return fig
+
+    def log_transform(self, log_fct: np.ufunc):
+        """Log transform data in-place.
+
+        Parameters
+        ----------
+        log_fct : np.ufunc
+            Numpy log-function
+
+        Raises
+        ------
+        Exception
+            if data has been previously log-transformed.
+        """
+        if self.is_log_transformed:
+            raise Exception(
+                f'Data was already log transformed, using {self.__class__.__name__}.log_fct: {self.log_fct}')
+        else:
+            self.df = log_fct(self.df)
+            self.is_log_transformed = True
+            self.log_fct = log_fct
+
+    def get_dectection_limit(self):
+        """Compute information on detection limit in dataset.
+
+        Returns
+        -------
+        str
+            Information on detection limit
+        """
+        self.detection_limit = self.df.min().min() if self.is_log_transformed else np.log10(
+            self.df).min().min()  # all zeros become nan.
+        return "Detection limit: {:6.3f}, corresponding to intensity value of {:,d}".format(
+            self.detection_limit,
+            int(10 ** self.detection_limit))
+
+    def __repr__(self):
+        keys = sorted(self.__dict__)
+        items = ("{}".format(k) for k in keys)
+        return "{} with attributes: {}".format(type(self).__name__, ", ".join(items))
+
+    # def __dir__(self):
+    #     return sorted(self.__dict__)
+
+    @property
+    def fname_stub(self):
+        assert hasattr(self, 'df'), f'Attribute df is missing: {self}'
+        return 'N{:05d}_M{:05d}'.format(*self.df.shape)
+
+
+class LatentAnalysis(Analysis):
+
+    def __init__(self, latent_space: pd.DataFrame, meta_data: pd.DataFrame, model_name: str,
+                 fig_size: Tuple[int, int] = (15, 15), folder: Path = None):
+        self.latent_space, self.meta_data = latent_space, meta_data
+        self.fig_size, self.folder = fig_size, folder
+        self.model_name = model_name
+        self.folder = Path(self.folder) if self.folder else Path('.')
+        assert len(
+            self.latent_space.shape) == 2, "Expected a two dimensional DataFrame."
+        self.latent_dim = self.latent_space.shape[-1]
+        if self.latent_dim > 2:
+            # pca, add option for different methods
+            self.latent_reduced, self.pca_ = run_pca(self.latent_space)
+        else:
+            self.latent_reduced = self.latent_space
+
+    def plot_by_date(self, meta_key: str = 'date', save: bool = True):
+        fig, ax = self._plot(fct=plot_date_map, meta_key=meta_key, save=save)
+        return fig, ax
+
+    def plot_by_category(self, meta_key: str, save: bool = True):
+        fig, ax = self._plot(fct=seaborn_scatter, meta_key=meta_key, save=save)
+        return fig, ax
+
+    def _plot(self, fct, meta_key: str, save: bool = True):
+        try:
+            meta_data = self.meta_data[meta_key]
+        except KeyError:
+            raise ValueError(f"Requested key: '{meta_key}' is not in available,"
+                             f" use: {', '.join(x for x in self.meta_data.columns)}")
+        fig, ax = plt.subplots(figsize=self.fig_size)
+        _ = fct(df=self.latent_reduced, ax=ax,
+                meta=meta_data.loc[self.latent_reduced.index],
+                title=f'{self.model_name} latent space PCA of {self.latent_dim} dimensions by {meta_key}')
+        if save:
+            vaep.plotting._savefig(fig, name=f'{self.model_name}_latent_by_{meta_key}',
+                                   folder=self.folder)
+        return fig, ax
+
+
+# def read_csv(fname:str, nrows:int, index_col:str=None)-> pd.DataFrame:
+#     return pd.read_csv(fname, index_col=index_col, low_memory=False, nrows=nrows)
+
+
+def get_consecutive_data_indices(df, n_samples):
+    index = df.sort_index().index
+    start_sample = len(index) - n_samples
+    start_sample = random.randint(0, start_sample)
+    return df.loc[index[start_sample:start_sample + n_samples]]
+
+
+def corr_lower_triangle(df):
+    """Compute the correlation matrix, returning only unique values."""
+    corr_df = df.corr()
+    lower_triangle = pd.DataFrame(
+        np.tril(np.ones(corr_df.shape), -1)).astype(bool)
+    lower_triangle.index, lower_triangle.columns = corr_df.index, corr_df.columns
+    return corr_df.where(lower_triangle)
+
+
+def plot_corr_histogram(corr_lower_triangle, bins=10):
+    fig, axes = plt.subplots(ncols=2, gridspec_kw={"width_ratios": [
+        5, 1], "wspace": 0.2}, figsize=(8, 4))
+    values = pd.Series(corr_lower_triangle.to_numpy().flatten()).dropna()
+    ax = axes[0]
+    ax = values.hist(ax=ax, bins=bins)
+    ax.yaxis.set_major_formatter("{x:,.0f}")
+    ax = axes[1]
+    plt.axis('off')
+    data = values.describe(percentiles=np.linspace(0.1, 1, 10)).round(2)
+    data.name = ''
+    _ = pd.plotting.table(ax=ax, data=data, loc="best", edges="open")
+    return fig, axes
+
+
+def plot_date_map(df, ax,
+                  dates: pd.Series = None,
+                  meta: pd.Series = None,
+                  title: str = 'by date',
+                  fontsize=8,
+                  size=2):
+    if dates is not None and meta is not None:
+        raise ValueError("Only set either dates or meta parameters.")
+        # ToDo: Clean up arguments
+    if dates is None:
+        dates = meta
+    cols = list(df.columns)
+    assert len(cols) == 2, f'Please provide two dimensons, not {df.columns}'
+    ax.set_title(title, fontsize=fontsize)
+    ax.set_xlabel(cols[0])
+    ax.set_ylabel(cols[1])
+    path_collection = scatter_plot_w_dates(
+        ax, df, dates=dates, errors='raise')
+    _ = add_date_colorbar(path_collection, ax=ax)
+
+
+def plot_scatter(df, ax,
+                 meta: pd.Series,
+                 feat_name_display: str = 'features',
+                 title: Optional[str] = None,
+                 alpha=ALPHA,
+                 fontsize=8,
+                 size=2):
+    cols = list(df.columns)
+    assert len(cols) == 2, f'Please provide two dimensons, not {df.columns}'
+    if not title:
+        title = f'by identified {feat_name_display}'
+    ax.set_title(title, fontsize=fontsize)
+    ax.set_xlabel(cols[0])
+    ax.set_ylabel(cols[1])
+    path_collection = ax.scatter(
+        x=cols[0], y=cols[1], s=size, c=meta, data=df, alpha=alpha)
+    _ = ax.get_figure().colorbar(path_collection, ax=ax,
+                                 label=f'Identified {feat_name_display}',
+                                 #  ticklocation='left', # ignored by matplotlib
+                                 location='right',  # ! left does not put colobar without overlapping y ticks
+                                 format="{x:,.0f}",
+                                 )
+
+
+def seaborn_scatter(df, ax,
+                    meta: pd.Series,
+                    title: str = 'by some metadata',
+                    alpha=ALPHA,
+                    fontsize=5,
+                    size=5):
+    cols = list(df.columns)
+    assert len(cols) == 2, f'Please provide two dimensons, not {df.columns}'
+    seaborn.scatterplot(x=df[cols[0]], y=df[cols[1]],
+                        hue=meta, ax=ax, palette='deep', s=size, alpha=alpha)
+    _ = ax.legend(fontsize=fontsize,
+                  title_fontsize=fontsize,
+                  markerscale=0.4,
+                  title=meta.name,
+                  )
+    ax.set_title(title, fontsize=fontsize)
+    return ax
+
+
+def scatter_plot_w_dates(ax, df,
+                         dates=None,
+                         marker=None,
+                         errors='raise',
+                         size=2):
+    """plot first vs. second column in DataFrame.
+    Use dates to color data.
+
+
+
+    errors : {'ignore', 'raise', 'coerce'}, default 'raise'
+        Passed on to pandas.to_datetime
+        - If 'raise', then invalid parsing will raise an exception.
+        - If 'coerce', then invalid parsing will be set as NaT.
+        - If 'ignore', then invalid parsing will return the input.
+    """
+    # Inspiration:  https://stackoverflow.com/a/59685599/9684872
+    cols = df.columns
+
+    if isinstance(dates, str):
+        dates = df['dates']
+
+    path_collection = ax.scatter(
+        x=df[cols[0]],
+        y=df[cols[1]],
+        c=[mdates.date2num(t) for t in pd.to_datetime(dates, errors=errors)
+           ] if dates is not None else None,
+        alpha=ALPHA,
+        s=size,
+        marker=marker,
+    )
+    return path_collection
+
+
+def add_date_colorbar(mappable, ax):
+    loc = mdates.AutoDateLocator()
+    cbar = ax.get_figure().colorbar(mappable, ax=ax, ticks=loc,
+                                    format=mdates.AutoDateFormatter(loc))
+    return cbar
+
+
+def cast_object_to_category(df: pd.DataFrame) -> pd.DataFrame:
+    """Cast object columns to category dtype.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        DataFrame with columns
+
+    Returns
+    -------
+    pd.DataFrame
+        DataFrame with category columns instead of object columns.
+    """
+    _columns = df.select_dtypes(include='object').columns
+    return df.astype({col: 'category' for col in _columns})
```

### Comparing `pimms-learn-0.2.0/vaep/analyzers/compare_predictions.py` & `pimms_learn-0.3.0/vaep/analyzers/compare_predictions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,86 +1,87 @@
-from __future__ import annotations
-
-from pathlib import Path
-
-import pandas as pd
-from typing import List
-
-
-def load_predictions(pred_files: List, shared_columns=['observed']):
-
-    pred_files = iter(pred_files)
-    fname = next(pred_files)
-    pred = pd.read_csv(fname, index_col=[0, 1])
-
-    for fname in pred_files:
-        _pred_file = pd.read_csv(fname, index_col=[0, 1])
-        if shared_columns:
-            assert all(pred[shared_columns] == _pred_file[shared_columns])
-            pred = pred.join(_pred_file.drop(shared_columns, axis=1))
-        else:
-            pred = pred.join(_pred_file)
-    return pred
-
-
-def load_split_prediction_by_modelkey(experiment_folder: Path,
-                                      split: str,
-                                      model_keys: list[str],
-                                      allow_missing=False,
-                                      shared_columns: list[str] = None):
-    """Load predictions from a list of models.
-
-    Parameters
-    ----------
-    experiment_folder : Path
-        Path to experiment folder
-    split : str
-        which split of simulated data to load
-    model_keys : List
-        List of model keys to be loaded
-    allow_missing : bool, optional
-        Ignore missing pred files of requested model, default False
-    shared_columns : List, optional
-        List of columns that are shared between all models, by default ['observed']
-
-    Returns
-    -------
-    pd.DataFrame
-        Prediction data frame with shared columns and model predictions
-    """
-    pred_files = [experiment_folder / 'preds' /
-                  f'pred_{split}_{key}.csv' for key in model_keys]
-    to_remove = list()
-    for file in pred_files:
-        if not file.exists():
-            if allow_missing:
-                print(f'WARNING: {file} does not exist')
-                to_remove.append(file)
-            else:
-                raise FileNotFoundError(f'{file} does not exist')
-    if to_remove:
-        for file in to_remove:
-            pred_files.remove(to_remove)
-    return load_predictions(pred_files, shared_columns=shared_columns)
-
-
-def load_single_csv_pred_file(fname: str | Path, value_name: str = 'intensity') -> pd.Series:
-    """Load a single pred file from a single model.
-     Last column are measurments, other are index.
-
-    Parameters
-    ----------
-    fname : str | Path
-        Path to csv file to be loaded
-    value_name : str, optional
-        name for measurments to be used, by default 'intensity'
-
-    Returns
-    -------
-    pd.Series
-        measurments as a single column with set indices
-    """
-    pred = pd.read_csv(fname)  # getattr for other file formats
-    pred = pred.set_index(pred.columns[:-1].tolist())
-    pred = pred.squeeze()
-    pred.name = value_name
-    return pred
+from __future__ import annotations
+
+from pathlib import Path
+from typing import List
+
+import pandas as pd
+
+
+def load_predictions(pred_files: List, shared_columns=['observed']):
+
+    pred_files = iter(pred_files)
+    fname = next(pred_files)
+    pred = pd.read_csv(fname, index_col=[0, 1])
+
+    for fname in pred_files:
+        _pred_file = pd.read_csv(fname, index_col=[0, 1])
+        idx_shared = pred.index.intersection(_pred_file.index)
+        assert len(idx_shared), f'No shared index between already loaded models {pred.columns} and {fname}'
+        if shared_columns:
+            assert all(pred.loc[idx_shared, shared_columns] == _pred_file.loc[idx_shared, shared_columns])
+            pred = pred.join(_pred_file.drop(shared_columns, axis=1))
+        else:
+            pred = pred.join(_pred_file)
+    return pred
+
+
+def load_split_prediction_by_modelkey(experiment_folder: Path,
+                                      split: str,
+                                      model_keys: list[str],
+                                      allow_missing=False,
+                                      shared_columns: list[str] = None):
+    """Load predictions from a list of models.
+
+    Parameters
+    ----------
+    experiment_folder : Path
+        Path to experiment folder
+    split : str
+        which split of simulated data to load
+    model_keys : List
+        List of model keys to be loaded
+    allow_missing : bool, optional
+        Ignore missing pred files of requested model, default False
+    shared_columns : List, optional
+        List of columns that are shared between all models, by default None
+
+    Returns
+    -------
+    pd.DataFrame
+        Prediction data frame with shared columns and model predictions
+    """
+    pred_files = [experiment_folder / 'preds' /
+                  f'pred_{split}_{key}.csv' for key in model_keys]
+    to_remove = list()
+    for file in pred_files:
+        if not file.exists():
+            if allow_missing:
+                print(f'WARNING: {file} does not exist')
+                to_remove.append(file)
+            else:
+                raise FileNotFoundError(f'{file} does not exist')
+    if to_remove:
+        pred_files.remove(to_remove)
+    return load_predictions(pred_files, shared_columns=shared_columns)
+
+
+def load_single_csv_pred_file(fname: str | Path, value_name: str = 'intensity') -> pd.Series:
+    """Load a single pred file from a single model.
+     Last column are measurments, other are index.
+
+    Parameters
+    ----------
+    fname : str | Path
+        Path to csv file to be loaded
+    value_name : str, optional
+        name for measurments to be used, by default 'intensity'
+
+    Returns
+    -------
+    pd.Series
+        measurments as a single column with set indices
+    """
+    pred = pd.read_csv(fname)  # getattr for other file formats
+    pred = pred.set_index(pred.columns[:-1].tolist())
+    pred = pred.squeeze()
+    pred.name = value_name
+    return pred
```

### Comparing `pimms-learn-0.2.0/vaep/analyzers/diff_analysis.py` & `pimms_learn-0.3.0/vaep/analyzers/diff_analysis.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from __future__ import annotations
-from collections import namedtuple
-import logging
-
-import pandas as pd
-
-logger = logging.getLogger()
-
-
-Cutoffs = namedtuple('Cutoffs', 'feat_completness_over_samples min_feat_in_sample')
-
-
-def select_raw_data(df: pd.DataFrame,
-                    data_completeness: float,
-                    frac_protein_groups: int) -> tuple[pd.DataFrame, Cutoffs]:
-    msg = 'N samples: {}, M feat: {}'
-    N, M = df.shape
-    logger.info("Initally: " + msg.format(N, M))
-    min_sample_for_feat = int(N * data_completeness)
-    df = df.dropna(axis=1, thresh=min_sample_for_feat)
-    logger.info(
-        f"Dropped features quantified in less than {int(min_sample_for_feat)} samples.")
-    N, M = df.shape
-    logger.info("After feat selection: " + msg.format(N, M))
-    min_feat_per_sample = int(M * frac_protein_groups)
-    logger.info(
-        f"Min No. of Protein-Groups in single sample: {min_feat_per_sample}")
-    df = df.dropna(axis=0, thresh=min_feat_per_sample)
-    logger.info("Finally: " + msg.format(*df.shape))
-
-    return df, Cutoffs(min_sample_for_feat, min_feat_per_sample)
-
-
-def select_feat(df_qc: pd.DataFrame, threshold: float = 0.4, axis: int = 0):
-    qc_cv_feat = df_qc.std(axis=axis) / df_qc.mean(axis=axis)
-    mask = qc_cv_feat < threshold
-    return qc_cv_feat.loc[mask].index
+from __future__ import annotations
+from collections import namedtuple
+import logging
+
+import pandas as pd
+
+logger = logging.getLogger()
+
+
+Cutoffs = namedtuple('Cutoffs', 'feat_completness_over_samples min_feat_in_sample')
+
+
+def select_raw_data(df: pd.DataFrame,
+                    data_completeness: float,
+                    frac_protein_groups: int) -> tuple[pd.DataFrame, Cutoffs]:
+    msg = 'N samples: {}, M feat: {}'
+    N, M = df.shape
+    logger.info("Initally: " + msg.format(N, M))
+    min_sample_for_feat = int(N * data_completeness)
+    df = df.dropna(axis=1, thresh=min_sample_for_feat)
+    logger.info(
+        f"Dropped features quantified in less than {int(min_sample_for_feat)} samples.")
+    N, M = df.shape
+    logger.info("After feat selection: " + msg.format(N, M))
+    min_feat_per_sample = int(M * frac_protein_groups)
+    logger.info(
+        f"Min No. of Protein-Groups in single sample: {min_feat_per_sample}")
+    df = df.dropna(axis=0, thresh=min_feat_per_sample)
+    logger.info("Finally: " + msg.format(*df.shape))
+
+    return df, Cutoffs(min_sample_for_feat, min_feat_per_sample)
+
+
+def select_feat(df_qc: pd.DataFrame, threshold: float = 0.4, axis: int = 0):
+    qc_cv_feat = df_qc.std(axis=axis) / df_qc.mean(axis=axis)
+    mask = qc_cv_feat < threshold
+    return qc_cv_feat.loc[mask].index
```

### Comparing `pimms-learn-0.2.0/vaep/data_handling.py` & `pimms_learn-0.3.0/vaep/data_handling.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-"""
-Functionality to handle protein and peptide datasets.
-"""
-import numpy as np
-import pandas as pd
-
-# coverage
-
-
-def coverage(X: pd.DataFrame, coverage_col: float, coverage_row: float):
-    """Select proteins by column depending on their coverage.
-    Of these selected proteins, where the rows have a certain number of overall proteins.
-    """
-    mask_col = X.isnull().mean() <= 1 - coverage_col
-    df = X.loc[:, mask_col]
-    mask_row = df.isnull().mean(axis=1) <= 1 - coverage_row
-    df = df.loc[mask_row, :]
-    return df
-
-
-def compute_stats_missing(X: pd.DataFrame,
-                          col_no_missing: str = 'no_missing',
-                          col_no_identified: str = 'no_identified',
-                          col_prop_samples: str = 'prop_samples') -> pd.DataFrame:
-    """Dataset of repeated samples indicating if an observation
-    has the variables observed or missing x in {0,1}"""
-    if X.index.name:
-        index_col = X.index.name
-    else:
-        index_col = 'INDEX'
-    sample_stats = X.index.to_frame(index=False).reset_index()
-    sample_stats.columns = ['SampleID_int', index_col]
-    sample_stats.set_index(index_col, inplace=True)
-
-    sample_stats[col_no_identified] = X.sum(axis=1)
-    sample_stats[col_no_missing] = (X == 0).sum(axis=1)
-
-    assert all(sample_stats[[col_no_identified, col_no_missing]].sum(
-        axis=1) == X.shape[1])
-    sample_stats = sample_stats.sort_values(
-        by=col_no_identified, ascending=False)
-    sample_stats[col_prop_samples] = np.array(
-        range(1, len(sample_stats) + 1)) / len(sample_stats)
-    return sample_stats
-
-
-def get_sorted_not_missing(X: pd.DataFrame) -> pd.DataFrame:
-    """Return a Dataframe with missing values. Order columns by degree of completness
-    over columns from variables least to most shared among observations."""
-    X = X.notna().astype(int)
-    return X[X.mean().sort_values().index]
+"""
+Functionality to handle protein and peptide datasets.
+"""
+import numpy as np
+import pandas as pd
+
+# coverage
+
+
+def coverage(X: pd.DataFrame, coverage_col: float, coverage_row: float):
+    """Select proteins by column depending on their coverage.
+    Of these selected proteins, where the rows have a certain number of overall proteins.
+    """
+    mask_col = X.isnull().mean() <= 1 - coverage_col
+    df = X.loc[:, mask_col]
+    mask_row = df.isnull().mean(axis=1) <= 1 - coverage_row
+    df = df.loc[mask_row, :]
+    return df
+
+
+def compute_stats_missing(X: pd.DataFrame,
+                          col_no_missing: str = 'no_missing',
+                          col_no_identified: str = 'no_identified',
+                          col_prop_samples: str = 'prop_samples') -> pd.DataFrame:
+    """Dataset of repeated samples indicating if an observation
+    has the variables observed or missing x in {0,1}"""
+    if X.index.name:
+        index_col = X.index.name
+    else:
+        index_col = 'INDEX'
+    sample_stats = X.index.to_frame(index=False).reset_index()
+    sample_stats.columns = ['SampleID_int', index_col]
+    sample_stats.set_index(index_col, inplace=True)
+
+    sample_stats[col_no_identified] = X.sum(axis=1)
+    sample_stats[col_no_missing] = (X == 0).sum(axis=1)
+
+    assert all(sample_stats[[col_no_identified, col_no_missing]].sum(
+        axis=1) == X.shape[1])
+    sample_stats = sample_stats.sort_values(
+        by=col_no_identified, ascending=False)
+    sample_stats[col_prop_samples] = np.array(
+        range(1, len(sample_stats) + 1)) / len(sample_stats)
+    return sample_stats
+
+
+def get_sorted_not_missing(X: pd.DataFrame) -> pd.DataFrame:
+    """Return a Dataframe with missing values. Order columns by degree of completness
+    over columns from variables least to most shared among observations."""
+    X = X.notna().astype(int)
+    return X[X.mean().sort_values().index]
```

### Comparing `pimms-learn-0.2.0/vaep/imputation.py` & `pimms_learn-0.3.0/vaep/imputation.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,251 +1,251 @@
-"""
-Reduce number of missing values of DDA massspectromety.
-
-Imputation can be down by column.
-
-
-"""
-from typing import Tuple, Dict
-from sklearn.neighbors import NearestNeighbors
-import scipy
-import numpy as np
-import pandas as pd
-import logging
-
-logger = logging.getLogger(__name__)
-
-
-RANDOMSEED = 123
-
-
-def impute_missing(protein_values, mean=None, std=None):
-    """
-    Imputation is based on the mean and standard deviation
-    from the protein_values.
-    If mean and standard deviation (std) are given,
-    missing values are imputed and protein_values are returned imputed.
-    If no mean and std are given, the mean and std are computed from
-    the non-missing protein_values.
-
-    Parameters
-    ----------
-    protein_values: Iterable
-    mean: float
-    std: float
-
-    Returns
-    ------
-    protein_values: pandas.Series
-    """
-    raise NotImplementedError('Will be the main function combining features')
-    # clip by zero?
-
-
-def _select_data(data: pd.DataFrame, threshold: float):
-    """Select (protein-) columns for imputation.
-
-    Based on the threshold representing the minimum proportion of available
-    data per protein, the columns of a `pandas.DataFrame` are selected.
-
-    Parameters
-    ----------
-    data: pandas.DataFrame
-    threshold: float
-        Threshold of percentage of non-missing values to select a column/feature.
-    """
-    columns_to_impute = data.notnull().mean() >= threshold
-    return columns_to_impute
-
-
-def _sparse_coo_array(data: pd.DataFrame):
-    """Return a sparse scipy matrix from dense `pandas.DataFrame` with many
-    missing values.
-    """
-    indices = np.nonzero(~np.isnan(data.to_numpy()))
-    data_selected_sparse = data.to_numpy()
-    data_selected_sparse = scipy.sparse.coo_matrix(
-        (data_selected_sparse[indices], indices),
-        shape=data_selected_sparse.shape)
-    return data_selected_sparse
-
-
-def _get_weighted_mean(distances, data):
-    """Compute weighted mean ignoring
-    identical entries"""
-    mask = distances > 0.0
-    weights = distances[mask] / distances[mask].sum()
-    weighted_sum = data.loc[mask].mul(weights, axis=0)
-    mean_imputed = weighted_sum.sum() / sum(mask)
-    return mean_imputed
-
-
-# define imputation methods
-# could be done in PCA transformed space
-def imputation_KNN(data, alone=True, threshold=0.5):
-    """
-
-
-    Parameters
-    ----------
-    data: pandas.DataFrame
-    alone: bool  # is not used
-    threshold: float
-        Threshold of missing data by column in interval (0, 1)
-    """
-    mask_selected = _select_data(data=data, threshold=threshold)
-    data_selected = data.loc[:, mask_selected].copy()
-    data_selected_sparse = _sparse_coo_array(data_selected)
-    # impute
-    knn_fitted = NearestNeighbors(n_neighbors=3, algorithm='brute').fit(
-        data_selected_sparse)
-    fit_distances, fit_neighbors = knn_fitted.kneighbors(data_selected_sparse)
-    for i, (distances, ids) in enumerate(zip(fit_distances, fit_neighbors)):
-        mean_imputed = _get_weighted_mean(distances, data_selected.loc[ids])
-        if all(distances == 0.0):
-            logger.warning(f"Did not find any neighbor for int-id: {i}")
-        else:
-            assert i == ids[distances == 0.0], (
-                "None or more then one identical data points "
-                "for ids: {}".format(ids[distances == 0.0])
-            )
-        mask = data_selected.iloc[i].isna()
-        data_selected.loc[i, mask] = mean_imputed.loc[mask]  # SettingWithCopyError
-
-    data.update(data_selected)
-    return data
-
-
-def imputation_normal_distribution(log_intensities: pd.Series,
-                                   mean_shift=1.8,
-                                   std_shrinkage=0.3,
-                                   copy=True):
-    """Impute missing log-transformed intensity values of a single feature.
-    Samples one value for imputation for all samples.
-
-    Parameters
-    ----------
-    log_intensities: pd.Series
-        Series of normally distributed values of a single feature (for all samples/runs).
-        Here usually log-transformed intensities.
-    mean_shift: integer, float
-        Shift the mean of the log_intensities by factors of their standard
-        deviation to the negative.
-    std_shrinkage: float
-        Value greater than zero by which to shrink (or inflate) the
-        standard deviation of the log_intensities.
-    """
-    np.random.seed(RANDOMSEED)
-    if not isinstance(log_intensities, pd.Series):
-        try:
-            log_intensities.Series(log_intensities)
-            logger.warning("Series created of Iterable.")
-        except BaseException:
-            raise ValueError(
-                "Plese provided data which is a pandas.Series or an Iterable")
-    if mean_shift < 0:
-        raise ValueError(
-            "Please specify a positive float as the std.-dev. is non-negative.")
-    if std_shrinkage <= 0:
-        raise ValueError(
-            "Please specify a positive float as shrinkage factor for std.-dev.")
-    if std_shrinkage >= 1:
-        logger.warning("Standard Deviation will increase for imputed values.")
-
-    mean = log_intensities.mean()
-    std = log_intensities.std()
-
-    mean_shifted = mean - (std * mean_shift)
-    std_shrinked = std * std_shrinkage
-
-    if copy:
-        log_intensities = log_intensities.copy(deep=True)
-
-    return log_intensities.where(log_intensities.notna(),
-                                 np.random.normal(mean_shifted, std_shrinked))
-
-
-def impute_shifted_normal(df_wide: pd.DataFrame,
-                          mean_shift: float = 1.8,
-                          std_shrinkage: float = 0.3,
-                          completeness: float = 0.6,
-                          axis=1,
-                          seed=RANDOMSEED) -> pd.Series:
-    """Get replacements for missing values.
-
-    Parameters
-    ----------
-    df_wide : pd.DataFrame
-        DataFrame in wide format, contains missing
-    mean_shift : float, optional
-        shift mean of feature by factor of standard deviations, by default 1.8
-    std_shrinkage : float, optional
-        shrinks standard deviation by facotr, by default 0.3
-    axis: int, optional
-        axis along which to impute, by default 1 (i.e. mean and std per row)
-
-    Returns
-    -------
-    pd.Series
-        Series of imputed values in long format.
-    """
-    # add check if there ar e NaNs or inf in data? see tests
-    # np.isinf(df_wide).values.sum()
-    if axis == 1:
-        min_N = int(len(df_wide) * completeness)
-        selected = df_wide.dropna(axis=1, thresh=min_N)
-    elif axis == 0:
-        min_M = int(df_wide.shape[1] * completeness)
-        selected = df_wide.dropna(axis=0, thresh=min_M)
-    else:
-        raise ValueError(
-            "Please specify axis as 0 or 1, for axis along which to impute.")
-    logger.info(
-        f"Meand and standard deviation based on seleted data of shape {selected.shape}")
-    mean = selected.mean(axis=axis)
-    std = selected.std(axis=axis)
-    mean_shifted = mean - (std * mean_shift)
-    std_shrinked = std * std_shrinkage
-    # rng=np.random.default_rng(seed=seed)
-    # rng.normal()
-    np.random.seed(seed)
-    N, M = df_wide.shape
-    if axis == 1:
-        imputed_shifted_normal = pd.DataFrame(
-            np.random.normal(mean_shifted, std_shrinked, size=(M, N)),
-            index=df_wide.columns,
-            columns=df_wide.index)
-        imputed_shifted_normal = imputed_shifted_normal.T
-    else:
-        imputed_shifted_normal = pd.DataFrame(
-            np.random.normal(mean_shifted, std_shrinked, size=(N, M)),
-            index=df_wide.index,
-            columns=df_wide.columns)
-    imputed_shifted_normal = imputed_shifted_normal[df_wide.isna()].stack()
-    return imputed_shifted_normal
-
-
-def imputation_mixed_norm_KNN(data):
-    # impute columns with less than 50% missing values with KNN
-    data = imputation_KNN(data, alone=False)  # ToDo: Alone is not used.
-    # impute remaining columns based on the distribution of the protein
-    data = imputation_normal_distribution(
-        data, mean_shift=1.8, std_shrinkage=0.3)
-    return data
-
-
-def compute_moments_shift(observed: pd.Series, imputed: pd.Series,
-                          names: Tuple[str, str] = ('observed', 'imputed')) -> Dict[str, float]:
-    """Summary of overall shift of mean and std. dev. of predictions for a imputation method."""
-    name_obs, name_model = names
-    data = {name: {'mean': series.mean(), 'std': series.std()} for series, name in zip([observed, imputed], names)}
-    observed, imputed = data[name_obs], data[name_model]
-    data[name_model]['mean shift (in std)'] = (observed["mean"] - imputed["mean"]) / observed["std"]
-    data[name_model]['std shrinkage'] = imputed["std"] / observed["std"]
-    return data
-
-
-def stats_by_level(series: pd.Series, index_level: int = 0, min_count: int = 5) -> pd.Series:
-    """Count, mean and std. dev. by index level."""
-    agg = series.groupby(level=index_level).agg(['count', 'mean', 'std'])
-    agg = agg.loc[agg['count'] > min_count]
-    return agg.mean()
+"""
+Reduce number of missing values of DDA massspectromety.
+
+Imputation can be down by column.
+
+
+"""
+from typing import Tuple, Dict
+from sklearn.neighbors import NearestNeighbors
+import scipy
+import numpy as np
+import pandas as pd
+import logging
+
+logger = logging.getLogger(__name__)
+
+
+RANDOMSEED = 123
+
+
+def impute_missing(protein_values, mean=None, std=None):
+    """
+    Imputation is based on the mean and standard deviation
+    from the protein_values.
+    If mean and standard deviation (std) are given,
+    missing values are imputed and protein_values are returned imputed.
+    If no mean and std are given, the mean and std are computed from
+    the non-missing protein_values.
+
+    Parameters
+    ----------
+    protein_values: Iterable
+    mean: float
+    std: float
+
+    Returns
+    ------
+    protein_values: pandas.Series
+    """
+    raise NotImplementedError('Will be the main function combining features')
+    # clip by zero?
+
+
+def _select_data(data: pd.DataFrame, threshold: float):
+    """Select (protein-) columns for imputation.
+
+    Based on the threshold representing the minimum proportion of available
+    data per protein, the columns of a `pandas.DataFrame` are selected.
+
+    Parameters
+    ----------
+    data: pandas.DataFrame
+    threshold: float
+        Threshold of percentage of non-missing values to select a column/feature.
+    """
+    columns_to_impute = data.notnull().mean() >= threshold
+    return columns_to_impute
+
+
+def _sparse_coo_array(data: pd.DataFrame):
+    """Return a sparse scipy matrix from dense `pandas.DataFrame` with many
+    missing values.
+    """
+    indices = np.nonzero(~np.isnan(data.to_numpy()))
+    data_selected_sparse = data.to_numpy()
+    data_selected_sparse = scipy.sparse.coo_matrix(
+        (data_selected_sparse[indices], indices),
+        shape=data_selected_sparse.shape)
+    return data_selected_sparse
+
+
+def _get_weighted_mean(distances, data):
+    """Compute weighted mean ignoring
+    identical entries"""
+    mask = distances > 0.0
+    weights = distances[mask] / distances[mask].sum()
+    weighted_sum = data.loc[mask].mul(weights, axis=0)
+    mean_imputed = weighted_sum.sum() / sum(mask)
+    return mean_imputed
+
+
+# define imputation methods
+# could be done in PCA transformed space
+def imputation_KNN(data, alone=True, threshold=0.5):
+    """
+
+
+    Parameters
+    ----------
+    data: pandas.DataFrame
+    alone: bool  # is not used
+    threshold: float
+        Threshold of missing data by column in interval (0, 1)
+    """
+    mask_selected = _select_data(data=data, threshold=threshold)
+    data_selected = data.loc[:, mask_selected].copy()
+    data_selected_sparse = _sparse_coo_array(data_selected)
+    # impute
+    knn_fitted = NearestNeighbors(n_neighbors=3, algorithm='brute').fit(
+        data_selected_sparse)
+    fit_distances, fit_neighbors = knn_fitted.kneighbors(data_selected_sparse)
+    for i, (distances, ids) in enumerate(zip(fit_distances, fit_neighbors)):
+        mean_imputed = _get_weighted_mean(distances, data_selected.loc[ids])
+        if all(distances == 0.0):
+            logger.warning(f"Did not find any neighbor for int-id: {i}")
+        else:
+            assert i == ids[distances == 0.0], (
+                "None or more then one identical data points "
+                "for ids: {}".format(ids[distances == 0.0])
+            )
+        mask = data_selected.iloc[i].isna()
+        data_selected.loc[i, mask] = mean_imputed.loc[mask]  # SettingWithCopyError
+
+    data.update(data_selected)
+    return data
+
+
+def imputation_normal_distribution(log_intensities: pd.Series,
+                                   mean_shift=1.8,
+                                   std_shrinkage=0.3,
+                                   copy=True):
+    """Impute missing log-transformed intensity values of a single feature.
+    Samples one value for imputation for all samples.
+
+    Parameters
+    ----------
+    log_intensities: pd.Series
+        Series of normally distributed values of a single feature (for all samples/runs).
+        Here usually log-transformed intensities.
+    mean_shift: integer, float
+        Shift the mean of the log_intensities by factors of their standard
+        deviation to the negative.
+    std_shrinkage: float
+        Value greater than zero by which to shrink (or inflate) the
+        standard deviation of the log_intensities.
+    """
+    np.random.seed(RANDOMSEED)
+    if not isinstance(log_intensities, pd.Series):
+        try:
+            log_intensities.Series(log_intensities)
+            logger.warning("Series created of Iterable.")
+        except BaseException:
+            raise ValueError(
+                "Plese provided data which is a pandas.Series or an Iterable")
+    if mean_shift < 0:
+        raise ValueError(
+            "Please specify a positive float as the std.-dev. is non-negative.")
+    if std_shrinkage <= 0:
+        raise ValueError(
+            "Please specify a positive float as shrinkage factor for std.-dev.")
+    if std_shrinkage >= 1:
+        logger.warning("Standard Deviation will increase for imputed values.")
+
+    mean = log_intensities.mean()
+    std = log_intensities.std()
+
+    mean_shifted = mean - (std * mean_shift)
+    std_shrinked = std * std_shrinkage
+
+    if copy:
+        log_intensities = log_intensities.copy(deep=True)
+
+    return log_intensities.where(log_intensities.notna(),
+                                 np.random.normal(mean_shifted, std_shrinked))
+
+
+def impute_shifted_normal(df_wide: pd.DataFrame,
+                          mean_shift: float = 1.8,
+                          std_shrinkage: float = 0.3,
+                          completeness: float = 0.6,
+                          axis=1,
+                          seed=RANDOMSEED) -> pd.Series:
+    """Get replacements for missing values.
+
+    Parameters
+    ----------
+    df_wide : pd.DataFrame
+        DataFrame in wide format, contains missing
+    mean_shift : float, optional
+        shift mean of feature by factor of standard deviations, by default 1.8
+    std_shrinkage : float, optional
+        shrinks standard deviation by facotr, by default 0.3
+    axis: int, optional
+        axis along which to impute, by default 1 (i.e. mean and std per row)
+
+    Returns
+    -------
+    pd.Series
+        Series of imputed values in long format.
+    """
+    # add check if there ar e NaNs or inf in data? see tests
+    # np.isinf(df_wide).values.sum()
+    if axis == 1:
+        min_N = int(len(df_wide) * completeness)
+        selected = df_wide.dropna(axis=1, thresh=min_N)
+    elif axis == 0:
+        min_M = int(df_wide.shape[1] * completeness)
+        selected = df_wide.dropna(axis=0, thresh=min_M)
+    else:
+        raise ValueError(
+            "Please specify axis as 0 or 1, for axis along which to impute.")
+    logger.info(
+        f"Meand and standard deviation based on seleted data of shape {selected.shape}")
+    mean = selected.mean(axis=axis)
+    std = selected.std(axis=axis)
+    mean_shifted = mean - (std * mean_shift)
+    std_shrinked = std * std_shrinkage
+    # rng=np.random.default_rng(seed=seed)
+    # rng.normal()
+    np.random.seed(seed)
+    N, M = df_wide.shape
+    if axis == 1:
+        imputed_shifted_normal = pd.DataFrame(
+            np.random.normal(mean_shifted, std_shrinked, size=(M, N)),
+            index=df_wide.columns,
+            columns=df_wide.index)
+        imputed_shifted_normal = imputed_shifted_normal.T
+    else:
+        imputed_shifted_normal = pd.DataFrame(
+            np.random.normal(mean_shifted, std_shrinked, size=(N, M)),
+            index=df_wide.index,
+            columns=df_wide.columns)
+    imputed_shifted_normal = imputed_shifted_normal[df_wide.isna()].stack()
+    return imputed_shifted_normal
+
+
+def imputation_mixed_norm_KNN(data):
+    # impute columns with less than 50% missing values with KNN
+    data = imputation_KNN(data, alone=False)  # ToDo: Alone is not used.
+    # impute remaining columns based on the distribution of the protein
+    data = imputation_normal_distribution(
+        data, mean_shift=1.8, std_shrinkage=0.3)
+    return data
+
+
+def compute_moments_shift(observed: pd.Series, imputed: pd.Series,
+                          names: Tuple[str, str] = ('observed', 'imputed')) -> Dict[str, float]:
+    """Summary of overall shift of mean and std. dev. of predictions for a imputation method."""
+    name_obs, name_model = names
+    data = {name: {'mean': series.mean(), 'std': series.std()} for series, name in zip([observed, imputed], names)}
+    observed, imputed = data[name_obs], data[name_model]
+    data[name_model]['mean shift (in std)'] = (observed["mean"] - imputed["mean"]) / observed["std"]
+    data[name_model]['std shrinkage'] = imputed["std"] / observed["std"]
+    return data
+
+
+def stats_by_level(series: pd.Series, index_level: int = 0, min_count: int = 5) -> pd.Series:
+    """Count, mean and std. dev. by index level."""
+    agg = series.groupby(level=index_level).agg(['count', 'mean', 'std'])
+    agg = agg.loc[agg['count'] > min_count]
+    return agg.mean()
```

### Comparing `pimms-learn-0.2.0/vaep/io/__init__.py` & `pimms_learn-0.3.0/vaep/io/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,174 +1,210 @@
-from collections import namedtuple
-import logging
-from typing import List, Tuple, Union
-import json
-from pathlib import Path, PurePath, PurePosixPath
-
-import numpy as np
-import pandas as pd
-
-import vaep.pandas
-
-PathsList = namedtuple('PathsList', ['files', 'folder'])
-
-
-logger = logging.getLogger(__name__)
-logger.info(f"Calling from {__name__}")
-
-
-def search_files(path='.', query='.txt'):
-    """Uses Pathlib to find relative to path files
-    with the query text in their file names. Returns
-    the path relative to the specified path.
-
-    Parameters
-    ----------
-    path : str, optional
-        Path to search, by default '.'
-    query : str, optional
-        query string for for filenames, by default '.txt'
-
-    Returns
-    -------
-    list
-        list with files as string containig query key.
-    """
-    path = Path(path)
-    files = []
-    for p in path.rglob("*"):
-        if query in p.name:
-            files.append(str(p.relative_to(path)))
-    return PathsList(files=files, folder=path)
-
-
-def search_subfolders(path='.', depth: int = 1, exclude_root: bool = False):
-    """Search subfolders relative to given path."""
-    if not isinstance(depth, int) and depth > 0:
-        raise ValueError(
-            f"Please provide an strictly positive integer, not {depth}")
-    EXCLUDED = ["*ipynb_checkpoints*"]
-
-    path = Path(path)
-    directories = [path]
-
-    def get_subfolders(path):
-        return [x for x in path.iterdir()
-                if x.is_dir() and
-                not any(x.match(excl) for excl in EXCLUDED)
-                ]
-
-    directories_previous = directories.copy()
-    while depth > 0:
-        directories_new = list()
-        for p in directories_previous:
-            directories_new.extend(
-                get_subfolders(p))
-        directories.extend(directories_new)
-        directories_previous = directories_new.copy()
-        depth -= 1
-
-    if exclude_root:
-        directories.pop(0)
-    return directories
-
-
-def resolve_path(path: Union[str, Path], to: Union[str, Path] = '.') -> Path:
-    """Resolve a path partly overlapping with to another path."""
-    pwd = Path(to).absolute()
-    pwd = [p for p in pwd.parts]
-    ret = [p for p in Path(path).parts if p not in pwd]
-    return Path('/'.join(ret))
-
-
-def get_fname_from_keys(keys, folder=Path('.'), file_ext='.pkl', remove_duplicates=True):
-    if remove_duplicates:
-        # https://stackoverflow.com/a/53657523/9684872
-        keys = list(dict.fromkeys(keys))
-    folder = Path(folder)
-    folder.mkdir(exist_ok=True, parents=True)
-    fname_dataset = folder / '{}{}'.format(vaep.pandas.replace_with(
-        ' '.join(keys), replace='- ', replace_with='_'), file_ext)
-    return fname_dataset
-
-
-def dump_to_csv(df: pd.DataFrame,
-                folder: Path,
-                outfolder: Path,
-                parent_folder_fct=None
-                ) -> None:
-    fname = f"{folder.stem}.csv"
-    if parent_folder_fct is not None:
-        outfolder = outfolder / parent_folder_fct(folder)
-    outfolder.mkdir(exist_ok=True, parents=True)
-    fname = outfolder / fname
-    logger.info(f"Dump to file: {fname}")
-    df.to_csv(fname)
-    return fname
-
-
-def dump_json(data_dict: dict, filename: Union[str, Path]):
-    """Dump dictionary as JSON.
-
-    Parameters
-    ----------
-    data_dict : dict
-        Dictionary with valid JSON entries to dump.
-    filename : Union[str, Path]
-        Filepath to save dictionary as JSON.
-    """
-    with open(filename, 'w') as f:
-        json.dump(obj=data_dict, fp=f, indent=4)
-
-
-def load_json(fname: Union[str, Path]) -> dict:
-    """Load JSON from disc.
-
-    Parameters
-    ----------
-    fname : Union[str, Path]
-        Filepath to JSON on disk.
-
-    Returns
-    -------
-    dict
-        Loaded JSON file.
-    """
-    with open(Path(fname)) as f:
-        d = json.load(f)
-    return d
-
-
-def parse_dict(input_dict: dict,
-               types: List[Tuple] = [(PurePath, lambda p: str(PurePosixPath(p))),
-                                     (np.ndarray, lambda a: a.to_list())]):
-    """Transform a set of items (instances) to their string representation"""
-    d = dict()
-    for k, v in input_dict.items():
-        for (old_type, fct) in types:
-            if isinstance(v, old_type):
-                v = fct(v)
-        d[k] = v
-    return d
-
-
-def extend_name(fname: Union[str, Path], extend_by: str, ext: str = None) -> Path:
-    """Extend the name of a file.
-
-    Parameters
-    ----------
-    fname : Union[str, Path]
-        Filepath to file to rename.
-    extend_by : str
-        Extend file stem by string
-
-    Returns
-    -------
-    Path
-        Changed filepath with extension
-    """
-    fname = Path(fname)
-    if ext is None:
-        ext = fname.suffix
-    fname = fname.parent / f"{fname.stem}{extend_by}"
-    fname = fname.with_suffix(ext)
-    return fname
+import json
+import logging
+import pickle
+from collections import namedtuple
+from pathlib import Path, PurePath, PurePosixPath
+from typing import Tuple, Union
+
+import numpy as np
+import pandas as pd
+
+import vaep.pandas
+
+PathsList = namedtuple('PathsList', ['files', 'folder'])
+
+
+logger = logging.getLogger(__name__)
+logger.info(f"Calling from {__name__}")
+
+
+def search_files(path='.', query='.txt'):
+    """Uses Pathlib to find relative to path files
+    with the query text in their file names. Returns
+    the path relative to the specified path.
+
+    Parameters
+    ----------
+    path : str, optional
+        Path to search, by default '.'
+    query : str, optional
+        query string for for filenames, by default '.txt'
+
+    Returns
+    -------
+    list
+        list with files as string containig query key.
+    """
+    path = Path(path)
+    files = []
+    for p in path.rglob("*"):
+        if query in p.name:
+            files.append(str(p.relative_to(path)))
+    return PathsList(files=files, folder=path)
+
+
+def search_subfolders(path='.', depth: int = 1, exclude_root: bool = False):
+    """Search subfolders relative to given path."""
+    if not isinstance(depth, int) and depth > 0:
+        raise ValueError(
+            f"Please provide an strictly positive integer, not {depth}")
+    EXCLUDED = ["*ipynb_checkpoints*"]
+
+    path = Path(path)
+    directories = [path]
+
+    def get_subfolders(path):
+        return [x for x in path.iterdir()
+                if x.is_dir() and not any(x.match(excl) for excl in EXCLUDED)
+                ]
+
+    directories_previous = directories.copy()
+    while depth > 0:
+        directories_new = list()
+        for p in directories_previous:
+            directories_new.extend(
+                get_subfolders(p))
+        directories.extend(directories_new)
+        directories_previous = directories_new.copy()
+        depth -= 1
+
+    if exclude_root:
+        directories.pop(0)
+    return directories
+
+
+def resolve_path(path: Union[str, Path], to: Union[str, Path] = '.') -> Path:
+    """Resolve a path partly overlapping with to another path."""
+    pwd = Path(to).absolute()
+    pwd = [p for p in pwd.parts]
+    ret = [p for p in Path(path).parts if p not in pwd]
+    return Path('/'.join(ret))
+
+
+def get_fname_from_keys(keys, folder='.', file_ext='.pkl', remove_duplicates=True):
+    if remove_duplicates:
+        # https://stackoverflow.com/a/53657523/9684872
+        keys = list(dict.fromkeys(keys))
+    folder = Path(folder)
+    folder.mkdir(exist_ok=True, parents=True)
+    fname_dataset = folder / '{}{}'.format(vaep.pandas.replace_with(
+        ' '.join(keys), replace='- ', replace_with='_'), file_ext)
+    return fname_dataset
+
+
+def dump_to_csv(df: pd.DataFrame,
+                folder: Path,
+                outfolder: Path,
+                parent_folder_fct=None
+                ) -> None:
+    fname = f"{folder.stem}.csv"
+    if parent_folder_fct is not None:
+        outfolder = outfolder / parent_folder_fct(folder)
+    outfolder.mkdir(exist_ok=True, parents=True)
+    fname = outfolder / fname
+    logger.info(f"Dump to file: {fname}")
+    df.to_csv(fname)
+    return fname
+
+
+def dump_json(data_dict: dict, filename: Union[str, Path]):
+    """Dump dictionary as JSON.
+
+    Parameters
+    ----------
+    data_dict : dict
+        Dictionary with valid JSON entries to dump.
+    filename : Union[str, Path]
+        Filepath to save dictionary as JSON.
+    """
+    with open(filename, 'w') as f:
+        json.dump(obj=data_dict, fp=f, indent=4)
+
+
+def to_pickle(obj, fname):
+    with open(fname, 'wb') as f:
+        pickle.dump(obj, f)
+
+
+def from_pickle(fname):
+    with open(fname, 'rb') as f:
+        return pickle.load(f)
+
+
+def load_json(fname: Union[str, Path]) -> dict:
+    """Load JSON from disc.
+
+    Parameters
+    ----------
+    fname : Union[str, Path]
+        Filepath to JSON on disk.
+
+    Returns
+    -------
+    dict
+        Loaded JSON file.
+    """
+    with open(Path(fname)) as f:
+        d = json.load(f)
+    return d
+
+
+def parse_dict(input_dict: dict,
+               types: Tuple[Tuple] = ((PurePath, lambda p: str(PurePosixPath(p))),
+                                      (np.ndarray, lambda a: a.to_list()))):
+    """Transform a set of items (instances) to their string representation"""
+    d = dict()
+    for k, v in input_dict.items():
+        for (old_type, fct) in types:
+            if isinstance(v, old_type):
+                v = fct(v)
+        d[k] = v
+    return d
+
+
+def extend_name(fname: Union[str, Path], extend_by: str, ext: str = None) -> Path:
+    """Extend the name of a file.
+
+    Parameters
+    ----------
+    fname : Union[str, Path]
+        Filepath to file to rename.
+    extend_by : str
+        Extend file stem by string
+
+    Returns
+    -------
+    Path
+        Changed filepath with extension
+    """
+    fname = Path(fname)
+    if ext is None:
+        ext = fname.suffix
+    fname = fname.parent / f"{fname.stem}{extend_by}"
+    fname = fname.with_suffix(ext)
+    return fname
+
+
+def add_indices(array: np.array, original_df: pd.DataFrame,
+                index_only: bool = False) -> pd.DataFrame:
+    """Add indices to array using provided origional DataFrame.
+
+    Parameters
+    ----------
+    array : np.array
+        Array of data to add indices to.
+    original_df : pd.DataFrame
+        Original DataFrame data was generated from.
+    index_only : bool, optional
+        Only add row index, by default False
+
+    Returns
+    -------
+    pd.DataFrame
+        DataFrame with array data and original indices.
+    """
+
+    index = original_df.index
+    columns = None
+    if not index_only:
+        columns = original_df.columns
+    return pd.DataFrame(array, index=index, columns=columns)
```

### Comparing `pimms-learn-0.2.0/vaep/io/dataloaders.py` & `pimms_learn-0.3.0/vaep/io/dataloaders.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,150 +1,156 @@
-import pandas
-import torch
-from typing import Tuple
-
-from torch.utils.data import Dataset
-# from fastai.data.load import DataLoader
-# from fastai.data.core import DataLoaders
-from fastai.data.all import *
-
-from vaep.io import datasets
-from vaep.io.datasets import DatasetWithTarget
-from vaep.transform import VaepPipeline
-
-
-class DataLoadersCreator():
-    """DataLoader creator. For training or evaluation."""
-
-    def __init__(self,
-                 df_train: pandas.DataFrame,
-                 df_valid: pandas.DataFrame,
-                 scaler,
-                 DataSetClass: torch.utils.data.Dataset,
-                 batch_size: int
-                 ):
-        """Helper function to create from pandas.DataFrame(s) in memory datasets.
-
-        Parameters
-        ----------
-        df_train : pandas.DataFrame
-            Training data samples in DataFrames.
-        df_valid : pandas.DataFrame
-            Validation data (for training) in DataFrames.
-        scaler : [type]
-            A pipeline of transform to apply to the dataset.
-        DataSetClass : torch.utils.data.Dataset
-            Type of dataset to use for generating single samples based on
-            DataFrames.
-        batch_size : int
-            Batch size to use.
-
-        Returns
-        -------
-        Tuple[torch.utils.data.Dataloader, torch.utils.data.Dataloader]
-            train and validation set dataloaders.
-        """
-        self.data_train = DataSetClass(
-            data=scaler.transform(df_train))
-        self.data_valid = DataSetClass(data=scaler.transform(df_valid))
-        self.scaler = scaler
-        self.batch_size = batch_size
-
-    def get_dls(self,
-                shuffle_train: bool = True,
-                **kwargs) -> Tuple[torch.utils.data.DataLoader,
-                                   torch.utils.data.DataLoader]:
-        self.shuffle_train = shuffle_train
-        dl_train = DataLoader(
-            dataset=self.data_train,
-            batch_size=self.batch_size, shuffle=shuffle_train, **kwargs)
-
-        dl_valid = DataLoader(
-            dataset=self.data_valid,
-            batch_size=self.batch_size, shuffle=False, **kwargs)
-        return dl_train, dl_valid
-
-    def __repr__(self):
-        return f"{self.__class__.__name__} for creating dataloaders with {self.batch_size}."
-
-
-def get_dls(train_X: pandas.DataFrame,
-            valid_X: pandas.DataFrame,
-            transformer: VaepPipeline,
-            bs: int = 64,
-            num_workers=0) -> DataLoaders:
-    """Create training and validation dataloaders
-
-    Parameters
-    ----------
-    train_X : pandas.DataFrame
-        Training Data, index is ignored for data fetching
-    valid_X : pandas.DataFrame
-        Validation data, won't be shuffled.
-    transformer : VaepPipeline
-        Pipeline with separate encode and decode
-    dataset : torch.utils.data.Dataset, optional
-        torch Dataset to yield encoded samples, by default DatasetWithTarget
-    bs : int, optional
-        batch size, by default 64
-
-    Returns
-    -------
-    fastai.data.core.DataLoaders
-        FastAI DataLoaders with train and valid Dataloder
-
-    Example
-    -------
-    import sklearn
-    from sklearn.impute import SimpleImputer
-    from sklearn.preprocessing import StandardScaler
-
-    from vaep.dataloader import get_dls
-    from vaep.transform import VaepPipeline
-
-    dae_default_pipeline = sklearn.pipeline.Pipeline(
-        [('normalize', StandardScaler()),
-         ('impute', SimpleImputer(add_indicator=False))
-         ])
-    # train_X, val_X = None, None # pandas.DataFrames
-    transforms = VaepPipeline(df_train=train_X,
-                                  encode=dae_default_pipeline,
-                                  decode=['normalize'])
-    dls = get_dls(train_X, val_X, transforms, bs=4)
-    """
-    train_ds = datasets.DatasetWithTarget(df=train_X,
-                                          transformer=transformer)
-    valid_ds = datasets.DatasetWithTargetSpecifyTarget(df=train_X,
-                                                       targets=valid_X,
-                                                       transformer=transformer)
-    # ! Need for script exection (as plain python file)
-    # https://pytorch.org/docs/stable/notes/windows.html#multiprocessing-error-without-if-clause-protection
-    return DataLoaders.from_dsets(train_ds, valid_ds, bs=bs, drop_last=False,
-                                  num_workers=num_workers)
-
-
-# dls.test_dl
-# needs to be part of setup procedure of a class
-def get_test_dl(df: pandas.DataFrame,
-                transformer: VaepPipeline,
-                dataset: Dataset = DatasetWithTarget,
-                bs: int = 64):
-    """[summary]
-
-    Parameters
-    ----------
-    df : pandas.DataFrame
-        Test data in a DataFrame
-    transformer : vaep.transform.VaepPipeline
-        Pipeline with separate encode and decode
-    dataset : torch.utils.data.Dataset, optional
-        torch Dataset to yield encoded samples, by default DatasetWithTarget
-    bs : int, optional
-        batch size, by default 64
-
-    Returns
-    -------
-    fastai.data.load.DataLoader
-        DataLoader from fastai for test data.
-    """
-    ds = dataset(df, transformer)
-    return DataLoader(ds, bs=bs, shuffle=False)
+import pandas
+import torch
+from typing import Tuple
+
+from torch.utils.data import Dataset
+from fastai.data.load import DataLoader
+from fastai.data.core import DataLoaders
+from fastai.data.all import *
+
+from vaep.io import datasets
+from vaep.io.datasets import DatasetWithTarget
+from vaep.transform import VaepPipeline
+
+import pandas as pd
+
+
+class DataLoadersCreator():
+    """DataLoader creator. For training or evaluation."""
+
+    def __init__(self,
+                 df_train: pandas.DataFrame,
+                 df_valid: pandas.DataFrame,
+                 scaler,
+                 DataSetClass: torch.utils.data.Dataset,
+                 batch_size: int
+                 ):
+        """Helper function to create from pandas.DataFrame(s) in memory datasets.
+
+        Parameters
+        ----------
+        df_train : pandas.DataFrame
+            Training data samples in DataFrames.
+        df_valid : pandas.DataFrame
+            Validation data (for training) in DataFrames.
+        scaler : [type]
+            A pipeline of transform to apply to the dataset.
+        DataSetClass : torch.utils.data.Dataset
+            Type of dataset to use for generating single samples based on
+            DataFrames.
+        batch_size : int
+            Batch size to use.
+
+        Returns
+        -------
+        Tuple[torch.utils.data.Dataloader, torch.utils.data.Dataloader]
+            train and validation set dataloaders.
+        """
+        self.data_train = DataSetClass(
+            data=scaler.transform(df_train))
+        self.data_valid = DataSetClass(data=scaler.transform(df_valid))
+        self.scaler = scaler
+        self.batch_size = batch_size
+
+    def get_dls(self,
+                shuffle_train: bool = True,
+                **kwargs) -> Tuple[torch.utils.data.DataLoader,
+                                   torch.utils.data.DataLoader]:
+        self.shuffle_train = shuffle_train
+        dl_train = DataLoader(
+            dataset=self.data_train,
+            batch_size=self.batch_size, shuffle=shuffle_train, **kwargs)
+
+        dl_valid = DataLoader(
+            dataset=self.data_valid,
+            batch_size=self.batch_size, shuffle=False, **kwargs)
+        return dl_train, dl_valid
+
+    def __repr__(self):
+        return f"{self.__class__.__name__} for creating dataloaders with {self.batch_size}."
+
+
+def get_dls(train_X: pandas.DataFrame,
+            valid_X: pandas.DataFrame,
+            transformer: VaepPipeline,
+            bs: int = 64,
+            num_workers=0) -> DataLoaders:
+    """Create training and validation dataloaders
+
+    Parameters
+    ----------
+    train_X : pandas.DataFrame
+        Training Data, index is ignored for data fetching
+    valid_X : pandas.DataFrame
+        Validation data, won't be shuffled.
+    transformer : VaepPipeline
+        Pipeline with separate encode and decode
+    bs : int, optional
+        batch size, by default 64
+    num_workers : int, optional
+        number of workers to use for data loading, by default 0
+
+    Returns
+    -------
+    fastai.data.core.DataLoaders
+        FastAI DataLoaders with train and valid Dataloder
+
+    Example
+    -------
+    import sklearn
+    from sklearn.impute import SimpleImputer
+    from sklearn.preprocessing import StandardScaler
+
+    from vaep.dataloader import get_dls
+    from vaep.transform import VaepPipeline
+
+    dae_default_pipeline = sklearn.pipeline.Pipeline(
+        [('normalize', StandardScaler()),
+         ('impute', SimpleImputer(add_indicator=False))
+         ])
+    # train_X, val_X = None, None # pandas.DataFrames
+    transforms = VaepPipeline(df_train=train_X,
+                                  encode=dae_default_pipeline,
+                                  decode=['normalize'])
+    dls = get_dls(train_X, val_X, transforms, bs=4)
+    """
+    train_ds = datasets.DatasetWithTarget(df=train_X,
+                                          transformer=transformer)
+    if valid_X is not None:
+        valid_ds = datasets.DatasetWithTargetSpecifyTarget(df=train_X,
+                                                           targets=valid_X,
+                                                           transformer=transformer)
+    else:
+        # empty dataset will be ignored by fastai in training loops
+        valid_ds = datasets.DatasetWithTarget(df=pd.DataFrame())
+    # ! Need for script exection (as plain python file)
+    # https://pytorch.org/docs/stable/notes/windows.html#multiprocessing-error-without-if-clause-protection
+    return DataLoaders.from_dsets(train_ds, valid_ds, bs=bs, drop_last=False,
+                                  num_workers=num_workers)
+
+
+# dls.test_dl
+# needs to be part of setup procedure of a class
+def get_test_dl(df: pandas.DataFrame,
+                transformer: VaepPipeline,
+                dataset: Dataset = DatasetWithTarget,
+                bs: int = 64):
+    """[summary]
+
+    Parameters
+    ----------
+    df : pandas.DataFrame
+        Test data in a DataFrame
+    transformer : vaep.transform.VaepPipeline
+        Pipeline with separate encode and decode
+    dataset : torch.utils.data.Dataset, optional
+        torch Dataset to yield encoded samples, by default DatasetWithTarget
+    bs : int, optional
+        batch size, by default 64
+
+    Returns
+    -------
+    fastai.data.load.DataLoader
+        DataLoader from fastai for test data.
+    """
+    ds = dataset(df, transformer)
+    return DataLoader(ds, bs=bs, shuffle=False)
```

### Comparing `pimms-learn-0.2.0/vaep/io/datasplits.py` & `pimms_learn-0.3.0/vaep/io/datasplits.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,208 +1,208 @@
-from __future__ import annotations
-from dataclasses import dataclass, field
-import logging
-from functools import partial
-from pathlib import Path
-from typing import Protocol
-
-import pandas as pd
-from pandas.core.algorithms import isin
-
-from vaep.pandas import interpolate
-from vaep.io.format import classname, class_full_module
-
-logger = logging.getLogger(__name__)
-
-FILE_FORMAT_TO_DUMP_FCT = {'pkl': ('to_pickle', 'read_pickle'),
-                           # 'pickle': 'to_pickle',
-                           'csv': ('to_csv', 'read_csv')}
-
-
-def long_format(df: pd.DataFrame,
-                colname_values: str = 'intensity',
-                # index_name: str = 'Sample ID'
-                ) -> pd.DataFrame:
-    # ToDo: Docstring as in class when finalized
-    names = df.columns.names
-    if None in names:
-        raise ValueError(f"Column names must not be None: {names}")
-    df_long = df.stack(names).to_frame(colname_values)
-    return df_long
-
-
-to_long_format = partial(
-    long_format, colname_values="intensity"  # , index_name="Sample ID"
-)
-
-
-def wide_format(df: pd.DataFrame,
-                columns: str = 'Sample ID',
-                name_values: str = 'intensity') -> pd.DataFrame:
-    # ToDo: Docstring as in class when finalized
-    df_wide = df.pivot(columns=columns, values=name_values)
-    df_wide = df_wide.T
-    return df_wide
-
-
-@dataclass
-class DataSplits():
-    is_wide_format: bool = field(init=True, repr=False)
-    train_X: pd.DataFrame = None
-    val_y: pd.DataFrame = None
-    test_y: pd.DataFrame = None
-
-    def __post_init__(self):
-        self._items = sorted(self.__dict__)
-        self._is_wide = self.is_wide_format
-        self._items.remove('is_wide_format')
-
-    def __getitem__(self, index):
-        return (self._items[index], getattr(self, self._items[index]))
-
-    def __dir__(self):
-        # return self._items
-        return ['dump', 'from_folder', 'interpolate', 'load', 'test_X', 'test_y',
-                'to_long_format', 'to_wide_format', 'train_X', 'val_X', 'val_y']
-
-    def dump(self, folder='data', file_format='csv') -> dict:
-        """dump in long format."""
-        folder = Path(folder)
-        folder.mkdir(parents=True, exist_ok=True)
-
-        if file_format not in FILE_FORMAT_TO_DUMP_FCT:
-            raise ValueError(f"Select one of these formats: {', '.join(FILE_FORMAT_TO_DUMP_FCT.keys())}")
-        dumps = {}
-        n_dumped = 0
-        for (_attr, _df) in self:
-            if _df is None:
-                logger.info(f"Missing attribute: {_attr}")
-                continue
-
-            _dim = _df.shape
-            if len(_dim) == 1:
-                logger.info(f"'{_attr}' has shape: {_df.shape}")
-            elif len(_dim) == 2:
-                logger.info(f"'{_attr}' had old shape: {_df.shape}")
-                _df = to_long_format(_df)
-                logger.info(f"'{_attr}' has new shape: {_df.shape}")
-            else:
-                raise ValueError()
-            fname = folder / f"{_attr}.{file_format}"
-            dumps[fname.name] = fname.as_posix()
-            logger.info(f"save '{_attr}' to file: {fname}")
-            dump_fct = getattr(_df, FILE_FORMAT_TO_DUMP_FCT[file_format][0])
-            dump_fct(fname)
-            n_dumped += 1
-        if not n_dumped:
-            raise ValueError(f'Nothing to dump, all None: {self}')
-            # _df.to_json(fname) # does not work easily for series
-        return dumps
-
-    def load(self, folder: str, use_wide_format=False, file_format='csv') -> None:
-        """Load data in place from folder"""
-        items = dict(self.__annotations__)
-        del items['is_wide_format']
-        args = load_items(folder=folder, items=items, use_wide_format=use_wide_format, file_format=file_format)
-        for _attr, _df in args.items():
-            setattr(self, _attr, _df)
-        self._is_wide = use_wide_format
-        return None  # could also be self
-
-    @classmethod
-    def from_folder(cls, folder: str, use_wide_format=False, file_format='csv') -> DataSplits:
-        """Build DataSplits instance from folder."""
-        items = dict(cls.__annotations__)
-        del items['is_wide_format']
-        args = load_items(folder=folder, items=items, use_wide_format=use_wide_format, file_format=file_format)
-        _data_splits = cls(**args, is_wide_format=use_wide_format)
-        _data_splits._is_wide = use_wide_format
-        return _data_splits
-
-    def to_wide_format(self):
-        if self._is_wide:
-            return
-
-        for _attr, _series in self:
-            if _series is None:
-                continue
-            _df = _series.unstack()
-            setattr(self, _attr, _df)
-        self._is_wide = True
-
-    def to_long_format(self, name_values: str = 'intensity'):
-        if not self._is_wide:
-            return
-
-        for _attr, _df in self:
-            if _df is None:
-                continue
-            _series = _df.stack()
-            _series.name = name_values
-            setattr(self, _attr, _series)
-        self._is_wide = False
-
-    # singledispatch possible
-    def interpolate(self, dataset: Union[str, pd.DataFrame]):
-        if issubclass(type(dataset), pd.DataFrame):
-            ds = dataset
-        elif issubclass(type(dataset), pd.Series):
-            ds = dataset.unstack()
-        elif issubclass(type(dataset), str):
-            try:
-                ds = getattr(self, dataset)
-            except AttributeError:
-                raise AttributeError(f"Please provide a valid attribute, not '{dataset}'. "
-                                     "Valid attributes are {}".format(', '.join(x for x in self._items)))
-            if dataset[-1] in ['y', 'Y']:
-                logger.warning(
-                    f'Attempting to interpolate target: {dataset} '
-                    '(this might make sense, but a warning')
-            if ds is None:
-                raise ValueError(f'Attribute is None: {dataset!r}.')
-            if not self._is_wide:
-                ds = ds.unstack()  # series is unstack to DataFrame
-        else:
-            raise TypeError(f"Unknown type: {classname(dataset)}."
-                            f" None of str, {class_full_module(pd.DataFrame)}, {class_full_module(pd.Series)}"
-                            )
-
-        return interpolate(wide_df=ds)
-
-
-def load_items(folder: str, items: dict, use_wide_format=False, file_format='csv') -> dict:
-    folder = Path(folder)
-    assert folder.exists(), f'Could not find folder: {folder}'
-    args = {}
-    for _attr, _cls in items.items():
-        # assert issubclass(_cls, (pd.DataFrame, pd.Series)) # now strings, see
-        # https://docs.python.org/3/whatsnew/3.7.html#pep-563-postponed-evaluation-of-annotations
-        fname = folder / f"{_attr}.{file_format}"
-        if not fname.exists():
-            raise FileNotFoundError(f"Missing file requested for attr '{_attr}', missing {fname}")
-        read_fct = getattr(pd, FILE_FORMAT_TO_DUMP_FCT[file_format][1])
-        _df = read_fct(fname)
-        # logic below is suited for csv reader -> maybe split up loading and saving later?
-        if len(_df.shape) == 1:
-            _df = _df.to_frame().reset_index()  # in case Series was pickled
-        cols = list(_df.columns)
-        if use_wide_format:
-            _df = wide_format(_df.set_index(cols[1:-1]), columns=cols[0], name_values=cols[-1])
-        else:
-            _df.set_index(cols[:-1], inplace=True)
-        logger.info(f"Loaded '{_attr}' from file: {fname}")
-        args[_attr] = _df.squeeze()
-    return args
-
-
-# set default file name -> intergrate into DataSplits?
-def load_freq(folder: str, file='freq_features.pkl'):
-    folder = Path(folder)
-    fname = folder / file
-    if fname.suffix == '.json':
-        freq_per_feature = pd.read_json(fname, orient='index').squeeze()
-        freq_per_feature.name = 'freq'
-    elif fname.suffix == '.pkl':
-        freq_per_feature = pd.read_pickle(fname)
-    else:
-        raise ValueError(f"Unknown Fileextension: {fname.suffix}")
-    return freq_per_feature
+from __future__ import annotations
+
+import logging
+from dataclasses import dataclass, field
+from functools import partial
+from pathlib import Path
+from typing import Union
+
+import pandas as pd
+
+from vaep.io.format import class_full_module, classname
+from vaep.pandas import interpolate
+
+logger = logging.getLogger(__name__)
+
+FILE_FORMAT_TO_DUMP_FCT = {'pkl': ('to_pickle', 'read_pickle'),
+                           # 'pickle': 'to_pickle',
+                           'csv': ('to_csv', 'read_csv')}
+
+
+def long_format(df: pd.DataFrame,
+                colname_values: str = 'intensity',
+                # index_name: str = 'Sample ID'
+                ) -> pd.DataFrame:
+    # ToDo: Docstring as in class when finalized
+    names = df.columns.names
+    if None in names:
+        raise ValueError(f"Column names must not be None: {names}")
+    df_long = df.stack(names).to_frame(colname_values)
+    return df_long
+
+
+to_long_format = partial(
+    long_format, colname_values="intensity"  # , index_name="Sample ID"
+)
+
+
+def wide_format(df: pd.DataFrame,
+                columns: str = 'Sample ID',
+                name_values: str = 'intensity') -> pd.DataFrame:
+    # ToDo: Docstring as in class when finalized
+    df_wide = df.pivot(columns=columns, values=name_values)
+    df_wide = df_wide.T
+    return df_wide
+
+
+@dataclass
+class DataSplits():
+    is_wide_format: bool = field(init=True, repr=False)
+    train_X: pd.DataFrame = None
+    val_y: pd.DataFrame = None
+    test_y: pd.DataFrame = None
+
+    def __post_init__(self):
+        self._items = sorted(self.__dict__)
+        self._is_wide = self.is_wide_format
+        self._items.remove('is_wide_format')
+
+    def __getitem__(self, index):
+        return (self._items[index], getattr(self, self._items[index]))
+
+    def __dir__(self):
+        # return self._items
+        return ['dump', 'from_folder', 'interpolate', 'load', 'test_X', 'test_y',
+                'to_long_format', 'to_wide_format', 'train_X', 'val_X', 'val_y']
+
+    def dump(self, folder='data', file_format='csv') -> dict:
+        """dump in long format."""
+        folder = Path(folder)
+        folder.mkdir(parents=True, exist_ok=True)
+
+        if file_format not in FILE_FORMAT_TO_DUMP_FCT:
+            raise ValueError(f"Select one of these formats: {', '.join(FILE_FORMAT_TO_DUMP_FCT.keys())}")
+        dumps = {}
+        n_dumped = 0
+        for (_attr, _df) in self:
+            if _df is None:
+                logger.info(f"Missing attribute: {_attr}")
+                continue
+
+            _dim = _df.shape
+            if len(_dim) == 1:
+                logger.info(f"'{_attr}' has shape: {_df.shape}")
+            elif len(_dim) == 2:
+                logger.info(f"'{_attr}' had old shape: {_df.shape}")
+                _df = to_long_format(_df)
+                logger.info(f"'{_attr}' has new shape: {_df.shape}")
+            else:
+                raise ValueError()
+            fname = folder / f"{_attr}.{file_format}"
+            dumps[fname.name] = fname.as_posix()
+            logger.info(f"save '{_attr}' to file: {fname}")
+            dump_fct = getattr(_df, FILE_FORMAT_TO_DUMP_FCT[file_format][0])
+            dump_fct(fname)
+            n_dumped += 1
+        if not n_dumped:
+            raise ValueError(f'Nothing to dump, all None: {self}')
+            # _df.to_json(fname) # does not work easily for series
+        return dumps
+
+    def load(self, folder: str, use_wide_format=False, file_format='csv') -> None:
+        """Load data in place from folder"""
+        items = dict(self.__annotations__)
+        del items['is_wide_format']
+        args = load_items(folder=folder, items=items, use_wide_format=use_wide_format, file_format=file_format)
+        for _attr, _df in args.items():
+            setattr(self, _attr, _df)
+        self._is_wide = use_wide_format
+        return None  # could also be self
+
+    @classmethod
+    def from_folder(cls, folder: str, use_wide_format=False, file_format='csv') -> DataSplits:
+        """Build DataSplits instance from folder."""
+        items = dict(cls.__annotations__)
+        del items['is_wide_format']
+        args = load_items(folder=folder, items=items, use_wide_format=use_wide_format, file_format=file_format)
+        _data_splits = cls(**args, is_wide_format=use_wide_format)
+        _data_splits._is_wide = use_wide_format
+        return _data_splits
+
+    def to_wide_format(self):
+        if self._is_wide:
+            return
+
+        for _attr, _series in self:
+            if _series is None:
+                continue
+            _df = _series.unstack()
+            setattr(self, _attr, _df)
+        self._is_wide = True
+
+    def to_long_format(self, name_values: str = 'intensity'):
+        if not self._is_wide:
+            return
+
+        for _attr, _df in self:
+            if _df is None:
+                continue
+            _series = _df.stack()
+            _series.name = name_values
+            setattr(self, _attr, _series)
+        self._is_wide = False
+
+    # singledispatch possible
+    def interpolate(self, dataset: Union[str, pd.DataFrame]):
+        if issubclass(type(dataset), pd.DataFrame):
+            ds = dataset
+        elif issubclass(type(dataset), pd.Series):
+            ds = dataset.unstack()
+        elif issubclass(type(dataset), str):
+            try:
+                ds = getattr(self, dataset)
+            except AttributeError:
+                raise AttributeError(f"Please provide a valid attribute, not '{dataset}'. "
+                                     "Valid attributes are {}".format(', '.join(x for x in self._items)))
+            if dataset[-1] in ['y', 'Y']:
+                logger.warning(
+                    f'Attempting to interpolate target: {dataset} '
+                    '(this might make sense, but a warning')
+            if ds is None:
+                raise ValueError(f'Attribute is None: {dataset!r}.')
+            if not self._is_wide:
+                ds = ds.unstack()  # series is unstack to DataFrame
+        else:
+            raise TypeError(f"Unknown type: {classname(dataset)}."
+                            f" None of str, {class_full_module(pd.DataFrame)}, {class_full_module(pd.Series)}"
+                            )
+
+        return interpolate(wide_df=ds)
+
+
+def load_items(folder: str, items: dict, use_wide_format=False, file_format='csv') -> dict:
+    folder = Path(folder)
+    assert folder.exists(), f'Could not find folder: {folder}'
+    args = {}
+    for _attr, _cls in items.items():
+        # assert issubclass(_cls, (pd.DataFrame, pd.Series)) # now strings, see
+        # https://docs.python.org/3/whatsnew/3.7.html#pep-563-postponed-evaluation-of-annotations
+        fname = folder / f"{_attr}.{file_format}"
+        if not fname.exists():
+            raise FileNotFoundError(f"Missing file requested for attr '{_attr}', missing {fname}")
+        read_fct = getattr(pd, FILE_FORMAT_TO_DUMP_FCT[file_format][1])
+        _df = read_fct(fname)
+        # logic below is suited for csv reader -> maybe split up loading and saving later?
+        if len(_df.shape) == 1:
+            _df = _df.to_frame().reset_index()  # in case Series was pickled
+        cols = list(_df.columns)
+        if use_wide_format:
+            _df = wide_format(_df.set_index(cols[1:-1]), columns=cols[0], name_values=cols[-1])
+        else:
+            _df.set_index(cols[:-1], inplace=True)
+        logger.info(f"Loaded '{_attr}' from file: {fname}")
+        args[_attr] = _df.squeeze()
+    return args
+
+
+# set default file name -> intergrate into DataSplits?
+def load_freq(folder: str, file='freq_features.pkl'):
+    folder = Path(folder)
+    fname = folder / file
+    if fname.suffix == '.json':
+        freq_per_feature = pd.read_json(fname, orient='index').squeeze()
+        freq_per_feature.name = 'freq'
+    elif fname.suffix == '.pkl':
+        freq_per_feature = pd.read_pickle(fname)
+    else:
+        raise ValueError(f"Unknown Fileextension: {fname.suffix}")
+    return freq_per_feature
```

### Comparing `pimms-learn-0.2.0/vaep/io/types.py` & `pimms_learn-0.3.0/vaep/io/types.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-"""
-papermill strategy to determine type
-see: https://github.com/nteract/papermill/blob/76906a882bb5b3e719ad113c7b2447e0ddffb2c7/papermill/cli.py#L275-L307
-"""
-
-
-def resolve_type(value):
-    if value == "True":
-        return True
-    elif value == "False":
-        return False
-    elif value == "None":
-        return None
-    elif _is_int(value):
-        return int(value)
-    elif _is_float(value):
-        return float(value)
-    else:
-        return value
-
-
-def _is_int(value):
-    """Use casting to check if value can convert to an `int`."""
-    try:
-        int(value)
-    except ValueError:
-        return False
-    else:
-        return True
-
-
-def _is_float(value):
-    """Use casting to check if value can convert to a `float`."""
-    try:
-        float(value)
-    except ValueError:
-        return False
-    else:
-        return True
+"""
+papermill strategy to determine type
+see: https://github.com/nteract/papermill/blob/76906a882bb5b3e719ad113c7b2447e0ddffb2c7/papermill/cli.py#L275-L307
+"""
+
+
+def resolve_type(value):
+    if value == "True":
+        return True
+    elif value == "False":
+        return False
+    elif value == "None":
+        return None
+    elif _is_int(value):
+        return int(value)
+    elif _is_float(value):
+        return float(value)
+    else:
+        return value
+
+
+def _is_int(value):
+    """Use casting to check if value can convert to an `int`."""
+    try:
+        int(value)
+    except ValueError:
+        return False
+    else:
+        return True
+
+
+def _is_float(value):
+    """Use casting to check if value can convert to a `float`."""
+    try:
+        float(value)
+    except ValueError:
+        return False
+    else:
+        return True
```

### Comparing `pimms-learn-0.2.0/vaep/logging.py` & `pimms_learn-0.3.0/vaep/logging.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-"""Custom logging setup for notebooks."""
-from pathlib import Path
-from datetime import datetime
-import logging
-import sys
-
-LOG_FOLDER = Path('logs')
-LOG_FOLDER.mkdir(exist_ok=True)
-
-
-def setup_nb_logger(level: int = logging.INFO,
-                    format_str: str = '%(name)s - %(levelname)-8s %(message)s') -> None:
-    logging.basicConfig(level=level, format=format_str)
-    root_logger = logging.getLogger()
-    root_logger.setLevel(level)  # in case root_logger existed already before calling basicConfig
-    c_format = logging.Formatter(format_str)
-    if root_logger.handlers:
-        handler = root_logger.handlers[0]
-    else:
-        handler = logging.StreamHandler(sys.stdout)
-    handler.setFormatter(c_format)
-    return root_logger
-
-
-def setup_logger_w_file(logger, level=logging.INFO, fname_base=None):
-    """Setup logging in project. Takes a logger an creates
-
-    Parameters
-    ----------
-    logger : logging.Logger
-        logger instance to configre
-    level : int, optional
-        logging level, by default logging.INFO
-    fname_base : str, optional
-        filename for logging, by default None
-
-    Returns
-    -------
-    logging.Logger
-        Configured logger instance for logging
-
-    Examples
-    --------
-    >>> import logging
-    >>> logger = logging.getLogger('vaep')
-    >>> _ = setup_logger_w_file(logger) # no logging to file
-    >>> logger.handlers = [] # reset logger
-    >>> _ = setup_logger_w_file() #
-
-    """
-    logger.setLevel(level)
-    logger.handlers = []  # remove any handler in case you reexecute the cell
-
-    c_format = logging.Formatter('%(name)s - %(levelname)-8s %(message)s')
-
-    c_handler = logging.StreamHandler(sys.stdout)
-    c_handler.setLevel(level)
-    c_handler.setFormatter(c_format)
-    logger.addHandler(c_handler)
-
-    if fname_base:
-        date_log_file = "{:%y%m%d_%H%M}".format(datetime.now())
-        f_handler = logging.FileHandler(
-            LOG_FOLDER / f"{fname_base}_{date_log_file}.txt")
-        f_handler.setLevel(level)
-        f_handler.setFormatter(c_format)
-        logger.addHandler(f_handler)
-
-    return logger
-
-
-setup_logger = setup_logger_w_file
+"""Custom logging setup for notebooks."""
+from pathlib import Path
+from datetime import datetime
+import logging
+import sys
+
+LOG_FOLDER = Path('logs')
+LOG_FOLDER.mkdir(exist_ok=True)
+
+
+def setup_nb_logger(level: int = logging.INFO,
+                    format_str: str = '%(name)s - %(levelname)-8s %(message)s') -> None:
+    logging.basicConfig(level=level, format=format_str)
+    root_logger = logging.getLogger()
+    root_logger.setLevel(level)  # in case root_logger existed already before calling basicConfig
+    c_format = logging.Formatter(format_str)
+    if root_logger.handlers:
+        handler = root_logger.handlers[0]
+    else:
+        handler = logging.StreamHandler(sys.stdout)
+    handler.setFormatter(c_format)
+    return root_logger
+
+
+def setup_logger_w_file(logger, level=logging.INFO, fname_base=None):
+    """Setup logging in project. Takes a logger an creates
+
+    Parameters
+    ----------
+    logger : logging.Logger
+        logger instance to configre
+    level : int, optional
+        logging level, by default logging.INFO
+    fname_base : str, optional
+        filename for logging, by default None
+
+    Returns
+    -------
+    logging.Logger
+        Configured logger instance for logging
+
+    Examples
+    --------
+    >>> import logging
+    >>> logger = logging.getLogger('vaep')
+    >>> _ = setup_logger_w_file(logger) # no logging to file
+    >>> logger.handlers = [] # reset logger
+    >>> _ = setup_logger_w_file() #
+
+    """
+    logger.setLevel(level)
+    logger.handlers = []  # remove any handler in case you reexecute the cell
+
+    c_format = logging.Formatter('%(name)s - %(levelname)-8s %(message)s')
+
+    c_handler = logging.StreamHandler(sys.stdout)
+    c_handler.setLevel(level)
+    c_handler.setFormatter(c_format)
+    logger.addHandler(c_handler)
+
+    if fname_base:
+        date_log_file = "{:%y%m%d_%H%M}".format(datetime.now())
+        f_handler = logging.FileHandler(
+            LOG_FOLDER / f"{fname_base}_{date_log_file}.txt")
+        f_handler.setLevel(level)
+        f_handler.setFormatter(c_format)
+        logger.addHandler(f_handler)
+
+    return logger
+
+
+setup_logger = setup_logger_w_file
```

### Comparing `pimms-learn-0.2.0/vaep/models/__init__.py` & `pimms_learn-0.3.0/vaep/models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,319 +1,324 @@
-from functools import reduce
-import logging
-from operator import mul
-from pathlib import Path
-import pickle
-import pprint
-from typing import Tuple, List, Callable, Union
-import json
-
-import matplotlib.pyplot as plt
-import numpy as np
-import pandas as pd
-import torch
-from fastcore.foundation import L
-from fastai import learner
-import sklearn.metrics as sklm
-
-from . import ae
-from . import analysis
-from . import collab
-from . import vae
-
-import vaep
-
-logger = logging.getLogger(__name__)
-
-
-def plot_loss(recorder: learner.Recorder,
-              norm_train: np.int64 = np.int64(1),
-              norm_val: np.int64 = np.int64(1),
-              skip_start: int = 5,
-              with_valid: bool = True,
-              ax: plt.Axes = None) -> plt.Axes:
-    """Adapted Recorder.plot_loss to accept matplotlib.axes.Axes argument.
-    Allows to build combined graphics.
-
-    Parameters
-    ----------
-    recorder : learner.Recorder
-        fastai Recorder object, learn.recorder
-    norm_train: np.int64, optional
-        Normalize epoch loss by number of training samples, by default 1
-    norm_val: np.int64, optional
-        Normalize epoch loss by number of validation samples, by default 1
-    skip_start : int, optional
-        Skip N first batch metrics, by default 5
-    with_valid : bool, optional
-        Add validation data loss, by default True
-    ax : plt.Axes, optional
-        Axes to plot on, by default None
-
-    Returns
-    -------
-    plt.Axes
-        [description]
-    """
-    if not ax:
-        fig, ax = plt.subplots()
-    ax.plot(list(range(skip_start, len(recorder.losses))),
-            recorder.losses[skip_start:] / norm_train, label='train')
-    if with_valid:
-        idx = (np.array(recorder.iters) < skip_start).sum()
-        ax.plot(recorder.iters[idx:], L(
-            recorder.values[idx:]).itemgot(1) / norm_val, label='valid')
-        ax.legend()
-    return ax
-
-
-def plot_training_losses(learner: learner.Learner,
-                         name: str,
-                         ax=None,
-                         save_recorder: bool = True,
-                         norm_factors=np.array([1, 1], dtype='int'),
-                         folder='figures',
-                         figsize=(15, 8)):
-    if ax is None:
-        fig, ax = plt.subplots(figsize=figsize)
-    else:
-        fig = ax.get_figure()
-    ax.set_title(f'{name} loss')
-    norm_train, norm_val = norm_factors  # exactly two
-    learner.recorder.plot_loss(skip_start=5, ax=ax,
-                               norm_train=norm_train, norm_val=norm_val)
-    name = name.lower()
-    _ = RecorderDump(learner.recorder, name).save(folder)
-    vaep.savefig(fig, name=f'{name}_training',
-                 folder=folder)
-    return fig
-
-
-def calc_net_weight_count(model: torch.nn.modules.module.Module) -> int:
-    model.train()
-    model_params = filter(lambda p: p.requires_grad, model.parameters())
-    weight_count = 0
-    for param in model_params:
-        weight_count += np.prod(param.size())
-    return int(weight_count)
-
-
-class RecorderDump:
-    """Simple Class to hold fastai Recorder Callback data for serialization using pickle.
-    """
-    filename_tmp = 'recorder_{}.pkl'
-
-    def __init__(self, recorder, name):
-        self.losses = recorder.losses
-        self.values = recorder.values
-        self.iters = recorder.iters
-        self.name = name
-
-    def save(self, folder=Path('.')):
-        with open(Path(folder) / self.filename_tmp.format(self.name), 'wb') as f:
-            pickle.dump(self, f)
-
-    @classmethod
-    def load(cls, filepath, name):
-        with open(Path(filepath) / cls.filename_tmp.format(name), 'rb') as f:
-            ret = pickle.load(f)
-        return ret
-
-    plot_loss = plot_loss
-
-
-def split_prediction_by_mask(pred: pd.DataFrame,
-                             mask: pd.DataFrame,
-                             check_keeps_all: bool = False) -> Tuple[pd.DataFrame, pd.DataFrame]:
-    """[summary]
-
-    Parameters
-    ----------
-    pred : pd.DataFrame
-        prediction DataFrame
-    mask : pd.DataFrame
-        Mask with same indices as pred DataFrame.
-    check_keeps_all : bool, optional
-        if True, perform sanity checks, by default False
-
-    Returns
-    -------
-    Tuple[pd.DataFrame, pd.DataFrame]
-        prediction for inversed mask, and predicitions for mask
-    """
-    test_pred_observed = pred[~mask].stack()
-    test_pred_real_na = pred[mask].stack()
-    if check_keeps_all:
-        assert len(test_pred_real_na) + \
-            len(test_pred_observed) == reduce(mul, pred.shape)
-    return test_pred_observed, test_pred_real_na
-
-
-def compare_indices(first_index: pd.Index, second_index: pd.Index) -> pd.Index:
-    """Show difference of indices in other index wrt. to first. First should be the larger
-    collection wrt to the second. This is the set difference of two Index objects.
-
-    If second index is a superset of indices of the first, the set will be empty,
-    although there  are differences (default behaviour in pandas).
-
-    Parameters
-    ----------
-    first_index : pd.Index
-        Index, should be superset
-    second_index : pd.Index
-        Index, should be the subset
-
-    Returns
-    -------
-    pd.Index
-        Return a new Index with elements of the first index not in second.
-    """
-    _diff_index = first_index.difference(second_index)
-    if len(_diff_index):
-        print("Some predictions couldn't be generated using the approach using artifical replicates.\n"
-              "These will be omitted for evaluation.")
-        for _index in _diff_index:
-            print(f"{_index[0]:<40}\t {_index[1]:<40}")
-    return _diff_index
-
-
-scoring = [('MSE', sklm.mean_squared_error),
-           ('MAE', sklm.mean_absolute_error)]
-
-
-def collect_metrics(metrics_jsons: List, key_fct: Callable) -> dict:
-    """Collect and aggregate a bunch of json metrics.
-
-    Parameters
-    ----------
-    metrics_jsons : List
-        list of filepaths to json metric files
-    key_fct : Callable
-        Callable which creates key function of a single filepath
-
-    Returns
-    -------
-    dict
-        Aggregated metrics dictionary with outer key defined by key_fct
-
-    Raises
-    ------
-    AssertionError:
-        If key should be overwritten, but value would change.
-    """
-    all_metrics = {}
-    for fname in metrics_jsons:
-        fname = Path(fname)
-        logger.info(f"Load file: {fname = }")
-
-        key = key_fct(fname)  # level, repeat
-
-        logger.debug(f"{key = }")
-        with open(fname) as f:
-            loaded = json.load(f)
-        loaded = vaep.pandas.flatten_dict_of_dicts(loaded)
-
-        if key not in all_metrics:
-            all_metrics[key] = loaded
-            continue
-        for k, v in loaded.items():
-            if k in all_metrics[key]:
-                logger.debug(f"Found existing key: {k = } ")
-                assert all_metrics[key][k] == v, "Diverging values for {k}: {v1} vs {v2}".format(
-                    k=k,
-                    v1=all_metrics[key][k],
-                    v2=v)
-            else:
-                all_metrics[key][k] = v
-    return all_metrics
-
-
-def calculte_metrics(pred_df: pd.DataFrame,
-                     true_col: List[str] = None,
-                     scoring: List[Tuple[str, Callable]] = scoring) -> dict:
-    """Create metrics based on predictions, a truth reference and a
-    list of scoring function with a name.
-
-    Parameters
-    ----------
-    pred_df : pd.DataFrame
-        Prediction DataFrame containing `true_col`.
-    true_col : List[str], optional
-        Column of ground truth values, by default None
-    scoring : List[Tuple[str, Callable]], optional
-        List of tuples. A tuple is a set of (key, funtion) pairs.
-        The function take y_true and y_pred - as for all sklearn metrics, by default scoring
-
-    Returns
-    -------
-    pd.DataFrame
-        [description]
-
-    Raises
-    ------
-    ValueError
-        [description]
-    """
-    if not true_col:
-        # assume first column is truth if None is given
-        y_true = pred_df.iloc[:, 0]
-        print(f'Selected as truth to compare to: {y_true.name}')
-        y_pred = pred_df.iloc[:, 1:]
-    else:
-        if issubclass(type(true_col), int):
-            y_true = pred_df.iloc[:, true_col]
-            y_pred = pred_df.drop(y_true.name, axis=1)
-        elif issubclass(type(true_col), str):
-            y_true = pred_df[true_col]
-            y_pred = pred_df.drop(true_col, axis=1)
-        else:
-            raise ValueError(
-                f'true_col has to be of type str or int, not {type(true_col)}')
-    if y_true.isna().any():
-        raise ValueError(f"Ground truth column '{y_true.name}' contains missing values. "
-                         "Drop these rows first.")
-
-    metrics = {}
-    for model_key in y_pred:
-        model_pred = y_pred[model_key]
-        model_pred_no_na = model_pred.dropna()
-        if len(model_pred) > len(model_pred_no_na):
-            logger.info(
-                f"Drop indices for {model_key}: "
-                "{}".format([(idx[0], idx[1])
-                             for idx
-                             in model_pred.index.difference(model_pred_no_na.index)]))
-
-        metrics[model_key] = dict(
-            [(k, float(f(y_true=y_true.loc[model_pred_no_na.index],
-                         y_pred=model_pred_no_na)))
-             for k, f in scoring]
-        )
-        metrics[model_key]['N'] = int(len(model_pred_no_na))
-        metrics[model_key]['prop'] = len(model_pred_no_na) / len(model_pred)
-    return metrics
-
-
-class Metrics():
-
-    def __init__(self):
-        self.metrics = {}
-
-    def add_metrics(self, pred, key):
-        self.metrics[key] = calculte_metrics(pred_df=pred.dropna())
-        return self.metrics[key]
-
-    def __repr__(self):
-        return pprint.pformat(self.metrics, indent=2, compact=True)
-
-
-def get_df_from_nested_dict(nested_dict,
-                            column_levels=['data_split', 'model', 'metric_name'],
-                            row_name='subset'):
-    metrics = {}
-    for k, run_metrics in nested_dict.items():
-        metrics[k] = vaep.pandas.flatten_dict_of_dicts(run_metrics)
-
-    metrics = pd.DataFrame.from_dict(metrics, orient='index')
-    metrics.columns.names = column_levels
-    metrics.index.name = row_name
-    return metrics
+import json
+import logging
+import pickle
+import pprint
+from functools import reduce
+from operator import mul
+from pathlib import Path
+from typing import Callable, List, Tuple
+
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
+import sklearn.metrics as sklm
+import torch
+from fastai import learner
+from fastcore.foundation import L
+
+import vaep
+
+from . import ae, analysis, collab, vae
+
+logger = logging.getLogger(__name__)
+
+NUMPY_ONE = np.int64(1)
+
+
+
+def plot_loss(recorder: learner.Recorder,
+              norm_train: np.int64 = NUMPY_ONE,
+              norm_val: np.int64 = NUMPY_ONE,
+              skip_start: int = 5,
+              with_valid: bool = True,
+              ax: plt.Axes = None) -> plt.Axes:
+    """Adapted Recorder.plot_loss to accept matplotlib.axes.Axes argument.
+    Allows to build combined graphics.
+
+    Parameters
+    ----------
+    recorder : learner.Recorder
+        fastai Recorder object, learn.recorder
+    norm_train: np.int64, optional
+        Normalize epoch loss by number of training samples, by default 1
+    norm_val: np.int64, optional
+        Normalize epoch loss by number of validation samples, by default 1
+    skip_start : int, optional
+        Skip N first batch metrics, by default 5
+    with_valid : bool, optional
+        Add validation data loss, by default True
+    ax : plt.Axes, optional
+        Axes to plot on, by default None
+
+    Returns
+    -------
+    plt.Axes
+        [description]
+    """
+    if not ax:
+        _, ax = plt.subplots()
+    ax.plot(list(range(skip_start, len(recorder.losses))),
+            recorder.losses[skip_start:] / norm_train, label='train')
+    if with_valid:
+        idx = (np.array(recorder.iters) < skip_start).sum()
+        ax.plot(recorder.iters[idx:], L(
+            recorder.values[idx:]).itemgot(1) / norm_val, label='valid')
+        ax.legend()
+    return ax
+
+
+NORM_ONES = np.array([1, 1], dtype='int')
+
+
+def plot_training_losses(learner: learner.Learner,
+                         name: str,
+                         ax=None,
+                         norm_factors=NORM_ONES,
+                         folder='figures',
+                         figsize=(15, 8)):
+    if ax is None:
+        fig, ax = plt.subplots(figsize=figsize)
+    else:
+        fig = ax.get_figure()
+    ax.set_title(f'{name} loss')
+    norm_train, norm_val = norm_factors  # exactly two
+    with_valid = True
+    if norm_val is None:
+        with_valid = False
+    learner.recorder.plot_loss(skip_start=5, ax=ax, with_valid=with_valid,
+                               norm_train=norm_train, norm_val=norm_val)
+    name = name.lower()
+    _ = RecorderDump(learner.recorder, name).save(folder)
+    vaep.savefig(fig, name=f'{name}_training',
+                 folder=folder)
+    return fig
+
+
+def calc_net_weight_count(model: torch.nn.modules.module.Module) -> int:
+    model.train()
+    model_params = filter(lambda p: p.requires_grad, model.parameters())
+    weight_count = 0
+    for param in model_params:
+        weight_count += np.prod(param.size())
+    return int(weight_count)
+
+
+class RecorderDump:
+    """Simple Class to hold fastai Recorder Callback data for serialization using pickle.
+    """
+    filename_tmp = 'recorder_{}.pkl'
+
+    def __init__(self, recorder, name):
+        self.losses = recorder.losses
+        self.values = recorder.values
+        self.iters = recorder.iters
+        self.name = name
+
+    def save(self, folder='.'):
+        with open(Path(folder) / self.filename_tmp.format(self.name), 'wb') as f:
+            pickle.dump(self, f)
+
+    @classmethod
+    def load(cls, filepath, name):
+        with open(Path(filepath) / cls.filename_tmp.format(name), 'rb') as f:
+            ret = pickle.load(f)
+        return ret
+
+    plot_loss = plot_loss
+
+
+def split_prediction_by_mask(pred: pd.DataFrame,
+                             mask: pd.DataFrame,
+                             check_keeps_all: bool = False) -> Tuple[pd.DataFrame, pd.DataFrame]:
+    """[summary]
+
+    Parameters
+    ----------
+    pred : pd.DataFrame
+        prediction DataFrame
+    mask : pd.DataFrame
+        Mask with same indices as pred DataFrame.
+    check_keeps_all : bool, optional
+        if True, perform sanity checks, by default False
+
+    Returns
+    -------
+    Tuple[pd.DataFrame, pd.DataFrame]
+        prediction for inversed mask, and predicitions for mask
+    """
+    test_pred_observed = pred[~mask].stack()
+    test_pred_real_na = pred[mask].stack()
+    if check_keeps_all:
+        assert len(test_pred_real_na) + \
+            len(test_pred_observed) == reduce(mul, pred.shape)
+    return test_pred_observed, test_pred_real_na
+
+
+def compare_indices(first_index: pd.Index, second_index: pd.Index) -> pd.Index:
+    """Show difference of indices in other index wrt. to first. First should be the larger
+    collection wrt to the second. This is the set difference of two Index objects.
+
+    If second index is a superset of indices of the first, the set will be empty,
+    although there  are differences (default behaviour in pandas).
+
+    Parameters
+    ----------
+    first_index : pd.Index
+        Index, should be superset
+    second_index : pd.Index
+        Index, should be the subset
+
+    Returns
+    -------
+    pd.Index
+        Return a new Index with elements of the first index not in second.
+    """
+    _diff_index = first_index.difference(second_index)
+    if len(_diff_index):
+        print("Some predictions couldn't be generated using the approach using artifical replicates.\n"
+              "These will be omitted for evaluation.")
+        for _index in _diff_index:
+            print(f"{_index[0]:<40}\t {_index[1]:<40}")
+    return _diff_index
+
+
+scoring = [('MSE', sklm.mean_squared_error),
+           ('MAE', sklm.mean_absolute_error)]
+
+
+def collect_metrics(metrics_jsons: List, key_fct: Callable) -> dict:
+    """Collect and aggregate a bunch of json metrics.
+
+    Parameters
+    ----------
+    metrics_jsons : List
+        list of filepaths to json metric files
+    key_fct : Callable
+        Callable which creates key function of a single filepath
+
+    Returns
+    -------
+    dict
+        Aggregated metrics dictionary with outer key defined by key_fct
+
+    Raises
+    ------
+    AssertionError:
+        If key should be overwritten, but value would change.
+    """
+    all_metrics = {}
+    for fname in metrics_jsons:
+        fname = Path(fname)
+        logger.info(f"Load file: {fname = }")
+
+        key = key_fct(fname)  # level, repeat
+
+        logger.debug(f"{key = }")
+        with open(fname) as f:
+            loaded = json.load(f)
+        loaded = vaep.pandas.flatten_dict_of_dicts(loaded)
+
+        if key not in all_metrics:
+            all_metrics[key] = loaded
+            continue
+        for k, v in loaded.items():
+            if k in all_metrics[key]:
+                logger.debug(f"Found existing key: {k = } ")
+                assert all_metrics[key][k] == v, "Diverging values for {k}: {v1} vs {v2}".format(
+                    k=k,
+                    v1=all_metrics[key][k],
+                    v2=v)
+            else:
+                all_metrics[key][k] = v
+    return all_metrics
+
+
+def calculte_metrics(pred_df: pd.DataFrame,
+                     true_col: List[str] = None,
+                     scoring: List[Tuple[str, Callable]] = scoring) -> dict:
+    """Create metrics based on predictions, a truth reference and a
+    list of scoring function with a name.
+
+    Parameters
+    ----------
+    pred_df : pd.DataFrame
+        Prediction DataFrame containing `true_col`.
+    true_col : List[str], optional
+        Column of ground truth values, by default None
+    scoring : List[Tuple[str, Callable]], optional
+        List of tuples. A tuple is a set of (key, funtion) pairs.
+        The function take y_true and y_pred - as for all sklearn metrics, by default scoring
+
+    Returns
+    -------
+    pd.DataFrame
+        [description]
+
+    Raises
+    ------
+    ValueError
+        [description]
+    """
+    if not true_col:
+        # assume first column is truth if None is given
+        y_true = pred_df.iloc[:, 0]
+        print(f'Selected as truth to compare to: {y_true.name}')
+        y_pred = pred_df.iloc[:, 1:]
+    else:
+        if issubclass(type(true_col), int):
+            y_true = pred_df.iloc[:, true_col]
+            y_pred = pred_df.drop(y_true.name, axis=1)
+        elif issubclass(type(true_col), str):
+            y_true = pred_df[true_col]
+            y_pred = pred_df.drop(true_col, axis=1)
+        else:
+            raise ValueError(
+                f'true_col has to be of type str or int, not {type(true_col)}')
+    if y_true.isna().any():
+        raise ValueError(f"Ground truth column '{y_true.name}' contains missing values. "
+                         "Drop these rows first.")
+
+    metrics = {}
+    for model_key in y_pred:
+        model_pred = y_pred[model_key]
+        model_pred_no_na = model_pred.dropna()
+        if len(model_pred) > len(model_pred_no_na):
+            logger.info(
+                f"Drop indices for {model_key}: "
+                "{}".format([(idx[0], idx[1])
+                             for idx
+                             in model_pred.index.difference(model_pred_no_na.index)]))
+
+        metrics[model_key] = dict(
+            [(k, float(f(y_true=y_true.loc[model_pred_no_na.index],
+                         y_pred=model_pred_no_na)))
+             for k, f in scoring]
+        )
+        metrics[model_key]['N'] = int(len(model_pred_no_na))
+        metrics[model_key]['prop'] = len(model_pred_no_na) / len(model_pred)
+    return metrics
+
+
+class Metrics():
+
+    def __init__(self):
+        self.metrics = {}
+
+    def add_metrics(self, pred, key):
+        self.metrics[key] = calculte_metrics(pred_df=pred.dropna())
+        return self.metrics[key]
+
+    def __repr__(self):
+        return pprint.pformat(self.metrics, indent=2, compact=True)
+
+
+def get_df_from_nested_dict(nested_dict,
+                            column_levels=('data_split', 'model', 'metric_name'),
+                            row_name='subset'):
+    metrics = {}
+    for k, run_metrics in nested_dict.items():
+        metrics[k] = vaep.pandas.flatten_dict_of_dicts(run_metrics)
+
+    metrics = pd.DataFrame.from_dict(metrics, orient='index')
+    metrics.columns.names = column_levels
+    metrics.index.name = row_name
+    return metrics
```

### Comparing `pimms-learn-0.2.0/vaep/models/collect_dumps.py` & `pimms_learn-0.3.0/vaep/models/collect_dumps.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,59 @@
-from functools import partial, update_wrapper
-import logging
-from pathlib import Path
-import json
-import yaml
-from typing import Iterable, Callable
-import vaep.pandas
-
-logger = logging.getLogger(__name__)
-
-
-def select_content(s: str, first_split):
-    s = s.split(first_split)[1]
-    assert isinstance(s, str), f"More than one split: {s}"
-    entries = s.split('_')
-    if len(entries) > 1:
-        s = '_'.join(entries[:-1])
-    return s
-
-
-def load_config_file(fname: Path, first_split='config_') -> dict:
-    with open(fname) as f:
-        loaded = yaml.safe_load(f)
-    key = f"{fname.parent.name}_{select_content(fname.stem, first_split=first_split)}"
-    return key, loaded
-
-
-def load_metric_file(fname: Path, first_split='metrics_') -> dict:
-    with open(fname) as f:
-        loaded = json.load(f)
-    loaded = vaep.pandas.flatten_dict_of_dicts(loaded)
-    key = f"{fname.parent.name}_{select_content(fname.stem, first_split=first_split)}"
-    return key, loaded
-
-
-def collect(paths: Iterable,
-            load_fn: Callable[[Path], dict],
-            ) -> dict:
-    all_metrics = []
-    for fname in paths:
-        fname = Path(fname)
-        key, loaded = load_fn(fname)
-        logger.debug(f"{key = }")
-        if 'id' not in loaded:
-            loaded['id'] = key
-        all_metrics.append(loaded)
-    return all_metrics
-
-
-collect_metrics = partial(collect,
-                          load_fn=load_metric_file,
-                          )
-collect_metrics = update_wrapper(collect_metrics, collect)
-
-collect_configs = partial(collect,
-                          load_fn=load_config_file,
-                          )
-collect_configs = update_wrapper(collect_configs, collect)
+""" Collects metrics and config files from the experiment directory structure."""
+from functools import partial, update_wrapper
+import logging
+from pathlib import Path
+import json
+import yaml
+from typing import Iterable, Callable
+import vaep.pandas
+
+logger = logging.getLogger(__name__)
+
+
+def select_content(s: str, first_split):
+    s = s.split(first_split)[1]
+    assert isinstance(s, str), f"More than one split: {s}"
+    entries = s.split('_')
+    if len(entries) > 1:
+        s = '_'.join(entries[:-1])
+    return s
+
+
+def load_config_file(fname: Path, first_split='config_') -> dict:
+    with open(fname) as f:
+        loaded = yaml.safe_load(f)
+    key = f"{fname.parent.name}_{select_content(fname.stem, first_split=first_split)}"
+    return key, loaded
+
+
+def load_metric_file(fname: Path, first_split='metrics_') -> dict:
+    with open(fname) as f:
+        loaded = json.load(f)
+    loaded = vaep.pandas.flatten_dict_of_dicts(loaded)
+    key = f"{fname.parent.name}_{select_content(fname.stem, first_split=first_split)}"
+    return key, loaded
+
+
+def collect(paths: Iterable,
+            load_fn: Callable[[Path], dict],
+            ) -> dict:
+    all_metrics = []
+    for fname in paths:
+        fname = Path(fname)
+        key, loaded = load_fn(fname)
+        logger.debug(f"{key = }")
+        if 'id' not in loaded:
+            loaded['id'] = key
+        all_metrics.append(loaded)
+    return all_metrics
+
+
+collect_metrics = partial(collect,
+                          load_fn=load_metric_file,
+                          )
+collect_metrics = update_wrapper(collect_metrics, collect)
+
+collect_configs = partial(collect,
+                          load_fn=load_config_file,
+                          )
+collect_configs = update_wrapper(collect_configs, collect)
```

### Comparing `pimms-learn-0.2.0/vaep/nb.py` & `pimms_learn-0.3.0/vaep/nb.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-from pathlib import Path
-from pprint import pformat
-import yaml
-
-import vaep.io
-
-import logging
-logger = logging.getLogger()
-
-
-class Config():
-    """Config class with a setter enforcing that config entries cannot
-    be overwritten.
-
-
-    Can contain configs, which are itself configs:
-    keys, paths,
-
-    """
-
-    def __setattr__(self, entry, value):
-        """Set if attribute not in instance."""
-        if hasattr(self, entry) and getattr(self, entry) != value:
-            raise AttributeError(
-                f'{entry} already set to {getattr(self, entry)}')
-        super().__setattr__(entry, value)
-
-    def __repr__(self):
-        return pformat(vars(self))  # does not work in Jupyter?
-
-    def overwrite_entry(self, entry, value):
-        """Explicitly overwrite a given value."""
-        super().__setattr__(entry, value)
-
-    def dump(self, fname=None):
-        if fname is None:
-            try:
-                fname = self.out_folder
-                fname = Path(fname) / 'model_config.yml'
-            except AttributeError:
-                raise AttributeError(
-                    'Specify fname or set "out_folder" attribute.')
-        d = vaep.io.parse_dict(input_dict=self.__dict__)
-        with open(fname, 'w') as f:
-            yaml.dump(d, f)
-        logger.info(f"Dumped config to: {fname}")
-
-    @classmethod
-    def from_dict(cls, d: dict):
-        cfg = cls()
-        for k, v in d.items():
-            setattr(cfg, k, v)
-        return cfg
-
-    def update_from_dict(self, params: dict):
-        for k, v in params.items():
-            try:
-                setattr(self, k, v)
-            except AttributeError:
-                logger.info(f"Already set attribute: {k} has value {v}")
-
-    def keys(self):
-        return vars(self).keys()
-
-    def items(self):
-        return vars(self).items()
-
-    def values(self):
-        return vars(self).values()
-
-
-def get_params(args: dict.keys, globals, remove=True) -> dict:
-    params = {k: v for k, v in globals.items() if k not in args and k[0] != '_'}
-    if not remove:
-        return params
-    remove_keys_from_globals(params.keys(), globals=globals)
-    return params
-
-
-def remove_keys_from_globals(keys: dict.keys, globals: dict):
-    for k in keys:
-        try:
-            del globals[k]
-            logger.info(f"Removed from global namespace: {k}")
-        except KeyError:
-            logger.warning(f"Key not found in globals(): {k}")
-
-
-def add_default_paths(cfg: Config, folder_data='', out_root=None):
-    """Add default paths to config."""
-    if out_root:
-        cfg.out_folder = Path(out_root)
-        cfg.out_folder.mkdir(exist_ok=True, parents=True)
-    else:
-        cfg.out_folder = cfg.folder_experiment
-    if folder_data:
-        cfg.data = Path(folder_data)
-    else:
-        cfg.data = cfg.folder_experiment / 'data'
-        cfg.data.mkdir(exist_ok=True, parents=True)
-    assert cfg.data.exists(), f"Directory not found: {cfg.data}"
-    del folder_data
-    cfg.out_figures = cfg.folder_experiment / 'figures'
-    cfg.out_figures.mkdir(exist_ok=True)
-    cfg.out_metrics = cfg.folder_experiment
-    cfg.out_metrics.mkdir(exist_ok=True)
-    cfg.out_models = cfg.folder_experiment
-    cfg.out_models.mkdir(exist_ok=True)
-    cfg.out_preds = cfg.folder_experiment / 'preds'
-    cfg.out_preds.mkdir(exist_ok=True)
-    return cfg
-
-
-def args_from_dict(args: dict) -> Config:
-    assert 'folder_experiment' in args, f'Specify "folder_experiment" in {args}.'
-    args['folder_experiment'] = Path(args['folder_experiment'])
-    args = Config().from_dict(args)
-    args.folder_experiment.mkdir(exist_ok=True, parents=True)
-    add_default_paths(args, folder_data=args.__dict__.get('folder_data', ''),
-                      out_root=args.__dict__.get('out_root', None))
-    return args
+from pathlib import Path
+from pprint import pformat
+import yaml
+
+import vaep.io
+
+import logging
+logger = logging.getLogger()
+
+
+class Config():
+    """Config class with a setter enforcing that config entries cannot
+    be overwritten.
+
+
+    Can contain configs, which are itself configs:
+    keys, paths,
+
+    """
+
+    def __setattr__(self, entry, value):
+        """Set if attribute not in instance."""
+        if hasattr(self, entry) and getattr(self, entry) != value:
+            raise AttributeError(
+                f'{entry} already set to {getattr(self, entry)}')
+        super().__setattr__(entry, value)
+
+    def __repr__(self):
+        return pformat(vars(self))  # does not work in Jupyter?
+
+    def overwrite_entry(self, entry, value):
+        """Explicitly overwrite a given value."""
+        super().__setattr__(entry, value)
+
+    def dump(self, fname=None):
+        if fname is None:
+            try:
+                fname = self.out_folder
+                fname = Path(fname) / 'model_config.yml'
+            except AttributeError:
+                raise AttributeError(
+                    'Specify fname or set "out_folder" attribute.')
+        d = vaep.io.parse_dict(input_dict=self.__dict__)
+        with open(fname, 'w') as f:
+            yaml.dump(d, f)
+        logger.info(f"Dumped config to: {fname}")
+
+    @classmethod
+    def from_dict(cls, d: dict):
+        cfg = cls()
+        for k, v in d.items():
+            setattr(cfg, k, v)
+        return cfg
+
+    def update_from_dict(self, params: dict):
+        for k, v in params.items():
+            try:
+                setattr(self, k, v)
+            except AttributeError:
+                logger.info(f"Already set attribute: {k} has value {v}")
+
+    def keys(self):
+        return vars(self).keys()
+
+    def items(self):
+        return vars(self).items()
+
+    def values(self):
+        return vars(self).values()
+
+
+def get_params(args: dict.keys, globals, remove=True) -> dict:
+    params = {k: v for k, v in globals.items() if k not in args and k[0] != '_'}
+    if not remove:
+        return params
+    remove_keys_from_globals(params.keys(), globals=globals)
+    return params
+
+
+def remove_keys_from_globals(keys: dict.keys, globals: dict):
+    for k in keys:
+        try:
+            del globals[k]
+            logger.info(f"Removed from global namespace: {k}")
+        except KeyError:
+            logger.warning(f"Key not found in globals(): {k}")
+
+
+def add_default_paths(cfg: Config, folder_data='', out_root=None):
+    """Add default paths to config."""
+    if out_root:
+        cfg.out_folder = Path(out_root)
+        cfg.out_folder.mkdir(exist_ok=True, parents=True)
+    else:
+        cfg.out_folder = cfg.folder_experiment
+    if folder_data:
+        cfg.data = Path(folder_data)
+    else:
+        cfg.data = cfg.folder_experiment / 'data'
+        cfg.data.mkdir(exist_ok=True, parents=True)
+    assert cfg.data.exists(), f"Directory not found: {cfg.data}"
+    del folder_data
+    cfg.out_figures = cfg.folder_experiment / 'figures'
+    cfg.out_figures.mkdir(exist_ok=True)
+    cfg.out_metrics = cfg.folder_experiment
+    cfg.out_metrics.mkdir(exist_ok=True)
+    cfg.out_models = cfg.folder_experiment
+    cfg.out_models.mkdir(exist_ok=True)
+    cfg.out_preds = cfg.folder_experiment / 'preds'
+    cfg.out_preds.mkdir(exist_ok=True)
+    return cfg
+
+
+def args_from_dict(args: dict) -> Config:
+    assert 'folder_experiment' in args, f'Specify "folder_experiment" in {args}.'
+    args['folder_experiment'] = Path(args['folder_experiment'])
+    args = Config().from_dict(args)
+    args.folder_experiment.mkdir(exist_ok=True, parents=True)
+    add_default_paths(args, folder_data=args.__dict__.get('folder_data', ''),
+                      out_root=args.__dict__.get('out_root', None))
+    return args
```

### Comparing `pimms-learn-0.2.0/vaep/pandas/__init__.py` & `pimms_learn-0.3.0/vaep/pandas/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,315 +1,301 @@
-import collections.abc
-from collections import namedtuple
-
-
-from types import SimpleNamespace
-
-from typing import Iterable
-
-import numpy as np
-import pandas as pd
-import omegaconf
-
-from .calc_errors import calc_errors_per_feat, get_absolute_error
-
-
-def combine_value_counts(X: pd.DataFrame, dropna=True) -> pd.DataFrame:
-    """Pass a selection of columns to combine it's value counts.
-
-    This performs no checks. Make sure the scale of the variables
-    you pass is comparable.
-
-    Parameters
-    ----------
-    X : pandas.DataFrame
-        A DataFrame of several columns with values in a similar range.
-    dropna : bool, optional
-        Exclude NA values from counting, by default True
-
-    Returns
-    -------
-    pandas.DataFrame
-        DataFrame of combined value counts.
-    """
-    """
-    """
-    _df = pd.DataFrame()
-    for col in X.columns:
-        _df = _df.join(X[col].value_counts(dropna=dropna), how='outer')
-    freq_targets = _df.sort_index()
-    return freq_targets
-
-
-def unique_cols(s: pd.Series) -> bool:
-    """Check all entries are equal in pandas.Series
-
-    Ref: https://stackoverflow.com/a/54405767/968487
-
-    Parameters
-    ----------
-    s : pandas.Series
-        Series to check uniqueness
-
-    Returns
-    -------
-    bool
-        Boolean on if all values are equal.
-    """
-    return (s.iloc[0] == s).all()
-
-
-def get_unique_non_unique_columns(df: pd.DataFrame) -> SimpleNamespace:
-    """Get back a namespace with an column.Index both
-    of the unique and non-unique columns.
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-
-    Returns
-    -------
-    types.SimpleNamespace
-        SimpleNamespace with `unique` and `non_unique` column names indices.
-    """
-
-    mask_unique_columns = df.apply(unique_cols)
-
-    columns = SimpleNamespace()
-    columns.unique = df.columns[mask_unique_columns]
-    columns.non_unique = df.columns[~mask_unique_columns]
-    return columns
-
-
-def prop_unique_index(df: pd.DataFrame) -> pd.DataFrame:
-    counts = df.index.value_counts()
-    prop = (counts > 1).sum() / len(counts)
-    return 1 - prop
-
-
-def replace_with(string_key: str, replace: str = "()/", replace_with: str = '') -> str:
-    for symbol in replace:
-        string_key = string_key.replace(symbol, replace_with)
-    return string_key
-
-
-def index_to_dict(index: pd.Index) -> dict:
-    cols = {replace_with(col.replace(' ', '_').replace(
-        '-', '_')): col for col in index}
-    return cols
-
-
-def get_columns_accessor(df: pd.DataFrame, all_lower_case=False) -> omegaconf.OmegaConf:
-    if isinstance(df.columns, pd.MultiIndex):
-        raise ValueError("MultiIndex not supported.")
-    cols = index_to_dict(df.columns)
-    if all_lower_case:
-        cols = {k.lower(): v for k, v in cols.items()}
-    return omegaconf.OmegaConf.create(cols)
-
-
-def get_columns_accessor_from_iterable(cols: Iterable[str],
-                                       all_lower_case=False) -> omegaconf.OmegaConf:
-    cols = index_to_dict(cols)
-    if all_lower_case:
-        cols = {k.lower(): v for k, v in cols.items()}
-    return omegaconf.OmegaConf.create(cols)
-
-
-def select_max_by(df: pd.DataFrame, grouping_columns: list, selection_column: str) -> pd.DataFrame:
-    df = df.sort_values(by=[*grouping_columns, selection_column], ascending=False)
-    df = df.drop_duplicates(subset=grouping_columns,
-                            keep='first')
-    return df
-
-
-def get_columns_namedtuple(df: pd.DataFrame) -> namedtuple:
-    """Create namedtuple instance of column names.
-    Spaces in column names are replaced with underscores in the look-up.
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        A pandas DataFrame
-
-    Returns
-    -------
-    namedtuple
-        NamedTuple instance with columns as attributes.
-    """
-    columns = df.columns.to_list()
-    column_keys = [x.replace(' ', '_') for x in columns]
-    ColumnsNamedTuple = namedtuple('Columns', column_keys)
-    return ColumnsNamedTuple(**{k: v for k, v in zip(column_keys, columns)})
-
-
-def highlight_min(s: pd.Series) -> list:
-    """Highlight the min in a Series yellow for using in pandas.DataFrame.style
-
-    Parameters
-    ----------
-    s : pd.Series
-        Pandas Series
-
-    Returns
-    -------
-    list
-        list of strings containing the background color for the values speciefied.
-        To be used as `pandas.DataFrame.style.apply(highlight_min)`
-    """
-    to_highlight = s == s.min()
-    return ['background-color: yellow' if v else '' for v in to_highlight]
-
-
-def _add_indices(array: np.array, original_df: pd.DataFrame,
-                 index_only: bool = False) -> pd.DataFrame:
-    index = original_df.index
-    columns = None
-    if not index_only:
-        columns = original_df.columns
-    return pd.DataFrame(array, index=index, columns=columns)
-
-
-def interpolate(wide_df: pd.DataFrame, name='interpolated') -> pd.DataFrame:
-    """Interpolate NA values with the values before and after.
-    Uses n=3 replicates.
-    First rows replicates are the two following.
-    Last rows replicates are the two preceding.
-
-    Parameters
-    ----------
-    wide_df : pd.DataFrame
-        rows are sample, columns are measurements
-    name : str, optional
-        name for measurement in columns, by default 'replicates'
-
-    Returns
-    -------
-    pd.DataFrame
-        pd.DataFrame in long-format
-    """
-    mask = wide_df.isna()
-    first_row = wide_df.iloc[0].copy()
-    last_row = wide_df.iloc[-1].copy()
-
-    m = first_row.isna()
-    first_row.loc[m] = wide_df.iloc[1:3, m.to_list()].mean()
-
-    m = last_row.isna()
-    last_row.loc[m] = wide_df.iloc[-3:-1, m.to_list()].mean()
-
-    ret = wide_df.interpolate(
-        method='linear', limit_direction='both', limit=1, axis=0)
-    ret.iloc[0] = first_row
-    ret.iloc[-1] = last_row
-
-    ret = ret[mask].stack().dropna().squeeze()  # does not work with MultiIndex columns
-    ret.rename(name, inplace=True)
-    return ret
-
-
-def flatten_dict_of_dicts(d: dict, parent_key: str = '') -> dict:
-    """Build tuples for nested dictionaries for use as `pandas.MultiIndex`.
-
-    Parameters
-    ----------
-    d : dict
-        Nested dictionary for which all keys are flattened to tuples.
-    parent_key : str, optional
-        Outer key (used for recursion), by default ''
-
-    Returns
-    -------
-    dict
-        Flattend dictionary with tuple keys: {(outer_key, ..., inner_key) : value}
-    """
-    # simplified and adapted from: https://stackoverflow.com/a/6027615/9684872
-    items = []
-    for k, v in d.items():
-        new_key = parent_key + (k,) if parent_key else (k,)
-        if isinstance(v, collections.abc.MutableMapping):
-            items.extend(flatten_dict_of_dicts(v, parent_key=new_key).items())
-        else:
-            items.append((new_key, v))
-    return dict(items)
-
-
-def key_map(d: dict) -> dict:
-    """Build a schema of dicts
-
-    Parameters
-    ----------
-    d : dict
-        dictionary of dictionaries
-
-    Returns
-    -------
-    dict
-        Key map of dictionaries
-    """
-    ret = {}
-    _keys = ()
-    for k, v in d.items():
-        if isinstance(v, dict):
-            ret[k] = key_map(v)
-        else:
-            _keys = (_keys) + (k, )
-    if _keys:
-        if ret:
-            print(
-                f"Dictionaries are not of the same length: {_keys = } and {ret = }")
-            for k in _keys:
-                ret[k] = None
-        else:
-            return _keys
-    return ret
-
-
-printable = '0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ '
-
-
-def parse_query_expression(s: str, printable: str = printable) -> str:
-    """Parse a query expression for pd.DataFrame.query to a file name.
-    Removes all characters not listed in printable."""
-    return ''.join(filter(lambda x: x in printable, s))
-
-
-def length(x):
-    """Len function which return 0 if object (probably np.nan) has no length.
-    Otherwise return length of list, pandas.Series, numpy.array, dict, etc."""
-    try:
-        return len(x)
-    except BaseException:
-        return 0
-
-
-def get_last_index_matching_proportion(df_counts: pd.DataFrame,
-                                       prop: float = 0.25,
-                                       prop_col: str = 'proportion') -> object:
-    """df_counts needs to be sorted by "prop_col" (descending).
-
-    Parameters
-    ----------
-    df_counts : pd.DataFrame
-        df counts with ascending values along proportion column.
-        Index should be unique.
-    prop : float, optional
-        cutoff, inclusive, by default 0.25
-    prop_col : str, optional
-        column name for proportion, by default 'proportion'
-
-    Returns
-    -------
-    object
-        Index value for cutoff
-    """
-    assert df_counts.index.is_unique
-    mask = df_counts[prop_col] >= prop
-    idx_cutoff = df_counts[prop_col].loc[mask].tail(1).index[0]
-    return idx_cutoff
-
-
-def get_lower_whiskers(df: pd.DataFrame, factor: float = 1.5) -> pd.Series:
-    ret = df.describe()
-    iqr = ret.loc['75%'] - ret.loc['25%']
-    ret = ret.loc['25%'] - iqr * factor
-    return ret
+import collections.abc
+from collections import namedtuple
+from types import SimpleNamespace
+from typing import Iterable, List, Optional
+
+import numpy as np
+import omegaconf
+import pandas as pd
+
+from .calc_errors import calc_errors_per_feat, get_absolute_error
+
+
+def unique_cols(s: pd.Series) -> bool:
+    """Check all entries are equal in pandas.Series
+
+    Ref: https://stackoverflow.com/a/54405767/968487
+
+    Parameters
+    ----------
+    s : pandas.Series
+        Series to check uniqueness
+
+    Returns
+    -------
+    bool
+        Boolean on if all values are equal.
+    """
+    return (s.iloc[0] == s).all()
+
+
+def get_unique_non_unique_columns(df: pd.DataFrame) -> SimpleNamespace:
+    """Get back a namespace with an column.Index both
+    of the unique and non-unique columns.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+
+    Returns
+    -------
+    types.SimpleNamespace
+        SimpleNamespace with `unique` and `non_unique` column names indices.
+    """
+
+    mask_unique_columns = df.apply(unique_cols)
+
+    columns = SimpleNamespace()
+    columns.unique = df.columns[mask_unique_columns]
+    columns.non_unique = df.columns[~mask_unique_columns]
+    return columns
+
+
+def prop_unique_index(df: pd.DataFrame) -> pd.DataFrame:
+    counts = df.index.value_counts()
+    prop = (counts > 1).sum() / len(counts)
+    return 1 - prop
+
+
+def replace_with(string_key: str, replace: str = "()/", replace_with: str = '') -> str:
+    for symbol in replace:
+        string_key = string_key.replace(symbol, replace_with)
+    return string_key
+
+
+def index_to_dict(index: pd.Index) -> dict:
+    cols = {replace_with(col.replace(' ', '_').replace(
+        '-', '_')): col for col in index}
+    return cols
+
+
+def get_columns_accessor(df: pd.DataFrame, all_lower_case=False) -> omegaconf.OmegaConf:
+    if isinstance(df.columns, pd.MultiIndex):
+        raise ValueError("MultiIndex not supported.")
+    cols = index_to_dict(df.columns)
+    if all_lower_case:
+        cols = {k.lower(): v for k, v in cols.items()}
+    return omegaconf.OmegaConf.create(cols)
+
+
+def get_columns_accessor_from_iterable(cols: Iterable[str],
+                                       all_lower_case=False) -> omegaconf.OmegaConf:
+    cols = index_to_dict(cols)
+    if all_lower_case:
+        cols = {k.lower(): v for k, v in cols.items()}
+    return omegaconf.OmegaConf.create(cols)
+
+
+def select_max_by(df: pd.DataFrame, grouping_columns: list, selection_column: str) -> pd.DataFrame:
+    df = df.sort_values(by=[*grouping_columns, selection_column], ascending=False)
+    df = df.drop_duplicates(subset=grouping_columns,
+                            keep='first')
+    return df
+
+
+def get_columns_namedtuple(df: pd.DataFrame) -> namedtuple:
+    """Create namedtuple instance of column names.
+    Spaces in column names are replaced with underscores in the look-up.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        A pandas DataFrame
+
+    Returns
+    -------
+    namedtuple
+        NamedTuple instance with columns as attributes.
+    """
+    columns = df.columns.to_list()
+    column_keys = [x.replace(' ', '_') for x in columns]
+    ColumnsNamedTuple = namedtuple('Columns', column_keys)
+    return ColumnsNamedTuple(**{k: v for k, v in zip(column_keys, columns)})
+
+
+def highlight_min(s: pd.Series) -> list:
+    """Highlight the min in a Series yellow for using in pandas.DataFrame.style
+
+    Parameters
+    ----------
+    s : pd.Series
+        Pandas Series
+
+    Returns
+    -------
+    list
+        list of strings containing the background color for the values speciefied.
+        To be used as `pandas.DataFrame.style.apply(highlight_min)`
+    """
+    to_highlight = s == s.min()
+    return ['background-color: yellow' if v else '' for v in to_highlight]
+
+
+def _add_indices(array: np.array, original_df: pd.DataFrame,
+                 index_only: bool = False) -> pd.DataFrame:
+    index = original_df.index
+    columns = None
+    if not index_only:
+        columns = original_df.columns
+    return pd.DataFrame(array, index=index, columns=columns)
+
+
+def interpolate(wide_df: pd.DataFrame, name='interpolated') -> pd.DataFrame:
+    """Interpolate NA values with the values before and after.
+    Uses n=3 replicates.
+    First rows replicates are the two following.
+    Last rows replicates are the two preceding.
+
+    Parameters
+    ----------
+    wide_df : pd.DataFrame
+        rows are sample, columns are measurements
+    name : str, optional
+        name for measurement in columns, by default 'replicates'
+
+    Returns
+    -------
+    pd.DataFrame
+        pd.DataFrame in long-format
+    """
+    mask = wide_df.isna()
+    first_row = wide_df.iloc[0].copy()
+    last_row = wide_df.iloc[-1].copy()
+
+    m = first_row.isna()
+    first_row.loc[m] = wide_df.iloc[1:3, m.to_list()].mean()
+
+    m = last_row.isna()
+    last_row.loc[m] = wide_df.iloc[-3:-1, m.to_list()].mean()
+
+    ret = wide_df.interpolate(
+        method='linear', limit_direction='both', limit=1, axis=0)
+    ret.iloc[0] = first_row
+    ret.iloc[-1] = last_row
+
+    ret = ret[mask].stack().dropna().squeeze()  # does not work with MultiIndex columns
+    ret.rename(name, inplace=True)
+    return ret
+
+
+def flatten_dict_of_dicts(d: dict, parent_key: str = '') -> dict:
+    """Build tuples for nested dictionaries for use as `pandas.MultiIndex`.
+
+    Parameters
+    ----------
+    d : dict
+        Nested dictionary for which all keys are flattened to tuples.
+    parent_key : str, optional
+        Outer key (used for recursion), by default ''
+
+    Returns
+    -------
+    dict
+        Flattend dictionary with tuple keys: {(outer_key, ..., inner_key) : value}
+    """
+    # simplified and adapted from: https://stackoverflow.com/a/6027615/9684872
+    items = []
+    for k, v in d.items():
+        new_key = parent_key + (k,) if parent_key else (k,)
+        if isinstance(v, collections.abc.MutableMapping):
+            items.extend(flatten_dict_of_dicts(v, parent_key=new_key).items())
+        else:
+            items.append((new_key, v))
+    return dict(items)
+
+
+def key_map(d: dict) -> dict:
+    """Build a schema of dicts
+
+    Parameters
+    ----------
+    d : dict
+        dictionary of dictionaries
+
+    Returns
+    -------
+    dict
+        Key map of dictionaries
+    """
+    ret = {}
+    _keys = ()
+    for k, v in d.items():
+        if isinstance(v, dict):
+            ret[k] = key_map(v)
+        else:
+            _keys = (_keys) + (k, )
+    if _keys:
+        if ret:
+            print(
+                f"Dictionaries are not of the same length: {_keys = } and {ret = }")
+            for k in _keys:
+                ret[k] = None
+        else:
+            return _keys
+    return ret
+
+
+printable = '0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ '
+
+
+def parse_query_expression(s: str, printable: str = printable) -> str:
+    """Parse a query expression for pd.DataFrame.query to a file name.
+    Removes all characters not listed in printable."""
+    return ''.join(filter(lambda x: x in printable, s))
+
+
+def length(x):
+    """Len function which return 0 if object (probably np.nan) has no length.
+    Otherwise return length of list, pandas.Series, numpy.array, dict, etc."""
+    try:
+        return len(x)
+    except BaseException:
+        return 0
+
+
+def get_last_index_matching_proportion(df_counts: pd.DataFrame,
+                                       prop: float = 0.25,
+                                       prop_col: str = 'proportion') -> object:
+    """df_counts needs to be sorted by "prop_col" (descending).
+
+    Parameters
+    ----------
+    df_counts : pd.DataFrame
+        df counts with ascending values along proportion column.
+        Index should be unique.
+    prop : float, optional
+        cutoff, inclusive, by default 0.25
+    prop_col : str, optional
+        column name for proportion, by default 'proportion'
+
+    Returns
+    -------
+    object
+        Index value for cutoff
+    """
+    assert df_counts.index.is_unique
+    mask = df_counts[prop_col] >= prop
+    idx_cutoff = df_counts[prop_col].loc[mask].tail(1).index[0]
+    return idx_cutoff
+
+
+def get_lower_whiskers(df: pd.DataFrame, factor: float = 1.5) -> pd.Series:
+    ret = df.describe()
+    iqr = ret.loc['75%'] - ret.loc['25%']
+    ret = ret.loc['25%'] - iqr * factor
+    return ret
+
+
+def get_counts_per_bin(df: pd.DataFrame, bins: range, columns: Optional[List[str]] = None):
+    """Return counts per bin for selected columns in DataFrame."""
+    counts_per_bin = dict()
+    if columns is None:
+        columns = df.columns.to_list()
+    for col in columns:
+        _series = (pd.cut(df[col], bins=bins)
+                   .to_frame()
+                   .groupby(col)
+                   .size())
+        _series.index.name = 'bin'
+        counts_per_bin[col] = _series
+    counts_per_bin = pd.DataFrame(counts_per_bin)
+    return counts_per_bin
```

### Comparing `pimms-learn-0.2.0/vaep/pandas/calc_errors.py` & `pimms_learn-0.3.0/vaep/pandas/calc_errors.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import pandas as pd
-
-
-def calc_errors_per_feat(pred: pd.DataFrame, freq_feat: pd.Series, target_col='observed') -> pd.DataFrame:
-    """Calculate absolute errors and sort by freq of features."""
-    n_obs = pred.groupby(freq_feat.index.name)[
-        target_col].count().rename('n_obs')
-    errors = pred.drop(target_col, axis=1).sub(pred[target_col], axis=0)
-    errors = errors.abs().groupby(freq_feat.index.name).mean()  # absolute error
-    errors = errors.join(freq_feat).join(n_obs)
-    errors = errors.sort_values(by=freq_feat.name, ascending=True)
-    errors.columns.name = 'model'
-    return errors
-
-
-def calc_errors_per_bin(pred: pd.DataFrame, target_col='observed') -> pd.DataFrame:
-    """Calculate absolute errors. Bin by integer value of simulated NA and provide count."""
-    errors = get_absolute_error(pred, y_true=target_col)
-    errors['bin'] = pred[target_col].astype(int)  # integer bin of simulated NA
-    n_obs = errors.groupby('bin').size().rename('n_obs')
-    errors = errors.join(n_obs, on='bin')
-    errors = errors.sort_values(by='n_obs', ascending=True)
-    errors.columns.name = 'model'
-    return errors
-
-
-def get_absolute_error(pred: pd.DataFrame, y_true: str = 'observed') -> pd.DataFrame:
-    errors = pred.drop(y_true, axis=1).sub(pred[y_true], axis=0)
-    return errors.abs()
+import pandas as pd
+
+
+def calc_errors_per_feat(pred: pd.DataFrame, freq_feat: pd.Series, target_col='observed') -> pd.DataFrame:
+    """Calculate absolute errors and sort by freq of features."""
+    n_obs = pred.groupby(freq_feat.index.name)[
+        target_col].count().rename('n_obs')
+    errors = pred.drop(target_col, axis=1).sub(pred[target_col], axis=0)
+    errors = errors.abs().groupby(freq_feat.index.name).mean()  # absolute error
+    errors = errors.join(freq_feat).join(n_obs)
+    errors = errors.sort_values(by=freq_feat.name, ascending=True)
+    errors.columns.name = 'model'
+    return errors
+
+
+def calc_errors_per_bin(pred: pd.DataFrame, target_col='observed') -> pd.DataFrame:
+    """Calculate absolute errors. Bin by integer value of simulated NA and provide count."""
+    errors = get_absolute_error(pred, y_true=target_col)
+    errors['bin'] = pred[target_col].astype(int)  # integer bin of simulated NA
+    n_obs = errors.groupby('bin').size().rename('n_obs')
+    errors = errors.join(n_obs, on='bin')
+    errors = errors.sort_values(by='n_obs', ascending=True)
+    errors.columns.name = 'model'
+    return errors
+
+
+def get_absolute_error(pred: pd.DataFrame, y_true: str = 'observed') -> pd.DataFrame:
+    errors = pred.drop(y_true, axis=1).sub(pred[y_true], axis=0)
+    return errors.abs()
```

### Comparing `pimms-learn-0.2.0/vaep/pandas/missing_data.py` & `pimms_learn-0.3.0/vaep/pandas/missing_data.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from __future__ import annotations
-from pathlib import Path
-import math
-
-import pandas as pd
-
-
-def percent_missing(df: pd.DataFrame) -> float:
-    return df.isna().sum().sum() / math.prod(df.shape)
-
-
-def percent_non_missing(df: pd.DataFrame) -> float:
-    return df.notna().sum().sum() / math.prod(df.shape)
-
-
-def list_files(folder='.') -> list[str]:
-    return [f.as_posix() for f in Path(folder).iterdir()]
-
-
-def get_record(data: pd.DataFrame, columns_sample=False) -> dict:
-    """Get summary record of data."""
-    if columns_sample:
-        M, N = data.shape
-    else:
-        N, M = data.shape
-    N_obs = data.notna().sum().sum()
-    N_mis = N * M - N_obs
-    missing = N_mis / (N_obs + N_mis)
-    record = dict(N=int(N),
-                  M=int(M),
-                  N_obs=int(N_obs),
-                  N_mis=int(N_mis),
-                  missing=float(missing), )
-    return record
+from __future__ import annotations
+from pathlib import Path
+import math
+
+import pandas as pd
+
+
+def percent_missing(df: pd.DataFrame) -> float:
+    return df.isna().sum().sum() / math.prod(df.shape)
+
+
+def percent_non_missing(df: pd.DataFrame) -> float:
+    return df.notna().sum().sum() / math.prod(df.shape)
+
+
+def list_files(folder='.') -> list[str]:
+    return [f.as_posix() for f in Path(folder).iterdir()]
+
+
+def get_record(data: pd.DataFrame, columns_sample=False) -> dict:
+    """Get summary record of data."""
+    if columns_sample:
+        M, N = data.shape
+    else:
+        N, M = data.shape
+    N_obs = data.notna().sum().sum()
+    N_mis = N * M - N_obs
+    missing = N_mis / (N_obs + N_mis)
+    record = dict(N=int(N),
+                  M=int(M),
+                  N_obs=int(N_obs),
+                  N_mis=int(N_mis),
+                  missing=float(missing), )
+    return record
```

### Comparing `pimms-learn-0.2.0/vaep/plotting/__init__.py` & `pimms_learn-0.3.0/vaep/plotting/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,326 +1,329 @@
-from __future__ import annotations
-
-from functools import partial
-import numpy as np
-import pandas as pd
-import matplotlib
-import logging
-import pathlib
-import matplotlib.pyplot as plt
-import seaborn
-
-import vaep.pandas
-
-from .errors import plot_rolling_error
-from . import errors
-from . import data
-from . import plotly
-from . defaults import order_categories, labels_dict, IDX_ORDER
-
-seaborn.set_style("whitegrid")
-# seaborn.set_theme()
-
-plt.rcParams['figure.figsize'] = [16.0, 7.0]  # [4, 2], [4, 3]
-plt.rcParams['pdf.fonttype'] = 42
-plt.rcParams['ps.fonttype'] = 42
-
-plt.rcParams['figure.dpi'] = 147
-
-
-logger = logging.getLogger(__name__)
-
-__all__ = ['plotly',
-           'data',
-           'errors',
-           'plot_rolling_error',
-           # define in this file
-           'savefig',
-           'select_xticks',
-           'select_dates',
-           'make_large_descriptors',
-           'plot_feat_counts',
-           'plot_cutoffs',
-           ]
-
-
-def _savefig(fig, name, folder: pathlib.Path = '.',
-             pdf=True,
-             dpi=300  # default 'figure'
-             ):
-    """Save matplotlib Figure (having method `savefig`) as pdf and png."""
-    folder = pathlib.Path(folder)
-    fname = folder / name
-    folder = fname.parent  # in case name specifies folders
-    folder.mkdir(exist_ok=True, parents=True)
-    fig.tight_layout()
-    fig.savefig(fname.with_suffix('.png'), dpi=dpi)
-    if pdf:
-        fig.savefig(fname.with_suffix('.pdf'), dpi=dpi)
-    logger.info(f"Saved Figures to {fname}")
-
-
-savefig = _savefig
-
-
-def select_xticks(ax: matplotlib.axes.Axes, max_ticks: int = 50) -> list:
-    """Limit the number of xticks displayed.
-
-    Parameters
-    ----------
-    ax : matplotlib.axes.Axes
-        Axes object to manipulate
-    max_ticks : int, optional
-        maximum number of set ticks on x-axis, by default 50
-
-    Returns
-    -------
-    list
-        list of current ticks for x-axis. Either new
-        or old (depending if something was changed).
-    """
-    x_ticks = ax.get_xticks()
-    offset = len(x_ticks) // max_ticks
-    if offset > 1:  # if larger than 1
-        return ax.set_xticks(x_ticks[::offset])
-    return x_ticks
-
-
-def select_dates(date_series: pd.Series, max_ticks=30) -> np.array:
-    """Get unique dates (single days) for selection in pd.plot.line
-    with xticks argument.
-
-    Parameters
-    ----------
-    date_series : pd.Series
-        datetime series to use (values, not index)
-    max_ticks : int, optional
-        maximum number of unique ticks to select, by default 30
-
-    Returns
-    -------
-    np.array
-        _description_
-    """
-    xticks = date_series.dt.date.unique()
-    offset = len(xticks) // max_ticks
-    if offset > 1:
-        return xticks[::offset]
-    else:
-        xticks
-
-
-def make_large_descriptors(size='xx-large'):
-    """Helper function to have very large titles, labes and tick texts for
-    matplotlib plots per default.
-
-    size: str
-        fontsize or allowed category. Change default if necessary, default 'xx-large'
-    """
-    plt.rcParams.update({k: size for k in ['xtick.labelsize',
-                                           'ytick.labelsize',
-                                           'axes.titlesize',
-                                           'axes.labelsize',
-                                           'legend.fontsize',
-                                           'legend.title_fontsize']
-                         })
-
-
-def add_prop_as_second_yaxis(ax: matplotlib.axes.Axes, n_samples: int,
-                             format_str: str = '{x:,.3f}') -> matplotlib.axes.Axes:
-    """Add proportion as second axis. Try to align cleverly
-
-    Parameters
-    ----------
-    ax : matplotlib.axes.Axes
-        Axes for which you want to add a second y-axis
-    n_samples : int
-        Number of total samples (to normalize against)
-
-    Returns
-    -------
-    matplotlib.axes.Axes
-        Second layover twin Axes with right-hand side y-axis
-    """
-    ax2 = ax.twinx()
-    n_min, n_max = np.round(ax.get_ybound())
-    logger.info(f"{n_min = }, {n_max = }")
-    lower_prop = n_min / n_samples + (ax.get_ybound()[0] - n_min) / n_samples
-    upper_prop = n_max / n_samples + (ax.get_ybound()[1] - n_max) / n_samples
-    logger.info(f'{lower_prop = }, {upper_prop = }')
-    ax2.set_ybound(lower_prop, upper_prop)
-    # _ = ax2.set_yticks(np.linspace(n_min/n_samples,
-    #                    n_max /n_samples, len(ax.get_yticks())-2))
-    _ = ax2.set_yticks(ax.get_yticks()[1:-1] / n_samples)
-    ax2.yaxis.set_major_formatter(
-        matplotlib.ticker.StrMethodFormatter(format_str))
-    return ax2
-
-
-def add_height_to_barplot(ax, size=5, rotated=False):
-    ax.annotate = partial(ax.annotate, text='NA',
-                          xytext=(0, int(size / 2)),
-                          ha='center',
-                          size=size,
-                          textcoords='offset points')
-    ax.annotate = partial(ax.annotate,
-                          rotation=0,
-                          va='center')
-    if rotated:
-        ax.annotate = partial(ax.annotate,
-                              xytext=(1, int(size / 3)),
-                              rotation=90,
-                              va='bottom')
-    for bar in ax.patches:
-        if not bar.get_height():
-            xy = (bar.get_x() + bar.get_width() / 2,
-                  0.0)
-            ax.annotate(text='NA',
-                        xy=xy,
-                        )
-            continue
-        ax.annotate(text=format(bar.get_height(), '.2f'),
-                    xy=(bar.get_x() + bar.get_width() / 2,
-                        bar.get_height()),
-                    )
-    return ax
-
-
-def add_text_to_barplot(ax, text, size=5):
-    for bar, text_ in zip(ax.patches, text):
-        logger.debug(f"{bar = }, f{text = }, {bar.get_height() = }")
-        if not bar.get_height():
-            continue
-        ax.annotate(text=text_,
-                    xy=(bar.get_x() + bar.get_width() / 2,
-                        bar.get_height()),
-                    xytext=(1, -5),
-                    rotation=90,
-                    ha='center',
-                    va='top',
-                    size=size,
-                    textcoords='offset points')
-    return ax
-
-
-def format_large_numbers(ax: matplotlib.axes.Axes,
-                         format_str: str = '{x:,.0f}') -> matplotlib.axes.Axes:
-    """Format large integer numbers to be read more easily.
-
-    Parameters
-    ----------
-    ax : matplotlib.axes.Axes
-        Axes which labels should be manipulated.
-    format_str : str, optional
-        Default float format string, by default '{x:,.0f}'
-
-    Returns
-    -------
-    matplotlib.axes.Axes
-        _description_
-    """
-    ax.xaxis.set_major_formatter(
-        matplotlib.ticker.StrMethodFormatter(format_str))
-    ax.yaxis.set_major_formatter(
-        matplotlib.ticker.StrMethodFormatter(format_str))
-    return ax
-
-
-def plot_feat_counts(df_counts: pd.DataFrame, feat_name: str, n_samples: int,
-                     ax=None, figsize=(15, 10),
-                     count_col='counts',
-                     **kwargs):
-    args = dict(
-        ylabel='count',
-        xlabel=f'{feat_name} ordered by completeness',
-        title=f'Count and proportion of {len(df_counts):,d} {feat_name}s over {n_samples:,d} samples',
-    )
-    args.update(kwargs)
-
-    ax = df_counts[count_col].plot(
-        figsize=figsize,
-
-        grid=True,
-        ax=ax,
-        **args)
-
-    # default nearly okay, but rather customize to see minimal and maxium proportion
-    # ax = peptide_counts['proportion'].plot(secondary_y=True, style='b')
-
-    ax2 = add_prop_as_second_yaxis(ax=ax, n_samples=n_samples)
-    ax2.set_ylabel('proportion')
-    ax = format_large_numbers(ax=ax)
-    return ax
-
-
-def plot_counts(df_counts: pd.DataFrame, n_samples,
-                feat_col_name: str = 'count',
-                feature_name=None,
-                ax=None, prop_feat=0.25, min_feat_prop=.01,
-                **kwargs):
-    """Plot counts based on get_df_counts."""
-    if feature_name is None:
-        feature_name = feat_col_name
-    # df_counts = df_counts[[feat_col_name]].copy()
-    ax = plot_feat_counts(df_counts,
-                          feat_name=feature_name,
-                          n_samples=n_samples,
-                          count_col=feat_col_name,
-                          ax=ax, **kwargs)
-    df_counts['prop'] = df_counts[feat_col_name] / n_samples
-    n_feat_cutoff = vaep.pandas.get_last_index_matching_proportion(
-        df_counts=df_counts, prop=prop_feat, prop_col='prop')
-    n_samples_cutoff = df_counts.loc[n_feat_cutoff, feat_col_name]
-    logger.info(f'{n_feat_cutoff = }, {n_samples_cutoff = }')
-    x_lim_max = vaep.pandas.get_last_index_matching_proportion(
-        df_counts, min_feat_prop, prop_col='prop')
-    logger.info(f'{x_lim_max = }')
-    ax.set_xlim(-1, x_lim_max)
-    ax.axvline(n_feat_cutoff, c='red')
-
-    # ax.text(n_feat_cutoff + 0.03 * x_lim_max,
-    #         n_samples_cutoff, '25% cutoff',
-    #         style='italic', fontsize=12,
-    #         bbox={'facecolor': 'grey', 'alpha': 0.5, 'pad': 10})
-
-    ax.annotate(f'{prop_feat*100}% cutoff',
-                xy=(n_feat_cutoff, n_samples_cutoff),
-                xytext=(n_feat_cutoff + 0.1 * x_lim_max, n_samples_cutoff),
-                fontsize=16,
-                arrowprops=dict(facecolor='black', shrink=0.05))
-    return ax
-
-
-def plot_cutoffs(df: pd.DataFrame,
-                 feat_completness_over_samples: int = None,
-                 min_feat_in_sample: int = None
-                 ) -> tuple[matplotlib.figure.Figure, np.array[matplotlib.axes.Axes]]:
-    """plot number of available features along index and columns (feat vs samples),
-    potentially including some cutoff.
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        DataFrame in wide data format.
-    feat_completness_over_samples : int, optional
-        horizental line to plot as cutoff for features, by default None
-    min_feat_in_sample : int, optional
-        horizental line to plot as cutoff for samples, by default None
-
-    Returns
-    -------
-    tuple[matplotlib.figure.Figure, np.array[matplotlib.axes.Axes]]
-        _description_
-    """
-    notna = df.notna()
-    fig, axes = plt.subplots(1, 2)
-    ax = axes[0]
-    notna.sum(axis=0).sort_values().plot(rot=90, ax=ax,
-                                         ylabel='count samples', xlabel='feature name')
-    if feat_completness_over_samples is not None:
-        ax.axhline(feat_completness_over_samples)
-    ax = axes[1]
-    notna.sum(axis=1).sort_values().plot(rot=90, ax=ax,
-                                         ylabel='count features', xlabel='sample name')
-    if min_feat_in_sample is not None:
-        ax.axhline(min_feat_in_sample)
-    return fig, axes
+from __future__ import annotations
+
+import logging
+import pathlib
+from functools import partial
+
+import matplotlib
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
+import seaborn
+
+import vaep.pandas
+
+from . import data, defaults, errors, plotly
+from .errors import plot_rolling_error
+
+# from . defaults import order_categories, labels_dict, IDX_ORDER
+
+seaborn.set_style("whitegrid")
+# seaborn.set_theme()
+
+plt.rcParams['figure.figsize'] = [16.0, 7.0]  # [4, 2], [4, 3]
+plt.rcParams['pdf.fonttype'] = 42
+plt.rcParams['ps.fonttype'] = 42
+
+plt.rcParams['figure.dpi'] = 147
+
+
+logger = logging.getLogger(__name__)
+
+__all__ = ['plotly',
+           'data',
+           'defaults',
+           'errors',
+           'plot_rolling_error',
+           # define in this file
+           'savefig',
+           'select_xticks',
+           'select_dates',
+           'make_large_descriptors',
+           'plot_feat_counts',
+           'plot_cutoffs',
+           ]
+
+
+def _savefig(fig, name, folder: pathlib.Path = '.',
+             pdf=True,
+             dpi=300,  # default 'figure',
+             tight_layout=True,
+             ):
+    """Save matplotlib Figure (having method `savefig`) as pdf and png."""
+    folder = pathlib.Path(folder)
+    fname = folder / name
+    folder = fname.parent  # in case name specifies folders
+    folder.mkdir(exist_ok=True, parents=True)
+    if tight_layout:
+        fig.tight_layout()
+    fig.savefig(fname.with_suffix('.png'), dpi=dpi)
+    if pdf:
+        fig.savefig(fname.with_suffix('.pdf'), dpi=dpi)
+    logger.info(f"Saved Figures to {fname}")
+
+
+savefig = _savefig
+
+
+def select_xticks(ax: matplotlib.axes.Axes, max_ticks: int = 50) -> list:
+    """Limit the number of xticks displayed.
+
+    Parameters
+    ----------
+    ax : matplotlib.axes.Axes
+        Axes object to manipulate
+    max_ticks : int, optional
+        maximum number of set ticks on x-axis, by default 50
+
+    Returns
+    -------
+    list
+        list of current ticks for x-axis. Either new
+        or old (depending if something was changed).
+    """
+    x_ticks = ax.get_xticks()
+    offset = len(x_ticks) // max_ticks
+    if offset > 1:  # if larger than 1
+        return ax.set_xticks(x_ticks[::offset])
+    return x_ticks
+
+
+def select_dates(date_series: pd.Series, max_ticks=30) -> np.array:
+    """Get unique dates (single days) for selection in pd.plot.line
+    with xticks argument.
+
+    Parameters
+    ----------
+    date_series : pd.Series
+        datetime series to use (values, not index)
+    max_ticks : int, optional
+        maximum number of unique ticks to select, by default 30
+
+    Returns
+    -------
+    np.array
+        _description_
+    """
+    xticks = date_series.dt.date.unique()
+    offset = len(xticks) // max_ticks
+    if offset > 1:
+        return xticks[::offset]
+    else:
+        xticks
+
+
+def make_large_descriptors(size='xx-large'):
+    """Helper function to have very large titles, labes and tick texts for
+    matplotlib plots per default.
+
+    size: str
+        fontsize or allowed category. Change default if necessary, default 'xx-large'
+    """
+    plt.rcParams.update({k: size for k in ['xtick.labelsize',
+                                           'ytick.labelsize',
+                                           'axes.titlesize',
+                                           'axes.labelsize',
+                                           'legend.fontsize',
+                                           'legend.title_fontsize']
+                         })
+
+
+def add_prop_as_second_yaxis(ax: matplotlib.axes.Axes, n_samples: int,
+                             format_str: str = '{x:,.3f}') -> matplotlib.axes.Axes:
+    """Add proportion as second axis. Try to align cleverly
+
+    Parameters
+    ----------
+    ax : matplotlib.axes.Axes
+        Axes for which you want to add a second y-axis
+    n_samples : int
+        Number of total samples (to normalize against)
+
+    Returns
+    -------
+    matplotlib.axes.Axes
+        Second layover twin Axes with right-hand side y-axis
+    """
+    ax2 = ax.twinx()
+    n_min, n_max = np.round(ax.get_ybound())
+    logger.info(f"{n_min = }, {n_max = }")
+    lower_prop = n_min / n_samples + (ax.get_ybound()[0] - n_min) / n_samples
+    upper_prop = n_max / n_samples + (ax.get_ybound()[1] - n_max) / n_samples
+    logger.info(f'{lower_prop = }, {upper_prop = }')
+    ax2.set_ybound(lower_prop, upper_prop)
+    # _ = ax2.set_yticks(np.linspace(n_min/n_samples,
+    #                    n_max /n_samples, len(ax.get_yticks())-2))
+    _ = ax2.set_yticks(ax.get_yticks()[1:-1] / n_samples)
+    ax2.yaxis.set_major_formatter(
+        matplotlib.ticker.StrMethodFormatter(format_str))
+    return ax2
+
+
+def add_height_to_barplot(ax, size=5, rotated=False):
+    ax.annotate = partial(ax.annotate, text='NA',
+                          xytext=(0, int(size / 2)),
+                          ha='center',
+                          size=size,
+                          textcoords='offset points')
+    ax.annotate = partial(ax.annotate,
+                          rotation=0,
+                          va='center')
+    if rotated:
+        ax.annotate = partial(ax.annotate,
+                              xytext=(1, int(size / 3)),
+                              rotation=90,
+                              va='bottom')
+    for bar in ax.patches:
+        if not bar.get_height():
+            xy = (bar.get_x() + bar.get_width() / 2,
+                  0.0)
+            ax.annotate(text='NA',
+                        xy=xy,
+                        )
+            continue
+        ax.annotate(text=format(bar.get_height(), '.2f'),
+                    xy=(bar.get_x() + bar.get_width() / 2,
+                        bar.get_height()),
+                    )
+    return ax
+
+
+def add_text_to_barplot(ax, text, size=5):
+    for bar, text_ in zip(ax.patches, text):
+        logger.debug(f"{bar = }, f{text = }, {bar.get_height() = }")
+        if not bar.get_height():
+            continue
+        ax.annotate(text=text_,
+                    xy=(bar.get_x() + bar.get_width() / 2,
+                        bar.get_height()),
+                    xytext=(1, -5),
+                    rotation=90,
+                    ha='center',
+                    va='top',
+                    size=size,
+                    textcoords='offset points')
+    return ax
+
+
+def format_large_numbers(ax: matplotlib.axes.Axes,
+                         format_str: str = '{x:,.0f}') -> matplotlib.axes.Axes:
+    """Format large integer numbers to be read more easily.
+
+    Parameters
+    ----------
+    ax : matplotlib.axes.Axes
+        Axes which labels should be manipulated.
+    format_str : str, optional
+        Default float format string, by default '{x:,.0f}'
+
+    Returns
+    -------
+    matplotlib.axes.Axes
+        _description_
+    """
+    ax.xaxis.set_major_formatter(
+        matplotlib.ticker.StrMethodFormatter(format_str))
+    ax.yaxis.set_major_formatter(
+        matplotlib.ticker.StrMethodFormatter(format_str))
+    return ax
+
+
+def plot_feat_counts(df_counts: pd.DataFrame, feat_name: str, n_samples: int,
+                     ax=None, figsize=(15, 10),
+                     count_col='counts',
+                     **kwargs):
+    args = dict(
+        ylabel='count',
+        xlabel=f'{feat_name} ordered by completeness',
+        title=f'Count and proportion of {len(df_counts):,d} {feat_name}s over {n_samples:,d} samples',
+    )
+    args.update(kwargs)
+
+    ax = df_counts[count_col].plot(
+        figsize=figsize,
+
+        grid=True,
+        ax=ax,
+        **args)
+
+    # default nearly okay, but rather customize to see minimal and maxium proportion
+    # ax = peptide_counts['proportion'].plot(secondary_y=True, style='b')
+
+    ax2 = add_prop_as_second_yaxis(ax=ax, n_samples=n_samples)
+    ax2.set_ylabel('proportion')
+    ax = format_large_numbers(ax=ax)
+    return ax
+
+
+def plot_counts(df_counts: pd.DataFrame, n_samples,
+                feat_col_name: str = 'count',
+                feature_name=None,
+                ax=None, prop_feat=0.25, min_feat_prop=.01,
+                **kwargs):
+    """Plot counts based on get_df_counts."""
+    if feature_name is None:
+        feature_name = feat_col_name
+    # df_counts = df_counts[[feat_col_name]].copy()
+    ax = plot_feat_counts(df_counts,
+                          feat_name=feature_name,
+                          n_samples=n_samples,
+                          count_col=feat_col_name,
+                          ax=ax, **kwargs)
+    df_counts['prop'] = df_counts[feat_col_name] / n_samples
+    n_feat_cutoff = vaep.pandas.get_last_index_matching_proportion(
+        df_counts=df_counts, prop=prop_feat, prop_col='prop')
+    n_samples_cutoff = df_counts.loc[n_feat_cutoff, feat_col_name]
+    logger.info(f'{n_feat_cutoff = }, {n_samples_cutoff = }')
+    x_lim_max = vaep.pandas.get_last_index_matching_proportion(
+        df_counts, min_feat_prop, prop_col='prop')
+    logger.info(f'{x_lim_max = }')
+    ax.set_xlim(-1, x_lim_max)
+    ax.axvline(n_feat_cutoff, c='red')
+
+    # ax.text(n_feat_cutoff + 0.03 * x_lim_max,
+    #         n_samples_cutoff, '25% cutoff',
+    #         style='italic', fontsize=12,
+    #         bbox={'facecolor': 'grey', 'alpha': 0.5, 'pad': 10})
+
+    ax.annotate(f'{prop_feat*100}% cutoff',
+                xy=(n_feat_cutoff, n_samples_cutoff),
+                xytext=(n_feat_cutoff + 0.1 * x_lim_max, n_samples_cutoff),
+                fontsize=16,
+                arrowprops=dict(facecolor='black', shrink=0.05))
+    return ax
+
+
+def plot_cutoffs(df: pd.DataFrame,
+                 feat_completness_over_samples: int = None,
+                 min_feat_in_sample: int = None
+                 ) -> tuple[matplotlib.figure.Figure, np.array[matplotlib.axes.Axes]]:
+    """plot number of available features along index and columns (feat vs samples),
+    potentially including some cutoff.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        DataFrame in wide data format.
+    feat_completness_over_samples : int, optional
+        horizental line to plot as cutoff for features, by default None
+    min_feat_in_sample : int, optional
+        horizental line to plot as cutoff for samples, by default None
+
+    Returns
+    -------
+    tuple[matplotlib.figure.Figure, np.array[matplotlib.axes.Axes]]
+        _description_
+    """
+    notna = df.notna()
+    fig, axes = plt.subplots(1, 2)
+    ax = axes[0]
+    notna.sum(axis=0).sort_values().plot(rot=90, ax=ax,
+                                         ylabel='count samples', xlabel='feature name')
+    if feat_completness_over_samples is not None:
+        ax.axhline(feat_completness_over_samples)
+    ax = axes[1]
+    notna.sum(axis=1).sort_values().plot(rot=90, ax=ax,
+                                         ylabel='count features', xlabel='sample name')
+    if min_feat_in_sample is not None:
+        ax.axhline(min_feat_in_sample)
+    return fig, axes
```

### Comparing `pimms-learn-0.2.0/vaep/plotting/defaults.py` & `pimms_learn-0.3.0/vaep/plotting/defaults.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,109 +1,90 @@
-import logging
-import matplotlib as mpl
-import seaborn as sns
-
-logger = logging.getLogger(__name__)
-
-# ! default seaborn color map only has 10 colors
-# https://seaborn.pydata.org/tutorial/color_palettes.html
-# sns.color_palette("husl", N) to get N distinct colors
-color_model_mapping = {
-    'KNN': sns.color_palette()[0],
-    'KNN_IMPUTE': sns.color_palette()[1],
-    'CF': sns.color_palette()[2],
-    'DAE': sns.color_palette()[3],
-    'VAE': sns.color_palette()[4],
-    'RF': sns.color_palette()[5],
-    'Median': sns.color_palette()[6],
-    'None': sns.color_palette()[7],
-    'BPCA': sns.color_palette()[8],
-    'MICE-CART': sns.color_palette()[9],
-
-}
-# other_colors = sns.color_palette()[8:]
-other_colors = sns.color_palette("husl", 20)
-color_model_mapping['IMPSEQ'] = other_colors[0]
-color_model_mapping['QRILC'] = other_colors[1]
-color_model_mapping['IMPSEQROB'] = other_colors[1]
-color_model_mapping['MICE-NORM'] = other_colors[2]
-color_model_mapping['SEQKNN'] = other_colors[3]
-color_model_mapping['IMPSEQROB'] = other_colors[4]
-color_model_mapping['GSIMP'] = other_colors[5]
-color_model_mapping['MSIMPUTE'] = other_colors[6]
-color_model_mapping['MSIMPUTE_MNAR'] = other_colors[7]
-color_model_mapping['TRKNN'] = other_colors[8]
-color_model_mapping['SVDMETHOD'] = other_colors[9]
-other_colors = other_colors[10:]
-
-
-def assign_colors(models):
-    i = 0
-    ret_colors = list()
-    for model in models:
-        if model in color_model_mapping:
-            ret_colors.append(color_model_mapping[model])
-        else:
-            pos = i % len(other_colors)
-            ret_colors.append(other_colors[pos])
-            i += 1
-    if i > len(other_colors):
-        logger.info("Reused some colors!")
-    return ret_colors
-
-
-class ModelColorVisualizer:
-
-    def __init__(self, models, palette):
-        self.models = models
-        self.palette = map(mpl.colors.colorConverter.to_rgb, palette)
-
-    def as_hex(self):
-        """Return a color palette with hex codes instead of RGB values."""
-        hex = [mpl.colors.rgb2hex(rgb) for rgb in self.palette]
-        return hex
-
-    def _repr_html_(self):
-        """Rich display of the color palette in an HTML frontend."""
-        s = 55
-        n = len(self.models)
-        html = f'<svg  width="{s*2}" height="{s*n/2}">'
-        for i, (m, c) in enumerate(zip(self.models, self.as_hex())):
-            html += (
-                f'<rect x="0" y="{i * s /2}" width="{s*2}" height="{s/2}" style="fill:{c};'
-                'stroke-width:2;stroke:rgb(255,255,255)" metadata="tt"/>'
-            )
-            html += f'<text x="{4}" y="{(i * s / 2) + 20}" font-size="12" fill="black">{m}</text>'
-        html += '</svg>'
-        return html
-
-
-labels_dict = {"NA not interpolated valid_collab collab MSE": 'MSE',
-               'batch_size': 'bs',
-               'n_hidden_layers': "No. of hidden layers",
-               'latent_dim': 'hidden layer dimension',
-               'subset_w_N': 'subset',
-               'n_params': 'no. of parameter',
-               "metric_value": 'value',
-               'metric_name': 'metric',
-               }
-
-order_categories = {'data level': ['proteinGroups', 'aggPeptides', 'evidence'],
-                    'model': ['median', 'interpolated', 'CF', 'DAE', 'VAE']}
-
-IDX_ORDER = (['proteinGroups', 'aggPeptides', 'evidence'],
-             ['median', 'interpolated', 'CF', 'DAE', 'VAE'])
-
-
-ORDER_MODELS = ['RSN', 'median', 'interpolated',
-                'CF', 'DAE', 'VAE',
-                ]
-
-l_colors_to_use_hex = ['#937860',  # seaborn brown
-                       '#4c72b0',  # seaborn blue
-                       '#dd8452',  # seaborn organe
-                       '#55a868',  # seaborn green
-                       '#c44e52',  # seaborn red
-                       '#8172b3',  # seaborn violete/lila
-                       ]
-
-d_colors_to_use_hex = {k: v for k, v in zip(ORDER_MODELS, l_colors_to_use_hex)}
+import logging
+
+import matplotlib as mpl
+import seaborn as sns
+
+logger = logging.getLogger(__name__)
+
+# ! default seaborn color map only has 10 colors
+# https://seaborn.pydata.org/tutorial/color_palettes.html
+# sns.color_palette("husl", N) to get N distinct colors
+color_model_mapping = {
+    'KNN': sns.color_palette()[0],
+    'KNN_IMPUTE': sns.color_palette()[1],
+    'CF': sns.color_palette()[2],
+    'DAE': sns.color_palette()[3],
+    'VAE': sns.color_palette()[4],
+    'RF': sns.color_palette()[5],
+    'Median': sns.color_palette()[6],
+    'None': sns.color_palette()[7],
+    'BPCA': sns.color_palette()[8],
+    'MICE-CART': sns.color_palette()[9],
+
+}
+# other_colors = sns.color_palette()[8:]
+other_colors = sns.color_palette("husl", 20)
+color_model_mapping['IMPSEQ'] = other_colors[0]
+color_model_mapping['QRILC'] = other_colors[1]
+color_model_mapping['IMPSEQROB'] = other_colors[1]
+color_model_mapping['MICE-NORM'] = other_colors[2]
+color_model_mapping['SEQKNN'] = other_colors[3]
+color_model_mapping['IMPSEQROB'] = other_colors[4]
+color_model_mapping['GSIMP'] = other_colors[5]
+color_model_mapping['MSIMPUTE'] = other_colors[6]
+color_model_mapping['MSIMPUTE_MNAR'] = other_colors[7]
+color_model_mapping['TRKNN'] = other_colors[8]
+color_model_mapping['SVDMETHOD'] = other_colors[9]
+other_colors = other_colors[10:]
+
+
+def assign_colors(models):
+    i = 0
+    ret_colors = list()
+    for model in models:
+        if model in color_model_mapping:
+            ret_colors.append(color_model_mapping[model])
+        else:
+            pos = i % len(other_colors)
+            ret_colors.append(other_colors[pos])
+            i += 1
+    if i > len(other_colors):
+        logger.info("Reused some colors!")
+    return ret_colors
+
+
+class ModelColorVisualizer:
+
+    def __init__(self, models, palette):
+        self.models = models
+        self.palette = map(mpl.colors.colorConverter.to_rgb, palette)
+
+    def as_hex(self):
+        """Return a color palette with hex codes instead of RGB values."""
+        hex = [mpl.colors.rgb2hex(rgb) for rgb in self.palette]
+        return hex
+
+    def _repr_html_(self):
+        """Rich display of the color palette in an HTML frontend."""
+        s = 55
+        n = len(self.models)
+        html = f'<svg  width="{s*2}" height="{s*n/2}">'
+        for i, (m, c) in enumerate(zip(self.models, self.as_hex())):
+            html += (
+                f'<rect x="0" y="{i * s /2}" width="{s*2}" height="{s/2}" style="fill:{c};'
+                'stroke-width:2;stroke:rgb(255,255,255)" metadata="tt"/>'
+            )
+            html += f'<text x="{4}" y="{(i * s / 2) + 20}" font-size="12" fill="black">{m}</text>'
+        html += '</svg>'
+        return html
+
+
+labels_dict = {"NA not interpolated valid_collab collab MSE": 'MSE',
+               'batch_size': 'bs',
+               'n_hidden_layers': "No. of hidden layers",
+               'latent_dim': 'hidden layer dimension',
+               'subset_w_N': 'subset',
+               'n_params': 'no. of parameter',
+               "metric_value": 'value',
+               'metric_name': 'metric',
+               }
+
```

### Comparing `pimms-learn-0.2.0/vaep/sklearn/ae_transformer.py` & `pimms_learn-0.3.0/vaep/sklearn/ae_transformer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,147 +1,155 @@
-"""Scikit-learn style interface for Denoising and Variational Autoencoder model."""
-from __future__ import annotations
-
-from sklearn.impute import SimpleImputer
-from sklearn.preprocessing import StandardScaler
-import sklearn
-
-from pathlib import Path
-
-
-from fastai.basics import *
-from fastai.callback.all import *
-from fastai.torch_basics import *
-
-from fastai import learner
-
-from sklearn.utils.validation import check_is_fitted
-from sklearn.base import BaseEstimator, TransformerMixin
-
-from typing import Optional
-
-import vaep.models as models
-from vaep.models import ae
-
-
-# patch plotting function
-from vaep.models import plot_loss
-learner.Recorder.plot_loss = plot_loss
-
-
-default_pipeline = sklearn.pipeline.Pipeline(
-    [
-        ('normalize', StandardScaler()),
-        ('impute', SimpleImputer(add_indicator=False))
-    ])
-
-
-class AETransformer(TransformerMixin, BaseEstimator):
-    """Collaborative Filtering transformer.
-
-
-    Parameters
-    ----------
-    demo_param : str, default='demo'
-        A parameter used for demonstation of how to pass and store paramters.
-
-    Attributes
-    ----------
-    n_features_ : int
-        The number of features of the data passed to :meth:`fit`.
-    """
-
-    def __init__(self,
-                 hidden_layers: list[int],
-                 latent_dim: int = 15,
-                 out_folder: str = '.',
-                 model='VAE',
-                 #  y_range:Optional[tuple[int]]=None,
-                 batch_size: int = 64,
-                 ):
-        self.hidden_layers = hidden_layers
-        self.latent_dim = latent_dim
-        self.batch_size = batch_size
-        self.out_folder = Path(out_folder)
-
-        if model == 'VAE':
-            self.model = models.vae.VAE
-            self.cbs = [ae.ModelAdapterVAE()]
-            self.loss_fct = models.vae.loss_fct
-        elif model == 'DAE':
-            self.model = ae.Autoencoder
-            self.cbs = [ae.ModelAdapter(p=0.2)]
-            self.loss_fct = MSELossFlat(reduction='sum')
-        else:
-            raise ValueError(f'Unknown model {model}, choose either "VAE" or "DAE"')
-        self.model_name = model
-        # ! patience?
-        # EarlyStoppingCallback(patience=args.patience)
-
-    def fit(self, X, y,
-            epochs_max: int = 100,
-            cuda: bool = True,
-            patience: Optional[int] = None):
-        self.analysis = ae.AutoEncoderAnalysis(  # datasplits=data,
-            train_df=X,
-            val_df=y,
-            model=self.model,
-            model_kwargs=dict(n_features=X.shape[-1],
-                              n_neurons=self.hidden_layers,
-                              last_decoder_activation=None,
-                              dim_latent=self.latent_dim),
-            transform=default_pipeline,
-            decode=['normalize'],
-            bs=self.batch_size)
-
-        self.n_params = self.analysis.n_params_ae
-        if cuda:
-            self.analysis.model = self.analysis.model.cuda()
-
-        # results = []
-        # loss_fct = partial(models.vae.loss_fct, results=results)
-        cbs = self.cbs
-        if patience is not None:
-            cbs = [*self.cbs, EarlyStoppingCallback(patience=patience)]
-        self.analysis.learn = Learner(dls=self.analysis.dls,
-                                      model=self.analysis.model,
-                                      loss_func=self.loss_fct,
-                                      cbs=cbs
-                                      )
-
-        suggested_lr = self.analysis.learn.lr_find()
-        self.analysis.params['suggested_inital_lr'] = suggested_lr.valley
-        self.analysis.learn.fit_one_cycle(epochs_max, lr_max=suggested_lr.valley)
-        self.epochs_trained_ = self.analysis.learn.epoch + 1
-        N_train_notna = X.notna().sum().sum()
-        N_val_notna = y.notna().sum().sum()
-        self.fig_loss_ = models.plot_training_losses(
-            self.analysis.learn, self.model_name,
-            folder=self.out_folder,
-            norm_factors=[N_train_notna, N_val_notna])
-        return self
-
-    def transform(self, X):
-        """ A reference implementation of a transform function.
-
-        Parameters
-        ----------
-        X : {array-like, sparse-matrix}, shape (n_samples, n_features)
-            The input samples.
-
-        Returns
-        -------
-        X_transformed : array, shape (n_samples, n_features)
-            The array containing the element-wise square roots of the values
-            in ``X``.
-        """
-        # Check is fit had been called
-        check_is_fitted(self, 'epochs_trained_')
-
-        self.analysis.model.eval()
-
-        pred, target = ae.get_preds_from_df(
-            df=X,
-            learn=self.analysis.learn,
-            position_pred_tuple=0,
-            transformer=self.analysis.transform)
-        return X.fillna(pred)
+"""Scikit-learn style interface for Denoising and Variational Autoencoder model."""
+from __future__ import annotations
+
+from sklearn.impute import SimpleImputer
+from sklearn.preprocessing import StandardScaler
+import sklearn
+
+from pathlib import Path
+import pandas as pd
+
+from fastai.losses import MSELossFlat
+from fastai.callback.tracker import EarlyStoppingCallback
+from fastai.learner import Learner
+from fastai.basics import *
+from fastai.callback.all import *
+from fastai.torch_basics import *
+
+from fastai import learner
+
+from sklearn.utils.validation import check_is_fitted
+from sklearn.base import BaseEstimator, TransformerMixin
+
+from typing import Optional
+
+import vaep.models as models
+from vaep.models import ae
+
+
+# patch plotting function
+from vaep.models import plot_loss
+learner.Recorder.plot_loss = plot_loss
+
+
+default_pipeline = sklearn.pipeline.Pipeline(
+    [
+        ('normalize', StandardScaler()),
+        ('impute', SimpleImputer(add_indicator=False))
+    ])
+
+
+class AETransformer(TransformerMixin, BaseEstimator):
+    """Collaborative Filtering transformer.
+
+
+    Parameters
+    ----------
+    demo_param : str, default='demo'
+        A parameter used for demonstation of how to pass and store paramters.
+
+    Attributes
+    ----------
+    n_features_ : int
+        The number of features of the data passed to :meth:`fit`.
+    """
+
+    def __init__(self,
+                 hidden_layers: list[int],
+                 latent_dim: int = 15,
+                 out_folder: str = '.',
+                 model='VAE',
+                 #  y_range:Optional[tuple[int]]=None,
+                 batch_size: int = 64,
+                 ):
+        self.hidden_layers = hidden_layers
+        self.latent_dim = latent_dim
+        self.batch_size = batch_size
+        self.out_folder = Path(out_folder)
+        self.out_folder.mkdir(exist_ok=True, parents=True)
+
+        if model == 'VAE':
+            self.model = models.vae.VAE
+            self.cbs = [ae.ModelAdapterVAE()]
+            self.loss_fct = models.vae.loss_fct
+        elif model == 'DAE':
+            self.model = ae.Autoencoder
+            self.cbs = [ae.ModelAdapter(p=0.2)]
+            self.loss_fct = MSELossFlat(reduction='sum')
+        else:
+            raise ValueError(f'Unknown model {model}, choose either "VAE" or "DAE"')
+        self.model_name = model
+        # ! patience?
+        # EarlyStoppingCallback(patience=args.patience)
+
+    def fit(self,
+            X: pd.DataFrame,
+            y: pd.DataFrame = None,
+            epochs_max: int = 100,
+            cuda: bool = True,
+            patience: Optional[int] = None):
+        self.analysis = ae.AutoEncoderAnalysis(  # datasplits=data,
+            train_df=X,
+            val_df=y,
+            model=self.model,
+            model_kwargs=dict(n_features=X.shape[-1],
+                              n_neurons=self.hidden_layers,
+                              last_decoder_activation=None,
+                              dim_latent=self.latent_dim),
+            transform=default_pipeline,
+            decode=['normalize'],
+            bs=self.batch_size)
+
+        self.n_params = self.analysis.n_params_ae
+        if cuda:
+            self.analysis.model = self.analysis.model.cuda()
+
+        # results = []
+        # loss_fct = partial(models.vae.loss_fct, results=results)
+        cbs = self.cbs
+        if patience is not None:
+            cbs = [*self.cbs, EarlyStoppingCallback(patience=patience)]
+        self.analysis.learn = Learner(dls=self.analysis.dls,
+                                      model=self.analysis.model,
+                                      loss_func=self.loss_fct,
+                                      cbs=cbs
+                                      )
+
+        suggested_lr = self.analysis.learn.lr_find()
+        self.analysis.params['suggested_inital_lr'] = suggested_lr.valley
+        self.analysis.learn.fit_one_cycle(epochs_max, lr_max=suggested_lr.valley)
+        self.epochs_trained_ = self.analysis.learn.epoch + 1
+        N_train_notna = X.notna().sum().sum()
+        N_val_notna = None
+        if y is not None:
+            N_val_notna = y.notna().sum().sum()
+        self.fig_loss_ = models.plot_training_losses(
+            self.analysis.learn, self.model_name,
+            folder=self.out_folder,
+            norm_factors=[N_train_notna, N_val_notna])
+        return self
+
+    def transform(self, X):
+        """ A reference implementation of a transform function.
+
+        Parameters
+        ----------
+        X : {array-like, sparse-matrix}, shape (n_samples, n_features)
+            The input samples.
+
+        Returns
+        -------
+        X_transformed : array, shape (n_samples, n_features)
+            The array containing the element-wise square roots of the values
+            in ``X``.
+        """
+        # Check is fit had been called
+        check_is_fitted(self, 'epochs_trained_')
+
+        self.analysis.model.eval()
+
+        pred, target = ae.get_preds_from_df(
+            df=X,
+            learn=self.analysis.learn,
+            position_pred_tuple=0,
+            transformer=self.analysis.transform)
+        return X.fillna(pred)
```

### Comparing `pimms-learn-0.2.0/vaep/sklearn/cf_transformer.py` & `pimms_learn-0.3.0/vaep/sklearn/cf_transformer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,179 +1,185 @@
-"""Scikit-learn style interface for Collaborative Filtering model."""
-from __future__ import annotations
-
-from pathlib import Path
-
-from fastai.tabular.all import *
-from fastai.collab import *
-
-from fastai import learner
-
-import pandas as pd
-
-from sklearn.utils.validation import check_is_fitted
-from sklearn.base import BaseEstimator, TransformerMixin
-
-import vaep
-from vaep.models import collab
-import vaep.models as models
-
-
-# patch plotting function
-from vaep.models import plot_loss
-learner.Recorder.plot_loss = plot_loss
-
-
-class CollaborativeFilteringTransformer(TransformerMixin, BaseEstimator):
-    """Collaborative Filtering transformer.
-
-
-    Parameters
-    ----------
-    demo_param : str, default='demo'
-        A parameter used for demonstation of how to pass and store paramters.
-
-    Attributes
-    ----------
-    n_features_ : int
-        The number of features of the data passed to :meth:`fit`.
-    """
-
-    def __init__(self,
-                 target_column: str,
-                 sample_column: str,
-                 item_column: str,
-                 n_factors: int = 15,
-                 out_folder: str = '.',
-                 #  y_range:Optional[tuple[int]]=None,
-                 batch_size: int = 4096,
-                 ):
-        self.target_column = target_column
-        self.item_column = item_column
-        self.sample_column = sample_column
-        self.n_factors = n_factors
-        self.out_folder = Path(out_folder)
-        self.batch_size = batch_size
-
-    def fit(self, X: pd.Series, y: pd.Series = None,
-            cuda: bool = True,
-            patience: int = 1,
-            epochs_max=20,):
-        """A reference implementation of a fitting function for a transformer.
-
-        Parameters
-        ----------
-        X : {array-like, sparse matrix}, shape (n_samples, n_features)
-            The training input samples.
-        y : None
-            There is no need of a target in a transformer, yet the pipeline API
-            requires this parameter.
-
-        Returns
-        -------
-        self : object
-            Returns self.
-        """
-        # ! X = check_array(X, accept_sparse=True)
-        self.model_kwargs = dict(
-
-
-            n_factors=self.n_factors,
-            y_range=(int(X.squeeze().min()),
-                     int(X.squeeze().max()) + 1)
-        )
-
-        if y is not None:
-            X, frac = collab.combine_data(X, y)
-        else:
-            X, frac = X.reset_index(), 0.0
-
-        self.dls = CollabDataLoaders.from_df(
-            X,
-            valid_pct=frac,
-            seed=42,
-            user_name=self.sample_column,
-            item_name=self.item_column,
-            rating_name=self.target_column,
-            bs=self.batch_size)
-        splits = None
-        if y is not None:
-            idx_splitter = IndexSplitter(list(range(len(X), len(X) + len(y))))
-            splits = idx_splitter(X)
-
-        self.cat_names = [self.sample_column, self.item_column]
-        self.to = TabularCollab(df=X,
-                                procs=[Categorify],
-                                cat_names=self.cat_names,
-                                y_names=[self.target_column],
-                                y_block=TransformBlock(),
-                                splits=splits)
-        self.dls = self.to.dataloaders(path='.', bs=self.batch_size)
-
-        self.model = EmbeddingDotBias.from_classes(
-            classes=self.dls.classes,
-            **self.model_kwargs)
-
-        self.n_params = models.calc_net_weight_count(self.model)
-        # ana_collab.params['n_parameters'] = args.n_params
-        self.learn = Learner(dls=self.dls,
-                             model=self.model,
-                             loss_func=MSELossFlat(),
-                             cbs=EarlyStoppingCallback(patience=patience) if y is not None else None,
-                             model_dir=self.out_folder)
-        if cuda:
-            self.learn.model = self.learn.model.cuda()
-
-        #
-        suggested_lr = self.learn.lr_find()
-        print(f"{suggested_lr.valley = :.5f}")
-
-        self.learn.fit_one_cycle(epochs_max,
-
-                                 lr_max=suggested_lr.valley)
-        self.plot_loss(y)
-        self.epochs_trained_ = self.learn.epoch + 1
-        self.model_kwargs['suggested_inital_lr'] = suggested_lr.valley
-        # ? own method?
-        # self.learn.save('collab_model')
-
-        return self
-
-    def transform(self, X):
-        """ A reference implementation of a transform function.
-
-        Parameters
-        ----------
-        X : {array-like, sparse-matrix}, shape (n_samples, n_features)
-            The input samples.
-
-        Returns
-        -------
-        X_transformed : array, shape (n_samples, n_features)
-            The array containing the element-wise square roots of the values
-            in ``X``.
-        """
-        # Check is fit had been called
-        check_is_fitted(self, 'epochs_trained_')
-
-        # ! Input validation
-        # X = check_array(X, accept_sparse=True)
-
-        X = X.squeeze()
-        mask = X.unstack().isna().stack()
-        idx_na = mask.loc[mask].index
-        dl_real_na = self.dls.test_dl(idx_na.to_frame())
-        pred_na, _ = self.learn.get_preds(dl=dl_real_na)
-        pred_na = pd.Series(pred_na, idx_na, name=self.target_column)
-        return pd.concat([X, pred_na])
-
-    def plot_loss(self, y, figsize=(8, 4)):  # -> Axes:
-        fig, ax = plt.subplots(figsize=figsize)
-        ax.set_title('CF loss: Reconstruction loss')
-        self.learn.recorder.plot_loss(skip_start=5, ax=ax,
-                                      with_valid=True if y is not None else False)
-        vaep.savefig(fig, name='collab_training',
-                     folder=self.out_folder)
-        self.model_kwargs['batch_size'] = self.batch_size
-        vaep.io.dump_json(self.model_kwargs, self.out_folder /
-                          'model_params_{}.json'.format('CF'))
-        return ax
+"""Scikit-learn style interface for Collaborative Filtering model."""
+from __future__ import annotations
+
+from pathlib import Path
+
+import matplotlib.pyplot as plt
+import pandas as pd
+from fastai import learner
+from fastai.callback.tracker import EarlyStoppingCallback
+from fastai.collab import *
+from fastai.collab import CollabDataLoaders, EmbeddingDotBias, TabularCollab
+from fastai.data.block import TransformBlock
+from fastai.data.transforms import IndexSplitter
+from fastai.learner import Learner
+from fastai.losses import MSELossFlat
+from fastai.tabular.all import *
+from fastai.tabular.core import Categorify
+from fastai.torch_core import default_device
+from sklearn.base import BaseEstimator, TransformerMixin
+from sklearn.utils.validation import check_is_fitted
+
+import vaep
+import vaep.models as models
+# patch plotting function
+from vaep.models import collab, plot_loss
+
+learner.Recorder.plot_loss = plot_loss
+
+
+class CollaborativeFilteringTransformer(TransformerMixin, BaseEstimator):
+    """Collaborative Filtering transformer.
+
+
+    Parameters
+    ----------
+    demo_param : str, default='demo'
+        A parameter used for demonstation of how to pass and store paramters.
+
+    Attributes
+    ----------
+    n_features_ : int
+        The number of features of the data passed to :meth:`fit`.
+    """
+
+    def __init__(self,
+                 target_column: str,
+                 sample_column: str,
+                 item_column: str,
+                 n_factors: int = 15,
+                 out_folder: str = '.',
+                 #  y_range:Optional[tuple[int]]=None,
+                 batch_size: int = 4096,
+                 ):
+        self.target_column = target_column
+        self.item_column = item_column
+        self.sample_column = sample_column
+        self.n_factors = n_factors
+        self.out_folder = Path(out_folder)
+        self.out_folder.mkdir(exist_ok=True, parents=True)
+        self.batch_size = batch_size
+
+    def fit(self, X: pd.Series, y: pd.Series = None,
+            cuda: bool = True,
+            patience: int = 1,
+            epochs_max=20,):
+        """A reference implementation of a fitting function for a transformer.
+
+        Parameters
+        ----------
+        X : {array-like, sparse matrix}, shape (n_samples, n_features)
+            The training input samples.
+        y : None
+            There is no need of a target in a transformer, yet the pipeline API
+            requires this parameter.
+
+        Returns
+        -------
+        self : object
+            Returns self.
+        """
+        # ! X = check_array(X, accept_sparse=True)
+        self.model_kwargs = dict(
+
+
+            n_factors=self.n_factors,
+            y_range=(int(X.squeeze().min()),
+                     int(X.squeeze().max()) + 1)
+        )
+        if not cuda:
+            default_device(use=False)  # set to cpu
+        if y is not None:
+            X, frac = collab.combine_data(X, y)
+        else:
+            X, frac = X.reset_index(), 0.0
+
+        self.dls = CollabDataLoaders.from_df(
+            X,
+            valid_pct=frac,
+            seed=42,
+            user_name=self.sample_column,
+            item_name=self.item_column,
+            rating_name=self.target_column,
+            bs=self.batch_size)
+        splits = None
+        if y is not None:
+            idx_splitter = IndexSplitter(list(range(len(X), len(X) + len(y))))
+            splits = idx_splitter(X)
+
+        self.cat_names = [self.sample_column, self.item_column]
+        self.to = TabularCollab(df=X,
+                                procs=[Categorify],
+                                cat_names=self.cat_names,
+                                y_names=[self.target_column],
+                                y_block=TransformBlock(),
+                                splits=splits)
+        self.dls = self.to.dataloaders(path='.', bs=self.batch_size)
+
+        self.model = EmbeddingDotBias.from_classes(
+            classes=self.dls.classes,
+            **self.model_kwargs)
+
+        self.n_params = models.calc_net_weight_count(self.model)
+        # ana_collab.params['n_parameters'] = args.n_params
+        self.learn = Learner(dls=self.dls,
+                             model=self.model,
+                             loss_func=MSELossFlat(),
+                             cbs=EarlyStoppingCallback(patience=patience) if y is not None else None,
+                             model_dir=self.out_folder)
+        if cuda:
+            self.learn.model = self.learn.model.cuda()
+
+        #
+        suggested_lr = self.learn.lr_find()
+        print(f"{suggested_lr.valley = :.5f}")
+
+        self.learn.fit_one_cycle(epochs_max,
+
+                                 lr_max=suggested_lr.valley)
+        self.plot_loss(y)
+        self.epochs_trained_ = self.learn.epoch + 1
+        self.model_kwargs['suggested_inital_lr'] = suggested_lr.valley
+        # ? own method?
+        # self.learn.save('collab_model')
+
+        return self
+
+    def transform(self, X):
+        """ A reference implementation of a transform function.
+
+        Parameters
+        ----------
+        X : {array-like, sparse-matrix}, shape (n_samples, n_features)
+            The input samples.
+
+        Returns
+        -------
+        X_transformed : array, shape (n_samples, n_features)
+            The array containing the element-wise square roots of the values
+            in ``X``.
+        """
+        # Check is fit had been called
+        check_is_fitted(self, 'epochs_trained_')
+
+        # ! Input validation
+        # X = check_array(X, accept_sparse=True)
+
+        X = X.squeeze()
+        mask = X.unstack().isna().stack()
+        idx_na = mask.loc[mask].index
+        dl_real_na = self.dls.test_dl(idx_na.to_frame())
+        pred_na, _ = self.learn.get_preds(dl=dl_real_na)
+        pred_na = pd.Series(pred_na, idx_na, name=self.target_column)
+        return pd.concat([X, pred_na])
+
+    def plot_loss(self, y, figsize=(8, 4)):  # -> Axes:
+        fig, ax = plt.subplots(figsize=figsize)
+        ax.set_title('CF loss: Reconstruction loss')
+        self.learn.recorder.plot_loss(skip_start=5, ax=ax,
+                                      with_valid=True if y is not None else False)
+        vaep.savefig(fig, name='collab_training',
+                     folder=self.out_folder)
+        self.model_kwargs['batch_size'] = self.batch_size
+        vaep.io.dump_json(self.model_kwargs,
+                          self.out_folder / 'model_params_{}.json'.format('CF'))
+        return ax
```

