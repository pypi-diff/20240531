# Comparing `tmp/stereopy-1.2.0.tar.gz` & `tmp/stereopy-1.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stereopy-1.2.0.tar", last modified: Fri Mar 29 09:07:22 2024, max compression
+gzip compressed data, was "stereopy-1.3.0b1.tar", last modified: Fri May 31 02:46:05 2024, max compression
```

## Comparing `stereopy-1.2.0.tar` & `stereopy-1.3.0b1.tar`

### file list

```diff
@@ -1,413 +1,426 @@
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.343959 stereopy-1.2.0/
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.242957 stereopy-1.2.0/.github/
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.257957 stereopy-1.2.0/.github/workflows/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1625 2024-03-25 07:06:26.000000 stereopy-1.2.0/.github/workflows/main.yml
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2935 2024-03-25 07:06:26.000000 stereopy-1.2.0/.github/workflows/pytest_conda_linux.yml
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      347 2024-03-25 07:06:26.000000 stereopy-1.2.0/.github/workflows/pytest_conda_linux_demo.yml
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1338 2024-03-25 07:06:26.000000 stereopy-1.2.0/.github/workflows/pytest_conda_linux_dev.yml
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      971 2024-03-25 07:06:26.000000 stereopy-1.2.0/.github/workflows/pytest_conda_linux_gpu.yml
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2158 2024-03-25 07:06:26.000000 stereopy-1.2.0/.github/workflows/pytest_conda_linux_image.yml
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      707 2023-09-14 03:30:39.000000 stereopy-1.2.0/.github/workflows/pytest_conda_win.yml
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1901 2024-03-25 07:06:26.000000 stereopy-1.2.0/.gitignore
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      433 2023-11-06 07:35:44.000000 stereopy-1.2.0/.readthedocs.yml
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1094 2023-09-14 03:30:39.000000 stereopy-1.2.0/LICENSE
--rw-r--r--   0 tanliwei  (1010) tanliwei  (1010)     4949 2024-03-29 09:07:22.342959 stereopy-1.2.0/PKG-INFO
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2072 2023-09-19 06:51:34.000000 stereopy-1.2.0/README.md
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       94 2023-09-14 03:30:44.000000 stereopy-1.2.0/pyproject.toml
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)  6652017 2023-09-14 03:30:44.000000 stereopy-1.2.0/quick_start.ipynb
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1870 2024-03-25 07:06:27.000000 stereopy-1.2.0/requirements.txt
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      359 2024-03-25 07:06:27.000000 stereopy-1.2.0/requirements_for_image.txt
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      223 2024-03-25 07:06:27.000000 stereopy-1.2.0/requirements_for_image_cu11x.txt
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      308 2024-03-25 07:06:27.000000 stereopy-1.2.0/requirements_for_image_cu12x.txt
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      185 2023-12-04 09:57:50.000000 stereopy-1.2.0/requirements_for_spatialign.txt
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       38 2024-03-29 09:07:22.343959 stereopy-1.2.0/setup.cfg
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2063 2023-12-04 09:57:50.000000 stereopy-1.2.0/setup.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.258957 stereopy-1.2.0/stereo/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      225 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/__init__.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.262957 stereopy-1.2.0/stereo/algorithm/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      195 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6297 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/_louvain.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4854 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/algorithm_base.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      210 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/algorithm/algorithm_err_code.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.263957 stereopy-1.2.0/stereo/algorithm/batch_qc/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       86 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     9977 2024-01-16 10:06:19.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/batchqc_raw.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2274 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/main.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.263957 stereopy-1.2.0/stereo/algorithm/batch_qc/module/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      345 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/module/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     7308 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/module/classifier.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      717 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/module/dataset.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      990 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/module/early_stop.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1032 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/module/loss.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1402 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/module/trainer.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      505 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/plot_batch_qc.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.264958 stereopy-1.2.0/stereo/algorithm/batch_qc/score/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      320 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/score/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1467 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/score/get_neighbors.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3522 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/score/kbet.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2393 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/score/ksim.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2717 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/score/lisi.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.264958 stereopy-1.2.0/stereo/algorithm/batch_qc/template/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      183 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/template/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1848 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/template/report_template_adjust.html
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2721 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/template/report_template_raw.html
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.266957 stereopy-1.2.0/stereo/algorithm/batch_qc/test/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      662 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/test/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2057 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/test/cdf_plot.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3053 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/test/describe_data.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1510 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/test/distribution_fitting.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1274 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/test/heatmap.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      748 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/test/joint_plot.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      814 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/test/kernel_plot.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2856 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/test/metric_score.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1629 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/test/pca_regression.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4146 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/test/qq_plot.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1172 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/test/umap_plot.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1149 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/test/var_mean_plot.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2155 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/test/variance_test.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.267958 stereopy-1.2.0/stereo/algorithm/batch_qc/utils/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      434 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/utils/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      615 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/utils/check_data.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      543 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/utils/generate_palette.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     5668 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/utils/html_utils.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1302 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/utils/pca_lowrank.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      652 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/batch_qc/utils/print_time.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.267958 stereopy-1.2.0/stereo/algorithm/ccd/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      301 2023-11-06 07:35:44.000000 stereopy-1.2.0/stereo/algorithm/ccd/__init__.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.268957 stereopy-1.2.0/stereo/algorithm/ccd/assets/
--rwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)    15086 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/algorithm/ccd/assets/favicon.ico
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    38801 2024-01-16 10:06:19.000000 stereopy-1.2.0/stereo/algorithm/ccd/community_clustering_algorithm.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3727 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/ccd/constants.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    20626 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/ccd/html_report.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4547 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/ccd/metrics.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    18171 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/algorithm/ccd/sliding_window.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3340 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/algorithm/ccd/utils.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.269958 stereopy-1.2.0/stereo/algorithm/cell_cell_communication/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      103 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/cell_cell_communication/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4273 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/cell_cell_communication/analysis_helper.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2531 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/cell_cell_communication/exceptions.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    62914 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/algorithm/cell_cell_communication/main.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    26665 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/algorithm/cell_cell_communication/plot_ccc.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    17475 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/cell_cell_communication/spatial_scoloc.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.269958 stereopy-1.2.0/stereo/algorithm/cell_cell_communication/utils/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      135 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/algorithm/cell_cell_communication/utils/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6972 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/cell_cell_communication/utils/database_utils.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3533 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/cell_cell_communication/utils/sqlalchemy_model.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    20063 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/cell_cell_communication/utils/sqlalchemy_repository.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     7241 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/cell_cell_communication/utils/visualization_process.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8952 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/cell_correction.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6514 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/cell_correction_fast.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    10614 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/cell_correction_fast_by_mask.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.271957 stereopy-1.2.0/stereo/algorithm/cell_pose/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      631 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/algorithm/cell_pose/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6183 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/algorithm/cell_pose/cell_pose.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    41529 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/algorithm/cell_pose/core.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    26416 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/algorithm/cell_pose/dynamics.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    21312 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/algorithm/cell_pose/io.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    10895 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/cell_pose/metrics.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    49055 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/algorithm/cell_pose/models.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8657 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/cell_pose/plot.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8903 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/cell_pose/resnet_torch.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    44168 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/algorithm/cell_pose/utils.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      516 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/cell_pose/version.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    15150 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/algorithm/co_occurrence.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    44668 2024-01-16 10:06:19.000000 stereopy-1.2.0/stereo/algorithm/community_detection.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     5464 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/dendrogram.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6785 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/dim_reduce.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.271957 stereopy-1.2.0/stereo/algorithm/dpt/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       58 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/dpt/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    45356 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/dpt/main.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    11591 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/dpt/pca.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    34168 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/dpt/struct.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6174 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/draw_contours.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     5420 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/gaussian_smooth.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     7257 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/gen_ccc_micro_envs.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    60202 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/gen_mesh.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3957 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/algorithm/get_niche.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     9862 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/highly_variable_genes.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4631 2024-01-16 10:06:19.000000 stereopy-1.2.0/stereo/algorithm/leiden.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2984 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/log1p_fake.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    10293 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/mannwhitneyu.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1014 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/ms_algorithm_base.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      543 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/algorithm/ms_community_detection.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      347 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/algorithm/ms_log1p_fake.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    15281 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/neighbors.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3071 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/normalization.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    13075 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/paga.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.272958 stereopy-1.2.0/stereo/algorithm/paste/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       90 2023-11-06 07:35:44.000000 stereopy-1.2.0/stereo/algorithm/paste/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    12207 2023-11-06 07:35:44.000000 stereopy-1.2.0/stereo/algorithm/paste/helper.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    16543 2023-11-06 07:35:44.000000 stereopy-1.2.0/stereo/algorithm/paste/methods.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2915 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/algorithm/paste/paste.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      437 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/phenograph.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.272958 stereopy-1.2.0/stereo/algorithm/regulatory_network_inference/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      104 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/regulatory_network_inference/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    24409 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/algorithm/regulatory_network_inference/main.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    29321 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/algorithm/regulatory_network_inference/plot_grn.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3330 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/scale.py
--rwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)     2876 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/scenic.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.273958 stereopy-1.2.0/stereo/algorithm/sctransform/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      410 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/sctransform/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     9426 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/sctransform/bw.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3700 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/sctransform/ksmooth.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     5818 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/sctransform/plotting.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2153 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/algorithm/sctransform/scale_data.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8371 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/sctransform/sctransform.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     7313 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/sctransform/utils.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    14651 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/sctransform/vst.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.274958 stereopy-1.2.0/stereo/algorithm/single_r/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      166 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/single_r/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    18413 2024-03-29 06:19:46.000000 stereopy-1.2.0/stereo/algorithm/single_r/single_r.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2076 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/algorithm/single_r/utils.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3382 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/algorithm/spatial_hotspot.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2531 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/spatial_pattern_score.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3130 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/statistics.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    13538 2024-03-29 08:14:51.000000 stereopy-1.2.0/stereo/algorithm/time_series_analysis.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    12094 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/algorithm/total_vi.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6498 2023-11-06 07:35:44.000000 stereopy-1.2.0/stereo/algorithm/umap.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      179 2024-03-29 08:59:59.000000 stereopy-1.2.0/stereo/common.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2151 2023-11-06 07:35:44.000000 stereopy-1.2.0/stereo/constant.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.276958 stereopy-1.2.0/stereo/core/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      247 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/core/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    10459 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/core/cell.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      335 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/core/constants.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4158 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/core/data.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     5924 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/core/gene.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    30215 2024-01-16 10:06:19.000000 stereopy-1.2.0/stereo/core/ms_data.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     9761 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/core/ms_pipeline.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    23547 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/core/result.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    73460 2024-03-29 06:19:46.000000 stereopy-1.2.0/stereo/core/st_pipeline.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    24639 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/core/stereo_exp_data.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     5070 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/core/tool_base.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.244957 stereopy-1.2.0/stereo/data/
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.244957 stereopy-1.2.0/stereo/data/algorithm/
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.244957 stereopy-1.2.0/stereo/data/algorithm/cell_cell_communication/
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.278958 stereopy-1.2.0/stereo/data/algorithm/cell_cell_communication/database/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)   442368 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/data/algorithm/cell_cell_communication/database/cellphonedb.db
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)   364544 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/data/algorithm/cell_cell_communication/database/celltalkdb.db
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)   737280 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/data/algorithm/cell_cell_communication/database/liana.db
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)   395756 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/data/algorithm/cell_cell_communication/database/mouse2human.csv
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.279958 stereopy-1.2.0/stereo/image/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      945 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/image/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4529 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/image/pyramid.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.280958 stereopy-1.2.0/stereo/image/segmentation/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       96 2023-11-06 07:35:44.000000 stereopy-1.2.0/stereo/image/segmentation/__init__.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.245957 stereopy-1.2.0/stereo/image/segmentation/seg_utils/
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.280958 stereopy-1.2.0/stereo/image/segmentation/seg_utils/base_cell_seg_pipe/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)        0 2023-11-06 07:35:44.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/base_cell_seg_pipe/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8231 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/base_cell_seg_pipe/cell_seg_pipeline.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8849 2023-11-06 07:35:44.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/base_cell_seg_pipe/find_maxima.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     5068 2023-11-06 07:35:44.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/base_cell_seg_pipe/grade.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.281958 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       94 2023-11-06 07:35:44.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    14589 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1/cell_infer.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6499 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1/cell_seg_pipeline_v1.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      726 2023-11-06 07:35:44.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1/dataset.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1628 2023-11-06 07:35:44.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1/image.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.282958 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1/models/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      656 2023-11-06 07:35:44.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1/models/SE_weight_module.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       31 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1/models/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    22796 2023-11-06 07:35:44.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1/models/epsanet.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8092 2023-11-06 07:35:44.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1/resnet_unet.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3461 2023-11-06 07:35:44.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1/tissue_seg.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2432 2023-11-06 07:35:44.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1/tissue_seg_pipeline.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    22157 2023-11-06 07:35:44.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1/utils.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.283958 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      105 2023-11-06 07:35:44.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4986 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/cell_infer.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4332 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/cell_seg_pipeline_v1_pro.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2272 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/dataset.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8461 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/find_maxima.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6021 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/grade.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1591 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/image.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.284958 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/models/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      656 2023-11-06 07:35:44.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/models/SE_weight_module.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       31 2023-11-06 07:35:44.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/models/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    16505 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/models/epsanet.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8149 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/resnet_unet.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2956 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/tissue_seg.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2456 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/tissue_seg_pipeline.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    23824 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/utils.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.284958 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v3/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       94 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v3/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2360 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/image/segmentation/seg_utils/v3/cell_seg_pipeline_v3.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4093 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/image/segmentation/segment.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.284958 stereopy-1.2.0/stereo/image/segmentation_deepcell/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)        0 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/image/segmentation_deepcell/__init__.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.285958 stereopy-1.2.0/stereo/image/segmentation_deepcell/seg_utils/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)        0 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/image/segmentation_deepcell/seg_utils/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    13919 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/image/segmentation_deepcell/seg_utils/cell_infer.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    13433 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/image/segmentation_deepcell/seg_utils/cell_seg_pipeline.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8539 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/image/segmentation_deepcell/seg_utils/find_maxima.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     5068 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/image/segmentation_deepcell/seg_utils/grade.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1621 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/image/segmentation_deepcell/seg_utils/image.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3244 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/image/segmentation_deepcell/seg_utils/tissue_seg.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2431 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/image/segmentation_deepcell/seg_utils/tissue_seg_pipeline.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    21264 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/image/segmentation_deepcell/seg_utils/utils.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2439 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/image/segmentation_deepcell/segment.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.286958 stereopy-1.2.0/stereo/image/tissue_cut/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       70 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/image/tissue_cut/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     9513 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/image/tissue_cut/pipeline.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.286958 stereopy-1.2.0/stereo/image/tissue_cut/tissue_cut_utils/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      130 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/image/tissue_cut/tissue_cut_utils/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6853 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/image/tissue_cut/tissue_cut_utils/tissue_seg_bcdu.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8165 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/image/tissue_cut/tissue_cut_utils/tissue_seg_bcdu_model.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1723 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/image/tissue_cut/tissue_cut_utils/tissue_seg_bcdu_uity.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    12576 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/image/tissue_cut/tissue_cut_utils/tissue_seg_net.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2911 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/image/tissue_cut/tissue_cut_utils/tissue_seg_utils.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.287958 stereopy-1.2.0/stereo/image/x2tif/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       73 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/image/x2tif/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4560 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/image/x2tif/x2tif.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.287958 stereopy-1.2.0/stereo/io/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      478 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/io/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    13255 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/io/h5ad.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    61004 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/io/reader.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4481 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/io/utils.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    17522 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/io/writer.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3836 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/log_manager.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.290958 stereopy-1.2.0/stereo/plots/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1338 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/plots/__init__.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.291958 stereopy-1.2.0/stereo/plots/_plot_basic/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      151 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/plots/_plot_basic/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1427 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/plots/_plot_basic/get_stereo_data.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    11860 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/plots/_plot_basic/heatmap_plt.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     9828 2024-01-16 10:06:19.000000 stereopy-1.2.0/stereo/plots/decorator.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.291958 stereopy-1.2.0/stereo/plots/interact_plot/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      197 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/plots/interact_plot/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4426 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/plots/interact_plot/annotation_cluster.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    10112 2024-01-16 10:06:19.000000 stereopy-1.2.0/stereo/plots/interact_plot/interactive_scatter.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    13533 2024-01-16 10:06:19.000000 stereopy-1.2.0/stereo/plots/interact_plot/poly_selection.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3275 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/plots/interact_plot/spatial_cluster.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    25182 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/plots/marker_genes.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     7652 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/plots/ms_plot.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1095 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/plots/ms_plot_base.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1280 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/plots/plot_base.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    19165 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/plots/plot_ccd.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    16725 2024-01-17 08:27:31.000000 stereopy-1.2.0/stereo/plots/plot_cells.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.292958 stereopy-1.2.0/stereo/plots/plot_cluster_traj/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       55 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/plots/plot_cluster_traj/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2858 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/plots/plot_cluster_traj/interp.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4094 2024-01-16 10:06:19.000000 stereopy-1.2.0/stereo/plots/plot_cluster_traj/plot_cluster_traj.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    20628 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/plots/plot_cluster_traj/traj.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.292958 stereopy-1.2.0/stereo/plots/plot_cluster_traj_3d/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       59 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/plots/plot_cluster_traj_3d/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3285 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/plots/plot_cluster_traj_3d/interp.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4830 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/plots/plot_cluster_traj_3d/plot_cluster_traj_3d.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    13057 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/plots/plot_cluster_traj_3d/traj.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     7401 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/plots/plot_clusters_heatmap.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     9976 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/plots/plot_clusters_scatter.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    55630 2024-01-17 03:17:26.000000 stereopy-1.2.0/stereo/plots/plot_collection.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4376 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/plots/plot_coo.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4253 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/plots/plot_dendrogram.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3038 2024-01-16 10:06:19.000000 stereopy-1.2.0/stereo/plots/plot_elbow.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     5232 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/plots/plot_genes_in_pseudotime.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    18297 2024-03-26 07:06:32.000000 stereopy-1.2.0/stereo/plots/plot_paga.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    39054 2024-01-16 10:06:19.000000 stereopy-1.2.0/stereo/plots/plot_time_series.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.293958 stereopy-1.2.0/stereo/plots/plot_vec/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       38 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/plots/plot_vec/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     5129 2024-01-16 10:06:19.000000 stereopy-1.2.0/stereo/plots/plot_vec/plot_vec.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    13707 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/plots/plot_vec/vec.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.293958 stereopy-1.2.0/stereo/plots/plot_vec_3d/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       43 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/plots/plot_vec_3d/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3134 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/plots/plot_vec_3d/plot_vec_3d.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    10105 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/plots/plot_vec_3d/vec.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    20940 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/plots/scatter.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    14312 2024-01-16 10:06:19.000000 stereopy-1.2.0/stereo/plots/violin.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.294958 stereopy-1.2.0/stereo/plots/vt3d_browser/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    22029 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/plots/vt3d_browser/PAGA_traj.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1086 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/plots/vt3d_browser/README.md
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      117 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/plots/vt3d_browser/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2650 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/plots/vt3d_browser/example.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.296958 stereopy-1.2.0/stereo/plots/vt3d_browser/examples/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)   233887 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/plots/vt3d_browser/examples/example_ccc.ipynb
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)   507177 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/plots/vt3d_browser/examples/example_grn.ipynb
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)   397934 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/plots/vt3d_browser/examples/example_mesh.ipynb
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)   115622 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/plots/vt3d_browser/examples/example_paga.ipynb
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    28322 2023-11-06 07:35:44.000000 stereopy-1.2.0/stereo/plots/vt3d_browser/stereopy_3D_browser.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.322959 stereopy-1.2.0/stereo/plots/vt3d_browser/vt3d_browser/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    28200 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/plots/vt3d_browser/vt3d_browser/535877f50039c0cb49a6196a5b7517cd.woff
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    11040 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/plots/vt3d_browser/vt3d_browser/6f0a76321d30f3c8120915e57f7bd77e.ttf
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    55956 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/plots/vt3d_browser/vt3d_browser/732389ded34cb9c52dd88271f1345af9.ttf
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      384 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/plots/vt3d_browser/vt3d_browser/index.html
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)  7362871 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/plots/vt3d_browser/vt3d_browser/index.js
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)  8129245 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/plots/vt3d_browser/vt3d_browser/index.js.map
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       16 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/plots/vt3d_browser/vt3d_browser/index1.html
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1497 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/plots/vt3d_browser/vt3d_browser/manifest.js
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    14640 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/plots/vt3d_browser/vt3d_browser/manifest.js.map
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)   890282 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/plots/vt3d_browser/vt3d_browser/vendor.js
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)  6646820 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/plots/vt3d_browser/vt3d_browser/vendor.js.map
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.332959 stereopy-1.2.0/stereo/preprocess/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      274 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/preprocess/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6385 2024-01-16 10:06:19.000000 stereopy-1.2.0/stereo/preprocess/filter.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1910 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/preprocess/normalize.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2975 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/preprocess/qc.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1335 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/preprocess/sc_transform.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.332959 stereopy-1.2.0/stereo/scripts/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)        0 2023-09-14 03:30:44.000000 stereopy-1.2.0/stereo/scripts/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     7872 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/scripts/ccd.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6805 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/stereo_config.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.335959 stereopy-1.2.0/stereo/tools/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    16063 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/tools/LR_interaction.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      471 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/tools/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     7325 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/tools/boundary.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    13269 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/tools/cell_correct.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4330 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/tools/cell_cut.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3070 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/tools/cell_segment.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    14777 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/tools/cell_type_anno.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     7431 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/tools/cluster.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     7026 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/tools/clustering.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     5333 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/tools/dim_reduce.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    15176 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/tools/find_markers.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3246 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/tools/gem_filter.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8304 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/tools/highly_variable_genes.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    13813 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/tools/rna_velocity.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4941 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/tools/spatial_lag.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      997 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/tools/spatial_pattern_score.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4841 2024-03-29 06:19:46.000000 stereopy-1.2.0/stereo/tools/tissue_extraction.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      491 2023-12-04 09:57:50.000000 stereopy-1.2.0/stereo/tools/tools.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.336959 stereopy-1.2.0/stereo/utils/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      491 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/utils/__init__.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2585 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/utils/_download.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1632 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/utils/correlation.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    16780 2024-01-16 10:06:19.000000 stereopy-1.2.0/stereo/utils/data_helper.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     7884 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/utils/hvg_utils.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     9874 2024-03-25 07:06:27.000000 stereopy-1.2.0/stereo/utils/pipeline_utils.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1411 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/utils/read_write_utils.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      868 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/utils/spmatrix_helper.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1963 2023-10-20 06:18:33.000000 stereopy-1.2.0/stereo/utils/time_consume.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.340959 stereopy-1.2.0/stereopy.egg-info/
--rw-r--r--   0 tanliwei  (1010) tanliwei  (1010)     4949 2024-03-29 09:07:18.000000 stereopy-1.2.0/stereopy.egg-info/PKG-INFO
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    13979 2024-03-29 09:07:22.000000 stereopy-1.2.0/stereopy.egg-info/SOURCES.txt
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)        1 2024-03-29 09:07:18.000000 stereopy-1.2.0/stereopy.egg-info/dependency_links.txt
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       48 2024-03-29 09:07:18.000000 stereopy-1.2.0/stereopy.egg-info/entry_points.txt
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1117 2024-03-29 09:07:18.000000 stereopy-1.2.0/stereopy.egg-info/requires.txt
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)        7 2024-03-29 09:07:18.000000 stereopy-1.2.0/stereopy.egg-info/top_level.txt
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.339959 stereopy-1.2.0/tests/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      102 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/extra_requirements.txt
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       74 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/image_requirements.txt
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      164 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/pytest.ini
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8177 2024-03-25 07:06:27.000000 stereopy-1.2.0/tests/settings.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2199 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/test_batch_integration.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6098 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/test_cell_community_detection.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      749 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/test_cell_cut.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     5923 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/test_clustering.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3179 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/test_h5ad_format.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    13779 2024-03-25 07:06:27.000000 stereopy-1.2.0/tests/test_io.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1663 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/test_io_h5ms.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6477 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/test_marker_genes.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6423 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/test_merge_3d_data.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    10388 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/test_ms_data.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2338 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/test_plot_cluster_traj.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3846 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/test_plot_vec.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3310 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/test_regulatory_network_inference.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2426 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/test_rna_velocity.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6891 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/test_sctransform.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      883 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/test_single_r.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1519 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/test_spatial_hotspot.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1373 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/test_stereo_exp_data.py
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4418 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/test_time_series_analysis.py
-drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-03-29 09:07:22.340959 stereopy-1.2.0/tests/workflows_conf/
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    12332 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/workflows_conf/environment_linux_gpu.yml
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1298 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/workflows_conf/environment_linux_py38.yml
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3948 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/workflows_conf/environment_linux_py39.yml
--rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1774 2023-09-14 03:30:44.000000 stereopy-1.2.0/tests/workflows_conf/environment_win.yml
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:05.083900 stereopy-1.3.0b1/
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:01.548836 stereopy-1.3.0b1/.github/
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:01.912842 stereopy-1.3.0b1/.github/workflows/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1625 2024-03-25 07:06:26.000000 stereopy-1.3.0b1/.github/workflows/main.yml
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2935 2024-03-25 07:06:26.000000 stereopy-1.3.0b1/.github/workflows/pytest_conda_linux.yml
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      348 2024-04-09 01:58:28.000000 stereopy-1.3.0b1/.github/workflows/pytest_conda_linux_demo.yml
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1338 2024-03-25 07:06:26.000000 stereopy-1.3.0b1/.github/workflows/pytest_conda_linux_dev.yml
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      971 2024-03-25 07:06:26.000000 stereopy-1.3.0b1/.github/workflows/pytest_conda_linux_gpu.yml
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2158 2024-03-25 07:06:26.000000 stereopy-1.3.0b1/.github/workflows/pytest_conda_linux_image.yml
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      707 2023-09-14 03:30:39.000000 stereopy-1.3.0b1/.github/workflows/pytest_conda_win.yml
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1901 2024-03-25 07:06:26.000000 stereopy-1.3.0b1/.gitignore
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      433 2023-11-06 07:35:44.000000 stereopy-1.3.0b1/.readthedocs.yml
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1094 2023-09-14 03:30:39.000000 stereopy-1.3.0b1/LICENSE
+-rw-r--r--   0 tanliwei  (1010) tanliwei  (1010)     4949 2024-05-31 02:46:05.082900 stereopy-1.3.0b1/PKG-INFO
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2072 2023-09-19 06:51:34.000000 stereopy-1.3.0b1/README.md
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       94 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/pyproject.toml
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)  6652017 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/quick_start.ipynb
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1868 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/requirements.txt
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      105 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/requirements_for_image.txt
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      223 2024-03-25 07:06:27.000000 stereopy-1.3.0b1/requirements_for_image_cu11x.txt
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      308 2024-03-25 07:06:27.000000 stereopy-1.3.0b1/requirements_for_image_cu12x.txt
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      185 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/requirements_for_spatialign.txt
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       38 2024-05-31 02:46:05.083900 stereopy-1.3.0b1/setup.cfg
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2063 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/setup.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:01.984844 stereopy-1.3.0b1/stereo/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      225 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/__init__.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:02.310850 stereopy-1.3.0b1/stereo/algorithm/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)        1 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/algorithm/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6297 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/_louvain.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4854 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/algorithm_base.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      210 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/algorithm/algorithm_err_code.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:02.401851 stereopy-1.3.0b1/stereo/algorithm/batch_qc/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       41 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     9977 2024-01-16 10:06:19.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/batchqc_raw.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2274 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/main.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:02.504853 stereopy-1.3.0b1/stereo/algorithm/batch_qc/module/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      345 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/module/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     7308 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/module/classifier.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      717 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/module/dataset.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      990 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/module/early_stop.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1032 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/module/loss.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1402 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/module/trainer.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:02.640856 stereopy-1.3.0b1/stereo/algorithm/batch_qc/score/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      320 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/score/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1467 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/score/get_neighbors.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3522 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/score/kbet.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2393 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/score/ksim.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2717 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/score/lisi.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:02.659856 stereopy-1.3.0b1/stereo/algorithm/batch_qc/template/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      183 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/template/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1848 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/template/report_template_adjust.html
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2721 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/template/report_template_raw.html
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:02.755858 stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      662 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2057 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/cdf_plot.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3053 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/describe_data.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1510 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/distribution_fitting.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1274 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/heatmap.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      748 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/joint_plot.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      814 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/kernel_plot.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2856 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/metric_score.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1629 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/pca_regression.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4146 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/qq_plot.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1172 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/umap_plot.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1149 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/var_mean_plot.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2155 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/variance_test.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:02.801859 stereopy-1.3.0b1/stereo/algorithm/batch_qc/utils/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      434 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/utils/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      615 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/utils/check_data.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      543 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/utils/generate_palette.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     5668 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/utils/html_utils.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1302 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/utils/pca_lowrank.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      652 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/batch_qc/utils/print_time.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:02.906860 stereopy-1.3.0b1/stereo/algorithm/ccd/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      301 2023-11-06 07:35:44.000000 stereopy-1.3.0b1/stereo/algorithm/ccd/__init__.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:02.909860 stereopy-1.3.0b1/stereo/algorithm/ccd/assets/
+-rwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)    15086 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/algorithm/ccd/assets/favicon.ico
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    38801 2024-01-16 10:06:19.000000 stereopy-1.3.0b1/stereo/algorithm/ccd/community_clustering_algorithm.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3727 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/ccd/constants.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    20626 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/ccd/html_report.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4547 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/ccd/metrics.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    18171 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/algorithm/ccd/sliding_window.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3340 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/algorithm/ccd/utils.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.014862 stereopy-1.3.0b1/stereo/algorithm/cell_cell_communication/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       55 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/algorithm/cell_cell_communication/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4273 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/cell_cell_communication/analysis_helper.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2531 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/cell_cell_communication/exceptions.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    62914 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/algorithm/cell_cell_communication/main.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    15546 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/algorithm/cell_cell_communication/spatial_scoloc.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.018863 stereopy-1.3.0b1/stereo/algorithm/cell_cell_communication/utils/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      135 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/algorithm/cell_cell_communication/utils/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6972 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/cell_cell_communication/utils/database_utils.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3533 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/cell_cell_communication/utils/sqlalchemy_model.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    20063 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/cell_cell_communication/utils/sqlalchemy_repository.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     7241 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/cell_cell_communication/utils/visualization_process.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8952 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/cell_correction.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6514 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/cell_correction_fast.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    10614 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/cell_correction_fast_by_mask.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.051863 stereopy-1.3.0b1/stereo/algorithm/cell_pose/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      631 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/algorithm/cell_pose/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6183 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/algorithm/cell_pose/cell_pose.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    41529 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/algorithm/cell_pose/core.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    26416 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/algorithm/cell_pose/dynamics.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    21312 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/algorithm/cell_pose/io.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    10895 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/cell_pose/metrics.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    49055 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/algorithm/cell_pose/models.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8657 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/cell_pose/plot.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8903 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/cell_pose/resnet_torch.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    44168 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/algorithm/cell_pose/utils.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      516 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/cell_pose/version.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    15150 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/algorithm/co_occurrence.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    44668 2024-01-16 10:06:19.000000 stereopy-1.3.0b1/stereo/algorithm/community_detection.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     5464 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/dendrogram.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6785 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/dim_reduce.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.060863 stereopy-1.3.0b1/stereo/algorithm/dpt/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       58 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/dpt/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    45356 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/dpt/main.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    11591 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/dpt/pca.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    34168 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/dpt/struct.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6174 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/draw_contours.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     5420 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/gaussian_smooth.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     7466 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/algorithm/gen_ccc_micro_envs.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    60202 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/gen_mesh.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3957 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/algorithm/get_niche.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     9862 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/highly_variable_genes.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4631 2024-01-16 10:06:19.000000 stereopy-1.3.0b1/stereo/algorithm/leiden.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2984 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/log1p_fake.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    10293 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/mannwhitneyu.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1014 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/ms_algorithm_base.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      543 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/algorithm/ms_community_detection.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      347 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/algorithm/ms_log1p_fake.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    15281 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/neighbors.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3071 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/normalization.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    13075 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/paga.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.077864 stereopy-1.3.0b1/stereo/algorithm/paste/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       90 2023-11-06 07:35:44.000000 stereopy-1.3.0b1/stereo/algorithm/paste/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    13429 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/algorithm/paste/helper.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    19511 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/algorithm/paste/methods.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3082 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/algorithm/paste/paste.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      437 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/phenograph.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.078863 stereopy-1.3.0b1/stereo/algorithm/regulatory_network_inference/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       60 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/algorithm/regulatory_network_inference/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    24409 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/algorithm/regulatory_network_inference/main.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3330 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/scale.py
+-rwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)     2876 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/scenic.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.088864 stereopy-1.3.0b1/stereo/algorithm/sctransform/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      410 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/sctransform/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     9426 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/sctransform/bw.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3700 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/sctransform/ksmooth.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     5818 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/sctransform/plotting.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2153 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/algorithm/sctransform/scale_data.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8371 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/sctransform/sctransform.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     7313 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/sctransform/utils.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    14651 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/sctransform/vst.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.091864 stereopy-1.3.0b1/stereo/algorithm/single_r/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      166 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/single_r/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    18413 2024-03-29 06:19:46.000000 stereopy-1.3.0b1/stereo/algorithm/single_r/single_r.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2076 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/algorithm/single_r/utils.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3382 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/algorithm/spatial_hotspot.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2531 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/spatial_pattern_score.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.096864 stereopy-1.3.0b1/stereo/algorithm/st_gears/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       26 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/algorithm/st_gears/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2028 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/algorithm/st_gears/calculate_max_kl.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     5084 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/algorithm/st_gears/granularity_adjusting.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     7161 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/algorithm/st_gears/helper.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     9664 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/algorithm/st_gears/main.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    11222 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/algorithm/st_gears/optim_pot.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    25814 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/algorithm/st_gears/recons.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    15136 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/algorithm/st_gears/regis.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    15506 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/algorithm/st_gears/visual.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4907 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/algorithm/st_gears/weight.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3130 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/algorithm/statistics.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    18860 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/algorithm/time_series_analysis.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    13864 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/algorithm/total_vi.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6498 2023-11-06 07:35:44.000000 stereopy-1.3.0b1/stereo/algorithm/umap.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      181 2024-05-31 02:45:04.000000 stereopy-1.3.0b1/stereo/common.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2151 2023-11-06 07:35:44.000000 stereopy-1.3.0b1/stereo/constant.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.120864 stereopy-1.3.0b1/stereo/core/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      247 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/core/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    11120 2024-05-14 08:11:03.000000 stereopy-1.3.0b1/stereo/core/cell.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      335 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/core/constants.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4229 2024-05-14 08:11:03.000000 stereopy-1.3.0b1/stereo/core/data.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6858 2024-05-14 08:11:03.000000 stereopy-1.3.0b1/stereo/core/gene.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    40871 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/core/ms_data.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    12292 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/core/ms_pipeline.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    24495 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/core/result.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    74685 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/core/st_pipeline.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    25006 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/core/stereo_exp_data.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     5070 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/core/tool_base.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:01.555836 stereopy-1.3.0b1/stereo/data/
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:01.556836 stereopy-1.3.0b1/stereo/data/algorithm/
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:01.556836 stereopy-1.3.0b1/stereo/data/algorithm/cell_cell_communication/
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.128864 stereopy-1.3.0b1/stereo/data/algorithm/cell_cell_communication/database/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)   442368 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/data/algorithm/cell_cell_communication/database/cellphonedb.db
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)   364544 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/data/algorithm/cell_cell_communication/database/celltalkdb.db
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)   737280 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/data/algorithm/cell_cell_communication/database/liana.db
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)   395756 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/data/algorithm/cell_cell_communication/database/mouse2human.csv
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.131865 stereopy-1.3.0b1/stereo/image/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      945 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/image/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4529 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/image/pyramid.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.132865 stereopy-1.3.0b1/stereo/image/segmentation/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       96 2023-11-06 07:35:44.000000 stereopy-1.3.0b1/stereo/image/segmentation/__init__.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:01.573836 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.163865 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/base_cell_seg_pipe/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)        0 2023-11-06 07:35:44.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/base_cell_seg_pipe/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8231 2024-03-25 07:06:27.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/base_cell_seg_pipe/cell_seg_pipeline.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8849 2023-11-06 07:35:44.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/base_cell_seg_pipe/find_maxima.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     5068 2023-11-06 07:35:44.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/base_cell_seg_pipe/grade.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.262867 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       94 2023-11-06 07:35:44.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    14589 2024-03-25 07:06:27.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1/cell_infer.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6499 2024-03-25 07:06:27.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1/cell_seg_pipeline_v1.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      726 2023-11-06 07:35:44.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1/dataset.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1628 2023-11-06 07:35:44.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1/image.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.289867 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1/models/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      656 2023-11-06 07:35:44.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1/models/SE_weight_module.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       31 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1/models/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    22796 2023-11-06 07:35:44.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1/models/epsanet.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8092 2023-11-06 07:35:44.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1/resnet_unet.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3461 2023-11-06 07:35:44.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1/tissue_seg.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2432 2023-11-06 07:35:44.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1/tissue_seg_pipeline.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    22157 2023-11-06 07:35:44.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1/utils.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.358869 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      105 2023-11-06 07:35:44.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4998 2024-05-14 08:11:03.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/cell_infer.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4332 2024-03-25 07:06:27.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/cell_seg_pipeline_v1_pro.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2272 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/dataset.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8461 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/find_maxima.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6021 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/grade.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1591 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/image.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.382869 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/models/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      656 2023-11-06 07:35:44.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/models/SE_weight_module.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       31 2023-11-06 07:35:44.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/models/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    16505 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/models/epsanet.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8149 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/resnet_unet.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2956 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/tissue_seg.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2456 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/tissue_seg_pipeline.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    23824 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/utils.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.391869 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v3/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       94 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v3/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2360 2024-03-25 07:06:27.000000 stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v3/cell_seg_pipeline_v3.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4093 2024-03-25 07:06:27.000000 stereopy-1.3.0b1/stereo/image/segmentation/segment.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.411870 stereopy-1.3.0b1/stereo/image/segmentation_deepcell/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)        0 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/image/segmentation_deepcell/__init__.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.509871 stereopy-1.3.0b1/stereo/image/segmentation_deepcell/seg_utils/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)        0 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/image/segmentation_deepcell/seg_utils/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    13919 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/image/segmentation_deepcell/seg_utils/cell_infer.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    13433 2024-03-25 07:06:27.000000 stereopy-1.3.0b1/stereo/image/segmentation_deepcell/seg_utils/cell_seg_pipeline.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8539 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/image/segmentation_deepcell/seg_utils/find_maxima.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     5068 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/image/segmentation_deepcell/seg_utils/grade.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1621 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/image/segmentation_deepcell/seg_utils/image.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3244 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/image/segmentation_deepcell/seg_utils/tissue_seg.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2431 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/image/segmentation_deepcell/seg_utils/tissue_seg_pipeline.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    21264 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/image/segmentation_deepcell/seg_utils/utils.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2439 2024-03-25 07:06:27.000000 stereopy-1.3.0b1/stereo/image/segmentation_deepcell/segment.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.516872 stereopy-1.3.0b1/stereo/image/tissue_cut/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       70 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/image/tissue_cut/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     9513 2024-03-25 07:06:27.000000 stereopy-1.3.0b1/stereo/image/tissue_cut/pipeline.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.548872 stereopy-1.3.0b1/stereo/image/tissue_cut/tissue_cut_utils/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      130 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/image/tissue_cut/tissue_cut_utils/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6853 2024-03-25 07:06:27.000000 stereopy-1.3.0b1/stereo/image/tissue_cut/tissue_cut_utils/tissue_seg_bcdu.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8165 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/image/tissue_cut/tissue_cut_utils/tissue_seg_bcdu_model.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1723 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/image/tissue_cut/tissue_cut_utils/tissue_seg_bcdu_uity.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    12576 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/image/tissue_cut/tissue_cut_utils/tissue_seg_net.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2911 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/image/tissue_cut/tissue_cut_utils/tissue_seg_utils.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.551872 stereopy-1.3.0b1/stereo/image/x2tif/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       73 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/image/x2tif/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4560 2024-03-25 07:06:27.000000 stereopy-1.3.0b1/stereo/image/x2tif/x2tif.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.591873 stereopy-1.3.0b1/stereo/io/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      478 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/io/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    14817 2024-05-14 08:11:03.000000 stereopy-1.3.0b1/stereo/io/h5ad.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    62546 2024-05-14 08:11:03.000000 stereopy-1.3.0b1/stereo/io/reader.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4867 2024-05-14 08:11:03.000000 stereopy-1.3.0b1/stereo/io/utils.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    18669 2024-05-14 08:11:03.000000 stereopy-1.3.0b1/stereo/io/writer.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3836 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/log_manager.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.802877 stereopy-1.3.0b1/stereo/plots/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1571 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/plots/__init__.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.812877 stereopy-1.3.0b1/stereo/plots/_plot_basic/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      151 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/plots/_plot_basic/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1427 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/plots/_plot_basic/get_stereo_data.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    11860 2024-03-25 07:06:27.000000 stereopy-1.3.0b1/stereo/plots/_plot_basic/heatmap_plt.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     9829 2024-05-14 08:11:03.000000 stereopy-1.3.0b1/stereo/plots/decorator.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.864878 stereopy-1.3.0b1/stereo/plots/interact_plot/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      197 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/plots/interact_plot/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4426 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/plots/interact_plot/annotation_cluster.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    14140 2024-05-14 08:11:03.000000 stereopy-1.3.0b1/stereo/plots/interact_plot/interactive_scatter.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    17730 2024-05-14 08:11:03.000000 stereopy-1.3.0b1/stereo/plots/interact_plot/poly_selection.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3275 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/plots/interact_plot/spatial_cluster.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    25375 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/plots/marker_genes.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     7652 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/plots/ms_plot.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1095 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/plots/ms_plot_base.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1280 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/plots/plot_base.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      505 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/plots/plot_batch_qc.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    26672 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/plots/plot_ccc.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    19165 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/plots/plot_ccd.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    16725 2024-01-17 08:27:31.000000 stereopy-1.3.0b1/stereo/plots/plot_cells.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.865878 stereopy-1.3.0b1/stereo/plots/plot_cluster_traj/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       55 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/plots/plot_cluster_traj/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2858 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/plots/plot_cluster_traj/interp.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4094 2024-01-16 10:06:19.000000 stereopy-1.3.0b1/stereo/plots/plot_cluster_traj/plot_cluster_traj.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    20628 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/plots/plot_cluster_traj/traj.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.933879 stereopy-1.3.0b1/stereo/plots/plot_cluster_traj_3d/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       59 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/plots/plot_cluster_traj_3d/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3285 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/plots/plot_cluster_traj_3d/interp.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4830 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/plots/plot_cluster_traj_3d/plot_cluster_traj_3d.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    13057 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/plots/plot_cluster_traj_3d/traj.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     7401 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/plots/plot_clusters_heatmap.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     9976 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/plots/plot_clusters_scatter.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    56571 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/plots/plot_collection.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4376 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/plots/plot_coo.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4253 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/plots/plot_dendrogram.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3038 2024-01-16 10:06:19.000000 stereopy-1.3.0b1/stereo/plots/plot_elbow.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     5232 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/plots/plot_genes_in_pseudotime.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    29321 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/plots/plot_grn.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     9275 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/plots/plot_ms_spatial_scatter.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    22924 2024-04-09 01:58:28.000000 stereopy-1.3.0b1/stereo/plots/plot_paga.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2852 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/plots/plot_st_gears.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    39054 2024-01-16 10:06:19.000000 stereopy-1.3.0b1/stereo/plots/plot_time_series.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.935879 stereopy-1.3.0b1/stereo/plots/plot_vec/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       38 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/plots/plot_vec/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     5129 2024-01-16 10:06:19.000000 stereopy-1.3.0b1/stereo/plots/plot_vec/plot_vec.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    13707 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/plots/plot_vec/vec.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:03.978880 stereopy-1.3.0b1/stereo/plots/plot_vec_3d/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       43 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/plots/plot_vec_3d/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3134 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/plots/plot_vec_3d/plot_vec_3d.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    10105 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/plots/plot_vec_3d/vec.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    20940 2024-03-25 07:06:27.000000 stereopy-1.3.0b1/stereo/plots/scatter.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    14369 2024-05-14 08:11:03.000000 stereopy-1.3.0b1/stereo/plots/violin.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:04.000880 stereopy-1.3.0b1/stereo/plots/vt3d_browser/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    22029 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/plots/vt3d_browser/PAGA_traj.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1086 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/plots/vt3d_browser/README.md
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      117 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/plots/vt3d_browser/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2650 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/plots/vt3d_browser/example.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:04.067882 stereopy-1.3.0b1/stereo/plots/vt3d_browser/examples/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)   233887 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/plots/vt3d_browser/examples/example_ccc.ipynb
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)   507177 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/plots/vt3d_browser/examples/example_grn.ipynb
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)   397934 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/plots/vt3d_browser/examples/example_mesh.ipynb
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)   115622 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/plots/vt3d_browser/examples/example_paga.ipynb
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    28479 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/plots/vt3d_browser/stereopy_3D_browser.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:04.502889 stereopy-1.3.0b1/stereo/plots/vt3d_browser/vt3d_browser/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    28200 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/plots/vt3d_browser/vt3d_browser/535877f50039c0cb49a6196a5b7517cd.woff
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    11040 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/plots/vt3d_browser/vt3d_browser/6f0a76321d30f3c8120915e57f7bd77e.ttf
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    55956 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/plots/vt3d_browser/vt3d_browser/732389ded34cb9c52dd88271f1345af9.ttf
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      384 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/plots/vt3d_browser/vt3d_browser/index.html
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)  7362871 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/plots/vt3d_browser/vt3d_browser/index.js
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)  8129245 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/plots/vt3d_browser/vt3d_browser/index.js.map
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       16 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/plots/vt3d_browser/vt3d_browser/index1.html
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1497 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/plots/vt3d_browser/vt3d_browser/manifest.js
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    14640 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/plots/vt3d_browser/vt3d_browser/manifest.js.map
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)   890282 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/plots/vt3d_browser/vt3d_browser/vendor.js
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)  6646820 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/plots/vt3d_browser/vt3d_browser/vendor.js.map
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:04.743894 stereopy-1.3.0b1/stereo/preprocess/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      274 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/preprocess/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6388 2024-05-14 08:11:03.000000 stereopy-1.3.0b1/stereo/preprocess/filter.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1910 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/preprocess/normalize.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2975 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/preprocess/qc.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1750 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/preprocess/sc_transform.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:04.746894 stereopy-1.3.0b1/stereo/scripts/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)        0 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/stereo/scripts/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     7872 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/scripts/ccd.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6805 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/stereo_config.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:04.896897 stereopy-1.3.0b1/stereo/tools/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    16063 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/tools/LR_interaction.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      471 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/tools/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     7325 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/tools/boundary.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    13269 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/tools/cell_correct.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4330 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/tools/cell_cut.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3070 2024-03-25 07:06:27.000000 stereopy-1.3.0b1/stereo/tools/cell_segment.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    14777 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/tools/cell_type_anno.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     7431 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/tools/cluster.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     7026 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/tools/clustering.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     5333 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/tools/dim_reduce.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    15176 2024-03-25 07:06:27.000000 stereopy-1.3.0b1/stereo/tools/find_markers.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3246 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/tools/gem_filter.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8304 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/tools/highly_variable_genes.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    13813 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/tools/rna_velocity.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4941 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/tools/spatial_lag.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      997 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/tools/spatial_pattern_score.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4841 2024-03-29 06:19:46.000000 stereopy-1.3.0b1/stereo/tools/tissue_extraction.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      491 2023-12-04 09:57:50.000000 stereopy-1.3.0b1/stereo/tools/tools.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:04.964898 stereopy-1.3.0b1/stereo/utils/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      491 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/utils/__init__.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2585 2024-03-25 07:06:27.000000 stereopy-1.3.0b1/stereo/utils/_download.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1632 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/utils/correlation.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    26102 2024-05-31 02:44:13.000000 stereopy-1.3.0b1/stereo/utils/data_helper.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     7884 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/utils/hvg_utils.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     9874 2024-03-25 07:06:27.000000 stereopy-1.3.0b1/stereo/utils/pipeline_utils.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1411 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/utils/read_write_utils.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      868 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/utils/spmatrix_helper.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1963 2023-10-20 06:18:33.000000 stereopy-1.3.0b1/stereo/utils/time_consume.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:04.966898 stereopy-1.3.0b1/stereopy.egg-info/
+-rw-r--r--   0 tanliwei  (1010) tanliwei  (1010)     4949 2024-05-31 02:45:45.000000 stereopy-1.3.0b1/stereopy.egg-info/PKG-INFO
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    14362 2024-05-31 02:46:01.000000 stereopy-1.3.0b1/stereopy.egg-info/SOURCES.txt
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)        1 2024-05-31 02:45:45.000000 stereopy-1.3.0b1/stereopy.egg-info/dependency_links.txt
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       48 2024-05-31 02:45:45.000000 stereopy-1.3.0b1/stereopy.egg-info/entry_points.txt
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1115 2024-05-31 02:45:45.000000 stereopy-1.3.0b1/stereopy.egg-info/requires.txt
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)        7 2024-05-31 02:45:45.000000 stereopy-1.3.0b1/stereopy.egg-info/top_level.txt
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:05.024899 stereopy-1.3.0b1/tests/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      102 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/extra_requirements.txt
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)       74 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/image_requirements.txt
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      164 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/pytest.ini
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     8177 2024-03-25 07:06:27.000000 stereopy-1.3.0b1/tests/settings.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2199 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/test_batch_integration.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6098 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/test_cell_community_detection.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      749 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/test_cell_cut.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     5923 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/test_clustering.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3179 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/test_h5ad_format.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    13779 2024-03-25 07:06:27.000000 stereopy-1.3.0b1/tests/test_io.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1663 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/test_io_h5ms.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6477 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/test_marker_genes.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6423 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/test_merge_3d_data.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    10388 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/test_ms_data.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2338 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/test_plot_cluster_traj.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3846 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/test_plot_vec.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3310 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/test_regulatory_network_inference.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     2426 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/test_rna_velocity.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     6891 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/test_sctransform.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)      883 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/test_single_r.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1519 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/test_spatial_hotspot.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1373 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/test_stereo_exp_data.py
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     4418 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/test_time_series_analysis.py
+drwxrwxr-x   0 tanliwei  (1010) tanliwei  (1010)        0 2024-05-31 02:46:05.077900 stereopy-1.3.0b1/tests/workflows_conf/
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)    12332 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/workflows_conf/environment_linux_gpu.yml
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1298 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/workflows_conf/environment_linux_py38.yml
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     3948 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/workflows_conf/environment_linux_py39.yml
+-rw-rw-r--   0 tanliwei  (1010) tanliwei  (1010)     1774 2023-09-14 03:30:44.000000 stereopy-1.3.0b1/tests/workflows_conf/environment_win.yml
```

### Comparing `stereopy-1.2.0/.github/workflows/main.yml` & `stereopy-1.3.0b1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/.github/workflows/pytest_conda_linux.yml` & `stereopy-1.3.0b1/.github/workflows/pytest_conda_linux.yml`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/.github/workflows/pytest_conda_linux_dev.yml` & `stereopy-1.3.0b1/.github/workflows/pytest_conda_linux_dev.yml`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/.github/workflows/pytest_conda_linux_gpu.yml` & `stereopy-1.3.0b1/.github/workflows/pytest_conda_linux_gpu.yml`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/.github/workflows/pytest_conda_linux_image.yml` & `stereopy-1.3.0b1/.github/workflows/pytest_conda_linux_image.yml`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/.github/workflows/pytest_conda_win.yml` & `stereopy-1.3.0b1/.github/workflows/pytest_conda_win.yml`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/.gitignore` & `stereopy-1.3.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/LICENSE` & `stereopy-1.3.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/PKG-INFO` & `stereopy-1.3.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stereopy
-Version: 1.2.0
+Version: 1.3.0b1
 Summary: Spatial transcriptomic analysis in python.
 Home-page: https://github.com/STOmics/Stereopy
 Author: STOmics
 Author-email: tanliwei@stomics.tech
 License: MIT License
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,15 @@
 Requires-Dist: imageio==2.31.1
 Requires-Dist: numpy==1.23.5
 Requires-Dist: matplotlib==3.7.1
 Requires-Dist: pandas>=1.5.3
 Requires-Dist: scipy==1.10.1
 Requires-Dist: seaborn==0.12.2
 Requires-Dist: h5py>=3.7.0
-Requires-Dist: gefpy~=1.1.3
+Requires-Dist: gefpy==1.1.6
 Requires-Dist: setuptools>=61.0.0
 Requires-Dist: numba==0.56.4
 Requires-Dist: statsmodels>=0.14.0
 Requires-Dist: leidenalg>=0.10.1
 Requires-Dist: umap-learn==0.5.1
 Requires-Dist: KDEpy==1.1.0
 Requires-Dist: shapely>=2.0.0
@@ -66,15 +66,15 @@
 Requires-Dist: gtfparse==1.2.1
 Requires-Dist: harmonypy==0.0.6
 Requires-Dist: SQLAlchemy==1.3.24
 Requires-Dist: fbpca>=1.0
 Requires-Dist: geosketch>=1.2
 Requires-Dist: pyscenic>=0.12.1
 Requires-Dist: onnxruntime==1.15.1
-Requires-Dist: POT==0.8.1.0
+Requires-Dist: POT==0.9.1
 Requires-Dist: distinctipy>=1.2.2
 Requires-Dist: joypy>=0.2.6
 Requires-Dist: lxml>=4.8.0
 Requires-Dist: fastcluster>=1.2.6
 Requires-Dist: pycirclize>=0.5.0
 Requires-Dist: plotly>=5.15.0
 Requires-Dist: cusingler
```

### Comparing `stereopy-1.2.0/README.md` & `stereopy-1.3.0b1/README.md`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/quick_start.ipynb` & `stereopy-1.3.0b1/quick_start.ipynb`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/requirements.txt` & `stereopy-1.3.0b1/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 imageio==2.31.1
 numpy==1.23.5
 matplotlib==3.7.1
 pandas>=1.5.3
 scipy==1.10.1
 seaborn==0.12.2
 h5py>=3.7.0
-gefpy~=1.1.3
+gefpy==1.1.6
 # setuptools>=41.0.0,<60.0.0
 setuptools>=61.0.0
 #todo python3.8/site-packages/umap/distances.py:1053: NumbaDeprecationWarning: The 'nopython' keyword argument was not supplied to the 'numba.jit' decorator.
 #The implicit default value for this argument is currently False, but it will be changed to True in Numba 0.59.0.
 #See https://numba.readthedocs.io/en/stable/reference/deprecation.html#deprecation-of-object-mode-fall-back-behaviour-when-using-jit for details.
 numba==0.56.4
 statsmodels>=0.14.0
@@ -71,15 +71,15 @@
 gtfparse==1.2.1
 harmonypy==0.0.6
 SQLAlchemy==1.3.24
 fbpca>=1.0
 geosketch>=1.2
 pyscenic>=0.12.1
 onnxruntime==1.15.1
-POT==0.8.1.0
+POT==0.9.1
 distinctipy>=1.2.2
 joypy>=0.2.6
 lxml>=4.8.0
 fastcluster>=1.2.6
 pycirclize>=0.5.0
 plotly>=5.15.0
 cusingler
```

### Comparing `stereopy-1.2.0/setup.py` & `stereopy-1.3.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/_louvain.py` & `stereopy-1.3.0b1/stereo/algorithm/_louvain.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/algorithm_base.py` & `stereopy-1.3.0b1/stereo/algorithm/algorithm_base.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/batchqc_raw.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/batchqc_raw.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/main.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/main.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/module/classifier.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/module/classifier.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/module/dataset.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/module/dataset.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/module/early_stop.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/module/early_stop.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/module/loss.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/module/loss.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/module/trainer.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/module/trainer.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/score/get_neighbors.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/score/get_neighbors.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/score/kbet.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/score/kbet.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/score/ksim.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/score/ksim.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/score/lisi.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/score/lisi.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/template/report_template_adjust.html` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/template/report_template_adjust.html`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/template/report_template_raw.html` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/template/report_template_raw.html`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/test/__init__.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/__init__.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/test/cdf_plot.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/cdf_plot.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/test/describe_data.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/describe_data.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/test/distribution_fitting.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/distribution_fitting.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/test/heatmap.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/heatmap.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/test/joint_plot.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/joint_plot.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/test/kernel_plot.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/kernel_plot.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/test/metric_score.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/metric_score.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/test/pca_regression.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/pca_regression.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/test/qq_plot.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/qq_plot.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/test/umap_plot.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/umap_plot.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/test/var_mean_plot.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/var_mean_plot.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/test/variance_test.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/test/variance_test.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/utils/check_data.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/utils/check_data.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/utils/generate_palette.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/utils/generate_palette.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/utils/html_utils.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/utils/html_utils.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/utils/pca_lowrank.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/utils/pca_lowrank.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/batch_qc/utils/print_time.py` & `stereopy-1.3.0b1/stereo/algorithm/batch_qc/utils/print_time.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/ccd/assets/favicon.ico` & `stereopy-1.3.0b1/stereo/algorithm/ccd/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/ccd/community_clustering_algorithm.py` & `stereopy-1.3.0b1/stereo/algorithm/ccd/community_clustering_algorithm.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/ccd/constants.py` & `stereopy-1.3.0b1/stereo/algorithm/ccd/constants.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/ccd/html_report.py` & `stereopy-1.3.0b1/stereo/algorithm/ccd/html_report.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/ccd/metrics.py` & `stereopy-1.3.0b1/stereo/algorithm/ccd/metrics.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/ccd/sliding_window.py` & `stereopy-1.3.0b1/stereo/algorithm/ccd/sliding_window.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/ccd/utils.py` & `stereopy-1.3.0b1/stereo/algorithm/ccd/utils.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/cell_cell_communication/analysis_helper.py` & `stereopy-1.3.0b1/stereo/algorithm/cell_cell_communication/analysis_helper.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/cell_cell_communication/exceptions.py` & `stereopy-1.3.0b1/stereo/algorithm/cell_cell_communication/exceptions.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/cell_cell_communication/main.py` & `stereopy-1.3.0b1/stereo/algorithm/cell_cell_communication/main.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/cell_cell_communication/plot_ccc.py` & `stereopy-1.3.0b1/stereo/plots/plot_ccc.py`

 * *Files 0% similar despite different names*

```diff
@@ -513,15 +513,15 @@
         return pd.DataFrame(cell_counts, columns=cell_list, index=self.stereo_exp_data.gene_names)
 
     def _get_expressed_genes(self, count_df, pct):
         count_df = count_df.loc[(count_df != 0).mean(axis=1) >= pct, :]
         return list(count_df.index)
 
     def _get_expressed_network(self, network, expressed_genes):
-        sub_network = network[network['from'].isin(expressed_genes) & network['to'].isin(expressed_genes)]
+        sub_network = network[network['from'].isin(expressed_genes) & network['to'].isin(expressed_genes)].copy()
         return sub_network
 
     def _get_shortest_path(self, graph, source, target, distance, weight):
         shortest_path = nx.shortest_path(graph, source=source, target=target, weight=distance)
         path_weight_sum = 0
         for i in range(len(shortest_path) - 1):
             path_weight_sum = path_weight_sum + graph.get_edge_data(shortest_path[i], shortest_path[i + 1])[weight]
```

### Comparing `stereopy-1.2.0/stereo/algorithm/cell_cell_communication/spatial_scoloc.py` & `stereopy-1.3.0b1/stereo/algorithm/cell_cell_communication/spatial_scoloc.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 import random
 
 import igraph as ig
 import networkx as nx
 import numpy as np
 import pandas as pd
-import scanpy as sc
 from scipy import stats
 
 from stereo.algorithm.cell_cell_communication.analysis_helper import write_to_file
 from stereo.algorithm.cell_cell_communication.exceptions import InvalidMicroEnvInput
 
 
 class GetMicroEnvs:
@@ -334,14 +333,15 @@
         subgroup = []
         for t in thresh:
             sub = self.split_micro_envs(pairwise_kl_df, type_name, t)
             threshold.append(t)
             subgroup.append(sub)
             if len(sub) == 1:
                 break
+        subgroup = str(subgroup)
         subgroup_df = pd.DataFrame({"threshold": threshold, "subgroup_result": subgroup})
         return subgroup_df
 
     def _get_mst(self, type_name, kl_array):
         """
         Generate minimum spanning tree from given kl matrix
         """
@@ -358,50 +358,7 @@
         xidx, yidx = np.nonzero(mst_maskarray)
         type_name = np.array(type_name, dtype='str')
         round_pd = pd.DataFrame()
         round_pd['from'] = type_name[xidx.tolist()]
         round_pd['to'] = type_name[yidx.tolist()]
         return round_pd
 
-
-if __name__ == "__main__":
-    fly = sc.read_h5ad(r'C:\Users\liuxiaobin\Desktop\E14-16h_a_count_normal_stereoseq.h5ad')
-    gene_name = [str(x) for x in fly.var_names]  # 13668 genes
-    spot_name = [str(x) for x in fly.obs_names]  # 15295 cells
-
-    coord_x = [x[0] for x in fly.obsm['spatial']]
-    coord_y = [x[1] for x in fly.obsm['spatial']]
-    coord_z = [x[2] for x in fly.obsm['spatial']]
-    coord = pd.DataFrame({'cell': spot_name, 'coord_x': coord_x, 'coord_y': coord_y, 'coord_z': coord_z})
-
-    cell_type = fly.obs['annotation']
-    meta = pd.DataFrame({'cell': spot_name, 'cell_type': cell_type}).reset_index(drop=True)
-
-    boot_prop = 0.8
-    n_boot = 100
-    dimension = 3
-    fill_rare = True
-    min_num = 30
-    binsize = 2
-    eps = 1e-20
-    output_path: str = r'E:\Stereopy\小试答辩\小试答辩3\测试数据'
-
-    tt = GetMicroEnvs()
-    final_mst, pairwise_kl_df, path = tt.main(meta, coord, n_boot=20)
-    tt.generate_micro_envs('mst', threshold=0.3, result_df=final_mst, output_path=path)
-    tt.generate_micro_envs('split', threshold=2, result_df=pairwise_kl_df, output_path=path)
-
-    mouse = sc.read_h5ad(r'C:\Users\liuxiaobin\Desktop\MouseBrainCellbin.h5ad')
-    gene_name = [str(x) for x in mouse.var_names]  # 22404 genes
-    spot_name = [str(x) for x in mouse.obs_names]  # 49921 cells
-
-    coord_x = [x[0] for x in mouse.obsm['spatial']]
-    coord_y = [x[1] for x in mouse.obsm['spatial']]
-    coord = pd.DataFrame({'cell': spot_name, 'coord_x': coord_x, 'coord_y': coord_y})
-
-    cell_type = mouse.obs['celltype_pred']
-    meta = pd.DataFrame({'cell': spot_name, 'cell_type': cell_type}).reset_index(drop=True)
-
-    mm = GetMicroEnvs()
-    final_mst, pairwise_kl_df, path = mm.main(meta, coord, n_boot=20, dimension=2)
-    mm.generate_micro_envs('mst', threshold=0.1, result_df=final_mst, output_path=path)
-    mm.generate_micro_envs('split', threshold=1, result_df=pairwise_kl_df, output_path=path)
```

### Comparing `stereopy-1.2.0/stereo/algorithm/cell_cell_communication/utils/database_utils.py` & `stereopy-1.3.0b1/stereo/algorithm/cell_cell_communication/utils/database_utils.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/cell_cell_communication/utils/sqlalchemy_model.py` & `stereopy-1.3.0b1/stereo/algorithm/cell_cell_communication/utils/sqlalchemy_model.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/cell_cell_communication/utils/sqlalchemy_repository.py` & `stereopy-1.3.0b1/stereo/algorithm/cell_cell_communication/utils/sqlalchemy_repository.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/cell_cell_communication/utils/visualization_process.py` & `stereopy-1.3.0b1/stereo/algorithm/cell_cell_communication/utils/visualization_process.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/cell_correction.py` & `stereopy-1.3.0b1/stereo/algorithm/cell_correction.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/cell_correction_fast.py` & `stereopy-1.3.0b1/stereo/algorithm/cell_correction_fast.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/cell_correction_fast_by_mask.py` & `stereopy-1.3.0b1/stereo/algorithm/cell_correction_fast_by_mask.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/cell_pose/__init__.py` & `stereopy-1.3.0b1/stereo/algorithm/cell_pose/__init__.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/cell_pose/cell_pose.py` & `stereopy-1.3.0b1/stereo/algorithm/cell_pose/cell_pose.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/cell_pose/core.py` & `stereopy-1.3.0b1/stereo/algorithm/cell_pose/core.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/cell_pose/dynamics.py` & `stereopy-1.3.0b1/stereo/algorithm/cell_pose/dynamics.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/cell_pose/io.py` & `stereopy-1.3.0b1/stereo/algorithm/cell_pose/io.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/cell_pose/metrics.py` & `stereopy-1.3.0b1/stereo/algorithm/cell_pose/metrics.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/cell_pose/models.py` & `stereopy-1.3.0b1/stereo/algorithm/cell_pose/models.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/cell_pose/plot.py` & `stereopy-1.3.0b1/stereo/algorithm/cell_pose/plot.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/cell_pose/resnet_torch.py` & `stereopy-1.3.0b1/stereo/algorithm/cell_pose/resnet_torch.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/cell_pose/utils.py` & `stereopy-1.3.0b1/stereo/algorithm/cell_pose/utils.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/cell_pose/version.py` & `stereopy-1.3.0b1/stereo/algorithm/cell_pose/version.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/co_occurrence.py` & `stereopy-1.3.0b1/stereo/algorithm/co_occurrence.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/community_detection.py` & `stereopy-1.3.0b1/stereo/algorithm/community_detection.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/dendrogram.py` & `stereopy-1.3.0b1/stereo/algorithm/dendrogram.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/dim_reduce.py` & `stereopy-1.3.0b1/stereo/algorithm/dim_reduce.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/dpt/main.py` & `stereopy-1.3.0b1/stereo/algorithm/dpt/main.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/dpt/pca.py` & `stereopy-1.3.0b1/stereo/algorithm/dpt/pca.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/dpt/struct.py` & `stereopy-1.3.0b1/stereo/algorithm/dpt/struct.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/draw_contours.py` & `stereopy-1.3.0b1/stereo/algorithm/draw_contours.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/gaussian_smooth.py` & `stereopy-1.3.0b1/stereo/algorithm/gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/gen_ccc_micro_envs.py` & `stereopy-1.3.0b1/stereo/algorithm/gen_ccc_micro_envs.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,18 +118,20 @@
                 'mst_final': mst_final,
                 'pairwise_kl_divergence': pairwise_kl_divergence,
                 'split_by_different_threshold': split_by_different_threshold
             }
             print("Now, you can choose a appropriate threshold based on this function's result.")
             if show_dividing_by_thresholds:
                 pn.extension()
-                split_by_different_threshold_copy = split_by_different_threshold.copy()
-                split_by_different_threshold_copy['subgroup_result'] = split_by_different_threshold_copy[
-                    'subgroup_result'].astype('U')
-                return pn.widgets.DataFrame(split_by_different_threshold_copy, disabled=True, show_index=False,
+                # split_by_different_threshold_copy = split_by_different_threshold.copy()
+                # split_by_different_threshold_copy['subgroup_result'] = split_by_different_threshold_copy[
+                #     'subgroup_result'].astype('U')
+                # return pn.widgets.DataFrame(split_by_different_threshold_copy, disabled=True, show_index=False,
+                #                             autosize_mode="fit_viewport", frozen_columns=1)
+                return pn.widgets.DataFrame(split_by_different_threshold, disabled=True, show_index=False,
                                             autosize_mode="fit_viewport", frozen_columns=1)
         else:
             if res_key not in self.pipeline_res:
                 raise PipelineResultInexistent(res_key)
 
             if method not in ['mst', 'split']:
                 raise ValueError(f"Invalid method({method}), choose it from 'mst' and 'split'")
```

### Comparing `stereopy-1.2.0/stereo/algorithm/gen_mesh.py` & `stereopy-1.3.0b1/stereo/algorithm/gen_mesh.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/get_niche.py` & `stereopy-1.3.0b1/stereo/algorithm/get_niche.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/highly_variable_genes.py` & `stereopy-1.3.0b1/stereo/algorithm/highly_variable_genes.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/leiden.py` & `stereopy-1.3.0b1/stereo/algorithm/leiden.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/log1p_fake.py` & `stereopy-1.3.0b1/stereo/algorithm/log1p_fake.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/mannwhitneyu.py` & `stereopy-1.3.0b1/stereo/algorithm/mannwhitneyu.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/ms_algorithm_base.py` & `stereopy-1.3.0b1/stereo/algorithm/ms_algorithm_base.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/ms_community_detection.py` & `stereopy-1.3.0b1/stereo/algorithm/ms_community_detection.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/neighbors.py` & `stereopy-1.3.0b1/stereo/algorithm/neighbors.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/normalization.py` & `stereopy-1.3.0b1/stereo/algorithm/normalization.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/paga.py` & `stereopy-1.3.0b1/stereo/algorithm/paga.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/paste/helper.py` & `stereopy-1.3.0b1/stereo/algorithm/paste/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 )
 
 # from anndata import AnnData
 import numpy as np
 import ot
 import scipy
 
-from stereo.core.stereo_exp_data import StereoExpData
+from stereo.core.stereo_exp_data import StereoExpData, AnnBasedStereoExpData
 
 
 def filter_for_common_genes(slices: List[StereoExpData]) -> None:
     """
     Filters for the intersection of genes between all slices.
 
     Args:
@@ -248,16 +248,23 @@
                                                                   output_params=output_params, matrix=matrix)
             thetas.append(theta)
             translations.append(tY)
         new_coor.append(y)
 
     # new_slices = []
     for i in range(len(slices)):
-        slices[i].raw_position = slices[i].position
-        slices[i].position = new_coor[i]
+        if isinstance(slices[i], AnnBasedStereoExpData):
+            if slices[i].position_z is not None:
+                slices[i].adata.obsm['spatial_paste_pairwise'] = np.concatenate((new_coor[i], slices[i].position_z), axis=1)
+            else:
+                slices[i].adata.obsm['spatial_paste_pairwise'] = new_coor[i]
+            slices[i].spatial_key = 'spatial_paste_pairwise'
+        else:
+            slices[i].raw_position = slices[i].position
+            slices[i].position = new_coor[i]
 
     if not output_params:
         return slices
     else:
         return slices, thetas, translations
 
 
@@ -310,23 +317,37 @@
             c, y, theta, tX, tY = generalized_procrustes_analysis(center_slice.position, slices[i].position, pis[i],
                                                                   output_params=output_params, matrix=matrix)
             thetas.append(theta)
             translations.append(tY)
         new_coor.append(y)
 
     for i in range(len(slices)):
-        slices[i].raw_position = slices[i].position
-        slices[i].position = new_coor[i]
+        if isinstance(slices[i], AnnBasedStereoExpData):
+            if slices[i].position_z is not None:
+                slices[i].adata.obsm['spatial_paste_center'] = np.concatenate((new_coor[i], slices[i].position_z), axis=1)
+            else:
+                slices[i].adata.obsm['spatial_paste_center'] = new_coor[i]
+            slices[i].spatial_key = 'spatial_paste_center'
+        else:
+            slices[i].raw_position = slices[i].position
+            slices[i].position = new_coor[i]
 
-    center_slice.raw_position = center_slice.position
-    center_slice.position = c
+    if isinstance(center_slice, AnnBasedStereoExpData):
+        if center_slice.position_z is not None:
+            center_slice.adata.obsm['spatial_paste_center'] = np.concatenate((center_slice.position, center_slice.position_z), axis=1)
+        else:
+            center_slice.adata.obsm['spatial_paste_center'] = c
+        center_slice.spatial_key = 'spatial_paste_center'
+    else:
+        center_slice.raw_position = center_slice.position
+        center_slice.position = c
     if not output_params:
-        return center_slice, slices[i]
+        return center_slice, slices
     else:
-        return center_slice, slices[i], thetas, translations
+        return center_slice, slices, thetas, translations
 
 
 def generalized_procrustes_analysis(X, Y, pi, output_params=False, matrix=False):
     """
     Finds and applies optimal rotation between spatial coordinates of two layers (may also do a reflection).
 
     Args:
```

### Comparing `stereopy-1.2.0/stereo/algorithm/paste/methods.py` & `stereopy-1.3.0b1/stereo/algorithm/paste/methods.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 )
 
 import numpy as np
 # from anndata import AnnData
 import ot
 from sklearn.decomposition import NMF
 
+
 from stereo.core.cell import Cell
 from stereo.core.gene import Gene
 from stereo.core.stereo_exp_data import StereoExpData
 from stereo.log_manager import LogManager
 from stereo.log_manager import logger
 from .helper import (
     kl_divergence_backend,
@@ -63,16 +64,18 @@
     :return: Alignment of spots. If ``return_obj = True``, additionally returns objective function output of FGW-OT.
     """  # noqa
 
     # Determine if gpu or cpu is being used
     if use_gpu:
         try:
             import torch
+            backend = ot.backend.TorchBackend()
         except Exception:
             logger.warning("We currently only have gpu support for Pytorch. Please install torch.")
+            backend = ot.backend.NumpyBackend()
 
         if isinstance(backend, ot.backend.TorchBackend):
             if torch.cuda.is_available():
                 if gpu_verbose:
                     logger.info("gpu is available, using gpu.")
             else:
                 if gpu_verbose:
@@ -220,16 +223,18 @@
         - List of pairwise alignment mappings of the center slice (rows) to each input slice (columns).
     """  # noqa
 
     # Determine if gpu or cpu is being used
     if use_gpu:
         try:
             import torch
+            backend = ot.backend.TorchBackend()
         except Exception:
             logger.warning("We currently only have gpu support for Pytorch. Please install torch.")
+            backend = ot.backend.NumpyBackend()
 
         if isinstance(backend, ot.backend.TorchBackend):
             if torch.cuda.is_available():
                 if gpu_verbose:
                     logger.info("gpu is available, using gpu.")
             else:
                 if gpu_verbose:
@@ -354,50 +359,123 @@
         model = NMF(n_components=n_components, solver='mu', beta_loss='kullback-leibler', init='random',
                     random_state=random_seed, max_iter=max_iter, verbose=verbose)
     W_new = model.fit_transform(B)
     H_new = model.components_
     return W_new, H_new
 
 
-def my_fused_gromov_wasserstein(M, C1, C2, p, q, G_init=None, loss_fun='square_loss', alpha=0.5, armijo=False,
-                                log=False, numItermax=200, use_gpu=False, **kwargs):
+def my_fused_gromov_wasserstein(M, C1, C2, p, q, G_init = None, loss_fun='square_loss', alpha=0.5, armijo=False, log=False,numItermax=200, tol_rel=1e-9, tol_abs=1e-9, use_gpu = False, **kwargs):
     """
     Adapted fused_gromov_wasserstein with the added capability of defining a G_init (inital mapping).
     Also added capability of utilizing different POT backends to speed up computation.
-
+    
     For more info, see: https://pythonot.github.io/gen_modules/ot.gromov.html
     """
 
     p, q = ot.utils.list_to_array(p, q)
 
     p0, q0, C10, C20, M0 = p, q, C1, C2, M
     nx = ot.backend.get_backend(p0, q0, C10, C20, M0)
 
     constC, hC1, hC2 = ot.gromov.init_matrix(C1, C2, p, q, loss_fun)
 
     if G_init is None:
         G0 = p[:, None] * q[None, :]
     else:
-        G0 = (1 / nx.sum(G_init)) * G_init
+        G0 = (1/nx.sum(G_init)) * G_init
         if use_gpu:
             G0 = G0.cuda()
 
     def f(G):
         return ot.gromov.gwloss(constC, hC1, hC2, G)
 
     def df(G):
         return ot.gromov.gwggrad(constC, hC1, hC2, G)
+    
+    if loss_fun == 'kl_loss':
+        armijo = True  # there is no closed form line-search with KL
+
+    if armijo:
+        def line_search(cost, G, deltaG, Mi, cost_G, **kwargs):
+            return ot.optim.line_search_armijo(cost, G, deltaG, Mi, cost_G, nx=nx, **kwargs)
+    else:
+        def line_search(cost, G, deltaG, Mi, cost_G, **kwargs):
+            return solve_gromov_linesearch(G, deltaG, cost_G, C1, C2, M=0., reg=1., nx=nx, **kwargs)
 
     if log:
-        res, log = ot.gromov.cg(p, q, (1 - alpha) * M, alpha, f, df, G0, armijo=armijo, C1=C1, C2=C2, constC=constC,
-                                log=True, numItermax=numItermax, **kwargs)
+        res, log = ot.optim.cg(p, q, (1 - alpha) * M, alpha, f, df, G0, line_search, log=True, numItermax=numItermax, stopThr=tol_rel, stopThr2=tol_abs, **kwargs)
 
         fgw_dist = log['loss'][-1]
 
         log['fgw_dist'] = fgw_dist
         log['u'] = log['u']
         log['v'] = log['v']
         return res, log
 
     else:
-        return ot.gromov.cg(p, q, (1 - alpha) * M, alpha, f, df, G0, armijo=armijo, C1=C1, C2=C2, constC=constC,
-                            **kwargs)
+        return ot.optim.cg(p, q, (1 - alpha) * M, alpha, f, df, G0, line_search, numItermax=numItermax, stopThr=tol_rel, stopThr2=tol_abs, **kwargs)
+
+def solve_gromov_linesearch(G, deltaG, cost_G, C1, C2, M, reg,
+                            alpha_min=None, alpha_max=None, nx=None, **kwargs):
+    """
+    Solve the linesearch in the FW iterations
+
+    Parameters
+    ----------
+
+    G : array-like, shape(ns,nt)
+        The transport map at a given iteration of the FW
+    deltaG : array-like (ns,nt)
+        Difference between the optimal map found by linearization in the FW algorithm and the value at a given iteration
+    cost_G : float
+        Value of the cost at `G`
+    C1 : array-like (ns,ns), optional
+        Structure matrix in the source domain.
+    C2 : array-like (nt,nt), optional
+        Structure matrix in the target domain.
+    M : array-like (ns,nt)
+        Cost matrix between the features.
+    reg : float
+        Regularization parameter.
+    alpha_min : float, optional
+        Minimum value for alpha
+    alpha_max : float, optional
+        Maximum value for alpha
+    nx : backend, optional
+        If let to its default value None, a backend test will be conducted.
+    Returns
+    -------
+    alpha : float
+        The optimal step size of the FW
+    fc : int
+        nb of function call. Useless here
+    cost_G : float
+        The value of the cost for the next iteration
+
+
+    .. _references-solve-linesearch:
+    References
+    ----------
+    .. [24] Vayer Titouan, Chapel Laetitia, Flamary Rémi, Tavenard Romain and Courty Nicolas
+        "Optimal Transport for structured data with application on graphs"
+        International Conference on Machine Learning (ICML). 2019.
+    """
+    if nx is None:
+        G, deltaG, C1, C2, M = ot.utils.list_to_array(G, deltaG, C1, C2, M)
+
+        if isinstance(M, int) or isinstance(M, float):
+            nx = ot.backend.get_backend(G, deltaG, C1, C2)
+        else:
+            nx = ot.backend.get_backend(G, deltaG, C1, C2, M)
+
+    dot = nx.dot(nx.dot(C1, deltaG), C2.T)
+    a = -2 * reg * nx.sum(dot * deltaG)
+    b = nx.sum(M * deltaG) - 2 * reg * (nx.sum(dot * G) + nx.sum(nx.dot(nx.dot(C1, G), C2.T) * deltaG))
+
+    alpha = ot.optim.solve_1d_linesearch_quad(a, b)
+    if alpha_min is not None or alpha_max is not None:
+        alpha = np.clip(alpha, alpha_min, alpha_max)
+
+    # the new cost is deduced from the line search quadratic function
+    cost_G = cost_G + a * (alpha ** 2) + b * alpha
+
+    return alpha, 1, cost_G
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stereopy-1.2.0/stereo/algorithm/paste/paste.py` & `stereopy-1.3.0b1/stereo/algorithm/paste/paste.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,20 @@
         :param initial_slice: slice to use as the initialization for center alignment, defaults to None
         :param slices: list of slices to align, defaults to None
 
         Other parameters refer to `algorithm.paste.pairwise_align` and `algorithm.paste.center_align`
         """
         if method not in ('pairwise', 'center'):
             raise ValueError(f'Error method({method}), it must be one of pairwise and center')
+        
+        try:
+            from tensorflow.python.ops.numpy_ops import np_config
+            np_config.enable_numpy_behavior()
+        except:
+            pass
 
         logger.info(f'Using method {method}')
         if method == 'pairwise':
             if slices is None:
                 slice_names = self.ms_data.names
                 slices = self.ms_data.data_list
             else:
```

### Comparing `stereopy-1.2.0/stereo/algorithm/regulatory_network_inference/main.py` & `stereopy-1.3.0b1/stereo/algorithm/regulatory_network_inference/main.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/regulatory_network_inference/plot_grn.py` & `stereopy-1.3.0b1/stereo/plots/plot_grn.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/scale.py` & `stereopy-1.3.0b1/stereo/algorithm/scale.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/scenic.py` & `stereopy-1.3.0b1/stereo/algorithm/scenic.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/sctransform/bw.py` & `stereopy-1.3.0b1/stereo/algorithm/sctransform/bw.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/sctransform/ksmooth.py` & `stereopy-1.3.0b1/stereo/algorithm/sctransform/ksmooth.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/sctransform/plotting.py` & `stereopy-1.3.0b1/stereo/algorithm/sctransform/plotting.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/sctransform/scale_data.py` & `stereopy-1.3.0b1/stereo/algorithm/sctransform/scale_data.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/sctransform/sctransform.py` & `stereopy-1.3.0b1/stereo/algorithm/sctransform/sctransform.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/sctransform/utils.py` & `stereopy-1.3.0b1/stereo/algorithm/sctransform/utils.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/sctransform/vst.py` & `stereopy-1.3.0b1/stereo/algorithm/sctransform/vst.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/single_r/single_r.py` & `stereopy-1.3.0b1/stereo/algorithm/single_r/single_r.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/single_r/utils.py` & `stereopy-1.3.0b1/stereo/algorithm/single_r/utils.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/spatial_hotspot.py` & `stereopy-1.3.0b1/stereo/algorithm/spatial_hotspot.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/spatial_pattern_score.py` & `stereopy-1.3.0b1/stereo/algorithm/spatial_pattern_score.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/statistics.py` & `stereopy-1.3.0b1/stereo/algorithm/statistics.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/algorithm/total_vi.py` & `stereopy-1.3.0b1/stereo/algorithm/total_vi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+import gc
 from copy import deepcopy
 from typing import Optional
 from typing import Union
 
+import numpy as np
+
 import anndata
 import pandas as pd
 
 try:
     import scvi
     import mudata
 except ImportError:
@@ -41,14 +44,15 @@
             rna_key: Union[str, int] = None,
             protein_key: Union[str, int] = None,
             hvg_key: Union[str, int] = None,
             res_key: str = 'totalVI',
             rna_use_raw: bool = False,
             protein_use_raw: bool = False,
             use_gpu: Union[int, str, bool] = None,
+            num_threads: int = None,
             train_kwargs: Optional[dict] = {},
             **kwags
     ):
         if rna_key is None:
             rna_data = self.ms_data[0]
         else:
             rna_data = self.ms_data[rna_key]
@@ -127,14 +131,15 @@
             protein_layer="counts" if protein_use_raw else None,
             modalities={
                 "rna_layer": "multiomics" if self._use_hvg else "rna",
                 "protein_layer": "protein",
             })
 
         total_vi = scvi.model.TOTALVI(mdata, **kwags)
+        scvi.settings.num_threads = num_threads
         total_vi.train(use_gpu=use_gpu, **train_kwargs)
 
         if not self._use_hvg:
             rna = rna_data
         else:
             rna = hvg_data
 
@@ -156,15 +161,16 @@
         return self
 
     def save_result(
             self,
             use_cluster_res_key: str = None,
             out_dir: str = None,
             diff_exp_file_name: str = None,
-            h5mu_file_name: str = None
+            h5mu_file_name: str = None,
+            fragment: int = 5
     ):
         import os.path as opth
         if out_dir is None or not opth.exists(out_dir):
             raise FileNotFoundError(f'The directory {out_dir} is not exists.')
 
         if self._use_hvg:
             clustered_data = self._hvg_data
@@ -180,30 +186,61 @@
         try:
             rna_adata: anndata.AnnData = stereo_to_anndata(self._rna_data, base_adata=mdata.mod['rna'],
                                                            split_batches=False)
             protein_adata: anndata.AnnData = stereo_to_anndata(self._protein_data, base_adata=mdata.mod['protein'],
                                                                split_batches=False)
             protein_adata.var['protein_names'] = protein_adata.var_names
             if self._use_hvg:
+                mdata.mod['multiomics'].uns['omics'] = [['Transcriptomics'], ['Proteomics']]
+                mdata.mod['multiomics'].uns['leiden_resolution'] = 1
                 hvg_adata: anndata.AnnData = stereo_to_anndata(self._hvg_data, base_adata=mdata.mod['multiomics'],
                                                                split_batches=False)
             mdata.update()
         finally:
             LogManager.start_logging()
 
         mod_key = 'multiomics' if self._use_hvg else 'rna'
         rna = hvg_adata if self._use_hvg else rna_adata
 
         de_df = self._total_vi_instance.differential_expression(groupby=f"{mod_key}:{use_cluster_res_key}", delta=0.5)
         if diff_exp_file_name is None:
             diff_exp_file_name = f'{self._rna_data.sn}_{self._rna_data.bin_size}_differential_expression.csv'
         de_df.to_csv(f'{out_dir}/{diff_exp_file_name}')
 
-        denoised_rna, denoised_protein = self._total_vi_instance.get_normalized_expression(n_samples=25,
-                                                                                           return_mean=True)
+        # Divide the 4000 gene list into 5 slices, After sharding,
+        # the output arrays need to be merged and the shapes need to be consistent.
+        frequency = len(rna.var_names) // fragment
+        assert (frequency != 0), 'The number of slices of genes is wrong, causing the array to go out of bounds'
+        denoised_rna_list = []
+        denoised_protein_list = []
+        rna_end = rna_start = 0
+        for i in range(fragment):
+            if i < fragment - 1:
+                rna_end += frequency
+                gene_list = rna.var_names[rna_start:rna_end]
+                rna_start = rna_end
+            else:
+                gene_list = rna.var_names[rna_start:]
+            denoised_rna_, denoised_protein_ = \
+                self._total_vi_instance.get_normalized_expression(n_samples=25,
+                                                                  batch_size=64,
+                                                                  gene_list=gene_list,
+                                                                  return_mean=True)
+            denoised_rna_list.append(denoised_rna_)
+            denoised_protein_list.append(denoised_protein_)
+            del denoised_rna_, denoised_protein_
+            gc.collect()
+
+        # Merging results after sharded model inference
+        denoised_rna = pd.concat(denoised_rna_list, axis=1)
+        denoised_protein = pd.concat(denoised_protein_list, axis=0)
+        # he protein uses the average of five results. Can the median be used
+        denoised_protein = denoised_protein.groupby(denoised_protein.index).sum()
+        denoised_protein = denoised_protein.div(fragment, fill_value=np.NaN)
+
         denoised_protein = denoised_protein.loc[rna_adata.obs_names]
 
         protein_foreground_prob = self._total_vi_instance.get_protein_foreground_probability(
             n_samples=25, return_mean=True).loc[rna_adata.obs_names]
 
         rna.layers['denoised_rna'] = denoised_rna
         protein_adata.layers['denoised_protein'] = denoised_protein
```

### Comparing `stereopy-1.2.0/stereo/algorithm/umap.py` & `stereopy-1.3.0b1/stereo/algorithm/umap.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/constant.py` & `stereopy-1.3.0b1/stereo/constant.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/core/cell.py` & `stereopy-1.3.0b1/stereo/core/cell.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,27 @@
 from anndata import AnnData
 
 
 class Cell(object):
 
     def __init__(
             self,
-            cell_name: Optional[np.ndarray],
+            obs: Optional[pd.DataFrame] = None,
+            cell_name: Optional[np.ndarray] = None,
             cell_border: Optional[np.ndarray] = None,
             batch: Optional[Union[np.ndarray, list, int, str]] = None
     ):
-        self._obs = pd.DataFrame(index=cell_name if cell_name is None else cell_name.astype('U'))
+        if obs is not None:
+            if not isinstance(obs, pd.DataFrame):
+                raise TypeError("obs must be a DataFrame.")
+            self._obs = obs
+            if cell_name is not None:
+                self.cell_name = cell_name
+        else:
+            self._obs = pd.DataFrame(index=cell_name if cell_name is None else cell_name.astype('U'))
         # self.loc = self._obs.loc
         self._matrix = dict()
         self._pairwise = dict()
         if batch is not None:
             self._obs['batch'] = self._set_batch(batch)
         self._cell_border = cell_border
         self.cell_point = None
@@ -51,21 +59,36 @@
             self._obs[key] = value
 
     def __getitem__(self, key):
         # if key not in self._obs.columns:
         #     return None
         return self._obs[key]
     
+    def __len__(self):
+        return self.size
+    
+    @property
+    def size(self):
+        return self._obs.index.size
+    
     @property
     def loc(self):
         return self._obs.loc
     
     @property
     def iloc(self):
         return self._obs.iloc
+    
+    @property
+    def to_csv(self):
+        return self._obs.to_csv
+    
+    @property
+    def obs(self):
+        return self._obs
 
     @property
     def total_counts(self):
         if 'total_counts' not in self._obs.columns:
             return None
         return self._obs['total_counts'].to_numpy()
 
@@ -204,15 +227,15 @@
 
 class AnnBasedCell(Cell):
 
     def __init__(self, based_ann_data: AnnData, cell_name: Optional[np.ndarray] = None,
                  cell_border: Optional[np.ndarray] = None,
                  batch: Optional[Union[np.ndarray, list, int, str]] = None):
         self.__based_ann_data = based_ann_data
-        super(AnnBasedCell, self).__init__(cell_name)
+        super(AnnBasedCell, self).__init__(cell_name=cell_name)
         if cell_border is not None:
             self.cell_border = cell_border
         if batch is not None:
             self.batch = batch
 
     def __setattr__(self, key, value):
         if key == '_obs':
@@ -325,9 +348,9 @@
     def cell_border(self, cell_border: np.ndarray):
         if not isinstance(cell_border, np.ndarray):
             raise TypeError('cell border must be a np.ndarray object.')
         if len(cell_border.shape) != 3:
             raise Exception(f'The cell border must have 3 dimensions, but now {len(cell_border.shape)}.')
         self.__based_ann_data.obsm['cell_border'] = cell_border
 
-    def to_df(self):
-        return self.__based_ann_data.obs
+    def to_df(self, copy=False):
+        return self.__based_ann_data.obs.copy(deep=True) if copy else self.__based_ann_data.obs
```

### Comparing `stereopy-1.2.0/stereo/core/data.py` & `stereopy-1.3.0b1/stereo/core/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                  file_path: Optional[str] = None,
                  file_format: Optional[str] = None,
                  output: Optional[str] = None,
                  partitions: int = 1):
         self._file = Path(file_path) if file_path is not None else None
         self._partitions = int(partitions)
         self._file_format = file_format
-        self.format_range = ['gem', 'gef', 'mtx', 'h5ad', 'scanpy_h5ad']
+        self.format_range = ['gem', 'gef', 'mtx', 'h5ad', 'scanpy_h5ad', 'h5ms', 'h5']
         self._output = output
 
     def check(self):
         """
         checking whether the params is in the range.
 
         :return:
@@ -63,14 +63,16 @@
         :param path:
         :return:
         """
         if path is None:
             logger.warning('the output path is set as None.')
             return
         out_dir = os.path.dirname(path)
+        if len(out_dir) == 0:
+            out_dir = './'
         if not os.path.exists(out_dir):
             os.makedirs(out_dir)
         if os.path.exists(path):
             logger.warning('the output file is exists, we will replace it with new file.')
 
     @staticmethod
     def file_check(file):
```

### Comparing `stereopy-1.2.0/stereo/core/gene.py` & `stereopy-1.3.0b1/stereo/core/gene.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,16 +12,27 @@
 
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 
 
 class Gene(object):
-    def __init__(self, gene_name: Optional[np.ndarray]):
-        self._var = pd.DataFrame(index=gene_name if gene_name is None else gene_name.astype('U'))
+    def __init__(
+            self,
+            var: Optional[pd.DataFrame] = None,
+            gene_name: Optional[np.ndarray] = None
+        ):
+        if var is not None:
+            if not isinstance(var, pd.DataFrame):
+                raise TypeError("var must be a DataFrame.")
+            self._var = var
+            if gene_name is not None:
+                self.gene_name = gene_name
+        else:
+            self._var = pd.DataFrame(index=gene_name if gene_name is None else gene_name.astype('U'))
         self._matrix = dict()
         self._pairwise = dict()
         # self.loc = self._var.loc
 
     def __contains__(self, item):
         return item in self._var.columns
 
@@ -36,21 +47,36 @@
         self._var[key] = value
 
     def __getitem__(self, key):
         # if key not in self._var.columns:
         #     return None
         return self._var[key]
     
+    def __len__(self):
+        return self.size
+    
+    @property
+    def size(self):
+        return self.gene_name.size
+    
     @property
     def loc(self):
         return self._var.loc
     
     @property
     def iloc(self):
         return self._var.iloc
+    
+    @property
+    def to_csv(self):
+        return self._var.to_csv
+    
+    @property
+    def var(self):
+        return self._var
 
     @property
     def n_cells(self):
         if 'n_cells' not in self._var.columns:
             return None
         return self._var['n_cells'].to_numpy()
 
@@ -95,27 +121,33 @@
         """
         set the name of gene.
 
         :param name: a numpy array of names.
         :return:
         """
         if not isinstance(name, np.ndarray):
-            raise TypeError('gene name must be a np.ndarray object.')
+            raise TypeError('gene name must be a np.ndarray.')
         self._var = self._var.reindex(name)
     
     @property
     def real_gene_name(self):
         if 'real_gene_name' in self._var.columns:
             return self._var['real_gene_name'].to_numpy().astype('U')
         else:
             return None
+    
+    @real_gene_name.setter
+    def real_gene_name(self, real_gene_name):
+        if not isinstance(real_gene_name, np.ndarray):
+            raise TypeError('gene name must be a np.ndarray.')
+        self._var['real_gene_name'] = real_gene_name
 
     def sub_set(self, index):
         """
-        get the subset of Gene by the index info， the Gene object will be inplaced by the subset.
+        get the subset of Gene by the index info, the Gene object will be inplaced by the subset.
 
         :param index: a numpy array of index info.
         :return: the subset of Gene object.
         """
         if isinstance(index, list) or isinstance(index, slice):
             self._var = self._var.iloc[index].copy()
         elif isinstance(index, np.ndarray):
@@ -145,15 +177,15 @@
         return self._var._repr_html_()
 
 
 class AnnBasedGene(Gene):
 
     def __init__(self, based_ann_data: AnnData, gene_name: Optional[np.ndarray] = None):
         self.__based_ann_data = based_ann_data
-        super(AnnBasedGene, self).__init__(gene_name)
+        super(AnnBasedGene, self).__init__(gene_name=gene_name)
 
     def __setattr__(self, key, value):
         if key == '_var':
             return
         object.__setattr__(self, key, value)
 
     def __str__(self):
@@ -207,9 +239,9 @@
     @property
     def real_gene_name(self):
         if 'real_gene_name' in self.__based_ann_data.var.columns:
             return self.__based_ann_data.var['real_gene_name'].to_numpy().astype('U')
         else:
             return None
 
-    def to_df(self):
-        return self.__based_ann_data.var
+    def to_df(self, copy=False):
+        return self.__based_ann_data.var.copy(deep=True) if copy else self.__based_ann_data.var
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `stereopy-1.2.0/stereo/core/ms_data.py` & `stereopy-1.3.0b1/stereo/core/ms_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from __future__ import annotations
 from dataclasses import dataclass, field
 from typing import List, Dict, Union, Literal, Optional
+from copy import deepcopy
 
 import numpy as np
 import pandas as pd
 
 from . import StPipeline, StereoExpData
 from .ms_pipeline import MSDataPipeLine
 from ..plots.plot_collection import PlotCollection
@@ -12,38 +14,84 @@
 def _default_idx() -> int:
     # return -1 function `__get_auto_key` will start with 0 instead of 1
     return -1
 
 
 @dataclass
 class _MSDataView(object):
+    _msdata: MSData = None
     _names: List[str] = field(default_factory=list)
     _data_list: List[StereoExpData] = field(default_factory=list)
+    _name_dict: Dict[str, StereoExpData] = field(default_factory=dict)
     _merged_data: StereoExpData = None
     _tl = None
     _plt = None
 
-    def __getitem__(self, key: slice):
-        if type(key) is not slice:
-            raise TypeError(f'{key} should be slice')
+    def __post_init__(self):
+        for name, data in zip(self._names, self._data_list):
+            self._name_dict[name] = data 
+
+    def __get_data_list(self, key_idx_list):
         data_list = []
         names = []
-        if type(key.start) is tuple or type(key.start) is list:
-            for obj_key in key.start:
-                data_list.append(self._data_list[self._names.index(obj_key)])
-                names.append(obj_key)
-        elif type(key.start) is int or type(key.stop) is int or type(key.step) is int:
-            data_list = self._data_list[key]
-            names = self._names[key]
-        elif key == slice(None):
+        for ki in key_idx_list:
+            if isinstance(ki, (str, np.str_)):
+                data_list.append(self._name_dict[ki])
+                names.append(ki)
+            elif isinstance(ki, (int, np.integer)):
+                ki = int(ki)
+                data_list.append(self._data_list[ki])
+                names.append(self._names[ki])
+            elif isinstance(ki, (list, tuple, np.ndarray, pd.Index)):
+                temp_data_list, temp_names = self.__get_data_list(ki)
+                data_list.extend(temp_data_list)
+                names.extend(temp_names)
+            else:
+                raise KeyError(ki)
+        return data_list, names
+    
+    def __check_slice(self, slice_obj: slice):
+        if not isinstance(slice_obj, slice):
+            raise TypeError(f'{slice_obj} should be slice')
+        if slice_obj.start is not None and isinstance(slice_obj.start, (str, np.str_)):
+            if slice_obj.start in self._name_dict:
+                new_start = self._names.index(slice_obj.start)
+            else:
+                new_start = None
+        else:
+            new_start = slice_obj.start
+        if slice_obj.stop is not None and isinstance(slice_obj.stop, (str, np.str_)):
+            if slice_obj.stop in self._name_dict:
+                new_stop = self._names.index(slice_obj.stop)
+            else:
+                new_stop = None
+        else:
+            new_stop = slice_obj.stop
+
+        if slice_obj.step is not None and not isinstance(slice_obj.step, (int, np.integer)):
+            raise TypeError(f'slice.step should be int')
+        
+        return slice(new_start, new_stop, slice_obj.step)
+    
+
+    def __getitem__(self, key: Union[str, int, list, tuple, np.ndarray, pd.Index, slice]) -> Union[StereoExpData, _MSDataView]:
+        if isinstance(key, (str, np.str_)):
+            return self._name_dict[key]
+        elif isinstance(key, (int, np.integer)):
+            return self._data_list[key]
+        elif isinstance(key, (list, tuple, np.ndarray, pd.Index)):
+            data_list, names = self.__get_data_list(key)
+            return _MSDataView(_msdata=self._msdata, _data_list=data_list, _names=names)
+        elif isinstance(key, slice):
+            key = self.__check_slice(key)
             data_list = self._data_list[key]
             names = self._names[key]
+            return _MSDataView(_msdata=self._msdata, _data_list=data_list, _names=names)
         else:
-            raise TypeError(f'{key} is slice but not in rules')
-        return _MSDataView(_data_list=data_list, _names=names)
+            raise KeyError(key)
 
     @property
     def tl(self):
         if self._tl is None:
             self._tl = TL(self)
         return self._tl
 
@@ -52,43 +100,74 @@
         if self._plt is None:
             self._plt = PLT(self)
         return self._plt
 
     @property
     def data_list(self):
         return self._data_list
+    
+    @property
+    def names(self):
+        return self._names
+    
+    @property
+    def num_slice(self):
+        return len(self._data_list)
 
     def __str__(self):
         return f'''data_list: {len(self._data_list)}'''
+    
+    def __len__(self):
+        return len(self._data_list)
 
     @property
     def merged_data(self):
+        if self._merged_data is None:
+            self._merged_data = self._msdata.integrate(scope=self._names)
         return self._merged_data
+    
+    @merged_data.setter
+    def merged_data(self, merged_data):
+        self._merged_data = merged_data
 
-    def integrate(self, reorganize_coordinate=False, **kwargs):
-        from stereo.utils.data_helper import merge
-        if "result" not in kwargs:
-            raise Exception("_MSDataView.integrate requires a upstream ms_data.tl.result object")
-
-        self.tl.result = kwargs["result"]
-        del kwargs["result"]
-
-        if len(self._data_list) > 1:
-            self._merged_data = merge(*self.data_list, reorganize_coordinate=reorganize_coordinate, **kwargs)
-        else:
-            from copy import deepcopy
-            self._merged_data = deepcopy(self._data_list[0])
-
-        obs_columns = self._merged_data.cells._obs.columns.tolist()
-        obs_columns.remove('batch')
-        if len(obs_columns) > 0:
-            self._merged_data.cells._obs.drop(columns=obs_columns, inplace=True)
-        var_columns = self._merged_data.genes._var.columns.tolist()
-        if len(var_columns) > 0:
-            self._merged_data.genes._var.drop(columns=var_columns, inplace=True)
+    # def integrate(self, reorganize_coordinate=False, **kwargs):
+    #     from stereo.utils.data_helper import merge
+    #     if "result" not in kwargs:
+    #         raise Exception("_MSDataView.integrate requires a upstream ms_data.tl.result object")
+
+    #     self.tl.result = kwargs["result"]
+    #     del kwargs["result"]
+
+    #     if 'var_type' in kwargs:
+    #         del kwargs['var_type']
+
+    #     if len(self._data_list) > 1:
+    #         self._merged_data = merge(*self.data_list, reorganize_coordinate=reorganize_coordinate, var_type=self._msdata._var_type, **kwargs)
+    #     else:
+    #         # from copy import deepcopy
+    #         self._merged_data = deepcopy(self._data_list[0])
+
+    #     obs_columns = self._merged_data.cells._obs.columns.drop('batch')
+    #     if len(obs_columns) > 0:
+    #         self._merged_data.cells._obs.drop(columns=obs_columns, inplace=True)
+    #     var_columns = self._merged_data.genes._var.columns
+    #     if 'real_gene_name' in var_columns:
+    #         var_columns.drop('real_gene_name')
+    #     if len(var_columns) > 0:
+    #         self._merged_data.genes._var.drop(columns=var_columns, inplace=True)
+    
+    def to_msdata(self) -> MSData:
+        return MSData(
+            _data_list=deepcopy(self._data_list),
+            _merged_data=deepcopy(self._merged_data),
+            _names=deepcopy(self._names),
+            _var_type=self._msdata._var_type,
+            _relationship=self._msdata._relationship,
+            _relationship_info=deepcopy(self._msdata._relationship_info)
+        )
 
 
 _NON_EDITABLE_ATTRS = {'data_list', 'names', '_obs', '_var', '_relationship', '_relationship_info'}
 _RELATIONSHIP_ENUM = {'continuous', 'time_series', 'other'}
 
 
 @dataclass
@@ -239,16 +318,26 @@
     def names(self):
         return self._names
 
     @names.setter
     def names(self, value: List[str]):
         if len(value) != len(self._data_list):
             raise Exception('new names\' length should be same as data_list')
-        self._names = value
+        self._names = list(value)
         self.reset_name(default_key=False)
+    
+    @property
+    def var_type(self):
+        return self._var_type
+    
+    @var_type.setter
+    def var_type(self, value: str):
+        if value not in {'intersect', 'union'}:
+            raise Exception(f'new var_type must be in {"intersect", "union"}')
+        self._var_type = value
 
     @property
     def relationship(self):
         return self._relationship
 
     @relationship.setter
     def relationship(self, value: str):
@@ -273,44 +362,90 @@
     def __copy__(self) -> object:
         # TODO temporarily can not copy、deepcopy, return self
         return self
 
     def __deepcopy__(self, _) -> object:
         return self
 
-    def __getitem__(self, key: Union[str, int, slice]) -> Union[StereoExpData, _MSDataView]:
-        if type(key) is int:
-            idx = key
-            return self._data_list[idx]
-        elif type(key) is str:
-            return self._name_dict[key]
-        elif type(key) is slice:
-            data_list = []
-            names = []
-            if type(key.start) is tuple or type(key.start) is list:
-                for obj_key in key.start:
-                    data_list.append(self._name_dict[obj_key])
-                    names.append(obj_key)
-            elif type(key.start) is int or type(key.stop) is int or type(key.step) is int:
-                data_list = self._data_list[key]
-                names = self._names[key]
-            elif key == slice(None):
-                data_list = self._data_list[key]
-                names = self._names[key]
+    def get_data_list(self, key_idx_list):
+        data_list = []
+        names = []
+        for ki in key_idx_list:
+            if isinstance(ki, (str, np.str_)):
+                data_list.append(self._name_dict[ki])
+                names.append(ki)
+            elif isinstance(ki, (int, np.integer)):
+                ki = int(ki)
+                data_list.append(self._data_list[ki])
+                names.append(self._names[ki])
+            elif isinstance(ki, (list, tuple, np.ndarray, pd.Index)):
+                temp_data_list, temp_names = self.get_data_list(ki)
+                data_list.extend(temp_data_list)
+                names.extend(temp_names)
+            else:
+                raise KeyError(ki)
+        return data_list, names
+    
+    def __check_slice(self, slice_obj: slice):
+        if not isinstance(slice_obj, slice):
+            raise TypeError(f'{slice_obj} should be slice')
+        if slice_obj.start is not None and isinstance(slice_obj.start, (str, np.str_)):
+            if slice_obj.start in self._name_dict:
+                new_start = self._names.index(slice_obj.start)
+            else:
+                new_start = None
+        else:
+            new_start = slice_obj.start
+        if slice_obj.stop is not None and isinstance(slice_obj.stop, (str, np.str_)):
+            if slice_obj.stop in self._name_dict:
+                new_stop = self._names.index(slice_obj.stop)
             else:
-                raise TypeError(f'{key} is slice but not in rules')
-            return _MSDataView(_data_list=data_list, _names=names)
-        raise TypeError(f'{key} is not one of Union[str, int]')
+                new_stop = None
+        else:
+            new_stop = slice_obj.stop
+
+        if slice_obj.step is not None and not isinstance(slice_obj.step, (int, np.integer)):
+            raise TypeError(f'slice.step should be int')
+        
+        return slice(new_start, new_stop, slice_obj.step)
+
+    def __getitem__(self, key: Union[str, int, list, tuple, np.ndarray, pd.Index, slice]) -> Union[StereoExpData, _MSDataView]:
+        if isinstance(key, (str, np.str_)):
+            return self._name_dict[key]
+        elif isinstance(key, (int, np.integer)):
+            return self._data_list[key]
+        elif isinstance(key, (list, tuple, np.ndarray, pd.Index)):
+            data_list, names = self.get_data_list(key)
+            return _MSDataView(_msdata=self, _data_list=data_list, _names=names)
+        elif isinstance(key, slice):
+            key = self.__check_slice(key)
+            data_list = self._data_list[key]
+            names = self._names[key]
+            return _MSDataView(_msdata=self, _data_list=data_list, _names=names)
+        else:
+            raise KeyError(key)
+        
 
     def __setitem__(self, key, value):
-        assert isinstance(key, str)
+        assert isinstance(key, (int, np.integer, str, np.str_))
         assert isinstance(value, StereoExpData)
+
         if key in self._name_dict:
-            self.del_data(key)
-        self.__real_add(value, key)
+            key = self._names.index(key)
+        if isinstance(key, (int, np.integer)):
+            if key >= self.num_slice:
+                raise IndexError("list index out of range")
+            old_obj = self._data_list[key]
+            name = self._names[key]
+            self._data_list[key] = value
+            self._name_dict[name] = value
+            self._data_dict.pop(id(old_obj))
+            self._data_dict[id(value)] = name
+        else:
+            self.__real_add(value, key)
 
     def __add__(self, other):
         assert isinstance(other, StereoExpData)
         self.__real_add(other)
         return self
 
     def __contains__(self, item) -> bool:
@@ -468,59 +603,152 @@
         return self
 
     def reset_name(self, start_idx=None, default_key=True) -> object:
         # if self.data_list is n, O(3n)
         self.__idx_generator = _default_idx() if start_idx is None else start_idx
         self._name_dict, self._data_dict = dict(), dict()
         for idx, obj in enumerate(self._data_list):
-            self._name_dict[self.__get_auto_key() if default_key else self._names[idx]] = obj
-        for name, obj in self._name_dict.items():
+            name = self.__get_auto_key() if default_key else self._names[idx]
+            self._name_dict[name] = obj
             self._data_dict[id(obj)] = name
-        self._names = []
-        for obj in self._data_list:
-            self._names.append(self._data_dict[id(obj)])
+            self._names[idx] = name
+        if len(self._data_list) < len(self._names):
+            self._names = self._names[0:len(self._data_list)]
         return self
 
 
 @dataclass
 class MSData(_MSDataStruct):
     __doc__ = _MSDataStruct.__doc__
 
     _tl = None
     _plt = None
+    _scopes_data: Dict[str, StereoExpData] = field(default_factory=dict)
 
     @property
     def tl(self):
         if self._tl is None:
             self._tl = TL(self)
         return self._tl
 
     @property
     def plt(self):
         if self._plt is None:
             self._plt = PLT(self)
         return self._plt
+    
+    @property
+    def scopes_data(self):
+        return self._scopes_data
+    
+    @scopes_data.setter
+    def scopes_data(self, value):
+        self._scopes_data = value
 
     @property
     def mss(self):
         return self.tl.result
 
-    def integrate(self, reorganize_coordinate=False, **kwargs):
+    def generate_scope_key(self, scope=None):
+        if scope is None:
+            scope = slice(None)
+        scope_key = scope
+        try:
+            if isinstance(scope, (int, np.integer)):
+                scope_key = f"scope_[{scope}]"
+            elif isinstance(scope, (str, np.str_)):
+                if scope in self._name_dict:
+                    scope_key = f"scope_[{self._names.index(scope)}]"
+                else:
+                    scope_key = scope
+            elif isinstance(scope, slice):
+                names = self[scope]._names
+                scope_key = f"scope_[{','.join([str(self._names.index(name)) for name in names])}]"  # noqa
+            elif isinstance(scope, (list, tuple, np.ndarray, pd.Index)):
+                _, names = self.get_data_list(scope)
+                scope_key = f"scope_[{','.join([str(self._names.index(name)) for name in names])}]"  # noqa
+        except:
+            scope_key = scope
+        finally:
+            return scope_key
+    
+    def remove_scopes_data(self, scope):
+        scope_key = self.generate_scope_key(scope)
+        if scope_key in self._scopes_data:
+            del self._scopes_data[scope_key]
+        if scope_key in self.tl.result_keys:
+            del self.tl.result_keys[scope_key]
+
+
+    def integrate(self, scope=None, remove_existed=False, **kwargs):
+        """
+        Integrate some single-samples specified by `scope` to a merged one.
+        
+        :param scope: Which scope of samples to be integrated, defaults to None.
+                        Each integrate sample is saved in memory, performing this function
+                        by passing duplicate `scope` will return the saved one.
+        :param remove_existed: Whether to remove the saved integrate sample when passing a duplicate `scope`, defaults to False.
+
+        """
         from stereo.utils.data_helper import merge
         if self._var_type not in {"union", "intersect"}:
             raise Exception("Please specify the operation on samples with the parameter '_var_type'")
-        self.merged_data = merge(*self.data_list, var_type=self._var_type, reorganize_coordinate=reorganize_coordinate,
-                                 **kwargs)
-        obs_columns = self.merged_data.cells._obs.columns.tolist()
-        obs_columns.remove('batch')
+        
+        if 'var_type' in kwargs:
+            del kwargs['var_type']
+        if 'batch_tags' in kwargs:
+            del kwargs['batch_tags']
+        
+        if remove_existed:
+            self.remove_scopes_data(scope)
+        scope_key = self.generate_scope_key(scope)
+        if scope_key in self._scopes_data:
+            return self._scopes_data[scope_key]
+        
+        if scope == None:
+            data_list = self.data_list
+        else:
+            data_list = self[scope].data_list
+        if len(data_list) > 1:
+            if scope is None:
+                batch_tags = None
+            else:
+                batch_tags = [self._names.index(name) for name in self[scope].names]
+            merged_data = merge(*data_list, var_type=self._var_type, batch_tags=batch_tags)
+        else:
+            merged_data = deepcopy(data_list[0])
+            batch = self._names.index(self[scope].names[0])
+            merged_data.cells.cell_name = np.char.add(merged_data.cells.cell_name, f'-{batch}')
+            merged_data.cells.batch = batch
+        
+        obs_columns = merged_data.cells._obs.columns.drop('batch')
         if len(obs_columns) > 0:
-            self.merged_data.cells._obs.drop(columns=obs_columns, inplace=True)
-        var_columns = self.merged_data.genes._var.columns.tolist()
+            merged_data.cells._obs.drop(columns=obs_columns, inplace=True)
+        var_columns = merged_data.genes._var.columns
+        if 'real_gene_name' in var_columns:
+            var_columns.drop('real_gene_name')
         if len(var_columns) > 0:
-            self.merged_data.genes._var.drop(columns=var_columns, inplace=True)
+            merged_data.genes._var.drop(columns=var_columns, inplace=True)
+        
+        def set_result_key_method(key):
+            self.tl.result_keys.setdefault(scope_key, [])
+            if key in self.tl.result_keys[scope_key]:
+                self.tl.result_keys[scope_key].remove(key)
+            self.tl.result_keys[scope_key].append(key)
+        
+        merged_data.tl.result.set_result_key_method = set_result_key_method
+        
+        scope_key = self.generate_scope_key(scope)
+        self._scopes_data[scope_key] = merged_data
+
+        if scope == None or scope == slice(None):
+            self._merged_data = merged_data
+
+        return merged_data
+
 
     def split_after_batching_integrate(self):
         if self._var_type == "union":
             raise NotImplementedError("Split a union data not implemented yet")
         from stereo.utils.data_helper import split
         self._data_list = split(self.merged_data)
         self.reset_name(default_key=False)
@@ -528,34 +756,34 @@
 
     def to_integrate(
             self,
             scope: slice,
             res_key: str,
             _from: slice,
             type: Literal['obs', 'var'] = 'obs',
-            item: Optional[list] = None,
+            item: Optional[Union[list, np.ndarray, str]] = None,
             fill=np.NaN,
             cluster: bool = True
     ):
         """
         Integrate an obs column or a var column from some single-samples spcified by `_from` to the merged sample. 
 
         :param scope: Which integrate mss group to save result.
         :param res_key: New column name in merged sample obs or var.
         :param _from: Where to get the single-sample target infomation.
-        :param type: obs or var level, defaults to 'obs'
-        :param item: The column names in single-sample obs or var, defaults to None
-        :param fill: Default value when the merged sample has no conrresponding item, defaults to np.NaN
-        :param cluster: Whether it is a clustering result, defaults to True
+        :param type: obs or var level, defaults to 'obs'.
+        :param item: The column names in single-sample obs or var, defaults to the value of `res_key`.
+        :param fill: Default value when the merged sample has no conrresponding item, defaults to np.NaN.
+        :param cluster: Whether it is a clustering result, defaults to True.
 
         .. note::
 
             The length of `scope` must be equal to `_from`.
 
-            The `type` just only supports 'obs' now.
+            The `type` just only supports 'obs' currently.
         
         Examples
         --------
         Constructing MSData from 5 single-samples.
 
         >>> import stereo as st
         >>> data1 = st.io.read_h5ad('../data/10.h5ad')
@@ -585,76 +813,95 @@
 
         Integrating an obs column named as 'celltype' from all samples to the merged sample, to name as 'celltype'
 
         >>> from stereo.core.ms_pipeline import slice_generator
         >>> ms_data.to_integrate(res_key='celltype', scope=slice_generator[:], _from=slice_generator[:], type='obs', item=['celltype'] * ms_data.num_slice)
 
         """
-        assert self.merged_data, "`to_integrate` need running function `integrate`"
-        assert self._names[scope] == self._names[_from], f"`scope`: {scope} should equal with _from: {_from}"
-        assert len(item) == len(self._names[_from]), "`item`'s length not equal to _from"
-        scope_names = self._names[scope]
+        # assert self.merged_data, "`to_integrate` need running function `integrate`"
+        # assert self._names[scope] == self._names[_from], f"`scope`: {scope} should equal with _from: {_from}"
+        # assert len(item) == len(self._names[_from]), "`item`'s length not equal to _from"
+        # scope_names = self._names[scope]
+        assert self[scope]._names == self[_from]._names, f"`scope`: {scope} should equal with _from: {_from}"
+        assert isinstance(item, str) or len(item) == len(self[_from]._names), "`item`'s length not equal to _from"
+        scope_names = self[scope]._names
+        scope_key = self.generate_scope_key(scope_names)
+        assert scope_key in self._scopes_data or self._merged_data, f"`to_integrate` need running function `integrate` first"
         if type == 'obs':
-            self.merged_data.cells._obs[res_key] = fill
+            if scope_key in self._scopes_data:
+                self._scopes_data[scope_key].cells[res_key] = fill
+            
+            if self._merged_data is not None:
+                self._merged_data.cells[res_key] = fill
         elif type == 'var':
             raise NotImplementedError
         else:
             raise Exception(f"`type`: {type} not in ['obs', 'var'], this should not happens!")
-
-        for idx, stereo_exp_data in enumerate(self._data_list[scope]):
+        
+        # for idx, stereo_exp_data in enumerate(self._data_list[scope]):
+        data_list = self[scope]._data_list
+        if item is None:
+            item = res_key
+        if isinstance(item, str):
+            item = [item] * len(data_list)
+        for idx, stereo_exp_data in enumerate(data_list):
             if type == 'obs':
-                res = stereo_exp_data.cells._obs[item[idx]]
+                res = stereo_exp_data.cells[item[idx]]
                 sample_idx = self._names.index(scope_names[idx])
                 new_index = res.index.astype('str') + f'-{sample_idx}'
                 # res.index = new_index
-                self.merged_data.cells._obs.loc[new_index, res_key] = res.to_numpy()
+                if scope_key in self._scopes_data:
+                    self._scopes_data[scope_key].cells.loc[new_index, res_key] = res.to_numpy()
+                
+                if self._merged_data is not None:
+                    self._merged_data.cells.loc[new_index, res_key] = res.to_numpy()
             elif type == 'var':
                 raise NotImplementedError
             else:
                 raise Exception(f"`type`: {type} not in ['obs', 'var'], this should not happens!")
         if type == 'obs':
-            scope_key_name = "scope_[" + ",".join([str(self._names.index(name)) for name in scope_names]) + "]"
-            self.tl.result.setdefault(scope_key_name, {})
             if cluster:
-                self.tl.result[scope_key_name][res_key] = pd.DataFrame({
-                    'bins': self.merged_data.cell_names,
-                    'group': self.merged_data.cells._obs[res_key].astype('category')
-                })
-                self.tl.result[scope_key_name][res_key].index = np.arange(self.merged_data.cell_names.size)
-            else:
-                self.tl.result[scope_key_name][res_key] = self.merged_data.cells._obs[res_key].to_frame()
+                if scope_key in self._scopes_data:
+                    self._scopes_data[scope_key].tl.reset_key_record('cluster', res_key)
+                    self._scopes_data[scope_key].tl.result.set_result_key_method(res_key)
+
+                if self._merged_data is not None:
+                    self._merged_data.tl.reset_key_record('cluster', res_key)
+                    self._merged_data.tl.result.set_result_key_method(res_key)
         elif type == 'var':
             raise NotImplementedError
         else:
             raise Exception(f"`type`: {type} not in ['obs', 'var'], this should not happens!")
 
     def to_isolated(
             self,
             scope: slice,
             res_key: str,
             to: slice,
             type: Literal['obs', 'var'] = 'obs',
-            item: Optional[list] = None,
+            item: Optional[Union[list, np.ndarray, str]] = None,
             fill=np.NaN
     ):
         """
         Copy a result from mss group specfied by scope to some single-samples specfied by `to`.
 
         :param scope: Which integrate mss group to get result.
         :param res_key: the key to get result from mms group.
         :param to: which single-samples are the result copy to.
         :param type: obs or var level, defaults to 'obs'
-        :param item: New column name in obs or var of single-sample, defaults to None
+        :param item: New column name in obs of single-sample, defaults to the value of `res_key`.
         :param fill: Default value when the single-sample has no conrresponding item, defaults to np.NaN
 
         .. note::
 
             The length of `scope` must be equal to `to`.
             
             Only supports clustering result when `type` is 'obs' and hvg result when `type` is 'var'.
+
+            Parameter `item` only available for obs type.
         
         Examples
         --------
         Constructing MSData from 5 single-samples.
 
         >>> import stereo as st
         >>> data1 = st.io.read_h5ad('../data/10.h5ad')
@@ -688,46 +935,57 @@
         Copy the 'leiden' result to all samples, to name as 'leiden'.
 
         >>> from stereo.core.ms_pipeline import slice_generator
         >>> ms_data.to_isolated(scope=slice_generator[:], res_key='leiden', to=slice_generator[:], type='obs', item=['leiden'] * 3)
         
         
         """
-        assert self.merged_data, "`to_integrate` need running function `integrate`"
-        assert self._names[scope] == self._names[to], f"`scope`: {scope} should equal with to: {to}"
-        assert len(item) == len(self._names[to]), "`item`'s length not equal to `to`"
-
-        scope_names = self._names[scope]
-        scope_key_name = "scope_[" + ",".join([str(self._names.index(name)) for name in scope_names]) + "]"
-        merged_res = self.tl.result[scope_key_name][res_key].copy(deep=True)
+        # assert self.merged_data, "`to_integrate` need running function `integrate`"
+        # assert self._names[scope] == self._names[to], f"`scope`: {scope} should equal with to: {to}"
+        # assert len(item) == len(self._names[to]), "`item`'s length not equal to `to`"
+        assert self[scope]._names == self[to]._names, f"`scope`: {scope} should equal with to: {to}"
+        assert isinstance(item, str) or len(item) == len(self[to]._names), "`item`'s length not equal to `to`"
+
+        scope_names = self[scope]._names
+        # scope_key_name = "scope_[" + ",".join([str(self._names.index(name)) for name in scope_names]) + "]"
+        scope_key = self.generate_scope_key(scope_names)
+        merged_res: pd.DataFrame = self.tl.result[scope_key][res_key].copy(deep=True)
         if type == "obs":
             # TODO: only support cluster data
-            if "bins" in merged_res.columns:
-                merged_res.index = merged_res["bins"]
-                del merged_res["bins"]
+            if "bins" not in merged_res.columns or "group" not in merged_res.columns:
+                raise Exception("Only soupport cluster result currently.")
+            merged_res.index = merged_res.apply(lambda row: row['bins'].rsplit('-', 1)[0], axis=1)
         elif type == "var":
             # TODO: only support hvg data
-            if res_key == "highly_variable_genes":
-                res_key = 'highly_variable'
-                merged_res = merged_res[res_key].to_frame()
+            merged_res.index = self._scopes_data[scope_key].genes.gene_name
 
-        for idx, stereo_exp_data in enumerate(self._data_list[scope]):
+        # for idx, stereo_exp_data in enumerate(self._data_list[scope]):
+        data_list = self[scope]._data_list
+        if item is None:
+            item = res_key
+        if isinstance(item, str):
+            item = [item] * len(data_list)
+        for idx, stereo_exp_data in enumerate(data_list):
             if type == 'obs':
-                sample_idx = self._names.index(scope_names[idx])
-                new_index = stereo_exp_data.cells._obs.index.astype('str') + f'-{sample_idx}'
-                bak_index = stereo_exp_data.cells._obs.index
-                stereo_exp_data.cells._obs.index = new_index
-                obs_bool_list = np.isin(merged_res.index.values, new_index.values)
-                stereo_exp_data.cells._obs.insert(0, item[idx], merged_res[obs_bool_list])
-                stereo_exp_data.cells._obs.index = bak_index
-            elif type == 'var':
-                obs_bool_list = np.isin(merged_res.index.values, stereo_exp_data.genes._var.index.values)
-                stereo_exp_data.genes._var.insert(0, item[idx], merged_res[obs_bool_list])
+                column_name = item[idx]
+                stereo_exp_data.cells._obs[column_name] = merged_res['group']
                 if fill is not np.NaN:
-                    stereo_exp_data.genes._var[stereo_exp_data.genes._var[res_key].values == np.NaN] = fill
+                    if stereo_exp_data.cells._obs[column_name].dtype.name == 'category':
+                        stereo_exp_data.cells._obs[column_name].cat.remove_unused_categories(inplace=True)
+                        stereo_exp_data.cells._obs[column_name].cat.add_categories(fill, inplace=True)
+                    stereo_exp_data.cells._obs[column_name].fillna(fill, inplace=True)
+            elif type == 'var':
+            
+                for column_name in merged_res.columns:
+                    stereo_exp_data.genes._var[column_name] = merged_res[column_name]
+                    if fill is not np.NaN:
+                        if stereo_exp_data.genes._var[column_name].dtype.name == 'category':
+                            stereo_exp_data.genes._var[column_name].cat.remove_unused_categories(inplace=True)
+                            stereo_exp_data.genes._var[column_name].cat.add_categories(fill, inplace=True)
+                        stereo_exp_data.genes._var[column_name].fillna(fill, inplace=True)
             else:
                 raise Exception(f"`type`: {type} not in ['obs', 'var'], this should not happens!")
             
     @staticmethod
     def to_msdata(
         data: StereoExpData,
         batch_key: str = 'batch',
@@ -756,15 +1014,15 @@
         return f'''ms_data: {self.shape}
 num_slice: {self.num_slice}
 names: {self.names}
 obs: {self.obs.columns.to_list()}
 var: {self.var.columns.to_list()}
 relationship: {self.relationship}
 var_type: {self._var_type} to {len(self.var.index)}
-mss: {[key + ":" + str(list(self.tl.result[key].keys())) for key in self.tl.result.keys()]}
+mss: {[key + ":" + str(value) for key, value in self.tl.result_keys.items()]}
 '''
 
     def __repr__(self):
         return self.__str__()
 
 
 TL = type('TL', (MSDataPipeLine,), {'ATTR_NAME': 'tl', "BASE_CLASS": StPipeline})
```

### Comparing `stereopy-1.2.0/stereo/core/ms_pipeline.py` & `stereopy-1.3.0b1/stereo/core/ms_pipeline.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,120 +1,155 @@
 import os
 from joblib import (
     Parallel,
     delayed,
     cpu_count
 )
 
-from stereo import logger
+import numpy as np
+
+from stereo.log_manager import logger
 from stereo.core import StPipeline
+from stereo.core.result import MSDataPipeLineResult
 from stereo.plots.decorator import download, download_only
 
 
 class _scope_slice(object):
 
     def __getitem__(self, item):
-        if type(item) is slice:
+        if isinstance(item, (int, np.integer, str, np.str_)):
+            return [item]
+        else:
             return item
 
 
 class MSDataPipeLine(object):
     ATTR_NAME = 'tl'
     BASE_CLASS = StPipeline
 
     def __init__(self, _ms_data):
         super().__init__()
         self.ms_data = _ms_data
-        self._result = dict()
+        self._result = MSDataPipeLineResult(self.ms_data)
+        self._result_keys = dict()
         self._key_record = dict()
-        # self._scope_data = dict()
+        self.__mode = "integrate"
+        self.__scope = slice(None)
 
     @property
     def result(self):
         return self._result
 
-    @result.setter
-    def result(self, new_result):
-        self._result = new_result
+    # @result.setter
+    # def result(self, new_result):
+    #     self._result = new_result
 
     @property
     def key_record(self):
         return self._key_record
 
     @key_record.setter
     def key_record(self, key_record):
         self._key_record = key_record
-
-    # @property
-    # def scope_data(self):
-    #     return self._scope_data
+    
+    @property
+    def result_keys(self):
+        return self._result_keys
+    
+    @result_keys.setter
+    def result_keys(self, result_keys):
+        self._result_keys = result_keys
+        self._reset_result_keys()
+    
+    @property
+    def mode(self):
+        return self.__mode
+    
+    @mode.setter
+    def mode(self, mode):
+        self.__mode = mode
+    
+    @property
+    def scope(self):    
+        return self.__scope
+    
+    @scope.setter
+    def scope(self, scope):
+        self.__scope = scope
+    
+    def _reset_result_keys(self):
+        for scope_key, result_keys in self._result_keys.items():
+            self._result_keys[scope_key] = []
+            for rk in result_keys:
+                if rk in self.result[scope_key]:
+                    self._result_keys[scope_key].append(rk)
 
     def _use_integrate_method(self, item, *args, **kwargs):
         if "mode" in kwargs:
             del kwargs["mode"]
 
         scope = kwargs.get("scope", slice(None))
         del kwargs["scope"]
 
-        if item in {"cal_qc", "filter_cells", "filter_genes", "sctransform", "log1p", "normalize_total",
-                    "scale", "raw_checkpoint", "batches_integrate"}:
-            if scope != slice(None):
-                raise Exception(f'{item} use integrate should use all sample')
-            ms_data_view = self.ms_data
-        elif scope == slice(None):
+        # if item in {"cal_qc", "filter_cells", "filter_genes", "sctransform", "log1p", "normalize_total",
+        #             "scale", "raw_checkpoint", "batches_integrate"}:
+        #     if scope != slice(None):
+        #         raise Exception(f'{item} use integrate should use all sample')
+        #     ms_data_view = self.ms_data
+        # elif scope == slice(None):
+        if len(self.ms_data[scope]) == len(self.ms_data):
             ms_data_view = self.ms_data
+            if ms_data_view.merged_data is None:
+                ms_data_view.integrate()
         else:
             ms_data_view = self.ms_data[scope]
-        if not ms_data_view.merged_data:
-            ms_data_view.integrate(result=self.ms_data.tl.result)
 
-        # key_name = "scope_[" + ",".join(
-        #     [str(self.ms_data._names.index(name)) for name in ms_data_view._names]) + "]"
-        # self._scope_data[key_name] = self.ms_data._merged_data
-
-        def callback_func(key, value):
-            key_name = "scope_[" + ",".join(
-                [str(self.ms_data._names.index(name)) for name in ms_data_view._names]) + "]"
-            self.ms_data.tl.result.setdefault(key_name, {})
-            self.ms_data.tl.result[key_name][key] = value
-
-        ms_data_view._merged_data.tl.result.set_item_callback = callback_func
-
-        def get_item_method(name):
-            key_name = "scope_[" + ",".join(
-                [str(self.ms_data._names.index(name)) for name in ms_data_view._names]) + "]"
-            scope_result = self.ms_data.tl.result.get(key_name, None)
-            if scope_result is None:
-                raise KeyError
-            method_result = scope_result.get(name, None)
-            return method_result
-
-        ms_data_view._merged_data.tl.result.get_item_method = get_item_method
-
-        def contain_method(item):
-            key_name = "scope_[" + ",".join(
-                [str(self.ms_data._names.index(name)) for name in ms_data_view._names]) + "]"
-            scope_result = self.ms_data.tl.result.get(key_name, None)
-            if scope_result is None:
-                return False
-            method_result = scope_result.get(item, None)
-            if method_result is None:
-                return False
-            return True
-
-        ms_data_view._merged_data.tl.result.contain_method = contain_method
-
-        def reset_key_record(key, res_key):
-            key_name = "scope_[" + ",".join(
-                [str(self.ms_data._names.index(name)) for name in ms_data_view._names]) + "]"
+        scope_key = self.ms_data.generate_scope_key(ms_data_view._names)
+        self.ms_data.scopes_data[scope_key] = ms_data_view.merged_data
 
-            ms_data_view._merged_data.tl._reset_key_record(key, res_key)
-            self._key_record[key_name] = ms_data_view._merged_data.tl.key_record
+        # def callback_func(key, value):
+        #     # key_name = "scope_[" + ",".join(
+        #     #     [str(self.ms_data._names.index(name)) for name in ms_data_view._names]) + "]"
+        #     self.ms_data.tl.result.setdefault(key_name, {})
+        #     self.ms_data.tl.result[key_name][key] = value
+
+        # ms_data_view._merged_data.tl.result.set_item_callback = callback_func
+
+        # def get_item_method(name):
+        #     # key_name = "scope_[" + ",".join(
+        #     #     [str(self.ms_data._names.index(name)) for name in ms_data_view._names]) + "]"
+        #     scope_result = self.ms_data.tl.result.get(key_name, None)
+        #     if scope_result is None:
+        #         raise KeyError
+        #     method_result = scope_result.get(name, None)
+        #     return method_result
+
+        # ms_data_view._merged_data.tl.result.get_item_method = get_item_method
+
+        # def contain_method(item):
+        #     # key_name = "scope_[" + ",".join(
+        #     #     [str(self.ms_data._names.index(name)) for name in ms_data_view._names]) + "]"
+        #     scope_result = self.ms_data.tl.result.get(key_name, None)
+        #     if scope_result is None:
+        #         return False
+        #     method_result = scope_result.get(item, None)
+        #     if method_result is None:
+        #         return False
+        #     return True
+
+        # ms_data_view._merged_data.tl.result.contain_method = contain_method
+
+        # def reset_key_record(key, res_key):
+        #     # key_name = "scope_[" + ",".join(
+        #     #     [str(self.ms_data._names.index(name)) for name in ms_data_view._names]) + "]"
 
-        ms_data_view._merged_data.tl.reset_key_record = reset_key_record
+        #     ms_data_view._merged_data.tl._reset_key_record(key, res_key)
+        #     self._key_record[key_name] = ms_data_view._merged_data.tl.key_record
+
+        # ms_data_view._merged_data.tl.reset_key_record = reset_key_record
 
         new_attr = self.__class__.BASE_CLASS.__dict__.get(item, None)
         if new_attr is None:
             if self.__class__.ATTR_NAME == "tl":
                 from stereo.algorithm.algorithm_base import AlgorithmBase
                 merged_data = ms_data_view.merged_data
                 new_attr = AlgorithmBase.get_attribute_helper(item, merged_data, merged_data.tl.result)
@@ -212,38 +247,73 @@
         if self.__class__.ATTR_NAME == 'tl':
             from stereo.algorithm.ms_algorithm_base import MSDataAlgorithmBase
             run_method = MSDataAlgorithmBase.get_attribute_helper(item, self.ms_data, self.result)
             if run_method:
                 return run_method
         elif self.__class__.ATTR_NAME == 'plt':
             from stereo.plots.ms_plot_base import MSDataPlotBase
-            run_method = MSDataPlotBase.get_attribute_helper(item, self.ms_data, self.result)
+            run_method = MSDataPlotBase.get_attribute_helper(item, self.ms_data, self.ms_data.tl.result)
             if run_method:
                 return download(run_method)
 
         def temp(*args, **kwargs):
             if "scope" not in kwargs:
-                kwargs["scope"] = slice_generator[:]
-            if "mode" in kwargs:
-                if kwargs["mode"] == "integrate":
-                    if self.ms_data.merged_data:
-                        return self._use_integrate_method(item, *args, **kwargs)
-                    else:
-                        raise Exception(
-                            "`mode` integrate should merge first, using `ms_data.integrate`"
-                        )
-                elif kwargs["mode"] == "isolated":
-                    self._run_isolated_method(item, *args, **kwargs)
-                else:
-                    raise Exception("`mode` should be one of [`integrate`, `isolated`]")
+                # kwargs["scope"] = slice_generator[:]
+                kwargs["scope"] = self.__scope
+            if "mode" not in kwargs:
+                kwargs["mode"] = self.__mode
+
+            if kwargs["mode"] == "integrate":
+                return self._use_integrate_method(item, *args, **kwargs)
+            elif kwargs["mode"] == "isolated":
+                self._run_isolated_method(item, *args, **kwargs)
             else:
-                if self.ms_data.merged_data:
-                    return self._use_integrate_method(item, *args, **kwargs)
-                else:
-                    raise Exception(
-                        "`mode` integrate should merge first, using `ms_data.integrate`"
-                    )
+                raise Exception("`mode` should be one of [`integrate`, `isolated`]")
+            # if "mode" in kwargs:
+            #     if kwargs["mode"] == "integrate":
+            #         # if self.ms_data.merged_data:
+            #         #     return self._use_integrate_method(item, *args, **kwargs)
+            #         # else:
+            #         #     raise Exception(
+            #         #         "`mode` integrate should merge first, using `ms_data.integrate`"
+            #         #     )
+            #         return self._use_integrate_method(item, *args, **kwargs)
+            #     elif kwargs["mode"] == "isolated":
+            #         self._run_isolated_method(item, *args, **kwargs)
+            #     else:
+            #         raise Exception("`mode` should be one of [`integrate`, `isolated`]")
+            # else:
+            #     # if self.ms_data.merged_data:
+            #     #     return self._use_integrate_method(item, *args, **kwargs)
+            #     # else:
+            #     #     raise Exception(
+            #     #         "`mode` integrate should merge first, using `ms_data.integrate`"
+            #     #     )
+            #     return self._use_integrate_method(item, *args, **kwargs)
 
         return temp
+    
+    def set_scope_and_mode(
+        self,
+        scope: slice = slice(None),
+        mode: str = "integrate"
+    ):
+        """
+        Set the `scope` and `mode` globally for Multi-slice analysis.
+
+        :param scope: the scope, defaults to slice(None)
+        :param mode: the mode, defaults to "integrate"
+        """
+        assert mode in ("integrate", "isolated"), 'mode should be one of [`integrate`, `isolated`]'
+        self.__mode = mode
+        self.__scope = scope
+        if self.__class__.ATTR_NAME == 'tl':
+            self.ms_data.plt.scope = scope
+            self.ms_data.plt.mode = mode
+        elif self.__class__.ATTR_NAME == 'plt':
+            self.ms_data.tl.scope = scope
+            self.ms_data.tl.mode = mode
+        else:
+            pass
 
 
 slice_generator = _scope_slice()
```

### Comparing `stereopy-1.2.0/stereo/core/result.py` & `stereopy-1.3.0b1/stereo/core/result.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from warnings import warn
+from typing import Union
 
 import pandas as pd
 import numpy as np
 from anndata import AnnData
 
+from stereo.core.stereo_exp_data import StereoExpData, AnnBasedStereoExpData
 
 class _BaseResult(object):
     CLUSTER_NAMES = {
         'leiden', 'louvain', 'phenograph', 'annotation', 'leiden_from_bins', 'louvain_from_bins',
         'phenograph_from_bins', 'annotation_from_bins', 'celltype', 'cell_type'
     }
     NOT_CLUSTER_PREFIX = {
@@ -32,42 +34,41 @@
         CLUSTER: CLUSTER_NAMES,
         CONNECTIVITY: CONNECTIVITY_NAMES,
         REDUCE: REDUCE_NAMES,
         HVG: HVG_NAMES,
         MARKER_GENES: MARKER_GENES_NAMES
     }
 
+    def __init__(self):
+        self.set_result_key_method = None
+
+    def __setitem__(self, key, _):
+        if self.set_result_key_method:
+            self.set_result_key_method(key)
+    
 
 class Result(_BaseResult, dict):
 
-    def __init__(self, stereo_exp_data):
-        super().__init__()
+    def __init__(
+        self,
+        stereo_exp_data: Union[StereoExpData, AnnBasedStereoExpData],
+        *args,
+        **kwargs
+    ):
+        # super().__init__()
+        if not isinstance(stereo_exp_data, (StereoExpData, AnnBasedStereoExpData)):
+            raise TypeError("stereo_exp_data must be an object of StereoExpData.")
+        
+        _BaseResult.__init__(self)
+        dict.__init__(self, *args, **kwargs)
         self.__stereo_exp_data = stereo_exp_data
         self.set_item_callback = None
         self.get_item_method = None
         self.contain_method = None
 
-    # def __deepcopy__(self, memo=None, _nil=[]):
-    #     if memo is None:
-    #         memo = {}
-    #     d = id(self)
-    #     y = memo.get(d, _nil)
-    #     if y is not _nil:
-    #         return y
-
-    #     cls = Result(None)
-    #     memo[d] = id(cls)
-    #     cls.__stereo_exp_data = deepcopy(self.__stereo_exp_data, memo)
-    #     cls.set_item_callback = deepcopy(self.set_item_callback, memo)
-    #     cls.get_item_method = deepcopy(self.get_item_method, memo)
-    #     cls.contain_method = deepcopy(self.contain_method, memo)
-    #     for key, value in self.items():
-    #         dict.__setitem__(cls, deepcopy(key, memo), deepcopy(value, memo))
-    #     return cls
-
     def __contains__(self, item):
         if self.contain_method:
             if self.contain_method(item):
                 return True
             # TODO: when get item in ms_data[some_idx].tl.result, if name match the ms_data rule, it is very confused
         if item in self.__stereo_exp_data.genes:
             return True
@@ -164,14 +165,16 @@
         elif type == Result.MARKER_GENES:
             self._set_marker_genes_res(key, value)
         else:
             return False
         return True
 
     def __setitem__(self, key, value):
+        _BaseResult.__setitem__(self, key, value)
+        
         if self.set_item_callback:
             self.set_item_callback(key, value)
             return
         for name_type, name_dict in Result.TYPE_NAMES_DICT.items():
             if key in name_dict and self._real_set_item(name_type, key, value):
                 return
         for name_type, name_dict in Result.TYPE_NAMES_DICT.items():
@@ -359,14 +362,16 @@
         elif type == AnnBasedResult.MARKER_GENES:
             self._set_marker_genes_res(key, value)
         else:
             return False
         return True
 
     def __setitem__(self, key, value):
+        super().__setitem__(key, value)
+
         for name_type, name_dict in AnnBasedResult.TYPE_NAMES_DICT.items():
             if key in name_dict and self._real_set_item(name_type, key, value):
                 return
 
         for name_type, name_dict in AnnBasedResult.TYPE_NAMES_DICT.items():
             for like_name in name_dict:
                 # if not key.startswith('gene_exp_') and like_name in key and self._real_set_item(name_type, key, value):
@@ -506,7 +511,37 @@
                 self.__based_ann_data.obsm[key] = value
             elif (len(value.shape) >= 2) and (value.shape[1] == self.__based_ann_data.shape[1]):
                 self.__based_ann_data.varm[key] = value
             else:
                 self.__based_ann_data.uns[key] = value
         else:
             self.__based_ann_data.uns[key] = value
+
+
+class MSDataPipeLineResult(dict):
+    def __init__(self, _ms_data):
+        self._ms_data = _ms_data
+    
+    def __getitem__(self, key):
+        scope_key = self._ms_data.generate_scope_key(key)
+        if scope_key in self._ms_data.scopes_data:
+            return self._ms_data.scopes_data[scope_key].tl.result
+        else:
+            return dict.__getitem__(self, key)
+
+    def keys(self):
+        super_keys = dict.keys(self)
+        tmp = {}
+        for key in super_keys:
+            tmp[key] = None
+        
+        for key in self._ms_data.tl.result_keys.keys():
+            tmp[key] = None
+        
+        return tmp.keys()
+    
+    def __contains__(self, key: object) -> bool:
+        scope_key = self._ms_data.generate_scope_key(key)
+        if scope_key in self._ms_data.tl.result_keys:
+            return True
+        else:
+            return dict.__contains__(self, key)
```

### Comparing `stereopy-1.2.0/stereo/core/st_pipeline.py` & `stereopy-1.3.0b1/stereo/core/st_pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,35 +195,44 @@
         An object of StereoExpData.
         Depending on `inplace`, if `True`, the data will be replaced by those filtered.
         """
         from ..preprocess.filter import filter_cells
         data = filter_cells(self.data, min_gene, max_gene, min_n_genes_by_counts, max_n_genes_by_counts, pct_counts_mt,
                             cell_list, inplace)
         if data.raw is not None and filter_raw:
-            filter_cells(data.raw, min_gene, max_gene, min_n_genes_by_counts, max_n_genes_by_counts, pct_counts_mt,
-                         cell_list, True)
+            # filter_cells(data.raw, min_gene, max_gene, min_n_genes_by_counts, max_n_genes_by_counts, pct_counts_mt,
+            #              cell_list, True)
+            filter_cells(data.raw, cell_list=data.cell_names, inplace=True)
+            if isinstance(data, AnnBasedStereoExpData):
+                data.adata.raw = data.raw.adata
         return data
 
     @logit
     def filter_genes(self,
                      min_cell: Optional[int] = None,
                      max_cell: Optional[int] = None,
+                     min_count: Optional[int] = None,
+                     max_count: Optional[int] = None,
                      gene_list: Optional[Union[list, np.ndarray]] = None,
                      mean_umi_gt: Optional[float] = None,
                      filter_raw: Optional[bool] = True,
                      inplace: bool = True):
         """
         Filter genes based on the numbers of cells or counts.
 
         Parameters
         ---------------------
         min_cell
             minimum number of cells expressed required for a gene to pass filering.
         max_cell
             maximum number of cells expressed required for a gene to pass filering.
+        min_count
+            minimum number of count expressed required for a gene to pass filtering.
+        max_count
+            maximum number of count expressed required for a gene to pass filtering.
         gene_list
             the list of genes to be retained.
         mean_umi_gt
             genes mean umi should greater than this.
         filter_raw
             whether to filter raw data meanwhile.
         inplace
@@ -231,17 +240,19 @@
 
         Returns
         --------------------
         An object of StereoExpData.
         Depending on `inplace`, if `True`, the data will be replaced by those filtered.
         """
         from ..preprocess.filter import filter_genes
-        data = filter_genes(self.data, min_cell, max_cell, gene_list, mean_umi_gt, inplace)
+        data = filter_genes(self.data, min_cell, max_cell, min_count, max_count, gene_list, mean_umi_gt, inplace)
         if data.raw is not None and filter_raw:
-            filter_genes(data.raw, min_cell, max_cell, gene_list, mean_umi_gt, True)
+            filter_genes(data.raw, gene_list=data.genes.gene_name, inplace=True)
+            if isinstance(data, AnnBasedStereoExpData):
+                data.adata.raw = data.raw.adata
         return data
 
     @logit
     def filter_by_hvgs(self,
                        hvg_res_key: str = 'highly_variable_genes',
                        filter_raw: bool = True,
                        inplace: bool = False):
@@ -264,18 +275,21 @@
         """
         if hvg_res_key not in self.result:
             raise KeyError(f'Can not find result of highly_variable_genes function by key {hvg_res_key}.')
 
         from ..preprocess import filter_genes
         hvgs_flag = self.result[hvg_res_key]['highly_variable'].to_numpy()
         hvgs = self.data.gene_names[hvgs_flag]
+        hvg_result_filtered = self.result[hvg_res_key][hvgs_flag]
         data = filter_genes(self.data, gene_list=hvgs, inplace=inplace)
         if data.raw is not None and filter_raw:
             filter_genes(data.raw, gene_list=hvgs, inplace=True)
-        data.tl.result[hvg_res_key] = data.tl.result[hvg_res_key][hvgs_flag]
+            if isinstance(data, AnnBasedStereoExpData):
+                data.adata.raw = data.raw.adata
+        data.tl.result[hvg_res_key] = hvg_result_filtered
         return data
 
     @logit
     def filter_coordinates(self,
                            min_x: int = None,
                            max_x: int = None,
                            min_y: int = None,
@@ -305,14 +319,16 @@
         An object of StereoExpData.
         Depending on `inplace`, if `True`, the data will be replaced by those filtered.
         """
         from ..preprocess.filter import filter_coordinates
         data = filter_coordinates(self.data, min_x, max_x, min_y, max_y, inplace)
         if data.raw is not None and filter_raw:
             filter_coordinates(data.raw, min_x, max_x, min_y, max_y, True)
+            if isinstance(data, AnnBasedStereoExpData):
+                data.adata.raw = data.raw.adata
         return data
 
     @logit
     def filter_by_clusters(
             self,
             cluster_res_key: str = 'cluster',
             groups: Union[str, np.ndarray, List[str]] = None,
@@ -351,14 +367,16 @@
         gene_exp_cluster_key = f'gene_exp_{cluster_res_key}'
         if gene_exp_cluster_key in data.tl.result:
             if isinstance(groups, str):
                 groups = [groups]
             data.tl.result[gene_exp_cluster_key] = data.tl.result[gene_exp_cluster_key][groups]
         if data.raw is not None and filter_raw:
             filter_cells(data.raw, cell_list=data.cell_names, inplace=True)
+            if isinstance(data, AnnBasedStereoExpData):
+                data.adata.raw = data.raw.adata
         return data
 
     @logit
     def log1p(self,
               inplace: bool = True,
               res_key: str = 'log1p'):
         """
@@ -527,14 +545,16 @@
         self.result[res_key] = sc_transform(data, n_cells, n_genes, filter_hvgs, var_features_n,
                                             exp_matrix_key=exp_matrix_key, seed_use=seed_use, **kwargs)
         key = 'sct'
         self.reset_key_record(key, res_key)
 
         if data.raw is not None and filter_raw and data.shape != data.raw.shape:
             filter_genes(data.raw, gene_list=data.gene_names, inplace=True)
+            if isinstance(data, AnnBasedStereoExpData):
+                data.adata.raw = data.raw.adata
 
     @logit
     def highly_variable_genes(
             self,
             groups: Optional[str] = None,
             method: Literal['seurat', 'cell_ranger', 'seurat_v3'] = 'seurat',
             n_top_genes: Optional[int] = 2000,
@@ -985,18 +1005,18 @@
         if gene_exp_cluster_res is not False:
             self.result[gene_cluster_res_key] = gene_exp_cluster_res
             self.reset_key_record('gene_exp_cluster', gene_cluster_res_key)
 
     @logit
     def find_marker_genes(self,
                           cluster_res_key,
-                          method: Literal['t_test', 'wilcoxon_test'] = 't_test',
+                          method: Literal['t_test', 'wilcoxon_test', 'logreg'] = 't_test',
                           case_groups: Union[str, np.ndarray, list] = 'all',
                           control_groups: Union[str, np.ndarray, list] = 'rest',
-                          corr_method: str = 'benjamini-hochberg',
+                          corr_method: Literal['bonferroni', 'benjamini-hochberg'] = 'benjamini-hochberg',
                           use_raw: bool = True,
                           use_highly_genes: bool = True,
                           hvg_res_key: Optional[str] = 'highly_variable_genes',
                           res_key: str = 'marker_genes',
                           output: Optional[str] = None,
                           sort_by='scores',
                           n_genes: Union[str, int] = 'all',
@@ -1007,15 +1027,15 @@
         A tool to find maker genes. For each group, find statistical test different genes
         between one group and the rest groups using `t_test` or `wilcoxon_test`.
 
         :param cluster_res_key: the key of clustering to get corresponding result from `self.result`.
         :param method: choose method for statistics.
         :param case_groups: case group, default all clusters.
         :param control_groups: control group, default the rest of groups.
-        :param corr_method: correlation method.
+        :param corr_method: p-value correction method, only available for `t_test` and `wilcoxon_test`.
         :param use_raw: whether to use raw express matrix for analysis, default True.
         :param use_highly_genes: whether to use only the expression of hypervariable genes as input, default True.
         :param hvg_res_key: the key of highly variable genes to get corresponding result.
         :param res_key: the key for storing result of marker genes.
         :param output: the path to output file `.csv`. If None, do not generate output file.
         :param sort_by: default to 'scores', the result will sort by the key, other options 'log2fc'.
         :param n_genes: default to 0, means will auto calculate n_genes by N = 10000/K². K is cluster number, and N is
@@ -1037,16 +1057,16 @@
         data = self.raw if use_raw else self.data
         data = self.subset_by_hvg(hvg_res_key, use_raw=use_raw, inplace=False) if use_highly_genes else data
 
         if n_jobs <= 0:
             n_jobs = cpu_count()
 
         from stereo.utils.pipeline_utils import calc_pct_and_pct_rest, cell_cluster_to_gene_exp_cluster
-        pct, pct_rest = calc_pct_and_pct_rest(self.data, cluster_res_key)
-        mean_count_in_cluster = cell_cluster_to_gene_exp_cluster(self.data, cluster_res_key, kind='mean')
+        pct, pct_rest = calc_pct_and_pct_rest(self.data, cluster_res_key, filter_raw=False)
+        mean_count_in_cluster = cell_cluster_to_gene_exp_cluster(self.data, cluster_res_key, kind='mean', filter_raw=False)
 
         tool = FindMarker(data=data, groups=self.result[cluster_res_key], method=method, case_groups=case_groups,
                           control_groups=control_groups, corr_method=corr_method, sort_by=sort_by,
                           n_genes=n_genes, ascending=ascending, n_jobs=n_jobs, pct=pct, pct_rest=pct_rest, mean_count=mean_count_in_cluster)
         result = tool.result
         result['parameters'] = {
             'cluster_res_key': cluster_res_key,
```

### Comparing `stereopy-1.2.0/stereo/core/stereo_exp_data.py` & `stereopy-1.3.0b1/stereo/core/stereo_exp_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,15 @@
         self._tl = None
         self._plt = None
         self._offset_x = offset_x
         self._offset_y = offset_y
         self._attr = attr if attr is not None else {'resolution': 500}
         self._merged = merged
         self._sn = self.get_sn_from_path(file_path)
+        self.bin_coord_offset = False
 
     def get_sn_from_path(self, file_path):
         """
         Get the SN information of input file.
         """
         if file_path is None:
             return None
@@ -168,16 +169,21 @@
         Get data subset by name list of cells or genes.
 
         :param cell_name: a list of cell name.
         :param gene_name: a list of gene name.
         :return:
         """
         data = copy.deepcopy(self)
-        cell_index = self.get_index(data.cells.cell_name, cell_name) if cell_name is not None else None
-        gene_index = self.get_index(data.genes.gene_name, gene_name) if gene_name is not None else None
+        cell_index, gene_index = None, None
+        if cell_name is not None:
+            cell_index = self.cells.obs.index.get_indexer(cell_name)
+            cell_index = cell_index[cell_index != -1]
+        if gene_name is not None:
+            gene_index = self.genes.var.index.get_indexer(gene_name)
+            gene_index = gene_index[gene_index != -1]
         return data.sub_by_index(cell_index, gene_index)
 
     def sub_exp_matrix_by_name(
             self,
             cell_name: Optional[Union[np.ndarray, list, str, int]] = None,
             gene_name: Optional[Union[np.ndarray, list, str]] = None,
             order_preserving: bool = True
@@ -591,39 +597,43 @@
         Check whether the matrix is sparse matrix type.
         """
         return issparse(self.exp_matrix)
 
     def reset_position(self):
         if self.position_offset is not None:
             batches = np.unique(self.cells.batch)
+            position = self.position
             for bno in batches:
                 idx = np.where(self.cells.batch == bno)[0]
-                self.position[idx] -= self.position_offset[bno]
-                self.position[idx] += self.position_min[bno]
+                position[idx] -= self.position_offset[bno]
+                position[idx] += self.position_min[bno]
+            self.position = position
         self.position_offset = None
         self.position_min = None
 
     def __add__(self, other):
         from stereo.core.ms_data import MSData
         if isinstance(other, StereoExpData):
-            ms_data = MSData([self, other])
+            return MSData([self, other])
+        elif isinstance(other, MSData):
+            return other.__add__(self)
         else:
-            raise TypeError
-        return ms_data
+            raise TypeError("only support StereoExpData and MSData!")
+        
 
 
 class AnnBasedStereoExpData(StereoExpData):
 
     def __init__(
             self,
             h5ad_file_path: str = None,
             based_ann_data: anndata.AnnData = None,
             bin_type: str = None,
             bin_size: int = None,
-            spatial_key: Union[str, list, np.ndarray] = 'spatial',
+            spatial_key: str = 'spatial',
             *args,
             **kwargs
     ):
         super(AnnBasedStereoExpData, self).__init__(*args, **kwargs)
         if h5ad_file_path is None and based_ann_data is None:
             raise Exception("Must to input the 'h5ad_file_path' or 'based_ann_data'.")
 
@@ -656,14 +666,15 @@
         from .st_pipeline import AnnBasedStPipeline
         self._tl = AnnBasedStPipeline(self._ann_data, self)
 
         if self._ann_data.raw:
             self._tl._raw = AnnBasedStereoExpData(based_ann_data=self._ann_data.raw.to_adata())
 
         self.spatial_key = spatial_key
+        self.file_format = 'h5ad'
 
     def __str__(self):
         return str(self._ann_data)
 
     def __repr__(self):
         return self.__str__()
 
@@ -755,15 +766,15 @@
             self._ann_data.obsm[self.spatial_key] = position
 
     @position_z.setter
     def position_z(self, position_z: np.ndarray):
         if (position_z.shape) == 1:
             position_z = position_z.reshape(-1, 1)
         if self.spatial_key in self._ann_data.obsm:
-            self._ann_data.obsm[self.spatial_key][:, 2] = np.concatenate(
+            self._ann_data.obsm[self.spatial_key] = np.concatenate(
                 [self._ann_data.obsm[self.spatial_key][:, [0, 1]], position_z], axis=1)
         else:
             self._ann_data.obs['z'] = position_z
 
     @property
     def bin_type(self):
         return self._ann_data.uns.get('bin_type', 'bins')
@@ -807,32 +818,32 @@
         self._ann_data.uns['sn'] = pd.DataFrame(sn_list, columns=['batch', 'sn'])
 
     def sub_by_index(self, cell_index=None, gene_index=None):
         if cell_index is not None:
             self._ann_data._inplace_subset_obs(cell_index)
         if gene_index is not None:
             self._ann_data._inplace_subset_var(gene_index)
-        if self._ann_data.raw:
-            self.tl.raw = AnnBasedStereoExpData(based_ann_data=self._ann_data.raw.to_adata())
+        # if self._ann_data.raw:
+        #     self.tl.raw = AnnBasedStereoExpData(based_ann_data=self._ann_data.raw.to_adata())
         return self
 
     def sub_by_name(
             self,
             cell_name: Optional[Union[np.ndarray, list]] = None,
             gene_name: Optional[Union[np.ndarray, list]] = None
     ):
         data = AnnBasedStereoExpData(self.file, based_ann_data=self._ann_data.copy())
         data._ann_data.obs_names_make_unique()
         data._ann_data.var_names_make_unique()
         if cell_name is not None:
             data._ann_data._inplace_subset_obs(cell_name)
         if gene_name is not None:
             data._ann_data._inplace_subset_var(gene_name)
-        if data._ann_data.raw:
-            data.tl.raw = AnnBasedStereoExpData(based_ann_data=data._ann_data.raw.to_adata())
+        # if data._ann_data.raw:
+        #     data.tl.raw = AnnBasedStereoExpData(based_ann_data=data._ann_data.raw.to_adata())
         return data
 
     # @staticmethod
     # def merge(*data, batch_key='batch'):
     #     from anndata import concat
     #     ann_data = concat([d._ann_data for d in data], axis=0, merge='same', label=batch_key, index_unique='-')
     #     return AnnBasedStereoExpData(based_ann_data=ann_data)
```

### Comparing `stereopy-1.2.0/stereo/core/tool_base.py` & `stereopy-1.3.0b1/stereo/core/tool_base.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/data/algorithm/cell_cell_communication/database/cellphonedb.db` & `stereopy-1.3.0b1/stereo/data/algorithm/cell_cell_communication/database/cellphonedb.db`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/data/algorithm/cell_cell_communication/database/celltalkdb.db` & `stereopy-1.3.0b1/stereo/data/algorithm/cell_cell_communication/database/celltalkdb.db`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/data/algorithm/cell_cell_communication/database/liana.db` & `stereopy-1.3.0b1/stereo/data/algorithm/cell_cell_communication/database/liana.db`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/data/algorithm/cell_cell_communication/database/mouse2human.csv` & `stereopy-1.3.0b1/stereo/data/algorithm/cell_cell_communication/database/mouse2human.csv`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/__init__.py` & `stereopy-1.3.0b1/stereo/image/__init__.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/pyramid.py` & `stereopy-1.3.0b1/stereo/image/pyramid.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/base_cell_seg_pipe/cell_seg_pipeline.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/base_cell_seg_pipe/cell_seg_pipeline.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/base_cell_seg_pipe/find_maxima.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/base_cell_seg_pipe/find_maxima.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/base_cell_seg_pipe/grade.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/base_cell_seg_pipe/grade.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1/cell_infer.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1/cell_infer.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1/cell_seg_pipeline_v1.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1/cell_seg_pipeline_v1.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1/dataset.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1/image.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1/image.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1/models/SE_weight_module.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1/models/SE_weight_module.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1/models/epsanet.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1/models/epsanet.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1/resnet_unet.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1/resnet_unet.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1/tissue_seg.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1/tissue_seg.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1/tissue_seg_pipeline.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1/tissue_seg_pipeline.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1/utils.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1/utils.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/cell_infer.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/cell_infer.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # import tensorflow as tf
 import torch
 from albumentations import Compose
 from albumentations.pytorch import ToTensorV2
 from skimage import filters
 from tqdm import tqdm
 
-from stereo import logger
+from stereo.log_manager import logger
 from .dataset import data_batch2
 from .resnet_unet import EpsaResUnet
 from .utils import (
     split_preproc
 )
 
 # os.environ["CUDA_VISIBLE_DEVICES"] = "-1"
```

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/cell_seg_pipeline_v1_pro.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/cell_seg_pipeline_v1_pro.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/dataset.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/dataset.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/find_maxima.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/find_maxima.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/grade.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/grade.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/image.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/image.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/models/SE_weight_module.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/models/SE_weight_module.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/models/epsanet.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/models/epsanet.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/resnet_unet.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/resnet_unet.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/tissue_seg.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/tissue_seg.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/tissue_seg_pipeline.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/tissue_seg_pipeline.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/v1_pro/utils.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v1_pro/utils.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/seg_utils/v3/cell_seg_pipeline_v3.py` & `stereopy-1.3.0b1/stereo/image/segmentation/seg_utils/v3/cell_seg_pipeline_v3.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation/segment.py` & `stereopy-1.3.0b1/stereo/image/segmentation/segment.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation_deepcell/seg_utils/cell_infer.py` & `stereopy-1.3.0b1/stereo/image/segmentation_deepcell/seg_utils/cell_infer.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation_deepcell/seg_utils/cell_seg_pipeline.py` & `stereopy-1.3.0b1/stereo/image/segmentation_deepcell/seg_utils/cell_seg_pipeline.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation_deepcell/seg_utils/find_maxima.py` & `stereopy-1.3.0b1/stereo/image/segmentation_deepcell/seg_utils/find_maxima.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation_deepcell/seg_utils/grade.py` & `stereopy-1.3.0b1/stereo/image/segmentation_deepcell/seg_utils/grade.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation_deepcell/seg_utils/image.py` & `stereopy-1.3.0b1/stereo/image/segmentation_deepcell/seg_utils/image.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation_deepcell/seg_utils/tissue_seg.py` & `stereopy-1.3.0b1/stereo/image/segmentation_deepcell/seg_utils/tissue_seg.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation_deepcell/seg_utils/tissue_seg_pipeline.py` & `stereopy-1.3.0b1/stereo/image/segmentation_deepcell/seg_utils/tissue_seg_pipeline.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation_deepcell/seg_utils/utils.py` & `stereopy-1.3.0b1/stereo/image/segmentation_deepcell/seg_utils/utils.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/segmentation_deepcell/segment.py` & `stereopy-1.3.0b1/stereo/image/segmentation_deepcell/segment.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/tissue_cut/pipeline.py` & `stereopy-1.3.0b1/stereo/image/tissue_cut/pipeline.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/tissue_cut/tissue_cut_utils/tissue_seg_bcdu.py` & `stereopy-1.3.0b1/stereo/image/tissue_cut/tissue_cut_utils/tissue_seg_bcdu.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/tissue_cut/tissue_cut_utils/tissue_seg_bcdu_model.py` & `stereopy-1.3.0b1/stereo/image/tissue_cut/tissue_cut_utils/tissue_seg_bcdu_model.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/tissue_cut/tissue_cut_utils/tissue_seg_bcdu_uity.py` & `stereopy-1.3.0b1/stereo/image/tissue_cut/tissue_cut_utils/tissue_seg_bcdu_uity.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/tissue_cut/tissue_cut_utils/tissue_seg_net.py` & `stereopy-1.3.0b1/stereo/image/tissue_cut/tissue_cut_utils/tissue_seg_net.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/tissue_cut/tissue_cut_utils/tissue_seg_utils.py` & `stereopy-1.3.0b1/stereo/image/tissue_cut/tissue_cut_utils/tissue_seg_utils.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/image/x2tif/x2tif.py` & `stereopy-1.3.0b1/stereo/image/x2tif/x2tif.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/io/h5ad.py` & `stereopy-1.3.0b1/stereo/io/h5ad.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 
 @write.register(Neighbors)
 def _(v, f, k):
     write_neighbors(f, k, v)
 
 
-def write_array(f, key, value, dataset_kwargs=MappingProxyType({})):
+def write_array(f: Union[h5py.File, h5py.Group], key, value, dataset_kwargs=MappingProxyType({})):
     # Convert unicode to fixed length strings
     if value.dtype.kind in {'U', 'O'}:
         value = value.astype(h5py.special_dtype(vlen=str))
     elif value.dtype.names is not None:
         value = _to_hdf5_vlen_strings(value)
     f.create_dataset(key, data=value, **dataset_kwargs)
 
@@ -93,34 +93,56 @@
     if 'maxshape' not in dataset_kwargs:
         dataset_kwargs = dict(maxshape=(None,), **dataset_kwargs)
     g.create_dataset('data', data=v.data, **dataset_kwargs)
     g.create_dataset('indices', data=v.indices, **dataset_kwargs)
     g.create_dataset('indptr', data=v.indptr, **dataset_kwargs)
 
 
-def write_genes(f, k, v, dataset_kwargs=MappingProxyType({})):
+# def write_genes(f, k, v: Gene, dataset_kwargs=MappingProxyType({})):
+#     g = f.create_group(k)
+#     g.attrs['encoding-type'] = 'gene'
+#     write_array(g, 'gene_name', v.gene_name, dataset_kwargs)
+#     if v.n_cells is not None:
+#         write_array(g, 'n_cells', v.n_cells, dataset_kwargs)
+#     if v.n_counts is not None:
+#         write_array(g, 'n_counts', v.n_counts, dataset_kwargs)
+#     if v.mean_umi is not None:
+#         write_array(g, 'mean_umi', v.n_counts, dataset_kwargs)
+#     if v.real_gene_name is not None:
+#         write_array(g, 'real_gene_name', v.real_gene_name, dataset_kwargs)
+
+def write_genes(f: h5py.File, k: str, v: Gene, dataset_kwargs=MappingProxyType({})):
     g = f.create_group(k)
     g.attrs['encoding-type'] = 'gene'
-    write_array(g, 'gene_name', v.gene_name, dataset_kwargs)
-    if v.n_cells is not None:
-        write_array(g, 'n_cells', v.n_cells, dataset_kwargs)
-    if v.n_counts is not None:
-        write_array(g, 'n_counts', v.n_counts, dataset_kwargs)
+    g.attrs['version'] = 'v2'
+    write_dataframe(g, 'var', v.to_df(), dataset_kwargs)
+
 
+# def write_cells(f, k, v: Cell, dataset_kwargs=MappingProxyType({})):
+#     g = f.create_group(k)
+#     g.attrs['encoding-type'] = 'cell'
+#     write_array(g, 'cell_name', v.cell_name, dataset_kwargs)
+#     if v.total_counts is not None:
+#         write_array(g, 'total_counts', v.total_counts, dataset_kwargs)
+#     if v.pct_counts_mt is not None:
+#         write_array(g, 'pct_counts_mt', v.pct_counts_mt, dataset_kwargs)
+#     if v.n_genes_by_counts is not None:
+#         write_array(g, 'n_genes_by_counts', v.n_genes_by_counts, dataset_kwargs)
+#     if v.batch is not None:
+#         write_array(g, 'batch', v.batch, dataset_kwargs)
+#     if v.cell_border is not None:
+#         write_array(g, 'cell_border', v.cell_border, dataset_kwargs)
 
-def write_cells(f, k, v, dataset_kwargs=MappingProxyType({})):
+def write_cells(f: h5py.File, k: str, v: Cell, dataset_kwargs=MappingProxyType({})):
     g = f.create_group(k)
     g.attrs['encoding-type'] = 'cell'
-    write_array(g, 'cell_name', v.cell_name, dataset_kwargs)
-    if v.total_counts is not None:
-        write_array(g, 'total_counts', v.total_counts, dataset_kwargs)
-    if v.pct_counts_mt is not None:
-        write_array(g, 'pct_counts_mt', v.pct_counts_mt, dataset_kwargs)
-    if v.n_genes_by_counts is not None:
-        write_array(g, 'n_genes_by_counts', v.n_genes_by_counts, dataset_kwargs)
+    g.attrs['version'] = 'v2'
+    write_dataframe(g, 'obs', v.to_df(), dataset_kwargs)
+    if v.cell_border is not None:
+        write_array(g, 'cell_border', v.cell_border, dataset_kwargs)
 
 
 def write_spmatrix_as_dense(f, key, value, dataset_kwargs=MappingProxyType({})):
     dset = f.create_dataset(key, shape=value.shape, dtype=value.dtype, **dataset_kwargs)
     compressed_axis = int(isinstance(value, sparse.csc_matrix))
     for idx in idx_chunks_along_axis(value.shape, compressed_axis, 1000):
         dset[idx] = value[idx].toarray()
@@ -250,36 +272,48 @@
         else sparse.csc_matrix(shape, dtype=dtype)
     mtx.data = group['data'][...]
     mtx.indices = group['indices'][...]
     mtx.indptr = group['indptr'][...]
     return mtx
 
 
-def read_genes(group) -> Gene:
-    gene_name = group['gene_name'][...]
-    gene = Gene(gene_name=gene_name)
-    n_cells = group['n_cells'][...] if 'n_cells' in group.keys() else None
-    n_counts = group['n_counts'][...] if 'n_counts' in group.keys() else None
-    gene.n_cells = n_cells
-    gene.n_counts = n_counts
+def read_genes(group: h5py.Group) -> Gene:
+    version = group.attrs.get('version', 'v1')
+    if version == 'v1':
+        gene_name = group['gene_name'][...]
+        gene = Gene(gene_name=gene_name)
+        n_cells = group['n_cells'][...] if 'n_cells' in group.keys() else None
+        n_counts = group['n_counts'][...] if 'n_counts' in group.keys() else None
+        gene.n_cells = n_cells
+        gene.n_counts = n_counts
+    else:
+        var = read_dataframe(group['var'])
+        gene = Gene(var=var)
     return gene
 
 
-def read_cells(group) -> Cell:
-    cell_name = group['cell_name'][...]
-    for i in range(cell_name.shape[0]):
-        if type(cell_name[i]) is bytes:
-            cell_name[i] = cell_name[i].decode()
-    cell = Cell(cell_name=cell_name)
-    total_counts = group['total_counts'][...] if 'total_counts' in group.keys() else None
-    pct_counts_mt = group['pct_counts_mt'][...] if 'pct_counts_mt' in group.keys() else None
-    n_genes_by_counts = group['n_genes_by_counts'][...] if 'n_genes_by_counts' in group.keys() else None
-    cell.total_counts = total_counts
-    cell.pct_counts_mt = pct_counts_mt
-    cell.n_genes_by_counts = n_genes_by_counts
+def read_cells(group: h5py.Group) -> Cell:
+    version = group.attrs.get('version', 'v1')
+    if version == 'v1':
+        cell_name = group['cell_name'][...]
+        for i in range(cell_name.shape[0]):
+            if type(cell_name[i]) is bytes:
+                cell_name[i] = cell_name[i].decode()
+        cell = Cell(cell_name=cell_name)
+        total_counts = group['total_counts'][...] if 'total_counts' in group.keys() else None
+        pct_counts_mt = group['pct_counts_mt'][...] if 'pct_counts_mt' in group.keys() else None
+        n_genes_by_counts = group['n_genes_by_counts'][...] if 'n_genes_by_counts' in group.keys() else None
+        cell.total_counts = total_counts
+        cell.pct_counts_mt = pct_counts_mt
+        cell.n_genes_by_counts = n_genes_by_counts
+    else:
+        obs = read_dataframe(group['obs'])
+        cell = Cell(obs=obs)
+        if 'cell_border' in group.keys():
+            cell.cell_border = group['cell_border'][...]
     return cell
 
 
 def read_series(dataset) -> Union[np.ndarray, pd.Categorical]:
     if 'categories' in dataset.attrs:
         categories = dataset.attrs['categories']
         ordered = False
```

### Comparing `stereopy-1.2.0/stereo/io/reader.py` & `stereopy-1.3.0b1/stereo/io/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,27 +29,32 @@
 from stereo.core.cell import Cell
 from stereo.core.constants import CHIP_RESOLUTION
 from stereo.core.gene import Gene
 from stereo.core.stereo_exp_data import AnnBasedStereoExpData
 from stereo.core.stereo_exp_data import StereoExpData
 from stereo.core.result import _BaseResult
 from stereo.io import h5ad
-from stereo.io.utils import remove_genes_number, integrate_matrix_by_genes, transform_marker_genes_to_anndata
+from stereo.io.utils import(
+    remove_genes_number,
+    integrate_matrix_by_genes,
+    transform_marker_genes_to_anndata,
+    get_gem_comments
+)
 from stereo.log_manager import logger
 from stereo.utils.read_write_utils import ReadWriteUtils
 
 
 @ReadWriteUtils.check_file_exists
 def read_gem(
         file_path: str,
         sep: str = '\t',
         bin_type: str = "bins",
         bin_size: int = 100,
         is_sparse: bool = True,
-        bin_coor_offset: bool = False,
+        bin_coord_offset: bool = False,
         gene_name_index: bool = False
 ):
     """
     Read the Stereo-seq GEM file, and generate the StereoExpData object.
 
     Parameters
     -------------
@@ -59,29 +64,31 @@
         the separator string.
     bin_type
         the bin type includes `'bins'` or `'cell_bins'`, default to `'bins'`.
     bin_size
         the size of bin to merge, when `bin_type` is set to `'bins'`.
     is_sparse
         the expression matrix is sparse matrix, if `True`, otherwise `np.ndarray`.
-    bin_coor_offset
+    bin_coord_offset
         if set it to True, the coordinates of bins are calculated as
         ((gene_coordinates - min_coordinates) // bin_size) * bin_size + min_coordinates + bin_size/2
     gene_name_index
         In a v0.1 gem file, the column geneID is the gene name actually, but in a v0.2,
         geneID just a ID for genes and there is an additional column called geneName where is the gene name,
         When the version of gem file is v0.2, set `gene_name_index` to True to set column geneName as index, otherwise,
         set column geneID, if a v0.1 gem file, `gene_name_index` will be ignored and column geneID is set as index.
 
     Returns
     -------------
     An object of StereoExpData.
     """
-    data = StereoExpData(file_path=file_path, bin_type=bin_type, bin_size=bin_size)
-    df = pd.read_csv(str(data.file), sep=sep, comment='#', header=0)
+    data = StereoExpData(file_path=file_path, file_format='gem', bin_type=bin_type, bin_size=bin_size)
+    comments_lines, _ = get_gem_comments(str(data.file))
+    # df = pd.read_csv(str(data.file), sep=sep, comment='#', header=0)
+    df = pd.read_csv(str(data.file), sep=sep, header=comments_lines, engine='pyarrow')
     if 'MIDCounts' in df.columns:
         df.rename(columns={'MIDCounts': 'UMICount'}, inplace=True)
     elif 'MIDCount' in df.columns:
         df.rename(columns={'MIDCount': 'UMICount'}, inplace=True)
     if 'CellID' in df.columns:
         df.rename(columns={'CellID': 'cell_id'}, inplace=True)
     if 'label' in df.columns:
@@ -97,48 +104,45 @@
         axis=0,
         inplace=True
     )
     gdf = None
     if data.bin_type == 'cell_bins':
         gdf = parse_cell_bin_coor(df)
     else:
-        if bin_coor_offset:
+        if bin_coord_offset:
             df = parse_bin_coor(df, bin_size)
         else:
             df = parse_bin_coor_no_offset(df, bin_size)
+    
+    if gene_name_index and 'geneName' in df.columns:
+        df['geneID'] = df['geneName']
+
     cells = df['cell_id'].unique()
     genes = df['geneID'].unique()
     cells_dict = dict(zip(cells, range(0, len(cells))))
     genes_dict = dict(zip(genes, range(0, len(genes))))
     rows = df['cell_id'].map(cells_dict)
     cols = df['geneID'].map(genes_dict)
     # logger.info(f'the martrix has {len(cells)} cells, and {len(genes)} genes.')
     exp_matrix = csr_matrix((df['UMICount'], (rows, cols)), shape=(cells.shape[0], genes.shape[0]), dtype=np.int32)
     data.cells = Cell(cell_name=cells)
+    data.genes = Gene(gene_name=genes)
+
+    if not gene_name_index and 'geneName' in df.columns:
+        gene_names = df.groupby(by='geneID').aggregate({'geneName': lambda n: np.unique(n)[0]})['geneName']
+        data.genes['real_gene_name'] = gene_names
 
-    if 'geneName' in df.columns:
-        gene_names = df['geneName'].unique().astype('U')
-        gene_names = remove_genes_number(gene_names)
-        if gene_name_index:
-            exp_matrix, gene_names = integrate_matrix_by_genes(gene_names, cells.shape[0],
-                                                       exp_matrix.data, exp_matrix.indices, exp_matrix.indptr)
-            data.genes = Gene(gene_name=gene_names)
-        else:
-            data.genes = Gene(gene_name=genes)
-            # data.genes['gene_name_underline'] = gene_names
-            data.genes['real_gene_name'] = gene_names
-    else:
-        data.genes = Gene(gene_name=genes)
     data.exp_matrix = exp_matrix if is_sparse else exp_matrix.toarray()
     if data.bin_type == 'bins':
         # data.position = df.loc[:, ['x_center', 'y_center']].drop_duplicates().values
         data.position = df.loc[:, ['bin_x', 'bin_y']].drop_duplicates().values
     else:
         data.position = gdf.loc[cells][['x_center', 'y_center']].values
         data.cells.cell_point = gdf.loc[cells]['cell_point'].values
+    data.position = data.position.astype(np.uint32)
     data.offset_x = df['x'].min()
     data.offset_y = df['y'].min()
     resolution = 500
     for chip_name in CHIP_RESOLUTION.keys():
         if data.sn[0:len(chip_name)] == chip_name:
             resolution = CHIP_RESOLUTION[chip_name]
             break
@@ -147,14 +151,15 @@
         'minY': df['y'].min(),
         'maxX': df['x'].max(),
         'maxY': df['y'].max(),
         'minExp': data.exp_matrix.min(),  # noqa
         'maxExp': data.exp_matrix.max(),  # noqa
         'resolution': resolution,
     }
+    data.bin_coord_offset = bin_coord_offset
     logger.info(f'the martrix has {data.cell_names.size} cells, and {data.gene_names.size} genes.')
     return data
 
 
 def parse_bin_coor(df, bin_size):
     """
     merge bins to a bin unit according to the bin size, also calculate the center coordinate of bin unit,
@@ -247,22 +252,26 @@
         logger.error('the input file is not exists, please check!')
         raise FileExistsError('the input file is not exists, please check!')
     with h5py.File(data.file, mode='r') as f:
         data = _read_stereo_h5ad_from_group(f, data, use_raw, use_result, bin_type, bin_size)
     return data
 
 
-def _read_stereo_h5ad_from_group(f, data: StereoExpData, use_raw, use_result, bin_type=None, bin_size=None):
+def _read_stereo_h5ad_from_group(f: Union[h5py.File, h5py.Group], data: StereoExpData, use_raw, use_result, bin_type=None, bin_size=None):
     # read data
     data.bin_type = bin_type if bin_type is not None else 'bins'
     data.bin_size = bin_size if bin_size is not None else 1
+    not_data_attr_keys = {'bin_type', 'bin_size', 'merged'}
     if f.attrs is not None:
         data.attr = {}
         for key, value in f.attrs.items():
-            data.attr[key] = value
+            if key not in not_data_attr_keys:
+                data.attr[key] = value
+            else:
+                setattr(data, key, value)
     for k in f.keys():
         if k == 'cells':
             data.cells = h5ad.read_group(f[k])
         elif k == 'genes':
             data.genes = h5ad.read_group(f[k])
         elif k == 'position':
             position = h5ad.read_dataset(f[k])
@@ -316,28 +325,33 @@
     # read key_record and result
     if use_result is True and 'key_record' in f.keys():
         h5ad.read_key_record(f['key_record'], data.tl.key_record)
         _read_stereo_h5_result(data.tl.key_record, data, f)
     return data
 
 
-def _read_stereo_h5_result(key_record: dict, data, f):
+def _read_stereo_h5_result(key_record: dict, data: StereoExpData, f: Union[h5py.File, h5py.Group]):
     import ast
     from ..utils.pipeline_utils import cell_cluster_to_gene_exp_cluster
+    key_record = deepcopy(key_record)
     for analysis_key in list(key_record.keys()):
         res_keys = key_record[analysis_key]
         for res_key in res_keys:
             if analysis_key == 'hvg':
                 hvg_df = h5ad.read_group(f[f'{res_key}@hvg'])
                 # str to interval
                 if 'mean_bin' in hvg_df.columns:
                     hvg_df['mean_bin'] = [to_interval(interval_string) for interval_string in hvg_df['mean_bin']]
                 data.tl.result[res_key] = hvg_df
             if analysis_key in ['pca', 'umap', 'totalVI', 'spatial_alignment_integration']:
                 data.tl.result[res_key] = pd.DataFrame(h5ad.read_dataset(f[f'{res_key}@{analysis_key}']))
+                if analysis_key == 'pca':
+                    variance_ratio_key = f'{res_key}_variance_ratio'
+                    if f'{variance_ratio_key}@{analysis_key}_variance_ratio' in f.keys():
+                        data.tl.result[variance_ratio_key] = h5ad.read_dataset(f[f'{variance_ratio_key}@{analysis_key}_variance_ratio'])  # noqa
             if analysis_key == 'neighbors':
                 data.tl.result[res_key] = {
                     # 'neighbor': h5ad.read_group(f[f'neighbor@{res_key}@neighbors']),
                     'connectivities': h5ad.read_group(f[f'connectivities@{res_key}@neighbors']),
                     'nn_dist': h5ad.read_group(f[f'nn_dist@{res_key}@neighbors'])
                 }
                 if f'neighbor@{res_key}@neighbors' in f:
@@ -428,52 +442,72 @@
     :param use_raw: Whether to load the raw data of each StereoExpData in MSData, defaults to True.
     :param use_result: Whether to load the analysis results which had been saved in h5ms file, defaults to True.
 
     :return: An object of MSData
     """
     from stereo.core.ms_data import MSData
     with h5py.File(file_path, mode='r') as f:
-        ms_data = MSData()
+        # ms_data = MSData()
         data_list = []
         merged_data = None
         names = []
         var_type = None
         relationship = None
-        result = {}
+        scopes_data = {}
+        result_keys = {}
+        # result = {}
         for k in f.keys():
             if k == 'sample':
                 for one_slice_key in f[k].keys():
                     data = StereoExpData()
                     data_list.append(
                         _read_stereo_h5ad_from_group(f[k][one_slice_key], data, use_raw, use_result))  # noqa
             elif k == 'sample_merged':
-                merged_data = StereoExpData()
-                merged_data = _read_stereo_h5ad_from_group(f[k], merged_data, use_raw, use_result)  # noqa
+                for mk in f[k].keys():
+                    scope_data = StereoExpData()
+                    scope_data = _read_stereo_h5ad_from_group(f[k][mk], scope_data, use_raw, use_result)
+                    scopes_data[mk] = scope_data
+                    if f[k][mk].attrs is not None:
+                        merged_from_all = f[k][mk].attrs.get('merged_from_all', False)
+                        if merged_from_all:
+                            merged_data = scope_data
+                # merged_data = StereoExpData()
+                # merged_data = _read_stereo_h5ad_from_group(f[k], merged_data, use_raw, use_result)  # noqa
             elif k == 'names':
                 names = h5ad.read_dataset(f[k])
+                if isinstance(names, np.ndarray):
+                    names = names.tolist()
             elif k == 'var_type':
                 var_type = h5ad.read_dataset(f[k])
             elif k == 'relationship':
                 relationship = h5ad.read_dataset(f[k])
-            elif k == 'mss':
-                for key in f['mss'].keys():
-                    data = StereoExpData()
-                    data.tl.result = {}
-                    h5ad.read_key_record(f['mss'][key]['key_record'], data.tl.key_record)
-                    _read_stereo_h5_result(data.tl.key_record, data, f['mss'][key])
-                    result[key] = data.tl.result
+            elif k == 'result_keys':
+                for rk in f[k].keys():
+                    result_keys[rk] = list(h5ad.read_dataset(f[k][rk]))
+            # elif k == 'mss':
+            #     for key in f['mss'].keys():
+            #         data = StereoExpData()
+            #         data.tl.result = {}
+            #         h5ad.read_key_record(f['mss'][key]['key_record'], data.tl.key_record)
+            #         _read_stereo_h5_result(data.tl.key_record, data, f['mss'][key])
+            #         result[key] = data.tl.result
             else:
                 logger.warn(f"{k} not in rules, did not read from h5ms")
 
-        ms_data._names = names
-        ms_data._var_type = var_type
-        ms_data._data_list = data_list
-        ms_data._merged_data = merged_data
-        ms_data.tl.result = result
-        ms_data._relationship = relationship
+        ms_data = MSData(
+            _data_list=data_list,
+            _names=names,
+            _var_type=var_type,
+            _relationship=relationship
+        )
+        ms_data.merged_data = merged_data
+        # ms_data.tl.result = result
+        ms_data.scopes_data = scopes_data
+        ms_data.tl.result_keys = result_keys
+
         return ms_data
 
 
 @ReadWriteUtils.check_file_exists
 def read_seurat_h5ad(
         file_path: str,
         use_raw: bool = False
@@ -1090,15 +1124,15 @@
     logger.info('read_gef begin ...')
     from gefpy.utils import gef_is_cell_bin
     is_cell_bin = gef_is_cell_bin(file_path)
     if bin_type == 'cell_bins':
         if not is_cell_bin:
             raise Exception('This file is not the type of CellBin.')
 
-        data = StereoExpData(file_path=file_path, bin_type=bin_type, bin_size=bin_size)
+        data = StereoExpData(file_path=file_path, file_format='gef', bin_type=bin_type, bin_size=bin_size)
         from gefpy.cgef_reader_cy import CgefR
         gef = CgefR(file_path, True)
         cellborders_coord_list, coord_count_per_cell = gef.get_cellborders([])
         border_points_count_per_cell = int(coord_count_per_cell / 2)
         cell_borders = cellborders_coord_list.reshape((-1, border_points_count_per_cell, 2))
         if gene_list is not None or region is not None:
             if gene_list is None:
```

### Comparing `stereopy-1.2.0/stereo/io/utils.py` & `stereopy-1.3.0b1/stereo/io/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from natsort import natsorted
 import numpy as np
 from scipy.sparse import csr_matrix
+import gzip
 
 def remove_genes_number(gene_names):
     underline = np.char.find(gene_names, '_', start=1, end=-1)
     underline = (underline > 0)
     if not np.any(underline):
         return gene_names
     gene_idx = np.arange(gene_names.size, dtype=np.uint64)
@@ -97,8 +98,22 @@
             group = k.split('.vs.')[0]
             dtype.append((group, marker_genes_res[k][k1].dtype))
         recarr = np.recarray(shape=marker_genes_res[k].shape[0], dtype=dtype)
         for k in groups_key:
             group = k.split('.vs.')[0]
             recarr[group] = marker_genes_res[k][k1].to_numpy()
         marker_genes_result[k2] = recarr
-    return marker_genes_result
+    return marker_genes_result
+
+def get_gem_comments(gem_file_path: str):
+    if gem_file_path.endswith('.gz'):
+        open_func =  gzip.open
+    else:
+        open_func = open
+    
+    comments = []
+    with open_func(gem_file_path, 'rb') as fp:
+        for line in fp:
+            if not line.startswith(b'#'):
+                break
+            comments.append(line)
+    return len(comments), comments
```

### Comparing `stereopy-1.2.0/stereo/io/writer.py` & `stereopy-1.3.0b1/stereo/io/writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,18 +82,21 @@
         if data.output is None:
             raise Exception("The output path must be set before writing.")
 
     with h5py.File(data.output, mode='w') as f:
         _write_one_h5ad(f, data, use_raw=use_raw, use_result=use_result, key_record=key_record)
 
 
-def _write_one_h5ad(f, data: StereoExpData, use_raw=False, use_result=True, key_record=None):
+def _write_one_h5ad(f: h5py.File, data: StereoExpData, use_raw=False, use_result=True, key_record=None):
     if data.attr is not None:
         for key, value in data.attr.items():
             f.attrs[key] = value
+    f.attrs['bin_type'] = data.bin_type
+    f.attrs['bin_size'] = data.bin_size
+    f.attrs['merged'] = data.merged
     if data.sn is not None:
         sn_list = []
         if isinstance(data.sn, str):
             sn_list = [['-1', data.sn]]
         else:
             for bno, sn in data.sn.items():
                 if sn is None:
@@ -111,17 +114,17 @@
         position = np.concatenate([data.position, data.position_z], axis=1)
     h5ad.write(position, f, 'position')
     if issparse(data.exp_matrix):
         sp_format = 'csr' if isinstance(data.exp_matrix, csr_matrix) else 'csc'
         h5ad.write(data.exp_matrix, f, 'exp_matrix', sp_format)
     else:
         h5ad.write(data.exp_matrix, f, 'exp_matrix')
-    h5ad.write(data.bin_type, f, 'bin_type')
-    h5ad.write(data.bin_size, f, 'bin_size')
-    h5ad.write(data.merged, f, 'merged')
+    # h5ad.write(data.bin_type, f, 'bin_type')
+    # h5ad.write(data.bin_size, f, 'bin_size')
+    # h5ad.write(data.merged, f, 'merged')
 
     if use_raw is True:
         same_genes = np.array_equal(data.tl.raw.gene_names, data.gene_names)
         same_cells = np.array_equal(data.tl.raw.cell_names, data.cell_names)
         if not same_genes:
             # if raw genes differ from genes
             h5ad.write(data.tl.raw.genes, f, 'genes@raw')
@@ -169,14 +172,18 @@
                 # interval to str
                 hvg_df: pd.DataFrame = deepcopy(data.tl.result[res_key])
                 if 'mean_bin' in hvg_df.columns:
                     hvg_df.mean_bin = [str(interval) for interval in data.tl.result[res_key].mean_bin]
                 h5ad.write(hvg_df, f, f'{res_key}@hvg')  # -> dataframe
             if analysis_key in ['pca', 'umap', 'totalVI', 'spatial_alignment_integration']:
                 h5ad.write(data.tl.result[res_key].values, f, f'{res_key}@{analysis_key}')  # -> array
+                if analysis_key == 'pca':
+                    variance_ratio_key = f"{res_key}_variance_ratio"
+                    if variance_ratio_key in data.tl.result:
+                        h5ad.write(data.tl.result[variance_ratio_key], f, f'{variance_ratio_key}@{analysis_key}_variance_ratio')
             if analysis_key == 'neighbors':
                 for neighbor_key, value in data.tl.result[res_key].items():
                     if value is None:
                         continue
                     if issparse(value):
                         sp_format = 'csr' if isinstance(value, csr_matrix) else 'csc'
                         h5ad.write(value, f, f'{neighbor_key}@{res_key}@neighbors', sp_format)  # -> csr_matrix
@@ -258,30 +265,42 @@
     :param output: The path of file into which MSData is saved.
     """
     with h5py.File(output, mode='w') as f:
         f.create_group('sample')
         for idx, data in enumerate(ms_data._data_list):
             f['sample'].create_group(f'sample_{idx}')
             _write_one_h5ad(f['sample'][f'sample_{idx}'], data)
-        if ms_data._merged_data:
+        # if ms_data._merged_data:
+        #     f.create_group('sample_merged')
+        #     _write_one_h5ad(f['sample_merged'], ms_data._merged_data)
+        if len(ms_data.scopes_data) > 0:
             f.create_group('sample_merged')
-            _write_one_h5ad(f['sample_merged'], ms_data._merged_data)
+            for scope_key, merged_data in ms_data.scopes_data.items():
+                g = f['sample_merged'].create_group(scope_key)
+                if ms_data.merged_data and id(ms_data.merged_data) == id(merged_data):
+                    g.attrs['merged_from_all'] = True
+                _write_one_h5ad(g, merged_data)
         h5ad.write_list(f, 'names', ms_data.names)
         h5ad.write_dataframe(f, 'obs', ms_data.obs)
         h5ad.write_dataframe(f, 'var', ms_data.var)
-        h5ad.write(ms_data._var_type, f, 'var_type')
+        h5ad.write(ms_data.var_type, f, 'var_type')
         h5ad.write(ms_data.relationship, f, 'relationship')
-        if ms_data.tl.result:
-            mss_f = f.create_group('mss')
-            for key in ms_data.tl.result.keys():
-                data = StereoExpData()
-                data.tl.result = ms_data.tl.result[key]
-                data.tl.key_record = ms_data.tl.key_record[key]
-                mss_f.create_group(key)
-                _write_one_h5ad_result(data, mss_f[key], data.tl.key_record)
+        if len(ms_data.tl.result_keys) > 0:
+            g = f.create_group('result_keys')
+            for scope_key, key_list in ms_data.tl.result_keys.items():
+                # g = f['result_keys'].create_group(f'result_keys_{i}')
+                h5ad.write(key_list, g, scope_key)
+        # if ms_data.tl.result:
+        #     mss_f = f.create_group('mss')
+        #     for key in ms_data.tl.result.keys():
+        #         data = StereoExpData()
+        #         data.tl.result = ms_data.tl.result[key]
+        #         data.tl.key_record = ms_data.tl.key_record[key]
+        #         mss_f.create_group(key)
+        #         _write_one_h5ad_result(data, mss_f[key], data.tl.key_record)
 
 
 def write_mid_gef(data: StereoExpData, output: str):
     """
     Write the StereoExpData object into a GEF (.h5) file.
 
     Parameters
```

### Comparing `stereopy-1.2.0/stereo/log_manager.py` & `stereopy-1.3.0b1/stereo/log_manager.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/__init__.py` & `stereopy-1.3.0b1/stereo/plots/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,7 +28,12 @@
 from .plot_clusters_scatter import ClustersGenesScatter
 from .plot_clusters_heatmap import ClustersGenesHeatmap
 from .plot_paga import PlotPaga
 from .plot_time_series import PlotTimeSeries
 from .plot_time_series import PlotTimeSeriesAnalysis
 from .plot_elbow import PlotElbow
 from .plot_genes_in_pseudotime import PlotGenesInPseudotime
+from .plot_st_gears import PlotStGears
+from .plot_ccc import PlotCellCellCommunication
+from .plot_grn import PlotRegulatoryNetwork
+from .plot_batch_qc import ShowBatchQcReport
+from .plot_ms_spatial_scatter import PlotMsSpatialScatter
```

### Comparing `stereopy-1.2.0/stereo/plots/_plot_basic/get_stereo_data.py` & `stereopy-1.3.0b1/stereo/plots/_plot_basic/get_stereo_data.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/_plot_basic/heatmap_plt.py` & `stereopy-1.3.0b1/stereo/plots/_plot_basic/heatmap_plt.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/decorator.py` & `stereopy-1.3.0b1/stereo/plots/decorator.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
                 try:
                     out_path = file_name_input.value
                     file_format = format_select.value
                     dpi = dpi_input.value if dpi_input.value > 0 else 100
                     if out_path is not None and len(out_path) > 0:
                         out_path = f"{out_path}_{func.__name__}.{file_format}"
                         figure.savefig(out_path, bbox_inches='tight', dpi=dpi)
-                        static_text.value = f'the plot has alrady been saved in the same directory as this notebook ' \
+                        static_text.value = f'the plot has already been saved in the same directory as this notebook ' \
                                             f'and named as <font color="red"><b>{out_path}</b></font>'
                 finally:
                     export_button.loading = False
 
             action = partial(_action, figure=fig)
             export_button.on_click(action)
             return pn.Column(
```

### Comparing `stereopy-1.2.0/stereo/plots/interact_plot/annotation_cluster.py` & `stereopy-1.3.0b1/stereo/plots/interact_plot/annotation_cluster.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/interact_plot/interactive_scatter.py` & `stereopy-1.3.0b1/stereo/plots/interact_plot/interactive_scatter.py`

 * *Files 25% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 import tifffile as tiff
 import numpy as np
 
 from stereo.log_manager import logger
 from stereo.stereo_config import stereo_conf
 from stereo.tools.tools import make_dirs
 from stereo.preprocess.filter import filter_genes
+from stereo.core.stereo_exp_data import StereoExpData
+from stereo.io.utils import get_gem_comments
 
 link = link_selections.instance()
 pn.param.ParamMethod.loading_indicator = True
 
 colormaps = stereo_conf.linear_colormaps
 
 
@@ -37,15 +39,15 @@
     def __init__(
             self,
             data,
             width: Optional[int] = 500,
             height: Optional[int] = 500,
             bgcolor='#2F2F4F',
     ):
-        self.data = data
+        self.data: StereoExpData = data
         self.width = width
         self.height = height
         self.bgcolor = bgcolor
         if self.data.cells.total_counts is None:
             total_counts = self.data.exp_matrix.sum(axis=1).T.A[
                 0] if self.data.issparse() else self.data.exp_matrix.sum(axis=1).T
         else:
@@ -134,39 +136,123 @@
         # for label in self.selected_exp_data.position.tolist():
         #     x_y = ','.join([str(label[0]), str(label[1])])
         #     if x_y in data_set:
         #         continue
         #     data_set.add(x_y)
         #     list_poly_selection_exp_coors.append(label)
         # return list_poly_selection_exp_coors
+    
+    def generate_gem_file(
+        self,
+        selected_areas: StereoExpData,
+        origin_file_path: str,
+        output_path: str,
+    ):
+        import numba as nb
+        import gzip
+
+        comments_lines, comments = get_gem_comments(origin_file_path)
+
+        original_gem_df = pd.read_csv(origin_file_path, sep='\t', header=comments_lines, engine='pyarrow')
+        original_gem_columns = original_gem_df.columns.copy(deep=True)
+        if 'MIDCounts' in original_gem_df.columns:
+            original_gem_df.rename(columns={'MIDCounts': 'UMICount'}, inplace=True)
+        elif 'MIDCount' in original_gem_df.columns:
+            original_gem_df.rename(columns={'MIDCount': 'UMICount'}, inplace=True)
+        if 'CellID' in original_gem_df.columns:
+            original_gem_df.rename(columns={'CellID': 'cell_id'}, inplace=True)
+        if 'label' in original_gem_df.columns:
+            original_gem_df.rename(columns={'label': 'cell_id'}, inplace=True)
+
+        if selected_areas.bin_type == 'bins':
+            @nb.njit(cache=True, nogil=True, parallel=True)
+            def __get_filtering_flag(data, bin_size, position, bin_coord_offset, num_threads):
+                num_threads = min(position.shape[0], num_threads)
+                num_per_thread = position.shape[0] // num_threads
+                num_left = position.shape[0] % num_threads
+                num_per_thread_list = np.repeat(num_per_thread, num_threads)
+                if num_left > 0:
+                    num_per_thread_list[0:num_left] += 1
+                interval = np.zeros(num_threads + 1, dtype=np.uint32)
+                interval[1:] = np.cumsum(num_per_thread_list)
+                flags = np.zeros((num_threads, data.shape[0]), dtype=np.bool8)
+                x = data[:, 0]
+                y = data[:, 1]
+                count = data[:, 2]
+                for i in nb.prange(num_threads):
+                    start = interval[i]
+                    end = interval[i + 1]
+                    for j in range(start, end):
+                        x_start, y_start = position[j]
+                        if bin_coord_offset:
+                            x_start -= bin_size // 2
+                            y_start -= bin_size // 2
+                        x_end = x_start + bin_size
+                        y_end = y_start + bin_size
+                        flags[i] |= ((x >= x_start) & (x < x_end) & (y >= y_start) & (y < y_end) & (count > 0))
+                flag = flags[0]
+                for f in flags[1:]:
+                    flag |= f
+                return flag
+
+            flag = __get_filtering_flag(
+                original_gem_df[['x', 'y', 'UMICount']].to_numpy(),
+                selected_areas.bin_size,
+                selected_areas.position,
+                selected_areas.bin_coord_offset,
+                nb.get_num_threads(),
+            )
+            selected_gem_df = original_gem_df[flag]
+        elif selected_areas.bin_type == 'cell_bins':
+            original_gem_df['cell_id'] = original_gem_df['cell_id'].astype('U')
+            flag = original_gem_df['cell_id'].isin(selected_areas.cells.cell_name)
+            flag = flag & (original_gem_df['UMICount'] > 0)
+            selected_gem_df = original_gem_df[flag]
+        else:
+            pass
+        selected_gem_df.columns = original_gem_columns
+        
+        if output_path.endswith('.gz'):
+            open_func = gzip.open
+        else:
+            open_func = open
+        with open_func(output_path, 'wb') as fp:
+            fp.writelines(comments)
+            selected_gem_df.to_csv(fp, sep='\t', index=False, mode='wb')
 
     def export_high_res_area(self, origin_file_path: str, output_path: str) -> str:
         """
         export selected area in high resolution
         Args:
             origin_file_path: origin file path which you read
             output_path: location the high res file storaged
         Returns:
             output_path
         """
         # coors = self.get_selected_area_coors()
         if self.selected_exp_data is None:
             raise Exception("No data has been selected, please click the 'export' button beforehand.")
-        coors = self.selected_exp_data.position.tolist()
-        print('coors length: %s' % len(coors))
-        if not coors:
-            raise Exception('Please select the data area first!')
-
         make_dirs(output_path)
-        from gefpy.cgef_adjust_cy import CgefAdjust
-        cg = CgefAdjust()
-        if self.data.bin_type == 'cell_bins':
-            cg.generate_cgef_by_coordinate(origin_file_path, output_path, coors)
+        if self.data.file_format == 'gef':
+            coors = self.selected_exp_data.position.tolist()
+            print('coors length: %s' % len(coors))
+            if not coors:
+                raise Exception('Please select the data area first!')
+
+            
+            from gefpy.cgef_adjust_cy import CgefAdjust
+            cg = CgefAdjust()
+            if self.data.bin_type == 'cell_bins':
+                cg.generate_cgef_by_coordinate(origin_file_path, output_path, coors)
+            else:
+                cg.generate_bgef_by_coordinate(origin_file_path, output_path, coors, self.data.bin_size)
+        elif self.data.file_format == 'gem':
+            self.generate_gem_file(self.selected_exp_data, origin_file_path, output_path)
         else:
-            cg.generate_bgef_by_coordinate(origin_file_path, output_path, coors, self.data.bin_size)
+            raise Exception('Only supports gef and gem file.')
 
         return output_path
 
     def export_roi_image(self, origin_file_path: str, output_path: str):
         if self.selected_areas_vertex is None or len(self.selected_areas_vertex) == 0:
             raise Exception("No data has been selected, please click the 'export' button beforehand.")
         drop = self.drop_checkbox.value
```

### Comparing `stereopy-1.2.0/stereo/plots/interact_plot/spatial_cluster.py` & `stereopy-1.3.0b1/stereo/plots/interact_plot/spatial_cluster.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/marker_genes.py` & `stereopy-1.3.0b1/stereo/plots/marker_genes.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,18 @@
             gene_list = [gene_list]
         if len(gene_list) == 0:
             continue
         gene_names.extend(list(gene_list))
         gene_group_labels.append(label)
         gene_group_positions.append((start, start + len(gene_list) - 1))
         start += len(gene_list)
-    draw_df = data_helper.exp_matrix2df(data, gene_name=np.array(gene_names))
+    if marker_res['parameters']['use_raw']:
+        draw_df = data_helper.exp_matrix2df(data.raw, gene_name=np.array(gene_names))
+    else:
+        draw_df = data_helper.exp_matrix2df(data, gene_name=np.array(gene_names))
     draw_df = pd.concat([draw_df, group], axis=1)
     draw_df['group'] = draw_df['group'].astype('category')
     draw_df = draw_df.set_index(['group'])
     draw_df = draw_df.sort_index()
     if min_value is not None or max_value is not None:
         draw_df.clip(lower=min_value, upper=max_value, inplace=True)
     return draw_df, gene_group_labels, gene_group_positions
@@ -382,15 +385,15 @@
             pct: pd.DataFrame = self.marker_genes_res['pct']
         pct = pct.set_index('genes')
         # marker_genes_res_dict = self._store_marker_genes_result_by_group()
         # mean_expressin_in_group = pipeline_utils.cell_cluster_to_gene_exp_cluster(
         #     self.data, self.marker_genes_parameters['cluster_res_key'], kind='mean')
         
         for g in groups:
-            if 'mean_count' not in marker_genes_res_dict[g].columns:
+            if g in marker_genes_res_dict and 'mean_count' not in marker_genes_res_dict[g].columns:
                 genes = marker_genes_res_dict[g].index
                 marker_genes_res_dict[g]['mean_count'] = mean_expressin_in_group[g].loc[genes].to_numpy()
             dot_size = pct[g].loc[gene_names].to_numpy() * 100
             if values_to_plot is None:
                 # yield pct[g][gene_index].values * 100, mean_expressin_in_group[g][gene_index].values
                 dot_color = mean_expressin_in_group[g].loc[gene_names].to_numpy()
             else:
@@ -441,15 +444,15 @@
         gene_intervals = []
         marker_genes_group_keys_to_show = []
         df_list = []
         if sort_by == 'logfoldchanges':
             sort_by = 'log2fc'
         marker_genes_res_dict = self._store_marker_genes_result_by_group()
         mean_expressin_in_group = pipeline_utils.cell_cluster_to_gene_exp_cluster(
-            self.data, self.marker_genes_parameters['cluster_res_key'], kind='mean')
+            self.data, self.marker_genes_parameters['cluster_res_key'], kind='mean', filter_raw=False)
         for mg_key in marker_genes_group_keys:
             if genes is None:
                 topn_res = self.marker_genes_res[mg_key].sort_values(by=sort_by, ascending=False).head(markers_num)
             else:
                 if isinstance(genes, str):
                     genes = [genes]
                 isin = self.marker_genes_res[mg_key]['genes'].isin(genes)
```

### Comparing `stereopy-1.2.0/stereo/plots/ms_plot.py` & `stereopy-1.3.0b1/stereo/plots/ms_plot.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/ms_plot_base.py` & `stereopy-1.3.0b1/stereo/plots/ms_plot_base.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/plot_base.py` & `stereopy-1.3.0b1/stereo/plots/plot_base.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/plot_ccd.py` & `stereopy-1.3.0b1/stereo/plots/plot_ccd.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/plot_cells.py` & `stereopy-1.3.0b1/stereo/plots/plot_cells.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/plot_cluster_traj/interp.py` & `stereopy-1.3.0b1/stereo/plots/plot_cluster_traj/interp.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/plot_cluster_traj/plot_cluster_traj.py` & `stereopy-1.3.0b1/stereo/plots/plot_cluster_traj/plot_cluster_traj.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/plot_cluster_traj/traj.py` & `stereopy-1.3.0b1/stereo/plots/plot_cluster_traj/traj.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/plot_cluster_traj_3d/interp.py` & `stereopy-1.3.0b1/stereo/plots/plot_cluster_traj_3d/interp.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/plot_cluster_traj_3d/plot_cluster_traj_3d.py` & `stereopy-1.3.0b1/stereo/plots/plot_cluster_traj_3d/plot_cluster_traj_3d.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/plot_cluster_traj_3d/traj.py` & `stereopy-1.3.0b1/stereo/plots/plot_cluster_traj_3d/traj.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/plot_clusters_heatmap.py` & `stereopy-1.3.0b1/stereo/plots/plot_clusters_heatmap.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/plot_clusters_scatter.py` & `stereopy-1.3.0b1/stereo/plots/plot_clusters_scatter.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/plot_collection.py` & `stereopy-1.3.0b1/stereo/plots/plot_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,16 +333,16 @@
             self,
             cells_key: Optional[list] = ["total_counts", "n_genes_by_counts"],
             ncols: Optional[int] = 2,
             dot_size: Optional[int] = None,
             palette: Optional[str] = 'stereo',
             width: Optional[int] = None,
             height: Optional[int] = None,
-            x_label: Optional[list] = ['spatial1', 'spatial1'],
-            y_label: Optional[list] = ['spatial2', 'spatial2'],
+            x_label: Optional[Union[list, str]] = 'spatial1',
+            y_label: Optional[Union[list, str]] = 'spatial2',
             title: Optional[str] = None,
             vmin: float = None,
             vmax: float = None,
             **kwargs
     ):
         """
         Spatial distribution of `total_counts` and `n_genes_by_counts`.
@@ -367,19 +367,23 @@
                                 | data5 ...  
                                 | ...   ...  
                                 ---------------
                 if set it to `False`, the coordinates will not be changed.
         :param horizontal_offset_additional: the additional offset between each slice on horizontal direction while reorganizing coordinates.
         :param vertical_offset_additional: the additional offset between each slice on vertical direction while reorganizing coordinates.
         :param vmin: The value representing the lower limit of the color scale. Values smaller than vmin are plotted with the same color as vmin.
-        :param vmax: The value representing the lower limit of the color scale. Values smaller than vmin are plotted with the same color as vmin.
+        :param vmax: The value representing the higher limit of the color scale. Values greater than vmax are plotted with the same color as vmax.
         """  # noqa
         from .scatter import multi_scatter
         if title is None:
             title = [' '.join(i.split('_')) for i in cells_key]
+        if isinstance(x_label, str):
+            x_label = [x_label] * len(cells_key)
+        if isinstance(y_label, str):
+            y_label = [y_label] * len(cells_key)
         fig = multi_scatter(
             x=self.data.position[:, 0],
             y=self.data.position[:, 1],
             hue=[self.data.cells.get_property(key) for key in cells_key],
             x_label=x_label,
             y_label=y_label,
             title=title,
@@ -435,15 +439,15 @@
                 if set it to `False`, the coordinates will not be changed.
         :param horizontal_offset_additional: the additional offset between each slice on horizontal direction while reorganizing coordinates.
         :param vertical_offset_additional: the additional offset between each slice on vertical direction while reorganizing coordinates.
         :param x_label: the x label.
         :param y_label: the y label.
         :param title: the title label.
         :param vmin: The value representing the lower limit of the color scale. Values smaller than vmin are plotted with the same color as vmin.
-        :param vmax: The value representing the lower limit of the color scale. Values smaller than vmin are plotted with the same color as vmin.
+        :param vmax: The value representing the higher limit of the color scale. Values greater than vmax are plotted with the same color as vmax.
 
         """  # noqa
         self.data.array2sparse()
         if isinstance(gene_name, str):
             gene_name = [gene_name]
         gene_idx = [np.argwhere(self.data.gene_names == gn)[0][0] for gn in gene_name]
         hue = self.data.exp_matrix[:, gene_idx].T
@@ -510,15 +514,15 @@
                                 | data5 ...  
                                 | ...   ...  
                                 ---------------
                 if set it to `False`, the coordinates will not be changed.
         :param horizontal_offset_additional: the additional offset between each slice on horizontal direction while reorganizing coordinates.
         :param vertical_offset_additional: the additional offset between each slice on vertical direction while reorganizing coordinates.
         :param vmin: The value representing the lower limit of the color scale. Values smaller than vmin are plotted with the same color as vmin.
-        :param vmax: The value representing the lower limit of the color scale. Values smaller than vmin are plotted with the same color as vmin.
+        :param vmax: The value representing the higher limit of the color scale. Values greater than vmax are plotted with the same color as vmax.
         """  # noqa
         if gene_name is None:
             idx = randint(0, len(self.data.tl.raw.gene_names) - 1)
             gene_name = self.data.gene_names[idx]
         else:
             if gene_name not in self.data.gene_names:
                 raise Exception(f'gene {gene_name} do not exist in expression matrix')
@@ -786,15 +790,15 @@
         :param colors: the color list.
         :param width: the figure width in pixels.
         :param height: the figure height in pixels.
         :param palette: color theme.
         :param out_path: the path to save the figure.
         :param out_dpi: the dpi when the figure is saved.
         :param vmin: The value representing the lower limit of the color scale. Values smaller than vmin are plotted with the same color as vmin.
-        :param vmax: The value representing the lower limit of the color scale. Values smaller than vmin are plotted with the same color as vmin.
+        :param vmax: The value representing the higher limit of the color scale. Values greater than vmax are plotted with the same color as vmax.
 
         """  # noqa
         res = self.check_res_key(res_key)
         if cluster_key:
             cluster_res = self.check_res_key(cluster_key)
             n = len(set(cluster_res['group']))
             if title is None:
@@ -841,14 +845,15 @@
     @plot_scale
     @reorganize_coordinate
     def cluster_scatter(
             self,
             res_key: str,
             groups: Optional[Union[str, list, np.ndarray]] = None,
             show_others: Optional[bool] = None,
+            others_color: Optional[str] = '#828282',
             title: Optional[str] = None,
             x_label: Optional[str] = None,
             y_label: Optional[str] = None,
             dot_size: Optional[int] = None,
             colors: Optional[str] = 'stereo_30',
             invert_y: Optional[bool] = True,
             hue_order: Optional[set] = None,
@@ -856,27 +861,33 @@
             height: Optional[int] = None,
             base_image: Optional[str] = None,
             base_im_cmap: Optional[str] = 'Greys',
             base_im_to_gray : bool = False,
             **kwargs
     ):
         """
-        Spatial distribution ofter scatter.
+        Spatial scatter distribution of clusters.
 
         :param res_key: cluster result key.
         :param groups: the group names.
+        :param show_others: whether to show others when groups is not None.
+                            by default, if `base_image` is None, `show_others` is True, otherwise `show_others` is False.
+        :param others_color: the color of others, only available when `groups` is not None and `show_others` is True.
         :param title: the plot title.
         :param x_label: the x label.
         :param y_label: the y label.
         :param dot_size: the dot size.
         :param colors: the color list.
         :param invert_y: whether to invert y-axis.
         :param hue_order: the classification method.
         :param width: the figure width in pixels.
         :param height: the figure height in pixels.
+        :param base_image: the path of mask image to be displayed as background, it must already be registered to the same coordinate system as the data.
+        :param base_im_cmap: the color map of the base image, only availabel when base image is gray scale image.
+        :param base_im_to_gray: whether to convert the base image to gray scale if base image is RGB/RGBA image.
         :param show_plotting_scale: wheter to display the plotting scale.
         :param out_path: the path to save the figure.
         :param out_dpi: the dpi when the figure is saved.
         :param reorganize_coordinate: if the data is merged from several slices, whether to reorganize the coordinates of the obs(cells), 
                 if set it to a number, like 2, the coordinates will be reorganized to 2 columns on coordinate system as below:
                                 ---------------
                                 | data1 data2
@@ -887,15 +898,15 @@
                 if set it to `False`, the coordinates will not be changed.
         :param horizontal_offset_additional: the additional offset between each slice on horizontal direction while reorganizing coordinates.
         :param vertical_offset_additional: the additional offset between each slice on vertical direction while reorganizing coordinates.
 
         :return: Spatial scatter distribution of clusters.
         """  # noqa
         res = self.check_res_key(res_key)
-        group_list = res['group'].to_numpy()
+        group_list = res['group'].to_numpy(copy=True)
         n = np.unique(group_list).size
         palette = stereo_conf.get_colors(colors, n=n)
         x = self.data.position[:, 0]
         y = self.data.position[:, 1]
         x_min, x_max = int(x.min()), int(x.max())
         y_min, y_max = int(y.min()), int(y.max())
         boundary = [x_min, x_max, y_min, y_max]
@@ -911,15 +922,15 @@
                     if base_image is None:
                         show_others = True
                     else:
                         show_others = False
                 if show_others:
                     group_list[~isin] = 'others'
                     n = np.unique(group_list).size
-                    palette = palette[0:n - 1] + ['#828282']
+                    palette = palette[0:n - 1] + [others_color]
                     hue_order = natsorted(np.unique(group_list[isin])) + ['others']
                 else:
                     group_list = group_list[isin]
                     n = np.unique(group_list).size
                     palette = palette[0:n]
                     hue_order = natsorted(np.unique(group_list))
                     x = x[isin]
@@ -1205,15 +1216,15 @@
         :param palette: Color theme, defaults to `'CET_L4'`.
         :param width: the figure width in pixels.
         :param height: the figure height in pixels.
         :param out_path: the path to save the figure.
         :param out_dpi: the dpi when the figure is saved.
         :param title: the plot title.
         :param vmin: The value representing the lower limit of the color scale. Values smaller than vmin are plotted with the same color as vmin.
-        :param vmax: The value representing the lower limit of the color scale. Values smaller than vmin are plotted with the same color as vmin.
+        :param vmax: The value representing the higher limit of the color scale. Values greater than vmax are plotted with the same color as vmax.
         """  # noqa
         res = self.check_res_key(res_key)
         scores = [res.module_scores[module] for module in range(1, res.modules.max() + 1)]
         vmin = np.percentile(scores, 1) if not vmin else vmin
         vmax = np.percentile(scores, 99) if not vmax else vmax
         title = [f"module {module}" for module in
                  range(1, res.modules.max() + 1)] if title is None and title != '' else title
```

### Comparing `stereopy-1.2.0/stereo/plots/plot_coo.py` & `stereopy-1.3.0b1/stereo/plots/plot_coo.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/plot_dendrogram.py` & `stereopy-1.3.0b1/stereo/plots/plot_dendrogram.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/plot_elbow.py` & `stereopy-1.3.0b1/stereo/plots/plot_elbow.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/plot_genes_in_pseudotime.py` & `stereopy-1.3.0b1/stereo/plots/plot_genes_in_pseudotime.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/plot_paga.py` & `stereopy-1.3.0b1/stereo/plots/plot_paga.py`

 * *Files 17% similar despite different names*

```diff
@@ -382,29 +382,29 @@
                 ig_layout = g.layout(layout, root=root, **kwds)
             else:
                 ig_layout = g.layout(layout, **kwds)
             positions = np.array(ig_layout.coords)
         self.stereo_exp_data.cells_matrix['paga_pos'] = positions
         return positions
 
-    def paga_compare(
+    def draw_graph(
             self,
             adjacency: str = 'connectivities_tree',
             color: Optional[str] = None,
             size: int = 1,
             threshold: float = 0.01,
             layout: _Layout = 'fr',
             random_state: int = 0,
             cmap: str = 'tab20',
             width: int = 15,
             height: int = 6,
             dot_size: int = 30
     ):
         """
-        abstract paga plot for the paga result and cell distribute around paga.
+        Force-directed graph drawing
 
         :param adjacency: keyword to use for paga or paga tree, available values include 'connectivities' and 'connectivities_tree'. # noqa
         :param color: the col in cells or a gene name to display in compare plot.
         :param size: cell spot size.
         :param threshold: prune edges lower than threshold.
         :param layout: the method to layout each node.
         :param random_state: to control the random initialization.
@@ -436,14 +436,126 @@
 
         if color in self.stereo_exp_data.cells:
             if self.stereo_exp_data.cells[color].dtype == 'category':
                 ax.scatter(cell_pos[:, 0], cell_pos[:, 1], s=size,
                            c=self.stereo_exp_data.cells[color].cat.codes.to_numpy(), cmap=cmap)
                 cell_pos_df = pd.DataFrame(cell_pos)
                 cell_pos_df[color] = self.stereo_exp_data.cells[color].to_list()
+                cell_center_pos_df = cell_pos_df.groupby(color).mean()
+                for s, row in cell_center_pos_df.iterrows():
+                    ax.text(row[0], row[1], s)
+            else:
+                ax.scatter(cell_pos[:, 0], cell_pos[:, 1], s=size, c=self.stereo_exp_data.cells[color])
+        elif color in self.stereo_exp_data.gene_names:
+            gene_list = list(self.stereo_exp_data.genes.to_df().index)
+            gene_index = gene_list.index(color)
+            clist = self.stereo_exp_data.exp_matrix[:, gene_index]
+            ax.scatter(cell_pos[:, 0], cell_pos[:, 1], s=size, c=clist)
+
+        ax.set_xticks([])
+        ax.set_yticks([])
+        return fig
+
+    def paga_compare(
+            self,
+            basis: Optional[str] = None,
+            adjacency: str = 'connectivities_tree',
+            color: Optional[str] = None,
+            size: int = 1,
+            threshold: float = 0.01,
+            cmap: str = 'tab20',
+            width: int = 15,
+            height: int = 6,
+            dot_size: int = 30
+    ):
+        """
+        abstract paga plot for the paga result and cell distribute around paga.
+
+        :param basis: the embedding of cells, default
+        :param adjacency: keyword to use for paga or paga tree, available values include 'connectivities' and 'connectivities_tree'. # noqa
+        :param color: the col in cells or a gene name to display in compare plot.
+        :param size: cell spot size.
+        :param threshold: prune edges lower than threshold.
+        :param cmap: colormap to use, default with tab20.
+        :param width: the figure width.
+        :param height: the figure height.
+        :param dot_size: The marker size in points**2 (typographic points are 1/72 in.).
+            Default is 30.
+
+        """
+
+        if color is None:
+            color = self.pipeline_res['paga']['groups']
+        if (color not in self.stereo_exp_data.cells) and (color not in self.stereo_exp_data.gene_names):
+            logger.info(
+                f"color is neither in cells nor in genes, use '{self.pipeline_res['paga']['groups']}' as default")
+            color = self.pipeline_res['paga']['groups']
+
+        if basis is None:
+            basis = 'umap'
+        if basis not in self.pipeline_res:
+            logger.info(
+                f"{basis} is not in result, use 'umap' as default")
+            basis = 'umap'
+            if basis not in self.pipeline_res:
+                logger.info(
+                    f"umap is not in result, please run umap first, try to use 'pca' instead")
+                basis = 'pca'
+                if basis not in self.pipeline_res:
+                    logger.info(
+                        f"pca is not in result, please specify a dim reduction result, try to run pca or umap first.")
+                    raise KeyError("basis not found: " + str(basis))
+
+        df = self.pipeline_res[basis].copy()
+        df = df[[0, 1]]
+        df[color] = list(self.stereo_exp_data.cells[color])
+        pos = df.groupby(color).mean()
+
+        # calculate node positions
+        adjacency_mat = self.pipeline_res['paga'][adjacency].copy()
+        if threshold > 0:
+            adjacency_mat.data[adjacency_mat.data < threshold] = 0
+            adjacency_mat.eliminate_zeros()
+
+        # network
+        G = pd.DataFrame(adjacency_mat.todense())
+        ct_list = self.stereo_exp_data.cells[color].cat.categories
+
+        pos = pos.loc[ct_list]
+        pos = pos.to_numpy()
+
+        G.index = ct_list
+        G.columns = ct_list
+        Edges = nx.from_pandas_adjacency(G).edges()
+        Nodes2pos = dict(zip(ct_list, list(pos)))
+
+        # parameter setting
+        fig = plt.figure(figsize=(width, height))
+        ax = plt.subplot(1, 2, 1)
+        # network
+        color_list = plt.get_cmap(cmap, len(ct_list))
+        ax.scatter(pos[:, 0], pos[:, 1], c=color_list.colors, zorder=1, s=dot_size)
+        for i in range(len(ct_list)):
+            ax.text(pos[i, 0], pos[i, 1], s=ct_list[i], zorder=2)
+        for i, j in Edges:
+            xi, yi = Nodes2pos[i]
+            xj, yj = Nodes2pos[j]
+            ax.plot([xi, xj], [yi, yj], color='black', zorder=0)
+
+        # plotting
+        ax = plt.subplot(1, 2, 2)
+
+        cell_pos = df[[0, 1]].to_numpy()
+
+        if color in self.stereo_exp_data.cells:
+            if self.stereo_exp_data.cells[color].dtype == 'category':
+                ax.scatter(cell_pos[:, 0], cell_pos[:, 1], s=size,
+                           c=self.stereo_exp_data.cells[color].cat.codes.to_numpy(), cmap=cmap)
+                cell_pos_df = pd.DataFrame(cell_pos)
+                cell_pos_df[color] = self.stereo_exp_data.cells[color].to_list()
                 cell_center_pos_df = cell_pos_df.groupby(color).mean()
                 for s, row in cell_center_pos_df.iterrows():
                     ax.text(row[0], row[1], s)
             else:
                 ax.scatter(cell_pos[:, 0], cell_pos[:, 1], s=size, c=self.stereo_exp_data.cells[color])
         elif color in self.stereo_exp_data.gene_names:
             gene_list = list(self.stereo_exp_data.genes.to_df().index)
```

### Comparing `stereopy-1.2.0/stereo/plots/plot_time_series.py` & `stereopy-1.3.0b1/stereo/plots/plot_time_series.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/plot_vec/plot_vec.py` & `stereopy-1.3.0b1/stereo/plots/plot_vec/plot_vec.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/plot_vec/vec.py` & `stereopy-1.3.0b1/stereo/plots/plot_vec/vec.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/plot_vec_3d/plot_vec_3d.py` & `stereopy-1.3.0b1/stereo/plots/plot_vec_3d/plot_vec_3d.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/plot_vec_3d/vec.py` & `stereopy-1.3.0b1/stereo/plots/plot_vec_3d/vec.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/scatter.py` & `stereopy-1.3.0b1/stereo/plots/scatter.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/violin.py` & `stereopy-1.3.0b1/stereo/plots/violin.py`

 * *Files 3% similar despite different names*

```diff
@@ -185,15 +185,15 @@
             df[added_k] = val.loc[:, idx]
 
     return df
 
 
 def violin_distribution(
         data,
-        keys: [str, Iterable] = None,
+        keys: Union[str, Iterable] = None,
         x_label: str = '',
         y_label: Optional[str] = None,
         show_stripplot: Optional[bool] = True,
         jitter: Optional[float] = 0.2,
         dot_size: Optional[float] = 0.8,
         log: Optional[bool] = False,
         rotation_angle: Optional[int] = 0,
@@ -216,17 +216,17 @@
     :param show_stripplot: whether to overlay a stripplot of specific percentage values.
     :param jitter: adjust the dispersion of points.
     :param dot_size: dot size.
     :param log: plot a graph on a logarithmic axis.
     :param rotation_angle: rotation of xtick labels.
     :param group_by: the key of the observation grouping to consider.
     :param multi_panel: Display keys in multiple panels also when groupby is not None.
-    :param scale: The method used to scale the width of each violin. If ‘width’ (the default), each violin will
-            have the same width. If ‘area’, each violin will have the same area.
-            If ‘count’, a violin’s width corresponds to the number of observations.
+    :param scale: The method used to scale the width of each violin. If 'width' (the default), each violin will
+            have the same width. If 'area', each violin will have the same area.
+            If 'count', a violin's width corresponds to the number of observations.
     :param ax: a matplotlib axes object. only works if plotting a single component.
     :param order: Order in which to show the categories.
     :param use_raw: Whether to use raw attribute of adata. Defaults to True if .raw is present.
     :param palette: color theme.
     :param title: the title.
 
     :return: None
@@ -277,14 +277,15 @@
             col_order=keys,
             sharey=False,
             order=keys,
             cut=0,
             inner=None,
             palette=palette
         )
+        fig = g.figure
 
         if show_stripplot:
             grouped_df = obs_df.groupby(x)
             for ax_id, key in zip(range(g.axes.shape[1]), keys):
                 sns.stripplot(
                     y=y,
                     data=grouped_df.get_group(key),
@@ -303,14 +304,15 @@
             for ax in g.axes[0]:
                 ax.tick_params(axis='x', labelrotation=rotation_angle)
     else:
         if ax is None:
             axs = setup_axes(ax=ax, panels=['x'] if group_by is None else keys, show_ticks=True, right_margin=0.3, )[0]
         else:
             axs = [ax]
+        fig = axs[0].figure
         for ax, y, ylab in zip(axs, ys, y_label):
             ax = sns.violinplot(x=x, y=y, data=obs_df, order=order, orient='vertical', scale=scale, ax=ax,
                                 palette=palette)
             if show_stripplot:
                 ax = sns.stripplot(
                     x=x,
                     y=y,
@@ -328,15 +330,16 @@
                 ax.set_ylabel(ylab)
             if log:
                 ax.set_yscale('log')
             if rotation_angle is not None:
                 ax.tick_params(axis='x', labelrotation=rotation_angle)
             if title:
                 ax.set_title(title.pop(0) if title else '')
-    pl.show()
+    return fig
+    # pl.show()
 
 
 def setup_axes(
         ax: Union[Axes, Sequence[Axes]] = None,
         panels='blue',
         colorbars=False,
         right_margin=None,
@@ -345,15 +348,15 @@
         show_ticks=False,
 ):
     """Grid of axes for plotting, legends and colorbars."""
     if projection not in {"2d", "3d"}:
         raise ValueError(f"Projection must be '2d' or '3d', was '{projection}'.")
 
     if left_margin is not None:
-        raise NotImplementedError('We currently don’t support `left_margin`.')
+        raise NotImplementedError("We currently don't support `left_margin`.")
 
     if np.any(colorbars) and right_margin is None:
         right_margin = 1 - rcParams['figure.subplot.right'] + 0.21
     elif right_margin is None:
         right_margin = 1 - rcParams['figure.subplot.right'] + 0.06
 
     # make a list of right margins for each panel
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `stereopy-1.2.0/stereo/plots/vt3d_browser/PAGA_traj.py` & `stereopy-1.3.0b1/stereo/plots/vt3d_browser/PAGA_traj.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/vt3d_browser/README.md` & `stereopy-1.3.0b1/stereo/plots/vt3d_browser/README.md`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/vt3d_browser/example.py` & `stereopy-1.3.0b1/stereo/plots/vt3d_browser/example.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/vt3d_browser/examples/example_ccc.ipynb` & `stereopy-1.3.0b1/stereo/plots/vt3d_browser/examples/example_ccc.ipynb`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/vt3d_browser/examples/example_grn.ipynb` & `stereopy-1.3.0b1/stereo/plots/vt3d_browser/examples/example_grn.ipynb`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/vt3d_browser/examples/example_mesh.ipynb` & `stereopy-1.3.0b1/stereo/plots/vt3d_browser/examples/example_mesh.ipynb`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/vt3d_browser/examples/example_paga.ipynb` & `stereopy-1.3.0b1/stereo/plots/vt3d_browser/examples/example_paga.ipynb`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/vt3d_browser/stereopy_3D_browser.py` & `stereopy-1.3.0b1/stereo/plots/vt3d_browser/stereopy_3D_browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 import math
 import os
 import re
 import time
 from http.server import BaseHTTPRequestHandler
 from http.server import HTTPServer
 from io import StringIO
+from copy import deepcopy
 
 import numpy as np
 import pandas as pd
 from IPython.display import IFrame
 from natsort import natsorted
 from scipy import stats
 
 from stereo.core.stereo_exp_data import StereoExpData
+from stereo.preprocess import filter_genes
 from .PAGA_traj import cal_plt_param_traj_clus_from_adata
 
 
 # import anndata as ad
 
 def updateItem(item):
     if isinstance(item, str):
@@ -650,14 +652,15 @@
     :param exp_cutoff: the expression threshold to filter un-expression cells.
     :param width: the window width to render
     :param height: the window height to render
     :parma port: the port id
 
     :return:
     """  # noqa
+    data = deepcopy(data)
     if paga_key is None and grn_key is None and ccc_key is None:
         raise Exception
 
     if grn_key is None:
         if paga_key is not None:
             cluster_label = data.tl.result[paga_key]['groups']
         else:
@@ -677,15 +680,16 @@
                 return
         elif isinstance(meshfile, dict):
             continue
         else:
             print(f'invalid mesh data :{meshfile}, return without any data browsing server...')
     # filter by geneset now
     if geneset is not None:
-        data = data.sub_by_name(gene_name=geneset)  # notice, invalid gene will case program raising exceptions
+        # data = data.sub_by_name(gene_name=geneset)  # notice, invalid gene will case program raising exceptions
+        filter_genes(data, gene_list=geneset, inplace=True)
     data.genes.gene_name = UpdateList(data.genes.gene_name, return_ndarray=True).astype('U')
     # create core datacache
     datacache = Stereo3DWebCache(data, meshes, cluster_label, spatial_label, exp_cutoff, paga_key, grn_key, ccc_key)
     ServerInstance.data_hook = datacache
     ServerInstance.front_dir = os.path.dirname(os.path.abspath(__file__)) + '/vt3d_browser'
     print(f'Current front-dir is {ServerInstance.front_dir}', flush=True)
     # create webserver
```

### Comparing `stereopy-1.2.0/stereo/plots/vt3d_browser/vt3d_browser/535877f50039c0cb49a6196a5b7517cd.woff` & `stereopy-1.3.0b1/stereo/plots/vt3d_browser/vt3d_browser/535877f50039c0cb49a6196a5b7517cd.woff`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/vt3d_browser/vt3d_browser/6f0a76321d30f3c8120915e57f7bd77e.ttf` & `stereopy-1.3.0b1/stereo/plots/vt3d_browser/vt3d_browser/6f0a76321d30f3c8120915e57f7bd77e.ttf`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/vt3d_browser/vt3d_browser/732389ded34cb9c52dd88271f1345af9.ttf` & `stereopy-1.3.0b1/stereo/plots/vt3d_browser/vt3d_browser/732389ded34cb9c52dd88271f1345af9.ttf`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/vt3d_browser/vt3d_browser/index.js` & `stereopy-1.3.0b1/stereo/plots/vt3d_browser/vt3d_browser/index.js`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/vt3d_browser/vt3d_browser/index.js.map` & `stereopy-1.3.0b1/stereo/plots/vt3d_browser/vt3d_browser/index.js.map`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/vt3d_browser/vt3d_browser/manifest.js` & `stereopy-1.3.0b1/stereo/plots/vt3d_browser/vt3d_browser/manifest.js`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/vt3d_browser/vt3d_browser/manifest.js.map` & `stereopy-1.3.0b1/stereo/plots/vt3d_browser/vt3d_browser/manifest.js.map`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/vt3d_browser/vt3d_browser/vendor.js` & `stereopy-1.3.0b1/stereo/plots/vt3d_browser/vt3d_browser/vendor.js`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/plots/vt3d_browser/vt3d_browser/vendor.js.map` & `stereopy-1.3.0b1/stereo/plots/vt3d_browser/vt3d_browser/vendor.js.map`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/preprocess/filter.py` & `stereopy-1.3.0b1/stereo/preprocess/filter.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,39 +51,37 @@
     :return: StereoExpData object.
     """
     data = data if inplace else copy.deepcopy(data)
     if min_gene is None and max_gene is None and cell_list is None and min_n_genes_by_counts is None \
             and max_n_genes_by_counts is None and pct_counts_mt is None:
         raise ValueError('At least one filter must be set.')
     cal_cells_indicators(data)
+    cell_subset = np.ones(data.cells.size, dtype=np.bool8)
     if min_gene:
-        cell_subset = data.cells.total_counts >= min_gene
-        data.sub_by_index(cell_index=cell_subset)
+        cell_subset &= data.cells.total_counts >= min_gene
     if max_gene:
-        cell_subset = data.cells.total_counts <= max_gene
-        data.sub_by_index(cell_index=cell_subset)
+        cell_subset &= data.cells.total_counts <= max_gene
     if min_n_genes_by_counts:
-        cell_subset = data.cells.n_genes_by_counts >= min_n_genes_by_counts
-        data.sub_by_index(cell_index=cell_subset)
+        cell_subset &= data.cells.n_genes_by_counts >= min_n_genes_by_counts
     if max_n_genes_by_counts:
-        cell_subset = data.cells.n_genes_by_counts <= max_n_genes_by_counts
-        data.sub_by_index(cell_index=cell_subset)
+        cell_subset &= data.cells.n_genes_by_counts <= max_n_genes_by_counts
     if pct_counts_mt:
-        cell_subset = data.cells.pct_counts_mt <= pct_counts_mt
-        data.sub_by_index(cell_index=cell_subset)
+        cell_subset &= data.cells.pct_counts_mt <= pct_counts_mt
     if cell_list is not None:
-        cell_subset = np.isin(data.cells.cell_name, cell_list)
-        data.sub_by_index(cell_index=cell_subset)
+        cell_subset &= np.isin(data.cells.cell_name, cell_list)
+    data.sub_by_index(cell_index=cell_subset)
     return data
 
 
 def filter_genes(
         data: StereoExpData,
         min_cell=None,
         max_cell=None,
+        min_count=None,
+        max_count=None,
         gene_list=None,
         mean_umi_gt=None,
         inplace=True
 ):
     """
     filter genes based on the numbers of cells.
 
@@ -93,29 +91,33 @@
     :param mean_umi_gt: Filter genes whose mean umi greater than this value.
     :param gene_list: the list of genes which will be filtered.
     :param inplace: whether inplace the original data or return a new data.
 
     :return: StereoExpData object.
     """
     data = data if inplace else copy.deepcopy(data)
-    if min_cell is None and max_cell is None and gene_list is None and mean_umi_gt is None:
-        raise ValueError('please set any of `min_cell` or `max_cell` or `gene_list` or `mean_umi_gt`')
+    if min_cell is None and max_cell is None \
+        and min_count is None and max_count is None \
+        and gene_list is None and mean_umi_gt is None:
+        raise ValueError('please set any of `min_cell`, `max_cell`, `min_count`, `max_count`, `gene_list` and `mean_umi_gt`')
     cal_genes_indicators(data)
+    gene_subset = np.ones(data.genes.size, dtype=np.bool8)
     if min_cell:
-        gene_subset = data.genes.n_cells >= min_cell
-        data.sub_by_index(gene_index=gene_subset)
+        gene_subset &= data.genes.n_cells >= min_cell
     if max_cell:
-        gene_subset = data.genes.n_cells <= max_cell
-        data.sub_by_index(gene_index=gene_subset)
+        gene_subset &= data.genes.n_cells <= max_cell
+    if min_count:
+        gene_subset &= data.genes.n_counts >= min_count
+    if max_count:
+        gene_subset &= data.genes.n_counts <= max_count
     if gene_list is not None:
-        gene_subset = np.isin(data.gene_names, gene_list)
-        data.sub_by_index(gene_index=gene_subset)
+        gene_subset &= np.isin(data.gene_names, gene_list)
     if mean_umi_gt is not None:
-        gene_subset = data.genes.mean_umi > mean_umi_gt
-        data.sub_by_index(gene_index=gene_subset)
+        gene_subset &= data.genes.mean_umi > mean_umi_gt
+    data.sub_by_index(gene_index=gene_subset)
     return data
 
 
 def filter_coordinates(
         data: StereoExpData,
         min_x=None,
         max_x=None,
```

### Comparing `stereopy-1.2.0/stereo/preprocess/normalize.py` & `stereopy-1.3.0b1/stereo/preprocess/normalize.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/preprocess/qc.py` & `stereopy-1.3.0b1/stereo/preprocess/qc.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/scripts/ccd.py` & `stereopy-1.3.0b1/stereo/scripts/ccd.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/stereo_config.py` & `stereopy-1.3.0b1/stereo/stereo_config.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/tools/LR_interaction.py` & `stereopy-1.3.0b1/stereo/tools/LR_interaction.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/tools/boundary.py` & `stereopy-1.3.0b1/stereo/tools/boundary.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/tools/cell_correct.py` & `stereopy-1.3.0b1/stereo/tools/cell_correct.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/tools/cell_cut.py` & `stereopy-1.3.0b1/stereo/tools/cell_cut.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/tools/cell_segment.py` & `stereopy-1.3.0b1/stereo/tools/cell_segment.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/tools/cell_type_anno.py` & `stereopy-1.3.0b1/stereo/tools/cell_type_anno.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/tools/cluster.py` & `stereopy-1.3.0b1/stereo/tools/cluster.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/tools/clustering.py` & `stereopy-1.3.0b1/stereo/tools/clustering.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/tools/dim_reduce.py` & `stereopy-1.3.0b1/stereo/tools/dim_reduce.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/tools/find_markers.py` & `stereopy-1.3.0b1/stereo/tools/find_markers.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/tools/gem_filter.py` & `stereopy-1.3.0b1/stereo/tools/gem_filter.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/tools/highly_variable_genes.py` & `stereopy-1.3.0b1/stereo/tools/highly_variable_genes.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/tools/rna_velocity.py` & `stereopy-1.3.0b1/stereo/tools/rna_velocity.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/tools/spatial_lag.py` & `stereopy-1.3.0b1/stereo/tools/spatial_lag.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/tools/spatial_pattern_score.py` & `stereopy-1.3.0b1/stereo/tools/spatial_pattern_score.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/tools/tissue_extraction.py` & `stereopy-1.3.0b1/stereo/tools/tissue_extraction.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/utils/_download.py` & `stereopy-1.3.0b1/stereo/utils/_download.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/utils/correlation.py` & `stereopy-1.3.0b1/stereo/utils/correlation.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/utils/hvg_utils.py` & `stereopy-1.3.0b1/stereo/utils/hvg_utils.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/utils/pipeline_utils.py` & `stereopy-1.3.0b1/stereo/utils/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/utils/read_write_utils.py` & `stereopy-1.3.0b1/stereo/utils/read_write_utils.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/utils/spmatrix_helper.py` & `stereopy-1.3.0b1/stereo/utils/spmatrix_helper.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereo/utils/time_consume.py` & `stereopy-1.3.0b1/stereo/utils/time_consume.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/stereopy.egg-info/PKG-INFO` & `stereopy-1.3.0b1/stereopy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stereopy
-Version: 1.2.0
+Version: 1.3.0b1
 Summary: Spatial transcriptomic analysis in python.
 Home-page: https://github.com/STOmics/Stereopy
 Author: STOmics
 Author-email: tanliwei@stomics.tech
 License: MIT License
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,15 @@
 Requires-Dist: imageio==2.31.1
 Requires-Dist: numpy==1.23.5
 Requires-Dist: matplotlib==3.7.1
 Requires-Dist: pandas>=1.5.3
 Requires-Dist: scipy==1.10.1
 Requires-Dist: seaborn==0.12.2
 Requires-Dist: h5py>=3.7.0
-Requires-Dist: gefpy~=1.1.3
+Requires-Dist: gefpy==1.1.6
 Requires-Dist: setuptools>=61.0.0
 Requires-Dist: numba==0.56.4
 Requires-Dist: statsmodels>=0.14.0
 Requires-Dist: leidenalg>=0.10.1
 Requires-Dist: umap-learn==0.5.1
 Requires-Dist: KDEpy==1.1.0
 Requires-Dist: shapely>=2.0.0
@@ -66,15 +66,15 @@
 Requires-Dist: gtfparse==1.2.1
 Requires-Dist: harmonypy==0.0.6
 Requires-Dist: SQLAlchemy==1.3.24
 Requires-Dist: fbpca>=1.0
 Requires-Dist: geosketch>=1.2
 Requires-Dist: pyscenic>=0.12.1
 Requires-Dist: onnxruntime==1.15.1
-Requires-Dist: POT==0.8.1.0
+Requires-Dist: POT==0.9.1
 Requires-Dist: distinctipy>=1.2.2
 Requires-Dist: joypy>=0.2.6
 Requires-Dist: lxml>=4.8.0
 Requires-Dist: fastcluster>=1.2.6
 Requires-Dist: pycirclize>=0.5.0
 Requires-Dist: plotly>=5.15.0
 Requires-Dist: cusingler
```

### Comparing `stereopy-1.2.0/stereopy.egg-info/SOURCES.txt` & `stereopy-1.3.0b1/stereopy.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 stereo/algorithm/statistics.py
 stereo/algorithm/time_series_analysis.py
 stereo/algorithm/total_vi.py
 stereo/algorithm/umap.py
 stereo/algorithm/batch_qc/__init__.py
 stereo/algorithm/batch_qc/batchqc_raw.py
 stereo/algorithm/batch_qc/main.py
-stereo/algorithm/batch_qc/plot_batch_qc.py
 stereo/algorithm/batch_qc/module/__init__.py
 stereo/algorithm/batch_qc/module/classifier.py
 stereo/algorithm/batch_qc/module/dataset.py
 stereo/algorithm/batch_qc/module/early_stop.py
 stereo/algorithm/batch_qc/module/loss.py
 stereo/algorithm/batch_qc/module/trainer.py
 stereo/algorithm/batch_qc/score/__init__.py
@@ -102,15 +101,14 @@
 stereo/algorithm/ccd/sliding_window.py
 stereo/algorithm/ccd/utils.py
 stereo/algorithm/ccd/assets/favicon.ico
 stereo/algorithm/cell_cell_communication/__init__.py
 stereo/algorithm/cell_cell_communication/analysis_helper.py
 stereo/algorithm/cell_cell_communication/exceptions.py
 stereo/algorithm/cell_cell_communication/main.py
-stereo/algorithm/cell_cell_communication/plot_ccc.py
 stereo/algorithm/cell_cell_communication/spatial_scoloc.py
 stereo/algorithm/cell_cell_communication/utils/__init__.py
 stereo/algorithm/cell_cell_communication/utils/database_utils.py
 stereo/algorithm/cell_cell_communication/utils/sqlalchemy_model.py
 stereo/algorithm/cell_cell_communication/utils/sqlalchemy_repository.py
 stereo/algorithm/cell_cell_communication/utils/visualization_process.py
 stereo/algorithm/cell_pose/__init__.py
@@ -130,26 +128,35 @@
 stereo/algorithm/dpt/struct.py
 stereo/algorithm/paste/__init__.py
 stereo/algorithm/paste/helper.py
 stereo/algorithm/paste/methods.py
 stereo/algorithm/paste/paste.py
 stereo/algorithm/regulatory_network_inference/__init__.py
 stereo/algorithm/regulatory_network_inference/main.py
-stereo/algorithm/regulatory_network_inference/plot_grn.py
 stereo/algorithm/sctransform/__init__.py
 stereo/algorithm/sctransform/bw.py
 stereo/algorithm/sctransform/ksmooth.py
 stereo/algorithm/sctransform/plotting.py
 stereo/algorithm/sctransform/scale_data.py
 stereo/algorithm/sctransform/sctransform.py
 stereo/algorithm/sctransform/utils.py
 stereo/algorithm/sctransform/vst.py
 stereo/algorithm/single_r/__init__.py
 stereo/algorithm/single_r/single_r.py
 stereo/algorithm/single_r/utils.py
+stereo/algorithm/st_gears/__init__.py
+stereo/algorithm/st_gears/calculate_max_kl.py
+stereo/algorithm/st_gears/granularity_adjusting.py
+stereo/algorithm/st_gears/helper.py
+stereo/algorithm/st_gears/main.py
+stereo/algorithm/st_gears/optim_pot.py
+stereo/algorithm/st_gears/recons.py
+stereo/algorithm/st_gears/regis.py
+stereo/algorithm/st_gears/visual.py
+stereo/algorithm/st_gears/weight.py
 stereo/core/__init__.py
 stereo/core/cell.py
 stereo/core/constants.py
 stereo/core/data.py
 stereo/core/gene.py
 stereo/core/ms_data.py
 stereo/core/ms_pipeline.py
@@ -225,24 +232,29 @@
 stereo/io/writer.py
 stereo/plots/__init__.py
 stereo/plots/decorator.py
 stereo/plots/marker_genes.py
 stereo/plots/ms_plot.py
 stereo/plots/ms_plot_base.py
 stereo/plots/plot_base.py
+stereo/plots/plot_batch_qc.py
+stereo/plots/plot_ccc.py
 stereo/plots/plot_ccd.py
 stereo/plots/plot_cells.py
 stereo/plots/plot_clusters_heatmap.py
 stereo/plots/plot_clusters_scatter.py
 stereo/plots/plot_collection.py
 stereo/plots/plot_coo.py
 stereo/plots/plot_dendrogram.py
 stereo/plots/plot_elbow.py
 stereo/plots/plot_genes_in_pseudotime.py
+stereo/plots/plot_grn.py
+stereo/plots/plot_ms_spatial_scatter.py
 stereo/plots/plot_paga.py
+stereo/plots/plot_st_gears.py
 stereo/plots/plot_time_series.py
 stereo/plots/scatter.py
 stereo/plots/violin.py
 stereo/plots/_plot_basic/__init__.py
 stereo/plots/_plot_basic/get_stereo_data.py
 stereo/plots/_plot_basic/heatmap_plt.py
 stereo/plots/interact_plot/__init__.py
```

### Comparing `stereopy-1.2.0/stereopy.egg-info/requires.txt` & `stereopy-1.3.0b1/stereopy.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 imageio==2.31.1
 numpy==1.23.5
 matplotlib==3.7.1
 pandas>=1.5.3
 scipy==1.10.1
 seaborn==0.12.2
 h5py>=3.7.0
-gefpy~=1.1.3
+gefpy==1.1.6
 setuptools>=61.0.0
 numba==0.56.4
 statsmodels>=0.14.0
 leidenalg>=0.10.1
 umap-learn==0.5.1
 KDEpy==1.1.0
 shapely>=2.0.0
@@ -49,15 +49,15 @@
 gtfparse==1.2.1
 harmonypy==0.0.6
 SQLAlchemy==1.3.24
 fbpca>=1.0
 geosketch>=1.2
 pyscenic>=0.12.1
 onnxruntime==1.15.1
-POT==0.8.1.0
+POT==0.9.1
 distinctipy>=1.2.2
 joypy>=0.2.6
 lxml>=4.8.0
 fastcluster>=1.2.6
 pycirclize>=0.5.0
 plotly>=5.15.0
 cusingler
```

### Comparing `stereopy-1.2.0/tests/settings.py` & `stereopy-1.3.0b1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/tests/test_batch_integration.py` & `stereopy-1.3.0b1/tests/test_batch_integration.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/tests/test_cell_community_detection.py` & `stereopy-1.3.0b1/tests/test_cell_community_detection.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/tests/test_cell_cut.py` & `stereopy-1.3.0b1/tests/test_cell_cut.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/tests/test_clustering.py` & `stereopy-1.3.0b1/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/tests/test_h5ad_format.py` & `stereopy-1.3.0b1/tests/test_h5ad_format.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/tests/test_io.py` & `stereopy-1.3.0b1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/tests/test_io_h5ms.py` & `stereopy-1.3.0b1/tests/test_io_h5ms.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/tests/test_marker_genes.py` & `stereopy-1.3.0b1/tests/test_marker_genes.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/tests/test_merge_3d_data.py` & `stereopy-1.3.0b1/tests/test_merge_3d_data.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/tests/test_ms_data.py` & `stereopy-1.3.0b1/tests/test_ms_data.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/tests/test_plot_cluster_traj.py` & `stereopy-1.3.0b1/tests/test_plot_cluster_traj.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/tests/test_plot_vec.py` & `stereopy-1.3.0b1/tests/test_plot_vec.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/tests/test_regulatory_network_inference.py` & `stereopy-1.3.0b1/tests/test_regulatory_network_inference.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/tests/test_rna_velocity.py` & `stereopy-1.3.0b1/tests/test_rna_velocity.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/tests/test_sctransform.py` & `stereopy-1.3.0b1/tests/test_sctransform.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/tests/test_single_r.py` & `stereopy-1.3.0b1/tests/test_single_r.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/tests/test_spatial_hotspot.py` & `stereopy-1.3.0b1/tests/test_spatial_hotspot.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/tests/test_stereo_exp_data.py` & `stereopy-1.3.0b1/tests/test_stereo_exp_data.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/tests/test_time_series_analysis.py` & `stereopy-1.3.0b1/tests/test_time_series_analysis.py`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/tests/workflows_conf/environment_linux_gpu.yml` & `stereopy-1.3.0b1/tests/workflows_conf/environment_linux_gpu.yml`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/tests/workflows_conf/environment_linux_py38.yml` & `stereopy-1.3.0b1/tests/workflows_conf/environment_linux_py38.yml`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/tests/workflows_conf/environment_linux_py39.yml` & `stereopy-1.3.0b1/tests/workflows_conf/environment_linux_py39.yml`

 * *Files identical despite different names*

### Comparing `stereopy-1.2.0/tests/workflows_conf/environment_win.yml` & `stereopy-1.3.0b1/tests/workflows_conf/environment_win.yml`

 * *Files identical despite different names*

